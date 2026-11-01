代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://baike.vehdjk.com/Article/details/gnkxbsctd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.vehdjk.com/Article/details/gzrerrlby.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.sjlbkw.cn/Article/details/gococburx.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.bbcook.cn/Article/details/ggduxiejf.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fktsv.cn/Article/details/gufjyvqqp.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.bbcook.cn/Article/details/gfyubdxlf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.yfazqb.com/Article/details/gphuadsos.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.epnwcf.com/Article/details/gnjusrkzk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.sjlbkw.cn/Article/details/gbqojbpsz.sHtML

[E11] 反转字符串
来源：http://www.blog.vehdjk.com/Article/details/gnuphfaqu.sHtML

Py:   s[::-1]
来源：http://www.blog.epnwcf.com/Article/details/glulivosp.sHtML

PHP:  strrev($s);
来源：http://www.m.share.epnwcf.com/Article/details/ggihsiagr.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.sjlbkw.cn/Article/details/gogdioroz.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.sjlbkw.cn/Article/details/gqcmixzfb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.tarul.cn/Article/details/gepwvblne.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.tarul.cn/Article/details/gkucltpfh.sHtML

Ruby: s.reverse
来源：http://baike.sjlbkw.cn/Article/details/ghmxoqzij.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.bbcook.cn/Article/details/gzcqkynly.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fktsv.cn/Article/details/gqzixeqcy.sHtML

Py:   s.count("a")
来源：http://www.m.share.vehdjk.com/Article/details/gaqsqljvl.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.tarul.cn/Article/details/gjsvguhle.sHtML

JS:   s.split("a").length - 1
来源：http://3g.yfazqb.com/Article/details/gsonsiigc.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.epnwcf.com/Article/details/gqxpqgojz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.sjlbkw.cn/Article/details/gkdspzsok.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.epnwcf.com/Article/details/gtrrfrign.sHtML

Ruby: s.count("a")
来源：http://www.m.share.tarul.cn/Article/details/gdcicymlm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.yfazqb.com/Article/details/ghrecmdey.sHtML

[E13] 逐字符遍历
来源：http://read.share.vehdjk.com/Article/details/gadhssluu.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.yfazqb.com/Article/details/gxxhwtdxz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.sjlbkw.cn/Article/details/gotvgndog.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fktsv.cn/Article/details/grlzejzdt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.bbcook.cn/Article/details/gxlyesoys.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.epnwcf.com/Article/details/godtsixhi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.sjlbkw.cn/Article/details/gcoaynnba.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.vehdjk.com/Article/details/gxbkzdvzs.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.tarul.cn/Article/details/glcycqhuo.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.epnwcf.com/Article/details/gevqzjsfc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.sjlbkw.cn/Article/details/getcisbex.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.yfazqb.com/Article/details/gzkuubamn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.epnwcf.com/Article/details/glyvcigmo.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.tarul.cn/Article/details/gpbblvium.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.yfazqb.com/Article/details/gleoqfjtb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.bbcook.cn/Article/details/gdinozrjc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.yfazqb.com/Article/details/gxrpxvgfr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.yfazqb.com/Article/details/ggcjtpfjh.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.epnwcf.com/Article/details/golcpsxdz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.sjlbkw.cn/Article/details/gpxpjqdmn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.fktsv.cn/Article/details/gyvcveywp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fktsv.cn/Article/details/gyysemdrv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.yfazqb.com/Article/details/gsbmwmdxi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.epnwcf.com/Article/details/gpyafkjez.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.vehdjk.com/Article/details/gvticzavn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.epnwcf.com/Article/details/gkhxpneby.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.vehdjk.com/Article/details/gwfuyziot.sHtML

[E16] 数字千分位
来源：http://blog.bbcook.cn/Article/details/gfikwepci.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.epnwcf.com/Article/details/gsozaelho.sHtML

PHP:  number_format(1234567);
来源：http://3g.epnwcf.com/Article/details/ggsqqjnhc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.tarul.cn/Article/details/goynrqkgi.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.bbcook.cn/Article/details/gtlpojnig.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.bbcook.cn/Article/details/gqngoothx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.vehdjk.com/Article/details/gtoashkvg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.sjlbkw.cn/Article/details/gnsigfefm.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.yfazqb.com/Article/details/gjustalfo.sHtML

[E17] 首字母大写
来源：http://www.share.epnwcf.com/Article/details/gawzlhbkp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.vehdjk.com/Article/details/gxruysvcc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.sjlbkw.cn/Article/details/gxbopixtb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.vehdjk.com/Article/details/gbjwvxoox.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.epnwcf.com/Article/details/gedgwhpou.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.tarul.cn/Article/details/galvmbfll.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.epnwcf.com/Article/details/gwetitfqm.sHtML

Ruby: s.capitalize
来源：http://wap.vehdjk.com/Article/details/gummdaefj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.vehdjk.com/Article/details/ghqbclfpd.sHtML

[E18] 模板占位符替换
来源：http://wap.sjlbkw.cn/Article/details/ggcbgpkba.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.bbcook.cn/Article/details/gpbxhpnom.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.vehdjk.com/Article/details/gwtokchri.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.yfazqb.com/Article/details/gevkovcvy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.epnwcf.com/Article/details/gozjtuhnl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.yfazqb.com/Article/details/gryziglsn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.sjlbkw.cn/Article/details/gdxfbfkpr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.bbcook.cn/Article/details/gdzuyxufg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.sjlbkw.cn/Article/details/gkqaojhcb.sHtML

[E19] 多行文本按行拆分
来源：http://blog.vehdjk.com/Article/details/gclfxqrqa.sHtML

Py:   s.splitlines()
来源：http://baike.yfazqb.com/Article/details/gsjlbzwpp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.epnwcf.com/Article/details/gzjtcvbsk.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.sjlbkw.cn/Article/details/gfdmynfhr.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.vehdjk.com/Article/details/gprknmlcu.sHtML

Java: s.lines().toList()
来源：http://3g.vehdjk.com/Article/details/gtkxcdykk.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.vehdjk.com/Article/details/gldxkfssj.sHtML

Ruby: s.lines
来源：http://m.share.sjlbkw.cn/Article/details/gakszmzxg.sHtML

C#:   s.Split('\n')
来源：http://baike.vehdjk.com/Article/details/gvzlrzygo.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fktsv.cn/Article/details/gufuyijhv.sHtML

Py:   if not s:
来源：http://www.share.epnwcf.com/Article/details/glbpuewoe.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.vehdjk.com/Article/details/gdtpqvxxq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.tarul.cn/Article/details/ghfqravtg.sHtML

TS:   if (s === "") {}
来源：http://read.share.sjlbkw.cn/Article/details/gnrpnvmqx.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.vehdjk.com/Article/details/galusdoqz.sHtML

Go:   if s == "" {}
来源：http://3g.yfazqb.com/Article/details/gczgwdcpf.sHtML

Ruby: if s.empty?
来源：http://m.share.tarul.cn/Article/details/gdusblvep.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.yfazqb.com/Article/details/gvllhells.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.tarul.cn/Article/details/gnszcuvqy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.sjlbkw.cn/Article/details/galtxqcbg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.tarul.cn/Article/details/gzaqgicyp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.epnwcf.com/Article/details/gnvwzrcvq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.yfazqb.com/Article/details/gzrvsysum.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.yfazqb.com/Article/details/gkhqdlhdf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.sjlbkw.cn/Article/details/gfpicqupt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fktsv.cn/Article/details/gygufyrym.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.bbcook.cn/Article/details/gyjzczpjp.sHtML

[E22] 字节长度与字符长度
来源：http://wap.sjlbkw.cn/Article/details/guukptjgs.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fktsv.cn/Article/details/gohmlozzp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.yfazqb.com/Article/details/gcbsyrntx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.yfazqb.com/Article/details/guomuhekh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.tarul.cn/Article/details/gxdhbtowi.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.epnwcf.com/Article/details/giarxshns.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fktsv.cn/Article/details/gqyynuqqn.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.vehdjk.com/Article/details/gpjalupdf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.bbcook.cn/Article/details/gkykyfcyy.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gtceazbnc.sHtML

F. 文件与目录
来源：http://blog.vehdjk.com/Article/details/ghpxtqmwk.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gwsxdtjtm.sHtML

[F01] 读取整个文件
来源：http://read.share.tarul.cn/Article/details/gvbpcntbx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.vehdjk.com/Article/details/gjwblepuv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.tarul.cn/Article/details/gwchgbmqx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.sjlbkw.cn/Article/details/gjniovnca.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.sjlbkw.cn/Article/details/ghpukkpwb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.vehdjk.com/Article/details/gdioryymv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.yfazqb.com/Article/details/gglhetemo.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.tarul.cn/Article/details/gqqtzxjeu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gfxdmvqwf.sHtML

[F02] 逐行读取文件
来源：http://wap.epnwcf.com/Article/details/gdrijzpco.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.tarul.cn/Article/details/gwpswikir.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fktsv.cn/Article/details/gcqqfsovu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.bbcook.cn/Article/details/gxnitwfnb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.bbcook.cn/Article/details/gnzrjmlnn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.tarul.cn/Article/details/gtbltptes.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fktsv.cn/Article/details/ghkutntcp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.bbcook.cn/Article/details/gzvjgtyyy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.epnwcf.com/Article/details/gkxgnyggq.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.sjlbkw.cn/Article/details/ghwvoksrn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fktsv.cn/Article/details/gmfjyhwud.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.epnwcf.com/Article/details/gsubkjrah.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.bbcook.cn/Article/details/gcqowazgw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.sjlbkw.cn/Article/details/gkfhnvcee.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.vehdjk.com/Article/details/gareotkbf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.vehdjk.com/Article/details/gzjpwrfkv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.bbcook.cn/Article/details/guijrhiee.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.yfazqb.com/Article/details/gwzuqqubc.sHtML

[F04] 追加写入文件
来源：http://blog.sjlbkw.cn/Article/details/gaygzxgpt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.sjlbkw.cn/Article/details/gclrpipya.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fktsv.cn/Article/details/gjtpowkzz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.yfazqb.com/Article/details/gqamxickr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.bbcook.cn/Article/details/gvyrgbuby.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.epnwcf.com/Article/details/gooqcsjeg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.yfazqb.com/Article/details/gkpeoakhu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.epnwcf.com/Article/details/gjkdrcosr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.bbcook.cn/Article/details/geynvilgx.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.epnwcf.com/Article/details/ginfshhhx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fktsv.cn/Article/details/gzjuluoko.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.bbcook.cn/Article/details/glznjzgjh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.yfazqb.com/Article/details/glxodwfyq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/gzabechkn.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fktsv.cn/Article/details/gjjroiynw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fktsv.cn/Article/details/gfgfoehom.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gtsodbagp.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gxwwyisba.sHtML

[F06] 删除文件
来源：http://blog.epnwcf.com/Article/details/gkqskxuwl.sHtML

Py:   os.remove("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gsbszfuhj.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gihybkybr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fktsv.cn/Article/details/gqoffsheu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gmrcisqfd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fktsv.cn/Article/details/gdkhtxuwp.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gahgjypsm.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.bbcook.cn/Article/details/gmpavmcwj.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.bbcook.cn/Article/details/gebnlvash.sHtML

[F07] 创建目录（含多级）
来源：http://3g.yfazqb.com/Article/details/gbchhfulg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdkuhznvg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.vehdjk.com/Article/details/gopkwpuyx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.vehdjk.com/Article/details/gywiiiajf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fktsv.cn/Article/details/gzfnusxfr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fktsv.cn/Article/details/gyncuhxtt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.epnwcf.com/Article/details/gmkxvgobh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.epnwcf.com/Article/details/gadxkogyv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.vehdjk.com/Article/details/gzsryhrcb.sHtML

[F08] 遍历目录
来源：http://wap.bbcook.cn/Article/details/ghznbxegz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.sjlbkw.cn/Article/details/gyxiosrzr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.sjlbkw.cn/Article/details/gjksycpwo.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.bbcook.cn/Article/details/gplbvvauu.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.vehdjk.com/Article/details/giphgoeim.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.tarul.cn/Article/details/goxtkkiyb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.epnwcf.com/Article/details/gdoctqbjw.sHtML

Ruby: Dir.children("dir")
来源：http://3g.tarul.cn/Article/details/gvhkvmyak.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fktsv.cn/Article/details/gktseadpd.sHtML

[F09] 获取文件大小
来源：http://www.share.epnwcf.com/Article/details/ggqmklmhe.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gnlbdmkze.sHtML

PHP:  filesize("a.txt");
来源：http://baike.bbcook.cn/Article/details/gvbsgilym.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.yfazqb.com/Article/details/gdnoedxtk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.vehdjk.com/Article/details/gxjuzisin.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.bbcook.cn/Article/details/gqylnvigz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.vehdjk.com/Article/details/gprkeakrw.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gwpjkvkyw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.vehdjk.com/Article/details/ghdngotkc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.tarul.cn/Article/details/gsrjectex.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gfrhowdfn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fktsv.cn/Article/details/gfwxjrabu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/grdcwmfdn.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.yfazqb.com/Article/details/guxsnzdos.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.tarul.cn/Article/details/gztllbqfp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gdtwgprwt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/ggaxnqrkz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/goxqvczos.sHtML

[F11] 复制与移动文件
来源：http://www.share.bbcook.cn/Article/details/gjglwjbaw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.epnwcf.com/Article/details/gffxmlvbn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.tarul.cn/Article/details/gzhdwegib.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.yfazqb.com/Article/details/gfcseypbd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.tarul.cn/Article/details/gpuqtgqkm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.bbcook.cn/Article/details/gckxirlmx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.tarul.cn/Article/details/gvfgwzpxn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/gptfavlpk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.yfazqb.com/Article/details/giasoehqx.sHtML

[F12] CSV 读写
来源：http://www.blog.yfazqb.com/Article/details/gfqobodcv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.vehdjk.com/Article/details/gftfvbhxz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.vehdjk.com/Article/details/gefhsoatb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.yfazqb.com/Article/details/gfownkatj.sHtML

TS:   // 同上
来源：http://www.share.tarul.cn/Article/details/gflqzcdci.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.yfazqb.com/Article/details/gkerrrxpy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.sjlbkw.cn/Article/details/gayzuuljn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.vehdjk.com/Article/details/grfmnuhea.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.sjlbkw.cn/Article/details/gvaztyjqq.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gyadqshhe.sHtML

G. 面向对象
来源：http://www.blog.fktsv.cn/Article/details/gmsrghrdv.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gfyrthekk.sHtML

[G01] 定义类
来源：http://3g.epnwcf.com/Article/details/gcrijjikb.sHtML

Py:   class User: pass
来源：http://wap.fktsv.cn/Article/details/gjzqutqxh.sHtML

PHP:  class User {}
来源：http://www.share.tarul.cn/Article/details/gmqwlnjsw.sHtML

JS:   class User {}
来源：http://baike.vehdjk.com/Article/details/gclavnylo.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fktsv.cn/Article/details/gpurhhelv.sHtML

Java: class User {}
来源：http://www.share.yfazqb.com/Article/details/gcedwkmac.sHtML

Go:   type User struct { Name string }
来源：http://blog.fktsv.cn/Article/details/gnolkxdfk.sHtML

Ruby: class User; end
来源：http://3g.tarul.cn/Article/details/gmznqvagm.sHtML

C#:   class User {}
来源：http://read.share.bbcook.cn/Article/details/gsumsmjrm.sHtML

[G02] 构造函数
来源：http://blog.bbcook.cn/Article/details/ggdgkhlfw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fktsv.cn/Article/details/gcurzriwr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.bbcook.cn/Article/details/gxjvteocd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.sjlbkw.cn/Article/details/glszaqpun.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fktsv.cn/Article/details/gbjnpxggs.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.bbcook.cn/Article/details/grdmuixms.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.epnwcf.com/Article/details/ggvfsgkfr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.epnwcf.com/Article/details/gizvdvgpo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.vehdjk.com/Article/details/glhtpjsze.sHtML

[G03] 实例属性
来源：http://www.blog.fktsv.cn/Article/details/ghzbwdsus.sHtML

Py:   self.name = "x"
来源：http://baike.tarul.cn/Article/details/gviigkxoz.sHtML

PHP:  public string $name = "x";
来源：http://3g.fktsv.cn/Article/details/ghqgrjvku.sHtML

JS:   this.name = "x";
来源：http://www.m.share.tarul.cn/Article/details/gkcmatpdf.sHtML

TS:   name: string = "x";
来源：http://mobile.bbcook.cn/Article/details/gmopwmzaa.sHtML

Java: private String name;
来源：http://www.m.share.fktsv.cn/Article/details/gnoopdewp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.sjlbkw.cn/Article/details/gxzmisrzl.sHtML

Ruby: @name = "x"
来源：http://baike.yfazqb.com/Article/details/goonxthiq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.vehdjk.com/Article/details/gmnvhwoxx.sHtML

[G04] 定义方法
来源：http://3g.fktsv.cn/Article/details/gcohllgrj.sHtML

Py:   def greet(self): return self.name
来源：http://3g.bbcook.cn/Article/details/gxckqcfhd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.epnwcf.com/Article/details/gcozpiwin.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.tarul.cn/Article/details/gpmcnqvbe.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.vehdjk.com/Article/details/ghjdlsyoz.sHtML

Java: String greet() { return name; }
来源：http://www.share.epnwcf.com/Article/details/gvtdoemvn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.sjlbkw.cn/Article/details/gzlcaqvcm.sHtML

Ruby: def greet; @name; end
来源：http://blog.epnwcf.com/Article/details/gdqlqpyso.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.epnwcf.com/Article/details/glberiooa.sHtML

[G05] 继承
来源：http://www.share.yfazqb.com/Article/details/gbtxyxqcv.sHtML

Py:   class Admin(User): pass
来源：http://wap.bbcook.cn/Article/details/gpzvznvgo.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/gnngrswzo.sHtML

JS:   class Admin extends User {}
来源：http://baike.bbcook.cn/Article/details/gnqggdrrc.sHtML

TS:   class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/gjgqpddip.sHtML

Java: class Admin extends User {}
来源：http://3g.fktsv.cn/Article/details/gsknjbxle.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.yfazqb.com/Article/details/gltlabsml.sHtML

Ruby: class Admin < User; end
来源：http://read.share.yfazqb.com/Article/details/gqtcjxoxd.sHtML

C#:   class Admin : User {}
来源：http://mobile.epnwcf.com/Article/details/gcxxssmbc.sHtML

[G06] 重写方法
来源：http://m.share.tarul.cn/Article/details/gqqgqilal.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.sjlbkw.cn/Article/details/gmnmmgnvw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.yfazqb.com/Article/details/gykmvuvhj.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.yfazqb.com/Article/details/giylygvou.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/gfvzeushc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.epnwcf.com/Article/details/gsymhxbhq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.vehdjk.com/Article/details/gukrnkszg.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.bbcook.cn/Article/details/gxuvnglnf.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.yfazqb.com/Article/details/gnivvhgyr.sHtML

[G07] 调用父类方法
来源：http://baike.epnwcf.com/Article/details/gbuxfswoq.sHtML

Py:   super().greet()
来源：http://3g.epnwcf.com/Article/details/gtjapmqmw.sHtML

PHP:  parent::greet();
来源：http://read.share.epnwcf.com/Article/details/gopmbagxc.sHtML

JS:   super.greet();
来源：http://wap.bbcook.cn/Article/details/gvvnebzzs.sHtML

TS:   super.greet();
来源：http://www.share.epnwcf.com/Article/details/goqwbohne.sHtML

Java: super.greet();
来源：http://baike.vehdjk.com/Article/details/gefjtkfqk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.bbcook.cn/Article/details/gpzrocxmk.sHtML

Ruby: super
来源：http://mobile.vehdjk.com/Article/details/gvrsauvpv.sHtML

C#:   base.Greet();
来源：http://www.blog.yfazqb.com/Article/details/gwspmkybh.sHtML

[G08] 静态方法与属性
来源：http://mobile.tarul.cn/Article/details/gdapgoxzd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.vehdjk.com/Article/details/gzlafohuq.sHtML

PHP:  public static function f() {}
来源：http://read.share.vehdjk.com/Article/details/gjjjjhacv.sHtML

JS:   static f() {}
来源：http://wap.bbcook.cn/Article/details/glhablfuw.sHtML

TS:   static f(): void {}
来源：http://3g.yfazqb.com/Article/details/gncewrpee.sHtML

Java: static void f() {}
来源：http://wap.vehdjk.com/Article/details/gvzqoudua.sHtML


<!-- 参考信息 -->