# Template
```javascript
templates:{
    [layerName]:{
        [pathname]:{ //__error_404,__error_500
            jsonx:{/* jsonx react element */},
            resources:{
                [propertyName]:'fetchPath',
                [propertyName]:{
                    fetchPath:'url',
                    fetchOptions:{
                        blocking:false,
                    }
                },
            },
            preRenderFunctions:[functionName,'func:window.functionName','func:viewx.functions.functionName'],
            // preRenderFunctionPipe:[functionName,window.functionName,viewx.functions.functionName],
            postRenderFunctions:[functionName,window.functionName,viewx.functions.functionName],
            // postRenderFunctionPipe:[functionName,window.functionName,viewx.functions.functionName],
            pageData:[
                {
                    tagName:'title',
                    innerHTML:'my title',
                    attributes:{prop1:value,prop2:value}
                }
            ],
        }
    }
}
```

# ViewX State
```javascript
views:{
    [layerName]:jsonx,
},
viewdata:{
    [layerName]:jsonx,
},
templates:{
    [layerName]:{
        [pathName]:{
            jsonx,
        }
    }
},
user:{},
auth:{},
ui:{},
```

# ViewX Configuration
```javascript
{
    customComponents:[
        {
            name:ComponentName,
            format:umd|jsonx,
            type:component|library,
            umdFilePath:url,
            jsonx,
            stylesheets:[url,],
        }
    ],
    customScripts:[url,],
    customStyles:[url,],
    customFunctions:[Function,],
    layers:[
        loading,
        modal,
        overlay,
        header,
        footer,
        nav,
        error,
        layout,
    ],
    settings:{
        debug:true,
        router:hash|memory|broswer,
        cacheTemplatesOffline:false,
        templatePath:url,
        templateFetchOptions:{},
    },
    querySelector:'#root',
    application:{
        state:{
            prop,
            prop2,
        },
        preRenderFunction:[functionName,'func:window.functionName','func:viewx.functions.functionName'],
        preRenderFunctionPipe:[functionName,window.functionName,viewx.functions.functionName],
        postRenderFunction:[functionName,window.functionName,viewx.functions.functionName],
        postRenderFunctionPipe:[functionName,window.functionName,viewx.functions.functionName],
    },
    templates:{},
}
```
