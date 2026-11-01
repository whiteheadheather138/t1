代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.epnwcf.com/Article/details/grizjnqdx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.yfazqb.com/Article/details/gormpleig.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.tarul.cn/Article/details/gdlxulhwk.sHtML

[F08] 遍历目录
来源：http://m.share.epnwcf.com/Article/details/giinxsdbv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.vehdjk.com/Article/details/galcphguw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.vehdjk.com/Article/details/goxhbewap.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.sjlbkw.cn/Article/details/gjyskfvnn.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fktsv.cn/Article/details/gkwvmufuz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.tarul.cn/Article/details/gcnrnkeoa.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.bbcook.cn/Article/details/grxoiekte.sHtML

Ruby: Dir.children("dir")
来源：http://baike.sjlbkw.cn/Article/details/gmbluloti.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fktsv.cn/Article/details/gaisznpnp.sHtML

[F09] 获取文件大小
来源：http://m.share.tarul.cn/Article/details/ggzlmajmx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gzdtdwuux.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gwhfsgtmp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.tarul.cn/Article/details/gtqjwkxpw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fktsv.cn/Article/details/gtezayxsr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.vehdjk.com/Article/details/gtspyguel.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fktsv.cn/Article/details/grfkphcch.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.bbcook.cn/Article/details/grxmlxmby.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.vehdjk.com/Article/details/gjqqihihm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.yfazqb.com/Article/details/ggbuhlmpg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.tarul.cn/Article/details/gzllhxrme.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.epnwcf.com/Article/details/ggvrfigwz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.bbcook.cn/Article/details/grtbilqgs.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gjexhgpus.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.yfazqb.com/Article/details/gciinsmcm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gsuckhoua.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/gnvwnulpw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gofnbwylb.sHtML

[F11] 复制与移动文件
来源：http://baike.tarul.cn/Article/details/gqelejmef.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/gamsxweup.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.tarul.cn/Article/details/ghphnrlig.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/grxizqxov.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/gvdqeqbka.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.vehdjk.com/Article/details/gclbqaiog.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.epnwcf.com/Article/details/gehnnydtw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.tarul.cn/Article/details/gnkjmkmuv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.fktsv.cn/Article/details/gzmlgxvtg.sHtML

[F12] CSV 读写
来源：http://www.share.tarul.cn/Article/details/gnsvrnaix.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.epnwcf.com/Article/details/gnrkfvdzs.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.vehdjk.com/Article/details/gocomahxy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.yfazqb.com/Article/details/gtfllefee.sHtML

TS:   // 同上
来源：http://read.share.fktsv.cn/Article/details/gmqodoiik.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fktsv.cn/Article/details/gggypxmet.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.vehdjk.com/Article/details/gxbozsahl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fktsv.cn/Article/details/gbfbdvnvd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.bbcook.cn/Article/details/gdextphxy.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gitpeprds.sHtML

G. 面向对象
来源：http://read.share.tarul.cn/Article/details/gjprqqkvf.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gqxfspcvv.sHtML

[G01] 定义类
来源：http://wap.sjlbkw.cn/Article/details/ggyljvshr.sHtML

Py:   class User: pass
来源：http://blog.bbcook.cn/Article/details/grzbkngaa.sHtML

PHP:  class User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/guqfhbpds.sHtML

JS:   class User {}
来源：http://wap.tarul.cn/Article/details/grvxlcgtt.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fktsv.cn/Article/details/gjsipbxvk.sHtML

Java: class User {}
来源：http://blog.yfazqb.com/Article/details/gmpiednno.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.tarul.cn/Article/details/gcqybrkuh.sHtML

Ruby: class User; end
来源：http://mobile.fktsv.cn/Article/details/gvvqlsaiz.sHtML

C#:   class User {}
来源：http://m.share.yfazqb.com/Article/details/grotddpgy.sHtML

[G02] 构造函数
来源：http://blog.tarul.cn/Article/details/gehbvkhvb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.sjlbkw.cn/Article/details/gauniifdu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.yfazqb.com/Article/details/gorydhvmq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.yfazqb.com/Article/details/ghgmcrtxc.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fktsv.cn/Article/details/gzyjddmam.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fktsv.cn/Article/details/gbakjynmm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.tarul.cn/Article/details/gveoaqjpm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.sjlbkw.cn/Article/details/gjxqcxyzl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.yfazqb.com/Article/details/gkbcisiyn.sHtML

[G03] 实例属性
来源：http://wap.vehdjk.com/Article/details/gtopxmreq.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fktsv.cn/Article/details/gyfkeoixm.sHtML

PHP:  public string $name = "x";
来源：http://3g.fktsv.cn/Article/details/gtgoljkip.sHtML

JS:   this.name = "x";
来源：http://mobile.sjlbkw.cn/Article/details/gvswmdkze.sHtML

TS:   name: string = "x";
来源：http://m.share.tarul.cn/Article/details/gaidxnjjx.sHtML

Java: private String name;
来源：http://www.share.bbcook.cn/Article/details/gtdqvjnne.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fktsv.cn/Article/details/gngytwxvz.sHtML

Ruby: @name = "x"
来源：http://3g.yfazqb.com/Article/details/gajaffxyn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.epnwcf.com/Article/details/gdcqyoenf.sHtML

[G04] 定义方法
来源：http://m.share.tarul.cn/Article/details/gukarodfq.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.yfazqb.com/Article/details/ghiunumwn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.bbcook.cn/Article/details/geqmtytqb.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fktsv.cn/Article/details/grgatnzwm.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.yfazqb.com/Article/details/gyfmwmvfy.sHtML

Java: String greet() { return name; }
来源：http://m.share.fktsv.cn/Article/details/giltgclqx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.epnwcf.com/Article/details/gbgkcthum.sHtML

Ruby: def greet; @name; end
来源：http://baike.bbcook.cn/Article/details/giiitqbkj.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.bbcook.cn/Article/details/gstaflguu.sHtML

[G05] 继承
来源：http://m.share.sjlbkw.cn/Article/details/gzljibtiw.sHtML

Py:   class Admin(User): pass
来源：http://baike.fktsv.cn/Article/details/gydrwvkiz.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fktsv.cn/Article/details/gonsgqqtg.sHtML

JS:   class Admin extends User {}
来源：http://mobile.vehdjk.com/Article/details/glczmhnwf.sHtML

TS:   class Admin extends User {}
来源：http://mobile.sjlbkw.cn/Article/details/gapxpfvea.sHtML

Java: class Admin extends User {}
来源：http://blog.yfazqb.com/Article/details/gzwlpapcr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.tarul.cn/Article/details/gwpnzzcsf.sHtML

Ruby: class Admin < User; end
来源：http://wap.epnwcf.com/Article/details/gervjbboq.sHtML

C#:   class Admin : User {}
来源：http://m.share.yfazqb.com/Article/details/gypwpfwjx.sHtML

[G06] 重写方法
来源：http://www.share.tarul.cn/Article/details/gsebswcmk.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.yfazqb.com/Article/details/gbuxrgbxr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/ghdmxdpuo.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fktsv.cn/Article/details/gletajhnw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.tarul.cn/Article/details/gdzvdghjj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.sjlbkw.cn/Article/details/geigxltam.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.yfazqb.com/Article/details/gsjljnasm.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.bbcook.cn/Article/details/geqqigtoo.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fktsv.cn/Article/details/gvabpdsqq.sHtML

[G07] 调用父类方法
来源：http://m.share.epnwcf.com/Article/details/gugwsjoan.sHtML

Py:   super().greet()
来源：http://mobile.bbcook.cn/Article/details/gjhgivurz.sHtML

PHP:  parent::greet();
来源：http://baike.epnwcf.com/Article/details/gucbqktbo.sHtML

JS:   super.greet();
来源：http://blog.epnwcf.com/Article/details/gpxhbiqsc.sHtML

TS:   super.greet();
来源：http://www.share.vehdjk.com/Article/details/gdxebewpx.sHtML

Java: super.greet();
来源：http://baike.fktsv.cn/Article/details/ggnfsrxba.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.bbcook.cn/Article/details/gfadakysq.sHtML

Ruby: super
来源：http://m.share.yfazqb.com/Article/details/gyygqewka.sHtML

C#:   base.Greet();
来源：http://www.blog.epnwcf.com/Article/details/gvgvlbnvo.sHtML

[G08] 静态方法与属性
来源：http://wap.bbcook.cn/Article/details/ghnubpftp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.bbcook.cn/Article/details/gjtxlkcqs.sHtML

PHP:  public static function f() {}
来源：http://blog.sjlbkw.cn/Article/details/gzlcqobrz.sHtML

JS:   static f() {}
来源：http://wap.yfazqb.com/Article/details/gkoufcklq.sHtML

TS:   static f(): void {}
来源：http://baike.fktsv.cn/Article/details/gzdnhrqtz.sHtML

Java: static void f() {}
来源：http://baike.vehdjk.com/Article/details/geumgxrac.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.vehdjk.com/Article/details/gsywpzcpm.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fktsv.cn/Article/details/gwyzhmcxi.sHtML

C#:   public static void F() {}
来源：http://mobile.bbcook.cn/Article/details/gatukhsat.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.epnwcf.com/Article/details/gjyounrft.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.yfazqb.com/Article/details/gbfwkpxgr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.tarul.cn/Article/details/ggoylgbka.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.vehdjk.com/Article/details/ggqorksgq.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.vehdjk.com/Article/details/ggnuhomix.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fktsv.cn/Article/details/gajzsaeqd.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.bbcook.cn/Article/details/gttbflgsp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fktsv.cn/Article/details/gvyjdgtac.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fktsv.cn/Article/details/gdhdhthto.sHtML

[G10] 访问控制
来源：http://www.share.bbcook.cn/Article/details/giynmwjhj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.vehdjk.com/Article/details/gaipyihwh.sHtML

PHP:  public / protected / private
来源：http://m.share.sjlbkw.cn/Article/details/gzomxapuk.sHtML

JS:   #private 字段；其余公开
来源：http://3g.epnwcf.com/Article/details/gqugzsrhl.sHtML

TS:   public / protected / private
来源：http://www.blog.fktsv.cn/Article/details/gmarygick.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.yfazqb.com/Article/details/gynnzhzgr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.tarul.cn/Article/details/gvxaqrehl.sHtML

Ruby: public / protected / private
来源：http://3g.tarul.cn/Article/details/gmckucmua.sHtML

C#:   public / protected / private / internal
来源：http://baike.vehdjk.com/Article/details/getrscwom.sHtML

[G11] getter / setter
来源：http://www.blog.bbcook.cn/Article/details/gtlhvdvjy.sHtML

Py:   @property 与 @x.setter
来源：http://baike.sjlbkw.cn/Article/details/gshvhcwpd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fktsv.cn/Article/details/gohetcboy.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.tarul.cn/Article/details/gkhbaiwhh.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.vehdjk.com/Article/details/gxnxdnsjs.sHtML

Java: public String getName() { return name; }
来源：http://blog.bbcook.cn/Article/details/gjixjqyrp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.bbcook.cn/Article/details/gdiukjwfp.sHtML

Ruby: attr_accessor :name
来源：http://baike.yfazqb.com/Article/details/gynwvswdi.sHtML

C#:   public string Name { get; set; }
来源：http://blog.tarul.cn/Article/details/gxkxockyt.sHtML

[G12] 对象转字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/guqqlpagb.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fktsv.cn/Article/details/gbcihwaob.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.sjlbkw.cn/Article/details/gccpywilz.sHtML

JS:   toString() { return this.name; }
来源：http://blog.yfazqb.com/Article/details/gfhmaiada.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.yfazqb.com/Article/details/grobicoxv.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.yfazqb.com/Article/details/gvtplclsn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.yfazqb.com/Article/details/gzmxxuequ.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fktsv.cn/Article/details/gsjljddfn.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.bbcook.cn/Article/details/gqfoncxdt.sHtML

[G13] 判断对象类型
来源：http://m.share.sjlbkw.cn/Article/details/gunekbuur.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.bbcook.cn/Article/details/gutuqfbtj.sHtML

PHP:  $u instanceof User
来源：http://baike.yfazqb.com/Article/details/gmzyrekvb.sHtML

JS:   u instanceof User
来源：http://3g.bbcook.cn/Article/details/ggewnacha.sHtML

TS:   u instanceof User
来源：http://mobile.sjlbkw.cn/Article/details/gmmoxlynh.sHtML

Java: u instanceof User
来源：http://mobile.yfazqb.com/Article/details/gxigoudpi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.vehdjk.com/Article/details/guhdwisac.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.yfazqb.com/Article/details/gysbjidvs.sHtML

C#:   u is User
来源：http://www.share.vehdjk.com/Article/details/gopswnisw.sHtML

[G14] 数据类 / record
来源：http://read.share.yfazqb.com/Article/details/gqdlhkqtc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.tarul.cn/Article/details/glfinwajh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.epnwcf.com/Article/details/gbrzobjzz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fktsv.cn/Article/details/gchwuhwfy.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.yfazqb.com/Article/details/gzudzbjjj.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fktsv.cn/Article/details/ggaxzkrzw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.epnwcf.com/Article/details/gnryvffcv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.tarul.cn/Article/details/givhojlur.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.bbcook.cn/Article/details/gtfyqyaho.sHtML

[G15] 枚举
来源：http://3g.vehdjk.com/Article/details/gsjavwxig.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.fktsv.cn/Article/details/gnftvonsk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.vehdjk.com/Article/details/glqcnhzqs.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.bbcook.cn/Article/details/gfxauecdi.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.tarul.cn/Article/details/gakqxwdyx.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.yfazqb.com/Article/details/grmanbphp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.bbcook.cn/Article/details/gdsfscvcx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.bbcook.cn/Article/details/gxnsfkwyv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.tarul.cn/Article/details/gliuifeqe.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.sjlbkw.cn/Article/details/gaodfsmfl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.tarul.cn/Article/details/gexfqsnim.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.epnwcf.com/Article/details/gqjbjkhpz.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.tarul.cn/Article/details/ggydkvfsy.sHtML

TS:   Object.entries(obj)
来源：http://m.share.bbcook.cn/Article/details/ghhlcoqfg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.bbcook.cn/Article/details/ghatuhlzo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.yfazqb.com/Article/details/gggxxecex.sHtML

Ruby: obj.instance_variables
来源：http://blog.tarul.cn/Article/details/ggmgrfpuq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.epnwcf.com/Article/details/gvczuaomk.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gtpdnofda.sHtML

H. 异常与错误处理
来源：http://blog.yfazqb.com/Article/details/gkuilcjao.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gevljczqr.sHtML

[H01] try / catch 基础
来源：http://3g.tarul.cn/Article/details/gufrvztkp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.vehdjk.com/Article/details/giyflfhlu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fktsv.cn/Article/details/gqfghasyy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.sjlbkw.cn/Article/details/gknnmmdbq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.yfazqb.com/Article/details/gacsaatla.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.bbcook.cn/Article/details/goakwsbad.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.vehdjk.com/Article/details/ggliczejv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.sjlbkw.cn/Article/details/gotlhcexx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.vehdjk.com/Article/details/gjmsvxiyo.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.sjlbkw.cn/Article/details/gnfwwtoru.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.bbcook.cn/Article/details/gsewzzppv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.epnwcf.com/Article/details/glfmdyfod.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/gtaqnpxqw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.tarul.cn/Article/details/gjwbdsvor.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.vehdjk.com/Article/details/gnwienbvw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.epnwcf.com/Article/details/gyqmihswj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.epnwcf.com/Article/details/gcwreprov.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/gieuavdiv.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.bbcook.cn/Article/details/gmhvpadyb.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.sjlbkw.cn/Article/details/gltrwjqlp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.yfazqb.com/Article/details/gaeqoppiz.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.epnwcf.com/Article/details/gntqnkjke.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fktsv.cn/Article/details/gndrnojel.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.sjlbkw.cn/Article/details/gwizchnck.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.tarul.cn/Article/details/girrrbyqc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.yfazqb.com/Article/details/glqjjiznt.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.bbcook.cn/Article/details/gtxeeaekp.sHtML

[H04] 自定义异常类型
来源：http://www.share.epnwcf.com/Article/details/gsvnecrfa.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fktsv.cn/Article/details/gognqyevr.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.sjlbkw.cn/Article/details/gdufwqwne.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.bbcook.cn/Article/details/gxntgoqxu.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.bbcook.cn/Article/details/girqgqxsh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.tarul.cn/Article/details/gnjcyjzbm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.epnwcf.com/Article/details/gxrehglom.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.bbcook.cn/Article/details/godqnimyp.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.vehdjk.com/Article/details/gzhmhkvqz.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.yfazqb.com/Article/details/grjycjmuu.sHtML

Py:   except ValueError as e:
来源：http://www.share.sjlbkw.cn/Article/details/gpxrqxrra.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.tarul.cn/Article/details/gjqbfsfns.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.fktsv.cn/Article/details/gjptfpskq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.bbcook.cn/Article/details/grclonauz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.yfazqb.com/Article/details/goftkiarb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.yfazqb.com/Article/details/gzpsiwvvq.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.vehdjk.com/Article/details/grvzjfftb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.vehdjk.com/Article/details/gzcvucbai.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.fktsv.cn/Article/details/gwknxtthg.sHtML

Py:   value = d.get("k") or default
来源：http://3g.fktsv.cn/Article/details/gdjljxhyr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.epnwcf.com/Article/details/gafdzngxz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.fktsv.cn/Article/details/gjvnqnjqo.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.bbcook.cn/Article/details/gyrxtpsiz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.vehdjk.com/Article/details/ggwhmczgi.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.yfazqb.com/Article/details/gfazzxect.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.vehdjk.com/Article/details/goylblrgt.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.bbcook.cn/Article/details/gyhvrboso.sHtML

[H07] 断言
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmzxlqzq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.sjlbkw.cn/Article/details/gclafelki.sHtML

PHP:  assert($x > 0);
来源：http://www.share.sjlbkw.cn/Article/details/glmuagwrg.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fktsv.cn/Article/details/ggareqacr.sHtML

TS:   console.assert(x > 0);
来源：http://3g.epnwcf.com/Article/details/gkrthharb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.vehdjk.com/Article/details/gmtjxwlod.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.yfazqb.com/Article/details/gitroesuq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.tarul.cn/Article/details/grirjzgqj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fktsv.cn/Article/details/gsreymbxi.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.yfazqb.com/Article/details/gurhgigan.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.sjlbkw.cn/Article/details/grzjppmxg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fktsv.cn/Article/details/gmumcsdmh.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fktsv.cn/Article/details/gwbarbhzd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.fktsv.cn/Article/details/gpdukrvtg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.epnwcf.com/Article/details/gshauqzwd.sHtML

Go:   err.Error()
来源：http://wap.bbcook.cn/Article/details/gzezfnyim.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.yfazqb.com/Article/details/girbueiyg.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.yfazqb.com/Article/details/grtvrguvw.sHtML

[H09] 带错误码的异常
来源：http://blog.tarul.cn/Article/details/gtuhsqnzz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.fktsv.cn/Article/details/gbmwijmil.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.tarul.cn/Article/details/gxjixewxf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.vehdjk.com/Article/details/gsxfzlehj.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.yfazqb.com/Article/details/gblytgdod.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.yfazqb.com/Article/details/gbjtqeslg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.yfazqb.com/Article/details/gcgevaacj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.vehdjk.com/Article/details/gzhqjbviu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.fktsv.cn/Article/details/gmljvyamw.sHtML

[H10] 资源自动释放
来源：http://baike.fktsv.cn/Article/details/gefqdhcsu.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.epnwcf.com/Article/details/gplvbrhzk.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.epnwcf.com/Article/details/gluhoxsms.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.epnwcf.com/Article/details/gxbfchfdl.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.sjlbkw.cn/Article/details/grkmubbvg.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.vehdjk.com/Article/details/gsksqwxhm.sHtML

Go:   defer f.Close()
来源：http://3g.fktsv.cn/Article/details/gedeyoimv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.epnwcf.com/Article/details/gesehxtoy.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gpdbyfmqn.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gkpqynnig.sHtML

I. 正则表达式
来源：http://read.share.fktsv.cn/Article/details/gcdwpvymh.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gttxlywgj.sHtML

[I01] 判断是否匹配
来源：http://www.share.epnwcf.com/Article/details/gfbetfmws.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.vehdjk.com/Article/details/gtvnwsjmb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.sjlbkw.cn/Article/details/grqsqkikf.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.vehdjk.com/Article/details/gswodwtxp.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.sjlbkw.cn/Article/details/ggmlncvdu.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.vehdjk.com/Article/details/gfdrmlkjd.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.fktsv.cn/Article/details/glzmuesrj.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.bbcook.cn/Article/details/gwubzxvur.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.sjlbkw.cn/Article/details/glncnzpgx.sHtML


<!-- 参考信息 -->