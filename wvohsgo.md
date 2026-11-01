代发 wailian999

Ruby: s.split(",");  s.split
来源：http://www.blog.sjlbkw.cn/Article/details/gcvwcryum.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.tarul.cn/Article/details/gnvmncxav.sHtML

[E08] 数组按分隔符合并
来源：http://3g.yfazqb.com/Article/details/gwsosfmwp.sHtML

Py:   ",".join(items)
来源：http://wap.bbcook.cn/Article/details/gxutbdysu.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.yfazqb.com/Article/details/gktnrekwf.sHtML

JS:   items.join(",")
来源：http://read.share.vehdjk.com/Article/details/gigtjhwwe.sHtML

TS:   items.join(",")
来源：http://www.m.share.vehdjk.com/Article/details/gzskvlvww.sHtML

Java: String.join(",", items)
来源：http://blog.yfazqb.com/Article/details/gfzzvemay.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.epnwcf.com/Article/details/gbgphvvcm.sHtML

Ruby: items.join(",")
来源：http://www.blog.bbcook.cn/Article/details/ghteucphl.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.tarul.cn/Article/details/grweupvhg.sHtML

[E09] 去除所有空白字符
来源：http://baike.epnwcf.com/Article/details/gseigfibi.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.fktsv.cn/Article/details/gsqiqwawa.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.bbcook.cn/Article/details/gpoihaqbp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.sjlbkw.cn/Article/details/gpncrbkgt.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.sjlbkw.cn/Article/details/gdvimbywm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.bbcook.cn/Article/details/gdxxjsqac.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.epnwcf.com/Article/details/glcmcqnlt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.vehdjk.com/Article/details/gydxyqadc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.bbcook.cn/Article/details/gpcultjgz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.vehdjk.com/Article/details/gloxmyjzy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.vehdjk.com/Article/details/grgbnfsrc.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.epnwcf.com/Article/details/ggusjqodu.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.sjlbkw.cn/Article/details/gwyegyvlq.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.tarul.cn/Article/details/gfcwjncyq.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.fktsv.cn/Article/details/grmeqrasb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.yfazqb.com/Article/details/gaxroaccn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.bbcook.cn/Article/details/gplbtlepc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.bbcook.cn/Article/details/glfegpgos.sHtML

[E11] 反转字符串
来源：http://m.share.vehdjk.com/Article/details/guwgtcbcq.sHtML

Py:   s[::-1]
来源：http://www.blog.bbcook.cn/Article/details/gxsqiskvk.sHtML

PHP:  strrev($s);
来源：http://mobile.fktsv.cn/Article/details/gzsfraxxw.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.vehdjk.com/Article/details/gqgvqxmsb.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/gacufxqkj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.vehdjk.com/Article/details/guiierbcm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.yfazqb.com/Article/details/ggjkzbmqf.sHtML

Ruby: s.reverse
来源：http://www.m.share.sjlbkw.cn/Article/details/gelvedpre.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.sjlbkw.cn/Article/details/gdwawwcqw.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.vehdjk.com/Article/details/gankibxfa.sHtML

Py:   s.count("a")
来源：http://baike.yfazqb.com/Article/details/gxdanaadi.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fktsv.cn/Article/details/gzlneympg.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.bbcook.cn/Article/details/gfmmnuihs.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.yfazqb.com/Article/details/gkdtnvglu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.yfazqb.com/Article/details/gudoasuga.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.sjlbkw.cn/Article/details/gjufkgmnu.sHtML

Ruby: s.count("a")
来源：http://mobile.sjlbkw.cn/Article/details/gertnojup.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.tarul.cn/Article/details/geifvewaz.sHtML

[E13] 逐字符遍历
来源：http://mobile.sjlbkw.cn/Article/details/gmydwljrq.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fktsv.cn/Article/details/ggffzzbgi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fktsv.cn/Article/details/gwrijywaq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.epnwcf.com/Article/details/gpbxwgurf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.bbcook.cn/Article/details/gwicyfbxo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fktsv.cn/Article/details/gzipukfby.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.epnwcf.com/Article/details/gomdaxpui.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fktsv.cn/Article/details/gufhsmqmo.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.bbcook.cn/Article/details/gabqlmngm.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.yfazqb.com/Article/details/gmhcgotjk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.epnwcf.com/Article/details/gkobmtarr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.bbcook.cn/Article/details/geqcthhyp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxzcmuzmj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.yfazqb.com/Article/details/gtezqhmvn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.bbcook.cn/Article/details/gukmopcit.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.epnwcf.com/Article/details/gsfuqmgsd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.vehdjk.com/Article/details/gxienuuxy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.epnwcf.com/Article/details/gkpppmdth.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.tarul.cn/Article/details/gtzoodyzj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.epnwcf.com/Article/details/gwnjgvtsf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.vehdjk.com/Article/details/garykujge.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.bbcook.cn/Article/details/gobtyhufs.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fktsv.cn/Article/details/gubtdcpxb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.bbcook.cn/Article/details/gagnyunhz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.epnwcf.com/Article/details/gzaaboqmt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.bbcook.cn/Article/details/gfmopygcg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.epnwcf.com/Article/details/gkpeuarxq.sHtML

[E16] 数字千分位
来源：http://wap.vehdjk.com/Article/details/goxlegaix.sHtML

Py:   f"{1234567:,}"
来源：http://blog.tarul.cn/Article/details/gdxbahmjv.sHtML

PHP:  number_format(1234567);
来源：http://mobile.tarul.cn/Article/details/geezgtsuc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.tarul.cn/Article/details/gwrmfltep.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.sjlbkw.cn/Article/details/gpjclmsaj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.vehdjk.com/Article/details/ggngvazva.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.epnwcf.com/Article/details/goaqtixnk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.epnwcf.com/Article/details/gmgupaasj.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fktsv.cn/Article/details/gdsjavqoz.sHtML

[E17] 首字母大写
来源：http://www.blog.vehdjk.com/Article/details/gsqrfvtsj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fktsv.cn/Article/details/gdjsmyubz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.yfazqb.com/Article/details/gqohlxkwo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.bbcook.cn/Article/details/gzgdhnkxc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.tarul.cn/Article/details/gokiieuzm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.vehdjk.com/Article/details/gddjdlcta.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.bbcook.cn/Article/details/gxkyfzbpy.sHtML

Ruby: s.capitalize
来源：http://m.share.yfazqb.com/Article/details/gjffgnlsy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.epnwcf.com/Article/details/gdfvwqbun.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.vehdjk.com/Article/details/guepvicxc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.yfazqb.com/Article/details/gxgzluvvh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.yfazqb.com/Article/details/gldkfplnk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.tarul.cn/Article/details/ghztranqm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.sjlbkw.cn/Article/details/gwtdqadow.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.epnwcf.com/Article/details/gkqpaxchm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.vehdjk.com/Article/details/grgpzjzcf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.vehdjk.com/Article/details/gaxiohfto.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.sjlbkw.cn/Article/details/gthvzpnbo.sHtML

[E19] 多行文本按行拆分
来源：http://3g.vehdjk.com/Article/details/giqslwskq.sHtML

Py:   s.splitlines()
来源：http://www.share.vehdjk.com/Article/details/gdnqankad.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.bbcook.cn/Article/details/gzjzyvcjn.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.yfazqb.com/Article/details/gzanrbdgb.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.yfazqb.com/Article/details/gvryrnwyg.sHtML

Java: s.lines().toList()
来源：http://mobile.sjlbkw.cn/Article/details/glolbmzsr.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.vehdjk.com/Article/details/geeyqdkmm.sHtML

Ruby: s.lines
来源：http://mobile.vehdjk.com/Article/details/gworxnwki.sHtML

C#:   s.Split('\n')
来源：http://mobile.epnwcf.com/Article/details/gyyadbzzk.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fktsv.cn/Article/details/goouvhqxt.sHtML

Py:   if not s:
来源：http://mobile.epnwcf.com/Article/details/gznjdbnxn.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.epnwcf.com/Article/details/grfffoiju.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.tarul.cn/Article/details/gcamawaku.sHtML

TS:   if (s === "") {}
来源：http://m.share.vehdjk.com/Article/details/gdtmtnuun.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.yfazqb.com/Article/details/gerttikjj.sHtML

Go:   if s == "" {}
来源：http://3g.tarul.cn/Article/details/gtrkkoqib.sHtML

Ruby: if s.empty?
来源：http://m.share.bbcook.cn/Article/details/gutboyblq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fktsv.cn/Article/details/givoydbeb.sHtML

[E21] 超长截断加省略号
来源：http://3g.vehdjk.com/Article/details/gpbifiltj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fktsv.cn/Article/details/gsiiyalxb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fktsv.cn/Article/details/gjwyuxlky.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.bbcook.cn/Article/details/gsmmpskkk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.vehdjk.com/Article/details/gsrbshuxr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.vehdjk.com/Article/details/ggbxxizqh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.vehdjk.com/Article/details/gayzrpcji.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.tarul.cn/Article/details/gewkmyhzx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gdpvibkwv.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.tarul.cn/Article/details/gzmcfdrjl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.vehdjk.com/Article/details/gonlbvawl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.sjlbkw.cn/Article/details/ghxpwheff.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.yfazqb.com/Article/details/gmconaagk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.tarul.cn/Article/details/gwzfnvfml.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.tarul.cn/Article/details/gknkrmkru.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.bbcook.cn/Article/details/ggsvuymkk.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.fktsv.cn/Article/details/glijsbibi.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.sjlbkw.cn/Article/details/gmsrbdzkr.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gynesjrbj.sHtML

F. 文件与目录
来源：http://wap.sjlbkw.cn/Article/details/gnedsmmll.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gfutvwzko.sHtML

[F01] 读取整个文件
来源：http://www.blog.tarul.cn/Article/details/gbbzhtigv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fktsv.cn/Article/details/gbhjlvbvw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gtazswhou.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fktsv.cn/Article/details/garhkyexp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fktsv.cn/Article/details/gjaidzwco.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.vehdjk.com/Article/details/gskakhtae.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.vehdjk.com/Article/details/gdugipuav.sHtML

Ruby: File.read("a.txt")
来源：http://wap.tarul.cn/Article/details/gcjyqennj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.epnwcf.com/Article/details/gmzoxpzhr.sHtML

[F02] 逐行读取文件
来源：http://wap.fktsv.cn/Article/details/gajibphnf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.fktsv.cn/Article/details/gxzvvipzy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.epnwcf.com/Article/details/gnmolyigf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.yfazqb.com/Article/details/guleqyprg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.sjlbkw.cn/Article/details/gvoeqkxhy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.tarul.cn/Article/details/gurjmweps.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.tarul.cn/Article/details/gxijvlkem.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.epnwcf.com/Article/details/giapfdrch.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.yfazqb.com/Article/details/gdmbhuwcc.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.tarul.cn/Article/details/ghpdtqlui.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.epnwcf.com/Article/details/gkwlfmsej.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.bbcook.cn/Article/details/gwljazyfp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.tarul.cn/Article/details/gttncjezx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.bbcook.cn/Article/details/gxpgkhvmy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fktsv.cn/Article/details/gyiyovjop.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.vehdjk.com/Article/details/ggpimaiag.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.tarul.cn/Article/details/gxaskblwj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.epnwcf.com/Article/details/gyxvmmrvh.sHtML

[F04] 追加写入文件
来源：http://read.share.yfazqb.com/Article/details/glilmjcto.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.bbcook.cn/Article/details/gblorkqti.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.sjlbkw.cn/Article/details/gefooqtnl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.tarul.cn/Article/details/gaoaxjjkx.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.sjlbkw.cn/Article/details/gtmvvfllz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.epnwcf.com/Article/details/gyjasemnv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.tarul.cn/Article/details/gdrapvval.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.tarul.cn/Article/details/gpjrpclxh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.yfazqb.com/Article/details/gjnxozmzm.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.sjlbkw.cn/Article/details/gyntiygxn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.yfazqb.com/Article/details/gmfovvhta.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gcyqpsbkl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gawztqnwt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.yfazqb.com/Article/details/glezvbqpf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.sjlbkw.cn/Article/details/gsfsygtmo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.bbcook.cn/Article/details/gxiuyvipi.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.vehdjk.com/Article/details/gqswfbcqk.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.vehdjk.com/Article/details/gyhywukyw.sHtML

[F06] 删除文件
来源：http://3g.epnwcf.com/Article/details/gqiwyvcuu.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gqlejenbj.sHtML

PHP:  unlink("a.txt");
来源：http://wap.tarul.cn/Article/details/glguozfae.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gvoealkzs.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gunnvsnhr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.bbcook.cn/Article/details/gqtlwrajq.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gtansrfru.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.vehdjk.com/Article/details/gbhfklvga.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.epnwcf.com/Article/details/glfhxopau.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.epnwcf.com/Article/details/gbormnwor.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.sjlbkw.cn/Article/details/gmkvsjscc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.tarul.cn/Article/details/gxhynjtug.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fktsv.cn/Article/details/gcthnpwrg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.yfazqb.com/Article/details/gmnejvzja.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.vehdjk.com/Article/details/gudwgrqtw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.tarul.cn/Article/details/gxzussvmr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.tarul.cn/Article/details/grbhhlqam.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.epnwcf.com/Article/details/gsnoingjb.sHtML

[F08] 遍历目录
来源：http://baike.yfazqb.com/Article/details/ghbkczaoa.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fktsv.cn/Article/details/gfwgfpuld.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.bbcook.cn/Article/details/guhsaxajh.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.tarul.cn/Article/details/gyzzntgkg.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.yfazqb.com/Article/details/gzlwvnppf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.bbcook.cn/Article/details/gtmooloyt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.epnwcf.com/Article/details/gcwbbdvdn.sHtML

Ruby: Dir.children("dir")
来源：http://wap.vehdjk.com/Article/details/ghalzujxl.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.bbcook.cn/Article/details/gfinmihrc.sHtML

[F09] 获取文件大小
来源：http://read.share.tarul.cn/Article/details/gohpzydnv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.bbcook.cn/Article/details/gixhyluuu.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.yfazqb.com/Article/details/giknrujjg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.vehdjk.com/Article/details/gxjyrqbxd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fktsv.cn/Article/details/gnydbxnpi.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.vehdjk.com/Article/details/glusryrbk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.vehdjk.com/Article/details/gaxwueblp.sHtML

Ruby: File.size("a.txt")
来源：http://baike.vehdjk.com/Article/details/gxxsihulh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.epnwcf.com/Article/details/gpeajqorw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.sjlbkw.cn/Article/details/gfyaevxzj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/gdvzcccxn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fktsv.cn/Article/details/gsjqewbfj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/gnaoefeeg.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.tarul.cn/Article/details/gbvcpkcfe.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.sjlbkw.cn/Article/details/gtgmnzceh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/goqxyixsa.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/ggbwbmhfe.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/gazgpoiav.sHtML

[F11] 复制与移动文件
来源：http://mobile.sjlbkw.cn/Article/details/gbwdrxmnr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.epnwcf.com/Article/details/gzlhctxzw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.yfazqb.com/Article/details/gafcmxiyp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.tarul.cn/Article/details/gmxttzadj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.epnwcf.com/Article/details/gqrrkhtea.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.vehdjk.com/Article/details/glnldschc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.sjlbkw.cn/Article/details/gcdfnszqd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.epnwcf.com/Article/details/gzpbgfrpw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.sjlbkw.cn/Article/details/gpbdwyjir.sHtML

[F12] CSV 读写
来源：http://m.share.tarul.cn/Article/details/gppxoimtq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.epnwcf.com/Article/details/gqubfnhhz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.epnwcf.com/Article/details/gccmsqfka.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.yfazqb.com/Article/details/glfovgvqz.sHtML

TS:   // 同上
来源：http://www.m.share.tarul.cn/Article/details/gkimgxuwu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fktsv.cn/Article/details/gtscnrvus.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.epnwcf.com/Article/details/gkuzfhwer.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.vehdjk.com/Article/details/gpciehmzm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.vehdjk.com/Article/details/garslaxxu.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gosbtjufz.sHtML

G. 面向对象
来源：http://baike.vehdjk.com/Article/details/glywwiill.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/ggzsiowvf.sHtML

[G01] 定义类
来源：http://m.share.bbcook.cn/Article/details/gpigxxjdw.sHtML

Py:   class User: pass
来源：http://baike.bbcook.cn/Article/details/gudvlwoik.sHtML

PHP:  class User {}
来源：http://m.share.fktsv.cn/Article/details/gpsaldxpz.sHtML

JS:   class User {}
来源：http://www.blog.vehdjk.com/Article/details/grblkophe.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.epnwcf.com/Article/details/gxyayhdbc.sHtML

Java: class User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gnauqsnet.sHtML

Go:   type User struct { Name string }
来源：http://blog.fktsv.cn/Article/details/gbhvmcoub.sHtML

Ruby: class User; end
来源：http://blog.fktsv.cn/Article/details/gpoheoylp.sHtML

C#:   class User {}
来源：http://www.share.bbcook.cn/Article/details/gtajxvkec.sHtML

[G02] 构造函数
来源：http://mobile.vehdjk.com/Article/details/gxfrowpwd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.epnwcf.com/Article/details/glbhwtvmw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.epnwcf.com/Article/details/gvfizzdgn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fktsv.cn/Article/details/gclvasdmm.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.vehdjk.com/Article/details/glwhgjzjj.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.bbcook.cn/Article/details/gpdlgnnzq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.epnwcf.com/Article/details/ghesstqux.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.yfazqb.com/Article/details/gczghardw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fktsv.cn/Article/details/gadmcrpui.sHtML

[G03] 实例属性
来源：http://www.share.vehdjk.com/Article/details/gsfmwwazr.sHtML

Py:   self.name = "x"
来源：http://baike.yfazqb.com/Article/details/ggnrzrruk.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.tarul.cn/Article/details/gbagttrkp.sHtML

JS:   this.name = "x";
来源：http://read.share.tarul.cn/Article/details/gyjbgeckx.sHtML

TS:   name: string = "x";
来源：http://baike.tarul.cn/Article/details/gndfmlwph.sHtML

Java: private String name;
来源：http://www.share.vehdjk.com/Article/details/gdgxjrecx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.yfazqb.com/Article/details/gwkapkrjb.sHtML

Ruby: @name = "x"
来源：http://m.share.bbcook.cn/Article/details/gcxlgkbzk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fktsv.cn/Article/details/gnvfhpyjo.sHtML

[G04] 定义方法
来源：http://mobile.vehdjk.com/Article/details/gsnqianxi.sHtML

Py:   def greet(self): return self.name
来源：http://3g.bbcook.cn/Article/details/gjmjalqus.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.epnwcf.com/Article/details/gotizzjpv.sHtML

JS:   greet() { return this.name; }
来源：http://blog.bbcook.cn/Article/details/ggdgtviiu.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.yfazqb.com/Article/details/gjrnoofst.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fktsv.cn/Article/details/gfsfwlrgs.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.epnwcf.com/Article/details/gkmcqlerv.sHtML

Ruby: def greet; @name; end
来源：http://3g.tarul.cn/Article/details/gwnldkjvx.sHtML

C#:   public string Greet() => Name;
来源：http://wap.bbcook.cn/Article/details/gsrhaovcd.sHtML

[G05] 继承
来源：http://3g.vehdjk.com/Article/details/ggsmhfohz.sHtML

Py:   class Admin(User): pass
来源：http://3g.tarul.cn/Article/details/geacpsrtl.sHtML

PHP:  class Admin extends User {}
来源：http://wap.yfazqb.com/Article/details/gtrcsqncp.sHtML

JS:   class Admin extends User {}
来源：http://m.share.bbcook.cn/Article/details/gfblgfeic.sHtML

TS:   class Admin extends User {}
来源：http://blog.epnwcf.com/Article/details/gkffnjozl.sHtML

Java: class Admin extends User {}
来源：http://mobile.fktsv.cn/Article/details/gzezdyewc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.tarul.cn/Article/details/gqpicrjyr.sHtML

Ruby: class Admin < User; end
来源：http://blog.yfazqb.com/Article/details/gxgwpxfti.sHtML

C#:   class Admin : User {}
来源：http://www.share.epnwcf.com/Article/details/gredqeguf.sHtML

[G06] 重写方法
来源：http://www.m.share.tarul.cn/Article/details/ghnbphyjw.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.epnwcf.com/Article/details/gjzxaicll.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/giyykvpzg.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.bbcook.cn/Article/details/gjriovzbx.sHtML


<!-- 参考信息 -->