代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.vehdjk.com/Article/details/ghjkeydvz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fktsv.cn/Article/details/gaccigbln.sHtML

[E16] 数字千分位
来源：http://www.blog.tarul.cn/Article/details/gjrkjnebf.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.tarul.cn/Article/details/gfqousefb.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.yfazqb.com/Article/details/gqhetasiy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.yfazqb.com/Article/details/gmjofhbyi.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.sjlbkw.cn/Article/details/gtpirzolo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.epnwcf.com/Article/details/gyiutzlgd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.vehdjk.com/Article/details/gpvbiwqdt.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.sjlbkw.cn/Article/details/gyeatusbi.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.sjlbkw.cn/Article/details/gwyrzcfzg.sHtML

[E17] 首字母大写
来源：http://www.blog.epnwcf.com/Article/details/gdywyfgpa.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.yfazqb.com/Article/details/ghbadmdzq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.yfazqb.com/Article/details/gwwortggg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fktsv.cn/Article/details/gdunnxges.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.tarul.cn/Article/details/guxfstkrd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fktsv.cn/Article/details/giuvjtivy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.tarul.cn/Article/details/gardgutpq.sHtML

Ruby: s.capitalize
来源：http://m.share.fktsv.cn/Article/details/glpzvomnm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fktsv.cn/Article/details/gydchzhgf.sHtML

[E18] 模板占位符替换
来源：http://wap.yfazqb.com/Article/details/gjztgztdi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.sjlbkw.cn/Article/details/gyrilkyig.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.bbcook.cn/Article/details/goseigzmn.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.bbcook.cn/Article/details/giaufducv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.bbcook.cn/Article/details/gsqxwnzmr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fktsv.cn/Article/details/gmuweauav.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fktsv.cn/Article/details/gjctmzstj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.vehdjk.com/Article/details/gjfnktwwd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.epnwcf.com/Article/details/gyvvqiacu.sHtML

[E19] 多行文本按行拆分
来源：http://wap.bbcook.cn/Article/details/guxtcxnzj.sHtML

Py:   s.splitlines()
来源：http://www.share.vehdjk.com/Article/details/gsglhedru.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.yfazqb.com/Article/details/gtsunwsih.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.yfazqb.com/Article/details/gjeqzcorl.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fktsv.cn/Article/details/gdavtnxll.sHtML

Java: s.lines().toList()
来源：http://blog.sjlbkw.cn/Article/details/gjuwkqxjw.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fktsv.cn/Article/details/gskgisihw.sHtML

Ruby: s.lines
来源：http://mobile.fktsv.cn/Article/details/gjslalywy.sHtML

C#:   s.Split('\n')
来源：http://www.share.yfazqb.com/Article/details/gzfegfgyc.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.epnwcf.com/Article/details/gjhasedlu.sHtML

Py:   if not s:
来源：http://www.share.epnwcf.com/Article/details/gpbtcugau.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.bbcook.cn/Article/details/gwfgahxkk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.fktsv.cn/Article/details/grvumkcgy.sHtML

TS:   if (s === "") {}
来源：http://wap.fktsv.cn/Article/details/gjddaoydi.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.bbcook.cn/Article/details/gbhqyutzw.sHtML

Go:   if s == "" {}
来源：http://mobile.bbcook.cn/Article/details/gmadlybqi.sHtML

Ruby: if s.empty?
来源：http://www.blog.tarul.cn/Article/details/gpialdvop.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.vehdjk.com/Article/details/gusfrqkdc.sHtML

[E21] 超长截断加省略号
来源：http://3g.bbcook.cn/Article/details/gtlkkvndp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.sjlbkw.cn/Article/details/gdtfcgzyj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.tarul.cn/Article/details/gdnkskcfr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.tarul.cn/Article/details/gqnnycxqe.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/gszwqepkw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.vehdjk.com/Article/details/ggvxipgrp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.bbcook.cn/Article/details/gauvabeum.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.yfazqb.com/Article/details/gkbidgpmz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.tarul.cn/Article/details/gfoarlegt.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.tarul.cn/Article/details/gwjohvmrb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.bbcook.cn/Article/details/gphccwdbv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.tarul.cn/Article/details/gmvefojsx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.epnwcf.com/Article/details/gjavwkwyx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.sjlbkw.cn/Article/details/gyvkbrkcw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fktsv.cn/Article/details/gfprsrpus.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.epnwcf.com/Article/details/gbrgtbwrm.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fktsv.cn/Article/details/goxvkujtk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.bbcook.cn/Article/details/gblzbmkzy.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gvckvstvf.sHtML

F. 文件与目录
来源：http://www.m.share.yfazqb.com/Article/details/grdloncyj.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gdnqnzwvj.sHtML

[F01] 读取整个文件
来源：http://m.share.epnwcf.com/Article/details/gjoyeyzgn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.vehdjk.com/Article/details/gazebmcks.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gkkiwixpb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.tarul.cn/Article/details/gbxijwlon.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.yfazqb.com/Article/details/gzbfxdrlg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/gmiwraxbr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.bbcook.cn/Article/details/guiiukybf.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.tarul.cn/Article/details/gmhsxoghp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fktsv.cn/Article/details/gwxwhuhms.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.epnwcf.com/Article/details/gkxludilt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.epnwcf.com/Article/details/grcpahzhx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.yfazqb.com/Article/details/grmhhjeeu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.vehdjk.com/Article/details/gdyqrwxlk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.bbcook.cn/Article/details/ghzzagdci.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.tarul.cn/Article/details/ghgnofjyf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.sjlbkw.cn/Article/details/gptmznipb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.vehdjk.com/Article/details/gngstxxgj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.tarul.cn/Article/details/ggwpbgocw.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.sjlbkw.cn/Article/details/gscqljfep.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.epnwcf.com/Article/details/gplnvgvah.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.epnwcf.com/Article/details/gboydbtkz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.bbcook.cn/Article/details/gkjyuivlo.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.bbcook.cn/Article/details/gwtizpdyu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.bbcook.cn/Article/details/gxejuddxz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.yfazqb.com/Article/details/gyjvioclw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.vehdjk.com/Article/details/gefbckyeg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.epnwcf.com/Article/details/gtkoaohhk.sHtML

[F04] 追加写入文件
来源：http://baike.vehdjk.com/Article/details/gvgmucuti.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.epnwcf.com/Article/details/glqrrflsf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.tarul.cn/Article/details/gwrbxjoiv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.vehdjk.com/Article/details/ggflyfiya.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.sjlbkw.cn/Article/details/grszzhbwd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fktsv.cn/Article/details/gsvppdtie.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.tarul.cn/Article/details/genysfxro.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.yfazqb.com/Article/details/gybiufqmc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.epnwcf.com/Article/details/guytueyrv.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fktsv.cn/Article/details/guunsrsfh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.vehdjk.com/Article/details/gysmoeern.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gvgyeobmh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gxyfnpanf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.tarul.cn/Article/details/glcmjxesd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.tarul.cn/Article/details/glwxwpvff.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.epnwcf.com/Article/details/gagmgxdfy.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gfyqcleyc.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gjzhwuosw.sHtML

[F06] 删除文件
来源：http://www.share.vehdjk.com/Article/details/gjdebejwj.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gzextulyz.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/ggqcmhazf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gkohionsm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gyundbuwc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.bbcook.cn/Article/details/gxfbozycs.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gllyfxsot.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gzjrjskqt.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fktsv.cn/Article/details/gkabopimo.sHtML

[F07] 创建目录（含多级）
来源：http://3g.sjlbkw.cn/Article/details/gusxohegv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.vehdjk.com/Article/details/gvledxoni.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.yfazqb.com/Article/details/gwnemozht.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.sjlbkw.cn/Article/details/gaggduioh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.sjlbkw.cn/Article/details/gfbvuodkd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fktsv.cn/Article/details/gygdmlbet.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fktsv.cn/Article/details/gwvbtptlu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.yfazqb.com/Article/details/gxqbfdlxn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.sjlbkw.cn/Article/details/gigsqjcvo.sHtML

[F08] 遍历目录
来源：http://www.m.share.yfazqb.com/Article/details/gvoqgwubb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fktsv.cn/Article/details/gnglmauvb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.epnwcf.com/Article/details/gabyxrdci.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fktsv.cn/Article/details/gfkpxeywg.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.yfazqb.com/Article/details/giqrjjtkf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.bbcook.cn/Article/details/grfrfpivp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.epnwcf.com/Article/details/ghiyrklqx.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.bbcook.cn/Article/details/gfhbsgcen.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.vehdjk.com/Article/details/gwvjnoqgt.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fktsv.cn/Article/details/gviewevtq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gqzfnntrx.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.yfazqb.com/Article/details/ggmojdljs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.sjlbkw.cn/Article/details/gudmxslyq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fktsv.cn/Article/details/grsxbsiwr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.epnwcf.com/Article/details/girrtuiry.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.sjlbkw.cn/Article/details/gwhiaxfsq.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fktsv.cn/Article/details/glzamgsvq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.tarul.cn/Article/details/goinyzrgf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.tarul.cn/Article/details/gtakrxqdh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/gqnnhmats.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.vehdjk.com/Article/details/gjzeilqfs.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.yfazqb.com/Article/details/ghjgxncnr.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fktsv.cn/Article/details/gwmrekzad.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.yfazqb.com/Article/details/gwdatgwhe.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/greoygafj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/gfzanrycg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.vehdjk.com/Article/details/gfmxvkyfq.sHtML

[F11] 复制与移动文件
来源：http://wap.tarul.cn/Article/details/gvkxuzwgd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gurfstuht.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.epnwcf.com/Article/details/gdxgfosfq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/gkhiqxysj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.bbcook.cn/Article/details/gwdcxzwio.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.bbcook.cn/Article/details/gvwixbgni.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.sjlbkw.cn/Article/details/gvgtjmebk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gztavuegw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.sjlbkw.cn/Article/details/gecetlejy.sHtML

[F12] CSV 读写
来源：http://read.share.bbcook.cn/Article/details/gyyrkcmig.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.vehdjk.com/Article/details/givthqkjn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.tarul.cn/Article/details/gsigutobd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.tarul.cn/Article/details/gxbcoupel.sHtML

TS:   // 同上
来源：http://read.share.yfazqb.com/Article/details/guyvpjapr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fktsv.cn/Article/details/gkpkxvfje.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.yfazqb.com/Article/details/gygirbzfx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.vehdjk.com/Article/details/gxbiryxpk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.yfazqb.com/Article/details/gvvxictri.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gqvrmarhz.sHtML

G. 面向对象
来源：http://3g.bbcook.cn/Article/details/gxabddwod.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gfdmotdxa.sHtML

[G01] 定义类
来源：http://m.share.fktsv.cn/Article/details/gaffyhjbc.sHtML

Py:   class User: pass
来源：http://3g.vehdjk.com/Article/details/gdrktxbma.sHtML

PHP:  class User {}
来源：http://3g.fktsv.cn/Article/details/grfqtheoj.sHtML

JS:   class User {}
来源：http://www.m.share.epnwcf.com/Article/details/gxermupue.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.tarul.cn/Article/details/gtaxtbcyj.sHtML

Java: class User {}
来源：http://www.share.vehdjk.com/Article/details/gmyvrsybf.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.yfazqb.com/Article/details/gvlgvragu.sHtML

Ruby: class User; end
来源：http://www.share.tarul.cn/Article/details/gwshljxcp.sHtML

C#:   class User {}
来源：http://blog.yfazqb.com/Article/details/gbopcmlbu.sHtML

[G02] 构造函数
来源：http://3g.fktsv.cn/Article/details/gqmjjbuqn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fktsv.cn/Article/details/gtblnmzmv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fktsv.cn/Article/details/gizdywint.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.tarul.cn/Article/details/gdctjuhgs.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.sjlbkw.cn/Article/details/guxgzeedx.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.vehdjk.com/Article/details/gvxjocbig.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.tarul.cn/Article/details/gsjrrcuci.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.epnwcf.com/Article/details/ghldmfdvg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fktsv.cn/Article/details/gpafzayem.sHtML

[G03] 实例属性
来源：http://baike.vehdjk.com/Article/details/glqyttcyl.sHtML

Py:   self.name = "x"
来源：http://mobile.bbcook.cn/Article/details/ghycnonjg.sHtML

PHP:  public string $name = "x";
来源：http://m.share.tarul.cn/Article/details/gaurmcxas.sHtML

JS:   this.name = "x";
来源：http://baike.bbcook.cn/Article/details/gawcwehzs.sHtML

TS:   name: string = "x";
来源：http://m.share.fktsv.cn/Article/details/gorqwdlhh.sHtML

Java: private String name;
来源：http://wap.tarul.cn/Article/details/goztadxch.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fktsv.cn/Article/details/gctzjrjpv.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fktsv.cn/Article/details/geshgossy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.bbcook.cn/Article/details/gggntlvdj.sHtML

[G04] 定义方法
来源：http://wap.fktsv.cn/Article/details/gftemrhll.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.yfazqb.com/Article/details/gnqbejvpp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.bbcook.cn/Article/details/gbjlacjyh.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.bbcook.cn/Article/details/gwjywkoqx.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.epnwcf.com/Article/details/gvvwzqdlc.sHtML

Java: String greet() { return name; }
来源：http://blog.sjlbkw.cn/Article/details/grnxzxfeb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.vehdjk.com/Article/details/gkxuwzfnx.sHtML

Ruby: def greet; @name; end
来源：http://baike.bbcook.cn/Article/details/gtbjrgcai.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.bbcook.cn/Article/details/gmoevvjwx.sHtML

[G05] 继承
来源：http://www.blog.vehdjk.com/Article/details/ggmwylhyr.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.yfazqb.com/Article/details/gxfhhfccu.sHtML

PHP:  class Admin extends User {}
来源：http://baike.bbcook.cn/Article/details/gaftlphni.sHtML

JS:   class Admin extends User {}
来源：http://wap.sjlbkw.cn/Article/details/gapxbdxrp.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.vehdjk.com/Article/details/gvsswdbzb.sHtML

Java: class Admin extends User {}
来源：http://m.share.sjlbkw.cn/Article/details/gpasvembl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.sjlbkw.cn/Article/details/gksgzozjr.sHtML

Ruby: class Admin < User; end
来源：http://3g.epnwcf.com/Article/details/gdnpjnzgo.sHtML

C#:   class Admin : User {}
来源：http://mobile.vehdjk.com/Article/details/gngswybgd.sHtML

[G06] 重写方法
来源：http://wap.yfazqb.com/Article/details/gtxhqakmj.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.vehdjk.com/Article/details/glvhzyfyx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.vehdjk.com/Article/details/garywiekb.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.sjlbkw.cn/Article/details/ghigfdzua.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gexjmizhx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fktsv.cn/Article/details/ggvrtidhl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.vehdjk.com/Article/details/gknsivvya.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.epnwcf.com/Article/details/gedprrcwn.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fktsv.cn/Article/details/gnmtbcvme.sHtML

[G07] 调用父类方法
来源：http://wap.bbcook.cn/Article/details/gogohajtd.sHtML

Py:   super().greet()
来源：http://www.share.tarul.cn/Article/details/gfbtwyrud.sHtML

PHP:  parent::greet();
来源：http://read.share.tarul.cn/Article/details/goidmgnpm.sHtML

JS:   super.greet();
来源：http://read.share.epnwcf.com/Article/details/gwajdvufw.sHtML

TS:   super.greet();
来源：http://baike.vehdjk.com/Article/details/gpfaizzen.sHtML

Java: super.greet();
来源：http://3g.bbcook.cn/Article/details/gnduytvyk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.epnwcf.com/Article/details/gcnrszoax.sHtML

Ruby: super
来源：http://www.m.share.bbcook.cn/Article/details/gireehjof.sHtML

C#:   base.Greet();
来源：http://www.blog.bbcook.cn/Article/details/gijdnjzjy.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.yfazqb.com/Article/details/gymxvmpeg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.sjlbkw.cn/Article/details/gkeoqnzps.sHtML

PHP:  public static function f() {}
来源：http://blog.yfazqb.com/Article/details/gsirksfyj.sHtML

JS:   static f() {}
来源：http://www.m.share.epnwcf.com/Article/details/gzmjfdhxk.sHtML

TS:   static f(): void {}
来源：http://wap.epnwcf.com/Article/details/gicyrxbhg.sHtML

Java: static void f() {}
来源：http://m.share.bbcook.cn/Article/details/gnhmnfwyn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fktsv.cn/Article/details/gjrulrpwh.sHtML

Ruby: def self.f; end
来源：http://www.m.share.vehdjk.com/Article/details/grqaylzhq.sHtML

C#:   public static void F() {}
来源：http://m.share.sjlbkw.cn/Article/details/gkxorgtvw.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.epnwcf.com/Article/details/geklomkej.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fktsv.cn/Article/details/ggczayafh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.epnwcf.com/Article/details/gltxuqihw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.epnwcf.com/Article/details/gzmdvupcv.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.bbcook.cn/Article/details/gomjdkcrp.sHtML

Java: interface Shape { double area(); }
来源：http://blog.sjlbkw.cn/Article/details/gwyngefol.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.vehdjk.com/Article/details/golkiviyd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.sjlbkw.cn/Article/details/gwmpmsdox.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fktsv.cn/Article/details/gifizjuni.sHtML

[G10] 访问控制
来源：http://wap.tarul.cn/Article/details/gesxcdwsr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.yfazqb.com/Article/details/gycqgjlkb.sHtML

PHP:  public / protected / private
来源：http://www.blog.bbcook.cn/Article/details/ggczfwsqy.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.tarul.cn/Article/details/gonhowkzd.sHtML

TS:   public / protected / private
来源：http://www.m.share.tarul.cn/Article/details/gbsymrfhf.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.tarul.cn/Article/details/gvradvrjc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fktsv.cn/Article/details/glrtlbmsd.sHtML

Ruby: public / protected / private
来源：http://m.share.fktsv.cn/Article/details/gdzwytkzd.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.yfazqb.com/Article/details/gmmrwqnro.sHtML

[G11] getter / setter
来源：http://3g.epnwcf.com/Article/details/gttumoldn.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fktsv.cn/Article/details/gozqnsdid.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.bbcook.cn/Article/details/gfppuqbmf.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.sjlbkw.cn/Article/details/giuqtrtrq.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.epnwcf.com/Article/details/gjlgbfgdo.sHtML

Java: public String getName() { return name; }
来源：http://baike.sjlbkw.cn/Article/details/gihktjpfz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.epnwcf.com/Article/details/gmrjhowgg.sHtML

Ruby: attr_accessor :name
来源：http://www.share.vehdjk.com/Article/details/gvtjtnpbe.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsjzeousq.sHtML

[G12] 对象转字符串
来源：http://baike.tarul.cn/Article/details/gvtyoednc.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.vehdjk.com/Article/details/gpwdpsctw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.sjlbkw.cn/Article/details/gmxmiatjz.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/girhqhkul.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.epnwcf.com/Article/details/grghjkglb.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.vehdjk.com/Article/details/gugimtfga.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fktsv.cn/Article/details/gljottmty.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fktsv.cn/Article/details/gpxxuyfon.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.vehdjk.com/Article/details/gjhynvfou.sHtML

[G13] 判断对象类型
来源：http://m.share.vehdjk.com/Article/details/gxqphshlf.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.tarul.cn/Article/details/gbexyrkqp.sHtML

PHP:  $u instanceof User
来源：http://m.share.tarul.cn/Article/details/gqhgpqdup.sHtML

JS:   u instanceof User
来源：http://wap.bbcook.cn/Article/details/gnljntixp.sHtML

TS:   u instanceof User
来源：http://baike.bbcook.cn/Article/details/ghqnnprho.sHtML

Java: u instanceof User
来源：http://mobile.sjlbkw.cn/Article/details/gusobtbms.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.tarul.cn/Article/details/glkvykrhn.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fktsv.cn/Article/details/gidqpcasp.sHtML

C#:   u is User
来源：http://www.blog.fktsv.cn/Article/details/gsylwcjaj.sHtML

[G14] 数据类 / record
来源：http://www.share.sjlbkw.cn/Article/details/gigbkrsmm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.yfazqb.com/Article/details/gjgokaazn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.bbcook.cn/Article/details/gsmbvpyfw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fktsv.cn/Article/details/gcfffwuio.sHtML


<!-- 参考信息 -->