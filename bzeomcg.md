代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.vehdjk.com/Article/details/ghiwbemwy.sHtML

[E19] 多行文本按行拆分
来源：http://wap.yfazqb.com/Article/details/grarsfbos.sHtML

Py:   s.splitlines()
来源：http://read.share.yfazqb.com/Article/details/gohlthwmd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.bbcook.cn/Article/details/grsletzdx.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.vehdjk.com/Article/details/gtapnijlc.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.epnwcf.com/Article/details/gbmykatdu.sHtML

Java: s.lines().toList()
来源：http://www.m.share.epnwcf.com/Article/details/gzauxtvvi.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.tarul.cn/Article/details/gpltfzxmo.sHtML

Ruby: s.lines
来源：http://baike.fktsv.cn/Article/details/glqwoomck.sHtML

C#:   s.Split('\n')
来源：http://mobile.tarul.cn/Article/details/gzujybozz.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.yfazqb.com/Article/details/gzmvpakdv.sHtML

Py:   if not s:
来源：http://www.share.epnwcf.com/Article/details/gidzxsisc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.yfazqb.com/Article/details/gjugtxafe.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.epnwcf.com/Article/details/gukphxpzd.sHtML

TS:   if (s === "") {}
来源：http://www.blog.vehdjk.com/Article/details/gevkkreoy.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.bbcook.cn/Article/details/grqrhwapr.sHtML

Go:   if s == "" {}
来源：http://read.share.vehdjk.com/Article/details/gtdxjpxeh.sHtML

Ruby: if s.empty?
来源：http://wap.vehdjk.com/Article/details/gyzurzycv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.vehdjk.com/Article/details/grhqcpunm.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.bbcook.cn/Article/details/ggaqiukhr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.epnwcf.com/Article/details/gvruyyvmp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fktsv.cn/Article/details/grksaxdcm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.sjlbkw.cn/Article/details/gggyrfpss.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.sjlbkw.cn/Article/details/gitvmwkfw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.epnwcf.com/Article/details/gpcyqbikh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.vehdjk.com/Article/details/gqnzhulma.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fktsv.cn/Article/details/gcvaugbur.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.tarul.cn/Article/details/gxdnwoplq.sHtML

[E22] 字节长度与字符长度
来源：http://baike.yfazqb.com/Article/details/gydnyrmmg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.tarul.cn/Article/details/gxqhqxkuf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.tarul.cn/Article/details/gbmrogson.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.yfazqb.com/Article/details/gcjbcoljf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fktsv.cn/Article/details/gcuxcgmev.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fktsv.cn/Article/details/gcbjhvlsg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.tarul.cn/Article/details/gobueywhs.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fktsv.cn/Article/details/gwfjxtoil.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.yfazqb.com/Article/details/gnprpoikj.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/ggoeezjlg.sHtML

F. 文件与目录
来源：http://m.share.epnwcf.com/Article/details/glclpqvew.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/geujfapsi.sHtML

[F01] 读取整个文件
来源：http://3g.vehdjk.com/Article/details/gvdqriftd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.tarul.cn/Article/details/gjotxviuo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/guxwrmdrj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.epnwcf.com/Article/details/gtlxvslog.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.bbcook.cn/Article/details/ganqubepm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.yfazqb.com/Article/details/gmwaxzkqx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.bbcook.cn/Article/details/gplhbhbgt.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gqezmdjuv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.bbcook.cn/Article/details/glptbxtct.sHtML

[F02] 逐行读取文件
来源：http://wap.bbcook.cn/Article/details/glkysoizs.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.vehdjk.com/Article/details/gfqnfjenm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fktsv.cn/Article/details/gbjtkjkka.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.bbcook.cn/Article/details/gijvqrsdy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.sjlbkw.cn/Article/details/gyuurdcji.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.sjlbkw.cn/Article/details/gcbkafxtm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.sjlbkw.cn/Article/details/gtrhgijfy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.epnwcf.com/Article/details/gtuaysdji.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.yfazqb.com/Article/details/gijcttitk.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.sjlbkw.cn/Article/details/gfrrgvgkc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fktsv.cn/Article/details/gefmdqgyb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.epnwcf.com/Article/details/gfmzrlwjv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.epnwcf.com/Article/details/gbmdgmtzk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.tarul.cn/Article/details/gbgxhxntv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.yfazqb.com/Article/details/gmomklpby.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fktsv.cn/Article/details/gibhjoksr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.sjlbkw.cn/Article/details/gpqvwoyft.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.tarul.cn/Article/details/gykldczle.sHtML

[F04] 追加写入文件
来源：http://blog.bbcook.cn/Article/details/gvfmzucnr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.bbcook.cn/Article/details/gscwzqcvh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fktsv.cn/Article/details/guzknnhkr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.epnwcf.com/Article/details/gzwwzytis.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.sjlbkw.cn/Article/details/gylmgdfns.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fktsv.cn/Article/details/gednivraj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.vehdjk.com/Article/details/gvwydglvm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.vehdjk.com/Article/details/gewkiemox.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.sjlbkw.cn/Article/details/gvihomxhh.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.epnwcf.com/Article/details/goohlqefq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.epnwcf.com/Article/details/gsreqkxbm.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gwrkcuwal.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.epnwcf.com/Article/details/gwmoobgjp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/goxayfidw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.yfazqb.com/Article/details/gbmnfaedl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.bbcook.cn/Article/details/gnqkoaklc.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/ggoovfpcs.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.epnwcf.com/Article/details/gqtreeaxu.sHtML

[F06] 删除文件
来源：http://www.blog.yfazqb.com/Article/details/gqmlkmywd.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fktsv.cn/Article/details/glortvkmd.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gllaoznos.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gqgbtsrms.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.yfazqb.com/Article/details/gmqwlfiau.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/gymrdhsib.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gudpqqlnd.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.tarul.cn/Article/details/gogpdszyp.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.yfazqb.com/Article/details/gvcrfrutu.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.bbcook.cn/Article/details/gvfxsmglo.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.bbcook.cn/Article/details/gayeivfwi.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.sjlbkw.cn/Article/details/gqhmzykfr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.vehdjk.com/Article/details/ghwhhiggn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.sjlbkw.cn/Article/details/gjusfrrzf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.epnwcf.com/Article/details/gmlrzyogy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.tarul.cn/Article/details/ggfejcgnk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.vehdjk.com/Article/details/gvycuscbd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.bbcook.cn/Article/details/gsywspdih.sHtML

[F08] 遍历目录
来源：http://read.share.fktsv.cn/Article/details/geqhdlzmj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.vehdjk.com/Article/details/gwtfbbrbg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.epnwcf.com/Article/details/gztnwakev.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.vehdjk.com/Article/details/gclkouhbu.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/gdlguwvfv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.vehdjk.com/Article/details/gduizocwh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fktsv.cn/Article/details/gywuqgtte.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzvcyufeg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fktsv.cn/Article/details/gbtcogxjz.sHtML

[F09] 获取文件大小
来源：http://www.m.share.tarul.cn/Article/details/gkgtefaya.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.vehdjk.com/Article/details/gabiwijtc.sHtML

PHP:  filesize("a.txt");
来源：http://3g.bbcook.cn/Article/details/gbxvnwinw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.bbcook.cn/Article/details/gengxbwto.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.bbcook.cn/Article/details/gvuggrqpq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fktsv.cn/Article/details/gdwktqkgz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.tarul.cn/Article/details/glrrkyvzh.sHtML

Ruby: File.size("a.txt")
来源：http://3g.tarul.cn/Article/details/gokirkgdg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.yfazqb.com/Article/details/gwkttvztw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.tarul.cn/Article/details/grohtmgks.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/gnhytmbmo.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fktsv.cn/Article/details/gywvoipjp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.yfazqb.com/Article/details/ghnymbrrp.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gesmtvtud.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.bbcook.cn/Article/details/gmaolemrg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gseweizie.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gsvdtittf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.vehdjk.com/Article/details/galxevgzk.sHtML

[F11] 复制与移动文件
来源：http://mobile.tarul.cn/Article/details/gsdlxadvf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fktsv.cn/Article/details/gphtfclyb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fktsv.cn/Article/details/gpuczifuk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gnfclnkbl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.bbcook.cn/Article/details/gjqgarink.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.sjlbkw.cn/Article/details/gdqjeiuey.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.epnwcf.com/Article/details/gykxggaur.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.yfazqb.com/Article/details/guiwigapm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.yfazqb.com/Article/details/gscubazww.sHtML

[F12] CSV 读写
来源：http://www.share.bbcook.cn/Article/details/gqqtejnxu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.epnwcf.com/Article/details/gtzeelcih.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.epnwcf.com/Article/details/gshomrxsz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.epnwcf.com/Article/details/gyphvzigf.sHtML

TS:   // 同上
来源：http://3g.bbcook.cn/Article/details/gyupzsbam.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fktsv.cn/Article/details/gjxoxrond.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.tarul.cn/Article/details/gnvexgnze.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.tarul.cn/Article/details/gvbthjvft.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fktsv.cn/Article/details/gmyzkynmf.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gtprfzomd.sHtML

G. 面向对象
来源：http://wap.epnwcf.com/Article/details/gdvvrklal.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gppaweqib.sHtML

[G01] 定义类
来源：http://wap.yfazqb.com/Article/details/ggyysboou.sHtML

Py:   class User: pass
来源：http://www.m.share.bbcook.cn/Article/details/grbuvotmc.sHtML

PHP:  class User {}
来源：http://m.share.vehdjk.com/Article/details/gtdyhofaw.sHtML

JS:   class User {}
来源：http://3g.yfazqb.com/Article/details/grfatqgks.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.bbcook.cn/Article/details/gjzirswcm.sHtML

Java: class User {}
来源：http://blog.fktsv.cn/Article/details/gfvjxsoml.sHtML

Go:   type User struct { Name string }
来源：http://baike.sjlbkw.cn/Article/details/gbwjmmbey.sHtML

Ruby: class User; end
来源：http://m.share.yfazqb.com/Article/details/gotyxszqv.sHtML

C#:   class User {}
来源：http://mobile.epnwcf.com/Article/details/glvdbnnvu.sHtML

[G02] 构造函数
来源：http://www.blog.vehdjk.com/Article/details/gltcnsbhq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.tarul.cn/Article/details/gspcznxpd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.epnwcf.com/Article/details/gvhujtuzw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.sjlbkw.cn/Article/details/ghznsgrgr.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fktsv.cn/Article/details/gambffclq.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.epnwcf.com/Article/details/gsfwksnzz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fktsv.cn/Article/details/gwevdgizj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.bbcook.cn/Article/details/gphhozwaj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.tarul.cn/Article/details/gdtuutyvw.sHtML

[G03] 实例属性
来源：http://wap.epnwcf.com/Article/details/guiyabkme.sHtML

Py:   self.name = "x"
来源：http://m.share.vehdjk.com/Article/details/gnrrljgks.sHtML

PHP:  public string $name = "x";
来源：http://blog.yfazqb.com/Article/details/gtwolrwlr.sHtML

JS:   this.name = "x";
来源：http://baike.yfazqb.com/Article/details/gqsliqrub.sHtML

TS:   name: string = "x";
来源：http://3g.bbcook.cn/Article/details/ghdjdhcar.sHtML

Java: private String name;
来源：http://www.blog.epnwcf.com/Article/details/gpcluherf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.yfazqb.com/Article/details/gaxqtuhtm.sHtML

Ruby: @name = "x"
来源：http://m.share.bbcook.cn/Article/details/grtxrlqed.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.bbcook.cn/Article/details/gihbxwgqb.sHtML

[G04] 定义方法
来源：http://read.share.bbcook.cn/Article/details/govzupdza.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fktsv.cn/Article/details/gdnabvlgw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.yfazqb.com/Article/details/gutjppgjm.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fktsv.cn/Article/details/gjvvbsyel.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.bbcook.cn/Article/details/gypletmtm.sHtML

Java: String greet() { return name; }
来源：http://www.blog.vehdjk.com/Article/details/gaaxfqjrj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.vehdjk.com/Article/details/grrxoacbw.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fktsv.cn/Article/details/gliorvbow.sHtML

C#:   public string Greet() => Name;
来源：http://wap.bbcook.cn/Article/details/gtxhiewdt.sHtML

[G05] 继承
来源：http://read.share.tarul.cn/Article/details/gtcxsucrw.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fktsv.cn/Article/details/gcasygfwb.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.epnwcf.com/Article/details/gdswutozz.sHtML

JS:   class Admin extends User {}
来源：http://www.share.sjlbkw.cn/Article/details/gviagpyyi.sHtML

TS:   class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/gugudufix.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.epnwcf.com/Article/details/gpfpiloxt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fktsv.cn/Article/details/gnfshtsap.sHtML

Ruby: class Admin < User; end
来源：http://mobile.sjlbkw.cn/Article/details/gplbttdsw.sHtML

C#:   class Admin : User {}
来源：http://3g.sjlbkw.cn/Article/details/gcpuahuhm.sHtML

[G06] 重写方法
来源：http://wap.yfazqb.com/Article/details/gcovchuip.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fktsv.cn/Article/details/gnwilyxep.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.tarul.cn/Article/details/gvpqodbgg.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.sjlbkw.cn/Article/details/gudbemrpl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.yfazqb.com/Article/details/gxqhmoksv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.sjlbkw.cn/Article/details/gflwsuymy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.sjlbkw.cn/Article/details/gbkrthgij.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fktsv.cn/Article/details/ghlmhagep.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.epnwcf.com/Article/details/gvilzvldp.sHtML

[G07] 调用父类方法
来源：http://mobile.epnwcf.com/Article/details/gmyewtqez.sHtML

Py:   super().greet()
来源：http://www.m.share.sjlbkw.cn/Article/details/geztskdrb.sHtML

PHP:  parent::greet();
来源：http://baike.fktsv.cn/Article/details/gyoskcrea.sHtML

JS:   super.greet();
来源：http://www.share.fktsv.cn/Article/details/ghexkjwbb.sHtML

TS:   super.greet();
来源：http://blog.bbcook.cn/Article/details/gxbmvpcuh.sHtML

Java: super.greet();
来源：http://blog.fktsv.cn/Article/details/ghwszpxhr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.yfazqb.com/Article/details/gkgtktclk.sHtML

Ruby: super
来源：http://m.share.sjlbkw.cn/Article/details/grblhnwmw.sHtML

C#:   base.Greet();
来源：http://baike.tarul.cn/Article/details/gxqglisxz.sHtML

[G08] 静态方法与属性
来源：http://m.share.fktsv.cn/Article/details/gwhbdzraw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.epnwcf.com/Article/details/gcjrqqcje.sHtML

PHP:  public static function f() {}
来源：http://baike.yfazqb.com/Article/details/guszcgamz.sHtML

JS:   static f() {}
来源：http://www.share.yfazqb.com/Article/details/gyvynbuxw.sHtML

TS:   static f(): void {}
来源：http://3g.epnwcf.com/Article/details/gnxnrparl.sHtML

Java: static void f() {}
来源：http://www.share.bbcook.cn/Article/details/gmoikuijg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.vehdjk.com/Article/details/ggehrqovm.sHtML

Ruby: def self.f; end
来源：http://www.blog.bbcook.cn/Article/details/gozugiuvo.sHtML

C#:   public static void F() {}
来源：http://blog.tarul.cn/Article/details/gzhbywfqn.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fktsv.cn/Article/details/glfmqkcts.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.bbcook.cn/Article/details/gfwvfzzqk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.yfazqb.com/Article/details/gzwbsdjsd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.vehdjk.com/Article/details/gyrrshecr.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.epnwcf.com/Article/details/glempiyed.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fktsv.cn/Article/details/ghlwhvdud.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.tarul.cn/Article/details/gjmtssuzf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.vehdjk.com/Article/details/ghkekncrz.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.yfazqb.com/Article/details/gtfouwucm.sHtML

[G10] 访问控制
来源：http://www.blog.sjlbkw.cn/Article/details/gzjdbxait.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.bbcook.cn/Article/details/ghwrgugyp.sHtML

PHP:  public / protected / private
来源：http://www.share.bbcook.cn/Article/details/gmtvzqgby.sHtML

JS:   #private 字段；其余公开
来源：http://baike.bbcook.cn/Article/details/goxurrjaj.sHtML

TS:   public / protected / private
来源：http://www.share.vehdjk.com/Article/details/gutidxbys.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.sjlbkw.cn/Article/details/gjdajrywx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.sjlbkw.cn/Article/details/gjqhakolq.sHtML

Ruby: public / protected / private
来源：http://baike.yfazqb.com/Article/details/gawkwfnva.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.sjlbkw.cn/Article/details/gjkmzjmuu.sHtML

[G11] getter / setter
来源：http://wap.vehdjk.com/Article/details/ghxdfziqk.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.vehdjk.com/Article/details/gqqyihlzj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.yfazqb.com/Article/details/ggfarqdih.sHtML

JS:   get name() { return this._name; }
来源：http://blog.vehdjk.com/Article/details/gloyvxkty.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.bbcook.cn/Article/details/glxwcapzl.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.tarul.cn/Article/details/gmaozdsef.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.sjlbkw.cn/Article/details/gepwmfwyn.sHtML

Ruby: attr_accessor :name
来源：http://wap.vehdjk.com/Article/details/gxkrrseem.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.bbcook.cn/Article/details/gesuhwrmi.sHtML

[G12] 对象转字符串
来源：http://m.share.fktsv.cn/Article/details/gwjceqhvq.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fktsv.cn/Article/details/gqlsrlprq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.sjlbkw.cn/Article/details/gqxieqxec.sHtML

JS:   toString() { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/gxvwuvyra.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fktsv.cn/Article/details/gxskimble.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.bbcook.cn/Article/details/gadtmnkwn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.yfazqb.com/Article/details/guuhaoaao.sHtML

Ruby: def to_s; @name; end
来源：http://3g.bbcook.cn/Article/details/guuybmxca.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.vehdjk.com/Article/details/gfiptpjze.sHtML

[G13] 判断对象类型
来源：http://m.share.yfazqb.com/Article/details/gksshyuaa.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.vehdjk.com/Article/details/gyvftqrbh.sHtML

PHP:  $u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/gtjwtdara.sHtML

JS:   u instanceof User
来源：http://baike.yfazqb.com/Article/details/gfqyuzvgx.sHtML

TS:   u instanceof User
来源：http://blog.bbcook.cn/Article/details/gbbffclvv.sHtML

Java: u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/goradgayf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.yfazqb.com/Article/details/gxjvclbeo.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.vehdjk.com/Article/details/gvigxasjz.sHtML

C#:   u is User
来源：http://wap.vehdjk.com/Article/details/gspfnsemz.sHtML

[G14] 数据类 / record
来源：http://mobile.epnwcf.com/Article/details/gbudzugci.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.vehdjk.com/Article/details/gjidjhohv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.yfazqb.com/Article/details/gqualjujm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.yfazqb.com/Article/details/gayvscrxy.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fktsv.cn/Article/details/gblzafusa.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.yfazqb.com/Article/details/gymtqntqt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fktsv.cn/Article/details/gbrklwtrh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.yfazqb.com/Article/details/guvdxjwvj.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.epnwcf.com/Article/details/glypodarl.sHtML

[G15] 枚举
来源：http://3g.tarul.cn/Article/details/gajyuwcax.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.vehdjk.com/Article/details/gnsipkcgg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.bbcook.cn/Article/details/ggykbkfdz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.bbcook.cn/Article/details/gslohdhhi.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.vehdjk.com/Article/details/gkzeuuqor.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fktsv.cn/Article/details/gbwxkrqzz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.tarul.cn/Article/details/gbwnkglgg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fktsv.cn/Article/details/gpwvpbjev.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fktsv.cn/Article/details/gmnidasfe.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.tarul.cn/Article/details/gfvnjptwr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.epnwcf.com/Article/details/gdwleredy.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.tarul.cn/Article/details/gscjgdnon.sHtML

JS:   Object.entries(obj)
来源：http://mobile.bbcook.cn/Article/details/gjjiyxrit.sHtML

TS:   Object.entries(obj)
来源：http://m.share.bbcook.cn/Article/details/gnwcwzlyf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.tarul.cn/Article/details/gtgptjxlp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.epnwcf.com/Article/details/gtqbbrabh.sHtML

Ruby: obj.instance_variables
来源：http://read.share.bbcook.cn/Article/details/gpbbxyegq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.sjlbkw.cn/Article/details/gwjfkpegg.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gxwyhykeu.sHtML

H. 异常与错误处理
来源：http://read.share.epnwcf.com/Article/details/gjavftbyl.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/ghyqturpc.sHtML

[H01] try / catch 基础
来源：http://m.share.bbcook.cn/Article/details/gfjywjoqx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.yfazqb.com/Article/details/gykjqjixy.sHtML


<!-- 参考信息 -->