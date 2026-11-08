代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：https://kq.zhonguo7118.cn

[D20] 统计每个元素出现次数
来源：https://tv.zhonguo5118.cn

Py:   Counter(arr)
来源：https://ri.zhonguo3118.cn

PHP:  array_count_values($arr);
来源：https://ot.zhonguo2118.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://ec.zhonguo7118.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://qu.zhonguo2118.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：https://ga.zhonguo1118.cn

Go:   // 手写 map[T]int
来源：https://ub.zhonguo8118.cn

Ruby: arr.tally
来源：https://io.zhonguo2118.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：https://aw.zhonguo1118.cn

[D21] 判断是否包含某元素
来源：https://bc.zhonguo6118.cn

Py:   x in arr
来源：https://xw.zhonguo8118.cn

PHP:  in_array($x, $arr, true);
来源：https://sz.zhonguo3118.cn

JS:   arr.includes(x)
来源：https://sz.zhonguo3118.cn

TS:   arr.includes(x)
来源：https://kl.zhonguo6118.cn

Java: list.contains(x)
来源：https://rc.zhonguo1118.cn

Go:   slices.Contains(arr, x)
来源：https://gf.zhonguo3118.cn

Ruby: arr.include?(x)
来源：https://hv.zhonguo4118.cn

C#:   list.Contains(x)
来源：https://qt.zhonguo1118.cn

[D22] 复制数组（避免共享引用）
来源：https://kd.zhonguo4118.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：https://ze.zhonguo1118.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：https://ta.zhonguo7118.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：https://zc.zhonguo2118.cn

TS:   [...arr];
来源：https://lt.zhonguo3118.cn

Java: new ArrayList<>(list);
来源：https://bf.zhonguo1118.cn

Go:   copied := append([]int(nil), arr...)
来源：https://ty.zhonguo4118.cn

Ruby: arr.dup;  arr.clone
来源：https://hw.zhonguo1118.cn

C#:   new List<int>(list);
来源：https://dh.zhonguo5118.cn

[D23] reduce 累积计算
来源：https://ad.zhonguo2118.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：https://fi.zhonguo2118.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：https://yj.zhonguo8118.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://zq.zhonguo1118.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://ji.zhonguo3118.cn

Java: list.stream().reduce(0, Integer::sum)
来源：https://zs.zhonguo1118.cn

Go:   // 手写循环
来源：https://pc.zhonguo7118.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：https://bt.zhonguo8118.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：https://cm.zhonguo8118.cn

[D24] 字典 / Map 基本操作
来源：https://lp.zhonguo7118.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：https://wh.zhonguo7118.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：https://tl.zhonguo4118.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：https://bp.zhonguo4118.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：https://je.zhonguo1118.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：https://ns.zhonguo3118.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：https://ub.zhonguo5118.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：https://ho.zhonguo5118.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：https://mf.zhonguo5118.cn

[D25] Set 集合去重与交并差
来源：https://rq.zhonguo5118.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：https://pl.zhonguo6118.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：https://lj.zhonguo2118.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：https://xo.zhonguo1118.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：https://bf.zhonguo1118.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：https://pv.zhonguo3118.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：https://sz.zhonguo5118.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：https://xq.zhonguo1118.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：https://of.zhonguo8118.cn

[D26] 数组转字符串
来源：https://wh.zhonguo1118.cn

Py:   ", ".join(map(str, arr))
来源：https://gl.zhonguo7118.cn

PHP:  implode(", ", $arr);
来源：https://wr.zhonguo3118.cn

JS:   arr.join(", ")
来源：https://mi.zhonguo1118.cn

TS:   arr.join(", ")
来源：https://iy.zhonguo5118.cn

Java: String.join(", ", list)
来源：https://vh.zhonguo8118.cn

Go:   strings.Join(strs, ", ")
来源：https://dp.zhonguo3118.cn

Ruby: arr.join(", ")
来源：https://yi.zhonguo5118.cn

C#:   string.Join(", ", list)
来源：https://hq.zhonguo4118.cn

================================================================================
来源：https://vj.zhonguo5118.cn

E. 字符串处理
来源：https://sq.zhonguo1118.cn

================================================================================
来源：https://hf.zhonguo5118.cn

[E01] 拼接字符串
来源：https://me.zhonguo6118.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：https://ng.zhonguo6118.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：https://jb.zhonguo1118.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：https://pp.zhonguo1118.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：https://ha.zhonguo7118.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：https://oq.zhonguo6118.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：https://ve.zhonguo5118.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：https://pw.zhonguo5118.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：https://yh.zhonguo5118.cn

[E02] 重复字符串
来源：https://rq.zhonguo8118.cn

Py:   "ab" * 3
来源：https://jm.zhonguo5118.cn

PHP:  str_repeat("ab", 3);
来源：https://pz.zhonguo5118.cn

JS:   "ab".repeat(3)
来源：https://tt.zhonguo1118.cn

TS:   "ab".repeat(3)
来源：https://qz.zhonguo7118.cn

Java: "ab".repeat(3)
来源：https://zl.zhonguo1118.cn

Go:   strings.Repeat("ab", 3)
来源：https://vp.zhonguo5118.cn

Ruby: "ab" * 3
来源：https://be.zhonguo2118.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：https://uq.zhonguo4118.cn

[E03] 截取子串
来源：https://rm.zhonguo1118.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：https://rf.zhonguo4118.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：https://mm.zhonguo7118.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：https://ro.zhonguo4118.cn

TS:   s.slice(1, 4)
来源：https://ne.zhonguo7118.cn

Java: s.substring(1, 4)
来源：https://hu.zhonguo7118.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：https://zt.zhonguo8118.cn

Ruby: s[1, 3];  s[1..3]
来源：https://av.zhonguo4118.cn

C#:   s.Substring(1, 3)
来源：https://rz.zhonguo8118.cn

[E04] 查找子串位置
来源：https://fa.zhonguo3118.cn

Py:   s.find("x");  s.index("x")
来源：https://th.zhonguo2118.cn

PHP:  strpos($s, "x");
来源：https://fl.zhonguo8118.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：https://uc.zhonguo6118.cn

TS:   s.indexOf("x")
来源：https://ho.zhonguo2118.cn

Java: s.indexOf("x")
来源：https://oj.zhonguo6118.cn

Go:   strings.Index(s, "x")
来源：https://yg.zhonguo4118.cn

Ruby: s.index("x")
来源：https://fc.zhonguo7118.cn

C#:   s.IndexOf("x")
来源：https://fk.zhonguo4118.cn

[E05] 判断包含 / 前缀 / 后缀
来源：https://uf.zhonguo1118.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：https://oc.zhonguo4118.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：https://yq.zhonguo3118.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：https://xe.zhonguo1118.cn

TS:   s.includes("x");  s.startsWith("a")
来源：https://ta.zhonguo5118.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：https://yk.zhonguo1118.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：https://wh.zhonguo7118.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：https://iz.zhonguo1118.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：https://ak.zhonguo4118.cn

[E06] 替换子串
来源：https://tr.zhonguo1118.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：https://yi.zhonguo1118.cn

PHP:  str_replace("a", "b", $s);
来源：https://is.zhonguo7118.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://xz.zhonguo3118.cn

TS:   s.replaceAll("a", "b")
来源：https://sg.zhonguo3118.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://yw.zhonguo2118.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：https://xx.zhonguo1118.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：https://tx.zhonguo2118.cn

C#:   s.Replace("a", "b")
来源：https://ay.zhonguo3118.cn

[E07] 按分隔符拆分
来源：https://vn.zhonguo8118.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：https://ky.zhonguo6118.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：https://yi.zhonguo1118.cn

JS:   s.split(",");  s.split(/\s+/)
来源：https://tb.zhonguo8118.cn

TS:   s.split(",")
来源：https://uc.zhonguo4118.cn

Java: s.split(",");  s.split("\\s+")
来源：https://xq.zhonguo6118.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：https://ko.zhonguo1118.cn

Ruby: s.split(",");  s.split
来源：https://fd.zhonguo4118.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：https://ao.zhonguo2118.cn

[E08] 数组按分隔符合并
来源：https://dq.zhonguo5118.cn

Py:   ",".join(items)
来源：https://ri.zhonguo4118.cn

PHP:  implode(",", $items);
来源：https://zh.zhonguo2118.cn

JS:   items.join(",")
来源：https://ka.zhonguo2118.cn

TS:   items.join(",")
来源：https://ho.zhonguo6118.cn

Java: String.join(",", items)
来源：https://gf.zhonguo7118.cn

Go:   strings.Join(items, ",")
来源：https://cl.zhonguo1118.cn

Ruby: items.join(",")
来源：https://np.zhonguo1118.cn

C#:   string.Join(",", items)
来源：https://jz.zhonguo2118.cn

[E09] 去除所有空白字符
来源：https://qq.zhonguo6118.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：https://ne.zhonguo8118.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：https://uw.zhonguo7118.cn

JS:   s.replace(/\s+/g, "")
来源：https://ta.zhonguo1118.cn

TS:   s.replace(/\s+/g, "")
来源：https://wh.zhonguo1118.cn

Java: s.replaceAll("\\s+", "")
来源：https://hx.zhonguo5118.cn

Go:   strings.Join(strings.Fields(s), "")
来源：https://pg.zhonguo2118.cn

Ruby: s.gsub(/\s+/, "")
来源：https://za.zhonguo5118.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：https://gt.zhonguo7118.cn

[E10] 左侧补零 / 定长填充
来源：https://vi.zhonguo3118.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：https://qj.zhonguo7118.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：https://lo.zhonguo1118.cn

JS:   "7".padStart(3, "0")
来源：https://sk.zhonguo5118.cn

TS:   "7".padStart(3, "0")
来源：https://nz.zhonguo7118.cn

Java: String.format("%03d", 7)
来源：https://yi.zhonguo8118.cn

Go:   fmt.Sprintf("%03d", 7)
来源：https://sy.zhonguo2118.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：https://ex.zhonguo7118.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：https://zq.zhonguo1118.cn

[E11] 反转字符串
来源：https://vp.zhonguo5118.cn

Py:   s[::-1]
来源：https://yo.zhonguo4118.cn

PHP:  strrev($s);
来源：https://fi.zhonguo6118.cn

JS:   [...s].reverse().join("")
来源：https://pe.zhonguo5118.cn

TS:   [...s].reverse().join("")
来源：https://au.zhonguo4118.cn

Java: new StringBuilder(s).reverse().toString()
来源：https://dh.zhonguo3118.cn

Go:   // 转 []rune 后倒序再转回 string
来源：https://gz.zhonguo2118.cn

Ruby: s.reverse
来源：https://dh.zhonguo4118.cn

C#:   new string(s.Reverse().ToArray())
来源：https://lc.zhonguo1118.cn

[E12] 统计某字符出现次数
来源：https://ho.zhonguo7118.cn

Py:   s.count("a")
来源：https://fq.zhonguo5118.cn

PHP:  substr_count($s, "a");
来源：https://wv.zhonguo1118.cn

JS:   s.split("a").length - 1
来源：https://og.zhonguo5118.cn

TS:   s.split("a").length - 1
来源：https://au.zhonguo3118.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：https://fw.zhonguo8118.cn

Go:   strings.Count(s, "a")
来源：https://lj.zhonguo4118.cn

Ruby: s.count("a")
来源：https://pd.zhonguo3118.cn

C#:   s.Count(c => c == 'a')
来源：https://ro.zhonguo4118.cn

[E13] 逐字符遍历
来源：https://zx.zhonguo5118.cn

Py:   for ch in s: print(ch)
来源：https://oc.zhonguo4118.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：https://tx.zhonguo1118.cn

JS:   for (const ch of s) { console.log(ch); }
来源：https://ai.zhonguo2118.cn

TS:   for (const ch of s) { console.log(ch); }
来源：https://hd.zhonguo2118.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：https://hv.zhonguo5118.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：https://hd.zhonguo6118.cn

Ruby: s.each_char { |ch| puts ch }
来源：https://ow.zhonguo4118.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：https://ms.zhonguo3118.cn

[E14] URL 编码与 Base64
来源：https://fw.zhonguo4118.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：https://if.zhonguo6118.cn

PHP:  urlencode($s);  base64_encode($s);
来源：https://ff.zhonguo6118.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：https://kb.zhonguo2118.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：https://vd.zhonguo8118.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：https://ln.zhonguo8118.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：https://pb.zhonguo5118.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：https://dv.zhonguo1118.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：https://jt.zhonguo2118.cn

[E15] HTML 转义 / 反转义
来源：https://wf.zhonguo8118.cn

Py:   html.escape(s);  html.unescape(s)
来源：https://ym.zhonguo4118.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：https://no.zhonguo4118.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：https://ya.zhonguo7118.cn

TS:   // 同上，务必做 XSS 过滤
来源：https://uy.zhonguo8118.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：https://mr.zhonguo6118.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：https://ut.zhonguo7118.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：https://ro.zhonguo8118.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：https://mm.zhonguo7118.cn

[E16] 数字千分位
来源：https://lk.zhonguo6118.cn

Py:   f"{1234567:,}"
来源：https://ru.zhonguo5118.cn

PHP:  number_format(1234567);
来源：https://aj.zhonguo7118.cn

JS:   (1234567).toLocaleString("en-US")
来源：https://pv.zhonguo7118.cn

TS:   (1234567).toLocaleString("en-US")
来源：https://wd.zhonguo7118.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：https://xc.zhonguo5118.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：https://lx.zhonguo6118.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：https://kv.zhonguo3118.cn

C#:   1234567.ToString("N0")
来源：https://nm.zhonguo1118.cn

[E17] 首字母大写
来源：https://xx.zhonguo7118.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：https://zz.zhonguo5118.cn

PHP:  ucfirst($s);  ucwords($s);
来源：https://nx.zhonguo1118.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://kh.zhonguo2118.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://ax.zhonguo1118.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：https://er.zhonguo4118.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：https://ek.zhonguo8118.cn

Ruby: s.capitalize
来源：https://cs.zhonguo7118.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：https://vp.zhonguo7118.cn

[E18] 模板占位符替换
来源：https://zy.zhonguo5118.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：https://uy.zhonguo5118.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：https://dy.zhonguo2118.cn

JS:   tpl.replaceAll("{name}", name)
来源：https://rl.zhonguo2118.cn

TS:   tpl.replaceAll("{name}", name)
来源：https://wd.zhonguo4118.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：https://uf.zhonguo2118.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：https://ex.zhonguo5118.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：https://pw.zhonguo5118.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：https://ez.zhonguo1118.cn

[E19] 多行文本按行拆分
来源：https://sn.zhonguo2118.cn

Py:   s.splitlines()
来源：https://ve.zhonguo2118.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：https://ur.zhonguo3118.cn

JS:   s.split(/\r?\n/)
来源：https://xd.zhonguo4118.cn

TS:   s.split(/\r?\n/)
来源：https://tg.zhonguo3118.cn

Java: s.lines().toList()
来源：https://gt.zhonguo1118.cn

Go:   strings.Split(s, "\n")
来源：https://hz.zhonguo8118.cn

Ruby: s.lines
来源：https://po.zhonguo7118.cn

C#:   s.Split('\n')
来源：https://hq.zhonguo4118.cn

[E20] 判断字符串是否为空
来源：https://dv.zhonguo7118.cn

Py:   if not s:
来源：https://kc.zhonguo8118.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：https://zy.zhonguo5118.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：https://ks.zhonguo8118.cn

TS:   if (s === "") {}
来源：https://ma.zhonguo4118.cn

Java: if (s.isEmpty()) {}
来源：https://hm.zhonguo8118.cn

Go:   if s == "" {}
来源：https://pg.zhonguo3118.cn

Ruby: if s.empty?
来源：https://yp.zhonguo6118.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：https://ov.zhonguo6118.cn

[E21] 超长截断加省略号
来源：https://mm.zhonguo3118.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：https://kn.zhonguo1118.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：https://oi.zhonguo3118.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://ob.zhonguo5118.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://kj.zhonguo7118.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：https://za.zhonguo4118.cn

Go:   // 按 rune 判断长度后截断
来源：https://ub.zhonguo7118.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：https://xa.zhonguo7118.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：https://nj.zhonguo1118.cn

[E22] 字节长度与字符长度
来源：https://zn.zhonguo8118.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：https://kn.zhonguo7118.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：https://dj.zhonguo6118.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：https://jq.zhonguo1118.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：https://oh.zhonguo7118.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：https://lp.zhonguo5118.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：https://xi.zhonguo5118.cn

Ruby: s.bytesize;  s.length
来源：https://er.zhonguo6118.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：https://bw.zhonguo4118.cn

================================================================================
来源：https://sf.zhonguo5118.cn

F. 文件与目录
来源：https://fv.zhonguo1118.cn

================================================================================
来源：https://qy.zhonguo4118.cn

[F01] 读取整个文件
来源：https://yk.zhonguo2118.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：https://hi.zhonguo3118.cn

PHP:  file_get_contents("a.txt");
来源：https://di.zhonguo2118.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：https://ap.zhonguo3118.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：https://vw.zhonguo8118.cn

Java: Files.readString(Path.of("a.txt"))
来源：https://ic.zhonguo1118.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：https://nv.zhonguo8118.cn

Ruby: File.read("a.txt")
来源：https://mt.zhonguo7118.cn

C#:   File.ReadAllText("a.txt");
来源：https://pt.zhonguo4118.cn

[F02] 逐行读取文件
来源：https://bz.zhonguo8118.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：https://gw.zhonguo2118.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：https://gu.zhonguo5118.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://pg.zhonguo3118.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://nk.zhonguo7118.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：https://tb.zhonguo2118.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：https://ft.zhonguo3118.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：https://qf.zhonguo4118.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：https://lw.zhonguo8118.cn

[F03] 写入文件（覆盖）
来源：https://qa.zhonguo2118.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：https://dp.zhonguo2118.cn

PHP:  file_put_contents("a.txt", "hi");
来源：https://od.zhonguo8118.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://wh.zhonguo2118.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://iz.zhonguo1118.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：https://cu.zhonguo6118.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：https://cw.zhonguo2118.cn

Ruby: File.write("a.txt", "hi")
来源：https://yf.zhonguo8118.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：https://ec.zhonguo3118.cn

[F04] 追加写入文件
来源：https://lk.zhonguo1118.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：https://dp.zhonguo6118.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：https://ub.zhonguo6118.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：https://rf.zhonguo6118.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：https://wg.zhonguo6118.cn


<!-- 参考信息 -->