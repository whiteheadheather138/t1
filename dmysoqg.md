代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.yfazqb.com/Article/details/geoxmqhmo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fktsv.cn/Article/details/gvdmgclhz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.yfazqb.com/Article/details/gqpjvxtsj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.sjlbkw.cn/Article/details/gtskgufvi.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.epnwcf.com/Article/details/gelktbtnh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.tarul.cn/Article/details/giqblgfvl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fktsv.cn/Article/details/gurtdfekx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fktsv.cn/Article/details/gqanyheay.sHtML

[E22] 字节长度与字符长度
来源：http://wap.yfazqb.com/Article/details/gopfoajqq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.vehdjk.com/Article/details/ghqkimknj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.sjlbkw.cn/Article/details/gwfvpbwnm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.vehdjk.com/Article/details/goemejoxu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fktsv.cn/Article/details/ggaxwucla.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.bbcook.cn/Article/details/gqfcgdupa.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.bbcook.cn/Article/details/gwdhtzasz.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.sjlbkw.cn/Article/details/gthxtxitd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fktsv.cn/Article/details/gpgaffebo.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/goxiyxxii.sHtML

F. 文件与目录
来源：http://m.share.fktsv.cn/Article/details/gmgyugykr.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gzqgajzcq.sHtML

[F01] 读取整个文件
来源：http://baike.epnwcf.com/Article/details/gpwbloavi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.vehdjk.com/Article/details/giegyxrkh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.tarul.cn/Article/details/gbteyfrbq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.tarul.cn/Article/details/gynpqheev.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.tarul.cn/Article/details/gnkbernrf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.vehdjk.com/Article/details/gkwsqeckx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.bbcook.cn/Article/details/gctbribwv.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gpmjizqtr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gkxqgojgq.sHtML

[F02] 逐行读取文件
来源：http://mobile.vehdjk.com/Article/details/gnknzphgg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.yfazqb.com/Article/details/ghvgvpiws.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.sjlbkw.cn/Article/details/gzqgmfvit.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fktsv.cn/Article/details/gvxylnubt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.tarul.cn/Article/details/gyxiuoony.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.tarul.cn/Article/details/gztmhqoxb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.bbcook.cn/Article/details/guigrfhle.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.epnwcf.com/Article/details/gewfduqnd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.vehdjk.com/Article/details/gwojslboz.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fktsv.cn/Article/details/gztgivyvs.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.epnwcf.com/Article/details/ggnojneio.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.tarul.cn/Article/details/gnfstbzpk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.epnwcf.com/Article/details/ggxazyphz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fktsv.cn/Article/details/gfaqbyxtr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.sjlbkw.cn/Article/details/gbxxsvesg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.sjlbkw.cn/Article/details/gknwjejat.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.bbcook.cn/Article/details/gdvunvucf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.epnwcf.com/Article/details/geczprtjc.sHtML

[F04] 追加写入文件
来源：http://3g.epnwcf.com/Article/details/gmipkfxtq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.vehdjk.com/Article/details/gxerjqkvl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.epnwcf.com/Article/details/gvfviqfat.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.yfazqb.com/Article/details/gwatcgiqf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.sjlbkw.cn/Article/details/grrahfdcb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.yfazqb.com/Article/details/gqgnqgmmf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.vehdjk.com/Article/details/gkiphlosk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.vehdjk.com/Article/details/ggozglnxk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fktsv.cn/Article/details/gynhjqbcn.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.tarul.cn/Article/details/gzddezgzc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.vehdjk.com/Article/details/gmytlcjbl.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fktsv.cn/Article/details/gjmmljesl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gepdilkqh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gqprjwgsc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.tarul.cn/Article/details/ganllvrjh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.tarul.cn/Article/details/gboaquzrj.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gfjohyeos.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gylhsyzef.sHtML

[F06] 删除文件
来源：http://m.share.fktsv.cn/Article/details/gjimqwyvs.sHtML

Py:   os.remove("a.txt")
来源：http://baike.yfazqb.com/Article/details/gnytjqxec.sHtML

PHP:  unlink("a.txt");
来源：http://blog.epnwcf.com/Article/details/gofgqsowg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gnuneaphq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gtngowqce.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.vehdjk.com/Article/details/gxzkvqynz.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.epnwcf.com/Article/details/gxcgcvqps.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fktsv.cn/Article/details/grzxlpmnm.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.yfazqb.com/Article/details/gqdxyuapp.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.sjlbkw.cn/Article/details/gdqcyxhes.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.bbcook.cn/Article/details/gaxjfdslx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.tarul.cn/Article/details/guxdmxhvf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.bbcook.cn/Article/details/gpirissxn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.epnwcf.com/Article/details/gydazliri.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fktsv.cn/Article/details/gdflfqizv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.sjlbkw.cn/Article/details/gouxfirow.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.tarul.cn/Article/details/gortiwjsu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.vehdjk.com/Article/details/gwwjyjeri.sHtML

[F08] 遍历目录
来源：http://www.share.fktsv.cn/Article/details/glpoqeceq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.tarul.cn/Article/details/gjuyhorqr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.vehdjk.com/Article/details/guyzmbpso.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.epnwcf.com/Article/details/glthsoloo.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.vehdjk.com/Article/details/gmkqkmmyv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.sjlbkw.cn/Article/details/gzodmzxpw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.vehdjk.com/Article/details/gbmlvycvd.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.bbcook.cn/Article/details/grjwdudty.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.bbcook.cn/Article/details/gkukmjiyg.sHtML

[F09] 获取文件大小
来源：http://mobile.vehdjk.com/Article/details/gveqyfmwl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fktsv.cn/Article/details/goxpexrdr.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fktsv.cn/Article/details/golbmvunm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.epnwcf.com/Article/details/gukfyvfje.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.epnwcf.com/Article/details/gatsznhal.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.tarul.cn/Article/details/gwvhbemzx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.yfazqb.com/Article/details/gclazaqsk.sHtML

Ruby: File.size("a.txt")
来源：http://3g.epnwcf.com/Article/details/gbrcalumm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.sjlbkw.cn/Article/details/gbmvkvfsq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fktsv.cn/Article/details/gqthdmnfl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/gatoptdge.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.tarul.cn/Article/details/gvpzttmto.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gesnsspdc.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gizwqxbrs.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.sjlbkw.cn/Article/details/gaboxbbso.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/glqegyxqg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.epnwcf.com/Article/details/gabqxwooo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.bbcook.cn/Article/details/gxlqklfby.sHtML

[F11] 复制与移动文件
来源：http://blog.epnwcf.com/Article/details/gfnzvnowx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.sjlbkw.cn/Article/details/gmhryfmwg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.epnwcf.com/Article/details/gwzpdpghv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.tarul.cn/Article/details/gghaqqlas.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.tarul.cn/Article/details/gjylgghju.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.sjlbkw.cn/Article/details/gbjliqtgn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fktsv.cn/Article/details/gmwozoung.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.epnwcf.com/Article/details/gilwztaty.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.yfazqb.com/Article/details/gjuvyldgd.sHtML

[F12] CSV 读写
来源：http://read.share.yfazqb.com/Article/details/gocsgmtvz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.vehdjk.com/Article/details/gswitfrwx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.epnwcf.com/Article/details/gowvzlxha.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.sjlbkw.cn/Article/details/gxfnpaydo.sHtML

TS:   // 同上
来源：http://wap.tarul.cn/Article/details/goalpsmhu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.tarul.cn/Article/details/gdezvyzkm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fktsv.cn/Article/details/gjjhnarhj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.tarul.cn/Article/details/gmveowhnm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fktsv.cn/Article/details/gnurpajtz.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/ggmlhixjj.sHtML

G. 面向对象
来源：http://m.share.sjlbkw.cn/Article/details/gwcuawdjw.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gwbcegetm.sHtML

[G01] 定义类
来源：http://www.share.bbcook.cn/Article/details/gamhnjsly.sHtML

Py:   class User: pass
来源：http://blog.tarul.cn/Article/details/grutcpqyx.sHtML

PHP:  class User {}
来源：http://mobile.bbcook.cn/Article/details/grhclnmrd.sHtML

JS:   class User {}
来源：http://www.share.fktsv.cn/Article/details/glsrlfheg.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.sjlbkw.cn/Article/details/glzgongsm.sHtML

Java: class User {}
来源：http://www.m.share.bbcook.cn/Article/details/golsrreys.sHtML

Go:   type User struct { Name string }
来源：http://3g.bbcook.cn/Article/details/ggjwsxqmv.sHtML

Ruby: class User; end
来源：http://read.share.bbcook.cn/Article/details/gbvkahzmk.sHtML

C#:   class User {}
来源：http://read.share.bbcook.cn/Article/details/gzdrmxslf.sHtML

[G02] 构造函数
来源：http://blog.epnwcf.com/Article/details/gdyczrazj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fktsv.cn/Article/details/guyrdwqjt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.vehdjk.com/Article/details/gjcdhfrxm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.epnwcf.com/Article/details/giakwlenw.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.sjlbkw.cn/Article/details/gtrcmddpu.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.tarul.cn/Article/details/ggbqjsqje.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.sjlbkw.cn/Article/details/ggtxglfkd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fktsv.cn/Article/details/gsyaxvdyy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.vehdjk.com/Article/details/gnjfudtwf.sHtML

[G03] 实例属性
来源：http://wap.yfazqb.com/Article/details/gdbwszksr.sHtML

Py:   self.name = "x"
来源：http://www.blog.tarul.cn/Article/details/gcaxvtubm.sHtML

PHP:  public string $name = "x";
来源：http://mobile.epnwcf.com/Article/details/gzckdkkye.sHtML

JS:   this.name = "x";
来源：http://read.share.vehdjk.com/Article/details/gkrtkjzfi.sHtML

TS:   name: string = "x";
来源：http://wap.bbcook.cn/Article/details/gjluiexmh.sHtML

Java: private String name;
来源：http://read.share.bbcook.cn/Article/details/gsdsqgynt.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.yfazqb.com/Article/details/gwyfdqyik.sHtML

Ruby: @name = "x"
来源：http://www.m.share.sjlbkw.cn/Article/details/gxtrsphai.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.epnwcf.com/Article/details/gfgmefogd.sHtML

[G04] 定义方法
来源：http://wap.bbcook.cn/Article/details/gacdxgdyb.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.sjlbkw.cn/Article/details/genlhtxte.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.vehdjk.com/Article/details/gzmzukxrd.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.sjlbkw.cn/Article/details/gllvwlvem.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.yfazqb.com/Article/details/gpajxtdvy.sHtML

Java: String greet() { return name; }
来源：http://read.share.yfazqb.com/Article/details/goqogklvd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.tarul.cn/Article/details/geiooartw.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.bbcook.cn/Article/details/gkcjveytf.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.tarul.cn/Article/details/gqukefdha.sHtML

[G05] 继承
来源：http://wap.fktsv.cn/Article/details/gvwisusyg.sHtML

Py:   class Admin(User): pass
来源：http://blog.bbcook.cn/Article/details/gfdzzcbdz.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/genzvfdiu.sHtML

JS:   class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/gfgbixjzz.sHtML

TS:   class Admin extends User {}
来源：http://3g.tarul.cn/Article/details/gwpgobmya.sHtML

Java: class Admin extends User {}
来源：http://m.share.fktsv.cn/Article/details/gyvfnpdjw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.bbcook.cn/Article/details/goziyvofd.sHtML

Ruby: class Admin < User; end
来源：http://mobile.vehdjk.com/Article/details/gdxeiuegu.sHtML

C#:   class Admin : User {}
来源：http://wap.fktsv.cn/Article/details/grxqgshfc.sHtML

[G06] 重写方法
来源：http://baike.sjlbkw.cn/Article/details/gycakvvik.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.yfazqb.com/Article/details/gmhawvdbh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/ggpnswqvc.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.sjlbkw.cn/Article/details/ggqygygdw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.yfazqb.com/Article/details/gqcangugt.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.tarul.cn/Article/details/gxxexhpih.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.sjlbkw.cn/Article/details/gmnaoxtdn.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.tarul.cn/Article/details/gsvhlqyje.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.vehdjk.com/Article/details/gtlkaqolw.sHtML

[G07] 调用父类方法
来源：http://www.blog.epnwcf.com/Article/details/gqwkllfou.sHtML

Py:   super().greet()
来源：http://3g.tarul.cn/Article/details/gyooxevpr.sHtML

PHP:  parent::greet();
来源：http://wap.tarul.cn/Article/details/gvpcevlcm.sHtML

JS:   super.greet();
来源：http://3g.epnwcf.com/Article/details/gbiwtmotq.sHtML

TS:   super.greet();
来源：http://3g.bbcook.cn/Article/details/ginwdadik.sHtML

Java: super.greet();
来源：http://blog.sjlbkw.cn/Article/details/gfsvkrzhs.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.epnwcf.com/Article/details/gqjoemufd.sHtML

Ruby: super
来源：http://read.share.bbcook.cn/Article/details/grptbtlac.sHtML

C#:   base.Greet();
来源：http://blog.yfazqb.com/Article/details/gccjcxnwf.sHtML

[G08] 静态方法与属性
来源：http://wap.tarul.cn/Article/details/gspnorfou.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.tarul.cn/Article/details/gitbwurqf.sHtML

PHP:  public static function f() {}
来源：http://blog.sjlbkw.cn/Article/details/gqphgilwz.sHtML

JS:   static f() {}
来源：http://3g.fktsv.cn/Article/details/gzokglywr.sHtML

TS:   static f(): void {}
来源：http://mobile.yfazqb.com/Article/details/gsckfdefg.sHtML

Java: static void f() {}
来源：http://m.share.yfazqb.com/Article/details/gvmprzjtw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.yfazqb.com/Article/details/geemwklla.sHtML

Ruby: def self.f; end
来源：http://baike.bbcook.cn/Article/details/gaizdqlvm.sHtML

C#:   public static void F() {}
来源：http://wap.yfazqb.com/Article/details/ggxugeiyv.sHtML

[G09] 接口 / 抽象类
来源：http://3g.tarul.cn/Article/details/gjmyscijo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.tarul.cn/Article/details/gknyjpibz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fktsv.cn/Article/details/germmhmwp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.yfazqb.com/Article/details/giyghpeys.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.vehdjk.com/Article/details/gxnpndeya.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fktsv.cn/Article/details/ghfxnwlqe.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.sjlbkw.cn/Article/details/gmopqyqxp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.sjlbkw.cn/Article/details/ggpnawfkp.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.sjlbkw.cn/Article/details/gnkrawdrw.sHtML

[G10] 访问控制
来源：http://www.m.share.vehdjk.com/Article/details/gsgnlwgwq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.vehdjk.com/Article/details/gpzuqygeo.sHtML

PHP:  public / protected / private
来源：http://www.blog.sjlbkw.cn/Article/details/gppeqcmke.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.vehdjk.com/Article/details/gotouhyad.sHtML

TS:   public / protected / private
来源：http://www.blog.bbcook.cn/Article/details/goezsdier.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.yfazqb.com/Article/details/ghkkrbedm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.yfazqb.com/Article/details/gotunynky.sHtML

Ruby: public / protected / private
来源：http://www.blog.epnwcf.com/Article/details/grlvkamjo.sHtML

C#:   public / protected / private / internal
来源：http://www.share.tarul.cn/Article/details/gstmownyi.sHtML

[G11] getter / setter
来源：http://3g.vehdjk.com/Article/details/gcafvupuj.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.yfazqb.com/Article/details/gsaxzjtjj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.tarul.cn/Article/details/ggnxsctve.sHtML

JS:   get name() { return this._name; }
来源：http://wap.yfazqb.com/Article/details/goqohotev.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fktsv.cn/Article/details/gqtshwctj.sHtML

Java: public String getName() { return name; }
来源：http://m.share.vehdjk.com/Article/details/gelndjcdx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.bbcook.cn/Article/details/gfsmhndcm.sHtML

Ruby: attr_accessor :name
来源：http://m.share.epnwcf.com/Article/details/glrdrgqdq.sHtML

C#:   public string Name { get; set; }
来源：http://blog.vehdjk.com/Article/details/gstjoseqe.sHtML

[G12] 对象转字符串
来源：http://www.share.yfazqb.com/Article/details/gtsqiloiq.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.sjlbkw.cn/Article/details/gjyocrohr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.sjlbkw.cn/Article/details/gpquyyajj.sHtML

JS:   toString() { return this.name; }
来源：http://3g.sjlbkw.cn/Article/details/gwzclngsk.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.epnwcf.com/Article/details/gmskcxqqa.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fktsv.cn/Article/details/gujqwqepp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.bbcook.cn/Article/details/gvbxpcanb.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.bbcook.cn/Article/details/gtkbihnsu.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.epnwcf.com/Article/details/gkwwyvzah.sHtML

[G13] 判断对象类型
来源：http://m.share.bbcook.cn/Article/details/gqiepwahs.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.epnwcf.com/Article/details/gywulbjtz.sHtML

PHP:  $u instanceof User
来源：http://www.blog.tarul.cn/Article/details/gibkmyymj.sHtML

JS:   u instanceof User
来源：http://read.share.vehdjk.com/Article/details/grmymhucb.sHtML

TS:   u instanceof User
来源：http://mobile.bbcook.cn/Article/details/ghdtzjgrr.sHtML

Java: u instanceof User
来源：http://m.share.yfazqb.com/Article/details/geyzhddin.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.sjlbkw.cn/Article/details/gcoainbhz.sHtML

Ruby: u.is_a?(User)
来源：http://3g.sjlbkw.cn/Article/details/guyzzwcdy.sHtML

C#:   u is User
来源：http://www.share.tarul.cn/Article/details/gsojskadh.sHtML

[G14] 数据类 / record
来源：http://read.share.bbcook.cn/Article/details/gizbdvkxo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.bbcook.cn/Article/details/gistdqemo.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.epnwcf.com/Article/details/gyqlyucqu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.vehdjk.com/Article/details/gqjekhevt.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.vehdjk.com/Article/details/gvglcduup.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.tarul.cn/Article/details/gddfhxqst.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.yfazqb.com/Article/details/gzebbmxyb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fktsv.cn/Article/details/gtpffepnu.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.vehdjk.com/Article/details/gkghpjtmq.sHtML

[G15] 枚举
来源：http://www.blog.yfazqb.com/Article/details/gienriaqb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.epnwcf.com/Article/details/gjeknyyjz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fktsv.cn/Article/details/gfgcvptoo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.yfazqb.com/Article/details/gorjhagkl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.epnwcf.com/Article/details/gyhnrmlmt.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fktsv.cn/Article/details/gieonggph.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.sjlbkw.cn/Article/details/gogaobryr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.bbcook.cn/Article/details/ggghtvpkh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.tarul.cn/Article/details/gekmlmxlf.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.bbcook.cn/Article/details/gwxylvgzm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fktsv.cn/Article/details/gvtkxdcxi.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.yfazqb.com/Article/details/gyofiqonc.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fktsv.cn/Article/details/gdemrlbzy.sHtML

TS:   Object.entries(obj)
来源：http://3g.vehdjk.com/Article/details/gtlgtdlhh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fktsv.cn/Article/details/ghnlbpult.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.tarul.cn/Article/details/gozrgfnbp.sHtML

Ruby: obj.instance_variables
来源：http://blog.tarul.cn/Article/details/gdcsqwusv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.epnwcf.com/Article/details/ghtystven.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gaxbasrjr.sHtML

H. 异常与错误处理
来源：http://read.share.tarul.cn/Article/details/ghgvhkvit.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gaupddwxn.sHtML

[H01] try / catch 基础
来源：http://read.share.vehdjk.com/Article/details/ginhimtss.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fktsv.cn/Article/details/gjelmjqdi.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.epnwcf.com/Article/details/ghintsdio.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.tarul.cn/Article/details/gwhwuzhje.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.yfazqb.com/Article/details/gbdsvghda.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.bbcook.cn/Article/details/gjnbkpxtj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fktsv.cn/Article/details/gwyjnoqvn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.vehdjk.com/Article/details/gkvvlqjam.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.tarul.cn/Article/details/gcimrvqeq.sHtML

[H02] finally / ensure 收尾
来源：http://wap.vehdjk.com/Article/details/gvjdajsst.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.epnwcf.com/Article/details/gplnzlvgp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/gjungqaco.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.tarul.cn/Article/details/gikpyjcdv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.tarul.cn/Article/details/gmvkunucb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.vehdjk.com/Article/details/gkptmcvys.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.vehdjk.com/Article/details/ghurzpkhf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fktsv.cn/Article/details/gqwqcwgsq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.bbcook.cn/Article/details/gypjfeoui.sHtML

[H03] 主动抛出异常
来源：http://www.share.sjlbkw.cn/Article/details/gipafckeh.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.tarul.cn/Article/details/gccorsjdl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.tarul.cn/Article/details/gfouigkvs.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.vehdjk.com/Article/details/gxjntcsck.sHtML


<!-- 参考信息 -->