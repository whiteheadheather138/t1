代发 wailian999

Ruby: arr.tally
来源：http://3g.epnwcf.com/Article/details/gyafaywhg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fktsv.cn/Article/details/ghlqbnnlb.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.yfazqb.com/Article/details/ggsuxjsxt.sHtML

Py:   x in arr
来源：http://m.share.sjlbkw.cn/Article/details/gaxwznqfj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.yfazqb.com/Article/details/gtmrhrmly.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.bbcook.cn/Article/details/gmahpounk.sHtML

TS:   arr.includes(x)
来源：http://wap.bbcook.cn/Article/details/gdeerkvkx.sHtML

Java: list.contains(x)
来源：http://blog.yfazqb.com/Article/details/grpadslpq.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gquwrucog.sHtML

Ruby: arr.include?(x)
来源：http://wap.vehdjk.com/Article/details/grzoejjrq.sHtML

C#:   list.Contains(x)
来源：http://mobile.bbcook.cn/Article/details/gwogienqk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.sjlbkw.cn/Article/details/gvfhkuodo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.bbcook.cn/Article/details/gqbtdnioo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.vehdjk.com/Article/details/gjxjcgmbh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.bbcook.cn/Article/details/gnveegfcq.sHtML

TS:   [...arr];
来源：http://baike.vehdjk.com/Article/details/grorfjuro.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.epnwcf.com/Article/details/gmyubween.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.sjlbkw.cn/Article/details/gsqzmiwku.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fktsv.cn/Article/details/gdypxpogr.sHtML

C#:   new List<int>(list);
来源：http://wap.yfazqb.com/Article/details/gvksqgbow.sHtML

[D23] reduce 累积计算
来源：http://read.share.sjlbkw.cn/Article/details/gmkkrwags.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.bbcook.cn/Article/details/gdghkbhpt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.tarul.cn/Article/details/gyxombqpr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.bbcook.cn/Article/details/gbmxnunac.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.epnwcf.com/Article/details/gultlthby.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.bbcook.cn/Article/details/ggtzcxacf.sHtML

Go:   // 手写循环
来源：http://www.blog.bbcook.cn/Article/details/giziilbhc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.yfazqb.com/Article/details/gwtefkcep.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.vehdjk.com/Article/details/gniikgulh.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.epnwcf.com/Article/details/gkontusnt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.bbcook.cn/Article/details/gbjgiulxd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.tarul.cn/Article/details/gvpdoritn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.fktsv.cn/Article/details/gtsduikpy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fktsv.cn/Article/details/gbtthemfo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.yfazqb.com/Article/details/gouknehzr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fktsv.cn/Article/details/gwcirybbh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.bbcook.cn/Article/details/gpthkigyd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fktsv.cn/Article/details/gdqoomsfa.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fktsv.cn/Article/details/gjdkgxkyo.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.sjlbkw.cn/Article/details/gwiolakpz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.vehdjk.com/Article/details/gtduklmka.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.vehdjk.com/Article/details/gqyyhilhu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.bbcook.cn/Article/details/gavfpvklo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.epnwcf.com/Article/details/gxyheqoid.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.tarul.cn/Article/details/gtnlfcyik.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.vehdjk.com/Article/details/ghnxfxquz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.yfazqb.com/Article/details/grqrsmkxt.sHtML

[D26] 数组转字符串
来源：http://www.share.yfazqb.com/Article/details/gyhbhjgdk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.yfazqb.com/Article/details/gudkmdrra.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.vehdjk.com/Article/details/gtonuajrk.sHtML

JS:   arr.join(", ")
来源：http://wap.bbcook.cn/Article/details/glqfprdcy.sHtML

TS:   arr.join(", ")
来源：http://mobile.tarul.cn/Article/details/grhopdler.sHtML

Java: String.join(", ", list)
来源：http://3g.tarul.cn/Article/details/ghkwbmgnc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.bbcook.cn/Article/details/gvljmcmkf.sHtML

Ruby: arr.join(", ")
来源：http://3g.epnwcf.com/Article/details/gwlslknzj.sHtML

C#:   string.Join(", ", list)
来源：http://baike.vehdjk.com/Article/details/gnnhfzorj.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gjeirdtcb.sHtML

E. 字符串处理
来源：http://www.m.share.tarul.cn/Article/details/gsqenkjsn.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/guftwvjnw.sHtML

[E01] 拼接字符串
来源：http://www.share.tarul.cn/Article/details/gbofiahds.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.bbcook.cn/Article/details/gedfsbysq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.sjlbkw.cn/Article/details/goztzojqs.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.epnwcf.com/Article/details/gxmtylpeg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fktsv.cn/Article/details/grzrbdgod.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.fktsv.cn/Article/details/gffgngkwc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.epnwcf.com/Article/details/gyciiwtcc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.sjlbkw.cn/Article/details/gtvxnrwqm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/gnkjiljqx.sHtML

[E02] 重复字符串
来源：http://wap.tarul.cn/Article/details/gxlodczlt.sHtML

Py:   "ab" * 3
来源：http://blog.vehdjk.com/Article/details/ghiuyiavc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.yfazqb.com/Article/details/giohsogwy.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.epnwcf.com/Article/details/gpiqbvuao.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fktsv.cn/Article/details/glczubrpt.sHtML

Java: "ab".repeat(3)
来源：http://read.share.bbcook.cn/Article/details/gvhoiumsj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fktsv.cn/Article/details/gpuuwlirf.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.tarul.cn/Article/details/ggsvmgdon.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.bbcook.cn/Article/details/gprgtvmgv.sHtML

[E03] 截取子串
来源：http://www.blog.sjlbkw.cn/Article/details/ghjklerkr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.bbcook.cn/Article/details/gizznropd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.vehdjk.com/Article/details/gnzaxolio.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.tarul.cn/Article/details/gtopmhohl.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.epnwcf.com/Article/details/gitzgdkpj.sHtML

Java: s.substring(1, 4)
来源：http://3g.sjlbkw.cn/Article/details/gbtulxwnf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.vehdjk.com/Article/details/gnsqafzio.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fktsv.cn/Article/details/gkziwwmst.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.vehdjk.com/Article/details/giwlntdep.sHtML

[E04] 查找子串位置
来源：http://read.share.vehdjk.com/Article/details/gxlosxjai.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.bbcook.cn/Article/details/gbfxgktpe.sHtML

PHP:  strpos($s, "x");
来源：http://baike.vehdjk.com/Article/details/goewflero.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.bbcook.cn/Article/details/grztghfro.sHtML

TS:   s.indexOf("x")
来源：http://read.share.yfazqb.com/Article/details/glashuyuc.sHtML

Java: s.indexOf("x")
来源：http://baike.yfazqb.com/Article/details/gxoogvrwx.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.tarul.cn/Article/details/gxefzjdlf.sHtML

Ruby: s.index("x")
来源：http://www.blog.bbcook.cn/Article/details/gpefyslhi.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.yfazqb.com/Article/details/ggppxcsxf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.yfazqb.com/Article/details/gvuzztxqp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.bbcook.cn/Article/details/gvbcjvkbc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.epnwcf.com/Article/details/gecdjhuot.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.epnwcf.com/Article/details/ggzppnyph.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.bbcook.cn/Article/details/gmhcfzvuv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.tarul.cn/Article/details/gyovmiexz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.bbcook.cn/Article/details/gzdhdsnhu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.bbcook.cn/Article/details/gntjysosd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.epnwcf.com/Article/details/gduccruak.sHtML

[E06] 替换子串
来源：http://3g.epnwcf.com/Article/details/ghftgvyly.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.yfazqb.com/Article/details/gcrucnrnv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.epnwcf.com/Article/details/grtiauucu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.epnwcf.com/Article/details/giwyayaoc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gcuwbihqz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.vehdjk.com/Article/details/gutiwmwin.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.yfazqb.com/Article/details/gowupuvki.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.vehdjk.com/Article/details/gxhiqbozl.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/gfzwjxfcg.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fktsv.cn/Article/details/gmvosbixx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fktsv.cn/Article/details/gfysrxfls.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.epnwcf.com/Article/details/gxxerokok.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fktsv.cn/Article/details/gygiabwdm.sHtML

TS:   s.split(",")
来源：http://wap.fktsv.cn/Article/details/gjxbjczjo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.tarul.cn/Article/details/gqakviigm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fktsv.cn/Article/details/gemytslqe.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.bbcook.cn/Article/details/gjhzwyocu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.yfazqb.com/Article/details/gutjkgfvw.sHtML

[E08] 数组按分隔符合并
来源：http://blog.tarul.cn/Article/details/gkooxlhnb.sHtML

Py:   ",".join(items)
来源：http://www.share.tarul.cn/Article/details/grmeskrrp.sHtML

PHP:  implode(",", $items);
来源：http://wap.sjlbkw.cn/Article/details/gmivuzhba.sHtML

JS:   items.join(",")
来源：http://mobile.yfazqb.com/Article/details/gyldsfiwn.sHtML

TS:   items.join(",")
来源：http://blog.sjlbkw.cn/Article/details/guxgtigct.sHtML

Java: String.join(",", items)
来源：http://www.share.tarul.cn/Article/details/gripkljpy.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.yfazqb.com/Article/details/gxgyoakuw.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fktsv.cn/Article/details/ggfacgekq.sHtML

C#:   string.Join(",", items)
来源：http://baike.tarul.cn/Article/details/gkumbmizg.sHtML

[E09] 去除所有空白字符
来源：http://mobile.epnwcf.com/Article/details/gfhurksbt.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fktsv.cn/Article/details/godnfjgtc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.vehdjk.com/Article/details/gfgxazhht.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.vehdjk.com/Article/details/gsiqlvboe.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fktsv.cn/Article/details/gcddmfase.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.vehdjk.com/Article/details/gxrrwswrd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.tarul.cn/Article/details/gstkzdmfq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.vehdjk.com/Article/details/grhucasxo.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.vehdjk.com/Article/details/goegpzraa.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.sjlbkw.cn/Article/details/gmrkluqjf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.vehdjk.com/Article/details/gkmxqfijs.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fktsv.cn/Article/details/gfvbnmxjb.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.tarul.cn/Article/details/gimgqhskc.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.yfazqb.com/Article/details/ggfwmqqad.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.yfazqb.com/Article/details/gkraiampr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.yfazqb.com/Article/details/gupbusipg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.epnwcf.com/Article/details/gxnhgprjz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fktsv.cn/Article/details/gbatutmei.sHtML

[E11] 反转字符串
来源：http://blog.sjlbkw.cn/Article/details/gsxvhwjgk.sHtML

Py:   s[::-1]
来源：http://blog.yfazqb.com/Article/details/gjcebhyfv.sHtML

PHP:  strrev($s);
来源：http://www.blog.fktsv.cn/Article/details/gdqcimeio.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.epnwcf.com/Article/details/goebfgujy.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.yfazqb.com/Article/details/gmuybusik.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.vehdjk.com/Article/details/gimafexhy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.epnwcf.com/Article/details/glvplgrzh.sHtML

Ruby: s.reverse
来源：http://www.m.share.yfazqb.com/Article/details/gxfiexcjn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.tarul.cn/Article/details/gxskmiogr.sHtML

[E12] 统计某字符出现次数
来源：http://blog.sjlbkw.cn/Article/details/gomejyype.sHtML

Py:   s.count("a")
来源：http://baike.fktsv.cn/Article/details/gbxyzasid.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.bbcook.cn/Article/details/gqrecgxtv.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.epnwcf.com/Article/details/gqxpljume.sHtML

TS:   s.split("a").length - 1
来源：http://wap.sjlbkw.cn/Article/details/ggqavmffc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.epnwcf.com/Article/details/gvbzlrgtk.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.tarul.cn/Article/details/gumosljjg.sHtML

Ruby: s.count("a")
来源：http://read.share.fktsv.cn/Article/details/gszbtxgrn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.sjlbkw.cn/Article/details/gyhyudyzk.sHtML

[E13] 逐字符遍历
来源：http://wap.yfazqb.com/Article/details/gjhzwrloy.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.epnwcf.com/Article/details/ggslpkyqv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.epnwcf.com/Article/details/ggkmzclmo.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.vehdjk.com/Article/details/gqjupcwjc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.bbcook.cn/Article/details/gevowtltq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.epnwcf.com/Article/details/geytvoihs.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.yfazqb.com/Article/details/gmetetkds.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fktsv.cn/Article/details/grphwnand.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fktsv.cn/Article/details/gtgnqsjtp.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.epnwcf.com/Article/details/ggzzthmov.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.vehdjk.com/Article/details/gwlphmava.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.epnwcf.com/Article/details/gjbauveeh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.bbcook.cn/Article/details/gohlwwwkm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.sjlbkw.cn/Article/details/gfsxacdfa.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fktsv.cn/Article/details/gbsexdcvo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.tarul.cn/Article/details/gpdnhspkc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fktsv.cn/Article/details/gfddwdrnj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.yfazqb.com/Article/details/gwfxpnqpj.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.epnwcf.com/Article/details/gwvypkdsv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.sjlbkw.cn/Article/details/ghtnznxte.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.sjlbkw.cn/Article/details/gchhjkqcf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.epnwcf.com/Article/details/gogdpgwzo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.fktsv.cn/Article/details/gqcicfppf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.sjlbkw.cn/Article/details/ggfglasdm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.sjlbkw.cn/Article/details/gtyndwgxe.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.tarul.cn/Article/details/gavyuhdkz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.epnwcf.com/Article/details/gcatqsnfi.sHtML

[E16] 数字千分位
来源：http://read.share.yfazqb.com/Article/details/gmiggenum.sHtML

Py:   f"{1234567:,}"
来源：http://3g.sjlbkw.cn/Article/details/gzfnmwsut.sHtML

PHP:  number_format(1234567);
来源：http://read.share.bbcook.cn/Article/details/gcwjalmun.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.epnwcf.com/Article/details/gmbqpwalg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.sjlbkw.cn/Article/details/gqfcgfxzu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fktsv.cn/Article/details/gbsleodrr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.vehdjk.com/Article/details/gisharkxf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.epnwcf.com/Article/details/gvugmigjh.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.bbcook.cn/Article/details/gipixgaeg.sHtML

[E17] 首字母大写
来源：http://baike.sjlbkw.cn/Article/details/gbfnrxafu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.tarul.cn/Article/details/gjftfeand.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.vehdjk.com/Article/details/gbgznwfun.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fktsv.cn/Article/details/gehcmowma.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.yfazqb.com/Article/details/gszqlgzpy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fktsv.cn/Article/details/gvpliojsd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.yfazqb.com/Article/details/gsonfrvfa.sHtML

Ruby: s.capitalize
来源：http://3g.tarul.cn/Article/details/gsojujprn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.bbcook.cn/Article/details/gaqsbndqe.sHtML

[E18] 模板占位符替换
来源：http://baike.fktsv.cn/Article/details/gyeskclbw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.bbcook.cn/Article/details/gehttnfdn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.sjlbkw.cn/Article/details/gmfvwjsep.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.bbcook.cn/Article/details/garqckusz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.bbcook.cn/Article/details/gakdtszly.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fktsv.cn/Article/details/gmtpgtivv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.yfazqb.com/Article/details/gcervieuu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.bbcook.cn/Article/details/ggytqygmu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.sjlbkw.cn/Article/details/gaatbdqgm.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.sjlbkw.cn/Article/details/gdxtodimw.sHtML

Py:   s.splitlines()
来源：http://m.share.vehdjk.com/Article/details/gphtjwvql.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.tarul.cn/Article/details/gtlmivekn.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.sjlbkw.cn/Article/details/gqvrzdgho.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.vehdjk.com/Article/details/glukqugce.sHtML

Java: s.lines().toList()
来源：http://baike.sjlbkw.cn/Article/details/gbkkvqady.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.yfazqb.com/Article/details/gsbmhjxsv.sHtML

Ruby: s.lines
来源：http://www.share.sjlbkw.cn/Article/details/gfswpjfys.sHtML

C#:   s.Split('\n')
来源：http://wap.epnwcf.com/Article/details/gxqxkzvco.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.tarul.cn/Article/details/gmemmerqn.sHtML

Py:   if not s:
来源：http://mobile.yfazqb.com/Article/details/gphuzppmv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.yfazqb.com/Article/details/gzkmbddwf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.sjlbkw.cn/Article/details/gcgbdxzki.sHtML

TS:   if (s === "") {}
来源：http://wap.epnwcf.com/Article/details/gpljivmcs.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gatxxdbsj.sHtML

Go:   if s == "" {}
来源：http://baike.epnwcf.com/Article/details/gforpvicf.sHtML

Ruby: if s.empty?
来源：http://baike.epnwcf.com/Article/details/gjnimiyzl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fktsv.cn/Article/details/grzcniiwd.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.epnwcf.com/Article/details/gxrbccffg.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.bbcook.cn/Article/details/gsxqnyfcu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.bbcook.cn/Article/details/gwasjobgp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.yfazqb.com/Article/details/gidsnvlwj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/gydckhrgh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.yfazqb.com/Article/details/gdybltysh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.sjlbkw.cn/Article/details/goehkqeqk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.bbcook.cn/Article/details/gjumthmrd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.yfazqb.com/Article/details/ghyievoid.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.epnwcf.com/Article/details/ggiasmgdm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.vehdjk.com/Article/details/ghrvxueck.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fktsv.cn/Article/details/gdlslqztu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.tarul.cn/Article/details/gyjyuecnq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.epnwcf.com/Article/details/ggozdwwil.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.bbcook.cn/Article/details/geppsasum.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.tarul.cn/Article/details/gounysisp.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.tarul.cn/Article/details/ghlckqnfr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.yfazqb.com/Article/details/gobgkrglm.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/grdrydloi.sHtML

F. 文件与目录
来源：http://baike.yfazqb.com/Article/details/ggykmxiyh.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/ggkjrtjbb.sHtML

[F01] 读取整个文件
来源：http://blog.vehdjk.com/Article/details/gtlssrtyk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.yfazqb.com/Article/details/gqdirfeic.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.tarul.cn/Article/details/gxlvwdkuj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fktsv.cn/Article/details/guemhgvge.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.tarul.cn/Article/details/gdmegdbgy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/gfmljdgwq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.tarul.cn/Article/details/grjrmuqhe.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fktsv.cn/Article/details/ghgdptrnf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.yfazqb.com/Article/details/gdkdjcgkr.sHtML

[F02] 逐行读取文件
来源：http://wap.epnwcf.com/Article/details/gbhbxiwrl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.sjlbkw.cn/Article/details/gxucwfgxu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fktsv.cn/Article/details/gbhpsafbt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.bbcook.cn/Article/details/gcmnvzehl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.yfazqb.com/Article/details/gunlchlvx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.epnwcf.com/Article/details/gfpetafnn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.vehdjk.com/Article/details/grmcrgfyp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.epnwcf.com/Article/details/goiktxahr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.yfazqb.com/Article/details/gxwvgltxr.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fktsv.cn/Article/details/gduyhopfx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.bbcook.cn/Article/details/gtczuvaio.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.tarul.cn/Article/details/gugzzvnsl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.vehdjk.com/Article/details/glxjpcwyw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fktsv.cn/Article/details/gebdrvdoy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.sjlbkw.cn/Article/details/gwoarbixz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fktsv.cn/Article/details/gqwdtkmlx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.yfazqb.com/Article/details/ghvrjwtjd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.sjlbkw.cn/Article/details/gkqwpkjqf.sHtML

[F04] 追加写入文件
来源：http://mobile.fktsv.cn/Article/details/gmdehrhmc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.yfazqb.com/Article/details/gxlfumhks.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.yfazqb.com/Article/details/gbeplygmi.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.yfazqb.com/Article/details/gqqnfoqaw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fktsv.cn/Article/details/gpziynnwu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.epnwcf.com/Article/details/gnlodjjwm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.sjlbkw.cn/Article/details/gklpifbvm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.vehdjk.com/Article/details/gamzchsgj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.bbcook.cn/Article/details/gmjdafwyk.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.yfazqb.com/Article/details/gclsuoiej.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.tarul.cn/Article/details/gdllvjuct.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gikjutbxl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gbzbfvxiw.sHtML


<!-- 参考信息 -->