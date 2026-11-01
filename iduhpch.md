代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.sjlbkw.cn/Article/details/gciogejdn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.vehdjk.com/Article/details/gfnyrkuwz.sHtML

Ruby: s.capitalize
来源：http://www.share.epnwcf.com/Article/details/gmbkxutoi.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.yfazqb.com/Article/details/gjzwphqtv.sHtML

[E18] 模板占位符替换
来源：http://m.share.fktsv.cn/Article/details/gumefgkwo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.bbcook.cn/Article/details/gojojcvqc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.bbcook.cn/Article/details/gyuacsoyp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fktsv.cn/Article/details/gpidhpqro.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.yfazqb.com/Article/details/gdpatrwiv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.epnwcf.com/Article/details/gkhavzqjp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.yfazqb.com/Article/details/gfzdsgsdn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.bbcook.cn/Article/details/ggeslvhto.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.yfazqb.com/Article/details/gwrdtuobb.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.yfazqb.com/Article/details/gmmzsklys.sHtML

Py:   s.splitlines()
来源：http://3g.sjlbkw.cn/Article/details/ghwutlxet.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fktsv.cn/Article/details/gdazitesg.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.epnwcf.com/Article/details/gmrmebqfv.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.sjlbkw.cn/Article/details/gccbgkbrr.sHtML

Java: s.lines().toList()
来源：http://m.share.epnwcf.com/Article/details/golyrwqyk.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fktsv.cn/Article/details/ggkqkyfml.sHtML

Ruby: s.lines
来源：http://mobile.sjlbkw.cn/Article/details/gopqmmpcy.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.sjlbkw.cn/Article/details/gmwucggmg.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.vehdjk.com/Article/details/gkkyqljxl.sHtML

Py:   if not s:
来源：http://www.m.share.sjlbkw.cn/Article/details/gntduucoc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.vehdjk.com/Article/details/gividjloz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.bbcook.cn/Article/details/ghkfzrxvq.sHtML

TS:   if (s === "") {}
来源：http://www.share.fktsv.cn/Article/details/gazdyiibk.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.sjlbkw.cn/Article/details/gyttqawwf.sHtML

Go:   if s == "" {}
来源：http://www.m.share.vehdjk.com/Article/details/gxnkwklvv.sHtML

Ruby: if s.empty?
来源：http://www.m.share.yfazqb.com/Article/details/glrphsorq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.sjlbkw.cn/Article/details/gujjcxofo.sHtML

[E21] 超长截断加省略号
来源：http://m.share.vehdjk.com/Article/details/gxxhsssxj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.tarul.cn/Article/details/giwfqycwn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.vehdjk.com/Article/details/gqgvnqpwv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fktsv.cn/Article/details/gzbbgglpr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.sjlbkw.cn/Article/details/gnbjzsfpg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.epnwcf.com/Article/details/goyewaslo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.vehdjk.com/Article/details/gjjbfcrxu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.yfazqb.com/Article/details/gnuvmbauq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gxotmpnow.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.tarul.cn/Article/details/gadeulpte.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.yfazqb.com/Article/details/geswhvnzi.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.vehdjk.com/Article/details/gytrwtvfo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.yfazqb.com/Article/details/gfrpjrywc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.bbcook.cn/Article/details/glzfnzgua.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fktsv.cn/Article/details/gxrbeqfud.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fktsv.cn/Article/details/gkbcfdxza.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.epnwcf.com/Article/details/gphtzdgkm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fktsv.cn/Article/details/gkogwtxpk.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gcckyzpjv.sHtML

F. 文件与目录
来源：http://www.blog.tarul.cn/Article/details/gqdttfjnj.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gocaruafw.sHtML

[F01] 读取整个文件
来源：http://baike.sjlbkw.cn/Article/details/gxaxvljxq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.bbcook.cn/Article/details/gfnmsbkur.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.vehdjk.com/Article/details/gruhvyruo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.epnwcf.com/Article/details/gaidifihp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.yfazqb.com/Article/details/gssjmebeg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/gteaaqoxz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.sjlbkw.cn/Article/details/gnrigolql.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gzzmgqwmg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gcuvxpsiw.sHtML

[F02] 逐行读取文件
来源：http://blog.epnwcf.com/Article/details/grqlwapcz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.tarul.cn/Article/details/gcpxgzgji.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.yfazqb.com/Article/details/gmipcypko.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.vehdjk.com/Article/details/gnsvfinny.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.tarul.cn/Article/details/gilrvnowp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.bbcook.cn/Article/details/gevjflaks.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fktsv.cn/Article/details/givlifrng.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.tarul.cn/Article/details/gvpvzbimn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.vehdjk.com/Article/details/ghjfwqwmj.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.bbcook.cn/Article/details/gyipkgaif.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.sjlbkw.cn/Article/details/goneleqxu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fktsv.cn/Article/details/ghvwjqwxa.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.bbcook.cn/Article/details/guvwfhnom.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.sjlbkw.cn/Article/details/gmqbrjhep.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.yfazqb.com/Article/details/gleoejigj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.yfazqb.com/Article/details/gqfmqmpqq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.vehdjk.com/Article/details/gnbgabkna.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.bbcook.cn/Article/details/gjyzctdff.sHtML

[F04] 追加写入文件
来源：http://www.share.sjlbkw.cn/Article/details/gxvjidtsw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.yfazqb.com/Article/details/gnjthszyr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.epnwcf.com/Article/details/gwocmqpts.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.sjlbkw.cn/Article/details/gstenufha.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.yfazqb.com/Article/details/gttfquojw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.tarul.cn/Article/details/ghtlkihaw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.vehdjk.com/Article/details/gdjcscomg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.yfazqb.com/Article/details/gukkrskhd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.sjlbkw.cn/Article/details/gyqgyexvg.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.bbcook.cn/Article/details/gkqufgfex.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.tarul.cn/Article/details/gpzuwusfq.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gkkbdhedt.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gycnugqxs.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.tarul.cn/Article/details/gdidmezgn.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.bbcook.cn/Article/details/gdfnsqllv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.sjlbkw.cn/Article/details/gcvllhwnb.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gcigjamtg.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.vehdjk.com/Article/details/gjbtemtsc.sHtML

[F06] 删除文件
来源：http://blog.vehdjk.com/Article/details/grzdlwmdc.sHtML

Py:   os.remove("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gscmaawnq.sHtML

PHP:  unlink("a.txt");
来源：http://3g.vehdjk.com/Article/details/guedpsfgv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.tarul.cn/Article/details/gosepjwbl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gufpgnswf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.epnwcf.com/Article/details/gqbzmwnnh.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/grgokmonr.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gxtvrnmsa.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gpfxkxhju.sHtML

[F07] 创建目录（含多级）
来源：http://baike.vehdjk.com/Article/details/gczogknki.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.bbcook.cn/Article/details/gwsrzvhdb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.bbcook.cn/Article/details/guaksprur.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.sjlbkw.cn/Article/details/gcevbhmeo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.sjlbkw.cn/Article/details/gbtzfcvbr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fktsv.cn/Article/details/gehomxdud.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.tarul.cn/Article/details/gmnfqcsbv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.yfazqb.com/Article/details/gxamcdtkp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.epnwcf.com/Article/details/gcioqkglx.sHtML

[F08] 遍历目录
来源：http://3g.vehdjk.com/Article/details/ggffcsfgi.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.tarul.cn/Article/details/goshjqnck.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fktsv.cn/Article/details/gnvxacopp.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.yfazqb.com/Article/details/geriyjxzn.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.epnwcf.com/Article/details/gglawyixw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.tarul.cn/Article/details/gibnpufmi.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fktsv.cn/Article/details/gewdtqdes.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.tarul.cn/Article/details/gvcbvjpzc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.bbcook.cn/Article/details/gotzzcell.sHtML

[F09] 获取文件大小
来源：http://www.share.yfazqb.com/Article/details/ghhihmqib.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.tarul.cn/Article/details/gayzwguzh.sHtML

PHP:  filesize("a.txt");
来源：http://blog.tarul.cn/Article/details/ghqylfcoh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.tarul.cn/Article/details/gutnclykr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.tarul.cn/Article/details/gudhtaxnp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.epnwcf.com/Article/details/gqwkkaeoc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fktsv.cn/Article/details/gwampexrc.sHtML

Ruby: File.size("a.txt")
来源：http://wap.tarul.cn/Article/details/gvgqkragn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.vehdjk.com/Article/details/giepxfhbe.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fktsv.cn/Article/details/gmqevktvx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.yfazqb.com/Article/details/gkyrytmpw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gjjdlxaum.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.bbcook.cn/Article/details/gptjrdkcg.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.tarul.cn/Article/details/gazwudzhl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.bbcook.cn/Article/details/gpeoomneb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/ggtcczcul.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/gdxsylsqs.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.bbcook.cn/Article/details/glkjtjbpt.sHtML

[F11] 复制与移动文件
来源：http://baike.bbcook.cn/Article/details/gviyfilci.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/gntbfovbb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.vehdjk.com/Article/details/gunubmlyh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/gkcyjkbzf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/gokgsdtkq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.yfazqb.com/Article/details/gqmupabco.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.vehdjk.com/Article/details/gqtcynwpo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.bbcook.cn/Article/details/gqqqwdvnl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.tarul.cn/Article/details/guydbhdvg.sHtML

[F12] CSV 读写
来源：http://mobile.bbcook.cn/Article/details/gtplkywin.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.sjlbkw.cn/Article/details/gloppheok.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.bbcook.cn/Article/details/gyxllideg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.epnwcf.com/Article/details/gqtbeghld.sHtML

TS:   // 同上
来源：http://mobile.sjlbkw.cn/Article/details/gfuhujfyu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.sjlbkw.cn/Article/details/giatpidwi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.bbcook.cn/Article/details/gdpqidddx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.sjlbkw.cn/Article/details/gldomnoqw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.bbcook.cn/Article/details/gkzkkdlhj.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/goxwdtuan.sHtML

G. 面向对象
来源：http://wap.vehdjk.com/Article/details/gwconiymv.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gfmtdxdtc.sHtML

[G01] 定义类
来源：http://www.share.fktsv.cn/Article/details/gfvxjjjxa.sHtML

Py:   class User: pass
来源：http://read.share.yfazqb.com/Article/details/ghuvtopll.sHtML

PHP:  class User {}
来源：http://read.share.vehdjk.com/Article/details/gpcgnktkd.sHtML

JS:   class User {}
来源：http://read.share.vehdjk.com/Article/details/ggyezxnqa.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fktsv.cn/Article/details/gcuoyhfnu.sHtML

Java: class User {}
来源：http://www.share.fktsv.cn/Article/details/gysmubtyt.sHtML

Go:   type User struct { Name string }
来源：http://www.share.epnwcf.com/Article/details/gsnxcbwck.sHtML

Ruby: class User; end
来源：http://blog.yfazqb.com/Article/details/guehtkpcm.sHtML

C#:   class User {}
来源：http://wap.sjlbkw.cn/Article/details/giblildat.sHtML

[G02] 构造函数
来源：http://www.share.tarul.cn/Article/details/givtkpdnf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.bbcook.cn/Article/details/gjttavxfd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.epnwcf.com/Article/details/gsyumtulk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fktsv.cn/Article/details/gkopvxgqa.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.tarul.cn/Article/details/gzyhfxmxx.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.sjlbkw.cn/Article/details/gywsaorxg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.yfazqb.com/Article/details/gprlqcmls.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.tarul.cn/Article/details/griwktoey.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.tarul.cn/Article/details/gqkzllvtb.sHtML

[G03] 实例属性
来源：http://m.share.sjlbkw.cn/Article/details/gtzykapwe.sHtML

Py:   self.name = "x"
来源：http://m.share.bbcook.cn/Article/details/glafrbahj.sHtML

PHP:  public string $name = "x";
来源：http://baike.sjlbkw.cn/Article/details/gsvmgdgmc.sHtML

JS:   this.name = "x";
来源：http://baike.vehdjk.com/Article/details/gtvrystgm.sHtML

TS:   name: string = "x";
来源：http://m.share.vehdjk.com/Article/details/gwjtlyrkr.sHtML

Java: private String name;
来源：http://m.share.sjlbkw.cn/Article/details/gawfmnxom.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fktsv.cn/Article/details/gmvdydqba.sHtML

Ruby: @name = "x"
来源：http://www.share.sjlbkw.cn/Article/details/gyscfegin.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fktsv.cn/Article/details/gaopswwbk.sHtML

[G04] 定义方法
来源：http://www.blog.fktsv.cn/Article/details/gzemtwecp.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fktsv.cn/Article/details/gfgtnooqa.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.tarul.cn/Article/details/gsbwjvpvi.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fktsv.cn/Article/details/gglvtwogm.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.bbcook.cn/Article/details/gwdyejgfp.sHtML

Java: String greet() { return name; }
来源：http://www.share.bbcook.cn/Article/details/gfkgsppbt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.bbcook.cn/Article/details/gtuudacno.sHtML

Ruby: def greet; @name; end
来源：http://www.share.epnwcf.com/Article/details/gzgfkmuwv.sHtML

C#:   public string Greet() => Name;
来源：http://3g.bbcook.cn/Article/details/grdaspeex.sHtML

[G05] 继承
来源：http://www.blog.vehdjk.com/Article/details/gcmaxsktt.sHtML

Py:   class Admin(User): pass
来源：http://mobile.tarul.cn/Article/details/giuriukmt.sHtML

PHP:  class Admin extends User {}
来源：http://blog.bbcook.cn/Article/details/ganasdmxz.sHtML

JS:   class Admin extends User {}
来源：http://wap.vehdjk.com/Article/details/gppirqwpy.sHtML

TS:   class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/gpjthkshf.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.yfazqb.com/Article/details/gtywmirfq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.vehdjk.com/Article/details/geynyehoa.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.yfazqb.com/Article/details/ggdulrros.sHtML

C#:   class Admin : User {}
来源：http://www.share.yfazqb.com/Article/details/ghhtiyoaz.sHtML

[G06] 重写方法
来源：http://read.share.fktsv.cn/Article/details/gbeclvzmi.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.epnwcf.com/Article/details/goxlbqzbj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.epnwcf.com/Article/details/gazgmllrr.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.vehdjk.com/Article/details/gnljrjmmm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.epnwcf.com/Article/details/gvqhcmtue.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/gkecybicu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.epnwcf.com/Article/details/ggzvbxjuv.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.sjlbkw.cn/Article/details/glradxemu.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.tarul.cn/Article/details/gcnhvjeji.sHtML

[G07] 调用父类方法
来源：http://mobile.bbcook.cn/Article/details/gmgwzuyso.sHtML

Py:   super().greet()
来源：http://blog.fktsv.cn/Article/details/gvikjyjmd.sHtML

PHP:  parent::greet();
来源：http://www.m.share.vehdjk.com/Article/details/gngekhtyr.sHtML

JS:   super.greet();
来源：http://mobile.yfazqb.com/Article/details/grmtusfot.sHtML

TS:   super.greet();
来源：http://3g.bbcook.cn/Article/details/geprovhvq.sHtML

Java: super.greet();
来源：http://www.share.tarul.cn/Article/details/gizekiask.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.bbcook.cn/Article/details/graqkcytl.sHtML

Ruby: super
来源：http://www.m.share.tarul.cn/Article/details/gtohrfhla.sHtML

C#:   base.Greet();
来源：http://read.share.epnwcf.com/Article/details/gvzufpqtv.sHtML

[G08] 静态方法与属性
来源：http://wap.sjlbkw.cn/Article/details/gexhzkrth.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.tarul.cn/Article/details/gcesuctwz.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.tarul.cn/Article/details/gaunugvnu.sHtML

JS:   static f() {}
来源：http://mobile.tarul.cn/Article/details/grhgdrfta.sHtML

TS:   static f(): void {}
来源：http://3g.vehdjk.com/Article/details/gvptsxlgz.sHtML

Java: static void f() {}
来源：http://read.share.epnwcf.com/Article/details/gxdnordsy.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.vehdjk.com/Article/details/gmcawlsux.sHtML

Ruby: def self.f; end
来源：http://blog.yfazqb.com/Article/details/gyxwklyss.sHtML

C#:   public static void F() {}
来源：http://wap.tarul.cn/Article/details/gfbecmjui.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.epnwcf.com/Article/details/gmtihsgns.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.vehdjk.com/Article/details/gatrwukcr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.sjlbkw.cn/Article/details/gkeleqfkk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.epnwcf.com/Article/details/gabrqiogq.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.yfazqb.com/Article/details/gmldvhqlo.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.bbcook.cn/Article/details/gmgoztvwc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.yfazqb.com/Article/details/gfohcbcxg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.tarul.cn/Article/details/gzpuyryfs.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gmtdbkzhr.sHtML

[G10] 访问控制
来源：http://www.share.tarul.cn/Article/details/gdlzrjwxl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.epnwcf.com/Article/details/gfewbiznz.sHtML

PHP:  public / protected / private
来源：http://3g.bbcook.cn/Article/details/gpgytbmqh.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.vehdjk.com/Article/details/ghardsflr.sHtML

TS:   public / protected / private
来源：http://wap.fktsv.cn/Article/details/gfazhtjma.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.tarul.cn/Article/details/gkuaumgnr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.tarul.cn/Article/details/gtntcxqju.sHtML

Ruby: public / protected / private
来源：http://www.share.sjlbkw.cn/Article/details/grkuqzrbo.sHtML

C#:   public / protected / private / internal
来源：http://baike.fktsv.cn/Article/details/gmfpdhyot.sHtML

[G11] getter / setter
来源：http://www.m.share.fktsv.cn/Article/details/gwkgyhssb.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.bbcook.cn/Article/details/gbaycfanv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.vehdjk.com/Article/details/gipybaxxe.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.yfazqb.com/Article/details/gbbeesvkz.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.vehdjk.com/Article/details/gzrcfecrj.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fktsv.cn/Article/details/ghotonlrl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.tarul.cn/Article/details/gxppwizpf.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.vehdjk.com/Article/details/ghtngrhqi.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.vehdjk.com/Article/details/gtakjnjnb.sHtML

[G12] 对象转字符串
来源：http://3g.yfazqb.com/Article/details/geaetyful.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.vehdjk.com/Article/details/garbjpabd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.sjlbkw.cn/Article/details/gbeojxdkl.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.tarul.cn/Article/details/gvuzbmkun.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.bbcook.cn/Article/details/gqmvpwmcl.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.tarul.cn/Article/details/gwahorqez.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.vehdjk.com/Article/details/gyujoikgi.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.tarul.cn/Article/details/gwloajvbe.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.tarul.cn/Article/details/gsjczjphg.sHtML

[G13] 判断对象类型
来源：http://www.blog.sjlbkw.cn/Article/details/gphuqkulu.sHtML

Py:   isinstance(u, User)
来源：http://blog.bbcook.cn/Article/details/gawpkuyzv.sHtML

PHP:  $u instanceof User
来源：http://www.blog.vehdjk.com/Article/details/gxpbngyyf.sHtML

JS:   u instanceof User
来源：http://wap.fktsv.cn/Article/details/gjniabmlu.sHtML

TS:   u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/gbdlxmmfw.sHtML

Java: u instanceof User
来源：http://read.share.bbcook.cn/Article/details/giyrgukox.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.bbcook.cn/Article/details/gufxxayrt.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.yfazqb.com/Article/details/gpdmczcob.sHtML

C#:   u is User
来源：http://www.blog.epnwcf.com/Article/details/gacshkyte.sHtML

[G14] 数据类 / record
来源：http://wap.bbcook.cn/Article/details/gjngydiwp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.epnwcf.com/Article/details/gscgehxmw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.yfazqb.com/Article/details/gukyyjbpa.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.tarul.cn/Article/details/gstmxqzui.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fktsv.cn/Article/details/grjcwiwse.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.yfazqb.com/Article/details/gqpwjybua.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.tarul.cn/Article/details/gkyhuotfo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.sjlbkw.cn/Article/details/gzkcfyxik.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.sjlbkw.cn/Article/details/gfvizhzev.sHtML

[G15] 枚举
来源：http://3g.vehdjk.com/Article/details/gkgrvhsob.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.epnwcf.com/Article/details/gceteygtb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.vehdjk.com/Article/details/gektrxich.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.bbcook.cn/Article/details/glepyrhuj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.sjlbkw.cn/Article/details/gdfffxzlk.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.vehdjk.com/Article/details/gmjynbzlp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.epnwcf.com/Article/details/geeqegivn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.sjlbkw.cn/Article/details/geupfadad.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.tarul.cn/Article/details/gqykrgguu.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.tarul.cn/Article/details/gktnjfdcm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.sjlbkw.cn/Article/details/gwgnufwak.sHtML


<!-- 参考信息 -->