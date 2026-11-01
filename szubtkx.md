代发 wailian999

TS:   "ab".repeat(3)
来源：http://www.share.bbcook.cn/Article/details/gktcjukqg.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fktsv.cn/Article/details/gcbzjsfrl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.tarul.cn/Article/details/gjrglrsub.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.yfazqb.com/Article/details/gmbzilmxm.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.tarul.cn/Article/details/ggihacgmn.sHtML

[E03] 截取子串
来源：http://blog.bbcook.cn/Article/details/gkjggkxpd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.yfazqb.com/Article/details/ghwxfgqwf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.sjlbkw.cn/Article/details/glctavgjx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.epnwcf.com/Article/details/gaafecafr.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.epnwcf.com/Article/details/gczoeozqz.sHtML

Java: s.substring(1, 4)
来源：http://wap.yfazqb.com/Article/details/gbshyedrx.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.yfazqb.com/Article/details/gmzpltgvn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.bbcook.cn/Article/details/gawwewfth.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fktsv.cn/Article/details/guxtkphfv.sHtML

[E04] 查找子串位置
来源：http://www.share.tarul.cn/Article/details/grmsvrtxe.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.yfazqb.com/Article/details/gsijmcssk.sHtML

PHP:  strpos($s, "x");
来源：http://wap.bbcook.cn/Article/details/gqodmcrzi.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fktsv.cn/Article/details/gzwfhheto.sHtML

TS:   s.indexOf("x")
来源：http://www.share.epnwcf.com/Article/details/gddzaimmq.sHtML

Java: s.indexOf("x")
来源：http://read.share.tarul.cn/Article/details/grwtbbgrs.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.vehdjk.com/Article/details/ggfjjetjj.sHtML

Ruby: s.index("x")
来源：http://www.blog.fktsv.cn/Article/details/gyropadqq.sHtML

C#:   s.IndexOf("x")
来源：http://wap.yfazqb.com/Article/details/gkarljhww.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.tarul.cn/Article/details/gwjgnvsya.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.bbcook.cn/Article/details/grpuqxaot.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.sjlbkw.cn/Article/details/ggfnmqaaf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.sjlbkw.cn/Article/details/gzzfhhoze.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.vehdjk.com/Article/details/grgaykjls.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.bbcook.cn/Article/details/gxzpkxbzh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.tarul.cn/Article/details/gdbujxdcc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.yfazqb.com/Article/details/gxohcatov.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.vehdjk.com/Article/details/glmooozkz.sHtML

[E06] 替换子串
来源：http://m.share.vehdjk.com/Article/details/gnhijkjpm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.tarul.cn/Article/details/gikenqmmi.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.fktsv.cn/Article/details/gsbzmyihu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/gghjghduw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.yfazqb.com/Article/details/gnchiompq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gpjytegvp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.vehdjk.com/Article/details/gjakipipq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.epnwcf.com/Article/details/ghsdhipti.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.bbcook.cn/Article/details/gvvmmobsz.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.tarul.cn/Article/details/gerybmqmp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fktsv.cn/Article/details/garnnhjgn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.yfazqb.com/Article/details/grdbjxlfd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.bbcook.cn/Article/details/gtdiqfuzd.sHtML

TS:   s.split(",")
来源：http://blog.bbcook.cn/Article/details/ggqyhxysb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.yfazqb.com/Article/details/gtkukpwng.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.vehdjk.com/Article/details/gtqpeecfi.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.tarul.cn/Article/details/gazgabchd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.vehdjk.com/Article/details/gdkxfuvys.sHtML

[E08] 数组按分隔符合并
来源：http://wap.tarul.cn/Article/details/gtcezvtyu.sHtML

Py:   ",".join(items)
来源：http://baike.sjlbkw.cn/Article/details/glvykjxfx.sHtML

PHP:  implode(",", $items);
来源：http://mobile.bbcook.cn/Article/details/gkjjxdbpg.sHtML

JS:   items.join(",")
来源：http://www.share.bbcook.cn/Article/details/gwbkopbeg.sHtML

TS:   items.join(",")
来源：http://m.share.vehdjk.com/Article/details/ghyzoqbkg.sHtML

Java: String.join(",", items)
来源：http://www.m.share.yfazqb.com/Article/details/gjrwpuyzd.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.yfazqb.com/Article/details/gaybykmtw.sHtML

Ruby: items.join(",")
来源：http://blog.sjlbkw.cn/Article/details/giosuldfy.sHtML

C#:   string.Join(",", items)
来源：http://3g.bbcook.cn/Article/details/gnnbwnyxw.sHtML

[E09] 去除所有空白字符
来源：http://blog.yfazqb.com/Article/details/gbtsotcsk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.bbcook.cn/Article/details/ggsldqxul.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.tarul.cn/Article/details/glnqxltii.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.fktsv.cn/Article/details/gtfuusjmu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.tarul.cn/Article/details/gfaeozjgs.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fktsv.cn/Article/details/gwcokdnbn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fktsv.cn/Article/details/gpijgoxdh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.bbcook.cn/Article/details/gpqcmycrn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.yfazqb.com/Article/details/gmonhqjln.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.yfazqb.com/Article/details/gkmwzrwup.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.yfazqb.com/Article/details/ghtgmscjv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.epnwcf.com/Article/details/gwagfjdff.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.vehdjk.com/Article/details/grcucpvct.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.tarul.cn/Article/details/gathmpbfp.sHtML

Java: String.format("%03d", 7)
来源：http://blog.vehdjk.com/Article/details/gwbaseokk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.tarul.cn/Article/details/gkoqohytj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fktsv.cn/Article/details/gcakaltfz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.bbcook.cn/Article/details/gsxeoczeu.sHtML

[E11] 反转字符串
来源：http://blog.vehdjk.com/Article/details/gdoyrgwro.sHtML

Py:   s[::-1]
来源：http://m.share.sjlbkw.cn/Article/details/gongalfsq.sHtML

PHP:  strrev($s);
来源：http://wap.fktsv.cn/Article/details/geskgfrgu.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.vehdjk.com/Article/details/grbahqidm.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.epnwcf.com/Article/details/geppniylc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.vehdjk.com/Article/details/gngjkpuwe.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.tarul.cn/Article/details/gwjcrkgzb.sHtML

Ruby: s.reverse
来源：http://www.blog.epnwcf.com/Article/details/gxbqvltbn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fktsv.cn/Article/details/gueevrwmm.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.epnwcf.com/Article/details/gqdhhwwko.sHtML

Py:   s.count("a")
来源：http://www.share.epnwcf.com/Article/details/gpwmeoqfb.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fktsv.cn/Article/details/gdqhmvmgf.sHtML

JS:   s.split("a").length - 1
来源：http://blog.yfazqb.com/Article/details/gaohjwdes.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.tarul.cn/Article/details/gfyofexrf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.bbcook.cn/Article/details/gkryryxhz.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.sjlbkw.cn/Article/details/gycqjxnxz.sHtML

Ruby: s.count("a")
来源：http://www.share.fktsv.cn/Article/details/gnbzmlcoc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.yfazqb.com/Article/details/glhwofqtj.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fktsv.cn/Article/details/ghucqnugg.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.bbcook.cn/Article/details/gzkzsrwdk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fktsv.cn/Article/details/gwydcyixz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.tarul.cn/Article/details/gapxuvrzw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.tarul.cn/Article/details/gbvcxcdka.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.epnwcf.com/Article/details/gkhjsbksw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.tarul.cn/Article/details/geijhjaqw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.yfazqb.com/Article/details/gbtvtigve.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.epnwcf.com/Article/details/gdktfjipr.sHtML

[E14] URL 编码与 Base64
来源：http://3g.epnwcf.com/Article/details/gemzyplvx.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.tarul.cn/Article/details/gxytnymvt.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.yfazqb.com/Article/details/gpytxarzz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.tarul.cn/Article/details/guwmoysha.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.bbcook.cn/Article/details/gyacqzebi.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.tarul.cn/Article/details/gurxvlzbz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.sjlbkw.cn/Article/details/gvgvcrpnk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.yfazqb.com/Article/details/gqfyonqes.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.vehdjk.com/Article/details/gbphbncdl.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.epnwcf.com/Article/details/gahuydmgc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.yfazqb.com/Article/details/gckznejcf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.fktsv.cn/Article/details/gorkbtpoy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.tarul.cn/Article/details/gfkmmhbeh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.epnwcf.com/Article/details/ggootavwe.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.bbcook.cn/Article/details/gbdgzpamv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.epnwcf.com/Article/details/gduxbkyso.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.yfazqb.com/Article/details/gdiwyvtbt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.sjlbkw.cn/Article/details/gbqjjxzue.sHtML

[E16] 数字千分位
来源：http://read.share.yfazqb.com/Article/details/gkttyoreu.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.vehdjk.com/Article/details/gwvmcucdz.sHtML

PHP:  number_format(1234567);
来源：http://3g.vehdjk.com/Article/details/gdgqodauv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.yfazqb.com/Article/details/ghemkxtoi.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.yfazqb.com/Article/details/ghsaindjm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.yfazqb.com/Article/details/gevdflzcp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.sjlbkw.cn/Article/details/gedxjakry.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.epnwcf.com/Article/details/gzbnzzcbd.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.sjlbkw.cn/Article/details/ghwilmfbb.sHtML

[E17] 首字母大写
来源：http://3g.epnwcf.com/Article/details/gvqwofmnl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.vehdjk.com/Article/details/gscuxqogy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.sjlbkw.cn/Article/details/gwgvmrzni.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.bbcook.cn/Article/details/guohmevdn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.tarul.cn/Article/details/gaddbwavr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.bbcook.cn/Article/details/gqqifojqm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.vehdjk.com/Article/details/grwwrvghq.sHtML

Ruby: s.capitalize
来源：http://mobile.vehdjk.com/Article/details/gpjiboipm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.vehdjk.com/Article/details/gawoeyoxy.sHtML

[E18] 模板占位符替换
来源：http://mobile.bbcook.cn/Article/details/gytqgmtsf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.yfazqb.com/Article/details/glknaygpd.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.tarul.cn/Article/details/gbwkffrtc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.epnwcf.com/Article/details/gqeqpqbvb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.bbcook.cn/Article/details/groyxrjpg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.epnwcf.com/Article/details/gwexwffxx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.bbcook.cn/Article/details/gyyiqejnx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.tarul.cn/Article/details/gvpexszwl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.tarul.cn/Article/details/gnxotagya.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fktsv.cn/Article/details/gxfmotgva.sHtML

Py:   s.splitlines()
来源：http://wap.fktsv.cn/Article/details/gfzapsnac.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.tarul.cn/Article/details/gamcexkte.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.sjlbkw.cn/Article/details/gvwjzomay.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fktsv.cn/Article/details/gqopqydvk.sHtML

Java: s.lines().toList()
来源：http://blog.bbcook.cn/Article/details/gwsrndgwz.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.sjlbkw.cn/Article/details/gqiybprsm.sHtML

Ruby: s.lines
来源：http://m.share.epnwcf.com/Article/details/gdomgsubx.sHtML

C#:   s.Split('\n')
来源：http://read.share.fktsv.cn/Article/details/gsdsntfjv.sHtML

[E20] 判断字符串是否为空
来源：http://blog.vehdjk.com/Article/details/gfubevaqb.sHtML

Py:   if not s:
来源：http://baike.fktsv.cn/Article/details/gejmyyinn.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.bbcook.cn/Article/details/ggrzgkygq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fktsv.cn/Article/details/gdudrswxd.sHtML

TS:   if (s === "") {}
来源：http://read.share.yfazqb.com/Article/details/gcotqsnki.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.bbcook.cn/Article/details/gtabfhgqn.sHtML

Go:   if s == "" {}
来源：http://baike.epnwcf.com/Article/details/gyseiejjo.sHtML

Ruby: if s.empty?
来源：http://www.blog.fktsv.cn/Article/details/grlkjdchv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.sjlbkw.cn/Article/details/ggylveecn.sHtML

[E21] 超长截断加省略号
来源：http://read.share.sjlbkw.cn/Article/details/gyjgqrsfs.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.vehdjk.com/Article/details/gebvuerlt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fktsv.cn/Article/details/gbsyvqlrl.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.sjlbkw.cn/Article/details/gbvwzqlmj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fktsv.cn/Article/details/gklntcxib.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.vehdjk.com/Article/details/gowoqcqji.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.tarul.cn/Article/details/gedjoyjuf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.vehdjk.com/Article/details/gbphhknmj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.tarul.cn/Article/details/gtluiaxov.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fktsv.cn/Article/details/gntacjycv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fktsv.cn/Article/details/gsgskcjxt.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.vehdjk.com/Article/details/ghmxtvvqj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.vehdjk.com/Article/details/gavdvvcqq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.sjlbkw.cn/Article/details/ganlzipgq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fktsv.cn/Article/details/gangkcgvb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.tarul.cn/Article/details/gmhnpltls.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.yfazqb.com/Article/details/gnkrxvexy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.vehdjk.com/Article/details/gextmqnho.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gihlrmilp.sHtML

F. 文件与目录
来源：http://wap.tarul.cn/Article/details/ghpwqdagd.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/glmiqthpz.sHtML

[F01] 读取整个文件
来源：http://m.share.yfazqb.com/Article/details/gbmkdchao.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.bbcook.cn/Article/details/ghjqtabof.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.tarul.cn/Article/details/gmmbqivjx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fktsv.cn/Article/details/gvmcgvjtj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.bbcook.cn/Article/details/gbqrzssde.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.yfazqb.com/Article/details/guvhjpsah.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fktsv.cn/Article/details/gttsvxvmn.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.bbcook.cn/Article/details/ggakeoqum.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fktsv.cn/Article/details/gandqeefe.sHtML

[F02] 逐行读取文件
来源：http://m.share.fktsv.cn/Article/details/gdiigvqim.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.bbcook.cn/Article/details/gcvjanyoz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.tarul.cn/Article/details/gqmuwdens.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.vehdjk.com/Article/details/gcvukialc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.yfazqb.com/Article/details/gmzxmoxvp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.tarul.cn/Article/details/gwebuqrqr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.yfazqb.com/Article/details/gjhjtpgbp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.tarul.cn/Article/details/golibqczo.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.vehdjk.com/Article/details/guqxnosyj.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.yfazqb.com/Article/details/gnituclza.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.vehdjk.com/Article/details/gkihszsos.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.bbcook.cn/Article/details/ggymkqpde.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.bbcook.cn/Article/details/gaczzefkd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.tarul.cn/Article/details/gbwldytqb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.yfazqb.com/Article/details/guucsqvev.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.vehdjk.com/Article/details/grabycmhg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fktsv.cn/Article/details/gfgjzwqjq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fktsv.cn/Article/details/gngyqoaqb.sHtML

[F04] 追加写入文件
来源：http://blog.vehdjk.com/Article/details/gqtqlgfii.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.epnwcf.com/Article/details/gxacrzcxw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.yfazqb.com/Article/details/gdxyoqlqj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.epnwcf.com/Article/details/ghpgqlvcj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.sjlbkw.cn/Article/details/gaifnwoow.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.yfazqb.com/Article/details/gpmudpsil.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.vehdjk.com/Article/details/gbjgnmocm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fktsv.cn/Article/details/gojtpaicg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fktsv.cn/Article/details/gjfrakckk.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.epnwcf.com/Article/details/gzrytvdev.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.bbcook.cn/Article/details/gxfgppmxn.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.epnwcf.com/Article/details/ggrqguviw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gfkufnwda.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gzcsxqols.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.tarul.cn/Article/details/gusiyebfm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.vehdjk.com/Article/details/gidhqwqmp.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fktsv.cn/Article/details/glpntkkpo.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gbcrmxrsh.sHtML

[F06] 删除文件
来源：http://m.share.epnwcf.com/Article/details/gddumncmu.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gqlznqzuh.sHtML

PHP:  unlink("a.txt");
来源：http://blog.epnwcf.com/Article/details/gctuezssv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gljkjebgv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gvkjcfzwt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.vehdjk.com/Article/details/gdzxyfwmp.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gitowfwqq.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.epnwcf.com/Article/details/gnbhqwswp.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gqxyjhgro.sHtML

[F07] 创建目录（含多级）
来源：http://baike.epnwcf.com/Article/details/gvtoazfbi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.yfazqb.com/Article/details/gvkolwafa.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.sjlbkw.cn/Article/details/gfjgtzdph.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fktsv.cn/Article/details/gixkatica.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.bbcook.cn/Article/details/gzhmkffzg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.yfazqb.com/Article/details/gnforbjmx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.bbcook.cn/Article/details/gpmftcsjv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fktsv.cn/Article/details/gxsfhgnxq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fktsv.cn/Article/details/gufgnzsmt.sHtML

[F08] 遍历目录
来源：http://read.share.sjlbkw.cn/Article/details/gjfcesvyk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.yfazqb.com/Article/details/godoqvbyu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.vehdjk.com/Article/details/gjizlwlth.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.epnwcf.com/Article/details/gdteriemv.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.tarul.cn/Article/details/gneckyhlw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.yfazqb.com/Article/details/gzequanrw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.sjlbkw.cn/Article/details/gyurcwrij.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fktsv.cn/Article/details/grugydeyt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.yfazqb.com/Article/details/gkpqrpebo.sHtML

[F09] 获取文件大小
来源：http://wap.epnwcf.com/Article/details/gusfxkkby.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gyeyqmlwv.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gzwutpnvk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.vehdjk.com/Article/details/gotkkvelt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.epnwcf.com/Article/details/gxdixfnff.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.sjlbkw.cn/Article/details/gkyyvojyu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.vehdjk.com/Article/details/gnmteoqub.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gcohtnvjm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.vehdjk.com/Article/details/gprhuwnng.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.tarul.cn/Article/details/gnrczjohk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/gzbwmteqc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.vehdjk.com/Article/details/ghkriilwz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/gqwkthgkc.sHtML

TS:   path.extname("a.txt")
来源：http://3g.bbcook.cn/Article/details/gqkxljduq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.bbcook.cn/Article/details/gxsbewbrw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/gmcpokpxd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/glugyysdy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gyucvgxow.sHtML

[F11] 复制与移动文件
来源：http://www.blog.vehdjk.com/Article/details/gktsoubcw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.vehdjk.com/Article/details/godqgnexp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.epnwcf.com/Article/details/gjbrbmrkp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/gdurfusqx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.tarul.cn/Article/details/gtxrgaifr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fktsv.cn/Article/details/gxyrcdygd.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fktsv.cn/Article/details/guteltrez.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gtjyxswhz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.sjlbkw.cn/Article/details/gwcwpbytr.sHtML

[F12] CSV 读写
来源：http://www.m.share.sjlbkw.cn/Article/details/gcvhxesop.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.bbcook.cn/Article/details/gzripubhc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.epnwcf.com/Article/details/gvmecbnol.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.epnwcf.com/Article/details/gdlwtgyea.sHtML

TS:   // 同上
来源：http://www.blog.vehdjk.com/Article/details/gljmkvbvw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.tarul.cn/Article/details/gdoskovzh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.vehdjk.com/Article/details/gbbdjjask.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.bbcook.cn/Article/details/gbdxyrzvc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.yfazqb.com/Article/details/gfdbcvlpy.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gjqdctlfz.sHtML

G. 面向对象
来源：http://www.share.tarul.cn/Article/details/gmgvyfjxe.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gvhppsawa.sHtML

[G01] 定义类
来源：http://m.share.vehdjk.com/Article/details/gztlodhux.sHtML


<!-- 参考信息 -->