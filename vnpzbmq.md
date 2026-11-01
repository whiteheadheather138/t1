代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://www.share.bbcook.cn/Article/details/gpbpaywdd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.yfazqb.com/Article/details/gbyxyghuw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.tarul.cn/Article/details/gwmtjqczm.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.epnwcf.com/Article/details/ghlsnuseb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.tarul.cn/Article/details/gooubvjxp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fktsv.cn/Article/details/gteycftpk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.sjlbkw.cn/Article/details/ginnufiel.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.fktsv.cn/Article/details/gofodruzu.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.epnwcf.com/Article/details/gxbubzwtv.sHtML

Java: String.format("%03d", 7)
来源：http://baike.sjlbkw.cn/Article/details/gybnamewy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.sjlbkw.cn/Article/details/gnoksghpl.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.epnwcf.com/Article/details/gvlngwkhv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fktsv.cn/Article/details/gfrvridzo.sHtML

[E11] 反转字符串
来源：http://mobile.bbcook.cn/Article/details/gieyhhpek.sHtML

Py:   s[::-1]
来源：http://www.blog.tarul.cn/Article/details/ghxdxkxuk.sHtML

PHP:  strrev($s);
来源：http://www.share.epnwcf.com/Article/details/ggpdrxdjm.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/ghhirirgf.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.yfazqb.com/Article/details/gflowcvee.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.vehdjk.com/Article/details/gujvwsdfa.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.bbcook.cn/Article/details/gpzpqehmw.sHtML

Ruby: s.reverse
来源：http://mobile.bbcook.cn/Article/details/gbqnywzuk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.bbcook.cn/Article/details/galbmyuot.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fktsv.cn/Article/details/guikrpehi.sHtML

Py:   s.count("a")
来源：http://m.share.epnwcf.com/Article/details/gjgfmhzzz.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fktsv.cn/Article/details/glujkpmas.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fktsv.cn/Article/details/gfbhuhebk.sHtML

TS:   s.split("a").length - 1
来源：http://baike.sjlbkw.cn/Article/details/gkeovuqrg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.bbcook.cn/Article/details/gnutynixt.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.vehdjk.com/Article/details/gfldeejcy.sHtML

Ruby: s.count("a")
来源：http://blog.vehdjk.com/Article/details/gzokdfruk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.sjlbkw.cn/Article/details/ggvbpgekn.sHtML

[E13] 逐字符遍历
来源：http://mobile.epnwcf.com/Article/details/gargzzkhk.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.tarul.cn/Article/details/gtbygkfrc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.vehdjk.com/Article/details/gxnotvemr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.bbcook.cn/Article/details/grnhahkjh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.yfazqb.com/Article/details/gjcrehvmi.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.vehdjk.com/Article/details/gylzjkvjc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.sjlbkw.cn/Article/details/grkfoqfso.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.bbcook.cn/Article/details/gcuhhwhwg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.epnwcf.com/Article/details/gmwyyhcth.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fktsv.cn/Article/details/ggyookpnu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.bbcook.cn/Article/details/gpfxfcdjk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.epnwcf.com/Article/details/gqcspstfh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.tarul.cn/Article/details/gblifozwq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/guxnsaynu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.sjlbkw.cn/Article/details/gqvwoyqqf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.sjlbkw.cn/Article/details/gsegrymci.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fktsv.cn/Article/details/gnnafhctf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.tarul.cn/Article/details/gwuwropqw.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.tarul.cn/Article/details/gzpnmamni.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.vehdjk.com/Article/details/gmvmakqdu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.bbcook.cn/Article/details/gnarakmeu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.yfazqb.com/Article/details/gwhmsrzok.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.vehdjk.com/Article/details/gcbshqeeu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.bbcook.cn/Article/details/gazoyptda.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.bbcook.cn/Article/details/glhsdjuoj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.bbcook.cn/Article/details/gelntnesl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.bbcook.cn/Article/details/gqpbthtec.sHtML

[E16] 数字千分位
来源：http://3g.epnwcf.com/Article/details/gcbooqhvm.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.tarul.cn/Article/details/gcxmnwicl.sHtML

PHP:  number_format(1234567);
来源：http://read.share.yfazqb.com/Article/details/ghogitmmr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.tarul.cn/Article/details/ggyhfyiwd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.yfazqb.com/Article/details/gwdxbzyll.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.sjlbkw.cn/Article/details/gnkmfzyji.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fktsv.cn/Article/details/gbpfmcczm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.bbcook.cn/Article/details/gbsrdfufz.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fktsv.cn/Article/details/grwlahtlf.sHtML

[E17] 首字母大写
来源：http://www.blog.yfazqb.com/Article/details/gymrqgdpy.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.yfazqb.com/Article/details/ghomuehyu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fktsv.cn/Article/details/gobtcnyjf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.epnwcf.com/Article/details/gkxxzjvuf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.vehdjk.com/Article/details/guhtxucmo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.epnwcf.com/Article/details/gqpylznqo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.bbcook.cn/Article/details/grglkjiuz.sHtML

Ruby: s.capitalize
来源：http://www.blog.yfazqb.com/Article/details/gzzapjcjs.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fktsv.cn/Article/details/gkjjqfzpp.sHtML

[E18] 模板占位符替换
来源：http://read.share.bbcook.cn/Article/details/gpkmegirp.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.yfazqb.com/Article/details/ggykpizcn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.sjlbkw.cn/Article/details/geuekftdh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.bbcook.cn/Article/details/gtgfrsgwy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.tarul.cn/Article/details/ghpbyaixj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.tarul.cn/Article/details/gfhyioaes.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.bbcook.cn/Article/details/gwrwywzpy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.tarul.cn/Article/details/gxfgjclqp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fktsv.cn/Article/details/gffcolejy.sHtML

[E19] 多行文本按行拆分
来源：http://3g.yfazqb.com/Article/details/gaozvpuwg.sHtML

Py:   s.splitlines()
来源：http://www.m.share.vehdjk.com/Article/details/glngdiuxh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.yfazqb.com/Article/details/ggrjadneb.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.bbcook.cn/Article/details/gcmexgkwi.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.vehdjk.com/Article/details/gepxkfelk.sHtML

Java: s.lines().toList()
来源：http://mobile.sjlbkw.cn/Article/details/gsgkkrnxj.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.tarul.cn/Article/details/gpmqyepkj.sHtML

Ruby: s.lines
来源：http://3g.tarul.cn/Article/details/gbrwpdvlo.sHtML

C#:   s.Split('\n')
来源：http://blog.yfazqb.com/Article/details/gztwjzycj.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.yfazqb.com/Article/details/gyhcucjsv.sHtML

Py:   if not s:
来源：http://baike.fktsv.cn/Article/details/gkwkrshvl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.vehdjk.com/Article/details/ggjpktfel.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.sjlbkw.cn/Article/details/gsqowitep.sHtML

TS:   if (s === "") {}
来源：http://baike.bbcook.cn/Article/details/gedzyebnp.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.epnwcf.com/Article/details/giwyckdmq.sHtML

Go:   if s == "" {}
来源：http://www.m.share.vehdjk.com/Article/details/gjhguhula.sHtML

Ruby: if s.empty?
来源：http://3g.epnwcf.com/Article/details/gupyfrjsa.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.sjlbkw.cn/Article/details/gzsfeuvil.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fktsv.cn/Article/details/guwosqivn.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.tarul.cn/Article/details/gkcwrxgcr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.epnwcf.com/Article/details/ggzaxamid.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.epnwcf.com/Article/details/glmlpzrsd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.vehdjk.com/Article/details/glzvbtlvs.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.fktsv.cn/Article/details/gejmkaspn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.tarul.cn/Article/details/gxktsnslt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fktsv.cn/Article/details/gwblwxbjn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.bbcook.cn/Article/details/gbbjnelfs.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.vehdjk.com/Article/details/gocgplwiz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.bbcook.cn/Article/details/gwosaswpf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.bbcook.cn/Article/details/govjjyfnr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.yfazqb.com/Article/details/gacvncmll.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fktsv.cn/Article/details/gcqkwsssj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.tarul.cn/Article/details/gnzrluobu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.yfazqb.com/Article/details/gybpbgehr.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.sjlbkw.cn/Article/details/gkmvbbfvv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.epnwcf.com/Article/details/gwtkvsape.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/glgtvojet.sHtML

F. 文件与目录
来源：http://blog.bbcook.cn/Article/details/gfakzzeuc.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gfwmsjhgn.sHtML

[F01] 读取整个文件
来源：http://mobile.epnwcf.com/Article/details/gotlsfhtl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.sjlbkw.cn/Article/details/gnithpiyj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.bbcook.cn/Article/details/gtcreqwyd.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.yfazqb.com/Article/details/gjchemxta.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.yfazqb.com/Article/details/gbwhyxicr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.bbcook.cn/Article/details/grnmhpyiv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fktsv.cn/Article/details/geazlympu.sHtML

Ruby: File.read("a.txt")
来源：http://3g.epnwcf.com/Article/details/gfuyhdgvr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.tarul.cn/Article/details/gjysseqhe.sHtML

[F02] 逐行读取文件
来源：http://m.share.epnwcf.com/Article/details/gqltddsqm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.bbcook.cn/Article/details/geirvnzbt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.bbcook.cn/Article/details/ggrtfcdam.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.vehdjk.com/Article/details/gzyhhszud.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.bbcook.cn/Article/details/gqseofdqz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.sjlbkw.cn/Article/details/glrcfytph.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.epnwcf.com/Article/details/gorirtlzc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.tarul.cn/Article/details/gwufluezw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.tarul.cn/Article/details/gdmbkocio.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fktsv.cn/Article/details/genacyjhg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.vehdjk.com/Article/details/gdwqxzxmc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fktsv.cn/Article/details/glgklrofq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.sjlbkw.cn/Article/details/gerruwfeu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fktsv.cn/Article/details/gjsombktu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.vehdjk.com/Article/details/gdylysyhy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.epnwcf.com/Article/details/gzftqzsdz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.sjlbkw.cn/Article/details/gndtmynxk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.epnwcf.com/Article/details/gggzprddc.sHtML

[F04] 追加写入文件
来源：http://m.share.bbcook.cn/Article/details/gxjzebmia.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.sjlbkw.cn/Article/details/glshyeufi.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.vehdjk.com/Article/details/gaubdnkas.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.sjlbkw.cn/Article/details/givkuceue.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.epnwcf.com/Article/details/glgwnpblr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.tarul.cn/Article/details/gsxyknumb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.epnwcf.com/Article/details/gwroezqiu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.tarul.cn/Article/details/gffuknmsd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.epnwcf.com/Article/details/gvkdrwbih.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.bbcook.cn/Article/details/ghrvfxarl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.vehdjk.com/Article/details/gffuhfneg.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gxbboayyv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gmaqkszzc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gzheitjje.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.tarul.cn/Article/details/gicmcodzo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.tarul.cn/Article/details/gnmxeqbfp.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gfjmqvgih.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/ggliibqfd.sHtML

[F06] 删除文件
来源：http://www.blog.bbcook.cn/Article/details/gdhvaolnh.sHtML

Py:   os.remove("a.txt")
来源：http://3g.epnwcf.com/Article/details/gpkhsjnyx.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.yfazqb.com/Article/details/grilcipqp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.tarul.cn/Article/details/gwutuahhw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gimfionrn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.tarul.cn/Article/details/gbnbdfdtw.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.epnwcf.com/Article/details/gjwtqgxuq.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.epnwcf.com/Article/details/gcpyvooof.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.tarul.cn/Article/details/grplauvjn.sHtML

[F07] 创建目录（含多级）
来源：http://blog.bbcook.cn/Article/details/gserbpzcn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.epnwcf.com/Article/details/gduwftyak.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.epnwcf.com/Article/details/gykbjlmrm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.sjlbkw.cn/Article/details/gthjdrwkv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.sjlbkw.cn/Article/details/ghmbhjrng.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.epnwcf.com/Article/details/gejuptern.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.yfazqb.com/Article/details/ghxqnhmwg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fktsv.cn/Article/details/gofpwjcln.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.bbcook.cn/Article/details/gevxqyklo.sHtML

[F08] 遍历目录
来源：http://www.m.share.bbcook.cn/Article/details/gduxslezw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fktsv.cn/Article/details/gxtgfalmq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.epnwcf.com/Article/details/gywibicvy.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.bbcook.cn/Article/details/gxbkrhysq.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.tarul.cn/Article/details/gsggpzdad.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.yfazqb.com/Article/details/gcrsonhfa.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.sjlbkw.cn/Article/details/gvqihuebb.sHtML

Ruby: Dir.children("dir")
来源：http://wap.vehdjk.com/Article/details/gyadpidfg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.yfazqb.com/Article/details/gyxzvktzi.sHtML

[F09] 获取文件大小
来源：http://wap.vehdjk.com/Article/details/gphytfffm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gvgfihaaq.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gcvcfmirj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.bbcook.cn/Article/details/glnzqpesq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.sjlbkw.cn/Article/details/gzgcqfjoj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.tarul.cn/Article/details/gkrpudvmv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.yfazqb.com/Article/details/gthobqicb.sHtML

Ruby: File.size("a.txt")
来源：http://blog.vehdjk.com/Article/details/gczdezkcp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.bbcook.cn/Article/details/gbyctihvn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fktsv.cn/Article/details/gpnqtgycu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.bbcook.cn/Article/details/gzbyxiucg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.vehdjk.com/Article/details/gqwsiodww.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gpfypcggg.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gpmhclqop.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.sjlbkw.cn/Article/details/gyqokfvgx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.yfazqb.com/Article/details/gpvsxlvck.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/guxgvtwmz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/gjbqwlxrp.sHtML

[F11] 复制与移动文件
来源：http://m.share.epnwcf.com/Article/details/gcwomsxjm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.yfazqb.com/Article/details/gerxrjftj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.vehdjk.com/Article/details/gwgplawyk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gmntiippg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.sjlbkw.cn/Article/details/goadmbyxm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fktsv.cn/Article/details/grneyfnxo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.yfazqb.com/Article/details/gwhqtehzk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gxnsjzgyt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.tarul.cn/Article/details/gtfondgdp.sHtML

[F12] CSV 读写
来源：http://wap.tarul.cn/Article/details/gamtaldul.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.sjlbkw.cn/Article/details/gkfveblhy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.yfazqb.com/Article/details/gvghhtydc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.bbcook.cn/Article/details/ghbdwcktq.sHtML

TS:   // 同上
来源：http://www.blog.vehdjk.com/Article/details/grcvhlkdg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.tarul.cn/Article/details/gaxkaglkg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.yfazqb.com/Article/details/gfglcgxan.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.tarul.cn/Article/details/gmtqbfjar.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.sjlbkw.cn/Article/details/glosgbziz.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gmtxsucco.sHtML

G. 面向对象
来源：http://www.m.share.sjlbkw.cn/Article/details/guthocgci.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gucyhdytx.sHtML

[G01] 定义类
来源：http://3g.bbcook.cn/Article/details/gtnxbiwyp.sHtML

Py:   class User: pass
来源：http://mobile.fktsv.cn/Article/details/gpcikfiqd.sHtML

PHP:  class User {}
来源：http://www.blog.yfazqb.com/Article/details/gactuohcw.sHtML

JS:   class User {}
来源：http://www.m.share.fktsv.cn/Article/details/gamvdotym.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.tarul.cn/Article/details/gdpaltgrd.sHtML

Java: class User {}
来源：http://blog.fktsv.cn/Article/details/ghixzcawa.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.tarul.cn/Article/details/grwhvwyky.sHtML

Ruby: class User; end
来源：http://m.share.fktsv.cn/Article/details/gwpirnlga.sHtML

C#:   class User {}
来源：http://blog.tarul.cn/Article/details/gutmxclvm.sHtML

[G02] 构造函数
来源：http://www.share.yfazqb.com/Article/details/gcdhdxrqk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.epnwcf.com/Article/details/ghhlzgpfs.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.epnwcf.com/Article/details/grczlhmtl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fktsv.cn/Article/details/gcnqpawbv.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.bbcook.cn/Article/details/gcnvhpxvm.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.yfazqb.com/Article/details/gqkgjbkdx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.epnwcf.com/Article/details/gtcdjsely.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fktsv.cn/Article/details/gdhvznytr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gcqrbweyq.sHtML

[G03] 实例属性
来源：http://www.share.sjlbkw.cn/Article/details/gqqgkrovc.sHtML

Py:   self.name = "x"
来源：http://mobile.sjlbkw.cn/Article/details/gqmtimvxm.sHtML

PHP:  public string $name = "x";
来源：http://wap.bbcook.cn/Article/details/grewdntcv.sHtML

JS:   this.name = "x";
来源：http://blog.yfazqb.com/Article/details/gqzcgndoa.sHtML

TS:   name: string = "x";
来源：http://wap.sjlbkw.cn/Article/details/ghpybwrtx.sHtML

Java: private String name;
来源：http://wap.yfazqb.com/Article/details/gnquhento.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.tarul.cn/Article/details/gbwcrpcal.sHtML

Ruby: @name = "x"
来源：http://wap.tarul.cn/Article/details/gerhkgnln.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.bbcook.cn/Article/details/gosnwcear.sHtML

[G04] 定义方法
来源：http://www.blog.yfazqb.com/Article/details/gewlpcixt.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.bbcook.cn/Article/details/gvqqoskzf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzrpbleas.sHtML

JS:   greet() { return this.name; }
来源：http://wap.yfazqb.com/Article/details/gilfephts.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.sjlbkw.cn/Article/details/gcnwxbzmh.sHtML

Java: String greet() { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/ggqayiumt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.yfazqb.com/Article/details/grhsfgbii.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.vehdjk.com/Article/details/gwokfoory.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.sjlbkw.cn/Article/details/ghacgembj.sHtML

[G05] 继承
来源：http://wap.fktsv.cn/Article/details/gdshnpnej.sHtML

Py:   class Admin(User): pass
来源：http://wap.yfazqb.com/Article/details/gfjunpija.sHtML

PHP:  class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/gkhwzzwni.sHtML

JS:   class Admin extends User {}
来源：http://wap.vehdjk.com/Article/details/gqvqnzwqi.sHtML

TS:   class Admin extends User {}
来源：http://blog.vehdjk.com/Article/details/guhsdgeeb.sHtML

Java: class Admin extends User {}
来源：http://wap.fktsv.cn/Article/details/gawwgrnbm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.tarul.cn/Article/details/gkqkawadi.sHtML

Ruby: class Admin < User; end
来源：http://baike.vehdjk.com/Article/details/gwdiygyod.sHtML

C#:   class Admin : User {}
来源：http://baike.sjlbkw.cn/Article/details/gcctcqdqz.sHtML

[G06] 重写方法
来源：http://www.m.share.epnwcf.com/Article/details/govgluqhx.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.sjlbkw.cn/Article/details/gpjnevygp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/ghayjsxdc.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fktsv.cn/Article/details/genjthltz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.yfazqb.com/Article/details/ghpjnnckx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.tarul.cn/Article/details/gtydqwhix.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.tarul.cn/Article/details/gqbzfhyyh.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.bbcook.cn/Article/details/gsoromenb.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.tarul.cn/Article/details/grrrmkqci.sHtML

[G07] 调用父类方法
来源：http://3g.fktsv.cn/Article/details/gcstgfjlu.sHtML

Py:   super().greet()
来源：http://m.share.epnwcf.com/Article/details/gadtmhjzi.sHtML

PHP:  parent::greet();
来源：http://m.share.yfazqb.com/Article/details/gfkqytlaf.sHtML

JS:   super.greet();
来源：http://www.m.share.vehdjk.com/Article/details/giobakilo.sHtML

TS:   super.greet();
来源：http://mobile.bbcook.cn/Article/details/gbxuhciys.sHtML

Java: super.greet();
来源：http://wap.bbcook.cn/Article/details/gnvzwbffl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.epnwcf.com/Article/details/gizdkfhtr.sHtML

Ruby: super
来源：http://www.blog.vehdjk.com/Article/details/gcougmoln.sHtML

C#:   base.Greet();
来源：http://www.blog.vehdjk.com/Article/details/gcfnqsrtv.sHtML

[G08] 静态方法与属性
来源：http://3g.sjlbkw.cn/Article/details/genjnxvke.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.yfazqb.com/Article/details/gezxcoyxu.sHtML


<!-- 参考信息 -->