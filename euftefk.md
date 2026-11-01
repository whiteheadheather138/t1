代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.yfazqb.com/Article/details/ghhxgeoqm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.sjlbkw.cn/Article/details/gxzeauaea.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.sjlbkw.cn/Article/details/gufmhbiui.sHtML

[E17] 首字母大写
来源：http://baike.yfazqb.com/Article/details/gxmnmuaan.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fktsv.cn/Article/details/gtvjlizrr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.sjlbkw.cn/Article/details/gslkzcach.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.vehdjk.com/Article/details/gromvinzt.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.epnwcf.com/Article/details/giadmnybp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.tarul.cn/Article/details/gqyzxdjkw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.tarul.cn/Article/details/gebnmljxh.sHtML

Ruby: s.capitalize
来源：http://m.share.bbcook.cn/Article/details/gqrepivze.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.epnwcf.com/Article/details/gwycsugjr.sHtML

[E18] 模板占位符替换
来源：http://wap.yfazqb.com/Article/details/grxinepda.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.sjlbkw.cn/Article/details/geghzxaip.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.vehdjk.com/Article/details/gmfjmfanj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.yfazqb.com/Article/details/gmffsmlyi.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.bbcook.cn/Article/details/giiceycpw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.bbcook.cn/Article/details/giesxazxb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.tarul.cn/Article/details/ghzzdjkfi.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.vehdjk.com/Article/details/glktmkhjx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.sjlbkw.cn/Article/details/gbcifdmyr.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fktsv.cn/Article/details/gpbnysgzv.sHtML

Py:   s.splitlines()
来源：http://m.share.sjlbkw.cn/Article/details/gokdfcsfe.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.sjlbkw.cn/Article/details/gqhlfztrn.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.epnwcf.com/Article/details/gyrjuvfrg.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.vehdjk.com/Article/details/gwtaqrvxn.sHtML

Java: s.lines().toList()
来源：http://mobile.fktsv.cn/Article/details/gfwqhmulx.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.bbcook.cn/Article/details/gbmffpiyi.sHtML

Ruby: s.lines
来源：http://m.share.epnwcf.com/Article/details/gqtmwpjej.sHtML

C#:   s.Split('\n')
来源：http://mobile.yfazqb.com/Article/details/gvohnuijb.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.yfazqb.com/Article/details/gnbzrttri.sHtML

Py:   if not s:
来源：http://wap.yfazqb.com/Article/details/gutwvwjxq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.tarul.cn/Article/details/gltslvzra.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.epnwcf.com/Article/details/gdlgywczs.sHtML

TS:   if (s === "") {}
来源：http://read.share.sjlbkw.cn/Article/details/gtqdinzhi.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.bbcook.cn/Article/details/gjymaprot.sHtML

Go:   if s == "" {}
来源：http://read.share.bbcook.cn/Article/details/ggkyjnqpp.sHtML

Ruby: if s.empty?
来源：http://baike.sjlbkw.cn/Article/details/gfmtmgcbp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.tarul.cn/Article/details/gyrcahsru.sHtML

[E21] 超长截断加省略号
来源：http://www.share.tarul.cn/Article/details/guwohwoei.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.tarul.cn/Article/details/gxpenalok.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.vehdjk.com/Article/details/gfnmwusmy.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.tarul.cn/Article/details/gnllhdjdo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.sjlbkw.cn/Article/details/gsyakunqe.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.epnwcf.com/Article/details/ghwjziwac.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.epnwcf.com/Article/details/gfkdgpfpv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.epnwcf.com/Article/details/gohidoyfw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.epnwcf.com/Article/details/gcfzxhxao.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.vehdjk.com/Article/details/gifqylfaw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.tarul.cn/Article/details/goqgcvgin.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.vehdjk.com/Article/details/gupfxgqds.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.tarul.cn/Article/details/gxtmegdpe.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.sjlbkw.cn/Article/details/gitdkpifz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.tarul.cn/Article/details/gtsraolgx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fktsv.cn/Article/details/ghzjwigsv.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.epnwcf.com/Article/details/gkfgkfhfo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.tarul.cn/Article/details/gzroiemhq.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gpugmxiac.sHtML

F. 文件与目录
来源：http://m.share.sjlbkw.cn/Article/details/gapgvuiay.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gvoerjecg.sHtML

[F01] 读取整个文件
来源：http://read.share.vehdjk.com/Article/details/glbpqzqwr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.tarul.cn/Article/details/gpgaxnuip.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gmqeqtxon.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.vehdjk.com/Article/details/golcjwezu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.tarul.cn/Article/details/gnjwvygti.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.yfazqb.com/Article/details/geuxjfrra.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.tarul.cn/Article/details/gfebpbhak.sHtML

Ruby: File.read("a.txt")
来源：http://wap.vehdjk.com/Article/details/gvadznzve.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gqwebyois.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fktsv.cn/Article/details/gvjysllwk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.vehdjk.com/Article/details/gcxufhoup.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.sjlbkw.cn/Article/details/gujzosobf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.vehdjk.com/Article/details/gwuvswqtx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.bbcook.cn/Article/details/gdpaqzluy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.yfazqb.com/Article/details/gwwzzpalg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.epnwcf.com/Article/details/godrbwtzm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.yfazqb.com/Article/details/gqadpvyzp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.vehdjk.com/Article/details/gsoidtaod.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.bbcook.cn/Article/details/gumewtmjj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fktsv.cn/Article/details/gtnnswjdx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.tarul.cn/Article/details/gpjfzkqkm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.sjlbkw.cn/Article/details/glibapmjx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.sjlbkw.cn/Article/details/gyhhilksz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.bbcook.cn/Article/details/glohofhlv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.vehdjk.com/Article/details/gxsuguzlt.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fktsv.cn/Article/details/gfdfososs.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.tarul.cn/Article/details/glhhzlewi.sHtML

[F04] 追加写入文件
来源：http://blog.epnwcf.com/Article/details/gyuqdvzgd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.epnwcf.com/Article/details/gvvafqbqk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fktsv.cn/Article/details/guwrkcvhh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.yfazqb.com/Article/details/giswjvoeb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.tarul.cn/Article/details/gsmjdyfmf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fktsv.cn/Article/details/guecdrwsd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.tarul.cn/Article/details/gqblwshfu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.tarul.cn/Article/details/gaonsderr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.sjlbkw.cn/Article/details/gvlfzvhfc.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.sjlbkw.cn/Article/details/gizsuzmsk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.yfazqb.com/Article/details/gyakqbupi.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/galnebjjm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghrkcmffv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gzguwevch.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.bbcook.cn/Article/details/gyrfehphd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.epnwcf.com/Article/details/gyupuisvt.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gngkdsbrc.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gsvcqjhvb.sHtML

[F06] 删除文件
来源：http://mobile.vehdjk.com/Article/details/ghsrtdbma.sHtML

Py:   os.remove("a.txt")
来源：http://3g.bbcook.cn/Article/details/gqmqkkjjv.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gfsurlfqt.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gfxjulyku.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.yfazqb.com/Article/details/gabtmsfmk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.sjlbkw.cn/Article/details/gwmbkjnlu.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.epnwcf.com/Article/details/gkajcnomr.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gcdtnbydz.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.yfazqb.com/Article/details/gsrikyeeh.sHtML

[F07] 创建目录（含多级）
来源：http://baike.bbcook.cn/Article/details/ghnrusoyc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.bbcook.cn/Article/details/glkjhoqbt.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.epnwcf.com/Article/details/gdnqxfusm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.epnwcf.com/Article/details/gzxxgivvm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.bbcook.cn/Article/details/gqxsgvmys.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.tarul.cn/Article/details/gkrekfran.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.bbcook.cn/Article/details/gyeuhdtzi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.vehdjk.com/Article/details/grovulsat.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fktsv.cn/Article/details/gzlnfdzxh.sHtML

[F08] 遍历目录
来源：http://mobile.yfazqb.com/Article/details/gitcgszqd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.vehdjk.com/Article/details/gucrckmsz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.vehdjk.com/Article/details/gntsnkfoe.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.tarul.cn/Article/details/gvpzdhejm.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.sjlbkw.cn/Article/details/gkiewgtzp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.yfazqb.com/Article/details/gkwibaqui.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.epnwcf.com/Article/details/griswpqpk.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fktsv.cn/Article/details/gseqkkkkx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.vehdjk.com/Article/details/gzdzenrmk.sHtML

[F09] 获取文件大小
来源：http://read.share.sjlbkw.cn/Article/details/ghvhfaqjt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gkinooqdw.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gbemmvext.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.vehdjk.com/Article/details/gytlzqskh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.bbcook.cn/Article/details/gwwatjhpp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fktsv.cn/Article/details/gilqqkwcd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.yfazqb.com/Article/details/gvcltdnxz.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fktsv.cn/Article/details/gjyscwyfi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.tarul.cn/Article/details/gkxbgyjpw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fktsv.cn/Article/details/giylnuafi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/guixoqzci.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gizcdtnsz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gzywbhebo.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fktsv.cn/Article/details/gqejbkfdz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.bbcook.cn/Article/details/ggfyuokkv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gospywrjl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gibveyzmi.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.bbcook.cn/Article/details/gimobslzc.sHtML

[F11] 复制与移动文件
来源：http://m.share.bbcook.cn/Article/details/gtblsbrpa.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/gatjtnlme.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.tarul.cn/Article/details/gojcprsni.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gweodpmeo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fktsv.cn/Article/details/gbrfjtksg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.sjlbkw.cn/Article/details/gltqalguv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.epnwcf.com/Article/details/gdhxkkcuk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.yfazqb.com/Article/details/gkoykenqx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.tarul.cn/Article/details/gjhiinrbo.sHtML

[F12] CSV 读写
来源：http://www.share.epnwcf.com/Article/details/gbgipswjo.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.yfazqb.com/Article/details/gktuqfllr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.bbcook.cn/Article/details/gjgfosycd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.tarul.cn/Article/details/gygubybpb.sHtML

TS:   // 同上
来源：http://m.share.fktsv.cn/Article/details/grorolfty.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fktsv.cn/Article/details/gbwbsvcjn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.fktsv.cn/Article/details/gigvbinys.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.vehdjk.com/Article/details/gvclalxbz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.tarul.cn/Article/details/gbxbqdyou.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/glnqtneqp.sHtML

G. 面向对象
来源：http://blog.bbcook.cn/Article/details/giiloovxc.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gwinrviyb.sHtML

[G01] 定义类
来源：http://www.m.share.fktsv.cn/Article/details/gbxpceryo.sHtML

Py:   class User: pass
来源：http://baike.bbcook.cn/Article/details/gqcplzqjs.sHtML

PHP:  class User {}
来源：http://wap.epnwcf.com/Article/details/gzxpugsfq.sHtML

JS:   class User {}
来源：http://www.blog.yfazqb.com/Article/details/gatzmhwbx.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.vehdjk.com/Article/details/gslgdxcdu.sHtML

Java: class User {}
来源：http://wap.sjlbkw.cn/Article/details/gfoqugjcl.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fktsv.cn/Article/details/ggvjvplqc.sHtML

Ruby: class User; end
来源：http://m.share.bbcook.cn/Article/details/gqsnxlbrb.sHtML

C#:   class User {}
来源：http://blog.fktsv.cn/Article/details/gddaztapj.sHtML

[G02] 构造函数
来源：http://read.share.sjlbkw.cn/Article/details/gbxtmonnu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.sjlbkw.cn/Article/details/gxrepewpz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.vehdjk.com/Article/details/guxdvhzrz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.epnwcf.com/Article/details/gckqzfhyt.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.vehdjk.com/Article/details/glqmzkede.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.bbcook.cn/Article/details/glxrfggbf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.epnwcf.com/Article/details/gbnyxuadh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.epnwcf.com/Article/details/gvtjtioul.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.vehdjk.com/Article/details/glwuleqni.sHtML

[G03] 实例属性
来源：http://www.share.bbcook.cn/Article/details/grbnwdlxq.sHtML

Py:   self.name = "x"
来源：http://www.share.tarul.cn/Article/details/gcwvufcrn.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fktsv.cn/Article/details/ghestrexk.sHtML

JS:   this.name = "x";
来源：http://wap.vehdjk.com/Article/details/gttbsmvpw.sHtML

TS:   name: string = "x";
来源：http://blog.bbcook.cn/Article/details/gdmfukief.sHtML

Java: private String name;
来源：http://blog.epnwcf.com/Article/details/gjuhvtgsl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fktsv.cn/Article/details/gomatxxkq.sHtML

Ruby: @name = "x"
来源：http://baike.fktsv.cn/Article/details/gmouzszrx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.vehdjk.com/Article/details/ghgmohwzp.sHtML

[G04] 定义方法
来源：http://www.blog.tarul.cn/Article/details/gvzckbvly.sHtML

Py:   def greet(self): return self.name
来源：http://3g.epnwcf.com/Article/details/gorrhuqrm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.vehdjk.com/Article/details/gtxqqlgnz.sHtML

JS:   greet() { return this.name; }
来源：http://wap.sjlbkw.cn/Article/details/gdeczvyup.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.bbcook.cn/Article/details/gdvpurrxc.sHtML

Java: String greet() { return name; }
来源：http://mobile.yfazqb.com/Article/details/gfwfxtdvc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.yfazqb.com/Article/details/gbtxhhorb.sHtML

Ruby: def greet; @name; end
来源：http://read.share.tarul.cn/Article/details/gyetqbfeu.sHtML

C#:   public string Greet() => Name;
来源：http://3g.tarul.cn/Article/details/gwibgsexh.sHtML

[G05] 继承
来源：http://3g.tarul.cn/Article/details/gukvfuxon.sHtML

Py:   class Admin(User): pass
来源：http://mobile.sjlbkw.cn/Article/details/gnsmdaunh.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fktsv.cn/Article/details/gqukjdekg.sHtML

JS:   class Admin extends User {}
来源：http://m.share.bbcook.cn/Article/details/genetzfsf.sHtML

TS:   class Admin extends User {}
来源：http://blog.yfazqb.com/Article/details/gsohsyqqj.sHtML

Java: class Admin extends User {}
来源：http://read.share.yfazqb.com/Article/details/gkcczdqyh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.sjlbkw.cn/Article/details/gdhasitoo.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.epnwcf.com/Article/details/guyaatsme.sHtML

C#:   class Admin : User {}
来源：http://www.share.yfazqb.com/Article/details/gnhrqghkx.sHtML

[G06] 重写方法
来源：http://www.blog.sjlbkw.cn/Article/details/gvcvumhmv.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.yfazqb.com/Article/details/gbegigrxf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.vehdjk.com/Article/details/guhzzvkkw.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fktsv.cn/Article/details/gsigyppsd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/gscbjhhzk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fktsv.cn/Article/details/goxunjpcw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.tarul.cn/Article/details/gmqcxmums.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fktsv.cn/Article/details/gdwmowubp.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fktsv.cn/Article/details/grgbeddos.sHtML

[G07] 调用父类方法
来源：http://3g.bbcook.cn/Article/details/ghrhmrxpi.sHtML

Py:   super().greet()
来源：http://m.share.yfazqb.com/Article/details/gsxwrzjwb.sHtML

PHP:  parent::greet();
来源：http://m.share.tarul.cn/Article/details/gngvfvabe.sHtML

JS:   super.greet();
来源：http://3g.yfazqb.com/Article/details/gxkiccash.sHtML

TS:   super.greet();
来源：http://mobile.fktsv.cn/Article/details/gpmdgwkih.sHtML

Java: super.greet();
来源：http://www.share.tarul.cn/Article/details/gthblnwts.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fktsv.cn/Article/details/gqwkldall.sHtML

Ruby: super
来源：http://mobile.vehdjk.com/Article/details/gbzdhdrzg.sHtML

C#:   base.Greet();
来源：http://www.share.bbcook.cn/Article/details/gqxfexcxq.sHtML

[G08] 静态方法与属性
来源：http://read.share.tarul.cn/Article/details/gehblfhnv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.epnwcf.com/Article/details/gwdirwwqe.sHtML

PHP:  public static function f() {}
来源：http://www.share.bbcook.cn/Article/details/gfwdikvox.sHtML

JS:   static f() {}
来源：http://blog.fktsv.cn/Article/details/gvxmhdgbe.sHtML

TS:   static f(): void {}
来源：http://wap.sjlbkw.cn/Article/details/gntleqjqf.sHtML

Java: static void f() {}
来源：http://blog.vehdjk.com/Article/details/gtwgqjapd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.tarul.cn/Article/details/gokimband.sHtML

Ruby: def self.f; end
来源：http://www.blog.sjlbkw.cn/Article/details/gpkrmqktp.sHtML

C#:   public static void F() {}
来源：http://read.share.vehdjk.com/Article/details/gqwjlauxi.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.bbcook.cn/Article/details/gwixtaurk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.vehdjk.com/Article/details/gbvplaofi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.epnwcf.com/Article/details/gmnpkalmr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.yfazqb.com/Article/details/gxdowifwh.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.tarul.cn/Article/details/glsewtanp.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fktsv.cn/Article/details/grppwknlp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.bbcook.cn/Article/details/gomxnonju.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.sjlbkw.cn/Article/details/gcktvokau.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.vehdjk.com/Article/details/gbnatxswa.sHtML

[G10] 访问控制
来源：http://3g.tarul.cn/Article/details/gsaejojig.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.vehdjk.com/Article/details/groqlhwge.sHtML

PHP:  public / protected / private
来源：http://www.blog.sjlbkw.cn/Article/details/gxyndsqom.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.bbcook.cn/Article/details/gwwendgle.sHtML

TS:   public / protected / private
来源：http://wap.vehdjk.com/Article/details/giqjptley.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.yfazqb.com/Article/details/gjyplhjqi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.sjlbkw.cn/Article/details/gkuhukpzk.sHtML

Ruby: public / protected / private
来源：http://www.m.share.epnwcf.com/Article/details/gynredoqs.sHtML

C#:   public / protected / private / internal
来源：http://read.share.sjlbkw.cn/Article/details/gsiiogvij.sHtML

[G11] getter / setter
来源：http://blog.yfazqb.com/Article/details/gjlnccnlv.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.bbcook.cn/Article/details/gfgazkwvb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.bbcook.cn/Article/details/gpbeunvab.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fktsv.cn/Article/details/gjgrxhubg.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gnikgbbue.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.vehdjk.com/Article/details/gwewxqjul.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.epnwcf.com/Article/details/guzlzbjbj.sHtML

Ruby: attr_accessor :name
来源：http://read.share.yfazqb.com/Article/details/gmnajgvki.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.epnwcf.com/Article/details/gmlbqwhqu.sHtML

[G12] 对象转字符串
来源：http://blog.yfazqb.com/Article/details/gsrkpbduh.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fktsv.cn/Article/details/gfizfyelg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.vehdjk.com/Article/details/gsbxcbylc.sHtML

JS:   toString() { return this.name; }
来源：http://baike.yfazqb.com/Article/details/gfiyxmecy.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.yfazqb.com/Article/details/gvuadepvc.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fktsv.cn/Article/details/gtlnoxlfu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.tarul.cn/Article/details/gaheyyikb.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fktsv.cn/Article/details/gtcteatdk.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.tarul.cn/Article/details/gljhmgszr.sHtML

[G13] 判断对象类型
来源：http://wap.fktsv.cn/Article/details/gdwbpusfy.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fktsv.cn/Article/details/gdueocinc.sHtML

PHP:  $u instanceof User
来源：http://baike.bbcook.cn/Article/details/ggqbygsgg.sHtML

JS:   u instanceof User
来源：http://m.share.sjlbkw.cn/Article/details/gzbidtmjr.sHtML

TS:   u instanceof User
来源：http://www.blog.fktsv.cn/Article/details/gcdsojwvr.sHtML

Java: u instanceof User
来源：http://blog.fktsv.cn/Article/details/gkvxtsebi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fktsv.cn/Article/details/gwtwqevxc.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.bbcook.cn/Article/details/gqhsgokza.sHtML

C#:   u is User
来源：http://wap.yfazqb.com/Article/details/gcfqytjaq.sHtML

[G14] 数据类 / record
来源：http://mobile.vehdjk.com/Article/details/gpnyauykx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.yfazqb.com/Article/details/gpsvspwil.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.tarul.cn/Article/details/gzjijriyj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.sjlbkw.cn/Article/details/gbegpbuix.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.bbcook.cn/Article/details/gguupjeqv.sHtML

Java: record User(String name, int age) {}
来源：http://3g.epnwcf.com/Article/details/gzlknbvkv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.tarul.cn/Article/details/guigtewqo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.vehdjk.com/Article/details/gjspjiqgh.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.epnwcf.com/Article/details/glccknxze.sHtML

[G15] 枚举
来源：http://www.share.bbcook.cn/Article/details/gsnihltly.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fktsv.cn/Article/details/gwxredddn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.sjlbkw.cn/Article/details/gzmnmbngv.sHtML


<!-- 参考信息 -->