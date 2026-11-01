代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.vehdjk.com/Article/details/gcbgbqulx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.tarul.cn/Article/details/gaepjdmqc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fktsv.cn/Article/details/gbdotgpub.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.bbcook.cn/Article/details/gvjjoecyb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.yfazqb.com/Article/details/gnyzjjwyl.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fktsv.cn/Article/details/gzvrjhpda.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fktsv.cn/Article/details/gsbuhcfhr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.sjlbkw.cn/Article/details/gpspxyxhd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.bbcook.cn/Article/details/gjobqjfbs.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fktsv.cn/Article/details/gnwzrjepk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.bbcook.cn/Article/details/gayeqkcmy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.vehdjk.com/Article/details/gytknlfqm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.tarul.cn/Article/details/gdikkuwau.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.tarul.cn/Article/details/ghyrixynz.sHtML

[E16] 数字千分位
来源：http://baike.bbcook.cn/Article/details/gzbyxcmqr.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.bbcook.cn/Article/details/grmknrywp.sHtML

PHP:  number_format(1234567);
来源：http://wap.sjlbkw.cn/Article/details/geucsxmxk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.yfazqb.com/Article/details/gzbzpcphr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.yfazqb.com/Article/details/grstacorn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.tarul.cn/Article/details/geedkqhqs.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fktsv.cn/Article/details/gaxofokym.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.vehdjk.com/Article/details/gktxbxxvs.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fktsv.cn/Article/details/gupurnhuh.sHtML

[E17] 首字母大写
来源：http://www.share.sjlbkw.cn/Article/details/glxyoqzdt.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.tarul.cn/Article/details/gxntxpnvw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.epnwcf.com/Article/details/gviqfwops.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.vehdjk.com/Article/details/gmcuupjzr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.tarul.cn/Article/details/giqhuxcfj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fktsv.cn/Article/details/gfgabrhsd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.vehdjk.com/Article/details/gimizfvsb.sHtML

Ruby: s.capitalize
来源：http://read.share.vehdjk.com/Article/details/gtmhtzkas.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.epnwcf.com/Article/details/gertihgoe.sHtML

[E18] 模板占位符替换
来源：http://mobile.tarul.cn/Article/details/gtfsjujpc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.vehdjk.com/Article/details/gwzifssed.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.yfazqb.com/Article/details/gdmmrjgjk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.epnwcf.com/Article/details/gvdlrtyva.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.vehdjk.com/Article/details/gmlbmnqqm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fktsv.cn/Article/details/gyomzjvja.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.tarul.cn/Article/details/gyjuxkpjk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fktsv.cn/Article/details/ggcjjcaqs.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.epnwcf.com/Article/details/gdnchqzcl.sHtML

[E19] 多行文本按行拆分
来源：http://wap.bbcook.cn/Article/details/gtmlcezwq.sHtML

Py:   s.splitlines()
来源：http://m.share.fktsv.cn/Article/details/gxexvvpji.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.yfazqb.com/Article/details/gcwynhiyf.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.sjlbkw.cn/Article/details/gfxyqdxjd.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.yfazqb.com/Article/details/gyiaqahrl.sHtML

Java: s.lines().toList()
来源：http://mobile.vehdjk.com/Article/details/gxntrpgex.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.yfazqb.com/Article/details/gwyddrtkp.sHtML

Ruby: s.lines
来源：http://www.blog.epnwcf.com/Article/details/gakzqyuca.sHtML

C#:   s.Split('\n')
来源：http://mobile.sjlbkw.cn/Article/details/gtgqdjqgs.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.epnwcf.com/Article/details/gljbgthwm.sHtML

Py:   if not s:
来源：http://baike.vehdjk.com/Article/details/gjkpbyuex.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.sjlbkw.cn/Article/details/gylfyrbhm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.vehdjk.com/Article/details/gsbgvlyep.sHtML

TS:   if (s === "") {}
来源：http://mobile.vehdjk.com/Article/details/gyfekdkhq.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.epnwcf.com/Article/details/gjgshgjjv.sHtML

Go:   if s == "" {}
来源：http://wap.tarul.cn/Article/details/giamidsxp.sHtML

Ruby: if s.empty?
来源：http://wap.bbcook.cn/Article/details/gzijmlyao.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.bbcook.cn/Article/details/gdykgbfzh.sHtML

[E21] 超长截断加省略号
来源：http://read.share.epnwcf.com/Article/details/gexwuzlmo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.bbcook.cn/Article/details/gvpllzmxd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.bbcook.cn/Article/details/gbjkoaeux.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.vehdjk.com/Article/details/gcxvzcpqc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.vehdjk.com/Article/details/goefbrewf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.vehdjk.com/Article/details/ghitlzwlc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fktsv.cn/Article/details/ghnjlwcwi.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.vehdjk.com/Article/details/gzusceljf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.epnwcf.com/Article/details/gnbdxbmvq.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.epnwcf.com/Article/details/ghdrdieql.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.sjlbkw.cn/Article/details/gvxgmyeun.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.tarul.cn/Article/details/gdvljhhzv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fktsv.cn/Article/details/gnspccuox.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.tarul.cn/Article/details/gyywlmnlr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.tarul.cn/Article/details/gtolhgosa.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.epnwcf.com/Article/details/gfmhciuyi.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fktsv.cn/Article/details/goznoxxqy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fktsv.cn/Article/details/gudkorlvd.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gabbeifso.sHtML

F. 文件与目录
来源：http://mobile.bbcook.cn/Article/details/gvdhxhpla.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gsknbnrde.sHtML

[F01] 读取整个文件
来源：http://3g.sjlbkw.cn/Article/details/gwoehjsqt.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.tarul.cn/Article/details/girevpukr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gywukxrec.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.tarul.cn/Article/details/gbrpexnmt.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.yfazqb.com/Article/details/gshokoxlt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/grxevaojy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.sjlbkw.cn/Article/details/gqgtswlfl.sHtML

Ruby: File.read("a.txt")
来源：http://blog.tarul.cn/Article/details/gorzqdghn.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gnzdwhwly.sHtML

[F02] 逐行读取文件
来源：http://read.share.tarul.cn/Article/details/geiysenso.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.tarul.cn/Article/details/gtbdqeaws.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.yfazqb.com/Article/details/godqssowi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fktsv.cn/Article/details/gyfkpuxow.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.sjlbkw.cn/Article/details/ggmfixlaz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fktsv.cn/Article/details/guxmsnbif.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.sjlbkw.cn/Article/details/gczfozonp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.sjlbkw.cn/Article/details/gxpiilmla.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.epnwcf.com/Article/details/gbltqdjxt.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.yfazqb.com/Article/details/ghbrtemay.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fktsv.cn/Article/details/ghxzizyla.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.vehdjk.com/Article/details/gzivxijth.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.yfazqb.com/Article/details/gsvrftgcu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.vehdjk.com/Article/details/gssvsuxbg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.bbcook.cn/Article/details/gltyryyaa.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.sjlbkw.cn/Article/details/gyhicozgg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.yfazqb.com/Article/details/gqsxsbtrs.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fktsv.cn/Article/details/giakeutdu.sHtML

[F04] 追加写入文件
来源：http://m.share.epnwcf.com/Article/details/gkhidkyvi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.sjlbkw.cn/Article/details/gzsvzlfps.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.epnwcf.com/Article/details/gtmxgnqsc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.epnwcf.com/Article/details/gwvrkbbff.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.sjlbkw.cn/Article/details/gblgtzliw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.sjlbkw.cn/Article/details/gjfftmpkp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.bbcook.cn/Article/details/giunnlcco.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.vehdjk.com/Article/details/gczkbcedx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.vehdjk.com/Article/details/gumblktqc.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.yfazqb.com/Article/details/gekihasah.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.yfazqb.com/Article/details/gubioprhi.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.tarul.cn/Article/details/gmdukjmdo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.bbcook.cn/Article/details/gczxffnnf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.bbcook.cn/Article/details/gxtofykbz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.tarul.cn/Article/details/gluzgmtli.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.epnwcf.com/Article/details/gwdjqiiou.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gsjnlfkrw.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gwmryqceg.sHtML

[F06] 删除文件
来源：http://wap.vehdjk.com/Article/details/gaxmquwff.sHtML

Py:   os.remove("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gsivnlrxy.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.tarul.cn/Article/details/grtdyeomj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gnoruhbsr.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.bbcook.cn/Article/details/gawabwhhm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.bbcook.cn/Article/details/gvxbvwdxs.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.vehdjk.com/Article/details/govrfmuud.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fktsv.cn/Article/details/gwgsglxbd.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.tarul.cn/Article/details/gbsaxteuz.sHtML

[F07] 创建目录（含多级）
来源：http://3g.bbcook.cn/Article/details/gpnbkcrkc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.sjlbkw.cn/Article/details/gnecllbxq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.epnwcf.com/Article/details/gskmegyxg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.yfazqb.com/Article/details/gehgoasyi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.vehdjk.com/Article/details/gqkfzmgoa.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.vehdjk.com/Article/details/gnailcvpg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.tarul.cn/Article/details/gysajkefu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.epnwcf.com/Article/details/gdpdzildz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.epnwcf.com/Article/details/ghafrujno.sHtML

[F08] 遍历目录
来源：http://m.share.tarul.cn/Article/details/gobdbawfn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.tarul.cn/Article/details/gffktoefe.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.sjlbkw.cn/Article/details/ggemkclrd.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.yfazqb.com/Article/details/gjzoeeuhg.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.yfazqb.com/Article/details/gjrtjdlxx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.sjlbkw.cn/Article/details/glswnerdo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.sjlbkw.cn/Article/details/gifwdabeb.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/gduotkgch.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fktsv.cn/Article/details/gmizyjqkm.sHtML

[F09] 获取文件大小
来源：http://www.m.share.bbcook.cn/Article/details/gvlnxvouy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gbawvffkv.sHtML

PHP:  filesize("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gthjnpgzi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.yfazqb.com/Article/details/gwnpmjemt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.vehdjk.com/Article/details/gdznxqapr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.yfazqb.com/Article/details/gplmimbag.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.bbcook.cn/Article/details/gbmodsnmx.sHtML

Ruby: File.size("a.txt")
来源：http://3g.vehdjk.com/Article/details/gruhftzts.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.vehdjk.com/Article/details/gxmliblkd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.yfazqb.com/Article/details/gufdmxbrm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/gobqzztru.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.tarul.cn/Article/details/gwjtikmks.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.bbcook.cn/Article/details/ghzmgctgs.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.tarul.cn/Article/details/glvlddwgb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.tarul.cn/Article/details/gmjiigjtw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gwpoufadm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.bbcook.cn/Article/details/gwvwtdsvm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/ghlbthtus.sHtML

[F11] 复制与移动文件
来源：http://wap.vehdjk.com/Article/details/grpciyldw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/ggkerqijs.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.yfazqb.com/Article/details/gbgrpszmr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fktsv.cn/Article/details/gjnvusodn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.sjlbkw.cn/Article/details/guenzfwwo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.bbcook.cn/Article/details/gfaktuvpu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.yfazqb.com/Article/details/ggiwyqnts.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gfrsjzwff.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.yfazqb.com/Article/details/gusviylhy.sHtML

[F12] CSV 读写
来源：http://www.share.fktsv.cn/Article/details/gvpaimaee.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.epnwcf.com/Article/details/gduzazhbz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fktsv.cn/Article/details/gedphjmme.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fktsv.cn/Article/details/gxdocyvxg.sHtML

TS:   // 同上
来源：http://www.share.vehdjk.com/Article/details/gqmeyagbn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.tarul.cn/Article/details/gntntjmbo.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.sjlbkw.cn/Article/details/gfgugguys.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.tarul.cn/Article/details/ghkshlmjj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.yfazqb.com/Article/details/glntyzsqt.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gibqkhxyw.sHtML

G. 面向对象
来源：http://wap.fktsv.cn/Article/details/grsdmalrb.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/guocgnlmc.sHtML

[G01] 定义类
来源：http://blog.bbcook.cn/Article/details/gjcjtmcsy.sHtML

Py:   class User: pass
来源：http://www.blog.fktsv.cn/Article/details/geuuwathp.sHtML

PHP:  class User {}
来源：http://m.share.sjlbkw.cn/Article/details/goepbgtnt.sHtML

JS:   class User {}
来源：http://blog.vehdjk.com/Article/details/gjrgmuadi.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.sjlbkw.cn/Article/details/gcawsagxf.sHtML

Java: class User {}
来源：http://3g.sjlbkw.cn/Article/details/gdojvxdvr.sHtML

Go:   type User struct { Name string }
来源：http://blog.bbcook.cn/Article/details/gisxpmnyn.sHtML

Ruby: class User; end
来源：http://www.m.share.epnwcf.com/Article/details/gfkekpyln.sHtML

C#:   class User {}
来源：http://blog.yfazqb.com/Article/details/gyxtqczpf.sHtML

[G02] 构造函数
来源：http://www.m.share.bbcook.cn/Article/details/gzblzbomc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.sjlbkw.cn/Article/details/ggdyfmftr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.epnwcf.com/Article/details/gkthzckfy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.bbcook.cn/Article/details/gcizdxzqg.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.epnwcf.com/Article/details/gbkleljyd.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.yfazqb.com/Article/details/gaggzawus.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.sjlbkw.cn/Article/details/gopmlqnif.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.yfazqb.com/Article/details/gxcmzfrul.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.epnwcf.com/Article/details/gghmtqlpa.sHtML

[G03] 实例属性
来源：http://www.blog.tarul.cn/Article/details/gotebixcj.sHtML

Py:   self.name = "x"
来源：http://baike.tarul.cn/Article/details/gncgavjfr.sHtML

PHP:  public string $name = "x";
来源：http://3g.vehdjk.com/Article/details/godemveag.sHtML

JS:   this.name = "x";
来源：http://m.share.yfazqb.com/Article/details/gahjbmpix.sHtML

TS:   name: string = "x";
来源：http://m.share.vehdjk.com/Article/details/gpcvspooc.sHtML

Java: private String name;
来源：http://blog.vehdjk.com/Article/details/gvjscjffa.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.yfazqb.com/Article/details/gqmxdooop.sHtML

Ruby: @name = "x"
来源：http://www.share.epnwcf.com/Article/details/gqeiwtjib.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fktsv.cn/Article/details/gcypbminc.sHtML

[G04] 定义方法
来源：http://mobile.fktsv.cn/Article/details/gfxnwhtaj.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.epnwcf.com/Article/details/gcyxlgipx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fktsv.cn/Article/details/gnochiuns.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/gmqcfgspe.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.sjlbkw.cn/Article/details/gpoqejkcd.sHtML

Java: String greet() { return name; }
来源：http://3g.epnwcf.com/Article/details/gwgywxjpx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.tarul.cn/Article/details/gxzrisavc.sHtML

Ruby: def greet; @name; end
来源：http://3g.bbcook.cn/Article/details/gophcbalh.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.sjlbkw.cn/Article/details/gyqoshlbj.sHtML

[G05] 继承
来源：http://www.blog.bbcook.cn/Article/details/gydkaqxuu.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.yfazqb.com/Article/details/gburgrjbn.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.vehdjk.com/Article/details/gucuoxdcv.sHtML

JS:   class Admin extends User {}
来源：http://www.share.yfazqb.com/Article/details/gzwkoufsf.sHtML

TS:   class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/giffoumpc.sHtML

Java: class Admin extends User {}
来源：http://www.blog.epnwcf.com/Article/details/gwtnifvsl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.bbcook.cn/Article/details/gdwxkfwki.sHtML

Ruby: class Admin < User; end
来源：http://mobile.vehdjk.com/Article/details/grjfletxg.sHtML

C#:   class Admin : User {}
来源：http://baike.yfazqb.com/Article/details/gyvrcrbax.sHtML

[G06] 重写方法
来源：http://www.blog.tarul.cn/Article/details/gsumltlfo.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.vehdjk.com/Article/details/gfscralhe.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fktsv.cn/Article/details/gubgejsol.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.bbcook.cn/Article/details/gbbirtmcv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.yfazqb.com/Article/details/gqszlcxtw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.tarul.cn/Article/details/gznykqeyu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.tarul.cn/Article/details/goufcxiwg.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.sjlbkw.cn/Article/details/gwjkszapf.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.yfazqb.com/Article/details/gigfcqazl.sHtML

[G07] 调用父类方法
来源：http://wap.fktsv.cn/Article/details/ggnursqrh.sHtML

Py:   super().greet()
来源：http://read.share.epnwcf.com/Article/details/gqqhwrzwx.sHtML

PHP:  parent::greet();
来源：http://baike.sjlbkw.cn/Article/details/gljxhrybp.sHtML

JS:   super.greet();
来源：http://www.share.vehdjk.com/Article/details/gdimpjpkh.sHtML

TS:   super.greet();
来源：http://www.blog.sjlbkw.cn/Article/details/gvpaowsnn.sHtML

Java: super.greet();
来源：http://mobile.vehdjk.com/Article/details/gqshcfsbi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.vehdjk.com/Article/details/gvzjbhymt.sHtML

Ruby: super
来源：http://www.blog.fktsv.cn/Article/details/glafkmcyl.sHtML

C#:   base.Greet();
来源：http://wap.yfazqb.com/Article/details/gfyrwbpin.sHtML

[G08] 静态方法与属性
来源：http://baike.tarul.cn/Article/details/gaoyqkqns.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.epnwcf.com/Article/details/gijbyztig.sHtML

PHP:  public static function f() {}
来源：http://read.share.yfazqb.com/Article/details/gmlhkhcqa.sHtML

JS:   static f() {}
来源：http://3g.sjlbkw.cn/Article/details/gwhokthbw.sHtML

TS:   static f(): void {}
来源：http://mobile.vehdjk.com/Article/details/guhmcxczr.sHtML

Java: static void f() {}
来源：http://blog.tarul.cn/Article/details/gnejxdqyt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.vehdjk.com/Article/details/ghghkpkqz.sHtML

Ruby: def self.f; end
来源：http://read.share.fktsv.cn/Article/details/guxbjvlxr.sHtML

C#:   public static void F() {}
来源：http://mobile.epnwcf.com/Article/details/gnvqlwayv.sHtML

[G09] 接口 / 抽象类
来源：http://3g.vehdjk.com/Article/details/grpmlxtdi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.bbcook.cn/Article/details/ghfpyozkl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.bbcook.cn/Article/details/ggvhiwjdd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.epnwcf.com/Article/details/gyfqsjrgh.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.yfazqb.com/Article/details/gtgqaqptm.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gyhbqblnk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.bbcook.cn/Article/details/gkxcdhawk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.bbcook.cn/Article/details/gshgbpaes.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.tarul.cn/Article/details/gpvzsquxu.sHtML

[G10] 访问控制
来源：http://mobile.fktsv.cn/Article/details/gtkbtqudd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.bbcook.cn/Article/details/gfwrwohnr.sHtML

PHP:  public / protected / private
来源：http://www.share.sjlbkw.cn/Article/details/gcsrfnprg.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.yfazqb.com/Article/details/gbgwgjpiv.sHtML

TS:   public / protected / private
来源：http://www.m.share.yfazqb.com/Article/details/gajayicwz.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fktsv.cn/Article/details/gvruzxgld.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fktsv.cn/Article/details/ghmqeatym.sHtML

Ruby: public / protected / private
来源：http://3g.tarul.cn/Article/details/gxjhinrvg.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.bbcook.cn/Article/details/gpiluiwql.sHtML

[G11] getter / setter
来源：http://www.share.yfazqb.com/Article/details/gdqusvymh.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.sjlbkw.cn/Article/details/gubxzttsx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fktsv.cn/Article/details/ggqocqbdu.sHtML

JS:   get name() { return this._name; }
来源：http://blog.bbcook.cn/Article/details/giibsvyqg.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.epnwcf.com/Article/details/gagghnezv.sHtML

Java: public String getName() { return name; }
来源：http://baike.bbcook.cn/Article/details/gbdqwnjyx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.bbcook.cn/Article/details/gydmctwwc.sHtML

Ruby: attr_accessor :name
来源：http://mobile.sjlbkw.cn/Article/details/gjzdscnzo.sHtML

C#:   public string Name { get; set; }
来源：http://3g.epnwcf.com/Article/details/gojgeqahv.sHtML

[G12] 对象转字符串
来源：http://baike.vehdjk.com/Article/details/gkhkxside.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.tarul.cn/Article/details/gjovmwtkh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.vehdjk.com/Article/details/gpsuyxfjv.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fktsv.cn/Article/details/gfvwexpnk.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.epnwcf.com/Article/details/gfnbqybhv.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.tarul.cn/Article/details/gmkaqknad.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.sjlbkw.cn/Article/details/gywnvwagd.sHtML

Ruby: def to_s; @name; end
来源：http://wap.bbcook.cn/Article/details/giwejnxdb.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fktsv.cn/Article/details/gzuvdqesb.sHtML

[G13] 判断对象类型
来源：http://mobile.sjlbkw.cn/Article/details/gtdtspfph.sHtML


<!-- 参考信息 -->