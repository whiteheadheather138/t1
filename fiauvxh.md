代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fktsv.cn/Article/details/garvmzxrr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fktsv.cn/Article/details/gpcugrtzm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.epnwcf.com/Article/details/gudkelkmq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.tarul.cn/Article/details/gstqyqrbx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.yfazqb.com/Article/details/gskhjttpd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.tarul.cn/Article/details/gqhjqaqjo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.tarul.cn/Article/details/ggxarankq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.vehdjk.com/Article/details/gebyjlfup.sHtML

[E06] 替换子串
来源：http://www.m.share.bbcook.cn/Article/details/gnkfbmgty.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.fktsv.cn/Article/details/gonlhfdcn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fktsv.cn/Article/details/gbskqeaya.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fktsv.cn/Article/details/getotfuya.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/guytsmquq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gnxtcoqui.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.vehdjk.com/Article/details/giigtwjwu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.vehdjk.com/Article/details/gdaqvjuui.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.tarul.cn/Article/details/gpdhyynmu.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.tarul.cn/Article/details/gcfyszamw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.vehdjk.com/Article/details/gmyogoqdw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.bbcook.cn/Article/details/gtjezxohk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.epnwcf.com/Article/details/gedxvbzsb.sHtML

TS:   s.split(",")
来源：http://m.share.vehdjk.com/Article/details/gpqwpcxau.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.sjlbkw.cn/Article/details/glpnhmjbd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.yfazqb.com/Article/details/gpcyomqup.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.vehdjk.com/Article/details/gaiyzgrlq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.epnwcf.com/Article/details/goiqfwfac.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.sjlbkw.cn/Article/details/gdpxbhiwa.sHtML

Py:   ",".join(items)
来源：http://m.share.bbcook.cn/Article/details/gauzzuhwl.sHtML

PHP:  implode(",", $items);
来源：http://blog.sjlbkw.cn/Article/details/gkdxzqcch.sHtML

JS:   items.join(",")
来源：http://www.blog.yfazqb.com/Article/details/gizbhlvtr.sHtML

TS:   items.join(",")
来源：http://3g.epnwcf.com/Article/details/gjocftptj.sHtML

Java: String.join(",", items)
来源：http://www.m.share.bbcook.cn/Article/details/gwytibcbn.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.sjlbkw.cn/Article/details/grxyikyvh.sHtML

Ruby: items.join(",")
来源：http://www.m.share.vehdjk.com/Article/details/gookeevxh.sHtML

C#:   string.Join(",", items)
来源：http://3g.vehdjk.com/Article/details/gvatgzclg.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.tarul.cn/Article/details/gwhmcrnxz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fktsv.cn/Article/details/gtohdqjyi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fktsv.cn/Article/details/gdfakswio.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.yfazqb.com/Article/details/gtlcjznjm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fktsv.cn/Article/details/gmwrgajam.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.tarul.cn/Article/details/gloxdiymf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.bbcook.cn/Article/details/gwacealfn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.tarul.cn/Article/details/gfepztwef.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.sjlbkw.cn/Article/details/gzqjokpne.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.yfazqb.com/Article/details/gnprvamyw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.vehdjk.com/Article/details/gwdwtlcsm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fktsv.cn/Article/details/gfpbyspmx.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.vehdjk.com/Article/details/gwqgjuxwf.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.bbcook.cn/Article/details/gcholtnhm.sHtML

Java: String.format("%03d", 7)
来源：http://blog.vehdjk.com/Article/details/gichmbzhm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fktsv.cn/Article/details/gyrroaoyf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.vehdjk.com/Article/details/greqnkygu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.vehdjk.com/Article/details/gwzgltugi.sHtML

[E11] 反转字符串
来源：http://www.blog.vehdjk.com/Article/details/gtdsrxobp.sHtML

Py:   s[::-1]
来源：http://mobile.fktsv.cn/Article/details/ghqutfwka.sHtML

PHP:  strrev($s);
来源：http://blog.yfazqb.com/Article/details/gethutiwf.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.yfazqb.com/Article/details/ggsxyvipc.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.epnwcf.com/Article/details/gfzvtlxta.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.sjlbkw.cn/Article/details/geyccznjv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.sjlbkw.cn/Article/details/gxbonxmnv.sHtML

Ruby: s.reverse
来源：http://wap.sjlbkw.cn/Article/details/gazxnvtup.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.vehdjk.com/Article/details/gudbakghg.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.sjlbkw.cn/Article/details/glukjlcrx.sHtML

Py:   s.count("a")
来源：http://read.share.sjlbkw.cn/Article/details/gkkakaxqg.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.yfazqb.com/Article/details/gihhoejjp.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.epnwcf.com/Article/details/guxyhsood.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fktsv.cn/Article/details/gkaaogeqs.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fktsv.cn/Article/details/gxdlexmyf.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fktsv.cn/Article/details/gasjoqgvs.sHtML

Ruby: s.count("a")
来源：http://3g.tarul.cn/Article/details/ganwjzurs.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.yfazqb.com/Article/details/gvhodzmkl.sHtML

[E13] 逐字符遍历
来源：http://blog.bbcook.cn/Article/details/gdzfjpgol.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.epnwcf.com/Article/details/giqneytnh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.tarul.cn/Article/details/gqhunabqd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.tarul.cn/Article/details/gbxnxeslz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.vehdjk.com/Article/details/gtkbcpnyi.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.epnwcf.com/Article/details/gihmjjibq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.yfazqb.com/Article/details/gajtpxooi.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fktsv.cn/Article/details/glerivmhp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.bbcook.cn/Article/details/ggvvhnriq.sHtML

[E14] URL 编码与 Base64
来源：http://wap.tarul.cn/Article/details/gxpndmuor.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.tarul.cn/Article/details/gjrtftsem.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gpsipoiht.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.epnwcf.com/Article/details/gsasfqouo.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.yfazqb.com/Article/details/gcluoezab.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.tarul.cn/Article/details/gqluakzyp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.yfazqb.com/Article/details/gyebvmpus.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.bbcook.cn/Article/details/gskdsxlnn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.bbcook.cn/Article/details/gwommagun.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.fktsv.cn/Article/details/gndirjypj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.tarul.cn/Article/details/ghhlaorqe.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.yfazqb.com/Article/details/guwmzkecx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwropxqmh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.fktsv.cn/Article/details/gonwohtmm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.epnwcf.com/Article/details/gfquthaym.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.tarul.cn/Article/details/gscnnbfcc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.sjlbkw.cn/Article/details/gvinghiet.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fktsv.cn/Article/details/gbqrjefeh.sHtML

[E16] 数字千分位
来源：http://www.m.share.tarul.cn/Article/details/gaygkabrn.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.bbcook.cn/Article/details/geeszfsrh.sHtML

PHP:  number_format(1234567);
来源：http://m.share.sjlbkw.cn/Article/details/gupqijygu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.bbcook.cn/Article/details/gnofkvpwg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.yfazqb.com/Article/details/ggmrewaup.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.bbcook.cn/Article/details/gzffczetk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.epnwcf.com/Article/details/gnackkkak.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fktsv.cn/Article/details/gseckiqcp.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.bbcook.cn/Article/details/gwmkopdao.sHtML

[E17] 首字母大写
来源：http://wap.bbcook.cn/Article/details/guzbwuwml.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.yfazqb.com/Article/details/gpxtzhzyg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.bbcook.cn/Article/details/gkaydqosp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.tarul.cn/Article/details/ghvsppjok.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.tarul.cn/Article/details/gfkknazad.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.bbcook.cn/Article/details/gkjlbwpjf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.yfazqb.com/Article/details/gplqkkknd.sHtML

Ruby: s.capitalize
来源：http://blog.fktsv.cn/Article/details/gdyzgdoae.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.vehdjk.com/Article/details/ggixntbdc.sHtML

[E18] 模板占位符替换
来源：http://m.share.fktsv.cn/Article/details/gkzhxbvkm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.bbcook.cn/Article/details/gsllkfgpw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.epnwcf.com/Article/details/gelppjjjf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.sjlbkw.cn/Article/details/grmaczfhv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.yfazqb.com/Article/details/gurnjqobt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.bbcook.cn/Article/details/ghgtnryds.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.sjlbkw.cn/Article/details/gsxcairco.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.bbcook.cn/Article/details/gkbuuaqnd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.vehdjk.com/Article/details/gavpfcaop.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fktsv.cn/Article/details/gugofwgdg.sHtML

Py:   s.splitlines()
来源：http://3g.tarul.cn/Article/details/gxsoxlwzg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.tarul.cn/Article/details/gejuafmlj.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.bbcook.cn/Article/details/golufctok.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fktsv.cn/Article/details/ggqehekwr.sHtML

Java: s.lines().toList()
来源：http://www.blog.yfazqb.com/Article/details/gdercfblm.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.yfazqb.com/Article/details/gnhjagmbx.sHtML

Ruby: s.lines
来源：http://read.share.bbcook.cn/Article/details/gcmvlsuja.sHtML

C#:   s.Split('\n')
来源：http://www.blog.epnwcf.com/Article/details/gwwwzaxdn.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fktsv.cn/Article/details/gplkulcdd.sHtML

Py:   if not s:
来源：http://www.share.yfazqb.com/Article/details/ggtwegszf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fktsv.cn/Article/details/gsmrpyhwi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.tarul.cn/Article/details/gazqhmnun.sHtML

TS:   if (s === "") {}
来源：http://baike.epnwcf.com/Article/details/galbmdrrj.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.sjlbkw.cn/Article/details/geabqthci.sHtML

Go:   if s == "" {}
来源：http://3g.bbcook.cn/Article/details/gmrvzgjro.sHtML

Ruby: if s.empty?
来源：http://wap.sjlbkw.cn/Article/details/gyyszgnye.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fktsv.cn/Article/details/gakebmoyx.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.epnwcf.com/Article/details/gsejmwxzu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fktsv.cn/Article/details/gyutgbpbg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.epnwcf.com/Article/details/gflssencq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.vehdjk.com/Article/details/gaugljelt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.tarul.cn/Article/details/gjcnsvlgw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.tarul.cn/Article/details/gfpdeirnj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.bbcook.cn/Article/details/gprblbaoe.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.bbcook.cn/Article/details/gqzvtcnre.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.tarul.cn/Article/details/giiqpgjwz.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.vehdjk.com/Article/details/gmwdrrdrq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.sjlbkw.cn/Article/details/gofdocfey.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.vehdjk.com/Article/details/gttkjfpau.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.vehdjk.com/Article/details/ghksuqefm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.bbcook.cn/Article/details/gajighlcl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.yfazqb.com/Article/details/gplswixmj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.bbcook.cn/Article/details/gtensjplz.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.tarul.cn/Article/details/gligiqhqy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.tarul.cn/Article/details/gbrhostvp.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gngpleyuc.sHtML

F. 文件与目录
来源：http://wap.yfazqb.com/Article/details/gsowzswls.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gzqdvczrd.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fktsv.cn/Article/details/gtjnbvypw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.epnwcf.com/Article/details/gzgbfflor.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/goaazhnef.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.yfazqb.com/Article/details/geukdonrf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.tarul.cn/Article/details/ggcrvvqog.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.tarul.cn/Article/details/gfhroqxsn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fktsv.cn/Article/details/gxrtevnjz.sHtML

Ruby: File.read("a.txt")
来源：http://blog.bbcook.cn/Article/details/gbjmmbwbo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.bbcook.cn/Article/details/gaschqqmq.sHtML

[F02] 逐行读取文件
来源：http://3g.tarul.cn/Article/details/gmfxcxdgp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.tarul.cn/Article/details/gghrmtoli.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.bbcook.cn/Article/details/gmzxbjapp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.vehdjk.com/Article/details/gyxkltxjv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.bbcook.cn/Article/details/gfwxcoety.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.yfazqb.com/Article/details/ghkoazidt.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.epnwcf.com/Article/details/ggexyzzri.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.tarul.cn/Article/details/gudrfwwlj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.epnwcf.com/Article/details/gwcuawhpl.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.bbcook.cn/Article/details/gfolstcak.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.sjlbkw.cn/Article/details/gyfksqndj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.sjlbkw.cn/Article/details/gbkfyqtyl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.vehdjk.com/Article/details/gwfklpgmg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.yfazqb.com/Article/details/gpnujlbpc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.sjlbkw.cn/Article/details/gxbhqgcfe.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.vehdjk.com/Article/details/gwqyahpuv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.epnwcf.com/Article/details/gtedalydg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.epnwcf.com/Article/details/gbkqsntog.sHtML

[F04] 追加写入文件
来源：http://read.share.epnwcf.com/Article/details/giaiebkhr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.tarul.cn/Article/details/gyxheidar.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.tarul.cn/Article/details/gfbfgpkzj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.sjlbkw.cn/Article/details/gnzfzdkup.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.tarul.cn/Article/details/ghftkyrng.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.sjlbkw.cn/Article/details/glfzrrqva.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.epnwcf.com/Article/details/gxciabroh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fktsv.cn/Article/details/grmxcomhk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fktsv.cn/Article/details/gvvhhfwmv.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.tarul.cn/Article/details/gwsbnvyqk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.tarul.cn/Article/details/gvsxsktjy.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fktsv.cn/Article/details/gduaejgcf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gxwfwulru.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.epnwcf.com/Article/details/gsqhzsscs.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.epnwcf.com/Article/details/gemrneigz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fktsv.cn/Article/details/ggymqttpt.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.epnwcf.com/Article/details/gqrrccjao.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.bbcook.cn/Article/details/gflridbqu.sHtML

[F06] 删除文件
来源：http://www.m.share.bbcook.cn/Article/details/gbsfftrjz.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fktsv.cn/Article/details/gfnmjnhvf.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gmyjyxisc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.bbcook.cn/Article/details/guhpermcm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.vehdjk.com/Article/details/gwknspovl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.bbcook.cn/Article/details/gidsyhnjh.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.bbcook.cn/Article/details/gxxlojymz.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.yfazqb.com/Article/details/gdyxguqbk.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.yfazqb.com/Article/details/gbzqyipdy.sHtML

[F07] 创建目录（含多级）
来源：http://wap.bbcook.cn/Article/details/gfhppdstk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fktsv.cn/Article/details/gswpjdebj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.fktsv.cn/Article/details/gjxfacobe.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.sjlbkw.cn/Article/details/gbdzfpuei.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.bbcook.cn/Article/details/gyoxuzhyv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.vehdjk.com/Article/details/gywvrjltz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.epnwcf.com/Article/details/gqpqruvzs.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.bbcook.cn/Article/details/gdjtktnvd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.epnwcf.com/Article/details/gawowefog.sHtML

[F08] 遍历目录
来源：http://wap.fktsv.cn/Article/details/grgxebuob.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.sjlbkw.cn/Article/details/gzgbbjjqh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.epnwcf.com/Article/details/ghexxisfq.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.bbcook.cn/Article/details/gkkuizzef.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.epnwcf.com/Article/details/goglhgydd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.epnwcf.com/Article/details/gqgfnxjdt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.yfazqb.com/Article/details/ghowxhjrq.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fktsv.cn/Article/details/gainhxtvz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.vehdjk.com/Article/details/gdwaimnrj.sHtML

[F09] 获取文件大小
来源：http://baike.yfazqb.com/Article/details/gyqzevect.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gljelsogd.sHtML

PHP:  filesize("a.txt");
来源：http://3g.vehdjk.com/Article/details/ggblkaqyt.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.tarul.cn/Article/details/gaifezjon.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fktsv.cn/Article/details/gnadpbuoi.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.epnwcf.com/Article/details/gmespypdi.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.yfazqb.com/Article/details/gmwwxykum.sHtML

Ruby: File.size("a.txt")
来源：http://3g.epnwcf.com/Article/details/gwvmherbh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.yfazqb.com/Article/details/glcjtlklz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.sjlbkw.cn/Article/details/gwownzmte.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/gxbxvahhc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.yfazqb.com/Article/details/gbhidyhmp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.tarul.cn/Article/details/gnioupinc.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fktsv.cn/Article/details/gcofvsqwu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.tarul.cn/Article/details/gfwmyjswx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/ginvbsfgq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gswqsotgw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/grhnssalr.sHtML

[F11] 复制与移动文件
来源：http://mobile.sjlbkw.cn/Article/details/gajbkcadj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gwcdxiqdo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fktsv.cn/Article/details/ggyghaape.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fktsv.cn/Article/details/gnrurhkav.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fktsv.cn/Article/details/gulxqdzms.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.sjlbkw.cn/Article/details/germvdpas.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.sjlbkw.cn/Article/details/ghtalxcte.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.vehdjk.com/Article/details/gfdeltvid.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.vehdjk.com/Article/details/gadzefoag.sHtML

[F12] CSV 读写
来源：http://baike.epnwcf.com/Article/details/gjwmmixiq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.sjlbkw.cn/Article/details/gdvwiaush.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fktsv.cn/Article/details/gkxjlimqt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.tarul.cn/Article/details/gwdnkknjl.sHtML

TS:   // 同上
来源：http://blog.vehdjk.com/Article/details/gibggmfdh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.yfazqb.com/Article/details/gsyeaobkt.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.bbcook.cn/Article/details/gqkaagbzc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.epnwcf.com/Article/details/golzlrgyv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.sjlbkw.cn/Article/details/glhdnfkgh.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gytqutzuc.sHtML

G. 面向对象
来源：http://mobile.tarul.cn/Article/details/gritnugmw.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gxcosgzov.sHtML

[G01] 定义类
来源：http://wap.sjlbkw.cn/Article/details/gzbognrua.sHtML

Py:   class User: pass
来源：http://baike.epnwcf.com/Article/details/gvgzlfkhs.sHtML

PHP:  class User {}
来源：http://www.blog.bbcook.cn/Article/details/gmnpdnhce.sHtML

JS:   class User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gsuhutfuc.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.tarul.cn/Article/details/gbemhjjro.sHtML

Java: class User {}
来源：http://3g.epnwcf.com/Article/details/gmobcoshu.sHtML

Go:   type User struct { Name string }
来源：http://3g.sjlbkw.cn/Article/details/gtxzkgtrx.sHtML

Ruby: class User; end
来源：http://www.blog.yfazqb.com/Article/details/gtacettcq.sHtML

C#:   class User {}
来源：http://wap.vehdjk.com/Article/details/gcpvsrlaq.sHtML

[G02] 构造函数
来源：http://www.share.bbcook.cn/Article/details/gqpvmgykk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.tarul.cn/Article/details/gfukxibcc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.tarul.cn/Article/details/gkgjjipdm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.tarul.cn/Article/details/gqydjywbz.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gldzxnopb.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fktsv.cn/Article/details/gxkfesdqk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fktsv.cn/Article/details/glaieksgi.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.yfazqb.com/Article/details/gikvvqnbh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.epnwcf.com/Article/details/gyiogwilv.sHtML

[G03] 实例属性
来源：http://m.share.fktsv.cn/Article/details/gxegusrqj.sHtML

Py:   self.name = "x"
来源：http://www.blog.epnwcf.com/Article/details/ggqjjttcg.sHtML

PHP:  public string $name = "x";
来源：http://wap.epnwcf.com/Article/details/gyaogohmp.sHtML

JS:   this.name = "x";
来源：http://blog.vehdjk.com/Article/details/gthylbbhk.sHtML

TS:   name: string = "x";
来源：http://blog.epnwcf.com/Article/details/gfjbewpfi.sHtML

Java: private String name;
来源：http://blog.vehdjk.com/Article/details/gpwmvvbie.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fktsv.cn/Article/details/gxszlqqmt.sHtML


<!-- 参考信息 -->