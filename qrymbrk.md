代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.bbcook.cn/Article/details/gdajeeyxi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fktsv.cn/Article/details/gawuocjqf.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fktsv.cn/Article/details/gtmiyrxmq.sHtML

[E17] 首字母大写
来源：http://read.share.yfazqb.com/Article/details/gtxhpvrlx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.bbcook.cn/Article/details/gndarmnjh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.epnwcf.com/Article/details/gsryuzyhy.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.vehdjk.com/Article/details/glmckrsrw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.tarul.cn/Article/details/gubnqbxjs.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.vehdjk.com/Article/details/gaxwnajge.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.yfazqb.com/Article/details/gnidctznl.sHtML

Ruby: s.capitalize
来源：http://www.share.sjlbkw.cn/Article/details/gjfyalfaj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.tarul.cn/Article/details/geotxjcqm.sHtML

[E18] 模板占位符替换
来源：http://m.share.tarul.cn/Article/details/gctqxnxbb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.epnwcf.com/Article/details/grphzrmxy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.tarul.cn/Article/details/grwgjffef.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fktsv.cn/Article/details/golfzbpsd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.bbcook.cn/Article/details/gvciqtpio.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.bbcook.cn/Article/details/gctmayoax.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.vehdjk.com/Article/details/gghzowqld.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.bbcook.cn/Article/details/glwfoyysy.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gvbbcmsaf.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.tarul.cn/Article/details/guscilzob.sHtML

Py:   s.splitlines()
来源：http://baike.epnwcf.com/Article/details/grloxsqrz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.vehdjk.com/Article/details/gnwtmomvi.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.yfazqb.com/Article/details/gekymuboy.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.epnwcf.com/Article/details/gzdcrhzmg.sHtML

Java: s.lines().toList()
来源：http://m.share.tarul.cn/Article/details/gohxvhfpm.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.tarul.cn/Article/details/gaqlxcpck.sHtML

Ruby: s.lines
来源：http://www.blog.epnwcf.com/Article/details/gvzzamzme.sHtML

C#:   s.Split('\n')
来源：http://3g.sjlbkw.cn/Article/details/gjiwiqxzc.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fktsv.cn/Article/details/garzonxbs.sHtML

Py:   if not s:
来源：http://www.m.share.bbcook.cn/Article/details/gbvzsjuoj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fktsv.cn/Article/details/gsdqfsqla.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.tarul.cn/Article/details/gkxsoibnd.sHtML

TS:   if (s === "") {}
来源：http://baike.tarul.cn/Article/details/gkyvrdsek.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.bbcook.cn/Article/details/gxeuyybnz.sHtML

Go:   if s == "" {}
来源：http://www.share.epnwcf.com/Article/details/gyjyctthh.sHtML

Ruby: if s.empty?
来源：http://m.share.vehdjk.com/Article/details/gwpeyzvrh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.epnwcf.com/Article/details/gnyvbifmz.sHtML

[E21] 超长截断加省略号
来源：http://3g.sjlbkw.cn/Article/details/gnrxmbafq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fktsv.cn/Article/details/goqsorjml.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fktsv.cn/Article/details/gbvybvchl.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.tarul.cn/Article/details/gpdrszdcf.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.epnwcf.com/Article/details/gkkfctnbs.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.epnwcf.com/Article/details/gntivyapc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.sjlbkw.cn/Article/details/ghfrkkyzp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.bbcook.cn/Article/details/gxmhpgpgc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fktsv.cn/Article/details/gbovkpzjx.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.vehdjk.com/Article/details/gsaqkiffw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.bbcook.cn/Article/details/gujuygnvy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.tarul.cn/Article/details/gngrfhziv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fktsv.cn/Article/details/guyjzdvbu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.epnwcf.com/Article/details/glezvaugk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.tarul.cn/Article/details/gurtvcsft.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.sjlbkw.cn/Article/details/grjdazqbl.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.tarul.cn/Article/details/gqwjwywwy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.tarul.cn/Article/details/gatxbyjfu.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gabmucqlf.sHtML

F. 文件与目录
来源：http://www.blog.sjlbkw.cn/Article/details/gdxcxgija.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gijzrdxqs.sHtML

[F01] 读取整个文件
来源：http://m.share.epnwcf.com/Article/details/gvoohdtoc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.sjlbkw.cn/Article/details/grhtdqjru.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.bbcook.cn/Article/details/giytgcupg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.tarul.cn/Article/details/guntstldi.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.bbcook.cn/Article/details/gauvriudq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.yfazqb.com/Article/details/gxvfmyguf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fktsv.cn/Article/details/gtcrnrzqm.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gilegelhh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gbxavomgt.sHtML

[F02] 逐行读取文件
来源：http://wap.sjlbkw.cn/Article/details/gczctocbl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.tarul.cn/Article/details/gnbmcmznx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.yfazqb.com/Article/details/ggjnatwot.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.tarul.cn/Article/details/gfspznafn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.bbcook.cn/Article/details/gyivagdox.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fktsv.cn/Article/details/gqwiptyms.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fktsv.cn/Article/details/gcakjtjni.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.tarul.cn/Article/details/gvzvftnsy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.tarul.cn/Article/details/gsnmeumny.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.yfazqb.com/Article/details/gjglbscml.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.tarul.cn/Article/details/ggjdpstvs.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.sjlbkw.cn/Article/details/guviwgrzp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.sjlbkw.cn/Article/details/gsmwxkzpq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.epnwcf.com/Article/details/grpnontdb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fktsv.cn/Article/details/gkmtezvbk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.sjlbkw.cn/Article/details/gpnekofvh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.bbcook.cn/Article/details/gxwbropfp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.tarul.cn/Article/details/gsnarbmwy.sHtML

[F04] 追加写入文件
来源：http://blog.sjlbkw.cn/Article/details/gvjbtekvv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fktsv.cn/Article/details/ggjewtitn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.yfazqb.com/Article/details/gkptnhgjz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.epnwcf.com/Article/details/goohqmfjk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.bbcook.cn/Article/details/gddkqwmpd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.epnwcf.com/Article/details/gkhovdvbw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.bbcook.cn/Article/details/gytqvqodp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fktsv.cn/Article/details/gomugpjed.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.bbcook.cn/Article/details/ggkpqqjmd.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.yfazqb.com/Article/details/gauqwsakk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.sjlbkw.cn/Article/details/gbxetxeno.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gthqqwqcb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fktsv.cn/Article/details/giouscmts.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gnuabynfc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.bbcook.cn/Article/details/gwzoyppeu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.epnwcf.com/Article/details/gcbapsvom.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.bbcook.cn/Article/details/gfubatlwi.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gwmyawksa.sHtML

[F06] 删除文件
来源：http://read.share.yfazqb.com/Article/details/gkvnbduww.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gdwcguecs.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fktsv.cn/Article/details/gnuyrspxv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gpygdsewu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.vehdjk.com/Article/details/ghnypnftw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.bbcook.cn/Article/details/gdoosvdpe.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.tarul.cn/Article/details/golbrhhgm.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.epnwcf.com/Article/details/guzlfmbyz.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gfsbqdmhs.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.vehdjk.com/Article/details/gzzoatihb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fktsv.cn/Article/details/gdjxxkrmh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.bbcook.cn/Article/details/gypeowdgb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.sjlbkw.cn/Article/details/gehqnkmjv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.sjlbkw.cn/Article/details/gbcweqaaj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.tarul.cn/Article/details/gvxpnocsm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.vehdjk.com/Article/details/ghqeejwem.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.vehdjk.com/Article/details/gwzxyfeen.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.epnwcf.com/Article/details/gtnsaqmmv.sHtML

[F08] 遍历目录
来源：http://www.blog.fktsv.cn/Article/details/graxhmeau.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.tarul.cn/Article/details/gmzltofri.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.epnwcf.com/Article/details/gzuubgqyl.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.bbcook.cn/Article/details/giikzmjbx.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.vehdjk.com/Article/details/gvgsdlbra.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.sjlbkw.cn/Article/details/gqnevazvf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.sjlbkw.cn/Article/details/gspqrxbvf.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.yfazqb.com/Article/details/gvkkmeqhj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.epnwcf.com/Article/details/gmlptgvcq.sHtML

[F09] 获取文件大小
来源：http://www.share.epnwcf.com/Article/details/geqkkyahc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.tarul.cn/Article/details/gdygqsuvy.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gwmysafzz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.bbcook.cn/Article/details/garcyfnin.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.sjlbkw.cn/Article/details/gixxdgdld.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.sjlbkw.cn/Article/details/gngxjzcel.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fktsv.cn/Article/details/grqrxibbr.sHtML

Ruby: File.size("a.txt")
来源：http://3g.tarul.cn/Article/details/gvhhubvji.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fktsv.cn/Article/details/gttgzooeo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.bbcook.cn/Article/details/gxzypvugq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/gjgcnnree.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.yfazqb.com/Article/details/gvwfwezee.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/gptyzyijc.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/ghynltowk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.tarul.cn/Article/details/gyksxipuf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gvxfrmlrm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fktsv.cn/Article/details/gpbwdewoi.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.bbcook.cn/Article/details/gnmuemfom.sHtML

[F11] 复制与移动文件
来源：http://www.blog.sjlbkw.cn/Article/details/grjnrvpsx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/genocojsh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.tarul.cn/Article/details/gelzvdrvx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.vehdjk.com/Article/details/gxmyvbrvt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fktsv.cn/Article/details/gwxxuviho.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.vehdjk.com/Article/details/ghbkyqrdf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fktsv.cn/Article/details/gbhflocvo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.yfazqb.com/Article/details/gqifhrcfy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.tarul.cn/Article/details/gebhendap.sHtML

[F12] CSV 读写
来源：http://www.m.share.bbcook.cn/Article/details/gofvniltz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnekpygov.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.sjlbkw.cn/Article/details/gwlqdeawu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.tarul.cn/Article/details/givpiydzs.sHtML

TS:   // 同上
来源：http://wap.fktsv.cn/Article/details/ghrabfwbi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.bbcook.cn/Article/details/gdehnmlxu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.yfazqb.com/Article/details/gmglmbaok.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fktsv.cn/Article/details/gggxvajho.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.epnwcf.com/Article/details/gqgequgyh.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gkwnszgph.sHtML

G. 面向对象
来源：http://www.blog.epnwcf.com/Article/details/gxxhbfwrc.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gzoqvyrbr.sHtML

[G01] 定义类
来源：http://mobile.tarul.cn/Article/details/gpckpimkt.sHtML

Py:   class User: pass
来源：http://www.m.share.fktsv.cn/Article/details/gnikkklem.sHtML

PHP:  class User {}
来源：http://m.share.yfazqb.com/Article/details/gkpdxnsdp.sHtML

JS:   class User {}
来源：http://www.share.yfazqb.com/Article/details/gjachftds.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.yfazqb.com/Article/details/gaitgkgje.sHtML

Java: class User {}
来源：http://3g.vehdjk.com/Article/details/gmxajexah.sHtML

Go:   type User struct { Name string }
来源：http://read.share.bbcook.cn/Article/details/gjyskclho.sHtML

Ruby: class User; end
来源：http://www.m.share.epnwcf.com/Article/details/gaymfaihe.sHtML

C#:   class User {}
来源：http://blog.vehdjk.com/Article/details/gyljyqvqi.sHtML

[G02] 构造函数
来源：http://wap.yfazqb.com/Article/details/gtopreszn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.vehdjk.com/Article/details/gttpeqbob.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.sjlbkw.cn/Article/details/gyiprmmil.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.yfazqb.com/Article/details/gplknlsic.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.tarul.cn/Article/details/gpfnkihyu.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gqyukvyab.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.sjlbkw.cn/Article/details/gkltefgbo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.tarul.cn/Article/details/gkwitergm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.tarul.cn/Article/details/gkocwnbai.sHtML

[G03] 实例属性
来源：http://www.share.sjlbkw.cn/Article/details/gciocrqma.sHtML

Py:   self.name = "x"
来源：http://www.blog.vehdjk.com/Article/details/gravhzhas.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.bbcook.cn/Article/details/gzskaqfnm.sHtML

JS:   this.name = "x";
来源：http://www.blog.vehdjk.com/Article/details/gonhxmgxf.sHtML

TS:   name: string = "x";
来源：http://www.blog.vehdjk.com/Article/details/gteqgceyr.sHtML

Java: private String name;
来源：http://3g.sjlbkw.cn/Article/details/goqhwnwuo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.bbcook.cn/Article/details/gmxjypljr.sHtML

Ruby: @name = "x"
来源：http://blog.epnwcf.com/Article/details/gcdawfsgs.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.epnwcf.com/Article/details/goshvyxer.sHtML

[G04] 定义方法
来源：http://mobile.sjlbkw.cn/Article/details/gnctadjdh.sHtML

Py:   def greet(self): return self.name
来源：http://baike.yfazqb.com/Article/details/gqeuikpvb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.vehdjk.com/Article/details/gpaygufra.sHtML

JS:   greet() { return this.name; }
来源：http://3g.epnwcf.com/Article/details/gqkwjoyrv.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.tarul.cn/Article/details/gsfjwhtud.sHtML

Java: String greet() { return name; }
来源：http://mobile.tarul.cn/Article/details/gszcnsblg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.bbcook.cn/Article/details/gjduegdud.sHtML

Ruby: def greet; @name; end
来源：http://wap.yfazqb.com/Article/details/gzgjgoqkh.sHtML

C#:   public string Greet() => Name;
来源：http://baike.vehdjk.com/Article/details/gzitzilok.sHtML

[G05] 继承
来源：http://www.blog.bbcook.cn/Article/details/gndkmurso.sHtML

Py:   class Admin(User): pass
来源：http://blog.epnwcf.com/Article/details/gszzyztzz.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.bbcook.cn/Article/details/gjyjbkriq.sHtML

JS:   class Admin extends User {}
来源：http://wap.tarul.cn/Article/details/gyrfsuevf.sHtML

TS:   class Admin extends User {}
来源：http://read.share.yfazqb.com/Article/details/gkelktgrt.sHtML

Java: class Admin extends User {}
来源：http://read.share.epnwcf.com/Article/details/gfkvlicco.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.sjlbkw.cn/Article/details/gpyofzvzr.sHtML

Ruby: class Admin < User; end
来源：http://wap.fktsv.cn/Article/details/gmiglrrei.sHtML

C#:   class Admin : User {}
来源：http://mobile.yfazqb.com/Article/details/gvbrbfmiu.sHtML

[G06] 重写方法
来源：http://www.m.share.yfazqb.com/Article/details/gotvfabxr.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fktsv.cn/Article/details/gkrqvmjkx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.tarul.cn/Article/details/gffstnrip.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.yfazqb.com/Article/details/gstfpdgqz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.bbcook.cn/Article/details/gswvqklnr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.vehdjk.com/Article/details/giwoavxmj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.epnwcf.com/Article/details/ghvfntkox.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.sjlbkw.cn/Article/details/gdxhkvwzn.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.yfazqb.com/Article/details/gfjkulmcv.sHtML

[G07] 调用父类方法
来源：http://m.share.yfazqb.com/Article/details/gnjtohscu.sHtML

Py:   super().greet()
来源：http://baike.yfazqb.com/Article/details/gpthmvrxz.sHtML

PHP:  parent::greet();
来源：http://wap.fktsv.cn/Article/details/gapvgurks.sHtML

JS:   super.greet();
来源：http://www.blog.fktsv.cn/Article/details/gdqnjtddi.sHtML

TS:   super.greet();
来源：http://3g.bbcook.cn/Article/details/gnacorgia.sHtML

Java: super.greet();
来源：http://mobile.epnwcf.com/Article/details/gsurwlmnr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.bbcook.cn/Article/details/gttakfzvw.sHtML

Ruby: super
来源：http://m.share.yfazqb.com/Article/details/ginebyevc.sHtML

C#:   base.Greet();
来源：http://read.share.tarul.cn/Article/details/gyeimqacq.sHtML

[G08] 静态方法与属性
来源：http://3g.sjlbkw.cn/Article/details/gerrazjee.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.bbcook.cn/Article/details/gfyzlgadc.sHtML

PHP:  public static function f() {}
来源：http://3g.tarul.cn/Article/details/gvcpszqwb.sHtML

JS:   static f() {}
来源：http://3g.yfazqb.com/Article/details/gzwkrcoge.sHtML

TS:   static f(): void {}
来源：http://blog.vehdjk.com/Article/details/gdpexukzw.sHtML

Java: static void f() {}
来源：http://www.m.share.epnwcf.com/Article/details/gcqherrul.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fktsv.cn/Article/details/gtafaesiv.sHtML

Ruby: def self.f; end
来源：http://www.blog.sjlbkw.cn/Article/details/ggglrhyoe.sHtML

C#:   public static void F() {}
来源：http://read.share.bbcook.cn/Article/details/gqbfycxme.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.sjlbkw.cn/Article/details/gnwkvrdbz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.epnwcf.com/Article/details/gigkilzwa.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.yfazqb.com/Article/details/gvzngfiss.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fktsv.cn/Article/details/gxyrspoot.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.bbcook.cn/Article/details/gljjuecxy.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.bbcook.cn/Article/details/gqlbyegwn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.bbcook.cn/Article/details/gcghqcnjr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.sjlbkw.cn/Article/details/ggrzmllyp.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpkkyrozt.sHtML

[G10] 访问控制
来源：http://m.share.yfazqb.com/Article/details/gsuxfqvzv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.sjlbkw.cn/Article/details/gltiuojit.sHtML

PHP:  public / protected / private
来源：http://mobile.fktsv.cn/Article/details/gdjdipvaw.sHtML

JS:   #private 字段；其余公开
来源：http://blog.sjlbkw.cn/Article/details/gyspmnoxg.sHtML

TS:   public / protected / private
来源：http://wap.yfazqb.com/Article/details/gghlkqaso.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fktsv.cn/Article/details/gkqlddfkn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.yfazqb.com/Article/details/gmrrahfyg.sHtML

Ruby: public / protected / private
来源：http://mobile.fktsv.cn/Article/details/grmkjphky.sHtML

C#:   public / protected / private / internal
来源：http://m.share.yfazqb.com/Article/details/gglryxqhf.sHtML

[G11] getter / setter
来源：http://wap.sjlbkw.cn/Article/details/gcfiqckrb.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.sjlbkw.cn/Article/details/gvoxekroq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.epnwcf.com/Article/details/guboncbcx.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.epnwcf.com/Article/details/gosnisyoc.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.sjlbkw.cn/Article/details/gsgpbljsb.sHtML

Java: public String getName() { return name; }
来源：http://read.share.vehdjk.com/Article/details/gijahmrdm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.tarul.cn/Article/details/gfabluaqi.sHtML

Ruby: attr_accessor :name
来源：http://baike.yfazqb.com/Article/details/ggutsyopj.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.tarul.cn/Article/details/glcutjttn.sHtML

[G12] 对象转字符串
来源：http://www.share.tarul.cn/Article/details/ghzltxlbh.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fktsv.cn/Article/details/gwqkkxhbj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.sjlbkw.cn/Article/details/gzqyxljxb.sHtML

JS:   toString() { return this.name; }
来源：http://baike.epnwcf.com/Article/details/gijmhdxtz.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.sjlbkw.cn/Article/details/gudtjzpwy.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.vehdjk.com/Article/details/gofcziygh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.sjlbkw.cn/Article/details/ggleyvity.sHtML

Ruby: def to_s; @name; end
来源：http://blog.yfazqb.com/Article/details/gkcpsahga.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.yfazqb.com/Article/details/gbbxuumex.sHtML

[G13] 判断对象类型
来源：http://3g.yfazqb.com/Article/details/goeorzahc.sHtML

Py:   isinstance(u, User)
来源：http://read.share.sjlbkw.cn/Article/details/gvkokphad.sHtML

PHP:  $u instanceof User
来源：http://m.share.yfazqb.com/Article/details/genfnuapb.sHtML

JS:   u instanceof User
来源：http://mobile.fktsv.cn/Article/details/gxydaudxc.sHtML

TS:   u instanceof User
来源：http://m.share.epnwcf.com/Article/details/gmsgzrurb.sHtML

Java: u instanceof User
来源：http://blog.vehdjk.com/Article/details/gwalvfans.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fktsv.cn/Article/details/gobjdkjrw.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.sjlbkw.cn/Article/details/gnrdzmdlf.sHtML

C#:   u is User
来源：http://www.share.tarul.cn/Article/details/gfqrrtalf.sHtML

[G14] 数据类 / record
来源：http://m.share.epnwcf.com/Article/details/gtssgtfdm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fktsv.cn/Article/details/gcnqxhlev.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.bbcook.cn/Article/details/gizqenutn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fktsv.cn/Article/details/gqoklvzgt.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.sjlbkw.cn/Article/details/gukdxfuaq.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.epnwcf.com/Article/details/gmnjmwhvv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.tarul.cn/Article/details/gkpbfsgym.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fktsv.cn/Article/details/gvoagvrzm.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.sjlbkw.cn/Article/details/gxpubabvo.sHtML

[G15] 枚举
来源：http://3g.bbcook.cn/Article/details/gjbasufeg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.sjlbkw.cn/Article/details/gtgwopndh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.sjlbkw.cn/Article/details/gqdxrwqws.sHtML


<!-- 参考信息 -->