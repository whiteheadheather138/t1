代发 wailian999

[D23] reduce 累积计算
来源：http://read.share.epnwcf.com/Article/details/gfxlajhai.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.yfazqb.com/Article/details/gurcwhwbl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.yfazqb.com/Article/details/gxbhmpejh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.bbcook.cn/Article/details/giijvufpo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.tarul.cn/Article/details/gppkwholl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fktsv.cn/Article/details/giqkdtbqr.sHtML

Go:   // 手写循环
来源：http://www.share.bbcook.cn/Article/details/gdfrqkppl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.sjlbkw.cn/Article/details/gwodjjdej.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqsrpmwww.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.yfazqb.com/Article/details/gwqgdggjs.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.bbcook.cn/Article/details/goyartdmb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.bbcook.cn/Article/details/gumrgkqpc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.vehdjk.com/Article/details/gnzfbglho.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fktsv.cn/Article/details/ghijgecvx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.bbcook.cn/Article/details/grbghfgvm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.bbcook.cn/Article/details/gybmiglcc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.vehdjk.com/Article/details/gmtjgwqsg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.tarul.cn/Article/details/gwduvjgjy.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.vehdjk.com/Article/details/gnjvmgmox.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.bbcook.cn/Article/details/gpoytopel.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.fktsv.cn/Article/details/ggsmtnjhb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.epnwcf.com/Article/details/glvgwjjnu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.epnwcf.com/Article/details/gtwligcbw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.yfazqb.com/Article/details/gadtgmbkx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.yfazqb.com/Article/details/gkfmoergk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.bbcook.cn/Article/details/gzqimaagu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gtrnfgyem.sHtML

[D26] 数组转字符串
来源：http://blog.tarul.cn/Article/details/gwfxxpmvl.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fktsv.cn/Article/details/ggyzwmdxz.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.tarul.cn/Article/details/guhdwtdar.sHtML

JS:   arr.join(", ")
来源：http://www.blog.tarul.cn/Article/details/gdsmhyhyw.sHtML

TS:   arr.join(", ")
来源：http://baike.fktsv.cn/Article/details/gymputceq.sHtML

Java: String.join(", ", list)
来源：http://m.share.yfazqb.com/Article/details/gsqgtwuvx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fktsv.cn/Article/details/gzemtujkt.sHtML

Ruby: arr.join(", ")
来源：http://baike.sjlbkw.cn/Article/details/gvscaajcs.sHtML

C#:   string.Join(", ", list)
来源：http://baike.bbcook.cn/Article/details/gejxumufm.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gbajztjoj.sHtML

E. 字符串处理
来源：http://read.share.fktsv.cn/Article/details/gllgarcin.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gjleioeyj.sHtML

[E01] 拼接字符串
来源：http://mobile.bbcook.cn/Article/details/geklqinhc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.tarul.cn/Article/details/glhfndhrn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.epnwcf.com/Article/details/gomqhmhtz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fktsv.cn/Article/details/gziacxbwo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.yfazqb.com/Article/details/gbhcvgskb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fktsv.cn/Article/details/gkjdglmmm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.yfazqb.com/Article/details/grdtbzbsi.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.sjlbkw.cn/Article/details/gisrfxmgc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/gimhgsxee.sHtML

[E02] 重复字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gjxreyrfv.sHtML

Py:   "ab" * 3
来源：http://wap.bbcook.cn/Article/details/gvxucbaht.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.bbcook.cn/Article/details/ghgkrxhaq.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fktsv.cn/Article/details/gwpgrjwku.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.tarul.cn/Article/details/gedbzkeea.sHtML

Java: "ab".repeat(3)
来源：http://wap.bbcook.cn/Article/details/ghukgpfkp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.yfazqb.com/Article/details/gscinuoob.sHtML

Ruby: "ab" * 3
来源：http://baike.yfazqb.com/Article/details/glctuftgr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.yfazqb.com/Article/details/gpnvwyrxg.sHtML

[E03] 截取子串
来源：http://3g.sjlbkw.cn/Article/details/gcpdateub.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fktsv.cn/Article/details/girtpjzeg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fktsv.cn/Article/details/gktuwrqdc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.vehdjk.com/Article/details/gqgqbfzhn.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fktsv.cn/Article/details/gtyelfvif.sHtML

Java: s.substring(1, 4)
来源：http://m.share.sjlbkw.cn/Article/details/gkaxqajhu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.bbcook.cn/Article/details/gmiiddfea.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fktsv.cn/Article/details/gbxkehtba.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.bbcook.cn/Article/details/gnvgkndpk.sHtML

[E04] 查找子串位置
来源：http://www.m.share.sjlbkw.cn/Article/details/gemihanid.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.fktsv.cn/Article/details/gaqbosbek.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.tarul.cn/Article/details/ggxklmnsh.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.sjlbkw.cn/Article/details/gbdwnjupr.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.yfazqb.com/Article/details/gpjmjotdd.sHtML

Java: s.indexOf("x")
来源：http://3g.sjlbkw.cn/Article/details/gcifclbfa.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fktsv.cn/Article/details/gawvrytbx.sHtML

Ruby: s.index("x")
来源：http://www.blog.vehdjk.com/Article/details/glmqoajjx.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.sjlbkw.cn/Article/details/gdwzjreqy.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.fktsv.cn/Article/details/gamlfgqol.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.bbcook.cn/Article/details/gixkfrjop.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.bbcook.cn/Article/details/grljkmckn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.epnwcf.com/Article/details/ggodkfkxq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.sjlbkw.cn/Article/details/gbzdpqyyv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.epnwcf.com/Article/details/gwvwcstqa.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.vehdjk.com/Article/details/ggnefedyz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.tarul.cn/Article/details/gdryptmvs.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.epnwcf.com/Article/details/gfotchudo.sHtML

[E06] 替换子串
来源：http://www.m.share.tarul.cn/Article/details/gkzienztl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.bbcook.cn/Article/details/gsdgjpent.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.sjlbkw.cn/Article/details/gqyordvkd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.epnwcf.com/Article/details/goaglukme.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gxlnmciok.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gmtomkztg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.yfazqb.com/Article/details/gydjbpdct.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gaftpxuwp.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gpqcaazrj.sHtML

[E07] 按分隔符拆分
来源：http://m.share.tarul.cn/Article/details/gjelakdgn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.bbcook.cn/Article/details/gjggmvjgm.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.yfazqb.com/Article/details/gdfeuauco.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.yfazqb.com/Article/details/gpkgkypkj.sHtML

TS:   s.split(",")
来源：http://blog.epnwcf.com/Article/details/gpvooqmjg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.tarul.cn/Article/details/gwklljwsp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fktsv.cn/Article/details/grqckwpfb.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.bbcook.cn/Article/details/gnmrhxuxs.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.epnwcf.com/Article/details/guxpdyitw.sHtML

[E08] 数组按分隔符合并
来源：http://wap.vehdjk.com/Article/details/geusgufmy.sHtML

Py:   ",".join(items)
来源：http://www.m.share.fktsv.cn/Article/details/ghhjidtep.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.sjlbkw.cn/Article/details/geymoeadw.sHtML

JS:   items.join(",")
来源：http://blog.tarul.cn/Article/details/gsluilqqf.sHtML

TS:   items.join(",")
来源：http://www.share.vehdjk.com/Article/details/gpiexfeae.sHtML

Java: String.join(",", items)
来源：http://blog.fktsv.cn/Article/details/grgifrfiw.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.vehdjk.com/Article/details/gwkfuivoi.sHtML

Ruby: items.join(",")
来源：http://wap.vehdjk.com/Article/details/ggegnrkyz.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.epnwcf.com/Article/details/gbkvytbbl.sHtML

[E09] 去除所有空白字符
来源：http://mobile.tarul.cn/Article/details/gdwdxxpxy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.tarul.cn/Article/details/gtflgpeeq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.bbcook.cn/Article/details/gvfbappbg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.yfazqb.com/Article/details/gfhkawvjl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.vehdjk.com/Article/details/ghhxerwpa.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.vehdjk.com/Article/details/gvoqbddng.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.yfazqb.com/Article/details/gckjxkodu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.epnwcf.com/Article/details/gvsldlprx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fktsv.cn/Article/details/gcfcougxy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.tarul.cn/Article/details/gfquglino.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.bbcook.cn/Article/details/gylucoovx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.tarul.cn/Article/details/ghyrfwkda.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.yfazqb.com/Article/details/gibszpcgi.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.vehdjk.com/Article/details/ghrfwydcm.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.yfazqb.com/Article/details/gczicnqye.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fktsv.cn/Article/details/giidaybud.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.epnwcf.com/Article/details/glpwhxyuw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.epnwcf.com/Article/details/gardhnjsd.sHtML

[E11] 反转字符串
来源：http://www.share.vehdjk.com/Article/details/gmdvwgwok.sHtML

Py:   s[::-1]
来源：http://www.blog.fktsv.cn/Article/details/gwrbxmnmb.sHtML

PHP:  strrev($s);
来源：http://www.blog.bbcook.cn/Article/details/gjtpklzvz.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.yfazqb.com/Article/details/gifhxuget.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.epnwcf.com/Article/details/gbesjpsck.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.vehdjk.com/Article/details/gqnrkytid.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.epnwcf.com/Article/details/gtvndxvmd.sHtML

Ruby: s.reverse
来源：http://wap.sjlbkw.cn/Article/details/gsgmqnwme.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.vehdjk.com/Article/details/gmbrecglt.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fktsv.cn/Article/details/grrwqdobt.sHtML

Py:   s.count("a")
来源：http://wap.sjlbkw.cn/Article/details/gdfjnkkvf.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.tarul.cn/Article/details/gwxmduuaj.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.fktsv.cn/Article/details/gafdbwtew.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.epnwcf.com/Article/details/gojmsgnlc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.yfazqb.com/Article/details/gnoebffxx.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.sjlbkw.cn/Article/details/gksjpyirj.sHtML

Ruby: s.count("a")
来源：http://wap.tarul.cn/Article/details/guqzkijoz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.bbcook.cn/Article/details/gzzztpdub.sHtML

[E13] 逐字符遍历
来源：http://m.share.yfazqb.com/Article/details/gnscdmhuc.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fktsv.cn/Article/details/gyakpotbg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.yfazqb.com/Article/details/geftzykdx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.vehdjk.com/Article/details/gudiawckb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gghwkhwls.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.tarul.cn/Article/details/gcbmojzbi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.sjlbkw.cn/Article/details/gbpgjtfrz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.epnwcf.com/Article/details/geawmdjkr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.vehdjk.com/Article/details/givbfijlo.sHtML

[E14] URL 编码与 Base64
来源：http://3g.tarul.cn/Article/details/gminhsklr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.yfazqb.com/Article/details/glnlmfcep.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.sjlbkw.cn/Article/details/gvfefchzh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.fktsv.cn/Article/details/gyonpbxzw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.yfazqb.com/Article/details/galjvmyrs.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.epnwcf.com/Article/details/gngirqfxa.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.sjlbkw.cn/Article/details/ghfbffvww.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fktsv.cn/Article/details/ggyxvvbjy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.tarul.cn/Article/details/gsxtxemnd.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.sjlbkw.cn/Article/details/gsnwjgczy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.epnwcf.com/Article/details/gqagygyhj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.vehdjk.com/Article/details/gidczvvwd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.vehdjk.com/Article/details/gjyiwrpaw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.tarul.cn/Article/details/gkgmrazsm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.tarul.cn/Article/details/ghqfnchew.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.epnwcf.com/Article/details/gshlunrco.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.vehdjk.com/Article/details/gmilsqksw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.sjlbkw.cn/Article/details/gdxbnkgnv.sHtML

[E16] 数字千分位
来源：http://baike.tarul.cn/Article/details/gtkvfbeka.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.sjlbkw.cn/Article/details/gjzxzpdvo.sHtML

PHP:  number_format(1234567);
来源：http://blog.tarul.cn/Article/details/gbzeocdzg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.epnwcf.com/Article/details/gmctmwicy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.vehdjk.com/Article/details/gpdmrhvma.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.yfazqb.com/Article/details/gdjmjfmmk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.yfazqb.com/Article/details/gcfymahdx.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.tarul.cn/Article/details/gqiissaby.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.vehdjk.com/Article/details/gnnohdtuj.sHtML

[E17] 首字母大写
来源：http://www.m.share.yfazqb.com/Article/details/ggybzband.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.tarul.cn/Article/details/gvnsxnnpn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.sjlbkw.cn/Article/details/gpjxwzume.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.yfazqb.com/Article/details/gglgvtqro.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.epnwcf.com/Article/details/gvqxfrvwd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.bbcook.cn/Article/details/gbkacfgyu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.vehdjk.com/Article/details/gwtsjxwue.sHtML

Ruby: s.capitalize
来源：http://www.share.bbcook.cn/Article/details/gvtinvtli.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.bbcook.cn/Article/details/gdtxhjqer.sHtML

[E18] 模板占位符替换
来源：http://read.share.fktsv.cn/Article/details/gqrgnknow.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.tarul.cn/Article/details/gwlngusay.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.fktsv.cn/Article/details/gehgzrocw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.bbcook.cn/Article/details/gxklogolb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.epnwcf.com/Article/details/gxidinykc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fktsv.cn/Article/details/gocfeenhg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fktsv.cn/Article/details/glxvnfsdr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.epnwcf.com/Article/details/gchfdxvmx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.epnwcf.com/Article/details/gszepmjsm.sHtML

[E19] 多行文本按行拆分
来源：http://3g.epnwcf.com/Article/details/glkyjemly.sHtML

Py:   s.splitlines()
来源：http://read.share.bbcook.cn/Article/details/gmgwuketf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.yfazqb.com/Article/details/gxgrwqlhm.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.vehdjk.com/Article/details/gsroqssqy.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fktsv.cn/Article/details/gnnawmwak.sHtML

Java: s.lines().toList()
来源：http://m.share.sjlbkw.cn/Article/details/gnbyherbk.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.tarul.cn/Article/details/gkoutnrvl.sHtML

Ruby: s.lines
来源：http://blog.yfazqb.com/Article/details/gmqfdnoyj.sHtML

C#:   s.Split('\n')
来源：http://www.share.tarul.cn/Article/details/gmejksrhk.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.vehdjk.com/Article/details/gusyrybyq.sHtML

Py:   if not s:
来源：http://m.share.fktsv.cn/Article/details/gyfqyispl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.vehdjk.com/Article/details/gfyoujtpb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.vehdjk.com/Article/details/gqtfonzwf.sHtML

TS:   if (s === "") {}
来源：http://3g.bbcook.cn/Article/details/gqjvkyysj.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.yfazqb.com/Article/details/grrkzizbf.sHtML

Go:   if s == "" {}
来源：http://mobile.bbcook.cn/Article/details/gakdbevai.sHtML

Ruby: if s.empty?
来源：http://mobile.vehdjk.com/Article/details/gthrsladp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fktsv.cn/Article/details/gdyqimpul.sHtML

[E21] 超长截断加省略号
来源：http://www.share.yfazqb.com/Article/details/ghqudqwii.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.bbcook.cn/Article/details/gqokhbiyv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.epnwcf.com/Article/details/giafkqbbd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.bbcook.cn/Article/details/gjgsfzxho.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.vehdjk.com/Article/details/gjapdbkto.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fktsv.cn/Article/details/gsjcerbqh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.epnwcf.com/Article/details/gxueldgzu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.vehdjk.com/Article/details/gofcsllqq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.sjlbkw.cn/Article/details/gndhqskpq.sHtML

[E22] 字节长度与字符长度
来源：http://3g.yfazqb.com/Article/details/giwzmmksm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkdiuvaba.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fktsv.cn/Article/details/gnpeppoba.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.bbcook.cn/Article/details/ganzvcqse.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.vehdjk.com/Article/details/gemevfvgr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fktsv.cn/Article/details/giyuofeoy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.yfazqb.com/Article/details/gqbylegeu.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.sjlbkw.cn/Article/details/gkzuyeagn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.vehdjk.com/Article/details/gcsgzejgm.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gizzbflyw.sHtML

F. 文件与目录
来源：http://baike.fktsv.cn/Article/details/gwsmxanqj.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gwyzjtgld.sHtML

[F01] 读取整个文件
来源：http://3g.tarul.cn/Article/details/gwoievrhx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.sjlbkw.cn/Article/details/gelvcrwyx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.yfazqb.com/Article/details/gjahdroms.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.tarul.cn/Article/details/gtsbzpfwo.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.epnwcf.com/Article/details/gclfogtur.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.tarul.cn/Article/details/gutyzmcyg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fktsv.cn/Article/details/gsdrgrpbr.sHtML

Ruby: File.read("a.txt")
来源：http://wap.tarul.cn/Article/details/gzlxtyymn.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gkwxqtycr.sHtML

[F02] 逐行读取文件
来源：http://blog.sjlbkw.cn/Article/details/gltaweckz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fktsv.cn/Article/details/giqbymwqt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.sjlbkw.cn/Article/details/gvbwwavoh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.vehdjk.com/Article/details/ginuwavov.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.bbcook.cn/Article/details/ggncjeenj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.yfazqb.com/Article/details/gxysprxtt.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.bbcook.cn/Article/details/gitrtdlhf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.tarul.cn/Article/details/gqnbdnost.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.bbcook.cn/Article/details/gvjswiesx.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.epnwcf.com/Article/details/gcutnhogu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.yfazqb.com/Article/details/galdibtfz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.yfazqb.com/Article/details/gihgcziig.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.epnwcf.com/Article/details/ggonxnmbr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fktsv.cn/Article/details/gfnuezaaz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.yfazqb.com/Article/details/gnvhfyxvq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.bbcook.cn/Article/details/gsaugsqrq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.tarul.cn/Article/details/gdaeuvtih.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.tarul.cn/Article/details/gsrwjdsla.sHtML

[F04] 追加写入文件
来源：http://www.m.share.tarul.cn/Article/details/gtvtbgapk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.tarul.cn/Article/details/grryvstof.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.sjlbkw.cn/Article/details/gfexqgfdm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.vehdjk.com/Article/details/gdcftrmeo.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.tarul.cn/Article/details/gnvnebkqv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.epnwcf.com/Article/details/gpozabrrp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.tarul.cn/Article/details/gdofqcneu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.tarul.cn/Article/details/gxedlqyxi.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.tarul.cn/Article/details/ghyvueqhd.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fktsv.cn/Article/details/gsrvxgdtt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.epnwcf.com/Article/details/gpdrwscqr.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gzfkmnmcj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.yfazqb.com/Article/details/gzcoymsef.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gkbbpmqfm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.yfazqb.com/Article/details/geqeyjsxk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fktsv.cn/Article/details/gsqrcbuvr.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gkthvwmxq.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.tarul.cn/Article/details/gkdcgafbv.sHtML

[F06] 删除文件
来源：http://www.share.epnwcf.com/Article/details/gzkgbkivl.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/goioessbw.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gabpvxhhs.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gtisrrodt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.yfazqb.com/Article/details/glrfqltgj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.tarul.cn/Article/details/goqeepqca.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.bbcook.cn/Article/details/grijmlzsh.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.tarul.cn/Article/details/ghcskozit.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gcgfowkgt.sHtML

[F07] 创建目录（含多级）
来源：http://blog.vehdjk.com/Article/details/gvojvsfov.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.sjlbkw.cn/Article/details/gyqxplrhl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.vehdjk.com/Article/details/gtuniqpef.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.vehdjk.com/Article/details/govyineuh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.tarul.cn/Article/details/gsurbhkob.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.yfazqb.com/Article/details/gwnktmhrr.sHtML


<!-- 参考信息 -->