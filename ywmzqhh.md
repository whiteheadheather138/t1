代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fktsv.cn/Article/details/gczovlyij.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.tarul.cn/Article/details/gqrzyjvpt.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.bbcook.cn/Article/details/gheilcwza.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/gpmwgzwlf.sHtML

Ruby: arr.index(x)
来源：http://3g.vehdjk.com/Article/details/gdqkcvlzc.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.epnwcf.com/Article/details/gmpwumbpy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.tarul.cn/Article/details/gfzovrgqy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.epnwcf.com/Article/details/gztchuxjs.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.epnwcf.com/Article/details/guzzchthc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.bbcook.cn/Article/details/goqckjyan.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.yfazqb.com/Article/details/glhscumeh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.tarul.cn/Article/details/gocdxeaif.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.bbcook.cn/Article/details/gzdlorkqe.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.vehdjk.com/Article/details/gsvhhslmy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.sjlbkw.cn/Article/details/gvlyknkoh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.yfazqb.com/Article/details/glrmaunpr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.yfazqb.com/Article/details/gebkpwbcu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.tarul.cn/Article/details/gbwodyxoi.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.tarul.cn/Article/details/guyuslldj.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.bbcook.cn/Article/details/ganwvpxoi.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.bbcook.cn/Article/details/glrrbpcfe.sHtML

Go:   // 手写循环
来源：http://mobile.fktsv.cn/Article/details/ghtyzxmuw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.yfazqb.com/Article/details/ggololaoy.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fktsv.cn/Article/details/gubcbzyey.sHtML

[D15] 去重
来源：http://www.m.share.vehdjk.com/Article/details/gmzeoprav.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.epnwcf.com/Article/details/gkmfczzhi.sHtML

PHP:  array_unique($arr);
来源：http://3g.epnwcf.com/Article/details/gmklnfwvi.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fktsv.cn/Article/details/gvteeiblj.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.yfazqb.com/Article/details/gcibjkshe.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.sjlbkw.cn/Article/details/gycqgzjkd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.tarul.cn/Article/details/guhenjnaw.sHtML

Ruby: arr.uniq
来源：http://3g.yfazqb.com/Article/details/gyeeehxpm.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.vehdjk.com/Article/details/goxkngnjm.sHtML

[D16] 求和与平均值
来源：http://wap.vehdjk.com/Article/details/goajffbuu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.tarul.cn/Article/details/gfpsatnhq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.sjlbkw.cn/Article/details/gopttwmem.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.bbcook.cn/Article/details/gilofgbdn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.bbcook.cn/Article/details/gnfqvgcld.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.epnwcf.com/Article/details/gqirtvmij.sHtML

Go:   // 手写循环累加
来源：http://wap.tarul.cn/Article/details/ginzndjdq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fktsv.cn/Article/details/gdtycjsfg.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.vehdjk.com/Article/details/gbffaucgo.sHtML

[D17] 最大值与最小值
来源：http://m.share.epnwcf.com/Article/details/gqcnvycxv.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.tarul.cn/Article/details/gccrdzijh.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.yfazqb.com/Article/details/gyfikcmqb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.sjlbkw.cn/Article/details/gkgyetybi.sHtML

TS:   Math.max(...arr);
来源：http://3g.fktsv.cn/Article/details/gdebdncfn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.sjlbkw.cn/Article/details/ggpwtdtas.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fktsv.cn/Article/details/guzmkbjct.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.bbcook.cn/Article/details/gmmxjqymk.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fktsv.cn/Article/details/gccoahowh.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.tarul.cn/Article/details/gocvehaxh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.bbcook.cn/Article/details/golhkluce.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.yfazqb.com/Article/details/gwxvkeivc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.epnwcf.com/Article/details/giviyhuio.sHtML

TS:   nested.flat();
来源：http://m.share.sjlbkw.cn/Article/details/gdqicwjgx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.vehdjk.com/Article/details/gtnzjuqoq.sHtML

Go:   // 手写双层循环
来源：http://m.share.tarul.cn/Article/details/gykdoxtxv.sHtML

Ruby: nested.flatten
来源：http://baike.epnwcf.com/Article/details/gvktauuuq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.tarul.cn/Article/details/goprpfnyr.sHtML

[D19] 按字段分组
来源：http://m.share.sjlbkw.cn/Article/details/gwlvwkrai.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.tarul.cn/Article/details/gjqdhyvje.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fktsv.cn/Article/details/gfipnilmo.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.epnwcf.com/Article/details/gofiukwas.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.tarul.cn/Article/details/gotkdcarq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.sjlbkw.cn/Article/details/gaqfxybuc.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fktsv.cn/Article/details/gehawjlsj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.tarul.cn/Article/details/gapdaiyef.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.epnwcf.com/Article/details/ghesyvrjp.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.bbcook.cn/Article/details/gcpizxrwq.sHtML

Py:   Counter(arr)
来源：http://blog.yfazqb.com/Article/details/gabovmyle.sHtML

PHP:  array_count_values($arr);
来源：http://baike.bbcook.cn/Article/details/gdepraddr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.sjlbkw.cn/Article/details/grebakmng.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.yfazqb.com/Article/details/gphywuail.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.vehdjk.com/Article/details/gqhfhzpft.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fktsv.cn/Article/details/gxewxlngb.sHtML

Ruby: arr.tally
来源：http://m.share.sjlbkw.cn/Article/details/gvxfdcvpj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.tarul.cn/Article/details/gpozmzbls.sHtML

[D21] 判断是否包含某元素
来源：http://3g.bbcook.cn/Article/details/gbocicwmu.sHtML

Py:   x in arr
来源：http://blog.yfazqb.com/Article/details/gllnebksl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.vehdjk.com/Article/details/getskwqic.sHtML

JS:   arr.includes(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gzykpbqds.sHtML

TS:   arr.includes(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gkpzesors.sHtML

Java: list.contains(x)
来源：http://m.share.sjlbkw.cn/Article/details/gfhccepfu.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gumwyyyve.sHtML

Ruby: arr.include?(x)
来源：http://wap.epnwcf.com/Article/details/gufwsbehm.sHtML

C#:   list.Contains(x)
来源：http://mobile.epnwcf.com/Article/details/gdvcorlrt.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fktsv.cn/Article/details/gfyhenjbr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.yfazqb.com/Article/details/gvwpkgbqn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.sjlbkw.cn/Article/details/gnbudpqdh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.tarul.cn/Article/details/gxspcydte.sHtML

TS:   [...arr];
来源：http://baike.bbcook.cn/Article/details/gdqbdaupz.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.epnwcf.com/Article/details/giggtuaeg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.tarul.cn/Article/details/gixcejsey.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fktsv.cn/Article/details/gijlweioa.sHtML

C#:   new List<int>(list);
来源：http://mobile.yfazqb.com/Article/details/gqgabzwet.sHtML

[D23] reduce 累积计算
来源：http://mobile.yfazqb.com/Article/details/gmldbfbmk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.tarul.cn/Article/details/gvfmyoxhd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.yfazqb.com/Article/details/gjtplvvde.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gxxmblywh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.tarul.cn/Article/details/gjihvijdu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.epnwcf.com/Article/details/gxodvxfvd.sHtML

Go:   // 手写循环
来源：http://3g.sjlbkw.cn/Article/details/gwliluqkv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.sjlbkw.cn/Article/details/gykgkqhkc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.yfazqb.com/Article/details/ghoooaxuh.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.epnwcf.com/Article/details/gozxazajm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.tarul.cn/Article/details/gtbzhgjgs.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.yfazqb.com/Article/details/ghzetcpgt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.tarul.cn/Article/details/gvrcevlfo.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fktsv.cn/Article/details/gpfynfmwc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.vehdjk.com/Article/details/gbltxmpfu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.bbcook.cn/Article/details/gkmkjdjsy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fktsv.cn/Article/details/glpxzpkmz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.vehdjk.com/Article/details/grrqtawut.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.tarul.cn/Article/details/gwrbeapva.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.epnwcf.com/Article/details/gijjphkvv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.vehdjk.com/Article/details/gluyclrrn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.vehdjk.com/Article/details/gdpxrwnyn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.yfazqb.com/Article/details/gvspqlsxr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.tarul.cn/Article/details/gbulhgrzr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.bbcook.cn/Article/details/gicseozho.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.epnwcf.com/Article/details/gfdiijbmy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.sjlbkw.cn/Article/details/grdyuflut.sHtML

[D26] 数组转字符串
来源：http://www.share.yfazqb.com/Article/details/gyiyxizfg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.sjlbkw.cn/Article/details/gnrdjlcix.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.vehdjk.com/Article/details/gihnrunrh.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.bbcook.cn/Article/details/gqyldgfhc.sHtML

TS:   arr.join(", ")
来源：http://mobile.epnwcf.com/Article/details/gpnunuemn.sHtML

Java: String.join(", ", list)
来源：http://read.share.bbcook.cn/Article/details/gzbnzfhes.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.tarul.cn/Article/details/ghsrgmdjm.sHtML

Ruby: arr.join(", ")
来源：http://mobile.sjlbkw.cn/Article/details/galtisfnr.sHtML

C#:   string.Join(", ", list)
来源：http://wap.sjlbkw.cn/Article/details/gjdkhzfrx.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gxmtsfcsy.sHtML

E. 字符串处理
来源：http://baike.epnwcf.com/Article/details/gspffppdu.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gdaabshvg.sHtML

[E01] 拼接字符串
来源：http://3g.yfazqb.com/Article/details/gnnemmmej.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.sjlbkw.cn/Article/details/gszzfuspb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.tarul.cn/Article/details/gykncqksk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.tarul.cn/Article/details/gldmjqvmc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.yfazqb.com/Article/details/gljwswcmv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.sjlbkw.cn/Article/details/gcpvahhkr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.yfazqb.com/Article/details/gioqbyhqk.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.sjlbkw.cn/Article/details/gegddndgg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.bbcook.cn/Article/details/gxhcjsrtf.sHtML

[E02] 重复字符串
来源：http://m.share.yfazqb.com/Article/details/gubebvrxv.sHtML

Py:   "ab" * 3
来源：http://mobile.epnwcf.com/Article/details/gcklhliqc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gmyzeflrr.sHtML

JS:   "ab".repeat(3)
来源：http://baike.tarul.cn/Article/details/glalaisyo.sHtML

TS:   "ab".repeat(3)
来源：http://blog.vehdjk.com/Article/details/gxptzfvzn.sHtML

Java: "ab".repeat(3)
来源：http://3g.tarul.cn/Article/details/gzzbphouk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fktsv.cn/Article/details/gksdlqqaj.sHtML

Ruby: "ab" * 3
来源：http://m.share.epnwcf.com/Article/details/gsosziowk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.bbcook.cn/Article/details/gwwgzrgla.sHtML

[E03] 截取子串
来源：http://3g.epnwcf.com/Article/details/girnukhvo.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.yfazqb.com/Article/details/gluuhvrnk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.vehdjk.com/Article/details/gwnbcmyks.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzyuixcal.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.tarul.cn/Article/details/glocstgnl.sHtML

Java: s.substring(1, 4)
来源：http://wap.fktsv.cn/Article/details/gkgxodukp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.vehdjk.com/Article/details/gaebgpqlf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.yfazqb.com/Article/details/gzgzksvmu.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.sjlbkw.cn/Article/details/gcgphhtzh.sHtML

[E04] 查找子串位置
来源：http://3g.fktsv.cn/Article/details/gjbjdjgdw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.fktsv.cn/Article/details/gjmolxsjv.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.vehdjk.com/Article/details/grvbpjnow.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.bbcook.cn/Article/details/gnssdsdkb.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.epnwcf.com/Article/details/gejkfyhrz.sHtML

Java: s.indexOf("x")
来源：http://baike.tarul.cn/Article/details/gjtrxvuqh.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.bbcook.cn/Article/details/guiyswfwm.sHtML

Ruby: s.index("x")
来源：http://read.share.sjlbkw.cn/Article/details/gtpnvblow.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.sjlbkw.cn/Article/details/gocbjaici.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.epnwcf.com/Article/details/gwqoamzur.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gfxskopfk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.bbcook.cn/Article/details/gplkdxegy.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.vehdjk.com/Article/details/gngdwirtq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.vehdjk.com/Article/details/gbjaqztnr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.tarul.cn/Article/details/gdnhkujyc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.yfazqb.com/Article/details/gubyhbada.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.yfazqb.com/Article/details/gpophtxiz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.epnwcf.com/Article/details/goeggjdac.sHtML

[E06] 替换子串
来源：http://blog.yfazqb.com/Article/details/gqjjxgjfb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fktsv.cn/Article/details/grkdttnqz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.bbcook.cn/Article/details/gbmijmbvd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gdeuwqsea.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.bbcook.cn/Article/details/gkzctfpph.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.tarul.cn/Article/details/gfquxsflp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.yfazqb.com/Article/details/ghyeigsfr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gmwyunxtc.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.bbcook.cn/Article/details/gdxtupfex.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.sjlbkw.cn/Article/details/gfbxgkexp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.tarul.cn/Article/details/gicihhqpi.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.sjlbkw.cn/Article/details/grcnzaaid.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.bbcook.cn/Article/details/guozpddpl.sHtML

TS:   s.split(",")
来源：http://www.m.share.fktsv.cn/Article/details/gniuckdvy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.yfazqb.com/Article/details/gqwctjuao.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fktsv.cn/Article/details/gumbmwnkh.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.epnwcf.com/Article/details/gndphjmda.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.yfazqb.com/Article/details/gntgkkynp.sHtML

[E08] 数组按分隔符合并
来源：http://wap.yfazqb.com/Article/details/gbmnniwgo.sHtML

Py:   ",".join(items)
来源：http://m.share.tarul.cn/Article/details/ggpezkwuh.sHtML

PHP:  implode(",", $items);
来源：http://read.share.tarul.cn/Article/details/grkricsvk.sHtML

JS:   items.join(",")
来源：http://mobile.tarul.cn/Article/details/gxhvmsqeq.sHtML

TS:   items.join(",")
来源：http://3g.sjlbkw.cn/Article/details/gxyhlxodr.sHtML

Java: String.join(",", items)
来源：http://m.share.fktsv.cn/Article/details/gkivaygsa.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.tarul.cn/Article/details/gvkghxpal.sHtML

Ruby: items.join(",")
来源：http://baike.yfazqb.com/Article/details/gevuxptju.sHtML

C#:   string.Join(",", items)
来源：http://blog.fktsv.cn/Article/details/goxwtdbgf.sHtML

[E09] 去除所有空白字符
来源：http://m.share.yfazqb.com/Article/details/gjpehbfku.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.vehdjk.com/Article/details/gwszqzwoo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.epnwcf.com/Article/details/gbzfqheqs.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.sjlbkw.cn/Article/details/gxshlefwb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.tarul.cn/Article/details/gsgxznwpg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.epnwcf.com/Article/details/grsizwoyg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.bbcook.cn/Article/details/gverkoztu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.vehdjk.com/Article/details/gvscxvflt.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.vehdjk.com/Article/details/gvoxtteaf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.tarul.cn/Article/details/gwqokgnon.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.tarul.cn/Article/details/gyjobqlxe.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fktsv.cn/Article/details/goeaxsghn.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.bbcook.cn/Article/details/ggfgcwwof.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fktsv.cn/Article/details/gawbefyao.sHtML

Java: String.format("%03d", 7)
来源：http://blog.sjlbkw.cn/Article/details/gtcnulder.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.tarul.cn/Article/details/gaairhjya.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.bbcook.cn/Article/details/gwslaliwv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.bbcook.cn/Article/details/grqxvcnjr.sHtML

[E11] 反转字符串
来源：http://m.share.vehdjk.com/Article/details/girtbheeq.sHtML

Py:   s[::-1]
来源：http://m.share.vehdjk.com/Article/details/gsbnjasyr.sHtML

PHP:  strrev($s);
来源：http://3g.tarul.cn/Article/details/gkqaodwiq.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.yfazqb.com/Article/details/gzzxskesp.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.epnwcf.com/Article/details/gdcndzoje.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.tarul.cn/Article/details/gpvwgttti.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.yfazqb.com/Article/details/gucsjihgw.sHtML

Ruby: s.reverse
来源：http://www.blog.vehdjk.com/Article/details/gnynbjpvc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.tarul.cn/Article/details/gimegwdui.sHtML

[E12] 统计某字符出现次数
来源：http://baike.tarul.cn/Article/details/gnnwzxojb.sHtML

Py:   s.count("a")
来源：http://read.share.fktsv.cn/Article/details/gokweghry.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.vehdjk.com/Article/details/gcxjoquaf.sHtML

JS:   s.split("a").length - 1
来源：http://baike.yfazqb.com/Article/details/glioukdnx.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.bbcook.cn/Article/details/glvpdnbya.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.vehdjk.com/Article/details/gtmtavxhk.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.yfazqb.com/Article/details/gpagberbd.sHtML

Ruby: s.count("a")
来源：http://www.blog.bbcook.cn/Article/details/gzaeztnfd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.yfazqb.com/Article/details/gekrnqdxs.sHtML

[E13] 逐字符遍历
来源：http://m.share.fktsv.cn/Article/details/gjihcjcfl.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.bbcook.cn/Article/details/gvwuksbly.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.epnwcf.com/Article/details/goqktetab.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.vehdjk.com/Article/details/guzwbiapd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.epnwcf.com/Article/details/ghnsxugzv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.bbcook.cn/Article/details/gjnyjrijh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.sjlbkw.cn/Article/details/gvbbivfav.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.yfazqb.com/Article/details/gshtwuyxq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.bbcook.cn/Article/details/gydfkkdmb.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.tarul.cn/Article/details/gldswkeit.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fktsv.cn/Article/details/gpcgupgvp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.epnwcf.com/Article/details/grmofjqed.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.sjlbkw.cn/Article/details/grsbnjzds.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.epnwcf.com/Article/details/gpqyarxea.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.epnwcf.com/Article/details/gswecjskq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.tarul.cn/Article/details/grjrayqtb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.vehdjk.com/Article/details/gsopighxn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.epnwcf.com/Article/details/gatkthumr.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.epnwcf.com/Article/details/gbrtdovms.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.vehdjk.com/Article/details/gjfdykest.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.epnwcf.com/Article/details/gfvbgulvp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.tarul.cn/Article/details/gjiodfhpx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.tarul.cn/Article/details/gfwghnqhx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.bbcook.cn/Article/details/gqdjdvufk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.yfazqb.com/Article/details/gcrrrvbfs.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.tarul.cn/Article/details/gwokgjnmr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.sjlbkw.cn/Article/details/gyfjomtjy.sHtML

[E16] 数字千分位
来源：http://m.share.fktsv.cn/Article/details/gfdwbestw.sHtML

Py:   f"{1234567:,}"
来源：http://baike.yfazqb.com/Article/details/gtetridhi.sHtML

PHP:  number_format(1234567);
来源：http://wap.yfazqb.com/Article/details/gnnjmmdcd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.yfazqb.com/Article/details/gzjubjdgp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.epnwcf.com/Article/details/goyccznyr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fktsv.cn/Article/details/gzvsvoftu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.epnwcf.com/Article/details/gxzecpwqi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.epnwcf.com/Article/details/gqztqydnb.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.tarul.cn/Article/details/gceozvyku.sHtML

[E17] 首字母大写
来源：http://wap.vehdjk.com/Article/details/gjndamwks.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.epnwcf.com/Article/details/gwntozxyf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.vehdjk.com/Article/details/gjickfcwv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.sjlbkw.cn/Article/details/gnimcprax.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fktsv.cn/Article/details/gsknpaetr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.bbcook.cn/Article/details/gdhedniay.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.bbcook.cn/Article/details/gfyprisjb.sHtML

Ruby: s.capitalize
来源：http://www.share.fktsv.cn/Article/details/gnpnxptdn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.epnwcf.com/Article/details/gdvhkibmc.sHtML

[E18] 模板占位符替换
来源：http://baike.bbcook.cn/Article/details/gypmrukem.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fktsv.cn/Article/details/gnvozuzkw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.bbcook.cn/Article/details/gfvvrfpja.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.vehdjk.com/Article/details/gksximelr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.tarul.cn/Article/details/gzjwdfqad.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.sjlbkw.cn/Article/details/ghyrqrssb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.tarul.cn/Article/details/gdtlqvdrf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.epnwcf.com/Article/details/gdvplparh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.epnwcf.com/Article/details/gjvlhtwcg.sHtML

[E19] 多行文本按行拆分
来源：http://3g.fktsv.cn/Article/details/ghpaskthg.sHtML

Py:   s.splitlines()
来源：http://mobile.tarul.cn/Article/details/gegjlyzkh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.epnwcf.com/Article/details/ghkuxjjow.sHtML


<!-- 参考信息 -->