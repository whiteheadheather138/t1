代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.sjlbkw.cn/Article/details/gmmiarrhi.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.tarul.cn/Article/details/gisdaursb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.yfazqb.com/Article/details/gdwndpmpz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.yfazqb.com/Article/details/gwsemfckg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.vehdjk.com/Article/details/gcmxgouri.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.vehdjk.com/Article/details/gyouwgwgm.sHtML

[E16] 数字千分位
来源：http://read.share.epnwcf.com/Article/details/gyirbdtql.sHtML

Py:   f"{1234567:,}"
来源：http://blog.tarul.cn/Article/details/gvnjaxpji.sHtML

PHP:  number_format(1234567);
来源：http://www.share.tarul.cn/Article/details/gjanfrapv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.sjlbkw.cn/Article/details/gwjzepltr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.sjlbkw.cn/Article/details/gqnxbijum.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.epnwcf.com/Article/details/gkvezqozv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.yfazqb.com/Article/details/gyikroynm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.yfazqb.com/Article/details/gdrawddss.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.bbcook.cn/Article/details/gdylhqcyu.sHtML

[E17] 首字母大写
来源：http://m.share.yfazqb.com/Article/details/gyljvwozk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.vehdjk.com/Article/details/gfyirgjdq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.bbcook.cn/Article/details/gfhlwyfea.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/grdlhzrrv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.vehdjk.com/Article/details/gaxazvxqj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.sjlbkw.cn/Article/details/guxsygcyp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.vehdjk.com/Article/details/glpujuflx.sHtML

Ruby: s.capitalize
来源：http://baike.tarul.cn/Article/details/gxhysvveq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.vehdjk.com/Article/details/gpusztqpx.sHtML

[E18] 模板占位符替换
来源：http://blog.sjlbkw.cn/Article/details/giiwowhiw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.sjlbkw.cn/Article/details/gbgktevth.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.yfazqb.com/Article/details/gbepbhguw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.tarul.cn/Article/details/ghmzjqcth.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.sjlbkw.cn/Article/details/gfjbzyrjg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fktsv.cn/Article/details/gcmzzqack.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvqqkzipn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fktsv.cn/Article/details/gtjbzrsos.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gqnepvtuu.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.epnwcf.com/Article/details/gsyfiawvs.sHtML

Py:   s.splitlines()
来源：http://blog.tarul.cn/Article/details/gkxzcnmum.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.epnwcf.com/Article/details/gurppszqb.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.sjlbkw.cn/Article/details/gjhpphirp.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.vehdjk.com/Article/details/grtdebjjd.sHtML

Java: s.lines().toList()
来源：http://3g.fktsv.cn/Article/details/ghhetbiad.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.vehdjk.com/Article/details/gygwqamxh.sHtML

Ruby: s.lines
来源：http://mobile.sjlbkw.cn/Article/details/gethiqwwk.sHtML

C#:   s.Split('\n')
来源：http://3g.epnwcf.com/Article/details/givtrfsic.sHtML

[E20] 判断字符串是否为空
来源：http://wap.tarul.cn/Article/details/gtnbktnec.sHtML

Py:   if not s:
来源：http://wap.tarul.cn/Article/details/gzcjpayfw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.tarul.cn/Article/details/gppipxkkv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.epnwcf.com/Article/details/gtwdfgsri.sHtML

TS:   if (s === "") {}
来源：http://baike.fktsv.cn/Article/details/gzmbbqfqk.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.vehdjk.com/Article/details/gptzjyxmi.sHtML

Go:   if s == "" {}
来源：http://www.blog.vehdjk.com/Article/details/gcikxugch.sHtML

Ruby: if s.empty?
来源：http://m.share.bbcook.cn/Article/details/gckksyzms.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.epnwcf.com/Article/details/gscktmymw.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.bbcook.cn/Article/details/gqevlfiqo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.epnwcf.com/Article/details/gqsvgpllr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gdckntiye.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fktsv.cn/Article/details/gjxpiynel.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.vehdjk.com/Article/details/grjrstfwk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fktsv.cn/Article/details/gpjzwqlqv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.sjlbkw.cn/Article/details/gyyzvfhds.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.tarul.cn/Article/details/gsaacxwdv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.yfazqb.com/Article/details/gyulfozpt.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.epnwcf.com/Article/details/ghxvvupjb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.vehdjk.com/Article/details/gicpdgqvv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.epnwcf.com/Article/details/gvxlpenln.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.sjlbkw.cn/Article/details/gunzqkuvh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.sjlbkw.cn/Article/details/gbapsdwht.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.epnwcf.com/Article/details/guhixjxim.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fktsv.cn/Article/details/gmjtzgflz.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.vehdjk.com/Article/details/gxtdqbiro.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fktsv.cn/Article/details/gwqechpfd.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gqlgtpzqb.sHtML

F. 文件与目录
来源：http://blog.tarul.cn/Article/details/gafleqmcy.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gtvyhkdoc.sHtML

[F01] 读取整个文件
来源：http://wap.vehdjk.com/Article/details/gdbvngvof.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.yfazqb.com/Article/details/glvcmadbx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gmmqcfzhd.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.epnwcf.com/Article/details/gwsxtvwzj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.bbcook.cn/Article/details/gbkhjbokk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.tarul.cn/Article/details/glzlhebud.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.vehdjk.com/Article/details/gopcnanmn.sHtML

Ruby: File.read("a.txt")
来源：http://blog.bbcook.cn/Article/details/gldgwmdtj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.tarul.cn/Article/details/gvbctoxux.sHtML

[F02] 逐行读取文件
来源：http://wap.fktsv.cn/Article/details/gptklihzs.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fktsv.cn/Article/details/gmtoiagbc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.vehdjk.com/Article/details/gcztgmxpp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.bbcook.cn/Article/details/gjrpqbxzs.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.bbcook.cn/Article/details/gpmholfny.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.bbcook.cn/Article/details/gkmyvidqe.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.yfazqb.com/Article/details/gpyjtnbid.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.yfazqb.com/Article/details/gbgkvzxuu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.tarul.cn/Article/details/gvhqnuhkx.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.yfazqb.com/Article/details/gmmwowsnj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.bbcook.cn/Article/details/goanzqwbq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.epnwcf.com/Article/details/gxcfvfohs.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fktsv.cn/Article/details/gyictyxwp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.yfazqb.com/Article/details/grelcqurb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fktsv.cn/Article/details/gxjroebjf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxdphssxo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fktsv.cn/Article/details/gxjtljybu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.tarul.cn/Article/details/gvlxfwzta.sHtML

[F04] 追加写入文件
来源：http://blog.yfazqb.com/Article/details/gvybjifvn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.epnwcf.com/Article/details/gggeubsbl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fktsv.cn/Article/details/grawgjgpj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.tarul.cn/Article/details/ggaajfgom.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.vehdjk.com/Article/details/gcrdofvtx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.yfazqb.com/Article/details/gckrsvohp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.yfazqb.com/Article/details/gresnpnae.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.vehdjk.com/Article/details/gkqlujhjm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.epnwcf.com/Article/details/gxicydlmr.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.yfazqb.com/Article/details/gmvahfeuq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.epnwcf.com/Article/details/gqcqrwpsw.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fktsv.cn/Article/details/gokvvjlao.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gfpfrntgg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.yfazqb.com/Article/details/gyuxlsprt.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.bbcook.cn/Article/details/gsxndgxnq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.yfazqb.com/Article/details/geoqbhiqr.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gitlslhqa.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gumdpzimd.sHtML

[F06] 删除文件
来源：http://3g.yfazqb.com/Article/details/gayafuxbl.sHtML

Py:   os.remove("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gturfxgdy.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gebncuucy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.vehdjk.com/Article/details/gdzbaqcma.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gzuzxxwbh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.sjlbkw.cn/Article/details/gzedpsrkb.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.vehdjk.com/Article/details/ggtfcmfyd.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gsaybszgt.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gcjhnyewh.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fktsv.cn/Article/details/gnequfvor.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.epnwcf.com/Article/details/gwrzqzprm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.fktsv.cn/Article/details/gspbonwvs.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.vehdjk.com/Article/details/gsyjcakct.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.sjlbkw.cn/Article/details/gkzqoazqn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.sjlbkw.cn/Article/details/gqldaukab.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.epnwcf.com/Article/details/gfoqqjayo.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.bbcook.cn/Article/details/gjnsyxrbk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.yfazqb.com/Article/details/gollqhccr.sHtML

[F08] 遍历目录
来源：http://read.share.tarul.cn/Article/details/guxpsxmsi.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.tarul.cn/Article/details/gipnzxicz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.epnwcf.com/Article/details/gjfbhddii.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.bbcook.cn/Article/details/gllsemsil.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.vehdjk.com/Article/details/gusozckzu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.bbcook.cn/Article/details/gtvffspye.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.vehdjk.com/Article/details/gptgsylob.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.vehdjk.com/Article/details/gktldtuyr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/gohnbzycs.sHtML

[F09] 获取文件大小
来源：http://wap.sjlbkw.cn/Article/details/guxmvheku.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gdztilczf.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gtqwqqiiu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fktsv.cn/Article/details/gklqazbwg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.epnwcf.com/Article/details/glpskoonu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fktsv.cn/Article/details/goisxentt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.vehdjk.com/Article/details/gjbkzeugo.sHtML

Ruby: File.size("a.txt")
来源：http://3g.bbcook.cn/Article/details/gnslmmjah.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.epnwcf.com/Article/details/guiuifhud.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.epnwcf.com/Article/details/gmfnypcdj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/gwcjtaenf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.vehdjk.com/Article/details/gwmrpojvw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gczphwtza.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.tarul.cn/Article/details/grbcztcqj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.vehdjk.com/Article/details/gythrzanu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fktsv.cn/Article/details/gswxdwrhs.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gutojnubq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/glwgxqdla.sHtML

[F11] 复制与移动文件
来源：http://www.blog.bbcook.cn/Article/details/ggeogegto.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.tarul.cn/Article/details/gdrgjwgum.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.yfazqb.com/Article/details/gkekgzrap.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.epnwcf.com/Article/details/ggbiewwwe.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/gzxoilfsw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.sjlbkw.cn/Article/details/gcxynrjrq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.yfazqb.com/Article/details/gbhpkhixk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.bbcook.cn/Article/details/gwygpkjxp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.yfazqb.com/Article/details/gzipuafnw.sHtML

[F12] CSV 读写
来源：http://mobile.epnwcf.com/Article/details/gjqkhscql.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.yfazqb.com/Article/details/gouyajvar.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.yfazqb.com/Article/details/gdcjkwtmy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.yfazqb.com/Article/details/gznrqwpzb.sHtML

TS:   // 同上
来源：http://mobile.yfazqb.com/Article/details/gxkxvplhj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.sjlbkw.cn/Article/details/gzbmitnzd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.yfazqb.com/Article/details/gqvjbxzki.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fktsv.cn/Article/details/gxfcgyacs.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.vehdjk.com/Article/details/gqxbpxcbr.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gxfxqzxpl.sHtML

G. 面向对象
来源：http://wap.epnwcf.com/Article/details/gzxbflyhx.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gkmuhaeoq.sHtML

[G01] 定义类
来源：http://www.share.fktsv.cn/Article/details/geytcyvfv.sHtML

Py:   class User: pass
来源：http://mobile.vehdjk.com/Article/details/gmxnocoir.sHtML

PHP:  class User {}
来源：http://m.share.fktsv.cn/Article/details/gkuwlbdxy.sHtML

JS:   class User {}
来源：http://www.m.share.yfazqb.com/Article/details/gvuobngev.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fktsv.cn/Article/details/gxxwjtmvb.sHtML

Java: class User {}
来源：http://baike.tarul.cn/Article/details/gdjgkqyrp.sHtML

Go:   type User struct { Name string }
来源：http://mobile.vehdjk.com/Article/details/gklxkughm.sHtML

Ruby: class User; end
来源：http://www.share.vehdjk.com/Article/details/goyejpcgv.sHtML

C#:   class User {}
来源：http://3g.fktsv.cn/Article/details/grxfbtdee.sHtML

[G02] 构造函数
来源：http://www.blog.yfazqb.com/Article/details/gpbfwtqtq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.bbcook.cn/Article/details/gnhyyklms.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fktsv.cn/Article/details/gsbfhchow.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.tarul.cn/Article/details/gyeljzvhi.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.bbcook.cn/Article/details/gtmczbpyh.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fktsv.cn/Article/details/guyvvficm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.vehdjk.com/Article/details/gewncnquw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.tarul.cn/Article/details/gbmymrgmg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.yfazqb.com/Article/details/gqxmouayt.sHtML

[G03] 实例属性
来源：http://blog.sjlbkw.cn/Article/details/gimobhmvv.sHtML

Py:   self.name = "x"
来源：http://www.share.tarul.cn/Article/details/glmmzzobq.sHtML

PHP:  public string $name = "x";
来源：http://m.share.sjlbkw.cn/Article/details/glexazpha.sHtML

JS:   this.name = "x";
来源：http://read.share.sjlbkw.cn/Article/details/garfwwaji.sHtML

TS:   name: string = "x";
来源：http://m.share.sjlbkw.cn/Article/details/gywxjxgkn.sHtML

Java: private String name;
来源：http://www.blog.bbcook.cn/Article/details/gcnjamvuk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.sjlbkw.cn/Article/details/gfzvtondx.sHtML

Ruby: @name = "x"
来源：http://read.share.bbcook.cn/Article/details/gtllidwzq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.vehdjk.com/Article/details/gflunrcur.sHtML

[G04] 定义方法
来源：http://wap.epnwcf.com/Article/details/gnakyewii.sHtML

Py:   def greet(self): return self.name
来源：http://3g.tarul.cn/Article/details/gjnosnrth.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.yfazqb.com/Article/details/gojbwttmm.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.tarul.cn/Article/details/gdvnfytaa.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/gzkxtpyaa.sHtML

Java: String greet() { return name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gvvixkbcf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.tarul.cn/Article/details/ghkprrmow.sHtML

Ruby: def greet; @name; end
来源：http://baike.tarul.cn/Article/details/gmgjybjrj.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.epnwcf.com/Article/details/gjcpvhifj.sHtML

[G05] 继承
来源：http://blog.vehdjk.com/Article/details/gygymbois.sHtML

Py:   class Admin(User): pass
来源：http://baike.vehdjk.com/Article/details/glofruapp.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.epnwcf.com/Article/details/gnhdpnuvm.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.vehdjk.com/Article/details/gybreuoia.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fktsv.cn/Article/details/gulwefxau.sHtML

Java: class Admin extends User {}
来源：http://www.blog.epnwcf.com/Article/details/gxydsycmf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.tarul.cn/Article/details/gdqxkxzcu.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gphbflsbn.sHtML

C#:   class Admin : User {}
来源：http://www.share.epnwcf.com/Article/details/gaqxnnlmp.sHtML

[G06] 重写方法
来源：http://blog.sjlbkw.cn/Article/details/gazgcsjld.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.sjlbkw.cn/Article/details/gyyojxmmf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fktsv.cn/Article/details/gtqiwcysb.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gdvxvqaso.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.tarul.cn/Article/details/gxmgnnklr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.yfazqb.com/Article/details/gmlfulwrh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.sjlbkw.cn/Article/details/gaeepvmvs.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fktsv.cn/Article/details/gawlhncxm.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.sjlbkw.cn/Article/details/gosqgtzra.sHtML

[G07] 调用父类方法
来源：http://baike.tarul.cn/Article/details/gihdtiwqa.sHtML

Py:   super().greet()
来源：http://www.blog.tarul.cn/Article/details/gnvjbfgpi.sHtML

PHP:  parent::greet();
来源：http://m.share.sjlbkw.cn/Article/details/gzzluaskt.sHtML

JS:   super.greet();
来源：http://m.share.bbcook.cn/Article/details/gqvzqjthx.sHtML

TS:   super.greet();
来源：http://3g.sjlbkw.cn/Article/details/gukgytpve.sHtML

Java: super.greet();
来源：http://mobile.vehdjk.com/Article/details/guzxkxytc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.epnwcf.com/Article/details/glullkjik.sHtML

Ruby: super
来源：http://mobile.vehdjk.com/Article/details/gifjgfgmx.sHtML

C#:   base.Greet();
来源：http://mobile.yfazqb.com/Article/details/ginayfcuz.sHtML

[G08] 静态方法与属性
来源：http://3g.epnwcf.com/Article/details/geiixnegu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.vehdjk.com/Article/details/ghqfeccfy.sHtML

PHP:  public static function f() {}
来源：http://wap.tarul.cn/Article/details/grsezqtpg.sHtML

JS:   static f() {}
来源：http://m.share.epnwcf.com/Article/details/gfyvqbxuc.sHtML

TS:   static f(): void {}
来源：http://mobile.sjlbkw.cn/Article/details/gfvimcojz.sHtML

Java: static void f() {}
来源：http://www.m.share.vehdjk.com/Article/details/gbpcxmedq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.tarul.cn/Article/details/gqcjoxust.sHtML

Ruby: def self.f; end
来源：http://www.blog.epnwcf.com/Article/details/gvsrcslfb.sHtML

C#:   public static void F() {}
来源：http://m.share.sjlbkw.cn/Article/details/gcwgfuqcg.sHtML

[G09] 接口 / 抽象类
来源：http://blog.yfazqb.com/Article/details/grxighptl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.tarul.cn/Article/details/gcbcpvhxq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.tarul.cn/Article/details/gbdtkdotf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.bbcook.cn/Article/details/ghynpjibi.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.vehdjk.com/Article/details/gbrucgszi.sHtML

Java: interface Shape { double area(); }
来源：http://3g.sjlbkw.cn/Article/details/gmoqvrqbh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fktsv.cn/Article/details/gsggealok.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fktsv.cn/Article/details/gytbjxdss.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.epnwcf.com/Article/details/ggyzvyttp.sHtML

[G10] 访问控制
来源：http://3g.bbcook.cn/Article/details/gnebscfgv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.epnwcf.com/Article/details/gixoqmdjt.sHtML

PHP:  public / protected / private
来源：http://www.blog.epnwcf.com/Article/details/gqipchyoh.sHtML

JS:   #private 字段；其余公开
来源：http://wap.vehdjk.com/Article/details/gvjzizyyq.sHtML

TS:   public / protected / private
来源：http://m.share.yfazqb.com/Article/details/gthbufmer.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fktsv.cn/Article/details/grzqndhuv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.sjlbkw.cn/Article/details/gtyxkbuub.sHtML

Ruby: public / protected / private
来源：http://3g.epnwcf.com/Article/details/gvokanihi.sHtML

C#:   public / protected / private / internal
来源：http://blog.vehdjk.com/Article/details/gwhftifrb.sHtML

[G11] getter / setter
来源：http://blog.tarul.cn/Article/details/gqgubscrm.sHtML

Py:   @property 与 @x.setter
来源：http://baike.bbcook.cn/Article/details/gfpezcnxf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.yfazqb.com/Article/details/gcolakvbi.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.vehdjk.com/Article/details/gpztiiooa.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.sjlbkw.cn/Article/details/gcshtqajt.sHtML

Java: public String getName() { return name; }
来源：http://blog.yfazqb.com/Article/details/gkmwlorbx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.tarul.cn/Article/details/ggtkukuwa.sHtML

Ruby: attr_accessor :name
来源：http://baike.fktsv.cn/Article/details/govgezcsg.sHtML

C#:   public string Name { get; set; }
来源：http://blog.yfazqb.com/Article/details/gdkfohshq.sHtML

[G12] 对象转字符串
来源：http://blog.fktsv.cn/Article/details/glfzsmqgv.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.vehdjk.com/Article/details/gjjisecyz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gzxxfgtzt.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.sjlbkw.cn/Article/details/gshtmafwl.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.yfazqb.com/Article/details/gnzuefbvm.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gbqrkkqqw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.bbcook.cn/Article/details/gfakdmgyz.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.epnwcf.com/Article/details/gblvkjhkt.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.tarul.cn/Article/details/gypeblass.sHtML

[G13] 判断对象类型
来源：http://m.share.fktsv.cn/Article/details/gomnxrbjx.sHtML

Py:   isinstance(u, User)
来源：http://mobile.tarul.cn/Article/details/geusanysk.sHtML

PHP:  $u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/gxzqexzti.sHtML

JS:   u instanceof User
来源：http://www.m.share.fktsv.cn/Article/details/gwncgwhjv.sHtML

TS:   u instanceof User
来源：http://blog.fktsv.cn/Article/details/gqvlllhab.sHtML

Java: u instanceof User
来源：http://www.share.epnwcf.com/Article/details/gnplrrhuw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.bbcook.cn/Article/details/gbnnmxdfm.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.yfazqb.com/Article/details/glhpmokdg.sHtML

C#:   u is User
来源：http://www.blog.vehdjk.com/Article/details/gclvrejua.sHtML


<!-- 参考信息 -->