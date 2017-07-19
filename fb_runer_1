test.describe('new_file_1', function () {
  let driver;
  //ok here was the links to facebook posts 
	let urls = ['https://www.facebook.com/madsmilexd/posts/1364154196956397:0','https://www.facebook.com/madsmilexd/posts/1083641195007700','https://www.facebook.com/madsmilexd/posts/1021604747878012'];
  //and here phrases for post post_id == phrase_id
  let phrases = ['first post wih remove 1','second post wih remove 1', 'third post wih remove 1'];
  let remove_by_ts = [1500396134,1500396138,1500409543];
  test.before(function () {
    driver = new Driver();
  });

  test.after(function () {
    driver.quit();
  });

  test.it('should pass', function () {
    urls.forEach(function(url, id){
    	driver.get(url);
      	let first_selector = '[data-utime="' + remove_by_ts[id] + '"]';
      window.mad_fb_pst_tmp_css = first_selector;
      	var comment_ts = driver.findElement(By.css(first_selector)).then(function(el){
        	driver.executeScript(function () {
              	return
            });
        });
      driver.findElement(By.className('UFIAddCommentInput')).click().then(function(){
         
           var element = driver.findElement(By.css('.UFIAddCommentInput'));
           var element = driver.findElement(By.css('.UFIAddCommentInput'));
          // element.sendKeys(phrases[id],Key.ENTER);         
          var comment = driver.findElement(By.css('.UFILastComment .livetimestamp')).getAttribute('data-utime').then(function(data){
            driver.findElement(By.css('.UFILastComment')).findElement(By.css('.UFICommentCloseButton')).click().then(function(){
              driver.findElement(By.css('[data-testid="ufi_comment_menu_delete"]')).click().then(function(){
                driver.sleep(1000);
                  driver.findElement(By.css('[data-testid="ufi_hide_dialog_delete_button"]')).click();
              });
            });

          });
        });
      driver.sleep(10000);
      	
    });

  });
});
