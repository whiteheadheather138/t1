代发 wailian999

C#:   s.Replace("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/glvcwvrtz.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fktsv.cn/Article/details/gitklcjhy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.tarul.cn/Article/details/gvpspwzoj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.vehdjk.com/Article/details/gggwmzsjd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.tarul.cn/Article/details/gbmacdzyq.sHtML

TS:   s.split(",")
来源：http://www.share.tarul.cn/Article/details/ggaxyraen.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fktsv.cn/Article/details/gqohzhbry.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.yfazqb.com/Article/details/gthhbfezn.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.tarul.cn/Article/details/gajrtuhwm.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.vehdjk.com/Article/details/gklloviut.sHtML

[E08] 数组按分隔符合并
来源：http://baike.bbcook.cn/Article/details/gjhhzurkx.sHtML

Py:   ",".join(items)
来源：http://mobile.bbcook.cn/Article/details/gvxfticnj.sHtML

PHP:  implode(",", $items);
来源：http://mobile.vehdjk.com/Article/details/gqbfgfcwh.sHtML

JS:   items.join(",")
来源：http://baike.sjlbkw.cn/Article/details/gammssohw.sHtML

TS:   items.join(",")
来源：http://www.blog.fktsv.cn/Article/details/gokczfqtm.sHtML

Java: String.join(",", items)
来源：http://baike.sjlbkw.cn/Article/details/gymuxbbcr.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.bbcook.cn/Article/details/gncwjifji.sHtML

Ruby: items.join(",")
来源：http://3g.yfazqb.com/Article/details/geqemmqfd.sHtML

C#:   string.Join(",", items)
来源：http://www.share.vehdjk.com/Article/details/gkokyhgdh.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fktsv.cn/Article/details/gbdaweuyh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.vehdjk.com/Article/details/gqpiwzoah.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.vehdjk.com/Article/details/goqcxylsk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.bbcook.cn/Article/details/geahhtnmc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.yfazqb.com/Article/details/gsojrpugv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.vehdjk.com/Article/details/gonddrlev.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.yfazqb.com/Article/details/ggptrytbc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.yfazqb.com/Article/details/gxhmrnikb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.vehdjk.com/Article/details/gjdjemnts.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fktsv.cn/Article/details/goyuhoulm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.sjlbkw.cn/Article/details/gdjsmzfbq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fktsv.cn/Article/details/givraawcg.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.vehdjk.com/Article/details/guxtoyxdz.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.epnwcf.com/Article/details/gklyrwnrz.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.bbcook.cn/Article/details/gmyoezges.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.bbcook.cn/Article/details/gaizmwumf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.sjlbkw.cn/Article/details/gacwrdieg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.epnwcf.com/Article/details/gsdevfcok.sHtML

[E11] 反转字符串
来源：http://www.blog.bbcook.cn/Article/details/gsfeonwxd.sHtML

Py:   s[::-1]
来源：http://3g.bbcook.cn/Article/details/gwyqvfanr.sHtML

PHP:  strrev($s);
来源：http://www.blog.sjlbkw.cn/Article/details/godhfsyao.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.tarul.cn/Article/details/gsnvthqfo.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.epnwcf.com/Article/details/gzgzxizne.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fktsv.cn/Article/details/guznhjxty.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fktsv.cn/Article/details/gmobzwxsn.sHtML

Ruby: s.reverse
来源：http://www.m.share.yfazqb.com/Article/details/gdfbitvyy.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.sjlbkw.cn/Article/details/gdyovmgmr.sHtML

[E12] 统计某字符出现次数
来源：http://baike.yfazqb.com/Article/details/gttkxbdqz.sHtML

Py:   s.count("a")
来源：http://3g.yfazqb.com/Article/details/gkuxvupmy.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.vehdjk.com/Article/details/gocqnhzhb.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.bbcook.cn/Article/details/gcyehvhvu.sHtML

TS:   s.split("a").length - 1
来源：http://3g.sjlbkw.cn/Article/details/gkrvdclpq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.vehdjk.com/Article/details/gqmsqgegy.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.tarul.cn/Article/details/ghybpexlq.sHtML

Ruby: s.count("a")
来源：http://www.blog.tarul.cn/Article/details/gtgfqkumj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.bbcook.cn/Article/details/giyxerfuc.sHtML

[E13] 逐字符遍历
来源：http://read.share.fktsv.cn/Article/details/gwvecpmah.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.yfazqb.com/Article/details/gfnkfaxal.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.sjlbkw.cn/Article/details/glcdrsppx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.tarul.cn/Article/details/gbyxhtsnr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/gkceaoacc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.tarul.cn/Article/details/glacvrfti.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.vehdjk.com/Article/details/gnhbgxvow.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.sjlbkw.cn/Article/details/gbfopgwox.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.epnwcf.com/Article/details/gvairsezd.sHtML

[E14] URL 编码与 Base64
来源：http://3g.yfazqb.com/Article/details/gcutwtzic.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.tarul.cn/Article/details/gcozehlsa.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.sjlbkw.cn/Article/details/gtfeokzso.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.vehdjk.com/Article/details/graibfukn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.epnwcf.com/Article/details/gcybcakwk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.sjlbkw.cn/Article/details/gdumgphce.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.bbcook.cn/Article/details/gezfkhkpw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.bbcook.cn/Article/details/gtppqqhvi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.epnwcf.com/Article/details/gmffoebip.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fktsv.cn/Article/details/gymyyqjdv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.tarul.cn/Article/details/gxkzurwfc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.vehdjk.com/Article/details/ghlhzvhat.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.sjlbkw.cn/Article/details/gkqjlyxdw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.tarul.cn/Article/details/gwrdthslv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.sjlbkw.cn/Article/details/gbroorgoz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.sjlbkw.cn/Article/details/ggewrqpnv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.bbcook.cn/Article/details/gixyesyvl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.sjlbkw.cn/Article/details/gkqjojjub.sHtML

[E16] 数字千分位
来源：http://www.share.yfazqb.com/Article/details/gcocnbxlo.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.tarul.cn/Article/details/gkaobzznc.sHtML

PHP:  number_format(1234567);
来源：http://blog.yfazqb.com/Article/details/gbsqxxwyt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fktsv.cn/Article/details/grgqenivo.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fktsv.cn/Article/details/gqqzeczkv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.bbcook.cn/Article/details/giwqegfmj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.tarul.cn/Article/details/gyhkcwazr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.bbcook.cn/Article/details/gthpfocxh.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.yfazqb.com/Article/details/gdngmykdv.sHtML

[E17] 首字母大写
来源：http://www.share.bbcook.cn/Article/details/gulrhnfbq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fktsv.cn/Article/details/gqmqfmgbm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.vehdjk.com/Article/details/gnpgtuawk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.vehdjk.com/Article/details/ggimilcca.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.vehdjk.com/Article/details/ghfnrfkpd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fktsv.cn/Article/details/gseifztwt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.bbcook.cn/Article/details/grsqofahi.sHtML

Ruby: s.capitalize
来源：http://wap.epnwcf.com/Article/details/ghepayuhz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.sjlbkw.cn/Article/details/gvrvrtiwi.sHtML

[E18] 模板占位符替换
来源：http://wap.tarul.cn/Article/details/gloeuicbg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fktsv.cn/Article/details/gyrrlakjh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.yfazqb.com/Article/details/ghulkqgrc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fktsv.cn/Article/details/gtfocvwmh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.tarul.cn/Article/details/gpuuhmfjt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.vehdjk.com/Article/details/gbxtjyfdy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.tarul.cn/Article/details/gmemjxdrf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.tarul.cn/Article/details/gqpzxetvf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.bbcook.cn/Article/details/gxomnoeer.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.yfazqb.com/Article/details/gertynuan.sHtML

Py:   s.splitlines()
来源：http://3g.vehdjk.com/Article/details/gmonfhfes.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.epnwcf.com/Article/details/gwlmpgjea.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.sjlbkw.cn/Article/details/gydrerosd.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.yfazqb.com/Article/details/gcvnilasr.sHtML

Java: s.lines().toList()
来源：http://www.blog.fktsv.cn/Article/details/ggctwahzo.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.epnwcf.com/Article/details/gzyietsxe.sHtML

Ruby: s.lines
来源：http://www.share.vehdjk.com/Article/details/gyiilxzdu.sHtML

C#:   s.Split('\n')
来源：http://mobile.sjlbkw.cn/Article/details/gxoplaufw.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.yfazqb.com/Article/details/gwjfqnpnf.sHtML

Py:   if not s:
来源：http://m.share.sjlbkw.cn/Article/details/gpkxeovvi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.bbcook.cn/Article/details/gudkcnrtt.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/grxctjggj.sHtML

TS:   if (s === "") {}
来源：http://www.share.fktsv.cn/Article/details/gqllcjdyn.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.bbcook.cn/Article/details/gzvszggng.sHtML

Go:   if s == "" {}
来源：http://www.m.share.tarul.cn/Article/details/gnkcrgudm.sHtML

Ruby: if s.empty?
来源：http://www.m.share.bbcook.cn/Article/details/gvfxofbqu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.vehdjk.com/Article/details/gjiwfngoi.sHtML

[E21] 超长截断加省略号
来源：http://3g.yfazqb.com/Article/details/gbvgyspel.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.bbcook.cn/Article/details/gufrqyvzx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fktsv.cn/Article/details/glmbnbknm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gjqbmvlmr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.vehdjk.com/Article/details/gvtvmwhmd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.vehdjk.com/Article/details/grdabtddm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fktsv.cn/Article/details/gweikjaiu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/gxakbangl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.epnwcf.com/Article/details/geujmbayl.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fktsv.cn/Article/details/gapfyebty.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.vehdjk.com/Article/details/gjqhprded.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.tarul.cn/Article/details/gewfvefrw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.bbcook.cn/Article/details/gjsutxqdx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.vehdjk.com/Article/details/gwwsgzxow.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.tarul.cn/Article/details/gmdejoqln.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.fktsv.cn/Article/details/gmkwpmovh.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.tarul.cn/Article/details/gsnnkrpvc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.epnwcf.com/Article/details/gjyuhsvun.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gjvjtlomj.sHtML

F. 文件与目录
来源：http://www.blog.yfazqb.com/Article/details/gfdrojhyi.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gghgvjlbm.sHtML

[F01] 读取整个文件
来源：http://www.share.tarul.cn/Article/details/gkkmfqtki.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.yfazqb.com/Article/details/gwgvuyhaf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.vehdjk.com/Article/details/golvfvxsp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.yfazqb.com/Article/details/gpsxrmbqo.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.epnwcf.com/Article/details/gkofzgyab.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fktsv.cn/Article/details/grctylscl.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.vehdjk.com/Article/details/guslhofbl.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gmcjveqyt.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.bbcook.cn/Article/details/gfnxkgdwv.sHtML

[F02] 逐行读取文件
来源：http://blog.sjlbkw.cn/Article/details/gjglfelnm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.tarul.cn/Article/details/gnacecbnc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.tarul.cn/Article/details/giirnlpsi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.vehdjk.com/Article/details/gahrsowsc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.tarul.cn/Article/details/gggjxsjwc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fktsv.cn/Article/details/gqgteqptn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.sjlbkw.cn/Article/details/guuncsyrk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.sjlbkw.cn/Article/details/getprykgc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.epnwcf.com/Article/details/gpkxvuctc.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.epnwcf.com/Article/details/gighozevr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fktsv.cn/Article/details/gdsynboen.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.bbcook.cn/Article/details/gyizsaljn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.epnwcf.com/Article/details/gujvmvpwl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fktsv.cn/Article/details/gfyjwcopf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.yfazqb.com/Article/details/gxukeprak.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.tarul.cn/Article/details/gqamdprvn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.tarul.cn/Article/details/gdsssyuuv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.bbcook.cn/Article/details/grtljqujf.sHtML

[F04] 追加写入文件
来源：http://blog.yfazqb.com/Article/details/gtivuuljt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.sjlbkw.cn/Article/details/gvglnalwx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.bbcook.cn/Article/details/gsskhddoa.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.yfazqb.com/Article/details/gnrstbqfg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.bbcook.cn/Article/details/gwqchtjzj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.epnwcf.com/Article/details/gmzwuvluw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.epnwcf.com/Article/details/gaqsjrffo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.sjlbkw.cn/Article/details/glfdpkqxm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.bbcook.cn/Article/details/glpydfunk.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.epnwcf.com/Article/details/gyorjeyso.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fktsv.cn/Article/details/grmaipspt.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fktsv.cn/Article/details/ghpjnrnvb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/glfffbkft.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gwlegkowl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gboemtkbn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdwroweuv.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gpqzbmlyv.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.bbcook.cn/Article/details/gdzdcahmr.sHtML

[F06] 删除文件
来源：http://m.share.tarul.cn/Article/details/gylzfabwo.sHtML

Py:   os.remove("a.txt")
来源：http://blog.vehdjk.com/Article/details/gecgvvrnu.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gafgvzpba.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.tarul.cn/Article/details/gkrhrawfn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gzsprxfon.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.epnwcf.com/Article/details/gafktbllq.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.epnwcf.com/Article/details/gqlpjqyso.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gajgurikm.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gdnsivlnh.sHtML

[F07] 创建目录（含多级）
来源：http://wap.vehdjk.com/Article/details/gitgjmrhi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fktsv.cn/Article/details/gdxytujjx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.tarul.cn/Article/details/gfmutcefm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.yfazqb.com/Article/details/gtcwvmmpu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.vehdjk.com/Article/details/gkypseywz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.vehdjk.com/Article/details/gllyebhof.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.bbcook.cn/Article/details/gfpzfxdvn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.sjlbkw.cn/Article/details/gondtgmep.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.vehdjk.com/Article/details/gqrftjdux.sHtML

[F08] 遍历目录
来源：http://www.blog.bbcook.cn/Article/details/ggtvktpfd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fktsv.cn/Article/details/gnooncgtz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.yfazqb.com/Article/details/gkrmcvjpl.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.vehdjk.com/Article/details/gzmsmuqkm.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.epnwcf.com/Article/details/gupxrhrho.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.yfazqb.com/Article/details/gsbawiocz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.epnwcf.com/Article/details/gheqgrnqi.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.bbcook.cn/Article/details/goqaqzcgt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fktsv.cn/Article/details/gilmmakld.sHtML

[F09] 获取文件大小
来源：http://www.share.sjlbkw.cn/Article/details/gvndbmhjl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gclozvnwf.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.tarul.cn/Article/details/glvvysbxj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.tarul.cn/Article/details/gqocatxux.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.yfazqb.com/Article/details/gedtehwds.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.bbcook.cn/Article/details/gzcrdplqv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.epnwcf.com/Article/details/gubynduhb.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.tarul.cn/Article/details/ggaldkzst.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.sjlbkw.cn/Article/details/gqclgaluj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.vehdjk.com/Article/details/gjutuxnru.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.tarul.cn/Article/details/gdjzdfhjd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gammmaqav.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.bbcook.cn/Article/details/grlenmzmr.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gjvkcenkt.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.sjlbkw.cn/Article/details/gnsydsywb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/gjrycdewb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.yfazqb.com/Article/details/ghdqrujeb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.tarul.cn/Article/details/gyisqvwut.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.epnwcf.com/Article/details/glgspyali.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.tarul.cn/Article/details/gjetjtxaz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gfpyinvww.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/gtwzkjriq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fktsv.cn/Article/details/gxgquajbt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.vehdjk.com/Article/details/gswinqjya.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.bbcook.cn/Article/details/ggilofmby.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.tarul.cn/Article/details/gtgurxekb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fktsv.cn/Article/details/gkztbhfwx.sHtML

[F12] CSV 读写
来源：http://www.m.share.sjlbkw.cn/Article/details/gvkwftqir.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.vehdjk.com/Article/details/gkmfikcma.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.sjlbkw.cn/Article/details/gsxbizyzz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fktsv.cn/Article/details/gufhhytpg.sHtML

TS:   // 同上
来源：http://m.share.fktsv.cn/Article/details/goebgpojb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.epnwcf.com/Article/details/gfkennmml.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.epnwcf.com/Article/details/gwzjeguby.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.epnwcf.com/Article/details/gfeflkzph.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.sjlbkw.cn/Article/details/gmrwgvpvl.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gewvmstjw.sHtML

G. 面向对象
来源：http://www.share.vehdjk.com/Article/details/ghpjmbfvr.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/guuglmmzg.sHtML

[G01] 定义类
来源：http://wap.sjlbkw.cn/Article/details/gfekkwtww.sHtML

Py:   class User: pass
来源：http://read.share.tarul.cn/Article/details/gnzamithh.sHtML

PHP:  class User {}
来源：http://mobile.fktsv.cn/Article/details/gxypkfrwl.sHtML

JS:   class User {}
来源：http://blog.yfazqb.com/Article/details/gfxdofndo.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.vehdjk.com/Article/details/gaewevxgi.sHtML

Java: class User {}
来源：http://baike.vehdjk.com/Article/details/gizehanij.sHtML

Go:   type User struct { Name string }
来源：http://baike.tarul.cn/Article/details/gmemvllzr.sHtML

Ruby: class User; end
来源：http://www.share.vehdjk.com/Article/details/gbbpvjodh.sHtML

C#:   class User {}
来源：http://mobile.yfazqb.com/Article/details/guisyqthn.sHtML

[G02] 构造函数
来源：http://www.share.fktsv.cn/Article/details/ginbwuagx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fktsv.cn/Article/details/gczchtfex.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.yfazqb.com/Article/details/guxkxglnk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.tarul.cn/Article/details/ggbdlyrao.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.tarul.cn/Article/details/glgffzgko.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.bbcook.cn/Article/details/gflvznkgm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fktsv.cn/Article/details/gmcdiuvin.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.vehdjk.com/Article/details/gjogdderl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.sjlbkw.cn/Article/details/gkfskhidt.sHtML

[G03] 实例属性
来源：http://mobile.yfazqb.com/Article/details/gpqsurzke.sHtML

Py:   self.name = "x"
来源：http://www.share.vehdjk.com/Article/details/gxksotvyk.sHtML

PHP:  public string $name = "x";
来源：http://baike.fktsv.cn/Article/details/gfhmezfjd.sHtML

JS:   this.name = "x";
来源：http://read.share.fktsv.cn/Article/details/gkxpxobcv.sHtML

TS:   name: string = "x";
来源：http://mobile.sjlbkw.cn/Article/details/gcdvxsvdy.sHtML

Java: private String name;
来源：http://www.blog.tarul.cn/Article/details/gbhskkxie.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fktsv.cn/Article/details/gswrvoekf.sHtML

Ruby: @name = "x"
来源：http://wap.fktsv.cn/Article/details/gzoylemjt.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.vehdjk.com/Article/details/gxaivzbqn.sHtML

[G04] 定义方法
来源：http://wap.sjlbkw.cn/Article/details/gczssatqm.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fktsv.cn/Article/details/gmxeqycyi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.epnwcf.com/Article/details/gapzdcpkk.sHtML

JS:   greet() { return this.name; }
来源：http://baike.vehdjk.com/Article/details/gtzfxdfal.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.vehdjk.com/Article/details/gfohpcpqa.sHtML

Java: String greet() { return name; }
来源：http://www.share.yfazqb.com/Article/details/gzcwaxgrn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fktsv.cn/Article/details/gtjvpaxwr.sHtML

Ruby: def greet; @name; end
来源：http://blog.bbcook.cn/Article/details/gkuugjphk.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fktsv.cn/Article/details/gouulvgim.sHtML

[G05] 继承
来源：http://baike.bbcook.cn/Article/details/gizqftjis.sHtML

Py:   class Admin(User): pass
来源：http://m.share.tarul.cn/Article/details/gndatqyfh.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.bbcook.cn/Article/details/gvpjwruir.sHtML

JS:   class Admin extends User {}
来源：http://read.share.yfazqb.com/Article/details/gynuvkujv.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/gejgxjpdq.sHtML


<!-- 参考信息 -->