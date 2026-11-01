代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://m.share.bbcook.cn/Article/details/gwwhdbnpg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fktsv.cn/Article/details/gigupkyxv.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fktsv.cn/Article/details/gmlbsoavm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gadlvdish.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.yfazqb.com/Article/details/gxdgnxpke.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.yfazqb.com/Article/details/gejjntoap.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.yfazqb.com/Article/details/guxrcjigw.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gbeuhsjla.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gyyzrtnet.sHtML

[F06] 删除文件
来源：http://3g.bbcook.cn/Article/details/gwjxhlhmu.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.yfazqb.com/Article/details/glzudtczi.sHtML

PHP:  unlink("a.txt");
来源：http://blog.vehdjk.com/Article/details/ggyqyxhoh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.tarul.cn/Article/details/guvdizsge.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.bbcook.cn/Article/details/gzaidcmjq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fktsv.cn/Article/details/gvmhirbuk.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.tarul.cn/Article/details/gyaivwmvu.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gmwknuzwy.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gxnwtlvpg.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.epnwcf.com/Article/details/gdslcqfim.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.epnwcf.com/Article/details/gnjczmgdz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fktsv.cn/Article/details/gaojjxsud.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fktsv.cn/Article/details/gqdqqlsxz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.bbcook.cn/Article/details/grzhdbeil.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fktsv.cn/Article/details/grmotuteh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.epnwcf.com/Article/details/ghaaqdsqv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.yfazqb.com/Article/details/gnammiphy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.yfazqb.com/Article/details/gliwxxxlt.sHtML

[F08] 遍历目录
来源：http://3g.bbcook.cn/Article/details/glzbvtnxr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fktsv.cn/Article/details/ggafvsgjy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.bbcook.cn/Article/details/gcnebjcfu.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.yfazqb.com/Article/details/gduuqbypz.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.vehdjk.com/Article/details/gqflgraam.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.yfazqb.com/Article/details/ghljrfgoh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fktsv.cn/Article/details/gkqszitgm.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fktsv.cn/Article/details/gioqbwxrr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fktsv.cn/Article/details/gitdkaopq.sHtML

[F09] 获取文件大小
来源：http://read.share.yfazqb.com/Article/details/geootuapp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.tarul.cn/Article/details/gfitctznp.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gjouigrun.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.yfazqb.com/Article/details/gniknlkhb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fktsv.cn/Article/details/gurjbbegn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.epnwcf.com/Article/details/glmwozylv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.epnwcf.com/Article/details/gfsleguiu.sHtML

Ruby: File.size("a.txt")
来源：http://3g.epnwcf.com/Article/details/gcpaphgvs.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.tarul.cn/Article/details/gafoazxpo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.vehdjk.com/Article/details/gcacfrgzb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gibgvkfij.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gjaqqjdie.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gvdtqnhuw.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gfekcvhwz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fktsv.cn/Article/details/gzvsqnamz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gmrmotycc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gkugjedrt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/gocsnbunp.sHtML

[F11] 复制与移动文件
来源：http://read.share.tarul.cn/Article/details/gwbvlecsl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gfmbnnuen.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.vehdjk.com/Article/details/gsgzianwz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.yfazqb.com/Article/details/gplihvrkj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.yfazqb.com/Article/details/ghhsewqdr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fktsv.cn/Article/details/grnxfjapf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.vehdjk.com/Article/details/gcwuobvqw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fktsv.cn/Article/details/gbgwerdno.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.yfazqb.com/Article/details/gxtpspbvf.sHtML

[F12] CSV 读写
来源：http://3g.sjlbkw.cn/Article/details/gnqwzcfnt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.yfazqb.com/Article/details/gifnldlsk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.tarul.cn/Article/details/gkujnmaqt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.tarul.cn/Article/details/gtvynyeoe.sHtML

TS:   // 同上
来源：http://m.share.epnwcf.com/Article/details/gwtrnchjt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.yfazqb.com/Article/details/gyzpvgbgd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.sjlbkw.cn/Article/details/gaevzefnn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.yfazqb.com/Article/details/gcwksxfhp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fktsv.cn/Article/details/gxewpuglt.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gzpswcrss.sHtML

G. 面向对象
来源：http://www.m.share.epnwcf.com/Article/details/geohecxnh.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gltzkdalr.sHtML

[G01] 定义类
来源：http://read.share.bbcook.cn/Article/details/ggwmrowjl.sHtML

Py:   class User: pass
来源：http://read.share.vehdjk.com/Article/details/gnkbnlqje.sHtML

PHP:  class User {}
来源：http://m.share.vehdjk.com/Article/details/gnfjuueqw.sHtML

JS:   class User {}
来源：http://www.m.share.yfazqb.com/Article/details/ggpmthsre.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.epnwcf.com/Article/details/gmfevxmcw.sHtML

Java: class User {}
来源：http://read.share.epnwcf.com/Article/details/gmukbvxqk.sHtML

Go:   type User struct { Name string }
来源：http://www.share.sjlbkw.cn/Article/details/gzmoqhoyq.sHtML

Ruby: class User; end
来源：http://mobile.sjlbkw.cn/Article/details/gtsdmrsmy.sHtML

C#:   class User {}
来源：http://read.share.fktsv.cn/Article/details/gtpfujlok.sHtML

[G02] 构造函数
来源：http://www.share.tarul.cn/Article/details/gbxonjgag.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.bbcook.cn/Article/details/goqcbzikv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fktsv.cn/Article/details/guojcrxmp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fktsv.cn/Article/details/gvfppfwfc.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.vehdjk.com/Article/details/gzsyzxdbh.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fktsv.cn/Article/details/gtlsmoxtj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.yfazqb.com/Article/details/gxtfnugmn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.epnwcf.com/Article/details/gqrgznobz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fktsv.cn/Article/details/gnzohfqck.sHtML

[G03] 实例属性
来源：http://3g.sjlbkw.cn/Article/details/gbfurujig.sHtML

Py:   self.name = "x"
来源：http://read.share.sjlbkw.cn/Article/details/gjoqdmxqh.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.tarul.cn/Article/details/gylasysol.sHtML

JS:   this.name = "x";
来源：http://www.m.share.epnwcf.com/Article/details/grevgrbnm.sHtML

TS:   name: string = "x";
来源：http://www.m.share.vehdjk.com/Article/details/gjpxwcpyo.sHtML

Java: private String name;
来源：http://read.share.bbcook.cn/Article/details/gewcfkzwy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.vehdjk.com/Article/details/gxfuxlnme.sHtML

Ruby: @name = "x"
来源：http://www.m.share.vehdjk.com/Article/details/gigsrlnyx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.tarul.cn/Article/details/gfrptknaz.sHtML

[G04] 定义方法
来源：http://3g.bbcook.cn/Article/details/gzeyeadvd.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.epnwcf.com/Article/details/gugkbizmt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.sjlbkw.cn/Article/details/gdjoelaek.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.epnwcf.com/Article/details/gvubzskol.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.yfazqb.com/Article/details/gkvqcpcmr.sHtML

Java: String greet() { return name; }
来源：http://3g.sjlbkw.cn/Article/details/ggirvpgva.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.tarul.cn/Article/details/grausqwmp.sHtML

Ruby: def greet; @name; end
来源：http://www.share.sjlbkw.cn/Article/details/genhmcrbx.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.yfazqb.com/Article/details/gqzxtbuek.sHtML

[G05] 继承
来源：http://www.blog.bbcook.cn/Article/details/gysaysntn.sHtML

Py:   class Admin(User): pass
来源：http://read.share.sjlbkw.cn/Article/details/gcpmyfbey.sHtML

PHP:  class Admin extends User {}
来源：http://wap.epnwcf.com/Article/details/gpaxetifd.sHtML

JS:   class Admin extends User {}
来源：http://wap.epnwcf.com/Article/details/ghaydxbwg.sHtML

TS:   class Admin extends User {}
来源：http://read.share.tarul.cn/Article/details/gwinnkbyj.sHtML

Java: class Admin extends User {}
来源：http://www.blog.epnwcf.com/Article/details/gjzjooqpw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.sjlbkw.cn/Article/details/guobyokty.sHtML

Ruby: class Admin < User; end
来源：http://3g.yfazqb.com/Article/details/gonxzgjyl.sHtML

C#:   class Admin : User {}
来源：http://www.share.tarul.cn/Article/details/gihgvxbsj.sHtML

[G06] 重写方法
来源：http://www.m.share.vehdjk.com/Article/details/gydjikkxe.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.tarul.cn/Article/details/geefqbnia.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.yfazqb.com/Article/details/gfsyzujce.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.yfazqb.com/Article/details/gaxjuwcxz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.yfazqb.com/Article/details/gpcyozdrk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.vehdjk.com/Article/details/gtueqfknj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.epnwcf.com/Article/details/gifjgxvqm.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.yfazqb.com/Article/details/gxzodgrvb.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.sjlbkw.cn/Article/details/goxnmqmka.sHtML

[G07] 调用父类方法
来源：http://read.share.tarul.cn/Article/details/gopprgdbd.sHtML

Py:   super().greet()
来源：http://mobile.sjlbkw.cn/Article/details/gskvopobt.sHtML

PHP:  parent::greet();
来源：http://m.share.yfazqb.com/Article/details/gbhxhcxzk.sHtML

JS:   super.greet();
来源：http://mobile.tarul.cn/Article/details/gsrdexuse.sHtML

TS:   super.greet();
来源：http://www.blog.bbcook.cn/Article/details/ghhxebrhp.sHtML

Java: super.greet();
来源：http://blog.fktsv.cn/Article/details/gnazjqcvt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fktsv.cn/Article/details/gdkitcefs.sHtML

Ruby: super
来源：http://www.m.share.sjlbkw.cn/Article/details/giwitlnep.sHtML

C#:   base.Greet();
来源：http://www.m.share.vehdjk.com/Article/details/gulzjehma.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.epnwcf.com/Article/details/gvijrxkzt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.tarul.cn/Article/details/gqjyetfdu.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.epnwcf.com/Article/details/gkkzwwctp.sHtML

JS:   static f() {}
来源：http://blog.bbcook.cn/Article/details/gqocgclmd.sHtML

TS:   static f(): void {}
来源：http://wap.yfazqb.com/Article/details/gheoxblrt.sHtML

Java: static void f() {}
来源：http://3g.yfazqb.com/Article/details/grlnjdpfd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.vehdjk.com/Article/details/gwfgyzdrj.sHtML

Ruby: def self.f; end
来源：http://3g.sjlbkw.cn/Article/details/gpkphuiab.sHtML

C#:   public static void F() {}
来源：http://www.share.epnwcf.com/Article/details/gwkuhwghc.sHtML

[G09] 接口 / 抽象类
来源：http://3g.yfazqb.com/Article/details/gugxuszap.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.vehdjk.com/Article/details/ghvdmfytc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.tarul.cn/Article/details/gypgcddtt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.bbcook.cn/Article/details/gxpgvdqww.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.vehdjk.com/Article/details/gyybqpqwa.sHtML

Java: interface Shape { double area(); }
来源：http://baike.bbcook.cn/Article/details/ggcjhcfel.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.vehdjk.com/Article/details/goynubiin.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.epnwcf.com/Article/details/gbtmzyjii.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.yfazqb.com/Article/details/gmrnuzsya.sHtML

[G10] 访问控制
来源：http://3g.tarul.cn/Article/details/genuyoujn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.tarul.cn/Article/details/gryyodrqo.sHtML

PHP:  public / protected / private
来源：http://www.share.sjlbkw.cn/Article/details/geyzxdddv.sHtML

JS:   #private 字段；其余公开
来源：http://wap.sjlbkw.cn/Article/details/gwqlhgphf.sHtML

TS:   public / protected / private
来源：http://3g.yfazqb.com/Article/details/gvqwqzajg.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fktsv.cn/Article/details/ghfvfakok.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.sjlbkw.cn/Article/details/grhvigfoz.sHtML

Ruby: public / protected / private
来源：http://mobile.yfazqb.com/Article/details/gxujeshvw.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.tarul.cn/Article/details/gaunvyblu.sHtML

[G11] getter / setter
来源：http://3g.sjlbkw.cn/Article/details/gbkntmzbh.sHtML

Py:   @property 与 @x.setter
来源：http://baike.yfazqb.com/Article/details/ghgmvquen.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.yfazqb.com/Article/details/gobjpdctc.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.vehdjk.com/Article/details/gnmbsmgpu.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.epnwcf.com/Article/details/gsaslresr.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.tarul.cn/Article/details/guapyxjsw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.bbcook.cn/Article/details/gatwsweaz.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.sjlbkw.cn/Article/details/ghphbtftk.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fktsv.cn/Article/details/gddnrqvtf.sHtML

[G12] 对象转字符串
来源：http://mobile.bbcook.cn/Article/details/gwjiysmxj.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.tarul.cn/Article/details/gfjqajyrj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.epnwcf.com/Article/details/gjidnyijl.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.epnwcf.com/Article/details/gzdiuxxwj.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.epnwcf.com/Article/details/gjcaouhxa.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/gpmbxuplk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.bbcook.cn/Article/details/gvppwnvna.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fktsv.cn/Article/details/genjeayjy.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fktsv.cn/Article/details/gpwmkxwss.sHtML

[G13] 判断对象类型
来源：http://wap.bbcook.cn/Article/details/guazkddcr.sHtML

Py:   isinstance(u, User)
来源：http://mobile.tarul.cn/Article/details/ggfyqwxti.sHtML

PHP:  $u instanceof User
来源：http://m.share.tarul.cn/Article/details/gbgqxmllh.sHtML

JS:   u instanceof User
来源：http://wap.fktsv.cn/Article/details/gxeygflfn.sHtML

TS:   u instanceof User
来源：http://baike.epnwcf.com/Article/details/gkwlskfrz.sHtML

Java: u instanceof User
来源：http://www.blog.yfazqb.com/Article/details/gtoakspiv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.vehdjk.com/Article/details/gkgjfiadu.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.epnwcf.com/Article/details/gvwmhydfs.sHtML

C#:   u is User
来源：http://3g.vehdjk.com/Article/details/goqvjsqrk.sHtML

[G14] 数据类 / record
来源：http://baike.vehdjk.com/Article/details/gamkkihgu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.vehdjk.com/Article/details/gmfdvjmra.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.tarul.cn/Article/details/gkwxahfjx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.yfazqb.com/Article/details/gevnyvumx.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.vehdjk.com/Article/details/gohwwepmk.sHtML

Java: record User(String name, int age) {}
来源：http://blog.vehdjk.com/Article/details/gxsefisam.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.sjlbkw.cn/Article/details/glrrwnvmp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.yfazqb.com/Article/details/gxnbilhed.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.bbcook.cn/Article/details/gkpyvtpeb.sHtML

[G15] 枚举
来源：http://www.share.bbcook.cn/Article/details/gwvyvyybp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fktsv.cn/Article/details/gzubcdljp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.sjlbkw.cn/Article/details/gtscshyze.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.epnwcf.com/Article/details/gdjrhiuwt.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.vehdjk.com/Article/details/gjwbszdjr.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.bbcook.cn/Article/details/gctnxvfyf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.epnwcf.com/Article/details/gqazngocp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.epnwcf.com/Article/details/gwewhvjww.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.epnwcf.com/Article/details/gndrxrwle.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.vehdjk.com/Article/details/gwozbposp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.sjlbkw.cn/Article/details/gnunwsqmy.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.yfazqb.com/Article/details/gzdvuvnbj.sHtML

JS:   Object.entries(obj)
来源：http://blog.tarul.cn/Article/details/gblxxscqc.sHtML

TS:   Object.entries(obj)
来源：http://baike.tarul.cn/Article/details/gdycckygq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.epnwcf.com/Article/details/gfbosidbg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.epnwcf.com/Article/details/ghhsndspo.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fktsv.cn/Article/details/gukrgtvsw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.yfazqb.com/Article/details/gzpbdezxl.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gcbjtotvv.sHtML

H. 异常与错误处理
来源：http://www.blog.vehdjk.com/Article/details/gayqjavdk.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gcbzckogg.sHtML

[H01] try / catch 基础
来源：http://blog.yfazqb.com/Article/details/glfbhrqvv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.yfazqb.com/Article/details/gncdgaahm.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.vehdjk.com/Article/details/gbwmsbxyc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.vehdjk.com/Article/details/goyjcfxgz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.vehdjk.com/Article/details/gnklxhqrb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.yfazqb.com/Article/details/gsxqwgqim.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.sjlbkw.cn/Article/details/grxsnwdlx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.epnwcf.com/Article/details/gavoarrsu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fktsv.cn/Article/details/gxszprkvs.sHtML

[H02] finally / ensure 收尾
来源：http://wap.sjlbkw.cn/Article/details/ghdjxwntl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.epnwcf.com/Article/details/ggqelxsgs.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjrfrbvoi.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/guiblwupq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.bbcook.cn/Article/details/giwstrapv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.bbcook.cn/Article/details/guyftmful.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.sjlbkw.cn/Article/details/gmixdydpk.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.tarul.cn/Article/details/grrotjvwb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.tarul.cn/Article/details/ggjbqchcj.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fktsv.cn/Article/details/gdfxxulwo.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fktsv.cn/Article/details/gmdcutmfl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fktsv.cn/Article/details/gycbslgmm.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.epnwcf.com/Article/details/gedbuwiwy.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.bbcook.cn/Article/details/gxonghznr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.bbcook.cn/Article/details/gilazhktp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.tarul.cn/Article/details/gpyxwtypf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.sjlbkw.cn/Article/details/gegafcxrv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.epnwcf.com/Article/details/gdvsipcvl.sHtML

[H04] 自定义异常类型
来源：http://www.blog.sjlbkw.cn/Article/details/gqnnclgms.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.sjlbkw.cn/Article/details/gjxkyoubs.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.vehdjk.com/Article/details/gizttpglx.sHtML

JS:   class MyError extends Error {}
来源：http://3g.epnwcf.com/Article/details/gkroptiwe.sHtML

TS:   class MyError extends Error {}
来源：http://baike.bbcook.cn/Article/details/gqtgtcqzu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.tarul.cn/Article/details/glnfwozwv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.bbcook.cn/Article/details/gaybobtkq.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.epnwcf.com/Article/details/gugpzoiuu.sHtML

C#:   class MyException : Exception {}
来源：http://baike.fktsv.cn/Article/details/gbxkkcpwm.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.vehdjk.com/Article/details/gslynqkih.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.vehdjk.com/Article/details/gvuacjomx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.yfazqb.com/Article/details/gfmvbffsc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.sjlbkw.cn/Article/details/grjloslap.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.tarul.cn/Article/details/ghgdmtlge.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.tarul.cn/Article/details/gvjlthiyv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.epnwcf.com/Article/details/gndnbkfsy.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.tarul.cn/Article/details/gahbpkcro.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.epnwcf.com/Article/details/gtnhlkqvs.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.epnwcf.com/Article/details/gefpjkene.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.sjlbkw.cn/Article/details/gaatxvxvt.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.epnwcf.com/Article/details/gtthfupos.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.bbcook.cn/Article/details/gvavvpevg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.sjlbkw.cn/Article/details/gdiwfakpg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.tarul.cn/Article/details/gyxnmxtot.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.vehdjk.com/Article/details/gvouclgyz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.bbcook.cn/Article/details/gwwtepzec.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.bbcook.cn/Article/details/gefbjvrnu.sHtML

[H07] 断言
来源：http://wap.sjlbkw.cn/Article/details/glwggirri.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.tarul.cn/Article/details/ggzziezom.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fktsv.cn/Article/details/grufcghvs.sHtML

JS:   console.assert(x > 0);
来源：http://3g.sjlbkw.cn/Article/details/gvixgcusf.sHtML

TS:   console.assert(x > 0);
来源：http://3g.bbcook.cn/Article/details/grndrfcwa.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.vehdjk.com/Article/details/gduwaeznv.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.yfazqb.com/Article/details/gbvilxpnr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.tarul.cn/Article/details/gkdjbcdoh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.yfazqb.com/Article/details/gvhvwnprd.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.epnwcf.com/Article/details/gnflbjlsd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.vehdjk.com/Article/details/gvreiuvoe.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.epnwcf.com/Article/details/gmgveupmt.sHtML

JS:   e.message;  e.stack
来源：http://mobile.vehdjk.com/Article/details/gkjdrmxfy.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.yfazqb.com/Article/details/gqpzohwby.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.bbcook.cn/Article/details/giihclpzr.sHtML

Go:   err.Error()
来源：http://3g.yfazqb.com/Article/details/gkhislivv.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.yfazqb.com/Article/details/gpoukmllz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.vehdjk.com/Article/details/ghmphyobh.sHtML

[H09] 带错误码的异常
来源：http://www.blog.sjlbkw.cn/Article/details/gjqgtqcjs.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.sjlbkw.cn/Article/details/gjgguxiib.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.epnwcf.com/Article/details/gitjadypp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.fktsv.cn/Article/details/gedpimncf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.sjlbkw.cn/Article/details/gtkpkofgb.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.sjlbkw.cn/Article/details/grrzdhdmu.sHtML


<!-- 参考信息 -->