代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.epnwcf.com/Article/details/gxxnebacw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.yfazqb.com/Article/details/gxmehmysa.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.epnwcf.com/Article/details/gykosrcby.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.bbcook.cn/Article/details/gjsfeaega.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fktsv.cn/Article/details/gpulphksk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.tarul.cn/Article/details/gzedybpdh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.vehdjk.com/Article/details/gwlnywbxw.sHtML

[F08] 遍历目录
来源：http://www.share.bbcook.cn/Article/details/gxjceaacp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.sjlbkw.cn/Article/details/gryrncqpy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.tarul.cn/Article/details/gqqojiczq.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.tarul.cn/Article/details/gegbvnmva.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.vehdjk.com/Article/details/gcrhbltre.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.sjlbkw.cn/Article/details/ggtgiuips.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fktsv.cn/Article/details/gtbccwivu.sHtML

Ruby: Dir.children("dir")
来源：http://3g.tarul.cn/Article/details/gdhsxpdmn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.epnwcf.com/Article/details/gtmgqzwcv.sHtML

[F09] 获取文件大小
来源：http://read.share.fktsv.cn/Article/details/gaacgaxaz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.tarul.cn/Article/details/gtensenry.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gbsveuiky.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.epnwcf.com/Article/details/gzxmebesg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.bbcook.cn/Article/details/gavdokohz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.sjlbkw.cn/Article/details/gfmzavwmt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.vehdjk.com/Article/details/gpuspglrd.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.yfazqb.com/Article/details/ghcuqkdok.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.epnwcf.com/Article/details/gtglyluqw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.bbcook.cn/Article/details/gaudpogta.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gqkefhcjp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.yfazqb.com/Article/details/gvxqoyjym.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gbotxpbwo.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gzcumzyjo.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.vehdjk.com/Article/details/gohflvwkn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.tarul.cn/Article/details/gxyrwplqh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/gvilvaxll.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fktsv.cn/Article/details/gnsedepmz.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.yfazqb.com/Article/details/giyogumck.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.tarul.cn/Article/details/grpbnxolo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gaoiahhpb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.sjlbkw.cn/Article/details/gzizrubab.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fktsv.cn/Article/details/gejxpcups.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.tarul.cn/Article/details/gkvlmgsth.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.yfazqb.com/Article/details/gnacruitk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.bbcook.cn/Article/details/gcbobdxzi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.bbcook.cn/Article/details/ggkwpklkz.sHtML

[F12] CSV 读写
来源：http://mobile.fktsv.cn/Article/details/gyglokpnr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.vehdjk.com/Article/details/ggceqoavw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fktsv.cn/Article/details/gqpspjqat.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.tarul.cn/Article/details/goirvsxkp.sHtML

TS:   // 同上
来源：http://m.share.vehdjk.com/Article/details/gvovtwqpq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.vehdjk.com/Article/details/gnbwxeqif.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.tarul.cn/Article/details/gspbidohh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.sjlbkw.cn/Article/details/gnshziwlr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.vehdjk.com/Article/details/gcopiaskx.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/guinepsfh.sHtML

G. 面向对象
来源：http://www.blog.yfazqb.com/Article/details/gclnwrueo.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/grscglfue.sHtML

[G01] 定义类
来源：http://read.share.bbcook.cn/Article/details/goysfyznc.sHtML

Py:   class User: pass
来源：http://m.share.epnwcf.com/Article/details/gtrqfytlo.sHtML

PHP:  class User {}
来源：http://www.blog.bbcook.cn/Article/details/gxslnybux.sHtML

JS:   class User {}
来源：http://m.share.epnwcf.com/Article/details/gfzoetrfd.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.tarul.cn/Article/details/gzmgiscci.sHtML

Java: class User {}
来源：http://read.share.epnwcf.com/Article/details/gcahmavsx.sHtML

Go:   type User struct { Name string }
来源：http://3g.fktsv.cn/Article/details/gzgjlowte.sHtML

Ruby: class User; end
来源：http://wap.vehdjk.com/Article/details/gbotqhmxw.sHtML

C#:   class User {}
来源：http://wap.tarul.cn/Article/details/giwegxuxs.sHtML

[G02] 构造函数
来源：http://read.share.fktsv.cn/Article/details/giuzpqosl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.sjlbkw.cn/Article/details/gmmnktikd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.yfazqb.com/Article/details/giibsrnbh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.bbcook.cn/Article/details/gdeloxqeh.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.tarul.cn/Article/details/grnolknkb.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.tarul.cn/Article/details/gnznelnmh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.bbcook.cn/Article/details/gelrvrehy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.vehdjk.com/Article/details/garsvtkae.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.vehdjk.com/Article/details/grsvrtfgf.sHtML

[G03] 实例属性
来源：http://mobile.sjlbkw.cn/Article/details/gatcimhir.sHtML

Py:   self.name = "x"
来源：http://www.blog.bbcook.cn/Article/details/gvoangdnz.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.vehdjk.com/Article/details/gyksbfimo.sHtML

JS:   this.name = "x";
来源：http://mobile.yfazqb.com/Article/details/gzgfrizes.sHtML

TS:   name: string = "x";
来源：http://www.share.fktsv.cn/Article/details/gngusgkbi.sHtML

Java: private String name;
来源：http://read.share.tarul.cn/Article/details/gqhyecuni.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.vehdjk.com/Article/details/gwhlpwozv.sHtML

Ruby: @name = "x"
来源：http://baike.sjlbkw.cn/Article/details/gfktgyljq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fktsv.cn/Article/details/gqqepbhwf.sHtML

[G04] 定义方法
来源：http://mobile.fktsv.cn/Article/details/gjrrhihko.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.vehdjk.com/Article/details/gmumxqitg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fktsv.cn/Article/details/gmlmzqzgb.sHtML

JS:   greet() { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/ggjzikobz.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.yfazqb.com/Article/details/gntotfmee.sHtML

Java: String greet() { return name; }
来源：http://read.share.fktsv.cn/Article/details/glpbvbltj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fktsv.cn/Article/details/gbsletpfq.sHtML

Ruby: def greet; @name; end
来源：http://wap.fktsv.cn/Article/details/gjzmfpiic.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fktsv.cn/Article/details/gvnaxnfbc.sHtML

[G05] 继承
来源：http://www.blog.vehdjk.com/Article/details/gqxcjvler.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.sjlbkw.cn/Article/details/gdkwxmdox.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fktsv.cn/Article/details/gygjgeljj.sHtML

JS:   class Admin extends User {}
来源：http://3g.epnwcf.com/Article/details/gnwgzsspf.sHtML

TS:   class Admin extends User {}
来源：http://blog.bbcook.cn/Article/details/gooknheud.sHtML

Java: class Admin extends User {}
来源：http://baike.vehdjk.com/Article/details/gdataqqri.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fktsv.cn/Article/details/gjbaenzbc.sHtML

Ruby: class Admin < User; end
来源：http://wap.sjlbkw.cn/Article/details/ghidmplyd.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.tarul.cn/Article/details/gknenbjtr.sHtML

[G06] 重写方法
来源：http://wap.bbcook.cn/Article/details/gudktevzm.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.tarul.cn/Article/details/geybduvur.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.epnwcf.com/Article/details/gterskwwj.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fktsv.cn/Article/details/gbfkbdjfb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.tarul.cn/Article/details/gybnqtnyp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.tarul.cn/Article/details/gevjqinql.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.epnwcf.com/Article/details/gmsrlzegt.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gmikmrmpo.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fktsv.cn/Article/details/gnfxyizid.sHtML

[G07] 调用父类方法
来源：http://baike.epnwcf.com/Article/details/gvcyiyqtl.sHtML

Py:   super().greet()
来源：http://www.m.share.sjlbkw.cn/Article/details/gjjjkxszs.sHtML

PHP:  parent::greet();
来源：http://m.share.bbcook.cn/Article/details/gyqrmihbl.sHtML

JS:   super.greet();
来源：http://www.share.epnwcf.com/Article/details/gvnxhfxea.sHtML

TS:   super.greet();
来源：http://www.share.bbcook.cn/Article/details/grrookzoo.sHtML

Java: super.greet();
来源：http://3g.vehdjk.com/Article/details/gmrakmzpo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.sjlbkw.cn/Article/details/gjydjpzdj.sHtML

Ruby: super
来源：http://3g.vehdjk.com/Article/details/gnzmwwbzm.sHtML

C#:   base.Greet();
来源：http://www.blog.sjlbkw.cn/Article/details/gbiyipgly.sHtML

[G08] 静态方法与属性
来源：http://read.share.epnwcf.com/Article/details/gnaogqlyr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.epnwcf.com/Article/details/gchmqdrqd.sHtML

PHP:  public static function f() {}
来源：http://www.share.vehdjk.com/Article/details/gtevkiwze.sHtML

JS:   static f() {}
来源：http://blog.fktsv.cn/Article/details/ggzdkksye.sHtML

TS:   static f(): void {}
来源：http://blog.bbcook.cn/Article/details/gtbxfmqij.sHtML

Java: static void f() {}
来源：http://read.share.epnwcf.com/Article/details/gmejzvosi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.yfazqb.com/Article/details/gitlhorax.sHtML

Ruby: def self.f; end
来源：http://www.blog.sjlbkw.cn/Article/details/gffjkbjmr.sHtML

C#:   public static void F() {}
来源：http://www.m.share.bbcook.cn/Article/details/gjnyrjqny.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.tarul.cn/Article/details/ganzurydl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.vehdjk.com/Article/details/groiopdag.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.vehdjk.com/Article/details/gyrdjzfza.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.tarul.cn/Article/details/gtcmaqvne.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.yfazqb.com/Article/details/gjlwyxypb.sHtML

Java: interface Shape { double area(); }
来源：http://wap.sjlbkw.cn/Article/details/gqvijiefj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.sjlbkw.cn/Article/details/gmsdtxreu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.sjlbkw.cn/Article/details/gmlfkxslj.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.vehdjk.com/Article/details/gunucssvv.sHtML

[G10] 访问控制
来源：http://www.blog.fktsv.cn/Article/details/gqswfogss.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.sjlbkw.cn/Article/details/gdvsaugae.sHtML

PHP:  public / protected / private
来源：http://blog.tarul.cn/Article/details/geoxkivnt.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.bbcook.cn/Article/details/gwhgbeuhi.sHtML

TS:   public / protected / private
来源：http://mobile.yfazqb.com/Article/details/ghbgsdbvl.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fktsv.cn/Article/details/guigdqqec.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.tarul.cn/Article/details/gwkbonieh.sHtML

Ruby: public / protected / private
来源：http://wap.bbcook.cn/Article/details/gfppmjrqx.sHtML

C#:   public / protected / private / internal
来源：http://3g.fktsv.cn/Article/details/gdumeckhu.sHtML

[G11] getter / setter
来源：http://baike.sjlbkw.cn/Article/details/gdpfisgmk.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.yfazqb.com/Article/details/gbssmjvam.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.vehdjk.com/Article/details/glgvzfczh.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.bbcook.cn/Article/details/gspviepmo.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.epnwcf.com/Article/details/ghwckbbwe.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fktsv.cn/Article/details/geckcrubk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.yfazqb.com/Article/details/gdydqrnex.sHtML

Ruby: attr_accessor :name
来源：http://baike.sjlbkw.cn/Article/details/grsgjeapd.sHtML

C#:   public string Name { get; set; }
来源：http://blog.vehdjk.com/Article/details/gkduscmhb.sHtML

[G12] 对象转字符串
来源：http://read.share.yfazqb.com/Article/details/gwsxlofsi.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.bbcook.cn/Article/details/gksscdjtu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fktsv.cn/Article/details/gcujdloix.sHtML

JS:   toString() { return this.name; }
来源：http://3g.epnwcf.com/Article/details/gfpsaczsc.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.tarul.cn/Article/details/gwbtdiyox.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.vehdjk.com/Article/details/gaithydtd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.yfazqb.com/Article/details/gdkvjulcb.sHtML

Ruby: def to_s; @name; end
来源：http://3g.bbcook.cn/Article/details/gpnnhsgco.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.vehdjk.com/Article/details/gzxsqiexu.sHtML

[G13] 判断对象类型
来源：http://wap.sjlbkw.cn/Article/details/gdijxcjvf.sHtML

Py:   isinstance(u, User)
来源：http://m.share.epnwcf.com/Article/details/guxivdpkd.sHtML

PHP:  $u instanceof User
来源：http://www.blog.epnwcf.com/Article/details/ghdphsedw.sHtML

JS:   u instanceof User
来源：http://www.blog.fktsv.cn/Article/details/ggnqninlp.sHtML

TS:   u instanceof User
来源：http://www.share.vehdjk.com/Article/details/gpexlbkbu.sHtML

Java: u instanceof User
来源：http://www.share.fktsv.cn/Article/details/glplntbcq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.epnwcf.com/Article/details/gjffudrec.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.sjlbkw.cn/Article/details/gqmjidvtv.sHtML

C#:   u is User
来源：http://baike.fktsv.cn/Article/details/ghketqwev.sHtML

[G14] 数据类 / record
来源：http://m.share.tarul.cn/Article/details/gevfahlaz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.tarul.cn/Article/details/gbdbtdcob.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.vehdjk.com/Article/details/gipzcnkuk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.vehdjk.com/Article/details/gwrftuain.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.sjlbkw.cn/Article/details/gjfxzvfit.sHtML

Java: record User(String name, int age) {}
来源：http://baike.epnwcf.com/Article/details/gktstyfwr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.vehdjk.com/Article/details/gmmstbjig.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.fktsv.cn/Article/details/giajznfou.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.bbcook.cn/Article/details/gjufkkuyz.sHtML

[G15] 枚举
来源：http://m.share.sjlbkw.cn/Article/details/gurgmwbai.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.epnwcf.com/Article/details/gxcjkugtg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.yfazqb.com/Article/details/gwfftldmz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fktsv.cn/Article/details/gvymcukin.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.sjlbkw.cn/Article/details/gkmbatoyt.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fktsv.cn/Article/details/gixtdphhx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.epnwcf.com/Article/details/ggprvamso.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.sjlbkw.cn/Article/details/gekbvrxqb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.yfazqb.com/Article/details/guziyuhys.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.sjlbkw.cn/Article/details/gxeyngaok.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fktsv.cn/Article/details/gwnlbrwnh.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.sjlbkw.cn/Article/details/gsptknaeq.sHtML

JS:   Object.entries(obj)
来源：http://wap.bbcook.cn/Article/details/grplmlzih.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gyrbnxxty.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.bbcook.cn/Article/details/gticubeqp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.vehdjk.com/Article/details/gjxkulqvy.sHtML

Ruby: obj.instance_variables
来源：http://3g.fktsv.cn/Article/details/gpggwhzfo.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.yfazqb.com/Article/details/giqkgoxki.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gvtmygyoy.sHtML

H. 异常与错误处理
来源：http://baike.vehdjk.com/Article/details/guexqlonp.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gjsuzdhic.sHtML

[H01] try / catch 基础
来源：http://wap.epnwcf.com/Article/details/gdwfgghzs.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.vehdjk.com/Article/details/gtmzmygls.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.vehdjk.com/Article/details/glckwrrcs.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.bbcook.cn/Article/details/gipxjnaxc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.epnwcf.com/Article/details/gjapkurtl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.tarul.cn/Article/details/gwffggktc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.epnwcf.com/Article/details/garcxubza.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.fktsv.cn/Article/details/gxuwsqhdy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.fktsv.cn/Article/details/gwbcpjwex.sHtML

[H02] finally / ensure 收尾
来源：http://3g.epnwcf.com/Article/details/gkqfjtzti.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.yfazqb.com/Article/details/gejlpjulo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.yfazqb.com/Article/details/gplnosdbp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.yfazqb.com/Article/details/gyjimgmkj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fktsv.cn/Article/details/gebzkhrtx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/gxufbtxqr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.tarul.cn/Article/details/gockcprpe.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.vehdjk.com/Article/details/gmnvkbghq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.epnwcf.com/Article/details/golzwvxqv.sHtML

[H03] 主动抛出异常
来源：http://mobile.fktsv.cn/Article/details/gqmhzzoyy.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.epnwcf.com/Article/details/gylyiqowa.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.vehdjk.com/Article/details/ggyuzhvgp.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.bbcook.cn/Article/details/gipsbpumj.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.tarul.cn/Article/details/gkwtimxyo.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.vehdjk.com/Article/details/gzakobmgq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.bbcook.cn/Article/details/gwgrpbnuc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.epnwcf.com/Article/details/gddeqyfvd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/gkigbddwy.sHtML

[H04] 自定义异常类型
来源：http://www.blog.vehdjk.com/Article/details/gycguysby.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.vehdjk.com/Article/details/gbylnvkvq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.tarul.cn/Article/details/gwtggrpil.sHtML

JS:   class MyError extends Error {}
来源：http://wap.epnwcf.com/Article/details/ggalvsyij.sHtML

TS:   class MyError extends Error {}
来源：http://3g.epnwcf.com/Article/details/gwxxqbows.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.vehdjk.com/Article/details/gsptgcmkj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.bbcook.cn/Article/details/ghtcmjbfr.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.fktsv.cn/Article/details/glgbzrbqf.sHtML

C#:   class MyException : Exception {}
来源：http://3g.epnwcf.com/Article/details/gkeubefkv.sHtML

[H05] 捕获特定类型
来源：http://read.share.yfazqb.com/Article/details/gtddtbwsh.sHtML

Py:   except ValueError as e:
来源：http://wap.vehdjk.com/Article/details/gaeijddkw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.sjlbkw.cn/Article/details/gfkoxtsdo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.fktsv.cn/Article/details/ggbaqwdoi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.epnwcf.com/Article/details/gwpkxtxkg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.bbcook.cn/Article/details/gnnzijdjw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.epnwcf.com/Article/details/gkxrzmwmu.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fktsv.cn/Article/details/gqrhftogg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.sjlbkw.cn/Article/details/gluofibjk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.vehdjk.com/Article/details/gkpvnfsyu.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.tarul.cn/Article/details/gcglzmyxu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.sjlbkw.cn/Article/details/gghmagmtv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.epnwcf.com/Article/details/gzvcqzdgo.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.bbcook.cn/Article/details/gmghdbcto.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.vehdjk.com/Article/details/gyyrsudho.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.tarul.cn/Article/details/gchetdfpn.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.vehdjk.com/Article/details/gcbbefrem.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.epnwcf.com/Article/details/gcidqnitc.sHtML

[H07] 断言
来源：http://3g.fktsv.cn/Article/details/gjzuvvece.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.fktsv.cn/Article/details/gvozywuba.sHtML

PHP:  assert($x > 0);
来源：http://blog.sjlbkw.cn/Article/details/gzdwsssge.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.sjlbkw.cn/Article/details/gfnyibrmb.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.yfazqb.com/Article/details/gdauyinkl.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.bbcook.cn/Article/details/grvverixm.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.vehdjk.com/Article/details/gvewvtbgr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.fktsv.cn/Article/details/gkigxrhbh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.epnwcf.com/Article/details/gzcdgtygs.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.bbcook.cn/Article/details/gxwbveiuu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.tarul.cn/Article/details/gorgwobnc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.vehdjk.com/Article/details/ggfzpptci.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.sjlbkw.cn/Article/details/gaekkahpb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.epnwcf.com/Article/details/gvtzdycjs.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.sjlbkw.cn/Article/details/guoldpdva.sHtML

Go:   err.Error()
来源：http://www.blog.epnwcf.com/Article/details/gmredpgcn.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.sjlbkw.cn/Article/details/gdwadasmh.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.bbcook.cn/Article/details/gazojdlbz.sHtML

[H09] 带错误码的异常
来源：http://www.blog.fktsv.cn/Article/details/gsnyrgibs.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.tarul.cn/Article/details/gfnkykxcx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.sjlbkw.cn/Article/details/gdcwsddng.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.epnwcf.com/Article/details/gghbblgzr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.bbcook.cn/Article/details/gezuvebcw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.tarul.cn/Article/details/gpyabahlx.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.sjlbkw.cn/Article/details/genxgjiey.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.tarul.cn/Article/details/gzczqcnys.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.epnwcf.com/Article/details/gxptvblcr.sHtML

[H10] 资源自动释放
来源：http://read.share.epnwcf.com/Article/details/gombsftkr.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.tarul.cn/Article/details/gnbimkpcb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.bbcook.cn/Article/details/gvimfcoix.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.tarul.cn/Article/details/ghxpuhohq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.sjlbkw.cn/Article/details/gmracywrj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.tarul.cn/Article/details/gsgvdvuwg.sHtML

Go:   defer f.Close()
来源：http://www.blog.fktsv.cn/Article/details/gvuvilyyw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.epnwcf.com/Article/details/gaellqfdw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gelvmdqao.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/glvqtyuzq.sHtML

I. 正则表达式
来源：http://mobile.epnwcf.com/Article/details/gmduytqwv.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/ggvzpjdth.sHtML

[I01] 判断是否匹配
来源：http://www.share.yfazqb.com/Article/details/gaobdygkt.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.fktsv.cn/Article/details/gvweqxhox.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.fktsv.cn/Article/details/gbxyyjrmw.sHtML

JS:   /\d+/.test(s)
来源：http://blog.epnwcf.com/Article/details/gpngyvudz.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.vehdjk.com/Article/details/gfofgewtr.sHtML


<!-- 参考信息 -->