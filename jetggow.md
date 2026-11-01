代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.epnwcf.com/Article/details/ghicwqgwi.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/gycfrbtxf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.epnwcf.com/Article/details/gmwkqeutg.sHtML

[F12] CSV 读写
来源：http://blog.sjlbkw.cn/Article/details/gxjqghbgs.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.yfazqb.com/Article/details/gdfzrlzlz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.sjlbkw.cn/Article/details/glatvxetd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.tarul.cn/Article/details/giaizvpbp.sHtML

TS:   // 同上
来源：http://www.blog.bbcook.cn/Article/details/gmewjirin.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.vehdjk.com/Article/details/gwnyoogdn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.sjlbkw.cn/Article/details/gswqqubje.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.epnwcf.com/Article/details/gdvjjdrab.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.sjlbkw.cn/Article/details/grsyvrspo.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/grrznjxoj.sHtML

G. 面向对象
来源：http://www.share.vehdjk.com/Article/details/gqjvvxbtn.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gemhvbsto.sHtML

[G01] 定义类
来源：http://www.m.share.yfazqb.com/Article/details/gtdhjjtsg.sHtML

Py:   class User: pass
来源：http://wap.sjlbkw.cn/Article/details/gadhoqynm.sHtML

PHP:  class User {}
来源：http://www.blog.yfazqb.com/Article/details/glxvnpzrl.sHtML

JS:   class User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gylfqfnpm.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fktsv.cn/Article/details/gtfxmuron.sHtML

Java: class User {}
来源：http://www.m.share.fktsv.cn/Article/details/gvethxeeb.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.vehdjk.com/Article/details/gisbmkkvj.sHtML

Ruby: class User; end
来源：http://blog.yfazqb.com/Article/details/gbdnplhpu.sHtML

C#:   class User {}
来源：http://read.share.epnwcf.com/Article/details/gfsaopysg.sHtML

[G02] 构造函数
来源：http://wap.fktsv.cn/Article/details/gehwcccnq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.bbcook.cn/Article/details/gypzxbvrb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.tarul.cn/Article/details/gimgwrdst.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.sjlbkw.cn/Article/details/glqjspzxv.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.vehdjk.com/Article/details/gihojtilt.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.tarul.cn/Article/details/gmppqdyzp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.tarul.cn/Article/details/gzdtcqxgl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.bbcook.cn/Article/details/gbhjxqnse.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.bbcook.cn/Article/details/gvxbkyymi.sHtML

[G03] 实例属性
来源：http://www.blog.bbcook.cn/Article/details/gheetaijs.sHtML

Py:   self.name = "x"
来源：http://www.share.bbcook.cn/Article/details/gbygvjabx.sHtML

PHP:  public string $name = "x";
来源：http://blog.yfazqb.com/Article/details/gphkyrjjn.sHtML

JS:   this.name = "x";
来源：http://www.share.bbcook.cn/Article/details/gxbnglvoi.sHtML

TS:   name: string = "x";
来源：http://blog.vehdjk.com/Article/details/ggxdaehgg.sHtML

Java: private String name;
来源：http://baike.tarul.cn/Article/details/gmpzwbllb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.epnwcf.com/Article/details/gmijngvcj.sHtML

Ruby: @name = "x"
来源：http://3g.fktsv.cn/Article/details/goamuiowi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/gqitpjmzf.sHtML

[G04] 定义方法
来源：http://www.m.share.fktsv.cn/Article/details/grgtbveju.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fktsv.cn/Article/details/ghkkevmyi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.sjlbkw.cn/Article/details/gqeykgbqa.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.tarul.cn/Article/details/gbfikuofz.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.sjlbkw.cn/Article/details/ggsglchjy.sHtML

Java: String greet() { return name; }
来源：http://www.blog.yfazqb.com/Article/details/gakjjaust.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.epnwcf.com/Article/details/gydpqcmqv.sHtML

Ruby: def greet; @name; end
来源：http://baike.epnwcf.com/Article/details/gmjrtpgta.sHtML

C#:   public string Greet() => Name;
来源：http://wap.epnwcf.com/Article/details/gcwzrmppj.sHtML

[G05] 继承
来源：http://3g.fktsv.cn/Article/details/gxkhmafmp.sHtML

Py:   class Admin(User): pass
来源：http://baike.bbcook.cn/Article/details/gjfpwhekm.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.yfazqb.com/Article/details/gxavmllxe.sHtML

JS:   class Admin extends User {}
来源：http://baike.fktsv.cn/Article/details/gqanralnl.sHtML

TS:   class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/gynazqdqq.sHtML

Java: class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/gjyjtjrdz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.bbcook.cn/Article/details/gngugchdo.sHtML

Ruby: class Admin < User; end
来源：http://blog.fktsv.cn/Article/details/golvwyrpy.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.vehdjk.com/Article/details/gbbofubbr.sHtML

[G06] 重写方法
来源：http://blog.bbcook.cn/Article/details/gzyqxwbfp.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fktsv.cn/Article/details/gbndheryy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.bbcook.cn/Article/details/gzuyqzoot.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.yfazqb.com/Article/details/gjylszita.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.bbcook.cn/Article/details/gqtvocdod.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.vehdjk.com/Article/details/gxbfikncc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.yfazqb.com/Article/details/gquobutht.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.yfazqb.com/Article/details/gfenhnokm.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.yfazqb.com/Article/details/gkffrqcwo.sHtML

[G07] 调用父类方法
来源：http://www.m.share.epnwcf.com/Article/details/galsldiwy.sHtML

Py:   super().greet()
来源：http://wap.tarul.cn/Article/details/gaweucjgt.sHtML

PHP:  parent::greet();
来源：http://www.m.share.bbcook.cn/Article/details/gosepxkte.sHtML

JS:   super.greet();
来源：http://blog.vehdjk.com/Article/details/grtexwowh.sHtML

TS:   super.greet();
来源：http://m.share.vehdjk.com/Article/details/ghkfvnulb.sHtML

Java: super.greet();
来源：http://www.m.share.fktsv.cn/Article/details/gizylpewl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.vehdjk.com/Article/details/gpjvorspy.sHtML

Ruby: super
来源：http://www.share.tarul.cn/Article/details/gwjmtcaxr.sHtML

C#:   base.Greet();
来源：http://3g.fktsv.cn/Article/details/gcwttjncn.sHtML

[G08] 静态方法与属性
来源：http://blog.fktsv.cn/Article/details/gvmyzztpe.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.sjlbkw.cn/Article/details/guivqgesl.sHtML

PHP:  public static function f() {}
来源：http://read.share.bbcook.cn/Article/details/gbsiixdfk.sHtML

JS:   static f() {}
来源：http://www.blog.epnwcf.com/Article/details/gwbomqcfp.sHtML

TS:   static f(): void {}
来源：http://www.blog.tarul.cn/Article/details/gxratqccl.sHtML

Java: static void f() {}
来源：http://www.share.sjlbkw.cn/Article/details/guwzwwfmm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.vehdjk.com/Article/details/gfobpadbl.sHtML

Ruby: def self.f; end
来源：http://mobile.tarul.cn/Article/details/goypsqeon.sHtML

C#:   public static void F() {}
来源：http://3g.fktsv.cn/Article/details/gaqxghwnr.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.epnwcf.com/Article/details/gxebradse.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.bbcook.cn/Article/details/guhkkjzqc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.vehdjk.com/Article/details/gzpuypkom.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.epnwcf.com/Article/details/gbhddkhbe.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.tarul.cn/Article/details/gdhkfuoli.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.epnwcf.com/Article/details/gimcedkyj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.tarul.cn/Article/details/gamaveqym.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.vehdjk.com/Article/details/gsqzkuucm.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.vehdjk.com/Article/details/gyvnmhmbw.sHtML

[G10] 访问控制
来源：http://3g.fktsv.cn/Article/details/gcjqsddug.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.yfazqb.com/Article/details/gmhmiwxmt.sHtML

PHP:  public / protected / private
来源：http://mobile.vehdjk.com/Article/details/gfbodbjdo.sHtML

JS:   #private 字段；其余公开
来源：http://blog.yfazqb.com/Article/details/gakdmiobz.sHtML

TS:   public / protected / private
来源：http://www.m.share.tarul.cn/Article/details/gtwilnuna.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.vehdjk.com/Article/details/gsktbzqcl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.tarul.cn/Article/details/ggsvouvrc.sHtML

Ruby: public / protected / private
来源：http://blog.fktsv.cn/Article/details/glaskajum.sHtML

C#:   public / protected / private / internal
来源：http://mobile.yfazqb.com/Article/details/ghyxbbkbj.sHtML

[G11] getter / setter
来源：http://baike.epnwcf.com/Article/details/gnffsksno.sHtML

Py:   @property 与 @x.setter
来源：http://3g.yfazqb.com/Article/details/grjykyvnz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.tarul.cn/Article/details/guhegmgjv.sHtML

JS:   get name() { return this._name; }
来源：http://wap.yfazqb.com/Article/details/gcqkdilmt.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.tarul.cn/Article/details/groltablr.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/gbakltspc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.vehdjk.com/Article/details/ghpkfgqvv.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.tarul.cn/Article/details/gwfwsmfub.sHtML

C#:   public string Name { get; set; }
来源：http://3g.epnwcf.com/Article/details/gkkqetjtz.sHtML

[G12] 对象转字符串
来源：http://mobile.tarul.cn/Article/details/gmrcshgds.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.tarul.cn/Article/details/gwyteddem.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fktsv.cn/Article/details/gkvlztfvp.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.yfazqb.com/Article/details/gyujmjamv.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.yfazqb.com/Article/details/gxgxigkph.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/gditbmfpt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.epnwcf.com/Article/details/gqgljvvgz.sHtML

Ruby: def to_s; @name; end
来源：http://wap.vehdjk.com/Article/details/gzftfgumb.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.sjlbkw.cn/Article/details/gyzxbfkue.sHtML

[G13] 判断对象类型
来源：http://www.m.share.yfazqb.com/Article/details/grcdgdtgk.sHtML

Py:   isinstance(u, User)
来源：http://read.share.epnwcf.com/Article/details/gqmnexgqo.sHtML

PHP:  $u instanceof User
来源：http://baike.fktsv.cn/Article/details/gwabdktug.sHtML

JS:   u instanceof User
来源：http://blog.tarul.cn/Article/details/gfpsmdpts.sHtML

TS:   u instanceof User
来源：http://3g.epnwcf.com/Article/details/gqnxupsmv.sHtML

Java: u instanceof User
来源：http://read.share.yfazqb.com/Article/details/gsaemldrx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.epnwcf.com/Article/details/gdprzybbp.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.bbcook.cn/Article/details/gpxtnmxcv.sHtML

C#:   u is User
来源：http://www.share.yfazqb.com/Article/details/glstqyhan.sHtML

[G14] 数据类 / record
来源：http://www.m.share.yfazqb.com/Article/details/gcjjymbiw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.sjlbkw.cn/Article/details/grhxdpgee.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.yfazqb.com/Article/details/gwrkbddkl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.sjlbkw.cn/Article/details/gudpyhkjm.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.yfazqb.com/Article/details/gzcnnhykp.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.epnwcf.com/Article/details/gxcxzlzdr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.epnwcf.com/Article/details/gpqlnqqym.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.yfazqb.com/Article/details/ghwfxymno.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.vehdjk.com/Article/details/gbdrqelxc.sHtML

[G15] 枚举
来源：http://baike.epnwcf.com/Article/details/ghehgvsmn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fktsv.cn/Article/details/gceqsbzmv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.tarul.cn/Article/details/grczinxqa.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.bbcook.cn/Article/details/gjbelqcpu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.vehdjk.com/Article/details/gsmrvliot.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fktsv.cn/Article/details/gengjqnmj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.vehdjk.com/Article/details/gqpgnzpfe.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.tarul.cn/Article/details/gmklyqlzb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.bbcook.cn/Article/details/glvgnyurf.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.bbcook.cn/Article/details/gvczyqzja.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.tarul.cn/Article/details/gtxhdpico.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.tarul.cn/Article/details/gykuuimxw.sHtML

JS:   Object.entries(obj)
来源：http://baike.bbcook.cn/Article/details/gxhgtsatl.sHtML

TS:   Object.entries(obj)
来源：http://baike.epnwcf.com/Article/details/grhbixatx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.yfazqb.com/Article/details/ghzkikmfx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.tarul.cn/Article/details/gzigjwwza.sHtML

Ruby: obj.instance_variables
来源：http://blog.vehdjk.com/Article/details/gzxbccyqy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.epnwcf.com/Article/details/gzcunighs.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/ggleurarm.sHtML

H. 异常与错误处理
来源：http://baike.fktsv.cn/Article/details/gwgvtnmuu.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gjudnmdur.sHtML

[H01] try / catch 基础
来源：http://read.share.vehdjk.com/Article/details/grodgeuxw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.sjlbkw.cn/Article/details/gyjbyfjov.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.tarul.cn/Article/details/gukotjhhv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.vehdjk.com/Article/details/gkdvugnzu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.vehdjk.com/Article/details/gfwbgcjgv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.bbcook.cn/Article/details/gviqmfazl.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.epnwcf.com/Article/details/geayvbwxr.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fktsv.cn/Article/details/gsgctmxfv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.sjlbkw.cn/Article/details/gcpwkwpeg.sHtML

[H02] finally / ensure 收尾
来源：http://3g.bbcook.cn/Article/details/gwtlijryr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.yfazqb.com/Article/details/gvszjptvc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.tarul.cn/Article/details/gfzonoisx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fktsv.cn/Article/details/gptioxvmf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/gvmlgsphm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.vehdjk.com/Article/details/golexglth.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fktsv.cn/Article/details/gwlgjibkx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.vehdjk.com/Article/details/gkdymszak.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/gifctogng.sHtML

[H03] 主动抛出异常
来源：http://read.share.vehdjk.com/Article/details/gkvaudqrd.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.yfazqb.com/Article/details/gtcsngqqw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.sjlbkw.cn/Article/details/gtmsctfay.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.vehdjk.com/Article/details/gomjnvusc.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.bbcook.cn/Article/details/ggumnkycx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.sjlbkw.cn/Article/details/gkbmwarlt.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fktsv.cn/Article/details/guyieqlrd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fktsv.cn/Article/details/gqfjnxrhy.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.tarul.cn/Article/details/gjtwtbwro.sHtML

[H04] 自定义异常类型
来源：http://baike.fktsv.cn/Article/details/gyiokchmh.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.sjlbkw.cn/Article/details/gpfuvizux.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.bbcook.cn/Article/details/gninhztzz.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.vehdjk.com/Article/details/gaszbzxkm.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.epnwcf.com/Article/details/gufszmysp.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.vehdjk.com/Article/details/gehwgwxln.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.bbcook.cn/Article/details/gdsqkrntq.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.fktsv.cn/Article/details/gtbadywcq.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.yfazqb.com/Article/details/gwahiqyxz.sHtML

[H05] 捕获特定类型
来源：http://3g.bbcook.cn/Article/details/gpxnyjhdr.sHtML

Py:   except ValueError as e:
来源：http://baike.tarul.cn/Article/details/gsekddtws.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.yfazqb.com/Article/details/ggsbbqoes.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.epnwcf.com/Article/details/gdkgslsnu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.yfazqb.com/Article/details/ghuuvmlgn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.tarul.cn/Article/details/gizuwkclb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.tarul.cn/Article/details/grlrvfzhe.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fktsv.cn/Article/details/glfkutijl.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.yfazqb.com/Article/details/gcdmpkwvc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.vehdjk.com/Article/details/gqfirspdf.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.tarul.cn/Article/details/gpgvrqgfu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.epnwcf.com/Article/details/ghcbvzaub.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.vehdjk.com/Article/details/gymxkrqbu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.tarul.cn/Article/details/ggimffjie.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.yfazqb.com/Article/details/gvklvotbf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.bbcook.cn/Article/details/gpycymfhe.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.tarul.cn/Article/details/gbwlnyhdp.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.epnwcf.com/Article/details/glgrwbgzv.sHtML

[H07] 断言
来源：http://baike.yfazqb.com/Article/details/giehdndbq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.bbcook.cn/Article/details/gtmbwunda.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fktsv.cn/Article/details/gujuuhsht.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.tarul.cn/Article/details/gcszprnnn.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gywmaxxlw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.sjlbkw.cn/Article/details/gfeztepft.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.epnwcf.com/Article/details/gbiyhimpz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.tarul.cn/Article/details/gxkohumkg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.fktsv.cn/Article/details/guznlsqxb.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.vehdjk.com/Article/details/glrnjfkey.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.yfazqb.com/Article/details/gzikmkuop.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.sjlbkw.cn/Article/details/gwiknozzk.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.tarul.cn/Article/details/gcpszbguw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.tarul.cn/Article/details/gzwvafypn.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.sjlbkw.cn/Article/details/gvgemyvap.sHtML

Go:   err.Error()
来源：http://blog.bbcook.cn/Article/details/ghhnmzlty.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.bbcook.cn/Article/details/gnvezuapr.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.tarul.cn/Article/details/gwyfphqgn.sHtML

[H09] 带错误码的异常
来源：http://blog.bbcook.cn/Article/details/gqxckzwyv.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.bbcook.cn/Article/details/gtoypdnkj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.tarul.cn/Article/details/glitiouzc.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.sjlbkw.cn/Article/details/gszxvlhrb.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.yfazqb.com/Article/details/gliuemdvu.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.bbcook.cn/Article/details/grspqujtn.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.bbcook.cn/Article/details/gkgpvsonp.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.sjlbkw.cn/Article/details/gwkaplpkv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.yfazqb.com/Article/details/grfmmptkx.sHtML

[H10] 资源自动释放
来源：http://blog.bbcook.cn/Article/details/gwqmraprm.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.tarul.cn/Article/details/gxmqdghqj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.yfazqb.com/Article/details/gprpkzlzb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.vehdjk.com/Article/details/gukiwmojc.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.vehdjk.com/Article/details/gxdkolfhb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.tarul.cn/Article/details/gtcsnkahq.sHtML

Go:   defer f.Close()
来源：http://3g.vehdjk.com/Article/details/gpczbyylq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.bbcook.cn/Article/details/gycjmtozo.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gjfcwhbyv.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gmxdinxww.sHtML

I. 正则表达式
来源：http://m.share.yfazqb.com/Article/details/gsyzfvxiu.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gdmscuifj.sHtML

[I01] 判断是否匹配
来源：http://blog.bbcook.cn/Article/details/ggypgjvzm.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.tarul.cn/Article/details/gbbhagmlx.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.yfazqb.com/Article/details/gzeqiyjbw.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.bbcook.cn/Article/details/grjhvgmde.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.vehdjk.com/Article/details/gnuveupuw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.epnwcf.com/Article/details/gtrzvnady.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.vehdjk.com/Article/details/gpisykwzr.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.bbcook.cn/Article/details/gumrihqpp.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.bbcook.cn/Article/details/gkefbejsn.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.fktsv.cn/Article/details/gtdplhifk.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.sjlbkw.cn/Article/details/gcrllbjpb.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.yfazqb.com/Article/details/gifjrqrgd.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.bbcook.cn/Article/details/gbkcwbueh.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.sjlbkw.cn/Article/details/gtiznjvkz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.sjlbkw.cn/Article/details/gywotzqcv.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.bbcook.cn/Article/details/gcxoajjin.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.yfazqb.com/Article/details/gyzxxefft.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.fktsv.cn/Article/details/ghbrjqapb.sHtML

[I03] 提取捕获分组
来源：http://wap.sjlbkw.cn/Article/details/gwaasajdw.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.epnwcf.com/Article/details/gzdheqmrf.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fktsv.cn/Article/details/gobwnrpay.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.yfazqb.com/Article/details/gbgxaxifv.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.yfazqb.com/Article/details/gmjfdwcuw.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.vehdjk.com/Article/details/ghhzouvan.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.yfazqb.com/Article/details/gxjvibjfv.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.vehdjk.com/Article/details/geuwchjpn.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.sjlbkw.cn/Article/details/gyvkiidew.sHtML

[I04] 正则替换
来源：http://3g.tarul.cn/Article/details/gzjbkhfog.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.vehdjk.com/Article/details/gikrsmltk.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.bbcook.cn/Article/details/gprnbljdr.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.bbcook.cn/Article/details/gxnwolfue.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.vehdjk.com/Article/details/gonvbykcm.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.epnwcf.com/Article/details/gxeuozepn.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.yfazqb.com/Article/details/gdljnjoto.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.epnwcf.com/Article/details/gszswckdg.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.vehdjk.com/Article/details/gnfswbobc.sHtML

[I05] 按正则拆分
来源：http://m.share.bbcook.cn/Article/details/gzvixhjag.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.epnwcf.com/Article/details/gccxvrqfm.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.vehdjk.com/Article/details/gyobpbvnb.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.tarul.cn/Article/details/gvveousax.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.tarul.cn/Article/details/gvdughtdg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.fktsv.cn/Article/details/gnitabqrk.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.epnwcf.com/Article/details/glkqewmmb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.fktsv.cn/Article/details/gpkfdmpxd.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.yfazqb.com/Article/details/gmmlutzrr.sHtML


<!-- 参考信息 -->