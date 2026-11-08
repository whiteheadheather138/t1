代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：https://hj.zhonguo7118.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：https://jh.zhonguo7118.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：https://jj.zhonguo7118.cn

Go:   // 手写循环累加
来源：https://yi.zhonguo8118.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：https://vz.zhonguo8118.cn

C#:   list.Sum();  list.Average()
来源：https://id.zhonguo7118.cn

[D17] 最大值与最小值
来源：https://ni.zhonguo2118.cn

Py:   max(arr);  min(arr)
来源：https://um.zhonguo5118.cn

PHP:  max($arr);  min($arr);
来源：https://tw.zhonguo3118.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：https://vg.zhonguo6118.cn

TS:   Math.max(...arr);
来源：https://oo.zhonguo2118.cn

Java: Collections.max(list);  Collections.min(list);
来源：https://ek.zhonguo7118.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：https://ug.zhonguo4118.cn

Ruby: arr.max;  arr.min
来源：https://kr.zhonguo2118.cn

C#:   list.Max();  list.Min()
来源：https://zt.zhonguo6118.cn

[D18] 扁平化嵌套数组
来源：https://wn.zhonguo2118.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：https://ls.zhonguo1118.cn

PHP:  array_merge(...$nested);
来源：https://zu.zhonguo6118.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：https://my.zhonguo1118.cn

TS:   nested.flat();
来源：https://jn.zhonguo5118.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：https://sx.zhonguo3118.cn

Go:   // 手写双层循环
来源：https://gu.zhonguo6118.cn

Ruby: nested.flatten
来源：https://ad.zhonguo6118.cn

C#:   nested.SelectMany(x => x).ToList()
来源：https://sf.zhonguo3118.cn

[D19] 按字段分组
来源：https://mx.zhonguo1118.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：https://vr.zhonguo8118.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：https://ui.zhonguo6118.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：https://xe.zhonguo4118.cn

TS:   Object.groupBy(arr, x => x.type)
来源：https://bi.zhonguo4118.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：https://mh.zhonguo5118.cn

Go:   // 手写 map[string][]T
来源：https://ns.zhonguo5118.cn

Ruby: arr.group_by { |x| x[:type] }
来源：https://ox.zhonguo7118.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：https://ac.zhonguo8118.cn

[D20] 统计每个元素出现次数
来源：https://om.zhonguo2118.cn

Py:   Counter(arr)
来源：https://me.zhonguo6118.cn

PHP:  array_count_values($arr);
来源：https://zx.zhonguo4118.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://lh.zhonguo6118.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://lv.zhonguo5118.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：https://to.zhonguo5118.cn

Go:   // 手写 map[T]int
来源：https://lu.zhonguo8118.cn

Ruby: arr.tally
来源：https://zy.zhonguo5118.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：https://cv.zhonguo1118.cn

[D21] 判断是否包含某元素
来源：https://ah.zhonguo2118.cn

Py:   x in arr
来源：https://wq.zhonguo5118.cn

PHP:  in_array($x, $arr, true);
来源：https://rg.zhonguo1118.cn

JS:   arr.includes(x)
来源：https://em.zhonguo5118.cn

TS:   arr.includes(x)
来源：https://oy.zhonguo8118.cn

Java: list.contains(x)
来源：https://ul.zhonguo6118.cn

Go:   slices.Contains(arr, x)
来源：https://ot.zhonguo4118.cn

Ruby: arr.include?(x)
来源：https://oa.zhonguo2118.cn

C#:   list.Contains(x)
来源：https://yd.zhonguo7118.cn

[D22] 复制数组（避免共享引用）
来源：https://jf.zhonguo5118.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：https://rh.zhonguo2118.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：https://yi.zhonguo6118.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：https://ue.zhonguo4118.cn

TS:   [...arr];
来源：https://dl.zhonguo1118.cn

Java: new ArrayList<>(list);
来源：https://qw.zhonguo2118.cn

Go:   copied := append([]int(nil), arr...)
来源：https://vf.zhonguo3118.cn

Ruby: arr.dup;  arr.clone
来源：https://to.zhonguo8118.cn

C#:   new List<int>(list);
来源：https://gd.zhonguo7118.cn

[D23] reduce 累积计算
来源：https://hd.zhonguo5118.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：https://xo.zhonguo8118.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：https://yb.zhonguo5118.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://yf.zhonguo1118.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://yi.zhonguo6118.cn

Java: list.stream().reduce(0, Integer::sum)
来源：https://mn.zhonguo7118.cn

Go:   // 手写循环
来源：https://yv.zhonguo4118.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：https://nl.zhonguo8118.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：https://qx.zhonguo3118.cn

[D24] 字典 / Map 基本操作
来源：https://os.zhonguo1118.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：https://kv.zhonguo4118.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：https://en.zhonguo7118.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：https://dz.zhonguo8118.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：https://pp.zhonguo3118.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：https://bq.zhonguo2118.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：https://fu.zhonguo4118.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：https://fb.zhonguo7118.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：https://oh.zhonguo2118.cn

[D25] Set 集合去重与交并差
来源：https://di.zhonguo8118.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：https://pr.zhonguo8118.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：https://mv.zhonguo4118.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：https://kt.zhonguo8118.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：https://is.zhonguo4118.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：https://vt.zhonguo7118.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：https://mr.zhonguo8118.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：https://nh.zhonguo7118.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：https://qg.zhonguo1118.cn

[D26] 数组转字符串
来源：https://pi.zhonguo1118.cn

Py:   ", ".join(map(str, arr))
来源：https://jg.zhonguo1118.cn

PHP:  implode(", ", $arr);
来源：https://du.zhonguo7118.cn

JS:   arr.join(", ")
来源：https://dy.zhonguo1118.cn

TS:   arr.join(", ")
来源：https://bs.zhonguo2118.cn

Java: String.join(", ", list)
来源：https://lq.zhonguo7118.cn

Go:   strings.Join(strs, ", ")
来源：https://cz.zhonguo3118.cn

Ruby: arr.join(", ")
来源：https://hk.zhonguo3118.cn

C#:   string.Join(", ", list)
来源：https://ec.zhonguo8118.cn

================================================================================
来源：https://zc.zhonguo2118.cn

E. 字符串处理
来源：https://je.zhonguo5118.cn

================================================================================
来源：https://yg.zhonguo1118.cn

[E01] 拼接字符串
来源：https://kx.zhonguo6118.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：https://ud.zhonguo5118.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：https://hk.zhonguo3118.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：https://lu.zhonguo2118.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：https://gx.zhonguo1118.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：https://qd.zhonguo2118.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：https://ki.zhonguo6118.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：https://wb.zhonguo6118.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：https://xl.zhonguo6118.cn

[E02] 重复字符串
来源：https://oy.zhonguo4118.cn

Py:   "ab" * 3
来源：https://ly.zhonguo2118.cn

PHP:  str_repeat("ab", 3);
来源：https://cr.zhonguo2118.cn

JS:   "ab".repeat(3)
来源：https://gc.zhonguo8118.cn

TS:   "ab".repeat(3)
来源：https://xy.zhonguo5118.cn

Java: "ab".repeat(3)
来源：https://sx.zhonguo1118.cn

Go:   strings.Repeat("ab", 3)
来源：https://wr.zhonguo6118.cn

Ruby: "ab" * 3
来源：https://nb.zhonguo8118.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：https://el.zhonguo4118.cn

[E03] 截取子串
来源：https://ld.zhonguo6118.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：https://eg.zhonguo2118.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：https://us.zhonguo6118.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：https://vv.zhonguo8118.cn

TS:   s.slice(1, 4)
来源：https://fu.zhonguo2118.cn

Java: s.substring(1, 4)
来源：https://cf.zhonguo1118.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：https://vt.zhonguo3118.cn

Ruby: s[1, 3];  s[1..3]
来源：https://ph.zhonguo6118.cn

C#:   s.Substring(1, 3)
来源：https://mx.zhonguo6118.cn

[E04] 查找子串位置
来源：https://il.zhonguo8118.cn

Py:   s.find("x");  s.index("x")
来源：https://uu.zhonguo5118.cn

PHP:  strpos($s, "x");
来源：https://af.zhonguo7118.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：https://ed.zhonguo2118.cn

TS:   s.indexOf("x")
来源：https://mj.zhonguo4118.cn

Java: s.indexOf("x")
来源：https://th.zhonguo1118.cn

Go:   strings.Index(s, "x")
来源：https://nf.zhonguo7118.cn

Ruby: s.index("x")
来源：https://oq.zhonguo1118.cn

C#:   s.IndexOf("x")
来源：https://mw.zhonguo3118.cn

[E05] 判断包含 / 前缀 / 后缀
来源：https://th.zhonguo6118.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：https://oc.zhonguo8118.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：https://ji.zhonguo3118.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：https://ii.zhonguo2118.cn

TS:   s.includes("x");  s.startsWith("a")
来源：https://fo.zhonguo7118.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：https://ds.zhonguo2118.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：https://jl.zhonguo3118.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：https://xp.zhonguo5118.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：https://jp.zhonguo4118.cn

[E06] 替换子串
来源：https://oi.zhonguo8118.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：https://mp.zhonguo5118.cn

PHP:  str_replace("a", "b", $s);
来源：https://av.zhonguo4118.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://hw.zhonguo8118.cn

TS:   s.replaceAll("a", "b")
来源：https://qo.zhonguo8118.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://sb.zhonguo2118.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：https://qw.zhonguo7118.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：https://bi.zhonguo7118.cn

C#:   s.Replace("a", "b")
来源：https://ib.zhonguo7118.cn

[E07] 按分隔符拆分
来源：https://lf.zhonguo3118.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：https://jy.zhonguo7118.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：https://xf.zhonguo7118.cn

JS:   s.split(",");  s.split(/\s+/)
来源：https://gl.zhonguo2118.cn

TS:   s.split(",")
来源：https://sl.zhonguo5118.cn

Java: s.split(",");  s.split("\\s+")
来源：https://aa.zhonguo6118.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：https://tj.zhonguo3118.cn

Ruby: s.split(",");  s.split
来源：https://lz.zhonguo4118.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：https://el.zhonguo6118.cn

[E08] 数组按分隔符合并
来源：https://sn.zhonguo8118.cn

Py:   ",".join(items)
来源：https://bz.zhonguo1118.cn

PHP:  implode(",", $items);
来源：https://yy.zhonguo2118.cn

JS:   items.join(",")
来源：https://ep.zhonguo4118.cn

TS:   items.join(",")
来源：https://jm.zhonguo8118.cn

Java: String.join(",", items)
来源：https://ac.zhonguo3118.cn

Go:   strings.Join(items, ",")
来源：https://kb.zhonguo6118.cn

Ruby: items.join(",")
来源：https://kp.zhonguo1118.cn

C#:   string.Join(",", items)
来源：https://ie.zhonguo2118.cn

[E09] 去除所有空白字符
来源：https://ht.zhonguo2118.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：https://en.zhonguo4118.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：https://ap.zhonguo2118.cn

JS:   s.replace(/\s+/g, "")
来源：https://xh.zhonguo6118.cn

TS:   s.replace(/\s+/g, "")
来源：https://gx.zhonguo2118.cn

Java: s.replaceAll("\\s+", "")
来源：https://yb.zhonguo6118.cn

Go:   strings.Join(strings.Fields(s), "")
来源：https://do.zhonguo3118.cn

Ruby: s.gsub(/\s+/, "")
来源：https://pp.zhonguo3118.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：https://sg.zhonguo4118.cn

[E10] 左侧补零 / 定长填充
来源：https://wc.zhonguo1118.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：https://ss.zhonguo2118.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：https://fx.zhonguo4118.cn

JS:   "7".padStart(3, "0")
来源：https://we.zhonguo2118.cn

TS:   "7".padStart(3, "0")
来源：https://gl.zhonguo1118.cn

Java: String.format("%03d", 7)
来源：https://sv.zhonguo5118.cn

Go:   fmt.Sprintf("%03d", 7)
来源：https://bf.zhonguo7118.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：https://mm.zhonguo8118.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：https://ck.zhonguo8118.cn

[E11] 反转字符串
来源：https://dd.zhonguo4118.cn

Py:   s[::-1]
来源：https://kr.zhonguo1118.cn

PHP:  strrev($s);
来源：https://at.zhonguo2118.cn

JS:   [...s].reverse().join("")
来源：https://ug.zhonguo5118.cn

TS:   [...s].reverse().join("")
来源：https://lk.zhonguo1118.cn

Java: new StringBuilder(s).reverse().toString()
来源：https://fp.zhonguo3118.cn

Go:   // 转 []rune 后倒序再转回 string
来源：https://zw.zhonguo5118.cn

Ruby: s.reverse
来源：https://jj.zhonguo3118.cn

C#:   new string(s.Reverse().ToArray())
来源：https://ai.zhonguo1118.cn

[E12] 统计某字符出现次数
来源：https://ur.zhonguo4118.cn

Py:   s.count("a")
来源：https://rv.zhonguo1118.cn

PHP:  substr_count($s, "a");
来源：https://rb.zhonguo6118.cn

JS:   s.split("a").length - 1
来源：https://gd.zhonguo3118.cn

TS:   s.split("a").length - 1
来源：https://mx.zhonguo4118.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：https://zn.zhonguo6118.cn

Go:   strings.Count(s, "a")
来源：https://wb.zhonguo2118.cn

Ruby: s.count("a")
来源：https://vs.zhonguo4118.cn

C#:   s.Count(c => c == 'a')
来源：https://ri.zhonguo8118.cn

[E13] 逐字符遍历
来源：https://jz.zhonguo8118.cn

Py:   for ch in s: print(ch)
来源：https://wj.zhonguo5118.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：https://hq.zhonguo2118.cn

JS:   for (const ch of s) { console.log(ch); }
来源：https://hc.zhonguo5118.cn

TS:   for (const ch of s) { console.log(ch); }
来源：https://qr.zhonguo6118.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：https://eb.zhonguo7118.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：https://qr.zhonguo8118.cn

Ruby: s.each_char { |ch| puts ch }
来源：https://cl.zhonguo1118.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：https://xz.zhonguo5118.cn

[E14] URL 编码与 Base64
来源：https://hn.zhonguo6118.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：https://gb.zhonguo5118.cn

PHP:  urlencode($s);  base64_encode($s);
来源：https://xs.zhonguo4118.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：https://eq.zhonguo7118.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：https://on.zhonguo8118.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：https://yh.zhonguo1118.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：https://yq.zhonguo5118.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：https://hh.zhonguo7118.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：https://yf.zhonguo5118.cn

[E15] HTML 转义 / 反转义
来源：https://zz.zhonguo8118.cn

Py:   html.escape(s);  html.unescape(s)
来源：https://fo.zhonguo3118.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：https://fv.zhonguo1118.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：https://ym.zhonguo8118.cn

TS:   // 同上，务必做 XSS 过滤
来源：https://qy.zhonguo5118.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：https://xq.zhonguo7118.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：https://eb.zhonguo6118.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：https://mq.zhonguo8118.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：https://qb.zhonguo6118.cn

[E16] 数字千分位
来源：https://iq.zhonguo2118.cn

Py:   f"{1234567:,}"
来源：https://dg.zhonguo2118.cn

PHP:  number_format(1234567);
来源：https://co.zhonguo8118.cn

JS:   (1234567).toLocaleString("en-US")
来源：https://id.zhonguo8118.cn

TS:   (1234567).toLocaleString("en-US")
来源：https://sk.zhonguo4118.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：https://vv.zhonguo2118.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：https://fk.zhonguo3118.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：https://hm.zhonguo3118.cn

C#:   1234567.ToString("N0")
来源：https://hi.zhonguo4118.cn

[E17] 首字母大写
来源：https://ra.zhonguo3118.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：https://wz.zhonguo3118.cn

PHP:  ucfirst($s);  ucwords($s);
来源：https://gf.zhonguo8118.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://ig.zhonguo4118.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://vt.zhonguo3118.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：https://fz.zhonguo3118.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：https://iz.zhonguo3118.cn

Ruby: s.capitalize
来源：https://hq.zhonguo5118.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：https://py.zhonguo7118.cn

[E18] 模板占位符替换
来源：https://vy.zhonguo1118.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：https://ux.zhonguo6118.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：https://fo.zhonguo6118.cn

JS:   tpl.replaceAll("{name}", name)
来源：https://hq.zhonguo4118.cn

TS:   tpl.replaceAll("{name}", name)
来源：https://sy.zhonguo6118.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：https://bt.zhonguo6118.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：https://hp.zhonguo2118.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：https://zc.zhonguo6118.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：https://ty.zhonguo8118.cn

[E19] 多行文本按行拆分
来源：https://dc.zhonguo2118.cn

Py:   s.splitlines()
来源：https://st.zhonguo5118.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：https://ei.zhonguo8118.cn

JS:   s.split(/\r?\n/)
来源：https://nm.zhonguo1118.cn

TS:   s.split(/\r?\n/)
来源：https://vq.zhonguo3118.cn

Java: s.lines().toList()
来源：https://id.zhonguo6118.cn

Go:   strings.Split(s, "\n")
来源：https://ov.zhonguo2118.cn

Ruby: s.lines
来源：https://si.zhonguo6118.cn

C#:   s.Split('\n')
来源：https://qz.zhonguo1118.cn

[E20] 判断字符串是否为空
来源：https://td.zhonguo8118.cn

Py:   if not s:
来源：https://eu.zhonguo5118.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：https://hg.zhonguo3118.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：https://vj.zhonguo7118.cn

TS:   if (s === "") {}
来源：https://zp.zhonguo7118.cn

Java: if (s.isEmpty()) {}
来源：https://gq.zhonguo8118.cn

Go:   if s == "" {}
来源：https://sh.zhonguo2118.cn

Ruby: if s.empty?
来源：https://ho.zhonguo3118.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：https://ue.zhonguo3118.cn

[E21] 超长截断加省略号
来源：https://yz.zhonguo2118.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：https://mc.zhonguo8118.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：https://dp.zhonguo3118.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://an.zhonguo8118.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://oh.zhonguo7118.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：https://mp.zhonguo4118.cn

Go:   // 按 rune 判断长度后截断
来源：https://pa.zhonguo3118.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：https://oy.zhonguo2118.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：https://qp.zhonguo8118.cn

[E22] 字节长度与字符长度
来源：https://kb.zhonguo3118.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：https://eo.zhonguo6118.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：https://gg.zhonguo8118.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：https://uu.zhonguo4118.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：https://dv.zhonguo8118.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：https://wh.zhonguo4118.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：https://un.zhonguo4118.cn

Ruby: s.bytesize;  s.length
来源：https://pj.zhonguo4118.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：https://ev.zhonguo4118.cn

================================================================================
来源：https://dv.zhonguo5118.cn

F. 文件与目录
来源：https://dd.zhonguo6118.cn

================================================================================
来源：https://sr.zhonguo7118.cn


<!-- 参考信息 -->