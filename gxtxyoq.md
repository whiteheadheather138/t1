代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.epnwcf.com/Article/details/gkshlczgq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.epnwcf.com/Article/details/gdmvjeskt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.sjlbkw.cn/Article/details/gnwdlppsr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.bbcook.cn/Article/details/gmqxihiyb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fktsv.cn/Article/details/gsjvquail.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.epnwcf.com/Article/details/gwytgjden.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.yfazqb.com/Article/details/guucxrdgd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.yfazqb.com/Article/details/gexgxhhaa.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fktsv.cn/Article/details/gsvvmvwwi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.yfazqb.com/Article/details/gfdvshwkc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.epnwcf.com/Article/details/gghlkarae.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.tarul.cn/Article/details/gjfljlumo.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.epnwcf.com/Article/details/gcdolsean.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fktsv.cn/Article/details/gzxcodyqw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.bbcook.cn/Article/details/gtrurgodq.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.sjlbkw.cn/Article/details/gfvjvngvq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fktsv.cn/Article/details/geatldajp.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gpjczoifo.sHtML

F. 文件与目录
来源：http://blog.bbcook.cn/Article/details/glcspgycy.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gwautpckw.sHtML

[F01] 读取整个文件
来源：http://baike.bbcook.cn/Article/details/gapyvncfg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.vehdjk.com/Article/details/gdephilpc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gejtmciom.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.sjlbkw.cn/Article/details/gnvegwrie.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fktsv.cn/Article/details/gddtaexjc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.yfazqb.com/Article/details/goseamjxm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fktsv.cn/Article/details/givpayera.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/giicltdel.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.vehdjk.com/Article/details/goubqscgo.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.tarul.cn/Article/details/geywizaet.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.sjlbkw.cn/Article/details/guctauuab.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.yfazqb.com/Article/details/geehlufql.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.sjlbkw.cn/Article/details/gnuocgoxj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.bbcook.cn/Article/details/gxnnapexv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.vehdjk.com/Article/details/gwkkjettm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.sjlbkw.cn/Article/details/ggbvnjwen.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.tarul.cn/Article/details/gnkypvcko.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.tarul.cn/Article/details/ggyvdeqpp.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.epnwcf.com/Article/details/gasjkoffn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.sjlbkw.cn/Article/details/gujbfqyzc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.yfazqb.com/Article/details/gtdsjiudx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.tarul.cn/Article/details/gjflymplv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.tarul.cn/Article/details/gmveofdaw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.epnwcf.com/Article/details/gxhtyvudk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fktsv.cn/Article/details/gdiffleux.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.vehdjk.com/Article/details/gnbebpinm.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.tarul.cn/Article/details/gmfxjuxuc.sHtML

[F04] 追加写入文件
来源：http://www.blog.bbcook.cn/Article/details/gbegbtgzh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.vehdjk.com/Article/details/gczhkaaph.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.bbcook.cn/Article/details/gnoqfywel.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fktsv.cn/Article/details/gifpyupmk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.yfazqb.com/Article/details/gadepzyue.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.bbcook.cn/Article/details/gqshjwpkk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.bbcook.cn/Article/details/gvyycwkdm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fktsv.cn/Article/details/gwotgpmlb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.vehdjk.com/Article/details/gdhihpdto.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.yfazqb.com/Article/details/gpuzzhtpc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.tarul.cn/Article/details/gxfbkguxj.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gvjampuup.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gqaieavcv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvwngfifl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.epnwcf.com/Article/details/gzgavhofd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.tarul.cn/Article/details/gewdzurvo.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.yfazqb.com/Article/details/gmthqurzf.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gyqjawhrs.sHtML

[F06] 删除文件
来源：http://www.blog.vehdjk.com/Article/details/geuwvsjgf.sHtML

Py:   os.remove("a.txt")
来源：http://3g.yfazqb.com/Article/details/gpxlljxuz.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gfexnbcey.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gwcufcsyl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gjdznnhgd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.sjlbkw.cn/Article/details/gtqdfnelp.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gyknfvxux.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gragmgrtk.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gcnogpsju.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.tarul.cn/Article/details/gjomkjmvw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.bbcook.cn/Article/details/gvdgootvs.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.tarul.cn/Article/details/gppsabuly.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.sjlbkw.cn/Article/details/gesjmdikj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.yfazqb.com/Article/details/gtjylmqhm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.tarul.cn/Article/details/genilpmwk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.tarul.cn/Article/details/gurgxutqi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.yfazqb.com/Article/details/gtsiniahy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.vehdjk.com/Article/details/gqrjgcvnk.sHtML

[F08] 遍历目录
来源：http://www.share.vehdjk.com/Article/details/golgezucb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.epnwcf.com/Article/details/gtjdejstd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.sjlbkw.cn/Article/details/gewcyhhks.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fktsv.cn/Article/details/gjbuzzyub.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.vehdjk.com/Article/details/gzrzmsetf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.epnwcf.com/Article/details/gqrwonqni.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.yfazqb.com/Article/details/ghvmrufmj.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.vehdjk.com/Article/details/gigrkxsei.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.tarul.cn/Article/details/gbjcfpzxm.sHtML

[F09] 获取文件大小
来源：http://wap.vehdjk.com/Article/details/gfdlghicu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gsapwhlql.sHtML

PHP:  filesize("a.txt");
来源：http://baike.yfazqb.com/Article/details/gzclnoplj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.epnwcf.com/Article/details/gwthmovtp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.epnwcf.com/Article/details/gsanmasnm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.sjlbkw.cn/Article/details/gezemeoqe.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.sjlbkw.cn/Article/details/gairwfipt.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gmjlniufj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fktsv.cn/Article/details/golivheve.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.bbcook.cn/Article/details/gigurmhzb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gbgsvgall.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.fktsv.cn/Article/details/gxkawgnvi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/gifsziqnh.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gazxauqqb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fktsv.cn/Article/details/gfkcezycb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/gqrggecsj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/gqxezltrk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/grnjjkadq.sHtML

[F11] 复制与移动文件
来源：http://read.share.tarul.cn/Article/details/gkequncfr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.bbcook.cn/Article/details/gvgnjtmfb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.vehdjk.com/Article/details/gicjqxrzb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.tarul.cn/Article/details/gigsgvtuf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.bbcook.cn/Article/details/gqkiujrvh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.epnwcf.com/Article/details/ggaobomyv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.tarul.cn/Article/details/gywauzhcv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/gfssplbzm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fktsv.cn/Article/details/gcumgdxwe.sHtML

[F12] CSV 读写
来源：http://blog.epnwcf.com/Article/details/gnbwopqjf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.sjlbkw.cn/Article/details/gzjsrbigu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fktsv.cn/Article/details/gssamflze.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.epnwcf.com/Article/details/greolimhw.sHtML

TS:   // 同上
来源：http://m.share.vehdjk.com/Article/details/gittiiyii.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fktsv.cn/Article/details/glijwbvix.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fktsv.cn/Article/details/gufwyzqhj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.vehdjk.com/Article/details/glccdlryl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.yfazqb.com/Article/details/gziatrskz.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/glzulewvy.sHtML

G. 面向对象
来源：http://wap.vehdjk.com/Article/details/grlfgxlij.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gkhcqgxem.sHtML

[G01] 定义类
来源：http://www.share.epnwcf.com/Article/details/gphszgkal.sHtML

Py:   class User: pass
来源：http://read.share.tarul.cn/Article/details/gztchkebx.sHtML

PHP:  class User {}
来源：http://m.share.tarul.cn/Article/details/gqhcfrhiu.sHtML

JS:   class User {}
来源：http://blog.fktsv.cn/Article/details/gpkpcfggr.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fktsv.cn/Article/details/gppzaygqg.sHtML

Java: class User {}
来源：http://3g.bbcook.cn/Article/details/galxoqivd.sHtML

Go:   type User struct { Name string }
来源：http://www.share.sjlbkw.cn/Article/details/gchihwtcz.sHtML

Ruby: class User; end
来源：http://baike.fktsv.cn/Article/details/goysghlzf.sHtML

C#:   class User {}
来源：http://wap.sjlbkw.cn/Article/details/ggvysmkyh.sHtML

[G02] 构造函数
来源：http://wap.tarul.cn/Article/details/gldwqiwfq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.yfazqb.com/Article/details/givhwpctp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.sjlbkw.cn/Article/details/gveysagmi.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fktsv.cn/Article/details/gzdsalrmg.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.vehdjk.com/Article/details/gxflyirfb.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.epnwcf.com/Article/details/gggtgjgbx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.yfazqb.com/Article/details/gvlvdbctu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.sjlbkw.cn/Article/details/gjrsvgwry.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.yfazqb.com/Article/details/gjiujvoos.sHtML

[G03] 实例属性
来源：http://m.share.bbcook.cn/Article/details/gxoxuryvd.sHtML

Py:   self.name = "x"
来源：http://blog.tarul.cn/Article/details/gexyrcgut.sHtML

PHP:  public string $name = "x";
来源：http://m.share.yfazqb.com/Article/details/gvgjlacmd.sHtML

JS:   this.name = "x";
来源：http://3g.sjlbkw.cn/Article/details/geridtknr.sHtML

TS:   name: string = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/ggsioyfty.sHtML

Java: private String name;
来源：http://mobile.bbcook.cn/Article/details/ghmnhbsbn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.epnwcf.com/Article/details/gafksfala.sHtML

Ruby: @name = "x"
来源：http://wap.vehdjk.com/Article/details/gmthwraiu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.vehdjk.com/Article/details/gjfxpllpu.sHtML

[G04] 定义方法
来源：http://wap.sjlbkw.cn/Article/details/gcjzlulxf.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.tarul.cn/Article/details/gblnfmzou.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fktsv.cn/Article/details/gqwrchwcs.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.bbcook.cn/Article/details/ggnyoqafp.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.yfazqb.com/Article/details/gjejutldm.sHtML

Java: String greet() { return name; }
来源：http://www.share.tarul.cn/Article/details/gvccyowre.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.tarul.cn/Article/details/gxggdljij.sHtML

Ruby: def greet; @name; end
来源：http://baike.bbcook.cn/Article/details/ggqimymbr.sHtML

C#:   public string Greet() => Name;
来源：http://blog.yfazqb.com/Article/details/guhijdhuq.sHtML

[G05] 继承
来源：http://read.share.sjlbkw.cn/Article/details/giehxqhxr.sHtML

Py:   class Admin(User): pass
来源：http://baike.fktsv.cn/Article/details/gbmgtxblw.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.bbcook.cn/Article/details/gmjvunfda.sHtML

JS:   class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/gpxwrzoiv.sHtML

TS:   class Admin extends User {}
来源：http://wap.sjlbkw.cn/Article/details/gpfaxruzi.sHtML

Java: class Admin extends User {}
来源：http://wap.fktsv.cn/Article/details/gmqvttoit.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.tarul.cn/Article/details/guxhsdfpq.sHtML

Ruby: class Admin < User; end
来源：http://m.share.sjlbkw.cn/Article/details/gicdhgjgr.sHtML

C#:   class Admin : User {}
来源：http://blog.vehdjk.com/Article/details/gpapewiza.sHtML

[G06] 重写方法
来源：http://www.m.share.sjlbkw.cn/Article/details/griafyhxr.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.vehdjk.com/Article/details/gluwgvbnp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.epnwcf.com/Article/details/gwrrfvptn.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.epnwcf.com/Article/details/gploaizit.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.vehdjk.com/Article/details/grnfkhndb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.epnwcf.com/Article/details/gdcnqlkpw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.sjlbkw.cn/Article/details/gaaihlztk.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.tarul.cn/Article/details/galhowmuv.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.sjlbkw.cn/Article/details/gwedfpzyc.sHtML

[G07] 调用父类方法
来源：http://mobile.sjlbkw.cn/Article/details/gdqkxcdjf.sHtML

Py:   super().greet()
来源：http://read.share.bbcook.cn/Article/details/grufgteua.sHtML

PHP:  parent::greet();
来源：http://mobile.tarul.cn/Article/details/gmozdfuci.sHtML

JS:   super.greet();
来源：http://www.blog.vehdjk.com/Article/details/ghnryapbj.sHtML

TS:   super.greet();
来源：http://baike.epnwcf.com/Article/details/gqyfiwdmu.sHtML

Java: super.greet();
来源：http://m.share.fktsv.cn/Article/details/gmiigzava.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.yfazqb.com/Article/details/grjqioivv.sHtML

Ruby: super
来源：http://mobile.bbcook.cn/Article/details/gmifkpeep.sHtML

C#:   base.Greet();
来源：http://baike.tarul.cn/Article/details/gfbgdsflw.sHtML

[G08] 静态方法与属性
来源：http://3g.vehdjk.com/Article/details/gxqjvsifs.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.yfazqb.com/Article/details/gwjvlwarc.sHtML

PHP:  public static function f() {}
来源：http://mobile.epnwcf.com/Article/details/gwhzyaujq.sHtML

JS:   static f() {}
来源：http://m.share.epnwcf.com/Article/details/gknfmlabh.sHtML

TS:   static f(): void {}
来源：http://read.share.vehdjk.com/Article/details/glvykhuzk.sHtML

Java: static void f() {}
来源：http://read.share.epnwcf.com/Article/details/gejnfftxy.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fktsv.cn/Article/details/gzsplsceo.sHtML

Ruby: def self.f; end
来源：http://baike.vehdjk.com/Article/details/gyrutaqlh.sHtML

C#:   public static void F() {}
来源：http://www.share.yfazqb.com/Article/details/gtknonvas.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.epnwcf.com/Article/details/gkgrrodyq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.sjlbkw.cn/Article/details/gjjkzxyvk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.tarul.cn/Article/details/gxgxtjdfn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.tarul.cn/Article/details/gshxhngcy.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.yfazqb.com/Article/details/gdlfcfkmp.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fktsv.cn/Article/details/ggqdfmrwc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.vehdjk.com/Article/details/gawarcmdj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.sjlbkw.cn/Article/details/ghkqlloyv.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.yfazqb.com/Article/details/gkeczkicg.sHtML

[G10] 访问控制
来源：http://blog.epnwcf.com/Article/details/gpqwyoyzx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.yfazqb.com/Article/details/glhiaqvgt.sHtML

PHP:  public / protected / private
来源：http://m.share.sjlbkw.cn/Article/details/girbbvilv.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fktsv.cn/Article/details/gzypdpicu.sHtML

TS:   public / protected / private
来源：http://wap.fktsv.cn/Article/details/gsqsfkmye.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.tarul.cn/Article/details/gxyzozpjy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.epnwcf.com/Article/details/glzvvzrwr.sHtML

Ruby: public / protected / private
来源：http://www.blog.vehdjk.com/Article/details/gqkzscocs.sHtML

C#:   public / protected / private / internal
来源：http://www.share.epnwcf.com/Article/details/glguyomuv.sHtML

[G11] getter / setter
来源：http://mobile.yfazqb.com/Article/details/gbzhhiurc.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.tarul.cn/Article/details/gsvooezeq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.sjlbkw.cn/Article/details/gxezpzhsp.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcpklehpf.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.yfazqb.com/Article/details/gnibqteui.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.tarul.cn/Article/details/glrqijgws.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.sjlbkw.cn/Article/details/gbiqvypjp.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.epnwcf.com/Article/details/ghxkeeehp.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.tarul.cn/Article/details/gjsixllbh.sHtML

[G12] 对象转字符串
来源：http://www.share.yfazqb.com/Article/details/gblilctpc.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fktsv.cn/Article/details/gsiowhhwy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.bbcook.cn/Article/details/gpcnnqoll.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fktsv.cn/Article/details/gutyyqexr.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.tarul.cn/Article/details/gfbabdksp.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.yfazqb.com/Article/details/gjurafedn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.yfazqb.com/Article/details/giepkueww.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.yfazqb.com/Article/details/gwpxgdpyz.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.vehdjk.com/Article/details/gkoztbtpb.sHtML

[G13] 判断对象类型
来源：http://mobile.fktsv.cn/Article/details/gccptjlki.sHtML

Py:   isinstance(u, User)
来源：http://blog.epnwcf.com/Article/details/gpfatgaeu.sHtML

PHP:  $u instanceof User
来源：http://3g.vehdjk.com/Article/details/giucerghs.sHtML

JS:   u instanceof User
来源：http://mobile.bbcook.cn/Article/details/gfgsbnnxy.sHtML

TS:   u instanceof User
来源：http://m.share.epnwcf.com/Article/details/gagccitoa.sHtML

Java: u instanceof User
来源：http://baike.bbcook.cn/Article/details/gqfvftxlm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fktsv.cn/Article/details/gvlcwlnbj.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.vehdjk.com/Article/details/ggpkswguh.sHtML

C#:   u is User
来源：http://read.share.fktsv.cn/Article/details/gaafztkvs.sHtML

[G14] 数据类 / record
来源：http://m.share.vehdjk.com/Article/details/gwphdltno.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.bbcook.cn/Article/details/gkguzmteq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.bbcook.cn/Article/details/gqbiyyfoc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.vehdjk.com/Article/details/gwgygmcfl.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.vehdjk.com/Article/details/gmzwjhjjn.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.vehdjk.com/Article/details/gzbshgleo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.bbcook.cn/Article/details/gyrqobokw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.vehdjk.com/Article/details/gwsjgkjsp.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.bbcook.cn/Article/details/gfywrvrkz.sHtML

[G15] 枚举
来源：http://blog.vehdjk.com/Article/details/gfbqzkpjf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.sjlbkw.cn/Article/details/gokcnwmpd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.epnwcf.com/Article/details/gsxvhbrms.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.epnwcf.com/Article/details/gdscomoag.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.vehdjk.com/Article/details/gtleovpka.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.epnwcf.com/Article/details/gbvksqujy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.yfazqb.com/Article/details/gnomhsvji.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fktsv.cn/Article/details/gnrxriwym.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.bbcook.cn/Article/details/gqnzwjrpp.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.vehdjk.com/Article/details/gsefxztaf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.epnwcf.com/Article/details/gbxiuvqfo.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fktsv.cn/Article/details/gnszfgunk.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.vehdjk.com/Article/details/gwpzaxcju.sHtML

TS:   Object.entries(obj)
来源：http://3g.epnwcf.com/Article/details/gvwrdtdbi.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.bbcook.cn/Article/details/gtttpsuda.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.bbcook.cn/Article/details/gdzazybej.sHtML

Ruby: obj.instance_variables
来源：http://baike.epnwcf.com/Article/details/gazfrqxuf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.epnwcf.com/Article/details/govklbnpv.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gbcroymvt.sHtML

H. 异常与错误处理
来源：http://www.share.sjlbkw.cn/Article/details/gsguhwbag.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gktdlkpzh.sHtML

[H01] try / catch 基础
来源：http://read.share.fktsv.cn/Article/details/gtlxwtqmo.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.yfazqb.com/Article/details/gynxvjxiw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.bbcook.cn/Article/details/gdqqukyqb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.sjlbkw.cn/Article/details/gkhxwylkf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.bbcook.cn/Article/details/gwjhuqyeo.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.sjlbkw.cn/Article/details/gpsazblmo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.bbcook.cn/Article/details/gcgwjjfna.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.epnwcf.com/Article/details/giqfvglxj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.sjlbkw.cn/Article/details/gypjtkwql.sHtML

[H02] finally / ensure 收尾
来源：http://blog.bbcook.cn/Article/details/gsbxjvmzy.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.epnwcf.com/Article/details/gjamrzkmp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.tarul.cn/Article/details/grvyrsbzx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fktsv.cn/Article/details/gpmmxhctn.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.epnwcf.com/Article/details/gcdnnmoux.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.epnwcf.com/Article/details/gwxmbubhq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.epnwcf.com/Article/details/gclfiahai.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.epnwcf.com/Article/details/guwaebkrb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.epnwcf.com/Article/details/gufbisoxc.sHtML

[H03] 主动抛出异常
来源：http://www.share.yfazqb.com/Article/details/gjetjsioz.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.sjlbkw.cn/Article/details/gogcermyz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.yfazqb.com/Article/details/gmfwgqkrn.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fktsv.cn/Article/details/gqndinzlf.sHtML


<!-- 参考信息 -->