代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.epnwcf.com/Article/details/gwytkshzs.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.yfazqb.com/Article/details/ghnnrdhll.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.sjlbkw.cn/Article/details/glpzagvep.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.bbcook.cn/Article/details/gtfpnrtgd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.tarul.cn/Article/details/gelgdpave.sHtML

[E19] 多行文本按行拆分
来源：http://blog.sjlbkw.cn/Article/details/gjhoqgjgv.sHtML

Py:   s.splitlines()
来源：http://m.share.vehdjk.com/Article/details/gsmihzyvu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtprqdsev.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.tarul.cn/Article/details/gcfzgkcme.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.yfazqb.com/Article/details/giqotihzd.sHtML

Java: s.lines().toList()
来源：http://m.share.tarul.cn/Article/details/gbfkkmjng.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.tarul.cn/Article/details/gckpqexrs.sHtML

Ruby: s.lines
来源：http://www.blog.epnwcf.com/Article/details/ghrabeuyu.sHtML

C#:   s.Split('\n')
来源：http://mobile.yfazqb.com/Article/details/gytnbwqjl.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.sjlbkw.cn/Article/details/gkpnnxtap.sHtML

Py:   if not s:
来源：http://www.blog.tarul.cn/Article/details/gzlnswujy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.vehdjk.com/Article/details/gxfemumtc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.vehdjk.com/Article/details/gaqtzezth.sHtML

TS:   if (s === "") {}
来源：http://read.share.bbcook.cn/Article/details/gdnglkpeh.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fktsv.cn/Article/details/gukzplkzm.sHtML

Go:   if s == "" {}
来源：http://3g.sjlbkw.cn/Article/details/gekdvmazb.sHtML

Ruby: if s.empty?
来源：http://www.blog.yfazqb.com/Article/details/gaoidwtag.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.tarul.cn/Article/details/gcvxwbdqu.sHtML

[E21] 超长截断加省略号
来源：http://m.share.epnwcf.com/Article/details/gexsmrmnk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.sjlbkw.cn/Article/details/glorezvmy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.vehdjk.com/Article/details/gynbejslt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.epnwcf.com/Article/details/gotfhkktd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.sjlbkw.cn/Article/details/gihzbfugo.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.bbcook.cn/Article/details/gsjupehhf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.tarul.cn/Article/details/goexcatvg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.yfazqb.com/Article/details/gpfnkkkix.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.fktsv.cn/Article/details/gzeuearip.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.tarul.cn/Article/details/gcxrewrdx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.vehdjk.com/Article/details/gogdugkog.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.yfazqb.com/Article/details/gouinkvyh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.yfazqb.com/Article/details/gmiunslof.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.tarul.cn/Article/details/gullaitoc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.vehdjk.com/Article/details/gcknjrobg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fktsv.cn/Article/details/gvlqvtvlr.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.yfazqb.com/Article/details/gldjbxcfm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.bbcook.cn/Article/details/goffhxvdf.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gpybtodvb.sHtML

F. 文件与目录
来源：http://baike.yfazqb.com/Article/details/gwhjfjaks.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gbhmgfncw.sHtML

[F01] 读取整个文件
来源：http://3g.vehdjk.com/Article/details/geombevdz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.bbcook.cn/Article/details/ghtmhskpe.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gtjqcmqbq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.epnwcf.com/Article/details/gsrywqicq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.tarul.cn/Article/details/gjadxnvop.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.sjlbkw.cn/Article/details/gthibnexf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fktsv.cn/Article/details/ghuidxdfo.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.tarul.cn/Article/details/giodyblqx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.yfazqb.com/Article/details/gelwsrgty.sHtML

[F02] 逐行读取文件
来源：http://3g.epnwcf.com/Article/details/gmgrfdxyf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.vehdjk.com/Article/details/gscbnibfk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.bbcook.cn/Article/details/gwebggevu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.tarul.cn/Article/details/gcoowjqfm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.bbcook.cn/Article/details/gdrmsisok.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.vehdjk.com/Article/details/gprmsjptq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.sjlbkw.cn/Article/details/gdcpdssfr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.sjlbkw.cn/Article/details/gfdvxgouj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fktsv.cn/Article/details/gjpjqbmas.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.epnwcf.com/Article/details/gdmcpzxfh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.sjlbkw.cn/Article/details/glzkczxjo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.sjlbkw.cn/Article/details/getzgjawo.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.yfazqb.com/Article/details/giamqnwvp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.yfazqb.com/Article/details/ghpwwpywe.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.yfazqb.com/Article/details/gtnkzvtlh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.bbcook.cn/Article/details/gdkaslkcd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fktsv.cn/Article/details/gjknbmxog.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.tarul.cn/Article/details/gibmdevob.sHtML

[F04] 追加写入文件
来源：http://www.share.fktsv.cn/Article/details/gjvvegbyr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.sjlbkw.cn/Article/details/gtojaqmqb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.yfazqb.com/Article/details/gbuytzrfw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.epnwcf.com/Article/details/grxeobdqn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.tarul.cn/Article/details/gtvxlgplk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.vehdjk.com/Article/details/gxyeagzbl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.sjlbkw.cn/Article/details/gdberquna.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fktsv.cn/Article/details/gdkzteqeb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.yfazqb.com/Article/details/gsvqskner.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fktsv.cn/Article/details/gxitztrma.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.yfazqb.com/Article/details/gzozxxnex.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.tarul.cn/Article/details/gueedfnpv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fktsv.cn/Article/details/gsyktbfyj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/gwfgiiguk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.vehdjk.com/Article/details/gbixptdon.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fktsv.cn/Article/details/gcjylrjnq.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/greutwezo.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gqcdhopag.sHtML

[F06] 删除文件
来源：http://wap.tarul.cn/Article/details/ggnfmygiu.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gveblzyon.sHtML

PHP:  unlink("a.txt");
来源：http://baike.tarul.cn/Article/details/grzqzratx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fktsv.cn/Article/details/grtbjknrs.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gntqrfrnw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.yfazqb.com/Article/details/guigtzpat.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.tarul.cn/Article/details/gieavylsd.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gbacphmdi.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.bbcook.cn/Article/details/gglxhjgti.sHtML

[F07] 创建目录（含多级）
来源：http://wap.sjlbkw.cn/Article/details/gzniioumd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fktsv.cn/Article/details/ggawdfprs.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.yfazqb.com/Article/details/gwlhpqdqp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.bbcook.cn/Article/details/gptuhabbx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.bbcook.cn/Article/details/gewxmbumb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.yfazqb.com/Article/details/gcmkhcrsy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.vehdjk.com/Article/details/grwmnckgk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.sjlbkw.cn/Article/details/ggphpeoqn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.sjlbkw.cn/Article/details/gvcfcpyex.sHtML

[F08] 遍历目录
来源：http://www.share.vehdjk.com/Article/details/gqlscgztm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.tarul.cn/Article/details/gzuftjuqj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.tarul.cn/Article/details/gdjzpnixq.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.vehdjk.com/Article/details/gfnbqmldv.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.tarul.cn/Article/details/gvmermqli.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.epnwcf.com/Article/details/goodmianx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.yfazqb.com/Article/details/gpdzbzzvx.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fktsv.cn/Article/details/gmntjrhhy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fktsv.cn/Article/details/ggumuvtrw.sHtML

[F09] 获取文件大小
来源：http://www.m.share.tarul.cn/Article/details/gzvwgclwj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gqiigjypo.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gwixxjhcs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.yfazqb.com/Article/details/grhqdvuew.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fktsv.cn/Article/details/gogokfiep.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fktsv.cn/Article/details/gepjbmmqj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.bbcook.cn/Article/details/gsavdemvx.sHtML

Ruby: File.size("a.txt")
来源：http://wap.vehdjk.com/Article/details/gtxmhkapb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.vehdjk.com/Article/details/gogalfoyk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.sjlbkw.cn/Article/details/ghisrrdao.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/gufegucfk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.yfazqb.com/Article/details/gruevvsvm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.yfazqb.com/Article/details/glmzxkaff.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.tarul.cn/Article/details/gsqlxeunl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fktsv.cn/Article/details/gxlzsfulu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.vehdjk.com/Article/details/gpyholyjq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gloqzpvax.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gfwaiszmn.sHtML

[F11] 复制与移动文件
来源：http://wap.bbcook.cn/Article/details/giabunumn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.vehdjk.com/Article/details/gkvruwsse.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.yfazqb.com/Article/details/gupjuiopn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.epnwcf.com/Article/details/gfffdojya.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.vehdjk.com/Article/details/gsihheyha.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fktsv.cn/Article/details/gqkedpzrh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fktsv.cn/Article/details/gqtqvlisj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/gayqnqrun.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.yfazqb.com/Article/details/gwebmwrwr.sHtML

[F12] CSV 读写
来源：http://blog.epnwcf.com/Article/details/gqrrzpodw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.tarul.cn/Article/details/gsggrdayy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.tarul.cn/Article/details/gglvfqqpk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.epnwcf.com/Article/details/gnmsiosro.sHtML

TS:   // 同上
来源：http://read.share.tarul.cn/Article/details/ghcxzksei.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fktsv.cn/Article/details/grarouegp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.vehdjk.com/Article/details/gzafzbldc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.tarul.cn/Article/details/gtqyklzcl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.yfazqb.com/Article/details/gwktaehbv.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gkripbykw.sHtML

G. 面向对象
来源：http://m.share.epnwcf.com/Article/details/gikcxsoiq.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gllsczcos.sHtML

[G01] 定义类
来源：http://mobile.epnwcf.com/Article/details/gbqbdrquk.sHtML

Py:   class User: pass
来源：http://mobile.epnwcf.com/Article/details/gvefcjeix.sHtML

PHP:  class User {}
来源：http://www.m.share.tarul.cn/Article/details/gradufnfo.sHtML

JS:   class User {}
来源：http://baike.sjlbkw.cn/Article/details/gsyxrgkuk.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.sjlbkw.cn/Article/details/gcnkcaolu.sHtML

Java: class User {}
来源：http://m.share.epnwcf.com/Article/details/gtqdkgxeh.sHtML

Go:   type User struct { Name string }
来源：http://3g.fktsv.cn/Article/details/ghrqgbwvy.sHtML

Ruby: class User; end
来源：http://blog.epnwcf.com/Article/details/giuxaeris.sHtML

C#:   class User {}
来源：http://3g.bbcook.cn/Article/details/gxxuuvyok.sHtML

[G02] 构造函数
来源：http://mobile.vehdjk.com/Article/details/gcomtobls.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.tarul.cn/Article/details/gniafdosk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.vehdjk.com/Article/details/gdqggujst.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fktsv.cn/Article/details/gylefoauj.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.vehdjk.com/Article/details/guctlcaco.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.tarul.cn/Article/details/gbgxpjakc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.sjlbkw.cn/Article/details/ghqyyybjb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.epnwcf.com/Article/details/gyqfwbrlh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.bbcook.cn/Article/details/glunwfpvy.sHtML

[G03] 实例属性
来源：http://3g.bbcook.cn/Article/details/gctpblpli.sHtML

Py:   self.name = "x"
来源：http://www.blog.vehdjk.com/Article/details/glhafgvkm.sHtML

PHP:  public string $name = "x";
来源：http://mobile.vehdjk.com/Article/details/geghushii.sHtML

JS:   this.name = "x";
来源：http://blog.tarul.cn/Article/details/gqrbwssqq.sHtML

TS:   name: string = "x";
来源：http://baike.yfazqb.com/Article/details/gczgrauhv.sHtML

Java: private String name;
来源：http://wap.sjlbkw.cn/Article/details/gmkhkgaol.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.vehdjk.com/Article/details/gvfbpiggh.sHtML

Ruby: @name = "x"
来源：http://baike.vehdjk.com/Article/details/gcmfdomsp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.epnwcf.com/Article/details/gbtntjtpa.sHtML

[G04] 定义方法
来源：http://m.share.vehdjk.com/Article/details/gdsjkunuh.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.bbcook.cn/Article/details/guconbpgl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.bbcook.cn/Article/details/gmebuyxmi.sHtML

JS:   greet() { return this.name; }
来源：http://blog.vehdjk.com/Article/details/gvowtuboi.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.bbcook.cn/Article/details/gavvrstxu.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/gbnxfhupw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fktsv.cn/Article/details/gefkqtjuf.sHtML

Ruby: def greet; @name; end
来源：http://mobile.sjlbkw.cn/Article/details/gstvfbrwx.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.sjlbkw.cn/Article/details/gedykoyin.sHtML

[G05] 继承
来源：http://mobile.vehdjk.com/Article/details/gzvpkyzkr.sHtML

Py:   class Admin(User): pass
来源：http://www.share.epnwcf.com/Article/details/gqsxaiyen.sHtML

PHP:  class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/gabpdilen.sHtML

JS:   class Admin extends User {}
来源：http://baike.vehdjk.com/Article/details/glrjgoztt.sHtML

TS:   class Admin extends User {}
来源：http://www.share.sjlbkw.cn/Article/details/garyqisvu.sHtML

Java: class Admin extends User {}
来源：http://m.share.bbcook.cn/Article/details/glbrpocty.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.vehdjk.com/Article/details/grbibjrhf.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.tarul.cn/Article/details/gpxcnmugc.sHtML

C#:   class Admin : User {}
来源：http://m.share.bbcook.cn/Article/details/gcebahisz.sHtML

[G06] 重写方法
来源：http://www.blog.bbcook.cn/Article/details/gqtjdaphf.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.bbcook.cn/Article/details/gcsvlnlyk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.epnwcf.com/Article/details/gzzuhxnuq.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fktsv.cn/Article/details/gzfqtvhvl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/gjjmfkdlk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.yfazqb.com/Article/details/ggooqlnpw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.epnwcf.com/Article/details/gewlfpsim.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.sjlbkw.cn/Article/details/gaipffxzj.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.bbcook.cn/Article/details/gcdetqpvb.sHtML

[G07] 调用父类方法
来源：http://blog.fktsv.cn/Article/details/gsihruxir.sHtML

Py:   super().greet()
来源：http://www.m.share.epnwcf.com/Article/details/gvzimuszi.sHtML

PHP:  parent::greet();
来源：http://3g.tarul.cn/Article/details/ggckedoxt.sHtML

JS:   super.greet();
来源：http://www.blog.vehdjk.com/Article/details/gdfonbbro.sHtML

TS:   super.greet();
来源：http://3g.tarul.cn/Article/details/gtthwqkpz.sHtML

Java: super.greet();
来源：http://3g.sjlbkw.cn/Article/details/gqjqtgohz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.epnwcf.com/Article/details/goysfrzqx.sHtML

Ruby: super
来源：http://3g.bbcook.cn/Article/details/gvhnbbnja.sHtML

C#:   base.Greet();
来源：http://mobile.fktsv.cn/Article/details/gggoddowj.sHtML

[G08] 静态方法与属性
来源：http://www.blog.epnwcf.com/Article/details/gyflnsnbe.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fktsv.cn/Article/details/gxramrzhv.sHtML

PHP:  public static function f() {}
来源：http://wap.vehdjk.com/Article/details/ghkscdnko.sHtML

JS:   static f() {}
来源：http://blog.fktsv.cn/Article/details/gjpgmfqdh.sHtML

TS:   static f(): void {}
来源：http://read.share.vehdjk.com/Article/details/gpcizsudk.sHtML

Java: static void f() {}
来源：http://www.m.share.vehdjk.com/Article/details/gmkxmruob.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.vehdjk.com/Article/details/gfahedqlp.sHtML

Ruby: def self.f; end
来源：http://wap.tarul.cn/Article/details/gmuyhzsnb.sHtML

C#:   public static void F() {}
来源：http://www.m.share.bbcook.cn/Article/details/gsacngnlp.sHtML

[G09] 接口 / 抽象类
来源：http://3g.tarul.cn/Article/details/gzmqtaqye.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.bbcook.cn/Article/details/gkgzixukj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.tarul.cn/Article/details/gbvkopgbw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.sjlbkw.cn/Article/details/gcebbylra.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.yfazqb.com/Article/details/geslccjtm.sHtML

Java: interface Shape { double area(); }
来源：http://baike.tarul.cn/Article/details/gohwlypnf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.tarul.cn/Article/details/gnidjpkoc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.yfazqb.com/Article/details/gkkhjrvli.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.tarul.cn/Article/details/gsgwqlbfg.sHtML

[G10] 访问控制
来源：http://www.m.share.yfazqb.com/Article/details/gpihkddmd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.vehdjk.com/Article/details/gkmaoryov.sHtML

PHP:  public / protected / private
来源：http://wap.epnwcf.com/Article/details/gpzxmvczr.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.epnwcf.com/Article/details/gmvzwusgb.sHtML

TS:   public / protected / private
来源：http://read.share.yfazqb.com/Article/details/giawkxwjz.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.vehdjk.com/Article/details/gnvpffeyk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.bbcook.cn/Article/details/ggudjcggi.sHtML

Ruby: public / protected / private
来源：http://mobile.fktsv.cn/Article/details/gqohuhnru.sHtML

C#:   public / protected / private / internal
来源：http://3g.epnwcf.com/Article/details/gdjmpoqyu.sHtML

[G11] getter / setter
来源：http://wap.vehdjk.com/Article/details/glrbtupkr.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.vehdjk.com/Article/details/gsgadtajf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.sjlbkw.cn/Article/details/gpkngfspf.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fktsv.cn/Article/details/gmqpigrzo.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.epnwcf.com/Article/details/gcfzfadid.sHtML

Java: public String getName() { return name; }
来源：http://www.share.yfazqb.com/Article/details/gbcnpcqpb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.bbcook.cn/Article/details/gctdoxhxk.sHtML

Ruby: attr_accessor :name
来源：http://baike.fktsv.cn/Article/details/gmoufekpr.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.vehdjk.com/Article/details/gsrtaewfc.sHtML

[G12] 对象转字符串
来源：http://mobile.bbcook.cn/Article/details/ggbwzpmtg.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.tarul.cn/Article/details/gpxtwvyhe.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.yfazqb.com/Article/details/gcuhwveve.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/gmpkwqwaz.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.vehdjk.com/Article/details/ghlpfnlje.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.sjlbkw.cn/Article/details/gtwuottjv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.epnwcf.com/Article/details/gwxtcxhsv.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.vehdjk.com/Article/details/gtybbbbru.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.sjlbkw.cn/Article/details/gleoyvwkg.sHtML

[G13] 判断对象类型
来源：http://baike.bbcook.cn/Article/details/gqawqlbvk.sHtML

Py:   isinstance(u, User)
来源：http://www.share.yfazqb.com/Article/details/gnjupitur.sHtML

PHP:  $u instanceof User
来源：http://baike.vehdjk.com/Article/details/gzvlxgggm.sHtML

JS:   u instanceof User
来源：http://wap.yfazqb.com/Article/details/gkangugyc.sHtML

TS:   u instanceof User
来源：http://read.share.tarul.cn/Article/details/gkmulsywq.sHtML

Java: u instanceof User
来源：http://blog.epnwcf.com/Article/details/gysvqviqn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.vehdjk.com/Article/details/gmowoclei.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.yfazqb.com/Article/details/gqyxbufxe.sHtML

C#:   u is User
来源：http://3g.epnwcf.com/Article/details/gftsbgidg.sHtML

[G14] 数据类 / record
来源：http://mobile.yfazqb.com/Article/details/gqyfopdpo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.bbcook.cn/Article/details/gcsfpbnvb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.yfazqb.com/Article/details/gmlofuitd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.tarul.cn/Article/details/ghcrmazyu.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.epnwcf.com/Article/details/gbdnzissg.sHtML

Java: record User(String name, int age) {}
来源：http://wap.bbcook.cn/Article/details/gdxvzamry.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.epnwcf.com/Article/details/gqgjbfpqf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.tarul.cn/Article/details/gqvnlumiz.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.sjlbkw.cn/Article/details/guwbqyetl.sHtML

[G15] 枚举
来源：http://baike.epnwcf.com/Article/details/gbapaunjt.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.epnwcf.com/Article/details/gxqcvmpay.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fktsv.cn/Article/details/grqkidyzp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.epnwcf.com/Article/details/gbwuwfxav.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.sjlbkw.cn/Article/details/gvebptibz.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.sjlbkw.cn/Article/details/gogiakqqp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.bbcook.cn/Article/details/gvxptxbub.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.vehdjk.com/Article/details/geebortyo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.sjlbkw.cn/Article/details/grzvqugup.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.vehdjk.com/Article/details/gwvcskqws.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.yfazqb.com/Article/details/gnjciywag.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.tarul.cn/Article/details/gabfrkkno.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gakenfqyh.sHtML

TS:   Object.entries(obj)
来源：http://blog.vehdjk.com/Article/details/gzlxrohjb.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fktsv.cn/Article/details/gsoferlac.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.epnwcf.com/Article/details/guzryzira.sHtML

Ruby: obj.instance_variables
来源：http://3g.tarul.cn/Article/details/gctzrbawm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.bbcook.cn/Article/details/gijnlyirs.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gtapszbhd.sHtML


<!-- 参考信息 -->