<input id="input">
<button onclick="submit()">submit</button>
<ul id="list">
    <li>name
    <button onclick="deleteitem(event)">delete</button>
    </li>
</ul>
<script>
    var ul=document.getElementById("list")
    var input=document.getElementById("input")
    function submit()
    {
        var listitem=document.createElement("li")
        listitem.innerHTML=input.value +"<button onclick='deleteitem(event)'>delete</button>"
        ul.append(listitem)  
    }
    function deleteitem(event)
    {
        event.target.parentElement.remove()
    }
</script>

