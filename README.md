
# Project Title

searchengine
A small search library.

Primarily intended to be a learning tool to teach the fundamentals of search.

Useful for embedding into Python apps

usage
Example::

import Python_based_microsearch

# Create an instance, pointing it to where the data should be stored.
ms = Python_based_microsearch.SE('/tmp/microsearch')

# Index some data.
ms.index('email_1', {'text': "Peter,\n\nI'm going to need those TPS reports on my desk first thing tomorrow! And clean up your desk!\n\nLumbergh"})
ms.index('email_2', {'text': 'Everyone,\n\nM-m-m-m-my red stapler has gone missing. H-h-has a-an-anyone seen it?\n\nMilton'})
ms.index('email_3', {'text': "Peter,\n\nYeah, I'm going to need you to come in on Saturday. Don't forget those reports.\n\nLumbergh"})
ms.index('email_4', {'text': 'How do you feel about becoming Management?\n\nThe Bobs'})

# Search on it.
ms.search('Peter')
ms.search('tps report')

