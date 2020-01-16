---
title: "Granularity"
date: 2020-01-16T12:35:30Z
---

## Levels of Granularity

### Unit Testing

These focus on testing a single part of the software in isolation; this is usually done at class level in OO programming.

Dependencies, ie. other units the class depends on have assumptions defined for them in the form of Mocks. 
 
```java

class MathOperations {

	private final float[] numbers;

	MathOperations(float[] numbers) {
		this.numbers = numbers; 
	}

	public float getSum() {
		return numbers.stream().sum();
	}
}

class MathOperationsTest {
	
	private final MathOperations fixture;
	private final float[] TEST_NUMBERS = new float[] {2.0, 4.0};

	@Before 
	public void setUp() {
		fixture = new MathOperations(TEST_NUMBERS);
	}

	@Test
	public void testSummation() {
		float result = fixture.getSum();
		float expected = 6.0;
		
		assertThat(expected, is(expected));
	}
}

```

### Component / System Testing

Focuses on testing a set of units combined together in order to produce an expected overall behaviour. 

Colloquially, functional testing is synonymous in this area.


### Integration Testing

Imagine creating a software system that needs to send out emails. How do we verify that it works with our current mail server?

Or perhaps, we rely on authentication from another server such as Facebook or Google?

Integration testing is all about verifying the behaviour of our software with its peers.

### Acceptance Testing

At the end of the day, we create software to address users needs. Whether we formulise these needs through use-cases, Business Requirement documents or user-stories, we need a way to test that our software meets these needs.

Acceptance testing is all about ensuring that our software meets these needs.

