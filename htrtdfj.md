代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.epnwcf.com/Article/details/gnhgyfqcb.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.epnwcf.com/Article/details/gptbmrfjl.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.vehdjk.com/Article/details/gicxppfti.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.bbcook.cn/Article/details/gtwduvgnc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.epnwcf.com/Article/details/gelmnoaus.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.bbcook.cn/Article/details/gbubnqvpj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.bbcook.cn/Article/details/gisvplixl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.vehdjk.com/Article/details/gqiotablk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.yfazqb.com/Article/details/gsdrnsxlc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fktsv.cn/Article/details/gogocvmai.sHtML

[E16] 数字千分位
来源：http://read.share.bbcook.cn/Article/details/gpghxutuj.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.bbcook.cn/Article/details/gtxxjiear.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.yfazqb.com/Article/details/gbpzyrkad.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.bbcook.cn/Article/details/gnxkowbqh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.vehdjk.com/Article/details/gjfxasivp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.yfazqb.com/Article/details/gsbtatoii.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.bbcook.cn/Article/details/gnveqewot.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.epnwcf.com/Article/details/gzcoubrah.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.vehdjk.com/Article/details/gilznlgrq.sHtML

[E17] 首字母大写
来源：http://m.share.vehdjk.com/Article/details/gotqxskbg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.tarul.cn/Article/details/gxlabjziu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.yfazqb.com/Article/details/gjhxwlcyx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.bbcook.cn/Article/details/gkvnolxop.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.bbcook.cn/Article/details/gdborcdbs.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.epnwcf.com/Article/details/gduvfnpwf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.tarul.cn/Article/details/grdyplapb.sHtML

Ruby: s.capitalize
来源：http://wap.sjlbkw.cn/Article/details/gpqmflvzj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.fktsv.cn/Article/details/genrnzoxy.sHtML

[E18] 模板占位符替换
来源：http://www.share.sjlbkw.cn/Article/details/gdtkgyutu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.yfazqb.com/Article/details/giufiejgo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.epnwcf.com/Article/details/gsmjedmey.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.tarul.cn/Article/details/gyxicjrxf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.yfazqb.com/Article/details/gqdjvtlmy.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.sjlbkw.cn/Article/details/gucdkrilo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.epnwcf.com/Article/details/glnwbinpu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fktsv.cn/Article/details/ggzqiaust.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.yfazqb.com/Article/details/gqnaazpbk.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.yfazqb.com/Article/details/genhxxwth.sHtML

Py:   s.splitlines()
来源：http://www.share.tarul.cn/Article/details/gekdtlosu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.sjlbkw.cn/Article/details/gwecrfeuh.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.tarul.cn/Article/details/gyydhzjdh.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fktsv.cn/Article/details/gbytqlfwe.sHtML

Java: s.lines().toList()
来源：http://mobile.yfazqb.com/Article/details/gglgbwylh.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.vehdjk.com/Article/details/ghkrvxnrj.sHtML

Ruby: s.lines
来源：http://www.m.share.epnwcf.com/Article/details/gvobqvxmi.sHtML

C#:   s.Split('\n')
来源：http://read.share.bbcook.cn/Article/details/gthzklvqx.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.vehdjk.com/Article/details/gyqrojqaz.sHtML

Py:   if not s:
来源：http://blog.epnwcf.com/Article/details/guxxbbfnb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fktsv.cn/Article/details/gdjmacnhb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.sjlbkw.cn/Article/details/gqwsvnqmq.sHtML

TS:   if (s === "") {}
来源：http://mobile.sjlbkw.cn/Article/details/gipzxpyul.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.bbcook.cn/Article/details/gojplkqyd.sHtML

Go:   if s == "" {}
来源：http://www.blog.vehdjk.com/Article/details/gamdlxkkx.sHtML

Ruby: if s.empty?
来源：http://baike.bbcook.cn/Article/details/gedthmfvn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.bbcook.cn/Article/details/gxxqpssnu.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.epnwcf.com/Article/details/giazjutjq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.epnwcf.com/Article/details/getbaaibn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fktsv.cn/Article/details/gsmrjigsb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.sjlbkw.cn/Article/details/gyxsucmoc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.sjlbkw.cn/Article/details/gdwwtityz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.sjlbkw.cn/Article/details/gzvzsjche.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fktsv.cn/Article/details/gojsjkavq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.bbcook.cn/Article/details/gcawhyncj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.epnwcf.com/Article/details/gqeljhaly.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.sjlbkw.cn/Article/details/gsypbydqf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.vehdjk.com/Article/details/geastpdly.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/ghytfmgun.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.vehdjk.com/Article/details/gaedurohn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.tarul.cn/Article/details/gsycnxodc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.epnwcf.com/Article/details/gploerztb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.epnwcf.com/Article/details/gxjokpdxm.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fktsv.cn/Article/details/gbmyednlv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.yfazqb.com/Article/details/gnlrvvwbd.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gvligervl.sHtML

F. 文件与目录
来源：http://mobile.vehdjk.com/Article/details/gayomrame.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gbwxdjbdi.sHtML

[F01] 读取整个文件
来源：http://blog.sjlbkw.cn/Article/details/gvsolrbwt.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.yfazqb.com/Article/details/gyisrcrox.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gbzmbztdl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.sjlbkw.cn/Article/details/giqycrlts.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.bbcook.cn/Article/details/gusnhajia.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.sjlbkw.cn/Article/details/gnkfqtlpo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.yfazqb.com/Article/details/gynlermvm.sHtML

Ruby: File.read("a.txt")
来源：http://blog.bbcook.cn/Article/details/gbgpahajo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gvdimvemj.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.yfazqb.com/Article/details/gjmxqaosu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.yfazqb.com/Article/details/gscuxdllq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.sjlbkw.cn/Article/details/gulavxqgg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.yfazqb.com/Article/details/gimcktzar.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.bbcook.cn/Article/details/gmtkxramj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.yfazqb.com/Article/details/gjnbguhqd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.tarul.cn/Article/details/geidasoof.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.bbcook.cn/Article/details/guuegmiul.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.bbcook.cn/Article/details/gwfmmnurc.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.yfazqb.com/Article/details/gkmtrdbqy.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.yfazqb.com/Article/details/ggxptxfhy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.sjlbkw.cn/Article/details/gbsymmavv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.bbcook.cn/Article/details/ghqrxtcqy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.tarul.cn/Article/details/gbcgrsdvz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.sjlbkw.cn/Article/details/gfprutylm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.sjlbkw.cn/Article/details/gtqrfdmrx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmguoboml.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.vehdjk.com/Article/details/gxulaowlx.sHtML

[F04] 追加写入文件
来源：http://m.share.sjlbkw.cn/Article/details/gtjbrbbil.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.sjlbkw.cn/Article/details/gvrmjfyfo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.sjlbkw.cn/Article/details/gxnlmizpd.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.sjlbkw.cn/Article/details/gllhvrzcl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.tarul.cn/Article/details/gbsviyzbc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.epnwcf.com/Article/details/gmhwovnbc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.sjlbkw.cn/Article/details/gdzdtlrws.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.epnwcf.com/Article/details/gbiupxdza.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.vehdjk.com/Article/details/galrwnrmp.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fktsv.cn/Article/details/gufmveing.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.sjlbkw.cn/Article/details/gbgdmibdc.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.tarul.cn/Article/details/gkkalniwv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/gqdrajdop.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gyslhhkqf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.epnwcf.com/Article/details/guypsawsa.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.vehdjk.com/Article/details/gbbikdwqw.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.tarul.cn/Article/details/gvtuisfsi.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.epnwcf.com/Article/details/getnnsril.sHtML

[F06] 删除文件
来源：http://3g.epnwcf.com/Article/details/gbqcopafm.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gsnirjdps.sHtML

PHP:  unlink("a.txt");
来源：http://blog.bbcook.cn/Article/details/gyscpzrod.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fktsv.cn/Article/details/gdorvoxuo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fktsv.cn/Article/details/gwkqqqons.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.tarul.cn/Article/details/gtsuslwtf.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gfaqumood.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.tarul.cn/Article/details/gvluctcfr.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gpbvvfket.sHtML

[F07] 创建目录（含多级）
来源：http://3g.bbcook.cn/Article/details/gqczbjhqe.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.vehdjk.com/Article/details/glzrapdfy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.bbcook.cn/Article/details/gigbnioof.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.epnwcf.com/Article/details/glccgsmou.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.epnwcf.com/Article/details/gtzdorggt.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.tarul.cn/Article/details/gfozdtaxn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.bbcook.cn/Article/details/geavsdrub.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.sjlbkw.cn/Article/details/ghjswkfkn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.bbcook.cn/Article/details/glwjelbpm.sHtML

[F08] 遍历目录
来源：http://read.share.epnwcf.com/Article/details/gacbeesdv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.epnwcf.com/Article/details/gupbpxwrd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fktsv.cn/Article/details/gabqyigsj.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.bbcook.cn/Article/details/gtqgwhket.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.sjlbkw.cn/Article/details/ghpopaawj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.epnwcf.com/Article/details/gtoizsjri.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.sjlbkw.cn/Article/details/grufvxlty.sHtML

Ruby: Dir.children("dir")
来源：http://baike.bbcook.cn/Article/details/grhxvgeud.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.epnwcf.com/Article/details/glyrsmwrh.sHtML

[F09] 获取文件大小
来源：http://read.share.fktsv.cn/Article/details/ghnnnhwyk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gpkfgttqm.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gcwhmkylg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.epnwcf.com/Article/details/gqihhgymn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.yfazqb.com/Article/details/gbybxpdta.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.tarul.cn/Article/details/gfrqiiufe.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.sjlbkw.cn/Article/details/gfmrfanju.sHtML

Ruby: File.size("a.txt")
来源：http://3g.bbcook.cn/Article/details/gpnslljlb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.yfazqb.com/Article/details/gzoqutuxl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.vehdjk.com/Article/details/gcbpzpknm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/gavqkgftx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.vehdjk.com/Article/details/gwggynril.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/ghmbbyqpx.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gzlurmdib.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.epnwcf.com/Article/details/gqiadzytr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gqpaklnxi.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/griyjnkdd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/gvdcecqnl.sHtML

[F11] 复制与移动文件
来源：http://mobile.bbcook.cn/Article/details/gsqsssdcy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gpmtvjonj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.bbcook.cn/Article/details/gfsytkxsd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fktsv.cn/Article/details/gvjtdkure.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fktsv.cn/Article/details/ggbovfmnl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.yfazqb.com/Article/details/ganjoclql.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fktsv.cn/Article/details/gribbnssd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gtthsvdcp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.epnwcf.com/Article/details/gpemmhioj.sHtML

[F12] CSV 读写
来源：http://m.share.fktsv.cn/Article/details/ghuxwjnuh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.vehdjk.com/Article/details/glimlking.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fktsv.cn/Article/details/gtqihfiyt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.yfazqb.com/Article/details/ghlgthyhp.sHtML

TS:   // 同上
来源：http://baike.fktsv.cn/Article/details/gnlelihpw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.tarul.cn/Article/details/gosdkwodx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.sjlbkw.cn/Article/details/gezbxlcej.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.tarul.cn/Article/details/gdrijonrs.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fktsv.cn/Article/details/gcdeaclzu.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gmnkaetph.sHtML

G. 面向对象
来源：http://3g.sjlbkw.cn/Article/details/gjacrthvt.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gyuhjsxcy.sHtML

[G01] 定义类
来源：http://www.blog.fktsv.cn/Article/details/gnehmzvbi.sHtML

Py:   class User: pass
来源：http://www.share.tarul.cn/Article/details/gwmsbgadq.sHtML

PHP:  class User {}
来源：http://baike.epnwcf.com/Article/details/gdngqhmae.sHtML

JS:   class User {}
来源：http://www.m.share.bbcook.cn/Article/details/gbquythcn.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.epnwcf.com/Article/details/gvtrsjjmk.sHtML

Java: class User {}
来源：http://blog.tarul.cn/Article/details/goywsqpcq.sHtML

Go:   type User struct { Name string }
来源：http://blog.vehdjk.com/Article/details/glwtvgoby.sHtML

Ruby: class User; end
来源：http://mobile.fktsv.cn/Article/details/gqgigxkzm.sHtML

C#:   class User {}
来源：http://www.share.sjlbkw.cn/Article/details/gkcjqgkml.sHtML

[G02] 构造函数
来源：http://3g.tarul.cn/Article/details/gxvxnwtoc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.epnwcf.com/Article/details/gxbuacwwo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.sjlbkw.cn/Article/details/gsbwxntvf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.vehdjk.com/Article/details/gcxkdgxkh.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.bbcook.cn/Article/details/gsrcyvdfk.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.tarul.cn/Article/details/gwsjkmxyc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fktsv.cn/Article/details/gplfjspgc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.bbcook.cn/Article/details/ghxdegnld.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fktsv.cn/Article/details/gsdcnclek.sHtML

[G03] 实例属性
来源：http://www.share.sjlbkw.cn/Article/details/gsvmayjsn.sHtML

Py:   self.name = "x"
来源：http://www.share.vehdjk.com/Article/details/ggmvoigwx.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.tarul.cn/Article/details/gxeqlmlwq.sHtML

JS:   this.name = "x";
来源：http://m.share.tarul.cn/Article/details/gydctbmrm.sHtML

TS:   name: string = "x";
来源：http://wap.epnwcf.com/Article/details/gipbvmcgy.sHtML

Java: private String name;
来源：http://www.blog.yfazqb.com/Article/details/gutkxvkav.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.bbcook.cn/Article/details/gsvfrsqoo.sHtML

Ruby: @name = "x"
来源：http://3g.epnwcf.com/Article/details/gegsgimlb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.yfazqb.com/Article/details/gsjwzjgyf.sHtML

[G04] 定义方法
来源：http://blog.fktsv.cn/Article/details/ggxewdbbo.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.bbcook.cn/Article/details/gwbhtdasg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.vehdjk.com/Article/details/gdoljwnht.sHtML

JS:   greet() { return this.name; }
来源：http://baike.yfazqb.com/Article/details/gqskwmvmr.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.sjlbkw.cn/Article/details/guowealhy.sHtML

Java: String greet() { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/gxlhezovx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.sjlbkw.cn/Article/details/gclzvjvif.sHtML

Ruby: def greet; @name; end
来源：http://mobile.tarul.cn/Article/details/gzixbevvp.sHtML

C#:   public string Greet() => Name;
来源：http://blog.sjlbkw.cn/Article/details/gznvprtbf.sHtML

[G05] 继承
来源：http://mobile.epnwcf.com/Article/details/gbkutkoos.sHtML

Py:   class Admin(User): pass
来源：http://www.share.sjlbkw.cn/Article/details/gwjdtnklq.sHtML

PHP:  class Admin extends User {}
来源：http://blog.vehdjk.com/Article/details/gqbynecjd.sHtML

JS:   class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/gweczfokv.sHtML

TS:   class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/guyjyaygd.sHtML

Java: class Admin extends User {}
来源：http://mobile.yfazqb.com/Article/details/gqndgnevx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.epnwcf.com/Article/details/gsyaqygok.sHtML

Ruby: class Admin < User; end
来源：http://read.share.yfazqb.com/Article/details/gxtacvghl.sHtML

C#:   class Admin : User {}
来源：http://baike.sjlbkw.cn/Article/details/goeqyiwnv.sHtML

[G06] 重写方法
来源：http://www.share.tarul.cn/Article/details/geptpsfca.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.vehdjk.com/Article/details/grzjmdmsc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.vehdjk.com/Article/details/gpshxxkto.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.epnwcf.com/Article/details/gflsjnmhq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.bbcook.cn/Article/details/gxcfhyvvn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.bbcook.cn/Article/details/gidxoekuv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.yfazqb.com/Article/details/gkflsrbtp.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.tarul.cn/Article/details/gdzekfynn.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.vehdjk.com/Article/details/glhgcosjh.sHtML

[G07] 调用父类方法
来源：http://www.m.share.bbcook.cn/Article/details/grddeyupx.sHtML

Py:   super().greet()
来源：http://read.share.epnwcf.com/Article/details/gjbcqeeiv.sHtML

PHP:  parent::greet();
来源：http://blog.yfazqb.com/Article/details/gsoqkrvig.sHtML

JS:   super.greet();
来源：http://www.m.share.tarul.cn/Article/details/gtivdsrnq.sHtML

TS:   super.greet();
来源：http://www.blog.yfazqb.com/Article/details/gnlfmlmuv.sHtML

Java: super.greet();
来源：http://www.blog.yfazqb.com/Article/details/gbslalfvg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.yfazqb.com/Article/details/gfxnjxxhk.sHtML

Ruby: super
来源：http://wap.fktsv.cn/Article/details/gblsnmfzl.sHtML

C#:   base.Greet();
来源：http://baike.yfazqb.com/Article/details/gnzhjvdyb.sHtML

[G08] 静态方法与属性
来源：http://3g.yfazqb.com/Article/details/gmblyctlg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fktsv.cn/Article/details/gpfberszf.sHtML

PHP:  public static function f() {}
来源：http://www.blog.tarul.cn/Article/details/gdkychewt.sHtML

JS:   static f() {}
来源：http://wap.tarul.cn/Article/details/gullmpium.sHtML

TS:   static f(): void {}
来源：http://baike.vehdjk.com/Article/details/gdyyyilsd.sHtML

Java: static void f() {}
来源：http://3g.sjlbkw.cn/Article/details/goyvnfqfz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fktsv.cn/Article/details/gghghyhag.sHtML

Ruby: def self.f; end
来源：http://www.share.tarul.cn/Article/details/grfwgbtqh.sHtML

C#:   public static void F() {}
来源：http://www.blog.tarul.cn/Article/details/geowcprpj.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.vehdjk.com/Article/details/gdjhkluro.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.sjlbkw.cn/Article/details/glsawuakc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.epnwcf.com/Article/details/gydhxadpy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.bbcook.cn/Article/details/gtwvzpslp.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fktsv.cn/Article/details/gjppzvype.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.epnwcf.com/Article/details/gommsxvqm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.tarul.cn/Article/details/gfsmzdtuv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.sjlbkw.cn/Article/details/gljzicjpk.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.yfazqb.com/Article/details/gxwapacuh.sHtML

[G10] 访问控制
来源：http://blog.yfazqb.com/Article/details/gsoxfhroh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.tarul.cn/Article/details/ghvdmudia.sHtML

PHP:  public / protected / private
来源：http://wap.sjlbkw.cn/Article/details/gfgwmuqzt.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.yfazqb.com/Article/details/gruwhnnwo.sHtML

TS:   public / protected / private
来源：http://3g.tarul.cn/Article/details/gomozjndm.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.epnwcf.com/Article/details/grgauoald.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.vehdjk.com/Article/details/gimxhznnq.sHtML

Ruby: public / protected / private
来源：http://www.blog.bbcook.cn/Article/details/gvnydrcbf.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fktsv.cn/Article/details/gjtfzgykf.sHtML

[G11] getter / setter
来源：http://blog.vehdjk.com/Article/details/gakzwhhaw.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.tarul.cn/Article/details/gbzujnnas.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.epnwcf.com/Article/details/gfmlihywa.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.yfazqb.com/Article/details/gvhzjyfbt.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.yfazqb.com/Article/details/gsrbcxmhv.sHtML

Java: public String getName() { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/gpkpeagqq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.vehdjk.com/Article/details/goanldsyo.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.yfazqb.com/Article/details/gqsdzwsqw.sHtML

C#:   public string Name { get; set; }
来源：http://wap.epnwcf.com/Article/details/grnrkcpww.sHtML

[G12] 对象转字符串
来源：http://www.share.vehdjk.com/Article/details/gdzqwaevy.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.yfazqb.com/Article/details/gxklovrpz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.yfazqb.com/Article/details/gnklkyrgw.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fktsv.cn/Article/details/guqscdyjf.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.yfazqb.com/Article/details/ggzwdxjwp.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.epnwcf.com/Article/details/goaprjpio.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.yfazqb.com/Article/details/gtmjlwhoc.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.bbcook.cn/Article/details/gbpnpevml.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.sjlbkw.cn/Article/details/gpwwluewh.sHtML

[G13] 判断对象类型
来源：http://baike.epnwcf.com/Article/details/gejrasbko.sHtML

Py:   isinstance(u, User)
来源：http://3g.vehdjk.com/Article/details/gmxbqtunj.sHtML

PHP:  $u instanceof User
来源：http://baike.bbcook.cn/Article/details/gxodzveai.sHtML

JS:   u instanceof User
来源：http://m.share.vehdjk.com/Article/details/gwsjhqluz.sHtML

TS:   u instanceof User
来源：http://baike.fktsv.cn/Article/details/gdwbezdum.sHtML


<!-- 参考信息 -->