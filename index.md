<!DOCTYPE html>
<html>

<body>
<!-- Tab links -->
<div class="tab">
  <button class="tablinks" onclick="openTab(event, ‘TAB 1’)">TAB 1</button>
  <button class="tablinks" onclick="openTab(event, ’TAB 2’)">TAB 2</button>
  <button class="tablinks" onclick="openTab(event, ‘TAB 3’)">TAB 3</button>
</div>

<!-- Tab content -->
<div id="TAB 1" class="tabcontent">
  <h3>TAB 1 header </h3>
  <p> TAB 1 content here </p>
</div>

<div id="TAB 2" class="tabcontent">
  <h3>TAB 2</h3>
  <p> TAB 2 content here </p>
</div>

<div id="TAB 3" class="tabcontent">
  <h3>TAB 3</h3>
  <p>TAB 3 content here </p>
</div>
  
<script>
function openTab(evt, tabName) {
  var i, tabcontent, tablinks;

  tabcontent = document.getElementsByClassName("tabcontent");
  for (i = 0; i < tabcontent.length; i++) {
	tabcontent[i].style.display = "none";
  }

  tablinks = document.getElementsByClassName("tablinks");
  for (i = 0; i < tablinks.length; i++) {
	tablinks[i].className = tablinks[i].className.replace(" active", "");
  }

  document.getElementById(tabName).style.display = "block";
  evt.currentTarget.className += " active";
}
  </script>
</body>
  
</html>
