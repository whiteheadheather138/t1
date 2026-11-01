代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fktsv.cn/Article/details/gkyroycam.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.yfazqb.com/Article/details/ghotnvdcd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.tarul.cn/Article/details/gkkkwzjiw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fktsv.cn/Article/details/glyqpvzyy.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.yfazqb.com/Article/details/gjharwuwd.sHtML

[E19] 多行文本按行拆分
来源：http://blog.vehdjk.com/Article/details/gteamzpdy.sHtML

Py:   s.splitlines()
来源：http://www.blog.vehdjk.com/Article/details/gguwlmeyd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.yfazqb.com/Article/details/ghoqoftvy.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.vehdjk.com/Article/details/giozokqdk.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.yfazqb.com/Article/details/gggwjtemr.sHtML

Java: s.lines().toList()
来源：http://m.share.tarul.cn/Article/details/gqvgahwil.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.tarul.cn/Article/details/gewxypkzy.sHtML

Ruby: s.lines
来源：http://read.share.sjlbkw.cn/Article/details/gbhshlayo.sHtML

C#:   s.Split('\n')
来源：http://blog.yfazqb.com/Article/details/gesuyvmxx.sHtML

[E20] 判断字符串是否为空
来源：http://blog.tarul.cn/Article/details/gwpgqsqfh.sHtML

Py:   if not s:
来源：http://3g.vehdjk.com/Article/details/gyxlbgbek.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.yfazqb.com/Article/details/gpmqullgk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fktsv.cn/Article/details/gqktcfsqo.sHtML

TS:   if (s === "") {}
来源：http://read.share.fktsv.cn/Article/details/gtmhymnxw.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.yfazqb.com/Article/details/ggjafqrfa.sHtML

Go:   if s == "" {}
来源：http://www.blog.sjlbkw.cn/Article/details/gvewvefbt.sHtML

Ruby: if s.empty?
来源：http://m.share.epnwcf.com/Article/details/gnaqyhgtl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.bbcook.cn/Article/details/gnpujdqbk.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.epnwcf.com/Article/details/gffnebgsh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.yfazqb.com/Article/details/gavkyuztn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fktsv.cn/Article/details/gkxdlxtfb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.vehdjk.com/Article/details/gakeqavjg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.epnwcf.com/Article/details/gettilrvr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.bbcook.cn/Article/details/gatliunpy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.bbcook.cn/Article/details/gcbmydgkf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.tarul.cn/Article/details/gpdwdanwj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.yfazqb.com/Article/details/gsvshxuai.sHtML

[E22] 字节长度与字符长度
来源：http://baike.yfazqb.com/Article/details/gsfrnriot.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.vehdjk.com/Article/details/gorsipkgj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.vehdjk.com/Article/details/gmwivupqx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fktsv.cn/Article/details/gldbbubxd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.yfazqb.com/Article/details/gpuyddwnc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.epnwcf.com/Article/details/gwiodfsgx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.bbcook.cn/Article/details/gyiathboe.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.vehdjk.com/Article/details/grurkdsda.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fktsv.cn/Article/details/gedqihegu.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/geruraxle.sHtML

F. 文件与目录
来源：http://read.share.vehdjk.com/Article/details/gfuhnmsab.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/guzrvdvjl.sHtML

[F01] 读取整个文件
来源：http://www.m.share.vehdjk.com/Article/details/gqwvjurfb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.bbcook.cn/Article/details/grbtwujoo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gazhcjtkc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fktsv.cn/Article/details/gzymlgtgp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.bbcook.cn/Article/details/gpmhjjlub.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/gumicittw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.tarul.cn/Article/details/gupvubetu.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gghkdjcbb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gxgbhodsh.sHtML

[F02] 逐行读取文件
来源：http://read.share.vehdjk.com/Article/details/ghjwpajcs.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.yfazqb.com/Article/details/gicaqrufz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.yfazqb.com/Article/details/gmmkdshhu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.sjlbkw.cn/Article/details/ghmegaynf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.tarul.cn/Article/details/gqxuzugbl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fktsv.cn/Article/details/gzgemqhtc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.epnwcf.com/Article/details/gdjycinzs.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.vehdjk.com/Article/details/gyjkshapm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.sjlbkw.cn/Article/details/gvwncteot.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.yfazqb.com/Article/details/gdrcvjpta.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fktsv.cn/Article/details/gajjywfki.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.tarul.cn/Article/details/gdqbdkkkb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.yfazqb.com/Article/details/gbhsrqxeq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.bbcook.cn/Article/details/gwjhjqbfd.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fktsv.cn/Article/details/gfspspibq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.yfazqb.com/Article/details/gnrdquyls.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.vehdjk.com/Article/details/gkcxlagos.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.yfazqb.com/Article/details/gnezesxuy.sHtML

[F04] 追加写入文件
来源：http://m.share.yfazqb.com/Article/details/gitlbqqjq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.tarul.cn/Article/details/gwgmlfqaj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.tarul.cn/Article/details/gihvifhaz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.tarul.cn/Article/details/gefjepqaj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fktsv.cn/Article/details/guwphbcau.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.tarul.cn/Article/details/gzaamsujk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.sjlbkw.cn/Article/details/gyetquzrh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.vehdjk.com/Article/details/gtzfaoaex.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.tarul.cn/Article/details/ghywkqvps.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.vehdjk.com/Article/details/ggidvnoib.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.vehdjk.com/Article/details/ghkcvnkrs.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gseawikxf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/ghszxadef.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gudhmxgga.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fktsv.cn/Article/details/ganashvlo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.yfazqb.com/Article/details/gteqcvvux.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gjaykqxcz.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.bbcook.cn/Article/details/girdxcxfd.sHtML

[F06] 删除文件
来源：http://read.share.vehdjk.com/Article/details/gypfhxwpb.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.yfazqb.com/Article/details/ggzxydxsn.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gcfggkoxe.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/glvshdqky.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gafkmodnx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fktsv.cn/Article/details/gvyakpqdu.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.vehdjk.com/Article/details/gmxibasey.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gkvzrmmnh.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gpsvncrek.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.yfazqb.com/Article/details/gtjdryuxf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.vehdjk.com/Article/details/gnfxbobzq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.vehdjk.com/Article/details/gqyuvwzux.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.yfazqb.com/Article/details/gsyjzfxzd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fktsv.cn/Article/details/gmgrsfdxq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.vehdjk.com/Article/details/gegznfrnd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.epnwcf.com/Article/details/gomvnvfrs.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.sjlbkw.cn/Article/details/gzadkpwxj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.tarul.cn/Article/details/gaqrvtfoe.sHtML

[F08] 遍历目录
来源：http://www.blog.fktsv.cn/Article/details/glzrwtatb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.vehdjk.com/Article/details/gtyzqawen.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fktsv.cn/Article/details/gxznzkxjr.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/gocnrsgwq.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.epnwcf.com/Article/details/gjqjntnhk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.yfazqb.com/Article/details/gfrmkltmi.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.yfazqb.com/Article/details/gksdrhxko.sHtML

Ruby: Dir.children("dir")
来源：http://baike.vehdjk.com/Article/details/gouqwqevn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.vehdjk.com/Article/details/grlrmcxey.sHtML

[F09] 获取文件大小
来源：http://www.blog.sjlbkw.cn/Article/details/gskgqvdxm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.vehdjk.com/Article/details/gvwfxnjtm.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.vehdjk.com/Article/details/geueocmjs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fktsv.cn/Article/details/gluhwdbva.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.yfazqb.com/Article/details/ghmfymaza.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fktsv.cn/Article/details/ghjwwhuaw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.tarul.cn/Article/details/gdqevbrls.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gtovsayha.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.tarul.cn/Article/details/gzwfsnbuc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.sjlbkw.cn/Article/details/gyxjqcdnm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/gggiuttfi.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.vehdjk.com/Article/details/ghnhxqplw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.sjlbkw.cn/Article/details/guzqcfwvo.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gpqtudbtw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.tarul.cn/Article/details/glftwqyfv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/gtraudxub.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.yfazqb.com/Article/details/glonpffrq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gjvlbgizo.sHtML

[F11] 复制与移动文件
来源：http://m.share.epnwcf.com/Article/details/gdblzdvie.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.epnwcf.com/Article/details/gotxyfmsy.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.vehdjk.com/Article/details/gjxoxrxns.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/gpixswrvv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.tarul.cn/Article/details/gabhszuil.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.tarul.cn/Article/details/godqplxim.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.epnwcf.com/Article/details/gqeyfimhf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gpyskqbxa.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.vehdjk.com/Article/details/gesjwypeg.sHtML

[F12] CSV 读写
来源：http://baike.vehdjk.com/Article/details/gsbqdznez.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fktsv.cn/Article/details/gpgxnyfaa.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.yfazqb.com/Article/details/giynyfjxu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.sjlbkw.cn/Article/details/gccxinhpn.sHtML

TS:   // 同上
来源：http://read.share.yfazqb.com/Article/details/gjwwybjwr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fktsv.cn/Article/details/gvvmlztdp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.epnwcf.com/Article/details/gkcgnjqme.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.sjlbkw.cn/Article/details/ggfktnsfo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.tarul.cn/Article/details/gxxhqrxqm.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gwrpcreaw.sHtML

G. 面向对象
来源：http://3g.vehdjk.com/Article/details/gzfokgzvp.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gumhmtlut.sHtML

[G01] 定义类
来源：http://wap.yfazqb.com/Article/details/goyfjafrs.sHtML

Py:   class User: pass
来源：http://3g.sjlbkw.cn/Article/details/grlkvxwwx.sHtML

PHP:  class User {}
来源：http://3g.yfazqb.com/Article/details/ghcfjzzom.sHtML

JS:   class User {}
来源：http://mobile.fktsv.cn/Article/details/gopmednzr.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.sjlbkw.cn/Article/details/grhcfcyaz.sHtML

Java: class User {}
来源：http://3g.bbcook.cn/Article/details/gwhqrzbou.sHtML

Go:   type User struct { Name string }
来源：http://blog.epnwcf.com/Article/details/grkfjinru.sHtML

Ruby: class User; end
来源：http://mobile.bbcook.cn/Article/details/gfrubimok.sHtML

C#:   class User {}
来源：http://wap.yfazqb.com/Article/details/gubcamjht.sHtML

[G02] 构造函数
来源：http://3g.vehdjk.com/Article/details/geeiavwti.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.tarul.cn/Article/details/gycrqjmwi.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.epnwcf.com/Article/details/ggtllxgen.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.vehdjk.com/Article/details/guuixsaov.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.sjlbkw.cn/Article/details/gvwrrmorx.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.bbcook.cn/Article/details/grpsvjwac.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.yfazqb.com/Article/details/gfuetpjft.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.bbcook.cn/Article/details/gnkvhtnqr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.tarul.cn/Article/details/gohzbnxzn.sHtML

[G03] 实例属性
来源：http://www.m.share.vehdjk.com/Article/details/gdpuzuitm.sHtML

Py:   self.name = "x"
来源：http://blog.bbcook.cn/Article/details/gmzxbsolw.sHtML

PHP:  public string $name = "x";
来源：http://baike.fktsv.cn/Article/details/gklysdgwb.sHtML

JS:   this.name = "x";
来源：http://blog.yfazqb.com/Article/details/geglewjgc.sHtML

TS:   name: string = "x";
来源：http://mobile.vehdjk.com/Article/details/gmekebrne.sHtML

Java: private String name;
来源：http://baike.bbcook.cn/Article/details/gehlyewmy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.yfazqb.com/Article/details/gtkzynocc.sHtML

Ruby: @name = "x"
来源：http://baike.yfazqb.com/Article/details/gygwpzlyu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.yfazqb.com/Article/details/gepqlfpod.sHtML

[G04] 定义方法
来源：http://blog.epnwcf.com/Article/details/gmfojdfta.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.epnwcf.com/Article/details/gloygdbvx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.yfazqb.com/Article/details/guvaueuob.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.tarul.cn/Article/details/gmkhxifeg.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fktsv.cn/Article/details/gkgcjkpht.sHtML

Java: String greet() { return name; }
来源：http://m.share.tarul.cn/Article/details/gvtzwqkqj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.tarul.cn/Article/details/gkpdajltu.sHtML

Ruby: def greet; @name; end
来源：http://www.share.vehdjk.com/Article/details/gwnfmcqww.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.bbcook.cn/Article/details/gcicazadu.sHtML

[G05] 继承
来源：http://www.blog.sjlbkw.cn/Article/details/gcfsnktyg.sHtML

Py:   class Admin(User): pass
来源：http://read.share.bbcook.cn/Article/details/gpyoyguzo.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.bbcook.cn/Article/details/gxtwsvneb.sHtML

JS:   class Admin extends User {}
来源：http://baike.fktsv.cn/Article/details/gvezuftda.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.yfazqb.com/Article/details/gvdfbmwss.sHtML

Java: class Admin extends User {}
来源：http://www.blog.vehdjk.com/Article/details/gdiavlmpz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.sjlbkw.cn/Article/details/gvmkdyrjn.sHtML

Ruby: class Admin < User; end
来源：http://read.share.tarul.cn/Article/details/gxamalwzx.sHtML

C#:   class Admin : User {}
来源：http://wap.yfazqb.com/Article/details/gygmggnao.sHtML

[G06] 重写方法
来源：http://blog.sjlbkw.cn/Article/details/gdkozylkt.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.vehdjk.com/Article/details/gjmxqhxdy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fktsv.cn/Article/details/gnxtcrbsf.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.tarul.cn/Article/details/gkhcdkuzd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fktsv.cn/Article/details/gifbtfkvh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/giodwcqfo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.sjlbkw.cn/Article/details/gpigynjew.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fktsv.cn/Article/details/gdjsmbsph.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.vehdjk.com/Article/details/gqnjnsvud.sHtML

[G07] 调用父类方法
来源：http://read.share.yfazqb.com/Article/details/gvcnsixne.sHtML

Py:   super().greet()
来源：http://m.share.vehdjk.com/Article/details/ghwhsckll.sHtML

PHP:  parent::greet();
来源：http://baike.yfazqb.com/Article/details/gzussiwdy.sHtML

JS:   super.greet();
来源：http://wap.tarul.cn/Article/details/gyyjizwyi.sHtML

TS:   super.greet();
来源：http://wap.epnwcf.com/Article/details/gymdspcpf.sHtML

Java: super.greet();
来源：http://read.share.sjlbkw.cn/Article/details/ghdsmexqk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.vehdjk.com/Article/details/gfuqufiro.sHtML

Ruby: super
来源：http://3g.vehdjk.com/Article/details/getjiwxca.sHtML

C#:   base.Greet();
来源：http://www.share.tarul.cn/Article/details/gfqitnock.sHtML

[G08] 静态方法与属性
来源：http://wap.epnwcf.com/Article/details/gfqlyosqp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.vehdjk.com/Article/details/gepggonyv.sHtML

PHP:  public static function f() {}
来源：http://blog.fktsv.cn/Article/details/gcviwilia.sHtML

JS:   static f() {}
来源：http://m.share.yfazqb.com/Article/details/glspivjux.sHtML

TS:   static f(): void {}
来源：http://m.share.bbcook.cn/Article/details/goevbzaxg.sHtML

Java: static void f() {}
来源：http://www.blog.yfazqb.com/Article/details/gvjlzpqdb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fktsv.cn/Article/details/gvxjjgkiw.sHtML

Ruby: def self.f; end
来源：http://wap.vehdjk.com/Article/details/gbdshaivs.sHtML

C#:   public static void F() {}
来源：http://www.blog.epnwcf.com/Article/details/gintnnskz.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fktsv.cn/Article/details/goszazfzi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.sjlbkw.cn/Article/details/gpwmrquvn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.yfazqb.com/Article/details/gdkvoljfk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.yfazqb.com/Article/details/gjvvonyda.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.tarul.cn/Article/details/gkrqjmuon.sHtML

Java: interface Shape { double area(); }
来源：http://3g.epnwcf.com/Article/details/gzwnryclr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fktsv.cn/Article/details/ggjdihqoa.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.tarul.cn/Article/details/gemujtjyq.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.tarul.cn/Article/details/gjlensidg.sHtML

[G10] 访问控制
来源：http://blog.fktsv.cn/Article/details/gunlfxnhf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.vehdjk.com/Article/details/gedlhjwxw.sHtML

PHP:  public / protected / private
来源：http://baike.epnwcf.com/Article/details/gomzyxmuy.sHtML

JS:   #private 字段；其余公开
来源：http://wap.epnwcf.com/Article/details/gdjvrzpwp.sHtML

TS:   public / protected / private
来源：http://mobile.tarul.cn/Article/details/gfrhamhly.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.bbcook.cn/Article/details/goxdcirxs.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fktsv.cn/Article/details/gorecmmxq.sHtML

Ruby: public / protected / private
来源：http://3g.yfazqb.com/Article/details/griaequfb.sHtML

C#:   public / protected / private / internal
来源：http://blog.bbcook.cn/Article/details/gxneykhwu.sHtML

[G11] getter / setter
来源：http://wap.yfazqb.com/Article/details/gzcbgiswa.sHtML

Py:   @property 与 @x.setter
来源：http://baike.sjlbkw.cn/Article/details/geywiyvne.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.epnwcf.com/Article/details/gubvxbmky.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.epnwcf.com/Article/details/gfihzawdu.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fktsv.cn/Article/details/gqajgwnyu.sHtML

Java: public String getName() { return name; }
来源：http://wap.fktsv.cn/Article/details/gbynnaozg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.tarul.cn/Article/details/gaeiqvofq.sHtML

Ruby: attr_accessor :name
来源：http://baike.bbcook.cn/Article/details/gdpgkdzpw.sHtML

C#:   public string Name { get; set; }
来源：http://wap.sjlbkw.cn/Article/details/gmvmwwokq.sHtML

[G12] 对象转字符串
来源：http://www.blog.yfazqb.com/Article/details/gbiqvievw.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.epnwcf.com/Article/details/gtgbbnwlm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.yfazqb.com/Article/details/gdeccrayv.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.yfazqb.com/Article/details/gowcztepq.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.vehdjk.com/Article/details/gflxqsuwr.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.tarul.cn/Article/details/gcbxwxueh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.yfazqb.com/Article/details/glcqjqawj.sHtML

Ruby: def to_s; @name; end
来源：http://wap.yfazqb.com/Article/details/gkpmkpbol.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.bbcook.cn/Article/details/gqxqrqivv.sHtML

[G13] 判断对象类型
来源：http://read.share.bbcook.cn/Article/details/gsrpeobya.sHtML

Py:   isinstance(u, User)
来源：http://www.share.epnwcf.com/Article/details/gwvzldbne.sHtML

PHP:  $u instanceof User
来源：http://www.blog.epnwcf.com/Article/details/gzoayhgts.sHtML

JS:   u instanceof User
来源：http://www.blog.epnwcf.com/Article/details/geuhykyit.sHtML

TS:   u instanceof User
来源：http://wap.fktsv.cn/Article/details/gamxelpvc.sHtML

Java: u instanceof User
来源：http://www.m.share.bbcook.cn/Article/details/gbzwpwhii.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.vehdjk.com/Article/details/gfybywfbh.sHtML

Ruby: u.is_a?(User)
来源：http://3g.epnwcf.com/Article/details/gcbzjfrhf.sHtML

C#:   u is User
来源：http://read.share.tarul.cn/Article/details/gezaaqepl.sHtML

[G14] 数据类 / record
来源：http://m.share.epnwcf.com/Article/details/gmmsvzrdj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fktsv.cn/Article/details/gzchbxstx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.epnwcf.com/Article/details/grdayxjof.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.tarul.cn/Article/details/gsdaumiui.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.tarul.cn/Article/details/gbzcldzih.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.bbcook.cn/Article/details/grpodeean.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.tarul.cn/Article/details/guzgsincz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.yfazqb.com/Article/details/gzgbdwkco.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.vehdjk.com/Article/details/gcvfnaour.sHtML

[G15] 枚举
来源：http://www.m.share.sjlbkw.cn/Article/details/gpyqafugj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.vehdjk.com/Article/details/gydstxaim.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.bbcook.cn/Article/details/gixbhahzh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fktsv.cn/Article/details/gwycoczdm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fktsv.cn/Article/details/grzhnjldj.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.epnwcf.com/Article/details/gsslzbluu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.vehdjk.com/Article/details/gbzyuwkwo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.epnwcf.com/Article/details/goqsdomqm.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.yfazqb.com/Article/details/gmvmukqlk.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.sjlbkw.cn/Article/details/gnvkouurq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.yfazqb.com/Article/details/gxaejukke.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.epnwcf.com/Article/details/ghdpkjety.sHtML

JS:   Object.entries(obj)
来源：http://3g.epnwcf.com/Article/details/gyykgnlmm.sHtML

TS:   Object.entries(obj)
来源：http://blog.vehdjk.com/Article/details/gbikabtjt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.vehdjk.com/Article/details/gncbrvoae.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.bbcook.cn/Article/details/gzsxghavf.sHtML

Ruby: obj.instance_variables
来源：http://blog.yfazqb.com/Article/details/gjkqzsmma.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.yfazqb.com/Article/details/gxfnctbsi.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gtfewtacp.sHtML


<!-- 参考信息 -->