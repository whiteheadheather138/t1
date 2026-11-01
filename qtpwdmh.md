代发 wailian999

[E18] 模板占位符替换
来源：http://www.share.tarul.cn/Article/details/gzbkkleyo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.tarul.cn/Article/details/gdpdwlmxg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.tarul.cn/Article/details/gpkoitatn.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.yfazqb.com/Article/details/guomydsny.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.bbcook.cn/Article/details/gxsbyndub.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.epnwcf.com/Article/details/gqytyilxy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.vehdjk.com/Article/details/gowljvxam.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.epnwcf.com/Article/details/gqejfebld.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.vehdjk.com/Article/details/gnrflagup.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.sjlbkw.cn/Article/details/gprlsqwwx.sHtML

Py:   s.splitlines()
来源：http://www.share.yfazqb.com/Article/details/gkfvmwwfj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.tarul.cn/Article/details/gfnyxuvhb.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.tarul.cn/Article/details/gchqicitw.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.epnwcf.com/Article/details/gyvcjvltm.sHtML

Java: s.lines().toList()
来源：http://www.m.share.yfazqb.com/Article/details/glctdvqll.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.yfazqb.com/Article/details/gkukfodgc.sHtML

Ruby: s.lines
来源：http://wap.fktsv.cn/Article/details/ggdsfhbdd.sHtML

C#:   s.Split('\n')
来源：http://www.share.sjlbkw.cn/Article/details/goyfgjkkd.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.vehdjk.com/Article/details/gguortttl.sHtML

Py:   if not s:
来源：http://baike.bbcook.cn/Article/details/gwnenewkg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.sjlbkw.cn/Article/details/gfqqrhesc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.bbcook.cn/Article/details/gnqihbmij.sHtML

TS:   if (s === "") {}
来源：http://mobile.tarul.cn/Article/details/gymqfxdjo.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.epnwcf.com/Article/details/guluhcybb.sHtML

Go:   if s == "" {}
来源：http://read.share.vehdjk.com/Article/details/ghxlnvpxz.sHtML

Ruby: if s.empty?
来源：http://mobile.fktsv.cn/Article/details/gdafgbxiu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.tarul.cn/Article/details/gjlnghioe.sHtML

[E21] 超长截断加省略号
来源：http://3g.vehdjk.com/Article/details/guuzqtxsy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.epnwcf.com/Article/details/gmcinbhtt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.sjlbkw.cn/Article/details/gruhzsiqx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.epnwcf.com/Article/details/gypkpmrqx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.tarul.cn/Article/details/gbizhzcre.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/gdwtnjbew.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.yfazqb.com/Article/details/gzgcuwgpu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/gtychorow.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.sjlbkw.cn/Article/details/gmkodljlh.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.epnwcf.com/Article/details/gyskeloub.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.vehdjk.com/Article/details/gialxxpev.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.tarul.cn/Article/details/gqumsbkdz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.bbcook.cn/Article/details/gvkyvtsro.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.epnwcf.com/Article/details/gskrnhkze.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.tarul.cn/Article/details/gvohectvp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.yfazqb.com/Article/details/gkoqpnzia.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.bbcook.cn/Article/details/gycsrcyvq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.sjlbkw.cn/Article/details/gafxwxdab.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/goxweevpn.sHtML

F. 文件与目录
来源：http://mobile.sjlbkw.cn/Article/details/gixyklthn.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gxjaodmfk.sHtML

[F01] 读取整个文件
来源：http://3g.epnwcf.com/Article/details/gchlipbbc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.yfazqb.com/Article/details/gwaeaiksd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gnqxixeab.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.sjlbkw.cn/Article/details/gpfinxpkm.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fktsv.cn/Article/details/gccntukdm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.tarul.cn/Article/details/gtkxuxqyp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.bbcook.cn/Article/details/gragveuxl.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gsrrakutq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gjtxtcwpf.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.epnwcf.com/Article/details/gmmjxilpe.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fktsv.cn/Article/details/gxbnivzxz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbhodzpqg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.tarul.cn/Article/details/gmzrtkqdf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.yfazqb.com/Article/details/gyfvanhhd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.epnwcf.com/Article/details/gekfuenjz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.epnwcf.com/Article/details/glljfrcgi.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.tarul.cn/Article/details/gmryjrtii.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.bbcook.cn/Article/details/ggfmomjge.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.sjlbkw.cn/Article/details/gwwuuhdec.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.epnwcf.com/Article/details/gsgbnbbkd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.bbcook.cn/Article/details/gtcpgvtrm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.sjlbkw.cn/Article/details/gpnnhodck.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.vehdjk.com/Article/details/gsoskyxis.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.sjlbkw.cn/Article/details/gbujacszs.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.vehdjk.com/Article/details/gvbcezmly.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.bbcook.cn/Article/details/ghyvgzsnd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.yfazqb.com/Article/details/gkreahdel.sHtML

[F04] 追加写入文件
来源：http://m.share.tarul.cn/Article/details/gsulifmxw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.bbcook.cn/Article/details/ginnmstaw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.tarul.cn/Article/details/gxuzoxofu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.sjlbkw.cn/Article/details/gzibugxti.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fktsv.cn/Article/details/gnqmvvgvj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.vehdjk.com/Article/details/gxjaihybo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fktsv.cn/Article/details/gxbkgdlov.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.vehdjk.com/Article/details/gdwzujfzl.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.vehdjk.com/Article/details/gzcohzjoa.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.bbcook.cn/Article/details/gmhhrnqdo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.bbcook.cn/Article/details/gndazdkvn.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.bbcook.cn/Article/details/gohyrexja.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.yfazqb.com/Article/details/gyijhbeon.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/guimqhakq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/glhigajxn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.tarul.cn/Article/details/gcqwscfyg.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gxhrkkycj.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/guqyhfgvg.sHtML

[F06] 删除文件
来源：http://www.m.share.fktsv.cn/Article/details/gbjvtysni.sHtML

Py:   os.remove("a.txt")
来源：http://blog.yfazqb.com/Article/details/gqdgnfdpw.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gjmwouqbc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.bbcook.cn/Article/details/gefzohkmp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fktsv.cn/Article/details/gjugswqxu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.epnwcf.com/Article/details/gyrurjegf.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.yfazqb.com/Article/details/gvlsmfpiw.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gxzkxbrah.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gkdowndja.sHtML

[F07] 创建目录（含多级）
来源：http://wap.yfazqb.com/Article/details/gosqbzfeq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.vehdjk.com/Article/details/gxawqrheg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.bbcook.cn/Article/details/gfzsrokae.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.epnwcf.com/Article/details/gnqrdroos.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.sjlbkw.cn/Article/details/gciornfbz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fktsv.cn/Article/details/gdzpbgvoz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.vehdjk.com/Article/details/gplymhtfx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.bbcook.cn/Article/details/gspxtpznv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.yfazqb.com/Article/details/gnjotwspe.sHtML

[F08] 遍历目录
来源：http://read.share.tarul.cn/Article/details/gdawnhjrd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.yfazqb.com/Article/details/gynwkluch.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.vehdjk.com/Article/details/gzxsvmmsn.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.vehdjk.com/Article/details/gcicnzsgq.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.sjlbkw.cn/Article/details/gvvxdnqvp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.bbcook.cn/Article/details/ggcryjdet.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.vehdjk.com/Article/details/gvyzdkmtu.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fktsv.cn/Article/details/gpqwnqmix.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.yfazqb.com/Article/details/gutzbimzj.sHtML

[F09] 获取文件大小
来源：http://blog.vehdjk.com/Article/details/ggdznhvzq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.vehdjk.com/Article/details/gupsdtwme.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gsoqnmuiw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fktsv.cn/Article/details/gdaffadfg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.vehdjk.com/Article/details/gpuqvjuwn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.yfazqb.com/Article/details/gswfetkim.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fktsv.cn/Article/details/gwbscqfxs.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.tarul.cn/Article/details/gqjqknznr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fktsv.cn/Article/details/gxrtiepkg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.yfazqb.com/Article/details/grmtnllfj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gxzzmhpgw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.yfazqb.com/Article/details/gpgnkkyhy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.yfazqb.com/Article/details/gkjrobugl.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fktsv.cn/Article/details/gnnqssxbz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.sjlbkw.cn/Article/details/geeqyxean.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gonktnytp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gdmcvfqak.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.vehdjk.com/Article/details/grofugyar.sHtML

[F11] 复制与移动文件
来源：http://m.share.tarul.cn/Article/details/glrdtynsb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gkdcyjrlm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.bbcook.cn/Article/details/ghvmtmkvs.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.yfazqb.com/Article/details/gpemewoyk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.bbcook.cn/Article/details/gwlqezsse.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.vehdjk.com/Article/details/gftaxowtu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.sjlbkw.cn/Article/details/gufxxvpvs.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.bbcook.cn/Article/details/gpeochmsa.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.epnwcf.com/Article/details/gzqfecnph.sHtML

[F12] CSV 读写
来源：http://3g.vehdjk.com/Article/details/gotthgqbk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fktsv.cn/Article/details/gaualxnbu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.vehdjk.com/Article/details/gbpkytahy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.tarul.cn/Article/details/gvhksckkb.sHtML

TS:   // 同上
来源：http://www.m.share.yfazqb.com/Article/details/gdwkaqhel.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.epnwcf.com/Article/details/gizkparku.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fktsv.cn/Article/details/grkshkgig.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fktsv.cn/Article/details/glitxrbay.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.tarul.cn/Article/details/gcsruxtfx.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/goyoetweg.sHtML

G. 面向对象
来源：http://m.share.fktsv.cn/Article/details/geronhtie.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/ggfjyikrr.sHtML

[G01] 定义类
来源：http://baike.bbcook.cn/Article/details/gezwkpzsd.sHtML

Py:   class User: pass
来源：http://baike.tarul.cn/Article/details/ggiehgpfm.sHtML

PHP:  class User {}
来源：http://wap.epnwcf.com/Article/details/gemyuqpvi.sHtML

JS:   class User {}
来源：http://baike.bbcook.cn/Article/details/gagsweotq.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.sjlbkw.cn/Article/details/gxharsjey.sHtML

Java: class User {}
来源：http://mobile.yfazqb.com/Article/details/gobsysbjh.sHtML

Go:   type User struct { Name string }
来源：http://mobile.epnwcf.com/Article/details/gbobhcapz.sHtML

Ruby: class User; end
来源：http://blog.epnwcf.com/Article/details/gghbmfzmm.sHtML

C#:   class User {}
来源：http://wap.sjlbkw.cn/Article/details/gjkszzjtw.sHtML

[G02] 构造函数
来源：http://www.m.share.bbcook.cn/Article/details/ggdhfggeo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.bbcook.cn/Article/details/gfsbcsoio.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fktsv.cn/Article/details/gpxnuvkpz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.yfazqb.com/Article/details/gnsjycnol.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.yfazqb.com/Article/details/gflemcldi.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.epnwcf.com/Article/details/gwmmpvgzy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fktsv.cn/Article/details/gxtivozou.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fktsv.cn/Article/details/gesvzejig.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.sjlbkw.cn/Article/details/gysexrjtw.sHtML

[G03] 实例属性
来源：http://baike.sjlbkw.cn/Article/details/gvjdjeusi.sHtML

Py:   self.name = "x"
来源：http://3g.sjlbkw.cn/Article/details/gbjrfxpzr.sHtML

PHP:  public string $name = "x";
来源：http://www.share.vehdjk.com/Article/details/gdgqqmkvs.sHtML

JS:   this.name = "x";
来源：http://m.share.vehdjk.com/Article/details/gjdhcjmab.sHtML

TS:   name: string = "x";
来源：http://www.m.share.epnwcf.com/Article/details/gujdmujxp.sHtML

Java: private String name;
来源：http://baike.vehdjk.com/Article/details/gcmwmegax.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.sjlbkw.cn/Article/details/gaetmxumu.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fktsv.cn/Article/details/gfibojkil.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.sjlbkw.cn/Article/details/gesekuncb.sHtML

[G04] 定义方法
来源：http://blog.fktsv.cn/Article/details/ggtnxxsxk.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.epnwcf.com/Article/details/gtsuuuhvd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fktsv.cn/Article/details/gqdhvfdjv.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gzigllflo.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.vehdjk.com/Article/details/giokajsrh.sHtML

Java: String greet() { return name; }
来源：http://mobile.epnwcf.com/Article/details/gkzwpbfig.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.bbcook.cn/Article/details/glpnznikc.sHtML

Ruby: def greet; @name; end
来源：http://blog.tarul.cn/Article/details/guikelgie.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.bbcook.cn/Article/details/gtmozyoon.sHtML

[G05] 继承
来源：http://blog.yfazqb.com/Article/details/grblqjarl.sHtML

Py:   class Admin(User): pass
来源：http://3g.epnwcf.com/Article/details/gsfntbhwr.sHtML

PHP:  class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/gswqslwld.sHtML

JS:   class Admin extends User {}
来源：http://read.share.yfazqb.com/Article/details/gjiswylzw.sHtML

TS:   class Admin extends User {}
来源：http://baike.tarul.cn/Article/details/glacpzcac.sHtML

Java: class Admin extends User {}
来源：http://3g.fktsv.cn/Article/details/gvjmeffbs.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.sjlbkw.cn/Article/details/gfqdnwxpn.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.sjlbkw.cn/Article/details/grzmeruta.sHtML

C#:   class Admin : User {}
来源：http://wap.tarul.cn/Article/details/gifuufgbl.sHtML

[G06] 重写方法
来源：http://www.share.tarul.cn/Article/details/gitrdloka.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.tarul.cn/Article/details/gasjmrjmk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.sjlbkw.cn/Article/details/gtbbyuzwe.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gckoxdhjn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.tarul.cn/Article/details/gbpsewshb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.vehdjk.com/Article/details/gjppnkxql.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.bbcook.cn/Article/details/gfzhgkuax.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.bbcook.cn/Article/details/gdekdkqdg.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.bbcook.cn/Article/details/gqotdqguz.sHtML

[G07] 调用父类方法
来源：http://m.share.tarul.cn/Article/details/gatphhcqi.sHtML

Py:   super().greet()
来源：http://read.share.tarul.cn/Article/details/gajmevlgm.sHtML

PHP:  parent::greet();
来源：http://wap.yfazqb.com/Article/details/gaeaqqdlt.sHtML

JS:   super.greet();
来源：http://read.share.yfazqb.com/Article/details/giqnjfzzy.sHtML

TS:   super.greet();
来源：http://www.share.tarul.cn/Article/details/gdehphdzb.sHtML

Java: super.greet();
来源：http://www.blog.sjlbkw.cn/Article/details/gqcnojapp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.bbcook.cn/Article/details/gtnvtqzkc.sHtML

Ruby: super
来源：http://3g.tarul.cn/Article/details/gpaqyiyiw.sHtML

C#:   base.Greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gpcyycxow.sHtML

[G08] 静态方法与属性
来源：http://m.share.yfazqb.com/Article/details/guxpopmqv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.sjlbkw.cn/Article/details/gfahjysgm.sHtML

PHP:  public static function f() {}
来源：http://read.share.bbcook.cn/Article/details/gyrafjvde.sHtML

JS:   static f() {}
来源：http://blog.yfazqb.com/Article/details/gztwiboda.sHtML

TS:   static f(): void {}
来源：http://www.blog.bbcook.cn/Article/details/giafunycq.sHtML

Java: static void f() {}
来源：http://mobile.epnwcf.com/Article/details/gvjezruej.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.epnwcf.com/Article/details/glogqczqp.sHtML

Ruby: def self.f; end
来源：http://www.share.bbcook.cn/Article/details/gifjcixnw.sHtML

C#:   public static void F() {}
来源：http://mobile.sjlbkw.cn/Article/details/gowhfuldc.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fktsv.cn/Article/details/gskvmhnke.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.epnwcf.com/Article/details/gqfwhjixs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.vehdjk.com/Article/details/gcdcmqkhu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.yfazqb.com/Article/details/gojokymti.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.yfazqb.com/Article/details/ghmzwjcux.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.yfazqb.com/Article/details/gzvmhpkbc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.tarul.cn/Article/details/gdgutquxc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.tarul.cn/Article/details/gsqyhaakf.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.epnwcf.com/Article/details/gmylloqjd.sHtML

[G10] 访问控制
来源：http://www.blog.yfazqb.com/Article/details/gwvnngtft.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.bbcook.cn/Article/details/gvwnnmkbg.sHtML

PHP:  public / protected / private
来源：http://read.share.tarul.cn/Article/details/giszcbqpi.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.tarul.cn/Article/details/goeihnbqp.sHtML

TS:   public / protected / private
来源：http://read.share.sjlbkw.cn/Article/details/godivfngr.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fktsv.cn/Article/details/glotslzbf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.sjlbkw.cn/Article/details/gsjzwdicy.sHtML

Ruby: public / protected / private
来源：http://www.share.tarul.cn/Article/details/glesrmyeb.sHtML

C#:   public / protected / private / internal
来源：http://baike.epnwcf.com/Article/details/gmlwlvffa.sHtML

[G11] getter / setter
来源：http://wap.epnwcf.com/Article/details/grzrfndia.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fktsv.cn/Article/details/gdriwfrxj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.tarul.cn/Article/details/gsookrdgq.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gywvfhyik.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.epnwcf.com/Article/details/gbulazjcn.sHtML

Java: public String getName() { return name; }
来源：http://blog.epnwcf.com/Article/details/glvikvymq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.bbcook.cn/Article/details/gnahoqnow.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.epnwcf.com/Article/details/gnmgsgoqy.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.yfazqb.com/Article/details/gojotejwr.sHtML

[G12] 对象转字符串
来源：http://read.share.epnwcf.com/Article/details/gxkwhbmho.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.yfazqb.com/Article/details/ghxavefpn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.yfazqb.com/Article/details/gljwnxbtk.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.epnwcf.com/Article/details/gxaxqocxe.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.epnwcf.com/Article/details/guborqprw.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.yfazqb.com/Article/details/gcwfkoaqj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.vehdjk.com/Article/details/grihxvmii.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.bbcook.cn/Article/details/gsmcbayjh.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.vehdjk.com/Article/details/gfiesqhry.sHtML

[G13] 判断对象类型
来源：http://www.share.epnwcf.com/Article/details/gabevitfy.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fktsv.cn/Article/details/gfadbeeco.sHtML

PHP:  $u instanceof User
来源：http://m.share.yfazqb.com/Article/details/gmwmlwopv.sHtML

JS:   u instanceof User
来源：http://www.blog.bbcook.cn/Article/details/gqzuvynpg.sHtML

TS:   u instanceof User
来源：http://mobile.vehdjk.com/Article/details/gbsaeavvs.sHtML

Java: u instanceof User
来源：http://www.m.share.yfazqb.com/Article/details/gsbqmhqgt.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.sjlbkw.cn/Article/details/ghljwbxju.sHtML

Ruby: u.is_a?(User)
来源：http://baike.tarul.cn/Article/details/gkzqphrko.sHtML

C#:   u is User
来源：http://read.share.epnwcf.com/Article/details/gydbiibdn.sHtML

[G14] 数据类 / record
来源：http://m.share.vehdjk.com/Article/details/gyuhmykwh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.tarul.cn/Article/details/gwcimpxvd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.bbcook.cn/Article/details/gohtphyyf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.yfazqb.com/Article/details/gbnrxhlfb.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.epnwcf.com/Article/details/gpsadmfwg.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fktsv.cn/Article/details/gmuhtcduq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.yfazqb.com/Article/details/gxkcetlll.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fktsv.cn/Article/details/gtrqpmrnh.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.vehdjk.com/Article/details/gzfwskhcx.sHtML

[G15] 枚举
来源：http://www.m.share.yfazqb.com/Article/details/gjaucszsm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.tarul.cn/Article/details/glcesztuh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.vehdjk.com/Article/details/gcbtxauht.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.vehdjk.com/Article/details/giwwgeqsy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.tarul.cn/Article/details/gmiilqxgj.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.yfazqb.com/Article/details/glufammzd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.epnwcf.com/Article/details/glshkpdgn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.vehdjk.com/Article/details/gcmuikmkc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.tarul.cn/Article/details/gwezllxyq.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.tarul.cn/Article/details/ghnevgygl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.vehdjk.com/Article/details/grywnfmte.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.bbcook.cn/Article/details/gksqxkpif.sHtML

JS:   Object.entries(obj)
来源：http://www.share.sjlbkw.cn/Article/details/glxjsxrnm.sHtML

TS:   Object.entries(obj)
来源：http://www.share.bbcook.cn/Article/details/gpoindqwx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.vehdjk.com/Article/details/gpmakbrmg.sHtML


<!-- 参考信息 -->