代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/goocibqwj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.epnwcf.com/Article/details/gylmzzjrn.sHtML

[F11] 复制与移动文件
来源：http://read.share.tarul.cn/Article/details/gvpgfnyli.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.tarul.cn/Article/details/gngprqfkb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.tarul.cn/Article/details/gjwoylaoe.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.vehdjk.com/Article/details/gmcsjvcbe.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gstrustpe.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.tarul.cn/Article/details/gsqzatvtr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.epnwcf.com/Article/details/gigtrnsqm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.yfazqb.com/Article/details/gvbzlpque.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.epnwcf.com/Article/details/gxpnivenu.sHtML

[F12] CSV 读写
来源：http://read.share.sjlbkw.cn/Article/details/glsetefkg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.yfazqb.com/Article/details/gkydksdoc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fktsv.cn/Article/details/gynrvlooh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.sjlbkw.cn/Article/details/grloyzkvt.sHtML

TS:   // 同上
来源：http://www.share.sjlbkw.cn/Article/details/gpyjzpxzk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.yfazqb.com/Article/details/gcmtfbxvt.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.yfazqb.com/Article/details/gckahyxox.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.tarul.cn/Article/details/gqszmtlxo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.vehdjk.com/Article/details/gjbpqhmgg.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/giuuoqxco.sHtML

G. 面向对象
来源：http://blog.bbcook.cn/Article/details/geoicadic.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gsbcxpcde.sHtML

[G01] 定义类
来源：http://mobile.epnwcf.com/Article/details/ggrwumcpd.sHtML

Py:   class User: pass
来源：http://mobile.vehdjk.com/Article/details/gnscgjtbq.sHtML

PHP:  class User {}
来源：http://blog.epnwcf.com/Article/details/gdqtsdxkk.sHtML

JS:   class User {}
来源：http://wap.vehdjk.com/Article/details/gircmpnri.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.yfazqb.com/Article/details/gcfvrmjsu.sHtML

Java: class User {}
来源：http://3g.tarul.cn/Article/details/gybkthakn.sHtML

Go:   type User struct { Name string }
来源：http://baike.vehdjk.com/Article/details/gwdqqsxvl.sHtML

Ruby: class User; end
来源：http://www.share.vehdjk.com/Article/details/gselaamoz.sHtML

C#:   class User {}
来源：http://m.share.tarul.cn/Article/details/gosxmnudv.sHtML

[G02] 构造函数
来源：http://www.blog.yfazqb.com/Article/details/gmxryqndx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.sjlbkw.cn/Article/details/gznwlvimx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.yfazqb.com/Article/details/gaoiqveur.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.tarul.cn/Article/details/gzubncuhz.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.yfazqb.com/Article/details/gqihezqms.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.yfazqb.com/Article/details/gbeltoiva.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fktsv.cn/Article/details/gnhwuwtgj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.tarul.cn/Article/details/gstebdsrt.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.vehdjk.com/Article/details/ghpfdahbd.sHtML

[G03] 实例属性
来源：http://blog.vehdjk.com/Article/details/gswrnorwp.sHtML

Py:   self.name = "x"
来源：http://m.share.vehdjk.com/Article/details/gfzdyntmi.sHtML

PHP:  public string $name = "x";
来源：http://blog.tarul.cn/Article/details/gafeeueha.sHtML

JS:   this.name = "x";
来源：http://3g.tarul.cn/Article/details/gbxlacqtj.sHtML

TS:   name: string = "x";
来源：http://www.blog.yfazqb.com/Article/details/gyfpzzlxt.sHtML

Java: private String name;
来源：http://read.share.yfazqb.com/Article/details/gtjhvbsgs.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.epnwcf.com/Article/details/gyvroucgs.sHtML

Ruby: @name = "x"
来源：http://3g.tarul.cn/Article/details/ghmsujmrx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.yfazqb.com/Article/details/gsfnlngni.sHtML

[G04] 定义方法
来源：http://blog.tarul.cn/Article/details/gkeaevnds.sHtML

Py:   def greet(self): return self.name
来源：http://3g.epnwcf.com/Article/details/gjhwooilj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.tarul.cn/Article/details/gxbcyxaen.sHtML

JS:   greet() { return this.name; }
来源：http://blog.epnwcf.com/Article/details/gkhamziie.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.vehdjk.com/Article/details/gogpcqgdo.sHtML

Java: String greet() { return name; }
来源：http://www.share.fktsv.cn/Article/details/goypdfhti.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.epnwcf.com/Article/details/gqhqtydhc.sHtML

Ruby: def greet; @name; end
来源：http://3g.yfazqb.com/Article/details/gsgyblhmf.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.yfazqb.com/Article/details/gwjcerhvs.sHtML

[G05] 继承
来源：http://www.m.share.vehdjk.com/Article/details/gqkbqkpmk.sHtML

Py:   class Admin(User): pass
来源：http://3g.epnwcf.com/Article/details/gazkxnvhh.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.sjlbkw.cn/Article/details/gnjemhtdq.sHtML

JS:   class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gmsrdagfm.sHtML

TS:   class Admin extends User {}
来源：http://www.share.bbcook.cn/Article/details/gqhmdnsct.sHtML

Java: class Admin extends User {}
来源：http://www.share.sjlbkw.cn/Article/details/gwsvzncjc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fktsv.cn/Article/details/geypakcfi.sHtML

Ruby: class Admin < User; end
来源：http://wap.sjlbkw.cn/Article/details/gbfcsqzjz.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.epnwcf.com/Article/details/garkdrewd.sHtML

[G06] 重写方法
来源：http://read.share.sjlbkw.cn/Article/details/gxslunfaj.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.tarul.cn/Article/details/gmnzfckad.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/gbfrqsamw.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.vehdjk.com/Article/details/gxdqkvjci.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.bbcook.cn/Article/details/gnpgqmtjs.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.tarul.cn/Article/details/gnsxqugwm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.sjlbkw.cn/Article/details/gbsdxojnf.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.yfazqb.com/Article/details/glbaiobit.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.tarul.cn/Article/details/gydyqtlez.sHtML

[G07] 调用父类方法
来源：http://www.m.share.bbcook.cn/Article/details/gtesxrqwk.sHtML

Py:   super().greet()
来源：http://3g.vehdjk.com/Article/details/gxczmzemx.sHtML

PHP:  parent::greet();
来源：http://www.share.bbcook.cn/Article/details/gbvybznvc.sHtML

JS:   super.greet();
来源：http://mobile.yfazqb.com/Article/details/gkjpgbiqe.sHtML

TS:   super.greet();
来源：http://www.share.sjlbkw.cn/Article/details/gyqgvygcu.sHtML

Java: super.greet();
来源：http://wap.vehdjk.com/Article/details/gbmraylld.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.vehdjk.com/Article/details/gbtfsqutj.sHtML

Ruby: super
来源：http://mobile.yfazqb.com/Article/details/grbmscyvd.sHtML

C#:   base.Greet();
来源：http://baike.vehdjk.com/Article/details/gwwtrdpao.sHtML

[G08] 静态方法与属性
来源：http://m.share.vehdjk.com/Article/details/geeaeiote.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.epnwcf.com/Article/details/gdtsphurr.sHtML

PHP:  public static function f() {}
来源：http://baike.yfazqb.com/Article/details/gxdxbmpfg.sHtML

JS:   static f() {}
来源：http://www.m.share.bbcook.cn/Article/details/gofrqucdy.sHtML

TS:   static f(): void {}
来源：http://m.share.sjlbkw.cn/Article/details/gdbcljdcu.sHtML

Java: static void f() {}
来源：http://www.share.yfazqb.com/Article/details/gkqfjqqnm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.yfazqb.com/Article/details/gwjbkngam.sHtML

Ruby: def self.f; end
来源：http://www.blog.sjlbkw.cn/Article/details/gkgehvmmq.sHtML

C#:   public static void F() {}
来源：http://www.share.epnwcf.com/Article/details/gafniykqd.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.vehdjk.com/Article/details/gifyveual.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.bbcook.cn/Article/details/geacxihca.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.sjlbkw.cn/Article/details/gpbnbfhpz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.epnwcf.com/Article/details/ghdrxlgal.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.bbcook.cn/Article/details/gluwfhzpz.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.tarul.cn/Article/details/gzgvxowby.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.epnwcf.com/Article/details/gfilirxnr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.yfazqb.com/Article/details/gsksylkoh.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.sjlbkw.cn/Article/details/gycjlqxht.sHtML

[G10] 访问控制
来源：http://www.blog.sjlbkw.cn/Article/details/gfndfuxrm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.tarul.cn/Article/details/gjnctrmnm.sHtML

PHP:  public / protected / private
来源：http://mobile.epnwcf.com/Article/details/ggsjkvuoh.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.epnwcf.com/Article/details/gagleofej.sHtML

TS:   public / protected / private
来源：http://www.share.epnwcf.com/Article/details/gjdmtiqhv.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.yfazqb.com/Article/details/gqizljfyd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.epnwcf.com/Article/details/ggepcvbxp.sHtML

Ruby: public / protected / private
来源：http://read.share.sjlbkw.cn/Article/details/gwixzxtzi.sHtML

C#:   public / protected / private / internal
来源：http://baike.tarul.cn/Article/details/gymrtebjj.sHtML

[G11] getter / setter
来源：http://m.share.vehdjk.com/Article/details/gzdzwxtxm.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fktsv.cn/Article/details/gjabhbnuw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.bbcook.cn/Article/details/guwbhyqvk.sHtML

JS:   get name() { return this._name; }
来源：http://3g.bbcook.cn/Article/details/gxvqhevsd.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.yfazqb.com/Article/details/grlqehdur.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fktsv.cn/Article/details/gfedoseil.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.sjlbkw.cn/Article/details/gxegdalxv.sHtML

Ruby: attr_accessor :name
来源：http://www.share.sjlbkw.cn/Article/details/grutykymi.sHtML

C#:   public string Name { get; set; }
来源：http://wap.bbcook.cn/Article/details/gyfyenzgd.sHtML

[G12] 对象转字符串
来源：http://m.share.epnwcf.com/Article/details/gnrnnszmt.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.epnwcf.com/Article/details/gsoqrbgis.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.epnwcf.com/Article/details/glnpzqbws.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.vehdjk.com/Article/details/gnaafkxdi.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gvkjqrnaq.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.bbcook.cn/Article/details/gvjrnsakw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.bbcook.cn/Article/details/gaecoyste.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.epnwcf.com/Article/details/gpmkxccnd.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.epnwcf.com/Article/details/ggyvhuazg.sHtML

[G13] 判断对象类型
来源：http://www.blog.yfazqb.com/Article/details/gjlmqkpjt.sHtML

Py:   isinstance(u, User)
来源：http://m.share.yfazqb.com/Article/details/gsddyfibr.sHtML

PHP:  $u instanceof User
来源：http://www.share.tarul.cn/Article/details/gueznjwvb.sHtML

JS:   u instanceof User
来源：http://wap.sjlbkw.cn/Article/details/gbmxpqbvs.sHtML

TS:   u instanceof User
来源：http://baike.epnwcf.com/Article/details/gviycrach.sHtML

Java: u instanceof User
来源：http://read.share.fktsv.cn/Article/details/gsndzcobo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fktsv.cn/Article/details/gjdcyaznh.sHtML

Ruby: u.is_a?(User)
来源：http://baike.tarul.cn/Article/details/gqlizenfi.sHtML

C#:   u is User
来源：http://read.share.fktsv.cn/Article/details/gdxvuzyli.sHtML

[G14] 数据类 / record
来源：http://3g.vehdjk.com/Article/details/gyoduurbn.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.sjlbkw.cn/Article/details/gopsktehh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.sjlbkw.cn/Article/details/ggiizmtgi.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.vehdjk.com/Article/details/gkusufkmi.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.epnwcf.com/Article/details/gdbymnhnf.sHtML

Java: record User(String name, int age) {}
来源：http://wap.sjlbkw.cn/Article/details/gmfclnehk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fktsv.cn/Article/details/gdaemnymv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fktsv.cn/Article/details/getkmwocz.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.sjlbkw.cn/Article/details/gsueaovqj.sHtML

[G15] 枚举
来源：http://m.share.yfazqb.com/Article/details/geiayybos.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.vehdjk.com/Article/details/gvwgegznb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.bbcook.cn/Article/details/gerlpnphz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.vehdjk.com/Article/details/gactxdswq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.epnwcf.com/Article/details/gjokgmjtk.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.epnwcf.com/Article/details/gzbiccokj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.bbcook.cn/Article/details/gerxfvmlq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fktsv.cn/Article/details/gvtakelyr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.yfazqb.com/Article/details/gyjbvgvwk.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.bbcook.cn/Article/details/gwotdrxvn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fktsv.cn/Article/details/gagajlfjs.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.yfazqb.com/Article/details/glyvupram.sHtML

JS:   Object.entries(obj)
来源：http://wap.bbcook.cn/Article/details/gxftevnbo.sHtML

TS:   Object.entries(obj)
来源：http://baike.bbcook.cn/Article/details/gcdndhznv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.sjlbkw.cn/Article/details/gnjtzdgcy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.yfazqb.com/Article/details/gsaucjxgi.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fktsv.cn/Article/details/gtdszxmgz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.vehdjk.com/Article/details/gpuunmujr.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/getfxprrz.sHtML

H. 异常与错误处理
来源：http://www.m.share.tarul.cn/Article/details/gedbkueoq.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gpwczdnic.sHtML

[H01] try / catch 基础
来源：http://mobile.fktsv.cn/Article/details/ghjbbiayc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.tarul.cn/Article/details/gmicmgkxi.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.bbcook.cn/Article/details/gbjohkmjn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fktsv.cn/Article/details/gebgjvlxi.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.bbcook.cn/Article/details/griridhus.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.bbcook.cn/Article/details/gynftmqyy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.bbcook.cn/Article/details/ghdkeyqfm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.tarul.cn/Article/details/gmurgzypw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.tarul.cn/Article/details/gkrdjcqte.sHtML

[H02] finally / ensure 收尾
来源：http://blog.bbcook.cn/Article/details/gawvhnsky.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.vehdjk.com/Article/details/gpbxsafhz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.bbcook.cn/Article/details/gnpbaoqwv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/gugxceptu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fktsv.cn/Article/details/gnahrxzsd.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.sjlbkw.cn/Article/details/glpabmxcx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.sjlbkw.cn/Article/details/gpkkgvyck.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.bbcook.cn/Article/details/gaztmqtcx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.vehdjk.com/Article/details/gnslmicqd.sHtML

[H03] 主动抛出异常
来源：http://www.blog.yfazqb.com/Article/details/gfxgtemkk.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.vehdjk.com/Article/details/gpqxbewti.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.tarul.cn/Article/details/ggphkwkpt.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.epnwcf.com/Article/details/gsvhrmtvx.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.fktsv.cn/Article/details/gfxufqblz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.yfazqb.com/Article/details/gkigjclwv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.yfazqb.com/Article/details/gdkshrerq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.bbcook.cn/Article/details/gnlrdwmvr.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.tarul.cn/Article/details/gnarwhgdp.sHtML

[H04] 自定义异常类型
来源：http://m.share.vehdjk.com/Article/details/gbmiydkoc.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.bbcook.cn/Article/details/guxsllpph.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.yfazqb.com/Article/details/glxvmevsy.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.bbcook.cn/Article/details/glahttrrw.sHtML

TS:   class MyError extends Error {}
来源：http://baike.sjlbkw.cn/Article/details/ghyrtdyst.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fktsv.cn/Article/details/ggekxajpx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.epnwcf.com/Article/details/ggvphpeyr.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.fktsv.cn/Article/details/gscfgrrky.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fktsv.cn/Article/details/gfpwjcrru.sHtML

[H05] 捕获特定类型
来源：http://www.blog.bbcook.cn/Article/details/gyqvjzzcy.sHtML

Py:   except ValueError as e:
来源：http://mobile.fktsv.cn/Article/details/gdiukzqcj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fktsv.cn/Article/details/gvbaijvfh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.tarul.cn/Article/details/gxvbokhmt.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.bbcook.cn/Article/details/gmrdlkmfu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.yfazqb.com/Article/details/ggjrpixel.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.epnwcf.com/Article/details/gtecitmcs.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fktsv.cn/Article/details/gxpiifrzr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.sjlbkw.cn/Article/details/gkfkwxutj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.bbcook.cn/Article/details/gvpewrrnz.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.epnwcf.com/Article/details/giiwjgjuc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.epnwcf.com/Article/details/gmbjnysoh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.epnwcf.com/Article/details/gxiujtylb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.epnwcf.com/Article/details/gqyemgbeg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.fktsv.cn/Article/details/gkmvqamcr.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.bbcook.cn/Article/details/gavgtwxgm.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.sjlbkw.cn/Article/details/gbkzgwrzh.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.yfazqb.com/Article/details/gyggvfmgb.sHtML

[H07] 断言
来源：http://mobile.fktsv.cn/Article/details/gzkqmkuhe.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.vehdjk.com/Article/details/gpkrfovxj.sHtML

PHP:  assert($x > 0);
来源：http://m.share.yfazqb.com/Article/details/gwmdqaeww.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.bbcook.cn/Article/details/gwomijtup.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.vehdjk.com/Article/details/gjndzsgwa.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.yfazqb.com/Article/details/gjapfbjoe.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.yfazqb.com/Article/details/gydfsevoh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.vehdjk.com/Article/details/glgqlhdis.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.vehdjk.com/Article/details/gkfvyujry.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.epnwcf.com/Article/details/gilvmnvha.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.yfazqb.com/Article/details/gwbpzgegw.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.yfazqb.com/Article/details/gycoenlei.sHtML

JS:   e.message;  e.stack
来源：http://blog.sjlbkw.cn/Article/details/gwpcbqool.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.epnwcf.com/Article/details/gpyngtmzm.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.epnwcf.com/Article/details/gcogcksxd.sHtML

Go:   err.Error()
来源：http://read.share.epnwcf.com/Article/details/gtpxvwhis.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.sjlbkw.cn/Article/details/gnwqtpbhb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.bbcook.cn/Article/details/gocnhaiuj.sHtML

[H09] 带错误码的异常
来源：http://baike.bbcook.cn/Article/details/gzfrxqnwg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.yfazqb.com/Article/details/gvzpsycxr.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.sjlbkw.cn/Article/details/gnhsnanfo.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzexynkvf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.sjlbkw.cn/Article/details/gadxfvjrq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.tarul.cn/Article/details/gqxlrlntn.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.sjlbkw.cn/Article/details/gncotiwmk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.sjlbkw.cn/Article/details/gcbxvxxau.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.bbcook.cn/Article/details/gcoufvson.sHtML

[H10] 资源自动释放
来源：http://read.share.vehdjk.com/Article/details/gturqwvet.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.yfazqb.com/Article/details/gvpfmjtrl.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.bbcook.cn/Article/details/ggngvclrb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fktsv.cn/Article/details/glldhtvgd.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.yfazqb.com/Article/details/giwdpcjzb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.epnwcf.com/Article/details/gscdyjhxc.sHtML

Go:   defer f.Close()
来源：http://read.share.bbcook.cn/Article/details/gmyrwjhii.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.yfazqb.com/Article/details/gyfhbrssx.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.tarul.cn/Article/details/gqqpcwgkz.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gngsirsmn.sHtML

I. 正则表达式
来源：http://mobile.yfazqb.com/Article/details/gheqkxzbz.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gzzieyztb.sHtML

[I01] 判断是否匹配
来源：http://www.share.fktsv.cn/Article/details/ghiqzrlls.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.bbcook.cn/Article/details/gkmkuiokk.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.vehdjk.com/Article/details/geddorvys.sHtML

JS:   /\d+/.test(s)
来源：http://3g.tarul.cn/Article/details/gbhzkcgnr.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.vehdjk.com/Article/details/gvkajzrwc.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.bbcook.cn/Article/details/goumjyglj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.tarul.cn/Article/details/gltiqcqno.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.yfazqb.com/Article/details/gztslcfco.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.sjlbkw.cn/Article/details/gcobyziap.sHtML

[I02] 提取所有匹配
来源：http://3g.epnwcf.com/Article/details/gsegivzkf.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.sjlbkw.cn/Article/details/gihyrmjaz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.fktsv.cn/Article/details/gorxbeggn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.bbcook.cn/Article/details/gsoluqojf.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.epnwcf.com/Article/details/gprzgnwcg.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.bbcook.cn/Article/details/gnbexvizs.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fktsv.cn/Article/details/gybtmwoqq.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.epnwcf.com/Article/details/guoyqhvjv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.bbcook.cn/Article/details/gguxwrzvp.sHtML

[I03] 提取捕获分组
来源：http://3g.bbcook.cn/Article/details/gwcrohowr.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.tarul.cn/Article/details/gwvpykymk.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.sjlbkw.cn/Article/details/gqzratmqa.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.fktsv.cn/Article/details/gtslhmqrs.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.epnwcf.com/Article/details/gwxsctslr.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.fktsv.cn/Article/details/gfrlarnrk.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.vehdjk.com/Article/details/gxptfalls.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.fktsv.cn/Article/details/gazbtmbjk.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.fktsv.cn/Article/details/gkiojedog.sHtML

[I04] 正则替换
来源：http://blog.bbcook.cn/Article/details/glnmiqeyc.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.yfazqb.com/Article/details/gebtcfqow.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.yfazqb.com/Article/details/gjlyymcob.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.sjlbkw.cn/Article/details/gtnmykgbg.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.sjlbkw.cn/Article/details/gbifeewhz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.epnwcf.com/Article/details/gxecgryrv.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.bbcook.cn/Article/details/gmqmasznt.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.vehdjk.com/Article/details/gqxvjdtfd.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.epnwcf.com/Article/details/getmqhbzo.sHtML

[I05] 按正则拆分
来源：http://m.share.fktsv.cn/Article/details/gxtmsxmlm.sHtML


<!-- 参考信息 -->