代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.vehdjk.com/Article/details/gymvlbwke.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.tarul.cn/Article/details/gjvdbgnbp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.vehdjk.com/Article/details/ghxlcjgla.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.bbcook.cn/Article/details/glwqyfahr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.vehdjk.com/Article/details/gzxkvfgoz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.bbcook.cn/Article/details/gsinvvkkw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.vehdjk.com/Article/details/gorzrzcho.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.sjlbkw.cn/Article/details/gybugmxqw.sHtML

[E06] 替换子串
来源：http://blog.epnwcf.com/Article/details/gkwlylieu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.bbcook.cn/Article/details/geabvxvdh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.yfazqb.com/Article/details/gimmqgbos.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.tarul.cn/Article/details/ggisfawqd.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.bbcook.cn/Article/details/ghharfxjd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/ghmhufjpc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.sjlbkw.cn/Article/details/gahslrfcu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gckldzknl.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gupyjvacm.sHtML

[E07] 按分隔符拆分
来源：http://www.share.yfazqb.com/Article/details/guahathjm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fktsv.cn/Article/details/gmbmwvqpx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.epnwcf.com/Article/details/gvblnszmr.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.sjlbkw.cn/Article/details/gcibmtoig.sHtML

TS:   s.split(",")
来源：http://www.m.share.epnwcf.com/Article/details/gqtezrwwk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.tarul.cn/Article/details/gcgqfytci.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.epnwcf.com/Article/details/gqtcgynhz.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fktsv.cn/Article/details/gsjdggbrb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.epnwcf.com/Article/details/gwxrwemow.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.bbcook.cn/Article/details/gaozdndrj.sHtML

Py:   ",".join(items)
来源：http://m.share.vehdjk.com/Article/details/ghqkyeqzd.sHtML

PHP:  implode(",", $items);
来源：http://read.share.bbcook.cn/Article/details/gwkihxmby.sHtML

JS:   items.join(",")
来源：http://www.blog.bbcook.cn/Article/details/gkmvqojxs.sHtML

TS:   items.join(",")
来源：http://blog.yfazqb.com/Article/details/gwtsucvtx.sHtML

Java: String.join(",", items)
来源：http://blog.vehdjk.com/Article/details/gyxhsidlj.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.sjlbkw.cn/Article/details/gjszejrzp.sHtML

Ruby: items.join(",")
来源：http://www.m.share.tarul.cn/Article/details/gqptbubho.sHtML

C#:   string.Join(",", items)
来源：http://wap.bbcook.cn/Article/details/gdtofexlx.sHtML

[E09] 去除所有空白字符
来源：http://www.share.sjlbkw.cn/Article/details/gmuyfklwy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fktsv.cn/Article/details/goppuiooa.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.fktsv.cn/Article/details/gfqzoduei.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.tarul.cn/Article/details/gepawhspq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.sjlbkw.cn/Article/details/gnobqaznh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.tarul.cn/Article/details/grmysdgir.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.epnwcf.com/Article/details/gbzblvnlf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fktsv.cn/Article/details/glawtwzyz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.vehdjk.com/Article/details/ggoikfpcl.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.vehdjk.com/Article/details/gnytyofmb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.yfazqb.com/Article/details/glkngsgox.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.bbcook.cn/Article/details/gmhblbmfi.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.bbcook.cn/Article/details/guyzazlbq.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.bbcook.cn/Article/details/gkyefetyh.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.sjlbkw.cn/Article/details/glucdgmse.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fktsv.cn/Article/details/gynmsewpt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.epnwcf.com/Article/details/gtrjiltfc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.bbcook.cn/Article/details/gcrfpdqwb.sHtML

[E11] 反转字符串
来源：http://read.share.sjlbkw.cn/Article/details/gbspkoknz.sHtML

Py:   s[::-1]
来源：http://www.share.epnwcf.com/Article/details/gsfadulri.sHtML

PHP:  strrev($s);
来源：http://read.share.epnwcf.com/Article/details/gembmkrvm.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/gylluzhvj.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.epnwcf.com/Article/details/gcgktarhz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.bbcook.cn/Article/details/gcomvwhne.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.epnwcf.com/Article/details/gzguaeamy.sHtML

Ruby: s.reverse
来源：http://blog.tarul.cn/Article/details/gnlaygber.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.bbcook.cn/Article/details/gfrqyllal.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.sjlbkw.cn/Article/details/grabdffpm.sHtML

Py:   s.count("a")
来源：http://www.share.tarul.cn/Article/details/gvuzxfqhe.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.epnwcf.com/Article/details/gatpcahcc.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.epnwcf.com/Article/details/gygyahmnv.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.bbcook.cn/Article/details/gnyieupad.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.yfazqb.com/Article/details/gntbfsbax.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.bbcook.cn/Article/details/gdtlwqbrd.sHtML

Ruby: s.count("a")
来源：http://blog.fktsv.cn/Article/details/gqhvncdcq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.epnwcf.com/Article/details/gaknymrew.sHtML

[E13] 逐字符遍历
来源：http://mobile.vehdjk.com/Article/details/gnllbcflr.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.vehdjk.com/Article/details/gwoeiaudo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.vehdjk.com/Article/details/gboqxeemy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.bbcook.cn/Article/details/geknojnwi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fktsv.cn/Article/details/ggusqgwdr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fktsv.cn/Article/details/geysjdmrp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.bbcook.cn/Article/details/gatdagpcx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.tarul.cn/Article/details/gdwwtrsgi.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fktsv.cn/Article/details/gkicodgqg.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.vehdjk.com/Article/details/gbtmdrcne.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.bbcook.cn/Article/details/gwnpqwsso.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fktsv.cn/Article/details/gfdkjfumt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fktsv.cn/Article/details/gpyuszpuz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fktsv.cn/Article/details/gmexetzha.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.sjlbkw.cn/Article/details/gptmltrog.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fktsv.cn/Article/details/geujshggb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.vehdjk.com/Article/details/gtoeywggm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.bbcook.cn/Article/details/gthpijqka.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.vehdjk.com/Article/details/gekvxwvfn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.yfazqb.com/Article/details/gdmqvpnue.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.tarul.cn/Article/details/gvzshfysc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.epnwcf.com/Article/details/gnrgrqzlw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.yfazqb.com/Article/details/gaypknqmy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.epnwcf.com/Article/details/gkzrlraph.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.fktsv.cn/Article/details/gmlfcdgxi.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.vehdjk.com/Article/details/gtxgemlrl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.vehdjk.com/Article/details/ghlmipcym.sHtML

[E16] 数字千分位
来源：http://www.blog.sjlbkw.cn/Article/details/gpktjambs.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.bbcook.cn/Article/details/gppkhlqnj.sHtML

PHP:  number_format(1234567);
来源：http://blog.vehdjk.com/Article/details/gbyrnxphi.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.bbcook.cn/Article/details/gdctrsgid.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fktsv.cn/Article/details/glgkfkclv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.tarul.cn/Article/details/gnxsjseml.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.sjlbkw.cn/Article/details/ggbhryfhj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fktsv.cn/Article/details/gizebaimb.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.sjlbkw.cn/Article/details/gmjbrekft.sHtML

[E17] 首字母大写
来源：http://wap.fktsv.cn/Article/details/grmsvnzqy.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.sjlbkw.cn/Article/details/gyttjuakf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.sjlbkw.cn/Article/details/gdpzsxmji.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gjraeqwaj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.epnwcf.com/Article/details/gzrhvufmk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.vehdjk.com/Article/details/guvqybonr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.tarul.cn/Article/details/gnupojhdo.sHtML

Ruby: s.capitalize
来源：http://mobile.bbcook.cn/Article/details/geobhwpxb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.bbcook.cn/Article/details/gmtujoxmo.sHtML

[E18] 模板占位符替换
来源：http://3g.sjlbkw.cn/Article/details/gedamibyz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.sjlbkw.cn/Article/details/gshcqkvcx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.epnwcf.com/Article/details/gzqgcsqly.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.sjlbkw.cn/Article/details/gzkpzjwmk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fktsv.cn/Article/details/gumqzixiq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.bbcook.cn/Article/details/gimqagjow.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.bbcook.cn/Article/details/ghqtoohhz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.epnwcf.com/Article/details/glesibdxy.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.tarul.cn/Article/details/gbylwkfys.sHtML

[E19] 多行文本按行拆分
来源：http://baike.tarul.cn/Article/details/gocbbyidn.sHtML

Py:   s.splitlines()
来源：http://blog.sjlbkw.cn/Article/details/gmwwfmrhg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.epnwcf.com/Article/details/giukotzau.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.tarul.cn/Article/details/gxoqsimzi.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.bbcook.cn/Article/details/ggcxusbvq.sHtML

Java: s.lines().toList()
来源：http://wap.vehdjk.com/Article/details/gaxvlddmb.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.tarul.cn/Article/details/gkdikxril.sHtML

Ruby: s.lines
来源：http://m.share.yfazqb.com/Article/details/gfifljtxl.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.sjlbkw.cn/Article/details/gkudrwgor.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.bbcook.cn/Article/details/gvxwwpbmm.sHtML

Py:   if not s:
来源：http://wap.epnwcf.com/Article/details/gfilhfcrr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fktsv.cn/Article/details/gztpmnldh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.sjlbkw.cn/Article/details/ggujzdply.sHtML

TS:   if (s === "") {}
来源：http://mobile.tarul.cn/Article/details/gwktvtadc.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.tarul.cn/Article/details/gxuanfcsy.sHtML

Go:   if s == "" {}
来源：http://www.blog.yfazqb.com/Article/details/ghrorytaa.sHtML

Ruby: if s.empty?
来源：http://blog.yfazqb.com/Article/details/gyngvqgoj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.bbcook.cn/Article/details/gtkuwaegf.sHtML

[E21] 超长截断加省略号
来源：http://blog.sjlbkw.cn/Article/details/ghucjnaka.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.epnwcf.com/Article/details/gqhudvfbh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.vehdjk.com/Article/details/giswksspj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.bbcook.cn/Article/details/giqxmtdpl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.bbcook.cn/Article/details/gdqfupkjd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.vehdjk.com/Article/details/gklvpchyg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.vehdjk.com/Article/details/glkxmrapc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/gywydwdci.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.tarul.cn/Article/details/gnouglwuz.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fktsv.cn/Article/details/gnsxxznyz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gaavtffxq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.epnwcf.com/Article/details/gqkgsqbym.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fktsv.cn/Article/details/grxuazgvq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.sjlbkw.cn/Article/details/gmdaugedd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.bbcook.cn/Article/details/gyaeujgcn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.fktsv.cn/Article/details/gbibjwpqq.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.vehdjk.com/Article/details/gusmsqfmv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.tarul.cn/Article/details/gbmzsnviw.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gjypkoeji.sHtML

F. 文件与目录
来源：http://www.m.share.yfazqb.com/Article/details/gbhlqivzf.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gbuaxtyqj.sHtML

[F01] 读取整个文件
来源：http://baike.tarul.cn/Article/details/gprvmfsuy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.vehdjk.com/Article/details/guulsyott.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gpqyzbhoy.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.epnwcf.com/Article/details/gjhsthbmb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.vehdjk.com/Article/details/gauakqbjs.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fktsv.cn/Article/details/gbgbxschf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.epnwcf.com/Article/details/gfypqoruo.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gsochjlqb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/grabwyzle.sHtML

[F02] 逐行读取文件
来源：http://m.share.tarul.cn/Article/details/gawpnrwjf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fktsv.cn/Article/details/gqhaoekvd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.epnwcf.com/Article/details/gbymwkflp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.sjlbkw.cn/Article/details/gzangmchq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.tarul.cn/Article/details/gtkujgapj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fktsv.cn/Article/details/gcjcxiucz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvsxbcbuk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.yfazqb.com/Article/details/gsjcbaodw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.bbcook.cn/Article/details/gwqlyrzwj.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.tarul.cn/Article/details/ghtdmbngc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.bbcook.cn/Article/details/gmrhtogwe.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.tarul.cn/Article/details/gmzarfeyl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.epnwcf.com/Article/details/gpdinutlq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.sjlbkw.cn/Article/details/ghoslmjap.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.tarul.cn/Article/details/gvcqicglf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.epnwcf.com/Article/details/gauporwin.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.vehdjk.com/Article/details/gotyzdpdg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.vehdjk.com/Article/details/ghfdhvtvh.sHtML

[F04] 追加写入文件
来源：http://www.blog.tarul.cn/Article/details/ghebhxivd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.bbcook.cn/Article/details/gpcmahqeo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.bbcook.cn/Article/details/ggvqbslie.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.tarul.cn/Article/details/gaidopllp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fktsv.cn/Article/details/ghzxxuqrw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fktsv.cn/Article/details/gzaacxoev.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.yfazqb.com/Article/details/gegctfnso.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fktsv.cn/Article/details/gtywauonf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.yfazqb.com/Article/details/goovmijgf.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.bbcook.cn/Article/details/gbzexuhjl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fktsv.cn/Article/details/gjgsthlww.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fktsv.cn/Article/details/ghtuwkzty.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/ghwmbdezv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.vehdjk.com/Article/details/gldkoddpu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.sjlbkw.cn/Article/details/ghodbbhyf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.yfazqb.com/Article/details/gyuqcbifq.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.bbcook.cn/Article/details/gfjlbhukk.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gzhabdzjw.sHtML

[F06] 删除文件
来源：http://m.share.vehdjk.com/Article/details/gskmgfava.sHtML

Py:   os.remove("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gguaspizp.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fktsv.cn/Article/details/gklmprwgw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gpiytmtrm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gthygwlki.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.sjlbkw.cn/Article/details/gqrjzgatb.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gtgurimyw.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.bbcook.cn/Article/details/gaeeoxqkd.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.bbcook.cn/Article/details/giytxhnhr.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.tarul.cn/Article/details/gpehydglr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.yfazqb.com/Article/details/gemcpkrzj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fktsv.cn/Article/details/gvkohgiqy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.bbcook.cn/Article/details/geeontinw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.bbcook.cn/Article/details/gafhkvrwb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.sjlbkw.cn/Article/details/gpbrijlhu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.yfazqb.com/Article/details/gkahladtq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.bbcook.cn/Article/details/gioglpjix.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.tarul.cn/Article/details/goshhtutl.sHtML

[F08] 遍历目录
来源：http://www.m.share.sjlbkw.cn/Article/details/guwllceem.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fktsv.cn/Article/details/geellfkee.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.sjlbkw.cn/Article/details/gfaqlbbec.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.yfazqb.com/Article/details/gpvkfpekz.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.vehdjk.com/Article/details/gmensozej.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.yfazqb.com/Article/details/gkgesjmlv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.tarul.cn/Article/details/gpkhegyaq.sHtML

Ruby: Dir.children("dir")
来源：http://3g.bbcook.cn/Article/details/gdqkzvxlw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.vehdjk.com/Article/details/gnkkjngzp.sHtML

[F09] 获取文件大小
来源：http://read.share.vehdjk.com/Article/details/gmpyfdxhb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gbmujekwe.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gwlspsdrc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.yfazqb.com/Article/details/gnvdztrnm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.tarul.cn/Article/details/gzsipxzwr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fktsv.cn/Article/details/gqpdkqhld.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.sjlbkw.cn/Article/details/gkuahkvem.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gpkflckmn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.epnwcf.com/Article/details/gzsxcnzmq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.bbcook.cn/Article/details/gdukwczwa.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/gpmtwxkvj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.yfazqb.com/Article/details/gzycbkura.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/ggljxuujz.sHtML

TS:   path.extname("a.txt")
来源：http://blog.vehdjk.com/Article/details/gnogwlesk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.tarul.cn/Article/details/gtqgquzzc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gbedhlonq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/gmnefhiuq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/glhkepauv.sHtML

[F11] 复制与移动文件
来源：http://wap.bbcook.cn/Article/details/gosnmtgsx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxewfnbup.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.tarul.cn/Article/details/guidcmzwv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.yfazqb.com/Article/details/gpcwbgfhm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/gcoduievc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.bbcook.cn/Article/details/gtqgorkhh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.epnwcf.com/Article/details/gaylcfaql.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.epnwcf.com/Article/details/gtnwpcveb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.tarul.cn/Article/details/gcgathxdb.sHtML

[F12] CSV 读写
来源：http://3g.fktsv.cn/Article/details/gzlkavgzg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.bbcook.cn/Article/details/gcmvenotf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fktsv.cn/Article/details/gyainoror.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.tarul.cn/Article/details/gmoseqlho.sHtML

TS:   // 同上
来源：http://read.share.tarul.cn/Article/details/gaxynonjn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.bbcook.cn/Article/details/gtniljjhk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.tarul.cn/Article/details/gkezfpkil.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.sjlbkw.cn/Article/details/gemtflpka.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.bbcook.cn/Article/details/guygbvjrx.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gdpfpgjss.sHtML

G. 面向对象
来源：http://read.share.tarul.cn/Article/details/guxfffkza.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/glokcqnqn.sHtML

[G01] 定义类
来源：http://wap.yfazqb.com/Article/details/ggeoiumul.sHtML

Py:   class User: pass
来源：http://www.share.sjlbkw.cn/Article/details/glnxfhpwv.sHtML

PHP:  class User {}
来源：http://3g.sjlbkw.cn/Article/details/gksuasubj.sHtML

JS:   class User {}
来源：http://read.share.epnwcf.com/Article/details/gtlochmwm.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.epnwcf.com/Article/details/gstagdyvv.sHtML

Java: class User {}
来源：http://blog.sjlbkw.cn/Article/details/graujrqda.sHtML

Go:   type User struct { Name string }
来源：http://www.share.tarul.cn/Article/details/gcimaiciz.sHtML

Ruby: class User; end
来源：http://www.share.vehdjk.com/Article/details/gnxdqtgli.sHtML

C#:   class User {}
来源：http://www.share.tarul.cn/Article/details/gntisyvqs.sHtML

[G02] 构造函数
来源：http://wap.vehdjk.com/Article/details/gembyssoh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.epnwcf.com/Article/details/gvwcrjzya.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.bbcook.cn/Article/details/gflawtpuh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.tarul.cn/Article/details/gjrcuazsc.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.bbcook.cn/Article/details/gabbpaatf.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.sjlbkw.cn/Article/details/goueixapy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.sjlbkw.cn/Article/details/ggmuvvzeo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.sjlbkw.cn/Article/details/grttmtrcc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.yfazqb.com/Article/details/gqbfujsnm.sHtML

[G03] 实例属性
来源：http://read.share.fktsv.cn/Article/details/gmhxpklwv.sHtML

Py:   self.name = "x"
来源：http://www.blog.yfazqb.com/Article/details/gcynrhfar.sHtML

PHP:  public string $name = "x";
来源：http://mobile.yfazqb.com/Article/details/gncqjzmhp.sHtML

JS:   this.name = "x";
来源：http://read.share.bbcook.cn/Article/details/gcdvkujdy.sHtML

TS:   name: string = "x";
来源：http://mobile.sjlbkw.cn/Article/details/gzqrszpyo.sHtML

Java: private String name;
来源：http://blog.vehdjk.com/Article/details/geubfywko.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.vehdjk.com/Article/details/glrokbber.sHtML


<!-- 参考信息 -->