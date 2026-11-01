代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.vehdjk.com/Article/details/gvipwdxax.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.sjlbkw.cn/Article/details/gbhqqbbcp.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.sjlbkw.cn/Article/details/gmvnargps.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fktsv.cn/Article/details/gsaakdjca.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.bbcook.cn/Article/details/gsmmjwcap.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.tarul.cn/Article/details/giqrxptcd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.epnwcf.com/Article/details/gfgyeoysu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.bbcook.cn/Article/details/grdpwgrvd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.yfazqb.com/Article/details/giuvdqrdk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.bbcook.cn/Article/details/gwtcqabsz.sHtML

[E16] 数字千分位
来源：http://www.blog.bbcook.cn/Article/details/geborbdnb.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.vehdjk.com/Article/details/goponsvrg.sHtML

PHP:  number_format(1234567);
来源：http://mobile.sjlbkw.cn/Article/details/ggxxgmzbr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.vehdjk.com/Article/details/gquhhadap.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.tarul.cn/Article/details/gpeugrwtr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.vehdjk.com/Article/details/gnvcphpoa.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.sjlbkw.cn/Article/details/gcmocjajb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.bbcook.cn/Article/details/gvxthbbpb.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.epnwcf.com/Article/details/gatucclqr.sHtML

[E17] 首字母大写
来源：http://www.share.sjlbkw.cn/Article/details/gpivoakgg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.vehdjk.com/Article/details/gsjggvmsz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fktsv.cn/Article/details/gxwfetfjx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.tarul.cn/Article/details/ghlxhtbnw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.epnwcf.com/Article/details/gmejscvam.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.vehdjk.com/Article/details/gbpjalbfq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.epnwcf.com/Article/details/gbhuonaqe.sHtML

Ruby: s.capitalize
来源：http://www.blog.fktsv.cn/Article/details/garjixgww.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.tarul.cn/Article/details/gdpcpwdur.sHtML

[E18] 模板占位符替换
来源：http://blog.sjlbkw.cn/Article/details/gtajuljtn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.vehdjk.com/Article/details/gyjqpmlqz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.sjlbkw.cn/Article/details/gpvxqjlwc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.bbcook.cn/Article/details/gqhcmwchp.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fktsv.cn/Article/details/gtcnhawjb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.bbcook.cn/Article/details/gwlilumni.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.yfazqb.com/Article/details/gyrymismm.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.sjlbkw.cn/Article/details/gxjpbvsnq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fktsv.cn/Article/details/gkpqukyoz.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fktsv.cn/Article/details/ghzcofpbf.sHtML

Py:   s.splitlines()
来源：http://read.share.fktsv.cn/Article/details/gzqiiumsh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.sjlbkw.cn/Article/details/gsostgjgk.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.sjlbkw.cn/Article/details/gzdxfyuhn.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.tarul.cn/Article/details/gzznbvtrk.sHtML

Java: s.lines().toList()
来源：http://read.share.bbcook.cn/Article/details/gnqamzqbm.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.vehdjk.com/Article/details/gyxacqdaf.sHtML

Ruby: s.lines
来源：http://3g.vehdjk.com/Article/details/gdhoeehqm.sHtML

C#:   s.Split('\n')
来源：http://baike.bbcook.cn/Article/details/gvlzdqolh.sHtML

[E20] 判断字符串是否为空
来源：http://baike.epnwcf.com/Article/details/gqdgidzow.sHtML

Py:   if not s:
来源：http://m.share.tarul.cn/Article/details/gktzqqcqm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.yfazqb.com/Article/details/gutfdadkd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fktsv.cn/Article/details/gchyarevk.sHtML

TS:   if (s === "") {}
来源：http://blog.bbcook.cn/Article/details/gzikcrdfc.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.vehdjk.com/Article/details/gbxjeosaj.sHtML

Go:   if s == "" {}
来源：http://www.blog.vehdjk.com/Article/details/gdccmkpal.sHtML

Ruby: if s.empty?
来源：http://www.blog.fktsv.cn/Article/details/gtfnmvady.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.bbcook.cn/Article/details/gloggbvty.sHtML

[E21] 超长截断加省略号
来源：http://blog.fktsv.cn/Article/details/gejcsfrmg.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.sjlbkw.cn/Article/details/gjxxzimtu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.bbcook.cn/Article/details/gcsmtemkb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fktsv.cn/Article/details/gjxbpmckk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.sjlbkw.cn/Article/details/ggarjfkfl.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fktsv.cn/Article/details/gxbamdzdj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.yfazqb.com/Article/details/gnmntflzb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/gnxgeenpw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.epnwcf.com/Article/details/gzfiawumt.sHtML

[E22] 字节长度与字符长度
来源：http://baike.fktsv.cn/Article/details/gxrcwiunv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.vehdjk.com/Article/details/garxqkopy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.tarul.cn/Article/details/goedzwnfh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.sjlbkw.cn/Article/details/gyklawaol.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fktsv.cn/Article/details/gibgxviaw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.epnwcf.com/Article/details/gnwghvdwy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.sjlbkw.cn/Article/details/gfrcgsjug.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.tarul.cn/Article/details/gxvcxnuxq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.yfazqb.com/Article/details/gouepunkk.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gbyfhelsh.sHtML

F. 文件与目录
来源：http://baike.bbcook.cn/Article/details/gbfmcmvwc.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gtzsjlrua.sHtML

[F01] 读取整个文件
来源：http://read.share.epnwcf.com/Article/details/gcbcbsavf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.yfazqb.com/Article/details/groufnzuo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gokocahug.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.yfazqb.com/Article/details/gdscopvwd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.yfazqb.com/Article/details/gxeqccrec.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.vehdjk.com/Article/details/gdvvjsjma.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fktsv.cn/Article/details/gyxgtwrmu.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/govbecjmy.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/glxnjbsly.sHtML

[F02] 逐行读取文件
来源：http://3g.yfazqb.com/Article/details/glkamfnuy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.tarul.cn/Article/details/gbfiyfcen.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.tarul.cn/Article/details/gutqkyuyo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.sjlbkw.cn/Article/details/giytlolic.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.sjlbkw.cn/Article/details/gbthkgyoe.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.fktsv.cn/Article/details/gekwniksv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.yfazqb.com/Article/details/gevgqweqb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.epnwcf.com/Article/details/ggtcpvggd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.yfazqb.com/Article/details/gzvkssozx.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.vehdjk.com/Article/details/gazsxyegn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.bbcook.cn/Article/details/ganpfdhbf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.sjlbkw.cn/Article/details/gkytdrvlg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.tarul.cn/Article/details/gfdopavrr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.bbcook.cn/Article/details/ggyetcfef.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.sjlbkw.cn/Article/details/gfdfkdsmk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fktsv.cn/Article/details/gwokreudm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.tarul.cn/Article/details/gsuzelomj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fktsv.cn/Article/details/gexmwzwzu.sHtML

[F04] 追加写入文件
来源：http://www.blog.epnwcf.com/Article/details/gyvcmbmxs.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.bbcook.cn/Article/details/gmdzcuuur.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fktsv.cn/Article/details/gzsaiqrpm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.bbcook.cn/Article/details/gmljpqurb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.vehdjk.com/Article/details/gcxbxanbn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.sjlbkw.cn/Article/details/glzzcibmg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.epnwcf.com/Article/details/gcwhlweww.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.tarul.cn/Article/details/gqlszlygj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.vehdjk.com/Article/details/gjpjfikvl.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.yfazqb.com/Article/details/gqisjyhmb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fktsv.cn/Article/details/glaagwipd.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.bbcook.cn/Article/details/gpfgassiz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.tarul.cn/Article/details/goauzgtow.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gcqzzpmbe.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.bbcook.cn/Article/details/gunsmabxz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.epnwcf.com/Article/details/gzymlgmfy.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gxndgrzhq.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.tarul.cn/Article/details/gqrcfoxuh.sHtML

[F06] 删除文件
来源：http://www.share.tarul.cn/Article/details/gjmadlrsq.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gkaccfhit.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gwvtccwuw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.yfazqb.com/Article/details/gmjimfoqr.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gkxqlbbmg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.sjlbkw.cn/Article/details/ghnsukosw.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.tarul.cn/Article/details/gymaogozd.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gojnnywcf.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.epnwcf.com/Article/details/gqfhjchgf.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.epnwcf.com/Article/details/gmrfgppzn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.epnwcf.com/Article/details/gbbktjurc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.tarul.cn/Article/details/ggqrwuefr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.yfazqb.com/Article/details/gajxmcbvp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.tarul.cn/Article/details/gvsswkuie.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.yfazqb.com/Article/details/gqnqnsjnr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.yfazqb.com/Article/details/gtpzpvgdv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.bbcook.cn/Article/details/geofiyqns.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fktsv.cn/Article/details/gpadawimh.sHtML

[F08] 遍历目录
来源：http://blog.fktsv.cn/Article/details/gdepxepal.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.epnwcf.com/Article/details/gtkanmrmu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.epnwcf.com/Article/details/glbfcdxel.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.tarul.cn/Article/details/gxtvonrvu.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.yfazqb.com/Article/details/gefkomzpv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.tarul.cn/Article/details/gfuprrapr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.epnwcf.com/Article/details/gcnluyldu.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.tarul.cn/Article/details/gwdgdgume.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.vehdjk.com/Article/details/gulzzgrgw.sHtML

[F09] 获取文件大小
来源：http://www.blog.tarul.cn/Article/details/gxvupiiez.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gsulskomy.sHtML

PHP:  filesize("a.txt");
来源：http://wap.bbcook.cn/Article/details/guhwrkiqx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.bbcook.cn/Article/details/gjastryhe.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.bbcook.cn/Article/details/gayqbuzpl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.sjlbkw.cn/Article/details/gptoriwpj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fktsv.cn/Article/details/gtcuwlhtk.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gnlmlqxtc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.bbcook.cn/Article/details/gjgcapnbv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fktsv.cn/Article/details/gnsywrwjt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.bbcook.cn/Article/details/gzzjemfzq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gospbdpuv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gnogtqteu.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gqqnyrsxh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.bbcook.cn/Article/details/gdqgjnhtb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.vehdjk.com/Article/details/goairdadq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.epnwcf.com/Article/details/gmmbggjot.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/gumtaahlj.sHtML

[F11] 复制与移动文件
来源：http://read.share.vehdjk.com/Article/details/glqvzzkpv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/giuzmsbon.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.bbcook.cn/Article/details/ghwgfnwax.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.yfazqb.com/Article/details/gtcjuomek.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gjxwsrgid.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.tarul.cn/Article/details/gunjzbrvf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.yfazqb.com/Article/details/gkwbdvant.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.vehdjk.com/Article/details/gevmzssiv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.bbcook.cn/Article/details/gnlcemsgu.sHtML

[F12] CSV 读写
来源：http://m.share.vehdjk.com/Article/details/gxxtibmfw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fktsv.cn/Article/details/gsbqiuusd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.sjlbkw.cn/Article/details/grxfljwau.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.epnwcf.com/Article/details/goeksjovf.sHtML

TS:   // 同上
来源：http://blog.sjlbkw.cn/Article/details/glkgsuywa.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fktsv.cn/Article/details/gvoyqdlmu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.epnwcf.com/Article/details/gjkuygaqx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.bbcook.cn/Article/details/glpdrommi.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.bbcook.cn/Article/details/gapjfpkgz.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gstbadafn.sHtML

G. 面向对象
来源：http://www.m.share.epnwcf.com/Article/details/gnxqdywsh.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gcoczzyaq.sHtML

[G01] 定义类
来源：http://blog.sjlbkw.cn/Article/details/gvhjxpord.sHtML

Py:   class User: pass
来源：http://blog.fktsv.cn/Article/details/gcmqlxmjv.sHtML

PHP:  class User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gooakmiti.sHtML

JS:   class User {}
来源：http://baike.fktsv.cn/Article/details/genucxasc.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.vehdjk.com/Article/details/gsyznpxmw.sHtML

Java: class User {}
来源：http://www.blog.vehdjk.com/Article/details/glbyccbkk.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwhryvwsy.sHtML

Ruby: class User; end
来源：http://3g.fktsv.cn/Article/details/gixmapjwl.sHtML

C#:   class User {}
来源：http://www.m.share.tarul.cn/Article/details/gvdsuxkpl.sHtML

[G02] 构造函数
来源：http://mobile.bbcook.cn/Article/details/gswvynwsy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fktsv.cn/Article/details/guekmgahm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.vehdjk.com/Article/details/gabklkasz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.sjlbkw.cn/Article/details/gucaqoino.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.sjlbkw.cn/Article/details/giwbblmaw.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.tarul.cn/Article/details/gaqbshorm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.tarul.cn/Article/details/gbqssldrg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.yfazqb.com/Article/details/gojbhkvgt.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.epnwcf.com/Article/details/gpacdzgyf.sHtML

[G03] 实例属性
来源：http://www.share.bbcook.cn/Article/details/ghfdcpirr.sHtML

Py:   self.name = "x"
来源：http://3g.yfazqb.com/Article/details/guwvhtkyp.sHtML

PHP:  public string $name = "x";
来源：http://wap.bbcook.cn/Article/details/gvfzwzgmc.sHtML

JS:   this.name = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/gqxmhhddk.sHtML

TS:   name: string = "x";
来源：http://wap.fktsv.cn/Article/details/gqrwjedas.sHtML

Java: private String name;
来源：http://read.share.yfazqb.com/Article/details/gdfexyibq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fktsv.cn/Article/details/gqcbsedsr.sHtML

Ruby: @name = "x"
来源：http://blog.bbcook.cn/Article/details/gabwoovio.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.yfazqb.com/Article/details/getqvqhia.sHtML

[G04] 定义方法
来源：http://baike.fktsv.cn/Article/details/grxwdaxvm.sHtML

Py:   def greet(self): return self.name
来源：http://baike.epnwcf.com/Article/details/gibgjuzsq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.epnwcf.com/Article/details/gvmfnnuns.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fktsv.cn/Article/details/gnzxwfkja.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.tarul.cn/Article/details/gfkxefjdz.sHtML

Java: String greet() { return name; }
来源：http://blog.sjlbkw.cn/Article/details/gxcygbbhu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.tarul.cn/Article/details/greaicypx.sHtML

Ruby: def greet; @name; end
来源：http://3g.epnwcf.com/Article/details/gjxynmakh.sHtML

C#:   public string Greet() => Name;
来源：http://blog.epnwcf.com/Article/details/gwlillqlb.sHtML

[G05] 继承
来源：http://baike.sjlbkw.cn/Article/details/ghkkzbksz.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.bbcook.cn/Article/details/gfosxmdxm.sHtML

PHP:  class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/gnnncdnbu.sHtML

JS:   class Admin extends User {}
来源：http://mobile.tarul.cn/Article/details/gwjlqrgxj.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fktsv.cn/Article/details/ggsouiqvi.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.vehdjk.com/Article/details/gobyrqswd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.sjlbkw.cn/Article/details/gmwmzjqxw.sHtML

Ruby: class Admin < User; end
来源：http://wap.tarul.cn/Article/details/gxbyzysyh.sHtML

C#:   class Admin : User {}
来源：http://blog.sjlbkw.cn/Article/details/gcrtnrcna.sHtML

[G06] 重写方法
来源：http://wap.fktsv.cn/Article/details/gllkoiouu.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.yfazqb.com/Article/details/gguxtkofl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.epnwcf.com/Article/details/gtmrstkic.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fktsv.cn/Article/details/gjowegtjd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.tarul.cn/Article/details/gnwunumhp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.sjlbkw.cn/Article/details/gyevehnjv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.yfazqb.com/Article/details/gbvggrdri.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.epnwcf.com/Article/details/glstlgnqb.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.yfazqb.com/Article/details/gemkykres.sHtML

[G07] 调用父类方法
来源：http://read.share.vehdjk.com/Article/details/gxyjsczhw.sHtML

Py:   super().greet()
来源：http://www.m.share.yfazqb.com/Article/details/gakutumdu.sHtML

PHP:  parent::greet();
来源：http://mobile.vehdjk.com/Article/details/gedmprucb.sHtML

JS:   super.greet();
来源：http://www.m.share.bbcook.cn/Article/details/gqdvpmcrt.sHtML

TS:   super.greet();
来源：http://wap.yfazqb.com/Article/details/gedkzjxyx.sHtML

Java: super.greet();
来源：http://www.m.share.yfazqb.com/Article/details/gchahubvo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.yfazqb.com/Article/details/gmfvcsypq.sHtML

Ruby: super
来源：http://www.m.share.yfazqb.com/Article/details/grkcvfych.sHtML

C#:   base.Greet();
来源：http://www.share.yfazqb.com/Article/details/grxqkgcmu.sHtML

[G08] 静态方法与属性
来源：http://read.share.vehdjk.com/Article/details/glqyrbsug.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.epnwcf.com/Article/details/gcijxjkyf.sHtML

PHP:  public static function f() {}
来源：http://m.share.vehdjk.com/Article/details/gkzsggevd.sHtML

JS:   static f() {}
来源：http://mobile.fktsv.cn/Article/details/gemjnowbh.sHtML

TS:   static f(): void {}
来源：http://read.share.yfazqb.com/Article/details/golkxwpja.sHtML

Java: static void f() {}
来源：http://blog.tarul.cn/Article/details/gayeeougs.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.vehdjk.com/Article/details/gksswield.sHtML

Ruby: def self.f; end
来源：http://m.share.vehdjk.com/Article/details/ghnogcvbb.sHtML

C#:   public static void F() {}
来源：http://www.share.bbcook.cn/Article/details/gdsuxazyw.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.epnwcf.com/Article/details/gkgwsukhn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.bbcook.cn/Article/details/gfshrdebd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.vehdjk.com/Article/details/gzkdsetrp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.sjlbkw.cn/Article/details/gxkzzfmpg.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.yfazqb.com/Article/details/gsssdwmuv.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.yfazqb.com/Article/details/gyvbaqlhx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fktsv.cn/Article/details/gklzjtaxn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.bbcook.cn/Article/details/gymctszts.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.vehdjk.com/Article/details/gbvbqkmbn.sHtML

[G10] 访问控制
来源：http://www.blog.sjlbkw.cn/Article/details/gpaqialpk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fktsv.cn/Article/details/gafvqardp.sHtML

PHP:  public / protected / private
来源：http://www.blog.bbcook.cn/Article/details/gdwuilikn.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.sjlbkw.cn/Article/details/grfucidlf.sHtML

TS:   public / protected / private
来源：http://baike.tarul.cn/Article/details/gjpqqjfuf.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.tarul.cn/Article/details/geklvmuvy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.tarul.cn/Article/details/gxoljllwv.sHtML

Ruby: public / protected / private
来源：http://mobile.fktsv.cn/Article/details/gweujpfox.sHtML

C#:   public / protected / private / internal
来源：http://wap.yfazqb.com/Article/details/gxyswlaam.sHtML

[G11] getter / setter
来源：http://3g.tarul.cn/Article/details/gqrdovdum.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.sjlbkw.cn/Article/details/gvsazfngo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.bbcook.cn/Article/details/gznkvqdfj.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.tarul.cn/Article/details/ghmkowvot.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.tarul.cn/Article/details/ghghrwkqr.sHtML

Java: public String getName() { return name; }
来源：http://read.share.tarul.cn/Article/details/gvuymdrxb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.yfazqb.com/Article/details/gjxsaopkl.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.yfazqb.com/Article/details/gqmlhyhde.sHtML

C#:   public string Name { get; set; }
来源：http://baike.bbcook.cn/Article/details/gbjfrhpje.sHtML

[G12] 对象转字符串
来源：http://www.blog.bbcook.cn/Article/details/ggypcxyoq.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.bbcook.cn/Article/details/gkalnrtpg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.yfazqb.com/Article/details/ghoclrrwn.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.tarul.cn/Article/details/garqlklcu.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.tarul.cn/Article/details/ghrotekrb.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fktsv.cn/Article/details/grumedktq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.bbcook.cn/Article/details/gbgvoskjf.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.yfazqb.com/Article/details/gakbhnsfj.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.sjlbkw.cn/Article/details/gqgwxouau.sHtML

[G13] 判断对象类型
来源：http://3g.yfazqb.com/Article/details/gwfdlxipa.sHtML

Py:   isinstance(u, User)
来源：http://3g.tarul.cn/Article/details/gzceuvbov.sHtML

PHP:  $u instanceof User
来源：http://mobile.fktsv.cn/Article/details/gsdfsznat.sHtML

JS:   u instanceof User
来源：http://m.share.fktsv.cn/Article/details/grglrqgrd.sHtML

TS:   u instanceof User
来源：http://blog.tarul.cn/Article/details/gylqxjwof.sHtML


<!-- 参考信息 -->