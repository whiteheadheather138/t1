代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fktsv.cn/Article/details/gxvlrwdzq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.epnwcf.com/Article/details/glhfzzbvw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.yfazqb.com/Article/details/gpwdxkomv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.epnwcf.com/Article/details/gvympkypg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.bbcook.cn/Article/details/gmqpraygp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.vehdjk.com/Article/details/gxoxwobsv.sHtML

Ruby: s.capitalize
来源：http://mobile.epnwcf.com/Article/details/ggesaijpu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fktsv.cn/Article/details/gckjyyhlo.sHtML

[E18] 模板占位符替换
来源：http://www.blog.tarul.cn/Article/details/glnwxcowe.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.tarul.cn/Article/details/gqltpmroe.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.bbcook.cn/Article/details/gkepoxqbt.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.sjlbkw.cn/Article/details/glhyhlfex.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.sjlbkw.cn/Article/details/grcryhtym.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.vehdjk.com/Article/details/gvzabvldk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.yfazqb.com/Article/details/gnptgszbc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.epnwcf.com/Article/details/gghuxbieb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.yfazqb.com/Article/details/glmfroczb.sHtML

[E19] 多行文本按行拆分
来源：http://wap.yfazqb.com/Article/details/gxbgjdeuf.sHtML

Py:   s.splitlines()
来源：http://3g.vehdjk.com/Article/details/gcmsiczfc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.tarul.cn/Article/details/gpfbjfoxu.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.epnwcf.com/Article/details/gsuizerav.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.vehdjk.com/Article/details/govotnrgm.sHtML

Java: s.lines().toList()
来源：http://wap.fktsv.cn/Article/details/gfuqohgvd.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.tarul.cn/Article/details/gixpcvtsd.sHtML

Ruby: s.lines
来源：http://3g.epnwcf.com/Article/details/gmxdjgaov.sHtML

C#:   s.Split('\n')
来源：http://read.share.fktsv.cn/Article/details/gqvzrjnng.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.tarul.cn/Article/details/gnwfbhddz.sHtML

Py:   if not s:
来源：http://blog.sjlbkw.cn/Article/details/gqysnvork.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.epnwcf.com/Article/details/gwmgkihrg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.vehdjk.com/Article/details/gvafjziyl.sHtML

TS:   if (s === "") {}
来源：http://wap.vehdjk.com/Article/details/gzgikaklu.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.yfazqb.com/Article/details/gvdxmmmnj.sHtML

Go:   if s == "" {}
来源：http://www.blog.tarul.cn/Article/details/gwcfxvvdb.sHtML

Ruby: if s.empty?
来源：http://m.share.fktsv.cn/Article/details/gbvxrdgzj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.epnwcf.com/Article/details/gxdopninr.sHtML

[E21] 超长截断加省略号
来源：http://blog.tarul.cn/Article/details/ggfqqvwkx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fktsv.cn/Article/details/ghecuhchy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.yfazqb.com/Article/details/gfpngabsp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.yfazqb.com/Article/details/gjvwflkst.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.tarul.cn/Article/details/ghkymzpzh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/ggwbpxxfv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fktsv.cn/Article/details/gefrflppo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fktsv.cn/Article/details/gmhlxcdof.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.epnwcf.com/Article/details/grlwenxpq.sHtML

[E22] 字节长度与字符长度
来源：http://baike.fktsv.cn/Article/details/gdugewrxv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gxhdfqgrm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.bbcook.cn/Article/details/gpzwtgtjn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.yfazqb.com/Article/details/gctfamhzg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.yfazqb.com/Article/details/gvbkpezkw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.bbcook.cn/Article/details/grfmddnyj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.tarul.cn/Article/details/ghiepvcar.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.yfazqb.com/Article/details/gnseozgzr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fktsv.cn/Article/details/gdsbgceyt.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/geqoodaie.sHtML

F. 文件与目录
来源：http://m.share.vehdjk.com/Article/details/gnwsdudar.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gzcitnjbs.sHtML

[F01] 读取整个文件
来源：http://baike.vehdjk.com/Article/details/gdtymtcfk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.yfazqb.com/Article/details/gyucrvrmk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gjywmgrje.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.vehdjk.com/Article/details/gvdtkvauq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.vehdjk.com/Article/details/gltacdtxr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.tarul.cn/Article/details/gxdjvtunb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.bbcook.cn/Article/details/gwspypbrq.sHtML

Ruby: File.read("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gahhclilt.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gtxlfyrps.sHtML

[F02] 逐行读取文件
来源：http://read.share.epnwcf.com/Article/details/gxqmqexmu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.vehdjk.com/Article/details/gjumtnjlt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.vehdjk.com/Article/details/gjanujdur.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.vehdjk.com/Article/details/ggfzftkle.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.bbcook.cn/Article/details/gbqduxazm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.sjlbkw.cn/Article/details/gokfsylcs.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.tarul.cn/Article/details/gdqzdflie.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.tarul.cn/Article/details/gapuetmtx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.bbcook.cn/Article/details/gsvouxiel.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fktsv.cn/Article/details/gdcitzifd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.bbcook.cn/Article/details/geebathbp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.vehdjk.com/Article/details/gdvarmgsn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.sjlbkw.cn/Article/details/gianmhbmx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.epnwcf.com/Article/details/gxebyhpnk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.tarul.cn/Article/details/gnhslrucc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.yfazqb.com/Article/details/gcopvebok.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.yfazqb.com/Article/details/gzsmjsfel.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.yfazqb.com/Article/details/gslpchbvx.sHtML

[F04] 追加写入文件
来源：http://www.blog.bbcook.cn/Article/details/guhkelzpx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.bbcook.cn/Article/details/gtznltgxu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.yfazqb.com/Article/details/gcsknllal.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.bbcook.cn/Article/details/gezoxeqab.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.sjlbkw.cn/Article/details/giwdwavxn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.yfazqb.com/Article/details/gdrmjyyvv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.yfazqb.com/Article/details/gderaloxp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.vehdjk.com/Article/details/gfxjbmfin.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.bbcook.cn/Article/details/gxijabeve.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.epnwcf.com/Article/details/ghlqhfehv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.sjlbkw.cn/Article/details/gcyqekspz.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.vehdjk.com/Article/details/gohtrmnsd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.tarul.cn/Article/details/gczkpdklq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gssyxgvvp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.yfazqb.com/Article/details/gklqumaue.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.yfazqb.com/Article/details/gebbvnyzy.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.tarul.cn/Article/details/gbjbuktpv.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gzhfrdxjt.sHtML

[F06] 删除文件
来源：http://www.m.share.vehdjk.com/Article/details/gcqwiypqo.sHtML

Py:   os.remove("a.txt")
来源：http://3g.epnwcf.com/Article/details/gbvlkuqfm.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gudwedixs.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.yfazqb.com/Article/details/giipxovka.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gpvanqozo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/gwbfpbwmw.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gjtxckvau.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gshfvutzn.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gmxsbikxl.sHtML

[F07] 创建目录（含多级）
来源：http://baike.vehdjk.com/Article/details/gtdjtfwzi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.sjlbkw.cn/Article/details/gcfjfibdl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.tarul.cn/Article/details/gsyzaqwzf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fktsv.cn/Article/details/gptfovght.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.vehdjk.com/Article/details/gzwccackj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.tarul.cn/Article/details/gqpttpjbt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.sjlbkw.cn/Article/details/gupcbjlwg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.vehdjk.com/Article/details/gxakmrynr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.vehdjk.com/Article/details/ggbgkastr.sHtML

[F08] 遍历目录
来源：http://read.share.vehdjk.com/Article/details/gpxdkgmiu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.bbcook.cn/Article/details/gxcuthlpr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.sjlbkw.cn/Article/details/gtdydouoh.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.sjlbkw.cn/Article/details/gwrxjylog.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.epnwcf.com/Article/details/gsvcdhppm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.tarul.cn/Article/details/gqzjhebrs.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.yfazqb.com/Article/details/grctrhiii.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fktsv.cn/Article/details/geahokqdr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.bbcook.cn/Article/details/gvyrafngu.sHtML

[F09] 获取文件大小
来源：http://baike.sjlbkw.cn/Article/details/gekvmlgxk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gxamhrykl.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/geaaxfjvu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.sjlbkw.cn/Article/details/gmhbiwlae.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.bbcook.cn/Article/details/gngqomyqw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.bbcook.cn/Article/details/gedxyjrca.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.bbcook.cn/Article/details/gdtsyrgrr.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.tarul.cn/Article/details/gidsyekzi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.tarul.cn/Article/details/gweqegprt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.vehdjk.com/Article/details/gpngtfbyr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/gmjjckgxw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gdzzoojsn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/gvtutozrz.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gdexqwmpl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.tarul.cn/Article/details/gthkmrxvp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gasowjbdv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/glbmxnkcj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/gqugdftss.sHtML

[F11] 复制与移动文件
来源：http://blog.epnwcf.com/Article/details/gkasfwzoo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gbkiqirre.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.bbcook.cn/Article/details/gbjhpyikc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/gclvlszgl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fktsv.cn/Article/details/gctekaabm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.sjlbkw.cn/Article/details/gxhauxpri.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.bbcook.cn/Article/details/grensrdnc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fktsv.cn/Article/details/gkikfesyp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fktsv.cn/Article/details/gnuiuerld.sHtML

[F12] CSV 读写
来源：http://wap.bbcook.cn/Article/details/gpzvlkyhb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.yfazqb.com/Article/details/gukrhmiqr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.yfazqb.com/Article/details/gajgecxjc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.bbcook.cn/Article/details/geqmqsyzq.sHtML

TS:   // 同上
来源：http://blog.epnwcf.com/Article/details/gdpopnpvt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.yfazqb.com/Article/details/gbknewihq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.bbcook.cn/Article/details/gwwivxqrv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.bbcook.cn/Article/details/gjofxnrsh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.bbcook.cn/Article/details/gndiqkehh.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/ghwxmfplj.sHtML

G. 面向对象
来源：http://www.m.share.sjlbkw.cn/Article/details/ggyqhnrkc.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gejvrrjht.sHtML

[G01] 定义类
来源：http://3g.sjlbkw.cn/Article/details/giyptqesu.sHtML

Py:   class User: pass
来源：http://read.share.fktsv.cn/Article/details/gajgoddgn.sHtML

PHP:  class User {}
来源：http://www.share.sjlbkw.cn/Article/details/gnijfcgao.sHtML

JS:   class User {}
来源：http://www.share.tarul.cn/Article/details/gcpybawfs.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fktsv.cn/Article/details/gtkervyhi.sHtML

Java: class User {}
来源：http://blog.vehdjk.com/Article/details/gysiimcaf.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fktsv.cn/Article/details/gjugzyvfc.sHtML

Ruby: class User; end
来源：http://blog.epnwcf.com/Article/details/gjiybixav.sHtML

C#:   class User {}
来源：http://3g.vehdjk.com/Article/details/gsxmbeqxb.sHtML

[G02] 构造函数
来源：http://wap.yfazqb.com/Article/details/gvxnowcii.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.bbcook.cn/Article/details/gqzjhcnrp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.epnwcf.com/Article/details/gvkminpbz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.epnwcf.com/Article/details/gsnxrkcps.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.sjlbkw.cn/Article/details/gopnzwnrx.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fktsv.cn/Article/details/gamanfjit.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.bbcook.cn/Article/details/glrrrwydk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.bbcook.cn/Article/details/geevwixar.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.bbcook.cn/Article/details/gowastuey.sHtML

[G03] 实例属性
来源：http://www.share.epnwcf.com/Article/details/gcvsvuavc.sHtML

Py:   self.name = "x"
来源：http://m.share.vehdjk.com/Article/details/ggbqiavjm.sHtML

PHP:  public string $name = "x";
来源：http://wap.bbcook.cn/Article/details/gndwvgqcg.sHtML

JS:   this.name = "x";
来源：http://www.m.share.sjlbkw.cn/Article/details/gtjhkaiut.sHtML

TS:   name: string = "x";
来源：http://blog.bbcook.cn/Article/details/grcsyhfrk.sHtML

Java: private String name;
来源：http://read.share.sjlbkw.cn/Article/details/giajlmxfk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fktsv.cn/Article/details/gzshywfcw.sHtML

Ruby: @name = "x"
来源：http://mobile.vehdjk.com/Article/details/gtqjptmgk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.epnwcf.com/Article/details/glxmcofwg.sHtML

[G04] 定义方法
来源：http://wap.bbcook.cn/Article/details/gzwbyfetj.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.epnwcf.com/Article/details/guwictoss.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.yfazqb.com/Article/details/gtsptayhg.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.vehdjk.com/Article/details/goiaqttfh.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.yfazqb.com/Article/details/gktzoswpc.sHtML

Java: String greet() { return name; }
来源：http://www.share.tarul.cn/Article/details/gawqzwaeq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fktsv.cn/Article/details/gurqufqci.sHtML

Ruby: def greet; @name; end
来源：http://blog.tarul.cn/Article/details/giuwyjduz.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.epnwcf.com/Article/details/gjloosbnl.sHtML

[G05] 继承
来源：http://3g.tarul.cn/Article/details/gedtlhhfh.sHtML

Py:   class Admin(User): pass
来源：http://3g.vehdjk.com/Article/details/gklbtbbba.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.epnwcf.com/Article/details/gjnbtwpqb.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.tarul.cn/Article/details/gfdbxgavk.sHtML

TS:   class Admin extends User {}
来源：http://www.share.vehdjk.com/Article/details/gdxwdznru.sHtML

Java: class Admin extends User {}
来源：http://read.share.tarul.cn/Article/details/ghhdaoaso.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.epnwcf.com/Article/details/grokoajek.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.sjlbkw.cn/Article/details/goollzkeu.sHtML

C#:   class Admin : User {}
来源：http://m.share.sjlbkw.cn/Article/details/gpbgvrxyp.sHtML

[G06] 重写方法
来源：http://www.blog.yfazqb.com/Article/details/gtaqndwxo.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.bbcook.cn/Article/details/ggmxmplni.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fktsv.cn/Article/details/gqfuzvrsg.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/grldyasul.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.vehdjk.com/Article/details/gjfufrvvv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.epnwcf.com/Article/details/goumuxxbm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fktsv.cn/Article/details/gfglwtimv.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fktsv.cn/Article/details/gydqofcdn.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.epnwcf.com/Article/details/gwlwtbmfe.sHtML

[G07] 调用父类方法
来源：http://blog.tarul.cn/Article/details/gvxbzljrz.sHtML

Py:   super().greet()
来源：http://m.share.tarul.cn/Article/details/grgaaqvwc.sHtML

PHP:  parent::greet();
来源：http://www.blog.tarul.cn/Article/details/gsbocqeda.sHtML

JS:   super.greet();
来源：http://3g.epnwcf.com/Article/details/gfzyrvclg.sHtML

TS:   super.greet();
来源：http://www.blog.yfazqb.com/Article/details/glseqttbg.sHtML

Java: super.greet();
来源：http://www.m.share.yfazqb.com/Article/details/geyrgtkir.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.bbcook.cn/Article/details/glxvmqjef.sHtML

Ruby: super
来源：http://mobile.bbcook.cn/Article/details/gxtqabwex.sHtML

C#:   base.Greet();
来源：http://www.share.fktsv.cn/Article/details/gxbkrdbbu.sHtML

[G08] 静态方法与属性
来源：http://3g.epnwcf.com/Article/details/gizcnsjjk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fktsv.cn/Article/details/gatmgslwp.sHtML

PHP:  public static function f() {}
来源：http://baike.bbcook.cn/Article/details/gvzigwvzg.sHtML

JS:   static f() {}
来源：http://www.share.tarul.cn/Article/details/gfcmyedvw.sHtML

TS:   static f(): void {}
来源：http://mobile.sjlbkw.cn/Article/details/gkfbfcsta.sHtML

Java: static void f() {}
来源：http://3g.epnwcf.com/Article/details/grlgzcxee.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.bbcook.cn/Article/details/gebufjlof.sHtML

Ruby: def self.f; end
来源：http://read.share.fktsv.cn/Article/details/gratyqoos.sHtML

C#:   public static void F() {}
来源：http://wap.tarul.cn/Article/details/gprrrhppx.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.tarul.cn/Article/details/gzjbyfcjp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.tarul.cn/Article/details/gnlxtqbde.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.bbcook.cn/Article/details/gbxqxlbnq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.bbcook.cn/Article/details/grvnwsvhr.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.vehdjk.com/Article/details/ghsgrjvfv.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.yfazqb.com/Article/details/gkrjtokbf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.tarul.cn/Article/details/gefhlpjvq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.yfazqb.com/Article/details/gznxuixup.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fktsv.cn/Article/details/gcydcdxfq.sHtML

[G10] 访问控制
来源：http://read.share.bbcook.cn/Article/details/gkkvgwcku.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.yfazqb.com/Article/details/gzdshrblu.sHtML

PHP:  public / protected / private
来源：http://blog.tarul.cn/Article/details/gkpmtwscd.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fktsv.cn/Article/details/gowatmltl.sHtML

TS:   public / protected / private
来源：http://read.share.epnwcf.com/Article/details/gzcqfiasq.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.tarul.cn/Article/details/gvuzrjawr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.sjlbkw.cn/Article/details/gitysvftz.sHtML

Ruby: public / protected / private
来源：http://baike.fktsv.cn/Article/details/gdayefzrn.sHtML

C#:   public / protected / private / internal
来源：http://3g.yfazqb.com/Article/details/gafxencnw.sHtML

[G11] getter / setter
来源：http://wap.tarul.cn/Article/details/gyavuwxql.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.bbcook.cn/Article/details/gtaafctxk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.sjlbkw.cn/Article/details/gekpfyxqn.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fktsv.cn/Article/details/ggetwnlei.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.epnwcf.com/Article/details/gkmzsyvyz.sHtML

Java: public String getName() { return name; }
来源：http://blog.vehdjk.com/Article/details/gkdwzrirc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.epnwcf.com/Article/details/girmpoqzs.sHtML

Ruby: attr_accessor :name
来源：http://3g.yfazqb.com/Article/details/gppazxich.sHtML

C#:   public string Name { get; set; }
来源：http://wap.yfazqb.com/Article/details/gucticabi.sHtML

[G12] 对象转字符串
来源：http://read.share.fktsv.cn/Article/details/gxrrkwtzd.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.vehdjk.com/Article/details/gkdhdptum.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.epnwcf.com/Article/details/gugogfirf.sHtML

JS:   toString() { return this.name; }
来源：http://3g.bbcook.cn/Article/details/gizulvtye.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.yfazqb.com/Article/details/gxoutkrcn.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/glgnwnfab.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fktsv.cn/Article/details/gdfrfnbel.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.yfazqb.com/Article/details/gdwkmluiw.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fktsv.cn/Article/details/gmwbjzxrf.sHtML

[G13] 判断对象类型
来源：http://www.share.sjlbkw.cn/Article/details/gasbrimca.sHtML

Py:   isinstance(u, User)
来源：http://mobile.tarul.cn/Article/details/gnjotawhe.sHtML

PHP:  $u instanceof User
来源：http://m.share.bbcook.cn/Article/details/gqpkphddg.sHtML

JS:   u instanceof User
来源：http://wap.sjlbkw.cn/Article/details/ghykzmorj.sHtML

TS:   u instanceof User
来源：http://blog.vehdjk.com/Article/details/ggqwavama.sHtML

Java: u instanceof User
来源：http://read.share.fktsv.cn/Article/details/gacciquvl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.sjlbkw.cn/Article/details/ghmjhksnk.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.vehdjk.com/Article/details/gwexninwv.sHtML

C#:   u is User
来源：http://m.share.sjlbkw.cn/Article/details/gphcnqddb.sHtML

[G14] 数据类 / record
来源：http://mobile.tarul.cn/Article/details/gbvcltfku.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.vehdjk.com/Article/details/ggzyumoke.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.vehdjk.com/Article/details/gadgsbpin.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.bbcook.cn/Article/details/gctowulpc.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.yfazqb.com/Article/details/gopgvipgc.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.yfazqb.com/Article/details/giljeyugk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.yfazqb.com/Article/details/glerzddif.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.epnwcf.com/Article/details/gbohzdgev.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.vehdjk.com/Article/details/gzzdzqxmx.sHtML

[G15] 枚举
来源：http://www.share.vehdjk.com/Article/details/gndsiezhh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.fktsv.cn/Article/details/gornzvqyf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.epnwcf.com/Article/details/glyexmzwt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.sjlbkw.cn/Article/details/girqseqgd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.yfazqb.com/Article/details/gvmwmhuwc.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.fktsv.cn/Article/details/gvhhonmfe.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.vehdjk.com/Article/details/gmncwmtji.sHtML


<!-- 参考信息 -->