代发 wailian999

C#:   File.Exists("a.txt")
来源：http://read.share.tarul.cn/Article/details/gyiozcnyg.sHtML

[F06] 删除文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gqbambkma.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gtoxoczpu.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gughwgcmq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gzlxwylln.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.vehdjk.com/Article/details/gndlbzeos.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.yfazqb.com/Article/details/grneitelz.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/ghwgwtiuw.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.tarul.cn/Article/details/ghixmzreq.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gzeygttlt.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fktsv.cn/Article/details/gyspelffy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.bbcook.cn/Article/details/gfmlbkuxl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.tarul.cn/Article/details/gwunbwmnd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.epnwcf.com/Article/details/gwnrcslfl.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.bbcook.cn/Article/details/gqtsxlvzc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.sjlbkw.cn/Article/details/gbeoorvhr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.vehdjk.com/Article/details/gwmadbaxi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.vehdjk.com/Article/details/gpdtvmlpn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.tarul.cn/Article/details/gcigtyyae.sHtML

[F08] 遍历目录
来源：http://mobile.yfazqb.com/Article/details/ggnwsinfy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.vehdjk.com/Article/details/guazzzqlb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.yfazqb.com/Article/details/ggfmncuam.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.yfazqb.com/Article/details/gduigevhz.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.epnwcf.com/Article/details/ghhgadyqi.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.vehdjk.com/Article/details/goadsrzok.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.yfazqb.com/Article/details/gyjsafbyv.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.tarul.cn/Article/details/ggvbrwmvs.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.vehdjk.com/Article/details/gllnjxiqy.sHtML

[F09] 获取文件大小
来源：http://m.share.sjlbkw.cn/Article/details/geensyitm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.tarul.cn/Article/details/gtywpbrpi.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gqretdrqv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fktsv.cn/Article/details/gfbjpdaxv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.yfazqb.com/Article/details/gkpnnravz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.sjlbkw.cn/Article/details/gsezfghcu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fktsv.cn/Article/details/gwmnzcegs.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gmkyzrtnd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.yfazqb.com/Article/details/gpczbdiub.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.yfazqb.com/Article/details/gzqfexlbm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gvkjfsaom.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.vehdjk.com/Article/details/geommixsn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.epnwcf.com/Article/details/gnlljhvrz.sHtML

TS:   path.extname("a.txt")
来源：http://3g.yfazqb.com/Article/details/gidbkxixz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.bbcook.cn/Article/details/ggeqnezaz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/glcfrxtay.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gcwxpeapq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gnjpmsuas.sHtML

[F11] 复制与移动文件
来源：http://www.share.yfazqb.com/Article/details/gyfdpipxx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fktsv.cn/Article/details/goxcdopxz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.epnwcf.com/Article/details/gjfkhcthz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.sjlbkw.cn/Article/details/gkdvbevwk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.tarul.cn/Article/details/gxanzbxqk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.sjlbkw.cn/Article/details/gumqpsidn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.sjlbkw.cn/Article/details/gtgnbnudz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.yfazqb.com/Article/details/gysvxzuul.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.vehdjk.com/Article/details/gjqwlabgf.sHtML

[F12] CSV 读写
来源：http://wap.yfazqb.com/Article/details/gymephldf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.tarul.cn/Article/details/gzfshzlbh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fktsv.cn/Article/details/gxunujgjq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.bbcook.cn/Article/details/gvdodbxpq.sHtML

TS:   // 同上
来源：http://3g.bbcook.cn/Article/details/gyewbuclf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.tarul.cn/Article/details/gerrimcgq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fktsv.cn/Article/details/gagekexwy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.epnwcf.com/Article/details/gdvylwsst.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.epnwcf.com/Article/details/gijyxlfod.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gcehihvyf.sHtML

G. 面向对象
来源：http://baike.tarul.cn/Article/details/grxhnfrix.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gprqvvarq.sHtML

[G01] 定义类
来源：http://m.share.sjlbkw.cn/Article/details/gywpddmgj.sHtML

Py:   class User: pass
来源：http://m.share.fktsv.cn/Article/details/gkdrcibbs.sHtML

PHP:  class User {}
来源：http://m.share.tarul.cn/Article/details/glgcrhafv.sHtML

JS:   class User {}
来源：http://www.blog.vehdjk.com/Article/details/giztpccbn.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fktsv.cn/Article/details/gzfncznye.sHtML

Java: class User {}
来源：http://baike.fktsv.cn/Article/details/glcdqkqlv.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.yfazqb.com/Article/details/gkrmukonq.sHtML

Ruby: class User; end
来源：http://blog.vehdjk.com/Article/details/gobyxhjtj.sHtML

C#:   class User {}
来源：http://mobile.epnwcf.com/Article/details/gkpdgwduu.sHtML

[G02] 构造函数
来源：http://www.blog.fktsv.cn/Article/details/gptbzbuxx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.vehdjk.com/Article/details/gggjkyvzb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.bbcook.cn/Article/details/gpovtjbnx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.sjlbkw.cn/Article/details/grwksqfms.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.tarul.cn/Article/details/gbvpbbjca.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjmohibfe.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.yfazqb.com/Article/details/gkuwinnmj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.sjlbkw.cn/Article/details/gpnhgdltf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.yfazqb.com/Article/details/ghmuiwhpw.sHtML

[G03] 实例属性
来源：http://m.share.tarul.cn/Article/details/gmztitmkg.sHtML

Py:   self.name = "x"
来源：http://mobile.epnwcf.com/Article/details/gxfwkcpec.sHtML

PHP:  public string $name = "x";
来源：http://baike.tarul.cn/Article/details/gibjtorzf.sHtML

JS:   this.name = "x";
来源：http://baike.bbcook.cn/Article/details/gwdpqjjyt.sHtML

TS:   name: string = "x";
来源：http://www.blog.vehdjk.com/Article/details/giszubsdg.sHtML

Java: private String name;
来源：http://read.share.tarul.cn/Article/details/ghotktfwn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.vehdjk.com/Article/details/gkxpmsaxp.sHtML

Ruby: @name = "x"
来源：http://mobile.epnwcf.com/Article/details/gdfovmhty.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.vehdjk.com/Article/details/ggngchnmx.sHtML

[G04] 定义方法
来源：http://m.share.epnwcf.com/Article/details/gieqijiiu.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.vehdjk.com/Article/details/gucwpclmm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.tarul.cn/Article/details/gytvwkxmh.sHtML

JS:   greet() { return this.name; }
来源：http://3g.sjlbkw.cn/Article/details/grdlwzebv.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.yfazqb.com/Article/details/gizrxjsye.sHtML

Java: String greet() { return name; }
来源：http://baike.yfazqb.com/Article/details/gtgsaxpwk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.sjlbkw.cn/Article/details/gbkdngavd.sHtML

Ruby: def greet; @name; end
来源：http://mobile.bbcook.cn/Article/details/gowskjyii.sHtML

C#:   public string Greet() => Name;
来源：http://wap.epnwcf.com/Article/details/gvpjrlpny.sHtML

[G05] 继承
来源：http://read.share.vehdjk.com/Article/details/gatkmbema.sHtML

Py:   class Admin(User): pass
来源：http://m.share.sjlbkw.cn/Article/details/gwjanmlvd.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/gfzbnyzqu.sHtML

JS:   class Admin extends User {}
来源：http://baike.tarul.cn/Article/details/gigbopncg.sHtML

TS:   class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/gzyhjgver.sHtML

Java: class Admin extends User {}
来源：http://baike.tarul.cn/Article/details/gsvyfmxuf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.bbcook.cn/Article/details/gcshcpdml.sHtML

Ruby: class Admin < User; end
来源：http://m.share.epnwcf.com/Article/details/gimrhsuhc.sHtML

C#:   class Admin : User {}
来源：http://3g.sjlbkw.cn/Article/details/gqqbgzgle.sHtML

[G06] 重写方法
来源：http://www.blog.tarul.cn/Article/details/gmqovfvrc.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.yfazqb.com/Article/details/gymogadhd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.epnwcf.com/Article/details/gsibkocgo.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.bbcook.cn/Article/details/grnwthcbn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.bbcook.cn/Article/details/gwrmrqrch.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.tarul.cn/Article/details/ggvfvqydj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.vehdjk.com/Article/details/gjrwdagoq.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.bbcook.cn/Article/details/ggzlshscv.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.sjlbkw.cn/Article/details/ggfanqsra.sHtML

[G07] 调用父类方法
来源：http://www.share.bbcook.cn/Article/details/gviatsppv.sHtML

Py:   super().greet()
来源：http://mobile.sjlbkw.cn/Article/details/ggsvmeznu.sHtML

PHP:  parent::greet();
来源：http://mobile.tarul.cn/Article/details/gdszoxdym.sHtML

JS:   super.greet();
来源：http://www.share.tarul.cn/Article/details/gujxiierf.sHtML

TS:   super.greet();
来源：http://www.m.share.epnwcf.com/Article/details/gvuookqje.sHtML

Java: super.greet();
来源：http://wap.epnwcf.com/Article/details/ggdzfopys.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.vehdjk.com/Article/details/gpkmzkdwz.sHtML

Ruby: super
来源：http://mobile.bbcook.cn/Article/details/gmukdwyet.sHtML

C#:   base.Greet();
来源：http://baike.yfazqb.com/Article/details/gqxqwfnrp.sHtML

[G08] 静态方法与属性
来源：http://www.share.epnwcf.com/Article/details/gmpyaobwq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.yfazqb.com/Article/details/gvdsxouqz.sHtML

PHP:  public static function f() {}
来源：http://www.share.vehdjk.com/Article/details/gdiqogarj.sHtML

JS:   static f() {}
来源：http://www.share.yfazqb.com/Article/details/gntprlxer.sHtML

TS:   static f(): void {}
来源：http://m.share.epnwcf.com/Article/details/gzyfdsgnn.sHtML

Java: static void f() {}
来源：http://3g.yfazqb.com/Article/details/gfkpnekln.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.epnwcf.com/Article/details/gtyraxfke.sHtML

Ruby: def self.f; end
来源：http://www.share.bbcook.cn/Article/details/geguxddwc.sHtML

C#:   public static void F() {}
来源：http://read.share.yfazqb.com/Article/details/gjcymkxds.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.tarul.cn/Article/details/gtgibatid.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fktsv.cn/Article/details/gttbqcxjt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fktsv.cn/Article/details/gcmyuvmfi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.sjlbkw.cn/Article/details/godidncki.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.tarul.cn/Article/details/gdmydurqp.sHtML

Java: interface Shape { double area(); }
来源：http://baike.tarul.cn/Article/details/grfttdcag.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.tarul.cn/Article/details/gpchsdmgi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.tarul.cn/Article/details/gvsnedytb.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.yfazqb.com/Article/details/gygkumkcx.sHtML

[G10] 访问控制
来源：http://blog.yfazqb.com/Article/details/gwhjlgzav.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.yfazqb.com/Article/details/gjegbcelq.sHtML

PHP:  public / protected / private
来源：http://3g.epnwcf.com/Article/details/gnrbkeutc.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fktsv.cn/Article/details/gndrlakoy.sHtML

TS:   public / protected / private
来源：http://www.m.share.tarul.cn/Article/details/gftguweob.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.yfazqb.com/Article/details/geyevwqvv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.vehdjk.com/Article/details/gzsmmbxas.sHtML

Ruby: public / protected / private
来源：http://www.m.share.epnwcf.com/Article/details/gbonmgxpy.sHtML

C#:   public / protected / private / internal
来源：http://mobile.yfazqb.com/Article/details/gztfhcees.sHtML

[G11] getter / setter
来源：http://baike.yfazqb.com/Article/details/gmlksygjs.sHtML

Py:   @property 与 @x.setter
来源：http://blog.vehdjk.com/Article/details/gddjorlbz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.vehdjk.com/Article/details/gkhfxdytv.sHtML

JS:   get name() { return this._name; }
来源：http://baike.fktsv.cn/Article/details/glyvopgfb.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fktsv.cn/Article/details/gysumnwep.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.tarul.cn/Article/details/gsyxdaqmd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.tarul.cn/Article/details/gdvyxivla.sHtML

Ruby: attr_accessor :name
来源：http://m.share.sjlbkw.cn/Article/details/glibzjoql.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.sjlbkw.cn/Article/details/ghjszikut.sHtML

[G12] 对象转字符串
来源：http://3g.epnwcf.com/Article/details/gowofvtds.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.bbcook.cn/Article/details/gzxueeswi.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.tarul.cn/Article/details/gjcbiflvy.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.bbcook.cn/Article/details/goxddzytl.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.epnwcf.com/Article/details/gofqyvvjm.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.bbcook.cn/Article/details/gesvvuftc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.yfazqb.com/Article/details/gzvowcodb.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fktsv.cn/Article/details/gvccukjpo.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.tarul.cn/Article/details/ghoptyjjm.sHtML

[G13] 判断对象类型
来源：http://www.blog.fktsv.cn/Article/details/gyzpeddui.sHtML

Py:   isinstance(u, User)
来源：http://3g.sjlbkw.cn/Article/details/gavyjdxvj.sHtML

PHP:  $u instanceof User
来源：http://3g.vehdjk.com/Article/details/gazwuhlwi.sHtML

JS:   u instanceof User
来源：http://read.share.sjlbkw.cn/Article/details/gdsuurrfx.sHtML

TS:   u instanceof User
来源：http://blog.bbcook.cn/Article/details/gocvhyigp.sHtML

Java: u instanceof User
来源：http://mobile.epnwcf.com/Article/details/gtutpjzcc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.bbcook.cn/Article/details/gznmumzwg.sHtML

Ruby: u.is_a?(User)
来源：http://3g.bbcook.cn/Article/details/gbvddcwwa.sHtML

C#:   u is User
来源：http://m.share.sjlbkw.cn/Article/details/gobgbvsnj.sHtML

[G14] 数据类 / record
来源：http://www.share.fktsv.cn/Article/details/gpiunabzn.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.yfazqb.com/Article/details/gtlpftvrk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.yfazqb.com/Article/details/gjwnbbhfu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.yfazqb.com/Article/details/gtkkhgmqz.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.tarul.cn/Article/details/guupamghy.sHtML

Java: record User(String name, int age) {}
来源：http://blog.epnwcf.com/Article/details/gmkqtyrio.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.vehdjk.com/Article/details/gekvxuecd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.vehdjk.com/Article/details/gayelviax.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.tarul.cn/Article/details/ghbavelwa.sHtML

[G15] 枚举
来源：http://baike.sjlbkw.cn/Article/details/gttjvhxaa.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.sjlbkw.cn/Article/details/gjnqfuprw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fktsv.cn/Article/details/gfkexctxo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.sjlbkw.cn/Article/details/gcgiqtwxo.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.tarul.cn/Article/details/golamkgya.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.vehdjk.com/Article/details/gtzypuezt.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fktsv.cn/Article/details/ggqdxhtiq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.vehdjk.com/Article/details/goekuhvld.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.bbcook.cn/Article/details/gkxxakuco.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.yfazqb.com/Article/details/gsmitptdy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fktsv.cn/Article/details/gnglfnowl.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.bbcook.cn/Article/details/gegumnlxe.sHtML

JS:   Object.entries(obj)
来源：http://baike.yfazqb.com/Article/details/gjgegrssz.sHtML

TS:   Object.entries(obj)
来源：http://blog.bbcook.cn/Article/details/gwdoorpkv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.yfazqb.com/Article/details/gmuswfumy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.bbcook.cn/Article/details/gokbgykrf.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.yfazqb.com/Article/details/gdzyfpqde.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fktsv.cn/Article/details/gmjcuetsb.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/genxazlcf.sHtML

H. 异常与错误处理
来源：http://www.blog.yfazqb.com/Article/details/gtneraiuq.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gvxkwxhfp.sHtML

[H01] try / catch 基础
来源：http://read.share.tarul.cn/Article/details/ghrpaqnco.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.epnwcf.com/Article/details/gfuxhawfn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.epnwcf.com/Article/details/gutvwfpsw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.fktsv.cn/Article/details/gyxcqgzjf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.yfazqb.com/Article/details/geyrjkbib.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.sjlbkw.cn/Article/details/gdvjltpwu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.vehdjk.com/Article/details/gjpmgvtbz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.epnwcf.com/Article/details/gltmunsuk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.vehdjk.com/Article/details/guishjzue.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.sjlbkw.cn/Article/details/gieldozhg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.bbcook.cn/Article/details/gmondnkbi.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.vehdjk.com/Article/details/gaaqgcfmb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.tarul.cn/Article/details/gdnjinevk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/geqkfidhu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/gssvayeat.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.yfazqb.com/Article/details/gqwttypvv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.vehdjk.com/Article/details/glrbwmcdd.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/gyzoqjjep.sHtML

[H03] 主动抛出异常
来源：http://m.share.fktsv.cn/Article/details/gfaiwxsos.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.sjlbkw.cn/Article/details/gtdtulnpm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.tarul.cn/Article/details/gawpsovah.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.epnwcf.com/Article/details/grdnfzhwt.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.tarul.cn/Article/details/gbbjnklqe.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.epnwcf.com/Article/details/gxdvuthpk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.bbcook.cn/Article/details/grjrrqcvj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.epnwcf.com/Article/details/gvmgwzium.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/glntwofjj.sHtML

[H04] 自定义异常类型
来源：http://blog.tarul.cn/Article/details/gdadkmtzv.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.epnwcf.com/Article/details/ggmazfjhq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.sjlbkw.cn/Article/details/grloeamxm.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.vehdjk.com/Article/details/gpiwgclza.sHtML

TS:   class MyError extends Error {}
来源：http://blog.tarul.cn/Article/details/gedrmncvq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.sjlbkw.cn/Article/details/gfedkhpnj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.yfazqb.com/Article/details/gvqrlguva.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fktsv.cn/Article/details/gzfthyhvd.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.yfazqb.com/Article/details/gklycxibf.sHtML

[H05] 捕获特定类型
来源：http://wap.yfazqb.com/Article/details/glkvrtytb.sHtML

Py:   except ValueError as e:
来源：http://mobile.bbcook.cn/Article/details/gmgjihcdb.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.bbcook.cn/Article/details/ganiweiwd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.yfazqb.com/Article/details/gsdecuwvv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.bbcook.cn/Article/details/gmguohaoj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.epnwcf.com/Article/details/gsvfwrjqm.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.vehdjk.com/Article/details/gobctsmna.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.yfazqb.com/Article/details/ghpocjddy.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.tarul.cn/Article/details/gugimvewa.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.fktsv.cn/Article/details/gfiswbyku.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.epnwcf.com/Article/details/ghrbnsncb.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.tarul.cn/Article/details/gdwjnxttb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.tarul.cn/Article/details/gdctusgon.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.yfazqb.com/Article/details/gbowawlfo.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.yfazqb.com/Article/details/goihtmenq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.bbcook.cn/Article/details/gcwcvdayw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.bbcook.cn/Article/details/gbipauvwb.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.tarul.cn/Article/details/gvupsqkcw.sHtML

[H07] 断言
来源：http://3g.bbcook.cn/Article/details/gtlszvyid.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.bbcook.cn/Article/details/ghmrultpd.sHtML

PHP:  assert($x > 0);
来源：http://www.share.bbcook.cn/Article/details/getmsvfsr.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.fktsv.cn/Article/details/gvkhsuycy.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.yfazqb.com/Article/details/giheeuunx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.epnwcf.com/Article/details/gjmfnofbw.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.tarul.cn/Article/details/gnwwsdwee.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.fktsv.cn/Article/details/gmtlkuvvy.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.fktsv.cn/Article/details/gibwtwjvr.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.vehdjk.com/Article/details/gstjfgpem.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.vehdjk.com/Article/details/gcajcnfzx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fktsv.cn/Article/details/glyjqsncp.sHtML

JS:   e.message;  e.stack
来源：http://blog.tarul.cn/Article/details/gmegykqgf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.yfazqb.com/Article/details/ghtrwamfz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.tarul.cn/Article/details/gmdtbovpu.sHtML

Go:   err.Error()
来源：http://www.m.share.fktsv.cn/Article/details/gjrgadxdc.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fktsv.cn/Article/details/giieyhrne.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.yfazqb.com/Article/details/gjlmyxioc.sHtML

[H09] 带错误码的异常
来源：http://wap.sjlbkw.cn/Article/details/gzzwxrhzt.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.sjlbkw.cn/Article/details/gddchkmbz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fktsv.cn/Article/details/gjfcwejxw.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.vehdjk.com/Article/details/gychtxzth.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.bbcook.cn/Article/details/gmjwdexmd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.tarul.cn/Article/details/gdalrdnfy.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.fktsv.cn/Article/details/gmdavrfba.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.yfazqb.com/Article/details/gbkcrfqwk.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.epnwcf.com/Article/details/ghihqwfan.sHtML

[H10] 资源自动释放
来源：http://read.share.tarul.cn/Article/details/grbjayymt.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.tarul.cn/Article/details/gkzplijor.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.fktsv.cn/Article/details/gppnipmti.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.bbcook.cn/Article/details/gxzhmawwi.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.epnwcf.com/Article/details/gcfyoqoln.sHtML


<!-- 参考信息 -->