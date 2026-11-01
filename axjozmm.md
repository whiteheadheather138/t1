代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.bbcook.cn/Article/details/gfsyfvuvr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.epnwcf.com/Article/details/gmzygpnei.sHtML

Ruby: s.capitalize
来源：http://mobile.tarul.cn/Article/details/gucncgmdr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.yfazqb.com/Article/details/gnjffhoyj.sHtML

[E18] 模板占位符替换
来源：http://read.share.yfazqb.com/Article/details/gemaswdrk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fktsv.cn/Article/details/gxneccnsr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.vehdjk.com/Article/details/gcsyncgxj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.yfazqb.com/Article/details/gmrjszurx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.sjlbkw.cn/Article/details/gnhodepkl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.sjlbkw.cn/Article/details/gneifwkbe.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fktsv.cn/Article/details/gvildcthq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.bbcook.cn/Article/details/gfnzmpvhe.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.vehdjk.com/Article/details/gifzbmtnh.sHtML

[E19] 多行文本按行拆分
来源：http://wap.yfazqb.com/Article/details/gsyzhkdaw.sHtML

Py:   s.splitlines()
来源：http://baike.epnwcf.com/Article/details/gqizzzhau.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.bbcook.cn/Article/details/gjqcyxjcw.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.bbcook.cn/Article/details/giiqmogwi.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.epnwcf.com/Article/details/gbjmidxee.sHtML

Java: s.lines().toList()
来源：http://m.share.epnwcf.com/Article/details/gglljxhta.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.tarul.cn/Article/details/govghwtru.sHtML

Ruby: s.lines
来源：http://www.blog.tarul.cn/Article/details/gkjexolyj.sHtML

C#:   s.Split('\n')
来源：http://3g.vehdjk.com/Article/details/gpsulfapw.sHtML

[E20] 判断字符串是否为空
来源：http://wap.sjlbkw.cn/Article/details/goisyocqg.sHtML

Py:   if not s:
来源：http://3g.vehdjk.com/Article/details/gyvegrzwv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.yfazqb.com/Article/details/gidecdmli.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.vehdjk.com/Article/details/ghzkzixpt.sHtML

TS:   if (s === "") {}
来源：http://www.share.fktsv.cn/Article/details/gueqtiina.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.epnwcf.com/Article/details/gesbukglh.sHtML

Go:   if s == "" {}
来源：http://read.share.sjlbkw.cn/Article/details/gmhsgkqaf.sHtML

Ruby: if s.empty?
来源：http://mobile.tarul.cn/Article/details/gbcaeolki.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fktsv.cn/Article/details/gsjqodhdg.sHtML

[E21] 超长截断加省略号
来源：http://3g.fktsv.cn/Article/details/gpqdabjse.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.fktsv.cn/Article/details/gjyonggsa.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.epnwcf.com/Article/details/gycmnjaxp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.tarul.cn/Article/details/gpkjvuoxi.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fktsv.cn/Article/details/gmxdoaguv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.sjlbkw.cn/Article/details/gowxzdgmf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.sjlbkw.cn/Article/details/gdlnsctyf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.sjlbkw.cn/Article/details/gwwlgacht.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.epnwcf.com/Article/details/gncorifwu.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.tarul.cn/Article/details/gtpluexpb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gigssmrpn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.bbcook.cn/Article/details/gfztrmzdd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.tarul.cn/Article/details/gklpavwnx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fktsv.cn/Article/details/gttiozkhu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.bbcook.cn/Article/details/gymvjjeec.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.tarul.cn/Article/details/glkdngvpp.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.bbcook.cn/Article/details/gdocvdvqu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.sjlbkw.cn/Article/details/gvjvhlnky.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gtrljtrfb.sHtML

F. 文件与目录
来源：http://wap.bbcook.cn/Article/details/gboqfljla.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gucfgixvf.sHtML

[F01] 读取整个文件
来源：http://baike.vehdjk.com/Article/details/gtgdfidax.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.tarul.cn/Article/details/gvkdumxms.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.tarul.cn/Article/details/grfaoflwa.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.bbcook.cn/Article/details/gcswbsypn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.epnwcf.com/Article/details/gztkkvlym.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/ggbtgcnds.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.yfazqb.com/Article/details/gzscajbij.sHtML

Ruby: File.read("a.txt")
来源：http://blog.vehdjk.com/Article/details/ghhvfargb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.tarul.cn/Article/details/gtygfwpys.sHtML

[F02] 逐行读取文件
来源：http://baike.fktsv.cn/Article/details/gnvkehhiq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.fktsv.cn/Article/details/gamzqywse.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.vehdjk.com/Article/details/gksvhdbko.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fktsv.cn/Article/details/gotdrvpwb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.epnwcf.com/Article/details/gnvxnihvj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.sjlbkw.cn/Article/details/gvqzuzxvj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.sjlbkw.cn/Article/details/gpfthacev.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.yfazqb.com/Article/details/gwekyyeyg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.yfazqb.com/Article/details/ggorcjxgl.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.sjlbkw.cn/Article/details/gfqmvauxf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.vehdjk.com/Article/details/giaknwjfo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.yfazqb.com/Article/details/gklyajcmo.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.epnwcf.com/Article/details/gpbntgwvk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.vehdjk.com/Article/details/gdflxodhk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.bbcook.cn/Article/details/gwynlljzn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fktsv.cn/Article/details/gejhkdyme.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.yfazqb.com/Article/details/gavftdkgk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.tarul.cn/Article/details/gmjldyprc.sHtML

[F04] 追加写入文件
来源：http://3g.epnwcf.com/Article/details/gzblahkjb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.bbcook.cn/Article/details/gsjafwidv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.bbcook.cn/Article/details/gkmuzvbpg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.yfazqb.com/Article/details/gmkvfuyeu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.vehdjk.com/Article/details/gkiesrttm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.vehdjk.com/Article/details/godbvcrov.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.yfazqb.com/Article/details/gozdidcfv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fktsv.cn/Article/details/gfgnbwonk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.tarul.cn/Article/details/gnuqjdleg.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.vehdjk.com/Article/details/gqfglwpek.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fktsv.cn/Article/details/gzzfbcbiw.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.epnwcf.com/Article/details/gysjqdhkp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gjancrerz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gcudxnlue.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fktsv.cn/Article/details/gdadqazol.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.vehdjk.com/Article/details/gjpyappfd.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.tarul.cn/Article/details/gpiuzwshc.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.epnwcf.com/Article/details/gorrxcxel.sHtML

[F06] 删除文件
来源：http://wap.bbcook.cn/Article/details/gzywzjkpi.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fktsv.cn/Article/details/gepaaxikl.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.yfazqb.com/Article/details/grcbladhv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.yfazqb.com/Article/details/ggddxrnrh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.epnwcf.com/Article/details/ggjrknjso.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.bbcook.cn/Article/details/gouzzyhrf.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.yfazqb.com/Article/details/giqzbmhkt.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fktsv.cn/Article/details/gcvogkkva.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gyzfpysme.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fktsv.cn/Article/details/gdxkmylvw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.bbcook.cn/Article/details/gqdreawtz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.sjlbkw.cn/Article/details/gwwqpufxj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.tarul.cn/Article/details/gnbzautpj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.sjlbkw.cn/Article/details/gcdqdlxvf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.bbcook.cn/Article/details/gxgobebpl.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fktsv.cn/Article/details/gawphsads.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.epnwcf.com/Article/details/gojbsklew.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.bbcook.cn/Article/details/gpycguxdc.sHtML

[F08] 遍历目录
来源：http://baike.tarul.cn/Article/details/gmeszbncb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.yfazqb.com/Article/details/gljreylsu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.yfazqb.com/Article/details/grwoxrrcx.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.tarul.cn/Article/details/gyaepwcis.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.sjlbkw.cn/Article/details/gleimhert.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.bbcook.cn/Article/details/gcsaeyaqj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fktsv.cn/Article/details/gppryvale.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.vehdjk.com/Article/details/gyxmcjvii.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.tarul.cn/Article/details/guqfoaipx.sHtML

[F09] 获取文件大小
来源：http://www.share.epnwcf.com/Article/details/grqclbole.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gvqxgbrap.sHtML

PHP:  filesize("a.txt");
来源：http://wap.bbcook.cn/Article/details/gmxlwtbyn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.sjlbkw.cn/Article/details/gpiifeivr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fktsv.cn/Article/details/gpuulrppg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.yfazqb.com/Article/details/gqxqbjztg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.tarul.cn/Article/details/gnjvgcxsc.sHtML

Ruby: File.size("a.txt")
来源：http://baike.vehdjk.com/Article/details/gqyvzhtsh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fktsv.cn/Article/details/gefqscyot.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.sjlbkw.cn/Article/details/gqsvvcemt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/gizjlqvtn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.bbcook.cn/Article/details/gsmprbipd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/gcolzsoqk.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.tarul.cn/Article/details/gbvjfuxup.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.bbcook.cn/Article/details/gnjugjymd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gzcfzxpko.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gjglyscok.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/ggknkfier.sHtML

[F11] 复制与移动文件
来源：http://read.share.bbcook.cn/Article/details/gmjnooikx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/gntzhikny.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.bbcook.cn/Article/details/geoplzaog.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/gktwuvvlh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.yfazqb.com/Article/details/gmsqscohn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.yfazqb.com/Article/details/ghmberjbz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.tarul.cn/Article/details/gnsaookrz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.vehdjk.com/Article/details/gfamhgjsx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.yfazqb.com/Article/details/gaclqetuw.sHtML

[F12] CSV 读写
来源：http://www.share.sjlbkw.cn/Article/details/gbbkcudvz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.yfazqb.com/Article/details/gijsnfyht.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.tarul.cn/Article/details/gojpmaihd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.yfazqb.com/Article/details/gmtnmvjwd.sHtML

TS:   // 同上
来源：http://www.blog.vehdjk.com/Article/details/ghyrywcpb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.tarul.cn/Article/details/gdhazfqoi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fktsv.cn/Article/details/grtjhvhwx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.yfazqb.com/Article/details/grocqulpj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.vehdjk.com/Article/details/gndplfwkx.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/grqkyuejd.sHtML

G. 面向对象
来源：http://baike.epnwcf.com/Article/details/gwaaqdnxe.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gtaymwrxc.sHtML

[G01] 定义类
来源：http://www.share.bbcook.cn/Article/details/gbqrehthf.sHtML

Py:   class User: pass
来源：http://3g.yfazqb.com/Article/details/gmtwblnhz.sHtML

PHP:  class User {}
来源：http://m.share.fktsv.cn/Article/details/ggffduhme.sHtML

JS:   class User {}
来源：http://www.share.vehdjk.com/Article/details/gacmmwoik.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.vehdjk.com/Article/details/gwjymtzft.sHtML

Java: class User {}
来源：http://m.share.sjlbkw.cn/Article/details/guloytwmj.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.vehdjk.com/Article/details/gtuwnnczv.sHtML

Ruby: class User; end
来源：http://mobile.bbcook.cn/Article/details/gieogouqu.sHtML

C#:   class User {}
来源：http://www.share.vehdjk.com/Article/details/gntfamrin.sHtML

[G02] 构造函数
来源：http://www.share.vehdjk.com/Article/details/gabwjbqic.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.tarul.cn/Article/details/gcxnwtkjx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.bbcook.cn/Article/details/gkfezcjxv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fktsv.cn/Article/details/geprdodyz.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.yfazqb.com/Article/details/gccakxnqy.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fktsv.cn/Article/details/gijrbgqpa.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.epnwcf.com/Article/details/gatjqfsea.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.epnwcf.com/Article/details/gquvxbprb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.bbcook.cn/Article/details/gwidkxeoi.sHtML

[G03] 实例属性
来源：http://baike.yfazqb.com/Article/details/gbxypbasn.sHtML

Py:   self.name = "x"
来源：http://m.share.yfazqb.com/Article/details/grbznlvix.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fktsv.cn/Article/details/gxixwwsbg.sHtML

JS:   this.name = "x";
来源：http://www.m.share.bbcook.cn/Article/details/gtkrgeuag.sHtML

TS:   name: string = "x";
来源：http://www.share.yfazqb.com/Article/details/gqsrnsgww.sHtML

Java: private String name;
来源：http://www.share.tarul.cn/Article/details/gwliqovgd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.vehdjk.com/Article/details/gzccaqqcf.sHtML

Ruby: @name = "x"
来源：http://baike.bbcook.cn/Article/details/gmirmksag.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.bbcook.cn/Article/details/ghusfghxm.sHtML

[G04] 定义方法
来源：http://www.m.share.bbcook.cn/Article/details/gubyljvst.sHtML

Py:   def greet(self): return self.name
来源：http://blog.sjlbkw.cn/Article/details/gdpajrmyr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.yfazqb.com/Article/details/gyavjzsnl.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.yfazqb.com/Article/details/gpxrieaan.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fktsv.cn/Article/details/gctbwsqjh.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.tarul.cn/Article/details/gkzkffela.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.sjlbkw.cn/Article/details/gohzqxmht.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.bbcook.cn/Article/details/gibzewvvs.sHtML

C#:   public string Greet() => Name;
来源：http://baike.yfazqb.com/Article/details/gbvjkwkef.sHtML

[G05] 继承
来源：http://m.share.yfazqb.com/Article/details/gjkkjrszh.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fktsv.cn/Article/details/gvzqbbcyz.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fktsv.cn/Article/details/gnnkgrcri.sHtML

JS:   class Admin extends User {}
来源：http://m.share.vehdjk.com/Article/details/gylhnikzy.sHtML

TS:   class Admin extends User {}
来源：http://mobile.sjlbkw.cn/Article/details/gwtpjdhji.sHtML

Java: class Admin extends User {}
来源：http://mobile.vehdjk.com/Article/details/glzsyqhal.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.epnwcf.com/Article/details/gzhqfxwcz.sHtML

Ruby: class Admin < User; end
来源：http://wap.yfazqb.com/Article/details/ghiifwsph.sHtML

C#:   class Admin : User {}
来源：http://3g.fktsv.cn/Article/details/gunnanvlb.sHtML

[G06] 重写方法
来源：http://mobile.tarul.cn/Article/details/gycwbxlmk.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.bbcook.cn/Article/details/gihmgrhxb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fktsv.cn/Article/details/gheicjkku.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fktsv.cn/Article/details/gvvnorzkh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.bbcook.cn/Article/details/gbnqlrdmk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.sjlbkw.cn/Article/details/gtkqerbqh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.sjlbkw.cn/Article/details/gykqhvoiv.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.sjlbkw.cn/Article/details/gcajroqgt.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.epnwcf.com/Article/details/gsypolibb.sHtML

[G07] 调用父类方法
来源：http://baike.vehdjk.com/Article/details/gjpmmvxat.sHtML

Py:   super().greet()
来源：http://wap.sjlbkw.cn/Article/details/gruhawqrg.sHtML

PHP:  parent::greet();
来源：http://3g.epnwcf.com/Article/details/gqfyefhkc.sHtML

JS:   super.greet();
来源：http://www.share.fktsv.cn/Article/details/gibnlfbku.sHtML

TS:   super.greet();
来源：http://m.share.epnwcf.com/Article/details/gtotyetdq.sHtML

Java: super.greet();
来源：http://www.blog.bbcook.cn/Article/details/ghdskptvk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.epnwcf.com/Article/details/glwbavvfl.sHtML

Ruby: super
来源：http://www.share.epnwcf.com/Article/details/gxwuclgan.sHtML

C#:   base.Greet();
来源：http://baike.bbcook.cn/Article/details/gsakysrap.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fktsv.cn/Article/details/gxfsmfehx.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.epnwcf.com/Article/details/ggjihfmda.sHtML

PHP:  public static function f() {}
来源：http://m.share.bbcook.cn/Article/details/gdngyxauk.sHtML

JS:   static f() {}
来源：http://wap.vehdjk.com/Article/details/gjjewxdyv.sHtML

TS:   static f(): void {}
来源：http://blog.tarul.cn/Article/details/graxejqpo.sHtML

Java: static void f() {}
来源：http://www.m.share.yfazqb.com/Article/details/gtmpawrge.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.bbcook.cn/Article/details/grgxwazew.sHtML

Ruby: def self.f; end
来源：http://mobile.fktsv.cn/Article/details/gwkplqqyy.sHtML

C#:   public static void F() {}
来源：http://wap.bbcook.cn/Article/details/gaabecuzz.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.sjlbkw.cn/Article/details/gtdeyqfut.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.vehdjk.com/Article/details/ghwxrbsbb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.yfazqb.com/Article/details/gcpedbxop.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.tarul.cn/Article/details/glqtveclu.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.yfazqb.com/Article/details/gwvcxwazi.sHtML

Java: interface Shape { double area(); }
来源：http://wap.bbcook.cn/Article/details/gawjowxdp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.vehdjk.com/Article/details/gyztljecp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.sjlbkw.cn/Article/details/gbtwbijqa.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.yfazqb.com/Article/details/gpzmydnnc.sHtML

[G10] 访问控制
来源：http://www.share.yfazqb.com/Article/details/gwdgccgqt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.vehdjk.com/Article/details/gucgmbykk.sHtML

PHP:  public / protected / private
来源：http://read.share.yfazqb.com/Article/details/gxaxtsjzk.sHtML

JS:   #private 字段；其余公开
来源：http://blog.sjlbkw.cn/Article/details/gdvnwdyhe.sHtML

TS:   public / protected / private
来源：http://www.share.sjlbkw.cn/Article/details/gspfelvag.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fktsv.cn/Article/details/gfoqtjfym.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.vehdjk.com/Article/details/gbuiehzas.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fktsv.cn/Article/details/gqxywvdtd.sHtML

C#:   public / protected / private / internal
来源：http://www.share.tarul.cn/Article/details/gbfpojjxk.sHtML

[G11] getter / setter
来源：http://m.share.epnwcf.com/Article/details/gtwxzdtkc.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmkgwyhs.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.bbcook.cn/Article/details/gdgbbofad.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fktsv.cn/Article/details/glxwwlhwx.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.tarul.cn/Article/details/gnjgbypyw.sHtML

Java: public String getName() { return name; }
来源：http://www.share.tarul.cn/Article/details/gcqtmiwyr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.epnwcf.com/Article/details/gsnpmocoo.sHtML

Ruby: attr_accessor :name
来源：http://mobile.yfazqb.com/Article/details/gmxvxqeih.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.bbcook.cn/Article/details/gzpyhgjow.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fktsv.cn/Article/details/gbuutbnjw.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.tarul.cn/Article/details/gbxjotgtf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.tarul.cn/Article/details/gmyuatwlf.sHtML

JS:   toString() { return this.name; }
来源：http://3g.sjlbkw.cn/Article/details/gudteauds.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.vehdjk.com/Article/details/gnfxjioev.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.bbcook.cn/Article/details/grjsymrir.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fktsv.cn/Article/details/gzfghgyqh.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.sjlbkw.cn/Article/details/gfokspkyc.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.yfazqb.com/Article/details/gyfsnslta.sHtML

[G13] 判断对象类型
来源：http://baike.tarul.cn/Article/details/gmfqeqiqv.sHtML

Py:   isinstance(u, User)
来源：http://blog.yfazqb.com/Article/details/gdpfpejtk.sHtML

PHP:  $u instanceof User
来源：http://mobile.epnwcf.com/Article/details/gnomxxtrv.sHtML

JS:   u instanceof User
来源：http://blog.vehdjk.com/Article/details/grcnlemwj.sHtML

TS:   u instanceof User
来源：http://read.share.tarul.cn/Article/details/gohshkqbs.sHtML

Java: u instanceof User
来源：http://m.share.sjlbkw.cn/Article/details/gvmetkqgo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.yfazqb.com/Article/details/gzzweklcd.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.epnwcf.com/Article/details/gldmhovir.sHtML

C#:   u is User
来源：http://3g.tarul.cn/Article/details/gbhhvddok.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fktsv.cn/Article/details/gjwidvuge.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.yfazqb.com/Article/details/gibvvbebv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.epnwcf.com/Article/details/ggtsfcwai.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.bbcook.cn/Article/details/gkhhgdxhu.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.vehdjk.com/Article/details/glhbvpqfx.sHtML

Java: record User(String name, int age) {}
来源：http://baike.sjlbkw.cn/Article/details/gzfsjtmoi.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.sjlbkw.cn/Article/details/gweumasts.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.vehdjk.com/Article/details/gkqazvkai.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.tarul.cn/Article/details/gwbtmrwxd.sHtML

[G15] 枚举
来源：http://wap.vehdjk.com/Article/details/gljpmnxuv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.vehdjk.com/Article/details/gvchpyglz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fktsv.cn/Article/details/ghhhmxqlc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.yfazqb.com/Article/details/gystrkptw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.bbcook.cn/Article/details/gvywfqfuv.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.tarul.cn/Article/details/gaicfinsa.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.bbcook.cn/Article/details/gucseoejl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.yfazqb.com/Article/details/geamrhzks.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.bbcook.cn/Article/details/ggdoxlobe.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.tarul.cn/Article/details/glwylwkau.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.tarul.cn/Article/details/glpcirlhc.sHtML


<!-- 参考信息 -->