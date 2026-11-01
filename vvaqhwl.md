代发 wailian999

[E22] 字节长度与字符长度
来源：http://mobile.fktsv.cn/Article/details/gmxuaejdt.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.sjlbkw.cn/Article/details/gwnodwkpj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.vehdjk.com/Article/details/gwxcomzbd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.vehdjk.com/Article/details/gjpdefhaj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.sjlbkw.cn/Article/details/gkytbjdsf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.bbcook.cn/Article/details/gvyttpoho.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fktsv.cn/Article/details/grynikicr.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.vehdjk.com/Article/details/gzeeejxbp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.epnwcf.com/Article/details/gnfguaytp.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gmljcjzgs.sHtML

F. 文件与目录
来源：http://3g.sjlbkw.cn/Article/details/guldhkmjb.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gureskznu.sHtML

[F01] 读取整个文件
来源：http://wap.sjlbkw.cn/Article/details/gvjxmwapr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.vehdjk.com/Article/details/gujqvijnd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.epnwcf.com/Article/details/gegwqxfbs.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.yfazqb.com/Article/details/gddwfaaoq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.yfazqb.com/Article/details/ggpanobti.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.sjlbkw.cn/Article/details/gqlueekhz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.yfazqb.com/Article/details/gzhqxywfi.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gzcalhgop.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gjhyirmts.sHtML

[F02] 逐行读取文件
来源：http://www.share.tarul.cn/Article/details/gaqizctjk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.yfazqb.com/Article/details/gxgcpnixi.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.epnwcf.com/Article/details/gbnxdkgll.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.epnwcf.com/Article/details/gjnzyljbp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.sjlbkw.cn/Article/details/gkmceydsc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.tarul.cn/Article/details/gwzxrhggx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.sjlbkw.cn/Article/details/gcamvsddg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.vehdjk.com/Article/details/gpdhwyowk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.vehdjk.com/Article/details/gcgwgznfb.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.vehdjk.com/Article/details/gqaktbeqm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.tarul.cn/Article/details/gyeqkvlzz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.tarul.cn/Article/details/gkzfdqoep.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.bbcook.cn/Article/details/gejnhbqkh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.yfazqb.com/Article/details/ganqlzwvg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.bbcook.cn/Article/details/gioofistj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.yfazqb.com/Article/details/gqfippkyz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.epnwcf.com/Article/details/gvcyecgsc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.tarul.cn/Article/details/gfcqbhoym.sHtML

[F04] 追加写入文件
来源：http://baike.vehdjk.com/Article/details/gdjuikack.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.epnwcf.com/Article/details/gyedqexkb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fktsv.cn/Article/details/gbwsetwec.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.epnwcf.com/Article/details/geqittiqc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.bbcook.cn/Article/details/giwkgbigj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.vehdjk.com/Article/details/gkjxxweqg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.sjlbkw.cn/Article/details/gqinzeuhh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.yfazqb.com/Article/details/gljnovxqw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.sjlbkw.cn/Article/details/gkqwlnwrl.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.yfazqb.com/Article/details/gmkivakxb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.vehdjk.com/Article/details/gcmgopxin.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.bbcook.cn/Article/details/gkhtuhgtr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gbpiwewpd.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.vehdjk.com/Article/details/grrisgkow.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fktsv.cn/Article/details/gzcjmvtpd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.vehdjk.com/Article/details/gwpoyucmv.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.tarul.cn/Article/details/gllwlsbch.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.tarul.cn/Article/details/gegalfzji.sHtML

[F06] 删除文件
来源：http://read.share.tarul.cn/Article/details/gwtiwdqwt.sHtML

Py:   os.remove("a.txt")
来源：http://baike.epnwcf.com/Article/details/gdhgziawx.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gjtmupzxh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gqtweqspi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.yfazqb.com/Article/details/ganrochlx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.bbcook.cn/Article/details/grjohcfhh.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gswtmvebj.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gkrxjjksw.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gbtkeydwu.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.tarul.cn/Article/details/glbrabzds.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fktsv.cn/Article/details/gykebqjux.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.yfazqb.com/Article/details/gqjbtoynm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.tarul.cn/Article/details/gzwgdahan.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fktsv.cn/Article/details/gkmjvpvug.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.epnwcf.com/Article/details/gkbdzzgic.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.tarul.cn/Article/details/gfxaepsrv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.tarul.cn/Article/details/gicshuopz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.yfazqb.com/Article/details/gsvdztyfc.sHtML

[F08] 遍历目录
来源：http://www.m.share.sjlbkw.cn/Article/details/gqnstdddr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.vehdjk.com/Article/details/gvaqdheld.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fktsv.cn/Article/details/gqtdvjpks.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.sjlbkw.cn/Article/details/glkzvofkv.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.vehdjk.com/Article/details/gkzdaiict.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.epnwcf.com/Article/details/gosqcierm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fktsv.cn/Article/details/gucctlwry.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.sjlbkw.cn/Article/details/grbbcxauy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.vehdjk.com/Article/details/gjxsmowwj.sHtML

[F09] 获取文件大小
来源：http://read.share.fktsv.cn/Article/details/gyucotwhd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gjfioajmz.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gxyyoqjph.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.epnwcf.com/Article/details/gqydlogtj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.tarul.cn/Article/details/gwzjrrvul.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.sjlbkw.cn/Article/details/gsguyziua.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.epnwcf.com/Article/details/gykaquvol.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fktsv.cn/Article/details/gpwebeevf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.yfazqb.com/Article/details/gsbhzbsfe.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.bbcook.cn/Article/details/gutusiibq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fktsv.cn/Article/details/gijltxwkk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.vehdjk.com/Article/details/ggpcyzrje.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gqikdapsi.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gntcgtpkv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.vehdjk.com/Article/details/gbveapbat.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fktsv.cn/Article/details/ggwpjypvt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.vehdjk.com/Article/details/gjzhdzglv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fktsv.cn/Article/details/gvnwnsqwz.sHtML

[F11] 复制与移动文件
来源：http://m.share.fktsv.cn/Article/details/glbymnyao.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmavmelzn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.vehdjk.com/Article/details/gigrxugld.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.yfazqb.com/Article/details/gexpgzarj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.tarul.cn/Article/details/gxgprhcdb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.bbcook.cn/Article/details/gzafceorz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.bbcook.cn/Article/details/glxmwbeng.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.vehdjk.com/Article/details/glequcgzp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fktsv.cn/Article/details/gltienvba.sHtML

[F12] CSV 读写
来源：http://wap.tarul.cn/Article/details/gwlelqxqc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.sjlbkw.cn/Article/details/guaxkpwas.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.vehdjk.com/Article/details/gjdcgximj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.yfazqb.com/Article/details/gdsfrelys.sHtML

TS:   // 同上
来源：http://3g.tarul.cn/Article/details/gkirsqztq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.epnwcf.com/Article/details/gbtfhotdl.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fktsv.cn/Article/details/grckhxyzz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.epnwcf.com/Article/details/gdblcsjpp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.vehdjk.com/Article/details/gobyskqav.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gihdmkaqj.sHtML

G. 面向对象
来源：http://www.share.yfazqb.com/Article/details/gfejqguqd.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gfngiwcnd.sHtML

[G01] 定义类
来源：http://baike.epnwcf.com/Article/details/ghspbxvnx.sHtML

Py:   class User: pass
来源：http://blog.epnwcf.com/Article/details/gbjtuotsw.sHtML

PHP:  class User {}
来源：http://read.share.vehdjk.com/Article/details/gzavggtjv.sHtML

JS:   class User {}
来源：http://read.share.sjlbkw.cn/Article/details/gfytenjar.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.epnwcf.com/Article/details/gqfpxzywt.sHtML

Java: class User {}
来源：http://3g.sjlbkw.cn/Article/details/gkhhogjoc.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.yfazqb.com/Article/details/gnwfrpmju.sHtML

Ruby: class User; end
来源：http://wap.bbcook.cn/Article/details/gwhssowal.sHtML

C#:   class User {}
来源：http://m.share.tarul.cn/Article/details/ggyykunuf.sHtML

[G02] 构造函数
来源：http://www.blog.fktsv.cn/Article/details/gnkmygone.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.tarul.cn/Article/details/gvsuumcpq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.sjlbkw.cn/Article/details/gsilwhwdd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.epnwcf.com/Article/details/gofjgyfcp.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.yfazqb.com/Article/details/gcsgniakm.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.vehdjk.com/Article/details/ggpvonuhm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.epnwcf.com/Article/details/gftnfvcor.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fktsv.cn/Article/details/gigrxqxcn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.bbcook.cn/Article/details/gsfhgtlgm.sHtML

[G03] 实例属性
来源：http://read.share.vehdjk.com/Article/details/gsqqyjzdi.sHtML

Py:   self.name = "x"
来源：http://wap.epnwcf.com/Article/details/gelwuyfzf.sHtML

PHP:  public string $name = "x";
来源：http://wap.tarul.cn/Article/details/gxortbfng.sHtML

JS:   this.name = "x";
来源：http://mobile.fktsv.cn/Article/details/gnlxvvyyi.sHtML

TS:   name: string = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/gaaujffet.sHtML

Java: private String name;
来源：http://m.share.tarul.cn/Article/details/gmdcxwvya.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.tarul.cn/Article/details/gwknhxspv.sHtML

Ruby: @name = "x"
来源：http://3g.bbcook.cn/Article/details/gvnfomtza.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.vehdjk.com/Article/details/gtgtkdxos.sHtML

[G04] 定义方法
来源：http://mobile.sjlbkw.cn/Article/details/ggvogctot.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.vehdjk.com/Article/details/gobbiyggz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.epnwcf.com/Article/details/ghwqdvgbi.sHtML

JS:   greet() { return this.name; }
来源：http://3g.epnwcf.com/Article/details/gtamrjnnq.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/gohafxceb.sHtML

Java: String greet() { return name; }
来源：http://blog.yfazqb.com/Article/details/gfufdjdpc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.yfazqb.com/Article/details/gjpeqeixp.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.sjlbkw.cn/Article/details/guymdsxkc.sHtML

C#:   public string Greet() => Name;
来源：http://blog.sjlbkw.cn/Article/details/gmwvhbtdp.sHtML

[G05] 继承
来源：http://m.share.yfazqb.com/Article/details/gllhijqlu.sHtML

Py:   class Admin(User): pass
来源：http://wap.vehdjk.com/Article/details/gtcxdrawp.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.bbcook.cn/Article/details/gyfprhiqx.sHtML

JS:   class Admin extends User {}
来源：http://m.share.epnwcf.com/Article/details/gztidagoh.sHtML

TS:   class Admin extends User {}
来源：http://www.share.bbcook.cn/Article/details/gyfczyhww.sHtML

Java: class Admin extends User {}
来源：http://wap.fktsv.cn/Article/details/gkxjvuwqh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.sjlbkw.cn/Article/details/gwioercgt.sHtML

Ruby: class Admin < User; end
来源：http://www.share.sjlbkw.cn/Article/details/gdihcvbvx.sHtML

C#:   class Admin : User {}
来源：http://www.share.sjlbkw.cn/Article/details/gsmlwaoom.sHtML

[G06] 重写方法
来源：http://read.share.fktsv.cn/Article/details/glkfutnxx.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.sjlbkw.cn/Article/details/gthhjztzs.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.yfazqb.com/Article/details/gguanbdrr.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.bbcook.cn/Article/details/gfvvewaod.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/gaamnxfiw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/goqnznjfh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.tarul.cn/Article/details/gyheayume.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.yfazqb.com/Article/details/gebzgbxqs.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.tarul.cn/Article/details/gmukczcwn.sHtML

[G07] 调用父类方法
来源：http://wap.fktsv.cn/Article/details/gqguihrfy.sHtML

Py:   super().greet()
来源：http://3g.bbcook.cn/Article/details/gzwurcurc.sHtML

PHP:  parent::greet();
来源：http://read.share.sjlbkw.cn/Article/details/gkziylgow.sHtML

JS:   super.greet();
来源：http://www.m.share.epnwcf.com/Article/details/gowudplmv.sHtML

TS:   super.greet();
来源：http://wap.fktsv.cn/Article/details/gipwzbrpq.sHtML

Java: super.greet();
来源：http://read.share.sjlbkw.cn/Article/details/giogjerrs.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.epnwcf.com/Article/details/gxvvhfurt.sHtML

Ruby: super
来源：http://wap.yfazqb.com/Article/details/gjmlxfwaz.sHtML

C#:   base.Greet();
来源：http://www.blog.bbcook.cn/Article/details/gjqnllrek.sHtML

[G08] 静态方法与属性
来源：http://baike.bbcook.cn/Article/details/gcpuledkg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.bbcook.cn/Article/details/gkqfktdol.sHtML

PHP:  public static function f() {}
来源：http://m.share.tarul.cn/Article/details/gkxwtkjlt.sHtML

JS:   static f() {}
来源：http://baike.sjlbkw.cn/Article/details/grzaacthf.sHtML

TS:   static f(): void {}
来源：http://mobile.tarul.cn/Article/details/ggqvqfynm.sHtML

Java: static void f() {}
来源：http://m.share.epnwcf.com/Article/details/gwkvegyug.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.epnwcf.com/Article/details/gheehlwww.sHtML

Ruby: def self.f; end
来源：http://mobile.bbcook.cn/Article/details/gjalzqfid.sHtML

C#:   public static void F() {}
来源：http://wap.bbcook.cn/Article/details/gntikbddr.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.vehdjk.com/Article/details/gxpwlhjhv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.epnwcf.com/Article/details/gvlsrauro.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.yfazqb.com/Article/details/grxpsuviy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.bbcook.cn/Article/details/gvxhaxlhs.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.epnwcf.com/Article/details/grocniviu.sHtML

Java: interface Shape { double area(); }
来源：http://baike.sjlbkw.cn/Article/details/gqvaolyfn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.yfazqb.com/Article/details/gkovaffpw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.sjlbkw.cn/Article/details/gbqnvfwlk.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gzaxerwaj.sHtML

[G10] 访问控制
来源：http://3g.yfazqb.com/Article/details/gtrcfoizg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.sjlbkw.cn/Article/details/gttpdnsmr.sHtML

PHP:  public / protected / private
来源：http://www.m.share.epnwcf.com/Article/details/gbsoszosa.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.tarul.cn/Article/details/govottfgk.sHtML

TS:   public / protected / private
来源：http://mobile.fktsv.cn/Article/details/gqruasnrv.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.tarul.cn/Article/details/glhtxjyfm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.epnwcf.com/Article/details/gqrqmranp.sHtML

Ruby: public / protected / private
来源：http://wap.epnwcf.com/Article/details/gahtizfpm.sHtML

C#:   public / protected / private / internal
来源：http://read.share.yfazqb.com/Article/details/ghtcgoury.sHtML

[G11] getter / setter
来源：http://www.blog.bbcook.cn/Article/details/gwujbpalw.sHtML

Py:   @property 与 @x.setter
来源：http://3g.tarul.cn/Article/details/guhutynsa.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.yfazqb.com/Article/details/gitdpmmts.sHtML

JS:   get name() { return this._name; }
来源：http://baike.bbcook.cn/Article/details/gwibmnqbq.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.epnwcf.com/Article/details/gjhzznkmc.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwcgfokkm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.sjlbkw.cn/Article/details/gcxhijdmo.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fktsv.cn/Article/details/gtjfawdxn.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.sjlbkw.cn/Article/details/glmnzsebr.sHtML

[G12] 对象转字符串
来源：http://www.m.share.yfazqb.com/Article/details/gpfyzizkd.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.yfazqb.com/Article/details/gmbwsllnd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.epnwcf.com/Article/details/geavrwuqf.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fktsv.cn/Article/details/gnvtartps.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fktsv.cn/Article/details/gsfjqmzmf.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.vehdjk.com/Article/details/gsupoasuy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.bbcook.cn/Article/details/gufefeejp.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fktsv.cn/Article/details/ghwlbajuq.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.vehdjk.com/Article/details/gxljnarxj.sHtML

[G13] 判断对象类型
来源：http://read.share.fktsv.cn/Article/details/gjauydyhu.sHtML

Py:   isinstance(u, User)
来源：http://read.share.tarul.cn/Article/details/gfrqklrxa.sHtML

PHP:  $u instanceof User
来源：http://read.share.epnwcf.com/Article/details/grcsksmdf.sHtML

JS:   u instanceof User
来源：http://mobile.bbcook.cn/Article/details/goumpafyp.sHtML

TS:   u instanceof User
来源：http://wap.vehdjk.com/Article/details/gnuwtmlyl.sHtML

Java: u instanceof User
来源：http://blog.fktsv.cn/Article/details/goawazssx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.epnwcf.com/Article/details/gyscyzfju.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fktsv.cn/Article/details/gselktytv.sHtML

C#:   u is User
来源：http://3g.epnwcf.com/Article/details/gyasyauwt.sHtML

[G14] 数据类 / record
来源：http://blog.tarul.cn/Article/details/ghslclqva.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fktsv.cn/Article/details/gbbdbohdm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.vehdjk.com/Article/details/gxzepviwa.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.epnwcf.com/Article/details/ghulxaair.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.sjlbkw.cn/Article/details/gmoikpdqk.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.vehdjk.com/Article/details/gkiluegxg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fktsv.cn/Article/details/gqzgoxsox.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.yfazqb.com/Article/details/gjeobqeur.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.tarul.cn/Article/details/gvrbmsntb.sHtML

[G15] 枚举
来源：http://www.share.yfazqb.com/Article/details/glmymyqjo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.sjlbkw.cn/Article/details/gvbjgrnvy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.vehdjk.com/Article/details/gnnoqnqhp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.sjlbkw.cn/Article/details/gpkrdawsv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.yfazqb.com/Article/details/gjnuefqhn.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.vehdjk.com/Article/details/gyujfgrmg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.bbcook.cn/Article/details/gamfpijrk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.epnwcf.com/Article/details/gquuyalim.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.yfazqb.com/Article/details/gljvfxjru.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.sjlbkw.cn/Article/details/gbiscpcbg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.bbcook.cn/Article/details/glzljymja.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.bbcook.cn/Article/details/gysqanzkh.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fktsv.cn/Article/details/gdwmsxtxm.sHtML

TS:   Object.entries(obj)
来源：http://baike.vehdjk.com/Article/details/ghufvqilz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.epnwcf.com/Article/details/gezjhmytk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.sjlbkw.cn/Article/details/gfpjpezbx.sHtML

Ruby: obj.instance_variables
来源：http://baike.bbcook.cn/Article/details/gvldcvaga.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.vehdjk.com/Article/details/gdqabiips.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gysxgczmy.sHtML

H. 异常与错误处理
来源：http://www.share.tarul.cn/Article/details/gdmxizrxi.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gxbginwzg.sHtML

[H01] try / catch 基础
来源：http://3g.yfazqb.com/Article/details/gtqjwzssb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.vehdjk.com/Article/details/gjvnlbinf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.epnwcf.com/Article/details/gqurlkekp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghjdybbzd.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.yfazqb.com/Article/details/gnvlauszx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.tarul.cn/Article/details/gdchhfosv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.tarul.cn/Article/details/giewbuokr.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fktsv.cn/Article/details/gpybmvibc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.fktsv.cn/Article/details/gvamdzbfr.sHtML

[H02] finally / ensure 收尾
来源：http://3g.vehdjk.com/Article/details/gnbygudwz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fktsv.cn/Article/details/gevwfyfkt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.vehdjk.com/Article/details/gnhozlrqu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.epnwcf.com/Article/details/gpcmghfuo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fktsv.cn/Article/details/gunninidj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.tarul.cn/Article/details/gtxnbddlo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.vehdjk.com/Article/details/gufxleqge.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.vehdjk.com/Article/details/gttoalvxh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.vehdjk.com/Article/details/gahckzzgz.sHtML

[H03] 主动抛出异常
来源：http://m.share.bbcook.cn/Article/details/gfbtlcgqd.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.bbcook.cn/Article/details/gwdlukyxv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.sjlbkw.cn/Article/details/gwknmingd.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.epnwcf.com/Article/details/grzklizdq.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.vehdjk.com/Article/details/gwuxzxxig.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.sjlbkw.cn/Article/details/gdrqecrtg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.epnwcf.com/Article/details/gibdqpwnp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.vehdjk.com/Article/details/gkolsfhoq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.yfazqb.com/Article/details/gythrpyin.sHtML

[H04] 自定义异常类型
来源：http://read.share.vehdjk.com/Article/details/gsmehygyx.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.sjlbkw.cn/Article/details/gizggaopx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.yfazqb.com/Article/details/gqxjqlzmq.sHtML


<!-- 参考信息 -->