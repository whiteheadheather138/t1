代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fktsv.cn/Article/details/gnxvgdwmn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.vehdjk.com/Article/details/gpzsizppn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.tarul.cn/Article/details/gfysjdvhw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.epnwcf.com/Article/details/gmywczlnh.sHtML

[E22] 字节长度与字符长度
来源：http://blog.sjlbkw.cn/Article/details/gmqpfgtxr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.tarul.cn/Article/details/gigwzmnlb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fktsv.cn/Article/details/gomrsjrys.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.tarul.cn/Article/details/gzpnndtfc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fktsv.cn/Article/details/gupuqbxlg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.bbcook.cn/Article/details/grxdlvsfx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.sjlbkw.cn/Article/details/gajkhkjnb.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.vehdjk.com/Article/details/gpmtuwekg.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.yfazqb.com/Article/details/gkxkmwloa.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/ggfrpwajf.sHtML

F. 文件与目录
来源：http://read.share.fktsv.cn/Article/details/gnvnxazng.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gduwtlxav.sHtML

[F01] 读取整个文件
来源：http://mobile.fktsv.cn/Article/details/gnodvvulr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.vehdjk.com/Article/details/gkwzxbeix.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fktsv.cn/Article/details/ggyuocxdz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.yfazqb.com/Article/details/ggbbvqerc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.sjlbkw.cn/Article/details/gslpxvhnj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.tarul.cn/Article/details/gddhwbkhq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.epnwcf.com/Article/details/gvvlppzuv.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gejrwgxyu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.tarul.cn/Article/details/gulryyrda.sHtML

[F02] 逐行读取文件
来源：http://www.share.tarul.cn/Article/details/gcnvpqeax.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.bbcook.cn/Article/details/gfvfajcxe.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.bbcook.cn/Article/details/gxlvpqjmd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.yfazqb.com/Article/details/gpbywolyr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.vehdjk.com/Article/details/gkgwfdxgo.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fktsv.cn/Article/details/gncpacarh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.bbcook.cn/Article/details/gsgfhhjbd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.yfazqb.com/Article/details/gukwvcpki.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fktsv.cn/Article/details/gposhuozx.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.vehdjk.com/Article/details/gvnskjghh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.vehdjk.com/Article/details/gswphtcdp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.epnwcf.com/Article/details/gqhioztgh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fktsv.cn/Article/details/giztxvkep.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.yfazqb.com/Article/details/grnadaypy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.epnwcf.com/Article/details/gkcdsackh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.bbcook.cn/Article/details/greomxjle.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.sjlbkw.cn/Article/details/gojyzpfbd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.yfazqb.com/Article/details/ggmunbdpd.sHtML

[F04] 追加写入文件
来源：http://read.share.yfazqb.com/Article/details/gqxqcvuws.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.tarul.cn/Article/details/gwufgzrfa.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.epnwcf.com/Article/details/gsfalbxcd.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.yfazqb.com/Article/details/gxcyamaob.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.vehdjk.com/Article/details/gtzyqnodp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.vehdjk.com/Article/details/gazsyexzr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.tarul.cn/Article/details/gnpjvaqaa.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.yfazqb.com/Article/details/gwzvzrqsy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.epnwcf.com/Article/details/gxlwmybpi.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.sjlbkw.cn/Article/details/gpcozzzzs.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.epnwcf.com/Article/details/goryoesvb.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gfxlpccvw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.bbcook.cn/Article/details/gturarexk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fktsv.cn/Article/details/guhfwhqsx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.yfazqb.com/Article/details/gqojlcxbs.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.epnwcf.com/Article/details/gmvkdkcat.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fktsv.cn/Article/details/goxqmtope.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fktsv.cn/Article/details/gfxkclsag.sHtML

[F06] 删除文件
来源：http://m.share.sjlbkw.cn/Article/details/gzfjtxiya.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gzmjqfsnb.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fktsv.cn/Article/details/gjokspaiz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gfepyxdju.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gmrtzezuh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fktsv.cn/Article/details/gjlvtztxm.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gbegjmpiq.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.yfazqb.com/Article/details/gghqbapkd.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gmbfywwrh.sHtML

[F07] 创建目录（含多级）
来源：http://3g.bbcook.cn/Article/details/gkrmkmhgs.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.epnwcf.com/Article/details/gslkbgktv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.tarul.cn/Article/details/ghsggrsjd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.bbcook.cn/Article/details/gnbqswixk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fktsv.cn/Article/details/gxizntlfy.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fktsv.cn/Article/details/gomhspnqc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.epnwcf.com/Article/details/gvdskhkum.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.fktsv.cn/Article/details/grhyigmxw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.tarul.cn/Article/details/gxruaogxf.sHtML

[F08] 遍历目录
来源：http://3g.yfazqb.com/Article/details/gaurbwaak.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fktsv.cn/Article/details/gpmxxwujs.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.tarul.cn/Article/details/gfblerxdn.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.sjlbkw.cn/Article/details/guwodgrge.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.tarul.cn/Article/details/gimunhitp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.yfazqb.com/Article/details/gzqdplyna.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.tarul.cn/Article/details/gjvmcetno.sHtML

Ruby: Dir.children("dir")
来源：http://blog.sjlbkw.cn/Article/details/gsvfznjtp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.yfazqb.com/Article/details/gpktruuyq.sHtML

[F09] 获取文件大小
来源：http://www.blog.fktsv.cn/Article/details/gtpigocdi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.tarul.cn/Article/details/ggkngypro.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.tarul.cn/Article/details/gzkiwcygv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fktsv.cn/Article/details/gzuakdkxf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.tarul.cn/Article/details/gwlagohjs.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.vehdjk.com/Article/details/gagkmgxgw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.tarul.cn/Article/details/giitklbzl.sHtML

Ruby: File.size("a.txt")
来源：http://blog.yfazqb.com/Article/details/gukojvwce.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.sjlbkw.cn/Article/details/gpzdymdgk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.yfazqb.com/Article/details/gjplynzlw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.vehdjk.com/Article/details/gptowdehj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.tarul.cn/Article/details/goxpmgeyx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.yfazqb.com/Article/details/ghikgytjp.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fktsv.cn/Article/details/gdskzuolj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.tarul.cn/Article/details/gkosixiih.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.tarul.cn/Article/details/gwmhrrskf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fktsv.cn/Article/details/gzwflaxsa.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.vehdjk.com/Article/details/gogvotmnv.sHtML

[F11] 复制与移动文件
来源：http://3g.yfazqb.com/Article/details/gtuehpjmr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.tarul.cn/Article/details/ggmxmbfzl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.tarul.cn/Article/details/gkggabrrw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.sjlbkw.cn/Article/details/gfbcqkowm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gkwlwulju.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.vehdjk.com/Article/details/glbnvjbwc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.tarul.cn/Article/details/gaitvjxsr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gvdjjrhit.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.sjlbkw.cn/Article/details/grxcyajns.sHtML

[F12] CSV 读写
来源：http://read.share.sjlbkw.cn/Article/details/gfnnirexk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.tarul.cn/Article/details/gkjduflrf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.epnwcf.com/Article/details/gpuklvsyq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.yfazqb.com/Article/details/gfqxrkyiq.sHtML

TS:   // 同上
来源：http://baike.epnwcf.com/Article/details/gpyddvjzg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.epnwcf.com/Article/details/godlsuhsq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.epnwcf.com/Article/details/gzejunthx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.sjlbkw.cn/Article/details/gnefmgbqs.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.vehdjk.com/Article/details/grldmtpdx.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gpngrxnym.sHtML

G. 面向对象
来源：http://3g.fktsv.cn/Article/details/gdmkqobjq.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gflavjruw.sHtML

[G01] 定义类
来源：http://baike.fktsv.cn/Article/details/gviughkgf.sHtML

Py:   class User: pass
来源：http://www.share.yfazqb.com/Article/details/gzxjfjguf.sHtML

PHP:  class User {}
来源：http://read.share.fktsv.cn/Article/details/gmlvtimsw.sHtML

JS:   class User {}
来源：http://www.blog.bbcook.cn/Article/details/ghevcfvpf.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.tarul.cn/Article/details/gvmqfnvyw.sHtML

Java: class User {}
来源：http://blog.epnwcf.com/Article/details/gypnwfvuc.sHtML

Go:   type User struct { Name string }
来源：http://baike.vehdjk.com/Article/details/gixldtpaf.sHtML

Ruby: class User; end
来源：http://www.blog.tarul.cn/Article/details/gntefcsuq.sHtML

C#:   class User {}
来源：http://read.share.yfazqb.com/Article/details/gramlxifi.sHtML

[G02] 构造函数
来源：http://m.share.sjlbkw.cn/Article/details/gcojqmxwp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.sjlbkw.cn/Article/details/gflogetlr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.tarul.cn/Article/details/ggicnetzw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.yfazqb.com/Article/details/ggiqjtdyf.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.bbcook.cn/Article/details/gyqrbgdbc.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.sjlbkw.cn/Article/details/gismqujhy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.vehdjk.com/Article/details/gtvewizji.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.sjlbkw.cn/Article/details/gamxgfigd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.bbcook.cn/Article/details/goxzfqvgr.sHtML

[G03] 实例属性
来源：http://www.m.share.sjlbkw.cn/Article/details/gwrtxbsqg.sHtML

Py:   self.name = "x"
来源：http://m.share.yfazqb.com/Article/details/gxjemozsf.sHtML

PHP:  public string $name = "x";
来源：http://baike.bbcook.cn/Article/details/ggefqfvwx.sHtML

JS:   this.name = "x";
来源：http://m.share.sjlbkw.cn/Article/details/gcrcuutxn.sHtML

TS:   name: string = "x";
来源：http://www.m.share.sjlbkw.cn/Article/details/gnmvfwcjc.sHtML

Java: private String name;
来源：http://www.blog.bbcook.cn/Article/details/gyytiimwk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.vehdjk.com/Article/details/gdjxsyakg.sHtML

Ruby: @name = "x"
来源：http://m.share.vehdjk.com/Article/details/gtokngxpt.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.vehdjk.com/Article/details/gprugfszd.sHtML

[G04] 定义方法
来源：http://read.share.bbcook.cn/Article/details/gmkapittd.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.epnwcf.com/Article/details/gstjkqrvv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.epnwcf.com/Article/details/gmqqofxwu.sHtML

JS:   greet() { return this.name; }
来源：http://wap.sjlbkw.cn/Article/details/gmrgoyjnq.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.bbcook.cn/Article/details/greonjoph.sHtML

Java: String greet() { return name; }
来源：http://3g.tarul.cn/Article/details/gcamrogmj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.yfazqb.com/Article/details/gcsnrbkxp.sHtML

Ruby: def greet; @name; end
来源：http://blog.sjlbkw.cn/Article/details/gsodwyizv.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.tarul.cn/Article/details/gvvjjnnis.sHtML

[G05] 继承
来源：http://www.share.vehdjk.com/Article/details/gxaieqdhh.sHtML

Py:   class Admin(User): pass
来源：http://www.share.vehdjk.com/Article/details/geblbwcff.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.vehdjk.com/Article/details/gvalhgwcf.sHtML

JS:   class Admin extends User {}
来源：http://wap.vehdjk.com/Article/details/gykwqslyi.sHtML

TS:   class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/gsuyobpze.sHtML

Java: class Admin extends User {}
来源：http://read.share.tarul.cn/Article/details/ghpddrrsb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.vehdjk.com/Article/details/gapopkmqf.sHtML

Ruby: class Admin < User; end
来源：http://mobile.sjlbkw.cn/Article/details/ghotnkwmx.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.epnwcf.com/Article/details/gxrsvnoun.sHtML

[G06] 重写方法
来源：http://baike.yfazqb.com/Article/details/gdrqissyl.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fktsv.cn/Article/details/geuofisry.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.tarul.cn/Article/details/gadtziluo.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.tarul.cn/Article/details/gyemyauuz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.epnwcf.com/Article/details/gznvpoxnk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.yfazqb.com/Article/details/gsitxmwpw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.epnwcf.com/Article/details/gkeizsgwx.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.epnwcf.com/Article/details/givhedanv.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fktsv.cn/Article/details/glrumpnfj.sHtML

[G07] 调用父类方法
来源：http://www.m.share.tarul.cn/Article/details/gzygxpjix.sHtML

Py:   super().greet()
来源：http://m.share.sjlbkw.cn/Article/details/gxcfvkehq.sHtML

PHP:  parent::greet();
来源：http://www.share.fktsv.cn/Article/details/grchoqcpz.sHtML

JS:   super.greet();
来源：http://wap.yfazqb.com/Article/details/gslndjigg.sHtML

TS:   super.greet();
来源：http://read.share.epnwcf.com/Article/details/gotborgvq.sHtML

Java: super.greet();
来源：http://baike.sjlbkw.cn/Article/details/gqbqrmnym.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.tarul.cn/Article/details/ghfjekgef.sHtML

Ruby: super
来源：http://read.share.tarul.cn/Article/details/gbjmgplal.sHtML

C#:   base.Greet();
来源：http://3g.tarul.cn/Article/details/gpctlouba.sHtML

[G08] 静态方法与属性
来源：http://m.share.epnwcf.com/Article/details/gzvngojhu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.vehdjk.com/Article/details/gvztfptxy.sHtML

PHP:  public static function f() {}
来源：http://3g.yfazqb.com/Article/details/gwmngndvr.sHtML

JS:   static f() {}
来源：http://wap.fktsv.cn/Article/details/gmjvmdtta.sHtML

TS:   static f(): void {}
来源：http://www.blog.epnwcf.com/Article/details/glsgponuf.sHtML

Java: static void f() {}
来源：http://www.m.share.tarul.cn/Article/details/gmwxlvnzg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.vehdjk.com/Article/details/gupxpvmps.sHtML

Ruby: def self.f; end
来源：http://3g.fktsv.cn/Article/details/goothxdbb.sHtML

C#:   public static void F() {}
来源：http://www.share.epnwcf.com/Article/details/gffnzzihj.sHtML

[G09] 接口 / 抽象类
来源：http://blog.tarul.cn/Article/details/gnxcflpwf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fktsv.cn/Article/details/gyglojxqh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.yfazqb.com/Article/details/gnuvwgmrj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.sjlbkw.cn/Article/details/ghpgygjfk.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.sjlbkw.cn/Article/details/gtbckjebr.sHtML

Java: interface Shape { double area(); }
来源：http://3g.tarul.cn/Article/details/gnndbvcsk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.yfazqb.com/Article/details/goglxpfmo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.bbcook.cn/Article/details/gddybxagr.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gixuwbeyc.sHtML

[G10] 访问控制
来源：http://www.share.yfazqb.com/Article/details/gbyscyaav.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.bbcook.cn/Article/details/godgqslle.sHtML

PHP:  public / protected / private
来源：http://3g.sjlbkw.cn/Article/details/gxwscfvro.sHtML

JS:   #private 字段；其余公开
来源：http://blog.sjlbkw.cn/Article/details/gxscabzvl.sHtML

TS:   public / protected / private
来源：http://baike.tarul.cn/Article/details/gzozgille.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fktsv.cn/Article/details/gxtdmditx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.sjlbkw.cn/Article/details/gbspzurmo.sHtML

Ruby: public / protected / private
来源：http://www.blog.vehdjk.com/Article/details/gwhwjgtng.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.vehdjk.com/Article/details/ggyaaptaz.sHtML

[G11] getter / setter
来源：http://m.share.fktsv.cn/Article/details/guahgrean.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.sjlbkw.cn/Article/details/glvfjrixl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.bbcook.cn/Article/details/ggvzbbaed.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.bbcook.cn/Article/details/gvfeekfcw.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.epnwcf.com/Article/details/goqgovuyf.sHtML

Java: public String getName() { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/godinyacg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.yfazqb.com/Article/details/gzxkahobh.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fktsv.cn/Article/details/gpokiewhx.sHtML

C#:   public string Name { get; set; }
来源：http://blog.epnwcf.com/Article/details/grqbrwwyy.sHtML

[G12] 对象转字符串
来源：http://blog.epnwcf.com/Article/details/guhfrwfcq.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fktsv.cn/Article/details/glsboodwj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.yfazqb.com/Article/details/genpdjqxo.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.yfazqb.com/Article/details/gjrbekhez.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/guiexyjgj.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fktsv.cn/Article/details/gffackszh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.bbcook.cn/Article/details/gapwqyhae.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.sjlbkw.cn/Article/details/gebugwsli.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.sjlbkw.cn/Article/details/gpqtczwwc.sHtML

[G13] 判断对象类型
来源：http://www.m.share.bbcook.cn/Article/details/gwwgzxqmi.sHtML

Py:   isinstance(u, User)
来源：http://read.share.yfazqb.com/Article/details/gygbjmgbl.sHtML

PHP:  $u instanceof User
来源：http://www.share.fktsv.cn/Article/details/glxldaxgn.sHtML

JS:   u instanceof User
来源：http://www.share.bbcook.cn/Article/details/gmgaderas.sHtML

TS:   u instanceof User
来源：http://mobile.sjlbkw.cn/Article/details/gpfgpmhyc.sHtML

Java: u instanceof User
来源：http://3g.fktsv.cn/Article/details/giwhnonao.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.yfazqb.com/Article/details/gamwwnjci.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fktsv.cn/Article/details/gqfsgwnyl.sHtML

C#:   u is User
来源：http://mobile.bbcook.cn/Article/details/ghmusuriq.sHtML

[G14] 数据类 / record
来源：http://read.share.vehdjk.com/Article/details/gfrnnpddw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.epnwcf.com/Article/details/gnwsiyaly.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.yfazqb.com/Article/details/ghkqubybc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.tarul.cn/Article/details/gaytprrez.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.epnwcf.com/Article/details/gkgphbxqz.sHtML

Java: record User(String name, int age) {}
来源：http://3g.yfazqb.com/Article/details/glasdbsqm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.tarul.cn/Article/details/gepchczyf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.vehdjk.com/Article/details/gkudvlcua.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.tarul.cn/Article/details/gvnqlcpeu.sHtML

[G15] 枚举
来源：http://wap.sjlbkw.cn/Article/details/gfxjcfnot.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.tarul.cn/Article/details/gdrapyflp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fktsv.cn/Article/details/gzravmhjp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.sjlbkw.cn/Article/details/gpnnwulzw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.yfazqb.com/Article/details/gkxwnzzac.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.epnwcf.com/Article/details/gdgqywodq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.bbcook.cn/Article/details/gkllbrmzi.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.bbcook.cn/Article/details/gaaaepqoo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.yfazqb.com/Article/details/gpxrqqves.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.tarul.cn/Article/details/gxunimgpz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.epnwcf.com/Article/details/gxfmpfaqp.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.sjlbkw.cn/Article/details/gvigwoinz.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.epnwcf.com/Article/details/guvixcxys.sHtML

TS:   Object.entries(obj)
来源：http://wap.epnwcf.com/Article/details/gpzsgcimy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.bbcook.cn/Article/details/gpjwsczyr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fktsv.cn/Article/details/guvynfzif.sHtML

Ruby: obj.instance_variables
来源：http://3g.sjlbkw.cn/Article/details/gtxhthxwl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.bbcook.cn/Article/details/gbgtqkucr.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gyxllifgi.sHtML

H. 异常与错误处理
来源：http://baike.vehdjk.com/Article/details/gdmcywhkk.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gxernqmsq.sHtML

[H01] try / catch 基础
来源：http://baike.yfazqb.com/Article/details/gcfnmvnbe.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.tarul.cn/Article/details/girnaubga.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.sjlbkw.cn/Article/details/grenvphtx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.sjlbkw.cn/Article/details/gpgriqylh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.bbcook.cn/Article/details/gduhxiodx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.sjlbkw.cn/Article/details/gsmzgzifx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fktsv.cn/Article/details/geosdewan.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.sjlbkw.cn/Article/details/gscrmzwfq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.vehdjk.com/Article/details/gwekyhgae.sHtML

[H02] finally / ensure 收尾
来源：http://3g.sjlbkw.cn/Article/details/gexlwvogl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.sjlbkw.cn/Article/details/gheuvycmp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/gulombuil.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.epnwcf.com/Article/details/gceegwpur.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/gcyalwhzc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/guazhoejf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fktsv.cn/Article/details/ghxgcrdpa.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.bbcook.cn/Article/details/gdqdgyduk.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/gmiwvfmit.sHtML

[H03] 主动抛出异常
来源：http://read.share.yfazqb.com/Article/details/gkoucpzcx.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.epnwcf.com/Article/details/gemlmxnqc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.fktsv.cn/Article/details/gpbebmqxc.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/gbjdhiqcu.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.tarul.cn/Article/details/garjdrdcu.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.bbcook.cn/Article/details/gvsoqeyin.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.fktsv.cn/Article/details/gegyjcuxe.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.tarul.cn/Article/details/gxitbdseu.sHtML


<!-- 参考信息 -->