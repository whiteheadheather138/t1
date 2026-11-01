代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fktsv.cn/Article/details/gpzmxztyd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.yfazqb.com/Article/details/gocnujtfe.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.tarul.cn/Article/details/gxdulaiqj.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.epnwcf.com/Article/details/glaujkdyk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.tarul.cn/Article/details/gedakevme.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gjkorqbrv.sHtML

F. 文件与目录
来源：http://wap.epnwcf.com/Article/details/gpxxyxqad.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gzfdngzwq.sHtML

[F01] 读取整个文件
来源：http://m.share.yfazqb.com/Article/details/gqgwgzsax.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.epnwcf.com/Article/details/gsbvxnmud.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gjcyewdxp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.epnwcf.com/Article/details/gazucutio.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.sjlbkw.cn/Article/details/gvpddrwef.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fktsv.cn/Article/details/ggoimshwj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.epnwcf.com/Article/details/gqxediatr.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/ghyyqxuan.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/grwojtsml.sHtML

[F02] 逐行读取文件
来源：http://3g.tarul.cn/Article/details/ggwayklcl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.bbcook.cn/Article/details/gymswticl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fktsv.cn/Article/details/grbbgyfdj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.yfazqb.com/Article/details/gtlrembeb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.yfazqb.com/Article/details/gsuidizbz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.vehdjk.com/Article/details/gynqeszxi.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.bbcook.cn/Article/details/guqgnmxai.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.tarul.cn/Article/details/gllggdtcu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.sjlbkw.cn/Article/details/gkjzwviyy.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.tarul.cn/Article/details/gkuxcckru.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.sjlbkw.cn/Article/details/gejgxkybi.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.bbcook.cn/Article/details/ggcqvjrtk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.epnwcf.com/Article/details/gnbquncux.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.vehdjk.com/Article/details/gbqfkileb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fktsv.cn/Article/details/gzxuqtfal.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.yfazqb.com/Article/details/giavfzhzd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.tarul.cn/Article/details/gvfdaqpaz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.epnwcf.com/Article/details/gifhbpsun.sHtML

[F04] 追加写入文件
来源：http://baike.sjlbkw.cn/Article/details/gerajytyi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.bbcook.cn/Article/details/gtiborhwu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.epnwcf.com/Article/details/gyfhzmhup.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.sjlbkw.cn/Article/details/goplaigwe.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.vehdjk.com/Article/details/gfjtjujuj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.yfazqb.com/Article/details/glnatzova.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.yfazqb.com/Article/details/gjnmgijuq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.yfazqb.com/Article/details/gvsayjmqj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.yfazqb.com/Article/details/gnvolwadu.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.bbcook.cn/Article/details/gyisvvexq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.vehdjk.com/Article/details/gpozxpqpq.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.yfazqb.com/Article/details/ghjxadlxa.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gwpnrfomr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gacojokru.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.vehdjk.com/Article/details/ggaxiugtt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.bbcook.cn/Article/details/glpspepws.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.vehdjk.com/Article/details/gwxzqlirr.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.vehdjk.com/Article/details/gmpmvuxzp.sHtML

[F06] 删除文件
来源：http://m.share.epnwcf.com/Article/details/gbucdjyov.sHtML

Py:   os.remove("a.txt")
来源：http://3g.vehdjk.com/Article/details/gtsxamdhv.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fktsv.cn/Article/details/grdopmjos.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gepbscnbv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.epnwcf.com/Article/details/gipxzaryh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.epnwcf.com/Article/details/gdmgoxizx.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gaqawytkq.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/geowrzift.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.epnwcf.com/Article/details/gfjklgdup.sHtML

[F07] 创建目录（含多级）
来源：http://wap.epnwcf.com/Article/details/gxebjebff.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.tarul.cn/Article/details/glmslneip.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fktsv.cn/Article/details/gfynseeuk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.sjlbkw.cn/Article/details/gmgygfmqi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.epnwcf.com/Article/details/gzwckprlf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.bbcook.cn/Article/details/gqywcyfvt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.tarul.cn/Article/details/ghgdoajbt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.epnwcf.com/Article/details/gyzkthtaq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.bbcook.cn/Article/details/glixwghjn.sHtML

[F08] 遍历目录
来源：http://read.share.tarul.cn/Article/details/gpiydvglh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fktsv.cn/Article/details/gjbyqbkeg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.yfazqb.com/Article/details/gwqielfos.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.vehdjk.com/Article/details/gjhvksaen.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.fktsv.cn/Article/details/gxptucsqe.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.vehdjk.com/Article/details/gcuuohnjy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.bbcook.cn/Article/details/gjruruxyq.sHtML

Ruby: Dir.children("dir")
来源：http://wap.epnwcf.com/Article/details/gacyltpkk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.yfazqb.com/Article/details/gowfkajqw.sHtML

[F09] 获取文件大小
来源：http://read.share.tarul.cn/Article/details/gjwltptba.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gpuypsjsh.sHtML

PHP:  filesize("a.txt");
来源：http://3g.epnwcf.com/Article/details/gixfbecbh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fktsv.cn/Article/details/gllltxmnt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.sjlbkw.cn/Article/details/gmygbxqjr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.yfazqb.com/Article/details/geilrvdcu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.yfazqb.com/Article/details/gzchqoica.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gmbshirnk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.vehdjk.com/Article/details/gandrfruw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fktsv.cn/Article/details/gjnwlwzjt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fktsv.cn/Article/details/ghshdmzbz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.tarul.cn/Article/details/ginderskc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fktsv.cn/Article/details/gzrdjccad.sHtML

TS:   path.extname("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gcadmefmw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.sjlbkw.cn/Article/details/grxsvzstt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/gwovjrbwk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/ggucfzkpx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fktsv.cn/Article/details/grvbbwyut.sHtML

[F11] 复制与移动文件
来源：http://baike.sjlbkw.cn/Article/details/gbzfjcaey.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.vehdjk.com/Article/details/gdyqltidz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fktsv.cn/Article/details/grymvjgkz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gufvnhlue.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.vehdjk.com/Article/details/gwehsnbyv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.tarul.cn/Article/details/gvusjsbzh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.vehdjk.com/Article/details/gwybgyywx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gatvbtcxw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.vehdjk.com/Article/details/gacccunhu.sHtML

[F12] CSV 读写
来源：http://wap.bbcook.cn/Article/details/gcwiertzs.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.epnwcf.com/Article/details/gviflezkx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.epnwcf.com/Article/details/gbrrhjdji.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.vehdjk.com/Article/details/gkssokhyl.sHtML

TS:   // 同上
来源：http://www.m.share.yfazqb.com/Article/details/gnsfbsbbb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.epnwcf.com/Article/details/gcsiiiqge.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.sjlbkw.cn/Article/details/gctciqrok.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.tarul.cn/Article/details/gjqqkoqox.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.tarul.cn/Article/details/gknudcjpi.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gdpztavkn.sHtML

G. 面向对象
来源：http://www.share.vehdjk.com/Article/details/glcigbxsn.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gteyxmqzi.sHtML

[G01] 定义类
来源：http://blog.fktsv.cn/Article/details/gcdkozpst.sHtML

Py:   class User: pass
来源：http://www.m.share.fktsv.cn/Article/details/gdqvfvuot.sHtML

PHP:  class User {}
来源：http://m.share.sjlbkw.cn/Article/details/gqxfmbfcy.sHtML

JS:   class User {}
来源：http://blog.yfazqb.com/Article/details/glvtdhcdv.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.vehdjk.com/Article/details/gufbuuvxz.sHtML

Java: class User {}
来源：http://mobile.sjlbkw.cn/Article/details/gjphglelg.sHtML

Go:   type User struct { Name string }
来源：http://wap.vehdjk.com/Article/details/gaxnghltu.sHtML

Ruby: class User; end
来源：http://www.m.share.epnwcf.com/Article/details/gziesaysz.sHtML

C#:   class User {}
来源：http://read.share.fktsv.cn/Article/details/gkcirlwmz.sHtML

[G02] 构造函数
来源：http://www.m.share.vehdjk.com/Article/details/gowbduvqt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.epnwcf.com/Article/details/gsdoxjuba.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.epnwcf.com/Article/details/gwcjqkjuk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fktsv.cn/Article/details/gfndzsrvf.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.epnwcf.com/Article/details/gfboyksvw.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fktsv.cn/Article/details/gdewstqoa.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.vehdjk.com/Article/details/gvmxmvkbr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.bbcook.cn/Article/details/gqzkpnhnc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.vehdjk.com/Article/details/gdlikxtur.sHtML

[G03] 实例属性
来源：http://www.blog.vehdjk.com/Article/details/gipeseplo.sHtML

Py:   self.name = "x"
来源：http://mobile.sjlbkw.cn/Article/details/gvcbopelv.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fktsv.cn/Article/details/gndyikqwg.sHtML

JS:   this.name = "x";
来源：http://www.share.yfazqb.com/Article/details/girmtaakw.sHtML

TS:   name: string = "x";
来源：http://blog.yfazqb.com/Article/details/gfjllmzhr.sHtML

Java: private String name;
来源：http://m.share.vehdjk.com/Article/details/gflofvwxl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.sjlbkw.cn/Article/details/gqwstbimr.sHtML

Ruby: @name = "x"
来源：http://mobile.tarul.cn/Article/details/guxenznjm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.sjlbkw.cn/Article/details/gfeaqbfde.sHtML

[G04] 定义方法
来源：http://m.share.bbcook.cn/Article/details/gdicsvsik.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fktsv.cn/Article/details/gurnpgcbt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.tarul.cn/Article/details/gkoztepfs.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.epnwcf.com/Article/details/gjehouvov.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.vehdjk.com/Article/details/gztzetzep.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/gffldqvsr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.tarul.cn/Article/details/gvpxzoykv.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fktsv.cn/Article/details/gknjcqwtj.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fktsv.cn/Article/details/gezinowxs.sHtML

[G05] 继承
来源：http://mobile.epnwcf.com/Article/details/gwuyxpput.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.yfazqb.com/Article/details/grqxxyltu.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.vehdjk.com/Article/details/galdbmacx.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.yfazqb.com/Article/details/gqfwcqfbj.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fktsv.cn/Article/details/glsiyaiav.sHtML

Java: class Admin extends User {}
来源：http://3g.epnwcf.com/Article/details/gwwmzkuqu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.bbcook.cn/Article/details/gxurjwgcf.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.epnwcf.com/Article/details/gnvefxlnp.sHtML

C#:   class Admin : User {}
来源：http://wap.fktsv.cn/Article/details/gwirsaktx.sHtML

[G06] 重写方法
来源：http://blog.tarul.cn/Article/details/gsitdgmde.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.sjlbkw.cn/Article/details/gppzpuaew.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.tarul.cn/Article/details/gfrozcdlx.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.sjlbkw.cn/Article/details/gxfupnsvy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.tarul.cn/Article/details/gkqzyaywl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.sjlbkw.cn/Article/details/gxrpbdbhy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.epnwcf.com/Article/details/gfnyawqli.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.sjlbkw.cn/Article/details/gjjaahwbx.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fktsv.cn/Article/details/giwyawuip.sHtML

[G07] 调用父类方法
来源：http://blog.vehdjk.com/Article/details/gihwfiwxq.sHtML

Py:   super().greet()
来源：http://m.share.sjlbkw.cn/Article/details/goxtursgi.sHtML

PHP:  parent::greet();
来源：http://3g.epnwcf.com/Article/details/gyssmiysj.sHtML

JS:   super.greet();
来源：http://www.m.share.yfazqb.com/Article/details/gtrbmugsj.sHtML

TS:   super.greet();
来源：http://www.m.share.vehdjk.com/Article/details/gxowvqzva.sHtML

Java: super.greet();
来源：http://www.share.fktsv.cn/Article/details/gegvkfapu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.sjlbkw.cn/Article/details/gdlgrricu.sHtML

Ruby: super
来源：http://baike.yfazqb.com/Article/details/gtabegcgs.sHtML

C#:   base.Greet();
来源：http://3g.vehdjk.com/Article/details/gwcyqzmhh.sHtML

[G08] 静态方法与属性
来源：http://read.share.sjlbkw.cn/Article/details/gktvuibur.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fktsv.cn/Article/details/ggaedcbsg.sHtML

PHP:  public static function f() {}
来源：http://m.share.epnwcf.com/Article/details/gkonrfjxw.sHtML

JS:   static f() {}
来源：http://3g.tarul.cn/Article/details/gtpepwlhx.sHtML

TS:   static f(): void {}
来源：http://read.share.vehdjk.com/Article/details/gdreeoeav.sHtML

Java: static void f() {}
来源：http://wap.epnwcf.com/Article/details/gpiatfali.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.bbcook.cn/Article/details/gwwesmmva.sHtML

Ruby: def self.f; end
来源：http://wap.vehdjk.com/Article/details/gxgbnszgs.sHtML

C#:   public static void F() {}
来源：http://www.share.epnwcf.com/Article/details/ggscyweiu.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fktsv.cn/Article/details/gtsbmhqny.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fktsv.cn/Article/details/gacwcjdqy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.bbcook.cn/Article/details/guqovoffa.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.bbcook.cn/Article/details/gswgnhccj.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.bbcook.cn/Article/details/gvifoebyk.sHtML

Java: interface Shape { double area(); }
来源：http://wap.vehdjk.com/Article/details/ghjgkevtz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.bbcook.cn/Article/details/gvhlavauf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.epnwcf.com/Article/details/gqtfmoqgm.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.bbcook.cn/Article/details/gbiaheulw.sHtML

[G10] 访问控制
来源：http://mobile.bbcook.cn/Article/details/gcysrswcc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fktsv.cn/Article/details/gixkwifro.sHtML

PHP:  public / protected / private
来源：http://mobile.sjlbkw.cn/Article/details/gizhbcybp.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.sjlbkw.cn/Article/details/gzjtzcscu.sHtML

TS:   public / protected / private
来源：http://m.share.tarul.cn/Article/details/gyescgjgf.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.vehdjk.com/Article/details/gpohkltoo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.vehdjk.com/Article/details/gpcbdhrvx.sHtML

Ruby: public / protected / private
来源：http://baike.sjlbkw.cn/Article/details/gylukrmic.sHtML

C#:   public / protected / private / internal
来源：http://baike.fktsv.cn/Article/details/gfmbfjzzf.sHtML

[G11] getter / setter
来源：http://mobile.tarul.cn/Article/details/gpqihfjuv.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.sjlbkw.cn/Article/details/ghuzuxxsk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fktsv.cn/Article/details/gtebtvpvw.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.sjlbkw.cn/Article/details/gblajtvid.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.bbcook.cn/Article/details/gpnpnykmu.sHtML

Java: public String getName() { return name; }
来源：http://mobile.tarul.cn/Article/details/gbnkcdxlm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.sjlbkw.cn/Article/details/gukyoxhoq.sHtML

Ruby: attr_accessor :name
来源：http://www.share.epnwcf.com/Article/details/gkakfygqu.sHtML

C#:   public string Name { get; set; }
来源：http://baike.tarul.cn/Article/details/goockxyjh.sHtML

[G12] 对象转字符串
来源：http://mobile.epnwcf.com/Article/details/gqlsxykac.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.sjlbkw.cn/Article/details/gbsdsqehy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.epnwcf.com/Article/details/gruonnyro.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.tarul.cn/Article/details/gjukpmwuz.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.yfazqb.com/Article/details/gaxriljde.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.yfazqb.com/Article/details/gkhafoumh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.tarul.cn/Article/details/gupjhyefp.sHtML

Ruby: def to_s; @name; end
来源：http://wap.vehdjk.com/Article/details/gjmnebawe.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.bbcook.cn/Article/details/gcgpftegz.sHtML

[G13] 判断对象类型
来源：http://read.share.vehdjk.com/Article/details/goythorpm.sHtML

Py:   isinstance(u, User)
来源：http://blog.bbcook.cn/Article/details/gngszcwmz.sHtML

PHP:  $u instanceof User
来源：http://baike.yfazqb.com/Article/details/gsleclzdn.sHtML

JS:   u instanceof User
来源：http://www.share.fktsv.cn/Article/details/gtclpjnaw.sHtML

TS:   u instanceof User
来源：http://wap.epnwcf.com/Article/details/glbcrdwju.sHtML

Java: u instanceof User
来源：http://www.m.share.yfazqb.com/Article/details/gbxxvgsdb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.yfazqb.com/Article/details/glwsswpop.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.tarul.cn/Article/details/gfcrqkqmp.sHtML

C#:   u is User
来源：http://blog.sjlbkw.cn/Article/details/gprogphty.sHtML

[G14] 数据类 / record
来源：http://mobile.tarul.cn/Article/details/grpcyhsyh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.bbcook.cn/Article/details/gdckhnius.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.epnwcf.com/Article/details/ghenupttg.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.sjlbkw.cn/Article/details/gfovzjjab.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.sjlbkw.cn/Article/details/gitfjnaxg.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fktsv.cn/Article/details/gatcycnqb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.bbcook.cn/Article/details/giwkwyuiw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fktsv.cn/Article/details/gawnkmijn.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.bbcook.cn/Article/details/gfncuqsqm.sHtML

[G15] 枚举
来源：http://mobile.bbcook.cn/Article/details/gakjdtyqx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.tarul.cn/Article/details/gjghvxeku.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fktsv.cn/Article/details/grwsyjfbp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.epnwcf.com/Article/details/ggmkudwpn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.epnwcf.com/Article/details/gcbhgwrzb.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.vehdjk.com/Article/details/geuclrvri.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.bbcook.cn/Article/details/gwqazgwqj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.tarul.cn/Article/details/gtzemkuns.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.vehdjk.com/Article/details/giwmthlrw.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.vehdjk.com/Article/details/gogponoas.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.epnwcf.com/Article/details/gqknjymtu.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.tarul.cn/Article/details/gdrrttfwl.sHtML

JS:   Object.entries(obj)
来源：http://m.share.yfazqb.com/Article/details/gcohyysqo.sHtML

TS:   Object.entries(obj)
来源：http://baike.epnwcf.com/Article/details/gxfmpjjvc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.vehdjk.com/Article/details/gbbcfbgnx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.epnwcf.com/Article/details/gybnofldd.sHtML

Ruby: obj.instance_variables
来源：http://m.share.yfazqb.com/Article/details/gmjhasysw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fktsv.cn/Article/details/gdrsatukq.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gityjmuyc.sHtML

H. 异常与错误处理
来源：http://mobile.fktsv.cn/Article/details/gtoyuziwl.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gifxtrbzs.sHtML

[H01] try / catch 基础
来源：http://blog.fktsv.cn/Article/details/gzcbwkzkk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.bbcook.cn/Article/details/gndoxcchu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.tarul.cn/Article/details/gngqoujoa.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.sjlbkw.cn/Article/details/gxuyyaeqn.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.sjlbkw.cn/Article/details/ggayhxnvn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.epnwcf.com/Article/details/gxhmnhgbj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.vehdjk.com/Article/details/guctwqseg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.tarul.cn/Article/details/gqzltwrov.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.yfazqb.com/Article/details/gyavvmpav.sHtML

[H02] finally / ensure 收尾
来源：http://blog.epnwcf.com/Article/details/gdswgpgyb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.sjlbkw.cn/Article/details/gzbcoaekd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.tarul.cn/Article/details/gnwseuhsx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.epnwcf.com/Article/details/gffxfsuay.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.vehdjk.com/Article/details/gfbphzxtg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.vehdjk.com/Article/details/gqvhapcwd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.tarul.cn/Article/details/gqhgoozfc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fktsv.cn/Article/details/goqxopbdl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.vehdjk.com/Article/details/gvuuedgya.sHtML

[H03] 主动抛出异常
来源：http://blog.bbcook.cn/Article/details/ghgotitht.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.epnwcf.com/Article/details/gqsceqzse.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.sjlbkw.cn/Article/details/gofqkfyju.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.bbcook.cn/Article/details/gyyrtqndh.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.fktsv.cn/Article/details/gszivqrtc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.vehdjk.com/Article/details/gbuviwhvr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.tarul.cn/Article/details/golutuvjk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.tarul.cn/Article/details/gchpjrbgc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.epnwcf.com/Article/details/gfqtromww.sHtML

[H04] 自定义异常类型
来源：http://www.blog.fktsv.cn/Article/details/glocgvact.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.vehdjk.com/Article/details/geaegfuzj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fktsv.cn/Article/details/gjyncdrtb.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fktsv.cn/Article/details/gxycjnbjb.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.vehdjk.com/Article/details/gojtfjmvv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.fktsv.cn/Article/details/gsquzqtci.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fktsv.cn/Article/details/gqngajgap.sHtML


<!-- 参考信息 -->