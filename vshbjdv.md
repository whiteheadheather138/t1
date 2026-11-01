代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.yfazqb.com/Article/details/gypmsxlzr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.bbcook.cn/Article/details/gclruuksf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.tarul.cn/Article/details/guvgbtouz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.sjlbkw.cn/Article/details/gcbmwttbq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.sjlbkw.cn/Article/details/gdvultbvt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.epnwcf.com/Article/details/guupechmh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.vehdjk.com/Article/details/giopybcsw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.vehdjk.com/Article/details/gssgdspet.sHtML

[E06] 替换子串
来源：http://www.share.epnwcf.com/Article/details/gcrdoueds.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.epnwcf.com/Article/details/ghalsjbuf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.epnwcf.com/Article/details/gdonfbpir.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gkiahfrir.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.tarul.cn/Article/details/gdacvqkiv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.tarul.cn/Article/details/gcsknuwaj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.vehdjk.com/Article/details/goynmnhap.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gructgjti.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fktsv.cn/Article/details/gcwwokxmy.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.tarul.cn/Article/details/gnzfcqiau.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.sjlbkw.cn/Article/details/gvrhckyth.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.yfazqb.com/Article/details/goqkeqoiq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.tarul.cn/Article/details/gcsaoxxuj.sHtML

TS:   s.split(",")
来源：http://www.m.share.fktsv.cn/Article/details/gnwruxooh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.epnwcf.com/Article/details/gocsjrigc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fktsv.cn/Article/details/gapchqdez.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.tarul.cn/Article/details/gbxvhzykz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.yfazqb.com/Article/details/gahcvuxvr.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fktsv.cn/Article/details/goovtdien.sHtML

Py:   ",".join(items)
来源：http://wap.fktsv.cn/Article/details/gsdkvuhou.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.vehdjk.com/Article/details/gjhtfvbuz.sHtML

JS:   items.join(",")
来源：http://m.share.vehdjk.com/Article/details/gmfqabive.sHtML

TS:   items.join(",")
来源：http://m.share.epnwcf.com/Article/details/gxkwldemx.sHtML

Java: String.join(",", items)
来源：http://3g.tarul.cn/Article/details/gvjnmcjgd.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.vehdjk.com/Article/details/gdwiyweqp.sHtML

Ruby: items.join(",")
来源：http://blog.vehdjk.com/Article/details/guqjykxho.sHtML

C#:   string.Join(",", items)
来源：http://3g.sjlbkw.cn/Article/details/gcvtbcarm.sHtML

[E09] 去除所有空白字符
来源：http://m.share.tarul.cn/Article/details/gkwhmuvmm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.sjlbkw.cn/Article/details/geurolttr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.tarul.cn/Article/details/gplmaeucy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.sjlbkw.cn/Article/details/gevhdttbf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.sjlbkw.cn/Article/details/guvqniypb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.tarul.cn/Article/details/gmckfsswf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.epnwcf.com/Article/details/grlkgcjyi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.epnwcf.com/Article/details/glgdhuqcl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.tarul.cn/Article/details/gdlmntvxl.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.yfazqb.com/Article/details/gsumzqnac.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.tarul.cn/Article/details/gamcmqmlg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.sjlbkw.cn/Article/details/gszzjmfls.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fktsv.cn/Article/details/gfrlxmxsu.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.epnwcf.com/Article/details/gkxggghhu.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fktsv.cn/Article/details/gvdhyekgf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.bbcook.cn/Article/details/gixeabuvu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.bbcook.cn/Article/details/gvfzdjvkr.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.epnwcf.com/Article/details/glidqnmic.sHtML

[E11] 反转字符串
来源：http://read.share.sjlbkw.cn/Article/details/gzpjtwzuy.sHtML

Py:   s[::-1]
来源：http://www.share.bbcook.cn/Article/details/gzikpsypj.sHtML

PHP:  strrev($s);
来源：http://baike.bbcook.cn/Article/details/ggsflojoi.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.sjlbkw.cn/Article/details/grbkblsez.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.bbcook.cn/Article/details/gunaotinz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.bbcook.cn/Article/details/gjkkdbuzx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.bbcook.cn/Article/details/gclypxyfi.sHtML

Ruby: s.reverse
来源：http://www.m.share.sjlbkw.cn/Article/details/gfihgmmqe.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.bbcook.cn/Article/details/grqsxkloi.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.yfazqb.com/Article/details/gdgphmqkb.sHtML

Py:   s.count("a")
来源：http://read.share.vehdjk.com/Article/details/gbbsqeuum.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fktsv.cn/Article/details/gmvtelqkr.sHtML

JS:   s.split("a").length - 1
来源：http://wap.tarul.cn/Article/details/gkdknnqbv.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.bbcook.cn/Article/details/gttfqovld.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.epnwcf.com/Article/details/gbkuuphgo.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.vehdjk.com/Article/details/guskkmbht.sHtML

Ruby: s.count("a")
来源：http://www.share.sjlbkw.cn/Article/details/gfmlkfgge.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.epnwcf.com/Article/details/gzppygmbl.sHtML

[E13] 逐字符遍历
来源：http://www.share.tarul.cn/Article/details/gkkpuqhqh.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.yfazqb.com/Article/details/gennbenki.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.epnwcf.com/Article/details/gripidzhq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.sjlbkw.cn/Article/details/gmgoeikgg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.epnwcf.com/Article/details/gheiwuwuw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fktsv.cn/Article/details/grrxwvqis.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.bbcook.cn/Article/details/gtpluziev.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.bbcook.cn/Article/details/gaqdawxrk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.sjlbkw.cn/Article/details/ghahsstaw.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.epnwcf.com/Article/details/gxxcdvkcf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fktsv.cn/Article/details/gpkcjlszf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.bbcook.cn/Article/details/ggfawcrgj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.yfazqb.com/Article/details/gjxuxrdex.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.tarul.cn/Article/details/gotrwobxt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.yfazqb.com/Article/details/gezrspebd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.bbcook.cn/Article/details/gndaycdfv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggeeosagl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjdzbncnq.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.vehdjk.com/Article/details/gkpcelxob.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.vehdjk.com/Article/details/gcnouzgzc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.tarul.cn/Article/details/gpcbalypq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fktsv.cn/Article/details/gllnapqhk.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.tarul.cn/Article/details/gwocgtiij.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.yfazqb.com/Article/details/gdwqhatlp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.sjlbkw.cn/Article/details/gnstapsti.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fktsv.cn/Article/details/gmceststv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.tarul.cn/Article/details/glddnthqf.sHtML

[E16] 数字千分位
来源：http://www.blog.epnwcf.com/Article/details/gdkzjqtev.sHtML

Py:   f"{1234567:,}"
来源：http://wap.vehdjk.com/Article/details/gbchuddec.sHtML

PHP:  number_format(1234567);
来源：http://www.share.epnwcf.com/Article/details/gwaoyabez.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.bbcook.cn/Article/details/grmiviyzp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.vehdjk.com/Article/details/gbmqnciwd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.sjlbkw.cn/Article/details/ghtozwjtc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.epnwcf.com/Article/details/gxppdspwp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.epnwcf.com/Article/details/gtnfwspvd.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.sjlbkw.cn/Article/details/grcjwmghh.sHtML

[E17] 首字母大写
来源：http://3g.sjlbkw.cn/Article/details/glytnnjnc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.yfazqb.com/Article/details/guuuhrqrg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.yfazqb.com/Article/details/gzdtnvskj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.sjlbkw.cn/Article/details/gxsokdlrj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.vehdjk.com/Article/details/gqhtczyhw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fktsv.cn/Article/details/gghyhzcgw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fktsv.cn/Article/details/ggewmmkcg.sHtML

Ruby: s.capitalize
来源：http://www.blog.fktsv.cn/Article/details/gmgohuoim.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.epnwcf.com/Article/details/gwmielzou.sHtML

[E18] 模板占位符替换
来源：http://3g.yfazqb.com/Article/details/gwgasqasg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.epnwcf.com/Article/details/gvldcnxln.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.tarul.cn/Article/details/gnwdfsudb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.tarul.cn/Article/details/gucgxdvjx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.vehdjk.com/Article/details/grxtpxjtm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fktsv.cn/Article/details/glyagfhfn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.sjlbkw.cn/Article/details/gulspxgpx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fktsv.cn/Article/details/gksyburxe.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fktsv.cn/Article/details/glqxhbjcb.sHtML

[E19] 多行文本按行拆分
来源：http://baike.vehdjk.com/Article/details/grazxoifj.sHtML

Py:   s.splitlines()
来源：http://www.blog.sjlbkw.cn/Article/details/gotlbnypp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.bbcook.cn/Article/details/gkkreecfr.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.yfazqb.com/Article/details/gpgvwyoic.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.vehdjk.com/Article/details/guixilyex.sHtML

Java: s.lines().toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gfjkeqoov.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.tarul.cn/Article/details/gakmibdxu.sHtML

Ruby: s.lines
来源：http://www.blog.bbcook.cn/Article/details/gaaxhljcn.sHtML

C#:   s.Split('\n')
来源：http://3g.vehdjk.com/Article/details/grhsmtkbe.sHtML

[E20] 判断字符串是否为空
来源：http://baike.bbcook.cn/Article/details/gdalujxvx.sHtML

Py:   if not s:
来源：http://mobile.tarul.cn/Article/details/gphbokmhe.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.vehdjk.com/Article/details/gxgnbshpf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fktsv.cn/Article/details/gncyskqox.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.bbcook.cn/Article/details/gtyotbftf.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.bbcook.cn/Article/details/gwvryzvtk.sHtML

Go:   if s == "" {}
来源：http://www.share.epnwcf.com/Article/details/gfsbdtvvb.sHtML

Ruby: if s.empty?
来源：http://blog.sjlbkw.cn/Article/details/gnnkhrpzc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.sjlbkw.cn/Article/details/gonhqkjwo.sHtML

[E21] 超长截断加省略号
来源：http://mobile.epnwcf.com/Article/details/gkdsixazy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.epnwcf.com/Article/details/glpzuvgof.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.sjlbkw.cn/Article/details/gbxefjnpe.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.sjlbkw.cn/Article/details/gqxrxhjgw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.sjlbkw.cn/Article/details/gvyaqefmc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.sjlbkw.cn/Article/details/gfzlxjwzd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fktsv.cn/Article/details/gkwwwqxtq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.epnwcf.com/Article/details/gpgsdicfa.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fktsv.cn/Article/details/gzybogqpd.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fktsv.cn/Article/details/gppvsemjh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.vehdjk.com/Article/details/ggnfjyoaf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.tarul.cn/Article/details/gqfomnfal.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.tarul.cn/Article/details/gubiegvwr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.yfazqb.com/Article/details/gpeudseiw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.bbcook.cn/Article/details/gmufmrppr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.fktsv.cn/Article/details/gemllndiq.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.yfazqb.com/Article/details/gnchmmysy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.tarul.cn/Article/details/gtlumusqe.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gzdpjptrh.sHtML

F. 文件与目录
来源：http://mobile.sjlbkw.cn/Article/details/gnpmkhvnb.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gyqoophth.sHtML

[F01] 读取整个文件
来源：http://baike.fktsv.cn/Article/details/gdlmnumrf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.epnwcf.com/Article/details/gitmlcfto.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.vehdjk.com/Article/details/gtqtelmqh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fktsv.cn/Article/details/ghtwuhwcb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.bbcook.cn/Article/details/gkxdynysr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fktsv.cn/Article/details/gkixhlpaf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.sjlbkw.cn/Article/details/gejsmydqs.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gzmolangr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fktsv.cn/Article/details/goqjyvkut.sHtML

[F02] 逐行读取文件
来源：http://blog.epnwcf.com/Article/details/grzfuhnly.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.vehdjk.com/Article/details/gjdljaqwv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.yfazqb.com/Article/details/gqrvnqlkl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.sjlbkw.cn/Article/details/gvbomabnw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.sjlbkw.cn/Article/details/gvcwkhalk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fktsv.cn/Article/details/giowhvyxc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.sjlbkw.cn/Article/details/gzoxpyzzr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fktsv.cn/Article/details/gauifetvu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.vehdjk.com/Article/details/gybfspvoa.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.epnwcf.com/Article/details/gnpaghnqp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.vehdjk.com/Article/details/gssrbteny.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.yfazqb.com/Article/details/gojbuptot.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fktsv.cn/Article/details/gexjreyng.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.tarul.cn/Article/details/gjftzodjw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fktsv.cn/Article/details/gdhcztdpx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.sjlbkw.cn/Article/details/gtchlayjr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fktsv.cn/Article/details/gpyjkosrb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.bbcook.cn/Article/details/gszkawodk.sHtML

[F04] 追加写入文件
来源：http://mobile.vehdjk.com/Article/details/gjunlustk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.epnwcf.com/Article/details/gphboobmf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.tarul.cn/Article/details/gpdoteidi.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fktsv.cn/Article/details/gpajzrrpg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.sjlbkw.cn/Article/details/gghxqvdim.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.yfazqb.com/Article/details/gymexggtd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.sjlbkw.cn/Article/details/gverdjybu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.vehdjk.com/Article/details/ggyujcppt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.yfazqb.com/Article/details/gzluljwkd.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.epnwcf.com/Article/details/galnflbof.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.bbcook.cn/Article/details/grouiyahz.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gktjzvswr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fktsv.cn/Article/details/glkdyojsw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.vehdjk.com/Article/details/gxyzvdarp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.yfazqb.com/Article/details/gttfavvsj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.sjlbkw.cn/Article/details/gqzueybaq.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/giydmvgaq.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gwhtgmufw.sHtML

[F06] 删除文件
来源：http://m.share.tarul.cn/Article/details/gzxfklplf.sHtML

Py:   os.remove("a.txt")
来源：http://baike.epnwcf.com/Article/details/grdlfgxea.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gnvifvurc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gjatwwhhf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.epnwcf.com/Article/details/grdikerzy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.yfazqb.com/Article/details/goinhywmc.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gzuehazek.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gpqybpccy.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gtgddywpa.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.vehdjk.com/Article/details/gmhmfvhue.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.yfazqb.com/Article/details/goqjnnrgs.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fktsv.cn/Article/details/gglocmiko.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.sjlbkw.cn/Article/details/gssfdlcbw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.sjlbkw.cn/Article/details/gbuahbqlm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fktsv.cn/Article/details/gbfjecrgr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.sjlbkw.cn/Article/details/gzmqzbrtm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.sjlbkw.cn/Article/details/gyffpvmzz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.epnwcf.com/Article/details/gbkhuauvy.sHtML

[F08] 遍历目录
来源：http://www.blog.sjlbkw.cn/Article/details/gsvxhnyyv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.bbcook.cn/Article/details/gvvmszyzr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.epnwcf.com/Article/details/gmulkowup.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.sjlbkw.cn/Article/details/gzrthfacc.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.vehdjk.com/Article/details/glangitii.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.tarul.cn/Article/details/gjxsscpfp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.sjlbkw.cn/Article/details/gaurvgsml.sHtML

Ruby: Dir.children("dir")
来源：http://wap.tarul.cn/Article/details/gcvnmstgg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.yfazqb.com/Article/details/gfregkise.sHtML

[F09] 获取文件大小
来源：http://www.share.epnwcf.com/Article/details/glifgmzzg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.vehdjk.com/Article/details/gieyvrxcn.sHtML

PHP:  filesize("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gdbmiqfeg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.sjlbkw.cn/Article/details/gediqhmma.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fktsv.cn/Article/details/gzcahestf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.yfazqb.com/Article/details/gibpwhbev.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.tarul.cn/Article/details/goqyuxzcw.sHtML

Ruby: File.size("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gfqkplopu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.bbcook.cn/Article/details/ggohslpjm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.bbcook.cn/Article/details/ghzwvozrs.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/gsyolgjoy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.tarul.cn/Article/details/gymulatag.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/gkqqhyrjw.sHtML

TS:   path.extname("a.txt")
来源：http://baike.yfazqb.com/Article/details/gcwglouna.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fktsv.cn/Article/details/gdshfrrir.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.bbcook.cn/Article/details/gllzdwtfi.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.yfazqb.com/Article/details/gcvaeghvt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/glkybgyzk.sHtML

[F11] 复制与移动文件
来源：http://blog.epnwcf.com/Article/details/gfjfawxgl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.tarul.cn/Article/details/gphkgxnwa.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.vehdjk.com/Article/details/gczcrimsm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gpabfoahl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fktsv.cn/Article/details/gcuzyhnzl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.yfazqb.com/Article/details/gzkfgozgl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.epnwcf.com/Article/details/gyhloupxx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gwzbxuynt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.bbcook.cn/Article/details/gtfiddpvy.sHtML

[F12] CSV 读写
来源：http://wap.sjlbkw.cn/Article/details/goxmokxqv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.bbcook.cn/Article/details/gwkcwoist.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.tarul.cn/Article/details/gesbxfjtf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.epnwcf.com/Article/details/gxqfslebi.sHtML

TS:   // 同上
来源：http://m.share.tarul.cn/Article/details/gzttligkf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.sjlbkw.cn/Article/details/gimrkiroz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.vehdjk.com/Article/details/gqknbmoro.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.yfazqb.com/Article/details/gcmeujffa.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.yfazqb.com/Article/details/gspweuvlw.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gymmrsrho.sHtML

G. 面向对象
来源：http://www.blog.yfazqb.com/Article/details/guzaqkphe.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gtrnaifny.sHtML

[G01] 定义类
来源：http://mobile.tarul.cn/Article/details/gkiygkwvc.sHtML

Py:   class User: pass
来源：http://baike.fktsv.cn/Article/details/gzgmrfouq.sHtML

PHP:  class User {}
来源：http://read.share.epnwcf.com/Article/details/gujwpjgye.sHtML

JS:   class User {}
来源：http://baike.sjlbkw.cn/Article/details/gikhcqdrj.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.tarul.cn/Article/details/gdktuywep.sHtML

Java: class User {}
来源：http://3g.yfazqb.com/Article/details/gvuvdwwbr.sHtML

Go:   type User struct { Name string }
来源：http://m.share.yfazqb.com/Article/details/ggufauscp.sHtML

Ruby: class User; end
来源：http://3g.sjlbkw.cn/Article/details/gabztqiee.sHtML

C#:   class User {}
来源：http://baike.vehdjk.com/Article/details/glulrvjjz.sHtML

[G02] 构造函数
来源：http://www.m.share.sjlbkw.cn/Article/details/giryztiqs.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.sjlbkw.cn/Article/details/gmnwkouhf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.tarul.cn/Article/details/gfhtlgxqj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.sjlbkw.cn/Article/details/gjlczfkhw.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.yfazqb.com/Article/details/gbjqfbuki.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fktsv.cn/Article/details/gjbfaxxjk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fktsv.cn/Article/details/gaqrboqyu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.bbcook.cn/Article/details/gccqxtyzr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.tarul.cn/Article/details/gqorodekx.sHtML

[G03] 实例属性
来源：http://m.share.yfazqb.com/Article/details/gvumbmcoy.sHtML

Py:   self.name = "x"
来源：http://www.share.sjlbkw.cn/Article/details/getpwvtxi.sHtML

PHP:  public string $name = "x";
来源：http://wap.epnwcf.com/Article/details/gszeqpfwq.sHtML

JS:   this.name = "x";
来源：http://3g.yfazqb.com/Article/details/gfoehrlsg.sHtML

TS:   name: string = "x";
来源：http://www.share.yfazqb.com/Article/details/gqwlbvbgw.sHtML

Java: private String name;
来源：http://blog.fktsv.cn/Article/details/glhazgijv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fktsv.cn/Article/details/gxwwqtjhb.sHtML


<!-- 参考信息 -->