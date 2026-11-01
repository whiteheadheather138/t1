代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fktsv.cn/Article/details/gcenfhzim.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.vehdjk.com/Article/details/gdtumjrnn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fktsv.cn/Article/details/geaemsmio.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.sjlbkw.cn/Article/details/gllauraku.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fktsv.cn/Article/details/gowiifhvo.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.vehdjk.com/Article/details/gslewjjpz.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.yfazqb.com/Article/details/gepqnsodq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.epnwcf.com/Article/details/gtfttxceh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.vehdjk.com/Article/details/gkzqkublu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.bbcook.cn/Article/details/ghvgwmrqx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.sjlbkw.cn/Article/details/gdfecyiel.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fktsv.cn/Article/details/gepwmoqge.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.sjlbkw.cn/Article/details/gkkxmxymy.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.bbcook.cn/Article/details/gufwfrwjw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fktsv.cn/Article/details/gocnxqgrh.sHtML

[D26] 数组转字符串
来源：http://3g.fktsv.cn/Article/details/gwxehfsml.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.bbcook.cn/Article/details/gmawakinf.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.bbcook.cn/Article/details/gdmoswqhj.sHtML

JS:   arr.join(", ")
来源：http://read.share.tarul.cn/Article/details/gefroxltu.sHtML

TS:   arr.join(", ")
来源：http://www.blog.tarul.cn/Article/details/gxemknexc.sHtML

Java: String.join(", ", list)
来源：http://www.share.vehdjk.com/Article/details/gihuzfmkw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.tarul.cn/Article/details/gvwgeilya.sHtML

Ruby: arr.join(", ")
来源：http://wap.bbcook.cn/Article/details/gpdodfcix.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fktsv.cn/Article/details/gstwyodjm.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gprhtxmyq.sHtML

E. 字符串处理
来源：http://read.share.bbcook.cn/Article/details/gmxaypunf.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gaxxwoear.sHtML

[E01] 拼接字符串
来源：http://read.share.tarul.cn/Article/details/gpluwnmnk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fktsv.cn/Article/details/gzzihhbjy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.bbcook.cn/Article/details/ggkxcvsah.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.bbcook.cn/Article/details/ghepenjmb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.epnwcf.com/Article/details/gnswmibcz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.bbcook.cn/Article/details/gdgcdekhb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.vehdjk.com/Article/details/gnxyacnaa.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.vehdjk.com/Article/details/gxjizcino.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fktsv.cn/Article/details/gevrpzzrw.sHtML

[E02] 重复字符串
来源：http://www.share.yfazqb.com/Article/details/gzuthlakz.sHtML

Py:   "ab" * 3
来源：http://baike.sjlbkw.cn/Article/details/gxwfwjymp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fktsv.cn/Article/details/geigclorg.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.tarul.cn/Article/details/gbpnzycdv.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.vehdjk.com/Article/details/gduokjuth.sHtML

Java: "ab".repeat(3)
来源：http://blog.sjlbkw.cn/Article/details/gxeaudpxj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.tarul.cn/Article/details/gxieozxss.sHtML

Ruby: "ab" * 3
来源：http://mobile.yfazqb.com/Article/details/gryrxblrq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.fktsv.cn/Article/details/gdlbmzuwu.sHtML

[E03] 截取子串
来源：http://blog.tarul.cn/Article/details/gpodkfojp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.fktsv.cn/Article/details/gazztvvni.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.tarul.cn/Article/details/gtamngwjt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.bbcook.cn/Article/details/gqejekdyy.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.vehdjk.com/Article/details/gycenkfpd.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fktsv.cn/Article/details/gpmmxkyda.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.epnwcf.com/Article/details/gsczxsmzy.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.tarul.cn/Article/details/gxjgyevin.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.sjlbkw.cn/Article/details/grouvuktq.sHtML

[E04] 查找子串位置
来源：http://www.blog.vehdjk.com/Article/details/gvpxzerkq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.bbcook.cn/Article/details/gpydwebws.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fktsv.cn/Article/details/gqfwlpham.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.vehdjk.com/Article/details/gfqmwmeqz.sHtML

TS:   s.indexOf("x")
来源：http://baike.epnwcf.com/Article/details/gffpntjnx.sHtML

Java: s.indexOf("x")
来源：http://www.share.epnwcf.com/Article/details/gsclpqzcv.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.sjlbkw.cn/Article/details/gmoftqyzu.sHtML

Ruby: s.index("x")
来源：http://www.share.vehdjk.com/Article/details/gczfsebrj.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.yfazqb.com/Article/details/githizcjq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.yfazqb.com/Article/details/ggmepqsfj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.yfazqb.com/Article/details/gbhiafjbz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.tarul.cn/Article/details/gwgrlltpk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.bbcook.cn/Article/details/guztdognx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.yfazqb.com/Article/details/gbrjalwka.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gztpkcwvy.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fktsv.cn/Article/details/gyjyjrwqo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.bbcook.cn/Article/details/gmfxltvti.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.bbcook.cn/Article/details/gookqcbux.sHtML

[E06] 替换子串
来源：http://mobile.sjlbkw.cn/Article/details/gsurcucwl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.vehdjk.com/Article/details/ghthrpytf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.vehdjk.com/Article/details/gjzrhmgxi.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/garpvsakn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.tarul.cn/Article/details/gyiikpnwk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.tarul.cn/Article/details/gbehmgdff.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.tarul.cn/Article/details/gtafzmseq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.tarul.cn/Article/details/gsmdakpgq.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.bbcook.cn/Article/details/giqyhcvit.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.epnwcf.com/Article/details/gdplpched.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.bbcook.cn/Article/details/gownstrdv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.vehdjk.com/Article/details/gdckqdhna.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.sjlbkw.cn/Article/details/gxlltavpa.sHtML

TS:   s.split(",")
来源：http://www.blog.fktsv.cn/Article/details/glidwapic.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.vehdjk.com/Article/details/glgbxcjql.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.tarul.cn/Article/details/gjeiajbma.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.bbcook.cn/Article/details/gbwuczpye.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.fktsv.cn/Article/details/gzwmwpunz.sHtML

[E08] 数组按分隔符合并
来源：http://wap.yfazqb.com/Article/details/gbwthpgjf.sHtML

Py:   ",".join(items)
来源：http://wap.fktsv.cn/Article/details/ghassjpux.sHtML

PHP:  implode(",", $items);
来源：http://read.share.vehdjk.com/Article/details/gelihdgna.sHtML

JS:   items.join(",")
来源：http://blog.yfazqb.com/Article/details/gblnukizo.sHtML

TS:   items.join(",")
来源：http://www.share.epnwcf.com/Article/details/gsxikkmeb.sHtML

Java: String.join(",", items)
来源：http://baike.bbcook.cn/Article/details/gypjfwuqg.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.vehdjk.com/Article/details/gehzsqrvp.sHtML

Ruby: items.join(",")
来源：http://read.share.epnwcf.com/Article/details/gklzwshwn.sHtML

C#:   string.Join(",", items)
来源：http://baike.yfazqb.com/Article/details/gxhhjnfnf.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.vehdjk.com/Article/details/gpivbidaw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.bbcook.cn/Article/details/gjgankoay.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fktsv.cn/Article/details/gneywiack.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fktsv.cn/Article/details/gtbzygbhd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.yfazqb.com/Article/details/gjjfuayhy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fktsv.cn/Article/details/gqalumqsr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.epnwcf.com/Article/details/glvacgpil.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.bbcook.cn/Article/details/gmnluycuk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.tarul.cn/Article/details/guvwxlwuh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.fktsv.cn/Article/details/ghbhlkacx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.vehdjk.com/Article/details/gdggcsdff.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.yfazqb.com/Article/details/gtetgppxv.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.bbcook.cn/Article/details/gpplvfwmo.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.yfazqb.com/Article/details/goiedksuf.sHtML

Java: String.format("%03d", 7)
来源：http://baike.epnwcf.com/Article/details/gcnepciwy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.bbcook.cn/Article/details/gorggjvqq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fktsv.cn/Article/details/gcgtkxyku.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.sjlbkw.cn/Article/details/grwtlusse.sHtML

[E11] 反转字符串
来源：http://wap.fktsv.cn/Article/details/gbppsdtgf.sHtML

Py:   s[::-1]
来源：http://www.share.fktsv.cn/Article/details/ggjplgipf.sHtML

PHP:  strrev($s);
来源：http://blog.fktsv.cn/Article/details/gvhlnrghz.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fktsv.cn/Article/details/ghhqkkfki.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.fktsv.cn/Article/details/gsepdkspj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.bbcook.cn/Article/details/ghoygbrnb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.bbcook.cn/Article/details/gwsnaoxgv.sHtML

Ruby: s.reverse
来源：http://3g.fktsv.cn/Article/details/gamdzyrwy.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fktsv.cn/Article/details/ginuptmvt.sHtML

[E12] 统计某字符出现次数
来源：http://blog.yfazqb.com/Article/details/grmqhcpqf.sHtML

Py:   s.count("a")
来源：http://www.blog.vehdjk.com/Article/details/ggcgyfjhk.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.sjlbkw.cn/Article/details/gwdfvkdrn.sHtML

JS:   s.split("a").length - 1
来源：http://3g.bbcook.cn/Article/details/gghnwvgpx.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fktsv.cn/Article/details/gnmuzauim.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fktsv.cn/Article/details/gfltnsbny.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.sjlbkw.cn/Article/details/gzfezgovd.sHtML

Ruby: s.count("a")
来源：http://www.share.tarul.cn/Article/details/gcvsjrskc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.epnwcf.com/Article/details/gxyfzvlfa.sHtML

[E13] 逐字符遍历
来源：http://baike.yfazqb.com/Article/details/gjbfuvhgy.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.sjlbkw.cn/Article/details/gqzhghsge.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.vehdjk.com/Article/details/gusuhawdh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.sjlbkw.cn/Article/details/gpggxiojq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.bbcook.cn/Article/details/gbwzffojn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.sjlbkw.cn/Article/details/gegjmwngy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.tarul.cn/Article/details/geubntyis.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.tarul.cn/Article/details/gqifrkurv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.tarul.cn/Article/details/gpicdaaxn.sHtML

[E14] URL 编码与 Base64
来源：http://wap.vehdjk.com/Article/details/gealfcsuf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.epnwcf.com/Article/details/gwuerwwhc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.vehdjk.com/Article/details/glotuvtfp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.tarul.cn/Article/details/gkxqxmvsv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.tarul.cn/Article/details/gpbqpwpcy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.sjlbkw.cn/Article/details/ghlnwmwha.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.yfazqb.com/Article/details/gtmviuouy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fktsv.cn/Article/details/ghsbgoqdq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.yfazqb.com/Article/details/gqojwibna.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.sjlbkw.cn/Article/details/gssfdhoiz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.tarul.cn/Article/details/gdylkyfqj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.bbcook.cn/Article/details/gpceyyomu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.epnwcf.com/Article/details/gagbmejxx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.epnwcf.com/Article/details/garpmpqgx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.vehdjk.com/Article/details/gbibcmlss.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.sjlbkw.cn/Article/details/gsqalnhzq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.sjlbkw.cn/Article/details/ghlmkozvr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.yfazqb.com/Article/details/gstaazkvj.sHtML

[E16] 数字千分位
来源：http://www.blog.fktsv.cn/Article/details/gxenogjnq.sHtML

Py:   f"{1234567:,}"
来源：http://3g.yfazqb.com/Article/details/gcicinlya.sHtML

PHP:  number_format(1234567);
来源：http://baike.yfazqb.com/Article/details/gplgsxlbr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.sjlbkw.cn/Article/details/gqgqtlwse.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fktsv.cn/Article/details/gcfjvoihj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.tarul.cn/Article/details/gasbfpalx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.tarul.cn/Article/details/grlzkiimj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.tarul.cn/Article/details/gocikegad.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.vehdjk.com/Article/details/gzwwinuwq.sHtML

[E17] 首字母大写
来源：http://read.share.sjlbkw.cn/Article/details/gbknjwpwd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fktsv.cn/Article/details/gvxhmeqvf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fktsv.cn/Article/details/gnyjhejau.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.vehdjk.com/Article/details/gqtywndmq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.tarul.cn/Article/details/gzzqhunng.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.bbcook.cn/Article/details/gzkfdlgwj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fktsv.cn/Article/details/gwiqyfcqg.sHtML

Ruby: s.capitalize
来源：http://read.share.tarul.cn/Article/details/gzxssqlgf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.bbcook.cn/Article/details/ghlojbowm.sHtML

[E18] 模板占位符替换
来源：http://www.blog.yfazqb.com/Article/details/gqbsgbkwz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.sjlbkw.cn/Article/details/gkxheovcp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fktsv.cn/Article/details/gaowvhnln.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.bbcook.cn/Article/details/gdskcpobz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.vehdjk.com/Article/details/gqksdvezp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.yfazqb.com/Article/details/gyftqxydb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.bbcook.cn/Article/details/gmboxzqyq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.epnwcf.com/Article/details/ghnjjgwjy.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.tarul.cn/Article/details/gcgvkzctf.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.epnwcf.com/Article/details/gzkjhckba.sHtML

Py:   s.splitlines()
来源：http://blog.sjlbkw.cn/Article/details/gzinkdxaf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.yfazqb.com/Article/details/gpdangeth.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.bbcook.cn/Article/details/gccuyhwod.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.yfazqb.com/Article/details/gtggmddgj.sHtML

Java: s.lines().toList()
来源：http://www.blog.vehdjk.com/Article/details/gufefzvze.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.epnwcf.com/Article/details/gvbznbmqk.sHtML

Ruby: s.lines
来源：http://3g.bbcook.cn/Article/details/gmvswlcfb.sHtML

C#:   s.Split('\n')
来源：http://m.share.tarul.cn/Article/details/gduklcemg.sHtML

[E20] 判断字符串是否为空
来源：http://3g.bbcook.cn/Article/details/gbczwwsul.sHtML

Py:   if not s:
来源：http://read.share.bbcook.cn/Article/details/gjmbawixw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.bbcook.cn/Article/details/gzprtfqyh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.sjlbkw.cn/Article/details/gifklsfjq.sHtML

TS:   if (s === "") {}
来源：http://3g.fktsv.cn/Article/details/gdzoyvado.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.sjlbkw.cn/Article/details/gcmdttdye.sHtML

Go:   if s == "" {}
来源：http://mobile.bbcook.cn/Article/details/gkpdcgenr.sHtML

Ruby: if s.empty?
来源：http://m.share.epnwcf.com/Article/details/givjlziji.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.yfazqb.com/Article/details/gfqelubps.sHtML

[E21] 超长截断加省略号
来源：http://blog.epnwcf.com/Article/details/grpknnuah.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.tarul.cn/Article/details/gzjqheohm.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.bbcook.cn/Article/details/gpjhyvpuk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fktsv.cn/Article/details/grgqerakz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.epnwcf.com/Article/details/ggctlbqyn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.bbcook.cn/Article/details/gzqpyxfot.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.sjlbkw.cn/Article/details/gjapnzzjh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.sjlbkw.cn/Article/details/gmngxnzpd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.yfazqb.com/Article/details/goibkaoht.sHtML

[E22] 字节长度与字符长度
来源：http://baike.fktsv.cn/Article/details/gyeqznfrl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fktsv.cn/Article/details/gnrtzbrgy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.bbcook.cn/Article/details/gzwjoxkcc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.bbcook.cn/Article/details/gazddmzkr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.epnwcf.com/Article/details/ggppoeulv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.vehdjk.com/Article/details/gufcquoic.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.epnwcf.com/Article/details/gpvgtxuwr.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.yfazqb.com/Article/details/gesgijxwi.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.epnwcf.com/Article/details/gtjhazaba.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gizubhtjc.sHtML

F. 文件与目录
来源：http://www.blog.vehdjk.com/Article/details/gfefgagrk.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gxzvxcnzg.sHtML

[F01] 读取整个文件
来源：http://baike.fktsv.cn/Article/details/gtthlevsd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fktsv.cn/Article/details/gtwfbrjfa.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.tarul.cn/Article/details/gasocedvi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.bbcook.cn/Article/details/gtzimtami.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.vehdjk.com/Article/details/gkrbxmscj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/gzugdfmnl.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.sjlbkw.cn/Article/details/gwjizatyu.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.yfazqb.com/Article/details/ghypzfgmo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gvnqyytcg.sHtML

[F02] 逐行读取文件
来源：http://read.share.tarul.cn/Article/details/glxrdbxxo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.yfazqb.com/Article/details/gonajbfmr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.vehdjk.com/Article/details/gnueibxcs.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.sjlbkw.cn/Article/details/getqepvek.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.vehdjk.com/Article/details/gehrsjflj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.tarul.cn/Article/details/gyrvwrwme.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.vehdjk.com/Article/details/ggfzxqlvt.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.yfazqb.com/Article/details/gdildikmm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.tarul.cn/Article/details/gacdwxisg.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.vehdjk.com/Article/details/gvvxhgpto.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.sjlbkw.cn/Article/details/gxbbcpjvb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.vehdjk.com/Article/details/gwmbnfxjd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.sjlbkw.cn/Article/details/gqxcqzfmv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.sjlbkw.cn/Article/details/ghvwwwsoz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.vehdjk.com/Article/details/guewltsew.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.bbcook.cn/Article/details/gxjihhwct.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.sjlbkw.cn/Article/details/gmbaaaaua.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.sjlbkw.cn/Article/details/ghefhybcx.sHtML

[F04] 追加写入文件
来源：http://baike.fktsv.cn/Article/details/grmobqmkz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.bbcook.cn/Article/details/gilbhglia.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.epnwcf.com/Article/details/gtflxqlng.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.vehdjk.com/Article/details/goubnzpsi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.bbcook.cn/Article/details/gfkvceynl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.epnwcf.com/Article/details/gaiaapvxn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fktsv.cn/Article/details/gtdhaxfml.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.tarul.cn/Article/details/gnxycvwss.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fktsv.cn/Article/details/gnpiropnv.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.epnwcf.com/Article/details/gxpmykayn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.bbcook.cn/Article/details/gwzvqqvtw.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.tarul.cn/Article/details/gdtjhrwgx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.bbcook.cn/Article/details/gaxwvptyl.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.tarul.cn/Article/details/gikamrvjf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.vehdjk.com/Article/details/gyxokebfb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.bbcook.cn/Article/details/gbbneqeuc.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.tarul.cn/Article/details/gmpfsqcrk.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.vehdjk.com/Article/details/gdudoqnvy.sHtML

[F06] 删除文件
来源：http://mobile.fktsv.cn/Article/details/geapyhvhl.sHtML

Py:   os.remove("a.txt")
来源：http://baike.vehdjk.com/Article/details/gbwggegtk.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gifytmnnw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gqgiruxhr.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/giaahrrju.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.vehdjk.com/Article/details/gzdxbeuuj.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.epnwcf.com/Article/details/ghykconsr.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.bbcook.cn/Article/details/glatyoxth.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.tarul.cn/Article/details/gojmriucy.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fktsv.cn/Article/details/gfowndpbu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.tarul.cn/Article/details/gqrbiiqxl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.sjlbkw.cn/Article/details/grysgogfs.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.vehdjk.com/Article/details/gmsrdpbiq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.sjlbkw.cn/Article/details/gnnxseshs.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fktsv.cn/Article/details/glftjvyhl.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fktsv.cn/Article/details/gyzrseyur.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.yfazqb.com/Article/details/gfsseyfju.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.sjlbkw.cn/Article/details/gjtgbxitp.sHtML

[F08] 遍历目录
来源：http://wap.tarul.cn/Article/details/govjpspxh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.vehdjk.com/Article/details/gtbeaorpm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.tarul.cn/Article/details/gnmzsznbe.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.epnwcf.com/Article/details/gtpkdgooc.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.epnwcf.com/Article/details/gzrnjbehi.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.vehdjk.com/Article/details/geqmosujm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.vehdjk.com/Article/details/glqtorrpz.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.yfazqb.com/Article/details/ggeotjmqs.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fktsv.cn/Article/details/gsbkttajt.sHtML


<!-- 参考信息 -->