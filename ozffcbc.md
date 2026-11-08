代发 wailian999

Py:   len(arr)
来源：https://mr.zhonguo8118.cn

PHP:  count($arr);
来源：https://db.zhonguo4118.cn

JS:   arr.length
来源：https://np.zhonguo6118.cn

TS:   arr.length
来源：https://iz.zhonguo8118.cn

Java: list.size();
来源：https://tk.zhonguo3118.cn

Go:   len(arr)
来源：https://ig.zhonguo6118.cn

Ruby: arr.length; arr.size
来源：https://rq.zhonguo5118.cn

C#:   list.Count;
来源：https://zl.zhonguo4118.cn

[D07] 切片 / 取子数组
来源：https://rt.zhonguo4118.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：https://zu.zhonguo1118.cn

PHP:  array_slice($arr, 1, 3);
来源：https://hr.zhonguo6118.cn

JS:   arr.slice(1, 4);
来源：https://jt.zhonguo5118.cn

TS:   arr.slice(1, 4);
来源：https://gc.zhonguo3118.cn

Java: list.subList(1, 4);
来源：https://sw.zhonguo6118.cn

Go:   arr[1:4]
来源：https://do.zhonguo6118.cn

Ruby: arr[1, 3]
来源：https://en.zhonguo7118.cn

C#:   list.GetRange(1, 3);
来源：https://dy.zhonguo5118.cn

[D08] 合并两个数组
来源：https://qf.zhonguo3118.cn

Py:   a + b;  a.extend(b)
来源：https://fb.zhonguo6118.cn

PHP:  array_merge($a, $b);
来源：https://fw.zhonguo6118.cn

JS:   [...a, ...b];  a.concat(b);
来源：https://yb.zhonguo5118.cn

TS:   [...a, ...b];
来源：https://bk.zhonguo7118.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：https://kp.zhonguo1118.cn

Go:   append(a, b...)
来源：https://ir.zhonguo6118.cn

Ruby: a + b;  a.concat(b)
来源：https://xp.zhonguo4118.cn

C#:   a.Concat(b).ToList()
来源：https://xo.zhonguo2118.cn

[D09] 排序（升序）
来源：https://zi.zhonguo8118.cn

Py:   sorted(arr);  arr.sort()
来源：https://pw.zhonguo1118.cn

PHP:  sort($arr);
来源：https://by.zhonguo8118.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：https://od.zhonguo6118.cn

TS:   [...arr].sort((x, y) => x - y);
来源：https://dh.zhonguo3118.cn

Java: Collections.sort(list);  list.sort(null);
来源：https://bc.zhonguo1118.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：https://oc.zhonguo5118.cn

Ruby: arr.sort
来源：https://dc.zhonguo5118.cn

C#:   list.Sort();
来源：https://vz.zhonguo8118.cn

[D10] 自定义排序（按字段 / 多条件）
来源：https://yr.zhonguo7118.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：https://ly.zhonguo7118.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://nz.zhonguo4118.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：https://dr.zhonguo1118.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：https://by.zhonguo5118.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：https://qj.zhonguo1118.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：https://pp.zhonguo4118.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：https://vu.zhonguo7118.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：https://bt.zhonguo7118.cn

[D11] 反转数组
来源：https://dc.zhonguo8118.cn

Py:   arr[::-1];  arr.reverse()
来源：https://bs.zhonguo5118.cn

PHP:  array_reverse($arr);
来源：https://cn.zhonguo2118.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：https://hb.zhonguo3118.cn

TS:   [...arr].reverse();
来源：https://gw.zhonguo1118.cn

Java: Collections.reverse(list);
来源：https://rx.zhonguo5118.cn

Go:   slices.Reverse(arr)
来源：https://of.zhonguo4118.cn

Ruby: arr.reverse
来源：https://dx.zhonguo4118.cn

C#:   list.Reverse();
来源：https://bk.zhonguo1118.cn

[D12] 查找元素下标
来源：https://vh.zhonguo5118.cn

Py:   arr.index(x);  x in arr
来源：https://as.zhonguo7118.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：https://oe.zhonguo4118.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://yf.zhonguo8118.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://ly.zhonguo2118.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：https://kd.zhonguo7118.cn

Go:   slices.Index(arr, x)
来源：https://nx.zhonguo5118.cn

Ruby: arr.index(x)
来源：https://va.zhonguo5118.cn

C#:   list.IndexOf(x);
来源：https://dz.zhonguo5118.cn

[D13] 过滤（保留满足条件的）
来源：https://dk.zhonguo2118.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：https://qh.zhonguo2118.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：https://qq.zhonguo4118.cn

JS:   arr.filter(x => x > 3)
来源：https://vb.zhonguo3118.cn

TS:   arr.filter(x => x > 3)
来源：https://tb.zhonguo8118.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：https://ao.zhonguo6118.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：https://tq.zhonguo3118.cn

Ruby: arr.select { |x| x > 3 }
来源：https://zl.zhonguo3118.cn

C#:   list.Where(x => x > 3).ToList()
来源：https://la.zhonguo4118.cn

[D14] 映射转换（每个元素变形）
来源：https://ki.zhonguo4118.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：https://co.zhonguo5118.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：https://fj.zhonguo5118.cn

JS:   arr.map(x => x * 2)
来源：https://wo.zhonguo5118.cn

TS:   arr.map(x => x * 2)
来源：https://py.zhonguo8118.cn

Java: list.stream().map(x -> x * 2).toList()
来源：https://tn.zhonguo7118.cn

Go:   // 手写循环
来源：https://qx.zhonguo7118.cn

Ruby: arr.map { |x| x * 2 }
来源：https://kd.zhonguo6118.cn

C#:   list.Select(x => x * 2).ToList()
来源：https://vx.zhonguo4118.cn

[D15] 去重
来源：https://fi.zhonguo5118.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：https://vv.zhonguo5118.cn

PHP:  array_unique($arr);
来源：https://go.zhonguo5118.cn

JS:   [...new Set(arr)]
来源：https://tz.zhonguo6118.cn

TS:   [...new Set(arr)]
来源：https://xm.zhonguo5118.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：https://bm.zhonguo1118.cn

Go:   // 用 map[T]struct{} 手写
来源：https://ng.zhonguo6118.cn

Ruby: arr.uniq
来源：https://do.zhonguo5118.cn

C#:   list.Distinct().ToList()
来源：https://wt.zhonguo6118.cn

[D16] 求和与平均值
来源：https://pe.zhonguo1118.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：https://ov.zhonguo2118.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：https://ka.zhonguo4118.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：https://yd.zhonguo3118.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：https://wz.zhonguo8118.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：https://zt.zhonguo6118.cn

Go:   // 手写循环累加
来源：https://cm.zhonguo2118.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：https://rr.zhonguo5118.cn

C#:   list.Sum();  list.Average()
来源：https://dn.zhonguo1118.cn

[D17] 最大值与最小值
来源：https://jt.zhonguo5118.cn

Py:   max(arr);  min(arr)
来源：https://ji.zhonguo6118.cn

PHP:  max($arr);  min($arr);
来源：https://cp.zhonguo4118.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：https://td.zhonguo8118.cn

TS:   Math.max(...arr);
来源：https://dy.zhonguo6118.cn

Java: Collections.max(list);  Collections.min(list);
来源：https://tq.zhonguo6118.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：https://ty.zhonguo3118.cn

Ruby: arr.max;  arr.min
来源：https://go.zhonguo3118.cn

C#:   list.Max();  list.Min()
来源：https://am.zhonguo3118.cn

[D18] 扁平化嵌套数组
来源：https://ac.zhonguo6118.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：https://ni.zhonguo8118.cn

PHP:  array_merge(...$nested);
来源：https://yv.zhonguo7118.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：https://jz.zhonguo3118.cn

TS:   nested.flat();
来源：https://ex.zhonguo4118.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：https://qu.zhonguo1118.cn

Go:   // 手写双层循环
来源：https://vd.zhonguo4118.cn

Ruby: nested.flatten
来源：https://lb.zhonguo1118.cn

C#:   nested.SelectMany(x => x).ToList()
来源：https://au.zhonguo5118.cn

[D19] 按字段分组
来源：https://dn.zhonguo5118.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：https://hz.zhonguo2118.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：https://qy.zhonguo5118.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：https://md.zhonguo7118.cn

TS:   Object.groupBy(arr, x => x.type)
来源：https://rg.zhonguo5118.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：https://ny.zhonguo7118.cn

Go:   // 手写 map[string][]T
来源：https://gb.zhonguo4118.cn

Ruby: arr.group_by { |x| x[:type] }
来源：https://zk.zhonguo3118.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：https://dm.zhonguo8118.cn

[D20] 统计每个元素出现次数
来源：https://sz.zhonguo6118.cn

Py:   Counter(arr)
来源：https://hx.zhonguo7118.cn

PHP:  array_count_values($arr);
来源：https://ef.zhonguo5118.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://ze.zhonguo5118.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://jl.zhonguo4118.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：https://is.zhonguo7118.cn

Go:   // 手写 map[T]int
来源：https://al.zhonguo1118.cn

Ruby: arr.tally
来源：https://ya.zhonguo3118.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：https://js.zhonguo6118.cn

[D21] 判断是否包含某元素
来源：https://ch.zhonguo3118.cn

Py:   x in arr
来源：https://xy.zhonguo7118.cn

PHP:  in_array($x, $arr, true);
来源：https://ah.zhonguo6118.cn

JS:   arr.includes(x)
来源：https://lx.zhonguo3118.cn

TS:   arr.includes(x)
来源：https://mq.zhonguo6118.cn

Java: list.contains(x)
来源：https://lw.zhonguo8118.cn

Go:   slices.Contains(arr, x)
来源：https://xj.zhonguo3118.cn

Ruby: arr.include?(x)
来源：https://sn.zhonguo6118.cn

C#:   list.Contains(x)
来源：https://es.zhonguo7118.cn

[D22] 复制数组（避免共享引用）
来源：https://uu.zhonguo7118.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：https://yb.zhonguo3118.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：https://ou.zhonguo8118.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：https://gl.zhonguo6118.cn

TS:   [...arr];
来源：https://oe.zhonguo2118.cn

Java: new ArrayList<>(list);
来源：https://kw.zhonguo3118.cn

Go:   copied := append([]int(nil), arr...)
来源：https://kh.zhonguo2118.cn

Ruby: arr.dup;  arr.clone
来源：https://il.zhonguo8118.cn

C#:   new List<int>(list);
来源：https://yx.zhonguo2118.cn

[D23] reduce 累积计算
来源：https://vv.zhonguo4118.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：https://ad.zhonguo1118.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：https://nd.zhonguo8118.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://nr.zhonguo2118.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://kt.zhonguo3118.cn

Java: list.stream().reduce(0, Integer::sum)
来源：https://og.zhonguo5118.cn

Go:   // 手写循环
来源：https://xo.zhonguo4118.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：https://vc.zhonguo6118.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：https://cq.zhonguo3118.cn

[D24] 字典 / Map 基本操作
来源：https://jo.zhonguo8118.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：https://dx.zhonguo3118.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：https://ec.zhonguo7118.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：https://tb.zhonguo5118.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：https://jv.zhonguo6118.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：https://hi.zhonguo4118.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：https://vn.zhonguo6118.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：https://dq.zhonguo5118.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：https://qk.zhonguo1118.cn

[D25] Set 集合去重与交并差
来源：https://vw.zhonguo6118.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：https://kw.zhonguo3118.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：https://us.zhonguo2118.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：https://ly.zhonguo1118.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：https://ou.zhonguo6118.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：https://dt.zhonguo2118.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：https://ds.zhonguo4118.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：https://qa.zhonguo6118.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：https://oa.zhonguo5118.cn

[D26] 数组转字符串
来源：https://vy.zhonguo7118.cn

Py:   ", ".join(map(str, arr))
来源：https://ih.zhonguo6118.cn

PHP:  implode(", ", $arr);
来源：https://fe.zhonguo6118.cn

JS:   arr.join(", ")
来源：https://cg.zhonguo2118.cn

TS:   arr.join(", ")
来源：https://jp.zhonguo7118.cn

Java: String.join(", ", list)
来源：https://ph.zhonguo2118.cn

Go:   strings.Join(strs, ", ")
来源：https://dg.zhonguo5118.cn

Ruby: arr.join(", ")
来源：https://kx.zhonguo1118.cn

C#:   string.Join(", ", list)
来源：https://fl.zhonguo2118.cn

================================================================================
来源：https://hd.zhonguo3118.cn

E. 字符串处理
来源：https://mf.zhonguo2118.cn

================================================================================
来源：https://oq.zhonguo5118.cn

[E01] 拼接字符串
来源：https://te.zhonguo1118.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：https://sg.zhonguo2118.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：https://yn.zhonguo8118.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：https://rj.zhonguo1118.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：https://kg.zhonguo2118.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：https://ji.zhonguo6118.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：https://sr.zhonguo2118.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：https://sz.zhonguo8118.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：https://yr.zhonguo7118.cn

[E02] 重复字符串
来源：https://fi.zhonguo1118.cn

Py:   "ab" * 3
来源：https://mj.zhonguo3118.cn

PHP:  str_repeat("ab", 3);
来源：https://qr.zhonguo2118.cn

JS:   "ab".repeat(3)
来源：https://sv.zhonguo2118.cn

TS:   "ab".repeat(3)
来源：https://ms.zhonguo4118.cn

Java: "ab".repeat(3)
来源：https://ia.zhonguo3118.cn

Go:   strings.Repeat("ab", 3)
来源：https://ko.zhonguo1118.cn

Ruby: "ab" * 3
来源：https://gy.zhonguo6118.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：https://ng.zhonguo3118.cn

[E03] 截取子串
来源：https://dc.zhonguo4118.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：https://od.zhonguo7118.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：https://nh.zhonguo2118.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：https://wv.zhonguo2118.cn

TS:   s.slice(1, 4)
来源：https://qj.zhonguo5118.cn

Java: s.substring(1, 4)
来源：https://zi.zhonguo6118.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：https://yz.zhonguo3118.cn

Ruby: s[1, 3];  s[1..3]
来源：https://hx.zhonguo8118.cn

C#:   s.Substring(1, 3)
来源：https://qu.zhonguo6118.cn

[E04] 查找子串位置
来源：https://uj.zhonguo3118.cn

Py:   s.find("x");  s.index("x")
来源：https://xx.zhonguo2118.cn

PHP:  strpos($s, "x");
来源：https://lf.zhonguo4118.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：https://yw.zhonguo3118.cn

TS:   s.indexOf("x")
来源：https://oy.zhonguo7118.cn

Java: s.indexOf("x")
来源：https://xy.zhonguo6118.cn

Go:   strings.Index(s, "x")
来源：https://wj.zhonguo6118.cn

Ruby: s.index("x")
来源：https://lu.zhonguo1118.cn

C#:   s.IndexOf("x")
来源：https://wm.zhonguo4118.cn

[E05] 判断包含 / 前缀 / 后缀
来源：https://wg.zhonguo4118.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：https://ms.zhonguo1118.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：https://jl.zhonguo4118.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：https://ee.zhonguo5118.cn

TS:   s.includes("x");  s.startsWith("a")
来源：https://js.zhonguo2118.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：https://oh.zhonguo6118.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：https://zm.zhonguo8118.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：https://ek.zhonguo6118.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：https://vf.zhonguo2118.cn

[E06] 替换子串
来源：https://om.zhonguo6118.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：https://sc.zhonguo2118.cn

PHP:  str_replace("a", "b", $s);
来源：https://ks.zhonguo6118.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://id.zhonguo7118.cn

TS:   s.replaceAll("a", "b")
来源：https://kf.zhonguo4118.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://xe.zhonguo8118.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：https://et.zhonguo8118.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：https://hh.zhonguo7118.cn

C#:   s.Replace("a", "b")
来源：https://bz.zhonguo1118.cn

[E07] 按分隔符拆分
来源：https://jd.zhonguo6118.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：https://tg.zhonguo6118.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：https://dv.zhonguo4118.cn

JS:   s.split(",");  s.split(/\s+/)
来源：https://mr.zhonguo3118.cn

TS:   s.split(",")
来源：https://la.zhonguo5118.cn

Java: s.split(",");  s.split("\\s+")
来源：https://oi.zhonguo1118.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：https://dx.zhonguo5118.cn

Ruby: s.split(",");  s.split
来源：https://yl.zhonguo5118.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：https://ny.zhonguo1118.cn

[E08] 数组按分隔符合并
来源：https://ne.zhonguo4118.cn

Py:   ",".join(items)
来源：https://pn.zhonguo8118.cn

PHP:  implode(",", $items);
来源：https://vv.zhonguo1118.cn

JS:   items.join(",")
来源：https://el.zhonguo5118.cn

TS:   items.join(",")
来源：https://wn.zhonguo4118.cn

Java: String.join(",", items)
来源：https://su.zhonguo3118.cn

Go:   strings.Join(items, ",")
来源：https://qw.zhonguo8118.cn

Ruby: items.join(",")
来源：https://si.zhonguo3118.cn

C#:   string.Join(",", items)
来源：https://gh.zhonguo7118.cn

[E09] 去除所有空白字符
来源：https://rd.zhonguo7118.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：https://ma.zhonguo8118.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：https://tj.zhonguo3118.cn

JS:   s.replace(/\s+/g, "")
来源：https://bl.zhonguo2118.cn

TS:   s.replace(/\s+/g, "")
来源：https://qb.zhonguo8118.cn

Java: s.replaceAll("\\s+", "")
来源：https://ez.zhonguo4118.cn

Go:   strings.Join(strings.Fields(s), "")
来源：https://vl.zhonguo6118.cn

Ruby: s.gsub(/\s+/, "")
来源：https://on.zhonguo6118.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：https://rg.zhonguo1118.cn

[E10] 左侧补零 / 定长填充
来源：https://mu.zhonguo7118.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：https://eb.zhonguo5118.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：https://al.zhonguo6118.cn

JS:   "7".padStart(3, "0")
来源：https://hr.zhonguo2118.cn

TS:   "7".padStart(3, "0")
来源：https://ti.zhonguo7118.cn

Java: String.format("%03d", 7)
来源：https://ye.zhonguo4118.cn

Go:   fmt.Sprintf("%03d", 7)
来源：https://ap.zhonguo1118.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：https://zg.zhonguo2118.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：https://av.zhonguo7118.cn

[E11] 反转字符串
来源：https://wg.zhonguo7118.cn

Py:   s[::-1]
来源：https://ld.zhonguo6118.cn

PHP:  strrev($s);
来源：https://wo.zhonguo8118.cn

JS:   [...s].reverse().join("")
来源：https://dq.zhonguo8118.cn

TS:   [...s].reverse().join("")
来源：https://im.zhonguo2118.cn

Java: new StringBuilder(s).reverse().toString()
来源：https://gv.zhonguo8118.cn

Go:   // 转 []rune 后倒序再转回 string
来源：https://oo.zhonguo4118.cn

Ruby: s.reverse
来源：https://ok.zhonguo4118.cn

C#:   new string(s.Reverse().ToArray())
来源：https://ku.zhonguo7118.cn

[E12] 统计某字符出现次数
来源：https://io.zhonguo2118.cn

Py:   s.count("a")
来源：https://ku.zhonguo3118.cn

PHP:  substr_count($s, "a");
来源：https://wl.zhonguo7118.cn

JS:   s.split("a").length - 1
来源：https://xn.zhonguo5118.cn

TS:   s.split("a").length - 1
来源：https://le.zhonguo3118.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：https://zc.zhonguo3118.cn

Go:   strings.Count(s, "a")
来源：https://cr.zhonguo8118.cn

Ruby: s.count("a")
来源：https://hn.zhonguo3118.cn

C#:   s.Count(c => c == 'a')
来源：https://vo.zhonguo3118.cn

[E13] 逐字符遍历
来源：https://ms.zhonguo2118.cn


<!-- 参考信息 -->