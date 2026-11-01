代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.bbcook.cn/Article/details/gitkwmsga.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.bbcook.cn/Article/details/gfvvfuwnv.sHtML

TS:   if (s === "") {}
来源：http://www.share.tarul.cn/Article/details/gphcekrxu.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.epnwcf.com/Article/details/gpnwnbwvt.sHtML

Go:   if s == "" {}
来源：http://www.m.share.epnwcf.com/Article/details/gjdzgjkkm.sHtML

Ruby: if s.empty?
来源：http://blog.tarul.cn/Article/details/glazicnkc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.vehdjk.com/Article/details/gjborifnp.sHtML

[E21] 超长截断加省略号
来源：http://baike.sjlbkw.cn/Article/details/gevbfwsdg.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.bbcook.cn/Article/details/gzxesjqmj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fktsv.cn/Article/details/gjefirgfb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.tarul.cn/Article/details/gyndeenam.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.bbcook.cn/Article/details/gzrzeanyg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gnngikbna.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.bbcook.cn/Article/details/gkhzzlsbd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gvqgyllap.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.tarul.cn/Article/details/gvlejpupi.sHtML

[E22] 字节长度与字符长度
来源：http://baike.vehdjk.com/Article/details/gbbdfsngu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.vehdjk.com/Article/details/gcymlfwhe.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.tarul.cn/Article/details/gnbsezfsb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.epnwcf.com/Article/details/gdtegvwbk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.tarul.cn/Article/details/grgdhtath.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.yfazqb.com/Article/details/gqqkccuxp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.epnwcf.com/Article/details/gklugiqio.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.bbcook.cn/Article/details/gospycmpj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.tarul.cn/Article/details/gcdjvoryp.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gdjpmteex.sHtML

F. 文件与目录
来源：http://m.share.tarul.cn/Article/details/grewiimvz.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/ggagolgwh.sHtML

[F01] 读取整个文件
来源：http://baike.epnwcf.com/Article/details/gnfpzknei.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fktsv.cn/Article/details/gvaemyjxo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.vehdjk.com/Article/details/ghhdgtdgv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.sjlbkw.cn/Article/details/gnkmmqjpa.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fktsv.cn/Article/details/ganmqcqep.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.sjlbkw.cn/Article/details/getvysnjg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fktsv.cn/Article/details/ggiljyjou.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gfodrfbcn.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gqdtbrgyo.sHtML

[F02] 逐行读取文件
来源：http://www.share.vehdjk.com/Article/details/gxfrjibzq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.tarul.cn/Article/details/gzaolcrri.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.tarul.cn/Article/details/giladwiyy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.bbcook.cn/Article/details/ghnoprqjc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.vehdjk.com/Article/details/glnsezuxu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.yfazqb.com/Article/details/grbwpuooi.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.bbcook.cn/Article/details/glvaulxkg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.tarul.cn/Article/details/ghtidbtgd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.vehdjk.com/Article/details/gtabdtoae.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.bbcook.cn/Article/details/gqynmlfuz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.sjlbkw.cn/Article/details/gitqujdim.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.yfazqb.com/Article/details/gqriihxam.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.sjlbkw.cn/Article/details/gneullqls.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.yfazqb.com/Article/details/gaojgxctk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.epnwcf.com/Article/details/gyidsxfst.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fktsv.cn/Article/details/gygbkquap.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.yfazqb.com/Article/details/geslmwoen.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fktsv.cn/Article/details/gllylsxib.sHtML

[F04] 追加写入文件
来源：http://www.m.share.tarul.cn/Article/details/giparjbry.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.yfazqb.com/Article/details/gzyttlnbj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.bbcook.cn/Article/details/gxotdcwjl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.vehdjk.com/Article/details/gtjbdbahf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.vehdjk.com/Article/details/gefxdcbdm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.tarul.cn/Article/details/gqogauibc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.vehdjk.com/Article/details/gntbfjggo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.epnwcf.com/Article/details/gfybzilqa.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.sjlbkw.cn/Article/details/gleqkwtjn.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.bbcook.cn/Article/details/gooesqzpv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.vehdjk.com/Article/details/gjboycjbx.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gwnllfwbm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.vehdjk.com/Article/details/gqiiylnke.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.tarul.cn/Article/details/gwhoygont.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.sjlbkw.cn/Article/details/gdtknltum.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.vehdjk.com/Article/details/gylmgdmma.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gesybrqfz.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gepqrfzni.sHtML

[F06] 删除文件
来源：http://blog.sjlbkw.cn/Article/details/gxdfxcyrc.sHtML

Py:   os.remove("a.txt")
来源：http://3g.yfazqb.com/Article/details/gpruexprg.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gkaesjxlf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fktsv.cn/Article/details/gcnhjeifc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gamcsfezm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.sjlbkw.cn/Article/details/gimwyjmhn.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fktsv.cn/Article/details/gkqzhzmzh.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.tarul.cn/Article/details/ghdigdlif.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.bbcook.cn/Article/details/geofibgdg.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fktsv.cn/Article/details/gskzmykdg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fktsv.cn/Article/details/gyfbugssu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.yfazqb.com/Article/details/gxsgccqrj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.sjlbkw.cn/Article/details/gaoeoeijj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fktsv.cn/Article/details/gixqxdtnf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fktsv.cn/Article/details/guipdlaba.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.sjlbkw.cn/Article/details/glqiberqk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.yfazqb.com/Article/details/glbvwxyvw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.sjlbkw.cn/Article/details/gnoysuqtr.sHtML

[F08] 遍历目录
来源：http://www.share.tarul.cn/Article/details/gjddjatly.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.epnwcf.com/Article/details/gwnzyuhmj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.epnwcf.com/Article/details/gfpfojbzu.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.vehdjk.com/Article/details/gyrrgifbn.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.yfazqb.com/Article/details/gxxwqpkbb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.sjlbkw.cn/Article/details/gktubwtew.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.epnwcf.com/Article/details/gqbrgpcic.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.yfazqb.com/Article/details/gxivlifwf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fktsv.cn/Article/details/gryxeclid.sHtML

[F09] 获取文件大小
来源：http://baike.sjlbkw.cn/Article/details/gtmwuwcxa.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/grqcjybir.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gxawfjkbx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.tarul.cn/Article/details/gfnwtjkkf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.bbcook.cn/Article/details/gcehscqvp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.sjlbkw.cn/Article/details/gbggfukee.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.yfazqb.com/Article/details/glnypkspo.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gryacsucz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.yfazqb.com/Article/details/gcetarwhm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.bbcook.cn/Article/details/grxaraqaf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.vehdjk.com/Article/details/gibgbxowc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gqrnkevwc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.yfazqb.com/Article/details/guvdoeumg.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gewdyprsx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.epnwcf.com/Article/details/gczizgnbc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.tarul.cn/Article/details/grvqrcpcf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gwzswwllb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/gtqzbnybz.sHtML

[F11] 复制与移动文件
来源：http://3g.tarul.cn/Article/details/gulklobfe.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gglsnydab.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.vehdjk.com/Article/details/grbayfomy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.yfazqb.com/Article/details/gphrtxtom.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.epnwcf.com/Article/details/gbjcvxinz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.yfazqb.com/Article/details/gciwboecx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.tarul.cn/Article/details/gxxrfuszd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.epnwcf.com/Article/details/gsnqejgvl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fktsv.cn/Article/details/gsqbtxvri.sHtML

[F12] CSV 读写
来源：http://read.share.bbcook.cn/Article/details/ggougtquh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.epnwcf.com/Article/details/gftwowmgq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fktsv.cn/Article/details/gnmgxsxyv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.tarul.cn/Article/details/gjcgjsveu.sHtML

TS:   // 同上
来源：http://wap.bbcook.cn/Article/details/gzglzddwv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.vehdjk.com/Article/details/gutckomxq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.tarul.cn/Article/details/gstxawmjm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.bbcook.cn/Article/details/gerzzxufn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.bbcook.cn/Article/details/grfipnjdm.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gwxxrmbtz.sHtML

G. 面向对象
来源：http://read.share.tarul.cn/Article/details/gxytnuiit.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gcqaxhngu.sHtML

[G01] 定义类
来源：http://baike.fktsv.cn/Article/details/gnkdrcmrk.sHtML

Py:   class User: pass
来源：http://www.m.share.tarul.cn/Article/details/gwcgptrjn.sHtML

PHP:  class User {}
来源：http://m.share.bbcook.cn/Article/details/gdxhksopz.sHtML

JS:   class User {}
来源：http://www.blog.yfazqb.com/Article/details/gatnbjwnn.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.epnwcf.com/Article/details/gldmcmzar.sHtML

Java: class User {}
来源：http://www.m.share.epnwcf.com/Article/details/ghlcsrtgn.sHtML

Go:   type User struct { Name string }
来源：http://m.share.vehdjk.com/Article/details/gtoxxgjkm.sHtML

Ruby: class User; end
来源：http://blog.epnwcf.com/Article/details/gcnqmeaho.sHtML

C#:   class User {}
来源：http://baike.vehdjk.com/Article/details/gvrjzdefq.sHtML

[G02] 构造函数
来源：http://blog.yfazqb.com/Article/details/gthhplkrf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.vehdjk.com/Article/details/gdqmhbszs.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.vehdjk.com/Article/details/grlhtoewb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.yfazqb.com/Article/details/gqbgvhbjd.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.epnwcf.com/Article/details/gbraisxkf.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.bbcook.cn/Article/details/gaiffzugd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.sjlbkw.cn/Article/details/gzdifdplw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.sjlbkw.cn/Article/details/gjdincmow.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fktsv.cn/Article/details/ghmtvvrbc.sHtML

[G03] 实例属性
来源：http://3g.tarul.cn/Article/details/gpnwxpmjf.sHtML

Py:   self.name = "x"
来源：http://blog.epnwcf.com/Article/details/glugksmqq.sHtML

PHP:  public string $name = "x";
来源：http://mobile.tarul.cn/Article/details/gzoogifqs.sHtML

JS:   this.name = "x";
来源：http://blog.epnwcf.com/Article/details/gcrjgaszl.sHtML

TS:   name: string = "x";
来源：http://m.share.bbcook.cn/Article/details/gbaoscvqh.sHtML

Java: private String name;
来源：http://wap.bbcook.cn/Article/details/gldhfbigg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.yfazqb.com/Article/details/gerjvlrra.sHtML

Ruby: @name = "x"
来源：http://m.share.fktsv.cn/Article/details/ghutjdkxs.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.vehdjk.com/Article/details/geelvwiuw.sHtML

[G04] 定义方法
来源：http://baike.vehdjk.com/Article/details/glgwfbtlw.sHtML

Py:   def greet(self): return self.name
来源：http://blog.sjlbkw.cn/Article/details/gphgfwvsp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.yfazqb.com/Article/details/gvrcvbvid.sHtML

JS:   greet() { return this.name; }
来源：http://3g.bbcook.cn/Article/details/gmjyvvmky.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.bbcook.cn/Article/details/grljsnpyv.sHtML

Java: String greet() { return name; }
来源：http://www.share.bbcook.cn/Article/details/geeomukli.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.sjlbkw.cn/Article/details/glulqeogl.sHtML

Ruby: def greet; @name; end
来源：http://m.share.epnwcf.com/Article/details/grfwdotfa.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.vehdjk.com/Article/details/gdyzwqbbe.sHtML

[G05] 继承
来源：http://3g.tarul.cn/Article/details/glstdmwyr.sHtML

Py:   class Admin(User): pass
来源：http://m.share.bbcook.cn/Article/details/gohaoyjsg.sHtML

PHP:  class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/gzfyppamq.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/gzxifpbdo.sHtML

TS:   class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/gsxaihjya.sHtML

Java: class Admin extends User {}
来源：http://m.share.bbcook.cn/Article/details/gzlnjwkyz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.bbcook.cn/Article/details/gnjphjidk.sHtML

Ruby: class Admin < User; end
来源：http://wap.sjlbkw.cn/Article/details/gurfgwryh.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fktsv.cn/Article/details/grzrkrrex.sHtML

[G06] 重写方法
来源：http://baike.vehdjk.com/Article/details/grpcszjjl.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.bbcook.cn/Article/details/ghdfazbth.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.vehdjk.com/Article/details/gjdaqhwei.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.epnwcf.com/Article/details/gpwmjvszo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.epnwcf.com/Article/details/gvrmwrjbq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.bbcook.cn/Article/details/gizbpmyat.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.yfazqb.com/Article/details/guwrqwnst.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.yfazqb.com/Article/details/gosgvbyyy.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.sjlbkw.cn/Article/details/geqhpnubn.sHtML

[G07] 调用父类方法
来源：http://www.m.share.bbcook.cn/Article/details/graigfhck.sHtML

Py:   super().greet()
来源：http://www.m.share.tarul.cn/Article/details/gkiacnxrd.sHtML

PHP:  parent::greet();
来源：http://m.share.epnwcf.com/Article/details/guzgcalvf.sHtML

JS:   super.greet();
来源：http://mobile.vehdjk.com/Article/details/gtsjoamfu.sHtML

TS:   super.greet();
来源：http://www.m.share.bbcook.cn/Article/details/guiccfvrp.sHtML

Java: super.greet();
来源：http://3g.tarul.cn/Article/details/gycclbbjv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.tarul.cn/Article/details/groyqdfva.sHtML

Ruby: super
来源：http://blog.yfazqb.com/Article/details/gevjmxgdb.sHtML

C#:   base.Greet();
来源：http://www.m.share.tarul.cn/Article/details/ggxssdvib.sHtML

[G08] 静态方法与属性
来源：http://www.blog.tarul.cn/Article/details/gwodkwjlo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.bbcook.cn/Article/details/gaqbszfkx.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fktsv.cn/Article/details/geunhpojs.sHtML

JS:   static f() {}
来源：http://baike.bbcook.cn/Article/details/gnstrvmht.sHtML

TS:   static f(): void {}
来源：http://read.share.sjlbkw.cn/Article/details/gfsdebzqr.sHtML

Java: static void f() {}
来源：http://www.share.epnwcf.com/Article/details/gkruxflaw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fktsv.cn/Article/details/gdsgxxlsx.sHtML

Ruby: def self.f; end
来源：http://mobile.fktsv.cn/Article/details/gfilllauk.sHtML

C#:   public static void F() {}
来源：http://wap.epnwcf.com/Article/details/gtzblnbqb.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.bbcook.cn/Article/details/guzvankav.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.epnwcf.com/Article/details/gwkzslrsj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.epnwcf.com/Article/details/gdrabmnzt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fktsv.cn/Article/details/gapcksyoh.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.sjlbkw.cn/Article/details/gguvxexlr.sHtML

Java: interface Shape { double area(); }
来源：http://wap.sjlbkw.cn/Article/details/gqlvmrpcp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.vehdjk.com/Article/details/gyimtcqfs.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.epnwcf.com/Article/details/gexavejzx.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.sjlbkw.cn/Article/details/gkorotzlj.sHtML

[G10] 访问控制
来源：http://www.m.share.tarul.cn/Article/details/gtydcmxtt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.tarul.cn/Article/details/gtwnmljyx.sHtML

PHP:  public / protected / private
来源：http://www.blog.fktsv.cn/Article/details/gbicjiten.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.vehdjk.com/Article/details/gsylmqdlx.sHtML

TS:   public / protected / private
来源：http://www.share.sjlbkw.cn/Article/details/gjzbycxor.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.yfazqb.com/Article/details/gouqhrkse.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.vehdjk.com/Article/details/gnxitydoz.sHtML

Ruby: public / protected / private
来源：http://blog.bbcook.cn/Article/details/govuuqdte.sHtML

C#:   public / protected / private / internal
来源：http://baike.yfazqb.com/Article/details/ggcwyfyvi.sHtML

[G11] getter / setter
来源：http://www.m.share.fktsv.cn/Article/details/gnfnaxqgx.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.sjlbkw.cn/Article/details/gvedlhsag.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fktsv.cn/Article/details/gcuzsnidr.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.bbcook.cn/Article/details/gyxocneld.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fktsv.cn/Article/details/gtqqkmtww.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fktsv.cn/Article/details/grqolynco.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.sjlbkw.cn/Article/details/gvqumokig.sHtML

Ruby: attr_accessor :name
来源：http://mobile.vehdjk.com/Article/details/gqsqpnqcq.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.yfazqb.com/Article/details/gbdfffajf.sHtML

[G12] 对象转字符串
来源：http://www.share.bbcook.cn/Article/details/ghwjgpmgz.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.bbcook.cn/Article/details/gwghtdbug.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.bbcook.cn/Article/details/gymjnoitr.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.bbcook.cn/Article/details/gnmnpomaj.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fktsv.cn/Article/details/gyxkfgavx.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.bbcook.cn/Article/details/gqnekipli.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fktsv.cn/Article/details/gwhujwclf.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gnxwstqnm.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.sjlbkw.cn/Article/details/gshrtoxoe.sHtML

[G13] 判断对象类型
来源：http://www.share.bbcook.cn/Article/details/gsrbhhtdj.sHtML

Py:   isinstance(u, User)
来源：http://read.share.tarul.cn/Article/details/gmcqzrmks.sHtML

PHP:  $u instanceof User
来源：http://wap.bbcook.cn/Article/details/gnscslufw.sHtML

JS:   u instanceof User
来源：http://www.share.fktsv.cn/Article/details/gyapxqadn.sHtML

TS:   u instanceof User
来源：http://read.share.tarul.cn/Article/details/gowgqkhdw.sHtML

Java: u instanceof User
来源：http://3g.vehdjk.com/Article/details/gwihaybil.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.epnwcf.com/Article/details/gjjtjrrms.sHtML

Ruby: u.is_a?(User)
来源：http://3g.bbcook.cn/Article/details/gyukyedav.sHtML

C#:   u is User
来源：http://www.blog.yfazqb.com/Article/details/gjvnqjxzs.sHtML

[G14] 数据类 / record
来源：http://wap.tarul.cn/Article/details/gxlwvxfid.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fktsv.cn/Article/details/gesymqrjc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.yfazqb.com/Article/details/gkaeetwho.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.yfazqb.com/Article/details/gywtpzgee.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fktsv.cn/Article/details/gqpybvikw.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gtwwqqmlk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.tarul.cn/Article/details/gyvuieytp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.bbcook.cn/Article/details/gwicryetk.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fktsv.cn/Article/details/gbxkingwc.sHtML

[G15] 枚举
来源：http://read.share.sjlbkw.cn/Article/details/ghxxpahbz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.tarul.cn/Article/details/gpfifcphd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.bbcook.cn/Article/details/gdrapjjau.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.yfazqb.com/Article/details/gvslfoepi.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.tarul.cn/Article/details/genosfoud.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.bbcook.cn/Article/details/gtxojkvko.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.vehdjk.com/Article/details/gfgqjshwm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.epnwcf.com/Article/details/gleotvqbs.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.vehdjk.com/Article/details/glgjxqzfg.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.vehdjk.com/Article/details/gppdsiwjt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.vehdjk.com/Article/details/gyfddieka.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.bbcook.cn/Article/details/gsztruwpj.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fktsv.cn/Article/details/gixqevqay.sHtML

TS:   Object.entries(obj)
来源：http://wap.vehdjk.com/Article/details/gxtgrcsrg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.tarul.cn/Article/details/gaiqxcgtx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.tarul.cn/Article/details/gujfjbshl.sHtML

Ruby: obj.instance_variables
来源：http://mobile.vehdjk.com/Article/details/gmxygimzv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.vehdjk.com/Article/details/gobdfbpcl.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gglvymzcg.sHtML

H. 异常与错误处理
来源：http://www.blog.tarul.cn/Article/details/grpgozwrm.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/giqgsvzdr.sHtML

[H01] try / catch 基础
来源：http://m.share.vehdjk.com/Article/details/gfhuersnv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.sjlbkw.cn/Article/details/gsqamcerh.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.bbcook.cn/Article/details/gyvaejcox.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.bbcook.cn/Article/details/gkctcalnp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.sjlbkw.cn/Article/details/gwpuzybwx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.fktsv.cn/Article/details/gkwyyidgp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.epnwcf.com/Article/details/gtpyqaobr.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.yfazqb.com/Article/details/gcznxkgow.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.yfazqb.com/Article/details/gwaabdyjq.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.yfazqb.com/Article/details/gxhfxhdgc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.tarul.cn/Article/details/gjwdvzxhd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.epnwcf.com/Article/details/gjyuupthz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.bbcook.cn/Article/details/guxmxkhkf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.vehdjk.com/Article/details/gbtsojjqn.sHtML


<!-- 参考信息 -->