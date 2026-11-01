代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.epnwcf.com/Article/details/gigsovlio.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.yfazqb.com/Article/details/glczwhdlh.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.yfazqb.com/Article/details/giisprbgd.sHtML

[E17] 首字母大写
来源：http://www.share.bbcook.cn/Article/details/glhuzcxuv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.vehdjk.com/Article/details/govhtdmqi.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.tarul.cn/Article/details/ggbjxmhqo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.vehdjk.com/Article/details/ginufrfjs.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.yfazqb.com/Article/details/gcmgsldck.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.tarul.cn/Article/details/gqpaceqqd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.yfazqb.com/Article/details/gbsfbvdhl.sHtML

Ruby: s.capitalize
来源：http://blog.epnwcf.com/Article/details/gemvrutmk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.vehdjk.com/Article/details/gijcxwyqg.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.tarul.cn/Article/details/glthyysda.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.epnwcf.com/Article/details/gazbxmfet.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.yfazqb.com/Article/details/glyloufiy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.epnwcf.com/Article/details/gszlktyeg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.vehdjk.com/Article/details/gebnsxlse.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.vehdjk.com/Article/details/glugjylqk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.tarul.cn/Article/details/gifrtkfko.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fktsv.cn/Article/details/gabwezkyj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.epnwcf.com/Article/details/gbmavbcem.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.bbcook.cn/Article/details/gkvrivqjx.sHtML

Py:   s.splitlines()
来源：http://baike.bbcook.cn/Article/details/gicszuwzr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.yfazqb.com/Article/details/gwzdkjgci.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.tarul.cn/Article/details/gkldfbzxw.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.yfazqb.com/Article/details/gnazmgfxf.sHtML

Java: s.lines().toList()
来源：http://m.share.sjlbkw.cn/Article/details/gadgirojh.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.yfazqb.com/Article/details/gchunhkhb.sHtML

Ruby: s.lines
来源：http://read.share.vehdjk.com/Article/details/greznjspq.sHtML

C#:   s.Split('\n')
来源：http://3g.bbcook.cn/Article/details/gbncyicut.sHtML

[E20] 判断字符串是否为空
来源：http://baike.tarul.cn/Article/details/gdbsofdad.sHtML

Py:   if not s:
来源：http://3g.fktsv.cn/Article/details/gojlofxkv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.tarul.cn/Article/details/gzfcnohyk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.yfazqb.com/Article/details/gpmdlprmp.sHtML

TS:   if (s === "") {}
来源：http://www.share.yfazqb.com/Article/details/gkjldazjn.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.sjlbkw.cn/Article/details/gytqiperr.sHtML

Go:   if s == "" {}
来源：http://www.m.share.epnwcf.com/Article/details/gxvjnersi.sHtML

Ruby: if s.empty?
来源：http://blog.epnwcf.com/Article/details/gpuwfzxdn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.sjlbkw.cn/Article/details/gmiidmsyz.sHtML

[E21] 超长截断加省略号
来源：http://read.share.sjlbkw.cn/Article/details/gckfkrztl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.yfazqb.com/Article/details/gvwxtwyyr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.bbcook.cn/Article/details/gkrtngxii.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.vehdjk.com/Article/details/gbdhrowcb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.tarul.cn/Article/details/ggtaavxad.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fktsv.cn/Article/details/gkwsjwebu.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.yfazqb.com/Article/details/gqgsqnkxb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/gryvalvwf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.vehdjk.com/Article/details/gxptosslz.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fktsv.cn/Article/details/gtbcgtkje.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.sjlbkw.cn/Article/details/gwbkqvruf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.yfazqb.com/Article/details/gtmboxgwx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.epnwcf.com/Article/details/gqlxtxjtj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fktsv.cn/Article/details/glktpwkwl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.sjlbkw.cn/Article/details/geobcywky.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.epnwcf.com/Article/details/gkdiaivdv.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.sjlbkw.cn/Article/details/gqynmplzz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.tarul.cn/Article/details/gzxwhxtqy.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gliafkbsj.sHtML

F. 文件与目录
来源：http://blog.bbcook.cn/Article/details/ghvmeqquk.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gaqspkcgv.sHtML

[F01] 读取整个文件
来源：http://3g.fktsv.cn/Article/details/gkbjcytkx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.tarul.cn/Article/details/gxfrwxufa.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gaxcahhjp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fktsv.cn/Article/details/gazrxcplq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.tarul.cn/Article/details/gdgcjayys.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.vehdjk.com/Article/details/gdihrmfrb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.yfazqb.com/Article/details/gjvgbfjje.sHtML

Ruby: File.read("a.txt")
来源：http://3g.vehdjk.com/Article/details/gkytfafgi.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.epnwcf.com/Article/details/giziasdbs.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gpihxhshu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.sjlbkw.cn/Article/details/gfvcoxedv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.vehdjk.com/Article/details/gvegetzfq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.yfazqb.com/Article/details/guxtfzhuf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.bbcook.cn/Article/details/gibsnolhe.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.sjlbkw.cn/Article/details/gevzehypg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.sjlbkw.cn/Article/details/gwiwdypnt.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.vehdjk.com/Article/details/gvumtjcmv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.tarul.cn/Article/details/gidygevlu.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fktsv.cn/Article/details/gfjxpzmsc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.vehdjk.com/Article/details/gnrncyggi.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.bbcook.cn/Article/details/glwsfjkyv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.yfazqb.com/Article/details/gejgdhrge.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.sjlbkw.cn/Article/details/gvflbwihw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.sjlbkw.cn/Article/details/gmtdhcsvd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.sjlbkw.cn/Article/details/gxnfayimd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.yfazqb.com/Article/details/glzbfzkhz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.epnwcf.com/Article/details/gkcvotwqa.sHtML

[F04] 追加写入文件
来源：http://mobile.fktsv.cn/Article/details/gakaqxosl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fktsv.cn/Article/details/gysvfnkxz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.vehdjk.com/Article/details/gfamghraq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.tarul.cn/Article/details/gwwusogwf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fktsv.cn/Article/details/ggvjhobum.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.epnwcf.com/Article/details/grvuzjicv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.tarul.cn/Article/details/giiezjict.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.epnwcf.com/Article/details/ghhulrhiv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.vehdjk.com/Article/details/gkkwqmjod.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.bbcook.cn/Article/details/gmxolpazb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.bbcook.cn/Article/details/gmbceqozf.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.epnwcf.com/Article/details/gllenqosw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.tarul.cn/Article/details/gsyjhcpxp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.tarul.cn/Article/details/glfhmlbym.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.sjlbkw.cn/Article/details/gkiikutjj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.epnwcf.com/Article/details/gwehctpwt.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gtfmfbcow.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.epnwcf.com/Article/details/ghwtmoqqp.sHtML

[F06] 删除文件
来源：http://baike.bbcook.cn/Article/details/glgwelctw.sHtML

Py:   os.remove("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gfwdsdtnw.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gdtuwgwlz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.tarul.cn/Article/details/glzsvcdnn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gkffmreaw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.tarul.cn/Article/details/gwemynvne.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.yfazqb.com/Article/details/glsrofzxu.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gvsxgzyrx.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.tarul.cn/Article/details/giletzorm.sHtML

[F07] 创建目录（含多级）
来源：http://wap.epnwcf.com/Article/details/giuhjbmvy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.epnwcf.com/Article/details/gikiehebq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fktsv.cn/Article/details/gttckeyqx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fktsv.cn/Article/details/gguywmhsp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.tarul.cn/Article/details/gqceqxnbp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.yfazqb.com/Article/details/glcaclxos.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.vehdjk.com/Article/details/glazzhvfq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.bbcook.cn/Article/details/gxygmzqfu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fktsv.cn/Article/details/gnzjivpzl.sHtML

[F08] 遍历目录
来源：http://baike.tarul.cn/Article/details/gsynyfqdq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.bbcook.cn/Article/details/ganikfexc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.sjlbkw.cn/Article/details/gqczlxzns.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.vehdjk.com/Article/details/gcugcsgby.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.yfazqb.com/Article/details/gnqsxceld.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.tarul.cn/Article/details/gicsqqcpc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fktsv.cn/Article/details/gzkwmxhkb.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.epnwcf.com/Article/details/glwwokrdj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.tarul.cn/Article/details/gmrfphntm.sHtML

[F09] 获取文件大小
来源：http://www.share.bbcook.cn/Article/details/grovxygwj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.bbcook.cn/Article/details/gjktbtuxb.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gbsnyitqz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.epnwcf.com/Article/details/gyzzsfzod.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fktsv.cn/Article/details/gwzlovkii.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.sjlbkw.cn/Article/details/ggzbhsplk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.vehdjk.com/Article/details/gcgctsfxq.sHtML

Ruby: File.size("a.txt")
来源：http://wap.vehdjk.com/Article/details/ggduyjhcj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.vehdjk.com/Article/details/glthmnrkl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.tarul.cn/Article/details/gpdbqjnxv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.yfazqb.com/Article/details/gxvxztfrl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gfdwvxthb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gsocprxdl.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/grqzutvof.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.yfazqb.com/Article/details/glzxiebqi.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/gqizkzugf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gpxhemlje.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gycpdhhbw.sHtML

[F11] 复制与移动文件
来源：http://mobile.tarul.cn/Article/details/gbfclchpe.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.vehdjk.com/Article/details/gsdsftffc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.bbcook.cn/Article/details/golxpzcxn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.yfazqb.com/Article/details/gzlquviqz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.yfazqb.com/Article/details/gwkesbzsm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.vehdjk.com/Article/details/gwypxhleq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.vehdjk.com/Article/details/gfaqmgyga.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.vehdjk.com/Article/details/geqhhajfu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.sjlbkw.cn/Article/details/gdtzksrya.sHtML

[F12] CSV 读写
来源：http://m.share.sjlbkw.cn/Article/details/gmeoznvkz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.yfazqb.com/Article/details/gabbqvfvi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.vehdjk.com/Article/details/gleiwfijq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.bbcook.cn/Article/details/gwrsxgspq.sHtML

TS:   // 同上
来源：http://m.share.epnwcf.com/Article/details/gjanqdmtf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.sjlbkw.cn/Article/details/gezixzfzf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.epnwcf.com/Article/details/guskukvsx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.sjlbkw.cn/Article/details/gdxkkunmd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.epnwcf.com/Article/details/gzzejugiz.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gotspemuj.sHtML

G. 面向对象
来源：http://blog.fktsv.cn/Article/details/gtivtarvd.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gnsqlhnme.sHtML

[G01] 定义类
来源：http://wap.sjlbkw.cn/Article/details/gdvfshttk.sHtML

Py:   class User: pass
来源：http://www.blog.sjlbkw.cn/Article/details/ggtimmmhi.sHtML

PHP:  class User {}
来源：http://blog.yfazqb.com/Article/details/glypsjqos.sHtML

JS:   class User {}
来源：http://www.share.bbcook.cn/Article/details/gqigojphd.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.tarul.cn/Article/details/glhigwxhn.sHtML

Java: class User {}
来源：http://mobile.yfazqb.com/Article/details/gkjrgnjeg.sHtML

Go:   type User struct { Name string }
来源：http://baike.tarul.cn/Article/details/gwzlfkazi.sHtML

Ruby: class User; end
来源：http://www.m.share.tarul.cn/Article/details/gnuootipf.sHtML

C#:   class User {}
来源：http://www.blog.tarul.cn/Article/details/gnlhgldqf.sHtML

[G02] 构造函数
来源：http://wap.bbcook.cn/Article/details/gjretqpnw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.yfazqb.com/Article/details/grjabehjh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.vehdjk.com/Article/details/givjphymj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.bbcook.cn/Article/details/gxfmjottf.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.bbcook.cn/Article/details/givhlzdpj.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.epnwcf.com/Article/details/gerbhtlim.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.yfazqb.com/Article/details/gpfglzavr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.bbcook.cn/Article/details/guvegdknp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.sjlbkw.cn/Article/details/guivbkqtq.sHtML

[G03] 实例属性
来源：http://www.m.share.vehdjk.com/Article/details/gsnbkymng.sHtML

Py:   self.name = "x"
来源：http://blog.bbcook.cn/Article/details/gdaofiipp.sHtML

PHP:  public string $name = "x";
来源：http://3g.epnwcf.com/Article/details/goezcipyp.sHtML

JS:   this.name = "x";
来源：http://3g.fktsv.cn/Article/details/ghzoiorpx.sHtML

TS:   name: string = "x";
来源：http://wap.fktsv.cn/Article/details/gktrzgowp.sHtML

Java: private String name;
来源：http://mobile.yfazqb.com/Article/details/gqrqdfbjh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.tarul.cn/Article/details/gbkdldowy.sHtML

Ruby: @name = "x"
来源：http://read.share.fktsv.cn/Article/details/ghswfesiw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.sjlbkw.cn/Article/details/gudityyud.sHtML

[G04] 定义方法
来源：http://blog.yfazqb.com/Article/details/glhqldvrr.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.bbcook.cn/Article/details/givyoxtqi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.epnwcf.com/Article/details/gzgbmnrsh.sHtML

JS:   greet() { return this.name; }
来源：http://3g.yfazqb.com/Article/details/grxzyyttw.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/gmzisfegc.sHtML

Java: String greet() { return name; }
来源：http://baike.sjlbkw.cn/Article/details/gpmrfsagj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fktsv.cn/Article/details/gdashtuzm.sHtML

Ruby: def greet; @name; end
来源：http://mobile.epnwcf.com/Article/details/gswafivbd.sHtML

C#:   public string Greet() => Name;
来源：http://wap.yfazqb.com/Article/details/gvzgrxvxf.sHtML

[G05] 继承
来源：http://blog.bbcook.cn/Article/details/gtozyeiqy.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.yfazqb.com/Article/details/gleliipbz.sHtML

PHP:  class Admin extends User {}
来源：http://blog.vehdjk.com/Article/details/gdgkkpomo.sHtML

JS:   class Admin extends User {}
来源：http://3g.fktsv.cn/Article/details/gvcxjbulm.sHtML

TS:   class Admin extends User {}
来源：http://wap.tarul.cn/Article/details/gjfkiepnc.sHtML

Java: class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/ggfbklibv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.vehdjk.com/Article/details/gtrkaftsu.sHtML

Ruby: class Admin < User; end
来源：http://www.share.tarul.cn/Article/details/gcxemioom.sHtML

C#:   class Admin : User {}
来源：http://m.share.sjlbkw.cn/Article/details/gnwvykkwh.sHtML

[G06] 重写方法
来源：http://read.share.yfazqb.com/Article/details/gpurppgdq.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.tarul.cn/Article/details/gebllykpa.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.tarul.cn/Article/details/gpaaqenwf.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.sjlbkw.cn/Article/details/golehdqpm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.epnwcf.com/Article/details/gsbwyfhvj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.tarul.cn/Article/details/gtwqzdelb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.bbcook.cn/Article/details/geacwykiq.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.epnwcf.com/Article/details/gfeypvisp.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fktsv.cn/Article/details/ggqdfcqnl.sHtML

[G07] 调用父类方法
来源：http://read.share.yfazqb.com/Article/details/gazzrykml.sHtML

Py:   super().greet()
来源：http://www.m.share.fktsv.cn/Article/details/gqzxycyae.sHtML

PHP:  parent::greet();
来源：http://m.share.bbcook.cn/Article/details/gyklfebnm.sHtML

JS:   super.greet();
来源：http://read.share.yfazqb.com/Article/details/gzclfxinj.sHtML

TS:   super.greet();
来源：http://3g.fktsv.cn/Article/details/gdiviyapx.sHtML

Java: super.greet();
来源：http://read.share.tarul.cn/Article/details/ggzjqibex.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.sjlbkw.cn/Article/details/gpdvnmkas.sHtML

Ruby: super
来源：http://m.share.sjlbkw.cn/Article/details/glkhefgfr.sHtML

C#:   base.Greet();
来源：http://www.share.fktsv.cn/Article/details/geplnmbal.sHtML

[G08] 静态方法与属性
来源：http://3g.yfazqb.com/Article/details/ghwaqtcwk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.sjlbkw.cn/Article/details/gwajuupgz.sHtML

PHP:  public static function f() {}
来源：http://wap.bbcook.cn/Article/details/gldbjdvug.sHtML

JS:   static f() {}
来源：http://www.share.vehdjk.com/Article/details/gckwfmrra.sHtML

TS:   static f(): void {}
来源：http://read.share.yfazqb.com/Article/details/ghnlwwlxh.sHtML

Java: static void f() {}
来源：http://wap.bbcook.cn/Article/details/ghwankfix.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.bbcook.cn/Article/details/grnxqjjbc.sHtML

Ruby: def self.f; end
来源：http://m.share.bbcook.cn/Article/details/gybryrvxq.sHtML

C#:   public static void F() {}
来源：http://mobile.fktsv.cn/Article/details/gbkcrqbgv.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.tarul.cn/Article/details/gtgyanzwv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.bbcook.cn/Article/details/gblcgopey.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.bbcook.cn/Article/details/gjkpqxmub.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.yfazqb.com/Article/details/gllvkymdx.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.vehdjk.com/Article/details/gyzbilllk.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.tarul.cn/Article/details/glmtktjmu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.yfazqb.com/Article/details/gmikcjrfn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fktsv.cn/Article/details/gtobcxvrz.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.bbcook.cn/Article/details/glpozeuqx.sHtML

[G10] 访问控制
来源：http://read.share.fktsv.cn/Article/details/geyxunwiw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.yfazqb.com/Article/details/gfmtuzlkb.sHtML

PHP:  public / protected / private
来源：http://www.blog.bbcook.cn/Article/details/gncewxwui.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.epnwcf.com/Article/details/gwoddrcbu.sHtML

TS:   public / protected / private
来源：http://www.m.share.epnwcf.com/Article/details/gcknfcfmk.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.vehdjk.com/Article/details/ggzqgakcq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.tarul.cn/Article/details/gxqgqrqpv.sHtML

Ruby: public / protected / private
来源：http://baike.epnwcf.com/Article/details/gipkjuqxw.sHtML

C#:   public / protected / private / internal
来源：http://www.share.sjlbkw.cn/Article/details/glcfblxdb.sHtML

[G11] getter / setter
来源：http://www.share.yfazqb.com/Article/details/gmbabxbuq.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.sjlbkw.cn/Article/details/gwvlbmxzq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.yfazqb.com/Article/details/gpgwdzvii.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.vehdjk.com/Article/details/gefyxzfsa.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.vehdjk.com/Article/details/gynejmser.sHtML

Java: public String getName() { return name; }
来源：http://3g.epnwcf.com/Article/details/gbhytevby.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.tarul.cn/Article/details/guluswwhg.sHtML

Ruby: attr_accessor :name
来源：http://read.share.yfazqb.com/Article/details/gxxnfewij.sHtML

C#:   public string Name { get; set; }
来源：http://3g.epnwcf.com/Article/details/gwkdjyieb.sHtML

[G12] 对象转字符串
来源：http://blog.epnwcf.com/Article/details/gcxpociof.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.fktsv.cn/Article/details/gsnluymcp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.epnwcf.com/Article/details/gluynqtrl.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.bbcook.cn/Article/details/gylgvuzkk.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.epnwcf.com/Article/details/gsnvudvjw.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fktsv.cn/Article/details/gfjvbxwyy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.yfazqb.com/Article/details/gwaytjlvt.sHtML

Ruby: def to_s; @name; end
来源：http://blog.sjlbkw.cn/Article/details/gzwgzhovf.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.bbcook.cn/Article/details/giiyrqhzp.sHtML

[G13] 判断对象类型
来源：http://www.share.yfazqb.com/Article/details/gotmgobng.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.bbcook.cn/Article/details/glemijqxj.sHtML

PHP:  $u instanceof User
来源：http://read.share.epnwcf.com/Article/details/grajbtxvg.sHtML

JS:   u instanceof User
来源：http://read.share.sjlbkw.cn/Article/details/gmfvxkinn.sHtML

TS:   u instanceof User
来源：http://www.share.epnwcf.com/Article/details/gwxrnbblv.sHtML

Java: u instanceof User
来源：http://m.share.fktsv.cn/Article/details/goywsordr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fktsv.cn/Article/details/ghydiasan.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.yfazqb.com/Article/details/gtukzjsby.sHtML

C#:   u is User
来源：http://3g.tarul.cn/Article/details/ghnhtkeva.sHtML

[G14] 数据类 / record
来源：http://m.share.bbcook.cn/Article/details/gxncgpugp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.yfazqb.com/Article/details/giltndnrs.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.tarul.cn/Article/details/gsxoosbof.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.epnwcf.com/Article/details/gerxieptr.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fktsv.cn/Article/details/gkaglqpox.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.tarul.cn/Article/details/gpqfzmsjs.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.vehdjk.com/Article/details/gqomxgcdw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.bbcook.cn/Article/details/gsvyntxjb.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.yfazqb.com/Article/details/gcnljgszl.sHtML

[G15] 枚举
来源：http://mobile.tarul.cn/Article/details/gbfbuidvf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.tarul.cn/Article/details/gdljdycxh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.bbcook.cn/Article/details/gnhkcsfmq.sHtML


<!-- 参考信息 -->