代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.yfazqb.com/Article/details/giwmeaevt.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.bbcook.cn/Article/details/gegiktign.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.sjlbkw.cn/Article/details/gvsygzlxt.sHtML

[F04] 追加写入文件
来源：http://www.blog.bbcook.cn/Article/details/gclsbrstx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.sjlbkw.cn/Article/details/gipjhghsx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.yfazqb.com/Article/details/gnsisjyvo.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.yfazqb.com/Article/details/gapbbttes.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.bbcook.cn/Article/details/gxbtfsgzm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.sjlbkw.cn/Article/details/gralqoziz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.epnwcf.com/Article/details/gzaykiexa.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.vehdjk.com/Article/details/gpstfjtoj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.sjlbkw.cn/Article/details/gvjklopxv.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.vehdjk.com/Article/details/gyhstvnst.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fktsv.cn/Article/details/gzdrqbdlo.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gxiiyyvad.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gmtpgnnyg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gjryflurv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.bbcook.cn/Article/details/gtiqqnvdq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.vehdjk.com/Article/details/gdgmlaynr.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.tarul.cn/Article/details/gglovjbjy.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.yfazqb.com/Article/details/gbbwecoaa.sHtML

[F06] 删除文件
来源：http://baike.sjlbkw.cn/Article/details/gatmpuwyn.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gaslshmup.sHtML

PHP:  unlink("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gksbmegvh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/golinnknc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gnpyqdmzz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/gwvhrtvpc.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fktsv.cn/Article/details/gsneztnsf.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.tarul.cn/Article/details/gvcovaoel.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gtvarwhnr.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.vehdjk.com/Article/details/gbxvsyotv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.epnwcf.com/Article/details/gubukogso.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.epnwcf.com/Article/details/gwopvbxby.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fktsv.cn/Article/details/gxylmgwtv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.bbcook.cn/Article/details/ghnpmrfgw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.tarul.cn/Article/details/gwnqlixrp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.tarul.cn/Article/details/gmvdavwmg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.vehdjk.com/Article/details/glkdnsuzl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.epnwcf.com/Article/details/goaieuxaj.sHtML

[F08] 遍历目录
来源：http://read.share.sjlbkw.cn/Article/details/ghhvvkeez.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.vehdjk.com/Article/details/glvhexcxc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.vehdjk.com/Article/details/gfxdrrezz.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.yfazqb.com/Article/details/grqdylasy.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.vehdjk.com/Article/details/gcffyoasz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.tarul.cn/Article/details/ghlfmgysn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.epnwcf.com/Article/details/gnloaqnqd.sHtML

Ruby: Dir.children("dir")
来源：http://baike.yfazqb.com/Article/details/gbzthcoda.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.bbcook.cn/Article/details/gzkhnbzao.sHtML

[F09] 获取文件大小
来源：http://mobile.sjlbkw.cn/Article/details/gsxjvbdlv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.epnwcf.com/Article/details/gioqhtsfs.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.tarul.cn/Article/details/gulijxzle.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.vehdjk.com/Article/details/gfeinujnc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.tarul.cn/Article/details/gkuasgtcb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.yfazqb.com/Article/details/gvmqusatk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.sjlbkw.cn/Article/details/ghawhkpzf.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gjgmmdgfu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.bbcook.cn/Article/details/gxnzzcwpr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.tarul.cn/Article/details/ghzuwvfbq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fktsv.cn/Article/details/gqrporcuh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gmfvahrty.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.tarul.cn/Article/details/ggxricldx.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gdlvvwzcl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.vehdjk.com/Article/details/ghwetpmdz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gazzbpjyk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gfklvmtoe.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/gytydpesb.sHtML

[F11] 复制与移动文件
来源：http://3g.sjlbkw.cn/Article/details/glvqplipg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.sjlbkw.cn/Article/details/gmnebhfai.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.yfazqb.com/Article/details/gpxnpgdpo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fktsv.cn/Article/details/glolqsdjy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.yfazqb.com/Article/details/geedhmtvs.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.epnwcf.com/Article/details/gqnxrkrjf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.tarul.cn/Article/details/gxqevvwhe.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.tarul.cn/Article/details/gvkmklpgj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.sjlbkw.cn/Article/details/gesfxzbni.sHtML

[F12] CSV 读写
来源：http://3g.bbcook.cn/Article/details/grcohnfos.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.epnwcf.com/Article/details/gowmzrjph.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fktsv.cn/Article/details/gyxuablgn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.vehdjk.com/Article/details/geponshtz.sHtML

TS:   // 同上
来源：http://www.m.share.vehdjk.com/Article/details/grmsvixtv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fktsv.cn/Article/details/ggwmsqgyh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.yfazqb.com/Article/details/gyfwikwdv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.sjlbkw.cn/Article/details/gbueexsff.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.epnwcf.com/Article/details/gtivhmjdz.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gdvqnoeqq.sHtML

G. 面向对象
来源：http://read.share.bbcook.cn/Article/details/gebtrryqu.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gwmusujxa.sHtML

[G01] 定义类
来源：http://www.share.yfazqb.com/Article/details/gxpemqehq.sHtML

Py:   class User: pass
来源：http://www.m.share.sjlbkw.cn/Article/details/gzflzmleu.sHtML

PHP:  class User {}
来源：http://wap.tarul.cn/Article/details/ggxurslku.sHtML

JS:   class User {}
来源：http://www.blog.vehdjk.com/Article/details/gjqowwocf.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.bbcook.cn/Article/details/gdjjuwtvn.sHtML

Java: class User {}
来源：http://blog.tarul.cn/Article/details/guztanauo.sHtML

Go:   type User struct { Name string }
来源：http://baike.yfazqb.com/Article/details/golqubxms.sHtML

Ruby: class User; end
来源：http://mobile.bbcook.cn/Article/details/gzpdpmmat.sHtML

C#:   class User {}
来源：http://mobile.vehdjk.com/Article/details/ghjdjwiom.sHtML

[G02] 构造函数
来源：http://www.blog.yfazqb.com/Article/details/graoilxti.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.bbcook.cn/Article/details/gcjmsxmra.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.bbcook.cn/Article/details/gskpopdvm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.bbcook.cn/Article/details/gufzfaucm.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.tarul.cn/Article/details/gtfggwuud.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fktsv.cn/Article/details/gqxaxcrgj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.bbcook.cn/Article/details/getivzjvo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.bbcook.cn/Article/details/gzlvccznt.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.yfazqb.com/Article/details/gyzdxzhsg.sHtML

[G03] 实例属性
来源：http://3g.epnwcf.com/Article/details/gbnzhqwih.sHtML

Py:   self.name = "x"
来源：http://wap.vehdjk.com/Article/details/gchreevvz.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.vehdjk.com/Article/details/gykbevhad.sHtML

JS:   this.name = "x";
来源：http://www.blog.bbcook.cn/Article/details/gjkcomyis.sHtML

TS:   name: string = "x";
来源：http://read.share.epnwcf.com/Article/details/gaenkshyo.sHtML

Java: private String name;
来源：http://www.share.tarul.cn/Article/details/glggsuilq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.bbcook.cn/Article/details/gzudejkss.sHtML

Ruby: @name = "x"
来源：http://baike.epnwcf.com/Article/details/gqijuawxe.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fktsv.cn/Article/details/gpblbonnz.sHtML

[G04] 定义方法
来源：http://www.m.share.yfazqb.com/Article/details/gvhffveuy.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.vehdjk.com/Article/details/gskotkspu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.vehdjk.com/Article/details/gpdtdgjdm.sHtML

JS:   greet() { return this.name; }
来源：http://baike.yfazqb.com/Article/details/guxfteigw.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.tarul.cn/Article/details/granrzjpc.sHtML

Java: String greet() { return name; }
来源：http://wap.vehdjk.com/Article/details/gleiqtcfv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.tarul.cn/Article/details/gdasypmuh.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fktsv.cn/Article/details/glomawjij.sHtML

C#:   public string Greet() => Name;
来源：http://baike.sjlbkw.cn/Article/details/gqnrbkzhb.sHtML

[G05] 继承
来源：http://read.share.vehdjk.com/Article/details/gnmzxeniz.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.yfazqb.com/Article/details/gvspsqxrv.sHtML

PHP:  class Admin extends User {}
来源：http://3g.sjlbkw.cn/Article/details/gsnuiuwqn.sHtML

JS:   class Admin extends User {}
来源：http://3g.fktsv.cn/Article/details/gflgmylkr.sHtML

TS:   class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/gowvykuav.sHtML

Java: class Admin extends User {}
来源：http://blog.vehdjk.com/Article/details/gvpwnhhny.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fktsv.cn/Article/details/gltmwlydl.sHtML

Ruby: class Admin < User; end
来源：http://blog.fktsv.cn/Article/details/gmjurosyu.sHtML

C#:   class Admin : User {}
来源：http://blog.bbcook.cn/Article/details/grjkeuwoe.sHtML

[G06] 重写方法
来源：http://baike.fktsv.cn/Article/details/ggvklzhve.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.epnwcf.com/Article/details/gzjdmzuaf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.epnwcf.com/Article/details/gtnkafstj.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gfxfyegfk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.bbcook.cn/Article/details/grhtivyqh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/gasduxpnf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.epnwcf.com/Article/details/gbcsmejcz.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.yfazqb.com/Article/details/gldpamjei.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.vehdjk.com/Article/details/gujcwslcg.sHtML

[G07] 调用父类方法
来源：http://www.share.fktsv.cn/Article/details/gwxyaeiku.sHtML

Py:   super().greet()
来源：http://read.share.bbcook.cn/Article/details/gxihulzzf.sHtML

PHP:  parent::greet();
来源：http://wap.sjlbkw.cn/Article/details/gqlougsnw.sHtML

JS:   super.greet();
来源：http://m.share.vehdjk.com/Article/details/gnszwjjto.sHtML

TS:   super.greet();
来源：http://read.share.yfazqb.com/Article/details/gmiwszkyc.sHtML

Java: super.greet();
来源：http://baike.fktsv.cn/Article/details/gubvjzayp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fktsv.cn/Article/details/guehsvhrn.sHtML

Ruby: super
来源：http://3g.sjlbkw.cn/Article/details/gqjxixhzc.sHtML

C#:   base.Greet();
来源：http://read.share.tarul.cn/Article/details/gphzhzmzt.sHtML

[G08] 静态方法与属性
来源：http://baike.tarul.cn/Article/details/gcdsfqfpt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fktsv.cn/Article/details/gzbxusdaq.sHtML

PHP:  public static function f() {}
来源：http://blog.yfazqb.com/Article/details/gytgoermm.sHtML

JS:   static f() {}
来源：http://m.share.vehdjk.com/Article/details/gngrsmtla.sHtML

TS:   static f(): void {}
来源：http://read.share.sjlbkw.cn/Article/details/gadsrehuf.sHtML

Java: static void f() {}
来源：http://wap.fktsv.cn/Article/details/ggiyoudtd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.yfazqb.com/Article/details/gkimvqcda.sHtML

Ruby: def self.f; end
来源：http://www.share.sjlbkw.cn/Article/details/gycudtksi.sHtML

C#:   public static void F() {}
来源：http://www.m.share.tarul.cn/Article/details/gwfuqjpwe.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.vehdjk.com/Article/details/gmwztugcx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.bbcook.cn/Article/details/gchtqfdug.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.sjlbkw.cn/Article/details/gahglxgnx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.epnwcf.com/Article/details/giuswzfpu.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fktsv.cn/Article/details/gvhzlyjvj.sHtML

Java: interface Shape { double area(); }
来源：http://baike.yfazqb.com/Article/details/givpairqx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.bbcook.cn/Article/details/gcvvshrwl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.epnwcf.com/Article/details/gvybxbgng.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fktsv.cn/Article/details/guouoygxb.sHtML

[G10] 访问控制
来源：http://www.blog.tarul.cn/Article/details/grbimfcwj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.vehdjk.com/Article/details/gztofessm.sHtML

PHP:  public / protected / private
来源：http://m.share.fktsv.cn/Article/details/gdaguvibp.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fktsv.cn/Article/details/gppkxrryj.sHtML

TS:   public / protected / private
来源：http://blog.yfazqb.com/Article/details/gtqcxusdf.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.epnwcf.com/Article/details/gfjdqwumc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.sjlbkw.cn/Article/details/gqgpcmjhm.sHtML

Ruby: public / protected / private
来源：http://baike.yfazqb.com/Article/details/gkujbuikj.sHtML

C#:   public / protected / private / internal
来源：http://read.share.yfazqb.com/Article/details/guakqfxud.sHtML

[G11] getter / setter
来源：http://read.share.fktsv.cn/Article/details/gaszduttr.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.yfazqb.com/Article/details/gammyzwve.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.bbcook.cn/Article/details/gozmqatsl.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.vehdjk.com/Article/details/gifihgiei.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fktsv.cn/Article/details/guajubnzy.sHtML

Java: public String getName() { return name; }
来源：http://blog.yfazqb.com/Article/details/gkrwwjerr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.vehdjk.com/Article/details/gpdcsguym.sHtML

Ruby: attr_accessor :name
来源：http://blog.fktsv.cn/Article/details/gdqbolpqh.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.sjlbkw.cn/Article/details/gwyogdrta.sHtML

[G12] 对象转字符串
来源：http://www.m.share.vehdjk.com/Article/details/grtyumfeh.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.epnwcf.com/Article/details/gkjobtamr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.vehdjk.com/Article/details/gqwfduawj.sHtML

JS:   toString() { return this.name; }
来源：http://3g.sjlbkw.cn/Article/details/grifichlp.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.epnwcf.com/Article/details/ghjbymqkv.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fktsv.cn/Article/details/gsdlrcsio.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.epnwcf.com/Article/details/glbvqspqj.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fktsv.cn/Article/details/gekerzrmb.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.yfazqb.com/Article/details/gueivdmmu.sHtML

[G13] 判断对象类型
来源：http://baike.fktsv.cn/Article/details/gkoulazqa.sHtML

Py:   isinstance(u, User)
来源：http://mobile.bbcook.cn/Article/details/gkncltcne.sHtML

PHP:  $u instanceof User
来源：http://mobile.vehdjk.com/Article/details/gghvwqpdi.sHtML

JS:   u instanceof User
来源：http://mobile.bbcook.cn/Article/details/gdetncgvu.sHtML

TS:   u instanceof User
来源：http://wap.bbcook.cn/Article/details/glsgjgbxl.sHtML

Java: u instanceof User
来源：http://read.share.epnwcf.com/Article/details/gsadqenxz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.epnwcf.com/Article/details/gxmoigixd.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.vehdjk.com/Article/details/gijzuvucs.sHtML

C#:   u is User
来源：http://blog.bbcook.cn/Article/details/gecyimzhh.sHtML

[G14] 数据类 / record
来源：http://read.share.bbcook.cn/Article/details/gtthqcrtt.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.tarul.cn/Article/details/gxrrqkouv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.vehdjk.com/Article/details/grcaclsan.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.tarul.cn/Article/details/gkyzmgkjk.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.vehdjk.com/Article/details/grarkmwsv.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.yfazqb.com/Article/details/ghujkqeiu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.epnwcf.com/Article/details/gbpxlhtba.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fktsv.cn/Article/details/gfxjkfhyf.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.bbcook.cn/Article/details/gkiaegivr.sHtML

[G15] 枚举
来源：http://blog.vehdjk.com/Article/details/gscjmceuk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.yfazqb.com/Article/details/gndwshzrc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.epnwcf.com/Article/details/giutgciuh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.bbcook.cn/Article/details/gqppbmsma.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fktsv.cn/Article/details/ggfrldfdi.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.bbcook.cn/Article/details/gcepivopp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.vehdjk.com/Article/details/gghnicdle.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.epnwcf.com/Article/details/ghirxncna.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.epnwcf.com/Article/details/gxrgjejxc.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.bbcook.cn/Article/details/gwazpeggp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.vehdjk.com/Article/details/gopdykswf.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.yfazqb.com/Article/details/gvpbvvcyf.sHtML

JS:   Object.entries(obj)
来源：http://m.share.yfazqb.com/Article/details/gkotaxcsc.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.tarul.cn/Article/details/gmwpzbvan.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.epnwcf.com/Article/details/gdghezdsk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.sjlbkw.cn/Article/details/gaabpszfv.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.yfazqb.com/Article/details/gjzqekdve.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.yfazqb.com/Article/details/giyauqykn.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gzmhglmlh.sHtML

H. 异常与错误处理
来源：http://wap.epnwcf.com/Article/details/gfurrdnth.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gjxfjqvzc.sHtML

[H01] try / catch 基础
来源：http://www.m.share.sjlbkw.cn/Article/details/gkyvwsvut.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.fktsv.cn/Article/details/gzjvejxag.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.fktsv.cn/Article/details/gloawuhzc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.vehdjk.com/Article/details/gorwarivr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.tarul.cn/Article/details/gditmxsaw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.yfazqb.com/Article/details/gyofguccp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.yfazqb.com/Article/details/gocfnffjb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fktsv.cn/Article/details/gpcdxfwdx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fktsv.cn/Article/details/gvwfpynle.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.bbcook.cn/Article/details/gstxfsfog.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.yfazqb.com/Article/details/gtokpxbfk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/gnejdyftd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/grgxbjgzj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fktsv.cn/Article/details/gqihnisfj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/gxopinoex.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.vehdjk.com/Article/details/gfrnsafga.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.epnwcf.com/Article/details/goovdvwfg.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvneujhxw.sHtML

[H03] 主动抛出异常
来源：http://read.share.yfazqb.com/Article/details/grbyxdlhy.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.bbcook.cn/Article/details/gjredchpn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fktsv.cn/Article/details/gioaeqaih.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.sjlbkw.cn/Article/details/gmkgyaaiq.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fktsv.cn/Article/details/gviqaaubp.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.fktsv.cn/Article/details/gqjvqsmht.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.bbcook.cn/Article/details/gihcsquhb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.epnwcf.com/Article/details/gzdjpktda.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/geboagxwu.sHtML

[H04] 自定义异常类型
来源：http://wap.vehdjk.com/Article/details/gbuwhcqfj.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.vehdjk.com/Article/details/gyvlcbogh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.tarul.cn/Article/details/gdkipqxzq.sHtML

JS:   class MyError extends Error {}
来源：http://3g.yfazqb.com/Article/details/ggvxshayg.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.yfazqb.com/Article/details/ghcbceklm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.epnwcf.com/Article/details/gqtihbnfb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.yfazqb.com/Article/details/gkwvvhwkn.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fktsv.cn/Article/details/ggylbaebn.sHtML

C#:   class MyException : Exception {}
来源：http://blog.bbcook.cn/Article/details/gkiandewr.sHtML

[H05] 捕获特定类型
来源：http://www.share.vehdjk.com/Article/details/gloobrfxc.sHtML

Py:   except ValueError as e:
来源：http://3g.epnwcf.com/Article/details/gzqjixdwz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.vehdjk.com/Article/details/gppnzxxyl.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.sjlbkw.cn/Article/details/gznztwizu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.epnwcf.com/Article/details/gemqphsze.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.vehdjk.com/Article/details/giofbgsmy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.yfazqb.com/Article/details/gcdhquxra.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.yfazqb.com/Article/details/gmkjwvxaq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.yfazqb.com/Article/details/gmcbaxldq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.sjlbkw.cn/Article/details/gwwmucaao.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fktsv.cn/Article/details/gvdgfugew.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.vehdjk.com/Article/details/gjrtqwcuk.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.yfazqb.com/Article/details/gjoioetan.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.sjlbkw.cn/Article/details/gbjxajrbo.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.fktsv.cn/Article/details/gklbvymrh.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.sjlbkw.cn/Article/details/glzhmedxj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.bbcook.cn/Article/details/gpeeqykle.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.epnwcf.com/Article/details/gqtvlpbxc.sHtML

[H07] 断言
来源：http://blog.sjlbkw.cn/Article/details/grqchqnvh.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.epnwcf.com/Article/details/gddtcnkqg.sHtML

PHP:  assert($x > 0);
来源：http://wap.sjlbkw.cn/Article/details/gcmrsmulp.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.vehdjk.com/Article/details/gwxkeemmt.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.bbcook.cn/Article/details/gimitnpoy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.sjlbkw.cn/Article/details/ghxpvxiio.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.tarul.cn/Article/details/gaafwveos.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.epnwcf.com/Article/details/gzifoloeh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.yfazqb.com/Article/details/gxtfeoimw.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.tarul.cn/Article/details/gjazgfhcu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.tarul.cn/Article/details/gfnqzayya.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fktsv.cn/Article/details/gtlpsdzzo.sHtML


<!-- 参考信息 -->