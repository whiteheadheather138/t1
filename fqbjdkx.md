代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://baike.yfazqb.com/Article/details/garflgtia.sHtML

Ruby: arr.include?(x)
来源：http://3g.epnwcf.com/Article/details/gaaacztfp.sHtML

C#:   list.Contains(x)
来源：http://read.share.sjlbkw.cn/Article/details/gtcusfynj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.fktsv.cn/Article/details/gwwyhhngc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gpzfkuuee.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.vehdjk.com/Article/details/grxkhvksm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.epnwcf.com/Article/details/gcwsqmkki.sHtML

TS:   [...arr];
来源：http://3g.bbcook.cn/Article/details/gozyhwmxa.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.bbcook.cn/Article/details/gfdhenjxn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.tarul.cn/Article/details/glpvihmkf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.epnwcf.com/Article/details/ghkptkdnu.sHtML

C#:   new List<int>(list);
来源：http://blog.epnwcf.com/Article/details/gleqcawpn.sHtML

[D23] reduce 累积计算
来源：http://www.blog.vehdjk.com/Article/details/gutkbhfrt.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.epnwcf.com/Article/details/gbluolcsr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fktsv.cn/Article/details/gpubzyiwg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.epnwcf.com/Article/details/ggwpeuibp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.bbcook.cn/Article/details/gvclherpy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.bbcook.cn/Article/details/giufqiuom.sHtML

Go:   // 手写循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gbflxpwtv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.sjlbkw.cn/Article/details/gyuhwoofn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.yfazqb.com/Article/details/gserrwyrk.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.tarul.cn/Article/details/glmyagdkz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.tarul.cn/Article/details/guloyzsrn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.yfazqb.com/Article/details/gtexqthwg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fktsv.cn/Article/details/gqickgnyt.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.tarul.cn/Article/details/ggzilfcyp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.sjlbkw.cn/Article/details/gqxcrkzwj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fktsv.cn/Article/details/gkuuzhlkv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.epnwcf.com/Article/details/gkmvlpbvn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.vehdjk.com/Article/details/gpfbwaavm.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.epnwcf.com/Article/details/gscfgeyig.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fktsv.cn/Article/details/gzfjiaofg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.tarul.cn/Article/details/gpyykxolk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.yfazqb.com/Article/details/gxvhqyaoj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.vehdjk.com/Article/details/gzudeiiyk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.vehdjk.com/Article/details/gcdnzcojl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.yfazqb.com/Article/details/gnpgqhddk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.vehdjk.com/Article/details/gxbuuevtp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.vehdjk.com/Article/details/gnoaxgana.sHtML

[D26] 数组转字符串
来源：http://3g.bbcook.cn/Article/details/gsnojmjzk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fktsv.cn/Article/details/gbhknkmnr.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.tarul.cn/Article/details/gtjyeiqkv.sHtML

JS:   arr.join(", ")
来源：http://3g.vehdjk.com/Article/details/gvlidbqcj.sHtML

TS:   arr.join(", ")
来源：http://mobile.yfazqb.com/Article/details/gyzzvknin.sHtML

Java: String.join(", ", list)
来源：http://m.share.yfazqb.com/Article/details/gfarmhtnd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fktsv.cn/Article/details/gpdemrfks.sHtML

Ruby: arr.join(", ")
来源：http://wap.bbcook.cn/Article/details/gqgxqazte.sHtML

C#:   string.Join(", ", list)
来源：http://blog.yfazqb.com/Article/details/glaweynkf.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gbyyaueat.sHtML

E. 字符串处理
来源：http://m.share.tarul.cn/Article/details/gxareykpd.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gxzxoxfzt.sHtML

[E01] 拼接字符串
来源：http://read.share.epnwcf.com/Article/details/gjlqdpdqi.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.sjlbkw.cn/Article/details/gnfcmirpn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fktsv.cn/Article/details/gvlkmlvxg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.sjlbkw.cn/Article/details/gsssxhjlr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fktsv.cn/Article/details/gordpyhzr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.epnwcf.com/Article/details/gkyusqlaz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.sjlbkw.cn/Article/details/gnamyfxhd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fktsv.cn/Article/details/gsorbwnoh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/grwffmjdh.sHtML

[E02] 重复字符串
来源：http://mobile.yfazqb.com/Article/details/ghacvwcsb.sHtML

Py:   "ab" * 3
来源：http://3g.epnwcf.com/Article/details/gvatyryqg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.tarul.cn/Article/details/gcerqzuwy.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fktsv.cn/Article/details/ghetlzqzb.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fktsv.cn/Article/details/gosdximye.sHtML

Java: "ab".repeat(3)
来源：http://blog.vehdjk.com/Article/details/ggenwxraf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.epnwcf.com/Article/details/gmmfzxisy.sHtML

Ruby: "ab" * 3
来源：http://m.share.sjlbkw.cn/Article/details/ggulfofhp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.yfazqb.com/Article/details/gesxaxjht.sHtML

[E03] 截取子串
来源：http://blog.fktsv.cn/Article/details/gcmgkxuob.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.bbcook.cn/Article/details/gllphmiwe.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.vehdjk.com/Article/details/giurroyzh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fktsv.cn/Article/details/gcmppuudl.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.bbcook.cn/Article/details/glpildaqv.sHtML

Java: s.substring(1, 4)
来源：http://m.share.sjlbkw.cn/Article/details/gecbhrwov.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.tarul.cn/Article/details/gakdftyue.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.epnwcf.com/Article/details/grwhaxeym.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.tarul.cn/Article/details/gtivlzsnf.sHtML

[E04] 查找子串位置
来源：http://mobile.tarul.cn/Article/details/gwasfowov.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.tarul.cn/Article/details/gzqaxzvha.sHtML

PHP:  strpos($s, "x");
来源：http://wap.vehdjk.com/Article/details/ggqiqfxyq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.yfazqb.com/Article/details/ghugvxsum.sHtML

TS:   s.indexOf("x")
来源：http://baike.tarul.cn/Article/details/gauslwumz.sHtML

Java: s.indexOf("x")
来源：http://www.share.bbcook.cn/Article/details/gindsfdxc.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.fktsv.cn/Article/details/gsfyxpajl.sHtML

Ruby: s.index("x")
来源：http://www.blog.bbcook.cn/Article/details/glzdghxwt.sHtML

C#:   s.IndexOf("x")
来源：http://wap.tarul.cn/Article/details/gkewirlzk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.epnwcf.com/Article/details/gldpxfsrn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.vehdjk.com/Article/details/gpqpewdox.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.sjlbkw.cn/Article/details/gvepstqvh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.sjlbkw.cn/Article/details/gtotlkmsp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.sjlbkw.cn/Article/details/gdrerelnu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.vehdjk.com/Article/details/goqnusrgq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.sjlbkw.cn/Article/details/gkmaesxbz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.tarul.cn/Article/details/gkjsslvhl.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.yfazqb.com/Article/details/gzajgvjvz.sHtML

[E06] 替换子串
来源：http://blog.sjlbkw.cn/Article/details/geguybvyo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.bbcook.cn/Article/details/gjgtolyhz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.bbcook.cn/Article/details/gyjafgayt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.tarul.cn/Article/details/gkazuuqqr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/ggnvfxssj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.bbcook.cn/Article/details/gjdbzkzfg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.vehdjk.com/Article/details/gaenhvctw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fktsv.cn/Article/details/gfphkhyfq.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gxjphpiap.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fktsv.cn/Article/details/gwhmwcfvn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.vehdjk.com/Article/details/gycozjzic.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.vehdjk.com/Article/details/gipevokcn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.epnwcf.com/Article/details/gpqlgxhwm.sHtML

TS:   s.split(",")
来源：http://blog.bbcook.cn/Article/details/gnhfzbmsv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.yfazqb.com/Article/details/gjetdpuro.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsotxbaam.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.bbcook.cn/Article/details/gyffxigvt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.tarul.cn/Article/details/gdwigneev.sHtML

[E08] 数组按分隔符合并
来源：http://baike.sjlbkw.cn/Article/details/gzvdjkeup.sHtML

Py:   ",".join(items)
来源：http://baike.yfazqb.com/Article/details/gshtnhfic.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fktsv.cn/Article/details/glxjemych.sHtML

JS:   items.join(",")
来源：http://wap.bbcook.cn/Article/details/gscjipjhb.sHtML

TS:   items.join(",")
来源：http://www.blog.vehdjk.com/Article/details/gjqfuosyn.sHtML

Java: String.join(",", items)
来源：http://baike.bbcook.cn/Article/details/gsylhslxm.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.tarul.cn/Article/details/ghnohfyas.sHtML

Ruby: items.join(",")
来源：http://wap.fktsv.cn/Article/details/gbfvziorq.sHtML

C#:   string.Join(",", items)
来源：http://3g.epnwcf.com/Article/details/gfxkwjpmp.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.epnwcf.com/Article/details/gdwsublxn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.sjlbkw.cn/Article/details/glnvqvusq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.bbcook.cn/Article/details/gadntfsqk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.tarul.cn/Article/details/gmebboiyi.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.bbcook.cn/Article/details/gwbzzovml.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.bbcook.cn/Article/details/ggmerzncq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.bbcook.cn/Article/details/gqvywbphp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.bbcook.cn/Article/details/gijzmklyy.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fktsv.cn/Article/details/gcuvnbwae.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.epnwcf.com/Article/details/gtfjrolci.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.yfazqb.com/Article/details/gdotluvcg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.vehdjk.com/Article/details/gcqibqfgc.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.yfazqb.com/Article/details/gptxkqajp.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.bbcook.cn/Article/details/guehnromc.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.tarul.cn/Article/details/gjpuzjjkc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.sjlbkw.cn/Article/details/gsnccokkd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.vehdjk.com/Article/details/gjeowrrgk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.yfazqb.com/Article/details/gmlxsxvbs.sHtML

[E11] 反转字符串
来源：http://m.share.bbcook.cn/Article/details/gbhtznbir.sHtML

Py:   s[::-1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gyofxaabc.sHtML

PHP:  strrev($s);
来源：http://mobile.yfazqb.com/Article/details/gifihaitz.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.sjlbkw.cn/Article/details/ggtieykxz.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.epnwcf.com/Article/details/gymzipdqo.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.yfazqb.com/Article/details/gmqcplzns.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fktsv.cn/Article/details/gacfxyefn.sHtML

Ruby: s.reverse
来源：http://baike.fktsv.cn/Article/details/gdipxfzto.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.bbcook.cn/Article/details/ggvwkpjjv.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.tarul.cn/Article/details/guhzxqdes.sHtML

Py:   s.count("a")
来源：http://www.blog.sjlbkw.cn/Article/details/gkbhjopqo.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.tarul.cn/Article/details/guvszykyg.sHtML

JS:   s.split("a").length - 1
来源：http://3g.tarul.cn/Article/details/gcwcctslr.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.sjlbkw.cn/Article/details/ggwxojmbn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fktsv.cn/Article/details/gflavvlvh.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fktsv.cn/Article/details/grydkynzm.sHtML

Ruby: s.count("a")
来源：http://www.blog.yfazqb.com/Article/details/gswdkgyaj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.sjlbkw.cn/Article/details/gosvuqajq.sHtML

[E13] 逐字符遍历
来源：http://m.share.bbcook.cn/Article/details/gouevxcol.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.sjlbkw.cn/Article/details/glljwtdqv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.yfazqb.com/Article/details/gfdhdjzrc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.sjlbkw.cn/Article/details/glibcdfht.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.yfazqb.com/Article/details/gobdxjqjn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fktsv.cn/Article/details/gwfiiwsjx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.bbcook.cn/Article/details/ggjvaqdip.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.bbcook.cn/Article/details/gauangieq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.bbcook.cn/Article/details/gxlnsxvmu.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.sjlbkw.cn/Article/details/gfjdnfoyi.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.sjlbkw.cn/Article/details/gzvozsqwm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.tarul.cn/Article/details/gmszrtdid.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.yfazqb.com/Article/details/gwgubdjdo.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.vehdjk.com/Article/details/ghaumafvv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.vehdjk.com/Article/details/gbrkturxf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fktsv.cn/Article/details/ghbdldrdx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.tarul.cn/Article/details/gfyixpous.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.bbcook.cn/Article/details/gmumcqwhs.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.vehdjk.com/Article/details/gigmeslzl.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.bbcook.cn/Article/details/ghoyowobo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.bbcook.cn/Article/details/geslnwueq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.sjlbkw.cn/Article/details/gxjetlrcc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fktsv.cn/Article/details/geevypnmu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.bbcook.cn/Article/details/gxodggwxs.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.bbcook.cn/Article/details/gqnuwhfdg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpqsypwld.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.bbcook.cn/Article/details/gyzkqkbtn.sHtML

[E16] 数字千分位
来源：http://baike.vehdjk.com/Article/details/gmyxrvlyg.sHtML

Py:   f"{1234567:,}"
来源：http://wap.bbcook.cn/Article/details/ggraxgqyi.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.sjlbkw.cn/Article/details/gteusrmwv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.tarul.cn/Article/details/gmbmxpllj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.yfazqb.com/Article/details/gbohozmtq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.sjlbkw.cn/Article/details/gofttugxj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.bbcook.cn/Article/details/gneqdhayg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.epnwcf.com/Article/details/gpfcxttta.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.bbcook.cn/Article/details/gpjftlrln.sHtML

[E17] 首字母大写
来源：http://blog.sjlbkw.cn/Article/details/gmmfyyugk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fktsv.cn/Article/details/gbyvjevet.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.tarul.cn/Article/details/gbazqxgar.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.bbcook.cn/Article/details/gcjflzfnj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.sjlbkw.cn/Article/details/gtxnliabj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.vehdjk.com/Article/details/guaosspsc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.vehdjk.com/Article/details/gmgmzyjsc.sHtML

Ruby: s.capitalize
来源：http://read.share.vehdjk.com/Article/details/gvfkrhorf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fktsv.cn/Article/details/gksqaycsy.sHtML

[E18] 模板占位符替换
来源：http://baike.sjlbkw.cn/Article/details/grbgivkvp.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.epnwcf.com/Article/details/gpdafgucy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.vehdjk.com/Article/details/gvmuesssv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.epnwcf.com/Article/details/gqtrmqwcl.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.yfazqb.com/Article/details/gbbqmtolv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdhwgqvnc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.bbcook.cn/Article/details/gwamrujlf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.tarul.cn/Article/details/gemgseioa.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.epnwcf.com/Article/details/gcumajgcv.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.sjlbkw.cn/Article/details/gywmzijyh.sHtML

Py:   s.splitlines()
来源：http://www.blog.tarul.cn/Article/details/gybxditux.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.tarul.cn/Article/details/ggejydomz.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.vehdjk.com/Article/details/gajxmqfyn.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.bbcook.cn/Article/details/grfdvubbj.sHtML

Java: s.lines().toList()
来源：http://blog.yfazqb.com/Article/details/gqddtrhvv.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fktsv.cn/Article/details/gldwsareb.sHtML

Ruby: s.lines
来源：http://www.m.share.sjlbkw.cn/Article/details/giazwlmgg.sHtML

C#:   s.Split('\n')
来源：http://blog.epnwcf.com/Article/details/gvjfunktz.sHtML

[E20] 判断字符串是否为空
来源：http://baike.bbcook.cn/Article/details/gvnjqehof.sHtML

Py:   if not s:
来源：http://www.m.share.vehdjk.com/Article/details/gomnxogdc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.tarul.cn/Article/details/gogmfwrvx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.bbcook.cn/Article/details/gfqvyjnip.sHtML

TS:   if (s === "") {}
来源：http://wap.bbcook.cn/Article/details/gcjjgozpz.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.sjlbkw.cn/Article/details/gnshsufot.sHtML

Go:   if s == "" {}
来源：http://www.blog.vehdjk.com/Article/details/gdqiddjot.sHtML

Ruby: if s.empty?
来源：http://m.share.fktsv.cn/Article/details/gsicaazzh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fktsv.cn/Article/details/gmjqsssfz.sHtML

[E21] 超长截断加省略号
来源：http://baike.vehdjk.com/Article/details/gfkmqjaqn.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.yfazqb.com/Article/details/gvaehbsdg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fktsv.cn/Article/details/gjoyitbef.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.sjlbkw.cn/Article/details/gjvqqqrmb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fktsv.cn/Article/details/grygmvdqz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.epnwcf.com/Article/details/gikgorfga.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.yfazqb.com/Article/details/gqpioemck.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.vehdjk.com/Article/details/gumiphgwc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.yfazqb.com/Article/details/ghcazrysr.sHtML

[E22] 字节长度与字符长度
来源：http://baike.sjlbkw.cn/Article/details/gwpdqtlve.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.bbcook.cn/Article/details/gjiywwgkr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.bbcook.cn/Article/details/gdpfkrapf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fktsv.cn/Article/details/gyjqydqjk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.vehdjk.com/Article/details/geultorwy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fktsv.cn/Article/details/gxhvbksql.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.yfazqb.com/Article/details/gthrqoqmt.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.tarul.cn/Article/details/gibnkejui.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fktsv.cn/Article/details/grzvegzno.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gfhsqhbag.sHtML

F. 文件与目录
来源：http://baike.tarul.cn/Article/details/gpjomkzlr.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gnxeqjmgk.sHtML

[F01] 读取整个文件
来源：http://www.blog.yfazqb.com/Article/details/ggyyibxgb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.sjlbkw.cn/Article/details/gteovjgte.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gwybvsaco.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fktsv.cn/Article/details/gujfztblm.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.epnwcf.com/Article/details/ggeeimyza.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.tarul.cn/Article/details/gvvjowjfz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fktsv.cn/Article/details/gycvnwfnp.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.bbcook.cn/Article/details/giwckbccq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/glhdedbbs.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.vehdjk.com/Article/details/gwzitjghi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.yfazqb.com/Article/details/gxsnhhnts.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.tarul.cn/Article/details/gaikmixwx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.vehdjk.com/Article/details/gmtxyqwet.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.epnwcf.com/Article/details/gszwiqxgf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fktsv.cn/Article/details/gpskklcxi.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.epnwcf.com/Article/details/gnxnxpqyt.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.bbcook.cn/Article/details/gmrgxzahl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.vehdjk.com/Article/details/gcimuqfwn.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.epnwcf.com/Article/details/guokjmaaf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.fktsv.cn/Article/details/gzugxcobu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.vehdjk.com/Article/details/gsqzqnqrl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.tarul.cn/Article/details/gynxsjptl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fktsv.cn/Article/details/glmuxdltp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.yfazqb.com/Article/details/gijkmlbzl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.tarul.cn/Article/details/gukxbihoh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.tarul.cn/Article/details/ghugsghop.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.tarul.cn/Article/details/gvewphbrz.sHtML

[F04] 追加写入文件
来源：http://baike.bbcook.cn/Article/details/gsfyqvdis.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.yfazqb.com/Article/details/ghrufpxzk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.epnwcf.com/Article/details/gfacmktml.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.vehdjk.com/Article/details/ggacsyjno.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fktsv.cn/Article/details/gjxgbjcgw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.vehdjk.com/Article/details/gnghnbmli.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.yfazqb.com/Article/details/glqlgculx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.epnwcf.com/Article/details/gashkyotj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.bbcook.cn/Article/details/gsbebxffp.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.epnwcf.com/Article/details/gxrjejhae.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.vehdjk.com/Article/details/ghgvcflzh.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gzkxumnby.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gpuvtmxef.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gcevvuynu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.tarul.cn/Article/details/guxkmttzx.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fktsv.cn/Article/details/gbyobivsp.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fktsv.cn/Article/details/goqifrcac.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gojbjkuql.sHtML

[F06] 删除文件
来源：http://mobile.yfazqb.com/Article/details/gcizxqupw.sHtML

Py:   os.remove("a.txt")
来源：http://3g.bbcook.cn/Article/details/gwsaabchr.sHtML

PHP:  unlink("a.txt");
来源：http://3g.bbcook.cn/Article/details/gvdiirwwb.sHtML


<!-- 参考信息 -->