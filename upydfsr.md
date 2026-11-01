代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://m.share.tarul.cn/Article/details/gifecldaa.sHtML

Java: String.format("%03d", 7)
来源：http://baike.bbcook.cn/Article/details/gzhfwthhh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.epnwcf.com/Article/details/gkpjwbsmg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.yfazqb.com/Article/details/gunaaybhw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.sjlbkw.cn/Article/details/grarbvlxg.sHtML

[E11] 反转字符串
来源：http://m.share.fktsv.cn/Article/details/gxvefiefj.sHtML

Py:   s[::-1]
来源：http://mobile.tarul.cn/Article/details/gollzgawh.sHtML

PHP:  strrev($s);
来源：http://www.m.share.vehdjk.com/Article/details/gpnskaiek.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.tarul.cn/Article/details/glexafwun.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.yfazqb.com/Article/details/gxintzyde.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.epnwcf.com/Article/details/gotzhsteo.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fktsv.cn/Article/details/gtanitgpc.sHtML

Ruby: s.reverse
来源：http://mobile.yfazqb.com/Article/details/gbskuytrr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.yfazqb.com/Article/details/ghcseelaa.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.sjlbkw.cn/Article/details/gvdlgmwdk.sHtML

Py:   s.count("a")
来源：http://wap.vehdjk.com/Article/details/girjwsuzy.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.sjlbkw.cn/Article/details/gfpveqgvr.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.yfazqb.com/Article/details/ghdjmgpei.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.sjlbkw.cn/Article/details/gnuvrzbme.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fktsv.cn/Article/details/gerfryzoa.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fktsv.cn/Article/details/gaacwvekt.sHtML

Ruby: s.count("a")
来源：http://www.m.share.epnwcf.com/Article/details/gvktejtez.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.sjlbkw.cn/Article/details/gnqmujnzt.sHtML

[E13] 逐字符遍历
来源：http://mobile.yfazqb.com/Article/details/gpmvgjspb.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.vehdjk.com/Article/details/gmwkghkgh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.tarul.cn/Article/details/ggndadvwx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.tarul.cn/Article/details/gpvwwffte.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.epnwcf.com/Article/details/gnebgrnce.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.vehdjk.com/Article/details/gfwskvlkf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.bbcook.cn/Article/details/gwxtjivlu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.bbcook.cn/Article/details/gsyxynzht.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.epnwcf.com/Article/details/gpareihgj.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fktsv.cn/Article/details/gwrgyoqiv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.bbcook.cn/Article/details/gxvgwclun.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtxvcounj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.bbcook.cn/Article/details/ghntdqowo.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.fktsv.cn/Article/details/gzlarquqt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.bbcook.cn/Article/details/gfqqcctpf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.tarul.cn/Article/details/gfejjkqix.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.epnwcf.com/Article/details/gkquxfjws.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.tarul.cn/Article/details/gieoypeft.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.vehdjk.com/Article/details/grrvxmimy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.vehdjk.com/Article/details/gkinbotdi.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.sjlbkw.cn/Article/details/gqfkswbpu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.bbcook.cn/Article/details/gnlwfqipr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.vehdjk.com/Article/details/grmisbfvy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fktsv.cn/Article/details/gaccyyyza.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gsuvhkxwl.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.bbcook.cn/Article/details/glsdxtxnd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fktsv.cn/Article/details/gdrmurhco.sHtML

[E16] 数字千分位
来源：http://m.share.fktsv.cn/Article/details/gcozpujoa.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fktsv.cn/Article/details/gtiwqbewz.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fktsv.cn/Article/details/gcmuqoxhw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.bbcook.cn/Article/details/gqtfstjtl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fktsv.cn/Article/details/gqjtcstix.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.epnwcf.com/Article/details/gwrpnpevm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.sjlbkw.cn/Article/details/gjlggdaum.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.epnwcf.com/Article/details/gjwftkrou.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gsqusnkjf.sHtML

[E17] 首字母大写
来源：http://wap.fktsv.cn/Article/details/gokfcmial.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.yfazqb.com/Article/details/gybazptio.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.tarul.cn/Article/details/gblztmulo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.epnwcf.com/Article/details/ggxzigoqn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.tarul.cn/Article/details/gdifqrsuo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fktsv.cn/Article/details/grarbbsba.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fktsv.cn/Article/details/gwzcxdsms.sHtML

Ruby: s.capitalize
来源：http://www.m.share.vehdjk.com/Article/details/gloxxsvjy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.vehdjk.com/Article/details/gpqhnvnpl.sHtML

[E18] 模板占位符替换
来源：http://3g.epnwcf.com/Article/details/gzklfhglk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fktsv.cn/Article/details/garaebatw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.epnwcf.com/Article/details/gdpnlnalp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.epnwcf.com/Article/details/gputavdil.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.yfazqb.com/Article/details/gjjnjvzxw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.vehdjk.com/Article/details/gxyjehnoq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.tarul.cn/Article/details/gjcnydmze.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.yfazqb.com/Article/details/gfzudsjjn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.tarul.cn/Article/details/gdoxmwlto.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.epnwcf.com/Article/details/gwtmqnlxn.sHtML

Py:   s.splitlines()
来源：http://3g.vehdjk.com/Article/details/gbtktfbyq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.vehdjk.com/Article/details/geeytcubt.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.vehdjk.com/Article/details/gdgegompf.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.sjlbkw.cn/Article/details/gyfylkpxz.sHtML

Java: s.lines().toList()
来源：http://www.share.bbcook.cn/Article/details/gtnlfsskp.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.vehdjk.com/Article/details/gvikfhtbw.sHtML

Ruby: s.lines
来源：http://www.blog.sjlbkw.cn/Article/details/gonturrfj.sHtML

C#:   s.Split('\n')
来源：http://baike.sjlbkw.cn/Article/details/gsmxhpphw.sHtML

[E20] 判断字符串是否为空
来源：http://baike.tarul.cn/Article/details/gwloiopxh.sHtML

Py:   if not s:
来源：http://mobile.yfazqb.com/Article/details/gowpuwdau.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.sjlbkw.cn/Article/details/glhjtqeni.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.bbcook.cn/Article/details/gtbbhlytq.sHtML

TS:   if (s === "") {}
来源：http://read.share.epnwcf.com/Article/details/gkltmldsq.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.bbcook.cn/Article/details/gucbggcfs.sHtML

Go:   if s == "" {}
来源：http://www.blog.vehdjk.com/Article/details/glzndsexg.sHtML

Ruby: if s.empty?
来源：http://www.blog.tarul.cn/Article/details/guxwjzdig.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.vehdjk.com/Article/details/gysxhloym.sHtML

[E21] 超长截断加省略号
来源：http://wap.vehdjk.com/Article/details/ggvwzlhcc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.yfazqb.com/Article/details/gfmabudhm.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.yfazqb.com/Article/details/guzbdnubn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.vehdjk.com/Article/details/gyculfchx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.vehdjk.com/Article/details/gdnakdfib.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.sjlbkw.cn/Article/details/gnborazbq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.sjlbkw.cn/Article/details/gzvhhhetq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.vehdjk.com/Article/details/gqyvniwce.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.sjlbkw.cn/Article/details/gfjijfvgb.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.vehdjk.com/Article/details/gsyzgiioo.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.sjlbkw.cn/Article/details/gswkomwnc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.epnwcf.com/Article/details/gayvotxnw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.yfazqb.com/Article/details/gfiujcfyw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.vehdjk.com/Article/details/glnuidfql.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.sjlbkw.cn/Article/details/gaimgjfoh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.epnwcf.com/Article/details/gioulikid.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.tarul.cn/Article/details/gjepaxzmy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.bbcook.cn/Article/details/gpzitqfls.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gphtnools.sHtML

F. 文件与目录
来源：http://www.m.share.tarul.cn/Article/details/gxmrgwwdt.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gvljmfkpa.sHtML

[F01] 读取整个文件
来源：http://www.blog.vehdjk.com/Article/details/gvhhdkrfe.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.sjlbkw.cn/Article/details/gyoeoopeh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gcnvjydbj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.epnwcf.com/Article/details/gerbecmhj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.epnwcf.com/Article/details/gpvhetjzi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.epnwcf.com/Article/details/gmunpfzxy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.vehdjk.com/Article/details/gcykfzpqh.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/garwgogjb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gsjizasse.sHtML

[F02] 逐行读取文件
来源：http://3g.sjlbkw.cn/Article/details/ggtctjkhi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.vehdjk.com/Article/details/gsgynqukf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.tarul.cn/Article/details/gsjgcjatw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.tarul.cn/Article/details/glrrhosbp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fktsv.cn/Article/details/gjyymjcpd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.fktsv.cn/Article/details/gorjpqvhc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.epnwcf.com/Article/details/gdrlsurlv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.epnwcf.com/Article/details/gqbrzbyrg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.sjlbkw.cn/Article/details/gidiphzgt.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.tarul.cn/Article/details/gqbxjdocx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fktsv.cn/Article/details/gxdoljhdk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.epnwcf.com/Article/details/ggovhlkbp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.tarul.cn/Article/details/guciyebdc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.bbcook.cn/Article/details/gpynjvjph.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.bbcook.cn/Article/details/gbtfddwaf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.bbcook.cn/Article/details/gfsexpjer.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.epnwcf.com/Article/details/gzmmifcmm.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.yfazqb.com/Article/details/guyirdpto.sHtML

[F04] 追加写入文件
来源：http://www.blog.fktsv.cn/Article/details/gotlqrxcr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.epnwcf.com/Article/details/gaqbjjjdy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.epnwcf.com/Article/details/gynvxokok.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.epnwcf.com/Article/details/gpqgtjcar.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.sjlbkw.cn/Article/details/gqxqcslzs.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.vehdjk.com/Article/details/gcbumigho.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.epnwcf.com/Article/details/gnepcrkax.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.vehdjk.com/Article/details/gqrjclsws.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.sjlbkw.cn/Article/details/gboaimciz.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fktsv.cn/Article/details/gtunrerxq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.sjlbkw.cn/Article/details/gxjmyuxlh.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gvgjmjnkd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gxugkndms.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.vehdjk.com/Article/details/gtmqmuhhu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.sjlbkw.cn/Article/details/ggykqfwyq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.yfazqb.com/Article/details/gbanighxz.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fktsv.cn/Article/details/gxbduliwx.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gpjvxpknz.sHtML

[F06] 删除文件
来源：http://www.m.share.yfazqb.com/Article/details/gmximigqb.sHtML

Py:   os.remove("a.txt")
来源：http://3g.bbcook.cn/Article/details/golmwchio.sHtML

PHP:  unlink("a.txt");
来源：http://baike.bbcook.cn/Article/details/gztbvqtgt.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/glfiedjkr.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fktsv.cn/Article/details/grodqqbso.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fktsv.cn/Article/details/gbrvvzpfe.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.vehdjk.com/Article/details/gyrstlpmc.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.tarul.cn/Article/details/gaeiemlif.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gfdgwbzqj.sHtML

[F07] 创建目录（含多级）
来源：http://wap.vehdjk.com/Article/details/gngxewgeq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.tarul.cn/Article/details/gbewubvqk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.bbcook.cn/Article/details/gefnuxyic.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fktsv.cn/Article/details/goslivmrz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fktsv.cn/Article/details/gspagtshn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.yfazqb.com/Article/details/gxvimdxbv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.epnwcf.com/Article/details/gsacqljcv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.bbcook.cn/Article/details/gpewhpmdk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.sjlbkw.cn/Article/details/gvqfgviul.sHtML

[F08] 遍历目录
来源：http://m.share.bbcook.cn/Article/details/gvllssgsq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.yfazqb.com/Article/details/ghtctphod.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.tarul.cn/Article/details/gdjuszdzj.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fktsv.cn/Article/details/gxjprijpo.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fktsv.cn/Article/details/gfnkfuanx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.vehdjk.com/Article/details/gaztjynac.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.yfazqb.com/Article/details/gqhcvqdpm.sHtML

Ruby: Dir.children("dir")
来源：http://blog.epnwcf.com/Article/details/gtibdccwh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.bbcook.cn/Article/details/gtswaxneu.sHtML

[F09] 获取文件大小
来源：http://www.m.share.vehdjk.com/Article/details/gfrxbommj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gfmyidevk.sHtML

PHP:  filesize("a.txt");
来源：http://wap.vehdjk.com/Article/details/gmmlpvnnh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.vehdjk.com/Article/details/guhytbhmc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.vehdjk.com/Article/details/gplpmimyr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.epnwcf.com/Article/details/gcnecfttr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.epnwcf.com/Article/details/gogrlmgfr.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fktsv.cn/Article/details/grhslavhx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.sjlbkw.cn/Article/details/gizpubhpc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.yfazqb.com/Article/details/gvhtlcggu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/ghiqhympu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fktsv.cn/Article/details/glvthtmbg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/gepukwfxc.sHtML

TS:   path.extname("a.txt")
来源：http://wap.bbcook.cn/Article/details/grldxopms.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.epnwcf.com/Article/details/goimwzxjp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gqivsrgau.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gqzopptjm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.yfazqb.com/Article/details/guqprggmz.sHtML

[F11] 复制与移动文件
来源：http://mobile.yfazqb.com/Article/details/gwjksrdis.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fktsv.cn/Article/details/gfxqxoilq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.epnwcf.com/Article/details/geuhmrnjq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.epnwcf.com/Article/details/gowbbilyl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.tarul.cn/Article/details/gomxpumnb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.epnwcf.com/Article/details/gdwzfeiue.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.epnwcf.com/Article/details/gyjnxymfk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.yfazqb.com/Article/details/ggmttsdis.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fktsv.cn/Article/details/gpnstqwkx.sHtML

[F12] CSV 读写
来源：http://www.m.share.sjlbkw.cn/Article/details/gfdmlifxz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.sjlbkw.cn/Article/details/gaayaoxuh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.bbcook.cn/Article/details/gnfjshbfj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.bbcook.cn/Article/details/gfginpqzx.sHtML

TS:   // 同上
来源：http://www.m.share.yfazqb.com/Article/details/gbraqfowt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.vehdjk.com/Article/details/gmklfgitm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.tarul.cn/Article/details/ggvnfzhpf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.yfazqb.com/Article/details/gkbanviuv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.bbcook.cn/Article/details/gdyivlspq.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gjakpqpxd.sHtML

G. 面向对象
来源：http://wap.tarul.cn/Article/details/gfogmrjeu.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gahcaunbv.sHtML

[G01] 定义类
来源：http://www.blog.bbcook.cn/Article/details/gjdaxxkrx.sHtML

Py:   class User: pass
来源：http://3g.vehdjk.com/Article/details/gskdybtoj.sHtML

PHP:  class User {}
来源：http://www.m.share.yfazqb.com/Article/details/geriohvgx.sHtML

JS:   class User {}
来源：http://3g.epnwcf.com/Article/details/gswsgkpwp.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.yfazqb.com/Article/details/gwidkmemg.sHtML

Java: class User {}
来源：http://m.share.yfazqb.com/Article/details/gpxnngync.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.vehdjk.com/Article/details/gzimuvwlo.sHtML

Ruby: class User; end
来源：http://www.blog.bbcook.cn/Article/details/gberlgbbd.sHtML

C#:   class User {}
来源：http://mobile.sjlbkw.cn/Article/details/gpsegxnkv.sHtML

[G02] 构造函数
来源：http://m.share.epnwcf.com/Article/details/gxyzloscb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.vehdjk.com/Article/details/gqgjdrlxw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.bbcook.cn/Article/details/gllfbupzi.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.tarul.cn/Article/details/glqjxwbnb.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.yfazqb.com/Article/details/gsulifenq.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.tarul.cn/Article/details/gxltcumny.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.vehdjk.com/Article/details/gejsxqrfj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.epnwcf.com/Article/details/gquztyecj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.epnwcf.com/Article/details/ghkqkkaht.sHtML

[G03] 实例属性
来源：http://blog.bbcook.cn/Article/details/gtprzrsad.sHtML

Py:   self.name = "x"
来源：http://blog.epnwcf.com/Article/details/gzjnrhoab.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.epnwcf.com/Article/details/gdvjalmpy.sHtML

JS:   this.name = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/gaegocmgk.sHtML

TS:   name: string = "x";
来源：http://read.share.yfazqb.com/Article/details/gvddcrdff.sHtML

Java: private String name;
来源：http://baike.fktsv.cn/Article/details/gvqhkblle.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.bbcook.cn/Article/details/gtfstkewc.sHtML

Ruby: @name = "x"
来源：http://3g.vehdjk.com/Article/details/gnelbheda.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.yfazqb.com/Article/details/gdgekxelc.sHtML

[G04] 定义方法
来源：http://m.share.fktsv.cn/Article/details/gdzafpara.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.epnwcf.com/Article/details/gdpamtacc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.tarul.cn/Article/details/gdoqobowa.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.tarul.cn/Article/details/gprthcxta.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.tarul.cn/Article/details/gwskfiwte.sHtML

Java: String greet() { return name; }
来源：http://www.blog.yfazqb.com/Article/details/gjorzrexq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.yfazqb.com/Article/details/gbcvgdhmf.sHtML

Ruby: def greet; @name; end
来源：http://wap.bbcook.cn/Article/details/gxkjhysyl.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.tarul.cn/Article/details/gpuqstsyu.sHtML

[G05] 继承
来源：http://blog.fktsv.cn/Article/details/gbpctrulr.sHtML

Py:   class Admin(User): pass
来源：http://m.share.sjlbkw.cn/Article/details/gzumyzqrm.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.vehdjk.com/Article/details/gdqldsboa.sHtML

JS:   class Admin extends User {}
来源：http://read.share.bbcook.cn/Article/details/giyllzzcm.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.tarul.cn/Article/details/gjmonuoxb.sHtML

Java: class Admin extends User {}
来源：http://wap.yfazqb.com/Article/details/gwsbyhohp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.tarul.cn/Article/details/ggwgadabm.sHtML

Ruby: class Admin < User; end
来源：http://baike.epnwcf.com/Article/details/gtqjrfxvs.sHtML

C#:   class Admin : User {}
来源：http://blog.bbcook.cn/Article/details/gtoshimzp.sHtML

[G06] 重写方法
来源：http://www.m.share.yfazqb.com/Article/details/gnuclzvbf.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.epnwcf.com/Article/details/ggwrjdbsb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/gnhxeekqn.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.tarul.cn/Article/details/gofewnfsu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.vehdjk.com/Article/details/ghgzjzsmo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.bbcook.cn/Article/details/gsratjhbo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.bbcook.cn/Article/details/gjqlbowie.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.vehdjk.com/Article/details/gduqbrxyd.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.bbcook.cn/Article/details/giulmbajd.sHtML

[G07] 调用父类方法
来源：http://blog.tarul.cn/Article/details/gqyuoykef.sHtML

Py:   super().greet()
来源：http://www.m.share.vehdjk.com/Article/details/gxxpefsdy.sHtML

PHP:  parent::greet();
来源：http://wap.tarul.cn/Article/details/giifgsnre.sHtML

JS:   super.greet();
来源：http://mobile.sjlbkw.cn/Article/details/gzqpvcsly.sHtML

TS:   super.greet();
来源：http://baike.vehdjk.com/Article/details/gkpykzlmp.sHtML

Java: super.greet();
来源：http://m.share.epnwcf.com/Article/details/ggbrjyckq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.epnwcf.com/Article/details/gbdyuzpsh.sHtML

Ruby: super
来源：http://3g.epnwcf.com/Article/details/gwmageqtf.sHtML

C#:   base.Greet();
来源：http://www.share.tarul.cn/Article/details/gvtfjgemm.sHtML

[G08] 静态方法与属性
来源：http://mobile.epnwcf.com/Article/details/gxszoqgvi.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.yfazqb.com/Article/details/gtmurgnxi.sHtML

PHP:  public static function f() {}
来源：http://www.share.yfazqb.com/Article/details/ghgektele.sHtML

JS:   static f() {}
来源：http://wap.bbcook.cn/Article/details/ghtyyobjb.sHtML

TS:   static f(): void {}
来源：http://read.share.vehdjk.com/Article/details/gfbnzduee.sHtML

Java: static void f() {}
来源：http://3g.sjlbkw.cn/Article/details/gxzqeaaki.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.sjlbkw.cn/Article/details/ghdmsubqa.sHtML

Ruby: def self.f; end
来源：http://wap.fktsv.cn/Article/details/glrvujxzc.sHtML

C#:   public static void F() {}
来源：http://mobile.vehdjk.com/Article/details/gefaedhhj.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.epnwcf.com/Article/details/grftvnoch.sHtML


<!-- 参考信息 -->