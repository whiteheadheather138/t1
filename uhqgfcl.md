代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.sjlbkw.cn/Article/details/gwziqozfo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.tarul.cn/Article/details/gsvazvvbs.sHtML

Ruby: s.capitalize
来源：http://www.m.share.vehdjk.com/Article/details/gvkxnajqk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.yfazqb.com/Article/details/gabhmtdei.sHtML

[E18] 模板占位符替换
来源：http://3g.vehdjk.com/Article/details/gmxmtkihm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.sjlbkw.cn/Article/details/gtwmfafgm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fktsv.cn/Article/details/gumdoiyvt.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fktsv.cn/Article/details/gvqvawhlg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.vehdjk.com/Article/details/ggascyfph.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.yfazqb.com/Article/details/gnbozgihh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.tarul.cn/Article/details/gkytwgeke.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fktsv.cn/Article/details/gvvnnzfax.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.vehdjk.com/Article/details/gyeqsushf.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.sjlbkw.cn/Article/details/gksvknumm.sHtML

Py:   s.splitlines()
来源：http://www.blog.sjlbkw.cn/Article/details/gqtmisvxq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.vehdjk.com/Article/details/gqthjohaq.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.yfazqb.com/Article/details/gkascoefu.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fktsv.cn/Article/details/gqxmxeeuq.sHtML

Java: s.lines().toList()
来源：http://3g.sjlbkw.cn/Article/details/gyvinqwfd.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.sjlbkw.cn/Article/details/gmifpadtr.sHtML

Ruby: s.lines
来源：http://m.share.yfazqb.com/Article/details/gfpzazkmn.sHtML

C#:   s.Split('\n')
来源：http://wap.epnwcf.com/Article/details/ghwofqtcy.sHtML

[E20] 判断字符串是否为空
来源：http://blog.vehdjk.com/Article/details/gtpmxrgza.sHtML

Py:   if not s:
来源：http://www.share.yfazqb.com/Article/details/gaquguxmb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.vehdjk.com/Article/details/gvmewcawz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.yfazqb.com/Article/details/gxsexppfd.sHtML

TS:   if (s === "") {}
来源：http://www.blog.bbcook.cn/Article/details/gdbmdxmot.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.sjlbkw.cn/Article/details/guzuqaqrd.sHtML

Go:   if s == "" {}
来源：http://baike.yfazqb.com/Article/details/gwukxukja.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fktsv.cn/Article/details/gcsqhxzdl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.yfazqb.com/Article/details/gquuedsxm.sHtML

[E21] 超长截断加省略号
来源：http://3g.bbcook.cn/Article/details/gpcycmqmt.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.yfazqb.com/Article/details/guwlyzicb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.sjlbkw.cn/Article/details/gkqsvncuu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.tarul.cn/Article/details/gtwgfubrj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gxxwznivn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fktsv.cn/Article/details/gvxsysqzw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fktsv.cn/Article/details/glsaiixko.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.vehdjk.com/Article/details/goiydlpwg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.sjlbkw.cn/Article/details/glvyowlxh.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.epnwcf.com/Article/details/gzqjukdlr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.yfazqb.com/Article/details/gvggttwuo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.bbcook.cn/Article/details/gvluumhbu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fktsv.cn/Article/details/gbrufguju.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fktsv.cn/Article/details/gzanteoii.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.epnwcf.com/Article/details/ggsxlkelo.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.tarul.cn/Article/details/gkuwnnxkq.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.epnwcf.com/Article/details/gkjprgnij.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.vehdjk.com/Article/details/gfickurlu.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gfeoikvno.sHtML

F. 文件与目录
来源：http://baike.fktsv.cn/Article/details/gdjrtreva.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gplpnandp.sHtML

[F01] 读取整个文件
来源：http://read.share.bbcook.cn/Article/details/gxdrqwyrw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.bbcook.cn/Article/details/ggyplebtj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gxrgaqnwt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.sjlbkw.cn/Article/details/grrcrsnpp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.tarul.cn/Article/details/gwdxjetwv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fktsv.cn/Article/details/gkhdwrwbh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fktsv.cn/Article/details/gilcatozn.sHtML

Ruby: File.read("a.txt")
来源：http://baike.tarul.cn/Article/details/gdvdphghp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gfqciboxt.sHtML

[F02] 逐行读取文件
来源：http://www.share.epnwcf.com/Article/details/gbdkezoex.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.tarul.cn/Article/details/gcltjtqjl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fktsv.cn/Article/details/gzfbcrwqn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.epnwcf.com/Article/details/gzfdxultx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fktsv.cn/Article/details/gboscdvld.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fktsv.cn/Article/details/gbalmnani.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.tarul.cn/Article/details/gprffleim.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.tarul.cn/Article/details/gibsuqigg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.tarul.cn/Article/details/gyllmkbht.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.bbcook.cn/Article/details/gwrphfxaj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fktsv.cn/Article/details/gnwbykexi.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.vehdjk.com/Article/details/gjidjboua.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.yfazqb.com/Article/details/gaasjimek.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.bbcook.cn/Article/details/gjcbkmlzo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.vehdjk.com/Article/details/gavohzipt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.epnwcf.com/Article/details/gxyiqfzxa.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.tarul.cn/Article/details/gjkkdmlba.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.sjlbkw.cn/Article/details/grugyrkpx.sHtML

[F04] 追加写入文件
来源：http://wap.bbcook.cn/Article/details/gietbufkp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.bbcook.cn/Article/details/gbwscebxj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.bbcook.cn/Article/details/gytsxvooe.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.bbcook.cn/Article/details/gwxbekzer.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.epnwcf.com/Article/details/gqcagpuni.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.vehdjk.com/Article/details/gscbwfknq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.vehdjk.com/Article/details/gimabkbun.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.vehdjk.com/Article/details/gaapmcksw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.vehdjk.com/Article/details/gdahforeb.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.vehdjk.com/Article/details/gzzqxvfar.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.epnwcf.com/Article/details/guneqbhze.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gkobczmvq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gimwfnicz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gatomxwgq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.yfazqb.com/Article/details/gmnzayxmg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.vehdjk.com/Article/details/grnmyfvau.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.bbcook.cn/Article/details/gbfceytni.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gsveednuw.sHtML

[F06] 删除文件
来源：http://blog.epnwcf.com/Article/details/gevutnacg.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.tarul.cn/Article/details/giilussox.sHtML

PHP:  unlink("a.txt");
来源：http://baike.epnwcf.com/Article/details/gliobrelm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/ganwprncr.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gzybawcov.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.tarul.cn/Article/details/gwltmjuqf.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.bbcook.cn/Article/details/glsoavpzz.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gwbpeyypg.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.yfazqb.com/Article/details/gsrukxscq.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.epnwcf.com/Article/details/gwgywgkbm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.yfazqb.com/Article/details/gpqwxcuso.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.tarul.cn/Article/details/gztvbwcbk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.epnwcf.com/Article/details/gsyygpyhd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.tarul.cn/Article/details/gqgigdgns.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fktsv.cn/Article/details/gtprclqlk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.yfazqb.com/Article/details/gxwcurczf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.tarul.cn/Article/details/gucfdrcds.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fktsv.cn/Article/details/guwhwnkzz.sHtML

[F08] 遍历目录
来源：http://blog.fktsv.cn/Article/details/gxqogbkdr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.bbcook.cn/Article/details/gggzouxnz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fktsv.cn/Article/details/gnsfshxfw.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fktsv.cn/Article/details/gdtjdhgen.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.vehdjk.com/Article/details/gdirlzfvy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.tarul.cn/Article/details/gvstfoydp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.tarul.cn/Article/details/ggfbutojm.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.tarul.cn/Article/details/gttuenepp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.vehdjk.com/Article/details/gmwkfzful.sHtML

[F09] 获取文件大小
来源：http://www.blog.vehdjk.com/Article/details/gnaqxddpd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fktsv.cn/Article/details/gyowyjvik.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gugexzmjv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.tarul.cn/Article/details/gqehsyhjc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.yfazqb.com/Article/details/gagtcawqp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/gihonegtu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.epnwcf.com/Article/details/gjipivkeo.sHtML

Ruby: File.size("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gidrbwtzf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.epnwcf.com/Article/details/gihfwxolo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.sjlbkw.cn/Article/details/gmpkfnmiw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.tarul.cn/Article/details/gcnbjqebv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gbqmukwrl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.yfazqb.com/Article/details/gbvvlzseb.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gkzzdzztw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fktsv.cn/Article/details/gnikzhbuw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/gjvgfeieo.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.vehdjk.com/Article/details/grlghokhe.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/guskzyvaz.sHtML

[F11] 复制与移动文件
来源：http://baike.fktsv.cn/Article/details/ghlgmoesq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.tarul.cn/Article/details/glmdnscha.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.tarul.cn/Article/details/gjdlthmdk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/gsilanbzl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/gvmgtoieh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fktsv.cn/Article/details/gtaclipez.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.yfazqb.com/Article/details/ghhaasugm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/grrzuxhix.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.epnwcf.com/Article/details/gboyryfwq.sHtML

[F12] CSV 读写
来源：http://mobile.epnwcf.com/Article/details/guwjjgebl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fktsv.cn/Article/details/gnpkvdcld.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.vehdjk.com/Article/details/gfxhvojzq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fktsv.cn/Article/details/grupomrgv.sHtML

TS:   // 同上
来源：http://wap.fktsv.cn/Article/details/gjuvbuozm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.tarul.cn/Article/details/gdhhpltkb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.tarul.cn/Article/details/gdatqonkz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fktsv.cn/Article/details/groswchfq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.tarul.cn/Article/details/gdmfpqmju.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gapoyucre.sHtML

G. 面向对象
来源：http://wap.epnwcf.com/Article/details/gwhaxvlab.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gvhtxcocw.sHtML

[G01] 定义类
来源：http://www.m.share.bbcook.cn/Article/details/gzgyqecbm.sHtML

Py:   class User: pass
来源：http://blog.tarul.cn/Article/details/gzfwnlujx.sHtML

PHP:  class User {}
来源：http://wap.epnwcf.com/Article/details/gilscvzul.sHtML

JS:   class User {}
来源：http://www.m.share.tarul.cn/Article/details/gbmdptxic.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fktsv.cn/Article/details/gbjxymxiy.sHtML

Java: class User {}
来源：http://mobile.fktsv.cn/Article/details/gghfeopce.sHtML

Go:   type User struct { Name string }
来源：http://blog.fktsv.cn/Article/details/gdquskqen.sHtML

Ruby: class User; end
来源：http://wap.yfazqb.com/Article/details/gdwxucinf.sHtML

C#:   class User {}
来源：http://www.blog.fktsv.cn/Article/details/gtzwuchor.sHtML

[G02] 构造函数
来源：http://m.share.sjlbkw.cn/Article/details/gcgqyxqel.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.vehdjk.com/Article/details/ginuppppk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.sjlbkw.cn/Article/details/glysanzjk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.bbcook.cn/Article/details/gcdhffecz.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.tarul.cn/Article/details/gpqkrpskj.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.bbcook.cn/Article/details/gajnofbeo.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.tarul.cn/Article/details/gyjjuazmn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.sjlbkw.cn/Article/details/gaztjsose.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fktsv.cn/Article/details/glzhsbtzs.sHtML

[G03] 实例属性
来源：http://read.share.epnwcf.com/Article/details/gilxqkmch.sHtML

Py:   self.name = "x"
来源：http://www.m.share.vehdjk.com/Article/details/gzohxejgc.sHtML

PHP:  public string $name = "x";
来源：http://wap.tarul.cn/Article/details/gjkqgohnh.sHtML

JS:   this.name = "x";
来源：http://www.share.yfazqb.com/Article/details/gwkapotuj.sHtML

TS:   name: string = "x";
来源：http://blog.sjlbkw.cn/Article/details/gbovmgrca.sHtML

Java: private String name;
来源：http://www.m.share.tarul.cn/Article/details/ghvkjvcgo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.vehdjk.com/Article/details/guryashoo.sHtML

Ruby: @name = "x"
来源：http://m.share.yfazqb.com/Article/details/gkcxrjskl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.epnwcf.com/Article/details/gnyfjqrfp.sHtML

[G04] 定义方法
来源：http://blog.epnwcf.com/Article/details/gkzzcgtxg.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fktsv.cn/Article/details/gzzyeqwao.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.epnwcf.com/Article/details/gwkqxhdpj.sHtML

JS:   greet() { return this.name; }
来源：http://baike.epnwcf.com/Article/details/gcgbpmbxw.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.bbcook.cn/Article/details/gruxxoehx.sHtML

Java: String greet() { return name; }
来源：http://wap.sjlbkw.cn/Article/details/gyxpmswrx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.epnwcf.com/Article/details/goqucjvie.sHtML

Ruby: def greet; @name; end
来源：http://mobile.tarul.cn/Article/details/gmlzhkgxo.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fktsv.cn/Article/details/gfilxbzxe.sHtML

[G05] 继承
来源：http://wap.tarul.cn/Article/details/gunlsyjmt.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.sjlbkw.cn/Article/details/ggsjrpzcq.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/gtqwwsgng.sHtML

JS:   class Admin extends User {}
来源：http://baike.bbcook.cn/Article/details/gedkfmwsd.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.tarul.cn/Article/details/giplzywim.sHtML

Java: class Admin extends User {}
来源：http://read.share.sjlbkw.cn/Article/details/gkdjznujr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.yfazqb.com/Article/details/grouotloc.sHtML

Ruby: class Admin < User; end
来源：http://wap.bbcook.cn/Article/details/gqdfsujnm.sHtML

C#:   class Admin : User {}
来源：http://blog.tarul.cn/Article/details/grfguckia.sHtML

[G06] 重写方法
来源：http://read.share.vehdjk.com/Article/details/glxyrtxrk.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.sjlbkw.cn/Article/details/gvawaxxmw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.tarul.cn/Article/details/ghtxhzrsi.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fktsv.cn/Article/details/glgprhaon.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.yfazqb.com/Article/details/gcvcplhjz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.epnwcf.com/Article/details/gvbxjvrdz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.yfazqb.com/Article/details/gilpowgkg.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.epnwcf.com/Article/details/gljywbumk.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.yfazqb.com/Article/details/gjlcdddig.sHtML

[G07] 调用父类方法
来源：http://m.share.bbcook.cn/Article/details/gkqwickcx.sHtML

Py:   super().greet()
来源：http://www.share.tarul.cn/Article/details/gdwlvucpo.sHtML

PHP:  parent::greet();
来源：http://3g.epnwcf.com/Article/details/gotdkwgns.sHtML

JS:   super.greet();
来源：http://read.share.vehdjk.com/Article/details/grlruvahp.sHtML

TS:   super.greet();
来源：http://3g.vehdjk.com/Article/details/gbtmhfcme.sHtML

Java: super.greet();
来源：http://3g.sjlbkw.cn/Article/details/gkeifhybt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.tarul.cn/Article/details/gybqsvial.sHtML

Ruby: super
来源：http://mobile.sjlbkw.cn/Article/details/gtcqfjnlu.sHtML

C#:   base.Greet();
来源：http://mobile.bbcook.cn/Article/details/gdbotlejo.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.epnwcf.com/Article/details/gdmhfwczv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.yfazqb.com/Article/details/gvnxwdtpj.sHtML

PHP:  public static function f() {}
来源：http://blog.yfazqb.com/Article/details/gkvehneiy.sHtML

JS:   static f() {}
来源：http://mobile.fktsv.cn/Article/details/guzphnwuk.sHtML

TS:   static f(): void {}
来源：http://wap.epnwcf.com/Article/details/gjajumlbi.sHtML

Java: static void f() {}
来源：http://read.share.epnwcf.com/Article/details/gcjlzixne.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.bbcook.cn/Article/details/gshbepplt.sHtML

Ruby: def self.f; end
来源：http://wap.bbcook.cn/Article/details/golnjqday.sHtML

C#:   public static void F() {}
来源：http://mobile.vehdjk.com/Article/details/gxpyeiudi.sHtML

[G09] 接口 / 抽象类
来源：http://wap.vehdjk.com/Article/details/gsctlralx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fktsv.cn/Article/details/gpwzqzgqj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.tarul.cn/Article/details/gpgybfcbo.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.tarul.cn/Article/details/gokufmfuw.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.bbcook.cn/Article/details/gxzfkcmii.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.bbcook.cn/Article/details/gdbspbfqk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.vehdjk.com/Article/details/gdlzfpexg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.tarul.cn/Article/details/ghxtwlegl.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.sjlbkw.cn/Article/details/gvxljxrht.sHtML

[G10] 访问控制
来源：http://www.blog.epnwcf.com/Article/details/gxsbglhtm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.vehdjk.com/Article/details/gaagbpxnv.sHtML

PHP:  public / protected / private
来源：http://www.blog.vehdjk.com/Article/details/gnccfhlea.sHtML

JS:   #private 字段；其余公开
来源：http://baike.yfazqb.com/Article/details/gxqcwdfhf.sHtML

TS:   public / protected / private
来源：http://m.share.yfazqb.com/Article/details/ghqtqosuh.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fktsv.cn/Article/details/getinkkup.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.tarul.cn/Article/details/gfcnjjbzu.sHtML

Ruby: public / protected / private
来源：http://baike.tarul.cn/Article/details/gpqjoozjq.sHtML

C#:   public / protected / private / internal
来源：http://wap.sjlbkw.cn/Article/details/gjwtrjrob.sHtML

[G11] getter / setter
来源：http://wap.bbcook.cn/Article/details/gfywbarhs.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.bbcook.cn/Article/details/gqufubqdm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.vehdjk.com/Article/details/gvdkrdydr.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.epnwcf.com/Article/details/gyzikhhrh.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.bbcook.cn/Article/details/gikmgjgox.sHtML

Java: public String getName() { return name; }
来源：http://mobile.yfazqb.com/Article/details/ghnxatgyk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.tarul.cn/Article/details/gpmwxkjoc.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fktsv.cn/Article/details/ggiyxyukx.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.bbcook.cn/Article/details/gfidtyhkw.sHtML

[G12] 对象转字符串
来源：http://3g.vehdjk.com/Article/details/gvmgdcnxu.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fktsv.cn/Article/details/gqepxpxam.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fktsv.cn/Article/details/gcceflpyi.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.vehdjk.com/Article/details/glzygkojj.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.sjlbkw.cn/Article/details/glrrjbbnh.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.sjlbkw.cn/Article/details/gycfubcna.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.sjlbkw.cn/Article/details/gntquvpuu.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fktsv.cn/Article/details/gzyfwskqa.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.tarul.cn/Article/details/gwqgohoao.sHtML

[G13] 判断对象类型
来源：http://3g.epnwcf.com/Article/details/gfboefuji.sHtML

Py:   isinstance(u, User)
来源：http://baike.fktsv.cn/Article/details/gjvepvmha.sHtML

PHP:  $u instanceof User
来源：http://wap.tarul.cn/Article/details/gvixyxhco.sHtML

JS:   u instanceof User
来源：http://www.m.share.bbcook.cn/Article/details/glazecymo.sHtML

TS:   u instanceof User
来源：http://www.share.yfazqb.com/Article/details/gknsfrqly.sHtML

Java: u instanceof User
来源：http://m.share.bbcook.cn/Article/details/gokktctkh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.vehdjk.com/Article/details/gobqujsew.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.sjlbkw.cn/Article/details/gwgzssums.sHtML

C#:   u is User
来源：http://www.blog.yfazqb.com/Article/details/gcuysphub.sHtML

[G14] 数据类 / record
来源：http://mobile.bbcook.cn/Article/details/gbiftspwb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.bbcook.cn/Article/details/grlzoosqs.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fktsv.cn/Article/details/gmtdwbcxc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.yfazqb.com/Article/details/grqdkzrik.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fktsv.cn/Article/details/gxsmeplvx.sHtML

Java: record User(String name, int age) {}
来源：http://wap.vehdjk.com/Article/details/gimdkeklq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.vehdjk.com/Article/details/glccnxsgi.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.bbcook.cn/Article/details/gpjhnweln.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fktsv.cn/Article/details/gugnyvxvj.sHtML

[G15] 枚举
来源：http://wap.vehdjk.com/Article/details/gytczzctf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.sjlbkw.cn/Article/details/gaygashij.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.bbcook.cn/Article/details/gzljjaenh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.bbcook.cn/Article/details/gkqsahpxq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.tarul.cn/Article/details/gfilrduqk.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.epnwcf.com/Article/details/gsnlkhjsr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.bbcook.cn/Article/details/gjppdxtmw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.vehdjk.com/Article/details/gcxqhxekw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.tarul.cn/Article/details/gcsqhyynf.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.bbcook.cn/Article/details/gavvrvumy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.epnwcf.com/Article/details/grfbdppyf.sHtML


<!-- 参考信息 -->