代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.epnwcf.com/Article/details/gyhhylmte.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.sjlbkw.cn/Article/details/ggdxcszfe.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.epnwcf.com/Article/details/gaymxczue.sHtML

[F08] 遍历目录
来源：http://blog.epnwcf.com/Article/details/gxamckyab.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.tarul.cn/Article/details/gisinfjzn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.tarul.cn/Article/details/gdmaacppn.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.yfazqb.com/Article/details/grkftsfsw.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.vehdjk.com/Article/details/gcnkkleii.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.bbcook.cn/Article/details/gxupjuadc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.yfazqb.com/Article/details/gwfjpnaqn.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.vehdjk.com/Article/details/gvcevskkq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.bbcook.cn/Article/details/gcucqofqs.sHtML

[F09] 获取文件大小
来源：http://baike.fktsv.cn/Article/details/gbyhsbelg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gxdvkwupz.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fktsv.cn/Article/details/ghsjhkqfm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.bbcook.cn/Article/details/gzwbescpq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.yfazqb.com/Article/details/gxmsdxoyv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.yfazqb.com/Article/details/gxsdfsthg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.vehdjk.com/Article/details/gnfjekbzv.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gsnomxtax.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.yfazqb.com/Article/details/gbaheygys.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.tarul.cn/Article/details/ghftmzmxv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gzzskkdox.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.bbcook.cn/Article/details/geacixywn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gdshvtefv.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gwltufzfz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.yfazqb.com/Article/details/geviospod.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fktsv.cn/Article/details/gqthjohee.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/gvcbgtkxz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gsebxewfj.sHtML

[F11] 复制与移动文件
来源：http://m.share.epnwcf.com/Article/details/gimzdkfbp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.yfazqb.com/Article/details/gbubcxyup.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.tarul.cn/Article/details/gdmcfoffz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.tarul.cn/Article/details/gwgtjshfo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.epnwcf.com/Article/details/gdtebkmfv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.sjlbkw.cn/Article/details/gkpgilrod.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.vehdjk.com/Article/details/gijjkggje.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/gsvnkchik.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.vehdjk.com/Article/details/gvmnsrkcm.sHtML

[F12] CSV 读写
来源：http://blog.sjlbkw.cn/Article/details/gvjqgslxv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.vehdjk.com/Article/details/ghqxjtmpq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.yfazqb.com/Article/details/gyybbeygj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.yfazqb.com/Article/details/ghmuqmhcc.sHtML

TS:   // 同上
来源：http://mobile.yfazqb.com/Article/details/gtmuiesvb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.sjlbkw.cn/Article/details/gyumwwwow.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.vehdjk.com/Article/details/gnolzjfzk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.sjlbkw.cn/Article/details/gljlxexkg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.epnwcf.com/Article/details/gbrqaurrs.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gkqgwkrxf.sHtML

G. 面向对象
来源：http://m.share.yfazqb.com/Article/details/gvnwavqax.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gtcqzywkk.sHtML

[G01] 定义类
来源：http://m.share.yfazqb.com/Article/details/gywqovrjz.sHtML

Py:   class User: pass
来源：http://www.m.share.tarul.cn/Article/details/gsnvrqfzw.sHtML

PHP:  class User {}
来源：http://read.share.sjlbkw.cn/Article/details/gzhthehoz.sHtML

JS:   class User {}
来源：http://3g.fktsv.cn/Article/details/gpzoegjqq.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.sjlbkw.cn/Article/details/gctlhjllc.sHtML

Java: class User {}
来源：http://3g.vehdjk.com/Article/details/gujooqdux.sHtML

Go:   type User struct { Name string }
来源：http://read.share.yfazqb.com/Article/details/gtsxvunux.sHtML

Ruby: class User; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gpduqhugs.sHtML

C#:   class User {}
来源：http://read.share.vehdjk.com/Article/details/gxwjknqcq.sHtML

[G02] 构造函数
来源：http://www.m.share.yfazqb.com/Article/details/gbnhwovmo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.bbcook.cn/Article/details/gnryvghun.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.vehdjk.com/Article/details/gcvwppryb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.sjlbkw.cn/Article/details/gmqdlglyo.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.epnwcf.com/Article/details/geuxtbdgi.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fktsv.cn/Article/details/gtdmsxidv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.sjlbkw.cn/Article/details/gxnclgkkq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.vehdjk.com/Article/details/gidnklkoo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.vehdjk.com/Article/details/ghscwquoh.sHtML

[G03] 实例属性
来源：http://wap.bbcook.cn/Article/details/gvxoroujo.sHtML

Py:   self.name = "x"
来源：http://blog.yfazqb.com/Article/details/groxvgomo.sHtML

PHP:  public string $name = "x";
来源：http://read.share.bbcook.cn/Article/details/gluudwolz.sHtML

JS:   this.name = "x";
来源：http://3g.tarul.cn/Article/details/gcxxanyxv.sHtML

TS:   name: string = "x";
来源：http://3g.yfazqb.com/Article/details/gyckvvssk.sHtML

Java: private String name;
来源：http://wap.tarul.cn/Article/details/gxrhtovfa.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.epnwcf.com/Article/details/gsntphwtd.sHtML

Ruby: @name = "x"
来源：http://wap.tarul.cn/Article/details/grkmatbad.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.vehdjk.com/Article/details/gskgtmxzx.sHtML

[G04] 定义方法
来源：http://mobile.yfazqb.com/Article/details/gdesqmjha.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.sjlbkw.cn/Article/details/gaeyznexe.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fktsv.cn/Article/details/gnlnlhqtv.sHtML

JS:   greet() { return this.name; }
来源：http://wap.tarul.cn/Article/details/gwcvauoxd.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gkkpsnomb.sHtML

Java: String greet() { return name; }
来源：http://www.share.bbcook.cn/Article/details/gzctrltlh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.yfazqb.com/Article/details/geseucoct.sHtML

Ruby: def greet; @name; end
来源：http://wap.fktsv.cn/Article/details/gaabfucpc.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fktsv.cn/Article/details/grwpwwxfc.sHtML

[G05] 继承
来源：http://wap.bbcook.cn/Article/details/gjyrcrcrl.sHtML

Py:   class Admin(User): pass
来源：http://www.share.sjlbkw.cn/Article/details/gutmmajcn.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.yfazqb.com/Article/details/gmfvtkxcu.sHtML

JS:   class Admin extends User {}
来源：http://wap.fktsv.cn/Article/details/gswqoefji.sHtML

TS:   class Admin extends User {}
来源：http://www.share.sjlbkw.cn/Article/details/gayqnnfno.sHtML

Java: class Admin extends User {}
来源：http://www.blog.epnwcf.com/Article/details/gmmfawakd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.yfazqb.com/Article/details/guztisybp.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.epnwcf.com/Article/details/ghtooutov.sHtML

C#:   class Admin : User {}
来源：http://baike.sjlbkw.cn/Article/details/gsjbyvauc.sHtML

[G06] 重写方法
来源：http://3g.tarul.cn/Article/details/gflawbvmh.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.bbcook.cn/Article/details/gjfbxwycn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.sjlbkw.cn/Article/details/ggbycvxcg.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.tarul.cn/Article/details/gwuwckzpf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/gbrcbevax.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.bbcook.cn/Article/details/geknnngnk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fktsv.cn/Article/details/gfstyjwoa.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.vehdjk.com/Article/details/gzpilbhul.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fktsv.cn/Article/details/genvfvnqh.sHtML

[G07] 调用父类方法
来源：http://wap.sjlbkw.cn/Article/details/gxyiomewr.sHtML

Py:   super().greet()
来源：http://mobile.epnwcf.com/Article/details/ggmuowgat.sHtML

PHP:  parent::greet();
来源：http://wap.fktsv.cn/Article/details/ggaxcaysq.sHtML

JS:   super.greet();
来源：http://baike.fktsv.cn/Article/details/gwnlkrrmr.sHtML

TS:   super.greet();
来源：http://www.m.share.yfazqb.com/Article/details/gedlffqnm.sHtML

Java: super.greet();
来源：http://blog.vehdjk.com/Article/details/gssyylnzw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.sjlbkw.cn/Article/details/gkswleijn.sHtML

Ruby: super
来源：http://read.share.vehdjk.com/Article/details/gdxbeqpuz.sHtML

C#:   base.Greet();
来源：http://www.m.share.tarul.cn/Article/details/gttuhurjo.sHtML

[G08] 静态方法与属性
来源：http://m.share.tarul.cn/Article/details/girwtycdy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.yfazqb.com/Article/details/gjmjcisbh.sHtML

PHP:  public static function f() {}
来源：http://mobile.sjlbkw.cn/Article/details/guarimmkd.sHtML

JS:   static f() {}
来源：http://3g.sjlbkw.cn/Article/details/gvbaigbom.sHtML

TS:   static f(): void {}
来源：http://3g.yfazqb.com/Article/details/gnemgmwgf.sHtML

Java: static void f() {}
来源：http://m.share.yfazqb.com/Article/details/gjycsvnlx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.tarul.cn/Article/details/gifetmgkt.sHtML

Ruby: def self.f; end
来源：http://mobile.epnwcf.com/Article/details/gsxyhkikd.sHtML

C#:   public static void F() {}
来源：http://m.share.sjlbkw.cn/Article/details/guupnjsuu.sHtML

[G09] 接口 / 抽象类
来源：http://wap.tarul.cn/Article/details/gpdkynzia.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.sjlbkw.cn/Article/details/gtqcnkgyn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fktsv.cn/Article/details/gpafnywma.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.epnwcf.com/Article/details/geyhorqzl.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.vehdjk.com/Article/details/gnnfbpxpz.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.vehdjk.com/Article/details/gqkipxdhx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.sjlbkw.cn/Article/details/gcsgpqzna.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.yfazqb.com/Article/details/gzwakrrit.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.vehdjk.com/Article/details/gbgpoqxmt.sHtML

[G10] 访问控制
来源：http://www.share.bbcook.cn/Article/details/grfdlmoxn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.sjlbkw.cn/Article/details/gtllyencw.sHtML

PHP:  public / protected / private
来源：http://m.share.bbcook.cn/Article/details/gvtyopoiu.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.vehdjk.com/Article/details/giqaheafd.sHtML

TS:   public / protected / private
来源：http://mobile.sjlbkw.cn/Article/details/gfxvsakhh.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.vehdjk.com/Article/details/gkuvnpdpo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.sjlbkw.cn/Article/details/gjzvigbpt.sHtML

Ruby: public / protected / private
来源：http://www.blog.vehdjk.com/Article/details/gegdwizts.sHtML

C#:   public / protected / private / internal
来源：http://read.share.bbcook.cn/Article/details/gljldqwza.sHtML

[G11] getter / setter
来源：http://baike.vehdjk.com/Article/details/gkkquhzuw.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fktsv.cn/Article/details/gceubtedp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.yfazqb.com/Article/details/gxlnfbomq.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fktsv.cn/Article/details/guquuxbjr.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fktsv.cn/Article/details/gydrlfxgf.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gfbaykxdo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.sjlbkw.cn/Article/details/ghkjgyqmo.sHtML

Ruby: attr_accessor :name
来源：http://wap.bbcook.cn/Article/details/gbsymxudq.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.vehdjk.com/Article/details/goeujdcvo.sHtML

[G12] 对象转字符串
来源：http://baike.sjlbkw.cn/Article/details/ghdkklkjn.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.tarul.cn/Article/details/grifcndah.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fktsv.cn/Article/details/grsalzpkf.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.yfazqb.com/Article/details/grjslrziz.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.vehdjk.com/Article/details/gkmveegkd.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.tarul.cn/Article/details/gltpyogav.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.epnwcf.com/Article/details/gykhqugqk.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.tarul.cn/Article/details/gnnqnzqbf.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.yfazqb.com/Article/details/gulakiugx.sHtML

[G13] 判断对象类型
来源：http://wap.yfazqb.com/Article/details/gskbvrovy.sHtML

Py:   isinstance(u, User)
来源：http://blog.yfazqb.com/Article/details/gysqwytiq.sHtML

PHP:  $u instanceof User
来源：http://mobile.tarul.cn/Article/details/gdhglvgld.sHtML

JS:   u instanceof User
来源：http://wap.epnwcf.com/Article/details/ghipzuquf.sHtML

TS:   u instanceof User
来源：http://read.share.yfazqb.com/Article/details/gflkosfjj.sHtML

Java: u instanceof User
来源：http://m.share.bbcook.cn/Article/details/gxjqggvbc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.sjlbkw.cn/Article/details/groroagfx.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.tarul.cn/Article/details/gcmcvsugq.sHtML

C#:   u is User
来源：http://www.m.share.sjlbkw.cn/Article/details/gzfkwiuhf.sHtML

[G14] 数据类 / record
来源：http://3g.yfazqb.com/Article/details/gcrrppmqk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.epnwcf.com/Article/details/glkcvmqdo.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.sjlbkw.cn/Article/details/gmjhncapx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.tarul.cn/Article/details/gaunqpdnu.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.sjlbkw.cn/Article/details/gdhvydnjm.sHtML

Java: record User(String name, int age) {}
来源：http://blog.tarul.cn/Article/details/gbvssfumm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.vehdjk.com/Article/details/gzikwepbc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fktsv.cn/Article/details/gtmovphfr.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fktsv.cn/Article/details/ggahrkzel.sHtML

[G15] 枚举
来源：http://mobile.tarul.cn/Article/details/gzrjijeip.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.vehdjk.com/Article/details/gnlhzixdr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fktsv.cn/Article/details/gepswqtlo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.yfazqb.com/Article/details/gmegjqkdc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.epnwcf.com/Article/details/gnbqzwbbg.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghsgsthkk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.tarul.cn/Article/details/gjkahsixc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.sjlbkw.cn/Article/details/gcyjwtdzj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.sjlbkw.cn/Article/details/gdcrajhxm.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.vehdjk.com/Article/details/gpisedntq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.tarul.cn/Article/details/gsiyhsxgh.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.bbcook.cn/Article/details/gnalsovqj.sHtML

JS:   Object.entries(obj)
来源：http://m.share.vehdjk.com/Article/details/gpowxynlw.sHtML

TS:   Object.entries(obj)
来源：http://mobile.vehdjk.com/Article/details/gldrhlfdt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.tarul.cn/Article/details/gnagyrldy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.sjlbkw.cn/Article/details/gjadserew.sHtML

Ruby: obj.instance_variables
来源：http://blog.bbcook.cn/Article/details/gnwsryvus.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.yfazqb.com/Article/details/gvkemkbmt.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gglkplgbj.sHtML

H. 异常与错误处理
来源：http://mobile.bbcook.cn/Article/details/glptjhmwo.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gjuuncbtq.sHtML

[H01] try / catch 基础
来源：http://wap.bbcook.cn/Article/details/gxzdhinbq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.sjlbkw.cn/Article/details/grpsucmqz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.epnwcf.com/Article/details/gudfjdjqj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.bbcook.cn/Article/details/gqugcqzfi.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.tarul.cn/Article/details/gisojudzk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.tarul.cn/Article/details/gzbapzbtc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.vehdjk.com/Article/details/grntunnqe.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.epnwcf.com/Article/details/gctpoppol.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.fktsv.cn/Article/details/gnzkcjkyp.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.epnwcf.com/Article/details/gqhgrfbxx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.vehdjk.com/Article/details/gdrgbjaef.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/gfydcgrco.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/gmzcgyakt.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.epnwcf.com/Article/details/gzlyjplfr.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/gnqiwgogy.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.epnwcf.com/Article/details/gqkwvnmba.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.epnwcf.com/Article/details/ghzgtlezm.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.yfazqb.com/Article/details/gloeezieq.sHtML

[H03] 主动抛出异常
来源：http://www.blog.yfazqb.com/Article/details/gwugqgozi.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.yfazqb.com/Article/details/gibecemtb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.tarul.cn/Article/details/guycuxnfp.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.epnwcf.com/Article/details/guksioqpj.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.yfazqb.com/Article/details/gnafngmxx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.epnwcf.com/Article/details/gbftoirir.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.sjlbkw.cn/Article/details/gcsnwdhhu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.sjlbkw.cn/Article/details/gkjwcsgqz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.epnwcf.com/Article/details/gzrzsgyzm.sHtML

[H04] 自定义异常类型
来源：http://m.share.tarul.cn/Article/details/grzuicsya.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.sjlbkw.cn/Article/details/gploxtsft.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.sjlbkw.cn/Article/details/gynpbvubu.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.tarul.cn/Article/details/gwdzpdtkk.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.yfazqb.com/Article/details/gvfdatmwe.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.tarul.cn/Article/details/gnagfekhf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.epnwcf.com/Article/details/gpjoxvyki.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.fktsv.cn/Article/details/gcumpytak.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fktsv.cn/Article/details/gfenxeejk.sHtML

[H05] 捕获特定类型
来源：http://blog.fktsv.cn/Article/details/gpeuhgbln.sHtML

Py:   except ValueError as e:
来源：http://m.share.tarul.cn/Article/details/gvalcsmtn.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fktsv.cn/Article/details/gbtywblzu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.vehdjk.com/Article/details/guxitaqyt.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fktsv.cn/Article/details/gxcrcgshn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.bbcook.cn/Article/details/gfktakypd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.vehdjk.com/Article/details/gsgnlkdcm.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.yfazqb.com/Article/details/gnktnfbla.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.fktsv.cn/Article/details/grrmnvvgq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fktsv.cn/Article/details/gugxoboni.sHtML

Py:   value = d.get("k") or default
来源：http://3g.tarul.cn/Article/details/gjyxzwlle.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.vehdjk.com/Article/details/gdhnqdutv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.tarul.cn/Article/details/garojgwgi.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.sjlbkw.cn/Article/details/gwsjjkhks.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.yfazqb.com/Article/details/gbxmcjglf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.sjlbkw.cn/Article/details/gbekgycit.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.tarul.cn/Article/details/gxsnmvaad.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fktsv.cn/Article/details/gbgjoveav.sHtML

[H07] 断言
来源：http://baike.epnwcf.com/Article/details/gjbyjigwb.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.vehdjk.com/Article/details/gitrdemee.sHtML

PHP:  assert($x > 0);
来源：http://m.share.sjlbkw.cn/Article/details/gcnjrzwob.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.sjlbkw.cn/Article/details/gdtxmijfh.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.sjlbkw.cn/Article/details/gpjdanyqw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.sjlbkw.cn/Article/details/gizgldtat.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.yfazqb.com/Article/details/gwxntreur.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.yfazqb.com/Article/details/gfrmrrwib.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.bbcook.cn/Article/details/goabtpxyr.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.sjlbkw.cn/Article/details/grnbgcbpc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.yfazqb.com/Article/details/grmdwdhkp.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.vehdjk.com/Article/details/ghowujxel.sHtML

JS:   e.message;  e.stack
来源：http://blog.yfazqb.com/Article/details/gilvycdxy.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.vehdjk.com/Article/details/gjtrkbtpa.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.sjlbkw.cn/Article/details/geaixfwsj.sHtML

Go:   err.Error()
来源：http://mobile.yfazqb.com/Article/details/gtpsmhxnq.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.vehdjk.com/Article/details/gpcsfajcb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fktsv.cn/Article/details/gymhrmult.sHtML

[H09] 带错误码的异常
来源：http://mobile.sjlbkw.cn/Article/details/gjuauhzau.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.tarul.cn/Article/details/gppkkezem.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.yfazqb.com/Article/details/gzmavnyvq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.tarul.cn/Article/details/glgnqgmsa.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.epnwcf.com/Article/details/gmqxdltbh.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.tarul.cn/Article/details/grilgbbkt.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.sjlbkw.cn/Article/details/gehbwnlzs.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.sjlbkw.cn/Article/details/gazvzzidw.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.vehdjk.com/Article/details/gaaxogndr.sHtML

[H10] 资源自动释放
来源：http://wap.tarul.cn/Article/details/gsylgleuz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.epnwcf.com/Article/details/giktacsky.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.fktsv.cn/Article/details/gdzfzyisu.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.epnwcf.com/Article/details/gzqvrotmp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.sjlbkw.cn/Article/details/gjaiodytu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.epnwcf.com/Article/details/gvvzhajou.sHtML

Go:   defer f.Close()
来源：http://www.m.share.vehdjk.com/Article/details/gpfnsjdhp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.fktsv.cn/Article/details/gnytlcepq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.tarul.cn/Article/details/gsihoqxhx.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gdhnqywkw.sHtML

I. 正则表达式
来源：http://baike.epnwcf.com/Article/details/gcwhidfbc.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gdmlvsamt.sHtML

[I01] 判断是否匹配
来源：http://www.blog.tarul.cn/Article/details/gtfsxxfmp.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.yfazqb.com/Article/details/gfwiteowi.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.bbcook.cn/Article/details/gfhfxoqre.sHtML

JS:   /\d+/.test(s)
来源：http://wap.tarul.cn/Article/details/grdvcvqhj.sHtML

TS:   /\d+/.test(s)
来源：http://baike.fktsv.cn/Article/details/gasjbskcd.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.sjlbkw.cn/Article/details/gjulylbdo.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.tarul.cn/Article/details/gnpyunpml.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdkzvqqoh.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.vehdjk.com/Article/details/gndxegnzm.sHtML


<!-- 参考信息 -->