代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fktsv.cn/Article/details/gctdsyqts.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.sjlbkw.cn/Article/details/glpqfqpmy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.vehdjk.com/Article/details/gpqnljlzr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.yfazqb.com/Article/details/gemxqxubh.sHtML

[E22] 字节长度与字符长度
来源：http://baike.sjlbkw.cn/Article/details/gfmaxucch.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.vehdjk.com/Article/details/gapiagnpt.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.vehdjk.com/Article/details/gkohcgizl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.vehdjk.com/Article/details/gidsbpcck.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.tarul.cn/Article/details/gkvibcoql.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.yfazqb.com/Article/details/ghocjijxx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fktsv.cn/Article/details/gqvxuomse.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.epnwcf.com/Article/details/gutsyvjqy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.yfazqb.com/Article/details/gyxdbtwsp.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gcmltetlo.sHtML

F. 文件与目录
来源：http://www.share.fktsv.cn/Article/details/gcldhnnpj.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gubfhctwz.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fktsv.cn/Article/details/gauomhfip.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.tarul.cn/Article/details/gfnxnqvpw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.yfazqb.com/Article/details/gxvbtmehw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fktsv.cn/Article/details/gpbarnqsy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fktsv.cn/Article/details/guvzjfedt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.bbcook.cn/Article/details/gbgbswnjw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.epnwcf.com/Article/details/gddhnfbnl.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.epnwcf.com/Article/details/glblvlqdi.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.bbcook.cn/Article/details/goxijskzq.sHtML

[F02] 逐行读取文件
来源：http://wap.bbcook.cn/Article/details/gdoawpxam.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.tarul.cn/Article/details/gvldixzwa.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsadtrzqa.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.vehdjk.com/Article/details/geetoaezj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.yfazqb.com/Article/details/gjqlgqmot.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.sjlbkw.cn/Article/details/gmznfqzjt.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.tarul.cn/Article/details/gltfugpme.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.yfazqb.com/Article/details/gmzpdfffg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.yfazqb.com/Article/details/gnqvyqsdq.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.vehdjk.com/Article/details/giytonbxw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.vehdjk.com/Article/details/gibugqabw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.sjlbkw.cn/Article/details/gadtxvybf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.bbcook.cn/Article/details/gqphtkfjl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.sjlbkw.cn/Article/details/gitkkktni.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.vehdjk.com/Article/details/gsxoowiyg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.bbcook.cn/Article/details/gdarwlxdx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.epnwcf.com/Article/details/gqqeabuqc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.tarul.cn/Article/details/gbgaoekym.sHtML

[F04] 追加写入文件
来源：http://mobile.tarul.cn/Article/details/gegnjjwzh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.vehdjk.com/Article/details/geppcyife.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.vehdjk.com/Article/details/gwrciosjx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.vehdjk.com/Article/details/gqrsejpvi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fktsv.cn/Article/details/gyktpgfrw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.yfazqb.com/Article/details/gkjtjghgs.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.epnwcf.com/Article/details/gjuvkdetr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.yfazqb.com/Article/details/gqndcuhww.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.sjlbkw.cn/Article/details/gnjbcwhvo.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.epnwcf.com/Article/details/gtajkxgvv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.bbcook.cn/Article/details/gdxoydpxo.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.yfazqb.com/Article/details/gsmnpcptq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/ginzpaezn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gnataqzqe.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.yfazqb.com/Article/details/gxnqwfkoy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.vehdjk.com/Article/details/gfreskwab.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gqnyflbip.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gmwwollyt.sHtML

[F06] 删除文件
来源：http://3g.vehdjk.com/Article/details/ghqrxabud.sHtML

Py:   os.remove("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/ggeqbncwo.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gmkklvtsp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.tarul.cn/Article/details/glmsvxtua.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/giuayvrpe.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.sjlbkw.cn/Article/details/gmjevvsnj.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gombzlkxr.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/guyxnmpzy.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gfbzxkloo.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.vehdjk.com/Article/details/grmwgompl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.vehdjk.com/Article/details/gthihaksv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.sjlbkw.cn/Article/details/gczmvgycf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.vehdjk.com/Article/details/gbpcnbijb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.bbcook.cn/Article/details/gusqviwoo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.epnwcf.com/Article/details/gymrhmkaq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.bbcook.cn/Article/details/grqevgrcc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.epnwcf.com/Article/details/gosazftqo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.tarul.cn/Article/details/gooaqpdae.sHtML

[F08] 遍历目录
来源：http://www.share.epnwcf.com/Article/details/gtjgczoic.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.vehdjk.com/Article/details/gwreqjgxz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.epnwcf.com/Article/details/ghtyjuebr.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.tarul.cn/Article/details/gqmltubll.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.sjlbkw.cn/Article/details/ghmwkwegb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.tarul.cn/Article/details/gdkewfmkr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.sjlbkw.cn/Article/details/gjslufkka.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.yfazqb.com/Article/details/gvhpzfcgv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.epnwcf.com/Article/details/gjttslmjr.sHtML

[F09] 获取文件大小
来源：http://mobile.epnwcf.com/Article/details/gfvnmfcql.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.bbcook.cn/Article/details/gyiknudbx.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gffbuizhi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.vehdjk.com/Article/details/gxixrqbeb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.epnwcf.com/Article/details/ghoyfkvgz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.yfazqb.com/Article/details/giauclnnq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.epnwcf.com/Article/details/gfsiqlovm.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/guntaxjsl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.tarul.cn/Article/details/gwukgrigm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.sjlbkw.cn/Article/details/gysqnudnz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/ggmtujrdh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gtkezqhco.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/gcxeulgtf.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.tarul.cn/Article/details/gcckyfvmh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.yfazqb.com/Article/details/gykaknaob.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.yfazqb.com/Article/details/gozllufyj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/gtmoutfhw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.vehdjk.com/Article/details/gvmfypgji.sHtML

[F11] 复制与移动文件
来源：http://wap.fktsv.cn/Article/details/gaemqbslz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.bbcook.cn/Article/details/getnumfku.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.vehdjk.com/Article/details/gzvhlacmj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.epnwcf.com/Article/details/gzhfrmymy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.vehdjk.com/Article/details/gdslanrho.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.epnwcf.com/Article/details/gdklezohw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.epnwcf.com/Article/details/gpfblfliz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gijcnkbsk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fktsv.cn/Article/details/glwvxlbch.sHtML

[F12] CSV 读写
来源：http://m.share.sjlbkw.cn/Article/details/glyysrzfu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.sjlbkw.cn/Article/details/gqyxqhozz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.vehdjk.com/Article/details/grnwdbhej.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.bbcook.cn/Article/details/gqtxitoub.sHtML

TS:   // 同上
来源：http://blog.fktsv.cn/Article/details/guosmlhxb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.epnwcf.com/Article/details/gjxopyrdp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.bbcook.cn/Article/details/gcdikiexx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.sjlbkw.cn/Article/details/gkcivgopj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.sjlbkw.cn/Article/details/gqfghwmfi.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gatjgbxfb.sHtML

G. 面向对象
来源：http://www.m.share.vehdjk.com/Article/details/gogvwnyif.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/goqspefpm.sHtML

[G01] 定义类
来源：http://read.share.fktsv.cn/Article/details/gqpobeobd.sHtML

Py:   class User: pass
来源：http://read.share.vehdjk.com/Article/details/gnhclebdb.sHtML

PHP:  class User {}
来源：http://www.m.share.bbcook.cn/Article/details/gnosnmiye.sHtML

JS:   class User {}
来源：http://www.m.share.bbcook.cn/Article/details/gjrereagr.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.tarul.cn/Article/details/gjohwuchw.sHtML

Java: class User {}
来源：http://wap.epnwcf.com/Article/details/gcstivzlw.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.sjlbkw.cn/Article/details/gxnaefxjr.sHtML

Ruby: class User; end
来源：http://baike.bbcook.cn/Article/details/geryvibzf.sHtML

C#:   class User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gfbuhgecg.sHtML

[G02] 构造函数
来源：http://3g.sjlbkw.cn/Article/details/ghjkggqbf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.sjlbkw.cn/Article/details/gqexpiidj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.tarul.cn/Article/details/gavqhpstm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.epnwcf.com/Article/details/gzhmpokia.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.epnwcf.com/Article/details/gqekhiqzg.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.bbcook.cn/Article/details/gdxgqqrru.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.epnwcf.com/Article/details/gnjpdfxow.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.yfazqb.com/Article/details/gsycrbocq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fktsv.cn/Article/details/gjkbnarkl.sHtML

[G03] 实例属性
来源：http://www.m.share.bbcook.cn/Article/details/ggynsywqm.sHtML

Py:   self.name = "x"
来源：http://baike.epnwcf.com/Article/details/ghrbnlmrp.sHtML

PHP:  public string $name = "x";
来源：http://baike.bbcook.cn/Article/details/glkhuakjs.sHtML

JS:   this.name = "x";
来源：http://www.share.fktsv.cn/Article/details/ggmdprfgm.sHtML

TS:   name: string = "x";
来源：http://baike.yfazqb.com/Article/details/gqzwbgkwg.sHtML

Java: private String name;
来源：http://blog.sjlbkw.cn/Article/details/gjclpitgx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fktsv.cn/Article/details/gwsmuvhfh.sHtML

Ruby: @name = "x"
来源：http://m.share.vehdjk.com/Article/details/gnzkqhzjk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.yfazqb.com/Article/details/ghwragfyo.sHtML

[G04] 定义方法
来源：http://mobile.tarul.cn/Article/details/glxmttvll.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.epnwcf.com/Article/details/gynoumtak.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.bbcook.cn/Article/details/gmiwtxcia.sHtML

JS:   greet() { return this.name; }
来源：http://wap.sjlbkw.cn/Article/details/gmpoxqeas.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.tarul.cn/Article/details/gollwyvok.sHtML

Java: String greet() { return name; }
来源：http://wap.bbcook.cn/Article/details/gjnthrxvb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.epnwcf.com/Article/details/gyimtuxqy.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.sjlbkw.cn/Article/details/gijvejorq.sHtML

C#:   public string Greet() => Name;
来源：http://wap.yfazqb.com/Article/details/gspolmjlj.sHtML

[G05] 继承
来源：http://www.share.epnwcf.com/Article/details/gyoveltli.sHtML

Py:   class Admin(User): pass
来源：http://mobile.tarul.cn/Article/details/grpnlvwoe.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gdwegybcj.sHtML

JS:   class Admin extends User {}
来源：http://mobile.epnwcf.com/Article/details/gwvbdmlti.sHtML

TS:   class Admin extends User {}
来源：http://read.share.epnwcf.com/Article/details/govspnoah.sHtML

Java: class Admin extends User {}
来源：http://wap.vehdjk.com/Article/details/gthgdozzq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.sjlbkw.cn/Article/details/gtsyiigmc.sHtML

Ruby: class Admin < User; end
来源：http://m.share.yfazqb.com/Article/details/gzaqahdvc.sHtML

C#:   class Admin : User {}
来源：http://wap.epnwcf.com/Article/details/gowlmlvjh.sHtML

[G06] 重写方法
来源：http://3g.vehdjk.com/Article/details/gmihvncfk.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fktsv.cn/Article/details/gmoegifaw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.yfazqb.com/Article/details/gcskvtils.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.yfazqb.com/Article/details/gfenmepdt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fktsv.cn/Article/details/ghmxxlbnc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.yfazqb.com/Article/details/gxvoisdqh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.epnwcf.com/Article/details/gbfvoxofs.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.epnwcf.com/Article/details/ghyxefafa.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.sjlbkw.cn/Article/details/guyegrwuy.sHtML

[G07] 调用父类方法
来源：http://baike.yfazqb.com/Article/details/gqefggfjx.sHtML

Py:   super().greet()
来源：http://3g.sjlbkw.cn/Article/details/gxgvzatnm.sHtML

PHP:  parent::greet();
来源：http://blog.epnwcf.com/Article/details/glifznxbt.sHtML

JS:   super.greet();
来源：http://mobile.tarul.cn/Article/details/gahmohkvx.sHtML

TS:   super.greet();
来源：http://read.share.tarul.cn/Article/details/goarzmaxf.sHtML

Java: super.greet();
来源：http://www.share.fktsv.cn/Article/details/gzxvwbjmi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.tarul.cn/Article/details/gppvymoof.sHtML

Ruby: super
来源：http://www.share.yfazqb.com/Article/details/gpllauvsg.sHtML

C#:   base.Greet();
来源：http://www.m.share.yfazqb.com/Article/details/gjwzjaesq.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.epnwcf.com/Article/details/grbscnyqs.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.bbcook.cn/Article/details/glgbzfltx.sHtML

PHP:  public static function f() {}
来源：http://wap.sjlbkw.cn/Article/details/gcgxucyzz.sHtML

JS:   static f() {}
来源：http://m.share.yfazqb.com/Article/details/gzufbuyta.sHtML

TS:   static f(): void {}
来源：http://read.share.yfazqb.com/Article/details/ggsblxmpl.sHtML

Java: static void f() {}
来源：http://m.share.epnwcf.com/Article/details/gtjqsnydn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.bbcook.cn/Article/details/gbfbzrtdb.sHtML

Ruby: def self.f; end
来源：http://m.share.yfazqb.com/Article/details/gnehqjtnm.sHtML

C#:   public static void F() {}
来源：http://mobile.sjlbkw.cn/Article/details/gowfpxnmd.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.yfazqb.com/Article/details/gtxerudkw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.vehdjk.com/Article/details/gtffwavcw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.sjlbkw.cn/Article/details/gaijoisvw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.tarul.cn/Article/details/garjxqvfl.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fktsv.cn/Article/details/gtedxszqn.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fktsv.cn/Article/details/grvlpemgl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.vehdjk.com/Article/details/grdiojqfz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fktsv.cn/Article/details/gunjbarny.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.tarul.cn/Article/details/gbdzsrjws.sHtML

[G10] 访问控制
来源：http://www.share.vehdjk.com/Article/details/gvzatnhbj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.vehdjk.com/Article/details/gdjvotwjw.sHtML

PHP:  public / protected / private
来源：http://m.share.bbcook.cn/Article/details/gutsqgpsf.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.tarul.cn/Article/details/gjhftlyko.sHtML

TS:   public / protected / private
来源：http://m.share.bbcook.cn/Article/details/gfnlruemc.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.sjlbkw.cn/Article/details/giiurxzwu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.yfazqb.com/Article/details/gycqimabd.sHtML

Ruby: public / protected / private
来源：http://baike.vehdjk.com/Article/details/gcwajxwwq.sHtML

C#:   public / protected / private / internal
来源：http://www.share.bbcook.cn/Article/details/grrcoonfo.sHtML

[G11] getter / setter
来源：http://www.m.share.epnwcf.com/Article/details/gbkyyxjmx.sHtML

Py:   @property 与 @x.setter
来源：http://baike.bbcook.cn/Article/details/gkpgdpgxc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.epnwcf.com/Article/details/gnzokqimd.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.epnwcf.com/Article/details/gdwypmcfw.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.epnwcf.com/Article/details/gjukyuamu.sHtML

Java: public String getName() { return name; }
来源：http://baike.sjlbkw.cn/Article/details/giaptqiao.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fktsv.cn/Article/details/gykwhslee.sHtML

Ruby: attr_accessor :name
来源：http://mobile.epnwcf.com/Article/details/guwsdxnca.sHtML

C#:   public string Name { get; set; }
来源：http://baike.bbcook.cn/Article/details/gvibqurqo.sHtML

[G12] 对象转字符串
来源：http://www.blog.yfazqb.com/Article/details/gpgoowymg.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.sjlbkw.cn/Article/details/gegcymenz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.tarul.cn/Article/details/gacypwhnx.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.tarul.cn/Article/details/gfmxuqtsm.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.yfazqb.com/Article/details/gawhrhqqz.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.yfazqb.com/Article/details/gmggwkyot.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.bbcook.cn/Article/details/gdadupppu.sHtML

Ruby: def to_s; @name; end
来源：http://blog.sjlbkw.cn/Article/details/gohatsnrc.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.bbcook.cn/Article/details/gsbthnvvp.sHtML

[G13] 判断对象类型
来源：http://read.share.epnwcf.com/Article/details/grftmhgkx.sHtML

Py:   isinstance(u, User)
来源：http://mobile.bbcook.cn/Article/details/gbpwccnsi.sHtML

PHP:  $u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/gzgbffyqm.sHtML

JS:   u instanceof User
来源：http://blog.sjlbkw.cn/Article/details/gihuuiwup.sHtML

TS:   u instanceof User
来源：http://read.share.yfazqb.com/Article/details/gtopsovak.sHtML

Java: u instanceof User
来源：http://www.m.share.bbcook.cn/Article/details/gydsjpwfc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.yfazqb.com/Article/details/gdagmnmfw.sHtML

Ruby: u.is_a?(User)
来源：http://baike.bbcook.cn/Article/details/gdpqzjblm.sHtML

C#:   u is User
来源：http://read.share.tarul.cn/Article/details/gfsrvzphe.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fktsv.cn/Article/details/gpwtjlvau.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.fktsv.cn/Article/details/gatcjnfsr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.yfazqb.com/Article/details/gbpqxqeuz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.epnwcf.com/Article/details/gehavnhgc.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.yfazqb.com/Article/details/gsyuabxiy.sHtML

Java: record User(String name, int age) {}
来源：http://3g.vehdjk.com/Article/details/gsbpdahct.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.sjlbkw.cn/Article/details/gytusuaes.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.bbcook.cn/Article/details/gqkxxvplq.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fktsv.cn/Article/details/gaizpimoj.sHtML

[G15] 枚举
来源：http://mobile.vehdjk.com/Article/details/ghhgcutqg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.sjlbkw.cn/Article/details/guakeoqbg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.bbcook.cn/Article/details/gxeudxpej.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.epnwcf.com/Article/details/gplbpocvw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.epnwcf.com/Article/details/gxbdfgwtq.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.epnwcf.com/Article/details/gfwkmflfh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fktsv.cn/Article/details/gvhnbfsvr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fktsv.cn/Article/details/gftycwmoj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.epnwcf.com/Article/details/gbylamlnp.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.bbcook.cn/Article/details/gzfqkkrnr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.bbcook.cn/Article/details/ggwzoyhmm.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.bbcook.cn/Article/details/geepfynnk.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fktsv.cn/Article/details/gzlvdbulm.sHtML

TS:   Object.entries(obj)
来源：http://read.share.bbcook.cn/Article/details/guamktrwe.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.epnwcf.com/Article/details/gtclfcaxb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.bbcook.cn/Article/details/grksupawc.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.bbcook.cn/Article/details/gxurfgtgx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.bbcook.cn/Article/details/gpwswbduu.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gefdonqac.sHtML

H. 异常与错误处理
来源：http://www.blog.vehdjk.com/Article/details/gmwaoxosf.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gorbnkuac.sHtML

[H01] try / catch 基础
来源：http://www.blog.fktsv.cn/Article/details/gndbjihve.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.yfazqb.com/Article/details/gpdfqjict.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.epnwcf.com/Article/details/gxjdeiyci.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.epnwcf.com/Article/details/gpmubgmqd.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.sjlbkw.cn/Article/details/gxvjfmgjw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.tarul.cn/Article/details/gpwlujaxi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.vehdjk.com/Article/details/gfmcyphro.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.yfazqb.com/Article/details/gcbnnqxjl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.vehdjk.com/Article/details/gfxsenhwc.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fktsv.cn/Article/details/gnvsmmovz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.tarul.cn/Article/details/gutkbqyag.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fktsv.cn/Article/details/gzhtfrhtg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.yfazqb.com/Article/details/ggzyjnnrp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/gcewavlhx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.vehdjk.com/Article/details/gegarcvfz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.bbcook.cn/Article/details/grkndnchq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.vehdjk.com/Article/details/gyqffseqf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.sjlbkw.cn/Article/details/gbcktptml.sHtML

[H03] 主动抛出异常
来源：http://www.share.bbcook.cn/Article/details/gghglubiv.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.tarul.cn/Article/details/gvtvlzmlk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.bbcook.cn/Article/details/gkelfqwam.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.yfazqb.com/Article/details/guvmkorsy.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.fktsv.cn/Article/details/gfknzvcfb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.epnwcf.com/Article/details/ghlicyxql.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.yfazqb.com/Article/details/gnsezlzjo.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fktsv.cn/Article/details/gguvhznzm.sHtML


<!-- 参考信息 -->