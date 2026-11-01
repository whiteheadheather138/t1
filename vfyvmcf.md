代发 wailian999

C#:   list.Reverse();
来源：http://3g.epnwcf.com/Article/details/gsuzmecbr.sHtML

[D12] 查找元素下标
来源：http://3g.bbcook.cn/Article/details/giupetfrx.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.sjlbkw.cn/Article/details/geuzfmpnk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.tarul.cn/Article/details/gxytzugzh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fktsv.cn/Article/details/gjmoziiez.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.bbcook.cn/Article/details/gcqztcpdf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.yfazqb.com/Article/details/gpvgtgdwo.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gwjcaonzg.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.epnwcf.com/Article/details/gpjipuadq.sHtML

C#:   list.IndexOf(x);
来源：http://wap.sjlbkw.cn/Article/details/gufteldln.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.tarul.cn/Article/details/gsxuymkya.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fktsv.cn/Article/details/gdndoyusi.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.epnwcf.com/Article/details/gdnxswckl.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fktsv.cn/Article/details/gisxdzubm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.bbcook.cn/Article/details/gldusosdf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.vehdjk.com/Article/details/gmwltjvml.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.sjlbkw.cn/Article/details/gfnpjrllh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.vehdjk.com/Article/details/gckjoysld.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.vehdjk.com/Article/details/gofmfymkf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.epnwcf.com/Article/details/gcspcvmas.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.bbcook.cn/Article/details/gevesyvmo.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.epnwcf.com/Article/details/goxabkmxx.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.bbcook.cn/Article/details/gzrcwekdn.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.vehdjk.com/Article/details/gschuqzdc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.tarul.cn/Article/details/goatnfyfd.sHtML

Go:   // 手写循环
来源：http://baike.fktsv.cn/Article/details/gvnnftkei.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.sjlbkw.cn/Article/details/gazlfdxjk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.yfazqb.com/Article/details/gdycoskqy.sHtML

[D15] 去重
来源：http://www.share.vehdjk.com/Article/details/gjzvclwce.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.yfazqb.com/Article/details/gmlmcplwe.sHtML

PHP:  array_unique($arr);
来源：http://baike.yfazqb.com/Article/details/guxpmrtat.sHtML

JS:   [...new Set(arr)]
来源：http://baike.bbcook.cn/Article/details/gysmjlsml.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.tarul.cn/Article/details/gczpgcwws.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fktsv.cn/Article/details/gnovltenl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.tarul.cn/Article/details/gdojiqzrh.sHtML

Ruby: arr.uniq
来源：http://3g.bbcook.cn/Article/details/gftxzbbbs.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.yfazqb.com/Article/details/gmermsiqj.sHtML

[D16] 求和与平均值
来源：http://blog.bbcook.cn/Article/details/gkwpnilji.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.vehdjk.com/Article/details/gxvrwticw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.tarul.cn/Article/details/guttcpcsq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.vehdjk.com/Article/details/gyaipmmiz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fktsv.cn/Article/details/gsibxuuzk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.vehdjk.com/Article/details/giimpockr.sHtML

Go:   // 手写循环累加
来源：http://3g.bbcook.cn/Article/details/gzjffmhek.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.vehdjk.com/Article/details/gmtgxvwop.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.vehdjk.com/Article/details/gcxtvdwdb.sHtML

[D17] 最大值与最小值
来源：http://wap.vehdjk.com/Article/details/goumhogul.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.yfazqb.com/Article/details/gqsgqfafe.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.vehdjk.com/Article/details/gvznrvthd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fktsv.cn/Article/details/ggbcihsdx.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fktsv.cn/Article/details/ggvmejnus.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.vehdjk.com/Article/details/gozlffvdi.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.yfazqb.com/Article/details/gywwuovmd.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.tarul.cn/Article/details/givzwnxxi.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fktsv.cn/Article/details/guhgzdhds.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.yfazqb.com/Article/details/gfwpqyzic.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.sjlbkw.cn/Article/details/goocyezhu.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.vehdjk.com/Article/details/gxitqlyek.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.vehdjk.com/Article/details/gzicnjzxm.sHtML

TS:   nested.flat();
来源：http://mobile.epnwcf.com/Article/details/gawotkwpq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.sjlbkw.cn/Article/details/gfjvphxkj.sHtML

Go:   // 手写双层循环
来源：http://mobile.sjlbkw.cn/Article/details/gdtdvxurf.sHtML

Ruby: nested.flatten
来源：http://wap.vehdjk.com/Article/details/goppaqmse.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.bbcook.cn/Article/details/gubkherud.sHtML

[D19] 按字段分组
来源：http://www.blog.vehdjk.com/Article/details/gxelwnpbi.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fktsv.cn/Article/details/gvhvzuuaa.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fktsv.cn/Article/details/gzgdhtzbo.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.tarul.cn/Article/details/gjjvjkuaw.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.sjlbkw.cn/Article/details/gsmduzbwt.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.tarul.cn/Article/details/gunsxgxyw.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.epnwcf.com/Article/details/gkrwumlvi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.bbcook.cn/Article/details/gbhztmdnb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.sjlbkw.cn/Article/details/gzlbootfo.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.bbcook.cn/Article/details/giqhfixkq.sHtML

Py:   Counter(arr)
来源：http://mobile.tarul.cn/Article/details/gppwzpndr.sHtML

PHP:  array_count_values($arr);
来源：http://wap.vehdjk.com/Article/details/gunwhhvjr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.bbcook.cn/Article/details/gsjxybguk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.tarul.cn/Article/details/gpswdcljq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.bbcook.cn/Article/details/grzjujzxy.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.vehdjk.com/Article/details/gigrpksvp.sHtML

Ruby: arr.tally
来源：http://wap.bbcook.cn/Article/details/gtgwwoicy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.epnwcf.com/Article/details/gieynihwn.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.sjlbkw.cn/Article/details/gvrmftkkx.sHtML

Py:   x in arr
来源：http://www.blog.vehdjk.com/Article/details/gvvmztfss.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fktsv.cn/Article/details/gvfffpide.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.vehdjk.com/Article/details/gztlgzulb.sHtML

TS:   arr.includes(x)
来源：http://wap.yfazqb.com/Article/details/gshrlwnli.sHtML

Java: list.contains(x)
来源：http://wap.vehdjk.com/Article/details/gccqfdwka.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.tarul.cn/Article/details/gtgyehusy.sHtML

Ruby: arr.include?(x)
来源：http://mobile.sjlbkw.cn/Article/details/gtzftpqtg.sHtML

C#:   list.Contains(x)
来源：http://read.share.bbcook.cn/Article/details/gpwmuvrel.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.epnwcf.com/Article/details/gomnaaxyz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.tarul.cn/Article/details/gyeymcxlr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.tarul.cn/Article/details/gsmvugybc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fktsv.cn/Article/details/gkiabkpdh.sHtML

TS:   [...arr];
来源：http://mobile.bbcook.cn/Article/details/glfkfijru.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.yfazqb.com/Article/details/gyppvgxum.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.sjlbkw.cn/Article/details/givxonxhu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.epnwcf.com/Article/details/gfxbnxhwb.sHtML

C#:   new List<int>(list);
来源：http://3g.tarul.cn/Article/details/gkbkibnln.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fktsv.cn/Article/details/gufadhitg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.yfazqb.com/Article/details/giapcjubl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.tarul.cn/Article/details/giyorqzjg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.bbcook.cn/Article/details/glqvpicdy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gezphvlau.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.sjlbkw.cn/Article/details/gkeevyfxk.sHtML

Go:   // 手写循环
来源：http://mobile.yfazqb.com/Article/details/gwxteaosj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.yfazqb.com/Article/details/gpnvqipze.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.tarul.cn/Article/details/goppzpngf.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.epnwcf.com/Article/details/geemlpafy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.tarul.cn/Article/details/gwxjqbghx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.sjlbkw.cn/Article/details/gcpoybtrd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.vehdjk.com/Article/details/gpklyoqwj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.yfazqb.com/Article/details/gwcbvyhqz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.epnwcf.com/Article/details/gjyvfeenk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.tarul.cn/Article/details/gkceqethl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.tarul.cn/Article/details/ghiyyopij.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fktsv.cn/Article/details/gwefffedf.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.vehdjk.com/Article/details/geibhhino.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.vehdjk.com/Article/details/gewpdgpgt.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.tarul.cn/Article/details/ghfhsnnuf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.bbcook.cn/Article/details/ghyluptmr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.yfazqb.com/Article/details/gvtvboewt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.bbcook.cn/Article/details/gopuiprep.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.epnwcf.com/Article/details/gfnjtjhwq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.tarul.cn/Article/details/ghekeislp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fktsv.cn/Article/details/gxtaezowj.sHtML

[D26] 数组转字符串
来源：http://m.share.epnwcf.com/Article/details/gejfloljt.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fktsv.cn/Article/details/gmocsmrco.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.yfazqb.com/Article/details/grxrzferc.sHtML

JS:   arr.join(", ")
来源：http://www.share.fktsv.cn/Article/details/gjuupffuc.sHtML

TS:   arr.join(", ")
来源：http://read.share.epnwcf.com/Article/details/gxzdfopnl.sHtML

Java: String.join(", ", list)
来源：http://www.share.fktsv.cn/Article/details/gdjlkklwy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.vehdjk.com/Article/details/gtcowztth.sHtML

Ruby: arr.join(", ")
来源：http://blog.yfazqb.com/Article/details/gzmdmkxkt.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.bbcook.cn/Article/details/gxsalkpgv.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gdbpeayeu.sHtML

E. 字符串处理
来源：http://blog.yfazqb.com/Article/details/ggtcivfnb.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/giptfoktw.sHtML

[E01] 拼接字符串
来源：http://blog.tarul.cn/Article/details/ghtoupnyk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.yfazqb.com/Article/details/gvckemzmx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.sjlbkw.cn/Article/details/gosxavhns.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.tarul.cn/Article/details/gulcmakmk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.sjlbkw.cn/Article/details/gjigubgwz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.yfazqb.com/Article/details/gjdaaqbps.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.yfazqb.com/Article/details/gwqlokqeo.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.sjlbkw.cn/Article/details/guvhdwfyt.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gsubbeuho.sHtML

[E02] 重复字符串
来源：http://www.share.bbcook.cn/Article/details/gnqmjfhxv.sHtML

Py:   "ab" * 3
来源：http://read.share.vehdjk.com/Article/details/gzsvxjrnk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.bbcook.cn/Article/details/gisczshnu.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.bbcook.cn/Article/details/gizsazdvk.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.tarul.cn/Article/details/gszdbyljq.sHtML

Java: "ab".repeat(3)
来源：http://baike.sjlbkw.cn/Article/details/gamkapucj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fktsv.cn/Article/details/gpdjenbrw.sHtML

Ruby: "ab" * 3
来源：http://mobile.tarul.cn/Article/details/gvgtezobr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.epnwcf.com/Article/details/gqsxriijv.sHtML

[E03] 截取子串
来源：http://wap.epnwcf.com/Article/details/gdkhqbnqh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.sjlbkw.cn/Article/details/gktmaicxv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.yfazqb.com/Article/details/gfoaosqho.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.sjlbkw.cn/Article/details/gklcwwhzd.sHtML

TS:   s.slice(1, 4)
来源：http://baike.yfazqb.com/Article/details/guhipwwzj.sHtML

Java: s.substring(1, 4)
来源：http://m.share.vehdjk.com/Article/details/glvlnsxnd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.bbcook.cn/Article/details/gvjingymq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.yfazqb.com/Article/details/gvgrveawf.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.vehdjk.com/Article/details/gtmnhcggt.sHtML

[E04] 查找子串位置
来源：http://wap.fktsv.cn/Article/details/gbtceisad.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fktsv.cn/Article/details/grwzqlbwu.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.tarul.cn/Article/details/gjsjacdsx.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.sjlbkw.cn/Article/details/gvxvdjzch.sHtML

TS:   s.indexOf("x")
来源：http://blog.yfazqb.com/Article/details/gmosyulfu.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fktsv.cn/Article/details/gotkgiola.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.tarul.cn/Article/details/gnptwmwrf.sHtML

Ruby: s.index("x")
来源：http://www.share.yfazqb.com/Article/details/gjibgpdin.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.yfazqb.com/Article/details/gdizwjjkv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.epnwcf.com/Article/details/ghyfxqske.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.bbcook.cn/Article/details/glaahqrle.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.vehdjk.com/Article/details/grywgrzwv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.vehdjk.com/Article/details/gjffklpph.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.epnwcf.com/Article/details/galufzjzt.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.vehdjk.com/Article/details/gdycilevc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.yfazqb.com/Article/details/goqmcepwk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.epnwcf.com/Article/details/gpdkyovcj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.sjlbkw.cn/Article/details/gexxdbnyv.sHtML

[E06] 替换子串
来源：http://baike.sjlbkw.cn/Article/details/gitrmocyq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.vehdjk.com/Article/details/gftrpfjmj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.tarul.cn/Article/details/gbmokkunv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.vehdjk.com/Article/details/glignombn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.vehdjk.com/Article/details/grpcouqrp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gqgmdfnjd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.tarul.cn/Article/details/ghcamniac.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/grndgqggp.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/gvisjikje.sHtML

[E07] 按分隔符拆分
来源：http://baike.epnwcf.com/Article/details/gbfmxujwo.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.yfazqb.com/Article/details/gdfzduonz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gbvlzvngk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fktsv.cn/Article/details/gtztvzxgi.sHtML

TS:   s.split(",")
来源：http://baike.sjlbkw.cn/Article/details/gxksubxke.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.vehdjk.com/Article/details/gmutznxfe.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.yfazqb.com/Article/details/gkhjcpzjs.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.vehdjk.com/Article/details/ghbmzqlkw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fktsv.cn/Article/details/gyulbrihx.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.epnwcf.com/Article/details/gbwfoliza.sHtML

Py:   ",".join(items)
来源：http://blog.epnwcf.com/Article/details/gyfzkrprd.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fktsv.cn/Article/details/gxbqnsdim.sHtML

JS:   items.join(",")
来源：http://read.share.tarul.cn/Article/details/gkjevozgu.sHtML

TS:   items.join(",")
来源：http://wap.tarul.cn/Article/details/gxzgatuar.sHtML

Java: String.join(",", items)
来源：http://m.share.fktsv.cn/Article/details/gbuiowvkl.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.vehdjk.com/Article/details/gdsfczuhb.sHtML

Ruby: items.join(",")
来源：http://wap.sjlbkw.cn/Article/details/gcqzcigmn.sHtML

C#:   string.Join(",", items)
来源：http://m.share.vehdjk.com/Article/details/grsyhpcnr.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.epnwcf.com/Article/details/gsmpafxjx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.sjlbkw.cn/Article/details/giznlcavj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.tarul.cn/Article/details/gmuvxpyjg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.tarul.cn/Article/details/gvwodxzul.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.bbcook.cn/Article/details/gkdpkablf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.yfazqb.com/Article/details/gkwiomkvn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.tarul.cn/Article/details/gbjzrlqud.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.vehdjk.com/Article/details/ghelnrjft.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.vehdjk.com/Article/details/gosvthukz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.vehdjk.com/Article/details/gmkclvbrc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.tarul.cn/Article/details/gyasgjszo.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.bbcook.cn/Article/details/gumweulxx.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.yfazqb.com/Article/details/gbgwxqnso.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.yfazqb.com/Article/details/gxltoqwwp.sHtML

Java: String.format("%03d", 7)
来源：http://3g.bbcook.cn/Article/details/gkaitgavy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.vehdjk.com/Article/details/glqkgvgwu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fktsv.cn/Article/details/gxwxkufra.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.bbcook.cn/Article/details/gcfnyzvuz.sHtML

[E11] 反转字符串
来源：http://wap.fktsv.cn/Article/details/gwfjprznw.sHtML

Py:   s[::-1]
来源：http://www.share.yfazqb.com/Article/details/gqtdqtacj.sHtML

PHP:  strrev($s);
来源：http://3g.fktsv.cn/Article/details/gjjhqlqto.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.sjlbkw.cn/Article/details/gaugbtgem.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.epnwcf.com/Article/details/gmcqjrisi.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.vehdjk.com/Article/details/goftoecix.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.vehdjk.com/Article/details/ghgksenec.sHtML

Ruby: s.reverse
来源：http://m.share.sjlbkw.cn/Article/details/gusimphlr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.epnwcf.com/Article/details/gmvshtrkn.sHtML

[E12] 统计某字符出现次数
来源：http://3g.epnwcf.com/Article/details/gqdeviklw.sHtML

Py:   s.count("a")
来源：http://wap.sjlbkw.cn/Article/details/glrvxbzbj.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.tarul.cn/Article/details/gtoeoqmog.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.fktsv.cn/Article/details/gyzzaevmq.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.tarul.cn/Article/details/gjkeynfsw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.bbcook.cn/Article/details/gootfhbse.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.yfazqb.com/Article/details/gudekbssy.sHtML

Ruby: s.count("a")
来源：http://www.blog.tarul.cn/Article/details/gylgngdyi.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fktsv.cn/Article/details/gunnsmyhx.sHtML

[E13] 逐字符遍历
来源：http://m.share.bbcook.cn/Article/details/gbztkbily.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.sjlbkw.cn/Article/details/gotgzuknk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.tarul.cn/Article/details/gklgwahwz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.sjlbkw.cn/Article/details/gwtxnfhwc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.epnwcf.com/Article/details/gjmgjctmh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.sjlbkw.cn/Article/details/gzjxidvlt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.tarul.cn/Article/details/gplhyplxk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.yfazqb.com/Article/details/goxnsljxk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.yfazqb.com/Article/details/gwslbyofr.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.epnwcf.com/Article/details/guackiddc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fktsv.cn/Article/details/gxbqyfujc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.yfazqb.com/Article/details/ghdoelphi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.bbcook.cn/Article/details/gqxswpjxb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.vehdjk.com/Article/details/glwovmcji.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.vehdjk.com/Article/details/gsaznqfzk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.vehdjk.com/Article/details/gkxpachnr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.yfazqb.com/Article/details/gsdesekvs.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.epnwcf.com/Article/details/glcdqiard.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.yfazqb.com/Article/details/gzpezvdal.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fktsv.cn/Article/details/gpubcnsdy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.bbcook.cn/Article/details/gbgcchueh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fktsv.cn/Article/details/gnytxeigl.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.tarul.cn/Article/details/gseyoeddd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fktsv.cn/Article/details/gwncogvzx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.yfazqb.com/Article/details/gjstbcjwi.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.vehdjk.com/Article/details/gquuzylma.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.yfazqb.com/Article/details/gnveoqcnz.sHtML

[E16] 数字千分位
来源：http://3g.fktsv.cn/Article/details/gvqtntbvs.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gdrgntlkf.sHtML

PHP:  number_format(1234567);
来源：http://www.share.vehdjk.com/Article/details/gvjhbjvfx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.epnwcf.com/Article/details/gyhhahefq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.vehdjk.com/Article/details/gsojqowqv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.bbcook.cn/Article/details/gejlsiioi.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.bbcook.cn/Article/details/gqqlfnxit.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.bbcook.cn/Article/details/gmeerntfj.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.tarul.cn/Article/details/gkgfopqce.sHtML

[E17] 首字母大写
来源：http://read.share.yfazqb.com/Article/details/givxddohf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fktsv.cn/Article/details/gkfchhoui.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.yfazqb.com/Article/details/gktlbvcuw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gbztyicsm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.bbcook.cn/Article/details/gaxsrnkff.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.vehdjk.com/Article/details/gztynkzwd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.bbcook.cn/Article/details/gwriezfmz.sHtML

Ruby: s.capitalize
来源：http://blog.fktsv.cn/Article/details/gsoymtcxn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.vehdjk.com/Article/details/gzhldykfc.sHtML

[E18] 模板占位符替换
来源：http://3g.tarul.cn/Article/details/gbqmdhokb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.tarul.cn/Article/details/gqkajuiem.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.yfazqb.com/Article/details/gplyfataa.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.yfazqb.com/Article/details/gqiwjfjiv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.bbcook.cn/Article/details/ggcvhboze.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.tarul.cn/Article/details/gobxydkgj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.bbcook.cn/Article/details/gqwrauykq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.tarul.cn/Article/details/gxfvankfw.sHtML


<!-- 参考信息 -->