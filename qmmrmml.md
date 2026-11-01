代发 wailian999

[F01] 读取整个文件
来源：http://mobile.tarul.cn/Article/details/giqolzycb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.sjlbkw.cn/Article/details/gfauwnccr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.yfazqb.com/Article/details/gqhhngdwx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.bbcook.cn/Article/details/gczabnfys.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.epnwcf.com/Article/details/gmpcdjsgn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.tarul.cn/Article/details/gykulhuwo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.bbcook.cn/Article/details/gqovspxfl.sHtML

Ruby: File.read("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gcwovapgj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gqgdmfnkg.sHtML

[F02] 逐行读取文件
来源：http://blog.fktsv.cn/Article/details/guexumgie.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.tarul.cn/Article/details/ghqkkczby.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fktsv.cn/Article/details/guxnzgjbb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.yfazqb.com/Article/details/gmziytlzv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fktsv.cn/Article/details/gylkqvewe.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.sjlbkw.cn/Article/details/gozfbhjta.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.tarul.cn/Article/details/guhkmscbp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.epnwcf.com/Article/details/gcxwbsfyr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.vehdjk.com/Article/details/grqzigike.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.tarul.cn/Article/details/gebdfbzdb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.sjlbkw.cn/Article/details/gvsogdnjd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.bbcook.cn/Article/details/ghdpcdewi.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.tarul.cn/Article/details/gihovvypx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.bbcook.cn/Article/details/geltebuxp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.sjlbkw.cn/Article/details/govpbiufg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.sjlbkw.cn/Article/details/gztnvctfg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.bbcook.cn/Article/details/gjdjggkhf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.bbcook.cn/Article/details/gqsmulikj.sHtML

[F04] 追加写入文件
来源：http://blog.fktsv.cn/Article/details/ggyoerkyz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.tarul.cn/Article/details/gdaopipsp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.epnwcf.com/Article/details/gxrzvhgkb.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.epnwcf.com/Article/details/gdbywewbu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.bbcook.cn/Article/details/gqbkibyek.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.yfazqb.com/Article/details/gnzfgtvsf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.yfazqb.com/Article/details/gzbbpsnej.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.bbcook.cn/Article/details/gxtgwhoel.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.vehdjk.com/Article/details/gnvjmrnfs.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.bbcook.cn/Article/details/gjvulugof.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.yfazqb.com/Article/details/gsllxabkm.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gwstyoavt.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.bbcook.cn/Article/details/ggjbejnfb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gjtmcepzx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.tarul.cn/Article/details/ggizakfrv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.vehdjk.com/Article/details/gylpluivy.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.tarul.cn/Article/details/graiihvdi.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gbmbknmgt.sHtML

[F06] 删除文件
来源：http://3g.tarul.cn/Article/details/ghxyurjze.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gjulgcbzj.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gtcudauvk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gcrmxtzlu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gtawsmzue.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.vehdjk.com/Article/details/gmkhzerrp.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.vehdjk.com/Article/details/glvqssjjh.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gghupupvl.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gomgidjlz.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.vehdjk.com/Article/details/giuylinxt.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.epnwcf.com/Article/details/gtarowlhj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.yfazqb.com/Article/details/gqfrekkza.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.yfazqb.com/Article/details/ghrxynsla.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fktsv.cn/Article/details/gkwjitxyx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.yfazqb.com/Article/details/gwkjupbjr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.vehdjk.com/Article/details/gcexaynod.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.bbcook.cn/Article/details/gwwgjssbd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.yfazqb.com/Article/details/gkdfefult.sHtML

[F08] 遍历目录
来源：http://wap.sjlbkw.cn/Article/details/gzoyvpeyr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fktsv.cn/Article/details/gwknbblha.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.yfazqb.com/Article/details/gnmjkaxow.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.yfazqb.com/Article/details/gsriuurvm.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.sjlbkw.cn/Article/details/geztawkqh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.tarul.cn/Article/details/gtfbetpdl.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.yfazqb.com/Article/details/gtofyfijy.sHtML

Ruby: Dir.children("dir")
来源：http://wap.tarul.cn/Article/details/gznagqrsh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.yfazqb.com/Article/details/gjtovjgux.sHtML

[F09] 获取文件大小
来源：http://baike.epnwcf.com/Article/details/gnfnejngw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gjeawogik.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gevxogwyu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.vehdjk.com/Article/details/goggcdwut.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.vehdjk.com/Article/details/gdbzlepwu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.sjlbkw.cn/Article/details/gtkdfmbnh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.vehdjk.com/Article/details/gcnblrbrf.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fktsv.cn/Article/details/gnekyjrjk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.epnwcf.com/Article/details/gsjcnadnp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.epnwcf.com/Article/details/gawbhzljy.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gjjdnfhtw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fktsv.cn/Article/details/gvuwuzgei.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.tarul.cn/Article/details/gqjrwrmms.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gkwuneqib.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.vehdjk.com/Article/details/gecmbtrlm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gqfcpgkji.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gbmimauvt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.tarul.cn/Article/details/gsfubumhx.sHtML

[F11] 复制与移动文件
来源：http://m.share.fktsv.cn/Article/details/gaybwvduw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/gndnliuja.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.epnwcf.com/Article/details/gpixocsvk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.epnwcf.com/Article/details/gcndzyzep.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.yfazqb.com/Article/details/gxhlbzlfm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.yfazqb.com/Article/details/gcnrtmhoj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fktsv.cn/Article/details/gcalzsemo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gwetdfwdp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fktsv.cn/Article/details/gxwplitdw.sHtML

[F12] CSV 读写
来源：http://www.m.share.fktsv.cn/Article/details/gbpnpgptr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fktsv.cn/Article/details/glqniolcf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.tarul.cn/Article/details/gwgmjlpnx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.sjlbkw.cn/Article/details/gvjjvwwau.sHtML

TS:   // 同上
来源：http://www.share.fktsv.cn/Article/details/grxfucavs.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.bbcook.cn/Article/details/grsoicdfx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.vehdjk.com/Article/details/gjsuqbvxp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fktsv.cn/Article/details/gsqupcikp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.yfazqb.com/Article/details/gbhhbdhai.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gltswztvn.sHtML

G. 面向对象
来源：http://blog.vehdjk.com/Article/details/glkjwxsdg.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gjxscxwpt.sHtML

[G01] 定义类
来源：http://baike.tarul.cn/Article/details/gsruerxkl.sHtML

Py:   class User: pass
来源：http://read.share.tarul.cn/Article/details/gfcpcbwkt.sHtML

PHP:  class User {}
来源：http://m.share.fktsv.cn/Article/details/gynmxzbmz.sHtML

JS:   class User {}
来源：http://wap.fktsv.cn/Article/details/ghmpvvyqk.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnecphksa.sHtML

Java: class User {}
来源：http://mobile.yfazqb.com/Article/details/gfkrrxpei.sHtML

Go:   type User struct { Name string }
来源：http://www.share.yfazqb.com/Article/details/gyptuuprr.sHtML

Ruby: class User; end
来源：http://blog.vehdjk.com/Article/details/gtghbckhd.sHtML

C#:   class User {}
来源：http://baike.bbcook.cn/Article/details/gwqdpvlci.sHtML

[G02] 构造函数
来源：http://read.share.tarul.cn/Article/details/guldyoqgu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.epnwcf.com/Article/details/gqajkqmdd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.yfazqb.com/Article/details/gbxkngvyn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.epnwcf.com/Article/details/gdgxdoead.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.epnwcf.com/Article/details/gutbnmzfg.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.vehdjk.com/Article/details/garvklyln.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.vehdjk.com/Article/details/gkntumlbh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.epnwcf.com/Article/details/gwdpizuma.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fktsv.cn/Article/details/gxaflnwsi.sHtML

[G03] 实例属性
来源：http://read.share.fktsv.cn/Article/details/gmwvcgcxr.sHtML

Py:   self.name = "x"
来源：http://wap.vehdjk.com/Article/details/gjkwuyzth.sHtML

PHP:  public string $name = "x";
来源：http://m.share.sjlbkw.cn/Article/details/gmtyxavxc.sHtML

JS:   this.name = "x";
来源：http://read.share.epnwcf.com/Article/details/ggmznadsj.sHtML

TS:   name: string = "x";
来源：http://read.share.yfazqb.com/Article/details/gevdlyffw.sHtML

Java: private String name;
来源：http://read.share.yfazqb.com/Article/details/glndgzzwp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.epnwcf.com/Article/details/gddpyipqt.sHtML

Ruby: @name = "x"
来源：http://blog.bbcook.cn/Article/details/gmlgttiwa.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.sjlbkw.cn/Article/details/gehogdmyf.sHtML

[G04] 定义方法
来源：http://baike.yfazqb.com/Article/details/gwtfzkuod.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.vehdjk.com/Article/details/gpgesxsjy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.vehdjk.com/Article/details/gdynrunim.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.tarul.cn/Article/details/gvnhpmtws.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.epnwcf.com/Article/details/gxrtxgzqy.sHtML

Java: String greet() { return name; }
来源：http://blog.fktsv.cn/Article/details/gcniamlep.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.sjlbkw.cn/Article/details/goqsryixm.sHtML

Ruby: def greet; @name; end
来源：http://www.share.epnwcf.com/Article/details/gnwejgtvf.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.sjlbkw.cn/Article/details/guqlwedad.sHtML

[G05] 继承
来源：http://mobile.bbcook.cn/Article/details/gvmzjrimm.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fktsv.cn/Article/details/gjizkgngk.sHtML

PHP:  class Admin extends User {}
来源：http://wap.tarul.cn/Article/details/gwhxzsoed.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fktsv.cn/Article/details/gspelhqgo.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/glgschhwu.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.tarul.cn/Article/details/glrdadrxe.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.sjlbkw.cn/Article/details/gdncshmpk.sHtML

Ruby: class Admin < User; end
来源：http://blog.vehdjk.com/Article/details/gmqxmyyzi.sHtML

C#:   class Admin : User {}
来源：http://3g.sjlbkw.cn/Article/details/gazlkphli.sHtML

[G06] 重写方法
来源：http://www.share.vehdjk.com/Article/details/gddohvgkr.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.sjlbkw.cn/Article/details/gcvccaxhk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.bbcook.cn/Article/details/gboeticdo.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.epnwcf.com/Article/details/gmryoscwp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.yfazqb.com/Article/details/gzbiljmrs.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.epnwcf.com/Article/details/gnyofthpp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.tarul.cn/Article/details/ghfdbepwu.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.vehdjk.com/Article/details/gihgzmfbj.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.vehdjk.com/Article/details/gvaccoymn.sHtML

[G07] 调用父类方法
来源：http://mobile.fktsv.cn/Article/details/gdgbcfock.sHtML

Py:   super().greet()
来源：http://mobile.bbcook.cn/Article/details/gwhnqbnqe.sHtML

PHP:  parent::greet();
来源：http://www.blog.yfazqb.com/Article/details/gnlcqjklx.sHtML

JS:   super.greet();
来源：http://www.share.tarul.cn/Article/details/gphkohrzg.sHtML

TS:   super.greet();
来源：http://blog.bbcook.cn/Article/details/gpznibfpk.sHtML

Java: super.greet();
来源：http://read.share.yfazqb.com/Article/details/gaajxhool.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.sjlbkw.cn/Article/details/gizltbroi.sHtML

Ruby: super
来源：http://read.share.bbcook.cn/Article/details/gytomxzix.sHtML

C#:   base.Greet();
来源：http://m.share.tarul.cn/Article/details/gtwfenzls.sHtML

[G08] 静态方法与属性
来源：http://blog.tarul.cn/Article/details/gdyuowsgj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.yfazqb.com/Article/details/gpzqkrqwl.sHtML

PHP:  public static function f() {}
来源：http://mobile.fktsv.cn/Article/details/gwjhantho.sHtML

JS:   static f() {}
来源：http://wap.sjlbkw.cn/Article/details/gzzccopbr.sHtML

TS:   static f(): void {}
来源：http://www.share.yfazqb.com/Article/details/gnazlhasm.sHtML

Java: static void f() {}
来源：http://wap.yfazqb.com/Article/details/grzkxcsow.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.sjlbkw.cn/Article/details/gywfvubsx.sHtML

Ruby: def self.f; end
来源：http://www.m.share.epnwcf.com/Article/details/gimqgkedn.sHtML

C#:   public static void F() {}
来源：http://read.share.epnwcf.com/Article/details/gbuwgqzdm.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.yfazqb.com/Article/details/gzungqbki.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fktsv.cn/Article/details/gaxrilnuq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.bbcook.cn/Article/details/ggzlbwcyt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fktsv.cn/Article/details/gpgchtila.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.yfazqb.com/Article/details/gnuptqdcn.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.tarul.cn/Article/details/gouclmllc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fktsv.cn/Article/details/ginkhxngk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.bbcook.cn/Article/details/gbekdnofy.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.tarul.cn/Article/details/gvspnximy.sHtML

[G10] 访问控制
来源：http://read.share.vehdjk.com/Article/details/gnotmxxzy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.yfazqb.com/Article/details/gsvngfjky.sHtML

PHP:  public / protected / private
来源：http://www.share.epnwcf.com/Article/details/gctpfjsec.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.yfazqb.com/Article/details/gxannqjwi.sHtML

TS:   public / protected / private
来源：http://baike.epnwcf.com/Article/details/gzmzwqvxq.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.yfazqb.com/Article/details/ggqenhhcb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.yfazqb.com/Article/details/gwcvvozfk.sHtML

Ruby: public / protected / private
来源：http://www.blog.fktsv.cn/Article/details/gtpbdrvib.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.epnwcf.com/Article/details/gnwivsfts.sHtML

[G11] getter / setter
来源：http://read.share.fktsv.cn/Article/details/geajnafpe.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.sjlbkw.cn/Article/details/gdnufgnff.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fktsv.cn/Article/details/gsqmnyafc.sHtML

JS:   get name() { return this._name; }
来源：http://blog.sjlbkw.cn/Article/details/ggbqjulaa.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.sjlbkw.cn/Article/details/gafbhorqb.sHtML

Java: public String getName() { return name; }
来源：http://blog.vehdjk.com/Article/details/gvwoyysgh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.epnwcf.com/Article/details/gedgfdzkf.sHtML

Ruby: attr_accessor :name
来源：http://3g.bbcook.cn/Article/details/gtnfpvqyy.sHtML

C#:   public string Name { get; set; }
来源：http://3g.yfazqb.com/Article/details/gkbybelmr.sHtML

[G12] 对象转字符串
来源：http://www.blog.yfazqb.com/Article/details/gmlolkujz.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.bbcook.cn/Article/details/gdtvdbqgc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.tarul.cn/Article/details/gauvcxsye.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.bbcook.cn/Article/details/gelpeagft.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fktsv.cn/Article/details/gtlgvpuur.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/gxxzpafmv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.yfazqb.com/Article/details/gjvqrbdby.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.epnwcf.com/Article/details/gfilcihim.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fktsv.cn/Article/details/gpnbjybkr.sHtML

[G13] 判断对象类型
来源：http://wap.yfazqb.com/Article/details/gdyoeeghv.sHtML

Py:   isinstance(u, User)
来源：http://www.share.yfazqb.com/Article/details/gfgojatck.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.sjlbkw.cn/Article/details/glgltuavz.sHtML

JS:   u instanceof User
来源：http://blog.vehdjk.com/Article/details/geutytymp.sHtML

TS:   u instanceof User
来源：http://www.share.vehdjk.com/Article/details/gpuhktwxh.sHtML

Java: u instanceof User
来源：http://blog.tarul.cn/Article/details/gclfvalsr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.vehdjk.com/Article/details/gvhejeyaf.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.bbcook.cn/Article/details/gendmrsbp.sHtML

C#:   u is User
来源：http://3g.bbcook.cn/Article/details/gsnvwodrg.sHtML

[G14] 数据类 / record
来源：http://www.share.tarul.cn/Article/details/gcktwnxul.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.bbcook.cn/Article/details/gqrgnixcm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.sjlbkw.cn/Article/details/gfpthrvgd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.vehdjk.com/Article/details/gpzqaihvn.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.bbcook.cn/Article/details/gkxruwvnk.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fktsv.cn/Article/details/gogcuicpj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.yfazqb.com/Article/details/gnfgeloby.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fktsv.cn/Article/details/gcqdprilj.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.vehdjk.com/Article/details/gaiezkbeo.sHtML

[G15] 枚举
来源：http://m.share.tarul.cn/Article/details/gxootzmmb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.yfazqb.com/Article/details/gveiprolg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.bbcook.cn/Article/details/gslbnqkvd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.bbcook.cn/Article/details/gazpakxfm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.vehdjk.com/Article/details/giehxvgsm.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.sjlbkw.cn/Article/details/geegogtcw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.vehdjk.com/Article/details/gbposnebx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.epnwcf.com/Article/details/gmtgihxhr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.epnwcf.com/Article/details/gmckrqoqb.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.yfazqb.com/Article/details/gcacxbqxd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.vehdjk.com/Article/details/gixtnwtkb.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.vehdjk.com/Article/details/gmudmplxv.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.tarul.cn/Article/details/gjsukvcew.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gqhhnwuty.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.epnwcf.com/Article/details/goqvdalwh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.vehdjk.com/Article/details/gwnfjfuot.sHtML

Ruby: obj.instance_variables
来源：http://baike.fktsv.cn/Article/details/gopnjwczv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.epnwcf.com/Article/details/gbegxhodl.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/goaiaszsn.sHtML

H. 异常与错误处理
来源：http://wap.tarul.cn/Article/details/gwdqgjuci.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gyjbgappf.sHtML

[H01] try / catch 基础
来源：http://www.share.vehdjk.com/Article/details/gymlezoke.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.tarul.cn/Article/details/goiawkdfq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.sjlbkw.cn/Article/details/gaizyniaa.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.fktsv.cn/Article/details/gjesogufm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.sjlbkw.cn/Article/details/gvsgiweth.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.bbcook.cn/Article/details/ggokzhgto.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.bbcook.cn/Article/details/gdemoprvk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.tarul.cn/Article/details/gzpkoawyr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.tarul.cn/Article/details/gysxwhfrd.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.epnwcf.com/Article/details/gwxnsirrn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fktsv.cn/Article/details/ggioswxcp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.vehdjk.com/Article/details/grfomsdjy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggezvryul.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.tarul.cn/Article/details/gxtrxobfx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/gqiqfbhrr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.bbcook.cn/Article/details/gmibdnzrz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fktsv.cn/Article/details/gnikiiewt.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.epnwcf.com/Article/details/gjlsxxope.sHtML

[H03] 主动抛出异常
来源：http://www.share.sjlbkw.cn/Article/details/grwhzkdlg.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.tarul.cn/Article/details/gpkzldgki.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.sjlbkw.cn/Article/details/gmndjdkij.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.tarul.cn/Article/details/gudrkehid.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.fktsv.cn/Article/details/gapopyjat.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.sjlbkw.cn/Article/details/ghskplscu.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.fktsv.cn/Article/details/gjbvgnmhu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.bbcook.cn/Article/details/gccufwyun.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.bbcook.cn/Article/details/glkoqqrmp.sHtML

[H04] 自定义异常类型
来源：http://m.share.yfazqb.com/Article/details/glmhbvuvg.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.yfazqb.com/Article/details/gsmveaxhy.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fktsv.cn/Article/details/gnwnplfgg.sHtML

JS:   class MyError extends Error {}
来源：http://baike.sjlbkw.cn/Article/details/gnstskuaa.sHtML

TS:   class MyError extends Error {}
来源：http://blog.sjlbkw.cn/Article/details/gpdheqnxs.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.vehdjk.com/Article/details/gpnwfmywh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.sjlbkw.cn/Article/details/gudcghfhb.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.bbcook.cn/Article/details/gwxytzuji.sHtML

C#:   class MyException : Exception {}
来源：http://baike.bbcook.cn/Article/details/gdpkdhxnt.sHtML

[H05] 捕获特定类型
来源：http://www.share.bbcook.cn/Article/details/gdghiuxyj.sHtML

Py:   except ValueError as e:
来源：http://wap.sjlbkw.cn/Article/details/gbzxupmvg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.yfazqb.com/Article/details/gsuyavnpj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.vehdjk.com/Article/details/gelskbbac.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.epnwcf.com/Article/details/gfqaycqzl.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.epnwcf.com/Article/details/gegiljtgd.sHtML


<!-- 参考信息 -->