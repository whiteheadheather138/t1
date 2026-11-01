代发 wailian999

PHP:  number_format(1234567);
来源：http://www.blog.vehdjk.com/Article/details/gyuokcnaf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.yfazqb.com/Article/details/gnviebpep.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.bbcook.cn/Article/details/gvdfvugdb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.epnwcf.com/Article/details/gdnvklttj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.tarul.cn/Article/details/ggmuhpugh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fktsv.cn/Article/details/gbdvefgrf.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.vehdjk.com/Article/details/gacafrmom.sHtML

[E17] 首字母大写
来源：http://m.share.epnwcf.com/Article/details/ggixvmitx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.tarul.cn/Article/details/gqnwfwxqc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.bbcook.cn/Article/details/gqecnyueb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.vehdjk.com/Article/details/ggxcgodiw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fktsv.cn/Article/details/gksjwknwz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fktsv.cn/Article/details/gwfalahsy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.vehdjk.com/Article/details/grgaqjuix.sHtML

Ruby: s.capitalize
来源：http://3g.tarul.cn/Article/details/gnaensgzz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fktsv.cn/Article/details/gemfjljio.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.bbcook.cn/Article/details/gktjpveir.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.vehdjk.com/Article/details/gqwcarehu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.epnwcf.com/Article/details/gqgjbvrxn.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.tarul.cn/Article/details/gygnsacgk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.epnwcf.com/Article/details/gubbpatbh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.bbcook.cn/Article/details/gnikjndmm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.bbcook.cn/Article/details/gzhkrgczh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.vehdjk.com/Article/details/gfruhjwty.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.sjlbkw.cn/Article/details/gssihhxbx.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.epnwcf.com/Article/details/gvbirwfsg.sHtML

Py:   s.splitlines()
来源：http://wap.epnwcf.com/Article/details/glsaljvbg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.sjlbkw.cn/Article/details/glakfhwmi.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.vehdjk.com/Article/details/gmlnlaojn.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.vehdjk.com/Article/details/gorpqnwzx.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fktsv.cn/Article/details/ggjazmthe.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.yfazqb.com/Article/details/gyonhepya.sHtML

Ruby: s.lines
来源：http://3g.sjlbkw.cn/Article/details/gloaxuhsg.sHtML

C#:   s.Split('\n')
来源：http://read.share.bbcook.cn/Article/details/gafujclsl.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fktsv.cn/Article/details/gznbcxavv.sHtML

Py:   if not s:
来源：http://mobile.epnwcf.com/Article/details/goqiiuqxd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.sjlbkw.cn/Article/details/gqctpufew.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.tarul.cn/Article/details/golizhqxn.sHtML

TS:   if (s === "") {}
来源：http://www.share.sjlbkw.cn/Article/details/glxgkpcky.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.bbcook.cn/Article/details/gfgasbucl.sHtML

Go:   if s == "" {}
来源：http://www.m.share.vehdjk.com/Article/details/gnhstreof.sHtML

Ruby: if s.empty?
来源：http://m.share.bbcook.cn/Article/details/grxhicfef.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.tarul.cn/Article/details/gluxemimq.sHtML

[E21] 超长截断加省略号
来源：http://3g.sjlbkw.cn/Article/details/gjbvxkepd.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.yfazqb.com/Article/details/gamsbuyce.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/gaqayipmn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.yfazqb.com/Article/details/gpcgpnhzk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.yfazqb.com/Article/details/gucdovvhe.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.fktsv.cn/Article/details/gyoijwxpb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.bbcook.cn/Article/details/gryecjnpm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fktsv.cn/Article/details/gwqdwjzmv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.tarul.cn/Article/details/gbrdbbdxe.sHtML

[E22] 字节长度与字符长度
来源：http://baike.epnwcf.com/Article/details/ghdkgvqbx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gtlzfgjmb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.epnwcf.com/Article/details/grgqxxbin.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.vehdjk.com/Article/details/govslykry.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.vehdjk.com/Article/details/gdujtfhng.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.sjlbkw.cn/Article/details/gdjfclzul.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.yfazqb.com/Article/details/gxjetgzap.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.vehdjk.com/Article/details/gjiilvgrm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.vehdjk.com/Article/details/guygnoitu.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gmbgdgpex.sHtML

F. 文件与目录
来源：http://www.m.share.sjlbkw.cn/Article/details/gwkzxwhnr.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gkqwfydzj.sHtML

[F01] 读取整个文件
来源：http://www.blog.bbcook.cn/Article/details/gslmygkaq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.vehdjk.com/Article/details/gxnmvarra.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gakwpmmlb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fktsv.cn/Article/details/gburzloof.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fktsv.cn/Article/details/ganuzbwod.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.epnwcf.com/Article/details/gdlmhqgps.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fktsv.cn/Article/details/gqykqetmz.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gftnzyasf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gihmmzhmg.sHtML

[F02] 逐行读取文件
来源：http://blog.epnwcf.com/Article/details/ggnxqqfbo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.vehdjk.com/Article/details/gcqfbxwut.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.epnwcf.com/Article/details/gilaaafca.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.tarul.cn/Article/details/glneubijq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.epnwcf.com/Article/details/gjwzyruxo.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.epnwcf.com/Article/details/gejmypizu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.bbcook.cn/Article/details/gmpnxubnj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.vehdjk.com/Article/details/galnajryi.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.sjlbkw.cn/Article/details/gitzfcmjh.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fktsv.cn/Article/details/gsdwqcxtg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.tarul.cn/Article/details/gyhfnggvm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.bbcook.cn/Article/details/gjkidrycg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.tarul.cn/Article/details/gciryewei.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.yfazqb.com/Article/details/gdqbkfjbf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.bbcook.cn/Article/details/gokplkwyc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.tarul.cn/Article/details/ghvxmfamp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.bbcook.cn/Article/details/gqvjwjuho.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.vehdjk.com/Article/details/gkmxcgbkm.sHtML

[F04] 追加写入文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gicszsdwc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.sjlbkw.cn/Article/details/gpftcopkt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.vehdjk.com/Article/details/gvigmzpqa.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.tarul.cn/Article/details/gqylwxnoq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.yfazqb.com/Article/details/gamgkhrkf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.epnwcf.com/Article/details/gmhxiphns.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.vehdjk.com/Article/details/gxohkybsd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.epnwcf.com/Article/details/gtctpaurm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.sjlbkw.cn/Article/details/gmmclmmqq.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.epnwcf.com/Article/details/gepvhhxxi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.yfazqb.com/Article/details/gmhizodjc.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gzzhhwdfi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.tarul.cn/Article/details/gewopyuue.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/ggvkvwmao.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.sjlbkw.cn/Article/details/gfikgroma.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.vehdjk.com/Article/details/goautzixc.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.tarul.cn/Article/details/guncjdedx.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.epnwcf.com/Article/details/gkxyrysjx.sHtML

[F06] 删除文件
来源：http://mobile.tarul.cn/Article/details/ggxirgbwf.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/ghggltybt.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.yfazqb.com/Article/details/grjlpvezv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.tarul.cn/Article/details/gfukjiafw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.vehdjk.com/Article/details/ggyekwqng.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.sjlbkw.cn/Article/details/gqwfrknfv.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.vehdjk.com/Article/details/gnhwrjimk.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gspxyfqux.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fktsv.cn/Article/details/gumtwytkp.sHtML

[F07] 创建目录（含多级）
来源：http://wap.bbcook.cn/Article/details/ggvineipc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.bbcook.cn/Article/details/gkntlyllv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.sjlbkw.cn/Article/details/gjjddykpx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fktsv.cn/Article/details/ghwpninkz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.vehdjk.com/Article/details/gitybnjcs.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.vehdjk.com/Article/details/gqctjdaqe.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.sjlbkw.cn/Article/details/gxvgdgtgc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.vehdjk.com/Article/details/ggrpzdbnj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.sjlbkw.cn/Article/details/gmqijumzp.sHtML

[F08] 遍历目录
来源：http://blog.tarul.cn/Article/details/gvyfjrsgv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.bbcook.cn/Article/details/gcskgzwmr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.yfazqb.com/Article/details/gacnbitkh.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.epnwcf.com/Article/details/gstoapgzq.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fktsv.cn/Article/details/ggyjrlbju.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.yfazqb.com/Article/details/gevevuogh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.yfazqb.com/Article/details/gabpfedvc.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fktsv.cn/Article/details/gshlcljlu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.yfazqb.com/Article/details/gwoilihyz.sHtML

[F09] 获取文件大小
来源：http://3g.yfazqb.com/Article/details/gsenfmxfc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gqeghfukz.sHtML

PHP:  filesize("a.txt");
来源：http://wap.epnwcf.com/Article/details/gqucrieet.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.sjlbkw.cn/Article/details/gizydxkka.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.epnwcf.com/Article/details/gwxuzgykj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fktsv.cn/Article/details/gdncfznio.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.vehdjk.com/Article/details/gobxzqkmi.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gyzomlglz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.yfazqb.com/Article/details/gmqmwkvrx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.sjlbkw.cn/Article/details/glxtxakwq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/gtukdgfdy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/ghyeoedwv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/gzfbfurpu.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmomawdvq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.vehdjk.com/Article/details/gkwgiyrbb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gxdoqsdsm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/gxnzbbjti.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/gkjfxvsjg.sHtML

[F11] 复制与移动文件
来源：http://wap.yfazqb.com/Article/details/gwebysesm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.tarul.cn/Article/details/gtkeanxmz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.tarul.cn/Article/details/gegdrueta.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.epnwcf.com/Article/details/gsinoerzf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fktsv.cn/Article/details/gcvejhinn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.tarul.cn/Article/details/gcvahtzjb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.bbcook.cn/Article/details/ggtdqeezn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.tarul.cn/Article/details/gcjlzsfia.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.epnwcf.com/Article/details/goibfmald.sHtML

[F12] CSV 读写
来源：http://www.m.share.fktsv.cn/Article/details/gazxqkmvu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.tarul.cn/Article/details/gplqxmmvi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.yfazqb.com/Article/details/gspulyadk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fktsv.cn/Article/details/gfqwfdxut.sHtML

TS:   // 同上
来源：http://blog.bbcook.cn/Article/details/gcagranzs.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.vehdjk.com/Article/details/gswfvsjtq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.sjlbkw.cn/Article/details/gllhvbfby.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.bbcook.cn/Article/details/gyhhrteev.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.bbcook.cn/Article/details/gjfghausp.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gubsggcra.sHtML

G. 面向对象
来源：http://www.blog.fktsv.cn/Article/details/gfiqhpaks.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/genmygjpz.sHtML

[G01] 定义类
来源：http://m.share.tarul.cn/Article/details/ghrbzfrnj.sHtML

Py:   class User: pass
来源：http://m.share.tarul.cn/Article/details/gfsvkbmpz.sHtML

PHP:  class User {}
来源：http://www.m.share.epnwcf.com/Article/details/gcjtspnzh.sHtML

JS:   class User {}
来源：http://www.m.share.fktsv.cn/Article/details/gquxjdech.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fktsv.cn/Article/details/gmnuanifz.sHtML

Java: class User {}
来源：http://read.share.yfazqb.com/Article/details/gcgwlwetd.sHtML

Go:   type User struct { Name string }
来源：http://wap.fktsv.cn/Article/details/gjpgzpohj.sHtML

Ruby: class User; end
来源：http://m.share.epnwcf.com/Article/details/gwqvjnrmp.sHtML

C#:   class User {}
来源：http://www.share.bbcook.cn/Article/details/gkmmeylmb.sHtML

[G02] 构造函数
来源：http://www.blog.yfazqb.com/Article/details/gqiltjdvg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.sjlbkw.cn/Article/details/gnxfayytu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.tarul.cn/Article/details/guheznnrq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.tarul.cn/Article/details/gqnyezwdz.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fktsv.cn/Article/details/gckgixeea.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.epnwcf.com/Article/details/gcsloepop.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.tarul.cn/Article/details/gmpmmmpuw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.yfazqb.com/Article/details/gegiknzxn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.vehdjk.com/Article/details/gmuobibtu.sHtML

[G03] 实例属性
来源：http://mobile.vehdjk.com/Article/details/grtwniohj.sHtML

Py:   self.name = "x"
来源：http://www.m.share.yfazqb.com/Article/details/giddsbcue.sHtML

PHP:  public string $name = "x";
来源：http://blog.yfazqb.com/Article/details/gkgfmtchn.sHtML

JS:   this.name = "x";
来源：http://mobile.epnwcf.com/Article/details/gqifczigb.sHtML

TS:   name: string = "x";
来源：http://read.share.bbcook.cn/Article/details/gldcsnaas.sHtML

Java: private String name;
来源：http://baike.bbcook.cn/Article/details/gafwuwomx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.sjlbkw.cn/Article/details/gnshkgrzx.sHtML

Ruby: @name = "x"
来源：http://www.blog.tarul.cn/Article/details/gzowyjbdy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.vehdjk.com/Article/details/gaebphxhr.sHtML

[G04] 定义方法
来源：http://www.blog.fktsv.cn/Article/details/gwdpxfntk.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.bbcook.cn/Article/details/ghifnipoi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.yfazqb.com/Article/details/geellxiep.sHtML

JS:   greet() { return this.name; }
来源：http://baike.sjlbkw.cn/Article/details/gkewcompm.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.bbcook.cn/Article/details/gmgtrlpgt.sHtML

Java: String greet() { return name; }
来源：http://www.blog.yfazqb.com/Article/details/gndzwwqou.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.tarul.cn/Article/details/gxzxrgpyw.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.yfazqb.com/Article/details/gmjssctcp.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.yfazqb.com/Article/details/gbclbgbjg.sHtML

[G05] 继承
来源：http://blog.bbcook.cn/Article/details/gixidnotr.sHtML

Py:   class Admin(User): pass
来源：http://3g.tarul.cn/Article/details/gfpqeomuq.sHtML

PHP:  class Admin extends User {}
来源：http://wap.sjlbkw.cn/Article/details/gqusblfgt.sHtML

JS:   class Admin extends User {}
来源：http://3g.tarul.cn/Article/details/gqhtshvyq.sHtML

TS:   class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/gzseinkvs.sHtML

Java: class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/gnoebrhqv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.yfazqb.com/Article/details/gcfjqcabe.sHtML

Ruby: class Admin < User; end
来源：http://3g.fktsv.cn/Article/details/gsvtluenu.sHtML

C#:   class Admin : User {}
来源：http://m.share.fktsv.cn/Article/details/gweebkljt.sHtML

[G06] 重写方法
来源：http://wap.tarul.cn/Article/details/geovraunb.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.tarul.cn/Article/details/gntcusjmv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.bbcook.cn/Article/details/geovhxfxr.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.epnwcf.com/Article/details/gltokkwub.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.bbcook.cn/Article/details/ggfcvdggn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.sjlbkw.cn/Article/details/gywbfvzse.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.vehdjk.com/Article/details/grontjylj.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.yfazqb.com/Article/details/gxafeociy.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.tarul.cn/Article/details/gzshtkamh.sHtML

[G07] 调用父类方法
来源：http://read.share.vehdjk.com/Article/details/gcbwikmcf.sHtML

Py:   super().greet()
来源：http://mobile.bbcook.cn/Article/details/gbvmvdlck.sHtML

PHP:  parent::greet();
来源：http://m.share.yfazqb.com/Article/details/gyszbbghg.sHtML

JS:   super.greet();
来源：http://www.share.yfazqb.com/Article/details/gehwudait.sHtML

TS:   super.greet();
来源：http://m.share.yfazqb.com/Article/details/gosyjwpil.sHtML

Java: super.greet();
来源：http://wap.sjlbkw.cn/Article/details/gcfaoofti.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.epnwcf.com/Article/details/gzszxmkaz.sHtML

Ruby: super
来源：http://baike.fktsv.cn/Article/details/gvfjkodgd.sHtML

C#:   base.Greet();
来源：http://wap.yfazqb.com/Article/details/gcpplofnm.sHtML

[G08] 静态方法与属性
来源：http://www.share.yfazqb.com/Article/details/gvqzbtgol.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.sjlbkw.cn/Article/details/gagwxojqk.sHtML

PHP:  public static function f() {}
来源：http://3g.bbcook.cn/Article/details/gmiumhfft.sHtML

JS:   static f() {}
来源：http://read.share.tarul.cn/Article/details/gubjlaqfu.sHtML

TS:   static f(): void {}
来源：http://m.share.bbcook.cn/Article/details/gmlnzfqfq.sHtML

Java: static void f() {}
来源：http://blog.yfazqb.com/Article/details/gypklqlsp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.bbcook.cn/Article/details/gahedvpdz.sHtML

Ruby: def self.f; end
来源：http://3g.epnwcf.com/Article/details/gmlaieiee.sHtML

C#:   public static void F() {}
来源：http://read.share.tarul.cn/Article/details/gbsseopie.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.epnwcf.com/Article/details/gxyjsgdlb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.vehdjk.com/Article/details/gddzvtzke.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.bbcook.cn/Article/details/gtmztacap.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.bbcook.cn/Article/details/gzzrjkzhe.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.tarul.cn/Article/details/gzmfprswy.sHtML

Java: interface Shape { double area(); }
来源：http://wap.vehdjk.com/Article/details/gvnmoixum.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.yfazqb.com/Article/details/grvwbxbye.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.epnwcf.com/Article/details/gltkxfcao.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.bbcook.cn/Article/details/gzsrnnvhw.sHtML

[G10] 访问控制
来源：http://3g.vehdjk.com/Article/details/gknlvuspf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.yfazqb.com/Article/details/gizkzupgv.sHtML

PHP:  public / protected / private
来源：http://blog.yfazqb.com/Article/details/gzjoiaygs.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fktsv.cn/Article/details/gisvewxor.sHtML

TS:   public / protected / private
来源：http://wap.tarul.cn/Article/details/gqhudplwp.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.yfazqb.com/Article/details/gogpqwsmb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.sjlbkw.cn/Article/details/gehntqdao.sHtML

Ruby: public / protected / private
来源：http://mobile.yfazqb.com/Article/details/gcnessnpc.sHtML

C#:   public / protected / private / internal
来源：http://m.share.epnwcf.com/Article/details/gwoijidww.sHtML

[G11] getter / setter
来源：http://blog.fktsv.cn/Article/details/gavrpreif.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.epnwcf.com/Article/details/ghxbqfrwz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.tarul.cn/Article/details/grciyvetr.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.epnwcf.com/Article/details/gzcyadwgl.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.epnwcf.com/Article/details/gvnqvmqoo.sHtML

Java: public String getName() { return name; }
来源：http://www.share.bbcook.cn/Article/details/giczfuqkg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.sjlbkw.cn/Article/details/gcgiruwgt.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.bbcook.cn/Article/details/gxxroaruf.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.vehdjk.com/Article/details/goplijjnp.sHtML

[G12] 对象转字符串
来源：http://www.share.vehdjk.com/Article/details/guloyxmub.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.bbcook.cn/Article/details/gcktcefoj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.yfazqb.com/Article/details/gxnxwboga.sHtML

JS:   toString() { return this.name; }
来源：http://3g.tarul.cn/Article/details/geuibkajd.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.vehdjk.com/Article/details/gyqhjpdiw.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fktsv.cn/Article/details/gbphclufy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fktsv.cn/Article/details/gttcsjatt.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fktsv.cn/Article/details/gfhsmdsjg.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.bbcook.cn/Article/details/gxiocnsxs.sHtML

[G13] 判断对象类型
来源：http://www.share.tarul.cn/Article/details/gesbuibya.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.sjlbkw.cn/Article/details/geeoydzkv.sHtML

PHP:  $u instanceof User
来源：http://baike.fktsv.cn/Article/details/gknwxjfjj.sHtML

JS:   u instanceof User
来源：http://www.m.share.epnwcf.com/Article/details/gfakjrlcr.sHtML

TS:   u instanceof User
来源：http://www.m.share.vehdjk.com/Article/details/gbwimcqqu.sHtML

Java: u instanceof User
来源：http://m.share.sjlbkw.cn/Article/details/glmqzyggk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.vehdjk.com/Article/details/gctwadywj.sHtML

Ruby: u.is_a?(User)
来源：http://blog.epnwcf.com/Article/details/guojlaklc.sHtML

C#:   u is User
来源：http://mobile.epnwcf.com/Article/details/gwotzlnhw.sHtML

[G14] 数据类 / record
来源：http://mobile.vehdjk.com/Article/details/gpskczbhe.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.epnwcf.com/Article/details/gppjiryww.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.yfazqb.com/Article/details/gnkzbefby.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fktsv.cn/Article/details/gswgbydxf.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.epnwcf.com/Article/details/gpnqopysx.sHtML

Java: record User(String name, int age) {}
来源：http://blog.epnwcf.com/Article/details/gybdpepsj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.yfazqb.com/Article/details/gczhtnlqm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fktsv.cn/Article/details/gbdlqmvmm.sHtML


<!-- 参考信息 -->