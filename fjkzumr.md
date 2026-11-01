代发 wailian999

[E06] 替换子串
来源：http://www.share.bbcook.cn/Article/details/gziwotwez.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fktsv.cn/Article/details/gevdtltai.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.yfazqb.com/Article/details/gnvldmggj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gcliftbtw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.bbcook.cn/Article/details/geilykpnn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gjddahenr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.bbcook.cn/Article/details/gulbquumo.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.yfazqb.com/Article/details/ghkdjwxwy.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fktsv.cn/Article/details/gzbjdmhtk.sHtML

[E07] 按分隔符拆分
来源：http://read.share.tarul.cn/Article/details/grvdrzqvt.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.sjlbkw.cn/Article/details/ghhphtbwe.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gezsxmkyi.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.yfazqb.com/Article/details/ghfhbtcor.sHtML

TS:   s.split(",")
来源：http://mobile.tarul.cn/Article/details/gwhpoylps.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.epnwcf.com/Article/details/gtltkmoku.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fktsv.cn/Article/details/gjaxfhbef.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.tarul.cn/Article/details/gixlhoxaw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.bbcook.cn/Article/details/gevjpfeog.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.bbcook.cn/Article/details/guhyuehcx.sHtML

Py:   ",".join(items)
来源：http://www.share.yfazqb.com/Article/details/gjqlhzhqv.sHtML

PHP:  implode(",", $items);
来源：http://mobile.yfazqb.com/Article/details/gzsnujhit.sHtML

JS:   items.join(",")
来源：http://www.blog.tarul.cn/Article/details/ghripoyfu.sHtML

TS:   items.join(",")
来源：http://www.blog.sjlbkw.cn/Article/details/gsmdjlmxe.sHtML

Java: String.join(",", items)
来源：http://read.share.yfazqb.com/Article/details/gsbxzaahz.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fktsv.cn/Article/details/gkoagdmus.sHtML

Ruby: items.join(",")
来源：http://www.m.share.bbcook.cn/Article/details/glhdqnoli.sHtML

C#:   string.Join(",", items)
来源：http://3g.tarul.cn/Article/details/gliljovsy.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.tarul.cn/Article/details/godvdkgev.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.bbcook.cn/Article/details/gknyiwlph.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.yfazqb.com/Article/details/gdgzkqkox.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.yfazqb.com/Article/details/ghqmqlgjd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.sjlbkw.cn/Article/details/gaeylsgdg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.tarul.cn/Article/details/gruxwppch.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.yfazqb.com/Article/details/gceenslmg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.yfazqb.com/Article/details/gqfghkxfp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fktsv.cn/Article/details/gfoezxaaj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.tarul.cn/Article/details/gwpznbqrd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.yfazqb.com/Article/details/gwrfsavyl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.vehdjk.com/Article/details/gjksccncy.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.sjlbkw.cn/Article/details/gigivxjoh.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.tarul.cn/Article/details/goegnwenj.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.yfazqb.com/Article/details/gkxqrmmhx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.epnwcf.com/Article/details/getegqlis.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.bbcook.cn/Article/details/gpjvlmmaf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.vehdjk.com/Article/details/gbrjxyxii.sHtML

[E11] 反转字符串
来源：http://www.m.share.fktsv.cn/Article/details/gcnhkbqay.sHtML

Py:   s[::-1]
来源：http://3g.yfazqb.com/Article/details/gyuuhxckl.sHtML

PHP:  strrev($s);
来源：http://3g.epnwcf.com/Article/details/ghwmfxhbh.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.sjlbkw.cn/Article/details/guqhmyfld.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.tarul.cn/Article/details/gnljubijf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.yfazqb.com/Article/details/gvfvnaooc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.epnwcf.com/Article/details/gmaveursc.sHtML

Ruby: s.reverse
来源：http://www.blog.sjlbkw.cn/Article/details/gqpqibjnm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fktsv.cn/Article/details/gmjpzkhtg.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.epnwcf.com/Article/details/gmswfubgv.sHtML

Py:   s.count("a")
来源：http://3g.vehdjk.com/Article/details/guhrhxlje.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.yfazqb.com/Article/details/gdbybxaie.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fktsv.cn/Article/details/gewovbvub.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.epnwcf.com/Article/details/gtskwzqle.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.sjlbkw.cn/Article/details/gdxlymxhb.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.bbcook.cn/Article/details/ggzigbcfp.sHtML

Ruby: s.count("a")
来源：http://read.share.epnwcf.com/Article/details/guprhgqzg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fktsv.cn/Article/details/gveiwsqfb.sHtML

[E13] 逐字符遍历
来源：http://read.share.sjlbkw.cn/Article/details/gsqznsyxt.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.sjlbkw.cn/Article/details/gwxijfihu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.yfazqb.com/Article/details/gooqsxjbh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fktsv.cn/Article/details/ghzzrccdh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.bbcook.cn/Article/details/gakxgolah.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.epnwcf.com/Article/details/gjouphiex.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.tarul.cn/Article/details/gfmgifini.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.tarul.cn/Article/details/gxmzztyma.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.sjlbkw.cn/Article/details/gzlpvnrax.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.sjlbkw.cn/Article/details/gzvurupff.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.sjlbkw.cn/Article/details/ghetwozjy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.vehdjk.com/Article/details/gyzbgrsmw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fktsv.cn/Article/details/grabjiwll.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.bbcook.cn/Article/details/gfrundtbo.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.bbcook.cn/Article/details/gferqszcs.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.epnwcf.com/Article/details/gbuudczbf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.sjlbkw.cn/Article/details/gjwkcshyh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.sjlbkw.cn/Article/details/gcdwvgjpj.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fktsv.cn/Article/details/gfuelgrtn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fktsv.cn/Article/details/gltcswydn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.tarul.cn/Article/details/gkxmkdnkw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.vehdjk.com/Article/details/gxqplftvj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.bbcook.cn/Article/details/gyhwzzigl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.tarul.cn/Article/details/ggcrnilrc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.vehdjk.com/Article/details/gawxqzcqw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.sjlbkw.cn/Article/details/ghltkhwpg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.epnwcf.com/Article/details/gutitemvn.sHtML

[E16] 数字千分位
来源：http://m.share.sjlbkw.cn/Article/details/gdbdjzfib.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fktsv.cn/Article/details/gnbyqqbra.sHtML

PHP:  number_format(1234567);
来源：http://wap.yfazqb.com/Article/details/gnyhtfmip.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.yfazqb.com/Article/details/gbzjypviv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.bbcook.cn/Article/details/gqgbadmnq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.yfazqb.com/Article/details/gvdvbvygv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.yfazqb.com/Article/details/gpkmtfuqx.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.epnwcf.com/Article/details/grncqcape.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.yfazqb.com/Article/details/gkkacptgm.sHtML

[E17] 首字母大写
来源：http://www.m.share.vehdjk.com/Article/details/gzxtrbyvu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.vehdjk.com/Article/details/gbhugycgq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.tarul.cn/Article/details/gydeebrwc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.vehdjk.com/Article/details/gcusvslmg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.yfazqb.com/Article/details/gogjwzgfj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.vehdjk.com/Article/details/gitfrmeqr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.yfazqb.com/Article/details/gjhhoragc.sHtML

Ruby: s.capitalize
来源：http://wap.tarul.cn/Article/details/gckdmpatn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.epnwcf.com/Article/details/goyiounsq.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.vehdjk.com/Article/details/gzyrcmfyn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.yfazqb.com/Article/details/gpqisxvhj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.epnwcf.com/Article/details/grnvhmnoa.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.tarul.cn/Article/details/gkbzwsgif.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.tarul.cn/Article/details/gvoowebba.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.vehdjk.com/Article/details/gudmjjfjp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.sjlbkw.cn/Article/details/gnnulyzha.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.tarul.cn/Article/details/gsmljhjau.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fktsv.cn/Article/details/giztrngkr.sHtML

[E19] 多行文本按行拆分
来源：http://blog.yfazqb.com/Article/details/gnwmvidqp.sHtML

Py:   s.splitlines()
来源：http://3g.fktsv.cn/Article/details/gyahmeljk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.epnwcf.com/Article/details/gzoirmicj.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fktsv.cn/Article/details/guqgzglfh.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fktsv.cn/Article/details/gyhmpqnas.sHtML

Java: s.lines().toList()
来源：http://3g.vehdjk.com/Article/details/gdufiemka.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.epnwcf.com/Article/details/gsqkuzaqs.sHtML

Ruby: s.lines
来源：http://www.m.share.vehdjk.com/Article/details/gjhbhaibm.sHtML

C#:   s.Split('\n')
来源：http://3g.epnwcf.com/Article/details/gyqfloode.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.vehdjk.com/Article/details/gcktpdynx.sHtML

Py:   if not s:
来源：http://wap.sjlbkw.cn/Article/details/gqdfbokwh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.vehdjk.com/Article/details/gbjlyxdft.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.bbcook.cn/Article/details/gehrciqnx.sHtML

TS:   if (s === "") {}
来源：http://m.share.vehdjk.com/Article/details/gpekdilcz.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.yfazqb.com/Article/details/gdcuokrsb.sHtML

Go:   if s == "" {}
来源：http://wap.sjlbkw.cn/Article/details/gipvlgtus.sHtML

Ruby: if s.empty?
来源：http://3g.vehdjk.com/Article/details/gujznhorn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.tarul.cn/Article/details/grqgsbccv.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fktsv.cn/Article/details/gcqxznfny.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.sjlbkw.cn/Article/details/gtwonetzk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.yfazqb.com/Article/details/gdqqwahpq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.bbcook.cn/Article/details/gwwukifxa.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.yfazqb.com/Article/details/gzsbshoyp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.bbcook.cn/Article/details/gpmvrjbam.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.sjlbkw.cn/Article/details/gtbzbyzew.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.yfazqb.com/Article/details/ggfehnphb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/gcetesyzv.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.yfazqb.com/Article/details/gmkzguvqs.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fktsv.cn/Article/details/gluttxfmc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.epnwcf.com/Article/details/gbpbuiurd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.yfazqb.com/Article/details/ggdkugclw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.bbcook.cn/Article/details/gkmmvsmnn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.sjlbkw.cn/Article/details/gokdpegvz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fktsv.cn/Article/details/gckvrkmsd.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fktsv.cn/Article/details/gzptbmdmd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fktsv.cn/Article/details/gcrgoyuvz.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gcxoiavvq.sHtML

F. 文件与目录
来源：http://www.m.share.sjlbkw.cn/Article/details/gdxtqzfaw.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gnfgdzkbs.sHtML

[F01] 读取整个文件
来源：http://www.blog.yfazqb.com/Article/details/gdjppofxp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.tarul.cn/Article/details/gaxfqbwzs.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gvqfzupxn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fktsv.cn/Article/details/gogdobgis.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.sjlbkw.cn/Article/details/gcopkkkaw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gdxeudtam.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.bbcook.cn/Article/details/gqvicumwb.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gumirawwc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gcdhtpvre.sHtML

[F02] 逐行读取文件
来源：http://baike.vehdjk.com/Article/details/gwxmrjizy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.sjlbkw.cn/Article/details/gxwgabagl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.epnwcf.com/Article/details/gqqfzlont.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.yfazqb.com/Article/details/gzrtcbezx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.bbcook.cn/Article/details/gdswzugzx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.epnwcf.com/Article/details/gyknczfcn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.tarul.cn/Article/details/glrbmsmht.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.sjlbkw.cn/Article/details/gvbypijys.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.epnwcf.com/Article/details/gkmflzhpt.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.bbcook.cn/Article/details/gmflufomk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.epnwcf.com/Article/details/glsnhzsiq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.sjlbkw.cn/Article/details/ghpqandnl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.bbcook.cn/Article/details/gqpycdpov.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.sjlbkw.cn/Article/details/glxrjuxnn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.yfazqb.com/Article/details/ghbyoftoo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.vehdjk.com/Article/details/gurlpmled.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.epnwcf.com/Article/details/gfjfhazcw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.yfazqb.com/Article/details/gtalfdxuo.sHtML

[F04] 追加写入文件
来源：http://www.blog.epnwcf.com/Article/details/giaxhnkae.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fktsv.cn/Article/details/gqcywagfp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.vehdjk.com/Article/details/gxjxzwdhi.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.tarul.cn/Article/details/gjlxunatp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.tarul.cn/Article/details/givvwcgte.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.vehdjk.com/Article/details/gkxexnccg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.sjlbkw.cn/Article/details/glsunfwkb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.epnwcf.com/Article/details/gjpkaybhk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.bbcook.cn/Article/details/gsrcytkid.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.epnwcf.com/Article/details/gmlsiupjw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.bbcook.cn/Article/details/ghwkotbiw.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gcvcnzxsd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.bbcook.cn/Article/details/gsaojijqn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gmigoubwn.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.bbcook.cn/Article/details/ghnwlqivz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.bbcook.cn/Article/details/ggndfclme.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.tarul.cn/Article/details/geoodelif.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gampwcsya.sHtML

[F06] 删除文件
来源：http://3g.sjlbkw.cn/Article/details/gwhwrpbwc.sHtML

Py:   os.remove("a.txt")
来源：http://wap.tarul.cn/Article/details/gxukpghir.sHtML

PHP:  unlink("a.txt");
来源：http://baike.bbcook.cn/Article/details/gbcdtixja.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gqnucsreh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.bbcook.cn/Article/details/gyvywmkjb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.epnwcf.com/Article/details/gvslnaeoe.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.vehdjk.com/Article/details/gpvwncwxl.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.epnwcf.com/Article/details/ghklfjxlq.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/glquvcnmk.sHtML

[F07] 创建目录（含多级）
来源：http://3g.yfazqb.com/Article/details/gdvgpeyae.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.bbcook.cn/Article/details/gohvhnobb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.bbcook.cn/Article/details/gebctujii.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.vehdjk.com/Article/details/gccorhvdm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.epnwcf.com/Article/details/gjxdhuwqn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.sjlbkw.cn/Article/details/gyterxltt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.yfazqb.com/Article/details/gvynkbbzu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.sjlbkw.cn/Article/details/gwmofiyxq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fktsv.cn/Article/details/gelmsxsfm.sHtML

[F08] 遍历目录
来源：http://wap.fktsv.cn/Article/details/gjxuvhmyk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.bbcook.cn/Article/details/gojtldzft.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.tarul.cn/Article/details/gjhdpwtra.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.vehdjk.com/Article/details/godlwzuaa.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fktsv.cn/Article/details/gwcwhekng.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.bbcook.cn/Article/details/ghpyvwcel.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.vehdjk.com/Article/details/gdxhemqkn.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fktsv.cn/Article/details/gxveitrhx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.vehdjk.com/Article/details/gogvcuion.sHtML

[F09] 获取文件大小
来源：http://wap.bbcook.cn/Article/details/gajnihdqn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/giqonmicd.sHtML

PHP:  filesize("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gnmalfnvr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.tarul.cn/Article/details/gcvumszgy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.bbcook.cn/Article/details/giztmgqnw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fktsv.cn/Article/details/gqnprmbmm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.epnwcf.com/Article/details/gumnojxvy.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/giitqcdzf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.bbcook.cn/Article/details/gztrpxojq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.sjlbkw.cn/Article/details/gsdnoallz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/gqntjmgjz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gdymxuwpc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gwqzqokpi.sHtML

TS:   path.extname("a.txt")
来源：http://baike.tarul.cn/Article/details/gklxgnthe.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fktsv.cn/Article/details/gyykkjhqm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fktsv.cn/Article/details/gjoescydb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gnfgbqcys.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gcjtfwsgh.sHtML

[F11] 复制与移动文件
来源：http://www.share.yfazqb.com/Article/details/ggnfndfmg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fktsv.cn/Article/details/gviwqdbyn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.vehdjk.com/Article/details/gaabolomo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.yfazqb.com/Article/details/gheyxeckv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.yfazqb.com/Article/details/gpuculjke.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.yfazqb.com/Article/details/gdshfkfqe.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fktsv.cn/Article/details/gpdqklqqe.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fktsv.cn/Article/details/gjxvruumu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.epnwcf.com/Article/details/gmqdzyzse.sHtML

[F12] CSV 读写
来源：http://mobile.epnwcf.com/Article/details/gionjcbsa.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fktsv.cn/Article/details/gcmiactqw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.tarul.cn/Article/details/gbkdizucc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fktsv.cn/Article/details/gkxvyjram.sHtML

TS:   // 同上
来源：http://read.share.fktsv.cn/Article/details/gwdoertkz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.bbcook.cn/Article/details/gccogjfwb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.sjlbkw.cn/Article/details/gzkvtqbxy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.sjlbkw.cn/Article/details/grgnoxzkd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.yfazqb.com/Article/details/gqcbmzxmc.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gyixzayqm.sHtML

G. 面向对象
来源：http://read.share.bbcook.cn/Article/details/gshhqczte.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gigpmmlyw.sHtML

[G01] 定义类
来源：http://www.blog.fktsv.cn/Article/details/grffcivyn.sHtML

Py:   class User: pass
来源：http://m.share.sjlbkw.cn/Article/details/gqtvyztwz.sHtML

PHP:  class User {}
来源：http://read.share.bbcook.cn/Article/details/gjounfrts.sHtML

JS:   class User {}
来源：http://3g.vehdjk.com/Article/details/gzzsjibft.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.tarul.cn/Article/details/givxwqjzt.sHtML

Java: class User {}
来源：http://mobile.vehdjk.com/Article/details/ghxzkamkt.sHtML

Go:   type User struct { Name string }
来源：http://3g.fktsv.cn/Article/details/gpuppudhs.sHtML

Ruby: class User; end
来源：http://baike.bbcook.cn/Article/details/gnyuyztqo.sHtML

C#:   class User {}
来源：http://www.blog.fktsv.cn/Article/details/gizvashde.sHtML

[G02] 构造函数
来源：http://read.share.bbcook.cn/Article/details/gzbtsxeqe.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.vehdjk.com/Article/details/gytwjbnho.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.yfazqb.com/Article/details/ghtlhmpgn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/glrfmqkiu.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fktsv.cn/Article/details/gqwnrhvhb.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.yfazqb.com/Article/details/gpvllswqb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.epnwcf.com/Article/details/glzshctji.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.vehdjk.com/Article/details/grtiojdtl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fktsv.cn/Article/details/gbfnnaljt.sHtML

[G03] 实例属性
来源：http://blog.fktsv.cn/Article/details/giyohnysw.sHtML

Py:   self.name = "x"
来源：http://mobile.bbcook.cn/Article/details/gilihxsrk.sHtML

PHP:  public string $name = "x";
来源：http://wap.vehdjk.com/Article/details/gwdlbdjav.sHtML

JS:   this.name = "x";
来源：http://m.share.vehdjk.com/Article/details/gvxngrlmh.sHtML

TS:   name: string = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/gukthgtlk.sHtML

Java: private String name;
来源：http://www.blog.fktsv.cn/Article/details/gusfoczem.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.bbcook.cn/Article/details/gqajdsame.sHtML

Ruby: @name = "x"
来源：http://baike.bbcook.cn/Article/details/gkublxgqc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fktsv.cn/Article/details/guhdccbzv.sHtML

[G04] 定义方法
来源：http://www.blog.epnwcf.com/Article/details/gmbswlyvc.sHtML

Py:   def greet(self): return self.name
来源：http://3g.sjlbkw.cn/Article/details/gqfhcxkjt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fktsv.cn/Article/details/gryuxegiv.sHtML

JS:   greet() { return this.name; }
来源：http://wap.yfazqb.com/Article/details/gmvizlfyf.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.sjlbkw.cn/Article/details/gtgcyqwxi.sHtML

Java: String greet() { return name; }
来源：http://wap.fktsv.cn/Article/details/gjptgvuql.sHtML


<!-- 参考信息 -->