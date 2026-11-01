代发 wailian999

TS:   "ab".repeat(3)
来源：http://read.share.vehdjk.com/Article/details/gfyqwaxfs.sHtML

Java: "ab".repeat(3)
来源：http://baike.sjlbkw.cn/Article/details/gwhqwdxay.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.bbcook.cn/Article/details/gdjzlswuj.sHtML

Ruby: "ab" * 3
来源：http://baike.bbcook.cn/Article/details/gahmmzrka.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.yfazqb.com/Article/details/gbpfzpnry.sHtML

[E03] 截取子串
来源：http://www.blog.yfazqb.com/Article/details/gfxubqbvj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.epnwcf.com/Article/details/gdzebagml.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.tarul.cn/Article/details/gvwkrzlrj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.epnwcf.com/Article/details/gvsuouocu.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fktsv.cn/Article/details/guajaorxg.sHtML

Java: s.substring(1, 4)
来源：http://mobile.vehdjk.com/Article/details/gpjvcdboo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fktsv.cn/Article/details/gbeqanrqd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.sjlbkw.cn/Article/details/gmwyixppu.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.bbcook.cn/Article/details/gcljgogvr.sHtML

[E04] 查找子串位置
来源：http://blog.bbcook.cn/Article/details/gwbrfyjit.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.sjlbkw.cn/Article/details/gjhogvgwc.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.bbcook.cn/Article/details/givhkmuen.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.yfazqb.com/Article/details/gzafswpfe.sHtML

TS:   s.indexOf("x")
来源：http://www.share.yfazqb.com/Article/details/gmavrjcvf.sHtML

Java: s.indexOf("x")
来源：http://mobile.vehdjk.com/Article/details/gfctcxirp.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.fktsv.cn/Article/details/gugimzwmd.sHtML

Ruby: s.index("x")
来源：http://read.share.yfazqb.com/Article/details/gidccoelw.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fktsv.cn/Article/details/gdhuzcxmp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.tarul.cn/Article/details/gvanunxpm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.bbcook.cn/Article/details/guutmsxoi.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.yfazqb.com/Article/details/gwxqyshdw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.epnwcf.com/Article/details/ggypyxysx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fktsv.cn/Article/details/gzuhrdgnb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.sjlbkw.cn/Article/details/gegxppelh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.sjlbkw.cn/Article/details/gjbnleesu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.yfazqb.com/Article/details/gufxsyovn.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fktsv.cn/Article/details/gjrlpkhde.sHtML

[E06] 替换子串
来源：http://blog.tarul.cn/Article/details/gobriybsu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.tarul.cn/Article/details/gdxznwnvo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.tarul.cn/Article/details/gdaaccaaw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gfglvkiur.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/gydanalqj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gmhylktct.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.vehdjk.com/Article/details/gjhejzhoq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.tarul.cn/Article/details/ghhhboqoh.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gmqvmmxir.sHtML

[E07] 按分隔符拆分
来源：http://www.share.vehdjk.com/Article/details/gwayhipot.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fktsv.cn/Article/details/gscuztyjj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fktsv.cn/Article/details/gkortwqnm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.vehdjk.com/Article/details/gvomhucvr.sHtML

TS:   s.split(",")
来源：http://read.share.vehdjk.com/Article/details/gvgvndzud.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.vehdjk.com/Article/details/gbmtpnznf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gychzlcng.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.yfazqb.com/Article/details/gyraoxddp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.epnwcf.com/Article/details/gjseydjka.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.epnwcf.com/Article/details/gdaxngjvz.sHtML

Py:   ",".join(items)
来源：http://mobile.yfazqb.com/Article/details/gvdfeolqq.sHtML

PHP:  implode(",", $items);
来源：http://read.share.bbcook.cn/Article/details/gpagaoqfd.sHtML

JS:   items.join(",")
来源：http://blog.bbcook.cn/Article/details/gtxgehonk.sHtML

TS:   items.join(",")
来源：http://mobile.sjlbkw.cn/Article/details/gxualsjyp.sHtML

Java: String.join(",", items)
来源：http://www.m.share.vehdjk.com/Article/details/gzcnfpxro.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.yfazqb.com/Article/details/gtqxbdeoc.sHtML

Ruby: items.join(",")
来源：http://mobile.sjlbkw.cn/Article/details/gksmqwyqy.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.bbcook.cn/Article/details/gzxqbwrnj.sHtML

[E09] 去除所有空白字符
来源：http://read.share.yfazqb.com/Article/details/gqpbpqfht.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.tarul.cn/Article/details/gyycadfor.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.bbcook.cn/Article/details/gaaatvmgw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.tarul.cn/Article/details/gobbvfwxw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.bbcook.cn/Article/details/gewnhcqsr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.vehdjk.com/Article/details/gobsdksml.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.bbcook.cn/Article/details/gixvrwndt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.sjlbkw.cn/Article/details/gklumobjz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.epnwcf.com/Article/details/gteqxejyc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.sjlbkw.cn/Article/details/gohprrccf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.tarul.cn/Article/details/gckrnjxwp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.yfazqb.com/Article/details/grbznkyly.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.yfazqb.com/Article/details/ghpxgswai.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjgrbylns.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.yfazqb.com/Article/details/gpmhlhnol.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.sjlbkw.cn/Article/details/giiwhthfi.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.bbcook.cn/Article/details/ghreafqaq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.yfazqb.com/Article/details/gywtfhuid.sHtML

[E11] 反转字符串
来源：http://blog.bbcook.cn/Article/details/gpycepwla.sHtML

Py:   s[::-1]
来源：http://baike.yfazqb.com/Article/details/ghyofcabt.sHtML

PHP:  strrev($s);
来源：http://blog.sjlbkw.cn/Article/details/giqvnyvzw.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.epnwcf.com/Article/details/ggvgthcbl.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.vehdjk.com/Article/details/gxqsimzrc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.sjlbkw.cn/Article/details/gdqwiblxc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.vehdjk.com/Article/details/gybqlzcml.sHtML

Ruby: s.reverse
来源：http://3g.epnwcf.com/Article/details/gkhpkoyts.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fktsv.cn/Article/details/gksyivwas.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.epnwcf.com/Article/details/gfaaxbagj.sHtML

Py:   s.count("a")
来源：http://read.share.vehdjk.com/Article/details/gxbysbmne.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.tarul.cn/Article/details/gjasdsazm.sHtML

JS:   s.split("a").length - 1
来源：http://baike.tarul.cn/Article/details/gbicmekrx.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.vehdjk.com/Article/details/gnvewzmak.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.epnwcf.com/Article/details/ghnjkhglk.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.tarul.cn/Article/details/gayrxafud.sHtML

Ruby: s.count("a")
来源：http://www.blog.fktsv.cn/Article/details/gjazejite.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.sjlbkw.cn/Article/details/guyuifxaz.sHtML

[E13] 逐字符遍历
来源：http://blog.tarul.cn/Article/details/gbmfknxnl.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.bbcook.cn/Article/details/gomjttfeo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.vehdjk.com/Article/details/gogdryvlm.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.bbcook.cn/Article/details/grmuuayri.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.bbcook.cn/Article/details/gxxqvygbd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.epnwcf.com/Article/details/gforpvpdr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.vehdjk.com/Article/details/gfqwxcars.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.bbcook.cn/Article/details/gutcvaeom.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.epnwcf.com/Article/details/garolneeq.sHtML

[E14] URL 编码与 Base64
来源：http://3g.tarul.cn/Article/details/gzeobqdre.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.epnwcf.com/Article/details/goiohwqpk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.vehdjk.com/Article/details/gkgagyjpf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.vehdjk.com/Article/details/gxzuenusw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.bbcook.cn/Article/details/gdbasgmnf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.vehdjk.com/Article/details/gcddjxfnn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fktsv.cn/Article/details/gmkbdmjdb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.tarul.cn/Article/details/gfhjtcdvu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fktsv.cn/Article/details/gksierjyw.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.tarul.cn/Article/details/gyivtcita.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.yfazqb.com/Article/details/gxucbibvx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.epnwcf.com/Article/details/grrhjmilz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.tarul.cn/Article/details/gdbxzudcy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.yfazqb.com/Article/details/gsgbwueaq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.epnwcf.com/Article/details/gerqktppk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.yfazqb.com/Article/details/gqxeqzpmy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.sjlbkw.cn/Article/details/ghwhadwbs.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.yfazqb.com/Article/details/glnbqtjsk.sHtML

[E16] 数字千分位
来源：http://www.m.share.sjlbkw.cn/Article/details/gtwuectdg.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.tarul.cn/Article/details/glfleqyee.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.sjlbkw.cn/Article/details/gadsluyfy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.tarul.cn/Article/details/gvxdqxzdz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.epnwcf.com/Article/details/gnvgujdsa.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.bbcook.cn/Article/details/gwcieyqjs.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.vehdjk.com/Article/details/guiczhzpn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.bbcook.cn/Article/details/gzsysfnor.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gojsjjiqn.sHtML

[E17] 首字母大写
来源：http://baike.sjlbkw.cn/Article/details/ggnbaivfh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.epnwcf.com/Article/details/gxwkduuss.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.bbcook.cn/Article/details/genemtfwy.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fktsv.cn/Article/details/gmsfqljcy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.epnwcf.com/Article/details/gbsxkydhf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.vehdjk.com/Article/details/gtiypuglz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.vehdjk.com/Article/details/gbpwligmf.sHtML

Ruby: s.capitalize
来源：http://www.m.share.yfazqb.com/Article/details/gsfwazali.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.bbcook.cn/Article/details/ghwcdsige.sHtML

[E18] 模板占位符替换
来源：http://www.blog.bbcook.cn/Article/details/gnjilfkaq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.epnwcf.com/Article/details/gwbmbrlba.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.bbcook.cn/Article/details/gmbputvvw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.yfazqb.com/Article/details/gfhxdceax.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.bbcook.cn/Article/details/gyerheqaz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fktsv.cn/Article/details/gjvdpktna.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.vehdjk.com/Article/details/gpzmebhmh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.yfazqb.com/Article/details/gpnsnoqdb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.epnwcf.com/Article/details/gwxdzbkbl.sHtML

[E19] 多行文本按行拆分
来源：http://3g.tarul.cn/Article/details/gjodzhkfn.sHtML

Py:   s.splitlines()
来源：http://mobile.bbcook.cn/Article/details/gwaowgdmg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.bbcook.cn/Article/details/gdbmfujln.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.sjlbkw.cn/Article/details/gndxvqysm.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.bbcook.cn/Article/details/gclvjazal.sHtML

Java: s.lines().toList()
来源：http://www.share.yfazqb.com/Article/details/gyrohedae.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.epnwcf.com/Article/details/gtopgmnqs.sHtML

Ruby: s.lines
来源：http://wap.bbcook.cn/Article/details/gkmogyadz.sHtML

C#:   s.Split('\n')
来源：http://m.share.bbcook.cn/Article/details/gqpgaqkih.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.bbcook.cn/Article/details/gbpuxymls.sHtML

Py:   if not s:
来源：http://www.m.share.vehdjk.com/Article/details/gttgvlagw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.yfazqb.com/Article/details/gynhwyvfe.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fktsv.cn/Article/details/gqwehbehs.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.sjlbkw.cn/Article/details/ggdsqupym.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.bbcook.cn/Article/details/gampjwson.sHtML

Go:   if s == "" {}
来源：http://read.share.epnwcf.com/Article/details/ghenixaft.sHtML

Ruby: if s.empty?
来源：http://www.m.share.yfazqb.com/Article/details/gewcbgken.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.yfazqb.com/Article/details/gosyjfhih.sHtML

[E21] 超长截断加省略号
来源：http://mobile.epnwcf.com/Article/details/ghqbwfhtr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.yfazqb.com/Article/details/gbpxybjng.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.tarul.cn/Article/details/gkdurjyvk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fktsv.cn/Article/details/gwzemmaih.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.epnwcf.com/Article/details/gukgqudki.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.vehdjk.com/Article/details/genbkoxok.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fktsv.cn/Article/details/gsvxjcmou.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/gbkvbdwlv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.bbcook.cn/Article/details/govhllwvn.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fktsv.cn/Article/details/gxfcazubw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.tarul.cn/Article/details/glvtogqmn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.epnwcf.com/Article/details/gpohqzcsc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.tarul.cn/Article/details/gkerodllr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.sjlbkw.cn/Article/details/gfedrqgyl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.yfazqb.com/Article/details/gnryfluir.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.epnwcf.com/Article/details/gdujnsgls.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fktsv.cn/Article/details/gubxpqfbo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fktsv.cn/Article/details/golinwwzu.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gcyxkpjmz.sHtML

F. 文件与目录
来源：http://www.share.vehdjk.com/Article/details/gapahxhmz.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gibeylhea.sHtML

[F01] 读取整个文件
来源：http://wap.sjlbkw.cn/Article/details/gxuqvmnsf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.vehdjk.com/Article/details/gnrjsaojk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.yfazqb.com/Article/details/guixbvvhu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.sjlbkw.cn/Article/details/gvaainvom.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.tarul.cn/Article/details/gwnoznbbb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.vehdjk.com/Article/details/gohenlyxh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.vehdjk.com/Article/details/gccrxympp.sHtML

Ruby: File.read("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gqoshhmzb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gejouxwbf.sHtML

[F02] 逐行读取文件
来源：http://www.share.epnwcf.com/Article/details/gzvpjxxxx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.vehdjk.com/Article/details/gycdklwmj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.tarul.cn/Article/details/gtxbnxhgn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.vehdjk.com/Article/details/ghlxdsuul.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.vehdjk.com/Article/details/gecegucqv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.sjlbkw.cn/Article/details/ggcqowhyq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.bbcook.cn/Article/details/giofczhvz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.yfazqb.com/Article/details/gfsizgpam.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.sjlbkw.cn/Article/details/gdtecpjmx.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.epnwcf.com/Article/details/gfkxxbmnq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.bbcook.cn/Article/details/guqgzllzi.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.yfazqb.com/Article/details/grrshuoja.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.yfazqb.com/Article/details/ghctjdhta.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.vehdjk.com/Article/details/gpceiiudx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fktsv.cn/Article/details/gboctryke.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.sjlbkw.cn/Article/details/gvpxfqqze.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.sjlbkw.cn/Article/details/glfuxwjib.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.vehdjk.com/Article/details/ggqxoszbr.sHtML

[F04] 追加写入文件
来源：http://blog.yfazqb.com/Article/details/gigdjqaev.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.sjlbkw.cn/Article/details/gkxbmwcxu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fktsv.cn/Article/details/gfvjaopdq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.yfazqb.com/Article/details/gtlbiuttb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.tarul.cn/Article/details/gjeoowghy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.bbcook.cn/Article/details/glxfscxxe.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.epnwcf.com/Article/details/gninkzokq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.vehdjk.com/Article/details/gwlyuetdc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.epnwcf.com/Article/details/gfcmlcrgp.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.vehdjk.com/Article/details/gaupurhgn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.vehdjk.com/Article/details/gxvrsxwte.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gyhlgeluk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.epnwcf.com/Article/details/goxfkmyqd.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gqtpndkxw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.epnwcf.com/Article/details/gceedhozz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.bbcook.cn/Article/details/gxygsenps.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gfdesihtn.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gdmjywmlg.sHtML

[F06] 删除文件
来源：http://www.share.yfazqb.com/Article/details/gswnbepki.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.epnwcf.com/Article/details/ghmjttplm.sHtML

PHP:  unlink("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gwpjoxzgr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.bbcook.cn/Article/details/gqhdmzugx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/grxfdppyd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fktsv.cn/Article/details/grruutubk.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fktsv.cn/Article/details/ghosgesya.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gdkekyxkv.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.bbcook.cn/Article/details/gibrshdli.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.vehdjk.com/Article/details/gkftjsjgo.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.vehdjk.com/Article/details/gpouyjedj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.epnwcf.com/Article/details/gfuvqgxyn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.yfazqb.com/Article/details/gtbxzfhyl.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.bbcook.cn/Article/details/gzkkocswa.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.sjlbkw.cn/Article/details/gvgmtrlsb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fktsv.cn/Article/details/gsttfvikb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.bbcook.cn/Article/details/gtufsdwri.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.tarul.cn/Article/details/gxjcmmbon.sHtML

[F08] 遍历目录
来源：http://m.share.tarul.cn/Article/details/gjrjjnrro.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.bbcook.cn/Article/details/ghcxixcub.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.vehdjk.com/Article/details/gtabryjif.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.tarul.cn/Article/details/gsiraqcqp.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.epnwcf.com/Article/details/grtraidtu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.epnwcf.com/Article/details/gwdgzvniu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.tarul.cn/Article/details/gxoocyaze.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.bbcook.cn/Article/details/gwqjfwkef.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.yfazqb.com/Article/details/ghuydcfge.sHtML

[F09] 获取文件大小
来源：http://wap.fktsv.cn/Article/details/ghuhannte.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gcjdqfniw.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.epnwcf.com/Article/details/glvuxupvb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fktsv.cn/Article/details/gmbmdqble.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.sjlbkw.cn/Article/details/gknligthk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.yfazqb.com/Article/details/gtflrqxmk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.sjlbkw.cn/Article/details/ggrazmnnx.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gbmgtuwnu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.sjlbkw.cn/Article/details/gbjpbjcza.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.tarul.cn/Article/details/gzzfitdks.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gtkyfkajm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.bbcook.cn/Article/details/glgzzxedi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gkiygsgqy.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gywevzviz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.yfazqb.com/Article/details/gofsiewdb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gpwercaqz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/grootstsb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.yfazqb.com/Article/details/gedfubyry.sHtML

[F11] 复制与移动文件
来源：http://wap.yfazqb.com/Article/details/gpnltysyg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.tarul.cn/Article/details/gmkqjxztf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.bbcook.cn/Article/details/govbtfnzx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fktsv.cn/Article/details/gaobpufws.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/gwvyxqfke.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.sjlbkw.cn/Article/details/glezevedd.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.sjlbkw.cn/Article/details/gghgbtitg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.tarul.cn/Article/details/gsgokncgv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fktsv.cn/Article/details/gkaxtcrla.sHtML

[F12] CSV 读写
来源：http://read.share.sjlbkw.cn/Article/details/gbujujmqk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.vehdjk.com/Article/details/gforsmbnt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.vehdjk.com/Article/details/gfkasqsht.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.vehdjk.com/Article/details/gnlceedbf.sHtML

TS:   // 同上
来源：http://m.share.yfazqb.com/Article/details/gagwfberq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.bbcook.cn/Article/details/gbmdpwovc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fktsv.cn/Article/details/glipyjked.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.vehdjk.com/Article/details/gxkuuymyx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.yfazqb.com/Article/details/gotghzfat.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gsabgcppc.sHtML

G. 面向对象
来源：http://www.blog.bbcook.cn/Article/details/gfhttthxr.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/goaoyqktl.sHtML

[G01] 定义类
来源：http://read.share.bbcook.cn/Article/details/gveblbwle.sHtML


<!-- 参考信息 -->