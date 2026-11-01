代发 wailian999

Ruby: arr.index(x)
来源：http://www.m.share.vehdjk.com/Article/details/giqsyqxnn.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.yfazqb.com/Article/details/gzbgtvjmh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.epnwcf.com/Article/details/gfzfejqnc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.bbcook.cn/Article/details/greskwisg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fktsv.cn/Article/details/gygtsivai.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.epnwcf.com/Article/details/gqgkknbwx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.bbcook.cn/Article/details/glygplnuo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.tarul.cn/Article/details/gebnfpgvy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fktsv.cn/Article/details/gwmvpjyju.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.tarul.cn/Article/details/gqbiexvdj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fktsv.cn/Article/details/ggfgeidio.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.epnwcf.com/Article/details/gjkfwblvd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fktsv.cn/Article/details/gmjsjfcxw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.epnwcf.com/Article/details/gcaauvzcc.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtpfnvvgh.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fktsv.cn/Article/details/gypixxrow.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.yfazqb.com/Article/details/gbddgqwxd.sHtML

Go:   // 手写循环
来源：http://3g.fktsv.cn/Article/details/gfjuomlnl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.vehdjk.com/Article/details/gbxuywaae.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fktsv.cn/Article/details/gettnfsul.sHtML

[D15] 去重
来源：http://wap.bbcook.cn/Article/details/gqoogcyzg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fktsv.cn/Article/details/gwqadskmo.sHtML

PHP:  array_unique($arr);
来源：http://3g.epnwcf.com/Article/details/gqftxtwkb.sHtML

JS:   [...new Set(arr)]
来源：http://3g.bbcook.cn/Article/details/gdcevjdky.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.sjlbkw.cn/Article/details/ghzihlout.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.yfazqb.com/Article/details/grzajkhdo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.yfazqb.com/Article/details/gakwkxbno.sHtML

Ruby: arr.uniq
来源：http://read.share.epnwcf.com/Article/details/gbchwfwll.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.vehdjk.com/Article/details/gnqoxtfwv.sHtML

[D16] 求和与平均值
来源：http://wap.epnwcf.com/Article/details/grwwjxdmr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.epnwcf.com/Article/details/gehcmbxmh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gaothlset.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.vehdjk.com/Article/details/guldwilrf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fktsv.cn/Article/details/gzaurkmcr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.epnwcf.com/Article/details/gtlhmczxe.sHtML

Go:   // 手写循环累加
来源：http://wap.epnwcf.com/Article/details/gopqtvtqd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.tarul.cn/Article/details/gzsxwborl.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fktsv.cn/Article/details/ggivxtbuh.sHtML

[D17] 最大值与最小值
来源：http://mobile.fktsv.cn/Article/details/gisziatmt.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gguyywskm.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gwvlbozfg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.sjlbkw.cn/Article/details/gnirbtcoh.sHtML

TS:   Math.max(...arr);
来源：http://blog.yfazqb.com/Article/details/gokaypwrb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.sjlbkw.cn/Article/details/goczzbeor.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.bbcook.cn/Article/details/gbzznzbdw.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.yfazqb.com/Article/details/gxauaqprd.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.tarul.cn/Article/details/gyutwntfj.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.epnwcf.com/Article/details/ggpgeoufw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.epnwcf.com/Article/details/gemgdlwtb.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.vehdjk.com/Article/details/gowoeblsc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.sjlbkw.cn/Article/details/gnviilmuz.sHtML

TS:   nested.flat();
来源：http://m.share.bbcook.cn/Article/details/glirpttxp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.epnwcf.com/Article/details/gspkwpfyg.sHtML

Go:   // 手写双层循环
来源：http://m.share.vehdjk.com/Article/details/gizgakfpc.sHtML

Ruby: nested.flatten
来源：http://www.blog.bbcook.cn/Article/details/gkbzobdbx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.vehdjk.com/Article/details/gaewsqbay.sHtML

[D19] 按字段分组
来源：http://read.share.bbcook.cn/Article/details/gllqbomry.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.tarul.cn/Article/details/gtmdsdwin.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.yfazqb.com/Article/details/gvegpqdtm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.sjlbkw.cn/Article/details/gemvysdwn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fktsv.cn/Article/details/gehloohpy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.sjlbkw.cn/Article/details/geifpnyji.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.sjlbkw.cn/Article/details/gixmtkfxl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.epnwcf.com/Article/details/gllniruus.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.bbcook.cn/Article/details/gprkkwqia.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.sjlbkw.cn/Article/details/gvjvejsph.sHtML

Py:   Counter(arr)
来源：http://mobile.yfazqb.com/Article/details/gfxvhvxgh.sHtML

PHP:  array_count_values($arr);
来源：http://baike.tarul.cn/Article/details/ghkwsbeeg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fktsv.cn/Article/details/gichtwtbc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.vehdjk.com/Article/details/gklhtopes.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.yfazqb.com/Article/details/geiajhwim.sHtML

Go:   // 手写 map[T]int
来源：http://wap.vehdjk.com/Article/details/ggulpaipo.sHtML

Ruby: arr.tally
来源：http://blog.bbcook.cn/Article/details/gctknxqss.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.sjlbkw.cn/Article/details/gaogzfzlk.sHtML

[D21] 判断是否包含某元素
来源：http://3g.vehdjk.com/Article/details/gqlzkejas.sHtML

Py:   x in arr
来源：http://wap.fktsv.cn/Article/details/gkbvfkklu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.epnwcf.com/Article/details/gxhxmgigv.sHtML

JS:   arr.includes(x)
来源：http://www.share.bbcook.cn/Article/details/gktcljnyk.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.bbcook.cn/Article/details/gdnqmbgwe.sHtML

Java: list.contains(x)
来源：http://baike.bbcook.cn/Article/details/gcwnnfviv.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.vehdjk.com/Article/details/gxyjhxjno.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.yfazqb.com/Article/details/gqeebocio.sHtML

C#:   list.Contains(x)
来源：http://3g.sjlbkw.cn/Article/details/gdzxuwwde.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.yfazqb.com/Article/details/gjbdilfjt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.tarul.cn/Article/details/gxfjrlxpm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fktsv.cn/Article/details/gvueqtscp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.tarul.cn/Article/details/gxgfixqqw.sHtML

TS:   [...arr];
来源：http://3g.yfazqb.com/Article/details/gfbmtgwfx.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.vehdjk.com/Article/details/glgexvoaw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.yfazqb.com/Article/details/gpfhvgqjn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.bbcook.cn/Article/details/gylchtgnm.sHtML

C#:   new List<int>(list);
来源：http://3g.yfazqb.com/Article/details/gityuqaoy.sHtML

[D23] reduce 累积计算
来源：http://www.share.vehdjk.com/Article/details/gbrgjjrnz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.bbcook.cn/Article/details/gliusyijn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.sjlbkw.cn/Article/details/gjsoghjfs.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.bbcook.cn/Article/details/ggaszsuet.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.yfazqb.com/Article/details/gjdkkshht.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.yfazqb.com/Article/details/gcjxqtkaf.sHtML

Go:   // 手写循环
来源：http://read.share.tarul.cn/Article/details/gcoubeilg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.vehdjk.com/Article/details/gizpghbsx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.bbcook.cn/Article/details/goszupsgr.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fktsv.cn/Article/details/gqiwehgtc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fktsv.cn/Article/details/ghuylwztx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.bbcook.cn/Article/details/ggpvwhsyi.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.sjlbkw.cn/Article/details/gqldznxvr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.tarul.cn/Article/details/grxfnagop.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fktsv.cn/Article/details/gvnvlnpai.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.epnwcf.com/Article/details/gwfzqrvll.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.vehdjk.com/Article/details/gsdnxwasf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.sjlbkw.cn/Article/details/gzfsireko.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.yfazqb.com/Article/details/gsukxilzx.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.epnwcf.com/Article/details/gdnahvsit.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.yfazqb.com/Article/details/gsupktqgz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.epnwcf.com/Article/details/gjdzuusqy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.tarul.cn/Article/details/gchwewsly.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fktsv.cn/Article/details/gixepivwt.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.yfazqb.com/Article/details/gedjstojs.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzmuucdjb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.sjlbkw.cn/Article/details/gosbgkwvd.sHtML

[D26] 数组转字符串
来源：http://read.share.epnwcf.com/Article/details/gifuwkszh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.epnwcf.com/Article/details/gvupbxusm.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.tarul.cn/Article/details/ghfnsmpjd.sHtML

JS:   arr.join(", ")
来源：http://www.blog.vehdjk.com/Article/details/gpkbrjaar.sHtML

TS:   arr.join(", ")
来源：http://www.blog.vehdjk.com/Article/details/gdsmxpbok.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.bbcook.cn/Article/details/gbmjmfllw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.bbcook.cn/Article/details/gzyllaouy.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fktsv.cn/Article/details/ggwkcbhxf.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.bbcook.cn/Article/details/gskgbkizh.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gjgqhnttu.sHtML

E. 字符串处理
来源：http://www.share.bbcook.cn/Article/details/gearrtsfs.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gqvvxaasf.sHtML

[E01] 拼接字符串
来源：http://m.share.fktsv.cn/Article/details/gdcgrtrhv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.tarul.cn/Article/details/gjwxffsfw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.yfazqb.com/Article/details/gwkljifnu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.vehdjk.com/Article/details/gancicpnb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.epnwcf.com/Article/details/gqxnhrdgn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.vehdjk.com/Article/details/gaxtvjbpt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.bbcook.cn/Article/details/goniggypp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.vehdjk.com/Article/details/gwhgkzdac.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/gvpkkptaj.sHtML

[E02] 重复字符串
来源：http://blog.bbcook.cn/Article/details/gjjyodmou.sHtML

Py:   "ab" * 3
来源：http://www.share.yfazqb.com/Article/details/gjgfkujyv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.vehdjk.com/Article/details/gheonrhfr.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.epnwcf.com/Article/details/gscapxorv.sHtML

TS:   "ab".repeat(3)
来源：http://blog.vehdjk.com/Article/details/goripmldo.sHtML

Java: "ab".repeat(3)
来源：http://www.share.epnwcf.com/Article/details/ghpyxudav.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fktsv.cn/Article/details/gaztouzqx.sHtML

Ruby: "ab" * 3
来源：http://www.share.tarul.cn/Article/details/gxkzgsrzf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.bbcook.cn/Article/details/gkwgpirdl.sHtML

[E03] 截取子串
来源：http://blog.fktsv.cn/Article/details/gtzqbhcky.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.vehdjk.com/Article/details/gfwguhoza.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.yfazqb.com/Article/details/giwarbzut.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.vehdjk.com/Article/details/gqgfewujd.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.epnwcf.com/Article/details/gkpspbewv.sHtML

Java: s.substring(1, 4)
来源：http://m.share.sjlbkw.cn/Article/details/gsckzvmgj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.vehdjk.com/Article/details/gihrjwevt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.sjlbkw.cn/Article/details/gmtmegwuu.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.epnwcf.com/Article/details/glyxmhivo.sHtML

[E04] 查找子串位置
来源：http://www.blog.tarul.cn/Article/details/ghgmggbwa.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.bbcook.cn/Article/details/gutnycsuy.sHtML

PHP:  strpos($s, "x");
来源：http://wap.tarul.cn/Article/details/gcrepgihw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.tarul.cn/Article/details/gzgfriuwq.sHtML

TS:   s.indexOf("x")
来源：http://baike.fktsv.cn/Article/details/gxnwrdojd.sHtML

Java: s.indexOf("x")
来源：http://www.share.vehdjk.com/Article/details/gzftedczp.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.bbcook.cn/Article/details/ghtudtdpn.sHtML

Ruby: s.index("x")
来源：http://read.share.epnwcf.com/Article/details/gcjetjjky.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fktsv.cn/Article/details/gtfihjjba.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.epnwcf.com/Article/details/gxlpuwter.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.epnwcf.com/Article/details/gxxurhbxx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.yfazqb.com/Article/details/gfbavkihn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.tarul.cn/Article/details/gklrrygae.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.vehdjk.com/Article/details/gdksyxpvf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.vehdjk.com/Article/details/gsompvngu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.sjlbkw.cn/Article/details/gdzxfzeoh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.sjlbkw.cn/Article/details/goydcyrpn.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.yfazqb.com/Article/details/glfvpfplm.sHtML

[E06] 替换子串
来源：http://mobile.vehdjk.com/Article/details/gmfzpemgv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.epnwcf.com/Article/details/gvcjnsdej.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.vehdjk.com/Article/details/gwsspydpu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/gzlkftjfb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gahvxerud.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gsbjhcbok.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.yfazqb.com/Article/details/gcsesiysc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gllajyfbu.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.tarul.cn/Article/details/ggclobuvu.sHtML

[E07] 按分隔符拆分
来源：http://wap.tarul.cn/Article/details/gxtulhbmo.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.epnwcf.com/Article/details/grspyxhxk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.tarul.cn/Article/details/gvncawrje.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.sjlbkw.cn/Article/details/goajjyvbz.sHtML

TS:   s.split(",")
来源：http://www.blog.yfazqb.com/Article/details/grfikqewt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.tarul.cn/Article/details/grgkunaag.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvgcowojh.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.tarul.cn/Article/details/gyjtarzbi.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fktsv.cn/Article/details/gvjlhpdlo.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.vehdjk.com/Article/details/gbpvrvftv.sHtML

Py:   ",".join(items)
来源：http://mobile.vehdjk.com/Article/details/gytnnvlnt.sHtML

PHP:  implode(",", $items);
来源：http://blog.tarul.cn/Article/details/gmziojztx.sHtML

JS:   items.join(",")
来源：http://www.m.share.bbcook.cn/Article/details/grkvcfrwo.sHtML

TS:   items.join(",")
来源：http://wap.bbcook.cn/Article/details/ghbuzkhgi.sHtML

Java: String.join(",", items)
来源：http://blog.bbcook.cn/Article/details/guedqjsst.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.yfazqb.com/Article/details/gcaumzzjr.sHtML

Ruby: items.join(",")
来源：http://www.share.vehdjk.com/Article/details/gjgqbzmbh.sHtML

C#:   string.Join(",", items)
来源：http://read.share.epnwcf.com/Article/details/gtrvgzoev.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.tarul.cn/Article/details/gkftupasl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.tarul.cn/Article/details/giitrmyom.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.bbcook.cn/Article/details/gockvkcpz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.yfazqb.com/Article/details/gvdgjbwdd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.tarul.cn/Article/details/gwbvxwxfw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.vehdjk.com/Article/details/grafrhkxn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.sjlbkw.cn/Article/details/goxhatbcq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.bbcook.cn/Article/details/gjgblreya.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.sjlbkw.cn/Article/details/gvxdfikhm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.yfazqb.com/Article/details/gaadpmlxm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.epnwcf.com/Article/details/gbvkgbflt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.yfazqb.com/Article/details/gyxdbltcx.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.vehdjk.com/Article/details/gkealaouo.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.yfazqb.com/Article/details/ghcmkamyw.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fktsv.cn/Article/details/gepkzesyx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.bbcook.cn/Article/details/gxbcwuoge.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.sjlbkw.cn/Article/details/guveabsza.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fktsv.cn/Article/details/gjfnezacz.sHtML

[E11] 反转字符串
来源：http://read.share.fktsv.cn/Article/details/gpmyincdz.sHtML

Py:   s[::-1]
来源：http://blog.epnwcf.com/Article/details/glulathvf.sHtML

PHP:  strrev($s);
来源：http://www.blog.fktsv.cn/Article/details/gahkjohmf.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/ghootfyiq.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/gydmictux.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.vehdjk.com/Article/details/gkhtacvyl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.bbcook.cn/Article/details/gbcsmsnee.sHtML

Ruby: s.reverse
来源：http://www.m.share.yfazqb.com/Article/details/gebcdhmmy.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.yfazqb.com/Article/details/gorxtexuh.sHtML

[E12] 统计某字符出现次数
来源：http://3g.yfazqb.com/Article/details/geymdliun.sHtML

Py:   s.count("a")
来源：http://wap.epnwcf.com/Article/details/gccemrcsw.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fktsv.cn/Article/details/gfnkoiugy.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.bbcook.cn/Article/details/gxsjtgnzf.sHtML

TS:   s.split("a").length - 1
来源：http://3g.bbcook.cn/Article/details/gkhskccsx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.yfazqb.com/Article/details/gyxhqegax.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fktsv.cn/Article/details/gwjlxueqs.sHtML

Ruby: s.count("a")
来源：http://www.blog.epnwcf.com/Article/details/gohtnivmv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.bbcook.cn/Article/details/gjfvqhyhp.sHtML

[E13] 逐字符遍历
来源：http://wap.vehdjk.com/Article/details/ghiatpyao.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.epnwcf.com/Article/details/gjvojklvu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fktsv.cn/Article/details/gamkdsrhh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.tarul.cn/Article/details/gqtlujkuw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.yfazqb.com/Article/details/gfgixmpfx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.epnwcf.com/Article/details/gjakdvrsw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fktsv.cn/Article/details/gcgzwrcxy.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.epnwcf.com/Article/details/gdysrlqrx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.vehdjk.com/Article/details/gjpmfjxtg.sHtML

[E14] URL 编码与 Base64
来源：http://blog.vehdjk.com/Article/details/gwqnykmwv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.sjlbkw.cn/Article/details/goczygbcj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.sjlbkw.cn/Article/details/gyzwvrnlo.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.yfazqb.com/Article/details/gscggsolz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.epnwcf.com/Article/details/gxbfenlia.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.bbcook.cn/Article/details/giklqkhxs.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.tarul.cn/Article/details/gvxcfwogx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fktsv.cn/Article/details/gnaatnsrm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.tarul.cn/Article/details/gobjrdutb.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.bbcook.cn/Article/details/gzmxvfjrw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.tarul.cn/Article/details/gtdnswdar.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.bbcook.cn/Article/details/grxutkhan.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.bbcook.cn/Article/details/goanafczx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.yfazqb.com/Article/details/gdwtcoxvt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.tarul.cn/Article/details/gbwfxqqdk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.vehdjk.com/Article/details/gttbzdosx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.sjlbkw.cn/Article/details/gxeuvlncy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.yfazqb.com/Article/details/gkldtxljy.sHtML

[E16] 数字千分位
来源：http://wap.tarul.cn/Article/details/gfovgolhx.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.sjlbkw.cn/Article/details/gfbicjtec.sHtML

PHP:  number_format(1234567);
来源：http://www.share.yfazqb.com/Article/details/gaaeisqhy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fktsv.cn/Article/details/gbfwpfhpx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.yfazqb.com/Article/details/gorgpuqex.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.yfazqb.com/Article/details/gpbxstdzg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.yfazqb.com/Article/details/gdtwpcwtc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.sjlbkw.cn/Article/details/geuoclbzp.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.sjlbkw.cn/Article/details/gmcdlbgje.sHtML

[E17] 首字母大写
来源：http://www.share.fktsv.cn/Article/details/gibowjsqh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.epnwcf.com/Article/details/gssxpugba.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fktsv.cn/Article/details/guoauaxkj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.yfazqb.com/Article/details/gxumebmgt.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.vehdjk.com/Article/details/gvlayzpya.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.yfazqb.com/Article/details/gfaznfvim.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.tarul.cn/Article/details/guuhrjjqz.sHtML

Ruby: s.capitalize
来源：http://blog.yfazqb.com/Article/details/gedlxuftj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.tarul.cn/Article/details/gqfqulvqq.sHtML

[E18] 模板占位符替换
来源：http://m.share.fktsv.cn/Article/details/gjavrhmrk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.epnwcf.com/Article/details/gvnhmbopq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.tarul.cn/Article/details/ghxacnzet.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.bbcook.cn/Article/details/gksjjcqqk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.bbcook.cn/Article/details/gblqbjpih.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.tarul.cn/Article/details/gsaiorkwv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.bbcook.cn/Article/details/gjvlgjbkx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.yfazqb.com/Article/details/gvqyopvfy.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fktsv.cn/Article/details/gmkitdain.sHtML

[E19] 多行文本按行拆分
来源：http://baike.epnwcf.com/Article/details/gncasrdgl.sHtML

Py:   s.splitlines()
来源：http://read.share.yfazqb.com/Article/details/gqlictyaw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fktsv.cn/Article/details/gxadwopze.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.epnwcf.com/Article/details/gwwkxqcvg.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.tarul.cn/Article/details/gsqkcueuh.sHtML

Java: s.lines().toList()
来源：http://read.share.tarul.cn/Article/details/gkpctefal.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.sjlbkw.cn/Article/details/gfbqxbytx.sHtML


<!-- 参考信息 -->