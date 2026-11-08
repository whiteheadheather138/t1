代发 wailian999

[C14] 泛型函数
来源：https://cl.zhonguo4118.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：https://wc.zhonguo8118.cn

PHP:  // 无泛型
来源：https://it.zhonguo8118.cn

JS:   // 无泛型
来源：https://vs.zhonguo6118.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：https://nu.zhonguo7118.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：https://yw.zhonguo4118.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：https://hf.zhonguo5118.cn

Ruby: # 无泛型
来源：https://yh.zhonguo7118.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：https://gb.zhonguo6118.cn

[C15] 解构 / 展开参数
来源：https://eo.zhonguo1118.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：https://bl.zhonguo1118.cn

PHP:  [$a, $b] = $pair;
来源：https://xg.zhonguo3118.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：https://lh.zhonguo5118.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：https://dv.zhonguo2118.cn

Java: // 无解构
来源：https://rs.zhonguo6118.cn

Go:   // 无解构
来源：https://jw.zhonguo6118.cn

Ruby: a, b = pair
来源：https://go.zhonguo6118.cn

C#:   var (a, b) = pair;
来源：https://if.zhonguo6118.cn

[C16] 函数 / 方法重载
来源：https://on.zhonguo6118.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：https://er.zhonguo5118.cn

PHP:  // 无重载
来源：https://vm.zhonguo3118.cn

JS:   // 无重载：靠 arguments.length 分支
来源：https://jh.zhonguo7118.cn

TS:   // 用联合类型或重载签名声明
来源：https://fy.zhonguo7118.cn

Java: void f(int a) {}  void f(String a) {}
来源：https://se.zhonguo4118.cn

Go:   // 无重载：用不同函数名
来源：https://lm.zhonguo5118.cn

Ruby: # 无重载：靠动态参数
来源：https://rj.zhonguo7118.cn

C#:   void F(int a) {}  void F(string a) {}
来源：https://ow.zhonguo4118.cn

================================================================================
来源：https://vj.zhonguo7118.cn

D. 数组 / 列表 / 集合
来源：https://ll.zhonguo8118.cn

================================================================================
来源：https://xe.zhonguo8118.cn

[D01] 创建数组 / 列表
来源：https://ci.zhonguo3118.cn

Py:   arr = [1, 2, 3];  empty = []
来源：https://tj.zhonguo7118.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：https://iq.zhonguo7118.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：https://rh.zhonguo5118.cn

TS:   const arr: number[] = [1, 2, 3];
来源：https://ii.zhonguo6118.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：https://mt.zhonguo5118.cn

Go:   arr := []int{1, 2, 3}
来源：https://cq.zhonguo6118.cn

Ruby: arr = [1, 2, 3]
来源：https://ar.zhonguo6118.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：https://cj.zhonguo6118.cn

[D02] 追加元素到末尾
来源：https://lt.zhonguo2118.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：https://cg.zhonguo1118.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：https://ew.zhonguo5118.cn

JS:   arr.push(4);
来源：https://nb.zhonguo8118.cn

TS:   arr.push(4);
来源：https://up.zhonguo7118.cn

Java: list.add(4);
来源：https://mq.zhonguo5118.cn

Go:   arr = append(arr, 4)
来源：https://fn.zhonguo2118.cn

Ruby: arr << 4; arr.push(5)
来源：https://im.zhonguo2118.cn

C#:   list.Add(4);
来源：https://rf.zhonguo1118.cn

[D03] 在指定位置插入元素
来源：https://to.zhonguo8118.cn

Py:   arr.insert(0, 0)
来源：https://tf.zhonguo4118.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：https://bd.zhonguo1118.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：https://pu.zhonguo1118.cn

TS:   arr.splice(0, 0, 0);
来源：https://lb.zhonguo5118.cn

Java: list.add(0, 0);
来源：https://yp.zhonguo7118.cn

Go:   arr = append([]int{0}, arr...)
来源：https://ke.zhonguo3118.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：https://rp.zhonguo7118.cn

C#:   list.Insert(0, 0);
来源：https://zh.zhonguo2118.cn

[D04] 删除元素
来源：https://su.zhonguo6118.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：https://gw.zhonguo7118.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：https://no.zhonguo8118.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：https://jf.zhonguo7118.cn

TS:   arr.splice(0, 1);
来源：https://vf.zhonguo3118.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：https://ml.zhonguo4118.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：https://ak.zhonguo8118.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：https://qh.zhonguo3118.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：https://sg.zhonguo6118.cn

[D05] 访问与修改元素
来源：https://ng.zhonguo8118.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：https://vu.zhonguo6118.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：https://bz.zhonguo4118.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：https://lj.zhonguo1118.cn

TS:   arr[0]; arr.at(-1);
来源：https://ik.zhonguo8118.cn

Java: list.get(0); list.set(0, 9);
来源：https://ln.zhonguo8118.cn

Go:   arr[0]; arr[0] = 9
来源：https://qo.zhonguo8118.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：https://wb.zhonguo4118.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：https://zv.zhonguo5118.cn

[D06] 数组长度
来源：https://ej.zhonguo3118.cn

Py:   len(arr)
来源：https://kw.zhonguo1118.cn

PHP:  count($arr);
来源：https://fu.zhonguo5118.cn

JS:   arr.length
来源：https://gn.zhonguo7118.cn

TS:   arr.length
来源：https://tq.zhonguo8118.cn

Java: list.size();
来源：https://rv.zhonguo8118.cn

Go:   len(arr)
来源：https://vx.zhonguo4118.cn

Ruby: arr.length; arr.size
来源：https://sq.zhonguo5118.cn

C#:   list.Count;
来源：https://an.zhonguo7118.cn

[D07] 切片 / 取子数组
来源：https://mq.zhonguo1118.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：https://rn.zhonguo4118.cn

PHP:  array_slice($arr, 1, 3);
来源：https://ej.zhonguo8118.cn

JS:   arr.slice(1, 4);
来源：https://pe.zhonguo4118.cn

TS:   arr.slice(1, 4);
来源：https://xj.zhonguo8118.cn

Java: list.subList(1, 4);
来源：https://jp.zhonguo5118.cn

Go:   arr[1:4]
来源：https://wk.zhonguo7118.cn

Ruby: arr[1, 3]
来源：https://tq.zhonguo1118.cn

C#:   list.GetRange(1, 3);
来源：https://fk.zhonguo8118.cn

[D08] 合并两个数组
来源：https://kx.zhonguo5118.cn

Py:   a + b;  a.extend(b)
来源：https://tf.zhonguo2118.cn

PHP:  array_merge($a, $b);
来源：https://ec.zhonguo2118.cn

JS:   [...a, ...b];  a.concat(b);
来源：https://et.zhonguo5118.cn

TS:   [...a, ...b];
来源：https://us.zhonguo6118.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：https://rh.zhonguo3118.cn

Go:   append(a, b...)
来源：https://lz.zhonguo8118.cn

Ruby: a + b;  a.concat(b)
来源：https://qq.zhonguo4118.cn

C#:   a.Concat(b).ToList()
来源：https://xh.zhonguo4118.cn

[D09] 排序（升序）
来源：https://jt.zhonguo6118.cn

Py:   sorted(arr);  arr.sort()
来源：https://wp.zhonguo2118.cn

PHP:  sort($arr);
来源：https://lx.zhonguo6118.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：https://qk.zhonguo2118.cn

TS:   [...arr].sort((x, y) => x - y);
来源：https://qz.zhonguo8118.cn

Java: Collections.sort(list);  list.sort(null);
来源：https://gf.zhonguo8118.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：https://yo.zhonguo4118.cn

Ruby: arr.sort
来源：https://wj.zhonguo1118.cn

C#:   list.Sort();
来源：https://oy.zhonguo8118.cn

[D10] 自定义排序（按字段 / 多条件）
来源：https://ez.zhonguo8118.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：https://rk.zhonguo8118.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://mo.zhonguo1118.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：https://gd.zhonguo5118.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：https://di.zhonguo5118.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：https://dz.zhonguo8118.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：https://ji.zhonguo2118.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：https://ga.zhonguo5118.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：https://pu.zhonguo7118.cn

[D11] 反转数组
来源：https://bc.zhonguo1118.cn

Py:   arr[::-1];  arr.reverse()
来源：https://qo.zhonguo6118.cn

PHP:  array_reverse($arr);
来源：https://xg.zhonguo7118.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：https://bu.zhonguo2118.cn

TS:   [...arr].reverse();
来源：https://ee.zhonguo3118.cn

Java: Collections.reverse(list);
来源：https://rz.zhonguo3118.cn

Go:   slices.Reverse(arr)
来源：https://gu.zhonguo5118.cn

Ruby: arr.reverse
来源：https://iz.zhonguo3118.cn

C#:   list.Reverse();
来源：https://yd.zhonguo1118.cn

[D12] 查找元素下标
来源：https://ag.zhonguo4118.cn

Py:   arr.index(x);  x in arr
来源：https://sh.zhonguo4118.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：https://xr.zhonguo1118.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://zw.zhonguo4118.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://jc.zhonguo4118.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：https://og.zhonguo1118.cn

Go:   slices.Index(arr, x)
来源：https://cg.zhonguo2118.cn

Ruby: arr.index(x)
来源：https://il.zhonguo4118.cn

C#:   list.IndexOf(x);
来源：https://rx.zhonguo5118.cn

[D13] 过滤（保留满足条件的）
来源：https://ol.zhonguo8118.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：https://mj.zhonguo8118.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：https://ee.zhonguo5118.cn

JS:   arr.filter(x => x > 3)
来源：https://al.zhonguo6118.cn

TS:   arr.filter(x => x > 3)
来源：https://ch.zhonguo1118.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：https://ip.zhonguo2118.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：https://gx.zhonguo1118.cn

Ruby: arr.select { |x| x > 3 }
来源：https://jg.zhonguo2118.cn

C#:   list.Where(x => x > 3).ToList()
来源：https://po.zhonguo8118.cn

[D14] 映射转换（每个元素变形）
来源：https://jp.zhonguo5118.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：https://rh.zhonguo2118.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：https://xi.zhonguo5118.cn

JS:   arr.map(x => x * 2)
来源：https://om.zhonguo1118.cn

TS:   arr.map(x => x * 2)
来源：https://eq.zhonguo5118.cn

Java: list.stream().map(x -> x * 2).toList()
来源：https://rn.zhonguo3118.cn

Go:   // 手写循环
来源：https://pr.zhonguo1118.cn

Ruby: arr.map { |x| x * 2 }
来源：https://ue.zhonguo3118.cn

C#:   list.Select(x => x * 2).ToList()
来源：https://it.zhonguo2118.cn

[D15] 去重
来源：https://oa.zhonguo2118.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：https://bo.zhonguo3118.cn

PHP:  array_unique($arr);
来源：https://gj.zhonguo8118.cn

JS:   [...new Set(arr)]
来源：https://dd.zhonguo6118.cn

TS:   [...new Set(arr)]
来源：https://hx.zhonguo8118.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：https://kz.zhonguo3118.cn

Go:   // 用 map[T]struct{} 手写
来源：https://pc.zhonguo4118.cn

Ruby: arr.uniq
来源：https://dj.zhonguo2118.cn

C#:   list.Distinct().ToList()
来源：https://nv.zhonguo2118.cn

[D16] 求和与平均值
来源：https://hs.zhonguo8118.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：https://bv.zhonguo6118.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：https://fw.zhonguo2118.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：https://hc.zhonguo3118.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：https://lv.zhonguo4118.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：https://so.zhonguo1118.cn

Go:   // 手写循环累加
来源：https://km.zhonguo6118.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：https://nc.zhonguo8118.cn

C#:   list.Sum();  list.Average()
来源：https://gz.zhonguo1118.cn

[D17] 最大值与最小值
来源：https://mr.zhonguo3118.cn

Py:   max(arr);  min(arr)
来源：https://kg.zhonguo1118.cn

PHP:  max($arr);  min($arr);
来源：https://bw.zhonguo8118.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：https://dr.zhonguo8118.cn

TS:   Math.max(...arr);
来源：https://jv.zhonguo7118.cn

Java: Collections.max(list);  Collections.min(list);
来源：https://ai.zhonguo4118.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：https://pe.zhonguo6118.cn

Ruby: arr.max;  arr.min
来源：https://sh.zhonguo6118.cn

C#:   list.Max();  list.Min()
来源：https://je.zhonguo5118.cn

[D18] 扁平化嵌套数组
来源：https://su.zhonguo2118.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：https://zz.zhonguo8118.cn

PHP:  array_merge(...$nested);
来源：https://mj.zhonguo3118.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：https://bz.zhonguo8118.cn

TS:   nested.flat();
来源：https://qa.zhonguo6118.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：https://fc.zhonguo2118.cn

Go:   // 手写双层循环
来源：https://ko.zhonguo7118.cn

Ruby: nested.flatten
来源：https://vx.zhonguo8118.cn

C#:   nested.SelectMany(x => x).ToList()
来源：https://wc.zhonguo8118.cn

[D19] 按字段分组
来源：https://qe.zhonguo2118.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：https://wr.zhonguo6118.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：https://bj.zhonguo1118.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：https://on.zhonguo6118.cn

TS:   Object.groupBy(arr, x => x.type)
来源：https://ps.zhonguo8118.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：https://la.zhonguo5118.cn

Go:   // 手写 map[string][]T
来源：https://dm.zhonguo2118.cn

Ruby: arr.group_by { |x| x[:type] }
来源：https://kv.zhonguo6118.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：https://lc.zhonguo2118.cn

[D20] 统计每个元素出现次数
来源：https://ar.zhonguo5118.cn

Py:   Counter(arr)
来源：https://iw.zhonguo6118.cn

PHP:  array_count_values($arr);
来源：https://ml.zhonguo4118.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://lq.zhonguo3118.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://ue.zhonguo7118.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：https://uk.zhonguo1118.cn

Go:   // 手写 map[T]int
来源：https://cc.zhonguo2118.cn

Ruby: arr.tally
来源：https://wu.zhonguo8118.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：https://sx.zhonguo4118.cn

[D21] 判断是否包含某元素
来源：https://zu.zhonguo4118.cn

Py:   x in arr
来源：https://yj.zhonguo4118.cn

PHP:  in_array($x, $arr, true);
来源：https://po.zhonguo5118.cn

JS:   arr.includes(x)
来源：https://dd.zhonguo4118.cn

TS:   arr.includes(x)
来源：https://tx.zhonguo2118.cn

Java: list.contains(x)
来源：https://cl.zhonguo6118.cn

Go:   slices.Contains(arr, x)
来源：https://eq.zhonguo2118.cn

Ruby: arr.include?(x)
来源：https://qe.zhonguo1118.cn

C#:   list.Contains(x)
来源：https://ao.zhonguo4118.cn

[D22] 复制数组（避免共享引用）
来源：https://tw.zhonguo2118.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：https://ph.zhonguo5118.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：https://ad.zhonguo5118.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：https://tl.zhonguo1118.cn

TS:   [...arr];
来源：https://yg.zhonguo1118.cn

Java: new ArrayList<>(list);
来源：https://vb.zhonguo5118.cn

Go:   copied := append([]int(nil), arr...)
来源：https://sc.zhonguo1118.cn

Ruby: arr.dup;  arr.clone
来源：https://vs.zhonguo6118.cn

C#:   new List<int>(list);
来源：https://gt.zhonguo3118.cn

[D23] reduce 累积计算
来源：https://cj.zhonguo6118.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：https://xd.zhonguo7118.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：https://oi.zhonguo7118.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://dz.zhonguo3118.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://tx.zhonguo8118.cn

Java: list.stream().reduce(0, Integer::sum)
来源：https://kd.zhonguo7118.cn

Go:   // 手写循环
来源：https://ie.zhonguo3118.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：https://dv.zhonguo3118.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：https://dw.zhonguo1118.cn

[D24] 字典 / Map 基本操作
来源：https://bw.zhonguo5118.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：https://ul.zhonguo6118.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：https://qs.zhonguo6118.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：https://xy.zhonguo7118.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：https://tm.zhonguo7118.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：https://xf.zhonguo5118.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：https://ze.zhonguo1118.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：https://fq.zhonguo6118.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：https://zy.zhonguo4118.cn

[D25] Set 集合去重与交并差
来源：https://ni.zhonguo5118.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：https://nh.zhonguo1118.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：https://zh.zhonguo3118.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：https://ba.zhonguo7118.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：https://ra.zhonguo4118.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：https://ii.zhonguo3118.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：https://iv.zhonguo2118.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：https://jv.zhonguo3118.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：https://wb.zhonguo2118.cn

[D26] 数组转字符串
来源：https://dg.zhonguo7118.cn

Py:   ", ".join(map(str, arr))
来源：https://pg.zhonguo4118.cn

PHP:  implode(", ", $arr);
来源：https://op.zhonguo4118.cn

JS:   arr.join(", ")
来源：https://pq.zhonguo6118.cn

TS:   arr.join(", ")
来源：https://xf.zhonguo4118.cn

Java: String.join(", ", list)
来源：https://xy.zhonguo4118.cn

Go:   strings.Join(strs, ", ")
来源：https://at.zhonguo1118.cn

Ruby: arr.join(", ")
来源：https://ik.zhonguo1118.cn

C#:   string.Join(", ", list)
来源：https://ak.zhonguo5118.cn

================================================================================
来源：https://oj.zhonguo2118.cn

E. 字符串处理
来源：https://mm.zhonguo2118.cn

================================================================================
来源：https://sy.zhonguo6118.cn

[E01] 拼接字符串
来源：https://af.zhonguo4118.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：https://jh.zhonguo7118.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：https://od.zhonguo1118.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：https://dc.zhonguo3118.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：https://hq.zhonguo4118.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：https://ag.zhonguo7118.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：https://bt.zhonguo3118.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：https://rw.zhonguo3118.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：https://cn.zhonguo3118.cn

[E02] 重复字符串
来源：https://rp.zhonguo3118.cn

Py:   "ab" * 3
来源：https://ab.zhonguo7118.cn

PHP:  str_repeat("ab", 3);
来源：https://ek.zhonguo7118.cn

JS:   "ab".repeat(3)
来源：https://io.zhonguo2118.cn

TS:   "ab".repeat(3)
来源：https://ef.zhonguo3118.cn

Java: "ab".repeat(3)
来源：https://pv.zhonguo5118.cn

Go:   strings.Repeat("ab", 3)
来源：https://tp.zhonguo6118.cn

Ruby: "ab" * 3
来源：https://cd.zhonguo8118.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：https://xf.zhonguo6118.cn

[E03] 截取子串
来源：https://ns.zhonguo4118.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：https://rg.zhonguo3118.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：https://hk.zhonguo3118.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：https://qe.zhonguo8118.cn

TS:   s.slice(1, 4)
来源：https://sm.zhonguo1118.cn

Java: s.substring(1, 4)
来源：https://ww.zhonguo5118.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：https://vq.zhonguo8118.cn

Ruby: s[1, 3];  s[1..3]
来源：https://ey.zhonguo5118.cn

C#:   s.Substring(1, 3)
来源：https://wa.zhonguo4118.cn

[E04] 查找子串位置
来源：https://gb.zhonguo4118.cn

Py:   s.find("x");  s.index("x")
来源：https://op.zhonguo2118.cn

PHP:  strpos($s, "x");
来源：https://jy.zhonguo7118.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：https://kf.zhonguo1118.cn

TS:   s.indexOf("x")
来源：https://tv.zhonguo1118.cn

Java: s.indexOf("x")
来源：https://tz.zhonguo3118.cn


<!-- 参考信息 -->