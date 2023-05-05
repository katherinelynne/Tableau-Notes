---


---

<h1 id="connecting-to-data"><span class="prefix"></span><span class="content">Connecting to Data</span><span class="suffix"></span></h1>
<h1 id="will-update-this-to-replace-it-with-my-personal-notes"><span class="prefix"></span><span class="content">Will update this to replace it with my personal notes</span><span class="suffix"></span></h1>
<p>Tableau has a lot of different ways to connect data, for example, your data could be stored on your local machine in a spreadsheet or a text file even. Others could include, big data, relational, cube (multideminsional) database on a server in your enterprise, public domain data available on the web such as U.S. Census Bureau information, or to a cloud database source such as Google Analytics, Amazon Redshift or Salesforce.</p>
<blockquote>
<p>a <strong>cube</strong> is a multidimensional database that contains dimensions and measures. It provides a single place where all related data, for analysis is stored. A multidimensional database is a type of database that is optimized for data warehouse and business intelligence (BI) applications. It organizes data into a multidimensional structure, where each dimension represents a different aspect of the data, such as time, location, or product.  i.e. Microsoft Analysis Services, Oracle Essbase, and SAP BW. <a href="https://databasetown.com/multidimensional-databases/#:~:text=This%20allows%20for%20faster%20and,Oracle%20Essbase,%20and%20SAP%20BW">What are multidimensional databases?</a></p>
</blockquote>
<p>Starting in 2019.3, Tableau Catalog is available as part of the Data Management offering for Tableau Server and Tableau Cloud. When Tableau Catalog is enabled in your environment, in addition to connecting to published data sources, you can connect to databases and tables from Tableau Server on the Connect pane in Tableau Desktop. For more information about Tableau Catalog, see “About Tableau Catalog” in the <a href="https://help.tableau.com/current/server/en-us/dm_catalog_overview.htm">Tableau Server</a> or <a href="https://help.tableau.com/current/online/en-us/dm_catalog_overview.htm">Tableau Cloud</a> Help. Starting in 2021.4, Data Management includes virtual connections, a central access point to data. For more information, see “About Virtual Connections and Data Policies” in the <a href="https://help.tableau.com/current/server/en-us/dm_vconn_overview.htm">Tableau Server(Link opens in a new window)</a> or <a href="https://help.tableau.com/current/online/en-us/dm_vconn_overview.htm">Tableau Cloud(Link opens in a new window)</a> help.</p>
<h2 id="tableau-desktop"><span class="prefix"></span><span class="content">Tableau Desktop</span><span class="suffix"></span></h2>
<p>When you launch Tableau Desktop, the data connectors that are available to you are listed on the <strong>Connect</strong> pane, which is the left pane on the <strong>Start</strong> page. Under Search for Data, select Tableau Server to find data using Tableau Server or Tableau Cloud. File types are listed next, then common server types, or servers that you’ve recently connected to. Click <strong>More</strong> to see the complete list of data connectors you can use.</p>
<p>For supported files and databases, Tableau provides native connectors that are built for and optimized for those types of data. If your file or database type is listed under Connect, use this native connector to connect to your data. If your file or database type is not listed, you might have the option of creating your own connection using Other Databases (JDBC), Other Databases (ODBC), a Web Data Connector, or a Connector Plugin built using the Tableau Connector SDK. Tableau provides limited support for connections that you create using these options.</p>
<p>The data connectors supported by your copy of Tableau Desktop are determined by the version you purchased. For more information, see the list of <a href="https://www.tableau.com/products/desktop#data-sources-professional">data connectors(Link opens in a new window)</a> on the Tableau website. After you’ve connected to data, you can save the connections to have them show up under the <strong>Saved data sources</strong> section on the <strong>Connect</strong> pane.</p>
<p>You supply different information for each data connection that you want to make. For example, for most data connections, you’ll need to supply a server name and your sign-in information. With some data connections, you can <a href="https://help.tableau.com/current/pro/desktop/en-us/connect_basic_initialsql.htm">Run Initial SQL</a> statements, and SSL-enabled servers require that you select the Require SSL check box when you connect. The following sections discuss the specific information you need to provide for each type of data you want to connect to.</p>
<p><strong>Tip:</strong> You can quickly create a data source in Tableau by copying and pasting data using the clipboard. For more information, see <a href="https://help.tableau.com/current/pro/desktop/en-us/clipboard_datasource.htm">Create a Data Source or Add a New Connection with Clipboard Data</a> .</p>
<h2 id="connecting-to-an-excel-workbook"><span class="prefix"></span><span class="content">Connecting to an Excel Workbook</span><span class="suffix"></span></h2>
<p>When you connect to an Excel workbook, the sheets associated with that workbook will appear in the left pane. When you drag a sheet to the right you are creating a Live connection to the data source.</p>
<ul>
<li>Tableau Public is on the cloud so we cant connect to an extract.</li>
</ul>
<h2 id="tableau-server-and-tableau-cloud-web-authoring"><span class="prefix"></span><span class="content">Tableau Server and Tableau Cloud web authoring</span><span class="suffix"></span></h2>
<p>Sign in to your Tableau site and select Create Workbook on the Home page to open the Connect to Data page. The tabs that you see on the page depend on the product you have.</p>
<ul>
<li><a href="https://help.tableau.com/current/pro/desktop/en-us/basicconnectoverview.htm#tableau-server">Tableau Server</a></li>
<li><a href="https://help.tableau.com/current/pro/desktop/en-us/basicconnectoverview.htm#tableau-cloud">Tableau Cloud</a></li>
</ul>
<p>On Tableau Server, select from the following tabs to connect to data:</p>
<ul>
<li><strong>On this site</strong>. Browse to or search for published data sources. If you have Data Management, you can also connect to data using a virtual connection. If you have Data Management with Tableau Catalog enabled, you can additionally connect to external assets like databases, files, and tables.</li>
<li><strong>Files</strong>. Upload Excel or text-based data sources (.xlsx, .csv, .tsv) directly in your browser.</li>
<li><strong>Connectors</strong>. Connect to data housed in a cloud database or on a server in your enterprise.</li>
</ul>
<p>For more information about connecting to data, see <a href="https://help.tableau.com/current/pro/desktop/en-us/creator_connect.htm">Creators: Connect to Data on the Web</a>.</p>
<p>The data connectors supported by your Tableau site are determined by your site’s server and your license level. For more information, see <a href="https://help.tableau.com/current/pro/desktop/en-us/web_author_overview.htm">What Can I Do with a Tableau Site?</a></p>
<p>After you’ve connected to data, you can save the connections to have them show up in the <strong>Data Sources</strong> section of your site.</p>
<h2 id="request-a-new-connector"><span class="prefix"></span><span class="content">Request a new connector</span><span class="suffix"></span></h2>
<p>If Tableau doesn’t have a native (built-in) connector for your data, consider requesting one on Tableau Community. Use <a href="https://community.tableau.com/community/ideas">Ideas(Link opens in a new window)</a> on Community to search for your connector to see if it’s been requested, and if it has been, vote for it. If it’s not listed, add it. Tableau regularly reviews Ideas on Community to help determine what features should be added to the product.</p>
<h2 id="other-articles-in-this-section"><span class="prefix"></span><span class="content">Other articles in this section</span><span class="suffix"></span></h2>
<ul>
<li><a href="https://help.tableau.com/current/pro/desktop/en-us/exampleconnections_overview.htm">Use Supported Connectors</a></li>
<li><a href="https://help.tableau.com/current/pro/desktop/en-us/gallery_connectors.htm">Use Partner-Built Connectors from the Extension Gallery</a></li>
<li><a href="https://help.tableau.com/current/pro/desktop/en-us/connect_customize.htm">Customize and Tune a Connection</a></li>
<li><a href="https://help.tableau.com/current/pro/desktop/en-us/connect_basic_initialsql.htm">Run Initial SQL</a></li>
</ul>

