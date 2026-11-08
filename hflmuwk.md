代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：https://is.zhonguo5118.cn

Go:   func add(a, b int) int
来源：https://zk.zhonguo7118.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：https://nj.zhonguo6118.cn

C#:   int Add(int a, int b) => a + b;
来源：https://tu.zhonguo2118.cn

[C14] 泛型函数
来源：https://pw.zhonguo5118.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：https://ym.zhonguo2118.cn

PHP:  // 无泛型
来源：https://xw.zhonguo3118.cn

JS:   // 无泛型
来源：https://ba.zhonguo6118.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：https://fe.zhonguo3118.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：https://re.zhonguo5118.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：https://zq.zhonguo2118.cn

Ruby: # 无泛型
来源：https://qy.zhonguo8118.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：https://ud.zhonguo5118.cn

[C15] 解构 / 展开参数
来源：https://rn.zhonguo4118.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：https://ma.zhonguo5118.cn

PHP:  [$a, $b] = $pair;
来源：https://wk.zhonguo5118.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：https://dr.zhonguo1118.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：https://ep.zhonguo1118.cn

Java: // 无解构
来源：https://il.zhonguo8118.cn

Go:   // 无解构
来源：https://hb.zhonguo1118.cn

Ruby: a, b = pair
来源：https://uy.zhonguo4118.cn

C#:   var (a, b) = pair;
来源：https://od.zhonguo8118.cn

[C16] 函数 / 方法重载
来源：https://zk.zhonguo3118.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：https://dx.zhonguo8118.cn

PHP:  // 无重载
来源：https://em.zhonguo7118.cn

JS:   // 无重载：靠 arguments.length 分支
来源：https://pn.zhonguo2118.cn

TS:   // 用联合类型或重载签名声明
来源：https://vx.zhonguo4118.cn

Java: void f(int a) {}  void f(String a) {}
来源：https://fz.zhonguo1118.cn

Go:   // 无重载：用不同函数名
来源：https://lq.zhonguo1118.cn

Ruby: # 无重载：靠动态参数
来源：https://fs.zhonguo5118.cn

C#:   void F(int a) {}  void F(string a) {}
来源：https://bt.zhonguo3118.cn

================================================================================
来源：https://pu.zhonguo7118.cn

D. 数组 / 列表 / 集合
来源：https://pc.zhonguo4118.cn

================================================================================
来源：https://mn.zhonguo4118.cn

[D01] 创建数组 / 列表
来源：https://ir.zhonguo6118.cn

Py:   arr = [1, 2, 3];  empty = []
来源：https://mj.zhonguo1118.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：https://uw.zhonguo5118.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：https://sb.zhonguo5118.cn

TS:   const arr: number[] = [1, 2, 3];
来源：https://zs.zhonguo3118.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：https://yv.zhonguo2118.cn

Go:   arr := []int{1, 2, 3}
来源：https://gs.zhonguo1118.cn

Ruby: arr = [1, 2, 3]
来源：https://jy.zhonguo6118.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：https://uc.zhonguo2118.cn

[D02] 追加元素到末尾
来源：https://sd.zhonguo6118.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：https://yd.zhonguo5118.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：https://rf.zhonguo4118.cn

JS:   arr.push(4);
来源：https://cp.zhonguo2118.cn

TS:   arr.push(4);
来源：https://gp.zhonguo5118.cn

Java: list.add(4);
来源：https://tp.zhonguo1118.cn

Go:   arr = append(arr, 4)
来源：https://bc.zhonguo7118.cn

Ruby: arr << 4; arr.push(5)
来源：https://is.zhonguo2118.cn

C#:   list.Add(4);
来源：https://xm.zhonguo6118.cn

[D03] 在指定位置插入元素
来源：https://tx.zhonguo5118.cn

Py:   arr.insert(0, 0)
来源：https://fy.zhonguo8118.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：https://fy.zhonguo4118.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：https://xl.zhonguo4118.cn

TS:   arr.splice(0, 0, 0);
来源：https://wb.zhonguo8118.cn

Java: list.add(0, 0);
来源：https://xp.zhonguo5118.cn

Go:   arr = append([]int{0}, arr...)
来源：https://hy.zhonguo3118.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：https://br.zhonguo6118.cn

C#:   list.Insert(0, 0);
来源：https://dc.zhonguo5118.cn

[D04] 删除元素
来源：https://op.zhonguo6118.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：https://se.zhonguo4118.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：https://tg.zhonguo5118.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：https://yx.zhonguo4118.cn

TS:   arr.splice(0, 1);
来源：https://wa.zhonguo3118.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：https://za.zhonguo3118.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：https://rf.zhonguo2118.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：https://bh.zhonguo6118.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：https://oi.zhonguo2118.cn

[D05] 访问与修改元素
来源：https://zj.zhonguo4118.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：https://gc.zhonguo5118.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：https://lp.zhonguo6118.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：https://mf.zhonguo5118.cn

TS:   arr[0]; arr.at(-1);
来源：https://ky.zhonguo7118.cn

Java: list.get(0); list.set(0, 9);
来源：https://us.zhonguo1118.cn

Go:   arr[0]; arr[0] = 9
来源：https://yn.zhonguo4118.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：https://kb.zhonguo2118.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：https://qz.zhonguo6118.cn

[D06] 数组长度
来源：https://yk.zhonguo6118.cn

Py:   len(arr)
来源：https://az.zhonguo1118.cn

PHP:  count($arr);
来源：https://tf.zhonguo6118.cn

JS:   arr.length
来源：https://gr.zhonguo3118.cn

TS:   arr.length
来源：https://wg.zhonguo5118.cn

Java: list.size();
来源：https://bi.zhonguo5118.cn

Go:   len(arr)
来源：https://kd.zhonguo1118.cn

Ruby: arr.length; arr.size
来源：https://uw.zhonguo3118.cn

C#:   list.Count;
来源：https://ln.zhonguo7118.cn

[D07] 切片 / 取子数组
来源：https://ba.zhonguo6118.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：https://vk.zhonguo3118.cn

PHP:  array_slice($arr, 1, 3);
来源：https://bo.zhonguo4118.cn

JS:   arr.slice(1, 4);
来源：https://or.zhonguo5118.cn

TS:   arr.slice(1, 4);
来源：https://xr.zhonguo7118.cn

Java: list.subList(1, 4);
来源：https://gk.zhonguo8118.cn

Go:   arr[1:4]
来源：https://nh.zhonguo8118.cn

Ruby: arr[1, 3]
来源：https://ke.zhonguo5118.cn

C#:   list.GetRange(1, 3);
来源：https://mq.zhonguo2118.cn

[D08] 合并两个数组
来源：https://nw.zhonguo2118.cn

Py:   a + b;  a.extend(b)
来源：https://gv.zhonguo4118.cn

PHP:  array_merge($a, $b);
来源：https://zc.zhonguo2118.cn

JS:   [...a, ...b];  a.concat(b);
来源：https://bp.zhonguo3118.cn

TS:   [...a, ...b];
来源：https://mo.zhonguo4118.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：https://iz.zhonguo7118.cn

Go:   append(a, b...)
来源：https://ca.zhonguo2118.cn

Ruby: a + b;  a.concat(b)
来源：https://oc.zhonguo8118.cn

C#:   a.Concat(b).ToList()
来源：https://dz.zhonguo5118.cn

[D09] 排序（升序）
来源：https://ki.zhonguo1118.cn

Py:   sorted(arr);  arr.sort()
来源：https://jw.zhonguo5118.cn

PHP:  sort($arr);
来源：https://vi.zhonguo3118.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：https://sy.zhonguo6118.cn

TS:   [...arr].sort((x, y) => x - y);
来源：https://qk.zhonguo4118.cn

Java: Collections.sort(list);  list.sort(null);
来源：https://xh.zhonguo6118.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：https://jk.zhonguo6118.cn

Ruby: arr.sort
来源：https://xm.zhonguo7118.cn

C#:   list.Sort();
来源：https://ys.zhonguo6118.cn

[D10] 自定义排序（按字段 / 多条件）
来源：https://no.zhonguo3118.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：https://xt.zhonguo8118.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://nf.zhonguo7118.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：https://bn.zhonguo2118.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：https://ar.zhonguo8118.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：https://xi.zhonguo2118.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：https://cz.zhonguo3118.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：https://wq.zhonguo7118.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：https://cx.zhonguo3118.cn

[D11] 反转数组
来源：https://cs.zhonguo6118.cn

Py:   arr[::-1];  arr.reverse()
来源：https://jg.zhonguo8118.cn

PHP:  array_reverse($arr);
来源：https://gl.zhonguo7118.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：https://kl.zhonguo3118.cn

TS:   [...arr].reverse();
来源：https://kk.zhonguo7118.cn

Java: Collections.reverse(list);
来源：https://ru.zhonguo3118.cn

Go:   slices.Reverse(arr)
来源：https://tc.zhonguo5118.cn

Ruby: arr.reverse
来源：https://tm.zhonguo4118.cn

C#:   list.Reverse();
来源：https://en.zhonguo2118.cn

[D12] 查找元素下标
来源：https://xf.zhonguo2118.cn

Py:   arr.index(x);  x in arr
来源：https://lp.zhonguo6118.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：https://qg.zhonguo1118.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://ps.zhonguo1118.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://yr.zhonguo3118.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：https://bl.zhonguo5118.cn

Go:   slices.Index(arr, x)
来源：https://yq.zhonguo2118.cn

Ruby: arr.index(x)
来源：https://ps.zhonguo2118.cn

C#:   list.IndexOf(x);
来源：https://ta.zhonguo6118.cn

[D13] 过滤（保留满足条件的）
来源：https://gx.zhonguo6118.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：https://vu.zhonguo3118.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：https://os.zhonguo5118.cn

JS:   arr.filter(x => x > 3)
来源：https://fa.zhonguo2118.cn

TS:   arr.filter(x => x > 3)
来源：https://eo.zhonguo6118.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：https://uy.zhonguo7118.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：https://vd.zhonguo5118.cn

Ruby: arr.select { |x| x > 3 }
来源：https://vs.zhonguo8118.cn

C#:   list.Where(x => x > 3).ToList()
来源：https://fa.zhonguo1118.cn

[D14] 映射转换（每个元素变形）
来源：https://gu.zhonguo1118.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：https://mc.zhonguo3118.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：https://wh.zhonguo7118.cn

JS:   arr.map(x => x * 2)
来源：https://fj.zhonguo8118.cn

TS:   arr.map(x => x * 2)
来源：https://ch.zhonguo4118.cn

Java: list.stream().map(x -> x * 2).toList()
来源：https://rv.zhonguo4118.cn

Go:   // 手写循环
来源：https://nu.zhonguo8118.cn

Ruby: arr.map { |x| x * 2 }
来源：https://cq.zhonguo7118.cn

C#:   list.Select(x => x * 2).ToList()
来源：https://wj.zhonguo5118.cn

[D15] 去重
来源：https://ow.zhonguo6118.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：https://rt.zhonguo4118.cn

PHP:  array_unique($arr);
来源：https://yu.zhonguo3118.cn

JS:   [...new Set(arr)]
来源：https://tu.zhonguo7118.cn

TS:   [...new Set(arr)]
来源：https://zy.zhonguo7118.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：https://wk.zhonguo6118.cn

Go:   // 用 map[T]struct{} 手写
来源：https://qn.zhonguo1118.cn

Ruby: arr.uniq
来源：https://wr.zhonguo2118.cn

C#:   list.Distinct().ToList()
来源：https://lo.zhonguo6118.cn

[D16] 求和与平均值
来源：https://vd.zhonguo7118.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：https://jx.zhonguo5118.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：https://ru.zhonguo8118.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：https://dx.zhonguo2118.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：https://bl.zhonguo8118.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：https://yn.zhonguo6118.cn

Go:   // 手写循环累加
来源：https://xy.zhonguo4118.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：https://ho.zhonguo6118.cn

C#:   list.Sum();  list.Average()
来源：https://ej.zhonguo2118.cn

[D17] 最大值与最小值
来源：https://lm.zhonguo4118.cn

Py:   max(arr);  min(arr)
来源：https://hv.zhonguo1118.cn

PHP:  max($arr);  min($arr);
来源：https://rc.zhonguo4118.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：https://pp.zhonguo7118.cn

TS:   Math.max(...arr);
来源：https://og.zhonguo2118.cn

Java: Collections.max(list);  Collections.min(list);
来源：https://fw.zhonguo4118.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：https://px.zhonguo7118.cn

Ruby: arr.max;  arr.min
来源：https://wq.zhonguo8118.cn

C#:   list.Max();  list.Min()
来源：https://xz.zhonguo6118.cn

[D18] 扁平化嵌套数组
来源：https://sq.zhonguo5118.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：https://st.zhonguo6118.cn

PHP:  array_merge(...$nested);
来源：https://mh.zhonguo6118.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：https://pm.zhonguo3118.cn

TS:   nested.flat();
来源：https://us.zhonguo4118.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：https://lu.zhonguo6118.cn

Go:   // 手写双层循环
来源：https://cv.zhonguo8118.cn

Ruby: nested.flatten
来源：https://ph.zhonguo7118.cn

C#:   nested.SelectMany(x => x).ToList()
来源：https://jw.zhonguo4118.cn

[D19] 按字段分组
来源：https://on.zhonguo2118.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：https://fa.zhonguo7118.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：https://rm.zhonguo1118.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：https://ds.zhonguo5118.cn

TS:   Object.groupBy(arr, x => x.type)
来源：https://dr.zhonguo2118.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：https://wh.zhonguo3118.cn

Go:   // 手写 map[string][]T
来源：https://xy.zhonguo7118.cn

Ruby: arr.group_by { |x| x[:type] }
来源：https://by.zhonguo7118.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：https://zz.zhonguo4118.cn

[D20] 统计每个元素出现次数
来源：https://vx.zhonguo1118.cn

Py:   Counter(arr)
来源：https://xr.zhonguo8118.cn

PHP:  array_count_values($arr);
来源：https://aj.zhonguo8118.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://bo.zhonguo3118.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://si.zhonguo1118.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：https://tn.zhonguo5118.cn

Go:   // 手写 map[T]int
来源：https://jn.zhonguo3118.cn

Ruby: arr.tally
来源：https://fp.zhonguo6118.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：https://dl.zhonguo2118.cn

[D21] 判断是否包含某元素
来源：https://bl.zhonguo6118.cn

Py:   x in arr
来源：https://rd.zhonguo1118.cn

PHP:  in_array($x, $arr, true);
来源：https://ds.zhonguo1118.cn

JS:   arr.includes(x)
来源：https://hp.zhonguo8118.cn

TS:   arr.includes(x)
来源：https://fj.zhonguo2118.cn

Java: list.contains(x)
来源：https://yo.zhonguo5118.cn

Go:   slices.Contains(arr, x)
来源：https://dg.zhonguo2118.cn

Ruby: arr.include?(x)
来源：https://bz.zhonguo8118.cn

C#:   list.Contains(x)
来源：https://yx.zhonguo3118.cn

[D22] 复制数组（避免共享引用）
来源：https://ws.zhonguo6118.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：https://ds.zhonguo2118.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：https://ia.zhonguo3118.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：https://qf.zhonguo5118.cn

TS:   [...arr];
来源：https://zi.zhonguo4118.cn

Java: new ArrayList<>(list);
来源：https://bf.zhonguo3118.cn

Go:   copied := append([]int(nil), arr...)
来源：https://tf.zhonguo8118.cn

Ruby: arr.dup;  arr.clone
来源：https://vh.zhonguo4118.cn

C#:   new List<int>(list);
来源：https://lx.zhonguo1118.cn

[D23] reduce 累积计算
来源：https://rp.zhonguo8118.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：https://sv.zhonguo6118.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：https://vs.zhonguo8118.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://md.zhonguo7118.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://on.zhonguo5118.cn

Java: list.stream().reduce(0, Integer::sum)
来源：https://we.zhonguo3118.cn

Go:   // 手写循环
来源：https://ae.zhonguo3118.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：https://ic.zhonguo8118.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：https://pv.zhonguo8118.cn

[D24] 字典 / Map 基本操作
来源：https://ln.zhonguo1118.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：https://iy.zhonguo5118.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：https://ls.zhonguo1118.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：https://wa.zhonguo5118.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：https://gk.zhonguo7118.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：https://bj.zhonguo5118.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：https://vm.zhonguo8118.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：https://pa.zhonguo8118.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：https://gf.zhonguo5118.cn

[D25] Set 集合去重与交并差
来源：https://xp.zhonguo8118.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：https://zv.zhonguo5118.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：https://az.zhonguo1118.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：https://ef.zhonguo1118.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：https://ri.zhonguo7118.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：https://rv.zhonguo7118.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：https://wp.zhonguo8118.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：https://qn.zhonguo8118.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：https://pm.zhonguo8118.cn

[D26] 数组转字符串
来源：https://za.zhonguo4118.cn

Py:   ", ".join(map(str, arr))
来源：https://kk.zhonguo2118.cn

PHP:  implode(", ", $arr);
来源：https://hq.zhonguo8118.cn

JS:   arr.join(", ")
来源：https://np.zhonguo4118.cn

TS:   arr.join(", ")
来源：https://wm.zhonguo5118.cn

Java: String.join(", ", list)
来源：https://vp.zhonguo4118.cn

Go:   strings.Join(strs, ", ")
来源：https://qx.zhonguo7118.cn

Ruby: arr.join(", ")
来源：https://vs.zhonguo8118.cn

C#:   string.Join(", ", list)
来源：https://sd.zhonguo4118.cn

================================================================================
来源：https://nx.zhonguo7118.cn

E. 字符串处理
来源：https://qv.zhonguo6118.cn

================================================================================
来源：https://vv.zhonguo6118.cn

[E01] 拼接字符串
来源：https://vd.zhonguo2118.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：https://xf.zhonguo6118.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：https://ja.zhonguo1118.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：https://vb.zhonguo1118.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：https://fc.zhonguo5118.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：https://gz.zhonguo8118.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：https://qu.zhonguo5118.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：https://hp.zhonguo1118.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：https://tx.zhonguo4118.cn

[E02] 重复字符串
来源：https://un.zhonguo3118.cn

Py:   "ab" * 3
来源：https://cj.zhonguo4118.cn

PHP:  str_repeat("ab", 3);
来源：https://de.zhonguo5118.cn

JS:   "ab".repeat(3)
来源：https://aq.zhonguo8118.cn

TS:   "ab".repeat(3)
来源：https://cu.zhonguo5118.cn

Java: "ab".repeat(3)
来源：https://me.zhonguo4118.cn

Go:   strings.Repeat("ab", 3)
来源：https://wo.zhonguo1118.cn

Ruby: "ab" * 3
来源：https://zr.zhonguo7118.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：https://id.zhonguo2118.cn

[E03] 截取子串
来源：https://sn.zhonguo6118.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：https://cy.zhonguo6118.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：https://mo.zhonguo5118.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：https://xp.zhonguo5118.cn

TS:   s.slice(1, 4)
来源：https://br.zhonguo2118.cn

Java: s.substring(1, 4)
来源：https://vo.zhonguo4118.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：https://ge.zhonguo2118.cn

Ruby: s[1, 3];  s[1..3]
来源：https://go.zhonguo7118.cn

C#:   s.Substring(1, 3)
来源：https://tt.zhonguo2118.cn

[E04] 查找子串位置
来源：https://ja.zhonguo7118.cn

Py:   s.find("x");  s.index("x")
来源：https://lk.zhonguo3118.cn


<!-- 参考信息 -->