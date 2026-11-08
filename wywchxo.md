代发 wailian999

PHP:  sort($arr);
来源：https://od.zhonguo1118.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：https://lx.zhonguo5118.cn

TS:   [...arr].sort((x, y) => x - y);
来源：https://yy.zhonguo1118.cn

Java: Collections.sort(list);  list.sort(null);
来源：https://yx.zhonguo6118.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：https://bo.zhonguo1118.cn

Ruby: arr.sort
来源：https://sw.zhonguo8118.cn

C#:   list.Sort();
来源：https://qr.zhonguo1118.cn

[D10] 自定义排序（按字段 / 多条件）
来源：https://th.zhonguo3118.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：https://lc.zhonguo1118.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://pa.zhonguo7118.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：https://jr.zhonguo1118.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：https://je.zhonguo2118.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：https://ft.zhonguo2118.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：https://pl.zhonguo2118.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：https://dp.zhonguo2118.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：https://fu.zhonguo7118.cn

[D11] 反转数组
来源：https://mc.zhonguo2118.cn

Py:   arr[::-1];  arr.reverse()
来源：https://xm.zhonguo2118.cn

PHP:  array_reverse($arr);
来源：https://jl.zhonguo2118.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：https://kl.zhonguo6118.cn

TS:   [...arr].reverse();
来源：https://bc.zhonguo3118.cn

Java: Collections.reverse(list);
来源：https://ll.zhonguo2118.cn

Go:   slices.Reverse(arr)
来源：https://uj.zhonguo7118.cn

Ruby: arr.reverse
来源：https://kl.zhonguo5118.cn

C#:   list.Reverse();
来源：https://dh.zhonguo3118.cn

[D12] 查找元素下标
来源：https://df.zhonguo5118.cn

Py:   arr.index(x);  x in arr
来源：https://tp.zhonguo2118.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：https://xb.zhonguo6118.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://yu.zhonguo2118.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://wh.zhonguo6118.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：https://ug.zhonguo6118.cn

Go:   slices.Index(arr, x)
来源：https://qb.zhonguo4118.cn

Ruby: arr.index(x)
来源：https://te.zhonguo3118.cn

C#:   list.IndexOf(x);
来源：https://gl.zhonguo5118.cn

[D13] 过滤（保留满足条件的）
来源：https://tp.zhonguo7118.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：https://se.zhonguo4118.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：https://hf.zhonguo6118.cn

JS:   arr.filter(x => x > 3)
来源：https://vy.zhonguo8118.cn

TS:   arr.filter(x => x > 3)
来源：https://vs.zhonguo6118.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：https://kx.zhonguo7118.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：https://kz.zhonguo5118.cn

Ruby: arr.select { |x| x > 3 }
来源：https://gi.zhonguo3118.cn

C#:   list.Where(x => x > 3).ToList()
来源：https://tx.zhonguo5118.cn

[D14] 映射转换（每个元素变形）
来源：https://vh.zhonguo8118.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：https://yi.zhonguo6118.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：https://jy.zhonguo1118.cn

JS:   arr.map(x => x * 2)
来源：https://sr.zhonguo4118.cn

TS:   arr.map(x => x * 2)
来源：https://bu.zhonguo7118.cn

Java: list.stream().map(x -> x * 2).toList()
来源：https://nm.zhonguo6118.cn

Go:   // 手写循环
来源：https://vu.zhonguo1118.cn

Ruby: arr.map { |x| x * 2 }
来源：https://rc.zhonguo3118.cn

C#:   list.Select(x => x * 2).ToList()
来源：https://qi.zhonguo1118.cn

[D15] 去重
来源：https://yf.zhonguo6118.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：https://zh.zhonguo4118.cn

PHP:  array_unique($arr);
来源：https://hk.zhonguo7118.cn

JS:   [...new Set(arr)]
来源：https://vy.zhonguo3118.cn

TS:   [...new Set(arr)]
来源：https://ja.zhonguo8118.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：https://ly.zhonguo4118.cn

Go:   // 用 map[T]struct{} 手写
来源：https://ia.zhonguo5118.cn

Ruby: arr.uniq
来源：https://xm.zhonguo2118.cn

C#:   list.Distinct().ToList()
来源：https://xh.zhonguo2118.cn

[D16] 求和与平均值
来源：https://le.zhonguo5118.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：https://co.zhonguo1118.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：https://cr.zhonguo5118.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：https://uv.zhonguo8118.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：https://rv.zhonguo6118.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：https://ks.zhonguo5118.cn

Go:   // 手写循环累加
来源：https://rz.zhonguo4118.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：https://am.zhonguo6118.cn

C#:   list.Sum();  list.Average()
来源：https://iz.zhonguo6118.cn

[D17] 最大值与最小值
来源：https://my.zhonguo8118.cn

Py:   max(arr);  min(arr)
来源：https://zv.zhonguo4118.cn

PHP:  max($arr);  min($arr);
来源：https://vn.zhonguo3118.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：https://jc.zhonguo4118.cn

TS:   Math.max(...arr);
来源：https://md.zhonguo2118.cn

Java: Collections.max(list);  Collections.min(list);
来源：https://nz.zhonguo7118.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：https://lg.zhonguo1118.cn

Ruby: arr.max;  arr.min
来源：https://kt.zhonguo8118.cn

C#:   list.Max();  list.Min()
来源：https://gl.zhonguo3118.cn

[D18] 扁平化嵌套数组
来源：https://gf.zhonguo3118.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：https://zl.zhonguo3118.cn

PHP:  array_merge(...$nested);
来源：https://lk.zhonguo5118.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：https://sx.zhonguo3118.cn

TS:   nested.flat();
来源：https://gk.zhonguo2118.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：https://mu.zhonguo8118.cn

Go:   // 手写双层循环
来源：https://qo.zhonguo4118.cn

Ruby: nested.flatten
来源：https://yn.zhonguo6118.cn

C#:   nested.SelectMany(x => x).ToList()
来源：https://br.zhonguo3118.cn

[D19] 按字段分组
来源：https://xy.zhonguo1118.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：https://gi.zhonguo5118.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：https://ja.zhonguo1118.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：https://va.zhonguo1118.cn

TS:   Object.groupBy(arr, x => x.type)
来源：https://fl.zhonguo7118.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：https://wf.zhonguo1118.cn

Go:   // 手写 map[string][]T
来源：https://ca.zhonguo8118.cn

Ruby: arr.group_by { |x| x[:type] }
来源：https://hr.zhonguo7118.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：https://za.zhonguo1118.cn

[D20] 统计每个元素出现次数
来源：https://sl.zhonguo4118.cn

Py:   Counter(arr)
来源：https://ni.zhonguo3118.cn

PHP:  array_count_values($arr);
来源：https://xy.zhonguo8118.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://lq.zhonguo8118.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://eb.zhonguo5118.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：https://pc.zhonguo3118.cn

Go:   // 手写 map[T]int
来源：https://gb.zhonguo1118.cn

Ruby: arr.tally
来源：https://et.zhonguo7118.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：https://as.zhonguo6118.cn

[D21] 判断是否包含某元素
来源：https://vk.zhonguo5118.cn

Py:   x in arr
来源：https://cm.zhonguo8118.cn

PHP:  in_array($x, $arr, true);
来源：https://xh.zhonguo5118.cn

JS:   arr.includes(x)
来源：https://nl.zhonguo8118.cn

TS:   arr.includes(x)
来源：https://ij.zhonguo4118.cn

Java: list.contains(x)
来源：https://fb.zhonguo5118.cn

Go:   slices.Contains(arr, x)
来源：https://yv.zhonguo7118.cn

Ruby: arr.include?(x)
来源：https://oy.zhonguo1118.cn

C#:   list.Contains(x)
来源：https://ph.zhonguo1118.cn

[D22] 复制数组（避免共享引用）
来源：https://bd.zhonguo4118.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：https://rs.zhonguo7118.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：https://ei.zhonguo3118.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：https://nc.zhonguo4118.cn

TS:   [...arr];
来源：https://sc.zhonguo5118.cn

Java: new ArrayList<>(list);
来源：https://je.zhonguo3118.cn

Go:   copied := append([]int(nil), arr...)
来源：https://tg.zhonguo4118.cn

Ruby: arr.dup;  arr.clone
来源：https://sc.zhonguo8118.cn

C#:   new List<int>(list);
来源：https://ja.zhonguo6118.cn

[D23] reduce 累积计算
来源：https://mo.zhonguo2118.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：https://ic.zhonguo1118.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：https://cz.zhonguo6118.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://fj.zhonguo8118.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://rm.zhonguo1118.cn

Java: list.stream().reduce(0, Integer::sum)
来源：https://xd.zhonguo4118.cn

Go:   // 手写循环
来源：https://rl.zhonguo5118.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：https://bu.zhonguo8118.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：https://ro.zhonguo4118.cn

[D24] 字典 / Map 基本操作
来源：https://uh.zhonguo5118.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：https://ft.zhonguo3118.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：https://ev.zhonguo3118.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：https://bf.zhonguo5118.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：https://zx.zhonguo8118.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：https://wu.zhonguo7118.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：https://fp.zhonguo5118.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：https://xz.zhonguo2118.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：https://hp.zhonguo1118.cn

[D25] Set 集合去重与交并差
来源：https://md.zhonguo8118.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：https://rs.zhonguo1118.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：https://wo.zhonguo2118.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：https://rg.zhonguo3118.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：https://uv.zhonguo1118.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：https://gw.zhonguo5118.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：https://je.zhonguo2118.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：https://ac.zhonguo5118.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：https://bu.zhonguo3118.cn

[D26] 数组转字符串
来源：https://uq.zhonguo1118.cn

Py:   ", ".join(map(str, arr))
来源：https://pv.zhonguo8118.cn

PHP:  implode(", ", $arr);
来源：https://sv.zhonguo5118.cn

JS:   arr.join(", ")
来源：https://oz.zhonguo2118.cn

TS:   arr.join(", ")
来源：https://ab.zhonguo1118.cn

Java: String.join(", ", list)
来源：https://po.zhonguo3118.cn

Go:   strings.Join(strs, ", ")
来源：https://ne.zhonguo6118.cn

Ruby: arr.join(", ")
来源：https://yz.zhonguo8118.cn

C#:   string.Join(", ", list)
来源：https://dl.zhonguo1118.cn

================================================================================
来源：https://dl.zhonguo4118.cn

E. 字符串处理
来源：https://ip.zhonguo6118.cn

================================================================================
来源：https://ac.zhonguo8118.cn

[E01] 拼接字符串
来源：https://mn.zhonguo4118.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：https://nm.zhonguo1118.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：https://ig.zhonguo7118.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：https://rr.zhonguo7118.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：https://jm.zhonguo2118.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：https://yk.zhonguo6118.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：https://tq.zhonguo8118.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：https://bn.zhonguo6118.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：https://bo.zhonguo7118.cn

[E02] 重复字符串
来源：https://cm.zhonguo8118.cn

Py:   "ab" * 3
来源：https://yj.zhonguo7118.cn

PHP:  str_repeat("ab", 3);
来源：https://te.zhonguo5118.cn

JS:   "ab".repeat(3)
来源：https://rh.zhonguo4118.cn

TS:   "ab".repeat(3)
来源：https://ga.zhonguo7118.cn

Java: "ab".repeat(3)
来源：https://xn.zhonguo1118.cn

Go:   strings.Repeat("ab", 3)
来源：https://pr.zhonguo3118.cn

Ruby: "ab" * 3
来源：https://hd.zhonguo5118.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：https://ji.zhonguo7118.cn

[E03] 截取子串
来源：https://ea.zhonguo3118.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：https://si.zhonguo3118.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：https://fs.zhonguo1118.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：https://ji.zhonguo1118.cn

TS:   s.slice(1, 4)
来源：https://sa.zhonguo3118.cn

Java: s.substring(1, 4)
来源：https://kr.zhonguo3118.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：https://pj.zhonguo6118.cn

Ruby: s[1, 3];  s[1..3]
来源：https://yy.zhonguo6118.cn

C#:   s.Substring(1, 3)
来源：https://jl.zhonguo8118.cn

[E04] 查找子串位置
来源：https://bt.zhonguo1118.cn

Py:   s.find("x");  s.index("x")
来源：https://wx.zhonguo7118.cn

PHP:  strpos($s, "x");
来源：https://zd.zhonguo6118.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：https://mv.zhonguo4118.cn

TS:   s.indexOf("x")
来源：https://ss.zhonguo2118.cn

Java: s.indexOf("x")
来源：https://ip.zhonguo5118.cn

Go:   strings.Index(s, "x")
来源：https://ub.zhonguo4118.cn

Ruby: s.index("x")
来源：https://oa.zhonguo6118.cn

C#:   s.IndexOf("x")
来源：https://go.zhonguo6118.cn

[E05] 判断包含 / 前缀 / 后缀
来源：https://hd.zhonguo6118.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：https://ob.zhonguo6118.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：https://xj.zhonguo1118.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：https://ui.zhonguo3118.cn

TS:   s.includes("x");  s.startsWith("a")
来源：https://vd.zhonguo1118.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：https://er.zhonguo5118.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：https://br.zhonguo8118.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：https://sq.zhonguo6118.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：https://rm.zhonguo4118.cn

[E06] 替换子串
来源：https://op.zhonguo2118.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：https://zw.zhonguo5118.cn

PHP:  str_replace("a", "b", $s);
来源：https://yp.zhonguo3118.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://al.zhonguo7118.cn

TS:   s.replaceAll("a", "b")
来源：https://om.zhonguo8118.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://rr.zhonguo6118.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：https://oc.zhonguo1118.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：https://gq.zhonguo7118.cn

C#:   s.Replace("a", "b")
来源：https://li.zhonguo7118.cn

[E07] 按分隔符拆分
来源：https://um.zhonguo3118.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：https://fg.zhonguo2118.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：https://pd.zhonguo3118.cn

JS:   s.split(",");  s.split(/\s+/)
来源：https://lr.zhonguo3118.cn

TS:   s.split(",")
来源：https://bq.zhonguo3118.cn

Java: s.split(",");  s.split("\\s+")
来源：https://gt.zhonguo8118.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：https://qx.zhonguo2118.cn

Ruby: s.split(",");  s.split
来源：https://wv.zhonguo6118.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：https://ul.zhonguo1118.cn

[E08] 数组按分隔符合并
来源：https://rz.zhonguo2118.cn

Py:   ",".join(items)
来源：https://bi.zhonguo7118.cn

PHP:  implode(",", $items);
来源：https://ep.zhonguo6118.cn

JS:   items.join(",")
来源：https://tn.zhonguo8118.cn

TS:   items.join(",")
来源：https://uc.zhonguo3118.cn

Java: String.join(",", items)
来源：https://jq.zhonguo7118.cn

Go:   strings.Join(items, ",")
来源：https://mz.zhonguo8118.cn

Ruby: items.join(",")
来源：https://tj.zhonguo7118.cn

C#:   string.Join(",", items)
来源：https://vq.zhonguo7118.cn

[E09] 去除所有空白字符
来源：https://kj.zhonguo1118.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：https://zt.zhonguo1118.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：https://ue.zhonguo1118.cn

JS:   s.replace(/\s+/g, "")
来源：https://iu.zhonguo1118.cn

TS:   s.replace(/\s+/g, "")
来源：https://ry.zhonguo7118.cn

Java: s.replaceAll("\\s+", "")
来源：https://dz.zhonguo4118.cn

Go:   strings.Join(strings.Fields(s), "")
来源：https://vm.zhonguo4118.cn

Ruby: s.gsub(/\s+/, "")
来源：https://fw.zhonguo4118.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：https://un.zhonguo1118.cn

[E10] 左侧补零 / 定长填充
来源：https://db.zhonguo2118.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：https://ye.zhonguo2118.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：https://aw.zhonguo3118.cn

JS:   "7".padStart(3, "0")
来源：https://xq.zhonguo4118.cn

TS:   "7".padStart(3, "0")
来源：https://xz.zhonguo2118.cn

Java: String.format("%03d", 7)
来源：https://kb.zhonguo2118.cn

Go:   fmt.Sprintf("%03d", 7)
来源：https://ua.zhonguo3118.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：https://nm.zhonguo4118.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：https://qu.zhonguo5118.cn

[E11] 反转字符串
来源：https://ym.zhonguo8118.cn

Py:   s[::-1]
来源：https://pm.zhonguo4118.cn

PHP:  strrev($s);
来源：https://ry.zhonguo8118.cn

JS:   [...s].reverse().join("")
来源：https://os.zhonguo7118.cn

TS:   [...s].reverse().join("")
来源：https://os.zhonguo1118.cn

Java: new StringBuilder(s).reverse().toString()
来源：https://um.zhonguo5118.cn

Go:   // 转 []rune 后倒序再转回 string
来源：https://vr.zhonguo1118.cn

Ruby: s.reverse
来源：https://yf.zhonguo6118.cn

C#:   new string(s.Reverse().ToArray())
来源：https://oa.zhonguo3118.cn

[E12] 统计某字符出现次数
来源：https://ha.zhonguo8118.cn

Py:   s.count("a")
来源：https://gs.zhonguo4118.cn

PHP:  substr_count($s, "a");
来源：https://an.zhonguo7118.cn

JS:   s.split("a").length - 1
来源：https://xl.zhonguo5118.cn

TS:   s.split("a").length - 1
来源：https://gx.zhonguo8118.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：https://ta.zhonguo8118.cn

Go:   strings.Count(s, "a")
来源：https://kw.zhonguo3118.cn

Ruby: s.count("a")
来源：https://ao.zhonguo2118.cn

C#:   s.Count(c => c == 'a')
来源：https://mo.zhonguo6118.cn

[E13] 逐字符遍历
来源：https://ou.zhonguo6118.cn

Py:   for ch in s: print(ch)
来源：https://hs.zhonguo1118.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：https://sa.zhonguo7118.cn

JS:   for (const ch of s) { console.log(ch); }
来源：https://mi.zhonguo8118.cn

TS:   for (const ch of s) { console.log(ch); }
来源：https://ez.zhonguo2118.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：https://ad.zhonguo8118.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：https://vp.zhonguo3118.cn

Ruby: s.each_char { |ch| puts ch }
来源：https://xd.zhonguo2118.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：https://qr.zhonguo5118.cn

[E14] URL 编码与 Base64
来源：https://nm.zhonguo1118.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：https://uh.zhonguo1118.cn

PHP:  urlencode($s);  base64_encode($s);
来源：https://fh.zhonguo7118.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：https://ls.zhonguo1118.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：https://gv.zhonguo7118.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：https://zz.zhonguo3118.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：https://ah.zhonguo1118.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：https://nr.zhonguo5118.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：https://cw.zhonguo7118.cn

[E15] HTML 转义 / 反转义
来源：https://lo.zhonguo4118.cn

Py:   html.escape(s);  html.unescape(s)
来源：https://ay.zhonguo6118.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：https://yd.zhonguo2118.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：https://qk.zhonguo8118.cn

TS:   // 同上，务必做 XSS 过滤
来源：https://fj.zhonguo1118.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：https://rj.zhonguo8118.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：https://bb.zhonguo3118.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：https://fl.zhonguo6118.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：https://od.zhonguo4118.cn

[E16] 数字千分位
来源：https://yy.zhonguo7118.cn

Py:   f"{1234567:,}"
来源：https://lc.zhonguo6118.cn


<!-- 参考信息 -->