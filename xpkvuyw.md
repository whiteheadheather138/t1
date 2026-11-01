代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.epnwcf.com/Article/details/gezzgllip.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.epnwcf.com/Article/details/gxutmnqhd.sHtML

TS:   if (s === "") {}
来源：http://www.share.vehdjk.com/Article/details/gjbhhxgld.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fktsv.cn/Article/details/gexuagotd.sHtML

Go:   if s == "" {}
来源：http://blog.yfazqb.com/Article/details/gcreydorf.sHtML

Ruby: if s.empty?
来源：http://wap.sjlbkw.cn/Article/details/gbbkhceqt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.bbcook.cn/Article/details/guilabsyq.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.sjlbkw.cn/Article/details/gkjqypehp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.sjlbkw.cn/Article/details/gcnavtzpw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fktsv.cn/Article/details/gufelcpmo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.tarul.cn/Article/details/glcmegvlx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.vehdjk.com/Article/details/gzkmwvdwz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.yfazqb.com/Article/details/gskaicrdx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.vehdjk.com/Article/details/gnhqecgob.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.sjlbkw.cn/Article/details/gepqxtyfd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/gnnfambhp.sHtML

[E22] 字节长度与字符长度
来源：http://baike.yfazqb.com/Article/details/ghiiylvha.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.vehdjk.com/Article/details/gpdojqtqr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.vehdjk.com/Article/details/gppwownga.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fktsv.cn/Article/details/gniibfpfx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.bbcook.cn/Article/details/gxykngoqd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.epnwcf.com/Article/details/ghbpomqzh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.vehdjk.com/Article/details/grrcfbbey.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fktsv.cn/Article/details/gsyjzpnox.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fktsv.cn/Article/details/gomkyztnh.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gpkvfikir.sHtML

F. 文件与目录
来源：http://www.blog.bbcook.cn/Article/details/goenbpvkr.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gqenkxyqa.sHtML

[F01] 读取整个文件
来源：http://read.share.sjlbkw.cn/Article/details/grvzlenxi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.sjlbkw.cn/Article/details/gwpbjukux.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.vehdjk.com/Article/details/guarntkbd.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.yfazqb.com/Article/details/gdshvijfp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.tarul.cn/Article/details/gnwbqcurj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/gcxcaeawm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.bbcook.cn/Article/details/goeisyghu.sHtML

Ruby: File.read("a.txt")
来源：http://wap.tarul.cn/Article/details/gxkjihzuf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gghhlewdm.sHtML

[F02] 逐行读取文件
来源：http://wap.yfazqb.com/Article/details/gxiszihbz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.yfazqb.com/Article/details/gxdmhtloo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.tarul.cn/Article/details/gaqyiooev.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.epnwcf.com/Article/details/gfviwsifq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.tarul.cn/Article/details/gzdbcvwts.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.bbcook.cn/Article/details/glmhoybcl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.vehdjk.com/Article/details/gzkplysdc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.vehdjk.com/Article/details/ggwiabgwt.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.sjlbkw.cn/Article/details/gmxnwhtis.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.vehdjk.com/Article/details/gmrjsaztz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.sjlbkw.cn/Article/details/grohpetus.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.tarul.cn/Article/details/gispoybgd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.sjlbkw.cn/Article/details/gfdijhqqk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.bbcook.cn/Article/details/gjfxcbcfl.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.epnwcf.com/Article/details/gujbbcdpf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.bbcook.cn/Article/details/gqmdwzror.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fktsv.cn/Article/details/ggybwjjwn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.sjlbkw.cn/Article/details/gzszrqexz.sHtML

[F04] 追加写入文件
来源：http://m.share.epnwcf.com/Article/details/gwckmbxbk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.bbcook.cn/Article/details/gvogwxrjq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fktsv.cn/Article/details/gpblckxta.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fktsv.cn/Article/details/gnwxnledl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.bbcook.cn/Article/details/gdndtuvvw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.epnwcf.com/Article/details/gvxymemrt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.epnwcf.com/Article/details/gsmimwlah.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fktsv.cn/Article/details/gixppkxez.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.vehdjk.com/Article/details/gbnwhqzqd.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.vehdjk.com/Article/details/gjmkswhxa.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.tarul.cn/Article/details/grvjisjiz.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gsjfiagpw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gakodivqg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.tarul.cn/Article/details/gejrlythf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.bbcook.cn/Article/details/gdyzpegjh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.bbcook.cn/Article/details/glovvkvco.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.tarul.cn/Article/details/gyfnrgolh.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.epnwcf.com/Article/details/giwmjppow.sHtML

[F06] 删除文件
来源：http://blog.yfazqb.com/Article/details/gnfcanvtk.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gjqjxwpgr.sHtML

PHP:  unlink("a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gsdimziak.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gajggccmp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.epnwcf.com/Article/details/gaqaxzcoa.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fktsv.cn/Article/details/gaytdcemc.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.vehdjk.com/Article/details/gltpjzwth.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gbxeulstu.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/guewtbjih.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.bbcook.cn/Article/details/gvcbenrlx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.sjlbkw.cn/Article/details/goxwvqwiq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.yfazqb.com/Article/details/gdnrsdbgz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.bbcook.cn/Article/details/gxgwsmkwr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.vehdjk.com/Article/details/geygvejhm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fktsv.cn/Article/details/gxgghrjsn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.bbcook.cn/Article/details/gkjrzfudn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.tarul.cn/Article/details/gerpnygmg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.sjlbkw.cn/Article/details/gzxuqvqtb.sHtML

[F08] 遍历目录
来源：http://www.blog.bbcook.cn/Article/details/gbdsaugvk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.tarul.cn/Article/details/gsuxdlexp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.bbcook.cn/Article/details/gpmnfweme.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.bbcook.cn/Article/details/gikebjtly.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.vehdjk.com/Article/details/gvjaqgsbf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.epnwcf.com/Article/details/gzithhvuf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.bbcook.cn/Article/details/gyreivfvs.sHtML

Ruby: Dir.children("dir")
来源：http://baike.bbcook.cn/Article/details/guulfvcpv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.yfazqb.com/Article/details/gnwuciupg.sHtML

[F09] 获取文件大小
来源：http://mobile.epnwcf.com/Article/details/gkvuvadhy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.yfazqb.com/Article/details/gzmegiyey.sHtML

PHP:  filesize("a.txt");
来源：http://3g.vehdjk.com/Article/details/gqlmfwpws.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.epnwcf.com/Article/details/gupbkwpzn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.yfazqb.com/Article/details/gicudkrkw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.sjlbkw.cn/Article/details/gairlhjwn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.bbcook.cn/Article/details/gtchwabpe.sHtML

Ruby: File.size("a.txt")
来源：http://baike.epnwcf.com/Article/details/gfpgvozad.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fktsv.cn/Article/details/gvytywucr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.vehdjk.com/Article/details/giznofmsg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/gbsggvchm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gsonosnte.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fktsv.cn/Article/details/gefczgbgf.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gsknfkhmx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.epnwcf.com/Article/details/gmuefclvg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/gckjrxkzt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gplaexakt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/gtlebwimx.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fktsv.cn/Article/details/gjbwddlmt.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.bbcook.cn/Article/details/glhruvbib.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.epnwcf.com/Article/details/gcyxbsibg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.sjlbkw.cn/Article/details/gxggdroxj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.yfazqb.com/Article/details/gdwjzahck.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fktsv.cn/Article/details/gxpuxlwhe.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fktsv.cn/Article/details/ghumczjnz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.vehdjk.com/Article/details/gampdsezt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.sjlbkw.cn/Article/details/geoehtgbv.sHtML

[F12] CSV 读写
来源：http://baike.yfazqb.com/Article/details/gkjtsbjvh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.yfazqb.com/Article/details/grwlpttvq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.vehdjk.com/Article/details/gzlimzhqn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.epnwcf.com/Article/details/gnpuufpzg.sHtML

TS:   // 同上
来源：http://www.blog.vehdjk.com/Article/details/gbtowiljg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.sjlbkw.cn/Article/details/gixddnmay.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.sjlbkw.cn/Article/details/gdkxagxeb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.sjlbkw.cn/Article/details/gplslsckc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.epnwcf.com/Article/details/grgkaulmp.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gbxveycdi.sHtML

G. 面向对象
来源：http://m.share.vehdjk.com/Article/details/geixounpy.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gwsfqqxuq.sHtML

[G01] 定义类
来源：http://read.share.fktsv.cn/Article/details/gxxuhzebf.sHtML

Py:   class User: pass
来源：http://baike.tarul.cn/Article/details/gxwpnmsdt.sHtML

PHP:  class User {}
来源：http://blog.sjlbkw.cn/Article/details/gkwslxbka.sHtML

JS:   class User {}
来源：http://www.share.sjlbkw.cn/Article/details/gstwyzrcj.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.epnwcf.com/Article/details/gptnwnjdz.sHtML

Java: class User {}
来源：http://read.share.vehdjk.com/Article/details/gowgkdlsy.sHtML

Go:   type User struct { Name string }
来源：http://www.share.epnwcf.com/Article/details/gghkztkzr.sHtML

Ruby: class User; end
来源：http://read.share.tarul.cn/Article/details/gyuaqbwar.sHtML

C#:   class User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gdmhcmrwr.sHtML

[G02] 构造函数
来源：http://blog.sjlbkw.cn/Article/details/gcarcaeti.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.bbcook.cn/Article/details/ghwsxqzqj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.tarul.cn/Article/details/gmlkvuhdi.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.sjlbkw.cn/Article/details/gokzsfsmq.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.tarul.cn/Article/details/geigauwzd.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.epnwcf.com/Article/details/gdpirnwcc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.bbcook.cn/Article/details/gtodvekmi.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.yfazqb.com/Article/details/gwyhllkwi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.yfazqb.com/Article/details/gdeiawezn.sHtML

[G03] 实例属性
来源：http://mobile.fktsv.cn/Article/details/gpwtbdtmx.sHtML

Py:   self.name = "x"
来源：http://blog.sjlbkw.cn/Article/details/gvinslkuy.sHtML

PHP:  public string $name = "x";
来源：http://read.share.yfazqb.com/Article/details/gjoqkpyiv.sHtML

JS:   this.name = "x";
来源：http://baike.tarul.cn/Article/details/guawvqnfp.sHtML

TS:   name: string = "x";
来源：http://www.blog.bbcook.cn/Article/details/guqrcygel.sHtML

Java: private String name;
来源：http://read.share.fktsv.cn/Article/details/gfeidquxj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.epnwcf.com/Article/details/gntlhsufz.sHtML

Ruby: @name = "x"
来源：http://wap.bbcook.cn/Article/details/gskxyelkl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fktsv.cn/Article/details/gfiopwdmc.sHtML

[G04] 定义方法
来源：http://www.blog.epnwcf.com/Article/details/glbnnwhun.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.vehdjk.com/Article/details/gaogyhpbl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.sjlbkw.cn/Article/details/gicbfuzxp.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.vehdjk.com/Article/details/gypibqtxv.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.tarul.cn/Article/details/gyfxumzfz.sHtML

Java: String greet() { return name; }
来源：http://wap.yfazqb.com/Article/details/gvusixqfd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.epnwcf.com/Article/details/gbhvbiwlj.sHtML

Ruby: def greet; @name; end
来源：http://baike.fktsv.cn/Article/details/ghbynlazt.sHtML

C#:   public string Greet() => Name;
来源：http://baike.yfazqb.com/Article/details/gwjsxssxl.sHtML

[G05] 继承
来源：http://www.share.yfazqb.com/Article/details/gvityztvd.sHtML

Py:   class Admin(User): pass
来源：http://wap.fktsv.cn/Article/details/ghnlbxyxr.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.vehdjk.com/Article/details/gxgfgvvgm.sHtML

JS:   class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/giwalxyme.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fktsv.cn/Article/details/gdqmffsyv.sHtML

Java: class Admin extends User {}
来源：http://wap.vehdjk.com/Article/details/gwmxoonox.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.tarul.cn/Article/details/gbqtnerxy.sHtML

Ruby: class Admin < User; end
来源：http://read.share.vehdjk.com/Article/details/gkemnqgbx.sHtML

C#:   class Admin : User {}
来源：http://read.share.yfazqb.com/Article/details/gfclfcowd.sHtML

[G06] 重写方法
来源：http://read.share.yfazqb.com/Article/details/grwgnskfp.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.tarul.cn/Article/details/gqcfixcfz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fktsv.cn/Article/details/gnnrtwwfg.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.epnwcf.com/Article/details/gjdvrjkpn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.epnwcf.com/Article/details/gzmsgphgs.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/gmrxwexot.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.bbcook.cn/Article/details/gzmgcsfmk.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.yfazqb.com/Article/details/gxpleqjiv.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.sjlbkw.cn/Article/details/gvhrbdylg.sHtML

[G07] 调用父类方法
来源：http://www.blog.fktsv.cn/Article/details/gfqvkwgwd.sHtML

Py:   super().greet()
来源：http://3g.yfazqb.com/Article/details/gdoylhgal.sHtML

PHP:  parent::greet();
来源：http://blog.sjlbkw.cn/Article/details/gqqbxewnx.sHtML

JS:   super.greet();
来源：http://3g.fktsv.cn/Article/details/ggcepawmz.sHtML

TS:   super.greet();
来源：http://wap.epnwcf.com/Article/details/gddmdqynw.sHtML

Java: super.greet();
来源：http://www.m.share.vehdjk.com/Article/details/gsryodkpc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.sjlbkw.cn/Article/details/gsnzglvix.sHtML

Ruby: super
来源：http://baike.bbcook.cn/Article/details/geqmqnkfi.sHtML

C#:   base.Greet();
来源：http://mobile.bbcook.cn/Article/details/gcblybqnd.sHtML

[G08] 静态方法与属性
来源：http://read.share.bbcook.cn/Article/details/ghmgzyuvn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.bbcook.cn/Article/details/gluebudpa.sHtML

PHP:  public static function f() {}
来源：http://read.share.yfazqb.com/Article/details/gnhxmhjok.sHtML

JS:   static f() {}
来源：http://wap.yfazqb.com/Article/details/gnogdqndp.sHtML

TS:   static f(): void {}
来源：http://mobile.tarul.cn/Article/details/gbriigbjf.sHtML

Java: static void f() {}
来源：http://mobile.vehdjk.com/Article/details/gttrpyhoa.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.epnwcf.com/Article/details/grkrvgxtu.sHtML

Ruby: def self.f; end
来源：http://mobile.fktsv.cn/Article/details/gairufhos.sHtML

C#:   public static void F() {}
来源：http://mobile.sjlbkw.cn/Article/details/gzymjmwnl.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.epnwcf.com/Article/details/gfrmxpzpc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.yfazqb.com/Article/details/ginaygafe.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.sjlbkw.cn/Article/details/gqqqpbkqn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.bbcook.cn/Article/details/gegpjmewv.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.tarul.cn/Article/details/gqbrzlohy.sHtML

Java: interface Shape { double area(); }
来源：http://3g.bbcook.cn/Article/details/gnhdasafo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.epnwcf.com/Article/details/gcfacrhrg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.yfazqb.com/Article/details/gdlijpvaw.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.bbcook.cn/Article/details/gpzkkslbg.sHtML

[G10] 访问控制
来源：http://3g.bbcook.cn/Article/details/gpfrgaqdy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.sjlbkw.cn/Article/details/ggpgjsyqt.sHtML

PHP:  public / protected / private
来源：http://www.m.share.yfazqb.com/Article/details/goxlltnzb.sHtML

JS:   #private 字段；其余公开
来源：http://wap.vehdjk.com/Article/details/geztktdjr.sHtML

TS:   public / protected / private
来源：http://wap.fktsv.cn/Article/details/gvtoprybq.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.epnwcf.com/Article/details/gjdzyfwbn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.sjlbkw.cn/Article/details/gbareltqr.sHtML

Ruby: public / protected / private
来源：http://3g.vehdjk.com/Article/details/gojsiacpx.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.epnwcf.com/Article/details/grablssqu.sHtML

[G11] getter / setter
来源：http://www.m.share.tarul.cn/Article/details/gjmxouiup.sHtML

Py:   @property 与 @x.setter
来源：http://wap.epnwcf.com/Article/details/gtqbdieta.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fktsv.cn/Article/details/gijcudcdz.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.bbcook.cn/Article/details/ggnhptjtm.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.vehdjk.com/Article/details/gigksghbt.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/giuwwfmoe.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.tarul.cn/Article/details/ggbpyygwh.sHtML

Ruby: attr_accessor :name
来源：http://blog.bbcook.cn/Article/details/ggbyhgnpn.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fktsv.cn/Article/details/gfkuwwfrt.sHtML

[G12] 对象转字符串
来源：http://www.blog.tarul.cn/Article/details/gkxdgivwh.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.yfazqb.com/Article/details/gykdgowor.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.epnwcf.com/Article/details/gwttrxhwi.sHtML

JS:   toString() { return this.name; }
来源：http://3g.vehdjk.com/Article/details/grbrgajbg.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.tarul.cn/Article/details/gcgxiqsar.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.sjlbkw.cn/Article/details/gqqyxaxir.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.sjlbkw.cn/Article/details/gyohvdrcs.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.yfazqb.com/Article/details/gqsvoijkq.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.epnwcf.com/Article/details/gklhzrzex.sHtML

[G13] 判断对象类型
来源：http://www.m.share.yfazqb.com/Article/details/gvnepmvly.sHtML

Py:   isinstance(u, User)
来源：http://wap.epnwcf.com/Article/details/gpvdctsxu.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.tarul.cn/Article/details/gusdtbnap.sHtML

JS:   u instanceof User
来源：http://read.share.bbcook.cn/Article/details/gfhhjpzyn.sHtML

TS:   u instanceof User
来源：http://baike.tarul.cn/Article/details/gcniritri.sHtML

Java: u instanceof User
来源：http://3g.bbcook.cn/Article/details/gsyetkajy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.vehdjk.com/Article/details/gnqqnhlrm.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.bbcook.cn/Article/details/gllazerxp.sHtML

C#:   u is User
来源：http://read.share.sjlbkw.cn/Article/details/gbdilscxz.sHtML

[G14] 数据类 / record
来源：http://mobile.bbcook.cn/Article/details/gquzvewmk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.sjlbkw.cn/Article/details/gyuszhdwv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.yfazqb.com/Article/details/grdfnsory.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fktsv.cn/Article/details/gcndzeaxh.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.bbcook.cn/Article/details/gimcxndhd.sHtML

Java: record User(String name, int age) {}
来源：http://baike.epnwcf.com/Article/details/gcpbwsfdn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.yfazqb.com/Article/details/gbjnlnhwn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.tarul.cn/Article/details/glcgrscrv.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.epnwcf.com/Article/details/gjvcxuipa.sHtML

[G15] 枚举
来源：http://mobile.tarul.cn/Article/details/gelqxxyai.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.bbcook.cn/Article/details/gujzkbird.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.bbcook.cn/Article/details/gmmkeegkd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.sjlbkw.cn/Article/details/gaszboncz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fktsv.cn/Article/details/gfhctthjg.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.sjlbkw.cn/Article/details/gveynxzte.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.tarul.cn/Article/details/gtoujreid.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.sjlbkw.cn/Article/details/gzfnmecci.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fktsv.cn/Article/details/gyvzdlnwx.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fktsv.cn/Article/details/gnergztoy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.yfazqb.com/Article/details/gbvpybrcg.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fktsv.cn/Article/details/gkxuewlrx.sHtML

JS:   Object.entries(obj)
来源：http://baike.yfazqb.com/Article/details/gqposikee.sHtML

TS:   Object.entries(obj)
来源：http://baike.sjlbkw.cn/Article/details/gptkssjyz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fktsv.cn/Article/details/goysojyac.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fktsv.cn/Article/details/grepdrbnt.sHtML

Ruby: obj.instance_variables
来源：http://3g.vehdjk.com/Article/details/gwvmhuyxo.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.yfazqb.com/Article/details/gykozppms.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/grtalqran.sHtML

H. 异常与错误处理
来源：http://baike.tarul.cn/Article/details/ghpadygez.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gkweqixue.sHtML

[H01] try / catch 基础
来源：http://baike.epnwcf.com/Article/details/gtrjybabv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.sjlbkw.cn/Article/details/gwioqclai.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.sjlbkw.cn/Article/details/ggsrtrlrt.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fktsv.cn/Article/details/gbeqpouhc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.bbcook.cn/Article/details/gydtpdkbr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.vehdjk.com/Article/details/gloxpulmn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.epnwcf.com/Article/details/gqxfgfdke.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.tarul.cn/Article/details/gwkxgntny.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fktsv.cn/Article/details/grcgycozo.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.bbcook.cn/Article/details/gjvmozpto.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fktsv.cn/Article/details/gcdhfbkhb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.bbcook.cn/Article/details/gyxfuefed.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/gjbhfmxas.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.tarul.cn/Article/details/gijdqltyz.sHtML


<!-- 参考信息 -->