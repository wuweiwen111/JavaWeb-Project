Under branch Main, I created a fake json file and url. The steps are following:
- Click on 'Settings', then find the 'Pages' section in the sidebar or menu.
- Under 'Source', select the branch you want to use (e.g., main) from the dropdown menu, and choose the folder (typically / (root)).

vue-project/src/views/tlias will need to access this json file by
  mounted(){
    axios.get("https://wuweiwen111.github.io/JavaWeb-Project/db.json").then((result)=>{
        this.tableData = result.data.data;
    })
  }
