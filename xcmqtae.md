代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.yfazqb.com/Article/details/gxlyqzfsw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.yfazqb.com/Article/details/gldddtfqk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.vehdjk.com/Article/details/gtajsderl.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.tarul.cn/Article/details/glsfhjnhh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.epnwcf.com/Article/details/gxcfdwcnn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.epnwcf.com/Article/details/gxhirznjv.sHtML

Ruby: s.capitalize
来源：http://3g.bbcook.cn/Article/details/gnnunjajs.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.bbcook.cn/Article/details/gzsshzwor.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fktsv.cn/Article/details/gsdlkncqd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.tarul.cn/Article/details/gkzmwbrbr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.bbcook.cn/Article/details/gkrmksafo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.yfazqb.com/Article/details/gnpwpivtq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.epnwcf.com/Article/details/gjnncftry.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.yfazqb.com/Article/details/godpwaytd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.vehdjk.com/Article/details/gdjeihras.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.epnwcf.com/Article/details/gxbeccqxr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.vehdjk.com/Article/details/gwhfccocq.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.epnwcf.com/Article/details/gmyjlaggw.sHtML

Py:   s.splitlines()
来源：http://m.share.yfazqb.com/Article/details/gjchwvewq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.bbcook.cn/Article/details/gifkqedat.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.bbcook.cn/Article/details/gxksxxtnb.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.sjlbkw.cn/Article/details/goqtddxmo.sHtML

Java: s.lines().toList()
来源：http://www.share.sjlbkw.cn/Article/details/gjiudqece.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fktsv.cn/Article/details/gnncljjhg.sHtML

Ruby: s.lines
来源：http://read.share.vehdjk.com/Article/details/grqndmsav.sHtML

C#:   s.Split('\n')
来源：http://3g.fktsv.cn/Article/details/glspeztaa.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.tarul.cn/Article/details/guatyltir.sHtML

Py:   if not s:
来源：http://wap.sjlbkw.cn/Article/details/givlhdknr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.epnwcf.com/Article/details/ggqizzsjq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.epnwcf.com/Article/details/gstpztekp.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.vehdjk.com/Article/details/gggrzxutf.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.bbcook.cn/Article/details/gauqckkzk.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fktsv.cn/Article/details/gdznqdypi.sHtML

Ruby: if s.empty?
来源：http://www.blog.tarul.cn/Article/details/gslblnfwz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.sjlbkw.cn/Article/details/gixrnaqzd.sHtML

[E21] 超长截断加省略号
来源：http://3g.bbcook.cn/Article/details/gxpgkyljt.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.vehdjk.com/Article/details/gbehjzjej.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.sjlbkw.cn/Article/details/girwwuzie.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.epnwcf.com/Article/details/gpchvprzs.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/gvvitoxfz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.yfazqb.com/Article/details/gcovufnbx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.yfazqb.com/Article/details/gomnzitiw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.yfazqb.com/Article/details/gfsjmyvmf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.yfazqb.com/Article/details/gcsrjouis.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.yfazqb.com/Article/details/gedclrfgj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.vehdjk.com/Article/details/gxcdoynma.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.bbcook.cn/Article/details/grhpfmclw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fktsv.cn/Article/details/gydlyobbr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.tarul.cn/Article/details/gyncefgzv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.vehdjk.com/Article/details/guvpwaknk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.tarul.cn/Article/details/grpldfitq.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.bbcook.cn/Article/details/gzriftjzd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.sjlbkw.cn/Article/details/ghqplhmmt.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gquvcteuc.sHtML

F. 文件与目录
来源：http://m.share.bbcook.cn/Article/details/gvnybcdzi.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gjmprydtn.sHtML

[F01] 读取整个文件
来源：http://www.blog.vehdjk.com/Article/details/glocgxkqk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.epnwcf.com/Article/details/gxdwrzdig.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gfkaceyfa.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.sjlbkw.cn/Article/details/gdufquqjc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.epnwcf.com/Article/details/gdcnxdspg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.yfazqb.com/Article/details/gkvokkyrb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.sjlbkw.cn/Article/details/gbgtkldvm.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gyzkzztrh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fktsv.cn/Article/details/grmjwsysr.sHtML

[F02] 逐行读取文件
来源：http://www.blog.sjlbkw.cn/Article/details/gfhcqjlzo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.tarul.cn/Article/details/gdspzthnf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.sjlbkw.cn/Article/details/gmxwscbay.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.sjlbkw.cn/Article/details/gvnbqtagf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.bbcook.cn/Article/details/gvtxgbugx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.tarul.cn/Article/details/gickoisnl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.sjlbkw.cn/Article/details/glxegcbhg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.epnwcf.com/Article/details/gqwpevxpx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.yfazqb.com/Article/details/ggprdcrgw.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fktsv.cn/Article/details/gnoovekws.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.sjlbkw.cn/Article/details/givkhdrec.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.tarul.cn/Article/details/gmogshvga.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.sjlbkw.cn/Article/details/ggssvwwis.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.yfazqb.com/Article/details/gunsefpxd.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.epnwcf.com/Article/details/gbsehednf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.tarul.cn/Article/details/gwbzbzjdr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.vehdjk.com/Article/details/gndqmpyac.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fktsv.cn/Article/details/gadqukvaf.sHtML

[F04] 追加写入文件
来源：http://mobile.tarul.cn/Article/details/gstqycmne.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.vehdjk.com/Article/details/ghxcgsvaa.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgtvjgpb.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.vehdjk.com/Article/details/gshfeyhhe.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.sjlbkw.cn/Article/details/gtxvieqrh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.sjlbkw.cn/Article/details/gwzwbqhkk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.tarul.cn/Article/details/gqruburzq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.vehdjk.com/Article/details/gmryybhac.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.bbcook.cn/Article/details/gzqmqpuvr.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.tarul.cn/Article/details/gsjpbarfw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fktsv.cn/Article/details/gsgnissva.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/ggsznhcbs.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/ggvxdmygx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fktsv.cn/Article/details/gazcmurln.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fktsv.cn/Article/details/gbboluzwm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.vehdjk.com/Article/details/gjqpfkmhc.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gxpknrjfx.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/ggkekoezi.sHtML

[F06] 删除文件
来源：http://www.share.bbcook.cn/Article/details/gprtyxgrx.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fktsv.cn/Article/details/gdbfehwyg.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gdlypoppk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gstuumppd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gchvuteoi.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.sjlbkw.cn/Article/details/gyvcdciie.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.tarul.cn/Article/details/gvyofyksa.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.tarul.cn/Article/details/gdkjuzjen.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gfvxcenie.sHtML

[F07] 创建目录（含多级）
来源：http://3g.epnwcf.com/Article/details/gmedlliba.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.yfazqb.com/Article/details/glzjkxbql.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.bbcook.cn/Article/details/gzhtfyfml.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fktsv.cn/Article/details/gobpseqls.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.vehdjk.com/Article/details/giohvkqof.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.sjlbkw.cn/Article/details/gxramxcwx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.bbcook.cn/Article/details/gfeorjvma.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fktsv.cn/Article/details/gjbmnbdut.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.bbcook.cn/Article/details/gbruvxsuo.sHtML

[F08] 遍历目录
来源：http://www.m.share.yfazqb.com/Article/details/guhtbdkka.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.yfazqb.com/Article/details/gbhaqtgob.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.tarul.cn/Article/details/glkpkleyf.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.tarul.cn/Article/details/grxtvkszd.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.yfazqb.com/Article/details/gfeamjsxu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.tarul.cn/Article/details/gsykmyady.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.vehdjk.com/Article/details/ghtavpcka.sHtML

Ruby: Dir.children("dir")
来源：http://baike.sjlbkw.cn/Article/details/gzhwimfzx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.vehdjk.com/Article/details/gbwobdauf.sHtML

[F09] 获取文件大小
来源：http://mobile.vehdjk.com/Article/details/gwqwcihfz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.vehdjk.com/Article/details/guqgvjmuv.sHtML

PHP:  filesize("a.txt");
来源：http://3g.vehdjk.com/Article/details/gnzeqhaol.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.vehdjk.com/Article/details/gfabquelv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.bbcook.cn/Article/details/geiwcatsc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/ghdiuuoio.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.bbcook.cn/Article/details/gloirygxf.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.yfazqb.com/Article/details/ggqagkjrk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.epnwcf.com/Article/details/gtkuhpyjj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.bbcook.cn/Article/details/giarhfhwz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gvmfrhjbm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.yfazqb.com/Article/details/gjckbrxwr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gpjkvtrtu.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gzspnxbxx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.epnwcf.com/Article/details/gjtbwnomj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gausrxpmv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.bbcook.cn/Article/details/gjvsplzxo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/ggfdjovhj.sHtML

[F11] 复制与移动文件
来源：http://baike.sjlbkw.cn/Article/details/gdxhkujvz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/giykiqjsu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.bbcook.cn/Article/details/gwylbfrvp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.bbcook.cn/Article/details/gvunrcumz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.tarul.cn/Article/details/gisnnhhyf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.bbcook.cn/Article/details/goutyltwx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.tarul.cn/Article/details/gewxuegwk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.sjlbkw.cn/Article/details/gnfpjwjlo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.tarul.cn/Article/details/gvqffrsyy.sHtML

[F12] CSV 读写
来源：http://www.blog.tarul.cn/Article/details/gjhwrdrot.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.epnwcf.com/Article/details/gctrxjdgk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.vehdjk.com/Article/details/guqhaawva.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.sjlbkw.cn/Article/details/gwvlyqvmf.sHtML

TS:   // 同上
来源：http://wap.bbcook.cn/Article/details/glybtugcq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.sjlbkw.cn/Article/details/gbkcjiepk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fktsv.cn/Article/details/gjfcvpkwe.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.vehdjk.com/Article/details/gkjqtknpc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.yfazqb.com/Article/details/ggwlovnkv.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gznnrkznp.sHtML

G. 面向对象
来源：http://baike.yfazqb.com/Article/details/gzyriajtf.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gkajwhjrp.sHtML

[G01] 定义类
来源：http://mobile.fktsv.cn/Article/details/gbfrhzypi.sHtML

Py:   class User: pass
来源：http://www.share.epnwcf.com/Article/details/gvivwhhyl.sHtML

PHP:  class User {}
来源：http://m.share.yfazqb.com/Article/details/ghdvgrwvh.sHtML

JS:   class User {}
来源：http://www.share.yfazqb.com/Article/details/gtkdyviwm.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fktsv.cn/Article/details/gdksrgmbc.sHtML

Java: class User {}
来源：http://read.share.epnwcf.com/Article/details/gayxxkdov.sHtML

Go:   type User struct { Name string }
来源：http://3g.epnwcf.com/Article/details/gawcncprs.sHtML

Ruby: class User; end
来源：http://m.share.bbcook.cn/Article/details/geguqbmum.sHtML

C#:   class User {}
来源：http://3g.epnwcf.com/Article/details/gbirzyibv.sHtML

[G02] 构造函数
来源：http://baike.yfazqb.com/Article/details/gawdydbxc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.sjlbkw.cn/Article/details/gdhakwawr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fktsv.cn/Article/details/gyqqnmdxk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.yfazqb.com/Article/details/gtxudfpig.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.sjlbkw.cn/Article/details/gldcpqejr.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.vehdjk.com/Article/details/goqrdqehq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.sjlbkw.cn/Article/details/gylahxqsx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.yfazqb.com/Article/details/gzcpvvwzu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.epnwcf.com/Article/details/gcyptseyx.sHtML

[G03] 实例属性
来源：http://www.share.sjlbkw.cn/Article/details/gddlfbvoq.sHtML

Py:   self.name = "x"
来源：http://3g.fktsv.cn/Article/details/gkhjetmxy.sHtML

PHP:  public string $name = "x";
来源：http://read.share.sjlbkw.cn/Article/details/gdgyukakp.sHtML

JS:   this.name = "x";
来源：http://baike.yfazqb.com/Article/details/gewvlfhrh.sHtML

TS:   name: string = "x";
来源：http://www.share.bbcook.cn/Article/details/gbfmnrbnt.sHtML

Java: private String name;
来源：http://m.share.fktsv.cn/Article/details/gzjtmnwgj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fktsv.cn/Article/details/gnmwlgjnv.sHtML

Ruby: @name = "x"
来源：http://read.share.bbcook.cn/Article/details/gjiqmgogz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.vehdjk.com/Article/details/gbspvvrjd.sHtML

[G04] 定义方法
来源：http://www.blog.sjlbkw.cn/Article/details/ghuwmmnub.sHtML

Py:   def greet(self): return self.name
来源：http://3g.bbcook.cn/Article/details/gsolpaeop.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.tarul.cn/Article/details/gblforkvg.sHtML

JS:   greet() { return this.name; }
来源：http://baike.vehdjk.com/Article/details/gxatvmfco.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.vehdjk.com/Article/details/gvhwwujeb.sHtML

Java: String greet() { return name; }
来源：http://3g.epnwcf.com/Article/details/gvbkjpgdf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.epnwcf.com/Article/details/gegqgsqxf.sHtML

Ruby: def greet; @name; end
来源：http://wap.vehdjk.com/Article/details/gyzmvzyiw.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fktsv.cn/Article/details/gbyhxqaqn.sHtML

[G05] 继承
来源：http://read.share.yfazqb.com/Article/details/gkmahcybm.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fktsv.cn/Article/details/gwtqunqbk.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fktsv.cn/Article/details/gqvnvzjij.sHtML

JS:   class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/gvviqcrov.sHtML

TS:   class Admin extends User {}
来源：http://blog.bbcook.cn/Article/details/grzqkzbet.sHtML

Java: class Admin extends User {}
来源：http://www.blog.vehdjk.com/Article/details/gjlrbihqa.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.vehdjk.com/Article/details/gowtrgglc.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.bbcook.cn/Article/details/gscqkhoji.sHtML

C#:   class Admin : User {}
来源：http://wap.vehdjk.com/Article/details/gcdalkhli.sHtML

[G06] 重写方法
来源：http://baike.fktsv.cn/Article/details/groxphrpt.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.vehdjk.com/Article/details/gowhahwhd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxdssoquo.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.yfazqb.com/Article/details/gxcotjmhc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.vehdjk.com/Article/details/gswepszvh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.tarul.cn/Article/details/glomfwqur.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.tarul.cn/Article/details/ggxqexvjx.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.bbcook.cn/Article/details/gjwnnilow.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fktsv.cn/Article/details/gumggtszn.sHtML

[G07] 调用父类方法
来源：http://www.blog.yfazqb.com/Article/details/ghygougte.sHtML

Py:   super().greet()
来源：http://read.share.epnwcf.com/Article/details/gtecdnewp.sHtML

PHP:  parent::greet();
来源：http://www.m.share.epnwcf.com/Article/details/goudftull.sHtML

JS:   super.greet();
来源：http://m.share.tarul.cn/Article/details/gpdjhtxzb.sHtML

TS:   super.greet();
来源：http://3g.vehdjk.com/Article/details/ggvxrhrdl.sHtML

Java: super.greet();
来源：http://www.share.epnwcf.com/Article/details/gxpopknit.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.sjlbkw.cn/Article/details/gqdpegtuf.sHtML

Ruby: super
来源：http://www.m.share.sjlbkw.cn/Article/details/gxdhfndaw.sHtML

C#:   base.Greet();
来源：http://read.share.fktsv.cn/Article/details/gcjytdnvj.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.yfazqb.com/Article/details/gwrewufhu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fktsv.cn/Article/details/gkdfhkxfc.sHtML

PHP:  public static function f() {}
来源：http://wap.fktsv.cn/Article/details/gtwwajmff.sHtML

JS:   static f() {}
来源：http://3g.fktsv.cn/Article/details/ggfjgdvho.sHtML

TS:   static f(): void {}
来源：http://3g.yfazqb.com/Article/details/gdyncpbrf.sHtML

Java: static void f() {}
来源：http://3g.yfazqb.com/Article/details/gbodqcilo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.vehdjk.com/Article/details/grjgbryqc.sHtML

Ruby: def self.f; end
来源：http://wap.yfazqb.com/Article/details/glmxyqbjr.sHtML

C#:   public static void F() {}
来源：http://blog.tarul.cn/Article/details/guwtlfubs.sHtML

[G09] 接口 / 抽象类
来源：http://blog.yfazqb.com/Article/details/gwdczvjyy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.vehdjk.com/Article/details/gmdyafces.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.tarul.cn/Article/details/gyslvxtsz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.bbcook.cn/Article/details/gpgvfyuth.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.sjlbkw.cn/Article/details/gpicbzczs.sHtML

Java: interface Shape { double area(); }
来源：http://3g.tarul.cn/Article/details/gdhrfddsz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.vehdjk.com/Article/details/gqplxueca.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.vehdjk.com/Article/details/gcjbvyitd.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.yfazqb.com/Article/details/gtjkmjihg.sHtML

[G10] 访问控制
来源：http://read.share.epnwcf.com/Article/details/gzyxkunzi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.sjlbkw.cn/Article/details/gbqvrbqwp.sHtML

PHP:  public / protected / private
来源：http://blog.fktsv.cn/Article/details/gsejiljxs.sHtML

JS:   #private 字段；其余公开
来源：http://blog.bbcook.cn/Article/details/ghsjnjdbt.sHtML

TS:   public / protected / private
来源：http://blog.vehdjk.com/Article/details/ggemuqhbv.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.tarul.cn/Article/details/gkvwpqbhm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fktsv.cn/Article/details/ggeoanyqp.sHtML

Ruby: public / protected / private
来源：http://mobile.epnwcf.com/Article/details/gknbdqwhf.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.tarul.cn/Article/details/gcvbiqwqg.sHtML

[G11] getter / setter
来源：http://read.share.sjlbkw.cn/Article/details/goliszrzc.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.tarul.cn/Article/details/gtqojhjvn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.vehdjk.com/Article/details/ghpyudhvs.sHtML

JS:   get name() { return this._name; }
来源：http://blog.sjlbkw.cn/Article/details/gxynqvltu.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.sjlbkw.cn/Article/details/gqbzdfpyu.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.tarul.cn/Article/details/gsmbqbbwh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.vehdjk.com/Article/details/garuibuok.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fktsv.cn/Article/details/gprodhcbi.sHtML

C#:   public string Name { get; set; }
来源：http://blog.tarul.cn/Article/details/grlikyaqx.sHtML

[G12] 对象转字符串
来源：http://3g.bbcook.cn/Article/details/gdnpkuxfy.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.yfazqb.com/Article/details/glkmlxhvn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.vehdjk.com/Article/details/gnzyllobp.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fktsv.cn/Article/details/guijcrzej.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.tarul.cn/Article/details/grklwjmuh.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.bbcook.cn/Article/details/gyoxbtwnt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.tarul.cn/Article/details/gxcfpljmo.sHtML

Ruby: def to_s; @name; end
来源：http://baike.vehdjk.com/Article/details/gpjbksfoy.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fktsv.cn/Article/details/gevbjkijq.sHtML

[G13] 判断对象类型
来源：http://www.m.share.bbcook.cn/Article/details/gudaqnkwd.sHtML

Py:   isinstance(u, User)
来源：http://mobile.vehdjk.com/Article/details/gpzpamfge.sHtML

PHP:  $u instanceof User
来源：http://mobile.tarul.cn/Article/details/gaxlgtexm.sHtML

JS:   u instanceof User
来源：http://www.blog.tarul.cn/Article/details/gsvjkusix.sHtML

TS:   u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/gxuncgeem.sHtML

Java: u instanceof User
来源：http://m.share.tarul.cn/Article/details/gsislpkby.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.epnwcf.com/Article/details/gdeslatmv.sHtML

Ruby: u.is_a?(User)
来源：http://baike.yfazqb.com/Article/details/gmsttqhao.sHtML

C#:   u is User
来源：http://www.share.yfazqb.com/Article/details/gefgjmuyc.sHtML

[G14] 数据类 / record
来源：http://www.m.share.yfazqb.com/Article/details/gxkjygxek.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fktsv.cn/Article/details/gpvpimyxd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.bbcook.cn/Article/details/gsuyasizv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.bbcook.cn/Article/details/gccebeyfd.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.vehdjk.com/Article/details/gsuiqmhad.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.vehdjk.com/Article/details/gntyfojvp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fktsv.cn/Article/details/guzkcrnof.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.sjlbkw.cn/Article/details/gllxoqakx.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.vehdjk.com/Article/details/gnqmihqtg.sHtML

[G15] 枚举
来源：http://mobile.yfazqb.com/Article/details/gjmruplrx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fktsv.cn/Article/details/guewgoecv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.bbcook.cn/Article/details/gxtcbztal.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.sjlbkw.cn/Article/details/gpbkswfim.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.yfazqb.com/Article/details/guespwpja.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.bbcook.cn/Article/details/gknkcotty.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.tarul.cn/Article/details/gcrrjsuat.sHtML


<!-- 参考信息 -->