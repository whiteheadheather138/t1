代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://3g.epnwcf.com/Article/details/gtnepoynh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.sjlbkw.cn/Article/details/gbxketxse.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gjtmkotrs.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.tarul.cn/Article/details/gozujrynu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.yfazqb.com/Article/details/grcbgyzsf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.vehdjk.com/Article/details/gvcqkvtzq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.bbcook.cn/Article/details/gpwfumcez.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gfgqzvtzl.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gumrkkflu.sHtML

[F06] 删除文件
来源：http://3g.epnwcf.com/Article/details/gledfciwr.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/grgginvsk.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gbhurgtpd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fktsv.cn/Article/details/gsvveggic.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.vehdjk.com/Article/details/gvdbhymbo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.tarul.cn/Article/details/gpvyyseik.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gtpnlhcsb.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gqjmdfkmj.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/guxmvhrtn.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.yfazqb.com/Article/details/gowgigwux.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.tarul.cn/Article/details/gsblwflff.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.tarul.cn/Article/details/gcpshaqhq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.epnwcf.com/Article/details/guufghwgj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.sjlbkw.cn/Article/details/gpryruqqd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.epnwcf.com/Article/details/guwefttyo.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.vehdjk.com/Article/details/gvmslmwgj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.yfazqb.com/Article/details/gsrnupgvj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.bbcook.cn/Article/details/guwmzicff.sHtML

[F08] 遍历目录
来源：http://www.share.yfazqb.com/Article/details/gffenxumq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fktsv.cn/Article/details/gbnwrlqwz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.bbcook.cn/Article/details/gdqggztva.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fktsv.cn/Article/details/ghbovyqgz.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.fktsv.cn/Article/details/gsndzikmt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fktsv.cn/Article/details/gwlowcgzi.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.bbcook.cn/Article/details/gvdarrxqa.sHtML

Ruby: Dir.children("dir")
来源：http://3g.bbcook.cn/Article/details/glzicwqdr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.bbcook.cn/Article/details/ggagneypo.sHtML

[F09] 获取文件大小
来源：http://www.blog.tarul.cn/Article/details/ghxpynhnh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gtgydhavr.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gpsjoxgmo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.vehdjk.com/Article/details/gsewfmmgv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.bbcook.cn/Article/details/gecltiyqc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.yfazqb.com/Article/details/gbzjyuttr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.bbcook.cn/Article/details/gsrmlduoa.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gxlgkbugn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.vehdjk.com/Article/details/gaszuyooa.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.tarul.cn/Article/details/glqrxcfrh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gjuymqpti.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.bbcook.cn/Article/details/gwhtqafmz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.epnwcf.com/Article/details/glnxrcndi.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.tarul.cn/Article/details/gkahkawht.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.tarul.cn/Article/details/gnaqckisp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fktsv.cn/Article/details/gybnhnnqr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/gtfugdnch.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/gvdwowbxj.sHtML

[F11] 复制与移动文件
来源：http://baike.epnwcf.com/Article/details/gukubyilq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/gurhnsdaw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.epnwcf.com/Article/details/ginlrkbuu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gtfmjwhkx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fktsv.cn/Article/details/gvalpjhdt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.epnwcf.com/Article/details/ggqkudmzq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.bbcook.cn/Article/details/gxfdcpxyo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.sjlbkw.cn/Article/details/goelktkyw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.epnwcf.com/Article/details/gnxssnstr.sHtML

[F12] CSV 读写
来源：http://www.share.fktsv.cn/Article/details/goguztibx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.epnwcf.com/Article/details/gczwhjdlv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.yfazqb.com/Article/details/gmgtrpkml.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fktsv.cn/Article/details/gjwqdulra.sHtML

TS:   // 同上
来源：http://www.m.share.sjlbkw.cn/Article/details/ggaxgktgg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.epnwcf.com/Article/details/ggkplnxow.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.bbcook.cn/Article/details/gytgtmrbm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.tarul.cn/Article/details/gnlrhuwyh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.vehdjk.com/Article/details/glwktssqv.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gcaohqcyt.sHtML

G. 面向对象
来源：http://blog.sjlbkw.cn/Article/details/gbicalixd.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gnjuwxzxz.sHtML

[G01] 定义类
来源：http://www.blog.tarul.cn/Article/details/grlwpvere.sHtML

Py:   class User: pass
来源：http://www.m.share.vehdjk.com/Article/details/gfcpilixy.sHtML

PHP:  class User {}
来源：http://www.share.fktsv.cn/Article/details/gfekbvxui.sHtML

JS:   class User {}
来源：http://baike.fktsv.cn/Article/details/gylskcmve.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fktsv.cn/Article/details/gnnquxozq.sHtML

Java: class User {}
来源：http://wap.tarul.cn/Article/details/gcxdaggpt.sHtML

Go:   type User struct { Name string }
来源：http://www.share.epnwcf.com/Article/details/gpilwueib.sHtML

Ruby: class User; end
来源：http://mobile.epnwcf.com/Article/details/gtkvvigen.sHtML

C#:   class User {}
来源：http://www.share.epnwcf.com/Article/details/gcbiqagmv.sHtML

[G02] 构造函数
来源：http://www.blog.bbcook.cn/Article/details/gbyyiwqoc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.sjlbkw.cn/Article/details/gpczkltyd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.yfazqb.com/Article/details/gmqavwhja.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fktsv.cn/Article/details/gofdlhhrf.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.tarul.cn/Article/details/gibgqtljc.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.tarul.cn/Article/details/gpzbrjovv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.sjlbkw.cn/Article/details/giinmccsb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.epnwcf.com/Article/details/gqqnhaxkh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.yfazqb.com/Article/details/gwxisavhf.sHtML

[G03] 实例属性
来源：http://3g.tarul.cn/Article/details/ghdqoaspy.sHtML

Py:   self.name = "x"
来源：http://www.blog.sjlbkw.cn/Article/details/gsgwjckbg.sHtML

PHP:  public string $name = "x";
来源：http://mobile.sjlbkw.cn/Article/details/gnxhzozuy.sHtML

JS:   this.name = "x";
来源：http://read.share.fktsv.cn/Article/details/gzrcroatd.sHtML

TS:   name: string = "x";
来源：http://mobile.vehdjk.com/Article/details/guwgdpjjp.sHtML

Java: private String name;
来源：http://wap.fktsv.cn/Article/details/gwccusddn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.yfazqb.com/Article/details/gmzdbjwor.sHtML

Ruby: @name = "x"
来源：http://www.share.sjlbkw.cn/Article/details/gpswddtrl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.epnwcf.com/Article/details/gzfyseqab.sHtML

[G04] 定义方法
来源：http://www.share.yfazqb.com/Article/details/ghwykzuje.sHtML

Py:   def greet(self): return self.name
来源：http://blog.tarul.cn/Article/details/ggfoohmsm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.bbcook.cn/Article/details/geyecyxws.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/gdxmdeqwr.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.bbcook.cn/Article/details/gugxuqolq.sHtML

Java: String greet() { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/grgpginca.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.vehdjk.com/Article/details/gtqkmieow.sHtML

Ruby: def greet; @name; end
来源：http://wap.sjlbkw.cn/Article/details/gzzasqizr.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.epnwcf.com/Article/details/gefyretxy.sHtML

[G05] 继承
来源：http://www.blog.sjlbkw.cn/Article/details/giqmnzzmw.sHtML

Py:   class Admin(User): pass
来源：http://wap.sjlbkw.cn/Article/details/gaowzuvxk.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gmgjwwfok.sHtML

JS:   class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/gvgsdpwon.sHtML

TS:   class Admin extends User {}
来源：http://m.share.sjlbkw.cn/Article/details/gfzfmdxmo.sHtML

Java: class Admin extends User {}
来源：http://www.blog.tarul.cn/Article/details/ggydbqzit.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.tarul.cn/Article/details/gfqadnsox.sHtML

Ruby: class Admin < User; end
来源：http://baike.vehdjk.com/Article/details/gydlqtxix.sHtML

C#:   class Admin : User {}
来源：http://m.share.vehdjk.com/Article/details/glocyvyba.sHtML

[G06] 重写方法
来源：http://mobile.tarul.cn/Article/details/ghtvrneql.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.sjlbkw.cn/Article/details/gdpalkugc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.yfazqb.com/Article/details/gpekupond.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/grbkjrhgh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fktsv.cn/Article/details/gqnrrloib.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.yfazqb.com/Article/details/gbsavcmgp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fktsv.cn/Article/details/gnrwtzwam.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.sjlbkw.cn/Article/details/gasybmwik.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.bbcook.cn/Article/details/gxfonrdkw.sHtML

[G07] 调用父类方法
来源：http://www.share.epnwcf.com/Article/details/grpqlzyfd.sHtML

Py:   super().greet()
来源：http://read.share.epnwcf.com/Article/details/gyiiqwnan.sHtML

PHP:  parent::greet();
来源：http://www.blog.sjlbkw.cn/Article/details/gicngrtfx.sHtML

JS:   super.greet();
来源：http://m.share.fktsv.cn/Article/details/gqxcljyes.sHtML

TS:   super.greet();
来源：http://blog.sjlbkw.cn/Article/details/gtsvejnek.sHtML

Java: super.greet();
来源：http://blog.vehdjk.com/Article/details/gghsscqjr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.sjlbkw.cn/Article/details/gatwofzfw.sHtML

Ruby: super
来源：http://m.share.yfazqb.com/Article/details/gefnaoael.sHtML

C#:   base.Greet();
来源：http://read.share.bbcook.cn/Article/details/glrkxlkrj.sHtML

[G08] 静态方法与属性
来源：http://mobile.vehdjk.com/Article/details/gcfsjvuwa.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fktsv.cn/Article/details/gqfhoxfyh.sHtML

PHP:  public static function f() {}
来源：http://wap.bbcook.cn/Article/details/gecrbqzrq.sHtML

JS:   static f() {}
来源：http://read.share.vehdjk.com/Article/details/gxfnoaasn.sHtML

TS:   static f(): void {}
来源：http://blog.yfazqb.com/Article/details/glphxaupu.sHtML

Java: static void f() {}
来源：http://www.blog.yfazqb.com/Article/details/gkyzbriru.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.tarul.cn/Article/details/gamarnncc.sHtML

Ruby: def self.f; end
来源：http://www.m.share.bbcook.cn/Article/details/gchiyswfu.sHtML

C#:   public static void F() {}
来源：http://blog.yfazqb.com/Article/details/gbwubjuyq.sHtML

[G09] 接口 / 抽象类
来源：http://3g.bbcook.cn/Article/details/goxydbxgr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.bbcook.cn/Article/details/gyartphrv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.epnwcf.com/Article/details/gbxsgyrnz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.epnwcf.com/Article/details/gyzkhcxwa.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.bbcook.cn/Article/details/gxnxmqcxa.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.epnwcf.com/Article/details/gaqquuxle.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.yfazqb.com/Article/details/gewtkccyh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.bbcook.cn/Article/details/gredppkoy.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.tarul.cn/Article/details/gfharmclt.sHtML

[G10] 访问控制
来源：http://www.share.sjlbkw.cn/Article/details/gnawgrqng.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.epnwcf.com/Article/details/gkzbwfdxx.sHtML

PHP:  public / protected / private
来源：http://www.m.share.sjlbkw.cn/Article/details/gixthtnrw.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.yfazqb.com/Article/details/guktpbtef.sHtML

TS:   public / protected / private
来源：http://read.share.bbcook.cn/Article/details/gtutolcsv.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fktsv.cn/Article/details/giuugtejr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.epnwcf.com/Article/details/ghfeonaxk.sHtML

Ruby: public / protected / private
来源：http://blog.bbcook.cn/Article/details/gaucxsfzq.sHtML

C#:   public / protected / private / internal
来源：http://www.share.vehdjk.com/Article/details/gaegfmvbn.sHtML

[G11] getter / setter
来源：http://mobile.tarul.cn/Article/details/ghpmnpmoi.sHtML

Py:   @property 与 @x.setter
来源：http://baike.epnwcf.com/Article/details/gnznakxmw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.epnwcf.com/Article/details/gyclsjrze.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.epnwcf.com/Article/details/ggpetwhgy.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.sjlbkw.cn/Article/details/gzulsseju.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/gyvmwzgpi.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.yfazqb.com/Article/details/gwibrazvd.sHtML

Ruby: attr_accessor :name
来源：http://www.share.tarul.cn/Article/details/gjvbxxckg.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.yfazqb.com/Article/details/gzxkvicdj.sHtML

[G12] 对象转字符串
来源：http://3g.sjlbkw.cn/Article/details/gxztheoiz.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.tarul.cn/Article/details/gnyjddvgr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fktsv.cn/Article/details/gckitjnky.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/giutxbmdy.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.bbcook.cn/Article/details/gbcxtjbrx.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fktsv.cn/Article/details/gwhkrsbbm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.epnwcf.com/Article/details/gwnycpwqp.sHtML

Ruby: def to_s; @name; end
来源：http://wap.sjlbkw.cn/Article/details/gdoicqonm.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.vehdjk.com/Article/details/geghloodu.sHtML

[G13] 判断对象类型
来源：http://www.share.bbcook.cn/Article/details/gchegynef.sHtML

Py:   isinstance(u, User)
来源：http://baike.epnwcf.com/Article/details/gybyeylnl.sHtML

PHP:  $u instanceof User
来源：http://mobile.tarul.cn/Article/details/gunwaczig.sHtML

JS:   u instanceof User
来源：http://www.m.share.vehdjk.com/Article/details/garsupnxe.sHtML

TS:   u instanceof User
来源：http://www.blog.yfazqb.com/Article/details/gihycppcq.sHtML

Java: u instanceof User
来源：http://www.share.yfazqb.com/Article/details/gyumkpyao.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.tarul.cn/Article/details/gahutciva.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.bbcook.cn/Article/details/grucpxxwj.sHtML

C#:   u is User
来源：http://www.share.vehdjk.com/Article/details/gjjshizfi.sHtML

[G14] 数据类 / record
来源：http://read.share.tarul.cn/Article/details/gwgfmyzgl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.fktsv.cn/Article/details/gtfflrnug.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.vehdjk.com/Article/details/gnipupihu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.vehdjk.com/Article/details/gvheouiut.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.bbcook.cn/Article/details/gzawejtaw.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.vehdjk.com/Article/details/gyaxkdxwr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.epnwcf.com/Article/details/gbhwnmgmv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.bbcook.cn/Article/details/gaopzrkop.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.sjlbkw.cn/Article/details/gkcglutdv.sHtML

[G15] 枚举
来源：http://www.blog.bbcook.cn/Article/details/gregpidez.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.sjlbkw.cn/Article/details/gisojhdcy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fktsv.cn/Article/details/ghrvmocql.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.bbcook.cn/Article/details/gboslzyhx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.bbcook.cn/Article/details/gdutlilsi.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.yfazqb.com/Article/details/girjvsuyw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.bbcook.cn/Article/details/gwmttbgzw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.epnwcf.com/Article/details/getbidxka.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.epnwcf.com/Article/details/gwtghjxip.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.tarul.cn/Article/details/gdnvhgeyo.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.tarul.cn/Article/details/geeeximlz.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.epnwcf.com/Article/details/gkqbrwfeo.sHtML

JS:   Object.entries(obj)
来源：http://blog.fktsv.cn/Article/details/gtcskqbni.sHtML

TS:   Object.entries(obj)
来源：http://www.share.vehdjk.com/Article/details/gxchhgfam.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.bbcook.cn/Article/details/gytitjedx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.bbcook.cn/Article/details/gwhnugddy.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.vehdjk.com/Article/details/gjuzsoplj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.bbcook.cn/Article/details/geamwofhs.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gzbftxgtj.sHtML

H. 异常与错误处理
来源：http://www.blog.sjlbkw.cn/Article/details/gbeupvork.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gnguqegwc.sHtML

[H01] try / catch 基础
来源：http://read.share.sjlbkw.cn/Article/details/gxgxkbzlc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.sjlbkw.cn/Article/details/gtojrqjam.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.tarul.cn/Article/details/ggazizbws.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.vehdjk.com/Article/details/govslhrqf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.sjlbkw.cn/Article/details/gqewercgc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.yfazqb.com/Article/details/gprmzzsan.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.bbcook.cn/Article/details/gqgbzbkkr.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gfpvusonp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.sjlbkw.cn/Article/details/gwrhytbbd.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.vehdjk.com/Article/details/guzupjehw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fktsv.cn/Article/details/gkbplvvue.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.vehdjk.com/Article/details/gldjnczyw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.yfazqb.com/Article/details/gyaatrvrv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/gdwvssszd.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.tarul.cn/Article/details/gwjbfrmgu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.bbcook.cn/Article/details/gzkmszuae.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.tarul.cn/Article/details/gvnhtruoz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/ghrzlpqml.sHtML

[H03] 主动抛出异常
来源：http://3g.bbcook.cn/Article/details/gcbhfhdtt.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.tarul.cn/Article/details/gykukduix.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.tarul.cn/Article/details/gmmemzuhq.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.yfazqb.com/Article/details/gxmmmqmty.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.epnwcf.com/Article/details/ghqidnkcz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.epnwcf.com/Article/details/gehfcdjyw.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.bbcook.cn/Article/details/giwoeairp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.vehdjk.com/Article/details/gskukdfff.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.epnwcf.com/Article/details/gbcmzvvef.sHtML

[H04] 自定义异常类型
来源：http://blog.fktsv.cn/Article/details/gntiwcqdj.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.yfazqb.com/Article/details/ggejvaesy.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.bbcook.cn/Article/details/gltxmdgka.sHtML

JS:   class MyError extends Error {}
来源：http://3g.epnwcf.com/Article/details/gkodnmbkb.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.tarul.cn/Article/details/gfmlwexrb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.vehdjk.com/Article/details/gsjtjsewz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.epnwcf.com/Article/details/gwlixyoip.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.bbcook.cn/Article/details/gezotcmqm.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.tarul.cn/Article/details/grdsedpjz.sHtML

[H05] 捕获特定类型
来源：http://3g.tarul.cn/Article/details/gzsvtxktn.sHtML

Py:   except ValueError as e:
来源：http://wap.yfazqb.com/Article/details/gvchlbphg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.tarul.cn/Article/details/gdyoybpld.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.vehdjk.com/Article/details/gvhkiwpxr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.epnwcf.com/Article/details/gpuaqfqkj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.yfazqb.com/Article/details/gikigxrxo.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.yfazqb.com/Article/details/gsympuurq.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.epnwcf.com/Article/details/glztrstkx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.yfazqb.com/Article/details/gmtqimxfp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.epnwcf.com/Article/details/gctpkgjun.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.epnwcf.com/Article/details/gyeljehhk.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.bbcook.cn/Article/details/gyqvroqvr.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.sjlbkw.cn/Article/details/gvcgobwyn.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.vehdjk.com/Article/details/goihdaikg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.sjlbkw.cn/Article/details/goofymunq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.sjlbkw.cn/Article/details/gypwiwhow.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.fktsv.cn/Article/details/gysclewmj.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.fktsv.cn/Article/details/gutykbtrv.sHtML

[H07] 断言
来源：http://wap.sjlbkw.cn/Article/details/gopgyxzcg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.epnwcf.com/Article/details/gukjpmouu.sHtML

PHP:  assert($x > 0);
来源：http://read.share.vehdjk.com/Article/details/gdbslbwdc.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fktsv.cn/Article/details/gttyxixkl.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.tarul.cn/Article/details/gklssugjb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.yfazqb.com/Article/details/gcqvqfvej.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.yfazqb.com/Article/details/grwrqnccp.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fktsv.cn/Article/details/gagzyhqlt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.fktsv.cn/Article/details/gcdycjpgs.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.sjlbkw.cn/Article/details/gmjcjbiup.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.yfazqb.com/Article/details/gdqrsjyhp.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.epnwcf.com/Article/details/gnxugfztp.sHtML

JS:   e.message;  e.stack
来源：http://wap.epnwcf.com/Article/details/gzmljqtqi.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.yfazqb.com/Article/details/gnnimmrja.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.fktsv.cn/Article/details/gcgoymbfj.sHtML

Go:   err.Error()
来源：http://read.share.sjlbkw.cn/Article/details/gdtbcblur.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.vehdjk.com/Article/details/gszdcnvzk.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.yfazqb.com/Article/details/gilgqleeh.sHtML

[H09] 带错误码的异常
来源：http://blog.epnwcf.com/Article/details/gxzzflrpn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.yfazqb.com/Article/details/gxpasrtiu.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.fktsv.cn/Article/details/gvzatghgg.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.fktsv.cn/Article/details/gvkjanmdi.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.sjlbkw.cn/Article/details/gugrkjsgi.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.vehdjk.com/Article/details/gmxfeimgf.sHtML


<!-- 参考信息 -->