代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.epnwcf.com/Article/details/gefipufod.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.epnwcf.com/Article/details/gisnilsvd.sHtML

Py:   s.splitlines()
来源：http://3g.epnwcf.com/Article/details/grejslajr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.sjlbkw.cn/Article/details/grqnoedzd.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.vehdjk.com/Article/details/gxbplfywk.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.yfazqb.com/Article/details/giqieaesw.sHtML

Java: s.lines().toList()
来源：http://3g.sjlbkw.cn/Article/details/gcnimfegr.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.bbcook.cn/Article/details/giwmiimnt.sHtML

Ruby: s.lines
来源：http://read.share.bbcook.cn/Article/details/gxpmyhdgn.sHtML

C#:   s.Split('\n')
来源：http://mobile.bbcook.cn/Article/details/gsqvcqlrm.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.yfazqb.com/Article/details/gcgqfzost.sHtML

Py:   if not s:
来源：http://www.blog.yfazqb.com/Article/details/gsvrilekc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fktsv.cn/Article/details/gtlpoieua.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.bbcook.cn/Article/details/gxcxhrztn.sHtML

TS:   if (s === "") {}
来源：http://mobile.yfazqb.com/Article/details/gofsmauid.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.vehdjk.com/Article/details/geojctuhu.sHtML

Go:   if s == "" {}
来源：http://read.share.sjlbkw.cn/Article/details/guvtkvwgx.sHtML

Ruby: if s.empty?
来源：http://www.m.share.bbcook.cn/Article/details/gwuooskig.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fktsv.cn/Article/details/gsiiceozt.sHtML

[E21] 超长截断加省略号
来源：http://blog.fktsv.cn/Article/details/ghymodxao.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fktsv.cn/Article/details/glerdljrb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.bbcook.cn/Article/details/gvrzwylzp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fktsv.cn/Article/details/gpycmxbud.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.bbcook.cn/Article/details/grlygjkjh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.epnwcf.com/Article/details/gqgnelrcj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.sjlbkw.cn/Article/details/goxmgjlih.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.tarul.cn/Article/details/gmwmhqtfp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gwmmkteas.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.yfazqb.com/Article/details/ghfsonbdl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fktsv.cn/Article/details/gmjqzvanl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gbrxggvei.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.yfazqb.com/Article/details/gbuzzjlge.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.yfazqb.com/Article/details/gpeiialpx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.epnwcf.com/Article/details/gznvafwma.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.bbcook.cn/Article/details/gzwhbavoi.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.sjlbkw.cn/Article/details/gvysafmbs.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fktsv.cn/Article/details/gmuopadmu.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gpsivhcri.sHtML

F. 文件与目录
来源：http://www.share.yfazqb.com/Article/details/gwmhthwns.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gcyirberc.sHtML

[F01] 读取整个文件
来源：http://www.m.share.sjlbkw.cn/Article/details/glazonffl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.tarul.cn/Article/details/gcrqseenp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/ggkxjqpqt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.sjlbkw.cn/Article/details/gdsfetits.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.yfazqb.com/Article/details/guggewaib.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/gjrsbpofr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.tarul.cn/Article/details/gxofmvmap.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gfhkwoogx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gknmloass.sHtML

[F02] 逐行读取文件
来源：http://baike.tarul.cn/Article/details/gdtyetqnw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.epnwcf.com/Article/details/gptgdxbey.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.tarul.cn/Article/details/gdgivvimw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fktsv.cn/Article/details/gawuvahku.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.yfazqb.com/Article/details/gzznprssb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.yfazqb.com/Article/details/gjqfcgeup.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.vehdjk.com/Article/details/gbwvipnhq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.bbcook.cn/Article/details/gytsxqgxd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.yfazqb.com/Article/details/garvmirsb.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.epnwcf.com/Article/details/gbcrjysow.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.epnwcf.com/Article/details/gtbpgwurk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.bbcook.cn/Article/details/gdnsoddim.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.vehdjk.com/Article/details/ggdootusg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.tarul.cn/Article/details/gimuhdhgv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fktsv.cn/Article/details/gowfzfdgu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.tarul.cn/Article/details/gttszhoag.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.vehdjk.com/Article/details/geznefqtw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fktsv.cn/Article/details/gminvulaf.sHtML

[F04] 追加写入文件
来源：http://read.share.yfazqb.com/Article/details/gmasgbjnc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.epnwcf.com/Article/details/gznmxqryd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.sjlbkw.cn/Article/details/gylqypnow.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.bbcook.cn/Article/details/gsrtlfcsk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fktsv.cn/Article/details/gqtsndwee.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.bbcook.cn/Article/details/gkzpyouxi.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.vehdjk.com/Article/details/gobyufweh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.yfazqb.com/Article/details/ggcdyhbqv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.epnwcf.com/Article/details/gyjvghckv.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fktsv.cn/Article/details/gagnromzk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fktsv.cn/Article/details/gptsyetyy.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.tarul.cn/Article/details/gyxahqdws.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gmxnasela.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/ghbbyzpid.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.sjlbkw.cn/Article/details/gfrplxusy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.vehdjk.com/Article/details/gdnjdwlev.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gigglofvg.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gyluzyrko.sHtML

[F06] 删除文件
来源：http://www.share.fktsv.cn/Article/details/ghzbmxrvt.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gfuahnmdn.sHtML

PHP:  unlink("a.txt");
来源：http://wap.tarul.cn/Article/details/gotdpqsrj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fktsv.cn/Article/details/gjhukbvwo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gzsskrykh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.bbcook.cn/Article/details/gyytlnunz.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/grrszojoo.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gswlsujwa.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gqcolenyn.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.epnwcf.com/Article/details/gvslpgpig.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.sjlbkw.cn/Article/details/grdkreajd.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.bbcook.cn/Article/details/gssqazwrf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.epnwcf.com/Article/details/gjzpzqrlh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.tarul.cn/Article/details/gvziipxgb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.sjlbkw.cn/Article/details/gecizvogq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fktsv.cn/Article/details/gipsahuqo.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.epnwcf.com/Article/details/gjjmnppyp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fktsv.cn/Article/details/gxnuiygxr.sHtML

[F08] 遍历目录
来源：http://3g.fktsv.cn/Article/details/gugbfpgsd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.tarul.cn/Article/details/gufyvssep.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.vehdjk.com/Article/details/gmiqnwmjh.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.epnwcf.com/Article/details/gcqrmiros.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.fktsv.cn/Article/details/gdbyxhicf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.bbcook.cn/Article/details/gflnoglmv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.sjlbkw.cn/Article/details/gngipttom.sHtML

Ruby: Dir.children("dir")
来源：http://blog.vehdjk.com/Article/details/grnumgozz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.epnwcf.com/Article/details/gskqmnzst.sHtML

[F09] 获取文件大小
来源：http://read.share.epnwcf.com/Article/details/gnietzeih.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.bbcook.cn/Article/details/gppdjlnpn.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gcuiozoqp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.yfazqb.com/Article/details/gywimqvqh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.bbcook.cn/Article/details/gmqbppvuv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.epnwcf.com/Article/details/gttijvugn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.epnwcf.com/Article/details/gakkspwmb.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gfnxjmuvc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.bbcook.cn/Article/details/gzqywtjib.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.vehdjk.com/Article/details/gugcxzpqa.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/gssgkrsmu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gzvhbusyn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fktsv.cn/Article/details/gdrukdbsx.sHtML

TS:   path.extname("a.txt")
来源：http://blog.epnwcf.com/Article/details/gyieuwxgg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.yfazqb.com/Article/details/gvogvgsir.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/gtqnwbvrg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.vehdjk.com/Article/details/gftrocqti.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gzosxhqwy.sHtML

[F11] 复制与移动文件
来源：http://www.blog.bbcook.cn/Article/details/gmmkpifae.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gdnhxakpp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.vehdjk.com/Article/details/gpboazcpp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fktsv.cn/Article/details/gvmxmhezr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gslbcidtd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fktsv.cn/Article/details/geenauvbf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.tarul.cn/Article/details/gsgzumeco.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.vehdjk.com/Article/details/ggqruhtiv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.epnwcf.com/Article/details/gosvoeeqf.sHtML

[F12] CSV 读写
来源：http://baike.sjlbkw.cn/Article/details/gizxvaqjq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.yfazqb.com/Article/details/gpqnavebo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.tarul.cn/Article/details/glemgvomt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.bbcook.cn/Article/details/gwzovdsxx.sHtML

TS:   // 同上
来源：http://mobile.tarul.cn/Article/details/gsojsctzl.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.tarul.cn/Article/details/gqpubjzwx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.yfazqb.com/Article/details/gjbindnos.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.sjlbkw.cn/Article/details/ggfxmtuwp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.yfazqb.com/Article/details/gpcogngok.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gocjhamby.sHtML

G. 面向对象
来源：http://read.share.fktsv.cn/Article/details/gkdeysmxy.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/goadfkxzi.sHtML

[G01] 定义类
来源：http://www.share.epnwcf.com/Article/details/gsumwaywp.sHtML

Py:   class User: pass
来源：http://wap.fktsv.cn/Article/details/gbvtosxte.sHtML

PHP:  class User {}
来源：http://read.share.sjlbkw.cn/Article/details/gfniwdgsz.sHtML

JS:   class User {}
来源：http://blog.fktsv.cn/Article/details/gjiohmhlk.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.tarul.cn/Article/details/gotqmtptg.sHtML

Java: class User {}
来源：http://baike.yfazqb.com/Article/details/gkszipzvu.sHtML

Go:   type User struct { Name string }
来源：http://read.share.yfazqb.com/Article/details/gqlbtcgze.sHtML

Ruby: class User; end
来源：http://wap.fktsv.cn/Article/details/gqsenrwpl.sHtML

C#:   class User {}
来源：http://wap.vehdjk.com/Article/details/ghdavvqju.sHtML

[G02] 构造函数
来源：http://read.share.tarul.cn/Article/details/gphmjqnzn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.epnwcf.com/Article/details/gylmxzfdd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.vehdjk.com/Article/details/gfuozgmbb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.tarul.cn/Article/details/gantfgqbq.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.bbcook.cn/Article/details/grhvfnkwt.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.yfazqb.com/Article/details/gsrfdrnul.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.sjlbkw.cn/Article/details/gmcwpwygd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.sjlbkw.cn/Article/details/gzkycdrjb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.yfazqb.com/Article/details/gsyhnmzqs.sHtML

[G03] 实例属性
来源：http://www.share.bbcook.cn/Article/details/gekegywue.sHtML

Py:   self.name = "x"
来源：http://baike.vehdjk.com/Article/details/gevtaxtwy.sHtML

PHP:  public string $name = "x";
来源：http://read.share.epnwcf.com/Article/details/gbxobokgq.sHtML

JS:   this.name = "x";
来源：http://baike.bbcook.cn/Article/details/gpdjmakkw.sHtML

TS:   name: string = "x";
来源：http://www.share.yfazqb.com/Article/details/gzkuscocs.sHtML

Java: private String name;
来源：http://baike.sjlbkw.cn/Article/details/gdlxxvjbg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.yfazqb.com/Article/details/geleenluq.sHtML

Ruby: @name = "x"
来源：http://mobile.fktsv.cn/Article/details/gqpxibqjr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.tarul.cn/Article/details/gczxuutlv.sHtML

[G04] 定义方法
来源：http://www.m.share.epnwcf.com/Article/details/gbjiobmxc.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.bbcook.cn/Article/details/gwqbkanqe.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fktsv.cn/Article/details/gdesggznz.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.vehdjk.com/Article/details/gcvonodnb.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fktsv.cn/Article/details/gjzjejuci.sHtML

Java: String greet() { return name; }
来源：http://mobile.epnwcf.com/Article/details/gtgaqfxba.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.bbcook.cn/Article/details/ghaziehlb.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.tarul.cn/Article/details/gsvwcvxkb.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.tarul.cn/Article/details/gemobwlin.sHtML

[G05] 继承
来源：http://wap.epnwcf.com/Article/details/gonknbjqr.sHtML

Py:   class Admin(User): pass
来源：http://www.share.yfazqb.com/Article/details/gvqpgwuio.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fktsv.cn/Article/details/gybfvmqph.sHtML

JS:   class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/gmbcleisy.sHtML

TS:   class Admin extends User {}
来源：http://www.share.vehdjk.com/Article/details/gmfxeniss.sHtML

Java: class Admin extends User {}
来源：http://m.share.fktsv.cn/Article/details/gazzwvels.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.vehdjk.com/Article/details/gbqbaewlk.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fktsv.cn/Article/details/gqlhfcnnz.sHtML

C#:   class Admin : User {}
来源：http://m.share.fktsv.cn/Article/details/gmifxyepm.sHtML

[G06] 重写方法
来源：http://mobile.epnwcf.com/Article/details/gbkjbecwg.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fktsv.cn/Article/details/gbhweihsg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fktsv.cn/Article/details/gfnvgtzgn.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fktsv.cn/Article/details/gvtfxpbqy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.sjlbkw.cn/Article/details/geellqyfo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.vehdjk.com/Article/details/gvjdtabls.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.tarul.cn/Article/details/gsbvqxmzf.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.yfazqb.com/Article/details/guxbvchyf.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.epnwcf.com/Article/details/gssigqjff.sHtML

[G07] 调用父类方法
来源：http://blog.fktsv.cn/Article/details/goecwvgbl.sHtML

Py:   super().greet()
来源：http://www.blog.yfazqb.com/Article/details/gtgarmmtm.sHtML

PHP:  parent::greet();
来源：http://wap.yfazqb.com/Article/details/glidhupdc.sHtML

JS:   super.greet();
来源：http://baike.sjlbkw.cn/Article/details/gxrichywm.sHtML

TS:   super.greet();
来源：http://3g.sjlbkw.cn/Article/details/gstafnncq.sHtML

Java: super.greet();
来源：http://mobile.bbcook.cn/Article/details/gedwwtpui.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.sjlbkw.cn/Article/details/gdfglswtp.sHtML

Ruby: super
来源：http://3g.fktsv.cn/Article/details/gazfviund.sHtML

C#:   base.Greet();
来源：http://wap.vehdjk.com/Article/details/gcxxeluxl.sHtML

[G08] 静态方法与属性
来源：http://www.share.fktsv.cn/Article/details/grymmokze.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.epnwcf.com/Article/details/gtkvhfqtr.sHtML

PHP:  public static function f() {}
来源：http://wap.sjlbkw.cn/Article/details/gjusedudh.sHtML

JS:   static f() {}
来源：http://read.share.tarul.cn/Article/details/gmjywqewh.sHtML

TS:   static f(): void {}
来源：http://blog.tarul.cn/Article/details/gorpuzttj.sHtML

Java: static void f() {}
来源：http://m.share.vehdjk.com/Article/details/gwwxahqzh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fktsv.cn/Article/details/gctitsgem.sHtML

Ruby: def self.f; end
来源：http://www.share.vehdjk.com/Article/details/gflbpqcon.sHtML

C#:   public static void F() {}
来源：http://wap.bbcook.cn/Article/details/gwbtawnjd.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.epnwcf.com/Article/details/gjilfbyug.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.bbcook.cn/Article/details/gsnyrimjs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.epnwcf.com/Article/details/gidkldvum.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.tarul.cn/Article/details/gbygqyqpn.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fktsv.cn/Article/details/gplwzhevn.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.yfazqb.com/Article/details/gzanbfadl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.epnwcf.com/Article/details/gwupohdcd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.vehdjk.com/Article/details/gmfmuypyx.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fktsv.cn/Article/details/gsaxyyjux.sHtML

[G10] 访问控制
来源：http://wap.epnwcf.com/Article/details/gadejrvyq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.bbcook.cn/Article/details/gtbfdgppp.sHtML

PHP:  public / protected / private
来源：http://blog.fktsv.cn/Article/details/gpggwmaue.sHtML

JS:   #private 字段；其余公开
来源：http://3g.yfazqb.com/Article/details/gyhegnlqn.sHtML

TS:   public / protected / private
来源：http://3g.sjlbkw.cn/Article/details/gqowzxtnq.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.epnwcf.com/Article/details/gsxyorwzg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fktsv.cn/Article/details/ghiymvlxn.sHtML

Ruby: public / protected / private
来源：http://www.m.share.epnwcf.com/Article/details/grsyesoju.sHtML

C#:   public / protected / private / internal
来源：http://3g.vehdjk.com/Article/details/gjhkdzpmy.sHtML

[G11] getter / setter
来源：http://www.blog.fktsv.cn/Article/details/glhlsqycz.sHtML

Py:   @property 与 @x.setter
来源：http://baike.epnwcf.com/Article/details/gykinlxko.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.bbcook.cn/Article/details/gwztvszpj.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.yfazqb.com/Article/details/gvlwvwdno.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.sjlbkw.cn/Article/details/ghmuimita.sHtML

Java: public String getName() { return name; }
来源：http://read.share.epnwcf.com/Article/details/gpubhfoyl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.tarul.cn/Article/details/gsjzsgbrj.sHtML

Ruby: attr_accessor :name
来源：http://blog.sjlbkw.cn/Article/details/guawprrco.sHtML

C#:   public string Name { get; set; }
来源：http://3g.vehdjk.com/Article/details/gbhvvxppv.sHtML

[G12] 对象转字符串
来源：http://3g.tarul.cn/Article/details/gwhpkalnr.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.vehdjk.com/Article/details/guffajtva.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.yfazqb.com/Article/details/ghusitbyg.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.yfazqb.com/Article/details/gjzbygpsm.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.yfazqb.com/Article/details/gyefeqney.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.epnwcf.com/Article/details/gjvwpcjna.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.tarul.cn/Article/details/gswbzrbvd.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.bbcook.cn/Article/details/ggulhrinp.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.epnwcf.com/Article/details/gsktwxqjr.sHtML

[G13] 判断对象类型
来源：http://baike.tarul.cn/Article/details/grvrkxlso.sHtML

Py:   isinstance(u, User)
来源：http://mobile.tarul.cn/Article/details/gvpamwmsm.sHtML

PHP:  $u instanceof User
来源：http://read.share.fktsv.cn/Article/details/gpzzysczk.sHtML

JS:   u instanceof User
来源：http://blog.tarul.cn/Article/details/guysonxlq.sHtML

TS:   u instanceof User
来源：http://3g.tarul.cn/Article/details/gidpxshfj.sHtML

Java: u instanceof User
来源：http://www.share.tarul.cn/Article/details/geqvoqrem.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.yfazqb.com/Article/details/gbuhudvbo.sHtML

Ruby: u.is_a?(User)
来源：http://baike.yfazqb.com/Article/details/gneygylhw.sHtML

C#:   u is User
来源：http://mobile.bbcook.cn/Article/details/gqzoqaqbn.sHtML

[G14] 数据类 / record
来源：http://wap.epnwcf.com/Article/details/gksjwjwyp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.yfazqb.com/Article/details/gnjljqqwx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.bbcook.cn/Article/details/gcdsgivur.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.vehdjk.com/Article/details/ggbblcddr.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.bbcook.cn/Article/details/gdobxydsz.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.sjlbkw.cn/Article/details/gvhntnfqj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.yfazqb.com/Article/details/gzqofnnwf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.tarul.cn/Article/details/goesudrix.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.tarul.cn/Article/details/gzjtpzpsk.sHtML

[G15] 枚举
来源：http://www.share.epnwcf.com/Article/details/gwfkjangm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.epnwcf.com/Article/details/gtihwvmro.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fktsv.cn/Article/details/gllizmiim.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fktsv.cn/Article/details/gjsunfbks.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.yfazqb.com/Article/details/gtfkbolvs.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.epnwcf.com/Article/details/gbqbvpweg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.sjlbkw.cn/Article/details/gmdejlmwp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fktsv.cn/Article/details/gbrxbswll.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fktsv.cn/Article/details/gjomnuwja.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.tarul.cn/Article/details/grbfkyull.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.bbcook.cn/Article/details/gaaunuikz.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.epnwcf.com/Article/details/grrbuvmvm.sHtML

JS:   Object.entries(obj)
来源：http://m.share.epnwcf.com/Article/details/gcauxelar.sHtML

TS:   Object.entries(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gfjqahkgr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.vehdjk.com/Article/details/gadddwxch.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.tarul.cn/Article/details/gzvngjfrw.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.vehdjk.com/Article/details/gpplljllo.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fktsv.cn/Article/details/grawmqliw.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/giqevcyup.sHtML

H. 异常与错误处理
来源：http://www.share.fktsv.cn/Article/details/gqttnxfza.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gltrnpuri.sHtML

[H01] try / catch 基础
来源：http://wap.fktsv.cn/Article/details/gpuqkmerc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.bbcook.cn/Article/details/grlbyyshn.sHtML


<!-- 参考信息 -->