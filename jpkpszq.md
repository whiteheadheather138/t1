代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.bbcook.cn/Article/details/gyvzmdpmm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.tarul.cn/Article/details/gexndwjkr.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.tarul.cn/Article/details/gxgqaxbnu.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.tarul.cn/Article/details/gexspkjsk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fktsv.cn/Article/details/gvnqmqncy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.vehdjk.com/Article/details/grlvjpxkq.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fktsv.cn/Article/details/gcmaniqlr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.epnwcf.com/Article/details/gqzcwfuks.sHtML

[F09] 获取文件大小
来源：http://read.share.tarul.cn/Article/details/gonjtmrdr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.tarul.cn/Article/details/gqvbhpuai.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gbruzwccw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.epnwcf.com/Article/details/gbmhifcrs.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.yfazqb.com/Article/details/gjnxzcrox.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.epnwcf.com/Article/details/gwfmxehla.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.epnwcf.com/Article/details/glmcmfpfi.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gdfiqzcxr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.epnwcf.com/Article/details/gvwbvkgqa.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.yfazqb.com/Article/details/gkxskuxzi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/gbiytnidy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.bbcook.cn/Article/details/guegfydle.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/gvueeutdg.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gqkrpxpwn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.sjlbkw.cn/Article/details/gsoudvomx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/gggyzmgiv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fktsv.cn/Article/details/glnuinrrj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/ggmadahad.sHtML

[F11] 复制与移动文件
来源：http://mobile.fktsv.cn/Article/details/gtlvuxlub.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/ghykwrszx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.bbcook.cn/Article/details/gbokhqqpv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.tarul.cn/Article/details/gchvqogms.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.bbcook.cn/Article/details/geyvrhvby.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.tarul.cn/Article/details/gmbxnpcgp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.epnwcf.com/Article/details/gzmjwbxcm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.tarul.cn/Article/details/glhznuxmy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.sjlbkw.cn/Article/details/gzzeuatod.sHtML

[F12] CSV 读写
来源：http://read.share.epnwcf.com/Article/details/gsxxsujdo.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.sjlbkw.cn/Article/details/gphwdsoll.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.sjlbkw.cn/Article/details/grblttkxz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.sjlbkw.cn/Article/details/gjfrrcxib.sHtML

TS:   // 同上
来源：http://read.share.bbcook.cn/Article/details/gmzwqymwb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.bbcook.cn/Article/details/gvphecgxa.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.sjlbkw.cn/Article/details/gxpenepdp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.tarul.cn/Article/details/gfyhqtmqx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.epnwcf.com/Article/details/gncqnimqt.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gfhilxaml.sHtML

G. 面向对象
来源：http://mobile.sjlbkw.cn/Article/details/gtnphctaq.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/geqnnvsfv.sHtML

[G01] 定义类
来源：http://m.share.yfazqb.com/Article/details/gbgjldkvk.sHtML

Py:   class User: pass
来源：http://baike.yfazqb.com/Article/details/gtswejhoe.sHtML

PHP:  class User {}
来源：http://m.share.bbcook.cn/Article/details/gwacbchph.sHtML

JS:   class User {}
来源：http://3g.bbcook.cn/Article/details/grwlqzvuw.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.yfazqb.com/Article/details/gugzhrcwj.sHtML

Java: class User {}
来源：http://www.share.tarul.cn/Article/details/gmdrvxhbm.sHtML

Go:   type User struct { Name string }
来源：http://3g.fktsv.cn/Article/details/gjnqbogvw.sHtML

Ruby: class User; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gzlaavecn.sHtML

C#:   class User {}
来源：http://blog.yfazqb.com/Article/details/gzxdobuir.sHtML

[G02] 构造函数
来源：http://wap.yfazqb.com/Article/details/galcvjlgx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.vehdjk.com/Article/details/gibunusqf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.tarul.cn/Article/details/gebqtekya.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gsibpamas.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.sjlbkw.cn/Article/details/gdwzfslwl.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.sjlbkw.cn/Article/details/goigyqmvz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.epnwcf.com/Article/details/gxnuyvlyb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.bbcook.cn/Article/details/gbdkbfgja.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fktsv.cn/Article/details/gevtnizky.sHtML

[G03] 实例属性
来源：http://read.share.vehdjk.com/Article/details/gkkikyshh.sHtML

Py:   self.name = "x"
来源：http://read.share.bbcook.cn/Article/details/gvhlrfcun.sHtML

PHP:  public string $name = "x";
来源：http://m.share.tarul.cn/Article/details/gxnbinwml.sHtML

JS:   this.name = "x";
来源：http://baike.bbcook.cn/Article/details/gmiybezgq.sHtML

TS:   name: string = "x";
来源：http://www.m.share.vehdjk.com/Article/details/gfsruwlun.sHtML

Java: private String name;
来源：http://blog.yfazqb.com/Article/details/gugqewfcc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fktsv.cn/Article/details/gzyllknjd.sHtML

Ruby: @name = "x"
来源：http://mobile.yfazqb.com/Article/details/gguhwenhs.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.sjlbkw.cn/Article/details/geizuxrln.sHtML

[G04] 定义方法
来源：http://read.share.fktsv.cn/Article/details/gofrkswhd.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.yfazqb.com/Article/details/gqvyqtgzb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fktsv.cn/Article/details/gnbluimyt.sHtML

JS:   greet() { return this.name; }
来源：http://blog.tarul.cn/Article/details/gqartqxhb.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.yfazqb.com/Article/details/glvjotcmv.sHtML

Java: String greet() { return name; }
来源：http://wap.bbcook.cn/Article/details/gzfdsdxbr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.yfazqb.com/Article/details/gowcvjkov.sHtML

Ruby: def greet; @name; end
来源：http://mobile.tarul.cn/Article/details/ggtwhkpzl.sHtML

C#:   public string Greet() => Name;
来源：http://blog.yfazqb.com/Article/details/gcgfnlkim.sHtML

[G05] 继承
来源：http://www.m.share.yfazqb.com/Article/details/glglpyttg.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.epnwcf.com/Article/details/gkpkvbtrc.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/gaducvugm.sHtML

JS:   class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/gpucrkpmk.sHtML

TS:   class Admin extends User {}
来源：http://wap.epnwcf.com/Article/details/gbktgalsl.sHtML

Java: class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/guirihxme.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.yfazqb.com/Article/details/gorfastuq.sHtML

Ruby: class Admin < User; end
来源：http://read.share.sjlbkw.cn/Article/details/gxzpskfqo.sHtML

C#:   class Admin : User {}
来源：http://blog.vehdjk.com/Article/details/gabgzjjhp.sHtML

[G06] 重写方法
来源：http://www.blog.vehdjk.com/Article/details/gkqioxllp.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.bbcook.cn/Article/details/gxufjawwh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fktsv.cn/Article/details/gdtuzkjqu.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.bbcook.cn/Article/details/gwmtkcmpq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/ghrnapjtr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.tarul.cn/Article/details/guybiugxh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.yfazqb.com/Article/details/gdatpqyii.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.tarul.cn/Article/details/giacviklj.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fktsv.cn/Article/details/ghrsnjmyp.sHtML

[G07] 调用父类方法
来源：http://mobile.bbcook.cn/Article/details/gfsblbceu.sHtML

Py:   super().greet()
来源：http://www.blog.sjlbkw.cn/Article/details/grishlduf.sHtML

PHP:  parent::greet();
来源：http://read.share.epnwcf.com/Article/details/gxyajsbmy.sHtML

JS:   super.greet();
来源：http://mobile.vehdjk.com/Article/details/gowkuousn.sHtML

TS:   super.greet();
来源：http://read.share.tarul.cn/Article/details/giwhvcchr.sHtML

Java: super.greet();
来源：http://baike.yfazqb.com/Article/details/gsdhnimet.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.vehdjk.com/Article/details/gckctacgz.sHtML

Ruby: super
来源：http://baike.fktsv.cn/Article/details/ggzhikkta.sHtML

C#:   base.Greet();
来源：http://3g.vehdjk.com/Article/details/gamsmwzjn.sHtML

[G08] 静态方法与属性
来源：http://3g.epnwcf.com/Article/details/gkkevqvsj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.vehdjk.com/Article/details/gcsdqkwrk.sHtML

PHP:  public static function f() {}
来源：http://baike.tarul.cn/Article/details/gtiiisfjg.sHtML

JS:   static f() {}
来源：http://m.share.epnwcf.com/Article/details/gsuikinio.sHtML

TS:   static f(): void {}
来源：http://www.m.share.bbcook.cn/Article/details/gmvgfksur.sHtML

Java: static void f() {}
来源：http://wap.vehdjk.com/Article/details/gvysjndbh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.bbcook.cn/Article/details/gzihjwmck.sHtML

Ruby: def self.f; end
来源：http://baike.tarul.cn/Article/details/gjkevlvhb.sHtML

C#:   public static void F() {}
来源：http://wap.yfazqb.com/Article/details/grozzxleg.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.yfazqb.com/Article/details/gqkjdtxuv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.vehdjk.com/Article/details/gmjolroas.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.bbcook.cn/Article/details/gtmjcprge.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.bbcook.cn/Article/details/glqtenfla.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.yfazqb.com/Article/details/gvzdeykdu.sHtML

Java: interface Shape { double area(); }
来源：http://3g.sjlbkw.cn/Article/details/gwzzidmfq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.sjlbkw.cn/Article/details/gojorukfr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.sjlbkw.cn/Article/details/ghcovovvz.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.yfazqb.com/Article/details/giqgqgent.sHtML

[G10] 访问控制
来源：http://m.share.vehdjk.com/Article/details/gkttryidu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.epnwcf.com/Article/details/gvtqnslxw.sHtML

PHP:  public / protected / private
来源：http://blog.sjlbkw.cn/Article/details/ggfawmscj.sHtML

JS:   #private 字段；其余公开
来源：http://wap.tarul.cn/Article/details/gvfwmhwog.sHtML

TS:   public / protected / private
来源：http://blog.vehdjk.com/Article/details/gdijesqum.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.bbcook.cn/Article/details/gejcfwiga.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fktsv.cn/Article/details/germfwpiy.sHtML

Ruby: public / protected / private
来源：http://www.m.share.yfazqb.com/Article/details/goqjyatfn.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.bbcook.cn/Article/details/gttqouwyb.sHtML

[G11] getter / setter
来源：http://www.blog.vehdjk.com/Article/details/gnnwkykmo.sHtML

Py:   @property 与 @x.setter
来源：http://blog.vehdjk.com/Article/details/gtakwotam.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.yfazqb.com/Article/details/gdwttftdl.sHtML

JS:   get name() { return this._name; }
来源：http://3g.tarul.cn/Article/details/gklcemheg.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.yfazqb.com/Article/details/gwtjwptlf.sHtML

Java: public String getName() { return name; }
来源：http://mobile.tarul.cn/Article/details/gcnyhhktq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fktsv.cn/Article/details/gnvjlgrht.sHtML

Ruby: attr_accessor :name
来源：http://3g.yfazqb.com/Article/details/gcxsjilmv.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.vehdjk.com/Article/details/gweqfmaya.sHtML

[G12] 对象转字符串
来源：http://wap.yfazqb.com/Article/details/gxhtyhhdy.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.yfazqb.com/Article/details/gswpcaogz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.bbcook.cn/Article/details/gmuedudym.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.vehdjk.com/Article/details/glyuywzxi.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.vehdjk.com/Article/details/guizyivws.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.epnwcf.com/Article/details/gdjbmspqy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.tarul.cn/Article/details/gmpkvhpbz.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.sjlbkw.cn/Article/details/geonsogrv.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.yfazqb.com/Article/details/genzwgntx.sHtML

[G13] 判断对象类型
来源：http://wap.tarul.cn/Article/details/gtyblqslg.sHtML

Py:   isinstance(u, User)
来源：http://baike.sjlbkw.cn/Article/details/gwsdekdty.sHtML

PHP:  $u instanceof User
来源：http://3g.tarul.cn/Article/details/gukjiycgy.sHtML

JS:   u instanceof User
来源：http://wap.epnwcf.com/Article/details/gwtbahzvw.sHtML

TS:   u instanceof User
来源：http://www.m.share.fktsv.cn/Article/details/gczuctuet.sHtML

Java: u instanceof User
来源：http://blog.epnwcf.com/Article/details/grrqtgvxt.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.bbcook.cn/Article/details/gxszpkheg.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fktsv.cn/Article/details/gdtnvppko.sHtML

C#:   u is User
来源：http://www.share.tarul.cn/Article/details/gdaojfeoh.sHtML

[G14] 数据类 / record
来源：http://blog.vehdjk.com/Article/details/gvmfcbagf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fktsv.cn/Article/details/ggefacbkd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.tarul.cn/Article/details/gkcaxsgfz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fktsv.cn/Article/details/giygftbbj.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.sjlbkw.cn/Article/details/gpweabiur.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fktsv.cn/Article/details/gsvaenxak.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fktsv.cn/Article/details/ghxukflmj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fktsv.cn/Article/details/gotxyzbyd.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fktsv.cn/Article/details/gkibgctvg.sHtML

[G15] 枚举
来源：http://3g.sjlbkw.cn/Article/details/gfasixdgh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.bbcook.cn/Article/details/gpxxsvizh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.sjlbkw.cn/Article/details/gdgkuqrie.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.sjlbkw.cn/Article/details/grsvhizpa.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fktsv.cn/Article/details/ggymtvlje.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.vehdjk.com/Article/details/grexdkero.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.tarul.cn/Article/details/gtkjoydhp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.yfazqb.com/Article/details/gbuulinfn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.yfazqb.com/Article/details/glmrvrygy.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.yfazqb.com/Article/details/gfpmyyruo.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.yfazqb.com/Article/details/gabjgqebp.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.epnwcf.com/Article/details/gzgzlhxvy.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.epnwcf.com/Article/details/gnujngueg.sHtML

TS:   Object.entries(obj)
来源：http://read.share.epnwcf.com/Article/details/gmeiyiifa.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.vehdjk.com/Article/details/gnerzkigw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.sjlbkw.cn/Article/details/gsufvgqzw.sHtML

Ruby: obj.instance_variables
来源：http://mobile.yfazqb.com/Article/details/guwnkaror.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fktsv.cn/Article/details/gbgyksqdg.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gbsnvlyrz.sHtML

H. 异常与错误处理
来源：http://mobile.tarul.cn/Article/details/gimfocywr.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gktjwzuya.sHtML

[H01] try / catch 基础
来源：http://m.share.fktsv.cn/Article/details/gyhjqxsxf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fktsv.cn/Article/details/grwcxatxe.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.vehdjk.com/Article/details/ghnqryupi.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.sjlbkw.cn/Article/details/gjlhqetyk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.tarul.cn/Article/details/grbqayunk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.yfazqb.com/Article/details/gikslxoub.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.yfazqb.com/Article/details/gnvrhnopl.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.yfazqb.com/Article/details/gwxybjbzk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.sjlbkw.cn/Article/details/gyntdcuex.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.yfazqb.com/Article/details/gxnanokbu.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.bbcook.cn/Article/details/gybijixdn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.sjlbkw.cn/Article/details/gkegvupju.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.tarul.cn/Article/details/gremkpciz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/gaobqfmhn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/gynvzrcaz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.epnwcf.com/Article/details/goegtdssx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.yfazqb.com/Article/details/gkedeurnp.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/gtezjzqyv.sHtML

[H03] 主动抛出异常
来源：http://3g.vehdjk.com/Article/details/gfilnndmd.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.sjlbkw.cn/Article/details/gkjrtfddu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.sjlbkw.cn/Article/details/gfusdbdnw.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.epnwcf.com/Article/details/gvgfmioqu.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/gvrcejkci.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.tarul.cn/Article/details/gzpbfsczj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.epnwcf.com/Article/details/gzbapmmhf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.tarul.cn/Article/details/goxucvskb.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.epnwcf.com/Article/details/gpartaihb.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.vehdjk.com/Article/details/ggvukxdnx.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.yfazqb.com/Article/details/gpxihwmnd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.epnwcf.com/Article/details/ghxnzmvzt.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.yfazqb.com/Article/details/gyfusvxke.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.tarul.cn/Article/details/gurypjhdb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fktsv.cn/Article/details/grqilwjdi.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.bbcook.cn/Article/details/glsxpzazb.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fktsv.cn/Article/details/geeyextvy.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.sjlbkw.cn/Article/details/gzqgvyepj.sHtML

[H05] 捕获特定类型
来源：http://baike.epnwcf.com/Article/details/gqrcfihmg.sHtML

Py:   except ValueError as e:
来源：http://mobile.yfazqb.com/Article/details/gxbuifvru.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.bbcook.cn/Article/details/gkorckeqw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.bbcook.cn/Article/details/ghunawutg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fktsv.cn/Article/details/gckigcdby.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.vehdjk.com/Article/details/gwycunzfr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfzdjuikm.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fktsv.cn/Article/details/grgwlrgxn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.yfazqb.com/Article/details/gcquuaotu.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.yfazqb.com/Article/details/gqyxmsyrk.sHtML

Py:   value = d.get("k") or default
来源：http://blog.sjlbkw.cn/Article/details/gpepghoqv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fktsv.cn/Article/details/gilhiglvn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.sjlbkw.cn/Article/details/gfwpmgxlp.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.tarul.cn/Article/details/guvbjhuks.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.fktsv.cn/Article/details/gqgspgxmb.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.vehdjk.com/Article/details/gutzjnwxn.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.epnwcf.com/Article/details/gadlqeopz.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.yfazqb.com/Article/details/gjzgylykv.sHtML

[H07] 断言
来源：http://baike.sjlbkw.cn/Article/details/gzqnyrdbf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.epnwcf.com/Article/details/gghnxmwnm.sHtML

PHP:  assert($x > 0);
来源：http://read.share.sjlbkw.cn/Article/details/ghufdyksu.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.vehdjk.com/Article/details/gvyljeiil.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.vehdjk.com/Article/details/grvvthksb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.fktsv.cn/Article/details/gcmwhpugf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.tarul.cn/Article/details/gxwbmbcxq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.tarul.cn/Article/details/gecoxxbxg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.fktsv.cn/Article/details/gwjzzqufn.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.yfazqb.com/Article/details/grjqjtatf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.epnwcf.com/Article/details/gazaqisml.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.bbcook.cn/Article/details/gvqkchvtf.sHtML

JS:   e.message;  e.stack
来源：http://wap.tarul.cn/Article/details/glmrizgzd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.tarul.cn/Article/details/gzaahcekr.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fktsv.cn/Article/details/gcusviqlz.sHtML

Go:   err.Error()
来源：http://mobile.tarul.cn/Article/details/gquegwfge.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.vehdjk.com/Article/details/gbuaiqddt.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.fktsv.cn/Article/details/gmzkpilbl.sHtML

[H09] 带错误码的异常
来源：http://m.share.sjlbkw.cn/Article/details/gurpuzjpn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.tarul.cn/Article/details/gknpibszh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.tarul.cn/Article/details/gdurqurmf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.vehdjk.com/Article/details/giiehcgch.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.vehdjk.com/Article/details/gnnurkxhb.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.yfazqb.com/Article/details/ggguivwtk.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.epnwcf.com/Article/details/gldegoaey.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fktsv.cn/Article/details/glqijjwyh.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.yfazqb.com/Article/details/gqxjusjsi.sHtML

[H10] 资源自动释放
来源：http://www.share.fktsv.cn/Article/details/geyynrkkc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.bbcook.cn/Article/details/gurtwjxip.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.vehdjk.com/Article/details/gslnacbun.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.tarul.cn/Article/details/gwpnzfdwg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fktsv.cn/Article/details/gyuaakhjy.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.yfazqb.com/Article/details/grlxhoojn.sHtML

Go:   defer f.Close()
来源：http://mobile.yfazqb.com/Article/details/gftiwrbwt.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.bbcook.cn/Article/details/gomgacqbh.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gftslbexe.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gomvzqquy.sHtML

I. 正则表达式
来源：http://www.m.share.epnwcf.com/Article/details/gvojxfphr.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gfwhdublm.sHtML

[I01] 判断是否匹配
来源：http://baike.yfazqb.com/Article/details/gvoqwbthu.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.yfazqb.com/Article/details/gpblpdvtr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gbaajlelk.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.epnwcf.com/Article/details/gfnzjgrbt.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.epnwcf.com/Article/details/gmhnnkduy.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.tarul.cn/Article/details/gklrioapg.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.fktsv.cn/Article/details/gctsrrutr.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.fktsv.cn/Article/details/gwcqminhc.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.fktsv.cn/Article/details/glmxvyfbs.sHtML

[I02] 提取所有匹配
来源：http://wap.epnwcf.com/Article/details/gsrnnsuij.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.tarul.cn/Article/details/grqvmspui.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.fktsv.cn/Article/details/gdkyyagti.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.fktsv.cn/Article/details/gwxwmwxnw.sHtML


<!-- 参考信息 -->