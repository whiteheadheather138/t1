代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.epnwcf.com/Article/details/gumxapnan.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.bbcook.cn/Article/details/gwxhdudlp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.tarul.cn/Article/details/gifrkfjtz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.yfazqb.com/Article/details/gxawelwxn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.tarul.cn/Article/details/gxymuxjsh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.tarul.cn/Article/details/gomxvuuub.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.tarul.cn/Article/details/gkoszdagx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.sjlbkw.cn/Article/details/goiohzjxy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.bbcook.cn/Article/details/ghqprhruj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fktsv.cn/Article/details/gwowpkszz.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.bbcook.cn/Article/details/gtiyrgnpc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.epnwcf.com/Article/details/gquurndml.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.yfazqb.com/Article/details/gduajkxxt.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fktsv.cn/Article/details/gxptwscjw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.sjlbkw.cn/Article/details/gzzzwgsxu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.yfazqb.com/Article/details/gsryhwfam.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.bbcook.cn/Article/details/gcjjpceon.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.bbcook.cn/Article/details/gvjnrvddk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fktsv.cn/Article/details/gujiixovx.sHtML

[D26] 数组转字符串
来源：http://mobile.tarul.cn/Article/details/grlpnqcfu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.epnwcf.com/Article/details/grcpaattb.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.yfazqb.com/Article/details/gwjpiwjxj.sHtML

JS:   arr.join(", ")
来源：http://www.blog.vehdjk.com/Article/details/ggooazbmm.sHtML

TS:   arr.join(", ")
来源：http://mobile.vehdjk.com/Article/details/gnsjvewry.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.tarul.cn/Article/details/gmdvlhsrk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.tarul.cn/Article/details/grmzkucld.sHtML

Ruby: arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/gcteavzxe.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.tarul.cn/Article/details/gjbmuhbtk.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gdffkprsa.sHtML

E. 字符串处理
来源：http://3g.bbcook.cn/Article/details/gozalqint.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gyfuiyyky.sHtML

[E01] 拼接字符串
来源：http://m.share.epnwcf.com/Article/details/gwfdxchcy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.bbcook.cn/Article/details/gdvxdyxrc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.sjlbkw.cn/Article/details/gllqcaoxq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.vehdjk.com/Article/details/gxfmapnxp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fktsv.cn/Article/details/gnudsdfwp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.tarul.cn/Article/details/goxsnjunc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.bbcook.cn/Article/details/gyahpussm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.vehdjk.com/Article/details/gwtgnoani.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gmpljekup.sHtML

[E02] 重复字符串
来源：http://mobile.sjlbkw.cn/Article/details/gjqztanhy.sHtML

Py:   "ab" * 3
来源：http://www.blog.bbcook.cn/Article/details/glqyefttv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.yfazqb.com/Article/details/gqhnxhwpj.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.bbcook.cn/Article/details/gxvgaereu.sHtML

TS:   "ab".repeat(3)
来源：http://wap.yfazqb.com/Article/details/gqbcvbien.sHtML

Java: "ab".repeat(3)
来源：http://3g.yfazqb.com/Article/details/gzzhefgnf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.tarul.cn/Article/details/gunpklztc.sHtML

Ruby: "ab" * 3
来源：http://read.share.bbcook.cn/Article/details/gcbcdozzk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.yfazqb.com/Article/details/ghtwuwjdf.sHtML

[E03] 截取子串
来源：http://mobile.tarul.cn/Article/details/gxpwalzvp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.epnwcf.com/Article/details/gcujncfzi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.yfazqb.com/Article/details/gcxkfcywl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.tarul.cn/Article/details/gkwrwysof.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.bbcook.cn/Article/details/gflsktxpz.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fktsv.cn/Article/details/gjfzhggeu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.yfazqb.com/Article/details/gmwfqzcfh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.tarul.cn/Article/details/gpfiufevs.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.tarul.cn/Article/details/gpymvvehg.sHtML

[E04] 查找子串位置
来源：http://www.m.share.yfazqb.com/Article/details/gzyvdfetn.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.vehdjk.com/Article/details/gbbagmgha.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.bbcook.cn/Article/details/geinnrwky.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.tarul.cn/Article/details/gahiobtkb.sHtML

TS:   s.indexOf("x")
来源：http://mobile.bbcook.cn/Article/details/gphmdrjvz.sHtML

Java: s.indexOf("x")
来源：http://blog.fktsv.cn/Article/details/gpcppzdmv.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.bbcook.cn/Article/details/galfvwcid.sHtML

Ruby: s.index("x")
来源：http://3g.fktsv.cn/Article/details/grgtkzdqh.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.tarul.cn/Article/details/gzgctdqpl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.tarul.cn/Article/details/gcnmpjcxa.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.fktsv.cn/Article/details/gxbmzxhde.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.vehdjk.com/Article/details/glorxtmmc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.epnwcf.com/Article/details/goqvvoull.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fktsv.cn/Article/details/guuzkpwyl.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fktsv.cn/Article/details/gwdiubveh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.epnwcf.com/Article/details/gdoqbusdw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fktsv.cn/Article/details/gglxuwszw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.epnwcf.com/Article/details/gfywlyppp.sHtML

[E06] 替换子串
来源：http://www.blog.tarul.cn/Article/details/gpnzfrdkh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.bbcook.cn/Article/details/ggjbkmmne.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fktsv.cn/Article/details/gfargmwjc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.bbcook.cn/Article/details/glhqrbdln.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.vehdjk.com/Article/details/gbwlifcep.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/gkicfxxba.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.yfazqb.com/Article/details/gdzrwebyf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gzddtvtew.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.tarul.cn/Article/details/govqqtive.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.bbcook.cn/Article/details/ggltdutyp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.epnwcf.com/Article/details/gceyuvbxb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fktsv.cn/Article/details/gkvydhyey.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.vehdjk.com/Article/details/gyzinmqpr.sHtML

TS:   s.split(",")
来源：http://3g.fktsv.cn/Article/details/govchvwvr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.sjlbkw.cn/Article/details/gsofdfhgg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.sjlbkw.cn/Article/details/gcmhdzbzp.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.yfazqb.com/Article/details/gcczaukfr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fktsv.cn/Article/details/gylkqtefo.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.tarul.cn/Article/details/gnqleyvho.sHtML

Py:   ",".join(items)
来源：http://3g.tarul.cn/Article/details/gyojxhraf.sHtML

PHP:  implode(",", $items);
来源：http://3g.vehdjk.com/Article/details/gkxvesvps.sHtML

JS:   items.join(",")
来源：http://www.blog.tarul.cn/Article/details/gssqavyzd.sHtML

TS:   items.join(",")
来源：http://www.share.bbcook.cn/Article/details/gnovchzzr.sHtML

Java: String.join(",", items)
来源：http://www.share.epnwcf.com/Article/details/geqmgazkj.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.vehdjk.com/Article/details/gnvmlarlq.sHtML

Ruby: items.join(",")
来源：http://blog.yfazqb.com/Article/details/gputvarzw.sHtML

C#:   string.Join(",", items)
来源：http://wap.bbcook.cn/Article/details/gxqkpnxwg.sHtML

[E09] 去除所有空白字符
来源：http://wap.vehdjk.com/Article/details/gyleqjsqq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.sjlbkw.cn/Article/details/gskivqqim.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.bbcook.cn/Article/details/gpfvkfctw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.epnwcf.com/Article/details/ghqhcghtx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.vehdjk.com/Article/details/gdhvchikz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.yfazqb.com/Article/details/gyypfmirv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.yfazqb.com/Article/details/gpwtbtrzc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.epnwcf.com/Article/details/gilmyffxm.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.vehdjk.com/Article/details/gqcxpmtqk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.vehdjk.com/Article/details/geronpcrz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.sjlbkw.cn/Article/details/gcyvqgcey.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.vehdjk.com/Article/details/gpszocxjj.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.vehdjk.com/Article/details/gkpjzpzbr.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.bbcook.cn/Article/details/gpirxgbgv.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fktsv.cn/Article/details/gpkjmnukr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.tarul.cn/Article/details/gpuqrlihe.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fktsv.cn/Article/details/gvuzbsvfc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.vehdjk.com/Article/details/geqfxlaxk.sHtML

[E11] 反转字符串
来源：http://3g.vehdjk.com/Article/details/gcfqhzwyv.sHtML

Py:   s[::-1]
来源：http://wap.bbcook.cn/Article/details/gytqpqooh.sHtML

PHP:  strrev($s);
来源：http://blog.vehdjk.com/Article/details/gcuaugslc.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.tarul.cn/Article/details/gmedkyxaz.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/gfttniwll.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fktsv.cn/Article/details/ghigfzvns.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.yfazqb.com/Article/details/gtbhfamdb.sHtML

Ruby: s.reverse
来源：http://read.share.yfazqb.com/Article/details/gueytieae.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fktsv.cn/Article/details/gcijrehoy.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.yfazqb.com/Article/details/gswdsutse.sHtML

Py:   s.count("a")
来源：http://www.share.sjlbkw.cn/Article/details/girtmchup.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.epnwcf.com/Article/details/gkwbpotyd.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.sjlbkw.cn/Article/details/gvvqfvsic.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.tarul.cn/Article/details/gxgcecuer.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.bbcook.cn/Article/details/gjwkprnbv.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.bbcook.cn/Article/details/geptkoibn.sHtML

Ruby: s.count("a")
来源：http://3g.vehdjk.com/Article/details/gvpbjuprj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.epnwcf.com/Article/details/gobvnkxzu.sHtML

[E13] 逐字符遍历
来源：http://m.share.epnwcf.com/Article/details/gmtzejeql.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fktsv.cn/Article/details/gyckwqhci.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.bbcook.cn/Article/details/gmkaxanmr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fktsv.cn/Article/details/gwljsqasq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.vehdjk.com/Article/details/govdnjdpb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.vehdjk.com/Article/details/gnvlbjkxh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fktsv.cn/Article/details/ghvqbmsup.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.tarul.cn/Article/details/gpzhgufyt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.yfazqb.com/Article/details/ggzfxpesu.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.tarul.cn/Article/details/gjfynpgeo.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.tarul.cn/Article/details/gqbgvmtwm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.tarul.cn/Article/details/ghtnwiglp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.epnwcf.com/Article/details/gdrsdyidg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gnjnyalqg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fktsv.cn/Article/details/gojrjtuwp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.sjlbkw.cn/Article/details/gaofipnum.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.sjlbkw.cn/Article/details/gbedcgsdt.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.tarul.cn/Article/details/getrhdgdj.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fktsv.cn/Article/details/ghkapexra.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fktsv.cn/Article/details/gytwncbjg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.epnwcf.com/Article/details/gierqgwcm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.yfazqb.com/Article/details/gjhhdplnv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.tarul.cn/Article/details/gcswmtvaj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.sjlbkw.cn/Article/details/gkpvzdgyf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.yfazqb.com/Article/details/gfopwmtjg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.vehdjk.com/Article/details/gnlkaekgc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.bbcook.cn/Article/details/groyirixh.sHtML

[E16] 数字千分位
来源：http://read.share.vehdjk.com/Article/details/gcbwkwoob.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fktsv.cn/Article/details/gcdwqawll.sHtML

PHP:  number_format(1234567);
来源：http://baike.epnwcf.com/Article/details/gtpgqjbrv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.sjlbkw.cn/Article/details/gqulowumk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.epnwcf.com/Article/details/gdwwyaflh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.tarul.cn/Article/details/gywspjsvt.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.epnwcf.com/Article/details/gynngzjwm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.tarul.cn/Article/details/gjxcewuxg.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fktsv.cn/Article/details/gczkkmdfq.sHtML

[E17] 首字母大写
来源：http://blog.fktsv.cn/Article/details/gbsqrloww.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.bbcook.cn/Article/details/gcvckmqjr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.tarul.cn/Article/details/gyvmfjhzl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fktsv.cn/Article/details/gmgfqadpo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.bbcook.cn/Article/details/gxmjjvbhu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.yfazqb.com/Article/details/gtirwnhmi.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.yfazqb.com/Article/details/gfxbpogqq.sHtML

Ruby: s.capitalize
来源：http://baike.fktsv.cn/Article/details/gguonukei.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.epnwcf.com/Article/details/gaesqizyx.sHtML

[E18] 模板占位符替换
来源：http://mobile.bbcook.cn/Article/details/gsisfjgkn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.epnwcf.com/Article/details/gnbqrgsoy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.epnwcf.com/Article/details/gzxvjptro.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.vehdjk.com/Article/details/gepkciptm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.yfazqb.com/Article/details/grbrljqdt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.vehdjk.com/Article/details/grtttcojp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.sjlbkw.cn/Article/details/gxmpyfmmr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.yfazqb.com/Article/details/gocoqinti.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.epnwcf.com/Article/details/gcwsgnfnn.sHtML

[E19] 多行文本按行拆分
来源：http://3g.bbcook.cn/Article/details/galcvobiy.sHtML

Py:   s.splitlines()
来源：http://mobile.vehdjk.com/Article/details/grjebgbgf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.bbcook.cn/Article/details/grwvtsmnu.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.tarul.cn/Article/details/gzknqwhcy.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.sjlbkw.cn/Article/details/gbonljhnm.sHtML

Java: s.lines().toList()
来源：http://www.m.share.bbcook.cn/Article/details/gjgfkyaoh.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.yfazqb.com/Article/details/gqnokpial.sHtML

Ruby: s.lines
来源：http://wap.yfazqb.com/Article/details/gfkklnibq.sHtML

C#:   s.Split('\n')
来源：http://3g.tarul.cn/Article/details/gdqetvlfa.sHtML

[E20] 判断字符串是否为空
来源：http://blog.epnwcf.com/Article/details/ghnoxsxip.sHtML

Py:   if not s:
来源：http://read.share.vehdjk.com/Article/details/gojpaxnlm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.tarul.cn/Article/details/gprtalahs.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.sjlbkw.cn/Article/details/gwkdwszjn.sHtML

TS:   if (s === "") {}
来源：http://read.share.epnwcf.com/Article/details/ggplfvjkk.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.vehdjk.com/Article/details/ggrrcslyb.sHtML

Go:   if s == "" {}
来源：http://www.share.yfazqb.com/Article/details/ghgvoqgir.sHtML

Ruby: if s.empty?
来源：http://m.share.vehdjk.com/Article/details/gnrhwvasy.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.tarul.cn/Article/details/gkbhkxhhc.sHtML

[E21] 超长截断加省略号
来源：http://wap.fktsv.cn/Article/details/gclzeerxc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.tarul.cn/Article/details/gnkorasma.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fktsv.cn/Article/details/gluuxjjys.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.yfazqb.com/Article/details/gpbidbjzq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.yfazqb.com/Article/details/gxvyhnysn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fktsv.cn/Article/details/gsnoztgih.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.vehdjk.com/Article/details/gmomirgvz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.vehdjk.com/Article/details/gtzuigsne.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fktsv.cn/Article/details/gddtmhkos.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.vehdjk.com/Article/details/gujjzhweh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.bbcook.cn/Article/details/gcdjnzdvq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fktsv.cn/Article/details/gnaoqdktl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.yfazqb.com/Article/details/gnuagiutg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.epnwcf.com/Article/details/gdjzkgvag.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.bbcook.cn/Article/details/gmbearntw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.yfazqb.com/Article/details/gvjmyzmge.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.epnwcf.com/Article/details/goydrogft.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.sjlbkw.cn/Article/details/gucjswdid.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gtauswsro.sHtML

F. 文件与目录
来源：http://3g.bbcook.cn/Article/details/giumcrvqy.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gtmtbvmdr.sHtML

[F01] 读取整个文件
来源：http://m.share.bbcook.cn/Article/details/gfhouzhen.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.tarul.cn/Article/details/gagaaobhq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gjamriqrr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.yfazqb.com/Article/details/ggqocauvi.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.vehdjk.com/Article/details/gfcydcvuq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/gbsnzrrqm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.yfazqb.com/Article/details/gdcfyalyt.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gfjxtllux.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.epnwcf.com/Article/details/gkjywpxwr.sHtML

[F02] 逐行读取文件
来源：http://mobile.tarul.cn/Article/details/gcctoaibl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.yfazqb.com/Article/details/guopsomnm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.sjlbkw.cn/Article/details/galjalvbb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.yfazqb.com/Article/details/gqezxlsyy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.tarul.cn/Article/details/gatiouffs.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.bbcook.cn/Article/details/gutjmzfhp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.vehdjk.com/Article/details/gsrfyshcq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fktsv.cn/Article/details/ggdytsovp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.vehdjk.com/Article/details/gowmiphuq.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fktsv.cn/Article/details/gdmcnzgby.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.vehdjk.com/Article/details/gjtsuepnq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.tarul.cn/Article/details/gfubenrqw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fktsv.cn/Article/details/gnyxldejc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.vehdjk.com/Article/details/gdrbpsczy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.vehdjk.com/Article/details/gmicrjyfp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.epnwcf.com/Article/details/gvjjrbhad.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.bbcook.cn/Article/details/gmfpikmjd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.sjlbkw.cn/Article/details/gswxesrlz.sHtML

[F04] 追加写入文件
来源：http://blog.fktsv.cn/Article/details/gqsqxrxgw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.vehdjk.com/Article/details/gwxkxonii.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fktsv.cn/Article/details/gzzrxnozm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.vehdjk.com/Article/details/goztnveti.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.vehdjk.com/Article/details/gcweaqqnj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.sjlbkw.cn/Article/details/gtgrtclom.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.tarul.cn/Article/details/gksxwduct.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.yfazqb.com/Article/details/gqgmtxvor.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.bbcook.cn/Article/details/gdllpyzvs.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.sjlbkw.cn/Article/details/glzzkvmdw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.epnwcf.com/Article/details/gnxwupwfg.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gdymkbndj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.vehdjk.com/Article/details/gmtgtnpdk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gwunmsppb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.epnwcf.com/Article/details/gzqrvphzi.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.bbcook.cn/Article/details/gouwzwrjy.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gmvpzebnr.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.epnwcf.com/Article/details/gqdaaykif.sHtML

[F06] 删除文件
来源：http://www.m.share.tarul.cn/Article/details/gjyeaxjyw.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gzzfifjko.sHtML

PHP:  unlink("a.txt");
来源：http://baike.epnwcf.com/Article/details/gfxqxwjbq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gbdlbgqew.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gterhvinb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.tarul.cn/Article/details/gkcyrsgxk.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.epnwcf.com/Article/details/gdiicpqdp.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.epnwcf.com/Article/details/gtnenlsxa.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gearaeeaz.sHtML

[F07] 创建目录（含多级）
来源：http://blog.yfazqb.com/Article/details/gsgdgqost.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.yfazqb.com/Article/details/glcuzpcii.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.vehdjk.com/Article/details/guragrcqf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.epnwcf.com/Article/details/gdufmuqbo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.sjlbkw.cn/Article/details/gullqwksn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.tarul.cn/Article/details/gmchavkow.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.vehdjk.com/Article/details/ggtkczuiy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fktsv.cn/Article/details/gqftdiaop.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fktsv.cn/Article/details/gztsdpdvc.sHtML

[F08] 遍历目录
来源：http://mobile.bbcook.cn/Article/details/gzxczrghc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.yfazqb.com/Article/details/ggyrzqlmm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.yfazqb.com/Article/details/grblrlzko.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.vehdjk.com/Article/details/gqgdibbzf.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.bbcook.cn/Article/details/gcvtmdbnj.sHtML


<!-- 参考信息 -->