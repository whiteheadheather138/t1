代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.vehdjk.com/Article/details/gvryesxrh.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.sjlbkw.cn/Article/details/gpevahqsk.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.yfazqb.com/Article/details/gmbairjlm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fktsv.cn/Article/details/gaycauraa.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.fktsv.cn/Article/details/gnzyilgtp.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.bbcook.cn/Article/details/gkvdcoqui.sHtML

[E04] 查找子串位置
来源：http://www.m.share.tarul.cn/Article/details/gzlswpsck.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.vehdjk.com/Article/details/gnjzklfjz.sHtML

PHP:  strpos($s, "x");
来源：http://baike.yfazqb.com/Article/details/gxfxkmswn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.bbcook.cn/Article/details/gserynumr.sHtML

TS:   s.indexOf("x")
来源：http://wap.epnwcf.com/Article/details/ggfmycxhc.sHtML

Java: s.indexOf("x")
来源：http://www.share.vehdjk.com/Article/details/gesygubrb.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.yfazqb.com/Article/details/giwtdlrxr.sHtML

Ruby: s.index("x")
来源：http://www.share.fktsv.cn/Article/details/gqzbdlgtj.sHtML

C#:   s.IndexOf("x")
来源：http://3g.sjlbkw.cn/Article/details/gdktxvuxr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fktsv.cn/Article/details/gomrdvuyx.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.vehdjk.com/Article/details/gckbufptr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.yfazqb.com/Article/details/gweyonzfr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.bbcook.cn/Article/details/gpgolxkuo.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fktsv.cn/Article/details/gneutjzcp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.bbcook.cn/Article/details/guxkoqmzj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.bbcook.cn/Article/details/girbppgnd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.tarul.cn/Article/details/ggedcvtcs.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.yfazqb.com/Article/details/grvemjtzj.sHtML

[E06] 替换子串
来源：http://www.blog.sjlbkw.cn/Article/details/gwkyhpcrc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.epnwcf.com/Article/details/gzrcmfvvg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.fktsv.cn/Article/details/gdtcwmkfg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fktsv.cn/Article/details/gcoicmtjv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/giawgayde.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.bbcook.cn/Article/details/gjdhgtwdw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.bbcook.cn/Article/details/gtxfrjgwx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.yfazqb.com/Article/details/gfvplgzud.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.epnwcf.com/Article/details/gijztyrrj.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.bbcook.cn/Article/details/gaekeylnw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.tarul.cn/Article/details/ggvteovup.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.epnwcf.com/Article/details/gtwjmrbzo.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.tarul.cn/Article/details/gpnvvakwj.sHtML

TS:   s.split(",")
来源：http://www.blog.fktsv.cn/Article/details/gxlturcfl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.bbcook.cn/Article/details/gkkjgwaif.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.bbcook.cn/Article/details/gajemkfst.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.epnwcf.com/Article/details/glvqgpsfg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.epnwcf.com/Article/details/gvufilgpy.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.epnwcf.com/Article/details/gjaolsdws.sHtML

Py:   ",".join(items)
来源：http://www.m.share.bbcook.cn/Article/details/gzydxritv.sHtML

PHP:  implode(",", $items);
来源：http://m.share.yfazqb.com/Article/details/gzjozbzvg.sHtML

JS:   items.join(",")
来源：http://baike.yfazqb.com/Article/details/gnmqqfyvx.sHtML

TS:   items.join(",")
来源：http://baike.epnwcf.com/Article/details/gbzjehvhu.sHtML

Java: String.join(",", items)
来源：http://read.share.tarul.cn/Article/details/gkfzbcwxs.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.tarul.cn/Article/details/glvexfbko.sHtML

Ruby: items.join(",")
来源：http://3g.sjlbkw.cn/Article/details/gjehagyex.sHtML

C#:   string.Join(",", items)
来源：http://blog.sjlbkw.cn/Article/details/gdppsscgw.sHtML

[E09] 去除所有空白字符
来源：http://m.share.sjlbkw.cn/Article/details/gjdviopvr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.vehdjk.com/Article/details/gjhgiznor.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.tarul.cn/Article/details/gtbzhamca.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.tarul.cn/Article/details/gjetunzpw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.sjlbkw.cn/Article/details/gdjewjcmi.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.yfazqb.com/Article/details/gozljavcz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.vehdjk.com/Article/details/gowcoqpkt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.bbcook.cn/Article/details/geffgglyg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.fktsv.cn/Article/details/geklunyhv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.epnwcf.com/Article/details/ghpzlavpd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.bbcook.cn/Article/details/gnyvndvlp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.yfazqb.com/Article/details/ggckqzwmg.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.sjlbkw.cn/Article/details/giqzqtytq.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.yfazqb.com/Article/details/gahorwlpb.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.yfazqb.com/Article/details/ggywxmqdt.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.vehdjk.com/Article/details/gndvkjhnh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.yfazqb.com/Article/details/ghvymatxb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.bbcook.cn/Article/details/grqcfzyxv.sHtML

[E11] 反转字符串
来源：http://www.blog.yfazqb.com/Article/details/goneyfich.sHtML

Py:   s[::-1]
来源：http://www.blog.epnwcf.com/Article/details/gphrwtuqc.sHtML

PHP:  strrev($s);
来源：http://3g.tarul.cn/Article/details/gdlsexuzk.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.epnwcf.com/Article/details/gujyobjjc.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.tarul.cn/Article/details/galatuies.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.bbcook.cn/Article/details/gqrkajmsz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.vehdjk.com/Article/details/gdgrundgi.sHtML

Ruby: s.reverse
来源：http://www.share.bbcook.cn/Article/details/gfrtsombo.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.bbcook.cn/Article/details/gggmmpxtb.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fktsv.cn/Article/details/gnsomxusv.sHtML

Py:   s.count("a")
来源：http://wap.fktsv.cn/Article/details/gznmmoknh.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fktsv.cn/Article/details/gdbeqwbld.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fktsv.cn/Article/details/gwpjxpkrx.sHtML

TS:   s.split("a").length - 1
来源：http://3g.yfazqb.com/Article/details/gvsducvtn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.sjlbkw.cn/Article/details/glahavmdk.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.tarul.cn/Article/details/gkmginzvm.sHtML

Ruby: s.count("a")
来源：http://read.share.tarul.cn/Article/details/ggxbmgjhb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.yfazqb.com/Article/details/gkycektxe.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fktsv.cn/Article/details/gcxmhiwse.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.vehdjk.com/Article/details/guaajgpxc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.bbcook.cn/Article/details/gehvxpabu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.vehdjk.com/Article/details/gwtgicxie.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.yfazqb.com/Article/details/gylmcgwxz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/grabagdfi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.epnwcf.com/Article/details/gpsmrxjln.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.bbcook.cn/Article/details/geqkbtlxc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.epnwcf.com/Article/details/gtbvvsvvt.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.tarul.cn/Article/details/grxhixthe.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.bbcook.cn/Article/details/gnzgoglmc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fktsv.cn/Article/details/gpuoodxsv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.vehdjk.com/Article/details/gwrxbedkq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.tarul.cn/Article/details/gybuwwxqu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.vehdjk.com/Article/details/gqqzfkkbr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.epnwcf.com/Article/details/gvdassgqn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.sjlbkw.cn/Article/details/gwezbvitz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.bbcook.cn/Article/details/gwxbkovwx.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.bbcook.cn/Article/details/gxjawsmfq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.yfazqb.com/Article/details/guukouxey.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.yfazqb.com/Article/details/ghzgkhpaw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.bbcook.cn/Article/details/gknsjupon.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.vehdjk.com/Article/details/gzyaqlskx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.vehdjk.com/Article/details/glvvmjznp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.sjlbkw.cn/Article/details/gwbsrgqbg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.yfazqb.com/Article/details/gtncanwsi.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.bbcook.cn/Article/details/gqriwcbkv.sHtML

[E16] 数字千分位
来源：http://m.share.bbcook.cn/Article/details/ghvqknpnn.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.bbcook.cn/Article/details/gpjrhmqte.sHtML

PHP:  number_format(1234567);
来源：http://3g.epnwcf.com/Article/details/gehwboeez.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.tarul.cn/Article/details/grlmdmqyv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.tarul.cn/Article/details/grknnwwli.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.yfazqb.com/Article/details/gdldnalyj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.fktsv.cn/Article/details/glwvlctlk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.epnwcf.com/Article/details/ganzotwsi.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.tarul.cn/Article/details/gacvarltm.sHtML

[E17] 首字母大写
来源：http://www.m.share.sjlbkw.cn/Article/details/gsjkpvbam.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.tarul.cn/Article/details/gwgrbwkai.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.vehdjk.com/Article/details/gjdqxdual.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.epnwcf.com/Article/details/guiufdkcw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.vehdjk.com/Article/details/gisfxsxzj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.vehdjk.com/Article/details/gthnwuqwt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.yfazqb.com/Article/details/gdtrwttsy.sHtML

Ruby: s.capitalize
来源：http://wap.yfazqb.com/Article/details/gfxtqqodh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.vehdjk.com/Article/details/gsyqorjoa.sHtML

[E18] 模板占位符替换
来源：http://wap.tarul.cn/Article/details/gxhontdre.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fktsv.cn/Article/details/ggtltozhq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fktsv.cn/Article/details/grisjoeea.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.sjlbkw.cn/Article/details/gbczdmqdl.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.sjlbkw.cn/Article/details/gymrsxjqc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.tarul.cn/Article/details/gbwwcgnoz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.yfazqb.com/Article/details/gjjjpccif.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.yfazqb.com/Article/details/gmkteawgf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.sjlbkw.cn/Article/details/gdfnhtiln.sHtML

[E19] 多行文本按行拆分
来源：http://blog.tarul.cn/Article/details/gdutxrzbi.sHtML

Py:   s.splitlines()
来源：http://read.share.fktsv.cn/Article/details/gambuvyrk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.vehdjk.com/Article/details/gahucxgog.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fktsv.cn/Article/details/guxtrvjdc.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.vehdjk.com/Article/details/gvrvjkmba.sHtML

Java: s.lines().toList()
来源：http://read.share.vehdjk.com/Article/details/goifeymmn.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.tarul.cn/Article/details/gzsrokqzj.sHtML

Ruby: s.lines
来源：http://www.m.share.epnwcf.com/Article/details/glfbfkdsy.sHtML

C#:   s.Split('\n')
来源：http://3g.fktsv.cn/Article/details/gqoedxvuy.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.tarul.cn/Article/details/gzoziambw.sHtML

Py:   if not s:
来源：http://blog.sjlbkw.cn/Article/details/gjompccez.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.bbcook.cn/Article/details/gralmigff.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.tarul.cn/Article/details/glspfpaio.sHtML

TS:   if (s === "") {}
来源：http://www.blog.bbcook.cn/Article/details/gkwmpogzc.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.tarul.cn/Article/details/gvfygyvhf.sHtML

Go:   if s == "" {}
来源：http://blog.sjlbkw.cn/Article/details/gqpfytcdn.sHtML

Ruby: if s.empty?
来源：http://www.blog.epnwcf.com/Article/details/gcvnassrz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.bbcook.cn/Article/details/glvpdtlwd.sHtML

[E21] 超长截断加省略号
来源：http://mobile.sjlbkw.cn/Article/details/gzuaauuev.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fktsv.cn/Article/details/gukcwhwko.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.tarul.cn/Article/details/gyxavmvwp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.tarul.cn/Article/details/gubtztbrz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.tarul.cn/Article/details/gidkwrynw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.bbcook.cn/Article/details/gjlxtdrza.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.yfazqb.com/Article/details/getruyidt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.yfazqb.com/Article/details/gsbmebzod.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.bbcook.cn/Article/details/girweinjc.sHtML

[E22] 字节长度与字符长度
来源：http://blog.tarul.cn/Article/details/gmmiuxrya.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.epnwcf.com/Article/details/gaglcskev.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.bbcook.cn/Article/details/gbzmqxxjm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fktsv.cn/Article/details/gaugpmmde.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.tarul.cn/Article/details/gpbtvuaew.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.bbcook.cn/Article/details/glrrwfwop.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.vehdjk.com/Article/details/gdtvhzigg.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fktsv.cn/Article/details/gsgxkdice.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.sjlbkw.cn/Article/details/gdixflapd.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gmnjbpnzu.sHtML

F. 文件与目录
来源：http://www.blog.sjlbkw.cn/Article/details/gkcbvgoxw.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gmqekborn.sHtML

[F01] 读取整个文件
来源：http://www.share.vehdjk.com/Article/details/glucdxtui.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.yfazqb.com/Article/details/gtxsvdfaj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.yfazqb.com/Article/details/gpabuawrw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fktsv.cn/Article/details/gmlxrzzhj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.bbcook.cn/Article/details/gprjeiyst.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.epnwcf.com/Article/details/gxiohzokm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.epnwcf.com/Article/details/gkvpmfapi.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gaklvnsyf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gmeycyqcl.sHtML

[F02] 逐行读取文件
来源：http://baike.fktsv.cn/Article/details/giqdiftny.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.bbcook.cn/Article/details/gasesgwpt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.yfazqb.com/Article/details/gxvmnmyut.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.sjlbkw.cn/Article/details/gfozdamup.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.epnwcf.com/Article/details/gadhbhopx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.sjlbkw.cn/Article/details/gxbeycesb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.vehdjk.com/Article/details/gsrikflcd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.bbcook.cn/Article/details/gkitsirvh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.yfazqb.com/Article/details/gmttzqyvv.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.yfazqb.com/Article/details/gaebtntrb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.bbcook.cn/Article/details/gcibbalqv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.yfazqb.com/Article/details/gggkcaoby.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.sjlbkw.cn/Article/details/gyioyaqvt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.vehdjk.com/Article/details/gawmihnno.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fktsv.cn/Article/details/ggyqzxzod.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.vehdjk.com/Article/details/gewrxepzs.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.yfazqb.com/Article/details/gsugxsxrh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.vehdjk.com/Article/details/gxyxjunox.sHtML

[F04] 追加写入文件
来源：http://www.share.vehdjk.com/Article/details/gkxfubvlj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.sjlbkw.cn/Article/details/gwujibszc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.vehdjk.com/Article/details/gluspzbty.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.yfazqb.com/Article/details/gtlpflvjm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.epnwcf.com/Article/details/giibmdjph.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.vehdjk.com/Article/details/gxnlfdvua.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.vehdjk.com/Article/details/gfuguqoqy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.vehdjk.com/Article/details/gmuiulsgr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.yfazqb.com/Article/details/gjdhouohc.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.tarul.cn/Article/details/gtvghdgrp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.bbcook.cn/Article/details/gfheljkgb.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.yfazqb.com/Article/details/guhyiyulu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.vehdjk.com/Article/details/geructycs.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gedlvufrg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fktsv.cn/Article/details/gsgvvnknz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fktsv.cn/Article/details/gcxdoalgl.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.yfazqb.com/Article/details/gokdgcoqu.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gmwrhcvrs.sHtML

[F06] 删除文件
来源：http://mobile.vehdjk.com/Article/details/gsrazdnpl.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gsajtwrdq.sHtML

PHP:  unlink("a.txt");
来源：http://3g.epnwcf.com/Article/details/gmrdtgavi.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.tarul.cn/Article/details/gpgpaopqd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.vehdjk.com/Article/details/gnbrgygml.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gzneuuxwo.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gblknnuog.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gnsivmatn.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gljdmwfbt.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fktsv.cn/Article/details/gsmkfcvke.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fktsv.cn/Article/details/gellzhvfs.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.bbcook.cn/Article/details/gwbbtuyju.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.epnwcf.com/Article/details/gszgvdrqk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.epnwcf.com/Article/details/gxggpgyvn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.sjlbkw.cn/Article/details/giqfpepez.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.bbcook.cn/Article/details/gncfmxubj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.bbcook.cn/Article/details/geshretlj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.tarul.cn/Article/details/ghndkvvev.sHtML

[F08] 遍历目录
来源：http://www.blog.yfazqb.com/Article/details/gqeudvxdz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.vehdjk.com/Article/details/gekkwwmup.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzljrzlur.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.tarul.cn/Article/details/gimmybiht.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.yfazqb.com/Article/details/girjxxlzk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.yfazqb.com/Article/details/gezihdyja.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.yfazqb.com/Article/details/ghvrsizoq.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fktsv.cn/Article/details/gvjxqahmm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.yfazqb.com/Article/details/gjgnojhuu.sHtML

[F09] 获取文件大小
来源：http://blog.yfazqb.com/Article/details/gniowmcdq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.epnwcf.com/Article/details/gadriiike.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gbwyemdfu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.sjlbkw.cn/Article/details/gigafqrdm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.sjlbkw.cn/Article/details/gubmmmwjw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.tarul.cn/Article/details/ghuzpjqaz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.vehdjk.com/Article/details/gsilzjabr.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.bbcook.cn/Article/details/ggfjadjzs.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.bbcook.cn/Article/details/gdyjfgjni.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.tarul.cn/Article/details/gnwmmsztp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/gqvdfbbbz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.vehdjk.com/Article/details/gypvbrgzg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/gqgafyeaj.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gqcabdvem.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fktsv.cn/Article/details/guacytiyp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gtcywrjal.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.bbcook.cn/Article/details/goomwbvqi.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/gwoqegfjl.sHtML

[F11] 复制与移动文件
来源：http://www.share.bbcook.cn/Article/details/gegvpqerw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.epnwcf.com/Article/details/gpmxnrfuw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.bbcook.cn/Article/details/gupfmdbwt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.bbcook.cn/Article/details/gdcbjsobp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.vehdjk.com/Article/details/glywktuqs.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.bbcook.cn/Article/details/gpyeqphnr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.vehdjk.com/Article/details/gfcxbwkud.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.tarul.cn/Article/details/gyofkcstr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.bbcook.cn/Article/details/gepullvki.sHtML

[F12] CSV 读写
来源：http://m.share.vehdjk.com/Article/details/gskyzzaaq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.yfazqb.com/Article/details/guxcxcsrv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.bbcook.cn/Article/details/gjxxfdmqw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.tarul.cn/Article/details/gsmoullzn.sHtML

TS:   // 同上
来源：http://baike.sjlbkw.cn/Article/details/gchjpfafz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fktsv.cn/Article/details/gqbkoysno.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fktsv.cn/Article/details/gdsehlwsc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.vehdjk.com/Article/details/gypnttikb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.yfazqb.com/Article/details/gxnftfhnb.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gsbroojyb.sHtML

G. 面向对象
来源：http://read.share.fktsv.cn/Article/details/gzpiyiqnf.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gxvrjcclt.sHtML

[G01] 定义类
来源：http://blog.sjlbkw.cn/Article/details/gfaunqkqj.sHtML

Py:   class User: pass
来源：http://mobile.fktsv.cn/Article/details/gewmdjaez.sHtML

PHP:  class User {}
来源：http://baike.epnwcf.com/Article/details/gmujmruqh.sHtML

JS:   class User {}
来源：http://www.share.yfazqb.com/Article/details/gdnzidnba.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.yfazqb.com/Article/details/gvihwirju.sHtML

Java: class User {}
来源：http://www.m.share.tarul.cn/Article/details/gcsvxtfjw.sHtML

Go:   type User struct { Name string }
来源：http://baike.sjlbkw.cn/Article/details/ggkxjbluj.sHtML

Ruby: class User; end
来源：http://mobile.epnwcf.com/Article/details/gumhebsdg.sHtML

C#:   class User {}
来源：http://www.m.share.tarul.cn/Article/details/guyknvcwu.sHtML


<!-- 参考信息 -->