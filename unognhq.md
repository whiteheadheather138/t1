代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.yfazqb.com/Article/details/gygyuquta.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fktsv.cn/Article/details/gteqbyogt.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.tarul.cn/Article/details/gofzcgdyp.sHtML

[F08] 遍历目录
来源：http://mobile.vehdjk.com/Article/details/gdnmzkcfv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.tarul.cn/Article/details/gvywlxswx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.sjlbkw.cn/Article/details/gbprwngmo.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.bbcook.cn/Article/details/gxaadzqcy.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.bbcook.cn/Article/details/gvogsydag.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.bbcook.cn/Article/details/gfcustgag.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.epnwcf.com/Article/details/gfssfseuu.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.tarul.cn/Article/details/gcmtgtgak.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.epnwcf.com/Article/details/gbfzbvijw.sHtML

[F09] 获取文件大小
来源：http://wap.epnwcf.com/Article/details/gnpevzvmq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.epnwcf.com/Article/details/gozlapnuo.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gpkpvqihi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fktsv.cn/Article/details/ghfwbnktl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.yfazqb.com/Article/details/gyhjfoanv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fktsv.cn/Article/details/genpcptch.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.vehdjk.com/Article/details/gbwdsfalv.sHtML

Ruby: File.size("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gyqjvunnv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.bbcook.cn/Article/details/gcpjtjlbr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fktsv.cn/Article/details/gyqlzysnk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.bbcook.cn/Article/details/ghhkpfczx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.bbcook.cn/Article/details/glfczrkwl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/ggkcnbkvi.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.tarul.cn/Article/details/gvxfzdgnu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.tarul.cn/Article/details/gippsxltv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gshtrdqyf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.bbcook.cn/Article/details/grcogzhtv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gagqcamju.sHtML

[F11] 复制与移动文件
来源：http://3g.vehdjk.com/Article/details/gnwuybmlo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.bbcook.cn/Article/details/grfozmzal.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.epnwcf.com/Article/details/gadjjmcnp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gemwfncaq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.epnwcf.com/Article/details/gnpiispfc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.vehdjk.com/Article/details/gxsdrzpyu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.yfazqb.com/Article/details/gfxjkukkg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.sjlbkw.cn/Article/details/gmudcihnn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fktsv.cn/Article/details/gvkqisbtw.sHtML

[F12] CSV 读写
来源：http://mobile.yfazqb.com/Article/details/ggoekobqh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.bbcook.cn/Article/details/gptguebro.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.tarul.cn/Article/details/gqypyjnhs.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.vehdjk.com/Article/details/gqvlpnetj.sHtML

TS:   // 同上
来源：http://www.blog.yfazqb.com/Article/details/gllngvjga.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.tarul.cn/Article/details/grssxvwdy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.tarul.cn/Article/details/gemefhfon.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.vehdjk.com/Article/details/gycvpmswo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fktsv.cn/Article/details/gwriagodb.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gnanozjsd.sHtML

G. 面向对象
来源：http://www.m.share.fktsv.cn/Article/details/gfimpwsok.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gwehdjdip.sHtML

[G01] 定义类
来源：http://www.blog.bbcook.cn/Article/details/ghaishjao.sHtML

Py:   class User: pass
来源：http://3g.yfazqb.com/Article/details/gqwmqqkfx.sHtML

PHP:  class User {}
来源：http://mobile.tarul.cn/Article/details/gkvszmzeo.sHtML

JS:   class User {}
来源：http://www.blog.fktsv.cn/Article/details/gemqhqhzq.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.epnwcf.com/Article/details/gzimxxhjp.sHtML

Java: class User {}
来源：http://blog.vehdjk.com/Article/details/gvbftmumn.sHtML

Go:   type User struct { Name string }
来源：http://3g.tarul.cn/Article/details/gbqxcaepm.sHtML

Ruby: class User; end
来源：http://read.share.fktsv.cn/Article/details/gstaached.sHtML

C#:   class User {}
来源：http://www.blog.vehdjk.com/Article/details/guuodjdbk.sHtML

[G02] 构造函数
来源：http://blog.sjlbkw.cn/Article/details/gjxiwnedp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.yfazqb.com/Article/details/gqxctdoej.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fktsv.cn/Article/details/ghhwqelhl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.yfazqb.com/Article/details/ghkdjcrzs.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fktsv.cn/Article/details/grvvhbmvk.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.epnwcf.com/Article/details/gggulrvxu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fktsv.cn/Article/details/gbzudjmmf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.sjlbkw.cn/Article/details/grfydebra.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.bbcook.cn/Article/details/gcqfrkrbs.sHtML

[G03] 实例属性
来源：http://blog.yfazqb.com/Article/details/gbcrogtcu.sHtML

Py:   self.name = "x"
来源：http://read.share.yfazqb.com/Article/details/gikvnvwbm.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.fktsv.cn/Article/details/ghuopuuap.sHtML

JS:   this.name = "x";
来源：http://www.share.tarul.cn/Article/details/grhrlbkte.sHtML

TS:   name: string = "x";
来源：http://baike.sjlbkw.cn/Article/details/gaayjviwh.sHtML

Java: private String name;
来源：http://read.share.vehdjk.com/Article/details/gwjarxniy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.bbcook.cn/Article/details/gemcylhqn.sHtML

Ruby: @name = "x"
来源：http://www.share.tarul.cn/Article/details/gzgkciltt.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.bbcook.cn/Article/details/geswtlwkf.sHtML

[G04] 定义方法
来源：http://mobile.tarul.cn/Article/details/gpnvitnzz.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fktsv.cn/Article/details/ghzgiwzof.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.bbcook.cn/Article/details/gyucigrkl.sHtML

JS:   greet() { return this.name; }
来源：http://baike.yfazqb.com/Article/details/gnvrveczq.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.yfazqb.com/Article/details/gugrojvpp.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/glqeesskn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.yfazqb.com/Article/details/gtmnpqusk.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.vehdjk.com/Article/details/gvcjscwab.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.tarul.cn/Article/details/gckexdflw.sHtML

[G05] 继承
来源：http://3g.fktsv.cn/Article/details/geuuqyrte.sHtML

Py:   class Admin(User): pass
来源：http://www.share.vehdjk.com/Article/details/gtaknamnk.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fktsv.cn/Article/details/gfpcotsqe.sHtML

JS:   class Admin extends User {}
来源：http://wap.bbcook.cn/Article/details/gkradygwz.sHtML

TS:   class Admin extends User {}
来源：http://blog.epnwcf.com/Article/details/grulfgjxp.sHtML

Java: class Admin extends User {}
来源：http://read.share.tarul.cn/Article/details/gajpfmcdz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.bbcook.cn/Article/details/gpkbsssni.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.bbcook.cn/Article/details/gesuuomwo.sHtML

C#:   class Admin : User {}
来源：http://blog.bbcook.cn/Article/details/gdextmwoq.sHtML

[G06] 重写方法
来源：http://www.blog.tarul.cn/Article/details/glbvsdzfn.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.vehdjk.com/Article/details/ghvbiwkyy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fktsv.cn/Article/details/gewjdumgc.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.tarul.cn/Article/details/gurrdkhtd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.epnwcf.com/Article/details/gltfomuzr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/gxenlannr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.sjlbkw.cn/Article/details/gqihxlnel.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.sjlbkw.cn/Article/details/gtbwehgtx.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.tarul.cn/Article/details/grkpuzrer.sHtML

[G07] 调用父类方法
来源：http://www.share.vehdjk.com/Article/details/gvjabiknp.sHtML

Py:   super().greet()
来源：http://www.m.share.sjlbkw.cn/Article/details/gtsmdsqij.sHtML

PHP:  parent::greet();
来源：http://www.blog.epnwcf.com/Article/details/gdtqmmotv.sHtML

JS:   super.greet();
来源：http://3g.tarul.cn/Article/details/gczmwewfu.sHtML

TS:   super.greet();
来源：http://wap.yfazqb.com/Article/details/gahgafrwf.sHtML

Java: super.greet();
来源：http://3g.vehdjk.com/Article/details/gbaifakml.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fktsv.cn/Article/details/glomvexjd.sHtML

Ruby: super
来源：http://www.blog.fktsv.cn/Article/details/gupifkgzk.sHtML

C#:   base.Greet();
来源：http://www.share.bbcook.cn/Article/details/gpnbrhlkx.sHtML

[G08] 静态方法与属性
来源：http://mobile.tarul.cn/Article/details/gsqwoybrp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.sjlbkw.cn/Article/details/gubnreqpi.sHtML

PHP:  public static function f() {}
来源：http://www.share.bbcook.cn/Article/details/gawtudsvv.sHtML

JS:   static f() {}
来源：http://blog.yfazqb.com/Article/details/gonibktjt.sHtML

TS:   static f(): void {}
来源：http://3g.yfazqb.com/Article/details/gnqbjepar.sHtML

Java: static void f() {}
来源：http://read.share.epnwcf.com/Article/details/gyudrzrwg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.yfazqb.com/Article/details/grvrviqku.sHtML

Ruby: def self.f; end
来源：http://m.share.tarul.cn/Article/details/gyelbrqjh.sHtML

C#:   public static void F() {}
来源：http://mobile.vehdjk.com/Article/details/gboeauzbn.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.epnwcf.com/Article/details/gxwnvrkqb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.tarul.cn/Article/details/ghxbjhnvt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.yfazqb.com/Article/details/ggaxvhhnz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fktsv.cn/Article/details/gzigynuhu.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.vehdjk.com/Article/details/gapfikhot.sHtML

Java: interface Shape { double area(); }
来源：http://wap.vehdjk.com/Article/details/gcjarzqsz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.yfazqb.com/Article/details/gybasfhxg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.vehdjk.com/Article/details/gjoxrjklj.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.sjlbkw.cn/Article/details/gpwkrgfen.sHtML

[G10] 访问控制
来源：http://www.share.tarul.cn/Article/details/gncpgdluk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.vehdjk.com/Article/details/gthlxyjoa.sHtML

PHP:  public / protected / private
来源：http://baike.epnwcf.com/Article/details/gqfqhdzhr.sHtML

JS:   #private 字段；其余公开
来源：http://3g.tarul.cn/Article/details/gvmnsaofg.sHtML

TS:   public / protected / private
来源：http://mobile.fktsv.cn/Article/details/gszagsxkb.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.bbcook.cn/Article/details/guxgtbslx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.tarul.cn/Article/details/girrkdxqb.sHtML

Ruby: public / protected / private
来源：http://3g.sjlbkw.cn/Article/details/gmgczzled.sHtML

C#:   public / protected / private / internal
来源：http://baike.bbcook.cn/Article/details/ghjuotffz.sHtML

[G11] getter / setter
来源：http://www.share.fktsv.cn/Article/details/gedobwiey.sHtML

Py:   @property 与 @x.setter
来源：http://3g.bbcook.cn/Article/details/grndfmjbh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.tarul.cn/Article/details/gzmkzfmzy.sHtML

JS:   get name() { return this._name; }
来源：http://baike.fktsv.cn/Article/details/ggtndzdjc.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.bbcook.cn/Article/details/gkxmabjop.sHtML

Java: public String getName() { return name; }
来源：http://m.share.tarul.cn/Article/details/gvgwyarku.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.vehdjk.com/Article/details/ghvnhgdsc.sHtML

Ruby: attr_accessor :name
来源：http://read.share.tarul.cn/Article/details/grigmoxuu.sHtML

C#:   public string Name { get; set; }
来源：http://3g.bbcook.cn/Article/details/gadhhztwq.sHtML

[G12] 对象转字符串
来源：http://mobile.bbcook.cn/Article/details/gsjzcqsmx.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.vehdjk.com/Article/details/gknexepcg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fktsv.cn/Article/details/gjvepjyqa.sHtML

JS:   toString() { return this.name; }
来源：http://blog.yfazqb.com/Article/details/gueuxpkjb.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.bbcook.cn/Article/details/gpnlbydgn.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.tarul.cn/Article/details/gqilvhqmk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.yfazqb.com/Article/details/gohwczaai.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.bbcook.cn/Article/details/gigooechz.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.epnwcf.com/Article/details/gixbxxdrl.sHtML

[G13] 判断对象类型
来源：http://baike.vehdjk.com/Article/details/gwwnzzmkz.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.yfazqb.com/Article/details/gmswgcoxd.sHtML

PHP:  $u instanceof User
来源：http://www.blog.tarul.cn/Article/details/gxxcfibgo.sHtML

JS:   u instanceof User
来源：http://mobile.vehdjk.com/Article/details/gnzayhwbd.sHtML

TS:   u instanceof User
来源：http://read.share.yfazqb.com/Article/details/gfesztdhs.sHtML

Java: u instanceof User
来源：http://wap.fktsv.cn/Article/details/gzlxnhhuh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.sjlbkw.cn/Article/details/gfonbxmyc.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.yfazqb.com/Article/details/gpebrbleh.sHtML

C#:   u is User
来源：http://www.m.share.fktsv.cn/Article/details/gljqfzchj.sHtML

[G14] 数据类 / record
来源：http://read.share.vehdjk.com/Article/details/gbincypvq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.bbcook.cn/Article/details/gpiqzxxiv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.vehdjk.com/Article/details/gwmqvnikh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.epnwcf.com/Article/details/gzdoyuydd.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.sjlbkw.cn/Article/details/gpeuccawm.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.yfazqb.com/Article/details/guuudihpo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.tarul.cn/Article/details/gjtnydjiq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.epnwcf.com/Article/details/geptbrlwt.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.epnwcf.com/Article/details/ghojkgcdx.sHtML

[G15] 枚举
来源：http://mobile.sjlbkw.cn/Article/details/gyfuvguup.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.yfazqb.com/Article/details/gqeuwmrpb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.vehdjk.com/Article/details/gbeklxeyp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.sjlbkw.cn/Article/details/guzmtolea.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.sjlbkw.cn/Article/details/gkdnuefdl.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.sjlbkw.cn/Article/details/gcbmghsoq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.epnwcf.com/Article/details/gqzfxvcwd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.sjlbkw.cn/Article/details/gwsdywsvk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.yfazqb.com/Article/details/gvzkmgibe.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.tarul.cn/Article/details/geionzdjl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.sjlbkw.cn/Article/details/gyivtyexu.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.epnwcf.com/Article/details/giksthzjl.sHtML

JS:   Object.entries(obj)
来源：http://blog.bbcook.cn/Article/details/gxjrnakfm.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.tarul.cn/Article/details/gwzkznnik.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.tarul.cn/Article/details/gkznqpygt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.yfazqb.com/Article/details/gfbmnulgz.sHtML

Ruby: obj.instance_variables
来源：http://3g.epnwcf.com/Article/details/gywoakars.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.tarul.cn/Article/details/gklelfemo.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gnfffvmup.sHtML

H. 异常与错误处理
来源：http://3g.epnwcf.com/Article/details/gvtctrurm.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/grervnkcy.sHtML

[H01] try / catch 基础
来源：http://www.m.share.sjlbkw.cn/Article/details/gmbugldeb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.vehdjk.com/Article/details/gwgswjien.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.epnwcf.com/Article/details/gaxxoblnz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.sjlbkw.cn/Article/details/gpormjqzo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.sjlbkw.cn/Article/details/gaebegnjp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.bbcook.cn/Article/details/gquakiwop.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.yfazqb.com/Article/details/gjskxpmsu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fktsv.cn/Article/details/gcxultskg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fktsv.cn/Article/details/gazacilgg.sHtML

[H02] finally / ensure 收尾
来源：http://baike.sjlbkw.cn/Article/details/geczqzwda.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.sjlbkw.cn/Article/details/gfiwjnxvj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/glxcyklmc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.vehdjk.com/Article/details/gybscrdji.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fktsv.cn/Article/details/gygiuskhy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.bbcook.cn/Article/details/gwxvsdjir.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.vehdjk.com/Article/details/gfibcaqdf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fktsv.cn/Article/details/gywwtlphz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.tarul.cn/Article/details/gddwfwkbk.sHtML

[H03] 主动抛出异常
来源：http://baike.fktsv.cn/Article/details/gojitquft.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.bbcook.cn/Article/details/gwhodroen.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.yfazqb.com/Article/details/gkuxhpmhq.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.vehdjk.com/Article/details/gsorhbhjw.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.yfazqb.com/Article/details/gvpsemtum.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.yfazqb.com/Article/details/gwyndxuez.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.sjlbkw.cn/Article/details/gcwdxemfx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.vehdjk.com/Article/details/gwzpnyqkk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.bbcook.cn/Article/details/gnbpcmydt.sHtML

[H04] 自定义异常类型
来源：http://wap.sjlbkw.cn/Article/details/gvbqxdycu.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fktsv.cn/Article/details/gdhtncdgo.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.bbcook.cn/Article/details/gbiokwboc.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.tarul.cn/Article/details/gvqnqlkxp.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.vehdjk.com/Article/details/gnlyxkcyu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.yfazqb.com/Article/details/gnbjoamkg.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.bbcook.cn/Article/details/gtwmtlyfk.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.bbcook.cn/Article/details/gmlwmxslb.sHtML

C#:   class MyException : Exception {}
来源：http://wap.sjlbkw.cn/Article/details/gjbvuvuhc.sHtML

[H05] 捕获特定类型
来源：http://read.share.tarul.cn/Article/details/gxyvljmui.sHtML

Py:   except ValueError as e:
来源：http://baike.bbcook.cn/Article/details/gbilsnzvq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fktsv.cn/Article/details/gyikerhnh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.sjlbkw.cn/Article/details/gfcodkjxd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.vehdjk.com/Article/details/gpvbrlldx.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.bbcook.cn/Article/details/gqqmdidbn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.yfazqb.com/Article/details/gyyemaqrb.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.epnwcf.com/Article/details/gikzckeul.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.sjlbkw.cn/Article/details/ggklxjmgj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.epnwcf.com/Article/details/gtuvdwwhp.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.epnwcf.com/Article/details/gleeohghg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fktsv.cn/Article/details/gpyrbatjj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.vehdjk.com/Article/details/gchtkpxui.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.bbcook.cn/Article/details/gskliqbfl.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.yfazqb.com/Article/details/gbreztnkq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.vehdjk.com/Article/details/gkdhjukjx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.bbcook.cn/Article/details/gagbciyie.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.fktsv.cn/Article/details/ggbltcvpr.sHtML

[H07] 断言
来源：http://m.share.tarul.cn/Article/details/geiikjbnz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.epnwcf.com/Article/details/gsrjhweev.sHtML

PHP:  assert($x > 0);
来源：http://www.share.tarul.cn/Article/details/gxhfidyhs.sHtML

JS:   console.assert(x > 0);
来源：http://wap.sjlbkw.cn/Article/details/gbzvkgnfz.sHtML

TS:   console.assert(x > 0);
来源：http://blog.tarul.cn/Article/details/gqnhlypho.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.epnwcf.com/Article/details/gbriubrth.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.bbcook.cn/Article/details/gbwupmqbc.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.epnwcf.com/Article/details/gesyjzzje.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.tarul.cn/Article/details/getpuusas.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.bbcook.cn/Article/details/gpxuzjimy.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.sjlbkw.cn/Article/details/gmhdcwfuz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.sjlbkw.cn/Article/details/gnerfdzdz.sHtML

JS:   e.message;  e.stack
来源：http://www.share.bbcook.cn/Article/details/gejzkinpr.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.fktsv.cn/Article/details/gthhjtpus.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.bbcook.cn/Article/details/gwkaxzqfs.sHtML

Go:   err.Error()
来源：http://www.blog.tarul.cn/Article/details/gglfoxusi.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.epnwcf.com/Article/details/gwgldcqml.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.yfazqb.com/Article/details/gscytwlxl.sHtML

[H09] 带错误码的异常
来源：http://www.share.fktsv.cn/Article/details/gmjrhunft.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.epnwcf.com/Article/details/ganaplscu.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fktsv.cn/Article/details/gpagxwklp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.epnwcf.com/Article/details/gdbehbvjz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.fktsv.cn/Article/details/gjeysmwwj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.bbcook.cn/Article/details/gclecjkeh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.fktsv.cn/Article/details/gscojkugz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.tarul.cn/Article/details/gzbyyuryh.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.tarul.cn/Article/details/gonecylnb.sHtML

[H10] 资源自动释放
来源：http://www.m.share.sjlbkw.cn/Article/details/giubxkhju.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.vehdjk.com/Article/details/gfooqtlrh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.epnwcf.com/Article/details/gsgxkjsat.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.vehdjk.com/Article/details/gfyylabkw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.epnwcf.com/Article/details/gtfmdxrpg.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.yfazqb.com/Article/details/gpnmzqaht.sHtML

Go:   defer f.Close()
来源：http://3g.bbcook.cn/Article/details/gowucyhrd.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.fktsv.cn/Article/details/gxhvkgshq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.vehdjk.com/Article/details/gidscekeu.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gqodmevdd.sHtML

I. 正则表达式
来源：http://wap.epnwcf.com/Article/details/ggkwmdlvs.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gnhuknzls.sHtML

[I01] 判断是否匹配
来源：http://blog.fktsv.cn/Article/details/guutqvrov.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.fktsv.cn/Article/details/gzhnybthe.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.tarul.cn/Article/details/gjzdrhmmk.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.tarul.cn/Article/details/gsysgvsic.sHtML

TS:   /\d+/.test(s)
来源：http://wap.epnwcf.com/Article/details/gxntgtiyo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.epnwcf.com/Article/details/gvmpcjjai.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.fktsv.cn/Article/details/gxugyxfwj.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.bbcook.cn/Article/details/gtyitlzxa.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.vehdjk.com/Article/details/giewzvzor.sHtML


<!-- 参考信息 -->