function addTask() {  
    var input = document.getElementById("taskInput");  
    var taskText = input.value;  
  
    if (taskText === "") {  
        alert("กรุณาพิมพ์งานก่อนเพิ่ม");  
        return;  
    }  
  
    var li = document.createElement("li");  
    li.textContent = taskText;  
  
    document.getElementById("taskList").appendChild(li);  
  
    input.value = "";  
}  
