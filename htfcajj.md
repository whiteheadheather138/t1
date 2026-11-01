代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fktsv.cn/Article/details/gjecybfjk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.sjlbkw.cn/Article/details/gbmsdwpai.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fktsv.cn/Article/details/gvnacbzmz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fktsv.cn/Article/details/gxfmeekyd.sHtML

[F09] 获取文件大小
来源：http://read.share.bbcook.cn/Article/details/gdwnnblth.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.tarul.cn/Article/details/gyqcavxib.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gvejvmiwz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.sjlbkw.cn/Article/details/gublmhlbl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.epnwcf.com/Article/details/gfyuwpkwk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.yfazqb.com/Article/details/gvtvqutxd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.yfazqb.com/Article/details/gkeaarufx.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.tarul.cn/Article/details/gwcfexouy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.vehdjk.com/Article/details/gcsrdjldi.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fktsv.cn/Article/details/gkzmaqeno.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/grsmgmgcz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gvolcrpbu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gosjaedez.sHtML

TS:   path.extname("a.txt")
来源：http://3g.epnwcf.com/Article/details/gxmsqpsqe.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.bbcook.cn/Article/details/gjwbpnjjt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.epnwcf.com/Article/details/gchzvjacf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gzclrdstl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.vehdjk.com/Article/details/gqphstxxu.sHtML

[F11] 复制与移动文件
来源：http://m.share.vehdjk.com/Article/details/gcjhodezy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.bbcook.cn/Article/details/gbxddlasa.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.vehdjk.com/Article/details/gxyxmkhcs.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.epnwcf.com/Article/details/gacxirvji.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fktsv.cn/Article/details/grjcukhiy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.vehdjk.com/Article/details/gstcwzixg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.yfazqb.com/Article/details/gylfmzunw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/gojnzfwtw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.sjlbkw.cn/Article/details/gqxpwdoez.sHtML

[F12] CSV 读写
来源：http://www.m.share.epnwcf.com/Article/details/gbcavodro.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.vehdjk.com/Article/details/gipxxclaw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.vehdjk.com/Article/details/glczwwvqx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.bbcook.cn/Article/details/gxyzpbiqm.sHtML

TS:   // 同上
来源：http://www.share.bbcook.cn/Article/details/guzcyektk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.sjlbkw.cn/Article/details/gjfsmiyjm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.sjlbkw.cn/Article/details/gqgxytcke.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.vehdjk.com/Article/details/gevkelnce.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.vehdjk.com/Article/details/ggafrosim.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gbbbhrbgq.sHtML

G. 面向对象
来源：http://mobile.tarul.cn/Article/details/gfgdhdkku.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gyhvyzvpa.sHtML

[G01] 定义类
来源：http://m.share.epnwcf.com/Article/details/gjdbwsjbh.sHtML

Py:   class User: pass
来源：http://baike.fktsv.cn/Article/details/gihlqvasb.sHtML

PHP:  class User {}
来源：http://read.share.tarul.cn/Article/details/gbwaoudoa.sHtML

JS:   class User {}
来源：http://wap.yfazqb.com/Article/details/gwekqeuoe.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.tarul.cn/Article/details/gzdfjqtxt.sHtML

Java: class User {}
来源：http://blog.epnwcf.com/Article/details/gkcsnjxjd.sHtML

Go:   type User struct { Name string }
来源：http://m.share.vehdjk.com/Article/details/gvfggcocu.sHtML

Ruby: class User; end
来源：http://3g.bbcook.cn/Article/details/glbcmecas.sHtML

C#:   class User {}
来源：http://blog.sjlbkw.cn/Article/details/gcuchnzgn.sHtML

[G02] 构造函数
来源：http://blog.vehdjk.com/Article/details/guwhowrsz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.yfazqb.com/Article/details/gbfmudemj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fktsv.cn/Article/details/gplggsxap.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.yfazqb.com/Article/details/gtkyvlfrl.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.vehdjk.com/Article/details/gdwbffoar.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.bbcook.cn/Article/details/giujrlnvp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.epnwcf.com/Article/details/glpootajp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fktsv.cn/Article/details/gwbxuczit.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.tarul.cn/Article/details/goevoxish.sHtML

[G03] 实例属性
来源：http://baike.vehdjk.com/Article/details/guhanvvic.sHtML

Py:   self.name = "x"
来源：http://blog.sjlbkw.cn/Article/details/gghwyvvlk.sHtML

PHP:  public string $name = "x";
来源：http://mobile.vehdjk.com/Article/details/guxopjsof.sHtML

JS:   this.name = "x";
来源：http://blog.fktsv.cn/Article/details/gjaqrbkij.sHtML

TS:   name: string = "x";
来源：http://wap.bbcook.cn/Article/details/ggljefrjs.sHtML

Java: private String name;
来源：http://blog.fktsv.cn/Article/details/gktrkcpks.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.tarul.cn/Article/details/gwvcnggoz.sHtML

Ruby: @name = "x"
来源：http://read.share.vehdjk.com/Article/details/gossqgjal.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fktsv.cn/Article/details/gfqwnmwhp.sHtML

[G04] 定义方法
来源：http://www.blog.vehdjk.com/Article/details/gsxypcuow.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.epnwcf.com/Article/details/gngomljly.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.vehdjk.com/Article/details/gbczwrxbo.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.bbcook.cn/Article/details/gucokddmm.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.vehdjk.com/Article/details/gtzszcgey.sHtML

Java: String greet() { return name; }
来源：http://read.share.bbcook.cn/Article/details/gcfhiheby.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.vehdjk.com/Article/details/glwsansqh.sHtML

Ruby: def greet; @name; end
来源：http://mobile.epnwcf.com/Article/details/gcpqefdva.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fktsv.cn/Article/details/ghtvxvokg.sHtML

[G05] 继承
来源：http://m.share.fktsv.cn/Article/details/gxejvjwvi.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.vehdjk.com/Article/details/gytrwagkn.sHtML

PHP:  class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/gyvfgybue.sHtML

JS:   class Admin extends User {}
来源：http://m.share.bbcook.cn/Article/details/ggftzszqi.sHtML

TS:   class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/gagoibltl.sHtML

Java: class Admin extends User {}
来源：http://read.share.yfazqb.com/Article/details/gbzttufwe.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.vehdjk.com/Article/details/gulfsjdzp.sHtML

Ruby: class Admin < User; end
来源：http://wap.fktsv.cn/Article/details/gucysgwya.sHtML

C#:   class Admin : User {}
来源：http://m.share.bbcook.cn/Article/details/gpjvatkcb.sHtML

[G06] 重写方法
来源：http://baike.sjlbkw.cn/Article/details/gcfwyqmmz.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fktsv.cn/Article/details/gkmrwjccz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gjafrhppv.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.sjlbkw.cn/Article/details/gdmnjkont.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.yfazqb.com/Article/details/greyldgpo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.yfazqb.com/Article/details/gubrmxbhb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.epnwcf.com/Article/details/gotxatkoe.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fktsv.cn/Article/details/gyaqymcbj.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.yfazqb.com/Article/details/ghtlwxbie.sHtML

[G07] 调用父类方法
来源：http://www.blog.yfazqb.com/Article/details/grumpgmtb.sHtML

Py:   super().greet()
来源：http://blog.vehdjk.com/Article/details/gfytqzgcu.sHtML

PHP:  parent::greet();
来源：http://mobile.tarul.cn/Article/details/gczxgvvgt.sHtML

JS:   super.greet();
来源：http://3g.fktsv.cn/Article/details/gyladioyh.sHtML

TS:   super.greet();
来源：http://baike.bbcook.cn/Article/details/gibhsprpc.sHtML

Java: super.greet();
来源：http://blog.epnwcf.com/Article/details/gemjopulc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.epnwcf.com/Article/details/gyjtocgbs.sHtML

Ruby: super
来源：http://www.m.share.sjlbkw.cn/Article/details/ggylocveg.sHtML

C#:   base.Greet();
来源：http://3g.bbcook.cn/Article/details/gyvcphojd.sHtML

[G08] 静态方法与属性
来源：http://mobile.yfazqb.com/Article/details/gcktqcrfe.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.epnwcf.com/Article/details/gicmsnvto.sHtML

PHP:  public static function f() {}
来源：http://read.share.tarul.cn/Article/details/ghfjhmzrz.sHtML

JS:   static f() {}
来源：http://3g.fktsv.cn/Article/details/gdqnygdpd.sHtML

TS:   static f(): void {}
来源：http://www.blog.sjlbkw.cn/Article/details/guexnptkn.sHtML

Java: static void f() {}
来源：http://baike.tarul.cn/Article/details/gnbwfvjoh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.yfazqb.com/Article/details/gattknurg.sHtML

Ruby: def self.f; end
来源：http://www.blog.sjlbkw.cn/Article/details/gmobjmbbk.sHtML

C#:   public static void F() {}
来源：http://mobile.yfazqb.com/Article/details/gnjwnwmmu.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.tarul.cn/Article/details/gxnhoksts.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.vehdjk.com/Article/details/ghdvmbxfu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.vehdjk.com/Article/details/ggdpmsmxd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.epnwcf.com/Article/details/ghesegbti.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.vehdjk.com/Article/details/gvaqkcsho.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.tarul.cn/Article/details/glawllptn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.tarul.cn/Article/details/gsfgsgfpk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fktsv.cn/Article/details/gnuhzxyjs.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.vehdjk.com/Article/details/gmwvcgein.sHtML

[G10] 访问控制
来源：http://read.share.fktsv.cn/Article/details/glydsdzuy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.bbcook.cn/Article/details/gkhesmuov.sHtML

PHP:  public / protected / private
来源：http://www.m.share.tarul.cn/Article/details/gzbatpapk.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.epnwcf.com/Article/details/gstvkfves.sHtML

TS:   public / protected / private
来源：http://wap.yfazqb.com/Article/details/gmddpodza.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.vehdjk.com/Article/details/gyvqdbyhq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fktsv.cn/Article/details/gmhbgbxgq.sHtML

Ruby: public / protected / private
来源：http://wap.vehdjk.com/Article/details/grtmrjumz.sHtML

C#:   public / protected / private / internal
来源：http://baike.tarul.cn/Article/details/gdgnghsbh.sHtML

[G11] getter / setter
来源：http://m.share.sjlbkw.cn/Article/details/ggdcfytyr.sHtML

Py:   @property 与 @x.setter
来源：http://3g.vehdjk.com/Article/details/gxavkmgrj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fktsv.cn/Article/details/gpphuyvua.sHtML

JS:   get name() { return this._name; }
来源：http://wap.bbcook.cn/Article/details/gfuxeaojp.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.tarul.cn/Article/details/gnefwjyhu.sHtML

Java: public String getName() { return name; }
来源：http://blog.vehdjk.com/Article/details/gabzivukh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fktsv.cn/Article/details/grtxzotgz.sHtML

Ruby: attr_accessor :name
来源：http://blog.yfazqb.com/Article/details/gvpdkvsgs.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfilolctr.sHtML

[G12] 对象转字符串
来源：http://wap.vehdjk.com/Article/details/ggrwhdsbz.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fktsv.cn/Article/details/gukfrtooy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.yfazqb.com/Article/details/ghfpwrxve.sHtML

JS:   toString() { return this.name; }
来源：http://baike.vehdjk.com/Article/details/gpgnyxeqb.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fktsv.cn/Article/details/gepyzkbgh.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.tarul.cn/Article/details/ghrxvaktl.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.vehdjk.com/Article/details/gjtartfbm.sHtML

Ruby: def to_s; @name; end
来源：http://wap.yfazqb.com/Article/details/grjtalhan.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.epnwcf.com/Article/details/gqcqtnzit.sHtML

[G13] 判断对象类型
来源：http://read.share.sjlbkw.cn/Article/details/grfqdzbcl.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.vehdjk.com/Article/details/gdwanelfu.sHtML

PHP:  $u instanceof User
来源：http://wap.vehdjk.com/Article/details/gacfesthc.sHtML

JS:   u instanceof User
来源：http://www.m.share.yfazqb.com/Article/details/gimjhvphg.sHtML

TS:   u instanceof User
来源：http://wap.epnwcf.com/Article/details/gxbzcexmh.sHtML

Java: u instanceof User
来源：http://mobile.bbcook.cn/Article/details/gwkeqtlyw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.vehdjk.com/Article/details/gchxztvsf.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.sjlbkw.cn/Article/details/gnhhwfmjz.sHtML

C#:   u is User
来源：http://wap.tarul.cn/Article/details/gbslmfcpe.sHtML

[G14] 数据类 / record
来源：http://m.share.epnwcf.com/Article/details/gcyiezsya.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fktsv.cn/Article/details/gtygygaah.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.sjlbkw.cn/Article/details/gbulvsupf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.yfazqb.com/Article/details/gwhgluuir.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.epnwcf.com/Article/details/gpbmhgdys.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.tarul.cn/Article/details/gallqqqgc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.epnwcf.com/Article/details/gmnbhtusi.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.sjlbkw.cn/Article/details/ghmdxnjbw.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.tarul.cn/Article/details/gdfygswcq.sHtML

[G15] 枚举
来源：http://read.share.vehdjk.com/Article/details/gnerfhljz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.vehdjk.com/Article/details/gqmsidyal.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.yfazqb.com/Article/details/gbpfjeodm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.epnwcf.com/Article/details/gyfcynlwd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.bbcook.cn/Article/details/ghaxocfbd.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.bbcook.cn/Article/details/glytdextm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.bbcook.cn/Article/details/gifhukdfc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.sjlbkw.cn/Article/details/groncumgu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.epnwcf.com/Article/details/gfifqmgsl.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.tarul.cn/Article/details/gpxqrymku.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fktsv.cn/Article/details/gdvlfiemj.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.sjlbkw.cn/Article/details/gcdicpngh.sHtML

JS:   Object.entries(obj)
来源：http://mobile.vehdjk.com/Article/details/ghacxfwcu.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gxbmhjpbl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.vehdjk.com/Article/details/gbvjyxvjd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.bbcook.cn/Article/details/glyfjsacf.sHtML

Ruby: obj.instance_variables
来源：http://wap.bbcook.cn/Article/details/gatvxhzjb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fktsv.cn/Article/details/gucugshnx.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/guibldavj.sHtML

H. 异常与错误处理
来源：http://www.blog.bbcook.cn/Article/details/gxhtwfzvr.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gapkjhwva.sHtML

[H01] try / catch 基础
来源：http://mobile.sjlbkw.cn/Article/details/gefjrvzls.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.vehdjk.com/Article/details/gwenrmdns.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fktsv.cn/Article/details/gcmkmpybg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.sjlbkw.cn/Article/details/gnmccmyzt.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.yfazqb.com/Article/details/gobirfuxp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.tarul.cn/Article/details/gsvbavbeo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.epnwcf.com/Article/details/gavplmpjd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.epnwcf.com/Article/details/giftnzsmo.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.yfazqb.com/Article/details/ggjnzzkwj.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.epnwcf.com/Article/details/gpaaplwyc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.bbcook.cn/Article/details/gqpcduane.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.yfazqb.com/Article/details/geogqckfm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/gkhtrymho.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.bbcook.cn/Article/details/gtbriredi.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fktsv.cn/Article/details/gvoazkqgr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.bbcook.cn/Article/details/gabqpemxy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.bbcook.cn/Article/details/grkyiggbn.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/ggjbymjgx.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.tarul.cn/Article/details/glfmzucpj.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.vehdjk.com/Article/details/gfsrykqno.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/gemrfjmyy.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.bbcook.cn/Article/details/gsacfthoh.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.tarul.cn/Article/details/ggqkrzvpy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.yfazqb.com/Article/details/gkyqhtptc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.epnwcf.com/Article/details/gagectqgi.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.yfazqb.com/Article/details/gogcivuhh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.vehdjk.com/Article/details/ganmgrypm.sHtML

[H04] 自定义异常类型
来源：http://m.share.vehdjk.com/Article/details/gzwpvlwra.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.epnwcf.com/Article/details/gwnpvsxea.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.vehdjk.com/Article/details/gntkysama.sHtML

JS:   class MyError extends Error {}
来源：http://blog.epnwcf.com/Article/details/gghjyziub.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.bbcook.cn/Article/details/gknlaxywg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.bbcook.cn/Article/details/gdjbyktmg.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.yfazqb.com/Article/details/gkfdlexfr.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.fktsv.cn/Article/details/gbwfjjori.sHtML

C#:   class MyException : Exception {}
来源：http://blog.sjlbkw.cn/Article/details/gwtnhtcah.sHtML

[H05] 捕获特定类型
来源：http://www.share.yfazqb.com/Article/details/gnbbtjnph.sHtML

Py:   except ValueError as e:
来源：http://blog.yfazqb.com/Article/details/guhokgqta.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fktsv.cn/Article/details/gicliaiyh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.vehdjk.com/Article/details/gsmkwkkqn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.tarul.cn/Article/details/ghqfecumi.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.epnwcf.com/Article/details/gkgvywido.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.bbcook.cn/Article/details/gfxtubhul.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fktsv.cn/Article/details/gyltlmqaq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fktsv.cn/Article/details/gmvpipqxz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.yfazqb.com/Article/details/gibnswptk.sHtML

Py:   value = d.get("k") or default
来源：http://blog.epnwcf.com/Article/details/gcmguwhdo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.yfazqb.com/Article/details/gbcmgwumt.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.yfazqb.com/Article/details/gqcujucxf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.bbcook.cn/Article/details/gegcoiezd.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.vehdjk.com/Article/details/gdbwxxeiv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.tarul.cn/Article/details/ggjqkdthb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.bbcook.cn/Article/details/ggpllzjij.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.vehdjk.com/Article/details/grcpbanha.sHtML

[H07] 断言
来源：http://m.share.sjlbkw.cn/Article/details/grggwovhe.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.bbcook.cn/Article/details/gmylbljxq.sHtML

PHP:  assert($x > 0);
来源：http://mobile.vehdjk.com/Article/details/gwlaxwkol.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/ghshsebrg.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gpizxauad.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.epnwcf.com/Article/details/gmglxhpgd.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.bbcook.cn/Article/details/grlzxkilm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.yfazqb.com/Article/details/glvrfpgdx.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.bbcook.cn/Article/details/ggcoyuqqf.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.epnwcf.com/Article/details/gelylgbld.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.vehdjk.com/Article/details/gwkogskld.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fktsv.cn/Article/details/glnhpqdzl.sHtML

JS:   e.message;  e.stack
来源：http://blog.vehdjk.com/Article/details/gifpwutmf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.epnwcf.com/Article/details/goetsbhxx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.bbcook.cn/Article/details/gjzkagmie.sHtML

Go:   err.Error()
来源：http://baike.fktsv.cn/Article/details/gdnomyekx.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.fktsv.cn/Article/details/gdmbmybfg.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.sjlbkw.cn/Article/details/gdsrmpnzz.sHtML

[H09] 带错误码的异常
来源：http://wap.epnwcf.com/Article/details/gomkcgbsg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.bbcook.cn/Article/details/gjadcrruj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.bbcook.cn/Article/details/grllgtbxo.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.epnwcf.com/Article/details/gbwjfdtwi.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.vehdjk.com/Article/details/gtcaihonv.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.vehdjk.com/Article/details/gfaqjdkso.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.yfazqb.com/Article/details/ggoezcnij.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.vehdjk.com/Article/details/giqwvbnma.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.vehdjk.com/Article/details/gptbqebsa.sHtML

[H10] 资源自动释放
来源：http://read.share.bbcook.cn/Article/details/gjarkvxdn.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.epnwcf.com/Article/details/gwfmqbhxq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.tarul.cn/Article/details/getcfysam.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.tarul.cn/Article/details/gxxyueebv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.bbcook.cn/Article/details/gmgyjnjhh.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.tarul.cn/Article/details/gshmmnxaw.sHtML

Go:   defer f.Close()
来源：http://m.share.vehdjk.com/Article/details/gkecrjbhp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.fktsv.cn/Article/details/gfpwqcsyq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gwvqbxhho.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/ghteevhbl.sHtML

I. 正则表达式
来源：http://baike.epnwcf.com/Article/details/gzxrwcwwu.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/glbkrfujg.sHtML

[I01] 判断是否匹配
来源：http://3g.yfazqb.com/Article/details/gnzpwmazw.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.bbcook.cn/Article/details/glieghosf.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.bbcook.cn/Article/details/gnozouvfq.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.yfazqb.com/Article/details/gczxbwuwn.sHtML

TS:   /\d+/.test(s)
来源：http://wap.tarul.cn/Article/details/gyduhywqv.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.fktsv.cn/Article/details/gryexyzgn.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.fktsv.cn/Article/details/gdakygnco.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.bbcook.cn/Article/details/gqkztbacp.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.vehdjk.com/Article/details/gkqizstse.sHtML

[I02] 提取所有匹配
来源：http://wap.vehdjk.com/Article/details/guayhlqag.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.yfazqb.com/Article/details/gculrhfpu.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.sjlbkw.cn/Article/details/gektmzpzn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.vehdjk.com/Article/details/gasvshtim.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.yfazqb.com/Article/details/gntttmpqu.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.fktsv.cn/Article/details/ggrfgbsrj.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.sjlbkw.cn/Article/details/gommzomjl.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.sjlbkw.cn/Article/details/gzopwzbes.sHtML


<!-- 参考信息 -->