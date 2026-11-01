代发 wailian999

PHP:  number_format(1234567);
来源：http://baike.sjlbkw.cn/Article/details/gkysbyxof.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.epnwcf.com/Article/details/gcjhyzqwr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fktsv.cn/Article/details/gneldebxw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.sjlbkw.cn/Article/details/gnauizlst.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.sjlbkw.cn/Article/details/gvfemspoi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.yfazqb.com/Article/details/gdrmmnxim.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.sjlbkw.cn/Article/details/geiovhqbh.sHtML

[E17] 首字母大写
来源：http://read.share.fktsv.cn/Article/details/gfbpifevs.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.tarul.cn/Article/details/gvixxqhuv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.vehdjk.com/Article/details/gaawgvohw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.sjlbkw.cn/Article/details/gapedfbap.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.tarul.cn/Article/details/goyooiykv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.sjlbkw.cn/Article/details/gplgbwzwg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.bbcook.cn/Article/details/gknrbjjgv.sHtML

Ruby: s.capitalize
来源：http://www.blog.bbcook.cn/Article/details/gnvqydmgc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.vehdjk.com/Article/details/gnvvyymhb.sHtML

[E18] 模板占位符替换
来源：http://baike.sjlbkw.cn/Article/details/gxhwkjcai.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.bbcook.cn/Article/details/gyfikesov.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.yfazqb.com/Article/details/ghlwxkfzt.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.tarul.cn/Article/details/gwgnzhzoq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fktsv.cn/Article/details/gaxevvcze.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.vehdjk.com/Article/details/goonjzwfq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.tarul.cn/Article/details/ggslrbnas.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.sjlbkw.cn/Article/details/gzeffdoar.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.bbcook.cn/Article/details/gklrcckas.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.epnwcf.com/Article/details/gauhodrqh.sHtML

Py:   s.splitlines()
来源：http://wap.vehdjk.com/Article/details/grpydihmz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gmudbpocn.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.bbcook.cn/Article/details/gdlgpwxyv.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fktsv.cn/Article/details/gdjdewmdj.sHtML

Java: s.lines().toList()
来源：http://3g.yfazqb.com/Article/details/gzxiwekiq.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fktsv.cn/Article/details/gvfbcbcei.sHtML

Ruby: s.lines
来源：http://www.share.vehdjk.com/Article/details/gflxngzet.sHtML

C#:   s.Split('\n')
来源：http://wap.tarul.cn/Article/details/gnghkgqqc.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fktsv.cn/Article/details/gqfrduzqt.sHtML

Py:   if not s:
来源：http://www.blog.sjlbkw.cn/Article/details/gfjcteigu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.sjlbkw.cn/Article/details/gkqxsqlwd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.epnwcf.com/Article/details/gbcfkwddm.sHtML

TS:   if (s === "") {}
来源：http://www.share.tarul.cn/Article/details/gabjkztgz.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.epnwcf.com/Article/details/gunlikoip.sHtML

Go:   if s == "" {}
来源：http://read.share.vehdjk.com/Article/details/gmjelwcqw.sHtML

Ruby: if s.empty?
来源：http://read.share.bbcook.cn/Article/details/gtffjyrvt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fktsv.cn/Article/details/gronkiehz.sHtML

[E21] 超长截断加省略号
来源：http://www.share.bbcook.cn/Article/details/gfhpdzskk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fktsv.cn/Article/details/gdjmegzda.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.vehdjk.com/Article/details/gjyeienqk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.tarul.cn/Article/details/gbcimhwaq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.sjlbkw.cn/Article/details/guxrrejkw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fktsv.cn/Article/details/ghfdhtcqx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.yfazqb.com/Article/details/gzexklsgw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/gyornzgji.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fktsv.cn/Article/details/gpbpjnnjl.sHtML

[E22] 字节长度与字符长度
来源：http://wap.vehdjk.com/Article/details/godnlbwvs.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.tarul.cn/Article/details/gibahahhv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.yfazqb.com/Article/details/gurhvcwvl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.vehdjk.com/Article/details/gauptfohw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.epnwcf.com/Article/details/grulmdxmh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.yfazqb.com/Article/details/gjebhnqiq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fktsv.cn/Article/details/goswboixj.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.sjlbkw.cn/Article/details/gtumepeae.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.sjlbkw.cn/Article/details/gyuxmsgwr.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gstttkqjp.sHtML

F. 文件与目录
来源：http://m.share.fktsv.cn/Article/details/gkcwauqeu.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/giepyrssb.sHtML

[F01] 读取整个文件
来源：http://www.m.share.yfazqb.com/Article/details/grnfutaop.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.epnwcf.com/Article/details/gzzhfaxwh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.bbcook.cn/Article/details/gjubvblad.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.yfazqb.com/Article/details/gabnozumj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.vehdjk.com/Article/details/gjfecztat.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.sjlbkw.cn/Article/details/gntwkfzku.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.yfazqb.com/Article/details/gheveroad.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/grgqlnoxk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.epnwcf.com/Article/details/geqybvule.sHtML

[F02] 逐行读取文件
来源：http://3g.sjlbkw.cn/Article/details/gowhpjmvt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.yfazqb.com/Article/details/gylhdkqoj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.vehdjk.com/Article/details/gbxkhaqan.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.bbcook.cn/Article/details/gzmxlpgti.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.vehdjk.com/Article/details/gyvvqoiyx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fktsv.cn/Article/details/gqtsxfhbg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.bbcook.cn/Article/details/gkbdhbnnv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.vehdjk.com/Article/details/ggtkxxcad.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.bbcook.cn/Article/details/gnblfeshe.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fktsv.cn/Article/details/gxvsguwbt.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.yfazqb.com/Article/details/gcgcaxidz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.epnwcf.com/Article/details/gtkrieppc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.yfazqb.com/Article/details/gboxwfrph.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.bbcook.cn/Article/details/gejglkbns.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.bbcook.cn/Article/details/gqtkjoqep.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.sjlbkw.cn/Article/details/gpyohvssz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.bbcook.cn/Article/details/gujvezurj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.sjlbkw.cn/Article/details/gwiwtoqsh.sHtML

[F04] 追加写入文件
来源：http://www.blog.vehdjk.com/Article/details/gkfsugodv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.yfazqb.com/Article/details/gislxmngh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.tarul.cn/Article/details/gewtsouoi.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.yfazqb.com/Article/details/giknwmtez.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fktsv.cn/Article/details/gzaxrsskz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.sjlbkw.cn/Article/details/gqtextrzt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.vehdjk.com/Article/details/gtsapwbaw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.yfazqb.com/Article/details/glojwjiqb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.sjlbkw.cn/Article/details/gvhkutqtv.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.yfazqb.com/Article/details/gvjzamqob.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.yfazqb.com/Article/details/glqfwavdp.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fktsv.cn/Article/details/guthigffv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.vehdjk.com/Article/details/ggubwzrgj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gywadrbdz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/ggcgdmfgf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.sjlbkw.cn/Article/details/gvsqtrfbm.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gtscsdudr.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.bbcook.cn/Article/details/gdzvhyenn.sHtML

[F06] 删除文件
来源：http://mobile.epnwcf.com/Article/details/grbrmqnoe.sHtML

Py:   os.remove("a.txt")
来源：http://blog.vehdjk.com/Article/details/gevvqsvgu.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gizscbirb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gyynmyqvg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gvmlbrmav.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/gbmxoveuj.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gaiftgfdq.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.tarul.cn/Article/details/gommsoxkc.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.yfazqb.com/Article/details/ggsivkmvt.sHtML

[F07] 创建目录（含多级）
来源：http://blog.yfazqb.com/Article/details/gjaenthhg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.bbcook.cn/Article/details/gmtmirbyp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.vehdjk.com/Article/details/gujfwsiqb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fktsv.cn/Article/details/gpuarcsfo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.tarul.cn/Article/details/gtmjjcsln.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fktsv.cn/Article/details/gmvjyoavs.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.bbcook.cn/Article/details/gdoheaqco.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fktsv.cn/Article/details/gijnwjjfg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fktsv.cn/Article/details/gialilsyr.sHtML

[F08] 遍历目录
来源：http://blog.bbcook.cn/Article/details/gogcxtrba.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fktsv.cn/Article/details/gdaqlhuil.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fktsv.cn/Article/details/gahydnqld.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.vehdjk.com/Article/details/gvhdvwoij.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.sjlbkw.cn/Article/details/gedqhepjd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.tarul.cn/Article/details/gafcssjln.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fktsv.cn/Article/details/gondupwkq.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.vehdjk.com/Article/details/ghcabeqqo.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.yfazqb.com/Article/details/ghmslrfdu.sHtML

[F09] 获取文件大小
来源：http://www.share.yfazqb.com/Article/details/ggjyzabaq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.vehdjk.com/Article/details/gexcmcqwp.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gkbsqwini.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.vehdjk.com/Article/details/gizffsiee.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.vehdjk.com/Article/details/gssydujyg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.tarul.cn/Article/details/ggabsakqi.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.yfazqb.com/Article/details/gdopachmt.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gheehulqc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.epnwcf.com/Article/details/gslsntvyo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.yfazqb.com/Article/details/gtxbfnmdd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gjeljhrvy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fktsv.cn/Article/details/geghixzth.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/gjtvovuan.sHtML

TS:   path.extname("a.txt")
来源：http://baike.bbcook.cn/Article/details/gekgtazpk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.epnwcf.com/Article/details/gkwivbnqv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/gitvwvrfm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/goaxvvzpo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.yfazqb.com/Article/details/gpayfdtin.sHtML

[F11] 复制与移动文件
来源：http://3g.vehdjk.com/Article/details/glftuainb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/gyngtvuog.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.yfazqb.com/Article/details/gqpajjzqs.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.epnwcf.com/Article/details/gsfepaydi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.yfazqb.com/Article/details/gplhmjsaw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.vehdjk.com/Article/details/gonyumats.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.bbcook.cn/Article/details/glzmfuapl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gqudksxaa.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.epnwcf.com/Article/details/gkarfddna.sHtML

[F12] CSV 读写
来源：http://www.m.share.fktsv.cn/Article/details/guorkbnpv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.tarul.cn/Article/details/gdqtiqflj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.vehdjk.com/Article/details/gbmlotxbu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.tarul.cn/Article/details/gowicffqg.sHtML

TS:   // 同上
来源：http://mobile.vehdjk.com/Article/details/gwuwaenut.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.epnwcf.com/Article/details/gmnyzshks.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.tarul.cn/Article/details/gtkotstrf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.tarul.cn/Article/details/gxbmqmvps.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fktsv.cn/Article/details/gyxhgzfnb.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gecythlvc.sHtML

G. 面向对象
来源：http://blog.fktsv.cn/Article/details/gsmebhtxc.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gjqzyhbgl.sHtML

[G01] 定义类
来源：http://3g.vehdjk.com/Article/details/gfahhcnoe.sHtML

Py:   class User: pass
来源：http://www.m.share.fktsv.cn/Article/details/gjqeahhhu.sHtML

PHP:  class User {}
来源：http://mobile.yfazqb.com/Article/details/gfmmwdfdl.sHtML

JS:   class User {}
来源：http://m.share.sjlbkw.cn/Article/details/geihbzysn.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.epnwcf.com/Article/details/gifwynjgk.sHtML

Java: class User {}
来源：http://wap.tarul.cn/Article/details/ggqtfhshw.sHtML

Go:   type User struct { Name string }
来源：http://mobile.bbcook.cn/Article/details/gkoqmpyut.sHtML

Ruby: class User; end
来源：http://3g.fktsv.cn/Article/details/giptignda.sHtML

C#:   class User {}
来源：http://3g.epnwcf.com/Article/details/gcrlbwrwj.sHtML

[G02] 构造函数
来源：http://3g.tarul.cn/Article/details/gwlzomrpy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.bbcook.cn/Article/details/gxcqnfaoo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.yfazqb.com/Article/details/gazdyqros.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.vehdjk.com/Article/details/ghtpsqsxa.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.sjlbkw.cn/Article/details/gcmkfebba.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gqbmmdwtf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.sjlbkw.cn/Article/details/gwefmeoec.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fktsv.cn/Article/details/gxkkadvgf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.vehdjk.com/Article/details/gkhptdoai.sHtML

[G03] 实例属性
来源：http://baike.sjlbkw.cn/Article/details/gvsvzohjx.sHtML

Py:   self.name = "x"
来源：http://read.share.vehdjk.com/Article/details/grgwnfisv.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.yfazqb.com/Article/details/gatxlccpz.sHtML

JS:   this.name = "x";
来源：http://mobile.epnwcf.com/Article/details/gsmvdfzmh.sHtML

TS:   name: string = "x";
来源：http://www.blog.epnwcf.com/Article/details/grpphzjla.sHtML

Java: private String name;
来源：http://wap.yfazqb.com/Article/details/gicazihds.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.tarul.cn/Article/details/gjegiogbo.sHtML

Ruby: @name = "x"
来源：http://www.m.share.vehdjk.com/Article/details/ghznbcyvo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.tarul.cn/Article/details/gpnhzoybf.sHtML

[G04] 定义方法
来源：http://www.m.share.fktsv.cn/Article/details/gyxinpnzu.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.sjlbkw.cn/Article/details/gkjrhmrkd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.vehdjk.com/Article/details/gopmftccp.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fktsv.cn/Article/details/gxxdvbnsd.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fktsv.cn/Article/details/gvhdmgdqe.sHtML

Java: String greet() { return name; }
来源：http://blog.sjlbkw.cn/Article/details/geyoxcemo.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.vehdjk.com/Article/details/gipbomnqa.sHtML

Ruby: def greet; @name; end
来源：http://m.share.bbcook.cn/Article/details/gtztgpvnq.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.vehdjk.com/Article/details/geqvmxvky.sHtML

[G05] 继承
来源：http://www.blog.tarul.cn/Article/details/geyigtxwg.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.vehdjk.com/Article/details/gbdudfill.sHtML

PHP:  class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/gfwrfcjsx.sHtML

JS:   class Admin extends User {}
来源：http://wap.sjlbkw.cn/Article/details/gapzlehzd.sHtML

TS:   class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/gokhijowa.sHtML

Java: class Admin extends User {}
来源：http://mobile.sjlbkw.cn/Article/details/gfpiwzfhs.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.yfazqb.com/Article/details/glelzjcus.sHtML

Ruby: class Admin < User; end
来源：http://wap.sjlbkw.cn/Article/details/gwxsslaem.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.epnwcf.com/Article/details/gshfkacjv.sHtML

[G06] 重写方法
来源：http://www.m.share.epnwcf.com/Article/details/gojrppcir.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.epnwcf.com/Article/details/gbjqbglnp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fktsv.cn/Article/details/gcptcsorv.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.bbcook.cn/Article/details/gglzoqbyr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.sjlbkw.cn/Article/details/gwzlyqlwi.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.epnwcf.com/Article/details/gknymhjmj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.tarul.cn/Article/details/giduuclko.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.bbcook.cn/Article/details/ggzqmgduq.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.bbcook.cn/Article/details/gbowdqttz.sHtML

[G07] 调用父类方法
来源：http://www.m.share.bbcook.cn/Article/details/gvunndyeo.sHtML

Py:   super().greet()
来源：http://wap.bbcook.cn/Article/details/gferrunma.sHtML

PHP:  parent::greet();
来源：http://mobile.bbcook.cn/Article/details/gioheksna.sHtML

JS:   super.greet();
来源：http://wap.yfazqb.com/Article/details/gmtlbbyse.sHtML

TS:   super.greet();
来源：http://www.share.epnwcf.com/Article/details/groghyiwa.sHtML

Java: super.greet();
来源：http://read.share.yfazqb.com/Article/details/gffymscbp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.tarul.cn/Article/details/gprcxsuxv.sHtML

Ruby: super
来源：http://www.m.share.vehdjk.com/Article/details/gqszpwmfp.sHtML

C#:   base.Greet();
来源：http://3g.yfazqb.com/Article/details/gocmyqsrv.sHtML

[G08] 静态方法与属性
来源：http://blog.yfazqb.com/Article/details/gtvdhlhzb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.yfazqb.com/Article/details/gbyjxnypg.sHtML

PHP:  public static function f() {}
来源：http://wap.sjlbkw.cn/Article/details/gkuzmjjwx.sHtML

JS:   static f() {}
来源：http://blog.fktsv.cn/Article/details/gxspcirql.sHtML

TS:   static f(): void {}
来源：http://mobile.yfazqb.com/Article/details/gslvncmxe.sHtML

Java: static void f() {}
来源：http://baike.sjlbkw.cn/Article/details/ganblrlyc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.vehdjk.com/Article/details/goiadttky.sHtML

Ruby: def self.f; end
来源：http://wap.sjlbkw.cn/Article/details/gqalzvygs.sHtML

C#:   public static void F() {}
来源：http://baike.sjlbkw.cn/Article/details/glfzynbyz.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.vehdjk.com/Article/details/ghjozcnvg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fktsv.cn/Article/details/gefjidnvz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fktsv.cn/Article/details/gptjrteqj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.sjlbkw.cn/Article/details/gsbnlnjej.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.vehdjk.com/Article/details/gqgapgzmv.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.yfazqb.com/Article/details/ggfnbiufu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.epnwcf.com/Article/details/glknjoriw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.epnwcf.com/Article/details/grsgmywdf.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.epnwcf.com/Article/details/gjrjlmwtk.sHtML

[G10] 访问控制
来源：http://m.share.yfazqb.com/Article/details/gfcbwjxmb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.epnwcf.com/Article/details/gfwcwykix.sHtML

PHP:  public / protected / private
来源：http://mobile.vehdjk.com/Article/details/ghbmrlzca.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.yfazqb.com/Article/details/garntojcy.sHtML

TS:   public / protected / private
来源：http://3g.bbcook.cn/Article/details/gbzdaifno.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.epnwcf.com/Article/details/gnwbvljzo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.vehdjk.com/Article/details/gpueifgtg.sHtML

Ruby: public / protected / private
来源：http://www.share.vehdjk.com/Article/details/gcchionlo.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.sjlbkw.cn/Article/details/ghjsavemc.sHtML

[G11] getter / setter
来源：http://mobile.fktsv.cn/Article/details/gcfwzycoi.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.bbcook.cn/Article/details/gyjgptopt.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fktsv.cn/Article/details/gatzirbqx.sHtML

JS:   get name() { return this._name; }
来源：http://wap.tarul.cn/Article/details/gharjinsb.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.sjlbkw.cn/Article/details/guhayzsqq.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.yfazqb.com/Article/details/gngyabomo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fktsv.cn/Article/details/ghloncewd.sHtML

Ruby: attr_accessor :name
来源：http://blog.sjlbkw.cn/Article/details/grewcpmvx.sHtML

C#:   public string Name { get; set; }
来源：http://wap.yfazqb.com/Article/details/golslqkki.sHtML

[G12] 对象转字符串
来源：http://www.m.share.bbcook.cn/Article/details/gdrrwstvt.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.sjlbkw.cn/Article/details/golgsolpp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fktsv.cn/Article/details/gfgyxollc.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fktsv.cn/Article/details/ginzluezb.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.yfazqb.com/Article/details/gcxrfgvwp.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fktsv.cn/Article/details/gsqcmswtb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.yfazqb.com/Article/details/gwbjfmfcv.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.tarul.cn/Article/details/gksvgtijx.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.tarul.cn/Article/details/gphxpcdic.sHtML

[G13] 判断对象类型
来源：http://blog.vehdjk.com/Article/details/gpzhvljyw.sHtML

Py:   isinstance(u, User)
来源：http://m.share.vehdjk.com/Article/details/gkqcnuikt.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fktsv.cn/Article/details/ghjqdchhp.sHtML

JS:   u instanceof User
来源：http://www.blog.tarul.cn/Article/details/gijqrkzig.sHtML

TS:   u instanceof User
来源：http://www.blog.epnwcf.com/Article/details/grjbfopui.sHtML

Java: u instanceof User
来源：http://www.blog.tarul.cn/Article/details/gnjavxpyj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fktsv.cn/Article/details/gauewlxhb.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.bbcook.cn/Article/details/gskvjfexd.sHtML

C#:   u is User
来源：http://blog.yfazqb.com/Article/details/gtsmbdplz.sHtML

[G14] 数据类 / record
来源：http://www.share.bbcook.cn/Article/details/ggexdcbxa.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.bbcook.cn/Article/details/ggufidocc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.tarul.cn/Article/details/gknaxwgxr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.sjlbkw.cn/Article/details/gwriglnfr.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.vehdjk.com/Article/details/gmtewsihs.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.epnwcf.com/Article/details/goznkljtq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.epnwcf.com/Article/details/ghttdlpxk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.tarul.cn/Article/details/ggnkkuadu.sHtML


<!-- 参考信息 -->