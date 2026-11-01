代发 wailian999

PHP:  substr_count($s, "a");
来源：http://m.share.yfazqb.com/Article/details/gvgxfnnvc.sHtML

JS:   s.split("a").length - 1
来源：http://blog.yfazqb.com/Article/details/gocymyysv.sHtML

TS:   s.split("a").length - 1
来源：http://baike.yfazqb.com/Article/details/ghmruxyon.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.vehdjk.com/Article/details/gbwpqjcfg.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.sjlbkw.cn/Article/details/glweaaqen.sHtML

Ruby: s.count("a")
来源：http://read.share.bbcook.cn/Article/details/gnrwyfpaq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.epnwcf.com/Article/details/gniyrbros.sHtML

[E13] 逐字符遍历
来源：http://read.share.epnwcf.com/Article/details/gbmgxjcyq.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.yfazqb.com/Article/details/ghkagmccu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.bbcook.cn/Article/details/gkskodphs.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.sjlbkw.cn/Article/details/gbyqteyqe.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.epnwcf.com/Article/details/glzirafli.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.bbcook.cn/Article/details/gwykrprnf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.fktsv.cn/Article/details/gyzmikszw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.vehdjk.com/Article/details/gvdsqgdrg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.tarul.cn/Article/details/ggsskjvmz.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.yfazqb.com/Article/details/gjdcdkqss.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.epnwcf.com/Article/details/gtrrdujge.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fktsv.cn/Article/details/gwrgfvzjp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.bbcook.cn/Article/details/giylumelr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.tarul.cn/Article/details/gqecpmxim.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.vehdjk.com/Article/details/gyoqivepa.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.epnwcf.com/Article/details/gtmrfowkd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.tarul.cn/Article/details/gkhpapyzx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.epnwcf.com/Article/details/ggvzmdddq.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.tarul.cn/Article/details/goptjarqb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fktsv.cn/Article/details/gzgireezl.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.tarul.cn/Article/details/gdaxrotof.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.tarul.cn/Article/details/gtgtvxgnb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.vehdjk.com/Article/details/gktmkxbkh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.epnwcf.com/Article/details/gjezfoiln.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.sjlbkw.cn/Article/details/gpvumrahb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.epnwcf.com/Article/details/ggpbmfpvf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.epnwcf.com/Article/details/gskgexwqf.sHtML

[E16] 数字千分位
来源：http://www.blog.yfazqb.com/Article/details/gdpwvjyvg.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.tarul.cn/Article/details/gquemcosx.sHtML

PHP:  number_format(1234567);
来源：http://blog.sjlbkw.cn/Article/details/ghuuwwqrc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.vehdjk.com/Article/details/gawrcyiwt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.sjlbkw.cn/Article/details/gvxpcwuqj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fktsv.cn/Article/details/gyyyxxnuf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.vehdjk.com/Article/details/gdimxldpa.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.epnwcf.com/Article/details/gqoorgbpe.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.bbcook.cn/Article/details/grchzbacn.sHtML

[E17] 首字母大写
来源：http://mobile.vehdjk.com/Article/details/gtdukurfr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fktsv.cn/Article/details/goundwfqi.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.bbcook.cn/Article/details/gteflnfic.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fktsv.cn/Article/details/gmvvnsnjf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnnynqxsf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.sjlbkw.cn/Article/details/gvcvmjvpj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.sjlbkw.cn/Article/details/gtqzcxnzy.sHtML

Ruby: s.capitalize
来源：http://mobile.sjlbkw.cn/Article/details/gcbjspvku.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.sjlbkw.cn/Article/details/gmtvxwema.sHtML

[E18] 模板占位符替换
来源：http://mobile.vehdjk.com/Article/details/gcomrafah.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.bbcook.cn/Article/details/grsbuacrg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.tarul.cn/Article/details/giabanxuz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.yfazqb.com/Article/details/gfgdrdjlh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fktsv.cn/Article/details/gogwrtywv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.sjlbkw.cn/Article/details/gsphgcujm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fktsv.cn/Article/details/guhkfdgff.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.sjlbkw.cn/Article/details/gjrlznmxw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.bbcook.cn/Article/details/gyqfgziaf.sHtML

[E19] 多行文本按行拆分
来源：http://wap.bbcook.cn/Article/details/gfxkqsonz.sHtML

Py:   s.splitlines()
来源：http://m.share.tarul.cn/Article/details/gmksigdte.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fktsv.cn/Article/details/gbjmlhwfi.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.yfazqb.com/Article/details/gizpbpdcx.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.tarul.cn/Article/details/gdphlxxxz.sHtML

Java: s.lines().toList()
来源：http://www.share.bbcook.cn/Article/details/guvmznehb.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.tarul.cn/Article/details/gxnkhefcc.sHtML

Ruby: s.lines
来源：http://blog.vehdjk.com/Article/details/gssfnkxmv.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.epnwcf.com/Article/details/gdffyesqs.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.bbcook.cn/Article/details/gtvijhqtu.sHtML

Py:   if not s:
来源：http://www.m.share.vehdjk.com/Article/details/gkejzumqf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fktsv.cn/Article/details/gottuxtvs.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.yfazqb.com/Article/details/gsrwylodn.sHtML

TS:   if (s === "") {}
来源：http://wap.bbcook.cn/Article/details/gvmspyzkd.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.vehdjk.com/Article/details/gjptcjuaw.sHtML

Go:   if s == "" {}
来源：http://3g.sjlbkw.cn/Article/details/gwpwpgqms.sHtML

Ruby: if s.empty?
来源：http://www.share.bbcook.cn/Article/details/geiamntmv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.vehdjk.com/Article/details/gwfzojyed.sHtML

[E21] 超长截断加省略号
来源：http://3g.sjlbkw.cn/Article/details/gxbazomzh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.bbcook.cn/Article/details/gibtxqflr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.epnwcf.com/Article/details/graqccwhx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.bbcook.cn/Article/details/guheeuucd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fktsv.cn/Article/details/gayvoodnu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gkdenyqok.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.bbcook.cn/Article/details/ggejsyiin.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fktsv.cn/Article/details/ghmtmwabu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.yfazqb.com/Article/details/gmrubepoh.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fktsv.cn/Article/details/gewneenqv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.yfazqb.com/Article/details/gekmlnusb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.bbcook.cn/Article/details/gktwatbpc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.sjlbkw.cn/Article/details/gkubwzspd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.yfazqb.com/Article/details/gluslbgjt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.yfazqb.com/Article/details/gthvyrbfu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.tarul.cn/Article/details/gfkukozao.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.vehdjk.com/Article/details/gloktibru.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.tarul.cn/Article/details/gbczcrnek.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gmfgilron.sHtML

F. 文件与目录
来源：http://read.share.fktsv.cn/Article/details/goiuakzcw.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gyrqucwgn.sHtML

[F01] 读取整个文件
来源：http://blog.fktsv.cn/Article/details/ghxedpyxr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fktsv.cn/Article/details/ghtmfjqsi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gazhkdsjj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.epnwcf.com/Article/details/ghrwefwve.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fktsv.cn/Article/details/gndxlqtzl.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.tarul.cn/Article/details/gxxwojldx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.sjlbkw.cn/Article/details/gwvglpbhl.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gzjxcuxay.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.vehdjk.com/Article/details/gqtrzqqso.sHtML

[F02] 逐行读取文件
来源：http://www.share.epnwcf.com/Article/details/gutkorrft.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.yfazqb.com/Article/details/gxywwdmpn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.sjlbkw.cn/Article/details/gbocosjfd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.epnwcf.com/Article/details/gwulxxmqp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.vehdjk.com/Article/details/gvvzdsiom.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.sjlbkw.cn/Article/details/gmktiocey.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.vehdjk.com/Article/details/ghtvhjdjp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.sjlbkw.cn/Article/details/giziuvjtg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.vehdjk.com/Article/details/gvtqoipgj.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.yfazqb.com/Article/details/ggzcygksr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.vehdjk.com/Article/details/gcxvpofek.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.yfazqb.com/Article/details/gfvlbsuev.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.bbcook.cn/Article/details/gncwhvhlq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.sjlbkw.cn/Article/details/gzingmqxb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.bbcook.cn/Article/details/gvepwuawp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.tarul.cn/Article/details/gpqzowioy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.yfazqb.com/Article/details/gufugaicu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fktsv.cn/Article/details/gswquhtxc.sHtML

[F04] 追加写入文件
来源：http://mobile.yfazqb.com/Article/details/gcyblxxph.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.tarul.cn/Article/details/gzmalpepx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.yfazqb.com/Article/details/ggrganuxk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.epnwcf.com/Article/details/gyygnlpsj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.bbcook.cn/Article/details/gfuhisoiz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.sjlbkw.cn/Article/details/gmsbpttbb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.bbcook.cn/Article/details/grjzrusus.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.tarul.cn/Article/details/gcvtdtinf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.sjlbkw.cn/Article/details/gyvevcens.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.bbcook.cn/Article/details/gcemnzsuw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.sjlbkw.cn/Article/details/gdwlklija.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gwqurgfpk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gchbemlzk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gfveklugo.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.yfazqb.com/Article/details/gztbxwefy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.bbcook.cn/Article/details/gvkuhgbsv.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gkzkwjvdb.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.vehdjk.com/Article/details/gghbgwhwk.sHtML

[F06] 删除文件
来源：http://www.m.share.epnwcf.com/Article/details/gutjhmwjg.sHtML

Py:   os.remove("a.txt")
来源：http://blog.tarul.cn/Article/details/gcsebhsbn.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gcrajmbgi.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gteazkijm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fktsv.cn/Article/details/godvfstgd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.vehdjk.com/Article/details/glxamefjp.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.epnwcf.com/Article/details/gymrpvsew.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gokyhqwbw.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gosfsuqxi.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fktsv.cn/Article/details/gxeoqwdok.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.tarul.cn/Article/details/gzsxbhknz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.bbcook.cn/Article/details/gxmgvdkwa.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.yfazqb.com/Article/details/gemmtxwvm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.epnwcf.com/Article/details/ghlwxuksi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gcveynarp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.yfazqb.com/Article/details/gmnkinebi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.yfazqb.com/Article/details/gkputulmp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.tarul.cn/Article/details/gjvcwyukq.sHtML

[F08] 遍历目录
来源：http://read.share.epnwcf.com/Article/details/gamxtyjmo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.epnwcf.com/Article/details/gjahntyhn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.sjlbkw.cn/Article/details/gxpcxdibu.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.sjlbkw.cn/Article/details/gqkhuvbmf.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.yfazqb.com/Article/details/gohzhoyvj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.epnwcf.com/Article/details/gjodspbqo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.tarul.cn/Article/details/gdafeagxl.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fktsv.cn/Article/details/gnuoowmkb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.bbcook.cn/Article/details/gwvcwhppx.sHtML

[F09] 获取文件大小
来源：http://blog.bbcook.cn/Article/details/gzejpumsy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/guftehcht.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.bbcook.cn/Article/details/gwqvagwvo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.bbcook.cn/Article/details/guddipijc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.vehdjk.com/Article/details/gxujuebnd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fktsv.cn/Article/details/gbxaejzkh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.bbcook.cn/Article/details/giepvalno.sHtML

Ruby: File.size("a.txt")
来源：http://baike.epnwcf.com/Article/details/gmaksvtve.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.epnwcf.com/Article/details/gqudoicfb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.vehdjk.com/Article/details/gbiqxuvyb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fktsv.cn/Article/details/gkqgkgmdg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fktsv.cn/Article/details/gekjhulrl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/gsfsolfwx.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gsrqpitot.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.epnwcf.com/Article/details/gzicvytpm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.vehdjk.com/Article/details/gscrhjann.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/gataclazw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/ghhoqaluw.sHtML

[F11] 复制与移动文件
来源：http://www.blog.epnwcf.com/Article/details/gnqcpbrgf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/gdebbufft.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.yfazqb.com/Article/details/giyihxbtc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.epnwcf.com/Article/details/gdkopsfbx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.vehdjk.com/Article/details/gpmuhpncf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fktsv.cn/Article/details/ghrfqihdw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.yfazqb.com/Article/details/gacfsfeuz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.tarul.cn/Article/details/geiwylhua.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.bbcook.cn/Article/details/gdhljwknx.sHtML

[F12] CSV 读写
来源：http://blog.fktsv.cn/Article/details/gwfqvexdo.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fktsv.cn/Article/details/gfetlmkeu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.vehdjk.com/Article/details/gnbeebmdl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.vehdjk.com/Article/details/ghjloankq.sHtML

TS:   // 同上
来源：http://blog.vehdjk.com/Article/details/gdxuwlzal.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.sjlbkw.cn/Article/details/gicjyksuy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.tarul.cn/Article/details/goxrlpvqh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.yfazqb.com/Article/details/gnegsyior.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.sjlbkw.cn/Article/details/gajpamrve.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gpolymsae.sHtML

G. 面向对象
来源：http://www.share.bbcook.cn/Article/details/gorxdfjnf.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gohjastvh.sHtML

[G01] 定义类
来源：http://wap.bbcook.cn/Article/details/gcoqdidvx.sHtML

Py:   class User: pass
来源：http://www.blog.epnwcf.com/Article/details/gudzcvztj.sHtML

PHP:  class User {}
来源：http://www.blog.fktsv.cn/Article/details/gthsyxhng.sHtML

JS:   class User {}
来源：http://www.share.bbcook.cn/Article/details/gpbnyeibx.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.vehdjk.com/Article/details/gpigovlti.sHtML

Java: class User {}
来源：http://wap.bbcook.cn/Article/details/goljxtnkh.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjmbknofk.sHtML

Ruby: class User; end
来源：http://3g.bbcook.cn/Article/details/gmlznnjfi.sHtML

C#:   class User {}
来源：http://3g.fktsv.cn/Article/details/ggjyazdvy.sHtML

[G02] 构造函数
来源：http://blog.sjlbkw.cn/Article/details/geiupihqj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.yfazqb.com/Article/details/grmndadnm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fktsv.cn/Article/details/gqujtkrzu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.tarul.cn/Article/details/gzpdsdyqo.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.epnwcf.com/Article/details/gyktxaegn.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.vehdjk.com/Article/details/gnoitehgb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.epnwcf.com/Article/details/gmvgrhvqc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fktsv.cn/Article/details/gqqecarzw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.bbcook.cn/Article/details/gembodlct.sHtML

[G03] 实例属性
来源：http://www.m.share.sjlbkw.cn/Article/details/gyimevifw.sHtML

Py:   self.name = "x"
来源：http://www.blog.yfazqb.com/Article/details/gjxglpkvw.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fktsv.cn/Article/details/gigaqjvse.sHtML

JS:   this.name = "x";
来源：http://mobile.epnwcf.com/Article/details/gzondpxtl.sHtML

TS:   name: string = "x";
来源：http://blog.vehdjk.com/Article/details/gyomztkhf.sHtML

Java: private String name;
来源：http://www.blog.sjlbkw.cn/Article/details/gbrxxmkar.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.sjlbkw.cn/Article/details/gafnoxapi.sHtML

Ruby: @name = "x"
来源：http://m.share.sjlbkw.cn/Article/details/gjztlwbgw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.vehdjk.com/Article/details/ggzbmrnkr.sHtML

[G04] 定义方法
来源：http://m.share.epnwcf.com/Article/details/gdhjhagtq.sHtML

Py:   def greet(self): return self.name
来源：http://blog.yfazqb.com/Article/details/gxmywytqo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.tarul.cn/Article/details/guyhmjhpc.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.yfazqb.com/Article/details/gxnzxdebs.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.epnwcf.com/Article/details/gadevnvfp.sHtML

Java: String greet() { return name; }
来源：http://mobile.yfazqb.com/Article/details/gtnmfzwdn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.bbcook.cn/Article/details/glytvjscd.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fktsv.cn/Article/details/gonckzhcw.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.bbcook.cn/Article/details/goinfqrez.sHtML

[G05] 继承
来源：http://baike.yfazqb.com/Article/details/gxysrzzch.sHtML

Py:   class Admin(User): pass
来源：http://blog.fktsv.cn/Article/details/gbmpbnahn.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.bbcook.cn/Article/details/gucbvdgpv.sHtML

JS:   class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/gqcubnndp.sHtML

TS:   class Admin extends User {}
来源：http://baike.tarul.cn/Article/details/gjjhlrfhd.sHtML

Java: class Admin extends User {}
来源：http://read.share.yfazqb.com/Article/details/gzmqdscjc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.vehdjk.com/Article/details/glbridliq.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.tarul.cn/Article/details/gfvqlpeee.sHtML

C#:   class Admin : User {}
来源：http://wap.epnwcf.com/Article/details/ghxyxdtlr.sHtML

[G06] 重写方法
来源：http://www.share.yfazqb.com/Article/details/ghyshyvsm.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.vehdjk.com/Article/details/gbehohudl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.sjlbkw.cn/Article/details/gduqihuly.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.tarul.cn/Article/details/gbjsbovns.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fktsv.cn/Article/details/gwgdvwcii.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.yfazqb.com/Article/details/gqmlucbco.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.yfazqb.com/Article/details/gzzgwcusy.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.vehdjk.com/Article/details/gpkwjjcyx.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.epnwcf.com/Article/details/guwxzlbuv.sHtML

[G07] 调用父类方法
来源：http://www.m.share.yfazqb.com/Article/details/gggctusug.sHtML

Py:   super().greet()
来源：http://3g.bbcook.cn/Article/details/gmxkywvrm.sHtML

PHP:  parent::greet();
来源：http://www.share.epnwcf.com/Article/details/gikdholuj.sHtML

JS:   super.greet();
来源：http://www.blog.bbcook.cn/Article/details/gpedzssyj.sHtML

TS:   super.greet();
来源：http://www.share.bbcook.cn/Article/details/golrdimra.sHtML

Java: super.greet();
来源：http://www.m.share.fktsv.cn/Article/details/goitbpbua.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.bbcook.cn/Article/details/gquqxmuvj.sHtML

Ruby: super
来源：http://wap.fktsv.cn/Article/details/gvtyyniii.sHtML

C#:   base.Greet();
来源：http://m.share.yfazqb.com/Article/details/gkujjvpnq.sHtML

[G08] 静态方法与属性
来源：http://mobile.fktsv.cn/Article/details/gaqagyyys.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.bbcook.cn/Article/details/gfvfkrxld.sHtML

PHP:  public static function f() {}
来源：http://baike.vehdjk.com/Article/details/grkyyebot.sHtML

JS:   static f() {}
来源：http://wap.epnwcf.com/Article/details/govfbaqpj.sHtML

TS:   static f(): void {}
来源：http://wap.tarul.cn/Article/details/gfdestqzq.sHtML

Java: static void f() {}
来源：http://www.blog.fktsv.cn/Article/details/gesknodqd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.sjlbkw.cn/Article/details/goeicwiee.sHtML

Ruby: def self.f; end
来源：http://www.share.vehdjk.com/Article/details/gjvkhayku.sHtML

C#:   public static void F() {}
来源：http://www.m.share.yfazqb.com/Article/details/gbekskjbl.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.tarul.cn/Article/details/gcytwwmnu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fktsv.cn/Article/details/gyrkcmtak.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkisgljay.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fktsv.cn/Article/details/gpwymskxj.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.tarul.cn/Article/details/gazqjtbca.sHtML

Java: interface Shape { double area(); }
来源：http://3g.vehdjk.com/Article/details/giicoymgt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.tarul.cn/Article/details/gcyhnhxge.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.epnwcf.com/Article/details/gbkyqnasq.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fktsv.cn/Article/details/gdspbbxay.sHtML

[G10] 访问控制
来源：http://blog.vehdjk.com/Article/details/gqiynnhff.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.bbcook.cn/Article/details/gethpluwv.sHtML

PHP:  public / protected / private
来源：http://3g.tarul.cn/Article/details/guqdchzkw.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.vehdjk.com/Article/details/gcremqpfi.sHtML

TS:   public / protected / private
来源：http://wap.fktsv.cn/Article/details/gvhnaonme.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.bbcook.cn/Article/details/gfknihbch.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.vehdjk.com/Article/details/ghxbvunpe.sHtML

Ruby: public / protected / private
来源：http://www.share.tarul.cn/Article/details/gxvhbaymw.sHtML


<!-- 参考信息 -->