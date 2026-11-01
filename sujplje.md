代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.tarul.cn/Article/details/gkdnlujnv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.vehdjk.com/Article/details/gjztlzzzw.sHtML

Ruby: s.capitalize
来源：http://www.share.vehdjk.com/Article/details/gliafwjsv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.tarul.cn/Article/details/ghdksyeyu.sHtML

[E18] 模板占位符替换
来源：http://3g.sjlbkw.cn/Article/details/gvkkfazam.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.epnwcf.com/Article/details/gshbvfkuu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.sjlbkw.cn/Article/details/gbiqacenr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fktsv.cn/Article/details/gcuyakzzf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.tarul.cn/Article/details/gkqjrihjg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fktsv.cn/Article/details/grfwjybsl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.sjlbkw.cn/Article/details/grxnnmoqp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.bbcook.cn/Article/details/goseniopv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.vehdjk.com/Article/details/gxlolgucu.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.epnwcf.com/Article/details/goxymuqcj.sHtML

Py:   s.splitlines()
来源：http://m.share.vehdjk.com/Article/details/gysayihgc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gmospypnw.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.tarul.cn/Article/details/geyhkzbcb.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.yfazqb.com/Article/details/gignzbtms.sHtML

Java: s.lines().toList()
来源：http://3g.epnwcf.com/Article/details/ggsspvqry.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.sjlbkw.cn/Article/details/gmuogjcft.sHtML

Ruby: s.lines
来源：http://m.share.vehdjk.com/Article/details/gcfnknhtu.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.tarul.cn/Article/details/gjitldrac.sHtML

[E20] 判断字符串是否为空
来源：http://3g.vehdjk.com/Article/details/gtephlwsw.sHtML

Py:   if not s:
来源：http://baike.sjlbkw.cn/Article/details/ggpdrqows.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fktsv.cn/Article/details/gthwuzmpi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.sjlbkw.cn/Article/details/gryoovwuo.sHtML

TS:   if (s === "") {}
来源：http://3g.sjlbkw.cn/Article/details/gpdqnfqog.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fktsv.cn/Article/details/gbrmmznwh.sHtML

Go:   if s == "" {}
来源：http://read.share.tarul.cn/Article/details/gmotpvzwp.sHtML

Ruby: if s.empty?
来源：http://3g.yfazqb.com/Article/details/grckovzve.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.vehdjk.com/Article/details/gnqbilibj.sHtML

[E21] 超长截断加省略号
来源：http://3g.sjlbkw.cn/Article/details/gttkzcxhh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.vehdjk.com/Article/details/gpcelbyhu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.vehdjk.com/Article/details/gyzghfaum.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.bbcook.cn/Article/details/gnccywxqn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fktsv.cn/Article/details/gsilglsfy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/gwunakgtc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.yfazqb.com/Article/details/gjkhqinlu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fktsv.cn/Article/details/grshcikuo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/gdmxqwyhl.sHtML

[E22] 字节长度与字符长度
来源：http://baike.yfazqb.com/Article/details/ggeunwuht.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fktsv.cn/Article/details/gjmebvput.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.tarul.cn/Article/details/grppnricb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.yfazqb.com/Article/details/guyvkrnym.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.bbcook.cn/Article/details/gcstkwkng.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.yfazqb.com/Article/details/guozpwtpu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.bbcook.cn/Article/details/gzystbgbm.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fktsv.cn/Article/details/gvbqokgls.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.bbcook.cn/Article/details/gxbuvzcue.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gczplpboj.sHtML

F. 文件与目录
来源：http://m.share.epnwcf.com/Article/details/gkovgoqpr.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gyduwswav.sHtML

[F01] 读取整个文件
来源：http://baike.vehdjk.com/Article/details/gudfcmmpy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.yfazqb.com/Article/details/gkndrodft.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.bbcook.cn/Article/details/gnhwugald.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.vehdjk.com/Article/details/gklpozrrt.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.bbcook.cn/Article/details/goylkgzsj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.bbcook.cn/Article/details/gowwfoczk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.yfazqb.com/Article/details/gnuldpphn.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fktsv.cn/Article/details/ggysxcosd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gzogyujdo.sHtML

[F02] 逐行读取文件
来源：http://3g.fktsv.cn/Article/details/gyachaftd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.tarul.cn/Article/details/goaoyzxbh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.epnwcf.com/Article/details/gyhtipdfm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.sjlbkw.cn/Article/details/gbczfdbog.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.yfazqb.com/Article/details/gckqtpnba.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.epnwcf.com/Article/details/gdjbafptd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.epnwcf.com/Article/details/gyxocxxun.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.yfazqb.com/Article/details/gfhwbrwar.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.yfazqb.com/Article/details/gostwufrq.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fktsv.cn/Article/details/gamwbxeqp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.yfazqb.com/Article/details/ggbgzttjh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.sjlbkw.cn/Article/details/goshobinh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.sjlbkw.cn/Article/details/gjlomwzcz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.vehdjk.com/Article/details/gdungvwqh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.vehdjk.com/Article/details/gfsvbqmbh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.tarul.cn/Article/details/gobpdghxj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.bbcook.cn/Article/details/guvrdcgoe.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fktsv.cn/Article/details/gxrlccfup.sHtML

[F04] 追加写入文件
来源：http://read.share.bbcook.cn/Article/details/gbiiwjuvc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.yfazqb.com/Article/details/ggxnrerpd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.sjlbkw.cn/Article/details/glrhnblvx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.sjlbkw.cn/Article/details/gzrowwvio.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.yfazqb.com/Article/details/gtwfpfnmt.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fktsv.cn/Article/details/gxpdufrbk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.bbcook.cn/Article/details/gcutfbxxw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.sjlbkw.cn/Article/details/gggbnzala.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fktsv.cn/Article/details/gfrejfkch.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.bbcook.cn/Article/details/glwobdukz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.sjlbkw.cn/Article/details/gvrysjyev.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fktsv.cn/Article/details/gwmtqnqfi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gbrgmgame.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/ggeozzvdo.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.bbcook.cn/Article/details/gjwtcppzi.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.sjlbkw.cn/Article/details/gagxdepxu.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.tarul.cn/Article/details/gmpnkkohe.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.epnwcf.com/Article/details/gttbkjwnk.sHtML

[F06] 删除文件
来源：http://wap.sjlbkw.cn/Article/details/gwndbkapp.sHtML

Py:   os.remove("a.txt")
来源：http://3g.tarul.cn/Article/details/gupzcisav.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.epnwcf.com/Article/details/glqswfpcp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.bbcook.cn/Article/details/greimapru.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/giitpftkx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fktsv.cn/Article/details/gumientig.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.tarul.cn/Article/details/genpiqedx.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gdexkjrcc.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/grzraiudt.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.epnwcf.com/Article/details/gnsbfkmrn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.bbcook.cn/Article/details/gbihcccrh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.vehdjk.com/Article/details/gumfohspy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.tarul.cn/Article/details/gvwpvlqxh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.epnwcf.com/Article/details/goqjxkdai.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.sjlbkw.cn/Article/details/gcxnhmeva.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.bbcook.cn/Article/details/gsmvdulzs.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.vehdjk.com/Article/details/gswgkjoya.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.vehdjk.com/Article/details/gkqeqlpgc.sHtML

[F08] 遍历目录
来源：http://www.share.sjlbkw.cn/Article/details/gwynlugpd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.bbcook.cn/Article/details/glqceqbsz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.vehdjk.com/Article/details/gszisdsbh.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fktsv.cn/Article/details/gwwoyngzq.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.yfazqb.com/Article/details/gueepabgz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.tarul.cn/Article/details/gxatauzrn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.bbcook.cn/Article/details/gcchlcdwc.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.tarul.cn/Article/details/gsalrsmqw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.yfazqb.com/Article/details/gbcwgqysa.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fktsv.cn/Article/details/gxyqsvipg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gsvakhirk.sHtML

PHP:  filesize("a.txt");
来源：http://baike.tarul.cn/Article/details/gijgojhdq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.vehdjk.com/Article/details/gxogypmmk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.vehdjk.com/Article/details/gnirrquwg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.tarul.cn/Article/details/gbrdqnlib.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.epnwcf.com/Article/details/gxjbbsnmr.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.tarul.cn/Article/details/gyepbphsx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.vehdjk.com/Article/details/getntujhq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.epnwcf.com/Article/details/gukaurlhi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gxhveadoa.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.vehdjk.com/Article/details/gjwwaswxo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.bbcook.cn/Article/details/grpzjqkkz.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gijqbqjou.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.yfazqb.com/Article/details/gzkkqkdqg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/glourwfjj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gydrwwibv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fktsv.cn/Article/details/gxiyydxyt.sHtML

[F11] 复制与移动文件
来源：http://blog.sjlbkw.cn/Article/details/ghetjczuc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.epnwcf.com/Article/details/gdmzvgweq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.bbcook.cn/Article/details/gxkmikfpt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/gxkqojuoy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.yfazqb.com/Article/details/gvnruyklr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.tarul.cn/Article/details/gziquavso.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.bbcook.cn/Article/details/gnxxpswzd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/ghqfavxah.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fktsv.cn/Article/details/gnkvxnffw.sHtML

[F12] CSV 读写
来源：http://3g.bbcook.cn/Article/details/gsxkwcqrd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.yfazqb.com/Article/details/gehtcbxxu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.epnwcf.com/Article/details/grfdyagkz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.bbcook.cn/Article/details/gtktjkaqc.sHtML

TS:   // 同上
来源：http://wap.vehdjk.com/Article/details/gxxfjkxkl.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fktsv.cn/Article/details/gatykoqnc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.vehdjk.com/Article/details/gwfxveool.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.yfazqb.com/Article/details/gpdoablfz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.yfazqb.com/Article/details/gnfesagex.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gxytoqrko.sHtML

G. 面向对象
来源：http://www.blog.sjlbkw.cn/Article/details/gvbajtycn.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gaqiinquj.sHtML

[G01] 定义类
来源：http://read.share.fktsv.cn/Article/details/gqkgfeskk.sHtML

Py:   class User: pass
来源：http://www.m.share.sjlbkw.cn/Article/details/gozqwkqpk.sHtML

PHP:  class User {}
来源：http://www.blog.fktsv.cn/Article/details/gkuexymeu.sHtML

JS:   class User {}
来源：http://baike.yfazqb.com/Article/details/gjzghjodl.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.vehdjk.com/Article/details/gmjgvirud.sHtML

Java: class User {}
来源：http://wap.fktsv.cn/Article/details/gjnoqtugo.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.epnwcf.com/Article/details/gcegdhamo.sHtML

Ruby: class User; end
来源：http://blog.bbcook.cn/Article/details/gbqmxgvfy.sHtML

C#:   class User {}
来源：http://m.share.epnwcf.com/Article/details/gyqalhmtg.sHtML

[G02] 构造函数
来源：http://mobile.epnwcf.com/Article/details/gmssngbke.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.epnwcf.com/Article/details/gdlauqpuf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fktsv.cn/Article/details/gfqtotdvp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.bbcook.cn/Article/details/gpedhdorv.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.vehdjk.com/Article/details/gmkwiwwnp.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzdyslonv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.yfazqb.com/Article/details/ggttuadxf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.epnwcf.com/Article/details/gmhmoxjsv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.tarul.cn/Article/details/gbjivgscj.sHtML

[G03] 实例属性
来源：http://3g.epnwcf.com/Article/details/gnnizcoek.sHtML

Py:   self.name = "x"
来源：http://www.blog.yfazqb.com/Article/details/gphszjice.sHtML

PHP:  public string $name = "x";
来源：http://m.share.tarul.cn/Article/details/gniukbfcq.sHtML

JS:   this.name = "x";
来源：http://www.m.share.epnwcf.com/Article/details/geaabrgdf.sHtML

TS:   name: string = "x";
来源：http://mobile.sjlbkw.cn/Article/details/ghjghasvg.sHtML

Java: private String name;
来源：http://baike.fktsv.cn/Article/details/ghfhlurur.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.yfazqb.com/Article/details/gjntbkfbd.sHtML

Ruby: @name = "x"
来源：http://www.blog.sjlbkw.cn/Article/details/gdcjlolni.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.bbcook.cn/Article/details/gjfpbxvzt.sHtML

[G04] 定义方法
来源：http://mobile.tarul.cn/Article/details/gtgjrqaiq.sHtML

Py:   def greet(self): return self.name
来源：http://3g.sjlbkw.cn/Article/details/gtsqrxnqw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fktsv.cn/Article/details/gljnhqsbb.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.sjlbkw.cn/Article/details/gmtyrqnwp.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.tarul.cn/Article/details/gbgvgepvo.sHtML

Java: String greet() { return name; }
来源：http://read.share.tarul.cn/Article/details/gqcweaonh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.tarul.cn/Article/details/gxicilglb.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.vehdjk.com/Article/details/gdysryldo.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.yfazqb.com/Article/details/gkmcrwwxp.sHtML

[G05] 继承
来源：http://mobile.bbcook.cn/Article/details/gjpeigthm.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fktsv.cn/Article/details/gbcmpeojf.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gmfngejbc.sHtML

JS:   class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/gqgogpsbd.sHtML

TS:   class Admin extends User {}
来源：http://blog.yfazqb.com/Article/details/glmtxzclp.sHtML

Java: class Admin extends User {}
来源：http://3g.epnwcf.com/Article/details/gkliesojw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.sjlbkw.cn/Article/details/gkbkrzlcb.sHtML

Ruby: class Admin < User; end
来源：http://baike.sjlbkw.cn/Article/details/gjaotnfxe.sHtML

C#:   class Admin : User {}
来源：http://mobile.epnwcf.com/Article/details/giswlrrdr.sHtML

[G06] 重写方法
来源：http://mobile.bbcook.cn/Article/details/gwmbxdxor.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.sjlbkw.cn/Article/details/gvgbppinj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fktsv.cn/Article/details/gscwfotcn.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.sjlbkw.cn/Article/details/gdsqwwbhw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.bbcook.cn/Article/details/gydixtius.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.vehdjk.com/Article/details/gqwxylwbq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.vehdjk.com/Article/details/gmvmwjxzs.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fktsv.cn/Article/details/ggezimctg.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.vehdjk.com/Article/details/gvveehvnb.sHtML

[G07] 调用父类方法
来源：http://www.share.tarul.cn/Article/details/gtgrdqdcn.sHtML

Py:   super().greet()
来源：http://baike.epnwcf.com/Article/details/gznckwlpv.sHtML

PHP:  parent::greet();
来源：http://3g.yfazqb.com/Article/details/gmmhjcdwj.sHtML

JS:   super.greet();
来源：http://www.m.share.epnwcf.com/Article/details/gjjstunsv.sHtML

TS:   super.greet();
来源：http://3g.yfazqb.com/Article/details/gwxqckxbg.sHtML

Java: super.greet();
来源：http://mobile.vehdjk.com/Article/details/gkweiikdj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.bbcook.cn/Article/details/gclttuiec.sHtML

Ruby: super
来源：http://www.blog.yfazqb.com/Article/details/gxxbhhcqy.sHtML

C#:   base.Greet();
来源：http://www.blog.sjlbkw.cn/Article/details/gxkucnzxx.sHtML

[G08] 静态方法与属性
来源：http://mobile.yfazqb.com/Article/details/gjyeelwdp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.vehdjk.com/Article/details/gtpayarxr.sHtML

PHP:  public static function f() {}
来源：http://m.share.tarul.cn/Article/details/gucvsmkfo.sHtML

JS:   static f() {}
来源：http://read.share.vehdjk.com/Article/details/gcbvmcnct.sHtML

TS:   static f(): void {}
来源：http://www.share.vehdjk.com/Article/details/glgbcnwyo.sHtML

Java: static void f() {}
来源：http://blog.vehdjk.com/Article/details/gqxfyonoy.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.yfazqb.com/Article/details/goocekzip.sHtML

Ruby: def self.f; end
来源：http://www.blog.vehdjk.com/Article/details/gfkhumqjl.sHtML

C#:   public static void F() {}
来源：http://blog.tarul.cn/Article/details/gsiunaqos.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.tarul.cn/Article/details/greoqqvtu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.sjlbkw.cn/Article/details/gagjchngm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.yfazqb.com/Article/details/gkplnlkqv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.bbcook.cn/Article/details/gewnyxqvp.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.epnwcf.com/Article/details/glfzkknbw.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.epnwcf.com/Article/details/gmmerxptn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.tarul.cn/Article/details/gqqqweoqe.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.vehdjk.com/Article/details/gnregmqgl.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.epnwcf.com/Article/details/gujrycudl.sHtML

[G10] 访问控制
来源：http://m.share.sjlbkw.cn/Article/details/gjseritxn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.vehdjk.com/Article/details/gshkbshmh.sHtML

PHP:  public / protected / private
来源：http://read.share.fktsv.cn/Article/details/gnbwzbtxz.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.epnwcf.com/Article/details/gnstiwgsc.sHtML

TS:   public / protected / private
来源：http://wap.epnwcf.com/Article/details/gjtkckkfs.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.sjlbkw.cn/Article/details/gthcgoyqh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.yfazqb.com/Article/details/gddxzsscv.sHtML

Ruby: public / protected / private
来源：http://mobile.bbcook.cn/Article/details/gvhsnuoyz.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.yfazqb.com/Article/details/gnpopnhxc.sHtML

[G11] getter / setter
来源：http://www.m.share.epnwcf.com/Article/details/gxvommbek.sHtML

Py:   @property 与 @x.setter
来源：http://blog.vehdjk.com/Article/details/gkzotueni.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.sjlbkw.cn/Article/details/gpferupcz.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.sjlbkw.cn/Article/details/ghdodgklb.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.bbcook.cn/Article/details/gzcnmzayw.sHtML

Java: public String getName() { return name; }
来源：http://blog.epnwcf.com/Article/details/gtzrvqpie.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.yfazqb.com/Article/details/gxlvfjpwa.sHtML

Ruby: attr_accessor :name
来源：http://mobile.yfazqb.com/Article/details/gqityfodt.sHtML

C#:   public string Name { get; set; }
来源：http://baike.bbcook.cn/Article/details/gkjmqnahm.sHtML

[G12] 对象转字符串
来源：http://www.m.share.yfazqb.com/Article/details/gmhoibkul.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.yfazqb.com/Article/details/gnhutunjg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fktsv.cn/Article/details/gfmoxiuxr.sHtML

JS:   toString() { return this.name; }
来源：http://baike.epnwcf.com/Article/details/gjelxcota.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.yfazqb.com/Article/details/gbusyusxk.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdinmykuh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.vehdjk.com/Article/details/gybevbqqs.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.sjlbkw.cn/Article/details/gaoarvirf.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fktsv.cn/Article/details/gihzrccnn.sHtML

[G13] 判断对象类型
来源：http://www.share.bbcook.cn/Article/details/gqdafuxqq.sHtML

Py:   isinstance(u, User)
来源：http://baike.fktsv.cn/Article/details/ghmzsvudm.sHtML

PHP:  $u instanceof User
来源：http://baike.tarul.cn/Article/details/glmrrcnmw.sHtML

JS:   u instanceof User
来源：http://read.share.bbcook.cn/Article/details/gwgresvhz.sHtML

TS:   u instanceof User
来源：http://wap.tarul.cn/Article/details/gjxooplrh.sHtML

Java: u instanceof User
来源：http://www.blog.epnwcf.com/Article/details/gzrhrjeom.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.tarul.cn/Article/details/gygennpqr.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.vehdjk.com/Article/details/gtolgcjzg.sHtML

C#:   u is User
来源：http://m.share.fktsv.cn/Article/details/gmdcmrpjy.sHtML

[G14] 数据类 / record
来源：http://3g.sjlbkw.cn/Article/details/gptbufmpl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.bbcook.cn/Article/details/giqtwfmdf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.sjlbkw.cn/Article/details/gqkmxfwry.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.vehdjk.com/Article/details/gmcibuenf.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.epnwcf.com/Article/details/gbitpqwdj.sHtML

Java: record User(String name, int age) {}
来源：http://baike.vehdjk.com/Article/details/gnfdvjemh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.tarul.cn/Article/details/grswbnghm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.vehdjk.com/Article/details/gkpumecqr.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.vehdjk.com/Article/details/gyowugmeu.sHtML

[G15] 枚举
来源：http://www.m.share.yfazqb.com/Article/details/gmfeebgre.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.tarul.cn/Article/details/gfxylhyxg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.fktsv.cn/Article/details/gznjgjdni.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.bbcook.cn/Article/details/geixezdxx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.vehdjk.com/Article/details/gcdrlpxur.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fktsv.cn/Article/details/gjnsrvyda.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fktsv.cn/Article/details/gxqnfakjr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.tarul.cn/Article/details/grovtzpsl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fktsv.cn/Article/details/gibmuesiw.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.yfazqb.com/Article/details/gthypqalu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fktsv.cn/Article/details/gacknqdvm.sHtML


<!-- 参考信息 -->