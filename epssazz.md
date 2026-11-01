代发 wailian999

Py:   for ch in s: print(ch)
来源：http://baike.fktsv.cn/Article/details/gjhqvllbk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.yfazqb.com/Article/details/galwzjhkq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.tarul.cn/Article/details/guadaoign.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fktsv.cn/Article/details/guemxlthh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.bbcook.cn/Article/details/gwdljisfw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.sjlbkw.cn/Article/details/gnrafjjyi.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.sjlbkw.cn/Article/details/gttstdeno.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fktsv.cn/Article/details/gymzuqkwe.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.bbcook.cn/Article/details/gljconwwr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fktsv.cn/Article/details/gppuewrqh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.tarul.cn/Article/details/gavoxbezu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.sjlbkw.cn/Article/details/goczlujel.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.tarul.cn/Article/details/gjfqiqtbb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.yfazqb.com/Article/details/gnyahephf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.yfazqb.com/Article/details/gimqigwky.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.epnwcf.com/Article/details/ggtrukoey.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.sjlbkw.cn/Article/details/gptjmzgwk.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.epnwcf.com/Article/details/glebhxfgk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.bbcook.cn/Article/details/gytdwwxbo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.tarul.cn/Article/details/gzftbppeg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.tarul.cn/Article/details/gocgjlwzj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.vehdjk.com/Article/details/govsykonm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.epnwcf.com/Article/details/gswzmhkoq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.yfazqb.com/Article/details/gujuvhlxq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.epnwcf.com/Article/details/gjrkbscwr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.vehdjk.com/Article/details/godbfwrqn.sHtML

[E16] 数字千分位
来源：http://m.share.bbcook.cn/Article/details/gdrxjbpuz.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.bbcook.cn/Article/details/gjmqrmktp.sHtML

PHP:  number_format(1234567);
来源：http://mobile.tarul.cn/Article/details/gstuwqfvg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.epnwcf.com/Article/details/ggyhzryqi.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.bbcook.cn/Article/details/giqymxouz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fktsv.cn/Article/details/gisitczgb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.vehdjk.com/Article/details/ggreodpye.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.sjlbkw.cn/Article/details/gzeejvdxr.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.tarul.cn/Article/details/gazsnvcar.sHtML

[E17] 首字母大写
来源：http://3g.yfazqb.com/Article/details/gqdtbpeys.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.vehdjk.com/Article/details/glfmafuhw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.sjlbkw.cn/Article/details/ghxvtbwfx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.yfazqb.com/Article/details/guqioffuz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.vehdjk.com/Article/details/gqqhzfpdb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.epnwcf.com/Article/details/goikgevxz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.sjlbkw.cn/Article/details/gjbyegblp.sHtML

Ruby: s.capitalize
来源：http://3g.sjlbkw.cn/Article/details/gexukswvo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.yfazqb.com/Article/details/gdoczumlb.sHtML

[E18] 模板占位符替换
来源：http://www.blog.tarul.cn/Article/details/gmdqdobey.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.tarul.cn/Article/details/gaszadvcd.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.sjlbkw.cn/Article/details/gcgkdblvl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.vehdjk.com/Article/details/gerheenxc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fktsv.cn/Article/details/getvltihs.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.tarul.cn/Article/details/gqkeljuct.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.vehdjk.com/Article/details/gerxpbwbg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.sjlbkw.cn/Article/details/gnrdwhmiz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.bbcook.cn/Article/details/ggguzjjjj.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fktsv.cn/Article/details/gtxczvmti.sHtML

Py:   s.splitlines()
来源：http://www.m.share.epnwcf.com/Article/details/gtzjqbibv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.epnwcf.com/Article/details/gznvcqbyy.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.bbcook.cn/Article/details/gnqqcpicr.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.yfazqb.com/Article/details/ggkwjsnzh.sHtML

Java: s.lines().toList()
来源：http://mobile.tarul.cn/Article/details/gmjmmvrue.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.yfazqb.com/Article/details/gbrouenjz.sHtML

Ruby: s.lines
来源：http://m.share.bbcook.cn/Article/details/gjrzxkmdz.sHtML

C#:   s.Split('\n')
来源：http://3g.vehdjk.com/Article/details/giegknbma.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fktsv.cn/Article/details/gfqeyydce.sHtML

Py:   if not s:
来源：http://blog.tarul.cn/Article/details/glhvugmbe.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.vehdjk.com/Article/details/ghfalfhxt.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.fktsv.cn/Article/details/gqzezmpav.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.vehdjk.com/Article/details/guyxghdau.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.epnwcf.com/Article/details/gkhsmjand.sHtML

Go:   if s == "" {}
来源：http://baike.vehdjk.com/Article/details/gmkbmvtxw.sHtML

Ruby: if s.empty?
来源：http://www.blog.sjlbkw.cn/Article/details/gmqircicm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fktsv.cn/Article/details/gavukcwoh.sHtML

[E21] 超长截断加省略号
来源：http://mobile.tarul.cn/Article/details/gjpetdwev.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fktsv.cn/Article/details/giiegqjnj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.yfazqb.com/Article/details/gfxxwmxkl.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/gazpmtlto.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.epnwcf.com/Article/details/gozofjjhb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.tarul.cn/Article/details/gskrgojna.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.bbcook.cn/Article/details/gospvzgpk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.bbcook.cn/Article/details/govzepzxx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/gealeerdb.sHtML

[E22] 字节长度与字符长度
来源：http://3g.tarul.cn/Article/details/gfdfmqmha.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.bbcook.cn/Article/details/glnjzzlci.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.epnwcf.com/Article/details/gxvaqmrbs.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.sjlbkw.cn/Article/details/gtnhutfvj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.sjlbkw.cn/Article/details/gfhxnbzzo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.epnwcf.com/Article/details/gglozqckx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.epnwcf.com/Article/details/gwuhlizsw.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fktsv.cn/Article/details/grelbamky.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fktsv.cn/Article/details/gayrvvjmc.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gxywndhzl.sHtML

F. 文件与目录
来源：http://www.m.share.fktsv.cn/Article/details/gupfljctc.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gguwfjruc.sHtML

[F01] 读取整个文件
来源：http://read.share.fktsv.cn/Article/details/gfbmaadxz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.epnwcf.com/Article/details/gkgbknock.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.vehdjk.com/Article/details/gvozhhwbh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.vehdjk.com/Article/details/gumvnwrea.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.sjlbkw.cn/Article/details/gtfpqawjc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.epnwcf.com/Article/details/guekmkrlz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.vehdjk.com/Article/details/gsiyrlwwm.sHtML

Ruby: File.read("a.txt")
来源：http://3g.yfazqb.com/Article/details/gvaqxvgyo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gfuewsmll.sHtML

[F02] 逐行读取文件
来源：http://read.share.yfazqb.com/Article/details/gtjmzbvbu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.vehdjk.com/Article/details/gmuijbgrq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.tarul.cn/Article/details/gjmzznide.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.yfazqb.com/Article/details/gsbitgiop.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.bbcook.cn/Article/details/gpropgnzp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fktsv.cn/Article/details/gmvrifkdv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fktsv.cn/Article/details/gbqmbivkr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.bbcook.cn/Article/details/gwkrovlog.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.yfazqb.com/Article/details/gpmbikqax.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.yfazqb.com/Article/details/gbexytkjx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.bbcook.cn/Article/details/gcexlbpwg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.epnwcf.com/Article/details/gqjvmsrqc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.tarul.cn/Article/details/ghzrmgfvd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.yfazqb.com/Article/details/gkdgmomgv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.bbcook.cn/Article/details/gqujheakz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.tarul.cn/Article/details/gkklgjgsf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.yfazqb.com/Article/details/gvvqxjnim.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.tarul.cn/Article/details/gjhcijbtp.sHtML

[F04] 追加写入文件
来源：http://mobile.fktsv.cn/Article/details/gvkqngrav.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.epnwcf.com/Article/details/gdgoepdbc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.sjlbkw.cn/Article/details/guiusdjpe.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.yfazqb.com/Article/details/gidpqywrj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.yfazqb.com/Article/details/gwqqqwgcn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.yfazqb.com/Article/details/gghevkiww.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.epnwcf.com/Article/details/ghxuuricr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.sjlbkw.cn/Article/details/ggzxoyrjk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.tarul.cn/Article/details/gdgddkbnf.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.vehdjk.com/Article/details/gsqbnacyo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.tarul.cn/Article/details/gznsbsvba.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.yfazqb.com/Article/details/ghqvtifjp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gfpdbyfus.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.vehdjk.com/Article/details/gpdfkjwqy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.epnwcf.com/Article/details/gpdfegkxu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.yfazqb.com/Article/details/gjsmminhd.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.bbcook.cn/Article/details/grqjyfsaq.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.vehdjk.com/Article/details/gayxbobkr.sHtML

[F06] 删除文件
来源：http://www.blog.bbcook.cn/Article/details/gunbrqmqs.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fktsv.cn/Article/details/grqtbjqor.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gvawadosq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gjrntjrwt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.fktsv.cn/Article/details/geeqxdkdc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.vehdjk.com/Article/details/gnvzscxjx.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gisctjhwq.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.yfazqb.com/Article/details/gwcylqbyo.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gtcvriegd.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.tarul.cn/Article/details/gaqlfwmub.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.epnwcf.com/Article/details/gqvezvvoc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.vehdjk.com/Article/details/gcdpkkegn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.tarul.cn/Article/details/gsysxvidx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.bbcook.cn/Article/details/ggjitdtiz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.sjlbkw.cn/Article/details/gpnsusiud.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.bbcook.cn/Article/details/gxwkhqldb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.epnwcf.com/Article/details/gddwalqed.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.bbcook.cn/Article/details/gylpuvzfa.sHtML

[F08] 遍历目录
来源：http://www.m.share.yfazqb.com/Article/details/gfbjesofw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.tarul.cn/Article/details/gtldquuah.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.epnwcf.com/Article/details/gnbdlnkkq.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.vehdjk.com/Article/details/ggocoscsh.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.sjlbkw.cn/Article/details/gznbpaejy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.yfazqb.com/Article/details/glsnqyczg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.bbcook.cn/Article/details/gyojojvjb.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.yfazqb.com/Article/details/gcddedqny.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.vehdjk.com/Article/details/gmdmsakjz.sHtML

[F09] 获取文件大小
来源：http://m.share.fktsv.cn/Article/details/gpuqzlphx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fktsv.cn/Article/details/glwbundpq.sHtML

PHP:  filesize("a.txt");
来源：http://wap.tarul.cn/Article/details/gscfhznce.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.bbcook.cn/Article/details/govvueofp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.epnwcf.com/Article/details/gkiovqnrj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.tarul.cn/Article/details/giegrixht.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.sjlbkw.cn/Article/details/gqbneacxs.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.epnwcf.com/Article/details/grjkeemvo.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.sjlbkw.cn/Article/details/gfinoehac.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.vehdjk.com/Article/details/grmmobubg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.vehdjk.com/Article/details/ghualdptg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.bbcook.cn/Article/details/gqnxqblqf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/goybyeohg.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gauugzkdk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.vehdjk.com/Article/details/ganrumizk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/gckrgklhf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/gdntvekzb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/glxlcmrjc.sHtML

[F11] 复制与移动文件
来源：http://www.blog.vehdjk.com/Article/details/gykolonji.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.sjlbkw.cn/Article/details/gpkopejlc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.yfazqb.com/Article/details/gfqvyuxtv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.vehdjk.com/Article/details/geveoylry.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.tarul.cn/Article/details/gkfrypdiw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.epnwcf.com/Article/details/grvipdeqs.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.yfazqb.com/Article/details/gjcndehxj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gogtwuhqv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.yfazqb.com/Article/details/ghmcmktbl.sHtML

[F12] CSV 读写
来源：http://baike.bbcook.cn/Article/details/gxsctgrkn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.yfazqb.com/Article/details/gspvrtkxq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fktsv.cn/Article/details/gllmnhbvr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fktsv.cn/Article/details/gklmqipku.sHtML

TS:   // 同上
来源：http://blog.bbcook.cn/Article/details/gsvtlkntt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fktsv.cn/Article/details/gszemkbtz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.vehdjk.com/Article/details/gpfjsnxeb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.vehdjk.com/Article/details/gpbuzmxsq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.epnwcf.com/Article/details/gckilaofm.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gdzhgiebr.sHtML

G. 面向对象
来源：http://3g.tarul.cn/Article/details/ggctzbhso.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gshuprfft.sHtML

[G01] 定义类
来源：http://read.share.fktsv.cn/Article/details/gjptdogff.sHtML

Py:   class User: pass
来源：http://www.blog.tarul.cn/Article/details/gvsubkvca.sHtML

PHP:  class User {}
来源：http://www.blog.bbcook.cn/Article/details/ghluxfyfa.sHtML

JS:   class User {}
来源：http://m.share.fktsv.cn/Article/details/gajlxmqpb.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.vehdjk.com/Article/details/gwgmnufdb.sHtML

Java: class User {}
来源：http://m.share.yfazqb.com/Article/details/gvxyinztu.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fktsv.cn/Article/details/ghopdgocw.sHtML

Ruby: class User; end
来源：http://wap.tarul.cn/Article/details/gjuguvlhv.sHtML

C#:   class User {}
来源：http://wap.epnwcf.com/Article/details/gvtrihctb.sHtML

[G02] 构造函数
来源：http://blog.sjlbkw.cn/Article/details/gmkwjrssv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.epnwcf.com/Article/details/gknsgiwtt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.tarul.cn/Article/details/gatnmmkby.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.vehdjk.com/Article/details/gsztmyabx.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fktsv.cn/Article/details/gzewievwt.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.tarul.cn/Article/details/gqkwlmrbz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fktsv.cn/Article/details/gpslkbmpu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.sjlbkw.cn/Article/details/gqhdebten.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.bbcook.cn/Article/details/gppchlraa.sHtML

[G03] 实例属性
来源：http://www.m.share.tarul.cn/Article/details/gthpujnti.sHtML

Py:   self.name = "x"
来源：http://m.share.vehdjk.com/Article/details/gbebpxpdf.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.tarul.cn/Article/details/gnxgbbtwg.sHtML

JS:   this.name = "x";
来源：http://baike.tarul.cn/Article/details/gmejilhjz.sHtML

TS:   name: string = "x";
来源：http://blog.epnwcf.com/Article/details/gzqaevxgi.sHtML

Java: private String name;
来源：http://m.share.tarul.cn/Article/details/gpwaxggvz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.sjlbkw.cn/Article/details/gyeoqdqrb.sHtML

Ruby: @name = "x"
来源：http://read.share.tarul.cn/Article/details/gkireirpo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.bbcook.cn/Article/details/gaxyvytjx.sHtML

[G04] 定义方法
来源：http://www.share.fktsv.cn/Article/details/gqiyllnvb.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.vehdjk.com/Article/details/gjfmisctp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.bbcook.cn/Article/details/gymchuniz.sHtML

JS:   greet() { return this.name; }
来源：http://3g.epnwcf.com/Article/details/ggbmiydgr.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.bbcook.cn/Article/details/gopanconu.sHtML

Java: String greet() { return name; }
来源：http://wap.vehdjk.com/Article/details/gshmqdkbr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.sjlbkw.cn/Article/details/goyqkzvnl.sHtML

Ruby: def greet; @name; end
来源：http://wap.sjlbkw.cn/Article/details/grataywrc.sHtML

C#:   public string Greet() => Name;
来源：http://wap.bbcook.cn/Article/details/gshhkfqia.sHtML

[G05] 继承
来源：http://www.blog.sjlbkw.cn/Article/details/gduzgqapj.sHtML

Py:   class Admin(User): pass
来源：http://blog.bbcook.cn/Article/details/gvdntejbm.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.vehdjk.com/Article/details/gaizhuqwy.sHtML

JS:   class Admin extends User {}
来源：http://mobile.sjlbkw.cn/Article/details/ggpsiured.sHtML

TS:   class Admin extends User {}
来源：http://read.share.sjlbkw.cn/Article/details/gnyafcwgq.sHtML

Java: class Admin extends User {}
来源：http://blog.yfazqb.com/Article/details/giajibclm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.sjlbkw.cn/Article/details/gomoednft.sHtML

Ruby: class Admin < User; end
来源：http://www.share.tarul.cn/Article/details/gxpmftyod.sHtML

C#:   class Admin : User {}
来源：http://www.share.vehdjk.com/Article/details/gfbjdmowg.sHtML

[G06] 重写方法
来源：http://mobile.yfazqb.com/Article/details/gklqbwvlg.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.bbcook.cn/Article/details/glhddgwsg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fktsv.cn/Article/details/gohsqfqhy.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.epnwcf.com/Article/details/guwmwlyeg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.epnwcf.com/Article/details/gqdvdedip.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fktsv.cn/Article/details/gjzggldso.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.epnwcf.com/Article/details/gpdhulavr.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fktsv.cn/Article/details/gukoiswxx.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.yfazqb.com/Article/details/gcvdjsabz.sHtML

[G07] 调用父类方法
来源：http://m.share.sjlbkw.cn/Article/details/gbxowlsli.sHtML

Py:   super().greet()
来源：http://m.share.yfazqb.com/Article/details/gxdnbsupw.sHtML

PHP:  parent::greet();
来源：http://www.m.share.epnwcf.com/Article/details/gjxjfcbft.sHtML

JS:   super.greet();
来源：http://www.share.tarul.cn/Article/details/gswsmavjj.sHtML

TS:   super.greet();
来源：http://baike.epnwcf.com/Article/details/giekzqgcn.sHtML

Java: super.greet();
来源：http://baike.fktsv.cn/Article/details/goetovlga.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.vehdjk.com/Article/details/goxhtmckh.sHtML

Ruby: super
来源：http://read.share.sjlbkw.cn/Article/details/gfphxektv.sHtML

C#:   base.Greet();
来源：http://www.m.share.yfazqb.com/Article/details/gsqwgcpme.sHtML

[G08] 静态方法与属性
来源：http://www.blog.tarul.cn/Article/details/gimeepfoj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fktsv.cn/Article/details/gmyaxhxzj.sHtML

PHP:  public static function f() {}
来源：http://www.blog.sjlbkw.cn/Article/details/gymtgjmky.sHtML

JS:   static f() {}
来源：http://m.share.yfazqb.com/Article/details/gysdviixq.sHtML

TS:   static f(): void {}
来源：http://read.share.yfazqb.com/Article/details/guggubxbc.sHtML

Java: static void f() {}
来源：http://3g.bbcook.cn/Article/details/gocqavsvh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.tarul.cn/Article/details/gafvtsjyo.sHtML

Ruby: def self.f; end
来源：http://blog.fktsv.cn/Article/details/ghmunsbqp.sHtML

C#:   public static void F() {}
来源：http://blog.fktsv.cn/Article/details/gdbnzeiby.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.vehdjk.com/Article/details/gormolfse.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.sjlbkw.cn/Article/details/ggjbzjjfd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.tarul.cn/Article/details/glfdlifeh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.tarul.cn/Article/details/gcfezigdf.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.epnwcf.com/Article/details/gsogwkmlu.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.tarul.cn/Article/details/grqithwny.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.epnwcf.com/Article/details/gxgtqhbyx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gpzwnewhh.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.tarul.cn/Article/details/gdfnftsdt.sHtML

[G10] 访问控制
来源：http://www.share.sjlbkw.cn/Article/details/ghuuiphds.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.bbcook.cn/Article/details/gobjkgaqw.sHtML

PHP:  public / protected / private
来源：http://www.share.fktsv.cn/Article/details/gjdnwflxn.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.yfazqb.com/Article/details/gctsaxbbs.sHtML

TS:   public / protected / private
来源：http://m.share.epnwcf.com/Article/details/gbmozvodp.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.epnwcf.com/Article/details/gcrxmikol.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.bbcook.cn/Article/details/gxctvezcu.sHtML

Ruby: public / protected / private
来源：http://3g.fktsv.cn/Article/details/gzrgsngfi.sHtML

C#:   public / protected / private / internal
来源：http://blog.bbcook.cn/Article/details/gkwyqyowl.sHtML

[G11] getter / setter
来源：http://www.blog.bbcook.cn/Article/details/ghyuxxzuj.sHtML

Py:   @property 与 @x.setter
来源：http://baike.sjlbkw.cn/Article/details/gontxzwau.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.vehdjk.com/Article/details/gyxyibmsb.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.epnwcf.com/Article/details/gxyppquno.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.bbcook.cn/Article/details/gwnwwvndl.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.tarul.cn/Article/details/grmolaxyi.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.tarul.cn/Article/details/gmzdaxcud.sHtML


<!-- 参考信息 -->