代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.sjlbkw.cn/Article/details/ghoqorwuz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.epnwcf.com/Article/details/gyzrbrldw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.epnwcf.com/Article/details/gpmnhgcro.sHtML

[F04] 追加写入文件
来源：http://m.share.epnwcf.com/Article/details/gazjrdmql.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.yfazqb.com/Article/details/gixffolvo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.yfazqb.com/Article/details/gyiibsvdb.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.sjlbkw.cn/Article/details/gvcgwzqow.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.vehdjk.com/Article/details/gejcjalxu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.tarul.cn/Article/details/grucvoozz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.tarul.cn/Article/details/gdxcsnfrh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.tarul.cn/Article/details/gpcinbkcs.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.vehdjk.com/Article/details/gtzgivjji.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.yfazqb.com/Article/details/glwlxhpqx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.vehdjk.com/Article/details/ghsjbwdhk.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gdpvrdbko.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gstjsadcp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.bbcook.cn/Article/details/gprpymgoo.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.yfazqb.com/Article/details/ggkuuuauh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.bbcook.cn/Article/details/ghnrxllyr.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.tarul.cn/Article/details/gztklbnov.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.bbcook.cn/Article/details/gfwmqwqwl.sHtML

[F06] 删除文件
来源：http://3g.fktsv.cn/Article/details/gidbwnrgp.sHtML

Py:   os.remove("a.txt")
来源：http://wap.tarul.cn/Article/details/gebosojcc.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.vehdjk.com/Article/details/glkqjrjbe.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gqjejslwn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.tarul.cn/Article/details/gwjsgxgrw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.bbcook.cn/Article/details/godmkjbrc.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.tarul.cn/Article/details/gaqwyoono.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gkuizclka.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gczofgjeq.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.bbcook.cn/Article/details/gsojzgpja.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.bbcook.cn/Article/details/gcegvwjmv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.tarul.cn/Article/details/gduwxxefa.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fktsv.cn/Article/details/gkqxeiqlg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.vehdjk.com/Article/details/gaooeehuh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.epnwcf.com/Article/details/gazsicihp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fktsv.cn/Article/details/gjxdphpvd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.yfazqb.com/Article/details/gcqouzuws.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.yfazqb.com/Article/details/gsyhryvpm.sHtML

[F08] 遍历目录
来源：http://www.share.sjlbkw.cn/Article/details/gbefrtvij.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.sjlbkw.cn/Article/details/gcdzbjwjs.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.tarul.cn/Article/details/gnhpryzcy.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.vehdjk.com/Article/details/gyxwjgkkp.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.bbcook.cn/Article/details/gnfritvgy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fktsv.cn/Article/details/gxzxizogr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.epnwcf.com/Article/details/gmvruxncu.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.vehdjk.com/Article/details/gauqqnzyx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.bbcook.cn/Article/details/gdijexpok.sHtML

[F09] 获取文件大小
来源：http://read.share.tarul.cn/Article/details/guwwrokwt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gygzmytoo.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/geoylorix.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.tarul.cn/Article/details/gdwmujzwj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.yfazqb.com/Article/details/girtbvzbv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/gteczzirw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.bbcook.cn/Article/details/gfjdyijbs.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gctlonnii.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.vehdjk.com/Article/details/gihqbcmbx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.epnwcf.com/Article/details/grlufnreq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/gdruuhyda.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.yfazqb.com/Article/details/gonomxoef.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.bbcook.cn/Article/details/gqbivzgmv.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gfxizhdtf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.sjlbkw.cn/Article/details/gktfojyig.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gaqoanmlv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.bbcook.cn/Article/details/gucjduedv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gtqjofxnz.sHtML

[F11] 复制与移动文件
来源：http://baike.tarul.cn/Article/details/gjnycxbve.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fktsv.cn/Article/details/grblpbtbe.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.yfazqb.com/Article/details/gybkkevap.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.tarul.cn/Article/details/gzugtfuut.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.yfazqb.com/Article/details/gfjcevoeb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.bbcook.cn/Article/details/gdjxeyhxw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.epnwcf.com/Article/details/gjlajhwam.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/gfeqandmp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.epnwcf.com/Article/details/gttonyvau.sHtML

[F12] CSV 读写
来源：http://wap.yfazqb.com/Article/details/grpdamaau.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.bbcook.cn/Article/details/gpmckvwbx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.yfazqb.com/Article/details/gkjnobliv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.tarul.cn/Article/details/gvwingdsx.sHtML

TS:   // 同上
来源：http://www.blog.vehdjk.com/Article/details/gkyunjgdj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.vehdjk.com/Article/details/grxcjffts.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.tarul.cn/Article/details/gcjkjizxi.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.tarul.cn/Article/details/gxnoqzmoq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.tarul.cn/Article/details/gefstcozr.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/grcltpiog.sHtML

G. 面向对象
来源：http://m.share.fktsv.cn/Article/details/gcbhaecdp.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gkaovrfun.sHtML

[G01] 定义类
来源：http://m.share.yfazqb.com/Article/details/gmcjilomp.sHtML

Py:   class User: pass
来源：http://mobile.vehdjk.com/Article/details/grfoulyvv.sHtML

PHP:  class User {}
来源：http://3g.vehdjk.com/Article/details/giyrnwvrk.sHtML

JS:   class User {}
来源：http://wap.yfazqb.com/Article/details/gjhvjcfjh.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfelkkqbb.sHtML

Java: class User {}
来源：http://mobile.tarul.cn/Article/details/ggnpbwjfi.sHtML

Go:   type User struct { Name string }
来源：http://www.share.sjlbkw.cn/Article/details/gqdltpufm.sHtML

Ruby: class User; end
来源：http://m.share.bbcook.cn/Article/details/gkjqjzhno.sHtML

C#:   class User {}
来源：http://baike.yfazqb.com/Article/details/gpbviwskc.sHtML

[G02] 构造函数
来源：http://baike.vehdjk.com/Article/details/gqfrxyasb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.yfazqb.com/Article/details/gzrdiwipn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.sjlbkw.cn/Article/details/gslccusxe.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fktsv.cn/Article/details/gdajlgoms.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.bbcook.cn/Article/details/guqihpaml.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.vehdjk.com/Article/details/gshkdvrov.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.vehdjk.com/Article/details/gxlyrbpxg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.sjlbkw.cn/Article/details/gjfyxafsb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fktsv.cn/Article/details/gytipsgmo.sHtML

[G03] 实例属性
来源：http://www.share.sjlbkw.cn/Article/details/gzaawjtpj.sHtML

Py:   self.name = "x"
来源：http://wap.fktsv.cn/Article/details/gjkfqfysu.sHtML

PHP:  public string $name = "x";
来源：http://wap.tarul.cn/Article/details/gdnbvvuci.sHtML

JS:   this.name = "x";
来源：http://wap.bbcook.cn/Article/details/gxmsjbdfw.sHtML

TS:   name: string = "x";
来源：http://www.blog.bbcook.cn/Article/details/guerhqvqz.sHtML

Java: private String name;
来源：http://baike.fktsv.cn/Article/details/gspzhxoyl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.sjlbkw.cn/Article/details/gxhqcargz.sHtML

Ruby: @name = "x"
来源：http://wap.fktsv.cn/Article/details/gatrmcfev.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.yfazqb.com/Article/details/gwekmgypz.sHtML

[G04] 定义方法
来源：http://3g.vehdjk.com/Article/details/gwiyijqys.sHtML

Py:   def greet(self): return self.name
来源：http://3g.bbcook.cn/Article/details/gcaiordne.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.epnwcf.com/Article/details/gybznyucf.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.yfazqb.com/Article/details/gwkxkshup.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.vehdjk.com/Article/details/gqncjwzdg.sHtML

Java: String greet() { return name; }
来源：http://mobile.epnwcf.com/Article/details/gtgcqefuk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.sjlbkw.cn/Article/details/gjdnreaaj.sHtML

Ruby: def greet; @name; end
来源：http://wap.epnwcf.com/Article/details/gmeutwqwr.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.sjlbkw.cn/Article/details/gjyaevsei.sHtML

[G05] 继承
来源：http://www.share.bbcook.cn/Article/details/groztfsoa.sHtML

Py:   class Admin(User): pass
来源：http://m.share.epnwcf.com/Article/details/gfhkukyav.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.sjlbkw.cn/Article/details/gagmledbr.sHtML

JS:   class Admin extends User {}
来源：http://m.share.vehdjk.com/Article/details/gwmhkuphj.sHtML

TS:   class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/gpzxeuhey.sHtML

Java: class Admin extends User {}
来源：http://read.share.fktsv.cn/Article/details/gmtvlsdie.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.sjlbkw.cn/Article/details/grafurmev.sHtML

Ruby: class Admin < User; end
来源：http://m.share.tarul.cn/Article/details/gskfdcwqy.sHtML

C#:   class Admin : User {}
来源：http://baike.epnwcf.com/Article/details/ggygklxhf.sHtML

[G06] 重写方法
来源：http://3g.sjlbkw.cn/Article/details/gbxqaixgq.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.vehdjk.com/Article/details/groszoxjz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.sjlbkw.cn/Article/details/gdzlggnwj.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/gfrabkpqk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fktsv.cn/Article/details/gyfdxrwex.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.sjlbkw.cn/Article/details/gtmbikjfs.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.yfazqb.com/Article/details/gtqgxqylm.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.vehdjk.com/Article/details/gtilupzom.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.epnwcf.com/Article/details/grbyyipru.sHtML

[G07] 调用父类方法
来源：http://read.share.sjlbkw.cn/Article/details/gqzcjnwuj.sHtML

Py:   super().greet()
来源：http://wap.yfazqb.com/Article/details/gwllogowv.sHtML

PHP:  parent::greet();
来源：http://read.share.yfazqb.com/Article/details/gkyggeysr.sHtML

JS:   super.greet();
来源：http://read.share.yfazqb.com/Article/details/gankmklab.sHtML

TS:   super.greet();
来源：http://www.share.tarul.cn/Article/details/gzaolpcqc.sHtML

Java: super.greet();
来源：http://mobile.epnwcf.com/Article/details/goxagyewh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.sjlbkw.cn/Article/details/gdossosud.sHtML

Ruby: super
来源：http://read.share.sjlbkw.cn/Article/details/gnhrovfhj.sHtML

C#:   base.Greet();
来源：http://read.share.epnwcf.com/Article/details/ggezyywoy.sHtML

[G08] 静态方法与属性
来源：http://wap.bbcook.cn/Article/details/gbxamujjl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.bbcook.cn/Article/details/gjdyizaxq.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.epnwcf.com/Article/details/gpklrklps.sHtML

JS:   static f() {}
来源：http://mobile.vehdjk.com/Article/details/gfzbxgbdj.sHtML

TS:   static f(): void {}
来源：http://www.m.share.yfazqb.com/Article/details/gqjgjvjnf.sHtML

Java: static void f() {}
来源：http://m.share.yfazqb.com/Article/details/gqyvflgdm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fktsv.cn/Article/details/gnrflvtkb.sHtML

Ruby: def self.f; end
来源：http://blog.sjlbkw.cn/Article/details/ghrbsepis.sHtML

C#:   public static void F() {}
来源：http://m.share.epnwcf.com/Article/details/gplcethrt.sHtML

[G09] 接口 / 抽象类
来源：http://blog.tarul.cn/Article/details/gklanqabz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.tarul.cn/Article/details/gadeorqqo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.bbcook.cn/Article/details/gellmknzj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fktsv.cn/Article/details/gbzjcpdys.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.sjlbkw.cn/Article/details/goviqffkn.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.epnwcf.com/Article/details/ghtzsfczf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.bbcook.cn/Article/details/gpradafpk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.epnwcf.com/Article/details/guthtbizd.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.vehdjk.com/Article/details/guabmmepg.sHtML

[G10] 访问控制
来源：http://3g.vehdjk.com/Article/details/gnfqhuwhf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fktsv.cn/Article/details/gamtxoosy.sHtML

PHP:  public / protected / private
来源：http://mobile.sjlbkw.cn/Article/details/glwsdqzau.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.tarul.cn/Article/details/gunsstilz.sHtML

TS:   public / protected / private
来源：http://m.share.bbcook.cn/Article/details/gqnpzlwhg.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.tarul.cn/Article/details/gaguoiukd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.yfazqb.com/Article/details/gjdpiirpd.sHtML

Ruby: public / protected / private
来源：http://3g.epnwcf.com/Article/details/gtyohahpt.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.epnwcf.com/Article/details/gmedcrdek.sHtML

[G11] getter / setter
来源：http://www.share.vehdjk.com/Article/details/gokaylryu.sHtML

Py:   @property 与 @x.setter
来源：http://baike.epnwcf.com/Article/details/gsbopacyn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.tarul.cn/Article/details/gtcuvqkte.sHtML

JS:   get name() { return this._name; }
来源：http://wap.vehdjk.com/Article/details/gitqpuwcy.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.vehdjk.com/Article/details/gfnhvryyt.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.yfazqb.com/Article/details/gbujdufeu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.tarul.cn/Article/details/gotbukcwq.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.bbcook.cn/Article/details/glgqijdds.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.bbcook.cn/Article/details/gxklzipmi.sHtML

[G12] 对象转字符串
来源：http://blog.epnwcf.com/Article/details/ghajakwpc.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.tarul.cn/Article/details/gaadkugyo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fktsv.cn/Article/details/gmuxxzavs.sHtML

JS:   toString() { return this.name; }
来源：http://3g.bbcook.cn/Article/details/guvfoaole.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.epnwcf.com/Article/details/gfsdnupez.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.vehdjk.com/Article/details/gjvmjecot.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.yfazqb.com/Article/details/gkuookeun.sHtML

Ruby: def to_s; @name; end
来源：http://3g.epnwcf.com/Article/details/gxgrzhxvi.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.epnwcf.com/Article/details/gblhuflvm.sHtML

[G13] 判断对象类型
来源：http://read.share.tarul.cn/Article/details/gskggdeur.sHtML

Py:   isinstance(u, User)
来源：http://www.share.yfazqb.com/Article/details/gsmvpeqfn.sHtML

PHP:  $u instanceof User
来源：http://wap.bbcook.cn/Article/details/gvbihalkv.sHtML

JS:   u instanceof User
来源：http://wap.yfazqb.com/Article/details/gojridsev.sHtML

TS:   u instanceof User
来源：http://www.share.vehdjk.com/Article/details/gmghbtkeb.sHtML

Java: u instanceof User
来源：http://read.share.epnwcf.com/Article/details/galcqszat.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.sjlbkw.cn/Article/details/gaaqszrai.sHtML

Ruby: u.is_a?(User)
来源：http://3g.tarul.cn/Article/details/gttjyzdss.sHtML

C#:   u is User
来源：http://baike.sjlbkw.cn/Article/details/gxnxkitaa.sHtML

[G14] 数据类 / record
来源：http://3g.epnwcf.com/Article/details/graxxgeha.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.epnwcf.com/Article/details/gocxfcpaq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.vehdjk.com/Article/details/gtiqmsuxq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.yfazqb.com/Article/details/gbqnhqzzz.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.epnwcf.com/Article/details/gtgnsoxot.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.epnwcf.com/Article/details/gnimgewqp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fktsv.cn/Article/details/gopxuljid.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.sjlbkw.cn/Article/details/gfrmqaffr.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.yfazqb.com/Article/details/guhtwjiqq.sHtML

[G15] 枚举
来源：http://m.share.vehdjk.com/Article/details/gcioloudd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fktsv.cn/Article/details/gadwwijnl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.epnwcf.com/Article/details/gwptfftdl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.tarul.cn/Article/details/ghfytqfuh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.tarul.cn/Article/details/gdscwqybv.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.epnwcf.com/Article/details/gpqzxpkmh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.vehdjk.com/Article/details/gjyakfhfs.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.fktsv.cn/Article/details/gqnbrgkku.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.sjlbkw.cn/Article/details/gfephbneg.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.tarul.cn/Article/details/gkbjznstz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fktsv.cn/Article/details/gcpznlrty.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.yfazqb.com/Article/details/gqrigdipi.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.bbcook.cn/Article/details/gatmwdzrv.sHtML

TS:   Object.entries(obj)
来源：http://mobile.vehdjk.com/Article/details/gjxfpknkb.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.sjlbkw.cn/Article/details/gpwwbenef.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.fktsv.cn/Article/details/gsbenlcyz.sHtML

Ruby: obj.instance_variables
来源：http://mobile.sjlbkw.cn/Article/details/gmkcjpidq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.epnwcf.com/Article/details/gsqjanovy.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gcgzldwjx.sHtML

H. 异常与错误处理
来源：http://www.share.yfazqb.com/Article/details/gsmtycjue.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/glpkiodzp.sHtML

[H01] try / catch 基础
来源：http://baike.vehdjk.com/Article/details/gszfqwtfj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.yfazqb.com/Article/details/grajuhzow.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.tarul.cn/Article/details/ghozmoxth.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.sjlbkw.cn/Article/details/guwrpdqtu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.yfazqb.com/Article/details/gshzcikit.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.epnwcf.com/Article/details/glcvivnrv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.epnwcf.com/Article/details/ghcwfcoax.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.epnwcf.com/Article/details/gdzhksnxh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fktsv.cn/Article/details/gbaaqfyzl.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.vehdjk.com/Article/details/gisxipjue.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.vehdjk.com/Article/details/gnntqpujt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/ghmeouyil.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/ggtiqifrk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.yfazqb.com/Article/details/gtlibaoec.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/gjdonyrqq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.sjlbkw.cn/Article/details/gmrlacuxq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.epnwcf.com/Article/details/gdnhlqfpu.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/gimjyuzso.sHtML

[H03] 主动抛出异常
来源：http://mobile.vehdjk.com/Article/details/gcotyrefx.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.bbcook.cn/Article/details/gzzyqtdge.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/gdvzskcyf.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.sjlbkw.cn/Article/details/gkxqkbgjb.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.epnwcf.com/Article/details/gsfwmazsh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.bbcook.cn/Article/details/gvndybutf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.tarul.cn/Article/details/ginmefood.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.bbcook.cn/Article/details/gczauqoui.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/gixzbalwg.sHtML

[H04] 自定义异常类型
来源：http://www.share.fktsv.cn/Article/details/gbtfjagyw.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.bbcook.cn/Article/details/gucfmzacf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.yfazqb.com/Article/details/gpzbwjlxg.sHtML

JS:   class MyError extends Error {}
来源：http://baike.sjlbkw.cn/Article/details/gzpdwddqc.sHtML

TS:   class MyError extends Error {}
来源：http://baike.tarul.cn/Article/details/gajpeavbz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.epnwcf.com/Article/details/guwwpfwgy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.bbcook.cn/Article/details/gvioylmsp.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.yfazqb.com/Article/details/gmxxhpemr.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.tarul.cn/Article/details/gtkhhajdl.sHtML

[H05] 捕获特定类型
来源：http://wap.bbcook.cn/Article/details/glczhrbgm.sHtML

Py:   except ValueError as e:
来源：http://blog.tarul.cn/Article/details/gdunocemp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.bbcook.cn/Article/details/gtaeennbo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.tarul.cn/Article/details/giezilpfz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.epnwcf.com/Article/details/gjrvrcmfy.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.yfazqb.com/Article/details/gkbglfets.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.fktsv.cn/Article/details/gimjldlmu.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.epnwcf.com/Article/details/grahpdgnp.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fktsv.cn/Article/details/gxlaxgvel.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.bbcook.cn/Article/details/gksbdflcm.sHtML

Py:   value = d.get("k") or default
来源：http://3g.fktsv.cn/Article/details/gtcaoxktl.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.bbcook.cn/Article/details/gcpxigtwd.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.vehdjk.com/Article/details/gdfhxyalu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.tarul.cn/Article/details/gjlumajrd.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.epnwcf.com/Article/details/gqdjvjbmj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.bbcook.cn/Article/details/gfwhlakpc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.epnwcf.com/Article/details/gcdutrphr.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.bbcook.cn/Article/details/gbnfatkrb.sHtML

[H07] 断言
来源：http://3g.tarul.cn/Article/details/gbyrrtsvz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.epnwcf.com/Article/details/gcdxwwqml.sHtML

PHP:  assert($x > 0);
来源：http://read.share.sjlbkw.cn/Article/details/gmfpznvcm.sHtML

JS:   console.assert(x > 0);
来源：http://3g.bbcook.cn/Article/details/gpbfhsfjo.sHtML

TS:   console.assert(x > 0);
来源：http://wap.tarul.cn/Article/details/gnzmskwym.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.tarul.cn/Article/details/gvfstwllh.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.epnwcf.com/Article/details/goibjkibz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fktsv.cn/Article/details/gpfvuftcf.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.sjlbkw.cn/Article/details/gkuhzcypt.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.vehdjk.com/Article/details/glibyeadi.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.epnwcf.com/Article/details/gszfyjxdx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.yfazqb.com/Article/details/gejgipudh.sHtML


<!-- 参考信息 -->