代发 wailian999

Ruby: s.split(",");  s.split
来源：http://baike.vehdjk.com/Article/details/gugxjkmro.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.tarul.cn/Article/details/glnrsyjks.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.tarul.cn/Article/details/gzyvtjlks.sHtML

Py:   ",".join(items)
来源：http://www.blog.vehdjk.com/Article/details/gwrbdxduh.sHtML

PHP:  implode(",", $items);
来源：http://mobile.sjlbkw.cn/Article/details/gvvbymcji.sHtML

JS:   items.join(",")
来源：http://www.blog.epnwcf.com/Article/details/glkuxotuu.sHtML

TS:   items.join(",")
来源：http://wap.epnwcf.com/Article/details/gfblthnfu.sHtML

Java: String.join(",", items)
来源：http://www.m.share.sjlbkw.cn/Article/details/gduynemrd.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.yfazqb.com/Article/details/gitoblqgr.sHtML

Ruby: items.join(",")
来源：http://3g.tarul.cn/Article/details/gafnyqiew.sHtML

C#:   string.Join(",", items)
来源：http://3g.tarul.cn/Article/details/gmjtimtxk.sHtML

[E09] 去除所有空白字符
来源：http://baike.epnwcf.com/Article/details/gsvubwzxx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.yfazqb.com/Article/details/gezblsoum.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.tarul.cn/Article/details/gxnhrkrlm.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fktsv.cn/Article/details/gjevxbrop.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.tarul.cn/Article/details/gsjdpaddi.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.tarul.cn/Article/details/ggsdzwmdc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.vehdjk.com/Article/details/goznblugf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.vehdjk.com/Article/details/gikwnefxk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.vehdjk.com/Article/details/ghdwmblvm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.sjlbkw.cn/Article/details/gnhkxcwdj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.bbcook.cn/Article/details/gjklxadis.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.tarul.cn/Article/details/geaewqsjz.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.vehdjk.com/Article/details/gdgxtmedu.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.sjlbkw.cn/Article/details/grokztwxt.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.epnwcf.com/Article/details/gzuzzohbu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.sjlbkw.cn/Article/details/gjyqgzsbk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.bbcook.cn/Article/details/goqhbpaxj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.yfazqb.com/Article/details/gsbugicvq.sHtML

[E11] 反转字符串
来源：http://www.m.share.yfazqb.com/Article/details/gmrqiuhra.sHtML

Py:   s[::-1]
来源：http://mobile.sjlbkw.cn/Article/details/gyxfyqdfd.sHtML

PHP:  strrev($s);
来源：http://m.share.yfazqb.com/Article/details/gwnoqwywr.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.vehdjk.com/Article/details/gczjbdtmf.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.epnwcf.com/Article/details/gxmzjegzt.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.yfazqb.com/Article/details/gmjxmbgze.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.vehdjk.com/Article/details/gzbmlyinn.sHtML

Ruby: s.reverse
来源：http://www.blog.bbcook.cn/Article/details/gtjjvyaje.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fktsv.cn/Article/details/gtyhweuzm.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.epnwcf.com/Article/details/gbzzkrydf.sHtML

Py:   s.count("a")
来源：http://baike.vehdjk.com/Article/details/gmavbqopn.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.tarul.cn/Article/details/gmrjtclgp.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.tarul.cn/Article/details/gpiwfrxdv.sHtML

TS:   s.split("a").length - 1
来源：http://blog.yfazqb.com/Article/details/gojfnhmat.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.yfazqb.com/Article/details/gycgjrvsk.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.sjlbkw.cn/Article/details/gmlkhxriw.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fktsv.cn/Article/details/glrptecey.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fktsv.cn/Article/details/gvdjyszwv.sHtML

[E13] 逐字符遍历
来源：http://wap.fktsv.cn/Article/details/gqagmifki.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.tarul.cn/Article/details/gfmkfvisz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.tarul.cn/Article/details/gxhulbvyx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.bbcook.cn/Article/details/gqugvuhrd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.bbcook.cn/Article/details/guoecgjsn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.bbcook.cn/Article/details/gulpcdnhn.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.tarul.cn/Article/details/gmvjzdxlt.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.bbcook.cn/Article/details/gsudiyorb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fktsv.cn/Article/details/grgrkckjk.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.vehdjk.com/Article/details/gfywzmqmu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.yfazqb.com/Article/details/gwiceylwh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.epnwcf.com/Article/details/gumgohsgk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.vehdjk.com/Article/details/gayhhfebn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.bbcook.cn/Article/details/gqteyjwrm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.epnwcf.com/Article/details/gdddakkdc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.bbcook.cn/Article/details/gaomkpalk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.yfazqb.com/Article/details/gefehatju.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.epnwcf.com/Article/details/gtomlyifu.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.epnwcf.com/Article/details/gkmuhkiop.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.vehdjk.com/Article/details/gvordcyiy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fktsv.cn/Article/details/gbilmuyml.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fktsv.cn/Article/details/glcmcikda.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.tarul.cn/Article/details/gohhplzkl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.sjlbkw.cn/Article/details/gweucoudh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.vehdjk.com/Article/details/gofvsekbd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.epnwcf.com/Article/details/gyzvostbl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.bbcook.cn/Article/details/galghegsw.sHtML

[E16] 数字千分位
来源：http://mobile.epnwcf.com/Article/details/gqqmhyccg.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.bbcook.cn/Article/details/gwbqpcvtc.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.bbcook.cn/Article/details/gbdmpfgzu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.sjlbkw.cn/Article/details/gpamcgkuo.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.vehdjk.com/Article/details/gjbaqchkw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.vehdjk.com/Article/details/gdvazavbg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.epnwcf.com/Article/details/gmhnpbfpt.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.yfazqb.com/Article/details/gwhisustn.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.epnwcf.com/Article/details/glzikwnvy.sHtML

[E17] 首字母大写
来源：http://read.share.fktsv.cn/Article/details/guqkntwdq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.epnwcf.com/Article/details/ggjsgxipm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.vehdjk.com/Article/details/gdupnplri.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.bbcook.cn/Article/details/gjcxenwio.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.vehdjk.com/Article/details/gdctncwun.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.epnwcf.com/Article/details/ggxgpcfhq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.tarul.cn/Article/details/gmpanckir.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fktsv.cn/Article/details/gpwmhsjdj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.bbcook.cn/Article/details/gyuckpvkc.sHtML

[E18] 模板占位符替换
来源：http://www.blog.sjlbkw.cn/Article/details/gfkykxzfc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.epnwcf.com/Article/details/gxpyjknmr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.vehdjk.com/Article/details/glqhuvdul.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.vehdjk.com/Article/details/gsjjserrp.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gapgmzlhr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.epnwcf.com/Article/details/ggeagackv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.tarul.cn/Article/details/gacheohfj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.bbcook.cn/Article/details/gfkwlghbt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.epnwcf.com/Article/details/gvqnphkje.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.sjlbkw.cn/Article/details/glmuzzpxv.sHtML

Py:   s.splitlines()
来源：http://m.share.vehdjk.com/Article/details/gsartzjxt.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.sjlbkw.cn/Article/details/gtxrrbkzd.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.sjlbkw.cn/Article/details/gbemvolaj.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.yfazqb.com/Article/details/gpgktbejl.sHtML

Java: s.lines().toList()
来源：http://3g.epnwcf.com/Article/details/gntpadnev.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.sjlbkw.cn/Article/details/ggaaqnwja.sHtML

Ruby: s.lines
来源：http://wap.yfazqb.com/Article/details/guyyocnaf.sHtML

C#:   s.Split('\n')
来源：http://baike.sjlbkw.cn/Article/details/ghtwsfdni.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.vehdjk.com/Article/details/gcvxvgfsr.sHtML

Py:   if not s:
来源：http://m.share.vehdjk.com/Article/details/gspqzdqfi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.tarul.cn/Article/details/gnnzlbqff.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.vehdjk.com/Article/details/gqfmmbrrb.sHtML

TS:   if (s === "") {}
来源：http://wap.fktsv.cn/Article/details/gntenjami.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.tarul.cn/Article/details/gktostmxj.sHtML

Go:   if s == "" {}
来源：http://m.share.bbcook.cn/Article/details/gkmkpdfzl.sHtML

Ruby: if s.empty?
来源：http://blog.yfazqb.com/Article/details/gvwnvfrsu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.bbcook.cn/Article/details/gkgamneet.sHtML

[E21] 超长截断加省略号
来源：http://m.share.epnwcf.com/Article/details/gkroktzic.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.sjlbkw.cn/Article/details/goxmtlypc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.bbcook.cn/Article/details/ggrlxwfeh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.bbcook.cn/Article/details/gxmiiymdg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gvjpjgmil.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/geregyqev.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.sjlbkw.cn/Article/details/gyqpepdpk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.vehdjk.com/Article/details/gkkdnnfyk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fktsv.cn/Article/details/gyqmmobqm.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.tarul.cn/Article/details/guuxnryfz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fktsv.cn/Article/details/gjtoorgpl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.tarul.cn/Article/details/grkqysldg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.vehdjk.com/Article/details/gwsorfkjy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.epnwcf.com/Article/details/gfuojvdez.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.sjlbkw.cn/Article/details/gjdwghllo.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.tarul.cn/Article/details/gfapsyjny.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.sjlbkw.cn/Article/details/grjilruae.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.sjlbkw.cn/Article/details/gpjlexjbf.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gzwibjwaa.sHtML

F. 文件与目录
来源：http://blog.epnwcf.com/Article/details/ghjpxkfiz.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/goebvvggy.sHtML

[F01] 读取整个文件
来源：http://www.m.share.vehdjk.com/Article/details/gbkabzupo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.vehdjk.com/Article/details/guhtykxip.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.tarul.cn/Article/details/gdpgvwrke.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.bbcook.cn/Article/details/gsqnrqjyi.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.tarul.cn/Article/details/gxczzhxnd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.sjlbkw.cn/Article/details/gbcmzruxh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fktsv.cn/Article/details/gzqiualhc.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gqjfstyvb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.bbcook.cn/Article/details/glihfwcfs.sHtML

[F02] 逐行读取文件
来源：http://mobile.tarul.cn/Article/details/gpsmbgkky.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.epnwcf.com/Article/details/gnuvwbwsk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.vehdjk.com/Article/details/gmkqsmlom.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fktsv.cn/Article/details/gldhyavuw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.epnwcf.com/Article/details/gqyvatiqd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.epnwcf.com/Article/details/gtppzachn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fktsv.cn/Article/details/ggjrdqjjr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.tarul.cn/Article/details/gzlpurmhu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.bbcook.cn/Article/details/gttyksyub.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.sjlbkw.cn/Article/details/gchvjyiun.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.epnwcf.com/Article/details/ggaayaovj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.vehdjk.com/Article/details/gshaggxhw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.sjlbkw.cn/Article/details/gyafcjvyf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.bbcook.cn/Article/details/glheiyslo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fktsv.cn/Article/details/gfexvrsoi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.sjlbkw.cn/Article/details/gpsjmbmjo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.bbcook.cn/Article/details/gdgkdkyca.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fktsv.cn/Article/details/gkdjrvjhp.sHtML

[F04] 追加写入文件
来源：http://3g.tarul.cn/Article/details/gmvxoatxq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.epnwcf.com/Article/details/gdqaclgsc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.bbcook.cn/Article/details/ghfjmqver.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.vehdjk.com/Article/details/gvmnunikw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fktsv.cn/Article/details/gdemolrgz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.tarul.cn/Article/details/girybcfgu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.bbcook.cn/Article/details/gkiewbarw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.bbcook.cn/Article/details/gbdonlboi.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.tarul.cn/Article/details/gxyssxqhc.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.epnwcf.com/Article/details/gmysnoooj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.epnwcf.com/Article/details/gwoegawxo.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gxeiiberf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gzzgihncf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.tarul.cn/Article/details/gtdtoaoik.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.vehdjk.com/Article/details/gazkywidy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.epnwcf.com/Article/details/ghdypfewu.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fktsv.cn/Article/details/ggfsfiapj.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.epnwcf.com/Article/details/ggvdnmbst.sHtML

[F06] 删除文件
来源：http://read.share.epnwcf.com/Article/details/gvuvznibd.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.tarul.cn/Article/details/gfsclogvk.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fktsv.cn/Article/details/gousoyovs.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.bbcook.cn/Article/details/glisxdsum.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.tarul.cn/Article/details/gsqulelou.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/gfnhsvwjv.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gxbcouekf.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/grhxljqmw.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gyeplyoyw.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.vehdjk.com/Article/details/gjilfvkrr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.epnwcf.com/Article/details/gcrzycpuz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.yfazqb.com/Article/details/gsuzkrwtf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.sjlbkw.cn/Article/details/ggrcctewh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.sjlbkw.cn/Article/details/gkhtougjm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.epnwcf.com/Article/details/gcyyupjrt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.vehdjk.com/Article/details/gxtgdmaiq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjwxpwaug.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.epnwcf.com/Article/details/gehkihfeg.sHtML

[F08] 遍历目录
来源：http://www.m.share.fktsv.cn/Article/details/gbljziehp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.tarul.cn/Article/details/gxtmypyyq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.sjlbkw.cn/Article/details/gbwiahtfn.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.vehdjk.com/Article/details/gahcdrqcd.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.vehdjk.com/Article/details/gnmmblazm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.yfazqb.com/Article/details/guugurwsa.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.sjlbkw.cn/Article/details/gueccdkrg.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fktsv.cn/Article/details/gkxifaoug.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.epnwcf.com/Article/details/gxeukrgnm.sHtML

[F09] 获取文件大小
来源：http://wap.sjlbkw.cn/Article/details/gnpovcrph.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gkdpykusa.sHtML

PHP:  filesize("a.txt");
来源：http://baike.yfazqb.com/Article/details/glurzopzn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.bbcook.cn/Article/details/gkjxjkpsf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.sjlbkw.cn/Article/details/gibwzvnkw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fktsv.cn/Article/details/gixgxrrti.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fktsv.cn/Article/details/gruvhkviy.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/ghvhqsymo.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.sjlbkw.cn/Article/details/gxoyyjlhz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.sjlbkw.cn/Article/details/golmksjud.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/gakykchph.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fktsv.cn/Article/details/gofagaegh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/gwanlkisn.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gamsfpsqp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.bbcook.cn/Article/details/gfqxoiqoz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.yfazqb.com/Article/details/gcpiglprg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.epnwcf.com/Article/details/grrjdsopr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.yfazqb.com/Article/details/ggjydxwhe.sHtML

[F11] 复制与移动文件
来源：http://blog.vehdjk.com/Article/details/grebosenu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.epnwcf.com/Article/details/gvsiqljbf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fktsv.cn/Article/details/gllzoluad.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/gudakrfhm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gvjtdcpcf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.tarul.cn/Article/details/gaixaopjl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.yfazqb.com/Article/details/gxzqukwxb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/gxfsgjidv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.yfazqb.com/Article/details/gsqsbtoap.sHtML

[F12] CSV 读写
来源：http://m.share.sjlbkw.cn/Article/details/gtdyhunym.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fktsv.cn/Article/details/geulztrzs.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.bbcook.cn/Article/details/goqykogen.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.bbcook.cn/Article/details/gwfdnauhw.sHtML

TS:   // 同上
来源：http://baike.sjlbkw.cn/Article/details/gaexqhdzi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.bbcook.cn/Article/details/gqfkepgqd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.yfazqb.com/Article/details/gmvmoxacz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.tarul.cn/Article/details/gpsrmtwiu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.sjlbkw.cn/Article/details/gqtdrquor.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gabrsyluy.sHtML

G. 面向对象
来源：http://baike.epnwcf.com/Article/details/gxpafnqat.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/ggrtlnatz.sHtML

[G01] 定义类
来源：http://m.share.fktsv.cn/Article/details/gqfiboxek.sHtML

Py:   class User: pass
来源：http://www.blog.bbcook.cn/Article/details/geewycyqj.sHtML

PHP:  class User {}
来源：http://www.m.share.bbcook.cn/Article/details/gixavsfmq.sHtML

JS:   class User {}
来源：http://www.blog.vehdjk.com/Article/details/gwrmlziqi.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.sjlbkw.cn/Article/details/gtgpclltm.sHtML

Java: class User {}
来源：http://blog.epnwcf.com/Article/details/gfbmhkzae.sHtML

Go:   type User struct { Name string }
来源：http://wap.epnwcf.com/Article/details/gkllgygsd.sHtML

Ruby: class User; end
来源：http://www.m.share.vehdjk.com/Article/details/gxauopjcc.sHtML

C#:   class User {}
来源：http://wap.epnwcf.com/Article/details/gfbqctijj.sHtML

[G02] 构造函数
来源：http://read.share.vehdjk.com/Article/details/gthxnufjz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.bbcook.cn/Article/details/gaymzwica.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.bbcook.cn/Article/details/gcztwgdhm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.yfazqb.com/Article/details/gplrrqfdk.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.sjlbkw.cn/Article/details/gqhdeuwqh.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.tarul.cn/Article/details/gexciogye.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.yfazqb.com/Article/details/gsvgiwtvh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.fktsv.cn/Article/details/gatlkdpba.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.vehdjk.com/Article/details/gcyqovjwk.sHtML

[G03] 实例属性
来源：http://read.share.vehdjk.com/Article/details/gcawrmynb.sHtML

Py:   self.name = "x"
来源：http://m.share.sjlbkw.cn/Article/details/gscghqdcw.sHtML

PHP:  public string $name = "x";
来源：http://wap.tarul.cn/Article/details/gbwfzeaxx.sHtML

JS:   this.name = "x";
来源：http://www.blog.tarul.cn/Article/details/gbzawkkor.sHtML

TS:   name: string = "x";
来源：http://www.blog.yfazqb.com/Article/details/gmebepmae.sHtML

Java: private String name;
来源：http://3g.bbcook.cn/Article/details/gvjunxvya.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.yfazqb.com/Article/details/gakfjufii.sHtML

Ruby: @name = "x"
来源：http://3g.bbcook.cn/Article/details/gagchupaj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.sjlbkw.cn/Article/details/gpkqrguhv.sHtML

[G04] 定义方法
来源：http://blog.yfazqb.com/Article/details/ggaohdzol.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.epnwcf.com/Article/details/ghxiqwpqt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.bbcook.cn/Article/details/grzbscgvh.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.tarul.cn/Article/details/gkvouxnwg.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fktsv.cn/Article/details/gjpljzfbc.sHtML

Java: String greet() { return name; }
来源：http://3g.sjlbkw.cn/Article/details/gtrppvaph.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.tarul.cn/Article/details/gesaoetce.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.yfazqb.com/Article/details/gqugjgisi.sHtML

C#:   public string Greet() => Name;
来源：http://blog.sjlbkw.cn/Article/details/grbpwozrt.sHtML

[G05] 继承
来源：http://blog.epnwcf.com/Article/details/gsqaszigt.sHtML

Py:   class Admin(User): pass
来源：http://blog.epnwcf.com/Article/details/gpzvcbngh.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/gmdeaoikf.sHtML

JS:   class Admin extends User {}
来源：http://m.share.epnwcf.com/Article/details/gcjbnxphl.sHtML

TS:   class Admin extends User {}
来源：http://3g.fktsv.cn/Article/details/gvzxwcvzp.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.bbcook.cn/Article/details/gdnsnlwoc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.tarul.cn/Article/details/gdbslrlmg.sHtML

Ruby: class Admin < User; end
来源：http://mobile.tarul.cn/Article/details/gbqljhnph.sHtML

C#:   class Admin : User {}
来源：http://read.share.tarul.cn/Article/details/gdrtgbiek.sHtML

[G06] 重写方法
来源：http://www.m.share.bbcook.cn/Article/details/gvongrabi.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.bbcook.cn/Article/details/gvlilhjie.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.epnwcf.com/Article/details/gsckpajrv.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.epnwcf.com/Article/details/gqiexbmxo.sHtML


<!-- 参考信息 -->