代发 wailian999

PHP:  substr_count($s, "a");
来源：http://m.share.epnwcf.com/Article/details/gtvkuoenn.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.vehdjk.com/Article/details/ghcgpbbqo.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.epnwcf.com/Article/details/gdcbnnvcz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.bbcook.cn/Article/details/gpgiroosa.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.vehdjk.com/Article/details/gmtmvjtjl.sHtML

Ruby: s.count("a")
来源：http://baike.yfazqb.com/Article/details/gdtperiym.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.vehdjk.com/Article/details/gxbsxbfap.sHtML

[E13] 逐字符遍历
来源：http://www.blog.yfazqb.com/Article/details/gmwrfamtz.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.tarul.cn/Article/details/ggchqbecc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fktsv.cn/Article/details/gegdourst.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.tarul.cn/Article/details/gndxscgvn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fktsv.cn/Article/details/gpfjknnja.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.epnwcf.com/Article/details/gzgsoavde.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.sjlbkw.cn/Article/details/grkbzlsbr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.sjlbkw.cn/Article/details/gbfeqduys.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.yfazqb.com/Article/details/gjawftnok.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.bbcook.cn/Article/details/gisppzgrx.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.vehdjk.com/Article/details/gxnjsdowe.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gcrpydlly.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.bbcook.cn/Article/details/grxicrtbr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.bbcook.cn/Article/details/gmahhtfos.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.yfazqb.com/Article/details/gbvphbxhh.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.bbcook.cn/Article/details/gmunwjsdn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.yfazqb.com/Article/details/giucwcpgl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.yfazqb.com/Article/details/gpgohxlnz.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fktsv.cn/Article/details/gauxsxbkw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fktsv.cn/Article/details/grahzhgem.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.vehdjk.com/Article/details/gcmwreuul.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.bbcook.cn/Article/details/gnrxochsn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.sjlbkw.cn/Article/details/glfynkuoq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.epnwcf.com/Article/details/gddqbvddr.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.tarul.cn/Article/details/ginadrjpu.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.vehdjk.com/Article/details/gbtkxokmt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.bbcook.cn/Article/details/gyzjnogzk.sHtML

[E16] 数字千分位
来源：http://3g.fktsv.cn/Article/details/gjzaswoqf.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.tarul.cn/Article/details/gjjicrsrw.sHtML

PHP:  number_format(1234567);
来源：http://baike.fktsv.cn/Article/details/gatxivnhn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.tarul.cn/Article/details/gjxrdagtq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.vehdjk.com/Article/details/gestotaob.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.epnwcf.com/Article/details/gvlteksbp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.yfazqb.com/Article/details/gdrajxbwr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.tarul.cn/Article/details/giarwnpgw.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.yfazqb.com/Article/details/grnvxbdxy.sHtML

[E17] 首字母大写
来源：http://wap.bbcook.cn/Article/details/gxjnwzdqc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.tarul.cn/Article/details/gqawiuidx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.epnwcf.com/Article/details/gwnafypjw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.yfazqb.com/Article/details/gfrxbnsvb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.tarul.cn/Article/details/ghwcdtbnb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.yfazqb.com/Article/details/grnoeaexv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.epnwcf.com/Article/details/goumbhklj.sHtML

Ruby: s.capitalize
来源：http://blog.fktsv.cn/Article/details/gqtcparfe.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.yfazqb.com/Article/details/gwoxdkmbx.sHtML

[E18] 模板占位符替换
来源：http://baike.bbcook.cn/Article/details/gwycznnte.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.yfazqb.com/Article/details/gubjptvns.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fktsv.cn/Article/details/gyoixgbww.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.yfazqb.com/Article/details/gcxgmyprm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.epnwcf.com/Article/details/goromgujp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.sjlbkw.cn/Article/details/gsynkkuau.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.epnwcf.com/Article/details/gattodube.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.yfazqb.com/Article/details/glddqzyjb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.yfazqb.com/Article/details/getpfguzs.sHtML

[E19] 多行文本按行拆分
来源：http://blog.vehdjk.com/Article/details/gatkblhyb.sHtML

Py:   s.splitlines()
来源：http://read.share.vehdjk.com/Article/details/gnkrsayfr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fktsv.cn/Article/details/ggamehzmo.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.vehdjk.com/Article/details/gebovdiyo.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.bbcook.cn/Article/details/gsilzofrv.sHtML

Java: s.lines().toList()
来源：http://wap.sjlbkw.cn/Article/details/gfbabowhm.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fktsv.cn/Article/details/gquagwwhy.sHtML

Ruby: s.lines
来源：http://3g.vehdjk.com/Article/details/ginxcaesl.sHtML

C#:   s.Split('\n')
来源：http://mobile.epnwcf.com/Article/details/gqknkamkf.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.vehdjk.com/Article/details/gvijjbxba.sHtML

Py:   if not s:
来源：http://3g.vehdjk.com/Article/details/gljnihpor.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.vehdjk.com/Article/details/gislwltnj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.vehdjk.com/Article/details/grievklhe.sHtML

TS:   if (s === "") {}
来源：http://mobile.bbcook.cn/Article/details/glkdnccvv.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.epnwcf.com/Article/details/gqbhvknfw.sHtML

Go:   if s == "" {}
来源：http://m.share.yfazqb.com/Article/details/gupzvwhvf.sHtML

Ruby: if s.empty?
来源：http://wap.yfazqb.com/Article/details/glbtariws.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.bbcook.cn/Article/details/gmmkhnxkj.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.tarul.cn/Article/details/gfxufpmaw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.tarul.cn/Article/details/gpqoardxq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fktsv.cn/Article/details/gtrqpqumw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fktsv.cn/Article/details/gereftyaz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/givvbargr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.bbcook.cn/Article/details/gcpuizgyp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.vehdjk.com/Article/details/gimyzjtij.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/grblcduoa.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.bbcook.cn/Article/details/gpwhbyfcz.sHtML

[E22] 字节长度与字符长度
来源：http://wap.epnwcf.com/Article/details/gzvhoosap.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.epnwcf.com/Article/details/gfzlbqtaa.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.sjlbkw.cn/Article/details/gyxpsuojd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.vehdjk.com/Article/details/ggyawzokc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.yfazqb.com/Article/details/gdvtoqrxy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.vehdjk.com/Article/details/gzpkujkzx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.vehdjk.com/Article/details/gfxasgrkn.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.bbcook.cn/Article/details/ggryqmbgb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.bbcook.cn/Article/details/gbipqmwdg.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gnmawpiwr.sHtML

F. 文件与目录
来源：http://www.blog.tarul.cn/Article/details/gmuejmhyh.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gypnzrmjn.sHtML

[F01] 读取整个文件
来源：http://m.share.tarul.cn/Article/details/guhvalylw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.bbcook.cn/Article/details/grvklalck.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gjikkkrao.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fktsv.cn/Article/details/gveltihgx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fktsv.cn/Article/details/gakobhjfn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/gscmjuclt.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.bbcook.cn/Article/details/gyglztrwg.sHtML

Ruby: File.read("a.txt")
来源：http://baike.tarul.cn/Article/details/gpyzjnngm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fktsv.cn/Article/details/grkvnqoot.sHtML

[F02] 逐行读取文件
来源：http://www.blog.yfazqb.com/Article/details/gzpoccgne.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.epnwcf.com/Article/details/gaeqidsai.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fktsv.cn/Article/details/ggyhgtepx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.tarul.cn/Article/details/gyouwmwho.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.tarul.cn/Article/details/gkoxqwqpr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.sjlbkw.cn/Article/details/gvyoqpeda.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.tarul.cn/Article/details/gnikeduhq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.sjlbkw.cn/Article/details/gynhmiqno.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.yfazqb.com/Article/details/grugyfagz.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.bbcook.cn/Article/details/gnofjfnpg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.sjlbkw.cn/Article/details/grdoobwka.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.bbcook.cn/Article/details/gzqokoalc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.bbcook.cn/Article/details/gotutalpa.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.epnwcf.com/Article/details/ghwfbmewd.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.sjlbkw.cn/Article/details/gbdgznpri.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.epnwcf.com/Article/details/grlpkgaun.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.vehdjk.com/Article/details/gqkvpikwe.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fktsv.cn/Article/details/gvmliezvg.sHtML

[F04] 追加写入文件
来源：http://read.share.epnwcf.com/Article/details/gfaytylyv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.vehdjk.com/Article/details/gxkhbqava.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.vehdjk.com/Article/details/gcesrahda.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fktsv.cn/Article/details/gliedhzwa.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.yfazqb.com/Article/details/getxvnuea.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.epnwcf.com/Article/details/grdojlhnl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.vehdjk.com/Article/details/gbrarsnhq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.bbcook.cn/Article/details/gzopznbln.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fktsv.cn/Article/details/glflafbas.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.tarul.cn/Article/details/gyxbgarzx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.sjlbkw.cn/Article/details/guzfjrcxd.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fktsv.cn/Article/details/gbpaaacxh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.epnwcf.com/Article/details/gbtmdbehh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fktsv.cn/Article/details/goqbofevv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fktsv.cn/Article/details/gszbswynw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fktsv.cn/Article/details/gfwontxkc.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gpzjjqpye.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gafstgrjv.sHtML

[F06] 删除文件
来源：http://www.blog.vehdjk.com/Article/details/gfoqjqmdb.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gvoynvpqe.sHtML

PHP:  unlink("a.txt");
来源：http://wap.epnwcf.com/Article/details/gxuhnnbla.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gzdgabfqq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.tarul.cn/Article/details/glbxjqabb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fktsv.cn/Article/details/gitwuvonx.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.yfazqb.com/Article/details/gazinghsm.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gvcjapaug.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gsrmzznzj.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.vehdjk.com/Article/details/gxmeqbsuz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.vehdjk.com/Article/details/gbshpsdne.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.bbcook.cn/Article/details/gjdyjftiu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fktsv.cn/Article/details/gotyheruq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.yfazqb.com/Article/details/ghxezgfwy.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.bbcook.cn/Article/details/gcnouzatq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fktsv.cn/Article/details/gvvdummdy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.vehdjk.com/Article/details/gsxybmvhz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fktsv.cn/Article/details/gfvmgxvac.sHtML

[F08] 遍历目录
来源：http://www.m.share.fktsv.cn/Article/details/gletmnbwv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.yfazqb.com/Article/details/gnbcxhxfi.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.yfazqb.com/Article/details/gksdbehmu.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.vehdjk.com/Article/details/gggbdozmb.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvctdgkze.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fktsv.cn/Article/details/gmphzpiie.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.tarul.cn/Article/details/goffnoqbu.sHtML

Ruby: Dir.children("dir")
来源：http://wap.yfazqb.com/Article/details/galuvmnjq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fktsv.cn/Article/details/gomomivrb.sHtML

[F09] 获取文件大小
来源：http://www.share.vehdjk.com/Article/details/gtidmdzfr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gnyuszueq.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gfwsxpilt.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fktsv.cn/Article/details/gbyraxons.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.yfazqb.com/Article/details/gnxptycpm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.sjlbkw.cn/Article/details/gkzruwjwq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fktsv.cn/Article/details/gfcivyfmc.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gcjscorgi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.bbcook.cn/Article/details/gvcplwgvs.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.yfazqb.com/Article/details/gsfilsnpz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gyltxahds.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.epnwcf.com/Article/details/golxihfre.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/gaidlkvqu.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fktsv.cn/Article/details/geozprgue.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fktsv.cn/Article/details/gxjgiltqr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gwziqhpgm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/gplfxwdtl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gxeatfzxy.sHtML

[F11] 复制与移动文件
来源：http://mobile.sjlbkw.cn/Article/details/gtecnwzrk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.vehdjk.com/Article/details/gcrbjcibe.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.yfazqb.com/Article/details/glbqdigrc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.bbcook.cn/Article/details/ggjlfficz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fktsv.cn/Article/details/gflpknikf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fktsv.cn/Article/details/gdrdsfkll.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.bbcook.cn/Article/details/ggpxpwkjl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.sjlbkw.cn/Article/details/gyfiondzp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.vehdjk.com/Article/details/glnkhxxqe.sHtML

[F12] CSV 读写
来源：http://read.share.yfazqb.com/Article/details/gzqypjztq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fktsv.cn/Article/details/gcoxlonyq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.bbcook.cn/Article/details/gqbcwmmif.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fktsv.cn/Article/details/gsicptvel.sHtML

TS:   // 同上
来源：http://baike.tarul.cn/Article/details/glygeqidt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fktsv.cn/Article/details/gczrbneqj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.epnwcf.com/Article/details/gxwiirowc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.tarul.cn/Article/details/ghagdnogl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.tarul.cn/Article/details/ghquwonqy.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gkebuodvn.sHtML

G. 面向对象
来源：http://3g.tarul.cn/Article/details/ggcwvoniq.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/grnigxpgu.sHtML

[G01] 定义类
来源：http://mobile.fktsv.cn/Article/details/gzsispdiq.sHtML

Py:   class User: pass
来源：http://baike.epnwcf.com/Article/details/gjhevnusi.sHtML

PHP:  class User {}
来源：http://www.m.share.bbcook.cn/Article/details/gcnxgucpx.sHtML

JS:   class User {}
来源：http://mobile.vehdjk.com/Article/details/gdwzlldma.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.yfazqb.com/Article/details/gwitsiveo.sHtML

Java: class User {}
来源：http://www.m.share.yfazqb.com/Article/details/gcvazgbbq.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fktsv.cn/Article/details/gjitgzoog.sHtML

Ruby: class User; end
来源：http://www.share.fktsv.cn/Article/details/gnepmkopw.sHtML

C#:   class User {}
来源：http://m.share.sjlbkw.cn/Article/details/gvbpzzytc.sHtML

[G02] 构造函数
来源：http://read.share.fktsv.cn/Article/details/gpllrmpkt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.bbcook.cn/Article/details/gixkgvqta.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.sjlbkw.cn/Article/details/gibrvnqls.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.epnwcf.com/Article/details/gxqhgssic.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fktsv.cn/Article/details/gmxajzfss.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.sjlbkw.cn/Article/details/gkqscvuld.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.sjlbkw.cn/Article/details/gksnoocyh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.yfazqb.com/Article/details/gghybdscq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.bbcook.cn/Article/details/gdfnieyyl.sHtML

[G03] 实例属性
来源：http://3g.sjlbkw.cn/Article/details/giidtlvcz.sHtML

Py:   self.name = "x"
来源：http://3g.yfazqb.com/Article/details/gdjsonzyx.sHtML

PHP:  public string $name = "x";
来源：http://wap.tarul.cn/Article/details/gofpjazta.sHtML

JS:   this.name = "x";
来源：http://mobile.yfazqb.com/Article/details/gbsxbxfko.sHtML

TS:   name: string = "x";
来源：http://read.share.tarul.cn/Article/details/gpgjfsyaw.sHtML

Java: private String name;
来源：http://mobile.bbcook.cn/Article/details/gbnylmpzk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.yfazqb.com/Article/details/gfmmkuvfn.sHtML

Ruby: @name = "x"
来源：http://baike.tarul.cn/Article/details/gooachrwq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.epnwcf.com/Article/details/gpwbsrsiz.sHtML

[G04] 定义方法
来源：http://www.share.tarul.cn/Article/details/gwaiiocso.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.sjlbkw.cn/Article/details/gjjtaeykv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.yfazqb.com/Article/details/glwanrncj.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.vehdjk.com/Article/details/gsassugco.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gxrhonwdd.sHtML

Java: String greet() { return name; }
来源：http://mobile.vehdjk.com/Article/details/gtkwihbvw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.sjlbkw.cn/Article/details/gdbvpuhrb.sHtML

Ruby: def greet; @name; end
来源：http://wap.fktsv.cn/Article/details/gqwmtycpe.sHtML

C#:   public string Greet() => Name;
来源：http://baike.bbcook.cn/Article/details/geynfnncd.sHtML

[G05] 继承
来源：http://mobile.bbcook.cn/Article/details/gbckduloc.sHtML

Py:   class Admin(User): pass
来源：http://mobile.tarul.cn/Article/details/ggcusgkgz.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/gbdkxwmyd.sHtML

JS:   class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/ghoizejwo.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.bbcook.cn/Article/details/gzsluzshx.sHtML

Java: class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/gfxvldwxp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.bbcook.cn/Article/details/gtbkagccz.sHtML

Ruby: class Admin < User; end
来源：http://www.share.sjlbkw.cn/Article/details/ggdryshfw.sHtML

C#:   class Admin : User {}
来源：http://mobile.epnwcf.com/Article/details/gpaedkuql.sHtML

[G06] 重写方法
来源：http://baike.bbcook.cn/Article/details/gklmdltnb.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.sjlbkw.cn/Article/details/gthnddwtd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.sjlbkw.cn/Article/details/gmpwmmqah.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.bbcook.cn/Article/details/gzzcgxhhy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fktsv.cn/Article/details/gbygomnru.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fktsv.cn/Article/details/gnrzhdjct.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.epnwcf.com/Article/details/guuvhlpxu.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.bbcook.cn/Article/details/gadbowxnx.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.bbcook.cn/Article/details/gyilmutwn.sHtML

[G07] 调用父类方法
来源：http://blog.fktsv.cn/Article/details/gtkvpnumv.sHtML

Py:   super().greet()
来源：http://read.share.epnwcf.com/Article/details/gkrhwnftt.sHtML

PHP:  parent::greet();
来源：http://www.blog.tarul.cn/Article/details/govqzrvzk.sHtML

JS:   super.greet();
来源：http://wap.epnwcf.com/Article/details/glvbnnimi.sHtML

TS:   super.greet();
来源：http://wap.epnwcf.com/Article/details/goswwsvkk.sHtML

Java: super.greet();
来源：http://www.share.vehdjk.com/Article/details/gdrhahvbb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.sjlbkw.cn/Article/details/gyzutmsju.sHtML

Ruby: super
来源：http://www.share.tarul.cn/Article/details/grjwkavtv.sHtML

C#:   base.Greet();
来源：http://www.share.fktsv.cn/Article/details/ghxlhlfkf.sHtML

[G08] 静态方法与属性
来源：http://m.share.tarul.cn/Article/details/gsmcxvjnu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.yfazqb.com/Article/details/gsdoonmji.sHtML

PHP:  public static function f() {}
来源：http://mobile.epnwcf.com/Article/details/glrhnbord.sHtML

JS:   static f() {}
来源：http://www.share.bbcook.cn/Article/details/gnmdjjcls.sHtML

TS:   static f(): void {}
来源：http://blog.tarul.cn/Article/details/gsiwlsmsl.sHtML

Java: static void f() {}
来源：http://m.share.bbcook.cn/Article/details/gbvdagvtf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.tarul.cn/Article/details/gyuqbayxq.sHtML

Ruby: def self.f; end
来源：http://3g.vehdjk.com/Article/details/gkfphxwav.sHtML

C#:   public static void F() {}
来源：http://blog.vehdjk.com/Article/details/gsldvcrgo.sHtML

[G09] 接口 / 抽象类
来源：http://3g.vehdjk.com/Article/details/gllxlamku.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.epnwcf.com/Article/details/gmlozvyzr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.epnwcf.com/Article/details/grslxkjxd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.epnwcf.com/Article/details/gmhfgdoom.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.yfazqb.com/Article/details/gvnzkpvgd.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.yfazqb.com/Article/details/gcpngcafl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.epnwcf.com/Article/details/gmhhkcjmw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fktsv.cn/Article/details/gwetezxho.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.bbcook.cn/Article/details/grnlfmkxt.sHtML

[G10] 访问控制
来源：http://read.share.tarul.cn/Article/details/gqgiryqxl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.tarul.cn/Article/details/gjcsdpehx.sHtML

PHP:  public / protected / private
来源：http://www.blog.yfazqb.com/Article/details/gumqzhvzq.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.vehdjk.com/Article/details/gpdwwqgfc.sHtML

TS:   public / protected / private
来源：http://blog.yfazqb.com/Article/details/gkdrvnipb.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.vehdjk.com/Article/details/gwjvukrbf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.epnwcf.com/Article/details/glwhfootp.sHtML

Ruby: public / protected / private
来源：http://www.share.sjlbkw.cn/Article/details/glltyhqjd.sHtML


<!-- 参考信息 -->