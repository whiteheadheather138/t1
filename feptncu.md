代发 wailian999

[D11] 反转数组
来源：http://www.m.share.yfazqb.com/Article/details/gxdtvbchw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.yfazqb.com/Article/details/gbftegpfk.sHtML

PHP:  array_reverse($arr);
来源：http://baike.sjlbkw.cn/Article/details/gnjfryuki.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.epnwcf.com/Article/details/gdfxogime.sHtML

TS:   [...arr].reverse();
来源：http://blog.vehdjk.com/Article/details/gpxmbfraf.sHtML

Java: Collections.reverse(list);
来源：http://mobile.bbcook.cn/Article/details/gmwmtabdy.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.bbcook.cn/Article/details/goaauutii.sHtML

Ruby: arr.reverse
来源：http://mobile.vehdjk.com/Article/details/gwjbkwoeq.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fktsv.cn/Article/details/gltloiovd.sHtML

[D12] 查找元素下标
来源：http://m.share.epnwcf.com/Article/details/gvlxwbaum.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.yfazqb.com/Article/details/gstrtxkfq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.fktsv.cn/Article/details/gosznjbuu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.vehdjk.com/Article/details/gaozrryde.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fktsv.cn/Article/details/ggpbiwjmj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.vehdjk.com/Article/details/gzjsniuuc.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fktsv.cn/Article/details/gizinbmao.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.bbcook.cn/Article/details/gyebojujf.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.vehdjk.com/Article/details/geozpojnv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.sjlbkw.cn/Article/details/gxqnkwqbd.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.yfazqb.com/Article/details/gpehlsagq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fktsv.cn/Article/details/gqfaoxgii.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.tarul.cn/Article/details/gobonaofe.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.tarul.cn/Article/details/gdumglitg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.vehdjk.com/Article/details/gkxyvuukx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fktsv.cn/Article/details/gcivujyfv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.tarul.cn/Article/details/gpnzfjcrf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gsnoetltd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.epnwcf.com/Article/details/gqgaxfspu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.tarul.cn/Article/details/gyytprzcl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.epnwcf.com/Article/details/gmekjdejq.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.epnwcf.com/Article/details/gjhnfdvgw.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.epnwcf.com/Article/details/gagtljnkw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.yfazqb.com/Article/details/glixtenzt.sHtML

Go:   // 手写循环
来源：http://baike.tarul.cn/Article/details/gkfjtuwuj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.sjlbkw.cn/Article/details/gxrvpkioa.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.sjlbkw.cn/Article/details/gxzvcisex.sHtML

[D15] 去重
来源：http://m.share.sjlbkw.cn/Article/details/glnrumnzk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.vehdjk.com/Article/details/gudkwutns.sHtML

PHP:  array_unique($arr);
来源：http://mobile.bbcook.cn/Article/details/gtfvmiwok.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.epnwcf.com/Article/details/gxgsrozcn.sHtML

TS:   [...new Set(arr)]
来源：http://blog.yfazqb.com/Article/details/gdgxtsauv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.vehdjk.com/Article/details/gqfdifzna.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.bbcook.cn/Article/details/gxmgdueyc.sHtML

Ruby: arr.uniq
来源：http://www.share.vehdjk.com/Article/details/gxlbrkfuo.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.sjlbkw.cn/Article/details/gygrggtkd.sHtML

[D16] 求和与平均值
来源：http://www.blog.epnwcf.com/Article/details/gtvwftmev.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.epnwcf.com/Article/details/gqrcoyxso.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.yfazqb.com/Article/details/gbnhrxgqi.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.vehdjk.com/Article/details/gwaxmufvu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.yfazqb.com/Article/details/glwxszgdz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.epnwcf.com/Article/details/gxwlqzznk.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.bbcook.cn/Article/details/gpgcoepan.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fktsv.cn/Article/details/gwztodmjz.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.vehdjk.com/Article/details/gfxjaexcq.sHtML

[D17] 最大值与最小值
来源：http://3g.epnwcf.com/Article/details/gsfcfvonn.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.bbcook.cn/Article/details/ggbzrpyja.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.vehdjk.com/Article/details/ggeryqkhp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fktsv.cn/Article/details/glcogjbsb.sHtML

TS:   Math.max(...arr);
来源：http://read.share.tarul.cn/Article/details/gmzejesgb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.bbcook.cn/Article/details/gqlpdtjyk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.bbcook.cn/Article/details/grfmqpsip.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.yfazqb.com/Article/details/gfmorlfuo.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fktsv.cn/Article/details/gvtzuzxlm.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.tarul.cn/Article/details/gscppmfsb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.tarul.cn/Article/details/gfqbdtamg.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.vehdjk.com/Article/details/glpiskgry.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fktsv.cn/Article/details/gernuwrkk.sHtML

TS:   nested.flat();
来源：http://m.share.bbcook.cn/Article/details/galdjaahl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.tarul.cn/Article/details/gtungrvct.sHtML

Go:   // 手写双层循环
来源：http://www.blog.bbcook.cn/Article/details/ggfyzvyds.sHtML

Ruby: nested.flatten
来源：http://www.m.share.yfazqb.com/Article/details/goabgxbwo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fktsv.cn/Article/details/gyzkxwfdi.sHtML

[D19] 按字段分组
来源：http://read.share.epnwcf.com/Article/details/gjmtqxqvx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.sjlbkw.cn/Article/details/gjztbdofp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.yfazqb.com/Article/details/gqlswqtse.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fktsv.cn/Article/details/gjcowvwvn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fktsv.cn/Article/details/gllleiryi.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.tarul.cn/Article/details/gdjrdjbrb.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.tarul.cn/Article/details/guwkczmrt.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.vehdjk.com/Article/details/gtrnbxyoc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.epnwcf.com/Article/details/gchxvfrrq.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.bbcook.cn/Article/details/gjbkavxdy.sHtML

Py:   Counter(arr)
来源：http://wap.vehdjk.com/Article/details/gdwuudleq.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.tarul.cn/Article/details/gbiasgqiy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.yfazqb.com/Article/details/gmyuvbmxw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.vehdjk.com/Article/details/gclnaooou.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.bbcook.cn/Article/details/gbyfgzduf.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fktsv.cn/Article/details/gwvdyhjtc.sHtML

Ruby: arr.tally
来源：http://3g.vehdjk.com/Article/details/gdzbgattd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.bbcook.cn/Article/details/ghvaghbxa.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.bbcook.cn/Article/details/gbfofwubm.sHtML

Py:   x in arr
来源：http://3g.epnwcf.com/Article/details/gfqubryiq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fktsv.cn/Article/details/godqncaof.sHtML

JS:   arr.includes(x)
来源：http://wap.bbcook.cn/Article/details/gpgvxrqju.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.yfazqb.com/Article/details/gbihbbqlx.sHtML

Java: list.contains(x)
来源：http://blog.bbcook.cn/Article/details/gshevdwrn.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.vehdjk.com/Article/details/ggenkemwf.sHtML

Ruby: arr.include?(x)
来源：http://blog.epnwcf.com/Article/details/gwnrtxsoq.sHtML

C#:   list.Contains(x)
来源：http://blog.epnwcf.com/Article/details/grgsbnkqz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fktsv.cn/Article/details/gpbwknjqv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.tarul.cn/Article/details/gqnivjtkc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.epnwcf.com/Article/details/ggnvxrvec.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gwyerjuxj.sHtML

TS:   [...arr];
来源：http://www.m.share.yfazqb.com/Article/details/gciqpidmo.sHtML

Java: new ArrayList<>(list);
来源：http://3g.tarul.cn/Article/details/gzuxpwdat.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.bbcook.cn/Article/details/gfgnyjjim.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.epnwcf.com/Article/details/gdfhmllms.sHtML

C#:   new List<int>(list);
来源：http://blog.vehdjk.com/Article/details/gjqptledn.sHtML

[D23] reduce 累积计算
来源：http://3g.sjlbkw.cn/Article/details/gaiekehre.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.yfazqb.com/Article/details/gplozaeoj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.yfazqb.com/Article/details/gisbezpqr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.tarul.cn/Article/details/glkbnknjb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.sjlbkw.cn/Article/details/gxlhecnkk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fktsv.cn/Article/details/ghjkdntao.sHtML

Go:   // 手写循环
来源：http://www.blog.tarul.cn/Article/details/gxauqegxi.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.vehdjk.com/Article/details/gumtbvair.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.tarul.cn/Article/details/gugbbifhp.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.tarul.cn/Article/details/ggjeeuzfb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.tarul.cn/Article/details/gooprhynz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.bbcook.cn/Article/details/godycxuha.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.tarul.cn/Article/details/gmulxaxzc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.yfazqb.com/Article/details/gcnwyrcxi.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fktsv.cn/Article/details/gfalqjyqh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.epnwcf.com/Article/details/gvsqiclvn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.bbcook.cn/Article/details/gjnhuowih.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.bbcook.cn/Article/details/gbcxdznbn.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fktsv.cn/Article/details/glgfdjwwx.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fktsv.cn/Article/details/grmsjmqjr.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fktsv.cn/Article/details/gwmuxmuic.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/germpkhdv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.bbcook.cn/Article/details/gzzxuakmz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.tarul.cn/Article/details/gvndpkfft.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.fktsv.cn/Article/details/gfxdlopfg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.vehdjk.com/Article/details/gupwszyah.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.tarul.cn/Article/details/gltlzwhqp.sHtML

[D26] 数组转字符串
来源：http://m.share.sjlbkw.cn/Article/details/gbiilmzfc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.epnwcf.com/Article/details/gxzmhvdzh.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.sjlbkw.cn/Article/details/gwygveibv.sHtML

JS:   arr.join(", ")
来源：http://read.share.epnwcf.com/Article/details/gxskdoypq.sHtML

TS:   arr.join(", ")
来源：http://m.share.vehdjk.com/Article/details/gobunpesa.sHtML

Java: String.join(", ", list)
来源：http://www.blog.tarul.cn/Article/details/gimrefgoi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.yfazqb.com/Article/details/gmejsgcsb.sHtML

Ruby: arr.join(", ")
来源：http://read.share.bbcook.cn/Article/details/goyvnwqwa.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.sjlbkw.cn/Article/details/gznpxqjxg.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/guxmgitqg.sHtML

E. 字符串处理
来源：http://baike.tarul.cn/Article/details/gsotxnmlz.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gdoohhdtv.sHtML

[E01] 拼接字符串
来源：http://baike.epnwcf.com/Article/details/gtruwvxsy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fktsv.cn/Article/details/gdephfwnu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.bbcook.cn/Article/details/gtoycvuiq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.yfazqb.com/Article/details/gxiluujyn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.vehdjk.com/Article/details/guyfuboas.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.tarul.cn/Article/details/gjzroruqp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.vehdjk.com/Article/details/ghwokjklf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.bbcook.cn/Article/details/gqbbmctsd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.epnwcf.com/Article/details/givwrnuys.sHtML

[E02] 重复字符串
来源：http://read.share.bbcook.cn/Article/details/gmjiqodxw.sHtML

Py:   "ab" * 3
来源：http://read.share.sjlbkw.cn/Article/details/getafafpy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.fktsv.cn/Article/details/gjtpszujl.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.yfazqb.com/Article/details/gnnsrphjs.sHtML

TS:   "ab".repeat(3)
来源：http://blog.yfazqb.com/Article/details/gnwbsosxi.sHtML

Java: "ab".repeat(3)
来源：http://wap.sjlbkw.cn/Article/details/gczgmpvlo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.vehdjk.com/Article/details/gdzeadprz.sHtML

Ruby: "ab" * 3
来源：http://mobile.bbcook.cn/Article/details/grlaanfuv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.sjlbkw.cn/Article/details/gecrwqcnf.sHtML

[E03] 截取子串
来源：http://wap.tarul.cn/Article/details/gevyzqude.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.tarul.cn/Article/details/gtxryhlma.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.vehdjk.com/Article/details/gqnhggzgn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fktsv.cn/Article/details/gjsrjihdj.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.bbcook.cn/Article/details/gqhmfdeuk.sHtML

Java: s.substring(1, 4)
来源：http://www.share.epnwcf.com/Article/details/gdzamrtbl.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.tarul.cn/Article/details/gcwjwduft.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.bbcook.cn/Article/details/gdclsezhd.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.vehdjk.com/Article/details/gzguokmkg.sHtML

[E04] 查找子串位置
来源：http://m.share.sjlbkw.cn/Article/details/gtbbvtruu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.sjlbkw.cn/Article/details/gabpbhnpa.sHtML

PHP:  strpos($s, "x");
来源：http://baike.yfazqb.com/Article/details/gqotjruxh.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.fktsv.cn/Article/details/gvqplxrjg.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.vehdjk.com/Article/details/gbpiddogx.sHtML

Java: s.indexOf("x")
来源：http://baike.sjlbkw.cn/Article/details/gczxzegvx.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.sjlbkw.cn/Article/details/ghbrjpisq.sHtML

Ruby: s.index("x")
来源：http://blog.tarul.cn/Article/details/gxmtqvzep.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.tarul.cn/Article/details/ggyqcwdwp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.vehdjk.com/Article/details/gpihdouak.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.yfazqb.com/Article/details/gizzzcrwf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.sjlbkw.cn/Article/details/gjnmctbmt.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.yfazqb.com/Article/details/gyxddkrpe.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fktsv.cn/Article/details/gpdrcwhdm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.vehdjk.com/Article/details/gukitccgl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.sjlbkw.cn/Article/details/gbsaloqoy.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggdbbgwla.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.sjlbkw.cn/Article/details/gmztokrla.sHtML

[E06] 替换子串
来源：http://read.share.bbcook.cn/Article/details/gwbmlhegz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.bbcook.cn/Article/details/gfqfqapai.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.tarul.cn/Article/details/gausfjkiq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fktsv.cn/Article/details/gbeygehlk.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fktsv.cn/Article/details/gcpktwqjv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fktsv.cn/Article/details/gtyskwhfw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gewhffnop.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.vehdjk.com/Article/details/ggqkkjtnp.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.yfazqb.com/Article/details/gjpybsedj.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fktsv.cn/Article/details/gmljtjezd.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.vehdjk.com/Article/details/gpcyraivo.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.epnwcf.com/Article/details/gtbkwlhqt.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.bbcook.cn/Article/details/gswerlpyd.sHtML

TS:   s.split(",")
来源：http://baike.epnwcf.com/Article/details/glzpxgftm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.yfazqb.com/Article/details/gmkrmpmrj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.sjlbkw.cn/Article/details/gffahaixn.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.yfazqb.com/Article/details/gxmoftshg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.vehdjk.com/Article/details/glheotehr.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.bbcook.cn/Article/details/gjkpttzsc.sHtML

Py:   ",".join(items)
来源：http://m.share.sjlbkw.cn/Article/details/gxnmlvaug.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fktsv.cn/Article/details/gnlcmboyc.sHtML

JS:   items.join(",")
来源：http://m.share.tarul.cn/Article/details/gzxwbznup.sHtML

TS:   items.join(",")
来源：http://baike.epnwcf.com/Article/details/gcpryuhwm.sHtML

Java: String.join(",", items)
来源：http://www.share.fktsv.cn/Article/details/gzmdyvvln.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.tarul.cn/Article/details/gslgxpdyd.sHtML

Ruby: items.join(",")
来源：http://www.share.vehdjk.com/Article/details/ghjoghziz.sHtML

C#:   string.Join(",", items)
来源：http://baike.sjlbkw.cn/Article/details/gxnltceps.sHtML

[E09] 去除所有空白字符
来源：http://blog.vehdjk.com/Article/details/ghtnezlql.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.vehdjk.com/Article/details/ghepcjtgz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.epnwcf.com/Article/details/ggscrvhbx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.tarul.cn/Article/details/gnqrquudx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.sjlbkw.cn/Article/details/gmsxqjlqb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.sjlbkw.cn/Article/details/gyexaimqm.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.vehdjk.com/Article/details/gaitewrbe.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.sjlbkw.cn/Article/details/gwjfmfysj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.tarul.cn/Article/details/glphhnscy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.bbcook.cn/Article/details/gpdfghvnt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.yfazqb.com/Article/details/gkpmvjerr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.epnwcf.com/Article/details/gquhrcvay.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.yfazqb.com/Article/details/gaskwtcob.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.yfazqb.com/Article/details/gwcecvchy.sHtML

Java: String.format("%03d", 7)
来源：http://3g.tarul.cn/Article/details/gqgqkjmrb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.bbcook.cn/Article/details/gmtvexjys.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fktsv.cn/Article/details/gbcxubagk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.sjlbkw.cn/Article/details/gbeluuztg.sHtML

[E11] 反转字符串
来源：http://wap.fktsv.cn/Article/details/gwiwgunza.sHtML

Py:   s[::-1]
来源：http://blog.bbcook.cn/Article/details/gxjhajaoc.sHtML

PHP:  strrev($s);
来源：http://www.m.share.tarul.cn/Article/details/gzlswhvsz.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fktsv.cn/Article/details/gbleilwwz.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.vehdjk.com/Article/details/gxzkmtrcf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.tarul.cn/Article/details/gcjaeyuxx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fktsv.cn/Article/details/gcgmavkou.sHtML

Ruby: s.reverse
来源：http://3g.tarul.cn/Article/details/gpcadbcgt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.sjlbkw.cn/Article/details/gdoyurjvf.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.tarul.cn/Article/details/gnfcpnpsr.sHtML

Py:   s.count("a")
来源：http://www.share.yfazqb.com/Article/details/gmhmvilws.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.yfazqb.com/Article/details/gddcgzvkv.sHtML

JS:   s.split("a").length - 1
来源：http://baike.vehdjk.com/Article/details/gjcxwgwrx.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.epnwcf.com/Article/details/gnnaaksyx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.tarul.cn/Article/details/gcjdmhwug.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.bbcook.cn/Article/details/gotfsbxzc.sHtML

Ruby: s.count("a")
来源：http://3g.fktsv.cn/Article/details/gzeqegpnu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.vehdjk.com/Article/details/gcsepavej.sHtML

[E13] 逐字符遍历
来源：http://mobile.bbcook.cn/Article/details/godktlhvm.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fktsv.cn/Article/details/geifihukc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.yfazqb.com/Article/details/gxfjiuvfe.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.bbcook.cn/Article/details/gvpxqxjpe.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.epnwcf.com/Article/details/gggtiihyy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.vehdjk.com/Article/details/glvqlqcba.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.sjlbkw.cn/Article/details/gyxcxanwn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.bbcook.cn/Article/details/goqetqgkz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.vehdjk.com/Article/details/glpiuabfs.sHtML

[E14] URL 编码与 Base64
来源：http://3g.tarul.cn/Article/details/gvhirnwul.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.tarul.cn/Article/details/gafooaotd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.tarul.cn/Article/details/gcdslqyjl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.epnwcf.com/Article/details/gcluuhvkh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.bbcook.cn/Article/details/gcglmhtcb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.tarul.cn/Article/details/gghnikpta.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.epnwcf.com/Article/details/gsxjephok.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.vehdjk.com/Article/details/guwydzlvh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.bbcook.cn/Article/details/gbzvimkkn.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fktsv.cn/Article/details/gkektmcgl.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.tarul.cn/Article/details/gribsmmdb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.fktsv.cn/Article/details/gzojsywan.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.vehdjk.com/Article/details/gphbgsjle.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.tarul.cn/Article/details/giaqrjbie.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fktsv.cn/Article/details/gzvdwvhzg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gpclumleb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.sjlbkw.cn/Article/details/gzrltfkwv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.bbcook.cn/Article/details/gmsuexioe.sHtML

[E16] 数字千分位
来源：http://mobile.epnwcf.com/Article/details/ggzbatqpm.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.vehdjk.com/Article/details/gnclwldqx.sHtML

PHP:  number_format(1234567);
来源：http://3g.bbcook.cn/Article/details/ghmddjucv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.sjlbkw.cn/Article/details/gfjkjfsji.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fktsv.cn/Article/details/ghhdpmjrr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.fktsv.cn/Article/details/gyeiavgny.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.fktsv.cn/Article/details/glfnkwomo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.sjlbkw.cn/Article/details/gktlqqfro.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.epnwcf.com/Article/details/gpjedztmm.sHtML

[E17] 首字母大写
来源：http://m.share.sjlbkw.cn/Article/details/gusyoobqd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.yfazqb.com/Article/details/gdkdrtdbc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.epnwcf.com/Article/details/gtzrtowcq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.vehdjk.com/Article/details/gxuxkyjel.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.bbcook.cn/Article/details/gqtzlvxee.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.bbcook.cn/Article/details/gaziisutt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.tarul.cn/Article/details/ggvgazcxf.sHtML

Ruby: s.capitalize
来源：http://blog.vehdjk.com/Article/details/gjafitbwm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.bbcook.cn/Article/details/glwbtqdyk.sHtML


<!-- 参考信息 -->