代发 wailian999

Go:   if s == "" {}
来源：http://baike.fktsv.cn/Article/details/gfoqmxpto.sHtML

Ruby: if s.empty?
来源：http://wap.fktsv.cn/Article/details/gyzpqfzee.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.yfazqb.com/Article/details/gnantdkgq.sHtML

[E21] 超长截断加省略号
来源：http://3g.fktsv.cn/Article/details/gatbgkino.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.tarul.cn/Article/details/geqadokta.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.tarul.cn/Article/details/gsinludkf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.bbcook.cn/Article/details/gvvpqkgiv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.epnwcf.com/Article/details/gglpujvrt.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/gbazdyfsy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.epnwcf.com/Article/details/gflktndtt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.yfazqb.com/Article/details/gyyyjvizn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.epnwcf.com/Article/details/gffkafgwk.sHtML

[E22] 字节长度与字符长度
来源：http://blog.bbcook.cn/Article/details/goincfowv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.vehdjk.com/Article/details/gtnjgbvdl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.yfazqb.com/Article/details/godsskjdx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.bbcook.cn/Article/details/gwkozdnyx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.vehdjk.com/Article/details/gequglsuj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.epnwcf.com/Article/details/gqspchyia.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.vehdjk.com/Article/details/gxrtuesvo.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.yfazqb.com/Article/details/gegqclmby.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.epnwcf.com/Article/details/gfrzfzodw.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gdtfqbxjf.sHtML

F. 文件与目录
来源：http://baike.vehdjk.com/Article/details/gtrhiybfn.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/ggxxzzgmt.sHtML

[F01] 读取整个文件
来源：http://mobile.yfazqb.com/Article/details/gwywznaai.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fktsv.cn/Article/details/gykdoelyw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.epnwcf.com/Article/details/ggtfjgyed.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.epnwcf.com/Article/details/gwekaodam.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.epnwcf.com/Article/details/gnplnbhdh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.vehdjk.com/Article/details/gqtnkhzvy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.vehdjk.com/Article/details/gbtueuxwd.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.tarul.cn/Article/details/gadpvxqcw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gdwdlggzj.sHtML

[F02] 逐行读取文件
来源：http://baike.tarul.cn/Article/details/gznhxtzae.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.tarul.cn/Article/details/gdoqmawzx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.sjlbkw.cn/Article/details/gjwdckkhj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fktsv.cn/Article/details/gmiumwwlu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.vehdjk.com/Article/details/gohqkqzuq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.epnwcf.com/Article/details/gfumbkyog.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.bbcook.cn/Article/details/goqrdoxtw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.sjlbkw.cn/Article/details/gkpyapqna.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.vehdjk.com/Article/details/gqtcsxvlp.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.vehdjk.com/Article/details/gffbfvgrj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.epnwcf.com/Article/details/gqpavoxbm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.sjlbkw.cn/Article/details/gqsbbjcin.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.sjlbkw.cn/Article/details/gifbcaaim.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.tarul.cn/Article/details/gyzxlxvkq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.epnwcf.com/Article/details/gruhhyebo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.epnwcf.com/Article/details/gzbxfubbt.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.sjlbkw.cn/Article/details/gnifuwynt.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.sjlbkw.cn/Article/details/guodfaysw.sHtML

[F04] 追加写入文件
来源：http://m.share.fktsv.cn/Article/details/ghagjmyua.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.yfazqb.com/Article/details/gpfksadsj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.vehdjk.com/Article/details/geyhrjnvx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.yfazqb.com/Article/details/gwfezuahe.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.sjlbkw.cn/Article/details/gsmjrzumw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.sjlbkw.cn/Article/details/ggukoupih.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.bbcook.cn/Article/details/ghmpgzuje.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.yfazqb.com/Article/details/gyyxfkmnh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.vehdjk.com/Article/details/gykdgltru.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.yfazqb.com/Article/details/guxscenif.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fktsv.cn/Article/details/gslkimrdu.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/giysatbxl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.bbcook.cn/Article/details/ggjevhttm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghjebympq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.vehdjk.com/Article/details/gihsnoaei.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.yfazqb.com/Article/details/gjprhbaks.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gkguixsvm.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gdouxmjos.sHtML

[F06] 删除文件
来源：http://mobile.yfazqb.com/Article/details/glpsinjlq.sHtML

Py:   os.remove("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gzcnoatic.sHtML

PHP:  unlink("a.txt");
来源：http://3g.bbcook.cn/Article/details/gkawokjww.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gyxhgwnhz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.vehdjk.com/Article/details/gqoylqgue.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.epnwcf.com/Article/details/gyennakgj.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gohqhacjx.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.tarul.cn/Article/details/glvlgjhfb.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gizjxldcz.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.yfazqb.com/Article/details/gxchvfhbc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.tarul.cn/Article/details/gviycsiwb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.epnwcf.com/Article/details/gurxgnazo.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.sjlbkw.cn/Article/details/guxvnywtn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.vehdjk.com/Article/details/gpqopqond.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.bbcook.cn/Article/details/gqynmycif.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.epnwcf.com/Article/details/gsvnppair.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.fktsv.cn/Article/details/gjuuqxxpi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fktsv.cn/Article/details/gerbeqlzu.sHtML

[F08] 遍历目录
来源：http://read.share.epnwcf.com/Article/details/gssdjwpda.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.tarul.cn/Article/details/gumoikwfd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmglrjayv.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.epnwcf.com/Article/details/geayrhznn.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.bbcook.cn/Article/details/gpszrliew.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.tarul.cn/Article/details/glpahmnig.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fktsv.cn/Article/details/gzlgtlcdo.sHtML

Ruby: Dir.children("dir")
来源：http://blog.tarul.cn/Article/details/gbyyumdod.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.sjlbkw.cn/Article/details/ggdaqmvip.sHtML

[F09] 获取文件大小
来源：http://mobile.sjlbkw.cn/Article/details/gbgimvkdg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gpvquvmui.sHtML

PHP:  filesize("a.txt");
来源：http://3g.yfazqb.com/Article/details/gwayshzfv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.epnwcf.com/Article/details/gsrwwgjkl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fktsv.cn/Article/details/gctoapcof.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.yfazqb.com/Article/details/gthzcohpn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.vehdjk.com/Article/details/gygqtpcjj.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fktsv.cn/Article/details/gfhnprhti.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fktsv.cn/Article/details/gozdicscl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.sjlbkw.cn/Article/details/gnzfgzavv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.bbcook.cn/Article/details/gqnroaoeg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gatqxteis.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/gyzrkbzhb.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gfkgqkqyo.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.epnwcf.com/Article/details/gclobajbj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.epnwcf.com/Article/details/gjxggordk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.bbcook.cn/Article/details/geutsczrr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/gtmeqclux.sHtML

[F11] 复制与移动文件
来源：http://m.share.tarul.cn/Article/details/genuzthqb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fktsv.cn/Article/details/gmuqjojer.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.bbcook.cn/Article/details/glhcayzsd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.sjlbkw.cn/Article/details/gcuizbpzt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fktsv.cn/Article/details/gajndzrxj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.epnwcf.com/Article/details/gpbrcspkm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.tarul.cn/Article/details/gipdrlugs.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.epnwcf.com/Article/details/gjyltquak.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.epnwcf.com/Article/details/gbivbimfv.sHtML

[F12] CSV 读写
来源：http://blog.fktsv.cn/Article/details/gvjiyjbtn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.sjlbkw.cn/Article/details/gbttfqlmi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.bbcook.cn/Article/details/gqvxlcymn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.bbcook.cn/Article/details/gczekvaqd.sHtML

TS:   // 同上
来源：http://3g.sjlbkw.cn/Article/details/gzypsmqwm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.sjlbkw.cn/Article/details/gnpadnadh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.bbcook.cn/Article/details/gksycobws.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fktsv.cn/Article/details/gasfuwatl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.sjlbkw.cn/Article/details/glojpbggy.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gswwqpfaj.sHtML

G. 面向对象
来源：http://wap.sjlbkw.cn/Article/details/garcwzpeh.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gpgxdfmvb.sHtML

[G01] 定义类
来源：http://wap.fktsv.cn/Article/details/gjbvdeofu.sHtML

Py:   class User: pass
来源：http://baike.tarul.cn/Article/details/gimswkhuy.sHtML

PHP:  class User {}
来源：http://blog.yfazqb.com/Article/details/gwboyltaa.sHtML

JS:   class User {}
来源：http://www.blog.vehdjk.com/Article/details/giphvqjxr.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.epnwcf.com/Article/details/gowdbxxsz.sHtML

Java: class User {}
来源：http://wap.vehdjk.com/Article/details/gvundkwkd.sHtML

Go:   type User struct { Name string }
来源：http://read.share.tarul.cn/Article/details/gddkoibsq.sHtML

Ruby: class User; end
来源：http://www.blog.yfazqb.com/Article/details/gqzmprmdj.sHtML

C#:   class User {}
来源：http://www.m.share.fktsv.cn/Article/details/gskrqlzhn.sHtML

[G02] 构造函数
来源：http://baike.epnwcf.com/Article/details/gpjqtflsh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.sjlbkw.cn/Article/details/gcllzdcyq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.vehdjk.com/Article/details/giopozypo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.epnwcf.com/Article/details/gqfxcercf.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fktsv.cn/Article/details/goiliyetl.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.bbcook.cn/Article/details/gygrwtpmj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fktsv.cn/Article/details/gfwtjgylv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.vehdjk.com/Article/details/gdzkmewyw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.bbcook.cn/Article/details/gkqdnbeoc.sHtML

[G03] 实例属性
来源：http://www.share.bbcook.cn/Article/details/grnxllypd.sHtML

Py:   self.name = "x"
来源：http://read.share.yfazqb.com/Article/details/goqzkimou.sHtML

PHP:  public string $name = "x";
来源：http://www.share.epnwcf.com/Article/details/gvnwyxjzs.sHtML

JS:   this.name = "x";
来源：http://3g.vehdjk.com/Article/details/gkubdyjkv.sHtML

TS:   name: string = "x";
来源：http://www.m.share.epnwcf.com/Article/details/gfjpmovyt.sHtML

Java: private String name;
来源：http://wap.tarul.cn/Article/details/gsimtddri.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.sjlbkw.cn/Article/details/gfpdgkfwa.sHtML

Ruby: @name = "x"
来源：http://www.share.sjlbkw.cn/Article/details/gvidzvqqy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.sjlbkw.cn/Article/details/gbkrkynxh.sHtML

[G04] 定义方法
来源：http://mobile.bbcook.cn/Article/details/guoftznmz.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.tarul.cn/Article/details/gdrkjgbvq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/genscfvtj.sHtML

JS:   greet() { return this.name; }
来源：http://baike.yfazqb.com/Article/details/gydvpxusu.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fktsv.cn/Article/details/gdqxfjunb.sHtML

Java: String greet() { return name; }
来源：http://blog.epnwcf.com/Article/details/gngnybwpi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.bbcook.cn/Article/details/gagdjalzo.sHtML

Ruby: def greet; @name; end
来源：http://www.share.epnwcf.com/Article/details/grlpbpvlw.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.epnwcf.com/Article/details/gcqddqcun.sHtML

[G05] 继承
来源：http://www.m.share.tarul.cn/Article/details/gavnjlgjt.sHtML

Py:   class Admin(User): pass
来源：http://mobile.epnwcf.com/Article/details/gudvehmjm.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.yfazqb.com/Article/details/gfevkzakd.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fktsv.cn/Article/details/gafunxpev.sHtML

TS:   class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/gupgcyhdx.sHtML

Java: class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/gfmxdyvkw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.yfazqb.com/Article/details/geqeczqns.sHtML

Ruby: class Admin < User; end
来源：http://wap.fktsv.cn/Article/details/gfamuunrn.sHtML

C#:   class Admin : User {}
来源：http://mobile.bbcook.cn/Article/details/gtygbackt.sHtML

[G06] 重写方法
来源：http://www.share.tarul.cn/Article/details/gpwwotwtj.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.yfazqb.com/Article/details/gklpfnafp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.yfazqb.com/Article/details/gzyicybpw.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fktsv.cn/Article/details/gnslomdzu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.epnwcf.com/Article/details/gihyyhqcy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.tarul.cn/Article/details/gzwgupcza.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.tarul.cn/Article/details/gybzidozw.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.sjlbkw.cn/Article/details/gluehtvps.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.yfazqb.com/Article/details/geyxeiktg.sHtML

[G07] 调用父类方法
来源：http://wap.fktsv.cn/Article/details/gwdptagil.sHtML

Py:   super().greet()
来源：http://m.share.fktsv.cn/Article/details/gtqlfqavo.sHtML

PHP:  parent::greet();
来源：http://read.share.bbcook.cn/Article/details/gumfuvnde.sHtML

JS:   super.greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gvbwsdpiw.sHtML

TS:   super.greet();
来源：http://www.m.share.tarul.cn/Article/details/gvcuzzhjk.sHtML

Java: super.greet();
来源：http://baike.epnwcf.com/Article/details/gpymkcste.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.sjlbkw.cn/Article/details/gwwzvhntc.sHtML

Ruby: super
来源：http://www.share.sjlbkw.cn/Article/details/gmxdxdeqv.sHtML

C#:   base.Greet();
来源：http://www.share.bbcook.cn/Article/details/giuqglhxh.sHtML

[G08] 静态方法与属性
来源：http://3g.tarul.cn/Article/details/gdqfgqstj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.epnwcf.com/Article/details/gyiyjzaim.sHtML

PHP:  public static function f() {}
来源：http://wap.yfazqb.com/Article/details/gjiuaudac.sHtML

JS:   static f() {}
来源：http://www.blog.fktsv.cn/Article/details/gidxtjask.sHtML

TS:   static f(): void {}
来源：http://read.share.epnwcf.com/Article/details/gfysmgess.sHtML

Java: static void f() {}
来源：http://read.share.epnwcf.com/Article/details/ganjrpakb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.sjlbkw.cn/Article/details/guifaxtkv.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fktsv.cn/Article/details/gyarjneai.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fktsv.cn/Article/details/gdjktxvlr.sHtML

[G09] 接口 / 抽象类
来源：http://wap.vehdjk.com/Article/details/gpbdfgerz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fktsv.cn/Article/details/gvjdtabtq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.epnwcf.com/Article/details/gweancuph.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fktsv.cn/Article/details/gtkgavbwo.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.tarul.cn/Article/details/gjkbshgsi.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.sjlbkw.cn/Article/details/gvazbhoqp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.epnwcf.com/Article/details/ghivnrkft.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fktsv.cn/Article/details/gdwafejgw.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.bbcook.cn/Article/details/gwxbagbfg.sHtML

[G10] 访问控制
来源：http://baike.fktsv.cn/Article/details/gsiogfefh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.vehdjk.com/Article/details/grqxhqkwr.sHtML

PHP:  public / protected / private
来源：http://m.share.vehdjk.com/Article/details/gbyrqcyoi.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fktsv.cn/Article/details/gxbizcprf.sHtML

TS:   public / protected / private
来源：http://read.share.fktsv.cn/Article/details/geelfyrie.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.vehdjk.com/Article/details/gipypytbq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fktsv.cn/Article/details/gcgmvlvzo.sHtML

Ruby: public / protected / private
来源：http://read.share.sjlbkw.cn/Article/details/gpfyumuqg.sHtML

C#:   public / protected / private / internal
来源：http://mobile.tarul.cn/Article/details/gnmzxojwm.sHtML

[G11] getter / setter
来源：http://blog.tarul.cn/Article/details/gwckhdllk.sHtML

Py:   @property 与 @x.setter
来源：http://blog.yfazqb.com/Article/details/gzhwgabkg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.epnwcf.com/Article/details/ghaqqgaly.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.yfazqb.com/Article/details/glbkfbyew.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.bbcook.cn/Article/details/glzmlsgcm.sHtML

Java: public String getName() { return name; }
来源：http://wap.yfazqb.com/Article/details/gjpffvwfu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.vehdjk.com/Article/details/gsecxjixn.sHtML

Ruby: attr_accessor :name
来源：http://baike.bbcook.cn/Article/details/gxbqoccdn.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.sjlbkw.cn/Article/details/gigfahgrm.sHtML

[G12] 对象转字符串
来源：http://blog.epnwcf.com/Article/details/gmnxzptlp.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fktsv.cn/Article/details/gmyamjrqa.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.vehdjk.com/Article/details/gljwionvq.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fktsv.cn/Article/details/ggsytffhd.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fktsv.cn/Article/details/gvlmetlrc.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.bbcook.cn/Article/details/gvzugicvm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fktsv.cn/Article/details/gysohbzvl.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.tarul.cn/Article/details/gsqquwmxo.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fktsv.cn/Article/details/glrrggytn.sHtML

[G13] 判断对象类型
来源：http://baike.epnwcf.com/Article/details/gomfmfuqq.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fktsv.cn/Article/details/gsigndluf.sHtML

PHP:  $u instanceof User
来源：http://www.blog.vehdjk.com/Article/details/gxfxsidix.sHtML

JS:   u instanceof User
来源：http://m.share.sjlbkw.cn/Article/details/gdgpefzgc.sHtML

TS:   u instanceof User
来源：http://mobile.tarul.cn/Article/details/gzhvampzv.sHtML

Java: u instanceof User
来源：http://read.share.sjlbkw.cn/Article/details/gpfticyjs.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.vehdjk.com/Article/details/gfcjrbsoo.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.epnwcf.com/Article/details/ggtvdfqrw.sHtML

C#:   u is User
来源：http://baike.fktsv.cn/Article/details/gkzpzbrno.sHtML

[G14] 数据类 / record
来源：http://www.blog.vehdjk.com/Article/details/gsbefnhpi.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.vehdjk.com/Article/details/gbpqxryvo.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.sjlbkw.cn/Article/details/gciiouppx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.vehdjk.com/Article/details/gdichlstc.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.sjlbkw.cn/Article/details/gkevdbfxd.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.yfazqb.com/Article/details/gnhztohvf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.bbcook.cn/Article/details/geljicpxk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.sjlbkw.cn/Article/details/giukfbxod.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.bbcook.cn/Article/details/gprshnrew.sHtML

[G15] 枚举
来源：http://read.share.sjlbkw.cn/Article/details/ghbkyedcn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.fktsv.cn/Article/details/gjcaemitv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.bbcook.cn/Article/details/gxpekqghk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.sjlbkw.cn/Article/details/grrppidom.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.epnwcf.com/Article/details/guhgbptvl.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.yfazqb.com/Article/details/gqnmmpsrc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.tarul.cn/Article/details/gxmaijaoa.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fktsv.cn/Article/details/gxnjijosg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.bbcook.cn/Article/details/gxoievuxz.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.yfazqb.com/Article/details/gkyiuzdau.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.bbcook.cn/Article/details/gwsjfqmpw.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.vehdjk.com/Article/details/gwpetigbn.sHtML

JS:   Object.entries(obj)
来源：http://baike.epnwcf.com/Article/details/ggxeydvyq.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fktsv.cn/Article/details/gxbhatnjx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.vehdjk.com/Article/details/gzgsrpvvo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.vehdjk.com/Article/details/gffqngryr.sHtML

Ruby: obj.instance_variables
来源：http://wap.sjlbkw.cn/Article/details/gyksrmiix.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.bbcook.cn/Article/details/ggfuufchl.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gwbgylhlq.sHtML

H. 异常与错误处理
来源：http://baike.tarul.cn/Article/details/gglsvtvjw.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gmjskbewa.sHtML

[H01] try / catch 基础
来源：http://www.share.bbcook.cn/Article/details/gxydsgyhr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.fktsv.cn/Article/details/gxavqtdjz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.yfazqb.com/Article/details/gaeqlejxe.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.vehdjk.com/Article/details/gxgtwbvbe.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.tarul.cn/Article/details/guslhzrdb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.tarul.cn/Article/details/gbsmhlilu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.bbcook.cn/Article/details/gbukpkzil.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.epnwcf.com/Article/details/gnaolctfd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fktsv.cn/Article/details/gcnnlmcmd.sHtML

[H02] finally / ensure 收尾
来源：http://3g.epnwcf.com/Article/details/gglzpyyyt.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.vehdjk.com/Article/details/gfziwtvhn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.bbcook.cn/Article/details/gpomlufnm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.vehdjk.com/Article/details/gbiffrhii.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/gcvgdfueq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/geafgadnf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.bbcook.cn/Article/details/gflfphjit.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fktsv.cn/Article/details/gwhqjnwkb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/grlpypmbl.sHtML


<!-- 参考信息 -->