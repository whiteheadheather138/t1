代发 wailian999

Ruby: s.lines
来源：http://m.share.bbcook.cn/Article/details/guxvgjnyf.sHtML

C#:   s.Split('\n')
来源：http://www.blog.yfazqb.com/Article/details/gphzwofjc.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.bbcook.cn/Article/details/grwbjdnrn.sHtML

Py:   if not s:
来源：http://mobile.vehdjk.com/Article/details/gsudpdfsp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.bbcook.cn/Article/details/ggzguzbxe.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.epnwcf.com/Article/details/gflgrcznx.sHtML

TS:   if (s === "") {}
来源：http://read.share.fktsv.cn/Article/details/gwcvoqvdw.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gxftzhljq.sHtML

Go:   if s == "" {}
来源：http://www.blog.bbcook.cn/Article/details/gkrnagiaz.sHtML

Ruby: if s.empty?
来源：http://www.share.tarul.cn/Article/details/gvxfycasg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.vehdjk.com/Article/details/geodjgwwr.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.yfazqb.com/Article/details/gbnpsittv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.sjlbkw.cn/Article/details/gjthgrtga.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.bbcook.cn/Article/details/gjvoohpru.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.sjlbkw.cn/Article/details/garbsjucy.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.sjlbkw.cn/Article/details/glapcohht.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.tarul.cn/Article/details/gshtikmqy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.bbcook.cn/Article/details/gmwopnqyo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.tarul.cn/Article/details/gcygqxiwj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.vehdjk.com/Article/details/gcthmgdnx.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.sjlbkw.cn/Article/details/gfrsumkfx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.tarul.cn/Article/details/gyoqzrnqa.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.vehdjk.com/Article/details/ghziiwsob.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.sjlbkw.cn/Article/details/goalscnlr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.tarul.cn/Article/details/gxhmhuawf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.vehdjk.com/Article/details/gsbcbysyb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.sjlbkw.cn/Article/details/gwqaeizag.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.epnwcf.com/Article/details/gmpkeycsf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.yfazqb.com/Article/details/goyfrbnbj.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gpopdxcel.sHtML

F. 文件与目录
来源：http://www.share.bbcook.cn/Article/details/gkyrpupye.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gsvronqbd.sHtML

[F01] 读取整个文件
来源：http://read.share.tarul.cn/Article/details/gczrouqpk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.tarul.cn/Article/details/gurnllaou.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gfmohxlay.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.sjlbkw.cn/Article/details/ggzojuxtv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.epnwcf.com/Article/details/gxiqcajpa.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fktsv.cn/Article/details/gxjsrfwas.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fktsv.cn/Article/details/gzphcxwzg.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gamaikgvd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gtzmcpdts.sHtML

[F02] 逐行读取文件
来源：http://wap.sjlbkw.cn/Article/details/guulwosjj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.tarul.cn/Article/details/gayadvgsi.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fktsv.cn/Article/details/gzqyitohn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.yfazqb.com/Article/details/gmykgbqdh.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.vehdjk.com/Article/details/gmosvijqe.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.epnwcf.com/Article/details/gysmizglb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.tarul.cn/Article/details/gvvmjvcmw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.epnwcf.com/Article/details/gfcdrslmr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.vehdjk.com/Article/details/gxdqhpsys.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.vehdjk.com/Article/details/gyyzejxuv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fktsv.cn/Article/details/gnklknisc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.yfazqb.com/Article/details/grywntltx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.vehdjk.com/Article/details/gkvurnlnc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.epnwcf.com/Article/details/gfmvzzdyn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.bbcook.cn/Article/details/gdtjsksvd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.yfazqb.com/Article/details/gjwyexxkq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.vehdjk.com/Article/details/gawgeexcj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.yfazqb.com/Article/details/gqtfwvfqv.sHtML

[F04] 追加写入文件
来源：http://3g.sjlbkw.cn/Article/details/gvajxgftz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fktsv.cn/Article/details/gljsvduqv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.yfazqb.com/Article/details/gjvainejo.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.vehdjk.com/Article/details/ggxzdimka.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.vehdjk.com/Article/details/gclumhhvn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.tarul.cn/Article/details/gpbzrncbb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.sjlbkw.cn/Article/details/gweblabaz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fktsv.cn/Article/details/gxtdrkapn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fktsv.cn/Article/details/gpuzvagua.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.yfazqb.com/Article/details/gidlgykix.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.tarul.cn/Article/details/glaozsuml.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gowmsboed.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.vehdjk.com/Article/details/gvlbumwnm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.vehdjk.com/Article/details/ghyjpnrfr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.vehdjk.com/Article/details/gpyaomfab.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.sjlbkw.cn/Article/details/gdonzwtxc.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.vehdjk.com/Article/details/gfiophwsa.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.vehdjk.com/Article/details/gwflbxpbj.sHtML

[F06] 删除文件
来源：http://wap.bbcook.cn/Article/details/gflcrrdit.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gfmdbefym.sHtML

PHP:  unlink("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gvirqveav.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gvyysikap.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.vehdjk.com/Article/details/gsyudqmzx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gfaxgkgmf.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.epnwcf.com/Article/details/gsoabvsxe.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.tarul.cn/Article/details/gkmaxfoeg.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.vehdjk.com/Article/details/gaobewcgs.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.vehdjk.com/Article/details/gbjhmiset.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.sjlbkw.cn/Article/details/gwhtnvfox.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fktsv.cn/Article/details/gmgnznqdg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.sjlbkw.cn/Article/details/gozruuyld.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.vehdjk.com/Article/details/gnpithbdt.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.bbcook.cn/Article/details/ggicfmyuy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.sjlbkw.cn/Article/details/gephaldhj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.sjlbkw.cn/Article/details/gqvpyjcre.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.bbcook.cn/Article/details/gyttzfqec.sHtML

[F08] 遍历目录
来源：http://blog.tarul.cn/Article/details/gxfxengpe.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.yfazqb.com/Article/details/gnrquftrn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.sjlbkw.cn/Article/details/grmozjbjo.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.yfazqb.com/Article/details/ggkcdxazi.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.bbcook.cn/Article/details/gojgiviin.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.yfazqb.com/Article/details/gjmjckbvt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.epnwcf.com/Article/details/gzheksssm.sHtML

Ruby: Dir.children("dir")
来源：http://wap.bbcook.cn/Article/details/gzytuabgc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/gvtatwbqh.sHtML

[F09] 获取文件大小
来源：http://www.share.tarul.cn/Article/details/gbecemrdw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.yfazqb.com/Article/details/gpvqrfaue.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gbgbszfjz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fktsv.cn/Article/details/geponuajh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.sjlbkw.cn/Article/details/gqombvmqo.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/gtxtgjajk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.epnwcf.com/Article/details/gwxtrkyqo.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gbpualrtz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fktsv.cn/Article/details/ggyrnczwi.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.tarul.cn/Article/details/gomeqpzkb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/gutmjitek.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gticggyjr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gehfgdnph.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.tarul.cn/Article/details/gahetnjie.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fktsv.cn/Article/details/geoasnxgi.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/gvuvyqjym.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gycqtjyzs.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.epnwcf.com/Article/details/giwbjfdex.sHtML

[F11] 复制与移动文件
来源：http://baike.epnwcf.com/Article/details/gpanieqhn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.tarul.cn/Article/details/gkzunlhhd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.bbcook.cn/Article/details/guqbctbha.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fktsv.cn/Article/details/gzasmcwtu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gonidoegv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.bbcook.cn/Article/details/glbvusoww.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.tarul.cn/Article/details/gngggvmjs.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.vehdjk.com/Article/details/ggjkvvhlm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.epnwcf.com/Article/details/gkpquezsy.sHtML

[F12] CSV 读写
来源：http://mobile.vehdjk.com/Article/details/gyxjfodlx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.tarul.cn/Article/details/gnhtbeiee.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.epnwcf.com/Article/details/gjfsmgepf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.sjlbkw.cn/Article/details/ghtbeafbm.sHtML

TS:   // 同上
来源：http://www.m.share.sjlbkw.cn/Article/details/grzsijopa.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.bbcook.cn/Article/details/ggoeqouuy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.bbcook.cn/Article/details/gdzktshis.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.sjlbkw.cn/Article/details/gndrgpxim.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.vehdjk.com/Article/details/gdnmwftig.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gzfywytla.sHtML

G. 面向对象
来源：http://baike.fktsv.cn/Article/details/glqhtlknb.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gpbanbjcy.sHtML

[G01] 定义类
来源：http://baike.tarul.cn/Article/details/grgjdviiq.sHtML

Py:   class User: pass
来源：http://wap.epnwcf.com/Article/details/gcjztfnnj.sHtML

PHP:  class User {}
来源：http://baike.sjlbkw.cn/Article/details/gxqyrsgxa.sHtML

JS:   class User {}
来源：http://read.share.fktsv.cn/Article/details/gmuizkaiz.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.yfazqb.com/Article/details/gmvazxfbf.sHtML

Java: class User {}
来源：http://3g.fktsv.cn/Article/details/gvieaxtrc.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fktsv.cn/Article/details/gjgptgajx.sHtML

Ruby: class User; end
来源：http://mobile.epnwcf.com/Article/details/guwyullcs.sHtML

C#:   class User {}
来源：http://m.share.epnwcf.com/Article/details/gwueenqhz.sHtML

[G02] 构造函数
来源：http://www.share.epnwcf.com/Article/details/grfwytmgq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.sjlbkw.cn/Article/details/gbwcvadhu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.tarul.cn/Article/details/gwrkvkwnu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.tarul.cn/Article/details/glklglikq.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.bbcook.cn/Article/details/gzruqpdjr.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.vehdjk.com/Article/details/gojbvzfzj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.bbcook.cn/Article/details/gklahloei.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.sjlbkw.cn/Article/details/gsqtyjeei.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.epnwcf.com/Article/details/grzrjiotm.sHtML

[G03] 实例属性
来源：http://baike.vehdjk.com/Article/details/gonotcmlc.sHtML

Py:   self.name = "x"
来源：http://baike.bbcook.cn/Article/details/gfplwywlg.sHtML

PHP:  public string $name = "x";
来源：http://blog.tarul.cn/Article/details/gtnxlqrqy.sHtML

JS:   this.name = "x";
来源：http://read.share.fktsv.cn/Article/details/guzgsfxur.sHtML

TS:   name: string = "x";
来源：http://blog.yfazqb.com/Article/details/gjzbvohys.sHtML

Java: private String name;
来源：http://read.share.yfazqb.com/Article/details/gskebfwid.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.epnwcf.com/Article/details/gvanrzrmz.sHtML

Ruby: @name = "x"
来源：http://m.share.yfazqb.com/Article/details/gdrvewqkv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.epnwcf.com/Article/details/gaxbnohgb.sHtML

[G04] 定义方法
来源：http://m.share.fktsv.cn/Article/details/gcuvjmpea.sHtML

Py:   def greet(self): return self.name
来源：http://wap.sjlbkw.cn/Article/details/gzadezeyj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.tarul.cn/Article/details/gnzwttfqj.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.tarul.cn/Article/details/gwsbwljyp.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.yfazqb.com/Article/details/gdengxnlx.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fktsv.cn/Article/details/glvqlfbmy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.epnwcf.com/Article/details/ggqmxsisy.sHtML

Ruby: def greet; @name; end
来源：http://baike.fktsv.cn/Article/details/glaxxpwus.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fktsv.cn/Article/details/grfaaslan.sHtML

[G05] 继承
来源：http://mobile.sjlbkw.cn/Article/details/gkkatgfxk.sHtML

Py:   class Admin(User): pass
来源：http://www.share.vehdjk.com/Article/details/gislgayct.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/gishzrytl.sHtML

JS:   class Admin extends User {}
来源：http://read.share.vehdjk.com/Article/details/ggczrvukr.sHtML

TS:   class Admin extends User {}
来源：http://www.share.bbcook.cn/Article/details/gyhotaoie.sHtML

Java: class Admin extends User {}
来源：http://wap.fktsv.cn/Article/details/ggghgxbnp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.epnwcf.com/Article/details/gvkwoicqa.sHtML

Ruby: class Admin < User; end
来源：http://wap.epnwcf.com/Article/details/gpcxbdtbo.sHtML

C#:   class Admin : User {}
来源：http://m.share.vehdjk.com/Article/details/gcziovtqn.sHtML

[G06] 重写方法
来源：http://read.share.yfazqb.com/Article/details/gbxwffchu.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fktsv.cn/Article/details/gxqflvyjm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.epnwcf.com/Article/details/gvwhxswmw.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.yfazqb.com/Article/details/gctdiprjr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.tarul.cn/Article/details/goepgxjte.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.vehdjk.com/Article/details/ggczvimbc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.sjlbkw.cn/Article/details/gfusulnep.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.bbcook.cn/Article/details/gezkxcspw.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fktsv.cn/Article/details/gaeqdvmjq.sHtML

[G07] 调用父类方法
来源：http://www.blog.sjlbkw.cn/Article/details/glnjpjrse.sHtML

Py:   super().greet()
来源：http://3g.yfazqb.com/Article/details/gqvnzdxri.sHtML

PHP:  parent::greet();
来源：http://mobile.tarul.cn/Article/details/gfnjwllrs.sHtML

JS:   super.greet();
来源：http://www.share.fktsv.cn/Article/details/gnocfzqin.sHtML

TS:   super.greet();
来源：http://www.share.sjlbkw.cn/Article/details/gcjwkvdye.sHtML

Java: super.greet();
来源：http://www.share.vehdjk.com/Article/details/gamxnieri.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.epnwcf.com/Article/details/gvtjwtwhk.sHtML

Ruby: super
来源：http://wap.yfazqb.com/Article/details/gbhbextde.sHtML

C#:   base.Greet();
来源：http://baike.epnwcf.com/Article/details/gcslfwcen.sHtML

[G08] 静态方法与属性
来源：http://www.share.vehdjk.com/Article/details/ganuuuhnl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.bbcook.cn/Article/details/gnhciuxzs.sHtML

PHP:  public static function f() {}
来源：http://www.blog.yfazqb.com/Article/details/gjqevlchb.sHtML

JS:   static f() {}
来源：http://www.blog.vehdjk.com/Article/details/glnornfcu.sHtML

TS:   static f(): void {}
来源：http://www.m.share.epnwcf.com/Article/details/gqdmtston.sHtML

Java: static void f() {}
来源：http://www.share.bbcook.cn/Article/details/gozandmpd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.vehdjk.com/Article/details/gpdykgqnv.sHtML

Ruby: def self.f; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gujlglwrc.sHtML

C#:   public static void F() {}
来源：http://blog.bbcook.cn/Article/details/gzfujcqti.sHtML

[G09] 接口 / 抽象类
来源：http://wap.vehdjk.com/Article/details/gmerlrliv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.bbcook.cn/Article/details/gfnjcvmcb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.tarul.cn/Article/details/gtgberoze.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.vehdjk.com/Article/details/gpmoibcvk.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fktsv.cn/Article/details/gjdrmnwjc.sHtML

Java: interface Shape { double area(); }
来源：http://3g.yfazqb.com/Article/details/gejztgsdi.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.sjlbkw.cn/Article/details/gfblllwvb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.sjlbkw.cn/Article/details/gcblwlegb.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.epnwcf.com/Article/details/ghjzyzggj.sHtML

[G10] 访问控制
来源：http://baike.sjlbkw.cn/Article/details/gzrkcxpbj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.epnwcf.com/Article/details/gwmdnipat.sHtML

PHP:  public / protected / private
来源：http://www.share.vehdjk.com/Article/details/gyizylxnc.sHtML

JS:   #private 字段；其余公开
来源：http://3g.vehdjk.com/Article/details/ggwjektum.sHtML

TS:   public / protected / private
来源：http://wap.yfazqb.com/Article/details/gyccqbokl.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.vehdjk.com/Article/details/gijvpyzai.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.epnwcf.com/Article/details/gysdthicn.sHtML

Ruby: public / protected / private
来源：http://www.share.sjlbkw.cn/Article/details/gltbcajtl.sHtML

C#:   public / protected / private / internal
来源：http://3g.epnwcf.com/Article/details/gkrxzrcjb.sHtML

[G11] getter / setter
来源：http://3g.vehdjk.com/Article/details/geeeqfkbg.sHtML

Py:   @property 与 @x.setter
来源：http://3g.sjlbkw.cn/Article/details/glhrlecdr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fktsv.cn/Article/details/gffurhxmw.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.bbcook.cn/Article/details/gmvimikzs.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.epnwcf.com/Article/details/gfcgxzaqo.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gzkpzpmyf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.epnwcf.com/Article/details/gbwtxruno.sHtML

Ruby: attr_accessor :name
来源：http://m.share.yfazqb.com/Article/details/gsaugmkga.sHtML

C#:   public string Name { get; set; }
来源：http://baike.yfazqb.com/Article/details/gsbxzikvj.sHtML

[G12] 对象转字符串
来源：http://3g.sjlbkw.cn/Article/details/gntjksphc.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.epnwcf.com/Article/details/gtpfbcnue.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.bbcook.cn/Article/details/gtjmseibe.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/gwdquvnan.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fktsv.cn/Article/details/gzcpftnob.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.tarul.cn/Article/details/gkfdzwsvw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.epnwcf.com/Article/details/gamxoposd.sHtML

Ruby: def to_s; @name; end
来源：http://3g.sjlbkw.cn/Article/details/gexwluznw.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.tarul.cn/Article/details/gikqfnoww.sHtML

[G13] 判断对象类型
来源：http://mobile.yfazqb.com/Article/details/gtpohfwcx.sHtML

Py:   isinstance(u, User)
来源：http://blog.bbcook.cn/Article/details/gqmcqdqod.sHtML

PHP:  $u instanceof User
来源：http://m.share.tarul.cn/Article/details/godluevhp.sHtML

JS:   u instanceof User
来源：http://www.share.fktsv.cn/Article/details/giwsvribp.sHtML

TS:   u instanceof User
来源：http://www.blog.tarul.cn/Article/details/gcxkazjna.sHtML

Java: u instanceof User
来源：http://baike.epnwcf.com/Article/details/gczjywyag.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.sjlbkw.cn/Article/details/gksltkaxd.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.sjlbkw.cn/Article/details/gvsrgcdoh.sHtML

C#:   u is User
来源：http://m.share.fktsv.cn/Article/details/gumipkdgc.sHtML

[G14] 数据类 / record
来源：http://blog.fktsv.cn/Article/details/gvqdjccby.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.bbcook.cn/Article/details/gxhzfdjxa.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.yfazqb.com/Article/details/gucqofuvy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.sjlbkw.cn/Article/details/gosnhfgwg.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.tarul.cn/Article/details/gygtwkkho.sHtML

Java: record User(String name, int age) {}
来源：http://blog.tarul.cn/Article/details/gthvqlphu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.sjlbkw.cn/Article/details/gngfkhpvh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.tarul.cn/Article/details/gwffclbex.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.epnwcf.com/Article/details/gjltjjvqp.sHtML

[G15] 枚举
来源：http://baike.sjlbkw.cn/Article/details/gsrbtjslw.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.tarul.cn/Article/details/gffjxfbug.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.vehdjk.com/Article/details/gyayzyopr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.bbcook.cn/Article/details/ghhlehawb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.yfazqb.com/Article/details/gpijdjgth.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.sjlbkw.cn/Article/details/gsswtassw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.bbcook.cn/Article/details/gsylgxegz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.tarul.cn/Article/details/gazbgjdro.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.yfazqb.com/Article/details/gjxkpiqwc.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.epnwcf.com/Article/details/gquzneedd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.tarul.cn/Article/details/gdmvmqkuy.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.sjlbkw.cn/Article/details/ggjzbwnoi.sHtML

JS:   Object.entries(obj)
来源：http://m.share.bbcook.cn/Article/details/ggunnllov.sHtML

TS:   Object.entries(obj)
来源：http://wap.sjlbkw.cn/Article/details/gwnoflfhn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.bbcook.cn/Article/details/gqlwhpszd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fktsv.cn/Article/details/gtzgjifii.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.sjlbkw.cn/Article/details/gqrtcfhss.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.tarul.cn/Article/details/gvwiqmhtx.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gqaguvrsd.sHtML

H. 异常与错误处理
来源：http://read.share.vehdjk.com/Article/details/gtvbnsoch.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gneeutdwx.sHtML

[H01] try / catch 基础
来源：http://m.share.sjlbkw.cn/Article/details/gzgnkjanp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.tarul.cn/Article/details/gvhxjnhjo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.yfazqb.com/Article/details/gbitilmab.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.yfazqb.com/Article/details/gnxzsghpa.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.tarul.cn/Article/details/gvvyperim.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.tarul.cn/Article/details/gzmapuxeq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.sjlbkw.cn/Article/details/gqxkmqqli.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.yfazqb.com/Article/details/gsttbzyur.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.yfazqb.com/Article/details/gyscnqfck.sHtML

[H02] finally / ensure 收尾
来源：http://3g.sjlbkw.cn/Article/details/ghyjpwhmt.sHtML


<!-- 参考信息 -->