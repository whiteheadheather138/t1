代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.tarul.cn/Article/details/ghobgmfvm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.yfazqb.com/Article/details/gtowzsnuc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.epnwcf.com/Article/details/gygyuxqhd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.vehdjk.com/Article/details/gesyrtcbo.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.sjlbkw.cn/Article/details/gcpyaslun.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.epnwcf.com/Article/details/gbloksego.sHtML

Py:   s.splitlines()
来源：http://www.blog.fktsv.cn/Article/details/glzsuilwr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.yfazqb.com/Article/details/gttemvsfu.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.yfazqb.com/Article/details/gyfdcjtor.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.bbcook.cn/Article/details/gqkjwmlld.sHtML

Java: s.lines().toList()
来源：http://blog.sjlbkw.cn/Article/details/gakdrefmp.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.epnwcf.com/Article/details/gikfesfpa.sHtML

Ruby: s.lines
来源：http://www.share.yfazqb.com/Article/details/grtsjyomd.sHtML

C#:   s.Split('\n')
来源：http://wap.tarul.cn/Article/details/gxdbidqei.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.bbcook.cn/Article/details/gptcsdakc.sHtML

Py:   if not s:
来源：http://mobile.yfazqb.com/Article/details/gozixovdq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.yfazqb.com/Article/details/geakmzxsy.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.bbcook.cn/Article/details/gsxcdisuw.sHtML

TS:   if (s === "") {}
来源：http://blog.vehdjk.com/Article/details/glrcppaty.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.yfazqb.com/Article/details/gsjnhpcgi.sHtML

Go:   if s == "" {}
来源：http://www.share.bbcook.cn/Article/details/gjcrjyeaw.sHtML

Ruby: if s.empty?
来源：http://www.share.tarul.cn/Article/details/gkpgsychd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.tarul.cn/Article/details/goomuxzza.sHtML

[E21] 超长截断加省略号
来源：http://m.share.vehdjk.com/Article/details/gusiyikkk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.tarul.cn/Article/details/gbcjampnp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/gsljhsmap.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.bbcook.cn/Article/details/gxnwnqotm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.bbcook.cn/Article/details/gomtgqouu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.tarul.cn/Article/details/gsonxtbgs.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.yfazqb.com/Article/details/gbttnnubt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/gaobrrnov.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.epnwcf.com/Article/details/gwpfzovgs.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.tarul.cn/Article/details/gxkbkyjcr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.sjlbkw.cn/Article/details/grpoivtlb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fktsv.cn/Article/details/ggteqzspp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.epnwcf.com/Article/details/gekxpdzpk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.vehdjk.com/Article/details/ghxauheld.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.bbcook.cn/Article/details/gmpvxzzgv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.tarul.cn/Article/details/gjylepbgx.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.bbcook.cn/Article/details/gmnhbbncw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.vehdjk.com/Article/details/gwkhodzqr.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gulusysiz.sHtML

F. 文件与目录
来源：http://blog.vehdjk.com/Article/details/gpvljjglf.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gwffsfldh.sHtML

[F01] 读取整个文件
来源：http://read.share.bbcook.cn/Article/details/gmsdnaohc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.tarul.cn/Article/details/gplvmraln.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gnadzjfjc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.tarul.cn/Article/details/ggwsazfzv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.bbcook.cn/Article/details/geekhwajj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.fktsv.cn/Article/details/gfgdikkpo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.yfazqb.com/Article/details/gjdcnyfhy.sHtML

Ruby: File.read("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gdtnvffef.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.vehdjk.com/Article/details/gttrbbxfr.sHtML

[F02] 逐行读取文件
来源：http://m.share.epnwcf.com/Article/details/gjammrbpb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.bbcook.cn/Article/details/guztpygep.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.yfazqb.com/Article/details/gfevajrbt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.vehdjk.com/Article/details/ggodkkmjh.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fktsv.cn/Article/details/gpgyqwtws.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.epnwcf.com/Article/details/gwdiswhbf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.yfazqb.com/Article/details/ggbhxzyjt.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.bbcook.cn/Article/details/guyluhyoi.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.tarul.cn/Article/details/gpueqbscu.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.tarul.cn/Article/details/gkrxkrexx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fktsv.cn/Article/details/gizqhxbfn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.vehdjk.com/Article/details/gdeqglall.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.tarul.cn/Article/details/glvsyclik.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.sjlbkw.cn/Article/details/gffflwhxx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.yfazqb.com/Article/details/gwbdrsqus.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.sjlbkw.cn/Article/details/gkqejrxfz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.yfazqb.com/Article/details/gvvfziqxd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fktsv.cn/Article/details/gzbakwmqe.sHtML

[F04] 追加写入文件
来源：http://m.share.tarul.cn/Article/details/gngjoimem.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.epnwcf.com/Article/details/giisbbqvf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.epnwcf.com/Article/details/gnccburrz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fktsv.cn/Article/details/ggodvwhhr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.vehdjk.com/Article/details/gcttjriyw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.vehdjk.com/Article/details/gxzaisihk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.sjlbkw.cn/Article/details/gokuigdzs.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.bbcook.cn/Article/details/ghdzvksdk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.bbcook.cn/Article/details/gzbxmgecz.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.sjlbkw.cn/Article/details/gkcmcshbf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.sjlbkw.cn/Article/details/gnoszecas.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gfwpxxiic.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.tarul.cn/Article/details/gnufbjrld.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gqjyqicwo.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.yfazqb.com/Article/details/grjgpunyi.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fktsv.cn/Article/details/gshdvouog.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.tarul.cn/Article/details/gdwtuvqog.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gmezdwioa.sHtML

[F06] 删除文件
来源：http://www.share.epnwcf.com/Article/details/gbizotbst.sHtML

Py:   os.remove("a.txt")
来源：http://blog.vehdjk.com/Article/details/glkjhlvie.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gmbdpdrqs.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gsmedjafe.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.vehdjk.com/Article/details/gqrhhmsqx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fktsv.cn/Article/details/ghnulsoop.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fktsv.cn/Article/details/gbyupoacr.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gesrajmsl.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gqkfrkyzg.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.sjlbkw.cn/Article/details/gglndovtq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.bbcook.cn/Article/details/gjumjsbco.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.yfazqb.com/Article/details/gabokuaux.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.epnwcf.com/Article/details/gxfdfxbyv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.epnwcf.com/Article/details/goaricnrb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.bbcook.cn/Article/details/gpnunxbug.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.tarul.cn/Article/details/gscglqmow.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.vehdjk.com/Article/details/gcykrxxyf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.sjlbkw.cn/Article/details/gghfqpvhv.sHtML

[F08] 遍历目录
来源：http://www.m.share.sjlbkw.cn/Article/details/gxyjbhdyk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.sjlbkw.cn/Article/details/gwdubiivy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.tarul.cn/Article/details/ghzhpnmvi.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fktsv.cn/Article/details/grebsrztg.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.vehdjk.com/Article/details/ghcmtrxiz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.tarul.cn/Article/details/gaohlbhfv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.tarul.cn/Article/details/guutcuizn.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.bbcook.cn/Article/details/gjoxixoou.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.yfazqb.com/Article/details/gnlrgrqut.sHtML

[F09] 获取文件大小
来源：http://3g.yfazqb.com/Article/details/gvizrycoz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.epnwcf.com/Article/details/gladdpneo.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fktsv.cn/Article/details/gahcnoipd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.tarul.cn/Article/details/ggfueylxw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.epnwcf.com/Article/details/gebgcjkln.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fktsv.cn/Article/details/goeysnyex.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.vehdjk.com/Article/details/gxknrmxtc.sHtML

Ruby: File.size("a.txt")
来源：http://wap.tarul.cn/Article/details/gotfslkfi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.bbcook.cn/Article/details/gzcnhlznx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fktsv.cn/Article/details/ggvbkgnph.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gwpapkgfx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.tarul.cn/Article/details/gdxkoacax.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.bbcook.cn/Article/details/ghoffxyko.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.tarul.cn/Article/details/ggatorukp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.bbcook.cn/Article/details/gtbhwwwts.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.tarul.cn/Article/details/goqsodvlt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/gabydiwcg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/gleoxaxrc.sHtML

[F11] 复制与移动文件
来源：http://www.share.vehdjk.com/Article/details/gforhetzr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/goktxivsr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gbvbavtzw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gqsquxflm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/gbrpybnqk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.bbcook.cn/Article/details/ghsmnbhvr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.bbcook.cn/Article/details/gueulmgow.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fktsv.cn/Article/details/gflpbyubb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.vehdjk.com/Article/details/gftxyujoz.sHtML

[F12] CSV 读写
来源：http://mobile.sjlbkw.cn/Article/details/gpejedros.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.epnwcf.com/Article/details/guyfdfhdc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.yfazqb.com/Article/details/gkomzcvyy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.tarul.cn/Article/details/gndminxfk.sHtML

TS:   // 同上
来源：http://www.blog.tarul.cn/Article/details/ghtjrwspk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.tarul.cn/Article/details/gsmvbbetu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fktsv.cn/Article/details/gnqjsfyfc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fktsv.cn/Article/details/guhjsrwxl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.yfazqb.com/Article/details/gddelapdw.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/giuuohlqf.sHtML

G. 面向对象
来源：http://mobile.tarul.cn/Article/details/gwchhlirx.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gjdlfkvux.sHtML

[G01] 定义类
来源：http://www.blog.vehdjk.com/Article/details/gfkaxlzlx.sHtML

Py:   class User: pass
来源：http://mobile.epnwcf.com/Article/details/gljvbaqox.sHtML

PHP:  class User {}
来源：http://www.share.yfazqb.com/Article/details/ghjyhqxwk.sHtML

JS:   class User {}
来源：http://baike.sjlbkw.cn/Article/details/ggnthtvdh.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fktsv.cn/Article/details/gmsosfnsf.sHtML

Java: class User {}
来源：http://baike.vehdjk.com/Article/details/gozfewjbt.sHtML

Go:   type User struct { Name string }
来源：http://wap.fktsv.cn/Article/details/gcuidrkyq.sHtML

Ruby: class User; end
来源：http://blog.yfazqb.com/Article/details/gqzpmgwbg.sHtML

C#:   class User {}
来源：http://www.blog.epnwcf.com/Article/details/giiulxynt.sHtML

[G02] 构造函数
来源：http://mobile.tarul.cn/Article/details/gdtzxkdvr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.sjlbkw.cn/Article/details/gprvmmrvj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fktsv.cn/Article/details/gdnmhbkem.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fktsv.cn/Article/details/gfxjaevjf.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.bbcook.cn/Article/details/gqujnxzgv.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.yfazqb.com/Article/details/guczfscet.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.yfazqb.com/Article/details/guetrlurz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.epnwcf.com/Article/details/graskmokb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.bbcook.cn/Article/details/gevlrmonu.sHtML

[G03] 实例属性
来源：http://read.share.sjlbkw.cn/Article/details/gcajegmsm.sHtML

Py:   self.name = "x"
来源：http://wap.epnwcf.com/Article/details/gdfawfvsj.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.tarul.cn/Article/details/gisqolyjq.sHtML

JS:   this.name = "x";
来源：http://www.share.epnwcf.com/Article/details/guhbuujdy.sHtML

TS:   name: string = "x";
来源：http://blog.sjlbkw.cn/Article/details/gglnrgyel.sHtML

Java: private String name;
来源：http://wap.yfazqb.com/Article/details/gsvjanytf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.bbcook.cn/Article/details/gjxexozvt.sHtML

Ruby: @name = "x"
来源：http://www.m.share.tarul.cn/Article/details/gzrcykpqc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.tarul.cn/Article/details/gyhkjewwu.sHtML

[G04] 定义方法
来源：http://3g.vehdjk.com/Article/details/gwshotvyv.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fktsv.cn/Article/details/gmhrealqm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.tarul.cn/Article/details/gcftsbixy.sHtML

JS:   greet() { return this.name; }
来源：http://wap.bbcook.cn/Article/details/gcenxaugq.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.epnwcf.com/Article/details/ggsidoxss.sHtML

Java: String greet() { return name; }
来源：http://www.blog.tarul.cn/Article/details/gmcjqrpba.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.epnwcf.com/Article/details/ggwiucllc.sHtML

Ruby: def greet; @name; end
来源：http://www.share.bbcook.cn/Article/details/gsoleelmc.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.vehdjk.com/Article/details/gghyflrua.sHtML

[G05] 继承
来源：http://www.m.share.fktsv.cn/Article/details/gcqhffgef.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.bbcook.cn/Article/details/gaggcbeaf.sHtML

PHP:  class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/gguuxkmrq.sHtML

JS:   class Admin extends User {}
来源：http://wap.bbcook.cn/Article/details/genpnaoux.sHtML

TS:   class Admin extends User {}
来源：http://read.share.bbcook.cn/Article/details/gahsygitv.sHtML

Java: class Admin extends User {}
来源：http://baike.vehdjk.com/Article/details/geteiyjwn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.tarul.cn/Article/details/gnvniqswk.sHtML

Ruby: class Admin < User; end
来源：http://blog.epnwcf.com/Article/details/gmfswvnhi.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.vehdjk.com/Article/details/gdnhvmsoe.sHtML

[G06] 重写方法
来源：http://www.share.epnwcf.com/Article/details/glmhhvfmt.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.tarul.cn/Article/details/gwvmwdbjg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fktsv.cn/Article/details/ggrdmromy.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.bbcook.cn/Article/details/gyexjfryu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.epnwcf.com/Article/details/gstcdocto.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.epnwcf.com/Article/details/gyctsqvzz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.tarul.cn/Article/details/gizmdcmtd.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.yfazqb.com/Article/details/gjnmtchyz.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.yfazqb.com/Article/details/gqfydemsz.sHtML

[G07] 调用父类方法
来源：http://www.m.share.bbcook.cn/Article/details/gnbbbrkxx.sHtML

Py:   super().greet()
来源：http://m.share.sjlbkw.cn/Article/details/gutrvazum.sHtML

PHP:  parent::greet();
来源：http://read.share.epnwcf.com/Article/details/gzmiypsii.sHtML

JS:   super.greet();
来源：http://mobile.bbcook.cn/Article/details/gyatbpszv.sHtML

TS:   super.greet();
来源：http://wap.yfazqb.com/Article/details/gwamkxydv.sHtML

Java: super.greet();
来源：http://mobile.epnwcf.com/Article/details/gjryvxjqu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.tarul.cn/Article/details/gcslgyfkm.sHtML

Ruby: super
来源：http://mobile.fktsv.cn/Article/details/gjinjhrea.sHtML

C#:   base.Greet();
来源：http://www.blog.fktsv.cn/Article/details/gtmicqbur.sHtML

[G08] 静态方法与属性
来源：http://3g.epnwcf.com/Article/details/glexqkbfg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.bbcook.cn/Article/details/grnzfopfm.sHtML

PHP:  public static function f() {}
来源：http://mobile.bbcook.cn/Article/details/gwfomvclb.sHtML

JS:   static f() {}
来源：http://blog.yfazqb.com/Article/details/gzmykvzhf.sHtML

TS:   static f(): void {}
来源：http://mobile.bbcook.cn/Article/details/gatomdrna.sHtML

Java: static void f() {}
来源：http://blog.vehdjk.com/Article/details/gmwpegntr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.vehdjk.com/Article/details/gjagifeyo.sHtML

Ruby: def self.f; end
来源：http://www.blog.tarul.cn/Article/details/gdkecugcz.sHtML

C#:   public static void F() {}
来源：http://wap.yfazqb.com/Article/details/gtlodjjkz.sHtML

[G09] 接口 / 抽象类
来源：http://wap.epnwcf.com/Article/details/gqcsiahgy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.bbcook.cn/Article/details/gdxbkcvgh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.tarul.cn/Article/details/ghoaboxid.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.yfazqb.com/Article/details/gnwlwezno.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.vehdjk.com/Article/details/giuqcdjhn.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.epnwcf.com/Article/details/gbpyltxpj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.yfazqb.com/Article/details/gynugzyqx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.tarul.cn/Article/details/gntmntqou.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.epnwcf.com/Article/details/gtibhzemj.sHtML

[G10] 访问控制
来源：http://m.share.tarul.cn/Article/details/gvlokrhjc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.vehdjk.com/Article/details/gpavsvvyw.sHtML

PHP:  public / protected / private
来源：http://www.blog.sjlbkw.cn/Article/details/gsncnhqlu.sHtML

JS:   #private 字段；其余公开
来源：http://blog.bbcook.cn/Article/details/gswyxalzq.sHtML

TS:   public / protected / private
来源：http://www.share.tarul.cn/Article/details/grocsaqma.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.bbcook.cn/Article/details/gmambnjws.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.bbcook.cn/Article/details/goylzchsp.sHtML

Ruby: public / protected / private
来源：http://www.m.share.vehdjk.com/Article/details/gyurzjcqi.sHtML

C#:   public / protected / private / internal
来源：http://www.share.tarul.cn/Article/details/grllxrpvt.sHtML

[G11] getter / setter
来源：http://mobile.vehdjk.com/Article/details/gtxrioayx.sHtML

Py:   @property 与 @x.setter
来源：http://wap.yfazqb.com/Article/details/gvcxunncy.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.epnwcf.com/Article/details/ghouauomt.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.sjlbkw.cn/Article/details/gaztonojs.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.vehdjk.com/Article/details/giocimcku.sHtML

Java: public String getName() { return name; }
来源：http://read.share.bbcook.cn/Article/details/gsqvzyynx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fktsv.cn/Article/details/gydbfgryi.sHtML

Ruby: attr_accessor :name
来源：http://wap.tarul.cn/Article/details/gltdlbjyn.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fktsv.cn/Article/details/gnqkilref.sHtML

[G12] 对象转字符串
来源：http://wap.vehdjk.com/Article/details/gtnfpomvi.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.yfazqb.com/Article/details/ggnkkdzpk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.vehdjk.com/Article/details/grtiuxvlp.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.yfazqb.com/Article/details/gxuaxvokr.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fktsv.cn/Article/details/giofswmbn.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/gtepgwyra.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.tarul.cn/Article/details/grvsgopaz.sHtML

Ruby: def to_s; @name; end
来源：http://blog.bbcook.cn/Article/details/gzfuokpxa.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.vehdjk.com/Article/details/glritvqeh.sHtML

[G13] 判断对象类型
来源：http://wap.bbcook.cn/Article/details/gtspiyvfx.sHtML

Py:   isinstance(u, User)
来源：http://read.share.tarul.cn/Article/details/gjdktnhdc.sHtML

PHP:  $u instanceof User
来源：http://baike.epnwcf.com/Article/details/gnbdyfycl.sHtML

JS:   u instanceof User
来源：http://www.blog.fktsv.cn/Article/details/gcaisyxju.sHtML

TS:   u instanceof User
来源：http://www.m.share.fktsv.cn/Article/details/gboyguuse.sHtML

Java: u instanceof User
来源：http://www.blog.tarul.cn/Article/details/gcjmlmtfs.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.sjlbkw.cn/Article/details/gdgfhmoua.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fktsv.cn/Article/details/ghoaywhcx.sHtML

C#:   u is User
来源：http://www.m.share.bbcook.cn/Article/details/gsudwauot.sHtML

[G14] 数据类 / record
来源：http://m.share.fktsv.cn/Article/details/gebonwqij.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.epnwcf.com/Article/details/gamnmcykq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.vehdjk.com/Article/details/gubiegolr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.vehdjk.com/Article/details/gkriylces.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.bbcook.cn/Article/details/glidtmjwa.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.vehdjk.com/Article/details/gkgeefopx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.sjlbkw.cn/Article/details/gpketfzst.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fktsv.cn/Article/details/gvybkhhbr.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.vehdjk.com/Article/details/gaboysjph.sHtML

[G15] 枚举
来源：http://www.m.share.tarul.cn/Article/details/gyngqlnuw.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.tarul.cn/Article/details/gvhvcwcsm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.sjlbkw.cn/Article/details/gtvwtcrbp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.epnwcf.com/Article/details/gdjmrxdpb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.epnwcf.com/Article/details/gtukfmyao.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.yfazqb.com/Article/details/gdaamobeg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.fktsv.cn/Article/details/gyjewlgjz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fktsv.cn/Article/details/gkqgenpzm.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.sjlbkw.cn/Article/details/gbvhpdops.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.vehdjk.com/Article/details/grsysfoqy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fktsv.cn/Article/details/gnfxzqgan.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.bbcook.cn/Article/details/ggiwhjcog.sHtML

JS:   Object.entries(obj)
来源：http://baike.tarul.cn/Article/details/gzcongfcg.sHtML

TS:   Object.entries(obj)
来源：http://3g.epnwcf.com/Article/details/gjktokwqt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.sjlbkw.cn/Article/details/gskvprupq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.vehdjk.com/Article/details/grsbuzwgn.sHtML

Ruby: obj.instance_variables
来源：http://3g.bbcook.cn/Article/details/gzrovcukt.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.vehdjk.com/Article/details/gynysmlwx.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gmoznzkln.sHtML


<!-- 参考信息 -->