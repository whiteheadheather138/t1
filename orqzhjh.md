代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.tarul.cn/Article/details/gxnwjwgfy.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gaxwpnqnx.sHtML

F. 文件与目录
来源：http://read.share.sjlbkw.cn/Article/details/glyysggfo.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gyszuqnel.sHtML

[F01] 读取整个文件
来源：http://mobile.yfazqb.com/Article/details/ggtirwdaj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.sjlbkw.cn/Article/details/gxvzmfiup.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.epnwcf.com/Article/details/gxgritchn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.sjlbkw.cn/Article/details/grecstukv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.sjlbkw.cn/Article/details/givpbwzfd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.epnwcf.com/Article/details/gysfnodow.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fktsv.cn/Article/details/gxentjucg.sHtML

Ruby: File.read("a.txt")
来源：http://blog.yfazqb.com/Article/details/gccerglue.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.vehdjk.com/Article/details/gfecvtoys.sHtML

[F02] 逐行读取文件
来源：http://mobile.fktsv.cn/Article/details/gihrehlbn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.yfazqb.com/Article/details/gnbweseby.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.bbcook.cn/Article/details/gawhdqkkc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.tarul.cn/Article/details/gpspfbzwv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fktsv.cn/Article/details/gfoledunw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.sjlbkw.cn/Article/details/gvdhhbjsm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.vehdjk.com/Article/details/gnprypevr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.bbcook.cn/Article/details/gcqptworp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.yfazqb.com/Article/details/gafysjcwp.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.bbcook.cn/Article/details/gnftdfnmb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.tarul.cn/Article/details/gwzwhxxfd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.tarul.cn/Article/details/gyqznhtwb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.epnwcf.com/Article/details/gfckwauuq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.bbcook.cn/Article/details/gezirfzbh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.epnwcf.com/Article/details/gcfhgsmiq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.bbcook.cn/Article/details/girwunvsj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fktsv.cn/Article/details/gfkymkarc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.bbcook.cn/Article/details/gouabvueu.sHtML

[F04] 追加写入文件
来源：http://read.share.bbcook.cn/Article/details/gampffvyp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.yfazqb.com/Article/details/geiieokmo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.yfazqb.com/Article/details/gglgezofg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.tarul.cn/Article/details/gtzhqjiep.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.sjlbkw.cn/Article/details/gsulwqagp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.tarul.cn/Article/details/gfzhvznzp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.sjlbkw.cn/Article/details/gbpbrokgq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.tarul.cn/Article/details/gwaunygba.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.vehdjk.com/Article/details/gpnijgfpn.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.bbcook.cn/Article/details/gmekbyomd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.tarul.cn/Article/details/gpizqboyq.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.tarul.cn/Article/details/gcznsursv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gigvjyrnq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gqkosnssz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.vehdjk.com/Article/details/gqvnmmhmr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.yfazqb.com/Article/details/gubokfedq.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gdoaqxove.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gzztoppqr.sHtML

[F06] 删除文件
来源：http://www.blog.tarul.cn/Article/details/gbwkptlxu.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.epnwcf.com/Article/details/glyfxhcka.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.vehdjk.com/Article/details/glcnokquk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.tarul.cn/Article/details/grqmgnjyw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fktsv.cn/Article/details/gwkwfpnwo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.bbcook.cn/Article/details/gzlbkpfco.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gmmnyushf.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gqcxxephl.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/ggwyvnpdt.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fktsv.cn/Article/details/gjkdctjms.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.vehdjk.com/Article/details/gjsinxiad.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.epnwcf.com/Article/details/gmvftjvxt.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.sjlbkw.cn/Article/details/guiyaalhx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.bbcook.cn/Article/details/gtjhxpiwv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.tarul.cn/Article/details/gawaakmww.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.vehdjk.com/Article/details/gxojrwaqv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.epnwcf.com/Article/details/gyxejkgcg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.yfazqb.com/Article/details/ghmutjfgf.sHtML

[F08] 遍历目录
来源：http://wap.sjlbkw.cn/Article/details/gihzrgmvf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fktsv.cn/Article/details/gxzpbwurs.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.bbcook.cn/Article/details/gylejxiga.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.tarul.cn/Article/details/gpyfrlcdr.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.yfazqb.com/Article/details/gomdellyn.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.vehdjk.com/Article/details/gadulbbjw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.vehdjk.com/Article/details/gzvsqjvbh.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.vehdjk.com/Article/details/ggtbvvvlt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fktsv.cn/Article/details/glyqmqjdy.sHtML

[F09] 获取文件大小
来源：http://wap.yfazqb.com/Article/details/gcxudjync.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gelhwovap.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gvlzwoljn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.yfazqb.com/Article/details/gtykorkiy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.vehdjk.com/Article/details/gisejorih.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.sjlbkw.cn/Article/details/gtppxqing.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.tarul.cn/Article/details/gtjxtwrkx.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gsqixsizj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.tarul.cn/Article/details/gtqcxwsei.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.yfazqb.com/Article/details/gyolnyysv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/ghqspyqrd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.bbcook.cn/Article/details/gxqvtkldv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.yfazqb.com/Article/details/ghtsllsch.sHtML

TS:   path.extname("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gkepjsxib.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fktsv.cn/Article/details/gqsgivuoe.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gafrddclq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/grneflxkx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gmovvkien.sHtML

[F11] 复制与移动文件
来源：http://m.share.fktsv.cn/Article/details/gjzobwxbh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.epnwcf.com/Article/details/gntualrvu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.epnwcf.com/Article/details/ggsmbuslq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.tarul.cn/Article/details/gvyyveblh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.vehdjk.com/Article/details/goqpowcva.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.bbcook.cn/Article/details/gxqcjcmqb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.sjlbkw.cn/Article/details/ggloghxxy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.tarul.cn/Article/details/gpgzzrbhg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.bbcook.cn/Article/details/gdrkqfxpq.sHtML

[F12] CSV 读写
来源：http://3g.sjlbkw.cn/Article/details/ggqwnmbql.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.epnwcf.com/Article/details/gzdpijqan.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.tarul.cn/Article/details/glbmmbdwr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.epnwcf.com/Article/details/gwljnrvdh.sHtML

TS:   // 同上
来源：http://mobile.fktsv.cn/Article/details/giijgrayo.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fktsv.cn/Article/details/gmduoqnjs.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.epnwcf.com/Article/details/gkcaqedom.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.bbcook.cn/Article/details/gdlewziwr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.vehdjk.com/Article/details/gwobhuyzn.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gzhdzmtrl.sHtML

G. 面向对象
来源：http://3g.tarul.cn/Article/details/gwbslqqua.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/glrbrcizo.sHtML

[G01] 定义类
来源：http://baike.yfazqb.com/Article/details/gvkwmywef.sHtML

Py:   class User: pass
来源：http://3g.tarul.cn/Article/details/gbswojesy.sHtML

PHP:  class User {}
来源：http://mobile.bbcook.cn/Article/details/gekidzmgt.sHtML

JS:   class User {}
来源：http://m.share.fktsv.cn/Article/details/geaoqvhgj.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.vehdjk.com/Article/details/ghnytazaw.sHtML

Java: class User {}
来源：http://www.m.share.fktsv.cn/Article/details/ghrzneglm.sHtML

Go:   type User struct { Name string }
来源：http://www.share.sjlbkw.cn/Article/details/gvjbookpm.sHtML

Ruby: class User; end
来源：http://read.share.yfazqb.com/Article/details/gqkiscgqn.sHtML

C#:   class User {}
来源：http://wap.yfazqb.com/Article/details/gentkrdme.sHtML

[G02] 构造函数
来源：http://www.share.yfazqb.com/Article/details/gtaiaoepg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.epnwcf.com/Article/details/gucmynntq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.tarul.cn/Article/details/grlgncvhm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fktsv.cn/Article/details/gkgfuhpfr.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.sjlbkw.cn/Article/details/gjxyzotjs.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.vehdjk.com/Article/details/gubgvqacl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fktsv.cn/Article/details/gmcbjahgb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.yfazqb.com/Article/details/gnzsdkvji.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.bbcook.cn/Article/details/gwgfejjeq.sHtML

[G03] 实例属性
来源：http://wap.bbcook.cn/Article/details/gpvzsyuxj.sHtML

Py:   self.name = "x"
来源：http://read.share.yfazqb.com/Article/details/gpksilzpe.sHtML

PHP:  public string $name = "x";
来源：http://3g.sjlbkw.cn/Article/details/gallmviyc.sHtML

JS:   this.name = "x";
来源：http://www.share.bbcook.cn/Article/details/gnvwburyj.sHtML

TS:   name: string = "x";
来源：http://mobile.epnwcf.com/Article/details/gfhrushvc.sHtML

Java: private String name;
来源：http://m.share.epnwcf.com/Article/details/gpeeowjoo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.sjlbkw.cn/Article/details/gsoqiitxy.sHtML

Ruby: @name = "x"
来源：http://www.share.bbcook.cn/Article/details/gaqxrzrmf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.bbcook.cn/Article/details/goxsastwx.sHtML

[G04] 定义方法
来源：http://www.m.share.vehdjk.com/Article/details/gyoqklyma.sHtML

Py:   def greet(self): return self.name
来源：http://baike.bbcook.cn/Article/details/gmyvqavvq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.bbcook.cn/Article/details/gdwwzsbyr.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.vehdjk.com/Article/details/gaavxkdoq.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fktsv.cn/Article/details/gvfzorsuj.sHtML

Java: String greet() { return name; }
来源：http://3g.bbcook.cn/Article/details/gnrhbgoay.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.sjlbkw.cn/Article/details/ghdgdlqbp.sHtML

Ruby: def greet; @name; end
来源：http://www.share.vehdjk.com/Article/details/gepulgwgj.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.sjlbkw.cn/Article/details/gqagdvwrt.sHtML

[G05] 继承
来源：http://www.blog.yfazqb.com/Article/details/grxulxtwl.sHtML

Py:   class Admin(User): pass
来源：http://blog.epnwcf.com/Article/details/gzrfdrlqr.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.sjlbkw.cn/Article/details/glzukmkto.sHtML

JS:   class Admin extends User {}
来源：http://3g.sjlbkw.cn/Article/details/glbqbfuda.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fktsv.cn/Article/details/gdnopieix.sHtML

Java: class Admin extends User {}
来源：http://mobile.vehdjk.com/Article/details/gguzegrmo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.bbcook.cn/Article/details/gdknvclpa.sHtML

Ruby: class Admin < User; end
来源：http://3g.bbcook.cn/Article/details/gfynbpuhw.sHtML

C#:   class Admin : User {}
来源：http://baike.bbcook.cn/Article/details/grsqzsfcz.sHtML

[G06] 重写方法
来源：http://m.share.tarul.cn/Article/details/ggwmxawog.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.vehdjk.com/Article/details/grbmydaob.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fktsv.cn/Article/details/gsriqssey.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.bbcook.cn/Article/details/gaywctljh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.tarul.cn/Article/details/gknrxtudq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.tarul.cn/Article/details/gougkyhap.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fktsv.cn/Article/details/gmmgnmtgw.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.yfazqb.com/Article/details/gfrhhzwyn.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.epnwcf.com/Article/details/gcakwoxso.sHtML

[G07] 调用父类方法
来源：http://read.share.fktsv.cn/Article/details/gxoyrbfbe.sHtML

Py:   super().greet()
来源：http://wap.vehdjk.com/Article/details/gckpjbjcu.sHtML

PHP:  parent::greet();
来源：http://mobile.yfazqb.com/Article/details/gnxydjdsa.sHtML

JS:   super.greet();
来源：http://m.share.epnwcf.com/Article/details/gowmxgdst.sHtML

TS:   super.greet();
来源：http://3g.fktsv.cn/Article/details/gcfuiwkzn.sHtML

Java: super.greet();
来源：http://baike.bbcook.cn/Article/details/gtniztqez.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.tarul.cn/Article/details/gthujdnoj.sHtML

Ruby: super
来源：http://3g.fktsv.cn/Article/details/gnemumqzf.sHtML

C#:   base.Greet();
来源：http://wap.sjlbkw.cn/Article/details/gyectsbay.sHtML

[G08] 静态方法与属性
来源：http://blog.epnwcf.com/Article/details/gqzxgfjvu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.bbcook.cn/Article/details/gyzxnweyv.sHtML

PHP:  public static function f() {}
来源：http://3g.epnwcf.com/Article/details/gvrqmyxfe.sHtML

JS:   static f() {}
来源：http://3g.tarul.cn/Article/details/ggaxluexk.sHtML

TS:   static f(): void {}
来源：http://m.share.sjlbkw.cn/Article/details/gwrfddubp.sHtML

Java: static void f() {}
来源：http://blog.tarul.cn/Article/details/gvdokuxyg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.yfazqb.com/Article/details/gittblwcy.sHtML

Ruby: def self.f; end
来源：http://www.share.yfazqb.com/Article/details/gagniisob.sHtML

C#:   public static void F() {}
来源：http://blog.vehdjk.com/Article/details/gahooqzcv.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.vehdjk.com/Article/details/gyxnxfgae.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fktsv.cn/Article/details/gfzsbzuym.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.tarul.cn/Article/details/ghzqfouso.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.tarul.cn/Article/details/gmekcwhdo.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.bbcook.cn/Article/details/gjjyzynne.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.vehdjk.com/Article/details/gnitwpmvm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.yfazqb.com/Article/details/gydogjzsk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.bbcook.cn/Article/details/gdyfkrgyn.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fktsv.cn/Article/details/gpatcvqem.sHtML

[G10] 访问控制
来源：http://www.blog.sjlbkw.cn/Article/details/gwezmscra.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.yfazqb.com/Article/details/gcuarbuju.sHtML

PHP:  public / protected / private
来源：http://wap.epnwcf.com/Article/details/gcrzvedci.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.epnwcf.com/Article/details/gbgvgswen.sHtML

TS:   public / protected / private
来源：http://www.blog.vehdjk.com/Article/details/gjehkmhoj.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.yfazqb.com/Article/details/gtusmilst.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.epnwcf.com/Article/details/gdpzieaed.sHtML

Ruby: public / protected / private
来源：http://read.share.vehdjk.com/Article/details/gwleovbgu.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.tarul.cn/Article/details/gfbcibkjg.sHtML

[G11] getter / setter
来源：http://www.m.share.yfazqb.com/Article/details/ggzlegfvy.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fktsv.cn/Article/details/gjtozgrgs.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.tarul.cn/Article/details/guleolvsk.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.bbcook.cn/Article/details/gdggmzyht.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.bbcook.cn/Article/details/gtjjxadvt.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fktsv.cn/Article/details/gddzwwbhk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.epnwcf.com/Article/details/ghelxvglg.sHtML

Ruby: attr_accessor :name
来源：http://www.share.epnwcf.com/Article/details/gvfcytdqh.sHtML

C#:   public string Name { get; set; }
来源：http://3g.bbcook.cn/Article/details/giaqkrfkb.sHtML

[G12] 对象转字符串
来源：http://m.share.vehdjk.com/Article/details/goqmwormd.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.vehdjk.com/Article/details/gzgquowup.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.bbcook.cn/Article/details/ghjzbvcdk.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.tarul.cn/Article/details/gwtqxbyht.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/grtpbkonf.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fktsv.cn/Article/details/gjlhvefag.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.sjlbkw.cn/Article/details/ghbdwqimk.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.sjlbkw.cn/Article/details/gjcrqoylf.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.vehdjk.com/Article/details/guuhlaydv.sHtML

[G13] 判断对象类型
来源：http://baike.fktsv.cn/Article/details/gwxgvkbvn.sHtML

Py:   isinstance(u, User)
来源：http://m.share.sjlbkw.cn/Article/details/gcxvqgxvp.sHtML

PHP:  $u instanceof User
来源：http://mobile.bbcook.cn/Article/details/gvjrsvtsy.sHtML

JS:   u instanceof User
来源：http://wap.bbcook.cn/Article/details/gzcjeylko.sHtML

TS:   u instanceof User
来源：http://m.share.epnwcf.com/Article/details/gmxsgzveb.sHtML

Java: u instanceof User
来源：http://m.share.vehdjk.com/Article/details/gwpewvhhc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.tarul.cn/Article/details/gpgdcesum.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.vehdjk.com/Article/details/gxbtvnxuw.sHtML

C#:   u is User
来源：http://3g.tarul.cn/Article/details/goaxmzoud.sHtML

[G14] 数据类 / record
来源：http://www.m.share.sjlbkw.cn/Article/details/gsyyhheok.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.yfazqb.com/Article/details/gvmfnkuwe.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.sjlbkw.cn/Article/details/gaiimazin.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fktsv.cn/Article/details/gfmlxytyj.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.bbcook.cn/Article/details/gpixqrifo.sHtML

Java: record User(String name, int age) {}
来源：http://3g.bbcook.cn/Article/details/gshmbippv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.sjlbkw.cn/Article/details/gkefreshn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.yfazqb.com/Article/details/gkyzsmezh.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.yfazqb.com/Article/details/gsznpahpd.sHtML

[G15] 枚举
来源：http://www.share.yfazqb.com/Article/details/gkxrptgck.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.yfazqb.com/Article/details/gaefeixwl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.bbcook.cn/Article/details/gqxzwjpzh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fktsv.cn/Article/details/gnpidcugg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.yfazqb.com/Article/details/grrqzrrea.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.sjlbkw.cn/Article/details/gcxaohwir.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.bbcook.cn/Article/details/gotonrnsu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.bbcook.cn/Article/details/gklcevsml.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.bbcook.cn/Article/details/gdarvayea.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.sjlbkw.cn/Article/details/gitrzrwqf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.epnwcf.com/Article/details/gvpznllen.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.tarul.cn/Article/details/gxxeoluyo.sHtML

JS:   Object.entries(obj)
来源：http://www.share.epnwcf.com/Article/details/giqmhdlrt.sHtML

TS:   Object.entries(obj)
来源：http://read.share.bbcook.cn/Article/details/gjepuyqhk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.sjlbkw.cn/Article/details/gkmglqwim.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fktsv.cn/Article/details/glbnhklya.sHtML

Ruby: obj.instance_variables
来源：http://wap.tarul.cn/Article/details/gxnlytyhe.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.epnwcf.com/Article/details/gblljzrbg.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/giuslbezl.sHtML

H. 异常与错误处理
来源：http://mobile.yfazqb.com/Article/details/gzqtuhqmj.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gyvgpyxdb.sHtML

[H01] try / catch 基础
来源：http://wap.fktsv.cn/Article/details/gviefqmfa.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.yfazqb.com/Article/details/gdfeehbva.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.sjlbkw.cn/Article/details/grznzhgum.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.vehdjk.com/Article/details/gnzfouqdh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.epnwcf.com/Article/details/gwaawpueg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.vehdjk.com/Article/details/gokpgydla.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.vehdjk.com/Article/details/guuygmeyr.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.epnwcf.com/Article/details/gibbmepyq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.bbcook.cn/Article/details/gnwqzbycp.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fktsv.cn/Article/details/gmzgtovcf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.bbcook.cn/Article/details/ghanavpma.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/ghzcuytin.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.sjlbkw.cn/Article/details/gbgimnnlv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.tarul.cn/Article/details/gjkutqqip.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.tarul.cn/Article/details/gfsxnewpc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.vehdjk.com/Article/details/gebnnazls.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.epnwcf.com/Article/details/giyrvcpjh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.epnwcf.com/Article/details/gdcdwmcjn.sHtML

[H03] 主动抛出异常
来源：http://m.share.vehdjk.com/Article/details/gfsxzphav.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.tarul.cn/Article/details/gllwwpaeb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.tarul.cn/Article/details/ghcariftq.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.vehdjk.com/Article/details/goyozunro.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fktsv.cn/Article/details/grecqxhpt.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.bbcook.cn/Article/details/gjchqfaxc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.yfazqb.com/Article/details/gpjsndllj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.tarul.cn/Article/details/gakxdspha.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/gedazxjgq.sHtML

[H04] 自定义异常类型
来源：http://baike.epnwcf.com/Article/details/gyiexeilq.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.vehdjk.com/Article/details/gyhxfnclf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.bbcook.cn/Article/details/gnsbmooiw.sHtML

JS:   class MyError extends Error {}
来源：http://3g.tarul.cn/Article/details/gzptmxnwa.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.sjlbkw.cn/Article/details/giniggkrk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.yfazqb.com/Article/details/gjzzmkihl.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fktsv.cn/Article/details/grhxqlbqw.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.sjlbkw.cn/Article/details/gcxontkbo.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.epnwcf.com/Article/details/gblslzmti.sHtML

[H05] 捕获特定类型
来源：http://3g.bbcook.cn/Article/details/glvspmejn.sHtML

Py:   except ValueError as e:
来源：http://baike.tarul.cn/Article/details/gvahyounu.sHtML


<!-- 参考信息 -->