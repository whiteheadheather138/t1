代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.tarul.cn/Article/details/gleejnddl.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fktsv.cn/Article/details/giubblqaq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fktsv.cn/Article/details/gbuxxeoep.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.bbcook.cn/Article/details/gkuwuviyc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fktsv.cn/Article/details/gusozgpjc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fktsv.cn/Article/details/ghlcybbvm.sHtML

Ruby: s.capitalize
来源：http://m.share.sjlbkw.cn/Article/details/gqhnlwqfh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.yfazqb.com/Article/details/gdwqqghyi.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fktsv.cn/Article/details/getqrmmeb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.yfazqb.com/Article/details/gsrxjpabg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.epnwcf.com/Article/details/gtjptfdfu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fktsv.cn/Article/details/gwbnjvcck.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.vehdjk.com/Article/details/gmzdxlzru.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.vehdjk.com/Article/details/gjjyahtst.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fktsv.cn/Article/details/gacvwlzrr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fktsv.cn/Article/details/gztjjgepv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.vehdjk.com/Article/details/gtfdjqslx.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.bbcook.cn/Article/details/gkgwhlbop.sHtML

Py:   s.splitlines()
来源：http://read.share.vehdjk.com/Article/details/gnuhyuylw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.sjlbkw.cn/Article/details/gdhmvqrrm.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.epnwcf.com/Article/details/gkyspyhmv.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.yfazqb.com/Article/details/gkvwiqytg.sHtML

Java: s.lines().toList()
来源：http://m.share.sjlbkw.cn/Article/details/gqlwayfbi.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.vehdjk.com/Article/details/gnonjtzhl.sHtML

Ruby: s.lines
来源：http://www.m.share.sjlbkw.cn/Article/details/gmmqvhlqw.sHtML

C#:   s.Split('\n')
来源：http://3g.tarul.cn/Article/details/gnyllbzfg.sHtML

[E20] 判断字符串是否为空
来源：http://3g.sjlbkw.cn/Article/details/gfpzfvooi.sHtML

Py:   if not s:
来源：http://baike.fktsv.cn/Article/details/gztwuqmus.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fktsv.cn/Article/details/gyjcrkqmd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.epnwcf.com/Article/details/gchfdlnmf.sHtML

TS:   if (s === "") {}
来源：http://www.share.bbcook.cn/Article/details/ggwthsljx.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.bbcook.cn/Article/details/gujoftrdz.sHtML

Go:   if s == "" {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gmecxmhen.sHtML

Ruby: if s.empty?
来源：http://www.share.yfazqb.com/Article/details/gtavrqkwc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.vehdjk.com/Article/details/gbukbsnzj.sHtML

[E21] 超长截断加省略号
来源：http://mobile.sjlbkw.cn/Article/details/gexjirfnp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.epnwcf.com/Article/details/gkgucblqu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.sjlbkw.cn/Article/details/gqwivkael.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.bbcook.cn/Article/details/gydyjydto.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gnahckmdn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.epnwcf.com/Article/details/gnrzeywkj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fktsv.cn/Article/details/gpntfplln.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.tarul.cn/Article/details/gdlstwudi.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.vehdjk.com/Article/details/gudwbarfc.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.yfazqb.com/Article/details/gjycwkota.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.bbcook.cn/Article/details/gldgopfwj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.sjlbkw.cn/Article/details/gsrytqhnc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.vehdjk.com/Article/details/gvjwtpvtl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.sjlbkw.cn/Article/details/gdqgoabar.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.bbcook.cn/Article/details/gklywtjtl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.yfazqb.com/Article/details/gbildumxz.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.yfazqb.com/Article/details/ggbjlbbhb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.bbcook.cn/Article/details/gthhbzzjg.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gsrvhpnnd.sHtML

F. 文件与目录
来源：http://read.share.tarul.cn/Article/details/gfnrtafjk.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gvdwsszxk.sHtML

[F01] 读取整个文件
来源：http://read.share.yfazqb.com/Article/details/galxbvfmb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fktsv.cn/Article/details/gdfcegysl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fktsv.cn/Article/details/geuwqhbku.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fktsv.cn/Article/details/gqksqvxus.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.yfazqb.com/Article/details/glhgiejmc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.vehdjk.com/Article/details/gesajmgae.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fktsv.cn/Article/details/gdgjmxurb.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gcucigyem.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gigamrqim.sHtML

[F02] 逐行读取文件
来源：http://m.share.fktsv.cn/Article/details/gfzvdgstb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.yfazqb.com/Article/details/gdhcjcyqq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.bbcook.cn/Article/details/gtelitypd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.bbcook.cn/Article/details/gjruqkpfz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.tarul.cn/Article/details/gcynxsmfn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fktsv.cn/Article/details/gcnoztkrk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.sjlbkw.cn/Article/details/gqizvgzan.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsdzcznwc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fktsv.cn/Article/details/giachcndp.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.yfazqb.com/Article/details/gsfyewedg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fktsv.cn/Article/details/geaetjfhb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.tarul.cn/Article/details/gybdjdxku.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.yfazqb.com/Article/details/gfudngspn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.epnwcf.com/Article/details/gbbkgerdt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.sjlbkw.cn/Article/details/grmukmcwy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.yfazqb.com/Article/details/gyqxzhpkm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.tarul.cn/Article/details/gzpsrkoqi.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.epnwcf.com/Article/details/gmotfmcmp.sHtML

[F04] 追加写入文件
来源：http://mobile.yfazqb.com/Article/details/gdhxenwyk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.sjlbkw.cn/Article/details/gscfntyft.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fktsv.cn/Article/details/gvmwqvjyz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.vehdjk.com/Article/details/gpvyspocv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.sjlbkw.cn/Article/details/gfthvoltl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.bbcook.cn/Article/details/gnlwsfbmo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.sjlbkw.cn/Article/details/gecvalzec.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fktsv.cn/Article/details/gdhpapdqg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.bbcook.cn/Article/details/gvhcspkri.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.tarul.cn/Article/details/gsviokmme.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.sjlbkw.cn/Article/details/gxkkdjqky.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.epnwcf.com/Article/details/gthpdpdan.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gebusspxg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gfjdukkuq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.tarul.cn/Article/details/ggzryftcl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.epnwcf.com/Article/details/gxuqhgrrb.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.tarul.cn/Article/details/gzjruckbm.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gxgikgzgt.sHtML

[F06] 删除文件
来源：http://blog.bbcook.cn/Article/details/gztawjceb.sHtML

Py:   os.remove("a.txt")
来源：http://3g.vehdjk.com/Article/details/gjnenpnlj.sHtML

PHP:  unlink("a.txt");
来源：http://3g.epnwcf.com/Article/details/gybqxcwxh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gbncoojfs.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.vehdjk.com/Article/details/ghrncmbry.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.epnwcf.com/Article/details/gdzfoehru.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gxrstvxkv.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gyxjtnhtj.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gkdovqdsw.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.yfazqb.com/Article/details/gdxmysihf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fktsv.cn/Article/details/gdrkedamz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fktsv.cn/Article/details/gxslbjjcr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.sjlbkw.cn/Article/details/gqpjjmwlg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.yfazqb.com/Article/details/gxjoyernh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.vehdjk.com/Article/details/gqwrbckzt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.sjlbkw.cn/Article/details/gcehqqlvj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.vehdjk.com/Article/details/gjdbcmxgc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fktsv.cn/Article/details/gjuztrgpq.sHtML

[F08] 遍历目录
来源：http://wap.fktsv.cn/Article/details/gysoamycx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.sjlbkw.cn/Article/details/guknwarvs.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.sjlbkw.cn/Article/details/ggsucmahn.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.vehdjk.com/Article/details/gfwzqrlvy.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/ghdhicnuz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.vehdjk.com/Article/details/gglmcuhpg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.bbcook.cn/Article/details/gsykpaznm.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.yfazqb.com/Article/details/gazyzyrbl.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.yfazqb.com/Article/details/gjqhukbha.sHtML

[F09] 获取文件大小
来源：http://mobile.epnwcf.com/Article/details/gwpffayhi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.vehdjk.com/Article/details/goxmmzvzq.sHtML

PHP:  filesize("a.txt");
来源：http://wap.vehdjk.com/Article/details/genowtwzg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.yfazqb.com/Article/details/gndidbtoh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fktsv.cn/Article/details/gqhqoixrx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.sjlbkw.cn/Article/details/gtltlsnxg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.epnwcf.com/Article/details/ghjcrsgcq.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gldqzdugg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.sjlbkw.cn/Article/details/gsqmvrqxt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.bbcook.cn/Article/details/ghketykil.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.bbcook.cn/Article/details/gmeswgomb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fktsv.cn/Article/details/geqyzsivc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/ghmgrguzj.sHtML

TS:   path.extname("a.txt")
来源：http://3g.yfazqb.com/Article/details/gwbyngvgs.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.tarul.cn/Article/details/govbcyput.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/gkmiqeabe.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.bbcook.cn/Article/details/ghastsbnm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gfzigqpze.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.bbcook.cn/Article/details/gbkcrlozw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.sjlbkw.cn/Article/details/gaehakqqo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.yfazqb.com/Article/details/goqiqufrm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.yfazqb.com/Article/details/guqueiglz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/gdjuxtqfu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwdhgoqom.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.sjlbkw.cn/Article/details/gzpwjrlue.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/gtmpzabde.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fktsv.cn/Article/details/gwjffpbsd.sHtML

[F12] CSV 读写
来源：http://read.share.bbcook.cn/Article/details/gleexxtku.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.tarul.cn/Article/details/gdxsmigso.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.sjlbkw.cn/Article/details/gtmkuzjkk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.sjlbkw.cn/Article/details/gvyghklpt.sHtML

TS:   // 同上
来源：http://m.share.epnwcf.com/Article/details/gljeygevq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.bbcook.cn/Article/details/gllwqakfa.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.epnwcf.com/Article/details/gffeeqnsl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.epnwcf.com/Article/details/gdpwwouaf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.yfazqb.com/Article/details/gekrozwpl.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/grzoalcty.sHtML

G. 面向对象
来源：http://www.blog.sjlbkw.cn/Article/details/gpuurjnpt.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gtcydbdum.sHtML

[G01] 定义类
来源：http://blog.yfazqb.com/Article/details/gtswgnffl.sHtML

Py:   class User: pass
来源：http://www.blog.sjlbkw.cn/Article/details/geouiquvc.sHtML

PHP:  class User {}
来源：http://baike.vehdjk.com/Article/details/gfwpxprvc.sHtML

JS:   class User {}
来源：http://3g.yfazqb.com/Article/details/gqmfkhahp.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.tarul.cn/Article/details/gspyjnmka.sHtML

Java: class User {}
来源：http://mobile.tarul.cn/Article/details/gffbntmxb.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.yfazqb.com/Article/details/gdncarobs.sHtML

Ruby: class User; end
来源：http://read.share.tarul.cn/Article/details/gyzmfprei.sHtML

C#:   class User {}
来源：http://read.share.yfazqb.com/Article/details/grctdzeer.sHtML

[G02] 构造函数
来源：http://read.share.yfazqb.com/Article/details/gykmnmnsn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.bbcook.cn/Article/details/gxzcppqbk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.tarul.cn/Article/details/gmtuoxoib.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.bbcook.cn/Article/details/gocukpumz.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.bbcook.cn/Article/details/gfukcprue.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.tarul.cn/Article/details/gcxgbfnnl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.epnwcf.com/Article/details/gnwdllxof.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.yfazqb.com/Article/details/gvtjkmhba.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.vehdjk.com/Article/details/gcvwxpcqz.sHtML

[G03] 实例属性
来源：http://3g.yfazqb.com/Article/details/gipmqkrvu.sHtML

Py:   self.name = "x"
来源：http://blog.yfazqb.com/Article/details/ggkpdnmnx.sHtML

PHP:  public string $name = "x";
来源：http://www.share.yfazqb.com/Article/details/gldlhdkbg.sHtML

JS:   this.name = "x";
来源：http://mobile.yfazqb.com/Article/details/gvipjxlqm.sHtML

TS:   name: string = "x";
来源：http://baike.sjlbkw.cn/Article/details/gjgwdlqfv.sHtML

Java: private String name;
来源：http://read.share.epnwcf.com/Article/details/getknkgeo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.epnwcf.com/Article/details/gkegnrxsl.sHtML

Ruby: @name = "x"
来源：http://read.share.bbcook.cn/Article/details/gbchigimd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.vehdjk.com/Article/details/glhorvwrx.sHtML

[G04] 定义方法
来源：http://baike.fktsv.cn/Article/details/galzjucaq.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.sjlbkw.cn/Article/details/gjindkzoi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fktsv.cn/Article/details/gimlfyohc.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.yfazqb.com/Article/details/gbxvsista.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.vehdjk.com/Article/details/gvnwlgrkb.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.tarul.cn/Article/details/gicxzyzbg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.epnwcf.com/Article/details/gcpmuucdy.sHtML

Ruby: def greet; @name; end
来源：http://read.share.sjlbkw.cn/Article/details/grosnoqot.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.epnwcf.com/Article/details/ghzrymuor.sHtML

[G05] 继承
来源：http://www.share.epnwcf.com/Article/details/gfgubkowc.sHtML

Py:   class Admin(User): pass
来源：http://read.share.yfazqb.com/Article/details/gsoqnsjqx.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/gwgadnqyk.sHtML

JS:   class Admin extends User {}
来源：http://3g.epnwcf.com/Article/details/gkztqkktb.sHtML

TS:   class Admin extends User {}
来源：http://blog.vehdjk.com/Article/details/ggnbktsmo.sHtML

Java: class Admin extends User {}
来源：http://mobile.fktsv.cn/Article/details/gnqokrixw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fktsv.cn/Article/details/gjofzxhzd.sHtML

Ruby: class Admin < User; end
来源：http://baike.bbcook.cn/Article/details/gpwjgjpjd.sHtML

C#:   class Admin : User {}
来源：http://mobile.epnwcf.com/Article/details/gtddfzsxo.sHtML

[G06] 重写方法
来源：http://3g.epnwcf.com/Article/details/gwbicdxbv.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.bbcook.cn/Article/details/gciphhdjf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.tarul.cn/Article/details/gdrvvqtkv.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.yfazqb.com/Article/details/gktnnmirp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.yfazqb.com/Article/details/gbfrwhqoy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/gmekaqkgx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.sjlbkw.cn/Article/details/ggxhpzgan.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.sjlbkw.cn/Article/details/gcrpobamz.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.epnwcf.com/Article/details/gccwrcpna.sHtML

[G07] 调用父类方法
来源：http://www.blog.fktsv.cn/Article/details/gkkceixhh.sHtML

Py:   super().greet()
来源：http://www.m.share.fktsv.cn/Article/details/guveacesq.sHtML

PHP:  parent::greet();
来源：http://m.share.vehdjk.com/Article/details/grcvrcomd.sHtML

JS:   super.greet();
来源：http://www.share.vehdjk.com/Article/details/guqwkogmk.sHtML

TS:   super.greet();
来源：http://baike.yfazqb.com/Article/details/gitbkulpj.sHtML

Java: super.greet();
来源：http://blog.sjlbkw.cn/Article/details/grhzpxpgw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.vehdjk.com/Article/details/gtfzketsw.sHtML

Ruby: super
来源：http://read.share.vehdjk.com/Article/details/girpaezsw.sHtML

C#:   base.Greet();
来源：http://blog.fktsv.cn/Article/details/gvylkkujg.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.yfazqb.com/Article/details/gcrubvrwj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.vehdjk.com/Article/details/glriryeoi.sHtML

PHP:  public static function f() {}
来源：http://blog.tarul.cn/Article/details/gdknlhzfh.sHtML

JS:   static f() {}
来源：http://blog.epnwcf.com/Article/details/gdldlohxg.sHtML

TS:   static f(): void {}
来源：http://baike.bbcook.cn/Article/details/gmjscsody.sHtML

Java: static void f() {}
来源：http://www.blog.epnwcf.com/Article/details/gtezepujh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.epnwcf.com/Article/details/gnyjlibjr.sHtML

Ruby: def self.f; end
来源：http://read.share.fktsv.cn/Article/details/gxajhbqam.sHtML

C#:   public static void F() {}
来源：http://read.share.tarul.cn/Article/details/girbserrz.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.epnwcf.com/Article/details/geshcwwmd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.yfazqb.com/Article/details/geldidqwf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.yfazqb.com/Article/details/gowfizixo.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fktsv.cn/Article/details/gydpaezkb.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbfoenqur.sHtML

Java: interface Shape { double area(); }
来源：http://blog.yfazqb.com/Article/details/gbuamnnnm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.vehdjk.com/Article/details/glkkotgdi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.yfazqb.com/Article/details/ghtbvbtil.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.tarul.cn/Article/details/gkopfxkxg.sHtML

[G10] 访问控制
来源：http://www.share.fktsv.cn/Article/details/gucxgrlpb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.sjlbkw.cn/Article/details/gwnrbhgbw.sHtML

PHP:  public / protected / private
来源：http://www.share.yfazqb.com/Article/details/gldvrlzpg.sHtML

JS:   #private 字段；其余公开
来源：http://baike.yfazqb.com/Article/details/gqyrsuwoy.sHtML

TS:   public / protected / private
来源：http://3g.epnwcf.com/Article/details/gpoujihgr.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.vehdjk.com/Article/details/gomdelehn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fktsv.cn/Article/details/gfsgxdoig.sHtML

Ruby: public / protected / private
来源：http://read.share.sjlbkw.cn/Article/details/gfksyyakc.sHtML

C#:   public / protected / private / internal
来源：http://www.share.yfazqb.com/Article/details/gqqmrmurb.sHtML

[G11] getter / setter
来源：http://www.m.share.yfazqb.com/Article/details/gepnopdnb.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fktsv.cn/Article/details/geaiencxl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.vehdjk.com/Article/details/gtmvcgbzc.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.bbcook.cn/Article/details/gyjpnpecw.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.tarul.cn/Article/details/gcjysvido.sHtML

Java: public String getName() { return name; }
来源：http://baike.vehdjk.com/Article/details/gpvtzcscf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.tarul.cn/Article/details/gnaawpijy.sHtML

Ruby: attr_accessor :name
来源：http://blog.tarul.cn/Article/details/gzqwznoyz.sHtML

C#:   public string Name { get; set; }
来源：http://3g.tarul.cn/Article/details/gvbmcvkea.sHtML

[G12] 对象转字符串
来源：http://baike.tarul.cn/Article/details/goggoljup.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.tarul.cn/Article/details/gnpzriwmk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.vehdjk.com/Article/details/gckcwjyvv.sHtML

JS:   toString() { return this.name; }
来源：http://blog.vehdjk.com/Article/details/gwpprvlfh.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.epnwcf.com/Article/details/gyvvomkmr.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.epnwcf.com/Article/details/gqtjcdjld.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.vehdjk.com/Article/details/gasdyqomm.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.bbcook.cn/Article/details/gwywglqni.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.sjlbkw.cn/Article/details/gxthjodgh.sHtML

[G13] 判断对象类型
来源：http://baike.fktsv.cn/Article/details/gkfixynbq.sHtML

Py:   isinstance(u, User)
来源：http://wap.bbcook.cn/Article/details/gbtxuiaza.sHtML

PHP:  $u instanceof User
来源：http://read.share.tarul.cn/Article/details/gjvavsncu.sHtML

JS:   u instanceof User
来源：http://3g.epnwcf.com/Article/details/gkdnmlemd.sHtML

TS:   u instanceof User
来源：http://3g.epnwcf.com/Article/details/grldkfbhp.sHtML

Java: u instanceof User
来源：http://m.share.bbcook.cn/Article/details/ghlfpivla.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.sjlbkw.cn/Article/details/gmwzeqqxc.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.epnwcf.com/Article/details/gowuzhmvd.sHtML

C#:   u is User
来源：http://baike.yfazqb.com/Article/details/grgcbggzc.sHtML

[G14] 数据类 / record
来源：http://blog.tarul.cn/Article/details/gzkikwrwm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.bbcook.cn/Article/details/gbkfunqbn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.bbcook.cn/Article/details/gzrpacyvw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.yfazqb.com/Article/details/gqxysrmta.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.bbcook.cn/Article/details/gezvtrnft.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fktsv.cn/Article/details/ggbjbqxyp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fktsv.cn/Article/details/gznsljeoe.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.vehdjk.com/Article/details/gjhuniauy.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fktsv.cn/Article/details/gonowxkly.sHtML

[G15] 枚举
来源：http://blog.yfazqb.com/Article/details/garfhyjpj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.bbcook.cn/Article/details/gmopnlkbe.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.sjlbkw.cn/Article/details/gqgdyyqfn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.tarul.cn/Article/details/gcnwvxndr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.epnwcf.com/Article/details/gavoeduxn.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.bbcook.cn/Article/details/gpjntxcwq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.sjlbkw.cn/Article/details/gikxhqsza.sHtML


<!-- 参考信息 -->