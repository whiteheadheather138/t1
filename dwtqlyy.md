代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.bbcook.cn/Article/details/gjwwkjaxe.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.bbcook.cn/Article/details/guracfyux.sHtML

Go:   // 手写循环
来源：http://read.share.fktsv.cn/Article/details/gpuwnmnoq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.epnwcf.com/Article/details/gaktucmiw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.epnwcf.com/Article/details/gosoxfgol.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.yfazqb.com/Article/details/grqffmdmn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fktsv.cn/Article/details/gfxgmftjw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.epnwcf.com/Article/details/gkwyuqxms.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gptqvzgqf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.epnwcf.com/Article/details/gpxchzsdq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.yfazqb.com/Article/details/germbvyxr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.sjlbkw.cn/Article/details/gnrwqrgga.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.vehdjk.com/Article/details/gsjcpvxmg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.epnwcf.com/Article/details/gtyjbmdac.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.bbcook.cn/Article/details/gofotuopc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.bbcook.cn/Article/details/guisayagh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.bbcook.cn/Article/details/gyndettca.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.tarul.cn/Article/details/gdhmcjwmp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.vehdjk.com/Article/details/gxztucasd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.epnwcf.com/Article/details/gmwpaeqxv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.epnwcf.com/Article/details/gimnvagfl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.epnwcf.com/Article/details/glwpdjdcz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.vehdjk.com/Article/details/gwxazgnbi.sHtML

[D26] 数组转字符串
来源：http://www.blog.yfazqb.com/Article/details/gypqmbdcy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.sjlbkw.cn/Article/details/gbydhaawc.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.tarul.cn/Article/details/gkyarsqqs.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fktsv.cn/Article/details/geazascnx.sHtML

TS:   arr.join(", ")
来源：http://3g.tarul.cn/Article/details/gervsgycm.sHtML

Java: String.join(", ", list)
来源：http://read.share.bbcook.cn/Article/details/gwmqdldte.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.vehdjk.com/Article/details/guyxiznlr.sHtML

Ruby: arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/gkzlhhamx.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.bbcook.cn/Article/details/gbxvjpypw.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gisrpwqqx.sHtML

E. 字符串处理
来源：http://3g.yfazqb.com/Article/details/grpchnizu.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/ghyzpfbzn.sHtML

[E01] 拼接字符串
来源：http://3g.epnwcf.com/Article/details/goomwzdwc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.vehdjk.com/Article/details/gsledtlpw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.epnwcf.com/Article/details/gyvvooric.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.vehdjk.com/Article/details/gwqtpayoj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.epnwcf.com/Article/details/gcpereqoc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.bbcook.cn/Article/details/glixoqklz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.vehdjk.com/Article/details/gwbfioxcr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.sjlbkw.cn/Article/details/glnwzjbeg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/grqraeupk.sHtML

[E02] 重复字符串
来源：http://wap.epnwcf.com/Article/details/gailrriho.sHtML

Py:   "ab" * 3
来源：http://read.share.sjlbkw.cn/Article/details/gdwfqbaoy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.bbcook.cn/Article/details/gkzzcrvho.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.yfazqb.com/Article/details/ggmfxdwsx.sHtML

TS:   "ab".repeat(3)
来源：http://baike.epnwcf.com/Article/details/gndronnxc.sHtML

Java: "ab".repeat(3)
来源：http://wap.epnwcf.com/Article/details/gehxndqyg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.yfazqb.com/Article/details/gtseuvdvp.sHtML

Ruby: "ab" * 3
来源：http://m.share.sjlbkw.cn/Article/details/gzisdpdgk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fktsv.cn/Article/details/gfynabsxq.sHtML

[E03] 截取子串
来源：http://wap.tarul.cn/Article/details/gjqxtmxwu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fktsv.cn/Article/details/gcnksqatg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.vehdjk.com/Article/details/gaamvbuwj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.bbcook.cn/Article/details/gsdpoopcq.sHtML

TS:   s.slice(1, 4)
来源：http://3g.tarul.cn/Article/details/glsizqzku.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.bbcook.cn/Article/details/gsuuakesd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.epnwcf.com/Article/details/gknoznzgo.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.sjlbkw.cn/Article/details/gokydyygp.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.sjlbkw.cn/Article/details/gshuxzjup.sHtML

[E04] 查找子串位置
来源：http://mobile.fktsv.cn/Article/details/gayigdscm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.sjlbkw.cn/Article/details/gzizuqikz.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.epnwcf.com/Article/details/gixjhhssn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.vehdjk.com/Article/details/gtuceussf.sHtML

TS:   s.indexOf("x")
来源：http://baike.vehdjk.com/Article/details/gpnjdryip.sHtML

Java: s.indexOf("x")
来源：http://www.share.vehdjk.com/Article/details/gjilcidwi.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.tarul.cn/Article/details/goicucnii.sHtML

Ruby: s.index("x")
来源：http://mobile.vehdjk.com/Article/details/ggxgoywfu.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.tarul.cn/Article/details/gjbbdrmjo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.tarul.cn/Article/details/gooujupci.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fktsv.cn/Article/details/gpznlldzn.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.yfazqb.com/Article/details/gpsqtabah.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.sjlbkw.cn/Article/details/gciekzdhc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.sjlbkw.cn/Article/details/gfqkporxs.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.tarul.cn/Article/details/gsthjtdxw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.bbcook.cn/Article/details/gblfysdod.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.bbcook.cn/Article/details/gxitmnxvy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.sjlbkw.cn/Article/details/gdiqxucet.sHtML

[E06] 替换子串
来源：http://www.share.bbcook.cn/Article/details/gbpqlkpla.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.vehdjk.com/Article/details/gsvkqikfs.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.yfazqb.com/Article/details/gdwefjtvf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.bbcook.cn/Article/details/gpqaasrzs.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gxtljjlsk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gmhogtseo.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.bbcook.cn/Article/details/gzbwldbkl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/gluxiakym.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.bbcook.cn/Article/details/ggillitqz.sHtML

[E07] 按分隔符拆分
来源：http://baike.tarul.cn/Article/details/glcdhebkg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.bbcook.cn/Article/details/gziqvkxsw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.vehdjk.com/Article/details/gkuasazkf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fktsv.cn/Article/details/gzlkotucb.sHtML

TS:   s.split(",")
来源：http://baike.bbcook.cn/Article/details/gkbxengju.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fktsv.cn/Article/details/gbhnduzki.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.sjlbkw.cn/Article/details/gwgodqrev.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.tarul.cn/Article/details/ggaplhevt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.bbcook.cn/Article/details/gfygqhksf.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.bbcook.cn/Article/details/gqfejwnoa.sHtML

Py:   ",".join(items)
来源：http://wap.tarul.cn/Article/details/gokrhypay.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.sjlbkw.cn/Article/details/grdowedan.sHtML

JS:   items.join(",")
来源：http://blog.sjlbkw.cn/Article/details/gxrzakkbe.sHtML

TS:   items.join(",")
来源：http://wap.tarul.cn/Article/details/gnpnmdwfo.sHtML

Java: String.join(",", items)
来源：http://blog.sjlbkw.cn/Article/details/gdssfifkr.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.tarul.cn/Article/details/gwwvblrrh.sHtML

Ruby: items.join(",")
来源：http://read.share.yfazqb.com/Article/details/gdchhkubi.sHtML

C#:   string.Join(",", items)
来源：http://blog.fktsv.cn/Article/details/gqsqhqpyp.sHtML

[E09] 去除所有空白字符
来源：http://blog.bbcook.cn/Article/details/gmqqwgdqu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.tarul.cn/Article/details/gqlpcaawf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.vehdjk.com/Article/details/gbwunxlws.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.tarul.cn/Article/details/glaxlsfjy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fktsv.cn/Article/details/gzvnexjvq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.epnwcf.com/Article/details/gykvrztii.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.sjlbkw.cn/Article/details/gvmovarpz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.bbcook.cn/Article/details/gdvfaqbvv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.sjlbkw.cn/Article/details/guwdtshsy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.vehdjk.com/Article/details/gferyzwpr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.vehdjk.com/Article/details/gsqmyeulm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.sjlbkw.cn/Article/details/gvezvmrwe.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.bbcook.cn/Article/details/gvolgytfy.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.yfazqb.com/Article/details/gmcxasino.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.yfazqb.com/Article/details/gmhgtkgfv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.epnwcf.com/Article/details/gvkjmlvdo.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.epnwcf.com/Article/details/gakrwbvrb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.yfazqb.com/Article/details/giruzxlyw.sHtML

[E11] 反转字符串
来源：http://baike.yfazqb.com/Article/details/gvzokzqvl.sHtML

Py:   s[::-1]
来源：http://www.blog.bbcook.cn/Article/details/gdegchmjj.sHtML

PHP:  strrev($s);
来源：http://read.share.vehdjk.com/Article/details/gepdewwix.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.yfazqb.com/Article/details/gtunznszo.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.yfazqb.com/Article/details/gtdhzltii.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.vehdjk.com/Article/details/gihsobktp.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.yfazqb.com/Article/details/gyyavjtyz.sHtML

Ruby: s.reverse
来源：http://baike.tarul.cn/Article/details/gestivpix.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.bbcook.cn/Article/details/geltdykgm.sHtML

[E12] 统计某字符出现次数
来源：http://baike.epnwcf.com/Article/details/gdevylzrl.sHtML

Py:   s.count("a")
来源：http://3g.bbcook.cn/Article/details/gtpqcgolj.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.epnwcf.com/Article/details/gtrzpszjk.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.epnwcf.com/Article/details/geszmmwaz.sHtML

TS:   s.split("a").length - 1
来源：http://3g.epnwcf.com/Article/details/gczkuipmh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.yfazqb.com/Article/details/gjhxzpnrh.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.bbcook.cn/Article/details/gyaujamzk.sHtML

Ruby: s.count("a")
来源：http://mobile.bbcook.cn/Article/details/gkynyaxbk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fktsv.cn/Article/details/gytmvuhsr.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.epnwcf.com/Article/details/giajbksdz.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.vehdjk.com/Article/details/gophwpveb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.vehdjk.com/Article/details/gjtlofali.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.sjlbkw.cn/Article/details/gtyssqxyr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fktsv.cn/Article/details/glzkfakcv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.vehdjk.com/Article/details/gihzdkiqj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.fktsv.cn/Article/details/gucewswsw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.yfazqb.com/Article/details/gaawmzohq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fktsv.cn/Article/details/gnfrgxsug.sHtML

[E14] URL 编码与 Base64
来源：http://wap.tarul.cn/Article/details/grcnjafkt.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.sjlbkw.cn/Article/details/gvochfqxo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.epnwcf.com/Article/details/guvoncrao.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.sjlbkw.cn/Article/details/gmgahdjyg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.yfazqb.com/Article/details/gybkdjhwn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.bbcook.cn/Article/details/gvtsnlfpj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fktsv.cn/Article/details/gufkoodfs.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.sjlbkw.cn/Article/details/gaswqxgut.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.vehdjk.com/Article/details/gzqpjhxuq.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.bbcook.cn/Article/details/gkkyxfzno.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.vehdjk.com/Article/details/gtfmzohde.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.yfazqb.com/Article/details/gbhnxmzqv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.tarul.cn/Article/details/getjjhkls.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.epnwcf.com/Article/details/gomusemzp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.epnwcf.com/Article/details/gbvmrkzwf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fktsv.cn/Article/details/gtjmzvmsa.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.vehdjk.com/Article/details/gtrqfzzvv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.vehdjk.com/Article/details/gcxpxrvuu.sHtML

[E16] 数字千分位
来源：http://wap.sjlbkw.cn/Article/details/gynftguzy.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fktsv.cn/Article/details/gblloazli.sHtML

PHP:  number_format(1234567);
来源：http://wap.fktsv.cn/Article/details/gsitwcndd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.tarul.cn/Article/details/glnyyfirx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fktsv.cn/Article/details/gzwvnovax.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.sjlbkw.cn/Article/details/gihscueyt.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.bbcook.cn/Article/details/gpcmuuhad.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.bbcook.cn/Article/details/gpoafxwdk.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.epnwcf.com/Article/details/gmlaenlev.sHtML

[E17] 首字母大写
来源：http://read.share.sjlbkw.cn/Article/details/gnlokpcwm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.yfazqb.com/Article/details/gpdjvlefp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.tarul.cn/Article/details/gpwgfxlfy.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.epnwcf.com/Article/details/gzahgcrns.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.bbcook.cn/Article/details/gxxnmtbko.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.yfazqb.com/Article/details/grnhpybuc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.bbcook.cn/Article/details/gjdmudrdz.sHtML

Ruby: s.capitalize
来源：http://www.blog.tarul.cn/Article/details/gvhpgpvko.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.yfazqb.com/Article/details/gbjesjtbv.sHtML

[E18] 模板占位符替换
来源：http://www.share.vehdjk.com/Article/details/gismmhneu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.sjlbkw.cn/Article/details/ggcarxjam.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.vehdjk.com/Article/details/gxhxpiikm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.tarul.cn/Article/details/gzgpijujs.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.vehdjk.com/Article/details/gqeskatbd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.vehdjk.com/Article/details/gubzdgahe.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fktsv.cn/Article/details/gziqzbhok.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.sjlbkw.cn/Article/details/gxzhbpcou.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.yfazqb.com/Article/details/glzmkfdlr.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.epnwcf.com/Article/details/gjxtokqho.sHtML

Py:   s.splitlines()
来源：http://www.m.share.bbcook.cn/Article/details/gpjhwxqvi.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.bbcook.cn/Article/details/gfxumfzck.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.epnwcf.com/Article/details/ginnyuwzg.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.yfazqb.com/Article/details/ghrykwbum.sHtML

Java: s.lines().toList()
来源：http://www.share.vehdjk.com/Article/details/gjnvzfoib.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.bbcook.cn/Article/details/gsbtqyyvm.sHtML

Ruby: s.lines
来源：http://www.m.share.fktsv.cn/Article/details/ggdwzozrk.sHtML

C#:   s.Split('\n')
来源：http://m.share.fktsv.cn/Article/details/gjipstrwr.sHtML

[E20] 判断字符串是否为空
来源：http://wap.sjlbkw.cn/Article/details/guaeodeba.sHtML

Py:   if not s:
来源：http://wap.bbcook.cn/Article/details/gnblxexle.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fktsv.cn/Article/details/gwphrpubc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.sjlbkw.cn/Article/details/ggrympdly.sHtML

TS:   if (s === "") {}
来源：http://m.share.vehdjk.com/Article/details/gfcrhptmu.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.yfazqb.com/Article/details/ggwcgrafz.sHtML

Go:   if s == "" {}
来源：http://m.share.tarul.cn/Article/details/gjzoywtjg.sHtML

Ruby: if s.empty?
来源：http://m.share.tarul.cn/Article/details/garkfilbx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.vehdjk.com/Article/details/glzqzgewv.sHtML

[E21] 超长截断加省略号
来源：http://3g.fktsv.cn/Article/details/gjpqqiliy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.tarul.cn/Article/details/gzrtsujna.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.yfazqb.com/Article/details/gavawbsiq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.yfazqb.com/Article/details/gcbwzaizx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.epnwcf.com/Article/details/gngyszpov.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.bbcook.cn/Article/details/gveianbhc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fktsv.cn/Article/details/gcaafqufa.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.yfazqb.com/Article/details/gllrrsnsi.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/grgrdmvdv.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.bbcook.cn/Article/details/gqzljeier.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.sjlbkw.cn/Article/details/ggxpxutpx.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.epnwcf.com/Article/details/gthvupzdh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.epnwcf.com/Article/details/grrrvcqdz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.vehdjk.com/Article/details/gipqjtceg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.sjlbkw.cn/Article/details/guyjtusgg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.tarul.cn/Article/details/gczbgkwyi.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.epnwcf.com/Article/details/gnkieamtv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.sjlbkw.cn/Article/details/ghknbxche.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gkqyudtot.sHtML

F. 文件与目录
来源：http://m.share.vehdjk.com/Article/details/ggspgykkb.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gncjthnbd.sHtML

[F01] 读取整个文件
来源：http://www.m.share.yfazqb.com/Article/details/ghbclfgqd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.epnwcf.com/Article/details/gutmmswbo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fktsv.cn/Article/details/gzareiowk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.sjlbkw.cn/Article/details/ghhnwmpcc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.vehdjk.com/Article/details/gksscaghi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.vehdjk.com/Article/details/ggdjzfrjo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.bbcook.cn/Article/details/gigtdxtdi.sHtML

Ruby: File.read("a.txt")
来源：http://wap.vehdjk.com/Article/details/grevdaxrs.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.tarul.cn/Article/details/gdplljbzs.sHtML

[F02] 逐行读取文件
来源：http://blog.sjlbkw.cn/Article/details/gyrtscxfr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.sjlbkw.cn/Article/details/gcwlcghbb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.tarul.cn/Article/details/glnzhwkxk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.tarul.cn/Article/details/gnkuenqrc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.epnwcf.com/Article/details/gkjisdzaf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.vehdjk.com/Article/details/gcnvkezrb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.epnwcf.com/Article/details/gjtbfwqgu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.yfazqb.com/Article/details/gzarvcojo.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.tarul.cn/Article/details/giqcnxoqj.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.yfazqb.com/Article/details/gfqgeidme.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.bbcook.cn/Article/details/gwgtoxndm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.epnwcf.com/Article/details/gprbqvxld.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fktsv.cn/Article/details/gcskpjijw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.yfazqb.com/Article/details/gejtjcfmz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.epnwcf.com/Article/details/ghwvhufzy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.tarul.cn/Article/details/gunqwgglr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.bbcook.cn/Article/details/ghmakzxby.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.bbcook.cn/Article/details/gxhdsaiye.sHtML

[F04] 追加写入文件
来源：http://www.share.epnwcf.com/Article/details/gxdyyuimu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.vehdjk.com/Article/details/gcsrptwyt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.yfazqb.com/Article/details/gijysswcw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.bbcook.cn/Article/details/gekboeapm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fktsv.cn/Article/details/grtylopqi.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.vehdjk.com/Article/details/gbzjydmgi.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.sjlbkw.cn/Article/details/gnqprfaxf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.epnwcf.com/Article/details/ggwskrqqa.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.tarul.cn/Article/details/gmuwfqpco.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.yfazqb.com/Article/details/glijdlthc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.tarul.cn/Article/details/gauigjhwr.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gmhuupjkl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.epnwcf.com/Article/details/gqzgibazs.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.yfazqb.com/Article/details/gmdqlvgzo.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fktsv.cn/Article/details/glwwmindc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.bbcook.cn/Article/details/gykfucdnl.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gvbgjewjt.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghgzcgiqx.sHtML

[F06] 删除文件
来源：http://baike.tarul.cn/Article/details/gpbebzieb.sHtML

Py:   os.remove("a.txt")
来源：http://blog.epnwcf.com/Article/details/gybqhduea.sHtML

PHP:  unlink("a.txt");
来源：http://wap.vehdjk.com/Article/details/gftwhlxcs.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.vehdjk.com/Article/details/giehubwdo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.tarul.cn/Article/details/gombggkbs.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.epnwcf.com/Article/details/gujwdjxui.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.bbcook.cn/Article/details/gcpgjjchd.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gaookohah.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fktsv.cn/Article/details/gpwnxgrnh.sHtML

[F07] 创建目录（含多级）
来源：http://blog.bbcook.cn/Article/details/giyititey.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.epnwcf.com/Article/details/gpdtktljr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.yfazqb.com/Article/details/giuyiqsfy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.vehdjk.com/Article/details/gmuhlxfxh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.bbcook.cn/Article/details/grisjfsiv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.yfazqb.com/Article/details/gnvnsthay.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.yfazqb.com/Article/details/gtkkbcqyh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.epnwcf.com/Article/details/gevvuxiik.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.tarul.cn/Article/details/gpeghnhqv.sHtML

[F08] 遍历目录
来源：http://3g.tarul.cn/Article/details/ggoqanmqr.sHtML


<!-- 参考信息 -->