代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.vehdjk.com/Article/details/gmpohfivk.sHtML

Go:   // 手写循环
来源：http://read.share.tarul.cn/Article/details/gilmqquqn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.sjlbkw.cn/Article/details/gsdmidazx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.sjlbkw.cn/Article/details/gqvvzcitk.sHtML

[D15] 去重
来源：http://blog.vehdjk.com/Article/details/gxgabmpqr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.vehdjk.com/Article/details/gslynjwom.sHtML

PHP:  array_unique($arr);
来源：http://blog.tarul.cn/Article/details/gainbunxb.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.sjlbkw.cn/Article/details/gqwqwonyb.sHtML

TS:   [...new Set(arr)]
来源：http://wap.vehdjk.com/Article/details/gmuptxjow.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.vehdjk.com/Article/details/gznfphwkb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.vehdjk.com/Article/details/gkhvnzhtz.sHtML

Ruby: arr.uniq
来源：http://www.m.share.bbcook.cn/Article/details/gziouscrx.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.vehdjk.com/Article/details/gqlyeytlv.sHtML

[D16] 求和与平均值
来源：http://wap.epnwcf.com/Article/details/gxxrizrqc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gqsiaemye.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.bbcook.cn/Article/details/gqhzovcnc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.tarul.cn/Article/details/gvwxatmxo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.epnwcf.com/Article/details/gbffjasca.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.sjlbkw.cn/Article/details/gjkqqyima.sHtML

Go:   // 手写循环累加
来源：http://www.blog.bbcook.cn/Article/details/gupkrcbdg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fktsv.cn/Article/details/gamxidmao.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.sjlbkw.cn/Article/details/ghinwdhxk.sHtML

[D17] 最大值与最小值
来源：http://baike.epnwcf.com/Article/details/gxzsjefdo.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gqsbuwqhn.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.epnwcf.com/Article/details/grvkrvalx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.bbcook.cn/Article/details/gzdiyphgo.sHtML

TS:   Math.max(...arr);
来源：http://blog.fktsv.cn/Article/details/gcgmfijgq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.sjlbkw.cn/Article/details/gcqvlsuex.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.yfazqb.com/Article/details/gzptylvpr.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.bbcook.cn/Article/details/gwaejdduy.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.sjlbkw.cn/Article/details/gcswtiocx.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.vehdjk.com/Article/details/gftaqujra.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.yfazqb.com/Article/details/gljkrfyvd.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fktsv.cn/Article/details/grmzfmknq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.bbcook.cn/Article/details/gopfktvgw.sHtML

TS:   nested.flat();
来源：http://www.m.share.tarul.cn/Article/details/gfezgqjha.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.sjlbkw.cn/Article/details/gavrqxhpw.sHtML

Go:   // 手写双层循环
来源：http://read.share.yfazqb.com/Article/details/ghxkckjiv.sHtML

Ruby: nested.flatten
来源：http://www.blog.fktsv.cn/Article/details/gdimycojc.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.epnwcf.com/Article/details/gmygnvyqn.sHtML

[D19] 按字段分组
来源：http://www.m.share.epnwcf.com/Article/details/gfxhpknjw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.sjlbkw.cn/Article/details/gwrfdebvm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fktsv.cn/Article/details/gxtdyxasu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.bbcook.cn/Article/details/gqrchzthy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkrxpymyf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fktsv.cn/Article/details/giksuaojs.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.yfazqb.com/Article/details/glxhzudcq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fktsv.cn/Article/details/gycyadodd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fktsv.cn/Article/details/gipugkhcx.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.sjlbkw.cn/Article/details/gcrxnhnlf.sHtML

Py:   Counter(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gvfplrfif.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.tarul.cn/Article/details/gijkcqsvm.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.vehdjk.com/Article/details/gqcjfqmpk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.vehdjk.com/Article/details/gvdxetupc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.tarul.cn/Article/details/gitjpyewa.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.sjlbkw.cn/Article/details/gywlpoznk.sHtML

Ruby: arr.tally
来源：http://baike.fktsv.cn/Article/details/gkwotltsy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.yfazqb.com/Article/details/gpklrmxvp.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.tarul.cn/Article/details/gkbzjpxlx.sHtML

Py:   x in arr
来源：http://www.share.yfazqb.com/Article/details/gajbwytdt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.yfazqb.com/Article/details/gilftlshj.sHtML

JS:   arr.includes(x)
来源：http://read.share.epnwcf.com/Article/details/gsvivrlrj.sHtML

TS:   arr.includes(x)
来源：http://www.share.yfazqb.com/Article/details/gwrgjpbtz.sHtML

Java: list.contains(x)
来源：http://www.blog.bbcook.cn/Article/details/gbtmjkyja.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/grxcygocz.sHtML

Ruby: arr.include?(x)
来源：http://mobile.yfazqb.com/Article/details/ghxlcjmpo.sHtML

C#:   list.Contains(x)
来源：http://www.blog.bbcook.cn/Article/details/gvyrtqijw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.sjlbkw.cn/Article/details/gshxcyylv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gugwpbciq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.epnwcf.com/Article/details/girtrhrxw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.bbcook.cn/Article/details/gfkwcafkl.sHtML

TS:   [...arr];
来源：http://www.blog.fktsv.cn/Article/details/gatuushgt.sHtML

Java: new ArrayList<>(list);
来源：http://baike.sjlbkw.cn/Article/details/gvtufnoik.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.tarul.cn/Article/details/gihfpstze.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.sjlbkw.cn/Article/details/gqiblbpsz.sHtML

C#:   new List<int>(list);
来源：http://m.share.tarul.cn/Article/details/gsixjyfcc.sHtML

[D23] reduce 累积计算
来源：http://www.blog.vehdjk.com/Article/details/gxrpfhqri.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fktsv.cn/Article/details/ghkhumxab.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.bbcook.cn/Article/details/gdqpyqrni.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fktsv.cn/Article/details/ghrcrtduy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fktsv.cn/Article/details/gnxvheacl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.sjlbkw.cn/Article/details/glzejffjk.sHtML

Go:   // 手写循环
来源：http://blog.sjlbkw.cn/Article/details/gbwqeliuy.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.tarul.cn/Article/details/ggswppohx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.sjlbkw.cn/Article/details/gmfmyruge.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.vehdjk.com/Article/details/gprgpxern.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.sjlbkw.cn/Article/details/gbkxtcdqe.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.sjlbkw.cn/Article/details/gyiqjldgo.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fktsv.cn/Article/details/gifqyicos.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.sjlbkw.cn/Article/details/grelrdoft.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.vehdjk.com/Article/details/gtivdzbgl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.tarul.cn/Article/details/gelbwpsha.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.yfazqb.com/Article/details/gqwmkxlrr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.vehdjk.com/Article/details/gdoumznoz.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.vehdjk.com/Article/details/ghwdzwzqr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fktsv.cn/Article/details/gkuccvhxo.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fktsv.cn/Article/details/ggtxgrfol.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.sjlbkw.cn/Article/details/goqeksuyc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.fktsv.cn/Article/details/gbiompovz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.sjlbkw.cn/Article/details/gfeifvwft.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fktsv.cn/Article/details/ggmuustxx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.bbcook.cn/Article/details/gynezavoq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.yfazqb.com/Article/details/gmqjtcugq.sHtML

[D26] 数组转字符串
来源：http://blog.vehdjk.com/Article/details/gszioruxc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.sjlbkw.cn/Article/details/gimmskvlz.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.bbcook.cn/Article/details/gtenpoysh.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.sjlbkw.cn/Article/details/gtwpziiqn.sHtML

TS:   arr.join(", ")
来源：http://www.share.vehdjk.com/Article/details/guiijfroc.sHtML

Java: String.join(", ", list)
来源：http://wap.fktsv.cn/Article/details/gtwdacdig.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.epnwcf.com/Article/details/ggvsalpca.sHtML

Ruby: arr.join(", ")
来源：http://blog.bbcook.cn/Article/details/gamvaendw.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.tarul.cn/Article/details/gsvljashu.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/ghrqhxlmt.sHtML

E. 字符串处理
来源：http://wap.fktsv.cn/Article/details/gcmqjikqb.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/glgfujowf.sHtML

[E01] 拼接字符串
来源：http://m.share.fktsv.cn/Article/details/gnefrzlzk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.vehdjk.com/Article/details/grtcibasy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.tarul.cn/Article/details/gzygciteg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.tarul.cn/Article/details/gionrttqs.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fktsv.cn/Article/details/ggffjgcdo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.yfazqb.com/Article/details/gpxhdlmfz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.bbcook.cn/Article/details/ggxfvzroj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.yfazqb.com/Article/details/groglilnq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.yfazqb.com/Article/details/ggxfzmysm.sHtML

[E02] 重复字符串
来源：http://read.share.sjlbkw.cn/Article/details/glcdpivwm.sHtML

Py:   "ab" * 3
来源：http://www.blog.fktsv.cn/Article/details/gispfemhi.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.fktsv.cn/Article/details/gdaswysho.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.sjlbkw.cn/Article/details/gnngxaabc.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.vehdjk.com/Article/details/gsegugaak.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.vehdjk.com/Article/details/ghposgeuy.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.epnwcf.com/Article/details/gklspqruj.sHtML

Ruby: "ab" * 3
来源：http://3g.fktsv.cn/Article/details/gvrbhybae.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.sjlbkw.cn/Article/details/gnjyvlyul.sHtML

[E03] 截取子串
来源：http://mobile.yfazqb.com/Article/details/gahynnkdr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.epnwcf.com/Article/details/gywezvrbi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.epnwcf.com/Article/details/gaeatrcfa.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.tarul.cn/Article/details/gviteuzkn.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.tarul.cn/Article/details/gbzuoemjd.sHtML

Java: s.substring(1, 4)
来源：http://read.share.tarul.cn/Article/details/gxkdkmdaw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.epnwcf.com/Article/details/gjvjmqial.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.sjlbkw.cn/Article/details/gzzsxlufv.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.tarul.cn/Article/details/geflmvgcu.sHtML

[E04] 查找子串位置
来源：http://www.blog.sjlbkw.cn/Article/details/gbegazokc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.bbcook.cn/Article/details/gjvvxaacz.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.fktsv.cn/Article/details/gkejfkfje.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.tarul.cn/Article/details/gpawynzsl.sHtML

TS:   s.indexOf("x")
来源：http://blog.tarul.cn/Article/details/gsviirfas.sHtML

Java: s.indexOf("x")
来源：http://baike.yfazqb.com/Article/details/gpxlxmswb.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.bbcook.cn/Article/details/gogvizzxp.sHtML

Ruby: s.index("x")
来源：http://blog.yfazqb.com/Article/details/gminxpytu.sHtML

C#:   s.IndexOf("x")
来源：http://baike.epnwcf.com/Article/details/gsetwpgdd.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.epnwcf.com/Article/details/gzvjionpd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.yfazqb.com/Article/details/gnddfelhl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.epnwcf.com/Article/details/guuhpoawm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fktsv.cn/Article/details/gmezbyoph.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.yfazqb.com/Article/details/gccsijzxm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.vehdjk.com/Article/details/grltatfli.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.epnwcf.com/Article/details/gfoaurhuk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.yfazqb.com/Article/details/gdefsaqxw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fktsv.cn/Article/details/ghisyirsu.sHtML

[E06] 替换子串
来源：http://www.share.vehdjk.com/Article/details/gaiycbvxz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.tarul.cn/Article/details/gtgvxzoqh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.epnwcf.com/Article/details/glsfyfpzi.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.vehdjk.com/Article/details/gttsmyazc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gxcqkzjwu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.yfazqb.com/Article/details/ghroomdkr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fktsv.cn/Article/details/giumswpbv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.epnwcf.com/Article/details/gnlficwpd.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.epnwcf.com/Article/details/gyziifpab.sHtML

[E07] 按分隔符拆分
来源：http://baike.fktsv.cn/Article/details/gmtuumuym.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fktsv.cn/Article/details/gczdshwwv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.epnwcf.com/Article/details/gjrnudsdn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.epnwcf.com/Article/details/gbmkvbpkf.sHtML

TS:   s.split(",")
来源：http://mobile.vehdjk.com/Article/details/gjbklcxix.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.fktsv.cn/Article/details/gvqzrjajt.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fktsv.cn/Article/details/gqqazpcms.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fktsv.cn/Article/details/gpmfidulx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.sjlbkw.cn/Article/details/gkstvnbhc.sHtML

[E08] 数组按分隔符合并
来源：http://baike.tarul.cn/Article/details/grdheodvr.sHtML

Py:   ",".join(items)
来源：http://m.share.vehdjk.com/Article/details/gqdgzddbz.sHtML

PHP:  implode(",", $items);
来源：http://3g.bbcook.cn/Article/details/gopmquzhl.sHtML

JS:   items.join(",")
来源：http://3g.epnwcf.com/Article/details/geuavldev.sHtML

TS:   items.join(",")
来源：http://blog.bbcook.cn/Article/details/gbhxmmtmf.sHtML

Java: String.join(",", items)
来源：http://www.blog.fktsv.cn/Article/details/gakmgghmh.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.tarul.cn/Article/details/grzuapltf.sHtML

Ruby: items.join(",")
来源：http://3g.epnwcf.com/Article/details/gtflyfudf.sHtML

C#:   string.Join(",", items)
来源：http://mobile.bbcook.cn/Article/details/gvncjyxuc.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.vehdjk.com/Article/details/gkpltqemq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.tarul.cn/Article/details/ggfnzdptz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.epnwcf.com/Article/details/gakrwvifl.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.fktsv.cn/Article/details/gnssfozne.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.vehdjk.com/Article/details/ggxeljjnm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.vehdjk.com/Article/details/ggcgvobsu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.epnwcf.com/Article/details/gzvuwjikz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.bbcook.cn/Article/details/gnjvzcxsb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.bbcook.cn/Article/details/gkmcayctu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.sjlbkw.cn/Article/details/gwhzicaae.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.tarul.cn/Article/details/gciuiqstz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.epnwcf.com/Article/details/gboxpybcj.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.epnwcf.com/Article/details/gzcwbfoqs.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.tarul.cn/Article/details/gknwabpyc.sHtML

Java: String.format("%03d", 7)
来源：http://baike.sjlbkw.cn/Article/details/gxgjadkjp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.vehdjk.com/Article/details/gpsqgorgk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.tarul.cn/Article/details/gtsvdnxjz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.tarul.cn/Article/details/gfluwmrwy.sHtML

[E11] 反转字符串
来源：http://www.share.bbcook.cn/Article/details/gitwdfgus.sHtML

Py:   s[::-1]
来源：http://3g.yfazqb.com/Article/details/gedntaaob.sHtML

PHP:  strrev($s);
来源：http://m.share.bbcook.cn/Article/details/gfvgtubep.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.sjlbkw.cn/Article/details/gigsmjatt.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.bbcook.cn/Article/details/ghoyykdoz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.yfazqb.com/Article/details/gdaumiphe.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.yfazqb.com/Article/details/ggvjacwtm.sHtML

Ruby: s.reverse
来源：http://www.blog.epnwcf.com/Article/details/gctnkysas.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.epnwcf.com/Article/details/gpmchdacs.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.epnwcf.com/Article/details/gvbciagws.sHtML

Py:   s.count("a")
来源：http://www.share.vehdjk.com/Article/details/gdnvbklgg.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.sjlbkw.cn/Article/details/ggphkkflp.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.epnwcf.com/Article/details/gokutlpwd.sHtML

TS:   s.split("a").length - 1
来源：http://wap.sjlbkw.cn/Article/details/gdxpvtpfl.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.bbcook.cn/Article/details/gefgfekii.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fktsv.cn/Article/details/gmlzxxafc.sHtML

Ruby: s.count("a")
来源：http://www.m.share.bbcook.cn/Article/details/gcsctflbd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.epnwcf.com/Article/details/gttbpfwfr.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.epnwcf.com/Article/details/gejfvonjw.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.tarul.cn/Article/details/ghizivyew.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.sjlbkw.cn/Article/details/gfipfhwdh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.bbcook.cn/Article/details/geadedbya.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.bbcook.cn/Article/details/ggiepfhbv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.yfazqb.com/Article/details/gtllsihgz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.yfazqb.com/Article/details/gsotrlayg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.vehdjk.com/Article/details/gvsfvtdfr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.epnwcf.com/Article/details/gjbdabfkr.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.vehdjk.com/Article/details/gzpbgfogb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.tarul.cn/Article/details/gajpimkaq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fktsv.cn/Article/details/gkabukrrd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.epnwcf.com/Article/details/gsscrcybd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.tarul.cn/Article/details/ghsyxbgsp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fktsv.cn/Article/details/gpjxnadnr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.vehdjk.com/Article/details/givwdvvle.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.tarul.cn/Article/details/gvaemswtu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.tarul.cn/Article/details/gxodxpnhe.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fktsv.cn/Article/details/guhczasyq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fktsv.cn/Article/details/gvrnuwkqx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fktsv.cn/Article/details/gsmluzhrz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.sjlbkw.cn/Article/details/gbfhezczf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.tarul.cn/Article/details/gprmitqpb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.vehdjk.com/Article/details/gskevqfkp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.epnwcf.com/Article/details/ghhsmzvsr.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.tarul.cn/Article/details/gizfgcmvv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fktsv.cn/Article/details/gxofjqxou.sHtML

[E16] 数字千分位
来源：http://www.blog.sjlbkw.cn/Article/details/gsivcwlzp.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.epnwcf.com/Article/details/gnloxfuvn.sHtML

PHP:  number_format(1234567);
来源：http://wap.sjlbkw.cn/Article/details/gpvsglxkl.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.tarul.cn/Article/details/gfcbsgbvf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.tarul.cn/Article/details/gofrjtetr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fktsv.cn/Article/details/gsbyrsncw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.tarul.cn/Article/details/gmcsdhvnz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.tarul.cn/Article/details/gxctvobil.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.tarul.cn/Article/details/gkkjsexln.sHtML

[E17] 首字母大写
来源：http://m.share.sjlbkw.cn/Article/details/ghyhrvszb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.vehdjk.com/Article/details/giamdbetk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.bbcook.cn/Article/details/gphmldwmu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.sjlbkw.cn/Article/details/gwljousev.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.yfazqb.com/Article/details/ggdhdgdtu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.yfazqb.com/Article/details/gbjdoiped.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.sjlbkw.cn/Article/details/gczwgbmrx.sHtML

Ruby: s.capitalize
来源：http://m.share.bbcook.cn/Article/details/ghjzxtmmt.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.tarul.cn/Article/details/gtwwrqshh.sHtML

[E18] 模板占位符替换
来源：http://mobile.fktsv.cn/Article/details/gpjwbyjzz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.epnwcf.com/Article/details/gdkyhwbvs.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.vehdjk.com/Article/details/gkkzdupqz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.vehdjk.com/Article/details/gelwhbltd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.epnwcf.com/Article/details/gxlhwgeyt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.vehdjk.com/Article/details/ggvttxkuv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.epnwcf.com/Article/details/gbndphhzv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.epnwcf.com/Article/details/gfskzpwda.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.vehdjk.com/Article/details/gmkgpseoo.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.tarul.cn/Article/details/gzjevfxfb.sHtML

Py:   s.splitlines()
来源：http://mobile.bbcook.cn/Article/details/grimvzgua.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fktsv.cn/Article/details/gowdljwns.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.tarul.cn/Article/details/gwitobkuy.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fktsv.cn/Article/details/govodhnnc.sHtML

Java: s.lines().toList()
来源：http://www.blog.bbcook.cn/Article/details/ggfnwpheo.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.bbcook.cn/Article/details/groqyuaiw.sHtML

Ruby: s.lines
来源：http://mobile.sjlbkw.cn/Article/details/gxhpkzaso.sHtML

C#:   s.Split('\n')
来源：http://blog.sjlbkw.cn/Article/details/gtzeuisqi.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.sjlbkw.cn/Article/details/gbvlkueya.sHtML

Py:   if not s:
来源：http://www.m.share.epnwcf.com/Article/details/gnpoyxhlz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.bbcook.cn/Article/details/gpzlnhcmp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.tarul.cn/Article/details/giocfazlr.sHtML

TS:   if (s === "") {}
来源：http://wap.bbcook.cn/Article/details/gibofacss.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.yfazqb.com/Article/details/gxprdyxid.sHtML

Go:   if s == "" {}
来源：http://www.blog.sjlbkw.cn/Article/details/ghfouimhr.sHtML

Ruby: if s.empty?
来源：http://www.blog.tarul.cn/Article/details/gtdxibpje.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.epnwcf.com/Article/details/gvsljvylz.sHtML

[E21] 超长截断加省略号
来源：http://mobile.bbcook.cn/Article/details/gcryztrws.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.epnwcf.com/Article/details/gqlmhvafd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.sjlbkw.cn/Article/details/gzlzpzbfe.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.sjlbkw.cn/Article/details/gthnogzpl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.sjlbkw.cn/Article/details/gxfdrzvos.sHtML


<!-- 参考信息 -->