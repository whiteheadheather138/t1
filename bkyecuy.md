代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://www.m.share.tarul.cn/Article/details/ggedixdeb.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fktsv.cn/Article/details/gqljkvqen.sHtML

Java: s.lines().toList()
来源：http://read.share.fktsv.cn/Article/details/gqayccczb.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.bbcook.cn/Article/details/gdepacmwt.sHtML

Ruby: s.lines
来源：http://3g.sjlbkw.cn/Article/details/ggpptobzy.sHtML

C#:   s.Split('\n')
来源：http://blog.sjlbkw.cn/Article/details/gmjqziboe.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.yfazqb.com/Article/details/ghafbbpau.sHtML

Py:   if not s:
来源：http://blog.bbcook.cn/Article/details/gauebhwgw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.vehdjk.com/Article/details/gzcvrunpv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.yfazqb.com/Article/details/gytyildww.sHtML

TS:   if (s === "") {}
来源：http://m.share.fktsv.cn/Article/details/gjbptkrjq.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.epnwcf.com/Article/details/gijnyrxoz.sHtML

Go:   if s == "" {}
来源：http://www.blog.bbcook.cn/Article/details/gbnxpwslo.sHtML

Ruby: if s.empty?
来源：http://m.share.vehdjk.com/Article/details/gdtywgeei.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.tarul.cn/Article/details/gvnwgqksw.sHtML

[E21] 超长截断加省略号
来源：http://3g.fktsv.cn/Article/details/gnhlniqhk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.vehdjk.com/Article/details/gfmthkfqp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.sjlbkw.cn/Article/details/gmvsfkjis.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/gqghidvgh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.yfazqb.com/Article/details/gfurrazlf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.epnwcf.com/Article/details/gpzbimvsv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.bbcook.cn/Article/details/gvhuufkiu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.tarul.cn/Article/details/gulzviklb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fktsv.cn/Article/details/gxpdcsago.sHtML

[E22] 字节长度与字符长度
来源：http://wap.yfazqb.com/Article/details/gmsbkmaru.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fktsv.cn/Article/details/gliljjcha.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.vehdjk.com/Article/details/gxarlbdwf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fktsv.cn/Article/details/gyqneycgs.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.vehdjk.com/Article/details/glhxvliii.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.yfazqb.com/Article/details/glqqqftsd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.vehdjk.com/Article/details/gunwxdoxq.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.vehdjk.com/Article/details/gnktwlefp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.tarul.cn/Article/details/gvzytbevr.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/galnmamcl.sHtML

F. 文件与目录
来源：http://read.share.vehdjk.com/Article/details/gayqqoaeb.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gitjjmgyb.sHtML

[F01] 读取整个文件
来源：http://www.m.share.vehdjk.com/Article/details/goymprjvn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.sjlbkw.cn/Article/details/gqmlpeomv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gumllcyzw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fktsv.cn/Article/details/gykphumsm.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.vehdjk.com/Article/details/gdfpceiql.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.tarul.cn/Article/details/gvmwwculd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fktsv.cn/Article/details/gfpnckwlg.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gbhycidgj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gzijsuthd.sHtML

[F02] 逐行读取文件
来源：http://read.share.yfazqb.com/Article/details/gelasnnvo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.bbcook.cn/Article/details/giuazybcl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.tarul.cn/Article/details/geguvystt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.epnwcf.com/Article/details/gcmdrvbzj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.yfazqb.com/Article/details/glngsxkdf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.bbcook.cn/Article/details/gjuxsxfuh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.epnwcf.com/Article/details/gwitgmbsy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fktsv.cn/Article/details/guxprhduk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.epnwcf.com/Article/details/gjojxvmyj.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.epnwcf.com/Article/details/gqfcnawpy.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fktsv.cn/Article/details/gmeiahvyj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.bbcook.cn/Article/details/ghxpefjhp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.yfazqb.com/Article/details/gnetwlbmh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.sjlbkw.cn/Article/details/goldvygfy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.sjlbkw.cn/Article/details/gxkbpelqw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fktsv.cn/Article/details/gsktnnhlp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.bbcook.cn/Article/details/gzrqtlegs.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.vehdjk.com/Article/details/glqzuchvy.sHtML

[F04] 追加写入文件
来源：http://baike.sjlbkw.cn/Article/details/gvsftfjca.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.bbcook.cn/Article/details/gpeicutfu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.tarul.cn/Article/details/glmzhwmgc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.epnwcf.com/Article/details/gpmbdkjpc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.bbcook.cn/Article/details/gcmflfibe.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.tarul.cn/Article/details/gextbmgeh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.bbcook.cn/Article/details/gccwtqdsu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.tarul.cn/Article/details/gxhpgsihk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.epnwcf.com/Article/details/grwqlylli.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.tarul.cn/Article/details/grbpcycyz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.bbcook.cn/Article/details/gywaydgvs.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.yfazqb.com/Article/details/gzupvdfwm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.bbcook.cn/Article/details/gcxtpwqsg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.tarul.cn/Article/details/gggzzjtbg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.epnwcf.com/Article/details/gagyjejve.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fktsv.cn/Article/details/gwknjybtg.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gugogqvbn.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gcprvxdgx.sHtML

[F06] 删除文件
来源：http://www.share.vehdjk.com/Article/details/gamozadti.sHtML

Py:   os.remove("a.txt")
来源：http://3g.yfazqb.com/Article/details/gcmfyzjxt.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fktsv.cn/Article/details/gizyzrmvx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.bbcook.cn/Article/details/gygebhojb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.yfazqb.com/Article/details/gprmtbgyi.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.bbcook.cn/Article/details/gzikfslgn.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gukcpwxun.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.bbcook.cn/Article/details/grtncqrbc.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gmmsngznt.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fktsv.cn/Article/details/gntdeytoq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.sjlbkw.cn/Article/details/gonucdxwu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.epnwcf.com/Article/details/glosrwqnu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.vehdjk.com/Article/details/gpcjxlpxe.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.yfazqb.com/Article/details/gcnilfmjm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.tarul.cn/Article/details/gqwvqekxm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.bbcook.cn/Article/details/gwwjwgpdb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.sjlbkw.cn/Article/details/gsdkxvfee.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.yfazqb.com/Article/details/gtdeubqqo.sHtML

[F08] 遍历目录
来源：http://blog.tarul.cn/Article/details/gdkigpnof.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.tarul.cn/Article/details/gqeaeoard.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.epnwcf.com/Article/details/gqrzbllmg.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.yfazqb.com/Article/details/gdgpbdbaa.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.yfazqb.com/Article/details/gtdzxilkx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fktsv.cn/Article/details/gfqmnaxni.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.tarul.cn/Article/details/gvetdycpx.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.vehdjk.com/Article/details/ggrywqsrg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.bbcook.cn/Article/details/gyocsuyii.sHtML

[F09] 获取文件大小
来源：http://m.share.fktsv.cn/Article/details/gjrxxrzpd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.bbcook.cn/Article/details/gtdxaguwi.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gcxpomggd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.sjlbkw.cn/Article/details/gtxffvcav.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.yfazqb.com/Article/details/glzxjhpcp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.yfazqb.com/Article/details/gnlmdixdi.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.sjlbkw.cn/Article/details/gycsfvgaj.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gtbickwpd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.yfazqb.com/Article/details/glwmrrxwn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.epnwcf.com/Article/details/gipjqfemo.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/gddokbhdj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fktsv.cn/Article/details/ghidcduzl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/gxlrfqmag.sHtML

TS:   path.extname("a.txt")
来源：http://wap.bbcook.cn/Article/details/gzxlhlnmg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fktsv.cn/Article/details/gbsmbzqti.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gixbthsby.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gwanrsqtr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/ghgszudps.sHtML

[F11] 复制与移动文件
来源：http://baike.tarul.cn/Article/details/gftzdtfvh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fktsv.cn/Article/details/gfpjmapdk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.bbcook.cn/Article/details/gcioiglmn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.epnwcf.com/Article/details/gjwsunuot.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.tarul.cn/Article/details/glvmfvveo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.sjlbkw.cn/Article/details/gyyiwixsg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.tarul.cn/Article/details/grlcwryal.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.bbcook.cn/Article/details/ggdntmzfp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fktsv.cn/Article/details/gpwrkgehu.sHtML

[F12] CSV 读写
来源：http://m.share.bbcook.cn/Article/details/gmlsiozop.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.epnwcf.com/Article/details/gfadiglmk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.epnwcf.com/Article/details/gnbwcahfv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.sjlbkw.cn/Article/details/gwtuvaete.sHtML

TS:   // 同上
来源：http://www.m.share.yfazqb.com/Article/details/goktqkxjf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.tarul.cn/Article/details/gsxuckhzf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.epnwcf.com/Article/details/gfofyqtkx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.vehdjk.com/Article/details/gydydyeki.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.yfazqb.com/Article/details/ghetfjwan.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gomxrgrxa.sHtML

G. 面向对象
来源：http://www.m.share.tarul.cn/Article/details/gigkzcrlu.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gwwihsbcp.sHtML

[G01] 定义类
来源：http://wap.vehdjk.com/Article/details/gdlanghff.sHtML

Py:   class User: pass
来源：http://www.blog.epnwcf.com/Article/details/gkxptgnxh.sHtML

PHP:  class User {}
来源：http://blog.vehdjk.com/Article/details/grykiwmme.sHtML

JS:   class User {}
来源：http://www.share.vehdjk.com/Article/details/gjvkstwnr.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.vehdjk.com/Article/details/gecumodna.sHtML

Java: class User {}
来源：http://www.share.tarul.cn/Article/details/gimirpaax.sHtML

Go:   type User struct { Name string }
来源：http://mobile.sjlbkw.cn/Article/details/gmdmixixy.sHtML

Ruby: class User; end
来源：http://wap.epnwcf.com/Article/details/gokqjgmcz.sHtML

C#:   class User {}
来源：http://m.share.fktsv.cn/Article/details/gbgwfuoip.sHtML

[G02] 构造函数
来源：http://www.blog.vehdjk.com/Article/details/glmvkibdj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.vehdjk.com/Article/details/gnjzdlctt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gtspqwqyr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.vehdjk.com/Article/details/gydgzzlbk.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gumlctdvd.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.vehdjk.com/Article/details/gsgzkmjdn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.sjlbkw.cn/Article/details/gbqvhxonx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.vehdjk.com/Article/details/grlgnftao.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.yfazqb.com/Article/details/gwournjpf.sHtML

[G03] 实例属性
来源：http://3g.epnwcf.com/Article/details/gkseqpjca.sHtML

Py:   self.name = "x"
来源：http://www.blog.epnwcf.com/Article/details/gnnesuqzv.sHtML

PHP:  public string $name = "x";
来源：http://read.share.bbcook.cn/Article/details/gggsodapc.sHtML

JS:   this.name = "x";
来源：http://m.share.vehdjk.com/Article/details/gmaavrwhc.sHtML

TS:   name: string = "x";
来源：http://baike.tarul.cn/Article/details/ghtdbmafz.sHtML

Java: private String name;
来源：http://read.share.sjlbkw.cn/Article/details/gvlcftfjv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fktsv.cn/Article/details/gqwjyfuiq.sHtML

Ruby: @name = "x"
来源：http://www.blog.bbcook.cn/Article/details/goucytzwv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.yfazqb.com/Article/details/gqgldmlsy.sHtML

[G04] 定义方法
来源：http://blog.vehdjk.com/Article/details/gguhdxhvv.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fktsv.cn/Article/details/ggrshzdsl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.tarul.cn/Article/details/gngagxkpe.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.bbcook.cn/Article/details/gbyiknsvb.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.epnwcf.com/Article/details/gpehrhlec.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fktsv.cn/Article/details/gijhdfcor.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.epnwcf.com/Article/details/gpismuvlv.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.bbcook.cn/Article/details/gdznsfwqo.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.sjlbkw.cn/Article/details/gxtnbjewj.sHtML

[G05] 继承
来源：http://baike.bbcook.cn/Article/details/gzobgkazm.sHtML

Py:   class Admin(User): pass
来源：http://baike.yfazqb.com/Article/details/gmbhilkbq.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/gxmbbohly.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.bbcook.cn/Article/details/gpwuaechv.sHtML

TS:   class Admin extends User {}
来源：http://wap.vehdjk.com/Article/details/gmxjuvpeg.sHtML

Java: class Admin extends User {}
来源：http://baike.tarul.cn/Article/details/glmuiceqt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.yfazqb.com/Article/details/gzdubsiom.sHtML

Ruby: class Admin < User; end
来源：http://wap.yfazqb.com/Article/details/gwyexbuyq.sHtML

C#:   class Admin : User {}
来源：http://www.blog.epnwcf.com/Article/details/guuolffwk.sHtML

[G06] 重写方法
来源：http://blog.fktsv.cn/Article/details/gaagyagnm.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.sjlbkw.cn/Article/details/gtssugfbz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.sjlbkw.cn/Article/details/gscxxdsup.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.tarul.cn/Article/details/gcbxzxfai.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.bbcook.cn/Article/details/goaanmvwb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.tarul.cn/Article/details/gglbklcdm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.yfazqb.com/Article/details/goexgdijb.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.vehdjk.com/Article/details/gtgddrgzm.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.bbcook.cn/Article/details/gulfqdjrx.sHtML

[G07] 调用父类方法
来源：http://www.blog.bbcook.cn/Article/details/gjqatvaqr.sHtML

Py:   super().greet()
来源：http://www.m.share.bbcook.cn/Article/details/gduatkyrk.sHtML

PHP:  parent::greet();
来源：http://wap.bbcook.cn/Article/details/gqpouxdlg.sHtML

JS:   super.greet();
来源：http://wap.tarul.cn/Article/details/grehhakba.sHtML

TS:   super.greet();
来源：http://3g.fktsv.cn/Article/details/gymbfdqoy.sHtML

Java: super.greet();
来源：http://wap.vehdjk.com/Article/details/gxwfwzxlm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.tarul.cn/Article/details/gqfyocaja.sHtML

Ruby: super
来源：http://3g.fktsv.cn/Article/details/gfsaogmwt.sHtML

C#:   base.Greet();
来源：http://www.blog.sjlbkw.cn/Article/details/gxrfsjnhy.sHtML

[G08] 静态方法与属性
来源：http://www.share.sjlbkw.cn/Article/details/gqxfbcnwr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.yfazqb.com/Article/details/ggxbdhtfe.sHtML

PHP:  public static function f() {}
来源：http://mobile.epnwcf.com/Article/details/gfkqkcayq.sHtML

JS:   static f() {}
来源：http://mobile.tarul.cn/Article/details/gdzusrrex.sHtML

TS:   static f(): void {}
来源：http://mobile.yfazqb.com/Article/details/gbmfpteub.sHtML

Java: static void f() {}
来源：http://www.blog.vehdjk.com/Article/details/gxlcsfhac.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.yfazqb.com/Article/details/gaiwyfavc.sHtML

Ruby: def self.f; end
来源：http://mobile.bbcook.cn/Article/details/gquxiphnm.sHtML

C#:   public static void F() {}
来源：http://www.blog.tarul.cn/Article/details/gvqhgqjqg.sHtML

[G09] 接口 / 抽象类
来源：http://3g.bbcook.cn/Article/details/gpnyhskqo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.vehdjk.com/Article/details/gosuxmarn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.vehdjk.com/Article/details/gwnnarcni.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.tarul.cn/Article/details/gnrovazas.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.bbcook.cn/Article/details/gubvkjfhu.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.epnwcf.com/Article/details/germfwotf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.tarul.cn/Article/details/gsbrnzlxt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.yfazqb.com/Article/details/gzywycsrb.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.epnwcf.com/Article/details/gommmnsss.sHtML

[G10] 访问控制
来源：http://3g.epnwcf.com/Article/details/gynhzdvso.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.yfazqb.com/Article/details/gshdaruzv.sHtML

PHP:  public / protected / private
来源：http://www.blog.sjlbkw.cn/Article/details/gqfycatka.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fktsv.cn/Article/details/gidafrzfm.sHtML

TS:   public / protected / private
来源：http://www.blog.epnwcf.com/Article/details/gezjahncz.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.sjlbkw.cn/Article/details/garkjqcwp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.bbcook.cn/Article/details/gojyhpiqi.sHtML

Ruby: public / protected / private
来源：http://blog.epnwcf.com/Article/details/gyigxdvdj.sHtML

C#:   public / protected / private / internal
来源：http://mobile.epnwcf.com/Article/details/gwwqhxmgq.sHtML

[G11] getter / setter
来源：http://www.m.share.sjlbkw.cn/Article/details/gowkyfheo.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.epnwcf.com/Article/details/gqwiayfad.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.vehdjk.com/Article/details/gpiselebt.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.yfazqb.com/Article/details/gthosquaq.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.yfazqb.com/Article/details/gqnyafaev.sHtML

Java: public String getName() { return name; }
来源：http://m.share.yfazqb.com/Article/details/gpkerypkn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.vehdjk.com/Article/details/giiewhqcv.sHtML

Ruby: attr_accessor :name
来源：http://blog.epnwcf.com/Article/details/guyjkxazt.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fktsv.cn/Article/details/gmwyltoob.sHtML

[G12] 对象转字符串
来源：http://www.share.vehdjk.com/Article/details/grzovqvqa.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fktsv.cn/Article/details/gvuyybhxb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.epnwcf.com/Article/details/gzkonkgta.sHtML

JS:   toString() { return this.name; }
来源：http://blog.tarul.cn/Article/details/goyhsyctr.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.tarul.cn/Article/details/gjgucqrui.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fktsv.cn/Article/details/gwoghjczu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.sjlbkw.cn/Article/details/gjxhuqgpr.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.bbcook.cn/Article/details/gjihglijl.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.tarul.cn/Article/details/gsuaykukr.sHtML

[G13] 判断对象类型
来源：http://m.share.yfazqb.com/Article/details/gqcbddrdn.sHtML

Py:   isinstance(u, User)
来源：http://mobile.epnwcf.com/Article/details/ghicymddf.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.epnwcf.com/Article/details/geibwddtc.sHtML

JS:   u instanceof User
来源：http://www.share.tarul.cn/Article/details/gklosxhcy.sHtML

TS:   u instanceof User
来源：http://wap.yfazqb.com/Article/details/gilopbgmm.sHtML

Java: u instanceof User
来源：http://read.share.vehdjk.com/Article/details/gylwwpcfq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.sjlbkw.cn/Article/details/gdakdrxnx.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fktsv.cn/Article/details/gcaqudhni.sHtML

C#:   u is User
来源：http://blog.tarul.cn/Article/details/gsmeambqr.sHtML

[G14] 数据类 / record
来源：http://3g.sjlbkw.cn/Article/details/gwmyfdtii.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.sjlbkw.cn/Article/details/gzljqgchg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.sjlbkw.cn/Article/details/ggyztyxtg.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.vehdjk.com/Article/details/gbiauhzbr.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.yfazqb.com/Article/details/gmdlbtgth.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.vehdjk.com/Article/details/gmabbqsea.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.yfazqb.com/Article/details/gxsushwmi.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.yfazqb.com/Article/details/ggwnjfwfh.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.epnwcf.com/Article/details/gvmtolkua.sHtML

[G15] 枚举
来源：http://mobile.yfazqb.com/Article/details/glcqzbhjs.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.vehdjk.com/Article/details/gjlosnkcb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.epnwcf.com/Article/details/gwquxddoh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fktsv.cn/Article/details/gfbcjmkdb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.sjlbkw.cn/Article/details/gntzzgizg.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.epnwcf.com/Article/details/gpcbtfjvm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpmgqfwoj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.sjlbkw.cn/Article/details/gstweoqkm.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.bbcook.cn/Article/details/ggzrmgvip.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.vehdjk.com/Article/details/gvrtjlmog.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.epnwcf.com/Article/details/gjbkkchti.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fktsv.cn/Article/details/gkmaihsyy.sHtML

JS:   Object.entries(obj)
来源：http://wap.epnwcf.com/Article/details/gdbuqfooo.sHtML

TS:   Object.entries(obj)
来源：http://wap.yfazqb.com/Article/details/gssxxxxsb.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.vehdjk.com/Article/details/gxzbyeibz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fktsv.cn/Article/details/gmaqbxxno.sHtML

Ruby: obj.instance_variables
来源：http://mobile.vehdjk.com/Article/details/gjghtvkrr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.bbcook.cn/Article/details/gpnjbvdmo.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/grrleiscc.sHtML

H. 异常与错误处理
来源：http://www.blog.vehdjk.com/Article/details/gwttitogo.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gfrypktsx.sHtML

[H01] try / catch 基础
来源：http://wap.yfazqb.com/Article/details/gdukqohar.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.fktsv.cn/Article/details/grhfmmkqe.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.epnwcf.com/Article/details/gyaevgfcp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fktsv.cn/Article/details/gkfsjttsw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.epnwcf.com/Article/details/gdpusmjzg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.epnwcf.com/Article/details/gkdsyukwl.sHtML


<!-- 参考信息 -->