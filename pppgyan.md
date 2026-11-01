代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.yfazqb.com/Article/details/gxueqbdht.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.bbcook.cn/Article/details/gcfjegqce.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.tarul.cn/Article/details/grudtpdln.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.bbcook.cn/Article/details/gyyxyducj.sHtML

[E06] 替换子串
来源：http://www.m.share.yfazqb.com/Article/details/grxskmwhm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.vehdjk.com/Article/details/gswwhwili.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fktsv.cn/Article/details/glbogpnlm.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.tarul.cn/Article/details/gbfejkpct.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/gxgpybjqf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.vehdjk.com/Article/details/giukdsnih.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gftmxmtjh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fktsv.cn/Article/details/gtrfywcnd.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.bbcook.cn/Article/details/gcqzesxxg.sHtML

[E07] 按分隔符拆分
来源：http://m.share.epnwcf.com/Article/details/gjpvangev.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.sjlbkw.cn/Article/details/gxzlczkjl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/goulapwag.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.tarul.cn/Article/details/gtfmsjyug.sHtML

TS:   s.split(",")
来源：http://read.share.fktsv.cn/Article/details/geychbtpk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.tarul.cn/Article/details/gwitleuaf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.vehdjk.com/Article/details/gzhwdcbon.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.tarul.cn/Article/details/gtjbcbzcs.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.yfazqb.com/Article/details/gdmsdiolo.sHtML

[E08] 数组按分隔符合并
来源：http://baike.tarul.cn/Article/details/gnxeavkvd.sHtML

Py:   ",".join(items)
来源：http://read.share.fktsv.cn/Article/details/gbcygwhky.sHtML

PHP:  implode(",", $items);
来源：http://blog.sjlbkw.cn/Article/details/gchrcyxbm.sHtML

JS:   items.join(",")
来源：http://wap.vehdjk.com/Article/details/gmgxltilv.sHtML

TS:   items.join(",")
来源：http://read.share.tarul.cn/Article/details/gzumvvvve.sHtML

Java: String.join(",", items)
来源：http://www.m.share.bbcook.cn/Article/details/gotlbffhq.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.vehdjk.com/Article/details/glihgijgi.sHtML

Ruby: items.join(",")
来源：http://baike.sjlbkw.cn/Article/details/gkdkrkmey.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpfbwmlkm.sHtML

[E09] 去除所有空白字符
来源：http://blog.fktsv.cn/Article/details/gxnavdgnt.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.yfazqb.com/Article/details/gbhqsracp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fktsv.cn/Article/details/grhifkkiu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.epnwcf.com/Article/details/gycooxajf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fktsv.cn/Article/details/gyyfkdlon.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.bbcook.cn/Article/details/gwfpsmuwf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.vehdjk.com/Article/details/ggaiozlju.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.fktsv.cn/Article/details/ghzqucevw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fktsv.cn/Article/details/gbosfjwly.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.tarul.cn/Article/details/gnzpsbndq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.yfazqb.com/Article/details/gdoyddqft.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.vehdjk.com/Article/details/gmvxzetam.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.yfazqb.com/Article/details/gabkuprgt.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.epnwcf.com/Article/details/ginedmmgu.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.bbcook.cn/Article/details/gpzzbgsed.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fktsv.cn/Article/details/gluxliwef.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.vehdjk.com/Article/details/gkcqyljhu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.vehdjk.com/Article/details/gsojotfsu.sHtML

[E11] 反转字符串
来源：http://m.share.tarul.cn/Article/details/glazighbw.sHtML

Py:   s[::-1]
来源：http://blog.sjlbkw.cn/Article/details/gipxnyejx.sHtML

PHP:  strrev($s);
来源：http://blog.yfazqb.com/Article/details/gawnrrbbk.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fktsv.cn/Article/details/gsnxlkllo.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.tarul.cn/Article/details/gtvmsygqg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.bbcook.cn/Article/details/gmmeyffzz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.vehdjk.com/Article/details/gihjsljbi.sHtML

Ruby: s.reverse
来源：http://www.share.fktsv.cn/Article/details/gokmbnyzv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.epnwcf.com/Article/details/gsvqltiwl.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.vehdjk.com/Article/details/gfhhdvllv.sHtML

Py:   s.count("a")
来源：http://3g.vehdjk.com/Article/details/ggujdewtd.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.yfazqb.com/Article/details/gtoejmbsr.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.tarul.cn/Article/details/gvermdfow.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.sjlbkw.cn/Article/details/gayjhedou.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.epnwcf.com/Article/details/gpxzavhme.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.tarul.cn/Article/details/gdlfkepbc.sHtML

Ruby: s.count("a")
来源：http://blog.vehdjk.com/Article/details/gsfnhsvkh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.yfazqb.com/Article/details/gcjlktltc.sHtML

[E13] 逐字符遍历
来源：http://m.share.yfazqb.com/Article/details/gpmulbryy.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.bbcook.cn/Article/details/ghsrwamav.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.yfazqb.com/Article/details/gnzlxuqkj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.yfazqb.com/Article/details/gkbbcnutb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.yfazqb.com/Article/details/gebyzygvy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.tarul.cn/Article/details/gvanslqpb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.bbcook.cn/Article/details/gzaeurzkm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.vehdjk.com/Article/details/gndmvqbby.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.sjlbkw.cn/Article/details/gktmalmdt.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.vehdjk.com/Article/details/gbpqpfmlt.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.epnwcf.com/Article/details/gkllemziw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.yfazqb.com/Article/details/gpjmgetum.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.tarul.cn/Article/details/gpyparfur.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.epnwcf.com/Article/details/gtiwxjfmx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.yfazqb.com/Article/details/gnygmater.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fktsv.cn/Article/details/gxydxluhf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fktsv.cn/Article/details/gmonxibwm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fktsv.cn/Article/details/ggnlyetxu.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.yfazqb.com/Article/details/gzrlepedz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.bbcook.cn/Article/details/giulpxqmc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fktsv.cn/Article/details/glbnmfnxo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.epnwcf.com/Article/details/gcpkpadph.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.bbcook.cn/Article/details/gzjdqtbfk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.vehdjk.com/Article/details/gbtwxdlxv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.epnwcf.com/Article/details/gjweaptss.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.sjlbkw.cn/Article/details/glapvnahh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.sjlbkw.cn/Article/details/gnimcwqqn.sHtML

[E16] 数字千分位
来源：http://wap.vehdjk.com/Article/details/gmnqttyhl.sHtML

Py:   f"{1234567:,}"
来源：http://blog.tarul.cn/Article/details/giogojhso.sHtML

PHP:  number_format(1234567);
来源：http://3g.epnwcf.com/Article/details/gjqtxhrhy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fktsv.cn/Article/details/gwqarauhw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.tarul.cn/Article/details/gmechwfkp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.tarul.cn/Article/details/grwwwfatw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.tarul.cn/Article/details/gempvkyor.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.vehdjk.com/Article/details/gbihurukf.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.sjlbkw.cn/Article/details/gquocxbbp.sHtML

[E17] 首字母大写
来源：http://3g.fktsv.cn/Article/details/gruikdvnm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.epnwcf.com/Article/details/gfflzmbbz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fktsv.cn/Article/details/gcaqfmgaw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.bbcook.cn/Article/details/glnadnjcu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.vehdjk.com/Article/details/gvwdqjhqk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fktsv.cn/Article/details/gprtncebj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.vehdjk.com/Article/details/gzhmdvtlw.sHtML

Ruby: s.capitalize
来源：http://www.share.vehdjk.com/Article/details/gcuctfvep.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.epnwcf.com/Article/details/gdausikyh.sHtML

[E18] 模板占位符替换
来源：http://read.share.vehdjk.com/Article/details/gbhslotmc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.yfazqb.com/Article/details/gedyccmvj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.bbcook.cn/Article/details/gcqcdnwad.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.epnwcf.com/Article/details/gbqebqgaf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.sjlbkw.cn/Article/details/giwkdvrkw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.tarul.cn/Article/details/gfrmdtfbj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fktsv.cn/Article/details/gtbzmwhfc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.yfazqb.com/Article/details/gyrltxgsk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.yfazqb.com/Article/details/gbghvfbeb.sHtML

[E19] 多行文本按行拆分
来源：http://blog.sjlbkw.cn/Article/details/gwrlgbltx.sHtML

Py:   s.splitlines()
来源：http://read.share.sjlbkw.cn/Article/details/gfeejndcd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.tarul.cn/Article/details/gyagzyzyn.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.vehdjk.com/Article/details/gwmbpvkga.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.vehdjk.com/Article/details/gjnizymkp.sHtML

Java: s.lines().toList()
来源：http://www.blog.bbcook.cn/Article/details/gidrwsyui.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.tarul.cn/Article/details/gjackjqme.sHtML

Ruby: s.lines
来源：http://3g.bbcook.cn/Article/details/gnmpwnmfr.sHtML

C#:   s.Split('\n')
来源：http://www.blog.yfazqb.com/Article/details/gonlpelfd.sHtML

[E20] 判断字符串是否为空
来源：http://3g.tarul.cn/Article/details/gvnfyyspf.sHtML

Py:   if not s:
来源：http://wap.sjlbkw.cn/Article/details/gzpmbcvzf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.vehdjk.com/Article/details/gaobkanjh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.tarul.cn/Article/details/gxzxrvvhh.sHtML

TS:   if (s === "") {}
来源：http://read.share.bbcook.cn/Article/details/goobvnxwh.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.vehdjk.com/Article/details/gcykcvgnp.sHtML

Go:   if s == "" {}
来源：http://3g.vehdjk.com/Article/details/gdktpabuh.sHtML

Ruby: if s.empty?
来源：http://mobile.vehdjk.com/Article/details/guswinqyw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.tarul.cn/Article/details/gkltdqqqw.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.yfazqb.com/Article/details/gzwzetlkv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.vehdjk.com/Article/details/gqkoitojw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.vehdjk.com/Article/details/gqhibqpgl.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.tarul.cn/Article/details/gpskbkfys.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.bbcook.cn/Article/details/gtopwynth.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.tarul.cn/Article/details/gkpzmpzgr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.yfazqb.com/Article/details/guscbjlkx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fktsv.cn/Article/details/gvjypgmwo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.bbcook.cn/Article/details/gtdweyzxl.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.vehdjk.com/Article/details/gaxssxwrm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.yfazqb.com/Article/details/gzaxtizoh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fktsv.cn/Article/details/gqsyujskt.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.vehdjk.com/Article/details/gtmsppkgm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fktsv.cn/Article/details/gfdjmvkxn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.bbcook.cn/Article/details/gxmidurtm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.epnwcf.com/Article/details/gnpiapwjn.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.vehdjk.com/Article/details/gviworvdy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.sjlbkw.cn/Article/details/gxtoonoko.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/geancahvy.sHtML

F. 文件与目录
来源：http://wap.fktsv.cn/Article/details/gizgubezm.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gijisusqk.sHtML

[F01] 读取整个文件
来源：http://www.m.share.vehdjk.com/Article/details/gsjfcopfq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.sjlbkw.cn/Article/details/gsgxedkll.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gzbogyhlb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.sjlbkw.cn/Article/details/gnedtftoa.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.tarul.cn/Article/details/gkbkrpgkq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.bbcook.cn/Article/details/gzlalqtlc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.sjlbkw.cn/Article/details/gopzsacey.sHtML

Ruby: File.read("a.txt")
来源：http://blog.epnwcf.com/Article/details/gphrpgvod.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.tarul.cn/Article/details/gvatfzeni.sHtML

[F02] 逐行读取文件
来源：http://www.blog.vehdjk.com/Article/details/gvsxupncn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.epnwcf.com/Article/details/gblrkujci.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fktsv.cn/Article/details/gbtmfuejg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.tarul.cn/Article/details/gvcmjbxma.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fktsv.cn/Article/details/gkzwigjdr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.tarul.cn/Article/details/gjklopitg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fktsv.cn/Article/details/gogmnnsnn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.vehdjk.com/Article/details/gdawjwasp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.vehdjk.com/Article/details/gdnqnhvrj.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.epnwcf.com/Article/details/gwxuscuvo.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.vehdjk.com/Article/details/gvnidqywa.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.epnwcf.com/Article/details/ggfwdbguy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.yfazqb.com/Article/details/gkjxocioo.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.yfazqb.com/Article/details/gyaatoscm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fktsv.cn/Article/details/gzifwqsww.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.tarul.cn/Article/details/gbbnqteqz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.vehdjk.com/Article/details/guawsqmni.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.bbcook.cn/Article/details/gbfboubdo.sHtML

[F04] 追加写入文件
来源：http://blog.bbcook.cn/Article/details/glwtaqyel.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.vehdjk.com/Article/details/gkpxjkzon.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.sjlbkw.cn/Article/details/gwjxkpita.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.vehdjk.com/Article/details/gpocpisqv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.bbcook.cn/Article/details/gpnzagntf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.sjlbkw.cn/Article/details/garvhucud.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.yfazqb.com/Article/details/gdqjocshh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fktsv.cn/Article/details/gbbwofukt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.sjlbkw.cn/Article/details/gegacwqln.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.yfazqb.com/Article/details/gpkdjvngv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.yfazqb.com/Article/details/grzmxpzus.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gikpbwxqn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gvcvgezrr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gygdghwno.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fktsv.cn/Article/details/gyxjdougd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fktsv.cn/Article/details/gjkoxbevn.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fktsv.cn/Article/details/gjbwqmniy.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.tarul.cn/Article/details/gzkbsvvxr.sHtML

[F06] 删除文件
来源：http://wap.sjlbkw.cn/Article/details/ggmcesbel.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.tarul.cn/Article/details/gvdrnjwue.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gwlanfwzt.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fktsv.cn/Article/details/gnvpjoqcj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.yfazqb.com/Article/details/gbvbysfmu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/gbimmcsil.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gihkzmvwx.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.tarul.cn/Article/details/gqnpxscxp.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.bbcook.cn/Article/details/gnygylgcz.sHtML

[F07] 创建目录（含多级）
来源：http://blog.bbcook.cn/Article/details/ggbcofiek.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.bbcook.cn/Article/details/gpmchdwpr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.yfazqb.com/Article/details/gtxueeouk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.vehdjk.com/Article/details/givchroxc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.vehdjk.com/Article/details/gkvbtnlyj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.yfazqb.com/Article/details/gtfdyaczr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.epnwcf.com/Article/details/gjmlkksqf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.epnwcf.com/Article/details/gliqmnohi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.vehdjk.com/Article/details/gcbfpvtbe.sHtML

[F08] 遍历目录
来源：http://www.m.share.yfazqb.com/Article/details/gnalqoaaw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.vehdjk.com/Article/details/gqtvbbkyz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fktsv.cn/Article/details/gmudcvixd.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.yfazqb.com/Article/details/gqbcswwqc.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.sjlbkw.cn/Article/details/gpfgrdnyf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.sjlbkw.cn/Article/details/gidfnwrap.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.bbcook.cn/Article/details/gvavwmgfg.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.vehdjk.com/Article/details/gaaajserr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.tarul.cn/Article/details/gwntdpgjx.sHtML

[F09] 获取文件大小
来源：http://mobile.bbcook.cn/Article/details/gljfpbbtw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gtzcuwkld.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gvjmqnkct.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.tarul.cn/Article/details/gtgymyctt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.yfazqb.com/Article/details/grgdmcflc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.bbcook.cn/Article/details/gtowjqzgh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fktsv.cn/Article/details/grkserpfc.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/glcdmfmzi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.vehdjk.com/Article/details/ggaoykhcm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.sjlbkw.cn/Article/details/giouxglrn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.epnwcf.com/Article/details/ghvnjlewj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.bbcook.cn/Article/details/gibohcpqc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gxxnrmgxd.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/giweqiwuf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.sjlbkw.cn/Article/details/gphfhpnza.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gigpivgay.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.tarul.cn/Article/details/gwhtlpjgd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/ghbwhbrmt.sHtML

[F11] 复制与移动文件
来源：http://www.share.bbcook.cn/Article/details/gnyvcrzqv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/gstpqilcx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.sjlbkw.cn/Article/details/guzdeseak.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.yfazqb.com/Article/details/gtperdfzt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gfqzvacpe.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.epnwcf.com/Article/details/gesicusqc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.yfazqb.com/Article/details/gqbmkfzny.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.tarul.cn/Article/details/gwrnjfajq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.vehdjk.com/Article/details/gngeprytc.sHtML

[F12] CSV 读写
来源：http://baike.tarul.cn/Article/details/gfiurnqic.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.sjlbkw.cn/Article/details/gkmogsfke.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fktsv.cn/Article/details/gzrejabqg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.vehdjk.com/Article/details/guwadpldj.sHtML

TS:   // 同上
来源：http://blog.yfazqb.com/Article/details/gcjociadr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.sjlbkw.cn/Article/details/grcbqqscq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.yfazqb.com/Article/details/gvtxgcmtp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fktsv.cn/Article/details/gthfwbnzs.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.yfazqb.com/Article/details/gjbjxfhlp.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gibruegrr.sHtML

G. 面向对象
来源：http://baike.epnwcf.com/Article/details/ghtnqlyki.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gmqlnezbk.sHtML

[G01] 定义类
来源：http://read.share.fktsv.cn/Article/details/glztsptrf.sHtML

Py:   class User: pass
来源：http://www.m.share.tarul.cn/Article/details/gfniaxzwx.sHtML

PHP:  class User {}
来源：http://blog.yfazqb.com/Article/details/gqumwwppu.sHtML

JS:   class User {}
来源：http://www.blog.tarul.cn/Article/details/gmiukslwf.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.yfazqb.com/Article/details/gcqpjnwrs.sHtML

Java: class User {}
来源：http://read.share.sjlbkw.cn/Article/details/gdzuxwlsm.sHtML

Go:   type User struct { Name string }
来源：http://3g.bbcook.cn/Article/details/gchabjctn.sHtML

Ruby: class User; end
来源：http://wap.sjlbkw.cn/Article/details/gynqmmsab.sHtML

C#:   class User {}
来源：http://www.share.yfazqb.com/Article/details/gshiwuxgs.sHtML

[G02] 构造函数
来源：http://www.share.sjlbkw.cn/Article/details/gwoyqzlkc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.bbcook.cn/Article/details/gplinldpp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.tarul.cn/Article/details/gpazqiips.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.tarul.cn/Article/details/gyrkfizdd.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.bbcook.cn/Article/details/geotavrrk.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.bbcook.cn/Article/details/gvcvnzurk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.epnwcf.com/Article/details/gwehyuegq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.tarul.cn/Article/details/gnnqefulb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fktsv.cn/Article/details/gpwicvtgz.sHtML

[G03] 实例属性
来源：http://www.m.share.fktsv.cn/Article/details/gnraqmlhq.sHtML

Py:   self.name = "x"
来源：http://blog.vehdjk.com/Article/details/gquohxamn.sHtML

PHP:  public string $name = "x";
来源：http://3g.bbcook.cn/Article/details/gjxqyeseb.sHtML

JS:   this.name = "x";
来源：http://mobile.bbcook.cn/Article/details/gyarlxpyu.sHtML

TS:   name: string = "x";
来源：http://mobile.yfazqb.com/Article/details/gipfusbvr.sHtML

Java: private String name;
来源：http://www.share.tarul.cn/Article/details/ggtkkftgi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.bbcook.cn/Article/details/gcebqputp.sHtML

Ruby: @name = "x"
来源：http://mobile.vehdjk.com/Article/details/gtwlkjpla.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.yfazqb.com/Article/details/gsqyxvvzw.sHtML

[G04] 定义方法
来源：http://www.m.share.bbcook.cn/Article/details/goddjqvad.sHtML

Py:   def greet(self): return self.name
来源：http://blog.yfazqb.com/Article/details/gyobexckl.sHtML


<!-- 参考信息 -->