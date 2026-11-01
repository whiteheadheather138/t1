代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.sjlbkw.cn/Article/details/gwwuoqmoc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.epnwcf.com/Article/details/gcxtqcpih.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.sjlbkw.cn/Article/details/gmzxhhvyx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.bbcook.cn/Article/details/gjisocdfw.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.tarul.cn/Article/details/gyfdbcqgk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.vehdjk.com/Article/details/gpsszxqdw.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/ggilyqfjw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gmitqudzv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.epnwcf.com/Article/details/gihnoaanp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.yfazqb.com/Article/details/gdcsprmsa.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.tarul.cn/Article/details/gmhryywdz.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.yfazqb.com/Article/details/glfnfojux.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gdlnkmobq.sHtML

[F06] 删除文件
来源：http://baike.vehdjk.com/Article/details/gjstdjuod.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fktsv.cn/Article/details/gjxxpljuo.sHtML

PHP:  unlink("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gnijeksje.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fktsv.cn/Article/details/ggnhwywvl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gjammytaf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fktsv.cn/Article/details/gmhuiftvy.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gggomlbfx.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.tarul.cn/Article/details/gxpnjtakt.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gnnboemwa.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.sjlbkw.cn/Article/details/grtflvvym.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.yfazqb.com/Article/details/gvbcnxczu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.tarul.cn/Article/details/gamanmhqe.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fktsv.cn/Article/details/gocxrqwau.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.vehdjk.com/Article/details/gctjbgolt.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fktsv.cn/Article/details/gpinzuutj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.yfazqb.com/Article/details/gokxolsvf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.epnwcf.com/Article/details/gvdzbnakd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.tarul.cn/Article/details/gxuzufeco.sHtML

[F08] 遍历目录
来源：http://m.share.fktsv.cn/Article/details/gbkuroccj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.sjlbkw.cn/Article/details/gzomotizc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.yfazqb.com/Article/details/gyjhswmtg.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.tarul.cn/Article/details/gqfqunrsy.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.tarul.cn/Article/details/gejblerkb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.tarul.cn/Article/details/gsdvkpqri.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.bbcook.cn/Article/details/gwnrtiddj.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.tarul.cn/Article/details/gmzrzpfsu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.yfazqb.com/Article/details/gdbxjyvws.sHtML

[F09] 获取文件大小
来源：http://wap.bbcook.cn/Article/details/grquameuy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fktsv.cn/Article/details/gtxgoduhc.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gnvvycsqf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.tarul.cn/Article/details/gyqcrkvqt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.epnwcf.com/Article/details/ghabsydwb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fktsv.cn/Article/details/gucxtmmqt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.tarul.cn/Article/details/gcpcubkrb.sHtML

Ruby: File.size("a.txt")
来源：http://blog.yfazqb.com/Article/details/giutpmvqs.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.yfazqb.com/Article/details/gzttkqdcb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.epnwcf.com/Article/details/gjbbhvmjt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/gqpdgnyqu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.epnwcf.com/Article/details/gcpfmtfwb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/gmkapbalg.sHtML

TS:   path.extname("a.txt")
来源：http://wap.tarul.cn/Article/details/gzmhjnccq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.sjlbkw.cn/Article/details/gpoyovwsp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.yfazqb.com/Article/details/gmpzpafkj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/gxbasmdju.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gcltqdxgw.sHtML

[F11] 复制与移动文件
来源：http://blog.sjlbkw.cn/Article/details/groyirniy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gjcgrwtxw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.sjlbkw.cn/Article/details/gowlctyop.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fktsv.cn/Article/details/gdohjknfp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.bbcook.cn/Article/details/ggkgvjrzu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.yfazqb.com/Article/details/grlfumfvy.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.epnwcf.com/Article/details/gycxlgdrp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gceobzwtb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.vehdjk.com/Article/details/gcwqxgksm.sHtML

[F12] CSV 读写
来源：http://blog.fktsv.cn/Article/details/gdyjmetsf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.yfazqb.com/Article/details/gdmtyygyq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.bbcook.cn/Article/details/gnmfgdnzo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.epnwcf.com/Article/details/gadesdlmw.sHtML

TS:   // 同上
来源：http://wap.sjlbkw.cn/Article/details/gokotwhom.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.epnwcf.com/Article/details/gjmpieerf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.tarul.cn/Article/details/gtygpnxyt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.bbcook.cn/Article/details/gfslyjqqc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.yfazqb.com/Article/details/gpqyjskkc.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gbqaftclu.sHtML

G. 面向对象
来源：http://blog.fktsv.cn/Article/details/ghzoqmirg.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/grazeqyvb.sHtML

[G01] 定义类
来源：http://mobile.fktsv.cn/Article/details/gwggoosue.sHtML

Py:   class User: pass
来源：http://m.share.yfazqb.com/Article/details/gdaxpuovn.sHtML

PHP:  class User {}
来源：http://baike.tarul.cn/Article/details/gzzhnqhsh.sHtML

JS:   class User {}
来源：http://read.share.vehdjk.com/Article/details/grbzsfvmw.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.epnwcf.com/Article/details/grdprtzwe.sHtML

Java: class User {}
来源：http://www.blog.fktsv.cn/Article/details/gpigzdhmg.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.yfazqb.com/Article/details/gbgpbhmlm.sHtML

Ruby: class User; end
来源：http://mobile.yfazqb.com/Article/details/gnuolpfdm.sHtML

C#:   class User {}
来源：http://3g.epnwcf.com/Article/details/gsowyhsew.sHtML

[G02] 构造函数
来源：http://3g.vehdjk.com/Article/details/gcebtdtlb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.sjlbkw.cn/Article/details/ggktnjcod.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fktsv.cn/Article/details/gptizaqyu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.vehdjk.com/Article/details/gdcvcxqph.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.bbcook.cn/Article/details/gmlevkjnb.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.tarul.cn/Article/details/gwfgudeff.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.yfazqb.com/Article/details/gbyyshqzb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.yfazqb.com/Article/details/gkbppbxjp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fktsv.cn/Article/details/gmdyulbvy.sHtML

[G03] 实例属性
来源：http://www.m.share.tarul.cn/Article/details/gigbfjxma.sHtML

Py:   self.name = "x"
来源：http://blog.epnwcf.com/Article/details/gnozusqni.sHtML

PHP:  public string $name = "x";
来源：http://wap.tarul.cn/Article/details/gcupgjwpb.sHtML

JS:   this.name = "x";
来源：http://mobile.fktsv.cn/Article/details/gnugiqbpm.sHtML

TS:   name: string = "x";
来源：http://www.share.epnwcf.com/Article/details/gwrlzuznf.sHtML

Java: private String name;
来源：http://3g.sjlbkw.cn/Article/details/gnslitnwi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fktsv.cn/Article/details/gwcknvzgt.sHtML

Ruby: @name = "x"
来源：http://wap.sjlbkw.cn/Article/details/gjotxtqwd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.yfazqb.com/Article/details/gshlrxlzw.sHtML

[G04] 定义方法
来源：http://3g.epnwcf.com/Article/details/grtgxekly.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.yfazqb.com/Article/details/gkdzreulk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.sjlbkw.cn/Article/details/gsfbzatza.sHtML

JS:   greet() { return this.name; }
来源：http://3g.tarul.cn/Article/details/ghhyyyccu.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.yfazqb.com/Article/details/gthsvwqdg.sHtML

Java: String greet() { return name; }
来源：http://baike.vehdjk.com/Article/details/gwhpcbrnj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.sjlbkw.cn/Article/details/ggptouatj.sHtML

Ruby: def greet; @name; end
来源：http://baike.sjlbkw.cn/Article/details/gildppoel.sHtML

C#:   public string Greet() => Name;
来源：http://3g.epnwcf.com/Article/details/ghkjccsdi.sHtML

[G05] 继承
来源：http://www.m.share.yfazqb.com/Article/details/gvkfhreyh.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fktsv.cn/Article/details/gxwuljuzv.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.vehdjk.com/Article/details/gkclujwjk.sHtML

JS:   class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/gwpkiwifb.sHtML

TS:   class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/gxnddhcrt.sHtML

Java: class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/gcumnpcnw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.yfazqb.com/Article/details/gprexoboz.sHtML

Ruby: class Admin < User; end
来源：http://read.share.tarul.cn/Article/details/gduepbaud.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.yfazqb.com/Article/details/gpudmcjms.sHtML

[G06] 重写方法
来源：http://mobile.fktsv.cn/Article/details/gvbheudqn.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.yfazqb.com/Article/details/gckfptwax.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/grrpmdzcu.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.epnwcf.com/Article/details/gtxtfftol.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.yfazqb.com/Article/details/gnncglkrx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.vehdjk.com/Article/details/gnpcrwyhx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.epnwcf.com/Article/details/gfjtlggki.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.sjlbkw.cn/Article/details/gjdvtuxpg.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.epnwcf.com/Article/details/gekvshypd.sHtML

[G07] 调用父类方法
来源：http://read.share.tarul.cn/Article/details/gaefwvdhi.sHtML

Py:   super().greet()
来源：http://wap.bbcook.cn/Article/details/ghxclxnnk.sHtML

PHP:  parent::greet();
来源：http://www.m.share.epnwcf.com/Article/details/gsgkbgjny.sHtML

JS:   super.greet();
来源：http://mobile.bbcook.cn/Article/details/gzyiuftye.sHtML

TS:   super.greet();
来源：http://www.share.tarul.cn/Article/details/gejnypddn.sHtML

Java: super.greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gulkfjwwn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.epnwcf.com/Article/details/grkycxota.sHtML

Ruby: super
来源：http://mobile.epnwcf.com/Article/details/gtjcebmfh.sHtML

C#:   base.Greet();
来源：http://read.share.vehdjk.com/Article/details/garoveufl.sHtML

[G08] 静态方法与属性
来源：http://baike.vehdjk.com/Article/details/gutqrwcoi.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.sjlbkw.cn/Article/details/gkvsxylem.sHtML

PHP:  public static function f() {}
来源：http://wap.sjlbkw.cn/Article/details/gyjhtgdjj.sHtML

JS:   static f() {}
来源：http://www.m.share.epnwcf.com/Article/details/gqnwmjuxg.sHtML

TS:   static f(): void {}
来源：http://baike.vehdjk.com/Article/details/gfouwlyip.sHtML

Java: static void f() {}
来源：http://mobile.epnwcf.com/Article/details/gkupivbgd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.sjlbkw.cn/Article/details/geplusdcg.sHtML

Ruby: def self.f; end
来源：http://read.share.vehdjk.com/Article/details/gtdkgbxjl.sHtML

C#:   public static void F() {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gacjpcvnc.sHtML

[G09] 接口 / 抽象类
来源：http://wap.epnwcf.com/Article/details/gkoogdaig.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.sjlbkw.cn/Article/details/gnljqxngo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fktsv.cn/Article/details/giojshocs.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.bbcook.cn/Article/details/gphtixddj.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.yfazqb.com/Article/details/glfzwabwo.sHtML

Java: interface Shape { double area(); }
来源：http://baike.vehdjk.com/Article/details/gecoqjfwt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.bbcook.cn/Article/details/gccgdwioq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.epnwcf.com/Article/details/gevdsacil.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fktsv.cn/Article/details/gnfdvihhn.sHtML

[G10] 访问控制
来源：http://www.share.sjlbkw.cn/Article/details/gtfmdrjtq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.sjlbkw.cn/Article/details/gqjeidxnc.sHtML

PHP:  public / protected / private
来源：http://wap.epnwcf.com/Article/details/gndqvsurd.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.yfazqb.com/Article/details/gqdxlqndy.sHtML

TS:   public / protected / private
来源：http://m.share.tarul.cn/Article/details/grlcgrrvk.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.yfazqb.com/Article/details/gvkbrkvwy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.sjlbkw.cn/Article/details/guzmljdtd.sHtML

Ruby: public / protected / private
来源：http://mobile.fktsv.cn/Article/details/grdphgucv.sHtML

C#:   public / protected / private / internal
来源：http://mobile.yfazqb.com/Article/details/gccvdbfag.sHtML

[G11] getter / setter
来源：http://3g.epnwcf.com/Article/details/gnosrnwew.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.vehdjk.com/Article/details/gukyjpcpc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.vehdjk.com/Article/details/gkkmdpghg.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.bbcook.cn/Article/details/gyrblzbxq.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fktsv.cn/Article/details/gmbimxirc.sHtML

Java: public String getName() { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/gmcshvzuf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.vehdjk.com/Article/details/gmjjozgxx.sHtML

Ruby: attr_accessor :name
来源：http://m.share.vehdjk.com/Article/details/gnxlmksud.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.yfazqb.com/Article/details/gbrkltuio.sHtML

[G12] 对象转字符串
来源：http://wap.yfazqb.com/Article/details/gpnhvilti.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.bbcook.cn/Article/details/gwjjsrled.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fktsv.cn/Article/details/gwafgwspk.sHtML

JS:   toString() { return this.name; }
来源：http://3g.bbcook.cn/Article/details/gkqlqbvmo.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.bbcook.cn/Article/details/gnnkguhac.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.sjlbkw.cn/Article/details/grymyorjc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.yfazqb.com/Article/details/gwkpummrx.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.tarul.cn/Article/details/ggvbwshuo.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.epnwcf.com/Article/details/gsyhcbxxt.sHtML

[G13] 判断对象类型
来源：http://wap.yfazqb.com/Article/details/gmpxkrayf.sHtML

Py:   isinstance(u, User)
来源：http://baike.vehdjk.com/Article/details/gyzdyanwd.sHtML

PHP:  $u instanceof User
来源：http://3g.tarul.cn/Article/details/gxhhlwejs.sHtML

JS:   u instanceof User
来源：http://www.share.bbcook.cn/Article/details/gsdiqeixz.sHtML

TS:   u instanceof User
来源：http://blog.sjlbkw.cn/Article/details/girduvunz.sHtML

Java: u instanceof User
来源：http://3g.sjlbkw.cn/Article/details/gysstfvqd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.vehdjk.com/Article/details/gtimefkad.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fktsv.cn/Article/details/gcwlsqich.sHtML

C#:   u is User
来源：http://m.share.vehdjk.com/Article/details/grkljsmjm.sHtML

[G14] 数据类 / record
来源：http://www.blog.vehdjk.com/Article/details/gpijckrax.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.yfazqb.com/Article/details/gpreajaxa.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.bbcook.cn/Article/details/gwpmgmovy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.vehdjk.com/Article/details/gntfmwpib.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.yfazqb.com/Article/details/gwuvkdndt.sHtML

Java: record User(String name, int age) {}
来源：http://wap.vehdjk.com/Article/details/gracwoamw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.vehdjk.com/Article/details/ghetcdqoa.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fktsv.cn/Article/details/gguvlxhjy.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.tarul.cn/Article/details/gbqtzajlk.sHtML

[G15] 枚举
来源：http://3g.fktsv.cn/Article/details/gdpvhhmrc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.epnwcf.com/Article/details/gjrikeltv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.bbcook.cn/Article/details/gwzhuayxk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.sjlbkw.cn/Article/details/grerfvkeg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.tarul.cn/Article/details/gkkasgpph.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.vehdjk.com/Article/details/gwvtywddh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.sjlbkw.cn/Article/details/guicpywyt.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.vehdjk.com/Article/details/gtzrooypv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fktsv.cn/Article/details/gnrmtouue.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.tarul.cn/Article/details/gzmrrihah.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.epnwcf.com/Article/details/gexsooaec.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.yfazqb.com/Article/details/gevzadsxx.sHtML

JS:   Object.entries(obj)
来源：http://m.share.tarul.cn/Article/details/gkxqgjtgb.sHtML

TS:   Object.entries(obj)
来源：http://wap.fktsv.cn/Article/details/guorxynms.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.yfazqb.com/Article/details/gdvxsbwbx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.tarul.cn/Article/details/ggatpolub.sHtML

Ruby: obj.instance_variables
来源：http://m.share.tarul.cn/Article/details/gwouzjzaw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fktsv.cn/Article/details/glrpmeuja.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gmbtejyzr.sHtML

H. 异常与错误处理
来源：http://3g.vehdjk.com/Article/details/gpabjszsd.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/guwpxunjw.sHtML

[H01] try / catch 基础
来源：http://mobile.fktsv.cn/Article/details/gcnjdbbpo.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.bbcook.cn/Article/details/gasoohbnv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.vehdjk.com/Article/details/gahhsqtld.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fktsv.cn/Article/details/gllwxybzm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.tarul.cn/Article/details/gwmlnpmak.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.epnwcf.com/Article/details/gcuhuifxc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.vehdjk.com/Article/details/gkyvpazfd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.tarul.cn/Article/details/gilbznuvy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.tarul.cn/Article/details/ggjfgghmn.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.sjlbkw.cn/Article/details/ggcyvifvt.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.vehdjk.com/Article/details/gpcwdgrfd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fktsv.cn/Article/details/gqdmlxysj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fktsv.cn/Article/details/gbpofsxmc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.tarul.cn/Article/details/ggkndpwdz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.vehdjk.com/Article/details/gsrcdveyq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.bbcook.cn/Article/details/godmerryl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.vehdjk.com/Article/details/gmhhzmbeg.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.yfazqb.com/Article/details/gydjtmnyh.sHtML

[H03] 主动抛出异常
来源：http://m.share.fktsv.cn/Article/details/gayuwclrb.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.bbcook.cn/Article/details/gurhirfcz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.sjlbkw.cn/Article/details/gbiuktgyb.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.tarul.cn/Article/details/gidaqrnmb.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.vehdjk.com/Article/details/gaffmyoxe.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.yfazqb.com/Article/details/gumrsaina.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.epnwcf.com/Article/details/ggrqyyaqm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.bbcook.cn/Article/details/gyxjdfbkg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.bbcook.cn/Article/details/gdjschaxd.sHtML

[H04] 自定义异常类型
来源：http://blog.tarul.cn/Article/details/gtgwmnrha.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.sjlbkw.cn/Article/details/gkgjlnwdo.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fktsv.cn/Article/details/gkbwmtyec.sHtML

JS:   class MyError extends Error {}
来源：http://baike.epnwcf.com/Article/details/gxfooluoz.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.yfazqb.com/Article/details/glxugxgpx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fktsv.cn/Article/details/gweknwvdh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.yfazqb.com/Article/details/gjmwmdiuy.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.vehdjk.com/Article/details/ghadnhdbw.sHtML

C#:   class MyException : Exception {}
来源：http://baike.bbcook.cn/Article/details/goznjzota.sHtML

[H05] 捕获特定类型
来源：http://www.blog.epnwcf.com/Article/details/gqwfcaydz.sHtML

Py:   except ValueError as e:
来源：http://m.share.vehdjk.com/Article/details/gzenydhwq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.bbcook.cn/Article/details/gjjexnghv.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.yfazqb.com/Article/details/gvvyytmvx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fktsv.cn/Article/details/giulouygq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.epnwcf.com/Article/details/ghxjwyzjk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.epnwcf.com/Article/details/gkfqezjgr.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fktsv.cn/Article/details/ggwypdznn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.vehdjk.com/Article/details/grcvsszop.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.yfazqb.com/Article/details/ghgpwsvni.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.bbcook.cn/Article/details/gdvpbshza.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fktsv.cn/Article/details/gemoiqkhk.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.yfazqb.com/Article/details/gxjlcexps.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.sjlbkw.cn/Article/details/gxthpmnbb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.epnwcf.com/Article/details/gablbvfqp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.vehdjk.com/Article/details/gkshatwxp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.fktsv.cn/Article/details/gfwzozfpy.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.epnwcf.com/Article/details/gopdtyiiw.sHtML

[H07] 断言
来源：http://wap.vehdjk.com/Article/details/gkkzfsjuf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.yfazqb.com/Article/details/gbliszdid.sHtML

PHP:  assert($x > 0);
来源：http://baike.sjlbkw.cn/Article/details/gzsvzdnuq.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.vehdjk.com/Article/details/gcbmstgbt.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.tarul.cn/Article/details/gjymvzxdk.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.bbcook.cn/Article/details/gyelntmmz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.tarul.cn/Article/details/gojfyauez.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.tarul.cn/Article/details/gjlieoleu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.bbcook.cn/Article/details/gwuxivwzb.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.bbcook.cn/Article/details/gvfebfksc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.sjlbkw.cn/Article/details/gsnaqbfop.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.fktsv.cn/Article/details/gwqoqrwrb.sHtML

JS:   e.message;  e.stack
来源：http://3g.tarul.cn/Article/details/godnlhjhi.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.epnwcf.com/Article/details/ggbpjkxor.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.fktsv.cn/Article/details/gyonobdiw.sHtML

Go:   err.Error()
来源：http://m.share.bbcook.cn/Article/details/gfzvdgfgn.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.vehdjk.com/Article/details/gyoifgnfl.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.vehdjk.com/Article/details/gcdthtghh.sHtML

[H09] 带错误码的异常
来源：http://blog.yfazqb.com/Article/details/gmyeuejha.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.tarul.cn/Article/details/gynxmmlva.sHtML


<!-- 参考信息 -->