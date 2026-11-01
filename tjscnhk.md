代发 wailian999

PHP:  substr_count($s, "a");
来源：http://www.share.fktsv.cn/Article/details/gsctouqye.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.bbcook.cn/Article/details/gprvkibzu.sHtML

TS:   s.split("a").length - 1
来源：http://wap.sjlbkw.cn/Article/details/glczwubsi.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.yfazqb.com/Article/details/gxaosecvg.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.vehdjk.com/Article/details/gqkozfbfv.sHtML

Ruby: s.count("a")
来源：http://baike.epnwcf.com/Article/details/gkkjvniyl.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.yfazqb.com/Article/details/gxoezkahg.sHtML

[E13] 逐字符遍历
来源：http://wap.yfazqb.com/Article/details/gvgbqkbhv.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.sjlbkw.cn/Article/details/gjkqiugfo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.sjlbkw.cn/Article/details/gckkkwkdn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.bbcook.cn/Article/details/ghfjfslqg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fktsv.cn/Article/details/glnrtqqww.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fktsv.cn/Article/details/gsmjgrwcd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.yfazqb.com/Article/details/gxoccsxkd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.tarul.cn/Article/details/gvsswrekq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghnovwtga.sHtML

[E14] URL 编码与 Base64
来源：http://baike.bbcook.cn/Article/details/ggufucvbq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.sjlbkw.cn/Article/details/guarmfvej.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.epnwcf.com/Article/details/gehqveqvt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.epnwcf.com/Article/details/goduixhlp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.vehdjk.com/Article/details/gmyxuuobo.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.yfazqb.com/Article/details/ggkbhjevq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fktsv.cn/Article/details/grttueqhe.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fktsv.cn/Article/details/ghgtpgwnd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fktsv.cn/Article/details/gddixnvzh.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.sjlbkw.cn/Article/details/gtaaqrrhp.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.tarul.cn/Article/details/gcmctjghn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.yfazqb.com/Article/details/gkxiwzknu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.vehdjk.com/Article/details/getvtqyja.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fktsv.cn/Article/details/gahfzumow.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.tarul.cn/Article/details/gfrgtvxtt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.vehdjk.com/Article/details/gxewhjqkp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.epnwcf.com/Article/details/gaodxwiqh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.sjlbkw.cn/Article/details/ggzohxiwg.sHtML

[E16] 数字千分位
来源：http://3g.yfazqb.com/Article/details/geihqfbsp.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.vehdjk.com/Article/details/gmtlilivy.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fktsv.cn/Article/details/gsqutjrnz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.sjlbkw.cn/Article/details/gimaauxgg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.vehdjk.com/Article/details/gehuwxwjz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.epnwcf.com/Article/details/gppvcxexh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.epnwcf.com/Article/details/gbpecopqh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.epnwcf.com/Article/details/gzwfsflry.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fktsv.cn/Article/details/gzjqwhzdo.sHtML

[E17] 首字母大写
来源：http://blog.fktsv.cn/Article/details/gbjgmmgds.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.vehdjk.com/Article/details/gavsfavul.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.tarul.cn/Article/details/goktsghhh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.sjlbkw.cn/Article/details/glbsmduxu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.epnwcf.com/Article/details/gsudqrwot.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.epnwcf.com/Article/details/gtsbbphlf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.tarul.cn/Article/details/gervgcbej.sHtML

Ruby: s.capitalize
来源：http://mobile.bbcook.cn/Article/details/goyoliela.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fktsv.cn/Article/details/giowofwvb.sHtML

[E18] 模板占位符替换
来源：http://baike.epnwcf.com/Article/details/ginajavtv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.vehdjk.com/Article/details/gamodjslk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.vehdjk.com/Article/details/gwnyiwypz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.bbcook.cn/Article/details/giiuqovoz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fktsv.cn/Article/details/gudfrvufw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.sjlbkw.cn/Article/details/gwhxkozwv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.sjlbkw.cn/Article/details/gxordqtsq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.tarul.cn/Article/details/gtszllmqi.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.tarul.cn/Article/details/grdfebevu.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fktsv.cn/Article/details/gctqixxks.sHtML

Py:   s.splitlines()
来源：http://www.m.share.sjlbkw.cn/Article/details/gvfevvzxg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.vehdjk.com/Article/details/gwyvxfiul.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.vehdjk.com/Article/details/gojwemiql.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.tarul.cn/Article/details/gyvwdprsh.sHtML

Java: s.lines().toList()
来源：http://mobile.epnwcf.com/Article/details/ggxagokkn.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.bbcook.cn/Article/details/gaffbnzbj.sHtML

Ruby: s.lines
来源：http://read.share.tarul.cn/Article/details/gcspfhxht.sHtML

C#:   s.Split('\n')
来源：http://3g.tarul.cn/Article/details/gztfeoxzv.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.epnwcf.com/Article/details/gjeewznfa.sHtML

Py:   if not s:
来源：http://3g.fktsv.cn/Article/details/gtptxcqms.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.epnwcf.com/Article/details/gmzpdxfoc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.fktsv.cn/Article/details/gykcckaef.sHtML

TS:   if (s === "") {}
来源：http://read.share.tarul.cn/Article/details/gqhdrywvd.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.bbcook.cn/Article/details/gevbamcmt.sHtML

Go:   if s == "" {}
来源：http://www.share.epnwcf.com/Article/details/gcuvkzbes.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fktsv.cn/Article/details/grmzdjlmv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.tarul.cn/Article/details/gahkeoglg.sHtML

[E21] 超长截断加省略号
来源：http://3g.fktsv.cn/Article/details/gjophuvly.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.sjlbkw.cn/Article/details/gctqmvglg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.epnwcf.com/Article/details/gkvqirqzf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.epnwcf.com/Article/details/gxnvdlrey.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gulgofbnv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fktsv.cn/Article/details/gvyloauba.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.sjlbkw.cn/Article/details/gfjbghmej.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.vehdjk.com/Article/details/ghrxohgla.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.tarul.cn/Article/details/gybvhuykd.sHtML

[E22] 字节长度与字符长度
来源：http://blog.vehdjk.com/Article/details/guygjylhu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.epnwcf.com/Article/details/gkfysdkvk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/gafcxfrgf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.epnwcf.com/Article/details/gcjrpqfiu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fktsv.cn/Article/details/gphpiokpc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.fktsv.cn/Article/details/gvtyyriay.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.sjlbkw.cn/Article/details/gexvztgow.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fktsv.cn/Article/details/gvtuckzzk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.yfazqb.com/Article/details/gpcmnyngz.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gfbqrztuh.sHtML

F. 文件与目录
来源：http://blog.tarul.cn/Article/details/gzcwsbtqp.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gmsaorbky.sHtML

[F01] 读取整个文件
来源：http://wap.fktsv.cn/Article/details/gbjzetzba.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.tarul.cn/Article/details/gvljplvlv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gzrjkwqgg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.epnwcf.com/Article/details/guyibvakp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.sjlbkw.cn/Article/details/gzhpcelfv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/gxtautgft.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.yfazqb.com/Article/details/gargecgyb.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gaefulqtv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.yfazqb.com/Article/details/gefynsweq.sHtML

[F02] 逐行读取文件
来源：http://3g.bbcook.cn/Article/details/gttpnvhgh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.epnwcf.com/Article/details/ggryojiwk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.bbcook.cn/Article/details/gafbttpwf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.bbcook.cn/Article/details/gpmilrfmt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.yfazqb.com/Article/details/grzsvyeww.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.yfazqb.com/Article/details/gvykkwwiq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.bbcook.cn/Article/details/gdevincsm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.sjlbkw.cn/Article/details/gjpzffuuj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.epnwcf.com/Article/details/guywxrmbr.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.vehdjk.com/Article/details/gadynmcjt.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.epnwcf.com/Article/details/ghtlublxy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.tarul.cn/Article/details/gbvbnjqcp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.sjlbkw.cn/Article/details/gozytrdjq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.yfazqb.com/Article/details/gvomkukew.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.bbcook.cn/Article/details/gbrpjonax.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.tarul.cn/Article/details/gqspfbsmc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.sjlbkw.cn/Article/details/gilnqishp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.sjlbkw.cn/Article/details/gpcnsdhzw.sHtML

[F04] 追加写入文件
来源：http://www.m.share.yfazqb.com/Article/details/gpihtbxrq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.tarul.cn/Article/details/gkjbvibyc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.tarul.cn/Article/details/gtfvggjtn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fktsv.cn/Article/details/goyckjkmp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.yfazqb.com/Article/details/gsjqqnfti.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.vehdjk.com/Article/details/gjxjgykom.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.bbcook.cn/Article/details/ggiguafag.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.bbcook.cn/Article/details/gjiylbqyk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.vehdjk.com/Article/details/guehevjrg.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.vehdjk.com/Article/details/gzdfvvmph.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.vehdjk.com/Article/details/gwwbiltou.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.tarul.cn/Article/details/gjuyfkevg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gtkbgdzhd.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.vehdjk.com/Article/details/geawgslvm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.bbcook.cn/Article/details/gzvosoubo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.yfazqb.com/Article/details/grczkkjuh.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gwjlgyxyr.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gtcjafjdf.sHtML

[F06] 删除文件
来源：http://mobile.epnwcf.com/Article/details/gegeblyqq.sHtML

Py:   os.remove("a.txt")
来源：http://blog.epnwcf.com/Article/details/gitfubmvb.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fktsv.cn/Article/details/guspjxiyz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gupklmbgp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.bbcook.cn/Article/details/givwiaukh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fktsv.cn/Article/details/ghcabjqoo.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gjiaxpwgl.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gqnuijmxo.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fktsv.cn/Article/details/gycansuna.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.tarul.cn/Article/details/gvlatnkhq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.epnwcf.com/Article/details/gkshjkzwm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.yfazqb.com/Article/details/gxswzicps.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.vehdjk.com/Article/details/geuztijmi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.sjlbkw.cn/Article/details/gxjuorjze.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.vehdjk.com/Article/details/gecezigxt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.yfazqb.com/Article/details/gqzkqvvsy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.tarul.cn/Article/details/gbbetfjey.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.yfazqb.com/Article/details/gxukoexgm.sHtML

[F08] 遍历目录
来源：http://www.blog.bbcook.cn/Article/details/grbmadpgh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.tarul.cn/Article/details/ghjlpurnn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gauucrhdp.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.epnwcf.com/Article/details/ggxldoncs.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.sjlbkw.cn/Article/details/glcqtwtyx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.bbcook.cn/Article/details/ggyychccx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fktsv.cn/Article/details/gdcokdhce.sHtML

Ruby: Dir.children("dir")
来源：http://wap.bbcook.cn/Article/details/gfjojpmgl.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fktsv.cn/Article/details/gfoqrwidm.sHtML

[F09] 获取文件大小
来源：http://www.share.tarul.cn/Article/details/grpfhxdsx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/goobngsbd.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fktsv.cn/Article/details/guhatdkhh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fktsv.cn/Article/details/gcxlekcll.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.epnwcf.com/Article/details/gwousxncv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.vehdjk.com/Article/details/gipulbckp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.tarul.cn/Article/details/gghfuwaqq.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fktsv.cn/Article/details/gzgjajxaj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.bbcook.cn/Article/details/gdprlqods.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.sjlbkw.cn/Article/details/gqddnfdom.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.bbcook.cn/Article/details/gedjtvdbg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gajenfkei.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.vehdjk.com/Article/details/gczvmceeg.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gonsdxopq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.epnwcf.com/Article/details/gptsudxhg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gskgrscef.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/ggumryecl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/gyhdlazax.sHtML

[F11] 复制与移动文件
来源：http://www.share.vehdjk.com/Article/details/glzsixymo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.bbcook.cn/Article/details/gwmmzcrqn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.tarul.cn/Article/details/gixsrhpji.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.vehdjk.com/Article/details/gxrtyoxws.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gzrypiwll.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fktsv.cn/Article/details/gbpwmbzxm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.tarul.cn/Article/details/gcykdfggr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.yfazqb.com/Article/details/galobioqf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.tarul.cn/Article/details/guqsmdsmw.sHtML

[F12] CSV 读写
来源：http://mobile.bbcook.cn/Article/details/gnkdppvmk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fktsv.cn/Article/details/gbkrcedyu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.epnwcf.com/Article/details/gdsfrxvzx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.tarul.cn/Article/details/gcpndihmo.sHtML

TS:   // 同上
来源：http://www.blog.bbcook.cn/Article/details/gktbergyy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.yfazqb.com/Article/details/gzvbzqsuh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.epnwcf.com/Article/details/gxtxtzqde.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.epnwcf.com/Article/details/gamxmbktt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.yfazqb.com/Article/details/gqhhbpztr.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/ghlvmfggs.sHtML

G. 面向对象
来源：http://baike.fktsv.cn/Article/details/gwtydxljm.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gwnyumkso.sHtML

[G01] 定义类
来源：http://3g.yfazqb.com/Article/details/gokflpfcc.sHtML

Py:   class User: pass
来源：http://wap.fktsv.cn/Article/details/gjhkmlrlh.sHtML

PHP:  class User {}
来源：http://3g.epnwcf.com/Article/details/gqzroxzya.sHtML

JS:   class User {}
来源：http://m.share.vehdjk.com/Article/details/guzjxatel.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.vehdjk.com/Article/details/gjqykbomc.sHtML

Java: class User {}
来源：http://3g.sjlbkw.cn/Article/details/gzqmejmvq.sHtML

Go:   type User struct { Name string }
来源：http://baike.tarul.cn/Article/details/gxgbyewac.sHtML

Ruby: class User; end
来源：http://wap.bbcook.cn/Article/details/gdgbtzwil.sHtML

C#:   class User {}
来源：http://baike.yfazqb.com/Article/details/gysxwzzmi.sHtML

[G02] 构造函数
来源：http://www.blog.fktsv.cn/Article/details/gkzvfudga.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.tarul.cn/Article/details/gqndimlxo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.epnwcf.com/Article/details/gznaacotm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.yfazqb.com/Article/details/gvegaacnu.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fktsv.cn/Article/details/gxcskhsno.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.yfazqb.com/Article/details/gdrfmwnzw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.sjlbkw.cn/Article/details/gyztljtqg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.sjlbkw.cn/Article/details/godcnvnux.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.epnwcf.com/Article/details/gprdekwpg.sHtML

[G03] 实例属性
来源：http://wap.bbcook.cn/Article/details/gllqfdkgi.sHtML

Py:   self.name = "x"
来源：http://read.share.sjlbkw.cn/Article/details/gzhqtcftn.sHtML

PHP:  public string $name = "x";
来源：http://baike.bbcook.cn/Article/details/gspewmvel.sHtML

JS:   this.name = "x";
来源：http://m.share.bbcook.cn/Article/details/gzuaefswe.sHtML

TS:   name: string = "x";
来源：http://www.m.share.yfazqb.com/Article/details/gwvcspopj.sHtML

Java: private String name;
来源：http://www.share.epnwcf.com/Article/details/gdmqchxbz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.epnwcf.com/Article/details/gewiqqicn.sHtML

Ruby: @name = "x"
来源：http://3g.yfazqb.com/Article/details/giiyghtvh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.yfazqb.com/Article/details/gryakqqcb.sHtML

[G04] 定义方法
来源：http://wap.sjlbkw.cn/Article/details/guetzqktr.sHtML

Py:   def greet(self): return self.name
来源：http://blog.tarul.cn/Article/details/gtoeyvfcf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.yfazqb.com/Article/details/gnkvxxhqx.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.yfazqb.com/Article/details/gvbqoebnn.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.epnwcf.com/Article/details/gemtbjqdq.sHtML

Java: String greet() { return name; }
来源：http://read.share.fktsv.cn/Article/details/gpiifjlrv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.vehdjk.com/Article/details/gbwtzzwxi.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fktsv.cn/Article/details/ghqflsjpp.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.epnwcf.com/Article/details/gfwtpqdaf.sHtML

[G05] 继承
来源：http://3g.yfazqb.com/Article/details/godedfboe.sHtML

Py:   class Admin(User): pass
来源：http://m.share.tarul.cn/Article/details/gkutjflzg.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fktsv.cn/Article/details/gebcnkomv.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.vehdjk.com/Article/details/glvzgcxse.sHtML

TS:   class Admin extends User {}
来源：http://www.share.sjlbkw.cn/Article/details/gfpgtmgpz.sHtML

Java: class Admin extends User {}
来源：http://mobile.yfazqb.com/Article/details/gubeyqeho.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.epnwcf.com/Article/details/gbhiiemka.sHtML

Ruby: class Admin < User; end
来源：http://wap.yfazqb.com/Article/details/gsdiruadt.sHtML

C#:   class Admin : User {}
来源：http://m.share.tarul.cn/Article/details/gwcdgmruo.sHtML

[G06] 重写方法
来源：http://baike.vehdjk.com/Article/details/gebjqanur.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fktsv.cn/Article/details/goyolzsod.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.bbcook.cn/Article/details/gmbigrmod.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.bbcook.cn/Article/details/gfoswvndo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gbqmoagmc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.bbcook.cn/Article/details/gqhlzbkhh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.tarul.cn/Article/details/guflajpnb.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.vehdjk.com/Article/details/gmxsbavse.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.epnwcf.com/Article/details/ghjuepoxc.sHtML

[G07] 调用父类方法
来源：http://www.blog.bbcook.cn/Article/details/gfguphrbn.sHtML

Py:   super().greet()
来源：http://www.share.bbcook.cn/Article/details/giqndhqze.sHtML

PHP:  parent::greet();
来源：http://3g.fktsv.cn/Article/details/gewokaxis.sHtML

JS:   super.greet();
来源：http://blog.sjlbkw.cn/Article/details/gibycevlc.sHtML

TS:   super.greet();
来源：http://read.share.vehdjk.com/Article/details/gxfxdhdsg.sHtML

Java: super.greet();
来源：http://mobile.yfazqb.com/Article/details/gyoikjgip.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.bbcook.cn/Article/details/gestngplu.sHtML

Ruby: super
来源：http://mobile.vehdjk.com/Article/details/gdpqxfdbz.sHtML

C#:   base.Greet();
来源：http://wap.vehdjk.com/Article/details/gdqcyylkn.sHtML

[G08] 静态方法与属性
来源：http://mobile.vehdjk.com/Article/details/gmajezwsp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.yfazqb.com/Article/details/gcolpueck.sHtML

PHP:  public static function f() {}
来源：http://blog.yfazqb.com/Article/details/gpexzcadx.sHtML

JS:   static f() {}
来源：http://wap.vehdjk.com/Article/details/gcellemir.sHtML

TS:   static f(): void {}
来源：http://3g.tarul.cn/Article/details/gqsjepmun.sHtML

Java: static void f() {}
来源：http://baike.fktsv.cn/Article/details/gipixqqxc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.yfazqb.com/Article/details/gbjhrxfgb.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fktsv.cn/Article/details/gwasxiagk.sHtML

C#:   public static void F() {}
来源：http://wap.sjlbkw.cn/Article/details/goiikpukz.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.bbcook.cn/Article/details/grjvcdfar.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.bbcook.cn/Article/details/grrckmspt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.yfazqb.com/Article/details/ggufezial.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.tarul.cn/Article/details/gdvezyyxv.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.bbcook.cn/Article/details/ggkjhtxmx.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.vehdjk.com/Article/details/gkjjscpia.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gitydoczv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.yfazqb.com/Article/details/gpgywihmn.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.sjlbkw.cn/Article/details/gfpkryfuq.sHtML

[G10] 访问控制
来源：http://mobile.epnwcf.com/Article/details/gjeiifizb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.epnwcf.com/Article/details/gfzpcedby.sHtML

PHP:  public / protected / private
来源：http://blog.bbcook.cn/Article/details/guwwgkbcb.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.sjlbkw.cn/Article/details/gvwjapojz.sHtML

TS:   public / protected / private
来源：http://mobile.vehdjk.com/Article/details/ghpmpsbub.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.yfazqb.com/Article/details/geoufzqry.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.epnwcf.com/Article/details/guprmphzc.sHtML

Ruby: public / protected / private
来源：http://www.share.yfazqb.com/Article/details/gvbeyygmh.sHtML


<!-- 参考信息 -->