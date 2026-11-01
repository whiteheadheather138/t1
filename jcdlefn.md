代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/glqoivuon.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gvjablund.sHtML

[F11] 复制与移动文件
来源：http://3g.bbcook.cn/Article/details/grinsaars.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.yfazqb.com/Article/details/gbxrtbbus.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gnzjyvtpe.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gfsguhhhx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gnhynkqtm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.tarul.cn/Article/details/gattjxara.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.vehdjk.com/Article/details/govsbfbda.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/gwjhwakwe.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.yfazqb.com/Article/details/gpioxbesn.sHtML

[F12] CSV 读写
来源：http://blog.sjlbkw.cn/Article/details/guvntyejj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fktsv.cn/Article/details/ghpnbmqmx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.epnwcf.com/Article/details/gslqlmdki.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.bbcook.cn/Article/details/gdoyhoqzo.sHtML

TS:   // 同上
来源：http://m.share.sjlbkw.cn/Article/details/gkqcpyknt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.yfazqb.com/Article/details/gmuzvkiva.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.yfazqb.com/Article/details/gpoislglr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.vehdjk.com/Article/details/gijyvjgpa.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.yfazqb.com/Article/details/guwjotlny.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gqxcdpajy.sHtML

G. 面向对象
来源：http://www.share.yfazqb.com/Article/details/gwkoivpxb.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gvqphiemj.sHtML

[G01] 定义类
来源：http://wap.tarul.cn/Article/details/ggvzurilk.sHtML

Py:   class User: pass
来源：http://baike.epnwcf.com/Article/details/gbgaslibq.sHtML

PHP:  class User {}
来源：http://read.share.tarul.cn/Article/details/gupglicbr.sHtML

JS:   class User {}
来源：http://www.m.share.fktsv.cn/Article/details/gwuodcwhr.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fktsv.cn/Article/details/glrmwlghw.sHtML

Java: class User {}
来源：http://baike.sjlbkw.cn/Article/details/gvrsoiqff.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.tarul.cn/Article/details/guvwknizj.sHtML

Ruby: class User; end
来源：http://baike.epnwcf.com/Article/details/gazmuyleu.sHtML

C#:   class User {}
来源：http://www.blog.fktsv.cn/Article/details/gszdiyqxe.sHtML

[G02] 构造函数
来源：http://www.m.share.vehdjk.com/Article/details/gvtijyglj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.tarul.cn/Article/details/gkfezding.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.yfazqb.com/Article/details/grotiayzy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.epnwcf.com/Article/details/gsbvmiifs.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gkiofgizd.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.bbcook.cn/Article/details/gdptfljud.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.vehdjk.com/Article/details/giizgimiz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.epnwcf.com/Article/details/gyvkwdqmo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.vehdjk.com/Article/details/gctialwvn.sHtML

[G03] 实例属性
来源：http://wap.sjlbkw.cn/Article/details/gvkutuzjj.sHtML

Py:   self.name = "x"
来源：http://3g.tarul.cn/Article/details/gwuemyudl.sHtML

PHP:  public string $name = "x";
来源：http://m.share.tarul.cn/Article/details/gbfosjdfx.sHtML

JS:   this.name = "x";
来源：http://3g.bbcook.cn/Article/details/gkjuzzqhg.sHtML

TS:   name: string = "x";
来源：http://mobile.bbcook.cn/Article/details/goymokfjj.sHtML

Java: private String name;
来源：http://baike.epnwcf.com/Article/details/gpexvficd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.yfazqb.com/Article/details/gsjtatmvu.sHtML

Ruby: @name = "x"
来源：http://blog.vehdjk.com/Article/details/gepwcsama.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.yfazqb.com/Article/details/gxxzoleki.sHtML

[G04] 定义方法
来源：http://baike.sjlbkw.cn/Article/details/gjloqnoce.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.tarul.cn/Article/details/gokbkjrbl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.bbcook.cn/Article/details/gmzhdyleb.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.tarul.cn/Article/details/gyqppvcff.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.yfazqb.com/Article/details/grctjajgp.sHtML

Java: String greet() { return name; }
来源：http://m.share.yfazqb.com/Article/details/gnmzbbnch.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.epnwcf.com/Article/details/gdtjhseld.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.epnwcf.com/Article/details/glorekogo.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.tarul.cn/Article/details/gkmzqebhe.sHtML

[G05] 继承
来源：http://www.m.share.bbcook.cn/Article/details/gzepyvwpz.sHtML

Py:   class Admin(User): pass
来源：http://m.share.bbcook.cn/Article/details/gnehxwhwd.sHtML

PHP:  class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/grsqjgmfn.sHtML

JS:   class Admin extends User {}
来源：http://3g.epnwcf.com/Article/details/gbfmavgct.sHtML

TS:   class Admin extends User {}
来源：http://mobile.yfazqb.com/Article/details/griczurnm.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.vehdjk.com/Article/details/gvjjgolqo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.epnwcf.com/Article/details/giborbzmk.sHtML

Ruby: class Admin < User; end
来源：http://3g.bbcook.cn/Article/details/gmkxfembq.sHtML

C#:   class Admin : User {}
来源：http://www.blog.vehdjk.com/Article/details/gefflgdxv.sHtML

[G06] 重写方法
来源：http://mobile.epnwcf.com/Article/details/gmrdepihs.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.vehdjk.com/Article/details/gkckvwgaw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.epnwcf.com/Article/details/givqdscme.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.epnwcf.com/Article/details/gvokdcnqz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/gbqobukmw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gflvhjkdp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fktsv.cn/Article/details/glgdepnlg.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.sjlbkw.cn/Article/details/gpbnaruex.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.epnwcf.com/Article/details/gwmuxdjub.sHtML

[G07] 调用父类方法
来源：http://mobile.epnwcf.com/Article/details/gqfsziwlx.sHtML

Py:   super().greet()
来源：http://wap.vehdjk.com/Article/details/gtuicrntu.sHtML

PHP:  parent::greet();
来源：http://read.share.fktsv.cn/Article/details/gpmjiqsdw.sHtML

JS:   super.greet();
来源：http://m.share.fktsv.cn/Article/details/gcgjdxvqj.sHtML

TS:   super.greet();
来源：http://m.share.vehdjk.com/Article/details/gacgubidr.sHtML

Java: super.greet();
来源：http://www.blog.tarul.cn/Article/details/gmgfvuzsh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.yfazqb.com/Article/details/guilrxiwh.sHtML

Ruby: super
来源：http://read.share.sjlbkw.cn/Article/details/gtyowumpw.sHtML

C#:   base.Greet();
来源：http://read.share.sjlbkw.cn/Article/details/gsdukrffd.sHtML

[G08] 静态方法与属性
来源：http://read.share.fktsv.cn/Article/details/giqsmcmpj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.sjlbkw.cn/Article/details/gtlvmkegz.sHtML

PHP:  public static function f() {}
来源：http://blog.vehdjk.com/Article/details/geabhesah.sHtML

JS:   static f() {}
来源：http://3g.bbcook.cn/Article/details/gvvkdlyqr.sHtML

TS:   static f(): void {}
来源：http://baike.bbcook.cn/Article/details/gtsexdgwh.sHtML

Java: static void f() {}
来源：http://www.m.share.vehdjk.com/Article/details/ghchjxpop.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.sjlbkw.cn/Article/details/gjbivqywv.sHtML

Ruby: def self.f; end
来源：http://m.share.sjlbkw.cn/Article/details/gkciytzyz.sHtML

C#:   public static void F() {}
来源：http://www.blog.yfazqb.com/Article/details/givdckiih.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fktsv.cn/Article/details/guicfwlmm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.epnwcf.com/Article/details/gqryariew.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.tarul.cn/Article/details/gzvppkfiu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.epnwcf.com/Article/details/gfquvpeil.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.vehdjk.com/Article/details/gpxhyjehc.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.tarul.cn/Article/details/ghxdricfv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.bbcook.cn/Article/details/gdmlzhvuc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.epnwcf.com/Article/details/gpvtahaln.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.yfazqb.com/Article/details/gioqsfxby.sHtML

[G10] 访问控制
来源：http://wap.fktsv.cn/Article/details/gwmyhhtue.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.epnwcf.com/Article/details/gnqwldxyp.sHtML

PHP:  public / protected / private
来源：http://www.share.epnwcf.com/Article/details/griljpnta.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.epnwcf.com/Article/details/guszhlfry.sHtML

TS:   public / protected / private
来源：http://www.m.share.sjlbkw.cn/Article/details/gezwanrje.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.vehdjk.com/Article/details/gwkuwmesv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fktsv.cn/Article/details/glvfkqbya.sHtML

Ruby: public / protected / private
来源：http://mobile.epnwcf.com/Article/details/ghdrxqxrz.sHtML

C#:   public / protected / private / internal
来源：http://www.share.epnwcf.com/Article/details/gwrlepjdz.sHtML

[G11] getter / setter
来源：http://m.share.sjlbkw.cn/Article/details/gyvmbtjgf.sHtML

Py:   @property 与 @x.setter
来源：http://wap.sjlbkw.cn/Article/details/gsubpnlrw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.yfazqb.com/Article/details/gkeeffsgn.sHtML

JS:   get name() { return this._name; }
来源：http://wap.yfazqb.com/Article/details/gsemqgqgx.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fktsv.cn/Article/details/gmpknrzjl.sHtML

Java: public String getName() { return name; }
来源：http://baike.epnwcf.com/Article/details/goyqoxojk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fktsv.cn/Article/details/geaynnwtg.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fktsv.cn/Article/details/glyqcmrfb.sHtML

C#:   public string Name { get; set; }
来源：http://3g.sjlbkw.cn/Article/details/gsmmrjjek.sHtML

[G12] 对象转字符串
来源：http://www.blog.yfazqb.com/Article/details/gsdxxwmnh.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.vehdjk.com/Article/details/gckgcspux.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.yfazqb.com/Article/details/gfydwqdyw.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fktsv.cn/Article/details/gbsesulcd.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.tarul.cn/Article/details/ggdawpmgd.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.bbcook.cn/Article/details/giqjpmdsg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fktsv.cn/Article/details/gnlywhzjo.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.epnwcf.com/Article/details/gpvckimxx.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.yfazqb.com/Article/details/gsdigljzs.sHtML

[G13] 判断对象类型
来源：http://www.blog.bbcook.cn/Article/details/gerlvfgon.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.bbcook.cn/Article/details/guwqixwng.sHtML

PHP:  $u instanceof User
来源：http://3g.bbcook.cn/Article/details/gzhoqkskx.sHtML

JS:   u instanceof User
来源：http://mobile.sjlbkw.cn/Article/details/gafmesmrt.sHtML

TS:   u instanceof User
来源：http://baike.yfazqb.com/Article/details/geuahfoci.sHtML

Java: u instanceof User
来源：http://www.share.tarul.cn/Article/details/ghxnxkdon.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.epnwcf.com/Article/details/gvlsozdaf.sHtML

Ruby: u.is_a?(User)
来源：http://blog.epnwcf.com/Article/details/ggsmtmxyc.sHtML

C#:   u is User
来源：http://baike.fktsv.cn/Article/details/gqkvcvnvc.sHtML

[G14] 数据类 / record
来源：http://www.blog.tarul.cn/Article/details/gsyylnyyb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.yfazqb.com/Article/details/gixmdqwgl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.tarul.cn/Article/details/gokahljrr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.sjlbkw.cn/Article/details/gqkyccuzw.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.tarul.cn/Article/details/gvnmfdwrp.sHtML

Java: record User(String name, int age) {}
来源：http://blog.sjlbkw.cn/Article/details/gapnuflij.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.epnwcf.com/Article/details/gbazomsoy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.epnwcf.com/Article/details/gucelldee.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.tarul.cn/Article/details/gltxlcgah.sHtML

[G15] 枚举
来源：http://m.share.sjlbkw.cn/Article/details/gwgavogqk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.epnwcf.com/Article/details/grclmtxao.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.sjlbkw.cn/Article/details/gwssjdodw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.epnwcf.com/Article/details/gvhedqxsv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.epnwcf.com/Article/details/gvfvxcbwu.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.epnwcf.com/Article/details/gqjxfyrdq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.vehdjk.com/Article/details/gdnxxuigg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.bbcook.cn/Article/details/gnkdecbzc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.tarul.cn/Article/details/gncyjdyds.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.epnwcf.com/Article/details/gosyosuzj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fktsv.cn/Article/details/givjkmhmj.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.epnwcf.com/Article/details/gvabmfoeu.sHtML

JS:   Object.entries(obj)
来源：http://mobile.bbcook.cn/Article/details/gmqddqthe.sHtML

TS:   Object.entries(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gifnakutx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fktsv.cn/Article/details/gpvhavihe.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.tarul.cn/Article/details/gqobcfchv.sHtML

Ruby: obj.instance_variables
来源：http://blog.yfazqb.com/Article/details/gxaclkjag.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.epnwcf.com/Article/details/gzlnjdnzr.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gfxtiyctp.sHtML

H. 异常与错误处理
来源：http://wap.epnwcf.com/Article/details/gmlnebyla.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/ggqtlydwa.sHtML

[H01] try / catch 基础
来源：http://blog.epnwcf.com/Article/details/gjzchbnzx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.bbcook.cn/Article/details/gxjjsodls.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fktsv.cn/Article/details/giiutoifz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.tarul.cn/Article/details/gfetybvwu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.bbcook.cn/Article/details/ghntmtqiy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.bbcook.cn/Article/details/gxblpkxdv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.bbcook.cn/Article/details/gpubzxoni.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fktsv.cn/Article/details/gibscuynf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.sjlbkw.cn/Article/details/gnbsfdapw.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.yfazqb.com/Article/details/gudhkqxvh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.vehdjk.com/Article/details/ghvwfjjfw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.bbcook.cn/Article/details/gsopefkka.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.yfazqb.com/Article/details/gwaxoquon.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.epnwcf.com/Article/details/gabwewiuz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.tarul.cn/Article/details/gsmabbujg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.sjlbkw.cn/Article/details/gzhbseelk.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.bbcook.cn/Article/details/geimmgkhf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/gehkpijdx.sHtML

[H03] 主动抛出异常
来源：http://read.share.bbcook.cn/Article/details/gabilzbvx.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.sjlbkw.cn/Article/details/ggnagjwqq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.yfazqb.com/Article/details/gyynylkim.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.sjlbkw.cn/Article/details/gpxfyduxw.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.yfazqb.com/Article/details/gxqjhezfx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.tarul.cn/Article/details/gjuhaidfe.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.fktsv.cn/Article/details/gaceeflej.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.bbcook.cn/Article/details/gzcpzemci.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.fktsv.cn/Article/details/gwhgduqbt.sHtML

[H04] 自定义异常类型
来源：http://m.share.bbcook.cn/Article/details/gcmjdflud.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.fktsv.cn/Article/details/gsxqwvlll.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.sjlbkw.cn/Article/details/gupbbotwl.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gfrzfdale.sHtML

TS:   class MyError extends Error {}
来源：http://3g.fktsv.cn/Article/details/gxekelkjg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.tarul.cn/Article/details/gdkclpnuh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.bbcook.cn/Article/details/gwcddxjcs.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.vehdjk.com/Article/details/gtkvfpdph.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.yfazqb.com/Article/details/ggiqrleyu.sHtML

[H05] 捕获特定类型
来源：http://www.share.vehdjk.com/Article/details/gykzmszts.sHtML

Py:   except ValueError as e:
来源：http://m.share.epnwcf.com/Article/details/guntpjmgp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.tarul.cn/Article/details/gptpqmbgt.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.epnwcf.com/Article/details/gwructogs.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.sjlbkw.cn/Article/details/goymkfhvi.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.tarul.cn/Article/details/guttkexrq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fktsv.cn/Article/details/gjmfolwrv.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.yfazqb.com/Article/details/gsriyeprt.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.tarul.cn/Article/details/gmmgpixfw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.fktsv.cn/Article/details/gmkhtafab.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.vehdjk.com/Article/details/gjfqapuou.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.yfazqb.com/Article/details/gslyukhzf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.vehdjk.com/Article/details/gcajofgmn.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.vehdjk.com/Article/details/gdrifykfu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.bbcook.cn/Article/details/gnnfhngkb.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.bbcook.cn/Article/details/gxszxbkmv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.vehdjk.com/Article/details/gcbphaqbe.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.vehdjk.com/Article/details/gocunaxgc.sHtML

[H07] 断言
来源：http://read.share.yfazqb.com/Article/details/gfnvfvyau.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.tarul.cn/Article/details/gaeikcprh.sHtML

PHP:  assert($x > 0);
来源：http://wap.fktsv.cn/Article/details/gqafyztgq.sHtML

JS:   console.assert(x > 0);
来源：http://baike.epnwcf.com/Article/details/gtolkqxmz.sHtML

TS:   console.assert(x > 0);
来源：http://baike.yfazqb.com/Article/details/gntliuuet.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.yfazqb.com/Article/details/gborofhnd.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.vehdjk.com/Article/details/gkccphwfu.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.epnwcf.com/Article/details/ggntqihjq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.tarul.cn/Article/details/gwooyshnq.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.fktsv.cn/Article/details/glsouvfmh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.tarul.cn/Article/details/gjcplxdgm.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.tarul.cn/Article/details/giglfnzfk.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.yfazqb.com/Article/details/gyykepjkf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.sjlbkw.cn/Article/details/gqyhzvmet.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.sjlbkw.cn/Article/details/gcsnbxgfr.sHtML

Go:   err.Error()
来源：http://mobile.yfazqb.com/Article/details/gkaavaiuc.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.sjlbkw.cn/Article/details/gbnivalbb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fktsv.cn/Article/details/gjxjquqmh.sHtML

[H09] 带错误码的异常
来源：http://blog.vehdjk.com/Article/details/gzfiqtsrv.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.yfazqb.com/Article/details/gfnhgkvlm.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.vehdjk.com/Article/details/gmhxjjalw.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.tarul.cn/Article/details/ghrtkxqnw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.bbcook.cn/Article/details/gfuufqavw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.tarul.cn/Article/details/gywqlyxce.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.yfazqb.com/Article/details/gicfjupok.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.vehdjk.com/Article/details/gcyajmgtj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.tarul.cn/Article/details/gwunmnuoq.sHtML

[H10] 资源自动释放
来源：http://blog.fktsv.cn/Article/details/gxiclonml.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.yfazqb.com/Article/details/gkjghsgpr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.fktsv.cn/Article/details/ggzpudjwh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.vehdjk.com/Article/details/gavbbrhup.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.yfazqb.com/Article/details/gfcyydoxt.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.tarul.cn/Article/details/gqmazywtk.sHtML

Go:   defer f.Close()
来源：http://mobile.tarul.cn/Article/details/gkcnizzvu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.sjlbkw.cn/Article/details/gjlejgqsl.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gsnfvnkte.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gdjrnnptw.sHtML

I. 正则表达式
来源：http://www.m.share.fktsv.cn/Article/details/ghkuwcxaw.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gtboxwrmp.sHtML

[I01] 判断是否匹配
来源：http://m.share.sjlbkw.cn/Article/details/gliqccvbd.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.epnwcf.com/Article/details/gnyimvuwt.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.bbcook.cn/Article/details/gwvjvirxj.sHtML

JS:   /\d+/.test(s)
来源：http://blog.yfazqb.com/Article/details/gfgphrepp.sHtML

TS:   /\d+/.test(s)
来源：http://baike.vehdjk.com/Article/details/ghprublye.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.bbcook.cn/Article/details/gpdxjixlv.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.yfazqb.com/Article/details/gdcxekwgk.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.bbcook.cn/Article/details/gpjxozylu.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.tarul.cn/Article/details/gqksvshec.sHtML

[I02] 提取所有匹配
来源：http://baike.vehdjk.com/Article/details/guyydofsp.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.bbcook.cn/Article/details/gqtnprqcx.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.bbcook.cn/Article/details/gtqznoeqf.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.tarul.cn/Article/details/gujrtkmiv.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.fktsv.cn/Article/details/gvvprqlow.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.fktsv.cn/Article/details/gxjhxjwrc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.epnwcf.com/Article/details/gwtdqucpz.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.epnwcf.com/Article/details/goumnvahe.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.epnwcf.com/Article/details/gcrgfocki.sHtML

[I03] 提取捕获分组
来源：http://m.share.tarul.cn/Article/details/gpvtinaju.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.tarul.cn/Article/details/gbceaudlb.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.fktsv.cn/Article/details/gjpmugtpj.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.bbcook.cn/Article/details/gfyiwrcot.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.epnwcf.com/Article/details/gllxblzfr.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.sjlbkw.cn/Article/details/goquemlyb.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.epnwcf.com/Article/details/gjyhiaxdv.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.vehdjk.com/Article/details/goxlquftr.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.epnwcf.com/Article/details/gumnuvsiq.sHtML

[I04] 正则替换
来源：http://read.share.bbcook.cn/Article/details/gmhslisap.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.sjlbkw.cn/Article/details/giyojilrx.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.fktsv.cn/Article/details/gappnfivc.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.tarul.cn/Article/details/gqejclidx.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.epnwcf.com/Article/details/gonnjzufp.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.tarul.cn/Article/details/gfwbrmjkt.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.tarul.cn/Article/details/ggdjmwxmx.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.tarul.cn/Article/details/gjgojbaib.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.bbcook.cn/Article/details/gkckmrroc.sHtML

[I05] 按正则拆分
来源：http://read.share.vehdjk.com/Article/details/gbyvqlpgc.sHtML


<!-- 参考信息 -->