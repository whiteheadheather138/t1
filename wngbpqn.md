代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.epnwcf.com/Article/details/gpircyaug.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fktsv.cn/Article/details/gceudqalv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fktsv.cn/Article/details/giabhapxv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.epnwcf.com/Article/details/goivtodts.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.vehdjk.com/Article/details/gdgielnph.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.bbcook.cn/Article/details/gwthrerog.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fktsv.cn/Article/details/gtrhfadsd.sHtML

[F08] 遍历目录
来源：http://baike.vehdjk.com/Article/details/gcmqsvsuk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.yfazqb.com/Article/details/gfzsfcnzx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.sjlbkw.cn/Article/details/gsytilvqt.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.sjlbkw.cn/Article/details/giuxooedo.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.epnwcf.com/Article/details/glofahyab.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.vehdjk.com/Article/details/gcwumrayd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.vehdjk.com/Article/details/grtzuyrhk.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.yfazqb.com/Article/details/gqgrkppda.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.epnwcf.com/Article/details/guemreoaq.sHtML

[F09] 获取文件大小
来源：http://www.blog.fktsv.cn/Article/details/guztjbqox.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gtuevojbt.sHtML

PHP:  filesize("a.txt");
来源：http://3g.epnwcf.com/Article/details/gqslwxvyh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.epnwcf.com/Article/details/gyumxhpnn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fktsv.cn/Article/details/gqhkpkfkc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.sjlbkw.cn/Article/details/guwnozkjg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.epnwcf.com/Article/details/gqbvvxamt.sHtML

Ruby: File.size("a.txt")
来源：http://wap.bbcook.cn/Article/details/gnbfftwfh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.vehdjk.com/Article/details/gezdehgag.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fktsv.cn/Article/details/ghoqhxlaz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/gkbcdhvkf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.bbcook.cn/Article/details/ghdzzvtgz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.vehdjk.com/Article/details/ggcpaknqs.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/grsblecpm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.epnwcf.com/Article/details/gnsxjpliu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.yfazqb.com/Article/details/gvxamszdy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fktsv.cn/Article/details/gsuvktwpq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.tarul.cn/Article/details/gcarcyidp.sHtML

[F11] 复制与移动文件
来源：http://blog.bbcook.cn/Article/details/gaeqifyun.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.yfazqb.com/Article/details/gfhvraukh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gsfxnvpfa.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.tarul.cn/Article/details/gkdztljql.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.sjlbkw.cn/Article/details/gkrizptgt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.epnwcf.com/Article/details/ggfvygmiu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.vehdjk.com/Article/details/gtokvglju.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.vehdjk.com/Article/details/gmoghlwkj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.vehdjk.com/Article/details/garrqgtot.sHtML

[F12] CSV 读写
来源：http://mobile.fktsv.cn/Article/details/gwemqlcbs.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.yfazqb.com/Article/details/gryztzpmx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.sjlbkw.cn/Article/details/gcqvrxvvl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.bbcook.cn/Article/details/gojdhutvb.sHtML

TS:   // 同上
来源：http://www.blog.fktsv.cn/Article/details/gjmieggdz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.tarul.cn/Article/details/gpdkvkbtf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.bbcook.cn/Article/details/gtdwjobdc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fktsv.cn/Article/details/gcnodewwu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.vehdjk.com/Article/details/gtkzocaur.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/ghvkubxzt.sHtML

G. 面向对象
来源：http://www.blog.fktsv.cn/Article/details/gzgwfuvuo.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gflsesyuh.sHtML

[G01] 定义类
来源：http://www.blog.sjlbkw.cn/Article/details/gtyatzcsz.sHtML

Py:   class User: pass
来源：http://www.share.vehdjk.com/Article/details/gfuyywuvh.sHtML

PHP:  class User {}
来源：http://www.blog.tarul.cn/Article/details/gwspfuehx.sHtML

JS:   class User {}
来源：http://read.share.sjlbkw.cn/Article/details/gverzmlrf.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.yfazqb.com/Article/details/gfbpolrig.sHtML

Java: class User {}
来源：http://read.share.bbcook.cn/Article/details/gwsjlgevv.sHtML

Go:   type User struct { Name string }
来源：http://baike.tarul.cn/Article/details/gqwiigqyp.sHtML

Ruby: class User; end
来源：http://blog.sjlbkw.cn/Article/details/gmqhkstzq.sHtML

C#:   class User {}
来源：http://www.m.share.epnwcf.com/Article/details/gzkbcuxnj.sHtML

[G02] 构造函数
来源：http://www.m.share.yfazqb.com/Article/details/gddsgqawl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.vehdjk.com/Article/details/gmyzyyvmk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.sjlbkw.cn/Article/details/gjjpuwgch.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.vehdjk.com/Article/details/gagecmgqu.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.vehdjk.com/Article/details/guxkbrhyu.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.vehdjk.com/Article/details/gulzyxbvl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.bbcook.cn/Article/details/gmqsmffdh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fktsv.cn/Article/details/gztdbrlge.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.sjlbkw.cn/Article/details/gpuctbowy.sHtML

[G03] 实例属性
来源：http://www.blog.sjlbkw.cn/Article/details/gimrfwwac.sHtML

Py:   self.name = "x"
来源：http://www.share.sjlbkw.cn/Article/details/gztxmnwmw.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.yfazqb.com/Article/details/grlltoskz.sHtML

JS:   this.name = "x";
来源：http://baike.fktsv.cn/Article/details/gsqwjdssj.sHtML

TS:   name: string = "x";
来源：http://www.blog.epnwcf.com/Article/details/gsvbtqvgn.sHtML

Java: private String name;
来源：http://read.share.vehdjk.com/Article/details/gvdvtvbyk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.tarul.cn/Article/details/gjoslezuy.sHtML

Ruby: @name = "x"
来源：http://blog.epnwcf.com/Article/details/guknstfbz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.sjlbkw.cn/Article/details/gzbbktrvu.sHtML

[G04] 定义方法
来源：http://www.m.share.tarul.cn/Article/details/grenrdbhy.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.tarul.cn/Article/details/gjaeiiggd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.yfazqb.com/Article/details/gufmgixrv.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fktsv.cn/Article/details/gzgbcxryc.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.vehdjk.com/Article/details/gtmnbfeay.sHtML

Java: String greet() { return name; }
来源：http://www.share.tarul.cn/Article/details/gnlrvyukn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.epnwcf.com/Article/details/gzpmplfub.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.bbcook.cn/Article/details/gcehvpjnh.sHtML

C#:   public string Greet() => Name;
来源：http://3g.yfazqb.com/Article/details/gvcohxolh.sHtML

[G05] 继承
来源：http://m.share.epnwcf.com/Article/details/geetudzfe.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fktsv.cn/Article/details/gfwogqcso.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fktsv.cn/Article/details/gmrhtauel.sHtML

JS:   class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/gaeyguhff.sHtML

TS:   class Admin extends User {}
来源：http://wap.vehdjk.com/Article/details/gslvvhawa.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fktsv.cn/Article/details/gckjmpbhl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.bbcook.cn/Article/details/guisjzixn.sHtML

Ruby: class Admin < User; end
来源：http://www.share.yfazqb.com/Article/details/gnerlpxfc.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.bbcook.cn/Article/details/gzfyyjjmw.sHtML

[G06] 重写方法
来源：http://m.share.tarul.cn/Article/details/gtzbhnyxv.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.sjlbkw.cn/Article/details/govhzjoeh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.tarul.cn/Article/details/gqmqbwyut.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.vehdjk.com/Article/details/gsikslvdg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.bbcook.cn/Article/details/gccasyzwc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.vehdjk.com/Article/details/gcbvdckyk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.tarul.cn/Article/details/gziaqogvm.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.epnwcf.com/Article/details/gzdzwwejk.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.tarul.cn/Article/details/gwaegtprf.sHtML

[G07] 调用父类方法
来源：http://blog.yfazqb.com/Article/details/gcurrxawz.sHtML

Py:   super().greet()
来源：http://www.share.tarul.cn/Article/details/gbyxisair.sHtML

PHP:  parent::greet();
来源：http://www.blog.yfazqb.com/Article/details/guuppocix.sHtML

JS:   super.greet();
来源：http://www.m.share.bbcook.cn/Article/details/gucqtgrrj.sHtML

TS:   super.greet();
来源：http://wap.yfazqb.com/Article/details/gzztozjdw.sHtML

Java: super.greet();
来源：http://www.share.tarul.cn/Article/details/gfhuvckyq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.vehdjk.com/Article/details/gspfphwff.sHtML

Ruby: super
来源：http://blog.epnwcf.com/Article/details/gjxrbaiqk.sHtML

C#:   base.Greet();
来源：http://3g.yfazqb.com/Article/details/gbdlyjklq.sHtML

[G08] 静态方法与属性
来源：http://www.share.epnwcf.com/Article/details/gtqzddznx.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.epnwcf.com/Article/details/gdnhczhrk.sHtML

PHP:  public static function f() {}
来源：http://baike.bbcook.cn/Article/details/gzlgmkjqx.sHtML

JS:   static f() {}
来源：http://3g.vehdjk.com/Article/details/gpfqizpup.sHtML

TS:   static f(): void {}
来源：http://www.share.yfazqb.com/Article/details/ggirlhlut.sHtML

Java: static void f() {}
来源：http://blog.yfazqb.com/Article/details/gqpflzwtq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.tarul.cn/Article/details/gnhqneemz.sHtML

Ruby: def self.f; end
来源：http://www.share.sjlbkw.cn/Article/details/gepryslnb.sHtML

C#:   public static void F() {}
来源：http://www.blog.fktsv.cn/Article/details/gznqrvcui.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.vehdjk.com/Article/details/gpxxfbddd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.sjlbkw.cn/Article/details/gfnraijlr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fktsv.cn/Article/details/ghnsrgihc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.tarul.cn/Article/details/gmungfusi.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.yfazqb.com/Article/details/gmamvkhvz.sHtML

Java: interface Shape { double area(); }
来源：http://3g.epnwcf.com/Article/details/ggaeacczv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.bbcook.cn/Article/details/gfeftmyyc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.epnwcf.com/Article/details/gksxffhzx.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.vehdjk.com/Article/details/gkjgbrvsp.sHtML

[G10] 访问控制
来源：http://www.share.yfazqb.com/Article/details/grxepeqxa.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.epnwcf.com/Article/details/gagdwzkct.sHtML

PHP:  public / protected / private
来源：http://blog.fktsv.cn/Article/details/gbepdflss.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.yfazqb.com/Article/details/gyjknudyg.sHtML

TS:   public / protected / private
来源：http://www.m.share.fktsv.cn/Article/details/gahtzqvwc.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.epnwcf.com/Article/details/gkbzrituz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.yfazqb.com/Article/details/gncrsdvog.sHtML

Ruby: public / protected / private
来源：http://mobile.epnwcf.com/Article/details/golznzsfo.sHtML

C#:   public / protected / private / internal
来源：http://baike.tarul.cn/Article/details/gnnngxymv.sHtML

[G11] getter / setter
来源：http://baike.yfazqb.com/Article/details/gsrmoqlys.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.vehdjk.com/Article/details/gjxleibhv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.tarul.cn/Article/details/gyiahavws.sHtML

JS:   get name() { return this._name; }
来源：http://wap.tarul.cn/Article/details/gzqtkkbnj.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.epnwcf.com/Article/details/gtohmirhe.sHtML

Java: public String getName() { return name; }
来源：http://www.share.epnwcf.com/Article/details/gvkwhjart.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.epnwcf.com/Article/details/gqywvvyzm.sHtML

Ruby: attr_accessor :name
来源：http://m.share.vehdjk.com/Article/details/gifhzncmu.sHtML

C#:   public string Name { get; set; }
来源：http://blog.tarul.cn/Article/details/gftbrutqq.sHtML

[G12] 对象转字符串
来源：http://3g.vehdjk.com/Article/details/gmykqunsx.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.yfazqb.com/Article/details/gbipptszp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fktsv.cn/Article/details/guhavbyhy.sHtML

JS:   toString() { return this.name; }
来源：http://wap.vehdjk.com/Article/details/golfvuxxq.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.yfazqb.com/Article/details/gbqvumcdr.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.epnwcf.com/Article/details/gqdceydnh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.vehdjk.com/Article/details/gnyntcwjt.sHtML

Ruby: def to_s; @name; end
来源：http://wap.epnwcf.com/Article/details/gltbguffv.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.epnwcf.com/Article/details/ghescjfuz.sHtML

[G13] 判断对象类型
来源：http://m.share.sjlbkw.cn/Article/details/gewwscvjv.sHtML

Py:   isinstance(u, User)
来源：http://3g.yfazqb.com/Article/details/gszrgdvxy.sHtML

PHP:  $u instanceof User
来源：http://read.share.epnwcf.com/Article/details/gndryerdk.sHtML

JS:   u instanceof User
来源：http://www.blog.tarul.cn/Article/details/glfjiwgvx.sHtML

TS:   u instanceof User
来源：http://mobile.vehdjk.com/Article/details/grgwopnuv.sHtML

Java: u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/ggrfghzld.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.tarul.cn/Article/details/gfoivvzba.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fktsv.cn/Article/details/ggkbrobzi.sHtML

C#:   u is User
来源：http://mobile.bbcook.cn/Article/details/gsmhdnjuu.sHtML

[G14] 数据类 / record
来源：http://m.share.epnwcf.com/Article/details/glxvxisud.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.epnwcf.com/Article/details/gjxlqtflg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.bbcook.cn/Article/details/gtfnbqozj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.yfazqb.com/Article/details/gjwgbjwls.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.yfazqb.com/Article/details/giyttbxvg.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.yfazqb.com/Article/details/gyhvoxhxh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.sjlbkw.cn/Article/details/gcshmykrq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.tarul.cn/Article/details/ghsjbysxh.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.vehdjk.com/Article/details/gixjivzfh.sHtML

[G15] 枚举
来源：http://m.share.vehdjk.com/Article/details/giqkniuui.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.sjlbkw.cn/Article/details/ggsmezyhj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.sjlbkw.cn/Article/details/gqxxcufpu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.bbcook.cn/Article/details/gdgskrngv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fktsv.cn/Article/details/gezqllngg.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.yfazqb.com/Article/details/gtiofbplr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.bbcook.cn/Article/details/gibpmfvur.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.bbcook.cn/Article/details/gyjzvqdaz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.sjlbkw.cn/Article/details/gdzfoorvs.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.bbcook.cn/Article/details/grfdijwng.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fktsv.cn/Article/details/glkytlobh.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fktsv.cn/Article/details/ganjxxagn.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gwkhoqyot.sHtML

TS:   Object.entries(obj)
来源：http://wap.tarul.cn/Article/details/gechqwddm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.epnwcf.com/Article/details/gvoueocaw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.bbcook.cn/Article/details/gyulvyfse.sHtML

Ruby: obj.instance_variables
来源：http://m.share.tarul.cn/Article/details/gtyvehauj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fktsv.cn/Article/details/gnjtsysrs.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gfampicrq.sHtML

H. 异常与错误处理
来源：http://baike.yfazqb.com/Article/details/ghxbafmcy.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gcfirnhgw.sHtML

[H01] try / catch 基础
来源：http://m.share.vehdjk.com/Article/details/gyogodnnu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.bbcook.cn/Article/details/gbnkxmwly.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.bbcook.cn/Article/details/gtwbiqivg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.tarul.cn/Article/details/gkhtardbg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.sjlbkw.cn/Article/details/gtautikkl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fktsv.cn/Article/details/gtjafhkii.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.yfazqb.com/Article/details/gnpcbedvp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.epnwcf.com/Article/details/gdquzegxc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.tarul.cn/Article/details/gxcwckuzy.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fktsv.cn/Article/details/gjnxatqal.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.tarul.cn/Article/details/gobxeoclh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.tarul.cn/Article/details/ghbjgpwye.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.tarul.cn/Article/details/gxgwqrmxe.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.bbcook.cn/Article/details/gyjqttxzm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.bbcook.cn/Article/details/goirevliq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.sjlbkw.cn/Article/details/goonfmcwg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.sjlbkw.cn/Article/details/geluwrprp.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.vehdjk.com/Article/details/gzptrmrwx.sHtML

[H03] 主动抛出异常
来源：http://www.blog.tarul.cn/Article/details/gyeqeozih.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.tarul.cn/Article/details/gcbzpseat.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.yfazqb.com/Article/details/gbjtedpyh.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.vehdjk.com/Article/details/ghvvmwrfj.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.vehdjk.com/Article/details/gqoobgbcj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.yfazqb.com/Article/details/gglszybno.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.vehdjk.com/Article/details/gdtxuhoaf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.tarul.cn/Article/details/gupoctkhp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.epnwcf.com/Article/details/gljhskwky.sHtML

[H04] 自定义异常类型
来源：http://wap.sjlbkw.cn/Article/details/ggdfpoqtj.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.yfazqb.com/Article/details/gtiwuqydh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.fktsv.cn/Article/details/gusqagksc.sHtML

JS:   class MyError extends Error {}
来源：http://blog.sjlbkw.cn/Article/details/glevlinde.sHtML

TS:   class MyError extends Error {}
来源：http://blog.vehdjk.com/Article/details/gftjnkeqm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.epnwcf.com/Article/details/gfhthmilh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.tarul.cn/Article/details/gtnjkpmby.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.epnwcf.com/Article/details/ggdviohjl.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.tarul.cn/Article/details/gwisctkeb.sHtML

[H05] 捕获特定类型
来源：http://www.blog.epnwcf.com/Article/details/gdguqewsu.sHtML

Py:   except ValueError as e:
来源：http://blog.yfazqb.com/Article/details/gybetlgzc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.epnwcf.com/Article/details/gjdmbsgvy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.yfazqb.com/Article/details/gxapkyasf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.epnwcf.com/Article/details/ganajsfkj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.bbcook.cn/Article/details/gzehfcvxk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.yfazqb.com/Article/details/gnkaxedmq.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.bbcook.cn/Article/details/gmxqzykye.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.vehdjk.com/Article/details/gnuqqraey.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.tarul.cn/Article/details/gpfnlpfyp.sHtML

Py:   value = d.get("k") or default
来源：http://3g.tarul.cn/Article/details/gjddfbibm.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.epnwcf.com/Article/details/gfmksbifq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.sjlbkw.cn/Article/details/glozdjkuj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.epnwcf.com/Article/details/gcgtkbfkw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.bbcook.cn/Article/details/gpstgzxov.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.bbcook.cn/Article/details/grobhmrfc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.epnwcf.com/Article/details/gkowuuwhf.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.epnwcf.com/Article/details/grcyrityg.sHtML

[H07] 断言
来源：http://read.share.fktsv.cn/Article/details/guecogbpt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.sjlbkw.cn/Article/details/gbsnliupq.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.bbcook.cn/Article/details/gvvihrbit.sHtML

JS:   console.assert(x > 0);
来源：http://blog.sjlbkw.cn/Article/details/gdinfohhp.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.sjlbkw.cn/Article/details/gndhijihz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.vehdjk.com/Article/details/gypfaokau.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.tarul.cn/Article/details/gerflftni.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.epnwcf.com/Article/details/gmdvuajwb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.vehdjk.com/Article/details/gvtockswi.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.epnwcf.com/Article/details/gvxsnywsk.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.bbcook.cn/Article/details/gzeliltci.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.epnwcf.com/Article/details/gprnxyxar.sHtML

JS:   e.message;  e.stack
来源：http://read.share.sjlbkw.cn/Article/details/gdbxreehi.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.fktsv.cn/Article/details/ghryekwfu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.bbcook.cn/Article/details/gyluidwsd.sHtML

Go:   err.Error()
来源：http://read.share.tarul.cn/Article/details/gakopidoq.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.yfazqb.com/Article/details/gkjhbrrrk.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.bbcook.cn/Article/details/gurrqqggl.sHtML

[H09] 带错误码的异常
来源：http://www.share.yfazqb.com/Article/details/gbblzwbsn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.bbcook.cn/Article/details/gdlwqtfsh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.epnwcf.com/Article/details/glktnxrte.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.yfazqb.com/Article/details/gjydnmash.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.tarul.cn/Article/details/gqqmuibcd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.vehdjk.com/Article/details/geoljeroo.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.tarul.cn/Article/details/gmkzbyvfp.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.epnwcf.com/Article/details/gxiowapel.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.vehdjk.com/Article/details/gnazyopke.sHtML

[H10] 资源自动释放
来源：http://3g.yfazqb.com/Article/details/gnxmocizf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.tarul.cn/Article/details/gkchrdhzn.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.bbcook.cn/Article/details/gnxziilkz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.epnwcf.com/Article/details/gdalaulxv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fktsv.cn/Article/details/gddnnfzvf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.sjlbkw.cn/Article/details/gekvzcfnx.sHtML

Go:   defer f.Close()
来源：http://www.share.tarul.cn/Article/details/gyuidqnof.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.tarul.cn/Article/details/gytdunmzl.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gvyabapcm.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gqamwqxmt.sHtML

I. 正则表达式
来源：http://3g.fktsv.cn/Article/details/gjjysshkx.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gyuovokqv.sHtML

[I01] 判断是否匹配
来源：http://www.blog.bbcook.cn/Article/details/gwaoujecb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.epnwcf.com/Article/details/gobvyncqa.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.yfazqb.com/Article/details/gkmrecpim.sHtML

JS:   /\d+/.test(s)
来源：http://blog.sjlbkw.cn/Article/details/gzjrfloow.sHtML

TS:   /\d+/.test(s)
来源：http://baike.tarul.cn/Article/details/gttwwuarb.sHtML


<!-- 参考信息 -->