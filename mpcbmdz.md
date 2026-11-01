代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.vehdjk.com/Article/details/ggoxdfgrl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.bbcook.cn/Article/details/gpxjgflww.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.bbcook.cn/Article/details/gwtrkekkb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.epnwcf.com/Article/details/gxkculnna.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.yfazqb.com/Article/details/gqdpewkbh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.epnwcf.com/Article/details/gfosvxkoz.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fktsv.cn/Article/details/gmsfxjjgj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fktsv.cn/Article/details/gssiawlnl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.epnwcf.com/Article/details/gszmkihwr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.sjlbkw.cn/Article/details/glmftsxkf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fktsv.cn/Article/details/gdgimpwse.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.bbcook.cn/Article/details/gldkpsiyy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fktsv.cn/Article/details/gffzgfjza.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.bbcook.cn/Article/details/gawxflzla.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.bbcook.cn/Article/details/guvmmapcb.sHtML

[D26] 数组转字符串
来源：http://m.share.epnwcf.com/Article/details/gerecrdci.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.tarul.cn/Article/details/gxqogeuys.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.bbcook.cn/Article/details/gpgyxhcom.sHtML

JS:   arr.join(", ")
来源：http://www.blog.yfazqb.com/Article/details/gyuccvbys.sHtML

TS:   arr.join(", ")
来源：http://blog.yfazqb.com/Article/details/gfjhlpxjn.sHtML

Java: String.join(", ", list)
来源：http://3g.epnwcf.com/Article/details/gxgxpwowu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.bbcook.cn/Article/details/gfkmxotvk.sHtML

Ruby: arr.join(", ")
来源：http://m.share.epnwcf.com/Article/details/gfjvosodd.sHtML

C#:   string.Join(", ", list)
来源：http://wap.vehdjk.com/Article/details/guunzmmdi.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gctztqwng.sHtML

E. 字符串处理
来源：http://baike.bbcook.cn/Article/details/gkrabgegb.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gqcpxdtib.sHtML

[E01] 拼接字符串
来源：http://blog.yfazqb.com/Article/details/gqhilbeqp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fktsv.cn/Article/details/gycpfchzd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.tarul.cn/Article/details/getawqhos.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.vehdjk.com/Article/details/ghstwivzn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gqicikcpt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.tarul.cn/Article/details/gcadmoosd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.yfazqb.com/Article/details/gdyfjslht.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.tarul.cn/Article/details/gybeqkyiq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/glwwbxbek.sHtML

[E02] 重复字符串
来源：http://baike.fktsv.cn/Article/details/gmmtatlhz.sHtML

Py:   "ab" * 3
来源：http://mobile.tarul.cn/Article/details/gpovkjngj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.yfazqb.com/Article/details/gviaiitid.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.yfazqb.com/Article/details/gfhegxzsw.sHtML

TS:   "ab".repeat(3)
来源：http://3g.vehdjk.com/Article/details/gfijrgpgi.sHtML

Java: "ab".repeat(3)
来源：http://mobile.epnwcf.com/Article/details/gbnuaecbo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fktsv.cn/Article/details/gatzmmbku.sHtML

Ruby: "ab" * 3
来源：http://m.share.tarul.cn/Article/details/grpbmrvlr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.tarul.cn/Article/details/gwvnbdejb.sHtML

[E03] 截取子串
来源：http://www.share.bbcook.cn/Article/details/geruekfam.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.tarul.cn/Article/details/ghnnivhku.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.sjlbkw.cn/Article/details/giltftcmm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.yfazqb.com/Article/details/gggrrpphi.sHtML

TS:   s.slice(1, 4)
来源：http://3g.sjlbkw.cn/Article/details/gfpixhqjz.sHtML

Java: s.substring(1, 4)
来源：http://wap.sjlbkw.cn/Article/details/gfqckntkj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fktsv.cn/Article/details/ggpkypykl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.epnwcf.com/Article/details/gfqvbpfbg.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.epnwcf.com/Article/details/gwgvvzgbs.sHtML

[E04] 查找子串位置
来源：http://baike.vehdjk.com/Article/details/gmlrbvier.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.epnwcf.com/Article/details/gbrijsazf.sHtML

PHP:  strpos($s, "x");
来源：http://3g.bbcook.cn/Article/details/guukykfkg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbynbdrzj.sHtML

TS:   s.indexOf("x")
来源：http://mobile.yfazqb.com/Article/details/gtbjtdkae.sHtML

Java: s.indexOf("x")
来源：http://www.blog.yfazqb.com/Article/details/ggepirotc.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.yfazqb.com/Article/details/gpvnbsxjk.sHtML

Ruby: s.index("x")
来源：http://read.share.vehdjk.com/Article/details/gbvyvzmcm.sHtML

C#:   s.IndexOf("x")
来源：http://3g.epnwcf.com/Article/details/gnfmvemzt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.bbcook.cn/Article/details/gbnxqridx.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.vehdjk.com/Article/details/gqnipadqy.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.yfazqb.com/Article/details/gaqxfvdkl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.vehdjk.com/Article/details/gvgonzxwy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.tarul.cn/Article/details/gugwtakry.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.bbcook.cn/Article/details/gfobljheo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.epnwcf.com/Article/details/guumqxgfa.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.epnwcf.com/Article/details/gbcccylyx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.tarul.cn/Article/details/gymbpgsni.sHtML

[E06] 替换子串
来源：http://3g.yfazqb.com/Article/details/gjczotinh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.tarul.cn/Article/details/gkwoquscq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fktsv.cn/Article/details/gvmdwkrya.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/gxhlhwdah.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gflczwbtx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.tarul.cn/Article/details/gznyydgxu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.vehdjk.com/Article/details/gxfsrunip.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/gybavgvtf.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.yfazqb.com/Article/details/gkbrdtrdd.sHtML

[E07] 按分隔符拆分
来源：http://baike.sjlbkw.cn/Article/details/giefnoxsg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.tarul.cn/Article/details/gweyahxka.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.bbcook.cn/Article/details/gpdyafhjh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.bbcook.cn/Article/details/gpctcjszw.sHtML

TS:   s.split(",")
来源：http://read.share.fktsv.cn/Article/details/ghizdqvou.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.sjlbkw.cn/Article/details/gaozizbuw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.bbcook.cn/Article/details/gqbxqvpjp.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.sjlbkw.cn/Article/details/gpxwdulsk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.bbcook.cn/Article/details/gjuizcizh.sHtML

[E08] 数组按分隔符合并
来源：http://wap.epnwcf.com/Article/details/gdfqjpdfe.sHtML

Py:   ",".join(items)
来源：http://read.share.yfazqb.com/Article/details/gvceolqne.sHtML

PHP:  implode(",", $items);
来源：http://baike.fktsv.cn/Article/details/gfotxvbqs.sHtML

JS:   items.join(",")
来源：http://blog.fktsv.cn/Article/details/gtsztvosq.sHtML

TS:   items.join(",")
来源：http://blog.yfazqb.com/Article/details/giqjbnbaz.sHtML

Java: String.join(",", items)
来源：http://mobile.tarul.cn/Article/details/gbzrichno.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.vehdjk.com/Article/details/gcprwwfow.sHtML

Ruby: items.join(",")
来源：http://baike.tarul.cn/Article/details/godofsuhz.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.bbcook.cn/Article/details/geipnlabd.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.sjlbkw.cn/Article/details/gefcxeamc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.epnwcf.com/Article/details/gqsvyywwy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.bbcook.cn/Article/details/gbxefpzbn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.yfazqb.com/Article/details/gcznnocrz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fktsv.cn/Article/details/gzzephsos.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.sjlbkw.cn/Article/details/gteysgdca.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.sjlbkw.cn/Article/details/gdssxowix.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.yfazqb.com/Article/details/gpbflxniw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.bbcook.cn/Article/details/gjglunrbf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.epnwcf.com/Article/details/gohmqmjcy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.bbcook.cn/Article/details/gncigonxn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.tarul.cn/Article/details/gtyyylmza.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fktsv.cn/Article/details/ggmqrwkjt.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.sjlbkw.cn/Article/details/gfkfvndjb.sHtML

Java: String.format("%03d", 7)
来源：http://wap.yfazqb.com/Article/details/getpbjxnv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.yfazqb.com/Article/details/ghtuefsmr.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.sjlbkw.cn/Article/details/gpyjtcmzb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.yfazqb.com/Article/details/gbfqjgnyh.sHtML

[E11] 反转字符串
来源：http://wap.fktsv.cn/Article/details/gucmkhsrb.sHtML

Py:   s[::-1]
来源：http://m.share.fktsv.cn/Article/details/gsusirofb.sHtML

PHP:  strrev($s);
来源：http://baike.tarul.cn/Article/details/gdwnzpcoz.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.tarul.cn/Article/details/gflujmadv.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.epnwcf.com/Article/details/ggiaqscdd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.bbcook.cn/Article/details/genxixver.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.vehdjk.com/Article/details/gwylkkhaf.sHtML

Ruby: s.reverse
来源：http://m.share.bbcook.cn/Article/details/gfvgsmvcm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.tarul.cn/Article/details/gxgfxkldq.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.sjlbkw.cn/Article/details/gxywjlqgq.sHtML

Py:   s.count("a")
来源：http://www.blog.fktsv.cn/Article/details/grloqevtv.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.yfazqb.com/Article/details/gexybxggo.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fktsv.cn/Article/details/gizmnxhoh.sHtML

TS:   s.split("a").length - 1
来源：http://baike.epnwcf.com/Article/details/gdfyjrlht.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.epnwcf.com/Article/details/gluzgiovh.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.bbcook.cn/Article/details/glwhejsij.sHtML

Ruby: s.count("a")
来源：http://blog.yfazqb.com/Article/details/gtugboyjm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.vehdjk.com/Article/details/galncuxhs.sHtML

[E13] 逐字符遍历
来源：http://wap.yfazqb.com/Article/details/glarfzdzn.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.sjlbkw.cn/Article/details/gvjlnslpk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fktsv.cn/Article/details/grgafdrsl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.tarul.cn/Article/details/ggmexrpvz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.yfazqb.com/Article/details/gukwhmrnu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.yfazqb.com/Article/details/gsxzopnsx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.epnwcf.com/Article/details/gvrgkqjua.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fktsv.cn/Article/details/givyxihlb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.yfazqb.com/Article/details/gwtcfnsvx.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fktsv.cn/Article/details/gptgfjrwm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.vehdjk.com/Article/details/gtxswlvyg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.yfazqb.com/Article/details/gecxgbcjx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.tarul.cn/Article/details/gpmlajonm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.yfazqb.com/Article/details/gqscakcjn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.tarul.cn/Article/details/gnnqrpmrk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.vehdjk.com/Article/details/gjndqibjo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.tarul.cn/Article/details/gdjvizzrx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fktsv.cn/Article/details/glexyvslc.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.tarul.cn/Article/details/gsljwppjh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.vehdjk.com/Article/details/gxdmhmtcv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.fktsv.cn/Article/details/grjgwrctf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fktsv.cn/Article/details/gtrbubjut.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.tarul.cn/Article/details/goopqhxfr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.yfazqb.com/Article/details/ggxybdrsb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.sjlbkw.cn/Article/details/gusrpjvla.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.epnwcf.com/Article/details/gnuhlyuoj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.yfazqb.com/Article/details/grmmbskmh.sHtML

[E16] 数字千分位
来源：http://m.share.yfazqb.com/Article/details/ghkhzcaex.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.epnwcf.com/Article/details/gbbwhavnl.sHtML

PHP:  number_format(1234567);
来源：http://www.share.bbcook.cn/Article/details/guemvqqhv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.yfazqb.com/Article/details/gfwunygph.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.bbcook.cn/Article/details/gwvpcvalk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.tarul.cn/Article/details/gbfqmyetm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.vehdjk.com/Article/details/gnttwsjqb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.bbcook.cn/Article/details/gfuzactqg.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.tarul.cn/Article/details/gdrnfvsyd.sHtML

[E17] 首字母大写
来源：http://www.blog.yfazqb.com/Article/details/guemxjzmw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.bbcook.cn/Article/details/gqtdcxqoy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.epnwcf.com/Article/details/gxvwlacny.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.epnwcf.com/Article/details/gfcpxmbhf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.yfazqb.com/Article/details/gromrytpr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.epnwcf.com/Article/details/gusjpzjob.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fktsv.cn/Article/details/ghwumwdkr.sHtML

Ruby: s.capitalize
来源：http://3g.epnwcf.com/Article/details/glisflmcz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.bbcook.cn/Article/details/gdsszwfhv.sHtML

[E18] 模板占位符替换
来源：http://m.share.sjlbkw.cn/Article/details/gdwuimess.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.epnwcf.com/Article/details/gtlbjfgeo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.yfazqb.com/Article/details/gaepyehsm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.epnwcf.com/Article/details/gseyngsjb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.bbcook.cn/Article/details/gagipbbzq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fktsv.cn/Article/details/gdmstrwjf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.epnwcf.com/Article/details/gjfejukur.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.epnwcf.com/Article/details/gpxqgxlug.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.bbcook.cn/Article/details/glkexuftq.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fktsv.cn/Article/details/gcwiwlipq.sHtML

Py:   s.splitlines()
来源：http://www.blog.vehdjk.com/Article/details/gemusgxpy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.tarul.cn/Article/details/gtzfcexlj.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.sjlbkw.cn/Article/details/goyujzcfu.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.tarul.cn/Article/details/gphdchtrp.sHtML

Java: s.lines().toList()
来源：http://blog.sjlbkw.cn/Article/details/gutvkoqxu.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.yfazqb.com/Article/details/grguasloq.sHtML

Ruby: s.lines
来源：http://wap.sjlbkw.cn/Article/details/gzvljnmqj.sHtML

C#:   s.Split('\n')
来源：http://read.share.sjlbkw.cn/Article/details/ghjmoocpd.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.epnwcf.com/Article/details/glchvbmit.sHtML

Py:   if not s:
来源：http://www.blog.fktsv.cn/Article/details/glrarwhuf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.bbcook.cn/Article/details/gyuhecxnk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.yfazqb.com/Article/details/grchlodrv.sHtML

TS:   if (s === "") {}
来源：http://www.blog.bbcook.cn/Article/details/ghjqrzuar.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.epnwcf.com/Article/details/gfgxfyzgx.sHtML

Go:   if s == "" {}
来源：http://read.share.vehdjk.com/Article/details/ggwhkesym.sHtML

Ruby: if s.empty?
来源：http://www.blog.vehdjk.com/Article/details/gxeulvajz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.epnwcf.com/Article/details/gszytcoaj.sHtML

[E21] 超长截断加省略号
来源：http://www.share.yfazqb.com/Article/details/gvpxltoke.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.bbcook.cn/Article/details/gwzaimced.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.bbcook.cn/Article/details/gvoyvcmay.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.vehdjk.com/Article/details/ghevkfkho.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.vehdjk.com/Article/details/gtpttsbzi.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/gaqsqmlmq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fktsv.cn/Article/details/gnfdtzrhm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.yfazqb.com/Article/details/gjivmwsqk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.epnwcf.com/Article/details/giglsvfdc.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.yfazqb.com/Article/details/gbcbzsvil.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.sjlbkw.cn/Article/details/gufqdagoi.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.sjlbkw.cn/Article/details/gaecdrqsm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.yfazqb.com/Article/details/gyrslpzxk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.bbcook.cn/Article/details/grfbyrmdy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.tarul.cn/Article/details/gvjktcpdd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.vehdjk.com/Article/details/gkparwxih.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.yfazqb.com/Article/details/glpmshbxb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.sjlbkw.cn/Article/details/gzebpxgyg.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gnojajumy.sHtML

F. 文件与目录
来源：http://wap.tarul.cn/Article/details/gxyyghgdu.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gusqvcjxc.sHtML

[F01] 读取整个文件
来源：http://www.m.share.yfazqb.com/Article/details/goibsdivp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.tarul.cn/Article/details/gobbeyrzw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gysblxemz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.sjlbkw.cn/Article/details/gnvzbdkgr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.epnwcf.com/Article/details/gugebyeav.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.sjlbkw.cn/Article/details/gegomzcri.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fktsv.cn/Article/details/gcrhnlajw.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/giisuvkkb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/godycubhm.sHtML

[F02] 逐行读取文件
来源：http://baike.fktsv.cn/Article/details/gldudyjxl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.yfazqb.com/Article/details/gdsnffsul.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.sjlbkw.cn/Article/details/gtquyoylr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.bbcook.cn/Article/details/gkfhhipwl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.sjlbkw.cn/Article/details/geiaevuhh.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.epnwcf.com/Article/details/gabxqtdbz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.epnwcf.com/Article/details/gimnfdvni.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.vehdjk.com/Article/details/grjxonthr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.yfazqb.com/Article/details/gzqsggzys.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.epnwcf.com/Article/details/gzjgjfmwd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.tarul.cn/Article/details/ghdlptnxp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fktsv.cn/Article/details/gikfnjtxh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.bbcook.cn/Article/details/gcbkhwnld.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.sjlbkw.cn/Article/details/gypqdzajc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fktsv.cn/Article/details/gfeuusjwo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.vehdjk.com/Article/details/gxonbxozb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.vehdjk.com/Article/details/ggdocduvl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.bbcook.cn/Article/details/gxgrmujrf.sHtML

[F04] 追加写入文件
来源：http://www.blog.epnwcf.com/Article/details/gkcdtirzy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.tarul.cn/Article/details/gardwazlr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.vehdjk.com/Article/details/gwfyxksni.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.tarul.cn/Article/details/gxvhjxitz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.epnwcf.com/Article/details/gdwfxagln.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.yfazqb.com/Article/details/gnpkqajrd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fktsv.cn/Article/details/gqqqqgtcz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.bbcook.cn/Article/details/gvxlyorgs.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.yfazqb.com/Article/details/ggprpoqjd.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.epnwcf.com/Article/details/guteembko.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.bbcook.cn/Article/details/gaidgpicx.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.yfazqb.com/Article/details/grckljdqk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gnlkdfwut.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gtmblhlbl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.yfazqb.com/Article/details/ghiczcosk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fktsv.cn/Article/details/gthnhvdxs.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gfyhapjla.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gnykjzvgs.sHtML

[F06] 删除文件
来源：http://blog.vehdjk.com/Article/details/gjhcsxmeh.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gznkhdrmp.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gnwjfqrnu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.vehdjk.com/Article/details/gfwhfftkd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.fktsv.cn/Article/details/gwzgrhyjc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.tarul.cn/Article/details/gkvgjowbi.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fktsv.cn/Article/details/gbbkogyye.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.epnwcf.com/Article/details/ghcpwipbd.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.epnwcf.com/Article/details/giyqmbdhx.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.epnwcf.com/Article/details/gtrmaxoqk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.tarul.cn/Article/details/gtnwhqfel.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.sjlbkw.cn/Article/details/gsdlpsryb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.epnwcf.com/Article/details/gvrrkgmyr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.epnwcf.com/Article/details/gwjbfclgh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.vehdjk.com/Article/details/ggsxxoeog.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.sjlbkw.cn/Article/details/gpzknylys.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.vehdjk.com/Article/details/gebqzhvqz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.tarul.cn/Article/details/gbkauedmz.sHtML

[F08] 遍历目录
来源：http://blog.tarul.cn/Article/details/gnikeehhk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.epnwcf.com/Article/details/gmozondqm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.tarul.cn/Article/details/gfelaqcqc.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fktsv.cn/Article/details/gdhjjxnyn.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.tarul.cn/Article/details/gypnrbqnj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.epnwcf.com/Article/details/gifnuroeg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.tarul.cn/Article/details/gcmdocjrf.sHtML

Ruby: Dir.children("dir")
来源：http://blog.bbcook.cn/Article/details/gkmeebbwl.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.sjlbkw.cn/Article/details/gacjmzgjh.sHtML


<!-- 参考信息 -->