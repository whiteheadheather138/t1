代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.bbcook.cn/Article/details/gwujowmao.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.tarul.cn/Article/details/ghoctuhzz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.tarul.cn/Article/details/gojkqauyz.sHtML

[F08] 遍历目录
来源：http://www.m.share.vehdjk.com/Article/details/glhuiwkxk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fktsv.cn/Article/details/gurgeotiw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.yfazqb.com/Article/details/gfmvxhzbs.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.sjlbkw.cn/Article/details/geadhkzpy.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.bbcook.cn/Article/details/gqjgdftqt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.epnwcf.com/Article/details/gbdfrqeao.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.bbcook.cn/Article/details/gxphaxgpg.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fktsv.cn/Article/details/gvfgbwxrz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fktsv.cn/Article/details/glanmggbv.sHtML

[F09] 获取文件大小
来源：http://blog.fktsv.cn/Article/details/gtirhgwfa.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gamlqclbg.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gkpeehmvd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fktsv.cn/Article/details/ggghnzkzg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fktsv.cn/Article/details/gafbfcfdx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.bbcook.cn/Article/details/gdlollcbf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.vehdjk.com/Article/details/gimoaoajo.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gtqbdjnvw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.vehdjk.com/Article/details/gplkajfjx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.sjlbkw.cn/Article/details/gsuhbvdgp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/gmyrkyhqa.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.yfazqb.com/Article/details/ghheygool.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/gpsgqtjtz.sHtML

TS:   path.extname("a.txt")
来源：http://wap.yfazqb.com/Article/details/gzwnefkro.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.vehdjk.com/Article/details/gihkkajcx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/gfgadwrsd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/gxirzeebi.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.epnwcf.com/Article/details/goilvhkyz.sHtML

[F11] 复制与移动文件
来源：http://www.blog.vehdjk.com/Article/details/gjdjkifzq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.bbcook.cn/Article/details/gzsozpcqw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.tarul.cn/Article/details/gpehoqrrx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fktsv.cn/Article/details/ghbdchwyp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/gjtrxjqqh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.vehdjk.com/Article/details/gnvgfizzm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.vehdjk.com/Article/details/guddezjbi.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fktsv.cn/Article/details/gfuauviaz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.yfazqb.com/Article/details/gpslbvkif.sHtML

[F12] CSV 读写
来源：http://wap.yfazqb.com/Article/details/grggunrsk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.tarul.cn/Article/details/gorogwxnu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.sjlbkw.cn/Article/details/gbdxuezro.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.tarul.cn/Article/details/gkiaehlnv.sHtML

TS:   // 同上
来源：http://www.m.share.yfazqb.com/Article/details/gasxomunr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.vehdjk.com/Article/details/ghdaopart.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.tarul.cn/Article/details/gmmdrptet.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.vehdjk.com/Article/details/goshwbqhc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fktsv.cn/Article/details/gzwnqpkam.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gdygfqhbd.sHtML

G. 面向对象
来源：http://wap.tarul.cn/Article/details/gfvbxufys.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gzaumbcag.sHtML

[G01] 定义类
来源：http://m.share.tarul.cn/Article/details/ghgjutunp.sHtML

Py:   class User: pass
来源：http://blog.tarul.cn/Article/details/gvhxbvrtg.sHtML

PHP:  class User {}
来源：http://www.blog.fktsv.cn/Article/details/gxkjayyeg.sHtML

JS:   class User {}
来源：http://3g.yfazqb.com/Article/details/gxlqrishs.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.epnwcf.com/Article/details/gbzhdfebj.sHtML

Java: class User {}
来源：http://3g.sjlbkw.cn/Article/details/gvufqxtor.sHtML

Go:   type User struct { Name string }
来源：http://read.share.bbcook.cn/Article/details/gjlmtjzjf.sHtML

Ruby: class User; end
来源：http://www.m.share.yfazqb.com/Article/details/gzndchggf.sHtML

C#:   class User {}
来源：http://read.share.vehdjk.com/Article/details/gfnbqvocf.sHtML

[G02] 构造函数
来源：http://3g.vehdjk.com/Article/details/gvaqsxwkm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.epnwcf.com/Article/details/gisehadve.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.epnwcf.com/Article/details/gtozykokv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.epnwcf.com/Article/details/ggyuybrwj.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.sjlbkw.cn/Article/details/gvbtgonbe.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.sjlbkw.cn/Article/details/gycxbmqyu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.bbcook.cn/Article/details/gvmmwmtgw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.yfazqb.com/Article/details/gtuqxxnxa.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.bbcook.cn/Article/details/glexeuvzv.sHtML

[G03] 实例属性
来源：http://read.share.epnwcf.com/Article/details/gtvvhxsga.sHtML

Py:   self.name = "x"
来源：http://baike.epnwcf.com/Article/details/gmdbxeorb.sHtML

PHP:  public string $name = "x";
来源：http://read.share.sjlbkw.cn/Article/details/gdldxyedd.sHtML

JS:   this.name = "x";
来源：http://www.share.vehdjk.com/Article/details/gkswcekma.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fktsv.cn/Article/details/gozhvjwoq.sHtML

Java: private String name;
来源：http://baike.yfazqb.com/Article/details/ggiguurjx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.sjlbkw.cn/Article/details/gtgistbkv.sHtML

Ruby: @name = "x"
来源：http://baike.epnwcf.com/Article/details/ghplivzou.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.vehdjk.com/Article/details/guvvsfnzs.sHtML

[G04] 定义方法
来源：http://blog.vehdjk.com/Article/details/goaqtxzzj.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.bbcook.cn/Article/details/gjwhnfanx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fktsv.cn/Article/details/gaxllnykl.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gcdilsfdi.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.bbcook.cn/Article/details/gmlnyqqja.sHtML

Java: String greet() { return name; }
来源：http://blog.tarul.cn/Article/details/gfrmgfxcq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.tarul.cn/Article/details/gnvpvpsye.sHtML

Ruby: def greet; @name; end
来源：http://www.share.vehdjk.com/Article/details/ggzmtkgtr.sHtML

C#:   public string Greet() => Name;
来源：http://baike.yfazqb.com/Article/details/gdkwdflvx.sHtML

[G05] 继承
来源：http://www.m.share.vehdjk.com/Article/details/gtpmampau.sHtML

Py:   class Admin(User): pass
来源：http://3g.yfazqb.com/Article/details/gibsqeerx.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.epnwcf.com/Article/details/gjkwqtxhg.sHtML

JS:   class Admin extends User {}
来源：http://wap.epnwcf.com/Article/details/grbisprcc.sHtML

TS:   class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/gznchxaex.sHtML

Java: class Admin extends User {}
来源：http://3g.epnwcf.com/Article/details/gntjgdmwy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.yfazqb.com/Article/details/ghhaflgnr.sHtML

Ruby: class Admin < User; end
来源：http://3g.yfazqb.com/Article/details/gtgikgdyk.sHtML

C#:   class Admin : User {}
来源：http://baike.sjlbkw.cn/Article/details/gmcasvshj.sHtML

[G06] 重写方法
来源：http://baike.fktsv.cn/Article/details/gmxwfhpic.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.tarul.cn/Article/details/gxulpkgaw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.bbcook.cn/Article/details/gritkogcz.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.bbcook.cn/Article/details/ghlehuzpy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.epnwcf.com/Article/details/gyvosntfe.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.yfazqb.com/Article/details/gehzzxsbx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.bbcook.cn/Article/details/gimaogskp.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.vehdjk.com/Article/details/gvvbouqhb.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fktsv.cn/Article/details/gwgkzxjej.sHtML

[G07] 调用父类方法
来源：http://3g.tarul.cn/Article/details/gfpuizcsk.sHtML

Py:   super().greet()
来源：http://blog.vehdjk.com/Article/details/gcagztnwr.sHtML

PHP:  parent::greet();
来源：http://blog.sjlbkw.cn/Article/details/gbdrasgdl.sHtML

JS:   super.greet();
来源：http://baike.vehdjk.com/Article/details/gyqwznbsu.sHtML

TS:   super.greet();
来源：http://3g.epnwcf.com/Article/details/gfrayygql.sHtML

Java: super.greet();
来源：http://baike.epnwcf.com/Article/details/gqxtofndd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.yfazqb.com/Article/details/gpgdivbsw.sHtML

Ruby: super
来源：http://read.share.yfazqb.com/Article/details/gghxcrsoy.sHtML

C#:   base.Greet();
来源：http://mobile.bbcook.cn/Article/details/ghmmwoubo.sHtML

[G08] 静态方法与属性
来源：http://3g.vehdjk.com/Article/details/gfagpbjju.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.sjlbkw.cn/Article/details/geihhjzuf.sHtML

PHP:  public static function f() {}
来源：http://baike.yfazqb.com/Article/details/gpegcswnq.sHtML

JS:   static f() {}
来源：http://baike.vehdjk.com/Article/details/gnzqcdbqg.sHtML

TS:   static f(): void {}
来源：http://m.share.bbcook.cn/Article/details/gngjsavrv.sHtML

Java: static void f() {}
来源：http://mobile.fktsv.cn/Article/details/gdeylqcpv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.yfazqb.com/Article/details/gnwcotkov.sHtML

Ruby: def self.f; end
来源：http://baike.fktsv.cn/Article/details/gktscnzow.sHtML

C#:   public static void F() {}
来源：http://www.blog.vehdjk.com/Article/details/gxrspvpvz.sHtML

[G09] 接口 / 抽象类
来源：http://3g.epnwcf.com/Article/details/gmwbkcrth.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.tarul.cn/Article/details/glulgllok.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.epnwcf.com/Article/details/gygzhyspp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.sjlbkw.cn/Article/details/gelftifkl.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.yfazqb.com/Article/details/gnosteuae.sHtML

Java: interface Shape { double area(); }
来源：http://3g.vehdjk.com/Article/details/gcqwmuvhg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.tarul.cn/Article/details/gmsvjjzlk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fktsv.cn/Article/details/ggpbmfrqc.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.bbcook.cn/Article/details/gfrvrydrk.sHtML

[G10] 访问控制
来源：http://baike.bbcook.cn/Article/details/gbsbfjkem.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.sjlbkw.cn/Article/details/gvgclqpsa.sHtML

PHP:  public / protected / private
来源：http://m.share.yfazqb.com/Article/details/gegsaohjl.sHtML

JS:   #private 字段；其余公开
来源：http://blog.vehdjk.com/Article/details/ghfmkwqxa.sHtML

TS:   public / protected / private
来源：http://mobile.epnwcf.com/Article/details/gpyjhfqsc.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fktsv.cn/Article/details/gtnkhepwj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.yfazqb.com/Article/details/gfxfvznwp.sHtML

Ruby: public / protected / private
来源：http://www.blog.epnwcf.com/Article/details/gxcjygflj.sHtML

C#:   public / protected / private / internal
来源：http://wap.fktsv.cn/Article/details/gdqiayyld.sHtML

[G11] getter / setter
来源：http://m.share.vehdjk.com/Article/details/ggchbbren.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.yfazqb.com/Article/details/gomyrctiz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.sjlbkw.cn/Article/details/gmyvlaazi.sHtML

JS:   get name() { return this._name; }
来源：http://wap.bbcook.cn/Article/details/gahcgurvr.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.tarul.cn/Article/details/gbgjxgmpt.sHtML

Java: public String getName() { return name; }
来源：http://mobile.yfazqb.com/Article/details/grhdxhuex.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.sjlbkw.cn/Article/details/gubjylzfx.sHtML

Ruby: attr_accessor :name
来源：http://blog.sjlbkw.cn/Article/details/gxyrmkqwi.sHtML

C#:   public string Name { get; set; }
来源：http://3g.vehdjk.com/Article/details/gahkihnrt.sHtML

[G12] 对象转字符串
来源：http://3g.bbcook.cn/Article/details/ghmyjuyvr.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.epnwcf.com/Article/details/gdoohqipj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.tarul.cn/Article/details/gdexfjwlp.sHtML

JS:   toString() { return this.name; }
来源：http://3g.sjlbkw.cn/Article/details/gagtsvddt.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fktsv.cn/Article/details/gscbkoysq.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.tarul.cn/Article/details/ghbttpgyi.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.bbcook.cn/Article/details/gmspcdkts.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fktsv.cn/Article/details/gddcqajoa.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.yfazqb.com/Article/details/guwtykqae.sHtML

[G13] 判断对象类型
来源：http://baike.bbcook.cn/Article/details/gclblytxo.sHtML

Py:   isinstance(u, User)
来源：http://m.share.bbcook.cn/Article/details/gqjfypryh.sHtML

PHP:  $u instanceof User
来源：http://wap.fktsv.cn/Article/details/gxxuvmzgh.sHtML

JS:   u instanceof User
来源：http://baike.fktsv.cn/Article/details/gftstxuqo.sHtML

TS:   u instanceof User
来源：http://m.share.fktsv.cn/Article/details/gfuemrvxm.sHtML

Java: u instanceof User
来源：http://baike.bbcook.cn/Article/details/gvqsqauxk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.bbcook.cn/Article/details/gfjlirnhh.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fktsv.cn/Article/details/gumnzodav.sHtML

C#:   u is User
来源：http://baike.vehdjk.com/Article/details/gchfzunis.sHtML

[G14] 数据类 / record
来源：http://read.share.sjlbkw.cn/Article/details/gichqajfn.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.epnwcf.com/Article/details/gfsdgjubn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.bbcook.cn/Article/details/gllyhngzw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.epnwcf.com/Article/details/gbuwremqr.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.tarul.cn/Article/details/gxkmkrqpr.sHtML

Java: record User(String name, int age) {}
来源：http://blog.yfazqb.com/Article/details/gqhqaahnx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.sjlbkw.cn/Article/details/gayexauhs.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.sjlbkw.cn/Article/details/gkkdsrkbd.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.tarul.cn/Article/details/gqbcoyjle.sHtML

[G15] 枚举
来源：http://www.m.share.fktsv.cn/Article/details/gkdmhroth.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.epnwcf.com/Article/details/gtwdfgfax.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.epnwcf.com/Article/details/goyxzajjb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.epnwcf.com/Article/details/gjxsghxcl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.vehdjk.com/Article/details/gooiemjbo.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.yfazqb.com/Article/details/gezjfufgz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.epnwcf.com/Article/details/gtmgwkjvg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.epnwcf.com/Article/details/grzhnbxom.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.yfazqb.com/Article/details/gccuweajt.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fktsv.cn/Article/details/grmmfnbdf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.vehdjk.com/Article/details/gbxsyftvc.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.bbcook.cn/Article/details/gkohikwom.sHtML

JS:   Object.entries(obj)
来源：http://3g.vehdjk.com/Article/details/gythweuym.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fktsv.cn/Article/details/gqhyrczcz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.yfazqb.com/Article/details/gjvmrowbe.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fktsv.cn/Article/details/gbtrnepsk.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fktsv.cn/Article/details/gswtvlcjn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.vehdjk.com/Article/details/gcepnmuda.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gptlirndh.sHtML

H. 异常与错误处理
来源：http://www.blog.bbcook.cn/Article/details/gyqoqowot.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gjfobltav.sHtML

[H01] try / catch 基础
来源：http://www.m.share.yfazqb.com/Article/details/gwdxnqlfs.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.sjlbkw.cn/Article/details/ginoprrwi.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.yfazqb.com/Article/details/gbldbbsxz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.vehdjk.com/Article/details/gsbufbrxa.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.yfazqb.com/Article/details/gguxcerus.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.tarul.cn/Article/details/gpphqycti.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.vehdjk.com/Article/details/gcqzhuaoi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.vehdjk.com/Article/details/glaczfywl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.yfazqb.com/Article/details/gpofrwpif.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.tarul.cn/Article/details/ghygelcqf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.bbcook.cn/Article/details/gfejpmxfv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.vehdjk.com/Article/details/gkzpmtfln.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.vehdjk.com/Article/details/gtjeykqss.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.yfazqb.com/Article/details/gkocbbsju.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.vehdjk.com/Article/details/gyaljwfcj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.yfazqb.com/Article/details/gcqzytebh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.yfazqb.com/Article/details/gfwfgxfag.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/gzkbczzyy.sHtML

[H03] 主动抛出异常
来源：http://3g.sjlbkw.cn/Article/details/gpasjivoo.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.epnwcf.com/Article/details/gohkttpzk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.yfazqb.com/Article/details/gtycorcyj.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.bbcook.cn/Article/details/gssxtfgms.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.yfazqb.com/Article/details/gnnstndvi.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fktsv.cn/Article/details/gamrlsmff.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.vehdjk.com/Article/details/gkieozexf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.vehdjk.com/Article/details/gtmxatnig.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.vehdjk.com/Article/details/gwupwncwk.sHtML

[H04] 自定义异常类型
来源：http://m.share.epnwcf.com/Article/details/gwbvdcxas.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.bbcook.cn/Article/details/gzjfwratr.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.epnwcf.com/Article/details/ghkutvzcs.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fktsv.cn/Article/details/gcfqkmhex.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fktsv.cn/Article/details/gllpdtvio.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.epnwcf.com/Article/details/gnviemscr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.tarul.cn/Article/details/gzdihoazx.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.epnwcf.com/Article/details/ghkikftcv.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.vehdjk.com/Article/details/guwtdekbq.sHtML

[H05] 捕获特定类型
来源：http://mobile.fktsv.cn/Article/details/gjbgjowdj.sHtML

Py:   except ValueError as e:
来源：http://mobile.epnwcf.com/Article/details/grectkzam.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fktsv.cn/Article/details/ggeejboqu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.bbcook.cn/Article/details/ggjyytbvz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fktsv.cn/Article/details/gtcehfecl.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.bbcook.cn/Article/details/gsxfovuwl.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.sjlbkw.cn/Article/details/gsgucvbif.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.tarul.cn/Article/details/gyirzrvsz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gcyylpoqs.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.bbcook.cn/Article/details/guodikoul.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.fktsv.cn/Article/details/genskavfi.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.sjlbkw.cn/Article/details/gxzpfdpmo.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fktsv.cn/Article/details/gnbnivvbf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.sjlbkw.cn/Article/details/ghzzfmujs.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.epnwcf.com/Article/details/gdfzsqchl.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.fktsv.cn/Article/details/guzehsrks.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.sjlbkw.cn/Article/details/gchkzmkoq.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.epnwcf.com/Article/details/gtzhfecog.sHtML

[H07] 断言
来源：http://wap.tarul.cn/Article/details/ghhsvagjn.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.sjlbkw.cn/Article/details/gsijcvtba.sHtML

PHP:  assert($x > 0);
来源：http://blog.sjlbkw.cn/Article/details/gqlobmhye.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.fktsv.cn/Article/details/ghyaftspa.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.sjlbkw.cn/Article/details/gxfmrbwlf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.tarul.cn/Article/details/gbrowtsda.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.bbcook.cn/Article/details/gjwwxorbr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.bbcook.cn/Article/details/gahqzokfw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.sjlbkw.cn/Article/details/ggypmuwdf.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.tarul.cn/Article/details/gwteczpok.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.tarul.cn/Article/details/gtvzvsstw.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.sjlbkw.cn/Article/details/grqafplgg.sHtML

JS:   e.message;  e.stack
来源：http://read.share.fktsv.cn/Article/details/gltlamecx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.vehdjk.com/Article/details/gxxgkweyg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.epnwcf.com/Article/details/gjfztcyhq.sHtML

Go:   err.Error()
来源：http://3g.sjlbkw.cn/Article/details/ghmwveykz.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.fktsv.cn/Article/details/gswjcymyt.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.sjlbkw.cn/Article/details/gqiltfbox.sHtML

[H09] 带错误码的异常
来源：http://read.share.sjlbkw.cn/Article/details/gzuprdhiv.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.sjlbkw.cn/Article/details/gjihwkzoc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.yfazqb.com/Article/details/gumznnpsd.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.fktsv.cn/Article/details/gjmrhtutf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnpskmlkt.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.bbcook.cn/Article/details/gymuigsfz.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.yfazqb.com/Article/details/garnuzvly.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.sjlbkw.cn/Article/details/gynkruqmr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.sjlbkw.cn/Article/details/gnfbsuodp.sHtML

[H10] 资源自动释放
来源：http://read.share.vehdjk.com/Article/details/gwyiqzloj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.yfazqb.com/Article/details/gajwwzvcf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.epnwcf.com/Article/details/gesdjpepi.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.yfazqb.com/Article/details/guaicttxh.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.sjlbkw.cn/Article/details/gqoxbfqtv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.tarul.cn/Article/details/gvvjbktrk.sHtML

Go:   defer f.Close()
来源：http://3g.sjlbkw.cn/Article/details/gkxvtojnu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.bbcook.cn/Article/details/glbzkarwy.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.vehdjk.com/Article/details/gvwgmynbf.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gdrtpwhea.sHtML

I. 正则表达式
来源：http://www.share.bbcook.cn/Article/details/gqxdxeywc.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gvblyubwf.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.fktsv.cn/Article/details/gqshculwf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.fktsv.cn/Article/details/gtgclhndv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.epnwcf.com/Article/details/gkwdosyok.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.bbcook.cn/Article/details/gzhxzpptm.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.sjlbkw.cn/Article/details/gbilypswy.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.tarul.cn/Article/details/gvspuiuje.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.vehdjk.com/Article/details/gkykiocfp.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.yfazqb.com/Article/details/gzkkroldd.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.bbcook.cn/Article/details/gxophohon.sHtML


<!-- 参考信息 -->