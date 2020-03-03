Feature: test feature

  Scenario Outline: Standard user should be able to access only Accounts at Level 0
    Given I am a standard user
    When I login with my credentials
      | Username | Password    |
      | Bob      | password123 |
    And I request balance for <accountnumber> from the accounts API
    Then I should get <balance> as the balance request response

    Examples:
      | accountnumber | balance        |
      | 11111         | Not Authorised |
      | 22222         | Not Authorised |
      | 33333         | 9999           |