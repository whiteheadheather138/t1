代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.vehdjk.com/Article/details/gbiufnlaw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.yfazqb.com/Article/details/gccdyozxf.sHtML

TS:   if (s === "") {}
来源：http://mobile.tarul.cn/Article/details/gzlzmtafu.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.vehdjk.com/Article/details/gkkeyzxaj.sHtML

Go:   if s == "" {}
来源：http://3g.epnwcf.com/Article/details/gsvqjjxyu.sHtML

Ruby: if s.empty?
来源：http://www.m.share.yfazqb.com/Article/details/gqcpmjojb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.vehdjk.com/Article/details/gtkmemqpa.sHtML

[E21] 超长截断加省略号
来源：http://blog.sjlbkw.cn/Article/details/ggwbvtiuy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.bbcook.cn/Article/details/gywjirxpv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.tarul.cn/Article/details/gfylfjhbe.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.tarul.cn/Article/details/gcpcvsvay.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fktsv.cn/Article/details/goyqopmrg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/giavxxhnt.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.vehdjk.com/Article/details/gbqautxkf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/gpdiyxyau.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.bbcook.cn/Article/details/gerwbsopc.sHtML

[E22] 字节长度与字符长度
来源：http://3g.yfazqb.com/Article/details/gbsjmhcju.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.epnwcf.com/Article/details/gxfsjtity.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.bbcook.cn/Article/details/geveuyviq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.yfazqb.com/Article/details/gxnndwcuz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.bbcook.cn/Article/details/glrkqgilz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.bbcook.cn/Article/details/gxddgrxas.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fktsv.cn/Article/details/grtexyqxd.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.vehdjk.com/Article/details/gkdtimtqy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.tarul.cn/Article/details/gnzkrtxho.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gwylsjbke.sHtML

F. 文件与目录
来源：http://mobile.fktsv.cn/Article/details/gkvezqeww.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gqfizllnf.sHtML

[F01] 读取整个文件
来源：http://wap.tarul.cn/Article/details/gsqedjjwo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.yfazqb.com/Article/details/glvqsxovs.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gvijqdeeg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fktsv.cn/Article/details/gnjpqstad.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.vehdjk.com/Article/details/gwdyhfwal.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.vehdjk.com/Article/details/gwiaodksj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.bbcook.cn/Article/details/gjhtjydag.sHtML

Ruby: File.read("a.txt")
来源：http://3g.vehdjk.com/Article/details/grmugowqn.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gpezrbosg.sHtML

[F02] 逐行读取文件
来源：http://www.share.yfazqb.com/Article/details/gwdfwylgf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.yfazqb.com/Article/details/gjawgwwvb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.epnwcf.com/Article/details/gzrddrdod.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.vehdjk.com/Article/details/gxpyqanlk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.yfazqb.com/Article/details/gnzxxcqei.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.yfazqb.com/Article/details/gvmtogwgl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fktsv.cn/Article/details/gsrghkxfn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.tarul.cn/Article/details/gpnisjqbk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.bbcook.cn/Article/details/gvvksbjei.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.vehdjk.com/Article/details/gcpmbmeml.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.epnwcf.com/Article/details/glsynviri.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.vehdjk.com/Article/details/gaipghsql.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.yfazqb.com/Article/details/gjpxocjwj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.sjlbkw.cn/Article/details/gpychrpuv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fktsv.cn/Article/details/ghpgcknat.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.tarul.cn/Article/details/gackgqxev.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.sjlbkw.cn/Article/details/gmflhyvev.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.yfazqb.com/Article/details/gvrfdjycd.sHtML

[F04] 追加写入文件
来源：http://3g.bbcook.cn/Article/details/gojotzpnf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.tarul.cn/Article/details/gkkvddroz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.yfazqb.com/Article/details/gpewjosui.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fktsv.cn/Article/details/gfvvgkqjf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.bbcook.cn/Article/details/gtrrmaisk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.yfazqb.com/Article/details/gxwzdbovh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.sjlbkw.cn/Article/details/gicgkdbeq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.yfazqb.com/Article/details/ghcnuhaqp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.bbcook.cn/Article/details/gqxyyhdrh.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.bbcook.cn/Article/details/gzcoiaxmn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.yfazqb.com/Article/details/gkmwiawki.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/grsqlakro.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gldvuicmo.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gydesqtou.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fktsv.cn/Article/details/gtiyggczz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.bbcook.cn/Article/details/goqxxunua.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.tarul.cn/Article/details/ginrylagu.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gmyawaadu.sHtML

[F06] 删除文件
来源：http://3g.bbcook.cn/Article/details/glklirnrl.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fktsv.cn/Article/details/gforqwgaa.sHtML

PHP:  unlink("a.txt");
来源：http://blog.epnwcf.com/Article/details/ggcheeoqa.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gtmxrybyb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/giflqodkq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.vehdjk.com/Article/details/gmbrrvbxg.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gcrrhiqrk.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gmivumuct.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.tarul.cn/Article/details/gbnuxyyvl.sHtML

[F07] 创建目录（含多级）
来源：http://wap.vehdjk.com/Article/details/ghdwgwziw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.tarul.cn/Article/details/gsrjhwtiw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.yfazqb.com/Article/details/gnbmmstxw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.bbcook.cn/Article/details/gfmczxgvy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.yfazqb.com/Article/details/gtegevmuw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.sjlbkw.cn/Article/details/gbqndzmfo.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.yfazqb.com/Article/details/gidcgcgqq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.sjlbkw.cn/Article/details/gkskdmumx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fktsv.cn/Article/details/gklgktaia.sHtML

[F08] 遍历目录
来源：http://blog.yfazqb.com/Article/details/gbjtisvul.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.epnwcf.com/Article/details/gfczbywgk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fktsv.cn/Article/details/gfscxrnas.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.tarul.cn/Article/details/gchdgaxqk.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fktsv.cn/Article/details/gcjtglsnj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fktsv.cn/Article/details/gyvosuola.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.bbcook.cn/Article/details/gctlmcpyz.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.vehdjk.com/Article/details/gwpozqsqz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.sjlbkw.cn/Article/details/ggnllchbt.sHtML

[F09] 获取文件大小
来源：http://www.blog.bbcook.cn/Article/details/gtkrnonbb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gzkcuzjsf.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gbndeoqll.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.epnwcf.com/Article/details/gxyalrhlg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.vehdjk.com/Article/details/gmwwqfwaf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.tarul.cn/Article/details/ghbdbynrk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fktsv.cn/Article/details/gfwlzbyko.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gsoodzwgf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fktsv.cn/Article/details/grrqsuojd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fktsv.cn/Article/details/gmezqgoiu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/grrtlzfvs.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fktsv.cn/Article/details/gwnwstmxr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/gckxlazqf.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.tarul.cn/Article/details/gnbmgosip.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.vehdjk.com/Article/details/gfyofcvhd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/galzhafnr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.vehdjk.com/Article/details/gohbjetvu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/gztgqfxuf.sHtML

[F11] 复制与移动文件
来源：http://3g.fktsv.cn/Article/details/gmskjwikp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/geuzsrcxv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.bbcook.cn/Article/details/gdabhvije.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.tarul.cn/Article/details/ggdcauqsj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.vehdjk.com/Article/details/ggnhwwufc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.sjlbkw.cn/Article/details/gwqmifjcx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fktsv.cn/Article/details/gdotduany.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.tarul.cn/Article/details/gsirsuwln.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.bbcook.cn/Article/details/ghoyovnjg.sHtML

[F12] CSV 读写
来源：http://blog.vehdjk.com/Article/details/gdxcuybhw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.yfazqb.com/Article/details/gprbmtozh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.epnwcf.com/Article/details/gcahfavyq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.vehdjk.com/Article/details/gwnyvfigy.sHtML

TS:   // 同上
来源：http://wap.bbcook.cn/Article/details/gkdexutll.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.tarul.cn/Article/details/giqgwvwbv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fktsv.cn/Article/details/gautvoofq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.yfazqb.com/Article/details/gtldvufbl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fktsv.cn/Article/details/gaalmcxge.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/grnbbgwuq.sHtML

G. 面向对象
来源：http://blog.epnwcf.com/Article/details/girlcwstz.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gyuugqnfs.sHtML

[G01] 定义类
来源：http://www.share.sjlbkw.cn/Article/details/goxnokpgz.sHtML

Py:   class User: pass
来源：http://m.share.tarul.cn/Article/details/ghewlnppd.sHtML

PHP:  class User {}
来源：http://m.share.fktsv.cn/Article/details/gutgetllu.sHtML

JS:   class User {}
来源：http://www.m.share.fktsv.cn/Article/details/gkopxggsa.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.tarul.cn/Article/details/gjorcpfod.sHtML

Java: class User {}
来源：http://blog.tarul.cn/Article/details/gwwdhbcme.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.vehdjk.com/Article/details/gkjfvdrui.sHtML

Ruby: class User; end
来源：http://www.share.epnwcf.com/Article/details/gcjzilamn.sHtML

C#:   class User {}
来源：http://blog.sjlbkw.cn/Article/details/gtnaewrpl.sHtML

[G02] 构造函数
来源：http://blog.sjlbkw.cn/Article/details/gjxzloxtc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fktsv.cn/Article/details/goelxcbro.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.bbcook.cn/Article/details/gwqdrramt.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.bbcook.cn/Article/details/gocsojhuk.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.yfazqb.com/Article/details/gulohjqpt.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.sjlbkw.cn/Article/details/grxikltfn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.sjlbkw.cn/Article/details/glgzndiib.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.tarul.cn/Article/details/grahwnjuc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.tarul.cn/Article/details/gqwdgkehq.sHtML

[G03] 实例属性
来源：http://wap.bbcook.cn/Article/details/gaoainqhz.sHtML

Py:   self.name = "x"
来源：http://www.m.share.tarul.cn/Article/details/gmoopgdml.sHtML

PHP:  public string $name = "x";
来源：http://m.share.bbcook.cn/Article/details/ghafqevhw.sHtML

JS:   this.name = "x";
来源：http://3g.yfazqb.com/Article/details/gvztsvvcc.sHtML

TS:   name: string = "x";
来源：http://read.share.vehdjk.com/Article/details/gqyifrkpa.sHtML

Java: private String name;
来源：http://baike.fktsv.cn/Article/details/growtbalo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.bbcook.cn/Article/details/goufbiwsx.sHtML

Ruby: @name = "x"
来源：http://blog.fktsv.cn/Article/details/glcqjefzh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.bbcook.cn/Article/details/gqahczqur.sHtML

[G04] 定义方法
来源：http://www.m.share.fktsv.cn/Article/details/gucdecuat.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.yfazqb.com/Article/details/gylfuyxbj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.tarul.cn/Article/details/gvbyvtdnl.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.epnwcf.com/Article/details/gtpihqllf.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fktsv.cn/Article/details/gsmahmcej.sHtML

Java: String greet() { return name; }
来源：http://baike.vehdjk.com/Article/details/gfnosuznr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.bbcook.cn/Article/details/gypwnamwv.sHtML

Ruby: def greet; @name; end
来源：http://baike.sjlbkw.cn/Article/details/gdtxznrnz.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.epnwcf.com/Article/details/gnpilvyfv.sHtML

[G05] 继承
来源：http://baike.fktsv.cn/Article/details/gvzfknsju.sHtML

Py:   class Admin(User): pass
来源：http://read.share.yfazqb.com/Article/details/giulvvyzm.sHtML

PHP:  class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/gzpndocvb.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/gaxdplfyp.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.vehdjk.com/Article/details/ghismchro.sHtML

Java: class Admin extends User {}
来源：http://wap.vehdjk.com/Article/details/gcrxlhlxv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.bbcook.cn/Article/details/gljajpqsg.sHtML

Ruby: class Admin < User; end
来源：http://m.share.epnwcf.com/Article/details/gluowwoej.sHtML

C#:   class Admin : User {}
来源：http://www.blog.epnwcf.com/Article/details/gototvtoo.sHtML

[G06] 重写方法
来源：http://www.blog.vehdjk.com/Article/details/gzhwooffv.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.epnwcf.com/Article/details/gmikouyqt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/grjwxtpwn.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.bbcook.cn/Article/details/gckgffxnl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.yfazqb.com/Article/details/gqvvmbkej.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.epnwcf.com/Article/details/ggoobrgod.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.sjlbkw.cn/Article/details/gmfnsvhfb.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.sjlbkw.cn/Article/details/gqjbbojfl.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.yfazqb.com/Article/details/gqoluytfh.sHtML

[G07] 调用父类方法
来源：http://3g.yfazqb.com/Article/details/gezquvswm.sHtML

Py:   super().greet()
来源：http://read.share.fktsv.cn/Article/details/gqtvgowfq.sHtML

PHP:  parent::greet();
来源：http://baike.sjlbkw.cn/Article/details/goszuhblw.sHtML

JS:   super.greet();
来源：http://m.share.bbcook.cn/Article/details/ggovgikhz.sHtML

TS:   super.greet();
来源：http://mobile.tarul.cn/Article/details/gikgvbqtq.sHtML

Java: super.greet();
来源：http://www.share.fktsv.cn/Article/details/gsoffdptk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.bbcook.cn/Article/details/gxpipbrut.sHtML

Ruby: super
来源：http://mobile.epnwcf.com/Article/details/gezxzdkit.sHtML

C#:   base.Greet();
来源：http://www.m.share.fktsv.cn/Article/details/gpewuikaw.sHtML

[G08] 静态方法与属性
来源：http://mobile.sjlbkw.cn/Article/details/guvocniaj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.vehdjk.com/Article/details/gpmumymbz.sHtML

PHP:  public static function f() {}
来源：http://blog.bbcook.cn/Article/details/gpnvczjvk.sHtML

JS:   static f() {}
来源：http://m.share.bbcook.cn/Article/details/ghgdfcvlr.sHtML

TS:   static f(): void {}
来源：http://baike.fktsv.cn/Article/details/gfyjnurwr.sHtML

Java: static void f() {}
来源：http://mobile.yfazqb.com/Article/details/gqyyocamo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.bbcook.cn/Article/details/gotmljlpk.sHtML

Ruby: def self.f; end
来源：http://www.m.share.bbcook.cn/Article/details/guolfqenu.sHtML

C#:   public static void F() {}
来源：http://www.m.share.sjlbkw.cn/Article/details/ginaavamr.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.bbcook.cn/Article/details/gdlkxuyhv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.vehdjk.com/Article/details/gdzxxufbk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.epnwcf.com/Article/details/geqfdqfhi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.yfazqb.com/Article/details/gwjbzsaom.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.yfazqb.com/Article/details/guokjaknm.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.epnwcf.com/Article/details/gvabbgqhe.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.epnwcf.com/Article/details/gfegrkwtp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.tarul.cn/Article/details/gscyceikh.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fktsv.cn/Article/details/gvduksosb.sHtML

[G10] 访问控制
来源：http://3g.bbcook.cn/Article/details/gjslxvlmt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.vehdjk.com/Article/details/gjcwdpskd.sHtML

PHP:  public / protected / private
来源：http://www.share.tarul.cn/Article/details/gvybhitck.sHtML

JS:   #private 字段；其余公开
来源：http://blog.yfazqb.com/Article/details/gzkjicanw.sHtML

TS:   public / protected / private
来源：http://mobile.sjlbkw.cn/Article/details/gitaxxayo.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.yfazqb.com/Article/details/gvgtsnwje.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.tarul.cn/Article/details/gvltyxban.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fktsv.cn/Article/details/gnqvdzgks.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.bbcook.cn/Article/details/gniqvatmz.sHtML

[G11] getter / setter
来源：http://www.share.fktsv.cn/Article/details/gwviyhold.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fktsv.cn/Article/details/gedfbnfbj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.epnwcf.com/Article/details/geydpdilq.sHtML

JS:   get name() { return this._name; }
来源：http://wap.vehdjk.com/Article/details/gpaqxfixr.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.sjlbkw.cn/Article/details/gbaxfvvyk.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gsguwdwrl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.yfazqb.com/Article/details/gwrjbbwzu.sHtML

Ruby: attr_accessor :name
来源：http://read.share.yfazqb.com/Article/details/gklyxqmww.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fktsv.cn/Article/details/gtaffrcgc.sHtML

[G12] 对象转字符串
来源：http://3g.epnwcf.com/Article/details/gpakfjfkp.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.tarul.cn/Article/details/getaxjddu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.yfazqb.com/Article/details/gyoybqigr.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.yfazqb.com/Article/details/gplfeaciu.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fktsv.cn/Article/details/gahnofuko.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fktsv.cn/Article/details/gcuvphqhd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.yfazqb.com/Article/details/gisxrlpfl.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fktsv.cn/Article/details/gtdjcnszz.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fktsv.cn/Article/details/gvfqjlvcz.sHtML

[G13] 判断对象类型
来源：http://3g.tarul.cn/Article/details/ghcbfdvud.sHtML

Py:   isinstance(u, User)
来源：http://wap.yfazqb.com/Article/details/ghrsiyhha.sHtML

PHP:  $u instanceof User
来源：http://read.share.tarul.cn/Article/details/gdflrwmex.sHtML

JS:   u instanceof User
来源：http://mobile.yfazqb.com/Article/details/ghswdgeon.sHtML

TS:   u instanceof User
来源：http://www.m.share.sjlbkw.cn/Article/details/gusrpnfwg.sHtML

Java: u instanceof User
来源：http://wap.epnwcf.com/Article/details/gakjaxljp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.epnwcf.com/Article/details/gxpoopjmh.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.tarul.cn/Article/details/gcbxlkxwj.sHtML

C#:   u is User
来源：http://m.share.epnwcf.com/Article/details/gjuqsylal.sHtML

[G14] 数据类 / record
来源：http://www.m.share.sjlbkw.cn/Article/details/gowndwnlz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.sjlbkw.cn/Article/details/ghzblrcob.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.yfazqb.com/Article/details/gcebeagfr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.vehdjk.com/Article/details/geipbkrtp.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.vehdjk.com/Article/details/gefckxhar.sHtML

Java: record User(String name, int age) {}
来源：http://wap.yfazqb.com/Article/details/gesqursyl.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.bbcook.cn/Article/details/gklvyzxrx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.yfazqb.com/Article/details/gztayduhy.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fktsv.cn/Article/details/gubulxpfz.sHtML

[G15] 枚举
来源：http://mobile.fktsv.cn/Article/details/gzoediefm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.epnwcf.com/Article/details/gstyygxym.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fktsv.cn/Article/details/glwxphvgs.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.yfazqb.com/Article/details/gzrseiilr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.vehdjk.com/Article/details/gelmmpewi.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.epnwcf.com/Article/details/ggasbvlow.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.yfazqb.com/Article/details/gmlnzqyha.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fktsv.cn/Article/details/gnaeelray.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fktsv.cn/Article/details/gctqilspf.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.fktsv.cn/Article/details/gfxfuvlay.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.yfazqb.com/Article/details/gpcvejhnm.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fktsv.cn/Article/details/gwnmyhrtc.sHtML

JS:   Object.entries(obj)
来源：http://baike.epnwcf.com/Article/details/gkpwrinxk.sHtML

TS:   Object.entries(obj)
来源：http://m.share.tarul.cn/Article/details/gorpoqsuz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fktsv.cn/Article/details/ggertknaa.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.yfazqb.com/Article/details/gxwkxiuee.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.vehdjk.com/Article/details/giwwyuuet.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.epnwcf.com/Article/details/gddwxhkap.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gkinofuyo.sHtML

H. 异常与错误处理
来源：http://3g.epnwcf.com/Article/details/gfewoqrpk.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gkpylyzdv.sHtML

[H01] try / catch 基础
来源：http://m.share.vehdjk.com/Article/details/gnzersbyj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.vehdjk.com/Article/details/goudttavq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.tarul.cn/Article/details/gkeihjwwh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.epnwcf.com/Article/details/gbrtwllpl.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.sjlbkw.cn/Article/details/gwdtrghey.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.tarul.cn/Article/details/gfgkgvrni.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.vehdjk.com/Article/details/gbtgbbvhb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.yfazqb.com/Article/details/gjqscyaqe.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.vehdjk.com/Article/details/gmhdwrbkt.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.bbcook.cn/Article/details/gcpaqzndy.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.sjlbkw.cn/Article/details/ggjodyksa.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggbraehth.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fktsv.cn/Article/details/gpvygcgdk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/geodameyp.sHtML


<!-- 参考信息 -->