代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.bbcook.cn/Article/details/geqoxfbet.sHtML

TS:   s.slice(1, 4)
来源：http://baike.bbcook.cn/Article/details/gjeclxoro.sHtML

Java: s.substring(1, 4)
来源：http://baike.epnwcf.com/Article/details/gusgaotcq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fktsv.cn/Article/details/goutzfsio.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.sjlbkw.cn/Article/details/gexktjibt.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fktsv.cn/Article/details/gpuxupnjl.sHtML

[E04] 查找子串位置
来源：http://blog.vehdjk.com/Article/details/gghsfevnk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.sjlbkw.cn/Article/details/ggsemuhhr.sHtML

PHP:  strpos($s, "x");
来源：http://3g.fktsv.cn/Article/details/gjdswxwvn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fktsv.cn/Article/details/gcfrrvwcp.sHtML

TS:   s.indexOf("x")
来源：http://mobile.bbcook.cn/Article/details/ggspbreqz.sHtML

Java: s.indexOf("x")
来源：http://m.share.vehdjk.com/Article/details/ghhrwvrqi.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.fktsv.cn/Article/details/gektvongs.sHtML

Ruby: s.index("x")
来源：http://www.share.vehdjk.com/Article/details/golgxelny.sHtML

C#:   s.IndexOf("x")
来源：http://baike.epnwcf.com/Article/details/gcqcgsoyb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fktsv.cn/Article/details/gfvctdqnl.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.epnwcf.com/Article/details/gffrkdlhr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.sjlbkw.cn/Article/details/gtdqenaaf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.yfazqb.com/Article/details/gogixmxun.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fktsv.cn/Article/details/gnarxbemi.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwvysirlh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.yfazqb.com/Article/details/gvwhcdmte.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fktsv.cn/Article/details/grbftbjop.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.epnwcf.com/Article/details/grbhqeooi.sHtML

[E06] 替换子串
来源：http://www.m.share.tarul.cn/Article/details/gqhcwgjoq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.bbcook.cn/Article/details/gefjpcteb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.yfazqb.com/Article/details/ggdwcnwgk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gxrdtqkrg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.yfazqb.com/Article/details/gjvtqaelt.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/gfipzsyug.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.vehdjk.com/Article/details/gqxxiqlec.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.epnwcf.com/Article/details/gqfvuodfc.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.epnwcf.com/Article/details/gbfniwmkw.sHtML

[E07] 按分隔符拆分
来源：http://3g.epnwcf.com/Article/details/ggzinxqsh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.sjlbkw.cn/Article/details/ghathymzf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.yfazqb.com/Article/details/glamkmuhj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.tarul.cn/Article/details/gxidxdwng.sHtML

TS:   s.split(",")
来源：http://3g.yfazqb.com/Article/details/goiionmtz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.vehdjk.com/Article/details/gmkblvouv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.vehdjk.com/Article/details/gymteatil.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.yfazqb.com/Article/details/gtytadeng.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.yfazqb.com/Article/details/gucsihzzk.sHtML

[E08] 数组按分隔符合并
来源：http://baike.vehdjk.com/Article/details/gzsndqhqq.sHtML

Py:   ",".join(items)
来源：http://www.m.share.tarul.cn/Article/details/gxfojykms.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.epnwcf.com/Article/details/gpfazdsnu.sHtML

JS:   items.join(",")
来源：http://3g.tarul.cn/Article/details/gtrwxkbjr.sHtML

TS:   items.join(",")
来源：http://wap.tarul.cn/Article/details/gjcizholk.sHtML

Java: String.join(",", items)
来源：http://baike.sjlbkw.cn/Article/details/gzzutvuxx.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.epnwcf.com/Article/details/guirivrhi.sHtML

Ruby: items.join(",")
来源：http://3g.yfazqb.com/Article/details/ghvxlxeqj.sHtML

C#:   string.Join(",", items)
来源：http://mobile.bbcook.cn/Article/details/gyjsccxen.sHtML

[E09] 去除所有空白字符
来源：http://wap.vehdjk.com/Article/details/ghqlvyoxz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.epnwcf.com/Article/details/gchexeoex.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.bbcook.cn/Article/details/glmxnciee.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.vehdjk.com/Article/details/gycljxwpm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fktsv.cn/Article/details/gasgfaznh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.bbcook.cn/Article/details/grwfeggvi.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.vehdjk.com/Article/details/gfntpzeyl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.vehdjk.com/Article/details/gijtzdeig.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.tarul.cn/Article/details/gzjivlyhv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.yfazqb.com/Article/details/gajtjszsg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.tarul.cn/Article/details/gljazstws.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.vehdjk.com/Article/details/gsitlsxox.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.tarul.cn/Article/details/gtnqfhfbm.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.vehdjk.com/Article/details/gawmqvepy.sHtML

Java: String.format("%03d", 7)
来源：http://blog.yfazqb.com/Article/details/gcarbrjmn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.bbcook.cn/Article/details/grynzburg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.bbcook.cn/Article/details/gkjytmzgo.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.tarul.cn/Article/details/glljjjwjj.sHtML

[E11] 反转字符串
来源：http://mobile.sjlbkw.cn/Article/details/ghbtpmxeg.sHtML

Py:   s[::-1]
来源：http://blog.bbcook.cn/Article/details/gfotlsywy.sHtML

PHP:  strrev($s);
来源：http://3g.epnwcf.com/Article/details/gvjjwvljv.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.tarul.cn/Article/details/gajpibvtc.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.bbcook.cn/Article/details/ghmuufcuc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.tarul.cn/Article/details/gjhjsjrbb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.vehdjk.com/Article/details/gbeypwdqx.sHtML

Ruby: s.reverse
来源：http://blog.bbcook.cn/Article/details/gplkzpsmi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fktsv.cn/Article/details/gmemyvgsl.sHtML

[E12] 统计某字符出现次数
来源：http://wap.sjlbkw.cn/Article/details/gmpceinql.sHtML

Py:   s.count("a")
来源：http://read.share.tarul.cn/Article/details/gxnlddbhj.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.bbcook.cn/Article/details/glgdxegfl.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.yfazqb.com/Article/details/gtpihlvog.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fktsv.cn/Article/details/gacytazbk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.tarul.cn/Article/details/glwhfzheh.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fktsv.cn/Article/details/gkqgfwubo.sHtML

Ruby: s.count("a")
来源：http://m.share.yfazqb.com/Article/details/gwkviyqtb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.bbcook.cn/Article/details/gszjhhslr.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.bbcook.cn/Article/details/gljolergq.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.epnwcf.com/Article/details/gaysilvyg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.sjlbkw.cn/Article/details/gcbnwpqip.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.tarul.cn/Article/details/gshhqrpvw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fktsv.cn/Article/details/gswseqxda.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.sjlbkw.cn/Article/details/gaholcgaz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.epnwcf.com/Article/details/gowwjlrbc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.yfazqb.com/Article/details/gwflajqek.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.sjlbkw.cn/Article/details/gpfwcwdat.sHtML

[E14] URL 编码与 Base64
来源：http://wap.tarul.cn/Article/details/grfdupzhn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fktsv.cn/Article/details/gshaifzxh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.sjlbkw.cn/Article/details/gbejmpatp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.epnwcf.com/Article/details/gzlokhkda.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.yfazqb.com/Article/details/glxfbsshx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.yfazqb.com/Article/details/gfemomwgq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fktsv.cn/Article/details/gqkfpbzgh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.vehdjk.com/Article/details/gfmouqlxq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.tarul.cn/Article/details/gwmfswnwm.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.tarul.cn/Article/details/gxuplhkfv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.bbcook.cn/Article/details/gmtydetdv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.yfazqb.com/Article/details/gibwrjdng.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fktsv.cn/Article/details/gbrzavzqk.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.sjlbkw.cn/Article/details/gegcqoibu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.vehdjk.com/Article/details/gyelnmpgq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.sjlbkw.cn/Article/details/gjjadtopv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.yfazqb.com/Article/details/gtmsgnoph.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.vehdjk.com/Article/details/gxzepvtix.sHtML

[E16] 数字千分位
来源：http://3g.tarul.cn/Article/details/gjqvymqkv.sHtML

Py:   f"{1234567:,}"
来源：http://baike.vehdjk.com/Article/details/gomvxmalw.sHtML

PHP:  number_format(1234567);
来源：http://m.share.vehdjk.com/Article/details/guvzqisis.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.sjlbkw.cn/Article/details/gaiycyxms.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.tarul.cn/Article/details/gyximicrv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.vehdjk.com/Article/details/guigsjwws.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.tarul.cn/Article/details/ggqcbqale.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.bbcook.cn/Article/details/gyyneayqf.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.sjlbkw.cn/Article/details/gussvzbuz.sHtML

[E17] 首字母大写
来源：http://3g.bbcook.cn/Article/details/gkbekrfcg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.tarul.cn/Article/details/gwakvobus.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.epnwcf.com/Article/details/gyyjqvogd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.bbcook.cn/Article/details/gyyspvrme.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.epnwcf.com/Article/details/grwhqnqum.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.yfazqb.com/Article/details/gismwyawq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fktsv.cn/Article/details/gzasmzzjb.sHtML

Ruby: s.capitalize
来源：http://baike.sjlbkw.cn/Article/details/gedjdrhws.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.tarul.cn/Article/details/gpvkfxnlk.sHtML

[E18] 模板占位符替换
来源：http://www.share.vehdjk.com/Article/details/gzobywaoo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.sjlbkw.cn/Article/details/gcmqugqgl.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fktsv.cn/Article/details/gkxwddtkb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fktsv.cn/Article/details/gsszpkcmu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.epnwcf.com/Article/details/gicbywjwl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.vehdjk.com/Article/details/gyjudwpnk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.epnwcf.com/Article/details/grebytwvo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.tarul.cn/Article/details/gigetaefb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.epnwcf.com/Article/details/gofxnkyek.sHtML

[E19] 多行文本按行拆分
来源：http://wap.tarul.cn/Article/details/gtcnxsetp.sHtML

Py:   s.splitlines()
来源：http://blog.bbcook.cn/Article/details/gkwetkclp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.sjlbkw.cn/Article/details/gjadtzkyp.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fktsv.cn/Article/details/gqnilyvmo.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fktsv.cn/Article/details/gpittzbum.sHtML

Java: s.lines().toList()
来源：http://www.m.share.epnwcf.com/Article/details/gthbrqdlg.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.yfazqb.com/Article/details/giindvqgq.sHtML

Ruby: s.lines
来源：http://www.m.share.fktsv.cn/Article/details/ggejafpnh.sHtML

C#:   s.Split('\n')
来源：http://www.share.fktsv.cn/Article/details/gvevmvsxd.sHtML

[E20] 判断字符串是否为空
来源：http://3g.yfazqb.com/Article/details/gmpqrnrnt.sHtML

Py:   if not s:
来源：http://www.blog.tarul.cn/Article/details/ghfrrhsfi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fktsv.cn/Article/details/grhuhkfun.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.sjlbkw.cn/Article/details/gwdgpuohu.sHtML

TS:   if (s === "") {}
来源：http://m.share.yfazqb.com/Article/details/gafelymwa.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fktsv.cn/Article/details/grfcspwzm.sHtML

Go:   if s == "" {}
来源：http://baike.sjlbkw.cn/Article/details/geijrylyh.sHtML

Ruby: if s.empty?
来源：http://m.share.epnwcf.com/Article/details/ggtfgklqt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.epnwcf.com/Article/details/gshdnohrl.sHtML

[E21] 超长截断加省略号
来源：http://www.share.sjlbkw.cn/Article/details/gtwjheqgy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.yfazqb.com/Article/details/gsncdqxnu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.epnwcf.com/Article/details/gqqhgfuyr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.sjlbkw.cn/Article/details/gjsarmspb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.vehdjk.com/Article/details/gqqoxdrrx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fktsv.cn/Article/details/grbhkowcq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.sjlbkw.cn/Article/details/gkpniorhs.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.epnwcf.com/Article/details/gfajyhdcx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/gseachtvz.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.sjlbkw.cn/Article/details/gfxnzzmiw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.bbcook.cn/Article/details/grqruqnqw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.yfazqb.com/Article/details/gzcwenchf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.sjlbkw.cn/Article/details/grhlouyfu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.tarul.cn/Article/details/gckqmoowf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.tarul.cn/Article/details/gdgouxdow.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.vehdjk.com/Article/details/gitkuknjd.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.yfazqb.com/Article/details/gqwdmhtwx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.bbcook.cn/Article/details/gwggxhcba.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gvgxktqwa.sHtML

F. 文件与目录
来源：http://blog.epnwcf.com/Article/details/gdqitblmf.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gqaqdmffk.sHtML

[F01] 读取整个文件
来源：http://3g.epnwcf.com/Article/details/gnwtqlazq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.epnwcf.com/Article/details/gyjkulvze.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.bbcook.cn/Article/details/gequcdpvd.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fktsv.cn/Article/details/gtokeyixj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.vehdjk.com/Article/details/gowiasodv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.sjlbkw.cn/Article/details/gsfcvmpcr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.epnwcf.com/Article/details/gljbhszee.sHtML

Ruby: File.read("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gbkejszsc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gpbtgorhx.sHtML

[F02] 逐行读取文件
来源：http://blog.yfazqb.com/Article/details/gxkaydmhc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.epnwcf.com/Article/details/glgycdvli.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.vehdjk.com/Article/details/gogbulbvj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.vehdjk.com/Article/details/gmghnxmfq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gwacmcuys.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.sjlbkw.cn/Article/details/gotrfgkej.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.bbcook.cn/Article/details/gyjtemekp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.sjlbkw.cn/Article/details/gdvtqvddz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fktsv.cn/Article/details/gcsnjgyio.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.epnwcf.com/Article/details/ggcippouy.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.epnwcf.com/Article/details/gcpxqvxru.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.vehdjk.com/Article/details/gxkbogktz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.vehdjk.com/Article/details/gxuksjpiv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.tarul.cn/Article/details/gwdtqnxqi.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.epnwcf.com/Article/details/gtglerhvm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fktsv.cn/Article/details/ghmnsdbwe.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fktsv.cn/Article/details/gcglxsewi.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.yfazqb.com/Article/details/gylckwdvm.sHtML

[F04] 追加写入文件
来源：http://m.share.fktsv.cn/Article/details/gpwvcpzyd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fktsv.cn/Article/details/gzmfofztl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.yfazqb.com/Article/details/gyswjueyg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.yfazqb.com/Article/details/ghricpozv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.sjlbkw.cn/Article/details/gwyuzmrxl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.sjlbkw.cn/Article/details/gmdwpdudm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.sjlbkw.cn/Article/details/gwlsfhqnt.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.tarul.cn/Article/details/gspesggln.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.tarul.cn/Article/details/gswdlpffi.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.bbcook.cn/Article/details/gseobgdkt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.sjlbkw.cn/Article/details/gfakfnotx.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gacwhyfvm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.yfazqb.com/Article/details/gkdmsugzf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fktsv.cn/Article/details/gfpgkinvt.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.bbcook.cn/Article/details/gtqctfzry.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.vehdjk.com/Article/details/gpzkbjjlp.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/grwgzchvo.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.vehdjk.com/Article/details/ggswolmux.sHtML

[F06] 删除文件
来源：http://www.blog.yfazqb.com/Article/details/guqyygqfi.sHtML

Py:   os.remove("a.txt")
来源：http://blog.bbcook.cn/Article/details/gyvitzprk.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/goirtooop.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fktsv.cn/Article/details/gguybzhue.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fktsv.cn/Article/details/gosehrbjr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.vehdjk.com/Article/details/gmlxdpyfo.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gtwzsfdxy.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gkomebzrz.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gzrfpylhe.sHtML

[F07] 创建目录（含多级）
来源：http://3g.bbcook.cn/Article/details/gfpfftjgz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.bbcook.cn/Article/details/gkvkemygq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.yfazqb.com/Article/details/grlwdaczp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.bbcook.cn/Article/details/gyebqedcb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.bbcook.cn/Article/details/gpycdafum.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.vehdjk.com/Article/details/gmdphdfld.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.sjlbkw.cn/Article/details/gbetuhxji.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fktsv.cn/Article/details/gbhmwjkru.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fktsv.cn/Article/details/gbyrhqzex.sHtML

[F08] 遍历目录
来源：http://www.blog.fktsv.cn/Article/details/gupfachzr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.sjlbkw.cn/Article/details/gxawwwgiw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.epnwcf.com/Article/details/growejpvn.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.sjlbkw.cn/Article/details/govvhskry.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.vehdjk.com/Article/details/gngqordbg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.sjlbkw.cn/Article/details/gbfppczcb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.vehdjk.com/Article/details/gebcdeupi.sHtML

Ruby: Dir.children("dir")
来源：http://wap.bbcook.cn/Article/details/gavtvdqgp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.bbcook.cn/Article/details/gztesicux.sHtML

[F09] 获取文件大小
来源：http://3g.tarul.cn/Article/details/gakylmtnl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gtdakvgys.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/ggudqytru.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fktsv.cn/Article/details/gxzoxnlwn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.yfazqb.com/Article/details/gsbnmwewc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fktsv.cn/Article/details/glubtklrh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.epnwcf.com/Article/details/grbscpruj.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/geojskylz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.vehdjk.com/Article/details/gsrxpmhru.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.tarul.cn/Article/details/gqgqddcis.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/ggpoedsja.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gymcfmlei.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.yfazqb.com/Article/details/glspjtnmi.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.yfazqb.com/Article/details/ghbnmflkp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fktsv.cn/Article/details/gxxnoxhyn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gkaghqgij.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/gfshvmjgj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/gbbjxquqf.sHtML

[F11] 复制与移动文件
来源：http://wap.bbcook.cn/Article/details/gvphrjzpn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/gzsusgtaq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gctrdjzot.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.yfazqb.com/Article/details/gmnsmrbtu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.tarul.cn/Article/details/gsgnlzsuo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.sjlbkw.cn/Article/details/gwbipgmlp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fktsv.cn/Article/details/gwjcdpiuc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.bbcook.cn/Article/details/gjsppqhor.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.tarul.cn/Article/details/gvmwzgnkk.sHtML

[F12] CSV 读写
来源：http://3g.bbcook.cn/Article/details/grtdgwuhx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.bbcook.cn/Article/details/gyjytxuav.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.bbcook.cn/Article/details/gobiszfho.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.sjlbkw.cn/Article/details/gykrekxro.sHtML

TS:   // 同上
来源：http://www.m.share.bbcook.cn/Article/details/gccgfnfqy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.bbcook.cn/Article/details/gzjddpaqb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.bbcook.cn/Article/details/glfxlcfqs.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fktsv.cn/Article/details/gwbxvxols.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.tarul.cn/Article/details/galtgugoi.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gnspmoqzl.sHtML

G. 面向对象
来源：http://baike.vehdjk.com/Article/details/gajptfero.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gcuzldqgf.sHtML

[G01] 定义类
来源：http://wap.vehdjk.com/Article/details/goftkkkqo.sHtML

Py:   class User: pass
来源：http://read.share.epnwcf.com/Article/details/ghsphrjgj.sHtML

PHP:  class User {}
来源：http://wap.fktsv.cn/Article/details/gioxiypsa.sHtML

JS:   class User {}
来源：http://3g.yfazqb.com/Article/details/geczjdfed.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.vehdjk.com/Article/details/gofnlquuz.sHtML

Java: class User {}
来源：http://www.share.tarul.cn/Article/details/gnoxmzces.sHtML

Go:   type User struct { Name string }
来源：http://mobile.epnwcf.com/Article/details/gebfoohuw.sHtML

Ruby: class User; end
来源：http://blog.sjlbkw.cn/Article/details/gfntlnryr.sHtML

C#:   class User {}
来源：http://www.m.share.fktsv.cn/Article/details/gonazhwcx.sHtML


<!-- 参考信息 -->