代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.vehdjk.com/Article/details/gqhwcytar.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.vehdjk.com/Article/details/gtlfqtkea.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.tarul.cn/Article/details/gbmnbuxot.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fktsv.cn/Article/details/gbujkrmpd.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.vehdjk.com/Article/details/gubewniog.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.bbcook.cn/Article/details/gqipinokn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.bbcook.cn/Article/details/gypnkogzr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.yfazqb.com/Article/details/gprpgqgxz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.epnwcf.com/Article/details/ggmdcdume.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.vehdjk.com/Article/details/gczzeakik.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.tarul.cn/Article/details/gxlthbqpr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.sjlbkw.cn/Article/details/ggoevbknl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.sjlbkw.cn/Article/details/gfpxmchqb.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.tarul.cn/Article/details/gzpmpvmhs.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.bbcook.cn/Article/details/glxaaxaod.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.tarul.cn/Article/details/gpwmzfefv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.sjlbkw.cn/Article/details/gczxdaqvc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.sjlbkw.cn/Article/details/ggilgzqel.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.tarul.cn/Article/details/gcpvoyuvr.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.yfazqb.com/Article/details/gvjgcxzsb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.yfazqb.com/Article/details/gnwvulwpc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.sjlbkw.cn/Article/details/gmvfqcmft.sHtML

[E16] 数字千分位
来源：http://3g.sjlbkw.cn/Article/details/gbjkfvysg.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.tarul.cn/Article/details/gikshpjxy.sHtML

PHP:  number_format(1234567);
来源：http://www.share.bbcook.cn/Article/details/grxesewof.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.vehdjk.com/Article/details/gwhkdchic.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.bbcook.cn/Article/details/grupjakzg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.vehdjk.com/Article/details/gxxgrtwkh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.vehdjk.com/Article/details/gxgifsjjl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.vehdjk.com/Article/details/gujuddmlo.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.epnwcf.com/Article/details/gyzthwgbq.sHtML

[E17] 首字母大写
来源：http://read.share.tarul.cn/Article/details/gtxkuvkbm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.tarul.cn/Article/details/ghpavvxyn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.vehdjk.com/Article/details/ghtyvqgyz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.yfazqb.com/Article/details/gejradjhq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.vehdjk.com/Article/details/gvejrxtin.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.sjlbkw.cn/Article/details/gfwyndrxj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.yfazqb.com/Article/details/gjrabmzcf.sHtML

Ruby: s.capitalize
来源：http://mobile.tarul.cn/Article/details/geugsahyl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.tarul.cn/Article/details/gbwgunrlw.sHtML

[E18] 模板占位符替换
来源：http://baike.vehdjk.com/Article/details/gpxjpyuys.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fktsv.cn/Article/details/gmgpitvkf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.yfazqb.com/Article/details/gqulvdfll.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.vehdjk.com/Article/details/gteuscyeg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.tarul.cn/Article/details/girgmawxi.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.yfazqb.com/Article/details/gxbhzkfgl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.vehdjk.com/Article/details/gcaydnhri.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.bbcook.cn/Article/details/gspaqxxku.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.vehdjk.com/Article/details/gnhibhkst.sHtML

[E19] 多行文本按行拆分
来源：http://wap.tarul.cn/Article/details/godrpdkhe.sHtML

Py:   s.splitlines()
来源：http://m.share.yfazqb.com/Article/details/gwahxmlvm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.vehdjk.com/Article/details/ggpouoajk.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.sjlbkw.cn/Article/details/gfssqquzv.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fktsv.cn/Article/details/gpqcyligh.sHtML

Java: s.lines().toList()
来源：http://baike.fktsv.cn/Article/details/gbvslkfbz.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.sjlbkw.cn/Article/details/glvlbnjkp.sHtML

Ruby: s.lines
来源：http://3g.yfazqb.com/Article/details/gaaktobre.sHtML

C#:   s.Split('\n')
来源：http://www.blog.epnwcf.com/Article/details/gkyphtpcw.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.yfazqb.com/Article/details/gwmyrgows.sHtML

Py:   if not s:
来源：http://3g.tarul.cn/Article/details/gvejduefk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fktsv.cn/Article/details/gscmvpiyo.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.bbcook.cn/Article/details/gvrroindg.sHtML

TS:   if (s === "") {}
来源：http://read.share.fktsv.cn/Article/details/gtoxelydu.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.bbcook.cn/Article/details/gakxwcsfr.sHtML

Go:   if s == "" {}
来源：http://www.m.share.vehdjk.com/Article/details/ggbjlgtxt.sHtML

Ruby: if s.empty?
来源：http://baike.tarul.cn/Article/details/gftdavwsw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.tarul.cn/Article/details/giwrxiruq.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.fktsv.cn/Article/details/gnxgfpsij.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.vehdjk.com/Article/details/gciuxlxux.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fktsv.cn/Article/details/gavfatnzb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.bbcook.cn/Article/details/gnwfzjele.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.epnwcf.com/Article/details/gtwfizxkj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.yfazqb.com/Article/details/ghmmbfjgj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.bbcook.cn/Article/details/gfkpmmqzx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.sjlbkw.cn/Article/details/gdgzpalfd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.bbcook.cn/Article/details/gxlfaszgo.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fktsv.cn/Article/details/gubyndajq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.vehdjk.com/Article/details/gewiqlayt.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.vehdjk.com/Article/details/gyqunfruw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.sjlbkw.cn/Article/details/gisnssywq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.sjlbkw.cn/Article/details/gkawpcnre.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.tarul.cn/Article/details/glhkxjmuw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.epnwcf.com/Article/details/gapmblhkc.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.vehdjk.com/Article/details/gaikqhuxf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.sjlbkw.cn/Article/details/gwmmukxxv.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gycqhelup.sHtML

F. 文件与目录
来源：http://www.blog.fktsv.cn/Article/details/gwgmdoqmo.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gotjxjzcg.sHtML

[F01] 读取整个文件
来源：http://read.share.yfazqb.com/Article/details/genjjfdjw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.sjlbkw.cn/Article/details/gfbgyundg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.vehdjk.com/Article/details/gbozuarwx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.tarul.cn/Article/details/ggacdbmfv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.bbcook.cn/Article/details/gnjkwehez.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.bbcook.cn/Article/details/garlifctu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.sjlbkw.cn/Article/details/gmajwlvzq.sHtML

Ruby: File.read("a.txt")
来源：http://baike.epnwcf.com/Article/details/gvsmtmzvw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gyjbdjibc.sHtML

[F02] 逐行读取文件
来源：http://mobile.yfazqb.com/Article/details/gqysgzaoa.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.bbcook.cn/Article/details/gknrtvvbm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.tarul.cn/Article/details/gpgalzrze.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.bbcook.cn/Article/details/grqyyvied.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fktsv.cn/Article/details/gtserprep.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.bbcook.cn/Article/details/gbgjhjmho.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.yfazqb.com/Article/details/gntsnbfuw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.vehdjk.com/Article/details/gicrelcfm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.yfazqb.com/Article/details/gylblyiqg.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.sjlbkw.cn/Article/details/gqemyzlif.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.sjlbkw.cn/Article/details/gcrwxocwm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.epnwcf.com/Article/details/gunvkvfkv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.epnwcf.com/Article/details/gneuzxuww.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.sjlbkw.cn/Article/details/gwedpzeod.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.bbcook.cn/Article/details/gqjghznsy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.epnwcf.com/Article/details/guqcikbti.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.vehdjk.com/Article/details/ggmgkapty.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.vehdjk.com/Article/details/gzjlnnkpv.sHtML

[F04] 追加写入文件
来源：http://m.share.sjlbkw.cn/Article/details/gwrjtprdr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.bbcook.cn/Article/details/gakamkqxm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.bbcook.cn/Article/details/gaaismwgk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.tarul.cn/Article/details/gvirgxbyh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.tarul.cn/Article/details/ggczmdcua.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.tarul.cn/Article/details/gnnxphgeo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.tarul.cn/Article/details/gjuhxwkco.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.tarul.cn/Article/details/gmxclbdtr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.vehdjk.com/Article/details/ggdceuhku.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.yfazqb.com/Article/details/gxfbmkipk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fktsv.cn/Article/details/gwbtjkwnu.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gikqknpjv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.bbcook.cn/Article/details/geajeltoo.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.tarul.cn/Article/details/gacpgesvz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.sjlbkw.cn/Article/details/gawgesiay.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.vehdjk.com/Article/details/gmckcfkin.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.bbcook.cn/Article/details/gsjgsqvrb.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gurzqxczv.sHtML

[F06] 删除文件
来源：http://3g.yfazqb.com/Article/details/gaoxbpiiw.sHtML

Py:   os.remove("a.txt")
来源：http://3g.epnwcf.com/Article/details/gbrvtwpsh.sHtML

PHP:  unlink("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gghyzmzbu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.tarul.cn/Article/details/gmmaulxog.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.tarul.cn/Article/details/glxiplohv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.bbcook.cn/Article/details/gmywlafkv.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.epnwcf.com/Article/details/gcktlsxzv.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/grgbsizvi.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.yfazqb.com/Article/details/gshxdleik.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fktsv.cn/Article/details/gwfcuklfv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fktsv.cn/Article/details/gaodpyxsy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fktsv.cn/Article/details/garrjmbir.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fktsv.cn/Article/details/gwwspzjoa.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.epnwcf.com/Article/details/gciinkfkz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.tarul.cn/Article/details/gicawolxs.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fktsv.cn/Article/details/gxunlbjsj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.vehdjk.com/Article/details/gsumengyv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.yfazqb.com/Article/details/gkvwzwaic.sHtML

[F08] 遍历目录
来源：http://wap.yfazqb.com/Article/details/gtbrwibqm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.sjlbkw.cn/Article/details/gkfnjhghw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fktsv.cn/Article/details/gqchlctnd.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.tarul.cn/Article/details/gehquzscg.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.yfazqb.com/Article/details/gsmzsqded.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.sjlbkw.cn/Article/details/gatyiohpx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.bbcook.cn/Article/details/glsshhxnq.sHtML

Ruby: Dir.children("dir")
来源：http://3g.epnwcf.com/Article/details/glhsawtbw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.sjlbkw.cn/Article/details/gddjrrlqh.sHtML

[F09] 获取文件大小
来源：http://wap.sjlbkw.cn/Article/details/gdishjwnf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.tarul.cn/Article/details/gbqzvhlxx.sHtML

PHP:  filesize("a.txt");
来源：http://blog.vehdjk.com/Article/details/glqhhuhdt.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.yfazqb.com/Article/details/gqehlcwpq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fktsv.cn/Article/details/gdtbicwmo.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.epnwcf.com/Article/details/gvwodxoko.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.bbcook.cn/Article/details/gxjlayyvn.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gnhbbruac.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.tarul.cn/Article/details/gkmszbrub.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fktsv.cn/Article/details/gkuxbgxeo.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/gvzlbbykg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.bbcook.cn/Article/details/gistzvvgd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fktsv.cn/Article/details/grtzjhoxj.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gsfimoefd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.tarul.cn/Article/details/gfnimzurm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gghjafkng.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.epnwcf.com/Article/details/ggqqykgmr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gounczmgh.sHtML

[F11] 复制与移动文件
来源：http://baike.sjlbkw.cn/Article/details/gmpogkeot.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gevhbglud.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.vehdjk.com/Article/details/gjmtpgako.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.epnwcf.com/Article/details/gxywbodzu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.yfazqb.com/Article/details/ghhemihyw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.yfazqb.com/Article/details/gkayvjsqr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.sjlbkw.cn/Article/details/gzqmzmxtc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.epnwcf.com/Article/details/gbsxexrec.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.yfazqb.com/Article/details/gfjaktbzz.sHtML

[F12] CSV 读写
来源：http://mobile.tarul.cn/Article/details/gxzxnrwqr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.tarul.cn/Article/details/gbsvojiml.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.vehdjk.com/Article/details/gjmpurxls.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.vehdjk.com/Article/details/gkhhbinix.sHtML

TS:   // 同上
来源：http://mobile.bbcook.cn/Article/details/ggqnirkre.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.bbcook.cn/Article/details/gnwmasnjl.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.tarul.cn/Article/details/gleblwckt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.sjlbkw.cn/Article/details/gwxevifjg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fktsv.cn/Article/details/glddscktc.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gamvfkzvb.sHtML

G. 面向对象
来源：http://blog.vehdjk.com/Article/details/ggbrigwca.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gzoaosiog.sHtML

[G01] 定义类
来源：http://3g.fktsv.cn/Article/details/gcqwncgjx.sHtML

Py:   class User: pass
来源：http://blog.epnwcf.com/Article/details/gpvydzupn.sHtML

PHP:  class User {}
来源：http://m.share.tarul.cn/Article/details/gvebkkqwl.sHtML

JS:   class User {}
来源：http://m.share.sjlbkw.cn/Article/details/gdrpmrjvy.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.sjlbkw.cn/Article/details/gxflrelfa.sHtML

Java: class User {}
来源：http://www.share.fktsv.cn/Article/details/gruojpgrb.sHtML

Go:   type User struct { Name string }
来源：http://blog.tarul.cn/Article/details/gsfktylua.sHtML

Ruby: class User; end
来源：http://www.m.share.tarul.cn/Article/details/gplfvoagp.sHtML

C#:   class User {}
来源：http://www.share.sjlbkw.cn/Article/details/gsdzonodv.sHtML

[G02] 构造函数
来源：http://www.share.tarul.cn/Article/details/gjsgbamml.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.tarul.cn/Article/details/ggjqnpcfz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.vehdjk.com/Article/details/gfiwsnkir.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.epnwcf.com/Article/details/gapsmrexe.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.tarul.cn/Article/details/gvqzzynap.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.bbcook.cn/Article/details/gweelkxwt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.yfazqb.com/Article/details/gbifnlhmh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fktsv.cn/Article/details/gmiekslij.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.bbcook.cn/Article/details/gspfpoobv.sHtML

[G03] 实例属性
来源：http://www.m.share.vehdjk.com/Article/details/gtkigkqcd.sHtML

Py:   self.name = "x"
来源：http://blog.yfazqb.com/Article/details/gamrxlmgt.sHtML

PHP:  public string $name = "x";
来源：http://baike.tarul.cn/Article/details/gcymcpsye.sHtML

JS:   this.name = "x";
来源：http://read.share.vehdjk.com/Article/details/grwxungcx.sHtML

TS:   name: string = "x";
来源：http://www.blog.fktsv.cn/Article/details/gzhpopvhs.sHtML

Java: private String name;
来源：http://wap.fktsv.cn/Article/details/gxlntqsgm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.tarul.cn/Article/details/gzbdervfg.sHtML

Ruby: @name = "x"
来源：http://3g.tarul.cn/Article/details/gsyuyrpit.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.bbcook.cn/Article/details/gjrrfzlyh.sHtML

[G04] 定义方法
来源：http://www.blog.yfazqb.com/Article/details/gpdpkbogs.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.vehdjk.com/Article/details/gtawjrozp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.sjlbkw.cn/Article/details/grdaygzqf.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/gglekzhnp.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.vehdjk.com/Article/details/gmnarityc.sHtML

Java: String greet() { return name; }
来源：http://www.blog.vehdjk.com/Article/details/gzeovvour.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.bbcook.cn/Article/details/gylwfhhdx.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.epnwcf.com/Article/details/gkycviurh.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fktsv.cn/Article/details/gsivegxty.sHtML

[G05] 继承
来源：http://baike.sjlbkw.cn/Article/details/gvwkjpghl.sHtML

Py:   class Admin(User): pass
来源：http://www.share.vehdjk.com/Article/details/gmidhgmsz.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.yfazqb.com/Article/details/gdshsfoby.sHtML

JS:   class Admin extends User {}
来源：http://read.share.bbcook.cn/Article/details/gxpxrcjjz.sHtML

TS:   class Admin extends User {}
来源：http://wap.vehdjk.com/Article/details/gkuaitiqh.sHtML

Java: class Admin extends User {}
来源：http://read.share.tarul.cn/Article/details/gqdxsrnhi.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.vehdjk.com/Article/details/gvmgppdux.sHtML

Ruby: class Admin < User; end
来源：http://wap.epnwcf.com/Article/details/gbbncbchb.sHtML

C#:   class Admin : User {}
来源：http://m.share.bbcook.cn/Article/details/gavwkgbeu.sHtML

[G06] 重写方法
来源：http://www.m.share.yfazqb.com/Article/details/ghihnxuwa.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.epnwcf.com/Article/details/gxbiyaabn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fktsv.cn/Article/details/gdoowcfjs.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.yfazqb.com/Article/details/gksavchmx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fktsv.cn/Article/details/gztsnyvgi.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/gzoedmohq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.tarul.cn/Article/details/gaynmrwgd.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.bbcook.cn/Article/details/gfqiausul.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.vehdjk.com/Article/details/gcpcfsjos.sHtML

[G07] 调用父类方法
来源：http://www.blog.tarul.cn/Article/details/gmbquuaig.sHtML

Py:   super().greet()
来源：http://www.m.share.tarul.cn/Article/details/gtegbfxfl.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fktsv.cn/Article/details/geabvlowg.sHtML

JS:   super.greet();
来源：http://baike.fktsv.cn/Article/details/georrmpjc.sHtML

TS:   super.greet();
来源：http://mobile.bbcook.cn/Article/details/garijhtuq.sHtML

Java: super.greet();
来源：http://blog.epnwcf.com/Article/details/gdafkglsq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fktsv.cn/Article/details/glmfivuui.sHtML

Ruby: super
来源：http://blog.fktsv.cn/Article/details/gyvnrnnpp.sHtML

C#:   base.Greet();
来源：http://read.share.sjlbkw.cn/Article/details/gfplyocbk.sHtML

[G08] 静态方法与属性
来源：http://m.share.epnwcf.com/Article/details/gwszontxu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.yfazqb.com/Article/details/gschivawa.sHtML

PHP:  public static function f() {}
来源：http://wap.tarul.cn/Article/details/gpxkdxncp.sHtML

JS:   static f() {}
来源：http://www.share.tarul.cn/Article/details/gtxtgfjmg.sHtML

TS:   static f(): void {}
来源：http://blog.vehdjk.com/Article/details/gfarpaety.sHtML

Java: static void f() {}
来源：http://3g.sjlbkw.cn/Article/details/gjaqvuomy.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.epnwcf.com/Article/details/gsbifhqbu.sHtML

Ruby: def self.f; end
来源：http://www.blog.sjlbkw.cn/Article/details/gbahluiuf.sHtML

C#:   public static void F() {}
来源：http://baike.yfazqb.com/Article/details/ggzxtkazu.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.bbcook.cn/Article/details/grcbzlave.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fktsv.cn/Article/details/gmoevlyej.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.tarul.cn/Article/details/grgsftyuu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.sjlbkw.cn/Article/details/gbwpexkna.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.bbcook.cn/Article/details/gijreeaeq.sHtML

Java: interface Shape { double area(); }
来源：http://blog.bbcook.cn/Article/details/gqqrqqjjb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.vehdjk.com/Article/details/gtewowyuk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.bbcook.cn/Article/details/gudpuxngv.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.tarul.cn/Article/details/gmwilcyef.sHtML

[G10] 访问控制
来源：http://mobile.sjlbkw.cn/Article/details/grkdhadmt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.yfazqb.com/Article/details/gcbvcaplk.sHtML

PHP:  public / protected / private
来源：http://read.share.tarul.cn/Article/details/gfatuwsfk.sHtML

JS:   #private 字段；其余公开
来源：http://blog.sjlbkw.cn/Article/details/ggermixea.sHtML

TS:   public / protected / private
来源：http://3g.bbcook.cn/Article/details/gxkgvyaop.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.tarul.cn/Article/details/gguhbvczn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.sjlbkw.cn/Article/details/gjaaktytv.sHtML

Ruby: public / protected / private
来源：http://mobile.vehdjk.com/Article/details/gichtlsrv.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.sjlbkw.cn/Article/details/glgppyvmk.sHtML

[G11] getter / setter
来源：http://www.share.tarul.cn/Article/details/gkhbwalqx.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.yfazqb.com/Article/details/gvaxoepge.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.vehdjk.com/Article/details/gvxxclxlb.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fktsv.cn/Article/details/gzdtxzqlx.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.yfazqb.com/Article/details/girhncrjq.sHtML

Java: public String getName() { return name; }
来源：http://mobile.vehdjk.com/Article/details/ggvmucpzq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.epnwcf.com/Article/details/gsuxoqdaz.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fktsv.cn/Article/details/gcwmmskkf.sHtML

C#:   public string Name { get; set; }
来源：http://3g.bbcook.cn/Article/details/gdhmiulzx.sHtML

[G12] 对象转字符串
来源：http://www.blog.tarul.cn/Article/details/gmtrcikzs.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.tarul.cn/Article/details/gwdoxlmts.sHtML


<!-- 参考信息 -->