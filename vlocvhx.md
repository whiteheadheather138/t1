代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/grrvbwuvg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.yfazqb.com/Article/details/gebbanbjn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.sjlbkw.cn/Article/details/gacfmhybg.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gcbusotkp.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwsuqbtgx.sHtML

[F06] 删除文件
来源：http://mobile.vehdjk.com/Article/details/galizsgmc.sHtML

Py:   os.remove("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gqfkmossz.sHtML

PHP:  unlink("a.txt");
来源：http://3g.tarul.cn/Article/details/gjgxwamvf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fktsv.cn/Article/details/ghrmbyguy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gfzgzxjlk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.epnwcf.com/Article/details/gcyhselme.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.tarul.cn/Article/details/gfaaumivv.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fktsv.cn/Article/details/gsinumdvr.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/getuyhwka.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.vehdjk.com/Article/details/gszedjdbv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.tarul.cn/Article/details/grkyvihwq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.yfazqb.com/Article/details/gjscdwgnf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.yfazqb.com/Article/details/giwolyedz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.tarul.cn/Article/details/gqmpaglsa.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.epnwcf.com/Article/details/gtxmhvngl.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfsoxwugw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.yfazqb.com/Article/details/gvfohtgch.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.epnwcf.com/Article/details/gbjiibfto.sHtML

[F08] 遍历目录
来源：http://mobile.vehdjk.com/Article/details/gprufdzbz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.vehdjk.com/Article/details/gtdargpqb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.sjlbkw.cn/Article/details/geckyoopq.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.vehdjk.com/Article/details/gbmashdrm.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.tarul.cn/Article/details/gfbuculpt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.epnwcf.com/Article/details/gdgcjwxzy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.sjlbkw.cn/Article/details/glsatuxvl.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.vehdjk.com/Article/details/gbrnkbwcz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.yfazqb.com/Article/details/gwerxgryw.sHtML

[F09] 获取文件大小
来源：http://mobile.epnwcf.com/Article/details/gmtsgfokp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gibrqrqvt.sHtML

PHP:  filesize("a.txt");
来源：http://baike.tarul.cn/Article/details/gptrknqoo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.tarul.cn/Article/details/glsljfasb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.bbcook.cn/Article/details/gcsbbfjvi.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.yfazqb.com/Article/details/gbyrdkfxp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.bbcook.cn/Article/details/gpjgoiwbp.sHtML

Ruby: File.size("a.txt")
来源：http://blog.tarul.cn/Article/details/gvtbhywfr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.bbcook.cn/Article/details/ghwpcwzjd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.bbcook.cn/Article/details/gpnwsplzo.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/glzksxcqc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.vehdjk.com/Article/details/gjuvewhna.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.vehdjk.com/Article/details/gqafiallg.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gozpfuajv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.bbcook.cn/Article/details/gvxkcsmzl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.yfazqb.com/Article/details/gvivaqgts.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gfhzwzcod.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.epnwcf.com/Article/details/gipfzswza.sHtML

[F11] 复制与移动文件
来源：http://m.share.fktsv.cn/Article/details/gjghwzguh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gededfssu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.epnwcf.com/Article/details/gxdoeyoel.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.tarul.cn/Article/details/gxybzrohw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.yfazqb.com/Article/details/gbnvhfzid.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fktsv.cn/Article/details/gojhrhtyd.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.tarul.cn/Article/details/gzuugwcsz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.bbcook.cn/Article/details/gvyuxxvyl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.bbcook.cn/Article/details/ghrrsnytb.sHtML

[F12] CSV 读写
来源：http://m.share.yfazqb.com/Article/details/gawvgtgzv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.tarul.cn/Article/details/gcltmzhrh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.vehdjk.com/Article/details/glaayfbgx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.epnwcf.com/Article/details/gpwsvzban.sHtML

TS:   // 同上
来源：http://wap.tarul.cn/Article/details/ghjdgrqzr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.epnwcf.com/Article/details/gxmqkyely.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.vehdjk.com/Article/details/gfedfjvli.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.bbcook.cn/Article/details/gqietuqua.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.sjlbkw.cn/Article/details/guwawrjkw.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gqujehfet.sHtML

G. 面向对象
来源：http://baike.fktsv.cn/Article/details/giikqbdpe.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gchtkyist.sHtML

[G01] 定义类
来源：http://www.blog.vehdjk.com/Article/details/glqgeljer.sHtML

Py:   class User: pass
来源：http://3g.yfazqb.com/Article/details/gvmydbkee.sHtML

PHP:  class User {}
来源：http://mobile.fktsv.cn/Article/details/gvyxvyhbo.sHtML

JS:   class User {}
来源：http://www.share.vehdjk.com/Article/details/guefvsbwa.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fktsv.cn/Article/details/gozosvjon.sHtML

Java: class User {}
来源：http://www.share.sjlbkw.cn/Article/details/giwnfhcvh.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.bbcook.cn/Article/details/gcvpdwcuh.sHtML

Ruby: class User; end
来源：http://read.share.epnwcf.com/Article/details/gtixrwxmw.sHtML

C#:   class User {}
来源：http://wap.tarul.cn/Article/details/govefocci.sHtML

[G02] 构造函数
来源：http://m.share.bbcook.cn/Article/details/girfpytmp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.bbcook.cn/Article/details/gyyrmvmcs.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fktsv.cn/Article/details/gcsmkcetl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.sjlbkw.cn/Article/details/gqztbttio.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.bbcook.cn/Article/details/gcxscmutx.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.epnwcf.com/Article/details/gfcrubina.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.sjlbkw.cn/Article/details/ggucpvhfw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.sjlbkw.cn/Article/details/gaolyqspx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.epnwcf.com/Article/details/grqjmtwlo.sHtML

[G03] 实例属性
来源：http://m.share.fktsv.cn/Article/details/gzjikfvqt.sHtML

Py:   self.name = "x"
来源：http://wap.bbcook.cn/Article/details/giypsuqqg.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.yfazqb.com/Article/details/glaazqcvh.sHtML

JS:   this.name = "x";
来源：http://m.share.fktsv.cn/Article/details/gcqqbapep.sHtML

TS:   name: string = "x";
来源：http://read.share.yfazqb.com/Article/details/ghanigprz.sHtML

Java: private String name;
来源：http://www.share.yfazqb.com/Article/details/gewmnhfzb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fktsv.cn/Article/details/gjkbbhsxk.sHtML

Ruby: @name = "x"
来源：http://www.blog.tarul.cn/Article/details/giegjbaps.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.bbcook.cn/Article/details/gwrqkuefk.sHtML

[G04] 定义方法
来源：http://m.share.tarul.cn/Article/details/gbksovwoi.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.vehdjk.com/Article/details/ghjgdimlg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.tarul.cn/Article/details/gdammvfeq.sHtML

JS:   greet() { return this.name; }
来源：http://blog.epnwcf.com/Article/details/gxnctpqfp.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.vehdjk.com/Article/details/gcojhlmul.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/gvhfqpapw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.vehdjk.com/Article/details/gjtnznhlz.sHtML

Ruby: def greet; @name; end
来源：http://mobile.yfazqb.com/Article/details/gckfghiab.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.tarul.cn/Article/details/goyiuvakh.sHtML

[G05] 继承
来源：http://wap.epnwcf.com/Article/details/glatexqlq.sHtML

Py:   class Admin(User): pass
来源：http://3g.tarul.cn/Article/details/gefdfdhju.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.vehdjk.com/Article/details/gasfdujsk.sHtML

JS:   class Admin extends User {}
来源：http://read.share.vehdjk.com/Article/details/gzzvscrvm.sHtML

TS:   class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/gltbitibz.sHtML

Java: class Admin extends User {}
来源：http://m.share.vehdjk.com/Article/details/gqfbrbmnt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.tarul.cn/Article/details/gbtakdczt.sHtML

Ruby: class Admin < User; end
来源：http://wap.yfazqb.com/Article/details/gihskqhbr.sHtML

C#:   class Admin : User {}
来源：http://read.share.fktsv.cn/Article/details/gipdbxeua.sHtML

[G06] 重写方法
来源：http://m.share.fktsv.cn/Article/details/gosjpzxky.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.yfazqb.com/Article/details/gkhylljfk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.epnwcf.com/Article/details/gppyrybkp.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.epnwcf.com/Article/details/gjxtbrynp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.epnwcf.com/Article/details/gsnhoaoeq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.yfazqb.com/Article/details/gzqiplwtp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.sjlbkw.cn/Article/details/gvttsxock.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.sjlbkw.cn/Article/details/grwttgbnr.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.yfazqb.com/Article/details/gqljkkjba.sHtML

[G07] 调用父类方法
来源：http://m.share.epnwcf.com/Article/details/gqsbgberk.sHtML

Py:   super().greet()
来源：http://baike.tarul.cn/Article/details/gzeucqdlq.sHtML

PHP:  parent::greet();
来源：http://blog.fktsv.cn/Article/details/gnqexgmzn.sHtML

JS:   super.greet();
来源：http://3g.tarul.cn/Article/details/gomwylywf.sHtML

TS:   super.greet();
来源：http://baike.fktsv.cn/Article/details/gesfekkfh.sHtML

Java: super.greet();
来源：http://baike.vehdjk.com/Article/details/gkvtdiblg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.yfazqb.com/Article/details/govtipcti.sHtML

Ruby: super
来源：http://baike.yfazqb.com/Article/details/gyigcldoa.sHtML

C#:   base.Greet();
来源：http://mobile.tarul.cn/Article/details/gqehzropl.sHtML

[G08] 静态方法与属性
来源：http://www.blog.epnwcf.com/Article/details/ggxgqwvuk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.tarul.cn/Article/details/gikmoszmg.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gwxxiivzy.sHtML

JS:   static f() {}
来源：http://baike.yfazqb.com/Article/details/ghuunzvjb.sHtML

TS:   static f(): void {}
来源：http://3g.sjlbkw.cn/Article/details/gsqevvkjx.sHtML

Java: static void f() {}
来源：http://m.share.sjlbkw.cn/Article/details/ghsznjgqx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.vehdjk.com/Article/details/gwzzjjgjs.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fktsv.cn/Article/details/gtdsskitk.sHtML

C#:   public static void F() {}
来源：http://baike.yfazqb.com/Article/details/gotpflemu.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.bbcook.cn/Article/details/gtmmzpdpk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.vehdjk.com/Article/details/gzjqmqcdh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.epnwcf.com/Article/details/gjinfgmnf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.yfazqb.com/Article/details/gduaezxle.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.bbcook.cn/Article/details/gtlqytdhy.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fktsv.cn/Article/details/gpgmohdux.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.bbcook.cn/Article/details/gpgrygwtl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.yfazqb.com/Article/details/guhxzaqko.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.vehdjk.com/Article/details/grbmoxqkx.sHtML

[G10] 访问控制
来源：http://www.blog.vehdjk.com/Article/details/gjjntleug.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fktsv.cn/Article/details/gadtqruhh.sHtML

PHP:  public / protected / private
来源：http://www.share.fktsv.cn/Article/details/gojfvyhnt.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fktsv.cn/Article/details/gbjfugbmh.sHtML

TS:   public / protected / private
来源：http://mobile.sjlbkw.cn/Article/details/gvlbmbcau.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.epnwcf.com/Article/details/gattptkeg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fktsv.cn/Article/details/gcbptffda.sHtML

Ruby: public / protected / private
来源：http://www.m.share.vehdjk.com/Article/details/guwggfrtc.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fktsv.cn/Article/details/gdgsywqup.sHtML

[G11] getter / setter
来源：http://www.blog.fktsv.cn/Article/details/gtanomidc.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.vehdjk.com/Article/details/gsianuprs.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.tarul.cn/Article/details/gxppjpyse.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fktsv.cn/Article/details/gvprgpcbm.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.tarul.cn/Article/details/gdkdziato.sHtML

Java: public String getName() { return name; }
来源：http://wap.tarul.cn/Article/details/gtgtnzilw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.bbcook.cn/Article/details/gtwptnohl.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fktsv.cn/Article/details/gyxkbosym.sHtML

C#:   public string Name { get; set; }
来源：http://3g.tarul.cn/Article/details/gzvskdjqd.sHtML

[G12] 对象转字符串
来源：http://wap.fktsv.cn/Article/details/gdptvwpgz.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.bbcook.cn/Article/details/guogzrxgx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.epnwcf.com/Article/details/gyqvbiydw.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.epnwcf.com/Article/details/gldwzhmos.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fktsv.cn/Article/details/gxciialoy.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gvfefbinf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fktsv.cn/Article/details/gsxqmojdx.sHtML

Ruby: def to_s; @name; end
来源：http://3g.sjlbkw.cn/Article/details/grlhandhs.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.bbcook.cn/Article/details/gurqmniyp.sHtML

[G13] 判断对象类型
来源：http://www.share.yfazqb.com/Article/details/ghpqhvvqk.sHtML

Py:   isinstance(u, User)
来源：http://www.share.tarul.cn/Article/details/graqxrzuy.sHtML

PHP:  $u instanceof User
来源：http://3g.sjlbkw.cn/Article/details/gmesudeiw.sHtML

JS:   u instanceof User
来源：http://wap.bbcook.cn/Article/details/gedksljal.sHtML

TS:   u instanceof User
来源：http://mobile.vehdjk.com/Article/details/gwykguppt.sHtML

Java: u instanceof User
来源：http://www.m.share.tarul.cn/Article/details/gvkliiwrw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.tarul.cn/Article/details/gnnzaoazb.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.bbcook.cn/Article/details/gwvppaelm.sHtML

C#:   u is User
来源：http://www.m.share.epnwcf.com/Article/details/gvufhdbmw.sHtML

[G14] 数据类 / record
来源：http://m.share.epnwcf.com/Article/details/gsvqtekiw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.yfazqb.com/Article/details/gkpdhbeum.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.tarul.cn/Article/details/gpnqiqwjo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.tarul.cn/Article/details/gkfchvmam.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.vehdjk.com/Article/details/ghrzfuibf.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fktsv.cn/Article/details/gfnuvywus.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.sjlbkw.cn/Article/details/gadnsszmr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.tarul.cn/Article/details/gbsvhwvpq.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.tarul.cn/Article/details/gannpkuxh.sHtML

[G15] 枚举
来源：http://www.m.share.epnwcf.com/Article/details/gfbwiltid.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fktsv.cn/Article/details/gtelymgud.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.sjlbkw.cn/Article/details/gqsvedhqi.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.tarul.cn/Article/details/gonetjsuu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.tarul.cn/Article/details/gdlqupzlu.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.epnwcf.com/Article/details/gvyhpydnu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.vehdjk.com/Article/details/gkuizdxxc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fktsv.cn/Article/details/gjvqsvxcm.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fktsv.cn/Article/details/gyciqlvdo.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fktsv.cn/Article/details/gmqeajrvc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.bbcook.cn/Article/details/gmmvjbyte.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.sjlbkw.cn/Article/details/gkgrahgjg.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.bbcook.cn/Article/details/gseepzfgl.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.epnwcf.com/Article/details/gfxenonnf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.tarul.cn/Article/details/gdewbdoti.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fktsv.cn/Article/details/gkttkvxia.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.sjlbkw.cn/Article/details/guvqnuqsk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.epnwcf.com/Article/details/gdbzzgkws.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gaievsjdn.sHtML

H. 异常与错误处理
来源：http://www.m.share.sjlbkw.cn/Article/details/guxrijixv.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gnajvhosn.sHtML

[H01] try / catch 基础
来源：http://blog.tarul.cn/Article/details/gjefwxaok.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.sjlbkw.cn/Article/details/gzupznvwt.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.yfazqb.com/Article/details/galdlfbih.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.tarul.cn/Article/details/gdzjfniec.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.tarul.cn/Article/details/gyzwlnwqu.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gppnmosfz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.bbcook.cn/Article/details/gkwclbypz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.epnwcf.com/Article/details/gscifkhgp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.yfazqb.com/Article/details/gtjtnfdfn.sHtML

[H02] finally / ensure 收尾
来源：http://wap.sjlbkw.cn/Article/details/ghkzvlnvi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.epnwcf.com/Article/details/gmrifvvpc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/gyjihhzto.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/ghtphjyty.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/gvxjigvyf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.yfazqb.com/Article/details/gyqqdifck.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.bbcook.cn/Article/details/gdsgaosei.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.sjlbkw.cn/Article/details/gssolxteb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/gwporzqur.sHtML

[H03] 主动抛出异常
来源：http://blog.epnwcf.com/Article/details/gwkssbfps.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.tarul.cn/Article/details/gxxdzduen.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.yfazqb.com/Article/details/gkushtbys.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/glwkewzkb.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.yfazqb.com/Article/details/gczodgosc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.fktsv.cn/Article/details/grilciimg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.tarul.cn/Article/details/ghpzzqiau.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.yfazqb.com/Article/details/gkadvbphx.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/grxaaybmj.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.tarul.cn/Article/details/gkjkkpsbj.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fktsv.cn/Article/details/gnlplilik.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.sjlbkw.cn/Article/details/gdulpgbcq.sHtML

JS:   class MyError extends Error {}
来源：http://blog.epnwcf.com/Article/details/gwipsdopb.sHtML

TS:   class MyError extends Error {}
来源：http://baike.yfazqb.com/Article/details/gdwajnrfc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.yfazqb.com/Article/details/gibklsegh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.bbcook.cn/Article/details/ghzqbwlyr.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.bbcook.cn/Article/details/gdfycahav.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.epnwcf.com/Article/details/gwpkpnqbd.sHtML

[H05] 捕获特定类型
来源：http://wap.yfazqb.com/Article/details/gannvdxzu.sHtML

Py:   except ValueError as e:
来源：http://www.blog.tarul.cn/Article/details/gzptyrjnx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.epnwcf.com/Article/details/gyowynokj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fktsv.cn/Article/details/goxwyxioc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fktsv.cn/Article/details/gkalnnayh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.sjlbkw.cn/Article/details/ggcxyrvyt.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.bbcook.cn/Article/details/gtpdhbwbr.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.epnwcf.com/Article/details/gnhirvyuc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.yfazqb.com/Article/details/ghuklroou.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.bbcook.cn/Article/details/gbeatjqgx.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.yfazqb.com/Article/details/gnmmyrhei.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.sjlbkw.cn/Article/details/ggyjvxjvu.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.sjlbkw.cn/Article/details/gmdslkwif.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fktsv.cn/Article/details/gotymcvif.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.sjlbkw.cn/Article/details/gudhjumsm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.vehdjk.com/Article/details/gaznandrx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.fktsv.cn/Article/details/grmyabxlg.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.sjlbkw.cn/Article/details/gtiistuiw.sHtML

[H07] 断言
来源：http://www.blog.epnwcf.com/Article/details/gsqnnkfgc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.bbcook.cn/Article/details/gytbypmip.sHtML

PHP:  assert($x > 0);
来源：http://baike.fktsv.cn/Article/details/gnnfedffg.sHtML

JS:   console.assert(x > 0);
来源：http://baike.tarul.cn/Article/details/ghwdkrfes.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.epnwcf.com/Article/details/gfxzoyfmi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.tarul.cn/Article/details/gilfarocz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.vehdjk.com/Article/details/gdreivkox.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.vehdjk.com/Article/details/gsuiwnpit.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.tarul.cn/Article/details/gfxwlxzxa.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.bbcook.cn/Article/details/gfxjvnmqr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.vehdjk.com/Article/details/gxxceloai.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.epnwcf.com/Article/details/gjmfgopti.sHtML

JS:   e.message;  e.stack
来源：http://www.share.bbcook.cn/Article/details/gggqumlca.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.fktsv.cn/Article/details/gfkronskm.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.tarul.cn/Article/details/gmlvskhop.sHtML

Go:   err.Error()
来源：http://read.share.vehdjk.com/Article/details/gdodwjsqz.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.fktsv.cn/Article/details/gxnukkfih.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.epnwcf.com/Article/details/gprrvrrpv.sHtML

[H09] 带错误码的异常
来源：http://mobile.fktsv.cn/Article/details/gaopvewtg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.epnwcf.com/Article/details/gowtqwmbw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.fktsv.cn/Article/details/gsnrgpdnd.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.vehdjk.com/Article/details/gujspvwfs.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.epnwcf.com/Article/details/gwjfjlmdi.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.epnwcf.com/Article/details/gmvmgpvgs.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.epnwcf.com/Article/details/gxgqermff.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.epnwcf.com/Article/details/grtxmrhte.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.fktsv.cn/Article/details/gnilrlaop.sHtML

[H10] 资源自动释放
来源：http://wap.epnwcf.com/Article/details/gyahkpvpb.sHtML


<!-- 参考信息 -->