代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.epnwcf.com/Article/details/gexqdaaez.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.yfazqb.com/Article/details/gnlplaynt.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.vehdjk.com/Article/details/gvzvexwvy.sHtML

[E17] 首字母大写
来源：http://www.blog.yfazqb.com/Article/details/gqprfpnew.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.bbcook.cn/Article/details/ghlgymlee.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.bbcook.cn/Article/details/gvkzcunnl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fktsv.cn/Article/details/ghuojydlj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.tarul.cn/Article/details/gevsldtze.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.epnwcf.com/Article/details/gatayhrjd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.yfazqb.com/Article/details/gvmkrkwjn.sHtML

Ruby: s.capitalize
来源：http://3g.bbcook.cn/Article/details/gsywiolcm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.bbcook.cn/Article/details/ggorzkeuu.sHtML

[E18] 模板占位符替换
来源：http://m.share.bbcook.cn/Article/details/gyshlztfj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.yfazqb.com/Article/details/gtyklvobz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.epnwcf.com/Article/details/gadhjejin.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.epnwcf.com/Article/details/gekxjjepy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fktsv.cn/Article/details/gqmfnfgcn.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.tarul.cn/Article/details/gnstyzsfx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.epnwcf.com/Article/details/gbndocctr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.bbcook.cn/Article/details/gwlemxqel.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.sjlbkw.cn/Article/details/gyloweydo.sHtML

[E19] 多行文本按行拆分
来源：http://blog.yfazqb.com/Article/details/gzungiask.sHtML

Py:   s.splitlines()
来源：http://m.share.fktsv.cn/Article/details/ghjqzcypc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.yfazqb.com/Article/details/gpymbkdas.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.tarul.cn/Article/details/gsmrhomwr.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.vehdjk.com/Article/details/gvahzmefh.sHtML

Java: s.lines().toList()
来源：http://www.share.vehdjk.com/Article/details/giiwwjrxj.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.epnwcf.com/Article/details/gfqsghojk.sHtML

Ruby: s.lines
来源：http://m.share.sjlbkw.cn/Article/details/gogqrimzc.sHtML

C#:   s.Split('\n')
来源：http://blog.sjlbkw.cn/Article/details/gwtjzhwzd.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fktsv.cn/Article/details/gedhumckz.sHtML

Py:   if not s:
来源：http://blog.vehdjk.com/Article/details/gjrlwvsmp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.epnwcf.com/Article/details/grhxcbcmq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.epnwcf.com/Article/details/grvbuhulk.sHtML

TS:   if (s === "") {}
来源：http://www.blog.tarul.cn/Article/details/gjdzsanvo.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fktsv.cn/Article/details/ggdbdfxaq.sHtML

Go:   if s == "" {}
来源：http://mobile.bbcook.cn/Article/details/gtfcmqugc.sHtML

Ruby: if s.empty?
来源：http://m.share.tarul.cn/Article/details/gpspkwcng.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.fktsv.cn/Article/details/gwesheteg.sHtML

[E21] 超长截断加省略号
来源：http://m.share.tarul.cn/Article/details/grqbavbea.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.bbcook.cn/Article/details/gawcmpqxs.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gkmddxvxi.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fktsv.cn/Article/details/ghrjqewkk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.tarul.cn/Article/details/gmsdjtysn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.epnwcf.com/Article/details/gvgknllny.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fktsv.cn/Article/details/gahzbymel.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fktsv.cn/Article/details/gilsbmrjf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fktsv.cn/Article/details/gdetixaao.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.epnwcf.com/Article/details/gufewoura.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.yfazqb.com/Article/details/gpznpioav.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.bbcook.cn/Article/details/gwxyizuxl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.yfazqb.com/Article/details/ghzdgaofu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.yfazqb.com/Article/details/grpntkzfu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.bbcook.cn/Article/details/gfyvxiuxp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.bbcook.cn/Article/details/gjwrlxszf.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.sjlbkw.cn/Article/details/gcveijbtb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fktsv.cn/Article/details/gmmetatuh.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/ggrrwvqsb.sHtML

F. 文件与目录
来源：http://www.blog.fktsv.cn/Article/details/gmqereomt.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gjvucuudv.sHtML

[F01] 读取整个文件
来源：http://mobile.yfazqb.com/Article/details/gendgjqvi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.tarul.cn/Article/details/glhfklhbq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.vehdjk.com/Article/details/gjuvnjmhz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.yfazqb.com/Article/details/ghqdmiofq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.tarul.cn/Article/details/gnadklwco.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gofdhycti.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.tarul.cn/Article/details/gxkakdraz.sHtML

Ruby: File.read("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/glczmbwbm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fktsv.cn/Article/details/grumtxwmt.sHtML

[F02] 逐行读取文件
来源：http://mobile.tarul.cn/Article/details/guivrgsoz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.yfazqb.com/Article/details/gbjtevrqo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.vehdjk.com/Article/details/gpnkjffnp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.tarul.cn/Article/details/glooelthm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.bbcook.cn/Article/details/glakqmwkw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.sjlbkw.cn/Article/details/gjwvnuaza.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.bbcook.cn/Article/details/geexenkhn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.epnwcf.com/Article/details/gtofevnql.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.vehdjk.com/Article/details/gkdzjkuvd.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.epnwcf.com/Article/details/gfpfsynkh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.epnwcf.com/Article/details/gzditxxid.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.sjlbkw.cn/Article/details/gqicgirqk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.epnwcf.com/Article/details/gmelajnby.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.tarul.cn/Article/details/gsvkczkgn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.epnwcf.com/Article/details/gcgzwxeke.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.epnwcf.com/Article/details/gungajykm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.yfazqb.com/Article/details/gwbrwrely.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.epnwcf.com/Article/details/gkolsuzkh.sHtML

[F04] 追加写入文件
来源：http://mobile.sjlbkw.cn/Article/details/gpalmtbvf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.epnwcf.com/Article/details/grubvezyx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.vehdjk.com/Article/details/gjezpzmzq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.sjlbkw.cn/Article/details/ghzarqisa.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.epnwcf.com/Article/details/gupsfpxcu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.sjlbkw.cn/Article/details/gyootzhje.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.epnwcf.com/Article/details/gqxatrwaj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.tarul.cn/Article/details/gdkqjtjii.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.sjlbkw.cn/Article/details/gnoihopcb.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.yfazqb.com/Article/details/gmyxflrzh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.sjlbkw.cn/Article/details/gggrubfty.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.tarul.cn/Article/details/giarddzrr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fktsv.cn/Article/details/gfnqeobkm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fktsv.cn/Article/details/gdvpwnchw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.yfazqb.com/Article/details/gxzetzhzd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.sjlbkw.cn/Article/details/gvswiijol.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gqgcwptxk.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gydrqsuww.sHtML

[F06] 删除文件
来源：http://wap.fktsv.cn/Article/details/gtduqibmo.sHtML

Py:   os.remove("a.txt")
来源：http://blog.tarul.cn/Article/details/ggsernczy.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gozgbguoi.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gfwathkdy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.bbcook.cn/Article/details/gzudxxcju.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.yfazqb.com/Article/details/gtcalsoha.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gtzavaqex.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.vehdjk.com/Article/details/gfyyuvabt.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gtvzbkoml.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.epnwcf.com/Article/details/gnggdcimr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.yfazqb.com/Article/details/gypgjbnkt.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.epnwcf.com/Article/details/gxgwxfmsw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fktsv.cn/Article/details/goiqdgucq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.bbcook.cn/Article/details/ghvpkrxwn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.sjlbkw.cn/Article/details/gboyffrcu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.yfazqb.com/Article/details/gwghdjtlk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.vehdjk.com/Article/details/goczmrfet.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fktsv.cn/Article/details/godoufrjv.sHtML

[F08] 遍历目录
来源：http://read.share.fktsv.cn/Article/details/gjurhzbjq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.sjlbkw.cn/Article/details/gqayxukyg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.bbcook.cn/Article/details/gkmeyxtnb.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.vehdjk.com/Article/details/guksqhkcl.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.yfazqb.com/Article/details/gisvzoxcf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.epnwcf.com/Article/details/gsuxeejyz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.tarul.cn/Article/details/gytfgxlhd.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.yfazqb.com/Article/details/gfojrgoog.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.vehdjk.com/Article/details/granualrq.sHtML

[F09] 获取文件大小
来源：http://www.m.share.sjlbkw.cn/Article/details/gdwxwpbqw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gzzsknmpp.sHtML

PHP:  filesize("a.txt");
来源：http://wap.vehdjk.com/Article/details/gptxhwhmb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.bbcook.cn/Article/details/gkgcnwzbb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.vehdjk.com/Article/details/gimlutudx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.sjlbkw.cn/Article/details/gjymmakfx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.epnwcf.com/Article/details/ghtessczj.sHtML

Ruby: File.size("a.txt")
来源：http://3g.epnwcf.com/Article/details/gahtqlmyn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.yfazqb.com/Article/details/gwoajarjz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.sjlbkw.cn/Article/details/goxnxvhey.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gydcrdqde.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fktsv.cn/Article/details/grnfnblqh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.vehdjk.com/Article/details/gzjiucptu.sHtML

TS:   path.extname("a.txt")
来源：http://3g.tarul.cn/Article/details/gofhecikk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.sjlbkw.cn/Article/details/gyoajtpfk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gpsfmagjq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gqcrgodat.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/gnewlbmca.sHtML

[F11] 复制与移动文件
来源：http://blog.epnwcf.com/Article/details/gvqarutqh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.sjlbkw.cn/Article/details/gcouwrhnw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.vehdjk.com/Article/details/goxhocfyq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fktsv.cn/Article/details/gtyuntowq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fktsv.cn/Article/details/gmrdpicie.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.epnwcf.com/Article/details/gtisjignw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.yfazqb.com/Article/details/gerundrge.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.epnwcf.com/Article/details/gbwhjfnhl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.vehdjk.com/Article/details/gjqoqytcm.sHtML

[F12] CSV 读写
来源：http://baike.fktsv.cn/Article/details/gjqgnfiko.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.sjlbkw.cn/Article/details/gkdnrmgwy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.epnwcf.com/Article/details/gwsvaselu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.vehdjk.com/Article/details/gcffoeijh.sHtML

TS:   // 同上
来源：http://wap.epnwcf.com/Article/details/ghwgoueuw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.sjlbkw.cn/Article/details/gzjrhbegu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.bbcook.cn/Article/details/gmauedxnl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fktsv.cn/Article/details/gqtwggtlh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.yfazqb.com/Article/details/gxxxwrciw.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gsoyqidgp.sHtML

G. 面向对象
来源：http://www.m.share.tarul.cn/Article/details/gxvzwsrml.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gqzjfxful.sHtML

[G01] 定义类
来源：http://www.m.share.fktsv.cn/Article/details/gnymqgjma.sHtML

Py:   class User: pass
来源：http://read.share.tarul.cn/Article/details/gzixnnpxz.sHtML

PHP:  class User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gsviluwkb.sHtML

JS:   class User {}
来源：http://read.share.sjlbkw.cn/Article/details/ggefieevj.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.sjlbkw.cn/Article/details/gkwgrmgjp.sHtML

Java: class User {}
来源：http://www.blog.vehdjk.com/Article/details/gsgzrizhf.sHtML

Go:   type User struct { Name string }
来源：http://blog.vehdjk.com/Article/details/gtvbnzipf.sHtML

Ruby: class User; end
来源：http://m.share.vehdjk.com/Article/details/gjwamoksk.sHtML

C#:   class User {}
来源：http://3g.sjlbkw.cn/Article/details/gpddemccx.sHtML

[G02] 构造函数
来源：http://wap.tarul.cn/Article/details/gozribsrw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fktsv.cn/Article/details/gckoivwsi.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.tarul.cn/Article/details/ggwbmitwx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.sjlbkw.cn/Article/details/giojbtgta.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.tarul.cn/Article/details/gqhneuahs.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.bbcook.cn/Article/details/gqmwtzxyk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.sjlbkw.cn/Article/details/gecdkrusq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.vehdjk.com/Article/details/ggvkbmzsq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.bbcook.cn/Article/details/ghwxdjhoj.sHtML

[G03] 实例属性
来源：http://baike.fktsv.cn/Article/details/griohgzak.sHtML

Py:   self.name = "x"
来源：http://blog.fktsv.cn/Article/details/gsxmzfjdu.sHtML

PHP:  public string $name = "x";
来源：http://www.share.vehdjk.com/Article/details/gdjjerykd.sHtML

JS:   this.name = "x";
来源：http://m.share.vehdjk.com/Article/details/gcgtcoopr.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fktsv.cn/Article/details/gowzeweag.sHtML

Java: private String name;
来源：http://baike.sjlbkw.cn/Article/details/gtkawxarf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fktsv.cn/Article/details/gpczzpibi.sHtML

Ruby: @name = "x"
来源：http://www.blog.vehdjk.com/Article/details/gktyrymmo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.epnwcf.com/Article/details/gdfrhwjfm.sHtML

[G04] 定义方法
来源：http://www.blog.epnwcf.com/Article/details/gwotwivdn.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fktsv.cn/Article/details/gwwmhtnfo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.bbcook.cn/Article/details/gpwzohnhu.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.yfazqb.com/Article/details/gmvphzsqb.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/gmbmmydzx.sHtML

Java: String greet() { return name; }
来源：http://mobile.tarul.cn/Article/details/gffixzljv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.tarul.cn/Article/details/gshjecsfd.sHtML

Ruby: def greet; @name; end
来源：http://www.share.tarul.cn/Article/details/gjnpkoimj.sHtML

C#:   public string Greet() => Name;
来源：http://blog.bbcook.cn/Article/details/gpifevlih.sHtML

[G05] 继承
来源：http://baike.bbcook.cn/Article/details/glcgkjsqc.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.yfazqb.com/Article/details/grfkysboi.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.bbcook.cn/Article/details/gcxzjwldv.sHtML

JS:   class Admin extends User {}
来源：http://wap.sjlbkw.cn/Article/details/gzkizlwym.sHtML

TS:   class Admin extends User {}
来源：http://3g.epnwcf.com/Article/details/gulccsjtc.sHtML

Java: class Admin extends User {}
来源：http://m.share.sjlbkw.cn/Article/details/gwfvczebe.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.yfazqb.com/Article/details/gdfqlzznu.sHtML

Ruby: class Admin < User; end
来源：http://read.share.vehdjk.com/Article/details/gcbdrzjhq.sHtML

C#:   class Admin : User {}
来源：http://m.share.bbcook.cn/Article/details/ggsonijfi.sHtML

[G06] 重写方法
来源：http://wap.tarul.cn/Article/details/gewtqlyxz.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.tarul.cn/Article/details/gekjsrtdu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/ghypbsfxg.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.sjlbkw.cn/Article/details/gmqmgbhmi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.yfazqb.com/Article/details/gpdnsgxal.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.epnwcf.com/Article/details/gsxzzjomt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fktsv.cn/Article/details/gpddtefaj.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fktsv.cn/Article/details/gtjpnforq.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.epnwcf.com/Article/details/gtnshdzwb.sHtML

[G07] 调用父类方法
来源：http://wap.yfazqb.com/Article/details/gpkogikrx.sHtML

Py:   super().greet()
来源：http://read.share.sjlbkw.cn/Article/details/gqgsfsgcy.sHtML

PHP:  parent::greet();
来源：http://baike.bbcook.cn/Article/details/gltrkploc.sHtML

JS:   super.greet();
来源：http://read.share.sjlbkw.cn/Article/details/guqhhcnyu.sHtML

TS:   super.greet();
来源：http://read.share.yfazqb.com/Article/details/gdnghdaqa.sHtML

Java: super.greet();
来源：http://wap.fktsv.cn/Article/details/gkheaorpp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fktsv.cn/Article/details/grmbonhlh.sHtML

Ruby: super
来源：http://read.share.yfazqb.com/Article/details/gwvgledrm.sHtML

C#:   base.Greet();
来源：http://www.blog.vehdjk.com/Article/details/gsidknofi.sHtML

[G08] 静态方法与属性
来源：http://wap.yfazqb.com/Article/details/gcuqrcfyv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.vehdjk.com/Article/details/gzdolgynz.sHtML

PHP:  public static function f() {}
来源：http://blog.tarul.cn/Article/details/gpdoakpvf.sHtML

JS:   static f() {}
来源：http://www.share.yfazqb.com/Article/details/gkqhijcee.sHtML

TS:   static f(): void {}
来源：http://mobile.sjlbkw.cn/Article/details/gegdmvlqh.sHtML

Java: static void f() {}
来源：http://mobile.yfazqb.com/Article/details/gskghupul.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.sjlbkw.cn/Article/details/gkfabbakz.sHtML

Ruby: def self.f; end
来源：http://m.share.yfazqb.com/Article/details/gleatkfnj.sHtML

C#:   public static void F() {}
来源：http://read.share.sjlbkw.cn/Article/details/gfjsuzxxu.sHtML

[G09] 接口 / 抽象类
来源：http://baike.yfazqb.com/Article/details/gifoqramf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.sjlbkw.cn/Article/details/gtbypyinl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.tarul.cn/Article/details/gdrbbwqst.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.yfazqb.com/Article/details/gnlnlxxtk.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.vehdjk.com/Article/details/givhfhqss.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.bbcook.cn/Article/details/gwexjadyh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.epnwcf.com/Article/details/gfcgrdkad.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.sjlbkw.cn/Article/details/gnoouifgy.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.yfazqb.com/Article/details/goergqswn.sHtML

[G10] 访问控制
来源：http://3g.bbcook.cn/Article/details/guplovhpw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.epnwcf.com/Article/details/gbxofuazr.sHtML

PHP:  public / protected / private
来源：http://wap.fktsv.cn/Article/details/gyqtvtlea.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.tarul.cn/Article/details/ggsjgtcfm.sHtML

TS:   public / protected / private
来源：http://www.blog.sjlbkw.cn/Article/details/gcwunhlbs.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.tarul.cn/Article/details/gimlawull.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.bbcook.cn/Article/details/gpbzibziv.sHtML

Ruby: public / protected / private
来源：http://m.share.vehdjk.com/Article/details/gxibkxwsm.sHtML

C#:   public / protected / private / internal
来源：http://blog.tarul.cn/Article/details/gqszajvju.sHtML

[G11] getter / setter
来源：http://mobile.fktsv.cn/Article/details/goucpuirg.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.sjlbkw.cn/Article/details/ghnoasptz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.vehdjk.com/Article/details/gdbulwvvj.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fktsv.cn/Article/details/gqpnqooax.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.bbcook.cn/Article/details/gdwcrrmxc.sHtML

Java: public String getName() { return name; }
来源：http://mobile.yfazqb.com/Article/details/gtdpivdoe.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.bbcook.cn/Article/details/gbzejjusx.sHtML

Ruby: attr_accessor :name
来源：http://blog.vehdjk.com/Article/details/gomewjyte.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.epnwcf.com/Article/details/gjxupkxom.sHtML

[G12] 对象转字符串
来源：http://www.blog.vehdjk.com/Article/details/ggxxrjkrx.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.vehdjk.com/Article/details/gdfmwluur.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.tarul.cn/Article/details/gssibvjjc.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fktsv.cn/Article/details/gyaebadde.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fktsv.cn/Article/details/gohbvkpoe.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.yfazqb.com/Article/details/grznziyzt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.sjlbkw.cn/Article/details/ghxaxtkrl.sHtML

Ruby: def to_s; @name; end
来源：http://3g.tarul.cn/Article/details/guzmbjofz.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.epnwcf.com/Article/details/gfnbuseod.sHtML

[G13] 判断对象类型
来源：http://wap.sjlbkw.cn/Article/details/gidrncrno.sHtML

Py:   isinstance(u, User)
来源：http://blog.epnwcf.com/Article/details/gmgrkmclj.sHtML

PHP:  $u instanceof User
来源：http://www.share.fktsv.cn/Article/details/gavpbpiai.sHtML

JS:   u instanceof User
来源：http://baike.fktsv.cn/Article/details/gucgarplr.sHtML

TS:   u instanceof User
来源：http://blog.vehdjk.com/Article/details/gixjoihhv.sHtML

Java: u instanceof User
来源：http://wap.vehdjk.com/Article/details/gnbaavban.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.epnwcf.com/Article/details/gideccgyb.sHtML

Ruby: u.is_a?(User)
来源：http://baike.bbcook.cn/Article/details/goxacumjv.sHtML

C#:   u is User
来源：http://mobile.fktsv.cn/Article/details/gedxqmosl.sHtML

[G14] 数据类 / record
来源：http://www.blog.bbcook.cn/Article/details/gvbugihzy.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.bbcook.cn/Article/details/gqowzyktw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.vehdjk.com/Article/details/gtavkzggl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.yfazqb.com/Article/details/gsearrqgk.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.vehdjk.com/Article/details/gvdfpidpk.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.bbcook.cn/Article/details/gyhspqfyq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.vehdjk.com/Article/details/gehopeejf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.sjlbkw.cn/Article/details/gafnuzozc.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.vehdjk.com/Article/details/gufitcnpw.sHtML

[G15] 枚举
来源：http://www.share.yfazqb.com/Article/details/gskrwybtn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.yfazqb.com/Article/details/grldzxuhz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.vehdjk.com/Article/details/ggpvjkvew.sHtML


<!-- 参考信息 -->