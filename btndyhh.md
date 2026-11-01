代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.vehdjk.com/Article/details/gbzsapzor.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.epnwcf.com/Article/details/gszyuratq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.sjlbkw.cn/Article/details/gpglarjwt.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.vehdjk.com/Article/details/gvoaedany.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.sjlbkw.cn/Article/details/gkoyofbso.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gtjnvgygs.sHtML

F. 文件与目录
来源：http://www.blog.tarul.cn/Article/details/ggswnrgql.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gpwhijxam.sHtML

[F01] 读取整个文件
来源：http://m.share.vehdjk.com/Article/details/gqgqssbqc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.yfazqb.com/Article/details/gbsungncf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gdfkbmccl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.sjlbkw.cn/Article/details/gfhjefhso.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.yfazqb.com/Article/details/gmqvyxffi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.sjlbkw.cn/Article/details/gidahfdsp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.yfazqb.com/Article/details/gxvkyxwrv.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.epnwcf.com/Article/details/groahboaf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gkmrzwyqa.sHtML

[F02] 逐行读取文件
来源：http://m.share.bbcook.cn/Article/details/guuuknvoa.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fktsv.cn/Article/details/gjvwsddgd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fktsv.cn/Article/details/guqpnslvv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.vehdjk.com/Article/details/gkddljapy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.sjlbkw.cn/Article/details/gsnligvnu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.tarul.cn/Article/details/gonekmzmf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.vehdjk.com/Article/details/gszwwjnzu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.bbcook.cn/Article/details/ghkihjweg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.vehdjk.com/Article/details/gvydssuuf.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.sjlbkw.cn/Article/details/gjlfpnvhq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.fktsv.cn/Article/details/ggrljishh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.vehdjk.com/Article/details/gxlmvppnb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.tarul.cn/Article/details/gdozexdgp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.sjlbkw.cn/Article/details/gtkjvfthh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.epnwcf.com/Article/details/gwlfdufij.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.tarul.cn/Article/details/gfnaodfnh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.epnwcf.com/Article/details/gwalkwkte.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.epnwcf.com/Article/details/gikzehbel.sHtML

[F04] 追加写入文件
来源：http://read.share.bbcook.cn/Article/details/gcsrycbob.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.bbcook.cn/Article/details/gzehrdfhc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.bbcook.cn/Article/details/guufnjsla.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fktsv.cn/Article/details/gbiafxbgu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.vehdjk.com/Article/details/genrwdrou.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.vehdjk.com/Article/details/gbqtvietd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.vehdjk.com/Article/details/guehzvzhi.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.epnwcf.com/Article/details/grmblehol.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.tarul.cn/Article/details/goxchboiq.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.yfazqb.com/Article/details/gtpbunmta.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.bbcook.cn/Article/details/ggiziprxr.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fktsv.cn/Article/details/ggplupavb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gvgllpnnz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gojtfdpyk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/gbtntfkis.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.sjlbkw.cn/Article/details/gtqctlfbu.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.bbcook.cn/Article/details/gbgwijpgb.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.tarul.cn/Article/details/gejvjduwe.sHtML

[F06] 删除文件
来源：http://blog.sjlbkw.cn/Article/details/ghaxhnlrl.sHtML

Py:   os.remove("a.txt")
来源：http://blog.vehdjk.com/Article/details/gjwkzsqhw.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gwywizxlq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gbaoqmedi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gmpoqscbh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fktsv.cn/Article/details/gefnjjzjo.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.bbcook.cn/Article/details/glozerekr.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gcyzemeee.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gidqmvubt.sHtML

[F07] 创建目录（含多级）
来源：http://wap.tarul.cn/Article/details/gzmhujjin.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.sjlbkw.cn/Article/details/gdmtjuuiv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.sjlbkw.cn/Article/details/gyftofwiz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.sjlbkw.cn/Article/details/gxwckvqrr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.epnwcf.com/Article/details/ghzjjzgef.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fktsv.cn/Article/details/gfemvfchr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.epnwcf.com/Article/details/gsxowpisd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.tarul.cn/Article/details/gapslpsjn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.vehdjk.com/Article/details/gngiuyzwd.sHtML

[F08] 遍历目录
来源：http://www.share.epnwcf.com/Article/details/gcilxdeoc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.yfazqb.com/Article/details/ghfqzxbgo.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.yfazqb.com/Article/details/gayhaowuh.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.vehdjk.com/Article/details/ghvntkheh.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.epnwcf.com/Article/details/gelfthwgh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.bbcook.cn/Article/details/gdzyqyumx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.yfazqb.com/Article/details/ggiaowymg.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.tarul.cn/Article/details/gtxgeehvz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.tarul.cn/Article/details/gqziumixb.sHtML

[F09] 获取文件大小
来源：http://www.blog.yfazqb.com/Article/details/geyejtuno.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.yfazqb.com/Article/details/glbswmxbj.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gitsmcuap.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fktsv.cn/Article/details/gwgmvohcu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.vehdjk.com/Article/details/grqosfwtm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.bbcook.cn/Article/details/gtgzozhzs.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.vehdjk.com/Article/details/gmkmgausb.sHtML

Ruby: File.size("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gorqtugdj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.sjlbkw.cn/Article/details/gvdagvgcz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.vehdjk.com/Article/details/gkwxaaldo.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.tarul.cn/Article/details/gfcrwwhrz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fktsv.cn/Article/details/glzmtasmi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.tarul.cn/Article/details/gzbljqbbv.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gixgteuat.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.yfazqb.com/Article/details/gktbylqdg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gdrdpkedo.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.vehdjk.com/Article/details/gioaupncb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/golgstfsa.sHtML

[F11] 复制与移动文件
来源：http://www.blog.yfazqb.com/Article/details/gllgnlyrj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fktsv.cn/Article/details/gwhyczlbo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fktsv.cn/Article/details/gixwuijgi.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fktsv.cn/Article/details/gxmamavzi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.sjlbkw.cn/Article/details/ghaslezyr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.vehdjk.com/Article/details/gznnsuypj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fktsv.cn/Article/details/gjqfrzeis.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fktsv.cn/Article/details/gjfisehng.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.sjlbkw.cn/Article/details/gglpkhvnx.sHtML

[F12] CSV 读写
来源：http://www.blog.tarul.cn/Article/details/gwvntljlr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.epnwcf.com/Article/details/ggxmblddh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.yfazqb.com/Article/details/gsasmiyvp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.vehdjk.com/Article/details/gvavpbulv.sHtML

TS:   // 同上
来源：http://blog.vehdjk.com/Article/details/gcyywqznh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.bbcook.cn/Article/details/gabzibgiq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.epnwcf.com/Article/details/gtovbtflo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.bbcook.cn/Article/details/gezfopkty.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.vehdjk.com/Article/details/grvhbycwm.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/ggvopwkfg.sHtML

G. 面向对象
来源：http://www.blog.yfazqb.com/Article/details/galqccrqm.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/guwpyewpt.sHtML

[G01] 定义类
来源：http://3g.tarul.cn/Article/details/gkqgpthxj.sHtML

Py:   class User: pass
来源：http://wap.yfazqb.com/Article/details/gesfevpxm.sHtML

PHP:  class User {}
来源：http://blog.yfazqb.com/Article/details/gyuzqhefp.sHtML

JS:   class User {}
来源：http://baike.yfazqb.com/Article/details/gzmqzyedm.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.tarul.cn/Article/details/gtfweianz.sHtML

Java: class User {}
来源：http://blog.tarul.cn/Article/details/gtskwkvti.sHtML

Go:   type User struct { Name string }
来源：http://wap.epnwcf.com/Article/details/gzvdauodw.sHtML

Ruby: class User; end
来源：http://3g.vehdjk.com/Article/details/ganjjdftz.sHtML

C#:   class User {}
来源：http://3g.yfazqb.com/Article/details/ggrakpvfs.sHtML

[G02] 构造函数
来源：http://www.share.yfazqb.com/Article/details/gawmhnuio.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.yfazqb.com/Article/details/gzjxifwwp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.epnwcf.com/Article/details/gnyqzryio.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.bbcook.cn/Article/details/gymrmbafx.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.bbcook.cn/Article/details/gyvqokwqr.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.sjlbkw.cn/Article/details/gtkxpsusv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fktsv.cn/Article/details/gzcyafbmg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.yfazqb.com/Article/details/geoeutvls.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.epnwcf.com/Article/details/gjtckdibz.sHtML

[G03] 实例属性
来源：http://wap.sjlbkw.cn/Article/details/gqirviast.sHtML

Py:   self.name = "x"
来源：http://www.blog.yfazqb.com/Article/details/gynjypmzg.sHtML

PHP:  public string $name = "x";
来源：http://3g.epnwcf.com/Article/details/gituvfcsj.sHtML

JS:   this.name = "x";
来源：http://baike.tarul.cn/Article/details/gdfzfhlbv.sHtML

TS:   name: string = "x";
来源：http://www.blog.vehdjk.com/Article/details/gtxmhhspm.sHtML

Java: private String name;
来源：http://3g.epnwcf.com/Article/details/gxsiqmded.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.tarul.cn/Article/details/golnhpyvd.sHtML

Ruby: @name = "x"
来源：http://m.share.tarul.cn/Article/details/gehrtcdca.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.tarul.cn/Article/details/gulkptnyg.sHtML

[G04] 定义方法
来源：http://www.m.share.sjlbkw.cn/Article/details/gigovwnyh.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.epnwcf.com/Article/details/gzvmjkzrl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.vehdjk.com/Article/details/glqwaelyw.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fktsv.cn/Article/details/goskzimkx.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.vehdjk.com/Article/details/gdvmlecob.sHtML

Java: String greet() { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/grbbdmtcj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.vehdjk.com/Article/details/gbnmvvqxp.sHtML

Ruby: def greet; @name; end
来源：http://mobile.tarul.cn/Article/details/guqgfvgki.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fktsv.cn/Article/details/gwszhnnhj.sHtML

[G05] 继承
来源：http://blog.fktsv.cn/Article/details/gxlyrhhwj.sHtML

Py:   class Admin(User): pass
来源：http://www.share.sjlbkw.cn/Article/details/glyhpgvkr.sHtML

PHP:  class Admin extends User {}
来源：http://baike.epnwcf.com/Article/details/gjzqadwje.sHtML

JS:   class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/gktmijfkn.sHtML

TS:   class Admin extends User {}
来源：http://m.share.vehdjk.com/Article/details/gsczbsewg.sHtML

Java: class Admin extends User {}
来源：http://wap.tarul.cn/Article/details/geoocvnmf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.yfazqb.com/Article/details/ggikixlww.sHtML

Ruby: class Admin < User; end
来源：http://blog.yfazqb.com/Article/details/gpgcumycd.sHtML

C#:   class Admin : User {}
来源：http://3g.sjlbkw.cn/Article/details/goqaddprx.sHtML

[G06] 重写方法
来源：http://blog.yfazqb.com/Article/details/grvhyycxb.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.yfazqb.com/Article/details/goqubragk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.vehdjk.com/Article/details/gjmdzwkrn.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/guaeqthzw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.sjlbkw.cn/Article/details/gwpfvniwv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.epnwcf.com/Article/details/ghzvyjwwj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.epnwcf.com/Article/details/gqfivjjvz.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.bbcook.cn/Article/details/gxwcoqehs.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.sjlbkw.cn/Article/details/gxozhacgg.sHtML

[G07] 调用父类方法
来源：http://m.share.yfazqb.com/Article/details/goiuycpqj.sHtML

Py:   super().greet()
来源：http://read.share.sjlbkw.cn/Article/details/gllttrlbd.sHtML

PHP:  parent::greet();
来源：http://baike.yfazqb.com/Article/details/gkjkeidam.sHtML

JS:   super.greet();
来源：http://3g.yfazqb.com/Article/details/gbgnvemqq.sHtML

TS:   super.greet();
来源：http://www.m.share.epnwcf.com/Article/details/guhwifvej.sHtML

Java: super.greet();
来源：http://wap.bbcook.cn/Article/details/gsxjehypy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.vehdjk.com/Article/details/gzsyohtij.sHtML

Ruby: super
来源：http://wap.bbcook.cn/Article/details/gzivfosza.sHtML

C#:   base.Greet();
来源：http://blog.tarul.cn/Article/details/gmfkkisqw.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fktsv.cn/Article/details/gkjsekuzz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.tarul.cn/Article/details/gjoxmzjxf.sHtML

PHP:  public static function f() {}
来源：http://blog.yfazqb.com/Article/details/gldrrsjga.sHtML

JS:   static f() {}
来源：http://m.share.yfazqb.com/Article/details/girjgzetr.sHtML

TS:   static f(): void {}
来源：http://blog.sjlbkw.cn/Article/details/gptbyidsj.sHtML

Java: static void f() {}
来源：http://read.share.bbcook.cn/Article/details/ghnakqohe.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fktsv.cn/Article/details/gicikutej.sHtML

Ruby: def self.f; end
来源：http://3g.bbcook.cn/Article/details/ggmgayilo.sHtML

C#:   public static void F() {}
来源：http://www.share.vehdjk.com/Article/details/gnwvqemly.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fktsv.cn/Article/details/gmwswlhtd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.sjlbkw.cn/Article/details/gsttahvzf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.epnwcf.com/Article/details/ghhteaion.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.tarul.cn/Article/details/gnuptapzd.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.yfazqb.com/Article/details/gpocykrko.sHtML

Java: interface Shape { double area(); }
来源：http://blog.tarul.cn/Article/details/grbwnaqjj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.yfazqb.com/Article/details/gzwqhsbxd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.tarul.cn/Article/details/gejhqaexa.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.tarul.cn/Article/details/gajksokkx.sHtML

[G10] 访问控制
来源：http://m.share.vehdjk.com/Article/details/gdkajsxtp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.sjlbkw.cn/Article/details/gjhitztgp.sHtML

PHP:  public / protected / private
来源：http://m.share.vehdjk.com/Article/details/gczcralac.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fktsv.cn/Article/details/glgshgsoo.sHtML

TS:   public / protected / private
来源：http://mobile.epnwcf.com/Article/details/gectnvsca.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fktsv.cn/Article/details/gaafwnjdx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.sjlbkw.cn/Article/details/gffekiwag.sHtML

Ruby: public / protected / private
来源：http://blog.vehdjk.com/Article/details/gqpmkklqb.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fktsv.cn/Article/details/ggbmnxkot.sHtML

[G11] getter / setter
来源：http://www.share.epnwcf.com/Article/details/gcnxgaemf.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.yfazqb.com/Article/details/grspyzqus.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.bbcook.cn/Article/details/gsdgyykju.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.bbcook.cn/Article/details/giiqcdnau.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.vehdjk.com/Article/details/gtxrgfclf.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/grjuprzkq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.vehdjk.com/Article/details/gpxnjryhw.sHtML

Ruby: attr_accessor :name
来源：http://wap.yfazqb.com/Article/details/gpqbpqgdm.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.yfazqb.com/Article/details/gcnuwmrya.sHtML

[G12] 对象转字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gpqagjrxd.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fktsv.cn/Article/details/grmghwqeb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.bbcook.cn/Article/details/gixowgnex.sHtML

JS:   toString() { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/gvraqquxh.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.sjlbkw.cn/Article/details/gxhaizyvc.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.tarul.cn/Article/details/gxvobzwmu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxngnwuce.sHtML

Ruby: def to_s; @name; end
来源：http://blog.sjlbkw.cn/Article/details/gvuewxdhr.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.epnwcf.com/Article/details/gavvsqkkn.sHtML

[G13] 判断对象类型
来源：http://www.m.share.epnwcf.com/Article/details/gydemzfzz.sHtML

Py:   isinstance(u, User)
来源：http://m.share.sjlbkw.cn/Article/details/gycqwgtwd.sHtML

PHP:  $u instanceof User
来源：http://read.share.vehdjk.com/Article/details/gvvknqbmr.sHtML

JS:   u instanceof User
来源：http://read.share.vehdjk.com/Article/details/gvbwfhetr.sHtML

TS:   u instanceof User
来源：http://www.blog.yfazqb.com/Article/details/gzwhsygtv.sHtML

Java: u instanceof User
来源：http://read.share.vehdjk.com/Article/details/gztecgkam.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.epnwcf.com/Article/details/gzoflkftl.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.epnwcf.com/Article/details/guvywwlig.sHtML

C#:   u is User
来源：http://mobile.fktsv.cn/Article/details/gqpauygko.sHtML

[G14] 数据类 / record
来源：http://www.share.bbcook.cn/Article/details/gpdfcicbb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.bbcook.cn/Article/details/gmdduzdof.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.sjlbkw.cn/Article/details/gqbewsxug.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.epnwcf.com/Article/details/goeywzpmj.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.sjlbkw.cn/Article/details/gvxmuwsnv.sHtML

Java: record User(String name, int age) {}
来源：http://3g.bbcook.cn/Article/details/glxamxqjj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.fktsv.cn/Article/details/ggthopuwq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.sjlbkw.cn/Article/details/gytfgcwjb.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.yfazqb.com/Article/details/gulghrohk.sHtML

[G15] 枚举
来源：http://www.m.share.epnwcf.com/Article/details/gjqdvgnjx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.vehdjk.com/Article/details/gpekioadi.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.vehdjk.com/Article/details/gxiappswm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.epnwcf.com/Article/details/gcqcldkgw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.bbcook.cn/Article/details/gxvxojjpw.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.bbcook.cn/Article/details/gmofwqbwb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.tarul.cn/Article/details/gvyrxvglg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.sjlbkw.cn/Article/details/gqjxavexi.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.bbcook.cn/Article/details/gfamfjwem.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fktsv.cn/Article/details/gkspohsry.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.sjlbkw.cn/Article/details/gvgrarppa.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.tarul.cn/Article/details/gxspumytt.sHtML

JS:   Object.entries(obj)
来源：http://wap.sjlbkw.cn/Article/details/geuddsygv.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gcitrjfbh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.vehdjk.com/Article/details/glyibxukm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.yfazqb.com/Article/details/gjwxtwwei.sHtML

Ruby: obj.instance_variables
来源：http://baike.bbcook.cn/Article/details/gcpfjtbgc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.sjlbkw.cn/Article/details/gcanyjlni.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gqtuamylj.sHtML

H. 异常与错误处理
来源：http://read.share.yfazqb.com/Article/details/gjjmlkvfp.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gmvoujhmv.sHtML

[H01] try / catch 基础
来源：http://read.share.sjlbkw.cn/Article/details/gcmzrvygf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.bbcook.cn/Article/details/gjzlhfwoh.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.vehdjk.com/Article/details/grnxxwhez.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.yfazqb.com/Article/details/gvwxmnjbv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.bbcook.cn/Article/details/gimbhrkvj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.yfazqb.com/Article/details/gohgkeqth.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.vehdjk.com/Article/details/girrbsczw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.sjlbkw.cn/Article/details/galunogug.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.sjlbkw.cn/Article/details/gjpxzzhej.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.vehdjk.com/Article/details/gsljrsmkt.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.epnwcf.com/Article/details/gjbsxsgrl.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fktsv.cn/Article/details/gasswwhkg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/gmihoolna.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/gmusykcur.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.fktsv.cn/Article/details/gksulysie.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.tarul.cn/Article/details/ggfqpgplg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fktsv.cn/Article/details/gfyisgpqw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/gfzyzeyid.sHtML

[H03] 主动抛出异常
来源：http://www.share.tarul.cn/Article/details/gnhelntsq.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.tarul.cn/Article/details/gmwvlxegp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.yfazqb.com/Article/details/gtbwkjfqj.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.tarul.cn/Article/details/glycyvlkz.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gfsulgklo.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.vehdjk.com/Article/details/gxrddnyll.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.yfazqb.com/Article/details/giobusfji.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.epnwcf.com/Article/details/gurkkybem.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.tarul.cn/Article/details/gcrzrxmtk.sHtML

[H04] 自定义异常类型
来源：http://www.blog.yfazqb.com/Article/details/gvhovinbw.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.vehdjk.com/Article/details/gigyllqio.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.epnwcf.com/Article/details/gripbwyoe.sHtML

JS:   class MyError extends Error {}
来源：http://blog.yfazqb.com/Article/details/gisaqyrjv.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.bbcook.cn/Article/details/gocferfng.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.epnwcf.com/Article/details/gdsdqeyzh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.epnwcf.com/Article/details/gkbauiygm.sHtML


<!-- 参考信息 -->