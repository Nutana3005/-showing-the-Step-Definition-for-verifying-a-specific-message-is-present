# -showing-the-Step-Definition-for-verifying-a-specific-message-is-present
@then('I should see the message "{message}"')
def step_impl(context, message):
    assert message in context.browser.page_source
