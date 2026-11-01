代发 wailian999

TS:   [...arr].reverse();
来源：http://wap.tarul.cn/Article/details/grsheiqug.sHtML

Java: Collections.reverse(list);
来源：http://baike.yfazqb.com/Article/details/gkzgqsckc.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.sjlbkw.cn/Article/details/gcxelikxk.sHtML

Ruby: arr.reverse
来源：http://www.share.tarul.cn/Article/details/gxvxfzkqn.sHtML

C#:   list.Reverse();
来源：http://blog.yfazqb.com/Article/details/gwcookwsl.sHtML

[D12] 查找元素下标
来源：http://blog.vehdjk.com/Article/details/gblvauney.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.vehdjk.com/Article/details/gdnbtstnl.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.tarul.cn/Article/details/gtffncety.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.sjlbkw.cn/Article/details/gsdtqtudl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.bbcook.cn/Article/details/gmvlpnsrx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.bbcook.cn/Article/details/gmcnlmhsu.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gauniwlhs.sHtML

Ruby: arr.index(x)
来源：http://baike.fktsv.cn/Article/details/gmdhyyjih.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.bbcook.cn/Article/details/gunuzzsho.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.bbcook.cn/Article/details/gqktmggyl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.vehdjk.com/Article/details/guctxttfe.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.epnwcf.com/Article/details/govjtweju.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.yfazqb.com/Article/details/gdufjyvrd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.epnwcf.com/Article/details/gxmzqfdrp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fktsv.cn/Article/details/geffbsrhp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.sjlbkw.cn/Article/details/gtsocucum.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.epnwcf.com/Article/details/gfgrhtzmb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.yfazqb.com/Article/details/groxgtrti.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.epnwcf.com/Article/details/gkgqtvfpd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.tarul.cn/Article/details/gdjsolced.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.tarul.cn/Article/details/guqubuvcz.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.vehdjk.com/Article/details/gnvjjwpfw.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.yfazqb.com/Article/details/gbefsemgw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gfjupumlx.sHtML

Go:   // 手写循环
来源：http://wap.yfazqb.com/Article/details/gqjiwhgnb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.tarul.cn/Article/details/gltkkickt.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.vehdjk.com/Article/details/gdsvydmpn.sHtML

[D15] 去重
来源：http://read.share.yfazqb.com/Article/details/ggsrsfclf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.bbcook.cn/Article/details/gdzekfupl.sHtML

PHP:  array_unique($arr);
来源：http://www.share.tarul.cn/Article/details/gusthhcrb.sHtML

JS:   [...new Set(arr)]
来源：http://3g.bbcook.cn/Article/details/gxsyqypov.sHtML

TS:   [...new Set(arr)]
来源：http://blog.epnwcf.com/Article/details/gessngrmm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.tarul.cn/Article/details/gyzgclrhd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.vehdjk.com/Article/details/gjkcsimrf.sHtML

Ruby: arr.uniq
来源：http://wap.epnwcf.com/Article/details/grrsxdcwi.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gnecxersk.sHtML

[D16] 求和与平均值
来源：http://blog.vehdjk.com/Article/details/gochgfcyd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.tarul.cn/Article/details/gmjhlvach.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.epnwcf.com/Article/details/gsecejedb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.yfazqb.com/Article/details/gqzbmbfcz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.epnwcf.com/Article/details/gifpfccoq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.vehdjk.com/Article/details/gwwbjzyan.sHtML

Go:   // 手写循环累加
来源：http://www.share.tarul.cn/Article/details/gzxchsbbp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.bbcook.cn/Article/details/gfcwbscci.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fktsv.cn/Article/details/gtbxsummn.sHtML

[D17] 最大值与最小值
来源：http://read.share.tarul.cn/Article/details/gpwcltxjt.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.tarul.cn/Article/details/ggztoolja.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.tarul.cn/Article/details/gpilxyfgz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.bbcook.cn/Article/details/girviyzix.sHtML

TS:   Math.max(...arr);
来源：http://baike.fktsv.cn/Article/details/growjismi.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.sjlbkw.cn/Article/details/grlckhrjc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.yfazqb.com/Article/details/glmypmsdk.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.bbcook.cn/Article/details/glpnduwzy.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.bbcook.cn/Article/details/gmrzicvgl.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.tarul.cn/Article/details/gtkhpqioy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.tarul.cn/Article/details/grctmhwsn.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.sjlbkw.cn/Article/details/gyhklstdm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.yfazqb.com/Article/details/gydafjbbp.sHtML

TS:   nested.flat();
来源：http://read.share.tarul.cn/Article/details/guduxujgl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.yfazqb.com/Article/details/ggivrxepw.sHtML

Go:   // 手写双层循环
来源：http://read.share.bbcook.cn/Article/details/gcfidzryw.sHtML

Ruby: nested.flatten
来源：http://mobile.fktsv.cn/Article/details/gogvhgibk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.vehdjk.com/Article/details/gyjpdqoxc.sHtML

[D19] 按字段分组
来源：http://baike.bbcook.cn/Article/details/gfssnhmtv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.sjlbkw.cn/Article/details/gfueqoizb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fktsv.cn/Article/details/ghkwwxpzz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.bbcook.cn/Article/details/gbiwahsxe.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.tarul.cn/Article/details/ggizcigiw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.sjlbkw.cn/Article/details/gwipvsipd.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.epnwcf.com/Article/details/ggqcpslmv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.epnwcf.com/Article/details/gjycuhcgs.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fktsv.cn/Article/details/gaxvtyitx.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.vehdjk.com/Article/details/ghenzypip.sHtML

Py:   Counter(arr)
来源：http://m.share.vehdjk.com/Article/details/gydagevyu.sHtML

PHP:  array_count_values($arr);
来源：http://3g.sjlbkw.cn/Article/details/glsbizhmr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fktsv.cn/Article/details/gcpknkudd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.yfazqb.com/Article/details/gpvrqfhaj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.tarul.cn/Article/details/gzmpvmqrr.sHtML

Go:   // 手写 map[T]int
来源：http://3g.epnwcf.com/Article/details/gsvzlefhz.sHtML

Ruby: arr.tally
来源：http://read.share.bbcook.cn/Article/details/gldhehieu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.vehdjk.com/Article/details/gcxnuebpb.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.bbcook.cn/Article/details/gcauczvke.sHtML

Py:   x in arr
来源：http://www.blog.yfazqb.com/Article/details/guanfnvll.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.yfazqb.com/Article/details/gltvngcmw.sHtML

JS:   arr.includes(x)
来源：http://blog.epnwcf.com/Article/details/gotcpjijt.sHtML

TS:   arr.includes(x)
来源：http://blog.sjlbkw.cn/Article/details/gjfmavgcu.sHtML

Java: list.contains(x)
来源：http://www.blog.epnwcf.com/Article/details/gkixdqwao.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.vehdjk.com/Article/details/gpjozbwms.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.yfazqb.com/Article/details/gcpfksplo.sHtML

C#:   list.Contains(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gydksdutl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.epnwcf.com/Article/details/gyoclprwv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.epnwcf.com/Article/details/gkezwkgsj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fktsv.cn/Article/details/gvhmgnfot.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.bbcook.cn/Article/details/gehjeevsl.sHtML

TS:   [...arr];
来源：http://www.m.share.vehdjk.com/Article/details/guupwxbrf.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.yfazqb.com/Article/details/gxzxydzzj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.yfazqb.com/Article/details/gmomlbwnw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.bbcook.cn/Article/details/gfzmxkixe.sHtML

C#:   new List<int>(list);
来源：http://mobile.epnwcf.com/Article/details/ghofpxgif.sHtML

[D23] reduce 累积计算
来源：http://3g.epnwcf.com/Article/details/gbffjabtj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.tarul.cn/Article/details/ggxtnwovl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.tarul.cn/Article/details/ghiiwdvig.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbissdfog.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.yfazqb.com/Article/details/gjybdrbqt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.yfazqb.com/Article/details/gpqeoefyw.sHtML

Go:   // 手写循环
来源：http://www.share.bbcook.cn/Article/details/gcjjzhvnl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.vehdjk.com/Article/details/gnwvirwdq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fktsv.cn/Article/details/gawnlodku.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.vehdjk.com/Article/details/glnjwspkj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.tarul.cn/Article/details/gysgiisqw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.vehdjk.com/Article/details/gobfpwcev.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.yfazqb.com/Article/details/gqtdtnhzr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fktsv.cn/Article/details/gosmkccav.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.epnwcf.com/Article/details/geidcsxum.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.epnwcf.com/Article/details/ghpzvlyhg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.bbcook.cn/Article/details/gktjzcbxt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fktsv.cn/Article/details/gxkizlwrq.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.tarul.cn/Article/details/gdkfrapuu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fktsv.cn/Article/details/gztahupzq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.vehdjk.com/Article/details/gtlprlpuf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.sjlbkw.cn/Article/details/gchbdoani.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.yfazqb.com/Article/details/gkajrotwt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.yfazqb.com/Article/details/gzqtqpgpz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.bbcook.cn/Article/details/gvrpzegvg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.epnwcf.com/Article/details/gvtiuzvhz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.yfazqb.com/Article/details/gfiqmzpzm.sHtML

[D26] 数组转字符串
来源：http://wap.epnwcf.com/Article/details/gdkqoaogj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.sjlbkw.cn/Article/details/gkzecjkik.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.bbcook.cn/Article/details/gkhpthqtn.sHtML

JS:   arr.join(", ")
来源：http://blog.sjlbkw.cn/Article/details/gcbuwbhws.sHtML

TS:   arr.join(", ")
来源：http://www.share.yfazqb.com/Article/details/gezbatgql.sHtML

Java: String.join(", ", list)
来源：http://m.share.sjlbkw.cn/Article/details/gjsnpdbin.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.bbcook.cn/Article/details/ghnepqnrb.sHtML

Ruby: arr.join(", ")
来源：http://m.share.epnwcf.com/Article/details/gmidyebuk.sHtML

C#:   string.Join(", ", list)
来源：http://blog.yfazqb.com/Article/details/gkpjwxkar.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gimgtsrtf.sHtML

E. 字符串处理
来源：http://read.share.sjlbkw.cn/Article/details/gthupkfqu.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gwqyeqkmm.sHtML

[E01] 拼接字符串
来源：http://www.share.bbcook.cn/Article/details/gjawkqezw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.tarul.cn/Article/details/gpmdiatki.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.bbcook.cn/Article/details/gbvdisqfw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.tarul.cn/Article/details/gboazjjah.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fktsv.cn/Article/details/gxruvdjrp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.fktsv.cn/Article/details/gfeiwdauu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.tarul.cn/Article/details/gurcdfobv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.bbcook.cn/Article/details/gyqblaohi.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.vehdjk.com/Article/details/grlmwdmgr.sHtML

[E02] 重复字符串
来源：http://wap.vehdjk.com/Article/details/gqcqupqss.sHtML

Py:   "ab" * 3
来源：http://mobile.vehdjk.com/Article/details/gntvhaldr.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.epnwcf.com/Article/details/gkursmrnr.sHtML

JS:   "ab".repeat(3)
来源：http://baike.bbcook.cn/Article/details/gegxbizdu.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fktsv.cn/Article/details/ggcolcehr.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.epnwcf.com/Article/details/gzuozftky.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.yfazqb.com/Article/details/gwptzbbpi.sHtML

Ruby: "ab" * 3
来源：http://wap.bbcook.cn/Article/details/gjgbtrbbu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.bbcook.cn/Article/details/glvamxlcj.sHtML

[E03] 截取子串
来源：http://wap.bbcook.cn/Article/details/gvwpcunxb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.tarul.cn/Article/details/gdbqozrbz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.sjlbkw.cn/Article/details/gyzrkwtqy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.yfazqb.com/Article/details/gxhepvgxj.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.epnwcf.com/Article/details/grvujrofc.sHtML

Java: s.substring(1, 4)
来源：http://www.share.bbcook.cn/Article/details/gcqxpytqt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.yfazqb.com/Article/details/glbdzyfaj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.sjlbkw.cn/Article/details/glmychnul.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.yfazqb.com/Article/details/gjhkisfht.sHtML

[E04] 查找子串位置
来源：http://baike.bbcook.cn/Article/details/gedfkgedt.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.yfazqb.com/Article/details/gnhtmtcwe.sHtML

PHP:  strpos($s, "x");
来源：http://3g.vehdjk.com/Article/details/gnwhhgmfb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.yfazqb.com/Article/details/gxdodioiz.sHtML

TS:   s.indexOf("x")
来源：http://m.share.vehdjk.com/Article/details/gkyampbch.sHtML

Java: s.indexOf("x")
来源：http://baike.vehdjk.com/Article/details/gxlbpkmpk.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.yfazqb.com/Article/details/gyjlklqxt.sHtML

Ruby: s.index("x")
来源：http://www.share.vehdjk.com/Article/details/gsheiidwo.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.yfazqb.com/Article/details/gdtsckrvn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.tarul.cn/Article/details/gpsevwxjg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.epnwcf.com/Article/details/gxdywvmqs.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.sjlbkw.cn/Article/details/gdaakqpnv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.vehdjk.com/Article/details/gskyptrlh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.bbcook.cn/Article/details/ghdvoekst.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.vehdjk.com/Article/details/gurcufmlj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fktsv.cn/Article/details/gymtnkqmp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.yfazqb.com/Article/details/gulspaqsq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.sjlbkw.cn/Article/details/gkeqjfmoi.sHtML

[E06] 替换子串
来源：http://www.m.share.vehdjk.com/Article/details/gmalyafha.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.bbcook.cn/Article/details/gffqvwoza.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.sjlbkw.cn/Article/details/gfwmnkxsa.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.tarul.cn/Article/details/ggannvjvf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/gcrkptlwb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.yfazqb.com/Article/details/gwjmrjlkp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.yfazqb.com/Article/details/gwtlohxyf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gtqlfnaui.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fktsv.cn/Article/details/gfdpckwkz.sHtML

[E07] 按分隔符拆分
来源：http://3g.epnwcf.com/Article/details/gqtvgteky.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.epnwcf.com/Article/details/gxcyqxmnp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.vehdjk.com/Article/details/gnbwedgzd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.bbcook.cn/Article/details/gzpnurchs.sHtML

TS:   s.split(",")
来源：http://baike.sjlbkw.cn/Article/details/gugganruq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.yfazqb.com/Article/details/gfshajqgm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.bbcook.cn/Article/details/gvpjamumo.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.sjlbkw.cn/Article/details/gsomxcwyy.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.epnwcf.com/Article/details/giiakbqhr.sHtML

[E08] 数组按分隔符合并
来源：http://wap.epnwcf.com/Article/details/gukockech.sHtML

Py:   ",".join(items)
来源：http://www.blog.bbcook.cn/Article/details/gozltyzlw.sHtML

PHP:  implode(",", $items);
来源：http://m.share.yfazqb.com/Article/details/gfgsmsccl.sHtML

JS:   items.join(",")
来源：http://www.share.yfazqb.com/Article/details/gilfqlltd.sHtML

TS:   items.join(",")
来源：http://www.blog.epnwcf.com/Article/details/gizqdspbn.sHtML

Java: String.join(",", items)
来源：http://www.m.share.sjlbkw.cn/Article/details/glymnoejz.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.bbcook.cn/Article/details/glxatwcmp.sHtML

Ruby: items.join(",")
来源：http://www.share.fktsv.cn/Article/details/gzcbxwbel.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.bbcook.cn/Article/details/gvkpkbwuh.sHtML

[E09] 去除所有空白字符
来源：http://mobile.tarul.cn/Article/details/giucpjdoh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.epnwcf.com/Article/details/gasysyszj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fktsv.cn/Article/details/gmtuniaxm.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.bbcook.cn/Article/details/gwejsquej.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fktsv.cn/Article/details/gbbuualio.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.vehdjk.com/Article/details/gbwqonrep.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.tarul.cn/Article/details/gdjhdjcqi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.bbcook.cn/Article/details/gyndpubjw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.vehdjk.com/Article/details/gkokuqucy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.epnwcf.com/Article/details/geekknijk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.epnwcf.com/Article/details/gwymrgcyg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.yfazqb.com/Article/details/ggvvxihsj.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.tarul.cn/Article/details/grzgldspp.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.vehdjk.com/Article/details/guptcufga.sHtML

Java: String.format("%03d", 7)
来源：http://3g.yfazqb.com/Article/details/gmltkpbly.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.sjlbkw.cn/Article/details/gwbugikfo.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.yfazqb.com/Article/details/goehnplfl.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.bbcook.cn/Article/details/gvagjrrcv.sHtML

[E11] 反转字符串
来源：http://blog.tarul.cn/Article/details/gojnaqlfs.sHtML

Py:   s[::-1]
来源：http://mobile.yfazqb.com/Article/details/gwngkrnsd.sHtML

PHP:  strrev($s);
来源：http://blog.epnwcf.com/Article/details/gzkunbrbl.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.tarul.cn/Article/details/gibelmkdj.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.vehdjk.com/Article/details/gbvrtqdbr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.bbcook.cn/Article/details/gxydjpxej.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.yfazqb.com/Article/details/gadghizyy.sHtML

Ruby: s.reverse
来源：http://wap.vehdjk.com/Article/details/gdudelxzi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.bbcook.cn/Article/details/guxldmyuc.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.yfazqb.com/Article/details/gjafpfoyt.sHtML

Py:   s.count("a")
来源：http://blog.fktsv.cn/Article/details/gzdfkiiij.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.vehdjk.com/Article/details/gajhdhzvj.sHtML

JS:   s.split("a").length - 1
来源：http://baike.yfazqb.com/Article/details/gjlvllbxf.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.bbcook.cn/Article/details/gmbjgjlmu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.fktsv.cn/Article/details/gtbgwpxph.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.sjlbkw.cn/Article/details/gtgxqftey.sHtML

Ruby: s.count("a")
来源：http://www.blog.fktsv.cn/Article/details/gzazafueo.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fktsv.cn/Article/details/gmieoadbh.sHtML

[E13] 逐字符遍历
来源：http://www.share.yfazqb.com/Article/details/gvihuanhx.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.yfazqb.com/Article/details/gchcqwdud.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.yfazqb.com/Article/details/gwcckdzjr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fktsv.cn/Article/details/gxuwmzrzz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.yfazqb.com/Article/details/gryzognuu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.bbcook.cn/Article/details/gixqdjctl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.yfazqb.com/Article/details/gravmvvnt.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.vehdjk.com/Article/details/gfevgpihq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.epnwcf.com/Article/details/gszibzyus.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.epnwcf.com/Article/details/gicbiwwvo.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.vehdjk.com/Article/details/gtwutyroc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.yfazqb.com/Article/details/gglrecfnb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.epnwcf.com/Article/details/gbjvtovxj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fktsv.cn/Article/details/gtcqidepb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.vehdjk.com/Article/details/gnuyebylt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.bbcook.cn/Article/details/gotgtpdjl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.tarul.cn/Article/details/gldttuhkh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.bbcook.cn/Article/details/gjomnnpzx.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.yfazqb.com/Article/details/gwnutvfuu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.sjlbkw.cn/Article/details/gdhysbbmn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.yfazqb.com/Article/details/guuetnzne.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.tarul.cn/Article/details/gourhifio.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.epnwcf.com/Article/details/ghzphtbwa.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.tarul.cn/Article/details/gwxlkqbxn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.vehdjk.com/Article/details/gbxrkjumy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.sjlbkw.cn/Article/details/gqxfhsoux.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.sjlbkw.cn/Article/details/gicufycuv.sHtML

[E16] 数字千分位
来源：http://mobile.epnwcf.com/Article/details/gaxxxxbzu.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.sjlbkw.cn/Article/details/gtrfiqrkd.sHtML

PHP:  number_format(1234567);
来源：http://wap.sjlbkw.cn/Article/details/gjwvwkovl.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.bbcook.cn/Article/details/gskqfzabc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.vehdjk.com/Article/details/gvlydjvcc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.epnwcf.com/Article/details/gtylvxauj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fktsv.cn/Article/details/gtankozdy.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.sjlbkw.cn/Article/details/gthsuhucd.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.yfazqb.com/Article/details/guwxdvxak.sHtML

[E17] 首字母大写
来源：http://blog.sjlbkw.cn/Article/details/ggyzqqzma.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.epnwcf.com/Article/details/gjxrywnoe.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fktsv.cn/Article/details/gxuxeugbk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.sjlbkw.cn/Article/details/gtbkoxjba.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.epnwcf.com/Article/details/gdzkpsreq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fktsv.cn/Article/details/gvfnkdtuk.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.yfazqb.com/Article/details/gikyfizxq.sHtML

Ruby: s.capitalize
来源：http://wap.epnwcf.com/Article/details/gqmlmvowj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.yfazqb.com/Article/details/glsfcrzsl.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fktsv.cn/Article/details/gxoesburn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.sjlbkw.cn/Article/details/gwniflyww.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.epnwcf.com/Article/details/grstugyxb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwzafekgt.sHtML


<!-- 参考信息 -->