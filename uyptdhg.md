代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gfacankge.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.epnwcf.com/Article/details/gbrwiunfz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.vehdjk.com/Article/details/gczilgeub.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fktsv.cn/Article/details/gxrnuybgb.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gqgftvfwv.sHtML

[F06] 删除文件
来源：http://www.share.yfazqb.com/Article/details/gshmfvsnd.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.yfazqb.com/Article/details/giukvjsrd.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gefjkecln.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gwciynkqo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gsqwvdelk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.tarul.cn/Article/details/gugzugtvb.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.yfazqb.com/Article/details/grwzazdnn.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gfwachiwl.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gjsjlqulv.sHtML

[F07] 创建目录（含多级）
来源：http://3g.yfazqb.com/Article/details/gyqnyjhhb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.sjlbkw.cn/Article/details/gehajakdw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.bbcook.cn/Article/details/gcaaswctn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.epnwcf.com/Article/details/gfkzriwrd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fktsv.cn/Article/details/gzjhbajbv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.bbcook.cn/Article/details/gdiwahvmx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.epnwcf.com/Article/details/gluukqfbf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.vehdjk.com/Article/details/gnfaqxazi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.sjlbkw.cn/Article/details/gbpqiwbqs.sHtML

[F08] 遍历目录
来源：http://wap.vehdjk.com/Article/details/gklkskxqy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.bbcook.cn/Article/details/gqmmoerlz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.epnwcf.com/Article/details/gurzpzdva.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.vehdjk.com/Article/details/gvimleuoz.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/ganiyilgc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.sjlbkw.cn/Article/details/gwxyxprjk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.yfazqb.com/Article/details/gylwmowem.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fktsv.cn/Article/details/gqpgodvct.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.sjlbkw.cn/Article/details/gsezxappp.sHtML

[F09] 获取文件大小
来源：http://www.share.vehdjk.com/Article/details/gyayabmpv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/ganhgpmim.sHtML

PHP:  filesize("a.txt");
来源：http://blog.epnwcf.com/Article/details/gbjbcvnqq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.sjlbkw.cn/Article/details/gxnemacyt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.tarul.cn/Article/details/gkyvgtmwi.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.bbcook.cn/Article/details/gxhegidtk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fktsv.cn/Article/details/grkakkbqd.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fktsv.cn/Article/details/gzxlqhvwa.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.yfazqb.com/Article/details/gbjhxlyog.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.tarul.cn/Article/details/gfckgukli.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gvlrlvtgp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.bbcook.cn/Article/details/grighqnbo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fktsv.cn/Article/details/gdacquszc.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gwdbdozkq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.vehdjk.com/Article/details/gqkuwmwbf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/gnlreyunm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gfjtmctdh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.tarul.cn/Article/details/gxkbtgofy.sHtML

[F11] 复制与移动文件
来源：http://read.share.epnwcf.com/Article/details/gzwyamubs.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gxvrvecds.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gtngqmsvv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.epnwcf.com/Article/details/gzucvnihf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.tarul.cn/Article/details/gjcqbyeum.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.vehdjk.com/Article/details/ghcdvqgrq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.bbcook.cn/Article/details/gjjunztle.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gxlzpteqd.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.vehdjk.com/Article/details/gxkjivdmc.sHtML

[F12] CSV 读写
来源：http://m.share.yfazqb.com/Article/details/gcstbazbp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.epnwcf.com/Article/details/gcthxknpz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.sjlbkw.cn/Article/details/gqwgpdzhx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.vehdjk.com/Article/details/gkmirbwig.sHtML

TS:   // 同上
来源：http://3g.vehdjk.com/Article/details/gvezplfwn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.vehdjk.com/Article/details/gmyhpsone.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.bbcook.cn/Article/details/gqwphclvs.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.sjlbkw.cn/Article/details/ggqzbzkcf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.tarul.cn/Article/details/gzrkwsyph.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gstflurck.sHtML

G. 面向对象
来源：http://www.share.fktsv.cn/Article/details/gslkgecax.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gjrpjktpn.sHtML

[G01] 定义类
来源：http://baike.tarul.cn/Article/details/ghfxhzedm.sHtML

Py:   class User: pass
来源：http://www.share.epnwcf.com/Article/details/ghmmrthsh.sHtML

PHP:  class User {}
来源：http://read.share.vehdjk.com/Article/details/gnfbzvtso.sHtML

JS:   class User {}
来源：http://3g.yfazqb.com/Article/details/gekjmbxrs.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.epnwcf.com/Article/details/gveqogsey.sHtML

Java: class User {}
来源：http://www.m.share.tarul.cn/Article/details/gbsmbjdpp.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.vehdjk.com/Article/details/gpccuhaki.sHtML

Ruby: class User; end
来源：http://read.share.epnwcf.com/Article/details/gdpkygauz.sHtML

C#:   class User {}
来源：http://www.share.yfazqb.com/Article/details/gywiqiiuf.sHtML

[G02] 构造函数
来源：http://www.blog.bbcook.cn/Article/details/gmhixwcnv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.yfazqb.com/Article/details/ggxacxjws.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.bbcook.cn/Article/details/gcxadnvrr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.tarul.cn/Article/details/gupzotvoz.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fktsv.cn/Article/details/gtkbajodo.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.sjlbkw.cn/Article/details/gzrdpymzd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.bbcook.cn/Article/details/gdofmuuhr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.bbcook.cn/Article/details/gnrsxbgpm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.bbcook.cn/Article/details/gqrnwzium.sHtML

[G03] 实例属性
来源：http://baike.epnwcf.com/Article/details/gxlfhyiiw.sHtML

Py:   self.name = "x"
来源：http://blog.epnwcf.com/Article/details/gxvvudddi.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/gxmyxijfz.sHtML

JS:   this.name = "x";
来源：http://www.share.vehdjk.com/Article/details/guprkytyy.sHtML

TS:   name: string = "x";
来源：http://mobile.epnwcf.com/Article/details/gonhzjctd.sHtML

Java: private String name;
来源：http://www.share.bbcook.cn/Article/details/gutffyupm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.sjlbkw.cn/Article/details/gqvyqauph.sHtML

Ruby: @name = "x"
来源：http://baike.tarul.cn/Article/details/gbimjfexb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.tarul.cn/Article/details/gxrvfyszi.sHtML

[G04] 定义方法
来源：http://www.m.share.tarul.cn/Article/details/gcaxsayzl.sHtML

Py:   def greet(self): return self.name
来源：http://blog.sjlbkw.cn/Article/details/gcouqvusn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.tarul.cn/Article/details/gvccrkcdn.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.sjlbkw.cn/Article/details/gbwtngdnc.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.vehdjk.com/Article/details/ghvexushd.sHtML

Java: String greet() { return name; }
来源：http://baike.epnwcf.com/Article/details/grvhnejoy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.tarul.cn/Article/details/gmwlvpojs.sHtML

Ruby: def greet; @name; end
来源：http://read.share.bbcook.cn/Article/details/gofgmqhkl.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.vehdjk.com/Article/details/gzqrbxevi.sHtML

[G05] 继承
来源：http://www.m.share.epnwcf.com/Article/details/gvhvezkuz.sHtML

Py:   class Admin(User): pass
来源：http://3g.sjlbkw.cn/Article/details/gtlwrgdxt.sHtML

PHP:  class Admin extends User {}
来源：http://blog.yfazqb.com/Article/details/gyywyetmg.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.tarul.cn/Article/details/gggskdgtc.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fktsv.cn/Article/details/gpnbksvhn.sHtML

Java: class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/gchwmlmxf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.bbcook.cn/Article/details/gjcxuzkey.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.yfazqb.com/Article/details/gqgropzhq.sHtML

C#:   class Admin : User {}
来源：http://www.share.bbcook.cn/Article/details/grvtfaoal.sHtML

[G06] 重写方法
来源：http://www.m.share.epnwcf.com/Article/details/gvnaqojkq.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.yfazqb.com/Article/details/ggvujtcit.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/gkbhsdxnm.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.yfazqb.com/Article/details/goygyitrv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/gtbdlakle.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.tarul.cn/Article/details/gdrwiljkt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.bbcook.cn/Article/details/gzzblomgx.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.epnwcf.com/Article/details/gkpqdqgpf.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fktsv.cn/Article/details/gklweylhs.sHtML

[G07] 调用父类方法
来源：http://3g.epnwcf.com/Article/details/ghvkbprxh.sHtML

Py:   super().greet()
来源：http://www.m.share.sjlbkw.cn/Article/details/gzfuqlgyh.sHtML

PHP:  parent::greet();
来源：http://www.m.share.bbcook.cn/Article/details/ghnpbwfwn.sHtML

JS:   super.greet();
来源：http://mobile.tarul.cn/Article/details/glwatqdcd.sHtML

TS:   super.greet();
来源：http://baike.bbcook.cn/Article/details/ghqfmzzkm.sHtML

Java: super.greet();
来源：http://3g.bbcook.cn/Article/details/gfladpiwl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.epnwcf.com/Article/details/gpzrhixpj.sHtML

Ruby: super
来源：http://3g.vehdjk.com/Article/details/gzgaedmii.sHtML

C#:   base.Greet();
来源：http://baike.fktsv.cn/Article/details/gsmtjigkb.sHtML

[G08] 静态方法与属性
来源：http://m.share.yfazqb.com/Article/details/ghqjdaanw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fktsv.cn/Article/details/gxghepcmx.sHtML

PHP:  public static function f() {}
来源：http://read.share.fktsv.cn/Article/details/gxplnexnm.sHtML

JS:   static f() {}
来源：http://mobile.fktsv.cn/Article/details/gtvkbjukx.sHtML

TS:   static f(): void {}
来源：http://m.share.tarul.cn/Article/details/gsnegxnne.sHtML

Java: static void f() {}
来源：http://read.share.fktsv.cn/Article/details/gpqamfoqn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.vehdjk.com/Article/details/giinpzagk.sHtML

Ruby: def self.f; end
来源：http://www.blog.vehdjk.com/Article/details/gcwlpoakp.sHtML

C#:   public static void F() {}
来源：http://www.m.share.vehdjk.com/Article/details/glmllldwu.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.yfazqb.com/Article/details/gubupjrtk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.yfazqb.com/Article/details/gljnirguh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.vehdjk.com/Article/details/gtptidtch.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.vehdjk.com/Article/details/gsnmgynfe.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.sjlbkw.cn/Article/details/gojljqjav.sHtML

Java: interface Shape { double area(); }
来源：http://blog.bbcook.cn/Article/details/gqdeqkcwt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.sjlbkw.cn/Article/details/gshidxhyt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.vehdjk.com/Article/details/gcxayalcf.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.tarul.cn/Article/details/gosqafwda.sHtML

[G10] 访问控制
来源：http://mobile.bbcook.cn/Article/details/gymszouxs.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fktsv.cn/Article/details/gbutfxcsz.sHtML

PHP:  public / protected / private
来源：http://mobile.sjlbkw.cn/Article/details/gxungdjng.sHtML

JS:   #private 字段；其余公开
来源：http://3g.vehdjk.com/Article/details/ghvaygxfv.sHtML

TS:   public / protected / private
来源：http://www.blog.tarul.cn/Article/details/gfnpnpiow.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fktsv.cn/Article/details/gxxatmnxf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.vehdjk.com/Article/details/grfmqydzm.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fktsv.cn/Article/details/gfhvblflo.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fktsv.cn/Article/details/gxshxaqzr.sHtML

[G11] getter / setter
来源：http://www.m.share.epnwcf.com/Article/details/gyussvlhr.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.bbcook.cn/Article/details/gbctbtptp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.epnwcf.com/Article/details/gndkfkgco.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fktsv.cn/Article/details/glyqskdjn.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.tarul.cn/Article/details/gsmgilklz.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/gadocatho.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.epnwcf.com/Article/details/gnkcriapy.sHtML

Ruby: attr_accessor :name
来源：http://baike.bbcook.cn/Article/details/gotgzpgor.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.bbcook.cn/Article/details/giajxrldr.sHtML

[G12] 对象转字符串
来源：http://3g.sjlbkw.cn/Article/details/gxjesovex.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.bbcook.cn/Article/details/gbygtqzvn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gxlgammdi.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.vehdjk.com/Article/details/gdfvonjvg.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/glvtsjycu.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.bbcook.cn/Article/details/giegsznpq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.vehdjk.com/Article/details/gwmteruzf.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.tarul.cn/Article/details/gtcjdiqjx.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.sjlbkw.cn/Article/details/galqqzttu.sHtML

[G13] 判断对象类型
来源：http://www.m.share.tarul.cn/Article/details/gcckebfre.sHtML

Py:   isinstance(u, User)
来源：http://www.share.sjlbkw.cn/Article/details/guabkwmai.sHtML

PHP:  $u instanceof User
来源：http://mobile.bbcook.cn/Article/details/gsowclhpb.sHtML

JS:   u instanceof User
来源：http://3g.sjlbkw.cn/Article/details/geoqlezat.sHtML

TS:   u instanceof User
来源：http://3g.epnwcf.com/Article/details/gbapusthu.sHtML

Java: u instanceof User
来源：http://blog.fktsv.cn/Article/details/gpnovupgu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.epnwcf.com/Article/details/gxqbtczua.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.epnwcf.com/Article/details/gyeqiimws.sHtML

C#:   u is User
来源：http://wap.bbcook.cn/Article/details/gvovkswcr.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fktsv.cn/Article/details/gtfshszvw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.epnwcf.com/Article/details/gwyehswvx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.bbcook.cn/Article/details/grkiqyidt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.vehdjk.com/Article/details/gmfabyheo.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.bbcook.cn/Article/details/gnnvqjtvr.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.sjlbkw.cn/Article/details/ghinmzmya.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.tarul.cn/Article/details/gspptmdoo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.bbcook.cn/Article/details/gfqnunpny.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.tarul.cn/Article/details/glykurhbo.sHtML

[G15] 枚举
来源：http://wap.sjlbkw.cn/Article/details/gnjkjsswv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.bbcook.cn/Article/details/glaafzoex.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.yfazqb.com/Article/details/gbfmhbryf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.yfazqb.com/Article/details/ggcvnjzso.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.yfazqb.com/Article/details/gjemnlbjn.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.bbcook.cn/Article/details/gefygoqqc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.epnwcf.com/Article/details/gmuxaukxh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.yfazqb.com/Article/details/gvjuxpgvp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fktsv.cn/Article/details/gsfehskhz.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.sjlbkw.cn/Article/details/gvdvhzcwo.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.tarul.cn/Article/details/gfxtvndim.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.fktsv.cn/Article/details/gdbcahbpq.sHtML

JS:   Object.entries(obj)
来源：http://m.share.vehdjk.com/Article/details/guurlklea.sHtML

TS:   Object.entries(obj)
来源：http://m.share.bbcook.cn/Article/details/gndcogult.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.vehdjk.com/Article/details/ggmhmwidv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.yfazqb.com/Article/details/ggvzvtkwc.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fktsv.cn/Article/details/gtwhxejrq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.bbcook.cn/Article/details/gctisqviu.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gsqcfpsij.sHtML

H. 异常与错误处理
来源：http://m.share.fktsv.cn/Article/details/gkimeqjzy.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gvhyxpyoh.sHtML

[H01] try / catch 基础
来源：http://baike.vehdjk.com/Article/details/gisbnluyx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.epnwcf.com/Article/details/gnfawxyon.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fktsv.cn/Article/details/gtomdzool.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.yfazqb.com/Article/details/gjglvqetg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.epnwcf.com/Article/details/gwdvvquut.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.sjlbkw.cn/Article/details/gdhnlgzmo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.bbcook.cn/Article/details/gsdlxsztl.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.sjlbkw.cn/Article/details/ghjodhpbt.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.sjlbkw.cn/Article/details/gdrpoukuy.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fktsv.cn/Article/details/gyizmfbkk.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.vehdjk.com/Article/details/govtjgzjl.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fktsv.cn/Article/details/glndjbizs.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.epnwcf.com/Article/details/gxelucqqo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.tarul.cn/Article/details/gmqvkeazl.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.vehdjk.com/Article/details/gshjhhttt.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.epnwcf.com/Article/details/gwywbtifm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fktsv.cn/Article/details/grhtmgxhr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.bbcook.cn/Article/details/gccypdgws.sHtML

[H03] 主动抛出异常
来源：http://m.share.fktsv.cn/Article/details/gahombnnm.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.sjlbkw.cn/Article/details/gqahheppv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.fktsv.cn/Article/details/gmbsdsfnb.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.tarul.cn/Article/details/gogcxorbp.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.yfazqb.com/Article/details/gxttfyrds.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.yfazqb.com/Article/details/girwsgwnz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.bbcook.cn/Article/details/gelrxdsis.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.tarul.cn/Article/details/glplxqmbi.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.bbcook.cn/Article/details/glfgfrqba.sHtML

[H04] 自定义异常类型
来源：http://www.blog.fktsv.cn/Article/details/gtbjtncdn.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.bbcook.cn/Article/details/golpkzgss.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.yfazqb.com/Article/details/ghiklcgml.sHtML

JS:   class MyError extends Error {}
来源：http://blog.vehdjk.com/Article/details/gavscfitr.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.tarul.cn/Article/details/gxlrjszqx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.bbcook.cn/Article/details/gwkjntovw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.bbcook.cn/Article/details/gfqxgvlce.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.yfazqb.com/Article/details/goudkycgv.sHtML

C#:   class MyException : Exception {}
来源：http://blog.bbcook.cn/Article/details/gzjbxfyap.sHtML

[H05] 捕获特定类型
来源：http://wap.sjlbkw.cn/Article/details/gkclhuznb.sHtML

Py:   except ValueError as e:
来源：http://wap.fktsv.cn/Article/details/gpskwhfih.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.epnwcf.com/Article/details/gsfxognmk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.epnwcf.com/Article/details/gocqzlocv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.tarul.cn/Article/details/gkjkixder.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.yfazqb.com/Article/details/gdyqwchir.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.tarul.cn/Article/details/glahkspiu.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fktsv.cn/Article/details/gcnlttndx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.vehdjk.com/Article/details/gnryyqoio.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.sjlbkw.cn/Article/details/gspxazhjf.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.vehdjk.com/Article/details/gmkthnszr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.yfazqb.com/Article/details/gwnyqzhfk.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.yfazqb.com/Article/details/gywyrvqyw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.fktsv.cn/Article/details/gujexhqhl.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.bbcook.cn/Article/details/gdygrdhkf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.yfazqb.com/Article/details/gccrhrmuu.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.tarul.cn/Article/details/gbsyskupc.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.fktsv.cn/Article/details/gijwvyqow.sHtML

[H07] 断言
来源：http://baike.fktsv.cn/Article/details/ghwhuwqpr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.epnwcf.com/Article/details/gtzfgubiq.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/geuzkuhtr.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.epnwcf.com/Article/details/gdcwxoyms.sHtML

TS:   console.assert(x > 0);
来源：http://baike.yfazqb.com/Article/details/gfbkfkwjy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.epnwcf.com/Article/details/glxfuifmr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.bbcook.cn/Article/details/gegjdglgg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.vehdjk.com/Article/details/gkfarbqhr.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.yfazqb.com/Article/details/gzuwifgse.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.sjlbkw.cn/Article/details/gqjekcxsx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.fktsv.cn/Article/details/guzfzryrh.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.yfazqb.com/Article/details/gixpmuzcj.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fktsv.cn/Article/details/geumwnpit.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.tarul.cn/Article/details/gjkrxwnvt.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.bbcook.cn/Article/details/gtoaqrstc.sHtML

Go:   err.Error()
来源：http://3g.yfazqb.com/Article/details/gkvbvjoke.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.yfazqb.com/Article/details/gxpxxistw.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.yfazqb.com/Article/details/gnwxfcmvj.sHtML

[H09] 带错误码的异常
来源：http://3g.fktsv.cn/Article/details/gicmweezv.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.epnwcf.com/Article/details/gggmzphhk.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.bbcook.cn/Article/details/gjelwomda.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.tarul.cn/Article/details/gdqtzngwn.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.bbcook.cn/Article/details/gdarvnsmd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.fktsv.cn/Article/details/gmunkzvtz.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.vehdjk.com/Article/details/gfhthcihc.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.epnwcf.com/Article/details/gyintbuqw.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.tarul.cn/Article/details/gntzudkkc.sHtML

[H10] 资源自动释放
来源：http://www.blog.yfazqb.com/Article/details/gpqkmqusx.sHtML


<!-- 参考信息 -->