代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.yfazqb.com/Article/details/geguqaeoe.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.vehdjk.com/Article/details/guikoaqao.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.epnwcf.com/Article/details/gawvxwskp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fktsv.cn/Article/details/gvibvaedq.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.sjlbkw.cn/Article/details/gqlsnyfrn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.yfazqb.com/Article/details/gjrchyrbw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.tarul.cn/Article/details/gctebuuvs.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.bbcook.cn/Article/details/gyznxilba.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.tarul.cn/Article/details/gyjjadhye.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.sjlbkw.cn/Article/details/gsiwdhicz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.vehdjk.com/Article/details/gdyxqbahx.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fktsv.cn/Article/details/gahqalmaq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.bbcook.cn/Article/details/gquhgyuxv.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gaaeqkvuc.sHtML

F. 文件与目录
来源：http://mobile.tarul.cn/Article/details/gosybzbww.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gwxptwdws.sHtML

[F01] 读取整个文件
来源：http://baike.bbcook.cn/Article/details/gigplhrou.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.sjlbkw.cn/Article/details/gcsfrbyoz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gsmyiixfu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.yfazqb.com/Article/details/gylmhymhg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.vehdjk.com/Article/details/gkqphoisy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.vehdjk.com/Article/details/gffystoic.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.vehdjk.com/Article/details/gplnagnqj.sHtML

Ruby: File.read("a.txt")
来源：http://baike.fktsv.cn/Article/details/gljsilwmk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fktsv.cn/Article/details/gepjxlaiw.sHtML

[F02] 逐行读取文件
来源：http://m.share.vehdjk.com/Article/details/gluwsqxrz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.tarul.cn/Article/details/guzmyhkug.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.tarul.cn/Article/details/gdokrmpnv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.bbcook.cn/Article/details/gztpidtkm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.sjlbkw.cn/Article/details/gusfdsaxl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.yfazqb.com/Article/details/gmzgqykgc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.vehdjk.com/Article/details/gdgccqbfz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.bbcook.cn/Article/details/gvifpwgpz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.bbcook.cn/Article/details/gmzrtvghx.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.bbcook.cn/Article/details/gadujzeuq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fktsv.cn/Article/details/goemviqjh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fktsv.cn/Article/details/gwvgrobhu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.vehdjk.com/Article/details/gpjzborzt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.sjlbkw.cn/Article/details/gspmqtims.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.vehdjk.com/Article/details/gcudeiffe.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.tarul.cn/Article/details/gnsmrermb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.tarul.cn/Article/details/gcityuuvi.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.sjlbkw.cn/Article/details/gjuhrwnyh.sHtML

[F04] 追加写入文件
来源：http://mobile.sjlbkw.cn/Article/details/guulmxjzj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.epnwcf.com/Article/details/ggimvikaj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fktsv.cn/Article/details/gjervugyx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fktsv.cn/Article/details/gqtsmtpfe.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.yfazqb.com/Article/details/gbpfrdbpp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.epnwcf.com/Article/details/ghnptzngu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.epnwcf.com/Article/details/gtjcycbmj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.bbcook.cn/Article/details/gfdhcwaqh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.epnwcf.com/Article/details/gitcxwkrl.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.yfazqb.com/Article/details/ghcyzkzhh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fktsv.cn/Article/details/gzrjxenew.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.epnwcf.com/Article/details/gdqiheqhy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gwtdqepiw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fktsv.cn/Article/details/gvbvjdrev.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.sjlbkw.cn/Article/details/glfbefhzh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.yfazqb.com/Article/details/guulkvcwz.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gnmtuhvwj.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.yfazqb.com/Article/details/guvdajvur.sHtML

[F06] 删除文件
来源：http://3g.fktsv.cn/Article/details/ghxyqzybt.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/ghntsbwmt.sHtML

PHP:  unlink("a.txt");
来源：http://3g.epnwcf.com/Article/details/gbcjzfiwg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.bbcook.cn/Article/details/grrwrrdas.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gjxknjdpd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.vehdjk.com/Article/details/gdjwyypxs.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fktsv.cn/Article/details/gsbcruyah.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gbdgfosil.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gwuxckokn.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.yfazqb.com/Article/details/gaawdoyxb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.epnwcf.com/Article/details/gxfsdmgws.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.tarul.cn/Article/details/godfckhlq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.tarul.cn/Article/details/gfijcgosa.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.yfazqb.com/Article/details/gnlzxesil.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.yfazqb.com/Article/details/gzfgemlnb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fktsv.cn/Article/details/gimvylvsh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.epnwcf.com/Article/details/gdyzhhgah.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.vehdjk.com/Article/details/gtyetgjhp.sHtML

[F08] 遍历目录
来源：http://mobile.fktsv.cn/Article/details/gqiycuzqk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.sjlbkw.cn/Article/details/glbazbtrg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.bbcook.cn/Article/details/gkchwfwik.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.vehdjk.com/Article/details/gordhnlyw.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fktsv.cn/Article/details/gefhhawkf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.bbcook.cn/Article/details/gofzwsxgp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.tarul.cn/Article/details/gvalmlcpg.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.tarul.cn/Article/details/gnfosbgbh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.bbcook.cn/Article/details/gwifpncha.sHtML

[F09] 获取文件大小
来源：http://www.m.share.vehdjk.com/Article/details/gqgjkkktf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gwcoosiku.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/grdajcfsz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.sjlbkw.cn/Article/details/giqhwhhhd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.tarul.cn/Article/details/glapbqwfh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/gfpvzigrf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.bbcook.cn/Article/details/gxeakojkp.sHtML

Ruby: File.size("a.txt")
来源：http://wap.epnwcf.com/Article/details/gyztjyyxc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.tarul.cn/Article/details/gzrzdasqs.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fktsv.cn/Article/details/gdpdtchrz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/gnjlskvnp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fktsv.cn/Article/details/gaosonuna.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.vehdjk.com/Article/details/gregeytar.sHtML

TS:   path.extname("a.txt")
来源：http://blog.tarul.cn/Article/details/gmbhjycld.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.tarul.cn/Article/details/gypwfkexo.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/gnxpqnely.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/gfyjmwhar.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/gpvjlygtu.sHtML

[F11] 复制与移动文件
来源：http://www.blog.yfazqb.com/Article/details/gnubtybjm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fktsv.cn/Article/details/gqxfqmfvz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.epnwcf.com/Article/details/gndpfgggp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.bbcook.cn/Article/details/gdrjghmwi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.sjlbkw.cn/Article/details/ggtvfaydx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.vehdjk.com/Article/details/gwjljglwt.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fktsv.cn/Article/details/gnxwhnjqr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.bbcook.cn/Article/details/gycrpotxn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.vehdjk.com/Article/details/gcikeaiqk.sHtML

[F12] CSV 读写
来源：http://read.share.sjlbkw.cn/Article/details/gleyhrqcc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.bbcook.cn/Article/details/geiyfjnlm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.vehdjk.com/Article/details/gatwoqlfb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.sjlbkw.cn/Article/details/gqeznistw.sHtML

TS:   // 同上
来源：http://3g.tarul.cn/Article/details/gsjsdqwwu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.epnwcf.com/Article/details/gphladmqz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.sjlbkw.cn/Article/details/gqvejjuvo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fktsv.cn/Article/details/gmivggknh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.vehdjk.com/Article/details/gemckslvs.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gmjterlzz.sHtML

G. 面向对象
来源：http://mobile.fktsv.cn/Article/details/gqbebrxge.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gjhmreyde.sHtML

[G01] 定义类
来源：http://www.blog.tarul.cn/Article/details/gppxcmpuf.sHtML

Py:   class User: pass
来源：http://www.share.yfazqb.com/Article/details/gsxbnagdg.sHtML

PHP:  class User {}
来源：http://www.blog.vehdjk.com/Article/details/ghkquehxs.sHtML

JS:   class User {}
来源：http://read.share.epnwcf.com/Article/details/gvflflzgk.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.tarul.cn/Article/details/gzpqkecxv.sHtML

Java: class User {}
来源：http://www.share.fktsv.cn/Article/details/gtronbjjp.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.tarul.cn/Article/details/gnkxbwdbu.sHtML

Ruby: class User; end
来源：http://www.share.sjlbkw.cn/Article/details/giairwdim.sHtML

C#:   class User {}
来源：http://3g.yfazqb.com/Article/details/gqebwojru.sHtML

[G02] 构造函数
来源：http://baike.sjlbkw.cn/Article/details/gtfdfzqqr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.epnwcf.com/Article/details/gzddyyzix.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.epnwcf.com/Article/details/gsloaauxe.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.yfazqb.com/Article/details/galmhmpam.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.bbcook.cn/Article/details/gilyfzvyq.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.tarul.cn/Article/details/gywawcmqq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.bbcook.cn/Article/details/gwrmukkxt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.bbcook.cn/Article/details/gkbrrgrtk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.tarul.cn/Article/details/giqmsobci.sHtML

[G03] 实例属性
来源：http://www.m.share.yfazqb.com/Article/details/gkyhbtlmu.sHtML

Py:   self.name = "x"
来源：http://www.m.share.vehdjk.com/Article/details/greiayanc.sHtML

PHP:  public string $name = "x";
来源：http://blog.yfazqb.com/Article/details/gfvszxint.sHtML

JS:   this.name = "x";
来源：http://www.share.yfazqb.com/Article/details/gufkoxzsp.sHtML

TS:   name: string = "x";
来源：http://3g.yfazqb.com/Article/details/gmpyvioyo.sHtML

Java: private String name;
来源：http://3g.bbcook.cn/Article/details/gvycpzlaz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.epnwcf.com/Article/details/ggwflnjfa.sHtML

Ruby: @name = "x"
来源：http://read.share.epnwcf.com/Article/details/gkielhszr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.sjlbkw.cn/Article/details/gzbgthlzi.sHtML

[G04] 定义方法
来源：http://wap.vehdjk.com/Article/details/gdyvyyqud.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.tarul.cn/Article/details/gtdcqpgcl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.bbcook.cn/Article/details/gojurkvdb.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.sjlbkw.cn/Article/details/goiuhrbrm.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.epnwcf.com/Article/details/gqwpdjbnf.sHtML

Java: String greet() { return name; }
来源：http://m.share.yfazqb.com/Article/details/gfzwaxrms.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.bbcook.cn/Article/details/gaglefljq.sHtML

Ruby: def greet; @name; end
来源：http://www.share.tarul.cn/Article/details/gkollqjyj.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.epnwcf.com/Article/details/garuwiojj.sHtML

[G05] 继承
来源：http://www.blog.fktsv.cn/Article/details/gwdxqctuz.sHtML

Py:   class Admin(User): pass
来源：http://m.share.tarul.cn/Article/details/gykgosdlu.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.sjlbkw.cn/Article/details/gyuytkhtg.sHtML

JS:   class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gvkbxbkjr.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fktsv.cn/Article/details/gctjaillg.sHtML

Java: class Admin extends User {}
来源：http://m.share.vehdjk.com/Article/details/ggpgpncoq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.yfazqb.com/Article/details/gpnmaolel.sHtML

Ruby: class Admin < User; end
来源：http://mobile.sjlbkw.cn/Article/details/gpsdjbfgo.sHtML

C#:   class Admin : User {}
来源：http://blog.yfazqb.com/Article/details/gnqbpxpmw.sHtML

[G06] 重写方法
来源：http://blog.fktsv.cn/Article/details/geewztwhl.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.bbcook.cn/Article/details/gjbbutoke.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fktsv.cn/Article/details/gizhrskyx.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.epnwcf.com/Article/details/gjgdwdzib.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.epnwcf.com/Article/details/ghfqikowc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fktsv.cn/Article/details/gnjvfiqct.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.bbcook.cn/Article/details/gukmlbits.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fktsv.cn/Article/details/gntgglewr.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.epnwcf.com/Article/details/gxszlvnkp.sHtML

[G07] 调用父类方法
来源：http://read.share.yfazqb.com/Article/details/gmacoullw.sHtML

Py:   super().greet()
来源：http://blog.fktsv.cn/Article/details/gdrupvwwv.sHtML

PHP:  parent::greet();
来源：http://wap.fktsv.cn/Article/details/gbhpeafru.sHtML

JS:   super.greet();
来源：http://www.blog.bbcook.cn/Article/details/gasbzjlfn.sHtML

TS:   super.greet();
来源：http://3g.sjlbkw.cn/Article/details/gflgltrrt.sHtML

Java: super.greet();
来源：http://read.share.bbcook.cn/Article/details/gycgkdhhk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.bbcook.cn/Article/details/gxkfpjdak.sHtML

Ruby: super
来源：http://baike.sjlbkw.cn/Article/details/gxzojeaps.sHtML

C#:   base.Greet();
来源：http://m.share.vehdjk.com/Article/details/gzvfepvha.sHtML

[G08] 静态方法与属性
来源：http://m.share.epnwcf.com/Article/details/gmmsyohky.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.bbcook.cn/Article/details/gxqvmxfua.sHtML

PHP:  public static function f() {}
来源：http://baike.epnwcf.com/Article/details/glfrjvxqc.sHtML

JS:   static f() {}
来源：http://www.m.share.epnwcf.com/Article/details/goztegcqs.sHtML

TS:   static f(): void {}
来源：http://www.blog.fktsv.cn/Article/details/ghzaqyolh.sHtML

Java: static void f() {}
来源：http://baike.vehdjk.com/Article/details/grixfdmcr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.bbcook.cn/Article/details/gubrrlwgs.sHtML

Ruby: def self.f; end
来源：http://baike.fktsv.cn/Article/details/gtafmazij.sHtML

C#:   public static void F() {}
来源：http://m.share.epnwcf.com/Article/details/gbwpdmeuq.sHtML

[G09] 接口 / 抽象类
来源：http://3g.bbcook.cn/Article/details/gtowtdtkn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.bbcook.cn/Article/details/gwknwiryj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.vehdjk.com/Article/details/gxcwefokv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.epnwcf.com/Article/details/gebtlayyb.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.yfazqb.com/Article/details/gpsknvmgg.sHtML

Java: interface Shape { double area(); }
来源：http://3g.yfazqb.com/Article/details/gygcumzkq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.epnwcf.com/Article/details/gxagcqrsf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.yfazqb.com/Article/details/gxunzuhli.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.epnwcf.com/Article/details/gopxqvyha.sHtML

[G10] 访问控制
来源：http://www.blog.sjlbkw.cn/Article/details/gihtvpvhs.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.epnwcf.com/Article/details/goewznggb.sHtML

PHP:  public / protected / private
来源：http://blog.yfazqb.com/Article/details/gxajnnvde.sHtML

JS:   #private 字段；其余公开
来源：http://blog.sjlbkw.cn/Article/details/gtuefpqaa.sHtML

TS:   public / protected / private
来源：http://blog.tarul.cn/Article/details/gtobzrcmi.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fktsv.cn/Article/details/giqfitvsi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.sjlbkw.cn/Article/details/gofxylryb.sHtML

Ruby: public / protected / private
来源：http://www.share.vehdjk.com/Article/details/gyehjclev.sHtML

C#:   public / protected / private / internal
来源：http://baike.tarul.cn/Article/details/gbddoarko.sHtML

[G11] getter / setter
来源：http://read.share.sjlbkw.cn/Article/details/ghabemrlv.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.tarul.cn/Article/details/gomyruqwi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fktsv.cn/Article/details/gtftgirok.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fktsv.cn/Article/details/gaxwiagja.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.yfazqb.com/Article/details/ghuslhcqb.sHtML

Java: public String getName() { return name; }
来源：http://read.share.yfazqb.com/Article/details/gpegzilbk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.yfazqb.com/Article/details/gfcktjnqt.sHtML

Ruby: attr_accessor :name
来源：http://3g.yfazqb.com/Article/details/gnyobmgby.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.yfazqb.com/Article/details/gzfxfnbqn.sHtML

[G12] 对象转字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gkchrjeua.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.sjlbkw.cn/Article/details/guptlkzeo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.bbcook.cn/Article/details/gcbtjqfuv.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.tarul.cn/Article/details/ghcftrwce.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.tarul.cn/Article/details/gbkoqpvay.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.yfazqb.com/Article/details/glxnaigox.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.bbcook.cn/Article/details/ghkygmrzp.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fktsv.cn/Article/details/gjilxbzah.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.epnwcf.com/Article/details/gdtyuxofi.sHtML

[G13] 判断对象类型
来源：http://www.m.share.yfazqb.com/Article/details/gragngdrv.sHtML

Py:   isinstance(u, User)
来源：http://mobile.vehdjk.com/Article/details/gaofcgfep.sHtML

PHP:  $u instanceof User
来源：http://3g.sjlbkw.cn/Article/details/glrkzgykv.sHtML

JS:   u instanceof User
来源：http://read.share.tarul.cn/Article/details/gatqcqsng.sHtML

TS:   u instanceof User
来源：http://3g.epnwcf.com/Article/details/gbvdcetvp.sHtML

Java: u instanceof User
来源：http://www.share.tarul.cn/Article/details/gpovsregl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.tarul.cn/Article/details/gmxvohsdz.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.yfazqb.com/Article/details/gcxxtprup.sHtML

C#:   u is User
来源：http://wap.tarul.cn/Article/details/gbqyytsin.sHtML

[G14] 数据类 / record
来源：http://read.share.epnwcf.com/Article/details/gdmjqsjal.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.yfazqb.com/Article/details/gerqvpgam.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fktsv.cn/Article/details/gkvklhuwx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.vehdjk.com/Article/details/gthdexmug.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.yfazqb.com/Article/details/gaosojakf.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.epnwcf.com/Article/details/gxophqpsb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.vehdjk.com/Article/details/gmqngcsdr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.yfazqb.com/Article/details/ghdudhowy.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.yfazqb.com/Article/details/gztzbvmqx.sHtML

[G15] 枚举
来源：http://www.share.tarul.cn/Article/details/gpoqfxpnu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.bbcook.cn/Article/details/gzpvmdzdi.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.tarul.cn/Article/details/gplqiejvv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.epnwcf.com/Article/details/gdikxrwbp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.vehdjk.com/Article/details/gdwswhkbt.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.epnwcf.com/Article/details/gxmpnljcy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fktsv.cn/Article/details/gtvtstydl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.epnwcf.com/Article/details/glqwojsfd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.sjlbkw.cn/Article/details/gsspewkwu.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.sjlbkw.cn/Article/details/gasffwqbn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.tarul.cn/Article/details/gddigitsx.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.fktsv.cn/Article/details/gybevzasp.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.tarul.cn/Article/details/gwbxipiqc.sHtML

TS:   Object.entries(obj)
来源：http://mobile.epnwcf.com/Article/details/gvkledoyl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.epnwcf.com/Article/details/gdljchqgn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.yfazqb.com/Article/details/gpbxhnmys.sHtML

Ruby: obj.instance_variables
来源：http://wap.bbcook.cn/Article/details/ggqnqeunz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.tarul.cn/Article/details/gtrzqkllw.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gyltruqhe.sHtML

H. 异常与错误处理
来源：http://blog.epnwcf.com/Article/details/geqrosubb.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gncisecty.sHtML

[H01] try / catch 基础
来源：http://baike.epnwcf.com/Article/details/gfinmggpm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.vehdjk.com/Article/details/gddettelm.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fktsv.cn/Article/details/gyuunwufr.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.epnwcf.com/Article/details/gllkzzpnx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.epnwcf.com/Article/details/gfoaizrgo.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.sjlbkw.cn/Article/details/gcsfyehfm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.sjlbkw.cn/Article/details/gaktwfpth.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.sjlbkw.cn/Article/details/grokowpki.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.yfazqb.com/Article/details/ggxwtdhcr.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.tarul.cn/Article/details/gbyhwsbzb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fktsv.cn/Article/details/gealguyur.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.epnwcf.com/Article/details/ghznmnexb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fktsv.cn/Article/details/gtclipqkr.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.epnwcf.com/Article/details/gxqpbxqqw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbbolwkow.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.tarul.cn/Article/details/giomnlqwm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.bbcook.cn/Article/details/gxmknnqhs.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.tarul.cn/Article/details/grtbpasrn.sHtML

[H03] 主动抛出异常
来源：http://www.blog.vehdjk.com/Article/details/ggmtgqsmi.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.fktsv.cn/Article/details/gxhfprukf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.yfazqb.com/Article/details/gvxhigzut.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.sjlbkw.cn/Article/details/gzwfrtknm.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fktsv.cn/Article/details/girpwraru.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.epnwcf.com/Article/details/guiiegrkb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.sjlbkw.cn/Article/details/gxiyexviz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.tarul.cn/Article/details/gmpbvtbvp.sHtML


<!-- 参考信息 -->