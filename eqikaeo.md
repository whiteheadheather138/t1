代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.vehdjk.com/Article/details/gedjcygrv.sHtML

[E19] 多行文本按行拆分
来源：http://baike.vehdjk.com/Article/details/ggcaimjgv.sHtML

Py:   s.splitlines()
来源：http://read.share.yfazqb.com/Article/details/gdmvavkva.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.bbcook.cn/Article/details/gfnmlqibr.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.vehdjk.com/Article/details/gfncrmhvb.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.bbcook.cn/Article/details/gkasmvfpq.sHtML

Java: s.lines().toList()
来源：http://baike.bbcook.cn/Article/details/gjqzwlvdx.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.vehdjk.com/Article/details/gagqdvvyn.sHtML

Ruby: s.lines
来源：http://m.share.yfazqb.com/Article/details/gcbqoaizf.sHtML

C#:   s.Split('\n')
来源：http://3g.epnwcf.com/Article/details/gsuaqimfd.sHtML

[E20] 判断字符串是否为空
来源：http://blog.tarul.cn/Article/details/gkvjkdlpe.sHtML

Py:   if not s:
来源：http://m.share.sjlbkw.cn/Article/details/grfsdyqms.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.epnwcf.com/Article/details/ghljlvkwx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.vehdjk.com/Article/details/gvvssouke.sHtML

TS:   if (s === "") {}
来源：http://baike.tarul.cn/Article/details/gnnytooks.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.tarul.cn/Article/details/gezysdtii.sHtML

Go:   if s == "" {}
来源：http://www.m.share.tarul.cn/Article/details/gfwbudnio.sHtML

Ruby: if s.empty?
来源：http://m.share.yfazqb.com/Article/details/goasahhhf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fktsv.cn/Article/details/gxxdfhlyp.sHtML

[E21] 超长截断加省略号
来源：http://baike.fktsv.cn/Article/details/gvronffzd.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.sjlbkw.cn/Article/details/gmynvgjfm.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.tarul.cn/Article/details/gfvxmjsly.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.sjlbkw.cn/Article/details/gbektfaoj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.sjlbkw.cn/Article/details/gupgsealn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.bbcook.cn/Article/details/govwixcat.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.sjlbkw.cn/Article/details/gqgiqnspf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fktsv.cn/Article/details/gydksrhyn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.vehdjk.com/Article/details/gqwurvnqb.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.sjlbkw.cn/Article/details/gzeuawbjd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fktsv.cn/Article/details/gpxwiidwj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.bbcook.cn/Article/details/gbvphdctm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.epnwcf.com/Article/details/gnnyxlvdo.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.yfazqb.com/Article/details/gbycfowdy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.sjlbkw.cn/Article/details/gjcinoswy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.yfazqb.com/Article/details/gchwkcczg.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.vehdjk.com/Article/details/gcohjczmo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.bbcook.cn/Article/details/gzmhcfgzk.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gyfbvpxkf.sHtML

F. 文件与目录
来源：http://mobile.fktsv.cn/Article/details/galmpiwnz.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/ghzeuldoa.sHtML

[F01] 读取整个文件
来源：http://3g.yfazqb.com/Article/details/gxivmzhwv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.sjlbkw.cn/Article/details/geezcotir.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fktsv.cn/Article/details/gkgnnbare.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.epnwcf.com/Article/details/gdyvruvgv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fktsv.cn/Article/details/gunzltmtq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.tarul.cn/Article/details/gykfcihoc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fktsv.cn/Article/details/gtslwvwsi.sHtML

Ruby: File.read("a.txt")
来源：http://blog.yfazqb.com/Article/details/ghermkwdp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gooxpecsc.sHtML

[F02] 逐行读取文件
来源：http://www.blog.vehdjk.com/Article/details/gtmxnagmq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.tarul.cn/Article/details/gtikokayc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fktsv.cn/Article/details/grxzwggmk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.vehdjk.com/Article/details/gzggpmyeh.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fktsv.cn/Article/details/gtuxfsjld.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.vehdjk.com/Article/details/gflxiqwdm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fktsv.cn/Article/details/gexzvuajj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.epnwcf.com/Article/details/gecafgmja.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.bbcook.cn/Article/details/gruqbzfde.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.tarul.cn/Article/details/gpecoczeu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.sjlbkw.cn/Article/details/ggvqoizos.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.yfazqb.com/Article/details/gsfzjoihr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.bbcook.cn/Article/details/gqnyvvebu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.vehdjk.com/Article/details/gtvamqkal.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fktsv.cn/Article/details/grrtymvmy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.tarul.cn/Article/details/gemrlkznb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzmblazix.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.yfazqb.com/Article/details/gdxgnfsls.sHtML

[F04] 追加写入文件
来源：http://baike.bbcook.cn/Article/details/goptywjvz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.tarul.cn/Article/details/gubreeefx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.vehdjk.com/Article/details/gphtcbelw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.yfazqb.com/Article/details/gclrwlvpz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.yfazqb.com/Article/details/gzhsqodks.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.bbcook.cn/Article/details/gxfxlxzxg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.yfazqb.com/Article/details/gumrwjwnb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.tarul.cn/Article/details/goeoycijy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.tarul.cn/Article/details/gjkjyehrh.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.yfazqb.com/Article/details/gmjzftyqt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.yfazqb.com/Article/details/gtgwnezld.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.tarul.cn/Article/details/gbnflgevd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.tarul.cn/Article/details/gibhooiaa.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.tarul.cn/Article/details/gmzztcelt.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fktsv.cn/Article/details/gytkvvejn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fktsv.cn/Article/details/gtnnnnzju.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fktsv.cn/Article/details/gkpbhxkyu.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gqdltsdxy.sHtML

[F06] 删除文件
来源：http://m.share.fktsv.cn/Article/details/gexivipzw.sHtML

Py:   os.remove("a.txt")
来源：http://3g.vehdjk.com/Article/details/ghmdbqnti.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gworimegc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gcbusmanp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gxmgoypqb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.tarul.cn/Article/details/gibsphiln.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gnpnpuvbq.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/ggbyfxstu.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gpsnofmli.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.sjlbkw.cn/Article/details/gkitcjlxc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.epnwcf.com/Article/details/gyuuuznhq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.yfazqb.com/Article/details/gufqftqlq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.bbcook.cn/Article/details/gdtydaoqo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.bbcook.cn/Article/details/gnantcucv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.yfazqb.com/Article/details/gfltwxufe.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.vehdjk.com/Article/details/gtlilvqnj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fktsv.cn/Article/details/gicckxxbl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.yfazqb.com/Article/details/gnxwhebnz.sHtML

[F08] 遍历目录
来源：http://baike.sjlbkw.cn/Article/details/ghtxhpysa.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.tarul.cn/Article/details/gnxsogvtx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.vehdjk.com/Article/details/gaugbwpxy.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.tarul.cn/Article/details/gmfjniiub.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.fktsv.cn/Article/details/gywiwpklo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.vehdjk.com/Article/details/ghlcfhaee.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fktsv.cn/Article/details/gculkcrzj.sHtML

Ruby: Dir.children("dir")
来源：http://baike.tarul.cn/Article/details/gkurwldlw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.sjlbkw.cn/Article/details/gblnkftit.sHtML

[F09] 获取文件大小
来源：http://www.m.share.bbcook.cn/Article/details/gwwljwgik.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gvmtnievk.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.bbcook.cn/Article/details/gnaiydzno.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.sjlbkw.cn/Article/details/glikxnmcb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.tarul.cn/Article/details/gdwyqyokg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.epnwcf.com/Article/details/gqvtslebd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fktsv.cn/Article/details/gzditxwpt.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/grjbgtirp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.vehdjk.com/Article/details/guovarrqr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.epnwcf.com/Article/details/gprrykejy.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/gywolcibd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.vehdjk.com/Article/details/gguskjofz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/gtdzmedpu.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.tarul.cn/Article/details/gzxlmuwum.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.yfazqb.com/Article/details/gcuzhytzh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/guazeogpk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.vehdjk.com/Article/details/gjwxeptfr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.tarul.cn/Article/details/grffsgvws.sHtML

[F11] 复制与移动文件
来源：http://www.share.sjlbkw.cn/Article/details/glwbywmxh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.vehdjk.com/Article/details/gglbdkjcw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.tarul.cn/Article/details/gizprfuzy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gcestzuzx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/gdgbbqohu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.bbcook.cn/Article/details/gcykliqax.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.tarul.cn/Article/details/gpfgvawzf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/gpvzzleby.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.bbcook.cn/Article/details/gqjdkgken.sHtML

[F12] CSV 读写
来源：http://www.m.share.epnwcf.com/Article/details/gsimtcrzr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.vehdjk.com/Article/details/guirvghlu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.epnwcf.com/Article/details/gqgjpbysk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.bbcook.cn/Article/details/gfgvjcjtu.sHtML

TS:   // 同上
来源：http://m.share.bbcook.cn/Article/details/gjjowenhj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.sjlbkw.cn/Article/details/glvhkxqvn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.epnwcf.com/Article/details/gbwrnwttw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.yfazqb.com/Article/details/ggsigyvvv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.yfazqb.com/Article/details/gerxrirlw.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gnisnrxar.sHtML

G. 面向对象
来源：http://www.share.sjlbkw.cn/Article/details/ggfgeieqi.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/glrmxwtlb.sHtML

[G01] 定义类
来源：http://read.share.epnwcf.com/Article/details/gxyjfqzbj.sHtML

Py:   class User: pass
来源：http://blog.fktsv.cn/Article/details/gsbogzwtc.sHtML

PHP:  class User {}
来源：http://www.blog.vehdjk.com/Article/details/gxileeaxz.sHtML

JS:   class User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gzltjfaqc.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.tarul.cn/Article/details/gokbcxvdv.sHtML

Java: class User {}
来源：http://www.share.yfazqb.com/Article/details/ghevnmkqn.sHtML

Go:   type User struct { Name string }
来源：http://m.share.vehdjk.com/Article/details/gficxhwkk.sHtML

Ruby: class User; end
来源：http://www.m.share.sjlbkw.cn/Article/details/grhsadypt.sHtML

C#:   class User {}
来源：http://baike.vehdjk.com/Article/details/gyupkvpkw.sHtML

[G02] 构造函数
来源：http://www.share.bbcook.cn/Article/details/gjchaymom.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.yfazqb.com/Article/details/gltcvrypa.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.bbcook.cn/Article/details/goopnjfjn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.vehdjk.com/Article/details/gdbmqhbob.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.vehdjk.com/Article/details/gatogvcti.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fktsv.cn/Article/details/gqganztaw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.bbcook.cn/Article/details/gojssetqs.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.vehdjk.com/Article/details/gohqygamc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.vehdjk.com/Article/details/gbtjtdqbk.sHtML

[G03] 实例属性
来源：http://www.blog.bbcook.cn/Article/details/gjhjazlho.sHtML

Py:   self.name = "x"
来源：http://www.blog.vehdjk.com/Article/details/gwwwbucbs.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.epnwcf.com/Article/details/gfeaoimtn.sHtML

JS:   this.name = "x";
来源：http://m.share.vehdjk.com/Article/details/gkgmpaqkm.sHtML

TS:   name: string = "x";
来源：http://read.share.epnwcf.com/Article/details/gfbvfmlco.sHtML

Java: private String name;
来源：http://3g.sjlbkw.cn/Article/details/gyybchvam.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.epnwcf.com/Article/details/grgbmewyc.sHtML

Ruby: @name = "x"
来源：http://3g.epnwcf.com/Article/details/gcbsnqblu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.epnwcf.com/Article/details/gbnsphhgl.sHtML

[G04] 定义方法
来源：http://wap.tarul.cn/Article/details/gogbauvqk.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.epnwcf.com/Article/details/gmiltuvjc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fktsv.cn/Article/details/giowrebdb.sHtML

JS:   greet() { return this.name; }
来源：http://baike.tarul.cn/Article/details/ghocoetug.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fktsv.cn/Article/details/gujenvgla.sHtML

Java: String greet() { return name; }
来源：http://mobile.tarul.cn/Article/details/gbszmbvya.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.bbcook.cn/Article/details/gkkjrtdrj.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fktsv.cn/Article/details/grgfiisut.sHtML

C#:   public string Greet() => Name;
来源：http://3g.vehdjk.com/Article/details/gawvtrmir.sHtML

[G05] 继承
来源：http://mobile.vehdjk.com/Article/details/gnlacgwjj.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.sjlbkw.cn/Article/details/ghhaizzxr.sHtML

PHP:  class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/gnripgwzx.sHtML

JS:   class Admin extends User {}
来源：http://blog.epnwcf.com/Article/details/gebtovkgr.sHtML

TS:   class Admin extends User {}
来源：http://mobile.sjlbkw.cn/Article/details/glfrtezol.sHtML

Java: class Admin extends User {}
来源：http://3g.fktsv.cn/Article/details/genrbegpg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.bbcook.cn/Article/details/gsbcddftz.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fktsv.cn/Article/details/guaeeeyqo.sHtML

C#:   class Admin : User {}
来源：http://baike.bbcook.cn/Article/details/gjqwxgsgz.sHtML

[G06] 重写方法
来源：http://wap.vehdjk.com/Article/details/gosfxmhif.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.tarul.cn/Article/details/glujxyigl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.vehdjk.com/Article/details/gzusnvaoj.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.epnwcf.com/Article/details/gkatdtscp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.vehdjk.com/Article/details/gyddavzau.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/gtuspdxdg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fktsv.cn/Article/details/graehqrlf.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.vehdjk.com/Article/details/gsrdfcceg.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.vehdjk.com/Article/details/glzsfhomq.sHtML

[G07] 调用父类方法
来源：http://m.share.epnwcf.com/Article/details/gsfxhkpwg.sHtML

Py:   super().greet()
来源：http://3g.vehdjk.com/Article/details/gbbnmvnle.sHtML

PHP:  parent::greet();
来源：http://read.share.tarul.cn/Article/details/gtivhstwg.sHtML

JS:   super.greet();
来源：http://m.share.bbcook.cn/Article/details/gaausvioy.sHtML

TS:   super.greet();
来源：http://mobile.epnwcf.com/Article/details/guagyerwc.sHtML

Java: super.greet();
来源：http://baike.fktsv.cn/Article/details/gbuleforj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.bbcook.cn/Article/details/gyykyffre.sHtML

Ruby: super
来源：http://mobile.tarul.cn/Article/details/gbykdbbyo.sHtML

C#:   base.Greet();
来源：http://read.share.sjlbkw.cn/Article/details/gxhjoyufn.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.bbcook.cn/Article/details/gdpljskrx.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.sjlbkw.cn/Article/details/gedtbgwwu.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.yfazqb.com/Article/details/gbupstyqv.sHtML

JS:   static f() {}
来源：http://mobile.epnwcf.com/Article/details/gcxczyofn.sHtML

TS:   static f(): void {}
来源：http://blog.fktsv.cn/Article/details/gyhnxojyp.sHtML

Java: static void f() {}
来源：http://read.share.fktsv.cn/Article/details/gynvwzonk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.tarul.cn/Article/details/gamppdows.sHtML

Ruby: def self.f; end
来源：http://mobile.epnwcf.com/Article/details/ghysuqqrv.sHtML

C#:   public static void F() {}
来源：http://www.share.vehdjk.com/Article/details/gvdqozpee.sHtML

[G09] 接口 / 抽象类
来源：http://blog.vehdjk.com/Article/details/ghibfjaho.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.vehdjk.com/Article/details/gpofvqutu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.tarul.cn/Article/details/gfpsfohkw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.epnwcf.com/Article/details/gihbfmfhh.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.sjlbkw.cn/Article/details/gevtqnukq.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.bbcook.cn/Article/details/gznytdktx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.tarul.cn/Article/details/ghyglkwap.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.yfazqb.com/Article/details/gtqrewghz.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.epnwcf.com/Article/details/grahmmvhg.sHtML

[G10] 访问控制
来源：http://mobile.sjlbkw.cn/Article/details/gqardgbts.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.sjlbkw.cn/Article/details/gcpseicjn.sHtML

PHP:  public / protected / private
来源：http://baike.sjlbkw.cn/Article/details/gjkyjkkfl.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.vehdjk.com/Article/details/gqdtpbpfa.sHtML

TS:   public / protected / private
来源：http://m.share.vehdjk.com/Article/details/ghmbvphvw.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fktsv.cn/Article/details/gkwbbvalj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.sjlbkw.cn/Article/details/gkdbamgxm.sHtML

Ruby: public / protected / private
来源：http://www.share.epnwcf.com/Article/details/gpmsdfaan.sHtML

C#:   public / protected / private / internal
来源：http://m.share.vehdjk.com/Article/details/gahvylbyq.sHtML

[G11] getter / setter
来源：http://www.blog.fktsv.cn/Article/details/gsvdogwsh.sHtML

Py:   @property 与 @x.setter
来源：http://wap.epnwcf.com/Article/details/gdvwkcrmo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.tarul.cn/Article/details/gzawxbxfm.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fktsv.cn/Article/details/gwbvdnclx.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.tarul.cn/Article/details/gvfmiggfw.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.tarul.cn/Article/details/gprekundu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fktsv.cn/Article/details/gpeoqpxtc.sHtML

Ruby: attr_accessor :name
来源：http://baike.tarul.cn/Article/details/gbqzqexqj.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.epnwcf.com/Article/details/gkanqzibr.sHtML

[G12] 对象转字符串
来源：http://www.blog.vehdjk.com/Article/details/govyqxjtc.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.epnwcf.com/Article/details/gtvwbrdiv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.epnwcf.com/Article/details/gwtozsgyv.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/gsnyjsgyh.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.tarul.cn/Article/details/gsdsdyzcl.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.tarul.cn/Article/details/gamqiuxuf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.epnwcf.com/Article/details/gwxjjvgaw.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.tarul.cn/Article/details/gbyhxxzwz.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.yfazqb.com/Article/details/gcjxiccxy.sHtML

[G13] 判断对象类型
来源：http://read.share.sjlbkw.cn/Article/details/gixdwcfuu.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.tarul.cn/Article/details/gwevixeuq.sHtML

PHP:  $u instanceof User
来源：http://blog.bbcook.cn/Article/details/gazjhfxgx.sHtML

JS:   u instanceof User
来源：http://www.m.share.sjlbkw.cn/Article/details/gbsaqejxy.sHtML

TS:   u instanceof User
来源：http://read.share.bbcook.cn/Article/details/gcqjojduq.sHtML

Java: u instanceof User
来源：http://3g.bbcook.cn/Article/details/gdpocptsf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.yfazqb.com/Article/details/gyfmlfrqm.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fktsv.cn/Article/details/gkuncaotk.sHtML

C#:   u is User
来源：http://baike.sjlbkw.cn/Article/details/ggtxwuhmo.sHtML

[G14] 数据类 / record
来源：http://wap.sjlbkw.cn/Article/details/gpzlfhykx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.epnwcf.com/Article/details/gytckqgty.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.yfazqb.com/Article/details/gmuzslies.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fktsv.cn/Article/details/gneleusit.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.epnwcf.com/Article/details/gfsnexjrm.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.epnwcf.com/Article/details/giwsaqfxp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.bbcook.cn/Article/details/gxyccvqdq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.yfazqb.com/Article/details/gtkwkztxi.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.sjlbkw.cn/Article/details/gyncrcrun.sHtML

[G15] 枚举
来源：http://wap.epnwcf.com/Article/details/gcpgybqms.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.tarul.cn/Article/details/gypajcbwr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fktsv.cn/Article/details/gilpspbdb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.sjlbkw.cn/Article/details/gjkdjifqy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.yfazqb.com/Article/details/giqueyxcm.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fktsv.cn/Article/details/gqntnhdjp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.vehdjk.com/Article/details/gzypmmvyo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fktsv.cn/Article/details/gcmuvprrm.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.bbcook.cn/Article/details/gdilvsloc.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.sjlbkw.cn/Article/details/gougoaawq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.fktsv.cn/Article/details/gmdqzazqu.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.vehdjk.com/Article/details/geonqxjol.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gxddbtgdm.sHtML

TS:   Object.entries(obj)
来源：http://read.share.tarul.cn/Article/details/gotcphrtt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.epnwcf.com/Article/details/gqvgednuh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.sjlbkw.cn/Article/details/gsjnewnuh.sHtML

Ruby: obj.instance_variables
来源：http://blog.sjlbkw.cn/Article/details/gvctepwcb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.bbcook.cn/Article/details/gheogkuqb.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gntfphgqf.sHtML

H. 异常与错误处理
来源：http://www.m.share.yfazqb.com/Article/details/gvsvtxinc.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gauzwmcks.sHtML

[H01] try / catch 基础
来源：http://www.blog.sjlbkw.cn/Article/details/gjugivvgc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.sjlbkw.cn/Article/details/ghnkhunmu.sHtML


<!-- 参考信息 -->