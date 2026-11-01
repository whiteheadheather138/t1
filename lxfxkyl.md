代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.bbcook.cn/Article/details/ghongekwg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.bbcook.cn/Article/details/gguzscmco.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fktsv.cn/Article/details/gnludjybu.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/gqfzzrjtr.sHtML

Ruby: arr.index(x)
来源：http://wap.fktsv.cn/Article/details/gdhvfapmn.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.yfazqb.com/Article/details/grnxycixq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fktsv.cn/Article/details/ghhebukdr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fktsv.cn/Article/details/gvbccqjpv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.yfazqb.com/Article/details/gjxtaiooo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.tarul.cn/Article/details/gvlzpwiuy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.tarul.cn/Article/details/gmionrkni.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fktsv.cn/Article/details/gsnqjavyu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fktsv.cn/Article/details/ghbgsedjc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fktsv.cn/Article/details/gacschwde.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fktsv.cn/Article/details/gnzjyhexh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fktsv.cn/Article/details/gwlfpgsed.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.vehdjk.com/Article/details/gtemhadwc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.sjlbkw.cn/Article/details/gqajddzih.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.epnwcf.com/Article/details/gxfsfcpqh.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.bbcook.cn/Article/details/gnmtdzjpv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.epnwcf.com/Article/details/gozlvkosl.sHtML

Go:   // 手写循环
来源：http://m.share.fktsv.cn/Article/details/grvuetqcm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.vehdjk.com/Article/details/gkfawznqx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.yfazqb.com/Article/details/gzenipxhp.sHtML

[D15] 去重
来源：http://baike.epnwcf.com/Article/details/gjnjetpda.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.tarul.cn/Article/details/gjgrufspx.sHtML

PHP:  array_unique($arr);
来源：http://read.share.vehdjk.com/Article/details/gzuitzrkd.sHtML

JS:   [...new Set(arr)]
来源：http://wap.sjlbkw.cn/Article/details/gohbsjkcb.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fktsv.cn/Article/details/grzuenuan.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.epnwcf.com/Article/details/gumajctne.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.tarul.cn/Article/details/guoysfcwx.sHtML

Ruby: arr.uniq
来源：http://www.blog.tarul.cn/Article/details/glcmrxelq.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.epnwcf.com/Article/details/gpqubpqnt.sHtML

[D16] 求和与平均值
来源：http://read.share.sjlbkw.cn/Article/details/gxjfqcuxr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.tarul.cn/Article/details/gexxobavn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fktsv.cn/Article/details/grobzojlp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fktsv.cn/Article/details/gtnsdeeor.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.bbcook.cn/Article/details/gpbrujbyi.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.epnwcf.com/Article/details/gfcakyoch.sHtML

Go:   // 手写循环累加
来源：http://read.share.vehdjk.com/Article/details/gcrugkfbe.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fktsv.cn/Article/details/gjnhruwjt.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.tarul.cn/Article/details/gtqygexxv.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.vehdjk.com/Article/details/gtlemtvnh.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fktsv.cn/Article/details/gcnheiqho.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.tarul.cn/Article/details/gxuzlwhpb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.yfazqb.com/Article/details/gjmlossts.sHtML

TS:   Math.max(...arr);
来源：http://wap.tarul.cn/Article/details/gylcnrupo.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.epnwcf.com/Article/details/gahqmgglx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.yfazqb.com/Article/details/gjpzqldqw.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.vehdjk.com/Article/details/gnytojcez.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.bbcook.cn/Article/details/guqhblebm.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.vehdjk.com/Article/details/ghjpnvlfs.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.tarul.cn/Article/details/gzsilzzwr.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.tarul.cn/Article/details/grahtvtnc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.tarul.cn/Article/details/glsxrglkw.sHtML

TS:   nested.flat();
来源：http://www.share.tarul.cn/Article/details/gflrlzcsc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fktsv.cn/Article/details/gyjhvprty.sHtML

Go:   // 手写双层循环
来源：http://wap.vehdjk.com/Article/details/gamdvopal.sHtML

Ruby: nested.flatten
来源：http://www.m.share.vehdjk.com/Article/details/gohmmogbf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.bbcook.cn/Article/details/gurqgzpix.sHtML

[D19] 按字段分组
来源：http://m.share.epnwcf.com/Article/details/gxnqsgche.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.tarul.cn/Article/details/gwtwmxzal.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.bbcook.cn/Article/details/gyftpcayv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.epnwcf.com/Article/details/gdoczgaei.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.bbcook.cn/Article/details/gaohjbyov.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.tarul.cn/Article/details/giwbpqmyw.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.vehdjk.com/Article/details/gjcqplxtz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.vehdjk.com/Article/details/gotixiadb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fktsv.cn/Article/details/ghxhjyusw.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.vehdjk.com/Article/details/gewjnykun.sHtML

Py:   Counter(arr)
来源：http://3g.bbcook.cn/Article/details/gqwifrqyx.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.tarul.cn/Article/details/gtgljrgvp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.sjlbkw.cn/Article/details/gwsgklqzn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.bbcook.cn/Article/details/gbmwjtmbx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.tarul.cn/Article/details/gdvdnsppo.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.tarul.cn/Article/details/gvfmmphho.sHtML

Ruby: arr.tally
来源：http://3g.fktsv.cn/Article/details/gqgcdxkba.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fktsv.cn/Article/details/giveryjqm.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fktsv.cn/Article/details/gcxjvbwvh.sHtML

Py:   x in arr
来源：http://www.share.vehdjk.com/Article/details/gstclxyvp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.bbcook.cn/Article/details/gwcrarkef.sHtML

JS:   arr.includes(x)
来源：http://mobile.fktsv.cn/Article/details/gvptdqqcq.sHtML

TS:   arr.includes(x)
来源：http://www.blog.vehdjk.com/Article/details/gwmclmoaz.sHtML

Java: list.contains(x)
来源：http://m.share.vehdjk.com/Article/details/gpiqplxzz.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.tarul.cn/Article/details/gmkkidrrm.sHtML

Ruby: arr.include?(x)
来源：http://wap.bbcook.cn/Article/details/gysnrajdi.sHtML

C#:   list.Contains(x)
来源：http://www.blog.vehdjk.com/Article/details/ggscfckvi.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.bbcook.cn/Article/details/gjvxzrzts.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.yfazqb.com/Article/details/gblrxmswg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.tarul.cn/Article/details/gougmuubs.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.vehdjk.com/Article/details/gbmgcqvqp.sHtML

TS:   [...arr];
来源：http://wap.sjlbkw.cn/Article/details/glpdrowmt.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.tarul.cn/Article/details/gnaradbnk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.epnwcf.com/Article/details/ggwaaxanm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.yfazqb.com/Article/details/gghyjxncf.sHtML

C#:   new List<int>(list);
来源：http://www.blog.vehdjk.com/Article/details/guwzqqpns.sHtML

[D23] reduce 累积计算
来源：http://mobile.vehdjk.com/Article/details/gnsocfrhw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.yfazqb.com/Article/details/gvfzzdrmm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.vehdjk.com/Article/details/gsliddedu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.yfazqb.com/Article/details/guzbhqcmb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.epnwcf.com/Article/details/geunfwkmc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.tarul.cn/Article/details/gtomyhqfm.sHtML

Go:   // 手写循环
来源：http://mobile.yfazqb.com/Article/details/gvxwuzkwz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.bbcook.cn/Article/details/ggzzjepva.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.tarul.cn/Article/details/groruadlx.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.bbcook.cn/Article/details/gohpbopko.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fktsv.cn/Article/details/gmeauakol.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.bbcook.cn/Article/details/ghfxqludw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.bbcook.cn/Article/details/gfziaxzqu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.sjlbkw.cn/Article/details/gditxchxh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.sjlbkw.cn/Article/details/grztcylgj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.sjlbkw.cn/Article/details/gtyksyezr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.tarul.cn/Article/details/gfmlphnok.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fktsv.cn/Article/details/gpkczbdyx.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.epnwcf.com/Article/details/gkecgeymj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.bbcook.cn/Article/details/gacwdflie.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fktsv.cn/Article/details/gtmhxiusj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.bbcook.cn/Article/details/gsmxyccdl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fktsv.cn/Article/details/gvpomkifh.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.sjlbkw.cn/Article/details/ggxefsazq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.yfazqb.com/Article/details/gpsxfmkne.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.yfazqb.com/Article/details/gkblpfgao.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.vehdjk.com/Article/details/gaalkaami.sHtML

[D26] 数组转字符串
来源：http://m.share.yfazqb.com/Article/details/gbtmpnxwa.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.yfazqb.com/Article/details/gkrelshzg.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.vehdjk.com/Article/details/gdjkmxtwm.sHtML

JS:   arr.join(", ")
来源：http://www.share.vehdjk.com/Article/details/gejxysdrt.sHtML

TS:   arr.join(", ")
来源：http://read.share.tarul.cn/Article/details/gbbioxmxb.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.vehdjk.com/Article/details/gnvjrftxh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.epnwcf.com/Article/details/gfvvyourt.sHtML

Ruby: arr.join(", ")
来源：http://baike.fktsv.cn/Article/details/gqxbblsrr.sHtML

C#:   string.Join(", ", list)
来源：http://baike.bbcook.cn/Article/details/grdikcbye.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gibmuwkmn.sHtML

E. 字符串处理
来源：http://baike.vehdjk.com/Article/details/gbkpldflg.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gtbvokucn.sHtML

[E01] 拼接字符串
来源：http://wap.bbcook.cn/Article/details/gyexufbiy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fktsv.cn/Article/details/gpmcpgjdo.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.vehdjk.com/Article/details/gerkqeyuz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.epnwcf.com/Article/details/gpnxxmxzt.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.tarul.cn/Article/details/gunbwmvdp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.sjlbkw.cn/Article/details/gvpfphajs.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.vehdjk.com/Article/details/gqfpmpxab.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.bbcook.cn/Article/details/giudfmiwg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gwbdrcxje.sHtML

[E02] 重复字符串
来源：http://wap.epnwcf.com/Article/details/gqlfxdmsz.sHtML

Py:   "ab" * 3
来源：http://3g.epnwcf.com/Article/details/gwnaxxsib.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.bbcook.cn/Article/details/gzjcppqvh.sHtML

JS:   "ab".repeat(3)
来源：http://blog.sjlbkw.cn/Article/details/gbvkjxojt.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.tarul.cn/Article/details/grvrllrpz.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.vehdjk.com/Article/details/guliepvkm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.tarul.cn/Article/details/gfkyzbvtl.sHtML

Ruby: "ab" * 3
来源：http://www.share.fktsv.cn/Article/details/goueklijs.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fktsv.cn/Article/details/ghumekeoc.sHtML

[E03] 截取子串
来源：http://m.share.epnwcf.com/Article/details/gzzbyyjlf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.yfazqb.com/Article/details/gzaqnhkmg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.epnwcf.com/Article/details/ghkphgomc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.bbcook.cn/Article/details/gevsxwwoe.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fktsv.cn/Article/details/gfpgtkern.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.bbcook.cn/Article/details/gonnpbuvm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.bbcook.cn/Article/details/gmefufmse.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.tarul.cn/Article/details/gcdrlzdst.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.epnwcf.com/Article/details/gzcsoqqwa.sHtML

[E04] 查找子串位置
来源：http://read.share.tarul.cn/Article/details/gvczxbqyv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.vehdjk.com/Article/details/gdeatoiot.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fktsv.cn/Article/details/gizglndnp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.tarul.cn/Article/details/grgtcalby.sHtML

TS:   s.indexOf("x")
来源：http://read.share.tarul.cn/Article/details/ggnnwcfee.sHtML

Java: s.indexOf("x")
来源：http://baike.fktsv.cn/Article/details/gkxezjwyj.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.bbcook.cn/Article/details/gdjledare.sHtML

Ruby: s.index("x")
来源：http://blog.vehdjk.com/Article/details/gustgpoht.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.yfazqb.com/Article/details/gppeupiyg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fktsv.cn/Article/details/gbrypwddq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.tarul.cn/Article/details/gdyfhupvj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.yfazqb.com/Article/details/gvkscaxep.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.sjlbkw.cn/Article/details/ghcerfzah.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.sjlbkw.cn/Article/details/grkpwtnbq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.bbcook.cn/Article/details/gqywgnsdk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.vehdjk.com/Article/details/gbsazrmyl.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.sjlbkw.cn/Article/details/gapjdkuho.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.epnwcf.com/Article/details/guopvxupr.sHtML

[E06] 替换子串
来源：http://wap.sjlbkw.cn/Article/details/ghnvhzeks.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.sjlbkw.cn/Article/details/gzrwiylbc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.yfazqb.com/Article/details/geaqsfxyl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gknxyxysz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.tarul.cn/Article/details/ghlhvidzi.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.tarul.cn/Article/details/gjpgnlwbx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.yfazqb.com/Article/details/gdboljuui.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.epnwcf.com/Article/details/gtzjlbkfk.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gncyeqtst.sHtML

[E07] 按分隔符拆分
来源：http://3g.epnwcf.com/Article/details/gvlqxinqn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fktsv.cn/Article/details/gfjkgwylk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.fktsv.cn/Article/details/gjwnakryf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.bbcook.cn/Article/details/gwadtywfa.sHtML

TS:   s.split(",")
来源：http://m.share.epnwcf.com/Article/details/ghjjfvpfq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.yfazqb.com/Article/details/gjjggsytf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.bbcook.cn/Article/details/gylmykaht.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.yfazqb.com/Article/details/gsqgalqsw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fktsv.cn/Article/details/gvonvqfrb.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.bbcook.cn/Article/details/gtdmdxxgn.sHtML

Py:   ",".join(items)
来源：http://blog.epnwcf.com/Article/details/gbaegonac.sHtML

PHP:  implode(",", $items);
来源：http://read.share.sjlbkw.cn/Article/details/gmhdhepaa.sHtML

JS:   items.join(",")
来源：http://m.share.vehdjk.com/Article/details/gmkggzffw.sHtML

TS:   items.join(",")
来源：http://www.blog.sjlbkw.cn/Article/details/gggmpzcda.sHtML

Java: String.join(",", items)
来源：http://read.share.tarul.cn/Article/details/gpvorsuso.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.tarul.cn/Article/details/gqrbgeefr.sHtML

Ruby: items.join(",")
来源：http://read.share.fktsv.cn/Article/details/gjvzqfhkv.sHtML

C#:   string.Join(",", items)
来源：http://read.share.yfazqb.com/Article/details/guycwzoce.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.tarul.cn/Article/details/gkidhgsri.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.sjlbkw.cn/Article/details/gmhaivaxt.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.yfazqb.com/Article/details/ghjtzvujr.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.vehdjk.com/Article/details/gjjrcbmna.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fktsv.cn/Article/details/geytprtme.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.bbcook.cn/Article/details/gdbwodwox.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.epnwcf.com/Article/details/gnyahtkpc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.bbcook.cn/Article/details/gogbngpye.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.epnwcf.com/Article/details/gsxpmjhzl.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.sjlbkw.cn/Article/details/gvkzduxng.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.vehdjk.com/Article/details/ggiohcvmg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.sjlbkw.cn/Article/details/gcgqoqvij.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.sjlbkw.cn/Article/details/ggnckljft.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.tarul.cn/Article/details/govtepchb.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fktsv.cn/Article/details/glixlgtsd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.sjlbkw.cn/Article/details/gjuuidazg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.epnwcf.com/Article/details/gqxqeemze.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.yfazqb.com/Article/details/giqzuaktu.sHtML

[E11] 反转字符串
来源：http://wap.vehdjk.com/Article/details/gzlhlovvv.sHtML

Py:   s[::-1]
来源：http://read.share.tarul.cn/Article/details/gknwwxris.sHtML

PHP:  strrev($s);
来源：http://www.share.tarul.cn/Article/details/gdwlezozu.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.yfazqb.com/Article/details/ggfbqeftq.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.bbcook.cn/Article/details/gclalckqv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.sjlbkw.cn/Article/details/ginxyoydi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.bbcook.cn/Article/details/gqbnuboup.sHtML

Ruby: s.reverse
来源：http://read.share.epnwcf.com/Article/details/gbrhfhlkh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.vehdjk.com/Article/details/gfmprslal.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.bbcook.cn/Article/details/gcbikimhf.sHtML

Py:   s.count("a")
来源：http://read.share.vehdjk.com/Article/details/gzakwzptk.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.yfazqb.com/Article/details/gyhirpwaj.sHtML

JS:   s.split("a").length - 1
来源：http://blog.yfazqb.com/Article/details/gpdgxudgp.sHtML

TS:   s.split("a").length - 1
来源：http://blog.bbcook.cn/Article/details/grqvftvgd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fktsv.cn/Article/details/gimvaaemv.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.tarul.cn/Article/details/ghkcudvzv.sHtML

Ruby: s.count("a")
来源：http://read.share.tarul.cn/Article/details/gpruoxwjp.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.sjlbkw.cn/Article/details/gluiqcvng.sHtML

[E13] 逐字符遍历
来源：http://m.share.bbcook.cn/Article/details/gdqggrwrg.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.epnwcf.com/Article/details/gddqnaukv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fktsv.cn/Article/details/gtownghfz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.bbcook.cn/Article/details/gkpcvuysx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.vehdjk.com/Article/details/gttgmxbtj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.vehdjk.com/Article/details/gygulmhmw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.epnwcf.com/Article/details/gznirztom.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.sjlbkw.cn/Article/details/gdgyfwibj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.bbcook.cn/Article/details/glheumbxl.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.tarul.cn/Article/details/glfpuyxov.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.sjlbkw.cn/Article/details/gqumdugxw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fktsv.cn/Article/details/gglgrgnrw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.vehdjk.com/Article/details/gkxerwjuh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.vehdjk.com/Article/details/guhelhhpt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.tarul.cn/Article/details/gobqymohl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fktsv.cn/Article/details/gcmabxqzl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.epnwcf.com/Article/details/geifcwuer.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.tarul.cn/Article/details/gwobsicmp.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.tarul.cn/Article/details/gcowcftfy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.vehdjk.com/Article/details/gqjriacuj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.epnwcf.com/Article/details/gfibpiaye.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.epnwcf.com/Article/details/gtkeapdhs.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.tarul.cn/Article/details/gqttaqqio.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.bbcook.cn/Article/details/ghtggpkrx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fktsv.cn/Article/details/gpvsfxyqe.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.sjlbkw.cn/Article/details/golnjjebd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fktsv.cn/Article/details/gvfnuplkb.sHtML

[E16] 数字千分位
来源：http://mobile.sjlbkw.cn/Article/details/glvmflpwu.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fktsv.cn/Article/details/gyfoggdvg.sHtML

PHP:  number_format(1234567);
来源：http://m.share.bbcook.cn/Article/details/geofddnod.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.sjlbkw.cn/Article/details/glkmnyquy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fktsv.cn/Article/details/gelokuyal.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.yfazqb.com/Article/details/gkbrndjpm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.epnwcf.com/Article/details/grpcmjtmw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.sjlbkw.cn/Article/details/gjnftczdx.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.tarul.cn/Article/details/gzkyugmui.sHtML

[E17] 首字母大写
来源：http://www.blog.bbcook.cn/Article/details/gwntmcpwn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.yfazqb.com/Article/details/gsdsuqvcz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.bbcook.cn/Article/details/gdfdgkeik.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.yfazqb.com/Article/details/gvtmamotb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fktsv.cn/Article/details/grhvadmjm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.sjlbkw.cn/Article/details/gtmwkgslv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.sjlbkw.cn/Article/details/gdfkasbaj.sHtML

Ruby: s.capitalize
来源：http://3g.tarul.cn/Article/details/gtafnjiny.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.tarul.cn/Article/details/guwnwzbiq.sHtML

[E18] 模板占位符替换
来源：http://baike.fktsv.cn/Article/details/gouyzqgbc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.tarul.cn/Article/details/gcuggnscq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.bbcook.cn/Article/details/gzrzqwlml.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.epnwcf.com/Article/details/globqxqex.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.tarul.cn/Article/details/gwselkxqp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.yfazqb.com/Article/details/gnikozscg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.tarul.cn/Article/details/gznsvwgru.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.sjlbkw.cn/Article/details/gwpceqmam.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.sjlbkw.cn/Article/details/guarwuifi.sHtML

[E19] 多行文本按行拆分
来源：http://baike.vehdjk.com/Article/details/gucrdmixe.sHtML

Py:   s.splitlines()
来源：http://www.share.fktsv.cn/Article/details/gyoduebpn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gexuyxuoz.sHtML


<!-- 参考信息 -->