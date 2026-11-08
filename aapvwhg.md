代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：https://xu.zhonguo8118.cn

JS:   arr.filter(x => x > 3)
来源：https://ih.zhonguo1118.cn

TS:   arr.filter(x => x > 3)
来源：https://qd.zhonguo3118.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：https://lk.zhonguo7118.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：https://bm.zhonguo4118.cn

Ruby: arr.select { |x| x > 3 }
来源：https://bw.zhonguo2118.cn

C#:   list.Where(x => x > 3).ToList()
来源：https://hc.zhonguo2118.cn

[D14] 映射转换（每个元素变形）
来源：https://mn.zhonguo7118.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：https://ct.zhonguo8118.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：https://bz.zhonguo4118.cn

JS:   arr.map(x => x * 2)
来源：https://ml.zhonguo4118.cn

TS:   arr.map(x => x * 2)
来源：https://ow.zhonguo1118.cn

Java: list.stream().map(x -> x * 2).toList()
来源：https://om.zhonguo4118.cn

Go:   // 手写循环
来源：https://mt.zhonguo5118.cn

Ruby: arr.map { |x| x * 2 }
来源：https://hr.zhonguo4118.cn

C#:   list.Select(x => x * 2).ToList()
来源：https://cn.zhonguo6118.cn

[D15] 去重
来源：https://xr.zhonguo1118.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：https://xv.zhonguo4118.cn

PHP:  array_unique($arr);
来源：https://si.zhonguo1118.cn

JS:   [...new Set(arr)]
来源：https://nj.zhonguo1118.cn

TS:   [...new Set(arr)]
来源：https://gt.zhonguo2118.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：https://mt.zhonguo6118.cn

Go:   // 用 map[T]struct{} 手写
来源：https://rm.zhonguo5118.cn

Ruby: arr.uniq
来源：https://vv.zhonguo6118.cn

C#:   list.Distinct().ToList()
来源：https://ls.zhonguo6118.cn

[D16] 求和与平均值
来源：https://uj.zhonguo1118.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：https://pd.zhonguo1118.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：https://ak.zhonguo3118.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：https://up.zhonguo3118.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：https://pr.zhonguo2118.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：https://jw.zhonguo8118.cn

Go:   // 手写循环累加
来源：https://ff.zhonguo1118.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：https://ac.zhonguo8118.cn

C#:   list.Sum();  list.Average()
来源：https://qy.zhonguo7118.cn

[D17] 最大值与最小值
来源：https://ra.zhonguo7118.cn

Py:   max(arr);  min(arr)
来源：https://dc.zhonguo6118.cn

PHP:  max($arr);  min($arr);
来源：https://wf.zhonguo5118.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：https://gv.zhonguo2118.cn

TS:   Math.max(...arr);
来源：https://ez.zhonguo3118.cn

Java: Collections.max(list);  Collections.min(list);
来源：https://ym.zhonguo5118.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：https://ax.zhonguo4118.cn

Ruby: arr.max;  arr.min
来源：https://yz.zhonguo2118.cn

C#:   list.Max();  list.Min()
来源：https://kl.zhonguo2118.cn

[D18] 扁平化嵌套数组
来源：https://kf.zhonguo4118.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：https://hy.zhonguo3118.cn

PHP:  array_merge(...$nested);
来源：https://bx.zhonguo5118.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：https://ej.zhonguo3118.cn

TS:   nested.flat();
来源：https://dy.zhonguo3118.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：https://zb.zhonguo4118.cn

Go:   // 手写双层循环
来源：https://yh.zhonguo2118.cn

Ruby: nested.flatten
来源：https://jx.zhonguo2118.cn

C#:   nested.SelectMany(x => x).ToList()
来源：https://fq.zhonguo3118.cn

[D19] 按字段分组
来源：https://nw.zhonguo8118.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：https://cw.zhonguo8118.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：https://ki.zhonguo5118.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：https://dh.zhonguo6118.cn

TS:   Object.groupBy(arr, x => x.type)
来源：https://hv.zhonguo7118.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：https://jp.zhonguo7118.cn

Go:   // 手写 map[string][]T
来源：https://ui.zhonguo3118.cn

Ruby: arr.group_by { |x| x[:type] }
来源：https://ux.zhonguo3118.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：https://xh.zhonguo1118.cn

[D20] 统计每个元素出现次数
来源：https://de.zhonguo8118.cn

Py:   Counter(arr)
来源：https://de.zhonguo3118.cn

PHP:  array_count_values($arr);
来源：https://kh.zhonguo8118.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://gl.zhonguo1118.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://oy.zhonguo4118.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：https://cv.zhonguo5118.cn

Go:   // 手写 map[T]int
来源：https://hr.zhonguo8118.cn

Ruby: arr.tally
来源：https://fv.zhonguo6118.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：https://jd.zhonguo7118.cn

[D21] 判断是否包含某元素
来源：https://la.zhonguo1118.cn

Py:   x in arr
来源：https://ga.zhonguo5118.cn

PHP:  in_array($x, $arr, true);
来源：https://wh.zhonguo3118.cn

JS:   arr.includes(x)
来源：https://rz.zhonguo1118.cn

TS:   arr.includes(x)
来源：https://cn.zhonguo5118.cn

Java: list.contains(x)
来源：https://qv.zhonguo8118.cn

Go:   slices.Contains(arr, x)
来源：https://to.zhonguo5118.cn

Ruby: arr.include?(x)
来源：https://zo.zhonguo2118.cn

C#:   list.Contains(x)
来源：https://fw.zhonguo1118.cn

[D22] 复制数组（避免共享引用）
来源：https://wa.zhonguo6118.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：https://jo.zhonguo4118.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：https://hj.zhonguo1118.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：https://no.zhonguo2118.cn

TS:   [...arr];
来源：https://so.zhonguo3118.cn

Java: new ArrayList<>(list);
来源：https://gh.zhonguo1118.cn

Go:   copied := append([]int(nil), arr...)
来源：https://gv.zhonguo3118.cn

Ruby: arr.dup;  arr.clone
来源：https://ow.zhonguo7118.cn

C#:   new List<int>(list);
来源：https://bc.zhonguo4118.cn

[D23] reduce 累积计算
来源：https://ww.zhonguo6118.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：https://ta.zhonguo5118.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：https://uw.zhonguo5118.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://or.zhonguo5118.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://jz.zhonguo5118.cn

Java: list.stream().reduce(0, Integer::sum)
来源：https://ef.zhonguo5118.cn

Go:   // 手写循环
来源：https://ul.zhonguo8118.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：https://js.zhonguo2118.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：https://se.zhonguo7118.cn

[D24] 字典 / Map 基本操作
来源：https://fe.zhonguo6118.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：https://qi.zhonguo7118.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：https://rh.zhonguo2118.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：https://nn.zhonguo2118.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：https://aq.zhonguo5118.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：https://pk.zhonguo4118.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：https://hd.zhonguo4118.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：https://bo.zhonguo8118.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：https://lj.zhonguo1118.cn

[D25] Set 集合去重与交并差
来源：https://cd.zhonguo8118.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：https://hl.zhonguo6118.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：https://ds.zhonguo7118.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：https://vl.zhonguo6118.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：https://yk.zhonguo6118.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：https://pk.zhonguo6118.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：https://mm.zhonguo4118.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：https://oe.zhonguo2118.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：https://ia.zhonguo1118.cn

[D26] 数组转字符串
来源：https://jj.zhonguo6118.cn

Py:   ", ".join(map(str, arr))
来源：https://ip.zhonguo7118.cn

PHP:  implode(", ", $arr);
来源：https://cm.zhonguo5118.cn

JS:   arr.join(", ")
来源：https://wm.zhonguo7118.cn

TS:   arr.join(", ")
来源：https://hc.zhonguo7118.cn

Java: String.join(", ", list)
来源：https://mw.zhonguo6118.cn

Go:   strings.Join(strs, ", ")
来源：https://in.zhonguo3118.cn

Ruby: arr.join(", ")
来源：https://hi.zhonguo3118.cn

C#:   string.Join(", ", list)
来源：https://di.zhonguo7118.cn

================================================================================
来源：https://xf.zhonguo7118.cn

E. 字符串处理
来源：https://ri.zhonguo3118.cn

================================================================================
来源：https://na.zhonguo3118.cn

[E01] 拼接字符串
来源：https://wl.zhonguo8118.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：https://jp.zhonguo4118.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：https://rg.zhonguo6118.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：https://pp.zhonguo1118.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：https://yo.zhonguo8118.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：https://gq.zhonguo6118.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：https://kt.zhonguo6118.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：https://xa.zhonguo8118.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：https://vl.zhonguo3118.cn

[E02] 重复字符串
来源：https://ba.zhonguo3118.cn

Py:   "ab" * 3
来源：https://ep.zhonguo5118.cn

PHP:  str_repeat("ab", 3);
来源：https://ov.zhonguo4118.cn

JS:   "ab".repeat(3)
来源：https://nm.zhonguo1118.cn

TS:   "ab".repeat(3)
来源：https://gn.zhonguo7118.cn

Java: "ab".repeat(3)
来源：https://eb.zhonguo2118.cn

Go:   strings.Repeat("ab", 3)
来源：https://gh.zhonguo6118.cn

Ruby: "ab" * 3
来源：https://qj.zhonguo3118.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：https://xn.zhonguo3118.cn

[E03] 截取子串
来源：https://zs.zhonguo6118.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：https://yf.zhonguo7118.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：https://rq.zhonguo1118.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：https://sm.zhonguo2118.cn

TS:   s.slice(1, 4)
来源：https://bf.zhonguo8118.cn

Java: s.substring(1, 4)
来源：https://kf.zhonguo1118.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：https://ti.zhonguo6118.cn

Ruby: s[1, 3];  s[1..3]
来源：https://oh.zhonguo1118.cn

C#:   s.Substring(1, 3)
来源：https://ha.zhonguo6118.cn

[E04] 查找子串位置
来源：https://ot.zhonguo6118.cn

Py:   s.find("x");  s.index("x")
来源：https://bb.zhonguo3118.cn

PHP:  strpos($s, "x");
来源：https://fa.zhonguo1118.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：https://oc.zhonguo1118.cn

TS:   s.indexOf("x")
来源：https://tx.zhonguo7118.cn

Java: s.indexOf("x")
来源：https://hb.zhonguo5118.cn

Go:   strings.Index(s, "x")
来源：https://so.zhonguo6118.cn

Ruby: s.index("x")
来源：https://vz.zhonguo4118.cn

C#:   s.IndexOf("x")
来源：https://kx.zhonguo4118.cn

[E05] 判断包含 / 前缀 / 后缀
来源：https://kn.zhonguo6118.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：https://ls.zhonguo1118.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：https://du.zhonguo5118.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：https://jy.zhonguo7118.cn

TS:   s.includes("x");  s.startsWith("a")
来源：https://rf.zhonguo1118.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：https://wb.zhonguo5118.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：https://th.zhonguo1118.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：https://qp.zhonguo5118.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：https://qp.zhonguo6118.cn

[E06] 替换子串
来源：https://ec.zhonguo6118.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：https://ea.zhonguo1118.cn

PHP:  str_replace("a", "b", $s);
来源：https://sb.zhonguo7118.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://oy.zhonguo3118.cn

TS:   s.replaceAll("a", "b")
来源：https://ch.zhonguo1118.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://rj.zhonguo4118.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：https://al.zhonguo6118.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：https://kd.zhonguo6118.cn

C#:   s.Replace("a", "b")
来源：https://ub.zhonguo2118.cn

[E07] 按分隔符拆分
来源：https://kf.zhonguo8118.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：https://uz.zhonguo8118.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：https://cf.zhonguo2118.cn

JS:   s.split(",");  s.split(/\s+/)
来源：https://qk.zhonguo3118.cn

TS:   s.split(",")
来源：https://bl.zhonguo3118.cn

Java: s.split(",");  s.split("\\s+")
来源：https://tu.zhonguo6118.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：https://du.zhonguo5118.cn

Ruby: s.split(",");  s.split
来源：https://ih.zhonguo7118.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：https://np.zhonguo1118.cn

[E08] 数组按分隔符合并
来源：https://ug.zhonguo2118.cn

Py:   ",".join(items)
来源：https://lp.zhonguo6118.cn

PHP:  implode(",", $items);
来源：https://st.zhonguo4118.cn

JS:   items.join(",")
来源：https://ku.zhonguo5118.cn

TS:   items.join(",")
来源：https://de.zhonguo4118.cn

Java: String.join(",", items)
来源：https://sy.zhonguo3118.cn

Go:   strings.Join(items, ",")
来源：https://kp.zhonguo2118.cn

Ruby: items.join(",")
来源：https://rh.zhonguo7118.cn

C#:   string.Join(",", items)
来源：https://yr.zhonguo3118.cn

[E09] 去除所有空白字符
来源：https://cx.zhonguo2118.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：https://ee.zhonguo4118.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：https://go.zhonguo5118.cn

JS:   s.replace(/\s+/g, "")
来源：https://if.zhonguo7118.cn

TS:   s.replace(/\s+/g, "")
来源：https://pi.zhonguo3118.cn

Java: s.replaceAll("\\s+", "")
来源：https://yr.zhonguo5118.cn

Go:   strings.Join(strings.Fields(s), "")
来源：https://gp.zhonguo6118.cn

Ruby: s.gsub(/\s+/, "")
来源：https://yf.zhonguo8118.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：https://jn.zhonguo4118.cn

[E10] 左侧补零 / 定长填充
来源：https://bx.zhonguo7118.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：https://dd.zhonguo2118.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：https://sz.zhonguo3118.cn

JS:   "7".padStart(3, "0")
来源：https://sw.zhonguo6118.cn

TS:   "7".padStart(3, "0")
来源：https://bx.zhonguo7118.cn

Java: String.format("%03d", 7)
来源：https://kk.zhonguo7118.cn

Go:   fmt.Sprintf("%03d", 7)
来源：https://op.zhonguo2118.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：https://yx.zhonguo8118.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：https://gk.zhonguo4118.cn

[E11] 反转字符串
来源：https://qy.zhonguo6118.cn

Py:   s[::-1]
来源：https://an.zhonguo5118.cn

PHP:  strrev($s);
来源：https://og.zhonguo4118.cn

JS:   [...s].reverse().join("")
来源：https://ue.zhonguo4118.cn

TS:   [...s].reverse().join("")
来源：https://ql.zhonguo8118.cn

Java: new StringBuilder(s).reverse().toString()
来源：https://tl.zhonguo3118.cn

Go:   // 转 []rune 后倒序再转回 string
来源：https://ry.zhonguo5118.cn

Ruby: s.reverse
来源：https://rt.zhonguo7118.cn

C#:   new string(s.Reverse().ToArray())
来源：https://ma.zhonguo4118.cn

[E12] 统计某字符出现次数
来源：https://ge.zhonguo1118.cn

Py:   s.count("a")
来源：https://is.zhonguo3118.cn

PHP:  substr_count($s, "a");
来源：https://em.zhonguo5118.cn

JS:   s.split("a").length - 1
来源：https://wj.zhonguo6118.cn

TS:   s.split("a").length - 1
来源：https://qc.zhonguo7118.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：https://yn.zhonguo7118.cn

Go:   strings.Count(s, "a")
来源：https://za.zhonguo8118.cn

Ruby: s.count("a")
来源：https://wf.zhonguo3118.cn

C#:   s.Count(c => c == 'a')
来源：https://ku.zhonguo5118.cn

[E13] 逐字符遍历
来源：https://wb.zhonguo2118.cn

Py:   for ch in s: print(ch)
来源：https://qv.zhonguo7118.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：https://op.zhonguo4118.cn

JS:   for (const ch of s) { console.log(ch); }
来源：https://we.zhonguo8118.cn

TS:   for (const ch of s) { console.log(ch); }
来源：https://xo.zhonguo1118.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：https://xt.zhonguo2118.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：https://kw.zhonguo2118.cn

Ruby: s.each_char { |ch| puts ch }
来源：https://yt.zhonguo5118.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：https://ay.zhonguo2118.cn

[E14] URL 编码与 Base64
来源：https://em.zhonguo4118.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：https://ae.zhonguo4118.cn

PHP:  urlencode($s);  base64_encode($s);
来源：https://eg.zhonguo3118.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：https://yq.zhonguo7118.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：https://rp.zhonguo4118.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：https://nm.zhonguo8118.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：https://rx.zhonguo1118.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：https://zv.zhonguo6118.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：https://te.zhonguo6118.cn

[E15] HTML 转义 / 反转义
来源：https://rk.zhonguo8118.cn

Py:   html.escape(s);  html.unescape(s)
来源：https://ep.zhonguo2118.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：https://gc.zhonguo1118.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：https://nd.zhonguo8118.cn

TS:   // 同上，务必做 XSS 过滤
来源：https://je.zhonguo3118.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：https://tu.zhonguo2118.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：https://ml.zhonguo1118.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：https://bi.zhonguo4118.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：https://eb.zhonguo2118.cn

[E16] 数字千分位
来源：https://oi.zhonguo5118.cn

Py:   f"{1234567:,}"
来源：https://kn.zhonguo7118.cn

PHP:  number_format(1234567);
来源：https://mv.zhonguo6118.cn

JS:   (1234567).toLocaleString("en-US")
来源：https://rv.zhonguo1118.cn

TS:   (1234567).toLocaleString("en-US")
来源：https://jj.zhonguo8118.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：https://lu.zhonguo4118.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：https://nt.zhonguo3118.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：https://wm.zhonguo7118.cn

C#:   1234567.ToString("N0")
来源：https://mn.zhonguo7118.cn

[E17] 首字母大写
来源：https://qh.zhonguo2118.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：https://hg.zhonguo1118.cn

PHP:  ucfirst($s);  ucwords($s);
来源：https://ft.zhonguo1118.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://tl.zhonguo1118.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://oo.zhonguo5118.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：https://pk.zhonguo5118.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：https://tw.zhonguo8118.cn

Ruby: s.capitalize
来源：https://du.zhonguo3118.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：https://wo.zhonguo4118.cn

[E18] 模板占位符替换
来源：https://vy.zhonguo1118.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：https://zg.zhonguo7118.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：https://xx.zhonguo1118.cn

JS:   tpl.replaceAll("{name}", name)
来源：https://ji.zhonguo5118.cn

TS:   tpl.replaceAll("{name}", name)
来源：https://ap.zhonguo3118.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：https://fz.zhonguo4118.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：https://az.zhonguo2118.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：https://si.zhonguo6118.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：https://av.zhonguo1118.cn

[E19] 多行文本按行拆分
来源：https://ej.zhonguo1118.cn

Py:   s.splitlines()
来源：https://in.zhonguo8118.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：https://zd.zhonguo3118.cn

JS:   s.split(/\r?\n/)
来源：https://kd.zhonguo1118.cn

TS:   s.split(/\r?\n/)
来源：https://nr.zhonguo7118.cn

Java: s.lines().toList()
来源：https://na.zhonguo4118.cn

Go:   strings.Split(s, "\n")
来源：https://zt.zhonguo2118.cn

Ruby: s.lines
来源：https://ju.zhonguo1118.cn

C#:   s.Split('\n')
来源：https://gt.zhonguo8118.cn

[E20] 判断字符串是否为空
来源：https://ry.zhonguo8118.cn

Py:   if not s:
来源：https://hl.zhonguo5118.cn


<!-- 参考信息 -->