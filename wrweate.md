代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：https://tp.zhonguo2118.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：https://pr.zhonguo1118.cn

JS:   arr.map(x => x * 2)
来源：https://go.zhonguo2118.cn

TS:   arr.map(x => x * 2)
来源：https://qm.zhonguo8118.cn

Java: list.stream().map(x -> x * 2).toList()
来源：https://ws.zhonguo4118.cn

Go:   // 手写循环
来源：https://ym.zhonguo4118.cn

Ruby: arr.map { |x| x * 2 }
来源：https://sp.zhonguo3118.cn

C#:   list.Select(x => x * 2).ToList()
来源：https://wl.zhonguo7118.cn

[D15] 去重
来源：https://wa.zhonguo2118.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：https://ds.zhonguo6118.cn

PHP:  array_unique($arr);
来源：https://yr.zhonguo6118.cn

JS:   [...new Set(arr)]
来源：https://mt.zhonguo8118.cn

TS:   [...new Set(arr)]
来源：https://ql.zhonguo8118.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：https://xa.zhonguo5118.cn

Go:   // 用 map[T]struct{} 手写
来源：https://rr.zhonguo1118.cn

Ruby: arr.uniq
来源：https://td.zhonguo2118.cn

C#:   list.Distinct().ToList()
来源：https://eh.zhonguo5118.cn

[D16] 求和与平均值
来源：https://di.zhonguo2118.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：https://tv.zhonguo3118.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：https://vd.zhonguo3118.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：https://xh.zhonguo7118.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：https://yi.zhonguo2118.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：https://aa.zhonguo3118.cn

Go:   // 手写循环累加
来源：https://ky.zhonguo5118.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：https://wo.zhonguo1118.cn

C#:   list.Sum();  list.Average()
来源：https://xu.zhonguo8118.cn

[D17] 最大值与最小值
来源：https://bj.zhonguo7118.cn

Py:   max(arr);  min(arr)
来源：https://rx.zhonguo1118.cn

PHP:  max($arr);  min($arr);
来源：https://rn.zhonguo4118.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：https://gy.zhonguo8118.cn

TS:   Math.max(...arr);
来源：https://ru.zhonguo2118.cn

Java: Collections.max(list);  Collections.min(list);
来源：https://vq.zhonguo1118.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：https://dp.zhonguo6118.cn

Ruby: arr.max;  arr.min
来源：https://bg.zhonguo7118.cn

C#:   list.Max();  list.Min()
来源：https://oi.zhonguo3118.cn

[D18] 扁平化嵌套数组
来源：https://vy.zhonguo4118.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：https://sj.zhonguo6118.cn

PHP:  array_merge(...$nested);
来源：https://xz.zhonguo1118.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：https://qb.zhonguo4118.cn

TS:   nested.flat();
来源：https://ca.zhonguo2118.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：https://at.zhonguo4118.cn

Go:   // 手写双层循环
来源：https://fj.zhonguo1118.cn

Ruby: nested.flatten
来源：https://zp.zhonguo2118.cn

C#:   nested.SelectMany(x => x).ToList()
来源：https://yg.zhonguo3118.cn

[D19] 按字段分组
来源：https://dh.zhonguo6118.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：https://pa.zhonguo7118.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：https://oi.zhonguo8118.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：https://je.zhonguo6118.cn

TS:   Object.groupBy(arr, x => x.type)
来源：https://mh.zhonguo6118.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：https://lq.zhonguo8118.cn

Go:   // 手写 map[string][]T
来源：https://qc.zhonguo5118.cn

Ruby: arr.group_by { |x| x[:type] }
来源：https://rt.zhonguo5118.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：https://pv.zhonguo1118.cn

[D20] 统计每个元素出现次数
来源：https://we.zhonguo2118.cn

Py:   Counter(arr)
来源：https://ey.zhonguo2118.cn

PHP:  array_count_values($arr);
来源：https://no.zhonguo7118.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://tr.zhonguo4118.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://rb.zhonguo8118.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：https://pw.zhonguo6118.cn

Go:   // 手写 map[T]int
来源：https://wu.zhonguo1118.cn

Ruby: arr.tally
来源：https://yf.zhonguo2118.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：https://km.zhonguo8118.cn

[D21] 判断是否包含某元素
来源：https://id.zhonguo1118.cn

Py:   x in arr
来源：https://ls.zhonguo5118.cn

PHP:  in_array($x, $arr, true);
来源：https://ar.zhonguo6118.cn

JS:   arr.includes(x)
来源：https://as.zhonguo8118.cn

TS:   arr.includes(x)
来源：https://xf.zhonguo7118.cn

Java: list.contains(x)
来源：https://xm.zhonguo3118.cn

Go:   slices.Contains(arr, x)
来源：https://kb.zhonguo6118.cn

Ruby: arr.include?(x)
来源：https://gy.zhonguo2118.cn

C#:   list.Contains(x)
来源：https://hp.zhonguo1118.cn

[D22] 复制数组（避免共享引用）
来源：https://pk.zhonguo8118.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：https://cc.zhonguo2118.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：https://qe.zhonguo1118.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：https://lt.zhonguo8118.cn

TS:   [...arr];
来源：https://wx.zhonguo4118.cn

Java: new ArrayList<>(list);
来源：https://gb.zhonguo7118.cn

Go:   copied := append([]int(nil), arr...)
来源：https://du.zhonguo3118.cn

Ruby: arr.dup;  arr.clone
来源：https://oc.zhonguo3118.cn

C#:   new List<int>(list);
来源：https://zw.zhonguo3118.cn

[D23] reduce 累积计算
来源：https://ct.zhonguo4118.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：https://nh.zhonguo6118.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：https://zw.zhonguo5118.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://ko.zhonguo7118.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://mk.zhonguo6118.cn

Java: list.stream().reduce(0, Integer::sum)
来源：https://th.zhonguo2118.cn

Go:   // 手写循环
来源：https://cf.zhonguo1118.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：https://fm.zhonguo2118.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：https://uj.zhonguo1118.cn

[D24] 字典 / Map 基本操作
来源：https://vo.zhonguo2118.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：https://gx.zhonguo4118.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：https://dn.zhonguo5118.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：https://sv.zhonguo2118.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：https://oh.zhonguo3118.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：https://td.zhonguo1118.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：https://pw.zhonguo6118.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：https://xr.zhonguo4118.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：https://vv.zhonguo4118.cn

[D25] Set 集合去重与交并差
来源：https://ce.zhonguo6118.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：https://zg.zhonguo8118.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：https://qg.zhonguo1118.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：https://zv.zhonguo6118.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：https://uj.zhonguo1118.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：https://hv.zhonguo3118.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：https://fg.zhonguo1118.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：https://uw.zhonguo7118.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：https://kk.zhonguo7118.cn

[D26] 数组转字符串
来源：https://xo.zhonguo6118.cn

Py:   ", ".join(map(str, arr))
来源：https://ob.zhonguo3118.cn

PHP:  implode(", ", $arr);
来源：https://eu.zhonguo2118.cn

JS:   arr.join(", ")
来源：https://sj.zhonguo7118.cn

TS:   arr.join(", ")
来源：https://nb.zhonguo8118.cn

Java: String.join(", ", list)
来源：https://fv.zhonguo2118.cn

Go:   strings.Join(strs, ", ")
来源：https://rx.zhonguo7118.cn

Ruby: arr.join(", ")
来源：https://rs.zhonguo1118.cn

C#:   string.Join(", ", list)
来源：https://ut.zhonguo1118.cn

================================================================================
来源：https://um.zhonguo3118.cn

E. 字符串处理
来源：https://ud.zhonguo4118.cn

================================================================================
来源：https://dv.zhonguo3118.cn

[E01] 拼接字符串
来源：https://gj.zhonguo4118.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：https://uu.zhonguo2118.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：https://ug.zhonguo8118.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：https://od.zhonguo4118.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：https://uh.zhonguo8118.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：https://fl.zhonguo5118.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：https://fl.zhonguo4118.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：https://dm.zhonguo8118.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：https://tq.zhonguo1118.cn

[E02] 重复字符串
来源：https://ge.zhonguo2118.cn

Py:   "ab" * 3
来源：https://sx.zhonguo6118.cn

PHP:  str_repeat("ab", 3);
来源：https://ei.zhonguo8118.cn

JS:   "ab".repeat(3)
来源：https://ls.zhonguo5118.cn

TS:   "ab".repeat(3)
来源：https://ts.zhonguo8118.cn

Java: "ab".repeat(3)
来源：https://sl.zhonguo2118.cn

Go:   strings.Repeat("ab", 3)
来源：https://ee.zhonguo5118.cn

Ruby: "ab" * 3
来源：https://yu.zhonguo5118.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：https://jz.zhonguo6118.cn

[E03] 截取子串
来源：https://xe.zhonguo8118.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：https://ka.zhonguo7118.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：https://di.zhonguo3118.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：https://px.zhonguo8118.cn

TS:   s.slice(1, 4)
来源：https://kk.zhonguo2118.cn

Java: s.substring(1, 4)
来源：https://yb.zhonguo4118.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：https://ak.zhonguo6118.cn

Ruby: s[1, 3];  s[1..3]
来源：https://gg.zhonguo7118.cn

C#:   s.Substring(1, 3)
来源：https://xo.zhonguo1118.cn

[E04] 查找子串位置
来源：https://te.zhonguo5118.cn

Py:   s.find("x");  s.index("x")
来源：https://zz.zhonguo8118.cn

PHP:  strpos($s, "x");
来源：https://qg.zhonguo3118.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：https://dk.zhonguo8118.cn

TS:   s.indexOf("x")
来源：https://hj.zhonguo5118.cn

Java: s.indexOf("x")
来源：https://pj.zhonguo8118.cn

Go:   strings.Index(s, "x")
来源：https://ie.zhonguo3118.cn

Ruby: s.index("x")
来源：https://mi.zhonguo6118.cn

C#:   s.IndexOf("x")
来源：https://fd.zhonguo7118.cn

[E05] 判断包含 / 前缀 / 后缀
来源：https://pe.zhonguo3118.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：https://yp.zhonguo1118.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：https://ur.zhonguo4118.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：https://om.zhonguo6118.cn

TS:   s.includes("x");  s.startsWith("a")
来源：https://zb.zhonguo4118.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：https://cr.zhonguo7118.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：https://gi.zhonguo6118.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：https://sz.zhonguo6118.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：https://tc.zhonguo8118.cn

[E06] 替换子串
来源：https://ea.zhonguo8118.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：https://ev.zhonguo5118.cn

PHP:  str_replace("a", "b", $s);
来源：https://cy.zhonguo3118.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://vl.zhonguo6118.cn

TS:   s.replaceAll("a", "b")
来源：https://lf.zhonguo3118.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://hm.zhonguo3118.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：https://ha.zhonguo5118.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：https://qo.zhonguo8118.cn

C#:   s.Replace("a", "b")
来源：https://dz.zhonguo4118.cn

[E07] 按分隔符拆分
来源：https://uc.zhonguo8118.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：https://mw.zhonguo3118.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：https://dr.zhonguo3118.cn

JS:   s.split(",");  s.split(/\s+/)
来源：https://jf.zhonguo6118.cn

TS:   s.split(",")
来源：https://lp.zhonguo8118.cn

Java: s.split(",");  s.split("\\s+")
来源：https://ma.zhonguo3118.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：https://ow.zhonguo6118.cn

Ruby: s.split(",");  s.split
来源：https://xj.zhonguo6118.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：https://cb.zhonguo8118.cn

[E08] 数组按分隔符合并
来源：https://uc.zhonguo1118.cn

Py:   ",".join(items)
来源：https://ff.zhonguo8118.cn

PHP:  implode(",", $items);
来源：https://be.zhonguo8118.cn

JS:   items.join(",")
来源：https://nx.zhonguo5118.cn

TS:   items.join(",")
来源：https://if.zhonguo8118.cn

Java: String.join(",", items)
来源：https://wt.zhonguo8118.cn

Go:   strings.Join(items, ",")
来源：https://ix.zhonguo2118.cn

Ruby: items.join(",")
来源：https://kd.zhonguo6118.cn

C#:   string.Join(",", items)
来源：https://fd.zhonguo5118.cn

[E09] 去除所有空白字符
来源：https://bu.zhonguo8118.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：https://ip.zhonguo6118.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：https://bu.zhonguo6118.cn

JS:   s.replace(/\s+/g, "")
来源：https://mh.zhonguo7118.cn

TS:   s.replace(/\s+/g, "")
来源：https://hx.zhonguo7118.cn

Java: s.replaceAll("\\s+", "")
来源：https://tx.zhonguo7118.cn

Go:   strings.Join(strings.Fields(s), "")
来源：https://tv.zhonguo4118.cn

Ruby: s.gsub(/\s+/, "")
来源：https://hf.zhonguo6118.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：https://se.zhonguo2118.cn

[E10] 左侧补零 / 定长填充
来源：https://zx.zhonguo5118.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：https://gm.zhonguo6118.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：https://md.zhonguo8118.cn

JS:   "7".padStart(3, "0")
来源：https://pz.zhonguo2118.cn

TS:   "7".padStart(3, "0")
来源：https://rz.zhonguo8118.cn

Java: String.format("%03d", 7)
来源：https://wq.zhonguo5118.cn

Go:   fmt.Sprintf("%03d", 7)
来源：https://tm.zhonguo4118.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：https://vg.zhonguo8118.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：https://fc.zhonguo7118.cn

[E11] 反转字符串
来源：https://ly.zhonguo5118.cn

Py:   s[::-1]
来源：https://ju.zhonguo1118.cn

PHP:  strrev($s);
来源：https://ds.zhonguo7118.cn

JS:   [...s].reverse().join("")
来源：https://aa.zhonguo4118.cn

TS:   [...s].reverse().join("")
来源：https://cq.zhonguo5118.cn

Java: new StringBuilder(s).reverse().toString()
来源：https://mm.zhonguo4118.cn

Go:   // 转 []rune 后倒序再转回 string
来源：https://gf.zhonguo4118.cn

Ruby: s.reverse
来源：https://mn.zhonguo3118.cn

C#:   new string(s.Reverse().ToArray())
来源：https://vs.zhonguo5118.cn

[E12] 统计某字符出现次数
来源：https://mo.zhonguo5118.cn

Py:   s.count("a")
来源：https://lp.zhonguo2118.cn

PHP:  substr_count($s, "a");
来源：https://jh.zhonguo7118.cn

JS:   s.split("a").length - 1
来源：https://iu.zhonguo1118.cn

TS:   s.split("a").length - 1
来源：https://bn.zhonguo7118.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：https://bn.zhonguo5118.cn

Go:   strings.Count(s, "a")
来源：https://oa.zhonguo3118.cn

Ruby: s.count("a")
来源：https://rd.zhonguo3118.cn

C#:   s.Count(c => c == 'a')
来源：https://vk.zhonguo8118.cn

[E13] 逐字符遍历
来源：https://ek.zhonguo6118.cn

Py:   for ch in s: print(ch)
来源：https://zk.zhonguo7118.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：https://zh.zhonguo4118.cn

JS:   for (const ch of s) { console.log(ch); }
来源：https://is.zhonguo4118.cn

TS:   for (const ch of s) { console.log(ch); }
来源：https://ap.zhonguo4118.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：https://zu.zhonguo5118.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：https://oz.zhonguo8118.cn

Ruby: s.each_char { |ch| puts ch }
来源：https://hk.zhonguo8118.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：https://pc.zhonguo7118.cn

[E14] URL 编码与 Base64
来源：https://mo.zhonguo3118.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：https://tu.zhonguo8118.cn

PHP:  urlencode($s);  base64_encode($s);
来源：https://hx.zhonguo5118.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：https://ri.zhonguo6118.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：https://yn.zhonguo5118.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：https://iy.zhonguo6118.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：https://kh.zhonguo3118.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：https://sl.zhonguo4118.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：https://rl.zhonguo5118.cn

[E15] HTML 转义 / 反转义
来源：https://hb.zhonguo4118.cn

Py:   html.escape(s);  html.unescape(s)
来源：https://nk.zhonguo4118.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：https://bi.zhonguo4118.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：https://ao.zhonguo4118.cn

TS:   // 同上，务必做 XSS 过滤
来源：https://ey.zhonguo3118.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：https://vc.zhonguo1118.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：https://ye.zhonguo2118.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：https://uc.zhonguo5118.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：https://oq.zhonguo5118.cn

[E16] 数字千分位
来源：https://sb.zhonguo6118.cn

Py:   f"{1234567:,}"
来源：https://ny.zhonguo7118.cn

PHP:  number_format(1234567);
来源：https://pl.zhonguo2118.cn

JS:   (1234567).toLocaleString("en-US")
来源：https://wa.zhonguo2118.cn

TS:   (1234567).toLocaleString("en-US")
来源：https://fc.zhonguo8118.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：https://hh.zhonguo1118.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：https://pz.zhonguo7118.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：https://sv.zhonguo2118.cn

C#:   1234567.ToString("N0")
来源：https://qt.zhonguo7118.cn

[E17] 首字母大写
来源：https://uw.zhonguo2118.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：https://uy.zhonguo7118.cn

PHP:  ucfirst($s);  ucwords($s);
来源：https://an.zhonguo7118.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://vi.zhonguo8118.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://wc.zhonguo8118.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：https://lt.zhonguo7118.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：https://xx.zhonguo3118.cn

Ruby: s.capitalize
来源：https://qn.zhonguo7118.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：https://xf.zhonguo7118.cn

[E18] 模板占位符替换
来源：https://fp.zhonguo6118.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：https://zy.zhonguo7118.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：https://zn.zhonguo3118.cn

JS:   tpl.replaceAll("{name}", name)
来源：https://pl.zhonguo2118.cn

TS:   tpl.replaceAll("{name}", name)
来源：https://xc.zhonguo8118.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：https://bl.zhonguo4118.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：https://nb.zhonguo1118.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：https://ma.zhonguo4118.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：https://br.zhonguo4118.cn

[E19] 多行文本按行拆分
来源：https://wq.zhonguo8118.cn

Py:   s.splitlines()
来源：https://dp.zhonguo5118.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：https://dv.zhonguo2118.cn

JS:   s.split(/\r?\n/)
来源：https://lh.zhonguo5118.cn

TS:   s.split(/\r?\n/)
来源：https://ss.zhonguo4118.cn

Java: s.lines().toList()
来源：https://ii.zhonguo2118.cn

Go:   strings.Split(s, "\n")
来源：https://ne.zhonguo6118.cn

Ruby: s.lines
来源：https://qy.zhonguo6118.cn

C#:   s.Split('\n')
来源：https://ak.zhonguo6118.cn

[E20] 判断字符串是否为空
来源：https://hi.zhonguo1118.cn

Py:   if not s:
来源：https://vl.zhonguo3118.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：https://te.zhonguo8118.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：https://jp.zhonguo6118.cn

TS:   if (s === "") {}
来源：https://kl.zhonguo8118.cn

Java: if (s.isEmpty()) {}
来源：https://ud.zhonguo8118.cn

Go:   if s == "" {}
来源：https://gb.zhonguo7118.cn

Ruby: if s.empty?
来源：https://zx.zhonguo4118.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：https://tm.zhonguo6118.cn

[E21] 超长截断加省略号
来源：https://ur.zhonguo1118.cn


<!-- 参考信息 -->