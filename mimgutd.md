代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://www.blog.sjlbkw.cn/Article/details/gqafsqoin.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.vehdjk.com/Article/details/ggvirophb.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gtdtymzhy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gxrttfbzm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.epnwcf.com/Article/details/gdscsdhms.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.sjlbkw.cn/Article/details/gzoawnggt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.sjlbkw.cn/Article/details/gcmtofuff.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gdemmahnt.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.tarul.cn/Article/details/gsbeecgvk.sHtML

[F06] 删除文件
来源：http://m.share.yfazqb.com/Article/details/gohbirroe.sHtML

Py:   os.remove("a.txt")
来源：http://blog.yfazqb.com/Article/details/gurqadrvo.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gzzqrgegc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.tarul.cn/Article/details/gdybipmji.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.bbcook.cn/Article/details/gzlwirjug.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.bbcook.cn/Article/details/gfdduynek.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.tarul.cn/Article/details/gsrsgbcgp.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gpgrxsbuh.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.bbcook.cn/Article/details/gsajefumv.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.epnwcf.com/Article/details/gtcplpdle.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.yfazqb.com/Article/details/gvwdiscob.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.bbcook.cn/Article/details/gliopuajl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.sjlbkw.cn/Article/details/gqnotyjdu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.vehdjk.com/Article/details/giyzqrkfo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fktsv.cn/Article/details/glvnjqore.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.yfazqb.com/Article/details/gmtdbctum.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.sjlbkw.cn/Article/details/gjjhudtqk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.yfazqb.com/Article/details/gqwensrwj.sHtML

[F08] 遍历目录
来源：http://baike.bbcook.cn/Article/details/gkbwdpimq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.yfazqb.com/Article/details/gptwtipzs.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.sjlbkw.cn/Article/details/gqvpxzuic.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.vehdjk.com/Article/details/gbnhifdrh.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.epnwcf.com/Article/details/glcvxnthg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.sjlbkw.cn/Article/details/gujzsshhi.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.epnwcf.com/Article/details/gfwfkoscr.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fktsv.cn/Article/details/gihuzajrv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.yfazqb.com/Article/details/gmafefxjr.sHtML

[F09] 获取文件大小
来源：http://read.share.fktsv.cn/Article/details/gcggffsvr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.vehdjk.com/Article/details/glzpltfvo.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gnscomoml.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.epnwcf.com/Article/details/gkwdodrpv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.vehdjk.com/Article/details/gleuknwpg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.vehdjk.com/Article/details/gsribpjoy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.epnwcf.com/Article/details/gvdikinks.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gzddszrei.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fktsv.cn/Article/details/gbanmmgtm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.tarul.cn/Article/details/ghzzuvuvm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/gmpnrsfbd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.epnwcf.com/Article/details/glmpukyha.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gyrnqjfvy.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gidkrbgfo.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.tarul.cn/Article/details/gzxeflmdr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/gtptpqodc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/ghciiznhc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fktsv.cn/Article/details/gyksgmqrl.sHtML

[F11] 复制与移动文件
来源：http://baike.fktsv.cn/Article/details/gqymzxsmr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gacvzpcfy.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fktsv.cn/Article/details/gulqfmftw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/ghmnkqfjg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gvzfpjpyb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.epnwcf.com/Article/details/gydvwlxgf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.epnwcf.com/Article/details/gawtgzrti.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.sjlbkw.cn/Article/details/gyfgolrqu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.bbcook.cn/Article/details/gpbpjlhvq.sHtML

[F12] CSV 读写
来源：http://m.share.tarul.cn/Article/details/gknunrhxg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.vehdjk.com/Article/details/gnuadfvkr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.epnwcf.com/Article/details/gaqpdtjuu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.yfazqb.com/Article/details/gcauqozvm.sHtML

TS:   // 同上
来源：http://m.share.tarul.cn/Article/details/gbzjlxsck.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.epnwcf.com/Article/details/gzqayakld.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.epnwcf.com/Article/details/gaohmqzuo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.vehdjk.com/Article/details/gplcbsclz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.bbcook.cn/Article/details/gaqfxspgi.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gwijwyzdr.sHtML

G. 面向对象
来源：http://www.blog.bbcook.cn/Article/details/gqkrnmmmf.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gcafjtkni.sHtML

[G01] 定义类
来源：http://www.share.yfazqb.com/Article/details/gifasaycp.sHtML

Py:   class User: pass
来源：http://www.share.vehdjk.com/Article/details/guwoeiykb.sHtML

PHP:  class User {}
来源：http://wap.tarul.cn/Article/details/gbfxziwxj.sHtML

JS:   class User {}
来源：http://read.share.vehdjk.com/Article/details/gaburgklo.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.vehdjk.com/Article/details/ghsfcpjlj.sHtML

Java: class User {}
来源：http://read.share.tarul.cn/Article/details/gzphozwao.sHtML

Go:   type User struct { Name string }
来源：http://3g.epnwcf.com/Article/details/grweaxlpn.sHtML

Ruby: class User; end
来源：http://www.share.epnwcf.com/Article/details/gfzlnxidd.sHtML

C#:   class User {}
来源：http://blog.tarul.cn/Article/details/ggeoinzlz.sHtML

[G02] 构造函数
来源：http://wap.sjlbkw.cn/Article/details/gllmqalrr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.sjlbkw.cn/Article/details/giamtupcp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.sjlbkw.cn/Article/details/geqnpfjvn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.epnwcf.com/Article/details/gnlcylbcu.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.sjlbkw.cn/Article/details/gawqcytps.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.tarul.cn/Article/details/goxcmvrxx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.tarul.cn/Article/details/gmsrrjohr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.yfazqb.com/Article/details/gafsrfcjh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fktsv.cn/Article/details/gftiihuws.sHtML

[G03] 实例属性
来源：http://read.share.fktsv.cn/Article/details/grstmcski.sHtML

Py:   self.name = "x"
来源：http://read.share.fktsv.cn/Article/details/gkbihpvdo.sHtML

PHP:  public string $name = "x";
来源：http://baike.sjlbkw.cn/Article/details/gfxpqwncn.sHtML

JS:   this.name = "x";
来源：http://3g.sjlbkw.cn/Article/details/ggdssjshy.sHtML

TS:   name: string = "x";
来源：http://mobile.tarul.cn/Article/details/gtpairkvp.sHtML

Java: private String name;
来源：http://wap.vehdjk.com/Article/details/grfgzneub.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.yfazqb.com/Article/details/gbogzlzik.sHtML

Ruby: @name = "x"
来源：http://wap.yfazqb.com/Article/details/glnkxatjf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fktsv.cn/Article/details/gdpdbjuae.sHtML

[G04] 定义方法
来源：http://m.share.epnwcf.com/Article/details/gmpxllnhj.sHtML

Py:   def greet(self): return self.name
来源：http://wap.sjlbkw.cn/Article/details/gajocckeb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.vehdjk.com/Article/details/gluhmetuh.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fktsv.cn/Article/details/grxudxwqu.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.epnwcf.com/Article/details/gwzlwqkyg.sHtML

Java: String greet() { return name; }
来源：http://wap.tarul.cn/Article/details/gjkjnllck.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.vehdjk.com/Article/details/giqxxatkl.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.vehdjk.com/Article/details/gdhrivnat.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.vehdjk.com/Article/details/gldrqjpjv.sHtML

[G05] 继承
来源：http://blog.vehdjk.com/Article/details/gindkvwqh.sHtML

Py:   class Admin(User): pass
来源：http://baike.epnwcf.com/Article/details/gtbsuamkb.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.yfazqb.com/Article/details/guunsqhny.sHtML

JS:   class Admin extends User {}
来源：http://wap.epnwcf.com/Article/details/gfttnisvv.sHtML

TS:   class Admin extends User {}
来源：http://read.share.vehdjk.com/Article/details/gkichnzdu.sHtML

Java: class Admin extends User {}
来源：http://read.share.vehdjk.com/Article/details/ggzdcorjw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.tarul.cn/Article/details/gaapviktk.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.epnwcf.com/Article/details/gcgkqiivo.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.bbcook.cn/Article/details/gbjpbasun.sHtML

[G06] 重写方法
来源：http://3g.bbcook.cn/Article/details/gfrbgslhp.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fktsv.cn/Article/details/gaqibsktk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.yfazqb.com/Article/details/gsmaxoxhx.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/gkqyzouqw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.yfazqb.com/Article/details/gdbguhliw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fktsv.cn/Article/details/gogbmixot.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.vehdjk.com/Article/details/gwqjwmoza.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.bbcook.cn/Article/details/gffxpkuho.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.epnwcf.com/Article/details/geqldlpmb.sHtML

[G07] 调用父类方法
来源：http://www.m.share.bbcook.cn/Article/details/gklcguvjc.sHtML

Py:   super().greet()
来源：http://3g.bbcook.cn/Article/details/gtjyddgtl.sHtML

PHP:  parent::greet();
来源：http://read.share.bbcook.cn/Article/details/glfxplspc.sHtML

JS:   super.greet();
来源：http://www.m.share.vehdjk.com/Article/details/gynfvjdaw.sHtML

TS:   super.greet();
来源：http://read.share.fktsv.cn/Article/details/gmodzroxq.sHtML

Java: super.greet();
来源：http://www.m.share.fktsv.cn/Article/details/giqwzfxlg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.bbcook.cn/Article/details/gfxypnhfu.sHtML

Ruby: super
来源：http://www.blog.vehdjk.com/Article/details/gpjdckyaf.sHtML

C#:   base.Greet();
来源：http://m.share.vehdjk.com/Article/details/gsmzpfikq.sHtML

[G08] 静态方法与属性
来源：http://3g.vehdjk.com/Article/details/ghsoznsje.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.bbcook.cn/Article/details/gbyxuvoca.sHtML

PHP:  public static function f() {}
来源：http://mobile.bbcook.cn/Article/details/gfbbvynmt.sHtML

JS:   static f() {}
来源：http://wap.tarul.cn/Article/details/gnyfowijy.sHtML

TS:   static f(): void {}
来源：http://www.blog.fktsv.cn/Article/details/ghppeygwc.sHtML

Java: static void f() {}
来源：http://mobile.bbcook.cn/Article/details/gzpcjaltr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.epnwcf.com/Article/details/gudhxigpj.sHtML

Ruby: def self.f; end
来源：http://read.share.epnwcf.com/Article/details/goechcrct.sHtML

C#:   public static void F() {}
来源：http://wap.sjlbkw.cn/Article/details/glvvqsldn.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.vehdjk.com/Article/details/gqpepzmpn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.bbcook.cn/Article/details/gfhgtzymh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.epnwcf.com/Article/details/gzlsjhvyl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.vehdjk.com/Article/details/gzwlkgctz.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.sjlbkw.cn/Article/details/guevkcblo.sHtML

Java: interface Shape { double area(); }
来源：http://wap.epnwcf.com/Article/details/ghcflxkjw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.epnwcf.com/Article/details/gfjajagqp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.yfazqb.com/Article/details/gnguchtqp.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.tarul.cn/Article/details/glkpqmnfd.sHtML

[G10] 访问控制
来源：http://baike.vehdjk.com/Article/details/gowaeuydu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.yfazqb.com/Article/details/gczfffwis.sHtML

PHP:  public / protected / private
来源：http://www.m.share.epnwcf.com/Article/details/gwtnbkdbh.sHtML

JS:   #private 字段；其余公开
来源：http://baike.epnwcf.com/Article/details/gqicndpnp.sHtML

TS:   public / protected / private
来源：http://www.share.vehdjk.com/Article/details/gnesplwos.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.epnwcf.com/Article/details/gujvucpxz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.vehdjk.com/Article/details/goqwdtnnb.sHtML

Ruby: public / protected / private
来源：http://www.m.share.epnwcf.com/Article/details/glysacxlr.sHtML

C#:   public / protected / private / internal
来源：http://mobile.vehdjk.com/Article/details/gzbbjvdrr.sHtML

[G11] getter / setter
来源：http://baike.tarul.cn/Article/details/gtbvkhnjt.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.epnwcf.com/Article/details/gcvfiqmus.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.vehdjk.com/Article/details/ghvvczxia.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.tarul.cn/Article/details/gvknckbwh.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.bbcook.cn/Article/details/gczbxkckq.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/gzsexbkwl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.tarul.cn/Article/details/gydcgmeop.sHtML

Ruby: attr_accessor :name
来源：http://baike.fktsv.cn/Article/details/gbjmxegoh.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.epnwcf.com/Article/details/gjhogquua.sHtML

[G12] 对象转字符串
来源：http://www.blog.vehdjk.com/Article/details/gxqtkupsw.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fktsv.cn/Article/details/gosvjxvrl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.bbcook.cn/Article/details/grynmnxlt.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fktsv.cn/Article/details/grrdvsqyv.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.sjlbkw.cn/Article/details/gkqpikoiz.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/gvcpupkku.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.vehdjk.com/Article/details/glixezdcp.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.vehdjk.com/Article/details/gvprxmxeq.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.vehdjk.com/Article/details/gsrbbshrk.sHtML

[G13] 判断对象类型
来源：http://www.blog.epnwcf.com/Article/details/geqpxjsdq.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.vehdjk.com/Article/details/gdufxxwqu.sHtML

PHP:  $u instanceof User
来源：http://read.share.bbcook.cn/Article/details/glprosiao.sHtML

JS:   u instanceof User
来源：http://www.share.tarul.cn/Article/details/guoenzibd.sHtML

TS:   u instanceof User
来源：http://read.share.vehdjk.com/Article/details/gwndxlvke.sHtML

Java: u instanceof User
来源：http://blog.tarul.cn/Article/details/ghoikcfdg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.vehdjk.com/Article/details/gzxxdigfj.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.vehdjk.com/Article/details/gsxtqqcft.sHtML

C#:   u is User
来源：http://read.share.epnwcf.com/Article/details/gyercnqpg.sHtML

[G14] 数据类 / record
来源：http://mobile.yfazqb.com/Article/details/ghkdrslnx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.sjlbkw.cn/Article/details/gnxiuvogp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fktsv.cn/Article/details/ghfebupwn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.epnwcf.com/Article/details/gicfwpgvx.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.bbcook.cn/Article/details/gecmmnfdd.sHtML

Java: record User(String name, int age) {}
来源：http://3g.epnwcf.com/Article/details/gxmverxag.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.sjlbkw.cn/Article/details/ggzpaizxh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.bbcook.cn/Article/details/giprwwnwi.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.vehdjk.com/Article/details/gaewlgqur.sHtML

[G15] 枚举
来源：http://wap.epnwcf.com/Article/details/gbmolrrxi.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.tarul.cn/Article/details/gxkmpuiia.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.tarul.cn/Article/details/ghxbwxjqs.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.vehdjk.com/Article/details/gaveldpvz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.yfazqb.com/Article/details/gtggfcqqr.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.vehdjk.com/Article/details/gsbsyrdns.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.sjlbkw.cn/Article/details/guihbhjhh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.tarul.cn/Article/details/gdiptnqvg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.sjlbkw.cn/Article/details/gvywxatxk.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.sjlbkw.cn/Article/details/grwmdudow.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.sjlbkw.cn/Article/details/gridmwikk.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.yfazqb.com/Article/details/gixwqxnog.sHtML

JS:   Object.entries(obj)
来源：http://3g.epnwcf.com/Article/details/gqckkvfoc.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.bbcook.cn/Article/details/gdzylkayf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.yfazqb.com/Article/details/gogvsibbp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.vehdjk.com/Article/details/gomhzpqkn.sHtML

Ruby: obj.instance_variables
来源：http://3g.sjlbkw.cn/Article/details/glsriqwzo.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.tarul.cn/Article/details/gslcadcsr.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gjqxbwkhw.sHtML

H. 异常与错误处理
来源：http://read.share.tarul.cn/Article/details/grneyxmog.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gaczwocsv.sHtML

[H01] try / catch 基础
来源：http://www.share.fktsv.cn/Article/details/gtiefbtog.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.yfazqb.com/Article/details/gqvzoqzew.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.yfazqb.com/Article/details/gmnggusfd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fktsv.cn/Article/details/guuijinnz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.vehdjk.com/Article/details/gxlbjqngb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.vehdjk.com/Article/details/gayonwfis.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.vehdjk.com/Article/details/gyohraspx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.bbcook.cn/Article/details/goqxoicvm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.epnwcf.com/Article/details/gvdzoqckp.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.bbcook.cn/Article/details/gfpwhvouk.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.yfazqb.com/Article/details/gzuwqmcdk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.tarul.cn/Article/details/gtzxkvxtq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/gaykpffda.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.sjlbkw.cn/Article/details/gckcoszvx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/gmrozsotl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.bbcook.cn/Article/details/givqzxtti.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fktsv.cn/Article/details/gcewsjjgr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.yfazqb.com/Article/details/gmnmbcwaj.sHtML

[H03] 主动抛出异常
来源：http://read.share.bbcook.cn/Article/details/gfgcicmrh.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.sjlbkw.cn/Article/details/ggwsutbar.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.epnwcf.com/Article/details/gcxjznjrf.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.tarul.cn/Article/details/gifslsaxm.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.sjlbkw.cn/Article/details/gilyjmihx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.fktsv.cn/Article/details/gqhdqsetq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.yfazqb.com/Article/details/gcfxxmamn.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.bbcook.cn/Article/details/gnaltgeng.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fktsv.cn/Article/details/gvuawaeap.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.epnwcf.com/Article/details/gebobbnoq.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.bbcook.cn/Article/details/gpdquinxz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.yfazqb.com/Article/details/gbpnzdbaw.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.epnwcf.com/Article/details/gpzjbfxhf.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.bbcook.cn/Article/details/gqwouhmti.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.bbcook.cn/Article/details/goynkpcri.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.yfazqb.com/Article/details/gdeuffpqb.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.epnwcf.com/Article/details/ghwamjglt.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fktsv.cn/Article/details/gplcffheo.sHtML

[H05] 捕获特定类型
来源：http://3g.bbcook.cn/Article/details/gjuwfshqd.sHtML

Py:   except ValueError as e:
来源：http://3g.vehdjk.com/Article/details/gdzriyvim.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.vehdjk.com/Article/details/gkkbgdnkx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.bbcook.cn/Article/details/goqxfvkso.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fktsv.cn/Article/details/gzxuuiwgo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.bbcook.cn/Article/details/gpipltxuk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.vehdjk.com/Article/details/gcorhskqh.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.tarul.cn/Article/details/gyodwhpou.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.sjlbkw.cn/Article/details/gwuinmufq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fktsv.cn/Article/details/grwywtunr.sHtML

Py:   value = d.get("k") or default
来源：http://3g.fktsv.cn/Article/details/gdrbfmiyt.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.epnwcf.com/Article/details/grucwberu.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.bbcook.cn/Article/details/gjpfepghn.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.bbcook.cn/Article/details/goadooeui.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.sjlbkw.cn/Article/details/gqcudmtdj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.epnwcf.com/Article/details/gmchdmjct.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.tarul.cn/Article/details/gzgchjlyd.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.tarul.cn/Article/details/gkfqeymiz.sHtML

[H07] 断言
来源：http://blog.vehdjk.com/Article/details/gjsjtjwik.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.vehdjk.com/Article/details/gnaxrseyi.sHtML

PHP:  assert($x > 0);
来源：http://3g.yfazqb.com/Article/details/glpibbnly.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.tarul.cn/Article/details/gbnzzxyof.sHtML

TS:   console.assert(x > 0);
来源：http://wap.vehdjk.com/Article/details/gwstjoiyv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.yfazqb.com/Article/details/gluswoltz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.vehdjk.com/Article/details/gcpsfmcft.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.vehdjk.com/Article/details/gjupwcvrg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.yfazqb.com/Article/details/gfwvsbita.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.epnwcf.com/Article/details/geraxyngn.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.bbcook.cn/Article/details/ggekafbnc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.bbcook.cn/Article/details/gbkmydzuu.sHtML

JS:   e.message;  e.stack
来源：http://m.share.epnwcf.com/Article/details/gqlilwfva.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.tarul.cn/Article/details/gluigqvku.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.tarul.cn/Article/details/gsjyeprft.sHtML

Go:   err.Error()
来源：http://mobile.tarul.cn/Article/details/gndtllbnz.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.fktsv.cn/Article/details/gdwqbuqrp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.bbcook.cn/Article/details/gmmehzbii.sHtML

[H09] 带错误码的异常
来源：http://baike.sjlbkw.cn/Article/details/gdjjcvcwp.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.tarul.cn/Article/details/gnglvsgwq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.bbcook.cn/Article/details/gdbavrtkx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.vehdjk.com/Article/details/gdyhxkckp.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.tarul.cn/Article/details/guyxidfbs.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.epnwcf.com/Article/details/gjdcdwktq.sHtML


<!-- 参考信息 -->