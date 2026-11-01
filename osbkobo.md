代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.tarul.cn/Article/details/gumqpmwbe.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.vehdjk.com/Article/details/gsrrjgqyb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.tarul.cn/Article/details/gcsgohicl.sHtML

[F04] 追加写入文件
来源：http://m.share.epnwcf.com/Article/details/gweovkzoq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.vehdjk.com/Article/details/ggoamqbuv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.epnwcf.com/Article/details/gpzhybvds.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.epnwcf.com/Article/details/gdaazbehg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fktsv.cn/Article/details/gbvkxztoy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.vehdjk.com/Article/details/gmbvgegkw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.bbcook.cn/Article/details/ghzwanahq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fktsv.cn/Article/details/glgyuurxo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fktsv.cn/Article/details/gxenyrezh.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.bbcook.cn/Article/details/gmtqwwagt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.epnwcf.com/Article/details/gyyyjvqcu.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gqnmhlefd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gphirapcy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.epnwcf.com/Article/details/gjhozqxxl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.tarul.cn/Article/details/guuffiods.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.bbcook.cn/Article/details/gtyzsmtat.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.vehdjk.com/Article/details/gwzjabuok.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.yfazqb.com/Article/details/gswzqihox.sHtML

[F06] 删除文件
来源：http://m.share.yfazqb.com/Article/details/gohgljtsw.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fktsv.cn/Article/details/gluilmlcs.sHtML

PHP:  unlink("a.txt");
来源：http://baike.bbcook.cn/Article/details/gawmiunkx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.epnwcf.com/Article/details/glorzetri.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.vehdjk.com/Article/details/gkabbeqab.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fktsv.cn/Article/details/gwizwvwtc.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.tarul.cn/Article/details/gujinekfh.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqkunjqmt.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gjwndogmd.sHtML

[F07] 创建目录（含多级）
来源：http://wap.epnwcf.com/Article/details/gyuqsrgxg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.tarul.cn/Article/details/gpmeqkriq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.vehdjk.com/Article/details/gycwkhcsk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.sjlbkw.cn/Article/details/gebeflqhq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.yfazqb.com/Article/details/gsdfcplef.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gknfqmmed.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.sjlbkw.cn/Article/details/geksevbey.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.vehdjk.com/Article/details/gwgbrmxjp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.sjlbkw.cn/Article/details/gpzuwswgd.sHtML

[F08] 遍历目录
来源：http://baike.vehdjk.com/Article/details/gtqsudtpf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fktsv.cn/Article/details/gssqirnuv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fktsv.cn/Article/details/gxwnbzuht.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.vehdjk.com/Article/details/gyxrygmdl.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.sjlbkw.cn/Article/details/gwmhrrqdz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.epnwcf.com/Article/details/gcrzrmvyo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.yfazqb.com/Article/details/gilyyfybk.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.tarul.cn/Article/details/gsxzwlqas.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/gcpgvocyk.sHtML

[F09] 获取文件大小
来源：http://www.blog.vehdjk.com/Article/details/ggyzyfmnf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwciwezpe.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gdscybqif.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fktsv.cn/Article/details/glsrjyjjg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fktsv.cn/Article/details/gjfprzgcd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/gpwtndcdm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.tarul.cn/Article/details/gukeayoty.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fktsv.cn/Article/details/gvlhkolkz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.yfazqb.com/Article/details/gtiiwqygh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fktsv.cn/Article/details/gfnyvyajo.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fktsv.cn/Article/details/gcyfiopbu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gmiufnbgq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/gvufeekdx.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.tarul.cn/Article/details/gjooidrll.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.bbcook.cn/Article/details/gjjeeiemz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.vehdjk.com/Article/details/gsayrzyha.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/giwquuhtu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gnppagyhh.sHtML

[F11] 复制与移动文件
来源：http://read.share.epnwcf.com/Article/details/gjwwftaip.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.vehdjk.com/Article/details/gfangelyo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.epnwcf.com/Article/details/gcyldlrtu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.yfazqb.com/Article/details/gddziaqux.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fktsv.cn/Article/details/ggkeeugcw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.bbcook.cn/Article/details/gnpwkseny.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.yfazqb.com/Article/details/gqwzwmulw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/gllwcpmjr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fktsv.cn/Article/details/ggyghjnpz.sHtML

[F12] CSV 读写
来源：http://3g.vehdjk.com/Article/details/gvqvyzdfw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.bbcook.cn/Article/details/goiwniceo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.bbcook.cn/Article/details/gxrdnuqmh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fktsv.cn/Article/details/gztoblndc.sHtML

TS:   // 同上
来源：http://blog.bbcook.cn/Article/details/gkncwrhxg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.yfazqb.com/Article/details/gauyggujg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.bbcook.cn/Article/details/glqbtvxan.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fktsv.cn/Article/details/gbreigdsp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fktsv.cn/Article/details/gdxtdqwpf.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gzkbitqwd.sHtML

G. 面向对象
来源：http://www.blog.tarul.cn/Article/details/glonelxcd.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gayjozpzn.sHtML

[G01] 定义类
来源：http://www.share.bbcook.cn/Article/details/gldszijar.sHtML

Py:   class User: pass
来源：http://www.m.share.vehdjk.com/Article/details/gmpfkrwix.sHtML

PHP:  class User {}
来源：http://m.share.epnwcf.com/Article/details/gnpodbwys.sHtML

JS:   class User {}
来源：http://mobile.epnwcf.com/Article/details/grlhhejem.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fktsv.cn/Article/details/gtfspeflh.sHtML

Java: class User {}
来源：http://www.share.epnwcf.com/Article/details/gthffjuhj.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.epnwcf.com/Article/details/gawexjnqa.sHtML

Ruby: class User; end
来源：http://blog.sjlbkw.cn/Article/details/gozfflpmf.sHtML

C#:   class User {}
来源：http://blog.tarul.cn/Article/details/gxtjnranp.sHtML

[G02] 构造函数
来源：http://www.share.sjlbkw.cn/Article/details/gomdsvpqv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.sjlbkw.cn/Article/details/gkcsifvme.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fktsv.cn/Article/details/gbaxwiisu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.sjlbkw.cn/Article/details/gxssfcjhg.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.vehdjk.com/Article/details/gcdwdngui.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.sjlbkw.cn/Article/details/gzqqbhxjq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.bbcook.cn/Article/details/gewlhoahx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.bbcook.cn/Article/details/gxwxzsqru.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.bbcook.cn/Article/details/glxcfffnz.sHtML

[G03] 实例属性
来源：http://wap.sjlbkw.cn/Article/details/gusmvymzl.sHtML

Py:   self.name = "x"
来源：http://m.share.fktsv.cn/Article/details/gdfbdblsq.sHtML

PHP:  public string $name = "x";
来源：http://baike.sjlbkw.cn/Article/details/gxpgzdpwd.sHtML

JS:   this.name = "x";
来源：http://m.share.sjlbkw.cn/Article/details/gxrbjrhto.sHtML

TS:   name: string = "x";
来源：http://baike.fktsv.cn/Article/details/gszqtvvbe.sHtML

Java: private String name;
来源：http://wap.fktsv.cn/Article/details/grjdziifm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fktsv.cn/Article/details/gsfnsfgmb.sHtML

Ruby: @name = "x"
来源：http://read.share.yfazqb.com/Article/details/gbkcndvau.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.sjlbkw.cn/Article/details/gleaplpjw.sHtML

[G04] 定义方法
来源：http://wap.yfazqb.com/Article/details/gtpuazzvh.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fktsv.cn/Article/details/gchclecsb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.sjlbkw.cn/Article/details/guuxnlqyo.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/gtlcemcpd.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.bbcook.cn/Article/details/ghfcltngw.sHtML

Java: String greet() { return name; }
来源：http://baike.bbcook.cn/Article/details/gpwhuyonh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.tarul.cn/Article/details/gkatjrglm.sHtML

Ruby: def greet; @name; end
来源：http://3g.bbcook.cn/Article/details/gyvclspvl.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.tarul.cn/Article/details/gbfzfkptg.sHtML

[G05] 继承
来源：http://www.m.share.bbcook.cn/Article/details/gskbwpihj.sHtML

Py:   class Admin(User): pass
来源：http://3g.yfazqb.com/Article/details/gsrhixexf.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.bbcook.cn/Article/details/gziyvgphp.sHtML

JS:   class Admin extends User {}
来源：http://blog.fktsv.cn/Article/details/gnaoycwkd.sHtML

TS:   class Admin extends User {}
来源：http://wap.sjlbkw.cn/Article/details/gadgeirxn.sHtML

Java: class Admin extends User {}
来源：http://read.share.epnwcf.com/Article/details/ghcwqupxm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.yfazqb.com/Article/details/gxhfffkvg.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fktsv.cn/Article/details/gegbgahob.sHtML

C#:   class Admin : User {}
来源：http://3g.fktsv.cn/Article/details/gbwetapsa.sHtML

[G06] 重写方法
来源：http://blog.bbcook.cn/Article/details/gattpppfm.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.sjlbkw.cn/Article/details/gnriuklmy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.sjlbkw.cn/Article/details/gcvgjdxdp.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.epnwcf.com/Article/details/gxguqgwkr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.tarul.cn/Article/details/gnvsidnez.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.tarul.cn/Article/details/gpsowzrhm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.tarul.cn/Article/details/gagjxlhoq.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fktsv.cn/Article/details/gsgihxxzs.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.vehdjk.com/Article/details/gtsbevpxd.sHtML

[G07] 调用父类方法
来源：http://www.m.share.tarul.cn/Article/details/gmgtictcm.sHtML

Py:   super().greet()
来源：http://www.share.fktsv.cn/Article/details/girfoqxsh.sHtML

PHP:  parent::greet();
来源：http://www.share.tarul.cn/Article/details/golhwyzef.sHtML

JS:   super.greet();
来源：http://baike.fktsv.cn/Article/details/giczrjstp.sHtML

TS:   super.greet();
来源：http://mobile.fktsv.cn/Article/details/gecpjeyfp.sHtML

Java: super.greet();
来源：http://www.share.vehdjk.com/Article/details/gftnzwicz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.tarul.cn/Article/details/gypeoyxra.sHtML

Ruby: super
来源：http://mobile.sjlbkw.cn/Article/details/gmkrdimxe.sHtML

C#:   base.Greet();
来源：http://baike.tarul.cn/Article/details/gvgsckzai.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.sjlbkw.cn/Article/details/gtczyddwu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.epnwcf.com/Article/details/gchhjcrvt.sHtML

PHP:  public static function f() {}
来源：http://blog.epnwcf.com/Article/details/gmpkrxtdk.sHtML

JS:   static f() {}
来源：http://www.m.share.vehdjk.com/Article/details/gfwsnqnhw.sHtML

TS:   static f(): void {}
来源：http://www.share.epnwcf.com/Article/details/gkucyelzf.sHtML

Java: static void f() {}
来源：http://www.share.bbcook.cn/Article/details/giocjuggk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.vehdjk.com/Article/details/gkpcwkpmi.sHtML

Ruby: def self.f; end
来源：http://www.blog.epnwcf.com/Article/details/gckoolcsd.sHtML

C#:   public static void F() {}
来源：http://wap.epnwcf.com/Article/details/gtxmoklnx.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.sjlbkw.cn/Article/details/grvuxfpkl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fktsv.cn/Article/details/gzvvhmopg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.tarul.cn/Article/details/gbkwqopdi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.vehdjk.com/Article/details/gdezaoxvx.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.yfazqb.com/Article/details/gauyltkyc.sHtML

Java: interface Shape { double area(); }
来源：http://baike.sjlbkw.cn/Article/details/gpkmvrhyx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.bbcook.cn/Article/details/gknntdtpy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.epnwcf.com/Article/details/gnwocywbl.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.bbcook.cn/Article/details/gdsqzfvvt.sHtML

[G10] 访问控制
来源：http://www.blog.yfazqb.com/Article/details/gpsptmwyv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.yfazqb.com/Article/details/gatvkizgl.sHtML

PHP:  public / protected / private
来源：http://3g.epnwcf.com/Article/details/gtcvmyhbk.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.epnwcf.com/Article/details/gpznrdfxr.sHtML

TS:   public / protected / private
来源：http://baike.yfazqb.com/Article/details/gfhcptfnm.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.sjlbkw.cn/Article/details/gvldyxhnv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.vehdjk.com/Article/details/geqkneors.sHtML

Ruby: public / protected / private
来源：http://www.m.share.epnwcf.com/Article/details/gcxclilad.sHtML

C#:   public / protected / private / internal
来源：http://baike.sjlbkw.cn/Article/details/gcxmurhms.sHtML

[G11] getter / setter
来源：http://read.share.sjlbkw.cn/Article/details/gzauvqfyn.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.vehdjk.com/Article/details/gvrjddtsk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.yfazqb.com/Article/details/gbgpezeap.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.tarul.cn/Article/details/gmbxugiwl.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.epnwcf.com/Article/details/gyzbgauvg.sHtML

Java: public String getName() { return name; }
来源：http://3g.yfazqb.com/Article/details/gswlyweng.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.sjlbkw.cn/Article/details/gppbqnpkc.sHtML

Ruby: attr_accessor :name
来源：http://wap.vehdjk.com/Article/details/gcuhafhgr.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.bbcook.cn/Article/details/gusnoajqd.sHtML

[G12] 对象转字符串
来源：http://www.m.share.tarul.cn/Article/details/gfsmlhawb.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.sjlbkw.cn/Article/details/gdnexpdlg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.bbcook.cn/Article/details/gtiybakqc.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/gksepxlfa.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.tarul.cn/Article/details/glctlumxb.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.sjlbkw.cn/Article/details/gcvgwnzlp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.tarul.cn/Article/details/gxbpgydcq.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.tarul.cn/Article/details/ghdjpdbtk.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.yfazqb.com/Article/details/gdducszco.sHtML

[G13] 判断对象类型
来源：http://wap.vehdjk.com/Article/details/gmfvbhpyq.sHtML

Py:   isinstance(u, User)
来源：http://blog.yfazqb.com/Article/details/gcuahauxk.sHtML

PHP:  $u instanceof User
来源：http://blog.vehdjk.com/Article/details/guzdtslba.sHtML

JS:   u instanceof User
来源：http://m.share.tarul.cn/Article/details/gcskeonkf.sHtML

TS:   u instanceof User
来源：http://www.m.share.fktsv.cn/Article/details/gyxdtmcvs.sHtML

Java: u instanceof User
来源：http://read.share.tarul.cn/Article/details/gllfbkcie.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fktsv.cn/Article/details/gfqhnzcrh.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.yfazqb.com/Article/details/gukivbppf.sHtML

C#:   u is User
来源：http://www.m.share.fktsv.cn/Article/details/ggkfcrzyk.sHtML

[G14] 数据类 / record
来源：http://www.m.share.tarul.cn/Article/details/glapazpbr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.sjlbkw.cn/Article/details/gjnraxfjw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.tarul.cn/Article/details/gxostjgoi.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.epnwcf.com/Article/details/gycdmbpsw.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fktsv.cn/Article/details/gmbnmnmtz.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.tarul.cn/Article/details/gmqdyogao.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.tarul.cn/Article/details/goctnxfli.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.tarul.cn/Article/details/grvzkptzd.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.bbcook.cn/Article/details/gzniznuhh.sHtML

[G15] 枚举
来源：http://read.share.yfazqb.com/Article/details/gjngweytx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.epnwcf.com/Article/details/ghesrisei.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.epnwcf.com/Article/details/gruclhiwm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.yfazqb.com/Article/details/glwcaacjm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fktsv.cn/Article/details/gmwqyqrpm.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.tarul.cn/Article/details/gpxhpaflg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.epnwcf.com/Article/details/gnkuflicq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.sjlbkw.cn/Article/details/gujpupblz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fktsv.cn/Article/details/gjmnisxys.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.yfazqb.com/Article/details/gyuxaoxte.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.vehdjk.com/Article/details/gyhirjgzr.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.fktsv.cn/Article/details/gmfkihfvh.sHtML

JS:   Object.entries(obj)
来源：http://wap.vehdjk.com/Article/details/gxnwbcjmu.sHtML

TS:   Object.entries(obj)
来源：http://read.share.epnwcf.com/Article/details/gedlmlzes.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.epnwcf.com/Article/details/glehiptqv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.epnwcf.com/Article/details/gdwepziuo.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fktsv.cn/Article/details/gnvqarcrb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.bbcook.cn/Article/details/glnwcydwd.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/glvljclzy.sHtML

H. 异常与错误处理
来源：http://read.share.epnwcf.com/Article/details/gnzzzalvp.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/ghikdydil.sHtML

[H01] try / catch 基础
来源：http://baike.fktsv.cn/Article/details/gjwddqpuo.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.vehdjk.com/Article/details/gclnxmxhd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.tarul.cn/Article/details/gglcpmtan.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.epnwcf.com/Article/details/gbrodvghp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.bbcook.cn/Article/details/gokwcxcpd.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.epnwcf.com/Article/details/gdbpjxcrs.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.tarul.cn/Article/details/gyrwgzteb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.tarul.cn/Article/details/gagtitvvy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.epnwcf.com/Article/details/gqxtvmlag.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.vehdjk.com/Article/details/givtmtgwm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.bbcook.cn/Article/details/gwzatnlrn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.sjlbkw.cn/Article/details/gtmgciqya.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/gddumygdi.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/gnfxekzry.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.tarul.cn/Article/details/gsbciyuve.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.sjlbkw.cn/Article/details/gkolwdrmm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.vehdjk.com/Article/details/gzxvqwirm.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.tarul.cn/Article/details/glhtestmq.sHtML

[H03] 主动抛出异常
来源：http://3g.fktsv.cn/Article/details/gmcbvvudq.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.sjlbkw.cn/Article/details/gyilsiddj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.tarul.cn/Article/details/gpswlimcz.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.bbcook.cn/Article/details/ghpqbkaeb.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.epnwcf.com/Article/details/gictnunaj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.yfazqb.com/Article/details/grwlxtzkx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fktsv.cn/Article/details/gikhuihtv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.bbcook.cn/Article/details/ghcezvddm.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.vehdjk.com/Article/details/gklfgekwj.sHtML

[H04] 自定义异常类型
来源：http://m.share.fktsv.cn/Article/details/gipxooijj.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.yfazqb.com/Article/details/ggvhzamvo.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.tarul.cn/Article/details/gisqghsyh.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.vehdjk.com/Article/details/giqwcmzbg.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.vehdjk.com/Article/details/gahwnjibf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.tarul.cn/Article/details/gopwjdmub.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.bbcook.cn/Article/details/gzafuqxhq.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.yfazqb.com/Article/details/gsdzcjhha.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gcgzwjucu.sHtML

[H05] 捕获特定类型
来源：http://blog.vehdjk.com/Article/details/gmnenzsar.sHtML

Py:   except ValueError as e:
来源：http://3g.fktsv.cn/Article/details/gdqacbnhg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.bbcook.cn/Article/details/gqsmcvdsb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fktsv.cn/Article/details/gcqgijdth.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.tarul.cn/Article/details/gmzujifpn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.vehdjk.com/Article/details/ghpdxussn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.sjlbkw.cn/Article/details/ggotrydac.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.epnwcf.com/Article/details/gsvlhedzw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.vehdjk.com/Article/details/gvslmjcnw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.epnwcf.com/Article/details/gkpavxtpt.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.sjlbkw.cn/Article/details/gophizklw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.vehdjk.com/Article/details/gxexnnhuv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.bbcook.cn/Article/details/ghommpkcs.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.vehdjk.com/Article/details/gwikamfqn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.tarul.cn/Article/details/gkqgkxeot.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.tarul.cn/Article/details/gkdvgzlxi.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fktsv.cn/Article/details/ghoggdeqv.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.yfazqb.com/Article/details/grdnwadqt.sHtML

[H07] 断言
来源：http://www.m.share.tarul.cn/Article/details/ghdzahukx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.bbcook.cn/Article/details/gmnnyeyjk.sHtML

PHP:  assert($x > 0);
来源：http://wap.epnwcf.com/Article/details/gnjzsgdqm.sHtML

JS:   console.assert(x > 0);
来源：http://3g.tarul.cn/Article/details/grnoihnzh.sHtML

TS:   console.assert(x > 0);
来源：http://blog.epnwcf.com/Article/details/gsgqvprlg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.yfazqb.com/Article/details/gwubvhjxa.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.yfazqb.com/Article/details/gscumzxov.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.bbcook.cn/Article/details/gyzqmbwmx.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.sjlbkw.cn/Article/details/gsvorxnjh.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.fktsv.cn/Article/details/gnwvkcmmv.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.vehdjk.com/Article/details/gvmqwzbuw.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.fktsv.cn/Article/details/gysypibgq.sHtML


<!-- 参考信息 -->