Start
   ↓
Create SqlConnection
   ↓
Open Connection
   ↓
Execute SqlCommand
   ↓
+---------------------+
| Choose Reading Method|
+---------------------+
         ↓
   +---------------------+
   |   Option 1:        |
   | SqlDataReader      |
   +---------------------+
         ↓
 Execute SqlCommand
   ↓
 Read Data from SqlDataReader
   ↓
 Process Data
   ↓
 Close SqlDataReader
   ↓
 Close SqlConnection
         ↓
      End
         
   +---------------------+
   |   Option 2:        |
   | DataAdapter &      |
   | DataSet            |
   +---------------------+
         ↓
 Initialize SqlDataAdapter
   ↓
 Fill DataSet
   ↓
 Access & Manipulate DataSet
   ↓
 Update Database (if needed)
   ↓
 Close SqlConnection
         ↓
      End
