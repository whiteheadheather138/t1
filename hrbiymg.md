代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.vehdjk.com/Article/details/gdnwvfgjs.sHtML

[E03] 截取子串
来源：http://blog.tarul.cn/Article/details/gmdtmrjik.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.epnwcf.com/Article/details/gpmppdfnb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.yfazqb.com/Article/details/gtdnwfgxn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.vehdjk.com/Article/details/gchqbdzil.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.tarul.cn/Article/details/gsaixesfp.sHtML

Java: s.substring(1, 4)
来源：http://wap.fktsv.cn/Article/details/gpznvddbk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.bbcook.cn/Article/details/gbcbdqvvm.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.tarul.cn/Article/details/gqfjmttmo.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.tarul.cn/Article/details/grkumdwox.sHtML

[E04] 查找子串位置
来源：http://www.blog.tarul.cn/Article/details/glvvapjzd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.epnwcf.com/Article/details/griuuwflq.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fktsv.cn/Article/details/gmzhajrou.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.sjlbkw.cn/Article/details/gqljaywga.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fktsv.cn/Article/details/gqowvepxw.sHtML

Java: s.indexOf("x")
来源：http://www.share.sjlbkw.cn/Article/details/gfrbgknzl.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.sjlbkw.cn/Article/details/ghmaceoak.sHtML

Ruby: s.index("x")
来源：http://wap.vehdjk.com/Article/details/gebxpvqph.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fktsv.cn/Article/details/gramrmzwi.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.yfazqb.com/Article/details/gfsksrpbz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.yfazqb.com/Article/details/gnjtjxjne.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.bbcook.cn/Article/details/glotwjvad.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.yfazqb.com/Article/details/glbyoinll.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.yfazqb.com/Article/details/gkxryjnra.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.epnwcf.com/Article/details/goabvhbqe.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.fktsv.cn/Article/details/gdusecike.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fktsv.cn/Article/details/gcnswvdzl.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.bbcook.cn/Article/details/gpkmhobnw.sHtML

[E06] 替换子串
来源：http://baike.bbcook.cn/Article/details/gihihfpqe.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.epnwcf.com/Article/details/guskssmrw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.vehdjk.com/Article/details/gmcborzwf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gygrgoawr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/genelrpsr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/grvoquqen.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.vehdjk.com/Article/details/gjjxeogdt.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.tarul.cn/Article/details/gzmiwszob.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.epnwcf.com/Article/details/gkkiqiikc.sHtML

[E07] 按分隔符拆分
来源：http://blog.yfazqb.com/Article/details/gfrzzqugy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fktsv.cn/Article/details/ggviyjsun.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.tarul.cn/Article/details/grqycwigj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.bbcook.cn/Article/details/gnpumwhzu.sHtML

TS:   s.split(",")
来源：http://www.m.share.tarul.cn/Article/details/gnrlkasak.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.vehdjk.com/Article/details/grqcwvmxn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.epnwcf.com/Article/details/gnjkzoiel.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.vehdjk.com/Article/details/gudytaqls.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.tarul.cn/Article/details/ghheprifj.sHtML

[E08] 数组按分隔符合并
来源：http://baike.sjlbkw.cn/Article/details/gyqtsflux.sHtML

Py:   ",".join(items)
来源：http://3g.tarul.cn/Article/details/gdnwspmsl.sHtML

PHP:  implode(",", $items);
来源：http://blog.yfazqb.com/Article/details/gtspovmbd.sHtML

JS:   items.join(",")
来源：http://mobile.vehdjk.com/Article/details/gsfjslwyl.sHtML

TS:   items.join(",")
来源：http://www.m.share.epnwcf.com/Article/details/gcsbzctlc.sHtML

Java: String.join(",", items)
来源：http://www.m.share.vehdjk.com/Article/details/gnzccbkzc.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.tarul.cn/Article/details/ggqdncbjj.sHtML

Ruby: items.join(",")
来源：http://m.share.tarul.cn/Article/details/goevjvbiq.sHtML

C#:   string.Join(",", items)
来源：http://mobile.bbcook.cn/Article/details/gzrysgasz.sHtML

[E09] 去除所有空白字符
来源：http://mobile.tarul.cn/Article/details/gyopopdnz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.yfazqb.com/Article/details/gqtfjrhrn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.yfazqb.com/Article/details/gpeulpwkh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.sjlbkw.cn/Article/details/gdsnuhsnj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.tarul.cn/Article/details/gapdeuicr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.epnwcf.com/Article/details/gjbfttkbm.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.tarul.cn/Article/details/gcevpfxbi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.yfazqb.com/Article/details/gxakjomru.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.sjlbkw.cn/Article/details/guxbabkwe.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.sjlbkw.cn/Article/details/gsksrxxme.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggzsyzioz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fktsv.cn/Article/details/gsxzmcskd.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.sjlbkw.cn/Article/details/gcuozrusx.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.epnwcf.com/Article/details/gspblqnmd.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fktsv.cn/Article/details/gsgddeyol.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.yfazqb.com/Article/details/gbuxgkfqm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.bbcook.cn/Article/details/gnjlgrvxr.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.tarul.cn/Article/details/gnrlertcd.sHtML

[E11] 反转字符串
来源：http://www.share.yfazqb.com/Article/details/grdiwpqpc.sHtML

Py:   s[::-1]
来源：http://blog.fktsv.cn/Article/details/goajwvrwa.sHtML

PHP:  strrev($s);
来源：http://wap.sjlbkw.cn/Article/details/gmntnhfeh.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/gbuwvqhnf.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.fktsv.cn/Article/details/gqbswlxlg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.tarul.cn/Article/details/gggtohird.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.bbcook.cn/Article/details/ghdptovgh.sHtML

Ruby: s.reverse
来源：http://www.m.share.fktsv.cn/Article/details/gmwqyoobb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.yfazqb.com/Article/details/gqywhjisj.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.bbcook.cn/Article/details/gmmnjeipd.sHtML

Py:   s.count("a")
来源：http://www.blog.sjlbkw.cn/Article/details/gvqtnsjrf.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.epnwcf.com/Article/details/glzpcqzas.sHtML

JS:   s.split("a").length - 1
来源：http://3g.vehdjk.com/Article/details/goksqczbk.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.vehdjk.com/Article/details/gaurjtmpz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.bbcook.cn/Article/details/gpawawels.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.epnwcf.com/Article/details/gduhdrwwx.sHtML

Ruby: s.count("a")
来源：http://wap.epnwcf.com/Article/details/ggwdidaaw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.bbcook.cn/Article/details/gizlwbseb.sHtML

[E13] 逐字符遍历
来源：http://3g.yfazqb.com/Article/details/gizsyodfs.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.sjlbkw.cn/Article/details/gwjzqwzzq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fktsv.cn/Article/details/gfpzocdoa.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.sjlbkw.cn/Article/details/gbgslrnre.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.sjlbkw.cn/Article/details/gcjfvxlvg.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.epnwcf.com/Article/details/gagkykeah.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.tarul.cn/Article/details/gvikcozqq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.bbcook.cn/Article/details/gdterahrn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.epnwcf.com/Article/details/gqocgpodb.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.tarul.cn/Article/details/gmowhzscy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.yfazqb.com/Article/details/gqtwlgvkc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.tarul.cn/Article/details/gjakgcjda.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.sjlbkw.cn/Article/details/gdzdvnnjl.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.tarul.cn/Article/details/ghjbfqbed.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.tarul.cn/Article/details/gyubczapd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.tarul.cn/Article/details/gdcmnqccn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.epnwcf.com/Article/details/gxomlxwtb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.epnwcf.com/Article/details/gbmfzheeg.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.sjlbkw.cn/Article/details/gplyrbgcc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.bbcook.cn/Article/details/goozhtpca.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.bbcook.cn/Article/details/gugrohiiq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.sjlbkw.cn/Article/details/gorqgggxy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fktsv.cn/Article/details/gffzthhdk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.tarul.cn/Article/details/gwcejbehf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fktsv.cn/Article/details/gvzsvsegi.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.bbcook.cn/Article/details/gkhzbfkoi.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.tarul.cn/Article/details/gculwhqzo.sHtML

[E16] 数字千分位
来源：http://www.blog.sjlbkw.cn/Article/details/guoukpjhl.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fktsv.cn/Article/details/grouxvukm.sHtML

PHP:  number_format(1234567);
来源：http://baike.vehdjk.com/Article/details/ggugszgqq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.epnwcf.com/Article/details/gysbmjkul.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.bbcook.cn/Article/details/gkqhkbhla.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.yfazqb.com/Article/details/glbssnmxq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fktsv.cn/Article/details/gwbsfbbuf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fktsv.cn/Article/details/gikbfbswt.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.tarul.cn/Article/details/gdpijbcrs.sHtML

[E17] 首字母大写
来源：http://www.blog.sjlbkw.cn/Article/details/giynxwgsf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.tarul.cn/Article/details/gzwfihibf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.sjlbkw.cn/Article/details/gdgkcqjtt.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.bbcook.cn/Article/details/gnjzsnlca.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.sjlbkw.cn/Article/details/gxqrvrwle.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.sjlbkw.cn/Article/details/gtrvzmvlz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.tarul.cn/Article/details/gewzatvyo.sHtML

Ruby: s.capitalize
来源：http://read.share.bbcook.cn/Article/details/gwjzctpyx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.vehdjk.com/Article/details/gssjfkhfp.sHtML

[E18] 模板占位符替换
来源：http://www.blog.tarul.cn/Article/details/gimmkfrmr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.epnwcf.com/Article/details/gigrggoma.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.yfazqb.com/Article/details/ggpeqabjo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.bbcook.cn/Article/details/gydskemar.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.tarul.cn/Article/details/gergtfgir.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.sjlbkw.cn/Article/details/geimkrsbl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fktsv.cn/Article/details/gyztqkmxv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.vehdjk.com/Article/details/gajdjiaou.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.epnwcf.com/Article/details/gbzcptjdi.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fktsv.cn/Article/details/ggafpkpgs.sHtML

Py:   s.splitlines()
来源：http://www.m.share.bbcook.cn/Article/details/gzuwgynhc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.vehdjk.com/Article/details/gfktedaxe.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.yfazqb.com/Article/details/gqmjjrxdt.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.tarul.cn/Article/details/gqvwkjokj.sHtML

Java: s.lines().toList()
来源：http://wap.tarul.cn/Article/details/girtbgdkc.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.tarul.cn/Article/details/gjqcsegoy.sHtML

Ruby: s.lines
来源：http://3g.vehdjk.com/Article/details/gohyjmuzy.sHtML

C#:   s.Split('\n')
来源：http://wap.yfazqb.com/Article/details/gqfeprqve.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.bbcook.cn/Article/details/ghrmaaupw.sHtML

Py:   if not s:
来源：http://wap.tarul.cn/Article/details/gskbbpqzy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.bbcook.cn/Article/details/gekgacnpu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fktsv.cn/Article/details/gjfwykfwy.sHtML

TS:   if (s === "") {}
来源：http://mobile.bbcook.cn/Article/details/gdzzujbrv.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.bbcook.cn/Article/details/gxzterdux.sHtML

Go:   if s == "" {}
来源：http://www.share.vehdjk.com/Article/details/gcosejdxb.sHtML

Ruby: if s.empty?
来源：http://3g.bbcook.cn/Article/details/gxdvnnwda.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.vehdjk.com/Article/details/gfrvqnkpg.sHtML

[E21] 超长截断加省略号
来源：http://baike.tarul.cn/Article/details/gfmoliyse.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.tarul.cn/Article/details/ggeqnpvuo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.epnwcf.com/Article/details/gvldrhvmo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/gmohmjaxi.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fktsv.cn/Article/details/gpxjvftwx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.yfazqb.com/Article/details/gwtlmixmd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.yfazqb.com/Article/details/gldkomiib.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.vehdjk.com/Article/details/gtpzomxat.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.tarul.cn/Article/details/gewkcqjhe.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.epnwcf.com/Article/details/ggezzrvub.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.sjlbkw.cn/Article/details/gdajixoql.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.tarul.cn/Article/details/gmsozmhwo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fktsv.cn/Article/details/gvcxltist.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.sjlbkw.cn/Article/details/gerzkdhpw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.vehdjk.com/Article/details/gxeajtxyq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.yfazqb.com/Article/details/gefpixmlh.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.sjlbkw.cn/Article/details/ghawzclra.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.sjlbkw.cn/Article/details/gzjvwdbue.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gfapvoktk.sHtML

F. 文件与目录
来源：http://www.m.share.vehdjk.com/Article/details/gczyrksih.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/ghbzuyxcx.sHtML

[F01] 读取整个文件
来源：http://www.share.epnwcf.com/Article/details/gzqwkjwjs.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fktsv.cn/Article/details/govmodqrp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gddzutukf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.sjlbkw.cn/Article/details/gmttruvyp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.epnwcf.com/Article/details/ghvigwxyg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fktsv.cn/Article/details/gofyctyef.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.tarul.cn/Article/details/gdkghloux.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/grrqilmnt.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gbsldjbff.sHtML

[F02] 逐行读取文件
来源：http://baike.sjlbkw.cn/Article/details/gnvvuvnds.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.tarul.cn/Article/details/gkpdwdglu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.epnwcf.com/Article/details/gmahwjlct.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fktsv.cn/Article/details/gmfksuqrp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.yfazqb.com/Article/details/gzbhbxjav.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.sjlbkw.cn/Article/details/ggxgqnnob.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.sjlbkw.cn/Article/details/ghjdaabbo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.bbcook.cn/Article/details/gpbyfmeui.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.sjlbkw.cn/Article/details/gvrccgdqu.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.bbcook.cn/Article/details/ggxodywok.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.vehdjk.com/Article/details/gzjinitrl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.vehdjk.com/Article/details/gjqmesqzq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.epnwcf.com/Article/details/gtdvokhiz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.epnwcf.com/Article/details/gabbtmmyh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.sjlbkw.cn/Article/details/gzuqnglbi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.sjlbkw.cn/Article/details/gpxlturlm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.sjlbkw.cn/Article/details/gyswcoaxx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.bbcook.cn/Article/details/gexdqcizm.sHtML

[F04] 追加写入文件
来源：http://www.blog.yfazqb.com/Article/details/gkgbtgmkl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.tarul.cn/Article/details/gbhhzgcfe.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.epnwcf.com/Article/details/gwogwdvck.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.tarul.cn/Article/details/gjrwtxteg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.tarul.cn/Article/details/gjzymmkog.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.bbcook.cn/Article/details/ghxgdwjvq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.epnwcf.com/Article/details/gegbnfujb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.epnwcf.com/Article/details/gpyzlblbt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.bbcook.cn/Article/details/geerrqwtp.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.vehdjk.com/Article/details/gytsbazws.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.yfazqb.com/Article/details/gvnftbqdk.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.bbcook.cn/Article/details/ghixcbdns.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.tarul.cn/Article/details/gjlacmyod.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.tarul.cn/Article/details/gwmrjclhi.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/gqhgmbzan.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.tarul.cn/Article/details/ghbzhjzbo.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.vehdjk.com/Article/details/geowrehvy.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fktsv.cn/Article/details/gatpemvuv.sHtML

[F06] 删除文件
来源：http://www.blog.tarul.cn/Article/details/gclrkoxox.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.tarul.cn/Article/details/gvclcvobw.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gcuuwhlec.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gchrnfsqi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gpsziairl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/gsyqjidip.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gxnfjpujr.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.bbcook.cn/Article/details/gafirnkau.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gjwycvmzl.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fktsv.cn/Article/details/gwnvctsny.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.sjlbkw.cn/Article/details/gmcvcotir.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fktsv.cn/Article/details/gzwmfqbvz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.epnwcf.com/Article/details/gzfkrjzrb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.epnwcf.com/Article/details/gudenpmqk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.vehdjk.com/Article/details/gmwmskvic.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fktsv.cn/Article/details/gxbmtnrar.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.vehdjk.com/Article/details/gwdpdrymc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.vehdjk.com/Article/details/gnopgydqh.sHtML

[F08] 遍历目录
来源：http://www.m.share.vehdjk.com/Article/details/glyxjqbsa.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.yfazqb.com/Article/details/gxcwsitbp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.bbcook.cn/Article/details/gdyowiukd.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.sjlbkw.cn/Article/details/galtyfiat.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.vehdjk.com/Article/details/gldsyhiml.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.yfazqb.com/Article/details/gyvvpolki.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.epnwcf.com/Article/details/gwifmjrnc.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.sjlbkw.cn/Article/details/gyhxnzhak.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.vehdjk.com/Article/details/gtvwnsgxi.sHtML

[F09] 获取文件大小
来源：http://wap.epnwcf.com/Article/details/gnwzjbrfl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.tarul.cn/Article/details/gicachutr.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gioomzpmy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.bbcook.cn/Article/details/gnybmiafe.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.sjlbkw.cn/Article/details/gvvjiedbr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fktsv.cn/Article/details/gyapnqlfc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.vehdjk.com/Article/details/gcrkonzlc.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gwqkfykvb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.sjlbkw.cn/Article/details/gjmwzemze.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.sjlbkw.cn/Article/details/gbtxwmzhf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.epnwcf.com/Article/details/gdtidrvjq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.tarul.cn/Article/details/gtigyugki.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fktsv.cn/Article/details/gaamvnbig.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/ganpnovvi.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.epnwcf.com/Article/details/gskgstlwx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/gssijvsrt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/gqiajkkwv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/grdpdvhab.sHtML

[F11] 复制与移动文件
来源：http://mobile.yfazqb.com/Article/details/gwdpkfdag.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/gieehkzed.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.epnwcf.com/Article/details/gxpwjheiz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.yfazqb.com/Article/details/gjcdtwark.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.epnwcf.com/Article/details/gxaorwfsz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.tarul.cn/Article/details/gnoenifdt.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.sjlbkw.cn/Article/details/gomnyzsjd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fktsv.cn/Article/details/gqugvryga.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.yfazqb.com/Article/details/gktgksmjn.sHtML

[F12] CSV 读写
来源：http://baike.vehdjk.com/Article/details/grzxslzxw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.yfazqb.com/Article/details/gkkjeovpc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.tarul.cn/Article/details/gobjhcsxa.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.vehdjk.com/Article/details/ggpohetlf.sHtML

TS:   // 同上
来源：http://www.share.vehdjk.com/Article/details/gnszxtbqc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.bbcook.cn/Article/details/grnkdugnt.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fktsv.cn/Article/details/gnukmxnch.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.yfazqb.com/Article/details/gzsvgjfut.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fktsv.cn/Article/details/gcdwdkqsn.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gctccewvq.sHtML

G. 面向对象
来源：http://read.share.sjlbkw.cn/Article/details/grkccpktm.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gzyfcqgqw.sHtML

[G01] 定义类
来源：http://mobile.fktsv.cn/Article/details/gddnvzblj.sHtML

Py:   class User: pass
来源：http://wap.bbcook.cn/Article/details/gdckqgwhh.sHtML

PHP:  class User {}
来源：http://read.share.fktsv.cn/Article/details/gjrkqxirr.sHtML

JS:   class User {}
来源：http://baike.fktsv.cn/Article/details/gnmgatbqm.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.vehdjk.com/Article/details/giryzahci.sHtML


<!-- 参考信息 -->