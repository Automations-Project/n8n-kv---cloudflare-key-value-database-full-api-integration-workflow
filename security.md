For Security Reasons we will summuray the n8n template code into text as follow:
**Workflow Summary:**
**Additional Processing:**
- **Set KV-NM Name (8)** (n8n-nodes-base.set)
  Details:
    - **Notes**: ```plaintext
Set Key-Value Namespace``` 
- **Set KV-NM Name (7)** (n8n-nodes-base.set)
**Data Fetching and Processing:**
- **List KV-NMs (10)** (n8n-nodes-base.httpRequest)
  Details:
    - **Notes**: ```plaintext
Get Available Namespaces``` 
- **List KV-NMs (9)** (n8n-nodes-base.httpRequest)
  Details:
    - **Notes**: ```plaintext
Get Available Namespaces``` 
- **List KV-NMs (8)** (n8n-nodes-base.httpRequest)
  Details:
    - **Notes**: ```plaintext
Get Available Namespaces``` 
- **Read MD from Key** (n8n-nodes-base.httpRequest)
  Details:
    - **Notes**: ```plaintext
/storage/kv/namespaces/``` 

**Additional Processing:**
- **Set KV-NM Name (6)** (n8n-nodes-base.set)
  Details:
    - **Notes**: ```plaintext
Set Key-Value Namespace``` 

**Data Fetching and Processing:**
- **List KV-NMs (7)** (n8n-nodes-base.httpRequest)
  Details:
    - **Notes**: ```plaintext
Get Available Namespaces``` 

**Additional Processing:**
- **Set KV-NM Name (5)** (n8n-nodes-base.set)
**Data Fetching and Processing:**
- **List KV-NMs (6)** (n8n-nodes-base.httpRequest)
  Details:
    - **Notes**: ```plaintext
Get Available Namespaces``` 

**Additional Processing:**
- **Set KV-NM Name (4)** (n8n-nodes-base.set)
  Details:
    - **Notes**: ```plaintext
Set Key-Value Namespace for kv``` 

**Data Fetching and Processing:**
- **List KV-NMs (4)** (n8n-nodes-base.httpRequest)
  Details:
    - **Notes**: ```plaintext
Get Available Namespaces``` 
- **Write V & MD of KV In NM** (n8n-nodes-base.httpRequest)
  Details:
    - **Notes**: ```plaintext
Put value with Metadata to NM key``` 

**Additional Processing:**
- **Set KV-NM Name (3)** (n8n-nodes-base.set)
  Details:
    - **Notes**: ```plaintext
Set Key-Value Namespace for Deleting``` 

**Data Fetching and Processing:**
- **List KV-NMs (3)** (n8n-nodes-base.httpRequest)
  Details:
    - **Notes**: ```plaintext
Get Available Namespaces``` 

**Additional Processing:**
- **Set KV-NM Name (1)** (n8n-nodes-base.set)
  Details:
    - **Notes**: ```plaintext
Set Key-Value Namespace for deleting``` 
- **Set KV-NM Name (2)** (n8n-nodes-base.set)
  Details:
    - **Notes**: ```plaintext
Set Key-Value Namespace for deleting``` 

**Data Fetching and Processing:**
- **List KV-NMs (2)** (n8n-nodes-base.httpRequest)
  Details:
    - **Notes**: ```plaintext
Get Available Namespaces``` 
- **List KV-NMs (1)** (n8n-nodes-base.httpRequest)
  Details:
    - **Notes**: ```plaintext
Get Available Namespaces``` 

**Additional Processing:**
- **Manual Trigger** (n8n-nodes-base.manualTrigger)
  Details:
    - **Notes**: ```plaintext
Replace Me``` 
- **Sticky Note15** (n8n-nodes-base.stickyNote)
  Details:
    - **Content**:
```plaintext
## This n8n template provides a seamless and efficient way to manage Key-Value (KV) pairs in Cloudflare's KV storage. all you need just take the part of action you want then use it with your workflow, keep in mind that the **_`Account Path`_** node is required for all actions as it's used to set the path of account, other authentication values is automatically set by n8n pre configured cloudflare api.
 ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌  ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌  ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌  ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌  ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌   ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌  ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌  ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌  ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌  ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌   ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌  ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌  ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌  ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌  ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌  ![Cloudflare Logo](https://cf-assets.www.cloudflare.com/slt3lc6tev37/7bIgGp4hk4SFO0o3SBbOKJ/546b2df59d9ef1ac226d70c40b17d019/Cloudflare-logo-transparent-v-rgb_thumbnail.png)

# shortcuts:
- ## **`NM`** or **`NMs`** =  _**`NameSpace/s`**_
- ## **`KV`** or **`KVs`** = _**`Key/s - Value/s`**_
- ## **`MD`** = _**`MetaData`**_
``` 
- **Sticky Note14** (n8n-nodes-base.stickyNote)
  Details:
    - **Content**:
```plaintext
##     ‌ ‌‌‌‌ ‌ ‌ ‌  ‌‌‌‌ ‌ ‌‌‌‌ ‌ ‌ ‌  ‌ ‌ Single Actions
``` 
- **Sticky Note13** (n8n-nodes-base.stickyNote)
  Details:
    - **Content**:
```plaintext
##     ‌ ‌‌‌‌ ‌ ‌ ‌ Specific Actions
``` 
- **Sticky Note12** (n8n-nodes-base.stickyNote)
  Details:
    - **Content**:
```plaintext
## Write KV
to change anything read [Docs](https://developers.cloudflare.com/api/operations/workers-kv-namespace-write-key-value-pair-with-metadata)
``` 

**Data Fetching and Processing:**
- **Read Value Of KV In NM** (n8n-nodes-base.httpRequest)
  Details:
    - **Notes**: ```plaintext
/storage/kv/namespaces/``` 

**Additional Processing:**
- **Sticky Note11** (n8n-nodes-base.stickyNote)
  Details:
    - **Content**:
```plaintext
## Read KV
to change anything read [Docs](https://developers.cloudflare.com/api/operations/workers-kv-namespace-read-key-value-pair)
``` 

**Data Fetching and Processing:**
- **Delete KV inside NM** (n8n-nodes-base.httpRequest)
  Details:
    - **Notes**: ```plaintext
Delete selected KV in NM``` 

**Additional Processing:**
- **Sticky Note10** (n8n-nodes-base.stickyNote)
  Details:
    - **Content**:
```plaintext
## Delete KV
to change anything read [Docs](https://developers.cloudflare.com/api/operations/workers-kv-namespace-delete-key-value-pair)
``` 
- **Sticky Note9** (n8n-nodes-base.stickyNote)
  Details:
    - **Content**:
```plaintext
## Read MD in spesific key
to change anything read [Docs](https://developers.cloudflare.com/api/operations/workers-kv-namespace-read-the-metadata-for-a-key)
``` 
- **Sticky Note8** (n8n-nodes-base.stickyNote)
  Details:
    - **Content**:
```plaintext
##     ‌ ‌‌‌‌ ‌ ‌ ‌ ‌‌‌‌ ‌   Bulk Actions
``` 

**Data Fetching and Processing:**
- **-Get Keys inside NM** (n8n-nodes-base.httpRequest)
  Details:
    - **Notes**: ```plaintext
Get Available Keys``` 

**Additional Processing:**
- **Sticky Note7** (n8n-nodes-base.stickyNote)
  Details:
    - **Content**:
```plaintext
## List NM-Keys
to change anything read [Docs](https://developers.cloudflare.com/api/operations/workers-kv-namespace-list-a-namespace'-s-keys)
``` 

**Data Fetching and Processing:**
- **Write KVs inside NM** (n8n-nodes-base.httpRequest)
  Details:
    - **Notes**: ```plaintext
/storage/kv/namespaces/``` 

**Additional Processing:**
- **Sticky Note6** (n8n-nodes-base.stickyNote)
  Details:
    - **Content**:
```plaintext
## Write multiple KV pairs
to change anything read [Docs](https://developers.cloudflare.com/api/operations/workers-kv-namespace-write-multiple-key-value-pairs)
``` 

**Data Fetching and Processing:**
- **Delete KVs inside NM** (n8n-nodes-base.httpRequest)
  Details:
    - **Notes**: ```plaintext
Delete bulk Keys-Values inside select Namespace``` 

**Additional Processing:**
- **Sticky Note5** (n8n-nodes-base.stickyNote)
  Details:
    - **Content**:
```plaintext
#  ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ **`Cloudflare Key-Value Full API integration Workflow`**
[![Hetzner Cloud](https://developers.cloudflare.com/assets/kv-write-fdb5578b.svg)](https://www.hetzner.com/cloud)
##  ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ _Integrate your N8N with CF KV Free instead of selfhosting Redis or any RAM based Storages!!_
``` 
- **Sticky Note4** (n8n-nodes-base.stickyNote)
  Details:
    - **Content**:
```plaintext
## Delete multiple KV pairs
to change anything read [Docs](https://developers.cloudflare.com/api/operations/workers-kv-namespace-delete-multiple-key-value-pairs)
``` 
- **Account Path** (n8n-nodes-base.set)
  Details:
    - **Notes**: ```plaintext
Required for all nodes``` 

**Data Fetching and Processing:**
- **Create KV-NM** (n8n-nodes-base.httpRequest)
  Details:
    - **Notes**: ```plaintext
Create New Key-Value Namespace``` 

**Additional Processing:**
- **KV to Rename** (n8n-nodes-base.set)
**Data Fetching and Processing:**
- **List KV-NMs (5)** (n8n-nodes-base.httpRequest)
  Details:
    - **Notes**: ```plaintext
Get Available Namespaces``` 
- **Delete KV1** (n8n-nodes-base.httpRequest)
  Details:
    - **Notes**: ```plaintext
/storage/kv/namespaces/``` 

**Additional Processing:**
- **Sticky Note3** (n8n-nodes-base.stickyNote)
  Details:
    - **Content**:
```plaintext
## Rename NM of KV (By Serach)
to change parameters read [Docs](https://developers.cloudflare.com/api/operations/workers-kv-namespace-rename-a-namespace)
``` 

**Data Fetching and Processing:**
- **Delete KV** (n8n-nodes-base.httpRequest)
  Details:
    - **Notes**: ```plaintext
Delete Selected KV``` 

**Additional Processing:**
- **Sticky Note2** (n8n-nodes-base.stickyNote)
  Details:
    - **Content**:
```plaintext
## Delete NM of KV (By Name Serach)
to change anything read [Docs](https://developers.cloudflare.com/api/operations/workers-kv-namespace-remove-a-namespace)
``` 
- **Sticky Note1** (n8n-nodes-base.stickyNote)
  Details:
    - **Content**:
```plaintext
## Create NM
to change parameters read [Docs](https://developers.cloudflare.com/api/operations/workers-kv-namespace-create-a-namespace)
``` 
- **Sticky Note** (n8n-nodes-base.stickyNote)
  Details:
    - **Content**:
```plaintext
## List NMs
to change parameters read [Docs](https://developers.cloudflare.com/api/operations/workers-kv-namespace-list-namespaces)
``` 
