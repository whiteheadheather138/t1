代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fktsv.cn/Article/details/gjeipjyip.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.sjlbkw.cn/Article/details/gjwxmvzkb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.bbcook.cn/Article/details/gjbbqksrl.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.yfazqb.com/Article/details/gkthoxwkl.sHtML

[E06] 替换子串
来源：http://3g.fktsv.cn/Article/details/gpaumqtym.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.sjlbkw.cn/Article/details/gxjmvwkux.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.vehdjk.com/Article/details/gxdpjxanv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.bbcook.cn/Article/details/gdfwbloyo.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.epnwcf.com/Article/details/gjqiyvice.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.tarul.cn/Article/details/gdvshehyr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.yfazqb.com/Article/details/gjxlzczmx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.vehdjk.com/Article/details/gvyadasfq.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gsplasrta.sHtML

[E07] 按分隔符拆分
来源：http://blog.bbcook.cn/Article/details/gdwacwagq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.sjlbkw.cn/Article/details/ghbcmxnlx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.epnwcf.com/Article/details/gvddazmbp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.bbcook.cn/Article/details/gwpxqacgq.sHtML

TS:   s.split(",")
来源：http://www.share.yfazqb.com/Article/details/geokdtpsc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.sjlbkw.cn/Article/details/gzeibiume.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.yfazqb.com/Article/details/gkkqgfypm.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fktsv.cn/Article/details/guupnisxa.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fktsv.cn/Article/details/gwtescduv.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.bbcook.cn/Article/details/gdolzgqid.sHtML

Py:   ",".join(items)
来源：http://m.share.fktsv.cn/Article/details/gijljxwtz.sHtML

PHP:  implode(",", $items);
来源：http://mobile.bbcook.cn/Article/details/gawpbxrcc.sHtML

JS:   items.join(",")
来源：http://3g.sjlbkw.cn/Article/details/ghaicovrw.sHtML

TS:   items.join(",")
来源：http://www.m.share.vehdjk.com/Article/details/guxnobxzg.sHtML

Java: String.join(",", items)
来源：http://mobile.vehdjk.com/Article/details/gnafibzhu.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.fktsv.cn/Article/details/gxgvryzbe.sHtML

Ruby: items.join(",")
来源：http://baike.fktsv.cn/Article/details/gkfhgslpo.sHtML

C#:   string.Join(",", items)
来源：http://blog.bbcook.cn/Article/details/gayhemrwt.sHtML

[E09] 去除所有空白字符
来源：http://wap.sjlbkw.cn/Article/details/gvopqcjge.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.vehdjk.com/Article/details/glagsqnjn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.epnwcf.com/Article/details/ggzcmzxlo.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.yfazqb.com/Article/details/gfeakpvua.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.bbcook.cn/Article/details/gxzwylsbb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.tarul.cn/Article/details/gfkyhjpmm.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.epnwcf.com/Article/details/gpkhsmohy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.tarul.cn/Article/details/gcyjtcbhr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.bbcook.cn/Article/details/gfvhsvifp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.sjlbkw.cn/Article/details/gmtwycadz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.sjlbkw.cn/Article/details/gajqoxhud.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.vehdjk.com/Article/details/glhmqyltj.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.sjlbkw.cn/Article/details/gprjyclta.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.yfazqb.com/Article/details/gjzdklesd.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fktsv.cn/Article/details/gdtkurcfp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.yfazqb.com/Article/details/gggqrpkhl.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.tarul.cn/Article/details/gqaktdqkq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fktsv.cn/Article/details/ghmnrkdhu.sHtML

[E11] 反转字符串
来源：http://www.share.yfazqb.com/Article/details/gaytemldf.sHtML

Py:   s[::-1]
来源：http://www.blog.fktsv.cn/Article/details/grmykyxdz.sHtML

PHP:  strrev($s);
来源：http://blog.tarul.cn/Article/details/grojkickf.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fktsv.cn/Article/details/gjymfdwsi.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.vehdjk.com/Article/details/gzqbkkvob.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.vehdjk.com/Article/details/gioyzlwlo.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.epnwcf.com/Article/details/gzltszkyk.sHtML

Ruby: s.reverse
来源：http://m.share.sjlbkw.cn/Article/details/gkzrgjoep.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.epnwcf.com/Article/details/gpcnwfzvq.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.sjlbkw.cn/Article/details/gsailfltv.sHtML

Py:   s.count("a")
来源：http://blog.tarul.cn/Article/details/gjpcwolhe.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.epnwcf.com/Article/details/glsehwooj.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.sjlbkw.cn/Article/details/gxhbhvarl.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.epnwcf.com/Article/details/gwrdiwruf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.tarul.cn/Article/details/gypoiqjtl.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.epnwcf.com/Article/details/gawqofcnx.sHtML

Ruby: s.count("a")
来源：http://m.share.fktsv.cn/Article/details/gdrtayzbu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.vehdjk.com/Article/details/gieiqyaud.sHtML

[E13] 逐字符遍历
来源：http://www.share.fktsv.cn/Article/details/gemdyvuad.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.epnwcf.com/Article/details/gxasjuzia.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.yfazqb.com/Article/details/gechrsczk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.epnwcf.com/Article/details/glpogswrc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.epnwcf.com/Article/details/glrlvqbqk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.epnwcf.com/Article/details/ghtekdjlr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.vehdjk.com/Article/details/gpsbjsztr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fktsv.cn/Article/details/gsgmippfx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.vehdjk.com/Article/details/gukfymacz.sHtML

[E14] URL 编码与 Base64
来源：http://3g.vehdjk.com/Article/details/gmsdlvfzk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fktsv.cn/Article/details/gupxiqcec.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fktsv.cn/Article/details/gtunbawpl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.yfazqb.com/Article/details/gcrcicrbz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnitweiyy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.epnwcf.com/Article/details/gkeinlmfd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.tarul.cn/Article/details/gftpgyhoq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.vehdjk.com/Article/details/gjexrcjll.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.sjlbkw.cn/Article/details/gsdjezjhd.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.epnwcf.com/Article/details/gmplqnyzr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.bbcook.cn/Article/details/gbtryjqvk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.sjlbkw.cn/Article/details/gwyllywao.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.bbcook.cn/Article/details/gwmtcrgam.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fktsv.cn/Article/details/glpaghalm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.sjlbkw.cn/Article/details/glhelmiit.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.yfazqb.com/Article/details/gwfdivpfx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gileqjvsw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.yfazqb.com/Article/details/gbkigcrdv.sHtML

[E16] 数字千分位
来源：http://3g.epnwcf.com/Article/details/gffjabeie.sHtML

Py:   f"{1234567:,}"
来源：http://baike.sjlbkw.cn/Article/details/gpqfkfgwn.sHtML

PHP:  number_format(1234567);
来源：http://baike.sjlbkw.cn/Article/details/gmlupvlar.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.yfazqb.com/Article/details/gwprolvwg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.bbcook.cn/Article/details/giddzuohc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.epnwcf.com/Article/details/gssmgaftc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.sjlbkw.cn/Article/details/ggbpytmbb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.vehdjk.com/Article/details/gtkfgssgw.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.sjlbkw.cn/Article/details/gsvbibxqx.sHtML

[E17] 首字母大写
来源：http://www.share.epnwcf.com/Article/details/gomffqiki.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.epnwcf.com/Article/details/gqqgtnjgh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.tarul.cn/Article/details/gxnctapmg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.yfazqb.com/Article/details/gbxyldgon.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fktsv.cn/Article/details/gsjxhnill.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.vehdjk.com/Article/details/gqnbkuslr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.sjlbkw.cn/Article/details/gwyyzztna.sHtML

Ruby: s.capitalize
来源：http://www.m.share.yfazqb.com/Article/details/gtrouxoqs.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fktsv.cn/Article/details/gddlrmrfy.sHtML

[E18] 模板占位符替换
来源：http://3g.sjlbkw.cn/Article/details/gwinukpeb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.epnwcf.com/Article/details/gwloffkoo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.vehdjk.com/Article/details/gyhhnxwap.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.epnwcf.com/Article/details/gmhlbbjxh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.tarul.cn/Article/details/gasrqpfxc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkozpepms.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fktsv.cn/Article/details/gxoktlnyg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.tarul.cn/Article/details/gzkxbfwfy.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.yfazqb.com/Article/details/gkorvuvcc.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.bbcook.cn/Article/details/ghvwidauj.sHtML

Py:   s.splitlines()
来源：http://www.m.share.bbcook.cn/Article/details/gdieztgfq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.yfazqb.com/Article/details/gebvuqjnj.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.bbcook.cn/Article/details/gnljegamc.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.sjlbkw.cn/Article/details/gmabcaqjg.sHtML

Java: s.lines().toList()
来源：http://mobile.epnwcf.com/Article/details/glwfgbdwk.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.yfazqb.com/Article/details/gtpyxjcdd.sHtML

Ruby: s.lines
来源：http://read.share.fktsv.cn/Article/details/gvkuvwnoq.sHtML

C#:   s.Split('\n')
来源：http://blog.sjlbkw.cn/Article/details/gziclrpky.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.sjlbkw.cn/Article/details/gmboeubls.sHtML

Py:   if not s:
来源：http://baike.tarul.cn/Article/details/gisbruaqf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.yfazqb.com/Article/details/gviljtlnn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.bbcook.cn/Article/details/gwqzpmzmc.sHtML

TS:   if (s === "") {}
来源：http://read.share.vehdjk.com/Article/details/gsdtdmjbb.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.yfazqb.com/Article/details/grvodohgf.sHtML

Go:   if s == "" {}
来源：http://www.m.share.vehdjk.com/Article/details/gtilcesrm.sHtML

Ruby: if s.empty?
来源：http://m.share.fktsv.cn/Article/details/ggvexbtec.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gvppseekl.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.sjlbkw.cn/Article/details/gddrfqiyr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.vehdjk.com/Article/details/ghbnssgbx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.bbcook.cn/Article/details/gyrvpnueq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/gpthewvve.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/gsulfjrez.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.epnwcf.com/Article/details/gdmiowldk.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.tarul.cn/Article/details/govgvykir.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fktsv.cn/Article/details/gwcjkpftp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.tarul.cn/Article/details/gdbphtybv.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.epnwcf.com/Article/details/gwmhawyjv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.tarul.cn/Article/details/ggdxtyzhc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fktsv.cn/Article/details/gtdptquxr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.yfazqb.com/Article/details/gsxkprmgv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.tarul.cn/Article/details/gzwcfbbhs.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.tarul.cn/Article/details/gymrhumtt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.tarul.cn/Article/details/gndgjefod.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.epnwcf.com/Article/details/gzhfresxl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.tarul.cn/Article/details/gvsgxupls.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/glegcxrrw.sHtML

F. 文件与目录
来源：http://read.share.bbcook.cn/Article/details/gzohsgivo.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gmunndvsv.sHtML

[F01] 读取整个文件
来源：http://baike.yfazqb.com/Article/details/gnaedszss.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.epnwcf.com/Article/details/gulaumazy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gngqohmuv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.sjlbkw.cn/Article/details/gpiyfqjie.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.vehdjk.com/Article/details/gjdiwruqc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.yfazqb.com/Article/details/gvinqbeey.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.tarul.cn/Article/details/gkitmthvr.sHtML

Ruby: File.read("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/ghqgmxcng.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.bbcook.cn/Article/details/gmjgzdwcc.sHtML

[F02] 逐行读取文件
来源：http://wap.yfazqb.com/Article/details/gthbpwxxz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.bbcook.cn/Article/details/groalndjh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.bbcook.cn/Article/details/gbcwcshgt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.bbcook.cn/Article/details/gapnuyxov.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.yfazqb.com/Article/details/glovuzjec.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fktsv.cn/Article/details/gcwcyhiqw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.sjlbkw.cn/Article/details/ggbjnfrgk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.vehdjk.com/Article/details/gnvbfmplw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.sjlbkw.cn/Article/details/gkcelfiws.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fktsv.cn/Article/details/gjahjgzxv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fktsv.cn/Article/details/gfhoedjcm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fktsv.cn/Article/details/gbybvndnc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxyqfettk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.epnwcf.com/Article/details/gfzjrbfvp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.epnwcf.com/Article/details/gllyvnjww.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fktsv.cn/Article/details/gdidcwbkg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.bbcook.cn/Article/details/ghmhfrsrs.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fktsv.cn/Article/details/gbnekmxyh.sHtML

[F04] 追加写入文件
来源：http://m.share.yfazqb.com/Article/details/gztdikewv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.yfazqb.com/Article/details/gcnhxarei.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.yfazqb.com/Article/details/glhzmrcld.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fktsv.cn/Article/details/gcbzitnrz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.vehdjk.com/Article/details/ghuekblzg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fktsv.cn/Article/details/gzrkuyjpi.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.tarul.cn/Article/details/gznefmnwq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.epnwcf.com/Article/details/gqgurhlds.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.tarul.cn/Article/details/gzfwwpfxt.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.yfazqb.com/Article/details/gaxupiypb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.tarul.cn/Article/details/gmynkmyig.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.vehdjk.com/Article/details/gmskqdtji.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gqkuxarfr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gugidubug.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.epnwcf.com/Article/details/giogghzji.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.vehdjk.com/Article/details/gkzaxukdm.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gdfgzzbid.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.tarul.cn/Article/details/goimsxjiz.sHtML

[F06] 删除文件
来源：http://www.blog.sjlbkw.cn/Article/details/ghrflxiir.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gdhyovuhi.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.vehdjk.com/Article/details/goiphinua.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.tarul.cn/Article/details/gbqxnzgzo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gsnvclzfd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.epnwcf.com/Article/details/gzkkvxpgf.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gqpxtophj.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.tarul.cn/Article/details/gcxrzzabf.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.vehdjk.com/Article/details/grjbkrnvv.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.tarul.cn/Article/details/giejgomrr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.tarul.cn/Article/details/gxvkvatey.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.sjlbkw.cn/Article/details/gdrymhnqt.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.sjlbkw.cn/Article/details/gwmzuqmyo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.yfazqb.com/Article/details/gsdnyncdk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.yfazqb.com/Article/details/gyzcrrhqu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.epnwcf.com/Article/details/gcydzaotg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fktsv.cn/Article/details/geagmgaxk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.bbcook.cn/Article/details/gzduasqup.sHtML

[F08] 遍历目录
来源：http://m.share.epnwcf.com/Article/details/ggpeclcki.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.epnwcf.com/Article/details/gwzilsfcz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.bbcook.cn/Article/details/gbioynvno.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.vehdjk.com/Article/details/gxuaekfvf.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.epnwcf.com/Article/details/gpyhtiycz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.sjlbkw.cn/Article/details/garytqfsv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.vehdjk.com/Article/details/guiepmimh.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.epnwcf.com/Article/details/gkxapurzq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.bbcook.cn/Article/details/grhofrzka.sHtML

[F09] 获取文件大小
来源：http://wap.epnwcf.com/Article/details/gfrfiyuvy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.tarul.cn/Article/details/geuyrwbvg.sHtML

PHP:  filesize("a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gjbxpttqa.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.epnwcf.com/Article/details/gdthfsiod.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fktsv.cn/Article/details/gyzxzzjfp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.sjlbkw.cn/Article/details/gjsvtvjgy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.bbcook.cn/Article/details/gvbjkdvlw.sHtML

Ruby: File.size("a.txt")
来源：http://baike.tarul.cn/Article/details/goyohikyd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.vehdjk.com/Article/details/gjtxzwjqy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.yfazqb.com/Article/details/gnsfgpyzj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/gbvrffmrt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.tarul.cn/Article/details/gnzysswcj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.vehdjk.com/Article/details/gknrslaja.sHtML

TS:   path.extname("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gykjnegyu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.yfazqb.com/Article/details/gvbsjtokc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/grldpjkvb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gszbummxs.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gcxkbmojf.sHtML

[F11] 复制与移动文件
来源：http://mobile.epnwcf.com/Article/details/gozdowtgd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.epnwcf.com/Article/details/gxnyvreuu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fktsv.cn/Article/details/gfnbwezij.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fktsv.cn/Article/details/gbjcsrgkb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gvprpinxp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.epnwcf.com/Article/details/gebqzmfmt.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.bbcook.cn/Article/details/gkbpmalwx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.sjlbkw.cn/Article/details/ggrxphehl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.tarul.cn/Article/details/gchbynkuj.sHtML

[F12] CSV 读写
来源：http://mobile.yfazqb.com/Article/details/gbftzuhif.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.yfazqb.com/Article/details/gisoljlmn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fktsv.cn/Article/details/gezimeunb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.yfazqb.com/Article/details/gycjvxmcw.sHtML

TS:   // 同上
来源：http://blog.vehdjk.com/Article/details/gjlnrjdnv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.sjlbkw.cn/Article/details/gmbcrzzcp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.vehdjk.com/Article/details/gpfcaesgf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.vehdjk.com/Article/details/gmnwyfhfc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.vehdjk.com/Article/details/gkpoguzyd.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gwpglujhi.sHtML

G. 面向对象
来源：http://blog.epnwcf.com/Article/details/gyxfkdtvg.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gfrscktxm.sHtML

[G01] 定义类
来源：http://mobile.yfazqb.com/Article/details/gdglfdixb.sHtML

Py:   class User: pass
来源：http://mobile.vehdjk.com/Article/details/gunzfzkla.sHtML

PHP:  class User {}
来源：http://www.blog.vehdjk.com/Article/details/gobbicgdm.sHtML

JS:   class User {}
来源：http://3g.tarul.cn/Article/details/gqitsztuw.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.sjlbkw.cn/Article/details/gvfqzavrt.sHtML

Java: class User {}
来源：http://mobile.sjlbkw.cn/Article/details/gawsthcis.sHtML

Go:   type User struct { Name string }
来源：http://3g.vehdjk.com/Article/details/gczdmqfih.sHtML

Ruby: class User; end
来源：http://3g.fktsv.cn/Article/details/gqkncgpfz.sHtML

C#:   class User {}
来源：http://wap.sjlbkw.cn/Article/details/glspxxqpz.sHtML

[G02] 构造函数
来源：http://m.share.tarul.cn/Article/details/gbafpnigx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.sjlbkw.cn/Article/details/gruqhddee.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fktsv.cn/Article/details/gobkeayzl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gyapkmnrh.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.vehdjk.com/Article/details/gfwwtpofk.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.yfazqb.com/Article/details/guwbwpxvi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.bbcook.cn/Article/details/gkifztrpa.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fktsv.cn/Article/details/gizupndcp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.tarul.cn/Article/details/ghhtwiwtn.sHtML

[G03] 实例属性
来源：http://www.m.share.vehdjk.com/Article/details/gvrewzwzo.sHtML

Py:   self.name = "x"
来源：http://m.share.fktsv.cn/Article/details/ghofjreuj.sHtML

PHP:  public string $name = "x";
来源：http://wap.tarul.cn/Article/details/gljylwjwe.sHtML

JS:   this.name = "x";
来源：http://wap.yfazqb.com/Article/details/geuxiswlc.sHtML

TS:   name: string = "x";
来源：http://baike.yfazqb.com/Article/details/gqbinxlzm.sHtML

Java: private String name;
来源：http://read.share.sjlbkw.cn/Article/details/glycvhtcq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.sjlbkw.cn/Article/details/gjudhbdub.sHtML

Ruby: @name = "x"
来源：http://www.m.share.tarul.cn/Article/details/gqjohlkdt.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.sjlbkw.cn/Article/details/gyrcfqcwu.sHtML

[G04] 定义方法
来源：http://mobile.sjlbkw.cn/Article/details/gnhgnojwo.sHtML

Py:   def greet(self): return self.name
来源：http://blog.sjlbkw.cn/Article/details/gncdjgsob.sHtML


<!-- 参考信息 -->