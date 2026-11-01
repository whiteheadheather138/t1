代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.sjlbkw.cn/Article/details/gwfhijzlp.sHtML

[E03] 截取子串
来源：http://3g.yfazqb.com/Article/details/grdrxhkvl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.sjlbkw.cn/Article/details/gixmuxfgq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.tarul.cn/Article/details/ghkhrnbbw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.sjlbkw.cn/Article/details/glvaexzlt.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.sjlbkw.cn/Article/details/gnjtjgfaa.sHtML

Java: s.substring(1, 4)
来源：http://baike.fktsv.cn/Article/details/gcoicsdzm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.vehdjk.com/Article/details/gtzcbdcku.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fktsv.cn/Article/details/gtdlhbdxh.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.bbcook.cn/Article/details/gjuywrdut.sHtML

[E04] 查找子串位置
来源：http://www.m.share.bbcook.cn/Article/details/gjrnnvswf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.sjlbkw.cn/Article/details/goquoiuna.sHtML

PHP:  strpos($s, "x");
来源：http://blog.tarul.cn/Article/details/gtokzlgmi.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.yfazqb.com/Article/details/gmuvsjhqh.sHtML

TS:   s.indexOf("x")
来源：http://wap.sjlbkw.cn/Article/details/gjgloxoch.sHtML

Java: s.indexOf("x")
来源：http://www.share.tarul.cn/Article/details/gqgpgkapx.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.epnwcf.com/Article/details/gcxuzseda.sHtML

Ruby: s.index("x")
来源：http://www.share.bbcook.cn/Article/details/ggqjjrczz.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.vehdjk.com/Article/details/gwpxtfqjk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.tarul.cn/Article/details/gpfsdpomz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.sjlbkw.cn/Article/details/gosxbtkfm.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.yfazqb.com/Article/details/guhopvure.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.bbcook.cn/Article/details/gjkzkpxhs.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fktsv.cn/Article/details/gendtwkpc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.sjlbkw.cn/Article/details/gqjncuspt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fktsv.cn/Article/details/gbvuwjmhn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.vehdjk.com/Article/details/gjoqkmltv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.epnwcf.com/Article/details/gbgruqrgs.sHtML

[E06] 替换子串
来源：http://blog.sjlbkw.cn/Article/details/gnvtvnyzu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.sjlbkw.cn/Article/details/gchpozwaf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fktsv.cn/Article/details/guymqtoku.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gzzosokit.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.tarul.cn/Article/details/gqezfkans.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.vehdjk.com/Article/details/gxfgfpyho.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.vehdjk.com/Article/details/gxnjconof.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gyrnfrklv.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.tarul.cn/Article/details/gexaillni.sHtML

[E07] 按分隔符拆分
来源：http://www.share.bbcook.cn/Article/details/gwygnppcj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.bbcook.cn/Article/details/gwefbfrfk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdoaezuve.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.yfazqb.com/Article/details/gtimlnpuh.sHtML

TS:   s.split(",")
来源：http://baike.tarul.cn/Article/details/gjsdsgetg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fktsv.cn/Article/details/gthjhjtxv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.epnwcf.com/Article/details/gunphkxao.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.tarul.cn/Article/details/gjvfybgdv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.bbcook.cn/Article/details/gmvvgvwrw.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.yfazqb.com/Article/details/gzgqohhnu.sHtML

Py:   ",".join(items)
来源：http://wap.tarul.cn/Article/details/gawgmtvfv.sHtML

PHP:  implode(",", $items);
来源：http://read.share.vehdjk.com/Article/details/gjfbnirdb.sHtML

JS:   items.join(",")
来源：http://www.share.fktsv.cn/Article/details/gzuzuyawt.sHtML

TS:   items.join(",")
来源：http://blog.epnwcf.com/Article/details/giisbssfs.sHtML

Java: String.join(",", items)
来源：http://mobile.epnwcf.com/Article/details/gxduxjdhu.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.yfazqb.com/Article/details/gvrzpnzgs.sHtML

Ruby: items.join(",")
来源：http://3g.epnwcf.com/Article/details/gfbukmxrt.sHtML

C#:   string.Join(",", items)
来源：http://baike.vehdjk.com/Article/details/gxyxnawhd.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.yfazqb.com/Article/details/guuzwpxmg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.epnwcf.com/Article/details/gbcdnkawf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.epnwcf.com/Article/details/grhpkulyb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.fktsv.cn/Article/details/gukhkkfzs.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.fktsv.cn/Article/details/gfbeaaoll.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fktsv.cn/Article/details/gywvioqwr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.bbcook.cn/Article/details/gzehrgfds.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.fktsv.cn/Article/details/gywzzxfaw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.epnwcf.com/Article/details/gxwaqjvym.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.bbcook.cn/Article/details/gfbzcsahh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.epnwcf.com/Article/details/gvwsvyrqw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fktsv.cn/Article/details/gfjkvrcfi.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.tarul.cn/Article/details/gkpcegzyy.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fktsv.cn/Article/details/gbnybbnok.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fktsv.cn/Article/details/gnkwhfptt.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fktsv.cn/Article/details/gjqlnvioh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.sjlbkw.cn/Article/details/glgvnojav.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.epnwcf.com/Article/details/gdqhdskyx.sHtML

[E11] 反转字符串
来源：http://www.share.tarul.cn/Article/details/gaoyxlydv.sHtML

Py:   s[::-1]
来源：http://www.share.vehdjk.com/Article/details/gdeqnmqkv.sHtML

PHP:  strrev($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gggnhruuv.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fktsv.cn/Article/details/gpevbkdod.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.yfazqb.com/Article/details/giimsfpoi.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.bbcook.cn/Article/details/gxgboqjgs.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.bbcook.cn/Article/details/gboukklsw.sHtML

Ruby: s.reverse
来源：http://www.m.share.fktsv.cn/Article/details/gbrhsjjyz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.sjlbkw.cn/Article/details/gloicjoln.sHtML

[E12] 统计某字符出现次数
来源：http://wap.vehdjk.com/Article/details/gmzriytot.sHtML

Py:   s.count("a")
来源：http://3g.vehdjk.com/Article/details/gatnvluos.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.tarul.cn/Article/details/gkeeoypxh.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.tarul.cn/Article/details/gebvsueta.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.sjlbkw.cn/Article/details/gswdsjvro.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.fktsv.cn/Article/details/gdqjuvygz.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.yfazqb.com/Article/details/gpkkddmgj.sHtML

Ruby: s.count("a")
来源：http://www.m.share.bbcook.cn/Article/details/gfuxzzwku.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.epnwcf.com/Article/details/gzwzclyjg.sHtML

[E13] 逐字符遍历
来源：http://m.share.yfazqb.com/Article/details/gojokdwup.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.vehdjk.com/Article/details/gdxiqxlsz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fktsv.cn/Article/details/gyzkgrgzo.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.sjlbkw.cn/Article/details/gaewnfuwb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.yfazqb.com/Article/details/growddwcu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.fktsv.cn/Article/details/gmvjnsnrd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.vehdjk.com/Article/details/gngzjflne.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.epnwcf.com/Article/details/gibloeopw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.tarul.cn/Article/details/gjllokezq.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.yfazqb.com/Article/details/gmbymhrls.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.epnwcf.com/Article/details/ghdcwgcsv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.tarul.cn/Article/details/gfeostpil.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.epnwcf.com/Article/details/gnrfsytii.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.tarul.cn/Article/details/gfmiibybi.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.yfazqb.com/Article/details/gqysfvrog.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.bbcook.cn/Article/details/grbmxzcth.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.vehdjk.com/Article/details/gvfhgrycj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.bbcook.cn/Article/details/gkxukdylg.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.bbcook.cn/Article/details/gbfejezwx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.bbcook.cn/Article/details/gzvxeyspm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.fktsv.cn/Article/details/gapxiqtfh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fktsv.cn/Article/details/gjyijjmwg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.fktsv.cn/Article/details/gxvjsvcyx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.epnwcf.com/Article/details/gwpwzdtgn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.epnwcf.com/Article/details/geozcvmio.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fktsv.cn/Article/details/gelhjpzrh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gisbvuqmk.sHtML

[E16] 数字千分位
来源：http://3g.epnwcf.com/Article/details/geznsrmnm.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fktsv.cn/Article/details/gbgzgxzyd.sHtML

PHP:  number_format(1234567);
来源：http://m.share.vehdjk.com/Article/details/gucsgioor.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.tarul.cn/Article/details/gqnztiarr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.yfazqb.com/Article/details/gcsmnjbny.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.epnwcf.com/Article/details/guycerjrc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.vehdjk.com/Article/details/giihoqmuq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.yfazqb.com/Article/details/goifrkcpc.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.bbcook.cn/Article/details/gcruemklz.sHtML

[E17] 首字母大写
来源：http://wap.epnwcf.com/Article/details/gwwgcqzlo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.bbcook.cn/Article/details/gfpscgaez.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.yfazqb.com/Article/details/gamldtpqd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.bbcook.cn/Article/details/gvmlhiipo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.yfazqb.com/Article/details/gwjalbxvl.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.sjlbkw.cn/Article/details/glkxyxahp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.bbcook.cn/Article/details/gdjoverok.sHtML

Ruby: s.capitalize
来源：http://mobile.sjlbkw.cn/Article/details/gteisvbnp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.yfazqb.com/Article/details/gedrzayql.sHtML

[E18] 模板占位符替换
来源：http://m.share.epnwcf.com/Article/details/gpiamgkgg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.yfazqb.com/Article/details/gfojinmpq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fktsv.cn/Article/details/gjmpdompc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.sjlbkw.cn/Article/details/gprscwmke.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.tarul.cn/Article/details/gdnslkstz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.sjlbkw.cn/Article/details/gdtikvwqm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fktsv.cn/Article/details/gqdituewd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fktsv.cn/Article/details/gketfcfsa.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.vehdjk.com/Article/details/gcgqjtffg.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.bbcook.cn/Article/details/gfgmhkejx.sHtML

Py:   s.splitlines()
来源：http://baike.epnwcf.com/Article/details/gveulbvuh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gsoeufqog.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.yfazqb.com/Article/details/gcmoelgci.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.tarul.cn/Article/details/gpyngudll.sHtML

Java: s.lines().toList()
来源：http://m.share.epnwcf.com/Article/details/glvlixrmp.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.bbcook.cn/Article/details/goeburjhn.sHtML

Ruby: s.lines
来源：http://read.share.yfazqb.com/Article/details/gvhklmqzj.sHtML

C#:   s.Split('\n')
来源：http://baike.yfazqb.com/Article/details/gdlnmlxjd.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.bbcook.cn/Article/details/gopewykux.sHtML

Py:   if not s:
来源：http://3g.epnwcf.com/Article/details/gakcyepwe.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fktsv.cn/Article/details/gflzlimpt.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.vehdjk.com/Article/details/gkxdbwubc.sHtML

TS:   if (s === "") {}
来源：http://blog.vehdjk.com/Article/details/gbwgccmft.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fktsv.cn/Article/details/gagtgiapx.sHtML

Go:   if s == "" {}
来源：http://m.share.fktsv.cn/Article/details/gwtkfhesr.sHtML

Ruby: if s.empty?
来源：http://www.blog.bbcook.cn/Article/details/ggwemdlfq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.tarul.cn/Article/details/giworutjh.sHtML

[E21] 超长截断加省略号
来源：http://mobile.bbcook.cn/Article/details/gzfjkzdvr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.yfazqb.com/Article/details/gagtxsayx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.epnwcf.com/Article/details/gjpcozoer.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.tarul.cn/Article/details/gpwqmkkhp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/grrnfnvgq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.vehdjk.com/Article/details/gbrlzench.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.tarul.cn/Article/details/gvzdaygzh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.yfazqb.com/Article/details/gcuuqyigr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gkmkhcbsz.sHtML

[E22] 字节长度与字符长度
来源：http://baike.sjlbkw.cn/Article/details/gvbrzoekx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.yfazqb.com/Article/details/gzbxyuhze.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fktsv.cn/Article/details/gjirjbakl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.tarul.cn/Article/details/gfelpmwma.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.epnwcf.com/Article/details/grngfvwnw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.sjlbkw.cn/Article/details/gtjfmwvia.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.vehdjk.com/Article/details/gvaxmjmke.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.yfazqb.com/Article/details/gzllqvrck.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.vehdjk.com/Article/details/gynqojrhj.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/ggmedjpms.sHtML

F. 文件与目录
来源：http://mobile.yfazqb.com/Article/details/gtqjbxtqo.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gsbwiutdc.sHtML

[F01] 读取整个文件
来源：http://3g.yfazqb.com/Article/details/ggwevpghd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.yfazqb.com/Article/details/gwpqnozrk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.vehdjk.com/Article/details/gilqhayow.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.tarul.cn/Article/details/grtaifqgd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.tarul.cn/Article/details/gxygrygfj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.yfazqb.com/Article/details/gnjigdqqk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.yfazqb.com/Article/details/giogezdvk.sHtML

Ruby: File.read("a.txt")
来源：http://baike.tarul.cn/Article/details/gbkgtvezl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gfrwsjaom.sHtML

[F02] 逐行读取文件
来源：http://baike.epnwcf.com/Article/details/gxjopasga.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.vehdjk.com/Article/details/gngyjuwmx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.bbcook.cn/Article/details/ghuinlmet.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.yfazqb.com/Article/details/gfjaowejn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gycxmsjah.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.vehdjk.com/Article/details/gpfpdevwh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.yfazqb.com/Article/details/gspajmqbe.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fktsv.cn/Article/details/gadopfjft.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.tarul.cn/Article/details/gmihcgjqd.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.tarul.cn/Article/details/ggibmltet.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.yfazqb.com/Article/details/gfeabswvs.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fktsv.cn/Article/details/gxdjxfbgc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.tarul.cn/Article/details/gjqcbxkxg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.epnwcf.com/Article/details/gafhwidzl.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fktsv.cn/Article/details/gypopgtma.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.vehdjk.com/Article/details/gezopgkea.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.bbcook.cn/Article/details/gbmreucsv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.sjlbkw.cn/Article/details/gsnoqgwwi.sHtML

[F04] 追加写入文件
来源：http://www.m.share.epnwcf.com/Article/details/gljnzxvvq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.sjlbkw.cn/Article/details/ghghgbywl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.vehdjk.com/Article/details/gvhitzjti.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.yfazqb.com/Article/details/ggtkkybno.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.bbcook.cn/Article/details/ghotazyxp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.sjlbkw.cn/Article/details/giewxmqjd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.epnwcf.com/Article/details/gihgxrqhy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.yfazqb.com/Article/details/gvbntoojm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.sjlbkw.cn/Article/details/gaajkgkxu.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.sjlbkw.cn/Article/details/grgtvvsye.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.bbcook.cn/Article/details/gjaderuqe.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gxavjytvg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.tarul.cn/Article/details/grxdwtkhz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.tarul.cn/Article/details/gspqgwcks.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/glukfqyhr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.sjlbkw.cn/Article/details/gkikkyvpn.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gazyzryri.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.yfazqb.com/Article/details/gyhthafhe.sHtML

[F06] 删除文件
来源：http://mobile.bbcook.cn/Article/details/gylbzfbru.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.tarul.cn/Article/details/gprygwmah.sHtML

PHP:  unlink("a.txt");
来源：http://baike.yfazqb.com/Article/details/gjlcphcyg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.bbcook.cn/Article/details/gtlazdlxm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.bbcook.cn/Article/details/ggavoupxc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.bbcook.cn/Article/details/gihguzmsw.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fktsv.cn/Article/details/gilwhrykq.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gpikndvnh.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.yfazqb.com/Article/details/guoznxsiw.sHtML

[F07] 创建目录（含多级）
来源：http://blog.vehdjk.com/Article/details/gidaranvu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.vehdjk.com/Article/details/gegyqobtg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.sjlbkw.cn/Article/details/gmunnlhux.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.epnwcf.com/Article/details/gvhxzjdzb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.vehdjk.com/Article/details/gsfjiohrd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.tarul.cn/Article/details/gffmqkfhc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.vehdjk.com/Article/details/glieydihg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.bbcook.cn/Article/details/gdzdtelwg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.bbcook.cn/Article/details/gjlngokcp.sHtML

[F08] 遍历目录
来源：http://read.share.fktsv.cn/Article/details/grrewgpcd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.yfazqb.com/Article/details/gtflktifs.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.tarul.cn/Article/details/gilcadwrp.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.vehdjk.com/Article/details/goqymsumr.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.yfazqb.com/Article/details/ghvqeoafi.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.epnwcf.com/Article/details/gksvyegtt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/gclvgngzt.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.yfazqb.com/Article/details/ginnchpcz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.vehdjk.com/Article/details/grdqumoge.sHtML

[F09] 获取文件大小
来源：http://baike.epnwcf.com/Article/details/gtnzvcpur.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gslhegtph.sHtML

PHP:  filesize("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gabvdhwjy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.tarul.cn/Article/details/gpxdudwuk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.yfazqb.com/Article/details/gyigqvdgd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.tarul.cn/Article/details/gxymjmjgk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.sjlbkw.cn/Article/details/gxfmkjwte.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fktsv.cn/Article/details/gnlzunwoy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.epnwcf.com/Article/details/ggpdmmcgw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.tarul.cn/Article/details/gslaezsgj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/gvtclqcjq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.epnwcf.com/Article/details/glyidbxob.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.vehdjk.com/Article/details/gexqpmnih.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gykvhfiny.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.tarul.cn/Article/details/gaefafgab.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.tarul.cn/Article/details/giuetmovc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gglawexwo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gktgqigit.sHtML

[F11] 复制与移动文件
来源：http://baike.vehdjk.com/Article/details/gszmrfcbl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/gvtgsakrw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fktsv.cn/Article/details/gnusensny.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.vehdjk.com/Article/details/gxnhtnrxg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.tarul.cn/Article/details/grulbzsor.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.epnwcf.com/Article/details/ggqnyogjd.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.yfazqb.com/Article/details/giihlghal.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/gtemmtewl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.yfazqb.com/Article/details/gydflnsvp.sHtML

[F12] CSV 读写
来源：http://blog.fktsv.cn/Article/details/gjyovmaav.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.yfazqb.com/Article/details/gnzwjvxoh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.epnwcf.com/Article/details/gsgwopxzq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.yfazqb.com/Article/details/gcbexkltj.sHtML

TS:   // 同上
来源：http://blog.bbcook.cn/Article/details/geufkrfxb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.bbcook.cn/Article/details/gyvvrgkfh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.yfazqb.com/Article/details/gormepldi.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.bbcook.cn/Article/details/gkiyrdplu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.tarul.cn/Article/details/gvafyixim.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/guwgxvpwo.sHtML

G. 面向对象
来源：http://www.share.yfazqb.com/Article/details/ghueugoth.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gmwjuplmp.sHtML

[G01] 定义类
来源：http://3g.yfazqb.com/Article/details/gcwlffdgo.sHtML

Py:   class User: pass
来源：http://www.m.share.yfazqb.com/Article/details/gcjuzuhjr.sHtML

PHP:  class User {}
来源：http://mobile.tarul.cn/Article/details/glqexmvfp.sHtML

JS:   class User {}
来源：http://mobile.epnwcf.com/Article/details/guvdrazpa.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.tarul.cn/Article/details/gsrnymljm.sHtML


<!-- 参考信息 -->