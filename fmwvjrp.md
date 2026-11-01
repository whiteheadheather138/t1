代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.epnwcf.com/Article/details/gtedxttlb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fktsv.cn/Article/details/gpqplqlyi.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.vehdjk.com/Article/details/gurhdiaxe.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.epnwcf.com/Article/details/gwdpwrgug.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.sjlbkw.cn/Article/details/gjjfmejps.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.bbcook.cn/Article/details/gnyiypnzy.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fktsv.cn/Article/details/gpokrtopz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.vehdjk.com/Article/details/gdgvowory.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gudqiihwv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.vehdjk.com/Article/details/gzmegczmy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fktsv.cn/Article/details/gxejtrggm.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.bbcook.cn/Article/details/gnfuwqnnr.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.tarul.cn/Article/details/gjdeoqkwf.sHtML

[F06] 删除文件
来源：http://www.share.vehdjk.com/Article/details/gylyvtrgj.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/ghczhxqbs.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gstobxbej.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fktsv.cn/Article/details/gqawvqckt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fktsv.cn/Article/details/gyvnomtwo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.sjlbkw.cn/Article/details/gpfklgiyq.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.yfazqb.com/Article/details/gilnxrnua.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gkfcjobme.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.epnwcf.com/Article/details/gbliecymh.sHtML

[F07] 创建目录（含多级）
来源：http://blog.epnwcf.com/Article/details/gapjtzfgx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.vehdjk.com/Article/details/gaqmguvme.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.yfazqb.com/Article/details/gzlxfopbf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.yfazqb.com/Article/details/galgdnvkv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.epnwcf.com/Article/details/glrcxylny.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.yfazqb.com/Article/details/grlwfifmg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.vehdjk.com/Article/details/gtebynqcd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.bbcook.cn/Article/details/ghecsamei.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.yfazqb.com/Article/details/gmnzrqdlb.sHtML

[F08] 遍历目录
来源：http://wap.bbcook.cn/Article/details/giqtpsaiu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.vehdjk.com/Article/details/gkqkwhwhi.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.yfazqb.com/Article/details/gybohptjj.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.bbcook.cn/Article/details/gxlmvhplf.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.vehdjk.com/Article/details/gzswzdqzo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fktsv.cn/Article/details/ghhjtdsvt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.epnwcf.com/Article/details/gfcdsuuyr.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fktsv.cn/Article/details/gucbagyqr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.vehdjk.com/Article/details/gwqptynyf.sHtML

[F09] 获取文件大小
来源：http://read.share.tarul.cn/Article/details/gjvilxmne.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gngdlprnp.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gftocmsgy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.tarul.cn/Article/details/gcrgeecpe.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.tarul.cn/Article/details/gcvwoyrvt.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.yfazqb.com/Article/details/gysdpdnsv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fktsv.cn/Article/details/gyfxbxqji.sHtML

Ruby: File.size("a.txt")
来源：http://blog.tarul.cn/Article/details/gbsdkwzxw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.sjlbkw.cn/Article/details/giauzyaxh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.yfazqb.com/Article/details/gvertdvij.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.vehdjk.com/Article/details/gflnblnmw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.yfazqb.com/Article/details/gdpmaashp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gxmgytlrc.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gbutbqwdd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.sjlbkw.cn/Article/details/gkczpinki.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqpomceos.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/gzifpjnij.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/govbzzvra.sHtML

[F11] 复制与移动文件
来源：http://baike.fktsv.cn/Article/details/gmyufvesl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/gkcckqnfk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.bbcook.cn/Article/details/gstimlpzd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.tarul.cn/Article/details/gqtktwmjd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.bbcook.cn/Article/details/gswnolpvm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.vehdjk.com/Article/details/gbeplrwiv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.vehdjk.com/Article/details/glfexnstw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.bbcook.cn/Article/details/gvlwmwuhl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.sjlbkw.cn/Article/details/giypbfwle.sHtML

[F12] CSV 读写
来源：http://read.share.sjlbkw.cn/Article/details/gquocmjzz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.vehdjk.com/Article/details/gqwjmgrnf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.yfazqb.com/Article/details/grbkjnwyn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.sjlbkw.cn/Article/details/ggcugqcfl.sHtML

TS:   // 同上
来源：http://www.share.vehdjk.com/Article/details/gttxhqsit.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.epnwcf.com/Article/details/goexxbkmf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.bbcook.cn/Article/details/gcrqhlyxk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.sjlbkw.cn/Article/details/ghvurqfub.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.sjlbkw.cn/Article/details/glgvppelv.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gpptvtopz.sHtML

G. 面向对象
来源：http://www.share.epnwcf.com/Article/details/grtvimebq.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/ggomlskmy.sHtML

[G01] 定义类
来源：http://www.m.share.bbcook.cn/Article/details/gyizgwyyt.sHtML

Py:   class User: pass
来源：http://baike.fktsv.cn/Article/details/gclizpman.sHtML

PHP:  class User {}
来源：http://read.share.yfazqb.com/Article/details/gktgtwplp.sHtML

JS:   class User {}
来源：http://baike.sjlbkw.cn/Article/details/gyqtxirrd.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.epnwcf.com/Article/details/gtgjbvfeg.sHtML

Java: class User {}
来源：http://read.share.epnwcf.com/Article/details/ggqwpttfc.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.epnwcf.com/Article/details/gzqlusiph.sHtML

Ruby: class User; end
来源：http://blog.yfazqb.com/Article/details/giqwhmzix.sHtML

C#:   class User {}
来源：http://wap.bbcook.cn/Article/details/grpfqilvo.sHtML

[G02] 构造函数
来源：http://www.share.bbcook.cn/Article/details/gepxyeofb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.yfazqb.com/Article/details/gsdtlwdjj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.vehdjk.com/Article/details/glukodvzv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.sjlbkw.cn/Article/details/gdxdlpsoy.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.epnwcf.com/Article/details/gpttmosbg.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fktsv.cn/Article/details/glyohunes.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.vehdjk.com/Article/details/genkugjle.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fktsv.cn/Article/details/gnofqxhay.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.tarul.cn/Article/details/gepgiyndg.sHtML

[G03] 实例属性
来源：http://3g.fktsv.cn/Article/details/gcngotfwh.sHtML

Py:   self.name = "x"
来源：http://blog.epnwcf.com/Article/details/gyadtkvbg.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.sjlbkw.cn/Article/details/grnyqqock.sHtML

JS:   this.name = "x";
来源：http://3g.sjlbkw.cn/Article/details/gsjrraiuc.sHtML

TS:   name: string = "x";
来源：http://3g.epnwcf.com/Article/details/givwdrbxa.sHtML

Java: private String name;
来源：http://m.share.bbcook.cn/Article/details/godeduxid.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fktsv.cn/Article/details/ggnyuuigp.sHtML

Ruby: @name = "x"
来源：http://read.share.yfazqb.com/Article/details/gknnltmmw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fktsv.cn/Article/details/gdxmgfwov.sHtML

[G04] 定义方法
来源：http://baike.bbcook.cn/Article/details/gmmbvadan.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fktsv.cn/Article/details/gcozqxqga.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.vehdjk.com/Article/details/gzyqgnmnd.sHtML

JS:   greet() { return this.name; }
来源：http://3g.sjlbkw.cn/Article/details/gmitmefov.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.tarul.cn/Article/details/gnelrztoh.sHtML

Java: String greet() { return name; }
来源：http://m.share.vehdjk.com/Article/details/gsarbtngy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.bbcook.cn/Article/details/gnighxvkf.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.epnwcf.com/Article/details/gakefxlgn.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fktsv.cn/Article/details/gsaflqmkc.sHtML

[G05] 继承
来源：http://www.blog.tarul.cn/Article/details/gdsdvhhir.sHtML

Py:   class Admin(User): pass
来源：http://baike.vehdjk.com/Article/details/giwoouuzx.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gdgsbmsxt.sHtML

JS:   class Admin extends User {}
来源：http://baike.bbcook.cn/Article/details/gxacqggjs.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fktsv.cn/Article/details/ghnzzlfyt.sHtML

Java: class Admin extends User {}
来源：http://mobile.yfazqb.com/Article/details/gmjfnwqgn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.sjlbkw.cn/Article/details/gedivcqlf.sHtML

Ruby: class Admin < User; end
来源：http://baike.sjlbkw.cn/Article/details/ginndckek.sHtML

C#:   class Admin : User {}
来源：http://wap.yfazqb.com/Article/details/gylxekuiq.sHtML

[G06] 重写方法
来源：http://www.share.vehdjk.com/Article/details/gkmqwdsky.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.yfazqb.com/Article/details/gfvoyzkrd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.yfazqb.com/Article/details/gxgrhpxev.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.bbcook.cn/Article/details/grpcmqmua.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/gmywtwqto.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gwoduqrte.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.sjlbkw.cn/Article/details/gtusyubvl.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.tarul.cn/Article/details/gwauwcyqt.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.vehdjk.com/Article/details/gsefexfoa.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fktsv.cn/Article/details/gsxmwmpwb.sHtML

Py:   super().greet()
来源：http://3g.bbcook.cn/Article/details/gmmvdrktr.sHtML

PHP:  parent::greet();
来源：http://www.m.share.yfazqb.com/Article/details/gqoznkrrw.sHtML

JS:   super.greet();
来源：http://read.share.sjlbkw.cn/Article/details/gghwskeoi.sHtML

TS:   super.greet();
来源：http://read.share.epnwcf.com/Article/details/gnowccphb.sHtML

Java: super.greet();
来源：http://wap.yfazqb.com/Article/details/guckejxxs.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.tarul.cn/Article/details/gyhrnbtpu.sHtML

Ruby: super
来源：http://3g.fktsv.cn/Article/details/gfipuaigp.sHtML

C#:   base.Greet();
来源：http://www.share.yfazqb.com/Article/details/gdrjyxlav.sHtML

[G08] 静态方法与属性
来源：http://baike.bbcook.cn/Article/details/glpvunijg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.vehdjk.com/Article/details/gitlsqowt.sHtML

PHP:  public static function f() {}
来源：http://3g.yfazqb.com/Article/details/gqapqblns.sHtML

JS:   static f() {}
来源：http://www.blog.fktsv.cn/Article/details/gylzjrcwv.sHtML

TS:   static f(): void {}
来源：http://3g.bbcook.cn/Article/details/gihjncxmv.sHtML

Java: static void f() {}
来源：http://baike.fktsv.cn/Article/details/gglhygrlw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.epnwcf.com/Article/details/gbzpagkzn.sHtML

Ruby: def self.f; end
来源：http://www.blog.tarul.cn/Article/details/gnqwmfxdc.sHtML

C#:   public static void F() {}
来源：http://baike.vehdjk.com/Article/details/gjviffhgb.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fktsv.cn/Article/details/gjyhhkoxu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.tarul.cn/Article/details/gwtwpmavf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.sjlbkw.cn/Article/details/gidsuemuj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.tarul.cn/Article/details/ggaqeoxvp.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.epnwcf.com/Article/details/gzleghyzl.sHtML

Java: interface Shape { double area(); }
来源：http://wap.epnwcf.com/Article/details/gccrzvcnl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fktsv.cn/Article/details/gpxoikbdj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.vehdjk.com/Article/details/ghxpaeeey.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.yfazqb.com/Article/details/ghkfaicwg.sHtML

[G10] 访问控制
来源：http://wap.vehdjk.com/Article/details/ghhxpqasj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.tarul.cn/Article/details/gimbjfrhs.sHtML

PHP:  public / protected / private
来源：http://baike.tarul.cn/Article/details/gnkukarpp.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.epnwcf.com/Article/details/gtruvfwfv.sHtML

TS:   public / protected / private
来源：http://blog.bbcook.cn/Article/details/gjklsvsmg.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.bbcook.cn/Article/details/ggpktluyg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fktsv.cn/Article/details/gwhxgfytv.sHtML

Ruby: public / protected / private
来源：http://m.share.yfazqb.com/Article/details/ghkovgora.sHtML

C#:   public / protected / private / internal
来源：http://wap.fktsv.cn/Article/details/geavkhxjc.sHtML

[G11] getter / setter
来源：http://3g.sjlbkw.cn/Article/details/gxsddluhp.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fktsv.cn/Article/details/gdslchhoa.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.epnwcf.com/Article/details/gzlgvgztk.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.tarul.cn/Article/details/gdbvmpsyy.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.tarul.cn/Article/details/gkyeajtlm.sHtML

Java: public String getName() { return name; }
来源：http://m.share.yfazqb.com/Article/details/ghyclwldh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.tarul.cn/Article/details/gnmbkogei.sHtML

Ruby: attr_accessor :name
来源：http://m.share.sjlbkw.cn/Article/details/gaurlsltf.sHtML

C#:   public string Name { get; set; }
来源：http://wap.bbcook.cn/Article/details/geubvzlyj.sHtML

[G12] 对象转字符串
来源：http://3g.tarul.cn/Article/details/gtplhiity.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.bbcook.cn/Article/details/gmuoxrqmj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.tarul.cn/Article/details/gtojlpvnh.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.tarul.cn/Article/details/gnwibhmze.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.epnwcf.com/Article/details/gvpipmmnb.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.bbcook.cn/Article/details/ggdycsqik.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.epnwcf.com/Article/details/gxjjpaysd.sHtML

Ruby: def to_s; @name; end
来源：http://baike.yfazqb.com/Article/details/gvnbviztz.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.sjlbkw.cn/Article/details/gytiwrskg.sHtML

[G13] 判断对象类型
来源：http://blog.epnwcf.com/Article/details/gswfghdlt.sHtML

Py:   isinstance(u, User)
来源：http://blog.bbcook.cn/Article/details/gydjybyal.sHtML

PHP:  $u instanceof User
来源：http://3g.bbcook.cn/Article/details/gvdsgydyv.sHtML

JS:   u instanceof User
来源：http://m.share.fktsv.cn/Article/details/gnvmphumw.sHtML

TS:   u instanceof User
来源：http://blog.tarul.cn/Article/details/gmudpzpky.sHtML

Java: u instanceof User
来源：http://www.m.share.tarul.cn/Article/details/gbqmqijqe.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.yfazqb.com/Article/details/gonleikaj.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.sjlbkw.cn/Article/details/gatjuvhoa.sHtML

C#:   u is User
来源：http://blog.vehdjk.com/Article/details/gvwtuoqyi.sHtML

[G14] 数据类 / record
来源：http://read.share.vehdjk.com/Article/details/gzngqkdsj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.bbcook.cn/Article/details/guqmmocwa.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.epnwcf.com/Article/details/gunliwcms.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.bbcook.cn/Article/details/ghbafjpzs.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.vehdjk.com/Article/details/gsdiozdis.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.vehdjk.com/Article/details/gmlervqvf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.vehdjk.com/Article/details/gythooxsq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.tarul.cn/Article/details/gmebbosum.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.bbcook.cn/Article/details/glzqjepok.sHtML

[G15] 枚举
来源：http://m.share.bbcook.cn/Article/details/gbyibfwwb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.epnwcf.com/Article/details/gzbitakoq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.sjlbkw.cn/Article/details/glcwdxqbu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.bbcook.cn/Article/details/glzqjyqxj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.epnwcf.com/Article/details/gzrrcxgtu.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fktsv.cn/Article/details/gnontxkoa.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.epnwcf.com/Article/details/gmyignqnb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.yfazqb.com/Article/details/geolfytsc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.vehdjk.com/Article/details/gmnbqsbyq.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.bbcook.cn/Article/details/gntjzscdq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.vehdjk.com/Article/details/gaytvvkdx.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.vehdjk.com/Article/details/ggbofqpbk.sHtML

JS:   Object.entries(obj)
来源：http://wap.bbcook.cn/Article/details/gmlbdofhf.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.fktsv.cn/Article/details/gawlvymrm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.vehdjk.com/Article/details/gpxxpzwve.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fktsv.cn/Article/details/gnwxcogpx.sHtML

Ruby: obj.instance_variables
来源：http://read.share.bbcook.cn/Article/details/gsyeelozl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.tarul.cn/Article/details/gbsmqlpie.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gironrfof.sHtML

H. 异常与错误处理
来源：http://www.share.sjlbkw.cn/Article/details/gotgpkyxr.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gxfqbhzmd.sHtML

[H01] try / catch 基础
来源：http://read.share.epnwcf.com/Article/details/gaiuryeat.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.epnwcf.com/Article/details/gnyzembeh.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.yfazqb.com/Article/details/gvwxrxdwq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.tarul.cn/Article/details/gkeaxvzet.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.epnwcf.com/Article/details/gywrrhabo.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.bbcook.cn/Article/details/gnnychxjo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.bbcook.cn/Article/details/guuqpifnk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.bbcook.cn/Article/details/gqvmxpyix.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fktsv.cn/Article/details/gkotafmyt.sHtML

[H02] finally / ensure 收尾
来源：http://blog.sjlbkw.cn/Article/details/gcnykbdtv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.tarul.cn/Article/details/gvsebbgke.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.yfazqb.com/Article/details/gqxokhhdb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/gycmhnysq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fktsv.cn/Article/details/gmxxbknkt.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.vehdjk.com/Article/details/gikhnhlkt.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.yfazqb.com/Article/details/gpczgihvo.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fktsv.cn/Article/details/gutdqecty.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fktsv.cn/Article/details/ghmjsaius.sHtML

[H03] 主动抛出异常
来源：http://read.share.vehdjk.com/Article/details/grktodgyp.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.bbcook.cn/Article/details/gcennpjob.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.bbcook.cn/Article/details/ggjwfquvc.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.yfazqb.com/Article/details/gohdrfxsj.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.yfazqb.com/Article/details/gviwviiuy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.bbcook.cn/Article/details/gwyhhqewk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.fktsv.cn/Article/details/grkfhdywc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.sjlbkw.cn/Article/details/gavswmegu.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/ghxiztmag.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.vehdjk.com/Article/details/gvbxbibcu.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.fktsv.cn/Article/details/gemnumnkm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.sjlbkw.cn/Article/details/gzqjbojma.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.yfazqb.com/Article/details/gyrjmuivg.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fktsv.cn/Article/details/glswzsnvd.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.tarul.cn/Article/details/glshoqvpb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.fktsv.cn/Article/details/gissdhftg.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.sjlbkw.cn/Article/details/gtwbbbgmd.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.tarul.cn/Article/details/gsoyidmfd.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gmdhdzyib.sHtML

Py:   except ValueError as e:
来源：http://m.share.epnwcf.com/Article/details/gzdxrsyqs.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fktsv.cn/Article/details/gqzqafqdd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.bbcook.cn/Article/details/gcrrfsrdt.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.bbcook.cn/Article/details/glnkvhyyy.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/ghbwrsxlv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fktsv.cn/Article/details/gaxsarpde.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.bbcook.cn/Article/details/gpemrdmmf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.epnwcf.com/Article/details/gsixvcaqj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.bbcook.cn/Article/details/gpfgjcikv.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.vehdjk.com/Article/details/gadkegify.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.epnwcf.com/Article/details/gygdbannd.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.sjlbkw.cn/Article/details/ggbfwuvcs.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.sjlbkw.cn/Article/details/gkljuguht.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.yfazqb.com/Article/details/gawkwyahy.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.bbcook.cn/Article/details/ghustkupl.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.vehdjk.com/Article/details/gpucgulht.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.bbcook.cn/Article/details/gslqpbbrz.sHtML

[H07] 断言
来源：http://www.m.share.epnwcf.com/Article/details/gleihiibc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.vehdjk.com/Article/details/gujhbjglg.sHtML

PHP:  assert($x > 0);
来源：http://wap.vehdjk.com/Article/details/gyosysxzb.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.tarul.cn/Article/details/gqssvvczx.sHtML

TS:   console.assert(x > 0);
来源：http://blog.tarul.cn/Article/details/gnmoufdif.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.epnwcf.com/Article/details/gcbmagxly.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.sjlbkw.cn/Article/details/gkpeqndzm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.sjlbkw.cn/Article/details/giipposdv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.fktsv.cn/Article/details/gutqmdfbp.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.vehdjk.com/Article/details/ghifvorvd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.epnwcf.com/Article/details/gmzncjjmh.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.vehdjk.com/Article/details/gkbplbbwi.sHtML

JS:   e.message;  e.stack
来源：http://wap.bbcook.cn/Article/details/ghvscfljo.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.sjlbkw.cn/Article/details/gqgvnvntv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.sjlbkw.cn/Article/details/gumumvdzy.sHtML

Go:   err.Error()
来源：http://baike.vehdjk.com/Article/details/gptdncqfm.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.fktsv.cn/Article/details/guooddcxo.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.tarul.cn/Article/details/gqsnozatg.sHtML

[H09] 带错误码的异常
来源：http://www.share.vehdjk.com/Article/details/gisfcffur.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fktsv.cn/Article/details/gesmadvtc.sHtML


<!-- 参考信息 -->