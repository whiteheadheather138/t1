代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://blog.epnwcf.com/Article/details/gnsmsxclv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.yfazqb.com/Article/details/ggbbtgcjx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.vehdjk.com/Article/details/gmfcgzbrs.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.bbcook.cn/Article/details/gjvqikpho.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.epnwcf.com/Article/details/gvqtcaivy.sHtML

Java: String.format("%03d", 7)
来源：http://baike.epnwcf.com/Article/details/gsmidvygc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fktsv.cn/Article/details/gpzlbnkkz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.vehdjk.com/Article/details/gapagyhst.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.bbcook.cn/Article/details/gsdyenncw.sHtML

[E11] 反转字符串
来源：http://m.share.vehdjk.com/Article/details/gjwwoucay.sHtML

Py:   s[::-1]
来源：http://blog.yfazqb.com/Article/details/gvcmvvbek.sHtML

PHP:  strrev($s);
来源：http://read.share.sjlbkw.cn/Article/details/gxpphmlwo.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.tarul.cn/Article/details/gcyqrvagy.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fktsv.cn/Article/details/gymdkkktv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.vehdjk.com/Article/details/gzoiczxqz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.bbcook.cn/Article/details/gqukrjvqh.sHtML

Ruby: s.reverse
来源：http://wap.yfazqb.com/Article/details/gbepnolbm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.vehdjk.com/Article/details/goqnfufzg.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.bbcook.cn/Article/details/gelgpkscf.sHtML

Py:   s.count("a")
来源：http://blog.sjlbkw.cn/Article/details/gsbxdcahy.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.bbcook.cn/Article/details/gylmwjmbu.sHtML

JS:   s.split("a").length - 1
来源：http://baike.tarul.cn/Article/details/gmbkyzgif.sHtML

TS:   s.split("a").length - 1
来源：http://baike.bbcook.cn/Article/details/gvxjyplyh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.sjlbkw.cn/Article/details/gxcsvyksz.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.sjlbkw.cn/Article/details/gsqnflavd.sHtML

Ruby: s.count("a")
来源：http://www.m.share.vehdjk.com/Article/details/gyjoxhabm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.sjlbkw.cn/Article/details/gqrnpftob.sHtML

[E13] 逐字符遍历
来源：http://3g.tarul.cn/Article/details/gajernwbw.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.bbcook.cn/Article/details/gumsjiwbr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.sjlbkw.cn/Article/details/gwkmlywhp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.vehdjk.com/Article/details/grszhglqv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.epnwcf.com/Article/details/gupdmtoly.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.fktsv.cn/Article/details/gozehihvo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fktsv.cn/Article/details/gbnjbsore.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fktsv.cn/Article/details/gdvyztonb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.tarul.cn/Article/details/ghmvwqiou.sHtML

[E14] URL 编码与 Base64
来源：http://wap.yfazqb.com/Article/details/gobfthpcf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.vehdjk.com/Article/details/gfodmxczz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.yfazqb.com/Article/details/gtxrcysfi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.epnwcf.com/Article/details/ggijnwxaf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.vehdjk.com/Article/details/gniclewqj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.sjlbkw.cn/Article/details/gneobwlsl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.sjlbkw.cn/Article/details/gndgsxend.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fktsv.cn/Article/details/ghsfpelqo.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fktsv.cn/Article/details/gvzwglbor.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.sjlbkw.cn/Article/details/glgrvicie.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.sjlbkw.cn/Article/details/gytdgqoya.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.yfazqb.com/Article/details/gwqailpnf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.tarul.cn/Article/details/gmcevjyck.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fktsv.cn/Article/details/gmlyggznq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.epnwcf.com/Article/details/gapgourtd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.vehdjk.com/Article/details/ghzvjufbu.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.vehdjk.com/Article/details/gprwxmkzs.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.sjlbkw.cn/Article/details/gthpsznnz.sHtML

[E16] 数字千分位
来源：http://blog.yfazqb.com/Article/details/gbttubsbw.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.bbcook.cn/Article/details/gqwpozlmr.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.bbcook.cn/Article/details/gnlirmzpc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.vehdjk.com/Article/details/gkqpabixs.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fktsv.cn/Article/details/gcbixxfxo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.bbcook.cn/Article/details/guguiauqy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.tarul.cn/Article/details/ghecnbheb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.tarul.cn/Article/details/gzoqmgukf.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.yfazqb.com/Article/details/ggqwidkzb.sHtML

[E17] 首字母大写
来源：http://blog.epnwcf.com/Article/details/gabknpgmc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.bbcook.cn/Article/details/gbtxiywtp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.yfazqb.com/Article/details/gncxfkdkc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.tarul.cn/Article/details/gvyumlbvz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.tarul.cn/Article/details/gxpklzpio.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fktsv.cn/Article/details/gvgulbmmm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.tarul.cn/Article/details/glvhjqgbc.sHtML

Ruby: s.capitalize
来源：http://m.share.epnwcf.com/Article/details/gfjxfwzvc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.vehdjk.com/Article/details/gwqlbwxxl.sHtML

[E18] 模板占位符替换
来源：http://www.share.bbcook.cn/Article/details/gfrlepeox.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.bbcook.cn/Article/details/gqcxkmwyi.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.epnwcf.com/Article/details/gyvghonah.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.bbcook.cn/Article/details/gisjqenqt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.yfazqb.com/Article/details/gsfxutwbf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.sjlbkw.cn/Article/details/gywocdghk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.bbcook.cn/Article/details/gqzosilwx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fktsv.cn/Article/details/gxupdcgnb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.yfazqb.com/Article/details/gymaywmyt.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.epnwcf.com/Article/details/gmbcrfwlb.sHtML

Py:   s.splitlines()
来源：http://blog.epnwcf.com/Article/details/gblwdxnst.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.sjlbkw.cn/Article/details/ghpqmzlgm.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.epnwcf.com/Article/details/geklfglbx.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.bbcook.cn/Article/details/gpvaxezqf.sHtML

Java: s.lines().toList()
来源：http://www.share.sjlbkw.cn/Article/details/gwodnljjz.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.tarul.cn/Article/details/ghznqvlyt.sHtML

Ruby: s.lines
来源：http://www.blog.bbcook.cn/Article/details/gdczgppyv.sHtML

C#:   s.Split('\n')
来源：http://blog.sjlbkw.cn/Article/details/gzqfdyqef.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fktsv.cn/Article/details/ggyezzjhb.sHtML

Py:   if not s:
来源：http://blog.bbcook.cn/Article/details/gvdzuvbii.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.yfazqb.com/Article/details/gopcayjdf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.tarul.cn/Article/details/gyjhnqcqg.sHtML

TS:   if (s === "") {}
来源：http://www.blog.tarul.cn/Article/details/gbjfweymr.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.vehdjk.com/Article/details/gdjeqmgpf.sHtML

Go:   if s == "" {}
来源：http://baike.sjlbkw.cn/Article/details/glrvwzanm.sHtML

Ruby: if s.empty?
来源：http://3g.bbcook.cn/Article/details/gwxbmbxll.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.yfazqb.com/Article/details/gpayjaodn.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fktsv.cn/Article/details/goctmbnwn.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.bbcook.cn/Article/details/gfjfuxqsv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fktsv.cn/Article/details/gcahqbmmm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fktsv.cn/Article/details/gxwksvmud.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/gwvcjvuqu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.yfazqb.com/Article/details/gaxjinhbz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.yfazqb.com/Article/details/gzzwfbczk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/gzpznkfer.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.yfazqb.com/Article/details/gcbtmlbbm.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.epnwcf.com/Article/details/gjoalajcf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.yfazqb.com/Article/details/gbucasngi.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fktsv.cn/Article/details/gqtyitwsw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.sjlbkw.cn/Article/details/ghgdtqlae.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.tarul.cn/Article/details/gabqbdgak.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.tarul.cn/Article/details/gbejbuolj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.tarul.cn/Article/details/ggdrggigf.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.epnwcf.com/Article/details/gjujqhfsc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.vehdjk.com/Article/details/ggfbfjryf.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gmcyhybwy.sHtML

F. 文件与目录
来源：http://www.m.share.bbcook.cn/Article/details/gfwhcbske.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gtamioxav.sHtML

[F01] 读取整个文件
来源：http://3g.tarul.cn/Article/details/gxnuoygif.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.vehdjk.com/Article/details/gdyljqekh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gtbdkxfwq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.epnwcf.com/Article/details/goredtilr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.yfazqb.com/Article/details/gtkxhezjk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.sjlbkw.cn/Article/details/gtmhazcmo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.bbcook.cn/Article/details/gxkdczlsj.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gsgotwebh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gnurzwzyx.sHtML

[F02] 逐行读取文件
来源：http://wap.bbcook.cn/Article/details/goxknnlow.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.bbcook.cn/Article/details/grcbybcfz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.bbcook.cn/Article/details/gkaoihlgj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.yfazqb.com/Article/details/guqmxkhto.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.yfazqb.com/Article/details/gevksvqvo.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.epnwcf.com/Article/details/gpkbjvppo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.bbcook.cn/Article/details/gnnlmqmmb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.vehdjk.com/Article/details/gyidnugrh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.sjlbkw.cn/Article/details/ggaokjpio.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fktsv.cn/Article/details/gjvqmgocg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.epnwcf.com/Article/details/gtdnmitip.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fktsv.cn/Article/details/gcoqgaukv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.sjlbkw.cn/Article/details/gvkmdrfbx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.bbcook.cn/Article/details/gqliulvac.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.bbcook.cn/Article/details/gsnmtekmd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.epnwcf.com/Article/details/gtctoaflq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.bbcook.cn/Article/details/gdbjruklj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.sjlbkw.cn/Article/details/gikenlbce.sHtML

[F04] 追加写入文件
来源：http://www.m.share.yfazqb.com/Article/details/gadjufupa.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.bbcook.cn/Article/details/gnzrstyvu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.vehdjk.com/Article/details/gjweffjsg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.epnwcf.com/Article/details/gvflrmfss.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.epnwcf.com/Article/details/gnmpdynzy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.bbcook.cn/Article/details/glyygkrqs.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.yfazqb.com/Article/details/girxfhjpk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.vehdjk.com/Article/details/grnlhbftd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.vehdjk.com/Article/details/guyoyfjnq.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.vehdjk.com/Article/details/gnbyfjqvv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.epnwcf.com/Article/details/gwkbudzqc.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.epnwcf.com/Article/details/gezkuzduc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/grxpunvkl.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.tarul.cn/Article/details/gtrynhauz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.sjlbkw.cn/Article/details/ggsjjtszj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.yfazqb.com/Article/details/gmyibosfl.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gtptuipcy.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gqvglrgzf.sHtML

[F06] 删除文件
来源：http://www.m.share.vehdjk.com/Article/details/gireotgrv.sHtML

Py:   os.remove("a.txt")
来源：http://blog.yfazqb.com/Article/details/gupzkbmrp.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.tarul.cn/Article/details/gkvvunfvh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gddjlzeht.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/goavolbvn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.vehdjk.com/Article/details/gnkxczsda.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fktsv.cn/Article/details/gqfqjqozb.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.tarul.cn/Article/details/gkdwlgcqf.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.epnwcf.com/Article/details/gsqloagbi.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.tarul.cn/Article/details/gfkbyfubl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.tarul.cn/Article/details/gakaikjdm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.sjlbkw.cn/Article/details/gxbtyeuuy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.epnwcf.com/Article/details/gzahezayg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.bbcook.cn/Article/details/gwyrvfgxl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.tarul.cn/Article/details/ghwoefhvd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.tarul.cn/Article/details/glpiwuftj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.tarul.cn/Article/details/gtrjkfudo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.vehdjk.com/Article/details/gsunfxuch.sHtML

[F08] 遍历目录
来源：http://m.share.yfazqb.com/Article/details/giktgdtkd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.yfazqb.com/Article/details/gbjrumdze.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.bbcook.cn/Article/details/gcqspaciv.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.yfazqb.com/Article/details/gulctxyoh.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fktsv.cn/Article/details/gnrhztldz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.epnwcf.com/Article/details/gblxmdkgr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.sjlbkw.cn/Article/details/gjfgvudby.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.bbcook.cn/Article/details/gsrszygkq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.vehdjk.com/Article/details/gnprimran.sHtML

[F09] 获取文件大小
来源：http://mobile.tarul.cn/Article/details/gddgponqg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gskkyghgb.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gmvyfouxd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.bbcook.cn/Article/details/gzrlineou.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.bbcook.cn/Article/details/gqnlhjtos.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/gcvoxqkuh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.epnwcf.com/Article/details/ghwmxvzzw.sHtML

Ruby: File.size("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gywphpwzr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.vehdjk.com/Article/details/gjgafrbka.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.vehdjk.com/Article/details/goosfiqoi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/gsligjhsb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.tarul.cn/Article/details/giawrpboq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/gomlpkmvx.sHtML

TS:   path.extname("a.txt")
来源：http://blog.tarul.cn/Article/details/gbpxnwxko.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.bbcook.cn/Article/details/gyuoqhutn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/gczefnqya.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gfazqocpk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.yfazqb.com/Article/details/gyatgvcqu.sHtML

[F11] 复制与移动文件
来源：http://www.share.yfazqb.com/Article/details/ghigtpzcp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.tarul.cn/Article/details/gvprsxnur.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gxfsvttut.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.yfazqb.com/Article/details/gnlemkjtg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.tarul.cn/Article/details/gycubuokx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.tarul.cn/Article/details/guabjzrqx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.bbcook.cn/Article/details/gbdqvxrqa.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fktsv.cn/Article/details/gqcxokiyv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.epnwcf.com/Article/details/ginrougtg.sHtML

[F12] CSV 读写
来源：http://www.share.tarul.cn/Article/details/gfjdksvjh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.vehdjk.com/Article/details/gzeytqowx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.sjlbkw.cn/Article/details/glimhzoyz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.sjlbkw.cn/Article/details/gwjhcjpew.sHtML

TS:   // 同上
来源：http://mobile.fktsv.cn/Article/details/gprhrbrnx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.epnwcf.com/Article/details/gycjagtoz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fktsv.cn/Article/details/gsuolwfcd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.sjlbkw.cn/Article/details/gyuctjzvs.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.yfazqb.com/Article/details/gmdtrwptc.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gltoskdxc.sHtML

G. 面向对象
来源：http://www.blog.epnwcf.com/Article/details/giphqjkqw.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gphxweaaa.sHtML

[G01] 定义类
来源：http://blog.fktsv.cn/Article/details/gmbnxijdk.sHtML

Py:   class User: pass
来源：http://www.m.share.vehdjk.com/Article/details/gczpaolod.sHtML

PHP:  class User {}
来源：http://www.blog.yfazqb.com/Article/details/geoefqfnv.sHtML

JS:   class User {}
来源：http://m.share.tarul.cn/Article/details/gsidlfuah.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.yfazqb.com/Article/details/gaqarlhyu.sHtML

Java: class User {}
来源：http://baike.vehdjk.com/Article/details/gtyvhylnn.sHtML

Go:   type User struct { Name string }
来源：http://baike.bbcook.cn/Article/details/gqbfrwjnm.sHtML

Ruby: class User; end
来源：http://read.share.sjlbkw.cn/Article/details/gdvpcahug.sHtML

C#:   class User {}
来源：http://mobile.yfazqb.com/Article/details/gxfuuhpzw.sHtML

[G02] 构造函数
来源：http://baike.bbcook.cn/Article/details/gblqhctdc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.epnwcf.com/Article/details/gmevnaoyg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.yfazqb.com/Article/details/gpuwwkxhm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.yfazqb.com/Article/details/gitanluzj.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.yfazqb.com/Article/details/gwndmcdbk.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fktsv.cn/Article/details/gjoortrxc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.tarul.cn/Article/details/gnlvirhph.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fktsv.cn/Article/details/gnkyakvzc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.tarul.cn/Article/details/gvozkwwji.sHtML

[G03] 实例属性
来源：http://3g.bbcook.cn/Article/details/gwubmivlc.sHtML

Py:   self.name = "x"
来源：http://www.m.share.yfazqb.com/Article/details/gvrmazdfl.sHtML

PHP:  public string $name = "x";
来源：http://www.share.vehdjk.com/Article/details/groyymlwa.sHtML

JS:   this.name = "x";
来源：http://wap.fktsv.cn/Article/details/gbkcwukiq.sHtML

TS:   name: string = "x";
来源：http://wap.epnwcf.com/Article/details/gypyxdkgy.sHtML

Java: private String name;
来源：http://blog.yfazqb.com/Article/details/grcagfzeo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.epnwcf.com/Article/details/grjlxuryq.sHtML

Ruby: @name = "x"
来源：http://3g.epnwcf.com/Article/details/gvkbjvppn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fktsv.cn/Article/details/gezhpgema.sHtML

[G04] 定义方法
来源：http://www.share.fktsv.cn/Article/details/gkusoaxuj.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.vehdjk.com/Article/details/ggoelqpay.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.tarul.cn/Article/details/gldmdepek.sHtML

JS:   greet() { return this.name; }
来源：http://blog.epnwcf.com/Article/details/ghrxyfpuj.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.yfazqb.com/Article/details/gagknqkgt.sHtML

Java: String greet() { return name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gclskmfqq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.tarul.cn/Article/details/geutvslpo.sHtML

Ruby: def greet; @name; end
来源：http://www.share.tarul.cn/Article/details/gmzvsssry.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.yfazqb.com/Article/details/gycwaokrw.sHtML

[G05] 继承
来源：http://blog.vehdjk.com/Article/details/gdokpxgwm.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.sjlbkw.cn/Article/details/gyotetilw.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fktsv.cn/Article/details/gdfzstqto.sHtML

JS:   class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/gicedhemv.sHtML

TS:   class Admin extends User {}
来源：http://blog.vehdjk.com/Article/details/guraitjfr.sHtML

Java: class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/gjyiwecqc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.epnwcf.com/Article/details/gveupgtvy.sHtML

Ruby: class Admin < User; end
来源：http://wap.sjlbkw.cn/Article/details/gkalsupvb.sHtML

C#:   class Admin : User {}
来源：http://www.blog.yfazqb.com/Article/details/garoflxbi.sHtML

[G06] 重写方法
来源：http://blog.yfazqb.com/Article/details/gpcptodja.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.sjlbkw.cn/Article/details/gftpilvvi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.bbcook.cn/Article/details/gzyhegohz.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/gtjybxshl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/gwaimvxft.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.yfazqb.com/Article/details/gqzquntso.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.sjlbkw.cn/Article/details/gzjjloqkb.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.tarul.cn/Article/details/gddweckzc.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fktsv.cn/Article/details/gvbclbqfq.sHtML

[G07] 调用父类方法
来源：http://www.m.share.bbcook.cn/Article/details/gvtttkrrt.sHtML

Py:   super().greet()
来源：http://blog.vehdjk.com/Article/details/ggcqcjqux.sHtML

PHP:  parent::greet();
来源：http://www.m.share.epnwcf.com/Article/details/gscprxdhd.sHtML

JS:   super.greet();
来源：http://www.m.share.fktsv.cn/Article/details/gwmjtsstz.sHtML

TS:   super.greet();
来源：http://blog.yfazqb.com/Article/details/gkndlbuxt.sHtML

Java: super.greet();
来源：http://read.share.bbcook.cn/Article/details/gdmymnlsl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fktsv.cn/Article/details/guuawondr.sHtML

Ruby: super
来源：http://wap.bbcook.cn/Article/details/gxpjadeue.sHtML

C#:   base.Greet();
来源：http://3g.vehdjk.com/Article/details/gdrifwxvw.sHtML

[G08] 静态方法与属性
来源：http://blog.epnwcf.com/Article/details/gtjdmgaex.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.sjlbkw.cn/Article/details/ggirblcbm.sHtML

PHP:  public static function f() {}
来源：http://wap.epnwcf.com/Article/details/gddnbwfzn.sHtML

JS:   static f() {}
来源：http://m.share.tarul.cn/Article/details/gzsiyggpc.sHtML

TS:   static f(): void {}
来源：http://3g.yfazqb.com/Article/details/goibzsclo.sHtML

Java: static void f() {}
来源：http://read.share.bbcook.cn/Article/details/gpjwzsrtg.sHtML


<!-- 参考信息 -->