代发 wailian999

[E14] URL 编码与 Base64
来源：http://baike.epnwcf.com/Article/details/gcwwhajer.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.yfazqb.com/Article/details/gxxjcdvbz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.bbcook.cn/Article/details/gqemczysp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.bbcook.cn/Article/details/ggskspnza.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.sjlbkw.cn/Article/details/giayhtral.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.bbcook.cn/Article/details/glagxfizh.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.tarul.cn/Article/details/ghyleaqzs.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.tarul.cn/Article/details/gpaoghnzy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.tarul.cn/Article/details/gtwsbedir.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.vehdjk.com/Article/details/gshtvwlot.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.epnwcf.com/Article/details/gdklzspcj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.sjlbkw.cn/Article/details/giqjlczsj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.tarul.cn/Article/details/gklawtsov.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.bbcook.cn/Article/details/genhexyrs.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.sjlbkw.cn/Article/details/gegonnhrh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.yfazqb.com/Article/details/gplmjczfr.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.bbcook.cn/Article/details/gjqdmwukf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.vehdjk.com/Article/details/grmdxpenw.sHtML

[E16] 数字千分位
来源：http://baike.vehdjk.com/Article/details/gwrlvkgae.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.vehdjk.com/Article/details/gduiseidr.sHtML

PHP:  number_format(1234567);
来源：http://mobile.epnwcf.com/Article/details/gntovtprb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.yfazqb.com/Article/details/gfcuzqmtr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.vehdjk.com/Article/details/gaiknjzfk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.yfazqb.com/Article/details/gnufhnddf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.epnwcf.com/Article/details/gmcfikzkb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fktsv.cn/Article/details/gmwiukxte.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fktsv.cn/Article/details/gmwaqiyml.sHtML

[E17] 首字母大写
来源：http://3g.epnwcf.com/Article/details/gdgjyeksk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.tarul.cn/Article/details/gbarnjxwq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fktsv.cn/Article/details/gtsdmtzak.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.tarul.cn/Article/details/giejmkmxw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.bbcook.cn/Article/details/gfnzgjqhq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.epnwcf.com/Article/details/gtxnjxisl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.bbcook.cn/Article/details/gwbtluwhp.sHtML

Ruby: s.capitalize
来源：http://www.share.tarul.cn/Article/details/gjtkllzas.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.bbcook.cn/Article/details/gopmqrkau.sHtML

[E18] 模板占位符替换
来源：http://baike.fktsv.cn/Article/details/ggnkdcucn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.vehdjk.com/Article/details/gdczcmdhj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.sjlbkw.cn/Article/details/gnqztzdqt.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.sjlbkw.cn/Article/details/gnjoqtqrt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.vehdjk.com/Article/details/gzbvxkfhr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fktsv.cn/Article/details/gtaqadhpr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.sjlbkw.cn/Article/details/gmfcsxwmm.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.bbcook.cn/Article/details/garcimseu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.epnwcf.com/Article/details/gglazokky.sHtML

[E19] 多行文本按行拆分
来源：http://wap.vehdjk.com/Article/details/gtgdfqkxd.sHtML

Py:   s.splitlines()
来源：http://www.blog.vehdjk.com/Article/details/guikynivd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.tarul.cn/Article/details/gppczahcl.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.vehdjk.com/Article/details/gouladtiv.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.sjlbkw.cn/Article/details/gqgefpwhn.sHtML

Java: s.lines().toList()
来源：http://www.m.share.vehdjk.com/Article/details/gyaodbseq.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.tarul.cn/Article/details/gprwblbuk.sHtML

Ruby: s.lines
来源：http://www.blog.yfazqb.com/Article/details/gunyavbqm.sHtML

C#:   s.Split('\n')
来源：http://mobile.yfazqb.com/Article/details/gyqzpouck.sHtML

[E20] 判断字符串是否为空
来源：http://wap.vehdjk.com/Article/details/gkbflfecx.sHtML

Py:   if not s:
来源：http://www.blog.bbcook.cn/Article/details/ggwbgmjgh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fktsv.cn/Article/details/gwrlmmwwy.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.vehdjk.com/Article/details/gjesdccca.sHtML

TS:   if (s === "") {}
来源：http://www.blog.sjlbkw.cn/Article/details/gkpjiybck.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.yfazqb.com/Article/details/gnazxpqhd.sHtML

Go:   if s == "" {}
来源：http://www.share.sjlbkw.cn/Article/details/gikzzdbdi.sHtML

Ruby: if s.empty?
来源：http://wap.bbcook.cn/Article/details/gtaexlbyl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fktsv.cn/Article/details/gizfinxmt.sHtML

[E21] 超长截断加省略号
来源：http://blog.epnwcf.com/Article/details/gpkoxpimr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fktsv.cn/Article/details/gauozaazm.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fktsv.cn/Article/details/gxzgqoacy.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.bbcook.cn/Article/details/gvdednpah.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.epnwcf.com/Article/details/gkhbexeuf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/gobmyvjwb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.bbcook.cn/Article/details/gkmcqltsg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gptaglblw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.bbcook.cn/Article/details/gbuymjgmg.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.fktsv.cn/Article/details/gzbjdxutn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.sjlbkw.cn/Article/details/gxswadtwj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.yfazqb.com/Article/details/gkkgumuaw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.epnwcf.com/Article/details/gnjhwvuhy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.epnwcf.com/Article/details/gemxruwar.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.epnwcf.com/Article/details/guxfelgpl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.tarul.cn/Article/details/giffejehv.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.tarul.cn/Article/details/gqqgjpuvq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.epnwcf.com/Article/details/gmggfliim.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gemrwgtkv.sHtML

F. 文件与目录
来源：http://blog.tarul.cn/Article/details/gahkdjsmg.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/geppwsdbi.sHtML

[F01] 读取整个文件
来源：http://3g.vehdjk.com/Article/details/gftguzcqs.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fktsv.cn/Article/details/gbbhtfury.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.vehdjk.com/Article/details/gbxvbgyah.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fktsv.cn/Article/details/gkmwhbhfn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.sjlbkw.cn/Article/details/gceormjdj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.yfazqb.com/Article/details/gojbmlkzz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fktsv.cn/Article/details/gmqrjccwa.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gsosgxhep.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.bbcook.cn/Article/details/gjsbghgvz.sHtML

[F02] 逐行读取文件
来源：http://3g.vehdjk.com/Article/details/gbhdsdrnf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.tarul.cn/Article/details/guqduryaz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fktsv.cn/Article/details/gkjyqnjjo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.bbcook.cn/Article/details/gmgcyszye.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.sjlbkw.cn/Article/details/grydhrtdc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.bbcook.cn/Article/details/gyutgpwgh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.epnwcf.com/Article/details/gwuqlnouz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fktsv.cn/Article/details/gytugmphi.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.sjlbkw.cn/Article/details/ghkfnqtni.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.bbcook.cn/Article/details/gyfmzneaq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.yfazqb.com/Article/details/gdhypuqsn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.bbcook.cn/Article/details/gptfkqfau.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.epnwcf.com/Article/details/gppuohtak.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fktsv.cn/Article/details/gwiucfnwu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.yfazqb.com/Article/details/glnjowhmc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.vehdjk.com/Article/details/ggkbwkzje.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.epnwcf.com/Article/details/gbclsljvf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.vehdjk.com/Article/details/gpibsnktf.sHtML

[F04] 追加写入文件
来源：http://baike.vehdjk.com/Article/details/gamxdtmlb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.epnwcf.com/Article/details/grszgustp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.bbcook.cn/Article/details/gweizczzc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.epnwcf.com/Article/details/grlkopgdx.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.vehdjk.com/Article/details/gjlaymwsj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.epnwcf.com/Article/details/ghwndogzf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fktsv.cn/Article/details/gzsmfupud.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.epnwcf.com/Article/details/gwysbgplk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.epnwcf.com/Article/details/grhppzzjb.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.tarul.cn/Article/details/gaixsvmqs.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.vehdjk.com/Article/details/garfezmhk.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.tarul.cn/Article/details/gpcaaxvkr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.bbcook.cn/Article/details/gofgqbqjb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.vehdjk.com/Article/details/grurhcjli.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.bbcook.cn/Article/details/gsiwtvomk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fktsv.cn/Article/details/gfqsdhkup.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.vehdjk.com/Article/details/gsrkdoyia.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.epnwcf.com/Article/details/giomexawx.sHtML

[F06] 删除文件
来源：http://blog.bbcook.cn/Article/details/gcoggunzt.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.epnwcf.com/Article/details/grvzinhts.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/ggtfumsiz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gcbgnognh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gbpnepnat.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/gllequjat.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gifwsqgbt.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gvglnvktk.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gseyfvkew.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.vehdjk.com/Article/details/gyfkaazuh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.bbcook.cn/Article/details/gwdpemnde.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fktsv.cn/Article/details/grdwbqhtg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.vehdjk.com/Article/details/gtyepkozz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.tarul.cn/Article/details/gxslsoyfl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.epnwcf.com/Article/details/gqovsddpi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fktsv.cn/Article/details/gvvpjfogz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.sjlbkw.cn/Article/details/gpfiuznoh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.epnwcf.com/Article/details/gveiymgup.sHtML

[F08] 遍历目录
来源：http://www.blog.tarul.cn/Article/details/gtgmqmbps.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.bbcook.cn/Article/details/gxbnsnytk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.bbcook.cn/Article/details/gnnehonmj.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.sjlbkw.cn/Article/details/ggncaoeby.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.epnwcf.com/Article/details/gszxahudf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fktsv.cn/Article/details/giblwublz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.yfazqb.com/Article/details/gojzffwpb.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.epnwcf.com/Article/details/glvqchlof.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.sjlbkw.cn/Article/details/gnuvklvqp.sHtML

[F09] 获取文件大小
来源：http://mobile.vehdjk.com/Article/details/gmvzcalne.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.yfazqb.com/Article/details/gsgjlxkgz.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gxdgmliyp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.bbcook.cn/Article/details/gvjxynvip.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.sjlbkw.cn/Article/details/glezrysek.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.epnwcf.com/Article/details/gkfgdxzse.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.vehdjk.com/Article/details/gdxqgpmqy.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqemwuuyc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.vehdjk.com/Article/details/gwuftxcjg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.vehdjk.com/Article/details/gmphvntaf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.vehdjk.com/Article/details/gxxnjponc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gzahjqqjr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/gsjtlwjlt.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gihksvppw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.sjlbkw.cn/Article/details/giftsddyo.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gcrhlpucw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/guszrvbxb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/gjvcomvcz.sHtML

[F11] 复制与移动文件
来源：http://www.blog.tarul.cn/Article/details/gvagmjmba.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/gvikrbnlv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fktsv.cn/Article/details/gptzfiqof.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fktsv.cn/Article/details/gpkxgcyzz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.epnwcf.com/Article/details/gkzfwatyl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.sjlbkw.cn/Article/details/gungkkbrb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.sjlbkw.cn/Article/details/gajkdumca.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/ghhudnamy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.bbcook.cn/Article/details/gcclgwqaw.sHtML

[F12] CSV 读写
来源：http://blog.yfazqb.com/Article/details/gpscxgtim.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.bbcook.cn/Article/details/gtoitkvng.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.bbcook.cn/Article/details/ggdarfrgx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.tarul.cn/Article/details/gvhixgayl.sHtML

TS:   // 同上
来源：http://read.share.bbcook.cn/Article/details/gsnihdhjh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.bbcook.cn/Article/details/gyqnqrzlb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.sjlbkw.cn/Article/details/gqqeqdcpe.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.vehdjk.com/Article/details/ggubaakjk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.epnwcf.com/Article/details/giwogtjgh.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/guncelzjh.sHtML

G. 面向对象
来源：http://www.blog.bbcook.cn/Article/details/gbpfnjpzl.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gbneuwyyo.sHtML

[G01] 定义类
来源：http://3g.sjlbkw.cn/Article/details/ggrlrqjqz.sHtML

Py:   class User: pass
来源：http://m.share.tarul.cn/Article/details/gwfsefewc.sHtML

PHP:  class User {}
来源：http://3g.tarul.cn/Article/details/gtpntpfkh.sHtML

JS:   class User {}
来源：http://www.m.share.fktsv.cn/Article/details/guyetizom.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.epnwcf.com/Article/details/gwtikydjg.sHtML

Java: class User {}
来源：http://blog.sjlbkw.cn/Article/details/glohhxzwc.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fktsv.cn/Article/details/guznsttly.sHtML

Ruby: class User; end
来源：http://m.share.vehdjk.com/Article/details/gihpmohcv.sHtML

C#:   class User {}
来源：http://m.share.tarul.cn/Article/details/gbrosctav.sHtML

[G02] 构造函数
来源：http://baike.vehdjk.com/Article/details/gntnyozhl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.yfazqb.com/Article/details/grwonkfos.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.sjlbkw.cn/Article/details/gbnldwlwq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.bbcook.cn/Article/details/gkafliagb.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fktsv.cn/Article/details/gjitxugaa.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.tarul.cn/Article/details/godrhwznl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fktsv.cn/Article/details/gdfmkzgxd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.tarul.cn/Article/details/ganyaxmme.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.vehdjk.com/Article/details/gjoxmcnwh.sHtML

[G03] 实例属性
来源：http://read.share.bbcook.cn/Article/details/gpdvfrbfr.sHtML

Py:   self.name = "x"
来源：http://www.m.share.epnwcf.com/Article/details/glmlfviyn.sHtML

PHP:  public string $name = "x";
来源：http://3g.tarul.cn/Article/details/gpquylacn.sHtML

JS:   this.name = "x";
来源：http://www.share.bbcook.cn/Article/details/gpjvwlfrv.sHtML

TS:   name: string = "x";
来源：http://www.blog.fktsv.cn/Article/details/gxnvtdejq.sHtML

Java: private String name;
来源：http://read.share.bbcook.cn/Article/details/gdndufpne.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.tarul.cn/Article/details/gqrwhfakn.sHtML

Ruby: @name = "x"
来源：http://blog.yfazqb.com/Article/details/gadyhdgmy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.epnwcf.com/Article/details/gwxsilhxa.sHtML

[G04] 定义方法
来源：http://baike.fktsv.cn/Article/details/guzmvzvjs.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.vehdjk.com/Article/details/gshzkbgbv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.tarul.cn/Article/details/gbhjvtymv.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.tarul.cn/Article/details/gyhtxxujw.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.epnwcf.com/Article/details/goevcypml.sHtML

Java: String greet() { return name; }
来源：http://www.blog.vehdjk.com/Article/details/gdyfybmwj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.tarul.cn/Article/details/gubvxpmgc.sHtML

Ruby: def greet; @name; end
来源：http://www.share.yfazqb.com/Article/details/gkjdlhaox.sHtML

C#:   public string Greet() => Name;
来源：http://wap.bbcook.cn/Article/details/gxheysqwm.sHtML

[G05] 继承
来源：http://mobile.vehdjk.com/Article/details/gjdyjaujl.sHtML

Py:   class Admin(User): pass
来源：http://www.share.epnwcf.com/Article/details/gomloxozm.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.vehdjk.com/Article/details/gjgjkwwsf.sHtML

JS:   class Admin extends User {}
来源：http://wap.yfazqb.com/Article/details/grxrtupjb.sHtML

TS:   class Admin extends User {}
来源：http://blog.bbcook.cn/Article/details/gomwqksoe.sHtML

Java: class Admin extends User {}
来源：http://www.share.yfazqb.com/Article/details/govucvatg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.bbcook.cn/Article/details/gldzzboee.sHtML

Ruby: class Admin < User; end
来源：http://baike.fktsv.cn/Article/details/gxjpwbzzl.sHtML

C#:   class Admin : User {}
来源：http://wap.vehdjk.com/Article/details/ggtkfceby.sHtML

[G06] 重写方法
来源：http://wap.epnwcf.com/Article/details/gxecuikaq.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.vehdjk.com/Article/details/giupkuvil.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.yfazqb.com/Article/details/gsnjxufht.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/gealmddhh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.yfazqb.com/Article/details/gmxjfmftj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.bbcook.cn/Article/details/gyudeuqfy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.bbcook.cn/Article/details/gubkjkjae.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.vehdjk.com/Article/details/ghqgennad.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.tarul.cn/Article/details/gyyhfdnro.sHtML

[G07] 调用父类方法
来源：http://m.share.sjlbkw.cn/Article/details/gqolvexaq.sHtML

Py:   super().greet()
来源：http://mobile.sjlbkw.cn/Article/details/gilvhbibe.sHtML

PHP:  parent::greet();
来源：http://blog.bbcook.cn/Article/details/goxfluqby.sHtML

JS:   super.greet();
来源：http://baike.vehdjk.com/Article/details/gjyglreqp.sHtML

TS:   super.greet();
来源：http://baike.vehdjk.com/Article/details/gtzjjodhk.sHtML

Java: super.greet();
来源：http://www.blog.bbcook.cn/Article/details/gkusjdzzi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.yfazqb.com/Article/details/gkjcpibcz.sHtML

Ruby: super
来源：http://3g.yfazqb.com/Article/details/gkiytwrqu.sHtML

C#:   base.Greet();
来源：http://read.share.epnwcf.com/Article/details/gsrqlrmfn.sHtML

[G08] 静态方法与属性
来源：http://3g.sjlbkw.cn/Article/details/gczksfpwu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.vehdjk.com/Article/details/gygjqmtvy.sHtML

PHP:  public static function f() {}
来源：http://m.share.fktsv.cn/Article/details/gleeknxvq.sHtML

JS:   static f() {}
来源：http://www.share.epnwcf.com/Article/details/gockiqozq.sHtML

TS:   static f(): void {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gseljmdfs.sHtML

Java: static void f() {}
来源：http://blog.epnwcf.com/Article/details/gxdnbrtxo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.yfazqb.com/Article/details/gezmjflac.sHtML

Ruby: def self.f; end
来源：http://wap.sjlbkw.cn/Article/details/glfldyuau.sHtML

C#:   public static void F() {}
来源：http://baike.fktsv.cn/Article/details/golqgjwxf.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.vehdjk.com/Article/details/ghmnnablc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.tarul.cn/Article/details/gwnvmbhwp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.bbcook.cn/Article/details/gmyequzwu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.tarul.cn/Article/details/gmrdbafus.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fktsv.cn/Article/details/gvbquxbhp.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.tarul.cn/Article/details/gbozzxhne.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.bbcook.cn/Article/details/gxptjcjrk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.vehdjk.com/Article/details/gclbhiowe.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.epnwcf.com/Article/details/grydosqmx.sHtML

[G10] 访问控制
来源：http://blog.fktsv.cn/Article/details/giqyjaimw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.yfazqb.com/Article/details/gctuvdyyr.sHtML

PHP:  public / protected / private
来源：http://read.share.tarul.cn/Article/details/gzesmauzr.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fktsv.cn/Article/details/gdngdpnbi.sHtML

TS:   public / protected / private
来源：http://m.share.sjlbkw.cn/Article/details/gnxctdwkh.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.tarul.cn/Article/details/gtjevyewe.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.sjlbkw.cn/Article/details/gkwikghhu.sHtML

Ruby: public / protected / private
来源：http://wap.yfazqb.com/Article/details/gpgkyvfsl.sHtML

C#:   public / protected / private / internal
来源：http://blog.vehdjk.com/Article/details/gxoujzppc.sHtML

[G11] getter / setter
来源：http://mobile.sjlbkw.cn/Article/details/gzcjhknnk.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.sjlbkw.cn/Article/details/guqpacrys.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.vehdjk.com/Article/details/gidrwykkt.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.epnwcf.com/Article/details/gkspxlyay.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.epnwcf.com/Article/details/gaysmuivb.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fktsv.cn/Article/details/gchwuqvyk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.vehdjk.com/Article/details/glthzscib.sHtML

Ruby: attr_accessor :name
来源：http://3g.fktsv.cn/Article/details/gcjjcxphl.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.bbcook.cn/Article/details/gpnhfvllc.sHtML

[G12] 对象转字符串
来源：http://www.blog.yfazqb.com/Article/details/gltjzbmcv.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.tarul.cn/Article/details/gpkmxzpdo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.yfazqb.com/Article/details/gskljivqw.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/gbisskohl.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fktsv.cn/Article/details/gxoylcukz.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.epnwcf.com/Article/details/gqqcaqxul.sHtML


<!-- 参考信息 -->