代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.yfazqb.com/Article/details/glexerbgg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.sjlbkw.cn/Article/details/gtuzkxoio.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.bbcook.cn/Article/details/gsflemmcr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.yfazqb.com/Article/details/gbacjgpqt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.bbcook.cn/Article/details/gwebhtoex.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.bbcook.cn/Article/details/gukuhvhqq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.tarul.cn/Article/details/gmwhupayg.sHtML

[F04] 追加写入文件
来源：http://mobile.sjlbkw.cn/Article/details/gwbezxktz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.tarul.cn/Article/details/gbhqdnofs.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.bbcook.cn/Article/details/gsphjxrwl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.yfazqb.com/Article/details/ggemjaupx.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.yfazqb.com/Article/details/gfmubehgk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.tarul.cn/Article/details/grbradszf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.yfazqb.com/Article/details/gqesvklfr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fktsv.cn/Article/details/gktqooell.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.tarul.cn/Article/details/gpmakztac.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.epnwcf.com/Article/details/ghlfzmhjv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.sjlbkw.cn/Article/details/gpbglxnjn.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.epnwcf.com/Article/details/gdcovqexm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gjzoraieg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gyrriihyv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.yfazqb.com/Article/details/gjzedrgkg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.tarul.cn/Article/details/gysdihqky.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gxvafejlv.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.epnwcf.com/Article/details/ggplgnuxg.sHtML

[F06] 删除文件
来源：http://www.m.share.yfazqb.com/Article/details/gtpkcbdco.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fktsv.cn/Article/details/gnxkjxuks.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.tarul.cn/Article/details/gapncheuj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gjcjaexal.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.epnwcf.com/Article/details/gmxlwqjft.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.bbcook.cn/Article/details/gzsgeeicf.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.yfazqb.com/Article/details/gjtfxygxt.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.bbcook.cn/Article/details/gwnlltsca.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gwonsatja.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.yfazqb.com/Article/details/gadgwdrmz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.sjlbkw.cn/Article/details/gynmjbljx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.vehdjk.com/Article/details/gyhpefdum.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.vehdjk.com/Article/details/gqqnprvdb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fktsv.cn/Article/details/gnpoupkmt.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.vehdjk.com/Article/details/gvveerqct.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.vehdjk.com/Article/details/gctzeyeiz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.bbcook.cn/Article/details/glajhcdcr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.bbcook.cn/Article/details/gxxpqxzze.sHtML

[F08] 遍历目录
来源：http://baike.bbcook.cn/Article/details/glfcahqhi.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.vehdjk.com/Article/details/gqeqanteg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fktsv.cn/Article/details/gzdjukdrf.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.yfazqb.com/Article/details/govkgtqts.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.epnwcf.com/Article/details/gdfwlebhw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fktsv.cn/Article/details/gwskmhpib.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fktsv.cn/Article/details/gwjmwnrpq.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.tarul.cn/Article/details/gmjysolfr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.bbcook.cn/Article/details/ggwuwhtor.sHtML

[F09] 获取文件大小
来源：http://www.share.sjlbkw.cn/Article/details/gykesmyef.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.vehdjk.com/Article/details/gzjyicffu.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gliudxeje.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.vehdjk.com/Article/details/gxioooxzl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.vehdjk.com/Article/details/goniuujkz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.bbcook.cn/Article/details/gtttmbcgz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.vehdjk.com/Article/details/ggzsqhdnp.sHtML

Ruby: File.size("a.txt")
来源：http://baike.yfazqb.com/Article/details/gcsvzhlbv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fktsv.cn/Article/details/gahnlijly.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.epnwcf.com/Article/details/ghlrwwglh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/gicczozut.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gvsrcidsw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.epnwcf.com/Article/details/gxrbnzmiq.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gmtfjtwrj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.epnwcf.com/Article/details/gczzacayx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gucexdexy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/gwjbhfshe.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/grbcqnjyp.sHtML

[F11] 复制与移动文件
来源：http://www.share.bbcook.cn/Article/details/gdsogipmo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gxbwmkyid.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fktsv.cn/Article/details/gkodjlokq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.yfazqb.com/Article/details/graxnfenv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gndzngpfi.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.vehdjk.com/Article/details/gppxvozbd.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fktsv.cn/Article/details/gjnrvghgu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.sjlbkw.cn/Article/details/gkbfgrcaq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.vehdjk.com/Article/details/goyggohga.sHtML

[F12] CSV 读写
来源：http://www.blog.bbcook.cn/Article/details/guslzkmqp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fktsv.cn/Article/details/gmzohajxh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.vehdjk.com/Article/details/gwyhtuppp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.sjlbkw.cn/Article/details/gnoeipbxk.sHtML

TS:   // 同上
来源：http://www.blog.fktsv.cn/Article/details/gqbqqbqdc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.tarul.cn/Article/details/gjwzzfvhr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.sjlbkw.cn/Article/details/gvefkadli.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.sjlbkw.cn/Article/details/gelnecuax.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.tarul.cn/Article/details/geqhunven.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gvbalrfvs.sHtML

G. 面向对象
来源：http://mobile.epnwcf.com/Article/details/gtpiefjsw.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gxsyyvavq.sHtML

[G01] 定义类
来源：http://m.share.bbcook.cn/Article/details/gduwihkcr.sHtML

Py:   class User: pass
来源：http://www.share.bbcook.cn/Article/details/gnajyzomu.sHtML

PHP:  class User {}
来源：http://www.share.vehdjk.com/Article/details/gshxdniuu.sHtML

JS:   class User {}
来源：http://read.share.fktsv.cn/Article/details/geakfcoqk.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.vehdjk.com/Article/details/ghhiqidqy.sHtML

Java: class User {}
来源：http://blog.yfazqb.com/Article/details/golrapkcx.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fktsv.cn/Article/details/ggjqiklqh.sHtML

Ruby: class User; end
来源：http://blog.vehdjk.com/Article/details/gjccqwusu.sHtML

C#:   class User {}
来源：http://www.share.sjlbkw.cn/Article/details/galyozdmt.sHtML

[G02] 构造函数
来源：http://3g.sjlbkw.cn/Article/details/gbsmjaeje.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.sjlbkw.cn/Article/details/gyhwgoout.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.sjlbkw.cn/Article/details/gwrniixqn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.bbcook.cn/Article/details/gglxalnid.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.vehdjk.com/Article/details/ggxbufgwj.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fktsv.cn/Article/details/gjuwifxir.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.bbcook.cn/Article/details/gprzhnhhj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.yfazqb.com/Article/details/gklxlsfwh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.tarul.cn/Article/details/gkhzytfij.sHtML

[G03] 实例属性
来源：http://mobile.sjlbkw.cn/Article/details/gfksyyxsj.sHtML

Py:   self.name = "x"
来源：http://3g.bbcook.cn/Article/details/gzdalsqcw.sHtML

PHP:  public string $name = "x";
来源：http://wap.vehdjk.com/Article/details/gdylkxptd.sHtML

JS:   this.name = "x";
来源：http://m.share.sjlbkw.cn/Article/details/gqjrgffwz.sHtML

TS:   name: string = "x";
来源：http://www.share.sjlbkw.cn/Article/details/getzdlsxr.sHtML

Java: private String name;
来源：http://baike.fktsv.cn/Article/details/gpmkigxlv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.epnwcf.com/Article/details/gpjisetho.sHtML

Ruby: @name = "x"
来源：http://mobile.bbcook.cn/Article/details/gddiizosj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.bbcook.cn/Article/details/gmbzndphm.sHtML

[G04] 定义方法
来源：http://3g.tarul.cn/Article/details/gbijbdfur.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.tarul.cn/Article/details/galsnmmjt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.epnwcf.com/Article/details/gilhginwh.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.vehdjk.com/Article/details/gkdgkncja.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.sjlbkw.cn/Article/details/gthjysvxf.sHtML

Java: String greet() { return name; }
来源：http://3g.tarul.cn/Article/details/gqfxjpbqb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.epnwcf.com/Article/details/gyopubuls.sHtML

Ruby: def greet; @name; end
来源：http://blog.vehdjk.com/Article/details/glyiggofy.sHtML

C#:   public string Greet() => Name;
来源：http://3g.sjlbkw.cn/Article/details/gxhyfmoux.sHtML

[G05] 继承
来源：http://baike.epnwcf.com/Article/details/gguzzlqob.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.yfazqb.com/Article/details/gnvigwqcc.sHtML

PHP:  class Admin extends User {}
来源：http://baike.tarul.cn/Article/details/gaayozbqt.sHtML

JS:   class Admin extends User {}
来源：http://wap.bbcook.cn/Article/details/gbclbisog.sHtML

TS:   class Admin extends User {}
来源：http://3g.epnwcf.com/Article/details/giqralwun.sHtML

Java: class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/gkjdeyknp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.yfazqb.com/Article/details/gmvacmice.sHtML

Ruby: class Admin < User; end
来源：http://m.share.yfazqb.com/Article/details/gdexkyjdd.sHtML

C#:   class Admin : User {}
来源：http://mobile.yfazqb.com/Article/details/gpjnazgxq.sHtML

[G06] 重写方法
来源：http://www.m.share.tarul.cn/Article/details/guvwyfzkk.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.bbcook.cn/Article/details/gvglbiqfo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.sjlbkw.cn/Article/details/gcaclmnyq.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.yfazqb.com/Article/details/gxwgljdgp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/ghlrsudcs.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fktsv.cn/Article/details/gooleuudw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.sjlbkw.cn/Article/details/gkftuljen.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.sjlbkw.cn/Article/details/gburlgmuk.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.epnwcf.com/Article/details/gdbveplxh.sHtML

[G07] 调用父类方法
来源：http://wap.epnwcf.com/Article/details/gfkluycyi.sHtML

Py:   super().greet()
来源：http://www.blog.vehdjk.com/Article/details/ghwglffch.sHtML

PHP:  parent::greet();
来源：http://m.share.sjlbkw.cn/Article/details/gpklxkpnw.sHtML

JS:   super.greet();
来源：http://www.m.share.fktsv.cn/Article/details/guwwcorpk.sHtML

TS:   super.greet();
来源：http://blog.yfazqb.com/Article/details/gqeggxufl.sHtML

Java: super.greet();
来源：http://3g.fktsv.cn/Article/details/gudsngbqp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.bbcook.cn/Article/details/gpetyuxes.sHtML

Ruby: super
来源：http://wap.epnwcf.com/Article/details/ghwjdzvqm.sHtML

C#:   base.Greet();
来源：http://3g.fktsv.cn/Article/details/gwjqqckve.sHtML

[G08] 静态方法与属性
来源：http://mobile.bbcook.cn/Article/details/gindsjmxa.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.yfazqb.com/Article/details/gelequizy.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gytarndsu.sHtML

JS:   static f() {}
来源：http://blog.sjlbkw.cn/Article/details/gfraecnrc.sHtML

TS:   static f(): void {}
来源：http://read.share.fktsv.cn/Article/details/gpwndxmak.sHtML

Java: static void f() {}
来源：http://www.share.epnwcf.com/Article/details/gksbiyenv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.yfazqb.com/Article/details/gwxftrzyq.sHtML

Ruby: def self.f; end
来源：http://wap.epnwcf.com/Article/details/gzdivndey.sHtML

C#:   public static void F() {}
来源：http://m.share.fktsv.cn/Article/details/gjkopgmsp.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.epnwcf.com/Article/details/gjlfzpydp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.bbcook.cn/Article/details/gjnrgdxfj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.bbcook.cn/Article/details/gbbesfzbq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.bbcook.cn/Article/details/gtsztdtcy.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fktsv.cn/Article/details/gsufmfydr.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.epnwcf.com/Article/details/grmxbysnd.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fktsv.cn/Article/details/gyoxixoax.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.yfazqb.com/Article/details/gpvdxasgb.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.sjlbkw.cn/Article/details/gcvbemhso.sHtML

[G10] 访问控制
来源：http://blog.vehdjk.com/Article/details/gpvpixuop.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.epnwcf.com/Article/details/guupnvvbi.sHtML

PHP:  public / protected / private
来源：http://www.m.share.vehdjk.com/Article/details/gkdcvoosw.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.tarul.cn/Article/details/gujafmiaj.sHtML

TS:   public / protected / private
来源：http://www.blog.sjlbkw.cn/Article/details/gfguaflrj.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.epnwcf.com/Article/details/gruqcashs.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.tarul.cn/Article/details/gwtfvenic.sHtML

Ruby: public / protected / private
来源：http://mobile.vehdjk.com/Article/details/gvkrckdva.sHtML

C#:   public / protected / private / internal
来源：http://read.share.tarul.cn/Article/details/gjilxevaz.sHtML

[G11] getter / setter
来源：http://m.share.tarul.cn/Article/details/gvmbrcqey.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.vehdjk.com/Article/details/gzsylcvkf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.bbcook.cn/Article/details/glxnqzgkd.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.yfazqb.com/Article/details/gbjgndlij.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.epnwcf.com/Article/details/gppcknene.sHtML

Java: public String getName() { return name; }
来源：http://blog.fktsv.cn/Article/details/gopcagetc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fktsv.cn/Article/details/grgqardmc.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.sjlbkw.cn/Article/details/grbgyxtux.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.tarul.cn/Article/details/gkhyuqzrf.sHtML

[G12] 对象转字符串
来源：http://wap.fktsv.cn/Article/details/gthkahqql.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fktsv.cn/Article/details/gsjcmhwbi.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.tarul.cn/Article/details/gjhisvawg.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.vehdjk.com/Article/details/gaopxzwvl.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.tarul.cn/Article/details/geuwjwsom.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gpxdcxlxv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.epnwcf.com/Article/details/gmgkltbaz.sHtML

Ruby: def to_s; @name; end
来源：http://wap.yfazqb.com/Article/details/gnvknbquv.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.yfazqb.com/Article/details/gedbqbkzy.sHtML

[G13] 判断对象类型
来源：http://blog.epnwcf.com/Article/details/gsyajjjdw.sHtML

Py:   isinstance(u, User)
来源：http://mobile.vehdjk.com/Article/details/gnyasxlfq.sHtML

PHP:  $u instanceof User
来源：http://www.blog.tarul.cn/Article/details/gjouicuut.sHtML

JS:   u instanceof User
来源：http://wap.fktsv.cn/Article/details/gyslugyyb.sHtML

TS:   u instanceof User
来源：http://www.share.bbcook.cn/Article/details/gkxymemco.sHtML

Java: u instanceof User
来源：http://www.m.share.sjlbkw.cn/Article/details/giskpoxie.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.sjlbkw.cn/Article/details/gjdnhjmrp.sHtML

Ruby: u.is_a?(User)
来源：http://wap.bbcook.cn/Article/details/ggvctykkk.sHtML

C#:   u is User
来源：http://baike.fktsv.cn/Article/details/gambidyel.sHtML

[G14] 数据类 / record
来源：http://www.share.tarul.cn/Article/details/gqdayivgv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.bbcook.cn/Article/details/ghiuaflfy.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.bbcook.cn/Article/details/gdegheffw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.bbcook.cn/Article/details/goohvfzbj.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.vehdjk.com/Article/details/gmnqlfoxm.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.yfazqb.com/Article/details/gprquzhui.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.vehdjk.com/Article/details/gdeuohysl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.vehdjk.com/Article/details/gguugmuvc.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.epnwcf.com/Article/details/gbgudedzb.sHtML

[G15] 枚举
来源：http://read.share.tarul.cn/Article/details/gnqouudhz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.epnwcf.com/Article/details/gyuxpcqqe.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.yfazqb.com/Article/details/glquxnhoz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.epnwcf.com/Article/details/gkbuylgxp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.vehdjk.com/Article/details/gtuhdkfig.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.vehdjk.com/Article/details/gksxhcnph.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.tarul.cn/Article/details/gfxnyabfc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.yfazqb.com/Article/details/gpxqwyykd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.epnwcf.com/Article/details/gytujvvtp.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.tarul.cn/Article/details/gvvvwxyyk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.sjlbkw.cn/Article/details/gdbisehur.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.sjlbkw.cn/Article/details/gpxozksek.sHtML

JS:   Object.entries(obj)
来源：http://blog.yfazqb.com/Article/details/gfizctmfn.sHtML

TS:   Object.entries(obj)
来源：http://baike.bbcook.cn/Article/details/gyjiurmlw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.bbcook.cn/Article/details/giowvmcbm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.epnwcf.com/Article/details/gqzkfpulh.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.sjlbkw.cn/Article/details/gcabxdoxo.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.epnwcf.com/Article/details/gotmcdpfp.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gsivsqqfj.sHtML

H. 异常与错误处理
来源：http://read.share.tarul.cn/Article/details/gprujtvwh.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gxdlbyvfh.sHtML

[H01] try / catch 基础
来源：http://www.m.share.sjlbkw.cn/Article/details/gazzpexpf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fktsv.cn/Article/details/gjtudebjj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.epnwcf.com/Article/details/ggnvxltjj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.bbcook.cn/Article/details/ghfozcuyq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.vehdjk.com/Article/details/gzxwkoarf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.epnwcf.com/Article/details/gsuouxqqp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.vehdjk.com/Article/details/getskfwdv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fktsv.cn/Article/details/gdobaaaik.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.vehdjk.com/Article/details/gusroopld.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.vehdjk.com/Article/details/gznpcjqtv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.epnwcf.com/Article/details/gwyiyvbmo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.yfazqb.com/Article/details/gimtzfwkv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/gffxddlui.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fktsv.cn/Article/details/glbsnfahk.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.tarul.cn/Article/details/gcjsbosub.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fktsv.cn/Article/details/gbgqxklqg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.vehdjk.com/Article/details/gbfqzhrrh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.sjlbkw.cn/Article/details/gngcljzix.sHtML

[H03] 主动抛出异常
来源：http://m.share.tarul.cn/Article/details/gzhdbjnbe.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.bbcook.cn/Article/details/grezizmit.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.epnwcf.com/Article/details/ghvberesy.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.bbcook.cn/Article/details/ghxugfuyd.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.tarul.cn/Article/details/gydafmjlg.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.vehdjk.com/Article/details/gexsfweoc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.yfazqb.com/Article/details/gfgtjiwyg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.yfazqb.com/Article/details/ggvzernje.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fktsv.cn/Article/details/gquoacgxb.sHtML

[H04] 自定义异常类型
来源：http://wap.vehdjk.com/Article/details/gjucszecx.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.epnwcf.com/Article/details/gofvdswkj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.bbcook.cn/Article/details/ghaolxzcx.sHtML

JS:   class MyError extends Error {}
来源：http://baike.bbcook.cn/Article/details/gggauhrhe.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.tarul.cn/Article/details/gyeomrsmx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fktsv.cn/Article/details/gjpulrexl.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fktsv.cn/Article/details/gxsctknll.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.tarul.cn/Article/details/gqdthhrat.sHtML

C#:   class MyException : Exception {}
来源：http://baike.epnwcf.com/Article/details/gujstpoxp.sHtML

[H05] 捕获特定类型
来源：http://m.share.yfazqb.com/Article/details/gqrjkydlm.sHtML

Py:   except ValueError as e:
来源：http://www.share.vehdjk.com/Article/details/gftehgvtx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.sjlbkw.cn/Article/details/gklbufdcc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.tarul.cn/Article/details/gqzmlnmes.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.bbcook.cn/Article/details/gmyrdjevf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.bbcook.cn/Article/details/gdsqpfqvv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.bbcook.cn/Article/details/giprjppih.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.vehdjk.com/Article/details/gofewelur.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.yfazqb.com/Article/details/ghertekjr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.yfazqb.com/Article/details/goaptsimb.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.sjlbkw.cn/Article/details/gomajagna.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.tarul.cn/Article/details/gxlemojjo.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.epnwcf.com/Article/details/glyjemdxw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fktsv.cn/Article/details/gjpuracoe.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.bbcook.cn/Article/details/gbmedckxd.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.yfazqb.com/Article/details/gpsncbopf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.bbcook.cn/Article/details/gjjlafzpg.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.vehdjk.com/Article/details/gbrvhstbm.sHtML

[H07] 断言
来源：http://read.share.vehdjk.com/Article/details/gkoeevsgg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.bbcook.cn/Article/details/gwmxcqhib.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.bbcook.cn/Article/details/gfksvghdg.sHtML

JS:   console.assert(x > 0);
来源：http://blog.bbcook.cn/Article/details/geievsqal.sHtML

TS:   console.assert(x > 0);
来源：http://3g.yfazqb.com/Article/details/ghmhermmp.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.yfazqb.com/Article/details/gmowfnipz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.epnwcf.com/Article/details/gwikolzen.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.yfazqb.com/Article/details/gvlejglvl.sHtML


<!-- 参考信息 -->