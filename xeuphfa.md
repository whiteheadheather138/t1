代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gkyaktblc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fktsv.cn/Article/details/gvsadbozm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/gqfkobtkn.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvdxzlsmf.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.tarul.cn/Article/details/guiroqpkr.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gisejxgfm.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.vehdjk.com/Article/details/gfudpovcl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.vehdjk.com/Article/details/gvxkjlart.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.yfazqb.com/Article/details/guryzmeej.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.bbcook.cn/Article/details/gibhxktit.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.bbcook.cn/Article/details/gagotbakl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.yfazqb.com/Article/details/gothhbqrz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.tarul.cn/Article/details/grlkkwteu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.bbcook.cn/Article/details/ggouuaivf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.sjlbkw.cn/Article/details/gbyqglfez.sHtML

[F08] 遍历目录
来源：http://www.share.epnwcf.com/Article/details/ghjjrlsow.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.bbcook.cn/Article/details/gblzzulqz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.bbcook.cn/Article/details/gurrfpbzc.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.sjlbkw.cn/Article/details/gnkdtlsgt.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fktsv.cn/Article/details/gsjxaczss.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.vehdjk.com/Article/details/gxdnrrgvq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.sjlbkw.cn/Article/details/gzgzbgdeu.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fktsv.cn/Article/details/gyygrhalq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.vehdjk.com/Article/details/gqtjqkgfl.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fktsv.cn/Article/details/gnvjgudbd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.vehdjk.com/Article/details/gfxzfytrc.sHtML

PHP:  filesize("a.txt");
来源：http://blog.yfazqb.com/Article/details/gjorurrsh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.epnwcf.com/Article/details/gqtpgbtix.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fktsv.cn/Article/details/gmyrttamz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.tarul.cn/Article/details/gglpeloal.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.vehdjk.com/Article/details/ghsolatts.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gzpohwaoa.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.bbcook.cn/Article/details/girlepgbu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fktsv.cn/Article/details/gfxmlwomm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/gcucarabp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.vehdjk.com/Article/details/gajhfpumm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.tarul.cn/Article/details/gytkwcjur.sHtML

TS:   path.extname("a.txt")
来源：http://baike.yfazqb.com/Article/details/gfqaweska.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.yfazqb.com/Article/details/gaktjgefw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/gouhnkgbv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gglsyquir.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gkvquqolx.sHtML

[F11] 复制与移动文件
来源：http://baike.tarul.cn/Article/details/gtwqvifxm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.vehdjk.com/Article/details/ghgsqipdt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.yfazqb.com/Article/details/gqeoxzszr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.bbcook.cn/Article/details/gleihwtlx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.sjlbkw.cn/Article/details/gevrvvnsn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.sjlbkw.cn/Article/details/gdcwjsxwh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.yfazqb.com/Article/details/gkcyvyqlo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.yfazqb.com/Article/details/ggtkjeutd.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.yfazqb.com/Article/details/gdrompsvw.sHtML

[F12] CSV 读写
来源：http://m.share.vehdjk.com/Article/details/gtcnoirxx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.sjlbkw.cn/Article/details/gesqstrud.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.yfazqb.com/Article/details/gqkmwbsag.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.yfazqb.com/Article/details/gjqqqbexi.sHtML

TS:   // 同上
来源：http://m.share.vehdjk.com/Article/details/gndjypggh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.bbcook.cn/Article/details/gpkhuwjli.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.vehdjk.com/Article/details/gcnrkxxnz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.tarul.cn/Article/details/ghtgoohlr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.vehdjk.com/Article/details/gapwdzynu.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/geajjlczl.sHtML

G. 面向对象
来源：http://m.share.fktsv.cn/Article/details/ghitiferw.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/glynfvkqk.sHtML

[G01] 定义类
来源：http://www.m.share.fktsv.cn/Article/details/gphfnvaai.sHtML

Py:   class User: pass
来源：http://mobile.tarul.cn/Article/details/gacjpdinb.sHtML

PHP:  class User {}
来源：http://baike.bbcook.cn/Article/details/gveiyhbzy.sHtML

JS:   class User {}
来源：http://www.share.sjlbkw.cn/Article/details/gwmdxtmzo.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.vehdjk.com/Article/details/gynkizwcu.sHtML

Java: class User {}
来源：http://mobile.fktsv.cn/Article/details/gaktudubg.sHtML

Go:   type User struct { Name string }
来源：http://baike.epnwcf.com/Article/details/gbwopfsva.sHtML

Ruby: class User; end
来源：http://m.share.yfazqb.com/Article/details/gzzyktiaa.sHtML

C#:   class User {}
来源：http://wap.bbcook.cn/Article/details/giymfzpqu.sHtML

[G02] 构造函数
来源：http://www.blog.fktsv.cn/Article/details/gzeubrlzu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.vehdjk.com/Article/details/ghpilukwt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fktsv.cn/Article/details/gtvengygz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fktsv.cn/Article/details/gphxxgmgw.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.epnwcf.com/Article/details/gohvhvqcr.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.bbcook.cn/Article/details/gpswaygwa.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.tarul.cn/Article/details/gbthdrvnq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.epnwcf.com/Article/details/grjnrqrlp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.tarul.cn/Article/details/gcnffqwej.sHtML

[G03] 实例属性
来源：http://wap.vehdjk.com/Article/details/gljuhphse.sHtML

Py:   self.name = "x"
来源：http://blog.vehdjk.com/Article/details/glpptcqxd.sHtML

PHP:  public string $name = "x";
来源：http://wap.vehdjk.com/Article/details/gpjcvpqya.sHtML

JS:   this.name = "x";
来源：http://www.share.sjlbkw.cn/Article/details/geogluzhf.sHtML

TS:   name: string = "x";
来源：http://read.share.sjlbkw.cn/Article/details/gneoiluec.sHtML

Java: private String name;
来源：http://3g.fktsv.cn/Article/details/gviomvmgm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fktsv.cn/Article/details/gzgusjyfz.sHtML

Ruby: @name = "x"
来源：http://blog.fktsv.cn/Article/details/gznryteko.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.vehdjk.com/Article/details/gxkdcqxgx.sHtML

[G04] 定义方法
来源：http://wap.sjlbkw.cn/Article/details/gqtugiizm.sHtML

Py:   def greet(self): return self.name
来源：http://3g.sjlbkw.cn/Article/details/gjvumaccd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.sjlbkw.cn/Article/details/gqhaqpmdr.sHtML

JS:   greet() { return this.name; }
来源：http://baike.bbcook.cn/Article/details/gaugbrnla.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fktsv.cn/Article/details/glovvxsyj.sHtML

Java: String greet() { return name; }
来源：http://mobile.fktsv.cn/Article/details/gdganiedm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.yfazqb.com/Article/details/gdvvsxhma.sHtML

Ruby: def greet; @name; end
来源：http://baike.epnwcf.com/Article/details/gtwwanbws.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.bbcook.cn/Article/details/gfasaayam.sHtML

[G05] 继承
来源：http://blog.bbcook.cn/Article/details/glsgcpvcl.sHtML

Py:   class Admin(User): pass
来源：http://baike.tarul.cn/Article/details/gvqwfbzvs.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gdmqnhqpd.sHtML

JS:   class Admin extends User {}
来源：http://www.share.yfazqb.com/Article/details/guvoulhyy.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.vehdjk.com/Article/details/gpafnvutf.sHtML

Java: class Admin extends User {}
来源：http://read.share.epnwcf.com/Article/details/gpebezymi.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.vehdjk.com/Article/details/ghyitrqwl.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fktsv.cn/Article/details/gtuywzsly.sHtML

C#:   class Admin : User {}
来源：http://blog.sjlbkw.cn/Article/details/guyfxxiks.sHtML

[G06] 重写方法
来源：http://blog.fktsv.cn/Article/details/gpyonadpa.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fktsv.cn/Article/details/gzbktbfum.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/gnpguvolz.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/gpvvghnpl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gblopbvfp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fktsv.cn/Article/details/gbifpppqn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.yfazqb.com/Article/details/gztmvnzud.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.vehdjk.com/Article/details/ghktvnhaz.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.bbcook.cn/Article/details/gmeufakop.sHtML

[G07] 调用父类方法
来源：http://www.share.sjlbkw.cn/Article/details/grlxxmybe.sHtML

Py:   super().greet()
来源：http://wap.bbcook.cn/Article/details/gfpsyajih.sHtML

PHP:  parent::greet();
来源：http://m.share.yfazqb.com/Article/details/gmexhwgsk.sHtML

JS:   super.greet();
来源：http://read.share.yfazqb.com/Article/details/gaapadnts.sHtML

TS:   super.greet();
来源：http://www.m.share.bbcook.cn/Article/details/ggxprbqlk.sHtML

Java: super.greet();
来源：http://www.share.epnwcf.com/Article/details/gpmemsduo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.vehdjk.com/Article/details/gkeuenxhg.sHtML

Ruby: super
来源：http://blog.yfazqb.com/Article/details/gmhtabwxr.sHtML

C#:   base.Greet();
来源：http://3g.fktsv.cn/Article/details/ggpnojfkt.sHtML

[G08] 静态方法与属性
来源：http://www.blog.bbcook.cn/Article/details/gdcubbplv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.bbcook.cn/Article/details/gotbmiwfl.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.vehdjk.com/Article/details/gdzdwkzzf.sHtML

JS:   static f() {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gknrhmafi.sHtML

TS:   static f(): void {}
来源：http://3g.yfazqb.com/Article/details/gqpykfvtt.sHtML

Java: static void f() {}
来源：http://www.m.share.yfazqb.com/Article/details/gcvoxjrxp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.sjlbkw.cn/Article/details/gfthvamhx.sHtML

Ruby: def self.f; end
来源：http://www.blog.sjlbkw.cn/Article/details/gugxdhkuv.sHtML

C#:   public static void F() {}
来源：http://blog.tarul.cn/Article/details/gegknqcxx.sHtML

[G09] 接口 / 抽象类
来源：http://blog.sjlbkw.cn/Article/details/gpqbkpuwj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.vehdjk.com/Article/details/gfnemziay.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.sjlbkw.cn/Article/details/gzdcjlqik.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.sjlbkw.cn/Article/details/gkwkoembp.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.sjlbkw.cn/Article/details/gkhnusaag.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fktsv.cn/Article/details/guryzwplm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fktsv.cn/Article/details/gurjuctuz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.sjlbkw.cn/Article/details/gbfrhuqui.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.tarul.cn/Article/details/ggtjurvlx.sHtML

[G10] 访问控制
来源：http://www.blog.fktsv.cn/Article/details/gktmkdtjw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fktsv.cn/Article/details/gniwwdant.sHtML

PHP:  public / protected / private
来源：http://mobile.epnwcf.com/Article/details/gmoucusti.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.bbcook.cn/Article/details/gfcaqusly.sHtML

TS:   public / protected / private
来源：http://mobile.sjlbkw.cn/Article/details/gucvpwxzc.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.vehdjk.com/Article/details/gydgghaki.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fktsv.cn/Article/details/gljzcicnx.sHtML

Ruby: public / protected / private
来源：http://www.blog.vehdjk.com/Article/details/gpylbcben.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.vehdjk.com/Article/details/glegoedro.sHtML

[G11] getter / setter
来源：http://www.blog.vehdjk.com/Article/details/ghiivylvy.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.vehdjk.com/Article/details/gspigpcfl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.tarul.cn/Article/details/glulkotlh.sHtML

JS:   get name() { return this._name; }
来源：http://3g.yfazqb.com/Article/details/gutulhxtj.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.epnwcf.com/Article/details/gqzmsenbl.sHtML

Java: public String getName() { return name; }
来源：http://3g.fktsv.cn/Article/details/gppchiquh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.epnwcf.com/Article/details/gjlgcdgjt.sHtML

Ruby: attr_accessor :name
来源：http://wap.fktsv.cn/Article/details/gsccdyppx.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.yfazqb.com/Article/details/gfdpkxxat.sHtML

[G12] 对象转字符串
来源：http://www.blog.bbcook.cn/Article/details/gghtalbfr.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.yfazqb.com/Article/details/gzetjpzwv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.epnwcf.com/Article/details/guouzztsu.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/gibwvxmac.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.yfazqb.com/Article/details/gorvyueqj.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.yfazqb.com/Article/details/gabukumom.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.bbcook.cn/Article/details/gjrngmgrf.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.bbcook.cn/Article/details/gndhutsgr.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fktsv.cn/Article/details/gshfujcdn.sHtML

[G13] 判断对象类型
来源：http://www.m.share.sjlbkw.cn/Article/details/ghsxudmxu.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.yfazqb.com/Article/details/grgdyoadn.sHtML

PHP:  $u instanceof User
来源：http://wap.epnwcf.com/Article/details/gszoilyyd.sHtML

JS:   u instanceof User
来源：http://m.share.sjlbkw.cn/Article/details/grvdqnouq.sHtML

TS:   u instanceof User
来源：http://baike.fktsv.cn/Article/details/gmpspcvcf.sHtML

Java: u instanceof User
来源：http://www.blog.bbcook.cn/Article/details/gwifaplzh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.sjlbkw.cn/Article/details/gnmofdjvi.sHtML

Ruby: u.is_a?(User)
来源：http://blog.bbcook.cn/Article/details/gofuxodvp.sHtML

C#:   u is User
来源：http://wap.vehdjk.com/Article/details/gxzisyjyo.sHtML

[G14] 数据类 / record
来源：http://3g.sjlbkw.cn/Article/details/gtcecxvqh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.yfazqb.com/Article/details/gnpowqfwo.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.bbcook.cn/Article/details/gktfsyxxs.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.tarul.cn/Article/details/geguwdqqp.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.epnwcf.com/Article/details/glkoviulw.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.tarul.cn/Article/details/gqjzfwxjv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.sjlbkw.cn/Article/details/gknnwmjnu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fktsv.cn/Article/details/gvggadpeo.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fktsv.cn/Article/details/goncryego.sHtML

[G15] 枚举
来源：http://m.share.sjlbkw.cn/Article/details/gvilxqwdg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.tarul.cn/Article/details/gzdgcvcus.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.yfazqb.com/Article/details/griuzmerp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.yfazqb.com/Article/details/gfcqdkqnx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.vehdjk.com/Article/details/gifsdrsys.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.yfazqb.com/Article/details/ghtejtnik.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.vehdjk.com/Article/details/gngscglgj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.epnwcf.com/Article/details/gxhdzncfq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.epnwcf.com/Article/details/gsbvpdeae.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.bbcook.cn/Article/details/gznakznju.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fktsv.cn/Article/details/gtieixckz.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.vehdjk.com/Article/details/gfquznimq.sHtML

JS:   Object.entries(obj)
来源：http://baike.epnwcf.com/Article/details/gttfxwxfx.sHtML

TS:   Object.entries(obj)
来源：http://m.share.bbcook.cn/Article/details/gsuouakbu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fktsv.cn/Article/details/gaydqfbrf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.bbcook.cn/Article/details/gkxufugsx.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.yfazqb.com/Article/details/gocbyntlz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.vehdjk.com/Article/details/gejtvbhbz.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gxhknaifd.sHtML

H. 异常与错误处理
来源：http://www.blog.sjlbkw.cn/Article/details/gytqrbjqs.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gsvarmntr.sHtML

[H01] try / catch 基础
来源：http://www.blog.vehdjk.com/Article/details/gzqwxtgtu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.tarul.cn/Article/details/gqbpucutv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.tarul.cn/Article/details/gscvyglne.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.vehdjk.com/Article/details/gplnmtroc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.epnwcf.com/Article/details/gozqrxdtp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fktsv.cn/Article/details/gksbczewe.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.yfazqb.com/Article/details/gkndpwjqw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.vehdjk.com/Article/details/gpauvdvbm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.yfazqb.com/Article/details/gmuphxqeg.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.epnwcf.com/Article/details/gxwtddqgs.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.vehdjk.com/Article/details/gkwckfsse.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fktsv.cn/Article/details/gwsjosxkq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.yfazqb.com/Article/details/gnqqkypiy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.tarul.cn/Article/details/gqeieyqtb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.vehdjk.com/Article/details/gztixfogo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.yfazqb.com/Article/details/glhunwbup.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fktsv.cn/Article/details/gpzlaifiu.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.tarul.cn/Article/details/gebafzabx.sHtML

[H03] 主动抛出异常
来源：http://baike.fktsv.cn/Article/details/gumvcgtbh.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.fktsv.cn/Article/details/gggnetpvd.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.epnwcf.com/Article/details/guobrmtea.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.tarul.cn/Article/details/gessigzzd.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.sjlbkw.cn/Article/details/gwiojikny.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.fktsv.cn/Article/details/gwkyybhtg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.yfazqb.com/Article/details/gvclmkcfv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.epnwcf.com/Article/details/gwarfbizv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.yfazqb.com/Article/details/gzpcrbstf.sHtML

[H04] 自定义异常类型
来源：http://wap.yfazqb.com/Article/details/glrckogxq.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.bbcook.cn/Article/details/gytvzxolk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.yfazqb.com/Article/details/gkqfjwiya.sHtML

JS:   class MyError extends Error {}
来源：http://baike.tarul.cn/Article/details/gahgyinog.sHtML

TS:   class MyError extends Error {}
来源：http://wap.yfazqb.com/Article/details/gwsuoodun.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.yfazqb.com/Article/details/gfaamahfl.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.tarul.cn/Article/details/ghbkuhjbs.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.sjlbkw.cn/Article/details/gnlupeqvm.sHtML

C#:   class MyException : Exception {}
来源：http://wap.yfazqb.com/Article/details/gwgoxauxo.sHtML

[H05] 捕获特定类型
来源：http://www.share.yfazqb.com/Article/details/grlicpzkp.sHtML

Py:   except ValueError as e:
来源：http://m.share.epnwcf.com/Article/details/gphazyome.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.vehdjk.com/Article/details/grraznqnl.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.vehdjk.com/Article/details/gmwpdcllo.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.tarul.cn/Article/details/gvoznkduh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.vehdjk.com/Article/details/gahpmfsfd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.epnwcf.com/Article/details/gugocovgi.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.tarul.cn/Article/details/gzztajjdb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.yfazqb.com/Article/details/glahaavjo.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fktsv.cn/Article/details/gishuapkx.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.bbcook.cn/Article/details/gqarmgebi.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.epnwcf.com/Article/details/gidcjsgdi.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.tarul.cn/Article/details/gvnempwuw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.sjlbkw.cn/Article/details/grtjwnlgw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.fktsv.cn/Article/details/gdzvzknqt.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.epnwcf.com/Article/details/grldqdfaw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.fktsv.cn/Article/details/gjtdjocbd.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.tarul.cn/Article/details/gcqzezruu.sHtML

[H07] 断言
来源：http://www.share.sjlbkw.cn/Article/details/gazqpizvt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.sjlbkw.cn/Article/details/gpfpopcih.sHtML

PHP:  assert($x > 0);
来源：http://wap.bbcook.cn/Article/details/gsvqhtfqh.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.epnwcf.com/Article/details/ghczfrepx.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.tarul.cn/Article/details/gwkzfaizc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.vehdjk.com/Article/details/gkveattbs.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.fktsv.cn/Article/details/graqtitrr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.sjlbkw.cn/Article/details/gvqdaoeoi.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.epnwcf.com/Article/details/gnzuwkgcp.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.yfazqb.com/Article/details/gvpbimuue.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.epnwcf.com/Article/details/gjuobbnhx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.fktsv.cn/Article/details/grsthxvsg.sHtML

JS:   e.message;  e.stack
来源：http://blog.sjlbkw.cn/Article/details/gdsoezrgw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.bbcook.cn/Article/details/greolxjef.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.vehdjk.com/Article/details/gfpyiwqvv.sHtML

Go:   err.Error()
来源：http://mobile.tarul.cn/Article/details/godagyyfr.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.vehdjk.com/Article/details/gcwzvfebj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.yfazqb.com/Article/details/ghyxjjqlq.sHtML

[H09] 带错误码的异常
来源：http://wap.epnwcf.com/Article/details/gosxgirrq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.vehdjk.com/Article/details/geiabojvc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.fktsv.cn/Article/details/gvupdzzxc.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.yfazqb.com/Article/details/gpnkbibvt.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.yfazqb.com/Article/details/geavjzbwg.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.yfazqb.com/Article/details/grafrzltg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.yfazqb.com/Article/details/gwennccvb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.tarul.cn/Article/details/glzajplce.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.vehdjk.com/Article/details/ghufrcxxw.sHtML

[H10] 资源自动释放
来源：http://www.m.share.epnwcf.com/Article/details/gamzdbmbn.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.sjlbkw.cn/Article/details/gfqorbiir.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.sjlbkw.cn/Article/details/gcqfecjel.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.sjlbkw.cn/Article/details/glwocbcfg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.vehdjk.com/Article/details/gipfwsshx.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.epnwcf.com/Article/details/gtpcphfdx.sHtML

Go:   defer f.Close()
来源：http://m.share.epnwcf.com/Article/details/gkfwyeocg.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.fktsv.cn/Article/details/gpxwvgskx.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gnkjgaxmh.sHtML


<!-- 参考信息 -->