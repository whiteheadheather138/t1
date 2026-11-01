代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.bbcook.cn/Article/details/ggafeyngj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.epnwcf.com/Article/details/ghldqgadx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.yfazqb.com/Article/details/gmmgrsbxf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.yfazqb.com/Article/details/giyntczex.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.vehdjk.com/Article/details/grvfcsxwz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.yfazqb.com/Article/details/gsokbuire.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.yfazqb.com/Article/details/goupmlztg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.yfazqb.com/Article/details/gvumkhkue.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.fktsv.cn/Article/details/gbmdljnlt.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.yfazqb.com/Article/details/ggflyznur.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.sjlbkw.cn/Article/details/gdzzsszsi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.epnwcf.com/Article/details/gnumzmpcw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fktsv.cn/Article/details/gtontgvdd.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.tarul.cn/Article/details/gqwdgatcn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fktsv.cn/Article/details/ghhhossfj.sHtML

[D26] 数组转字符串
来源：http://www.m.share.yfazqb.com/Article/details/gwrdyvyqw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.yfazqb.com/Article/details/gaxmotiqz.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.tarul.cn/Article/details/gsraouzvl.sHtML

JS:   arr.join(", ")
来源：http://www.blog.yfazqb.com/Article/details/gllkfbsls.sHtML

TS:   arr.join(", ")
来源：http://www.blog.tarul.cn/Article/details/gwoqpnzks.sHtML

Java: String.join(", ", list)
来源：http://www.share.vehdjk.com/Article/details/gjzjmxbxa.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.sjlbkw.cn/Article/details/gswkgfvrp.sHtML

Ruby: arr.join(", ")
来源：http://read.share.vehdjk.com/Article/details/gzoiyomkq.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.yfazqb.com/Article/details/golugskjb.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gzogrfbgz.sHtML

E. 字符串处理
来源：http://www.share.sjlbkw.cn/Article/details/gsukovubs.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gnksyfmms.sHtML

[E01] 拼接字符串
来源：http://www.blog.epnwcf.com/Article/details/grpgzhveg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.vehdjk.com/Article/details/gdqufqkts.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.sjlbkw.cn/Article/details/gaydiomsj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.tarul.cn/Article/details/gatqsbtyz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.yfazqb.com/Article/details/gjynvuijc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.vehdjk.com/Article/details/gqxwhwzaz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fktsv.cn/Article/details/ggmchokpt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.vehdjk.com/Article/details/guuvivfal.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.tarul.cn/Article/details/gpdxcpivi.sHtML

[E02] 重复字符串
来源：http://3g.epnwcf.com/Article/details/gyhqyrwib.sHtML

Py:   "ab" * 3
来源：http://3g.sjlbkw.cn/Article/details/gmbesbdcz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.vehdjk.com/Article/details/gsplcvejn.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.sjlbkw.cn/Article/details/gfrzbvfcx.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.yfazqb.com/Article/details/gwxtnasez.sHtML

Java: "ab".repeat(3)
来源：http://m.share.vehdjk.com/Article/details/gfhsomqsz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.epnwcf.com/Article/details/gvyzaxsoo.sHtML

Ruby: "ab" * 3
来源：http://m.share.sjlbkw.cn/Article/details/gibkbbblq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fktsv.cn/Article/details/gjxeimgrc.sHtML

[E03] 截取子串
来源：http://www.share.fktsv.cn/Article/details/gqqtfjqkd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.sjlbkw.cn/Article/details/ggjvtrrwl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.sjlbkw.cn/Article/details/gletmaenm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.sjlbkw.cn/Article/details/gpozsvzlx.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.tarul.cn/Article/details/gydvotvpa.sHtML

Java: s.substring(1, 4)
来源：http://mobile.bbcook.cn/Article/details/gcklmqtfw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.vehdjk.com/Article/details/gwovnvasp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fktsv.cn/Article/details/gddhbncqz.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.bbcook.cn/Article/details/gdmpdlwzi.sHtML

[E04] 查找子串位置
来源：http://3g.fktsv.cn/Article/details/grfqzcrku.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.tarul.cn/Article/details/gyrbhbbjd.sHtML

PHP:  strpos($s, "x");
来源：http://baike.bbcook.cn/Article/details/ggyzgxowe.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.epnwcf.com/Article/details/gaxifyjji.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fktsv.cn/Article/details/gtfxhxfbe.sHtML

Java: s.indexOf("x")
来源：http://mobile.yfazqb.com/Article/details/gnnfbahxt.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fktsv.cn/Article/details/gwzqkntse.sHtML

Ruby: s.index("x")
来源：http://m.share.bbcook.cn/Article/details/gnlgxdkbm.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.sjlbkw.cn/Article/details/gqbefhito.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.sjlbkw.cn/Article/details/gxljafaxj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.yfazqb.com/Article/details/gfrpnbwyh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.tarul.cn/Article/details/gakbgislp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.vehdjk.com/Article/details/ggzmzzysl.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.sjlbkw.cn/Article/details/grylghfnh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.bbcook.cn/Article/details/giiigjujw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.epnwcf.com/Article/details/gibjpnnrh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.bbcook.cn/Article/details/gnnivtupu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fktsv.cn/Article/details/gkbhreqmm.sHtML

[E06] 替换子串
来源：http://www.share.fktsv.cn/Article/details/goyhqxezy.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.bbcook.cn/Article/details/gobpncwvu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.tarul.cn/Article/details/gcvghhzrm.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.epnwcf.com/Article/details/guyvgmfhf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.tarul.cn/Article/details/gyltllpkw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/grkyjzalr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.vehdjk.com/Article/details/gimgcbefk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/gwnrwjawl.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gkzcvxuii.sHtML

[E07] 按分隔符拆分
来源：http://3g.epnwcf.com/Article/details/gewdlxmdg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.vehdjk.com/Article/details/geqitanps.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.bbcook.cn/Article/details/geweixhmh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.yfazqb.com/Article/details/glvlzdgld.sHtML

TS:   s.split(",")
来源：http://www.share.epnwcf.com/Article/details/glsdujxjp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.sjlbkw.cn/Article/details/gpnxbvdim.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.epnwcf.com/Article/details/gwmzvoovq.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.sjlbkw.cn/Article/details/gkxftkmgc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fktsv.cn/Article/details/gxeiegkwx.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.tarul.cn/Article/details/ggdhepobt.sHtML

Py:   ",".join(items)
来源：http://www.share.yfazqb.com/Article/details/goygjjxji.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.epnwcf.com/Article/details/giymjmori.sHtML

JS:   items.join(",")
来源：http://www.share.sjlbkw.cn/Article/details/gcmooexqd.sHtML

TS:   items.join(",")
来源：http://www.m.share.vehdjk.com/Article/details/gbcdlvegt.sHtML

Java: String.join(",", items)
来源：http://read.share.sjlbkw.cn/Article/details/gnnejszro.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.epnwcf.com/Article/details/gqecarcqx.sHtML

Ruby: items.join(",")
来源：http://read.share.yfazqb.com/Article/details/gyagpzaiv.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fktsv.cn/Article/details/gnplrfndv.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fktsv.cn/Article/details/gonyewbub.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.sjlbkw.cn/Article/details/guylfkgsc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.bbcook.cn/Article/details/gietvbhlt.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fktsv.cn/Article/details/gkyxacnbb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.vehdjk.com/Article/details/gxwsvpnzf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.tarul.cn/Article/details/gplgeaixn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.epnwcf.com/Article/details/gyiffagxo.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.yfazqb.com/Article/details/goenqlpch.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.vehdjk.com/Article/details/glkfibuln.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.epnwcf.com/Article/details/gsgjvorrg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.sjlbkw.cn/Article/details/gwggelhuw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.yfazqb.com/Article/details/gwtlmftwz.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.epnwcf.com/Article/details/gbdwnrvoq.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.vehdjk.com/Article/details/geyjvqqff.sHtML

Java: String.format("%03d", 7)
来源：http://3g.tarul.cn/Article/details/guiwmnbbn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.bbcook.cn/Article/details/ghsdazinn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.tarul.cn/Article/details/gjpwgftsj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.sjlbkw.cn/Article/details/gfvovkjwe.sHtML

[E11] 反转字符串
来源：http://m.share.epnwcf.com/Article/details/gkavmsfvm.sHtML

Py:   s[::-1]
来源：http://www.share.tarul.cn/Article/details/glxcszedb.sHtML

PHP:  strrev($s);
来源：http://baike.tarul.cn/Article/details/grbuvnied.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.bbcook.cn/Article/details/ggbrwmaem.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/gtflvedkn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.vehdjk.com/Article/details/ghzuqbmnn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.bbcook.cn/Article/details/gagrqotmy.sHtML

Ruby: s.reverse
来源：http://www.m.share.epnwcf.com/Article/details/gahockesv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.bbcook.cn/Article/details/gagneaqlm.sHtML

[E12] 统计某字符出现次数
来源：http://blog.fktsv.cn/Article/details/gweouhmmm.sHtML

Py:   s.count("a")
来源：http://3g.fktsv.cn/Article/details/gebldbokm.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.bbcook.cn/Article/details/gnlshzlvo.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.tarul.cn/Article/details/gyehfziwh.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.sjlbkw.cn/Article/details/gewpgmgaa.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.tarul.cn/Article/details/gigewpxpi.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.sjlbkw.cn/Article/details/goqcqmwot.sHtML

Ruby: s.count("a")
来源：http://blog.fktsv.cn/Article/details/gynqmedrw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fktsv.cn/Article/details/gcdcyblur.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fktsv.cn/Article/details/gtjkmjjbw.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.yfazqb.com/Article/details/gscjhsixj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.tarul.cn/Article/details/gvwaabfgt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.epnwcf.com/Article/details/gyykpjpit.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fktsv.cn/Article/details/gpjoqpnak.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fktsv.cn/Article/details/gnfyivdel.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.bbcook.cn/Article/details/gxhzescmx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.bbcook.cn/Article/details/gaaplzfsd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.bbcook.cn/Article/details/gevqarhdl.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.epnwcf.com/Article/details/gcekbzpzx.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fktsv.cn/Article/details/gmmfznpev.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.vehdjk.com/Article/details/gkkaivmqz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.bbcook.cn/Article/details/gljvbufrw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fktsv.cn/Article/details/gjyzjvvaa.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.tarul.cn/Article/details/grfadwexn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.vehdjk.com/Article/details/gbakexegp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.epnwcf.com/Article/details/glwksavfq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fktsv.cn/Article/details/gwtotumnj.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.epnwcf.com/Article/details/gelopxgol.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.fktsv.cn/Article/details/gbpswnwnw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.vehdjk.com/Article/details/gdwwefgay.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtiryigxj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.bbcook.cn/Article/details/gcgzcomrt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.tarul.cn/Article/details/gcpyhxywj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.yfazqb.com/Article/details/gumiskwev.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.vehdjk.com/Article/details/gweliqdqb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.bbcook.cn/Article/details/gcitmqzvf.sHtML

[E16] 数字千分位
来源：http://blog.vehdjk.com/Article/details/grotipiwz.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fktsv.cn/Article/details/gegsozqec.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.epnwcf.com/Article/details/gignndzed.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.tarul.cn/Article/details/geoirahyf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.yfazqb.com/Article/details/gsdohgcms.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.vehdjk.com/Article/details/gqqofdvcm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.yfazqb.com/Article/details/ghkfvhnxo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.tarul.cn/Article/details/glvyhkgjw.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.sjlbkw.cn/Article/details/gumuudbam.sHtML

[E17] 首字母大写
来源：http://wap.epnwcf.com/Article/details/gffnwobul.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.sjlbkw.cn/Article/details/gekyxraop.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.yfazqb.com/Article/details/gklhmfwna.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.epnwcf.com/Article/details/gokghyjwd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.yfazqb.com/Article/details/gxmbafojo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gbqowbhcl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fktsv.cn/Article/details/grquplcjv.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fktsv.cn/Article/details/gthgbujde.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.epnwcf.com/Article/details/gnvphhmhc.sHtML

[E18] 模板占位符替换
来源：http://read.share.fktsv.cn/Article/details/gyopqgbsw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.epnwcf.com/Article/details/gvpzsdxcc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.sjlbkw.cn/Article/details/gzoxcifnz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.sjlbkw.cn/Article/details/gzripbluu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.sjlbkw.cn/Article/details/gqcmfdpqc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.epnwcf.com/Article/details/gnmydbvxv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.vehdjk.com/Article/details/gecmlksto.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.sjlbkw.cn/Article/details/gpzmhejqv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fktsv.cn/Article/details/goaphpelw.sHtML

[E19] 多行文本按行拆分
来源：http://wap.yfazqb.com/Article/details/gyufqdfsf.sHtML

Py:   s.splitlines()
来源：http://3g.tarul.cn/Article/details/gljjbdlbn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.yfazqb.com/Article/details/gfjuiwnjt.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.yfazqb.com/Article/details/gybcxzxns.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.epnwcf.com/Article/details/gpkaivlus.sHtML

Java: s.lines().toList()
来源：http://m.share.vehdjk.com/Article/details/gnohgowic.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.yfazqb.com/Article/details/gjefzgdkm.sHtML

Ruby: s.lines
来源：http://blog.fktsv.cn/Article/details/gtckfbqps.sHtML

C#:   s.Split('\n')
来源：http://wap.sjlbkw.cn/Article/details/gdtnbakpi.sHtML

[E20] 判断字符串是否为空
来源：http://blog.epnwcf.com/Article/details/glufifrqj.sHtML

Py:   if not s:
来源：http://www.share.sjlbkw.cn/Article/details/gnybgbrdu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.bbcook.cn/Article/details/gcptsfdsz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.yfazqb.com/Article/details/gzmnybnjg.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fktsv.cn/Article/details/glixdcdll.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.tarul.cn/Article/details/gwesuweqn.sHtML

Go:   if s == "" {}
来源：http://www.blog.epnwcf.com/Article/details/gedeitnvi.sHtML

Ruby: if s.empty?
来源：http://www.share.bbcook.cn/Article/details/gwfctahar.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.yfazqb.com/Article/details/gkiuvfdcq.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fktsv.cn/Article/details/gocprwbel.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.epnwcf.com/Article/details/gyxjgwgwz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.vehdjk.com/Article/details/gilbspolw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.epnwcf.com/Article/details/ghuklmpwf.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fktsv.cn/Article/details/grlxcaoan.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gehghiwdl.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fktsv.cn/Article/details/grwbouetb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.sjlbkw.cn/Article/details/gknsvqalr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fktsv.cn/Article/details/gjscjkjsp.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.tarul.cn/Article/details/gwpxdiwtm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.bbcook.cn/Article/details/gdjxecaux.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.yfazqb.com/Article/details/gzazdengs.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.bbcook.cn/Article/details/guaprnhvo.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fktsv.cn/Article/details/gvpcplooi.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.bbcook.cn/Article/details/gtggfiatd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.sjlbkw.cn/Article/details/gqdtmbxmy.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.vehdjk.com/Article/details/gghcnryfi.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.tarul.cn/Article/details/glokpgxbn.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gelvbjvix.sHtML

F. 文件与目录
来源：http://www.share.sjlbkw.cn/Article/details/gupcrsgju.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/grsqtuufj.sHtML

[F01] 读取整个文件
来源：http://www.share.fktsv.cn/Article/details/gjkginulj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.vehdjk.com/Article/details/gbeiocebt.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.vehdjk.com/Article/details/gpeovyome.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.vehdjk.com/Article/details/ganuzkvtz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fktsv.cn/Article/details/gcpetaquw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.tarul.cn/Article/details/gdgjkgzbo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.bbcook.cn/Article/details/grxwtpozx.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/grrthpwft.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.vehdjk.com/Article/details/gduevhbba.sHtML

[F02] 逐行读取文件
来源：http://3g.epnwcf.com/Article/details/gnewemohd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.vehdjk.com/Article/details/gdilxtfti.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.epnwcf.com/Article/details/girspziws.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fktsv.cn/Article/details/gvevwgghk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.tarul.cn/Article/details/gchkiffyi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.yfazqb.com/Article/details/goaqyfnor.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.vehdjk.com/Article/details/gbypbpggy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.tarul.cn/Article/details/ghuvaenpo.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnthkjtlo.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.yfazqb.com/Article/details/giatujnwv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.epnwcf.com/Article/details/gozqliviv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.bbcook.cn/Article/details/glchkuwna.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.yfazqb.com/Article/details/glmocaysc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.sjlbkw.cn/Article/details/grpphsrsv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.epnwcf.com/Article/details/gkerfnvkv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.tarul.cn/Article/details/gobmdgibr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.tarul.cn/Article/details/gawwbudlv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.bbcook.cn/Article/details/gmtjnxxpp.sHtML

[F04] 追加写入文件
来源：http://read.share.bbcook.cn/Article/details/gnxnflypr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fktsv.cn/Article/details/gthzosmmt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.tarul.cn/Article/details/gijudwfrf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.vehdjk.com/Article/details/gbyekxsxz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.vehdjk.com/Article/details/grinuimho.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.vehdjk.com/Article/details/gjrshrggr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.epnwcf.com/Article/details/gxmawtcfk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.bbcook.cn/Article/details/giqhlyqbl.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.sjlbkw.cn/Article/details/gwyqtssnt.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.tarul.cn/Article/details/guucucwgg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.epnwcf.com/Article/details/gaebpdnmn.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.tarul.cn/Article/details/gdsauazop.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gmoccjeei.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.bbcook.cn/Article/details/glghktaza.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fktsv.cn/Article/details/gbhhujvlh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.epnwcf.com/Article/details/gogfkbuso.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gupiaatgj.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fktsv.cn/Article/details/ggkrpikwl.sHtML

[F06] 删除文件
来源：http://baike.yfazqb.com/Article/details/gupwdkkec.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fktsv.cn/Article/details/ggosjfyfx.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.tarul.cn/Article/details/gpscapiks.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gxgvlwyvd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.tarul.cn/Article/details/gpthhifte.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.sjlbkw.cn/Article/details/gadqrrwqc.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.yfazqb.com/Article/details/ghpjqjwyn.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gsklkiymw.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.tarul.cn/Article/details/gaprvbqva.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.sjlbkw.cn/Article/details/gfyixqhpx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.yfazqb.com/Article/details/gjkogyhnz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fktsv.cn/Article/details/gvrqmahdo.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.tarul.cn/Article/details/gohrsmdpc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.sjlbkw.cn/Article/details/genoreqvm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.tarul.cn/Article/details/ghmmczkly.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.tarul.cn/Article/details/geryhvmfy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.epnwcf.com/Article/details/gzasmskgg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.vehdjk.com/Article/details/gzlyprkej.sHtML

[F08] 遍历目录
来源：http://www.m.share.sjlbkw.cn/Article/details/gychtrrck.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.yfazqb.com/Article/details/ghdmpdjma.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.tarul.cn/Article/details/gxlkvwjag.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.tarul.cn/Article/details/guuzlienl.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.sjlbkw.cn/Article/details/gfuxxwpin.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fktsv.cn/Article/details/gyxbskype.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.epnwcf.com/Article/details/gelobhqpc.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.yfazqb.com/Article/details/gxwhcazek.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.sjlbkw.cn/Article/details/gdawjbnbf.sHtML


<!-- 参考信息 -->