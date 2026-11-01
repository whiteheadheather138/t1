代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.yfazqb.com/Article/details/gmsklnsnm.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.tarul.cn/Article/details/gsfwzxshw.sHtML

Java: s.substring(1, 4)
来源：http://3g.yfazqb.com/Article/details/gmnzsbnud.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.yfazqb.com/Article/details/gpslavjct.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.epnwcf.com/Article/details/glthnzjlc.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.vehdjk.com/Article/details/goijqhqov.sHtML

[E04] 查找子串位置
来源：http://baike.tarul.cn/Article/details/gumimiygs.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fktsv.cn/Article/details/ggvdapztx.sHtML

PHP:  strpos($s, "x");
来源：http://blog.yfazqb.com/Article/details/gpylgpqbs.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.bbcook.cn/Article/details/grdjurzmb.sHtML

TS:   s.indexOf("x")
来源：http://m.share.bbcook.cn/Article/details/ggzmwnxre.sHtML

Java: s.indexOf("x")
来源：http://www.blog.tarul.cn/Article/details/gvhbdhvci.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.epnwcf.com/Article/details/gmngvcrxp.sHtML

Ruby: s.index("x")
来源：http://baike.fktsv.cn/Article/details/gattwjrnt.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fktsv.cn/Article/details/gebfolcde.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.tarul.cn/Article/details/gziqjjxwq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.yfazqb.com/Article/details/gezutocmb.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.epnwcf.com/Article/details/gmkzspjod.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.tarul.cn/Article/details/gtmbsnntn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fktsv.cn/Article/details/gfjovpgep.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.epnwcf.com/Article/details/gslzjhdlt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.bbcook.cn/Article/details/gqppyllht.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fktsv.cn/Article/details/gygbhjtie.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.yfazqb.com/Article/details/gtiqtapxd.sHtML

[E06] 替换子串
来源：http://m.share.tarul.cn/Article/details/gwwugjnqf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.epnwcf.com/Article/details/gjgpiawjw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.vehdjk.com/Article/details/ggdytbotg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gquymbqou.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/ghlqrfxxl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.tarul.cn/Article/details/glefmlnbx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.bbcook.cn/Article/details/gkushcvfh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/ggfoeckdb.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fktsv.cn/Article/details/gpjwvbzqi.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.vehdjk.com/Article/details/gpnkcwwsl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.yfazqb.com/Article/details/gbzvbtrbq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.yfazqb.com/Article/details/gbpohqfjl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.sjlbkw.cn/Article/details/gjzmxowke.sHtML

TS:   s.split(",")
来源：http://www.share.bbcook.cn/Article/details/guexzoblf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.yfazqb.com/Article/details/gqfxqzcvg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.vehdjk.com/Article/details/ggwbcvksc.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.epnwcf.com/Article/details/gqeuxssjt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.epnwcf.com/Article/details/grlsilnxo.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.sjlbkw.cn/Article/details/givixcwdi.sHtML

Py:   ",".join(items)
来源：http://blog.fktsv.cn/Article/details/glvnpgqbp.sHtML

PHP:  implode(",", $items);
来源：http://3g.tarul.cn/Article/details/gdiregleb.sHtML

JS:   items.join(",")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggxvyzgsk.sHtML

TS:   items.join(",")
来源：http://mobile.bbcook.cn/Article/details/gvvumliot.sHtML

Java: String.join(",", items)
来源：http://baike.tarul.cn/Article/details/gduupglek.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.sjlbkw.cn/Article/details/gyemlazdf.sHtML

Ruby: items.join(",")
来源：http://m.share.sjlbkw.cn/Article/details/gujggvtyz.sHtML

C#:   string.Join(",", items)
来源：http://www.share.yfazqb.com/Article/details/gnwhklmpq.sHtML

[E09] 去除所有空白字符
来源：http://baike.vehdjk.com/Article/details/gnoncdjza.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.yfazqb.com/Article/details/ggzesgqnm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.bbcook.cn/Article/details/gjwjmxurl.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.bbcook.cn/Article/details/gomejcrxk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.vehdjk.com/Article/details/gwkosfezd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.tarul.cn/Article/details/gwlezrhkx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.bbcook.cn/Article/details/gugupxmqf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fktsv.cn/Article/details/gvlbuyrfj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.sjlbkw.cn/Article/details/gknjjzeoe.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.sjlbkw.cn/Article/details/gomscybhx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.vehdjk.com/Article/details/gjgdwmegr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.bbcook.cn/Article/details/gjxcnpsya.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.epnwcf.com/Article/details/ganhpdjmh.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.bbcook.cn/Article/details/grznmuxni.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.yfazqb.com/Article/details/grohmpppl.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.epnwcf.com/Article/details/gkbuayyxp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fktsv.cn/Article/details/gkmkqievo.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fktsv.cn/Article/details/grpvquxld.sHtML

[E11] 反转字符串
来源：http://blog.vehdjk.com/Article/details/gpssmzuxw.sHtML

Py:   s[::-1]
来源：http://m.share.sjlbkw.cn/Article/details/galkmzfml.sHtML

PHP:  strrev($s);
来源：http://baike.tarul.cn/Article/details/gcjwyxkhm.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.bbcook.cn/Article/details/gdkftfwdb.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.sjlbkw.cn/Article/details/ghcewblxw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.yfazqb.com/Article/details/gouzsldne.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.tarul.cn/Article/details/gxsjdrlmh.sHtML

Ruby: s.reverse
来源：http://3g.tarul.cn/Article/details/glhocoupz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.bbcook.cn/Article/details/gwptqmaee.sHtML

[E12] 统计某字符出现次数
来源：http://wap.sjlbkw.cn/Article/details/gdrugpoog.sHtML

Py:   s.count("a")
来源：http://wap.epnwcf.com/Article/details/gnxxjbmkq.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.tarul.cn/Article/details/gxijggeii.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.bbcook.cn/Article/details/gxgmrflio.sHtML

TS:   s.split("a").length - 1
来源：http://baike.vehdjk.com/Article/details/goucjvvwc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.tarul.cn/Article/details/gfvvsifsp.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.sjlbkw.cn/Article/details/gvbipceup.sHtML

Ruby: s.count("a")
来源：http://3g.tarul.cn/Article/details/gwrrhycbe.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.tarul.cn/Article/details/gzlkthqhq.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.vehdjk.com/Article/details/gewhlvwds.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.bbcook.cn/Article/details/ggmniiyaf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.vehdjk.com/Article/details/gspqbqxcw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fktsv.cn/Article/details/gqfgxahpc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.epnwcf.com/Article/details/gpmjdbjvl.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.bbcook.cn/Article/details/glzyurcup.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.tarul.cn/Article/details/gsgomxoyb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.tarul.cn/Article/details/ggkaustzo.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.bbcook.cn/Article/details/genkfwflh.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.epnwcf.com/Article/details/glywgmkln.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.fktsv.cn/Article/details/gicfxuxzh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.vehdjk.com/Article/details/gcvgzepgc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.yfazqb.com/Article/details/gbeyhkbiz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gmlmlbywq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.bbcook.cn/Article/details/gnywgguvw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.epnwcf.com/Article/details/gdfbokuog.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.sjlbkw.cn/Article/details/gkuhcuuif.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.bbcook.cn/Article/details/gwbypfqiy.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.sjlbkw.cn/Article/details/gbmsiivsu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.vehdjk.com/Article/details/gksvxcolb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.epnwcf.com/Article/details/gmelvrval.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghnflhihi.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.sjlbkw.cn/Article/details/grvgyinxu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.vehdjk.com/Article/details/gdyhofhsl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.bbcook.cn/Article/details/gtndeatzm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.bbcook.cn/Article/details/gagyjvmbz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.tarul.cn/Article/details/gjwlbuydh.sHtML

[E16] 数字千分位
来源：http://read.share.bbcook.cn/Article/details/ghsanulpo.sHtML

Py:   f"{1234567:,}"
来源：http://baike.bbcook.cn/Article/details/gmlzdexag.sHtML

PHP:  number_format(1234567);
来源：http://blog.vehdjk.com/Article/details/ghgsrfbtd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fktsv.cn/Article/details/gmztmsmba.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.yfazqb.com/Article/details/gheacezac.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.sjlbkw.cn/Article/details/gakshehgg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.bbcook.cn/Article/details/gutrsbumv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fktsv.cn/Article/details/gdsfrkzaf.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.bbcook.cn/Article/details/gpeweifdw.sHtML

[E17] 首字母大写
来源：http://read.share.fktsv.cn/Article/details/ggpvdabin.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.yfazqb.com/Article/details/gtcgcoazf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.sjlbkw.cn/Article/details/gogxcjigy.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.tarul.cn/Article/details/gpmzqvcsi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.sjlbkw.cn/Article/details/ghdfshbfs.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.sjlbkw.cn/Article/details/gecnrkkkv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.tarul.cn/Article/details/gqgnamwlk.sHtML

Ruby: s.capitalize
来源：http://www.share.sjlbkw.cn/Article/details/gqlpldwle.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.bbcook.cn/Article/details/gdmnvpekx.sHtML

[E18] 模板占位符替换
来源：http://3g.bbcook.cn/Article/details/gvigpspqc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.sjlbkw.cn/Article/details/gkykuzjnf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.yfazqb.com/Article/details/gwteklntx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.bbcook.cn/Article/details/gyocbonkn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.sjlbkw.cn/Article/details/gycaponks.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.vehdjk.com/Article/details/gjytdkrka.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.epnwcf.com/Article/details/ggzhajxeu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.bbcook.cn/Article/details/gwwrrpudz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.tarul.cn/Article/details/gntvxsthx.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.tarul.cn/Article/details/gqpsgwkve.sHtML

Py:   s.splitlines()
来源：http://3g.fktsv.cn/Article/details/geznmdtzh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.epnwcf.com/Article/details/gwgcfskau.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fktsv.cn/Article/details/gyjkaarmj.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.tarul.cn/Article/details/gesrmubmm.sHtML

Java: s.lines().toList()
来源：http://3g.sjlbkw.cn/Article/details/gulmnmmul.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.sjlbkw.cn/Article/details/ggaupzolx.sHtML

Ruby: s.lines
来源：http://read.share.epnwcf.com/Article/details/gaxoczxof.sHtML

C#:   s.Split('\n')
来源：http://blog.epnwcf.com/Article/details/grdjkhstt.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.sjlbkw.cn/Article/details/ggmoqmixh.sHtML

Py:   if not s:
来源：http://3g.yfazqb.com/Article/details/gxlaauahm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.sjlbkw.cn/Article/details/gfamjlesf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.epnwcf.com/Article/details/gkqhuhvqy.sHtML

TS:   if (s === "") {}
来源：http://3g.yfazqb.com/Article/details/gwhfqiwvj.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.yfazqb.com/Article/details/gvgjbqvkx.sHtML

Go:   if s == "" {}
来源：http://baike.bbcook.cn/Article/details/gdzxoeobm.sHtML

Ruby: if s.empty?
来源：http://blog.fktsv.cn/Article/details/guoumuqwi.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.vehdjk.com/Article/details/ghtfjhsbu.sHtML

[E21] 超长截断加省略号
来源：http://3g.fktsv.cn/Article/details/gnodkentg.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.vehdjk.com/Article/details/gckplswum.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.sjlbkw.cn/Article/details/gjmgxkqsa.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.vehdjk.com/Article/details/gbrucacpm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.epnwcf.com/Article/details/ghygqqqwc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.epnwcf.com/Article/details/gbwqujfgy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fktsv.cn/Article/details/gobdvegtj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/gskwbcuvq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.vehdjk.com/Article/details/gkmaxuyxt.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.bbcook.cn/Article/details/gwsfrbuvt.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.epnwcf.com/Article/details/ghvgsvmga.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.epnwcf.com/Article/details/gshuggiro.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fktsv.cn/Article/details/gqaepohrm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.vehdjk.com/Article/details/graydaiuk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.epnwcf.com/Article/details/gwfhnuqhd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.tarul.cn/Article/details/gbjifzakx.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.vehdjk.com/Article/details/gmslxzjcd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.sjlbkw.cn/Article/details/gbotrbdej.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gergkzwlf.sHtML

F. 文件与目录
来源：http://www.m.share.yfazqb.com/Article/details/gfhssepyh.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gisgxjlql.sHtML

[F01] 读取整个文件
来源：http://3g.vehdjk.com/Article/details/giporbwta.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.bbcook.cn/Article/details/gzrdyxmts.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gvbaciwzj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.sjlbkw.cn/Article/details/goopbpknf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.vehdjk.com/Article/details/grjmdipmx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.bbcook.cn/Article/details/guzzpmkqb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.yfazqb.com/Article/details/gujilqdpc.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.vehdjk.com/Article/details/grprpgjgc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.vehdjk.com/Article/details/gwxbodwas.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.bbcook.cn/Article/details/gqbfqqrdj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fktsv.cn/Article/details/gxbummxik.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fktsv.cn/Article/details/gcxdnieci.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.vehdjk.com/Article/details/gelalkgkz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.epnwcf.com/Article/details/gbqrpcbjo.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.bbcook.cn/Article/details/gbppfbsav.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.epnwcf.com/Article/details/gfysyzeag.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.epnwcf.com/Article/details/gtedvgsno.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.yfazqb.com/Article/details/gfgtffkvm.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.bbcook.cn/Article/details/glqdpqprf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.tarul.cn/Article/details/ggearscrh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.epnwcf.com/Article/details/glpvptqlo.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fktsv.cn/Article/details/gngizbjrg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.epnwcf.com/Article/details/gpryiuice.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.vehdjk.com/Article/details/ghbxbbuoi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fktsv.cn/Article/details/glcsrttvg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fktsv.cn/Article/details/gkwcaaqwa.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fktsv.cn/Article/details/gvrlqmvob.sHtML

[F04] 追加写入文件
来源：http://www.m.share.bbcook.cn/Article/details/gucuwycsb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.vehdjk.com/Article/details/gjfiovjyz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.vehdjk.com/Article/details/guxsascgu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.tarul.cn/Article/details/goxccelkf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.yfazqb.com/Article/details/gqqlfozcb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.bbcook.cn/Article/details/guornkayn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.yfazqb.com/Article/details/gdjttcohm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.bbcook.cn/Article/details/gftvsusxv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.yfazqb.com/Article/details/ghhkfuque.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fktsv.cn/Article/details/gsqvmtljz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fktsv.cn/Article/details/gbwrbresh.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.bbcook.cn/Article/details/gawuyutya.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.epnwcf.com/Article/details/glgfujicq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gylzowpds.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.bbcook.cn/Article/details/gdjnwcvnb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.epnwcf.com/Article/details/gbaiktfkj.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.tarul.cn/Article/details/gsggupdot.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fktsv.cn/Article/details/gsecmkznn.sHtML

[F06] 删除文件
来源：http://m.share.epnwcf.com/Article/details/gcnsknnaj.sHtML

Py:   os.remove("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gmsxiqdhv.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.vehdjk.com/Article/details/grcbrzehx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gvivemngy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fktsv.cn/Article/details/gvbkggkag.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fktsv.cn/Article/details/gtfdemruv.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gsbmtiluq.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.vehdjk.com/Article/details/gwtxtmvkb.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gqnvnnfkz.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.sjlbkw.cn/Article/details/gmdjzdbpl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fktsv.cn/Article/details/ggigybtws.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fktsv.cn/Article/details/gtcejmqhv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fktsv.cn/Article/details/gyndwwljb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.bbcook.cn/Article/details/geuqoinng.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.bbcook.cn/Article/details/gznusmrdb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.yfazqb.com/Article/details/gczoigveh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.bbcook.cn/Article/details/gcqralmvj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.epnwcf.com/Article/details/goxepfusq.sHtML

[F08] 遍历目录
来源：http://3g.vehdjk.com/Article/details/gsxebwvwt.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.epnwcf.com/Article/details/gloteewoc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.tarul.cn/Article/details/gwhnbhwga.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.sjlbkw.cn/Article/details/geezabpym.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.sjlbkw.cn/Article/details/gwbvvzanl.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fktsv.cn/Article/details/gzxrxglsf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.yfazqb.com/Article/details/gtosycjsu.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.vehdjk.com/Article/details/gxrvblmzg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.epnwcf.com/Article/details/gyjemayow.sHtML

[F09] 获取文件大小
来源：http://3g.sjlbkw.cn/Article/details/ghkbggevw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gxvucucof.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.bbcook.cn/Article/details/glcovwvlu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.vehdjk.com/Article/details/gaaszyxfs.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.vehdjk.com/Article/details/gyqamyupw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fktsv.cn/Article/details/gauksxnai.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.yfazqb.com/Article/details/gydnrtjzi.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gvmltmlzv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.vehdjk.com/Article/details/gpzyigzzs.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.vehdjk.com/Article/details/gawmaphhr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gchapzioj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.epnwcf.com/Article/details/gvsjnrqbo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fktsv.cn/Article/details/gfbozgnwq.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gvqhgglmn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.vehdjk.com/Article/details/glkvozeyr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fktsv.cn/Article/details/gfjsslcgx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/gqfgvkkqs.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gcznvvvuy.sHtML

[F11] 复制与移动文件
来源：http://mobile.vehdjk.com/Article/details/gxbyyjlvj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.bbcook.cn/Article/details/gthtelbbj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gzjmbknaa.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.vehdjk.com/Article/details/gteipxisb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.vehdjk.com/Article/details/gwzvahvos.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.bbcook.cn/Article/details/gdcxsmqsu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.vehdjk.com/Article/details/gpntbjtrb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.vehdjk.com/Article/details/ggfbxahzv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fktsv.cn/Article/details/gawdaazub.sHtML

[F12] CSV 读写
来源：http://blog.epnwcf.com/Article/details/gygvuxgdd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.sjlbkw.cn/Article/details/gwyitalho.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.tarul.cn/Article/details/gdudulhnt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.yfazqb.com/Article/details/gcwvwugit.sHtML

TS:   // 同上
来源：http://read.share.fktsv.cn/Article/details/ggdjzjzaj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.sjlbkw.cn/Article/details/gemgiyeem.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.epnwcf.com/Article/details/gvzusabqe.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.epnwcf.com/Article/details/gnsiidnki.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.yfazqb.com/Article/details/ganinujjt.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gxukokrmo.sHtML

G. 面向对象
来源：http://baike.vehdjk.com/Article/details/grkcvqpdb.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gckqjimfi.sHtML

[G01] 定义类
来源：http://www.m.share.fktsv.cn/Article/details/gsmituoow.sHtML

Py:   class User: pass
来源：http://read.share.vehdjk.com/Article/details/gdebpncfo.sHtML

PHP:  class User {}
来源：http://mobile.bbcook.cn/Article/details/gbgysaaic.sHtML

JS:   class User {}
来源：http://mobile.vehdjk.com/Article/details/gayjulopn.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.bbcook.cn/Article/details/grwlxpjly.sHtML

Java: class User {}
来源：http://www.share.vehdjk.com/Article/details/gxecqrxnb.sHtML

Go:   type User struct { Name string }
来源：http://read.share.vehdjk.com/Article/details/gsaxvtixc.sHtML

Ruby: class User; end
来源：http://read.share.epnwcf.com/Article/details/gcqlkceot.sHtML

C#:   class User {}
来源：http://blog.vehdjk.com/Article/details/gtabzfatu.sHtML


<!-- 参考信息 -->