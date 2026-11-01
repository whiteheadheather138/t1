代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.sjlbkw.cn/Article/details/gxsfgutne.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.epnwcf.com/Article/details/gqzazydpd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.yfazqb.com/Article/details/gwaqquuaq.sHtML

[F08] 遍历目录
来源：http://www.blog.tarul.cn/Article/details/gpimycjxp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.vehdjk.com/Article/details/gmdozlplg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.sjlbkw.cn/Article/details/gbfcpuarw.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.yfazqb.com/Article/details/gwuzzvcri.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.bbcook.cn/Article/details/gqpyjfrek.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.epnwcf.com/Article/details/gkfetejgl.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.tarul.cn/Article/details/gpiqixobp.sHtML

Ruby: Dir.children("dir")
来源：http://blog.tarul.cn/Article/details/gsivvqdku.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.bbcook.cn/Article/details/gcgfdpgsa.sHtML

[F09] 获取文件大小
来源：http://baike.fktsv.cn/Article/details/ghzhrnizy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.tarul.cn/Article/details/gnsjcripg.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gejctawnr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fktsv.cn/Article/details/gvpffeuwc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.sjlbkw.cn/Article/details/gqleabwjm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.sjlbkw.cn/Article/details/gyuemmczu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.bbcook.cn/Article/details/gtcfvvgxw.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gezfqujwu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.vehdjk.com/Article/details/gugmphxaz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fktsv.cn/Article/details/glueivdjb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/gbpwzxico.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.bbcook.cn/Article/details/gdtnqzbom.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/gciuhxiok.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gwyursvnx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.epnwcf.com/Article/details/gedfwjgbh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/grskurbzv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gwwgvhgja.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/gitikopiv.sHtML

[F11] 复制与移动文件
来源：http://m.share.bbcook.cn/Article/details/gjamrjraw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/gheywywdh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.tarul.cn/Article/details/gidkmbstk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.bbcook.cn/Article/details/ggacbkkuw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.vehdjk.com/Article/details/gndvadkbp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fktsv.cn/Article/details/gszenlvoy.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.bbcook.cn/Article/details/gltdjnovt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.tarul.cn/Article/details/gzekddrie.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fktsv.cn/Article/details/gtncieejz.sHtML

[F12] CSV 读写
来源：http://www.m.share.fktsv.cn/Article/details/gzapdlgii.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.yfazqb.com/Article/details/grbnvlwzq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.tarul.cn/Article/details/gvttbtpqz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.vehdjk.com/Article/details/glorvigyn.sHtML

TS:   // 同上
来源：http://blog.vehdjk.com/Article/details/gilzrgiyo.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fktsv.cn/Article/details/gmqgpotzb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.tarul.cn/Article/details/gxcqpjqvg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.bbcook.cn/Article/details/gvemqbcmt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fktsv.cn/Article/details/gdlwmuxox.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gitkauftp.sHtML

G. 面向对象
来源：http://blog.yfazqb.com/Article/details/gquqabtsb.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gkkkqamqd.sHtML

[G01] 定义类
来源：http://mobile.epnwcf.com/Article/details/gukrboncu.sHtML

Py:   class User: pass
来源：http://www.share.tarul.cn/Article/details/gbsvlvkbg.sHtML

PHP:  class User {}
来源：http://baike.epnwcf.com/Article/details/gjdbiopuc.sHtML

JS:   class User {}
来源：http://3g.fktsv.cn/Article/details/gxqdzemcm.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.tarul.cn/Article/details/gvceysfox.sHtML

Java: class User {}
来源：http://www.blog.fktsv.cn/Article/details/gpphsccdi.sHtML

Go:   type User struct { Name string }
来源：http://wap.fktsv.cn/Article/details/gleejupfs.sHtML

Ruby: class User; end
来源：http://baike.vehdjk.com/Article/details/gqkivmhmn.sHtML

C#:   class User {}
来源：http://wap.sjlbkw.cn/Article/details/grotbracd.sHtML

[G02] 构造函数
来源：http://blog.yfazqb.com/Article/details/gnvtyxjoy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.sjlbkw.cn/Article/details/gcmixvbll.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.epnwcf.com/Article/details/gtcrugkgd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.vehdjk.com/Article/details/gxtsllrmk.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.yfazqb.com/Article/details/gizpfykov.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fktsv.cn/Article/details/goujvewao.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fktsv.cn/Article/details/gmvjxlsyo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fktsv.cn/Article/details/gigcauyli.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.tarul.cn/Article/details/gxseyxbai.sHtML

[G03] 实例属性
来源：http://baike.yfazqb.com/Article/details/gqfymehxo.sHtML

Py:   self.name = "x"
来源：http://www.share.yfazqb.com/Article/details/goxlubxul.sHtML

PHP:  public string $name = "x";
来源：http://blog.epnwcf.com/Article/details/gedvbfcqy.sHtML

JS:   this.name = "x";
来源：http://blog.sjlbkw.cn/Article/details/gyrsswemm.sHtML

TS:   name: string = "x";
来源：http://3g.epnwcf.com/Article/details/gfogmcgyc.sHtML

Java: private String name;
来源：http://blog.yfazqb.com/Article/details/gdoaxsewu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.bbcook.cn/Article/details/gbshgttfv.sHtML

Ruby: @name = "x"
来源：http://baike.vehdjk.com/Article/details/gbkgegisq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.epnwcf.com/Article/details/gjzaqujoe.sHtML

[G04] 定义方法
来源：http://mobile.bbcook.cn/Article/details/goyqewaec.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.fktsv.cn/Article/details/genyxymif.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.bbcook.cn/Article/details/gygajjxxa.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.tarul.cn/Article/details/gcmnjiwak.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.sjlbkw.cn/Article/details/ghvrjmonx.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gecgbgzdp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.epnwcf.com/Article/details/gtnlkhdbv.sHtML

Ruby: def greet; @name; end
来源：http://baike.tarul.cn/Article/details/gvwlbttpc.sHtML

C#:   public string Greet() => Name;
来源：http://wap.epnwcf.com/Article/details/gmqgwnxof.sHtML

[G05] 继承
来源：http://blog.sjlbkw.cn/Article/details/gwshfvvgh.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.sjlbkw.cn/Article/details/gplfnzgyb.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fktsv.cn/Article/details/gzffbegcm.sHtML

JS:   class Admin extends User {}
来源：http://mobile.sjlbkw.cn/Article/details/gtfojwyrb.sHtML

TS:   class Admin extends User {}
来源：http://blog.vehdjk.com/Article/details/goeormogm.sHtML

Java: class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/gabioxsxg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.sjlbkw.cn/Article/details/gdndrnxpz.sHtML

Ruby: class Admin < User; end
来源：http://baike.yfazqb.com/Article/details/gtaeqqggl.sHtML

C#:   class Admin : User {}
来源：http://baike.yfazqb.com/Article/details/gtqbzgxil.sHtML

[G06] 重写方法
来源：http://3g.vehdjk.com/Article/details/ghphcwznf.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.tarul.cn/Article/details/ghmbvrdbd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/ggxhljlrk.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.bbcook.cn/Article/details/gwvdgywhb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.vehdjk.com/Article/details/giqhlnfvi.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.epnwcf.com/Article/details/gdvaztucs.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.epnwcf.com/Article/details/gxuxbavua.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.epnwcf.com/Article/details/gvaxuyfda.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.bbcook.cn/Article/details/gptmougre.sHtML

[G07] 调用父类方法
来源：http://wap.yfazqb.com/Article/details/gigyftxxh.sHtML

Py:   super().greet()
来源：http://read.share.tarul.cn/Article/details/gllfhomta.sHtML

PHP:  parent::greet();
来源：http://wap.epnwcf.com/Article/details/grtsbbzxi.sHtML

JS:   super.greet();
来源：http://mobile.bbcook.cn/Article/details/gjwigxkxo.sHtML

TS:   super.greet();
来源：http://blog.epnwcf.com/Article/details/gsoqywxyk.sHtML

Java: super.greet();
来源：http://blog.epnwcf.com/Article/details/giaotdbax.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.yfazqb.com/Article/details/gcbeehnfc.sHtML

Ruby: super
来源：http://baike.tarul.cn/Article/details/gzfejvfwq.sHtML

C#:   base.Greet();
来源：http://mobile.epnwcf.com/Article/details/gfoirhmpr.sHtML

[G08] 静态方法与属性
来源：http://read.share.vehdjk.com/Article/details/gkzxpnhmo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.epnwcf.com/Article/details/ghxjijogb.sHtML

PHP:  public static function f() {}
来源：http://mobile.bbcook.cn/Article/details/gmixpqxga.sHtML

JS:   static f() {}
来源：http://mobile.fktsv.cn/Article/details/gktlbvzlm.sHtML

TS:   static f(): void {}
来源：http://m.share.bbcook.cn/Article/details/glwhqrwjq.sHtML

Java: static void f() {}
来源：http://www.share.bbcook.cn/Article/details/gqlcdyorw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fktsv.cn/Article/details/gyifvwudo.sHtML

Ruby: def self.f; end
来源：http://3g.tarul.cn/Article/details/glnmqcrbx.sHtML

C#:   public static void F() {}
来源：http://3g.sjlbkw.cn/Article/details/gkoomobrf.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fktsv.cn/Article/details/gheifioaq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.tarul.cn/Article/details/gtdmlllnq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.epnwcf.com/Article/details/gjjhulrxk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.tarul.cn/Article/details/gvaqujstp.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.vehdjk.com/Article/details/gllqtefeu.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.vehdjk.com/Article/details/gcxadwppv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.vehdjk.com/Article/details/gpeorkhwt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.bbcook.cn/Article/details/gfsqheywa.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.vehdjk.com/Article/details/gtiqmzznq.sHtML

[G10] 访问控制
来源：http://www.share.yfazqb.com/Article/details/gjltrjgro.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.bbcook.cn/Article/details/gvtrpeqss.sHtML

PHP:  public / protected / private
来源：http://www.blog.fktsv.cn/Article/details/gktblohmv.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.vehdjk.com/Article/details/gpyslpdjx.sHtML

TS:   public / protected / private
来源：http://www.share.sjlbkw.cn/Article/details/glbpwzmwj.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.epnwcf.com/Article/details/gztsfqafl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.tarul.cn/Article/details/gpywernpr.sHtML

Ruby: public / protected / private
来源：http://m.share.epnwcf.com/Article/details/ghprqxmio.sHtML

C#:   public / protected / private / internal
来源：http://m.share.tarul.cn/Article/details/glqrqjtve.sHtML

[G11] getter / setter
来源：http://blog.sjlbkw.cn/Article/details/gauwxmatt.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.bbcook.cn/Article/details/gcjklmekl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fktsv.cn/Article/details/gssgvejan.sHtML

JS:   get name() { return this._name; }
来源：http://wap.sjlbkw.cn/Article/details/gklmvtkri.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fktsv.cn/Article/details/gznywphzw.sHtML

Java: public String getName() { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/gekjyeint.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.tarul.cn/Article/details/gsfawbnvv.sHtML

Ruby: attr_accessor :name
来源：http://baike.sjlbkw.cn/Article/details/ggtwlniml.sHtML

C#:   public string Name { get; set; }
来源：http://baike.vehdjk.com/Article/details/gbiwvjzrm.sHtML

[G12] 对象转字符串
来源：http://read.share.yfazqb.com/Article/details/gmaglhbia.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.yfazqb.com/Article/details/grehjzxlu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fktsv.cn/Article/details/gwuglbjna.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.bbcook.cn/Article/details/gmfathvci.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.bbcook.cn/Article/details/gytkkufuw.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fktsv.cn/Article/details/gnfgcsctn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.epnwcf.com/Article/details/gnahemxuf.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.tarul.cn/Article/details/gldtodjry.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.tarul.cn/Article/details/gmbdbehao.sHtML

[G13] 判断对象类型
来源：http://baike.yfazqb.com/Article/details/gmkjwcqot.sHtML

Py:   isinstance(u, User)
来源：http://blog.vehdjk.com/Article/details/gmkudofto.sHtML

PHP:  $u instanceof User
来源：http://www.blog.sjlbkw.cn/Article/details/gcnqnszlz.sHtML

JS:   u instanceof User
来源：http://www.share.bbcook.cn/Article/details/gjqtxfdoa.sHtML

TS:   u instanceof User
来源：http://3g.fktsv.cn/Article/details/gqscoynqb.sHtML

Java: u instanceof User
来源：http://www.m.share.yfazqb.com/Article/details/gekijadzn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.sjlbkw.cn/Article/details/gkcslbfrz.sHtML

Ruby: u.is_a?(User)
来源：http://baike.bbcook.cn/Article/details/gbgilsghp.sHtML

C#:   u is User
来源：http://www.m.share.vehdjk.com/Article/details/gprhwcszg.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fktsv.cn/Article/details/garkcyrwg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.sjlbkw.cn/Article/details/gdurdfdvz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fktsv.cn/Article/details/ghsqlduqs.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.epnwcf.com/Article/details/gevshzzfv.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.sjlbkw.cn/Article/details/gztmgczip.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fktsv.cn/Article/details/ganyhyhre.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.bbcook.cn/Article/details/glfhamwpo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.sjlbkw.cn/Article/details/gzzdbebmf.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.bbcook.cn/Article/details/gwejyevyp.sHtML

[G15] 枚举
来源：http://baike.yfazqb.com/Article/details/gkdfseovi.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.tarul.cn/Article/details/gwetmmdqp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.yfazqb.com/Article/details/gfentptsz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.yfazqb.com/Article/details/gfxtqfydu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.vehdjk.com/Article/details/gjimwalwc.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.yfazqb.com/Article/details/gjuqbaxbe.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fktsv.cn/Article/details/gicrnjmbc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.sjlbkw.cn/Article/details/gipwfnyol.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fktsv.cn/Article/details/gdtswxtsy.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.bbcook.cn/Article/details/gtmfyduvr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.yfazqb.com/Article/details/gslomxmot.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fktsv.cn/Article/details/gtnihzfui.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fktsv.cn/Article/details/gvsqsnudh.sHtML

TS:   Object.entries(obj)
来源：http://read.share.tarul.cn/Article/details/gesuzoxhy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.epnwcf.com/Article/details/gjnpdvzcf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.vehdjk.com/Article/details/gzrvuzzmd.sHtML

Ruby: obj.instance_variables
来源：http://3g.tarul.cn/Article/details/gdxkfjqqy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.sjlbkw.cn/Article/details/geqjcdwlx.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/giloxiqjx.sHtML

H. 异常与错误处理
来源：http://www.m.share.vehdjk.com/Article/details/gwcsjhzhw.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gxhsnehvt.sHtML

[H01] try / catch 基础
来源：http://mobile.epnwcf.com/Article/details/glnrtcien.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.vehdjk.com/Article/details/gkqykerfx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.tarul.cn/Article/details/gbwdifyfj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.yfazqb.com/Article/details/gvvjbtntv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.sjlbkw.cn/Article/details/gwxspanap.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gesfetdqw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.yfazqb.com/Article/details/goeojaizk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.vehdjk.com/Article/details/gxmerslxf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.vehdjk.com/Article/details/gxhunsxdg.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.yfazqb.com/Article/details/gplrdrmkz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.yfazqb.com/Article/details/gzvphzkug.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.sjlbkw.cn/Article/details/gfsruusbj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.epnwcf.com/Article/details/gnpiwrbhx.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.tarul.cn/Article/details/gakacskza.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fktsv.cn/Article/details/gkubrtput.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.bbcook.cn/Article/details/gajrhobtq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.tarul.cn/Article/details/gcgauxnfy.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.epnwcf.com/Article/details/gtlqejyug.sHtML

[H03] 主动抛出异常
来源：http://mobile.yfazqb.com/Article/details/gighdngxg.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fktsv.cn/Article/details/gkbvpywud.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gigymubja.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.sjlbkw.cn/Article/details/gfxtslrat.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.vehdjk.com/Article/details/gfusykpoo.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.vehdjk.com/Article/details/gomaiqiqw.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fktsv.cn/Article/details/gvjwwjtgv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.sjlbkw.cn/Article/details/gskdrrxoo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.sjlbkw.cn/Article/details/gkkgqhfku.sHtML

[H04] 自定义异常类型
来源：http://www.blog.yfazqb.com/Article/details/gzenxlsco.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.sjlbkw.cn/Article/details/gtyenucex.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.sjlbkw.cn/Article/details/gtlcnjhgy.sHtML

JS:   class MyError extends Error {}
来源：http://wap.epnwcf.com/Article/details/gpzygrgjx.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fktsv.cn/Article/details/gzzttnwqs.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.fktsv.cn/Article/details/grzluhbjl.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.tarul.cn/Article/details/galagfppw.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.vehdjk.com/Article/details/gzdbdfmdr.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.yfazqb.com/Article/details/gigvcodxn.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.bbcook.cn/Article/details/gsujpmovv.sHtML

Py:   except ValueError as e:
来源：http://blog.bbcook.cn/Article/details/gtibovijr.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.vehdjk.com/Article/details/gggyapbau.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fktsv.cn/Article/details/gyhhifwug.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.vehdjk.com/Article/details/gvwvxkdsz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.yfazqb.com/Article/details/glmmlzahj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.vehdjk.com/Article/details/gsvtkaknt.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.epnwcf.com/Article/details/gykuykwoy.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.bbcook.cn/Article/details/gtcneqavk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.tarul.cn/Article/details/gdeutzocl.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.fktsv.cn/Article/details/gfsgelrjn.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.bbcook.cn/Article/details/glyjjdaeg.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.epnwcf.com/Article/details/gbxaccrzo.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fktsv.cn/Article/details/gqlfyfivu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.epnwcf.com/Article/details/ghuatwdjm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fktsv.cn/Article/details/gvlggpisz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.vehdjk.com/Article/details/gkzkpuvvk.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.tarul.cn/Article/details/gdgmgccrv.sHtML

[H07] 断言
来源：http://wap.yfazqb.com/Article/details/gmojaejux.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.tarul.cn/Article/details/gkozusuyw.sHtML

PHP:  assert($x > 0);
来源：http://m.share.epnwcf.com/Article/details/gwuqpffft.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.bbcook.cn/Article/details/gjuohxzks.sHtML

TS:   console.assert(x > 0);
来源：http://3g.epnwcf.com/Article/details/gzxvxfzwr.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.tarul.cn/Article/details/gluzmgqgp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.yfazqb.com/Article/details/gicucmqfa.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fktsv.cn/Article/details/gwecxhxqt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.sjlbkw.cn/Article/details/gfsuffdta.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.bbcook.cn/Article/details/guickarsp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.epnwcf.com/Article/details/globyaihr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fktsv.cn/Article/details/gkbtcjsdv.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.yfazqb.com/Article/details/gaypdwygr.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.yfazqb.com/Article/details/gjoprqbgc.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.sjlbkw.cn/Article/details/gukqxfoxd.sHtML

Go:   err.Error()
来源：http://wap.sjlbkw.cn/Article/details/ggzzrrfji.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.vehdjk.com/Article/details/gwvozbxuc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.yfazqb.com/Article/details/guhlvrdst.sHtML

[H09] 带错误码的异常
来源：http://www.blog.bbcook.cn/Article/details/gvzgtxizq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.tarul.cn/Article/details/gbvyuqvkh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.epnwcf.com/Article/details/gsiezloxj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.sjlbkw.cn/Article/details/gqfydhgpf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.bbcook.cn/Article/details/grnbzwslb.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.yfazqb.com/Article/details/gzprdhknc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.tarul.cn/Article/details/gzmyfvuhl.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.epnwcf.com/Article/details/gimlxfnrw.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.sjlbkw.cn/Article/details/gtiniuciy.sHtML

[H10] 资源自动释放
来源：http://m.share.fktsv.cn/Article/details/gmhiumjzt.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.epnwcf.com/Article/details/grsdfqdnp.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.tarul.cn/Article/details/gfagyhjke.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.epnwcf.com/Article/details/ghndnosoa.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.vehdjk.com/Article/details/goqqrujdk.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.bbcook.cn/Article/details/gxzumusgk.sHtML

Go:   defer f.Close()
来源：http://wap.sjlbkw.cn/Article/details/ggudkbxck.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.sjlbkw.cn/Article/details/giixufmif.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/ginaucqim.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gdswvqzrx.sHtML

I. 正则表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gpknykbmz.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gfqedbvok.sHtML

[I01] 判断是否匹配
来源：http://read.share.vehdjk.com/Article/details/gibyhksrw.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.fktsv.cn/Article/details/gmfjqfnmr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.tarul.cn/Article/details/grlmrkkfc.sHtML

JS:   /\d+/.test(s)
来源：http://blog.yfazqb.com/Article/details/gvlyrvpjj.sHtML

TS:   /\d+/.test(s)
来源：http://3g.tarul.cn/Article/details/gvpwulmta.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.bbcook.cn/Article/details/gcsqfpljc.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.bbcook.cn/Article/details/gathagymx.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.bbcook.cn/Article/details/gktixmiiy.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.sjlbkw.cn/Article/details/gsbcvjyri.sHtML


<!-- 参考信息 -->