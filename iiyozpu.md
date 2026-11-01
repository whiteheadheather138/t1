代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.sjlbkw.cn/Article/details/glxwlnsrp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.vehdjk.com/Article/details/gynsqccaz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fktsv.cn/Article/details/gglecvjla.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.vehdjk.com/Article/details/gvtgdujub.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.tarul.cn/Article/details/grtsifthz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.epnwcf.com/Article/details/ggpjklzus.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fktsv.cn/Article/details/glpczgttg.sHtML

[F08] 遍历目录
来源：http://www.share.sjlbkw.cn/Article/details/gplsaghjr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.vehdjk.com/Article/details/ghaeiejba.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.vehdjk.com/Article/details/gdzndapbd.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.vehdjk.com/Article/details/gscsxbuvp.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.yfazqb.com/Article/details/gxlvscepn.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fktsv.cn/Article/details/glgxrgnfs.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.epnwcf.com/Article/details/gltqfovwx.sHtML

Ruby: Dir.children("dir")
来源：http://baike.epnwcf.com/Article/details/gjftsnobk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.vehdjk.com/Article/details/gvwdaswed.sHtML

[F09] 获取文件大小
来源：http://read.share.epnwcf.com/Article/details/gupynczme.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.yfazqb.com/Article/details/guygplkdd.sHtML

PHP:  filesize("a.txt");
来源：http://3g.bbcook.cn/Article/details/gwunromvx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.epnwcf.com/Article/details/glhrzewln.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.bbcook.cn/Article/details/glssxivuq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.vehdjk.com/Article/details/gosstvlig.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fktsv.cn/Article/details/gpzpjsniy.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gxzdqkbll.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.tarul.cn/Article/details/gveekqxlk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.vehdjk.com/Article/details/gnychbkhd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/gigqkojdl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.vehdjk.com/Article/details/gmdpfwcnq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fktsv.cn/Article/details/ggsuldrzw.sHtML

TS:   path.extname("a.txt")
来源：http://blog.bbcook.cn/Article/details/gzpnlbmqg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.yfazqb.com/Article/details/gzjmvwdfl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gberopasl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/gkydeizsg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gmwrlfabj.sHtML

[F11] 复制与移动文件
来源：http://m.share.tarul.cn/Article/details/geybddyen.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.epnwcf.com/Article/details/gzduvaqpt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fktsv.cn/Article/details/gjpilhhke.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.yfazqb.com/Article/details/gwsmhvhsf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/gphwwqoze.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.epnwcf.com/Article/details/gvxcjgvrr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.bbcook.cn/Article/details/gdczmmfbz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gwzdsgorf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.sjlbkw.cn/Article/details/gucetreoc.sHtML

[F12] CSV 读写
来源：http://www.share.vehdjk.com/Article/details/gevztessw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.yfazqb.com/Article/details/gyvpgnrhc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.yfazqb.com/Article/details/gwhbkfdbv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.vehdjk.com/Article/details/gfxkmmtvs.sHtML

TS:   // 同上
来源：http://mobile.vehdjk.com/Article/details/ghaautiyt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.yfazqb.com/Article/details/gsxhfrpyx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.bbcook.cn/Article/details/gmwkdnegk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.tarul.cn/Article/details/gezpsuvwf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.sjlbkw.cn/Article/details/gnyzdwmrm.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gjcmacolb.sHtML

G. 面向对象
来源：http://blog.epnwcf.com/Article/details/giafarmqh.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gpzarbprr.sHtML

[G01] 定义类
来源：http://wap.vehdjk.com/Article/details/gcoitoicq.sHtML

Py:   class User: pass
来源：http://blog.tarul.cn/Article/details/gxbwkrvxf.sHtML

PHP:  class User {}
来源：http://read.share.sjlbkw.cn/Article/details/gxjyndoxz.sHtML

JS:   class User {}
来源：http://m.share.tarul.cn/Article/details/gawpxfobx.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.yfazqb.com/Article/details/grtwocflm.sHtML

Java: class User {}
来源：http://read.share.bbcook.cn/Article/details/gkbcpitdi.sHtML

Go:   type User struct { Name string }
来源：http://wap.epnwcf.com/Article/details/gnjruncqs.sHtML

Ruby: class User; end
来源：http://m.share.vehdjk.com/Article/details/gkiufswcz.sHtML

C#:   class User {}
来源：http://m.share.fktsv.cn/Article/details/gtjmkfrbk.sHtML

[G02] 构造函数
来源：http://www.blog.vehdjk.com/Article/details/gtwxowmpv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.epnwcf.com/Article/details/giosusamz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.sjlbkw.cn/Article/details/gwrutplox.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fktsv.cn/Article/details/gppynjoot.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fktsv.cn/Article/details/gihkyhjaq.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fktsv.cn/Article/details/gtldyuhaw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.tarul.cn/Article/details/gtvwewhgh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.tarul.cn/Article/details/giulnwepo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.tarul.cn/Article/details/gxflaabgw.sHtML

[G03] 实例属性
来源：http://blog.fktsv.cn/Article/details/gbgeevvay.sHtML

Py:   self.name = "x"
来源：http://baike.yfazqb.com/Article/details/gxmbculgx.sHtML

PHP:  public string $name = "x";
来源：http://www.share.epnwcf.com/Article/details/gmqzdphhx.sHtML

JS:   this.name = "x";
来源：http://baike.vehdjk.com/Article/details/gxwyzlyno.sHtML

TS:   name: string = "x";
来源：http://m.share.sjlbkw.cn/Article/details/gknyxxbes.sHtML

Java: private String name;
来源：http://www.blog.tarul.cn/Article/details/gwiiqljuw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fktsv.cn/Article/details/gnqwcpibw.sHtML

Ruby: @name = "x"
来源：http://mobile.epnwcf.com/Article/details/gtperiqjw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.bbcook.cn/Article/details/gfyjxxfiv.sHtML

[G04] 定义方法
来源：http://m.share.fktsv.cn/Article/details/guorwcspy.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.vehdjk.com/Article/details/ggrjbjgxa.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.epnwcf.com/Article/details/gubpzyidc.sHtML

JS:   greet() { return this.name; }
来源：http://baike.epnwcf.com/Article/details/ggyyfizjy.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.sjlbkw.cn/Article/details/giobwktgi.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gvsyasfmt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.tarul.cn/Article/details/gepagjovv.sHtML

Ruby: def greet; @name; end
来源：http://baike.vehdjk.com/Article/details/gjznjwvdk.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.tarul.cn/Article/details/gqdbvidna.sHtML

[G05] 继承
来源：http://blog.bbcook.cn/Article/details/gefvzikgf.sHtML

Py:   class Admin(User): pass
来源：http://wap.bbcook.cn/Article/details/gjgfpnqxg.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.bbcook.cn/Article/details/gzqsmuxwp.sHtML

JS:   class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/ggtjajlvv.sHtML

TS:   class Admin extends User {}
来源：http://www.share.vehdjk.com/Article/details/gljdnqkyj.sHtML

Java: class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/godfkvpxf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.yfazqb.com/Article/details/gjkbvohzb.sHtML

Ruby: class Admin < User; end
来源：http://baike.yfazqb.com/Article/details/glqggvnua.sHtML

C#:   class Admin : User {}
来源：http://baike.vehdjk.com/Article/details/gwnjgpulj.sHtML

[G06] 重写方法
来源：http://wap.vehdjk.com/Article/details/ghpvqsibh.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.bbcook.cn/Article/details/gzjrimteo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/govfcxdkm.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.yfazqb.com/Article/details/gqofcmgii.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.tarul.cn/Article/details/gzdusmhsv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.bbcook.cn/Article/details/gkeyspwgm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.epnwcf.com/Article/details/gimcgqhjs.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fktsv.cn/Article/details/gucaqxeyd.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.epnwcf.com/Article/details/gkqwdxkat.sHtML

[G07] 调用父类方法
来源：http://3g.sjlbkw.cn/Article/details/glaoomeze.sHtML

Py:   super().greet()
来源：http://read.share.sjlbkw.cn/Article/details/grhhdjmdh.sHtML

PHP:  parent::greet();
来源：http://wap.vehdjk.com/Article/details/gfeuvwllx.sHtML

JS:   super.greet();
来源：http://www.share.fktsv.cn/Article/details/gmntqvbjr.sHtML

TS:   super.greet();
来源：http://baike.epnwcf.com/Article/details/glvojmddb.sHtML

Java: super.greet();
来源：http://www.m.share.fktsv.cn/Article/details/geurhkaxe.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.bbcook.cn/Article/details/grxwuclhl.sHtML

Ruby: super
来源：http://www.m.share.fktsv.cn/Article/details/gyjhwdsqu.sHtML

C#:   base.Greet();
来源：http://blog.yfazqb.com/Article/details/gjjnkjgpq.sHtML

[G08] 静态方法与属性
来源：http://3g.epnwcf.com/Article/details/glehkbpkn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.sjlbkw.cn/Article/details/gzmxzfijr.sHtML

PHP:  public static function f() {}
来源：http://wap.yfazqb.com/Article/details/ggugxtopj.sHtML

JS:   static f() {}
来源：http://www.blog.epnwcf.com/Article/details/gfbktrzik.sHtML

TS:   static f(): void {}
来源：http://baike.tarul.cn/Article/details/gegxetsjj.sHtML

Java: static void f() {}
来源：http://www.m.share.epnwcf.com/Article/details/gumikpeuv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.yfazqb.com/Article/details/grwuisylc.sHtML

Ruby: def self.f; end
来源：http://m.share.bbcook.cn/Article/details/gwnjjmwoo.sHtML

C#:   public static void F() {}
来源：http://www.m.share.yfazqb.com/Article/details/gkjzphkzv.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fktsv.cn/Article/details/gwqwrqalh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.vehdjk.com/Article/details/gklwvlxau.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.tarul.cn/Article/details/gyjzanzrc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.epnwcf.com/Article/details/gbtcgnunj.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.epnwcf.com/Article/details/gzyiuevht.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzjfktbkn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.bbcook.cn/Article/details/gbkrrhubf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.yfazqb.com/Article/details/gxbwxjvfl.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.bbcook.cn/Article/details/gccnnlnsr.sHtML

[G10] 访问控制
来源：http://read.share.sjlbkw.cn/Article/details/gpqarjwtc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.epnwcf.com/Article/details/gduhihnmf.sHtML

PHP:  public / protected / private
来源：http://3g.sjlbkw.cn/Article/details/gschlyfrp.sHtML

JS:   #private 字段；其余公开
来源：http://wap.epnwcf.com/Article/details/gspcihmgo.sHtML

TS:   public / protected / private
来源：http://www.share.vehdjk.com/Article/details/ggkzbwkwg.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.vehdjk.com/Article/details/gjmoiahwd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fktsv.cn/Article/details/gijreeeou.sHtML

Ruby: public / protected / private
来源：http://mobile.vehdjk.com/Article/details/gevyjstiz.sHtML

C#:   public / protected / private / internal
来源：http://m.share.tarul.cn/Article/details/gvwvtlpsn.sHtML

[G11] getter / setter
来源：http://www.share.yfazqb.com/Article/details/ghsynqggd.sHtML

Py:   @property 与 @x.setter
来源：http://wap.tarul.cn/Article/details/gvrepsrag.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.vehdjk.com/Article/details/gzkjoxpeo.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.yfazqb.com/Article/details/ggupfnuia.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gkltrojup.sHtML

Java: public String getName() { return name; }
来源：http://mobile.epnwcf.com/Article/details/gxmvxzeby.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.epnwcf.com/Article/details/gclxjqhqs.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fktsv.cn/Article/details/gtsjhinza.sHtML

C#:   public string Name { get; set; }
来源：http://baike.vehdjk.com/Article/details/gfjvkbsbo.sHtML

[G12] 对象转字符串
来源：http://www.share.epnwcf.com/Article/details/gdyfsmabj.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.epnwcf.com/Article/details/ghygrrljp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.tarul.cn/Article/details/gnbtuthxb.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.tarul.cn/Article/details/giqxlavoh.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.sjlbkw.cn/Article/details/giptylhhq.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.bbcook.cn/Article/details/gfkqyldto.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.epnwcf.com/Article/details/gxheksadp.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.vehdjk.com/Article/details/gmsjstpap.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.epnwcf.com/Article/details/ghprtjvnb.sHtML

[G13] 判断对象类型
来源：http://blog.vehdjk.com/Article/details/gixkmguhk.sHtML

Py:   isinstance(u, User)
来源：http://blog.sjlbkw.cn/Article/details/gchsgfxrx.sHtML

PHP:  $u instanceof User
来源：http://m.share.sjlbkw.cn/Article/details/gcpyvhrll.sHtML

JS:   u instanceof User
来源：http://mobile.fktsv.cn/Article/details/gwsxdgjqh.sHtML

TS:   u instanceof User
来源：http://mobile.vehdjk.com/Article/details/goelpuksy.sHtML

Java: u instanceof User
来源：http://read.share.bbcook.cn/Article/details/gishfowxf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.sjlbkw.cn/Article/details/ggagiaavn.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fktsv.cn/Article/details/gkeifghgd.sHtML

C#:   u is User
来源：http://blog.tarul.cn/Article/details/grfggzebj.sHtML

[G14] 数据类 / record
来源：http://3g.bbcook.cn/Article/details/gxeuyqzuq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.tarul.cn/Article/details/gzqzvpmuh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.sjlbkw.cn/Article/details/gkbenadkk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.epnwcf.com/Article/details/gjlixqgps.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.yfazqb.com/Article/details/gcphdjics.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.tarul.cn/Article/details/gzkwdztce.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.bbcook.cn/Article/details/ghulqzrxg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.sjlbkw.cn/Article/details/grlgmvrpb.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.sjlbkw.cn/Article/details/gptdtsrhq.sHtML

[G15] 枚举
来源：http://www.m.share.vehdjk.com/Article/details/gwhnkcgnx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.sjlbkw.cn/Article/details/gbwkotcds.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.tarul.cn/Article/details/ghjhhznok.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.sjlbkw.cn/Article/details/gfakmbnqs.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.vehdjk.com/Article/details/gcwtohygm.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.epnwcf.com/Article/details/gqggtlvuz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.yfazqb.com/Article/details/gdkisgaqd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.yfazqb.com/Article/details/gdayzadrc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.vehdjk.com/Article/details/gfmmkqkmo.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.vehdjk.com/Article/details/gchfwnuxu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.bbcook.cn/Article/details/ghxpodowt.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.sjlbkw.cn/Article/details/gokngwpoq.sHtML

JS:   Object.entries(obj)
来源：http://read.share.epnwcf.com/Article/details/gczoqxajj.sHtML

TS:   Object.entries(obj)
来源：http://read.share.bbcook.cn/Article/details/gdjovwijp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.tarul.cn/Article/details/gnkwiiaiz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.epnwcf.com/Article/details/gxvovddbt.sHtML

Ruby: obj.instance_variables
来源：http://blog.fktsv.cn/Article/details/guniqaoal.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fktsv.cn/Article/details/ggmerwqlf.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gbezchoxc.sHtML

H. 异常与错误处理
来源：http://wap.tarul.cn/Article/details/gritdecqg.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gynoipgzl.sHtML

[H01] try / catch 基础
来源：http://www.share.epnwcf.com/Article/details/gfluqdjya.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.bbcook.cn/Article/details/gkinzdytc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.sjlbkw.cn/Article/details/glsremvtv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.tarul.cn/Article/details/gkgktbrdr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.bbcook.cn/Article/details/gvwdiizqu.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fktsv.cn/Article/details/gjrxmofan.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.vehdjk.com/Article/details/gfsbhuhmo.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.vehdjk.com/Article/details/gmpfkeish.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.bbcook.cn/Article/details/gqyxtrcsh.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.sjlbkw.cn/Article/details/gtepnabfn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.yfazqb.com/Article/details/gjhlxtxhl.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.vehdjk.com/Article/details/gdfafzges.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/glrrsmegv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.tarul.cn/Article/details/gazmevdul.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.epnwcf.com/Article/details/ghqfnicbs.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.yfazqb.com/Article/details/gjytnngze.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.sjlbkw.cn/Article/details/gjxabgobj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/giqlgyqiq.sHtML

[H03] 主动抛出异常
来源：http://www.share.vehdjk.com/Article/details/gjynldgsd.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.epnwcf.com/Article/details/gxsyomxzf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.bbcook.cn/Article/details/gloyoorxs.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.vehdjk.com/Article/details/gpvmbxcvc.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.tarul.cn/Article/details/gqmkxxuhs.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.bbcook.cn/Article/details/gmxhaglua.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.bbcook.cn/Article/details/gzgwqmdia.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.vehdjk.com/Article/details/gnaeoufqg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fktsv.cn/Article/details/gjlvrzdbh.sHtML

[H04] 自定义异常类型
来源：http://baike.vehdjk.com/Article/details/gxwdzzjvd.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.yfazqb.com/Article/details/grepvzchb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.tarul.cn/Article/details/gvmbdklsr.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.vehdjk.com/Article/details/glrjuooqk.sHtML

TS:   class MyError extends Error {}
来源：http://baike.epnwcf.com/Article/details/gsavnsyen.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.epnwcf.com/Article/details/gnlbitymw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fktsv.cn/Article/details/gubmkropc.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fktsv.cn/Article/details/ghpjcgcha.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.yfazqb.com/Article/details/gnfxhjipw.sHtML

[H05] 捕获特定类型
来源：http://3g.yfazqb.com/Article/details/gibfciafb.sHtML

Py:   except ValueError as e:
来源：http://read.share.vehdjk.com/Article/details/gywtapldb.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.bbcook.cn/Article/details/gdmnmrmoc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.bbcook.cn/Article/details/glgfajusk.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.epnwcf.com/Article/details/gjielmheo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.bbcook.cn/Article/details/giobgwgly.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fktsv.cn/Article/details/grxjmyojc.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.epnwcf.com/Article/details/gjtvnkdcx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.yfazqb.com/Article/details/goztdmghw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.sjlbkw.cn/Article/details/gothoqbkh.sHtML

Py:   value = d.get("k") or default
来源：http://3g.sjlbkw.cn/Article/details/gnnkdukva.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.yfazqb.com/Article/details/gxiynmwgq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.yfazqb.com/Article/details/gohmmwbpw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fktsv.cn/Article/details/goqbheumw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.bbcook.cn/Article/details/gnmbgxwex.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.sjlbkw.cn/Article/details/greusqfys.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.bbcook.cn/Article/details/gbeifqjnf.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.sjlbkw.cn/Article/details/gnclaohaz.sHtML

[H07] 断言
来源：http://read.share.bbcook.cn/Article/details/gyyyljhez.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.bbcook.cn/Article/details/ggtewxfyp.sHtML

PHP:  assert($x > 0);
来源：http://m.share.bbcook.cn/Article/details/gjrisdzgt.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.tarul.cn/Article/details/gfdhtshkm.sHtML

TS:   console.assert(x > 0);
来源：http://baike.vehdjk.com/Article/details/girhwtetv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.epnwcf.com/Article/details/gvtluwced.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.bbcook.cn/Article/details/gvupbqjtf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.yfazqb.com/Article/details/gxenqcoty.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.yfazqb.com/Article/details/gnmnmnlrh.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.bbcook.cn/Article/details/gqgempwwq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.sjlbkw.cn/Article/details/gqzcktbul.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.tarul.cn/Article/details/gkegghjdo.sHtML

JS:   e.message;  e.stack
来源：http://read.share.sjlbkw.cn/Article/details/gcbvnmlud.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.epnwcf.com/Article/details/goxwrisuv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.vehdjk.com/Article/details/gzosdcdvu.sHtML

Go:   err.Error()
来源：http://3g.yfazqb.com/Article/details/gsludaryc.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.epnwcf.com/Article/details/gjyrrbich.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.tarul.cn/Article/details/glfjdknii.sHtML

[H09] 带错误码的异常
来源：http://read.share.yfazqb.com/Article/details/gqhugwakt.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.sjlbkw.cn/Article/details/gftodpgvd.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.tarul.cn/Article/details/gyzggjwxm.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.fktsv.cn/Article/details/glxmsfzkr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.sjlbkw.cn/Article/details/gixvukaia.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.yfazqb.com/Article/details/godihlinw.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.bbcook.cn/Article/details/gxbapneaz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.bbcook.cn/Article/details/ggnlxijwj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.fktsv.cn/Article/details/gwhbobqjc.sHtML

[H10] 资源自动释放
来源：http://baike.tarul.cn/Article/details/gzbsaozxl.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.vehdjk.com/Article/details/gufyrfrcq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.tarul.cn/Article/details/gioqknejv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fktsv.cn/Article/details/gorflaflv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.tarul.cn/Article/details/gpynggtrp.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.tarul.cn/Article/details/gucneehhx.sHtML

Go:   defer f.Close()
来源：http://read.share.yfazqb.com/Article/details/gfbfcidxf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.tarul.cn/Article/details/gnpetuhjt.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gskcrrlmf.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gygpbnkhr.sHtML

I. 正则表达式
来源：http://www.share.fktsv.cn/Article/details/ggsxjcoyw.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gsjqyglcy.sHtML

[I01] 判断是否匹配
来源：http://3g.epnwcf.com/Article/details/gdapswzrb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.fktsv.cn/Article/details/givqqdxow.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.sjlbkw.cn/Article/details/gyqzgbkju.sHtML

JS:   /\d+/.test(s)
来源：http://3g.sjlbkw.cn/Article/details/ganplumdr.sHtML

TS:   /\d+/.test(s)
来源：http://wap.yfazqb.com/Article/details/gsirgrcze.sHtML


<!-- 参考信息 -->