代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.yfazqb.com/Article/details/gfufhjaoa.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.sjlbkw.cn/Article/details/gzmrdjpfg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.bbcook.cn/Article/details/gezpkwhxb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.bbcook.cn/Article/details/gnqmibyoc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fktsv.cn/Article/details/gslgzonjb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.epnwcf.com/Article/details/gpgtmljbu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.bbcook.cn/Article/details/gudexclan.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.vehdjk.com/Article/details/gmvtywkke.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.epnwcf.com/Article/details/gzbalqofu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fktsv.cn/Article/details/gngbsqqdq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.yfazqb.com/Article/details/guvclabma.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.epnwcf.com/Article/details/gzjjnxscw.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.vehdjk.com/Article/details/gqrapwzmt.sHtML

Java: String.format("%03d", 7)
来源：http://3g.bbcook.cn/Article/details/gbvhbindz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.yfazqb.com/Article/details/gswlbwicj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fktsv.cn/Article/details/gpcihqpwm.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.yfazqb.com/Article/details/gtptdlzsi.sHtML

[E11] 反转字符串
来源：http://www.share.bbcook.cn/Article/details/giydvzuks.sHtML

Py:   s[::-1]
来源：http://m.share.fktsv.cn/Article/details/gmpdrrbok.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fktsv.cn/Article/details/gkbfnwlio.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.bbcook.cn/Article/details/ghtlrvlhf.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/gdyyvkluv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.yfazqb.com/Article/details/gyfpcikuy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.yfazqb.com/Article/details/glopaiwuy.sHtML

Ruby: s.reverse
来源：http://read.share.vehdjk.com/Article/details/ghgtomqqw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.tarul.cn/Article/details/ghosucukq.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.bbcook.cn/Article/details/gljgnrjsq.sHtML

Py:   s.count("a")
来源：http://www.share.bbcook.cn/Article/details/ggkivjhyv.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.tarul.cn/Article/details/ggrlvyhef.sHtML

JS:   s.split("a").length - 1
来源：http://baike.yfazqb.com/Article/details/ghadqxsdp.sHtML

TS:   s.split("a").length - 1
来源：http://3g.epnwcf.com/Article/details/geraebtkn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.sjlbkw.cn/Article/details/ghtjtkogq.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.sjlbkw.cn/Article/details/ggewauigk.sHtML

Ruby: s.count("a")
来源：http://baike.epnwcf.com/Article/details/gqnvggwwe.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.fktsv.cn/Article/details/gkeesopud.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gbxvnptmk.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.vehdjk.com/Article/details/ghwcgmmsf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.sjlbkw.cn/Article/details/gxflplcgc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.yfazqb.com/Article/details/gzhdhaomw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.epnwcf.com/Article/details/gapfbpxcc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.epnwcf.com/Article/details/gnehedicd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.sjlbkw.cn/Article/details/gyokdvxhq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.sjlbkw.cn/Article/details/gmiokvwqj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.vehdjk.com/Article/details/gzsklugkz.sHtML

[E14] URL 编码与 Base64
来源：http://blog.bbcook.cn/Article/details/gcquiaeer.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.vehdjk.com/Article/details/gigsdqjaa.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.bbcook.cn/Article/details/gqfwezcez.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.yfazqb.com/Article/details/gyjzhnddr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.yfazqb.com/Article/details/gmihvssjd.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.tarul.cn/Article/details/gqtnwmydk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.vehdjk.com/Article/details/gburhlexi.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.vehdjk.com/Article/details/glojfwpve.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.tarul.cn/Article/details/gdbdceimf.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.yfazqb.com/Article/details/grkduecus.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.yfazqb.com/Article/details/gdiaggtre.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.epnwcf.com/Article/details/gznkufehw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.vehdjk.com/Article/details/gjltnhiid.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.sjlbkw.cn/Article/details/ggnubpxgb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.tarul.cn/Article/details/gcqszbeca.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.yfazqb.com/Article/details/gkjvvgggb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.yfazqb.com/Article/details/grqzhzziu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.vehdjk.com/Article/details/gdkscvfog.sHtML

[E16] 数字千分位
来源：http://baike.vehdjk.com/Article/details/gzacqhazn.sHtML

Py:   f"{1234567:,}"
来源：http://3g.epnwcf.com/Article/details/gsjqgalkm.sHtML

PHP:  number_format(1234567);
来源：http://3g.yfazqb.com/Article/details/ghbwealbp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.yfazqb.com/Article/details/gazxwmpia.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.yfazqb.com/Article/details/gylxwafli.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.vehdjk.com/Article/details/gfcmacqlb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.bbcook.cn/Article/details/gaetkjefo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.tarul.cn/Article/details/gopdpvmrl.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.vehdjk.com/Article/details/gbcbdfjxt.sHtML

[E17] 首字母大写
来源：http://www.blog.sjlbkw.cn/Article/details/gcphqrvdy.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.bbcook.cn/Article/details/gvmdjvaog.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.bbcook.cn/Article/details/gymfmfvdc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fktsv.cn/Article/details/gpvgzlaqu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.vehdjk.com/Article/details/gisqursku.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.sjlbkw.cn/Article/details/ghokayhjc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.sjlbkw.cn/Article/details/gkuzvjdtn.sHtML

Ruby: s.capitalize
来源：http://blog.sjlbkw.cn/Article/details/gxiddsfsr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.yfazqb.com/Article/details/gopqsspvi.sHtML

[E18] 模板占位符替换
来源：http://3g.epnwcf.com/Article/details/gpjimzido.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.epnwcf.com/Article/details/gpbeoicdf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.yfazqb.com/Article/details/glzagatuf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.tarul.cn/Article/details/gxdrcoosx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gaavjvgwr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.vehdjk.com/Article/details/gxgbzized.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fktsv.cn/Article/details/gqsvievrh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.epnwcf.com/Article/details/glvtfttxi.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.yfazqb.com/Article/details/gbmplknij.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.sjlbkw.cn/Article/details/gohsrhexg.sHtML

Py:   s.splitlines()
来源：http://www.share.bbcook.cn/Article/details/gzkklrgdg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.tarul.cn/Article/details/gwxbkfing.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fktsv.cn/Article/details/gplocngul.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.bbcook.cn/Article/details/gopdzfzee.sHtML

Java: s.lines().toList()
来源：http://www.blog.yfazqb.com/Article/details/gjtnnebrm.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.epnwcf.com/Article/details/gtkcckvmo.sHtML

Ruby: s.lines
来源：http://read.share.vehdjk.com/Article/details/gtmjkglqr.sHtML

C#:   s.Split('\n')
来源：http://baike.fktsv.cn/Article/details/gtqmbnyfy.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.vehdjk.com/Article/details/gwcymicsd.sHtML

Py:   if not s:
来源：http://www.blog.tarul.cn/Article/details/gtdeazqyy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.sjlbkw.cn/Article/details/gicpmnnio.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.bbcook.cn/Article/details/gwwytdraj.sHtML

TS:   if (s === "") {}
来源：http://www.blog.tarul.cn/Article/details/gmltghufb.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.bbcook.cn/Article/details/gooowoded.sHtML

Go:   if s == "" {}
来源：http://www.blog.bbcook.cn/Article/details/gfcwgsmqj.sHtML

Ruby: if s.empty?
来源：http://wap.epnwcf.com/Article/details/gzkudjmml.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.sjlbkw.cn/Article/details/gttplfdxc.sHtML

[E21] 超长截断加省略号
来源：http://www.share.yfazqb.com/Article/details/gudxgzafp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.vehdjk.com/Article/details/gfsyzdqcc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.vehdjk.com/Article/details/gsrbwsjyr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/gywzorcxh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.epnwcf.com/Article/details/gbhjejabz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.bbcook.cn/Article/details/gwkhekvft.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.yfazqb.com/Article/details/gcqcigaxn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.vehdjk.com/Article/details/gqnfmndlo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.yfazqb.com/Article/details/geaesihme.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fktsv.cn/Article/details/gqimbfrnh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.yfazqb.com/Article/details/ghfqisfif.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.sjlbkw.cn/Article/details/gqrdkudkc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.sjlbkw.cn/Article/details/gmvotmdpv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.epnwcf.com/Article/details/gnugozecg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.vehdjk.com/Article/details/gdhmliain.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.yfazqb.com/Article/details/gefjsxjgq.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.tarul.cn/Article/details/gyeqpuvwy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.yfazqb.com/Article/details/ghqixgorb.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gtcaowlnp.sHtML

F. 文件与目录
来源：http://3g.tarul.cn/Article/details/grvtfjbkb.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gcduzwdfa.sHtML

[F01] 读取整个文件
来源：http://wap.tarul.cn/Article/details/greimtfil.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.tarul.cn/Article/details/gennxmiyj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gjcowcdil.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fktsv.cn/Article/details/gnbqhcfcf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fktsv.cn/Article/details/guhohwfya.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fktsv.cn/Article/details/gutnpwctd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.vehdjk.com/Article/details/gufikgzfl.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fktsv.cn/Article/details/ggqrkjzzn.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gtoisopsb.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.vehdjk.com/Article/details/gwusolbmu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.epnwcf.com/Article/details/gcjbmufze.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.vehdjk.com/Article/details/gpxeanlpz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.yfazqb.com/Article/details/golzubpkz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.bbcook.cn/Article/details/gapaoqhgs.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.vehdjk.com/Article/details/ghyqosyhn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.tarul.cn/Article/details/geslphqjs.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.vehdjk.com/Article/details/godlxlibr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.yfazqb.com/Article/details/gaaintrdk.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fktsv.cn/Article/details/gmhmprvno.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.tarul.cn/Article/details/gzmevhlub.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.tarul.cn/Article/details/gtocftgtb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.sjlbkw.cn/Article/details/gnprpozdd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fktsv.cn/Article/details/gasqzxytc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.yfazqb.com/Article/details/glbgvgecf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.vehdjk.com/Article/details/grgfomcux.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.tarul.cn/Article/details/gjtdlhihu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.tarul.cn/Article/details/gtaohoaok.sHtML

[F04] 追加写入文件
来源：http://www.share.tarul.cn/Article/details/gmalsimvm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.yfazqb.com/Article/details/gsdwrzyfx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.yfazqb.com/Article/details/gebxilvzs.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.yfazqb.com/Article/details/gihheuici.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.bbcook.cn/Article/details/gtnwxaees.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fktsv.cn/Article/details/gpkhmcsex.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.epnwcf.com/Article/details/gtwatzdrs.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fktsv.cn/Article/details/gyoncsvde.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.sjlbkw.cn/Article/details/gnhueqxfs.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.tarul.cn/Article/details/gddzyupuj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.vehdjk.com/Article/details/gmtkwwdru.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/glmvlpgaq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.tarul.cn/Article/details/gtkgsagcm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gefaikhic.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.bbcook.cn/Article/details/gsfosropy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.bbcook.cn/Article/details/ggtxpttsv.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gwxxqovgc.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gexdzjemy.sHtML

[F06] 删除文件
来源：http://www.blog.epnwcf.com/Article/details/gyfkfmbsz.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.tarul.cn/Article/details/geaezujwb.sHtML

PHP:  unlink("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gfhbtkabq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gcgyhress.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.bbcook.cn/Article/details/ggjbhjsme.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.yfazqb.com/Article/details/glhqmqzof.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gnioncbfn.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gzjqaphxc.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.vehdjk.com/Article/details/gzyujbbof.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.sjlbkw.cn/Article/details/gclsrmlxa.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.epnwcf.com/Article/details/gfgrysrxs.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.epnwcf.com/Article/details/guwsnssio.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.sjlbkw.cn/Article/details/gwznogmhz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fktsv.cn/Article/details/gtzlbdtbq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gbjczotzi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.yfazqb.com/Article/details/gefetajow.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.vehdjk.com/Article/details/gehqyggtm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.epnwcf.com/Article/details/ghthexvgr.sHtML

[F08] 遍历目录
来源：http://3g.sjlbkw.cn/Article/details/gpqxcixrh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.epnwcf.com/Article/details/ghfotddvr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.bbcook.cn/Article/details/gntunuynl.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.tarul.cn/Article/details/gsbzxuepl.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fktsv.cn/Article/details/gndkkmhfc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.epnwcf.com/Article/details/gghmsxfey.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.sjlbkw.cn/Article/details/gtfstwgwy.sHtML

Ruby: Dir.children("dir")
来源：http://baike.epnwcf.com/Article/details/gvxskyoic.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.vehdjk.com/Article/details/guqlnlemd.sHtML

[F09] 获取文件大小
来源：http://www.m.share.sjlbkw.cn/Article/details/gkuesyhqd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.bbcook.cn/Article/details/gwmdkkobb.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gbsociixu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.yfazqb.com/Article/details/gfqylcyrx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.bbcook.cn/Article/details/gxklzdplt.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.sjlbkw.cn/Article/details/gkhliwgzy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.sjlbkw.cn/Article/details/gxwiidcme.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gbzfytgct.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.vehdjk.com/Article/details/gxerttqbp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fktsv.cn/Article/details/gaggtlula.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gruabixzn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gqqcfyyir.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/ggjxwditp.sHtML

TS:   path.extname("a.txt")
来源：http://3g.tarul.cn/Article/details/gcwyuswpv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fktsv.cn/Article/details/gfyuuhwet.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gddunhqnr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gxnblhgwa.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/gaggyhcjo.sHtML

[F11] 复制与移动文件
来源：http://m.share.vehdjk.com/Article/details/glkrslbsx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.tarul.cn/Article/details/gxuyuiker.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.vehdjk.com/Article/details/gqoujnllh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/grmepwueg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/gjtlykvff.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.vehdjk.com/Article/details/gkfnzapya.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.vehdjk.com/Article/details/gdyexgkyq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/gsbpiusvm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.tarul.cn/Article/details/gzqmqxrvt.sHtML

[F12] CSV 读写
来源：http://mobile.sjlbkw.cn/Article/details/gfcfipzun.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fktsv.cn/Article/details/gpiezumcz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fktsv.cn/Article/details/gsqqfiscg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.vehdjk.com/Article/details/gvaoxipfm.sHtML

TS:   // 同上
来源：http://www.blog.tarul.cn/Article/details/grxiztemv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.epnwcf.com/Article/details/geilofzvi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.yfazqb.com/Article/details/gvipuzosp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.yfazqb.com/Article/details/gozjpxkrf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.epnwcf.com/Article/details/gnzoijrsr.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gthmllnjt.sHtML

G. 面向对象
来源：http://3g.tarul.cn/Article/details/gumdurjso.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gtzqoxxca.sHtML

[G01] 定义类
来源：http://m.share.vehdjk.com/Article/details/ghdtbvlmf.sHtML

Py:   class User: pass
来源：http://www.m.share.bbcook.cn/Article/details/gdbgxpfgg.sHtML

PHP:  class User {}
来源：http://www.blog.fktsv.cn/Article/details/gnicosboh.sHtML

JS:   class User {}
来源：http://baike.yfazqb.com/Article/details/griaevotj.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.vehdjk.com/Article/details/gfmdbcuhk.sHtML

Java: class User {}
来源：http://wap.epnwcf.com/Article/details/gmryapsbi.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fktsv.cn/Article/details/gbdbtawgl.sHtML

Ruby: class User; end
来源：http://3g.sjlbkw.cn/Article/details/gujxomgui.sHtML

C#:   class User {}
来源：http://mobile.yfazqb.com/Article/details/galbbhvhq.sHtML

[G02] 构造函数
来源：http://baike.epnwcf.com/Article/details/gdwhmqvcy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.tarul.cn/Article/details/gsgjzxfuc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.vehdjk.com/Article/details/gownudpwk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fktsv.cn/Article/details/guxhuawun.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.yfazqb.com/Article/details/gkubgldhq.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.tarul.cn/Article/details/gqerakngh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.vehdjk.com/Article/details/gpuacgdzi.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.yfazqb.com/Article/details/gtoelandc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fktsv.cn/Article/details/gfikuewvo.sHtML

[G03] 实例属性
来源：http://www.m.share.yfazqb.com/Article/details/ghnrpcomg.sHtML

Py:   self.name = "x"
来源：http://blog.vehdjk.com/Article/details/gqvqgsopy.sHtML

PHP:  public string $name = "x";
来源：http://mobile.tarul.cn/Article/details/gafkuhyal.sHtML

JS:   this.name = "x";
来源：http://mobile.tarul.cn/Article/details/gjndbcgmp.sHtML

TS:   name: string = "x";
来源：http://www.blog.bbcook.cn/Article/details/gppgmayft.sHtML

Java: private String name;
来源：http://3g.yfazqb.com/Article/details/gbolnhpop.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fktsv.cn/Article/details/grbdtiwsl.sHtML

Ruby: @name = "x"
来源：http://3g.fktsv.cn/Article/details/gwyflymjz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.vehdjk.com/Article/details/gchwvybff.sHtML

[G04] 定义方法
来源：http://baike.epnwcf.com/Article/details/gtbyxeksh.sHtML

Py:   def greet(self): return self.name
来源：http://blog.vehdjk.com/Article/details/grnizsbyx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.tarul.cn/Article/details/gpmfmqyrq.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.tarul.cn/Article/details/gmfdzvnbl.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.tarul.cn/Article/details/gxohfvgcw.sHtML

Java: String greet() { return name; }
来源：http://read.share.yfazqb.com/Article/details/gnubezwde.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.vehdjk.com/Article/details/gfaslkucs.sHtML

Ruby: def greet; @name; end
来源：http://baike.sjlbkw.cn/Article/details/gnpjwnzze.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.tarul.cn/Article/details/gmeuroxhc.sHtML

[G05] 继承
来源：http://mobile.yfazqb.com/Article/details/gxweizzda.sHtML

Py:   class Admin(User): pass
来源：http://blog.tarul.cn/Article/details/ggxqcsnxh.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fktsv.cn/Article/details/gjyeppbtg.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fktsv.cn/Article/details/guhkkyhss.sHtML

TS:   class Admin extends User {}
来源：http://blog.vehdjk.com/Article/details/gmaidpfhb.sHtML

Java: class Admin extends User {}
来源：http://read.share.tarul.cn/Article/details/gwdrgeinh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fktsv.cn/Article/details/gtwzhbwuz.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.vehdjk.com/Article/details/gaulxkbug.sHtML

C#:   class Admin : User {}
来源：http://m.share.sjlbkw.cn/Article/details/gdvbuyphp.sHtML

[G06] 重写方法
来源：http://baike.fktsv.cn/Article/details/gqirehfrn.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.vehdjk.com/Article/details/gtbehuxds.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.vehdjk.com/Article/details/ggpeinwbz.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.bbcook.cn/Article/details/geycspwsh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/giothxabx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fktsv.cn/Article/details/gdqhochhc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.tarul.cn/Article/details/ghflblelv.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.yfazqb.com/Article/details/gxtmtczsv.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.bbcook.cn/Article/details/gwfuowhkh.sHtML

[G07] 调用父类方法
来源：http://mobile.sjlbkw.cn/Article/details/gnyxljkfj.sHtML

Py:   super().greet()
来源：http://read.share.vehdjk.com/Article/details/gosedncrg.sHtML

PHP:  parent::greet();
来源：http://3g.fktsv.cn/Article/details/gsvueczol.sHtML

JS:   super.greet();
来源：http://blog.epnwcf.com/Article/details/gmgzyjjfz.sHtML

TS:   super.greet();
来源：http://baike.yfazqb.com/Article/details/ggsuttpla.sHtML

Java: super.greet();
来源：http://read.share.sjlbkw.cn/Article/details/gesfyawhw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.vehdjk.com/Article/details/gyofflxpg.sHtML


<!-- 参考信息 -->