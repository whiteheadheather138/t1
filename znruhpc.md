代发 wailian999

TS:   [...arr].reverse();
来源：https://gp.zhonguo3118.cn

Java: Collections.reverse(list);
来源：https://qy.zhonguo2118.cn

Go:   slices.Reverse(arr)
来源：https://ug.zhonguo2118.cn

Ruby: arr.reverse
来源：https://qg.zhonguo4118.cn

C#:   list.Reverse();
来源：https://mq.zhonguo1118.cn

[D12] 查找元素下标
来源：https://in.zhonguo1118.cn

Py:   arr.index(x);  x in arr
来源：https://vw.zhonguo8118.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：https://ij.zhonguo1118.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://gm.zhonguo6118.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://kz.zhonguo5118.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：https://fz.zhonguo3118.cn

Go:   slices.Index(arr, x)
来源：https://zf.zhonguo7118.cn

Ruby: arr.index(x)
来源：https://xh.zhonguo8118.cn

C#:   list.IndexOf(x);
来源：https://ht.zhonguo3118.cn

[D13] 过滤（保留满足条件的）
来源：https://dh.zhonguo3118.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：https://bm.zhonguo2118.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：https://wb.zhonguo5118.cn

JS:   arr.filter(x => x > 3)
来源：https://ek.zhonguo8118.cn

TS:   arr.filter(x => x > 3)
来源：https://uy.zhonguo2118.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：https://tl.zhonguo1118.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：https://xg.zhonguo7118.cn

Ruby: arr.select { |x| x > 3 }
来源：https://nr.zhonguo2118.cn

C#:   list.Where(x => x > 3).ToList()
来源：https://wu.zhonguo2118.cn

[D14] 映射转换（每个元素变形）
来源：https://iu.zhonguo3118.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：https://hq.zhonguo6118.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：https://za.zhonguo8118.cn

JS:   arr.map(x => x * 2)
来源：https://rm.zhonguo5118.cn

TS:   arr.map(x => x * 2)
来源：https://zq.zhonguo3118.cn

Java: list.stream().map(x -> x * 2).toList()
来源：https://ty.zhonguo5118.cn

Go:   // 手写循环
来源：https://jq.zhonguo4118.cn

Ruby: arr.map { |x| x * 2 }
来源：https://qu.zhonguo8118.cn

C#:   list.Select(x => x * 2).ToList()
来源：https://op.zhonguo2118.cn

[D15] 去重
来源：https://jl.zhonguo5118.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：https://ad.zhonguo6118.cn

PHP:  array_unique($arr);
来源：https://oh.zhonguo4118.cn

JS:   [...new Set(arr)]
来源：https://mk.zhonguo4118.cn

TS:   [...new Set(arr)]
来源：https://qo.zhonguo1118.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：https://cn.zhonguo7118.cn

Go:   // 用 map[T]struct{} 手写
来源：https://yh.zhonguo4118.cn

Ruby: arr.uniq
来源：https://mk.zhonguo3118.cn

C#:   list.Distinct().ToList()
来源：https://tj.zhonguo1118.cn

[D16] 求和与平均值
来源：https://gw.zhonguo3118.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：https://oy.zhonguo7118.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：https://zg.zhonguo5118.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：https://mh.zhonguo4118.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：https://js.zhonguo5118.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：https://zo.zhonguo6118.cn

Go:   // 手写循环累加
来源：https://bq.zhonguo7118.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：https://tm.zhonguo2118.cn

C#:   list.Sum();  list.Average()
来源：https://eb.zhonguo3118.cn

[D17] 最大值与最小值
来源：https://et.zhonguo7118.cn

Py:   max(arr);  min(arr)
来源：https://bn.zhonguo1118.cn

PHP:  max($arr);  min($arr);
来源：https://nz.zhonguo8118.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：https://fj.zhonguo3118.cn

TS:   Math.max(...arr);
来源：https://tn.zhonguo3118.cn

Java: Collections.max(list);  Collections.min(list);
来源：https://qp.zhonguo4118.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：https://nj.zhonguo2118.cn

Ruby: arr.max;  arr.min
来源：https://cj.zhonguo2118.cn

C#:   list.Max();  list.Min()
来源：https://ku.zhonguo3118.cn

[D18] 扁平化嵌套数组
来源：https://tp.zhonguo6118.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：https://ud.zhonguo4118.cn

PHP:  array_merge(...$nested);
来源：https://ck.zhonguo4118.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：https://pc.zhonguo4118.cn

TS:   nested.flat();
来源：https://xw.zhonguo7118.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：https://ip.zhonguo3118.cn

Go:   // 手写双层循环
来源：https://mq.zhonguo7118.cn

Ruby: nested.flatten
来源：https://on.zhonguo3118.cn

C#:   nested.SelectMany(x => x).ToList()
来源：https://ec.zhonguo5118.cn

[D19] 按字段分组
来源：https://ni.zhonguo8118.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：https://yp.zhonguo5118.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：https://og.zhonguo8118.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：https://dt.zhonguo3118.cn

TS:   Object.groupBy(arr, x => x.type)
来源：https://pn.zhonguo4118.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：https://hc.zhonguo6118.cn

Go:   // 手写 map[string][]T
来源：https://in.zhonguo4118.cn

Ruby: arr.group_by { |x| x[:type] }
来源：https://cp.zhonguo7118.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：https://kj.zhonguo2118.cn

[D20] 统计每个元素出现次数
来源：https://zx.zhonguo5118.cn

Py:   Counter(arr)
来源：https://py.zhonguo4118.cn

PHP:  array_count_values($arr);
来源：https://ar.zhonguo8118.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://id.zhonguo8118.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://sb.zhonguo1118.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：https://ok.zhonguo1118.cn

Go:   // 手写 map[T]int
来源：https://rb.zhonguo3118.cn

Ruby: arr.tally
来源：https://gb.zhonguo8118.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：https://cb.zhonguo6118.cn

[D21] 判断是否包含某元素
来源：https://zc.zhonguo5118.cn

Py:   x in arr
来源：https://ob.zhonguo4118.cn

PHP:  in_array($x, $arr, true);
来源：https://ox.zhonguo1118.cn

JS:   arr.includes(x)
来源：https://vn.zhonguo4118.cn

TS:   arr.includes(x)
来源：https://pf.zhonguo7118.cn

Java: list.contains(x)
来源：https://kd.zhonguo5118.cn

Go:   slices.Contains(arr, x)
来源：https://uf.zhonguo4118.cn

Ruby: arr.include?(x)
来源：https://dy.zhonguo1118.cn

C#:   list.Contains(x)
来源：https://fe.zhonguo3118.cn

[D22] 复制数组（避免共享引用）
来源：https://io.zhonguo3118.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：https://nx.zhonguo7118.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：https://qx.zhonguo8118.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：https://nw.zhonguo4118.cn

TS:   [...arr];
来源：https://vd.zhonguo8118.cn

Java: new ArrayList<>(list);
来源：https://ew.zhonguo5118.cn

Go:   copied := append([]int(nil), arr...)
来源：https://us.zhonguo3118.cn

Ruby: arr.dup;  arr.clone
来源：https://np.zhonguo7118.cn

C#:   new List<int>(list);
来源：https://wb.zhonguo7118.cn

[D23] reduce 累积计算
来源：https://fl.zhonguo5118.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：https://de.zhonguo8118.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：https://tt.zhonguo1118.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://uw.zhonguo8118.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://ae.zhonguo5118.cn

Java: list.stream().reduce(0, Integer::sum)
来源：https://cd.zhonguo5118.cn

Go:   // 手写循环
来源：https://hh.zhonguo5118.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：https://bx.zhonguo4118.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：https://hs.zhonguo1118.cn

[D24] 字典 / Map 基本操作
来源：https://sc.zhonguo1118.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：https://zy.zhonguo1118.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：https://fh.zhonguo3118.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：https://dh.zhonguo8118.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：https://lb.zhonguo7118.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：https://ih.zhonguo8118.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：https://wa.zhonguo6118.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：https://qy.zhonguo6118.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：https://ia.zhonguo7118.cn

[D25] Set 集合去重与交并差
来源：https://yb.zhonguo7118.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：https://ys.zhonguo5118.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：https://dz.zhonguo6118.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：https://ky.zhonguo2118.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：https://ys.zhonguo5118.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：https://kb.zhonguo6118.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：https://un.zhonguo6118.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：https://iv.zhonguo5118.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：https://mp.zhonguo7118.cn

[D26] 数组转字符串
来源：https://dj.zhonguo3118.cn

Py:   ", ".join(map(str, arr))
来源：https://zv.zhonguo1118.cn

PHP:  implode(", ", $arr);
来源：https://re.zhonguo2118.cn

JS:   arr.join(", ")
来源：https://oc.zhonguo8118.cn

TS:   arr.join(", ")
来源：https://rv.zhonguo6118.cn

Java: String.join(", ", list)
来源：https://dk.zhonguo4118.cn

Go:   strings.Join(strs, ", ")
来源：https://dm.zhonguo6118.cn

Ruby: arr.join(", ")
来源：https://yl.zhonguo5118.cn

C#:   string.Join(", ", list)
来源：https://na.zhonguo8118.cn

================================================================================
来源：https://tu.zhonguo6118.cn

E. 字符串处理
来源：https://ay.zhonguo7118.cn

================================================================================
来源：https://ph.zhonguo3118.cn

[E01] 拼接字符串
来源：https://ah.zhonguo2118.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：https://ea.zhonguo3118.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：https://kl.zhonguo1118.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：https://dz.zhonguo6118.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：https://ni.zhonguo8118.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：https://yb.zhonguo2118.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：https://uj.zhonguo4118.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：https://ip.zhonguo6118.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：https://ds.zhonguo8118.cn

[E02] 重复字符串
来源：https://es.zhonguo5118.cn

Py:   "ab" * 3
来源：https://dl.zhonguo1118.cn

PHP:  str_repeat("ab", 3);
来源：https://gp.zhonguo2118.cn

JS:   "ab".repeat(3)
来源：https://om.zhonguo3118.cn

TS:   "ab".repeat(3)
来源：https://sx.zhonguo6118.cn

Java: "ab".repeat(3)
来源：https://lx.zhonguo6118.cn

Go:   strings.Repeat("ab", 3)
来源：https://oc.zhonguo6118.cn

Ruby: "ab" * 3
来源：https://jd.zhonguo2118.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：https://dg.zhonguo2118.cn

[E03] 截取子串
来源：https://ro.zhonguo5118.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：https://ni.zhonguo1118.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：https://do.zhonguo8118.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：https://ur.zhonguo4118.cn

TS:   s.slice(1, 4)
来源：https://td.zhonguo1118.cn

Java: s.substring(1, 4)
来源：https://ui.zhonguo4118.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：https://je.zhonguo8118.cn

Ruby: s[1, 3];  s[1..3]
来源：https://sf.zhonguo2118.cn

C#:   s.Substring(1, 3)
来源：https://lw.zhonguo8118.cn

[E04] 查找子串位置
来源：https://ao.zhonguo1118.cn

Py:   s.find("x");  s.index("x")
来源：https://zn.zhonguo7118.cn

PHP:  strpos($s, "x");
来源：https://dv.zhonguo7118.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：https://pr.zhonguo3118.cn

TS:   s.indexOf("x")
来源：https://ke.zhonguo5118.cn

Java: s.indexOf("x")
来源：https://tf.zhonguo5118.cn

Go:   strings.Index(s, "x")
来源：https://lz.zhonguo3118.cn

Ruby: s.index("x")
来源：https://xc.zhonguo7118.cn

C#:   s.IndexOf("x")
来源：https://nw.zhonguo6118.cn

[E05] 判断包含 / 前缀 / 后缀
来源：https://op.zhonguo5118.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：https://oi.zhonguo4118.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：https://lr.zhonguo4118.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：https://qc.zhonguo3118.cn

TS:   s.includes("x");  s.startsWith("a")
来源：https://cc.zhonguo2118.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：https://oj.zhonguo1118.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：https://wb.zhonguo4118.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：https://oc.zhonguo3118.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：https://tn.zhonguo3118.cn

[E06] 替换子串
来源：https://jc.zhonguo8118.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：https://jg.zhonguo6118.cn

PHP:  str_replace("a", "b", $s);
来源：https://ug.zhonguo7118.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://tp.zhonguo4118.cn

TS:   s.replaceAll("a", "b")
来源：https://ie.zhonguo7118.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://fu.zhonguo3118.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：https://ac.zhonguo5118.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：https://zt.zhonguo6118.cn

C#:   s.Replace("a", "b")
来源：https://ip.zhonguo7118.cn

[E07] 按分隔符拆分
来源：https://em.zhonguo2118.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：https://fh.zhonguo6118.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：https://hi.zhonguo1118.cn

JS:   s.split(",");  s.split(/\s+/)
来源：https://zx.zhonguo2118.cn

TS:   s.split(",")
来源：https://wq.zhonguo4118.cn

Java: s.split(",");  s.split("\\s+")
来源：https://cn.zhonguo3118.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：https://ta.zhonguo1118.cn

Ruby: s.split(",");  s.split
来源：https://tr.zhonguo7118.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：https://wr.zhonguo6118.cn

[E08] 数组按分隔符合并
来源：https://qh.zhonguo4118.cn

Py:   ",".join(items)
来源：https://of.zhonguo2118.cn

PHP:  implode(",", $items);
来源：https://kt.zhonguo4118.cn

JS:   items.join(",")
来源：https://rp.zhonguo8118.cn

TS:   items.join(",")
来源：https://ot.zhonguo7118.cn

Java: String.join(",", items)
来源：https://ao.zhonguo5118.cn

Go:   strings.Join(items, ",")
来源：https://kk.zhonguo7118.cn

Ruby: items.join(",")
来源：https://vj.zhonguo4118.cn

C#:   string.Join(",", items)
来源：https://rn.zhonguo7118.cn

[E09] 去除所有空白字符
来源：https://uj.zhonguo1118.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：https://qf.zhonguo4118.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：https://pw.zhonguo8118.cn

JS:   s.replace(/\s+/g, "")
来源：https://hh.zhonguo5118.cn

TS:   s.replace(/\s+/g, "")
来源：https://nn.zhonguo6118.cn

Java: s.replaceAll("\\s+", "")
来源：https://jc.zhonguo4118.cn

Go:   strings.Join(strings.Fields(s), "")
来源：https://gh.zhonguo1118.cn

Ruby: s.gsub(/\s+/, "")
来源：https://ti.zhonguo6118.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：https://kc.zhonguo2118.cn

[E10] 左侧补零 / 定长填充
来源：https://eb.zhonguo5118.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：https://wq.zhonguo6118.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：https://ki.zhonguo3118.cn

JS:   "7".padStart(3, "0")
来源：https://qx.zhonguo1118.cn

TS:   "7".padStart(3, "0")
来源：https://nl.zhonguo1118.cn

Java: String.format("%03d", 7)
来源：https://wr.zhonguo4118.cn

Go:   fmt.Sprintf("%03d", 7)
来源：https://ql.zhonguo5118.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：https://rk.zhonguo2118.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：https://fi.zhonguo2118.cn

[E11] 反转字符串
来源：https://bi.zhonguo8118.cn

Py:   s[::-1]
来源：https://se.zhonguo8118.cn

PHP:  strrev($s);
来源：https://qp.zhonguo5118.cn

JS:   [...s].reverse().join("")
来源：https://bv.zhonguo4118.cn

TS:   [...s].reverse().join("")
来源：https://cp.zhonguo2118.cn

Java: new StringBuilder(s).reverse().toString()
来源：https://sl.zhonguo7118.cn

Go:   // 转 []rune 后倒序再转回 string
来源：https://ce.zhonguo2118.cn

Ruby: s.reverse
来源：https://pa.zhonguo5118.cn

C#:   new string(s.Reverse().ToArray())
来源：https://dz.zhonguo2118.cn

[E12] 统计某字符出现次数
来源：https://jm.zhonguo8118.cn

Py:   s.count("a")
来源：https://vv.zhonguo2118.cn

PHP:  substr_count($s, "a");
来源：https://fh.zhonguo2118.cn

JS:   s.split("a").length - 1
来源：https://wx.zhonguo2118.cn

TS:   s.split("a").length - 1
来源：https://oa.zhonguo1118.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：https://zq.zhonguo7118.cn

Go:   strings.Count(s, "a")
来源：https://yz.zhonguo2118.cn

Ruby: s.count("a")
来源：https://tp.zhonguo2118.cn

C#:   s.Count(c => c == 'a')
来源：https://li.zhonguo8118.cn

[E13] 逐字符遍历
来源：https://lg.zhonguo7118.cn

Py:   for ch in s: print(ch)
来源：https://hu.zhonguo4118.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：https://dj.zhonguo4118.cn

JS:   for (const ch of s) { console.log(ch); }
来源：https://eu.zhonguo4118.cn

TS:   for (const ch of s) { console.log(ch); }
来源：https://ym.zhonguo5118.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：https://zd.zhonguo5118.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：https://aq.zhonguo7118.cn

Ruby: s.each_char { |ch| puts ch }
来源：https://sd.zhonguo5118.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：https://cs.zhonguo8118.cn

[E14] URL 编码与 Base64
来源：https://ys.zhonguo5118.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：https://zy.zhonguo7118.cn

PHP:  urlencode($s);  base64_encode($s);
来源：https://oo.zhonguo8118.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：https://zq.zhonguo2118.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：https://wu.zhonguo5118.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：https://hd.zhonguo5118.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：https://lu.zhonguo8118.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：https://ad.zhonguo8118.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：https://ck.zhonguo8118.cn

[E15] HTML 转义 / 反转义
来源：https://vn.zhonguo6118.cn

Py:   html.escape(s);  html.unescape(s)
来源：https://gx.zhonguo7118.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：https://eo.zhonguo2118.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：https://do.zhonguo2118.cn

TS:   // 同上，务必做 XSS 过滤
来源：https://fq.zhonguo3118.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：https://ef.zhonguo2118.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：https://sf.zhonguo2118.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：https://rz.zhonguo7118.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：https://yn.zhonguo6118.cn

[E16] 数字千分位
来源：https://yb.zhonguo3118.cn

Py:   f"{1234567:,}"
来源：https://dc.zhonguo1118.cn

PHP:  number_format(1234567);
来源：https://si.zhonguo1118.cn

JS:   (1234567).toLocaleString("en-US")
来源：https://kx.zhonguo1118.cn

TS:   (1234567).toLocaleString("en-US")
来源：https://tk.zhonguo6118.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：https://ux.zhonguo7118.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：https://qk.zhonguo7118.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：https://hu.zhonguo2118.cn

C#:   1234567.ToString("N0")
来源：https://ov.zhonguo2118.cn

[E17] 首字母大写
来源：https://gb.zhonguo3118.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：https://yw.zhonguo7118.cn

PHP:  ucfirst($s);  ucwords($s);
来源：https://th.zhonguo2118.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://xr.zhonguo6118.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://ob.zhonguo1118.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：https://ha.zhonguo6118.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：https://th.zhonguo4118.cn

Ruby: s.capitalize
来源：https://tv.zhonguo1118.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：https://gd.zhonguo4118.cn

[E18] 模板占位符替换
来源：https://pv.zhonguo4118.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：https://bf.zhonguo6118.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：https://at.zhonguo5118.cn

JS:   tpl.replaceAll("{name}", name)
来源：https://jh.zhonguo7118.cn


<!-- 参考信息 -->