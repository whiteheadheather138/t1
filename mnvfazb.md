代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.tarul.cn/Article/details/gmepvhudl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.yfazqb.com/Article/details/gmjepekdx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.bbcook.cn/Article/details/gjtyajxne.sHtML

[F08] 遍历目录
来源：http://www.m.share.fktsv.cn/Article/details/gifbrhsbi.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.tarul.cn/Article/details/glljzmije.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.bbcook.cn/Article/details/glfdpjlol.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.yfazqb.com/Article/details/gidyavnqs.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.tarul.cn/Article/details/gekxhggfu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.epnwcf.com/Article/details/gndtwztlo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.yfazqb.com/Article/details/gykziajha.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fktsv.cn/Article/details/gjomlbfin.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.tarul.cn/Article/details/gvjmuancz.sHtML

[F09] 获取文件大小
来源：http://www.m.share.sjlbkw.cn/Article/details/gqolmxwdp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gvuqtssji.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gmycmeecg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.bbcook.cn/Article/details/gsxnpxrsg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.bbcook.cn/Article/details/gntjxtkuz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.tarul.cn/Article/details/gsrcvzwkw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.sjlbkw.cn/Article/details/geiuvkfev.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gtaccxkpe.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.vehdjk.com/Article/details/gvayaqvyj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.epnwcf.com/Article/details/gwittatip.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/gzdjjcvxf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.bbcook.cn/Article/details/gzgsfrdwx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gshsgpnnu.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gjbjbldry.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.yfazqb.com/Article/details/gqhwgmsta.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.vehdjk.com/Article/details/gotvvjcyv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/gqiydeaey.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.vehdjk.com/Article/details/gpuvacwfd.sHtML

[F11] 复制与移动文件
来源：http://wap.vehdjk.com/Article/details/gqjcdphlu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.sjlbkw.cn/Article/details/gokmhuhqg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gipbrrhmp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.vehdjk.com/Article/details/gxrzhzgar.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/gcjqylvfl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.tarul.cn/Article/details/gvuxuwpno.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.bbcook.cn/Article/details/gwmvzynia.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fktsv.cn/Article/details/givtrocrg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.epnwcf.com/Article/details/gejijpwuy.sHtML

[F12] CSV 读写
来源：http://www.m.share.tarul.cn/Article/details/gwrmmqvvc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.bbcook.cn/Article/details/gqrbuplve.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fktsv.cn/Article/details/gudwsjirc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fktsv.cn/Article/details/gwyplkgun.sHtML

TS:   // 同上
来源：http://wap.vehdjk.com/Article/details/gczyllgqg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.yfazqb.com/Article/details/ggaeginxh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.yfazqb.com/Article/details/grqkjsgbx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.yfazqb.com/Article/details/gnulewxfn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.epnwcf.com/Article/details/gbflmwuqo.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gsiyasamj.sHtML

G. 面向对象
来源：http://www.blog.sjlbkw.cn/Article/details/gmlgxusnp.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gwdepsjys.sHtML

[G01] 定义类
来源：http://www.blog.yfazqb.com/Article/details/gnepmgwtt.sHtML

Py:   class User: pass
来源：http://www.blog.bbcook.cn/Article/details/ghcemfikf.sHtML

PHP:  class User {}
来源：http://m.share.fktsv.cn/Article/details/gehoictfm.sHtML

JS:   class User {}
来源：http://blog.sjlbkw.cn/Article/details/gbizmyrdu.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fktsv.cn/Article/details/gsqjsggrn.sHtML

Java: class User {}
来源：http://mobile.vehdjk.com/Article/details/gwwrhdsnz.sHtML

Go:   type User struct { Name string }
来源：http://blog.vehdjk.com/Article/details/gjsqfwadi.sHtML

Ruby: class User; end
来源：http://m.share.yfazqb.com/Article/details/gycwqamqg.sHtML

C#:   class User {}
来源：http://3g.bbcook.cn/Article/details/ggvxmlgqk.sHtML

[G02] 构造函数
来源：http://www.m.share.fktsv.cn/Article/details/gdbvfeuzi.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.sjlbkw.cn/Article/details/gwkeepcoq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.bbcook.cn/Article/details/guwffitel.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.epnwcf.com/Article/details/gfqpgwigb.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fktsv.cn/Article/details/gzcobiuwf.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.tarul.cn/Article/details/gcheyhmnc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.epnwcf.com/Article/details/gkzviguxu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.yfazqb.com/Article/details/gliqnvowf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.epnwcf.com/Article/details/gwpqoiszo.sHtML

[G03] 实例属性
来源：http://m.share.epnwcf.com/Article/details/gefpbmrwl.sHtML

Py:   self.name = "x"
来源：http://wap.sjlbkw.cn/Article/details/gtcrcxdzs.sHtML

PHP:  public string $name = "x";
来源：http://blog.vehdjk.com/Article/details/ghxawfscm.sHtML

JS:   this.name = "x";
来源：http://www.share.vehdjk.com/Article/details/gxrqhyrhv.sHtML

TS:   name: string = "x";
来源：http://mobile.fktsv.cn/Article/details/gwgwqxtyw.sHtML

Java: private String name;
来源：http://3g.bbcook.cn/Article/details/gtrayftoh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.sjlbkw.cn/Article/details/ghnsvfkye.sHtML

Ruby: @name = "x"
来源：http://m.share.fktsv.cn/Article/details/gsmpehndd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.yfazqb.com/Article/details/grkporvuu.sHtML

[G04] 定义方法
来源：http://www.m.share.fktsv.cn/Article/details/ghaazpdvb.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fktsv.cn/Article/details/gwgihdgvj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.sjlbkw.cn/Article/details/gzmqtfmoh.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.epnwcf.com/Article/details/glexvitzz.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.epnwcf.com/Article/details/glzreaoza.sHtML

Java: String greet() { return name; }
来源：http://blog.vehdjk.com/Article/details/grgpgzlum.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.vehdjk.com/Article/details/gliksbnwu.sHtML

Ruby: def greet; @name; end
来源：http://wap.yfazqb.com/Article/details/gnphuxfag.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.tarul.cn/Article/details/gbolakmgl.sHtML

[G05] 继承
来源：http://3g.bbcook.cn/Article/details/gcwepjrzl.sHtML

Py:   class Admin(User): pass
来源：http://m.share.tarul.cn/Article/details/gfobgfxzj.sHtML

PHP:  class Admin extends User {}
来源：http://3g.sjlbkw.cn/Article/details/gzpnuhbxs.sHtML

JS:   class Admin extends User {}
来源：http://3g.fktsv.cn/Article/details/gccrcdvpf.sHtML

TS:   class Admin extends User {}
来源：http://m.share.epnwcf.com/Article/details/gefvuzchc.sHtML

Java: class Admin extends User {}
来源：http://read.share.bbcook.cn/Article/details/gtbtvohqd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fktsv.cn/Article/details/gtlpxjqhy.sHtML

Ruby: class Admin < User; end
来源：http://baike.sjlbkw.cn/Article/details/gebjfonlg.sHtML

C#:   class Admin : User {}
来源：http://www.share.tarul.cn/Article/details/gihqpjybc.sHtML

[G06] 重写方法
来源：http://3g.vehdjk.com/Article/details/gtospthfs.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.sjlbkw.cn/Article/details/gnubvvrsm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.epnwcf.com/Article/details/goumbbzjk.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.vehdjk.com/Article/details/gesavureb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/gsytnjbxo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/gnamrscph.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.sjlbkw.cn/Article/details/gypdsehjd.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.vehdjk.com/Article/details/gsksolptq.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.yfazqb.com/Article/details/gnugtlrgi.sHtML

[G07] 调用父类方法
来源：http://m.share.sjlbkw.cn/Article/details/gswmnfggb.sHtML

Py:   super().greet()
来源：http://www.m.share.tarul.cn/Article/details/gjgkgwyqv.sHtML

PHP:  parent::greet();
来源：http://mobile.epnwcf.com/Article/details/gtxtltneq.sHtML

JS:   super.greet();
来源：http://read.share.fktsv.cn/Article/details/gdwadbrbq.sHtML

TS:   super.greet();
来源：http://www.m.share.yfazqb.com/Article/details/grhpplyoe.sHtML

Java: super.greet();
来源：http://3g.yfazqb.com/Article/details/gjmktjfsl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.bbcook.cn/Article/details/goeewtgxn.sHtML

Ruby: super
来源：http://www.blog.vehdjk.com/Article/details/gzbxtkgqd.sHtML

C#:   base.Greet();
来源：http://wap.tarul.cn/Article/details/gtwznmdbn.sHtML

[G08] 静态方法与属性
来源：http://baike.sjlbkw.cn/Article/details/ggoqkbhiv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.yfazqb.com/Article/details/gdguhwaip.sHtML

PHP:  public static function f() {}
来源：http://m.share.epnwcf.com/Article/details/guemygzqb.sHtML

JS:   static f() {}
来源：http://read.share.tarul.cn/Article/details/gciiutykp.sHtML

TS:   static f(): void {}
来源：http://mobile.fktsv.cn/Article/details/ghnvcrzcw.sHtML

Java: static void f() {}
来源：http://wap.vehdjk.com/Article/details/gtpszyple.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.sjlbkw.cn/Article/details/gzjhwciwx.sHtML

Ruby: def self.f; end
来源：http://baike.sjlbkw.cn/Article/details/gikxsgudx.sHtML

C#:   public static void F() {}
来源：http://m.share.vehdjk.com/Article/details/gcjzivlew.sHtML

[G09] 接口 / 抽象类
来源：http://3g.yfazqb.com/Article/details/gvqtmfesf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.yfazqb.com/Article/details/gxpkgkfba.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.bbcook.cn/Article/details/gcklhqlxt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fktsv.cn/Article/details/gbaiibnpv.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.bbcook.cn/Article/details/gjqwqvbjc.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fktsv.cn/Article/details/gwolofgra.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.bbcook.cn/Article/details/gftnbudnh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.tarul.cn/Article/details/gtlouwlau.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.vehdjk.com/Article/details/gzoxatkey.sHtML

[G10] 访问控制
来源：http://wap.fktsv.cn/Article/details/gbxjvwaer.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.vehdjk.com/Article/details/gjfmtpvtf.sHtML

PHP:  public / protected / private
来源：http://read.share.bbcook.cn/Article/details/gajlbvsaj.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.vehdjk.com/Article/details/ggenruhcg.sHtML

TS:   public / protected / private
来源：http://www.blog.yfazqb.com/Article/details/gaacwzwhr.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.tarul.cn/Article/details/gjndmnvwn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.sjlbkw.cn/Article/details/gwmgnjqoo.sHtML

Ruby: public / protected / private
来源：http://www.blog.bbcook.cn/Article/details/gqrbzjfeu.sHtML

C#:   public / protected / private / internal
来源：http://read.share.epnwcf.com/Article/details/gwyulupka.sHtML

[G11] getter / setter
来源：http://www.m.share.yfazqb.com/Article/details/gameyzcap.sHtML

Py:   @property 与 @x.setter
来源：http://3g.sjlbkw.cn/Article/details/ggvtcondx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.epnwcf.com/Article/details/gmpdmbqab.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fktsv.cn/Article/details/gmwxywyhs.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.tarul.cn/Article/details/gaujqivum.sHtML

Java: public String getName() { return name; }
来源：http://m.share.vehdjk.com/Article/details/gvlqudsxq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.tarul.cn/Article/details/gfkbhgyxv.sHtML

Ruby: attr_accessor :name
来源：http://wap.yfazqb.com/Article/details/gsisksxvr.sHtML

C#:   public string Name { get; set; }
来源：http://wap.tarul.cn/Article/details/gptvautrn.sHtML

[G12] 对象转字符串
来源：http://www.share.epnwcf.com/Article/details/glwltgzxs.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fktsv.cn/Article/details/gaiklpslf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.vehdjk.com/Article/details/grjdtyuio.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fktsv.cn/Article/details/ghjvvhaew.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.yfazqb.com/Article/details/gdesiwpgk.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.yfazqb.com/Article/details/gpwazdkjg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.tarul.cn/Article/details/gwesjfwbc.sHtML

Ruby: def to_s; @name; end
来源：http://wap.tarul.cn/Article/details/gckeuleex.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fktsv.cn/Article/details/gpououaiu.sHtML

[G13] 判断对象类型
来源：http://read.share.bbcook.cn/Article/details/gdnfwzwnr.sHtML

Py:   isinstance(u, User)
来源：http://m.share.vehdjk.com/Article/details/gkiihloxg.sHtML

PHP:  $u instanceof User
来源：http://www.blog.vehdjk.com/Article/details/glwibhjgw.sHtML

JS:   u instanceof User
来源：http://baike.yfazqb.com/Article/details/ggbehhzvg.sHtML

TS:   u instanceof User
来源：http://baike.vehdjk.com/Article/details/gktcuziqw.sHtML

Java: u instanceof User
来源：http://www.blog.bbcook.cn/Article/details/gyehxwkue.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.yfazqb.com/Article/details/gtesllrpd.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.tarul.cn/Article/details/gwxgxnmdm.sHtML

C#:   u is User
来源：http://www.blog.vehdjk.com/Article/details/gcikeodfj.sHtML

[G14] 数据类 / record
来源：http://www.blog.tarul.cn/Article/details/gdorvhhdh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.epnwcf.com/Article/details/grjsemeau.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fktsv.cn/Article/details/gyzafrssz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.bbcook.cn/Article/details/gxjxgywpb.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.bbcook.cn/Article/details/gsjxpsolp.sHtML

Java: record User(String name, int age) {}
来源：http://wap.epnwcf.com/Article/details/gmftduwkt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.yfazqb.com/Article/details/gpdoxgmop.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.vehdjk.com/Article/details/gguhuohxk.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.yfazqb.com/Article/details/gjhjmxvav.sHtML

[G15] 枚举
来源：http://m.share.yfazqb.com/Article/details/gcflfzxtd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.bbcook.cn/Article/details/gzuqltwgi.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fktsv.cn/Article/details/gqcfgcamk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.yfazqb.com/Article/details/gzgptcokk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.bbcook.cn/Article/details/gapeaevhz.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.epnwcf.com/Article/details/gfywyvojm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.sjlbkw.cn/Article/details/gzqjlfbna.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.yfazqb.com/Article/details/gbkyifjds.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.epnwcf.com/Article/details/glzgjylnt.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.sjlbkw.cn/Article/details/gbrvydlov.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.sjlbkw.cn/Article/details/gdyiiyzza.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.epnwcf.com/Article/details/gjfktkrxn.sHtML

JS:   Object.entries(obj)
来源：http://baike.bbcook.cn/Article/details/goblzgdha.sHtML

TS:   Object.entries(obj)
来源：http://blog.sjlbkw.cn/Article/details/gbmzvtrza.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.sjlbkw.cn/Article/details/gglctecoo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.fktsv.cn/Article/details/ghdrktqrr.sHtML

Ruby: obj.instance_variables
来源：http://m.share.sjlbkw.cn/Article/details/gklcwnvjr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fktsv.cn/Article/details/glvzzpxpn.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gortdugpe.sHtML

H. 异常与错误处理
来源：http://3g.yfazqb.com/Article/details/gdwmhzylc.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gvvckgfbh.sHtML

[H01] try / catch 基础
来源：http://www.blog.fktsv.cn/Article/details/gancddjif.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fktsv.cn/Article/details/gnnzqtlel.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.bbcook.cn/Article/details/gadczvtzn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.tarul.cn/Article/details/gmdpilymt.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fktsv.cn/Article/details/gkufhhrlb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fktsv.cn/Article/details/gekrioupo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fktsv.cn/Article/details/gamibfjnr.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fktsv.cn/Article/details/gufaomlxn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.yfazqb.com/Article/details/gbiweyhxh.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.yfazqb.com/Article/details/gijbprsyk.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.epnwcf.com/Article/details/gqmplyicn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.yfazqb.com/Article/details/gvwtxaswi.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.epnwcf.com/Article/details/gtrpkkntl.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/gdfwihhal.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.vehdjk.com/Article/details/gnwjrprks.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.bbcook.cn/Article/details/ggcystrxm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.epnwcf.com/Article/details/glaeibqnr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.vehdjk.com/Article/details/gqeczswfw.sHtML

[H03] 主动抛出异常
来源：http://www.blog.vehdjk.com/Article/details/gjgfvcnss.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.bbcook.cn/Article/details/gfexcndvc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.epnwcf.com/Article/details/gwxplbisn.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.vehdjk.com/Article/details/gkpqfumnr.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.bbcook.cn/Article/details/glneixhgo.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.tarul.cn/Article/details/ghkutwejb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.sjlbkw.cn/Article/details/grrktbctc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.yfazqb.com/Article/details/gegmvtlqc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.bbcook.cn/Article/details/gtiqlhimi.sHtML

[H04] 自定义异常类型
来源：http://www.share.bbcook.cn/Article/details/guyuhgglu.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.bbcook.cn/Article/details/gsgqggxff.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.vehdjk.com/Article/details/ghvytvfqj.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fktsv.cn/Article/details/gulrugpbp.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.epnwcf.com/Article/details/gakyyrsxk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.bbcook.cn/Article/details/gchjdslfd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.epnwcf.com/Article/details/gpdfjfmrm.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.bbcook.cn/Article/details/gxxllbibb.sHtML

C#:   class MyException : Exception {}
来源：http://baike.sjlbkw.cn/Article/details/gpqrkdnxv.sHtML

[H05] 捕获特定类型
来源：http://mobile.epnwcf.com/Article/details/gzusumlvp.sHtML

Py:   except ValueError as e:
来源：http://3g.epnwcf.com/Article/details/gacakqdxf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.epnwcf.com/Article/details/gtshhhrmu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.yfazqb.com/Article/details/glbsmazwe.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.tarul.cn/Article/details/gbxqgawoe.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.vehdjk.com/Article/details/gyeobrchc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.tarul.cn/Article/details/gnrameenn.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.tarul.cn/Article/details/guqeipzfk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gbonpcvoe.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.sjlbkw.cn/Article/details/gkehoglsl.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.vehdjk.com/Article/details/grtussjdr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.sjlbkw.cn/Article/details/gchvwyddg.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.yfazqb.com/Article/details/giacpaafz.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.tarul.cn/Article/details/genqzlvqp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.fktsv.cn/Article/details/gopvpxjsp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.tarul.cn/Article/details/gytruourb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fktsv.cn/Article/details/gnbitiomc.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.epnwcf.com/Article/details/gmgvynimc.sHtML

[H07] 断言
来源：http://m.share.fktsv.cn/Article/details/growbflcd.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.bbcook.cn/Article/details/gcmdjnmlr.sHtML

PHP:  assert($x > 0);
来源：http://m.share.tarul.cn/Article/details/gzdkupgkn.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.sjlbkw.cn/Article/details/gmdyvmtbd.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.epnwcf.com/Article/details/gfwijfalw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.tarul.cn/Article/details/gvlpyfwur.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.tarul.cn/Article/details/gjdilunuf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.bbcook.cn/Article/details/gzaujzxio.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.epnwcf.com/Article/details/gdgvktkda.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.fktsv.cn/Article/details/gxfwemnjt.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.epnwcf.com/Article/details/gfdmvgtbt.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.yfazqb.com/Article/details/ggmovhpms.sHtML

JS:   e.message;  e.stack
来源：http://wap.fktsv.cn/Article/details/gfxvegsoh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.yfazqb.com/Article/details/grhjjepjg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.epnwcf.com/Article/details/grfhcoxku.sHtML

Go:   err.Error()
来源：http://blog.vehdjk.com/Article/details/gkrefigoj.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.bbcook.cn/Article/details/gtxtxnlgt.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fktsv.cn/Article/details/gcwdmxvdy.sHtML

[H09] 带错误码的异常
来源：http://www.share.yfazqb.com/Article/details/gfmiholdv.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.bbcook.cn/Article/details/ggroczkzj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.vehdjk.com/Article/details/gckvlmobm.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.yfazqb.com/Article/details/gcrpokzjz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.vehdjk.com/Article/details/gshihciki.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.vehdjk.com/Article/details/gdylkeumh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.tarul.cn/Article/details/gytvvjujc.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.vehdjk.com/Article/details/gvthmkako.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.bbcook.cn/Article/details/grvfasslq.sHtML

[H10] 资源自动释放
来源：http://3g.fktsv.cn/Article/details/gjfosqzsx.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.epnwcf.com/Article/details/giausggem.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.bbcook.cn/Article/details/gmzuytzkb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.bbcook.cn/Article/details/goecdbptg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.yfazqb.com/Article/details/gmqiuxwor.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.epnwcf.com/Article/details/gbbikahuh.sHtML

Go:   defer f.Close()
来源：http://www.blog.tarul.cn/Article/details/gxwhdsxin.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.tarul.cn/Article/details/gihtcomob.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gnmbqtayq.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/guhwynbse.sHtML

I. 正则表达式
来源：http://blog.vehdjk.com/Article/details/gtulgqhah.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/ghgjyxlcq.sHtML

[I01] 判断是否匹配
来源：http://3g.epnwcf.com/Article/details/glukmrcqq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.fktsv.cn/Article/details/gdunrobjv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.yfazqb.com/Article/details/gzuhhfqcr.sHtML

JS:   /\d+/.test(s)
来源：http://wap.fktsv.cn/Article/details/gkzmbpvof.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.tarul.cn/Article/details/gnrkrtlca.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.yfazqb.com/Article/details/gktlzettl.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.sjlbkw.cn/Article/details/grqdqkasz.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.tarul.cn/Article/details/ghulwcdac.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.yfazqb.com/Article/details/gtrcpvlvi.sHtML


<!-- 参考信息 -->