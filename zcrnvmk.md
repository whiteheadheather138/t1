代发 wailian999

Py:   len(arr)
来源：https://cz.zhonguo2118.cn

PHP:  count($arr);
来源：https://ts.zhonguo1118.cn

JS:   arr.length
来源：https://xy.zhonguo4118.cn

TS:   arr.length
来源：https://vn.zhonguo1118.cn

Java: list.size();
来源：https://tr.zhonguo8118.cn

Go:   len(arr)
来源：https://ui.zhonguo6118.cn

Ruby: arr.length; arr.size
来源：https://me.zhonguo8118.cn

C#:   list.Count;
来源：https://wn.zhonguo3118.cn

[D07] 切片 / 取子数组
来源：https://oz.zhonguo6118.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：https://he.zhonguo6118.cn

PHP:  array_slice($arr, 1, 3);
来源：https://cg.zhonguo4118.cn

JS:   arr.slice(1, 4);
来源：https://ll.zhonguo7118.cn

TS:   arr.slice(1, 4);
来源：https://zw.zhonguo5118.cn

Java: list.subList(1, 4);
来源：https://dz.zhonguo8118.cn

Go:   arr[1:4]
来源：https://og.zhonguo4118.cn

Ruby: arr[1, 3]
来源：https://ii.zhonguo6118.cn

C#:   list.GetRange(1, 3);
来源：https://mr.zhonguo3118.cn

[D08] 合并两个数组
来源：https://qa.zhonguo4118.cn

Py:   a + b;  a.extend(b)
来源：https://cc.zhonguo4118.cn

PHP:  array_merge($a, $b);
来源：https://ae.zhonguo1118.cn

JS:   [...a, ...b];  a.concat(b);
来源：https://ow.zhonguo5118.cn

TS:   [...a, ...b];
来源：https://yd.zhonguo5118.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：https://kx.zhonguo2118.cn

Go:   append(a, b...)
来源：https://bm.zhonguo8118.cn

Ruby: a + b;  a.concat(b)
来源：https://gk.zhonguo3118.cn

C#:   a.Concat(b).ToList()
来源：https://qj.zhonguo6118.cn

[D09] 排序（升序）
来源：https://or.zhonguo5118.cn

Py:   sorted(arr);  arr.sort()
来源：https://hs.zhonguo6118.cn

PHP:  sort($arr);
来源：https://nv.zhonguo8118.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：https://xi.zhonguo1118.cn

TS:   [...arr].sort((x, y) => x - y);
来源：https://pf.zhonguo6118.cn

Java: Collections.sort(list);  list.sort(null);
来源：https://sk.zhonguo8118.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：https://pu.zhonguo5118.cn

Ruby: arr.sort
来源：https://as.zhonguo4118.cn

C#:   list.Sort();
来源：https://ry.zhonguo7118.cn

[D10] 自定义排序（按字段 / 多条件）
来源：https://uh.zhonguo6118.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：https://ie.zhonguo6118.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://en.zhonguo5118.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：https://tv.zhonguo2118.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：https://ze.zhonguo4118.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：https://vv.zhonguo5118.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：https://ln.zhonguo2118.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：https://vm.zhonguo3118.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：https://kh.zhonguo2118.cn

[D11] 反转数组
来源：https://sr.zhonguo8118.cn

Py:   arr[::-1];  arr.reverse()
来源：https://rf.zhonguo3118.cn

PHP:  array_reverse($arr);
来源：https://mm.zhonguo7118.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：https://br.zhonguo2118.cn

TS:   [...arr].reverse();
来源：https://fd.zhonguo2118.cn

Java: Collections.reverse(list);
来源：https://vl.zhonguo2118.cn

Go:   slices.Reverse(arr)
来源：https://ts.zhonguo2118.cn

Ruby: arr.reverse
来源：https://ti.zhonguo5118.cn

C#:   list.Reverse();
来源：https://ys.zhonguo6118.cn

[D12] 查找元素下标
来源：https://zs.zhonguo6118.cn

Py:   arr.index(x);  x in arr
来源：https://sb.zhonguo3118.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：https://na.zhonguo1118.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://rf.zhonguo2118.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://ex.zhonguo1118.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：https://uu.zhonguo8118.cn

Go:   slices.Index(arr, x)
来源：https://ym.zhonguo5118.cn

Ruby: arr.index(x)
来源：https://sx.zhonguo5118.cn

C#:   list.IndexOf(x);
来源：https://lt.zhonguo4118.cn

[D13] 过滤（保留满足条件的）
来源：https://xr.zhonguo2118.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：https://cu.zhonguo7118.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：https://yi.zhonguo2118.cn

JS:   arr.filter(x => x > 3)
来源：https://ew.zhonguo8118.cn

TS:   arr.filter(x => x > 3)
来源：https://gb.zhonguo7118.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：https://cp.zhonguo1118.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：https://jo.zhonguo3118.cn

Ruby: arr.select { |x| x > 3 }
来源：https://kv.zhonguo7118.cn

C#:   list.Where(x => x > 3).ToList()
来源：https://er.zhonguo8118.cn

[D14] 映射转换（每个元素变形）
来源：https://fo.zhonguo6118.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：https://gn.zhonguo6118.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：https://bb.zhonguo6118.cn

JS:   arr.map(x => x * 2)
来源：https://wf.zhonguo4118.cn

TS:   arr.map(x => x * 2)
来源：https://rz.zhonguo4118.cn

Java: list.stream().map(x -> x * 2).toList()
来源：https://tv.zhonguo4118.cn

Go:   // 手写循环
来源：https://dy.zhonguo3118.cn

Ruby: arr.map { |x| x * 2 }
来源：https://fa.zhonguo2118.cn

C#:   list.Select(x => x * 2).ToList()
来源：https://li.zhonguo7118.cn

[D15] 去重
来源：https://wm.zhonguo5118.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：https://pv.zhonguo1118.cn

PHP:  array_unique($arr);
来源：https://sc.zhonguo5118.cn

JS:   [...new Set(arr)]
来源：https://vn.zhonguo2118.cn

TS:   [...new Set(arr)]
来源：https://dj.zhonguo8118.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：https://xm.zhonguo1118.cn

Go:   // 用 map[T]struct{} 手写
来源：https://mh.zhonguo1118.cn

Ruby: arr.uniq
来源：https://fo.zhonguo4118.cn

C#:   list.Distinct().ToList()
来源：https://tl.zhonguo2118.cn

[D16] 求和与平均值
来源：https://rm.zhonguo5118.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：https://fk.zhonguo4118.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：https://ux.zhonguo2118.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：https://bn.zhonguo2118.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：https://hx.zhonguo5118.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：https://bf.zhonguo8118.cn

Go:   // 手写循环累加
来源：https://td.zhonguo8118.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：https://ia.zhonguo3118.cn

C#:   list.Sum();  list.Average()
来源：https://wg.zhonguo4118.cn

[D17] 最大值与最小值
来源：https://iz.zhonguo6118.cn

Py:   max(arr);  min(arr)
来源：https://ez.zhonguo4118.cn

PHP:  max($arr);  min($arr);
来源：https://rf.zhonguo7118.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：https://kz.zhonguo6118.cn

TS:   Math.max(...arr);
来源：https://ic.zhonguo5118.cn

Java: Collections.max(list);  Collections.min(list);
来源：https://fo.zhonguo7118.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：https://vh.zhonguo4118.cn

Ruby: arr.max;  arr.min
来源：https://tj.zhonguo4118.cn

C#:   list.Max();  list.Min()
来源：https://gt.zhonguo3118.cn

[D18] 扁平化嵌套数组
来源：https://om.zhonguo1118.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：https://bp.zhonguo8118.cn

PHP:  array_merge(...$nested);
来源：https://em.zhonguo8118.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：https://fg.zhonguo5118.cn

TS:   nested.flat();
来源：https://wi.zhonguo6118.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：https://wd.zhonguo4118.cn

Go:   // 手写双层循环
来源：https://mm.zhonguo6118.cn

Ruby: nested.flatten
来源：https://gk.zhonguo6118.cn

C#:   nested.SelectMany(x => x).ToList()
来源：https://kh.zhonguo6118.cn

[D19] 按字段分组
来源：https://ei.zhonguo4118.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：https://xp.zhonguo3118.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：https://ob.zhonguo3118.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：https://id.zhonguo1118.cn

TS:   Object.groupBy(arr, x => x.type)
来源：https://ub.zhonguo5118.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：https://ih.zhonguo6118.cn

Go:   // 手写 map[string][]T
来源：https://qn.zhonguo4118.cn

Ruby: arr.group_by { |x| x[:type] }
来源：https://cy.zhonguo1118.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：https://go.zhonguo1118.cn

[D20] 统计每个元素出现次数
来源：https://ml.zhonguo6118.cn

Py:   Counter(arr)
来源：https://ip.zhonguo1118.cn

PHP:  array_count_values($arr);
来源：https://lj.zhonguo2118.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://pj.zhonguo5118.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://zk.zhonguo8118.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：https://rf.zhonguo4118.cn

Go:   // 手写 map[T]int
来源：https://cl.zhonguo2118.cn

Ruby: arr.tally
来源：https://xf.zhonguo4118.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：https://md.zhonguo6118.cn

[D21] 判断是否包含某元素
来源：https://zr.zhonguo8118.cn

Py:   x in arr
来源：https://cm.zhonguo6118.cn

PHP:  in_array($x, $arr, true);
来源：https://tw.zhonguo8118.cn

JS:   arr.includes(x)
来源：https://ge.zhonguo6118.cn

TS:   arr.includes(x)
来源：https://zn.zhonguo7118.cn

Java: list.contains(x)
来源：https://wh.zhonguo2118.cn

Go:   slices.Contains(arr, x)
来源：https://xf.zhonguo2118.cn

Ruby: arr.include?(x)
来源：https://bz.zhonguo1118.cn

C#:   list.Contains(x)
来源：https://lx.zhonguo4118.cn

[D22] 复制数组（避免共享引用）
来源：https://iw.zhonguo3118.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：https://ld.zhonguo1118.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：https://rb.zhonguo2118.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：https://jf.zhonguo5118.cn

TS:   [...arr];
来源：https://gf.zhonguo5118.cn

Java: new ArrayList<>(list);
来源：https://cy.zhonguo4118.cn

Go:   copied := append([]int(nil), arr...)
来源：https://ad.zhonguo8118.cn

Ruby: arr.dup;  arr.clone
来源：https://st.zhonguo4118.cn

C#:   new List<int>(list);
来源：https://ma.zhonguo4118.cn

[D23] reduce 累积计算
来源：https://ux.zhonguo6118.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：https://yu.zhonguo2118.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：https://mo.zhonguo7118.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://zg.zhonguo4118.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://if.zhonguo2118.cn

Java: list.stream().reduce(0, Integer::sum)
来源：https://cq.zhonguo7118.cn

Go:   // 手写循环
来源：https://ji.zhonguo8118.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：https://qk.zhonguo5118.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：https://na.zhonguo8118.cn

[D24] 字典 / Map 基本操作
来源：https://yo.zhonguo4118.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：https://xn.zhonguo7118.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：https://bf.zhonguo7118.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：https://cs.zhonguo4118.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：https://qh.zhonguo8118.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：https://vp.zhonguo5118.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：https://qp.zhonguo4118.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：https://uh.zhonguo8118.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：https://cy.zhonguo6118.cn

[D25] Set 集合去重与交并差
来源：https://kx.zhonguo6118.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：https://pp.zhonguo3118.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：https://ey.zhonguo5118.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：https://vi.zhonguo3118.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：https://ix.zhonguo4118.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：https://af.zhonguo2118.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：https://lr.zhonguo3118.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：https://wq.zhonguo6118.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：https://lq.zhonguo8118.cn

[D26] 数组转字符串
来源：https://ln.zhonguo3118.cn

Py:   ", ".join(map(str, arr))
来源：https://mh.zhonguo7118.cn

PHP:  implode(", ", $arr);
来源：https://ow.zhonguo4118.cn

JS:   arr.join(", ")
来源：https://dz.zhonguo8118.cn

TS:   arr.join(", ")
来源：https://am.zhonguo3118.cn

Java: String.join(", ", list)
来源：https://mm.zhonguo1118.cn

Go:   strings.Join(strs, ", ")
来源：https://qk.zhonguo3118.cn

Ruby: arr.join(", ")
来源：https://ph.zhonguo6118.cn

C#:   string.Join(", ", list)
来源：https://qv.zhonguo1118.cn

================================================================================
来源：https://ro.zhonguo2118.cn

E. 字符串处理
来源：https://po.zhonguo5118.cn

================================================================================
来源：https://lh.zhonguo7118.cn

[E01] 拼接字符串
来源：https://qz.zhonguo5118.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：https://su.zhonguo4118.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：https://gr.zhonguo3118.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：https://lz.zhonguo2118.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：https://ms.zhonguo3118.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：https://xa.zhonguo2118.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：https://nd.zhonguo5118.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：https://sr.zhonguo4118.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：https://ln.zhonguo3118.cn

[E02] 重复字符串
来源：https://nr.zhonguo2118.cn

Py:   "ab" * 3
来源：https://nj.zhonguo1118.cn

PHP:  str_repeat("ab", 3);
来源：https://yw.zhonguo4118.cn

JS:   "ab".repeat(3)
来源：https://ls.zhonguo8118.cn

TS:   "ab".repeat(3)
来源：https://hi.zhonguo6118.cn

Java: "ab".repeat(3)
来源：https://ly.zhonguo7118.cn

Go:   strings.Repeat("ab", 3)
来源：https://ni.zhonguo5118.cn

Ruby: "ab" * 3
来源：https://ru.zhonguo3118.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：https://dd.zhonguo1118.cn

[E03] 截取子串
来源：https://xo.zhonguo7118.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：https://qu.zhonguo8118.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：https://ep.zhonguo2118.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：https://mu.zhonguo7118.cn

TS:   s.slice(1, 4)
来源：https://zp.zhonguo4118.cn

Java: s.substring(1, 4)
来源：https://gm.zhonguo8118.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：https://jm.zhonguo2118.cn

Ruby: s[1, 3];  s[1..3]
来源：https://fy.zhonguo1118.cn

C#:   s.Substring(1, 3)
来源：https://vj.zhonguo8118.cn

[E04] 查找子串位置
来源：https://wi.zhonguo6118.cn

Py:   s.find("x");  s.index("x")
来源：https://rb.zhonguo6118.cn

PHP:  strpos($s, "x");
来源：https://he.zhonguo3118.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：https://xs.zhonguo4118.cn

TS:   s.indexOf("x")
来源：https://tn.zhonguo2118.cn

Java: s.indexOf("x")
来源：https://py.zhonguo3118.cn

Go:   strings.Index(s, "x")
来源：https://bf.zhonguo1118.cn

Ruby: s.index("x")
来源：https://ae.zhonguo1118.cn

C#:   s.IndexOf("x")
来源：https://zk.zhonguo7118.cn

[E05] 判断包含 / 前缀 / 后缀
来源：https://az.zhonguo4118.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：https://oa.zhonguo5118.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：https://lh.zhonguo5118.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：https://ny.zhonguo2118.cn

TS:   s.includes("x");  s.startsWith("a")
来源：https://it.zhonguo6118.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：https://wm.zhonguo7118.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：https://zg.zhonguo8118.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：https://tu.zhonguo5118.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：https://zd.zhonguo6118.cn

[E06] 替换子串
来源：https://mh.zhonguo7118.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：https://au.zhonguo1118.cn

PHP:  str_replace("a", "b", $s);
来源：https://gg.zhonguo3118.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://db.zhonguo1118.cn

TS:   s.replaceAll("a", "b")
来源：https://ee.zhonguo3118.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://pr.zhonguo1118.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：https://lo.zhonguo5118.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：https://wy.zhonguo4118.cn

C#:   s.Replace("a", "b")
来源：https://qn.zhonguo6118.cn

[E07] 按分隔符拆分
来源：https://ls.zhonguo8118.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：https://ft.zhonguo1118.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：https://zk.zhonguo7118.cn

JS:   s.split(",");  s.split(/\s+/)
来源：https://iq.zhonguo5118.cn

TS:   s.split(",")
来源：https://zt.zhonguo2118.cn

Java: s.split(",");  s.split("\\s+")
来源：https://oz.zhonguo5118.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：https://yw.zhonguo7118.cn

Ruby: s.split(",");  s.split
来源：https://os.zhonguo7118.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：https://la.zhonguo1118.cn

[E08] 数组按分隔符合并
来源：https://kf.zhonguo7118.cn

Py:   ",".join(items)
来源：https://ip.zhonguo4118.cn

PHP:  implode(",", $items);
来源：https://xq.zhonguo1118.cn

JS:   items.join(",")
来源：https://nf.zhonguo5118.cn

TS:   items.join(",")
来源：https://ky.zhonguo1118.cn

Java: String.join(",", items)
来源：https://ws.zhonguo6118.cn

Go:   strings.Join(items, ",")
来源：https://ui.zhonguo8118.cn

Ruby: items.join(",")
来源：https://bk.zhonguo8118.cn

C#:   string.Join(",", items)
来源：https://bq.zhonguo8118.cn

[E09] 去除所有空白字符
来源：https://oj.zhonguo4118.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：https://ay.zhonguo5118.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：https://nv.zhonguo5118.cn

JS:   s.replace(/\s+/g, "")
来源：https://ig.zhonguo3118.cn

TS:   s.replace(/\s+/g, "")
来源：https://ak.zhonguo8118.cn

Java: s.replaceAll("\\s+", "")
来源：https://pn.zhonguo3118.cn

Go:   strings.Join(strings.Fields(s), "")
来源：https://vp.zhonguo7118.cn

Ruby: s.gsub(/\s+/, "")
来源：https://am.zhonguo1118.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：https://iv.zhonguo6118.cn

[E10] 左侧补零 / 定长填充
来源：https://bw.zhonguo5118.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：https://fg.zhonguo6118.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：https://xe.zhonguo1118.cn

JS:   "7".padStart(3, "0")
来源：https://cd.zhonguo7118.cn

TS:   "7".padStart(3, "0")
来源：https://vv.zhonguo5118.cn

Java: String.format("%03d", 7)
来源：https://hp.zhonguo1118.cn

Go:   fmt.Sprintf("%03d", 7)
来源：https://xu.zhonguo5118.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：https://vy.zhonguo3118.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：https://re.zhonguo6118.cn

[E11] 反转字符串
来源：https://dg.zhonguo5118.cn

Py:   s[::-1]
来源：https://ed.zhonguo2118.cn

PHP:  strrev($s);
来源：https://bz.zhonguo8118.cn

JS:   [...s].reverse().join("")
来源：https://sm.zhonguo5118.cn

TS:   [...s].reverse().join("")
来源：https://yy.zhonguo6118.cn

Java: new StringBuilder(s).reverse().toString()
来源：https://ab.zhonguo3118.cn

Go:   // 转 []rune 后倒序再转回 string
来源：https://tf.zhonguo8118.cn

Ruby: s.reverse
来源：https://qj.zhonguo8118.cn

C#:   new string(s.Reverse().ToArray())
来源：https://ep.zhonguo8118.cn

[E12] 统计某字符出现次数
来源：https://zu.zhonguo1118.cn

Py:   s.count("a")
来源：https://bm.zhonguo1118.cn

PHP:  substr_count($s, "a");
来源：https://du.zhonguo5118.cn

JS:   s.split("a").length - 1
来源：https://ua.zhonguo5118.cn

TS:   s.split("a").length - 1
来源：https://dg.zhonguo5118.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：https://lu.zhonguo8118.cn

Go:   strings.Count(s, "a")
来源：https://zb.zhonguo5118.cn

Ruby: s.count("a")
来源：https://jq.zhonguo7118.cn

C#:   s.Count(c => c == 'a')
来源：https://wn.zhonguo5118.cn

[E13] 逐字符遍历
来源：https://sz.zhonguo5118.cn


<!-- 参考信息 -->