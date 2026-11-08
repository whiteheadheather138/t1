代发 wailian999

PHP:  max($arr);  min($arr);
来源：https://lm.zhonguo3118.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：https://uv.zhonguo3118.cn

TS:   Math.max(...arr);
来源：https://xh.zhonguo2118.cn

Java: Collections.max(list);  Collections.min(list);
来源：https://mx.zhonguo3118.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：https://le.zhonguo8118.cn

Ruby: arr.max;  arr.min
来源：https://jw.zhonguo1118.cn

C#:   list.Max();  list.Min()
来源：https://qe.zhonguo8118.cn

[D18] 扁平化嵌套数组
来源：https://yc.zhonguo5118.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：https://aq.zhonguo4118.cn

PHP:  array_merge(...$nested);
来源：https://xv.zhonguo3118.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：https://jz.zhonguo5118.cn

TS:   nested.flat();
来源：https://kx.zhonguo2118.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：https://it.zhonguo7118.cn

Go:   // 手写双层循环
来源：https://es.zhonguo3118.cn

Ruby: nested.flatten
来源：https://li.zhonguo7118.cn

C#:   nested.SelectMany(x => x).ToList()
来源：https://gc.zhonguo6118.cn

[D19] 按字段分组
来源：https://sk.zhonguo8118.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：https://ya.zhonguo4118.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：https://yy.zhonguo1118.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：https://gi.zhonguo8118.cn

TS:   Object.groupBy(arr, x => x.type)
来源：https://sy.zhonguo6118.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：https://jk.zhonguo4118.cn

Go:   // 手写 map[string][]T
来源：https://ff.zhonguo5118.cn

Ruby: arr.group_by { |x| x[:type] }
来源：https://ws.zhonguo8118.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：https://mn.zhonguo6118.cn

[D20] 统计每个元素出现次数
来源：https://wk.zhonguo3118.cn

Py:   Counter(arr)
来源：https://qb.zhonguo1118.cn

PHP:  array_count_values($arr);
来源：https://ok.zhonguo3118.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://nj.zhonguo2118.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://mu.zhonguo8118.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：https://dl.zhonguo5118.cn

Go:   // 手写 map[T]int
来源：https://ru.zhonguo1118.cn

Ruby: arr.tally
来源：https://tk.zhonguo6118.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：https://cu.zhonguo8118.cn

[D21] 判断是否包含某元素
来源：https://ny.zhonguo6118.cn

Py:   x in arr
来源：https://gl.zhonguo5118.cn

PHP:  in_array($x, $arr, true);
来源：https://fl.zhonguo7118.cn

JS:   arr.includes(x)
来源：https://xr.zhonguo8118.cn

TS:   arr.includes(x)
来源：https://pd.zhonguo3118.cn

Java: list.contains(x)
来源：https://gd.zhonguo6118.cn

Go:   slices.Contains(arr, x)
来源：https://yt.zhonguo7118.cn

Ruby: arr.include?(x)
来源：https://oo.zhonguo7118.cn

C#:   list.Contains(x)
来源：https://an.zhonguo1118.cn

[D22] 复制数组（避免共享引用）
来源：https://ma.zhonguo2118.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：https://ft.zhonguo3118.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：https://pu.zhonguo8118.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：https://gc.zhonguo4118.cn

TS:   [...arr];
来源：https://ar.zhonguo3118.cn

Java: new ArrayList<>(list);
来源：https://oi.zhonguo5118.cn

Go:   copied := append([]int(nil), arr...)
来源：https://pf.zhonguo1118.cn

Ruby: arr.dup;  arr.clone
来源：https://yt.zhonguo1118.cn

C#:   new List<int>(list);
来源：https://wl.zhonguo3118.cn

[D23] reduce 累积计算
来源：https://wp.zhonguo6118.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：https://ud.zhonguo5118.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：https://wz.zhonguo4118.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://qw.zhonguo5118.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://qs.zhonguo4118.cn

Java: list.stream().reduce(0, Integer::sum)
来源：https://xn.zhonguo7118.cn

Go:   // 手写循环
来源：https://zy.zhonguo1118.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：https://ml.zhonguo6118.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：https://wg.zhonguo4118.cn

[D24] 字典 / Map 基本操作
来源：https://tn.zhonguo2118.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：https://ld.zhonguo2118.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：https://ed.zhonguo2118.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：https://du.zhonguo4118.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：https://bm.zhonguo5118.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：https://qg.zhonguo3118.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：https://vd.zhonguo4118.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：https://ac.zhonguo6118.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：https://po.zhonguo8118.cn

[D25] Set 集合去重与交并差
来源：https://xr.zhonguo4118.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：https://tm.zhonguo5118.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：https://yu.zhonguo6118.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：https://di.zhonguo5118.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：https://sk.zhonguo5118.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：https://wv.zhonguo7118.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：https://tc.zhonguo6118.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：https://hz.zhonguo2118.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：https://id.zhonguo1118.cn

[D26] 数组转字符串
来源：https://pq.zhonguo5118.cn

Py:   ", ".join(map(str, arr))
来源：https://le.zhonguo3118.cn

PHP:  implode(", ", $arr);
来源：https://dn.zhonguo8118.cn

JS:   arr.join(", ")
来源：https://rh.zhonguo3118.cn

TS:   arr.join(", ")
来源：https://cs.zhonguo7118.cn

Java: String.join(", ", list)
来源：https://qg.zhonguo6118.cn

Go:   strings.Join(strs, ", ")
来源：https://on.zhonguo5118.cn

Ruby: arr.join(", ")
来源：https://ac.zhonguo5118.cn

C#:   string.Join(", ", list)
来源：https://db.zhonguo5118.cn

================================================================================
来源：https://ad.zhonguo1118.cn

E. 字符串处理
来源：https://ee.zhonguo6118.cn

================================================================================
来源：https://yt.zhonguo5118.cn

[E01] 拼接字符串
来源：https://si.zhonguo3118.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：https://fe.zhonguo5118.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：https://qe.zhonguo6118.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：https://fd.zhonguo4118.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：https://uv.zhonguo6118.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：https://xl.zhonguo8118.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：https://fu.zhonguo7118.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：https://gv.zhonguo7118.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：https://ks.zhonguo2118.cn

[E02] 重复字符串
来源：https://zr.zhonguo3118.cn

Py:   "ab" * 3
来源：https://pm.zhonguo2118.cn

PHP:  str_repeat("ab", 3);
来源：https://wu.zhonguo4118.cn

JS:   "ab".repeat(3)
来源：https://dh.zhonguo7118.cn

TS:   "ab".repeat(3)
来源：https://rz.zhonguo7118.cn

Java: "ab".repeat(3)
来源：https://bd.zhonguo7118.cn

Go:   strings.Repeat("ab", 3)
来源：https://sv.zhonguo8118.cn

Ruby: "ab" * 3
来源：https://gg.zhonguo3118.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：https://ik.zhonguo6118.cn

[E03] 截取子串
来源：https://xe.zhonguo5118.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：https://cl.zhonguo5118.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：https://db.zhonguo6118.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：https://yc.zhonguo7118.cn

TS:   s.slice(1, 4)
来源：https://tq.zhonguo7118.cn

Java: s.substring(1, 4)
来源：https://nw.zhonguo2118.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：https://pl.zhonguo1118.cn

Ruby: s[1, 3];  s[1..3]
来源：https://vd.zhonguo6118.cn

C#:   s.Substring(1, 3)
来源：https://gt.zhonguo1118.cn

[E04] 查找子串位置
来源：https://vg.zhonguo6118.cn

Py:   s.find("x");  s.index("x")
来源：https://nt.zhonguo5118.cn

PHP:  strpos($s, "x");
来源：https://bb.zhonguo4118.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：https://kp.zhonguo5118.cn

TS:   s.indexOf("x")
来源：https://rg.zhonguo5118.cn

Java: s.indexOf("x")
来源：https://ir.zhonguo5118.cn

Go:   strings.Index(s, "x")
来源：https://ej.zhonguo3118.cn

Ruby: s.index("x")
来源：https://ch.zhonguo5118.cn

C#:   s.IndexOf("x")
来源：https://it.zhonguo8118.cn

[E05] 判断包含 / 前缀 / 后缀
来源：https://vp.zhonguo5118.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：https://tt.zhonguo3118.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：https://zc.zhonguo6118.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：https://qc.zhonguo2118.cn

TS:   s.includes("x");  s.startsWith("a")
来源：https://kv.zhonguo4118.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：https://tr.zhonguo2118.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：https://er.zhonguo7118.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：https://tt.zhonguo3118.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：https://kq.zhonguo4118.cn

[E06] 替换子串
来源：https://gt.zhonguo2118.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：https://ay.zhonguo4118.cn

PHP:  str_replace("a", "b", $s);
来源：https://gk.zhonguo5118.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://kr.zhonguo5118.cn

TS:   s.replaceAll("a", "b")
来源：https://gt.zhonguo1118.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://dr.zhonguo4118.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：https://nq.zhonguo2118.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：https://tp.zhonguo2118.cn

C#:   s.Replace("a", "b")
来源：https://rc.zhonguo2118.cn

[E07] 按分隔符拆分
来源：https://tl.zhonguo3118.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：https://kf.zhonguo5118.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：https://af.zhonguo4118.cn

JS:   s.split(",");  s.split(/\s+/)
来源：https://zj.zhonguo3118.cn

TS:   s.split(",")
来源：https://xl.zhonguo3118.cn

Java: s.split(",");  s.split("\\s+")
来源：https://uk.zhonguo5118.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：https://xc.zhonguo6118.cn

Ruby: s.split(",");  s.split
来源：https://tw.zhonguo6118.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：https://ql.zhonguo1118.cn

[E08] 数组按分隔符合并
来源：https://jv.zhonguo5118.cn

Py:   ",".join(items)
来源：https://tk.zhonguo5118.cn

PHP:  implode(",", $items);
来源：https://lb.zhonguo3118.cn

JS:   items.join(",")
来源：https://oh.zhonguo5118.cn

TS:   items.join(",")
来源：https://gy.zhonguo4118.cn

Java: String.join(",", items)
来源：https://xj.zhonguo5118.cn

Go:   strings.Join(items, ",")
来源：https://bs.zhonguo2118.cn

Ruby: items.join(",")
来源：https://oq.zhonguo7118.cn

C#:   string.Join(",", items)
来源：https://kp.zhonguo4118.cn

[E09] 去除所有空白字符
来源：https://vn.zhonguo5118.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：https://kk.zhonguo2118.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：https://rg.zhonguo1118.cn

JS:   s.replace(/\s+/g, "")
来源：https://qj.zhonguo4118.cn

TS:   s.replace(/\s+/g, "")
来源：https://ng.zhonguo7118.cn

Java: s.replaceAll("\\s+", "")
来源：https://ee.zhonguo4118.cn

Go:   strings.Join(strings.Fields(s), "")
来源：https://qk.zhonguo7118.cn

Ruby: s.gsub(/\s+/, "")
来源：https://kb.zhonguo7118.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：https://fn.zhonguo8118.cn

[E10] 左侧补零 / 定长填充
来源：https://go.zhonguo6118.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：https://ts.zhonguo4118.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：https://ps.zhonguo1118.cn

JS:   "7".padStart(3, "0")
来源：https://hy.zhonguo5118.cn

TS:   "7".padStart(3, "0")
来源：https://yl.zhonguo2118.cn

Java: String.format("%03d", 7)
来源：https://bz.zhonguo5118.cn

Go:   fmt.Sprintf("%03d", 7)
来源：https://re.zhonguo5118.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：https://qq.zhonguo4118.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：https://ww.zhonguo1118.cn

[E11] 反转字符串
来源：https://sp.zhonguo5118.cn

Py:   s[::-1]
来源：https://ku.zhonguo7118.cn

PHP:  strrev($s);
来源：https://gn.zhonguo1118.cn

JS:   [...s].reverse().join("")
来源：https://lp.zhonguo6118.cn

TS:   [...s].reverse().join("")
来源：https://pc.zhonguo4118.cn

Java: new StringBuilder(s).reverse().toString()
来源：https://lv.zhonguo5118.cn

Go:   // 转 []rune 后倒序再转回 string
来源：https://jw.zhonguo2118.cn

Ruby: s.reverse
来源：https://zq.zhonguo6118.cn

C#:   new string(s.Reverse().ToArray())
来源：https://ca.zhonguo8118.cn

[E12] 统计某字符出现次数
来源：https://yu.zhonguo1118.cn

Py:   s.count("a")
来源：https://pg.zhonguo5118.cn

PHP:  substr_count($s, "a");
来源：https://ik.zhonguo2118.cn

JS:   s.split("a").length - 1
来源：https://si.zhonguo2118.cn

TS:   s.split("a").length - 1
来源：https://ei.zhonguo2118.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：https://mv.zhonguo6118.cn

Go:   strings.Count(s, "a")
来源：https://uc.zhonguo1118.cn

Ruby: s.count("a")
来源：https://cv.zhonguo5118.cn

C#:   s.Count(c => c == 'a')
来源：https://rq.zhonguo8118.cn

[E13] 逐字符遍历
来源：https://db.zhonguo1118.cn

Py:   for ch in s: print(ch)
来源：https://xg.zhonguo1118.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：https://gj.zhonguo6118.cn

JS:   for (const ch of s) { console.log(ch); }
来源：https://wb.zhonguo5118.cn

TS:   for (const ch of s) { console.log(ch); }
来源：https://ta.zhonguo3118.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：https://yk.zhonguo4118.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：https://oa.zhonguo3118.cn

Ruby: s.each_char { |ch| puts ch }
来源：https://va.zhonguo8118.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：https://wn.zhonguo2118.cn

[E14] URL 编码与 Base64
来源：https://ln.zhonguo3118.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：https://iu.zhonguo5118.cn

PHP:  urlencode($s);  base64_encode($s);
来源：https://bf.zhonguo7118.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：https://uy.zhonguo2118.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：https://kj.zhonguo3118.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：https://ea.zhonguo1118.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：https://yh.zhonguo2118.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：https://pg.zhonguo8118.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：https://lt.zhonguo3118.cn

[E15] HTML 转义 / 反转义
来源：https://pr.zhonguo3118.cn

Py:   html.escape(s);  html.unescape(s)
来源：https://li.zhonguo3118.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：https://bn.zhonguo7118.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：https://ty.zhonguo3118.cn

TS:   // 同上，务必做 XSS 过滤
来源：https://lh.zhonguo1118.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：https://ax.zhonguo7118.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：https://pd.zhonguo1118.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：https://fz.zhonguo8118.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：https://hg.zhonguo7118.cn

[E16] 数字千分位
来源：https://tx.zhonguo1118.cn

Py:   f"{1234567:,}"
来源：https://cb.zhonguo5118.cn

PHP:  number_format(1234567);
来源：https://vw.zhonguo6118.cn

JS:   (1234567).toLocaleString("en-US")
来源：https://mi.zhonguo2118.cn

TS:   (1234567).toLocaleString("en-US")
来源：https://rk.zhonguo6118.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：https://dk.zhonguo3118.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：https://rw.zhonguo7118.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：https://tt.zhonguo2118.cn

C#:   1234567.ToString("N0")
来源：https://hs.zhonguo5118.cn

[E17] 首字母大写
来源：https://ny.zhonguo2118.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：https://vh.zhonguo3118.cn

PHP:  ucfirst($s);  ucwords($s);
来源：https://nu.zhonguo7118.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://ua.zhonguo1118.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://hh.zhonguo5118.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：https://pv.zhonguo1118.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：https://er.zhonguo6118.cn

Ruby: s.capitalize
来源：https://gi.zhonguo3118.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：https://ia.zhonguo8118.cn

[E18] 模板占位符替换
来源：https://dz.zhonguo2118.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：https://ot.zhonguo3118.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：https://sr.zhonguo5118.cn

JS:   tpl.replaceAll("{name}", name)
来源：https://nt.zhonguo6118.cn

TS:   tpl.replaceAll("{name}", name)
来源：https://km.zhonguo2118.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：https://hf.zhonguo5118.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：https://al.zhonguo2118.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：https://tb.zhonguo7118.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：https://zt.zhonguo5118.cn

[E19] 多行文本按行拆分
来源：https://on.zhonguo7118.cn

Py:   s.splitlines()
来源：https://re.zhonguo6118.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：https://ru.zhonguo6118.cn

JS:   s.split(/\r?\n/)
来源：https://de.zhonguo3118.cn

TS:   s.split(/\r?\n/)
来源：https://md.zhonguo5118.cn

Java: s.lines().toList()
来源：https://ah.zhonguo5118.cn

Go:   strings.Split(s, "\n")
来源：https://tf.zhonguo7118.cn

Ruby: s.lines
来源：https://au.zhonguo8118.cn

C#:   s.Split('\n')
来源：https://vl.zhonguo7118.cn

[E20] 判断字符串是否为空
来源：https://gb.zhonguo1118.cn

Py:   if not s:
来源：https://jx.zhonguo6118.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：https://eq.zhonguo8118.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：https://nx.zhonguo6118.cn

TS:   if (s === "") {}
来源：https://xv.zhonguo5118.cn

Java: if (s.isEmpty()) {}
来源：https://dz.zhonguo1118.cn

Go:   if s == "" {}
来源：https://yn.zhonguo2118.cn

Ruby: if s.empty?
来源：https://yf.zhonguo2118.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：https://ox.zhonguo2118.cn

[E21] 超长截断加省略号
来源：https://pf.zhonguo1118.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：https://hj.zhonguo5118.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：https://ah.zhonguo1118.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://yb.zhonguo5118.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://uc.zhonguo1118.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：https://mj.zhonguo1118.cn

Go:   // 按 rune 判断长度后截断
来源：https://ss.zhonguo1118.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：https://xs.zhonguo1118.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：https://wz.zhonguo3118.cn

[E22] 字节长度与字符长度
来源：https://ry.zhonguo4118.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：https://ji.zhonguo7118.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：https://df.zhonguo4118.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：https://qc.zhonguo8118.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：https://bo.zhonguo3118.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：https://jv.zhonguo4118.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：https://vk.zhonguo4118.cn

Ruby: s.bytesize;  s.length
来源：https://cd.zhonguo1118.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：https://pf.zhonguo4118.cn

================================================================================
来源：https://hu.zhonguo3118.cn

F. 文件与目录
来源：https://tr.zhonguo2118.cn

================================================================================
来源：https://hf.zhonguo2118.cn

[F01] 读取整个文件
来源：https://oc.zhonguo8118.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：https://ei.zhonguo2118.cn

PHP:  file_get_contents("a.txt");
来源：https://mb.zhonguo6118.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：https://kv.zhonguo6118.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：https://to.zhonguo3118.cn

Java: Files.readString(Path.of("a.txt"))
来源：https://xq.zhonguo5118.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：https://ww.zhonguo1118.cn

Ruby: File.read("a.txt")
来源：https://fn.zhonguo7118.cn


<!-- 参考信息 -->