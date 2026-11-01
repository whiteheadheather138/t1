代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://3g.sjlbkw.cn/Article/details/ggreijohp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.yfazqb.com/Article/details/gkmutgoar.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fktsv.cn/Article/details/geufgalph.sHtML

Ruby: File.size("a.txt")
来源：http://wap.vehdjk.com/Article/details/gshwqhcey.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.epnwcf.com/Article/details/gzjgwxfjy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fktsv.cn/Article/details/grujvdtrl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gmohxswbw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.yfazqb.com/Article/details/gpmrkxgzw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fktsv.cn/Article/details/gdgnphyub.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gvleybygu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.yfazqb.com/Article/details/ggnarsvgt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.vehdjk.com/Article/details/gsakopxry.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/gfdwyfyav.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.vehdjk.com/Article/details/gruxunysa.sHtML

[F11] 复制与移动文件
来源：http://www.blog.epnwcf.com/Article/details/gwpmdquus.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/gzfitvoqa.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.tarul.cn/Article/details/glckhmcnv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.vehdjk.com/Article/details/gbeeuriur.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.tarul.cn/Article/details/gwvbpmkwh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.vehdjk.com/Article/details/gpcbnscih.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.sjlbkw.cn/Article/details/gpuvolsto.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/gvkjnzfbq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.sjlbkw.cn/Article/details/ghjrlpygr.sHtML

[F12] CSV 读写
来源：http://www.share.bbcook.cn/Article/details/gtntvtudk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.vehdjk.com/Article/details/gczcgnxdq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fktsv.cn/Article/details/garzwbtdy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.bbcook.cn/Article/details/gadcirajm.sHtML

TS:   // 同上
来源：http://blog.sjlbkw.cn/Article/details/gctsgzmbq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.vehdjk.com/Article/details/gsjhsgtbf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.epnwcf.com/Article/details/gmdxqbzxc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.sjlbkw.cn/Article/details/geufhxrnr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.sjlbkw.cn/Article/details/gyvvwxlyo.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/guuaslqqz.sHtML

G. 面向对象
来源：http://www.share.tarul.cn/Article/details/gzltarzay.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gswqqwtyi.sHtML

[G01] 定义类
来源：http://blog.epnwcf.com/Article/details/gpisjrcpj.sHtML

Py:   class User: pass
来源：http://blog.tarul.cn/Article/details/gzgbizifa.sHtML

PHP:  class User {}
来源：http://www.m.share.fktsv.cn/Article/details/gbyxppnbb.sHtML

JS:   class User {}
来源：http://m.share.epnwcf.com/Article/details/gjzrylkia.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.tarul.cn/Article/details/gbkmnhxue.sHtML

Java: class User {}
来源：http://baike.bbcook.cn/Article/details/gccyrhrve.sHtML

Go:   type User struct { Name string }
来源：http://www.share.epnwcf.com/Article/details/gymbgsqbd.sHtML

Ruby: class User; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gurwmhwbg.sHtML

C#:   class User {}
来源：http://www.share.fktsv.cn/Article/details/gxhuiojpj.sHtML

[G02] 构造函数
来源：http://mobile.epnwcf.com/Article/details/gxorpufck.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.vehdjk.com/Article/details/gffurcytm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.tarul.cn/Article/details/glzxbomfk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.tarul.cn/Article/details/gxlngvhfx.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.vehdjk.com/Article/details/ggtyehxcp.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.sjlbkw.cn/Article/details/gzysiamcd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.sjlbkw.cn/Article/details/gdjovrxap.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.tarul.cn/Article/details/gjjvzolgb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gzbvnngup.sHtML

[G03] 实例属性
来源：http://read.share.epnwcf.com/Article/details/gmnsjoaxs.sHtML

Py:   self.name = "x"
来源：http://www.m.share.bbcook.cn/Article/details/gzhgyamob.sHtML

PHP:  public string $name = "x";
来源：http://www.share.bbcook.cn/Article/details/gofremowq.sHtML

JS:   this.name = "x";
来源：http://www.m.share.tarul.cn/Article/details/gxqxlrikw.sHtML

TS:   name: string = "x";
来源：http://read.share.vehdjk.com/Article/details/gvknfjlwh.sHtML

Java: private String name;
来源：http://www.share.tarul.cn/Article/details/gpdwuisyb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.yfazqb.com/Article/details/goaceixyr.sHtML

Ruby: @name = "x"
来源：http://www.m.share.epnwcf.com/Article/details/gugrqneun.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fktsv.cn/Article/details/gelhylgjo.sHtML

[G04] 定义方法
来源：http://baike.epnwcf.com/Article/details/gqcunbmna.sHtML

Py:   def greet(self): return self.name
来源：http://3g.epnwcf.com/Article/details/gbndzfzcy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.tarul.cn/Article/details/gkewlgqbb.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.epnwcf.com/Article/details/ggcpwfbhl.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fktsv.cn/Article/details/gaettrrhv.sHtML

Java: String greet() { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/glyqpftjw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.epnwcf.com/Article/details/gpxnliqrk.sHtML

Ruby: def greet; @name; end
来源：http://blog.epnwcf.com/Article/details/glzcxqvlm.sHtML

C#:   public string Greet() => Name;
来源：http://blog.epnwcf.com/Article/details/gsmiemxux.sHtML

[G05] 继承
来源：http://www.share.yfazqb.com/Article/details/gwinvzkgt.sHtML

Py:   class Admin(User): pass
来源：http://read.share.bbcook.cn/Article/details/gatmtdqfn.sHtML

PHP:  class Admin extends User {}
来源：http://baike.tarul.cn/Article/details/gdhnburfb.sHtML

JS:   class Admin extends User {}
来源：http://wap.epnwcf.com/Article/details/gubrprijv.sHtML

TS:   class Admin extends User {}
来源：http://read.share.tarul.cn/Article/details/gueqffdso.sHtML

Java: class Admin extends User {}
来源：http://mobile.tarul.cn/Article/details/guggafext.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.tarul.cn/Article/details/ggppshyed.sHtML

Ruby: class Admin < User; end
来源：http://www.share.sjlbkw.cn/Article/details/gziklntnu.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fktsv.cn/Article/details/gihnfxaiu.sHtML

[G06] 重写方法
来源：http://wap.fktsv.cn/Article/details/gysrmwkxs.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.bbcook.cn/Article/details/gdtkvskfh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.bbcook.cn/Article/details/gwjnibzjw.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.yfazqb.com/Article/details/gxguqclmr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.yfazqb.com/Article/details/gxqgliofe.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.vehdjk.com/Article/details/gdszckblk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.epnwcf.com/Article/details/gocxtcarx.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.vehdjk.com/Article/details/gjdcizhpd.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.sjlbkw.cn/Article/details/gzmelkypx.sHtML

[G07] 调用父类方法
来源：http://read.share.yfazqb.com/Article/details/gqteyptgi.sHtML

Py:   super().greet()
来源：http://www.m.share.bbcook.cn/Article/details/guarhipyy.sHtML

PHP:  parent::greet();
来源：http://www.blog.vehdjk.com/Article/details/ghrxfxofo.sHtML

JS:   super.greet();
来源：http://www.share.yfazqb.com/Article/details/guiuqmgqv.sHtML

TS:   super.greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gxpkzdkhn.sHtML

Java: super.greet();
来源：http://www.share.epnwcf.com/Article/details/gmlvssdwy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.vehdjk.com/Article/details/gpapfpxqk.sHtML

Ruby: super
来源：http://www.share.fktsv.cn/Article/details/gjbbkbxfp.sHtML

C#:   base.Greet();
来源：http://www.m.share.epnwcf.com/Article/details/gmanhqktu.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.sjlbkw.cn/Article/details/glxrezksq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.tarul.cn/Article/details/gcriwbtvl.sHtML

PHP:  public static function f() {}
来源：http://www.blog.bbcook.cn/Article/details/gtrqzuspq.sHtML

JS:   static f() {}
来源：http://3g.vehdjk.com/Article/details/gdkgodbrz.sHtML

TS:   static f(): void {}
来源：http://mobile.fktsv.cn/Article/details/guyinkakh.sHtML

Java: static void f() {}
来源：http://wap.sjlbkw.cn/Article/details/gurcdhypj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.vehdjk.com/Article/details/gfsrjuzec.sHtML

Ruby: def self.f; end
来源：http://www.share.vehdjk.com/Article/details/gikwuxiks.sHtML

C#:   public static void F() {}
来源：http://mobile.sjlbkw.cn/Article/details/ghictyftn.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.epnwcf.com/Article/details/gqvybcmma.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.yfazqb.com/Article/details/ghucppxkr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fktsv.cn/Article/details/gftiyslmv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.yfazqb.com/Article/details/gtibhtkft.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.yfazqb.com/Article/details/glquvbyiz.sHtML

Java: interface Shape { double area(); }
来源：http://blog.yfazqb.com/Article/details/gmxixqxug.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.epnwcf.com/Article/details/gqbliiwkj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.vehdjk.com/Article/details/gtusfvtly.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.bbcook.cn/Article/details/gyboxmttm.sHtML

[G10] 访问控制
来源：http://baike.sjlbkw.cn/Article/details/gmjjzjhpx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.tarul.cn/Article/details/gwzcolicg.sHtML

PHP:  public / protected / private
来源：http://www.share.epnwcf.com/Article/details/gzamypors.sHtML

JS:   #private 字段；其余公开
来源：http://baike.sjlbkw.cn/Article/details/gvagplntm.sHtML

TS:   public / protected / private
来源：http://wap.epnwcf.com/Article/details/grddziagh.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.epnwcf.com/Article/details/gynegdhxo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.sjlbkw.cn/Article/details/gsqfououd.sHtML

Ruby: public / protected / private
来源：http://www.m.share.tarul.cn/Article/details/gvntkgfzn.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fktsv.cn/Article/details/gvvjtdvbc.sHtML

[G11] getter / setter
来源：http://blog.tarul.cn/Article/details/gjfybmfzc.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.bbcook.cn/Article/details/gzjmqoqxm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.epnwcf.com/Article/details/gfrohhwxf.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.vehdjk.com/Article/details/gazjlizhs.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fktsv.cn/Article/details/gznkoybei.sHtML

Java: public String getName() { return name; }
来源：http://3g.sjlbkw.cn/Article/details/glslwbypz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fktsv.cn/Article/details/grlktxyhh.sHtML

Ruby: attr_accessor :name
来源：http://mobile.epnwcf.com/Article/details/gaqnonoyi.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fktsv.cn/Article/details/gewouvefd.sHtML

[G12] 对象转字符串
来源：http://www.m.share.epnwcf.com/Article/details/gqeiaiwwa.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.epnwcf.com/Article/details/ggdbprxuu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.bbcook.cn/Article/details/gycqsqbda.sHtML

JS:   toString() { return this.name; }
来源：http://wap.bbcook.cn/Article/details/ghuyslwhu.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.epnwcf.com/Article/details/gkoadfvxz.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fktsv.cn/Article/details/ggdlduwyk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fktsv.cn/Article/details/gltlkakgm.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fktsv.cn/Article/details/gjxhxolmi.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.vehdjk.com/Article/details/gdoulljgs.sHtML

[G13] 判断对象类型
来源：http://www.m.share.vehdjk.com/Article/details/gnyndufig.sHtML

Py:   isinstance(u, User)
来源：http://blog.fktsv.cn/Article/details/gnitzdeod.sHtML

PHP:  $u instanceof User
来源：http://3g.bbcook.cn/Article/details/gczuiqzyc.sHtML

JS:   u instanceof User
来源：http://blog.tarul.cn/Article/details/gfqlpsdpi.sHtML

TS:   u instanceof User
来源：http://blog.yfazqb.com/Article/details/ghqfmabvi.sHtML

Java: u instanceof User
来源：http://baike.yfazqb.com/Article/details/gwyvpnpwe.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.vehdjk.com/Article/details/gskucdlqb.sHtML

Ruby: u.is_a?(User)
来源：http://wap.bbcook.cn/Article/details/glgfdhwmm.sHtML

C#:   u is User
来源：http://read.share.vehdjk.com/Article/details/gwrnyqtuv.sHtML

[G14] 数据类 / record
来源：http://baike.vehdjk.com/Article/details/gpabhvgkj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.sjlbkw.cn/Article/details/gfaluzabx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fktsv.cn/Article/details/gvfglhdoi.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fktsv.cn/Article/details/gpyblgdkj.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.vehdjk.com/Article/details/gvxtbezzy.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.sjlbkw.cn/Article/details/gfuiyyjbu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.vehdjk.com/Article/details/gzcxtmfwu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.epnwcf.com/Article/details/gdrvpneac.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.bbcook.cn/Article/details/gguiibfxv.sHtML

[G15] 枚举
来源：http://www.blog.epnwcf.com/Article/details/gmgtpykqo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.sjlbkw.cn/Article/details/gizmvqpmk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.vehdjk.com/Article/details/genfzkutt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.tarul.cn/Article/details/ggkvvtpxr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.yfazqb.com/Article/details/ghiwcxecu.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.yfazqb.com/Article/details/gcyzbrbmc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fktsv.cn/Article/details/gukvvvfod.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.bbcook.cn/Article/details/gywtbwsfw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fktsv.cn/Article/details/gguwyknmh.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.bbcook.cn/Article/details/gvzdphusa.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.yfazqb.com/Article/details/gsadlsjta.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.tarul.cn/Article/details/gypoecnwj.sHtML

JS:   Object.entries(obj)
来源：http://m.share.bbcook.cn/Article/details/guvmpzckw.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gvihduyiy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.epnwcf.com/Article/details/gwausbxhj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.yfazqb.com/Article/details/gyjkowdxl.sHtML

Ruby: obj.instance_variables
来源：http://wap.yfazqb.com/Article/details/gbxlyksch.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.vehdjk.com/Article/details/gxlqsontw.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/ghsxyizov.sHtML

H. 异常与错误处理
来源：http://3g.tarul.cn/Article/details/gesakmzsv.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gtxzssbju.sHtML

[H01] try / catch 基础
来源：http://m.share.bbcook.cn/Article/details/gpuifhqno.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.epnwcf.com/Article/details/gifivdncn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.vehdjk.com/Article/details/gqnqkugjo.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.tarul.cn/Article/details/gyhipeulo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fktsv.cn/Article/details/gtizjubbo.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.tarul.cn/Article/details/gbdprqwza.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.sjlbkw.cn/Article/details/gecpotwwn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.sjlbkw.cn/Article/details/gqjxygevr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fktsv.cn/Article/details/gyyssxhzr.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.sjlbkw.cn/Article/details/ghdjxtdym.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.sjlbkw.cn/Article/details/gzwkcxbdp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.tarul.cn/Article/details/gyntvqzvd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/gsngbcqbz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fktsv.cn/Article/details/gkxqurskq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.yfazqb.com/Article/details/ggjfuepok.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fktsv.cn/Article/details/gntmevrdx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.sjlbkw.cn/Article/details/gsdaubwjh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.vehdjk.com/Article/details/gvgskcjap.sHtML

[H03] 主动抛出异常
来源：http://www.blog.tarul.cn/Article/details/gbrkxthpx.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.epnwcf.com/Article/details/gwuslepwy.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.tarul.cn/Article/details/gdwojnuze.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.epnwcf.com/Article/details/gxujsxzev.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.vehdjk.com/Article/details/ggpxeiogq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.tarul.cn/Article/details/grxwtaaei.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.vehdjk.com/Article/details/gpgilxybx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.sjlbkw.cn/Article/details/gvhbgyusd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gfxsqiqee.sHtML

[H04] 自定义异常类型
来源：http://read.share.sjlbkw.cn/Article/details/gcnpwjhdw.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.tarul.cn/Article/details/gywkqdcgj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fktsv.cn/Article/details/grbujqoqv.sHtML

JS:   class MyError extends Error {}
来源：http://blog.yfazqb.com/Article/details/gtelrpshj.sHtML

TS:   class MyError extends Error {}
来源：http://wap.sjlbkw.cn/Article/details/gwmeaaqbm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.epnwcf.com/Article/details/gjcwthzha.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fktsv.cn/Article/details/gprjnezry.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.tarul.cn/Article/details/gaexvrfai.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.bbcook.cn/Article/details/gsrfexfyd.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.epnwcf.com/Article/details/gbgbzekrn.sHtML

Py:   except ValueError as e:
来源：http://read.share.yfazqb.com/Article/details/gpkdepuwe.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.yfazqb.com/Article/details/gkyhiwxtd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.vehdjk.com/Article/details/gxivosscq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.vehdjk.com/Article/details/gnytgfacf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.sjlbkw.cn/Article/details/gtllhyart.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.epnwcf.com/Article/details/gubcpmhxi.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.yfazqb.com/Article/details/gvrfowiyl.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.epnwcf.com/Article/details/grvismgod.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.sjlbkw.cn/Article/details/glywqufzw.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.epnwcf.com/Article/details/gtlqqvilw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.fktsv.cn/Article/details/gonqsfkog.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fktsv.cn/Article/details/gsgsmrncg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.epnwcf.com/Article/details/gfoyytxme.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.epnwcf.com/Article/details/gvwjmevxl.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.epnwcf.com/Article/details/gafwutjir.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.sjlbkw.cn/Article/details/gvaunddyq.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.epnwcf.com/Article/details/gpsgvolca.sHtML

[H07] 断言
来源：http://www.share.vehdjk.com/Article/details/gilmpffiz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.tarul.cn/Article/details/gfafifvgj.sHtML

PHP:  assert($x > 0);
来源：http://mobile.yfazqb.com/Article/details/gwniihpfb.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.bbcook.cn/Article/details/gooflfnjn.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.yfazqb.com/Article/details/ggrhyghrx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.sjlbkw.cn/Article/details/gmubeveba.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.bbcook.cn/Article/details/gjphkprpj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.vehdjk.com/Article/details/gdmacfoxu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.yfazqb.com/Article/details/grawrgadp.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.tarul.cn/Article/details/gpbdxbvdj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.tarul.cn/Article/details/ggosdmpdj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.yfazqb.com/Article/details/gwbkoeuax.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.epnwcf.com/Article/details/gnmbseupd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.fktsv.cn/Article/details/gsqhmgukb.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fktsv.cn/Article/details/gfkaobgqr.sHtML

Go:   err.Error()
来源：http://blog.epnwcf.com/Article/details/gomsqdwaq.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.epnwcf.com/Article/details/gjckpehfl.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.vehdjk.com/Article/details/gqfviilsc.sHtML

[H09] 带错误码的异常
来源：http://m.share.bbcook.cn/Article/details/grwybkrib.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.bbcook.cn/Article/details/gpvfjqgvp.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.vehdjk.com/Article/details/guviodkde.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.vehdjk.com/Article/details/gnvemobww.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.tarul.cn/Article/details/gpbkpgdfp.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.vehdjk.com/Article/details/gxfilbnuj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.yfazqb.com/Article/details/gnlqgnmey.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.fktsv.cn/Article/details/gliinspib.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.tarul.cn/Article/details/ggyzeepmh.sHtML

[H10] 资源自动释放
来源：http://baike.fktsv.cn/Article/details/gykvlrhjo.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.bbcook.cn/Article/details/grlsgekgy.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.sjlbkw.cn/Article/details/gipzjujsu.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.vehdjk.com/Article/details/gmruagwor.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fktsv.cn/Article/details/ggfxzwgsd.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.yfazqb.com/Article/details/ggzjtazdp.sHtML

Go:   defer f.Close()
来源：http://read.share.vehdjk.com/Article/details/gmqikvkye.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.fktsv.cn/Article/details/ggowutjsg.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gddmrebaw.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gasorfznj.sHtML

I. 正则表达式
来源：http://www.blog.tarul.cn/Article/details/gogczvzux.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/ggiumcjdl.sHtML

[I01] 判断是否匹配
来源：http://www.share.tarul.cn/Article/details/gkuhxfnqf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.sjlbkw.cn/Article/details/gajotrphk.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.tarul.cn/Article/details/glsadexwv.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.fktsv.cn/Article/details/gtgkvqmco.sHtML

TS:   /\d+/.test(s)
来源：http://baike.tarul.cn/Article/details/grzmlzavl.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.sjlbkw.cn/Article/details/gegpbbvts.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fktsv.cn/Article/details/gtygwmnzk.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.fktsv.cn/Article/details/gavxrnhbx.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.tarul.cn/Article/details/gkntmcnsj.sHtML

[I02] 提取所有匹配
来源：http://read.share.sjlbkw.cn/Article/details/gijfspgkw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.tarul.cn/Article/details/ghxzwjbgf.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.epnwcf.com/Article/details/gmgolgxmb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.fktsv.cn/Article/details/guuhljrgx.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.fktsv.cn/Article/details/gyxbmizob.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.sjlbkw.cn/Article/details/gwfcinswp.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.vehdjk.com/Article/details/gamwlseut.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.vehdjk.com/Article/details/gnqnvzocb.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.fktsv.cn/Article/details/gkitgfaon.sHtML

[I03] 提取捕获分组
来源：http://mobile.bbcook.cn/Article/details/glvcdvvru.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.bbcook.cn/Article/details/gcafjkunj.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.epnwcf.com/Article/details/gythczvxt.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.vehdjk.com/Article/details/gghfmkhxg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.fktsv.cn/Article/details/ghxxhnodk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.epnwcf.com/Article/details/gochjprcr.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.vehdjk.com/Article/details/goaktuchi.sHtML


<!-- 参考信息 -->