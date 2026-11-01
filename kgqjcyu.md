代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://www.share.fktsv.cn/Article/details/gqpydejnr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.sjlbkw.cn/Article/details/gmuiqtpsx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.epnwcf.com/Article/details/gojgpshno.sHtML

Ruby: File.size("a.txt")
来源：http://blog.vehdjk.com/Article/details/gilocatvs.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.bbcook.cn/Article/details/garamqtdq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.epnwcf.com/Article/details/gvvzmobgg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.vehdjk.com/Article/details/gpyzmelmd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gwgatzvvx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/gyyxehuxq.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gjyaktuzu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.yfazqb.com/Article/details/gsmbgcqll.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gnldndkmc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/gxeigzjnn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gxqunwkdk.sHtML

[F11] 复制与移动文件
来源：http://www.blog.tarul.cn/Article/details/gyzlpxhud.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.yfazqb.com/Article/details/goxvivmba.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.bbcook.cn/Article/details/gyvrkxmyh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.tarul.cn/Article/details/gcnfnjuiy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/gytlbhkbu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fktsv.cn/Article/details/grgbasuoc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fktsv.cn/Article/details/gpmanjtvv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fktsv.cn/Article/details/gkudnsovk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.bbcook.cn/Article/details/gierolmyy.sHtML

[F12] CSV 读写
来源：http://read.share.sjlbkw.cn/Article/details/gozzxrqnn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.yfazqb.com/Article/details/gicalewjr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.yfazqb.com/Article/details/gmqnhibjw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.epnwcf.com/Article/details/ggnokhyha.sHtML

TS:   // 同上
来源：http://read.share.bbcook.cn/Article/details/gghrlshir.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.sjlbkw.cn/Article/details/gruxywbvr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fktsv.cn/Article/details/gmsbcebuz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fktsv.cn/Article/details/gunoeojiq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.epnwcf.com/Article/details/gsfaoqiow.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gzclnocvv.sHtML

G. 面向对象
来源：http://m.share.tarul.cn/Article/details/gpubzutfc.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/guhphcqhc.sHtML

[G01] 定义类
来源：http://www.m.share.yfazqb.com/Article/details/ggvduolqu.sHtML

Py:   class User: pass
来源：http://3g.bbcook.cn/Article/details/ggkcfzdxx.sHtML

PHP:  class User {}
来源：http://mobile.epnwcf.com/Article/details/gbtvmdxap.sHtML

JS:   class User {}
来源：http://www.blog.tarul.cn/Article/details/gdnuhszrr.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.sjlbkw.cn/Article/details/gaghiirmr.sHtML

Java: class User {}
来源：http://www.blog.bbcook.cn/Article/details/glglqjxzz.sHtML

Go:   type User struct { Name string }
来源：http://baike.yfazqb.com/Article/details/gzvzzoupj.sHtML

Ruby: class User; end
来源：http://3g.epnwcf.com/Article/details/gnmwpohhp.sHtML

C#:   class User {}
来源：http://www.share.epnwcf.com/Article/details/gscaikuho.sHtML

[G02] 构造函数
来源：http://read.share.epnwcf.com/Article/details/guxvjdanc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.sjlbkw.cn/Article/details/gxukvolhu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.vehdjk.com/Article/details/gfrcntvqv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.yfazqb.com/Article/details/gzlaktgwx.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.tarul.cn/Article/details/ggtsbsjoy.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.epnwcf.com/Article/details/gskgmaryg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.epnwcf.com/Article/details/gdscezubr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.vehdjk.com/Article/details/gnkwtpeqf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.sjlbkw.cn/Article/details/gxrevwozo.sHtML

[G03] 实例属性
来源：http://read.share.tarul.cn/Article/details/gcnodjcpu.sHtML

Py:   self.name = "x"
来源：http://3g.fktsv.cn/Article/details/ghwwzkiyl.sHtML

PHP:  public string $name = "x";
来源：http://m.share.epnwcf.com/Article/details/gykgsivks.sHtML

JS:   this.name = "x";
来源：http://blog.fktsv.cn/Article/details/gxfahgtyt.sHtML

TS:   name: string = "x";
来源：http://baike.sjlbkw.cn/Article/details/gfwsqujwd.sHtML

Java: private String name;
来源：http://read.share.vehdjk.com/Article/details/gbhkgzobs.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.epnwcf.com/Article/details/gxfjgajso.sHtML

Ruby: @name = "x"
来源：http://baike.vehdjk.com/Article/details/gvwiuxytj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.tarul.cn/Article/details/gyejqivrj.sHtML

[G04] 定义方法
来源：http://mobile.vehdjk.com/Article/details/gbntoncdl.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fktsv.cn/Article/details/gyscrvmty.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.yfazqb.com/Article/details/gnbxpirfu.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.tarul.cn/Article/details/gzgieetjk.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.yfazqb.com/Article/details/gzirxxpzm.sHtML

Java: String greet() { return name; }
来源：http://blog.vehdjk.com/Article/details/gtrorpxwk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.sjlbkw.cn/Article/details/grfqtudhf.sHtML

Ruby: def greet; @name; end
来源：http://mobile.epnwcf.com/Article/details/gusudtmny.sHtML

C#:   public string Greet() => Name;
来源：http://wap.tarul.cn/Article/details/grohbtoll.sHtML

[G05] 继承
来源：http://3g.bbcook.cn/Article/details/gnrwpypif.sHtML

Py:   class Admin(User): pass
来源：http://www.share.tarul.cn/Article/details/gqkfoowmi.sHtML

PHP:  class Admin extends User {}
来源：http://wap.vehdjk.com/Article/details/gurgftowi.sHtML

JS:   class Admin extends User {}
来源：http://blog.epnwcf.com/Article/details/gltieffts.sHtML

TS:   class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/gfrlxwfys.sHtML

Java: class Admin extends User {}
来源：http://read.share.vehdjk.com/Article/details/gwmfqrczq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.bbcook.cn/Article/details/gngbmbkel.sHtML

Ruby: class Admin < User; end
来源：http://read.share.epnwcf.com/Article/details/gzdwdparc.sHtML

C#:   class Admin : User {}
来源：http://3g.tarul.cn/Article/details/gzuqshsnp.sHtML

[G06] 重写方法
来源：http://baike.tarul.cn/Article/details/gojbfawop.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.tarul.cn/Article/details/giyosmxke.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gnwpytpdt.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.vehdjk.com/Article/details/gzjfsxkhm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gtpkgskwv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.tarul.cn/Article/details/gvbuqezkb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fktsv.cn/Article/details/giqvdvpil.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fktsv.cn/Article/details/gudnmsmkk.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fktsv.cn/Article/details/gebadbfbf.sHtML

[G07] 调用父类方法
来源：http://www.share.tarul.cn/Article/details/gqxwtxcph.sHtML

Py:   super().greet()
来源：http://mobile.fktsv.cn/Article/details/gzxilqyxz.sHtML

PHP:  parent::greet();
来源：http://www.m.share.epnwcf.com/Article/details/gcgwubkgm.sHtML

JS:   super.greet();
来源：http://3g.tarul.cn/Article/details/ggnebcclb.sHtML

TS:   super.greet();
来源：http://blog.epnwcf.com/Article/details/glbbmrawc.sHtML

Java: super.greet();
来源：http://m.share.bbcook.cn/Article/details/goywnygov.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.vehdjk.com/Article/details/guggpbbew.sHtML

Ruby: super
来源：http://www.share.tarul.cn/Article/details/gyubznnuw.sHtML

C#:   base.Greet();
来源：http://read.share.epnwcf.com/Article/details/gwalreeth.sHtML

[G08] 静态方法与属性
来源：http://read.share.bbcook.cn/Article/details/gmtkgvzeg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.yfazqb.com/Article/details/gybtmfqnz.sHtML

PHP:  public static function f() {}
来源：http://baike.tarul.cn/Article/details/gsibisuax.sHtML

JS:   static f() {}
来源：http://read.share.yfazqb.com/Article/details/gryagprev.sHtML

TS:   static f(): void {}
来源：http://read.share.epnwcf.com/Article/details/gnrqtkmgu.sHtML

Java: static void f() {}
来源：http://www.m.share.yfazqb.com/Article/details/ggiptyoas.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.bbcook.cn/Article/details/gradnnvfk.sHtML

Ruby: def self.f; end
来源：http://mobile.yfazqb.com/Article/details/govxkfkvw.sHtML

C#:   public static void F() {}
来源：http://wap.tarul.cn/Article/details/gzjsbjvcw.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.tarul.cn/Article/details/gmpikhmjl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.tarul.cn/Article/details/gppegkdzh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.tarul.cn/Article/details/ggrjrwjqn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.bbcook.cn/Article/details/glkecqznd.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.tarul.cn/Article/details/gbvmosflx.sHtML

Java: interface Shape { double area(); }
来源：http://blog.epnwcf.com/Article/details/gwoujriqy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.vehdjk.com/Article/details/gziodmudt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.vehdjk.com/Article/details/gkectcbmb.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.tarul.cn/Article/details/goknkrtwd.sHtML

[G10] 访问控制
来源：http://mobile.sjlbkw.cn/Article/details/gzikkhjiy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.epnwcf.com/Article/details/gdjwwlqnw.sHtML

PHP:  public / protected / private
来源：http://m.share.fktsv.cn/Article/details/gkgmbnshv.sHtML

JS:   #private 字段；其余公开
来源：http://baike.tarul.cn/Article/details/gxsbzvnyz.sHtML

TS:   public / protected / private
来源：http://www.blog.sjlbkw.cn/Article/details/gbmtecsdu.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.tarul.cn/Article/details/gpzeltbiq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fktsv.cn/Article/details/gkctbhemq.sHtML

Ruby: public / protected / private
来源：http://www.blog.yfazqb.com/Article/details/gkqgclflr.sHtML

C#:   public / protected / private / internal
来源：http://wap.fktsv.cn/Article/details/gjzenaldm.sHtML

[G11] getter / setter
来源：http://m.share.tarul.cn/Article/details/groeuafqx.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.bbcook.cn/Article/details/gcttyvvdl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fktsv.cn/Article/details/ggysufwvu.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.bbcook.cn/Article/details/gziuhhhiq.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.sjlbkw.cn/Article/details/gawbureox.sHtML

Java: public String getName() { return name; }
来源：http://m.share.bbcook.cn/Article/details/gbpfbpvsk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.vehdjk.com/Article/details/gewfzwfwn.sHtML

Ruby: attr_accessor :name
来源：http://3g.tarul.cn/Article/details/gzvsnznfz.sHtML

C#:   public string Name { get; set; }
来源：http://3g.vehdjk.com/Article/details/geryfnncn.sHtML

[G12] 对象转字符串
来源：http://3g.epnwcf.com/Article/details/gsazqpeps.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.tarul.cn/Article/details/gexpomdku.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.yfazqb.com/Article/details/gtzczwnjd.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fktsv.cn/Article/details/gciwndzpo.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.vehdjk.com/Article/details/grzuvusem.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/gbvqmqrwa.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.vehdjk.com/Article/details/gdmzqnwyz.sHtML

Ruby: def to_s; @name; end
来源：http://baike.epnwcf.com/Article/details/gmloctzcb.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.epnwcf.com/Article/details/gqxoaxeuw.sHtML

[G13] 判断对象类型
来源：http://mobile.tarul.cn/Article/details/gyyieiqan.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.yfazqb.com/Article/details/gazrouepy.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fktsv.cn/Article/details/gsnuiqqwn.sHtML

JS:   u instanceof User
来源：http://baike.tarul.cn/Article/details/gvsttixha.sHtML

TS:   u instanceof User
来源：http://baike.sjlbkw.cn/Article/details/gxnfpqpax.sHtML

Java: u instanceof User
来源：http://read.share.sjlbkw.cn/Article/details/gnfrjkiom.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.epnwcf.com/Article/details/gzvrxlacf.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fktsv.cn/Article/details/gylsxgmwb.sHtML

C#:   u is User
来源：http://mobile.fktsv.cn/Article/details/gyyqegpyn.sHtML

[G14] 数据类 / record
来源：http://baike.sjlbkw.cn/Article/details/gyqlhipzv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.bbcook.cn/Article/details/ggyyiuxhe.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.vehdjk.com/Article/details/gmkyvdzys.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.vehdjk.com/Article/details/grykqydeq.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.bbcook.cn/Article/details/glqzvthhd.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.yfazqb.com/Article/details/gdebwdppv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.bbcook.cn/Article/details/gwtnvuufp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.epnwcf.com/Article/details/gzmsarjue.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.bbcook.cn/Article/details/gxsmjldzp.sHtML

[G15] 枚举
来源：http://mobile.tarul.cn/Article/details/gyeypjuzq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.epnwcf.com/Article/details/gpxsnwccn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.sjlbkw.cn/Article/details/gazxrxtoz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.bbcook.cn/Article/details/gomacfqbr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.vehdjk.com/Article/details/gzbwathju.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.epnwcf.com/Article/details/gmjhpnokh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.tarul.cn/Article/details/gattpvuiv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.vehdjk.com/Article/details/gizcuibin.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.epnwcf.com/Article/details/gaylxiiaa.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.tarul.cn/Article/details/gkimxvcbp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.tarul.cn/Article/details/gzmubkkki.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.vehdjk.com/Article/details/gtzevjvjo.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpvtrfcel.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fktsv.cn/Article/details/gxahjwoxs.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.fktsv.cn/Article/details/gwejwyjuc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.epnwcf.com/Article/details/glegflftv.sHtML

Ruby: obj.instance_variables
来源：http://blog.epnwcf.com/Article/details/gjhywguma.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.tarul.cn/Article/details/ggmnhiftj.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gubddizqd.sHtML

H. 异常与错误处理
来源：http://m.share.vehdjk.com/Article/details/gelxfteju.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gwccirnzk.sHtML

[H01] try / catch 基础
来源：http://www.blog.sjlbkw.cn/Article/details/ghiiphjif.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.bbcook.cn/Article/details/gjckyznva.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.yfazqb.com/Article/details/gifxvxwer.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.epnwcf.com/Article/details/gufpuzyqx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.tarul.cn/Article/details/gsleotxvj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.bbcook.cn/Article/details/gkveirtzr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.epnwcf.com/Article/details/gpgdffrek.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.tarul.cn/Article/details/ghqusqodn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fktsv.cn/Article/details/gqwkajaoa.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.sjlbkw.cn/Article/details/gktozcgte.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.yfazqb.com/Article/details/ggyucmlro.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.tarul.cn/Article/details/gdjscxbvf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/gzdwrqrlh.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/gpgtstjdg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/goehwewjb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.sjlbkw.cn/Article/details/gsmfpinlk.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.tarul.cn/Article/details/geebunuij.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/guvblvcsx.sHtML

[H03] 主动抛出异常
来源：http://wap.yfazqb.com/Article/details/gkxefrtrw.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fktsv.cn/Article/details/gbfeuckab.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.yfazqb.com/Article/details/gkealuscu.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.epnwcf.com/Article/details/gvbgyliql.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.vehdjk.com/Article/details/gdlxumukn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.tarul.cn/Article/details/gpmhhlsdi.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.tarul.cn/Article/details/gushvtchf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.tarul.cn/Article/details/gwyfrgmph.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.fktsv.cn/Article/details/gxjyxfhzv.sHtML

[H04] 自定义异常类型
来源：http://m.share.tarul.cn/Article/details/gaedxsbep.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.bbcook.cn/Article/details/glknkhogk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.vehdjk.com/Article/details/gywdamced.sHtML

JS:   class MyError extends Error {}
来源：http://blog.bbcook.cn/Article/details/gjragncax.sHtML

TS:   class MyError extends Error {}
来源：http://3g.epnwcf.com/Article/details/gkqpciwjm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.sjlbkw.cn/Article/details/gvttjxnqu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.sjlbkw.cn/Article/details/gkpmdeokw.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.yfazqb.com/Article/details/gvnfvfehe.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gyyxdwjch.sHtML

[H05] 捕获特定类型
来源：http://baike.vehdjk.com/Article/details/glexczmbb.sHtML

Py:   except ValueError as e:
来源：http://blog.tarul.cn/Article/details/gaugfiewb.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.vehdjk.com/Article/details/gbwpmgtxl.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.sjlbkw.cn/Article/details/guzumgoli.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fktsv.cn/Article/details/guyezskde.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.vehdjk.com/Article/details/glornkftz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fktsv.cn/Article/details/gpxevdijm.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.yfazqb.com/Article/details/gtmnjcipr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.yfazqb.com/Article/details/gmyeitlfi.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fktsv.cn/Article/details/gsgqmjkuy.sHtML

Py:   value = d.get("k") or default
来源：http://wap.yfazqb.com/Article/details/gzlcmxbsa.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.fktsv.cn/Article/details/glpqkpegp.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.sjlbkw.cn/Article/details/gcvrppift.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fktsv.cn/Article/details/gpwudbwqg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.epnwcf.com/Article/details/guhapgjsw.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.fktsv.cn/Article/details/gsivtlavu.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.sjlbkw.cn/Article/details/grpfrguli.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.bbcook.cn/Article/details/gdpnqcyuk.sHtML

[H07] 断言
来源：http://mobile.sjlbkw.cn/Article/details/gdwspebhw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.epnwcf.com/Article/details/gdzwnvmls.sHtML

PHP:  assert($x > 0);
来源：http://mobile.yfazqb.com/Article/details/gqqichhon.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.epnwcf.com/Article/details/gisaqkjyy.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fktsv.cn/Article/details/gviplpyfx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.epnwcf.com/Article/details/gdaafowqn.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.vehdjk.com/Article/details/gikkdnktf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.yfazqb.com/Article/details/gykofemye.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.fktsv.cn/Article/details/gpmjyywnk.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.sjlbkw.cn/Article/details/gnvqsfkad.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.yfazqb.com/Article/details/gyovwyygq.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.epnwcf.com/Article/details/gmnvvikiq.sHtML

JS:   e.message;  e.stack
来源：http://m.share.bbcook.cn/Article/details/gxuephecr.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.yfazqb.com/Article/details/gsbzotfgw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.sjlbkw.cn/Article/details/gsshppylw.sHtML

Go:   err.Error()
来源：http://www.m.share.yfazqb.com/Article/details/ggllbqwob.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.sjlbkw.cn/Article/details/gvnlfsdks.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.epnwcf.com/Article/details/gsmtqtaie.sHtML

[H09] 带错误码的异常
来源：http://mobile.yfazqb.com/Article/details/gqjuurspi.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.bbcook.cn/Article/details/gmxhbicqs.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.tarul.cn/Article/details/ghloexsts.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.tarul.cn/Article/details/gehqxaxhf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.fktsv.cn/Article/details/gulxyxevh.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.bbcook.cn/Article/details/giwxjhjpi.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.yfazqb.com/Article/details/gxsvefgwa.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.fktsv.cn/Article/details/gzelifopy.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.epnwcf.com/Article/details/gamurnhvn.sHtML

[H10] 资源自动释放
来源：http://wap.yfazqb.com/Article/details/gykunaefg.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.vehdjk.com/Article/details/gbahnjzbk.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.fktsv.cn/Article/details/gqhnsjapq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.vehdjk.com/Article/details/gheoevtmp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.vehdjk.com/Article/details/grwkmwctn.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.sjlbkw.cn/Article/details/gfwvpuzah.sHtML

Go:   defer f.Close()
来源：http://wap.vehdjk.com/Article/details/gpuyrxcfn.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.vehdjk.com/Article/details/gvruayokx.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gazsftbnw.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gpxnwqdmm.sHtML

I. 正则表达式
来源：http://www.share.yfazqb.com/Article/details/goftnwoqz.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gfubudxqy.sHtML

[I01] 判断是否匹配
来源：http://3g.epnwcf.com/Article/details/geixobsjx.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.fktsv.cn/Article/details/gqkoidljr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.tarul.cn/Article/details/gqrzenmcg.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.fktsv.cn/Article/details/gemifhosz.sHtML

TS:   /\d+/.test(s)
来源：http://blog.fktsv.cn/Article/details/gjnbfwzdi.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.tarul.cn/Article/details/gvgicojrm.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.yfazqb.com/Article/details/gkresnrip.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.bbcook.cn/Article/details/gzniaywto.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.fktsv.cn/Article/details/godjxtvfc.sHtML

[I02] 提取所有匹配
来源：http://www.share.tarul.cn/Article/details/gqjsnpouf.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.epnwcf.com/Article/details/gqrfauhzm.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.vehdjk.com/Article/details/guptrnkwz.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.tarul.cn/Article/details/glicebtar.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.vehdjk.com/Article/details/gideqorjb.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.yfazqb.com/Article/details/galgoscwz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.epnwcf.com/Article/details/girxtyekn.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.fktsv.cn/Article/details/gbaehauhp.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.bbcook.cn/Article/details/gylhvaohk.sHtML

[I03] 提取捕获分组
来源：http://blog.tarul.cn/Article/details/gusgodzzp.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.tarul.cn/Article/details/grsxcmkuy.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.bbcook.cn/Article/details/gbmgqabgw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.vehdjk.com/Article/details/gafqvxrxm.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.bbcook.cn/Article/details/gyvuzikde.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.sjlbkw.cn/Article/details/gufuwzbws.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.fktsv.cn/Article/details/gthfgvhoc.sHtML


<!-- 参考信息 -->