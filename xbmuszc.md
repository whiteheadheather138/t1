代发 wailian999

Py:   len(arr)
来源：https://ap.zhonguo8118.cn

PHP:  count($arr);
来源：https://qw.zhonguo6118.cn

JS:   arr.length
来源：https://nh.zhonguo5118.cn

TS:   arr.length
来源：https://yo.zhonguo8118.cn

Java: list.size();
来源：https://cf.zhonguo2118.cn

Go:   len(arr)
来源：https://zj.zhonguo6118.cn

Ruby: arr.length; arr.size
来源：https://tt.zhonguo3118.cn

C#:   list.Count;
来源：https://xv.zhonguo7118.cn

[D07] 切片 / 取子数组
来源：https://xk.zhonguo3118.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：https://tf.zhonguo2118.cn

PHP:  array_slice($arr, 1, 3);
来源：https://kd.zhonguo6118.cn

JS:   arr.slice(1, 4);
来源：https://rr.zhonguo6118.cn

TS:   arr.slice(1, 4);
来源：https://gx.zhonguo3118.cn

Java: list.subList(1, 4);
来源：https://ti.zhonguo2118.cn

Go:   arr[1:4]
来源：https://cz.zhonguo8118.cn

Ruby: arr[1, 3]
来源：https://rg.zhonguo2118.cn

C#:   list.GetRange(1, 3);
来源：https://wp.zhonguo1118.cn

[D08] 合并两个数组
来源：https://eo.zhonguo7118.cn

Py:   a + b;  a.extend(b)
来源：https://gs.zhonguo8118.cn

PHP:  array_merge($a, $b);
来源：https://ks.zhonguo4118.cn

JS:   [...a, ...b];  a.concat(b);
来源：https://ik.zhonguo6118.cn

TS:   [...a, ...b];
来源：https://se.zhonguo8118.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：https://jl.zhonguo5118.cn

Go:   append(a, b...)
来源：https://et.zhonguo5118.cn

Ruby: a + b;  a.concat(b)
来源：https://sj.zhonguo2118.cn

C#:   a.Concat(b).ToList()
来源：https://pg.zhonguo8118.cn

[D09] 排序（升序）
来源：https://zd.zhonguo3118.cn

Py:   sorted(arr);  arr.sort()
来源：https://qg.zhonguo1118.cn

PHP:  sort($arr);
来源：https://dm.zhonguo7118.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：https://qr.zhonguo6118.cn

TS:   [...arr].sort((x, y) => x - y);
来源：https://wh.zhonguo4118.cn

Java: Collections.sort(list);  list.sort(null);
来源：https://vp.zhonguo5118.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：https://fj.zhonguo6118.cn

Ruby: arr.sort
来源：https://hn.zhonguo3118.cn

C#:   list.Sort();
来源：https://zx.zhonguo6118.cn

[D10] 自定义排序（按字段 / 多条件）
来源：https://kt.zhonguo4118.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：https://fj.zhonguo2118.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://fj.zhonguo6118.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：https://xh.zhonguo2118.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：https://fg.zhonguo3118.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：https://by.zhonguo5118.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：https://bj.zhonguo6118.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：https://pq.zhonguo3118.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：https://wa.zhonguo8118.cn

[D11] 反转数组
来源：https://ov.zhonguo7118.cn

Py:   arr[::-1];  arr.reverse()
来源：https://vz.zhonguo6118.cn

PHP:  array_reverse($arr);
来源：https://hi.zhonguo1118.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：https://ta.zhonguo4118.cn

TS:   [...arr].reverse();
来源：https://oq.zhonguo2118.cn

Java: Collections.reverse(list);
来源：https://yo.zhonguo1118.cn

Go:   slices.Reverse(arr)
来源：https://li.zhonguo7118.cn

Ruby: arr.reverse
来源：https://tx.zhonguo1118.cn

C#:   list.Reverse();
来源：https://tn.zhonguo4118.cn

[D12] 查找元素下标
来源：https://iw.zhonguo4118.cn

Py:   arr.index(x);  x in arr
来源：https://jf.zhonguo8118.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：https://hx.zhonguo3118.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://yu.zhonguo3118.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://xz.zhonguo5118.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：https://sw.zhonguo1118.cn

Go:   slices.Index(arr, x)
来源：https://vm.zhonguo2118.cn

Ruby: arr.index(x)
来源：https://gc.zhonguo5118.cn

C#:   list.IndexOf(x);
来源：https://qi.zhonguo6118.cn

[D13] 过滤（保留满足条件的）
来源：https://cw.zhonguo1118.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：https://zd.zhonguo5118.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：https://se.zhonguo4118.cn

JS:   arr.filter(x => x > 3)
来源：https://zz.zhonguo4118.cn

TS:   arr.filter(x => x > 3)
来源：https://iw.zhonguo6118.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：https://ss.zhonguo1118.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：https://rb.zhonguo8118.cn

Ruby: arr.select { |x| x > 3 }
来源：https://za.zhonguo7118.cn

C#:   list.Where(x => x > 3).ToList()
来源：https://ue.zhonguo8118.cn

[D14] 映射转换（每个元素变形）
来源：https://if.zhonguo6118.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：https://pe.zhonguo8118.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：https://pq.zhonguo8118.cn

JS:   arr.map(x => x * 2)
来源：https://dp.zhonguo7118.cn

TS:   arr.map(x => x * 2)
来源：https://vp.zhonguo3118.cn

Java: list.stream().map(x -> x * 2).toList()
来源：https://cg.zhonguo3118.cn

Go:   // 手写循环
来源：https://ok.zhonguo5118.cn

Ruby: arr.map { |x| x * 2 }
来源：https://hd.zhonguo2118.cn

C#:   list.Select(x => x * 2).ToList()
来源：https://tp.zhonguo6118.cn

[D15] 去重
来源：https://jq.zhonguo8118.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：https://vv.zhonguo1118.cn

PHP:  array_unique($arr);
来源：https://qn.zhonguo5118.cn

JS:   [...new Set(arr)]
来源：https://kd.zhonguo7118.cn

TS:   [...new Set(arr)]
来源：https://sn.zhonguo2118.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：https://kb.zhonguo1118.cn

Go:   // 用 map[T]struct{} 手写
来源：https://uc.zhonguo7118.cn

Ruby: arr.uniq
来源：https://dx.zhonguo2118.cn

C#:   list.Distinct().ToList()
来源：https://ig.zhonguo1118.cn

[D16] 求和与平均值
来源：https://wo.zhonguo7118.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：https://ie.zhonguo8118.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：https://kg.zhonguo7118.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：https://zj.zhonguo7118.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：https://og.zhonguo5118.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：https://ym.zhonguo1118.cn

Go:   // 手写循环累加
来源：https://ri.zhonguo3118.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：https://ej.zhonguo4118.cn

C#:   list.Sum();  list.Average()
来源：https://oh.zhonguo7118.cn

[D17] 最大值与最小值
来源：https://pe.zhonguo6118.cn

Py:   max(arr);  min(arr)
来源：https://wv.zhonguo5118.cn

PHP:  max($arr);  min($arr);
来源：https://pv.zhonguo5118.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：https://jr.zhonguo3118.cn

TS:   Math.max(...arr);
来源：https://py.zhonguo7118.cn

Java: Collections.max(list);  Collections.min(list);
来源：https://vy.zhonguo2118.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：https://ww.zhonguo6118.cn

Ruby: arr.max;  arr.min
来源：https://im.zhonguo8118.cn

C#:   list.Max();  list.Min()
来源：https://lm.zhonguo4118.cn

[D18] 扁平化嵌套数组
来源：https://hj.zhonguo5118.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：https://la.zhonguo6118.cn

PHP:  array_merge(...$nested);
来源：https://ez.zhonguo8118.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：https://lk.zhonguo5118.cn

TS:   nested.flat();
来源：https://qf.zhonguo1118.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：https://tj.zhonguo1118.cn

Go:   // 手写双层循环
来源：https://rr.zhonguo1118.cn

Ruby: nested.flatten
来源：https://wh.zhonguo2118.cn

C#:   nested.SelectMany(x => x).ToList()
来源：https://ga.zhonguo2118.cn

[D19] 按字段分组
来源：https://gv.zhonguo6118.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：https://ej.zhonguo7118.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：https://qt.zhonguo7118.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：https://mq.zhonguo7118.cn

TS:   Object.groupBy(arr, x => x.type)
来源：https://wt.zhonguo1118.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：https://jw.zhonguo1118.cn

Go:   // 手写 map[string][]T
来源：https://jm.zhonguo7118.cn

Ruby: arr.group_by { |x| x[:type] }
来源：https://hr.zhonguo8118.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：https://fz.zhonguo6118.cn

[D20] 统计每个元素出现次数
来源：https://sr.zhonguo4118.cn

Py:   Counter(arr)
来源：https://qz.zhonguo5118.cn

PHP:  array_count_values($arr);
来源：https://uq.zhonguo6118.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://ob.zhonguo2118.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://nc.zhonguo4118.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：https://hy.zhonguo8118.cn

Go:   // 手写 map[T]int
来源：https://bx.zhonguo8118.cn

Ruby: arr.tally
来源：https://vn.zhonguo7118.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：https://ir.zhonguo5118.cn

[D21] 判断是否包含某元素
来源：https://rg.zhonguo2118.cn

Py:   x in arr
来源：https://di.zhonguo8118.cn

PHP:  in_array($x, $arr, true);
来源：https://mm.zhonguo7118.cn

JS:   arr.includes(x)
来源：https://be.zhonguo7118.cn

TS:   arr.includes(x)
来源：https://me.zhonguo4118.cn

Java: list.contains(x)
来源：https://rw.zhonguo2118.cn

Go:   slices.Contains(arr, x)
来源：https://zc.zhonguo1118.cn

Ruby: arr.include?(x)
来源：https://ip.zhonguo8118.cn

C#:   list.Contains(x)
来源：https://kw.zhonguo7118.cn

[D22] 复制数组（避免共享引用）
来源：https://rg.zhonguo8118.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：https://yt.zhonguo8118.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：https://vg.zhonguo4118.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：https://zd.zhonguo7118.cn

TS:   [...arr];
来源：https://hw.zhonguo1118.cn

Java: new ArrayList<>(list);
来源：https://ib.zhonguo1118.cn

Go:   copied := append([]int(nil), arr...)
来源：https://ia.zhonguo1118.cn

Ruby: arr.dup;  arr.clone
来源：https://zq.zhonguo6118.cn

C#:   new List<int>(list);
来源：https://xw.zhonguo3118.cn

[D23] reduce 累积计算
来源：https://ps.zhonguo3118.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：https://qp.zhonguo6118.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：https://oc.zhonguo6118.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://ar.zhonguo8118.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://dr.zhonguo3118.cn

Java: list.stream().reduce(0, Integer::sum)
来源：https://ct.zhonguo3118.cn

Go:   // 手写循环
来源：https://jc.zhonguo7118.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：https://cu.zhonguo2118.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：https://sd.zhonguo8118.cn

[D24] 字典 / Map 基本操作
来源：https://jh.zhonguo3118.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：https://vd.zhonguo1118.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：https://zi.zhonguo3118.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：https://pe.zhonguo2118.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：https://cg.zhonguo4118.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：https://oj.zhonguo6118.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：https://dl.zhonguo7118.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：https://pz.zhonguo1118.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：https://ry.zhonguo2118.cn

[D25] Set 集合去重与交并差
来源：https://vn.zhonguo4118.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：https://rj.zhonguo5118.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：https://sx.zhonguo6118.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：https://yi.zhonguo7118.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：https://rd.zhonguo1118.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：https://fd.zhonguo3118.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：https://kx.zhonguo6118.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：https://yo.zhonguo6118.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：https://hu.zhonguo6118.cn

[D26] 数组转字符串
来源：https://pq.zhonguo6118.cn

Py:   ", ".join(map(str, arr))
来源：https://nf.zhonguo2118.cn

PHP:  implode(", ", $arr);
来源：https://ka.zhonguo1118.cn

JS:   arr.join(", ")
来源：https://ou.zhonguo7118.cn

TS:   arr.join(", ")
来源：https://zp.zhonguo6118.cn

Java: String.join(", ", list)
来源：https://gd.zhonguo2118.cn

Go:   strings.Join(strs, ", ")
来源：https://lz.zhonguo6118.cn

Ruby: arr.join(", ")
来源：https://wy.zhonguo2118.cn

C#:   string.Join(", ", list)
来源：https://yq.zhonguo7118.cn

================================================================================
来源：https://vp.zhonguo4118.cn

E. 字符串处理
来源：https://zt.zhonguo5118.cn

================================================================================
来源：https://my.zhonguo7118.cn

[E01] 拼接字符串
来源：https://cx.zhonguo2118.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：https://nj.zhonguo5118.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：https://li.zhonguo6118.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：https://jn.zhonguo2118.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：https://qu.zhonguo7118.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：https://uf.zhonguo2118.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：https://hw.zhonguo4118.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：https://qk.zhonguo6118.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：https://hw.zhonguo2118.cn

[E02] 重复字符串
来源：https://ne.zhonguo4118.cn

Py:   "ab" * 3
来源：https://ks.zhonguo1118.cn

PHP:  str_repeat("ab", 3);
来源：https://qk.zhonguo6118.cn

JS:   "ab".repeat(3)
来源：https://bo.zhonguo2118.cn

TS:   "ab".repeat(3)
来源：https://rg.zhonguo4118.cn

Java: "ab".repeat(3)
来源：https://qo.zhonguo7118.cn

Go:   strings.Repeat("ab", 3)
来源：https://tj.zhonguo2118.cn

Ruby: "ab" * 3
来源：https://ay.zhonguo5118.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：https://wv.zhonguo4118.cn

[E03] 截取子串
来源：https://px.zhonguo3118.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：https://zj.zhonguo4118.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：https://lr.zhonguo3118.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：https://xh.zhonguo7118.cn

TS:   s.slice(1, 4)
来源：https://xo.zhonguo1118.cn

Java: s.substring(1, 4)
来源：https://hh.zhonguo6118.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：https://ns.zhonguo5118.cn

Ruby: s[1, 3];  s[1..3]
来源：https://jo.zhonguo8118.cn

C#:   s.Substring(1, 3)
来源：https://pi.zhonguo7118.cn

[E04] 查找子串位置
来源：https://sj.zhonguo8118.cn

Py:   s.find("x");  s.index("x")
来源：https://lr.zhonguo7118.cn

PHP:  strpos($s, "x");
来源：https://mo.zhonguo3118.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：https://jo.zhonguo5118.cn

TS:   s.indexOf("x")
来源：https://ox.zhonguo3118.cn

Java: s.indexOf("x")
来源：https://er.zhonguo2118.cn

Go:   strings.Index(s, "x")
来源：https://cy.zhonguo4118.cn

Ruby: s.index("x")
来源：https://ez.zhonguo2118.cn

C#:   s.IndexOf("x")
来源：https://ki.zhonguo8118.cn

[E05] 判断包含 / 前缀 / 后缀
来源：https://fy.zhonguo5118.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：https://sv.zhonguo2118.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：https://vg.zhonguo1118.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：https://vb.zhonguo3118.cn

TS:   s.includes("x");  s.startsWith("a")
来源：https://jp.zhonguo2118.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：https://mu.zhonguo6118.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：https://ji.zhonguo2118.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：https://px.zhonguo5118.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：https://ew.zhonguo7118.cn

[E06] 替换子串
来源：https://xt.zhonguo2118.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：https://ht.zhonguo4118.cn

PHP:  str_replace("a", "b", $s);
来源：https://tt.zhonguo5118.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://xp.zhonguo1118.cn

TS:   s.replaceAll("a", "b")
来源：https://tv.zhonguo3118.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://ea.zhonguo3118.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：https://yb.zhonguo2118.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：https://cq.zhonguo7118.cn

C#:   s.Replace("a", "b")
来源：https://tw.zhonguo5118.cn

[E07] 按分隔符拆分
来源：https://vq.zhonguo3118.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：https://dj.zhonguo6118.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：https://qm.zhonguo1118.cn

JS:   s.split(",");  s.split(/\s+/)
来源：https://qf.zhonguo4118.cn

TS:   s.split(",")
来源：https://ak.zhonguo7118.cn

Java: s.split(",");  s.split("\\s+")
来源：https://en.zhonguo6118.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：https://wn.zhonguo4118.cn

Ruby: s.split(",");  s.split
来源：https://za.zhonguo5118.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：https://oy.zhonguo7118.cn

[E08] 数组按分隔符合并
来源：https://kd.zhonguo2118.cn

Py:   ",".join(items)
来源：https://fp.zhonguo2118.cn

PHP:  implode(",", $items);
来源：https://oa.zhonguo8118.cn

JS:   items.join(",")
来源：https://on.zhonguo6118.cn

TS:   items.join(",")
来源：https://pp.zhonguo2118.cn

Java: String.join(",", items)
来源：https://az.zhonguo7118.cn

Go:   strings.Join(items, ",")
来源：https://gp.zhonguo8118.cn

Ruby: items.join(",")
来源：https://qs.zhonguo5118.cn

C#:   string.Join(",", items)
来源：https://vp.zhonguo6118.cn

[E09] 去除所有空白字符
来源：https://qw.zhonguo2118.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：https://ky.zhonguo4118.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：https://ek.zhonguo1118.cn

JS:   s.replace(/\s+/g, "")
来源：https://ol.zhonguo1118.cn

TS:   s.replace(/\s+/g, "")
来源：https://kx.zhonguo4118.cn

Java: s.replaceAll("\\s+", "")
来源：https://mh.zhonguo4118.cn

Go:   strings.Join(strings.Fields(s), "")
来源：https://rn.zhonguo4118.cn

Ruby: s.gsub(/\s+/, "")
来源：https://sm.zhonguo6118.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：https://tq.zhonguo3118.cn

[E10] 左侧补零 / 定长填充
来源：https://ff.zhonguo2118.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：https://ek.zhonguo8118.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：https://cn.zhonguo1118.cn

JS:   "7".padStart(3, "0")
来源：https://jy.zhonguo6118.cn

TS:   "7".padStart(3, "0")
来源：https://ts.zhonguo6118.cn

Java: String.format("%03d", 7)
来源：https://il.zhonguo1118.cn

Go:   fmt.Sprintf("%03d", 7)
来源：https://zb.zhonguo8118.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：https://ho.zhonguo6118.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：https://ca.zhonguo4118.cn

[E11] 反转字符串
来源：https://lu.zhonguo6118.cn

Py:   s[::-1]
来源：https://lm.zhonguo5118.cn

PHP:  strrev($s);
来源：https://cc.zhonguo3118.cn

JS:   [...s].reverse().join("")
来源：https://wc.zhonguo6118.cn

TS:   [...s].reverse().join("")
来源：https://hu.zhonguo8118.cn

Java: new StringBuilder(s).reverse().toString()
来源：https://uf.zhonguo7118.cn

Go:   // 转 []rune 后倒序再转回 string
来源：https://yl.zhonguo4118.cn

Ruby: s.reverse
来源：https://uf.zhonguo4118.cn

C#:   new string(s.Reverse().ToArray())
来源：https://lt.zhonguo2118.cn

[E12] 统计某字符出现次数
来源：https://yc.zhonguo3118.cn

Py:   s.count("a")
来源：https://jv.zhonguo4118.cn

PHP:  substr_count($s, "a");
来源：https://bo.zhonguo1118.cn

JS:   s.split("a").length - 1
来源：https://yy.zhonguo5118.cn

TS:   s.split("a").length - 1
来源：https://kb.zhonguo1118.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：https://bv.zhonguo4118.cn

Go:   strings.Count(s, "a")
来源：https://ws.zhonguo5118.cn

Ruby: s.count("a")
来源：https://tf.zhonguo7118.cn

C#:   s.Count(c => c == 'a')
来源：https://gp.zhonguo7118.cn

[E13] 逐字符遍历
来源：https://jj.zhonguo4118.cn


<!-- 参考信息 -->