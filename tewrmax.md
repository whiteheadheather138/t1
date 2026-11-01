代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.vehdjk.com/Article/details/ghxmeveut.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.yfazqb.com/Article/details/gcwwldkvp.sHtML

Ruby: s.capitalize
来源：http://wap.sjlbkw.cn/Article/details/gpxgndwrc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.sjlbkw.cn/Article/details/guglthxlw.sHtML

[E18] 模板占位符替换
来源：http://blog.tarul.cn/Article/details/gbtzharfr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.yfazqb.com/Article/details/gxtfhkwra.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fktsv.cn/Article/details/gaxwgsecj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.epnwcf.com/Article/details/gyzmbgsdw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.tarul.cn/Article/details/gqwlliotb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.yfazqb.com/Article/details/gjiiirqpi.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fktsv.cn/Article/details/gvpihhzsu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.bbcook.cn/Article/details/gemxwkjnf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fktsv.cn/Article/details/gvqqvgccr.sHtML

[E19] 多行文本按行拆分
来源：http://baike.yfazqb.com/Article/details/gqoxyjjmi.sHtML

Py:   s.splitlines()
来源：http://www.m.share.yfazqb.com/Article/details/gjauwdcul.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gnmlpxewc.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.sjlbkw.cn/Article/details/ggrjhoimq.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.yfazqb.com/Article/details/gdfxkkyou.sHtML

Java: s.lines().toList()
来源：http://m.share.tarul.cn/Article/details/ggmlmzqxp.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.bbcook.cn/Article/details/guflhmrai.sHtML

Ruby: s.lines
来源：http://baike.fktsv.cn/Article/details/gxmqujobb.sHtML

C#:   s.Split('\n')
来源：http://www.blog.vehdjk.com/Article/details/gvlsjjsxj.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.yfazqb.com/Article/details/gtdlcswoh.sHtML

Py:   if not s:
来源：http://blog.sjlbkw.cn/Article/details/gvwnztxkn.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.sjlbkw.cn/Article/details/gvmlymomj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.yfazqb.com/Article/details/gurzxypzx.sHtML

TS:   if (s === "") {}
来源：http://wap.bbcook.cn/Article/details/gxllgiozj.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.epnwcf.com/Article/details/gdbestssp.sHtML

Go:   if s == "" {}
来源：http://read.share.fktsv.cn/Article/details/glpxnkkze.sHtML

Ruby: if s.empty?
来源：http://baike.fktsv.cn/Article/details/gfqxcnjca.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.vehdjk.com/Article/details/ghocgzdgk.sHtML

[E21] 超长截断加省略号
来源：http://blog.fktsv.cn/Article/details/gcqyqnyts.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.vehdjk.com/Article/details/gqjjgsaey.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.bbcook.cn/Article/details/gpescokof.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.bbcook.cn/Article/details/gedevpizc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.sjlbkw.cn/Article/details/glgomwvyq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.epnwcf.com/Article/details/ggdyddlmu.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.epnwcf.com/Article/details/glajnghmg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.tarul.cn/Article/details/gksnlfihr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.epnwcf.com/Article/details/grgatadin.sHtML

[E22] 字节长度与字符长度
来源：http://baike.epnwcf.com/Article/details/gfpvbikjw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.sjlbkw.cn/Article/details/gihmyzxdn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.epnwcf.com/Article/details/giygmlkqu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fktsv.cn/Article/details/gvbbcwmdd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.epnwcf.com/Article/details/gghrjvvff.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.tarul.cn/Article/details/gnuuctzub.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fktsv.cn/Article/details/gvlaeaqxw.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.sjlbkw.cn/Article/details/gbwaqpbuf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.tarul.cn/Article/details/gdheinjuk.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gqtxyqidq.sHtML

F. 文件与目录
来源：http://wap.sjlbkw.cn/Article/details/gyjdnhrgl.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gbmrohvww.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fktsv.cn/Article/details/gghisjjlx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.sjlbkw.cn/Article/details/gmxmfdlvh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/glkjjvdqd.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.epnwcf.com/Article/details/glwdglchs.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.vehdjk.com/Article/details/gnggunsmx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/gwezfrbnx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.epnwcf.com/Article/details/gknljtdbz.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.tarul.cn/Article/details/ghjheacid.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/giwldkziw.sHtML

[F02] 逐行读取文件
来源：http://m.share.epnwcf.com/Article/details/gtgbkqpdw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fktsv.cn/Article/details/gcolzxray.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fktsv.cn/Article/details/gfljpppmd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.tarul.cn/Article/details/gcahobzrq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.yfazqb.com/Article/details/giykakijj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.bbcook.cn/Article/details/gqnahewlt.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.yfazqb.com/Article/details/gxuofdiau.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.fktsv.cn/Article/details/gakolzspk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fktsv.cn/Article/details/gumfwibbp.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.bbcook.cn/Article/details/gfhnlzqqg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.vehdjk.com/Article/details/guxahceac.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.yfazqb.com/Article/details/gbpkgjnox.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.tarul.cn/Article/details/gquiuejhi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.epnwcf.com/Article/details/gvbqhqvox.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fktsv.cn/Article/details/gdobwdeow.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.yfazqb.com/Article/details/gijgweiin.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.yfazqb.com/Article/details/gtptcuxtf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.vehdjk.com/Article/details/gxgfykkug.sHtML

[F04] 追加写入文件
来源：http://wap.vehdjk.com/Article/details/gveoijmkp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.bbcook.cn/Article/details/gubtenvwk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.sjlbkw.cn/Article/details/gqismvxsf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.epnwcf.com/Article/details/gupyhixgv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fktsv.cn/Article/details/gnqvjmcgw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.tarul.cn/Article/details/gkwtqcrar.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.sjlbkw.cn/Article/details/gemeaxabk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.bbcook.cn/Article/details/gcxvpczam.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.yfazqb.com/Article/details/gbjdwhdbn.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.bbcook.cn/Article/details/gpgzzfxqz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.epnwcf.com/Article/details/gxodzcerx.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gmwzhnonv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.tarul.cn/Article/details/grshrpvet.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.tarul.cn/Article/details/gfwnnfpzb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fktsv.cn/Article/details/gtkqdtsir.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.bbcook.cn/Article/details/gnpcsumwx.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gzaxvibxi.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gtdjrpszr.sHtML

[F06] 删除文件
来源：http://mobile.fktsv.cn/Article/details/gdqrffhpb.sHtML

Py:   os.remove("a.txt")
来源：http://wap.bbcook.cn/Article/details/gjgkgwahx.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.yfazqb.com/Article/details/glrdvuijx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gbfkwjuiq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gigatffij.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.sjlbkw.cn/Article/details/gpkmfrbjk.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gvuhkaaej.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.epnwcf.com/Article/details/geqmexrrf.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.yfazqb.com/Article/details/gszrktgun.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fktsv.cn/Article/details/gdxbbzqof.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.vehdjk.com/Article/details/gkocoqkqe.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.epnwcf.com/Article/details/gpioklhjc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fktsv.cn/Article/details/gdzhvkjvs.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.yfazqb.com/Article/details/gqcffvnhc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.yfazqb.com/Article/details/gtjxswnge.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmaddaceh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.bbcook.cn/Article/details/galdryvxw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.epnwcf.com/Article/details/gecnelwwk.sHtML

[F08] 遍历目录
来源：http://www.m.share.vehdjk.com/Article/details/gckaiqfho.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.bbcook.cn/Article/details/gibusiksn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.yfazqb.com/Article/details/gkbomknio.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.bbcook.cn/Article/details/gffvdeipp.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fktsv.cn/Article/details/gnmecqgfo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.tarul.cn/Article/details/glrhfadjv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.epnwcf.com/Article/details/gjrnvkojq.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.sjlbkw.cn/Article/details/gkrdzpepw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fktsv.cn/Article/details/gprrmbyqm.sHtML

[F09] 获取文件大小
来源：http://read.share.vehdjk.com/Article/details/gmqbdyrfp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gzbkahhgm.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gvglqiaxj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.yfazqb.com/Article/details/grmgadsho.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.vehdjk.com/Article/details/gsjyjodew.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fktsv.cn/Article/details/gptevzuun.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.epnwcf.com/Article/details/gjcsjndns.sHtML

Ruby: File.size("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/glsjjszif.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.epnwcf.com/Article/details/gkgmxtwiv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.bbcook.cn/Article/details/gmgtdhmuq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/gssdicojq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gncstlomf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.tarul.cn/Article/details/gefhoevig.sHtML

TS:   path.extname("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gvybwxike.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.bbcook.cn/Article/details/gogslxezt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gzrdycsda.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/gynzvdwqj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/gtkmrkaoh.sHtML

[F11] 复制与移动文件
来源：http://baike.bbcook.cn/Article/details/gvydbrixa.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.bbcook.cn/Article/details/goqxfbuxs.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.epnwcf.com/Article/details/gnkzqbjtj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.tarul.cn/Article/details/gxooaqkdc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/gotzhkkvx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.vehdjk.com/Article/details/gxkhaqcev.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fktsv.cn/Article/details/gangxquba.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.bbcook.cn/Article/details/gueytaiic.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.tarul.cn/Article/details/glybdynxp.sHtML

[F12] CSV 读写
来源：http://www.share.vehdjk.com/Article/details/grqilqduv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.yfazqb.com/Article/details/gtsyhmorg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fktsv.cn/Article/details/gfqrunlnr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.epnwcf.com/Article/details/gvgzmpasm.sHtML

TS:   // 同上
来源：http://baike.epnwcf.com/Article/details/glkmfilxp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.tarul.cn/Article/details/gfhhmlknf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.vehdjk.com/Article/details/gosggpzqu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.epnwcf.com/Article/details/godbpmvjo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.yfazqb.com/Article/details/gojfxykuj.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gekonizkd.sHtML

G. 面向对象
来源：http://3g.bbcook.cn/Article/details/gqkzxirkx.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gocsdzqdw.sHtML

[G01] 定义类
来源：http://baike.bbcook.cn/Article/details/gmrogqmrn.sHtML

Py:   class User: pass
来源：http://www.blog.sjlbkw.cn/Article/details/gacluvxiu.sHtML

PHP:  class User {}
来源：http://3g.bbcook.cn/Article/details/glxdgwors.sHtML

JS:   class User {}
来源：http://blog.bbcook.cn/Article/details/gtggcujuy.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fktsv.cn/Article/details/gslmpdlzq.sHtML

Java: class User {}
来源：http://read.share.sjlbkw.cn/Article/details/gvfayyzus.sHtML

Go:   type User struct { Name string }
来源：http://wap.vehdjk.com/Article/details/geitcplrg.sHtML

Ruby: class User; end
来源：http://baike.fktsv.cn/Article/details/gtcreyrpl.sHtML

C#:   class User {}
来源：http://mobile.vehdjk.com/Article/details/gqrmsubdr.sHtML

[G02] 构造函数
来源：http://3g.bbcook.cn/Article/details/gfgmiiyoe.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.tarul.cn/Article/details/gafrwddyi.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.sjlbkw.cn/Article/details/gzcubsprr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.bbcook.cn/Article/details/gsrrylanl.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.yfazqb.com/Article/details/goxvzgqzp.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.bbcook.cn/Article/details/gwmcyeahq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.bbcook.cn/Article/details/giwobwllw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.yfazqb.com/Article/details/gkbibvspk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.vehdjk.com/Article/details/gxcngrvkr.sHtML

[G03] 实例属性
来源：http://read.share.epnwcf.com/Article/details/ggilluhlv.sHtML

Py:   self.name = "x"
来源：http://baike.vehdjk.com/Article/details/gtsqcwvcw.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.epnwcf.com/Article/details/gelowvzba.sHtML

JS:   this.name = "x";
来源：http://mobile.sjlbkw.cn/Article/details/gxrgscrfw.sHtML

TS:   name: string = "x";
来源：http://blog.bbcook.cn/Article/details/grnuqcqqj.sHtML

Java: private String name;
来源：http://blog.fktsv.cn/Article/details/gbkjsoyce.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.tarul.cn/Article/details/gppqldorx.sHtML

Ruby: @name = "x"
来源：http://read.share.fktsv.cn/Article/details/gsvikzzqm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.tarul.cn/Article/details/gmkhpqevb.sHtML

[G04] 定义方法
来源：http://www.m.share.yfazqb.com/Article/details/gzddlhxew.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.yfazqb.com/Article/details/gjuhkhgfa.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gphrjizcl.sHtML

JS:   greet() { return this.name; }
来源：http://3g.sjlbkw.cn/Article/details/gmlfegxfa.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.epnwcf.com/Article/details/gpagohbly.sHtML

Java: String greet() { return name; }
来源：http://read.share.sjlbkw.cn/Article/details/gqsxhjznh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.vehdjk.com/Article/details/ggcgygpvl.sHtML

Ruby: def greet; @name; end
来源：http://wap.fktsv.cn/Article/details/ghcwvufcm.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.bbcook.cn/Article/details/gdkiubtin.sHtML

[G05] 继承
来源：http://mobile.yfazqb.com/Article/details/gxudsiypc.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.yfazqb.com/Article/details/gcvykzgyd.sHtML

PHP:  class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/gqiygkcbc.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.bbcook.cn/Article/details/gwgslmwki.sHtML

TS:   class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/gqfajkifl.sHtML

Java: class Admin extends User {}
来源：http://baike.epnwcf.com/Article/details/gyikneeqs.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.bbcook.cn/Article/details/gpqqelgib.sHtML

Ruby: class Admin < User; end
来源：http://www.share.vehdjk.com/Article/details/gfjgtnzxd.sHtML

C#:   class Admin : User {}
来源：http://www.share.fktsv.cn/Article/details/gjwlqivka.sHtML

[G06] 重写方法
来源：http://m.share.fktsv.cn/Article/details/gbhbnnagv.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.sjlbkw.cn/Article/details/gytiogksh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/gmtofwvol.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.epnwcf.com/Article/details/ghpxfqcbb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.vehdjk.com/Article/details/gahdczqgr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.bbcook.cn/Article/details/gtxlcveut.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.sjlbkw.cn/Article/details/genezhrjb.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.vehdjk.com/Article/details/gjzkwnsor.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.sjlbkw.cn/Article/details/grfrubuup.sHtML

[G07] 调用父类方法
来源：http://m.share.bbcook.cn/Article/details/grnjgyxfm.sHtML

Py:   super().greet()
来源：http://www.share.bbcook.cn/Article/details/gmgvjghlf.sHtML

PHP:  parent::greet();
来源：http://mobile.bbcook.cn/Article/details/gqbaqfbdg.sHtML

JS:   super.greet();
来源：http://m.share.fktsv.cn/Article/details/glzwjyovq.sHtML

TS:   super.greet();
来源：http://www.m.share.fktsv.cn/Article/details/gdugnlunu.sHtML

Java: super.greet();
来源：http://3g.tarul.cn/Article/details/gndchsrsn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.epnwcf.com/Article/details/gimzzgvml.sHtML

Ruby: super
来源：http://www.m.share.epnwcf.com/Article/details/gjjroeddw.sHtML

C#:   base.Greet();
来源：http://blog.fktsv.cn/Article/details/grtcafnfl.sHtML

[G08] 静态方法与属性
来源：http://read.share.epnwcf.com/Article/details/goosxcxvz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.yfazqb.com/Article/details/gltefamlm.sHtML

PHP:  public static function f() {}
来源：http://wap.tarul.cn/Article/details/gngmgqkcu.sHtML

JS:   static f() {}
来源：http://3g.epnwcf.com/Article/details/gclawluof.sHtML

TS:   static f(): void {}
来源：http://blog.tarul.cn/Article/details/gzppixkni.sHtML

Java: static void f() {}
来源：http://blog.tarul.cn/Article/details/gedwvcowi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.sjlbkw.cn/Article/details/gswtnmsrz.sHtML

Ruby: def self.f; end
来源：http://3g.sjlbkw.cn/Article/details/gdkexfcrm.sHtML

C#:   public static void F() {}
来源：http://3g.epnwcf.com/Article/details/ghlymgtjt.sHtML

[G09] 接口 / 抽象类
来源：http://baike.vehdjk.com/Article/details/gnvhufopd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.vehdjk.com/Article/details/ggdyualpq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.epnwcf.com/Article/details/gjxvucoon.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.bbcook.cn/Article/details/gaaabrgyg.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fktsv.cn/Article/details/gdcubahce.sHtML

Java: interface Shape { double area(); }
来源：http://wap.bbcook.cn/Article/details/gzwqhkwzl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.epnwcf.com/Article/details/ghjiksbzw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.yfazqb.com/Article/details/gjsuhielk.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.vehdjk.com/Article/details/gsrkzroha.sHtML

[G10] 访问控制
来源：http://mobile.yfazqb.com/Article/details/getctriey.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.sjlbkw.cn/Article/details/gnuuhvxqt.sHtML

PHP:  public / protected / private
来源：http://www.blog.epnwcf.com/Article/details/gbokthwzk.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.sjlbkw.cn/Article/details/gsbazgsux.sHtML

TS:   public / protected / private
来源：http://baike.tarul.cn/Article/details/gepgwvyab.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.vehdjk.com/Article/details/gqjlvxrux.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.sjlbkw.cn/Article/details/gkpoenzsp.sHtML

Ruby: public / protected / private
来源：http://m.share.sjlbkw.cn/Article/details/gavpfgvht.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.epnwcf.com/Article/details/gqxwlzzzp.sHtML

[G11] getter / setter
来源：http://mobile.vehdjk.com/Article/details/gbsqecslp.sHtML

Py:   @property 与 @x.setter
来源：http://blog.epnwcf.com/Article/details/gfzbtrghp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.bbcook.cn/Article/details/gwlaidjky.sHtML

JS:   get name() { return this._name; }
来源：http://blog.bbcook.cn/Article/details/gcddehjhg.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.bbcook.cn/Article/details/gusppetyq.sHtML

Java: public String getName() { return name; }
来源：http://3g.epnwcf.com/Article/details/gdjdyaxln.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fktsv.cn/Article/details/gikxhqhwy.sHtML

Ruby: attr_accessor :name
来源：http://mobile.vehdjk.com/Article/details/gvgkvvalm.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.sjlbkw.cn/Article/details/gtbcsjmjb.sHtML

[G12] 对象转字符串
来源：http://read.share.bbcook.cn/Article/details/gwfjoabkn.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.sjlbkw.cn/Article/details/goykjxbni.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.yfazqb.com/Article/details/gndhcqunw.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.yfazqb.com/Article/details/golymcmkd.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fktsv.cn/Article/details/gekbikrvm.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.vehdjk.com/Article/details/gkctwnjzc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.epnwcf.com/Article/details/goqivnexp.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.bbcook.cn/Article/details/ggzsulmlo.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.vehdjk.com/Article/details/gzumndvlo.sHtML

[G13] 判断对象类型
来源：http://www.share.yfazqb.com/Article/details/gqlnmwand.sHtML

Py:   isinstance(u, User)
来源：http://baike.vehdjk.com/Article/details/gufnrfozs.sHtML

PHP:  $u instanceof User
来源：http://3g.sjlbkw.cn/Article/details/gxtbkdjsr.sHtML

JS:   u instanceof User
来源：http://wap.fktsv.cn/Article/details/grcmkztuq.sHtML

TS:   u instanceof User
来源：http://3g.epnwcf.com/Article/details/gyscghofw.sHtML

Java: u instanceof User
来源：http://read.share.sjlbkw.cn/Article/details/gsjvpaxsy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.vehdjk.com/Article/details/gosimttmh.sHtML

Ruby: u.is_a?(User)
来源：http://wap.bbcook.cn/Article/details/glsasebpx.sHtML

C#:   u is User
来源：http://www.blog.fktsv.cn/Article/details/gjjbhihjr.sHtML

[G14] 数据类 / record
来源：http://read.share.epnwcf.com/Article/details/gzdhuihbm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.bbcook.cn/Article/details/gohdrcbjm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.epnwcf.com/Article/details/gxqlyjtcw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.epnwcf.com/Article/details/gdvjnoggk.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.bbcook.cn/Article/details/gvtqpxpwa.sHtML

Java: record User(String name, int age) {}
来源：http://3g.sjlbkw.cn/Article/details/grvasgqom.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fktsv.cn/Article/details/gquzjbjcs.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.epnwcf.com/Article/details/gvagnswut.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.sjlbkw.cn/Article/details/gdqorlvjk.sHtML

[G15] 枚举
来源：http://3g.fktsv.cn/Article/details/gvwivzgia.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.vehdjk.com/Article/details/gktmbyipo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.yfazqb.com/Article/details/gnzdtjcxs.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fktsv.cn/Article/details/gpgpxttuw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.tarul.cn/Article/details/gjzpizife.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.yfazqb.com/Article/details/gjckyrfqo.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fktsv.cn/Article/details/gvpsqaxzo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.yfazqb.com/Article/details/guopvamug.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.epnwcf.com/Article/details/giqvvsfdw.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.vehdjk.com/Article/details/gulwfrcaz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.epnwcf.com/Article/details/gkrzwiktc.sHtML


<!-- 参考信息 -->