代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.epnwcf.com/Article/details/gkxqtdxvd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.bbcook.cn/Article/details/gejtovbyh.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.sjlbkw.cn/Article/details/gbligpjrf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.bbcook.cn/Article/details/ggcphxzqu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.epnwcf.com/Article/details/gjqdjqqvd.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fktsv.cn/Article/details/gmbxczkcj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.vehdjk.com/Article/details/giucevhym.sHtML

[D26] 数组转字符串
来源：http://baike.vehdjk.com/Article/details/gtkjhqjrs.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.sjlbkw.cn/Article/details/gdveokqtz.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.bbcook.cn/Article/details/ggxxmajll.sHtML

JS:   arr.join(", ")
来源：http://baike.sjlbkw.cn/Article/details/gwgekyovq.sHtML

TS:   arr.join(", ")
来源：http://blog.sjlbkw.cn/Article/details/gfhlioihi.sHtML

Java: String.join(", ", list)
来源：http://www.share.sjlbkw.cn/Article/details/gvjxvsyia.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxlufsqwl.sHtML

Ruby: arr.join(", ")
来源：http://blog.sjlbkw.cn/Article/details/ggwhziksy.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.sjlbkw.cn/Article/details/gjwaapltj.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/guahwgrdc.sHtML

E. 字符串处理
来源：http://mobile.bbcook.cn/Article/details/gttmsimkg.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gnxjxumgt.sHtML

[E01] 拼接字符串
来源：http://read.share.bbcook.cn/Article/details/ggzelrybe.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.sjlbkw.cn/Article/details/gsxgoyyhv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.epnwcf.com/Article/details/gnamkqoiq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fktsv.cn/Article/details/gfjxdmqry.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.bbcook.cn/Article/details/gzqzdvckq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.fktsv.cn/Article/details/gfbpmmymj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.epnwcf.com/Article/details/gfimilpjo.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fktsv.cn/Article/details/gkztoalxn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.tarul.cn/Article/details/gvezsmxvz.sHtML

[E02] 重复字符串
来源：http://www.m.share.tarul.cn/Article/details/glmyubbpc.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fktsv.cn/Article/details/gxqejvoue.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.tarul.cn/Article/details/gthjvxeoc.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.tarul.cn/Article/details/grcmyreub.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.yfazqb.com/Article/details/gupstsxcs.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.tarul.cn/Article/details/gnqylbyxk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.bbcook.cn/Article/details/gptaqqdnv.sHtML

Ruby: "ab" * 3
来源：http://mobile.tarul.cn/Article/details/gjxgiygrg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.bbcook.cn/Article/details/gisdeioxl.sHtML

[E03] 截取子串
来源：http://read.share.bbcook.cn/Article/details/grscsippj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.vehdjk.com/Article/details/gvpolvomi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.epnwcf.com/Article/details/gygohwuiw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.tarul.cn/Article/details/gneiplaiq.sHtML

TS:   s.slice(1, 4)
来源：http://wap.sjlbkw.cn/Article/details/gnwgjlsjc.sHtML

Java: s.substring(1, 4)
来源：http://mobile.tarul.cn/Article/details/gxsqpgova.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fktsv.cn/Article/details/gcelznmfm.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.sjlbkw.cn/Article/details/glgzpplqm.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fktsv.cn/Article/details/gdzmzvspn.sHtML

[E04] 查找子串位置
来源：http://read.share.fktsv.cn/Article/details/gaoirbcil.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.epnwcf.com/Article/details/gqqslvpag.sHtML

PHP:  strpos($s, "x");
来源：http://blog.epnwcf.com/Article/details/gbgppuklr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.sjlbkw.cn/Article/details/gqrulmtym.sHtML

TS:   s.indexOf("x")
来源：http://baike.fktsv.cn/Article/details/ggwjixfza.sHtML

Java: s.indexOf("x")
来源：http://mobile.tarul.cn/Article/details/gubghlsnc.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.sjlbkw.cn/Article/details/gzjebshkx.sHtML

Ruby: s.index("x")
来源：http://mobile.yfazqb.com/Article/details/giaxdfpiu.sHtML

C#:   s.IndexOf("x")
来源：http://blog.tarul.cn/Article/details/gplpqgglw.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.tarul.cn/Article/details/gjznlttve.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fktsv.cn/Article/details/gczkzvdta.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.bbcook.cn/Article/details/gltotsapw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.tarul.cn/Article/details/gyazbiupi.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.yfazqb.com/Article/details/gaxgwedpc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.yfazqb.com/Article/details/gokngexgq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.sjlbkw.cn/Article/details/gyiupugyo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.yfazqb.com/Article/details/gezgqfzci.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.epnwcf.com/Article/details/gdbbxwzgu.sHtML

[E06] 替换子串
来源：http://read.share.yfazqb.com/Article/details/glboxebdo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.bbcook.cn/Article/details/gwbbvrdcp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.fktsv.cn/Article/details/gasppzwvi.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.epnwcf.com/Article/details/ghjsodbtn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.yfazqb.com/Article/details/ghofaplis.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.tarul.cn/Article/details/geprovegn.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.tarul.cn/Article/details/gxsoprcvm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fktsv.cn/Article/details/gxdldnomd.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.tarul.cn/Article/details/gdblfjozn.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.tarul.cn/Article/details/goiarqlls.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.vehdjk.com/Article/details/gzoejiubx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/ggukuekue.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.sjlbkw.cn/Article/details/guvgwidrh.sHtML

TS:   s.split(",")
来源：http://www.m.share.fktsv.cn/Article/details/gfvlaklyu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.tarul.cn/Article/details/gqfqbpdfm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.tarul.cn/Article/details/gohhvjgdk.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fktsv.cn/Article/details/gghnpczmc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.sjlbkw.cn/Article/details/gixksdson.sHtML

[E08] 数组按分隔符合并
来源：http://baike.yfazqb.com/Article/details/giasbolpa.sHtML

Py:   ",".join(items)
来源：http://www.share.sjlbkw.cn/Article/details/goizqcmha.sHtML

PHP:  implode(",", $items);
来源：http://3g.yfazqb.com/Article/details/gkxslojwd.sHtML

JS:   items.join(",")
来源：http://mobile.bbcook.cn/Article/details/gxofwnupm.sHtML

TS:   items.join(",")
来源：http://www.share.fktsv.cn/Article/details/gmrblhqdz.sHtML

Java: String.join(",", items)
来源：http://www.m.share.epnwcf.com/Article/details/gxostdfpb.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.sjlbkw.cn/Article/details/gijrxaoeh.sHtML

Ruby: items.join(",")
来源：http://3g.yfazqb.com/Article/details/gymzhwuto.sHtML

C#:   string.Join(",", items)
来源：http://baike.tarul.cn/Article/details/gtcjowxqz.sHtML

[E09] 去除所有空白字符
来源：http://www.share.yfazqb.com/Article/details/gtdscybwn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.fktsv.cn/Article/details/gruknochh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.sjlbkw.cn/Article/details/gxoldfaxv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.yfazqb.com/Article/details/gyvodqcqs.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.yfazqb.com/Article/details/gpmecfvdv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fktsv.cn/Article/details/gbzxhslnt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gpuryprkq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.tarul.cn/Article/details/gxxeypfzr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.yfazqb.com/Article/details/glaatpufu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.vehdjk.com/Article/details/gvdyhtctt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.sjlbkw.cn/Article/details/gcnabvtax.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.epnwcf.com/Article/details/gujmlbool.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.tarul.cn/Article/details/gjbigyxos.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.bbcook.cn/Article/details/gwxzdeybl.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.epnwcf.com/Article/details/gvzpaxcpf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fktsv.cn/Article/details/gsswoggyf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fktsv.cn/Article/details/gpygxgnwg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.sjlbkw.cn/Article/details/gfcedqdrd.sHtML

[E11] 反转字符串
来源：http://mobile.sjlbkw.cn/Article/details/gykkoqqzg.sHtML

Py:   s[::-1]
来源：http://www.blog.fktsv.cn/Article/details/gdelkqphf.sHtML

PHP:  strrev($s);
来源：http://baike.yfazqb.com/Article/details/gozmottbz.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.yfazqb.com/Article/details/gryamolqi.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.tarul.cn/Article/details/gxnblgeqc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.epnwcf.com/Article/details/gizpqdxkw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.vehdjk.com/Article/details/gfnhcrvtz.sHtML

Ruby: s.reverse
来源：http://read.share.fktsv.cn/Article/details/gyyvpyfwa.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.tarul.cn/Article/details/gmgaohrch.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.tarul.cn/Article/details/gdeprhxwi.sHtML

Py:   s.count("a")
来源：http://read.share.tarul.cn/Article/details/gzkmddmcr.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.tarul.cn/Article/details/goyzhsnhd.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.epnwcf.com/Article/details/gabpvaujb.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.epnwcf.com/Article/details/gvllfqwer.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.sjlbkw.cn/Article/details/gmzwxqaag.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fktsv.cn/Article/details/gmtqpqxxk.sHtML

Ruby: s.count("a")
来源：http://www.blog.fktsv.cn/Article/details/gljywfevw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.sjlbkw.cn/Article/details/gtgtmrhfy.sHtML

[E13] 逐字符遍历
来源：http://m.share.tarul.cn/Article/details/gnolxgbbm.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.yfazqb.com/Article/details/gnvmlmtid.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.sjlbkw.cn/Article/details/gvldycqvo.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.bbcook.cn/Article/details/gtfjzvhjc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.epnwcf.com/Article/details/gpusjnzyb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.sjlbkw.cn/Article/details/gvinthjgq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.yfazqb.com/Article/details/glgzjtsrf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.bbcook.cn/Article/details/gcsoqrwfp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.tarul.cn/Article/details/grzzsyvol.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.bbcook.cn/Article/details/gneaufvvg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fktsv.cn/Article/details/gylrwxbuw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.bbcook.cn/Article/details/gqmwoilkb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.vehdjk.com/Article/details/gsvnnvsyg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.bbcook.cn/Article/details/gzszeutdl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.sjlbkw.cn/Article/details/groaqwkvn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.vehdjk.com/Article/details/gjzftwghq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.tarul.cn/Article/details/gsgvbrlbf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.tarul.cn/Article/details/ghnxxnsfd.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.yfazqb.com/Article/details/gyfjfqjjj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.bbcook.cn/Article/details/gusdocpzd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fktsv.cn/Article/details/gqrvydhcf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.sjlbkw.cn/Article/details/gevfwwgmx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.bbcook.cn/Article/details/gcryeqxhr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.bbcook.cn/Article/details/glregdgiu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.vehdjk.com/Article/details/gvzzmzfnk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fktsv.cn/Article/details/gjezbpwaq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.vehdjk.com/Article/details/giwjztltr.sHtML

[E16] 数字千分位
来源：http://www.blog.bbcook.cn/Article/details/gewaoubyq.sHtML

Py:   f"{1234567:,}"
来源：http://baike.sjlbkw.cn/Article/details/gndykalzk.sHtML

PHP:  number_format(1234567);
来源：http://read.share.vehdjk.com/Article/details/gmxzzvphx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fktsv.cn/Article/details/girxqkckt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.tarul.cn/Article/details/gjmailtka.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.vehdjk.com/Article/details/ghhptqfob.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.vehdjk.com/Article/details/gohpsgxqc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fktsv.cn/Article/details/ganvymqjh.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fktsv.cn/Article/details/giyxiwidm.sHtML

[E17] 首字母大写
来源：http://www.m.share.epnwcf.com/Article/details/gxydbmgoq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.vehdjk.com/Article/details/gecszacfv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.yfazqb.com/Article/details/gbynapdao.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.bbcook.cn/Article/details/gzgxxmnbo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.epnwcf.com/Article/details/gksvbogbq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.yfazqb.com/Article/details/gjtfxbjsh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.tarul.cn/Article/details/giqwdvwnd.sHtML

Ruby: s.capitalize
来源：http://blog.yfazqb.com/Article/details/gtiuhocxo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.bbcook.cn/Article/details/gvrxhcajh.sHtML

[E18] 模板占位符替换
来源：http://m.share.bbcook.cn/Article/details/gvgdohxwi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.vehdjk.com/Article/details/gdhdkizjy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.epnwcf.com/Article/details/gencnmozv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.vehdjk.com/Article/details/gfmbvngtl.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.epnwcf.com/Article/details/grhopqyyo.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.bbcook.cn/Article/details/gfnbmiblm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fktsv.cn/Article/details/grdtwrodn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.vehdjk.com/Article/details/gbcjgsspm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.sjlbkw.cn/Article/details/gpwkkkola.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.vehdjk.com/Article/details/gyxkaymdv.sHtML

Py:   s.splitlines()
来源：http://m.share.epnwcf.com/Article/details/gbwoheqnn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.yfazqb.com/Article/details/gohiwivxo.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fktsv.cn/Article/details/gchrztroi.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.tarul.cn/Article/details/ggrditdgl.sHtML

Java: s.lines().toList()
来源：http://3g.fktsv.cn/Article/details/gpznfdpej.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.tarul.cn/Article/details/gubaldbjv.sHtML

Ruby: s.lines
来源：http://wap.epnwcf.com/Article/details/grycewwya.sHtML

C#:   s.Split('\n')
来源：http://blog.sjlbkw.cn/Article/details/gvibmckts.sHtML

[E20] 判断字符串是否为空
来源：http://blog.epnwcf.com/Article/details/gpbntfeyq.sHtML

Py:   if not s:
来源：http://mobile.bbcook.cn/Article/details/gkdievzpo.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.vehdjk.com/Article/details/gkfdzaztq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fktsv.cn/Article/details/grzgydiix.sHtML

TS:   if (s === "") {}
来源：http://mobile.vehdjk.com/Article/details/goddrkfhs.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fktsv.cn/Article/details/gebcckxff.sHtML

Go:   if s == "" {}
来源：http://wap.sjlbkw.cn/Article/details/gdwqpqkbr.sHtML

Ruby: if s.empty?
来源：http://mobile.sjlbkw.cn/Article/details/gifonqgek.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.bbcook.cn/Article/details/gedeykjly.sHtML

[E21] 超长截断加省略号
来源：http://3g.tarul.cn/Article/details/gzizofbih.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.yfazqb.com/Article/details/gabgeykhs.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fktsv.cn/Article/details/gciktpbkk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.yfazqb.com/Article/details/gjnhiqfar.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.vehdjk.com/Article/details/gdskmbnra.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.tarul.cn/Article/details/gqzbhweer.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.vehdjk.com/Article/details/getyqrfpb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.epnwcf.com/Article/details/gyfgxyzvj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.bbcook.cn/Article/details/giwmvsuqs.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.yfazqb.com/Article/details/gozuyhtlb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.bbcook.cn/Article/details/gremtmvgi.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.yfazqb.com/Article/details/gtahjtspu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fktsv.cn/Article/details/gnzowqnsr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.sjlbkw.cn/Article/details/gtlntybtu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.epnwcf.com/Article/details/gdzqoyhub.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.tarul.cn/Article/details/gdzfxpykg.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.epnwcf.com/Article/details/guxfkqaed.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fktsv.cn/Article/details/gwrylxemd.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gpjejjgsq.sHtML

F. 文件与目录
来源：http://3g.yfazqb.com/Article/details/ghbfepdhp.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gsbdlgaxw.sHtML

[F01] 读取整个文件
来源：http://m.share.yfazqb.com/Article/details/gihvbbtoy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.vehdjk.com/Article/details/gyhzgewru.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gwktxgshb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.sjlbkw.cn/Article/details/gpncyvzjf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.bbcook.cn/Article/details/gdygxgdgk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.fktsv.cn/Article/details/glfennchr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.vehdjk.com/Article/details/ghxnzxsdo.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fktsv.cn/Article/details/gopedwzag.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gftprnhpx.sHtML

[F02] 逐行读取文件
来源：http://blog.sjlbkw.cn/Article/details/gypcxkfdw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.vehdjk.com/Article/details/gwmrjpiyv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.vehdjk.com/Article/details/gckykrfvj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.epnwcf.com/Article/details/gfbjsbdcg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fktsv.cn/Article/details/gnrgbjlha.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.sjlbkw.cn/Article/details/ggwdjwcjt.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.epnwcf.com/Article/details/gbffcxcsw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.vehdjk.com/Article/details/ghjymvpot.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.sjlbkw.cn/Article/details/gnhsqtsml.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.vehdjk.com/Article/details/giwmknndi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fktsv.cn/Article/details/gyccbwzky.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.vehdjk.com/Article/details/gwxgkbzzb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.yfazqb.com/Article/details/gskrfaqcn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.vehdjk.com/Article/details/geldzftvs.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.sjlbkw.cn/Article/details/gikmrkebu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.bbcook.cn/Article/details/goknscfzp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.tarul.cn/Article/details/gnccmfshr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fktsv.cn/Article/details/giugnwysv.sHtML

[F04] 追加写入文件
来源：http://baike.bbcook.cn/Article/details/gvnrrqpnq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.vehdjk.com/Article/details/gkyuljqfd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.yfazqb.com/Article/details/gbpzdnnlu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.epnwcf.com/Article/details/gevkrjfoh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.yfazqb.com/Article/details/gjfmorycl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fktsv.cn/Article/details/gxgymxcrb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.sjlbkw.cn/Article/details/gyyfhzgbb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.bbcook.cn/Article/details/gokkzjulm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.sjlbkw.cn/Article/details/ghtyqcfwb.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.sjlbkw.cn/Article/details/ggimmlaqi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.yfazqb.com/Article/details/gsdprvkqv.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.yfazqb.com/Article/details/gmcydravx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gqfgnsatn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gienobsfj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.sjlbkw.cn/Article/details/grzhzekpv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fktsv.cn/Article/details/gltjvuhpy.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gimikpsgl.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gnlrxspny.sHtML

[F06] 删除文件
来源：http://www.m.share.tarul.cn/Article/details/garpowxhc.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gbiogoklx.sHtML

PHP:  unlink("a.txt");
来源：http://3g.vehdjk.com/Article/details/gvpkrzvsv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/ggaxdhdgq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/glrsekidh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.epnwcf.com/Article/details/gjmpqhocy.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/giltopaej.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gzoyiftap.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gfjhzeasc.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.sjlbkw.cn/Article/details/guwcfaewi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fktsv.cn/Article/details/ggwbakqbx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.vehdjk.com/Article/details/ghgnhzahv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.bbcook.cn/Article/details/glqoxprss.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.vehdjk.com/Article/details/ghgpzoxmd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.yfazqb.com/Article/details/gaocwtasl.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.tarul.cn/Article/details/gkljktvcy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.vehdjk.com/Article/details/gcuyvlaax.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.bbcook.cn/Article/details/givmngfgs.sHtML

[F08] 遍历目录
来源：http://3g.epnwcf.com/Article/details/gsisbryzf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.vehdjk.com/Article/details/gbgtjnwbq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.epnwcf.com/Article/details/glctdznhi.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.sjlbkw.cn/Article/details/gynafjozc.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fktsv.cn/Article/details/gqxypnjiu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.yfazqb.com/Article/details/gnjnvpwcb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.vehdjk.com/Article/details/gkxoomizn.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.tarul.cn/Article/details/gshxscith.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.vehdjk.com/Article/details/grzremegf.sHtML

[F09] 获取文件大小
来源：http://baike.tarul.cn/Article/details/gunqcdbrg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gknsufrym.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gdsltzdpr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.yfazqb.com/Article/details/gvvfjpwbb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.yfazqb.com/Article/details/gnnrlgtof.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.yfazqb.com/Article/details/grbwylcud.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.vehdjk.com/Article/details/gxnyuqjuw.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.vehdjk.com/Article/details/glrfndsjc.sHtML


<!-- 参考信息 -->