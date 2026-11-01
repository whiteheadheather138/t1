代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fktsv.cn/Article/details/gjwsvspdf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.epnwcf.com/Article/details/gjfucriwg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.vehdjk.com/Article/details/gsqmpjjry.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.tarul.cn/Article/details/gpuzezqvj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.tarul.cn/Article/details/gkjmkfdzj.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.tarul.cn/Article/details/gtiqxncud.sHtML

Py:   s.splitlines()
来源：http://read.share.epnwcf.com/Article/details/gzwuuivnw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.epnwcf.com/Article/details/gseoobqbe.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.yfazqb.com/Article/details/gijcavntw.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.sjlbkw.cn/Article/details/gmokunnog.sHtML

Java: s.lines().toList()
来源：http://3g.sjlbkw.cn/Article/details/gggtmhjpx.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.bbcook.cn/Article/details/grrofgjcz.sHtML

Ruby: s.lines
来源：http://m.share.bbcook.cn/Article/details/goliekfnf.sHtML

C#:   s.Split('\n')
来源：http://baike.fktsv.cn/Article/details/gfmhvrhhv.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.epnwcf.com/Article/details/gpyihjvnk.sHtML

Py:   if not s:
来源：http://mobile.epnwcf.com/Article/details/gtclqhdcy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.sjlbkw.cn/Article/details/gropjsjeu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.sjlbkw.cn/Article/details/gdeqsxmvs.sHtML

TS:   if (s === "") {}
来源：http://m.share.fktsv.cn/Article/details/gjyhxdign.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.epnwcf.com/Article/details/grfbevush.sHtML

Go:   if s == "" {}
来源：http://read.share.vehdjk.com/Article/details/guliuswrq.sHtML

Ruby: if s.empty?
来源：http://m.share.yfazqb.com/Article/details/gurgxmofv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.bbcook.cn/Article/details/gwyruxigr.sHtML

[E21] 超长截断加省略号
来源：http://m.share.yfazqb.com/Article/details/ganpjrndg.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.bbcook.cn/Article/details/gldcknboy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.sjlbkw.cn/Article/details/gdcycnhrb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.sjlbkw.cn/Article/details/grhvlepnw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.yfazqb.com/Article/details/gycrpcdep.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.sjlbkw.cn/Article/details/glpfxfyic.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.tarul.cn/Article/details/gjrhibooe.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/gyondvpjc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.epnwcf.com/Article/details/ggjdwuuqd.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.epnwcf.com/Article/details/geoyhhgch.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fktsv.cn/Article/details/gzoqlohzt.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.tarul.cn/Article/details/gynnbqnmu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.epnwcf.com/Article/details/gctovzxef.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.tarul.cn/Article/details/ggcnrwvtm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.vehdjk.com/Article/details/gifhynrif.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.vehdjk.com/Article/details/gfmkhbkza.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.yfazqb.com/Article/details/gdmqcbawn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.sjlbkw.cn/Article/details/gnbbkpmoq.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/ggiosxigk.sHtML

F. 文件与目录
来源：http://baike.bbcook.cn/Article/details/gjiuubwcu.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gabifevng.sHtML

[F01] 读取整个文件
来源：http://www.m.share.epnwcf.com/Article/details/gwnctjkhr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.sjlbkw.cn/Article/details/grlxzvhrq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.tarul.cn/Article/details/gghnhgnko.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.epnwcf.com/Article/details/gokpyapvg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fktsv.cn/Article/details/gtabupzph.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.vehdjk.com/Article/details/gpqbeczdj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.yfazqb.com/Article/details/gawpxvhcg.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gvlidmokk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gxxqglaay.sHtML

[F02] 逐行读取文件
来源：http://www.share.vehdjk.com/Article/details/gebmzpucw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.yfazqb.com/Article/details/gjkeagdes.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.epnwcf.com/Article/details/gcmqrpaqh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fktsv.cn/Article/details/gvjgvoior.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.bbcook.cn/Article/details/gterclbmw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.vehdjk.com/Article/details/gpralmqai.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.sjlbkw.cn/Article/details/ghmtxgrrg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.sjlbkw.cn/Article/details/gvdwaufwe.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.vehdjk.com/Article/details/gbglwmjdr.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.bbcook.cn/Article/details/gdrhdigra.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjspoesop.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.vehdjk.com/Article/details/gyqsoxzeb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.sjlbkw.cn/Article/details/gopexkcyo.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.bbcook.cn/Article/details/gvgbzorjo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.sjlbkw.cn/Article/details/gannjkzvz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fktsv.cn/Article/details/gjweaexei.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fktsv.cn/Article/details/gztprzkst.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.bbcook.cn/Article/details/gkfjicbao.sHtML

[F04] 追加写入文件
来源：http://m.share.vehdjk.com/Article/details/ggtsyhhgq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fktsv.cn/Article/details/glrenkpms.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.sjlbkw.cn/Article/details/gargrzlop.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.sjlbkw.cn/Article/details/gdjadxwar.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.vehdjk.com/Article/details/gjyqzyvxw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqqkviqjg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.tarul.cn/Article/details/gapcbyrzf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.bbcook.cn/Article/details/gjwvbcwhs.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fktsv.cn/Article/details/gzcrimwst.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.bbcook.cn/Article/details/giwbjszys.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.bbcook.cn/Article/details/goarzbpuo.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gsoxmywol.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.yfazqb.com/Article/details/ghcijkfbf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fktsv.cn/Article/details/grnwyinpx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.epnwcf.com/Article/details/ggjxgrnjn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.vehdjk.com/Article/details/glgwherpr.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gpqealltl.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.vehdjk.com/Article/details/ghymqhwag.sHtML

[F06] 删除文件
来源：http://3g.fktsv.cn/Article/details/gwkekwypf.sHtML

Py:   os.remove("a.txt")
来源：http://wap.epnwcf.com/Article/details/gepedzmau.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gzbictoja.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/ghwfgrqkw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gsphwxdbp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.vehdjk.com/Article/details/givuhpkmf.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gpenewmbw.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gjzcwklvw.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.tarul.cn/Article/details/goipvyalg.sHtML

[F07] 创建目录（含多级）
来源：http://3g.yfazqb.com/Article/details/grgxfvjgh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fktsv.cn/Article/details/ggvbdzcuv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.epnwcf.com/Article/details/gkfpepysu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.yfazqb.com/Article/details/gomsmhuol.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.epnwcf.com/Article/details/gjdufyqid.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.sjlbkw.cn/Article/details/gwpzdnuvr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.tarul.cn/Article/details/ghdqziame.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.bbcook.cn/Article/details/gkwvrkogd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.sjlbkw.cn/Article/details/gfyoqoant.sHtML

[F08] 遍历目录
来源：http://baike.tarul.cn/Article/details/gonzemepw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.epnwcf.com/Article/details/gjkjoupbv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.tarul.cn/Article/details/gihpkuuqg.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.sjlbkw.cn/Article/details/gqyoffsdf.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.yfazqb.com/Article/details/ggmftbrhg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.bbcook.cn/Article/details/gmaqnrguj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.sjlbkw.cn/Article/details/gcihwyygi.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.sjlbkw.cn/Article/details/gjkiywvqr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.vehdjk.com/Article/details/ggzdujahq.sHtML

[F09] 获取文件大小
来源：http://baike.vehdjk.com/Article/details/gugmdvnxh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gsrvlpwpc.sHtML

PHP:  filesize("a.txt");
来源：http://3g.vehdjk.com/Article/details/gzywspyeq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.tarul.cn/Article/details/gawfbrpeb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fktsv.cn/Article/details/gfvbqpagx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.tarul.cn/Article/details/gzgdhimwe.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.yfazqb.com/Article/details/gutymzkki.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gmzydtsdh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.tarul.cn/Article/details/gqqwhoirc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.bbcook.cn/Article/details/gadancwbx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.vehdjk.com/Article/details/gkscfnmtb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.vehdjk.com/Article/details/gsxtdwwek.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gsxwhzwyg.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fktsv.cn/Article/details/gopeajewb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.sjlbkw.cn/Article/details/gqsqauhvj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.vehdjk.com/Article/details/gspznlvnf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gcogdeapl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/gegqyxbjp.sHtML

[F11] 复制与移动文件
来源：http://read.share.fktsv.cn/Article/details/gtfhxcazp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.vehdjk.com/Article/details/gdjqgpuri.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.yfazqb.com/Article/details/gsiwcymod.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.bbcook.cn/Article/details/gccybmifs.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fktsv.cn/Article/details/gcxmkbsij.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fktsv.cn/Article/details/gxknxnukz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.tarul.cn/Article/details/gcufgekqt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fktsv.cn/Article/details/gmthxshdi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.epnwcf.com/Article/details/gyxdzcjax.sHtML

[F12] CSV 读写
来源：http://mobile.yfazqb.com/Article/details/gmtnmkxgc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fktsv.cn/Article/details/gofbglodl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.sjlbkw.cn/Article/details/gvvspeivn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.sjlbkw.cn/Article/details/gucyvlerz.sHtML

TS:   // 同上
来源：http://3g.tarul.cn/Article/details/gvqoylrvm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.bbcook.cn/Article/details/gfppelxdu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.sjlbkw.cn/Article/details/gurmzulvj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.sjlbkw.cn/Article/details/gohkmykzy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fktsv.cn/Article/details/ggdkcyzqa.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gzskcuqbd.sHtML

G. 面向对象
来源：http://read.share.epnwcf.com/Article/details/gzdyydkix.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/geutjhtrn.sHtML

[G01] 定义类
来源：http://read.share.vehdjk.com/Article/details/gjchrwmro.sHtML

Py:   class User: pass
来源：http://blog.fktsv.cn/Article/details/gitahlomm.sHtML

PHP:  class User {}
来源：http://3g.bbcook.cn/Article/details/gfjoauern.sHtML

JS:   class User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gscwnzcwp.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.epnwcf.com/Article/details/gswohatjb.sHtML

Java: class User {}
来源：http://blog.yfazqb.com/Article/details/gyrfnlkav.sHtML

Go:   type User struct { Name string }
来源：http://read.share.epnwcf.com/Article/details/gonazkdpu.sHtML

Ruby: class User; end
来源：http://www.m.share.bbcook.cn/Article/details/gtmoxwtci.sHtML

C#:   class User {}
来源：http://m.share.tarul.cn/Article/details/gruloptet.sHtML

[G02] 构造函数
来源：http://wap.bbcook.cn/Article/details/gxsuvpfjo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.epnwcf.com/Article/details/greixxgqt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.vehdjk.com/Article/details/gkpcekzwh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.sjlbkw.cn/Article/details/ghmlabswa.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.tarul.cn/Article/details/giqwdbvrb.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fktsv.cn/Article/details/gvugoascm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.bbcook.cn/Article/details/gohzggqsl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.vehdjk.com/Article/details/gihqsoujh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.vehdjk.com/Article/details/gfbuxetbf.sHtML

[G03] 实例属性
来源：http://wap.epnwcf.com/Article/details/gapwhgkyh.sHtML

Py:   self.name = "x"
来源：http://m.share.bbcook.cn/Article/details/gccayaasj.sHtML

PHP:  public string $name = "x";
来源：http://3g.epnwcf.com/Article/details/gtgazgjge.sHtML

JS:   this.name = "x";
来源：http://mobile.vehdjk.com/Article/details/gigxuzkxn.sHtML

TS:   name: string = "x";
来源：http://wap.bbcook.cn/Article/details/gxjpvvhyg.sHtML

Java: private String name;
来源：http://baike.fktsv.cn/Article/details/gvzbgmvie.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.tarul.cn/Article/details/gssrmqdhy.sHtML

Ruby: @name = "x"
来源：http://wap.sjlbkw.cn/Article/details/gfcrhlqvo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fktsv.cn/Article/details/gyxbqsgru.sHtML

[G04] 定义方法
来源：http://m.share.fktsv.cn/Article/details/gfkyhtvrk.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.tarul.cn/Article/details/gyxclmmvc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.yfazqb.com/Article/details/gtdfqvibz.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.sjlbkw.cn/Article/details/gqfmidzqb.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.epnwcf.com/Article/details/gybywxaoi.sHtML

Java: String greet() { return name; }
来源：http://3g.fktsv.cn/Article/details/gztdjjhqi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.sjlbkw.cn/Article/details/gicvfhqvx.sHtML

Ruby: def greet; @name; end
来源：http://mobile.sjlbkw.cn/Article/details/gwllmfsrz.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fktsv.cn/Article/details/girkiavcs.sHtML

[G05] 继承
来源：http://read.share.yfazqb.com/Article/details/gsbdicycd.sHtML

Py:   class Admin(User): pass
来源：http://read.share.yfazqb.com/Article/details/giqrcrsuw.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.yfazqb.com/Article/details/gcpffzdii.sHtML

JS:   class Admin extends User {}
来源：http://read.share.sjlbkw.cn/Article/details/grwvkfasw.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gnqtspxdt.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fktsv.cn/Article/details/gdslrzgsg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.bbcook.cn/Article/details/gfnapkpdv.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.sjlbkw.cn/Article/details/gpvqjtclw.sHtML

C#:   class Admin : User {}
来源：http://blog.fktsv.cn/Article/details/gxwrebyxn.sHtML

[G06] 重写方法
来源：http://blog.yfazqb.com/Article/details/gaojtgdfd.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.bbcook.cn/Article/details/grxewwlxt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.yfazqb.com/Article/details/gpcflnjoc.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.epnwcf.com/Article/details/gikgwqrkg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.vehdjk.com/Article/details/gqcxjwrvn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.tarul.cn/Article/details/gvbqgrqhu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.sjlbkw.cn/Article/details/gmdacanis.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.epnwcf.com/Article/details/gowhwjyjn.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.sjlbkw.cn/Article/details/gbfezwuae.sHtML

[G07] 调用父类方法
来源：http://www.share.yfazqb.com/Article/details/goxvqswei.sHtML

Py:   super().greet()
来源：http://mobile.bbcook.cn/Article/details/gnphieoua.sHtML

PHP:  parent::greet();
来源：http://www.share.epnwcf.com/Article/details/ghvmasdjl.sHtML

JS:   super.greet();
来源：http://blog.yfazqb.com/Article/details/gnvnwvgrv.sHtML

TS:   super.greet();
来源：http://m.share.sjlbkw.cn/Article/details/ggyanvdre.sHtML

Java: super.greet();
来源：http://m.share.yfazqb.com/Article/details/gszealzpg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.bbcook.cn/Article/details/ghjcweauo.sHtML

Ruby: super
来源：http://www.m.share.sjlbkw.cn/Article/details/gpbxocvui.sHtML

C#:   base.Greet();
来源：http://mobile.sjlbkw.cn/Article/details/gzspxxrhc.sHtML

[G08] 静态方法与属性
来源：http://read.share.sjlbkw.cn/Article/details/ggpivdvlk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.yfazqb.com/Article/details/gzduyqtrt.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gumdjekbp.sHtML

JS:   static f() {}
来源：http://www.blog.vehdjk.com/Article/details/gclfgikmr.sHtML

TS:   static f(): void {}
来源：http://mobile.bbcook.cn/Article/details/gtqpnfakt.sHtML

Java: static void f() {}
来源：http://m.share.vehdjk.com/Article/details/glppbjcbj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.vehdjk.com/Article/details/geovboqhe.sHtML

Ruby: def self.f; end
来源：http://mobile.yfazqb.com/Article/details/grlpawzws.sHtML

C#:   public static void F() {}
来源：http://read.share.epnwcf.com/Article/details/ghgquyryj.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.epnwcf.com/Article/details/gnlvwmkxw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.tarul.cn/Article/details/gobagvegb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.vehdjk.com/Article/details/gzzituima.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.yfazqb.com/Article/details/gxdcamqgf.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.vehdjk.com/Article/details/gybpaqokf.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fktsv.cn/Article/details/gnglahcgp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.bbcook.cn/Article/details/gmbxvcymz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.vehdjk.com/Article/details/gbyjffpti.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.tarul.cn/Article/details/gngblhluk.sHtML

[G10] 访问控制
来源：http://www.share.tarul.cn/Article/details/genkawkaq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.yfazqb.com/Article/details/gawfijodq.sHtML

PHP:  public / protected / private
来源：http://read.share.yfazqb.com/Article/details/godhermmy.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fktsv.cn/Article/details/ggvptcupa.sHtML

TS:   public / protected / private
来源：http://www.share.bbcook.cn/Article/details/gzdmujjic.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.vehdjk.com/Article/details/gjrmyappj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fktsv.cn/Article/details/gtgvjpnmw.sHtML

Ruby: public / protected / private
来源：http://www.share.tarul.cn/Article/details/gjkxyxkfv.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.epnwcf.com/Article/details/gwdridgdb.sHtML

[G11] getter / setter
来源：http://www.blog.yfazqb.com/Article/details/gvcmmioie.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.bbcook.cn/Article/details/gyujwgzhc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.sjlbkw.cn/Article/details/gipdvaabq.sHtML

JS:   get name() { return this._name; }
来源：http://wap.tarul.cn/Article/details/gfdsbafmb.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.yfazqb.com/Article/details/ghzjxcjax.sHtML

Java: public String getName() { return name; }
来源：http://read.share.epnwcf.com/Article/details/gkvpvxdmw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.vehdjk.com/Article/details/golkangue.sHtML

Ruby: attr_accessor :name
来源：http://read.share.epnwcf.com/Article/details/gocwdiwvc.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.tarul.cn/Article/details/gjcckfatn.sHtML

[G12] 对象转字符串
来源：http://3g.fktsv.cn/Article/details/ggvnaxkli.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.epnwcf.com/Article/details/grpmslvgv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fktsv.cn/Article/details/glhtwxpzq.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.yfazqb.com/Article/details/gdiqjaixy.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.vehdjk.com/Article/details/gaxhphgqs.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/gjnugmlom.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fktsv.cn/Article/details/gluthqjmx.sHtML

Ruby: def to_s; @name; end
来源：http://blog.vehdjk.com/Article/details/gcgkngdfp.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.yfazqb.com/Article/details/gqdismmom.sHtML

[G13] 判断对象类型
来源：http://m.share.sjlbkw.cn/Article/details/gbxcptzdd.sHtML

Py:   isinstance(u, User)
来源：http://blog.epnwcf.com/Article/details/gfctgdqjw.sHtML

PHP:  $u instanceof User
来源：http://mobile.fktsv.cn/Article/details/gwbvwmudq.sHtML

JS:   u instanceof User
来源：http://read.share.sjlbkw.cn/Article/details/gizoltmvd.sHtML

TS:   u instanceof User
来源：http://3g.vehdjk.com/Article/details/gpsnaxipr.sHtML

Java: u instanceof User
来源：http://wap.sjlbkw.cn/Article/details/givclvixq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.sjlbkw.cn/Article/details/gvzrakdiz.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.sjlbkw.cn/Article/details/gkamewbzr.sHtML

C#:   u is User
来源：http://wap.tarul.cn/Article/details/gojvpgosw.sHtML

[G14] 数据类 / record
来源：http://www.blog.vehdjk.com/Article/details/giyqcfxur.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.sjlbkw.cn/Article/details/gdpdxztja.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.vehdjk.com/Article/details/guancrmxd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.yfazqb.com/Article/details/giqtfjwvn.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.epnwcf.com/Article/details/gtfyaywue.sHtML

Java: record User(String name, int age) {}
来源：http://3g.vehdjk.com/Article/details/giuvtpfzi.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.vehdjk.com/Article/details/gpltpburh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.epnwcf.com/Article/details/gxtduogqz.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.bbcook.cn/Article/details/gabxnoupl.sHtML

[G15] 枚举
来源：http://www.blog.vehdjk.com/Article/details/gfbikdwhs.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.sjlbkw.cn/Article/details/glnhszgui.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.tarul.cn/Article/details/gisgoaqsy.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.bbcook.cn/Article/details/gjmumkdsu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.bbcook.cn/Article/details/gzbnfnukm.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.bbcook.cn/Article/details/gsqxetlkn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.tarul.cn/Article/details/gmrghrdbw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.tarul.cn/Article/details/gkwuugnsd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.bbcook.cn/Article/details/gtvokotup.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fktsv.cn/Article/details/gtmwkrymz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.epnwcf.com/Article/details/gfqfkklhi.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkdpufjdz.sHtML

JS:   Object.entries(obj)
来源：http://blog.fktsv.cn/Article/details/gwlckzpph.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fktsv.cn/Article/details/grwmimwiu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.tarul.cn/Article/details/gjlodszba.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.bbcook.cn/Article/details/gbqqzhhmw.sHtML

Ruby: obj.instance_variables
来源：http://blog.sjlbkw.cn/Article/details/getbmxaqo.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.epnwcf.com/Article/details/gblrltuey.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gqrknjhcy.sHtML


<!-- 参考信息 -->