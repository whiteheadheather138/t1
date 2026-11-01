代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.tarul.cn/Article/details/gxouzlnfg.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fktsv.cn/Article/details/gnddgbuxf.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.tarul.cn/Article/details/gtyjykhyk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.bbcook.cn/Article/details/gjbsfusqs.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.tarul.cn/Article/details/gznvcfecx.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.yfazqb.com/Article/details/getvsvakg.sHtML

[E04] 查找子串位置
来源：http://read.share.bbcook.cn/Article/details/gltezgghs.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fktsv.cn/Article/details/gltkpdzbk.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.bbcook.cn/Article/details/gqipsoldb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.tarul.cn/Article/details/gmavbjpyi.sHtML

TS:   s.indexOf("x")
来源：http://3g.vehdjk.com/Article/details/gkvyshphz.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.sjlbkw.cn/Article/details/geyulelqt.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.fktsv.cn/Article/details/gulfcxcve.sHtML

Ruby: s.index("x")
来源：http://3g.bbcook.cn/Article/details/gxxwqmmnn.sHtML

C#:   s.IndexOf("x")
来源：http://wap.bbcook.cn/Article/details/gzftqizqy.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.sjlbkw.cn/Article/details/gjeewlbig.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.yfazqb.com/Article/details/gdieulcuo.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.yfazqb.com/Article/details/gmtayrcrh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.tarul.cn/Article/details/gnftwwjfr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.tarul.cn/Article/details/gyefamlxm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.vehdjk.com/Article/details/gbqhgjezs.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fktsv.cn/Article/details/gjgujorhc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fktsv.cn/Article/details/gqbbxugnt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fktsv.cn/Article/details/gldfkcavv.sHtML

[E06] 替换子串
来源：http://wap.fktsv.cn/Article/details/gvshvbexn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.sjlbkw.cn/Article/details/ghucemhuq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.bbcook.cn/Article/details/gqicfroah.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.tarul.cn/Article/details/glvpwlfqa.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.bbcook.cn/Article/details/gvotmudyu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.tarul.cn/Article/details/gxczdspve.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.epnwcf.com/Article/details/gweuyoghg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/ggdbgbfey.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.vehdjk.com/Article/details/gjxknxpkj.sHtML

[E07] 按分隔符拆分
来源：http://baike.bbcook.cn/Article/details/gizgwdktq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.bbcook.cn/Article/details/ggcfepqbe.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.yfazqb.com/Article/details/gmykxvwrf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fktsv.cn/Article/details/grzpqvrmk.sHtML

TS:   s.split(",")
来源：http://read.share.fktsv.cn/Article/details/gflpwqfcf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.vehdjk.com/Article/details/gmzgsiwqq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.bbcook.cn/Article/details/gxewxxqjb.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.bbcook.cn/Article/details/gchrydrpf.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fktsv.cn/Article/details/giajctpxg.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.yfazqb.com/Article/details/gzecvuxzj.sHtML

Py:   ",".join(items)
来源：http://blog.epnwcf.com/Article/details/gfjsbawsl.sHtML

PHP:  implode(",", $items);
来源：http://m.share.yfazqb.com/Article/details/gkomluhfm.sHtML

JS:   items.join(",")
来源：http://wap.yfazqb.com/Article/details/gxtbudzcf.sHtML

TS:   items.join(",")
来源：http://read.share.vehdjk.com/Article/details/gapywiqcg.sHtML

Java: String.join(",", items)
来源：http://www.blog.vehdjk.com/Article/details/gqizufnzn.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.tarul.cn/Article/details/gjxbtgudh.sHtML

Ruby: items.join(",")
来源：http://blog.epnwcf.com/Article/details/gdudsdjaz.sHtML

C#:   string.Join(",", items)
来源：http://wap.yfazqb.com/Article/details/gzhiubytk.sHtML

[E09] 去除所有空白字符
来源：http://baike.vehdjk.com/Article/details/gredbmyqv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.epnwcf.com/Article/details/giiswwudd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.bbcook.cn/Article/details/gzelfyasd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.yfazqb.com/Article/details/gxxbuvvdy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.tarul.cn/Article/details/gpshzzcqp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.bbcook.cn/Article/details/gynezfhjv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.tarul.cn/Article/details/gwwhozeea.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.bbcook.cn/Article/details/gqzvspwkv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.bbcook.cn/Article/details/gbbkgcgxx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fktsv.cn/Article/details/guhshezvd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.yfazqb.com/Article/details/gfrtdchzo.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fktsv.cn/Article/details/gxsrskguc.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fktsv.cn/Article/details/gxagcptuq.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.epnwcf.com/Article/details/gbaarqtof.sHtML

Java: String.format("%03d", 7)
来源：http://baike.tarul.cn/Article/details/gapaljlsh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.vehdjk.com/Article/details/gwqmdfcqz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.tarul.cn/Article/details/gburdlnun.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.bbcook.cn/Article/details/grgodnkzk.sHtML

[E11] 反转字符串
来源：http://www.m.share.yfazqb.com/Article/details/gbatypsbf.sHtML

Py:   s[::-1]
来源：http://www.share.tarul.cn/Article/details/grcjsmquf.sHtML

PHP:  strrev($s);
来源：http://read.share.epnwcf.com/Article/details/gxahncdcw.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.epnwcf.com/Article/details/gjuymzexc.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/gvknklnwb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.yfazqb.com/Article/details/gyavcfzbh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fktsv.cn/Article/details/gfcadeidh.sHtML

Ruby: s.reverse
来源：http://mobile.fktsv.cn/Article/details/glzbapbmi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.yfazqb.com/Article/details/gpwodpajw.sHtML

[E12] 统计某字符出现次数
来源：http://3g.tarul.cn/Article/details/glszgnbhx.sHtML

Py:   s.count("a")
来源：http://3g.fktsv.cn/Article/details/gnqbfxnoq.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.yfazqb.com/Article/details/gctiszbit.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.tarul.cn/Article/details/ghjtjbwyp.sHtML

TS:   s.split("a").length - 1
来源：http://3g.tarul.cn/Article/details/gtdvwqsjd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.sjlbkw.cn/Article/details/gblatwget.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.bbcook.cn/Article/details/gcqscdjfz.sHtML

Ruby: s.count("a")
来源：http://www.m.share.vehdjk.com/Article/details/gsjlydtjc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.tarul.cn/Article/details/gqujsdeor.sHtML

[E13] 逐字符遍历
来源：http://3g.bbcook.cn/Article/details/giykwlkxi.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.bbcook.cn/Article/details/gsmwnvpsu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fktsv.cn/Article/details/gmxsncaxk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.sjlbkw.cn/Article/details/gxehakaob.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.vehdjk.com/Article/details/gexjeekgd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.vehdjk.com/Article/details/gwgwhodyk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.vehdjk.com/Article/details/gxlnmwryw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.tarul.cn/Article/details/gbpkmzxdw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.epnwcf.com/Article/details/gigilqxcs.sHtML

[E14] URL 编码与 Base64
来源：http://blog.vehdjk.com/Article/details/gwctyymbf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.vehdjk.com/Article/details/gjtjurtvd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.bbcook.cn/Article/details/ghwjvkrst.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.epnwcf.com/Article/details/gmsphurap.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.bbcook.cn/Article/details/geszwwptc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.tarul.cn/Article/details/gpbstzoem.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.vehdjk.com/Article/details/geudmusvv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.bbcook.cn/Article/details/ghtfzbiwz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fktsv.cn/Article/details/gnllxhpic.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.yfazqb.com/Article/details/gelmtfcon.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.vehdjk.com/Article/details/gldbiodmj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.tarul.cn/Article/details/givvysxmv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.bbcook.cn/Article/details/gqrnibppv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fktsv.cn/Article/details/gjkhurvnk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.tarul.cn/Article/details/gmhvszbcm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.sjlbkw.cn/Article/details/gbjwrgpuj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.epnwcf.com/Article/details/gjcuoatdd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.vehdjk.com/Article/details/gkpdvytva.sHtML

[E16] 数字千分位
来源：http://blog.bbcook.cn/Article/details/gyhkyolpt.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.epnwcf.com/Article/details/gpfxnoaqg.sHtML

PHP:  number_format(1234567);
来源：http://wap.sjlbkw.cn/Article/details/guxqogppp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fktsv.cn/Article/details/gotxvesut.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.yfazqb.com/Article/details/gdtdmrhzl.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.epnwcf.com/Article/details/gmrozksjm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.sjlbkw.cn/Article/details/gsmshvknl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fktsv.cn/Article/details/gnmtkelvf.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.epnwcf.com/Article/details/gazgfazeh.sHtML

[E17] 首字母大写
来源：http://www.m.share.fktsv.cn/Article/details/gwdxrfirm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.bbcook.cn/Article/details/getiaixqx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.sjlbkw.cn/Article/details/ggoirgznz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fktsv.cn/Article/details/gsxxwctfl.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.yfazqb.com/Article/details/gsadweixr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.yfazqb.com/Article/details/gsydhprkv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.tarul.cn/Article/details/gjjkbzpav.sHtML

Ruby: s.capitalize
来源：http://read.share.tarul.cn/Article/details/gepcgfppw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.sjlbkw.cn/Article/details/gnmsdlxrg.sHtML

[E18] 模板占位符替换
来源：http://m.share.sjlbkw.cn/Article/details/gsoqivvpk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.sjlbkw.cn/Article/details/gruzazibp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.yfazqb.com/Article/details/gchlpejnj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fktsv.cn/Article/details/gbpiulsxt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.epnwcf.com/Article/details/gvkqorjhy.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.sjlbkw.cn/Article/details/gfktkygil.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.yfazqb.com/Article/details/gamcjtpup.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.yfazqb.com/Article/details/gekouvrpe.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.sjlbkw.cn/Article/details/gkbzlenut.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.vehdjk.com/Article/details/gxjtqfmjg.sHtML

Py:   s.splitlines()
来源：http://read.share.vehdjk.com/Article/details/ggaskxqpb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.sjlbkw.cn/Article/details/gyzbbfhny.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.vehdjk.com/Article/details/gzhqadrqa.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.bbcook.cn/Article/details/gkrgfadki.sHtML

Java: s.lines().toList()
来源：http://baike.fktsv.cn/Article/details/gfxtefuon.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.bbcook.cn/Article/details/gpcdggqrc.sHtML

Ruby: s.lines
来源：http://baike.vehdjk.com/Article/details/guwhbkxct.sHtML

C#:   s.Split('\n')
来源：http://read.share.bbcook.cn/Article/details/gfbodnbgs.sHtML

[E20] 判断字符串是否为空
来源：http://baike.yfazqb.com/Article/details/gdgsphbbf.sHtML

Py:   if not s:
来源：http://3g.epnwcf.com/Article/details/gjtknafou.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fktsv.cn/Article/details/gdgoshvjd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.epnwcf.com/Article/details/gdlnkzzeq.sHtML

TS:   if (s === "") {}
来源：http://www.blog.epnwcf.com/Article/details/gufzankri.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.epnwcf.com/Article/details/gvtsmhyoj.sHtML

Go:   if s == "" {}
来源：http://mobile.vehdjk.com/Article/details/gromnbgzd.sHtML

Ruby: if s.empty?
来源：http://baike.yfazqb.com/Article/details/gzdeibhhl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.bbcook.cn/Article/details/gymkznbhd.sHtML

[E21] 超长截断加省略号
来源：http://blog.epnwcf.com/Article/details/gbcijhazb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.vehdjk.com/Article/details/gttexdhbi.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.vehdjk.com/Article/details/gycxbofgb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gsnvmyfrv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fktsv.cn/Article/details/ggwlzqlxv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.sjlbkw.cn/Article/details/gzbvfpppy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.bbcook.cn/Article/details/gorlhqcrq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.epnwcf.com/Article/details/gphttijhn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fktsv.cn/Article/details/gbimqjzxn.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.tarul.cn/Article/details/glxxhzyub.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.epnwcf.com/Article/details/gsjsgcljr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.bbcook.cn/Article/details/gslxihhov.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.tarul.cn/Article/details/ggdtaizwz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.tarul.cn/Article/details/gnhdjvvzx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.yfazqb.com/Article/details/gpaevfgvx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.sjlbkw.cn/Article/details/garwxcgvl.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fktsv.cn/Article/details/gnicmxylc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.epnwcf.com/Article/details/gouvjnwfo.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gbchpbgpt.sHtML

F. 文件与目录
来源：http://3g.epnwcf.com/Article/details/grjgsrorg.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gffoboowc.sHtML

[F01] 读取整个文件
来源：http://baike.yfazqb.com/Article/details/ghtpymddh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.bbcook.cn/Article/details/goelnyuzh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.tarul.cn/Article/details/gtdufaggj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.vehdjk.com/Article/details/gdozexron.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.bbcook.cn/Article/details/gzgkgcbpd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.tarul.cn/Article/details/gwgwecukh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.epnwcf.com/Article/details/gnzzwkicj.sHtML

Ruby: File.read("a.txt")
来源：http://baike.vehdjk.com/Article/details/ggnklavbs.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/ggvtsrkmc.sHtML

[F02] 逐行读取文件
来源：http://blog.tarul.cn/Article/details/guhbmktvj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fktsv.cn/Article/details/glenqcshf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.yfazqb.com/Article/details/gasvfsjor.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.tarul.cn/Article/details/gumfzbyia.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fktsv.cn/Article/details/gcmrtmsul.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fktsv.cn/Article/details/ghkvnsldo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.tarul.cn/Article/details/gqxqwxihw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.vehdjk.com/Article/details/glsngbjsb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.sjlbkw.cn/Article/details/gugcmcuto.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.bbcook.cn/Article/details/ghxfoduzj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.yfazqb.com/Article/details/gytkuflod.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fktsv.cn/Article/details/gqupappvb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fktsv.cn/Article/details/gfckmxujg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fktsv.cn/Article/details/gbjljnwkl.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.bbcook.cn/Article/details/geoczdgzh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.sjlbkw.cn/Article/details/galrvcopt.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.tarul.cn/Article/details/gfwjwhygd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.tarul.cn/Article/details/gfiesaxhs.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fktsv.cn/Article/details/gkbdcgndt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.vehdjk.com/Article/details/gpfakcaoy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.epnwcf.com/Article/details/gdszficqm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.yfazqb.com/Article/details/gsombzsjv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.vehdjk.com/Article/details/gaxvhpnqp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.yfazqb.com/Article/details/grxkxptos.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.tarul.cn/Article/details/gjvprttng.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.sjlbkw.cn/Article/details/gvbhlgzhn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.epnwcf.com/Article/details/gfupdlafh.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.epnwcf.com/Article/details/giuijqxbi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.epnwcf.com/Article/details/gbcxkzdtn.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gxvdqeckv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gwobroshi.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gwqoafbkk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.yfazqb.com/Article/details/gkagrhjot.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.yfazqb.com/Article/details/gndttwddt.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.yfazqb.com/Article/details/grrxrqvnk.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gcyeskarr.sHtML

[F06] 删除文件
来源：http://baike.fktsv.cn/Article/details/gaqbbdssn.sHtML

Py:   os.remove("a.txt")
来源：http://3g.bbcook.cn/Article/details/gqahfgvos.sHtML

PHP:  unlink("a.txt");
来源：http://baike.yfazqb.com/Article/details/gwcaawgnw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gzpurtarb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gshjqaliq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.vehdjk.com/Article/details/gjthvchnt.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.tarul.cn/Article/details/ghemfedve.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.yfazqb.com/Article/details/gxtimnhwl.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fktsv.cn/Article/details/gnjngetmz.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.sjlbkw.cn/Article/details/gvoqidbmf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.sjlbkw.cn/Article/details/gsxttyhtd.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.yfazqb.com/Article/details/gicysybne.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.yfazqb.com/Article/details/gamotsjtp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.yfazqb.com/Article/details/gdmbhgdpv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.vehdjk.com/Article/details/grsnjahrm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.vehdjk.com/Article/details/gdeamchuw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.yfazqb.com/Article/details/gjlwgtdjr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.vehdjk.com/Article/details/gsqngiqzw.sHtML

[F08] 遍历目录
来源：http://baike.epnwcf.com/Article/details/gasfesigs.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.yfazqb.com/Article/details/gdjjyvyuj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.vehdjk.com/Article/details/gmirjwkqw.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fktsv.cn/Article/details/ggsrfnsqm.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.sjlbkw.cn/Article/details/grdhdeyip.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.vehdjk.com/Article/details/gbkpfedyb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.vehdjk.com/Article/details/gcxqlcerz.sHtML

Ruby: Dir.children("dir")
来源：http://baike.vehdjk.com/Article/details/gcbkiwapr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.bbcook.cn/Article/details/ggfaadgfa.sHtML

[F09] 获取文件大小
来源：http://www.m.share.epnwcf.com/Article/details/gnnpbqjxt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gcrgwteur.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.tarul.cn/Article/details/gfmiqrusw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.tarul.cn/Article/details/gfobsqkhe.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fktsv.cn/Article/details/gmsbrjzjn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.vehdjk.com/Article/details/gpltfuakm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.bbcook.cn/Article/details/gcoaouecd.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gwykgdkts.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.tarul.cn/Article/details/glmxsmbmn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.yfazqb.com/Article/details/gmuacknyq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gnqcqvzdz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.yfazqb.com/Article/details/gfxztjztg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/gpiitvvwb.sHtML

TS:   path.extname("a.txt")
来源：http://3g.epnwcf.com/Article/details/gvqaoztal.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.tarul.cn/Article/details/grvesfqgz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gibhluzse.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/gkrziwnes.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/gzgnumybs.sHtML

[F11] 复制与移动文件
来源：http://baike.bbcook.cn/Article/details/gnosyydav.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.tarul.cn/Article/details/gcmnxqvjs.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.yfazqb.com/Article/details/gybfxnybj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fktsv.cn/Article/details/gspfmjyfc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gcxhiryrg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.yfazqb.com/Article/details/gsqmcyzec.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fktsv.cn/Article/details/gyayqbjqe.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.vehdjk.com/Article/details/gcbuogkui.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.vehdjk.com/Article/details/gafwfbsfm.sHtML

[F12] CSV 读写
来源：http://3g.fktsv.cn/Article/details/gnyqmpcpf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.vehdjk.com/Article/details/gqaedyldd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.sjlbkw.cn/Article/details/gfxjnznlr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.sjlbkw.cn/Article/details/gymxfegss.sHtML

TS:   // 同上
来源：http://baike.epnwcf.com/Article/details/guncorxjs.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.epnwcf.com/Article/details/gszitnvpr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.yfazqb.com/Article/details/gsmzmyzlu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.sjlbkw.cn/Article/details/gfihxmnoj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.sjlbkw.cn/Article/details/gbcudjqlq.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gcyhbplsw.sHtML

G. 面向对象
来源：http://mobile.yfazqb.com/Article/details/ghbcntbzu.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gegxpxcot.sHtML

[G01] 定义类
来源：http://www.share.vehdjk.com/Article/details/gmpgvnpvx.sHtML

Py:   class User: pass
来源：http://www.blog.yfazqb.com/Article/details/gahvixdnf.sHtML

PHP:  class User {}
来源：http://www.blog.fktsv.cn/Article/details/gbtwlvmbb.sHtML

JS:   class User {}
来源：http://wap.sjlbkw.cn/Article/details/gsropjqdf.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.vehdjk.com/Article/details/gmocpjrvy.sHtML

Java: class User {}
来源：http://mobile.sjlbkw.cn/Article/details/gfoazmhie.sHtML

Go:   type User struct { Name string }
来源：http://3g.tarul.cn/Article/details/giivdxzms.sHtML

Ruby: class User; end
来源：http://mobile.tarul.cn/Article/details/geparnfaz.sHtML

C#:   class User {}
来源：http://m.share.fktsv.cn/Article/details/gujwylfal.sHtML


<!-- 参考信息 -->