<!-- markdownlint-disable -->

<a href="../src/charm_state.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

# <kbd>module</kbd> `charm_state.py`
State of the Charm. 

**Global Variables**
---------------
- **COS_AGENT_INTEGRATION_NAME**


---

## <kbd>class</kbd> `CharmConfigInvalidError`
Raised when charm config is invalid. 



**Attributes:**
 
 - <b>`msg`</b>:  Explanation of the error. 

<a href="../src/charm_state.py#L27"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>function</kbd> `__init__`

```python
__init__(msg: str)
```

Initialize a new instance of the CharmConfigInvalidError exception. 



**Args:**
 
 - <b>`msg`</b>:  Explanation of the error. 





---

## <kbd>class</kbd> `ProxyConfig`
Proxy configuration. 



**Attributes:**
 
 - <b>`http_proxy`</b>:  HTTP proxy address. 
 - <b>`https_proxy`</b>:  HTTPS proxy address. 
 - <b>`no_proxy`</b>:  Comma-separated list of hosts that should not be proxied. 
 - <b>`use_aproxy`</b>:  Whether aproxy should be used. 


---

#### <kbd>property</kbd> aproxy_address

Return the aproxy address. 



---

<a href="../src/charm_state.py#L85"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>classmethod</kbd> `check_fields`

```python
check_fields(values: dict) → dict
```

Validate the proxy configuration. 

---

<a href="../src/charm_state.py#L51"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>classmethod</kbd> `from_charm`

```python
from_charm(charm: CharmBase) → ProxyConfig
```

Initialize the proxy config from charm. 



**Args:**
 
 - <b>`charm`</b>:  The charm instance. 



**Returns:**
 Current proxy config of the charm. 


---

## <kbd>class</kbd> `State`
The charm state. 



**Attributes:**
 
 - <b>`is_metrics_logging_available`</b>:  Whether the charm is able to issue metrics. 
 - <b>`proxy_config`</b>:  Whether aproxy should be used. 




---

<a href="../src/charm_state.py#L109"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>classmethod</kbd> `from_charm`

```python
from_charm(charm: CharmBase) → State
```

Initialize the state from charm. 



**Args:**
 
 - <b>`charm`</b>:  The charm instance. 



**Returns:**
 Current state of the charm. 


