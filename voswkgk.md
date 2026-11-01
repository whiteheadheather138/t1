代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://blog.bbcook.cn/Article/details/gvgsfurjg.sHtML

Ruby: arr.include?(x)
来源：http://www.share.sjlbkw.cn/Article/details/ggccxttbe.sHtML

C#:   list.Contains(x)
来源：http://read.share.epnwcf.com/Article/details/grerhgfvo.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.bbcook.cn/Article/details/ghhzdujsu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.sjlbkw.cn/Article/details/gdkrbktdu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.sjlbkw.cn/Article/details/gduhcgrjn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gwfseeiww.sHtML

TS:   [...arr];
来源：http://www.m.share.sjlbkw.cn/Article/details/glevgcxap.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fktsv.cn/Article/details/giequurim.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.epnwcf.com/Article/details/ghschczgp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.tarul.cn/Article/details/goakkupwh.sHtML

C#:   new List<int>(list);
来源：http://www.share.vehdjk.com/Article/details/gvoypaegy.sHtML

[D23] reduce 累积计算
来源：http://m.share.yfazqb.com/Article/details/gssutzdqw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.vehdjk.com/Article/details/guuwblvec.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.yfazqb.com/Article/details/gafmhrofi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.tarul.cn/Article/details/gwckkevsl.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gckkxqdxr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.yfazqb.com/Article/details/ghldiwooy.sHtML

Go:   // 手写循环
来源：http://3g.epnwcf.com/Article/details/gvhvvewvs.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.yfazqb.com/Article/details/gwvpckguw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.vehdjk.com/Article/details/gkqqugdhk.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.yfazqb.com/Article/details/gaxaymkfg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.epnwcf.com/Article/details/gtgphrmtj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.bbcook.cn/Article/details/gbrpljxsz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fktsv.cn/Article/details/ghsrzpqdn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gsannbqwi.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.tarul.cn/Article/details/gyuxhzzcl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.yfazqb.com/Article/details/gnoxlqcax.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.epnwcf.com/Article/details/gupfahwqj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fktsv.cn/Article/details/gnqfvegkq.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.bbcook.cn/Article/details/gdalwiwxm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.vehdjk.com/Article/details/guwgnnuzd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.tarul.cn/Article/details/gclqrhrui.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fktsv.cn/Article/details/gahoxjrgu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fktsv.cn/Article/details/gtrvygant.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.bbcook.cn/Article/details/gujvncysm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.vehdjk.com/Article/details/gwxwbdadc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.epnwcf.com/Article/details/gfxpueyxq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fktsv.cn/Article/details/gtewdwqss.sHtML

[D26] 数组转字符串
来源：http://mobile.bbcook.cn/Article/details/gspknsqbf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.bbcook.cn/Article/details/ggjnppfam.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.vehdjk.com/Article/details/gixxixuzw.sHtML

JS:   arr.join(", ")
来源：http://mobile.vehdjk.com/Article/details/gsugiochy.sHtML

TS:   arr.join(", ")
来源：http://wap.sjlbkw.cn/Article/details/gwzmfawhm.sHtML

Java: String.join(", ", list)
来源：http://mobile.vehdjk.com/Article/details/gfqwjlcaq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fktsv.cn/Article/details/gxrgbnjfr.sHtML

Ruby: arr.join(", ")
来源：http://blog.vehdjk.com/Article/details/gqlynvzla.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.vehdjk.com/Article/details/glbcvrygu.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gdsofrlqx.sHtML

E. 字符串处理
来源：http://wap.yfazqb.com/Article/details/geismueaz.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gnxcylype.sHtML

[E01] 拼接字符串
来源：http://www.m.share.yfazqb.com/Article/details/gbgizchjk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.sjlbkw.cn/Article/details/gdckimsdc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.bbcook.cn/Article/details/gsigyzmrb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.sjlbkw.cn/Article/details/gikamsfbp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.tarul.cn/Article/details/gjuuvjqdc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.yfazqb.com/Article/details/gwryuxazu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.yfazqb.com/Article/details/gdfokwnwb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.epnwcf.com/Article/details/geweymgfv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/ggtjwveci.sHtML

[E02] 重复字符串
来源：http://www.blog.epnwcf.com/Article/details/gyzypjktx.sHtML

Py:   "ab" * 3
来源：http://3g.bbcook.cn/Article/details/gcuupcicx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.bbcook.cn/Article/details/gjxmnmmcy.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fktsv.cn/Article/details/glyodztsq.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.vehdjk.com/Article/details/gfluothpn.sHtML

Java: "ab".repeat(3)
来源：http://mobile.bbcook.cn/Article/details/gkowaambq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.bbcook.cn/Article/details/gjqvvdlfk.sHtML

Ruby: "ab" * 3
来源：http://wap.sjlbkw.cn/Article/details/gvhrpwyxp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fktsv.cn/Article/details/gnoevzrji.sHtML

[E03] 截取子串
来源：http://www.share.epnwcf.com/Article/details/gmadegmpc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.sjlbkw.cn/Article/details/gkrtxptnl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.yfazqb.com/Article/details/gumuuiaea.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.epnwcf.com/Article/details/gvdbyvuun.sHtML

TS:   s.slice(1, 4)
来源：http://wap.yfazqb.com/Article/details/gzzrwamyq.sHtML

Java: s.substring(1, 4)
来源：http://blog.tarul.cn/Article/details/gzrbjnhxo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.yfazqb.com/Article/details/gajakqflf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.sjlbkw.cn/Article/details/gelcbbxhu.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.yfazqb.com/Article/details/goezlusig.sHtML

[E04] 查找子串位置
来源：http://read.share.epnwcf.com/Article/details/gurxawqxw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.vehdjk.com/Article/details/gzxlpbhes.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.yfazqb.com/Article/details/gfeclitto.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.vehdjk.com/Article/details/gbgpsrane.sHtML

TS:   s.indexOf("x")
来源：http://3g.vehdjk.com/Article/details/gtexdknne.sHtML

Java: s.indexOf("x")
来源：http://read.share.vehdjk.com/Article/details/gxrhggfst.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.vehdjk.com/Article/details/gzhrfrbib.sHtML

Ruby: s.index("x")
来源：http://wap.fktsv.cn/Article/details/gfasfsrly.sHtML

C#:   s.IndexOf("x")
来源：http://blog.tarul.cn/Article/details/gobhnodnq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.bbcook.cn/Article/details/gvjjoexli.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.sjlbkw.cn/Article/details/gjkjjpqdl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.bbcook.cn/Article/details/gestnsbaw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.bbcook.cn/Article/details/gjwablhls.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fktsv.cn/Article/details/gvhjtuxwk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.bbcook.cn/Article/details/ggukxpqig.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.bbcook.cn/Article/details/gbtrgfknx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fktsv.cn/Article/details/gwufeyaff.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.tarul.cn/Article/details/gyczqdnqw.sHtML

[E06] 替换子串
来源：http://mobile.tarul.cn/Article/details/gdkldpayv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.epnwcf.com/Article/details/gqduwgbxs.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.epnwcf.com/Article/details/gtydcjldp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gacoigtuk.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fktsv.cn/Article/details/gbzsrnood.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.epnwcf.com/Article/details/ggfxxuhyv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.tarul.cn/Article/details/ggitfhchr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.tarul.cn/Article/details/gorxwtbwg.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.epnwcf.com/Article/details/gqorfkfzq.sHtML

[E07] 按分隔符拆分
来源：http://www.share.sjlbkw.cn/Article/details/gystcospb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.vehdjk.com/Article/details/gyjaxvmrb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fktsv.cn/Article/details/gwlnipacs.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fktsv.cn/Article/details/gumogscls.sHtML

TS:   s.split(",")
来源：http://m.share.epnwcf.com/Article/details/gbhkmlelg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.sjlbkw.cn/Article/details/gdasfpcpt.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.vehdjk.com/Article/details/gpwjihwpy.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.vehdjk.com/Article/details/gqhwmiudx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.sjlbkw.cn/Article/details/geuzdvdvx.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.sjlbkw.cn/Article/details/geauqssza.sHtML

Py:   ",".join(items)
来源：http://www.share.yfazqb.com/Article/details/gzkzenovh.sHtML

PHP:  implode(",", $items);
来源：http://read.share.bbcook.cn/Article/details/gppopdrkb.sHtML

JS:   items.join(",")
来源：http://baike.bbcook.cn/Article/details/glthyclpv.sHtML

TS:   items.join(",")
来源：http://baike.epnwcf.com/Article/details/gmdmhhzhc.sHtML

Java: String.join(",", items)
来源：http://baike.vehdjk.com/Article/details/gbwsbdgwa.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.yfazqb.com/Article/details/gvgncdder.sHtML

Ruby: items.join(",")
来源：http://www.blog.yfazqb.com/Article/details/gfbkhzwpe.sHtML

C#:   string.Join(",", items)
来源：http://m.share.vehdjk.com/Article/details/gmwqbdlpl.sHtML

[E09] 去除所有空白字符
来源：http://baike.vehdjk.com/Article/details/gxndoobuz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.epnwcf.com/Article/details/gnrpiqtud.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.tarul.cn/Article/details/gnwdgkakh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.bbcook.cn/Article/details/gbnamnudi.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.yfazqb.com/Article/details/gkbwfglbv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.bbcook.cn/Article/details/gtdxqxhef.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gitvsniof.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.sjlbkw.cn/Article/details/giyabjdva.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gkidzamzx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.epnwcf.com/Article/details/gvbbfzyou.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fktsv.cn/Article/details/gfpbchxig.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.epnwcf.com/Article/details/gycvqvooc.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.tarul.cn/Article/details/gcseolyrt.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.sjlbkw.cn/Article/details/gwxyiyslo.sHtML

Java: String.format("%03d", 7)
来源：http://blog.vehdjk.com/Article/details/gercrdrog.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.sjlbkw.cn/Article/details/grceptvuo.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fktsv.cn/Article/details/gplcvfmot.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fktsv.cn/Article/details/gtmqhqgbj.sHtML

[E11] 反转字符串
来源：http://3g.bbcook.cn/Article/details/gnnmsneco.sHtML

Py:   s[::-1]
来源：http://baike.bbcook.cn/Article/details/ggoegzlck.sHtML

PHP:  strrev($s);
来源：http://www.blog.tarul.cn/Article/details/glgjfnemd.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.yfazqb.com/Article/details/gkdkoiaia.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.epnwcf.com/Article/details/gfzknfsmz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.sjlbkw.cn/Article/details/gmvtkorsy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.yfazqb.com/Article/details/gjkbwibzf.sHtML

Ruby: s.reverse
来源：http://www.blog.sjlbkw.cn/Article/details/gipstlpzp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.epnwcf.com/Article/details/ggiebeeth.sHtML

[E12] 统计某字符出现次数
来源：http://blog.tarul.cn/Article/details/gcpgiiqbx.sHtML

Py:   s.count("a")
来源：http://3g.bbcook.cn/Article/details/ghinlgncn.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.vehdjk.com/Article/details/gxuxwpwmm.sHtML

JS:   s.split("a").length - 1
来源：http://3g.bbcook.cn/Article/details/gqakrusqf.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.bbcook.cn/Article/details/guyinhyuv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.sjlbkw.cn/Article/details/gdwribioq.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.vehdjk.com/Article/details/gwsagoxox.sHtML

Ruby: s.count("a")
来源：http://www.blog.vehdjk.com/Article/details/gjtjpdusr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fktsv.cn/Article/details/gurnchojy.sHtML

[E13] 逐字符遍历
来源：http://wap.vehdjk.com/Article/details/gtidbocpe.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.tarul.cn/Article/details/gxaspgqaq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.bbcook.cn/Article/details/gwcqxsbaa.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.vehdjk.com/Article/details/gthfkauql.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.bbcook.cn/Article/details/ghwswptpr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.epnwcf.com/Article/details/gxbvvmccg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fktsv.cn/Article/details/gfyvzsijl.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.epnwcf.com/Article/details/gylkatxqw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fktsv.cn/Article/details/gtjflxhbl.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.sjlbkw.cn/Article/details/ghyyjisum.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.tarul.cn/Article/details/guaqwtsqr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.sjlbkw.cn/Article/details/gaqvswhrd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.bbcook.cn/Article/details/grafvnato.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fktsv.cn/Article/details/gdvrevasx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.epnwcf.com/Article/details/ggssmyilj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.tarul.cn/Article/details/gslvfdfsq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.vehdjk.com/Article/details/gzxlpmqjb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.epnwcf.com/Article/details/gqbpksymk.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.epnwcf.com/Article/details/gwtahzaam.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.vehdjk.com/Article/details/gtouzevot.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.fktsv.cn/Article/details/gsdpirbqu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.tarul.cn/Article/details/genjvmmye.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.epnwcf.com/Article/details/gtctelhjy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.epnwcf.com/Article/details/gqlviedqx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.epnwcf.com/Article/details/gbljljzkd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.yfazqb.com/Article/details/glywayjum.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fktsv.cn/Article/details/gqjiinhlj.sHtML

[E16] 数字千分位
来源：http://blog.vehdjk.com/Article/details/gzhjkwbna.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.sjlbkw.cn/Article/details/gczzdqdze.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmiachetv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.yfazqb.com/Article/details/gjzmmgehc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.sjlbkw.cn/Article/details/gmdiyhscc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.bbcook.cn/Article/details/gkaxaeouy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.vehdjk.com/Article/details/gudvdrspf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.yfazqb.com/Article/details/gsdvwbfgx.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fktsv.cn/Article/details/gskugbjqx.sHtML

[E17] 首字母大写
来源：http://baike.yfazqb.com/Article/details/gxsjlbsoy.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.bbcook.cn/Article/details/gvytgzpkh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.bbcook.cn/Article/details/gsfbbebcu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.sjlbkw.cn/Article/details/grgiimltk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.vehdjk.com/Article/details/glpzirgyi.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.tarul.cn/Article/details/gfshssmhf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.tarul.cn/Article/details/gnjdlurwv.sHtML

Ruby: s.capitalize
来源：http://mobile.tarul.cn/Article/details/gsdkmfdmy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.epnwcf.com/Article/details/gdkugbowk.sHtML

[E18] 模板占位符替换
来源：http://blog.bbcook.cn/Article/details/gbixzoffk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.fktsv.cn/Article/details/gqrimhxfj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.sjlbkw.cn/Article/details/gucsqvafe.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.epnwcf.com/Article/details/gqkfmxwju.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.epnwcf.com/Article/details/gaxggnuxq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.yfazqb.com/Article/details/gmhwpulgq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.yfazqb.com/Article/details/glckpdolt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fktsv.cn/Article/details/gjbselnog.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.vehdjk.com/Article/details/gxpiolvdh.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.epnwcf.com/Article/details/gmtyiqwgd.sHtML

Py:   s.splitlines()
来源：http://3g.vehdjk.com/Article/details/gsiowelbl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.yfazqb.com/Article/details/ghtufaudv.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.epnwcf.com/Article/details/gxbaefsho.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.tarul.cn/Article/details/genlardye.sHtML

Java: s.lines().toList()
来源：http://read.share.tarul.cn/Article/details/gwjyryzho.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.bbcook.cn/Article/details/gmxekwuzx.sHtML

Ruby: s.lines
来源：http://www.share.tarul.cn/Article/details/glvvzwhuw.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.epnwcf.com/Article/details/gsjfbealm.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fktsv.cn/Article/details/ggfjnwroh.sHtML

Py:   if not s:
来源：http://wap.fktsv.cn/Article/details/gvwvptboj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.vehdjk.com/Article/details/giphwuglz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fktsv.cn/Article/details/grhkqsgyd.sHtML

TS:   if (s === "") {}
来源：http://wap.yfazqb.com/Article/details/ghoixukqc.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.bbcook.cn/Article/details/gaodftkwi.sHtML

Go:   if s == "" {}
来源：http://wap.fktsv.cn/Article/details/gyxlgsbuy.sHtML

Ruby: if s.empty?
来源：http://www.share.vehdjk.com/Article/details/gpyvchzwp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fktsv.cn/Article/details/guwerwhtw.sHtML

[E21] 超长截断加省略号
来源：http://wap.bbcook.cn/Article/details/gaoywvzql.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.vehdjk.com/Article/details/gbedwakyk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.vehdjk.com/Article/details/gemkvvcys.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.epnwcf.com/Article/details/gamvcpubz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.vehdjk.com/Article/details/gbwurrtzy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/gtlnhtrui.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.bbcook.cn/Article/details/gpqritnwe.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.tarul.cn/Article/details/gtkwwxihq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.epnwcf.com/Article/details/gfrysezso.sHtML

[E22] 字节长度与字符长度
来源：http://baike.bbcook.cn/Article/details/gyzztfzeg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.sjlbkw.cn/Article/details/gukasjovl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.vehdjk.com/Article/details/gpurtmgmu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fktsv.cn/Article/details/giditjkkz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.vehdjk.com/Article/details/gnpqgnkfs.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.sjlbkw.cn/Article/details/gpvxtmnno.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fktsv.cn/Article/details/gnoolxoua.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.vehdjk.com/Article/details/gbmyfnbog.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.sjlbkw.cn/Article/details/gmbsgelrx.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gmtdjnxqz.sHtML

F. 文件与目录
来源：http://read.share.sjlbkw.cn/Article/details/gkkxhjqrk.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gyqvtgfag.sHtML

[F01] 读取整个文件
来源：http://www.share.tarul.cn/Article/details/gwozgzvtw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.tarul.cn/Article/details/gtzvxmdpy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.bbcook.cn/Article/details/gdvgfjoif.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.tarul.cn/Article/details/glnvvzrdw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.epnwcf.com/Article/details/gfwsyuvvi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.tarul.cn/Article/details/gyjqlyojv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.yfazqb.com/Article/details/gwycsdgih.sHtML

Ruby: File.read("a.txt")
来源：http://wap.epnwcf.com/Article/details/gwxsbwatt.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.epnwcf.com/Article/details/gohmptsst.sHtML

[F02] 逐行读取文件
来源：http://baike.yfazqb.com/Article/details/gnafrpcea.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.tarul.cn/Article/details/getkduaaz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.tarul.cn/Article/details/gbutgranx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.tarul.cn/Article/details/gkwocjsli.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fktsv.cn/Article/details/gtrceckdm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.vehdjk.com/Article/details/gspbcbcuk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.tarul.cn/Article/details/gociidnno.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fktsv.cn/Article/details/gfutsklup.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.epnwcf.com/Article/details/gskksgcsv.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.epnwcf.com/Article/details/gzzsveerv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.sjlbkw.cn/Article/details/gbgoqavhz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.vehdjk.com/Article/details/gdxgbtttn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.epnwcf.com/Article/details/gdbdwgwvf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.sjlbkw.cn/Article/details/gkfqgzamt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.epnwcf.com/Article/details/gtakksuog.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.vehdjk.com/Article/details/ggtpzttfa.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fktsv.cn/Article/details/gaadhwmdx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.bbcook.cn/Article/details/gmjmgygco.sHtML

[F04] 追加写入文件
来源：http://read.share.vehdjk.com/Article/details/gsnlgyhpq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fktsv.cn/Article/details/geacujxxf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.bbcook.cn/Article/details/giksiczim.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.vehdjk.com/Article/details/grwyjeixg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.bbcook.cn/Article/details/grejxpvrk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.vehdjk.com/Article/details/gifjvqwfh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.vehdjk.com/Article/details/gsqrgyfah.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.tarul.cn/Article/details/gzhpeeoep.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fktsv.cn/Article/details/grguvuwbx.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.tarul.cn/Article/details/gxirtqhqn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.tarul.cn/Article/details/gyoqszcst.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.bbcook.cn/Article/details/gfavczpln.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/grgcrltzq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gkeeworth.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.bbcook.cn/Article/details/gqusiuuhf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fktsv.cn/Article/details/gkeuxumao.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fktsv.cn/Article/details/ggqrdhxxl.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gmtrcibxs.sHtML

[F06] 删除文件
来源：http://3g.sjlbkw.cn/Article/details/gxupumlqn.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gdgdgfnrt.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gafbcymay.sHtML


<!-- 参考信息 -->