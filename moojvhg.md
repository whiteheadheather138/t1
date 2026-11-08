代发 wailian999

[C14] 泛型函数
来源：https://ns.zhonguo8118.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：https://mu.zhonguo5118.cn

PHP:  // 无泛型
来源：https://vm.zhonguo1118.cn

JS:   // 无泛型
来源：https://va.zhonguo4118.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：https://sr.zhonguo7118.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：https://om.zhonguo7118.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：https://ij.zhonguo7118.cn

Ruby: # 无泛型
来源：https://oy.zhonguo3118.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：https://vv.zhonguo4118.cn

[C15] 解构 / 展开参数
来源：https://xe.zhonguo3118.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：https://ag.zhonguo8118.cn

PHP:  [$a, $b] = $pair;
来源：https://on.zhonguo5118.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：https://xv.zhonguo7118.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：https://qp.zhonguo6118.cn

Java: // 无解构
来源：https://gv.zhonguo5118.cn

Go:   // 无解构
来源：https://zm.zhonguo3118.cn

Ruby: a, b = pair
来源：https://xd.zhonguo4118.cn

C#:   var (a, b) = pair;
来源：https://ce.zhonguo5118.cn

[C16] 函数 / 方法重载
来源：https://hn.zhonguo6118.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：https://zg.zhonguo8118.cn

PHP:  // 无重载
来源：https://en.zhonguo1118.cn

JS:   // 无重载：靠 arguments.length 分支
来源：https://nl.zhonguo7118.cn

TS:   // 用联合类型或重载签名声明
来源：https://eq.zhonguo1118.cn

Java: void f(int a) {}  void f(String a) {}
来源：https://eu.zhonguo5118.cn

Go:   // 无重载：用不同函数名
来源：https://bb.zhonguo2118.cn

Ruby: # 无重载：靠动态参数
来源：https://ds.zhonguo3118.cn

C#:   void F(int a) {}  void F(string a) {}
来源：https://dj.zhonguo7118.cn

================================================================================
来源：https://ow.zhonguo3118.cn

D. 数组 / 列表 / 集合
来源：https://eq.zhonguo7118.cn

================================================================================
来源：https://ig.zhonguo4118.cn

[D01] 创建数组 / 列表
来源：https://km.zhonguo4118.cn

Py:   arr = [1, 2, 3];  empty = []
来源：https://fn.zhonguo1118.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：https://ue.zhonguo2118.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：https://xc.zhonguo8118.cn

TS:   const arr: number[] = [1, 2, 3];
来源：https://gp.zhonguo8118.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：https://ih.zhonguo5118.cn

Go:   arr := []int{1, 2, 3}
来源：https://pu.zhonguo2118.cn

Ruby: arr = [1, 2, 3]
来源：https://mj.zhonguo4118.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：https://eh.zhonguo3118.cn

[D02] 追加元素到末尾
来源：https://kw.zhonguo4118.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：https://nt.zhonguo4118.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：https://to.zhonguo6118.cn

JS:   arr.push(4);
来源：https://rv.zhonguo4118.cn

TS:   arr.push(4);
来源：https://lz.zhonguo1118.cn

Java: list.add(4);
来源：https://hb.zhonguo5118.cn

Go:   arr = append(arr, 4)
来源：https://al.zhonguo6118.cn

Ruby: arr << 4; arr.push(5)
来源：https://wj.zhonguo2118.cn

C#:   list.Add(4);
来源：https://gk.zhonguo5118.cn

[D03] 在指定位置插入元素
来源：https://uf.zhonguo5118.cn

Py:   arr.insert(0, 0)
来源：https://cu.zhonguo2118.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：https://oh.zhonguo4118.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：https://bz.zhonguo2118.cn

TS:   arr.splice(0, 0, 0);
来源：https://vc.zhonguo2118.cn

Java: list.add(0, 0);
来源：https://ig.zhonguo5118.cn

Go:   arr = append([]int{0}, arr...)
来源：https://ik.zhonguo4118.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：https://tm.zhonguo5118.cn

C#:   list.Insert(0, 0);
来源：https://ba.zhonguo5118.cn

[D04] 删除元素
来源：https://ic.zhonguo2118.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：https://eh.zhonguo2118.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：https://bk.zhonguo4118.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：https://mz.zhonguo3118.cn

TS:   arr.splice(0, 1);
来源：https://mq.zhonguo2118.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：https://xy.zhonguo8118.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：https://qo.zhonguo7118.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：https://oh.zhonguo2118.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：https://ik.zhonguo8118.cn

[D05] 访问与修改元素
来源：https://vy.zhonguo7118.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：https://tb.zhonguo4118.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：https://xf.zhonguo8118.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：https://ew.zhonguo1118.cn

TS:   arr[0]; arr.at(-1);
来源：https://yi.zhonguo4118.cn

Java: list.get(0); list.set(0, 9);
来源：https://qz.zhonguo2118.cn

Go:   arr[0]; arr[0] = 9
来源：https://cc.zhonguo3118.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：https://zx.zhonguo3118.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：https://gc.zhonguo2118.cn

[D06] 数组长度
来源：https://ck.zhonguo1118.cn

Py:   len(arr)
来源：https://es.zhonguo5118.cn

PHP:  count($arr);
来源：https://iw.zhonguo7118.cn

JS:   arr.length
来源：https://bk.zhonguo1118.cn

TS:   arr.length
来源：https://ix.zhonguo8118.cn

Java: list.size();
来源：https://eo.zhonguo4118.cn

Go:   len(arr)
来源：https://cj.zhonguo1118.cn

Ruby: arr.length; arr.size
来源：https://ei.zhonguo5118.cn

C#:   list.Count;
来源：https://sh.zhonguo1118.cn

[D07] 切片 / 取子数组
来源：https://ao.zhonguo7118.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：https://tc.zhonguo2118.cn

PHP:  array_slice($arr, 1, 3);
来源：https://bv.zhonguo7118.cn

JS:   arr.slice(1, 4);
来源：https://ip.zhonguo8118.cn

TS:   arr.slice(1, 4);
来源：https://lg.zhonguo6118.cn

Java: list.subList(1, 4);
来源：https://nx.zhonguo3118.cn

Go:   arr[1:4]
来源：https://pl.zhonguo5118.cn

Ruby: arr[1, 3]
来源：https://xp.zhonguo6118.cn

C#:   list.GetRange(1, 3);
来源：https://un.zhonguo6118.cn

[D08] 合并两个数组
来源：https://ci.zhonguo7118.cn

Py:   a + b;  a.extend(b)
来源：https://rs.zhonguo8118.cn

PHP:  array_merge($a, $b);
来源：https://hf.zhonguo5118.cn

JS:   [...a, ...b];  a.concat(b);
来源：https://ag.zhonguo8118.cn

TS:   [...a, ...b];
来源：https://vt.zhonguo2118.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：https://fa.zhonguo8118.cn

Go:   append(a, b...)
来源：https://as.zhonguo1118.cn

Ruby: a + b;  a.concat(b)
来源：https://xq.zhonguo5118.cn

C#:   a.Concat(b).ToList()
来源：https://og.zhonguo1118.cn

[D09] 排序（升序）
来源：https://xy.zhonguo8118.cn

Py:   sorted(arr);  arr.sort()
来源：https://vv.zhonguo3118.cn

PHP:  sort($arr);
来源：https://wu.zhonguo6118.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：https://nx.zhonguo3118.cn

TS:   [...arr].sort((x, y) => x - y);
来源：https://xa.zhonguo1118.cn

Java: Collections.sort(list);  list.sort(null);
来源：https://wb.zhonguo7118.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：https://bi.zhonguo8118.cn

Ruby: arr.sort
来源：https://nx.zhonguo2118.cn

C#:   list.Sort();
来源：https://gw.zhonguo1118.cn

[D10] 自定义排序（按字段 / 多条件）
来源：https://rq.zhonguo7118.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：https://es.zhonguo1118.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://ev.zhonguo7118.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：https://wp.zhonguo5118.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：https://hx.zhonguo7118.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：https://ly.zhonguo8118.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：https://qz.zhonguo4118.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：https://yp.zhonguo6118.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：https://ei.zhonguo4118.cn

[D11] 反转数组
来源：https://jh.zhonguo7118.cn

Py:   arr[::-1];  arr.reverse()
来源：https://zu.zhonguo6118.cn

PHP:  array_reverse($arr);
来源：https://qa.zhonguo6118.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：https://bv.zhonguo2118.cn

TS:   [...arr].reverse();
来源：https://bh.zhonguo6118.cn

Java: Collections.reverse(list);
来源：https://ag.zhonguo3118.cn

Go:   slices.Reverse(arr)
来源：https://tv.zhonguo8118.cn

Ruby: arr.reverse
来源：https://zv.zhonguo3118.cn

C#:   list.Reverse();
来源：https://bo.zhonguo3118.cn

[D12] 查找元素下标
来源：https://pn.zhonguo5118.cn

Py:   arr.index(x);  x in arr
来源：https://qy.zhonguo4118.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：https://el.zhonguo8118.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://ca.zhonguo6118.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://ty.zhonguo1118.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：https://kk.zhonguo1118.cn

Go:   slices.Index(arr, x)
来源：https://qn.zhonguo2118.cn

Ruby: arr.index(x)
来源：https://dx.zhonguo4118.cn

C#:   list.IndexOf(x);
来源：https://ex.zhonguo7118.cn

[D13] 过滤（保留满足条件的）
来源：https://it.zhonguo8118.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：https://la.zhonguo5118.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：https://wc.zhonguo1118.cn

JS:   arr.filter(x => x > 3)
来源：https://hu.zhonguo4118.cn

TS:   arr.filter(x => x > 3)
来源：https://ux.zhonguo2118.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：https://cj.zhonguo2118.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：https://ma.zhonguo4118.cn

Ruby: arr.select { |x| x > 3 }
来源：https://ql.zhonguo2118.cn

C#:   list.Where(x => x > 3).ToList()
来源：https://hp.zhonguo6118.cn

[D14] 映射转换（每个元素变形）
来源：https://nw.zhonguo1118.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：https://tq.zhonguo3118.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：https://dy.zhonguo3118.cn

JS:   arr.map(x => x * 2)
来源：https://ht.zhonguo8118.cn

TS:   arr.map(x => x * 2)
来源：https://dj.zhonguo4118.cn

Java: list.stream().map(x -> x * 2).toList()
来源：https://us.zhonguo4118.cn

Go:   // 手写循环
来源：https://th.zhonguo7118.cn

Ruby: arr.map { |x| x * 2 }
来源：https://bk.zhonguo2118.cn

C#:   list.Select(x => x * 2).ToList()
来源：https://ac.zhonguo5118.cn

[D15] 去重
来源：https://ny.zhonguo4118.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：https://vk.zhonguo3118.cn

PHP:  array_unique($arr);
来源：https://ra.zhonguo7118.cn

JS:   [...new Set(arr)]
来源：https://wr.zhonguo8118.cn

TS:   [...new Set(arr)]
来源：https://py.zhonguo7118.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：https://wk.zhonguo7118.cn

Go:   // 用 map[T]struct{} 手写
来源：https://ap.zhonguo2118.cn

Ruby: arr.uniq
来源：https://ji.zhonguo3118.cn

C#:   list.Distinct().ToList()
来源：https://zf.zhonguo8118.cn

[D16] 求和与平均值
来源：https://lq.zhonguo4118.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：https://pf.zhonguo3118.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：https://wz.zhonguo3118.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：https://lx.zhonguo6118.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：https://il.zhonguo7118.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：https://od.zhonguo8118.cn

Go:   // 手写循环累加
来源：https://ls.zhonguo7118.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：https://xx.zhonguo6118.cn

C#:   list.Sum();  list.Average()
来源：https://we.zhonguo4118.cn

[D17] 最大值与最小值
来源：https://aj.zhonguo5118.cn

Py:   max(arr);  min(arr)
来源：https://sq.zhonguo1118.cn

PHP:  max($arr);  min($arr);
来源：https://tn.zhonguo2118.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：https://dc.zhonguo1118.cn

TS:   Math.max(...arr);
来源：https://ky.zhonguo8118.cn

Java: Collections.max(list);  Collections.min(list);
来源：https://qz.zhonguo3118.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：https://jl.zhonguo5118.cn

Ruby: arr.max;  arr.min
来源：https://or.zhonguo8118.cn

C#:   list.Max();  list.Min()
来源：https://ud.zhonguo4118.cn

[D18] 扁平化嵌套数组
来源：https://cu.zhonguo5118.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：https://nk.zhonguo4118.cn

PHP:  array_merge(...$nested);
来源：https://ui.zhonguo8118.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：https://mp.zhonguo1118.cn

TS:   nested.flat();
来源：https://hu.zhonguo6118.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：https://zd.zhonguo6118.cn

Go:   // 手写双层循环
来源：https://dt.zhonguo5118.cn

Ruby: nested.flatten
来源：https://hv.zhonguo6118.cn

C#:   nested.SelectMany(x => x).ToList()
来源：https://ze.zhonguo7118.cn

[D19] 按字段分组
来源：https://gl.zhonguo7118.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：https://hq.zhonguo6118.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：https://dz.zhonguo7118.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：https://dm.zhonguo7118.cn

TS:   Object.groupBy(arr, x => x.type)
来源：https://sp.zhonguo1118.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：https://lf.zhonguo5118.cn

Go:   // 手写 map[string][]T
来源：https://dr.zhonguo2118.cn

Ruby: arr.group_by { |x| x[:type] }
来源：https://vb.zhonguo1118.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：https://pf.zhonguo3118.cn

[D20] 统计每个元素出现次数
来源：https://ui.zhonguo3118.cn

Py:   Counter(arr)
来源：https://qm.zhonguo5118.cn

PHP:  array_count_values($arr);
来源：https://lk.zhonguo5118.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://ev.zhonguo4118.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://ze.zhonguo5118.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：https://gg.zhonguo3118.cn

Go:   // 手写 map[T]int
来源：https://og.zhonguo6118.cn

Ruby: arr.tally
来源：https://yi.zhonguo8118.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：https://kh.zhonguo4118.cn

[D21] 判断是否包含某元素
来源：https://qz.zhonguo1118.cn

Py:   x in arr
来源：https://xd.zhonguo4118.cn

PHP:  in_array($x, $arr, true);
来源：https://mq.zhonguo1118.cn

JS:   arr.includes(x)
来源：https://nv.zhonguo7118.cn

TS:   arr.includes(x)
来源：https://lc.zhonguo5118.cn

Java: list.contains(x)
来源：https://yg.zhonguo1118.cn

Go:   slices.Contains(arr, x)
来源：https://av.zhonguo7118.cn

Ruby: arr.include?(x)
来源：https://aj.zhonguo3118.cn

C#:   list.Contains(x)
来源：https://we.zhonguo2118.cn

[D22] 复制数组（避免共享引用）
来源：https://at.zhonguo3118.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：https://nq.zhonguo5118.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：https://nq.zhonguo7118.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：https://da.zhonguo5118.cn

TS:   [...arr];
来源：https://jc.zhonguo7118.cn

Java: new ArrayList<>(list);
来源：https://nt.zhonguo4118.cn

Go:   copied := append([]int(nil), arr...)
来源：https://yc.zhonguo7118.cn

Ruby: arr.dup;  arr.clone
来源：https://rt.zhonguo5118.cn

C#:   new List<int>(list);
来源：https://vx.zhonguo6118.cn

[D23] reduce 累积计算
来源：https://zg.zhonguo2118.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：https://mn.zhonguo8118.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：https://eu.zhonguo8118.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://mv.zhonguo4118.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://sk.zhonguo7118.cn

Java: list.stream().reduce(0, Integer::sum)
来源：https://yk.zhonguo1118.cn

Go:   // 手写循环
来源：https://ms.zhonguo7118.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：https://al.zhonguo6118.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：https://wr.zhonguo7118.cn

[D24] 字典 / Map 基本操作
来源：https://vw.zhonguo4118.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：https://mj.zhonguo4118.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：https://qi.zhonguo5118.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：https://mp.zhonguo3118.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：https://vu.zhonguo4118.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：https://iz.zhonguo6118.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：https://gz.zhonguo1118.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：https://ep.zhonguo2118.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：https://bz.zhonguo4118.cn

[D25] Set 集合去重与交并差
来源：https://qw.zhonguo2118.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：https://ou.zhonguo5118.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：https://bn.zhonguo3118.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：https://zy.zhonguo5118.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：https://na.zhonguo5118.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：https://th.zhonguo4118.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：https://kb.zhonguo5118.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：https://fj.zhonguo3118.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：https://mi.zhonguo6118.cn

[D26] 数组转字符串
来源：https://ik.zhonguo1118.cn

Py:   ", ".join(map(str, arr))
来源：https://xq.zhonguo1118.cn

PHP:  implode(", ", $arr);
来源：https://hh.zhonguo3118.cn

JS:   arr.join(", ")
来源：https://hv.zhonguo5118.cn

TS:   arr.join(", ")
来源：https://af.zhonguo2118.cn

Java: String.join(", ", list)
来源：https://zl.zhonguo3118.cn

Go:   strings.Join(strs, ", ")
来源：https://lx.zhonguo7118.cn

Ruby: arr.join(", ")
来源：https://ne.zhonguo1118.cn

C#:   string.Join(", ", list)
来源：https://jd.zhonguo3118.cn

================================================================================
来源：https://ma.zhonguo7118.cn

E. 字符串处理
来源：https://el.zhonguo2118.cn

================================================================================
来源：https://ml.zhonguo3118.cn

[E01] 拼接字符串
来源：https://bl.zhonguo2118.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：https://ru.zhonguo4118.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：https://cd.zhonguo5118.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：https://er.zhonguo3118.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：https://rq.zhonguo4118.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：https://qn.zhonguo6118.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：https://wf.zhonguo7118.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：https://vj.zhonguo6118.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：https://zm.zhonguo1118.cn

[E02] 重复字符串
来源：https://sm.zhonguo8118.cn

Py:   "ab" * 3
来源：https://fn.zhonguo3118.cn

PHP:  str_repeat("ab", 3);
来源：https://jb.zhonguo1118.cn

JS:   "ab".repeat(3)
来源：https://om.zhonguo4118.cn

TS:   "ab".repeat(3)
来源：https://xi.zhonguo4118.cn

Java: "ab".repeat(3)
来源：https://hk.zhonguo6118.cn

Go:   strings.Repeat("ab", 3)
来源：https://ao.zhonguo7118.cn

Ruby: "ab" * 3
来源：https://as.zhonguo3118.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：https://ao.zhonguo4118.cn

[E03] 截取子串
来源：https://hy.zhonguo3118.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：https://ra.zhonguo3118.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：https://qg.zhonguo5118.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：https://jq.zhonguo7118.cn

TS:   s.slice(1, 4)
来源：https://vk.zhonguo7118.cn

Java: s.substring(1, 4)
来源：https://pg.zhonguo8118.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：https://ug.zhonguo4118.cn

Ruby: s[1, 3];  s[1..3]
来源：https://ix.zhonguo3118.cn

C#:   s.Substring(1, 3)
来源：https://xl.zhonguo4118.cn

[E04] 查找子串位置
来源：https://xp.zhonguo6118.cn

Py:   s.find("x");  s.index("x")
来源：https://vb.zhonguo5118.cn

PHP:  strpos($s, "x");
来源：https://cp.zhonguo4118.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：https://nt.zhonguo5118.cn

TS:   s.indexOf("x")
来源：https://fw.zhonguo6118.cn

Java: s.indexOf("x")
来源：https://gl.zhonguo2118.cn


<!-- 参考信息 -->