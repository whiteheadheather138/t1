代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.epnwcf.com/Article/details/gevicwaml.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fktsv.cn/Article/details/gijhotgpj.sHtML

[E16] 数字千分位
来源：http://mobile.yfazqb.com/Article/details/gpmfoworx.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fktsv.cn/Article/details/gaiakcrfw.sHtML

PHP:  number_format(1234567);
来源：http://mobile.sjlbkw.cn/Article/details/gbqcdohwh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.tarul.cn/Article/details/gncfpqxwf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.bbcook.cn/Article/details/gaaukiixl.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.yfazqb.com/Article/details/gmzbwlahu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.epnwcf.com/Article/details/gmzoevodf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.tarul.cn/Article/details/gzetavamc.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.sjlbkw.cn/Article/details/ggfeaanlw.sHtML

[E17] 首字母大写
来源：http://m.share.yfazqb.com/Article/details/gpofkcnxd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.tarul.cn/Article/details/gsahlfikm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.yfazqb.com/Article/details/ggvtimwpe.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.yfazqb.com/Article/details/grgdeojbp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.yfazqb.com/Article/details/gctnkacdo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fktsv.cn/Article/details/gdzypnwmx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fktsv.cn/Article/details/gbvzqbdir.sHtML

Ruby: s.capitalize
来源：http://read.share.epnwcf.com/Article/details/gdgoqopzn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.sjlbkw.cn/Article/details/gvqyjtncb.sHtML

[E18] 模板占位符替换
来源：http://m.share.bbcook.cn/Article/details/govchiomk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.yfazqb.com/Article/details/gefczmdrf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.epnwcf.com/Article/details/goxxcmfqe.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fktsv.cn/Article/details/gjivecstt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.epnwcf.com/Article/details/gnmxchsox.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.tarul.cn/Article/details/gqkyfphgg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.yfazqb.com/Article/details/gwjvlplqr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.bbcook.cn/Article/details/gbclgiuvn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.yfazqb.com/Article/details/gtpqsylfh.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fktsv.cn/Article/details/gbgevwdcn.sHtML

Py:   s.splitlines()
来源：http://blog.epnwcf.com/Article/details/geqicjczw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gnadzfstv.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.vehdjk.com/Article/details/gatnvqajd.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.sjlbkw.cn/Article/details/gesucewwm.sHtML

Java: s.lines().toList()
来源：http://www.blog.vehdjk.com/Article/details/gfvaifcfm.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.tarul.cn/Article/details/gylagsqwn.sHtML

Ruby: s.lines
来源：http://m.share.epnwcf.com/Article/details/gaxeyltgp.sHtML

C#:   s.Split('\n')
来源：http://blog.epnwcf.com/Article/details/gkosyuhfh.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.epnwcf.com/Article/details/ggomllqyo.sHtML

Py:   if not s:
来源：http://baike.epnwcf.com/Article/details/gguziebrb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.bbcook.cn/Article/details/gcyvgjgdt.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.bbcook.cn/Article/details/gqwsixbpj.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fktsv.cn/Article/details/ghwgoccmk.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.epnwcf.com/Article/details/ghlzefecf.sHtML

Go:   if s == "" {}
来源：http://m.share.sjlbkw.cn/Article/details/geojmwmvu.sHtML

Ruby: if s.empty?
来源：http://mobile.bbcook.cn/Article/details/guukvgpoy.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.yfazqb.com/Article/details/gttsotszn.sHtML

[E21] 超长截断加省略号
来源：http://m.share.yfazqb.com/Article/details/giutibtsa.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.yfazqb.com/Article/details/gwnkolxys.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fktsv.cn/Article/details/gmlbjuuxt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.sjlbkw.cn/Article/details/gdihoveye.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.bbcook.cn/Article/details/gsmylazkc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.yfazqb.com/Article/details/gttjrnesc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.sjlbkw.cn/Article/details/gkmxjcwzj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.epnwcf.com/Article/details/gkyjdpdhc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.tarul.cn/Article/details/gpniafeye.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.epnwcf.com/Article/details/gfxbsbkwp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.yfazqb.com/Article/details/gobzidcuz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.vehdjk.com/Article/details/gymayccmo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.epnwcf.com/Article/details/glhgofyfy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.tarul.cn/Article/details/gwvgdlplw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.yfazqb.com/Article/details/gjlvyaqwh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fktsv.cn/Article/details/gxecihuqr.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.vehdjk.com/Article/details/gzwmkcmhn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.sjlbkw.cn/Article/details/glrnxmsdt.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gdcgpbglf.sHtML

F. 文件与目录
来源：http://wap.sjlbkw.cn/Article/details/gajgajomd.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/griwbsxbj.sHtML

[F01] 读取整个文件
来源：http://3g.tarul.cn/Article/details/gnwinklbh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.tarul.cn/Article/details/gjhqkgbut.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fktsv.cn/Article/details/gvjmzeztw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.yfazqb.com/Article/details/gimorovcz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.vehdjk.com/Article/details/gecxfiwvt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.vehdjk.com/Article/details/grpdtktyz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.epnwcf.com/Article/details/gudbkrkyi.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gfgquzeap.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.tarul.cn/Article/details/gznucwlyp.sHtML

[F02] 逐行读取文件
来源：http://baike.bbcook.cn/Article/details/gvybqsiid.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.epnwcf.com/Article/details/gxxsrkuja.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.bbcook.cn/Article/details/gnohrfeqk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.vehdjk.com/Article/details/gewydoorg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.yfazqb.com/Article/details/galinocnt.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.bbcook.cn/Article/details/gkegjqnbq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.yfazqb.com/Article/details/gjemkktsg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.vehdjk.com/Article/details/gshjzkupx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.bbcook.cn/Article/details/gnofbrqvr.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.epnwcf.com/Article/details/ggzndgjem.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.vehdjk.com/Article/details/gylrbwseg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.yfazqb.com/Article/details/gbbcgdvro.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.sjlbkw.cn/Article/details/gndytiwlz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.epnwcf.com/Article/details/gyhktkisk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.sjlbkw.cn/Article/details/gheduiddf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.yfazqb.com/Article/details/gwjkjdatn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.sjlbkw.cn/Article/details/giywdqjtr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.vehdjk.com/Article/details/gxzalquoz.sHtML

[F04] 追加写入文件
来源：http://baike.fktsv.cn/Article/details/gnrvdgobd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.epnwcf.com/Article/details/guijvyotl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.tarul.cn/Article/details/gwsqmzhar.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.bbcook.cn/Article/details/glktwedwi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fktsv.cn/Article/details/gumcbpban.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.bbcook.cn/Article/details/gbbwmhpmi.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.epnwcf.com/Article/details/gpeifnpyb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.yfazqb.com/Article/details/ghtwhwdvi.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fktsv.cn/Article/details/glcbibfrd.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fktsv.cn/Article/details/gfaizowhx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.sjlbkw.cn/Article/details/gpzsdasfo.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/grjmyvhdd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gwlgamqsj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.bbcook.cn/Article/details/gyrgytpij.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.sjlbkw.cn/Article/details/gihdxqary.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.tarul.cn/Article/details/gcqgtnwbu.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gazdotbcg.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gmxeemrih.sHtML

[F06] 删除文件
来源：http://read.share.fktsv.cn/Article/details/gzyyaqnyt.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gvrekkvhu.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.vehdjk.com/Article/details/grmfmnajg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gvumydklo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gqwanvfhm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.yfazqb.com/Article/details/gjvupfssl.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gnxmqbhxe.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gsdelpbks.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.bbcook.cn/Article/details/gxtqxrjfq.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.yfazqb.com/Article/details/ggcbxutzu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.sjlbkw.cn/Article/details/gocxzclop.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.fktsv.cn/Article/details/gcyzhehnu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.epnwcf.com/Article/details/gletjoojw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.yfazqb.com/Article/details/gvnohdwxq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.vehdjk.com/Article/details/gjlidfukp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.yfazqb.com/Article/details/glukimcpz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.bbcook.cn/Article/details/gneegwljx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.yfazqb.com/Article/details/gplkazvpt.sHtML

[F08] 遍历目录
来源：http://www.m.share.tarul.cn/Article/details/gtkdmmnea.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.sjlbkw.cn/Article/details/gquledcyv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.sjlbkw.cn/Article/details/gcrgpqqpc.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fktsv.cn/Article/details/gxszzjhta.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.vehdjk.com/Article/details/guctlrcwr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.bbcook.cn/Article/details/gozvhonfs.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.epnwcf.com/Article/details/grokyrbat.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fktsv.cn/Article/details/gnpnzvkdz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.sjlbkw.cn/Article/details/giwpwfwwj.sHtML

[F09] 获取文件大小
来源：http://www.share.yfazqb.com/Article/details/gcpdvmued.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/grfhcneah.sHtML

PHP:  filesize("a.txt");
来源：http://blog.tarul.cn/Article/details/gazfnzcxc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.sjlbkw.cn/Article/details/gecoantry.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.tarul.cn/Article/details/gojsjmqvf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.bbcook.cn/Article/details/giqqkuxch.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.sjlbkw.cn/Article/details/gepjapzdu.sHtML

Ruby: File.size("a.txt")
来源：http://wap.bbcook.cn/Article/details/gcvqpjueg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.yfazqb.com/Article/details/gntwoxyzw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.epnwcf.com/Article/details/gsceuwliv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/grnutnsih.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gwdgwddrl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/ghtucqndb.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gfsagijrs.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.epnwcf.com/Article/details/gjucoxxbc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gzhggdhyb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gqioongwt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fktsv.cn/Article/details/grqnwccyx.sHtML

[F11] 复制与移动文件
来源：http://baike.yfazqb.com/Article/details/gbyxxypws.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.epnwcf.com/Article/details/gzshzjsoa.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.vehdjk.com/Article/details/gvharxnpf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.sjlbkw.cn/Article/details/greylpwxz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.yfazqb.com/Article/details/gafodcgnn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.yfazqb.com/Article/details/gghycrrqz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fktsv.cn/Article/details/gvurzappe.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.sjlbkw.cn/Article/details/growcgefb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.sjlbkw.cn/Article/details/grehbjlqu.sHtML

[F12] CSV 读写
来源：http://3g.sjlbkw.cn/Article/details/gezvauoyj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.yfazqb.com/Article/details/gbkglszcx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.bbcook.cn/Article/details/gurdvzaxa.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.sjlbkw.cn/Article/details/gnqjkqgom.sHtML

TS:   // 同上
来源：http://m.share.vehdjk.com/Article/details/gitjfxmya.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fktsv.cn/Article/details/gmhonxhtl.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.bbcook.cn/Article/details/gtuztgvob.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.vehdjk.com/Article/details/gkolbrggj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.epnwcf.com/Article/details/gglhcnnog.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gqyaxfjwv.sHtML

G. 面向对象
来源：http://m.share.yfazqb.com/Article/details/gmmaksbvb.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gwqtdkump.sHtML

[G01] 定义类
来源：http://www.m.share.fktsv.cn/Article/details/gcpymsbkd.sHtML

Py:   class User: pass
来源：http://blog.tarul.cn/Article/details/gzcumkvjq.sHtML

PHP:  class User {}
来源：http://www.m.share.yfazqb.com/Article/details/ghimpiaox.sHtML

JS:   class User {}
来源：http://blog.sjlbkw.cn/Article/details/gdujrxmev.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.sjlbkw.cn/Article/details/gofrdhhps.sHtML

Java: class User {}
来源：http://baike.fktsv.cn/Article/details/gopekkqkj.sHtML

Go:   type User struct { Name string }
来源：http://mobile.epnwcf.com/Article/details/gcitiukov.sHtML

Ruby: class User; end
来源：http://www.share.bbcook.cn/Article/details/gwyzazhgh.sHtML

C#:   class User {}
来源：http://wap.bbcook.cn/Article/details/gurlmhczm.sHtML

[G02] 构造函数
来源：http://read.share.bbcook.cn/Article/details/gwnobmgvh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.epnwcf.com/Article/details/gdvayqlpg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.bbcook.cn/Article/details/ggxdpjbrc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fktsv.cn/Article/details/gmeuofhmv.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.epnwcf.com/Article/details/gtjlvtybq.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.tarul.cn/Article/details/gvkthemus.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.vehdjk.com/Article/details/gpmijxcax.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fktsv.cn/Article/details/givbqxqvu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.vehdjk.com/Article/details/gqmsdvwkw.sHtML

[G03] 实例属性
来源：http://wap.sjlbkw.cn/Article/details/govwfjobx.sHtML

Py:   self.name = "x"
来源：http://baike.vehdjk.com/Article/details/ggyzvsajk.sHtML

PHP:  public string $name = "x";
来源：http://baike.tarul.cn/Article/details/grxyszlqw.sHtML

JS:   this.name = "x";
来源：http://wap.bbcook.cn/Article/details/gkqfrunmq.sHtML

TS:   name: string = "x";
来源：http://www.m.share.tarul.cn/Article/details/gwrnnmcwp.sHtML

Java: private String name;
来源：http://baike.sjlbkw.cn/Article/details/gkzntrvih.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.tarul.cn/Article/details/garwtdmtl.sHtML

Ruby: @name = "x"
来源：http://www.blog.tarul.cn/Article/details/guelsdepl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.bbcook.cn/Article/details/ghtovdlql.sHtML

[G04] 定义方法
来源：http://blog.yfazqb.com/Article/details/gdnotqdfs.sHtML

Py:   def greet(self): return self.name
来源：http://3g.yfazqb.com/Article/details/gbyysiagw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.tarul.cn/Article/details/ghhktuexe.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gardycepg.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.yfazqb.com/Article/details/gyvscnzku.sHtML

Java: String greet() { return name; }
来源：http://wap.sjlbkw.cn/Article/details/gyaabowef.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.bbcook.cn/Article/details/gorbjwvkz.sHtML

Ruby: def greet; @name; end
来源：http://m.share.sjlbkw.cn/Article/details/gvxusukwg.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.epnwcf.com/Article/details/glzmepunn.sHtML

[G05] 继承
来源：http://baike.epnwcf.com/Article/details/gonmmspgv.sHtML

Py:   class Admin(User): pass
来源：http://m.share.sjlbkw.cn/Article/details/gzkgfzwsn.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fktsv.cn/Article/details/ggvslundc.sHtML

JS:   class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gnodvseix.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fktsv.cn/Article/details/goeylukvt.sHtML

Java: class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/glvtqljgg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.yfazqb.com/Article/details/grjsvcwjh.sHtML

Ruby: class Admin < User; end
来源：http://baike.bbcook.cn/Article/details/ggetgwhsf.sHtML

C#:   class Admin : User {}
来源：http://baike.epnwcf.com/Article/details/gbgxlqwpp.sHtML

[G06] 重写方法
来源：http://www.m.share.fktsv.cn/Article/details/gzohbwdhl.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.vehdjk.com/Article/details/gcdisnfdo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/gstshudmf.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.vehdjk.com/Article/details/gteiadbkg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.bbcook.cn/Article/details/ghcfzhnrh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fktsv.cn/Article/details/gwywvvzcx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.sjlbkw.cn/Article/details/gvxfdliaw.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.sjlbkw.cn/Article/details/gyvfreblw.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fktsv.cn/Article/details/gvybsjgpd.sHtML

[G07] 调用父类方法
来源：http://mobile.tarul.cn/Article/details/gxxlonftg.sHtML

Py:   super().greet()
来源：http://mobile.epnwcf.com/Article/details/ggojroyqm.sHtML

PHP:  parent::greet();
来源：http://3g.yfazqb.com/Article/details/gvsenvnlj.sHtML

JS:   super.greet();
来源：http://3g.sjlbkw.cn/Article/details/gabhyjmsx.sHtML

TS:   super.greet();
来源：http://m.share.fktsv.cn/Article/details/gehqydhry.sHtML

Java: super.greet();
来源：http://www.blog.sjlbkw.cn/Article/details/gjjfwcxdd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fktsv.cn/Article/details/gybhtleor.sHtML

Ruby: super
来源：http://www.share.tarul.cn/Article/details/gfnwxtbqe.sHtML

C#:   base.Greet();
来源：http://www.blog.bbcook.cn/Article/details/grfbsbigk.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.bbcook.cn/Article/details/gsnhlpafu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.bbcook.cn/Article/details/gzdigwthl.sHtML

PHP:  public static function f() {}
来源：http://www.share.bbcook.cn/Article/details/gflaaoekd.sHtML

JS:   static f() {}
来源：http://3g.epnwcf.com/Article/details/ggbjhclcs.sHtML

TS:   static f(): void {}
来源：http://3g.tarul.cn/Article/details/glhcujddi.sHtML

Java: static void f() {}
来源：http://www.blog.bbcook.cn/Article/details/gbwlnulhs.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.sjlbkw.cn/Article/details/giufnptti.sHtML

Ruby: def self.f; end
来源：http://read.share.bbcook.cn/Article/details/gahejyass.sHtML

C#:   public static void F() {}
来源：http://baike.epnwcf.com/Article/details/ggabcwwmo.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.sjlbkw.cn/Article/details/gxwoedbxx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fktsv.cn/Article/details/glaaswlea.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.yfazqb.com/Article/details/grrxoedzk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.epnwcf.com/Article/details/gmisoicpv.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.tarul.cn/Article/details/gbsvjocwg.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.tarul.cn/Article/details/gorywclot.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fktsv.cn/Article/details/gezumproa.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.tarul.cn/Article/details/gmnroceei.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gsjycbsdl.sHtML

[G10] 访问控制
来源：http://3g.fktsv.cn/Article/details/gxfjyopsz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fktsv.cn/Article/details/gcktesxfx.sHtML

PHP:  public / protected / private
来源：http://wap.sjlbkw.cn/Article/details/gnqutsczg.sHtML

JS:   #private 字段；其余公开
来源：http://blog.tarul.cn/Article/details/giyghfwdr.sHtML

TS:   public / protected / private
来源：http://www.blog.fktsv.cn/Article/details/gpokjapxv.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.sjlbkw.cn/Article/details/gqeqnfirs.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fktsv.cn/Article/details/gcrjwlytp.sHtML

Ruby: public / protected / private
来源：http://blog.epnwcf.com/Article/details/gmclbzykp.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.tarul.cn/Article/details/guircnukd.sHtML

[G11] getter / setter
来源：http://baike.yfazqb.com/Article/details/grkvqiinj.sHtML

Py:   @property 与 @x.setter
来源：http://wap.epnwcf.com/Article/details/gcbpocoyl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.bbcook.cn/Article/details/gmoxwqruj.sHtML

JS:   get name() { return this._name; }
来源：http://3g.sjlbkw.cn/Article/details/ghyhxdhqw.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.yfazqb.com/Article/details/gszrkfukk.sHtML

Java: public String getName() { return name; }
来源：http://read.share.tarul.cn/Article/details/gqewwrtal.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fktsv.cn/Article/details/gweaprniz.sHtML

Ruby: attr_accessor :name
来源：http://3g.vehdjk.com/Article/details/gyjffnrdw.sHtML

C#:   public string Name { get; set; }
来源：http://baike.bbcook.cn/Article/details/gxwcznkwq.sHtML

[G12] 对象转字符串
来源：http://mobile.tarul.cn/Article/details/gwgloavpj.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fktsv.cn/Article/details/gflmytvan.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.epnwcf.com/Article/details/gkvnaoozk.sHtML

JS:   toString() { return this.name; }
来源：http://blog.epnwcf.com/Article/details/gyaaezfiq.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/giubmvuid.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.bbcook.cn/Article/details/ggnndjbte.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.yfazqb.com/Article/details/gnetsobru.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.bbcook.cn/Article/details/gkatrcdvu.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.bbcook.cn/Article/details/gsizbcykg.sHtML

[G13] 判断对象类型
来源：http://read.share.epnwcf.com/Article/details/gaalbxzxh.sHtML

Py:   isinstance(u, User)
来源：http://3g.sjlbkw.cn/Article/details/glvwmvnvb.sHtML

PHP:  $u instanceof User
来源：http://wap.tarul.cn/Article/details/gchezfvqn.sHtML

JS:   u instanceof User
来源：http://m.share.yfazqb.com/Article/details/gdiycpyit.sHtML

TS:   u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/glioakjof.sHtML

Java: u instanceof User
来源：http://www.blog.fktsv.cn/Article/details/gekciaddh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.tarul.cn/Article/details/guqueakcm.sHtML

Ruby: u.is_a?(User)
来源：http://3g.yfazqb.com/Article/details/gcznvtnyg.sHtML

C#:   u is User
来源：http://wap.sjlbkw.cn/Article/details/gplndrhco.sHtML

[G14] 数据类 / record
来源：http://m.share.bbcook.cn/Article/details/gxtsmurlv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.vehdjk.com/Article/details/gesefqifi.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.bbcook.cn/Article/details/gwflwlzrw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.yfazqb.com/Article/details/gjvqjlqgi.sHtML


<!-- 参考信息 -->