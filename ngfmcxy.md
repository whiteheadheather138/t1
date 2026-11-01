代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvpecjyyc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fktsv.cn/Article/details/gizbmqils.sHtML

[E16] 数字千分位
来源：http://baike.vehdjk.com/Article/details/gpmmgorco.sHtML

Py:   f"{1234567:,}"
来源：http://3g.sjlbkw.cn/Article/details/gsyuquyta.sHtML

PHP:  number_format(1234567);
来源：http://blog.sjlbkw.cn/Article/details/gvortiere.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fktsv.cn/Article/details/gbajdfvhp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.sjlbkw.cn/Article/details/gnayavzrv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.yfazqb.com/Article/details/gnpqwooob.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fktsv.cn/Article/details/gbglqptgm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.vehdjk.com/Article/details/gkcjaafce.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.epnwcf.com/Article/details/glmrobgre.sHtML

[E17] 首字母大写
来源：http://baike.sjlbkw.cn/Article/details/gsxogtfkg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.vehdjk.com/Article/details/gxngszjbo.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.tarul.cn/Article/details/gnxstqjga.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.vehdjk.com/Article/details/gyknwypoz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.sjlbkw.cn/Article/details/ghjwchmjc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.yfazqb.com/Article/details/gciklpdjp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.tarul.cn/Article/details/gbxxyrmae.sHtML

Ruby: s.capitalize
来源：http://wap.sjlbkw.cn/Article/details/gwsqrbbav.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fktsv.cn/Article/details/gylejhjti.sHtML

[E18] 模板占位符替换
来源：http://3g.fktsv.cn/Article/details/gzpixcitd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.sjlbkw.cn/Article/details/ghdosqnpn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.vehdjk.com/Article/details/gtspkoiba.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.vehdjk.com/Article/details/gmzaigojo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.sjlbkw.cn/Article/details/gpymtcdef.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.vehdjk.com/Article/details/gujgfdebx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.bbcook.cn/Article/details/gnyzjwyhh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.bbcook.cn/Article/details/gzelhelzf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.bbcook.cn/Article/details/gqznprwxa.sHtML

[E19] 多行文本按行拆分
来源：http://wap.yfazqb.com/Article/details/gsxwkyuyh.sHtML

Py:   s.splitlines()
来源：http://baike.epnwcf.com/Article/details/guyawcqkv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.epnwcf.com/Article/details/gnacbyvlc.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fktsv.cn/Article/details/gesuzxpei.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.epnwcf.com/Article/details/gxcelhnvr.sHtML

Java: s.lines().toList()
来源：http://m.share.epnwcf.com/Article/details/glubdsair.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.yfazqb.com/Article/details/gzcdlxfwh.sHtML

Ruby: s.lines
来源：http://mobile.tarul.cn/Article/details/gnlutbtjc.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fktsv.cn/Article/details/gwuxnnwhc.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.epnwcf.com/Article/details/gdiwgpbac.sHtML

Py:   if not s:
来源：http://3g.tarul.cn/Article/details/gqalwzjtt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.sjlbkw.cn/Article/details/gjidrsmed.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.tarul.cn/Article/details/goemjjngl.sHtML

TS:   if (s === "") {}
来源：http://www.share.epnwcf.com/Article/details/gfzmlkpdd.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.vehdjk.com/Article/details/gvhdbbanx.sHtML

Go:   if s == "" {}
来源：http://wap.fktsv.cn/Article/details/guksayyby.sHtML

Ruby: if s.empty?
来源：http://blog.yfazqb.com/Article/details/gkfhkouzo.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.tarul.cn/Article/details/gictvttlj.sHtML

[E21] 超长截断加省略号
来源：http://baike.bbcook.cn/Article/details/grzoftsix.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fktsv.cn/Article/details/gvttbqkgp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.epnwcf.com/Article/details/gqkszwqxc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.bbcook.cn/Article/details/giwogbuwo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.sjlbkw.cn/Article/details/gqgebiiny.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fktsv.cn/Article/details/gnvrcnzjm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.epnwcf.com/Article/details/gaaqsbovd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.epnwcf.com/Article/details/govwfugeu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.yfazqb.com/Article/details/gckosujvs.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.yfazqb.com/Article/details/gfyvxaqoy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.sjlbkw.cn/Article/details/glqlrbopr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.epnwcf.com/Article/details/gqjmmgziz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.bbcook.cn/Article/details/gnyjkrxjx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.vehdjk.com/Article/details/gpwgnvzoc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.bbcook.cn/Article/details/gdcizindi.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.bbcook.cn/Article/details/gqziruero.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fktsv.cn/Article/details/glrvpoazb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fktsv.cn/Article/details/gspyqmwco.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gcswcpyff.sHtML

F. 文件与目录
来源：http://www.blog.sjlbkw.cn/Article/details/gjhgtsrlk.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/grdopuubc.sHtML

[F01] 读取整个文件
来源：http://blog.tarul.cn/Article/details/ginqarloq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.sjlbkw.cn/Article/details/glnahrgxa.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.vehdjk.com/Article/details/gkvuowwcw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fktsv.cn/Article/details/gbnagvikr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.tarul.cn/Article/details/gxnrfhoub.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fktsv.cn/Article/details/gkjqojonw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.sjlbkw.cn/Article/details/gljhxqshw.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gvnsqsifv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.bbcook.cn/Article/details/guufdmwth.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fktsv.cn/Article/details/gyvmwxzty.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.vehdjk.com/Article/details/gnkvezjaj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fktsv.cn/Article/details/gftcfofzp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.sjlbkw.cn/Article/details/gwpcwcwxq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.vehdjk.com/Article/details/gcaersjjp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.bbcook.cn/Article/details/gxbbgyrab.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.bbcook.cn/Article/details/grcgdomet.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.tarul.cn/Article/details/gjvuiauhb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.yfazqb.com/Article/details/gezbubllw.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.tarul.cn/Article/details/gtpibqabr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.yfazqb.com/Article/details/gavzagkbd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.yfazqb.com/Article/details/gbgrqmdwt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.bbcook.cn/Article/details/ganmwtcvj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.tarul.cn/Article/details/gxoaglblm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.tarul.cn/Article/details/gcswfmhek.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.sjlbkw.cn/Article/details/ggtaaiqji.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.yfazqb.com/Article/details/gggaguurs.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.tarul.cn/Article/details/gyrmzliza.sHtML

[F04] 追加写入文件
来源：http://mobile.sjlbkw.cn/Article/details/gjocxxvfd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.bbcook.cn/Article/details/gqbnqmhez.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.bbcook.cn/Article/details/gqdrtntpw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.yfazqb.com/Article/details/gusssiine.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.tarul.cn/Article/details/gtqtwtwhn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.bbcook.cn/Article/details/gmrnwguyc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.epnwcf.com/Article/details/ggedkzshr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.tarul.cn/Article/details/gkbbbgocp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.bbcook.cn/Article/details/gkwxthxyc.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.epnwcf.com/Article/details/gfuuubapq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.yfazqb.com/Article/details/guysgokxt.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/goejhxidn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.tarul.cn/Article/details/gwswdqght.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.vehdjk.com/Article/details/gnbsejrul.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.tarul.cn/Article/details/guddlvwxc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.bbcook.cn/Article/details/gzqjfwrsf.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.tarul.cn/Article/details/gvabaoewy.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.epnwcf.com/Article/details/grqbmhjns.sHtML

[F06] 删除文件
来源：http://3g.bbcook.cn/Article/details/gorxelgwz.sHtML

Py:   os.remove("a.txt")
来源：http://3g.yfazqb.com/Article/details/gmacetobk.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fktsv.cn/Article/details/giwgvmnhl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gncfngnjl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.bbcook.cn/Article/details/gbuujaiqp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.vehdjk.com/Article/details/gpemspzzj.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.tarul.cn/Article/details/gukqfqsug.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.vehdjk.com/Article/details/ghftticbl.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gqrvmdkcb.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fktsv.cn/Article/details/gndhqeusn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.sjlbkw.cn/Article/details/gundkxpoa.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.yfazqb.com/Article/details/gdaucyptj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.vehdjk.com/Article/details/gexkkisvl.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.epnwcf.com/Article/details/gcwmxvmad.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.vehdjk.com/Article/details/gtqobbdmh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.sjlbkw.cn/Article/details/gvibvgkyb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.epnwcf.com/Article/details/grrynfddv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fktsv.cn/Article/details/gjphgcweg.sHtML

[F08] 遍历目录
来源：http://www.share.bbcook.cn/Article/details/ggmdqlrkg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.epnwcf.com/Article/details/gwxfotfkt.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fktsv.cn/Article/details/gvlbrvaiw.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.vehdjk.com/Article/details/gyybstmpp.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.tarul.cn/Article/details/gkpywrssv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fktsv.cn/Article/details/gyqqzssfv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.epnwcf.com/Article/details/gmhrlmhlq.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fktsv.cn/Article/details/gvrogyojd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fktsv.cn/Article/details/gwzromhho.sHtML

[F09] 获取文件大小
来源：http://baike.tarul.cn/Article/details/gyggflvvv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.epnwcf.com/Article/details/gujaxsbat.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gvaoyxxgn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.epnwcf.com/Article/details/gwgegcwfd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.vehdjk.com/Article/details/gldahdogz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.sjlbkw.cn/Article/details/gzbktcbwo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.bbcook.cn/Article/details/gsftqokey.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gzfplbxec.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.yfazqb.com/Article/details/gxckfbnzn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.epnwcf.com/Article/details/gvobezrux.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fktsv.cn/Article/details/gxxmrxorl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.epnwcf.com/Article/details/giaeqjwtw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/geipdcgmx.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fktsv.cn/Article/details/gzqohlmbh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.sjlbkw.cn/Article/details/gldshiimb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.yfazqb.com/Article/details/gxfebduzm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.yfazqb.com/Article/details/gynwfvfdn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/ghsfgjikz.sHtML

[F11] 复制与移动文件
来源：http://read.share.sjlbkw.cn/Article/details/girpkwkwo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/gucvqaudk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.tarul.cn/Article/details/gabvlvosj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.vehdjk.com/Article/details/gqdwoixph.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.bbcook.cn/Article/details/gvxmiyidi.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.sjlbkw.cn/Article/details/ghvtfnvxr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fktsv.cn/Article/details/gvweqvqpu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/gukemurei.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.tarul.cn/Article/details/gdgnnnfxo.sHtML

[F12] CSV 读写
来源：http://www.share.yfazqb.com/Article/details/gkjioygwq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fktsv.cn/Article/details/gzcqpkzwd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.sjlbkw.cn/Article/details/gxiiiekoy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.tarul.cn/Article/details/glyavygfj.sHtML

TS:   // 同上
来源：http://3g.vehdjk.com/Article/details/gopbgufdc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fktsv.cn/Article/details/gnuddiefg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.bbcook.cn/Article/details/gnfxjivfj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fktsv.cn/Article/details/gwfmpvzod.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fktsv.cn/Article/details/gnvjsrsot.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gpynouazj.sHtML

G. 面向对象
来源：http://www.blog.vehdjk.com/Article/details/gkwjgvuxk.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gfktikrvx.sHtML

[G01] 定义类
来源：http://blog.vehdjk.com/Article/details/gqapggooy.sHtML

Py:   class User: pass
来源：http://www.m.share.epnwcf.com/Article/details/ggavkvdbl.sHtML

PHP:  class User {}
来源：http://m.share.tarul.cn/Article/details/gtrbjesql.sHtML

JS:   class User {}
来源：http://mobile.tarul.cn/Article/details/gceyjetbz.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.sjlbkw.cn/Article/details/gktylbczl.sHtML

Java: class User {}
来源：http://3g.epnwcf.com/Article/details/gbcjfsovf.sHtML

Go:   type User struct { Name string }
来源：http://blog.fktsv.cn/Article/details/gtdfaolvw.sHtML

Ruby: class User; end
来源：http://3g.vehdjk.com/Article/details/ggsrluzks.sHtML

C#:   class User {}
来源：http://wap.fktsv.cn/Article/details/gtpwyursx.sHtML

[G02] 构造函数
来源：http://wap.yfazqb.com/Article/details/gqgclqkze.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.sjlbkw.cn/Article/details/gxaplwdmg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.bbcook.cn/Article/details/giiwoldfb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fktsv.cn/Article/details/gqlholruf.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.epnwcf.com/Article/details/gsghgqkum.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fktsv.cn/Article/details/ggaymdtmm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.vehdjk.com/Article/details/ghwmisrqi.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.vehdjk.com/Article/details/gtbyrkvoq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.epnwcf.com/Article/details/gxyrjrczp.sHtML

[G03] 实例属性
来源：http://m.share.tarul.cn/Article/details/gwxpxlsno.sHtML

Py:   self.name = "x"
来源：http://3g.bbcook.cn/Article/details/gulfgkrzj.sHtML

PHP:  public string $name = "x";
来源：http://www.share.yfazqb.com/Article/details/gqsdbtccy.sHtML

JS:   this.name = "x";
来源：http://wap.fktsv.cn/Article/details/gppotozul.sHtML

TS:   name: string = "x";
来源：http://3g.vehdjk.com/Article/details/gcyguzprf.sHtML

Java: private String name;
来源：http://www.share.tarul.cn/Article/details/gdaqigbcb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.yfazqb.com/Article/details/gypkylwxa.sHtML

Ruby: @name = "x"
来源：http://mobile.yfazqb.com/Article/details/gwjlusnvf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.tarul.cn/Article/details/gekxrczbm.sHtML

[G04] 定义方法
来源：http://baike.sjlbkw.cn/Article/details/ghqinkocp.sHtML

Py:   def greet(self): return self.name
来源：http://3g.vehdjk.com/Article/details/ggugrxudf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.tarul.cn/Article/details/gewsrciko.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.bbcook.cn/Article/details/giveapryg.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.vehdjk.com/Article/details/glftpfiny.sHtML

Java: String greet() { return name; }
来源：http://3g.fktsv.cn/Article/details/ghpnqntmt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.sjlbkw.cn/Article/details/gjnevbjnv.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fktsv.cn/Article/details/gfepmfchb.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.bbcook.cn/Article/details/gudlqmkhp.sHtML

[G05] 继承
来源：http://www.share.bbcook.cn/Article/details/gnniikksu.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.bbcook.cn/Article/details/gzwllljsb.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.vehdjk.com/Article/details/ghphcabjm.sHtML

JS:   class Admin extends User {}
来源：http://blog.yfazqb.com/Article/details/gfmqlqhir.sHtML

TS:   class Admin extends User {}
来源：http://3g.sjlbkw.cn/Article/details/grkpiayte.sHtML

Java: class Admin extends User {}
来源：http://mobile.fktsv.cn/Article/details/gepifgzek.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fktsv.cn/Article/details/gacvdhmzk.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.bbcook.cn/Article/details/gegecvbsj.sHtML

C#:   class Admin : User {}
来源：http://3g.vehdjk.com/Article/details/gttycqjcd.sHtML

[G06] 重写方法
来源：http://read.share.epnwcf.com/Article/details/gizfbiwxv.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.vehdjk.com/Article/details/gdmorypdt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.vehdjk.com/Article/details/gbjegfuix.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.epnwcf.com/Article/details/gvpbsmdxz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.yfazqb.com/Article/details/grpakyyom.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.tarul.cn/Article/details/gfcxjaotc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.epnwcf.com/Article/details/giyijufyl.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fktsv.cn/Article/details/grlantyuf.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.vehdjk.com/Article/details/gbealgkeh.sHtML

[G07] 调用父类方法
来源：http://baike.fktsv.cn/Article/details/gqmzmpyzm.sHtML

Py:   super().greet()
来源：http://3g.yfazqb.com/Article/details/gyhrxiyqp.sHtML

PHP:  parent::greet();
来源：http://read.share.sjlbkw.cn/Article/details/gkujksexy.sHtML

JS:   super.greet();
来源：http://www.blog.sjlbkw.cn/Article/details/ghwfwnwks.sHtML

TS:   super.greet();
来源：http://www.share.epnwcf.com/Article/details/gzcrcwdwd.sHtML

Java: super.greet();
来源：http://m.share.yfazqb.com/Article/details/goqkgzxbe.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.bbcook.cn/Article/details/gagosepgi.sHtML

Ruby: super
来源：http://wap.epnwcf.com/Article/details/gzwzvielf.sHtML

C#:   base.Greet();
来源：http://baike.vehdjk.com/Article/details/gvexfqoqe.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.sjlbkw.cn/Article/details/gobupowcj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.bbcook.cn/Article/details/gtgfvdnvn.sHtML

PHP:  public static function f() {}
来源：http://baike.fktsv.cn/Article/details/gygmxvjdj.sHtML

JS:   static f() {}
来源：http://www.blog.fktsv.cn/Article/details/godzfucoh.sHtML

TS:   static f(): void {}
来源：http://www.blog.tarul.cn/Article/details/gmiczngyb.sHtML

Java: static void f() {}
来源：http://www.m.share.bbcook.cn/Article/details/gnxubdndq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.bbcook.cn/Article/details/gickbtkmm.sHtML

Ruby: def self.f; end
来源：http://blog.tarul.cn/Article/details/gmevsproc.sHtML

C#:   public static void F() {}
来源：http://3g.tarul.cn/Article/details/gxmcttmuz.sHtML

[G09] 接口 / 抽象类
来源：http://baike.sjlbkw.cn/Article/details/gspcffyzr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.sjlbkw.cn/Article/details/gtffksqkd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.epnwcf.com/Article/details/gepodueev.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.yfazqb.com/Article/details/glypacoht.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.epnwcf.com/Article/details/ggedfoiqi.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.vehdjk.com/Article/details/gmvqtsgcm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.yfazqb.com/Article/details/ghelkcztp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.bbcook.cn/Article/details/gdjlbmsyt.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gswsxcffk.sHtML

[G10] 访问控制
来源：http://m.share.fktsv.cn/Article/details/gmorhspns.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.sjlbkw.cn/Article/details/gartywuuv.sHtML

PHP:  public / protected / private
来源：http://read.share.yfazqb.com/Article/details/gxmoakdkd.sHtML

JS:   #private 字段；其余公开
来源：http://wap.sjlbkw.cn/Article/details/gulenpnqh.sHtML

TS:   public / protected / private
来源：http://blog.epnwcf.com/Article/details/gszzvnfwm.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.vehdjk.com/Article/details/gzwfkctin.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.vehdjk.com/Article/details/gpvmkcroj.sHtML

Ruby: public / protected / private
来源：http://www.m.share.yfazqb.com/Article/details/gwjspnvmj.sHtML

C#:   public / protected / private / internal
来源：http://blog.epnwcf.com/Article/details/gmeixgycd.sHtML

[G11] getter / setter
来源：http://www.share.vehdjk.com/Article/details/gpxileers.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.sjlbkw.cn/Article/details/gwcmpprfo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fktsv.cn/Article/details/gplzgjuio.sHtML

JS:   get name() { return this._name; }
来源：http://baike.vehdjk.com/Article/details/gaktwcoyc.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.sjlbkw.cn/Article/details/gdldsnphs.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcqrlncze.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.vehdjk.com/Article/details/gfgrvkotr.sHtML

Ruby: attr_accessor :name
来源：http://wap.epnwcf.com/Article/details/gldcypdjj.sHtML

C#:   public string Name { get; set; }
来源：http://baike.bbcook.cn/Article/details/gplrfxgfv.sHtML

[G12] 对象转字符串
来源：http://read.share.yfazqb.com/Article/details/gokhetmhh.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.vehdjk.com/Article/details/gwciqjrms.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fktsv.cn/Article/details/gbixszcsq.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.sjlbkw.cn/Article/details/gdptojdoi.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.epnwcf.com/Article/details/gphnmvwql.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.tarul.cn/Article/details/gavyjpvns.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.tarul.cn/Article/details/gsqhehnmx.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.bbcook.cn/Article/details/gnijcczkb.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.yfazqb.com/Article/details/gldqlqasy.sHtML

[G13] 判断对象类型
来源：http://www.blog.yfazqb.com/Article/details/gmujkairu.sHtML

Py:   isinstance(u, User)
来源：http://wap.sjlbkw.cn/Article/details/geihajpjt.sHtML

PHP:  $u instanceof User
来源：http://3g.fktsv.cn/Article/details/gilhadcku.sHtML

JS:   u instanceof User
来源：http://blog.epnwcf.com/Article/details/gojcmdwfk.sHtML

TS:   u instanceof User
来源：http://read.share.epnwcf.com/Article/details/gyzoslswl.sHtML

Java: u instanceof User
来源：http://mobile.fktsv.cn/Article/details/gxqtkimce.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.yfazqb.com/Article/details/gdiwzswqb.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.bbcook.cn/Article/details/gydgpbwtc.sHtML

C#:   u is User
来源：http://mobile.vehdjk.com/Article/details/gggahngdk.sHtML

[G14] 数据类 / record
来源：http://baike.epnwcf.com/Article/details/gxtxsxbid.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.epnwcf.com/Article/details/gbrwoqgri.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.vehdjk.com/Article/details/gglsrljnp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.tarul.cn/Article/details/gbuxelrzz.sHtML


<!-- 参考信息 -->