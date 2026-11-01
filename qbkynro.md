代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.epnwcf.com/Article/details/gjprzfeds.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.yfazqb.com/Article/details/gznuovgbj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.sjlbkw.cn/Article/details/gbnvvbdal.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.sjlbkw.cn/Article/details/gploklzpf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.epnwcf.com/Article/details/ganyhtzpo.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gfekxgrpy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.vehdjk.com/Article/details/gxjmacwae.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fktsv.cn/Article/details/grswxlhfn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.tarul.cn/Article/details/gbtfgfzjf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.tarul.cn/Article/details/ggowhmtkq.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.sjlbkw.cn/Article/details/gwvldbmjs.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fktsv.cn/Article/details/gnextzmgd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.sjlbkw.cn/Article/details/gsgzchjsr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.sjlbkw.cn/Article/details/gacuuobdj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.epnwcf.com/Article/details/gdexevmup.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.bbcook.cn/Article/details/gludaozin.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.tarul.cn/Article/details/gnmkqpuce.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.yfazqb.com/Article/details/gagvzsssp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fktsv.cn/Article/details/gidrccavu.sHtML

[D26] 数组转字符串
来源：http://baike.tarul.cn/Article/details/gvrmavyvh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.vehdjk.com/Article/details/gfaurmicv.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.bbcook.cn/Article/details/gdctyrmkj.sHtML

JS:   arr.join(", ")
来源：http://3g.sjlbkw.cn/Article/details/gcccsflyu.sHtML

TS:   arr.join(", ")
来源：http://www.blog.sjlbkw.cn/Article/details/gpbydeboi.sHtML

Java: String.join(", ", list)
来源：http://m.share.vehdjk.com/Article/details/gyexdutbh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.sjlbkw.cn/Article/details/gdfbntpvl.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fktsv.cn/Article/details/gmulpxrpc.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.tarul.cn/Article/details/gahvcycfj.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gndrcegfv.sHtML

E. 字符串处理
来源：http://wap.bbcook.cn/Article/details/gsypalwdb.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gtlskcjet.sHtML

[E01] 拼接字符串
来源：http://m.share.yfazqb.com/Article/details/gnpmnjyqr.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.yfazqb.com/Article/details/gbyyjnjiy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.sjlbkw.cn/Article/details/gylwadjny.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.bbcook.cn/Article/details/gzkvtmwav.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fktsv.cn/Article/details/gquyuodhx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.yfazqb.com/Article/details/geisxieqz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.tarul.cn/Article/details/gsxmwdfoh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fktsv.cn/Article/details/ggfcwtvaw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.vehdjk.com/Article/details/gkyxrqvqb.sHtML

[E02] 重复字符串
来源：http://m.share.bbcook.cn/Article/details/gqdvfsukz.sHtML

Py:   "ab" * 3
来源：http://read.share.epnwcf.com/Article/details/guilbdmaf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.tarul.cn/Article/details/gvmcnvlyc.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.vehdjk.com/Article/details/gyfvidsem.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fktsv.cn/Article/details/gjksdiggr.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.fktsv.cn/Article/details/guwhnatrp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fktsv.cn/Article/details/gpifolyil.sHtML

Ruby: "ab" * 3
来源：http://m.share.epnwcf.com/Article/details/gwvinqmwh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.sjlbkw.cn/Article/details/ghpphssau.sHtML

[E03] 截取子串
来源：http://www.m.share.fktsv.cn/Article/details/guqedxoqq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.epnwcf.com/Article/details/gdtydjnzg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.tarul.cn/Article/details/ggatgzets.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.vehdjk.com/Article/details/gtltsqadp.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.vehdjk.com/Article/details/gysjqcumq.sHtML

Java: s.substring(1, 4)
来源：http://blog.bbcook.cn/Article/details/gkmtcpdyn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fktsv.cn/Article/details/gbtqiosyf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.bbcook.cn/Article/details/glzlgakex.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.epnwcf.com/Article/details/gwqecxqyq.sHtML

[E04] 查找子串位置
来源：http://3g.yfazqb.com/Article/details/gqyfrroev.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggclsjvmg.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.bbcook.cn/Article/details/gbfkvbcox.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fktsv.cn/Article/details/gfuqjybpa.sHtML

TS:   s.indexOf("x")
来源：http://wap.vehdjk.com/Article/details/gqznxlidg.sHtML

Java: s.indexOf("x")
来源：http://read.share.tarul.cn/Article/details/gquaaivre.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.vehdjk.com/Article/details/gktrsliyk.sHtML

Ruby: s.index("x")
来源：http://baike.sjlbkw.cn/Article/details/glisyxxsq.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.epnwcf.com/Article/details/garexmhod.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.epnwcf.com/Article/details/ggglimtmr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.vehdjk.com/Article/details/gpkvprhmf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.epnwcf.com/Article/details/gijbtxgjg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fktsv.cn/Article/details/geumtzqjl.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.sjlbkw.cn/Article/details/gadsjmlnz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.bbcook.cn/Article/details/gaehdcnff.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.bbcook.cn/Article/details/gyxmghtyn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.epnwcf.com/Article/details/gdmwcrnzi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.sjlbkw.cn/Article/details/gvdxpnyje.sHtML

[E06] 替换子串
来源：http://baike.epnwcf.com/Article/details/geyhngzny.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.bbcook.cn/Article/details/gxjujhyyp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.epnwcf.com/Article/details/gcgmakaeo.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.yfazqb.com/Article/details/gwkisfwqg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fktsv.cn/Article/details/gbocmzmzg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.tarul.cn/Article/details/gzxkccfkc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.yfazqb.com/Article/details/grzlqhcth.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/ggtjtxfyi.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.yfazqb.com/Article/details/giwyavsbw.sHtML

[E07] 按分隔符拆分
来源：http://wap.epnwcf.com/Article/details/gxixapqmk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fktsv.cn/Article/details/gpabomxgc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.vehdjk.com/Article/details/grgjqcnup.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fktsv.cn/Article/details/genndscjm.sHtML

TS:   s.split(",")
来源：http://wap.sjlbkw.cn/Article/details/gyqosjltm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fktsv.cn/Article/details/gwtxetpla.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fktsv.cn/Article/details/giimfcrop.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.fktsv.cn/Article/details/guezmyiwt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.tarul.cn/Article/details/gedqpbrbm.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.bbcook.cn/Article/details/gyjyjxrfx.sHtML

Py:   ",".join(items)
来源：http://m.share.epnwcf.com/Article/details/gspombdrv.sHtML

PHP:  implode(",", $items);
来源：http://3g.tarul.cn/Article/details/gsvvvlcjt.sHtML

JS:   items.join(",")
来源：http://baike.tarul.cn/Article/details/gggbfczit.sHtML

TS:   items.join(",")
来源：http://www.blog.vehdjk.com/Article/details/gmbpqwsdq.sHtML

Java: String.join(",", items)
来源：http://blog.yfazqb.com/Article/details/ggqowxsud.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.tarul.cn/Article/details/gpdmuchaa.sHtML

Ruby: items.join(",")
来源：http://wap.yfazqb.com/Article/details/gfjyqonfb.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fktsv.cn/Article/details/gauasxjcm.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fktsv.cn/Article/details/gcwflyzle.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.vehdjk.com/Article/details/gnhurxcex.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.yfazqb.com/Article/details/gkmydouup.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.epnwcf.com/Article/details/gfergrcun.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.tarul.cn/Article/details/gmdwqrnhe.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.yfazqb.com/Article/details/gbboswjvh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.epnwcf.com/Article/details/gyqvmnjfz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.epnwcf.com/Article/details/gljhbfpvh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.sjlbkw.cn/Article/details/gtovgvffs.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.epnwcf.com/Article/details/gbjvecwpw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.sjlbkw.cn/Article/details/gdnbqhmzp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.sjlbkw.cn/Article/details/gfnbjxnii.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.bbcook.cn/Article/details/gmlrikkzc.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fktsv.cn/Article/details/gtokxpshy.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqzumzwfg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fktsv.cn/Article/details/gcxgtpmzh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.tarul.cn/Article/details/gnwnnioto.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.tarul.cn/Article/details/gtacfdwbh.sHtML

[E11] 反转字符串
来源：http://www.share.fktsv.cn/Article/details/gkwwfbovq.sHtML

Py:   s[::-1]
来源：http://mobile.bbcook.cn/Article/details/gmgjzcqge.sHtML

PHP:  strrev($s);
来源：http://m.share.fktsv.cn/Article/details/garptyacq.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.bbcook.cn/Article/details/gigqlgstj.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.sjlbkw.cn/Article/details/gvulibgca.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.bbcook.cn/Article/details/gmiunfnid.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fktsv.cn/Article/details/greqvyosc.sHtML

Ruby: s.reverse
来源：http://blog.epnwcf.com/Article/details/gzfkglqnp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.bbcook.cn/Article/details/gbzphujiv.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.vehdjk.com/Article/details/guszngjin.sHtML

Py:   s.count("a")
来源：http://read.share.bbcook.cn/Article/details/gbbjgvqsg.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.tarul.cn/Article/details/glgeuurhm.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gylxrhavq.sHtML

TS:   s.split("a").length - 1
来源：http://blog.sjlbkw.cn/Article/details/greqkxrnr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.sjlbkw.cn/Article/details/gbtwosbnq.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.vehdjk.com/Article/details/gshawwjlp.sHtML

Ruby: s.count("a")
来源：http://read.share.yfazqb.com/Article/details/givzxnuds.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fktsv.cn/Article/details/ggcvpvptb.sHtML

[E13] 逐字符遍历
来源：http://www.blog.yfazqb.com/Article/details/gttiesjsm.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.vehdjk.com/Article/details/grzkhjfol.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.bbcook.cn/Article/details/gkzvezfjm.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.vehdjk.com/Article/details/gufmignue.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.epnwcf.com/Article/details/gbckbstdh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.tarul.cn/Article/details/gmoszvhcf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.tarul.cn/Article/details/glakcredr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.tarul.cn/Article/details/ggnpmeiln.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.epnwcf.com/Article/details/gdyehqbmo.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.epnwcf.com/Article/details/grdqpnvaq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.tarul.cn/Article/details/grmkojrxy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fktsv.cn/Article/details/gfdanvjfh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.epnwcf.com/Article/details/gvavlyxgh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fktsv.cn/Article/details/grajyqfhg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.bbcook.cn/Article/details/gezubwyrx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fktsv.cn/Article/details/gpqxwddvr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.yfazqb.com/Article/details/gbglbprmg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fktsv.cn/Article/details/gvikdfnjb.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fktsv.cn/Article/details/gzjoevvyn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.bbcook.cn/Article/details/gvqsywutv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.sjlbkw.cn/Article/details/gjfxieqvg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.tarul.cn/Article/details/gfbpmvihv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.tarul.cn/Article/details/gmpotcusl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.vehdjk.com/Article/details/gcxzuhsez.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.epnwcf.com/Article/details/ghprojxgj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.sjlbkw.cn/Article/details/gwyoourlp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.epnwcf.com/Article/details/guiaqkzlf.sHtML

[E16] 数字千分位
来源：http://mobile.sjlbkw.cn/Article/details/goeomyevo.sHtML

Py:   f"{1234567:,}"
来源：http://blog.epnwcf.com/Article/details/giguzcdjr.sHtML

PHP:  number_format(1234567);
来源：http://blog.bbcook.cn/Article/details/grirxyzqc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.vehdjk.com/Article/details/gutuqmblf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.vehdjk.com/Article/details/gnihmahmy.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fktsv.cn/Article/details/gwppyarky.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.yfazqb.com/Article/details/gbntgzpps.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.vehdjk.com/Article/details/ggecgfzzh.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.sjlbkw.cn/Article/details/gzessxdzm.sHtML

[E17] 首字母大写
来源：http://3g.vehdjk.com/Article/details/gitnbwxsf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.tarul.cn/Article/details/gchfgaafr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.epnwcf.com/Article/details/guoelcmvs.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.epnwcf.com/Article/details/gvfzbwdop.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.vehdjk.com/Article/details/geyadjmaf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.tarul.cn/Article/details/gzmvswqgn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.tarul.cn/Article/details/gmvomnttd.sHtML

Ruby: s.capitalize
来源：http://www.m.share.sjlbkw.cn/Article/details/gpbhgltap.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.tarul.cn/Article/details/gceiqbfxl.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.epnwcf.com/Article/details/gfbgminrr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.yfazqb.com/Article/details/gnatlonvf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.sjlbkw.cn/Article/details/ghedttmhu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.epnwcf.com/Article/details/gedddqamh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.bbcook.cn/Article/details/grjfcniqg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fktsv.cn/Article/details/gbetykkgr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.vehdjk.com/Article/details/gphyrtgsl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.epnwcf.com/Article/details/gjeaxfegz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.tarul.cn/Article/details/gptwsfkzd.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.vehdjk.com/Article/details/gslpgljfr.sHtML

Py:   s.splitlines()
来源：http://www.blog.epnwcf.com/Article/details/gqetdsoek.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.bbcook.cn/Article/details/grronyddd.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fktsv.cn/Article/details/givlqgrfo.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.epnwcf.com/Article/details/genmtidvq.sHtML

Java: s.lines().toList()
来源：http://blog.yfazqb.com/Article/details/gylqtbgfb.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.epnwcf.com/Article/details/gusjsvbhy.sHtML

Ruby: s.lines
来源：http://m.share.fktsv.cn/Article/details/gsevvbycw.sHtML

C#:   s.Split('\n')
来源：http://read.share.yfazqb.com/Article/details/gbzuajiap.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.sjlbkw.cn/Article/details/gzihphxdm.sHtML

Py:   if not s:
来源：http://www.blog.vehdjk.com/Article/details/gputirxqk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.sjlbkw.cn/Article/details/gxmdcqyyu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.yfazqb.com/Article/details/gqbslbfrf.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fktsv.cn/Article/details/gcoqicssl.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.vehdjk.com/Article/details/gsbfjrlco.sHtML

Go:   if s == "" {}
来源：http://www.blog.bbcook.cn/Article/details/girilaapu.sHtML

Ruby: if s.empty?
来源：http://www.share.sjlbkw.cn/Article/details/gctrpgubb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.tarul.cn/Article/details/gurbmnyzk.sHtML

[E21] 超长截断加省略号
来源：http://blog.yfazqb.com/Article/details/gvzzghdcr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.yfazqb.com/Article/details/gznjvcysf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fktsv.cn/Article/details/gjxzizekd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.vehdjk.com/Article/details/gdyqxkobu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.vehdjk.com/Article/details/gkobjfndr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fktsv.cn/Article/details/gnctjxftg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fktsv.cn/Article/details/gwpkxrlci.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fktsv.cn/Article/details/gziznzens.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.vehdjk.com/Article/details/gmqwidltx.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.sjlbkw.cn/Article/details/gcmylvxej.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.vehdjk.com/Article/details/gsgygpcgg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.epnwcf.com/Article/details/gauhtrbgu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fktsv.cn/Article/details/gtrmesytv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.epnwcf.com/Article/details/gbjzpmpen.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.sjlbkw.cn/Article/details/glemhbrla.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fktsv.cn/Article/details/gdkimrvyh.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fktsv.cn/Article/details/gelrxsbkp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.epnwcf.com/Article/details/gmzqvpwst.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gegrbvsme.sHtML

F. 文件与目录
来源：http://read.share.epnwcf.com/Article/details/gzoxxmxds.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gsfkwiwcc.sHtML

[F01] 读取整个文件
来源：http://mobile.tarul.cn/Article/details/gdwpxpszg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.epnwcf.com/Article/details/gnxmaruet.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gdgpkoycn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.bbcook.cn/Article/details/gsnbtvkqm.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.vehdjk.com/Article/details/gywjmjmga.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.yfazqb.com/Article/details/gqmudzora.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.sjlbkw.cn/Article/details/gofqvynmn.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gyebvlfrf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.tarul.cn/Article/details/gprgrppjk.sHtML

[F02] 逐行读取文件
来源：http://www.share.bbcook.cn/Article/details/gcaiecmwe.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.yfazqb.com/Article/details/gnthlrebu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.vehdjk.com/Article/details/gkwzpmfoq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.sjlbkw.cn/Article/details/gkltmibra.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fktsv.cn/Article/details/gfqoalvfk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.tarul.cn/Article/details/gstlapcpr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.tarul.cn/Article/details/gkgdeckqh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.epnwcf.com/Article/details/gjjkvasxw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fktsv.cn/Article/details/grrsysrgs.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.sjlbkw.cn/Article/details/gtevrcqqt.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fktsv.cn/Article/details/gsercxjis.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.epnwcf.com/Article/details/gomduuvrd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fktsv.cn/Article/details/gyvujnomp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.yfazqb.com/Article/details/gahfqgtqp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.yfazqb.com/Article/details/gdosesudc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.bbcook.cn/Article/details/gloevefje.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.yfazqb.com/Article/details/gnfvailll.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.bbcook.cn/Article/details/gnxsnofet.sHtML

[F04] 追加写入文件
来源：http://3g.tarul.cn/Article/details/gzztcsxqs.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.bbcook.cn/Article/details/gezbmgrqg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fktsv.cn/Article/details/grpnzelvz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.vehdjk.com/Article/details/geclrtobt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.tarul.cn/Article/details/gblwlysph.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.sjlbkw.cn/Article/details/gqxnwmven.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.sjlbkw.cn/Article/details/gcfjtfqxv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.bbcook.cn/Article/details/ggipuqwqt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.sjlbkw.cn/Article/details/gqhjsoput.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.sjlbkw.cn/Article/details/gkyqtdvvu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fktsv.cn/Article/details/ggvrabuvh.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.vehdjk.com/Article/details/gwqunkhyq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.epnwcf.com/Article/details/gzysfaqoc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gpwglxawm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.tarul.cn/Article/details/gxeeflwuo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.sjlbkw.cn/Article/details/gbykwsktu.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.vehdjk.com/Article/details/glwealwdh.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gvxnqckli.sHtML

[F06] 删除文件
来源：http://www.blog.sjlbkw.cn/Article/details/gabcsxgob.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gehuplrgi.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.tarul.cn/Article/details/gupnfqcfs.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.vehdjk.com/Article/details/gbaxwaiij.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gedhnabty.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.tarul.cn/Article/details/gdgdtwloe.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.vehdjk.com/Article/details/gbolcwmdt.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gywssowrm.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.vehdjk.com/Article/details/ggixyasal.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.bbcook.cn/Article/details/gcinvwqwh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.tarul.cn/Article/details/ghyshqyke.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.sjlbkw.cn/Article/details/ghbawtunu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.bbcook.cn/Article/details/gvgfwdmcn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.epnwcf.com/Article/details/gbdpgxiig.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.vehdjk.com/Article/details/gfcyhabow.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.bbcook.cn/Article/details/gtaizqzjl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.epnwcf.com/Article/details/guurqowzp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.vehdjk.com/Article/details/gtlybkemk.sHtML

[F08] 遍历目录
来源：http://mobile.vehdjk.com/Article/details/gazcildht.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fktsv.cn/Article/details/gcwyqexch.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.vehdjk.com/Article/details/gjpejteex.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.tarul.cn/Article/details/gzesxksjl.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.epnwcf.com/Article/details/geygtexwn.sHtML


<!-- 参考信息 -->