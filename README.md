# write-a-trigger-to-preavent-to-delete-if-that-account-has-more-than-2-or-contacts-
write a trigger to preavent to delete if that account has more than 2 or contacts 
publlic static void  preaventdelete(list<Account> accountOldlist)
{  
    set<id> mysetsids=new set<id>();
    
   for(account acc: accountOldlist)
    {

    mysetsids.ass(acc.id)
    }


  map<id,account> accountmap=new map([select id(select id from contacts) from account where id IN:mysetside]);


for(Account accc1:accountIdlist)
{

    if(accountmap.get(acc.id).contact.sixe()>=2)
  {

   acc.addError('This acccount Has more han 2 child conyas you can no delete ')
}
}

