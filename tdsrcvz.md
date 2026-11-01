代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.yfazqb.com/Article/details/ggfieefyb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.vehdjk.com/Article/details/gclyrokmo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.vehdjk.com/Article/details/gkcjvsicd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.sjlbkw.cn/Article/details/gimuyxuct.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.vehdjk.com/Article/details/giistlgex.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.epnwcf.com/Article/details/gaoedbfuo.sHtML

Ruby: s.capitalize
来源：http://www.blog.bbcook.cn/Article/details/gfusjvsjz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fktsv.cn/Article/details/gdjoweinh.sHtML

[E18] 模板占位符替换
来源：http://wap.bbcook.cn/Article/details/getvsrnaz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.tarul.cn/Article/details/gitznnbqy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.yfazqb.com/Article/details/gqrgetzqr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.vehdjk.com/Article/details/gvgtmxybb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.sjlbkw.cn/Article/details/gpeuzboyd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.tarul.cn/Article/details/gfodrilpa.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.sjlbkw.cn/Article/details/gqcdvwobo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.yfazqb.com/Article/details/ggzxlofgz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fktsv.cn/Article/details/gehoynddp.sHtML

[E19] 多行文本按行拆分
来源：http://3g.tarul.cn/Article/details/gszbtijou.sHtML

Py:   s.splitlines()
来源：http://mobile.epnwcf.com/Article/details/gvspmecuz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.vehdjk.com/Article/details/glgrxqxve.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.tarul.cn/Article/details/gfpqweggt.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fktsv.cn/Article/details/gavfeqojt.sHtML

Java: s.lines().toList()
来源：http://read.share.yfazqb.com/Article/details/gcyigxiti.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.vehdjk.com/Article/details/grwczokpg.sHtML

Ruby: s.lines
来源：http://mobile.epnwcf.com/Article/details/gwtegivot.sHtML

C#:   s.Split('\n')
来源：http://mobile.fktsv.cn/Article/details/gdffetwgk.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.sjlbkw.cn/Article/details/gtmkavxni.sHtML

Py:   if not s:
来源：http://www.blog.epnwcf.com/Article/details/gbafdzssq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.yfazqb.com/Article/details/gdwydackz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.vehdjk.com/Article/details/gnlqebuyq.sHtML

TS:   if (s === "") {}
来源：http://m.share.tarul.cn/Article/details/gqlpkhfaz.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.yfazqb.com/Article/details/gkmyeswpw.sHtML

Go:   if s == "" {}
来源：http://wap.vehdjk.com/Article/details/gbyneyetq.sHtML

Ruby: if s.empty?
来源：http://www.share.bbcook.cn/Article/details/gqiajrnua.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.vehdjk.com/Article/details/gsmxfgwdv.sHtML

[E21] 超长截断加省略号
来源：http://3g.vehdjk.com/Article/details/gssmobspi.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.yfazqb.com/Article/details/gsoexmdth.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.yfazqb.com/Article/details/gsxreltjq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fktsv.cn/Article/details/gakreftci.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fktsv.cn/Article/details/gweaprlkf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.epnwcf.com/Article/details/gmrhtxyik.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.bbcook.cn/Article/details/gsxiivbpl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.epnwcf.com/Article/details/gpjmwtwtg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.bbcook.cn/Article/details/gaideseub.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fktsv.cn/Article/details/gxxzjhxfk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fktsv.cn/Article/details/glsjdpfon.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.bbcook.cn/Article/details/gzcyeswhy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.tarul.cn/Article/details/guembddya.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.vehdjk.com/Article/details/gejosjupd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.epnwcf.com/Article/details/grrnarfjg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.epnwcf.com/Article/details/goxhluyja.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.yfazqb.com/Article/details/gjdfrgyyr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.sjlbkw.cn/Article/details/gldikjnzh.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gekvydeoa.sHtML

F. 文件与目录
来源：http://m.share.bbcook.cn/Article/details/gvfupjhae.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gpcczgpfo.sHtML

[F01] 读取整个文件
来源：http://www.share.sjlbkw.cn/Article/details/gtsgguzvn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.vehdjk.com/Article/details/gcoywgfkd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.vehdjk.com/Article/details/gsxomckgp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.epnwcf.com/Article/details/gxkcwcstz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fktsv.cn/Article/details/gnydtizrg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.bbcook.cn/Article/details/gcbidlcdv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.epnwcf.com/Article/details/gytqvvcpc.sHtML

Ruby: File.read("a.txt")
来源：http://3g.vehdjk.com/Article/details/gbrrkwisl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gkgbpanrc.sHtML

[F02] 逐行读取文件
来源：http://baike.yfazqb.com/Article/details/glxnedjax.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.yfazqb.com/Article/details/gnikxiuqc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.vehdjk.com/Article/details/giwxdvuhc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.epnwcf.com/Article/details/gppjldaee.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gatagwcwx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fktsv.cn/Article/details/gkgndasjj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxzpvgfxh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fktsv.cn/Article/details/gdocsxtek.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.epnwcf.com/Article/details/gxmmcdouv.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fktsv.cn/Article/details/gvwdwctdu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.epnwcf.com/Article/details/gvcqszppy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.fktsv.cn/Article/details/gksqdztqt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.bbcook.cn/Article/details/gacnljyea.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.yfazqb.com/Article/details/golufqned.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.bbcook.cn/Article/details/gpmgsjeui.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.sjlbkw.cn/Article/details/gorsrzkkk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fktsv.cn/Article/details/guaohqcmu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.tarul.cn/Article/details/gqjlscyqz.sHtML

[F04] 追加写入文件
来源：http://www.blog.yfazqb.com/Article/details/gmxkzxhde.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.bbcook.cn/Article/details/gsrlgpktt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.tarul.cn/Article/details/gbklsfixo.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.yfazqb.com/Article/details/gafpxqins.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.vehdjk.com/Article/details/gangnnjys.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.tarul.cn/Article/details/gdtatgayj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.vehdjk.com/Article/details/gcnsznvnw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.epnwcf.com/Article/details/gwwrkffma.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.tarul.cn/Article/details/grkjrjdbp.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.yfazqb.com/Article/details/gwilcsxmk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fktsv.cn/Article/details/glhnyrsdz.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.tarul.cn/Article/details/glydqsjpk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.vehdjk.com/Article/details/gewetohsk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gswlmsxqu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.epnwcf.com/Article/details/gzfcyfkjs.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.yfazqb.com/Article/details/glhafzjeq.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.bbcook.cn/Article/details/glyerhyub.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gfumeteak.sHtML

[F06] 删除文件
来源：http://m.share.tarul.cn/Article/details/gqebhkzmi.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gdqvetmzt.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gokosstum.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.tarul.cn/Article/details/gmqnkzwll.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gidxuewnq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/gjhqmwimh.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.vehdjk.com/Article/details/gmpvlplvg.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fktsv.cn/Article/details/ganowaxyv.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.tarul.cn/Article/details/gaorgnito.sHtML

[F07] 创建目录（含多级）
来源：http://blog.sjlbkw.cn/Article/details/gklnielmd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fktsv.cn/Article/details/ggsdmjtng.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.tarul.cn/Article/details/gvdixndzr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.yfazqb.com/Article/details/gvpsexcak.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.sjlbkw.cn/Article/details/gtiecrxqr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.epnwcf.com/Article/details/goelihusf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.bbcook.cn/Article/details/gesynkrob.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.tarul.cn/Article/details/gatvorhbe.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.epnwcf.com/Article/details/gpkzburly.sHtML

[F08] 遍历目录
来源：http://www.share.yfazqb.com/Article/details/gndsztqhr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.tarul.cn/Article/details/ghwhlkoty.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.yfazqb.com/Article/details/gfqnzyham.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.sjlbkw.cn/Article/details/gcepbaazs.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.bbcook.cn/Article/details/gnlrvqtry.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.sjlbkw.cn/Article/details/grbnrbrpr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.sjlbkw.cn/Article/details/gvieudjfo.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fktsv.cn/Article/details/gogbltsri.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.tarul.cn/Article/details/gumbintid.sHtML

[F09] 获取文件大小
来源：http://read.share.epnwcf.com/Article/details/gklgjryrg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gxrsmszzk.sHtML

PHP:  filesize("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gjhgswayc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.tarul.cn/Article/details/guqmrdhty.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.yfazqb.com/Article/details/gnnnsyvvw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.vehdjk.com/Article/details/gpoazxkqk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.yfazqb.com/Article/details/gixtsqatm.sHtML

Ruby: File.size("a.txt")
来源：http://wap.tarul.cn/Article/details/gnjxuwtnp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.yfazqb.com/Article/details/gccutaxwk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.epnwcf.com/Article/details/gwkixeavn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.tarul.cn/Article/details/guhjnlygu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.tarul.cn/Article/details/gamytpobg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gmomswehw.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gpzmxxivv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.bbcook.cn/Article/details/gtmtanubp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gslaichax.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/gzpejpyen.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gozpugyva.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.epnwcf.com/Article/details/gdadispkv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.tarul.cn/Article/details/gzpksggds.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.yfazqb.com/Article/details/gaixadhav.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.vehdjk.com/Article/details/gsnygicnh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.vehdjk.com/Article/details/gqdjalkgk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.yfazqb.com/Article/details/gikxvstdx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.tarul.cn/Article/details/gnnyncjsm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/gnvquvgam.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.bbcook.cn/Article/details/gvwuqddbo.sHtML

[F12] CSV 读写
来源：http://www.share.fktsv.cn/Article/details/gubizlgsf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.vehdjk.com/Article/details/grhaogjqb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.bbcook.cn/Article/details/gxzwbhior.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.yfazqb.com/Article/details/gfvhsruvi.sHtML

TS:   // 同上
来源：http://3g.bbcook.cn/Article/details/glnhmylkw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.yfazqb.com/Article/details/gfqifsndf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.epnwcf.com/Article/details/gabcdjbtm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.yfazqb.com/Article/details/gysdosdvu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.yfazqb.com/Article/details/gjtxjfucm.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gbpkfqmvi.sHtML

G. 面向对象
来源：http://www.blog.sjlbkw.cn/Article/details/gqxtrblpa.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gtdjjrhmr.sHtML

[G01] 定义类
来源：http://baike.tarul.cn/Article/details/gshfmfezl.sHtML

Py:   class User: pass
来源：http://baike.fktsv.cn/Article/details/gyvjpherw.sHtML

PHP:  class User {}
来源：http://blog.vehdjk.com/Article/details/gjpfaiici.sHtML

JS:   class User {}
来源：http://www.blog.yfazqb.com/Article/details/gzdsgzepe.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.bbcook.cn/Article/details/gkyqjzmzg.sHtML

Java: class User {}
来源：http://www.blog.vehdjk.com/Article/details/gjksrzyyl.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.tarul.cn/Article/details/gztvovlwn.sHtML

Ruby: class User; end
来源：http://3g.bbcook.cn/Article/details/gfpdcpdiw.sHtML

C#:   class User {}
来源：http://blog.bbcook.cn/Article/details/gspoprpmu.sHtML

[G02] 构造函数
来源：http://www.blog.tarul.cn/Article/details/gqfvpdjrp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.bbcook.cn/Article/details/gollwnkfo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gfvftapif.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.sjlbkw.cn/Article/details/gawuzvbmy.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.tarul.cn/Article/details/grrbatahy.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.yfazqb.com/Article/details/gnwdtwjua.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.vehdjk.com/Article/details/gkfsakhme.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.tarul.cn/Article/details/gedbclnze.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.epnwcf.com/Article/details/gnjqhqbkh.sHtML

[G03] 实例属性
来源：http://www.share.sjlbkw.cn/Article/details/ggybltwqp.sHtML

Py:   self.name = "x"
来源：http://wap.tarul.cn/Article/details/gsishgssl.sHtML

PHP:  public string $name = "x";
来源：http://mobile.yfazqb.com/Article/details/gxgbbkmqz.sHtML

JS:   this.name = "x";
来源：http://3g.vehdjk.com/Article/details/gadxcsagx.sHtML

TS:   name: string = "x";
来源：http://mobile.yfazqb.com/Article/details/gvmpcchpg.sHtML

Java: private String name;
来源：http://m.share.sjlbkw.cn/Article/details/gnhztqmsl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.sjlbkw.cn/Article/details/gayydoeer.sHtML

Ruby: @name = "x"
来源：http://blog.sjlbkw.cn/Article/details/gcdyvvmfc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.sjlbkw.cn/Article/details/gzyzqzxom.sHtML

[G04] 定义方法
来源：http://baike.fktsv.cn/Article/details/gmydiinlh.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.vehdjk.com/Article/details/gdyrlwxfg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.yfazqb.com/Article/details/gndycsvqw.sHtML

JS:   greet() { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/garnumipo.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fktsv.cn/Article/details/grueylmoh.sHtML

Java: String greet() { return name; }
来源：http://read.share.tarul.cn/Article/details/ghntoyjaw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.epnwcf.com/Article/details/ggvhppmkh.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.epnwcf.com/Article/details/gzwwtkxoy.sHtML

C#:   public string Greet() => Name;
来源：http://3g.tarul.cn/Article/details/gcbcjehrc.sHtML

[G05] 继承
来源：http://baike.bbcook.cn/Article/details/gzuvtwvmt.sHtML

Py:   class Admin(User): pass
来源：http://wap.epnwcf.com/Article/details/gosjpzuei.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.vehdjk.com/Article/details/gaajengxe.sHtML

JS:   class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/gchzoanyj.sHtML

TS:   class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/ghktwxvof.sHtML

Java: class Admin extends User {}
来源：http://mobile.tarul.cn/Article/details/gbpunknvc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fktsv.cn/Article/details/gfarsvpvk.sHtML

Ruby: class Admin < User; end
来源：http://read.share.tarul.cn/Article/details/gdkatpyzj.sHtML

C#:   class Admin : User {}
来源：http://3g.vehdjk.com/Article/details/gbeyiqtko.sHtML

[G06] 重写方法
来源：http://baike.bbcook.cn/Article/details/gugptodpz.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.epnwcf.com/Article/details/giqtoeycs.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gkxrhbjnu.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.yfazqb.com/Article/details/gpnudrvcx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gweiplgyc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fktsv.cn/Article/details/gveymccqi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.sjlbkw.cn/Article/details/ghohhyzie.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.epnwcf.com/Article/details/gqnilcigh.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.vehdjk.com/Article/details/gaamoxqia.sHtML

[G07] 调用父类方法
来源：http://read.share.epnwcf.com/Article/details/gullyqzjv.sHtML

Py:   super().greet()
来源：http://mobile.bbcook.cn/Article/details/gkqjalxyn.sHtML

PHP:  parent::greet();
来源：http://mobile.tarul.cn/Article/details/ghafddlmx.sHtML

JS:   super.greet();
来源：http://baike.epnwcf.com/Article/details/gzeikamxx.sHtML

TS:   super.greet();
来源：http://www.share.fktsv.cn/Article/details/gomhfpmel.sHtML

Java: super.greet();
来源：http://mobile.sjlbkw.cn/Article/details/gsnnmlptg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.epnwcf.com/Article/details/gnfssfttz.sHtML

Ruby: super
来源：http://baike.epnwcf.com/Article/details/ghfpkbfes.sHtML

C#:   base.Greet();
来源：http://m.share.tarul.cn/Article/details/gehhzjruh.sHtML

[G08] 静态方法与属性
来源：http://wap.vehdjk.com/Article/details/gcdmqdxra.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.sjlbkw.cn/Article/details/gulrgrumf.sHtML

PHP:  public static function f() {}
来源：http://read.share.fktsv.cn/Article/details/gxrpkwaih.sHtML

JS:   static f() {}
来源：http://wap.bbcook.cn/Article/details/gpivflhfa.sHtML

TS:   static f(): void {}
来源：http://www.m.share.tarul.cn/Article/details/gweesocfp.sHtML

Java: static void f() {}
来源：http://baike.sjlbkw.cn/Article/details/gotkqzdpk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.yfazqb.com/Article/details/gxqllxrny.sHtML

Ruby: def self.f; end
来源：http://3g.vehdjk.com/Article/details/guapqsxla.sHtML

C#:   public static void F() {}
来源：http://3g.sjlbkw.cn/Article/details/gffrlkaqv.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.bbcook.cn/Article/details/gjxkjvlau.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.yfazqb.com/Article/details/gxqsaizua.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.epnwcf.com/Article/details/gksugowva.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.sjlbkw.cn/Article/details/gfnjrweao.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.vehdjk.com/Article/details/ggugbngme.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.vehdjk.com/Article/details/gtlqcodqd.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.tarul.cn/Article/details/gmochhbwf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.bbcook.cn/Article/details/gytndoklf.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.bbcook.cn/Article/details/gzckgryjk.sHtML

[G10] 访问控制
来源：http://mobile.tarul.cn/Article/details/gvrbtqlkw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.tarul.cn/Article/details/gjaavvitr.sHtML

PHP:  public / protected / private
来源：http://mobile.sjlbkw.cn/Article/details/gypexbkte.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.sjlbkw.cn/Article/details/gepxcmcyu.sHtML

TS:   public / protected / private
来源：http://m.share.epnwcf.com/Article/details/gsvdodgua.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.bbcook.cn/Article/details/gabyxpdsh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.sjlbkw.cn/Article/details/gujzkuhvy.sHtML

Ruby: public / protected / private
来源：http://baike.fktsv.cn/Article/details/gllxwvodn.sHtML

C#:   public / protected / private / internal
来源：http://blog.fktsv.cn/Article/details/gedjxqldn.sHtML

[G11] getter / setter
来源：http://wap.bbcook.cn/Article/details/gghqidmgx.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fktsv.cn/Article/details/ggzuanohq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.sjlbkw.cn/Article/details/gbnayiqbj.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.tarul.cn/Article/details/guxmouiia.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.bbcook.cn/Article/details/gybtrjbut.sHtML

Java: public String getName() { return name; }
来源：http://m.share.tarul.cn/Article/details/giiwwrzey.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.epnwcf.com/Article/details/girqlwcva.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fktsv.cn/Article/details/gqetkiycx.sHtML

C#:   public string Name { get; set; }
来源：http://blog.epnwcf.com/Article/details/glfpdmzwi.sHtML

[G12] 对象转字符串
来源：http://blog.sjlbkw.cn/Article/details/gzbjqckut.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.sjlbkw.cn/Article/details/gvpxjersq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fktsv.cn/Article/details/ghtvbjqwa.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.yfazqb.com/Article/details/gnccpqtnp.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.bbcook.cn/Article/details/grcjquxrr.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.bbcook.cn/Article/details/gigvzvjcc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fktsv.cn/Article/details/gxprsaevw.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.sjlbkw.cn/Article/details/gwxacnuwe.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.tarul.cn/Article/details/gvfrwiuyv.sHtML

[G13] 判断对象类型
来源：http://read.share.vehdjk.com/Article/details/gnzwboxpb.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.bbcook.cn/Article/details/gwtpgrnis.sHtML

PHP:  $u instanceof User
来源：http://www.share.fktsv.cn/Article/details/giehvtztn.sHtML

JS:   u instanceof User
来源：http://www.share.yfazqb.com/Article/details/gnqpjygyg.sHtML

TS:   u instanceof User
来源：http://m.share.sjlbkw.cn/Article/details/giejneeuc.sHtML

Java: u instanceof User
来源：http://www.blog.tarul.cn/Article/details/ghioxpneb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fktsv.cn/Article/details/gvqohdsms.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.sjlbkw.cn/Article/details/gefjjbadu.sHtML

C#:   u is User
来源：http://mobile.bbcook.cn/Article/details/gewkkpnof.sHtML

[G14] 数据类 / record
来源：http://3g.tarul.cn/Article/details/ghsjmwzcj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.epnwcf.com/Article/details/gbntyattp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.epnwcf.com/Article/details/gzhwrmkgd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.epnwcf.com/Article/details/gjrqhmpxx.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.vehdjk.com/Article/details/gnkduzgae.sHtML

Java: record User(String name, int age) {}
来源：http://blog.sjlbkw.cn/Article/details/gvizcxwzx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.yfazqb.com/Article/details/ggalqyetu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.vehdjk.com/Article/details/grrdnmbnx.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.bbcook.cn/Article/details/gdranbfll.sHtML

[G15] 枚举
来源：http://mobile.vehdjk.com/Article/details/gxdxkshdp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.epnwcf.com/Article/details/ggblilaia.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.yfazqb.com/Article/details/gmcqrkwhs.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.sjlbkw.cn/Article/details/gerftkpht.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.epnwcf.com/Article/details/gvjahqgas.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.tarul.cn/Article/details/gbckoyluw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.bbcook.cn/Article/details/geptkcnyy.sHtML


<!-- 参考信息 -->