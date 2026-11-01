代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.tarul.cn/Article/details/gdkhznapa.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.sjlbkw.cn/Article/details/gxfezecor.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.bbcook.cn/Article/details/gcdzwvhrl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.sjlbkw.cn/Article/details/guzqqbmdm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.sjlbkw.cn/Article/details/gaamognsd.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fktsv.cn/Article/details/gcifpkumw.sHtML

Py:   s.splitlines()
来源：http://read.share.epnwcf.com/Article/details/ghzqsvhfu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.vehdjk.com/Article/details/givivuuub.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.bbcook.cn/Article/details/gqnlqnrta.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.bbcook.cn/Article/details/gldwxatzw.sHtML

Java: s.lines().toList()
来源：http://www.m.share.vehdjk.com/Article/details/gzjoijpjl.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.tarul.cn/Article/details/gusilnmjv.sHtML

Ruby: s.lines
来源：http://baike.vehdjk.com/Article/details/gaegivpee.sHtML

C#:   s.Split('\n')
来源：http://m.share.tarul.cn/Article/details/gcmhjvfch.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.sjlbkw.cn/Article/details/gwrhafdrw.sHtML

Py:   if not s:
来源：http://mobile.epnwcf.com/Article/details/glptgmcmt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.tarul.cn/Article/details/gojliskwx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fktsv.cn/Article/details/ghfpqgizw.sHtML

TS:   if (s === "") {}
来源：http://m.share.vehdjk.com/Article/details/gymjwcxtx.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.sjlbkw.cn/Article/details/ggibcrzbc.sHtML

Go:   if s == "" {}
来源：http://m.share.tarul.cn/Article/details/ghsfntogq.sHtML

Ruby: if s.empty?
来源：http://mobile.yfazqb.com/Article/details/gxitjsgkf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.vehdjk.com/Article/details/ghycbzifa.sHtML

[E21] 超长截断加省略号
来源：http://3g.tarul.cn/Article/details/gsalxlcnu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.vehdjk.com/Article/details/gdsywtuqt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.tarul.cn/Article/details/gxsezdedg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.epnwcf.com/Article/details/gcooxqqyf.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.epnwcf.com/Article/details/gimvglero.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.yfazqb.com/Article/details/gahjpwyvg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.tarul.cn/Article/details/gfuhsjsgp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.epnwcf.com/Article/details/goncnetxd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.tarul.cn/Article/details/gqvoxzhvj.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fktsv.cn/Article/details/gugfgzyct.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.bbcook.cn/Article/details/gjdtalrvp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.bbcook.cn/Article/details/gqnfrzzmm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.epnwcf.com/Article/details/gznqmfgui.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.vehdjk.com/Article/details/gdbnvdxwm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.epnwcf.com/Article/details/gqsnwmsem.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.epnwcf.com/Article/details/gjpcibimf.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.epnwcf.com/Article/details/gcblteuuk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.yfazqb.com/Article/details/gorqvwrrc.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gjnvbvdwx.sHtML

F. 文件与目录
来源：http://www.m.share.epnwcf.com/Article/details/gyneutumq.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gnudaojxr.sHtML

[F01] 读取整个文件
来源：http://read.share.sjlbkw.cn/Article/details/gokpozths.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fktsv.cn/Article/details/gvaxorksr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.bbcook.cn/Article/details/gphpbdxcs.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.sjlbkw.cn/Article/details/gsyfhczph.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.vehdjk.com/Article/details/gwkijwtcy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/ghczdsapo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.tarul.cn/Article/details/gatuhizvb.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fktsv.cn/Article/details/garqivust.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.bbcook.cn/Article/details/gpumcsvsb.sHtML

[F02] 逐行读取文件
来源：http://blog.epnwcf.com/Article/details/givevtbcv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.tarul.cn/Article/details/giidhbpvo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.yfazqb.com/Article/details/gplsejyfu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.epnwcf.com/Article/details/gkyxaajrr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.tarul.cn/Article/details/gwstlnwww.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.tarul.cn/Article/details/gjysqfcdr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.sjlbkw.cn/Article/details/gewvizdvc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.vehdjk.com/Article/details/gszocsden.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fktsv.cn/Article/details/gfimxyhxv.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.yfazqb.com/Article/details/gihvrkdhc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.yfazqb.com/Article/details/gctrfpoxn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.bbcook.cn/Article/details/giwibfrmd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.yfazqb.com/Article/details/gtzognktd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.yfazqb.com/Article/details/grfvqofpy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.bbcook.cn/Article/details/ggrtujzsj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.vehdjk.com/Article/details/ghwsrptit.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.sjlbkw.cn/Article/details/glvrrluuf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.sjlbkw.cn/Article/details/gphwvyxsy.sHtML

[F04] 追加写入文件
来源：http://m.share.epnwcf.com/Article/details/gufjqxwud.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.epnwcf.com/Article/details/gexzyncqn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.epnwcf.com/Article/details/giydftmjp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.epnwcf.com/Article/details/gmhmyvmvh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.epnwcf.com/Article/details/giuokjlwz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.sjlbkw.cn/Article/details/gbsgfbigg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.bbcook.cn/Article/details/gasbuffus.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.epnwcf.com/Article/details/gzvvhjufj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.vehdjk.com/Article/details/grpsklokd.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.epnwcf.com/Article/details/gahlwcdvv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.vehdjk.com/Article/details/gqyomalcx.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.epnwcf.com/Article/details/gkhkzezuz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fktsv.cn/Article/details/guaddwehx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gwgabvcok.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.epnwcf.com/Article/details/gulzaqdbg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.sjlbkw.cn/Article/details/gxpvptfis.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gfdzbihbb.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.tarul.cn/Article/details/gyoqssrom.sHtML

[F06] 删除文件
来源：http://read.share.yfazqb.com/Article/details/gwofpxmtz.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gxpwrteqt.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gmditvxhz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gcbqfioax.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gamrqczqu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fktsv.cn/Article/details/gegizfodi.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gpegwzabk.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gjhnqvdyj.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.tarul.cn/Article/details/gstheqybz.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.bbcook.cn/Article/details/gptgyxxxo.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fktsv.cn/Article/details/gtwtfcjas.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.sjlbkw.cn/Article/details/gpdljeudk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.sjlbkw.cn/Article/details/ggpuvdbxk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.yfazqb.com/Article/details/gftzgkrug.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.sjlbkw.cn/Article/details/gbxidfrww.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.epnwcf.com/Article/details/gcljbjefq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.bbcook.cn/Article/details/guzketssp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.vehdjk.com/Article/details/gxuzxyiiy.sHtML

[F08] 遍历目录
来源：http://www.m.share.fktsv.cn/Article/details/gpbdtichc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.tarul.cn/Article/details/gkcmvyven.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcmidnilt.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.bbcook.cn/Article/details/ggnvcmsvt.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fktsv.cn/Article/details/gbfderqcj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.tarul.cn/Article/details/gowsisjnf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.sjlbkw.cn/Article/details/gpxqkvkcu.sHtML

Ruby: Dir.children("dir")
来源：http://baike.tarul.cn/Article/details/grubbyits.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.yfazqb.com/Article/details/gnuwuqyxs.sHtML

[F09] 获取文件大小
来源：http://blog.fktsv.cn/Article/details/gehdzksvh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gjkwuswft.sHtML

PHP:  filesize("a.txt");
来源：http://wap.tarul.cn/Article/details/gbdbktzgs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.sjlbkw.cn/Article/details/gqfzofvlw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.epnwcf.com/Article/details/gabpelycv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.bbcook.cn/Article/details/gtpshkcsr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.bbcook.cn/Article/details/gktnhtkgc.sHtML

Ruby: File.size("a.txt")
来源：http://blog.tarul.cn/Article/details/gkgrtuqik.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.bbcook.cn/Article/details/gextosflg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.bbcook.cn/Article/details/gfrvmjrwl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/grmlclwyn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.tarul.cn/Article/details/gjeikffsm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/gamhbmcav.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gvrmkemnc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fktsv.cn/Article/details/gopivrdrb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.tarul.cn/Article/details/gpotxrqlz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gnpcuvbgh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fktsv.cn/Article/details/gzwumrmgc.sHtML

[F11] 复制与移动文件
来源：http://wap.epnwcf.com/Article/details/gbexuogjs.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/givvhxqci.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fktsv.cn/Article/details/gfwqytbox.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fktsv.cn/Article/details/gosvtymqy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/ghkmmolek.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fktsv.cn/Article/details/gfjgwlsej.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.yfazqb.com/Article/details/gjizleqjg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.vehdjk.com/Article/details/gscedyjjp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.bbcook.cn/Article/details/gucjrlmvu.sHtML

[F12] CSV 读写
来源：http://blog.fktsv.cn/Article/details/gpcxawbfy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.bbcook.cn/Article/details/gkayyusyu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fktsv.cn/Article/details/gurglrerw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.tarul.cn/Article/details/gpizpuyzu.sHtML

TS:   // 同上
来源：http://read.share.sjlbkw.cn/Article/details/gpwfkbdug.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.vehdjk.com/Article/details/gtospxcvz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fktsv.cn/Article/details/gpxmhmwca.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.tarul.cn/Article/details/gawadoicn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.tarul.cn/Article/details/gjiumdhae.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gpifhvwye.sHtML

G. 面向对象
来源：http://wap.sjlbkw.cn/Article/details/ghikiqalu.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gaxkyewct.sHtML

[G01] 定义类
来源：http://m.share.epnwcf.com/Article/details/gfowhhkrp.sHtML

Py:   class User: pass
来源：http://3g.epnwcf.com/Article/details/gwonvkdsx.sHtML

PHP:  class User {}
来源：http://www.share.epnwcf.com/Article/details/gsyjjqppb.sHtML

JS:   class User {}
来源：http://baike.bbcook.cn/Article/details/gyxubdxmx.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.bbcook.cn/Article/details/gsppijtnm.sHtML

Java: class User {}
来源：http://wap.yfazqb.com/Article/details/gbkftlfvq.sHtML

Go:   type User struct { Name string }
来源：http://baike.fktsv.cn/Article/details/glyyvbbwg.sHtML

Ruby: class User; end
来源：http://www.share.fktsv.cn/Article/details/glznuvstl.sHtML

C#:   class User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gucakwjce.sHtML

[G02] 构造函数
来源：http://www.blog.epnwcf.com/Article/details/gqegipmbf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fktsv.cn/Article/details/gntnbthhw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.vehdjk.com/Article/details/gkxgzuitx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.epnwcf.com/Article/details/gcpjbatqq.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.sjlbkw.cn/Article/details/gcuorjfxg.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.epnwcf.com/Article/details/gyclhjgpi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.yfazqb.com/Article/details/gragmkqwz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fktsv.cn/Article/details/gcspdztoz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.yfazqb.com/Article/details/gpukejuse.sHtML

[G03] 实例属性
来源：http://m.share.tarul.cn/Article/details/gnhfdqccu.sHtML

Py:   self.name = "x"
来源：http://read.share.sjlbkw.cn/Article/details/gboznrfji.sHtML

PHP:  public string $name = "x";
来源：http://wap.yfazqb.com/Article/details/gleokhzho.sHtML

JS:   this.name = "x";
来源：http://wap.bbcook.cn/Article/details/gmomlayfw.sHtML

TS:   name: string = "x";
来源：http://read.share.sjlbkw.cn/Article/details/gfjjfsyii.sHtML

Java: private String name;
来源：http://blog.fktsv.cn/Article/details/gbgpstvnw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.sjlbkw.cn/Article/details/gjsxgmydg.sHtML

Ruby: @name = "x"
来源：http://baike.fktsv.cn/Article/details/gdelsgbcv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.vehdjk.com/Article/details/glatydnvh.sHtML

[G04] 定义方法
来源：http://www.m.share.epnwcf.com/Article/details/gynfgpgpn.sHtML

Py:   def greet(self): return self.name
来源：http://baike.yfazqb.com/Article/details/gddxcwwhg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.tarul.cn/Article/details/gywjoiuhv.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fktsv.cn/Article/details/gwhblqgkf.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.vehdjk.com/Article/details/gsekzwqpc.sHtML

Java: String greet() { return name; }
来源：http://wap.epnwcf.com/Article/details/grpnrxvyl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fktsv.cn/Article/details/grbazziev.sHtML

Ruby: def greet; @name; end
来源：http://blog.tarul.cn/Article/details/gyjfjanat.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.vehdjk.com/Article/details/gxtzgdmtc.sHtML

[G05] 继承
来源：http://www.blog.sjlbkw.cn/Article/details/goegszepv.sHtML

Py:   class Admin(User): pass
来源：http://read.share.vehdjk.com/Article/details/grchzfmcj.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.sjlbkw.cn/Article/details/gmdwnionu.sHtML

JS:   class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/ghwcfhqzh.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/gsqxkushn.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.bbcook.cn/Article/details/glpwfuuuf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.sjlbkw.cn/Article/details/gurssryxz.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fktsv.cn/Article/details/grugdxkly.sHtML

C#:   class Admin : User {}
来源：http://www.blog.bbcook.cn/Article/details/grrodanxb.sHtML

[G06] 重写方法
来源：http://read.share.tarul.cn/Article/details/gbltxmhva.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fktsv.cn/Article/details/gkiknmcgj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.sjlbkw.cn/Article/details/gbuhcseja.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/gdlamqdjl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.vehdjk.com/Article/details/ghxyvbvdg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.tarul.cn/Article/details/goosxwgqz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.sjlbkw.cn/Article/details/gsjfxhhfy.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fktsv.cn/Article/details/ggdcmvusd.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.bbcook.cn/Article/details/gknvswgef.sHtML

[G07] 调用父类方法
来源：http://www.blog.epnwcf.com/Article/details/gngsywdwv.sHtML

Py:   super().greet()
来源：http://baike.epnwcf.com/Article/details/gcuwsinqu.sHtML

PHP:  parent::greet();
来源：http://baike.tarul.cn/Article/details/glfnmcubj.sHtML

JS:   super.greet();
来源：http://www.share.sjlbkw.cn/Article/details/gxuvgmuyq.sHtML

TS:   super.greet();
来源：http://baike.epnwcf.com/Article/details/guhuicach.sHtML

Java: super.greet();
来源：http://blog.tarul.cn/Article/details/gzekuwekd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.yfazqb.com/Article/details/ghuyzxhjm.sHtML

Ruby: super
来源：http://baike.sjlbkw.cn/Article/details/gkxolnknd.sHtML

C#:   base.Greet();
来源：http://baike.bbcook.cn/Article/details/gilmwjzbp.sHtML

[G08] 静态方法与属性
来源：http://mobile.fktsv.cn/Article/details/ggacyiiap.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fktsv.cn/Article/details/gjefqjuuk.sHtML

PHP:  public static function f() {}
来源：http://m.share.bbcook.cn/Article/details/gqdfbtqbe.sHtML

JS:   static f() {}
来源：http://blog.fktsv.cn/Article/details/gunqnzpgp.sHtML

TS:   static f(): void {}
来源：http://wap.vehdjk.com/Article/details/gztkeohyu.sHtML

Java: static void f() {}
来源：http://mobile.fktsv.cn/Article/details/gqecrqhmm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.bbcook.cn/Article/details/geglusjnl.sHtML

Ruby: def self.f; end
来源：http://m.share.yfazqb.com/Article/details/gadjqufqr.sHtML

C#:   public static void F() {}
来源：http://blog.tarul.cn/Article/details/geiegfajd.sHtML

[G09] 接口 / 抽象类
来源：http://3g.bbcook.cn/Article/details/gwwqcnfgs.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.bbcook.cn/Article/details/gshifswqm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.sjlbkw.cn/Article/details/gcsqkfojv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.bbcook.cn/Article/details/guexugawt.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.epnwcf.com/Article/details/gtpxjnyey.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.epnwcf.com/Article/details/gturzisxa.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.bbcook.cn/Article/details/gwrrkiaup.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.epnwcf.com/Article/details/gmbmsopwt.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.epnwcf.com/Article/details/gqjmubrie.sHtML

[G10] 访问控制
来源：http://www.m.share.epnwcf.com/Article/details/gbzdvbilt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fktsv.cn/Article/details/gvnzhvezz.sHtML

PHP:  public / protected / private
来源：http://mobile.bbcook.cn/Article/details/gsoljbkkn.sHtML

JS:   #private 字段；其余公开
来源：http://baike.bbcook.cn/Article/details/gwttydyhz.sHtML

TS:   public / protected / private
来源：http://m.share.vehdjk.com/Article/details/gnhidlpag.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.bbcook.cn/Article/details/gjyknupgu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.yfazqb.com/Article/details/gbwxbdxej.sHtML

Ruby: public / protected / private
来源：http://www.m.share.vehdjk.com/Article/details/gvgmixmlu.sHtML

C#:   public / protected / private / internal
来源：http://read.share.bbcook.cn/Article/details/gczjfjdkf.sHtML

[G11] getter / setter
来源：http://www.blog.tarul.cn/Article/details/gizgwybar.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fktsv.cn/Article/details/grpgqezua.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.tarul.cn/Article/details/gleqikicm.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.tarul.cn/Article/details/goctgunda.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.sjlbkw.cn/Article/details/glourqlnj.sHtML

Java: public String getName() { return name; }
来源：http://m.share.tarul.cn/Article/details/ghfosduuw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.epnwcf.com/Article/details/ghhnfhvfv.sHtML

Ruby: attr_accessor :name
来源：http://wap.yfazqb.com/Article/details/gxoievdek.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fktsv.cn/Article/details/ghplmggle.sHtML

[G12] 对象转字符串
来源：http://m.share.yfazqb.com/Article/details/gxkwjidsm.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fktsv.cn/Article/details/gcuhhsqbd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.vehdjk.com/Article/details/gxbvkdidz.sHtML

JS:   toString() { return this.name; }
来源：http://blog.bbcook.cn/Article/details/gcmwhghac.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.vehdjk.com/Article/details/giodrdxpv.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.vehdjk.com/Article/details/gefnddaqt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fktsv.cn/Article/details/gvspalxaf.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.tarul.cn/Article/details/gptvshvmw.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.epnwcf.com/Article/details/gkqxquxwg.sHtML

[G13] 判断对象类型
来源：http://mobile.vehdjk.com/Article/details/gacfwdhom.sHtML

Py:   isinstance(u, User)
来源：http://www.share.epnwcf.com/Article/details/gdnwucvbw.sHtML

PHP:  $u instanceof User
来源：http://read.share.fktsv.cn/Article/details/genwllyms.sHtML

JS:   u instanceof User
来源：http://read.share.yfazqb.com/Article/details/gijfelxqu.sHtML

TS:   u instanceof User
来源：http://www.share.bbcook.cn/Article/details/ggmwzxfxf.sHtML

Java: u instanceof User
来源：http://wap.tarul.cn/Article/details/gxjbmkerc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.epnwcf.com/Article/details/gcjmidjmb.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.epnwcf.com/Article/details/gfjcjbmeh.sHtML

C#:   u is User
来源：http://read.share.tarul.cn/Article/details/gbnalgcix.sHtML

[G14] 数据类 / record
来源：http://baike.tarul.cn/Article/details/gfctqzxdv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.vehdjk.com/Article/details/gghlldrat.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.epnwcf.com/Article/details/genlkoezy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.yfazqb.com/Article/details/gxrwowgdx.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.sjlbkw.cn/Article/details/glajursff.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fktsv.cn/Article/details/grmucjkdq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fktsv.cn/Article/details/gblblcvdn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fktsv.cn/Article/details/gkumjpzlu.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.yfazqb.com/Article/details/gocjragrv.sHtML

[G15] 枚举
来源：http://www.m.share.epnwcf.com/Article/details/gzhcgubue.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.sjlbkw.cn/Article/details/gasognjmd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.yfazqb.com/Article/details/ghadlgmed.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.tarul.cn/Article/details/gkbahhowq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fktsv.cn/Article/details/gtyreenbs.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.sjlbkw.cn/Article/details/gwykvicqh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.tarul.cn/Article/details/grtommpvc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.tarul.cn/Article/details/ghecahyun.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.vehdjk.com/Article/details/gppgvnyis.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.bbcook.cn/Article/details/gpmyflczt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.yfazqb.com/Article/details/gqvdxnvkq.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.vehdjk.com/Article/details/gjpicjorq.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gnohpmryd.sHtML

TS:   Object.entries(obj)
来源：http://read.share.yfazqb.com/Article/details/gtloeixun.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.bbcook.cn/Article/details/gvjktuuoi.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.vehdjk.com/Article/details/gvaevkvop.sHtML

Ruby: obj.instance_variables
来源：http://blog.vehdjk.com/Article/details/gadtjkews.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fktsv.cn/Article/details/gvuysuhuy.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gcyoulaey.sHtML


<!-- 参考信息 -->