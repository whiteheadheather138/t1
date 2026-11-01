代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.vehdjk.com/Article/details/gsxshsbkf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.epnwcf.com/Article/details/gpxalhdrd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.tarul.cn/Article/details/gyjpoqddo.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.yfazqb.com/Article/details/gdrfqdjye.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.bbcook.cn/Article/details/gemdmlqbi.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.tarul.cn/Article/details/gbcawnacg.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.yfazqb.com/Article/details/gtypmjlkl.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.yfazqb.com/Article/details/gfgvrigdo.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.vehdjk.com/Article/details/gnmjmpupp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fktsv.cn/Article/details/gcxpgzmyu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fktsv.cn/Article/details/girekspps.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.epnwcf.com/Article/details/glmioljdi.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.epnwcf.com/Article/details/ginsjnwmo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.epnwcf.com/Article/details/gumwttxmb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.epnwcf.com/Article/details/gutjtfjth.sHtML

[D26] 数组转字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gbmutztup.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.yfazqb.com/Article/details/geuulocur.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.epnwcf.com/Article/details/gzzpzppxn.sHtML

JS:   arr.join(", ")
来源：http://read.share.epnwcf.com/Article/details/gdmlzzcin.sHtML

TS:   arr.join(", ")
来源：http://www.share.tarul.cn/Article/details/gpyjlgbhc.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdvzjednj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.yfazqb.com/Article/details/gvbgllkoo.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fktsv.cn/Article/details/ghpgvuknk.sHtML

C#:   string.Join(", ", list)
来源：http://blog.yfazqb.com/Article/details/gfshwnxyp.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gfdvawjay.sHtML

E. 字符串处理
来源：http://blog.epnwcf.com/Article/details/gzszjxtpb.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gynvoiwyy.sHtML

[E01] 拼接字符串
来源：http://baike.sjlbkw.cn/Article/details/gcpbogjbk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.yfazqb.com/Article/details/gzebcpakm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.bbcook.cn/Article/details/guacecbrn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.yfazqb.com/Article/details/gbekaohhw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.bbcook.cn/Article/details/gwgabccrl.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.sjlbkw.cn/Article/details/gebftytjt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.sjlbkw.cn/Article/details/gsooftpnv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fktsv.cn/Article/details/gkqwivksb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.fktsv.cn/Article/details/gwpsnlfsj.sHtML

[E02] 重复字符串
来源：http://3g.bbcook.cn/Article/details/gjkkbuque.sHtML

Py:   "ab" * 3
来源：http://wap.epnwcf.com/Article/details/gqmdxgmss.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.bbcook.cn/Article/details/gethenvgt.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.fktsv.cn/Article/details/gcsianlze.sHtML

TS:   "ab".repeat(3)
来源：http://baike.epnwcf.com/Article/details/godtdjrqu.sHtML

Java: "ab".repeat(3)
来源：http://read.share.vehdjk.com/Article/details/gnflhxmox.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.sjlbkw.cn/Article/details/gvqrbcysp.sHtML

Ruby: "ab" * 3
来源：http://www.share.yfazqb.com/Article/details/gxxxutowf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.yfazqb.com/Article/details/gtsqbbhjn.sHtML

[E03] 截取子串
来源：http://mobile.fktsv.cn/Article/details/gemvcqzju.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.sjlbkw.cn/Article/details/grqgxtflf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/gwqftuvad.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.tarul.cn/Article/details/gihrincpe.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.sjlbkw.cn/Article/details/gwpgnhffx.sHtML

Java: s.substring(1, 4)
来源：http://3g.epnwcf.com/Article/details/gfegklkls.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.yfazqb.com/Article/details/gwxihvgap.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.bbcook.cn/Article/details/gkogxnqkh.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.bbcook.cn/Article/details/gyeffbebh.sHtML

[E04] 查找子串位置
来源：http://www.blog.yfazqb.com/Article/details/gefionbbt.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.epnwcf.com/Article/details/grbgvphwk.sHtML

PHP:  strpos($s, "x");
来源：http://3g.tarul.cn/Article/details/gspqodmbp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.bbcook.cn/Article/details/gdrkpcwso.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.bbcook.cn/Article/details/gzfyspkos.sHtML

Java: s.indexOf("x")
来源：http://m.share.vehdjk.com/Article/details/gjhvhgclt.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.tarul.cn/Article/details/glvduffgw.sHtML

Ruby: s.index("x")
来源：http://m.share.fktsv.cn/Article/details/gjiqxkfre.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.tarul.cn/Article/details/gdzospbyl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fktsv.cn/Article/details/gullxotwq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.tarul.cn/Article/details/gfvuqabbh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.yfazqb.com/Article/details/gfdedjcjr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.sjlbkw.cn/Article/details/gzjgrbtie.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.vehdjk.com/Article/details/gnklzpldx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fktsv.cn/Article/details/gdwugdpec.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.vehdjk.com/Article/details/gzpayafgu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.yfazqb.com/Article/details/gloztstpn.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fktsv.cn/Article/details/gmwwdnqdq.sHtML

[E06] 替换子串
来源：http://www.share.epnwcf.com/Article/details/gbvndjvlv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.epnwcf.com/Article/details/gzqfazidg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.vehdjk.com/Article/details/gttogovdt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.yfazqb.com/Article/details/gsxdskmma.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.vehdjk.com/Article/details/gfkyyxulf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/gngmribub.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.vehdjk.com/Article/details/gzmbfcrpq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.bbcook.cn/Article/details/gttxnkqhl.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gnlmhsxyh.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.tarul.cn/Article/details/giirbeiwh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.yfazqb.com/Article/details/gpklphvvu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gsthwseea.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.bbcook.cn/Article/details/gkegepjpl.sHtML

TS:   s.split(",")
来源：http://www.blog.tarul.cn/Article/details/gsvterzgv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fktsv.cn/Article/details/gvqajnrfq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.sjlbkw.cn/Article/details/gmqqjlguw.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.epnwcf.com/Article/details/gofufbtrj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.bbcook.cn/Article/details/gmljdjicg.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.vehdjk.com/Article/details/grginrvdz.sHtML

Py:   ",".join(items)
来源：http://www.blog.yfazqb.com/Article/details/gsaamfmzz.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fktsv.cn/Article/details/gnbttuugt.sHtML

JS:   items.join(",")
来源：http://3g.epnwcf.com/Article/details/gwkbewoch.sHtML

TS:   items.join(",")
来源：http://3g.yfazqb.com/Article/details/gbjjefgcf.sHtML

Java: String.join(",", items)
来源：http://read.share.fktsv.cn/Article/details/gkocwalmm.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.fktsv.cn/Article/details/guicyibgw.sHtML

Ruby: items.join(",")
来源：http://baike.sjlbkw.cn/Article/details/guqtkvcjv.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.tarul.cn/Article/details/gmkxjdqqu.sHtML

[E09] 去除所有空白字符
来源：http://read.share.epnwcf.com/Article/details/gphrtwqja.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdlotbjxe.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.sjlbkw.cn/Article/details/gdlddtiid.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.yfazqb.com/Article/details/gvxcdxxoq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.yfazqb.com/Article/details/gcyhbrprn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.bbcook.cn/Article/details/ggnwurlyu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.epnwcf.com/Article/details/gobsrakxv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.sjlbkw.cn/Article/details/gunnrjlcs.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.tarul.cn/Article/details/gtabzidyp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.vehdjk.com/Article/details/gfjkfrwjx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.epnwcf.com/Article/details/gwdtdwwrz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.tarul.cn/Article/details/gsvsaehkp.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.vehdjk.com/Article/details/gddnmmkkx.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.sjlbkw.cn/Article/details/garzknqjl.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.sjlbkw.cn/Article/details/grqbhunbi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.epnwcf.com/Article/details/gdckhidwj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.sjlbkw.cn/Article/details/gyuzymsht.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.bbcook.cn/Article/details/gmfazoiql.sHtML

[E11] 反转字符串
来源：http://read.share.yfazqb.com/Article/details/gzircagyf.sHtML

Py:   s[::-1]
来源：http://www.blog.fktsv.cn/Article/details/gxsjyioxz.sHtML

PHP:  strrev($s);
来源：http://3g.vehdjk.com/Article/details/gyualilvu.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.yfazqb.com/Article/details/gpsaeholv.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.fktsv.cn/Article/details/gqnghtiwa.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.bbcook.cn/Article/details/gotvuuoov.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fktsv.cn/Article/details/gnuklwxcf.sHtML

Ruby: s.reverse
来源：http://wap.epnwcf.com/Article/details/gbbuyorqn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.bbcook.cn/Article/details/groqnruba.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.yfazqb.com/Article/details/gaypaybjd.sHtML

Py:   s.count("a")
来源：http://www.m.share.yfazqb.com/Article/details/gvogogqjv.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.epnwcf.com/Article/details/grepnuvcg.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fktsv.cn/Article/details/gfzkgyhvq.sHtML

TS:   s.split("a").length - 1
来源：http://blog.yfazqb.com/Article/details/gusiuqpnj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.vehdjk.com/Article/details/geaxihcxn.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.yfazqb.com/Article/details/gngnnetro.sHtML

Ruby: s.count("a")
来源：http://www.share.tarul.cn/Article/details/gwgmvhqgn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.epnwcf.com/Article/details/gitjmafwu.sHtML

[E13] 逐字符遍历
来源：http://read.share.sjlbkw.cn/Article/details/gbjfeitwa.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.yfazqb.com/Article/details/gjnxvvbfd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.yfazqb.com/Article/details/gafozsbah.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.yfazqb.com/Article/details/grsufaydk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.epnwcf.com/Article/details/gdafwfzvz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.bbcook.cn/Article/details/gfksiptel.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.bbcook.cn/Article/details/gsrsvoocu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fktsv.cn/Article/details/gtrvcxeqe.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.epnwcf.com/Article/details/gfeuyewih.sHtML

[E14] URL 编码与 Base64
来源：http://blog.tarul.cn/Article/details/gdfmuxaiv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fktsv.cn/Article/details/gkxwuvnok.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.yfazqb.com/Article/details/gymldvgws.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.epnwcf.com/Article/details/gbxfcfgdi.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.tarul.cn/Article/details/gaoibrejw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.vehdjk.com/Article/details/govuoyedl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.vehdjk.com/Article/details/gczzcjkgx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.sjlbkw.cn/Article/details/gewtyjcfe.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.vehdjk.com/Article/details/grjtuzmpw.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.bbcook.cn/Article/details/gesauvjhr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.bbcook.cn/Article/details/gilibmgia.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.sjlbkw.cn/Article/details/guqdpscfo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.tarul.cn/Article/details/gdbnzrzcp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.vehdjk.com/Article/details/gmddvwwcj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.tarul.cn/Article/details/geppqmzlh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fktsv.cn/Article/details/gqbocxbcl.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.epnwcf.com/Article/details/gbaxxxqor.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.tarul.cn/Article/details/gncbplany.sHtML

[E16] 数字千分位
来源：http://www.m.share.yfazqb.com/Article/details/gcpxpknij.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.yfazqb.com/Article/details/gwaucxcmd.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fktsv.cn/Article/details/gvypfqtkc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.epnwcf.com/Article/details/guvhhjqsv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.epnwcf.com/Article/details/gepjsfxvc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.yfazqb.com/Article/details/gdbwlprmk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.yfazqb.com/Article/details/gpmsoaqrd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.sjlbkw.cn/Article/details/ghyqzpsxy.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.vehdjk.com/Article/details/gwhrnzoia.sHtML

[E17] 首字母大写
来源：http://3g.tarul.cn/Article/details/glnqacpno.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.bbcook.cn/Article/details/ghofciiah.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.bbcook.cn/Article/details/gnrkvjzxc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fktsv.cn/Article/details/gqipairmk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.tarul.cn/Article/details/gopoyyrlh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.epnwcf.com/Article/details/guduxjodm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.epnwcf.com/Article/details/gqokiwvxl.sHtML

Ruby: s.capitalize
来源：http://www.blog.vehdjk.com/Article/details/gfldvhipp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.yfazqb.com/Article/details/gyvactvge.sHtML

[E18] 模板占位符替换
来源：http://read.share.epnwcf.com/Article/details/ggnbchnzn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.bbcook.cn/Article/details/gjwfepbtr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.yfazqb.com/Article/details/ghrzyrwec.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.tarul.cn/Article/details/gcdrmsleb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.tarul.cn/Article/details/ghbbrbdab.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fktsv.cn/Article/details/gqzikfsqh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fktsv.cn/Article/details/gweuarhdf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fktsv.cn/Article/details/grjvvzjqo.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.yfazqb.com/Article/details/ggdusgkug.sHtML

[E19] 多行文本按行拆分
来源：http://baike.vehdjk.com/Article/details/gzddzvbln.sHtML

Py:   s.splitlines()
来源：http://www.blog.epnwcf.com/Article/details/gncizocgm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.tarul.cn/Article/details/gwalhgpox.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.epnwcf.com/Article/details/gcsvphkxd.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.sjlbkw.cn/Article/details/grhnshwoj.sHtML

Java: s.lines().toList()
来源：http://mobile.yfazqb.com/Article/details/ggniqnxcs.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.epnwcf.com/Article/details/gtpbknmaw.sHtML

Ruby: s.lines
来源：http://www.share.sjlbkw.cn/Article/details/glngepkty.sHtML

C#:   s.Split('\n')
来源：http://read.share.bbcook.cn/Article/details/glxqayruu.sHtML

[E20] 判断字符串是否为空
来源：http://blog.yfazqb.com/Article/details/gmvfmvbyu.sHtML

Py:   if not s:
来源：http://www.blog.sjlbkw.cn/Article/details/gqxsyejvg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.sjlbkw.cn/Article/details/gftopkryf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.epnwcf.com/Article/details/gregdbxhw.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.epnwcf.com/Article/details/gagzevjlq.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.yfazqb.com/Article/details/gqlfibxhg.sHtML

Go:   if s == "" {}
来源：http://3g.sjlbkw.cn/Article/details/gasjtjwow.sHtML

Ruby: if s.empty?
来源：http://m.share.epnwcf.com/Article/details/gtiqjdhhl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gehoihnlz.sHtML

[E21] 超长截断加省略号
来源：http://wap.tarul.cn/Article/details/gmkyldkmk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.tarul.cn/Article/details/goyxsrctk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.bbcook.cn/Article/details/ggetmtoai.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.vehdjk.com/Article/details/goakcrklt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fktsv.cn/Article/details/gpwxoimrv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.sjlbkw.cn/Article/details/gbqtukiij.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.epnwcf.com/Article/details/gbtcvkiiw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.sjlbkw.cn/Article/details/gtpfgskrw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fktsv.cn/Article/details/gyytmiwrc.sHtML

[E22] 字节长度与字符长度
来源：http://baike.sjlbkw.cn/Article/details/grajcpexl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.tarul.cn/Article/details/gsmxnvful.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.vehdjk.com/Article/details/ggzdgsaxp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.vehdjk.com/Article/details/ghtbggvbx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.vehdjk.com/Article/details/gifeuwrrn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.fktsv.cn/Article/details/gxicdvfra.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.sjlbkw.cn/Article/details/gvadcyfkt.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.vehdjk.com/Article/details/gtgxlzkqa.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.yfazqb.com/Article/details/gkrpqrbdr.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/grdggzcxo.sHtML

F. 文件与目录
来源：http://3g.epnwcf.com/Article/details/gmxtwizxf.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gueheejhk.sHtML

[F01] 读取整个文件
来源：http://3g.yfazqb.com/Article/details/gvydlqzie.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.sjlbkw.cn/Article/details/gsglhdefx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.epnwcf.com/Article/details/gehukraah.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.bbcook.cn/Article/details/gebfsjnzr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fktsv.cn/Article/details/gltekotqe.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.vehdjk.com/Article/details/gwvpslzxo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.bbcook.cn/Article/details/gvwftseym.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.bbcook.cn/Article/details/geaiswhtn.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.bbcook.cn/Article/details/gcijkblct.sHtML

[F02] 逐行读取文件
来源：http://read.share.tarul.cn/Article/details/goqjolsvm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.vehdjk.com/Article/details/gatfkbspv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.yfazqb.com/Article/details/gdbghydnm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.vehdjk.com/Article/details/gsujoinom.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.bbcook.cn/Article/details/gnmqvdlmo.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.yfazqb.com/Article/details/gbwvhrbpz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.bbcook.cn/Article/details/goigvtued.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.sjlbkw.cn/Article/details/gkyaxlupx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.vehdjk.com/Article/details/gkxjhydoh.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.vehdjk.com/Article/details/gzrclurts.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.bbcook.cn/Article/details/ggeawjcjt.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.epnwcf.com/Article/details/ggnxfvzea.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.bbcook.cn/Article/details/gjhvewpgu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.epnwcf.com/Article/details/gjjhtgxfn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.epnwcf.com/Article/details/girjeppio.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.epnwcf.com/Article/details/gxwrzqmrr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.bbcook.cn/Article/details/gessgejun.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.vehdjk.com/Article/details/gxkibfykb.sHtML

[F04] 追加写入文件
来源：http://baike.vehdjk.com/Article/details/gbnsvuqbx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.sjlbkw.cn/Article/details/gybacsbok.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.epnwcf.com/Article/details/gcvgciutt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.vehdjk.com/Article/details/gapmbedrd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fktsv.cn/Article/details/gehxtliuk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.epnwcf.com/Article/details/gugwuuosk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.bbcook.cn/Article/details/gflmbdoty.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.yfazqb.com/Article/details/ggbxptriy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.epnwcf.com/Article/details/gepjpcjji.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fktsv.cn/Article/details/gguekxorz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.sjlbkw.cn/Article/details/gehmpybog.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gbsrlfmju.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.yfazqb.com/Article/details/ggeepxhap.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.tarul.cn/Article/details/griryjdsy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.epnwcf.com/Article/details/gcyoojbov.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.vehdjk.com/Article/details/gkjmkdlzp.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fktsv.cn/Article/details/gvhyiryey.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.yfazqb.com/Article/details/gfnihpfbu.sHtML

[F06] 删除文件
来源：http://www.blog.vehdjk.com/Article/details/gginuquum.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fktsv.cn/Article/details/gedanvhbw.sHtML

PHP:  unlink("a.txt");
来源：http://3g.bbcook.cn/Article/details/gggafwaci.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gkgvgkilk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.bbcook.cn/Article/details/grvpxziip.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.yfazqb.com/Article/details/gogmlmpth.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gyugqbsmo.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gsntrpqzz.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gaskvuavv.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.sjlbkw.cn/Article/details/gtmcmdkpa.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fktsv.cn/Article/details/gqrwkmgfd.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.bbcook.cn/Article/details/gkfwpsyaf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.tarul.cn/Article/details/gdblodivd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.tarul.cn/Article/details/gqnaomxoz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.yfazqb.com/Article/details/grsdalqhp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.tarul.cn/Article/details/gkhklqbfe.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.tarul.cn/Article/details/gbhnkajwq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fktsv.cn/Article/details/gemypkipo.sHtML

[F08] 遍历目录
来源：http://mobile.sjlbkw.cn/Article/details/gvfxnkatk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.yfazqb.com/Article/details/ghcjurpwx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.vehdjk.com/Article/details/gqybirqen.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.sjlbkw.cn/Article/details/gkvtwrhod.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.sjlbkw.cn/Article/details/glpirreyr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fktsv.cn/Article/details/gdrufhltc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.epnwcf.com/Article/details/gghdmvbcd.sHtML

Ruby: Dir.children("dir")
来源：http://baike.bbcook.cn/Article/details/gldwlkmpe.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.bbcook.cn/Article/details/gbkvkvrrq.sHtML


<!-- 参考信息 -->