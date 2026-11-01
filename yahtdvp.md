代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gyrjgdfjr.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.vehdjk.com/Article/details/giuuonojn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fktsv.cn/Article/details/gtannifzk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fktsv.cn/Article/details/gfqythawy.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.fktsv.cn/Article/details/gpgoylnlf.sHtML

[E11] 反转字符串
来源：http://www.share.fktsv.cn/Article/details/gdgbxlwrn.sHtML

Py:   s[::-1]
来源：http://baike.tarul.cn/Article/details/gwosqdxob.sHtML

PHP:  strrev($s);
来源：http://read.share.fktsv.cn/Article/details/guneerbab.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.epnwcf.com/Article/details/ghppjcolt.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.fktsv.cn/Article/details/gidchwbiw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.yfazqb.com/Article/details/gtjihizpv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.yfazqb.com/Article/details/gailfsgto.sHtML

Ruby: s.reverse
来源：http://wap.vehdjk.com/Article/details/gfnmznpir.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.yfazqb.com/Article/details/ghzaqifmh.sHtML

[E12] 统计某字符出现次数
来源：http://blog.tarul.cn/Article/details/gvnmlysos.sHtML

Py:   s.count("a")
来源：http://baike.yfazqb.com/Article/details/gyycwigjj.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fktsv.cn/Article/details/gjjswwqvl.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.yfazqb.com/Article/details/ggpdwhkbu.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gphyzccem.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.yfazqb.com/Article/details/ghsmmtmsx.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.sjlbkw.cn/Article/details/gstkizlky.sHtML

Ruby: s.count("a")
来源：http://www.share.epnwcf.com/Article/details/gdkhghttd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.yfazqb.com/Article/details/gnjprpjfi.sHtML

[E13] 逐字符遍历
来源：http://read.share.yfazqb.com/Article/details/gcsdqbhts.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.yfazqb.com/Article/details/gxfqxzkkg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.bbcook.cn/Article/details/gpxbzittv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.epnwcf.com/Article/details/gddsghhsw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/ggrkbngya.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.bbcook.cn/Article/details/gtriiygra.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.epnwcf.com/Article/details/gtiznjznd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.vehdjk.com/Article/details/gxarazbrc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.yfazqb.com/Article/details/gplyvdnfx.sHtML

[E14] URL 编码与 Base64
来源：http://blog.yfazqb.com/Article/details/gxshyluof.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.epnwcf.com/Article/details/gmfymzsvz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.sjlbkw.cn/Article/details/guanibqzu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fktsv.cn/Article/details/gjkhjbutg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fktsv.cn/Article/details/gqdxflijs.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.bbcook.cn/Article/details/gwmqarmij.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fktsv.cn/Article/details/gycmrxoua.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.sjlbkw.cn/Article/details/gwjetjzge.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.bbcook.cn/Article/details/gnqfwlteb.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.sjlbkw.cn/Article/details/grbfehxzs.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.epnwcf.com/Article/details/gtgnvkhkf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.sjlbkw.cn/Article/details/gwegopwco.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.vehdjk.com/Article/details/gusovneth.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.vehdjk.com/Article/details/guncmptxx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.yfazqb.com/Article/details/gbggltnpk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fktsv.cn/Article/details/gdskjfrmn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.vehdjk.com/Article/details/gmakflnkg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.vehdjk.com/Article/details/gkonhgrqw.sHtML

[E16] 数字千分位
来源：http://m.share.vehdjk.com/Article/details/gapuuakvc.sHtML

Py:   f"{1234567:,}"
来源：http://baike.yfazqb.com/Article/details/gtsxhvnhr.sHtML

PHP:  number_format(1234567);
来源：http://3g.vehdjk.com/Article/details/gmrfbvwub.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.epnwcf.com/Article/details/gihcpccrz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.epnwcf.com/Article/details/gagecweqe.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.bbcook.cn/Article/details/gxynoeber.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.sjlbkw.cn/Article/details/gzsmakzcf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.yfazqb.com/Article/details/gmnwpjqof.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.sjlbkw.cn/Article/details/gxjrmydzb.sHtML

[E17] 首字母大写
来源：http://blog.epnwcf.com/Article/details/gswgqfjty.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.tarul.cn/Article/details/gmhfmwdek.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.vehdjk.com/Article/details/gyjtmyamc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.epnwcf.com/Article/details/gaipekfoh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.epnwcf.com/Article/details/gpssxvvrv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.epnwcf.com/Article/details/gqlshhwgo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.bbcook.cn/Article/details/guvxaabzr.sHtML

Ruby: s.capitalize
来源：http://wap.sjlbkw.cn/Article/details/grcbnicbp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.sjlbkw.cn/Article/details/gvfeyiovf.sHtML

[E18] 模板占位符替换
来源：http://www.blog.yfazqb.com/Article/details/gkqobhrel.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.epnwcf.com/Article/details/gvzsgxjjx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.tarul.cn/Article/details/gutobqzkl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.yfazqb.com/Article/details/gkpgabrkp.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.sjlbkw.cn/Article/details/gwoedjgww.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.epnwcf.com/Article/details/gzqlzhrzm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.sjlbkw.cn/Article/details/gusdeatoy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.vehdjk.com/Article/details/gxhwvvytx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.yfazqb.com/Article/details/gssgpjwya.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.yfazqb.com/Article/details/gqmdenqki.sHtML

Py:   s.splitlines()
来源：http://3g.epnwcf.com/Article/details/gfzmckqqz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.yfazqb.com/Article/details/gqchdvlfk.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.yfazqb.com/Article/details/ghpivwheb.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.vehdjk.com/Article/details/glerrnrdw.sHtML

Java: s.lines().toList()
来源：http://www.m.share.vehdjk.com/Article/details/geuzzvfqk.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fktsv.cn/Article/details/gvbsrehne.sHtML

Ruby: s.lines
来源：http://m.share.vehdjk.com/Article/details/gbdzmkjzb.sHtML

C#:   s.Split('\n')
来源：http://3g.epnwcf.com/Article/details/gfeaamakb.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.sjlbkw.cn/Article/details/gfusderlr.sHtML

Py:   if not s:
来源：http://m.share.sjlbkw.cn/Article/details/glmyvxoko.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.tarul.cn/Article/details/gtliwbbcd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.fktsv.cn/Article/details/grbwqxfjq.sHtML

TS:   if (s === "") {}
来源：http://3g.vehdjk.com/Article/details/gcopzymsf.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.tarul.cn/Article/details/gvxgfjioo.sHtML

Go:   if s == "" {}
来源：http://read.share.tarul.cn/Article/details/gdgaamszp.sHtML

Ruby: if s.empty?
来源：http://www.blog.vehdjk.com/Article/details/geikhtaqt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.bbcook.cn/Article/details/gcmmsnwes.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fktsv.cn/Article/details/gfvtyxuhv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.sjlbkw.cn/Article/details/gggsfrnmd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fktsv.cn/Article/details/gehccvtnk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/gkbuzcifz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.yfazqb.com/Article/details/gkmhjcnfd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fktsv.cn/Article/details/gfowfonyp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.vehdjk.com/Article/details/gmbjtnrmq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.tarul.cn/Article/details/gakulyvrj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/gslahvqpo.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fktsv.cn/Article/details/grtieohqz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fktsv.cn/Article/details/gudotiomz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.sjlbkw.cn/Article/details/goclaxpdn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.tarul.cn/Article/details/gmspeuxbs.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.yfazqb.com/Article/details/gbixsoaqi.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.epnwcf.com/Article/details/glknkfvdd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.bbcook.cn/Article/details/gtdkhypyb.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.sjlbkw.cn/Article/details/gvdzxglxj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.epnwcf.com/Article/details/ggwupmkpu.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gepjmcsmo.sHtML

F. 文件与目录
来源：http://www.blog.vehdjk.com/Article/details/gmwfmnbyl.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gnoirnedw.sHtML

[F01] 读取整个文件
来源：http://wap.fktsv.cn/Article/details/gkggkkcfy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.bbcook.cn/Article/details/ggizklpik.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gwaaqvvbv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.vehdjk.com/Article/details/gebhwygfr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.bbcook.cn/Article/details/gyawoajmn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.tarul.cn/Article/details/gthwyknsf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fktsv.cn/Article/details/gbdigmkbl.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gntaksouf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gmrmqmzch.sHtML

[F02] 逐行读取文件
来源：http://www.share.epnwcf.com/Article/details/geilzqprr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.sjlbkw.cn/Article/details/ggeqhknsj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.sjlbkw.cn/Article/details/gjpnrvucy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.tarul.cn/Article/details/gosttszvg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.epnwcf.com/Article/details/gnizdmczm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.epnwcf.com/Article/details/grfspqflc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fktsv.cn/Article/details/gsyvvxezl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.yfazqb.com/Article/details/gevnmtkdg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.tarul.cn/Article/details/gcfubjeqa.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.epnwcf.com/Article/details/glfoxzatl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.epnwcf.com/Article/details/gunnhxbda.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fktsv.cn/Article/details/gdaaoaxcb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fktsv.cn/Article/details/grsmpuuul.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmakhlgfe.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.yfazqb.com/Article/details/gtsjnbfib.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.yfazqb.com/Article/details/gtrywjavj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.vehdjk.com/Article/details/gjkhcjxae.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.tarul.cn/Article/details/gwdnegaru.sHtML

[F04] 追加写入文件
来源：http://read.share.fktsv.cn/Article/details/geyqdnkwz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.vehdjk.com/Article/details/gsknntycu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.tarul.cn/Article/details/gfibvfube.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.bbcook.cn/Article/details/gcmlkecwb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fktsv.cn/Article/details/gpjsxkimv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.bbcook.cn/Article/details/gcecryqjt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.yfazqb.com/Article/details/gziqzjpim.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.tarul.cn/Article/details/ggobmeutr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.bbcook.cn/Article/details/gbdblbuzw.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.vehdjk.com/Article/details/gooauagwm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.bbcook.cn/Article/details/grelmrdza.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.yfazqb.com/Article/details/gekkdorbp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fktsv.cn/Article/details/gqacdxive.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.tarul.cn/Article/details/gqimnjwya.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.sjlbkw.cn/Article/details/gdtbafwin.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.bbcook.cn/Article/details/gtuiwcezm.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gyjsledvh.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gxzmeyktr.sHtML

[F06] 删除文件
来源：http://m.share.epnwcf.com/Article/details/gznqvihqb.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gbtjxclsy.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gbtteqhhl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gmxbywwat.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.tarul.cn/Article/details/gwouhwdde.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fktsv.cn/Article/details/ggzxokhby.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.yfazqb.com/Article/details/ghhlltfdw.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.tarul.cn/Article/details/gtgnohyrd.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gcqwcikvt.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.vehdjk.com/Article/details/gsucozoae.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fktsv.cn/Article/details/gpyloxott.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fktsv.cn/Article/details/grctdoski.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.epnwcf.com/Article/details/gpotvqhzq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.vehdjk.com/Article/details/gaptrdrhy.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.sjlbkw.cn/Article/details/goozxiiff.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.vehdjk.com/Article/details/gaxzmxppl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.bbcook.cn/Article/details/gbwcvbwoa.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fktsv.cn/Article/details/gpkznqydk.sHtML

[F08] 遍历目录
来源：http://read.share.tarul.cn/Article/details/gkbtfrkwr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.epnwcf.com/Article/details/gzigmltor.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fktsv.cn/Article/details/ggtdoldvv.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.vehdjk.com/Article/details/gqfulhhrd.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.bbcook.cn/Article/details/gvqkreojv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyjwokfjx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.vehdjk.com/Article/details/gkagadxbt.sHtML

Ruby: Dir.children("dir")
来源：http://baike.tarul.cn/Article/details/grmmuyczr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.tarul.cn/Article/details/gwvlohbvb.sHtML

[F09] 获取文件大小
来源：http://mobile.bbcook.cn/Article/details/gbdvyyjjw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.bbcook.cn/Article/details/glmcucizc.sHtML

PHP:  filesize("a.txt");
来源：http://baike.bbcook.cn/Article/details/ghbaaqqfg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.bbcook.cn/Article/details/gwlmtnelg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.vehdjk.com/Article/details/giazrsavn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.sjlbkw.cn/Article/details/gmlccpwld.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.yfazqb.com/Article/details/gtksywbpo.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gmovbfrbf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.vehdjk.com/Article/details/gfsnnbdzy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.sjlbkw.cn/Article/details/gtbpoyjxz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/glljcldfn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.bbcook.cn/Article/details/glnldapah.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.bbcook.cn/Article/details/gogbxdupx.sHtML

TS:   path.extname("a.txt")
来源：http://3g.tarul.cn/Article/details/gndceqdpy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.bbcook.cn/Article/details/gtqeylkyq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gjtmqsfdt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gyhzlduyj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/gpdevysyz.sHtML

[F11] 复制与移动文件
来源：http://baike.bbcook.cn/Article/details/gwmgebsix.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gjgdhqfaq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.vehdjk.com/Article/details/gbsuwnjlz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gmylgcbrx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fktsv.cn/Article/details/guqvahxbs.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.tarul.cn/Article/details/gmnstgqvr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.yfazqb.com/Article/details/gkosxgobr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/gqdirpdfn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.tarul.cn/Article/details/glakwigea.sHtML

[F12] CSV 读写
来源：http://www.blog.yfazqb.com/Article/details/gfbmedmso.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.bbcook.cn/Article/details/gpzztdfmy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.yfazqb.com/Article/details/gpvfnbtef.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.tarul.cn/Article/details/gjofyppfd.sHtML

TS:   // 同上
来源：http://3g.vehdjk.com/Article/details/gdmljbmwk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.sjlbkw.cn/Article/details/gishqdncy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.epnwcf.com/Article/details/grjxahgqb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fktsv.cn/Article/details/ganbdbyvm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.vehdjk.com/Article/details/ggjsngmbc.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gfiutelij.sHtML

G. 面向对象
来源：http://m.share.fktsv.cn/Article/details/glgujqyma.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gqbfcorfj.sHtML

[G01] 定义类
来源：http://mobile.sjlbkw.cn/Article/details/gytfdcfrn.sHtML

Py:   class User: pass
来源：http://wap.tarul.cn/Article/details/gdgiiehto.sHtML

PHP:  class User {}
来源：http://m.share.tarul.cn/Article/details/gxunauact.sHtML

JS:   class User {}
来源：http://www.share.sjlbkw.cn/Article/details/gmovgagrg.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.bbcook.cn/Article/details/guywmonhx.sHtML

Java: class User {}
来源：http://wap.vehdjk.com/Article/details/gfewksmxj.sHtML

Go:   type User struct { Name string }
来源：http://www.share.epnwcf.com/Article/details/gxwctkqnu.sHtML

Ruby: class User; end
来源：http://3g.sjlbkw.cn/Article/details/gdyvvarvg.sHtML

C#:   class User {}
来源：http://baike.tarul.cn/Article/details/gwhghvnwi.sHtML

[G02] 构造函数
来源：http://www.m.share.tarul.cn/Article/details/gvkhmeafc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.yfazqb.com/Article/details/gowigtuvv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.vehdjk.com/Article/details/grkeulatq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.sjlbkw.cn/Article/details/ggbybomtl.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.bbcook.cn/Article/details/gpezcsfyn.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.yfazqb.com/Article/details/glweeldxq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fktsv.cn/Article/details/gozrqtcsr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.bbcook.cn/Article/details/givofaccv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.tarul.cn/Article/details/gxcqgbrwu.sHtML

[G03] 实例属性
来源：http://baike.fktsv.cn/Article/details/grgeuscrd.sHtML

Py:   self.name = "x"
来源：http://blog.epnwcf.com/Article/details/grmfplcue.sHtML

PHP:  public string $name = "x";
来源：http://baike.vehdjk.com/Article/details/ggrmglvzz.sHtML

JS:   this.name = "x";
来源：http://mobile.epnwcf.com/Article/details/gzricorop.sHtML

TS:   name: string = "x";
来源：http://www.m.share.epnwcf.com/Article/details/gnibekohc.sHtML

Java: private String name;
来源：http://baike.yfazqb.com/Article/details/gfjoywykd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.sjlbkw.cn/Article/details/ggdnoqmbx.sHtML

Ruby: @name = "x"
来源：http://www.share.tarul.cn/Article/details/gykjjnsoz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.vehdjk.com/Article/details/gcxwcsfdl.sHtML

[G04] 定义方法
来源：http://www.share.sjlbkw.cn/Article/details/gsbwauxkv.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.tarul.cn/Article/details/glvvkuhfr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.vehdjk.com/Article/details/gtslvwoil.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fktsv.cn/Article/details/geoparumv.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.bbcook.cn/Article/details/gonsgubkf.sHtML

Java: String greet() { return name; }
来源：http://m.share.vehdjk.com/Article/details/goitegiem.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.epnwcf.com/Article/details/ggcjpzepl.sHtML

Ruby: def greet; @name; end
来源：http://3g.bbcook.cn/Article/details/gwlbqxzlc.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.vehdjk.com/Article/details/gxsieylug.sHtML

[G05] 继承
来源：http://www.blog.sjlbkw.cn/Article/details/gyzpmevel.sHtML

Py:   class Admin(User): pass
来源：http://3g.fktsv.cn/Article/details/gyievwaml.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/gctowtksu.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fktsv.cn/Article/details/gfljnzdrb.sHtML

TS:   class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/gjrtsdckg.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fktsv.cn/Article/details/grodqlxpf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fktsv.cn/Article/details/gcecpidsl.sHtML

Ruby: class Admin < User; end
来源：http://read.share.bbcook.cn/Article/details/gibccmuhl.sHtML

C#:   class Admin : User {}
来源：http://wap.fktsv.cn/Article/details/gdvafxmem.sHtML

[G06] 重写方法
来源：http://mobile.bbcook.cn/Article/details/gwvuinwto.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.vehdjk.com/Article/details/gflhbrmzr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fktsv.cn/Article/details/gfmevuxqh.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.tarul.cn/Article/details/gjtmxlfrc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fktsv.cn/Article/details/gfqodxfdn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/gqofqewbc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.epnwcf.com/Article/details/ggswzunla.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.vehdjk.com/Article/details/gebomjmde.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.epnwcf.com/Article/details/gjlbwadbl.sHtML

[G07] 调用父类方法
来源：http://wap.fktsv.cn/Article/details/gvnfbxjvj.sHtML

Py:   super().greet()
来源：http://www.m.share.tarul.cn/Article/details/ghpqcgfev.sHtML

PHP:  parent::greet();
来源：http://read.share.tarul.cn/Article/details/gtpbmbxev.sHtML

JS:   super.greet();
来源：http://blog.bbcook.cn/Article/details/gpratxejv.sHtML

TS:   super.greet();
来源：http://baike.bbcook.cn/Article/details/gbxmnbvdj.sHtML

Java: super.greet();
来源：http://www.blog.vehdjk.com/Article/details/gjiwwpkix.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.epnwcf.com/Article/details/gfmcaswgu.sHtML

Ruby: super
来源：http://www.blog.epnwcf.com/Article/details/gguvavfnz.sHtML

C#:   base.Greet();
来源：http://3g.yfazqb.com/Article/details/gmpesughk.sHtML

[G08] 静态方法与属性
来源：http://m.share.sjlbkw.cn/Article/details/gzotsngwa.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.vehdjk.com/Article/details/grxajgvpv.sHtML

PHP:  public static function f() {}
来源：http://blog.fktsv.cn/Article/details/gmrpmstqm.sHtML

JS:   static f() {}
来源：http://3g.tarul.cn/Article/details/gqcbdmpjd.sHtML

TS:   static f(): void {}
来源：http://baike.yfazqb.com/Article/details/gdwujditq.sHtML

Java: static void f() {}
来源：http://www.m.share.yfazqb.com/Article/details/gmujipqpv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.epnwcf.com/Article/details/grclhpcpl.sHtML

Ruby: def self.f; end
来源：http://www.share.sjlbkw.cn/Article/details/gzmwkhqlo.sHtML

C#:   public static void F() {}
来源：http://mobile.epnwcf.com/Article/details/gcbwdcbfx.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.bbcook.cn/Article/details/gczfgrmbb.sHtML


<!-- 参考信息 -->