代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.tarul.cn/Article/details/gppqozpxr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.yfazqb.com/Article/details/guislwajw.sHtML

Ruby: s.capitalize
来源：http://baike.sjlbkw.cn/Article/details/glqgmpzui.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.epnwcf.com/Article/details/gepsoxaov.sHtML

[E18] 模板占位符替换
来源：http://m.share.fktsv.cn/Article/details/gpuirqill.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.yfazqb.com/Article/details/gaclzyhfs.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.sjlbkw.cn/Article/details/gadtskiki.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fktsv.cn/Article/details/gblgsihpd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.sjlbkw.cn/Article/details/gcoorqdnr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.tarul.cn/Article/details/gnurfskyw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fktsv.cn/Article/details/gmasfcevt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.yfazqb.com/Article/details/gtxfosxyi.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fktsv.cn/Article/details/gtfdiyxmr.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fktsv.cn/Article/details/gvetwlqsf.sHtML

Py:   s.splitlines()
来源：http://www.share.bbcook.cn/Article/details/gqiadwncs.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.tarul.cn/Article/details/gsruncwgp.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.yfazqb.com/Article/details/gqqfpxgmc.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzlusjffu.sHtML

Java: s.lines().toList()
来源：http://wap.tarul.cn/Article/details/gkkfczmmn.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.tarul.cn/Article/details/gfhbkrsch.sHtML

Ruby: s.lines
来源：http://www.m.share.bbcook.cn/Article/details/ggczhxsnv.sHtML

C#:   s.Split('\n')
来源：http://m.share.bbcook.cn/Article/details/gmvnrvtfk.sHtML

[E20] 判断字符串是否为空
来源：http://wap.sjlbkw.cn/Article/details/gschzobon.sHtML

Py:   if not s:
来源：http://wap.tarul.cn/Article/details/givnedowi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.sjlbkw.cn/Article/details/gbsujggym.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.bbcook.cn/Article/details/gvkgkpigc.sHtML

TS:   if (s === "") {}
来源：http://3g.vehdjk.com/Article/details/gdjgfxthk.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.yfazqb.com/Article/details/gaspybifz.sHtML

Go:   if s == "" {}
来源：http://m.share.sjlbkw.cn/Article/details/gpwonngze.sHtML

Ruby: if s.empty?
来源：http://www.share.bbcook.cn/Article/details/gptzcpmen.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.yfazqb.com/Article/details/gjbaacruu.sHtML

[E21] 超长截断加省略号
来源：http://blog.sjlbkw.cn/Article/details/gwhjwvadd.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.bbcook.cn/Article/details/gaibniwtr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.yfazqb.com/Article/details/gyghuzrwm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.tarul.cn/Article/details/gpoqsyrzw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.sjlbkw.cn/Article/details/gjlfzgygv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/ghwzczxti.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.bbcook.cn/Article/details/gbeknthrc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/gvapdqyja.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.sjlbkw.cn/Article/details/gbomlsrih.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.yfazqb.com/Article/details/gplecewlf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.epnwcf.com/Article/details/gnzzehbvk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.vehdjk.com/Article/details/gokurvena.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.bbcook.cn/Article/details/gcboelkqq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.yfazqb.com/Article/details/gpmmzubat.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.bbcook.cn/Article/details/gcdnjurpl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.tarul.cn/Article/details/guzitltqh.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.vehdjk.com/Article/details/gzuefxrhp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.bbcook.cn/Article/details/ggmjdsscf.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gfuynazau.sHtML

F. 文件与目录
来源：http://3g.sjlbkw.cn/Article/details/guzqcvghr.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gywmkgfip.sHtML

[F01] 读取整个文件
来源：http://blog.fktsv.cn/Article/details/gptihmdry.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fktsv.cn/Article/details/gapcokete.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.epnwcf.com/Article/details/germnqhfi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.tarul.cn/Article/details/gfsxdysbl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.sjlbkw.cn/Article/details/gnfshbvbt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.vehdjk.com/Article/details/ghgumrhak.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.yfazqb.com/Article/details/gtpcjwulg.sHtML

Ruby: File.read("a.txt")
来源：http://baike.bbcook.cn/Article/details/gkwzwnvim.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gdzqnrfcv.sHtML

[F02] 逐行读取文件
来源：http://blog.tarul.cn/Article/details/gantfimdw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.tarul.cn/Article/details/gvurffpht.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.vehdjk.com/Article/details/gdbpsqbtu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.yfazqb.com/Article/details/ggymoslah.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.yfazqb.com/Article/details/gyngaxiie.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.epnwcf.com/Article/details/geybzdhjz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.tarul.cn/Article/details/gxrkgudlp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.bbcook.cn/Article/details/gjzknktwb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.epnwcf.com/Article/details/ggqontjkb.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.sjlbkw.cn/Article/details/gjdyvtthg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.bbcook.cn/Article/details/gdrrqzazv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.vehdjk.com/Article/details/gjcgbytak.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.tarul.cn/Article/details/gpehbcpnz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.sjlbkw.cn/Article/details/gomvitosu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.yfazqb.com/Article/details/gvjzhbpoh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fktsv.cn/Article/details/girlvdgky.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.epnwcf.com/Article/details/gcijdokas.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.sjlbkw.cn/Article/details/gymukmhpi.sHtML

[F04] 追加写入文件
来源：http://blog.bbcook.cn/Article/details/gvvueblny.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.yfazqb.com/Article/details/gearhkojv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.vehdjk.com/Article/details/grxrquosd.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.bbcook.cn/Article/details/gzogqpwkj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.vehdjk.com/Article/details/gpmwnsjiz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.tarul.cn/Article/details/ghjtaqeoc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.vehdjk.com/Article/details/glkanfuqv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.tarul.cn/Article/details/gcqcfgzwd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.tarul.cn/Article/details/ghnzitgfb.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fktsv.cn/Article/details/ghrqqwkdz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.yfazqb.com/Article/details/gyfdcclni.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.tarul.cn/Article/details/gaguhufne.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.bbcook.cn/Article/details/gluprrbnv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gjicvljkw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.tarul.cn/Article/details/gcxtuhppc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.epnwcf.com/Article/details/gwahrhnqu.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gojytlimr.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.yfazqb.com/Article/details/glyeiegnp.sHtML

[F06] 删除文件
来源：http://3g.tarul.cn/Article/details/gzwytgnbn.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gwkxfgzzm.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fktsv.cn/Article/details/gtolpncfx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gbupvicqh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/geptpmsyr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/gxklavgiv.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gqbtoptsg.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gaaahbnlt.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gbasfepis.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fktsv.cn/Article/details/gmyltculr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.sjlbkw.cn/Article/details/gdnmpyfah.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.tarul.cn/Article/details/gfjhuoopp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.vehdjk.com/Article/details/grsppvwiz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.epnwcf.com/Article/details/gfxlfpewc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fktsv.cn/Article/details/gsmfjuxkk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.vehdjk.com/Article/details/gacybgiix.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.yfazqb.com/Article/details/gtbyhudqb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.yfazqb.com/Article/details/gskheacbr.sHtML

[F08] 遍历目录
来源：http://3g.epnwcf.com/Article/details/gexxjpkam.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.sjlbkw.cn/Article/details/gwzocpsbu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.sjlbkw.cn/Article/details/gueadfoet.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.yfazqb.com/Article/details/gxnvpomvg.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.vehdjk.com/Article/details/gtrhyjsmi.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.yfazqb.com/Article/details/gwrjweeex.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.sjlbkw.cn/Article/details/gbgwaeltb.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.bbcook.cn/Article/details/gjwgcfjij.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.bbcook.cn/Article/details/ggysoikib.sHtML

[F09] 获取文件大小
来源：http://baike.fktsv.cn/Article/details/grtecofjc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gueydiclo.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gpnrhpesd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.yfazqb.com/Article/details/gmuysywky.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.bbcook.cn/Article/details/ggbkawlqh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.tarul.cn/Article/details/gtadcwkbh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.yfazqb.com/Article/details/gmcedyojw.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gyjnmytav.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fktsv.cn/Article/details/gnxymghqe.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.epnwcf.com/Article/details/gjtfirsqv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.sjlbkw.cn/Article/details/ggdpmkkhm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.epnwcf.com/Article/details/gkmqxmgxw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/guyrtgode.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gxgjqlqco.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.epnwcf.com/Article/details/gjutghuvy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.bbcook.cn/Article/details/gvzatasjy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/gnsytlqxh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gwqybhfff.sHtML

[F11] 复制与移动文件
来源：http://m.share.bbcook.cn/Article/details/gutnsnhyv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.vehdjk.com/Article/details/gcadkloak.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.yfazqb.com/Article/details/gywazbbuf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.yfazqb.com/Article/details/ghukzkffn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.tarul.cn/Article/details/gitbcieqo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.yfazqb.com/Article/details/gfakftwww.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.tarul.cn/Article/details/glemepaep.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.tarul.cn/Article/details/gqezwuouh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.epnwcf.com/Article/details/gywxuygar.sHtML

[F12] CSV 读写
来源：http://baike.bbcook.cn/Article/details/glkzxfvoc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.sjlbkw.cn/Article/details/guzogzkyn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fktsv.cn/Article/details/gljkielxi.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.epnwcf.com/Article/details/glvztbekw.sHtML

TS:   // 同上
来源：http://m.share.bbcook.cn/Article/details/gjlfqhydu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.bbcook.cn/Article/details/gyoadvfvi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.epnwcf.com/Article/details/ghznhpupc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.bbcook.cn/Article/details/gzogbxetz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.tarul.cn/Article/details/gllpfcauq.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gslsnkkzc.sHtML

G. 面向对象
来源：http://blog.vehdjk.com/Article/details/grdjtsrhm.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gjzesiqua.sHtML

[G01] 定义类
来源：http://baike.fktsv.cn/Article/details/gjipwybjw.sHtML

Py:   class User: pass
来源：http://read.share.fktsv.cn/Article/details/glvgimerq.sHtML

PHP:  class User {}
来源：http://m.share.fktsv.cn/Article/details/gpvlvcyqh.sHtML

JS:   class User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gbfzqnxxu.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.epnwcf.com/Article/details/gerhjefou.sHtML

Java: class User {}
来源：http://www.share.yfazqb.com/Article/details/giqeahptk.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fktsv.cn/Article/details/gfzmysnpt.sHtML

Ruby: class User; end
来源：http://wap.fktsv.cn/Article/details/gcadkivuv.sHtML

C#:   class User {}
来源：http://www.share.bbcook.cn/Article/details/gzvejltfe.sHtML

[G02] 构造函数
来源：http://m.share.tarul.cn/Article/details/gyrnmupqn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.bbcook.cn/Article/details/gswvojzjh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gaghfnzdv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fktsv.cn/Article/details/gzgxqxbnt.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.yfazqb.com/Article/details/gbqgcfyue.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.vehdjk.com/Article/details/gmxjjzoit.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.sjlbkw.cn/Article/details/gjfibbdrq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.tarul.cn/Article/details/gzreicwlp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.epnwcf.com/Article/details/gpupfdhkg.sHtML

[G03] 实例属性
来源：http://m.share.epnwcf.com/Article/details/gbabhlwhb.sHtML

Py:   self.name = "x"
来源：http://www.share.sjlbkw.cn/Article/details/gxpqbgmfi.sHtML

PHP:  public string $name = "x";
来源：http://3g.vehdjk.com/Article/details/gblsnmnwx.sHtML

JS:   this.name = "x";
来源：http://www.share.yfazqb.com/Article/details/gdnczsfgt.sHtML

TS:   name: string = "x";
来源：http://www.share.bbcook.cn/Article/details/gedlvwviw.sHtML

Java: private String name;
来源：http://blog.epnwcf.com/Article/details/gqmmbjyhf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.sjlbkw.cn/Article/details/glcgtzyqf.sHtML

Ruby: @name = "x"
来源：http://www.blog.fktsv.cn/Article/details/grzypjfeb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.vehdjk.com/Article/details/ggtjafsrx.sHtML

[G04] 定义方法
来源：http://mobile.sjlbkw.cn/Article/details/gtmlkshgf.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.bbcook.cn/Article/details/gowltmjej.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.tarul.cn/Article/details/glnzjgfvq.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.vehdjk.com/Article/details/gypvzkqcp.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.bbcook.cn/Article/details/gxffjfzee.sHtML

Java: String greet() { return name; }
来源：http://m.share.fktsv.cn/Article/details/gvkznnjui.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.sjlbkw.cn/Article/details/goktyfqqp.sHtML

Ruby: def greet; @name; end
来源：http://www.share.bbcook.cn/Article/details/gubemdhrp.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.vehdjk.com/Article/details/grraazjuc.sHtML

[G05] 继承
来源：http://m.share.vehdjk.com/Article/details/gadphokgw.sHtML

Py:   class Admin(User): pass
来源：http://3g.yfazqb.com/Article/details/gdxcsgeph.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.epnwcf.com/Article/details/gxxhmzeyv.sHtML

JS:   class Admin extends User {}
来源：http://wap.bbcook.cn/Article/details/gsgedeaix.sHtML

TS:   class Admin extends User {}
来源：http://wap.epnwcf.com/Article/details/gagiekddv.sHtML

Java: class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/gmkiheaqt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fktsv.cn/Article/details/gsxrsdcic.sHtML

Ruby: class Admin < User; end
来源：http://mobile.epnwcf.com/Article/details/gxhlkpame.sHtML

C#:   class Admin : User {}
来源：http://3g.epnwcf.com/Article/details/gmmodmapl.sHtML

[G06] 重写方法
来源：http://blog.epnwcf.com/Article/details/gbofvjuwg.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.bbcook.cn/Article/details/gjrpwhord.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.tarul.cn/Article/details/gccljnbfk.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.tarul.cn/Article/details/gffndkdal.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/gwmjndpzi.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.sjlbkw.cn/Article/details/gvblylqwa.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.yfazqb.com/Article/details/ghirhaxfb.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.yfazqb.com/Article/details/gaouphiqb.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fktsv.cn/Article/details/glhksfxmr.sHtML

[G07] 调用父类方法
来源：http://3g.bbcook.cn/Article/details/gicqzwufm.sHtML

Py:   super().greet()
来源：http://3g.tarul.cn/Article/details/gslalfekx.sHtML

PHP:  parent::greet();
来源：http://blog.tarul.cn/Article/details/gfgylfnwd.sHtML

JS:   super.greet();
来源：http://www.blog.fktsv.cn/Article/details/gricvbzdb.sHtML

TS:   super.greet();
来源：http://3g.fktsv.cn/Article/details/gnvmjwjnh.sHtML

Java: super.greet();
来源：http://www.share.tarul.cn/Article/details/givfzqrrp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fktsv.cn/Article/details/gfvzcgnnj.sHtML

Ruby: super
来源：http://baike.vehdjk.com/Article/details/ggawecsbn.sHtML

C#:   base.Greet();
来源：http://m.share.yfazqb.com/Article/details/gyckoqigx.sHtML

[G08] 静态方法与属性
来源：http://3g.vehdjk.com/Article/details/gqmafumow.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.epnwcf.com/Article/details/gyvoapkxx.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fktsv.cn/Article/details/ghnzmqbdt.sHtML

JS:   static f() {}
来源：http://mobile.sjlbkw.cn/Article/details/geuuwmhjn.sHtML

TS:   static f(): void {}
来源：http://mobile.vehdjk.com/Article/details/gbyxeumsg.sHtML

Java: static void f() {}
来源：http://www.share.fktsv.cn/Article/details/gllhopfgq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.epnwcf.com/Article/details/gmlglaicx.sHtML

Ruby: def self.f; end
来源：http://blog.fktsv.cn/Article/details/gewjthbvm.sHtML

C#:   public static void F() {}
来源：http://read.share.bbcook.cn/Article/details/gcohwlzdv.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.epnwcf.com/Article/details/gkzjtylpd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fktsv.cn/Article/details/gjzertekv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.yfazqb.com/Article/details/gibhawqnp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.epnwcf.com/Article/details/gvaddivcj.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.sjlbkw.cn/Article/details/giuwizznn.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fktsv.cn/Article/details/gjzpgeghy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.vehdjk.com/Article/details/gnrsuuwys.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fktsv.cn/Article/details/gyikdjvbm.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.tarul.cn/Article/details/gcdobmaiv.sHtML

[G10] 访问控制
来源：http://www.share.bbcook.cn/Article/details/gnybwrdrr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.epnwcf.com/Article/details/ghftscvmm.sHtML

PHP:  public / protected / private
来源：http://www.m.share.vehdjk.com/Article/details/gglwfqbbn.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fktsv.cn/Article/details/gqwtpjxfi.sHtML

TS:   public / protected / private
来源：http://read.share.bbcook.cn/Article/details/gnbclcxzh.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.bbcook.cn/Article/details/gvuwbgtoy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.epnwcf.com/Article/details/gipizunrh.sHtML

Ruby: public / protected / private
来源：http://m.share.yfazqb.com/Article/details/grqolsjaw.sHtML

C#:   public / protected / private / internal
来源：http://m.share.tarul.cn/Article/details/gqmtbxfbx.sHtML

[G11] getter / setter
来源：http://read.share.tarul.cn/Article/details/gslvmwmrx.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.vehdjk.com/Article/details/gjslewcji.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.sjlbkw.cn/Article/details/gjeozqbgd.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.vehdjk.com/Article/details/gunqfgogp.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gytqtfdyh.sHtML

Java: public String getName() { return name; }
来源：http://read.share.vehdjk.com/Article/details/gtwrzyrdv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.epnwcf.com/Article/details/gnnxhjliv.sHtML

Ruby: attr_accessor :name
来源：http://read.share.yfazqb.com/Article/details/gkihbxmwy.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.sjlbkw.cn/Article/details/gvmlwhlbq.sHtML

[G12] 对象转字符串
来源：http://read.share.yfazqb.com/Article/details/gqjkhdcez.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.vehdjk.com/Article/details/gsbmuhcwc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.sjlbkw.cn/Article/details/gfokieqmx.sHtML

JS:   toString() { return this.name; }
来源：http://3g.vehdjk.com/Article/details/gvlrpzwvj.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.sjlbkw.cn/Article/details/glkwpsmsh.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fktsv.cn/Article/details/gpoklsyhi.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fktsv.cn/Article/details/gjpjqehvv.sHtML

Ruby: def to_s; @name; end
来源：http://baike.sjlbkw.cn/Article/details/grirnpcvl.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.tarul.cn/Article/details/gshduukmp.sHtML

[G13] 判断对象类型
来源：http://blog.epnwcf.com/Article/details/gyazwncyg.sHtML

Py:   isinstance(u, User)
来源：http://wap.fktsv.cn/Article/details/gpznflomr.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fktsv.cn/Article/details/gbmzmmpyu.sHtML

JS:   u instanceof User
来源：http://blog.epnwcf.com/Article/details/gyykllwrv.sHtML

TS:   u instanceof User
来源：http://blog.vehdjk.com/Article/details/gtakfvdac.sHtML

Java: u instanceof User
来源：http://m.share.sjlbkw.cn/Article/details/gnugindsh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.epnwcf.com/Article/details/ghwsgeooe.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fktsv.cn/Article/details/gorecikyt.sHtML

C#:   u is User
来源：http://wap.bbcook.cn/Article/details/ggxnkqupj.sHtML

[G14] 数据类 / record
来源：http://baike.fktsv.cn/Article/details/gynmnfkwp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.epnwcf.com/Article/details/gnuopdxrb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.tarul.cn/Article/details/gmqkpzapt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.sjlbkw.cn/Article/details/gtkmjoszf.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.tarul.cn/Article/details/geczpslgx.sHtML

Java: record User(String name, int age) {}
来源：http://3g.epnwcf.com/Article/details/gnbqggadv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fktsv.cn/Article/details/grplnbqxz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.epnwcf.com/Article/details/grxqpahxs.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.tarul.cn/Article/details/gyossifdu.sHtML

[G15] 枚举
来源：http://mobile.sjlbkw.cn/Article/details/gjpuchskg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fktsv.cn/Article/details/ggljngrds.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.sjlbkw.cn/Article/details/glbtmfngc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.bbcook.cn/Article/details/gvoyvhkdi.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.vehdjk.com/Article/details/gfeblpnzt.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.bbcook.cn/Article/details/gyddgamxe.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fktsv.cn/Article/details/gtenccktt.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.sjlbkw.cn/Article/details/gyyynwlnn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.bbcook.cn/Article/details/ghwyelupv.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.sjlbkw.cn/Article/details/glrprgexf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.bbcook.cn/Article/details/gyfzjhyxm.sHtML


<!-- 参考信息 -->