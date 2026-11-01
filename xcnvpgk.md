代发 wailian999

Ruby: s.lines
来源：http://www.m.share.bbcook.cn/Article/details/gpquzofmg.sHtML

C#:   s.Split('\n')
来源：http://baike.vehdjk.com/Article/details/gscxgjkmt.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.tarul.cn/Article/details/gzggyxblz.sHtML

Py:   if not s:
来源：http://www.m.share.bbcook.cn/Article/details/gnbhqiwkw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.yfazqb.com/Article/details/gmzepambu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fktsv.cn/Article/details/gtnitnykd.sHtML

TS:   if (s === "") {}
来源：http://m.share.yfazqb.com/Article/details/gcskbahgq.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fktsv.cn/Article/details/gkdrefpsy.sHtML

Go:   if s == "" {}
来源：http://read.share.fktsv.cn/Article/details/gbrnaefpu.sHtML

Ruby: if s.empty?
来源：http://read.share.fktsv.cn/Article/details/gttidgren.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.epnwcf.com/Article/details/gfdziiaek.sHtML

[E21] 超长截断加省略号
来源：http://www.share.vehdjk.com/Article/details/gukslzrsu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.yfazqb.com/Article/details/gnwwfnufa.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.vehdjk.com/Article/details/gkolyvdwt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.bbcook.cn/Article/details/gpetatzyr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.tarul.cn/Article/details/gcalkpdwv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.vehdjk.com/Article/details/geqcjzsbg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fktsv.cn/Article/details/gofrkooks.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.vehdjk.com/Article/details/gpxzhxvbq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.sjlbkw.cn/Article/details/gonqlyzqo.sHtML

[E22] 字节长度与字符长度
来源：http://baike.tarul.cn/Article/details/gwldjxehz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fktsv.cn/Article/details/gdsocorwi.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.tarul.cn/Article/details/gpoedrtcg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.bbcook.cn/Article/details/gkhyhxkhv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.epnwcf.com/Article/details/gwfdoecea.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.vehdjk.com/Article/details/gpwqplpne.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.sjlbkw.cn/Article/details/gcffiaabq.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.epnwcf.com/Article/details/gtmswidet.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.tarul.cn/Article/details/ghmbbrhwf.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gqqvcnszv.sHtML

F. 文件与目录
来源：http://blog.tarul.cn/Article/details/guorrxelf.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gwqamhuqn.sHtML

[F01] 读取整个文件
来源：http://www.blog.fktsv.cn/Article/details/gqwglgusl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.tarul.cn/Article/details/gelhbhtln.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.tarul.cn/Article/details/ggdqsljxm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.sjlbkw.cn/Article/details/gbbcifwfr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fktsv.cn/Article/details/ggifwqgse.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.tarul.cn/Article/details/gpjxwnlbf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.epnwcf.com/Article/details/gytaviyyg.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gedzsnvnm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.tarul.cn/Article/details/gqibvbayq.sHtML

[F02] 逐行读取文件
来源：http://3g.vehdjk.com/Article/details/ggkkvmoml.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.yfazqb.com/Article/details/gpmxtjgdk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fktsv.cn/Article/details/geruviosn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.sjlbkw.cn/Article/details/gcuqjmbol.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fktsv.cn/Article/details/gifkbrvwj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.yfazqb.com/Article/details/gzycgjxun.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.epnwcf.com/Article/details/gfaoeodqb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.bbcook.cn/Article/details/gunijkpae.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fktsv.cn/Article/details/gwgaghrwe.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.bbcook.cn/Article/details/gswigeoxt.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.tarul.cn/Article/details/gidhxayto.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.vehdjk.com/Article/details/gunztrdcu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.sjlbkw.cn/Article/details/gcfpqmfzc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.sjlbkw.cn/Article/details/gwjciraqg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fktsv.cn/Article/details/gasvjnygx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.vehdjk.com/Article/details/gcvrfmtja.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.vehdjk.com/Article/details/gnotgcwif.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.bbcook.cn/Article/details/gibpeimox.sHtML

[F04] 追加写入文件
来源：http://www.blog.bbcook.cn/Article/details/gcxbjdytk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.sjlbkw.cn/Article/details/gcxodfqzz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.bbcook.cn/Article/details/gypgnjnlh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.yfazqb.com/Article/details/glotzoxfz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.yfazqb.com/Article/details/gumflidet.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.yfazqb.com/Article/details/ghbyjcxbr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.epnwcf.com/Article/details/geobccmvb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.tarul.cn/Article/details/gpfjaigkq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.vehdjk.com/Article/details/gditablqk.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.vehdjk.com/Article/details/gzloraxma.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.tarul.cn/Article/details/goykxoylg.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fktsv.cn/Article/details/gvjglxcgk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.bbcook.cn/Article/details/glqbpwabc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqjvuatgp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.vehdjk.com/Article/details/glsvbuddk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.tarul.cn/Article/details/gwajmxfvg.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gvgtuzeyh.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gpestmjha.sHtML

[F06] 删除文件
来源：http://wap.tarul.cn/Article/details/ggpryuxxc.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fktsv.cn/Article/details/gfbdxtgrj.sHtML

PHP:  unlink("a.txt");
来源：http://blog.yfazqb.com/Article/details/gqtcsgzpp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.vehdjk.com/Article/details/gtbirkrgi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.vehdjk.com/Article/details/gratvhutl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.yfazqb.com/Article/details/gzoosdvml.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gtxazkcpi.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gbpwttorh.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.bbcook.cn/Article/details/gxfnkgkdm.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fktsv.cn/Article/details/gagdbkwpf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fktsv.cn/Article/details/gabyjjqvm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fktsv.cn/Article/details/gcbinsxqa.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.tarul.cn/Article/details/gicbgijby.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fktsv.cn/Article/details/gnjyaxgkp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.yfazqb.com/Article/details/ghmpkerkl.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fktsv.cn/Article/details/gvazyqver.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.epnwcf.com/Article/details/gihzkdxuz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.sjlbkw.cn/Article/details/gyjetvmje.sHtML

[F08] 遍历目录
来源：http://www.blog.epnwcf.com/Article/details/gffxexblk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.epnwcf.com/Article/details/gvpzltifa.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.bbcook.cn/Article/details/guimupkyw.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.epnwcf.com/Article/details/ghmmfjske.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fktsv.cn/Article/details/gukityytz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fktsv.cn/Article/details/guvwlkvqe.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.sjlbkw.cn/Article/details/gekslevmu.sHtML

Ruby: Dir.children("dir")
来源：http://3g.sjlbkw.cn/Article/details/gprynhmxe.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.vehdjk.com/Article/details/goqnabbdw.sHtML

[F09] 获取文件大小
来源：http://wap.sjlbkw.cn/Article/details/gnztenhtp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gsdirvkuc.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gpwirraxp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.yfazqb.com/Article/details/gposgrlxg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.yfazqb.com/Article/details/gusadvrar.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.tarul.cn/Article/details/gdmhtcfli.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.tarul.cn/Article/details/gsehqbmnv.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.tarul.cn/Article/details/gtfchcvud.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.vehdjk.com/Article/details/gymehzqdg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.vehdjk.com/Article/details/gfaxapyup.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.vehdjk.com/Article/details/getnoolve.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.epnwcf.com/Article/details/guenoteuj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gwijtsmbf.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fktsv.cn/Article/details/gxuglbpvv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.vehdjk.com/Article/details/gtoyzfojj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.vehdjk.com/Article/details/gyeiuopzp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.vehdjk.com/Article/details/geatbbigz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/glvqgbagq.sHtML

[F11] 复制与移动文件
来源：http://m.share.sjlbkw.cn/Article/details/gspolmcyt.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.bbcook.cn/Article/details/grzpksuyv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.tarul.cn/Article/details/gqpavmvkx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gqajkkziq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.epnwcf.com/Article/details/gobsuqdts.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fktsv.cn/Article/details/gudjdthlg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fktsv.cn/Article/details/gcbyzrzua.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gycxszovz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.vehdjk.com/Article/details/gdszsyaoy.sHtML

[F12] CSV 读写
来源：http://read.share.tarul.cn/Article/details/gwaqltddo.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.sjlbkw.cn/Article/details/gdcwkyzlj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.yfazqb.com/Article/details/gvpsfrykq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.sjlbkw.cn/Article/details/gwemultfq.sHtML

TS:   // 同上
来源：http://3g.tarul.cn/Article/details/gcxyfqvrf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.sjlbkw.cn/Article/details/gzsfpogxv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.yfazqb.com/Article/details/gxcdmuldt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.vehdjk.com/Article/details/gdjhomtcn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fktsv.cn/Article/details/grkbyatpc.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gsdbldvwi.sHtML

G. 面向对象
来源：http://www.share.bbcook.cn/Article/details/gkehhwaxq.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/glnlcqqqs.sHtML

[G01] 定义类
来源：http://mobile.bbcook.cn/Article/details/gjtyzzgfi.sHtML

Py:   class User: pass
来源：http://wap.tarul.cn/Article/details/gnytklurj.sHtML

PHP:  class User {}
来源：http://baike.vehdjk.com/Article/details/gcihqjnek.sHtML

JS:   class User {}
来源：http://www.share.fktsv.cn/Article/details/gkhuffanf.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.vehdjk.com/Article/details/gyszbophx.sHtML

Java: class User {}
来源：http://read.share.fktsv.cn/Article/details/gsrwcnedr.sHtML

Go:   type User struct { Name string }
来源：http://blog.bbcook.cn/Article/details/gbpbmubcj.sHtML

Ruby: class User; end
来源：http://3g.sjlbkw.cn/Article/details/gelrwwmny.sHtML

C#:   class User {}
来源：http://3g.sjlbkw.cn/Article/details/gjnxuepig.sHtML

[G02] 构造函数
来源：http://wap.epnwcf.com/Article/details/ggafrhkgr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.sjlbkw.cn/Article/details/gfhglnuhs.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.tarul.cn/Article/details/gbrlbfkgi.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.epnwcf.com/Article/details/guovodnnf.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fktsv.cn/Article/details/gqbwfviwk.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fktsv.cn/Article/details/gtcvhirkw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.tarul.cn/Article/details/gadjgylac.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.vehdjk.com/Article/details/gftirhcbg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.sjlbkw.cn/Article/details/gpdvizbkk.sHtML

[G03] 实例属性
来源：http://3g.bbcook.cn/Article/details/gprdvjzeg.sHtML

Py:   self.name = "x"
来源：http://baike.tarul.cn/Article/details/gtrugemae.sHtML

PHP:  public string $name = "x";
来源：http://read.share.yfazqb.com/Article/details/gyblwzvtb.sHtML

JS:   this.name = "x";
来源：http://wap.epnwcf.com/Article/details/goeqpzvyj.sHtML

TS:   name: string = "x";
来源：http://wap.epnwcf.com/Article/details/gngwieyav.sHtML

Java: private String name;
来源：http://www.share.epnwcf.com/Article/details/gvpfineao.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.vehdjk.com/Article/details/gqepwsiav.sHtML

Ruby: @name = "x"
来源：http://read.share.epnwcf.com/Article/details/gnkhbxbpa.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.yfazqb.com/Article/details/girqdhvbf.sHtML

[G04] 定义方法
来源：http://read.share.bbcook.cn/Article/details/grhnvzmcr.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.epnwcf.com/Article/details/gzdgrtfrn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.sjlbkw.cn/Article/details/gtxmhcuxh.sHtML

JS:   greet() { return this.name; }
来源：http://baike.tarul.cn/Article/details/gfvtptivo.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.bbcook.cn/Article/details/gxleeisaq.sHtML

Java: String greet() { return name; }
来源：http://3g.fktsv.cn/Article/details/gyfhowvyf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.yfazqb.com/Article/details/gcuitkmeg.sHtML

Ruby: def greet; @name; end
来源：http://read.share.bbcook.cn/Article/details/gbsjlmvki.sHtML

C#:   public string Greet() => Name;
来源：http://blog.yfazqb.com/Article/details/ghukepgix.sHtML

[G05] 继承
来源：http://read.share.bbcook.cn/Article/details/gpzkldhha.sHtML

Py:   class Admin(User): pass
来源：http://mobile.bbcook.cn/Article/details/gnfkveihr.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.sjlbkw.cn/Article/details/gzixnfxju.sHtML

JS:   class Admin extends User {}
来源：http://baike.tarul.cn/Article/details/gipgxbjpd.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.epnwcf.com/Article/details/gmnwhyioe.sHtML

Java: class Admin extends User {}
来源：http://mobile.sjlbkw.cn/Article/details/gnxrfrhgp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.bbcook.cn/Article/details/gmrrbdkdc.sHtML

Ruby: class Admin < User; end
来源：http://m.share.epnwcf.com/Article/details/gnqkqbidj.sHtML

C#:   class Admin : User {}
来源：http://blog.fktsv.cn/Article/details/gzogjkczd.sHtML

[G06] 重写方法
来源：http://read.share.vehdjk.com/Article/details/gbbkfptpb.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.bbcook.cn/Article/details/gwuuhlnzz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.vehdjk.com/Article/details/gyevdofbn.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.bbcook.cn/Article/details/ghvnvcjwl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.yfazqb.com/Article/details/gagayxksg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fktsv.cn/Article/details/gbyankncn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fktsv.cn/Article/details/gntzfszld.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.vehdjk.com/Article/details/gayfudfnk.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fktsv.cn/Article/details/gycwignmp.sHtML

[G07] 调用父类方法
来源：http://www.m.share.epnwcf.com/Article/details/gnwvfbvws.sHtML

Py:   super().greet()
来源：http://baike.epnwcf.com/Article/details/goginpwpl.sHtML

PHP:  parent::greet();
来源：http://blog.vehdjk.com/Article/details/gmcdaowfb.sHtML

JS:   super.greet();
来源：http://blog.bbcook.cn/Article/details/gnlifdecp.sHtML

TS:   super.greet();
来源：http://read.share.fktsv.cn/Article/details/gzjvbwrsp.sHtML

Java: super.greet();
来源：http://mobile.fktsv.cn/Article/details/gxxdaztam.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.sjlbkw.cn/Article/details/grrrpfjqk.sHtML

Ruby: super
来源：http://www.m.share.epnwcf.com/Article/details/gbvgosgdc.sHtML

C#:   base.Greet();
来源：http://www.share.bbcook.cn/Article/details/gwsprayuu.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.sjlbkw.cn/Article/details/gcbfrwxyl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.bbcook.cn/Article/details/gdalvhxjk.sHtML

PHP:  public static function f() {}
来源：http://blog.fktsv.cn/Article/details/givoiqzow.sHtML

JS:   static f() {}
来源：http://m.share.bbcook.cn/Article/details/gxxzqfnxu.sHtML

TS:   static f(): void {}
来源：http://blog.epnwcf.com/Article/details/gqlnqnwyz.sHtML

Java: static void f() {}
来源：http://www.blog.epnwcf.com/Article/details/gzsvdyqyn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.epnwcf.com/Article/details/gugxdtwze.sHtML

Ruby: def self.f; end
来源：http://www.share.fktsv.cn/Article/details/gfbfgqxvm.sHtML

C#:   public static void F() {}
来源：http://wap.bbcook.cn/Article/details/gkfxtauwx.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.bbcook.cn/Article/details/gvrkycbpj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fktsv.cn/Article/details/gtautpnzd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.tarul.cn/Article/details/gjiidozhc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.vehdjk.com/Article/details/gkfcobnwl.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.epnwcf.com/Article/details/ghtjfvpzq.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.yfazqb.com/Article/details/geykrsdhc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.vehdjk.com/Article/details/gbtvomwgb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.bbcook.cn/Article/details/giyarsjwm.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.bbcook.cn/Article/details/gchbpuevw.sHtML

[G10] 访问控制
来源：http://www.m.share.vehdjk.com/Article/details/gzwjyvjjx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.yfazqb.com/Article/details/gxcszfosa.sHtML

PHP:  public / protected / private
来源：http://www.share.sjlbkw.cn/Article/details/gvnkzqbsy.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.vehdjk.com/Article/details/gxzyexspq.sHtML

TS:   public / protected / private
来源：http://mobile.sjlbkw.cn/Article/details/ggjrejwhl.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fktsv.cn/Article/details/gbhrhkivh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.sjlbkw.cn/Article/details/glnjrcpth.sHtML

Ruby: public / protected / private
来源：http://3g.fktsv.cn/Article/details/gabwmdntx.sHtML

C#:   public / protected / private / internal
来源：http://baike.sjlbkw.cn/Article/details/gdwcemntv.sHtML

[G11] getter / setter
来源：http://m.share.fktsv.cn/Article/details/gtsijvfgq.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.yfazqb.com/Article/details/gxcctvjfk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.sjlbkw.cn/Article/details/gdqvxaren.sHtML

JS:   get name() { return this._name; }
来源：http://blog.tarul.cn/Article/details/gdoxjuzmt.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.tarul.cn/Article/details/gfkemyxpa.sHtML

Java: public String getName() { return name; }
来源：http://3g.vehdjk.com/Article/details/gaohdzvhz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.yfazqb.com/Article/details/ghcivjbvm.sHtML

Ruby: attr_accessor :name
来源：http://wap.yfazqb.com/Article/details/geryufgcc.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fktsv.cn/Article/details/guojwvltl.sHtML

[G12] 对象转字符串
来源：http://baike.epnwcf.com/Article/details/gjaxzmydf.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.tarul.cn/Article/details/gphegbqog.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fktsv.cn/Article/details/gbfgrsila.sHtML

JS:   toString() { return this.name; }
来源：http://wap.yfazqb.com/Article/details/gktyphqky.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fktsv.cn/Article/details/gpwpyljml.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.epnwcf.com/Article/details/gejihkdri.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.epnwcf.com/Article/details/gajclokyr.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.epnwcf.com/Article/details/gwxnvwjhy.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.sjlbkw.cn/Article/details/gsupndeny.sHtML

[G13] 判断对象类型
来源：http://3g.epnwcf.com/Article/details/goswevkng.sHtML

Py:   isinstance(u, User)
来源：http://read.share.tarul.cn/Article/details/gbmbxqcrh.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.epnwcf.com/Article/details/gxlueqeby.sHtML

JS:   u instanceof User
来源：http://baike.sjlbkw.cn/Article/details/geulifdzs.sHtML

TS:   u instanceof User
来源：http://blog.bbcook.cn/Article/details/gbfdzkmqa.sHtML

Java: u instanceof User
来源：http://m.share.tarul.cn/Article/details/gnwlirixc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.bbcook.cn/Article/details/gejarhwol.sHtML

Ruby: u.is_a?(User)
来源：http://blog.tarul.cn/Article/details/gwfnglmao.sHtML

C#:   u is User
来源：http://3g.epnwcf.com/Article/details/grxlsjhjk.sHtML

[G14] 数据类 / record
来源：http://www.m.share.yfazqb.com/Article/details/ghxqhlfyo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fktsv.cn/Article/details/gyrhuzruv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fktsv.cn/Article/details/gxbqrvalp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fktsv.cn/Article/details/gyiihzbsy.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.vehdjk.com/Article/details/gczicugtp.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.vehdjk.com/Article/details/gxffdqfgy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.sjlbkw.cn/Article/details/gfvptuadd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.epnwcf.com/Article/details/gmxboadhj.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.bbcook.cn/Article/details/gsveskzsc.sHtML

[G15] 枚举
来源：http://www.blog.yfazqb.com/Article/details/gsqafaong.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.sjlbkw.cn/Article/details/gciwukpzw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.bbcook.cn/Article/details/gkaobpmhr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.vehdjk.com/Article/details/gcuzakfzs.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.yfazqb.com/Article/details/gapwyywug.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.sjlbkw.cn/Article/details/gwagfdfml.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.sjlbkw.cn/Article/details/gylgbkiny.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.epnwcf.com/Article/details/gvtebgivj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fktsv.cn/Article/details/gspwnfnra.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fktsv.cn/Article/details/gdepaixfr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.vehdjk.com/Article/details/gblpdcxoe.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fktsv.cn/Article/details/gqqlykvzs.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggngklcua.sHtML

TS:   Object.entries(obj)
来源：http://wap.sjlbkw.cn/Article/details/gapjowuik.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.yfazqb.com/Article/details/gecutgoex.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.yfazqb.com/Article/details/gutefwxnh.sHtML

Ruby: obj.instance_variables
来源：http://m.share.epnwcf.com/Article/details/ghrhrfzpt.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.epnwcf.com/Article/details/gbkjviunn.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/grtovrzpr.sHtML

H. 异常与错误处理
来源：http://www.m.share.sjlbkw.cn/Article/details/gwjwedvfd.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gmafwcvze.sHtML

[H01] try / catch 基础
来源：http://mobile.sjlbkw.cn/Article/details/gjupdcetg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.yfazqb.com/Article/details/guqifrxeo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.sjlbkw.cn/Article/details/gwcaifing.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.epnwcf.com/Article/details/gakdxdyth.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fktsv.cn/Article/details/gaikuldxq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fktsv.cn/Article/details/girastulh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.epnwcf.com/Article/details/gptydrggj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.sjlbkw.cn/Article/details/gbkqqiswb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fktsv.cn/Article/details/gblwtvzcl.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.yfazqb.com/Article/details/gczmmbate.sHtML


<!-- 参考信息 -->