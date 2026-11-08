代发 wailian999

PHP:  in_array($x, $arr, true);
来源：https://hv.zhonguo7118.cn

JS:   arr.includes(x)
来源：https://bo.zhonguo8118.cn

TS:   arr.includes(x)
来源：https://xw.zhonguo6118.cn

Java: list.contains(x)
来源：https://fv.zhonguo7118.cn

Go:   slices.Contains(arr, x)
来源：https://jl.zhonguo2118.cn

Ruby: arr.include?(x)
来源：https://eo.zhonguo4118.cn

C#:   list.Contains(x)
来源：https://qw.zhonguo7118.cn

[D22] 复制数组（避免共享引用）
来源：https://gm.zhonguo1118.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：https://om.zhonguo6118.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：https://zx.zhonguo7118.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：https://zj.zhonguo2118.cn

TS:   [...arr];
来源：https://jb.zhonguo5118.cn

Java: new ArrayList<>(list);
来源：https://op.zhonguo6118.cn

Go:   copied := append([]int(nil), arr...)
来源：https://je.zhonguo8118.cn

Ruby: arr.dup;  arr.clone
来源：https://ax.zhonguo2118.cn

C#:   new List<int>(list);
来源：https://xc.zhonguo2118.cn

[D23] reduce 累积计算
来源：https://kd.zhonguo2118.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：https://tt.zhonguo5118.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：https://we.zhonguo3118.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://yg.zhonguo6118.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://wy.zhonguo7118.cn

Java: list.stream().reduce(0, Integer::sum)
来源：https://ej.zhonguo1118.cn

Go:   // 手写循环
来源：https://gh.zhonguo1118.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：https://um.zhonguo6118.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：https://on.zhonguo3118.cn

[D24] 字典 / Map 基本操作
来源：https://sm.zhonguo5118.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：https://mq.zhonguo5118.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：https://du.zhonguo8118.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：https://xa.zhonguo2118.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：https://yp.zhonguo6118.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：https://ok.zhonguo3118.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：https://un.zhonguo8118.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：https://qe.zhonguo1118.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：https://zm.zhonguo4118.cn

[D25] Set 集合去重与交并差
来源：https://kx.zhonguo3118.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：https://ig.zhonguo6118.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：https://gh.zhonguo2118.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：https://fm.zhonguo5118.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：https://yn.zhonguo2118.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：https://zu.zhonguo1118.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：https://ar.zhonguo2118.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：https://jl.zhonguo4118.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：https://zf.zhonguo7118.cn

[D26] 数组转字符串
来源：https://bv.zhonguo4118.cn

Py:   ", ".join(map(str, arr))
来源：https://zk.zhonguo2118.cn

PHP:  implode(", ", $arr);
来源：https://wj.zhonguo2118.cn

JS:   arr.join(", ")
来源：https://rh.zhonguo7118.cn

TS:   arr.join(", ")
来源：https://kp.zhonguo6118.cn

Java: String.join(", ", list)
来源：https://ql.zhonguo1118.cn

Go:   strings.Join(strs, ", ")
来源：https://zs.zhonguo2118.cn

Ruby: arr.join(", ")
来源：https://zu.zhonguo6118.cn

C#:   string.Join(", ", list)
来源：https://mn.zhonguo7118.cn

================================================================================
来源：https://jb.zhonguo3118.cn

E. 字符串处理
来源：https://bt.zhonguo8118.cn

================================================================================
来源：https://vg.zhonguo5118.cn

[E01] 拼接字符串
来源：https://dh.zhonguo6118.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：https://zo.zhonguo8118.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：https://ug.zhonguo6118.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：https://fq.zhonguo7118.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：https://th.zhonguo3118.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：https://vc.zhonguo5118.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：https://um.zhonguo7118.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：https://jh.zhonguo3118.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：https://rv.zhonguo5118.cn

[E02] 重复字符串
来源：https://om.zhonguo2118.cn

Py:   "ab" * 3
来源：https://gr.zhonguo5118.cn

PHP:  str_repeat("ab", 3);
来源：https://wm.zhonguo7118.cn

JS:   "ab".repeat(3)
来源：https://mp.zhonguo6118.cn

TS:   "ab".repeat(3)
来源：https://dj.zhonguo8118.cn

Java: "ab".repeat(3)
来源：https://cg.zhonguo8118.cn

Go:   strings.Repeat("ab", 3)
来源：https://wy.zhonguo2118.cn

Ruby: "ab" * 3
来源：https://jd.zhonguo3118.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：https://tf.zhonguo3118.cn

[E03] 截取子串
来源：https://rj.zhonguo6118.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：https://pt.zhonguo5118.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：https://fe.zhonguo8118.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：https://ag.zhonguo2118.cn

TS:   s.slice(1, 4)
来源：https://ao.zhonguo3118.cn

Java: s.substring(1, 4)
来源：https://bq.zhonguo5118.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：https://as.zhonguo3118.cn

Ruby: s[1, 3];  s[1..3]
来源：https://qu.zhonguo4118.cn

C#:   s.Substring(1, 3)
来源：https://hx.zhonguo5118.cn

[E04] 查找子串位置
来源：https://ew.zhonguo3118.cn

Py:   s.find("x");  s.index("x")
来源：https://kl.zhonguo8118.cn

PHP:  strpos($s, "x");
来源：https://dt.zhonguo1118.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：https://as.zhonguo7118.cn

TS:   s.indexOf("x")
来源：https://yq.zhonguo6118.cn

Java: s.indexOf("x")
来源：https://jx.zhonguo3118.cn

Go:   strings.Index(s, "x")
来源：https://vu.zhonguo3118.cn

Ruby: s.index("x")
来源：https://yv.zhonguo3118.cn

C#:   s.IndexOf("x")
来源：https://gy.zhonguo1118.cn

[E05] 判断包含 / 前缀 / 后缀
来源：https://xs.zhonguo8118.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：https://yo.zhonguo7118.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：https://nt.zhonguo3118.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：https://yo.zhonguo2118.cn

TS:   s.includes("x");  s.startsWith("a")
来源：https://xi.zhonguo8118.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：https://na.zhonguo1118.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：https://oo.zhonguo4118.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：https://fn.zhonguo3118.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：https://np.zhonguo2118.cn

[E06] 替换子串
来源：https://sw.zhonguo1118.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：https://kq.zhonguo1118.cn

PHP:  str_replace("a", "b", $s);
来源：https://gt.zhonguo3118.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://fv.zhonguo4118.cn

TS:   s.replaceAll("a", "b")
来源：https://pg.zhonguo1118.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://bi.zhonguo7118.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：https://ly.zhonguo8118.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：https://xl.zhonguo8118.cn

C#:   s.Replace("a", "b")
来源：https://yn.zhonguo5118.cn

[E07] 按分隔符拆分
来源：https://nj.zhonguo8118.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：https://jm.zhonguo1118.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：https://ru.zhonguo4118.cn

JS:   s.split(",");  s.split(/\s+/)
来源：https://wr.zhonguo3118.cn

TS:   s.split(",")
来源：https://mw.zhonguo5118.cn

Java: s.split(",");  s.split("\\s+")
来源：https://wx.zhonguo8118.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：https://rg.zhonguo3118.cn

Ruby: s.split(",");  s.split
来源：https://av.zhonguo5118.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：https://qf.zhonguo6118.cn

[E08] 数组按分隔符合并
来源：https://vn.zhonguo1118.cn

Py:   ",".join(items)
来源：https://hs.zhonguo7118.cn

PHP:  implode(",", $items);
来源：https://vn.zhonguo1118.cn

JS:   items.join(",")
来源：https://bx.zhonguo7118.cn

TS:   items.join(",")
来源：https://me.zhonguo7118.cn

Java: String.join(",", items)
来源：https://ny.zhonguo7118.cn

Go:   strings.Join(items, ",")
来源：https://yq.zhonguo6118.cn

Ruby: items.join(",")
来源：https://iu.zhonguo6118.cn

C#:   string.Join(",", items)
来源：https://jb.zhonguo3118.cn

[E09] 去除所有空白字符
来源：https://jx.zhonguo5118.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：https://zi.zhonguo3118.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：https://hq.zhonguo6118.cn

JS:   s.replace(/\s+/g, "")
来源：https://sn.zhonguo3118.cn

TS:   s.replace(/\s+/g, "")
来源：https://ol.zhonguo6118.cn

Java: s.replaceAll("\\s+", "")
来源：https://li.zhonguo4118.cn

Go:   strings.Join(strings.Fields(s), "")
来源：https://am.zhonguo4118.cn

Ruby: s.gsub(/\s+/, "")
来源：https://pj.zhonguo6118.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：https://qp.zhonguo3118.cn

[E10] 左侧补零 / 定长填充
来源：https://xe.zhonguo2118.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：https://ww.zhonguo7118.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：https://gp.zhonguo8118.cn

JS:   "7".padStart(3, "0")
来源：https://xj.zhonguo5118.cn

TS:   "7".padStart(3, "0")
来源：https://kx.zhonguo8118.cn

Java: String.format("%03d", 7)
来源：https://ox.zhonguo3118.cn

Go:   fmt.Sprintf("%03d", 7)
来源：https://dw.zhonguo1118.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：https://uf.zhonguo2118.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：https://fg.zhonguo6118.cn

[E11] 反转字符串
来源：https://zt.zhonguo4118.cn

Py:   s[::-1]
来源：https://lb.zhonguo3118.cn

PHP:  strrev($s);
来源：https://he.zhonguo6118.cn

JS:   [...s].reverse().join("")
来源：https://zr.zhonguo1118.cn

TS:   [...s].reverse().join("")
来源：https://dp.zhonguo2118.cn

Java: new StringBuilder(s).reverse().toString()
来源：https://zk.zhonguo2118.cn

Go:   // 转 []rune 后倒序再转回 string
来源：https://ci.zhonguo6118.cn

Ruby: s.reverse
来源：https://ur.zhonguo4118.cn

C#:   new string(s.Reverse().ToArray())
来源：https://cm.zhonguo6118.cn

[E12] 统计某字符出现次数
来源：https://pr.zhonguo5118.cn

Py:   s.count("a")
来源：https://po.zhonguo3118.cn

PHP:  substr_count($s, "a");
来源：https://mt.zhonguo4118.cn

JS:   s.split("a").length - 1
来源：https://qw.zhonguo5118.cn

TS:   s.split("a").length - 1
来源：https://ge.zhonguo2118.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：https://za.zhonguo7118.cn

Go:   strings.Count(s, "a")
来源：https://it.zhonguo8118.cn

Ruby: s.count("a")
来源：https://rg.zhonguo6118.cn

C#:   s.Count(c => c == 'a')
来源：https://nj.zhonguo5118.cn

[E13] 逐字符遍历
来源：https://zp.zhonguo3118.cn

Py:   for ch in s: print(ch)
来源：https://gr.zhonguo2118.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：https://ac.zhonguo3118.cn

JS:   for (const ch of s) { console.log(ch); }
来源：https://eg.zhonguo1118.cn

TS:   for (const ch of s) { console.log(ch); }
来源：https://et.zhonguo5118.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：https://kc.zhonguo2118.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：https://hm.zhonguo4118.cn

Ruby: s.each_char { |ch| puts ch }
来源：https://ak.zhonguo1118.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：https://rz.zhonguo1118.cn

[E14] URL 编码与 Base64
来源：https://co.zhonguo4118.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：https://rw.zhonguo1118.cn

PHP:  urlencode($s);  base64_encode($s);
来源：https://lx.zhonguo3118.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：https://vt.zhonguo5118.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：https://js.zhonguo7118.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：https://kv.zhonguo3118.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：https://ai.zhonguo3118.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：https://wh.zhonguo5118.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：https://ws.zhonguo6118.cn

[E15] HTML 转义 / 反转义
来源：https://qo.zhonguo8118.cn

Py:   html.escape(s);  html.unescape(s)
来源：https://ed.zhonguo6118.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：https://mx.zhonguo8118.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：https://co.zhonguo8118.cn

TS:   // 同上，务必做 XSS 过滤
来源：https://ut.zhonguo6118.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：https://ti.zhonguo8118.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：https://dd.zhonguo4118.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：https://xk.zhonguo7118.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：https://al.zhonguo8118.cn

[E16] 数字千分位
来源：https://pe.zhonguo3118.cn

Py:   f"{1234567:,}"
来源：https://an.zhonguo5118.cn

PHP:  number_format(1234567);
来源：https://vp.zhonguo5118.cn

JS:   (1234567).toLocaleString("en-US")
来源：https://rt.zhonguo1118.cn

TS:   (1234567).toLocaleString("en-US")
来源：https://tw.zhonguo2118.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：https://xv.zhonguo3118.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：https://dx.zhonguo2118.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：https://gl.zhonguo1118.cn

C#:   1234567.ToString("N0")
来源：https://dr.zhonguo6118.cn

[E17] 首字母大写
来源：https://us.zhonguo4118.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：https://ak.zhonguo6118.cn

PHP:  ucfirst($s);  ucwords($s);
来源：https://le.zhonguo5118.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://mq.zhonguo4118.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://mk.zhonguo8118.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：https://pf.zhonguo3118.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：https://pm.zhonguo2118.cn

Ruby: s.capitalize
来源：https://uo.zhonguo8118.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：https://sv.zhonguo4118.cn

[E18] 模板占位符替换
来源：https://dh.zhonguo6118.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：https://or.zhonguo3118.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：https://jy.zhonguo3118.cn

JS:   tpl.replaceAll("{name}", name)
来源：https://il.zhonguo3118.cn

TS:   tpl.replaceAll("{name}", name)
来源：https://cj.zhonguo3118.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：https://df.zhonguo8118.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：https://yb.zhonguo6118.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：https://uy.zhonguo1118.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：https://xt.zhonguo8118.cn

[E19] 多行文本按行拆分
来源：https://qi.zhonguo3118.cn

Py:   s.splitlines()
来源：https://mk.zhonguo1118.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：https://tp.zhonguo1118.cn

JS:   s.split(/\r?\n/)
来源：https://ib.zhonguo3118.cn

TS:   s.split(/\r?\n/)
来源：https://qp.zhonguo6118.cn

Java: s.lines().toList()
来源：https://ec.zhonguo8118.cn

Go:   strings.Split(s, "\n")
来源：https://jw.zhonguo7118.cn

Ruby: s.lines
来源：https://ky.zhonguo2118.cn

C#:   s.Split('\n')
来源：https://ok.zhonguo4118.cn

[E20] 判断字符串是否为空
来源：https://ft.zhonguo6118.cn

Py:   if not s:
来源：https://hm.zhonguo8118.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：https://ew.zhonguo6118.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：https://vh.zhonguo5118.cn

TS:   if (s === "") {}
来源：https://wg.zhonguo2118.cn

Java: if (s.isEmpty()) {}
来源：https://iw.zhonguo3118.cn

Go:   if s == "" {}
来源：https://wk.zhonguo8118.cn

Ruby: if s.empty?
来源：https://me.zhonguo2118.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：https://iw.zhonguo5118.cn

[E21] 超长截断加省略号
来源：https://to.zhonguo4118.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：https://dh.zhonguo3118.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：https://jb.zhonguo7118.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://ns.zhonguo1118.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://gw.zhonguo5118.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：https://fz.zhonguo4118.cn

Go:   // 按 rune 判断长度后截断
来源：https://eu.zhonguo5118.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：https://eo.zhonguo5118.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：https://sc.zhonguo6118.cn

[E22] 字节长度与字符长度
来源：https://oq.zhonguo4118.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：https://rf.zhonguo2118.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：https://zy.zhonguo7118.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：https://xb.zhonguo6118.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：https://ju.zhonguo4118.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：https://yn.zhonguo4118.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：https://mt.zhonguo7118.cn

Ruby: s.bytesize;  s.length
来源：https://ou.zhonguo1118.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：https://gc.zhonguo8118.cn

================================================================================
来源：https://mo.zhonguo8118.cn

F. 文件与目录
来源：https://dh.zhonguo4118.cn

================================================================================
来源：https://fc.zhonguo8118.cn

[F01] 读取整个文件
来源：https://qh.zhonguo5118.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：https://px.zhonguo4118.cn

PHP:  file_get_contents("a.txt");
来源：https://xv.zhonguo4118.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：https://sp.zhonguo3118.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：https://ky.zhonguo4118.cn

Java: Files.readString(Path.of("a.txt"))
来源：https://cj.zhonguo2118.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：https://jb.zhonguo1118.cn

Ruby: File.read("a.txt")
来源：https://mz.zhonguo8118.cn

C#:   File.ReadAllText("a.txt");
来源：https://ra.zhonguo8118.cn

[F02] 逐行读取文件
来源：https://qy.zhonguo3118.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：https://oz.zhonguo2118.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：https://yz.zhonguo2118.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://et.zhonguo1118.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://cd.zhonguo7118.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：https://tp.zhonguo2118.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：https://vy.zhonguo7118.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：https://ci.zhonguo3118.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：https://sf.zhonguo2118.cn

[F03] 写入文件（覆盖）
来源：https://lu.zhonguo4118.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：https://do.zhonguo3118.cn

PHP:  file_put_contents("a.txt", "hi");
来源：https://hn.zhonguo7118.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://gy.zhonguo6118.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://er.zhonguo5118.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：https://re.zhonguo5118.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：https://nj.zhonguo1118.cn

Ruby: File.write("a.txt", "hi")
来源：https://wl.zhonguo3118.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：https://uc.zhonguo5118.cn

[F04] 追加写入文件
来源：https://ob.zhonguo8118.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：https://vn.zhonguo3118.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：https://ou.zhonguo8118.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：https://qx.zhonguo6118.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：https://ds.zhonguo7118.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：https://gt.zhonguo4118.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：https://ae.zhonguo7118.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：https://lh.zhonguo1118.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：https://lj.zhonguo3118.cn

[F05] 判断文件或目录是否存在
来源：https://sq.zhonguo7118.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：https://vg.zhonguo2118.cn

PHP:  file_exists("a.txt");
来源：https://xz.zhonguo7118.cn

JS:   fs.existsSync("a.txt")
来源：https://rf.zhonguo3118.cn

TS:   fs.existsSync("a.txt")
来源：https://rc.zhonguo3118.cn

Java: Files.exists(Path.of("a.txt"))
来源：https://mk.zhonguo1118.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：https://ag.zhonguo4118.cn

Ruby: File.exist?("a.txt")
来源：https://ne.zhonguo4118.cn


<!-- 参考信息 -->