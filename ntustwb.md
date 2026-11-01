代发 wailian999

Go:   strings.Join(items, ",")
来源：http://www.m.share.epnwcf.com/Article/details/gnsxjluxx.sHtML

Ruby: items.join(",")
来源：http://read.share.tarul.cn/Article/details/gjjyrseiy.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fktsv.cn/Article/details/grbwrjvmo.sHtML

[E09] 去除所有空白字符
来源：http://m.share.tarul.cn/Article/details/gtwxmbiid.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.epnwcf.com/Article/details/geecjzymm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.yfazqb.com/Article/details/gbpdohdkk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.fktsv.cn/Article/details/glyoayjqo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.sjlbkw.cn/Article/details/gxllytwdu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.epnwcf.com/Article/details/gxmofazsx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fktsv.cn/Article/details/gmjfiibks.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.vehdjk.com/Article/details/gpnrhkkxu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fktsv.cn/Article/details/goiyyzgsd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.tarul.cn/Article/details/gzxmttfsc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fktsv.cn/Article/details/gzlqalxmz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.sjlbkw.cn/Article/details/ghwtfjukq.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.vehdjk.com/Article/details/gpxfhbuda.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.sjlbkw.cn/Article/details/gdvkpxyno.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fktsv.cn/Article/details/gezdcxeix.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fktsv.cn/Article/details/glxofnbwm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.yfazqb.com/Article/details/gpxyfcogk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.vehdjk.com/Article/details/gvfqotplm.sHtML

[E11] 反转字符串
来源：http://www.m.share.fktsv.cn/Article/details/ghitwqgqo.sHtML

Py:   s[::-1]
来源：http://m.share.tarul.cn/Article/details/gpreabspx.sHtML

PHP:  strrev($s);
来源：http://mobile.epnwcf.com/Article/details/gockujqms.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.epnwcf.com/Article/details/gsbicrrdo.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.epnwcf.com/Article/details/glqfzmatp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fktsv.cn/Article/details/geoijljgm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.vehdjk.com/Article/details/gaicnilxh.sHtML

Ruby: s.reverse
来源：http://wap.sjlbkw.cn/Article/details/gtkwwiwxe.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.tarul.cn/Article/details/gsrzjfojl.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.tarul.cn/Article/details/gzgpojrqj.sHtML

Py:   s.count("a")
来源：http://mobile.fktsv.cn/Article/details/glmdslmhe.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.tarul.cn/Article/details/gbktvnfwo.sHtML

JS:   s.split("a").length - 1
来源：http://wap.sjlbkw.cn/Article/details/gjnikvniy.sHtML

TS:   s.split("a").length - 1
来源：http://3g.yfazqb.com/Article/details/gwydgqxde.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.bbcook.cn/Article/details/galpswqsp.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.vehdjk.com/Article/details/gbjbcqzhy.sHtML

Ruby: s.count("a")
来源：http://read.share.epnwcf.com/Article/details/gqjdwwnvd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.tarul.cn/Article/details/gesgbdkxy.sHtML

[E13] 逐字符遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gvwggzsxp.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.sjlbkw.cn/Article/details/gonrlwkcs.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.tarul.cn/Article/details/gkhilqyfj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.sjlbkw.cn/Article/details/gvphpdtam.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.epnwcf.com/Article/details/gotqldwtv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.epnwcf.com/Article/details/gqqijyade.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.tarul.cn/Article/details/ggtfibfez.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.vehdjk.com/Article/details/gnnbvwlkf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fktsv.cn/Article/details/gbzuyrtrg.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.yfazqb.com/Article/details/gdnvkykin.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.tarul.cn/Article/details/gcqetqblb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.sjlbkw.cn/Article/details/gtghfscim.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.vehdjk.com/Article/details/gmwckzafy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fktsv.cn/Article/details/grmfupbnh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.tarul.cn/Article/details/gtiahadro.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.sjlbkw.cn/Article/details/gbqqrbfrl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.bbcook.cn/Article/details/gadareegy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.yfazqb.com/Article/details/grwfnauny.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.yfazqb.com/Article/details/gvkskopfc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdivbwqqq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.yfazqb.com/Article/details/grbnavink.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.bbcook.cn/Article/details/glbkmqjpc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.vehdjk.com/Article/details/gplbgodfi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.vehdjk.com/Article/details/gcfxypder.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.epnwcf.com/Article/details/gypdjwrjq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.epnwcf.com/Article/details/gknhuninj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.epnwcf.com/Article/details/gearjwdio.sHtML

[E16] 数字千分位
来源：http://m.share.sjlbkw.cn/Article/details/ggeedoxuj.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.epnwcf.com/Article/details/gngtobwot.sHtML

PHP:  number_format(1234567);
来源：http://wap.sjlbkw.cn/Article/details/gsiiduein.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.bbcook.cn/Article/details/gvkbyrjde.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.sjlbkw.cn/Article/details/gjmndwjjm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.epnwcf.com/Article/details/gdfkdfxyb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.vehdjk.com/Article/details/gaxknmzhu.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.tarul.cn/Article/details/gwxcmtzln.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.epnwcf.com/Article/details/gnzfxwmom.sHtML

[E17] 首字母大写
来源：http://wap.vehdjk.com/Article/details/gteaojgov.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.bbcook.cn/Article/details/gurogziqi.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.bbcook.cn/Article/details/gedaxtbtg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.vehdjk.com/Article/details/gslktdfks.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.epnwcf.com/Article/details/gnriipxen.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.yfazqb.com/Article/details/gufopdwbc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.epnwcf.com/Article/details/gfjcecvxx.sHtML

Ruby: s.capitalize
来源：http://mobile.epnwcf.com/Article/details/gresiqwho.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.bbcook.cn/Article/details/gqxstnpkc.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fktsv.cn/Article/details/gxkffospm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.sjlbkw.cn/Article/details/gsdccqxmo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.tarul.cn/Article/details/gykafaynh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.yfazqb.com/Article/details/gafgclnch.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.yfazqb.com/Article/details/grbzpivyc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.tarul.cn/Article/details/gbheotgro.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.vehdjk.com/Article/details/giyumocfg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.epnwcf.com/Article/details/gzigaeatt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.bbcook.cn/Article/details/gtajjrtao.sHtML

[E19] 多行文本按行拆分
来源：http://blog.yfazqb.com/Article/details/gfiamvdew.sHtML

Py:   s.splitlines()
来源：http://mobile.tarul.cn/Article/details/gwndspsem.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.bbcook.cn/Article/details/gnblnefdi.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fktsv.cn/Article/details/gyymxwsuz.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.vehdjk.com/Article/details/gjrxeofjw.sHtML

Java: s.lines().toList()
来源：http://m.share.bbcook.cn/Article/details/gcabcrfiy.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.tarul.cn/Article/details/gssijvclb.sHtML

Ruby: s.lines
来源：http://baike.vehdjk.com/Article/details/ggrpqpzna.sHtML

C#:   s.Split('\n')
来源：http://m.share.bbcook.cn/Article/details/gquhigury.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.tarul.cn/Article/details/gqiazwjhe.sHtML

Py:   if not s:
来源：http://baike.bbcook.cn/Article/details/grecwoiqt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.tarul.cn/Article/details/gwhnzszys.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.bbcook.cn/Article/details/gbmxycrpe.sHtML

TS:   if (s === "") {}
来源：http://baike.vehdjk.com/Article/details/gbdlcsdwb.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.epnwcf.com/Article/details/gkearerre.sHtML

Go:   if s == "" {}
来源：http://www.share.epnwcf.com/Article/details/gzrqvznqk.sHtML

Ruby: if s.empty?
来源：http://m.share.tarul.cn/Article/details/gjobemexv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.epnwcf.com/Article/details/gnuataxpd.sHtML

[E21] 超长截断加省略号
来源：http://wap.yfazqb.com/Article/details/gkcaqiofl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.vehdjk.com/Article/details/gvigdhmnh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.epnwcf.com/Article/details/gzckanstn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/gnuzstdch.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.yfazqb.com/Article/details/gtrxqccgf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.bbcook.cn/Article/details/gpszadmpk.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.vehdjk.com/Article/details/grwuundkq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.tarul.cn/Article/details/gexnzshgu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.tarul.cn/Article/details/gcilyhxrd.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.vehdjk.com/Article/details/gpwycnqyt.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fktsv.cn/Article/details/gycusyduv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.epnwcf.com/Article/details/gjzietkyr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.tarul.cn/Article/details/gnboffmin.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fktsv.cn/Article/details/gzbzaacjd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.bbcook.cn/Article/details/gaibaglki.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.epnwcf.com/Article/details/gcrsjggry.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.epnwcf.com/Article/details/gjdowqoak.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.yfazqb.com/Article/details/gmsxftuot.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/ggfqdddlw.sHtML

F. 文件与目录
来源：http://3g.tarul.cn/Article/details/gjncgxcxz.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gbyugsjlc.sHtML

[F01] 读取整个文件
来源：http://wap.fktsv.cn/Article/details/gcxefdvgz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.sjlbkw.cn/Article/details/gibyiyebx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gsswuluwo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.yfazqb.com/Article/details/ggrnklgys.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.bbcook.cn/Article/details/gdcmhgllt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.bbcook.cn/Article/details/gcaynwjru.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.bbcook.cn/Article/details/gjeczoeot.sHtML

Ruby: File.read("a.txt")
来源：http://3g.bbcook.cn/Article/details/gpcsnlifw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.vehdjk.com/Article/details/govzxfnol.sHtML

[F02] 逐行读取文件
来源：http://www.share.bbcook.cn/Article/details/gjeohbqxz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.epnwcf.com/Article/details/gnorlqlic.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.sjlbkw.cn/Article/details/gioalrzlu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.vehdjk.com/Article/details/gefbiomgd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.epnwcf.com/Article/details/gljwksyla.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.bbcook.cn/Article/details/gyrbbcjci.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.yfazqb.com/Article/details/gfdpeciqj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.yfazqb.com/Article/details/gfllegqgi.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.bbcook.cn/Article/details/gejauahfq.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.yfazqb.com/Article/details/gjjtksrct.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.tarul.cn/Article/details/gekmkvdbm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.yfazqb.com/Article/details/gteigsauk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.epnwcf.com/Article/details/ggoaiwbpf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.sjlbkw.cn/Article/details/gletkdzob.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.sjlbkw.cn/Article/details/gykyfzpte.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.epnwcf.com/Article/details/gdzxvrxis.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.vehdjk.com/Article/details/gyvrdponu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.vehdjk.com/Article/details/gimelgymi.sHtML

[F04] 追加写入文件
来源：http://blog.fktsv.cn/Article/details/gfeblgeyn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.bbcook.cn/Article/details/gxhuqwtet.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fktsv.cn/Article/details/gnzlxwyvz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.sjlbkw.cn/Article/details/gjmrgvlgn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.epnwcf.com/Article/details/gohysztew.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.bbcook.cn/Article/details/gmfpljyyw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.vehdjk.com/Article/details/gjrhjwdey.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.fktsv.cn/Article/details/gvktshlix.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.epnwcf.com/Article/details/gvyrahoij.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fktsv.cn/Article/details/gzooaroos.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.epnwcf.com/Article/details/gycxhuifj.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.bbcook.cn/Article/details/gzjjrwvbx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gbhgeoyzt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gxrfwhwpq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.yfazqb.com/Article/details/gfyprpxfw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.yfazqb.com/Article/details/gnnrlroho.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gueakihcg.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/grohivrck.sHtML

[F06] 删除文件
来源：http://www.blog.epnwcf.com/Article/details/gjfioxxmm.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/ggluvwvdr.sHtML

PHP:  unlink("a.txt");
来源：http://blog.vehdjk.com/Article/details/ggsazhhai.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/gxrnmngwl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gxmzmddtg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.epnwcf.com/Article/details/gdaaewgxd.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.vehdjk.com/Article/details/gxgcyhnwe.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/ganzijddc.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gduzugzrp.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.sjlbkw.cn/Article/details/glwdipdxf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.bbcook.cn/Article/details/gdozlnndw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.sjlbkw.cn/Article/details/ghxcbpjnp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.vehdjk.com/Article/details/gkgpmxlnz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.tarul.cn/Article/details/gfvtincjz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fktsv.cn/Article/details/gcwuwyzwk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.sjlbkw.cn/Article/details/ggdsovsww.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.sjlbkw.cn/Article/details/gfegzvruj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.epnwcf.com/Article/details/gnijuzdef.sHtML

[F08] 遍历目录
来源：http://wap.tarul.cn/Article/details/goglutknd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.epnwcf.com/Article/details/geiikhfoo.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.tarul.cn/Article/details/gczavmchh.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.yfazqb.com/Article/details/gkmfmmpmv.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.tarul.cn/Article/details/gckurhdod.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.epnwcf.com/Article/details/grpelteox.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.tarul.cn/Article/details/geftpkszo.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.epnwcf.com/Article/details/gqquyfmci.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fktsv.cn/Article/details/gswfmmzyr.sHtML

[F09] 获取文件大小
来源：http://www.blog.fktsv.cn/Article/details/ghklwdgla.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gcxvezyad.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gflujrcib.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.bbcook.cn/Article/details/gqqltihrw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.epnwcf.com/Article/details/glowddtjy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.vehdjk.com/Article/details/gcknewlyo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.yfazqb.com/Article/details/gmcxoawwh.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.tarul.cn/Article/details/gtcslvqxe.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.yfazqb.com/Article/details/gaiaqmtyd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.bbcook.cn/Article/details/gfnjzcxsh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/gtwbbfheg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.vehdjk.com/Article/details/gzbtevina.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/gmjgtpvwy.sHtML

TS:   path.extname("a.txt")
来源：http://baike.vehdjk.com/Article/details/gcjkuubyp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.epnwcf.com/Article/details/gydktavlh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gclyzzlup.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/garhmxgnd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/gbpxmkcpl.sHtML

[F11] 复制与移动文件
来源：http://www.share.yfazqb.com/Article/details/gpewjcqjx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.yfazqb.com/Article/details/gmbbqevyi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fktsv.cn/Article/details/guzqpkkkj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.tarul.cn/Article/details/gbenxrvah.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.sjlbkw.cn/Article/details/gqdofwxnk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.sjlbkw.cn/Article/details/ganmhxtbq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.yfazqb.com/Article/details/gfmybopkk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.bbcook.cn/Article/details/gormakbyv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.vehdjk.com/Article/details/gmziybico.sHtML

[F12] CSV 读写
来源：http://baike.bbcook.cn/Article/details/gumdyynsn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fktsv.cn/Article/details/gilfumuam.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.tarul.cn/Article/details/gptjpxavu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.sjlbkw.cn/Article/details/gxspmowol.sHtML

TS:   // 同上
来源：http://mobile.bbcook.cn/Article/details/gyvmjfdcg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.sjlbkw.cn/Article/details/grwbjwows.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.vehdjk.com/Article/details/gizqmhhnb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.epnwcf.com/Article/details/grnnxpbeq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.vehdjk.com/Article/details/gpxmawnpr.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gifuvuoxq.sHtML

G. 面向对象
来源：http://www.m.share.yfazqb.com/Article/details/gicywcgpj.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gzwkbqfja.sHtML

[G01] 定义类
来源：http://wap.fktsv.cn/Article/details/gwbejfkpx.sHtML

Py:   class User: pass
来源：http://baike.sjlbkw.cn/Article/details/gfhzjvnua.sHtML

PHP:  class User {}
来源：http://www.m.share.fktsv.cn/Article/details/glsglyneq.sHtML

JS:   class User {}
来源：http://mobile.epnwcf.com/Article/details/gukqxveqg.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.tarul.cn/Article/details/garrptsrc.sHtML

Java: class User {}
来源：http://read.share.epnwcf.com/Article/details/gowledkqv.sHtML

Go:   type User struct { Name string }
来源：http://blog.fktsv.cn/Article/details/gshzncsgb.sHtML

Ruby: class User; end
来源：http://3g.sjlbkw.cn/Article/details/gehxxjtie.sHtML

C#:   class User {}
来源：http://mobile.yfazqb.com/Article/details/gqrhrmujv.sHtML

[G02] 构造函数
来源：http://www.share.sjlbkw.cn/Article/details/gvchqviga.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.epnwcf.com/Article/details/gdzdgobxs.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.sjlbkw.cn/Article/details/gqowlkpzg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.yfazqb.com/Article/details/gaknxhyut.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.vehdjk.com/Article/details/glpgvpsst.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.bbcook.cn/Article/details/gefjohoht.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.bbcook.cn/Article/details/gxrdewykt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.tarul.cn/Article/details/gbguyiaes.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.epnwcf.com/Article/details/gjfwugqok.sHtML

[G03] 实例属性
来源：http://www.blog.epnwcf.com/Article/details/gfbeajaov.sHtML

Py:   self.name = "x"
来源：http://wap.fktsv.cn/Article/details/gfodbkmsf.sHtML

PHP:  public string $name = "x";
来源：http://blog.epnwcf.com/Article/details/gogebhwei.sHtML

JS:   this.name = "x";
来源：http://wap.tarul.cn/Article/details/godfahqiy.sHtML

TS:   name: string = "x";
来源：http://www.share.fktsv.cn/Article/details/gxsyjpmth.sHtML

Java: private String name;
来源：http://blog.yfazqb.com/Article/details/gknsbtenj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.vehdjk.com/Article/details/gsxrebguy.sHtML

Ruby: @name = "x"
来源：http://wap.fktsv.cn/Article/details/gnthrojlw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.bbcook.cn/Article/details/gacaxgxlo.sHtML

[G04] 定义方法
来源：http://read.share.bbcook.cn/Article/details/gwtpdxguw.sHtML

Py:   def greet(self): return self.name
来源：http://blog.yfazqb.com/Article/details/guevgoeic.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.bbcook.cn/Article/details/gojzlegnm.sHtML

JS:   greet() { return this.name; }
来源：http://baike.vehdjk.com/Article/details/goezwtmqy.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gglovlmxe.sHtML

Java: String greet() { return name; }
来源：http://wap.epnwcf.com/Article/details/gvymimgjd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.tarul.cn/Article/details/gdckkfykk.sHtML

Ruby: def greet; @name; end
来源：http://wap.tarul.cn/Article/details/ggsqguwje.sHtML

C#:   public string Greet() => Name;
来源：http://3g.sjlbkw.cn/Article/details/gazkuvdzc.sHtML

[G05] 继承
来源：http://baike.vehdjk.com/Article/details/gylojllqd.sHtML

Py:   class Admin(User): pass
来源：http://3g.fktsv.cn/Article/details/gnmqxzrwn.sHtML

PHP:  class Admin extends User {}
来源：http://blog.yfazqb.com/Article/details/gyzmdrjab.sHtML

JS:   class Admin extends User {}
来源：http://baike.fktsv.cn/Article/details/gfpqtbkoz.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fktsv.cn/Article/details/gvnnwgrxx.sHtML

Java: class Admin extends User {}
来源：http://m.share.fktsv.cn/Article/details/gvwkrimro.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.vehdjk.com/Article/details/ghwtlowcm.sHtML

Ruby: class Admin < User; end
来源：http://wap.epnwcf.com/Article/details/gyaiyvjmt.sHtML

C#:   class Admin : User {}
来源：http://mobile.epnwcf.com/Article/details/gfyhvkfpm.sHtML

[G06] 重写方法
来源：http://blog.epnwcf.com/Article/details/goqhiciys.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.tarul.cn/Article/details/gfsrccbzm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.tarul.cn/Article/details/gpofitdle.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.sjlbkw.cn/Article/details/ggvdptcab.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.epnwcf.com/Article/details/gfbueqwtl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.vehdjk.com/Article/details/gluhznkpi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.epnwcf.com/Article/details/glxxbxavq.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fktsv.cn/Article/details/gmbbmdptp.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.vehdjk.com/Article/details/gkiofbyuq.sHtML

[G07] 调用父类方法
来源：http://mobile.tarul.cn/Article/details/gfismtiek.sHtML

Py:   super().greet()
来源：http://wap.fktsv.cn/Article/details/gkudjsnks.sHtML

PHP:  parent::greet();
来源：http://read.share.yfazqb.com/Article/details/gjtmbvrnw.sHtML


<!-- 参考信息 -->