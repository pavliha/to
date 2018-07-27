# utill-to

It is just simple util that helps you to write less code

###### So instead of writing:

```javascript
try{
    const response = await this.instance.post(url, params)
}
catch(err){
    throw "Some error"
} 
```
###### You could write like that:
```javascript 
import to from 'to-util'

const [err, response] = await to(this.instance.post(url, params))
if(err) throw "Some error"

return response
```
