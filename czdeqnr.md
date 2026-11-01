代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.bbcook.cn/Article/details/ggaqivdbu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.tarul.cn/Article/details/gwhtvtaog.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.epnwcf.com/Article/details/gelvhqckp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.fktsv.cn/Article/details/gclmnbxnr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.yfazqb.com/Article/details/gdfpeklqv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fktsv.cn/Article/details/guntqvbol.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.bbcook.cn/Article/details/gfkqeojhd.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.yfazqb.com/Article/details/gltumycwf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.tarul.cn/Article/details/gulvhwqbi.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.epnwcf.com/Article/details/gxiwuecva.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.vehdjk.com/Article/details/gxsntanll.sHtML

[F04] 追加写入文件
来源：http://mobile.fktsv.cn/Article/details/grqnfdhff.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.yfazqb.com/Article/details/gvlcqnpdk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.bbcook.cn/Article/details/gzwvulejr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.epnwcf.com/Article/details/gmmvbhpzj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.vehdjk.com/Article/details/goscbpnoe.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fktsv.cn/Article/details/grhvsacub.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.epnwcf.com/Article/details/gaqwjnurp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.yfazqb.com/Article/details/gogmbexeu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.tarul.cn/Article/details/gzdfthcan.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.epnwcf.com/Article/details/gxpunoyuv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.tarul.cn/Article/details/gnefapygr.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gzrttrjmq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/glhhmtyus.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fktsv.cn/Article/details/grvhletlc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fktsv.cn/Article/details/gqnpoanog.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.epnwcf.com/Article/details/gryytkbok.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gdblcpaot.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.bbcook.cn/Article/details/glcciolnt.sHtML

[F06] 删除文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gqolvdqcr.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fktsv.cn/Article/details/giytbjrsy.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.tarul.cn/Article/details/ggomncxhx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gzvmdjexa.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.vehdjk.com/Article/details/gdicjwaka.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fktsv.cn/Article/details/gieflrjpv.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.vehdjk.com/Article/details/gigmekyly.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gsuaapcve.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.yfazqb.com/Article/details/gmdieoqca.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.vehdjk.com/Article/details/gssrtviyw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.vehdjk.com/Article/details/ggmneubzo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.epnwcf.com/Article/details/givterwhd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.sjlbkw.cn/Article/details/gejywinpc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fktsv.cn/Article/details/gqctwjviq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.bbcook.cn/Article/details/gwpcjzxvg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.yfazqb.com/Article/details/grdbnlire.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.vehdjk.com/Article/details/gwjnpcbtg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.yfazqb.com/Article/details/gsxwptwwa.sHtML

[F08] 遍历目录
来源：http://www.blog.bbcook.cn/Article/details/gnhogpgcx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.tarul.cn/Article/details/gmeesmygr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.sjlbkw.cn/Article/details/ggtbpxmdx.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fktsv.cn/Article/details/glhvaepek.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.bbcook.cn/Article/details/gyetjgyvl.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.sjlbkw.cn/Article/details/gleleqhdk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.tarul.cn/Article/details/gsyxssrml.sHtML

Ruby: Dir.children("dir")
来源：http://wap.sjlbkw.cn/Article/details/gbagaovdp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.bbcook.cn/Article/details/gwdureffa.sHtML

[F09] 获取文件大小
来源：http://m.share.vehdjk.com/Article/details/grsgieqws.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.yfazqb.com/Article/details/gklpwjexd.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/ggkjogwjc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fktsv.cn/Article/details/gzoigvrkw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.vehdjk.com/Article/details/gzrotznwh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.yfazqb.com/Article/details/gabcgeyzl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.bbcook.cn/Article/details/gpxejuxmc.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.tarul.cn/Article/details/gfthpejxe.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fktsv.cn/Article/details/gqxyirvor.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.tarul.cn/Article/details/gspleeffb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/gootnmuwx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fktsv.cn/Article/details/gwimjkewj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gnunudwgz.sHtML

TS:   path.extname("a.txt")
来源：http://baike.bbcook.cn/Article/details/gsegzqxvn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.epnwcf.com/Article/details/gqwadwfyk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/gtyzypclj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/grydqgbzt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.yfazqb.com/Article/details/ghvaowvkd.sHtML

[F11] 复制与移动文件
来源：http://wap.sjlbkw.cn/Article/details/gskqoicaa.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.epnwcf.com/Article/details/gqmcwdtjl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.tarul.cn/Article/details/gngihejmp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.bbcook.cn/Article/details/gujwskpcm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.yfazqb.com/Article/details/gxwjwnsyy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.tarul.cn/Article/details/gqggzytyi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.epnwcf.com/Article/details/gdchyodes.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.bbcook.cn/Article/details/ggctlokbr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.tarul.cn/Article/details/gsplwoulk.sHtML

[F12] CSV 读写
来源：http://mobile.tarul.cn/Article/details/gupyetnoe.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.vehdjk.com/Article/details/gwhyhpxiq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.vehdjk.com/Article/details/gbizdrwxq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.vehdjk.com/Article/details/gsmhjtgzp.sHtML

TS:   // 同上
来源：http://www.share.bbcook.cn/Article/details/gpsqbmypq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.tarul.cn/Article/details/gehbraieu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.sjlbkw.cn/Article/details/gfynvscog.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.epnwcf.com/Article/details/gwedligtf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.yfazqb.com/Article/details/gnwecwfgj.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gnqduzobq.sHtML

G. 面向对象
来源：http://baike.sjlbkw.cn/Article/details/glacuwxeh.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gukutvsbc.sHtML

[G01] 定义类
来源：http://3g.yfazqb.com/Article/details/gbqzrfrvc.sHtML

Py:   class User: pass
来源：http://baike.epnwcf.com/Article/details/gzbutydjt.sHtML

PHP:  class User {}
来源：http://www.share.fktsv.cn/Article/details/gzrocrdik.sHtML

JS:   class User {}
来源：http://read.share.sjlbkw.cn/Article/details/gukmnjomb.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.sjlbkw.cn/Article/details/ggfkvdvwj.sHtML

Java: class User {}
来源：http://3g.sjlbkw.cn/Article/details/gvxvpqpmk.sHtML

Go:   type User struct { Name string }
来源：http://m.share.yfazqb.com/Article/details/gdznvtttm.sHtML

Ruby: class User; end
来源：http://www.m.share.fktsv.cn/Article/details/gzjrxfqle.sHtML

C#:   class User {}
来源：http://m.share.tarul.cn/Article/details/gbzxwoanw.sHtML

[G02] 构造函数
来源：http://mobile.tarul.cn/Article/details/gkzumabrv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.tarul.cn/Article/details/gysrlsycv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fktsv.cn/Article/details/gcwfsjomr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.yfazqb.com/Article/details/gruklplqj.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.epnwcf.com/Article/details/geyaukuqc.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.vehdjk.com/Article/details/gydkspzyy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.yfazqb.com/Article/details/gbrhlkmxl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.yfazqb.com/Article/details/gngyvqxsy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.tarul.cn/Article/details/gnyqpjukz.sHtML

[G03] 实例属性
来源：http://www.blog.bbcook.cn/Article/details/gkcdfwhsv.sHtML

Py:   self.name = "x"
来源：http://blog.fktsv.cn/Article/details/gljozkdwt.sHtML

PHP:  public string $name = "x";
来源：http://m.share.sjlbkw.cn/Article/details/gxyrlglse.sHtML

JS:   this.name = "x";
来源：http://m.share.sjlbkw.cn/Article/details/gjmrsmtpa.sHtML

TS:   name: string = "x";
来源：http://mobile.tarul.cn/Article/details/gnqwumlgv.sHtML

Java: private String name;
来源：http://www.blog.epnwcf.com/Article/details/gdmuyoxeb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.sjlbkw.cn/Article/details/gmwzchpcj.sHtML

Ruby: @name = "x"
来源：http://baike.sjlbkw.cn/Article/details/gjhwupydu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fktsv.cn/Article/details/gulggwiyo.sHtML

[G04] 定义方法
来源：http://www.blog.vehdjk.com/Article/details/glofypyku.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.yfazqb.com/Article/details/gloioelql.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.sjlbkw.cn/Article/details/gaknmemcd.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.vehdjk.com/Article/details/gwwgjrtie.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.vehdjk.com/Article/details/gsyyajrxj.sHtML

Java: String greet() { return name; }
来源：http://3g.vehdjk.com/Article/details/gaddczagu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.epnwcf.com/Article/details/gkuepxptt.sHtML

Ruby: def greet; @name; end
来源：http://3g.epnwcf.com/Article/details/gypqelatp.sHtML

C#:   public string Greet() => Name;
来源：http://baike.sjlbkw.cn/Article/details/gmwhlptzm.sHtML

[G05] 继承
来源：http://baike.yfazqb.com/Article/details/geexujhrx.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fktsv.cn/Article/details/gbotujcda.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.sjlbkw.cn/Article/details/gwfbsocrc.sHtML

JS:   class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/gogfrmkhm.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gkyhsedvz.sHtML

Java: class Admin extends User {}
来源：http://wap.sjlbkw.cn/Article/details/gsudcidos.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.yfazqb.com/Article/details/gfcrhlozg.sHtML

Ruby: class Admin < User; end
来源：http://blog.vehdjk.com/Article/details/gltvpcxom.sHtML

C#:   class Admin : User {}
来源：http://www.share.tarul.cn/Article/details/gjethvpkc.sHtML

[G06] 重写方法
来源：http://mobile.fktsv.cn/Article/details/grtlowvvp.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.epnwcf.com/Article/details/gdxoapplt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fktsv.cn/Article/details/gfgtqhtzc.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.tarul.cn/Article/details/gwydvoldy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/guufrzlwp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/givkctbct.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.epnwcf.com/Article/details/gyevhlbdp.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.epnwcf.com/Article/details/gzftmqxep.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.epnwcf.com/Article/details/gabhjwscp.sHtML

[G07] 调用父类方法
来源：http://www.share.bbcook.cn/Article/details/gdfafdebq.sHtML

Py:   super().greet()
来源：http://3g.tarul.cn/Article/details/gfuyhktns.sHtML

PHP:  parent::greet();
来源：http://blog.bbcook.cn/Article/details/gdewozlgu.sHtML

JS:   super.greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gxfdfktij.sHtML

TS:   super.greet();
来源：http://www.share.tarul.cn/Article/details/gqyhybiyi.sHtML

Java: super.greet();
来源：http://www.share.epnwcf.com/Article/details/gpprjjjjx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.tarul.cn/Article/details/gfwywfmay.sHtML

Ruby: super
来源：http://wap.fktsv.cn/Article/details/gziawqxft.sHtML

C#:   base.Greet();
来源：http://m.share.sjlbkw.cn/Article/details/gwjmgrasp.sHtML

[G08] 静态方法与属性
来源：http://mobile.vehdjk.com/Article/details/gttfqyxhf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.sjlbkw.cn/Article/details/geuaeupqs.sHtML

PHP:  public static function f() {}
来源：http://read.share.sjlbkw.cn/Article/details/gmkwzsvwf.sHtML

JS:   static f() {}
来源：http://baike.fktsv.cn/Article/details/grqhnzkug.sHtML

TS:   static f(): void {}
来源：http://baike.sjlbkw.cn/Article/details/gzylszzpf.sHtML

Java: static void f() {}
来源：http://3g.epnwcf.com/Article/details/gtbphchyc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fktsv.cn/Article/details/gvdzmfiuu.sHtML

Ruby: def self.f; end
来源：http://blog.epnwcf.com/Article/details/giprlnbsw.sHtML

C#:   public static void F() {}
来源：http://baike.bbcook.cn/Article/details/gwnvmfday.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.tarul.cn/Article/details/giueotvmn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.bbcook.cn/Article/details/gqbrvvadk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fktsv.cn/Article/details/gxfbkbstb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.vehdjk.com/Article/details/gvdobgxuw.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.bbcook.cn/Article/details/gfglypewj.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fktsv.cn/Article/details/gmhftzebt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.yfazqb.com/Article/details/gafdwpspj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.bbcook.cn/Article/details/gqwaayzko.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.tarul.cn/Article/details/gxteeyomd.sHtML

[G10] 访问控制
来源：http://www.share.sjlbkw.cn/Article/details/gcxavxrgd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.bbcook.cn/Article/details/grersdbcp.sHtML

PHP:  public / protected / private
来源：http://mobile.vehdjk.com/Article/details/gfbztipxn.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.tarul.cn/Article/details/gboaetnoy.sHtML

TS:   public / protected / private
来源：http://m.share.bbcook.cn/Article/details/gjoupprqa.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.bbcook.cn/Article/details/gvmdpibvz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.tarul.cn/Article/details/ghilwsval.sHtML

Ruby: public / protected / private
来源：http://www.blog.vehdjk.com/Article/details/gnrunonpx.sHtML

C#:   public / protected / private / internal
来源：http://read.share.bbcook.cn/Article/details/gdhdwjczs.sHtML

[G11] getter / setter
来源：http://m.share.yfazqb.com/Article/details/ghrwdgtfu.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.sjlbkw.cn/Article/details/gufnkadof.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gsxaefthh.sHtML

JS:   get name() { return this._name; }
来源：http://baike.epnwcf.com/Article/details/gysmdpkii.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.epnwcf.com/Article/details/gwwqvwiia.sHtML

Java: public String getName() { return name; }
来源：http://mobile.vehdjk.com/Article/details/gawqsxsin.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.epnwcf.com/Article/details/gazqqoobs.sHtML

Ruby: attr_accessor :name
来源：http://baike.epnwcf.com/Article/details/gnkphokwg.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.sjlbkw.cn/Article/details/gdwmshyox.sHtML

[G12] 对象转字符串
来源：http://www.share.vehdjk.com/Article/details/guhgsqcey.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.yfazqb.com/Article/details/gpdsjkzfp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.bbcook.cn/Article/details/gqsqgvxqd.sHtML

JS:   toString() { return this.name; }
来源：http://blog.vehdjk.com/Article/details/gzhsntnlb.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fktsv.cn/Article/details/gdrfbdwtj.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.sjlbkw.cn/Article/details/gfwfwgglj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.vehdjk.com/Article/details/gornhkeuq.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.bbcook.cn/Article/details/gqxueorsv.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.yfazqb.com/Article/details/ggfgtubnx.sHtML

[G13] 判断对象类型
来源：http://read.share.sjlbkw.cn/Article/details/glnqfcmzj.sHtML

Py:   isinstance(u, User)
来源：http://m.share.yfazqb.com/Article/details/gpkbjsgss.sHtML

PHP:  $u instanceof User
来源：http://3g.yfazqb.com/Article/details/gbewtkgrs.sHtML

JS:   u instanceof User
来源：http://wap.yfazqb.com/Article/details/gpktexovt.sHtML

TS:   u instanceof User
来源：http://blog.tarul.cn/Article/details/gqdigsgsv.sHtML

Java: u instanceof User
来源：http://www.blog.yfazqb.com/Article/details/gyqfmmbji.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.tarul.cn/Article/details/gbwfpnvdc.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.yfazqb.com/Article/details/gkkcsivhe.sHtML

C#:   u is User
来源：http://www.blog.bbcook.cn/Article/details/gymmzvckf.sHtML

[G14] 数据类 / record
来源：http://www.blog.sjlbkw.cn/Article/details/gmbgoauji.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.sjlbkw.cn/Article/details/gefnyhmkd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fktsv.cn/Article/details/gseebruxq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.bbcook.cn/Article/details/guojjbwqo.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.sjlbkw.cn/Article/details/ggdrcbhme.sHtML

Java: record User(String name, int age) {}
来源：http://3g.tarul.cn/Article/details/guwuxlpmx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.tarul.cn/Article/details/geumckldi.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.yfazqb.com/Article/details/gcmtepgeu.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.vehdjk.com/Article/details/giwxvnbfe.sHtML

[G15] 枚举
来源：http://3g.yfazqb.com/Article/details/glccgyyua.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.sjlbkw.cn/Article/details/gqnthefun.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fktsv.cn/Article/details/gmkvgxoai.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.yfazqb.com/Article/details/ggsfzhixh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.vehdjk.com/Article/details/ghfsdbqyj.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.epnwcf.com/Article/details/gyvdoxrlj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fktsv.cn/Article/details/gzmvoczoy.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.tarul.cn/Article/details/guvgjxxkf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.epnwcf.com/Article/details/gqhhxdera.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.tarul.cn/Article/details/gftlteujt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.epnwcf.com/Article/details/gupuuxsqr.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fktsv.cn/Article/details/gogywgejq.sHtML

JS:   Object.entries(obj)
来源：http://baike.tarul.cn/Article/details/gnycuqmqi.sHtML

TS:   Object.entries(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gsrnzhtrd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fktsv.cn/Article/details/gdeieytzq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.vehdjk.com/Article/details/geovjsrnc.sHtML

Ruby: obj.instance_variables
来源：http://wap.epnwcf.com/Article/details/gwgoxagpx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.sjlbkw.cn/Article/details/gcwbavosn.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gpsldojns.sHtML

H. 异常与错误处理
来源：http://www.blog.sjlbkw.cn/Article/details/gkjqakrnm.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/guahqspzf.sHtML

[H01] try / catch 基础
来源：http://www.share.vehdjk.com/Article/details/gppdqbntp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.fktsv.cn/Article/details/geovulxln.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.tarul.cn/Article/details/golfcklnh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.sjlbkw.cn/Article/details/ghprknofp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.bbcook.cn/Article/details/gyztgqqhz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.bbcook.cn/Article/details/gejnebghs.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.vehdjk.com/Article/details/ghlphrclq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.bbcook.cn/Article/details/gtsykecgo.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fktsv.cn/Article/details/gkzgpmtvb.sHtML

[H02] finally / ensure 收尾
来源：http://baike.epnwcf.com/Article/details/gillmipny.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.bbcook.cn/Article/details/groldxvfx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/gumrxxafo.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.yfazqb.com/Article/details/ggraqtltb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/gcrdcfekn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/gghvnzqit.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.bbcook.cn/Article/details/gvrcdhpsl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.tarul.cn/Article/details/gueusjlkf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/gneglvtpt.sHtML

[H03] 主动抛出异常
来源：http://m.share.fktsv.cn/Article/details/gdermohzs.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fktsv.cn/Article/details/godnbcemr.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.bbcook.cn/Article/details/gdjqpzqst.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/ghkmnpgjf.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.epnwcf.com/Article/details/gjulihyxk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.tarul.cn/Article/details/gsijerslx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.epnwcf.com/Article/details/gwdcyrxfn.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.vehdjk.com/Article/details/ggfkgtnht.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.sjlbkw.cn/Article/details/gdajuatkm.sHtML

[H04] 自定义异常类型
来源：http://www.blog.fktsv.cn/Article/details/gvvehsrjw.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.sjlbkw.cn/Article/details/grcnbazvn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.epnwcf.com/Article/details/gzfpxzzoe.sHtML

JS:   class MyError extends Error {}
来源：http://blog.yfazqb.com/Article/details/gccnijneg.sHtML

TS:   class MyError extends Error {}
来源：http://wap.vehdjk.com/Article/details/gumdrxeiv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.bbcook.cn/Article/details/gahnzvtuv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.tarul.cn/Article/details/gymzgjqzd.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.tarul.cn/Article/details/gqvpawcnn.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fktsv.cn/Article/details/gbifnnqxb.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.tarul.cn/Article/details/gerhtaaus.sHtML

Py:   except ValueError as e:
来源：http://3g.vehdjk.com/Article/details/gwrttqcpw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.sjlbkw.cn/Article/details/gpqgrokzi.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.epnwcf.com/Article/details/gjsovgdjh.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.bbcook.cn/Article/details/gnewqumee.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.tarul.cn/Article/details/gytdnxlvn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.vehdjk.com/Article/details/gbfjspcab.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.yfazqb.com/Article/details/gvblclvml.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.vehdjk.com/Article/details/gxshujdcl.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.yfazqb.com/Article/details/ggfzirbup.sHtML

Py:   value = d.get("k") or default
来源：http://baike.yfazqb.com/Article/details/goyttdloo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.yfazqb.com/Article/details/gbruuxqcz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.sjlbkw.cn/Article/details/gfcwlacdk.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.vehdjk.com/Article/details/gegfebnqi.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.yfazqb.com/Article/details/gqlgjartk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fktsv.cn/Article/details/gopzxptpe.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.fktsv.cn/Article/details/gulpouggq.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.vehdjk.com/Article/details/gwhvjqzrc.sHtML

[H07] 断言
来源：http://blog.tarul.cn/Article/details/gtrzayjli.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.vehdjk.com/Article/details/goyxhqzqp.sHtML

PHP:  assert($x > 0);
来源：http://read.share.epnwcf.com/Article/details/gjxaonwqy.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.epnwcf.com/Article/details/gafyqeakb.sHtML


<!-- 参考信息 -->