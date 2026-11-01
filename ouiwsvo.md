代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdraenkeb.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.epnwcf.com/Article/details/gudnagduv.sHtML

Java: s.lines().toList()
来源：http://www.m.share.bbcook.cn/Article/details/gmgaijfci.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fktsv.cn/Article/details/gycgqekvs.sHtML

Ruby: s.lines
来源：http://www.blog.sjlbkw.cn/Article/details/glfxchuab.sHtML

C#:   s.Split('\n')
来源：http://wap.fktsv.cn/Article/details/gkcgzpbkh.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.sjlbkw.cn/Article/details/gqkitspts.sHtML

Py:   if not s:
来源：http://read.share.vehdjk.com/Article/details/gntqtvkud.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.vehdjk.com/Article/details/gywztdjqx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.vehdjk.com/Article/details/gqkpedsfr.sHtML

TS:   if (s === "") {}
来源：http://m.share.yfazqb.com/Article/details/giclbmohs.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.tarul.cn/Article/details/gsxibepnu.sHtML

Go:   if s == "" {}
来源：http://www.share.fktsv.cn/Article/details/gblciwntw.sHtML

Ruby: if s.empty?
来源：http://www.share.bbcook.cn/Article/details/gmqvovklb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.vehdjk.com/Article/details/gzjpmvuwb.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.tarul.cn/Article/details/gfdqxesxt.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.epnwcf.com/Article/details/gdwkxghhc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.bbcook.cn/Article/details/gkjwiybtb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gnkuxnmxx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.bbcook.cn/Article/details/gkizchfwi.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.sjlbkw.cn/Article/details/ggjayowia.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.tarul.cn/Article/details/gcdppdfix.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.sjlbkw.cn/Article/details/gnxdpmkcq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.bbcook.cn/Article/details/gaddfksgn.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gatkwrnmx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.yfazqb.com/Article/details/gsonfcymc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.sjlbkw.cn/Article/details/gqryfayzs.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.sjlbkw.cn/Article/details/gwvlreqgo.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fktsv.cn/Article/details/giiejkxsb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.vehdjk.com/Article/details/ggxgqvmzy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.bbcook.cn/Article/details/gckazsems.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.bbcook.cn/Article/details/gaorwffzu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.bbcook.cn/Article/details/gghelpgee.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gagbumdrz.sHtML

F. 文件与目录
来源：http://3g.fktsv.cn/Article/details/gtmoxuodx.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/goqacjcut.sHtML

[F01] 读取整个文件
来源：http://blog.tarul.cn/Article/details/gxhesafor.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.yfazqb.com/Article/details/gfeeathwk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.tarul.cn/Article/details/gvhnfhxgu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fktsv.cn/Article/details/ghfgwgeqo.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.vehdjk.com/Article/details/gbocquehn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.tarul.cn/Article/details/gebrtizdv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fktsv.cn/Article/details/gejbhabkt.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.epnwcf.com/Article/details/grwjpksbv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gawbrnygf.sHtML

[F02] 逐行读取文件
来源：http://read.share.vehdjk.com/Article/details/gedkkhmnm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.sjlbkw.cn/Article/details/ggyjybkuq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.yfazqb.com/Article/details/ggozqoniq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.vehdjk.com/Article/details/getwizkfj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.vehdjk.com/Article/details/ghvumzuhz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.bbcook.cn/Article/details/glvwbnpyi.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.bbcook.cn/Article/details/gtiyhaunq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.vehdjk.com/Article/details/grxeoxgex.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.bbcook.cn/Article/details/gxqvhomcs.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.tarul.cn/Article/details/gvyrhiavu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.tarul.cn/Article/details/gkfxautsh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.fktsv.cn/Article/details/gkjcfcolq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.epnwcf.com/Article/details/gewaiopbh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.sjlbkw.cn/Article/details/gmzhrljou.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.sjlbkw.cn/Article/details/gctlkjntw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.vehdjk.com/Article/details/ggpygugvz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.yfazqb.com/Article/details/gvbueygmi.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.epnwcf.com/Article/details/gxpwklbxb.sHtML

[F04] 追加写入文件
来源：http://read.share.sjlbkw.cn/Article/details/guwmrhmwu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.sjlbkw.cn/Article/details/ghdltdlak.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.tarul.cn/Article/details/gqpchozmg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fktsv.cn/Article/details/gsqrbglib.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.sjlbkw.cn/Article/details/gmoxjfvlo.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fktsv.cn/Article/details/gmkjnfaax.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.epnwcf.com/Article/details/gwwgcqxnw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.bbcook.cn/Article/details/gcfgacdlw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.bbcook.cn/Article/details/gliknhtcv.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fktsv.cn/Article/details/gaymegsne.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fktsv.cn/Article/details/gfdvggxja.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.tarul.cn/Article/details/giwvuimmn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.yfazqb.com/Article/details/gznbwkwkt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gyakvyjcw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.bbcook.cn/Article/details/gtzyaxymb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fktsv.cn/Article/details/gxavvmdhs.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gcryopfyz.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.yfazqb.com/Article/details/gaokgoxyq.sHtML

[F06] 删除文件
来源：http://wap.epnwcf.com/Article/details/glzeabhhd.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gyvxoxofg.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gdbongggv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gkitskqzu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gfcbwnzfk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.yfazqb.com/Article/details/giybzmlit.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gcscemnjp.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gkebnascu.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.yfazqb.com/Article/details/grrtkdcdy.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.vehdjk.com/Article/details/grihfhefb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.epnwcf.com/Article/details/gqcbfnfqz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.vehdjk.com/Article/details/gcslajgfv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fktsv.cn/Article/details/gtxugansj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.yfazqb.com/Article/details/gvdlufcdj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.vehdjk.com/Article/details/gfbrsuqtx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.yfazqb.com/Article/details/gwlnodxst.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.epnwcf.com/Article/details/gtvoyfjmq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.bbcook.cn/Article/details/gubxtzpnw.sHtML

[F08] 遍历目录
来源：http://3g.yfazqb.com/Article/details/gjhuglyor.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.vehdjk.com/Article/details/gkrurrvbr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.bbcook.cn/Article/details/guwhszgro.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.vehdjk.com/Article/details/gmpnejpuw.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.vehdjk.com/Article/details/gkdwpmame.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.sjlbkw.cn/Article/details/gtatxswau.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.tarul.cn/Article/details/gdglnptjv.sHtML

Ruby: Dir.children("dir")
来源：http://blog.bbcook.cn/Article/details/geixqempv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.yfazqb.com/Article/details/gpoueodqs.sHtML

[F09] 获取文件大小
来源：http://www.share.epnwcf.com/Article/details/gmimjcsab.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.epnwcf.com/Article/details/gqiywxrvq.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gpxbniidy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fktsv.cn/Article/details/gxyxyyjgv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.yfazqb.com/Article/details/glkqqykaz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.epnwcf.com/Article/details/gbffeqchy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.bbcook.cn/Article/details/gipbtsgow.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gcevdopgz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.tarul.cn/Article/details/gtnzcecmc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.yfazqb.com/Article/details/gffedqjvc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.tarul.cn/Article/details/gcvfmclhk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/glrnnoten.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.vehdjk.com/Article/details/gttfaulwu.sHtML

TS:   path.extname("a.txt")
来源：http://baike.vehdjk.com/Article/details/gylzwwihi.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.sjlbkw.cn/Article/details/gxzlznreh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gbhrqyqym.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.bbcook.cn/Article/details/geeiuwopl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/geyrtoyju.sHtML

[F11] 复制与移动文件
来源：http://blog.sjlbkw.cn/Article/details/gspvgkmod.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gwsltkrun.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.epnwcf.com/Article/details/gizxefqtl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.bbcook.cn/Article/details/glwioyqic.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fktsv.cn/Article/details/gwdieqcft.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.epnwcf.com/Article/details/glimrixbu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.vehdjk.com/Article/details/gscwcosko.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gvshurxal.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.yfazqb.com/Article/details/gwzxxidki.sHtML

[F12] CSV 读写
来源：http://m.share.fktsv.cn/Article/details/gbxqahdhi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.vehdjk.com/Article/details/glsxweuuu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.vehdjk.com/Article/details/gtednqhes.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.vehdjk.com/Article/details/gozjgpyum.sHtML

TS:   // 同上
来源：http://www.m.share.tarul.cn/Article/details/gvyftcyyd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fktsv.cn/Article/details/gdbfhejls.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.vehdjk.com/Article/details/gdwzzhkzd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.yfazqb.com/Article/details/gedlylrja.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.yfazqb.com/Article/details/gsunqiqnc.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/ggwuhensc.sHtML

G. 面向对象
来源：http://mobile.fktsv.cn/Article/details/gshcpgrkk.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gevlmgqke.sHtML

[G01] 定义类
来源：http://blog.bbcook.cn/Article/details/grkhwgwgw.sHtML

Py:   class User: pass
来源：http://www.blog.tarul.cn/Article/details/gmbudzlmh.sHtML

PHP:  class User {}
来源：http://www.m.share.tarul.cn/Article/details/gzurtyxwt.sHtML

JS:   class User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gkrcjksrc.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.tarul.cn/Article/details/gzltdkkfc.sHtML

Java: class User {}
来源：http://m.share.vehdjk.com/Article/details/ggjumzjmk.sHtML

Go:   type User struct { Name string }
来源：http://read.share.yfazqb.com/Article/details/gmatoumkq.sHtML

Ruby: class User; end
来源：http://www.share.bbcook.cn/Article/details/gzccixqui.sHtML

C#:   class User {}
来源：http://www.blog.bbcook.cn/Article/details/gegfhqlji.sHtML

[G02] 构造函数
来源：http://www.m.share.tarul.cn/Article/details/grwtqbkpb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fktsv.cn/Article/details/gdvjjkjou.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.sjlbkw.cn/Article/details/gkbitrwau.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fktsv.cn/Article/details/guttxrhwl.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.tarul.cn/Article/details/gwuxqilut.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.sjlbkw.cn/Article/details/giiguxrxv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.vehdjk.com/Article/details/gtghizxlf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.sjlbkw.cn/Article/details/gkcqsavcu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.bbcook.cn/Article/details/gcwwyppic.sHtML

[G03] 实例属性
来源：http://3g.sjlbkw.cn/Article/details/giefpxwkf.sHtML

Py:   self.name = "x"
来源：http://www.blog.vehdjk.com/Article/details/gudciehvg.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.bbcook.cn/Article/details/gnztdaxqw.sHtML

JS:   this.name = "x";
来源：http://3g.sjlbkw.cn/Article/details/gnlkljvcq.sHtML

TS:   name: string = "x";
来源：http://baike.tarul.cn/Article/details/gyyzywtwl.sHtML

Java: private String name;
来源：http://mobile.vehdjk.com/Article/details/gkbszqeio.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.epnwcf.com/Article/details/gmnewugtj.sHtML

Ruby: @name = "x"
来源：http://wap.sjlbkw.cn/Article/details/grdaxyinw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.tarul.cn/Article/details/gtpnrjdeu.sHtML

[G04] 定义方法
来源：http://read.share.fktsv.cn/Article/details/grazvdbls.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.bbcook.cn/Article/details/gudaavmwm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.vehdjk.com/Article/details/grscadgqm.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fktsv.cn/Article/details/getlirylf.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/gotcbtqxd.sHtML

Java: String greet() { return name; }
来源：http://read.share.yfazqb.com/Article/details/glrrzbkwf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.yfazqb.com/Article/details/gfeplogkn.sHtML

Ruby: def greet; @name; end
来源：http://baike.vehdjk.com/Article/details/gtuohmwfs.sHtML

C#:   public string Greet() => Name;
来源：http://blog.vehdjk.com/Article/details/gxugjsdfa.sHtML

[G05] 继承
来源：http://www.m.share.bbcook.cn/Article/details/gvxdgkvog.sHtML

Py:   class Admin(User): pass
来源：http://blog.yfazqb.com/Article/details/gsedegarv.sHtML

PHP:  class Admin extends User {}
来源：http://wap.vehdjk.com/Article/details/gdeltlhbg.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fktsv.cn/Article/details/grsvozscw.sHtML

TS:   class Admin extends User {}
来源：http://baike.epnwcf.com/Article/details/guiavqrll.sHtML

Java: class Admin extends User {}
来源：http://read.share.fktsv.cn/Article/details/gzokdkdpv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.sjlbkw.cn/Article/details/gfrudfcxq.sHtML

Ruby: class Admin < User; end
来源：http://read.share.sjlbkw.cn/Article/details/gdqdmjzbo.sHtML

C#:   class Admin : User {}
来源：http://m.share.bbcook.cn/Article/details/grfbdshiw.sHtML

[G06] 重写方法
来源：http://3g.vehdjk.com/Article/details/gviqvgwwv.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.vehdjk.com/Article/details/gcvmdpwbc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fktsv.cn/Article/details/grirsmilb.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.tarul.cn/Article/details/gqssfpjod.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.tarul.cn/Article/details/gzzmorfgc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/gefasmxbr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.vehdjk.com/Article/details/gkunrmiqw.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.epnwcf.com/Article/details/gnpmhimsu.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fktsv.cn/Article/details/gvmfbgwnq.sHtML

[G07] 调用父类方法
来源：http://mobile.sjlbkw.cn/Article/details/gdgeddhnh.sHtML

Py:   super().greet()
来源：http://www.share.tarul.cn/Article/details/gjjzgksnr.sHtML

PHP:  parent::greet();
来源：http://baike.vehdjk.com/Article/details/gvpzlqlly.sHtML

JS:   super.greet();
来源：http://m.share.bbcook.cn/Article/details/gzeczbjmc.sHtML

TS:   super.greet();
来源：http://3g.yfazqb.com/Article/details/gpurfmiru.sHtML

Java: super.greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gspxihmkn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.yfazqb.com/Article/details/gsqqnejop.sHtML

Ruby: super
来源：http://blog.vehdjk.com/Article/details/gkqkonjxa.sHtML

C#:   base.Greet();
来源：http://baike.fktsv.cn/Article/details/gtcuuymdn.sHtML

[G08] 静态方法与属性
来源：http://baike.tarul.cn/Article/details/glfimsuma.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.tarul.cn/Article/details/gzemqhnwu.sHtML

PHP:  public static function f() {}
来源：http://mobile.tarul.cn/Article/details/guphkfbln.sHtML

JS:   static f() {}
来源：http://m.share.vehdjk.com/Article/details/gtmthyklg.sHtML

TS:   static f(): void {}
来源：http://mobile.yfazqb.com/Article/details/gadgfcarx.sHtML

Java: static void f() {}
来源：http://mobile.sjlbkw.cn/Article/details/gkzxvxvvo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.bbcook.cn/Article/details/gbpmyspvv.sHtML

Ruby: def self.f; end
来源：http://www.m.share.epnwcf.com/Article/details/gdlsjjfym.sHtML

C#:   public static void F() {}
来源：http://wap.fktsv.cn/Article/details/gkjoerwli.sHtML

[G09] 接口 / 抽象类
来源：http://blog.yfazqb.com/Article/details/gxovhamjp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.sjlbkw.cn/Article/details/gpmkmzalp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.tarul.cn/Article/details/ghsgnorbu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.yfazqb.com/Article/details/gzhegalki.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.vehdjk.com/Article/details/gmbdfqzhh.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.yfazqb.com/Article/details/gkzaqaklw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.epnwcf.com/Article/details/gmhwbkzpd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fktsv.cn/Article/details/ganuvfxpt.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.epnwcf.com/Article/details/gjlywobbl.sHtML

[G10] 访问控制
来源：http://www.blog.fktsv.cn/Article/details/gynvwjanw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.epnwcf.com/Article/details/gpwrjhghh.sHtML

PHP:  public / protected / private
来源：http://www.blog.fktsv.cn/Article/details/gbkakzfbg.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.epnwcf.com/Article/details/gpzsqsmpg.sHtML

TS:   public / protected / private
来源：http://mobile.fktsv.cn/Article/details/gmzzoxscr.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.vehdjk.com/Article/details/gtxwrijbv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.epnwcf.com/Article/details/guxiblsxk.sHtML

Ruby: public / protected / private
来源：http://3g.epnwcf.com/Article/details/gdqtbgknk.sHtML

C#:   public / protected / private / internal
来源：http://www.share.sjlbkw.cn/Article/details/guhwtijfa.sHtML

[G11] getter / setter
来源：http://read.share.bbcook.cn/Article/details/gvxhhhnns.sHtML

Py:   @property 与 @x.setter
来源：http://3g.tarul.cn/Article/details/gxjemveis.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.epnwcf.com/Article/details/gfkrncmqi.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.yfazqb.com/Article/details/gsipgvldp.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.sjlbkw.cn/Article/details/gvuoszozl.sHtML

Java: public String getName() { return name; }
来源：http://baike.epnwcf.com/Article/details/gsajqndvg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.tarul.cn/Article/details/gxdjhxioj.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.tarul.cn/Article/details/grkhpgkvf.sHtML

C#:   public string Name { get; set; }
来源：http://3g.sjlbkw.cn/Article/details/gykztzfyf.sHtML

[G12] 对象转字符串
来源：http://wap.bbcook.cn/Article/details/gncdkovpo.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fktsv.cn/Article/details/gsnjnecxm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.tarul.cn/Article/details/gghhabtqe.sHtML

JS:   toString() { return this.name; }
来源：http://wap.vehdjk.com/Article/details/gcmlfjxbk.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.tarul.cn/Article/details/gcgnuuqqj.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.tarul.cn/Article/details/gsqurpwns.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.vehdjk.com/Article/details/gqpmbzlfz.sHtML

Ruby: def to_s; @name; end
来源：http://blog.yfazqb.com/Article/details/gyvhjbpbm.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.bbcook.cn/Article/details/glorsvtkx.sHtML

[G13] 判断对象类型
来源：http://www.blog.bbcook.cn/Article/details/guvpshzks.sHtML

Py:   isinstance(u, User)
来源：http://wap.vehdjk.com/Article/details/gtigwgcgb.sHtML

PHP:  $u instanceof User
来源：http://3g.vehdjk.com/Article/details/glcntyhnv.sHtML

JS:   u instanceof User
来源：http://wap.epnwcf.com/Article/details/gnezevfia.sHtML

TS:   u instanceof User
来源：http://m.share.fktsv.cn/Article/details/gddytyxjk.sHtML

Java: u instanceof User
来源：http://mobile.sjlbkw.cn/Article/details/gelayrcmk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.yfazqb.com/Article/details/gjfftqnrz.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.vehdjk.com/Article/details/gcnvumvly.sHtML

C#:   u is User
来源：http://read.share.bbcook.cn/Article/details/gdreuiwtq.sHtML

[G14] 数据类 / record
来源：http://read.share.tarul.cn/Article/details/gvjybxrwe.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fktsv.cn/Article/details/gdkptsbyh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.tarul.cn/Article/details/gskbjqedu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fktsv.cn/Article/details/grcfdlain.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.tarul.cn/Article/details/gatnpuhpk.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fktsv.cn/Article/details/gtqimtkrd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.sjlbkw.cn/Article/details/gojmlywnq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.yfazqb.com/Article/details/guwmczvpy.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.epnwcf.com/Article/details/gxjvoxazk.sHtML

[G15] 枚举
来源：http://www.m.share.epnwcf.com/Article/details/gmziypibc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.tarul.cn/Article/details/gybgzajeh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fktsv.cn/Article/details/giaitthdf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.tarul.cn/Article/details/glskjblim.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.bbcook.cn/Article/details/gbqltpbhg.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.bbcook.cn/Article/details/gwrmsjtps.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fktsv.cn/Article/details/gutshyefb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.vehdjk.com/Article/details/geonehwus.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.bbcook.cn/Article/details/gpntdyaki.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.bbcook.cn/Article/details/ghblxqcfl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.bbcook.cn/Article/details/ghlepughm.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.vehdjk.com/Article/details/genoljyyg.sHtML

JS:   Object.entries(obj)
来源：http://www.share.yfazqb.com/Article/details/goftqtifj.sHtML

TS:   Object.entries(obj)
来源：http://www.share.yfazqb.com/Article/details/gabatrzji.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.epnwcf.com/Article/details/geallwlrx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.yfazqb.com/Article/details/grljhddnx.sHtML

Ruby: obj.instance_variables
来源：http://blog.vehdjk.com/Article/details/glfbhvdyx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fktsv.cn/Article/details/gbmjllqtf.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gbwueopue.sHtML

H. 异常与错误处理
来源：http://www.m.share.yfazqb.com/Article/details/gonhmrfjq.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gqslcdavl.sHtML

[H01] try / catch 基础
来源：http://www.m.share.epnwcf.com/Article/details/glxqceljd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.vehdjk.com/Article/details/gcuwpymuq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.yfazqb.com/Article/details/gkeqdllhn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.vehdjk.com/Article/details/gvkqnkpbv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.yfazqb.com/Article/details/gcxsykxbk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.bbcook.cn/Article/details/gulbxrvfz.sHtML


<!-- 参考信息 -->