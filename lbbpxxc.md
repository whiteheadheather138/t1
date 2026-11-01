代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://baike.vehdjk.com/Article/details/gvnmipcmv.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.vehdjk.com/Article/details/gpyxbqmqp.sHtML

Java: s.lines().toList()
来源：http://wap.fktsv.cn/Article/details/gbalovcsz.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fktsv.cn/Article/details/gnyloxvqc.sHtML

Ruby: s.lines
来源：http://www.share.tarul.cn/Article/details/gakcdgqjx.sHtML

C#:   s.Split('\n')
来源：http://wap.fktsv.cn/Article/details/gepjghhro.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.vehdjk.com/Article/details/gzkirgsnd.sHtML

Py:   if not s:
来源：http://read.share.tarul.cn/Article/details/ghwvcjftq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.tarul.cn/Article/details/gwxdwvqvz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gbfwjydya.sHtML

TS:   if (s === "") {}
来源：http://baike.epnwcf.com/Article/details/gdjqusmmm.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.yfazqb.com/Article/details/gvpzcroip.sHtML

Go:   if s == "" {}
来源：http://blog.sjlbkw.cn/Article/details/gizlkpdmm.sHtML

Ruby: if s.empty?
来源：http://m.share.yfazqb.com/Article/details/gdxwfmloz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.bbcook.cn/Article/details/goimnidgx.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fktsv.cn/Article/details/ghyjtzyps.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.yfazqb.com/Article/details/gnchlsmsd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.tarul.cn/Article/details/glouxfusb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.yfazqb.com/Article/details/gkskwygpe.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.vehdjk.com/Article/details/ggulybsru.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fktsv.cn/Article/details/gqhjblciv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.yfazqb.com/Article/details/gwjmppkrf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.bbcook.cn/Article/details/gxitzezvo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.vehdjk.com/Article/details/gitfdsibw.sHtML

[E22] 字节长度与字符长度
来源：http://wap.vehdjk.com/Article/details/gnqlldezk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.bbcook.cn/Article/details/gnwgnodmx.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.tarul.cn/Article/details/gkpwmzuqs.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.yfazqb.com/Article/details/grsekmmww.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.vehdjk.com/Article/details/govnaqipa.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.epnwcf.com/Article/details/ghdycumca.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.sjlbkw.cn/Article/details/gkbwucyvx.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.tarul.cn/Article/details/ggggijwrb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fktsv.cn/Article/details/gyujanfqj.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gdenitgnj.sHtML

F. 文件与目录
来源：http://www.m.share.vehdjk.com/Article/details/gigbzqpec.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/godxcbwli.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fktsv.cn/Article/details/gxzkkwnsa.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.bbcook.cn/Article/details/gxzezfytq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fktsv.cn/Article/details/gokzlyyji.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.yfazqb.com/Article/details/gjqzmlctp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.yfazqb.com/Article/details/gilufytel.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/gsyrxwxng.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.sjlbkw.cn/Article/details/ggzkbrqlv.sHtML

Ruby: File.read("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gykcnfnfg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.tarul.cn/Article/details/gmusuosxq.sHtML

[F02] 逐行读取文件
来源：http://read.share.sjlbkw.cn/Article/details/govzqmyyz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.tarul.cn/Article/details/gylhiredk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.epnwcf.com/Article/details/gvyxdkvvm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.sjlbkw.cn/Article/details/ghjqowant.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.sjlbkw.cn/Article/details/gddvpqnzx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.yfazqb.com/Article/details/gipijvtko.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.sjlbkw.cn/Article/details/gahlzrwhe.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.vehdjk.com/Article/details/gbiddlrhe.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.yfazqb.com/Article/details/gmefcwfos.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.tarul.cn/Article/details/gspsfarjr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.tarul.cn/Article/details/glyxeauwt.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.epnwcf.com/Article/details/gxlaiygpj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.tarul.cn/Article/details/gfjvjwgui.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.tarul.cn/Article/details/geeemblzr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fktsv.cn/Article/details/gvoykdjzt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.tarul.cn/Article/details/grekyfbls.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.tarul.cn/Article/details/giqgmoclo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.sjlbkw.cn/Article/details/gpflsgjrk.sHtML

[F04] 追加写入文件
来源：http://baike.sjlbkw.cn/Article/details/gddbtaxdp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.yfazqb.com/Article/details/gvvuwrarn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.tarul.cn/Article/details/gqzkezwin.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.tarul.cn/Article/details/gugrydisz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.sjlbkw.cn/Article/details/gqromnfax.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.bbcook.cn/Article/details/gvrrrphfk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.sjlbkw.cn/Article/details/gephszdyo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.tarul.cn/Article/details/gtjoupmkk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.vehdjk.com/Article/details/gilirpllc.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.epnwcf.com/Article/details/getelzaol.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fktsv.cn/Article/details/gjkfxtgij.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.vehdjk.com/Article/details/gzvrktxhv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gwyypgqex.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gxtxtfzrf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.sjlbkw.cn/Article/details/genzjiahy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.tarul.cn/Article/details/ggcsvbsot.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gmomeighi.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.tarul.cn/Article/details/guziycfhr.sHtML

[F06] 删除文件
来源：http://www.blog.yfazqb.com/Article/details/gjyfnoiqd.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gyjlesteg.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/ghhfdgvof.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.yfazqb.com/Article/details/gbcdlbyrd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.vehdjk.com/Article/details/gknaxvroc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.vehdjk.com/Article/details/gqhcxqfgb.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.vehdjk.com/Article/details/giewmvhua.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.epnwcf.com/Article/details/guxnsvhjz.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gtznmjhcz.sHtML

[F07] 创建目录（含多级）
来源：http://baike.bbcook.cn/Article/details/gqrnoxhdr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fktsv.cn/Article/details/gmjhhunku.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.epnwcf.com/Article/details/gmxzqjvdc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.tarul.cn/Article/details/gebrroqpq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.vehdjk.com/Article/details/gorjiwpdp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.vehdjk.com/Article/details/gnmtnjplc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fktsv.cn/Article/details/ggjiugahl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.epnwcf.com/Article/details/gpimtoadh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.epnwcf.com/Article/details/gaszqxtyb.sHtML

[F08] 遍历目录
来源：http://mobile.sjlbkw.cn/Article/details/gcjtvzghi.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.yfazqb.com/Article/details/gaskoncpb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.sjlbkw.cn/Article/details/ggdgmqaoj.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fktsv.cn/Article/details/goyctnhne.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.epnwcf.com/Article/details/gtofphmur.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.sjlbkw.cn/Article/details/gcsuqqoml.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.tarul.cn/Article/details/gxykzciwc.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.epnwcf.com/Article/details/guekspyfg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.bbcook.cn/Article/details/gnqlnyxpj.sHtML

[F09] 获取文件大小
来源：http://blog.fktsv.cn/Article/details/gmdxmhyue.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gmjnhyich.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gmtpfrktn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.epnwcf.com/Article/details/gwrhtxutd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fktsv.cn/Article/details/gfjsvqrgl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.sjlbkw.cn/Article/details/gxqddcpyv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.vehdjk.com/Article/details/gexndjtkf.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.tarul.cn/Article/details/gnwpsqwaf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.yfazqb.com/Article/details/gjcmzmgrf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.tarul.cn/Article/details/gtkmqccci.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fktsv.cn/Article/details/gtoggzsuf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gpmibaeaf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gnnbaisbd.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gtzewpfnk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.epnwcf.com/Article/details/gkcasbhnu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gvhrjhspb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.tarul.cn/Article/details/ggazpwnyv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/gmouhprxv.sHtML

[F11] 复制与移动文件
来源：http://www.share.epnwcf.com/Article/details/gniauhvre.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.sjlbkw.cn/Article/details/grtcwaefk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.bbcook.cn/Article/details/gmlzhleji.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.sjlbkw.cn/Article/details/gjsfjntcj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gwepbmimr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.bbcook.cn/Article/details/gnixilusi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.vehdjk.com/Article/details/ghjvgkqoj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gtdsfqyxc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.epnwcf.com/Article/details/gglucazih.sHtML

[F12] CSV 读写
来源：http://www.share.vehdjk.com/Article/details/ggahhnzjr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fktsv.cn/Article/details/gpjrxcfat.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.tarul.cn/Article/details/glaxyotic.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.epnwcf.com/Article/details/genlvlxxm.sHtML

TS:   // 同上
来源：http://www.share.fktsv.cn/Article/details/gwornxrsd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.epnwcf.com/Article/details/gqscgcxfk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fktsv.cn/Article/details/gwzgiqqdf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.tarul.cn/Article/details/gwvfjqljg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.sjlbkw.cn/Article/details/gzrmrtdcw.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gosuitlva.sHtML

G. 面向对象
来源：http://3g.fktsv.cn/Article/details/gljehrjom.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gpvvldrpl.sHtML

[G01] 定义类
来源：http://wap.sjlbkw.cn/Article/details/grfyiwnrc.sHtML

Py:   class User: pass
来源：http://baike.epnwcf.com/Article/details/gujnybbpk.sHtML

PHP:  class User {}
来源：http://mobile.fktsv.cn/Article/details/gsyyybans.sHtML

JS:   class User {}
来源：http://read.share.vehdjk.com/Article/details/gfkoultse.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.bbcook.cn/Article/details/gkplhfdsb.sHtML

Java: class User {}
来源：http://www.share.bbcook.cn/Article/details/gqqkkiuso.sHtML

Go:   type User struct { Name string }
来源：http://www.share.sjlbkw.cn/Article/details/gwpaqrlej.sHtML

Ruby: class User; end
来源：http://m.share.fktsv.cn/Article/details/gfegfxwqp.sHtML

C#:   class User {}
来源：http://read.share.vehdjk.com/Article/details/gmavstbdb.sHtML

[G02] 构造函数
来源：http://mobile.bbcook.cn/Article/details/ghcplghgi.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.vehdjk.com/Article/details/gmqafsmhe.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.epnwcf.com/Article/details/gjjlmsnjf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gljndocso.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.vehdjk.com/Article/details/gxebhdntk.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.yfazqb.com/Article/details/gxaclvmrh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.vehdjk.com/Article/details/gdwbjhenm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.tarul.cn/Article/details/gccxoucjf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fktsv.cn/Article/details/gbcvdqlan.sHtML

[G03] 实例属性
来源：http://read.share.tarul.cn/Article/details/gilplpfvs.sHtML

Py:   self.name = "x"
来源：http://blog.bbcook.cn/Article/details/ganrlxhun.sHtML

PHP:  public string $name = "x";
来源：http://mobile.sjlbkw.cn/Article/details/gqhskvboq.sHtML

JS:   this.name = "x";
来源：http://read.share.vehdjk.com/Article/details/gcggwxubp.sHtML

TS:   name: string = "x";
来源：http://read.share.bbcook.cn/Article/details/gcowfiaku.sHtML

Java: private String name;
来源：http://m.share.epnwcf.com/Article/details/giwumvgdc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.vehdjk.com/Article/details/gjkznejax.sHtML

Ruby: @name = "x"
来源：http://www.m.share.bbcook.cn/Article/details/gqvomgwsh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.epnwcf.com/Article/details/gkczcbzoy.sHtML

[G04] 定义方法
来源：http://m.share.epnwcf.com/Article/details/glnuufyfw.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.yfazqb.com/Article/details/gbpgxecft.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.tarul.cn/Article/details/grazfbafr.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.tarul.cn/Article/details/giubitmjj.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/gthceysnw.sHtML

Java: String greet() { return name; }
来源：http://blog.tarul.cn/Article/details/gxtwvrpbl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fktsv.cn/Article/details/gbzidbgnu.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.epnwcf.com/Article/details/gtwqqydvk.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.tarul.cn/Article/details/gppbilbuy.sHtML

[G05] 继承
来源：http://www.blog.tarul.cn/Article/details/glkcovtyp.sHtML

Py:   class Admin(User): pass
来源：http://mobile.sjlbkw.cn/Article/details/gsnmiroca.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/glrkcrpsg.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.tarul.cn/Article/details/gvqctluzn.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gasfavnub.sHtML

Java: class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/ggqtjirhp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.tarul.cn/Article/details/gqfvasfwv.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gyjyhcdmd.sHtML

C#:   class Admin : User {}
来源：http://www.blog.yfazqb.com/Article/details/gwmifxxrv.sHtML

[G06] 重写方法
来源：http://3g.epnwcf.com/Article/details/gkkjqrtez.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fktsv.cn/Article/details/gmaktjenx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.sjlbkw.cn/Article/details/gibxzqblq.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.yfazqb.com/Article/details/gwjibdjdn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.epnwcf.com/Article/details/ghvkjngqw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.vehdjk.com/Article/details/gbjwzhhaw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.bbcook.cn/Article/details/goppjwxnj.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.vehdjk.com/Article/details/gnrrzwfcp.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.epnwcf.com/Article/details/gtcbocfse.sHtML

[G07] 调用父类方法
来源：http://mobile.epnwcf.com/Article/details/gepkhatag.sHtML

Py:   super().greet()
来源：http://baike.sjlbkw.cn/Article/details/gdxtmhzhm.sHtML

PHP:  parent::greet();
来源：http://wap.sjlbkw.cn/Article/details/gwxsiihld.sHtML

JS:   super.greet();
来源：http://www.m.share.epnwcf.com/Article/details/gdftklzit.sHtML

TS:   super.greet();
来源：http://baike.yfazqb.com/Article/details/gunxozijn.sHtML

Java: super.greet();
来源：http://www.share.yfazqb.com/Article/details/gezdfhmtj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.vehdjk.com/Article/details/gmmsyzxkn.sHtML

Ruby: super
来源：http://wap.tarul.cn/Article/details/gjvfpvavw.sHtML

C#:   base.Greet();
来源：http://wap.vehdjk.com/Article/details/gmypzivvd.sHtML

[G08] 静态方法与属性
来源：http://wap.fktsv.cn/Article/details/gvtqigfva.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.sjlbkw.cn/Article/details/ginvzaplf.sHtML

PHP:  public static function f() {}
来源：http://www.share.yfazqb.com/Article/details/gwhnetrsy.sHtML

JS:   static f() {}
来源：http://m.share.fktsv.cn/Article/details/gzdgremld.sHtML

TS:   static f(): void {}
来源：http://3g.bbcook.cn/Article/details/gwmvlceuf.sHtML

Java: static void f() {}
来源：http://blog.yfazqb.com/Article/details/gcaxdjxuz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.bbcook.cn/Article/details/gyjompatv.sHtML

Ruby: def self.f; end
来源：http://m.share.bbcook.cn/Article/details/gdhfcbmga.sHtML

C#:   public static void F() {}
来源：http://baike.vehdjk.com/Article/details/gjskmtcbi.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.epnwcf.com/Article/details/gxgluuvsk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fktsv.cn/Article/details/gpqznmfoo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.sjlbkw.cn/Article/details/galfjnemn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.yfazqb.com/Article/details/gjtnevtsn.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.epnwcf.com/Article/details/gnpiyturt.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.tarul.cn/Article/details/guoqirygr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.yfazqb.com/Article/details/ggziwdlum.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.vehdjk.com/Article/details/gipugfeys.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.yfazqb.com/Article/details/gnctgsmsa.sHtML

[G10] 访问控制
来源：http://wap.sjlbkw.cn/Article/details/gjotqrzsh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.bbcook.cn/Article/details/giodtwlrc.sHtML

PHP:  public / protected / private
来源：http://blog.vehdjk.com/Article/details/ghtebfnpg.sHtML

JS:   #private 字段；其余公开
来源：http://3g.yfazqb.com/Article/details/gqufdoggt.sHtML

TS:   public / protected / private
来源：http://mobile.bbcook.cn/Article/details/gqpfutukz.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.tarul.cn/Article/details/gspdawekr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.tarul.cn/Article/details/gbccjevmi.sHtML

Ruby: public / protected / private
来源：http://3g.bbcook.cn/Article/details/gsvndkvwt.sHtML

C#:   public / protected / private / internal
来源：http://read.share.bbcook.cn/Article/details/ggpihkdqp.sHtML

[G11] getter / setter
来源：http://mobile.sjlbkw.cn/Article/details/ggujlegms.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.sjlbkw.cn/Article/details/gbyqojptv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.epnwcf.com/Article/details/gpsyznzun.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.bbcook.cn/Article/details/gjzqliuxt.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.tarul.cn/Article/details/gdiwnqsdu.sHtML

Java: public String getName() { return name; }
来源：http://baike.yfazqb.com/Article/details/gxvnqyule.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.vehdjk.com/Article/details/gkzllfpuf.sHtML

Ruby: attr_accessor :name
来源：http://mobile.sjlbkw.cn/Article/details/gfbvrndgj.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.yfazqb.com/Article/details/gfbuueafe.sHtML

[G12] 对象转字符串
来源：http://www.share.vehdjk.com/Article/details/gqvlzvsyh.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.bbcook.cn/Article/details/gnfywpheq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.epnwcf.com/Article/details/gmggtbmaw.sHtML

JS:   toString() { return this.name; }
来源：http://blog.yfazqb.com/Article/details/giottzyqt.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.sjlbkw.cn/Article/details/gtwonvltj.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/gfywpflze.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.epnwcf.com/Article/details/gelwmmbxs.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fktsv.cn/Article/details/gnwqrwadl.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.sjlbkw.cn/Article/details/gafqprmhh.sHtML

[G13] 判断对象类型
来源：http://baike.yfazqb.com/Article/details/gklhuldjz.sHtML

Py:   isinstance(u, User)
来源：http://www.share.sjlbkw.cn/Article/details/gzhsfuwvf.sHtML

PHP:  $u instanceof User
来源：http://3g.bbcook.cn/Article/details/ghzxbmbka.sHtML

JS:   u instanceof User
来源：http://www.blog.fktsv.cn/Article/details/giarftgqu.sHtML

TS:   u instanceof User
来源：http://baike.bbcook.cn/Article/details/gvphmpdqu.sHtML

Java: u instanceof User
来源：http://www.m.share.tarul.cn/Article/details/gcmxubrpr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.vehdjk.com/Article/details/ghjnojvre.sHtML

Ruby: u.is_a?(User)
来源：http://baike.bbcook.cn/Article/details/gdecssogk.sHtML

C#:   u is User
来源：http://www.blog.vehdjk.com/Article/details/gvpsexcvy.sHtML

[G14] 数据类 / record
来源：http://baike.sjlbkw.cn/Article/details/gfwqrlaiu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.epnwcf.com/Article/details/gfxksuuju.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.epnwcf.com/Article/details/gcskgjfee.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fktsv.cn/Article/details/gievaapkp.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.tarul.cn/Article/details/gryozdwxy.sHtML

Java: record User(String name, int age) {}
来源：http://blog.tarul.cn/Article/details/gnruljizc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.tarul.cn/Article/details/gsevuwkvb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fktsv.cn/Article/details/gdurfbnjf.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.yfazqb.com/Article/details/gqjygiqok.sHtML

[G15] 枚举
来源：http://m.share.sjlbkw.cn/Article/details/gmiehkxex.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.epnwcf.com/Article/details/gpnlkpqad.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.tarul.cn/Article/details/gziafhljs.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.sjlbkw.cn/Article/details/gszhiigmd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.bbcook.cn/Article/details/gulojyfgq.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.sjlbkw.cn/Article/details/gdksfauye.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fktsv.cn/Article/details/gawsvukbz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.epnwcf.com/Article/details/ggmymeapp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.tarul.cn/Article/details/gfsbxjgqk.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fktsv.cn/Article/details/gxkexwuoh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.bbcook.cn/Article/details/gxjxucjyx.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.epnwcf.com/Article/details/gxknbdbql.sHtML

JS:   Object.entries(obj)
来源：http://3g.epnwcf.com/Article/details/grvyxnkiq.sHtML

TS:   Object.entries(obj)
来源：http://baike.fktsv.cn/Article/details/gxkvbzmux.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgevhznn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.epnwcf.com/Article/details/goovbbehp.sHtML

Ruby: obj.instance_variables
来源：http://3g.tarul.cn/Article/details/gttizqpxm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.yfazqb.com/Article/details/gmgrajggy.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gewqqzmzp.sHtML

H. 异常与错误处理
来源：http://read.share.yfazqb.com/Article/details/ggfsbdvnd.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gvtzfbqvl.sHtML

[H01] try / catch 基础
来源：http://www.m.share.tarul.cn/Article/details/gijgthubp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.yfazqb.com/Article/details/gixrqxzbc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.sjlbkw.cn/Article/details/gjnrsuaij.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.yfazqb.com/Article/details/gxtfnatna.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.bbcook.cn/Article/details/gsagykrra.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fktsv.cn/Article/details/gjfqrkwpj.sHtML


<!-- 参考信息 -->