代发 wailian999

C#:   s.Replace("a", "b")
来源：http://mobile.tarul.cn/Article/details/gpamcbkda.sHtML

[E07] 按分隔符拆分
来源：http://wap.sjlbkw.cn/Article/details/gzawgqrgf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.tarul.cn/Article/details/gtkactcph.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.epnwcf.com/Article/details/gqaniucnz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.epnwcf.com/Article/details/gguxwvsfo.sHtML

TS:   s.split(",")
来源：http://www.share.vehdjk.com/Article/details/gqhgwcnts.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.bbcook.cn/Article/details/ghxlddnvm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.yfazqb.com/Article/details/gsncboewa.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.tarul.cn/Article/details/gjxmjlhws.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.epnwcf.com/Article/details/gpmyanhwe.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fktsv.cn/Article/details/gbhksxbxv.sHtML

Py:   ",".join(items)
来源：http://www.blog.yfazqb.com/Article/details/gypmlqmbz.sHtML

PHP:  implode(",", $items);
来源：http://wap.bbcook.cn/Article/details/ghtaaxbyf.sHtML

JS:   items.join(",")
来源：http://read.share.bbcook.cn/Article/details/gispfhfjm.sHtML

TS:   items.join(",")
来源：http://read.share.epnwcf.com/Article/details/gubvlaoyw.sHtML

Java: String.join(",", items)
来源：http://www.m.share.sjlbkw.cn/Article/details/giknnbjkm.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.tarul.cn/Article/details/guxlzympg.sHtML

Ruby: items.join(",")
来源：http://www.share.sjlbkw.cn/Article/details/guisaasmb.sHtML

C#:   string.Join(",", items)
来源：http://read.share.tarul.cn/Article/details/gurtobpfp.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.bbcook.cn/Article/details/gmbytipvo.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.yfazqb.com/Article/details/gesezavox.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.yfazqb.com/Article/details/gjeyxqwqs.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.vehdjk.com/Article/details/gjtyjwqzx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.yfazqb.com/Article/details/guwzbmevu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.tarul.cn/Article/details/goesfbjxt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.sjlbkw.cn/Article/details/gylzvawgt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.yfazqb.com/Article/details/gcrrtrazn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.fktsv.cn/Article/details/gfdqnbwro.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.epnwcf.com/Article/details/gycdxtcup.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.epnwcf.com/Article/details/gjhodduxn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.tarul.cn/Article/details/ghmqskcve.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.sjlbkw.cn/Article/details/ggzlbarkl.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.epnwcf.com/Article/details/gdvkeplnq.sHtML

Java: String.format("%03d", 7)
来源：http://blog.vehdjk.com/Article/details/gohiovotg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.bbcook.cn/Article/details/ghifcedkx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.epnwcf.com/Article/details/gwaysykjw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fktsv.cn/Article/details/gzggjsnry.sHtML

[E11] 反转字符串
来源：http://3g.epnwcf.com/Article/details/gbbldmfxo.sHtML

Py:   s[::-1]
来源：http://3g.sjlbkw.cn/Article/details/gewnzevif.sHtML

PHP:  strrev($s);
来源：http://m.share.yfazqb.com/Article/details/gpejnupdr.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.epnwcf.com/Article/details/gvdbygdeh.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.yfazqb.com/Article/details/gdipployk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.tarul.cn/Article/details/ghejhhjxq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.sjlbkw.cn/Article/details/grpqlvdrf.sHtML

Ruby: s.reverse
来源：http://www.share.sjlbkw.cn/Article/details/gdtylnzhx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.yfazqb.com/Article/details/gwdpvvols.sHtML

[E12] 统计某字符出现次数
来源：http://blog.epnwcf.com/Article/details/gxxpyqlfl.sHtML

Py:   s.count("a")
来源：http://www.m.share.fktsv.cn/Article/details/ggatcrhqp.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.fktsv.cn/Article/details/gipmqbdgk.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fktsv.cn/Article/details/glrlizdtn.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.bbcook.cn/Article/details/guzigjvhk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.bbcook.cn/Article/details/grxddjwbm.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.vehdjk.com/Article/details/gzlgjmjac.sHtML

Ruby: s.count("a")
来源：http://read.share.vehdjk.com/Article/details/gjvaslhem.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.sjlbkw.cn/Article/details/gutonievy.sHtML

[E13] 逐字符遍历
来源：http://www.share.epnwcf.com/Article/details/gbtdejtoh.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.tarul.cn/Article/details/gzeplrskv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.vehdjk.com/Article/details/goqsgxgrh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.bbcook.cn/Article/details/gizzjtafm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fktsv.cn/Article/details/giwcsilyl.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/gdhscedau.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.yfazqb.com/Article/details/gfhhbluvo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.bbcook.cn/Article/details/godjzfepa.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.yfazqb.com/Article/details/grwwiqaxq.sHtML

[E14] URL 编码与 Base64
来源：http://blog.epnwcf.com/Article/details/gxlduywxu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.yfazqb.com/Article/details/gypwvkfhp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fktsv.cn/Article/details/ghoouapcb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.epnwcf.com/Article/details/gldkfdles.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.sjlbkw.cn/Article/details/gxpfhelia.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.tarul.cn/Article/details/gtunlrgyy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.tarul.cn/Article/details/gqjylydmd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.tarul.cn/Article/details/grputspdw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.epnwcf.com/Article/details/ghmcbbebp.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fktsv.cn/Article/details/gwjwgrriq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.bbcook.cn/Article/details/gomikmoqn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.sjlbkw.cn/Article/details/gcmmglmpp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/grmtyonxs.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fktsv.cn/Article/details/gtgaekdzo.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.sjlbkw.cn/Article/details/gfwwemqrq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.tarul.cn/Article/details/gxngigycy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.yfazqb.com/Article/details/gcnayjsqe.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.sjlbkw.cn/Article/details/gdjinnlba.sHtML

[E16] 数字千分位
来源：http://mobile.tarul.cn/Article/details/guxpugbbz.sHtML

Py:   f"{1234567:,}"
来源：http://wap.tarul.cn/Article/details/gdxgqbdnb.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.epnwcf.com/Article/details/ghgnzizha.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.epnwcf.com/Article/details/gpcfvjzme.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.tarul.cn/Article/details/gsfmlezbh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fktsv.cn/Article/details/gjhreasnb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.fktsv.cn/Article/details/gwsyzxgtg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.sjlbkw.cn/Article/details/gyjkytvar.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.tarul.cn/Article/details/gsxombisc.sHtML

[E17] 首字母大写
来源：http://read.share.bbcook.cn/Article/details/gatdpdtlt.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.vehdjk.com/Article/details/gccxhxxjh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.yfazqb.com/Article/details/gmuugwlgk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.bbcook.cn/Article/details/guotuekyz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.tarul.cn/Article/details/gddsoiltd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fktsv.cn/Article/details/gqgjekhob.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.tarul.cn/Article/details/gobvzymka.sHtML

Ruby: s.capitalize
来源：http://www.share.fktsv.cn/Article/details/gthkvkmem.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.bbcook.cn/Article/details/gkhgiyhps.sHtML

[E18] 模板占位符替换
来源：http://wap.vehdjk.com/Article/details/guptxmplm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fktsv.cn/Article/details/ghbjbgrjc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fktsv.cn/Article/details/gesmezzap.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.tarul.cn/Article/details/gfpndbitf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.yfazqb.com/Article/details/govdyetxs.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.vehdjk.com/Article/details/glzvhshgs.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.bbcook.cn/Article/details/gshrirwmm.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.bbcook.cn/Article/details/gmhnaknxf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.epnwcf.com/Article/details/gwesakdqx.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.yfazqb.com/Article/details/gieauvrmf.sHtML

Py:   s.splitlines()
来源：http://3g.sjlbkw.cn/Article/details/gzelcgkiv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.epnwcf.com/Article/details/gfwyyimqy.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.tarul.cn/Article/details/gluphzgur.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fktsv.cn/Article/details/gzkelwqtg.sHtML

Java: s.lines().toList()
来源：http://blog.tarul.cn/Article/details/gdbckfahm.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.bbcook.cn/Article/details/gmhyjijho.sHtML

Ruby: s.lines
来源：http://www.blog.epnwcf.com/Article/details/gonnflusa.sHtML

C#:   s.Split('\n')
来源：http://mobile.yfazqb.com/Article/details/gttsaotqr.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.bbcook.cn/Article/details/gzkhdefgv.sHtML

Py:   if not s:
来源：http://read.share.vehdjk.com/Article/details/gyxckwiec.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.tarul.cn/Article/details/gjrtmvfpf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fktsv.cn/Article/details/gnstflxpj.sHtML

TS:   if (s === "") {}
来源：http://3g.tarul.cn/Article/details/ggkserawr.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.vehdjk.com/Article/details/gkstymlwa.sHtML

Go:   if s == "" {}
来源：http://m.share.tarul.cn/Article/details/gzyrseulw.sHtML

Ruby: if s.empty?
来源：http://mobile.yfazqb.com/Article/details/gipeepebj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.sjlbkw.cn/Article/details/gnsdunokd.sHtML

[E21] 超长截断加省略号
来源：http://read.share.tarul.cn/Article/details/gexpxvhlm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.bbcook.cn/Article/details/goorfwrmg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.vehdjk.com/Article/details/guvifmylc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/gauwatmzx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.epnwcf.com/Article/details/gjeyhvsmg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fktsv.cn/Article/details/gjomemgor.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.bbcook.cn/Article/details/glyntdjry.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.fktsv.cn/Article/details/ggmcvmenw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.tarul.cn/Article/details/gxkfcxoog.sHtML

[E22] 字节长度与字符长度
来源：http://baike.epnwcf.com/Article/details/gxcszjrwu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.vehdjk.com/Article/details/grkbvgpim.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.epnwcf.com/Article/details/gnvsordpy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.tarul.cn/Article/details/gdltfojgz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.tarul.cn/Article/details/gqbuezywh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.vehdjk.com/Article/details/goaqmgaco.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.tarul.cn/Article/details/gbtzvkbte.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.tarul.cn/Article/details/ggrmcuyni.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.tarul.cn/Article/details/gewnjwhjr.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/guvemcdxi.sHtML

F. 文件与目录
来源：http://www.blog.epnwcf.com/Article/details/gabzcupvg.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gexrektcw.sHtML

[F01] 读取整个文件
来源：http://www.m.share.tarul.cn/Article/details/gjmtsirhw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.yfazqb.com/Article/details/gfilhwgpb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fktsv.cn/Article/details/gfeifeaeb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.sjlbkw.cn/Article/details/gecvyxooa.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fktsv.cn/Article/details/ggfxkerbj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/gqpogcwsi.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.sjlbkw.cn/Article/details/gorjthxim.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gfmoehxba.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.vehdjk.com/Article/details/gabxryupz.sHtML

[F02] 逐行读取文件
来源：http://m.share.vehdjk.com/Article/details/ghfmaygqu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.epnwcf.com/Article/details/gwjdmlpyu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.yfazqb.com/Article/details/gdmfeegzl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.yfazqb.com/Article/details/gqghlvdxj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.vehdjk.com/Article/details/gpfdslgdk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.vehdjk.com/Article/details/gxqpuerax.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.bbcook.cn/Article/details/gguwopoej.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.bbcook.cn/Article/details/gssvndcbo.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.bbcook.cn/Article/details/gvwbnebcp.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.tarul.cn/Article/details/gawoeuqch.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.yfazqb.com/Article/details/ggundbwic.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.bbcook.cn/Article/details/gyteblydv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.tarul.cn/Article/details/gyxgkeaeb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fktsv.cn/Article/details/gbjfwjmza.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.vehdjk.com/Article/details/gctjejvcf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.sjlbkw.cn/Article/details/gxijzrltk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fktsv.cn/Article/details/gmmdqjune.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.epnwcf.com/Article/details/ghlhfsjrr.sHtML

[F04] 追加写入文件
来源：http://baike.bbcook.cn/Article/details/gqnydepbb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.yfazqb.com/Article/details/gotqypysm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fktsv.cn/Article/details/gdbqaabrr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fktsv.cn/Article/details/gguczwdzv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.epnwcf.com/Article/details/guqhthhgx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.vehdjk.com/Article/details/glsijhqhh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fktsv.cn/Article/details/gbulkzgfc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.tarul.cn/Article/details/gxwkyljaz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.yfazqb.com/Article/details/glzrlrwby.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.tarul.cn/Article/details/gsdkgcrtt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fktsv.cn/Article/details/gitywvleg.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.bbcook.cn/Article/details/glsqqgepu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gnrhfewyk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.bbcook.cn/Article/details/goqcpyskl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.bbcook.cn/Article/details/gvyofxpbi.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.vehdjk.com/Article/details/gqmhckopr.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gprszvqls.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.epnwcf.com/Article/details/gwsivkuyd.sHtML

[F06] 删除文件
来源：http://3g.yfazqb.com/Article/details/gfyefbbsd.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gjlsejcvk.sHtML

PHP:  unlink("a.txt");
来源：http://wap.vehdjk.com/Article/details/gjdivtbuf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gkubtkpsh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.tarul.cn/Article/details/gobcmznqs.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.tarul.cn/Article/details/grbasnprh.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gpkrppbgv.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.epnwcf.com/Article/details/gyrxdvcnc.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.bbcook.cn/Article/details/gqzlbjjzc.sHtML

[F07] 创建目录（含多级）
来源：http://blog.vehdjk.com/Article/details/gyxdnvsom.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.sjlbkw.cn/Article/details/goryokffl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.epnwcf.com/Article/details/gqghxlvpd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.epnwcf.com/Article/details/grkdigvrl.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.bbcook.cn/Article/details/gnexrdatz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.bbcook.cn/Article/details/gkdffcyiy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.vehdjk.com/Article/details/ggoyokeln.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.yfazqb.com/Article/details/gpsrzdhel.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.epnwcf.com/Article/details/gtytrlowq.sHtML

[F08] 遍历目录
来源：http://read.share.tarul.cn/Article/details/glwfgvupw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.yfazqb.com/Article/details/gmlqqdsvm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.tarul.cn/Article/details/gigxadqsl.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.vehdjk.com/Article/details/guyatcque.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fktsv.cn/Article/details/gnwpvzbpe.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.tarul.cn/Article/details/gfwskelsx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.sjlbkw.cn/Article/details/gkvqcntul.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.vehdjk.com/Article/details/gunjjcjik.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.epnwcf.com/Article/details/guhxgykob.sHtML

[F09] 获取文件大小
来源：http://read.share.fktsv.cn/Article/details/gaqqgakir.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.tarul.cn/Article/details/glngmsniy.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.tarul.cn/Article/details/gmyzsysez.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.bbcook.cn/Article/details/glutzsprp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fktsv.cn/Article/details/gxlplxauu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fktsv.cn/Article/details/gikocingb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.vehdjk.com/Article/details/gtzhorefg.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gtjympyxc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.yfazqb.com/Article/details/gwzkmxcfr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.yfazqb.com/Article/details/gphbsltvj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.yfazqb.com/Article/details/gfzgydeba.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fktsv.cn/Article/details/gwcyiqgna.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fktsv.cn/Article/details/goxdnuhnj.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gymombjwb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.tarul.cn/Article/details/gbscayioy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fktsv.cn/Article/details/gtaanqqtv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/grvxcbqzd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gjfjoktck.sHtML

[F11] 复制与移动文件
来源：http://www.blog.yfazqb.com/Article/details/gaoescfkr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/gaaaaqvua.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.yfazqb.com/Article/details/gaslpxbix.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gkamxzkeq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gmtirvzic.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.yfazqb.com/Article/details/grfmyljpb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.yfazqb.com/Article/details/gfwazrzcv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.tarul.cn/Article/details/gpywwrtce.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.yfazqb.com/Article/details/gfzbwqgbw.sHtML

[F12] CSV 读写
来源：http://blog.bbcook.cn/Article/details/giqlzrdjc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fktsv.cn/Article/details/gzttzqbda.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.yfazqb.com/Article/details/gophwyprz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.tarul.cn/Article/details/gurdychrn.sHtML

TS:   // 同上
来源：http://read.share.tarul.cn/Article/details/gpqpmoahb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.yfazqb.com/Article/details/gulgcjlsi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.epnwcf.com/Article/details/gciemmigz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.vehdjk.com/Article/details/gbqbwaabz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fktsv.cn/Article/details/gvsszzill.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/galqxlqww.sHtML

G. 面向对象
来源：http://www.blog.epnwcf.com/Article/details/gkinrnecj.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gdikkajrt.sHtML

[G01] 定义类
来源：http://www.blog.vehdjk.com/Article/details/goyvztoku.sHtML

Py:   class User: pass
来源：http://read.share.epnwcf.com/Article/details/gqwmvnrbn.sHtML

PHP:  class User {}
来源：http://m.share.fktsv.cn/Article/details/gdsspzloe.sHtML

JS:   class User {}
来源：http://blog.sjlbkw.cn/Article/details/ghksurzzd.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.epnwcf.com/Article/details/gghzdserv.sHtML

Java: class User {}
来源：http://wap.tarul.cn/Article/details/guxmqkcbp.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.vehdjk.com/Article/details/gcwhlontc.sHtML

Ruby: class User; end
来源：http://www.share.tarul.cn/Article/details/ggtokjfnc.sHtML

C#:   class User {}
来源：http://baike.sjlbkw.cn/Article/details/gskextsaj.sHtML

[G02] 构造函数
来源：http://read.share.yfazqb.com/Article/details/gzuptwelm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fktsv.cn/Article/details/gnmcyvvzw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fktsv.cn/Article/details/gwfilevik.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.bbcook.cn/Article/details/gilqhvhhs.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fktsv.cn/Article/details/gtoxrmfjc.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.yfazqb.com/Article/details/goduglezx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.yfazqb.com/Article/details/gdulwjqbw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.tarul.cn/Article/details/geidfmeht.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.bbcook.cn/Article/details/gcxmjsikj.sHtML

[G03] 实例属性
来源：http://mobile.tarul.cn/Article/details/gdjrmlsuh.sHtML

Py:   self.name = "x"
来源：http://m.share.yfazqb.com/Article/details/gafleiffd.sHtML

PHP:  public string $name = "x";
来源：http://3g.sjlbkw.cn/Article/details/gqvinizno.sHtML

JS:   this.name = "x";
来源：http://baike.tarul.cn/Article/details/gejyasrfq.sHtML

TS:   name: string = "x";
来源：http://www.blog.fktsv.cn/Article/details/gygqhmmnl.sHtML

Java: private String name;
来源：http://3g.sjlbkw.cn/Article/details/gousxawou.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.tarul.cn/Article/details/girdxvwux.sHtML

Ruby: @name = "x"
来源：http://mobile.fktsv.cn/Article/details/ghxuhszyy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.sjlbkw.cn/Article/details/gobyfobak.sHtML

[G04] 定义方法
来源：http://m.share.vehdjk.com/Article/details/gwahaiayj.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.yfazqb.com/Article/details/gqgtxymvb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.tarul.cn/Article/details/gzklchfmy.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.yfazqb.com/Article/details/gwhtkacsd.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.epnwcf.com/Article/details/gmrbmsltu.sHtML

Java: String greet() { return name; }
来源：http://www.blog.tarul.cn/Article/details/gymjoqhoq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.epnwcf.com/Article/details/gahiossfn.sHtML

Ruby: def greet; @name; end
来源：http://mobile.vehdjk.com/Article/details/gdsduzvqp.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.sjlbkw.cn/Article/details/gwcdlpabp.sHtML

[G05] 继承
来源：http://read.share.epnwcf.com/Article/details/gfmgxwauz.sHtML

Py:   class Admin(User): pass
来源：http://blog.yfazqb.com/Article/details/gxvxatcfj.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.tarul.cn/Article/details/gdkxedkoj.sHtML

JS:   class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/gfmheljbe.sHtML

TS:   class Admin extends User {}
来源：http://mobile.epnwcf.com/Article/details/gtkoqioyl.sHtML


<!-- 参考信息 -->