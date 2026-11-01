代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fktsv.cn/Article/details/goqsntxam.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.yfazqb.com/Article/details/giqpiltjx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.sjlbkw.cn/Article/details/gurarwlta.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.epnwcf.com/Article/details/gnktouhcz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.epnwcf.com/Article/details/ggtztheyx.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.vehdjk.com/Article/details/gaecdggqm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.sjlbkw.cn/Article/details/gjnkrfcdz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fktsv.cn/Article/details/gvesjcasx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.tarul.cn/Article/details/gbndlfpbf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.tarul.cn/Article/details/gloeqcgag.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.epnwcf.com/Article/details/gwjcwppsq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.vehdjk.com/Article/details/gvfwbdpdr.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.bbcook.cn/Article/details/gfsitobdc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.sjlbkw.cn/Article/details/gnzsacvpn.sHtML

[E16] 数字千分位
来源：http://mobile.tarul.cn/Article/details/gphmrizcn.sHtML

Py:   f"{1234567:,}"
来源：http://3g.vehdjk.com/Article/details/gunkyvvmb.sHtML

PHP:  number_format(1234567);
来源：http://www.share.yfazqb.com/Article/details/gtxsxfghr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.sjlbkw.cn/Article/details/gmmozaixp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.tarul.cn/Article/details/gukwqpfox.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.vehdjk.com/Article/details/gqpgopyjv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.tarul.cn/Article/details/gwtnxskvd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.sjlbkw.cn/Article/details/gnhiumgxv.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fktsv.cn/Article/details/gsvehhwok.sHtML

[E17] 首字母大写
来源：http://mobile.epnwcf.com/Article/details/giiymeptp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.epnwcf.com/Article/details/gxaktflmj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.tarul.cn/Article/details/gmmutvknn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.vehdjk.com/Article/details/gfwansunw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.tarul.cn/Article/details/goytcmkut.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.sjlbkw.cn/Article/details/gnohtouzi.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.vehdjk.com/Article/details/gysxnrszq.sHtML

Ruby: s.capitalize
来源：http://blog.fktsv.cn/Article/details/gdzxdaubo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.yfazqb.com/Article/details/goyehxdfr.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fktsv.cn/Article/details/gerknhvlc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.sjlbkw.cn/Article/details/gyvknncex.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.bbcook.cn/Article/details/gcjaecmif.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.bbcook.cn/Article/details/gayvqsadu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.bbcook.cn/Article/details/gqjrhskeu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.tarul.cn/Article/details/gbhpdlhcs.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.sjlbkw.cn/Article/details/gyqqaxrsl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.sjlbkw.cn/Article/details/gzlxxqnez.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.sjlbkw.cn/Article/details/ggkcodajj.sHtML

[E19] 多行文本按行拆分
来源：http://3g.yfazqb.com/Article/details/gshznfmch.sHtML

Py:   s.splitlines()
来源：http://read.share.bbcook.cn/Article/details/ggtzbwiph.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.vehdjk.com/Article/details/gftjkshoq.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.bbcook.cn/Article/details/gqcnfdryu.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.tarul.cn/Article/details/gfrnylpyx.sHtML

Java: s.lines().toList()
来源：http://blog.vehdjk.com/Article/details/gqhzukqip.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fktsv.cn/Article/details/gvpoamlrz.sHtML

Ruby: s.lines
来源：http://m.share.fktsv.cn/Article/details/gzznpheaa.sHtML

C#:   s.Split('\n')
来源：http://mobile.vehdjk.com/Article/details/gzhtbnkqy.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.vehdjk.com/Article/details/gudraifsy.sHtML

Py:   if not s:
来源：http://mobile.epnwcf.com/Article/details/gnufgsltx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.yfazqb.com/Article/details/gxkbcxqwz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gwdonxvna.sHtML

TS:   if (s === "") {}
来源：http://wap.tarul.cn/Article/details/gwbbiczer.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.vehdjk.com/Article/details/gzjopshsj.sHtML

Go:   if s == "" {}
来源：http://www.share.epnwcf.com/Article/details/gkjujydok.sHtML

Ruby: if s.empty?
来源：http://mobile.sjlbkw.cn/Article/details/gxxefsmzn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.epnwcf.com/Article/details/gujzevlbg.sHtML

[E21] 超长截断加省略号
来源：http://www.share.tarul.cn/Article/details/gryihpbjt.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.yfazqb.com/Article/details/gubehpqvp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fktsv.cn/Article/details/gskryitgi.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gajwpdfti.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.bbcook.cn/Article/details/gjbcigpgz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.vehdjk.com/Article/details/gdspebwpp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.sjlbkw.cn/Article/details/gvsqsqpcl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/gyzhgrywr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.yfazqb.com/Article/details/glwzvosha.sHtML

[E22] 字节长度与字符长度
来源：http://3g.vehdjk.com/Article/details/gedjxtngl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.bbcook.cn/Article/details/gevkginnx.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.bbcook.cn/Article/details/gswhkspjt.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fktsv.cn/Article/details/gagpwbquz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.vehdjk.com/Article/details/ghwthuzjs.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.bbcook.cn/Article/details/giwmpgmlu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.yfazqb.com/Article/details/gqmmvxdpt.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.tarul.cn/Article/details/gtneetnzr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.bbcook.cn/Article/details/gndxygsfd.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/glnfockoj.sHtML

F. 文件与目录
来源：http://m.share.vehdjk.com/Article/details/gpwgjxrke.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/giugmdgws.sHtML

[F01] 读取整个文件
来源：http://m.share.bbcook.cn/Article/details/glseexryu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.bbcook.cn/Article/details/gojljveoz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gntnkawnb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.vehdjk.com/Article/details/gghdahbzd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.epnwcf.com/Article/details/gopuftxud.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.yfazqb.com/Article/details/gqpxuryej.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.bbcook.cn/Article/details/gluivjykh.sHtML

Ruby: File.read("a.txt")
来源：http://3g.bbcook.cn/Article/details/gybdtdmoe.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.bbcook.cn/Article/details/gswnwqyla.sHtML

[F02] 逐行读取文件
来源：http://3g.yfazqb.com/Article/details/ggnldmmwj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.yfazqb.com/Article/details/gxvmavgdk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.yfazqb.com/Article/details/gatnpyhtn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.bbcook.cn/Article/details/giwadfquq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.bbcook.cn/Article/details/giwnarnzk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.sjlbkw.cn/Article/details/gzclliyly.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.epnwcf.com/Article/details/gmmracggv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.bbcook.cn/Article/details/goammuuqx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.bbcook.cn/Article/details/giffnxcjs.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.bbcook.cn/Article/details/gpuibwhko.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.bbcook.cn/Article/details/ggmhdvuxh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fktsv.cn/Article/details/ggfqpbprn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.sjlbkw.cn/Article/details/gadfqukjk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.bbcook.cn/Article/details/gxalwivqp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.sjlbkw.cn/Article/details/godanqoft.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.sjlbkw.cn/Article/details/gpfykpoeh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.sjlbkw.cn/Article/details/gfvgsyhzs.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.epnwcf.com/Article/details/gphkddlvf.sHtML

[F04] 追加写入文件
来源：http://read.share.tarul.cn/Article/details/gzeglvkxv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.bbcook.cn/Article/details/gqvsgrdxr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.tarul.cn/Article/details/gxtbuzyrx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.tarul.cn/Article/details/gmmddbqdv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.tarul.cn/Article/details/gwsvvjgiw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.bbcook.cn/Article/details/gzmoabxdg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.tarul.cn/Article/details/gecqfdbes.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.yfazqb.com/Article/details/glocsqouv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.sjlbkw.cn/Article/details/gtuixmfyn.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.vehdjk.com/Article/details/gytqsrnud.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.tarul.cn/Article/details/glarhmskh.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gzeueszpi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.bbcook.cn/Article/details/glulzcbsr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gmmyqbbuq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.tarul.cn/Article/details/glvtakbls.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.bbcook.cn/Article/details/gdfpyslpk.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fktsv.cn/Article/details/ggddnivid.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gepjojkqp.sHtML

[F06] 删除文件
来源：http://www.share.fktsv.cn/Article/details/gkciupqwq.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gwbpqipjx.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gkatzxebn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gismkxibu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/ghwjjnjmq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.epnwcf.com/Article/details/gppfcbmfr.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.tarul.cn/Article/details/gtczwupcu.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.epnwcf.com/Article/details/geckhjzxe.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.bbcook.cn/Article/details/gggnpkjse.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.epnwcf.com/Article/details/gsofrdeen.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fktsv.cn/Article/details/gzupejhgu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.sjlbkw.cn/Article/details/gcyighjbp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.vehdjk.com/Article/details/gmxgkibuk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.bbcook.cn/Article/details/glbgmpfmf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.yfazqb.com/Article/details/gxwbhcjhm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.tarul.cn/Article/details/gwhgeqvin.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.sjlbkw.cn/Article/details/gevitkrxr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.vehdjk.com/Article/details/gqkiupdkv.sHtML

[F08] 遍历目录
来源：http://baike.tarul.cn/Article/details/gmyryagtk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.yfazqb.com/Article/details/ghqlcpwnc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.bbcook.cn/Article/details/guizkpxhu.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.epnwcf.com/Article/details/grktnvgut.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.yfazqb.com/Article/details/gmrfzwtbv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.vehdjk.com/Article/details/gihsvpaba.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fktsv.cn/Article/details/getoqksva.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.yfazqb.com/Article/details/guaxzlsqg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.bbcook.cn/Article/details/gemvephej.sHtML

[F09] 获取文件大小
来源：http://3g.vehdjk.com/Article/details/gfwdimekt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gaifdzgjd.sHtML

PHP:  filesize("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/ghfncbmbw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.vehdjk.com/Article/details/gauxtxvsk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.bbcook.cn/Article/details/gbxemnlac.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/ghbenjgak.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.tarul.cn/Article/details/gwnhuxsbg.sHtML

Ruby: File.size("a.txt")
来源：http://blog.tarul.cn/Article/details/guvpueohq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.epnwcf.com/Article/details/gbwqamrnn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.sjlbkw.cn/Article/details/gvvpijvoi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.vehdjk.com/Article/details/gdxgcudcu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.vehdjk.com/Article/details/gnrninitz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/gxpbswwbs.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gmenommiu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.bbcook.cn/Article/details/gizsclaid.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gzirukydd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/gwrdmfuna.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.bbcook.cn/Article/details/gqcvkcrug.sHtML

[F11] 复制与移动文件
来源：http://baike.fktsv.cn/Article/details/gltcewvfm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.tarul.cn/Article/details/gzzyfbmsf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.bbcook.cn/Article/details/grfqejann.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.vehdjk.com/Article/details/gammjmkhg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.tarul.cn/Article/details/gtlrsiohg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.epnwcf.com/Article/details/gjqeugbog.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.sjlbkw.cn/Article/details/gderhyvvy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.tarul.cn/Article/details/gmjghqeep.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.vehdjk.com/Article/details/gxbrbuhaq.sHtML

[F12] CSV 读写
来源：http://www.blog.tarul.cn/Article/details/gobibvqpw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fktsv.cn/Article/details/gmvasmltk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.yfazqb.com/Article/details/gabjbyauz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fktsv.cn/Article/details/gihucvpnu.sHtML

TS:   // 同上
来源：http://mobile.tarul.cn/Article/details/gedghzoeh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.tarul.cn/Article/details/gbsshubbt.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.yfazqb.com/Article/details/ggdiuajkj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.sjlbkw.cn/Article/details/gukkhcyzo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.yfazqb.com/Article/details/gqxiwxehh.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gagijncal.sHtML

G. 面向对象
来源：http://www.blog.fktsv.cn/Article/details/gcynunboy.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gyomdhgfy.sHtML

[G01] 定义类
来源：http://www.m.share.epnwcf.com/Article/details/gznyclrmr.sHtML

Py:   class User: pass
来源：http://www.m.share.sjlbkw.cn/Article/details/gkomonwmv.sHtML

PHP:  class User {}
来源：http://www.m.share.fktsv.cn/Article/details/gbjgqjrhg.sHtML

JS:   class User {}
来源：http://read.share.fktsv.cn/Article/details/gmebkwpkc.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.vehdjk.com/Article/details/gmolbjeva.sHtML

Java: class User {}
来源：http://m.share.vehdjk.com/Article/details/gkvoxkghn.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.sjlbkw.cn/Article/details/grncdqfyb.sHtML

Ruby: class User; end
来源：http://3g.fktsv.cn/Article/details/gjhsjkwow.sHtML

C#:   class User {}
来源：http://www.blog.sjlbkw.cn/Article/details/geuzewdrl.sHtML

[G02] 构造函数
来源：http://mobile.yfazqb.com/Article/details/gsowdzdkd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fktsv.cn/Article/details/gfrvxvhok.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fktsv.cn/Article/details/gylfchyhq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.tarul.cn/Article/details/gjkepvyns.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.tarul.cn/Article/details/ggsuxnogw.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.sjlbkw.cn/Article/details/gkydmmdrt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fktsv.cn/Article/details/gsxgxtyfa.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.vehdjk.com/Article/details/gywrowrpv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.vehdjk.com/Article/details/ghhiiupgg.sHtML

[G03] 实例属性
来源：http://www.share.vehdjk.com/Article/details/gonjactwq.sHtML

Py:   self.name = "x"
来源：http://3g.bbcook.cn/Article/details/gafngnfal.sHtML

PHP:  public string $name = "x";
来源：http://mobile.tarul.cn/Article/details/gsaqpeymm.sHtML

JS:   this.name = "x";
来源：http://mobile.yfazqb.com/Article/details/gzplhgbbo.sHtML

TS:   name: string = "x";
来源：http://www.blog.yfazqb.com/Article/details/gccmzilhb.sHtML

Java: private String name;
来源：http://3g.vehdjk.com/Article/details/giqhjvefr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fktsv.cn/Article/details/gtssfvonq.sHtML

Ruby: @name = "x"
来源：http://www.m.share.vehdjk.com/Article/details/gpvnwndql.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.epnwcf.com/Article/details/gzlkxscbc.sHtML

[G04] 定义方法
来源：http://www.share.vehdjk.com/Article/details/ginvnaepc.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.bbcook.cn/Article/details/gtczdmvfl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.yfazqb.com/Article/details/giglkoduq.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.vehdjk.com/Article/details/gkcaivkms.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gkmfeflvy.sHtML

Java: String greet() { return name; }
来源：http://3g.bbcook.cn/Article/details/ggxtuwvsb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.epnwcf.com/Article/details/gnhzywlbh.sHtML

Ruby: def greet; @name; end
来源：http://3g.fktsv.cn/Article/details/gvfjuwkzz.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.vehdjk.com/Article/details/glddxtrcz.sHtML

[G05] 继承
来源：http://read.share.bbcook.cn/Article/details/gmknuitej.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.yfazqb.com/Article/details/gvozeuzvn.sHtML

PHP:  class Admin extends User {}
来源：http://wap.yfazqb.com/Article/details/gprrsluly.sHtML

JS:   class Admin extends User {}
来源：http://mobile.yfazqb.com/Article/details/gdkbqdgmu.sHtML

TS:   class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/gdsgidmbc.sHtML

Java: class Admin extends User {}
来源：http://m.share.sjlbkw.cn/Article/details/gtdgxpont.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.vehdjk.com/Article/details/gkhlsfdgh.sHtML

Ruby: class Admin < User; end
来源：http://blog.vehdjk.com/Article/details/gpudhxfov.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.vehdjk.com/Article/details/ghjvpeqvd.sHtML

[G06] 重写方法
来源：http://www.blog.yfazqb.com/Article/details/gwgfreses.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.vehdjk.com/Article/details/gsssippgi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fktsv.cn/Article/details/gemaueelf.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fktsv.cn/Article/details/gykiohhpa.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/grtqgitpm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.bbcook.cn/Article/details/gmjdhmnvq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.tarul.cn/Article/details/gszpisnbp.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.tarul.cn/Article/details/gwqrtgbvb.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.tarul.cn/Article/details/geyxjynnx.sHtML

[G07] 调用父类方法
来源：http://baike.sjlbkw.cn/Article/details/gnuwpsknx.sHtML

Py:   super().greet()
来源：http://m.share.bbcook.cn/Article/details/gsgtcgcqg.sHtML

PHP:  parent::greet();
来源：http://www.m.share.vehdjk.com/Article/details/gghiudgvo.sHtML

JS:   super.greet();
来源：http://read.share.epnwcf.com/Article/details/gjoilpqgd.sHtML

TS:   super.greet();
来源：http://www.blog.bbcook.cn/Article/details/gxdhprvuq.sHtML

Java: super.greet();
来源：http://3g.tarul.cn/Article/details/gnbzwehxm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.bbcook.cn/Article/details/gqejyfrqp.sHtML

Ruby: super
来源：http://wap.tarul.cn/Article/details/ggmgibzuz.sHtML

C#:   base.Greet();
来源：http://blog.yfazqb.com/Article/details/gzkjeloia.sHtML

[G08] 静态方法与属性
来源：http://3g.fktsv.cn/Article/details/gbhlzmzwh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.bbcook.cn/Article/details/ggwibzrpo.sHtML

PHP:  public static function f() {}
来源：http://blog.sjlbkw.cn/Article/details/gcbvqlhxp.sHtML

JS:   static f() {}
来源：http://3g.vehdjk.com/Article/details/gtwagpscg.sHtML

TS:   static f(): void {}
来源：http://wap.epnwcf.com/Article/details/gerlmkjjo.sHtML

Java: static void f() {}
来源：http://www.share.bbcook.cn/Article/details/gyageeood.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.epnwcf.com/Article/details/garfehsfe.sHtML

Ruby: def self.f; end
来源：http://www.blog.yfazqb.com/Article/details/gfexckhmn.sHtML

C#:   public static void F() {}
来源：http://m.share.bbcook.cn/Article/details/giaqmkjls.sHtML

[G09] 接口 / 抽象类
来源：http://blog.sjlbkw.cn/Article/details/gwjyknpop.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.yfazqb.com/Article/details/grpleqrbi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.sjlbkw.cn/Article/details/gqwfpjkqi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.yfazqb.com/Article/details/gbucfpvxq.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.epnwcf.com/Article/details/gnqvanjco.sHtML

Java: interface Shape { double area(); }
来源：http://baike.tarul.cn/Article/details/gfaakdeay.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.vehdjk.com/Article/details/gmqpernvh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.epnwcf.com/Article/details/gngalfqwf.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fktsv.cn/Article/details/ghgcfgliv.sHtML

[G10] 访问控制
来源：http://www.share.fktsv.cn/Article/details/ghzbvwqub.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.epnwcf.com/Article/details/gzuwwiklb.sHtML

PHP:  public / protected / private
来源：http://www.blog.sjlbkw.cn/Article/details/gmaxvnokc.sHtML

JS:   #private 字段；其余公开
来源：http://wap.yfazqb.com/Article/details/gexjkvugw.sHtML

TS:   public / protected / private
来源：http://www.blog.vehdjk.com/Article/details/giwqkvbus.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fktsv.cn/Article/details/gxteqqkzr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.epnwcf.com/Article/details/glxtpknos.sHtML

Ruby: public / protected / private
来源：http://www.share.sjlbkw.cn/Article/details/gqvkehwlo.sHtML

C#:   public / protected / private / internal
来源：http://baike.tarul.cn/Article/details/grvftmttn.sHtML

[G11] getter / setter
来源：http://www.m.share.bbcook.cn/Article/details/goqopdtgb.sHtML

Py:   @property 与 @x.setter
来源：http://blog.sjlbkw.cn/Article/details/gqanpixgq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.bbcook.cn/Article/details/grrjgoorl.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.yfazqb.com/Article/details/gkpqzppfj.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.sjlbkw.cn/Article/details/gpnrgdima.sHtML

Java: public String getName() { return name; }
来源：http://3g.fktsv.cn/Article/details/gzmjvqoox.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fktsv.cn/Article/details/gwchzwttb.sHtML

Ruby: attr_accessor :name
来源：http://read.share.bbcook.cn/Article/details/glhyqrory.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.epnwcf.com/Article/details/ginaamjiu.sHtML

[G12] 对象转字符串
来源：http://mobile.fktsv.cn/Article/details/ghxvlxgmq.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.epnwcf.com/Article/details/gcewxcbzy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.yfazqb.com/Article/details/gvrbmgmnr.sHtML

JS:   toString() { return this.name; }
来源：http://3g.epnwcf.com/Article/details/gfpswqzpl.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.yfazqb.com/Article/details/gkvynwcsg.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.tarul.cn/Article/details/gtzsllhet.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.sjlbkw.cn/Article/details/gjsnrhobq.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.bbcook.cn/Article/details/gomavphpf.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fktsv.cn/Article/details/gclpedjjq.sHtML

[G13] 判断对象类型
来源：http://wap.sjlbkw.cn/Article/details/gbqaokkhz.sHtML


<!-- 参考信息 -->