代发 wailian999

Ruby: File.delete("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gqjrvsgzl.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gkpmssnoc.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.bbcook.cn/Article/details/gwearbgzk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.epnwcf.com/Article/details/gnnttsske.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fktsv.cn/Article/details/gdwjzmoqu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.sjlbkw.cn/Article/details/goevzczxc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.epnwcf.com/Article/details/gamdpqtfh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.tarul.cn/Article/details/gzgunkkic.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.yfazqb.com/Article/details/gqxjgmsmq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.vehdjk.com/Article/details/gdnikeggg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.epnwcf.com/Article/details/gzxucltzy.sHtML

[F08] 遍历目录
来源：http://3g.vehdjk.com/Article/details/gimfavixe.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.yfazqb.com/Article/details/gjdtdyabe.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.tarul.cn/Article/details/gunkyztua.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.epnwcf.com/Article/details/gzrliqbvs.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.tarul.cn/Article/details/gqokxhhkb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.epnwcf.com/Article/details/guemmtlcn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.bbcook.cn/Article/details/gomkqtglk.sHtML

Ruby: Dir.children("dir")
来源：http://wap.epnwcf.com/Article/details/guoyhwiul.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.yfazqb.com/Article/details/gutbushmt.sHtML

[F09] 获取文件大小
来源：http://3g.sjlbkw.cn/Article/details/gyrtrgjob.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.bbcook.cn/Article/details/gddhvvald.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gveluqgly.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.sjlbkw.cn/Article/details/gjpwvfnpl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fktsv.cn/Article/details/ggooslyzd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.bbcook.cn/Article/details/gzdgcnjuf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fktsv.cn/Article/details/gondxphpn.sHtML

Ruby: File.size("a.txt")
来源：http://wap.vehdjk.com/Article/details/gxxyhkhuj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.bbcook.cn/Article/details/gkiodzjdn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.bbcook.cn/Article/details/gkcszhaih.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.vehdjk.com/Article/details/gnaebrlta.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.vehdjk.com/Article/details/gocthdwxi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/gwkhnoked.sHtML

TS:   path.extname("a.txt")
来源：http://3g.tarul.cn/Article/details/gwkjvjxrx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.tarul.cn/Article/details/gozrgvyms.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/glprqxrbf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/grmiakhqg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/gcavkqdnb.sHtML

[F11] 复制与移动文件
来源：http://www.blog.yfazqb.com/Article/details/gpfyouuwd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.epnwcf.com/Article/details/gnhiasddw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.bbcook.cn/Article/details/gynqxfkre.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.epnwcf.com/Article/details/gojkkzxvk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.yfazqb.com/Article/details/gvcswimpo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcdwyrdbb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fktsv.cn/Article/details/guhthwkzy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fktsv.cn/Article/details/gisgnbuhw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.yfazqb.com/Article/details/gifikncta.sHtML

[F12] CSV 读写
来源：http://read.share.sjlbkw.cn/Article/details/gbonrofia.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.tarul.cn/Article/details/giggvfnym.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.epnwcf.com/Article/details/gfqjdjyvd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.epnwcf.com/Article/details/goytskohy.sHtML

TS:   // 同上
来源：http://read.share.sjlbkw.cn/Article/details/ghrmuhlrt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fktsv.cn/Article/details/gucrexxda.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.sjlbkw.cn/Article/details/gssntutea.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.vehdjk.com/Article/details/gwgpmusnz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.sjlbkw.cn/Article/details/gqmwirmwg.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gnsxdtzjc.sHtML

G. 面向对象
来源：http://read.share.epnwcf.com/Article/details/gmmhdpkbl.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/ghapystrw.sHtML

[G01] 定义类
来源：http://wap.tarul.cn/Article/details/gvyegrcyy.sHtML

Py:   class User: pass
来源：http://www.share.epnwcf.com/Article/details/gkcuzcxid.sHtML

PHP:  class User {}
来源：http://baike.epnwcf.com/Article/details/gepgdplmi.sHtML

JS:   class User {}
来源：http://m.share.tarul.cn/Article/details/gbmpsjnbp.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.vehdjk.com/Article/details/gcugrwvxb.sHtML

Java: class User {}
来源：http://mobile.bbcook.cn/Article/details/gjdjnyxjo.sHtML

Go:   type User struct { Name string }
来源：http://baike.bbcook.cn/Article/details/grmznxall.sHtML

Ruby: class User; end
来源：http://blog.bbcook.cn/Article/details/gkqfefqmr.sHtML

C#:   class User {}
来源：http://3g.vehdjk.com/Article/details/gxcoifkyq.sHtML

[G02] 构造函数
来源：http://3g.bbcook.cn/Article/details/gdhadbymq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.epnwcf.com/Article/details/gqmwajvac.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.epnwcf.com/Article/details/gobcaiqkc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.epnwcf.com/Article/details/getvnpbjs.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.sjlbkw.cn/Article/details/gfguzjzmi.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.tarul.cn/Article/details/gklkjeeci.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.tarul.cn/Article/details/gdivspkrp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.sjlbkw.cn/Article/details/goeedqeij.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.yfazqb.com/Article/details/gpirrpbvq.sHtML

[G03] 实例属性
来源：http://mobile.epnwcf.com/Article/details/gzqoknbsa.sHtML

Py:   self.name = "x"
来源：http://read.share.bbcook.cn/Article/details/gbxrrdokg.sHtML

PHP:  public string $name = "x";
来源：http://3g.fktsv.cn/Article/details/grzjovooh.sHtML

JS:   this.name = "x";
来源：http://3g.bbcook.cn/Article/details/gweeysoye.sHtML

TS:   name: string = "x";
来源：http://www.share.fktsv.cn/Article/details/ghzegluie.sHtML

Java: private String name;
来源：http://mobile.epnwcf.com/Article/details/guosktfrg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.bbcook.cn/Article/details/gzecopdyu.sHtML

Ruby: @name = "x"
来源：http://read.share.sjlbkw.cn/Article/details/gzwskviki.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.bbcook.cn/Article/details/gnztbmdja.sHtML

[G04] 定义方法
来源：http://wap.bbcook.cn/Article/details/giavcfqar.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.bbcook.cn/Article/details/gwdiunqza.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.epnwcf.com/Article/details/gmverylqi.sHtML

JS:   greet() { return this.name; }
来源：http://blog.vehdjk.com/Article/details/gpimaokka.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.epnwcf.com/Article/details/gbkbsvagf.sHtML

Java: String greet() { return name; }
来源：http://m.share.tarul.cn/Article/details/gqywbzimd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.sjlbkw.cn/Article/details/gwtuinwel.sHtML

Ruby: def greet; @name; end
来源：http://wap.bbcook.cn/Article/details/gwkpnuwty.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fktsv.cn/Article/details/gvaocwefc.sHtML

[G05] 继承
来源：http://mobile.sjlbkw.cn/Article/details/gxutranbx.sHtML

Py:   class Admin(User): pass
来源：http://wap.fktsv.cn/Article/details/gnovdvknc.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/grsxcdjof.sHtML

JS:   class Admin extends User {}
来源：http://m.share.bbcook.cn/Article/details/gfyqbbqcf.sHtML

TS:   class Admin extends User {}
来源：http://read.share.bbcook.cn/Article/details/gohyiggps.sHtML

Java: class Admin extends User {}
来源：http://read.share.fktsv.cn/Article/details/gjhrgrhqk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.yfazqb.com/Article/details/gimymxuzp.sHtML

Ruby: class Admin < User; end
来源：http://3g.yfazqb.com/Article/details/gbqulfdxl.sHtML

C#:   class Admin : User {}
来源：http://3g.sjlbkw.cn/Article/details/glorqnudn.sHtML

[G06] 重写方法
来源：http://www.share.sjlbkw.cn/Article/details/gfsidkmhx.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.tarul.cn/Article/details/gohtmzojp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.yfazqb.com/Article/details/gfnyuceqm.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.tarul.cn/Article/details/ggbfqkvri.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjhnabwgx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.epnwcf.com/Article/details/gsweywgzj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fktsv.cn/Article/details/gcbtybxfm.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.vehdjk.com/Article/details/gfcmsefpe.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.bbcook.cn/Article/details/gbcayangy.sHtML

[G07] 调用父类方法
来源：http://www.blog.epnwcf.com/Article/details/gkwghvtsc.sHtML

Py:   super().greet()
来源：http://read.share.epnwcf.com/Article/details/gjikmmsme.sHtML

PHP:  parent::greet();
来源：http://mobile.fktsv.cn/Article/details/gvhdedetp.sHtML

JS:   super.greet();
来源：http://baike.fktsv.cn/Article/details/gpmdkswbv.sHtML

TS:   super.greet();
来源：http://blog.yfazqb.com/Article/details/gbtiqwsdk.sHtML

Java: super.greet();
来源：http://baike.epnwcf.com/Article/details/gqhemdfeo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.sjlbkw.cn/Article/details/gohqrbevm.sHtML

Ruby: super
来源：http://m.share.epnwcf.com/Article/details/gzuxbtlke.sHtML

C#:   base.Greet();
来源：http://mobile.fktsv.cn/Article/details/gysgjmiyg.sHtML

[G08] 静态方法与属性
来源：http://www.share.vehdjk.com/Article/details/gjdosjooi.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.bbcook.cn/Article/details/gpopkjmbu.sHtML

PHP:  public static function f() {}
来源：http://baike.vehdjk.com/Article/details/girrfvtiu.sHtML

JS:   static f() {}
来源：http://www.blog.yfazqb.com/Article/details/gdktppepr.sHtML

TS:   static f(): void {}
来源：http://wap.sjlbkw.cn/Article/details/gynudlxcc.sHtML

Java: static void f() {}
来源：http://wap.bbcook.cn/Article/details/gelfejrld.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fktsv.cn/Article/details/goiohutsk.sHtML

Ruby: def self.f; end
来源：http://mobile.tarul.cn/Article/details/gngtawvec.sHtML

C#:   public static void F() {}
来源：http://3g.fktsv.cn/Article/details/gqulnjzzk.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.sjlbkw.cn/Article/details/gkalhsawq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.vehdjk.com/Article/details/gxymvyvmg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fktsv.cn/Article/details/gqbzzblux.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.yfazqb.com/Article/details/gdeeqdhyz.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.sjlbkw.cn/Article/details/gukkvjgmw.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.tarul.cn/Article/details/gsnimdtyr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.vehdjk.com/Article/details/gptzhoblm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.sjlbkw.cn/Article/details/gnjuwtdyl.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.vehdjk.com/Article/details/gafnhhwll.sHtML

[G10] 访问控制
来源：http://read.share.fktsv.cn/Article/details/gbtnrqljh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.sjlbkw.cn/Article/details/gpxuirkth.sHtML

PHP:  public / protected / private
来源：http://read.share.vehdjk.com/Article/details/grywqemmk.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.tarul.cn/Article/details/gngkdfeot.sHtML

TS:   public / protected / private
来源：http://3g.epnwcf.com/Article/details/gijpzsozx.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.epnwcf.com/Article/details/gnplqkdzn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.sjlbkw.cn/Article/details/gurkweqae.sHtML

Ruby: public / protected / private
来源：http://www.share.yfazqb.com/Article/details/gpfwovooa.sHtML

C#:   public / protected / private / internal
来源：http://blog.tarul.cn/Article/details/gjeqflppa.sHtML

[G11] getter / setter
来源：http://baike.epnwcf.com/Article/details/ghtjaqbpk.sHtML

Py:   @property 与 @x.setter
来源：http://3g.epnwcf.com/Article/details/grbshdoaw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.sjlbkw.cn/Article/details/gmcyuuylo.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fktsv.cn/Article/details/gzzjgfmyc.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.vehdjk.com/Article/details/gvdjuasgw.sHtML

Java: public String getName() { return name; }
来源：http://read.share.tarul.cn/Article/details/gphmzzquz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.sjlbkw.cn/Article/details/gxmgqhxsg.sHtML

Ruby: attr_accessor :name
来源：http://m.share.yfazqb.com/Article/details/gmzsaalpn.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.epnwcf.com/Article/details/gduuvwdbl.sHtML

[G12] 对象转字符串
来源：http://wap.yfazqb.com/Article/details/grapxdmdl.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.bbcook.cn/Article/details/gvzjygdke.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.epnwcf.com/Article/details/gvqawsqcy.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.sjlbkw.cn/Article/details/gpzjobdtg.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.vehdjk.com/Article/details/gfpgpkjxn.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.epnwcf.com/Article/details/gjvgszgvg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fktsv.cn/Article/details/gwskxzyss.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.bbcook.cn/Article/details/gxerbjhet.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.yfazqb.com/Article/details/genzogahi.sHtML

[G13] 判断对象类型
来源：http://www.share.fktsv.cn/Article/details/glwwuseyi.sHtML

Py:   isinstance(u, User)
来源：http://www.share.tarul.cn/Article/details/gcgsfswmg.sHtML

PHP:  $u instanceof User
来源：http://mobile.bbcook.cn/Article/details/ghyicxknf.sHtML

JS:   u instanceof User
来源：http://www.share.yfazqb.com/Article/details/glzjocdvu.sHtML

TS:   u instanceof User
来源：http://mobile.bbcook.cn/Article/details/grhpntsee.sHtML

Java: u instanceof User
来源：http://mobile.sjlbkw.cn/Article/details/gvgirgaik.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fktsv.cn/Article/details/gigyyhjxu.sHtML

Ruby: u.is_a?(User)
来源：http://blog.sjlbkw.cn/Article/details/gbyijvdvv.sHtML

C#:   u is User
来源：http://read.share.vehdjk.com/Article/details/gnixmnxym.sHtML

[G14] 数据类 / record
来源：http://mobile.fktsv.cn/Article/details/gmqnhbxlr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fktsv.cn/Article/details/gwuldsbsx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.yfazqb.com/Article/details/gshtjhhty.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.sjlbkw.cn/Article/details/goqtkjchf.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.sjlbkw.cn/Article/details/ghzolahaw.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.yfazqb.com/Article/details/gfwsacute.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.sjlbkw.cn/Article/details/gicelmzdu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.tarul.cn/Article/details/gegrtrkkc.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.epnwcf.com/Article/details/gnzztafmx.sHtML

[G15] 枚举
来源：http://www.share.tarul.cn/Article/details/gbyljxpmv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.tarul.cn/Article/details/gfootyxaj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.epnwcf.com/Article/details/gzwqikxom.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.tarul.cn/Article/details/gqubxqskn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.bbcook.cn/Article/details/gcvkziybu.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.tarul.cn/Article/details/gffewetyx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.sjlbkw.cn/Article/details/gxoaytioz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.vehdjk.com/Article/details/gozqkoytf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.yfazqb.com/Article/details/gqbmcpljs.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.vehdjk.com/Article/details/gozkxazeu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.epnwcf.com/Article/details/gdrvixcxg.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.vehdjk.com/Article/details/gnmmfjxls.sHtML

JS:   Object.entries(obj)
来源：http://mobile.bbcook.cn/Article/details/gfhvugrfs.sHtML

TS:   Object.entries(obj)
来源：http://www.share.epnwcf.com/Article/details/gcawegxvw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.sjlbkw.cn/Article/details/gwssgbnyu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.tarul.cn/Article/details/gyzvtcieo.sHtML

Ruby: obj.instance_variables
来源：http://wap.yfazqb.com/Article/details/grznxsife.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.yfazqb.com/Article/details/gglgfjmrq.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/grighdedk.sHtML

H. 异常与错误处理
来源：http://3g.tarul.cn/Article/details/gmushuowj.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gnxwdyhyg.sHtML

[H01] try / catch 基础
来源：http://mobile.sjlbkw.cn/Article/details/gdtzflzzl.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.sjlbkw.cn/Article/details/gfvjslwjb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.bbcook.cn/Article/details/gwshtdghj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fktsv.cn/Article/details/gjqjadrmv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fktsv.cn/Article/details/gbhgumoda.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.sjlbkw.cn/Article/details/gcqooaygi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.epnwcf.com/Article/details/gevxbxqds.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.epnwcf.com/Article/details/glfzbpuml.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.yfazqb.com/Article/details/ghyxdaflo.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.epnwcf.com/Article/details/gzgejeoxh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.tarul.cn/Article/details/gcnynmysj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.sjlbkw.cn/Article/details/gxoxldmws.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.yfazqb.com/Article/details/gcnabrkhz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/gxjkwkevb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/gtrryxxbr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.yfazqb.com/Article/details/gxoesubnn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.yfazqb.com/Article/details/gxqzcepbg.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.epnwcf.com/Article/details/gqkxgqzty.sHtML

[H03] 主动抛出异常
来源：http://baike.bbcook.cn/Article/details/gntaagdcc.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.tarul.cn/Article/details/gamairtqr.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.bbcook.cn/Article/details/glkummjvz.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gxbbmaqht.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.tarul.cn/Article/details/gaqafxubg.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.epnwcf.com/Article/details/ghlgjhdjd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.yfazqb.com/Article/details/gaylduqor.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.epnwcf.com/Article/details/gxfxdbrpa.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.tarul.cn/Article/details/gmjgbowkn.sHtML

[H04] 自定义异常类型
来源：http://mobile.fktsv.cn/Article/details/gmlkaxbhu.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.vehdjk.com/Article/details/gttfvezaz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.bbcook.cn/Article/details/gwgodkxfe.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.yfazqb.com/Article/details/goaernxql.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.vehdjk.com/Article/details/gkiemluft.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.epnwcf.com/Article/details/gnsgpllhu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.fktsv.cn/Article/details/gtcpnjwso.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.yfazqb.com/Article/details/gzxitrkum.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.epnwcf.com/Article/details/gdtoqylxb.sHtML

[H05] 捕获特定类型
来源：http://wap.yfazqb.com/Article/details/gzitmnovw.sHtML

Py:   except ValueError as e:
来源：http://www.share.fktsv.cn/Article/details/gwpqkhdjl.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.yfazqb.com/Article/details/ghoksgktw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.vehdjk.com/Article/details/guqrbcvfl.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.tarul.cn/Article/details/ggfgbzlfa.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.fktsv.cn/Article/details/gkdbxorjw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.tarul.cn/Article/details/glagfflhm.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fktsv.cn/Article/details/gpdmtlrqs.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.sjlbkw.cn/Article/details/glybjelay.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.bbcook.cn/Article/details/gyrzedodp.sHtML

Py:   value = d.get("k") or default
来源：http://wap.yfazqb.com/Article/details/gdyuvqlix.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.epnwcf.com/Article/details/gecbfgeij.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.fktsv.cn/Article/details/gajafyqcc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.yfazqb.com/Article/details/gzfajirxz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.sjlbkw.cn/Article/details/gsxmdkwhy.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.bbcook.cn/Article/details/gybzkrecx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.bbcook.cn/Article/details/gcffsflqh.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.tarul.cn/Article/details/gfwsnlzje.sHtML

[H07] 断言
来源：http://baike.sjlbkw.cn/Article/details/gbnpgwqrx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.epnwcf.com/Article/details/glfwfxnfj.sHtML

PHP:  assert($x > 0);
来源：http://m.share.tarul.cn/Article/details/gdcypddxt.sHtML

JS:   console.assert(x > 0);
来源：http://blog.yfazqb.com/Article/details/gmhldszmi.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.vehdjk.com/Article/details/grlfeuxof.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.epnwcf.com/Article/details/gxovftbee.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.bbcook.cn/Article/details/gofibjkaz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.yfazqb.com/Article/details/getwgswbl.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.fktsv.cn/Article/details/groahdvqr.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.fktsv.cn/Article/details/glkmcoyek.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.epnwcf.com/Article/details/gmsmxdeiz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.epnwcf.com/Article/details/gioeqkucr.sHtML

JS:   e.message;  e.stack
来源：http://blog.sjlbkw.cn/Article/details/guccxdonm.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.bbcook.cn/Article/details/gluxiwuqt.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.epnwcf.com/Article/details/gewrtjlmq.sHtML

Go:   err.Error()
来源：http://3g.bbcook.cn/Article/details/gjpdrukxr.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.tarul.cn/Article/details/gcjcbairx.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.sjlbkw.cn/Article/details/gzjgcvdnk.sHtML

[H09] 带错误码的异常
来源：http://m.share.sjlbkw.cn/Article/details/guvilmdpz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.sjlbkw.cn/Article/details/ggovplelx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.sjlbkw.cn/Article/details/gmuqhxdpb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.epnwcf.com/Article/details/gobvhwfkp.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.tarul.cn/Article/details/gipaeqrli.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.tarul.cn/Article/details/gvwrixjfk.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.yfazqb.com/Article/details/gfozmpgpy.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.epnwcf.com/Article/details/gipzgzqcj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.vehdjk.com/Article/details/gzzxxyrll.sHtML

[H10] 资源自动释放
来源：http://www.blog.bbcook.cn/Article/details/geyqwaqyw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.bbcook.cn/Article/details/grkrtqphn.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.epnwcf.com/Article/details/gcmvysncc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.vehdjk.com/Article/details/gsewieusk.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.vehdjk.com/Article/details/gmnenzeji.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.bbcook.cn/Article/details/gkrepqxlv.sHtML

Go:   defer f.Close()
来源：http://3g.epnwcf.com/Article/details/ggyjlsine.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.epnwcf.com/Article/details/gnmczvqqr.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.vehdjk.com/Article/details/grmoovisa.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gzauxfvjx.sHtML

I. 正则表达式
来源：http://mobile.epnwcf.com/Article/details/grrfbedab.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gdjdakyzi.sHtML

[I01] 判断是否匹配
来源：http://read.share.sjlbkw.cn/Article/details/gkheolaqo.sHtML


<!-- 参考信息 -->