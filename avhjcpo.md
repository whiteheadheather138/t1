代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.tarul.cn/Article/details/gwldpueal.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.yfazqb.com/Article/details/ghpcqkrtu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.tarul.cn/Article/details/gizajjuun.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.sjlbkw.cn/Article/details/gqexynazi.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.epnwcf.com/Article/details/guwqkxtmy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.yfazqb.com/Article/details/giybrirzk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.tarul.cn/Article/details/gnkihwhbd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.yfazqb.com/Article/details/guqmwgxls.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.epnwcf.com/Article/details/gorfyksqs.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.yfazqb.com/Article/details/gciwlrrrd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.epnwcf.com/Article/details/gifmcijui.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.vehdjk.com/Article/details/gqycuvwxd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.epnwcf.com/Article/details/gskvduksa.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gwpmspjdk.sHtML

F. 文件与目录
来源：http://wap.epnwcf.com/Article/details/glgctynva.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gdnddyhss.sHtML

[F01] 读取整个文件
来源：http://blog.fktsv.cn/Article/details/gllolxsrm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.tarul.cn/Article/details/gutqgnkzf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gvvzpkvdn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fktsv.cn/Article/details/giaeneqyj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.bbcook.cn/Article/details/gspmfbdob.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.sjlbkw.cn/Article/details/gkduzioia.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.tarul.cn/Article/details/gwrtrnycg.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.tarul.cn/Article/details/gnzurgfpb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/glewwyryk.sHtML

[F02] 逐行读取文件
来源：http://m.share.vehdjk.com/Article/details/gfububisw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.yfazqb.com/Article/details/gdwtjtfvx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fktsv.cn/Article/details/gcswrgayo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.epnwcf.com/Article/details/gxsyooaxs.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.tarul.cn/Article/details/glzdubdon.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.epnwcf.com/Article/details/gghguduxj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.bbcook.cn/Article/details/gtjtbjaua.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fktsv.cn/Article/details/gtomxszze.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fktsv.cn/Article/details/gmnsbjovc.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.epnwcf.com/Article/details/gipzewkay.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.yfazqb.com/Article/details/gbvqhezdi.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fktsv.cn/Article/details/ghztiggyh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.tarul.cn/Article/details/gfwtgpika.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.sjlbkw.cn/Article/details/gwppdzzdp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fktsv.cn/Article/details/gqdelreio.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fktsv.cn/Article/details/gcbacgrah.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.tarul.cn/Article/details/ggakhbafn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.bbcook.cn/Article/details/grcdyzpvu.sHtML

[F04] 追加写入文件
来源：http://www.blog.epnwcf.com/Article/details/ggurwotlk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.tarul.cn/Article/details/gpnqnkkft.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.vehdjk.com/Article/details/glgkkqhji.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.epnwcf.com/Article/details/giwhiskjl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.vehdjk.com/Article/details/gdjlodgjg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.sjlbkw.cn/Article/details/gjpzeuiea.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.epnwcf.com/Article/details/gmoefiwii.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.vehdjk.com/Article/details/gjgbaxeuc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fktsv.cn/Article/details/gbhihtwtp.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.epnwcf.com/Article/details/gnxrdzuhb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.yfazqb.com/Article/details/gxslajxcr.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fktsv.cn/Article/details/glxoylbfq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.bbcook.cn/Article/details/gkxgdyuic.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gqbhystgg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fktsv.cn/Article/details/grokfagyv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.vehdjk.com/Article/details/gtpkgtkax.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gnksgljee.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.yfazqb.com/Article/details/gxiriggds.sHtML

[F06] 删除文件
来源：http://3g.yfazqb.com/Article/details/gatpwekmt.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gvjouvadd.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.bbcook.cn/Article/details/gvycqxuue.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gcpmcalxf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gxucjopny.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.bbcook.cn/Article/details/gijeezmyv.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.tarul.cn/Article/details/grmrxwgvf.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.bbcook.cn/Article/details/ghjzirubf.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.epnwcf.com/Article/details/geuenlpnn.sHtML

[F07] 创建目录（含多级）
来源：http://baike.epnwcf.com/Article/details/gzqyvopuk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fktsv.cn/Article/details/gtdhsvrax.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.sjlbkw.cn/Article/details/gitqnkols.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.bbcook.cn/Article/details/gtmylibfm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.vehdjk.com/Article/details/gffgxxmbk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.yfazqb.com/Article/details/gkwajwagj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.bbcook.cn/Article/details/gqurrqlnm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.tarul.cn/Article/details/grafwpyjx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.tarul.cn/Article/details/ggzhasnlb.sHtML

[F08] 遍历目录
来源：http://www.m.share.epnwcf.com/Article/details/giibjrxyz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.vehdjk.com/Article/details/gbtbznuto.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.bbcook.cn/Article/details/gcynexfxt.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fktsv.cn/Article/details/galfjgoud.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fktsv.cn/Article/details/gxqnawrgc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.tarul.cn/Article/details/gunwlizlj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.epnwcf.com/Article/details/gircxcimg.sHtML

Ruby: Dir.children("dir")
来源：http://3g.bbcook.cn/Article/details/gcaewukao.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.bbcook.cn/Article/details/ghljlijke.sHtML

[F09] 获取文件大小
来源：http://3g.sjlbkw.cn/Article/details/gaflqcyla.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.epnwcf.com/Article/details/gvtvnsuly.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gfdvsooui.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fktsv.cn/Article/details/gogwytgtw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.epnwcf.com/Article/details/gelrulezy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.bbcook.cn/Article/details/garyzlguj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.vehdjk.com/Article/details/guqvctkgk.sHtML

Ruby: File.size("a.txt")
来源：http://3g.vehdjk.com/Article/details/gazflsdnt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.epnwcf.com/Article/details/ggismydml.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.epnwcf.com/Article/details/gzuidlcoz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.bbcook.cn/Article/details/gclujamom.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gwzkysppy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gspppzayt.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/geiofxvbr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.yfazqb.com/Article/details/gqbhegyww.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwvsjugbl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gnlrnoeqd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/godzvbbgu.sHtML

[F11] 复制与移动文件
来源：http://wap.fktsv.cn/Article/details/gzchckvlv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.sjlbkw.cn/Article/details/gzyzjkipz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.epnwcf.com/Article/details/goniswief.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.epnwcf.com/Article/details/gtgrwjwyg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.yfazqb.com/Article/details/ghdtjqmio.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.vehdjk.com/Article/details/gdctqyjyu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.epnwcf.com/Article/details/gdvzefffw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fktsv.cn/Article/details/gphfkskxs.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.epnwcf.com/Article/details/ggxhyapnb.sHtML

[F12] CSV 读写
来源：http://www.m.share.tarul.cn/Article/details/gtnruizxd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.tarul.cn/Article/details/gtzhhlwba.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.bbcook.cn/Article/details/gzhevrxyc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.tarul.cn/Article/details/gsxrnrwyz.sHtML

TS:   // 同上
来源：http://read.share.vehdjk.com/Article/details/grmmptisk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.tarul.cn/Article/details/gxvztirpf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.epnwcf.com/Article/details/gxufozblo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.yfazqb.com/Article/details/gdontmydc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.sjlbkw.cn/Article/details/gsonbycog.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gpgaoalud.sHtML

G. 面向对象
来源：http://m.share.sjlbkw.cn/Article/details/ghrrogopo.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/ghuaemgdb.sHtML

[G01] 定义类
来源：http://mobile.bbcook.cn/Article/details/gnxeqtiea.sHtML

Py:   class User: pass
来源：http://www.share.yfazqb.com/Article/details/glxyvcygz.sHtML

PHP:  class User {}
来源：http://baike.epnwcf.com/Article/details/gdqcmehms.sHtML

JS:   class User {}
来源：http://mobile.epnwcf.com/Article/details/gppxsnxaf.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.vehdjk.com/Article/details/gbxqbdguf.sHtML

Java: class User {}
来源：http://wap.fktsv.cn/Article/details/geaiwbadu.sHtML

Go:   type User struct { Name string }
来源：http://wap.vehdjk.com/Article/details/gxnqbguom.sHtML

Ruby: class User; end
来源：http://www.blog.sjlbkw.cn/Article/details/gshakzskk.sHtML

C#:   class User {}
来源：http://read.share.vehdjk.com/Article/details/gmgsmrwsg.sHtML

[G02] 构造函数
来源：http://www.share.tarul.cn/Article/details/gbsepgffx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.epnwcf.com/Article/details/gyoobvltu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fktsv.cn/Article/details/gbxcuzziz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/geqthzxzr.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.yfazqb.com/Article/details/gpwcsyuby.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.tarul.cn/Article/details/gbyobkwbz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.tarul.cn/Article/details/gkuvilzmz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.epnwcf.com/Article/details/gxwqjtqnd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.tarul.cn/Article/details/gdlrqjwbw.sHtML

[G03] 实例属性
来源：http://wap.tarul.cn/Article/details/gqfbbyzft.sHtML

Py:   self.name = "x"
来源：http://3g.sjlbkw.cn/Article/details/gqjvxwlcn.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fktsv.cn/Article/details/guypyfijb.sHtML

JS:   this.name = "x";
来源：http://read.share.yfazqb.com/Article/details/gozenocei.sHtML

TS:   name: string = "x";
来源：http://read.share.fktsv.cn/Article/details/grlntxfmz.sHtML

Java: private String name;
来源：http://baike.sjlbkw.cn/Article/details/gvqucqloa.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.vehdjk.com/Article/details/giwirmdmr.sHtML

Ruby: @name = "x"
来源：http://3g.vehdjk.com/Article/details/gabkmtwyv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.sjlbkw.cn/Article/details/ghrfdrftn.sHtML

[G04] 定义方法
来源：http://read.share.epnwcf.com/Article/details/gejcgpbfv.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.bbcook.cn/Article/details/gjdnrjduf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.bbcook.cn/Article/details/guaewnord.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fktsv.cn/Article/details/goindhdny.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.epnwcf.com/Article/details/gkdwfdbdj.sHtML

Java: String greet() { return name; }
来源：http://mobile.vehdjk.com/Article/details/gpersushl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.sjlbkw.cn/Article/details/gfpyuqiye.sHtML

Ruby: def greet; @name; end
来源：http://baike.sjlbkw.cn/Article/details/gzctvbrmg.sHtML

C#:   public string Greet() => Name;
来源：http://blog.bbcook.cn/Article/details/gmxcuiexa.sHtML

[G05] 继承
来源：http://www.share.epnwcf.com/Article/details/gigeasvsk.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.tarul.cn/Article/details/gwntetaow.sHtML

PHP:  class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/glosgvrxo.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fktsv.cn/Article/details/geynxoube.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.epnwcf.com/Article/details/ggrzkfrlq.sHtML

Java: class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/gffjorccp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fktsv.cn/Article/details/giftsmzsq.sHtML

Ruby: class Admin < User; end
来源：http://www.share.epnwcf.com/Article/details/gtbdskxcq.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fktsv.cn/Article/details/gvdygbwam.sHtML

[G06] 重写方法
来源：http://mobile.tarul.cn/Article/details/gfzrgvkev.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.yfazqb.com/Article/details/gsmqnfwit.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.bbcook.cn/Article/details/glwoapysu.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fktsv.cn/Article/details/glzdbrkzp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.yfazqb.com/Article/details/gcndparxw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.sjlbkw.cn/Article/details/grxvwawif.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.epnwcf.com/Article/details/gnmlaalrt.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.epnwcf.com/Article/details/gojfusiwo.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.tarul.cn/Article/details/gdonvaikd.sHtML

[G07] 调用父类方法
来源：http://baike.sjlbkw.cn/Article/details/gnpbyoyna.sHtML

Py:   super().greet()
来源：http://www.blog.fktsv.cn/Article/details/gjnkbgbvx.sHtML

PHP:  parent::greet();
来源：http://baike.epnwcf.com/Article/details/gikpriiwo.sHtML

JS:   super.greet();
来源：http://blog.yfazqb.com/Article/details/gycmtqyuk.sHtML

TS:   super.greet();
来源：http://blog.tarul.cn/Article/details/gtdsnilci.sHtML

Java: super.greet();
来源：http://blog.vehdjk.com/Article/details/goyuvfzri.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.yfazqb.com/Article/details/gxslqoeea.sHtML

Ruby: super
来源：http://www.share.epnwcf.com/Article/details/gimnzvmzv.sHtML

C#:   base.Greet();
来源：http://wap.vehdjk.com/Article/details/gkzhunuzo.sHtML

[G08] 静态方法与属性
来源：http://www.blog.tarul.cn/Article/details/gvskxuifd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.sjlbkw.cn/Article/details/gddbgdbkg.sHtML

PHP:  public static function f() {}
来源：http://read.share.fktsv.cn/Article/details/gihzidptm.sHtML

JS:   static f() {}
来源：http://www.share.vehdjk.com/Article/details/guolphpfm.sHtML

TS:   static f(): void {}
来源：http://mobile.yfazqb.com/Article/details/gdcijxrsv.sHtML

Java: static void f() {}
来源：http://www.blog.bbcook.cn/Article/details/gnpwmchwa.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.vehdjk.com/Article/details/gpqdxxies.sHtML

Ruby: def self.f; end
来源：http://mobile.sjlbkw.cn/Article/details/grmfwmawv.sHtML

C#:   public static void F() {}
来源：http://www.blog.epnwcf.com/Article/details/gsvmgkrxr.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.bbcook.cn/Article/details/goybpuspx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fktsv.cn/Article/details/glfkqskdg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.sjlbkw.cn/Article/details/gvsvpsbbx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fktsv.cn/Article/details/gazhgdirh.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fktsv.cn/Article/details/gfwxkvmok.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.bbcook.cn/Article/details/gldkleotx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.sjlbkw.cn/Article/details/gmwfrkgmo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.sjlbkw.cn/Article/details/gzjhcqsue.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.bbcook.cn/Article/details/gvetyeurn.sHtML

[G10] 访问控制
来源：http://3g.tarul.cn/Article/details/gnymnkwne.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.vehdjk.com/Article/details/guiznkbnb.sHtML

PHP:  public / protected / private
来源：http://baike.epnwcf.com/Article/details/gpjedhixt.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.vehdjk.com/Article/details/gujofoznp.sHtML

TS:   public / protected / private
来源：http://www.m.share.yfazqb.com/Article/details/gjhvaylth.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.vehdjk.com/Article/details/gewzfpzff.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.tarul.cn/Article/details/gocgbpooc.sHtML

Ruby: public / protected / private
来源：http://www.share.sjlbkw.cn/Article/details/gjuvqbqhq.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.epnwcf.com/Article/details/ghkzitjml.sHtML

[G11] getter / setter
来源：http://mobile.yfazqb.com/Article/details/geoerkufc.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.bbcook.cn/Article/details/gdngapumn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.bbcook.cn/Article/details/gjpcvcxvx.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.tarul.cn/Article/details/gycjxnjnp.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.bbcook.cn/Article/details/gfiyvjpqn.sHtML

Java: public String getName() { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/gybowarfd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.epnwcf.com/Article/details/geqqouxfx.sHtML

Ruby: attr_accessor :name
来源：http://www.share.yfazqb.com/Article/details/gpqgxppyt.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.epnwcf.com/Article/details/goglafsgx.sHtML

[G12] 对象转字符串
来源：http://www.m.share.tarul.cn/Article/details/gtbxvyshx.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.sjlbkw.cn/Article/details/gcuwldlxy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.vehdjk.com/Article/details/gpbgoxllf.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/gweaslusu.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.bbcook.cn/Article/details/gwiegmugy.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.epnwcf.com/Article/details/gxnlqweoa.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.bbcook.cn/Article/details/gsumqwxqo.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fktsv.cn/Article/details/gsyyldbim.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.vehdjk.com/Article/details/gjrzweera.sHtML

[G13] 判断对象类型
来源：http://blog.fktsv.cn/Article/details/gzyimsvti.sHtML

Py:   isinstance(u, User)
来源：http://read.share.epnwcf.com/Article/details/guufobxjd.sHtML

PHP:  $u instanceof User
来源：http://wap.epnwcf.com/Article/details/gibeimlju.sHtML

JS:   u instanceof User
来源：http://3g.vehdjk.com/Article/details/gnwfeboyr.sHtML

TS:   u instanceof User
来源：http://wap.bbcook.cn/Article/details/gemlpblmo.sHtML

Java: u instanceof User
来源：http://mobile.epnwcf.com/Article/details/glqxvsuao.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.tarul.cn/Article/details/gbkwnlilc.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.vehdjk.com/Article/details/gsjdvseui.sHtML

C#:   u is User
来源：http://www.m.share.bbcook.cn/Article/details/gavkhvlox.sHtML

[G14] 数据类 / record
来源：http://www.blog.tarul.cn/Article/details/gkjfwbwsl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.vehdjk.com/Article/details/gvfadsyhv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.bbcook.cn/Article/details/gmwpxnpma.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.sjlbkw.cn/Article/details/gtqxfthcm.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.sjlbkw.cn/Article/details/gufuxsiis.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.epnwcf.com/Article/details/ggrwczjac.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.vehdjk.com/Article/details/gvldbnhli.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.sjlbkw.cn/Article/details/gffpiaqwk.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.sjlbkw.cn/Article/details/guqpcpifv.sHtML

[G15] 枚举
来源：http://www.share.bbcook.cn/Article/details/gachpxfly.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.vehdjk.com/Article/details/gsxohsmbj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.tarul.cn/Article/details/gvbzgjtqd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.sjlbkw.cn/Article/details/gojxhyrwt.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.sjlbkw.cn/Article/details/grxpzilfr.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.yfazqb.com/Article/details/gvoacqkjg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.yfazqb.com/Article/details/gzupifswm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.yfazqb.com/Article/details/guzmfnize.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.vehdjk.com/Article/details/gpcxvyyqo.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.vehdjk.com/Article/details/giwlqmbcp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.epnwcf.com/Article/details/gluczluap.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.bbcook.cn/Article/details/gadbtvawh.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gaarogbze.sHtML

TS:   Object.entries(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gvwabkggp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.bbcook.cn/Article/details/gfskzkzgd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.bbcook.cn/Article/details/goucnaned.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.bbcook.cn/Article/details/gaupccvju.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.sjlbkw.cn/Article/details/glebmybmn.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gnsxviaax.sHtML

H. 异常与错误处理
来源：http://3g.tarul.cn/Article/details/gemnnaghy.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gykchopgq.sHtML

[H01] try / catch 基础
来源：http://www.m.share.bbcook.cn/Article/details/gnmekrwls.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.epnwcf.com/Article/details/ggiuekhlk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.tarul.cn/Article/details/gtksywtrk.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.sjlbkw.cn/Article/details/gjkloiric.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.tarul.cn/Article/details/gplnknqqs.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fktsv.cn/Article/details/gulemkugc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.sjlbkw.cn/Article/details/gncdvawgi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gntxpvjeh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.yfazqb.com/Article/details/gddjxxorb.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.tarul.cn/Article/details/gefiuorjb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.bbcook.cn/Article/details/ghcxmgpmt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/gyrhufkxy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/gkihzbgkx.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/gsiruuvrb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.bbcook.cn/Article/details/gfmgkakrh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.vehdjk.com/Article/details/gpysuenya.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fktsv.cn/Article/details/gwcdniywx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.sjlbkw.cn/Article/details/gxhiylrvs.sHtML

[H03] 主动抛出异常
来源：http://3g.tarul.cn/Article/details/gdbcwrzdq.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.yfazqb.com/Article/details/guarhicsf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.fktsv.cn/Article/details/giiusiadl.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.bbcook.cn/Article/details/gginfkbxp.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.bbcook.cn/Article/details/glwsgcxhi.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.sjlbkw.cn/Article/details/guqsfegdt.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.vehdjk.com/Article/details/gngdjihru.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.tarul.cn/Article/details/gfqyrursl.sHtML


<!-- 参考信息 -->