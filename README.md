# Elasticsearch中文文档——基于v7.11

基于官方v7.11文档，翻译为中文，并发布在网站。

[在网站查看文档](https://docs.es.shiyueshuyi.xyz)

文档列表及完成进度：

- :heavy_check_mark: 什么是 Elasticsearch？ [:link:](https://docs.es.shiyueshuyi.xyz/#/es)
  - :heavy_check_mark: 数据输入：文档和索引 [:link:](https://docs.es.shiyueshuyi.xyz/#/intro/datain)
  - :heavy_check_mark: 信息输出：搜索和分析 [:link:](https://docs.es.shiyueshuyi.xyz/#/intro/inforout)
  - :heavy_check_mark: 可伸缩性和弹性 [:link:](https://docs.es.shiyueshuyi.xyz/#/intro/scalability)
- :heavy_check_mark: Elasticsearch 入门 [:link:](https://docs.es.shiyueshuyi.xyz/#/getting_started/getting_started)
  - :heavy_check_mark: 启动并运行 Elasticsearch [:link:](https://docs.es.shiyueshuyi.xyz/#/getting_started/install)
  - :heavy_check_mark: 索引一些文档 [:link:](https://docs.es.shiyueshuyi.xyz/#/getting_started/index)
  - :heavy_check_mark: 开始搜索 [:link:](https://docs.es.shiyueshuyi.xyz/#/getting_started/search)
  - :heavy_check_mark: 使用聚合分析结果  [:link:](https://docs.es.shiyueshuyi.xyz/#/getting_started/aggregations)
  - :heavy_check_mark: 何去何从 [:link:](https://docs.es.shiyueshuyi.xyz/#/getting_started/nextstep)
- :heavy_check_mark: 设置 Elasticsearch [:link:](https://docs.es.shiyueshuyi.xyz/#/setup/setup)
  - :heavy_check_mark: 安装 Elasticsearch [:link:](https://docs.es.shiyueshuyi.xyz/#/setup/install)
    - :heavy_check_mark: Linux 或 MacOS 上用存档安装 Elasticsearch [:link:](https://docs.es.shiyueshuyi.xyz/#/setup/install/linux)
    - :heavy_check_mark: 在 Windows 上用 `.zip` 安装 Elasticsearch [:link:](https://docs.es.shiyueshuyi.xyz/#/setup/install/windows)
    - :heavy_check_mark: 使用 Debian 包安装 Elasticsearch [:link:](https://docs.es.shiyueshuyi.xyz/#/setup/install/debian)
    - :heavy_check_mark: 使用 RPM 安装 Elasticsearch [:link:](https://docs.es.shiyueshuyi.xyz/#/setup/install/rpm)
    - :heavy_check_mark: 使用 Windows MSI 安装程序安装 Elasticsearch [:link:](https://docs.es.shiyueshuyi.xyz/#/setup/install/msi)
    - :heavy_check_mark: 使用 Docker 安装 Elasticsearch [:link:](https://docs.es.shiyueshuyi.xyz/#/setup/install/docker)
    - :heavy_check_mark: 使用 Homebrew 在 macOS 上安装 Elasticsearch [:link:](https://docs.es.shiyueshuyi.xyz/#/setup/install/brew)
  - Configuring Elasticsearch
    - Setting JVM options
    - Secure settings
    - Auditing settings
    - Circuit breaker settings
    - Cluster-level shard allocation and routing settings
    - Cross-cluster replication settings
    - Discovery and cluster formation settings
    - Field data cache settings
    - HTTP
    - Index lifecycle management settings
    - Index management settings
    - Index recovery settings
    - Indexing buffer settings
    - License settings
    - Local gateway settings
    - Logging
    - Machine learning settings
    - Monitoring settings
    - Node
    - Network settings
    - Node query cache settings
    - Search settings
    - Security settings
    - Shard request cache settings
    - Snapshot lifecycle management settings
    - Transforms settings
    - Transport
    - Thread pools
    - Watcher settings
    - Advanced configuration settings
  - Important Elasticsearch configuration
  - Important System Configuration
    - Configuring system settings
    - Disable swapping
    - File Descriptors
    - Virtual memory
    - Number of threads
    - DNS cache settings
    - JNA temporary directory not mounted with noexec
    - TCP retransmission timeout
  - Bootstrap Checks
    - Heap size check
    - File descriptor check
    - Memory lock check
    - Maximum number of threads check
    - Max file size check
    - Maximum size virtual memory check
    - Maximum map count check
    - Client JVM check
    - Use serial collector check
    - System call filter check
    - OnError and OnOutOfMemoryError checks
    - Early-access check
    - G1GC check
    - All permission check
    - Discovery configuration check
  - Bootstrap Checks for X-Pack
  - Starting Elasticsearch
  - Stopping Elasticsearch
  - Discovery and cluster formation
    - Discovery
    - Quorum-based decision making
    - Voting configurations
    - Bootstrapping a cluster
    - Publishing the cluster state
    - Cluster fault detection
  - Add and remove nodes in your cluster
  - Full-cluster restart and rolling restart
  - Remote clusters
  - Set up X-Pack
  - Configuring X-Pack Java Clients
  - Plugins
- Upgrade Elasticsearch
  - Rolling upgrades
  - Full cluster restart upgrade
  - Reindex before upgrading
    - Reindex in place
    - Reindex from a remote cluster
- :heavy_check_mark: 索引模块 [:link:](https://docs.es.shiyueshuyi.xyz/#/index_modules/index_modules)
  - :heavy_check_mark: 分析 [:link:](https://docs.es.shiyueshuyi.xyz/#/index_modules/analysis)
  - :heavy_check_mark: 索引分片分配 [:link:](https://docs.es.shiyueshuyi.xyz/#/index_modules/index_shard_allocation/index_shard_allocation)
    - :heavy_check_mark: 索引级分片分配过滤 [:link:](https://docs.es.shiyueshuyi.xyz/#/index_modules/index_shard_allocation/shard_allocation_filtering)
    - :heavy_check_mark: 当节点离开时延迟分配 [:link:](https://docs.es.shiyueshuyi.xyz/#/index_modules/index_shard_allocation/delaying_allocation)
    - :heavy_check_mark: 索引恢复优先级 [:link:](https://docs.es.shiyueshuyi.xyz/#/index_modules/index_shard_allocation/index_recovery_prioritization)
    - :heavy_check_mark: 每节点分片总数  [:link:](https://docs.es.shiyueshuyi.xyz/#/index_modules/index_shard_allocation/total_shards_per_node)
    - :heavy_check_mark: 索引级数据层分配过滤 [:link:](https://docs.es.shiyueshuyi.xyz/#/index_modules/index_shard_allocation/data_tier_allocation_filtering)
  - :heavy_check_mark: 索引块 [:link:](https://docs.es.shiyueshuyi.xyz/#/index_modules/index_blocks)
  - :heavy_check_mark: 映射器  [:link:](https://docs.es.shiyueshuyi.xyz/#/index_modules/mapper)
  - Merge
  - Similarity module
  - Slow Log
  - Store
    - Preloading data into the file system cache
  - Translog
  - History retention
  - Index Sorting
    - Use index sorting to speed up conjunctions
  - Indexing pressure
- Mapping
  - Dynamic mapping
    - Dynamic field mapping
    - Dynamic templates
  - Explicit mapping
  - Runtime fields
    - Map a runtime field
    - Define runtime fields in a search request
    - Override field values at query time
    - Retrieve a runtime field
    - Explore your data with runtime fields
  - Field data types
    - Aggregate metric
    - Alias
    - Arrays
    - Binary
    - Boolean
    - Date
    - Date nanoseconds
    - Dense vector
    - Flattened
    - Geo-point
    - Geo-shape
    - Histogram
    - IP
    - Join
    - Keyword
    - Nested
    - Numeric
    - Object
    - Percolator
    - Point
    - Range
    - Rank feature
    - Rank features
    - Search-as-you-type
    - Shape
    - Sparse vector
    - Text
    - Token count
    - Unsigned long
    - Version
  - Metadata fields
    - `_doc_count` field
    - `_field_names` field
    - `_ignored` field
    - `_id` field
    - `_index` field
    - `_meta` field
    - `_routing` field
    - `_source` field
    - `_type` field
  - Mapping parameters
    - `analyzer`
    - `boost`
    - `coerce`
    - `copy_to`
    - `doc_values`
    - `dynamic`
    - `eager_global_ordinals`
    - `enabled`
    - `format`
    - `ignore_above`
    - `ignore_malformed`
    - `index`
    - `index_options`
    - `index_phrases`
    - `index_prefixes`
    - `meta`
    - `fields`
    - `normalizer`
    - `norms`
    - `null_value`
    - `position_increment_gap`
    - `properties`
    - `search_analyzer`
    - `similarity`
    - `store`
    - `term_vector`
  - Mapping limit settings
  - Removal of mapping types
- Text analysis
  - Overview
  - Concepts
    - Anatomy of an analyzer
    - Index and search analysis
    - Stemming
    - Token graphs
  - Configure text analysis
    - Test an analyzer
    - Configuring built-in analyzers
    - Create a custom analyzer
    - Specify an analyzer
  - Built-in analyzer reference
    - Fingerprint
    - Keyword
    - Language
    - Pattern
    - Simple
    - Standard
    - Stop
    - Whitespace
  - Tokenizer reference
    - Character group
    - Classic
    - Edge n-gram
    - Keyword
    - Letter
    - Lowercase
    - N-gram
    - Path hierarchy
    - Pattern
    - Simple pattern
    - Simple pattern split
    - Standard
    - Thai
    - UAX URL email
    - Whitespace
  - Token filter reference
    - Apostrophe
    - ASCII folding
    - CJK bigram
    - CJK width
    - Classic
    - Common grams
    - Conditional
    - Decimal digit
    - Delimited payload
    - Dictionary decompounder
    - Edge n-gram
    - Elision
    - Fingerprint
    - Flatten graph
    - Hunspell
    - Hyphenation decompounder
    - Keep types
    - Keep words
    - Keyword marker
    - Keyword repeat
    - KStem
    - Length
    - Limit token count
    - Lowercase
    - MinHash
    - Multiplexer
    - N-gram
    - Normalization
    - Pattern capture
    - Pattern replace
    - Phonetic
    - Porter stem
    - Predicate script
    - Remove duplicates
    - Reverse
    - Shingle
    - Snowball
    - Stemmer
    - Stemmer override
    - Stop
    - Synonym
    - Synonym graph
    - Trim
    - Truncate
    - Unique
    - Uppercase
    - Word delimiter
    - Word delimiter graph
  - Character filters reference
    - HTML strip
    - Mapping
    - Pattern replace
  - Normalizers
- Index templates
  - Simulate multi-component templates
- Data streams
  - Set up a data stream
  - Use a data stream
  - Change mappings and settings for a data stream
- Ingest node
  - Pipeline Definition
  - Accessing Data in Pipelines
  - Conditional Execution in Pipelines
    - Handling Nested Fields in Conditionals
    - Complex Conditionals
    - Conditionals with the Pipeline Processor
    - Conditionals with the Regular Expressions
  - Handling Failures in Pipelines
  - Enrich your data
    - Set up an enrich processor
    - Enrich policy definition
    - Example: Enrich your data based on geolocation
    - Example: Enrich your data based on exact values
  - Processors
    - Append
    - Bytes
    - Circle
    - Convert
    - CSV
    - Date
    - Date index name
    - Dissect
    - Dot expander
    - Drop
    - Enrich
    - Fail
    - Foreach
    - GeoIP
    - Grok
    - Gsub
    - HTML strip
    - Inference
    - Join
    - JSON
    - KV
    - Lowercase
    - Pipeline
    - Remove
    - Rename
    - Script
    - Set
    - Set security user
    - Sort
    - Split
    - Trim
    - Uppercase
    - URL decode
    - User agent
- Search your data
  - Collapse search results
  - Filter search results
  - Highlighting
  - Long-running searches
  - Near real-time search
  - Paginate search results
  - Retrieve inner hits
  - Retrieve selected fields
  - Search across clusters
  - Search multiple data streams and indices
  - Search shard routing
  - Sort search results
- Query DSL
  - Query and filter context
  - Compound queries
    - Boolean
    - Boosting
    - Constant score
    - Disjunction max
    - Function score
  - Full text queries
    - Intervals
    - Match
    - Match boolean prefix
    - Match phrase
    - Match phrase prefix
    - Multi-match
    - Common Terms Query
    - Query string
    - Simple query string
  - Geo queries
    - Geo-bounding box
    - Geo-distance
    - Geo-polygon
    - Geo-shape
  - Shape queries
    - Shape
  - Joining queries
    - Nested
    - Has child
    - Has parent
    - Parent ID
  - Match all
  - Span queries
    - Span containing
    - Span field masking
    - Span first
    - Span multi-term
    - Span near
    - Span not
    - Span or
    - Span term
    - Span within
  - Specialized queries
    - Distance feature
    - More like this
    - Percolate
    - Rank feature
    - Script
    - Script score
    - Wrapper
    - Pinned Query
  - Term-level queries
    - Exists
    - Fuzzy
    - IDs
    - Prefix
    - Range
    - Regexp
    - Term
    - Terms
    - Terms set
    - Type Query
    - Wildcard
  - minimum_should_match parameter
  - rewrite parameter
  - Regular expression syntax
- Aggregations
  - Bucket aggregations
    - Adjacency matrix
    - Auto-interval date histogram
    - Children
    - Composite
    - Date histogram
    - Date range
    - Diversified sampler
    - Filter
    - Filters
    - Geo-distance
    - Geohash grid
    - Geotile grid
    - Global
    - Histogram
    - IP range
    - Missing
    - Nested
    - Parent
    - Range
    - Rare terms
    - Reverse nested
    - Sampler
    - Significant terms
    - Significant text
    - Terms
    - Variable width histogram
    - Subtleties of bucketing range fields
  - Metrics aggregations
    - Avg
    - Boxplot
    - Cardinality
    - Extended stats
    - Geo-bounds
    - Geo-centroid
    - Geo-Line
    - Matrix stats
    - Max
    - Median absolute deviation
    - Min
    - Percentile ranks
    - Percentiles
    - Rate
    - Scripted metric
    - Stats
    - String stats
    - Sum
    - T-test
    - Top hits
    - Top metrics
    - Value count
    - Weighted avg
  - Pipeline aggregations
    - Avg bucket
    - Bucket script
    - Bucket selector
    - Bucket sort
    - Cumulative cardinality
    - Cumulative sum
    - Derivative
    - Extended stats bucket
    - Inference bucket
    - Max bucket
    - Min bucket
    - Moving average
    - Moving function
    - Moving percentiles
    - Normalize
    - Percentiles bucket
    - Serial differencing
    - Stats bucket
    - Sum bucket
- EQL
  - Syntax reference
  - Function reference
  - Pipe reference
  - Example: Detect threats with EQL
- SQL access
  - Overview
  - Getting Started with SQL
  - Conventions and Terminology
    - Mapping concepts across SQL and Elasticsearch
  - Security
  - SQL REST API
    - Overview
    - Response Data Formats
    - Paginating through a large response
    - Filtering using Elasticsearch Query DSL
    - Columnar results
    - Passing parameters to a query
    - Supported REST parameters
  - SQL Translate API
  - SQL CLI
  - SQL JDBC
    - API usage
  - SQL ODBC
    - Driver installation
    - Configuration
  - SQL Client Applications
    - DBeaver
    - DbVisualizer
    - Microsoft Excel
    - Microsoft Power BI Desktop
    - Microsoft PowerShell
    - MicroStrategy Desktop
    - Qlik Sense Desktop
    - SQuirreL SQL
    - SQL Workbench/J
    - Tableau Desktop
  - SQL Language
    - Lexical Structure
    - SQL Commands
    - DESCRIBE TABLE
    - SELECT
    - SHOW COLUMNS
    - SHOW FUNCTIONS
    - SHOW TABLES
    - Data Types
    - Index patterns
    - Frozen Indices
  - Functions and Operators
    - Comparison Operators
    - Logical Operators
    - Math Operators
    - Cast Operators
    - LIKE and RLIKE Operators
    - Aggregate Functions
    - Grouping Functions
    - Date/Time and Interval Functions and Operators
    - Full-Text Search Functions
    - Mathematical Functions
    - String Functions
    - Type Conversion Functions
    - Geo Functions
    - Conditional Functions And Expressions
    - System Functions
  - Reserved keywords
  - SQL Limitations
- Scripting
  - How to use scripts
    - Scripts and search speed
  - Accessing document fields and special variables
  - Scripting and security
  - Painless scripting language
  - Lucene expressions language
  - Advanced scripts using script engines
- Data management
  - Data tiers
  - Index management
- ILM: Manage the index lifecycle
  - Overview
  - Concepts
    - Index lifecycle
    - Rollover
    - Policy updates
  - Automate rollover
  - Customize built-in ILM policies
  - Index lifecycle actions
    - Allocate
    - Delete
    - Force merge
    - Freeze
    - Migrate
    - Read only
    - Rollover
    - Searchable snapshot
    - Set priority
    - Shrink
    - Unfollow
    - Wait for snapshot
  - Configure a lifecycle policy
  - Resolve lifecycle policy execution errors
  - Start and stop index lifecycle management
  - Manage existing indices
  - Skip rollover
  - Restore a managed data stream or index
- Autoscaling
  - Autoscaling deciders
    - Reactive storage decider
    - Proactive storage decider
    - Machine learning decider
    - Fixed decider
- Monitor a cluster
  - Overview
  - How it works
  - Monitoring in a production environment
  - Collecting monitoring data with Metricbeat
  - Collecting log data with Filebeat
  - Configuring indices for monitoring
  - Legacy collection methods
    - Collectors
    - Exporters
    - Local exporters
    - HTTP exporters
    - Pausing data collection
  - Troubleshooting
- Frozen indices
  - Best practices
  - Searching a frozen index
  - Monitoring frozen indices
- Roll up or transform your data
  - Rolling up historical data
    - Overview
    - API quick reference
    - Getting started
    - Understanding groups
    - Rollup aggregation limitations
    - Rollup search limitations
  - Transforming data
    - Overview
    - Setup
    - When to use transforms
    - Transforms at scale
    - How checkpoints work
    - API quick reference
    - Tutorial: Transforming the eCommerce sample data
    - Examples
    - Painless examples
    - Troubleshooting
    - Limitations
- Set up a cluster for high availability
  - Designing for resilience
    - Resilience in small clusters
    - Resilience in larger clusters
  - Back up a cluster
    - Back up the data
    - Back up the cluster configuration
    - Back up the security configuration
    - Restore the security configuration
    - Restore the data
  - Cross-cluster replication
    - Set up cross-cluster replication
    - Manage cross-cluster replication
    - Manage auto-follow patterns
    - Upgrading clusters
- Snapshot and restore
  - Register repository
  - Create a snapshot
  - Restore a snapshot
  - Monitor snapshot and restore
  - Delete a snapshot
  - SLM: Manage the snapshot lifecycle
    - Tutorial: Automate backups with SLM
    - Security and SLM
    - Snapshot retention
  - Searchable snapshots
- Secure a cluster
  - Overview
  - Configuring security
  - User authentication
  - Configuring SAML single-sign-on on the Elastic Stack
  - Configuring single sign-on to the Elastic Stack using OpenID Connect
  - User authorization
  - Enabling audit logging
  - Encrypting communications
  - Restricting connections with IP filtering
  - Cross cluster search, clients, and integrations
  - Tutorial: Getting started with security
  - Tutorial: Encrypting communications
  - Troubleshooting
  - Limitations
- Watch for cluster and index events
  - Getting started with Watcher
  - How Watcher works
  - Encrypting sensitive data in Watcher
  - Inputs
    - Simple input
    - Search input
    - HTTP input
    - Chain input
  - Triggers
    - Schedule trigger
  - Conditions
    - Always condition
    - Never condition
    - Compare condition
    - Array compare condition
    - Script condition
  - Actions
    - Running an action for each element in an array
    - Adding conditions to actions
    - Email action
    - Webhook action
    - Index action
    - Logging action
    - Slack action
    - PagerDuty action
    - Jira action
  - Transforms
    - Search payload transform
    - Script payload transform
    - Chain payload transform
  - Java API
  - Managing watches
  - Example watches
    - Watching the status of an Elasticsearch cluster
    - Watching event data
  - Troubleshooting
  - Limitations
- Command line tools
  - elasticsearch-certgen
  - elasticsearch-certutil
  - elasticsearch-croneval
  - elasticsearch-keystore
  - elasticsearch-migrate
  - elasticsearch-node
  - elasticsearch-saml-metadata
  - elasticsearch-setup-passwords
  - elasticsearch-shard
  - elasticsearch-syskeygen
  - elasticsearch-users
- How To
  - General recommendations
  - Recipes
  - Tune for indexing speed
  - Tune for search speed
  - Tune for disk usage
  - Size your shards
- Glossary of terms
- :heavy_check_mark: REST API [:link:](https://docs.es.shiyueshuyi.xyz/#/rest_apis/rest_apis)
  - :heavy_check_mark: API 约定 [:link:](https://docs.es.shiyueshuyi.xyz/#/rest_apis/api_convention/api_convention)
    - :heavy_check_mark: 多目标语法 [:link:](https://docs.es.shiyueshuyi.xyz/#/rest_apis/api_convention/multi_target_syntax)
    - :heavy_check_mark: 索引名中的日期数学支持 [:link:](https://docs.es.shiyueshuyi.xyz/#/rest_apis/api_convention/date_math_support_in_index_names)
    - :heavy_check_mark: Cron 表达式 [:link:](https://docs.es.shiyueshuyi.xyz/#/rest_apis/api_convention/cron_expressions)
    - :heavy_check_mark: 常用选项 [:link:](https://docs.es.shiyueshuyi.xyz/#/rest_apis/api_convention/common_options)
    - :heavy_check_mark: 基于 URL 的访问控制 [:link:](https://docs.es.shiyueshuyi.xyz/#/rest_apis/api_convention/url-based_access_control)
  - Autoscaling APIs
    - Get autoscaling capacity
    - Delete autoscaling policy
    - Get autoscaling policy
    - Put autoscaling policy
  - Compact and aligned text (CAT) APIs
    - cat aliases
    - cat allocation
    - cat anomaly detectors
    - cat count
    - cat data frame analytics
    - cat datafeeds
    - cat fielddata
    - cat health
    - cat indices
    - cat master
    - cat nodeattrs
    - cat nodes
    - cat pending tasks
    - cat plugins
    - cat recovery
    - cat repositories
    - cat segments
    - cat shards
    - cat snapshots
    - cat task management
    - cat templates
    - cat thread pool
    - cat trained model
    - cat transforms
  - Cluster APIs
    - Cluster allocation explain
    - Cluster get settings
    - Cluster health
    - Cluster reroute
    - Cluster state
    - Cluster stats
    - Cluster update settings
    - Nodes feature usage
    - Nodes hot threads
    - Nodes info
    - Nodes reload secure settings
    - Nodes stats
    - Pending cluster tasks
    - Remote cluster info
    - Task management
    - Voting configuration exclusions
  - Cross-cluster replication APIs
    - Get CCR stats
    - Create follower
    - Pause follower
    - Resume follower
    - Unfollow
    - Forget follower
    - Get follower stats
    - Get follower info
    - Create auto-follow pattern
    - Delete auto-follow pattern
    - Get auto-follow pattern
    - Pause auto-follow pattern
    - Resume auto-follow pattern
  - Data stream APIs
    - Create data stream
    - Delete data stream
    - Get data stream
    - Migrate to data stream
    - Data stream stats
    - Promote data stream
  - Document APIs
    - Reading and Writing documents
    - Index
    - Get
    - Delete
    - Delete by query
    - Update
    - Update by query
    - Multi get
    - Bulk
    - Reindex
    - Term vectors
    - Multi term vectors
    - ?refresh
    - Optimistic concurrency control
  - Enrich APIs
    - Put enrich policy
    - Delete enrich policy
    - Get enrich policy
    - Execute enrich policy
    - Enrich stats
  - Graph explore API
  - :heavy_check_mark: 索引 API [:link:](https://docs.es.shiyueshuyi.xyz/#/rest_apis/index_apis/index_apis)
    - Add index alias
    - Analyze
    - Clear cache
    - :heavy_check_mark: 复制索引 [:link:](https://docs.es.shiyueshuyi.xyz/#/rest_apis/index_apis/clone_index)
    - :heavy_check_mark: 关闭索引 [:link:](https://docs.es.shiyueshuyi.xyz/#/rest_apis/index_apis/close_index)
    - :heavy_check_mark: 创建索引 [:link:](https://docs.es.shiyueshuyi.xyz/#/rest_apis/index_apis/create_index)
    - :heavy_check_mark: 删除索引 [:link:](https://docs.es.shiyueshuyi.xyz/#/rest_apis/index_apis/delete_index)
    - Delete index alias
    - Delete component template
    - Delete index template
    - Delete index template (legacy)
    - Flush
    - Force merge
    - :heavy_check_mark: 冻结索引 [:link:](https://docs.es.shiyueshuyi.xyz/#/rest_apis/index_apis/freeze_index)
    - Get component template
    - Get field mapping
    - :heavy_check_mark: 获取索引 [:link:](https://docs.es.shiyueshuyi.xyz/#/rest_apis/index_apis/get_index)
    - Get index alias
    - Get index settings
    - Get index template
    - Get index template (legacy)
    - Get mapping
    - Index alias exists
    - :heavy_check_mark: 索引存在 [:link:](https://docs.es.shiyueshuyi.xyz/#/rest_apis/index_apis/index_exists)
    - Index recovery
    - Index segments
    - Index shard stores
    - Index stats
    - Index template exists (legacy)
    - :heavy_check_mark: 开启索引 [:link:](https://docs.es.shiyueshuyi.xyz/#/rest_apis/index_apis/open_index)
    - Put index template
    - Put index template (legacy)
    - Put component template
    - Put mapping
    - Refresh
    - :heavy_check_mark: 解析索引 [:link:](https://docs.es.shiyueshuyi.xyz/#/rest_apis/index_apis/resolve_index)
    - :heavy_check_mark: 翻转索引 [:link:](https://docs.es.shiyueshuyi.xyz/#/rest_apis/index_apis/rollover_index)
    - :heavy_check_mark: 收缩索引 [:link:](https://docs.es.shiyueshuyi.xyz/#/rest_apis/index_apis/shrink_index)
    - Simulate index
    - Simulate template
    - :heavy_check_mark: 拆分索引 [:link:](https://docs.es.shiyueshuyi.xyz/#/rest_apis/index_apis/split_index)
    - Synced flush
    - Type exists
    - :heavy_check_mark: 解冻索引 [:link:](https://docs.es.shiyueshuyi.xyz/#/rest_apis/index_apis/unfreeze_index)
    - Update index settings
    - :heavy_check_mark: 更新映射 [:link:](https://docs.es.shiyueshuyi.xyz/#/rest_apis/index_apis/update_mapping)
  - Index lifecycle management APIs
    - Create policy
    - Get policy
    - Delete policy
    - Move to step
    - Remove policy
    - Retry policy
    - Get index lifecycle management status
    - Explain lifecycle
    - Start index lifecycle management
    - Stop index lifecycle management
  - Ingest APIs
    - Put pipeline
    - Get pipeline
    - Delete pipeline
    - Simulate pipeline
  - Info API
  - Licensing APIs
    - Delete license
    - Get license
    - Get trial status
    - Start trial
    - Get basic status
    - Start basic
    - Update license
  - Machine learning anomaly detection APIs
    - Add events to calendar
    - Add jobs to calendar
    - Close jobs
    - Create jobs
    - Create calendars
    - Create datafeeds
    - Create filters
    - Delete calendars
    - Delete datafeeds
    - Delete events from calendar
    - Delete filters
    - Delete forecasts
    - Delete jobs
    - Delete jobs from calendar
    - Delete model snapshots
    - Delete expired data
    - Estimate model memory
    - Find file structure
    - Flush jobs
    - Forecast jobs
    - Get buckets
    - Get calendars
    - Get categories
    - Get datafeeds
    - Get datafeed statistics
    - Get influencers
    - Get jobs
    - Get job statistics
    - Get machine learning info
    - Get model snapshots
    - Get overall buckets
    - Get scheduled events
    - Get filters
    - Get records
    - Open jobs
    - Post data to jobs
    - Preview datafeeds
    - Revert model snapshots
    - Set upgrade mode
    - Start datafeeds
    - Stop datafeeds
    - Update datafeeds
    - Update filters
    - Update jobs
    - Update model snapshots
    - Upgrade model snapshots
  - Machine learning data frame analytics APIs
    - Create data frame analytics jobs
    - Create trained models
    - Update data frame analytics jobs
    - Delete data frame analytics jobs
    - Delete trained models
    - Evaluate data frame analytics
    - Explain data frame analytics
    - Get data frame analytics jobs
    - Get data frame analytics jobs stats
    - Get trained models
    - Get trained models stats
    - Start data frame analytics jobs
    - Stop data frame analytics jobs
  - Migration APIs
    - Deprecation info
  - Reload search analyzers API
  - Repositories metering APIs
    - Get repositories metering information
    - Clear repositories metering archive
  - Rollup APIs
    - Create rollup jobs
    - Delete rollup jobs
    - Get job
    - Get rollup caps
    - Get rollup index caps
    - Rollup search
    - Start rollup jobs
    - Stop rollup jobs
  - Search APIs
    - Search
    - Async search
    - Point in time
    - Scroll
    - Clear scroll
    - Search template
    - Multi search template
    - Search shards
    - Suggesters
    - Multi search
    - EQL search
    - Get async EQL search
    - Delete async EQL search
    - Count
    - Validate
    - Explain
    - Profile
    - Field capabilities
    - Ranking evaluation
  - Searchable snapshots APIs
    - Mount snapshot
  - Security APIs
    - Authenticate
    - Change passwords
    - Clear cache
    - Clear roles cache
    - Clear privileges cache
    - Clear API key cache
    - Create API keys
    - Create or update application privileges
    - Create or update role mappings
    - Create or update roles
    - Create or update users
    - Delegate PKI authentication
    - Delete application privileges
    - Delete role mappings
    - Delete roles
    - Delete users
    - Disable users
    - Enable users
    - Get API key information
    - Get application privileges
    - Get builtin privileges
    - Get role mappings
    - Get roles
    - Get token
    - Get users
    - Grant API keys
    - Has privileges
    - Invalidate API key
    - Invalidate token
    - OpenID Connect prepare authentication
    - OpenID Connect authenticate
    - OpenID Connect logout
    - SAML prepare authentication
    - SAML authenticate
    - SAML logout
    - SAML invalidate
    - SAML service provider metadata
    - SSL certificate
  - Snapshot and restore APIs
    - Put snapshot repository
    - Verify snapshot repository
    - Get snapshot repository
    - Delete snapshot repository
    - Clean up snapshot repository
    - Clone snapshot
    - Create snapshot
    - Get snapshot
    - Get snapshot status
    - Restore snapshot
    - Delete snapshot
  - Snapshot lifecycle management APIs
    - Put policy
    - Get policy
    - Delete policy
    - Execute snapshot lifecycle policy
    - Execute snapshot retention policy
    - Get snapshot lifecycle management status
    - Get snapshot lifecycle stats
    - Start snapshot lifecycle management
    - Stop snapshot lifecycle management
  - Transform APIs
    - Create transform
    - Delete transform
    - Get transforms
    - Get transform statistics
    - Preview transform
    - Start transform
    - Stop transforms
    - Update transform
  - Usage API
  - Watcher APIs
    - Ack watch
    - Activate watch
    - Deactivate watch
    - Delete watch
    - Execute watch
    - Get watch
    - Get Watcher stats
    - Query watches
    - Put watch
    - Start watch service
    - Stop watch service
  - Definitions
    - Role mapping resources
  - Migration guide
  - Dependencies and versions
