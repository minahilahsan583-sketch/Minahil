---
layout: single
title: "Portfolio & Gallery"
permalink: /portfolio/
author_profile: true
header:
  overlay_image: https://images.unsplash.com/photo-1518770660439-4636190af475?q=80&w=2070&auto=format&fit=crop
  overlay_filter: 0.5
---

# Technical Gallery

A visually-driven display of my technical work, code samples, and campus activities.

---

### UI/UX Design Concepts
I explore modern UI/UX principles to ensure that my engineering solutions are user-friendly and aesthetically pleasing.

![Web UI Design]({{ '/assets/images/project_3_web.png' | relative_url }})

---

### Python Data Analysis Snippet
Here is a sample of how I structure data cleaning and preparation using the powerful Pandas library.

```python
import pandas as pd

# Load dataset
df = pd.read_csv('kidney_disease_data.csv')

# Handling missing values
df.fillna(df.mean(), inplace=True)

# Normalizing data
from sklearn.preprocessing import StandardScaler
scaler = StandardScaler()
df_scaled = scaler.fit_transform(df)
```

---

### C++ MySQL Integration
Example of how I integrate a C++ frontend with a MySQL backend for student records.

```cpp
#include <mysql_driver.h>
#include <mysql_connection.h>

void connectDB() {
    sql::mysql::MySQL_Driver *driver;
    sql::Connection *con;

    driver = sql::mysql::get_mysql_driver_instance();
    con = driver->connect("tcp://127.0.0.1:3306", "minahil", "secure_pass");
}
```

---

### Technical Exhibition 2026
Memories from out first big showcase under the mentorship of **Dr. Bilal**.

<div class="gallery">
  <figure>
    <img src="{{ '/assets/images/minahil_lab_1.png' | relative_url }}" alt="Lab Setup">
    <figcaption>Preparing for the exhibition in the engineering lab.</figcaption>
  </figure>
  <figure>
    <img src="{{ '/assets/images/kidney_project_1.png' | relative_url }}" alt="Project Display">
    <figcaption>Displaying our Kidney Disease Prediction System.</figcaption>
  </figure>
  <figure>
    <img src="{{ '/assets/images/minahil_intro_1.png' | relative_url }}" alt="Team Spirit">
    <figcaption>Collaborating with peers on campus.</figcaption>
  </figure>
</div>

---

> [!NOTE]
> All work samples and code displayed here are regularly updated with my latest achievements.
