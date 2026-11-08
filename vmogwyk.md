代发 wailian999

[D07] 切片 / 取子数组
来源：https://zo.zhonguo6118.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：https://xx.zhonguo2118.cn

PHP:  array_slice($arr, 1, 3);
来源：https://bu.zhonguo5118.cn

JS:   arr.slice(1, 4);
来源：https://pw.zhonguo1118.cn

TS:   arr.slice(1, 4);
来源：https://nh.zhonguo8118.cn

Java: list.subList(1, 4);
来源：https://te.zhonguo8118.cn

Go:   arr[1:4]
来源：https://db.zhonguo2118.cn

Ruby: arr[1, 3]
来源：https://gb.zhonguo3118.cn

C#:   list.GetRange(1, 3);
来源：https://dv.zhonguo2118.cn

[D08] 合并两个数组
来源：https://jo.zhonguo1118.cn

Py:   a + b;  a.extend(b)
来源：https://cp.zhonguo1118.cn

PHP:  array_merge($a, $b);
来源：https://aa.zhonguo1118.cn

JS:   [...a, ...b];  a.concat(b);
来源：https://mq.zhonguo1118.cn

TS:   [...a, ...b];
来源：https://by.zhonguo6118.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：https://zr.zhonguo7118.cn

Go:   append(a, b...)
来源：https://tw.zhonguo4118.cn

Ruby: a + b;  a.concat(b)
来源：https://sz.zhonguo3118.cn

C#:   a.Concat(b).ToList()
来源：https://my.zhonguo3118.cn

[D09] 排序（升序）
来源：https://sh.zhonguo5118.cn

Py:   sorted(arr);  arr.sort()
来源：https://ub.zhonguo8118.cn

PHP:  sort($arr);
来源：https://id.zhonguo2118.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：https://jj.zhonguo4118.cn

TS:   [...arr].sort((x, y) => x - y);
来源：https://ih.zhonguo6118.cn

Java: Collections.sort(list);  list.sort(null);
来源：https://ho.zhonguo1118.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：https://ds.zhonguo3118.cn

Ruby: arr.sort
来源：https://yc.zhonguo6118.cn

C#:   list.Sort();
来源：https://sw.zhonguo4118.cn

[D10] 自定义排序（按字段 / 多条件）
来源：https://qs.zhonguo5118.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：https://sr.zhonguo6118.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://ns.zhonguo3118.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：https://us.zhonguo4118.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：https://am.zhonguo6118.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：https://hf.zhonguo4118.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：https://qj.zhonguo6118.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：https://uf.zhonguo7118.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：https://pn.zhonguo5118.cn

[D11] 反转数组
来源：https://vy.zhonguo3118.cn

Py:   arr[::-1];  arr.reverse()
来源：https://mh.zhonguo5118.cn

PHP:  array_reverse($arr);
来源：https://az.zhonguo8118.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：https://lk.zhonguo7118.cn

TS:   [...arr].reverse();
来源：https://zm.zhonguo7118.cn

Java: Collections.reverse(list);
来源：https://nm.zhonguo5118.cn

Go:   slices.Reverse(arr)
来源：https://fq.zhonguo5118.cn

Ruby: arr.reverse
来源：https://lg.zhonguo2118.cn

C#:   list.Reverse();
来源：https://ts.zhonguo5118.cn

[D12] 查找元素下标
来源：https://qf.zhonguo6118.cn

Py:   arr.index(x);  x in arr
来源：https://bz.zhonguo6118.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：https://ia.zhonguo5118.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://ib.zhonguo2118.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://hp.zhonguo3118.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：https://he.zhonguo8118.cn

Go:   slices.Index(arr, x)
来源：https://as.zhonguo7118.cn

Ruby: arr.index(x)
来源：https://ft.zhonguo4118.cn

C#:   list.IndexOf(x);
来源：https://yb.zhonguo7118.cn

[D13] 过滤（保留满足条件的）
来源：https://dw.zhonguo1118.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：https://jf.zhonguo5118.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：https://zn.zhonguo4118.cn

JS:   arr.filter(x => x > 3)
来源：https://fi.zhonguo6118.cn

TS:   arr.filter(x => x > 3)
来源：https://ba.zhonguo6118.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：https://el.zhonguo7118.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：https://pu.zhonguo8118.cn

Ruby: arr.select { |x| x > 3 }
来源：https://qs.zhonguo6118.cn

C#:   list.Where(x => x > 3).ToList()
来源：https://bs.zhonguo8118.cn

[D14] 映射转换（每个元素变形）
来源：https://wf.zhonguo8118.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：https://bf.zhonguo6118.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：https://ey.zhonguo4118.cn

JS:   arr.map(x => x * 2)
来源：https://le.zhonguo1118.cn

TS:   arr.map(x => x * 2)
来源：https://rw.zhonguo6118.cn

Java: list.stream().map(x -> x * 2).toList()
来源：https://cw.zhonguo8118.cn

Go:   // 手写循环
来源：https://vw.zhonguo4118.cn

Ruby: arr.map { |x| x * 2 }
来源：https://bz.zhonguo3118.cn

C#:   list.Select(x => x * 2).ToList()
来源：https://rv.zhonguo3118.cn

[D15] 去重
来源：https://sr.zhonguo8118.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：https://dx.zhonguo3118.cn

PHP:  array_unique($arr);
来源：https://bl.zhonguo1118.cn

JS:   [...new Set(arr)]
来源：https://ct.zhonguo1118.cn

TS:   [...new Set(arr)]
来源：https://ix.zhonguo7118.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：https://ws.zhonguo7118.cn

Go:   // 用 map[T]struct{} 手写
来源：https://ni.zhonguo6118.cn

Ruby: arr.uniq
来源：https://iy.zhonguo8118.cn

C#:   list.Distinct().ToList()
来源：https://tb.zhonguo2118.cn

[D16] 求和与平均值
来源：https://oy.zhonguo1118.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：https://di.zhonguo3118.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：https://jo.zhonguo5118.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：https://yo.zhonguo7118.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：https://pg.zhonguo5118.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：https://xg.zhonguo2118.cn

Go:   // 手写循环累加
来源：https://vh.zhonguo8118.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：https://gc.zhonguo4118.cn

C#:   list.Sum();  list.Average()
来源：https://ig.zhonguo8118.cn

[D17] 最大值与最小值
来源：https://vt.zhonguo6118.cn

Py:   max(arr);  min(arr)
来源：https://wx.zhonguo5118.cn

PHP:  max($arr);  min($arr);
来源：https://fp.zhonguo4118.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：https://ha.zhonguo2118.cn

TS:   Math.max(...arr);
来源：https://wo.zhonguo3118.cn

Java: Collections.max(list);  Collections.min(list);
来源：https://ne.zhonguo1118.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：https://lx.zhonguo7118.cn

Ruby: arr.max;  arr.min
来源：https://qo.zhonguo6118.cn

C#:   list.Max();  list.Min()
来源：https://lu.zhonguo1118.cn

[D18] 扁平化嵌套数组
来源：https://dn.zhonguo6118.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：https://ot.zhonguo7118.cn

PHP:  array_merge(...$nested);
来源：https://oh.zhonguo8118.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：https://rh.zhonguo5118.cn

TS:   nested.flat();
来源：https://dr.zhonguo8118.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：https://jk.zhonguo5118.cn

Go:   // 手写双层循环
来源：https://sy.zhonguo5118.cn

Ruby: nested.flatten
来源：https://ox.zhonguo7118.cn

C#:   nested.SelectMany(x => x).ToList()
来源：https://wl.zhonguo4118.cn

[D19] 按字段分组
来源：https://yl.zhonguo4118.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：https://qq.zhonguo6118.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：https://av.zhonguo5118.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：https://js.zhonguo5118.cn

TS:   Object.groupBy(arr, x => x.type)
来源：https://sj.zhonguo1118.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：https://td.zhonguo8118.cn

Go:   // 手写 map[string][]T
来源：https://zf.zhonguo7118.cn

Ruby: arr.group_by { |x| x[:type] }
来源：https://po.zhonguo7118.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：https://cj.zhonguo3118.cn

[D20] 统计每个元素出现次数
来源：https://iz.zhonguo2118.cn

Py:   Counter(arr)
来源：https://jk.zhonguo4118.cn

PHP:  array_count_values($arr);
来源：https://sr.zhonguo2118.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://ig.zhonguo4118.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://kd.zhonguo7118.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：https://ue.zhonguo6118.cn

Go:   // 手写 map[T]int
来源：https://fa.zhonguo1118.cn

Ruby: arr.tally
来源：https://os.zhonguo3118.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：https://wv.zhonguo7118.cn

[D21] 判断是否包含某元素
来源：https://ic.zhonguo3118.cn

Py:   x in arr
来源：https://tb.zhonguo8118.cn

PHP:  in_array($x, $arr, true);
来源：https://eb.zhonguo6118.cn

JS:   arr.includes(x)
来源：https://na.zhonguo2118.cn

TS:   arr.includes(x)
来源：https://cn.zhonguo6118.cn

Java: list.contains(x)
来源：https://nk.zhonguo2118.cn

Go:   slices.Contains(arr, x)
来源：https://aj.zhonguo6118.cn

Ruby: arr.include?(x)
来源：https://az.zhonguo2118.cn

C#:   list.Contains(x)
来源：https://by.zhonguo1118.cn

[D22] 复制数组（避免共享引用）
来源：https://yb.zhonguo5118.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：https://lg.zhonguo6118.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：https://wm.zhonguo7118.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：https://bj.zhonguo5118.cn

TS:   [...arr];
来源：https://nn.zhonguo1118.cn

Java: new ArrayList<>(list);
来源：https://iv.zhonguo4118.cn

Go:   copied := append([]int(nil), arr...)
来源：https://zl.zhonguo5118.cn

Ruby: arr.dup;  arr.clone
来源：https://zc.zhonguo2118.cn

C#:   new List<int>(list);
来源：https://lv.zhonguo7118.cn

[D23] reduce 累积计算
来源：https://is.zhonguo2118.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：https://oy.zhonguo5118.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：https://vf.zhonguo1118.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://wu.zhonguo4118.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://jk.zhonguo1118.cn

Java: list.stream().reduce(0, Integer::sum)
来源：https://nc.zhonguo6118.cn

Go:   // 手写循环
来源：https://xh.zhonguo6118.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：https://fj.zhonguo1118.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：https://lk.zhonguo6118.cn

[D24] 字典 / Map 基本操作
来源：https://hs.zhonguo2118.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：https://pc.zhonguo2118.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：https://ix.zhonguo7118.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：https://em.zhonguo5118.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：https://ky.zhonguo6118.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：https://mb.zhonguo6118.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：https://ha.zhonguo7118.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：https://uv.zhonguo2118.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：https://yl.zhonguo8118.cn

[D25] Set 集合去重与交并差
来源：https://xv.zhonguo1118.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：https://as.zhonguo7118.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：https://sh.zhonguo6118.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：https://io.zhonguo4118.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：https://ea.zhonguo8118.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：https://dg.zhonguo7118.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：https://xi.zhonguo1118.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：https://kv.zhonguo4118.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：https://nh.zhonguo2118.cn

[D26] 数组转字符串
来源：https://kw.zhonguo8118.cn

Py:   ", ".join(map(str, arr))
来源：https://fh.zhonguo5118.cn

PHP:  implode(", ", $arr);
来源：https://en.zhonguo6118.cn

JS:   arr.join(", ")
来源：https://bm.zhonguo3118.cn

TS:   arr.join(", ")
来源：https://wp.zhonguo7118.cn

Java: String.join(", ", list)
来源：https://zc.zhonguo2118.cn

Go:   strings.Join(strs, ", ")
来源：https://je.zhonguo1118.cn

Ruby: arr.join(", ")
来源：https://ft.zhonguo8118.cn

C#:   string.Join(", ", list)
来源：https://lz.zhonguo6118.cn

================================================================================
来源：https://hc.zhonguo3118.cn

E. 字符串处理
来源：https://of.zhonguo8118.cn

================================================================================
来源：https://bn.zhonguo6118.cn

[E01] 拼接字符串
来源：https://iq.zhonguo5118.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：https://lw.zhonguo6118.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：https://aj.zhonguo2118.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：https://ji.zhonguo1118.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：https://xe.zhonguo4118.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：https://au.zhonguo5118.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：https://uy.zhonguo4118.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：https://kk.zhonguo4118.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：https://dc.zhonguo3118.cn

[E02] 重复字符串
来源：https://tq.zhonguo6118.cn

Py:   "ab" * 3
来源：https://by.zhonguo7118.cn

PHP:  str_repeat("ab", 3);
来源：https://xi.zhonguo2118.cn

JS:   "ab".repeat(3)
来源：https://oa.zhonguo5118.cn

TS:   "ab".repeat(3)
来源：https://nl.zhonguo5118.cn

Java: "ab".repeat(3)
来源：https://de.zhonguo3118.cn

Go:   strings.Repeat("ab", 3)
来源：https://ff.zhonguo5118.cn

Ruby: "ab" * 3
来源：https://ss.zhonguo1118.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：https://mv.zhonguo3118.cn

[E03] 截取子串
来源：https://ak.zhonguo1118.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：https://hb.zhonguo7118.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：https://nr.zhonguo3118.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：https://ez.zhonguo5118.cn

TS:   s.slice(1, 4)
来源：https://mn.zhonguo7118.cn

Java: s.substring(1, 4)
来源：https://xu.zhonguo1118.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：https://lk.zhonguo3118.cn

Ruby: s[1, 3];  s[1..3]
来源：https://hr.zhonguo4118.cn

C#:   s.Substring(1, 3)
来源：https://hz.zhonguo4118.cn

[E04] 查找子串位置
来源：https://sd.zhonguo7118.cn

Py:   s.find("x");  s.index("x")
来源：https://ey.zhonguo7118.cn

PHP:  strpos($s, "x");
来源：https://cn.zhonguo4118.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：https://bi.zhonguo7118.cn

TS:   s.indexOf("x")
来源：https://hj.zhonguo4118.cn

Java: s.indexOf("x")
来源：https://pq.zhonguo4118.cn

Go:   strings.Index(s, "x")
来源：https://uc.zhonguo3118.cn

Ruby: s.index("x")
来源：https://mg.zhonguo8118.cn

C#:   s.IndexOf("x")
来源：https://ne.zhonguo8118.cn

[E05] 判断包含 / 前缀 / 后缀
来源：https://zf.zhonguo8118.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：https://if.zhonguo5118.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：https://ab.zhonguo4118.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：https://dq.zhonguo3118.cn

TS:   s.includes("x");  s.startsWith("a")
来源：https://qw.zhonguo3118.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：https://hb.zhonguo3118.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：https://la.zhonguo1118.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：https://al.zhonguo5118.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：https://mc.zhonguo5118.cn

[E06] 替换子串
来源：https://fj.zhonguo2118.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：https://yk.zhonguo8118.cn

PHP:  str_replace("a", "b", $s);
来源：https://tk.zhonguo8118.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://ta.zhonguo7118.cn

TS:   s.replaceAll("a", "b")
来源：https://dm.zhonguo4118.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://zz.zhonguo8118.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：https://wl.zhonguo7118.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：https://cu.zhonguo4118.cn

C#:   s.Replace("a", "b")
来源：https://eh.zhonguo6118.cn

[E07] 按分隔符拆分
来源：https://ae.zhonguo7118.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：https://ll.zhonguo5118.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：https://jb.zhonguo4118.cn

JS:   s.split(",");  s.split(/\s+/)
来源：https://ip.zhonguo7118.cn

TS:   s.split(",")
来源：https://lp.zhonguo7118.cn

Java: s.split(",");  s.split("\\s+")
来源：https://ic.zhonguo1118.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：https://cw.zhonguo8118.cn

Ruby: s.split(",");  s.split
来源：https://eb.zhonguo4118.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：https://ly.zhonguo6118.cn

[E08] 数组按分隔符合并
来源：https://pt.zhonguo5118.cn

Py:   ",".join(items)
来源：https://fd.zhonguo6118.cn

PHP:  implode(",", $items);
来源：https://jf.zhonguo4118.cn

JS:   items.join(",")
来源：https://sm.zhonguo8118.cn

TS:   items.join(",")
来源：https://un.zhonguo8118.cn

Java: String.join(",", items)
来源：https://at.zhonguo8118.cn

Go:   strings.Join(items, ",")
来源：https://hs.zhonguo5118.cn

Ruby: items.join(",")
来源：https://nb.zhonguo4118.cn

C#:   string.Join(",", items)
来源：https://vs.zhonguo1118.cn

[E09] 去除所有空白字符
来源：https://ny.zhonguo1118.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：https://gl.zhonguo4118.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：https://wd.zhonguo8118.cn

JS:   s.replace(/\s+/g, "")
来源：https://gs.zhonguo3118.cn

TS:   s.replace(/\s+/g, "")
来源：https://km.zhonguo1118.cn

Java: s.replaceAll("\\s+", "")
来源：https://ks.zhonguo7118.cn

Go:   strings.Join(strings.Fields(s), "")
来源：https://ya.zhonguo7118.cn

Ruby: s.gsub(/\s+/, "")
来源：https://do.zhonguo1118.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：https://gx.zhonguo2118.cn

[E10] 左侧补零 / 定长填充
来源：https://xc.zhonguo3118.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：https://mz.zhonguo5118.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：https://xt.zhonguo7118.cn

JS:   "7".padStart(3, "0")
来源：https://ug.zhonguo7118.cn

TS:   "7".padStart(3, "0")
来源：https://xt.zhonguo3118.cn

Java: String.format("%03d", 7)
来源：https://yt.zhonguo7118.cn

Go:   fmt.Sprintf("%03d", 7)
来源：https://up.zhonguo2118.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：https://so.zhonguo4118.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：https://ab.zhonguo7118.cn

[E11] 反转字符串
来源：https://jb.zhonguo2118.cn

Py:   s[::-1]
来源：https://zg.zhonguo3118.cn

PHP:  strrev($s);
来源：https://jp.zhonguo1118.cn

JS:   [...s].reverse().join("")
来源：https://si.zhonguo5118.cn

TS:   [...s].reverse().join("")
来源：https://az.zhonguo1118.cn

Java: new StringBuilder(s).reverse().toString()
来源：https://mi.zhonguo6118.cn

Go:   // 转 []rune 后倒序再转回 string
来源：https://jp.zhonguo7118.cn

Ruby: s.reverse
来源：https://nm.zhonguo8118.cn

C#:   new string(s.Reverse().ToArray())
来源：https://kj.zhonguo6118.cn

[E12] 统计某字符出现次数
来源：https://ip.zhonguo1118.cn

Py:   s.count("a")
来源：https://zb.zhonguo4118.cn

PHP:  substr_count($s, "a");
来源：https://ha.zhonguo6118.cn

JS:   s.split("a").length - 1
来源：https://rl.zhonguo5118.cn

TS:   s.split("a").length - 1
来源：https://tj.zhonguo2118.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：https://vj.zhonguo2118.cn

Go:   strings.Count(s, "a")
来源：https://qk.zhonguo7118.cn

Ruby: s.count("a")
来源：https://uv.zhonguo5118.cn

C#:   s.Count(c => c == 'a')
来源：https://sk.zhonguo6118.cn

[E13] 逐字符遍历
来源：https://ta.zhonguo5118.cn

Py:   for ch in s: print(ch)
来源：https://cg.zhonguo4118.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：https://mu.zhonguo8118.cn

JS:   for (const ch of s) { console.log(ch); }
来源：https://mr.zhonguo8118.cn

TS:   for (const ch of s) { console.log(ch); }
来源：https://xc.zhonguo3118.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：https://cu.zhonguo7118.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：https://ny.zhonguo1118.cn

Ruby: s.each_char { |ch| puts ch }
来源：https://da.zhonguo5118.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：https://mz.zhonguo3118.cn


<!-- 参考信息 -->