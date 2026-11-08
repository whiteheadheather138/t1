代发 wailian999

D. 数组 / 列表 / 集合
来源：https://ys.zhonguo3118.cn

================================================================================
来源：https://ms.zhonguo6118.cn

[D01] 创建数组 / 列表
来源：https://xr.zhonguo7118.cn

Py:   arr = [1, 2, 3];  empty = []
来源：https://gt.zhonguo6118.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：https://bf.zhonguo6118.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：https://yn.zhonguo6118.cn

TS:   const arr: number[] = [1, 2, 3];
来源：https://rs.zhonguo3118.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：https://gd.zhonguo3118.cn

Go:   arr := []int{1, 2, 3}
来源：https://qd.zhonguo1118.cn

Ruby: arr = [1, 2, 3]
来源：https://bw.zhonguo4118.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：https://yr.zhonguo8118.cn

[D02] 追加元素到末尾
来源：https://sd.zhonguo4118.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：https://yt.zhonguo8118.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：https://zw.zhonguo5118.cn

JS:   arr.push(4);
来源：https://wy.zhonguo1118.cn

TS:   arr.push(4);
来源：https://vd.zhonguo7118.cn

Java: list.add(4);
来源：https://zj.zhonguo4118.cn

Go:   arr = append(arr, 4)
来源：https://zt.zhonguo2118.cn

Ruby: arr << 4; arr.push(5)
来源：https://wi.zhonguo4118.cn

C#:   list.Add(4);
来源：https://hd.zhonguo7118.cn

[D03] 在指定位置插入元素
来源：https://ps.zhonguo6118.cn

Py:   arr.insert(0, 0)
来源：https://in.zhonguo4118.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：https://rc.zhonguo7118.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：https://fg.zhonguo3118.cn

TS:   arr.splice(0, 0, 0);
来源：https://hs.zhonguo7118.cn

Java: list.add(0, 0);
来源：https://vh.zhonguo4118.cn

Go:   arr = append([]int{0}, arr...)
来源：https://vi.zhonguo8118.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：https://rc.zhonguo5118.cn

C#:   list.Insert(0, 0);
来源：https://jh.zhonguo2118.cn

[D04] 删除元素
来源：https://by.zhonguo2118.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：https://dc.zhonguo6118.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：https://uy.zhonguo4118.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：https://rw.zhonguo2118.cn

TS:   arr.splice(0, 1);
来源：https://ad.zhonguo5118.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：https://ey.zhonguo4118.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：https://iy.zhonguo5118.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：https://bt.zhonguo7118.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：https://kj.zhonguo1118.cn

[D05] 访问与修改元素
来源：https://ez.zhonguo8118.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：https://tb.zhonguo5118.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：https://dq.zhonguo4118.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：https://lv.zhonguo3118.cn

TS:   arr[0]; arr.at(-1);
来源：https://nm.zhonguo7118.cn

Java: list.get(0); list.set(0, 9);
来源：https://dv.zhonguo4118.cn

Go:   arr[0]; arr[0] = 9
来源：https://hx.zhonguo8118.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：https://kp.zhonguo1118.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：https://sw.zhonguo6118.cn

[D06] 数组长度
来源：https://vi.zhonguo2118.cn

Py:   len(arr)
来源：https://vp.zhonguo6118.cn

PHP:  count($arr);
来源：https://xs.zhonguo8118.cn

JS:   arr.length
来源：https://fs.zhonguo7118.cn

TS:   arr.length
来源：https://qw.zhonguo6118.cn

Java: list.size();
来源：https://ci.zhonguo4118.cn

Go:   len(arr)
来源：https://rr.zhonguo8118.cn

Ruby: arr.length; arr.size
来源：https://pl.zhonguo7118.cn

C#:   list.Count;
来源：https://ar.zhonguo3118.cn

[D07] 切片 / 取子数组
来源：https://ts.zhonguo5118.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：https://fo.zhonguo3118.cn

PHP:  array_slice($arr, 1, 3);
来源：https://fu.zhonguo4118.cn

JS:   arr.slice(1, 4);
来源：https://ll.zhonguo5118.cn

TS:   arr.slice(1, 4);
来源：https://ij.zhonguo8118.cn

Java: list.subList(1, 4);
来源：https://iz.zhonguo8118.cn

Go:   arr[1:4]
来源：https://rk.zhonguo7118.cn

Ruby: arr[1, 3]
来源：https://hp.zhonguo4118.cn

C#:   list.GetRange(1, 3);
来源：https://gq.zhonguo6118.cn

[D08] 合并两个数组
来源：https://qg.zhonguo1118.cn

Py:   a + b;  a.extend(b)
来源：https://zs.zhonguo4118.cn

PHP:  array_merge($a, $b);
来源：https://qv.zhonguo5118.cn

JS:   [...a, ...b];  a.concat(b);
来源：https://zr.zhonguo4118.cn

TS:   [...a, ...b];
来源：https://mn.zhonguo3118.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：https://an.zhonguo2118.cn

Go:   append(a, b...)
来源：https://or.zhonguo4118.cn

Ruby: a + b;  a.concat(b)
来源：https://fv.zhonguo4118.cn

C#:   a.Concat(b).ToList()
来源：https://vk.zhonguo4118.cn

[D09] 排序（升序）
来源：https://bu.zhonguo3118.cn

Py:   sorted(arr);  arr.sort()
来源：https://qz.zhonguo4118.cn

PHP:  sort($arr);
来源：https://bt.zhonguo7118.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：https://cb.zhonguo1118.cn

TS:   [...arr].sort((x, y) => x - y);
来源：https://we.zhonguo7118.cn

Java: Collections.sort(list);  list.sort(null);
来源：https://nc.zhonguo8118.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：https://ss.zhonguo1118.cn

Ruby: arr.sort
来源：https://na.zhonguo8118.cn

C#:   list.Sort();
来源：https://ng.zhonguo4118.cn

[D10] 自定义排序（按字段 / 多条件）
来源：https://vd.zhonguo3118.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：https://uy.zhonguo3118.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://wk.zhonguo7118.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：https://jr.zhonguo6118.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：https://lk.zhonguo8118.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：https://lj.zhonguo4118.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：https://oz.zhonguo8118.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：https://dm.zhonguo6118.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：https://eb.zhonguo2118.cn

[D11] 反转数组
来源：https://ln.zhonguo6118.cn

Py:   arr[::-1];  arr.reverse()
来源：https://wh.zhonguo3118.cn

PHP:  array_reverse($arr);
来源：https://tl.zhonguo4118.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：https://nc.zhonguo1118.cn

TS:   [...arr].reverse();
来源：https://hk.zhonguo3118.cn

Java: Collections.reverse(list);
来源：https://ty.zhonguo7118.cn

Go:   slices.Reverse(arr)
来源：https://qn.zhonguo8118.cn

Ruby: arr.reverse
来源：https://zw.zhonguo7118.cn

C#:   list.Reverse();
来源：https://ju.zhonguo4118.cn

[D12] 查找元素下标
来源：https://qm.zhonguo3118.cn

Py:   arr.index(x);  x in arr
来源：https://lk.zhonguo4118.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：https://cr.zhonguo8118.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://es.zhonguo8118.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://cp.zhonguo6118.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：https://gw.zhonguo8118.cn

Go:   slices.Index(arr, x)
来源：https://mm.zhonguo6118.cn

Ruby: arr.index(x)
来源：https://mm.zhonguo3118.cn

C#:   list.IndexOf(x);
来源：https://fn.zhonguo7118.cn

[D13] 过滤（保留满足条件的）
来源：https://ih.zhonguo4118.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：https://sx.zhonguo3118.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：https://tj.zhonguo5118.cn

JS:   arr.filter(x => x > 3)
来源：https://fi.zhonguo7118.cn

TS:   arr.filter(x => x > 3)
来源：https://xn.zhonguo1118.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：https://nc.zhonguo7118.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：https://cj.zhonguo2118.cn

Ruby: arr.select { |x| x > 3 }
来源：https://ua.zhonguo6118.cn

C#:   list.Where(x => x > 3).ToList()
来源：https://em.zhonguo4118.cn

[D14] 映射转换（每个元素变形）
来源：https://bj.zhonguo3118.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：https://go.zhonguo5118.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：https://yk.zhonguo7118.cn

JS:   arr.map(x => x * 2)
来源：https://hb.zhonguo4118.cn

TS:   arr.map(x => x * 2)
来源：https://bq.zhonguo5118.cn

Java: list.stream().map(x -> x * 2).toList()
来源：https://at.zhonguo8118.cn

Go:   // 手写循环
来源：https://yj.zhonguo7118.cn

Ruby: arr.map { |x| x * 2 }
来源：https://lm.zhonguo5118.cn

C#:   list.Select(x => x * 2).ToList()
来源：https://jg.zhonguo1118.cn

[D15] 去重
来源：https://nm.zhonguo6118.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：https://uz.zhonguo1118.cn

PHP:  array_unique($arr);
来源：https://jf.zhonguo5118.cn

JS:   [...new Set(arr)]
来源：https://nq.zhonguo2118.cn

TS:   [...new Set(arr)]
来源：https://ll.zhonguo3118.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：https://fg.zhonguo8118.cn

Go:   // 用 map[T]struct{} 手写
来源：https://ur.zhonguo1118.cn

Ruby: arr.uniq
来源：https://ap.zhonguo2118.cn

C#:   list.Distinct().ToList()
来源：https://fg.zhonguo6118.cn

[D16] 求和与平均值
来源：https://uz.zhonguo4118.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：https://ye.zhonguo6118.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：https://ps.zhonguo2118.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：https://xp.zhonguo5118.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：https://rt.zhonguo1118.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：https://yl.zhonguo5118.cn

Go:   // 手写循环累加
来源：https://mv.zhonguo1118.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：https://ob.zhonguo3118.cn

C#:   list.Sum();  list.Average()
来源：https://gr.zhonguo1118.cn

[D17] 最大值与最小值
来源：https://sn.zhonguo7118.cn

Py:   max(arr);  min(arr)
来源：https://tr.zhonguo7118.cn

PHP:  max($arr);  min($arr);
来源：https://uy.zhonguo7118.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：https://qw.zhonguo4118.cn

TS:   Math.max(...arr);
来源：https://di.zhonguo1118.cn

Java: Collections.max(list);  Collections.min(list);
来源：https://qv.zhonguo6118.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：https://pc.zhonguo4118.cn

Ruby: arr.max;  arr.min
来源：https://hz.zhonguo7118.cn

C#:   list.Max();  list.Min()
来源：https://yj.zhonguo1118.cn

[D18] 扁平化嵌套数组
来源：https://lt.zhonguo4118.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：https://rh.zhonguo2118.cn

PHP:  array_merge(...$nested);
来源：https://dr.zhonguo7118.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：https://ru.zhonguo7118.cn

TS:   nested.flat();
来源：https://ie.zhonguo8118.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：https://qs.zhonguo5118.cn

Go:   // 手写双层循环
来源：https://qn.zhonguo6118.cn

Ruby: nested.flatten
来源：https://iq.zhonguo3118.cn

C#:   nested.SelectMany(x => x).ToList()
来源：https://bi.zhonguo7118.cn

[D19] 按字段分组
来源：https://ys.zhonguo3118.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：https://gc.zhonguo6118.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：https://hm.zhonguo4118.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：https://zh.zhonguo2118.cn

TS:   Object.groupBy(arr, x => x.type)
来源：https://wr.zhonguo3118.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：https://jn.zhonguo8118.cn

Go:   // 手写 map[string][]T
来源：https://ik.zhonguo5118.cn

Ruby: arr.group_by { |x| x[:type] }
来源：https://vv.zhonguo7118.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：https://fm.zhonguo6118.cn

[D20] 统计每个元素出现次数
来源：https://yx.zhonguo3118.cn

Py:   Counter(arr)
来源：https://gl.zhonguo3118.cn

PHP:  array_count_values($arr);
来源：https://xi.zhonguo8118.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://oh.zhonguo7118.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://gr.zhonguo5118.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：https://qc.zhonguo8118.cn

Go:   // 手写 map[T]int
来源：https://rh.zhonguo3118.cn

Ruby: arr.tally
来源：https://cp.zhonguo8118.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：https://qf.zhonguo4118.cn

[D21] 判断是否包含某元素
来源：https://tk.zhonguo8118.cn

Py:   x in arr
来源：https://kk.zhonguo2118.cn

PHP:  in_array($x, $arr, true);
来源：https://sx.zhonguo8118.cn

JS:   arr.includes(x)
来源：https://vv.zhonguo3118.cn

TS:   arr.includes(x)
来源：https://qv.zhonguo5118.cn

Java: list.contains(x)
来源：https://pb.zhonguo4118.cn

Go:   slices.Contains(arr, x)
来源：https://xl.zhonguo6118.cn

Ruby: arr.include?(x)
来源：https://qt.zhonguo2118.cn

C#:   list.Contains(x)
来源：https://vk.zhonguo4118.cn

[D22] 复制数组（避免共享引用）
来源：https://zq.zhonguo6118.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：https://wu.zhonguo2118.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：https://ka.zhonguo4118.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：https://cr.zhonguo8118.cn

TS:   [...arr];
来源：https://wt.zhonguo7118.cn

Java: new ArrayList<>(list);
来源：https://rg.zhonguo2118.cn

Go:   copied := append([]int(nil), arr...)
来源：https://xk.zhonguo2118.cn

Ruby: arr.dup;  arr.clone
来源：https://xz.zhonguo5118.cn

C#:   new List<int>(list);
来源：https://ga.zhonguo7118.cn

[D23] reduce 累积计算
来源：https://gw.zhonguo2118.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：https://ru.zhonguo6118.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：https://ub.zhonguo1118.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://mc.zhonguo3118.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://dw.zhonguo7118.cn

Java: list.stream().reduce(0, Integer::sum)
来源：https://vc.zhonguo1118.cn

Go:   // 手写循环
来源：https://cm.zhonguo4118.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：https://na.zhonguo1118.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：https://qq.zhonguo1118.cn

[D24] 字典 / Map 基本操作
来源：https://gh.zhonguo8118.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：https://vw.zhonguo3118.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：https://gz.zhonguo7118.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：https://un.zhonguo3118.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：https://am.zhonguo2118.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：https://lv.zhonguo3118.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：https://se.zhonguo4118.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：https://yo.zhonguo3118.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：https://us.zhonguo3118.cn

[D25] Set 集合去重与交并差
来源：https://fr.zhonguo7118.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：https://zg.zhonguo4118.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：https://df.zhonguo8118.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：https://jv.zhonguo3118.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：https://pr.zhonguo2118.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：https://mo.zhonguo7118.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：https://dm.zhonguo6118.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：https://qo.zhonguo1118.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：https://xj.zhonguo4118.cn

[D26] 数组转字符串
来源：https://lk.zhonguo4118.cn

Py:   ", ".join(map(str, arr))
来源：https://rr.zhonguo5118.cn

PHP:  implode(", ", $arr);
来源：https://ck.zhonguo1118.cn

JS:   arr.join(", ")
来源：https://ae.zhonguo8118.cn

TS:   arr.join(", ")
来源：https://ke.zhonguo7118.cn

Java: String.join(", ", list)
来源：https://oe.zhonguo1118.cn

Go:   strings.Join(strs, ", ")
来源：https://fi.zhonguo5118.cn

Ruby: arr.join(", ")
来源：https://bn.zhonguo5118.cn

C#:   string.Join(", ", list)
来源：https://qv.zhonguo3118.cn

================================================================================
来源：https://no.zhonguo5118.cn

E. 字符串处理
来源：https://dt.zhonguo4118.cn

================================================================================
来源：https://bc.zhonguo5118.cn

[E01] 拼接字符串
来源：https://vo.zhonguo3118.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：https://jc.zhonguo2118.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：https://pu.zhonguo8118.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：https://ks.zhonguo4118.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：https://wg.zhonguo5118.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：https://bq.zhonguo2118.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：https://qi.zhonguo7118.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：https://yn.zhonguo1118.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：https://ra.zhonguo5118.cn

[E02] 重复字符串
来源：https://sh.zhonguo6118.cn

Py:   "ab" * 3
来源：https://bk.zhonguo8118.cn

PHP:  str_repeat("ab", 3);
来源：https://aj.zhonguo7118.cn

JS:   "ab".repeat(3)
来源：https://wd.zhonguo6118.cn

TS:   "ab".repeat(3)
来源：https://ik.zhonguo1118.cn

Java: "ab".repeat(3)
来源：https://jj.zhonguo2118.cn

Go:   strings.Repeat("ab", 3)
来源：https://hi.zhonguo2118.cn

Ruby: "ab" * 3
来源：https://xr.zhonguo2118.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：https://ci.zhonguo6118.cn

[E03] 截取子串
来源：https://ea.zhonguo3118.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：https://sf.zhonguo6118.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：https://jh.zhonguo5118.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：https://uo.zhonguo3118.cn

TS:   s.slice(1, 4)
来源：https://mu.zhonguo7118.cn

Java: s.substring(1, 4)
来源：https://rk.zhonguo2118.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：https://br.zhonguo2118.cn

Ruby: s[1, 3];  s[1..3]
来源：https://mt.zhonguo8118.cn

C#:   s.Substring(1, 3)
来源：https://vl.zhonguo7118.cn

[E04] 查找子串位置
来源：https://fc.zhonguo7118.cn

Py:   s.find("x");  s.index("x")
来源：https://bk.zhonguo8118.cn

PHP:  strpos($s, "x");
来源：https://zk.zhonguo3118.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：https://xm.zhonguo5118.cn

TS:   s.indexOf("x")
来源：https://ka.zhonguo8118.cn

Java: s.indexOf("x")
来源：https://sf.zhonguo4118.cn

Go:   strings.Index(s, "x")
来源：https://dm.zhonguo3118.cn

Ruby: s.index("x")
来源：https://jy.zhonguo2118.cn

C#:   s.IndexOf("x")
来源：https://wi.zhonguo4118.cn

[E05] 判断包含 / 前缀 / 后缀
来源：https://dj.zhonguo8118.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：https://ms.zhonguo4118.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：https://hk.zhonguo1118.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：https://de.zhonguo4118.cn

TS:   s.includes("x");  s.startsWith("a")
来源：https://eb.zhonguo1118.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：https://se.zhonguo4118.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：https://lv.zhonguo1118.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：https://hj.zhonguo6118.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：https://kj.zhonguo2118.cn

[E06] 替换子串
来源：https://rc.zhonguo8118.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：https://xa.zhonguo1118.cn

PHP:  str_replace("a", "b", $s);
来源：https://qs.zhonguo3118.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://xk.zhonguo3118.cn

TS:   s.replaceAll("a", "b")
来源：https://uv.zhonguo4118.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://tg.zhonguo5118.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：https://iq.zhonguo6118.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：https://zd.zhonguo6118.cn

C#:   s.Replace("a", "b")
来源：https://hg.zhonguo7118.cn

[E07] 按分隔符拆分
来源：https://qb.zhonguo7118.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：https://ew.zhonguo7118.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：https://vk.zhonguo1118.cn

JS:   s.split(",");  s.split(/\s+/)
来源：https://jn.zhonguo4118.cn

TS:   s.split(",")
来源：https://fx.zhonguo3118.cn

Java: s.split(",");  s.split("\\s+")
来源：https://zd.zhonguo8118.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：https://tw.zhonguo6118.cn


<!-- 参考信息 -->