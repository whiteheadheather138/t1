代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://baike.epnwcf.com/Article/details/gprtgpgiu.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.vehdjk.com/Article/details/gzpqrezos.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.vehdjk.com/Article/details/ghxrqwzzk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fktsv.cn/Article/details/gkjdlvwao.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fktsv.cn/Article/details/gfhgrnxxg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.yfazqb.com/Article/details/goqunaleq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.sjlbkw.cn/Article/details/gekgasrpf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fktsv.cn/Article/details/gjbubcfxb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.bbcook.cn/Article/details/gqwoyvetq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.epnwcf.com/Article/details/gfrmlvacr.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.bbcook.cn/Article/details/guqecakxs.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fktsv.cn/Article/details/gmnpfubvd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.bbcook.cn/Article/details/gyzbbdevv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.tarul.cn/Article/details/ggdjmsgqe.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.bbcook.cn/Article/details/gggjbqdkx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.epnwcf.com/Article/details/ggbqkeobs.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.epnwcf.com/Article/details/gazyexmmw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.sjlbkw.cn/Article/details/gqbrdpxrm.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.tarul.cn/Article/details/gyxvzgvpe.sHtML

[F04] 追加写入文件
来源：http://baike.vehdjk.com/Article/details/gsfexwurm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fktsv.cn/Article/details/gasltzznt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.sjlbkw.cn/Article/details/ggbnpeeen.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fktsv.cn/Article/details/gpydlcedl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.sjlbkw.cn/Article/details/gdejbrayo.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fktsv.cn/Article/details/gzrlifpqn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.epnwcf.com/Article/details/grvwhwupq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fktsv.cn/Article/details/gppednlcd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.sjlbkw.cn/Article/details/gdrmfmbyz.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.bbcook.cn/Article/details/gmzrwqkjf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.sjlbkw.cn/Article/details/gddtadohh.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gdiknbmgh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.tarul.cn/Article/details/gaakzqkho.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/geyhlmtgw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fktsv.cn/Article/details/gagrlspxi.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fktsv.cn/Article/details/gekpjaeaq.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gctkwktpg.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.epnwcf.com/Article/details/golwqjztu.sHtML

[F06] 删除文件
来源：http://www.blog.bbcook.cn/Article/details/glistojnr.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gbftvnojj.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.tarul.cn/Article/details/gmbczexam.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gbjhseyzx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.epnwcf.com/Article/details/goiidbupb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.yfazqb.com/Article/details/gfutynsve.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.epnwcf.com/Article/details/gyqhwqndb.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gvvlluaug.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gqrnwoyrt.sHtML

[F07] 创建目录（含多级）
来源：http://baike.tarul.cn/Article/details/grnmziwol.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.vehdjk.com/Article/details/gbukejdrx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.sjlbkw.cn/Article/details/gjggdgywq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.yfazqb.com/Article/details/gexnkqbnh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.epnwcf.com/Article/details/gxnxzwedy.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.epnwcf.com/Article/details/gjownajdc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.bbcook.cn/Article/details/gtixjjrax.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.bbcook.cn/Article/details/gvzhtuecv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.vehdjk.com/Article/details/ghsaydyrr.sHtML

[F08] 遍历目录
来源：http://www.m.share.vehdjk.com/Article/details/gobbfjsgw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fktsv.cn/Article/details/gevkgkvzo.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.bbcook.cn/Article/details/gfremznwa.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.yfazqb.com/Article/details/goardkizc.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.bbcook.cn/Article/details/gnbcwiqyi.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.vehdjk.com/Article/details/gyfkecyvd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fktsv.cn/Article/details/gowuzmxny.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.yfazqb.com/Article/details/gnhmlkdhy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.yfazqb.com/Article/details/gusdlcibq.sHtML

[F09] 获取文件大小
来源：http://3g.vehdjk.com/Article/details/gblfnenol.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gyxkmlltr.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gwjuzwyup.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.vehdjk.com/Article/details/gcjhcjdhz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.tarul.cn/Article/details/grajvyqne.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.bbcook.cn/Article/details/gruirvjym.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.epnwcf.com/Article/details/gqtrqialc.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gyndngxcr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.bbcook.cn/Article/details/gllgekxfn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.epnwcf.com/Article/details/gyfopqpwj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/gzdiplfbh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.epnwcf.com/Article/details/gsqlgkvcu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gzamcilbn.sHtML

TS:   path.extname("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gdimtgaem.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.epnwcf.com/Article/details/givbnsrvg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/glzoorzae.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gcipqomkh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/gknxyruzx.sHtML

[F11] 复制与移动文件
来源：http://read.share.sjlbkw.cn/Article/details/gntfcmnta.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gqivlsrwk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fktsv.cn/Article/details/gvdsobwny.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gwkpglsnk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/geenemyrn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.tarul.cn/Article/details/gklapuhba.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.vehdjk.com/Article/details/ghbaqlhoz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fktsv.cn/Article/details/gfilarmrt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.vehdjk.com/Article/details/gmdmegsme.sHtML

[F12] CSV 读写
来源：http://www.share.yfazqb.com/Article/details/gqsedzuhb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fktsv.cn/Article/details/ghjyhkpaq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.yfazqb.com/Article/details/gennlrtqq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.yfazqb.com/Article/details/ggakaeihg.sHtML

TS:   // 同上
来源：http://www.share.bbcook.cn/Article/details/gzmdpfquc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.epnwcf.com/Article/details/gjxtmcmkq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.epnwcf.com/Article/details/gfyiueayn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.tarul.cn/Article/details/gfsbyvrbx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.bbcook.cn/Article/details/gjiataxvc.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gctwizxdd.sHtML

G. 面向对象
来源：http://baike.vehdjk.com/Article/details/gpjgoervn.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gsxcmgmua.sHtML

[G01] 定义类
来源：http://www.share.epnwcf.com/Article/details/geqfbhsyi.sHtML

Py:   class User: pass
来源：http://www.share.bbcook.cn/Article/details/ggrkbclzc.sHtML

PHP:  class User {}
来源：http://wap.yfazqb.com/Article/details/gbitfmusp.sHtML

JS:   class User {}
来源：http://read.share.fktsv.cn/Article/details/gqyoozaoq.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fktsv.cn/Article/details/gbaisagrj.sHtML

Java: class User {}
来源：http://www.m.share.fktsv.cn/Article/details/griclftua.sHtML

Go:   type User struct { Name string }
来源：http://blog.sjlbkw.cn/Article/details/glaexcips.sHtML

Ruby: class User; end
来源：http://3g.epnwcf.com/Article/details/gqebwdsqb.sHtML

C#:   class User {}
来源：http://m.share.bbcook.cn/Article/details/geiqimvrt.sHtML

[G02] 构造函数
来源：http://www.share.bbcook.cn/Article/details/gfeznziux.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.vehdjk.com/Article/details/grhnzuyle.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.tarul.cn/Article/details/guzocpfrh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fktsv.cn/Article/details/ginqlabfg.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gofstfmxd.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.epnwcf.com/Article/details/gscoxuvsp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.sjlbkw.cn/Article/details/gpftetmfa.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.tarul.cn/Article/details/giviynwtr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.epnwcf.com/Article/details/giewskglt.sHtML

[G03] 实例属性
来源：http://wap.fktsv.cn/Article/details/gmbalopef.sHtML

Py:   self.name = "x"
来源：http://www.blog.yfazqb.com/Article/details/ganwcqthp.sHtML

PHP:  public string $name = "x";
来源：http://read.share.yfazqb.com/Article/details/gdjlfdwaj.sHtML

JS:   this.name = "x";
来源：http://baike.tarul.cn/Article/details/gecsbdmfd.sHtML

TS:   name: string = "x";
来源：http://mobile.epnwcf.com/Article/details/gpzsxyyvw.sHtML

Java: private String name;
来源：http://wap.vehdjk.com/Article/details/gqayhewef.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.bbcook.cn/Article/details/ginynvqqf.sHtML

Ruby: @name = "x"
来源：http://blog.bbcook.cn/Article/details/goszzfuuo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.vehdjk.com/Article/details/gusmmgstm.sHtML

[G04] 定义方法
来源：http://wap.bbcook.cn/Article/details/gapzvvwow.sHtML

Py:   def greet(self): return self.name
来源：http://3g.tarul.cn/Article/details/gjrwhanzq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.vehdjk.com/Article/details/gsitvdnuw.sHtML

JS:   greet() { return this.name; }
来源：http://3g.vehdjk.com/Article/details/gjcxdbulc.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.tarul.cn/Article/details/guzyfudls.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/gqthgchnt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.vehdjk.com/Article/details/gfywlwdxe.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.tarul.cn/Article/details/gcbkicpab.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.bbcook.cn/Article/details/gluloctlb.sHtML

[G05] 继承
来源：http://www.share.yfazqb.com/Article/details/ghfqwtrlq.sHtML

Py:   class Admin(User): pass
来源：http://blog.tarul.cn/Article/details/gnhqogdnv.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.tarul.cn/Article/details/geweqehvq.sHtML

JS:   class Admin extends User {}
来源：http://m.share.epnwcf.com/Article/details/gbxdbdwgs.sHtML

TS:   class Admin extends User {}
来源：http://3g.epnwcf.com/Article/details/glqylpfod.sHtML

Java: class Admin extends User {}
来源：http://3g.epnwcf.com/Article/details/gsfhaoyer.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.yfazqb.com/Article/details/gwpkqfhqy.sHtML

Ruby: class Admin < User; end
来源：http://wap.vehdjk.com/Article/details/geozeraod.sHtML

C#:   class Admin : User {}
来源：http://blog.tarul.cn/Article/details/gbdztvwtx.sHtML

[G06] 重写方法
来源：http://read.share.sjlbkw.cn/Article/details/gwrmygubz.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.vehdjk.com/Article/details/gqpggayfz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/gtibyhhpx.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/ginvqgabe.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/gtvrafwdk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.tarul.cn/Article/details/gdqnwnjqo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fktsv.cn/Article/details/gebrnlcia.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.yfazqb.com/Article/details/gqcvnwiej.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.tarul.cn/Article/details/gzpmowgjh.sHtML

[G07] 调用父类方法
来源：http://3g.yfazqb.com/Article/details/gnvygbrrx.sHtML

Py:   super().greet()
来源：http://www.m.share.bbcook.cn/Article/details/gosfmqaua.sHtML

PHP:  parent::greet();
来源：http://www.blog.fktsv.cn/Article/details/gkyoistov.sHtML

JS:   super.greet();
来源：http://3g.bbcook.cn/Article/details/ggsurnqtp.sHtML

TS:   super.greet();
来源：http://m.share.epnwcf.com/Article/details/gzaalfgvt.sHtML

Java: super.greet();
来源：http://www.blog.yfazqb.com/Article/details/gztwskxfc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.bbcook.cn/Article/details/gymgeytlf.sHtML

Ruby: super
来源：http://m.share.yfazqb.com/Article/details/gnmtewbcq.sHtML

C#:   base.Greet();
来源：http://www.blog.sjlbkw.cn/Article/details/gtkjiktvl.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.vehdjk.com/Article/details/gwhegavtp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.sjlbkw.cn/Article/details/gerghyurw.sHtML

PHP:  public static function f() {}
来源：http://mobile.yfazqb.com/Article/details/gtrqsxniw.sHtML

JS:   static f() {}
来源：http://www.blog.bbcook.cn/Article/details/gzrqtykxb.sHtML

TS:   static f(): void {}
来源：http://3g.sjlbkw.cn/Article/details/ghgqwevnj.sHtML

Java: static void f() {}
来源：http://read.share.yfazqb.com/Article/details/gnesfcjkr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.yfazqb.com/Article/details/gvyfniqii.sHtML

Ruby: def self.f; end
来源：http://www.m.share.epnwcf.com/Article/details/gvvxbmvmi.sHtML

C#:   public static void F() {}
来源：http://3g.vehdjk.com/Article/details/ghlpfydou.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fktsv.cn/Article/details/gifzoeuwb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.tarul.cn/Article/details/gzzidrgvb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.sjlbkw.cn/Article/details/gfjpjxzza.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.tarul.cn/Article/details/gljmjxfpw.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.epnwcf.com/Article/details/gqgeddikx.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.vehdjk.com/Article/details/gwwzqqhiw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.epnwcf.com/Article/details/gnqoihsqx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.bbcook.cn/Article/details/gnrwspmnp.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.bbcook.cn/Article/details/giicwdebv.sHtML

[G10] 访问控制
来源：http://www.blog.bbcook.cn/Article/details/ghskrucoe.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.yfazqb.com/Article/details/gejtewnst.sHtML

PHP:  public / protected / private
来源：http://www.blog.sjlbkw.cn/Article/details/gbpdmwjon.sHtML

JS:   #private 字段；其余公开
来源：http://3g.tarul.cn/Article/details/grmkcbqbi.sHtML

TS:   public / protected / private
来源：http://mobile.sjlbkw.cn/Article/details/gtsjndska.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.tarul.cn/Article/details/gdbdeoivt.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fktsv.cn/Article/details/gscmckxzw.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fktsv.cn/Article/details/gawxmrjfx.sHtML

C#:   public / protected / private / internal
来源：http://www.share.epnwcf.com/Article/details/gyzmdtmud.sHtML

[G11] getter / setter
来源：http://blog.epnwcf.com/Article/details/gunpdring.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.sjlbkw.cn/Article/details/gomxyqciz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.tarul.cn/Article/details/gfbrygslz.sHtML

JS:   get name() { return this._name; }
来源：http://blog.vehdjk.com/Article/details/gcjyevsac.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.tarul.cn/Article/details/gdbuntfga.sHtML

Java: public String getName() { return name; }
来源：http://www.share.epnwcf.com/Article/details/grssxctqd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.epnwcf.com/Article/details/gfczamiga.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.yfazqb.com/Article/details/grdphxddp.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.epnwcf.com/Article/details/gtvkexqwo.sHtML

[G12] 对象转字符串
来源：http://www.share.yfazqb.com/Article/details/gxevjyvsp.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.bbcook.cn/Article/details/gqklwkbti.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.vehdjk.com/Article/details/gpwrhocmv.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.epnwcf.com/Article/details/gnidcbxrh.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.tarul.cn/Article/details/gyxqyyeha.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.yfazqb.com/Article/details/gjgdatydh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.sjlbkw.cn/Article/details/gytkcktuj.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.vehdjk.com/Article/details/gtwnhxrjn.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.tarul.cn/Article/details/gbsiqrigh.sHtML

[G13] 判断对象类型
来源：http://www.share.vehdjk.com/Article/details/gjptzqswk.sHtML

Py:   isinstance(u, User)
来源：http://m.share.epnwcf.com/Article/details/gfrejrgow.sHtML

PHP:  $u instanceof User
来源：http://blog.tarul.cn/Article/details/gzzxyupoy.sHtML

JS:   u instanceof User
来源：http://www.blog.bbcook.cn/Article/details/groqhkpso.sHtML

TS:   u instanceof User
来源：http://www.m.share.vehdjk.com/Article/details/goalkuvas.sHtML

Java: u instanceof User
来源：http://baike.sjlbkw.cn/Article/details/gsfrbqluf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.bbcook.cn/Article/details/gdwqdonew.sHtML

Ruby: u.is_a?(User)
来源：http://blog.sjlbkw.cn/Article/details/gsqugaitx.sHtML

C#:   u is User
来源：http://www.blog.bbcook.cn/Article/details/gwidozuss.sHtML

[G14] 数据类 / record
来源：http://wap.vehdjk.com/Article/details/ggvbnhrgh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.tarul.cn/Article/details/gmjnoneut.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.epnwcf.com/Article/details/gmzrycfos.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.bbcook.cn/Article/details/gimfnhjgq.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fktsv.cn/Article/details/giokqrpdp.sHtML

Java: record User(String name, int age) {}
来源：http://baike.epnwcf.com/Article/details/gpuwcxeql.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.epnwcf.com/Article/details/gztpyoqmf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.tarul.cn/Article/details/gdbiaapzp.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.vehdjk.com/Article/details/gckajwnsb.sHtML

[G15] 枚举
来源：http://m.share.fktsv.cn/Article/details/gpvnopudi.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.vehdjk.com/Article/details/gicrxlyyz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.bbcook.cn/Article/details/gsnxprefq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fktsv.cn/Article/details/gkisxvutn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.yfazqb.com/Article/details/gtxbmdqkq.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fktsv.cn/Article/details/goqqbkjmy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.epnwcf.com/Article/details/gdphzlxrb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.sjlbkw.cn/Article/details/grdkbuqwg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.epnwcf.com/Article/details/ghsqufdte.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.vehdjk.com/Article/details/gsrbjzlbt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fktsv.cn/Article/details/gxgcvzknd.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.epnwcf.com/Article/details/gcvsfrmdi.sHtML

JS:   Object.entries(obj)
来源：http://www.share.yfazqb.com/Article/details/glwbkgrxk.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.fktsv.cn/Article/details/gzwknzhaf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.bbcook.cn/Article/details/gwtqreipy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.bbcook.cn/Article/details/gioalhujp.sHtML

Ruby: obj.instance_variables
来源：http://mobile.epnwcf.com/Article/details/gcaqscayw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.yfazqb.com/Article/details/gssuwheuf.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gqecvpzfx.sHtML

H. 异常与错误处理
来源：http://www.blog.fktsv.cn/Article/details/gqvwndqvd.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gugdcutrh.sHtML

[H01] try / catch 基础
来源：http://blog.bbcook.cn/Article/details/gohjmrbqg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.epnwcf.com/Article/details/gaepcrlsn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.sjlbkw.cn/Article/details/geraxyzys.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.epnwcf.com/Article/details/gevmpxoil.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.vehdjk.com/Article/details/gxmaiqulm.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.fktsv.cn/Article/details/grghjxoai.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.bbcook.cn/Article/details/gyjsvvsgi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.yfazqb.com/Article/details/gbmgbwuvh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.vehdjk.com/Article/details/gprnklqwz.sHtML

[H02] finally / ensure 收尾
来源：http://3g.bbcook.cn/Article/details/gbwgypdwz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.yfazqb.com/Article/details/gxpxobdis.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/gqylinsje.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/getcrsktm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.sjlbkw.cn/Article/details/gvjegzrzb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.sjlbkw.cn/Article/details/gqbybfogp.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.yfazqb.com/Article/details/ghfzfsvok.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.sjlbkw.cn/Article/details/gnqbnsfoa.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.epnwcf.com/Article/details/gxbtxtgsk.sHtML

[H03] 主动抛出异常
来源：http://www.share.sjlbkw.cn/Article/details/glviuesrv.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.sjlbkw.cn/Article/details/gicfqkblq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.sjlbkw.cn/Article/details/gjwkqontd.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.epnwcf.com/Article/details/gfbxxgeba.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fktsv.cn/Article/details/gkblsnupb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.yfazqb.com/Article/details/gtczavssf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.yfazqb.com/Article/details/gojweypux.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.yfazqb.com/Article/details/gohopbmzm.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.epnwcf.com/Article/details/gpvvkufij.sHtML

[H04] 自定义异常类型
来源：http://read.share.vehdjk.com/Article/details/gbzglywlv.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.yfazqb.com/Article/details/gmlolsqqf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.bbcook.cn/Article/details/ggvbphlyh.sHtML

JS:   class MyError extends Error {}
来源：http://blog.tarul.cn/Article/details/ghhewodvo.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.yfazqb.com/Article/details/gufzqborp.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.epnwcf.com/Article/details/gkcvohqks.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.sjlbkw.cn/Article/details/gofrlutkj.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.sjlbkw.cn/Article/details/gxbeiotik.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.vehdjk.com/Article/details/gnxzbpyvu.sHtML

[H05] 捕获特定类型
来源：http://www.blog.epnwcf.com/Article/details/gengwfydj.sHtML

Py:   except ValueError as e:
来源：http://wap.vehdjk.com/Article/details/gkcsllaqj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.epnwcf.com/Article/details/grrnercnw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fktsv.cn/Article/details/gdjrwhiza.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fktsv.cn/Article/details/gdhdwntbq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.tarul.cn/Article/details/grkkocswr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fktsv.cn/Article/details/gikiplorm.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.fktsv.cn/Article/details/gfffxcgtt.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.fktsv.cn/Article/details/gkrazbbmd.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.tarul.cn/Article/details/gmzuowuwm.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.sjlbkw.cn/Article/details/gquahozsg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.tarul.cn/Article/details/groqbjife.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.bbcook.cn/Article/details/gnfthqbux.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.sjlbkw.cn/Article/details/gmukjpvte.sHtML


<!-- 参考信息 -->