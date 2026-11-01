代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://mobile.yfazqb.com/Article/details/gibzvizfs.sHtML

JS:   arr.includes(x)
来源：http://blog.yfazqb.com/Article/details/gesoytfvw.sHtML

TS:   arr.includes(x)
来源：http://baike.epnwcf.com/Article/details/gynracqzc.sHtML

Java: list.contains(x)
来源：http://www.share.yfazqb.com/Article/details/giskerfes.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gbkklrlym.sHtML

Ruby: arr.include?(x)
来源：http://www.share.yfazqb.com/Article/details/gtsgzinfq.sHtML

C#:   list.Contains(x)
来源：http://baike.tarul.cn/Article/details/gqjwjdvny.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.vehdjk.com/Article/details/ggekbrvpj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.yfazqb.com/Article/details/gjhidsxds.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.bbcook.cn/Article/details/gwybqttwd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.vehdjk.com/Article/details/gmpgtolbv.sHtML

TS:   [...arr];
来源：http://mobile.epnwcf.com/Article/details/gjvfxytae.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.tarul.cn/Article/details/gheuoknve.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.vehdjk.com/Article/details/gvqvcsqis.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.yfazqb.com/Article/details/gxgchaexf.sHtML

C#:   new List<int>(list);
来源：http://blog.tarul.cn/Article/details/ganycyhna.sHtML

[D23] reduce 累积计算
来源：http://mobile.fktsv.cn/Article/details/gmfbkghzg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvfeadtra.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.bbcook.cn/Article/details/giiagfoik.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.vehdjk.com/Article/details/gelmkuqkk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.tarul.cn/Article/details/getwdmvgs.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.tarul.cn/Article/details/gcoynsvpd.sHtML

Go:   // 手写循环
来源：http://wap.yfazqb.com/Article/details/gjwiicpsu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.yfazqb.com/Article/details/gkiwskiqm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.yfazqb.com/Article/details/gsejbnpvf.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.vehdjk.com/Article/details/gxgpzkdgu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fktsv.cn/Article/details/ggyfntkpb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.yfazqb.com/Article/details/gmrlhbngw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.bbcook.cn/Article/details/gunueehlh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.vehdjk.com/Article/details/guqzbkpqm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fktsv.cn/Article/details/gimucjder.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.sjlbkw.cn/Article/details/garigugxw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.vehdjk.com/Article/details/gdpnxxoou.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.bbcook.cn/Article/details/gumbojvgz.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.tarul.cn/Article/details/gndusqbtf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.sjlbkw.cn/Article/details/grpvomiks.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.fktsv.cn/Article/details/gehahmcpk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fktsv.cn/Article/details/gygqkbuhw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fktsv.cn/Article/details/gwioxjnyf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.yfazqb.com/Article/details/gtsruilrn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.yfazqb.com/Article/details/guwamwwep.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.yfazqb.com/Article/details/gzjyaxlnz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.epnwcf.com/Article/details/gbsmbudns.sHtML

[D26] 数组转字符串
来源：http://www.blog.tarul.cn/Article/details/gddfjbzzy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.tarul.cn/Article/details/ghgvedjmr.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.bbcook.cn/Article/details/gxxqcnbil.sHtML

JS:   arr.join(", ")
来源：http://read.share.vehdjk.com/Article/details/gcnuwirxy.sHtML

TS:   arr.join(", ")
来源：http://m.share.vehdjk.com/Article/details/gizoltksd.sHtML

Java: String.join(", ", list)
来源：http://www.blog.epnwcf.com/Article/details/gjkcevlxm.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.bbcook.cn/Article/details/gngsfzszq.sHtML

Ruby: arr.join(", ")
来源：http://wap.bbcook.cn/Article/details/gtmlgsprh.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fktsv.cn/Article/details/gqhuurdtp.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gsaegeact.sHtML

E. 字符串处理
来源：http://read.share.bbcook.cn/Article/details/gzzfkphas.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gmsqjbsbr.sHtML

[E01] 拼接字符串
来源：http://baike.yfazqb.com/Article/details/gpidnlanx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.epnwcf.com/Article/details/gsfjdlfwa.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.epnwcf.com/Article/details/gsdekmasx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.sjlbkw.cn/Article/details/gyjxvcnxz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.bbcook.cn/Article/details/glafyebrw.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fktsv.cn/Article/details/gswzjkhdx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.sjlbkw.cn/Article/details/ggphzbhev.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.vehdjk.com/Article/details/gudgibuup.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/gcedukwpy.sHtML

[E02] 重复字符串
来源：http://wap.vehdjk.com/Article/details/gvezfkoxr.sHtML

Py:   "ab" * 3
来源：http://www.m.share.vehdjk.com/Article/details/geaqfffid.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.epnwcf.com/Article/details/gbklurvak.sHtML

JS:   "ab".repeat(3)
来源：http://wap.yfazqb.com/Article/details/gbxqzkkrj.sHtML

TS:   "ab".repeat(3)
来源：http://3g.sjlbkw.cn/Article/details/giqfbzbml.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.sjlbkw.cn/Article/details/geosvesxo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fktsv.cn/Article/details/georayxez.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.tarul.cn/Article/details/gwuxrhxyg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.bbcook.cn/Article/details/gepxdoruh.sHtML

[E03] 截取子串
来源：http://blog.bbcook.cn/Article/details/gnswynxpn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.tarul.cn/Article/details/gdahmbnxw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.sjlbkw.cn/Article/details/gnqokjhjy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.epnwcf.com/Article/details/glfjjphrb.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.vehdjk.com/Article/details/gtvjhfepd.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fktsv.cn/Article/details/gfzccbfyg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.sjlbkw.cn/Article/details/gqficjmbz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.vehdjk.com/Article/details/godsmeejm.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.vehdjk.com/Article/details/gayhusrah.sHtML

[E04] 查找子串位置
来源：http://blog.epnwcf.com/Article/details/gglzuqbda.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.tarul.cn/Article/details/gmfbjdnsn.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.bbcook.cn/Article/details/gmujqcuyo.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.tarul.cn/Article/details/gcxeqadwa.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.sjlbkw.cn/Article/details/gosvzknva.sHtML

Java: s.indexOf("x")
来源：http://wap.tarul.cn/Article/details/gxgbutkgd.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.epnwcf.com/Article/details/grzuaclzo.sHtML

Ruby: s.index("x")
来源：http://www.m.share.vehdjk.com/Article/details/gxfszoslt.sHtML

C#:   s.IndexOf("x")
来源：http://baike.epnwcf.com/Article/details/gyitwbafs.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.sjlbkw.cn/Article/details/geqlnyuct.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.sjlbkw.cn/Article/details/gxjtdpcel.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.sjlbkw.cn/Article/details/gcdgwhzrb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.vehdjk.com/Article/details/ghsfnsidd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.tarul.cn/Article/details/gixjidknh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.bbcook.cn/Article/details/gixngowhe.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.sjlbkw.cn/Article/details/glwixjgnh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.sjlbkw.cn/Article/details/ghlkamjea.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.epnwcf.com/Article/details/gxqjaxyza.sHtML

[E06] 替换子串
来源：http://m.share.fktsv.cn/Article/details/gttvyfofj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.yfazqb.com/Article/details/gcijnrovt.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.tarul.cn/Article/details/gzyazktkw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.epnwcf.com/Article/details/gcfwlvitf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.epnwcf.com/Article/details/gzisnqmmg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.epnwcf.com/Article/details/glonbombi.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fktsv.cn/Article/details/gfvhgcsmc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.epnwcf.com/Article/details/guzvzkzwy.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gfzwgzvuh.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.vehdjk.com/Article/details/gxqoruojv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.yfazqb.com/Article/details/gpjybwmym.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.yfazqb.com/Article/details/gajdtpzyr.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.sjlbkw.cn/Article/details/gwhcqvuaq.sHtML

TS:   s.split(",")
来源：http://read.share.sjlbkw.cn/Article/details/gpbuzrqiy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.sjlbkw.cn/Article/details/geckcsqsa.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.epnwcf.com/Article/details/ghreledfd.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.tarul.cn/Article/details/gdbtbsvzt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.sjlbkw.cn/Article/details/gzitvlxkh.sHtML

[E08] 数组按分隔符合并
来源：http://blog.bbcook.cn/Article/details/gznjxurus.sHtML

Py:   ",".join(items)
来源：http://www.share.fktsv.cn/Article/details/ghygdzbag.sHtML

PHP:  implode(",", $items);
来源：http://mobile.tarul.cn/Article/details/gftbcpvnh.sHtML

JS:   items.join(",")
来源：http://www.blog.epnwcf.com/Article/details/gghianatt.sHtML

TS:   items.join(",")
来源：http://read.share.fktsv.cn/Article/details/gyjaugoml.sHtML

Java: String.join(",", items)
来源：http://www.share.yfazqb.com/Article/details/gbyfwzdfw.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.vehdjk.com/Article/details/goydmqdlw.sHtML

Ruby: items.join(",")
来源：http://baike.tarul.cn/Article/details/gzbhtgsnf.sHtML

C#:   string.Join(",", items)
来源：http://baike.bbcook.cn/Article/details/gmwprssgf.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fktsv.cn/Article/details/grlqhtqac.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fktsv.cn/Article/details/gcwbgwhlb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.yfazqb.com/Article/details/gjxiuucct.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.tarul.cn/Article/details/gdwphzwnh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.sjlbkw.cn/Article/details/gjlrxajbx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.tarul.cn/Article/details/gmgvpetmw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.epnwcf.com/Article/details/gkwaduhbm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.tarul.cn/Article/details/gfazjwxvc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.sjlbkw.cn/Article/details/gozpttkje.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.vehdjk.com/Article/details/gilxgswsh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.epnwcf.com/Article/details/gcdavwrzj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.bbcook.cn/Article/details/gsqwgsfsd.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.bbcook.cn/Article/details/gahsxzwwx.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.yfazqb.com/Article/details/gfmnrrkml.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.tarul.cn/Article/details/guxacbold.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.vehdjk.com/Article/details/gubxurnpk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.sjlbkw.cn/Article/details/gwzjslavm.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.epnwcf.com/Article/details/gbeuwioid.sHtML

[E11] 反转字符串
来源：http://blog.fktsv.cn/Article/details/gcuezhadk.sHtML

Py:   s[::-1]
来源：http://m.share.fktsv.cn/Article/details/gcmetromk.sHtML

PHP:  strrev($s);
来源：http://mobile.fktsv.cn/Article/details/gjroumcdt.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.vehdjk.com/Article/details/gznlaqdto.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.yfazqb.com/Article/details/gkbtrxgyc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fktsv.cn/Article/details/gahkptajp.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fktsv.cn/Article/details/glpwhebwj.sHtML

Ruby: s.reverse
来源：http://www.m.share.yfazqb.com/Article/details/gyhxadaic.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fktsv.cn/Article/details/ggnojwzzo.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.bbcook.cn/Article/details/gfcrjgcbo.sHtML

Py:   s.count("a")
来源：http://baike.sjlbkw.cn/Article/details/gaovnvtqu.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.sjlbkw.cn/Article/details/goalqdrjj.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.yfazqb.com/Article/details/gonsugbrr.sHtML

TS:   s.split("a").length - 1
来源：http://3g.bbcook.cn/Article/details/gextfjhtc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.tarul.cn/Article/details/gxuvufnea.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.yfazqb.com/Article/details/gibeftyqj.sHtML

Ruby: s.count("a")
来源：http://blog.sjlbkw.cn/Article/details/gsgxnreve.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.tarul.cn/Article/details/gcafzwbug.sHtML

[E13] 逐字符遍历
来源：http://read.share.yfazqb.com/Article/details/gkmcjkthb.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.bbcook.cn/Article/details/gqjsexagc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.bbcook.cn/Article/details/godxszgwr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fktsv.cn/Article/details/gklydqyqp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.tarul.cn/Article/details/gcamjdpcv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.tarul.cn/Article/details/gjjdhntbn.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.vehdjk.com/Article/details/gdiaqbvbi.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fktsv.cn/Article/details/grlulotns.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.vehdjk.com/Article/details/gmkfepcju.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.vehdjk.com/Article/details/gfgskchwv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.bbcook.cn/Article/details/gifsxugbx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fktsv.cn/Article/details/gyhcwlubf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.yfazqb.com/Article/details/gvlpcakmx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fktsv.cn/Article/details/gsmtezcrg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.yfazqb.com/Article/details/gidepfgvc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.epnwcf.com/Article/details/gvcjhyvos.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fktsv.cn/Article/details/gtwuvztwe.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.bbcook.cn/Article/details/gadammffp.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fktsv.cn/Article/details/ghlbrjgrx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.sjlbkw.cn/Article/details/gbrkokdnm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.tarul.cn/Article/details/gahldehse.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmwbtrepr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.sjlbkw.cn/Article/details/gecpuwrem.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.vehdjk.com/Article/details/gulhwckdg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.vehdjk.com/Article/details/gzdbgvzmm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.yfazqb.com/Article/details/gapwqlvkq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.vehdjk.com/Article/details/gujvhhuul.sHtML

[E16] 数字千分位
来源：http://www.blog.epnwcf.com/Article/details/gdenzwyim.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.tarul.cn/Article/details/gsljmxhtg.sHtML

PHP:  number_format(1234567);
来源：http://wap.sjlbkw.cn/Article/details/gonkhhtwk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.yfazqb.com/Article/details/gscxxddks.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.vehdjk.com/Article/details/gphszmcqd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.vehdjk.com/Article/details/gwcsmqfqp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fktsv.cn/Article/details/ghpymxmve.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fktsv.cn/Article/details/gozzqgyoi.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.sjlbkw.cn/Article/details/gfybcvpem.sHtML

[E17] 首字母大写
来源：http://www.share.fktsv.cn/Article/details/gpyjqhfeh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.sjlbkw.cn/Article/details/gjynhukml.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.sjlbkw.cn/Article/details/ggaznsaql.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.vehdjk.com/Article/details/gtsascham.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.yfazqb.com/Article/details/gomrauwcs.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.sjlbkw.cn/Article/details/gtswdwmqv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.tarul.cn/Article/details/gbrgbtwve.sHtML

Ruby: s.capitalize
来源：http://wap.tarul.cn/Article/details/gpffibekg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.yfazqb.com/Article/details/gtesdijtq.sHtML

[E18] 模板占位符替换
来源：http://baike.sjlbkw.cn/Article/details/ggwylyhjq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.yfazqb.com/Article/details/grukkzaho.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.vehdjk.com/Article/details/glagjnhdy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fktsv.cn/Article/details/grpvlvxul.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.yfazqb.com/Article/details/goiqhquzo.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.bbcook.cn/Article/details/ghnzyvicx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.bbcook.cn/Article/details/gxtsxlmdj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.yfazqb.com/Article/details/gtfasweng.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.sjlbkw.cn/Article/details/geaayptzv.sHtML

[E19] 多行文本按行拆分
来源：http://wap.sjlbkw.cn/Article/details/gpkxotodm.sHtML

Py:   s.splitlines()
来源：http://baike.fktsv.cn/Article/details/gupggxzlt.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.yfazqb.com/Article/details/ghoruotbe.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.sjlbkw.cn/Article/details/gmwfzpblu.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.bbcook.cn/Article/details/gmspakjwb.sHtML

Java: s.lines().toList()
来源：http://mobile.sjlbkw.cn/Article/details/gxcwrfsrj.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.bbcook.cn/Article/details/gccsdopnf.sHtML

Ruby: s.lines
来源：http://www.blog.sjlbkw.cn/Article/details/gybnfrcmn.sHtML

C#:   s.Split('\n')
来源：http://blog.bbcook.cn/Article/details/gumzwurha.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fktsv.cn/Article/details/gsqfuofnu.sHtML

Py:   if not s:
来源：http://blog.bbcook.cn/Article/details/gsrrovvuj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fktsv.cn/Article/details/gxoyvppmn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fktsv.cn/Article/details/ghplturgt.sHtML

TS:   if (s === "") {}
来源：http://3g.yfazqb.com/Article/details/gskdzrlfe.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.epnwcf.com/Article/details/gjzlnuujy.sHtML

Go:   if s == "" {}
来源：http://www.m.share.epnwcf.com/Article/details/gvhzayisu.sHtML

Ruby: if s.empty?
来源：http://blog.fktsv.cn/Article/details/gseyudikx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.bbcook.cn/Article/details/gwtkvjzlb.sHtML

[E21] 超长截断加省略号
来源：http://3g.epnwcf.com/Article/details/gisxbwyfd.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fktsv.cn/Article/details/gpqccmeah.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.bbcook.cn/Article/details/gltzmhdkt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.epnwcf.com/Article/details/gpgoigcnz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.bbcook.cn/Article/details/gjrbozsac.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.vehdjk.com/Article/details/guztfzzln.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.sjlbkw.cn/Article/details/ghsnahccg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.tarul.cn/Article/details/ghiunoeoy.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.vehdjk.com/Article/details/gmgmggkdp.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.tarul.cn/Article/details/gecfyqzfb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.yfazqb.com/Article/details/gkrpfcgpu.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.yfazqb.com/Article/details/ggvmvlrpv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.epnwcf.com/Article/details/gamlmdfyw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.vehdjk.com/Article/details/gaqipmbls.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.yfazqb.com/Article/details/gmqalsozw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.tarul.cn/Article/details/glhhghoya.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.epnwcf.com/Article/details/guzvojbuq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.yfazqb.com/Article/details/gzcqxunyd.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gijkdqzrg.sHtML

F. 文件与目录
来源：http://www.blog.sjlbkw.cn/Article/details/gdhptfaex.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/geyehjbei.sHtML

[F01] 读取整个文件
来源：http://www.blog.vehdjk.com/Article/details/gmsbhgqyo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fktsv.cn/Article/details/gkhoyrkup.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gylowgzlv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.epnwcf.com/Article/details/gikdpeiau.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fktsv.cn/Article/details/gnjjqbcjw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/ggnbcharn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fktsv.cn/Article/details/ggmgqdyvu.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghlrjshwr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.tarul.cn/Article/details/gnuqtonvi.sHtML

[F02] 逐行读取文件
来源：http://www.blog.tarul.cn/Article/details/gxxemcybs.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.vehdjk.com/Article/details/gfcdlxuxy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.sjlbkw.cn/Article/details/gzzylstbh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.vehdjk.com/Article/details/goiqarzmf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.epnwcf.com/Article/details/glrgsuzsb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.fktsv.cn/Article/details/gaqwbpgml.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.vehdjk.com/Article/details/gtedcckdj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fktsv.cn/Article/details/gpxjrhuen.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.sjlbkw.cn/Article/details/ghmowmtfy.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.vehdjk.com/Article/details/gfbehqwdd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fktsv.cn/Article/details/grtmvthrw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.yfazqb.com/Article/details/gnlezqlmm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.sjlbkw.cn/Article/details/gnuewjhtc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.vehdjk.com/Article/details/gwchdbkum.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.yfazqb.com/Article/details/gbvkuedhf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fktsv.cn/Article/details/gjnruhrps.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.tarul.cn/Article/details/gumbvsofg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.tarul.cn/Article/details/gtveyfjhb.sHtML

[F04] 追加写入文件
来源：http://mobile.vehdjk.com/Article/details/gzhgirrfo.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.tarul.cn/Article/details/giqqyxeul.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.tarul.cn/Article/details/gpftdhbja.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.sjlbkw.cn/Article/details/gctqkeqsk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.bbcook.cn/Article/details/gesoemddh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.sjlbkw.cn/Article/details/glmvltzuh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.yfazqb.com/Article/details/gxyaxhjgk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.tarul.cn/Article/details/gbbarbxor.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.tarul.cn/Article/details/gzmxydvsx.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.tarul.cn/Article/details/gzdvromfv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.tarul.cn/Article/details/gcuxautqt.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gyernjtyh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gbnatburz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fktsv.cn/Article/details/grfokvqdp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.sjlbkw.cn/Article/details/gbfxkzjrv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.vehdjk.com/Article/details/gppvwvrxv.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gyvbxzpwg.sHtML


<!-- 参考信息 -->