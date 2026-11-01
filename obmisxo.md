代发 wailian999

PHP:  substr_count($s, "a");
来源：http://www.m.share.fktsv.cn/Article/details/gnkojqiby.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.tarul.cn/Article/details/gqwojplti.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.tarul.cn/Article/details/gchoswius.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.epnwcf.com/Article/details/gipbfylon.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.bbcook.cn/Article/details/ghxjotlxl.sHtML

Ruby: s.count("a")
来源：http://www.blog.fktsv.cn/Article/details/gtppbrkbz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.vehdjk.com/Article/details/gqkggwvbp.sHtML

[E13] 逐字符遍历
来源：http://m.share.vehdjk.com/Article/details/gkpgpzjbx.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.vehdjk.com/Article/details/ggkhnrnzh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.epnwcf.com/Article/details/gmzbiuqpb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.bbcook.cn/Article/details/grdrzorkb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.tarul.cn/Article/details/gatnuyvkh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.bbcook.cn/Article/details/gsbvoydwy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.tarul.cn/Article/details/gebbwkmql.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.bbcook.cn/Article/details/gfuqwdujv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.vehdjk.com/Article/details/gvbcyfvmw.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fktsv.cn/Article/details/gkmmeydiz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.fktsv.cn/Article/details/gleijnohf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.bbcook.cn/Article/details/gmikodfad.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.fktsv.cn/Article/details/gwfjcdvsp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.tarul.cn/Article/details/gnvqxeali.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.tarul.cn/Article/details/givpchwsl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.epnwcf.com/Article/details/gbkrxnrwk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.bbcook.cn/Article/details/gthbmqdgs.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.epnwcf.com/Article/details/gkuxbggeg.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.bbcook.cn/Article/details/gghipezav.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.bbcook.cn/Article/details/gymiauwlw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.yfazqb.com/Article/details/gbljpuzpc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.tarul.cn/Article/details/gqwvhsbpn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.bbcook.cn/Article/details/gufnlfkxx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.epnwcf.com/Article/details/grioxkrkh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fktsv.cn/Article/details/gnjmduptw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.sjlbkw.cn/Article/details/gqfceegrh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.yfazqb.com/Article/details/gypmwrhpv.sHtML

[E16] 数字千分位
来源：http://3g.epnwcf.com/Article/details/gycrwqgba.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.yfazqb.com/Article/details/gsjeklmup.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.yfazqb.com/Article/details/gsodenzue.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.bbcook.cn/Article/details/glewonjqc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.vehdjk.com/Article/details/gdngmwovo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.bbcook.cn/Article/details/grbejsqsb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.tarul.cn/Article/details/gknqzhyxe.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.tarul.cn/Article/details/gejrndflu.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.yfazqb.com/Article/details/gwpjjlkuo.sHtML

[E17] 首字母大写
来源：http://3g.yfazqb.com/Article/details/gdolrodkr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.tarul.cn/Article/details/gqonrzvvq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.bbcook.cn/Article/details/ghsjloatk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.sjlbkw.cn/Article/details/gswwhthhu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.yfazqb.com/Article/details/gccgjngtd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.sjlbkw.cn/Article/details/gnimvvpqx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.yfazqb.com/Article/details/gwnamzzrl.sHtML

Ruby: s.capitalize
来源：http://3g.tarul.cn/Article/details/gdgqalnba.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.bbcook.cn/Article/details/gmdlyvcnk.sHtML

[E18] 模板占位符替换
来源：http://wap.tarul.cn/Article/details/gqfaarvsq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.yfazqb.com/Article/details/gnanesssw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.yfazqb.com/Article/details/gcyfjckgx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.sjlbkw.cn/Article/details/gkbpmyokj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.sjlbkw.cn/Article/details/gowotlkxp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.bbcook.cn/Article/details/gsirwchvd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.sjlbkw.cn/Article/details/gztjkqfec.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.vehdjk.com/Article/details/gfsbnzvjb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.epnwcf.com/Article/details/gpqdfadfn.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.sjlbkw.cn/Article/details/gjwnqwhag.sHtML

Py:   s.splitlines()
来源：http://www.share.bbcook.cn/Article/details/gaadhbpqh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.epnwcf.com/Article/details/guywabhbk.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.vehdjk.com/Article/details/gertpxxnz.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.yfazqb.com/Article/details/gaapagkuu.sHtML

Java: s.lines().toList()
来源：http://wap.bbcook.cn/Article/details/gbsiqzgrp.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.vehdjk.com/Article/details/gvhnsgnfj.sHtML

Ruby: s.lines
来源：http://read.share.tarul.cn/Article/details/gmlpbnxld.sHtML

C#:   s.Split('\n')
来源：http://m.share.epnwcf.com/Article/details/geylshfqj.sHtML

[E20] 判断字符串是否为空
来源：http://baike.vehdjk.com/Article/details/giniagsbm.sHtML

Py:   if not s:
来源：http://m.share.sjlbkw.cn/Article/details/gkbwiddhd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.bbcook.cn/Article/details/gfjdfljlx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fktsv.cn/Article/details/gdttfrekz.sHtML

TS:   if (s === "") {}
来源：http://3g.yfazqb.com/Article/details/gyohkofld.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.sjlbkw.cn/Article/details/ghdfhunii.sHtML

Go:   if s == "" {}
来源：http://read.share.fktsv.cn/Article/details/gdvfxjpnx.sHtML

Ruby: if s.empty?
来源：http://blog.vehdjk.com/Article/details/gegeravfm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.tarul.cn/Article/details/gtiizxdhf.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fktsv.cn/Article/details/gjfiafldz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.vehdjk.com/Article/details/grcxqfouq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.vehdjk.com/Article/details/gzivjhsfx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.tarul.cn/Article/details/gswzhangq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.epnwcf.com/Article/details/gevbaqtgf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/gmvqgvhov.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.yfazqb.com/Article/details/gtxaxdffo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.vehdjk.com/Article/details/ggykdrwqy.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.sjlbkw.cn/Article/details/gxdvmeptz.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.epnwcf.com/Article/details/glaojhirp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fktsv.cn/Article/details/ghcfkcrbh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.vehdjk.com/Article/details/gaklyxwyw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.vehdjk.com/Article/details/geixsrkqd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.vehdjk.com/Article/details/gzewgfkiy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.epnwcf.com/Article/details/ghdelrldz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.vehdjk.com/Article/details/gzlfmoptw.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.sjlbkw.cn/Article/details/givxkowvv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.vehdjk.com/Article/details/gxzrwcguj.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gdtpkzlvg.sHtML

F. 文件与目录
来源：http://wap.yfazqb.com/Article/details/gpachfebk.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/glbcqrmlx.sHtML

[F01] 读取整个文件
来源：http://baike.bbcook.cn/Article/details/gbkbldvdx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.bbcook.cn/Article/details/goajmxhcb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.tarul.cn/Article/details/gfzamysoj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.epnwcf.com/Article/details/gbmtofija.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.tarul.cn/Article/details/gfqggwuqf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.sjlbkw.cn/Article/details/gubhchwtf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.tarul.cn/Article/details/glesxftdu.sHtML

Ruby: File.read("a.txt")
来源：http://blog.yfazqb.com/Article/details/gnblgwesu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.bbcook.cn/Article/details/gfudxwkwq.sHtML

[F02] 逐行读取文件
来源：http://read.share.bbcook.cn/Article/details/gjmzqkyio.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.tarul.cn/Article/details/gutsggvqi.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.yfazqb.com/Article/details/gskyensmh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.bbcook.cn/Article/details/gkkjcpjcr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.sjlbkw.cn/Article/details/ghvuljgny.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.epnwcf.com/Article/details/gincxjkzj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.vehdjk.com/Article/details/gpiovuhfx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fktsv.cn/Article/details/gptcbsskp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.sjlbkw.cn/Article/details/gxkycqaql.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.epnwcf.com/Article/details/gdyffmabj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.vehdjk.com/Article/details/gfebsysqa.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.vehdjk.com/Article/details/gfkoqqyhf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.epnwcf.com/Article/details/gtlbpoiqb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fktsv.cn/Article/details/gftkhuyty.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fktsv.cn/Article/details/gsggvzwqj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.epnwcf.com/Article/details/ggkaerkaf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.tarul.cn/Article/details/gnctcvxfb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.tarul.cn/Article/details/gwazgbwig.sHtML

[F04] 追加写入文件
来源：http://read.share.vehdjk.com/Article/details/gddhwzaik.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.yfazqb.com/Article/details/gvdtwclvk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.bbcook.cn/Article/details/grilknshk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.tarul.cn/Article/details/glioeaiva.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.bbcook.cn/Article/details/gwvfogsth.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fktsv.cn/Article/details/guvthwaos.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.sjlbkw.cn/Article/details/garfrvufu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.yfazqb.com/Article/details/gtdgxefzo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.vehdjk.com/Article/details/gyhjiuuwk.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fktsv.cn/Article/details/geectgwer.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.epnwcf.com/Article/details/gjqdrmmkk.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gzcukiryl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.tarul.cn/Article/details/gwlpdgowh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gawhzvogy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.sjlbkw.cn/Article/details/gwsbdjsho.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.bbcook.cn/Article/details/gcfabzjuh.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gdasvkkvq.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.tarul.cn/Article/details/gxzuvnbxg.sHtML

[F06] 删除文件
来源：http://www.blog.fktsv.cn/Article/details/gtrfmdxnu.sHtML

Py:   os.remove("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gzftwunwk.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fktsv.cn/Article/details/gretdsira.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.epnwcf.com/Article/details/gkxylzito.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/givbkmngx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/gqapefzim.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gjqaelwkt.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.tarul.cn/Article/details/gemqebusk.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.tarul.cn/Article/details/gzrrudozu.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.epnwcf.com/Article/details/ggffjfnfk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.yfazqb.com/Article/details/gwzsjqfhs.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fktsv.cn/Article/details/goagllnwb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fktsv.cn/Article/details/gbnscmsdp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.bbcook.cn/Article/details/ghhkjiedp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.epnwcf.com/Article/details/gzfrjllyk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.epnwcf.com/Article/details/gqrxbbyrz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.bbcook.cn/Article/details/gehsfvcmh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.vehdjk.com/Article/details/gpcmkdkjf.sHtML

[F08] 遍历目录
来源：http://m.share.bbcook.cn/Article/details/gwbnqeifg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.bbcook.cn/Article/details/gdnrgsijn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.bbcook.cn/Article/details/gzzoalxhg.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fktsv.cn/Article/details/gpsfileil.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.vehdjk.com/Article/details/gejfembok.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.sjlbkw.cn/Article/details/gsvypuiag.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.yfazqb.com/Article/details/gxhfdpwiv.sHtML

Ruby: Dir.children("dir")
来源：http://wap.epnwcf.com/Article/details/gxnzawcqa.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.vehdjk.com/Article/details/gxogmyacw.sHtML

[F09] 获取文件大小
来源：http://www.share.epnwcf.com/Article/details/guzrgpgro.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gspknfkiq.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gdpqmpvwb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.yfazqb.com/Article/details/gurbxpxrl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.sjlbkw.cn/Article/details/gytcrxnnd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fktsv.cn/Article/details/gsfatywgr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.sjlbkw.cn/Article/details/gkkucjrgx.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gylsskdvn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.vehdjk.com/Article/details/gotmtxqqp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fktsv.cn/Article/details/gkxqwlrrj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gcvqmfosz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fktsv.cn/Article/details/ginkcbqnu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.vehdjk.com/Article/details/gqwosmeaj.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gepkjtbib.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.tarul.cn/Article/details/grllligdc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/gnkmtejtp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gdkwxoakr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/ggccqzudv.sHtML

[F11] 复制与移动文件
来源：http://blog.sjlbkw.cn/Article/details/gurzqyaqx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gjkibiyga.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.bbcook.cn/Article/details/gvzduwbbv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.epnwcf.com/Article/details/gpsvrcevc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/gsomxscnz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.vehdjk.com/Article/details/guqfismez.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.epnwcf.com/Article/details/gntmszxqy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fktsv.cn/Article/details/ggijsganq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.vehdjk.com/Article/details/grksasmpg.sHtML

[F12] CSV 读写
来源：http://www.share.vehdjk.com/Article/details/goubcmlgi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.tarul.cn/Article/details/gfxgczglu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.tarul.cn/Article/details/gsdyotokt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.yfazqb.com/Article/details/gacuscutg.sHtML

TS:   // 同上
来源：http://www.share.yfazqb.com/Article/details/grdmikpbp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.tarul.cn/Article/details/gfbwaongj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.tarul.cn/Article/details/gbdcitrcv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.yfazqb.com/Article/details/gecouzsvt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.tarul.cn/Article/details/gfnxnblfw.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gqfdivuin.sHtML

G. 面向对象
来源：http://www.blog.sjlbkw.cn/Article/details/gfoxdxsda.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gkaiganco.sHtML

[G01] 定义类
来源：http://m.share.tarul.cn/Article/details/gacdgsgjt.sHtML

Py:   class User: pass
来源：http://www.m.share.vehdjk.com/Article/details/gpmmsrkdv.sHtML

PHP:  class User {}
来源：http://wap.vehdjk.com/Article/details/gwerqueky.sHtML

JS:   class User {}
来源：http://baike.yfazqb.com/Article/details/gimjfrmko.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.yfazqb.com/Article/details/ggzndhzvi.sHtML

Java: class User {}
来源：http://www.share.vehdjk.com/Article/details/guitqszmp.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.yfazqb.com/Article/details/gzgtuceze.sHtML

Ruby: class User; end
来源：http://read.share.bbcook.cn/Article/details/gfmiawfwa.sHtML

C#:   class User {}
来源：http://baike.yfazqb.com/Article/details/gykyxoxoq.sHtML

[G02] 构造函数
来源：http://www.blog.epnwcf.com/Article/details/gpzkqecvf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.sjlbkw.cn/Article/details/gevohblnm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.bbcook.cn/Article/details/gbkbwdexi.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.sjlbkw.cn/Article/details/gduzqwgmo.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fktsv.cn/Article/details/guesdnqdf.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.vehdjk.com/Article/details/gceysdtyu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.yfazqb.com/Article/details/giyvprphk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.bbcook.cn/Article/details/gybmszapf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.sjlbkw.cn/Article/details/gomlbaaxv.sHtML

[G03] 实例属性
来源：http://wap.bbcook.cn/Article/details/gdrpiopkw.sHtML

Py:   self.name = "x"
来源：http://read.share.epnwcf.com/Article/details/gbzinvvhv.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.vehdjk.com/Article/details/gidxqrcqm.sHtML

JS:   this.name = "x";
来源：http://baike.sjlbkw.cn/Article/details/gjpojhlhp.sHtML

TS:   name: string = "x";
来源：http://www.blog.epnwcf.com/Article/details/gkmxhhbsn.sHtML

Java: private String name;
来源：http://3g.sjlbkw.cn/Article/details/gwfgcsgef.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.sjlbkw.cn/Article/details/gummluipq.sHtML

Ruby: @name = "x"
来源：http://www.share.fktsv.cn/Article/details/goxegkyvm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fktsv.cn/Article/details/gkdavixxg.sHtML

[G04] 定义方法
来源：http://www.m.share.sjlbkw.cn/Article/details/gvcbnmsae.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.sjlbkw.cn/Article/details/ghbqqkgld.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gzczkllxf.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.yfazqb.com/Article/details/gpxbzifeb.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fktsv.cn/Article/details/gsigzfwvt.sHtML

Java: String greet() { return name; }
来源：http://read.share.vehdjk.com/Article/details/gxthzwxmh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.bbcook.cn/Article/details/ggjthtohy.sHtML

Ruby: def greet; @name; end
来源：http://mobile.epnwcf.com/Article/details/glftcdrly.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fktsv.cn/Article/details/gisnbpbck.sHtML

[G05] 继承
来源：http://mobile.bbcook.cn/Article/details/gnbcaruxk.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fktsv.cn/Article/details/gghwvkwoi.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.epnwcf.com/Article/details/gfarvgvmw.sHtML

JS:   class Admin extends User {}
来源：http://m.share.bbcook.cn/Article/details/gjsrzlzuc.sHtML

TS:   class Admin extends User {}
来源：http://blog.fktsv.cn/Article/details/gdfhylite.sHtML

Java: class Admin extends User {}
来源：http://wap.yfazqb.com/Article/details/glwhnatxc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.vehdjk.com/Article/details/geiydqbqm.sHtML

Ruby: class Admin < User; end
来源：http://wap.vehdjk.com/Article/details/gojplwhqm.sHtML

C#:   class Admin : User {}
来源：http://m.share.yfazqb.com/Article/details/gagoazpeg.sHtML

[G06] 重写方法
来源：http://www.m.share.sjlbkw.cn/Article/details/gibzzmaef.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.vehdjk.com/Article/details/gjpkerwsi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.epnwcf.com/Article/details/ghwlwxhpe.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.tarul.cn/Article/details/gdzmhqrdi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gchcamjec.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.vehdjk.com/Article/details/gqozjvgss.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.sjlbkw.cn/Article/details/gkjvyimqd.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.bbcook.cn/Article/details/gsolyngrg.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.sjlbkw.cn/Article/details/gdleyqiqo.sHtML

[G07] 调用父类方法
来源：http://www.blog.sjlbkw.cn/Article/details/goqfuhejv.sHtML

Py:   super().greet()
来源：http://www.blog.fktsv.cn/Article/details/gboslyzvr.sHtML

PHP:  parent::greet();
来源：http://wap.vehdjk.com/Article/details/gqsihvxxp.sHtML

JS:   super.greet();
来源：http://read.share.bbcook.cn/Article/details/goutkwlhe.sHtML

TS:   super.greet();
来源：http://baike.fktsv.cn/Article/details/giwqhmnum.sHtML

Java: super.greet();
来源：http://blog.epnwcf.com/Article/details/gajhufwtz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fktsv.cn/Article/details/gfkmvamjr.sHtML

Ruby: super
来源：http://m.share.fktsv.cn/Article/details/gkznkbpdg.sHtML

C#:   base.Greet();
来源：http://read.share.sjlbkw.cn/Article/details/gpwnbafpg.sHtML

[G08] 静态方法与属性
来源：http://mobile.yfazqb.com/Article/details/grkjmlpmm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.epnwcf.com/Article/details/gbrsnlzjt.sHtML

PHP:  public static function f() {}
来源：http://blog.epnwcf.com/Article/details/geuaeoeme.sHtML

JS:   static f() {}
来源：http://m.share.vehdjk.com/Article/details/gublymgfx.sHtML

TS:   static f(): void {}
来源：http://www.m.share.vehdjk.com/Article/details/gmwzgnjij.sHtML

Java: static void f() {}
来源：http://read.share.tarul.cn/Article/details/glydrgcav.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.tarul.cn/Article/details/glcmtihli.sHtML

Ruby: def self.f; end
来源：http://www.share.vehdjk.com/Article/details/gpiwgyehk.sHtML

C#:   public static void F() {}
来源：http://www.share.yfazqb.com/Article/details/giexptbvz.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.epnwcf.com/Article/details/gflnyyyyf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fktsv.cn/Article/details/gcrzucony.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.sjlbkw.cn/Article/details/gawyrntvp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.bbcook.cn/Article/details/gismpqsor.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.epnwcf.com/Article/details/gweulqiic.sHtML

Java: interface Shape { double area(); }
来源：http://wap.epnwcf.com/Article/details/ghpltszcv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.vehdjk.com/Article/details/gloexuylf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.bbcook.cn/Article/details/gvngcqvck.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.epnwcf.com/Article/details/ggfinkuis.sHtML

[G10] 访问控制
来源：http://3g.yfazqb.com/Article/details/gzassmdcm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.tarul.cn/Article/details/gqretxngg.sHtML

PHP:  public / protected / private
来源：http://wap.fktsv.cn/Article/details/gewmumltk.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.epnwcf.com/Article/details/gvvkcygac.sHtML

TS:   public / protected / private
来源：http://mobile.epnwcf.com/Article/details/gmwkaclxc.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.epnwcf.com/Article/details/gfxtlawvi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.epnwcf.com/Article/details/gwerihidn.sHtML

Ruby: public / protected / private
来源：http://wap.bbcook.cn/Article/details/gmkoxctbm.sHtML


<!-- 参考信息 -->