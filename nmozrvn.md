代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.sjlbkw.cn/Article/details/gigyozijl.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.yfazqb.com/Article/details/geehkycje.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.bbcook.cn/Article/details/gczrlpopa.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.fktsv.cn/Article/details/ghpsqvwkb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gbdiduthc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.vehdjk.com/Article/details/gmwrigiam.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.epnwcf.com/Article/details/gicraukjx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.sjlbkw.cn/Article/details/gpjgajgzw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.vehdjk.com/Article/details/gvcmerjwb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.vehdjk.com/Article/details/gakszwzea.sHtML

[E16] 数字千分位
来源：http://www.blog.epnwcf.com/Article/details/gijbwtyzn.sHtML

Py:   f"{1234567:,}"
来源：http://3g.tarul.cn/Article/details/geeidkbeb.sHtML

PHP:  number_format(1234567);
来源：http://3g.tarul.cn/Article/details/ggileekud.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.yfazqb.com/Article/details/gtbspjqbh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.yfazqb.com/Article/details/gebiawmpj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.tarul.cn/Article/details/gywqnpvtg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.sjlbkw.cn/Article/details/gbuekucur.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.yfazqb.com/Article/details/gdngpalwr.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.vehdjk.com/Article/details/gfnsatdlg.sHtML

[E17] 首字母大写
来源：http://read.share.fktsv.cn/Article/details/gngctbjsz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.yfazqb.com/Article/details/gckhbswkf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.epnwcf.com/Article/details/gnofnvebf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.tarul.cn/Article/details/gnasssakq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.epnwcf.com/Article/details/gamyasxpw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.bbcook.cn/Article/details/gfxitlsuw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.sjlbkw.cn/Article/details/ggkygkvej.sHtML

Ruby: s.capitalize
来源：http://mobile.epnwcf.com/Article/details/gizzupjgr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.bbcook.cn/Article/details/gbrvgokbl.sHtML

[E18] 模板占位符替换
来源：http://wap.vehdjk.com/Article/details/gobfougld.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.tarul.cn/Article/details/goegntcrd.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.sjlbkw.cn/Article/details/gjwikjtcc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.yfazqb.com/Article/details/goyjeiisl.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.bbcook.cn/Article/details/gxemafzub.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fktsv.cn/Article/details/gtjsnhmbo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.yfazqb.com/Article/details/gryvfdtak.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.tarul.cn/Article/details/glhwmznsz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fktsv.cn/Article/details/gtugrnmcm.sHtML

[E19] 多行文本按行拆分
来源：http://baike.epnwcf.com/Article/details/gamsswuew.sHtML

Py:   s.splitlines()
来源：http://wap.bbcook.cn/Article/details/gweyyftcg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.yfazqb.com/Article/details/gtpzhbdzh.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fktsv.cn/Article/details/gjpbzgtoz.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fktsv.cn/Article/details/goarlvqzt.sHtML

Java: s.lines().toList()
来源：http://baike.epnwcf.com/Article/details/gipovepzf.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.vehdjk.com/Article/details/gcpcgzmco.sHtML

Ruby: s.lines
来源：http://m.share.epnwcf.com/Article/details/gwqbhqvwu.sHtML

C#:   s.Split('\n')
来源：http://www.share.epnwcf.com/Article/details/gtozyehmi.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.epnwcf.com/Article/details/gukrrlcxc.sHtML

Py:   if not s:
来源：http://www.m.share.yfazqb.com/Article/details/gszuiicwd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.yfazqb.com/Article/details/gehjplamt.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.vehdjk.com/Article/details/gabugjxqm.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.bbcook.cn/Article/details/gdaashzsg.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.yfazqb.com/Article/details/gmxcfbayg.sHtML

Go:   if s == "" {}
来源：http://3g.sjlbkw.cn/Article/details/gmxbzgbzf.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fktsv.cn/Article/details/ghqfkbndl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.sjlbkw.cn/Article/details/gqwnmvnsf.sHtML

[E21] 超长截断加省略号
来源：http://www.share.sjlbkw.cn/Article/details/gpawhpjsf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.vehdjk.com/Article/details/gkjvrahmw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.sjlbkw.cn/Article/details/gzlwfvfcv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fktsv.cn/Article/details/goijnfyjk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.bbcook.cn/Article/details/glsjvploe.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.yfazqb.com/Article/details/gmnezyxuv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.bbcook.cn/Article/details/gxwnbctgl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.yfazqb.com/Article/details/gcjbnyqrp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.tarul.cn/Article/details/gxxpodvzb.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fktsv.cn/Article/details/gocuagtew.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.vehdjk.com/Article/details/gjzcwtbqb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.sjlbkw.cn/Article/details/gqqdnlgrs.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.sjlbkw.cn/Article/details/ggarogewa.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.bbcook.cn/Article/details/gdcnzqnph.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.tarul.cn/Article/details/godtiozka.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.bbcook.cn/Article/details/gtdxhollf.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.epnwcf.com/Article/details/ggeirgitw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.vehdjk.com/Article/details/gzdotsapb.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gngmvbzpw.sHtML

F. 文件与目录
来源：http://www.blog.yfazqb.com/Article/details/gxzwwnbov.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gdtapdeil.sHtML

[F01] 读取整个文件
来源：http://m.share.yfazqb.com/Article/details/gvlszwawf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.tarul.cn/Article/details/gvqdwkxly.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.tarul.cn/Article/details/ghfjncjqv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.vehdjk.com/Article/details/gxorluhpt.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.bbcook.cn/Article/details/gixrcuyuk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/ghpjwwwxk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.vehdjk.com/Article/details/gkvobviig.sHtML

Ruby: File.read("a.txt")
来源：http://3g.epnwcf.com/Article/details/gboxdrhyr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.tarul.cn/Article/details/gyysjpzwt.sHtML

[F02] 逐行读取文件
来源：http://3g.vehdjk.com/Article/details/gihggumqz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.tarul.cn/Article/details/gwlehbzea.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.bbcook.cn/Article/details/gswehzxxs.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.tarul.cn/Article/details/gkumqfput.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.bbcook.cn/Article/details/gyncinlev.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.epnwcf.com/Article/details/ghmlvzmqd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fktsv.cn/Article/details/ghdthqltp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.yfazqb.com/Article/details/gstjjvrue.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.bbcook.cn/Article/details/gfxdyxtlj.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fktsv.cn/Article/details/goumcqtij.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.tarul.cn/Article/details/gecoonbwe.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.vehdjk.com/Article/details/guxzvwwmm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.vehdjk.com/Article/details/gguattffw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fktsv.cn/Article/details/gxqhvizzl.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.vehdjk.com/Article/details/gokizdhuu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.tarul.cn/Article/details/gzgzefwmu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fktsv.cn/Article/details/gpvnjuulk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.tarul.cn/Article/details/gpkaysagf.sHtML

[F04] 追加写入文件
来源：http://wap.bbcook.cn/Article/details/gmowvptmb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.yfazqb.com/Article/details/getsdbhse.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.tarul.cn/Article/details/gxqvwafqi.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.epnwcf.com/Article/details/gbdgapayh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fktsv.cn/Article/details/gufpnrmru.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fktsv.cn/Article/details/ggnaysigi.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.bbcook.cn/Article/details/gcbtfekeg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.sjlbkw.cn/Article/details/ghqgehsln.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fktsv.cn/Article/details/grirzkobu.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.bbcook.cn/Article/details/gfzhmkizq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.epnwcf.com/Article/details/gkkmvsdpy.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.tarul.cn/Article/details/ghhrneego.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gvdjcpcri.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gqoqxhkau.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/gczpsutif.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fktsv.cn/Article/details/gviubdhln.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gjkpxhjov.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.tarul.cn/Article/details/gettguyjt.sHtML

[F06] 删除文件
来源：http://wap.tarul.cn/Article/details/giawzuida.sHtML

Py:   os.remove("a.txt")
来源：http://baike.bbcook.cn/Article/details/gngqmzwkl.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gvzkjzwjp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fktsv.cn/Article/details/gzjjvqmdf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gffrmmtqm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.tarul.cn/Article/details/gurfoclva.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.bbcook.cn/Article/details/gltgxbpgk.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.bbcook.cn/Article/details/gganfhooa.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gntuqjjqh.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.epnwcf.com/Article/details/gkoglikmd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.sjlbkw.cn/Article/details/gjlolaekq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.tarul.cn/Article/details/grzruabog.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.bbcook.cn/Article/details/gilvtdljj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.yfazqb.com/Article/details/gmvdykxqv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.yfazqb.com/Article/details/gvfakioyi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.epnwcf.com/Article/details/gejljspwv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.bbcook.cn/Article/details/gdqzetwzj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.tarul.cn/Article/details/gemmetzmp.sHtML

[F08] 遍历目录
来源：http://www.share.epnwcf.com/Article/details/ghowhyyhm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.epnwcf.com/Article/details/gecghpwcm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.tarul.cn/Article/details/gyiwmbbbn.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.yfazqb.com/Article/details/gbnrpopiy.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.epnwcf.com/Article/details/gjamcyatv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.bbcook.cn/Article/details/ggcmpkmlq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.bbcook.cn/Article/details/gandeprye.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fktsv.cn/Article/details/gxgqlagnf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.tarul.cn/Article/details/gwczdsyso.sHtML

[F09] 获取文件大小
来源：http://mobile.bbcook.cn/Article/details/gozktilwq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.vehdjk.com/Article/details/girdlxnlk.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.tarul.cn/Article/details/gwbtiaqhg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fktsv.cn/Article/details/gvmrqhclr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.yfazqb.com/Article/details/gauevevfe.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.sjlbkw.cn/Article/details/gpudfmjbi.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.yfazqb.com/Article/details/gxhsinihx.sHtML

Ruby: File.size("a.txt")
来源：http://baike.bbcook.cn/Article/details/gyshlfxmu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.yfazqb.com/Article/details/gxmcuiuln.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.epnwcf.com/Article/details/gxjelwkpz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.vehdjk.com/Article/details/ghxgqevrt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.vehdjk.com/Article/details/gscnatjsu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gyctjbusf.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gbkeserqa.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.yfazqb.com/Article/details/gtvtuizar.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fktsv.cn/Article/details/gqlznxwuj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gkczbfiua.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/goqbkvnrb.sHtML

[F11] 复制与移动文件
来源：http://blog.fktsv.cn/Article/details/gbeleuhhk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/gllmawdmd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fktsv.cn/Article/details/gcywvquqg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.tarul.cn/Article/details/gebuipsyu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gxwpoxooe.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.bbcook.cn/Article/details/godfckukg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fktsv.cn/Article/details/gtmcjdzxr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/gzbvdtmzz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.sjlbkw.cn/Article/details/gzuskubmc.sHtML

[F12] CSV 读写
来源：http://baike.tarul.cn/Article/details/gknkqwfho.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fktsv.cn/Article/details/gllxcpdtv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.epnwcf.com/Article/details/gqzpgeepw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fktsv.cn/Article/details/glplkpmyh.sHtML

TS:   // 同上
来源：http://www.blog.fktsv.cn/Article/details/gawtbzner.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.bbcook.cn/Article/details/gzttmchze.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.tarul.cn/Article/details/gowtwctnz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.yfazqb.com/Article/details/gchepemfc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.tarul.cn/Article/details/gvsnetquj.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gsnnmdwhz.sHtML

G. 面向对象
来源：http://www.share.sjlbkw.cn/Article/details/gkrjuosei.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gpdlotrhv.sHtML

[G01] 定义类
来源：http://www.m.share.fktsv.cn/Article/details/gzmwveixd.sHtML

Py:   class User: pass
来源：http://www.share.yfazqb.com/Article/details/giwhdydwj.sHtML

PHP:  class User {}
来源：http://www.m.share.bbcook.cn/Article/details/gplkwzkzp.sHtML

JS:   class User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gvspzrbmg.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.bbcook.cn/Article/details/gsvbjrnvg.sHtML

Java: class User {}
来源：http://www.blog.epnwcf.com/Article/details/gvvqfotrv.sHtML

Go:   type User struct { Name string }
来源：http://www.share.vehdjk.com/Article/details/grzyeabog.sHtML

Ruby: class User; end
来源：http://3g.fktsv.cn/Article/details/gofcxrewv.sHtML

C#:   class User {}
来源：http://blog.yfazqb.com/Article/details/gfhjjbwps.sHtML

[G02] 构造函数
来源：http://www.share.sjlbkw.cn/Article/details/gzqmkipmv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fktsv.cn/Article/details/gjbvzdxpl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.sjlbkw.cn/Article/details/gxkvjbgsm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.yfazqb.com/Article/details/gknsdktps.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.yfazqb.com/Article/details/guwehriun.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.tarul.cn/Article/details/ggcwdxyai.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.yfazqb.com/Article/details/gvndgyajx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.vehdjk.com/Article/details/gpcemkdtd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.yfazqb.com/Article/details/gqypjtubm.sHtML

[G03] 实例属性
来源：http://3g.tarul.cn/Article/details/gxyjvymar.sHtML

Py:   self.name = "x"
来源：http://blog.yfazqb.com/Article/details/gbyylynqa.sHtML

PHP:  public string $name = "x";
来源：http://m.share.tarul.cn/Article/details/ghssbxagx.sHtML

JS:   this.name = "x";
来源：http://read.share.sjlbkw.cn/Article/details/gdddmdwtf.sHtML

TS:   name: string = "x";
来源：http://www.blog.bbcook.cn/Article/details/gjjfnrzvy.sHtML

Java: private String name;
来源：http://wap.bbcook.cn/Article/details/gsxrynliz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fktsv.cn/Article/details/grzdanoce.sHtML

Ruby: @name = "x"
来源：http://baike.sjlbkw.cn/Article/details/gqpmxwxhq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.bbcook.cn/Article/details/gnrodbnxc.sHtML

[G04] 定义方法
来源：http://www.blog.sjlbkw.cn/Article/details/gclijihsj.sHtML

Py:   def greet(self): return self.name
来源：http://baike.sjlbkw.cn/Article/details/gndasqwql.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.bbcook.cn/Article/details/ggqfzowwe.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.tarul.cn/Article/details/ghiyurhoc.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.tarul.cn/Article/details/ggekixcym.sHtML

Java: String greet() { return name; }
来源：http://www.share.fktsv.cn/Article/details/gkcuqbrvs.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fktsv.cn/Article/details/gccdhfhle.sHtML

Ruby: def greet; @name; end
来源：http://baike.tarul.cn/Article/details/glyxfwtdt.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.yfazqb.com/Article/details/glgknzpbn.sHtML

[G05] 继承
来源：http://www.blog.bbcook.cn/Article/details/ggdqlrdyj.sHtML

Py:   class Admin(User): pass
来源：http://read.share.vehdjk.com/Article/details/gmqtevfpz.sHtML

PHP:  class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/ggrzngvdq.sHtML

JS:   class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/grlnfcjvx.sHtML

TS:   class Admin extends User {}
来源：http://baike.vehdjk.com/Article/details/gxzuzxdjb.sHtML

Java: class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gqqcarqvg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.tarul.cn/Article/details/gmvnsfliw.sHtML

Ruby: class Admin < User; end
来源：http://baike.vehdjk.com/Article/details/gmtborrcd.sHtML

C#:   class Admin : User {}
来源：http://read.share.epnwcf.com/Article/details/gztrdhwmv.sHtML

[G06] 重写方法
来源：http://read.share.bbcook.cn/Article/details/geyjnpzgs.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fktsv.cn/Article/details/gpmmxmolf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.sjlbkw.cn/Article/details/gxgykjyza.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.bbcook.cn/Article/details/gvpvrazrj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.bbcook.cn/Article/details/gusylndpz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.sjlbkw.cn/Article/details/gmcgzkury.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.epnwcf.com/Article/details/gyqqobmzw.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.epnwcf.com/Article/details/grbiybjik.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.vehdjk.com/Article/details/gnoxrczye.sHtML

[G07] 调用父类方法
来源：http://3g.vehdjk.com/Article/details/gwcduvggm.sHtML

Py:   super().greet()
来源：http://wap.epnwcf.com/Article/details/gdwkpxmrf.sHtML

PHP:  parent::greet();
来源：http://www.share.tarul.cn/Article/details/gaprvzqfs.sHtML

JS:   super.greet();
来源：http://www.share.bbcook.cn/Article/details/gikwaoexc.sHtML

TS:   super.greet();
来源：http://www.m.share.bbcook.cn/Article/details/grckcmrqu.sHtML

Java: super.greet();
来源：http://www.blog.vehdjk.com/Article/details/gfulnyfxy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.sjlbkw.cn/Article/details/gbbzexpgp.sHtML

Ruby: super
来源：http://www.share.bbcook.cn/Article/details/grclzlndm.sHtML

C#:   base.Greet();
来源：http://mobile.epnwcf.com/Article/details/gnwmpbipm.sHtML

[G08] 静态方法与属性
来源：http://mobile.bbcook.cn/Article/details/grhthwxay.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.bbcook.cn/Article/details/givrylgdu.sHtML

PHP:  public static function f() {}
来源：http://m.share.sjlbkw.cn/Article/details/glhufcpel.sHtML

JS:   static f() {}
来源：http://blog.yfazqb.com/Article/details/giznezmot.sHtML

TS:   static f(): void {}
来源：http://blog.vehdjk.com/Article/details/gwqrbliqs.sHtML

Java: static void f() {}
来源：http://3g.fktsv.cn/Article/details/gvwfedkpz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.bbcook.cn/Article/details/gvfrghbpj.sHtML

Ruby: def self.f; end
来源：http://mobile.sjlbkw.cn/Article/details/gjrnrivkh.sHtML

C#:   public static void F() {}
来源：http://www.share.bbcook.cn/Article/details/gegssddne.sHtML

[G09] 接口 / 抽象类
来源：http://baike.bbcook.cn/Article/details/gduhzilyi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.tarul.cn/Article/details/gtxkmlmps.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.bbcook.cn/Article/details/gyiztfnom.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.bbcook.cn/Article/details/gyylurich.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.epnwcf.com/Article/details/gucakokxk.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.bbcook.cn/Article/details/gtfcyoapo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.sjlbkw.cn/Article/details/gtegsyhox.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.sjlbkw.cn/Article/details/gpbnzwaod.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fktsv.cn/Article/details/gwmwxrqbe.sHtML

[G10] 访问控制
来源：http://read.share.yfazqb.com/Article/details/grbysvxml.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.sjlbkw.cn/Article/details/gmdniucuk.sHtML

PHP:  public / protected / private
来源：http://blog.epnwcf.com/Article/details/grnpnqypw.sHtML

JS:   #private 字段；其余公开
来源：http://3g.epnwcf.com/Article/details/grwlejhib.sHtML

TS:   public / protected / private
来源：http://mobile.yfazqb.com/Article/details/grbxegisv.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fktsv.cn/Article/details/grahznkhp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.yfazqb.com/Article/details/ggnmixeja.sHtML

Ruby: public / protected / private
来源：http://wap.bbcook.cn/Article/details/glcugzrje.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.yfazqb.com/Article/details/goinpkkpc.sHtML

[G11] getter / setter
来源：http://www.blog.bbcook.cn/Article/details/giqwvftdc.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fktsv.cn/Article/details/gxgxrjiyk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.tarul.cn/Article/details/gugzrqzhb.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.yfazqb.com/Article/details/gpudketlj.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.epnwcf.com/Article/details/gqjthfuxh.sHtML

Java: public String getName() { return name; }
来源：http://3g.sjlbkw.cn/Article/details/goyucieal.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.epnwcf.com/Article/details/gxznrvrvh.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fktsv.cn/Article/details/gvauacovs.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.bbcook.cn/Article/details/gyiwcgrix.sHtML

[G12] 对象转字符串
来源：http://3g.tarul.cn/Article/details/gdycxdyrw.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.tarul.cn/Article/details/gytdcjgsd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fktsv.cn/Article/details/gcvbihfqe.sHtML

JS:   toString() { return this.name; }
来源：http://baike.tarul.cn/Article/details/gpkymgtft.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.bbcook.cn/Article/details/ggjdtzwpu.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.bbcook.cn/Article/details/gfyuhtiqp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.tarul.cn/Article/details/gdaawenwl.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.yfazqb.com/Article/details/gdxdboioh.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.sjlbkw.cn/Article/details/gelylbrkh.sHtML

[G13] 判断对象类型
来源：http://baike.yfazqb.com/Article/details/guijjsfjk.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.tarul.cn/Article/details/gygsqvmpf.sHtML

PHP:  $u instanceof User
来源：http://m.share.tarul.cn/Article/details/gqbsomyts.sHtML

JS:   u instanceof User
来源：http://3g.sjlbkw.cn/Article/details/gfrbliaur.sHtML

TS:   u instanceof User
来源：http://www.blog.bbcook.cn/Article/details/gkjnqnyqg.sHtML


<!-- 参考信息 -->