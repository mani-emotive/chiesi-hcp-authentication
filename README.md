# chiesi-hcp-authentication
describe('Home Page', function() {
    it ('should open the Home Page', function(){

        browser.manage().window().maximize();
        //browser.driver.get('http://chiesistage.thinkemotive.com');
        browser.driver.get('http://chiesistage:Duplicated34Precancelled@chiesistage.thinkemotive.com');

        browser.sleep(5000);

    });
    it('hcp sign in', function () {

        browser.driver.findElement(By.xpath('/html/body/div[3]/div[2]/div/div[4]/div/button[2]')).click();
        //browser.waitForAngular();
        browser.sleep(2000);

            expect(browser.driver.getCurrentUrl()).toMatch('http://chiesistage.thinkemotive.com');
        browser.sleep(5000);

            //expect(browser.driver.getCurrentUrl()).toMatch('https://e-mastr.com/');
        }, 10000);
});
