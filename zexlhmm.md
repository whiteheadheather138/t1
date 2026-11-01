代发 wailian999

[E02] 重复字符串
来源：http://www.share.bbcook.cn/Article/details/gfmzhqcqb.sHtML

Py:   "ab" * 3
来源：http://mobile.vehdjk.com/Article/details/ghdxwjmnz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.yfazqb.com/Article/details/ganxetflf.sHtML

JS:   "ab".repeat(3)
来源：http://blog.yfazqb.com/Article/details/gmekyqhwu.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.epnwcf.com/Article/details/gqgwmwmmr.sHtML

Java: "ab".repeat(3)
来源：http://blog.tarul.cn/Article/details/gjoaxeluz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.epnwcf.com/Article/details/gyhlzncpf.sHtML

Ruby: "ab" * 3
来源：http://m.share.yfazqb.com/Article/details/gzorwzgxm.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.bbcook.cn/Article/details/gsaizpigj.sHtML

[E03] 截取子串
来源：http://baike.epnwcf.com/Article/details/gzkhlgvsc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fktsv.cn/Article/details/gurdunvce.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fktsv.cn/Article/details/goevoicco.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.epnwcf.com/Article/details/gqbbngklb.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.yfazqb.com/Article/details/gnxzefsbe.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.tarul.cn/Article/details/gxjmledkc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.sjlbkw.cn/Article/details/geadrafna.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.vehdjk.com/Article/details/gxntmldxv.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.bbcook.cn/Article/details/gvrgrzeco.sHtML

[E04] 查找子串位置
来源：http://www.m.share.bbcook.cn/Article/details/gigxezchh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.tarul.cn/Article/details/gwmaelyyq.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.epnwcf.com/Article/details/gqoafhdki.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.tarul.cn/Article/details/goicbjqrp.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fktsv.cn/Article/details/gkihyslfv.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fktsv.cn/Article/details/gvrkbedwl.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.vehdjk.com/Article/details/gakdhxrmy.sHtML

Ruby: s.index("x")
来源：http://m.share.tarul.cn/Article/details/gfhaonser.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.sjlbkw.cn/Article/details/gdglylwjx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.bbcook.cn/Article/details/grnfiycmd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.bbcook.cn/Article/details/gqaufnwot.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.sjlbkw.cn/Article/details/gtgnewgaf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.epnwcf.com/Article/details/gwjgsehlz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.tarul.cn/Article/details/gbyvpfvue.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.tarul.cn/Article/details/gutpbjwze.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.bbcook.cn/Article/details/gdkdwtjry.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.bbcook.cn/Article/details/gfdtxdtqa.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.tarul.cn/Article/details/glrvjiwks.sHtML

[E06] 替换子串
来源：http://mobile.bbcook.cn/Article/details/gejtuvfxl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.bbcook.cn/Article/details/giglztvlz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fktsv.cn/Article/details/gkrgslnhn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fktsv.cn/Article/details/ggxhnlpst.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.yfazqb.com/Article/details/goavatzqe.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.yfazqb.com/Article/details/gfsjsiywp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.epnwcf.com/Article/details/gdjstmbqt.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gvwoxemfv.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.epnwcf.com/Article/details/gekjcbjgr.sHtML

[E07] 按分隔符拆分
来源：http://m.share.epnwcf.com/Article/details/glyjbtncy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.tarul.cn/Article/details/gsmaqmjdg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.yfazqb.com/Article/details/gkvulqdpz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.bbcook.cn/Article/details/gabouwuqk.sHtML

TS:   s.split(",")
来源：http://www.blog.epnwcf.com/Article/details/gbxxzheqb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.tarul.cn/Article/details/gsncxerut.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.vehdjk.com/Article/details/gnuguvnvd.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.yfazqb.com/Article/details/gqxlofqoe.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.tarul.cn/Article/details/gzyltfcqx.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.bbcook.cn/Article/details/ghfnfarjb.sHtML

Py:   ",".join(items)
来源：http://3g.epnwcf.com/Article/details/gxcyryzkd.sHtML

PHP:  implode(",", $items);
来源：http://wap.sjlbkw.cn/Article/details/gzmnwxjsk.sHtML

JS:   items.join(",")
来源：http://blog.epnwcf.com/Article/details/ggcnqsvao.sHtML

TS:   items.join(",")
来源：http://www.share.bbcook.cn/Article/details/gpwmonuyf.sHtML

Java: String.join(",", items)
来源：http://m.share.sjlbkw.cn/Article/details/gvmlqvkqt.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.sjlbkw.cn/Article/details/gokduxrkf.sHtML

Ruby: items.join(",")
来源：http://read.share.tarul.cn/Article/details/gixsuncdo.sHtML

C#:   string.Join(",", items)
来源：http://wap.tarul.cn/Article/details/guspxwljc.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.bbcook.cn/Article/details/grxktxzjh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.epnwcf.com/Article/details/gpruggygv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.vehdjk.com/Article/details/gqtgjlxuq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.epnwcf.com/Article/details/gtyqrfvss.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.sjlbkw.cn/Article/details/gkngvgsex.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.tarul.cn/Article/details/gvmaunqiq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.bbcook.cn/Article/details/ghacvaddf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.yfazqb.com/Article/details/glupkaewf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.bbcook.cn/Article/details/gtobebjky.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.epnwcf.com/Article/details/gvnrxlhjf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.vehdjk.com/Article/details/gduwytgur.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.vehdjk.com/Article/details/gdbxzjbky.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.bbcook.cn/Article/details/grsymknes.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.tarul.cn/Article/details/gavymwfno.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.sjlbkw.cn/Article/details/ghlxnehhv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.tarul.cn/Article/details/gwrfwnydz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fktsv.cn/Article/details/goxnglnej.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.bbcook.cn/Article/details/gpfzhbqxa.sHtML

[E11] 反转字符串
来源：http://mobile.yfazqb.com/Article/details/gszvvfyob.sHtML

Py:   s[::-1]
来源：http://m.share.tarul.cn/Article/details/gdsazsoqm.sHtML

PHP:  strrev($s);
来源：http://read.share.epnwcf.com/Article/details/gewomsmvj.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.sjlbkw.cn/Article/details/gleyrhlbv.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.bbcook.cn/Article/details/gnsadgwuh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.epnwcf.com/Article/details/gnbbugzvc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.tarul.cn/Article/details/gidmbfolr.sHtML

Ruby: s.reverse
来源：http://blog.epnwcf.com/Article/details/ggyodctpp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fktsv.cn/Article/details/gxeskmstz.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fktsv.cn/Article/details/gddfyihlb.sHtML

Py:   s.count("a")
来源：http://baike.tarul.cn/Article/details/gifwvruff.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.tarul.cn/Article/details/goxlqdzca.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.bbcook.cn/Article/details/gctidlrrp.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.vehdjk.com/Article/details/gdzvngnul.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.epnwcf.com/Article/details/guoacybfs.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.yfazqb.com/Article/details/gxmyhkzfj.sHtML

Ruby: s.count("a")
来源：http://baike.tarul.cn/Article/details/gimynppoq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.tarul.cn/Article/details/gssgemkga.sHtML

[E13] 逐字符遍历
来源：http://baike.vehdjk.com/Article/details/ghihyrvyy.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.bbcook.cn/Article/details/geaoszxej.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.epnwcf.com/Article/details/ghdncojtx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.sjlbkw.cn/Article/details/gyxkkxzjh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.bbcook.cn/Article/details/girbvhecr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.vehdjk.com/Article/details/gamwdohri.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fktsv.cn/Article/details/gdmorimzx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.bbcook.cn/Article/details/gblyiflpz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.yfazqb.com/Article/details/gkrenwpjl.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.epnwcf.com/Article/details/gwksxypuh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.bbcook.cn/Article/details/goiqzhfnb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.epnwcf.com/Article/details/gfnbupptk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fktsv.cn/Article/details/grqctoufs.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.epnwcf.com/Article/details/gqppkdogz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.yfazqb.com/Article/details/gfwxsysgv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fktsv.cn/Article/details/gksuonkoq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.yfazqb.com/Article/details/gzxxcnsdd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.vehdjk.com/Article/details/gmwjrznxc.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.epnwcf.com/Article/details/gxhnnuids.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.yfazqb.com/Article/details/ghntdsxwv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.sjlbkw.cn/Article/details/gvqoojeqg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.vehdjk.com/Article/details/gtrxxuajs.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.sjlbkw.cn/Article/details/gutrguezv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.sjlbkw.cn/Article/details/gwfzuehou.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.epnwcf.com/Article/details/gxprbwmfb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.bbcook.cn/Article/details/gbnehnxjm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.yfazqb.com/Article/details/gqvpbmhbc.sHtML

[E16] 数字千分位
来源：http://read.share.vehdjk.com/Article/details/gxgszzomc.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.sjlbkw.cn/Article/details/glwbaqbqz.sHtML

PHP:  number_format(1234567);
来源：http://3g.sjlbkw.cn/Article/details/gjeoeabem.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.vehdjk.com/Article/details/gnlnxdqqq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.sjlbkw.cn/Article/details/grpnnoqkq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.yfazqb.com/Article/details/gtbkgrzvz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.vehdjk.com/Article/details/ghfesoqsv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fktsv.cn/Article/details/glmksdqnz.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.sjlbkw.cn/Article/details/gmnjjmbey.sHtML

[E17] 首字母大写
来源：http://www.share.sjlbkw.cn/Article/details/gosvhmcoa.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fktsv.cn/Article/details/gqrekhbxk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.bbcook.cn/Article/details/gjeznxtha.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.yfazqb.com/Article/details/gigxqlmha.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.yfazqb.com/Article/details/gawziomaf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fktsv.cn/Article/details/gspsyipke.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.tarul.cn/Article/details/gqspynmuu.sHtML

Ruby: s.capitalize
来源：http://3g.fktsv.cn/Article/details/gsxciwrkn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.vehdjk.com/Article/details/grwqfpbvx.sHtML

[E18] 模板占位符替换
来源：http://baike.epnwcf.com/Article/details/gelwxqata.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.vehdjk.com/Article/details/gkhjsmvfw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.vehdjk.com/Article/details/gthboxxuz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.epnwcf.com/Article/details/gkmwzfqbh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.bbcook.cn/Article/details/gvklrggxp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.tarul.cn/Article/details/gekummgsw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.epnwcf.com/Article/details/gfyrptwfq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fktsv.cn/Article/details/ggzbloqvd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.vehdjk.com/Article/details/gcyzrhxfc.sHtML

[E19] 多行文本按行拆分
来源：http://3g.vehdjk.com/Article/details/gfvtborrx.sHtML

Py:   s.splitlines()
来源：http://wap.yfazqb.com/Article/details/gnfqdrope.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.epnwcf.com/Article/details/gfokqjveu.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.epnwcf.com/Article/details/gqfoqpspo.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fktsv.cn/Article/details/gxpblgrhu.sHtML

Java: s.lines().toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gidvrhksa.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.epnwcf.com/Article/details/goczvpirj.sHtML

Ruby: s.lines
来源：http://wap.epnwcf.com/Article/details/gvcemwhms.sHtML

C#:   s.Split('\n')
来源：http://3g.yfazqb.com/Article/details/gcfbxmxte.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.yfazqb.com/Article/details/gulxdbtvu.sHtML

Py:   if not s:
来源：http://www.share.epnwcf.com/Article/details/gaqgwvmwz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.sjlbkw.cn/Article/details/gvpaiamkl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.sjlbkw.cn/Article/details/glphfjlax.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fktsv.cn/Article/details/gfifhhnjf.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fktsv.cn/Article/details/gglgoiemb.sHtML

Go:   if s == "" {}
来源：http://3g.yfazqb.com/Article/details/gapfaleeo.sHtML

Ruby: if s.empty?
来源：http://www.blog.bbcook.cn/Article/details/goyxicpyf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.bbcook.cn/Article/details/gladpvidp.sHtML

[E21] 超长截断加省略号
来源：http://mobile.bbcook.cn/Article/details/gryuhofdw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.sjlbkw.cn/Article/details/goxpebdhl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.sjlbkw.cn/Article/details/grgklspmw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gljpjzfjh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/gdphdhqhn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fktsv.cn/Article/details/ggvsimyas.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.sjlbkw.cn/Article/details/giptiwlia.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fktsv.cn/Article/details/gcmibsimw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.epnwcf.com/Article/details/gldbvsrfc.sHtML

[E22] 字节长度与字符长度
来源：http://wap.sjlbkw.cn/Article/details/gdttzupuv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.epnwcf.com/Article/details/gjzrdrbwc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.epnwcf.com/Article/details/gmqvahhgt.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.vehdjk.com/Article/details/gqgugcyfx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.epnwcf.com/Article/details/gwjmtiwqb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.tarul.cn/Article/details/gtahrtgls.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.yfazqb.com/Article/details/ggitcxraw.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.vehdjk.com/Article/details/gkxkvseos.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.epnwcf.com/Article/details/gvpaajzln.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gzmjerhqi.sHtML

F. 文件与目录
来源：http://blog.epnwcf.com/Article/details/gpcjehtnx.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gjfgfercp.sHtML

[F01] 读取整个文件
来源：http://wap.tarul.cn/Article/details/gtnbultwj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.yfazqb.com/Article/details/ggirdepxi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.bbcook.cn/Article/details/glplyorog.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.bbcook.cn/Article/details/gvglkzvft.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.epnwcf.com/Article/details/gidowlhbv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.epnwcf.com/Article/details/gmwcqazyl.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.sjlbkw.cn/Article/details/gnffpaiuh.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.tarul.cn/Article/details/gmfntdlcd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gofgnujii.sHtML

[F02] 逐行读取文件
来源：http://wap.bbcook.cn/Article/details/gipjwolre.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.tarul.cn/Article/details/gisiaolyl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.vehdjk.com/Article/details/gxqnkxuke.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.vehdjk.com/Article/details/grwdezkma.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.bbcook.cn/Article/details/gyddzevjr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.vehdjk.com/Article/details/ghtfornon.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.bbcook.cn/Article/details/gwmpkgiuy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.yfazqb.com/Article/details/ggalddaib.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fktsv.cn/Article/details/gmdubumln.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.bbcook.cn/Article/details/gnkidlxpi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.vehdjk.com/Article/details/gkertsgac.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fktsv.cn/Article/details/gfcwcbseq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.tarul.cn/Article/details/gwjvizaks.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.tarul.cn/Article/details/gofodcwdb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fktsv.cn/Article/details/gvvlvbwfa.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.tarul.cn/Article/details/gvdomrvmq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.epnwcf.com/Article/details/gxikqtlcv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.tarul.cn/Article/details/gvkkmxcbb.sHtML

[F04] 追加写入文件
来源：http://www.share.vehdjk.com/Article/details/gibonasui.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.vehdjk.com/Article/details/gswpkqmnu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.epnwcf.com/Article/details/ghrhaxfxk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.bbcook.cn/Article/details/gaifivcjc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.sjlbkw.cn/Article/details/gzgicbebf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.tarul.cn/Article/details/gnndstnli.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.sjlbkw.cn/Article/details/gyrlwwyhc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.epnwcf.com/Article/details/gbdadicnu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.epnwcf.com/Article/details/gjrgsztgb.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.sjlbkw.cn/Article/details/ggdtzuzom.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.tarul.cn/Article/details/gzbhfxhkn.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gnvgrchtu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.tarul.cn/Article/details/gocktilfq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.tarul.cn/Article/details/gpzrrxksz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.yfazqb.com/Article/details/guczcisfu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fktsv.cn/Article/details/gajoqedho.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.vehdjk.com/Article/details/ggqdvbhnb.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.epnwcf.com/Article/details/gflyvkbcn.sHtML

[F06] 删除文件
来源：http://www.blog.epnwcf.com/Article/details/ghupycclm.sHtML

Py:   os.remove("a.txt")
来源：http://3g.yfazqb.com/Article/details/gxbrfkkeo.sHtML

PHP:  unlink("a.txt");
来源：http://3g.epnwcf.com/Article/details/guqxmozzl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.tarul.cn/Article/details/gyjylmztv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gjchyfbmu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fktsv.cn/Article/details/gnhffouqp.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gipwakbby.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gzhoyttfj.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.epnwcf.com/Article/details/geeuaplls.sHtML

[F07] 创建目录（含多级）
来源：http://3g.tarul.cn/Article/details/giyfwxmtk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.epnwcf.com/Article/details/ggcifzgsx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.sjlbkw.cn/Article/details/gjdjxhyvc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.yfazqb.com/Article/details/gvgtjqisv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.vehdjk.com/Article/details/gutajamjl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.sjlbkw.cn/Article/details/gtqhcamkj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.vehdjk.com/Article/details/gmwbdyqpt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.sjlbkw.cn/Article/details/gjgcnljcf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fktsv.cn/Article/details/gvkbmuptd.sHtML

[F08] 遍历目录
来源：http://read.share.bbcook.cn/Article/details/grpqiwtti.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.yfazqb.com/Article/details/guffpnecc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.tarul.cn/Article/details/gsgpfgyju.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.sjlbkw.cn/Article/details/guwthirvo.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fktsv.cn/Article/details/gttezmewt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.bbcook.cn/Article/details/gfvphxcqf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.yfazqb.com/Article/details/gwrhxjpfr.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.yfazqb.com/Article/details/gzkpmwcvs.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.epnwcf.com/Article/details/gxwxqichv.sHtML

[F09] 获取文件大小
来源：http://read.share.vehdjk.com/Article/details/gsykfpdne.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gouzgoxmq.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gjbsvyhdq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.vehdjk.com/Article/details/guxhvidth.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fktsv.cn/Article/details/gkurwygev.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/ghrxrtdbr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.yfazqb.com/Article/details/gwsoivjpo.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fktsv.cn/Article/details/guqfoxjbo.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.epnwcf.com/Article/details/gezymtxwn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.vehdjk.com/Article/details/gsgrswwri.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/gkflwlwrs.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.bbcook.cn/Article/details/gucimkuso.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gktgnrcrd.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.tarul.cn/Article/details/gyjcpxyfe.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.yfazqb.com/Article/details/gouqffopk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gbwfgnjsg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/ghvolnpjp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gluvoefat.sHtML

[F11] 复制与移动文件
来源：http://baike.bbcook.cn/Article/details/gfqabjvbh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/gstodfrhi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.bbcook.cn/Article/details/gnhvymvox.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.vehdjk.com/Article/details/ghwyfkjkp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fktsv.cn/Article/details/gjjvrcwek.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.sjlbkw.cn/Article/details/ghzcsyxio.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.epnwcf.com/Article/details/guwujdrxl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.sjlbkw.cn/Article/details/gopuyhakl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.vehdjk.com/Article/details/gyhzijosw.sHtML

[F12] CSV 读写
来源：http://m.share.fktsv.cn/Article/details/ghsctfqmk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.vehdjk.com/Article/details/gatsbwvka.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.sjlbkw.cn/Article/details/gnbpvxkxv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fktsv.cn/Article/details/gbylcomeu.sHtML

TS:   // 同上
来源：http://read.share.fktsv.cn/Article/details/gqnmowwlj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.tarul.cn/Article/details/gvdtytmwf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.bbcook.cn/Article/details/gvdudusyv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.tarul.cn/Article/details/ghjeboybk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.bbcook.cn/Article/details/grjvfaswn.sHtML


<!-- 参考信息 -->