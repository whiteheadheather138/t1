代发 wailian999

[C14] 泛型函数
来源：https://ay.zhonguo5118.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：https://wm.zhonguo6118.cn

PHP:  // 无泛型
来源：https://xd.zhonguo8118.cn

JS:   // 无泛型
来源：https://pp.zhonguo7118.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：https://ci.zhonguo1118.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：https://yr.zhonguo8118.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：https://gy.zhonguo4118.cn

Ruby: # 无泛型
来源：https://wu.zhonguo5118.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：https://le.zhonguo5118.cn

[C15] 解构 / 展开参数
来源：https://io.zhonguo8118.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：https://kv.zhonguo5118.cn

PHP:  [$a, $b] = $pair;
来源：https://bb.zhonguo2118.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：https://rq.zhonguo5118.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：https://cr.zhonguo4118.cn

Java: // 无解构
来源：https://ls.zhonguo7118.cn

Go:   // 无解构
来源：https://vh.zhonguo2118.cn

Ruby: a, b = pair
来源：https://zv.zhonguo7118.cn

C#:   var (a, b) = pair;
来源：https://ld.zhonguo2118.cn

[C16] 函数 / 方法重载
来源：https://ww.zhonguo6118.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：https://yg.zhonguo1118.cn

PHP:  // 无重载
来源：https://jx.zhonguo5118.cn

JS:   // 无重载：靠 arguments.length 分支
来源：https://tk.zhonguo8118.cn

TS:   // 用联合类型或重载签名声明
来源：https://kv.zhonguo2118.cn

Java: void f(int a) {}  void f(String a) {}
来源：https://np.zhonguo4118.cn

Go:   // 无重载：用不同函数名
来源：https://eg.zhonguo3118.cn

Ruby: # 无重载：靠动态参数
来源：https://mv.zhonguo7118.cn

C#:   void F(int a) {}  void F(string a) {}
来源：https://ck.zhonguo7118.cn

================================================================================
来源：https://kd.zhonguo6118.cn

D. 数组 / 列表 / 集合
来源：https://gg.zhonguo5118.cn

================================================================================
来源：https://ja.zhonguo6118.cn

[D01] 创建数组 / 列表
来源：https://ir.zhonguo1118.cn

Py:   arr = [1, 2, 3];  empty = []
来源：https://yj.zhonguo8118.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：https://gq.zhonguo4118.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：https://cp.zhonguo6118.cn

TS:   const arr: number[] = [1, 2, 3];
来源：https://xc.zhonguo3118.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：https://zb.zhonguo1118.cn

Go:   arr := []int{1, 2, 3}
来源：https://vd.zhonguo5118.cn

Ruby: arr = [1, 2, 3]
来源：https://dj.zhonguo7118.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：https://lx.zhonguo6118.cn

[D02] 追加元素到末尾
来源：https://hm.zhonguo8118.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：https://up.zhonguo5118.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：https://dy.zhonguo6118.cn

JS:   arr.push(4);
来源：https://dh.zhonguo5118.cn

TS:   arr.push(4);
来源：https://ua.zhonguo1118.cn

Java: list.add(4);
来源：https://fq.zhonguo2118.cn

Go:   arr = append(arr, 4)
来源：https://fw.zhonguo4118.cn

Ruby: arr << 4; arr.push(5)
来源：https://rg.zhonguo1118.cn

C#:   list.Add(4);
来源：https://sy.zhonguo4118.cn

[D03] 在指定位置插入元素
来源：https://uu.zhonguo1118.cn

Py:   arr.insert(0, 0)
来源：https://gl.zhonguo6118.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：https://rp.zhonguo4118.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：https://je.zhonguo1118.cn

TS:   arr.splice(0, 0, 0);
来源：https://kg.zhonguo5118.cn

Java: list.add(0, 0);
来源：https://ek.zhonguo8118.cn

Go:   arr = append([]int{0}, arr...)
来源：https://bq.zhonguo5118.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：https://ae.zhonguo4118.cn

C#:   list.Insert(0, 0);
来源：https://pd.zhonguo4118.cn

[D04] 删除元素
来源：https://wq.zhonguo2118.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：https://ef.zhonguo4118.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：https://ya.zhonguo2118.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：https://wb.zhonguo5118.cn

TS:   arr.splice(0, 1);
来源：https://sj.zhonguo8118.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：https://gr.zhonguo5118.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：https://rt.zhonguo2118.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：https://pt.zhonguo2118.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：https://vm.zhonguo5118.cn

[D05] 访问与修改元素
来源：https://zx.zhonguo3118.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：https://jy.zhonguo4118.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：https://kk.zhonguo8118.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：https://kz.zhonguo3118.cn

TS:   arr[0]; arr.at(-1);
来源：https://qc.zhonguo6118.cn

Java: list.get(0); list.set(0, 9);
来源：https://uj.zhonguo5118.cn

Go:   arr[0]; arr[0] = 9
来源：https://iz.zhonguo2118.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：https://eh.zhonguo1118.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：https://dh.zhonguo7118.cn

[D06] 数组长度
来源：https://gl.zhonguo5118.cn

Py:   len(arr)
来源：https://fv.zhonguo3118.cn

PHP:  count($arr);
来源：https://gx.zhonguo7118.cn

JS:   arr.length
来源：https://uh.zhonguo2118.cn

TS:   arr.length
来源：https://ww.zhonguo5118.cn

Java: list.size();
来源：https://ov.zhonguo1118.cn

Go:   len(arr)
来源：https://bu.zhonguo7118.cn

Ruby: arr.length; arr.size
来源：https://mj.zhonguo1118.cn

C#:   list.Count;
来源：https://mg.zhonguo6118.cn

[D07] 切片 / 取子数组
来源：https://az.zhonguo1118.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：https://zb.zhonguo3118.cn

PHP:  array_slice($arr, 1, 3);
来源：https://tf.zhonguo5118.cn

JS:   arr.slice(1, 4);
来源：https://ci.zhonguo3118.cn

TS:   arr.slice(1, 4);
来源：https://gv.zhonguo1118.cn

Java: list.subList(1, 4);
来源：https://ox.zhonguo5118.cn

Go:   arr[1:4]
来源：https://sg.zhonguo2118.cn

Ruby: arr[1, 3]
来源：https://tm.zhonguo7118.cn

C#:   list.GetRange(1, 3);
来源：https://wh.zhonguo4118.cn

[D08] 合并两个数组
来源：https://ri.zhonguo5118.cn

Py:   a + b;  a.extend(b)
来源：https://sn.zhonguo1118.cn

PHP:  array_merge($a, $b);
来源：https://rv.zhonguo8118.cn

JS:   [...a, ...b];  a.concat(b);
来源：https://xt.zhonguo3118.cn

TS:   [...a, ...b];
来源：https://la.zhonguo6118.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：https://st.zhonguo2118.cn

Go:   append(a, b...)
来源：https://kn.zhonguo4118.cn

Ruby: a + b;  a.concat(b)
来源：https://fa.zhonguo4118.cn

C#:   a.Concat(b).ToList()
来源：https://ik.zhonguo1118.cn

[D09] 排序（升序）
来源：https://io.zhonguo7118.cn

Py:   sorted(arr);  arr.sort()
来源：https://bh.zhonguo2118.cn

PHP:  sort($arr);
来源：https://mk.zhonguo5118.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：https://zo.zhonguo1118.cn

TS:   [...arr].sort((x, y) => x - y);
来源：https://zw.zhonguo6118.cn

Java: Collections.sort(list);  list.sort(null);
来源：https://tq.zhonguo1118.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：https://ev.zhonguo8118.cn

Ruby: arr.sort
来源：https://wm.zhonguo8118.cn

C#:   list.Sort();
来源：https://bo.zhonguo1118.cn

[D10] 自定义排序（按字段 / 多条件）
来源：https://mg.zhonguo4118.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：https://na.zhonguo3118.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://nc.zhonguo4118.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：https://uz.zhonguo8118.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：https://zd.zhonguo4118.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：https://dk.zhonguo7118.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：https://ja.zhonguo4118.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：https://it.zhonguo8118.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：https://zs.zhonguo7118.cn

[D11] 反转数组
来源：https://py.zhonguo6118.cn

Py:   arr[::-1];  arr.reverse()
来源：https://hu.zhonguo1118.cn

PHP:  array_reverse($arr);
来源：https://we.zhonguo5118.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：https://zf.zhonguo2118.cn

TS:   [...arr].reverse();
来源：https://qs.zhonguo8118.cn

Java: Collections.reverse(list);
来源：https://ep.zhonguo5118.cn

Go:   slices.Reverse(arr)
来源：https://tz.zhonguo7118.cn

Ruby: arr.reverse
来源：https://xj.zhonguo7118.cn

C#:   list.Reverse();
来源：https://eh.zhonguo4118.cn

[D12] 查找元素下标
来源：https://hl.zhonguo4118.cn

Py:   arr.index(x);  x in arr
来源：https://ma.zhonguo3118.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：https://il.zhonguo4118.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://fp.zhonguo2118.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://mm.zhonguo5118.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：https://zn.zhonguo8118.cn

Go:   slices.Index(arr, x)
来源：https://hy.zhonguo6118.cn

Ruby: arr.index(x)
来源：https://bo.zhonguo3118.cn

C#:   list.IndexOf(x);
来源：https://ic.zhonguo2118.cn

[D13] 过滤（保留满足条件的）
来源：https://az.zhonguo6118.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：https://oo.zhonguo7118.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：https://rg.zhonguo5118.cn

JS:   arr.filter(x => x > 3)
来源：https://hv.zhonguo7118.cn

TS:   arr.filter(x => x > 3)
来源：https://yz.zhonguo5118.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：https://xi.zhonguo2118.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：https://wo.zhonguo5118.cn

Ruby: arr.select { |x| x > 3 }
来源：https://eg.zhonguo1118.cn

C#:   list.Where(x => x > 3).ToList()
来源：https://gf.zhonguo2118.cn

[D14] 映射转换（每个元素变形）
来源：https://tb.zhonguo5118.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：https://we.zhonguo3118.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：https://ft.zhonguo7118.cn

JS:   arr.map(x => x * 2)
来源：https://fk.zhonguo4118.cn

TS:   arr.map(x => x * 2)
来源：https://ls.zhonguo7118.cn

Java: list.stream().map(x -> x * 2).toList()
来源：https://ew.zhonguo4118.cn

Go:   // 手写循环
来源：https://bb.zhonguo3118.cn

Ruby: arr.map { |x| x * 2 }
来源：https://rt.zhonguo7118.cn

C#:   list.Select(x => x * 2).ToList()
来源：https://jm.zhonguo5118.cn

[D15] 去重
来源：https://yw.zhonguo5118.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：https://wn.zhonguo8118.cn

PHP:  array_unique($arr);
来源：https://sy.zhonguo1118.cn

JS:   [...new Set(arr)]
来源：https://mu.zhonguo3118.cn

TS:   [...new Set(arr)]
来源：https://ga.zhonguo7118.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：https://ic.zhonguo8118.cn

Go:   // 用 map[T]struct{} 手写
来源：https://pi.zhonguo3118.cn

Ruby: arr.uniq
来源：https://wl.zhonguo8118.cn

C#:   list.Distinct().ToList()
来源：https://ho.zhonguo1118.cn

[D16] 求和与平均值
来源：https://tz.zhonguo7118.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：https://at.zhonguo6118.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：https://ki.zhonguo1118.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：https://ll.zhonguo7118.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：https://yn.zhonguo8118.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：https://jj.zhonguo5118.cn

Go:   // 手写循环累加
来源：https://xa.zhonguo5118.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：https://at.zhonguo7118.cn

C#:   list.Sum();  list.Average()
来源：https://tz.zhonguo2118.cn

[D17] 最大值与最小值
来源：https://xf.zhonguo8118.cn

Py:   max(arr);  min(arr)
来源：https://vv.zhonguo3118.cn

PHP:  max($arr);  min($arr);
来源：https://jb.zhonguo6118.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：https://bq.zhonguo5118.cn

TS:   Math.max(...arr);
来源：https://rs.zhonguo2118.cn

Java: Collections.max(list);  Collections.min(list);
来源：https://nf.zhonguo4118.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：https://hc.zhonguo5118.cn

Ruby: arr.max;  arr.min
来源：https://ba.zhonguo7118.cn

C#:   list.Max();  list.Min()
来源：https://bd.zhonguo3118.cn

[D18] 扁平化嵌套数组
来源：https://me.zhonguo8118.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：https://fk.zhonguo4118.cn

PHP:  array_merge(...$nested);
来源：https://ge.zhonguo2118.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：https://fj.zhonguo7118.cn

TS:   nested.flat();
来源：https://aj.zhonguo7118.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：https://dm.zhonguo2118.cn

Go:   // 手写双层循环
来源：https://hm.zhonguo1118.cn

Ruby: nested.flatten
来源：https://ij.zhonguo1118.cn

C#:   nested.SelectMany(x => x).ToList()
来源：https://cb.zhonguo1118.cn

[D19] 按字段分组
来源：https://kd.zhonguo8118.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：https://zx.zhonguo6118.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：https://te.zhonguo6118.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：https://lh.zhonguo5118.cn

TS:   Object.groupBy(arr, x => x.type)
来源：https://gx.zhonguo2118.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：https://rc.zhonguo6118.cn

Go:   // 手写 map[string][]T
来源：https://dl.zhonguo1118.cn

Ruby: arr.group_by { |x| x[:type] }
来源：https://rm.zhonguo4118.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：https://af.zhonguo7118.cn

[D20] 统计每个元素出现次数
来源：https://fk.zhonguo6118.cn

Py:   Counter(arr)
来源：https://oq.zhonguo6118.cn

PHP:  array_count_values($arr);
来源：https://tu.zhonguo1118.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://so.zhonguo1118.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://sp.zhonguo6118.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：https://jo.zhonguo7118.cn

Go:   // 手写 map[T]int
来源：https://ud.zhonguo8118.cn

Ruby: arr.tally
来源：https://rb.zhonguo3118.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：https://iy.zhonguo2118.cn

[D21] 判断是否包含某元素
来源：https://by.zhonguo6118.cn

Py:   x in arr
来源：https://tx.zhonguo3118.cn

PHP:  in_array($x, $arr, true);
来源：https://ef.zhonguo7118.cn

JS:   arr.includes(x)
来源：https://je.zhonguo8118.cn

TS:   arr.includes(x)
来源：https://gc.zhonguo2118.cn

Java: list.contains(x)
来源：https://fz.zhonguo8118.cn

Go:   slices.Contains(arr, x)
来源：https://yy.zhonguo7118.cn

Ruby: arr.include?(x)
来源：https://ma.zhonguo6118.cn

C#:   list.Contains(x)
来源：https://gd.zhonguo6118.cn

[D22] 复制数组（避免共享引用）
来源：https://ri.zhonguo2118.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：https://uu.zhonguo3118.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：https://li.zhonguo2118.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：https://wd.zhonguo2118.cn

TS:   [...arr];
来源：https://im.zhonguo7118.cn

Java: new ArrayList<>(list);
来源：https://rf.zhonguo6118.cn

Go:   copied := append([]int(nil), arr...)
来源：https://aa.zhonguo1118.cn

Ruby: arr.dup;  arr.clone
来源：https://fv.zhonguo6118.cn

C#:   new List<int>(list);
来源：https://iq.zhonguo3118.cn

[D23] reduce 累积计算
来源：https://yd.zhonguo4118.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：https://cq.zhonguo7118.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：https://uc.zhonguo7118.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://xq.zhonguo6118.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://gj.zhonguo8118.cn

Java: list.stream().reduce(0, Integer::sum)
来源：https://pa.zhonguo2118.cn

Go:   // 手写循环
来源：https://dg.zhonguo5118.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：https://js.zhonguo3118.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：https://ty.zhonguo6118.cn

[D24] 字典 / Map 基本操作
来源：https://cs.zhonguo1118.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：https://qj.zhonguo1118.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：https://fj.zhonguo7118.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：https://aq.zhonguo3118.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：https://oj.zhonguo6118.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：https://wd.zhonguo6118.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：https://sn.zhonguo4118.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：https://xp.zhonguo3118.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：https://nb.zhonguo5118.cn

[D25] Set 集合去重与交并差
来源：https://ti.zhonguo6118.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：https://pm.zhonguo7118.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：https://rz.zhonguo2118.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：https://ht.zhonguo4118.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：https://ck.zhonguo1118.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：https://zb.zhonguo4118.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：https://ti.zhonguo4118.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：https://pz.zhonguo2118.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：https://cx.zhonguo8118.cn

[D26] 数组转字符串
来源：https://ba.zhonguo1118.cn

Py:   ", ".join(map(str, arr))
来源：https://qn.zhonguo2118.cn

PHP:  implode(", ", $arr);
来源：https://oa.zhonguo1118.cn

JS:   arr.join(", ")
来源：https://kz.zhonguo4118.cn

TS:   arr.join(", ")
来源：https://ae.zhonguo6118.cn

Java: String.join(", ", list)
来源：https://cn.zhonguo6118.cn

Go:   strings.Join(strs, ", ")
来源：https://dx.zhonguo2118.cn

Ruby: arr.join(", ")
来源：https://jk.zhonguo3118.cn

C#:   string.Join(", ", list)
来源：https://ao.zhonguo6118.cn

================================================================================
来源：https://tz.zhonguo8118.cn

E. 字符串处理
来源：https://zu.zhonguo1118.cn

================================================================================
来源：https://lx.zhonguo7118.cn

[E01] 拼接字符串
来源：https://vd.zhonguo1118.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：https://lz.zhonguo5118.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：https://wj.zhonguo1118.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：https://ql.zhonguo7118.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：https://mn.zhonguo4118.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：https://iq.zhonguo3118.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：https://xt.zhonguo5118.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：https://cr.zhonguo7118.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：https://ej.zhonguo5118.cn

[E02] 重复字符串
来源：https://aw.zhonguo7118.cn

Py:   "ab" * 3
来源：https://yv.zhonguo7118.cn

PHP:  str_repeat("ab", 3);
来源：https://uc.zhonguo1118.cn

JS:   "ab".repeat(3)
来源：https://vm.zhonguo2118.cn

TS:   "ab".repeat(3)
来源：https://nn.zhonguo3118.cn

Java: "ab".repeat(3)
来源：https://xz.zhonguo2118.cn

Go:   strings.Repeat("ab", 3)
来源：https://jj.zhonguo5118.cn

Ruby: "ab" * 3
来源：https://hf.zhonguo2118.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：https://xw.zhonguo4118.cn

[E03] 截取子串
来源：https://sz.zhonguo1118.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：https://dl.zhonguo4118.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：https://in.zhonguo2118.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：https://sd.zhonguo7118.cn

TS:   s.slice(1, 4)
来源：https://eq.zhonguo8118.cn

Java: s.substring(1, 4)
来源：https://ns.zhonguo5118.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：https://jt.zhonguo3118.cn

Ruby: s[1, 3];  s[1..3]
来源：https://zi.zhonguo2118.cn

C#:   s.Substring(1, 3)
来源：https://cl.zhonguo7118.cn

[E04] 查找子串位置
来源：https://fh.zhonguo4118.cn

Py:   s.find("x");  s.index("x")
来源：https://ul.zhonguo6118.cn

PHP:  strpos($s, "x");
来源：https://da.zhonguo6118.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：https://sz.zhonguo7118.cn

TS:   s.indexOf("x")
来源：https://yh.zhonguo5118.cn

Java: s.indexOf("x")
来源：https://jb.zhonguo4118.cn


<!-- 参考信息 -->