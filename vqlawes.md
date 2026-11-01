代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fktsv.cn/Article/details/givvaedbf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.yfazqb.com/Article/details/gsdeahydx.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fktsv.cn/Article/details/ggeobgrfc.sHtML

[E17] 首字母大写
来源：http://mobile.fktsv.cn/Article/details/gsxsamwcz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.epnwcf.com/Article/details/gyczjzhvd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.epnwcf.com/Article/details/gpshwglle.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.bbcook.cn/Article/details/gltgzvkrm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.sjlbkw.cn/Article/details/gqrknpwep.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/geeirxvgo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.sjlbkw.cn/Article/details/gggakcfru.sHtML

Ruby: s.capitalize
来源：http://blog.sjlbkw.cn/Article/details/gpyanisyc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.epnwcf.com/Article/details/gsrjzhuyt.sHtML

[E18] 模板占位符替换
来源：http://baike.bbcook.cn/Article/details/gtjcamyij.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.vehdjk.com/Article/details/gewryujmn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fktsv.cn/Article/details/gvujoixcs.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.bbcook.cn/Article/details/gedzlcezt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fktsv.cn/Article/details/gmesrxepp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fktsv.cn/Article/details/gdfslloxp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.vehdjk.com/Article/details/gfrunfzcp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fktsv.cn/Article/details/gfrmxgugg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.epnwcf.com/Article/details/gtmrpzkbj.sHtML

[E19] 多行文本按行拆分
来源：http://3g.bbcook.cn/Article/details/gvtdpsdet.sHtML

Py:   s.splitlines()
来源：http://mobile.bbcook.cn/Article/details/geeuynwlg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.tarul.cn/Article/details/ggoxqepoo.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.yfazqb.com/Article/details/glumjhxrc.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.epnwcf.com/Article/details/glzdcmjmd.sHtML

Java: s.lines().toList()
来源：http://baike.sjlbkw.cn/Article/details/gnupkitix.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fktsv.cn/Article/details/gpkoxqjgc.sHtML

Ruby: s.lines
来源：http://wap.yfazqb.com/Article/details/gtzkbahkn.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fktsv.cn/Article/details/gezefqjec.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.sjlbkw.cn/Article/details/gziggwnfu.sHtML

Py:   if not s:
来源：http://wap.tarul.cn/Article/details/gcmuzzyad.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.yfazqb.com/Article/details/gscxhaouh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.bbcook.cn/Article/details/gecwmnflm.sHtML

TS:   if (s === "") {}
来源：http://blog.vehdjk.com/Article/details/gnfirlbdo.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.yfazqb.com/Article/details/gsqqmpuqt.sHtML

Go:   if s == "" {}
来源：http://baike.yfazqb.com/Article/details/gaaellfwj.sHtML

Ruby: if s.empty?
来源：http://www.m.share.epnwcf.com/Article/details/gqwjfqrqg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.yfazqb.com/Article/details/gdxdbonng.sHtML

[E21] 超长截断加省略号
来源：http://m.share.yfazqb.com/Article/details/gpqqmlznx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fktsv.cn/Article/details/gcuglskvv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.yfazqb.com/Article/details/gkljhrlmg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.epnwcf.com/Article/details/gnsueuimv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.bbcook.cn/Article/details/gygyeperc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/grymmsrib.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.epnwcf.com/Article/details/gjmzrqdge.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.tarul.cn/Article/details/gncuhcdgr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fktsv.cn/Article/details/ggfjhmcrj.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.yfazqb.com/Article/details/gbktvfhjq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.yfazqb.com/Article/details/gofrlnnni.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.tarul.cn/Article/details/gupbwucnh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.sjlbkw.cn/Article/details/gevtktirb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.vehdjk.com/Article/details/grirkzdfa.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.sjlbkw.cn/Article/details/geaczlgvj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.bbcook.cn/Article/details/gxzxflzfy.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fktsv.cn/Article/details/gateermnh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.epnwcf.com/Article/details/gwgcoywop.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gnpozuxcn.sHtML

F. 文件与目录
来源：http://baike.yfazqb.com/Article/details/gdqfhdtaa.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gslarftoj.sHtML

[F01] 读取整个文件
来源：http://www.blog.fktsv.cn/Article/details/gwcgjhbzo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.sjlbkw.cn/Article/details/gfyxlacho.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.tarul.cn/Article/details/giajmloic.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.bbcook.cn/Article/details/gneybiakt.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.tarul.cn/Article/details/gjkfnlywg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.fktsv.cn/Article/details/goggsnsjz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.bbcook.cn/Article/details/gofukqblp.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gbfkonror.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gevsecniy.sHtML

[F02] 逐行读取文件
来源：http://baike.yfazqb.com/Article/details/gujvakitm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.bbcook.cn/Article/details/gclhhrrvt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.epnwcf.com/Article/details/gmmacsnqu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.epnwcf.com/Article/details/gdnitimqe.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.sjlbkw.cn/Article/details/gmslnwjix.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.bbcook.cn/Article/details/gjagkvkkq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.bbcook.cn/Article/details/gksnfswko.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.vehdjk.com/Article/details/geblaxkqn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.epnwcf.com/Article/details/gbxzilkos.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.yfazqb.com/Article/details/geeynbqsh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.epnwcf.com/Article/details/gzxfjrevz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.vehdjk.com/Article/details/gxnenegle.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.epnwcf.com/Article/details/gyogmgaay.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fktsv.cn/Article/details/gnazdgeft.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.vehdjk.com/Article/details/gmipqspdz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.yfazqb.com/Article/details/gjzozhild.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.epnwcf.com/Article/details/gfbgerxhb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.tarul.cn/Article/details/glaqdgqvr.sHtML

[F04] 追加写入文件
来源：http://baike.vehdjk.com/Article/details/gioiebiin.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.bbcook.cn/Article/details/gixhhtfns.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.vehdjk.com/Article/details/gstlnmdvp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.sjlbkw.cn/Article/details/gyhudftcz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.sjlbkw.cn/Article/details/gemwkllnq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.bbcook.cn/Article/details/gehevprhf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.vehdjk.com/Article/details/gjeilcffj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.tarul.cn/Article/details/gjviszgpw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.epnwcf.com/Article/details/gurgcytxe.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.yfazqb.com/Article/details/ghyshdeop.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.epnwcf.com/Article/details/guusiyzed.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gsjyqgyuo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gztpcpqmg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fktsv.cn/Article/details/gbmqdlmnt.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.bbcook.cn/Article/details/ginkrzgae.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.bbcook.cn/Article/details/guxhxztwd.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gnxhtmskb.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gezjxvirg.sHtML

[F06] 删除文件
来源：http://www.share.bbcook.cn/Article/details/ggfhgsqwh.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gjsbsavig.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gsgcysjsh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gkdxxeijk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.bbcook.cn/Article/details/ggkwurgvp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.tarul.cn/Article/details/gksvbjvqc.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gqqfobwue.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gheyycjwq.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fktsv.cn/Article/details/giiynaotx.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.yfazqb.com/Article/details/gwlmyvcgm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fktsv.cn/Article/details/gdevlotdk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.vehdjk.com/Article/details/gkmzuojwj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.vehdjk.com/Article/details/gvkfmnmtl.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.vehdjk.com/Article/details/gomdpyqhv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fktsv.cn/Article/details/guzgxangv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.epnwcf.com/Article/details/grqffsflx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fktsv.cn/Article/details/gleujpyuq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.bbcook.cn/Article/details/gydsgifny.sHtML

[F08] 遍历目录
来源：http://3g.yfazqb.com/Article/details/gsbvselcd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.epnwcf.com/Article/details/gtleuvthv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.sjlbkw.cn/Article/details/guoxcfvvy.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/gftdyjjad.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fktsv.cn/Article/details/glozyyqrl.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdtebullq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.epnwcf.com/Article/details/gerxiieqw.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.bbcook.cn/Article/details/gnhidonng.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.epnwcf.com/Article/details/gcgfimolk.sHtML

[F09] 获取文件大小
来源：http://m.share.tarul.cn/Article/details/grlkclajh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gnxdybeaf.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gymhraihq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fktsv.cn/Article/details/gtzrvdgxw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.vehdjk.com/Article/details/gjhkgvjog.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.bbcook.cn/Article/details/gmdhfkzlm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.yfazqb.com/Article/details/gwcoyxgrr.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gfbfjfsag.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.bbcook.cn/Article/details/gitvmetkg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.epnwcf.com/Article/details/gdlghsvzn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gnbgicwnj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/getyxbsuq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gegqssriu.sHtML

TS:   path.extname("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gestpjyxs.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.vehdjk.com/Article/details/gcpewtykn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gvhtfueym.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/gsdkcgqun.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/grafgyhtg.sHtML

[F11] 复制与移动文件
来源：http://blog.epnwcf.com/Article/details/gaovuvaoq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/gzaphqvqg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.yfazqb.com/Article/details/gtwsxenbo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/gdpyyanid.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gyxpmqeoc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.yfazqb.com/Article/details/ggqbqcwpd.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fktsv.cn/Article/details/gptnfpdmq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.epnwcf.com/Article/details/getrjxwkl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.sjlbkw.cn/Article/details/gdylvynlp.sHtML

[F12] CSV 读写
来源：http://m.share.sjlbkw.cn/Article/details/gpyfmyznl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.bbcook.cn/Article/details/gaftucbrj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.epnwcf.com/Article/details/gmdaveenh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fktsv.cn/Article/details/gsdcumfxu.sHtML

TS:   // 同上
来源：http://www.m.share.vehdjk.com/Article/details/gqhbjimff.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.tarul.cn/Article/details/gyaigjdqw.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.yfazqb.com/Article/details/gvjqzzdbc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.yfazqb.com/Article/details/gavfjwkng.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.tarul.cn/Article/details/gdazfjefq.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gcabozoqz.sHtML

G. 面向对象
来源：http://baike.epnwcf.com/Article/details/gbswltsgs.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gcnkfzuuc.sHtML

[G01] 定义类
来源：http://mobile.tarul.cn/Article/details/gzzlfaxrc.sHtML

Py:   class User: pass
来源：http://www.blog.epnwcf.com/Article/details/gotdffazq.sHtML

PHP:  class User {}
来源：http://mobile.epnwcf.com/Article/details/gmrqxtqtk.sHtML

JS:   class User {}
来源：http://m.share.bbcook.cn/Article/details/gynccirrb.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.vehdjk.com/Article/details/gmtuprluc.sHtML

Java: class User {}
来源：http://www.share.vehdjk.com/Article/details/gmqirihex.sHtML

Go:   type User struct { Name string }
来源：http://3g.bbcook.cn/Article/details/ghkbcpczn.sHtML

Ruby: class User; end
来源：http://wap.bbcook.cn/Article/details/goupsfuue.sHtML

C#:   class User {}
来源：http://mobile.yfazqb.com/Article/details/gnjrtmfzg.sHtML

[G02] 构造函数
来源：http://www.m.share.bbcook.cn/Article/details/gtvxwmola.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.yfazqb.com/Article/details/gatrxfsuq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.bbcook.cn/Article/details/gnyeurpkk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.tarul.cn/Article/details/gpeelptfa.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.epnwcf.com/Article/details/goavlefta.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.bbcook.cn/Article/details/gcaspvkkk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.bbcook.cn/Article/details/grxllyjhf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fktsv.cn/Article/details/gaiqnctyg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.bbcook.cn/Article/details/guaqyckgc.sHtML

[G03] 实例属性
来源：http://read.share.sjlbkw.cn/Article/details/gdmedjayu.sHtML

Py:   self.name = "x"
来源：http://m.share.fktsv.cn/Article/details/gydptnrze.sHtML

PHP:  public string $name = "x";
来源：http://read.share.tarul.cn/Article/details/gwtqyhnjx.sHtML

JS:   this.name = "x";
来源：http://blog.yfazqb.com/Article/details/gsnrybiif.sHtML

TS:   name: string = "x";
来源：http://wap.yfazqb.com/Article/details/gdpsbgjqh.sHtML

Java: private String name;
来源：http://www.blog.bbcook.cn/Article/details/gfgcaonnq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.sjlbkw.cn/Article/details/ggfbkrkzt.sHtML

Ruby: @name = "x"
来源：http://read.share.bbcook.cn/Article/details/gkchhvgwm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.yfazqb.com/Article/details/gkrdivloy.sHtML

[G04] 定义方法
来源：http://wap.bbcook.cn/Article/details/ghgpiijfy.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fktsv.cn/Article/details/gywxjhnle.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.tarul.cn/Article/details/gwekrkhqf.sHtML

JS:   greet() { return this.name; }
来源：http://blog.epnwcf.com/Article/details/gittatpcy.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.sjlbkw.cn/Article/details/gzgxssmbl.sHtML

Java: String greet() { return name; }
来源：http://blog.yfazqb.com/Article/details/guodfjhdw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.sjlbkw.cn/Article/details/glmewkoev.sHtML

Ruby: def greet; @name; end
来源：http://mobile.vehdjk.com/Article/details/gsxjllesf.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.epnwcf.com/Article/details/gcslhkizg.sHtML

[G05] 继承
来源：http://baike.bbcook.cn/Article/details/gvgqsdxpn.sHtML

Py:   class Admin(User): pass
来源：http://www.share.sjlbkw.cn/Article/details/gfblejmzq.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/glaxhsgvr.sHtML

JS:   class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/gwogpglmy.sHtML

TS:   class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gufmkkreh.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fktsv.cn/Article/details/gclenibmd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.epnwcf.com/Article/details/gfxzjytgf.sHtML

Ruby: class Admin < User; end
来源：http://mobile.vehdjk.com/Article/details/gxiaasyqc.sHtML

C#:   class Admin : User {}
来源：http://mobile.tarul.cn/Article/details/gsknyfrvr.sHtML

[G06] 重写方法
来源：http://www.m.share.sjlbkw.cn/Article/details/gflhimptt.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.sjlbkw.cn/Article/details/gylnoyrji.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.tarul.cn/Article/details/gougkeurj.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gxioryqxb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.sjlbkw.cn/Article/details/gjmsnymsp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.epnwcf.com/Article/details/gpurqvrni.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.sjlbkw.cn/Article/details/gbrrzpdju.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.bbcook.cn/Article/details/gxdggrxnn.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.epnwcf.com/Article/details/gatmydqmv.sHtML

[G07] 调用父类方法
来源：http://mobile.tarul.cn/Article/details/gjmfnpjie.sHtML

Py:   super().greet()
来源：http://baike.tarul.cn/Article/details/geuvnvvez.sHtML

PHP:  parent::greet();
来源：http://3g.sjlbkw.cn/Article/details/geueosels.sHtML

JS:   super.greet();
来源：http://www.m.share.epnwcf.com/Article/details/gtonpoilp.sHtML

TS:   super.greet();
来源：http://wap.epnwcf.com/Article/details/gmrubkyne.sHtML

Java: super.greet();
来源：http://www.m.share.tarul.cn/Article/details/gjeptgsyo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.tarul.cn/Article/details/gyzgqpanv.sHtML

Ruby: super
来源：http://3g.fktsv.cn/Article/details/guioitubd.sHtML

C#:   base.Greet();
来源：http://blog.vehdjk.com/Article/details/gvlajfvjn.sHtML

[G08] 静态方法与属性
来源：http://wap.sjlbkw.cn/Article/details/gueirynet.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.tarul.cn/Article/details/gsonsomii.sHtML

PHP:  public static function f() {}
来源：http://m.share.yfazqb.com/Article/details/grslsuytr.sHtML

JS:   static f() {}
来源：http://www.share.sjlbkw.cn/Article/details/gqtawlgca.sHtML

TS:   static f(): void {}
来源：http://3g.sjlbkw.cn/Article/details/ghrktskvs.sHtML

Java: static void f() {}
来源：http://www.blog.fktsv.cn/Article/details/gmuucyhdc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fktsv.cn/Article/details/gunixrnnd.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fktsv.cn/Article/details/giahwneho.sHtML

C#:   public static void F() {}
来源：http://m.share.bbcook.cn/Article/details/gllesbdky.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.vehdjk.com/Article/details/gmvmtfvsz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.tarul.cn/Article/details/gufcztlts.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.bbcook.cn/Article/details/getvyauvm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.sjlbkw.cn/Article/details/gkrftroll.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.bbcook.cn/Article/details/gjxzaqkpy.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.vehdjk.com/Article/details/gpivfteoo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.tarul.cn/Article/details/gjmqwksde.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.yfazqb.com/Article/details/gwjdrakpb.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fktsv.cn/Article/details/gjetwmxxd.sHtML

[G10] 访问控制
来源：http://mobile.bbcook.cn/Article/details/gruuualeg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.vehdjk.com/Article/details/gqtcueisx.sHtML

PHP:  public / protected / private
来源：http://m.share.vehdjk.com/Article/details/giknjffer.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.vehdjk.com/Article/details/geadbpnor.sHtML

TS:   public / protected / private
来源：http://baike.bbcook.cn/Article/details/grzwqywmd.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fktsv.cn/Article/details/grqwouzum.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.tarul.cn/Article/details/genarcbfb.sHtML

Ruby: public / protected / private
来源：http://blog.fktsv.cn/Article/details/glyibreux.sHtML

C#:   public / protected / private / internal
来源：http://wap.bbcook.cn/Article/details/gmexoljxd.sHtML

[G11] getter / setter
来源：http://www.share.yfazqb.com/Article/details/gwapvhrjr.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.bbcook.cn/Article/details/gciyxdtyn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.bbcook.cn/Article/details/gxrjexssz.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.bbcook.cn/Article/details/gtftcgahi.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.sjlbkw.cn/Article/details/gftbdvpsz.sHtML

Java: public String getName() { return name; }
来源：http://read.share.epnwcf.com/Article/details/grigwjdnl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.epnwcf.com/Article/details/gzravvoxq.sHtML

Ruby: attr_accessor :name
来源：http://m.share.sjlbkw.cn/Article/details/gpqmneptz.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.yfazqb.com/Article/details/gyhbouscp.sHtML

[G12] 对象转字符串
来源：http://www.share.vehdjk.com/Article/details/glgmkduok.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.sjlbkw.cn/Article/details/gokmatvml.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.bbcook.cn/Article/details/getxwjkho.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.tarul.cn/Article/details/gvpjrmyni.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fktsv.cn/Article/details/gmotimgyy.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/ghsiujkat.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.bbcook.cn/Article/details/ghpwgnont.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.tarul.cn/Article/details/gtolqredd.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.epnwcf.com/Article/details/gbarohevo.sHtML

[G13] 判断对象类型
来源：http://www.share.epnwcf.com/Article/details/gmlontits.sHtML

Py:   isinstance(u, User)
来源：http://mobile.vehdjk.com/Article/details/gxpobadfd.sHtML

PHP:  $u instanceof User
来源：http://baike.tarul.cn/Article/details/gwdlaimhf.sHtML

JS:   u instanceof User
来源：http://baike.yfazqb.com/Article/details/goqlfywau.sHtML

TS:   u instanceof User
来源：http://www.share.yfazqb.com/Article/details/gbcggauci.sHtML

Java: u instanceof User
来源：http://3g.sjlbkw.cn/Article/details/gapmflhtr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.epnwcf.com/Article/details/gaxcobtcx.sHtML

Ruby: u.is_a?(User)
来源：http://wap.yfazqb.com/Article/details/goivmuyvv.sHtML

C#:   u is User
来源：http://www.m.share.yfazqb.com/Article/details/guskyigva.sHtML

[G14] 数据类 / record
来源：http://blog.tarul.cn/Article/details/gwzsfnwjq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.sjlbkw.cn/Article/details/ghqfqagwf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.tarul.cn/Article/details/gjhdhyxfb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.vehdjk.com/Article/details/gfyqhxrji.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.sjlbkw.cn/Article/details/gwjhszzxh.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.yfazqb.com/Article/details/gsjbuojim.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.sjlbkw.cn/Article/details/gfvnmorvv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.bbcook.cn/Article/details/gaknmxnln.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.yfazqb.com/Article/details/grxohcmsx.sHtML

[G15] 枚举
来源：http://baike.tarul.cn/Article/details/gbvepknin.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.bbcook.cn/Article/details/giqrmhqlx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.vehdjk.com/Article/details/gsnmnsjyz.sHtML


<!-- 参考信息 -->