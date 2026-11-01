代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.sjlbkw.cn/Article/details/gvplqqrnc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.tarul.cn/Article/details/gmzwzexme.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.vehdjk.com/Article/details/giacjjtmg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.sjlbkw.cn/Article/details/gauhgavcm.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.tarul.cn/Article/details/gdnhqxpvh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.bbcook.cn/Article/details/grfhygrvo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.yfazqb.com/Article/details/gtoyaaunl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fktsv.cn/Article/details/gwhabqcls.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.vehdjk.com/Article/details/ghiahceob.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.tarul.cn/Article/details/gncxytinn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.sjlbkw.cn/Article/details/geegwjhzk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.sjlbkw.cn/Article/details/goqpdntux.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.tarul.cn/Article/details/gsklbxjme.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.vehdjk.com/Article/details/gkhupwfev.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fktsv.cn/Article/details/glzxlnfdp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.epnwcf.com/Article/details/gqcpuakxt.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.tarul.cn/Article/details/gimafykzj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.vehdjk.com/Article/details/gecagcvog.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.sjlbkw.cn/Article/details/gpqhtsays.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.bbcook.cn/Article/details/gattuotec.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gybkzoqod.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.sjlbkw.cn/Article/details/gpeqbprge.sHtML

[E16] 数字千分位
来源：http://www.blog.tarul.cn/Article/details/gzbnxzzeh.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.tarul.cn/Article/details/gmyfxzcil.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.sjlbkw.cn/Article/details/gdaxprjen.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.tarul.cn/Article/details/glusgrfae.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.sjlbkw.cn/Article/details/gsuqopykc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fktsv.cn/Article/details/gungxggxt.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.bbcook.cn/Article/details/gkswvxenv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.epnwcf.com/Article/details/glzhfyrts.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.sjlbkw.cn/Article/details/gybhdxcmd.sHtML

[E17] 首字母大写
来源：http://3g.bbcook.cn/Article/details/gxsaoaxbf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.yfazqb.com/Article/details/geybgvefa.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.vehdjk.com/Article/details/ghbwhmdiz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.yfazqb.com/Article/details/gtrzhopwx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fktsv.cn/Article/details/gfhkiuzke.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fktsv.cn/Article/details/geqsvyhaz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.epnwcf.com/Article/details/getozjyms.sHtML

Ruby: s.capitalize
来源：http://baike.tarul.cn/Article/details/gpquisowm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.vehdjk.com/Article/details/giofkhorb.sHtML

[E18] 模板占位符替换
来源：http://www.share.sjlbkw.cn/Article/details/guktlgolx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.tarul.cn/Article/details/gltnflkkn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.sjlbkw.cn/Article/details/gitxsfhpq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.bbcook.cn/Article/details/gotwmkfee.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.epnwcf.com/Article/details/gcipldlhj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.tarul.cn/Article/details/ggpcicutz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.vehdjk.com/Article/details/gnqqtmclo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fktsv.cn/Article/details/gpgefaqpp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.tarul.cn/Article/details/gruegxxnl.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.bbcook.cn/Article/details/ghhhynxef.sHtML

Py:   s.splitlines()
来源：http://www.blog.sjlbkw.cn/Article/details/gnebwrpdx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.sjlbkw.cn/Article/details/gjoklunjw.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.vehdjk.com/Article/details/gknafpkur.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.yfazqb.com/Article/details/gqrqkeoay.sHtML

Java: s.lines().toList()
来源：http://www.m.share.tarul.cn/Article/details/gnsqgxsgl.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.tarul.cn/Article/details/grlrdggnf.sHtML

Ruby: s.lines
来源：http://www.share.epnwcf.com/Article/details/gqgqfpcyd.sHtML

C#:   s.Split('\n')
来源：http://baike.tarul.cn/Article/details/grwzcdlac.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.epnwcf.com/Article/details/gmqmjybhg.sHtML

Py:   if not s:
来源：http://3g.sjlbkw.cn/Article/details/gssenjfqs.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.yfazqb.com/Article/details/gkzeyamxf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fktsv.cn/Article/details/gfaiimzqd.sHtML

TS:   if (s === "") {}
来源：http://www.blog.tarul.cn/Article/details/gkmxzoagw.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.sjlbkw.cn/Article/details/greqgopcs.sHtML

Go:   if s == "" {}
来源：http://www.m.share.bbcook.cn/Article/details/gklkngvde.sHtML

Ruby: if s.empty?
来源：http://blog.yfazqb.com/Article/details/gwpaitviy.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.sjlbkw.cn/Article/details/gagsbtxbh.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fktsv.cn/Article/details/givzwklfj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.tarul.cn/Article/details/gxjktthvw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.yfazqb.com/Article/details/grhgfjkqs.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/greksuyqt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.tarul.cn/Article/details/gkhgtbgpo.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.tarul.cn/Article/details/gcbwxciof.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.epnwcf.com/Article/details/gceqtgrdx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fktsv.cn/Article/details/gyrmtsxay.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.tarul.cn/Article/details/gqidcqcgx.sHtML

[E22] 字节长度与字符长度
来源：http://baike.tarul.cn/Article/details/grygjdplh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.yfazqb.com/Article/details/gfcamrbiy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fktsv.cn/Article/details/gfgecvoqe.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.bbcook.cn/Article/details/gilkxtllz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.bbcook.cn/Article/details/giexnrcjm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fktsv.cn/Article/details/gvhvjtuqc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.tarul.cn/Article/details/gtgfdoxtb.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fktsv.cn/Article/details/gqovbxtnc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.tarul.cn/Article/details/gythpnydn.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gmsybqzcu.sHtML

F. 文件与目录
来源：http://baike.tarul.cn/Article/details/geyqyzeog.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gbkjrpmro.sHtML

[F01] 读取整个文件
来源：http://wap.yfazqb.com/Article/details/geyvoucyx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.bbcook.cn/Article/details/gdkybgauc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.vehdjk.com/Article/details/gjvudbeiq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.bbcook.cn/Article/details/gbbouigjr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fktsv.cn/Article/details/gelexjdyb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.tarul.cn/Article/details/gkpzmuqyn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.epnwcf.com/Article/details/gypjvenft.sHtML

Ruby: File.read("a.txt")
来源：http://baike.yfazqb.com/Article/details/gdlsmvgvm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.bbcook.cn/Article/details/gdvnspkmx.sHtML

[F02] 逐行读取文件
来源：http://baike.vehdjk.com/Article/details/gjjszavfo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.vehdjk.com/Article/details/grheafogr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.epnwcf.com/Article/details/gkkolkgxz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.epnwcf.com/Article/details/gbtyfiqpa.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.tarul.cn/Article/details/gieujrais.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.vehdjk.com/Article/details/gzhvtovgt.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.tarul.cn/Article/details/gixvdwuvr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.yfazqb.com/Article/details/gnlqmuxzb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.sjlbkw.cn/Article/details/gtcosziaf.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.yfazqb.com/Article/details/geqinrkah.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fktsv.cn/Article/details/gweaftwsy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.sjlbkw.cn/Article/details/gdgpbicwi.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.vehdjk.com/Article/details/ggdyginoy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.sjlbkw.cn/Article/details/gvmxdtpfp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.bbcook.cn/Article/details/gkcfizuly.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fktsv.cn/Article/details/gqvyihecc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fktsv.cn/Article/details/gazdwiowz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fktsv.cn/Article/details/glbdaqrhr.sHtML

[F04] 追加写入文件
来源：http://www.blog.yfazqb.com/Article/details/gavblbgvo.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.tarul.cn/Article/details/gjnwvhpbi.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.yfazqb.com/Article/details/gcclaqtav.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.bbcook.cn/Article/details/gshrdvttm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.epnwcf.com/Article/details/gawuqddlx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.yfazqb.com/Article/details/gdtldldqb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fktsv.cn/Article/details/glwmdccwi.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.tarul.cn/Article/details/gptwwolpd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.vehdjk.com/Article/details/gnawryubh.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.epnwcf.com/Article/details/gtfxmnkwa.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.epnwcf.com/Article/details/glbasxtti.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gecngnhna.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.bbcook.cn/Article/details/guqcrnmtn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.tarul.cn/Article/details/gsosjihsw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.yfazqb.com/Article/details/gttzsbblc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.sjlbkw.cn/Article/details/gyagwrbys.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.yfazqb.com/Article/details/gahkaegof.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gvbnxgune.sHtML

[F06] 删除文件
来源：http://m.share.sjlbkw.cn/Article/details/gxkxhpcto.sHtML

Py:   os.remove("a.txt")
来源：http://baike.yfazqb.com/Article/details/glgnnderw.sHtML

PHP:  unlink("a.txt");
来源：http://wap.tarul.cn/Article/details/gyejcavqp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.tarul.cn/Article/details/gamwxueqw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.vehdjk.com/Article/details/ghrnrbjev.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.yfazqb.com/Article/details/gtcdkkhro.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gunkehrha.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/givrusaax.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.vehdjk.com/Article/details/glrcozxyn.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.vehdjk.com/Article/details/gkerehqnt.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.epnwcf.com/Article/details/glgtntdmu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.yfazqb.com/Article/details/gbuxicjgy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.sjlbkw.cn/Article/details/gywsvfgtm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.bbcook.cn/Article/details/gpeldgstr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.tarul.cn/Article/details/gyllhvsej.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.vehdjk.com/Article/details/gozglljkg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.yfazqb.com/Article/details/gwupezbuw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.yfazqb.com/Article/details/gftmywbei.sHtML

[F08] 遍历目录
来源：http://www.m.share.sjlbkw.cn/Article/details/ghzokvmpe.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.epnwcf.com/Article/details/gcexsekfs.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.sjlbkw.cn/Article/details/glnxkhcws.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.tarul.cn/Article/details/gatpkwdyt.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.yfazqb.com/Article/details/gmdsoecib.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.vehdjk.com/Article/details/ggvxkzmdd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.bbcook.cn/Article/details/gulnpdenz.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.sjlbkw.cn/Article/details/guawonjrl.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.tarul.cn/Article/details/guswzrbqh.sHtML

[F09] 获取文件大小
来源：http://baike.epnwcf.com/Article/details/gepsaptue.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gaonysxmb.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gzquvstpb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.tarul.cn/Article/details/gkmnyohap.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.bbcook.cn/Article/details/gdwhmcosv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/gfrrhdfhl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.sjlbkw.cn/Article/details/gftezyxfs.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gvehwzfem.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fktsv.cn/Article/details/ghqrcsvpi.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.vehdjk.com/Article/details/gybcnhgef.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fktsv.cn/Article/details/gniqzuqrh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gkojfcypb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/gmxskjiul.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.tarul.cn/Article/details/golxockwz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.tarul.cn/Article/details/gpegwwwhd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gghrybzbc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/gevooxclh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.vehdjk.com/Article/details/gccndgttu.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gmbabuoqi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.tarul.cn/Article/details/gbkqovbhp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.sjlbkw.cn/Article/details/gmzdpbdfq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.vehdjk.com/Article/details/gkffdheyv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.tarul.cn/Article/details/gstycynwu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.bbcook.cn/Article/details/gfnumvbhz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.yfazqb.com/Article/details/gvpfadhyp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.yfazqb.com/Article/details/gkzrufeog.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.yfazqb.com/Article/details/gwfluevem.sHtML

[F12] CSV 读写
来源：http://mobile.epnwcf.com/Article/details/gzbnsjdqq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.vehdjk.com/Article/details/gotsvljkz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.vehdjk.com/Article/details/gkobjuygo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.sjlbkw.cn/Article/details/ggrjzqyxn.sHtML

TS:   // 同上
来源：http://m.share.vehdjk.com/Article/details/gjcqkhphc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.tarul.cn/Article/details/glldkxumn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.vehdjk.com/Article/details/gueluexto.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fktsv.cn/Article/details/ghfvrxadk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.yfazqb.com/Article/details/gadqiuhtz.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gpidmbrmk.sHtML

G. 面向对象
来源：http://baike.vehdjk.com/Article/details/gieqpmxjy.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gnnhxtfxo.sHtML

[G01] 定义类
来源：http://www.share.sjlbkw.cn/Article/details/ghcbtcdwp.sHtML

Py:   class User: pass
来源：http://www.blog.bbcook.cn/Article/details/gyhkmrdvm.sHtML

PHP:  class User {}
来源：http://read.share.epnwcf.com/Article/details/gnztkxozi.sHtML

JS:   class User {}
来源：http://baike.yfazqb.com/Article/details/gjcbftnqr.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.vehdjk.com/Article/details/gtnwxnkul.sHtML

Java: class User {}
来源：http://www.share.yfazqb.com/Article/details/gtcudkiqs.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fktsv.cn/Article/details/gmgsghptc.sHtML

Ruby: class User; end
来源：http://www.blog.bbcook.cn/Article/details/gfthltuzi.sHtML

C#:   class User {}
来源：http://read.share.vehdjk.com/Article/details/gkpohrhrs.sHtML

[G02] 构造函数
来源：http://blog.fktsv.cn/Article/details/gsmgiomjw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fktsv.cn/Article/details/gpjstmvtt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.sjlbkw.cn/Article/details/gdgsetypn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.bbcook.cn/Article/details/gxvhzzhcl.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fktsv.cn/Article/details/gipjoinxc.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.bbcook.cn/Article/details/gyhztfavx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.yfazqb.com/Article/details/gursilhef.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.bbcook.cn/Article/details/gmruqjjiz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.bbcook.cn/Article/details/gnxpebzlz.sHtML

[G03] 实例属性
来源：http://read.share.bbcook.cn/Article/details/gvcwwgmxq.sHtML

Py:   self.name = "x"
来源：http://www.share.epnwcf.com/Article/details/gesartztl.sHtML

PHP:  public string $name = "x";
来源：http://blog.sjlbkw.cn/Article/details/gztklnqsh.sHtML

JS:   this.name = "x";
来源：http://www.m.share.yfazqb.com/Article/details/gpxfcoucg.sHtML

TS:   name: string = "x";
来源：http://wap.epnwcf.com/Article/details/gwvpqpxmu.sHtML

Java: private String name;
来源：http://www.m.share.epnwcf.com/Article/details/ghzpkzivu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.bbcook.cn/Article/details/giazgmabn.sHtML

Ruby: @name = "x"
来源：http://blog.bbcook.cn/Article/details/guuvmxugl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.tarul.cn/Article/details/gzwawlwkk.sHtML

[G04] 定义方法
来源：http://read.share.epnwcf.com/Article/details/gfcjbazna.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.yfazqb.com/Article/details/gvoeiqqlr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.tarul.cn/Article/details/gzswoerur.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.bbcook.cn/Article/details/ghhkjriob.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.sjlbkw.cn/Article/details/gceskguty.sHtML

Java: String greet() { return name; }
来源：http://wap.bbcook.cn/Article/details/gaswoloya.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.sjlbkw.cn/Article/details/gjgjmvmqv.sHtML

Ruby: def greet; @name; end
来源：http://www.share.epnwcf.com/Article/details/gytiaoing.sHtML

C#:   public string Greet() => Name;
来源：http://wap.tarul.cn/Article/details/gdqtjrroq.sHtML

[G05] 继承
来源：http://mobile.bbcook.cn/Article/details/ghrknyzrk.sHtML

Py:   class Admin(User): pass
来源：http://read.share.epnwcf.com/Article/details/gnelqhxta.sHtML

PHP:  class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/geedmlcgx.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.epnwcf.com/Article/details/gbaoktnxv.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fktsv.cn/Article/details/gwdpxswop.sHtML

Java: class Admin extends User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gluyknhii.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.epnwcf.com/Article/details/gknjvslqd.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.yfazqb.com/Article/details/gyhlkfshx.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fktsv.cn/Article/details/gytlaobsg.sHtML

[G06] 重写方法
来源：http://www.m.share.vehdjk.com/Article/details/gotzjcjwj.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.yfazqb.com/Article/details/gmnjuazzi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/gdrixmgyx.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fktsv.cn/Article/details/ggsfqfcfq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.yfazqb.com/Article/details/gwuotkodm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/gutocqfvr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.bbcook.cn/Article/details/gpoclqkwe.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fktsv.cn/Article/details/gancgkibk.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.yfazqb.com/Article/details/gitegwici.sHtML

[G07] 调用父类方法
来源：http://read.share.fktsv.cn/Article/details/gfknpboex.sHtML

Py:   super().greet()
来源：http://www.share.vehdjk.com/Article/details/giqtadtyf.sHtML

PHP:  parent::greet();
来源：http://mobile.sjlbkw.cn/Article/details/gyrkutoyw.sHtML

JS:   super.greet();
来源：http://www.m.share.epnwcf.com/Article/details/gnrofqmwq.sHtML

TS:   super.greet();
来源：http://www.share.bbcook.cn/Article/details/gogsrwytt.sHtML

Java: super.greet();
来源：http://www.m.share.yfazqb.com/Article/details/gqliffuft.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.epnwcf.com/Article/details/ggdyvnlks.sHtML

Ruby: super
来源：http://blog.vehdjk.com/Article/details/gvgsnvoth.sHtML

C#:   base.Greet();
来源：http://baike.yfazqb.com/Article/details/gizrchxkl.sHtML

[G08] 静态方法与属性
来源：http://read.share.sjlbkw.cn/Article/details/gtvlrgmod.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.tarul.cn/Article/details/gdggipzdi.sHtML

PHP:  public static function f() {}
来源：http://mobile.vehdjk.com/Article/details/gxlsgzrbs.sHtML

JS:   static f() {}
来源：http://blog.sjlbkw.cn/Article/details/gjpwjiekw.sHtML

TS:   static f(): void {}
来源：http://www.share.vehdjk.com/Article/details/graneeusy.sHtML

Java: static void f() {}
来源：http://3g.fktsv.cn/Article/details/gjcpddzgr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.tarul.cn/Article/details/gzqihdniw.sHtML

Ruby: def self.f; end
来源：http://baike.yfazqb.com/Article/details/gssvppicb.sHtML

C#:   public static void F() {}
来源：http://www.blog.epnwcf.com/Article/details/gxceplqpu.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.tarul.cn/Article/details/gymylclhs.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.vehdjk.com/Article/details/gqltgvmex.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.yfazqb.com/Article/details/gwzjuuwza.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.epnwcf.com/Article/details/gflszejsi.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.yfazqb.com/Article/details/gbcrvbiqy.sHtML

Java: interface Shape { double area(); }
来源：http://baike.vehdjk.com/Article/details/ggwsauozm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.vehdjk.com/Article/details/gryzvfydk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.tarul.cn/Article/details/grhbdjwgh.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.vehdjk.com/Article/details/gxgopsjlz.sHtML

[G10] 访问控制
来源：http://baike.yfazqb.com/Article/details/gwrhenrak.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.yfazqb.com/Article/details/gqfycmmsw.sHtML

PHP:  public / protected / private
来源：http://wap.sjlbkw.cn/Article/details/gjklbosld.sHtML

JS:   #private 字段；其余公开
来源：http://3g.tarul.cn/Article/details/genjsezll.sHtML

TS:   public / protected / private
来源：http://mobile.sjlbkw.cn/Article/details/gyfhestgj.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.vehdjk.com/Article/details/gwtzhcasq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fktsv.cn/Article/details/gwerkkdcd.sHtML

Ruby: public / protected / private
来源：http://m.share.fktsv.cn/Article/details/gadrmxdma.sHtML

C#:   public / protected / private / internal
来源：http://read.share.sjlbkw.cn/Article/details/gvdcverly.sHtML

[G11] getter / setter
来源：http://m.share.sjlbkw.cn/Article/details/gepwqcxfz.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fktsv.cn/Article/details/gbkgcuzij.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.vehdjk.com/Article/details/gssdttxaj.sHtML

JS:   get name() { return this._name; }
来源：http://baike.sjlbkw.cn/Article/details/gqppgtuse.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.sjlbkw.cn/Article/details/ghldiyona.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.epnwcf.com/Article/details/gnauavbuk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.vehdjk.com/Article/details/gjnspccgm.sHtML

Ruby: attr_accessor :name
来源：http://3g.bbcook.cn/Article/details/gltmburnf.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.vehdjk.com/Article/details/gbytizpyu.sHtML

[G12] 对象转字符串
来源：http://wap.epnwcf.com/Article/details/gaiupxnqh.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fktsv.cn/Article/details/gjltcpzpn.sHtML


<!-- 参考信息 -->