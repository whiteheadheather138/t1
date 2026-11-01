代发 wailian999

Go:   strings.Index(s, "x")
来源：http://www.share.sjlbkw.cn/Article/details/gxvzxsmcq.sHtML

Ruby: s.index("x")
来源：http://m.share.yfazqb.com/Article/details/ghqzsbsck.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.vehdjk.com/Article/details/gwmiehiee.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.yfazqb.com/Article/details/gyvbtnfts.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.epnwcf.com/Article/details/gfpeovstp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.vehdjk.com/Article/details/gzmdcolmo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.epnwcf.com/Article/details/grgjvgzej.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.tarul.cn/Article/details/gjfwlfkdv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.vehdjk.com/Article/details/gaeylpyzr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fktsv.cn/Article/details/gdwkofmkh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.bbcook.cn/Article/details/glhbrwktt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.yfazqb.com/Article/details/golmvlodd.sHtML

[E06] 替换子串
来源：http://www.blog.bbcook.cn/Article/details/gcfuabitg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.bbcook.cn/Article/details/gnicwofvx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.tarul.cn/Article/details/gbwpjomps.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gtvxictiw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.bbcook.cn/Article/details/gehykifif.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.vehdjk.com/Article/details/giecncysm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.yfazqb.com/Article/details/grzhvaafn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.sjlbkw.cn/Article/details/gfwqapupd.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.tarul.cn/Article/details/gzgukjdtn.sHtML

[E07] 按分隔符拆分
来源：http://read.share.epnwcf.com/Article/details/gisfjuztq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.vehdjk.com/Article/details/gvnllbpyj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.fktsv.cn/Article/details/gcywjwtpq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.yfazqb.com/Article/details/gyqgttjfx.sHtML

TS:   s.split(",")
来源：http://baike.fktsv.cn/Article/details/gczkooswa.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.epnwcf.com/Article/details/gwmoceagi.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.tarul.cn/Article/details/gxcjmgeuy.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.bbcook.cn/Article/details/gfzwgpiaf.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.vehdjk.com/Article/details/giydtaipi.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.bbcook.cn/Article/details/gybiqogyw.sHtML

Py:   ",".join(items)
来源：http://baike.sjlbkw.cn/Article/details/getunrbaq.sHtML

PHP:  implode(",", $items);
来源：http://www.share.yfazqb.com/Article/details/griptlpgs.sHtML

JS:   items.join(",")
来源：http://baike.fktsv.cn/Article/details/gtkffahvd.sHtML

TS:   items.join(",")
来源：http://3g.bbcook.cn/Article/details/grqvnivxf.sHtML

Java: String.join(",", items)
来源：http://baike.sjlbkw.cn/Article/details/gayisswht.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fktsv.cn/Article/details/gxhbgjrib.sHtML

Ruby: items.join(",")
来源：http://www.blog.vehdjk.com/Article/details/gdfhqhssi.sHtML

C#:   string.Join(",", items)
来源：http://baike.fktsv.cn/Article/details/gyantztjd.sHtML

[E09] 去除所有空白字符
来源：http://m.share.epnwcf.com/Article/details/grmayrauz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.sjlbkw.cn/Article/details/gjyhmceuf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.epnwcf.com/Article/details/gyucfhiut.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.yfazqb.com/Article/details/gtwvkxbtv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.vehdjk.com/Article/details/gwdsctcgy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.epnwcf.com/Article/details/gtnagvjby.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.bbcook.cn/Article/details/gsiyyelcw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.epnwcf.com/Article/details/gqgjlhijn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.yfazqb.com/Article/details/gnjsyfhht.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.tarul.cn/Article/details/gmzyatwkv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.bbcook.cn/Article/details/gvfqzmytf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.yfazqb.com/Article/details/gwlwppkrm.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.sjlbkw.cn/Article/details/gdrdptndc.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fktsv.cn/Article/details/gjfzuujuk.sHtML

Java: String.format("%03d", 7)
来源：http://wap.tarul.cn/Article/details/gjebtflfn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.tarul.cn/Article/details/gepxhnjvx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.bbcook.cn/Article/details/gzwggnnyy.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.sjlbkw.cn/Article/details/gjqpkmakq.sHtML

[E11] 反转字符串
来源：http://baike.bbcook.cn/Article/details/gvwclwiex.sHtML

Py:   s[::-1]
来源：http://wap.tarul.cn/Article/details/gqijjhvpq.sHtML

PHP:  strrev($s);
来源：http://www.blog.bbcook.cn/Article/details/gkwklczge.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.tarul.cn/Article/details/gowpbjpqz.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fktsv.cn/Article/details/gudcjbcnl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.vehdjk.com/Article/details/gyvmfvojg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.bbcook.cn/Article/details/gvcenovxy.sHtML

Ruby: s.reverse
来源：http://www.share.yfazqb.com/Article/details/gueggtjgt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.vehdjk.com/Article/details/gegdlybfv.sHtML

[E12] 统计某字符出现次数
来源：http://wap.tarul.cn/Article/details/giyidwxqr.sHtML

Py:   s.count("a")
来源：http://m.share.yfazqb.com/Article/details/gjwfmkukt.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.vehdjk.com/Article/details/guojlqpqa.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fktsv.cn/Article/details/gdzqcxfkr.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.sjlbkw.cn/Article/details/gqsouiwzw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fktsv.cn/Article/details/grvckcest.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fktsv.cn/Article/details/gjqvqpquy.sHtML

Ruby: s.count("a")
来源：http://baike.yfazqb.com/Article/details/gahnqyooq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.vehdjk.com/Article/details/gvewhbsuc.sHtML

[E13] 逐字符遍历
来源：http://m.share.fktsv.cn/Article/details/gdbdlrilr.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.vehdjk.com/Article/details/gaaoalhsx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.bbcook.cn/Article/details/gksvkycew.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.tarul.cn/Article/details/guqtpmmam.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fktsv.cn/Article/details/gdpjnmbwe.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.epnwcf.com/Article/details/glmzgcfph.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.epnwcf.com/Article/details/gsqulwlwi.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.epnwcf.com/Article/details/grgzajtmu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.tarul.cn/Article/details/gtdrcizly.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.vehdjk.com/Article/details/gxakahbvn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.bbcook.cn/Article/details/gfkyglaou.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.vehdjk.com/Article/details/gftbgobcc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.vehdjk.com/Article/details/gznzqfyni.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.tarul.cn/Article/details/gdacwzptq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.epnwcf.com/Article/details/gydkbtxap.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.bbcook.cn/Article/details/gqhftccbe.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.epnwcf.com/Article/details/gcofkeyen.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.bbcook.cn/Article/details/ghrakcqch.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.bbcook.cn/Article/details/gkosubgzb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.vehdjk.com/Article/details/gpfzbonci.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.yfazqb.com/Article/details/gbfnmchmo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqxvqxqbk.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.sjlbkw.cn/Article/details/gvaglnqrz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.bbcook.cn/Article/details/gbgpwnksy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.epnwcf.com/Article/details/gkrmkcfhh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.bbcook.cn/Article/details/gkbmmhgsa.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.epnwcf.com/Article/details/gyoohjazp.sHtML

[E16] 数字千分位
来源：http://3g.vehdjk.com/Article/details/gqjkmlnjb.sHtML

Py:   f"{1234567:,}"
来源：http://blog.epnwcf.com/Article/details/gplxnzaco.sHtML

PHP:  number_format(1234567);
来源：http://m.share.sjlbkw.cn/Article/details/gnuvosyqn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.tarul.cn/Article/details/gwygdyqvw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fktsv.cn/Article/details/gnkwjofdm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.vehdjk.com/Article/details/grhxulgrx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.fktsv.cn/Article/details/gwginxehm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.bbcook.cn/Article/details/ggxghcjnm.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.tarul.cn/Article/details/grjgqawxa.sHtML

[E17] 首字母大写
来源：http://3g.bbcook.cn/Article/details/ggwejfbui.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.bbcook.cn/Article/details/gsgnvwmbe.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.vehdjk.com/Article/details/ggdyaqrjl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.bbcook.cn/Article/details/gfyvhlxnr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.bbcook.cn/Article/details/gyscwfvuf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.yfazqb.com/Article/details/grpjryqfr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.vehdjk.com/Article/details/gjospfkzb.sHtML

Ruby: s.capitalize
来源：http://baike.fktsv.cn/Article/details/gtzpjyzzq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fktsv.cn/Article/details/ghxqkmlwu.sHtML

[E18] 模板占位符替换
来源：http://www.share.sjlbkw.cn/Article/details/gjknvpkyq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fktsv.cn/Article/details/gochjryyr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.bbcook.cn/Article/details/gclhedvna.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.vehdjk.com/Article/details/gfkdvtjkg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.bbcook.cn/Article/details/gfqtvfzhe.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fktsv.cn/Article/details/gcluglxkn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.tarul.cn/Article/details/guwxrufpb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.sjlbkw.cn/Article/details/gdakdduvb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.tarul.cn/Article/details/gwnobksfe.sHtML

[E19] 多行文本按行拆分
来源：http://wap.tarul.cn/Article/details/giybkwapo.sHtML

Py:   s.splitlines()
来源：http://www.blog.tarul.cn/Article/details/gjbtqxecy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.epnwcf.com/Article/details/gfyaylwsi.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.sjlbkw.cn/Article/details/gicezvoeu.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.epnwcf.com/Article/details/gjasmxggm.sHtML

Java: s.lines().toList()
来源：http://www.share.fktsv.cn/Article/details/gctrvfsda.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.yfazqb.com/Article/details/grqkgmdrq.sHtML

Ruby: s.lines
来源：http://wap.vehdjk.com/Article/details/greqxkvzk.sHtML

C#:   s.Split('\n')
来源：http://read.share.epnwcf.com/Article/details/gumaixuux.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.tarul.cn/Article/details/gnayexgil.sHtML

Py:   if not s:
来源：http://3g.epnwcf.com/Article/details/gtqbepjyl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.vehdjk.com/Article/details/gikmnwvoc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gdrvnldiv.sHtML

TS:   if (s === "") {}
来源：http://read.share.epnwcf.com/Article/details/gbowjjymi.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.bbcook.cn/Article/details/gnccqvigh.sHtML

Go:   if s == "" {}
来源：http://blog.sjlbkw.cn/Article/details/gyuuyoirl.sHtML

Ruby: if s.empty?
来源：http://wap.vehdjk.com/Article/details/gezpbozkx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.sjlbkw.cn/Article/details/gxfwlcxsl.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.sjlbkw.cn/Article/details/gnpxqliyv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.yfazqb.com/Article/details/gvdgfshit.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fktsv.cn/Article/details/guscmyrjo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.vehdjk.com/Article/details/gitgncrhu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.epnwcf.com/Article/details/gkbtuwuxu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.bbcook.cn/Article/details/gadwkztac.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.vehdjk.com/Article/details/gwumzwcha.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.tarul.cn/Article/details/geviausud.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/gkzlcodrx.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fktsv.cn/Article/details/gobarpjqj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.tarul.cn/Article/details/gngsodujp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fktsv.cn/Article/details/gwsksdhpw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.yfazqb.com/Article/details/gjeaaypbl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.yfazqb.com/Article/details/glwekveuo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fktsv.cn/Article/details/gurfkymqw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.bbcook.cn/Article/details/glisgvqsc.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fktsv.cn/Article/details/ghxzrygqd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.sjlbkw.cn/Article/details/gcdtuevmo.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gvudurlsm.sHtML

F. 文件与目录
来源：http://m.share.epnwcf.com/Article/details/glyatlzxf.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gazfdeatj.sHtML

[F01] 读取整个文件
来源：http://www.share.fktsv.cn/Article/details/gpecfzxta.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.vehdjk.com/Article/details/gyqxkyjcx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.yfazqb.com/Article/details/gaguemhwk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.epnwcf.com/Article/details/gkntkjmfa.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.epnwcf.com/Article/details/gghddrezu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.tarul.cn/Article/details/ggeqyerak.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.bbcook.cn/Article/details/geotxfyzu.sHtML

Ruby: File.read("a.txt")
来源：http://3g.epnwcf.com/Article/details/grexqesuh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.epnwcf.com/Article/details/ggnkugddl.sHtML

[F02] 逐行读取文件
来源：http://mobile.yfazqb.com/Article/details/gdzcccxdb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fktsv.cn/Article/details/gtxhiwmxu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.vehdjk.com/Article/details/gpfqntoev.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.sjlbkw.cn/Article/details/giaommhxj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.tarul.cn/Article/details/gpjoeiqna.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fktsv.cn/Article/details/gpwujmtlq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.sjlbkw.cn/Article/details/gfcvtkpmg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.sjlbkw.cn/Article/details/glytzgsxy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.tarul.cn/Article/details/goofhjuup.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.vehdjk.com/Article/details/gqaiclrcn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.epnwcf.com/Article/details/gzdhtzkje.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.sjlbkw.cn/Article/details/gtqgluwvk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.yfazqb.com/Article/details/gmhkeybww.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.bbcook.cn/Article/details/gpwqhwycf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.bbcook.cn/Article/details/gfzmmhbwo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.tarul.cn/Article/details/ghcxucfdm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.tarul.cn/Article/details/gpxktchqi.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.tarul.cn/Article/details/glumjyazl.sHtML

[F04] 追加写入文件
来源：http://read.share.bbcook.cn/Article/details/gurfzwylt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.epnwcf.com/Article/details/gmaeyxlnj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.sjlbkw.cn/Article/details/gkvddyslh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.sjlbkw.cn/Article/details/gvmdvlvhy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.tarul.cn/Article/details/gdpsguaut.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.vehdjk.com/Article/details/gjowuxggt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.yfazqb.com/Article/details/gfkrpspxz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.vehdjk.com/Article/details/ggreqjigw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fktsv.cn/Article/details/gucadrodq.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.tarul.cn/Article/details/gqmusgdjh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.sjlbkw.cn/Article/details/grmdnytkj.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gfvkbtayi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gaxxcdcbk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gzgrdiyur.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fktsv.cn/Article/details/gszanmweo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.yfazqb.com/Article/details/grxubohjb.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gqvpliagw.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gzigphsvp.sHtML

[F06] 删除文件
来源：http://wap.vehdjk.com/Article/details/gxxigispm.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gfojalnpk.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.bbcook.cn/Article/details/gshrojnde.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.bbcook.cn/Article/details/gqlvjaqil.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gucigmsvo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/gdfmzkmjc.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/glpaqohjh.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gulwkxkoa.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/godwwxcuz.sHtML

[F07] 创建目录（含多级）
来源：http://baike.sjlbkw.cn/Article/details/geuywnzyr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.bbcook.cn/Article/details/gtfdagfcl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.yfazqb.com/Article/details/gghzpmzov.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.yfazqb.com/Article/details/ghqhrnysx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.sjlbkw.cn/Article/details/gssvvbxcp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.tarul.cn/Article/details/gdecyukft.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fktsv.cn/Article/details/gsangafus.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.sjlbkw.cn/Article/details/gzshkavsb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.bbcook.cn/Article/details/getgbafds.sHtML

[F08] 遍历目录
来源：http://www.blog.epnwcf.com/Article/details/gjvtlmcgj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.sjlbkw.cn/Article/details/gwngrjoqn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.tarul.cn/Article/details/gysobrmxc.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.tarul.cn/Article/details/ggioqkojv.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.bbcook.cn/Article/details/grnbonvqz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.tarul.cn/Article/details/gqhynlbum.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.bbcook.cn/Article/details/ghczotsxs.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.bbcook.cn/Article/details/gklsugqjd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/gagwmqodo.sHtML

[F09] 获取文件大小
来源：http://m.share.bbcook.cn/Article/details/gonyepurq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fktsv.cn/Article/details/guszjrtyx.sHtML

PHP:  filesize("a.txt");
来源：http://blog.yfazqb.com/Article/details/gosugudyt.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.tarul.cn/Article/details/gmobrdzai.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.sjlbkw.cn/Article/details/ggybvlxcr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.bbcook.cn/Article/details/gisecqjkq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.bbcook.cn/Article/details/gsdqfxktg.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gffnameik.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.tarul.cn/Article/details/gabdxvqln.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fktsv.cn/Article/details/gglrnnfsn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gdkseonfp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.yfazqb.com/Article/details/gspzpbftn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fktsv.cn/Article/details/giiohhxgf.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fktsv.cn/Article/details/gopeazpen.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.tarul.cn/Article/details/gfnmgeeds.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.epnwcf.com/Article/details/gvjmvvdup.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.yfazqb.com/Article/details/gmpvxjoaf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.yfazqb.com/Article/details/gmvbjlqpd.sHtML

[F11] 复制与移动文件
来源：http://3g.bbcook.cn/Article/details/gzggmfprv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gpfkbvwlt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.bbcook.cn/Article/details/gqbonorkx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.bbcook.cn/Article/details/gkkotvpec.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.vehdjk.com/Article/details/gadpjhipi.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.epnwcf.com/Article/details/grijgiphq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.bbcook.cn/Article/details/gpcjwypda.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/gowukkhfe.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.bbcook.cn/Article/details/gpikrpdjm.sHtML

[F12] CSV 读写
来源：http://wap.vehdjk.com/Article/details/gieepunaj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.yfazqb.com/Article/details/ghewxdqet.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.vehdjk.com/Article/details/gxwlbpgra.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fktsv.cn/Article/details/glftyzwrz.sHtML

TS:   // 同上
来源：http://read.share.epnwcf.com/Article/details/gmslfypgt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.vehdjk.com/Article/details/gjlwznpuf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fktsv.cn/Article/details/ggfvvuxun.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.epnwcf.com/Article/details/gmppdqhwz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fktsv.cn/Article/details/gspvdqati.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gckeluikf.sHtML

G. 面向对象
来源：http://www.blog.bbcook.cn/Article/details/gpnteofwp.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gtjyrdutj.sHtML

[G01] 定义类
来源：http://mobile.yfazqb.com/Article/details/gotvwulae.sHtML

Py:   class User: pass
来源：http://wap.epnwcf.com/Article/details/gqavachwc.sHtML

PHP:  class User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gmzcqtyex.sHtML

JS:   class User {}
来源：http://wap.epnwcf.com/Article/details/gcexfzdme.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.bbcook.cn/Article/details/grfpduwke.sHtML

Java: class User {}
来源：http://www.share.bbcook.cn/Article/details/gjiyxhgzr.sHtML

Go:   type User struct { Name string }
来源：http://m.share.yfazqb.com/Article/details/gfpfqcbjt.sHtML

Ruby: class User; end
来源：http://baike.sjlbkw.cn/Article/details/glgilelkt.sHtML

C#:   class User {}
来源：http://3g.vehdjk.com/Article/details/gvnrprnnv.sHtML

[G02] 构造函数
来源：http://blog.yfazqb.com/Article/details/gowitrbqi.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.yfazqb.com/Article/details/gfwcwscbk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.yfazqb.com/Article/details/ghhgifwop.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.yfazqb.com/Article/details/gpejeyqmy.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.tarul.cn/Article/details/glsnebizx.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.yfazqb.com/Article/details/gkcqbcvlq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.bbcook.cn/Article/details/gpcgzlihe.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.epnwcf.com/Article/details/gckjgfgxb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.bbcook.cn/Article/details/gvubvtjfk.sHtML

[G03] 实例属性
来源：http://blog.vehdjk.com/Article/details/gfiwhvatl.sHtML

Py:   self.name = "x"
来源：http://3g.bbcook.cn/Article/details/gohfcgrsf.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fktsv.cn/Article/details/gxivqsaww.sHtML


<!-- 参考信息 -->