代发 wailian999

[D23] reduce 累积计算
来源：https://yw.zhonguo3118.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：https://ha.zhonguo5118.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：https://xr.zhonguo5118.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://zs.zhonguo6118.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://rt.zhonguo3118.cn

Java: list.stream().reduce(0, Integer::sum)
来源：https://lh.zhonguo1118.cn

Go:   // 手写循环
来源：https://ug.zhonguo4118.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：https://wd.zhonguo1118.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：https://tx.zhonguo2118.cn

[D24] 字典 / Map 基本操作
来源：https://jt.zhonguo1118.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：https://ho.zhonguo1118.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：https://hm.zhonguo5118.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：https://nm.zhonguo1118.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：https://vo.zhonguo8118.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：https://hi.zhonguo7118.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：https://aj.zhonguo2118.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：https://gv.zhonguo5118.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：https://ae.zhonguo1118.cn

[D25] Set 集合去重与交并差
来源：https://aj.zhonguo8118.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：https://zw.zhonguo6118.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：https://kr.zhonguo2118.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：https://gq.zhonguo2118.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：https://zw.zhonguo6118.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：https://rm.zhonguo4118.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：https://xd.zhonguo6118.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：https://ub.zhonguo7118.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：https://ez.zhonguo1118.cn

[D26] 数组转字符串
来源：https://ku.zhonguo5118.cn

Py:   ", ".join(map(str, arr))
来源：https://zb.zhonguo7118.cn

PHP:  implode(", ", $arr);
来源：https://pt.zhonguo5118.cn

JS:   arr.join(", ")
来源：https://gj.zhonguo8118.cn

TS:   arr.join(", ")
来源：https://rr.zhonguo7118.cn

Java: String.join(", ", list)
来源：https://xz.zhonguo7118.cn

Go:   strings.Join(strs, ", ")
来源：https://wk.zhonguo5118.cn

Ruby: arr.join(", ")
来源：https://zm.zhonguo5118.cn

C#:   string.Join(", ", list)
来源：https://vs.zhonguo5118.cn

================================================================================
来源：https://ha.zhonguo1118.cn

E. 字符串处理
来源：https://dv.zhonguo8118.cn

================================================================================
来源：https://ru.zhonguo1118.cn

[E01] 拼接字符串
来源：https://gd.zhonguo4118.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：https://ld.zhonguo6118.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：https://uh.zhonguo6118.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：https://xi.zhonguo7118.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：https://hu.zhonguo2118.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：https://nc.zhonguo5118.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：https://id.zhonguo4118.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：https://qu.zhonguo3118.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：https://ul.zhonguo6118.cn

[E02] 重复字符串
来源：https://ok.zhonguo5118.cn

Py:   "ab" * 3
来源：https://jy.zhonguo6118.cn

PHP:  str_repeat("ab", 3);
来源：https://hb.zhonguo7118.cn

JS:   "ab".repeat(3)
来源：https://mx.zhonguo6118.cn

TS:   "ab".repeat(3)
来源：https://js.zhonguo7118.cn

Java: "ab".repeat(3)
来源：https://cj.zhonguo2118.cn

Go:   strings.Repeat("ab", 3)
来源：https://gl.zhonguo2118.cn

Ruby: "ab" * 3
来源：https://qw.zhonguo2118.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：https://wf.zhonguo6118.cn

[E03] 截取子串
来源：https://yh.zhonguo3118.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：https://aq.zhonguo7118.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：https://bh.zhonguo5118.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：https://fz.zhonguo1118.cn

TS:   s.slice(1, 4)
来源：https://wi.zhonguo3118.cn

Java: s.substring(1, 4)
来源：https://qw.zhonguo1118.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：https://fm.zhonguo7118.cn

Ruby: s[1, 3];  s[1..3]
来源：https://il.zhonguo5118.cn

C#:   s.Substring(1, 3)
来源：https://jy.zhonguo3118.cn

[E04] 查找子串位置
来源：https://jo.zhonguo7118.cn

Py:   s.find("x");  s.index("x")
来源：https://lf.zhonguo1118.cn

PHP:  strpos($s, "x");
来源：https://ui.zhonguo6118.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：https://ji.zhonguo2118.cn

TS:   s.indexOf("x")
来源：https://tq.zhonguo4118.cn

Java: s.indexOf("x")
来源：https://yw.zhonguo8118.cn

Go:   strings.Index(s, "x")
来源：https://en.zhonguo4118.cn

Ruby: s.index("x")
来源：https://tr.zhonguo4118.cn

C#:   s.IndexOf("x")
来源：https://lo.zhonguo5118.cn

[E05] 判断包含 / 前缀 / 后缀
来源：https://kt.zhonguo4118.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：https://mu.zhonguo3118.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：https://xo.zhonguo7118.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：https://gl.zhonguo3118.cn

TS:   s.includes("x");  s.startsWith("a")
来源：https://oi.zhonguo2118.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：https://ja.zhonguo6118.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：https://cv.zhonguo1118.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：https://cs.zhonguo7118.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：https://zs.zhonguo8118.cn

[E06] 替换子串
来源：https://kt.zhonguo7118.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：https://hd.zhonguo1118.cn

PHP:  str_replace("a", "b", $s);
来源：https://ki.zhonguo3118.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://el.zhonguo4118.cn

TS:   s.replaceAll("a", "b")
来源：https://gk.zhonguo4118.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://wq.zhonguo2118.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：https://rm.zhonguo5118.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：https://gm.zhonguo8118.cn

C#:   s.Replace("a", "b")
来源：https://gd.zhonguo6118.cn

[E07] 按分隔符拆分
来源：https://jw.zhonguo5118.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：https://id.zhonguo6118.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：https://gc.zhonguo8118.cn

JS:   s.split(",");  s.split(/\s+/)
来源：https://rp.zhonguo1118.cn

TS:   s.split(",")
来源：https://uj.zhonguo8118.cn

Java: s.split(",");  s.split("\\s+")
来源：https://gq.zhonguo2118.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：https://fm.zhonguo7118.cn

Ruby: s.split(",");  s.split
来源：https://br.zhonguo3118.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：https://dx.zhonguo4118.cn

[E08] 数组按分隔符合并
来源：https://yo.zhonguo2118.cn

Py:   ",".join(items)
来源：https://hc.zhonguo7118.cn

PHP:  implode(",", $items);
来源：https://lm.zhonguo5118.cn

JS:   items.join(",")
来源：https://ht.zhonguo8118.cn

TS:   items.join(",")
来源：https://kt.zhonguo2118.cn

Java: String.join(",", items)
来源：https://ry.zhonguo8118.cn

Go:   strings.Join(items, ",")
来源：https://qk.zhonguo6118.cn

Ruby: items.join(",")
来源：https://bx.zhonguo7118.cn

C#:   string.Join(",", items)
来源：https://zx.zhonguo3118.cn

[E09] 去除所有空白字符
来源：https://pi.zhonguo6118.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：https://wn.zhonguo7118.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：https://xj.zhonguo5118.cn

JS:   s.replace(/\s+/g, "")
来源：https://im.zhonguo8118.cn

TS:   s.replace(/\s+/g, "")
来源：https://ao.zhonguo8118.cn

Java: s.replaceAll("\\s+", "")
来源：https://za.zhonguo4118.cn

Go:   strings.Join(strings.Fields(s), "")
来源：https://ro.zhonguo1118.cn

Ruby: s.gsub(/\s+/, "")
来源：https://de.zhonguo2118.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：https://jd.zhonguo8118.cn

[E10] 左侧补零 / 定长填充
来源：https://hh.zhonguo3118.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：https://yd.zhonguo7118.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：https://ai.zhonguo2118.cn

JS:   "7".padStart(3, "0")
来源：https://jn.zhonguo5118.cn

TS:   "7".padStart(3, "0")
来源：https://ri.zhonguo7118.cn

Java: String.format("%03d", 7)
来源：https://ac.zhonguo3118.cn

Go:   fmt.Sprintf("%03d", 7)
来源：https://jz.zhonguo3118.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：https://xf.zhonguo4118.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：https://ft.zhonguo7118.cn

[E11] 反转字符串
来源：https://ku.zhonguo8118.cn

Py:   s[::-1]
来源：https://rj.zhonguo5118.cn

PHP:  strrev($s);
来源：https://hc.zhonguo8118.cn

JS:   [...s].reverse().join("")
来源：https://ys.zhonguo5118.cn

TS:   [...s].reverse().join("")
来源：https://jg.zhonguo7118.cn

Java: new StringBuilder(s).reverse().toString()
来源：https://br.zhonguo3118.cn

Go:   // 转 []rune 后倒序再转回 string
来源：https://qm.zhonguo3118.cn

Ruby: s.reverse
来源：https://rp.zhonguo6118.cn

C#:   new string(s.Reverse().ToArray())
来源：https://gm.zhonguo1118.cn

[E12] 统计某字符出现次数
来源：https://hc.zhonguo5118.cn

Py:   s.count("a")
来源：https://mr.zhonguo3118.cn

PHP:  substr_count($s, "a");
来源：https://gu.zhonguo7118.cn

JS:   s.split("a").length - 1
来源：https://yj.zhonguo6118.cn

TS:   s.split("a").length - 1
来源：https://zl.zhonguo2118.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：https://ql.zhonguo3118.cn

Go:   strings.Count(s, "a")
来源：https://as.zhonguo6118.cn

Ruby: s.count("a")
来源：https://rn.zhonguo3118.cn

C#:   s.Count(c => c == 'a')
来源：https://tu.zhonguo5118.cn

[E13] 逐字符遍历
来源：https://ae.zhonguo4118.cn

Py:   for ch in s: print(ch)
来源：https://st.zhonguo5118.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：https://db.zhonguo8118.cn

JS:   for (const ch of s) { console.log(ch); }
来源：https://vc.zhonguo7118.cn

TS:   for (const ch of s) { console.log(ch); }
来源：https://ih.zhonguo2118.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：https://dm.zhonguo4118.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：https://br.zhonguo3118.cn

Ruby: s.each_char { |ch| puts ch }
来源：https://aj.zhonguo6118.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：https://ni.zhonguo1118.cn

[E14] URL 编码与 Base64
来源：https://yf.zhonguo4118.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：https://kd.zhonguo8118.cn

PHP:  urlencode($s);  base64_encode($s);
来源：https://lr.zhonguo1118.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：https://yv.zhonguo2118.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：https://ep.zhonguo7118.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：https://iq.zhonguo3118.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：https://oj.zhonguo7118.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：https://hj.zhonguo7118.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：https://ag.zhonguo3118.cn

[E15] HTML 转义 / 反转义
来源：https://jx.zhonguo5118.cn

Py:   html.escape(s);  html.unescape(s)
来源：https://ve.zhonguo7118.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：https://te.zhonguo4118.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：https://yy.zhonguo6118.cn

TS:   // 同上，务必做 XSS 过滤
来源：https://tq.zhonguo5118.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：https://nx.zhonguo6118.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：https://hx.zhonguo8118.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：https://hy.zhonguo4118.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：https://ns.zhonguo6118.cn

[E16] 数字千分位
来源：https://jn.zhonguo6118.cn

Py:   f"{1234567:,}"
来源：https://vv.zhonguo4118.cn

PHP:  number_format(1234567);
来源：https://wc.zhonguo4118.cn

JS:   (1234567).toLocaleString("en-US")
来源：https://nn.zhonguo1118.cn

TS:   (1234567).toLocaleString("en-US")
来源：https://sn.zhonguo6118.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：https://jt.zhonguo8118.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：https://br.zhonguo6118.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：https://ch.zhonguo1118.cn

C#:   1234567.ToString("N0")
来源：https://il.zhonguo3118.cn

[E17] 首字母大写
来源：https://zu.zhonguo5118.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：https://cz.zhonguo3118.cn

PHP:  ucfirst($s);  ucwords($s);
来源：https://cn.zhonguo1118.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://pa.zhonguo3118.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://dt.zhonguo6118.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：https://mr.zhonguo8118.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：https://yq.zhonguo7118.cn

Ruby: s.capitalize
来源：https://sv.zhonguo1118.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：https://fz.zhonguo1118.cn

[E18] 模板占位符替换
来源：https://xp.zhonguo1118.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：https://ix.zhonguo2118.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：https://vw.zhonguo4118.cn

JS:   tpl.replaceAll("{name}", name)
来源：https://wv.zhonguo4118.cn

TS:   tpl.replaceAll("{name}", name)
来源：https://vk.zhonguo4118.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：https://br.zhonguo1118.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：https://qe.zhonguo8118.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：https://tu.zhonguo4118.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：https://sx.zhonguo7118.cn

[E19] 多行文本按行拆分
来源：https://qt.zhonguo3118.cn

Py:   s.splitlines()
来源：https://zs.zhonguo5118.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：https://ui.zhonguo3118.cn

JS:   s.split(/\r?\n/)
来源：https://ss.zhonguo2118.cn

TS:   s.split(/\r?\n/)
来源：https://fv.zhonguo2118.cn

Java: s.lines().toList()
来源：https://bp.zhonguo3118.cn

Go:   strings.Split(s, "\n")
来源：https://nv.zhonguo6118.cn

Ruby: s.lines
来源：https://ug.zhonguo7118.cn

C#:   s.Split('\n')
来源：https://ft.zhonguo7118.cn

[E20] 判断字符串是否为空
来源：https://mw.zhonguo2118.cn

Py:   if not s:
来源：https://nt.zhonguo8118.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：https://wj.zhonguo6118.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：https://aw.zhonguo7118.cn

TS:   if (s === "") {}
来源：https://ah.zhonguo1118.cn

Java: if (s.isEmpty()) {}
来源：https://cn.zhonguo2118.cn

Go:   if s == "" {}
来源：https://vx.zhonguo8118.cn

Ruby: if s.empty?
来源：https://nx.zhonguo2118.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：https://lh.zhonguo2118.cn

[E21] 超长截断加省略号
来源：https://po.zhonguo2118.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：https://vl.zhonguo8118.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：https://ml.zhonguo7118.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://wd.zhonguo8118.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://cu.zhonguo8118.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：https://at.zhonguo8118.cn

Go:   // 按 rune 判断长度后截断
来源：https://yo.zhonguo1118.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：https://ih.zhonguo6118.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：https://fs.zhonguo3118.cn

[E22] 字节长度与字符长度
来源：https://jk.zhonguo6118.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：https://ag.zhonguo1118.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：https://qe.zhonguo4118.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：https://sx.zhonguo1118.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：https://dr.zhonguo2118.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：https://fi.zhonguo7118.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：https://hw.zhonguo3118.cn

Ruby: s.bytesize;  s.length
来源：https://wu.zhonguo8118.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：https://km.zhonguo5118.cn

================================================================================
来源：https://sm.zhonguo6118.cn

F. 文件与目录
来源：https://vf.zhonguo5118.cn

================================================================================
来源：https://rt.zhonguo6118.cn

[F01] 读取整个文件
来源：https://qf.zhonguo5118.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：https://os.zhonguo3118.cn

PHP:  file_get_contents("a.txt");
来源：https://am.zhonguo5118.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：https://ce.zhonguo7118.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：https://nq.zhonguo7118.cn

Java: Files.readString(Path.of("a.txt"))
来源：https://pn.zhonguo8118.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：https://tm.zhonguo8118.cn

Ruby: File.read("a.txt")
来源：https://ph.zhonguo5118.cn

C#:   File.ReadAllText("a.txt");
来源：https://se.zhonguo3118.cn

[F02] 逐行读取文件
来源：https://kg.zhonguo4118.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：https://ui.zhonguo8118.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：https://zn.zhonguo6118.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://ho.zhonguo8118.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://gq.zhonguo4118.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：https://md.zhonguo6118.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：https://zk.zhonguo8118.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：https://wa.zhonguo4118.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：https://pd.zhonguo1118.cn

[F03] 写入文件（覆盖）
来源：https://ws.zhonguo2118.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：https://it.zhonguo2118.cn

PHP:  file_put_contents("a.txt", "hi");
来源：https://mw.zhonguo3118.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://af.zhonguo3118.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://bg.zhonguo5118.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：https://bc.zhonguo7118.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：https://cy.zhonguo1118.cn

Ruby: File.write("a.txt", "hi")
来源：https://ml.zhonguo3118.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：https://xv.zhonguo5118.cn

[F04] 追加写入文件
来源：https://rs.zhonguo7118.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：https://ff.zhonguo3118.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：https://qr.zhonguo2118.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：https://rw.zhonguo3118.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：https://ys.zhonguo2118.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：https://nj.zhonguo2118.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：https://ej.zhonguo5118.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：https://mh.zhonguo3118.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：https://pc.zhonguo7118.cn

[F05] 判断文件或目录是否存在
来源：https://sx.zhonguo4118.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：https://bi.zhonguo4118.cn

PHP:  file_exists("a.txt");
来源：https://ut.zhonguo8118.cn

JS:   fs.existsSync("a.txt")
来源：https://gi.zhonguo8118.cn

TS:   fs.existsSync("a.txt")
来源：https://mu.zhonguo2118.cn

Java: Files.exists(Path.of("a.txt"))
来源：https://wl.zhonguo6118.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：https://jc.zhonguo2118.cn

Ruby: File.exist?("a.txt")
来源：https://tp.zhonguo4118.cn

C#:   File.Exists("a.txt")
来源：https://cb.zhonguo7118.cn

[F06] 删除文件
来源：https://xj.zhonguo6118.cn

Py:   os.remove("a.txt")
来源：https://wm.zhonguo7118.cn

PHP:  unlink("a.txt");
来源：https://cf.zhonguo5118.cn

JS:   fs.unlinkSync("a.txt")
来源：https://sp.zhonguo6118.cn

TS:   fs.unlinkSync("a.txt")
来源：https://wd.zhonguo2118.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：https://hz.zhonguo1118.cn

Go:   os.Remove("a.txt")
来源：https://zy.zhonguo8118.cn

Ruby: File.delete("a.txt")
来源：https://bm.zhonguo7118.cn

C#:   File.Delete("a.txt");
来源：https://mb.zhonguo2118.cn

[F07] 创建目录（含多级）
来源：https://wx.zhonguo2118.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：https://gn.zhonguo3118.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：https://zz.zhonguo5118.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://ye.zhonguo8118.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://vl.zhonguo8118.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：https://bk.zhonguo5118.cn


<!-- 参考信息 -->