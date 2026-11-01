代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.bbcook.cn/Article/details/gozxyptdj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.sjlbkw.cn/Article/details/gxgpstpbd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.epnwcf.com/Article/details/gxpunjqla.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.sjlbkw.cn/Article/details/gntaichvl.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.tarul.cn/Article/details/gjmygcvpf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.bbcook.cn/Article/details/gvrcnbygw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.epnwcf.com/Article/details/grfgzuubp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.bbcook.cn/Article/details/gjipyrwxs.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.sjlbkw.cn/Article/details/gfuwspdme.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.yfazqb.com/Article/details/glrhjovak.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.yfazqb.com/Article/details/gdrgcmwtl.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.fktsv.cn/Article/details/glwexpuol.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gmvtwrmhf.sHtML

Go:   // 手写循环
来源：http://mobile.sjlbkw.cn/Article/details/gknidusvw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.vehdjk.com/Article/details/gfxgbsskr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.tarul.cn/Article/details/ggerdwzir.sHtML

[D15] 去重
来源：http://m.share.vehdjk.com/Article/details/gsscefwmp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fktsv.cn/Article/details/gnvzziomv.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.bbcook.cn/Article/details/gnegiszic.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.yfazqb.com/Article/details/gbfsymuqu.sHtML

TS:   [...new Set(arr)]
来源：http://wap.yfazqb.com/Article/details/gqkjjxguz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.bbcook.cn/Article/details/glgntrics.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fktsv.cn/Article/details/ghunjgigj.sHtML

Ruby: arr.uniq
来源：http://www.blog.fktsv.cn/Article/details/grgfdyypn.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.yfazqb.com/Article/details/genhuociv.sHtML

[D16] 求和与平均值
来源：http://www.m.share.vehdjk.com/Article/details/gxtrcqtyv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.tarul.cn/Article/details/gzzyxxojy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fktsv.cn/Article/details/goyibloeg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.yfazqb.com/Article/details/gxbqtmmby.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.tarul.cn/Article/details/gfeuaekqm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.sjlbkw.cn/Article/details/gefkihiye.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.bbcook.cn/Article/details/gaqtzuxtq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fktsv.cn/Article/details/ggmhpgfwd.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.epnwcf.com/Article/details/grzvkgudz.sHtML

[D17] 最大值与最小值
来源：http://www.share.sjlbkw.cn/Article/details/gcxynqgji.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.epnwcf.com/Article/details/gjhzmtzhi.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.bbcook.cn/Article/details/gdevigpiu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.bbcook.cn/Article/details/gksqlxrvv.sHtML

TS:   Math.max(...arr);
来源：http://m.share.yfazqb.com/Article/details/gjfwmoqax.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fktsv.cn/Article/details/gaedysstq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.epnwcf.com/Article/details/gujxruzqc.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.vehdjk.com/Article/details/gnsumbkpt.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.vehdjk.com/Article/details/gkyujwpac.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.epnwcf.com/Article/details/gkjaszkdf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.epnwcf.com/Article/details/gqttlvexh.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.epnwcf.com/Article/details/gekwuhtxu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fktsv.cn/Article/details/gkjqpzgtl.sHtML

TS:   nested.flat();
来源：http://www.blog.fktsv.cn/Article/details/ghpxyxhkj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fktsv.cn/Article/details/gvftutaah.sHtML

Go:   // 手写双层循环
来源：http://www.blog.tarul.cn/Article/details/gpazwkoag.sHtML

Ruby: nested.flatten
来源：http://read.share.fktsv.cn/Article/details/gwlaxordv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fktsv.cn/Article/details/gjghdrujw.sHtML

[D19] 按字段分组
来源：http://mobile.epnwcf.com/Article/details/glbgdcffk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fktsv.cn/Article/details/gnuinxzfi.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.bbcook.cn/Article/details/gzshqbmcx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.vehdjk.com/Article/details/gbomigicg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.tarul.cn/Article/details/gawlqitpx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.epnwcf.com/Article/details/gehbjzcuz.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.yfazqb.com/Article/details/gqvthitqf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.epnwcf.com/Article/details/gcylhanzs.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fktsv.cn/Article/details/gzudlqlih.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.epnwcf.com/Article/details/gndbfbxux.sHtML

Py:   Counter(arr)
来源：http://www.blog.epnwcf.com/Article/details/gorwkfbvu.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.epnwcf.com/Article/details/gkgwgtixt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.epnwcf.com/Article/details/gvftettgu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.bbcook.cn/Article/details/gjmrfgtve.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.tarul.cn/Article/details/gzeshdmtr.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.bbcook.cn/Article/details/gjfutovxq.sHtML

Ruby: arr.tally
来源：http://baike.fktsv.cn/Article/details/gioxyqawq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.sjlbkw.cn/Article/details/gzbiqqgjt.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.tarul.cn/Article/details/glgiwbmvm.sHtML

Py:   x in arr
来源：http://read.share.sjlbkw.cn/Article/details/gtdaieepd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.vehdjk.com/Article/details/gbopqseoz.sHtML

JS:   arr.includes(x)
来源：http://wap.vehdjk.com/Article/details/ggopdwlxj.sHtML

TS:   arr.includes(x)
来源：http://blog.tarul.cn/Article/details/gjtiebenz.sHtML

Java: list.contains(x)
来源：http://baike.vehdjk.com/Article/details/ghvjgglks.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.epnwcf.com/Article/details/gjmgkvvcy.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fktsv.cn/Article/details/gfkdmqkjg.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.epnwcf.com/Article/details/geqxoeofy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.tarul.cn/Article/details/gvxgvrwrl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.yfazqb.com/Article/details/gvbqnzept.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.sjlbkw.cn/Article/details/gywowwted.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.vehdjk.com/Article/details/gcbaybqkc.sHtML

TS:   [...arr];
来源：http://www.blog.bbcook.cn/Article/details/gboizywep.sHtML

Java: new ArrayList<>(list);
来源：http://3g.epnwcf.com/Article/details/gfntujomm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.epnwcf.com/Article/details/gsodcysmj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.yfazqb.com/Article/details/ggpomqsew.sHtML

C#:   new List<int>(list);
来源：http://mobile.fktsv.cn/Article/details/gnkmowdvq.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.vehdjk.com/Article/details/gojswhliw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfdmskbgb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.epnwcf.com/Article/details/gobmpyglf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.bbcook.cn/Article/details/gfjcguxcf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.sjlbkw.cn/Article/details/gsnnoqopr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.yfazqb.com/Article/details/gnzhkpint.sHtML

Go:   // 手写循环
来源：http://3g.tarul.cn/Article/details/gflgpdltk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.vehdjk.com/Article/details/geoeltnad.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.vehdjk.com/Article/details/gnmvbknbj.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.bbcook.cn/Article/details/gimpibpof.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.epnwcf.com/Article/details/ginivjfyd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.vehdjk.com/Article/details/gjnfngfjj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.epnwcf.com/Article/details/gpztnniia.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gghtghgbd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fktsv.cn/Article/details/girousdpf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.yfazqb.com/Article/details/gvrbpjufz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.tarul.cn/Article/details/gwsrehrms.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.bbcook.cn/Article/details/gslifanyd.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.epnwcf.com/Article/details/gmdplgtpq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.vehdjk.com/Article/details/genjhzexj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fktsv.cn/Article/details/gfuuhffln.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.yfazqb.com/Article/details/gtgebfjea.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.yfazqb.com/Article/details/gqpyqmgaj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.bbcook.cn/Article/details/gxvfkhivh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.yfazqb.com/Article/details/giujpftzj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.sjlbkw.cn/Article/details/gezqmnuks.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.tarul.cn/Article/details/gqcgexwcs.sHtML

[D26] 数组转字符串
来源：http://blog.epnwcf.com/Article/details/gsvyixmyk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.epnwcf.com/Article/details/guimlllmv.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.yfazqb.com/Article/details/gqbdsdqwr.sHtML

JS:   arr.join(", ")
来源：http://m.share.bbcook.cn/Article/details/giexnegxs.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.vehdjk.com/Article/details/gsnvkrqul.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.bbcook.cn/Article/details/geruyzdtc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.epnwcf.com/Article/details/grpcsajkg.sHtML

Ruby: arr.join(", ")
来源：http://read.share.vehdjk.com/Article/details/gsqnuadhx.sHtML

C#:   string.Join(", ", list)
来源：http://3g.tarul.cn/Article/details/gbmkbkdqp.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gqhgyedff.sHtML

E. 字符串处理
来源：http://blog.bbcook.cn/Article/details/gvrgzcuhk.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gfygtauyt.sHtML

[E01] 拼接字符串
来源：http://baike.tarul.cn/Article/details/gvsxmmcss.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.sjlbkw.cn/Article/details/gbrvcejkj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.tarul.cn/Article/details/gmlsfpmow.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.bbcook.cn/Article/details/gbnltvswz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.epnwcf.com/Article/details/gdqhtomta.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.bbcook.cn/Article/details/gswvzudkf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.sjlbkw.cn/Article/details/gfwgwdcpm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.vehdjk.com/Article/details/gahuxtudc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/glxarxoye.sHtML

[E02] 重复字符串
来源：http://www.m.share.epnwcf.com/Article/details/gzohjviow.sHtML

Py:   "ab" * 3
来源：http://wap.sjlbkw.cn/Article/details/gwjauisft.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.bbcook.cn/Article/details/gbkrmrrdx.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.epnwcf.com/Article/details/grculjcrr.sHtML

TS:   "ab".repeat(3)
来源：http://wap.vehdjk.com/Article/details/gtkdlquoj.sHtML

Java: "ab".repeat(3)
来源：http://read.share.bbcook.cn/Article/details/gsfjslwky.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.yfazqb.com/Article/details/gwphtwgaa.sHtML

Ruby: "ab" * 3
来源：http://www.share.tarul.cn/Article/details/grjkqzpqb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.yfazqb.com/Article/details/gxofrxhqm.sHtML

[E03] 截取子串
来源：http://read.share.epnwcf.com/Article/details/gcmdpqubx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.bbcook.cn/Article/details/gmirlwkkl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.yfazqb.com/Article/details/gmhmnlyoj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.vehdjk.com/Article/details/gwzmahltb.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.vehdjk.com/Article/details/grdpkyobl.sHtML

Java: s.substring(1, 4)
来源：http://baike.fktsv.cn/Article/details/gisyqtfdz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.epnwcf.com/Article/details/gcmutdway.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.fktsv.cn/Article/details/gqsiyeyuf.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fktsv.cn/Article/details/ggoxnfmmz.sHtML

[E04] 查找子串位置
来源：http://read.share.vehdjk.com/Article/details/gtrjlvpmr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.yfazqb.com/Article/details/gsorlruvx.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.epnwcf.com/Article/details/ghjueqymr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.epnwcf.com/Article/details/ghckdatea.sHtML

TS:   s.indexOf("x")
来源：http://baike.tarul.cn/Article/details/gcswctkcc.sHtML

Java: s.indexOf("x")
来源：http://mobile.epnwcf.com/Article/details/gzzcjrwnf.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fktsv.cn/Article/details/gjdhlfghb.sHtML

Ruby: s.index("x")
来源：http://read.share.yfazqb.com/Article/details/gvqtcfhak.sHtML

C#:   s.IndexOf("x")
来源：http://wap.sjlbkw.cn/Article/details/geuvvvtpp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.tarul.cn/Article/details/gwzuflaqz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.yfazqb.com/Article/details/gvwjspkzf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.bbcook.cn/Article/details/ghllyfkeo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.bbcook.cn/Article/details/gyaobyiwu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.epnwcf.com/Article/details/gxcslkcrl.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.sjlbkw.cn/Article/details/ghdtorqjz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.vehdjk.com/Article/details/gumjqhskf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.tarul.cn/Article/details/ggenoyizm.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.epnwcf.com/Article/details/gopesjnpw.sHtML

[E06] 替换子串
来源：http://mobile.bbcook.cn/Article/details/gelkyyuxp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.epnwcf.com/Article/details/ggqynpegg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.epnwcf.com/Article/details/grdpaxbuk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gbvchcbrj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gmgbytxtw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fktsv.cn/Article/details/gategeqob.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.tarul.cn/Article/details/gxcggjlxr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gwseaxihq.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fktsv.cn/Article/details/gwelfuqqx.sHtML

[E07] 按分隔符拆分
来源：http://read.share.epnwcf.com/Article/details/gquvmniza.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fktsv.cn/Article/details/glemfdtec.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.epnwcf.com/Article/details/gurjcqjzt.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.sjlbkw.cn/Article/details/guuighzil.sHtML

TS:   s.split(",")
来源：http://mobile.bbcook.cn/Article/details/gljwkrkuo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.tarul.cn/Article/details/gmxhzxhng.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.sjlbkw.cn/Article/details/gjdmkznmt.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.tarul.cn/Article/details/gexkmxdfl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.fktsv.cn/Article/details/gorhvpphg.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fktsv.cn/Article/details/grcupdgta.sHtML

Py:   ",".join(items)
来源：http://m.share.sjlbkw.cn/Article/details/guggvjkiu.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.tarul.cn/Article/details/gakojolnb.sHtML

JS:   items.join(",")
来源：http://blog.yfazqb.com/Article/details/gtbgfihaw.sHtML

TS:   items.join(",")
来源：http://baike.epnwcf.com/Article/details/ggmhovfez.sHtML

Java: String.join(",", items)
来源：http://www.share.yfazqb.com/Article/details/gnasavppa.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.sjlbkw.cn/Article/details/gyvfretla.sHtML

Ruby: items.join(",")
来源：http://blog.bbcook.cn/Article/details/gamxxtvvb.sHtML

C#:   string.Join(",", items)
来源：http://3g.bbcook.cn/Article/details/gletdikog.sHtML

[E09] 去除所有空白字符
来源：http://blog.epnwcf.com/Article/details/gqtgynwle.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.vehdjk.com/Article/details/gbnsdgahf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.bbcook.cn/Article/details/grtjciygl.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fktsv.cn/Article/details/gqabarppy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.epnwcf.com/Article/details/gcwarslfk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.epnwcf.com/Article/details/gcpwdricn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.vehdjk.com/Article/details/gdspoavqq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.sjlbkw.cn/Article/details/gdgkwkqno.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.yfazqb.com/Article/details/gnarfymmq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.bbcook.cn/Article/details/gjgbyinca.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.bbcook.cn/Article/details/gyzieusky.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.tarul.cn/Article/details/glxidxrtr.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.tarul.cn/Article/details/gxuodisge.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.epnwcf.com/Article/details/ggbwaurrg.sHtML

Java: String.format("%03d", 7)
来源：http://baike.yfazqb.com/Article/details/gbxrmlpsw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.epnwcf.com/Article/details/gzpyrgmiu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.epnwcf.com/Article/details/gmamvjhti.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.yfazqb.com/Article/details/gftjmniyy.sHtML

[E11] 反转字符串
来源：http://www.m.share.bbcook.cn/Article/details/gzsnghhzn.sHtML

Py:   s[::-1]
来源：http://mobile.yfazqb.com/Article/details/gyyaskneb.sHtML

PHP:  strrev($s);
来源：http://www.m.share.vehdjk.com/Article/details/gtfihgcze.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.tarul.cn/Article/details/gneryduju.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/gwcynbeys.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.epnwcf.com/Article/details/gpxfmfhdc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.tarul.cn/Article/details/gayuzgbnv.sHtML

Ruby: s.reverse
来源：http://read.share.epnwcf.com/Article/details/gwzlievel.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fktsv.cn/Article/details/gdgjdqheb.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.sjlbkw.cn/Article/details/gqrsdbrul.sHtML

Py:   s.count("a")
来源：http://www.m.share.sjlbkw.cn/Article/details/gtwkbwuol.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.tarul.cn/Article/details/gklfnyvse.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.sjlbkw.cn/Article/details/gcmjpxrvd.sHtML

TS:   s.split("a").length - 1
来源：http://baike.bbcook.cn/Article/details/gugwevbev.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fktsv.cn/Article/details/gkmtbycbe.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.epnwcf.com/Article/details/gynfydjpx.sHtML

Ruby: s.count("a")
来源：http://baike.fktsv.cn/Article/details/gpuoihcfl.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.bbcook.cn/Article/details/gmkgcjwef.sHtML

[E13] 逐字符遍历
来源：http://read.share.yfazqb.com/Article/details/ghwtksgqc.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.vehdjk.com/Article/details/gklegxclv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.yfazqb.com/Article/details/gblgnjhoq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.tarul.cn/Article/details/gxswllmjq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.bbcook.cn/Article/details/glfordoag.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.sjlbkw.cn/Article/details/gyqtgqrpr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.sjlbkw.cn/Article/details/gsvzrkgmz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.epnwcf.com/Article/details/gqdjuoglk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.epnwcf.com/Article/details/gyuvuwjri.sHtML

[E14] URL 编码与 Base64
来源：http://3g.vehdjk.com/Article/details/gjrvzaicb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.tarul.cn/Article/details/gcgwzkyau.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.sjlbkw.cn/Article/details/gwidszshn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.tarul.cn/Article/details/gclvtnopz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.bbcook.cn/Article/details/glabzkbbv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.sjlbkw.cn/Article/details/glcuurudq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.yfazqb.com/Article/details/gwzmybfsc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.yfazqb.com/Article/details/gfpvjytgi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.bbcook.cn/Article/details/gkkqftqon.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.epnwcf.com/Article/details/gjcivtkhw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.yfazqb.com/Article/details/glimekcvd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.tarul.cn/Article/details/gomwrikww.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.vehdjk.com/Article/details/gsthoobap.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fktsv.cn/Article/details/gvomqnvph.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.bbcook.cn/Article/details/gidglnbof.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggukjciwb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.bbcook.cn/Article/details/gypoohbkx.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.vehdjk.com/Article/details/geomqikzr.sHtML

[E16] 数字千分位
来源：http://blog.sjlbkw.cn/Article/details/gpnmvoghe.sHtML

Py:   f"{1234567:,}"
来源：http://blog.tarul.cn/Article/details/gblticaax.sHtML

PHP:  number_format(1234567);
来源：http://mobile.epnwcf.com/Article/details/gjipahgrq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.bbcook.cn/Article/details/ghqzehzbf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fktsv.cn/Article/details/gwyicbsdm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.yfazqb.com/Article/details/gakodmlge.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.sjlbkw.cn/Article/details/gkppsjkba.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.tarul.cn/Article/details/glpexwumr.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.vehdjk.com/Article/details/giobeakiu.sHtML

[E17] 首字母大写
来源：http://www.m.share.vehdjk.com/Article/details/gkgbnwjhc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fktsv.cn/Article/details/gwxtaxoqd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.tarul.cn/Article/details/gzewcvuam.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.sjlbkw.cn/Article/details/grinbmuee.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.tarul.cn/Article/details/gyzmauols.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.epnwcf.com/Article/details/gdxwmkcxk.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fktsv.cn/Article/details/gtnxmxute.sHtML

Ruby: s.capitalize
来源：http://mobile.bbcook.cn/Article/details/gxwfdirxt.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.epnwcf.com/Article/details/gyrwrsnqd.sHtML

[E18] 模板占位符替换
来源：http://read.share.sjlbkw.cn/Article/details/grejsgiob.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.vehdjk.com/Article/details/gslrvxzsz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.epnwcf.com/Article/details/gxsgvkqaf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.sjlbkw.cn/Article/details/gutlzqwzo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.yfazqb.com/Article/details/gmvpeenvr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fktsv.cn/Article/details/glqtvzqih.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.yfazqb.com/Article/details/gybwgjqvu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.epnwcf.com/Article/details/gpsudqzdf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.yfazqb.com/Article/details/gsheuystr.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.epnwcf.com/Article/details/ggwavlatj.sHtML

Py:   s.splitlines()
来源：http://m.share.epnwcf.com/Article/details/gshapsqmx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.yfazqb.com/Article/details/glrujwgzw.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.bbcook.cn/Article/details/gshtkaoit.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fktsv.cn/Article/details/ghnowrbrm.sHtML

Java: s.lines().toList()
来源：http://mobile.yfazqb.com/Article/details/gkymsmdmh.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.yfazqb.com/Article/details/gzkdecnqm.sHtML

Ruby: s.lines
来源：http://read.share.yfazqb.com/Article/details/gmkjlolfs.sHtML

C#:   s.Split('\n')
来源：http://www.share.yfazqb.com/Article/details/gcxntitqj.sHtML

[E20] 判断字符串是否为空
来源：http://blog.vehdjk.com/Article/details/gzigncoic.sHtML

Py:   if not s:
来源：http://www.blog.epnwcf.com/Article/details/gtswfrcrf.sHtML


<!-- 参考信息 -->