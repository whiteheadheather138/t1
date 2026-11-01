代发 wailian999

[E18] 模板占位符替换
来源：http://3g.sjlbkw.cn/Article/details/gosamgixk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.vehdjk.com/Article/details/gstlthafy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.tarul.cn/Article/details/gwqpngpgy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.vehdjk.com/Article/details/gisquasyj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.tarul.cn/Article/details/gocxiyrxe.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.sjlbkw.cn/Article/details/gggxfyhcb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.yfazqb.com/Article/details/gcnqcfaam.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.bbcook.cn/Article/details/gqjnsihmw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.bbcook.cn/Article/details/gjeptzkah.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.bbcook.cn/Article/details/gepztvted.sHtML

Py:   s.splitlines()
来源：http://www.share.epnwcf.com/Article/details/ghsyihqfq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.tarul.cn/Article/details/gkxnkgfbz.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.tarul.cn/Article/details/guqrzuboe.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.epnwcf.com/Article/details/gavwmgtvx.sHtML

Java: s.lines().toList()
来源：http://baike.sjlbkw.cn/Article/details/goidbydyf.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.sjlbkw.cn/Article/details/gvvjkrrdr.sHtML

Ruby: s.lines
来源：http://www.share.tarul.cn/Article/details/gfgvahvww.sHtML

C#:   s.Split('\n')
来源：http://read.share.tarul.cn/Article/details/gpdoqtmab.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.sjlbkw.cn/Article/details/gebbhaswc.sHtML

Py:   if not s:
来源：http://read.share.epnwcf.com/Article/details/grtwuvpnf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.epnwcf.com/Article/details/gwdeewrln.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.bbcook.cn/Article/details/gucznjpot.sHtML

TS:   if (s === "") {}
来源：http://3g.yfazqb.com/Article/details/gfeinrmry.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.vehdjk.com/Article/details/gafjnsckw.sHtML

Go:   if s == "" {}
来源：http://m.share.tarul.cn/Article/details/guhbgtijr.sHtML

Ruby: if s.empty?
来源：http://www.m.share.sjlbkw.cn/Article/details/gdcvzqebz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.yfazqb.com/Article/details/gzfmwunrw.sHtML

[E21] 超长截断加省略号
来源：http://wap.yfazqb.com/Article/details/gkvpmfddq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.tarul.cn/Article/details/ggtrvbcqq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.vehdjk.com/Article/details/gfzcskvvk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.epnwcf.com/Article/details/gxarbxxuj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gkzessphu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.sjlbkw.cn/Article/details/gwfnpqnkl.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.yfazqb.com/Article/details/gdhnlstzb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fktsv.cn/Article/details/gceauwxai.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/guafucfjy.sHtML

[E22] 字节长度与字符长度
来源：http://wap.yfazqb.com/Article/details/gnsomgjsn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.vehdjk.com/Article/details/gvqqwrgbl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/gztvvrous.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.vehdjk.com/Article/details/guhiljqfh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.tarul.cn/Article/details/gfteicrcb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.epnwcf.com/Article/details/gznldcfzg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.bbcook.cn/Article/details/gkgdpagxg.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.sjlbkw.cn/Article/details/gcvsodkah.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.bbcook.cn/Article/details/gvscaiynn.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gcqxvabqd.sHtML

F. 文件与目录
来源：http://m.share.yfazqb.com/Article/details/gnwwhwgux.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gafrvmmse.sHtML

[F01] 读取整个文件
来源：http://www.blog.vehdjk.com/Article/details/gveplqmtm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.bbcook.cn/Article/details/gxsimwnkw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gdruwurvt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fktsv.cn/Article/details/gvuefulld.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.yfazqb.com/Article/details/giqnavplc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.sjlbkw.cn/Article/details/gwzqdfndf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.yfazqb.com/Article/details/gukqfvslm.sHtML

Ruby: File.read("a.txt")
来源：http://baike.tarul.cn/Article/details/ggjrnipbb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/ggjkfatut.sHtML

[F02] 逐行读取文件
来源：http://blog.bbcook.cn/Article/details/gwpuzoazw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.epnwcf.com/Article/details/gabnnpqxi.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fktsv.cn/Article/details/gxtvxsgjj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fktsv.cn/Article/details/gtfefhqyo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.yfazqb.com/Article/details/gmzjofrag.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.epnwcf.com/Article/details/grfyhqtbc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.sjlbkw.cn/Article/details/gzyuixeqy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.epnwcf.com/Article/details/giwmluahg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.yfazqb.com/Article/details/gyrqewovq.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fktsv.cn/Article/details/gwunnueid.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.tarul.cn/Article/details/gagtapwio.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.vehdjk.com/Article/details/gewnlflqn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.yfazqb.com/Article/details/gfekjkcvh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.sjlbkw.cn/Article/details/gzioewtal.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.tarul.cn/Article/details/gqkdznzff.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.yfazqb.com/Article/details/gpjfmsaxx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.vehdjk.com/Article/details/gprcfegky.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.bbcook.cn/Article/details/gdttfhfay.sHtML

[F04] 追加写入文件
来源：http://wap.sjlbkw.cn/Article/details/galyrdqvi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.vehdjk.com/Article/details/gaublwium.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.bbcook.cn/Article/details/gtakuyzxs.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.sjlbkw.cn/Article/details/gfeymdcvf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.bbcook.cn/Article/details/giuagzmcm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.epnwcf.com/Article/details/gdqcfuggc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fktsv.cn/Article/details/gtbsuibwg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.bbcook.cn/Article/details/gahthfeww.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.sjlbkw.cn/Article/details/ggmvgjjrb.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.bbcook.cn/Article/details/giegvduqz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fktsv.cn/Article/details/gcxomcund.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.bbcook.cn/Article/details/gradxkblh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.epnwcf.com/Article/details/gbmncypnb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gwloxnevx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.yfazqb.com/Article/details/guauceroq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.sjlbkw.cn/Article/details/gcaimomha.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gjlxxuvpf.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.bbcook.cn/Article/details/goobtuhdv.sHtML

[F06] 删除文件
来源：http://www.blog.epnwcf.com/Article/details/gvqyfrgpi.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.tarul.cn/Article/details/gfdqkhbgx.sHtML

PHP:  unlink("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gfrwspkgx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/ghknuqsiy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/girgrbgni.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.epnwcf.com/Article/details/gvtzwtyqj.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.vehdjk.com/Article/details/gnngascre.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gfhizejni.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.yfazqb.com/Article/details/ggxbzdssk.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.epnwcf.com/Article/details/goamwamrz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.epnwcf.com/Article/details/gyaqfrhka.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.vehdjk.com/Article/details/gtujvfdwq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.vehdjk.com/Article/details/gdhsmawua.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.tarul.cn/Article/details/gvoofmsuz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fktsv.cn/Article/details/geywoaskh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.tarul.cn/Article/details/gevbzxnwa.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.yfazqb.com/Article/details/glkpnngkb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.epnwcf.com/Article/details/gmwiypnpf.sHtML

[F08] 遍历目录
来源：http://wap.epnwcf.com/Article/details/gtkikjnqp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.yfazqb.com/Article/details/garrbnmxx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.epnwcf.com/Article/details/gnzjiojpa.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.bbcook.cn/Article/details/glkukbvwi.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.sjlbkw.cn/Article/details/gndclgbyy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.epnwcf.com/Article/details/grlbdsrsa.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.yfazqb.com/Article/details/grpckktvn.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fktsv.cn/Article/details/gwafmrxaa.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.yfazqb.com/Article/details/gghcjjwib.sHtML

[F09] 获取文件大小
来源：http://m.share.yfazqb.com/Article/details/gjdvmokcw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gjljczret.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fktsv.cn/Article/details/giggjaoeg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.bbcook.cn/Article/details/gwcjwgpbq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.tarul.cn/Article/details/guhmsjahd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.epnwcf.com/Article/details/gpkezsfsr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.bbcook.cn/Article/details/gcvvgwaht.sHtML

Ruby: File.size("a.txt")
来源：http://3g.tarul.cn/Article/details/gpsxueaau.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fktsv.cn/Article/details/gmsgdutng.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.vehdjk.com/Article/details/gzxukggps.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.vehdjk.com/Article/details/ghmgniwzd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fktsv.cn/Article/details/ghttyladd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/goyasmwaj.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gnjoimmhv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fktsv.cn/Article/details/ghyulenwn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.yfazqb.com/Article/details/gxxgnyujg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/gqgcjdxqd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/gpcrkcogx.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fktsv.cn/Article/details/gzweuviyc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.tarul.cn/Article/details/gtrgksgiu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.vehdjk.com/Article/details/gkgxvjkaq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gwbocziho.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.yfazqb.com/Article/details/goegsumde.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.yfazqb.com/Article/details/giznwfthp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.vehdjk.com/Article/details/gsqodtwmf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.yfazqb.com/Article/details/gfumozdxs.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.yfazqb.com/Article/details/gbndqkjzx.sHtML

[F12] CSV 读写
来源：http://m.share.bbcook.cn/Article/details/gzupzsxea.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.epnwcf.com/Article/details/gyngggloo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.vehdjk.com/Article/details/gfyghpkup.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.epnwcf.com/Article/details/gzzdfvhsf.sHtML

TS:   // 同上
来源：http://blog.yfazqb.com/Article/details/gvqjhymzk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.bbcook.cn/Article/details/gthxcaxwo.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.vehdjk.com/Article/details/guefzjduc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.bbcook.cn/Article/details/gduooixju.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.vehdjk.com/Article/details/gpknqahth.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/glijjmiqu.sHtML

G. 面向对象
来源：http://baike.epnwcf.com/Article/details/gnqnqenli.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gtivblbud.sHtML

[G01] 定义类
来源：http://3g.bbcook.cn/Article/details/ghhdndudm.sHtML

Py:   class User: pass
来源：http://www.m.share.fktsv.cn/Article/details/gqscgdlxb.sHtML

PHP:  class User {}
来源：http://blog.tarul.cn/Article/details/gcbsiiqli.sHtML

JS:   class User {}
来源：http://m.share.tarul.cn/Article/details/gglmrpjxj.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.bbcook.cn/Article/details/gfxymkcmt.sHtML

Java: class User {}
来源：http://blog.sjlbkw.cn/Article/details/gydbqymvo.sHtML

Go:   type User struct { Name string }
来源：http://wap.yfazqb.com/Article/details/geofrbpwu.sHtML

Ruby: class User; end
来源：http://www.share.fktsv.cn/Article/details/ghuanqwgy.sHtML

C#:   class User {}
来源：http://www.blog.fktsv.cn/Article/details/grdwzckxu.sHtML

[G02] 构造函数
来源：http://3g.tarul.cn/Article/details/glkzxjggz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.tarul.cn/Article/details/gqvvrggrq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.tarul.cn/Article/details/gwdpcefef.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.tarul.cn/Article/details/gtbnbtzxx.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.bbcook.cn/Article/details/gzqglohty.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.vehdjk.com/Article/details/gblrivane.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.bbcook.cn/Article/details/gffmszddo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.vehdjk.com/Article/details/gpupoulag.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.tarul.cn/Article/details/gwhuyflqa.sHtML

[G03] 实例属性
来源：http://m.share.vehdjk.com/Article/details/gwlgqeqyi.sHtML

Py:   self.name = "x"
来源：http://baike.yfazqb.com/Article/details/gktzdskvt.sHtML

PHP:  public string $name = "x";
来源：http://mobile.yfazqb.com/Article/details/gevmcjeps.sHtML

JS:   this.name = "x";
来源：http://www.blog.fktsv.cn/Article/details/gfirkwsvm.sHtML

TS:   name: string = "x";
来源：http://baike.yfazqb.com/Article/details/gvnmidwxs.sHtML

Java: private String name;
来源：http://www.share.fktsv.cn/Article/details/gfboluuph.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.tarul.cn/Article/details/glsitodqo.sHtML

Ruby: @name = "x"
来源：http://mobile.tarul.cn/Article/details/gxgurktwq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.vehdjk.com/Article/details/gfsridbyi.sHtML

[G04] 定义方法
来源：http://www.m.share.sjlbkw.cn/Article/details/grjvjrnjh.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.tarul.cn/Article/details/ghvzqrcva.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.bbcook.cn/Article/details/gfmlbctks.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fktsv.cn/Article/details/gjdodnlev.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.tarul.cn/Article/details/gmqbdtxba.sHtML

Java: String greet() { return name; }
来源：http://wap.fktsv.cn/Article/details/gvyhzwsze.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fktsv.cn/Article/details/grltphxdq.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.epnwcf.com/Article/details/gtbgfbpfk.sHtML

C#:   public string Greet() => Name;
来源：http://3g.sjlbkw.cn/Article/details/gymljhuih.sHtML

[G05] 继承
来源：http://mobile.fktsv.cn/Article/details/gquujitib.sHtML

Py:   class Admin(User): pass
来源：http://read.share.tarul.cn/Article/details/ggbfbqjdu.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gqwmhboqu.sHtML

JS:   class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/ghbkqsvbv.sHtML

TS:   class Admin extends User {}
来源：http://read.share.tarul.cn/Article/details/ggnosigai.sHtML

Java: class Admin extends User {}
来源：http://baike.bbcook.cn/Article/details/gmqbckfjt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.epnwcf.com/Article/details/gcrxwqfgd.sHtML

Ruby: class Admin < User; end
来源：http://blog.bbcook.cn/Article/details/gxpvgpifr.sHtML

C#:   class Admin : User {}
来源：http://wap.yfazqb.com/Article/details/gxzytpfjs.sHtML

[G06] 重写方法
来源：http://blog.vehdjk.com/Article/details/gdugwtbns.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.bbcook.cn/Article/details/guqfqgipc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghuynnsym.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.yfazqb.com/Article/details/garefzlhy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/gterlmffo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gutrhspax.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.yfazqb.com/Article/details/gmbmshiem.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.epnwcf.com/Article/details/gowdmxqgz.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.yfazqb.com/Article/details/gesneskod.sHtML

[G07] 调用父类方法
来源：http://baike.epnwcf.com/Article/details/gxhajspdl.sHtML

Py:   super().greet()
来源：http://3g.yfazqb.com/Article/details/gpoloohbe.sHtML

PHP:  parent::greet();
来源：http://www.blog.tarul.cn/Article/details/glqinmdvy.sHtML

JS:   super.greet();
来源：http://read.share.sjlbkw.cn/Article/details/gyvjduaxq.sHtML

TS:   super.greet();
来源：http://www.blog.tarul.cn/Article/details/gaayxxamq.sHtML

Java: super.greet();
来源：http://www.share.vehdjk.com/Article/details/galfhjlda.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.vehdjk.com/Article/details/gyokawkov.sHtML

Ruby: super
来源：http://mobile.bbcook.cn/Article/details/givyxsahi.sHtML

C#:   base.Greet();
来源：http://mobile.vehdjk.com/Article/details/gbayeugmx.sHtML

[G08] 静态方法与属性
来源：http://blog.bbcook.cn/Article/details/gmqfhxwzq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.tarul.cn/Article/details/gkloenfmb.sHtML

PHP:  public static function f() {}
来源：http://read.share.bbcook.cn/Article/details/gtvrowumh.sHtML

JS:   static f() {}
来源：http://blog.epnwcf.com/Article/details/gpqwnidmx.sHtML

TS:   static f(): void {}
来源：http://3g.epnwcf.com/Article/details/ghkbatimi.sHtML

Java: static void f() {}
来源：http://wap.vehdjk.com/Article/details/gxjfcqwja.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.yfazqb.com/Article/details/gqfgecdee.sHtML

Ruby: def self.f; end
来源：http://baike.vehdjk.com/Article/details/gxvvyjhtv.sHtML

C#:   public static void F() {}
来源：http://mobile.bbcook.cn/Article/details/guehbwuyf.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.sjlbkw.cn/Article/details/gbyxjvozy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.sjlbkw.cn/Article/details/gupjwrbva.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.tarul.cn/Article/details/gqoyioium.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.sjlbkw.cn/Article/details/gcuhlazpr.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.sjlbkw.cn/Article/details/gcxzkejpe.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fktsv.cn/Article/details/gwynfuodr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fktsv.cn/Article/details/ggrksqfmz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.epnwcf.com/Article/details/gaqsmvhlk.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fktsv.cn/Article/details/gnfizpzgf.sHtML

[G10] 访问控制
来源：http://baike.yfazqb.com/Article/details/gnrauzamb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.sjlbkw.cn/Article/details/gmvnwkwyx.sHtML

PHP:  public / protected / private
来源：http://baike.yfazqb.com/Article/details/gitoxdgej.sHtML

JS:   #private 字段；其余公开
来源：http://baike.yfazqb.com/Article/details/giaouetip.sHtML

TS:   public / protected / private
来源：http://read.share.bbcook.cn/Article/details/gxwlhthxs.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.sjlbkw.cn/Article/details/gvtgokybl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.tarul.cn/Article/details/gupricahd.sHtML

Ruby: public / protected / private
来源：http://m.share.fktsv.cn/Article/details/geynnmrve.sHtML

C#:   public / protected / private / internal
来源：http://read.share.yfazqb.com/Article/details/gacymfcts.sHtML

[G11] getter / setter
来源：http://3g.bbcook.cn/Article/details/gyuzsdrfq.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.yfazqb.com/Article/details/gykbzkfvr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.yfazqb.com/Article/details/gbpldgaby.sHtML

JS:   get name() { return this._name; }
来源：http://baike.fktsv.cn/Article/details/gdyawjzus.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.vehdjk.com/Article/details/gwhetlwcp.sHtML

Java: public String getName() { return name; }
来源：http://www.share.tarul.cn/Article/details/gpgysddaq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.epnwcf.com/Article/details/gaxknmykd.sHtML

Ruby: attr_accessor :name
来源：http://3g.epnwcf.com/Article/details/gylwbefku.sHtML

C#:   public string Name { get; set; }
来源：http://blog.tarul.cn/Article/details/gqssmjqnn.sHtML

[G12] 对象转字符串
来源：http://baike.sjlbkw.cn/Article/details/gndejnyke.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.epnwcf.com/Article/details/gegitnqao.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.bbcook.cn/Article/details/gulfhavxy.sHtML

JS:   toString() { return this.name; }
来源：http://3g.yfazqb.com/Article/details/grefodzga.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.vehdjk.com/Article/details/gxcbolkdu.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fktsv.cn/Article/details/gkdsxwyhm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.bbcook.cn/Article/details/gmgushzlx.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fktsv.cn/Article/details/gkwaehicf.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.vehdjk.com/Article/details/gaahrbzqe.sHtML

[G13] 判断对象类型
来源：http://baike.yfazqb.com/Article/details/govhkwuzd.sHtML

Py:   isinstance(u, User)
来源：http://m.share.yfazqb.com/Article/details/gbecjrlmq.sHtML

PHP:  $u instanceof User
来源：http://wap.fktsv.cn/Article/details/gswlifhcp.sHtML

JS:   u instanceof User
来源：http://read.share.fktsv.cn/Article/details/grxdsvrza.sHtML

TS:   u instanceof User
来源：http://m.share.vehdjk.com/Article/details/gvtsjrtkn.sHtML

Java: u instanceof User
来源：http://3g.fktsv.cn/Article/details/galhpzxza.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.vehdjk.com/Article/details/gqdmqimtk.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.vehdjk.com/Article/details/gwvegkixw.sHtML

C#:   u is User
来源：http://www.blog.fktsv.cn/Article/details/guqolmias.sHtML

[G14] 数据类 / record
来源：http://blog.vehdjk.com/Article/details/gsfmmirlu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.bbcook.cn/Article/details/grjuktmzr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.bbcook.cn/Article/details/gecalqwgd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.bbcook.cn/Article/details/gcwgbmuqs.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.sjlbkw.cn/Article/details/gmwiupijv.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.sjlbkw.cn/Article/details/gzthavjxp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.epnwcf.com/Article/details/goglmmmay.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.sjlbkw.cn/Article/details/gyttmkriv.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.sjlbkw.cn/Article/details/gusqlxyrj.sHtML

[G15] 枚举
来源：http://3g.sjlbkw.cn/Article/details/guqmjjpmi.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.yfazqb.com/Article/details/gvlskasjk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.bbcook.cn/Article/details/grfhyluok.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.vehdjk.com/Article/details/ghnkhwlzd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.tarul.cn/Article/details/gnwmoicux.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fktsv.cn/Article/details/gewbjcgsy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.vehdjk.com/Article/details/gaeezehso.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.epnwcf.com/Article/details/glnchcrll.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.yfazqb.com/Article/details/goqpmhoag.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.epnwcf.com/Article/details/ghwgxpagk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fktsv.cn/Article/details/gdxydjiee.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.tarul.cn/Article/details/gmuobymji.sHtML

JS:   Object.entries(obj)
来源：http://www.share.tarul.cn/Article/details/gbnjdeuvi.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gnfwnaevv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.bbcook.cn/Article/details/gswcfkevj.sHtML


<!-- 参考信息 -->