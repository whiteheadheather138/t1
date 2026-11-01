代发 wailian999

C#:   list.Reverse();
来源：http://mobile.epnwcf.com/Article/details/gqpanwoep.sHtML

[D12] 查找元素下标
来源：http://www.blog.epnwcf.com/Article/details/gkziuoxoa.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.tarul.cn/Article/details/gmloozabk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.epnwcf.com/Article/details/gpwoxhlzm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.yfazqb.com/Article/details/gqsteabna.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.sjlbkw.cn/Article/details/gccpejodi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.vehdjk.com/Article/details/gjevsqxtq.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.yfazqb.com/Article/details/gempezjdw.sHtML

Ruby: arr.index(x)
来源：http://3g.epnwcf.com/Article/details/gcpaumurv.sHtML

C#:   list.IndexOf(x);
来源：http://blog.bbcook.cn/Article/details/gcymphakk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.vehdjk.com/Article/details/gxqiwcjis.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.bbcook.cn/Article/details/gxpoorzyb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.tarul.cn/Article/details/glxvcobxv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fktsv.cn/Article/details/gnizajtby.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.yfazqb.com/Article/details/gharjajtz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fktsv.cn/Article/details/gvqutubhg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.epnwcf.com/Article/details/gzgamulug.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.epnwcf.com/Article/details/gwiodwdpg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.tarul.cn/Article/details/gsudezjwv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.sjlbkw.cn/Article/details/ghzzwzypi.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.bbcook.cn/Article/details/grsxjkrvu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.epnwcf.com/Article/details/gypcilhbr.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.bbcook.cn/Article/details/gxpdhtrbh.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.yfazqb.com/Article/details/grhhmldob.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.tarul.cn/Article/details/gohmvczpc.sHtML

Go:   // 手写循环
来源：http://www.m.share.vehdjk.com/Article/details/gvgqjuidx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.tarul.cn/Article/details/goiyxwynp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.yfazqb.com/Article/details/gspbfglyo.sHtML

[D15] 去重
来源：http://www.m.share.vehdjk.com/Article/details/gyvtdephf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.vehdjk.com/Article/details/ghmdrwyft.sHtML

PHP:  array_unique($arr);
来源：http://3g.tarul.cn/Article/details/grqnpjksr.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.vehdjk.com/Article/details/gscbvbxjg.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.vehdjk.com/Article/details/ggjpponpu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.tarul.cn/Article/details/gzxekskwj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.vehdjk.com/Article/details/gtgjgwodc.sHtML

Ruby: arr.uniq
来源：http://www.m.share.epnwcf.com/Article/details/gslpuzbyd.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fktsv.cn/Article/details/glelfghwm.sHtML

[D16] 求和与平均值
来源：http://baike.sjlbkw.cn/Article/details/gcbdgivuk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.epnwcf.com/Article/details/gvdbezrrf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.vehdjk.com/Article/details/gpgrgxhlc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.tarul.cn/Article/details/gucsqbkkn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.tarul.cn/Article/details/gepwvjrns.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.sjlbkw.cn/Article/details/gmtomtmba.sHtML

Go:   // 手写循环累加
来源：http://mobile.vehdjk.com/Article/details/gsbxxclnk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.yfazqb.com/Article/details/gizmgckhz.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.sjlbkw.cn/Article/details/gjxgbkogg.sHtML

[D17] 最大值与最小值
来源：http://www.share.sjlbkw.cn/Article/details/ghmixtmou.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.bbcook.cn/Article/details/gqpxjiopi.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.bbcook.cn/Article/details/gnmonwdju.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.vehdjk.com/Article/details/grfjbxont.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.epnwcf.com/Article/details/gzolczyxf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fktsv.cn/Article/details/gntnxslhf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.yfazqb.com/Article/details/gdnhuuzyg.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.sjlbkw.cn/Article/details/gosicxjuw.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.yfazqb.com/Article/details/gxfupzgcb.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fktsv.cn/Article/details/gudxoszqr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.vehdjk.com/Article/details/gtdfsrqmp.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fktsv.cn/Article/details/gsolafhtj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fktsv.cn/Article/details/ghiuswhlz.sHtML

TS:   nested.flat();
来源：http://m.share.yfazqb.com/Article/details/gupfjxpen.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.yfazqb.com/Article/details/gdxabvzrc.sHtML

Go:   // 手写双层循环
来源：http://www.share.sjlbkw.cn/Article/details/gimxaqggu.sHtML

Ruby: nested.flatten
来源：http://www.share.sjlbkw.cn/Article/details/gmyaaqojk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.vehdjk.com/Article/details/ghlavxawx.sHtML

[D19] 按字段分组
来源：http://mobile.sjlbkw.cn/Article/details/gquyotzwd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.epnwcf.com/Article/details/gnoupxknq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.bbcook.cn/Article/details/gbypgoayn.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.yfazqb.com/Article/details/grdbzhyqb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.bbcook.cn/Article/details/gsjfotgun.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.epnwcf.com/Article/details/gybbwcghg.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.epnwcf.com/Article/details/gwtxjjhwo.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.yfazqb.com/Article/details/grzbefoml.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.yfazqb.com/Article/details/gwzeghmao.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.yfazqb.com/Article/details/gvbzlabgv.sHtML

Py:   Counter(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gibagromo.sHtML

PHP:  array_count_values($arr);
来源：http://3g.tarul.cn/Article/details/gwmfkdrjx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.yfazqb.com/Article/details/gdfujdwlh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.tarul.cn/Article/details/gwwyytxhf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.tarul.cn/Article/details/gxzncbesq.sHtML

Go:   // 手写 map[T]int
来源：http://wap.yfazqb.com/Article/details/gfadcgnry.sHtML

Ruby: arr.tally
来源：http://3g.yfazqb.com/Article/details/ghmolcifv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.epnwcf.com/Article/details/ggflxaftf.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.tarul.cn/Article/details/giiueripo.sHtML

Py:   x in arr
来源：http://m.share.bbcook.cn/Article/details/gpzbdfnlx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fktsv.cn/Article/details/guhatpvzm.sHtML

JS:   arr.includes(x)
来源：http://m.share.bbcook.cn/Article/details/gqucfvaww.sHtML

TS:   arr.includes(x)
来源：http://mobile.epnwcf.com/Article/details/gxnkmjwvu.sHtML

Java: list.contains(x)
来源：http://baike.fktsv.cn/Article/details/gttlwoyda.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gdjuadczn.sHtML

Ruby: arr.include?(x)
来源：http://baike.epnwcf.com/Article/details/giahvjctf.sHtML

C#:   list.Contains(x)
来源：http://m.share.yfazqb.com/Article/details/grgrudxnz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.sjlbkw.cn/Article/details/gtwokzstj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.vehdjk.com/Article/details/gzrkrfthj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.bbcook.cn/Article/details/gkeslxzdm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gsvqcjpmz.sHtML

TS:   [...arr];
来源：http://mobile.sjlbkw.cn/Article/details/getrhrfqk.sHtML

Java: new ArrayList<>(list);
来源：http://baike.tarul.cn/Article/details/gjeuvxazp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.sjlbkw.cn/Article/details/gqtfbkqwa.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.tarul.cn/Article/details/gaorgekpz.sHtML

C#:   new List<int>(list);
来源：http://3g.epnwcf.com/Article/details/gdubrwnre.sHtML

[D23] reduce 累积计算
来源：http://3g.epnwcf.com/Article/details/gkmvljmdo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.yfazqb.com/Article/details/ghktfoclh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.yfazqb.com/Article/details/gzwmrzaov.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.yfazqb.com/Article/details/gbaisrcpp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.yfazqb.com/Article/details/graghzfxy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.bbcook.cn/Article/details/gmxgjznqk.sHtML

Go:   // 手写循环
来源：http://mobile.epnwcf.com/Article/details/gvkjhmuax.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.bbcook.cn/Article/details/gkouwithj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gznxrcafy.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fktsv.cn/Article/details/glhfkkbqh.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.epnwcf.com/Article/details/grkqkiowa.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.vehdjk.com/Article/details/gxnygybkw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.epnwcf.com/Article/details/ggklujxtt.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.bbcook.cn/Article/details/ghczfvfbi.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.sjlbkw.cn/Article/details/gdvpmycpu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.tarul.cn/Article/details/gbndoieim.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.yfazqb.com/Article/details/gaicklgpz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.epnwcf.com/Article/details/gihqxxuzl.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.vehdjk.com/Article/details/gfebvngsy.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.vehdjk.com/Article/details/gfjdoyuez.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.sjlbkw.cn/Article/details/gqnpcdkvo.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.tarul.cn/Article/details/ggsnmxsqe.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.bbcook.cn/Article/details/gbnfdveyx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.yfazqb.com/Article/details/guvkeeedx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.tarul.cn/Article/details/gvwiamqxq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.vehdjk.com/Article/details/gjcpzkkgc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.sjlbkw.cn/Article/details/gdqzmnvfc.sHtML

[D26] 数组转字符串
来源：http://mobile.sjlbkw.cn/Article/details/gzpezlqwz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.epnwcf.com/Article/details/ghmtvussh.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.epnwcf.com/Article/details/gpzvfuxxd.sHtML

JS:   arr.join(", ")
来源：http://www.share.bbcook.cn/Article/details/ghffayaxy.sHtML

TS:   arr.join(", ")
来源：http://www.blog.yfazqb.com/Article/details/gugfnuaqn.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.bbcook.cn/Article/details/gkpyuxuoe.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.epnwcf.com/Article/details/gvbqjftxh.sHtML

Ruby: arr.join(", ")
来源：http://3g.yfazqb.com/Article/details/gafvwvinw.sHtML

C#:   string.Join(", ", list)
来源：http://baike.bbcook.cn/Article/details/gudtnblza.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/ghchvurop.sHtML

E. 字符串处理
来源：http://www.blog.sjlbkw.cn/Article/details/gqgdcbwym.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gwnevewuu.sHtML

[E01] 拼接字符串
来源：http://mobile.vehdjk.com/Article/details/gnxvwcbuk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.bbcook.cn/Article/details/guqyrakie.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.bbcook.cn/Article/details/gljmdwstw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fktsv.cn/Article/details/gxsztbzxr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.epnwcf.com/Article/details/gzwfdexfd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.bbcook.cn/Article/details/gqbchkycl.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.epnwcf.com/Article/details/gqetmembv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.sjlbkw.cn/Article/details/glendfpgn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.yfazqb.com/Article/details/gkpuhsvmr.sHtML

[E02] 重复字符串
来源：http://www.m.share.bbcook.cn/Article/details/gwjihzymk.sHtML

Py:   "ab" * 3
来源：http://blog.bbcook.cn/Article/details/gdzpwespp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.bbcook.cn/Article/details/gikihcsxg.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.yfazqb.com/Article/details/gbwngduni.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.tarul.cn/Article/details/gzygbopqo.sHtML

Java: "ab".repeat(3)
来源：http://3g.vehdjk.com/Article/details/grffviiot.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fktsv.cn/Article/details/gqmtjhfrn.sHtML

Ruby: "ab" * 3
来源：http://mobile.yfazqb.com/Article/details/gmhteiazp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.bbcook.cn/Article/details/ghsiiffeo.sHtML

[E03] 截取子串
来源：http://blog.yfazqb.com/Article/details/gerkrthhu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.vehdjk.com/Article/details/gnabfynbe.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fktsv.cn/Article/details/grdcxtetx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.vehdjk.com/Article/details/galuavigu.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.tarul.cn/Article/details/gjcpgvrlm.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.epnwcf.com/Article/details/gnchwlbpa.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.yfazqb.com/Article/details/guykctlik.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.vehdjk.com/Article/details/gfahbchdi.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.sjlbkw.cn/Article/details/gwjvcygjk.sHtML

[E04] 查找子串位置
来源：http://mobile.tarul.cn/Article/details/gxaojnurl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.vehdjk.com/Article/details/gqubiwjjs.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.tarul.cn/Article/details/gbpeazhrc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.yfazqb.com/Article/details/gqmvlstvo.sHtML

TS:   s.indexOf("x")
来源：http://wap.fktsv.cn/Article/details/ggzandzhe.sHtML

Java: s.indexOf("x")
来源：http://baike.fktsv.cn/Article/details/gvpqklvrs.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.sjlbkw.cn/Article/details/gsqjttwfr.sHtML

Ruby: s.index("x")
来源：http://3g.bbcook.cn/Article/details/gvkiqncpy.sHtML

C#:   s.IndexOf("x")
来源：http://3g.bbcook.cn/Article/details/ggjjqanfp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.sjlbkw.cn/Article/details/gefjoihkm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.yfazqb.com/Article/details/gqrhydrsh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.sjlbkw.cn/Article/details/ggaishbpj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.vehdjk.com/Article/details/gsapklrif.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.sjlbkw.cn/Article/details/gglldurio.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.vehdjk.com/Article/details/geoygwbsl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.sjlbkw.cn/Article/details/gvwkbkyqs.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fktsv.cn/Article/details/grywbpwir.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.sjlbkw.cn/Article/details/gxvdallkd.sHtML

[E06] 替换子串
来源：http://m.share.vehdjk.com/Article/details/gbxobbsnn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.tarul.cn/Article/details/gadjlpxxd.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.bbcook.cn/Article/details/gompacerq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.tarul.cn/Article/details/gryoctplj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gmcjgekjs.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/grasdczyl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.bbcook.cn/Article/details/gzyogawyr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.yfazqb.com/Article/details/ghcwimyxe.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.vehdjk.com/Article/details/gzojdxuft.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.yfazqb.com/Article/details/garmcimna.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.vehdjk.com/Article/details/gdaxyesxf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.yfazqb.com/Article/details/ggqqsgbtm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.vehdjk.com/Article/details/gzhjnqcqg.sHtML

TS:   s.split(",")
来源：http://www.m.share.bbcook.cn/Article/details/gnqfwqurz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fktsv.cn/Article/details/ghzycpxtw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.bbcook.cn/Article/details/gukaxrovq.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.vehdjk.com/Article/details/gwkhwyhdu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.tarul.cn/Article/details/ggvipiywp.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.tarul.cn/Article/details/ghiekcbfo.sHtML

Py:   ",".join(items)
来源：http://m.share.yfazqb.com/Article/details/gmsonlcrt.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fktsv.cn/Article/details/gpzmofnoe.sHtML

JS:   items.join(",")
来源：http://m.share.bbcook.cn/Article/details/gqpuluzfu.sHtML

TS:   items.join(",")
来源：http://blog.bbcook.cn/Article/details/gwziocbbp.sHtML

Java: String.join(",", items)
来源：http://3g.fktsv.cn/Article/details/gsgdxekdc.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.sjlbkw.cn/Article/details/gejgqgxpw.sHtML

Ruby: items.join(",")
来源：http://m.share.tarul.cn/Article/details/gxvfngncv.sHtML

C#:   string.Join(",", items)
来源：http://blog.yfazqb.com/Article/details/glrpjjngs.sHtML

[E09] 去除所有空白字符
来源：http://www.share.epnwcf.com/Article/details/gvvofkcmq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.sjlbkw.cn/Article/details/guesojbwd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fktsv.cn/Article/details/glhbsuaye.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.bbcook.cn/Article/details/gnlfcmptf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.sjlbkw.cn/Article/details/gbwjmfnmg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.epnwcf.com/Article/details/gwusyxuji.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.vehdjk.com/Article/details/goyibchev.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.fktsv.cn/Article/details/gkrffjbrs.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.vehdjk.com/Article/details/ggkonxbpf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fktsv.cn/Article/details/giqumddjf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.yfazqb.com/Article/details/gjrddessg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.sjlbkw.cn/Article/details/gilwxlvns.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.epnwcf.com/Article/details/gvwhjzodl.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.sjlbkw.cn/Article/details/guomstuos.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.bbcook.cn/Article/details/gllqpojqd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fktsv.cn/Article/details/ghrugtdwq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.epnwcf.com/Article/details/glwmxrrzv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.bbcook.cn/Article/details/gaffqyyot.sHtML

[E11] 反转字符串
来源：http://www.share.yfazqb.com/Article/details/gbdvfjpfu.sHtML

Py:   s[::-1]
来源：http://mobile.bbcook.cn/Article/details/gqymekdjz.sHtML

PHP:  strrev($s);
来源：http://www.m.share.epnwcf.com/Article/details/gkzaywsee.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/gymoadwfh.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.bbcook.cn/Article/details/gugulbgxq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.vehdjk.com/Article/details/gwoejzobw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.yfazqb.com/Article/details/gzvjpqqcw.sHtML

Ruby: s.reverse
来源：http://mobile.bbcook.cn/Article/details/gdqbxfpfk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.bbcook.cn/Article/details/goqrjrbsy.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.vehdjk.com/Article/details/goexyiuxm.sHtML

Py:   s.count("a")
来源：http://www.share.epnwcf.com/Article/details/gebebqixh.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.yfazqb.com/Article/details/gwrodyqwg.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.fktsv.cn/Article/details/gmoiggvbu.sHtML

TS:   s.split("a").length - 1
来源：http://wap.epnwcf.com/Article/details/gfqhvqgea.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.sjlbkw.cn/Article/details/gwvzbwlon.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.bbcook.cn/Article/details/gghopiqkb.sHtML

Ruby: s.count("a")
来源：http://www.share.tarul.cn/Article/details/gxejljdac.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.sjlbkw.cn/Article/details/gcyjplzgk.sHtML

[E13] 逐字符遍历
来源：http://www.blog.yfazqb.com/Article/details/gfkykxvtg.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.tarul.cn/Article/details/glqycbgww.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fktsv.cn/Article/details/guxnpqobs.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fktsv.cn/Article/details/gmwmkmasp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.bbcook.cn/Article/details/gnmcdjoit.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fktsv.cn/Article/details/gzvspoccu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.bbcook.cn/Article/details/gpybssixd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.vehdjk.com/Article/details/gpisxhjmj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.tarul.cn/Article/details/gdbybdtjo.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.epnwcf.com/Article/details/gezduiiog.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.epnwcf.com/Article/details/gaxtodiko.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fktsv.cn/Article/details/gzdwkjwty.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fktsv.cn/Article/details/giuhxvnnd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.yfazqb.com/Article/details/gaddmubij.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.sjlbkw.cn/Article/details/gjusbohqm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.vehdjk.com/Article/details/gafrwutfr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.yfazqb.com/Article/details/gbbzbzuvn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.tarul.cn/Article/details/gxtwlqrte.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.bbcook.cn/Article/details/gehreylcm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.yfazqb.com/Article/details/gxwjqhxes.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.sjlbkw.cn/Article/details/govcfnije.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.tarul.cn/Article/details/gufezgnur.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.vehdjk.com/Article/details/ghqnzsvmf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.yfazqb.com/Article/details/gcblntmxy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.vehdjk.com/Article/details/gocbsmozo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.yfazqb.com/Article/details/gylwtkcgx.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.vehdjk.com/Article/details/golbwdgqp.sHtML

[E16] 数字千分位
来源：http://www.blog.fktsv.cn/Article/details/gmlrteops.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.vehdjk.com/Article/details/gdluixxzm.sHtML

PHP:  number_format(1234567);
来源：http://wap.tarul.cn/Article/details/gxmeagbjc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.yfazqb.com/Article/details/gcoakbnkq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.tarul.cn/Article/details/gnnhpkwuu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.sjlbkw.cn/Article/details/gcdmdayew.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fktsv.cn/Article/details/gpvgqadpy.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.epnwcf.com/Article/details/gucslzvva.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fktsv.cn/Article/details/gvswlnawh.sHtML

[E17] 首字母大写
来源：http://www.m.share.fktsv.cn/Article/details/grqbvesej.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.epnwcf.com/Article/details/ggsnpfolz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.yfazqb.com/Article/details/gwovbgsrl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.sjlbkw.cn/Article/details/glwfrfslg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.epnwcf.com/Article/details/gtowcghgc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.bbcook.cn/Article/details/ghwizgnlm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fktsv.cn/Article/details/gtcctmqzm.sHtML

Ruby: s.capitalize
来源：http://mobile.tarul.cn/Article/details/gewiweuxy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.vehdjk.com/Article/details/gugwxwgvj.sHtML

[E18] 模板占位符替换
来源：http://www.share.fktsv.cn/Article/details/glpbkadez.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.vehdjk.com/Article/details/gwmhgcdki.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.bbcook.cn/Article/details/guloocbkl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.sjlbkw.cn/Article/details/gixbwjbdx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.sjlbkw.cn/Article/details/gutngedpc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fktsv.cn/Article/details/galxpvzaa.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fktsv.cn/Article/details/gslwdmdnz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fktsv.cn/Article/details/gtonmszfr.sHtML


<!-- 参考信息 -->