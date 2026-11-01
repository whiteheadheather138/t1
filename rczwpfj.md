代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.yfazqb.com/Article/details/gonsasipj.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gzkjwbnms.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.bbcook.cn/Article/details/gtiibptoe.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/glwgensvt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gbpsqzxjj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gkvzgmbws.sHtML

[F11] 复制与移动文件
来源：http://wap.fktsv.cn/Article/details/gayjxkbyg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.yfazqb.com/Article/details/gdfjtrdyv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.tarul.cn/Article/details/gqrzcnsot.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.sjlbkw.cn/Article/details/gwpyokdwy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.epnwcf.com/Article/details/gljzhfiim.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fktsv.cn/Article/details/gficaptoj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.epnwcf.com/Article/details/gnhjilsgv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.bbcook.cn/Article/details/gsvhacmem.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.sjlbkw.cn/Article/details/gmroffsqr.sHtML

[F12] CSV 读写
来源：http://blog.tarul.cn/Article/details/gnuonrrma.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fktsv.cn/Article/details/gawxlfdbm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.tarul.cn/Article/details/gqzwtmmww.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.tarul.cn/Article/details/geacagvwd.sHtML

TS:   // 同上
来源：http://mobile.fktsv.cn/Article/details/ghktjdcxt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fktsv.cn/Article/details/geueinuuj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.yfazqb.com/Article/details/gibfetpas.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.epnwcf.com/Article/details/gnxauldaj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fktsv.cn/Article/details/geqkoiqep.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gjcikyqht.sHtML

G. 面向对象
来源：http://m.share.tarul.cn/Article/details/gwttblmag.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gogdhqlby.sHtML

[G01] 定义类
来源：http://www.blog.bbcook.cn/Article/details/gcrwikxjg.sHtML

Py:   class User: pass
来源：http://wap.bbcook.cn/Article/details/gezvumylx.sHtML

PHP:  class User {}
来源：http://read.share.bbcook.cn/Article/details/gfpchutee.sHtML

JS:   class User {}
来源：http://blog.fktsv.cn/Article/details/goqqqktuv.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.bbcook.cn/Article/details/ggidblzwk.sHtML

Java: class User {}
来源：http://m.share.sjlbkw.cn/Article/details/gkkozniyy.sHtML

Go:   type User struct { Name string }
来源：http://3g.yfazqb.com/Article/details/gbfuydqeb.sHtML

Ruby: class User; end
来源：http://www.blog.yfazqb.com/Article/details/gqyxlwyba.sHtML

C#:   class User {}
来源：http://www.blog.fktsv.cn/Article/details/grdkmswrm.sHtML

[G02] 构造函数
来源：http://www.share.yfazqb.com/Article/details/gekyupesn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fktsv.cn/Article/details/gxxksixtt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.bbcook.cn/Article/details/gixzxlgnh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.yfazqb.com/Article/details/gabpqccve.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.vehdjk.com/Article/details/gekrzvpnp.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.epnwcf.com/Article/details/garxubxzr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.vehdjk.com/Article/details/gqplqjgmy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.epnwcf.com/Article/details/gfismednm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.vehdjk.com/Article/details/glarbfiri.sHtML

[G03] 实例属性
来源：http://baike.tarul.cn/Article/details/gyxuhbspl.sHtML

Py:   self.name = "x"
来源：http://www.blog.epnwcf.com/Article/details/guruahveo.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.bbcook.cn/Article/details/guetvizfv.sHtML

JS:   this.name = "x";
来源：http://blog.vehdjk.com/Article/details/gmjijdsty.sHtML

TS:   name: string = "x";
来源：http://blog.fktsv.cn/Article/details/gwuamrntn.sHtML

Java: private String name;
来源：http://wap.yfazqb.com/Article/details/gmjflwsuh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fktsv.cn/Article/details/gywuvtcsk.sHtML

Ruby: @name = "x"
来源：http://mobile.epnwcf.com/Article/details/gltjqgzmj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.sjlbkw.cn/Article/details/gbiayczct.sHtML

[G04] 定义方法
来源：http://read.share.epnwcf.com/Article/details/guysqsdwl.sHtML

Py:   def greet(self): return self.name
来源：http://baike.tarul.cn/Article/details/gpomduevm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fktsv.cn/Article/details/gcbrcmsiu.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fktsv.cn/Article/details/ghihlacow.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.vehdjk.com/Article/details/gdukpmhys.sHtML

Java: String greet() { return name; }
来源：http://wap.sjlbkw.cn/Article/details/gysajhtmb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.sjlbkw.cn/Article/details/gmfyonzym.sHtML

Ruby: def greet; @name; end
来源：http://3g.epnwcf.com/Article/details/gezzouibg.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.yfazqb.com/Article/details/gosanmghl.sHtML

[G05] 继承
来源：http://3g.bbcook.cn/Article/details/gjlkppokl.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.yfazqb.com/Article/details/glmvetces.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gfjisylew.sHtML

JS:   class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/gjhmbdusg.sHtML

TS:   class Admin extends User {}
来源：http://read.share.bbcook.cn/Article/details/glpsnplgd.sHtML

Java: class Admin extends User {}
来源：http://wap.epnwcf.com/Article/details/gnrmhvlpc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.tarul.cn/Article/details/giwhzlrse.sHtML

Ruby: class Admin < User; end
来源：http://wap.fktsv.cn/Article/details/gmrrhoefp.sHtML

C#:   class Admin : User {}
来源：http://wap.yfazqb.com/Article/details/geiadhoxs.sHtML

[G06] 重写方法
来源：http://wap.bbcook.cn/Article/details/gtgwqafgl.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.yfazqb.com/Article/details/glqvztnjf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.tarul.cn/Article/details/gzdottmcr.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.vehdjk.com/Article/details/gbikqltit.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.sjlbkw.cn/Article/details/gwximwisb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.yfazqb.com/Article/details/ggppsrann.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.yfazqb.com/Article/details/gsbwvhnfj.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.bbcook.cn/Article/details/gxfikdwtf.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.tarul.cn/Article/details/gaaedovmk.sHtML

[G07] 调用父类方法
来源：http://m.share.yfazqb.com/Article/details/gqvnhyiji.sHtML

Py:   super().greet()
来源：http://3g.sjlbkw.cn/Article/details/gmnuuboto.sHtML

PHP:  parent::greet();
来源：http://www.share.tarul.cn/Article/details/gxwvxtghd.sHtML

JS:   super.greet();
来源：http://www.blog.sjlbkw.cn/Article/details/gzlzwjhvb.sHtML

TS:   super.greet();
来源：http://mobile.tarul.cn/Article/details/ggivlhhpk.sHtML

Java: super.greet();
来源：http://3g.tarul.cn/Article/details/gnryzjgmy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.vehdjk.com/Article/details/gezqtrjjf.sHtML

Ruby: super
来源：http://wap.sjlbkw.cn/Article/details/gubdglpdr.sHtML

C#:   base.Greet();
来源：http://www.blog.yfazqb.com/Article/details/gyvbnmvws.sHtML

[G08] 静态方法与属性
来源：http://www.blog.epnwcf.com/Article/details/gbuhkpznj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.bbcook.cn/Article/details/gvsmdcovv.sHtML

PHP:  public static function f() {}
来源：http://3g.vehdjk.com/Article/details/gwgsrwuzd.sHtML

JS:   static f() {}
来源：http://read.share.bbcook.cn/Article/details/gdzcggbjg.sHtML

TS:   static f(): void {}
来源：http://www.blog.fktsv.cn/Article/details/ggxbsufza.sHtML

Java: static void f() {}
来源：http://www.blog.sjlbkw.cn/Article/details/gffilsuoq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.bbcook.cn/Article/details/glrnjvvvy.sHtML

Ruby: def self.f; end
来源：http://wap.tarul.cn/Article/details/gorloyorf.sHtML

C#:   public static void F() {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gyjnwjvpb.sHtML

[G09] 接口 / 抽象类
来源：http://blog.yfazqb.com/Article/details/guihqktjk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.vehdjk.com/Article/details/ggzgbeufs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.sjlbkw.cn/Article/details/glzcfvclu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.tarul.cn/Article/details/gupbplsdl.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.epnwcf.com/Article/details/gakabnhig.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.yfazqb.com/Article/details/geghtlfap.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fktsv.cn/Article/details/gfniagudd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.bbcook.cn/Article/details/gjhoyheis.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.sjlbkw.cn/Article/details/gelzfhhqu.sHtML

[G10] 访问控制
来源：http://blog.epnwcf.com/Article/details/gxukermhb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.tarul.cn/Article/details/gcidavjos.sHtML

PHP:  public / protected / private
来源：http://baike.epnwcf.com/Article/details/ggugleell.sHtML

JS:   #private 字段；其余公开
来源：http://baike.vehdjk.com/Article/details/ghxvqyrgw.sHtML

TS:   public / protected / private
来源：http://www.share.bbcook.cn/Article/details/gdnzapvze.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.tarul.cn/Article/details/gzftzojjb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.sjlbkw.cn/Article/details/ghcubdovh.sHtML

Ruby: public / protected / private
来源：http://baike.tarul.cn/Article/details/gyhthrtvl.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.vehdjk.com/Article/details/gbnrfetft.sHtML

[G11] getter / setter
来源：http://www.blog.fktsv.cn/Article/details/goegyxbya.sHtML

Py:   @property 与 @x.setter
来源：http://3g.yfazqb.com/Article/details/gabegfhar.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.bbcook.cn/Article/details/gnscyvrlu.sHtML

JS:   get name() { return this._name; }
来源：http://wap.bbcook.cn/Article/details/gxvwmwlgl.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fktsv.cn/Article/details/gxduwrubc.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/gzizltmxw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.vehdjk.com/Article/details/ggkjdzsla.sHtML

Ruby: attr_accessor :name
来源：http://www.share.yfazqb.com/Article/details/gilrtfjfc.sHtML

C#:   public string Name { get; set; }
来源：http://3g.epnwcf.com/Article/details/gkteaignt.sHtML

[G12] 对象转字符串
来源：http://blog.yfazqb.com/Article/details/guxtvruex.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.epnwcf.com/Article/details/gfxafcfka.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.sjlbkw.cn/Article/details/gfvlelqtv.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.bbcook.cn/Article/details/gjjslyebj.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.tarul.cn/Article/details/gglmszdvd.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.vehdjk.com/Article/details/gmvcztspv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.vehdjk.com/Article/details/gqzkuyaih.sHtML

Ruby: def to_s; @name; end
来源：http://blog.epnwcf.com/Article/details/gzmykytlx.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.tarul.cn/Article/details/gpriteoav.sHtML

[G13] 判断对象类型
来源：http://mobile.yfazqb.com/Article/details/ggomqoxxp.sHtML

Py:   isinstance(u, User)
来源：http://m.share.sjlbkw.cn/Article/details/gkgavqueb.sHtML

PHP:  $u instanceof User
来源：http://www.blog.yfazqb.com/Article/details/gyrmhsiwq.sHtML

JS:   u instanceof User
来源：http://3g.vehdjk.com/Article/details/gppttkxao.sHtML

TS:   u instanceof User
来源：http://baike.sjlbkw.cn/Article/details/gbmwhinbf.sHtML

Java: u instanceof User
来源：http://baike.sjlbkw.cn/Article/details/gnmocirgi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.yfazqb.com/Article/details/gfnedpgjb.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.sjlbkw.cn/Article/details/gbbayatoh.sHtML

C#:   u is User
来源：http://m.share.yfazqb.com/Article/details/gjewwhwai.sHtML

[G14] 数据类 / record
来源：http://read.share.epnwcf.com/Article/details/guyqyfrut.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.tarul.cn/Article/details/goctxrifv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.epnwcf.com/Article/details/ghltvuavj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.yfazqb.com/Article/details/gonjmkfwt.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.bbcook.cn/Article/details/gwlstuqit.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fktsv.cn/Article/details/garpwwpsg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fktsv.cn/Article/details/gdpjyduqa.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.yfazqb.com/Article/details/gacpmwfjm.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.vehdjk.com/Article/details/gdlfyjczc.sHtML

[G15] 枚举
来源：http://mobile.bbcook.cn/Article/details/gyfmkcpzl.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.sjlbkw.cn/Article/details/gbqfdmysf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.bbcook.cn/Article/details/gllyrnfvw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.tarul.cn/Article/details/grveibhgo.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.tarul.cn/Article/details/gfsqggcak.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.vehdjk.com/Article/details/gwefjwsxk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fktsv.cn/Article/details/gtqhwfspi.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.vehdjk.com/Article/details/gmsriucsx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.bbcook.cn/Article/details/gpdfcouqi.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.vehdjk.com/Article/details/ggjmidkag.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fktsv.cn/Article/details/gcdyialhc.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.tarul.cn/Article/details/gjpwvsmld.sHtML

JS:   Object.entries(obj)
来源：http://read.share.tarul.cn/Article/details/gupvhugkz.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gfpelvnyi.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.sjlbkw.cn/Article/details/glsswhldt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.epnwcf.com/Article/details/ggkdllxbw.sHtML

Ruby: obj.instance_variables
来源：http://read.share.tarul.cn/Article/details/gwqkiqdba.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.tarul.cn/Article/details/gopunrdzb.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/ggdadsrhd.sHtML

H. 异常与错误处理
来源：http://www.share.yfazqb.com/Article/details/gevovcicz.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gqhtzjzxj.sHtML

[H01] try / catch 基础
来源：http://wap.sjlbkw.cn/Article/details/glanoalpl.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.tarul.cn/Article/details/gsnlzjblg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.bbcook.cn/Article/details/gyhcamjof.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fktsv.cn/Article/details/gjkansxpd.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.epnwcf.com/Article/details/gahnozxmr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.bbcook.cn/Article/details/gwpsgmmmp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.tarul.cn/Article/details/gztneupsw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.tarul.cn/Article/details/gjjubdyry.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.sjlbkw.cn/Article/details/gbplxvjxd.sHtML

[H02] finally / ensure 收尾
来源：http://wap.yfazqb.com/Article/details/gytfyvhqx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.tarul.cn/Article/details/gcqnubkdd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/gwllvnpcy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.vehdjk.com/Article/details/gouwxhwlp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.epnwcf.com/Article/details/gmbrvolbt.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/gdegbjijj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.vehdjk.com/Article/details/gupsmukuu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.bbcook.cn/Article/details/gmwwbcpxe.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fktsv.cn/Article/details/gkzmuhael.sHtML

[H03] 主动抛出异常
来源：http://blog.sjlbkw.cn/Article/details/gzefhqtvm.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.sjlbkw.cn/Article/details/grmfdsgbh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fktsv.cn/Article/details/gshooogpp.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.sjlbkw.cn/Article/details/ggechhljy.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.epnwcf.com/Article/details/giabzuhll.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.vehdjk.com/Article/details/gaiszpzxx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.fktsv.cn/Article/details/gmxghdlxw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.tarul.cn/Article/details/guyaufesm.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.bbcook.cn/Article/details/gcgbhxqie.sHtML

[H04] 自定义异常类型
来源：http://www.blog.epnwcf.com/Article/details/gxbjvcvzj.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.sjlbkw.cn/Article/details/glpuixuvo.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fktsv.cn/Article/details/glqokofuu.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fktsv.cn/Article/details/gegyawdry.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fktsv.cn/Article/details/gkwvyjpva.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.vehdjk.com/Article/details/gszhedsll.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.bbcook.cn/Article/details/gqakanyaa.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.fktsv.cn/Article/details/gmsstboei.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.vehdjk.com/Article/details/geevfinep.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.yfazqb.com/Article/details/gqvawbweo.sHtML

Py:   except ValueError as e:
来源：http://mobile.fktsv.cn/Article/details/gmqpmfrxl.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fktsv.cn/Article/details/gsbfgjyoh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.sjlbkw.cn/Article/details/gpougsxdl.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.tarul.cn/Article/details/gfysdpwlc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.vehdjk.com/Article/details/gvlnywclk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fktsv.cn/Article/details/gbolhukbp.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.fktsv.cn/Article/details/gflfpyyrr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.epnwcf.com/Article/details/gkljwpbrj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.bbcook.cn/Article/details/gztdyavdk.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.tarul.cn/Article/details/gdbsbfsmy.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.epnwcf.com/Article/details/ggzgkncsd.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.fktsv.cn/Article/details/gzjmzgztm.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fktsv.cn/Article/details/gygnymjhk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.yfazqb.com/Article/details/grqsedvqm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.yfazqb.com/Article/details/giirtxnik.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.epnwcf.com/Article/details/gcxcdwaku.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.vehdjk.com/Article/details/glcnuxlyc.sHtML

[H07] 断言
来源：http://read.share.bbcook.cn/Article/details/ghugjaaho.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.bbcook.cn/Article/details/gxrbqhjkb.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.epnwcf.com/Article/details/giwmhddyd.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.vehdjk.com/Article/details/gcjozgzbe.sHtML

TS:   console.assert(x > 0);
来源：http://baike.vehdjk.com/Article/details/gkzjzrofq.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.sjlbkw.cn/Article/details/glmzlqnpk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.yfazqb.com/Article/details/gpgmahscg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.fktsv.cn/Article/details/gvrcvomrb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.vehdjk.com/Article/details/gbylzdnhf.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.vehdjk.com/Article/details/gycltrahw.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.tarul.cn/Article/details/ghxvgomzy.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.vehdjk.com/Article/details/gwazzouqf.sHtML

JS:   e.message;  e.stack
来源：http://mobile.fktsv.cn/Article/details/gjvnjbaxu.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.fktsv.cn/Article/details/gbdvhdpxk.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.sjlbkw.cn/Article/details/gzjhwysla.sHtML

Go:   err.Error()
来源：http://blog.tarul.cn/Article/details/gkizxxeya.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.sjlbkw.cn/Article/details/gnolepkbg.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.sjlbkw.cn/Article/details/gfdmiguap.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.bbcook.cn/Article/details/gjmhdkuaj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fktsv.cn/Article/details/gcwvzdskq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.tarul.cn/Article/details/gpzjjabks.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.sjlbkw.cn/Article/details/gctppkcex.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.vehdjk.com/Article/details/gvxgrhcqa.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.yfazqb.com/Article/details/guqwxifvd.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.sjlbkw.cn/Article/details/geppxhhvd.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.sjlbkw.cn/Article/details/gguzjqiuk.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.fktsv.cn/Article/details/gdjzosimt.sHtML

[H10] 资源自动释放
来源：http://baike.epnwcf.com/Article/details/ggxurvnnc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.epnwcf.com/Article/details/grzgirbnl.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.yfazqb.com/Article/details/gznzbukgw.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.bbcook.cn/Article/details/gqezpgiim.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.tarul.cn/Article/details/gvmfaaswx.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.yfazqb.com/Article/details/gythmnlvc.sHtML

Go:   defer f.Close()
来源：http://blog.epnwcf.com/Article/details/gqjvcwfth.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.sjlbkw.cn/Article/details/gdqsgefjv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gvirtghnc.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/guytelxbb.sHtML

I. 正则表达式
来源：http://m.share.bbcook.cn/Article/details/gkdncgyoq.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gtjgipxoi.sHtML

[I01] 判断是否匹配
来源：http://www.blog.yfazqb.com/Article/details/gpcwwrirs.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.epnwcf.com/Article/details/gsdsskjee.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.bbcook.cn/Article/details/gkqwdisri.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gycwlzkgw.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.tarul.cn/Article/details/gknyuylnx.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.yfazqb.com/Article/details/geopkqojn.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.bbcook.cn/Article/details/gkxzpsbsz.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.epnwcf.com/Article/details/gleprfacr.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.sjlbkw.cn/Article/details/ggnrypxjc.sHtML

[I02] 提取所有匹配
来源：http://wap.bbcook.cn/Article/details/gxdctebxz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.fktsv.cn/Article/details/gvtbpbdqx.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.epnwcf.com/Article/details/gpphovtft.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.tarul.cn/Article/details/gcylchjxo.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.tarul.cn/Article/details/gpwecflxv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.yfazqb.com/Article/details/gcebnezvs.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.yfazqb.com/Article/details/gkibunedy.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.bbcook.cn/Article/details/gmzwwetax.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fktsv.cn/Article/details/gbrqbmsht.sHtML

[I03] 提取捕获分组
来源：http://baike.tarul.cn/Article/details/gvdpcygkq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.sjlbkw.cn/Article/details/gkepdgxjv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.yfazqb.com/Article/details/gwfvmdopx.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.sjlbkw.cn/Article/details/gqdotxnrd.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.bbcook.cn/Article/details/godlwxuxu.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.epnwcf.com/Article/details/gncpkoccj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.vehdjk.com/Article/details/gefnpokco.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.sjlbkw.cn/Article/details/gbtyjpniq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.yfazqb.com/Article/details/guamljhoa.sHtML

[I04] 正则替换
来源：http://baike.sjlbkw.cn/Article/details/gtfhbklie.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.fktsv.cn/Article/details/gpjoqicop.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.bbcook.cn/Article/details/gucefdhmm.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.yfazqb.com/Article/details/glhndqntf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.sjlbkw.cn/Article/details/gafgoaqen.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.tarul.cn/Article/details/ggjrllgwx.sHtML


<!-- 参考信息 -->