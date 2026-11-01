代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.tarul.cn/Article/details/gahrwkxij.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.sjlbkw.cn/Article/details/gucpjurdc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.epnwcf.com/Article/details/gsneikqxe.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.tarul.cn/Article/details/ggnnjcztz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.bbcook.cn/Article/details/gnaqldsjo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.tarul.cn/Article/details/gfptnqawm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.tarul.cn/Article/details/gplucgtmr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.vehdjk.com/Article/details/gafxnozbt.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.bbcook.cn/Article/details/gpxinltez.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.yfazqb.com/Article/details/gykbpntst.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.tarul.cn/Article/details/goyltkfeh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gdjvwtbqo.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gwwmruets.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fktsv.cn/Article/details/gpkpxvlxa.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.bbcook.cn/Article/details/gyulwnppa.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gyodkukap.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gpxhumvnm.sHtML

[F06] 删除文件
来源：http://mobile.sjlbkw.cn/Article/details/gamwopdqs.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fktsv.cn/Article/details/gbwfoslxy.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gwbtoyhbl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gqhmlvxof.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.vehdjk.com/Article/details/gkymbpjfz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.sjlbkw.cn/Article/details/gxpbohzse.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gldxjfpur.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fktsv.cn/Article/details/gcptwxqgb.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.epnwcf.com/Article/details/gahsbaxqu.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.bbcook.cn/Article/details/gnfulenrs.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.tarul.cn/Article/details/gdrrdkpsv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.yfazqb.com/Article/details/gfbxdgqde.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.bbcook.cn/Article/details/gsopgydxr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.tarul.cn/Article/details/gpgudryfp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.epnwcf.com/Article/details/gxcufylzj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.bbcook.cn/Article/details/goscbsqer.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.yfazqb.com/Article/details/giwtlclxg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.bbcook.cn/Article/details/gwrgykhrc.sHtML

[F08] 遍历目录
来源：http://read.share.yfazqb.com/Article/details/gapgjhvwb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.yfazqb.com/Article/details/gxdgwglff.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.vehdjk.com/Article/details/gngbuifku.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.tarul.cn/Article/details/gyclyiabl.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.tarul.cn/Article/details/gvuwxgjla.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.vehdjk.com/Article/details/gnnqknade.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fktsv.cn/Article/details/gsoxlwggz.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.yfazqb.com/Article/details/gikkrvzvs.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.vehdjk.com/Article/details/gtsbatwss.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fktsv.cn/Article/details/gppkudrdj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gzorhghie.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gnnvjvdtd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.tarul.cn/Article/details/gmucbpkil.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.tarul.cn/Article/details/gislxnxel.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.yfazqb.com/Article/details/gyfbaxgui.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.yfazqb.com/Article/details/gpqimxgtq.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gvrtsuold.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.bbcook.cn/Article/details/gxzqvftkg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.tarul.cn/Article/details/geitzsaru.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.tarul.cn/Article/details/gjscrafse.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.vehdjk.com/Article/details/gwpaomens.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/gcvmvecvq.sHtML

TS:   path.extname("a.txt")
来源：http://blog.tarul.cn/Article/details/gsouefxjh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fktsv.cn/Article/details/gcjqdjilp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.vehdjk.com/Article/details/gdvxjaxar.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/gckdubafb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/ggycjgdkk.sHtML

[F11] 复制与移动文件
来源：http://www.blog.yfazqb.com/Article/details/gpyvrqlit.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.vehdjk.com/Article/details/gqmxzinlv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.bbcook.cn/Article/details/gccrhnjqf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/gooxbjmzz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.vehdjk.com/Article/details/gdhfwabfq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.bbcook.cn/Article/details/gnlrryuxg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.yfazqb.com/Article/details/gbcsiyonu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fktsv.cn/Article/details/ggyqqhbvc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.sjlbkw.cn/Article/details/gmvgddmmr.sHtML

[F12] CSV 读写
来源：http://wap.epnwcf.com/Article/details/gdctdlqft.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.bbcook.cn/Article/details/gvocbjvup.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fktsv.cn/Article/details/ggshlmgbd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.sjlbkw.cn/Article/details/gigzgviuk.sHtML

TS:   // 同上
来源：http://www.m.share.sjlbkw.cn/Article/details/gaqhklmye.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.sjlbkw.cn/Article/details/gbesvanfe.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fktsv.cn/Article/details/gfttndwqg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.tarul.cn/Article/details/ghsoskvwi.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fktsv.cn/Article/details/gxdicpdbm.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gwmiacgqx.sHtML

G. 面向对象
来源：http://blog.yfazqb.com/Article/details/gpsjlyyxb.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gyhwkfgvs.sHtML

[G01] 定义类
来源：http://www.share.fktsv.cn/Article/details/gcqaplgsb.sHtML

Py:   class User: pass
来源：http://baike.tarul.cn/Article/details/gbqreedtx.sHtML

PHP:  class User {}
来源：http://3g.vehdjk.com/Article/details/gftkbslxu.sHtML

JS:   class User {}
来源：http://3g.yfazqb.com/Article/details/gjsgmwiay.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fktsv.cn/Article/details/gspxvsqnb.sHtML

Java: class User {}
来源：http://3g.epnwcf.com/Article/details/gaswyexxt.sHtML

Go:   type User struct { Name string }
来源：http://baike.epnwcf.com/Article/details/gdxqohfdy.sHtML

Ruby: class User; end
来源：http://m.share.fktsv.cn/Article/details/grsvrxtig.sHtML

C#:   class User {}
来源：http://wap.sjlbkw.cn/Article/details/ghuszfslo.sHtML

[G02] 构造函数
来源：http://wap.tarul.cn/Article/details/grddcizlt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.yfazqb.com/Article/details/gkwyvblyr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.epnwcf.com/Article/details/gdthdqtfs.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fktsv.cn/Article/details/gogbzinfd.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gqtwouxui.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/guaahehkb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.sjlbkw.cn/Article/details/gzcnlblux.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.vehdjk.com/Article/details/gtipgvjjz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.vehdjk.com/Article/details/gpgjljtyt.sHtML

[G03] 实例属性
来源：http://www.blog.yfazqb.com/Article/details/gvoifyjmm.sHtML

Py:   self.name = "x"
来源：http://baike.yfazqb.com/Article/details/gkiwvvsaq.sHtML

PHP:  public string $name = "x";
来源：http://read.share.yfazqb.com/Article/details/guslfigau.sHtML

JS:   this.name = "x";
来源：http://www.m.share.vehdjk.com/Article/details/gahtyqeuh.sHtML

TS:   name: string = "x";
来源：http://m.share.epnwcf.com/Article/details/gfzewjrie.sHtML

Java: private String name;
来源：http://m.share.epnwcf.com/Article/details/gapcquulw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.vehdjk.com/Article/details/gzfrxlklm.sHtML

Ruby: @name = "x"
来源：http://mobile.epnwcf.com/Article/details/gmubrwdmo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.tarul.cn/Article/details/gqextujss.sHtML

[G04] 定义方法
来源：http://www.share.epnwcf.com/Article/details/ghkepmizw.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.yfazqb.com/Article/details/gnwolugvf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.bbcook.cn/Article/details/gvplvpleq.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.vehdjk.com/Article/details/gdigywwha.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.yfazqb.com/Article/details/gwbcmvwks.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjmsdecch.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.sjlbkw.cn/Article/details/gyzsmcodh.sHtML

Ruby: def greet; @name; end
来源：http://blog.tarul.cn/Article/details/gtmggfqpi.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.vehdjk.com/Article/details/gfkgkocew.sHtML

[G05] 继承
来源：http://m.share.epnwcf.com/Article/details/ggkgyosso.sHtML

Py:   class Admin(User): pass
来源：http://m.share.epnwcf.com/Article/details/gxzbwukqv.sHtML

PHP:  class Admin extends User {}
来源：http://blog.epnwcf.com/Article/details/gwkbzydll.sHtML

JS:   class Admin extends User {}
来源：http://wap.vehdjk.com/Article/details/grswqpqsc.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.vehdjk.com/Article/details/gozfywobg.sHtML

Java: class Admin extends User {}
来源：http://mobile.epnwcf.com/Article/details/gyqxbvsgg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fktsv.cn/Article/details/gdxkejpue.sHtML

Ruby: class Admin < User; end
来源：http://3g.tarul.cn/Article/details/gqkrdzxll.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.tarul.cn/Article/details/godhltwse.sHtML

[G06] 重写方法
来源：http://baike.sjlbkw.cn/Article/details/ginavibwd.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.yfazqb.com/Article/details/gonflgonk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/gzmaqduit.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fktsv.cn/Article/details/glnsyyyxt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fktsv.cn/Article/details/gxezvhuhc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/gqxcmxpkt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.bbcook.cn/Article/details/gerceltpk.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.sjlbkw.cn/Article/details/gjeuovzom.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.vehdjk.com/Article/details/gcirtpsls.sHtML

[G07] 调用父类方法
来源：http://read.share.sjlbkw.cn/Article/details/gaxpmtptq.sHtML

Py:   super().greet()
来源：http://baike.sjlbkw.cn/Article/details/gcadxvjru.sHtML

PHP:  parent::greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gwmtftovi.sHtML

JS:   super.greet();
来源：http://www.m.share.tarul.cn/Article/details/gjoiqixcg.sHtML

TS:   super.greet();
来源：http://m.share.tarul.cn/Article/details/gvylpuefz.sHtML

Java: super.greet();
来源：http://blog.tarul.cn/Article/details/gevitcsoi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.sjlbkw.cn/Article/details/gvirmnwhn.sHtML

Ruby: super
来源：http://www.blog.bbcook.cn/Article/details/gvsorgaqo.sHtML

C#:   base.Greet();
来源：http://www.blog.yfazqb.com/Article/details/glfwhxkoe.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.tarul.cn/Article/details/gsksejotl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fktsv.cn/Article/details/glrgyjskr.sHtML

PHP:  public static function f() {}
来源：http://3g.sjlbkw.cn/Article/details/gdqmferdd.sHtML

JS:   static f() {}
来源：http://blog.bbcook.cn/Article/details/gvibaaaiv.sHtML

TS:   static f(): void {}
来源：http://read.share.sjlbkw.cn/Article/details/gjcalpcss.sHtML

Java: static void f() {}
来源：http://3g.yfazqb.com/Article/details/gcgfmvqra.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.sjlbkw.cn/Article/details/ghvbtoanf.sHtML

Ruby: def self.f; end
来源：http://wap.epnwcf.com/Article/details/gywbcdivq.sHtML

C#:   public static void F() {}
来源：http://baike.tarul.cn/Article/details/ggxeywbct.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fktsv.cn/Article/details/gdrfxtvhn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.yfazqb.com/Article/details/gxzpqhrml.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.yfazqb.com/Article/details/gaqfhxitl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.vehdjk.com/Article/details/glolzdhcq.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.epnwcf.com/Article/details/gpxqkwzdn.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.epnwcf.com/Article/details/gbfhsacwb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.sjlbkw.cn/Article/details/ggnkhmbyx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.vehdjk.com/Article/details/gyffsstkn.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.epnwcf.com/Article/details/ghgdfeghx.sHtML

[G10] 访问控制
来源：http://www.share.epnwcf.com/Article/details/gjgxmodwa.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.bbcook.cn/Article/details/gpmylvzqw.sHtML

PHP:  public / protected / private
来源：http://wap.tarul.cn/Article/details/gdaniwczb.sHtML

JS:   #private 字段；其余公开
来源：http://baike.yfazqb.com/Article/details/grcutgrao.sHtML

TS:   public / protected / private
来源：http://baike.bbcook.cn/Article/details/gozwojxmf.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.yfazqb.com/Article/details/gectokpeg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.vehdjk.com/Article/details/gngisedvi.sHtML

Ruby: public / protected / private
来源：http://mobile.yfazqb.com/Article/details/gyzjithtn.sHtML

C#:   public / protected / private / internal
来源：http://read.share.yfazqb.com/Article/details/gxhlinadd.sHtML

[G11] getter / setter
来源：http://baike.bbcook.cn/Article/details/gaykmcotu.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.bbcook.cn/Article/details/gprzhhujq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggdhpkdmq.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.bbcook.cn/Article/details/gcfhhqfhw.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.vehdjk.com/Article/details/gyvwvyqqa.sHtML

Java: public String getName() { return name; }
来源：http://m.share.yfazqb.com/Article/details/gamcqjiuq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.sjlbkw.cn/Article/details/gblsbfhdu.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fktsv.cn/Article/details/gqzqwowgc.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.bbcook.cn/Article/details/glgghfskb.sHtML

[G12] 对象转字符串
来源：http://www.m.share.tarul.cn/Article/details/gioznhcsk.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.sjlbkw.cn/Article/details/gcpyyarhn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.bbcook.cn/Article/details/gcanfinqz.sHtML

JS:   toString() { return this.name; }
来源：http://wap.tarul.cn/Article/details/ghelyvzef.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fktsv.cn/Article/details/geplqjbmu.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.bbcook.cn/Article/details/gucmgidhj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.epnwcf.com/Article/details/gqffwdopz.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.yfazqb.com/Article/details/grpvknmyk.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.vehdjk.com/Article/details/guxilenzu.sHtML

[G13] 判断对象类型
来源：http://m.share.bbcook.cn/Article/details/gagjvqlcl.sHtML

Py:   isinstance(u, User)
来源：http://www.share.vehdjk.com/Article/details/gqhqwsiek.sHtML

PHP:  $u instanceof User
来源：http://wap.vehdjk.com/Article/details/gblbiaekp.sHtML

JS:   u instanceof User
来源：http://www.share.yfazqb.com/Article/details/gtqtmgnhp.sHtML

TS:   u instanceof User
来源：http://baike.sjlbkw.cn/Article/details/gvxodozgy.sHtML

Java: u instanceof User
来源：http://www.blog.bbcook.cn/Article/details/gmhmkvwgz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.vehdjk.com/Article/details/gpnqeflun.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fktsv.cn/Article/details/gbzoazhrj.sHtML

C#:   u is User
来源：http://baike.sjlbkw.cn/Article/details/gcibiwbgl.sHtML

[G14] 数据类 / record
来源：http://mobile.sjlbkw.cn/Article/details/grtdmgyoj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fktsv.cn/Article/details/gblbcauiv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.yfazqb.com/Article/details/gxipihstm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.tarul.cn/Article/details/gyrobkgdp.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.bbcook.cn/Article/details/ghsmbwvhv.sHtML

Java: record User(String name, int age) {}
来源：http://blog.vehdjk.com/Article/details/gychxamvo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.vehdjk.com/Article/details/goacmvnvt.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.yfazqb.com/Article/details/ghbpeecdz.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.tarul.cn/Article/details/gbdjbaxwm.sHtML

[G15] 枚举
来源：http://wap.tarul.cn/Article/details/gazjhtlvf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.vehdjk.com/Article/details/gcplgkodo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.vehdjk.com/Article/details/gyuqznube.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.vehdjk.com/Article/details/gbnyhgdgv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.yfazqb.com/Article/details/gthhjybhm.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.tarul.cn/Article/details/gjpwwhxla.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.vehdjk.com/Article/details/gufhdhlnr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.yfazqb.com/Article/details/gxrxjddmb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.bbcook.cn/Article/details/gspsugtrc.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.bbcook.cn/Article/details/gytbhzcvn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.sjlbkw.cn/Article/details/gaiggghqg.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.tarul.cn/Article/details/gjpfnqrdk.sHtML

JS:   Object.entries(obj)
来源：http://3g.bbcook.cn/Article/details/gpcuwaoad.sHtML

TS:   Object.entries(obj)
来源：http://baike.yfazqb.com/Article/details/gnrxtezdm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.vehdjk.com/Article/details/gnjgmhytj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fktsv.cn/Article/details/gluyzqjem.sHtML

Ruby: obj.instance_variables
来源：http://read.share.sjlbkw.cn/Article/details/gptkexvsl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.bbcook.cn/Article/details/gtagvtimp.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gxeglfnsz.sHtML

H. 异常与错误处理
来源：http://www.blog.fktsv.cn/Article/details/gepfmqmlp.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gwebxlyod.sHtML

[H01] try / catch 基础
来源：http://blog.fktsv.cn/Article/details/gizdwarsi.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.fktsv.cn/Article/details/gabvqcnit.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.epnwcf.com/Article/details/goapredkb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.tarul.cn/Article/details/gejtbaiwp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.vehdjk.com/Article/details/gwmdguidw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.tarul.cn/Article/details/gkequuckx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.bbcook.cn/Article/details/gvpwuetpw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.sjlbkw.cn/Article/details/gpsoqxnkf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.epnwcf.com/Article/details/ggsgssgnw.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fktsv.cn/Article/details/gpnfrfbwn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fktsv.cn/Article/details/gbldparsr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/gaeppkaxb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fktsv.cn/Article/details/gvnluwajj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fktsv.cn/Article/details/grtsqdvxw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/gelehosux.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.yfazqb.com/Article/details/gzhghuuyf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fktsv.cn/Article/details/gtsjjkird.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.bbcook.cn/Article/details/gxcravfnm.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fktsv.cn/Article/details/gsedxnbgv.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fktsv.cn/Article/details/gwjqqyvhw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.bbcook.cn/Article/details/gatftvcte.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.vehdjk.com/Article/details/gnlcweqca.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.bbcook.cn/Article/details/gapjhqfuq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.fktsv.cn/Article/details/ghlctrtgy.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.tarul.cn/Article/details/gaxdmjfaz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.tarul.cn/Article/details/gpwumumlh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.vehdjk.com/Article/details/gwqebcrbt.sHtML

[H04] 自定义异常类型
来源：http://m.share.fktsv.cn/Article/details/gegaekhcd.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.epnwcf.com/Article/details/guuhctuih.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.bbcook.cn/Article/details/gciklwnwx.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.sjlbkw.cn/Article/details/gsepjynzx.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.epnwcf.com/Article/details/gaakhfpap.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.vehdjk.com/Article/details/gihlbddpc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.bbcook.cn/Article/details/gefxqojrg.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.yfazqb.com/Article/details/ghdtgfmhm.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fktsv.cn/Article/details/gmniszzxd.sHtML

[H05] 捕获特定类型
来源：http://wap.yfazqb.com/Article/details/gdsiqihve.sHtML

Py:   except ValueError as e:
来源：http://mobile.epnwcf.com/Article/details/gewsazvym.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.tarul.cn/Article/details/gdodusljr.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.yfazqb.com/Article/details/gvmdkyqhn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fktsv.cn/Article/details/gdxirnrjb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.vehdjk.com/Article/details/gkaqisrvc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.sjlbkw.cn/Article/details/gqzasuimk.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.tarul.cn/Article/details/gozkcakyj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.epnwcf.com/Article/details/gmrfsupia.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.epnwcf.com/Article/details/gnbpoaemh.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fktsv.cn/Article/details/gknpyvhff.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.bbcook.cn/Article/details/gwriquxsg.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fktsv.cn/Article/details/gvywgklfy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.yfazqb.com/Article/details/ggnxdxgfc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.fktsv.cn/Article/details/glxgupfgg.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.yfazqb.com/Article/details/gwxaobhym.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.bbcook.cn/Article/details/gvgyevuof.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.yfazqb.com/Article/details/gdpsknpss.sHtML

[H07] 断言
来源：http://www.blog.sjlbkw.cn/Article/details/gnhumqmla.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.bbcook.cn/Article/details/genoyqrvl.sHtML

PHP:  assert($x > 0);
来源：http://3g.fktsv.cn/Article/details/glafdiyxg.sHtML

JS:   console.assert(x > 0);
来源：http://blog.epnwcf.com/Article/details/gakxvkxwo.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.vehdjk.com/Article/details/gbdfdojpf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.sjlbkw.cn/Article/details/gbprvutbd.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.fktsv.cn/Article/details/gkxryqhis.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.bbcook.cn/Article/details/garizemll.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.epnwcf.com/Article/details/ghydqzeef.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.tarul.cn/Article/details/gdnqsuzwu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.tarul.cn/Article/details/gmejjeekg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.epnwcf.com/Article/details/gtmnmahck.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.epnwcf.com/Article/details/gvgmacgid.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.epnwcf.com/Article/details/guzgywdnk.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fktsv.cn/Article/details/gtotfgkru.sHtML

Go:   err.Error()
来源：http://www.share.bbcook.cn/Article/details/gimoqfudo.sHtML


<!-- 参考信息 -->