# Blitz Test №7
**1.** Кои са необходимите функции, които типа `T` трябва да притежава, за да бъде приложима шаблонната функция `areEqual`?
```c++
template <typename T>
bool areEqual(const T& lhs, const T& rhs)
{
	if (lhs.size() != rhs.size())
	{
		return false;
	}

	for (size_t i = 0; i < lhs.size(); i++)
	{
		if (lhs[i] != rhs[i])
		{
			return false;
		}
	}

	return true;
}
```

**2.** Напишете **шаблонна** функция `linearSearch`, която извършва линейно търсене измежду елементите на подаден `Vector` от обекти. Функцията приема вектор от обекти от шаблонен тип, както и търсения обект. Резултатът от функцията е индекса на намерения елемент, а ако него го няма - връща `-1`.
