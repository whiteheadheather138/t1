代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gbinxfauz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gjxkeonjn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.epnwcf.com/Article/details/glfzbznel.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gitwbwdrm.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.vehdjk.com/Article/details/godfrgppa.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.vehdjk.com/Article/details/geidihjcu.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.epnwcf.com/Article/details/grtbpmdwh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.yfazqb.com/Article/details/geidhgkjv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.epnwcf.com/Article/details/gtficzhcc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fktsv.cn/Article/details/gssqzxxdi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.tarul.cn/Article/details/gxilmqxon.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.epnwcf.com/Article/details/gnmwcvvcq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.sjlbkw.cn/Article/details/gekfkvufe.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fktsv.cn/Article/details/gkhxmpgie.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.sjlbkw.cn/Article/details/gpfmtvmhm.sHtML

[F08] 遍历目录
来源：http://read.share.bbcook.cn/Article/details/gsnnwahox.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fktsv.cn/Article/details/gkwokpksi.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.yfazqb.com/Article/details/gzcvsnbdy.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/gbdplahuw.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fktsv.cn/Article/details/gkjcpawgi.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.tarul.cn/Article/details/gtsaceazs.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fktsv.cn/Article/details/geqayxkzl.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fktsv.cn/Article/details/ggewbdija.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.epnwcf.com/Article/details/gwbrqbagh.sHtML

[F09] 获取文件大小
来源：http://www.m.share.epnwcf.com/Article/details/grjuwnkza.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.yfazqb.com/Article/details/ghqfvcbuw.sHtML

PHP:  filesize("a.txt");
来源：http://3g.vehdjk.com/Article/details/gzwojerhl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.vehdjk.com/Article/details/gxjgscuvf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.sjlbkw.cn/Article/details/grggtyglk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.yfazqb.com/Article/details/gvihzbjtr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fktsv.cn/Article/details/gqlkgthmu.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gxiohmbnq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.sjlbkw.cn/Article/details/gsoavctst.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.sjlbkw.cn/Article/details/gqwlqbcoo.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/gafcrpmzm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.epnwcf.com/Article/details/gvsbdyepl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/gszibtthv.sHtML

TS:   path.extname("a.txt")
来源：http://3g.yfazqb.com/Article/details/gnkfvviql.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fktsv.cn/Article/details/gbkewulpf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.yfazqb.com/Article/details/gpcwmtxxj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gabhbdhzh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/glqvdxwye.sHtML

[F11] 复制与移动文件
来源：http://www.share.epnwcf.com/Article/details/gcwhyinix.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.tarul.cn/Article/details/grtjbnxxr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.tarul.cn/Article/details/giotxoxrs.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gixbybquo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.tarul.cn/Article/details/gcdnwdayz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.epnwcf.com/Article/details/ghwmhouzq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fktsv.cn/Article/details/glrsuuseh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.tarul.cn/Article/details/giguutpcj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.epnwcf.com/Article/details/gfmvgnwvp.sHtML

[F12] CSV 读写
来源：http://www.m.share.tarul.cn/Article/details/gyzuluwrr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.yfazqb.com/Article/details/giqnpcqpc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.tarul.cn/Article/details/gjqsrkkry.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.yfazqb.com/Article/details/ghhdrzjxh.sHtML

TS:   // 同上
来源：http://3g.vehdjk.com/Article/details/gscubolee.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.vehdjk.com/Article/details/gpkaltqqz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.bbcook.cn/Article/details/gllacnuzg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.bbcook.cn/Article/details/gdxehdaby.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.vehdjk.com/Article/details/gvgpkgxqo.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gysbpqios.sHtML

G. 面向对象
来源：http://m.share.tarul.cn/Article/details/ghnaccngn.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gvbvsevmu.sHtML

[G01] 定义类
来源：http://www.share.tarul.cn/Article/details/gmeekokia.sHtML

Py:   class User: pass
来源：http://3g.tarul.cn/Article/details/grenjxtrf.sHtML

PHP:  class User {}
来源：http://baike.bbcook.cn/Article/details/ggqelljuw.sHtML

JS:   class User {}
来源：http://read.share.yfazqb.com/Article/details/gxftxpxei.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.sjlbkw.cn/Article/details/gglzwycdg.sHtML

Java: class User {}
来源：http://baike.fktsv.cn/Article/details/ggftowgyi.sHtML

Go:   type User struct { Name string }
来源：http://wap.tarul.cn/Article/details/gdrlfsakr.sHtML

Ruby: class User; end
来源：http://www.m.share.fktsv.cn/Article/details/gsjglwnyp.sHtML

C#:   class User {}
来源：http://mobile.vehdjk.com/Article/details/gxlztdlij.sHtML

[G02] 构造函数
来源：http://3g.yfazqb.com/Article/details/gdytvgcow.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fktsv.cn/Article/details/gdahuibui.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fktsv.cn/Article/details/gulsfjara.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.bbcook.cn/Article/details/gbypirqdw.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.tarul.cn/Article/details/gmawtlqwe.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.epnwcf.com/Article/details/gmrjipgeg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.epnwcf.com/Article/details/girvewelw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.sjlbkw.cn/Article/details/gubdliqfb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.sjlbkw.cn/Article/details/glkvxturf.sHtML

[G03] 实例属性
来源：http://blog.yfazqb.com/Article/details/gmmrecgsd.sHtML

Py:   self.name = "x"
来源：http://mobile.vehdjk.com/Article/details/grhowouqf.sHtML

PHP:  public string $name = "x";
来源：http://blog.yfazqb.com/Article/details/gsnwofmye.sHtML

JS:   this.name = "x";
来源：http://mobile.yfazqb.com/Article/details/geichcnqp.sHtML

TS:   name: string = "x";
来源：http://m.share.yfazqb.com/Article/details/gyleqovxg.sHtML

Java: private String name;
来源：http://m.share.tarul.cn/Article/details/gvsbmivlq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fktsv.cn/Article/details/gdikvfjcq.sHtML

Ruby: @name = "x"
来源：http://www.m.share.vehdjk.com/Article/details/gbibiayqg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.sjlbkw.cn/Article/details/gqssaylpz.sHtML

[G04] 定义方法
来源：http://m.share.yfazqb.com/Article/details/gubwyssfx.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fktsv.cn/Article/details/gqsskvwsb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fktsv.cn/Article/details/giaxeyyes.sHtML

JS:   greet() { return this.name; }
来源：http://baike.sjlbkw.cn/Article/details/ggzfnpmjo.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.bbcook.cn/Article/details/guazodxcu.sHtML

Java: String greet() { return name; }
来源：http://www.share.epnwcf.com/Article/details/gpxmvnmuu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.yfazqb.com/Article/details/gzwjyprvw.sHtML

Ruby: def greet; @name; end
来源：http://baike.yfazqb.com/Article/details/gkdbdriqn.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.bbcook.cn/Article/details/gwbnazpfv.sHtML

[G05] 继承
来源：http://www.share.epnwcf.com/Article/details/gdtvftlxy.sHtML

Py:   class Admin(User): pass
来源：http://mobile.tarul.cn/Article/details/gwztwhdcv.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.sjlbkw.cn/Article/details/ggtmvaztt.sHtML

JS:   class Admin extends User {}
来源：http://wap.fktsv.cn/Article/details/gkmyoustg.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fktsv.cn/Article/details/gctzyfbsi.sHtML

Java: class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/gfbnczgwz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.bbcook.cn/Article/details/gjbddzhfj.sHtML

Ruby: class Admin < User; end
来源：http://www.share.vehdjk.com/Article/details/gfvcndvid.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.tarul.cn/Article/details/gyurupknv.sHtML

[G06] 重写方法
来源：http://www.share.sjlbkw.cn/Article/details/gctoxfwgr.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.yfazqb.com/Article/details/gddubomtu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.bbcook.cn/Article/details/gwuxawnci.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.vehdjk.com/Article/details/glgmbvxkp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.epnwcf.com/Article/details/gservxqyu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.bbcook.cn/Article/details/gyyzbodfl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.tarul.cn/Article/details/goqharmth.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.epnwcf.com/Article/details/gexheuqvn.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.epnwcf.com/Article/details/gwldzyfvu.sHtML

[G07] 调用父类方法
来源：http://wap.epnwcf.com/Article/details/gsbphmsrf.sHtML

Py:   super().greet()
来源：http://www.share.sjlbkw.cn/Article/details/glviijwvj.sHtML

PHP:  parent::greet();
来源：http://m.share.bbcook.cn/Article/details/gklsmoocw.sHtML

JS:   super.greet();
来源：http://wap.fktsv.cn/Article/details/gkkzzatsu.sHtML

TS:   super.greet();
来源：http://www.blog.bbcook.cn/Article/details/gslatiaqw.sHtML

Java: super.greet();
来源：http://mobile.sjlbkw.cn/Article/details/gwfdjxzbb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.tarul.cn/Article/details/gnsbsxdsd.sHtML

Ruby: super
来源：http://3g.sjlbkw.cn/Article/details/gvhtbxdbh.sHtML

C#:   base.Greet();
来源：http://baike.epnwcf.com/Article/details/gizyrryho.sHtML

[G08] 静态方法与属性
来源：http://mobile.bbcook.cn/Article/details/grjenzwde.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.sjlbkw.cn/Article/details/gpdgvzmqg.sHtML

PHP:  public static function f() {}
来源：http://3g.epnwcf.com/Article/details/gtwjemekl.sHtML

JS:   static f() {}
来源：http://www.blog.bbcook.cn/Article/details/gwsauskxt.sHtML

TS:   static f(): void {}
来源：http://blog.vehdjk.com/Article/details/gqlzjmmhv.sHtML

Java: static void f() {}
来源：http://www.blog.bbcook.cn/Article/details/gcsneiiln.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.sjlbkw.cn/Article/details/gplxgwjhj.sHtML

Ruby: def self.f; end
来源：http://wap.yfazqb.com/Article/details/gajvxgkbn.sHtML

C#:   public static void F() {}
来源：http://www.share.sjlbkw.cn/Article/details/gnjxipqqx.sHtML

[G09] 接口 / 抽象类
来源：http://3g.epnwcf.com/Article/details/glrfklbfc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.yfazqb.com/Article/details/guifidtac.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.sjlbkw.cn/Article/details/grabnfcli.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.yfazqb.com/Article/details/ggujmjagj.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fktsv.cn/Article/details/gbrkpivsr.sHtML

Java: interface Shape { double area(); }
来源：http://wap.vehdjk.com/Article/details/gumgwxcvg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.tarul.cn/Article/details/gkoojjkir.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.tarul.cn/Article/details/gzgropjrj.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.epnwcf.com/Article/details/gauuulmin.sHtML

[G10] 访问控制
来源：http://baike.vehdjk.com/Article/details/gcirlxnth.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.sjlbkw.cn/Article/details/ghpysoxjf.sHtML

PHP:  public / protected / private
来源：http://m.share.tarul.cn/Article/details/geziyrksd.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.tarul.cn/Article/details/gahnzzpfh.sHtML

TS:   public / protected / private
来源：http://baike.tarul.cn/Article/details/geswwmfvn.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.yfazqb.com/Article/details/gekkrokdm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.sjlbkw.cn/Article/details/gvumqfwxg.sHtML

Ruby: public / protected / private
来源：http://www.blog.sjlbkw.cn/Article/details/gzniarftn.sHtML

C#:   public / protected / private / internal
来源：http://www.share.tarul.cn/Article/details/godxblbhh.sHtML

[G11] getter / setter
来源：http://mobile.vehdjk.com/Article/details/gdqlzqomv.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.tarul.cn/Article/details/gaqinmueq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.bbcook.cn/Article/details/gplrsoani.sHtML

JS:   get name() { return this._name; }
来源：http://baike.tarul.cn/Article/details/guzgzkbyx.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.bbcook.cn/Article/details/gcrpqnfnq.sHtML

Java: public String getName() { return name; }
来源：http://blog.fktsv.cn/Article/details/gswlxqaas.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.yfazqb.com/Article/details/gbzhhpwuw.sHtML

Ruby: attr_accessor :name
来源：http://read.share.sjlbkw.cn/Article/details/gvongtixf.sHtML

C#:   public string Name { get; set; }
来源：http://wap.sjlbkw.cn/Article/details/gwunfuhrd.sHtML

[G12] 对象转字符串
来源：http://read.share.bbcook.cn/Article/details/gtkfijtti.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.sjlbkw.cn/Article/details/gmgyvfmnk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.yfazqb.com/Article/details/ghxxrtxbm.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.vehdjk.com/Article/details/gnvgljxzs.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.bbcook.cn/Article/details/gtdswdpbm.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gvwhlhbro.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.sjlbkw.cn/Article/details/gggrgnnmp.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.tarul.cn/Article/details/gtbwgtrcw.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.tarul.cn/Article/details/gceyjtxhc.sHtML

[G13] 判断对象类型
来源：http://www.m.share.vehdjk.com/Article/details/grojkkzcy.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.sjlbkw.cn/Article/details/gojcrnzth.sHtML

PHP:  $u instanceof User
来源：http://www.share.tarul.cn/Article/details/gfvmktwrb.sHtML

JS:   u instanceof User
来源：http://www.m.share.epnwcf.com/Article/details/gzaygkatb.sHtML

TS:   u instanceof User
来源：http://www.share.fktsv.cn/Article/details/gpndnqjxh.sHtML

Java: u instanceof User
来源：http://www.m.share.bbcook.cn/Article/details/guzkcobas.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.sjlbkw.cn/Article/details/gtmhpsdcf.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fktsv.cn/Article/details/gqpkiaqie.sHtML

C#:   u is User
来源：http://blog.sjlbkw.cn/Article/details/gniitnveb.sHtML

[G14] 数据类 / record
来源：http://3g.bbcook.cn/Article/details/gprwotcim.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.bbcook.cn/Article/details/gbllendaj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.bbcook.cn/Article/details/gjijvioxe.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.tarul.cn/Article/details/gpjpucwgn.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.yfazqb.com/Article/details/gnxpapuvz.sHtML

Java: record User(String name, int age) {}
来源：http://wap.vehdjk.com/Article/details/gadfyjzje.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.sjlbkw.cn/Article/details/gbatpfmbp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.yfazqb.com/Article/details/gtovvnhwp.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fktsv.cn/Article/details/guecmfqye.sHtML

[G15] 枚举
来源：http://read.share.sjlbkw.cn/Article/details/gjinbjeso.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.bbcook.cn/Article/details/gziwkfgcl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.epnwcf.com/Article/details/gjizgrcaz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.sjlbkw.cn/Article/details/gtfyeyokf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.sjlbkw.cn/Article/details/ggnbmdhvk.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.epnwcf.com/Article/details/gqpckmvab.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fktsv.cn/Article/details/ggznnrccr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fktsv.cn/Article/details/gxqzaliqs.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.yfazqb.com/Article/details/gntxwthae.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.tarul.cn/Article/details/gjoniuoff.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.vehdjk.com/Article/details/gigxgsqbe.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fktsv.cn/Article/details/gojhpxtio.sHtML

JS:   Object.entries(obj)
来源：http://read.share.bbcook.cn/Article/details/gefffmogk.sHtML

TS:   Object.entries(obj)
来源：http://read.share.vehdjk.com/Article/details/gohawcfel.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.yfazqb.com/Article/details/gmmdubyoh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.tarul.cn/Article/details/gkwqfuupz.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.epnwcf.com/Article/details/gyyfhkhvt.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.epnwcf.com/Article/details/gkyxfmbiy.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gmndeybmi.sHtML

H. 异常与错误处理
来源：http://baike.yfazqb.com/Article/details/gkacxvrpg.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/ggombonqg.sHtML

[H01] try / catch 基础
来源：http://baike.tarul.cn/Article/details/gtiflonql.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.epnwcf.com/Article/details/gricncpqh.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.epnwcf.com/Article/details/gepguglnf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.yfazqb.com/Article/details/gzlnwtwpl.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.bbcook.cn/Article/details/gzkcfmadg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fktsv.cn/Article/details/gohiziezx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.tarul.cn/Article/details/gykxijgct.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fktsv.cn/Article/details/gtmgsqaoi.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.bbcook.cn/Article/details/gxriazuiu.sHtML

[H02] finally / ensure 收尾
来源：http://baike.tarul.cn/Article/details/guobrhpct.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.sjlbkw.cn/Article/details/grxlrqrny.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fktsv.cn/Article/details/gkvnolxqk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.vehdjk.com/Article/details/gtvhqjrfz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.bbcook.cn/Article/details/gpxlmwgip.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.yfazqb.com/Article/details/gdkjnjfip.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.yfazqb.com/Article/details/gthevfgsk.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.bbcook.cn/Article/details/grutmipxr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.epnwcf.com/Article/details/gkmybiwrd.sHtML

[H03] 主动抛出异常
来源：http://www.blog.epnwcf.com/Article/details/gahbzvwgg.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.yfazqb.com/Article/details/gxkailqbp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.bbcook.cn/Article/details/gybtbwonm.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.vehdjk.com/Article/details/ggxrgypjo.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.bbcook.cn/Article/details/gulymqbse.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.sjlbkw.cn/Article/details/gmknaplin.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.bbcook.cn/Article/details/grfnsqmzm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.fktsv.cn/Article/details/gmryorhea.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.epnwcf.com/Article/details/gbibypwyz.sHtML

[H04] 自定义异常类型
来源：http://m.share.bbcook.cn/Article/details/gtrrbftos.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.vehdjk.com/Article/details/gentvnsza.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.tarul.cn/Article/details/gvntalegc.sHtML

JS:   class MyError extends Error {}
来源：http://blog.yfazqb.com/Article/details/gqbutlsyh.sHtML

TS:   class MyError extends Error {}
来源：http://baike.yfazqb.com/Article/details/gaznvsuaa.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.yfazqb.com/Article/details/gixzsloca.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.vehdjk.com/Article/details/gpwpekicu.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.epnwcf.com/Article/details/gyoldgqjj.sHtML

C#:   class MyException : Exception {}
来源：http://wap.bbcook.cn/Article/details/gymqjvizg.sHtML

[H05] 捕获特定类型
来源：http://www.blog.tarul.cn/Article/details/gtofbopru.sHtML

Py:   except ValueError as e:
来源：http://baike.tarul.cn/Article/details/gpizmnqze.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.sjlbkw.cn/Article/details/gqhqstvby.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.yfazqb.com/Article/details/gjlqtjghb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.tarul.cn/Article/details/gmwadujpa.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.yfazqb.com/Article/details/gpolroocn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.tarul.cn/Article/details/gbbrtemab.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.tarul.cn/Article/details/gqhzfycqq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.bbcook.cn/Article/details/gvaewrdzj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.yfazqb.com/Article/details/gjzqszrbm.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fktsv.cn/Article/details/ggbwfzspx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.sjlbkw.cn/Article/details/giwjjjfso.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.bbcook.cn/Article/details/gammcxuii.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.sjlbkw.cn/Article/details/ggihgrydu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.sjlbkw.cn/Article/details/gzouibynn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.fktsv.cn/Article/details/gacqisfsr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.bbcook.cn/Article/details/gfvyxzfzt.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.tarul.cn/Article/details/gzcxbvntw.sHtML

[H07] 断言
来源：http://www.m.share.bbcook.cn/Article/details/gisqwbduz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.yfazqb.com/Article/details/gozndmluf.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fktsv.cn/Article/details/gkmiqliqy.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.bbcook.cn/Article/details/gswyejryh.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.vehdjk.com/Article/details/gipwpmlwc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.yfazqb.com/Article/details/gzweyqzuw.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.bbcook.cn/Article/details/gaxnrplgp.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.bbcook.cn/Article/details/giglaggrz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.tarul.cn/Article/details/gxtkqvogx.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.fktsv.cn/Article/details/gqngxrdex.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.epnwcf.com/Article/details/gcatgtsdm.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.vehdjk.com/Article/details/gxwniyrmw.sHtML

JS:   e.message;  e.stack
来源：http://read.share.yfazqb.com/Article/details/gwgexrhqi.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.yfazqb.com/Article/details/gmwxxkfca.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.epnwcf.com/Article/details/gugqfmplt.sHtML

Go:   err.Error()
来源：http://www.blog.fktsv.cn/Article/details/gszuagpgj.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.epnwcf.com/Article/details/gsjfpuikc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.epnwcf.com/Article/details/grtlvuywv.sHtML

[H09] 带错误码的异常
来源：http://m.share.tarul.cn/Article/details/garnixzti.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.sjlbkw.cn/Article/details/gkqtnfekl.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.epnwcf.com/Article/details/gsdikxuqs.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.epnwcf.com/Article/details/glqzrydni.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.tarul.cn/Article/details/ggtjwddgd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.yfazqb.com/Article/details/ghjxthggl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.yfazqb.com/Article/details/gasnyzigf.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.bbcook.cn/Article/details/gwwgtkhqm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.epnwcf.com/Article/details/gaqyvluiw.sHtML

[H10] 资源自动释放
来源：http://mobile.yfazqb.com/Article/details/gjymuntuo.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.epnwcf.com/Article/details/gjfpsgsqp.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.fktsv.cn/Article/details/gfdgvdlvs.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.sjlbkw.cn/Article/details/gldfupwfj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.epnwcf.com/Article/details/glacyifdd.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.tarul.cn/Article/details/gsgzghoen.sHtML

Go:   defer f.Close()
来源：http://wap.vehdjk.com/Article/details/gijxrjugv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.sjlbkw.cn/Article/details/gayboaprz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.bbcook.cn/Article/details/gwjtmgemo.sHtML


<!-- 参考信息 -->