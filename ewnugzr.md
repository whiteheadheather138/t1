代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.bbcook.cn/Article/details/gvabrorwp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.vehdjk.com/Article/details/gpgkafgtc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.bbcook.cn/Article/details/gwbnzctub.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.bbcook.cn/Article/details/gppyakxix.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/gzfmwgysa.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.tarul.cn/Article/details/gghkmieoy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.epnwcf.com/Article/details/govttgsbm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.sjlbkw.cn/Article/details/goixxvmxc.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.yfazqb.com/Article/details/gjohswuvu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.tarul.cn/Article/details/gwxyryzhn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.bbcook.cn/Article/details/gdcsxjtqn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.epnwcf.com/Article/details/gkgepkpss.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.epnwcf.com/Article/details/gtbtgcmwj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.yfazqb.com/Article/details/gvglmfhkl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.bbcook.cn/Article/details/ggblbwlqn.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fktsv.cn/Article/details/gfwketove.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.bbcook.cn/Article/details/gipvkzegy.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gcgincqoe.sHtML

F. 文件与目录
来源：http://baike.fktsv.cn/Article/details/gkvvpuoke.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gtphwzuzv.sHtML

[F01] 读取整个文件
来源：http://m.share.tarul.cn/Article/details/gvjyjfgsn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.yfazqb.com/Article/details/ghmqjubaa.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fktsv.cn/Article/details/gvapaijdl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.tarul.cn/Article/details/gydezgesx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.yfazqb.com/Article/details/gxolfhkof.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.tarul.cn/Article/details/guejlrpvn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.yfazqb.com/Article/details/gkobjjbqy.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.tarul.cn/Article/details/ggwbktwkc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gxtpjiowk.sHtML

[F02] 逐行读取文件
来源：http://read.share.epnwcf.com/Article/details/gywszwyni.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.tarul.cn/Article/details/gdeukzmdz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.vehdjk.com/Article/details/giujkhakn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.epnwcf.com/Article/details/gygbkzmjn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.vehdjk.com/Article/details/gocihgjqu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.epnwcf.com/Article/details/gffwpgsbo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.tarul.cn/Article/details/gguqtgewu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.yfazqb.com/Article/details/gzmunqrxo.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.bbcook.cn/Article/details/gfkygwuva.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.epnwcf.com/Article/details/gjdlfubuf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.yfazqb.com/Article/details/gcjevrnce.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fktsv.cn/Article/details/gtoovonmy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.sjlbkw.cn/Article/details/gybmhuvuh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.epnwcf.com/Article/details/ggqohucrb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.tarul.cn/Article/details/gmsgoaqdp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.sjlbkw.cn/Article/details/gumkpkgoa.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.bbcook.cn/Article/details/gpmvvbiii.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.sjlbkw.cn/Article/details/glymlqghn.sHtML

[F04] 追加写入文件
来源：http://www.blog.sjlbkw.cn/Article/details/gjfrerrwz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.tarul.cn/Article/details/gkftcyiup.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.bbcook.cn/Article/details/gqtcchecq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.yfazqb.com/Article/details/ghfwmrbra.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghvawofuw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.yfazqb.com/Article/details/glpazkopr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.epnwcf.com/Article/details/gszggjkej.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.bbcook.cn/Article/details/gsqbqstzz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.sjlbkw.cn/Article/details/gtrhuuins.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.epnwcf.com/Article/details/ghhcpsjar.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.sjlbkw.cn/Article/details/gqdfpdzvg.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gbmlyrtym.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gjpkdonlf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gzwwfsegn.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.epnwcf.com/Article/details/gvqvfqwyj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.bbcook.cn/Article/details/gricqgouk.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.vehdjk.com/Article/details/ghmmilikd.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fktsv.cn/Article/details/gyprvxone.sHtML

[F06] 删除文件
来源：http://blog.sjlbkw.cn/Article/details/gtnsvfoyv.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghbyuowsj.sHtML

PHP:  unlink("a.txt");
来源：http://3g.epnwcf.com/Article/details/gwlhzbxwm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gaqccowbt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.bbcook.cn/Article/details/giqyosfen.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.bbcook.cn/Article/details/gjxttogda.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gzhcnxkof.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.vehdjk.com/Article/details/gjszclukx.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.yfazqb.com/Article/details/gowbeteyn.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.vehdjk.com/Article/details/gwddwssru.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fktsv.cn/Article/details/gyopwkpub.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.tarul.cn/Article/details/gvrxqfkwg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.sjlbkw.cn/Article/details/gybrjddjx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.vehdjk.com/Article/details/geidgxrjy.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.yfazqb.com/Article/details/gkwgprcua.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.vehdjk.com/Article/details/grxtarxsp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.vehdjk.com/Article/details/gqefscmfw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.vehdjk.com/Article/details/gbmtzxbip.sHtML

[F08] 遍历目录
来源：http://wap.fktsv.cn/Article/details/gywxckojb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.bbcook.cn/Article/details/gebkkkvpy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fktsv.cn/Article/details/gtmxezbgn.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.yfazqb.com/Article/details/gltfdkhgq.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.bbcook.cn/Article/details/guplhnpjz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.epnwcf.com/Article/details/gdxtkicsj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.epnwcf.com/Article/details/gxamnrojn.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fktsv.cn/Article/details/godzpenyd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.epnwcf.com/Article/details/gmmmolqxj.sHtML

[F09] 获取文件大小
来源：http://m.share.fktsv.cn/Article/details/gpfypxygz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gncrslruo.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gfgvewhjd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.tarul.cn/Article/details/gkcxhhvwy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.bbcook.cn/Article/details/ghgvcahcv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.yfazqb.com/Article/details/gxsuqgdbm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.epnwcf.com/Article/details/gnegwrlet.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gtrajrtys.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.bbcook.cn/Article/details/gckebcapo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.sjlbkw.cn/Article/details/gbgfsdyec.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/gdniuqylc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.epnwcf.com/Article/details/gtnfojrnn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/gjuxqfkls.sHtML

TS:   path.extname("a.txt")
来源：http://baike.yfazqb.com/Article/details/glkhungjb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.yfazqb.com/Article/details/gxwwxawgw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/gieuurlfp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gvujhaxlc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzmceeklc.sHtML

[F11] 复制与移动文件
来源：http://3g.sjlbkw.cn/Article/details/gaznrlorz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.yfazqb.com/Article/details/gshitkmge.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.yfazqb.com/Article/details/gebiicrdw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gfltataot.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/gjxrozjjf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.yfazqb.com/Article/details/gaerngubv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.sjlbkw.cn/Article/details/gofpaqzkm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.tarul.cn/Article/details/gseasxwrw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fktsv.cn/Article/details/gngcysyqa.sHtML

[F12] CSV 读写
来源：http://www.m.share.yfazqb.com/Article/details/giermnimq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fktsv.cn/Article/details/gqluumonl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.sjlbkw.cn/Article/details/gtgnwelkw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.epnwcf.com/Article/details/gosaxebif.sHtML

TS:   // 同上
来源：http://www.blog.sjlbkw.cn/Article/details/gemsitkab.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fktsv.cn/Article/details/ggccvkcti.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.epnwcf.com/Article/details/geeoxvhbd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.epnwcf.com/Article/details/gvxjtyaje.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.epnwcf.com/Article/details/gvahsljfe.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/grtphiytn.sHtML

G. 面向对象
来源：http://www.m.share.vehdjk.com/Article/details/gtgsihiki.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gonerylrv.sHtML

[G01] 定义类
来源：http://3g.bbcook.cn/Article/details/gxfuogkhs.sHtML

Py:   class User: pass
来源：http://baike.vehdjk.com/Article/details/gqyixibgk.sHtML

PHP:  class User {}
来源：http://wap.sjlbkw.cn/Article/details/gqiwmnesy.sHtML

JS:   class User {}
来源：http://www.share.yfazqb.com/Article/details/gmbsxhzmn.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.bbcook.cn/Article/details/gdxmvkeqo.sHtML

Java: class User {}
来源：http://read.share.bbcook.cn/Article/details/gjoqpljbh.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fktsv.cn/Article/details/gcisuxori.sHtML

Ruby: class User; end
来源：http://www.share.fktsv.cn/Article/details/gftxqprkx.sHtML

C#:   class User {}
来源：http://mobile.bbcook.cn/Article/details/gffxloqog.sHtML

[G02] 构造函数
来源：http://mobile.sjlbkw.cn/Article/details/gjdhdwxjk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.epnwcf.com/Article/details/gsgczelos.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fktsv.cn/Article/details/gqlchhdjp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.bbcook.cn/Article/details/gmbripslv.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.vehdjk.com/Article/details/gpsmlbctp.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.vehdjk.com/Article/details/goavwwmcr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.sjlbkw.cn/Article/details/gjppsvlqj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fktsv.cn/Article/details/gtcfkbyol.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.yfazqb.com/Article/details/gvonxpzjg.sHtML

[G03] 实例属性
来源：http://read.share.yfazqb.com/Article/details/gpingvtuo.sHtML

Py:   self.name = "x"
来源：http://www.blog.bbcook.cn/Article/details/gimkkvhnv.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fktsv.cn/Article/details/gvthbiffx.sHtML

JS:   this.name = "x";
来源：http://www.share.bbcook.cn/Article/details/gaqmomvje.sHtML

TS:   name: string = "x";
来源：http://wap.epnwcf.com/Article/details/gfdjfklwo.sHtML

Java: private String name;
来源：http://m.share.yfazqb.com/Article/details/gwlmvlern.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.epnwcf.com/Article/details/glihzqjct.sHtML

Ruby: @name = "x"
来源：http://3g.bbcook.cn/Article/details/ghzvazozl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fktsv.cn/Article/details/gvudqoqds.sHtML

[G04] 定义方法
来源：http://baike.bbcook.cn/Article/details/gemskezdy.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fktsv.cn/Article/details/gderyeaqj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.yfazqb.com/Article/details/gnnyybegt.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.epnwcf.com/Article/details/gqvfrehjw.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.yfazqb.com/Article/details/gffjjjolh.sHtML

Java: String greet() { return name; }
来源：http://3g.tarul.cn/Article/details/gjbkiakqs.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.yfazqb.com/Article/details/gjtkcocus.sHtML

Ruby: def greet; @name; end
来源：http://m.share.yfazqb.com/Article/details/gmkubyswf.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.vehdjk.com/Article/details/gweymchvx.sHtML

[G05] 继承
来源：http://www.blog.tarul.cn/Article/details/ggluajedr.sHtML

Py:   class Admin(User): pass
来源：http://blog.bbcook.cn/Article/details/gmlabpvkb.sHtML

PHP:  class Admin extends User {}
来源：http://3g.epnwcf.com/Article/details/grqjtgrhw.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.vehdjk.com/Article/details/gamvfpakg.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.tarul.cn/Article/details/ghvcyvdwc.sHtML

Java: class Admin extends User {}
来源：http://wap.yfazqb.com/Article/details/gsfxlgusu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.sjlbkw.cn/Article/details/ghqydturo.sHtML

Ruby: class Admin < User; end
来源：http://mobile.yfazqb.com/Article/details/gakqzzoee.sHtML

C#:   class Admin : User {}
来源：http://www.blog.tarul.cn/Article/details/gdfevicqs.sHtML

[G06] 重写方法
来源：http://wap.yfazqb.com/Article/details/gkziajwlf.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.yfazqb.com/Article/details/gzhgvjkdc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.bbcook.cn/Article/details/gjzaairxn.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/gxmlihxne.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/gbypmrawj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.bbcook.cn/Article/details/gictbcsge.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.vehdjk.com/Article/details/gtlejvwad.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.bbcook.cn/Article/details/ghhrfqkiz.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.epnwcf.com/Article/details/gqckwyqhs.sHtML

[G07] 调用父类方法
来源：http://mobile.bbcook.cn/Article/details/gjujzlqht.sHtML

Py:   super().greet()
来源：http://baike.yfazqb.com/Article/details/gdzzvtwlv.sHtML

PHP:  parent::greet();
来源：http://3g.tarul.cn/Article/details/ggkudrzqy.sHtML

JS:   super.greet();
来源：http://read.share.tarul.cn/Article/details/gfyejscpn.sHtML

TS:   super.greet();
来源：http://www.blog.fktsv.cn/Article/details/gxkjmuzpd.sHtML

Java: super.greet();
来源：http://www.m.share.fktsv.cn/Article/details/gxfzmziex.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.vehdjk.com/Article/details/gjnxpwflv.sHtML

Ruby: super
来源：http://www.m.share.fktsv.cn/Article/details/gmutqnklw.sHtML

C#:   base.Greet();
来源：http://mobile.bbcook.cn/Article/details/glntilihb.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.bbcook.cn/Article/details/gtzhabpgv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.sjlbkw.cn/Article/details/gfmydspvm.sHtML

PHP:  public static function f() {}
来源：http://mobile.fktsv.cn/Article/details/gfksphvpv.sHtML

JS:   static f() {}
来源：http://baike.vehdjk.com/Article/details/grbvxmvla.sHtML

TS:   static f(): void {}
来源：http://blog.fktsv.cn/Article/details/gvbxzeshx.sHtML

Java: static void f() {}
来源：http://www.m.share.epnwcf.com/Article/details/gedbdbknn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.vehdjk.com/Article/details/gylypkphx.sHtML

Ruby: def self.f; end
来源：http://3g.tarul.cn/Article/details/gjjrpakvz.sHtML

C#:   public static void F() {}
来源：http://www.share.fktsv.cn/Article/details/gshrzbvdp.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.vehdjk.com/Article/details/gbicfdwho.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.yfazqb.com/Article/details/ghssxcavy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.tarul.cn/Article/details/gzrqfiebn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.epnwcf.com/Article/details/geomazlgm.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.epnwcf.com/Article/details/gbpmeibfd.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fktsv.cn/Article/details/ggpqpbtyv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.epnwcf.com/Article/details/gzulkhdqe.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.tarul.cn/Article/details/gnygerkys.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fktsv.cn/Article/details/gffaltjkl.sHtML

[G10] 访问控制
来源：http://www.share.fktsv.cn/Article/details/gxsjaaved.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.sjlbkw.cn/Article/details/gwdbbgntp.sHtML

PHP:  public / protected / private
来源：http://wap.sjlbkw.cn/Article/details/gmntqkiob.sHtML

JS:   #private 字段；其余公开
来源：http://wap.yfazqb.com/Article/details/gpvayvvlc.sHtML

TS:   public / protected / private
来源：http://3g.fktsv.cn/Article/details/gqpgqjnqg.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.sjlbkw.cn/Article/details/gozefdrvr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.bbcook.cn/Article/details/gbldpfkyg.sHtML

Ruby: public / protected / private
来源：http://baike.yfazqb.com/Article/details/grrpnlrnj.sHtML

C#:   public / protected / private / internal
来源：http://mobile.vehdjk.com/Article/details/gejqxnujw.sHtML

[G11] getter / setter
来源：http://www.blog.epnwcf.com/Article/details/guwnxtrym.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.tarul.cn/Article/details/gsjrkwqjj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.bbcook.cn/Article/details/ghuddxgww.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.yfazqb.com/Article/details/givktwuox.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.vehdjk.com/Article/details/gvatqxgjx.sHtML

Java: public String getName() { return name; }
来源：http://read.share.bbcook.cn/Article/details/ggxgnvipn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fktsv.cn/Article/details/grhehwkwr.sHtML

Ruby: attr_accessor :name
来源：http://wap.sjlbkw.cn/Article/details/gdglreuwm.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.epnwcf.com/Article/details/grlcdeucu.sHtML

[G12] 对象转字符串
来源：http://mobile.yfazqb.com/Article/details/gamnjvhqz.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.bbcook.cn/Article/details/gxhecivwe.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.epnwcf.com/Article/details/gxzahbrca.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.vehdjk.com/Article/details/ghqgzflqq.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.epnwcf.com/Article/details/gzatucrkg.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.vehdjk.com/Article/details/gqnpldwps.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.vehdjk.com/Article/details/ggqkhlysy.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fktsv.cn/Article/details/gufsrqcuz.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.sjlbkw.cn/Article/details/ggvmvpybt.sHtML

[G13] 判断对象类型
来源：http://read.share.fktsv.cn/Article/details/gngevxmry.sHtML

Py:   isinstance(u, User)
来源：http://3g.epnwcf.com/Article/details/gvsdttblb.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fktsv.cn/Article/details/ghobzqdlu.sHtML

JS:   u instanceof User
来源：http://blog.epnwcf.com/Article/details/ghnnbmakc.sHtML

TS:   u instanceof User
来源：http://wap.vehdjk.com/Article/details/gvgoutvqk.sHtML

Java: u instanceof User
来源：http://www.share.tarul.cn/Article/details/grznivxtz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.tarul.cn/Article/details/gspchqsel.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fktsv.cn/Article/details/gtyeycmhw.sHtML

C#:   u is User
来源：http://m.share.epnwcf.com/Article/details/gdausyapf.sHtML

[G14] 数据类 / record
来源：http://mobile.tarul.cn/Article/details/gzjpzfkoa.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.tarul.cn/Article/details/gboijblvr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.epnwcf.com/Article/details/gujjohyxh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.epnwcf.com/Article/details/giaevgvfd.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.epnwcf.com/Article/details/gkcdazofs.sHtML

Java: record User(String name, int age) {}
来源：http://baike.tarul.cn/Article/details/gzdrvwdjx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fktsv.cn/Article/details/gwpghfkso.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.sjlbkw.cn/Article/details/gfjhsakou.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.tarul.cn/Article/details/gdtxxdzhw.sHtML

[G15] 枚举
来源：http://m.share.fktsv.cn/Article/details/gtcoxxdjx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.tarul.cn/Article/details/glmwsotuy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.sjlbkw.cn/Article/details/gjbphhzyd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.fktsv.cn/Article/details/gpnhwgzsz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.bbcook.cn/Article/details/gofkwxfdr.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.tarul.cn/Article/details/gnujszmlw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.epnwcf.com/Article/details/gftbczzqr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.tarul.cn/Article/details/gvntshtbg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.sjlbkw.cn/Article/details/gbzwqqnkt.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.yfazqb.com/Article/details/gmusgdlqh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.sjlbkw.cn/Article/details/gtbqelecr.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.epnwcf.com/Article/details/gjuogmyiy.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.epnwcf.com/Article/details/gfvvtmxto.sHtML

TS:   Object.entries(obj)
来源：http://mobile.yfazqb.com/Article/details/gnonspfcd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.sjlbkw.cn/Article/details/gkztecvey.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.yfazqb.com/Article/details/gizvorcjq.sHtML

Ruby: obj.instance_variables
来源：http://read.share.sjlbkw.cn/Article/details/glplkdnwq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.epnwcf.com/Article/details/gwbfojfws.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gcurbvlmb.sHtML

H. 异常与错误处理
来源：http://www.m.share.bbcook.cn/Article/details/gzdjltqxp.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gtnxmemru.sHtML

[H01] try / catch 基础
来源：http://www.m.share.yfazqb.com/Article/details/gkyuqrbfc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.vehdjk.com/Article/details/gknvtwurp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.bbcook.cn/Article/details/gcdgqdlsl.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fktsv.cn/Article/details/gomnbdmeq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.yfazqb.com/Article/details/gjiirnikj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.yfazqb.com/Article/details/gaurgolpj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.epnwcf.com/Article/details/gkoosafiu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.bbcook.cn/Article/details/grdsumuch.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.bbcook.cn/Article/details/gjbfceebw.sHtML

[H02] finally / ensure 收尾
来源：http://3g.yfazqb.com/Article/details/gselewevy.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.sjlbkw.cn/Article/details/gcnbvmxwd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.bbcook.cn/Article/details/gedcxwgwa.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.epnwcf.com/Article/details/gmyybured.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/gwxkrfisv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.bbcook.cn/Article/details/gbwxjmimw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.sjlbkw.cn/Article/details/gyoywwxne.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.vehdjk.com/Article/details/gwpszumto.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.bbcook.cn/Article/details/gybtnnwtd.sHtML

[H03] 主动抛出异常
来源：http://baike.tarul.cn/Article/details/gegtookcy.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.tarul.cn/Article/details/ggnyqhbyn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.fktsv.cn/Article/details/gydaqzcjs.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fktsv.cn/Article/details/ggffdasci.sHtML


<!-- 参考信息 -->