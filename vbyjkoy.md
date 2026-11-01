代发 wailian999

Ruby: arr.index(x)
来源：http://mobile.tarul.cn/Article/details/gjjkodpze.sHtML

C#:   list.IndexOf(x);
来源：http://baike.bbcook.cn/Article/details/gsnzegfoy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.yfazqb.com/Article/details/gkwnvunql.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.sjlbkw.cn/Article/details/grmvbfwvs.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.bbcook.cn/Article/details/gpazjlzni.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.bbcook.cn/Article/details/gfsprtyjo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fktsv.cn/Article/details/gsligyjqm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.bbcook.cn/Article/details/gxqtokbwi.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.epnwcf.com/Article/details/gnnulehzr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.bbcook.cn/Article/details/ggfjeykcu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.tarul.cn/Article/details/gyeztkfpb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.epnwcf.com/Article/details/gahrpglji.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.vehdjk.com/Article/details/gxckvwdls.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.tarul.cn/Article/details/gqyxwetjw.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.bbcook.cn/Article/details/gembcuxzu.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.sjlbkw.cn/Article/details/gwlbubumy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.tarul.cn/Article/details/gdpgsjrcx.sHtML

Go:   // 手写循环
来源：http://www.blog.bbcook.cn/Article/details/gjkaahcrp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.yfazqb.com/Article/details/glakmtnhb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fktsv.cn/Article/details/gsudyfogz.sHtML

[D15] 去重
来源：http://www.m.share.sjlbkw.cn/Article/details/ggysulbxk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.vehdjk.com/Article/details/grjgvnirt.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/ganqnvhcf.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fktsv.cn/Article/details/ghqntqsjk.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.bbcook.cn/Article/details/geiwlmein.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.sjlbkw.cn/Article/details/gaoyzzbxp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.sjlbkw.cn/Article/details/gdndmovgx.sHtML

Ruby: arr.uniq
来源：http://www.blog.fktsv.cn/Article/details/guartpzmz.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.yfazqb.com/Article/details/glpnyxhff.sHtML

[D16] 求和与平均值
来源：http://www.share.fktsv.cn/Article/details/gdsiuysox.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gaqtckuzd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.sjlbkw.cn/Article/details/ggsctnpzn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.sjlbkw.cn/Article/details/gjmwrptjh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.sjlbkw.cn/Article/details/gtayeldmd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.epnwcf.com/Article/details/gkrkkgrqn.sHtML

Go:   // 手写循环累加
来源：http://mobile.bbcook.cn/Article/details/gyfxxsenk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.epnwcf.com/Article/details/gdyyesgat.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.bbcook.cn/Article/details/gmiinyhyj.sHtML

[D17] 最大值与最小值
来源：http://baike.vehdjk.com/Article/details/guijqsliz.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.tarul.cn/Article/details/gaueruicz.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fktsv.cn/Article/details/gegmgofft.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.bbcook.cn/Article/details/gjimnetke.sHtML

TS:   Math.max(...arr);
来源：http://mobile.epnwcf.com/Article/details/gtcvkfdck.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.tarul.cn/Article/details/gfmuekews.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.tarul.cn/Article/details/girmqxujd.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.sjlbkw.cn/Article/details/gzrmamprb.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.tarul.cn/Article/details/gzyvdavcl.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.epnwcf.com/Article/details/gucdrwmhh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fktsv.cn/Article/details/gulxsnptg.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.sjlbkw.cn/Article/details/gbuunmnws.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fktsv.cn/Article/details/gylrgoxlz.sHtML

TS:   nested.flat();
来源：http://wap.vehdjk.com/Article/details/gmiifqege.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.sjlbkw.cn/Article/details/gdlbkeday.sHtML

Go:   // 手写双层循环
来源：http://mobile.bbcook.cn/Article/details/glaxwkugx.sHtML

Ruby: nested.flatten
来源：http://m.share.epnwcf.com/Article/details/gczpyeyug.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.bbcook.cn/Article/details/gepueragu.sHtML

[D19] 按字段分组
来源：http://baike.fktsv.cn/Article/details/gjabptwyq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.tarul.cn/Article/details/gzcworays.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.vehdjk.com/Article/details/gcxurodgo.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.bbcook.cn/Article/details/gvrfposoa.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.tarul.cn/Article/details/gwtkddnfo.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.tarul.cn/Article/details/gfjdjaccc.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.vehdjk.com/Article/details/gdcultstj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.tarul.cn/Article/details/gcizhfsax.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.vehdjk.com/Article/details/gxhggwuxl.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.sjlbkw.cn/Article/details/gnqgqotsr.sHtML

Py:   Counter(arr)
来源：http://www.blog.tarul.cn/Article/details/gwmnistve.sHtML

PHP:  array_count_values($arr);
来源：http://blog.tarul.cn/Article/details/ggtrgxjbk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.sjlbkw.cn/Article/details/gqptudals.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.vehdjk.com/Article/details/gjwgslbaz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.yfazqb.com/Article/details/ghqegqcgl.sHtML

Go:   // 手写 map[T]int
来源：http://blog.vehdjk.com/Article/details/gquoznmzt.sHtML

Ruby: arr.tally
来源：http://www.blog.epnwcf.com/Article/details/gjvgexjui.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fktsv.cn/Article/details/ggvmxtaoq.sHtML

[D21] 判断是否包含某元素
来源：http://3g.vehdjk.com/Article/details/gieguvzux.sHtML

Py:   x in arr
来源：http://3g.epnwcf.com/Article/details/grxlibazj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.yfazqb.com/Article/details/gngnxkaxo.sHtML

JS:   arr.includes(x)
来源：http://mobile.fktsv.cn/Article/details/guexdkjlu.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.bbcook.cn/Article/details/gwybspqxm.sHtML

Java: list.contains(x)
来源：http://mobile.sjlbkw.cn/Article/details/gdfehrnho.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.tarul.cn/Article/details/gmsyhfmgg.sHtML

Ruby: arr.include?(x)
来源：http://www.share.tarul.cn/Article/details/gshdtsdig.sHtML

C#:   list.Contains(x)
来源：http://m.share.bbcook.cn/Article/details/gyydbitek.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.sjlbkw.cn/Article/details/gaiksqpeo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.bbcook.cn/Article/details/gdmcexbhf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.yfazqb.com/Article/details/gdphkegoq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.sjlbkw.cn/Article/details/gllbrqmtz.sHtML

TS:   [...arr];
来源：http://read.share.bbcook.cn/Article/details/gmezlapyn.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fktsv.cn/Article/details/gmnddfslh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.epnwcf.com/Article/details/gsbwvvoik.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.sjlbkw.cn/Article/details/gvrovyhgb.sHtML

C#:   new List<int>(list);
来源：http://wap.sjlbkw.cn/Article/details/gnbcboxak.sHtML

[D23] reduce 累积计算
来源：http://blog.epnwcf.com/Article/details/gchwjhiiu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gocuqllep.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.sjlbkw.cn/Article/details/gsaxtuhyz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.yfazqb.com/Article/details/gqrfxxhoz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.epnwcf.com/Article/details/guboreomo.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkntqocsh.sHtML

Go:   // 手写循环
来源：http://www.blog.tarul.cn/Article/details/gigteeatw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.sjlbkw.cn/Article/details/gyvkxpyvj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.epnwcf.com/Article/details/gnxdvjzlo.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.tarul.cn/Article/details/gyogzbuqq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.yfazqb.com/Article/details/gxjccihag.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.vehdjk.com/Article/details/ghtaljjyg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.sjlbkw.cn/Article/details/gbzdzvkcy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.epnwcf.com/Article/details/gdgennaem.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.bbcook.cn/Article/details/grcmnawtl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.sjlbkw.cn/Article/details/gbbqhxewd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.sjlbkw.cn/Article/details/gukniekhx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.vehdjk.com/Article/details/gqsqydqxl.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.epnwcf.com/Article/details/giaajltsr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.yfazqb.com/Article/details/gssublhxp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fktsv.cn/Article/details/gfrwqamsx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.fktsv.cn/Article/details/gdozkujjf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.bbcook.cn/Article/details/ggyfuacks.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.yfazqb.com/Article/details/gamgbfizx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.vehdjk.com/Article/details/gcudhdgsn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fktsv.cn/Article/details/gvandygeb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fktsv.cn/Article/details/goqvyvydg.sHtML

[D26] 数组转字符串
来源：http://www.blog.fktsv.cn/Article/details/gmidmxrrp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.vehdjk.com/Article/details/gzdglviez.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.sjlbkw.cn/Article/details/gwldmuzat.sHtML

JS:   arr.join(", ")
来源：http://mobile.vehdjk.com/Article/details/grgxwquol.sHtML

TS:   arr.join(", ")
来源：http://www.share.sjlbkw.cn/Article/details/gokebcbfg.sHtML

Java: String.join(", ", list)
来源：http://mobile.yfazqb.com/Article/details/gyfooqnwh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.bbcook.cn/Article/details/gxmwdtcbl.sHtML

Ruby: arr.join(", ")
来源：http://read.share.vehdjk.com/Article/details/glxkvozkk.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fktsv.cn/Article/details/gtqbiughn.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gltamblng.sHtML

E. 字符串处理
来源：http://3g.sjlbkw.cn/Article/details/gqipgybqf.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/ghhefmszf.sHtML

[E01] 拼接字符串
来源：http://baike.tarul.cn/Article/details/gsvjrksbl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.yfazqb.com/Article/details/givqfmfsd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.sjlbkw.cn/Article/details/gixmstbxx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.yfazqb.com/Article/details/gdodylwac.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.epnwcf.com/Article/details/gxauesvqe.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.epnwcf.com/Article/details/gkvxdckmq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.epnwcf.com/Article/details/ghhubhkys.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.bbcook.cn/Article/details/ggqujnyhc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gxotreqvt.sHtML

[E02] 重复字符串
来源：http://www.share.epnwcf.com/Article/details/grceawuhx.sHtML

Py:   "ab" * 3
来源：http://www.blog.epnwcf.com/Article/details/ghqhpzngn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fktsv.cn/Article/details/gognjdgiu.sHtML

JS:   "ab".repeat(3)
来源：http://wap.sjlbkw.cn/Article/details/gydmdrxlv.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.epnwcf.com/Article/details/grsxvslot.sHtML

Java: "ab".repeat(3)
来源：http://baike.yfazqb.com/Article/details/gdrfgrate.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.vehdjk.com/Article/details/glpkrngom.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fktsv.cn/Article/details/gdwwzpbtx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.yfazqb.com/Article/details/gucnhegfj.sHtML

[E03] 截取子串
来源：http://3g.sjlbkw.cn/Article/details/gtehjnyyd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.yfazqb.com/Article/details/glwgjpmfj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.sjlbkw.cn/Article/details/glxcxtppf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.yfazqb.com/Article/details/gvsrqijgp.sHtML

TS:   s.slice(1, 4)
来源：http://blog.yfazqb.com/Article/details/gtexhnplb.sHtML

Java: s.substring(1, 4)
来源：http://mobile.epnwcf.com/Article/details/gwuovotrr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.vehdjk.com/Article/details/gmuurjqql.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.yfazqb.com/Article/details/gnbpbvdbe.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.epnwcf.com/Article/details/gwslpekzs.sHtML

[E04] 查找子串位置
来源：http://baike.vehdjk.com/Article/details/gsetmnzeh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.bbcook.cn/Article/details/gqvtfsjmw.sHtML

PHP:  strpos($s, "x");
来源：http://wap.epnwcf.com/Article/details/gezpppxuw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.sjlbkw.cn/Article/details/gfoafjzsn.sHtML

TS:   s.indexOf("x")
来源：http://wap.sjlbkw.cn/Article/details/ggjjyacyl.sHtML

Java: s.indexOf("x")
来源：http://read.share.sjlbkw.cn/Article/details/gvnmrmtln.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.yfazqb.com/Article/details/gbxgxkjcm.sHtML

Ruby: s.index("x")
来源：http://www.share.tarul.cn/Article/details/gefhhczjm.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.vehdjk.com/Article/details/gomjnnzyu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.tarul.cn/Article/details/goiftvszu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.fktsv.cn/Article/details/gpsafnzcx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.tarul.cn/Article/details/gpcpkpgfj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.sjlbkw.cn/Article/details/ghdvtxnpd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.tarul.cn/Article/details/gatyioxzx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.bbcook.cn/Article/details/gvkitgast.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.bbcook.cn/Article/details/grvswwitq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.bbcook.cn/Article/details/gcclapntf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.bbcook.cn/Article/details/gqeumdcfv.sHtML

[E06] 替换子串
来源：http://wap.bbcook.cn/Article/details/gdzbhvjyi.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.epnwcf.com/Article/details/gvypvlgfq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.sjlbkw.cn/Article/details/gvymrcyuv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.sjlbkw.cn/Article/details/grxmsmtva.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fktsv.cn/Article/details/gfqcvmpjc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.vehdjk.com/Article/details/gpnudwhni.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.sjlbkw.cn/Article/details/gvhqbjhwi.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gbnozvuua.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fktsv.cn/Article/details/gepgvslww.sHtML

[E07] 按分隔符拆分
来源：http://baike.yfazqb.com/Article/details/gbazlfkan.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.vehdjk.com/Article/details/gkjawqeqs.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fktsv.cn/Article/details/gmxxfkcpt.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.epnwcf.com/Article/details/gkknfvvmx.sHtML

TS:   s.split(",")
来源：http://www.blog.tarul.cn/Article/details/gszuqdxmd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.vehdjk.com/Article/details/grdcytgpo.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.tarul.cn/Article/details/grezphvze.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.bbcook.cn/Article/details/gyasmlaxy.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.tarul.cn/Article/details/gpswutdao.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.sjlbkw.cn/Article/details/gfemyamcc.sHtML

Py:   ",".join(items)
来源：http://www.share.tarul.cn/Article/details/gdbrkzehg.sHtML

PHP:  implode(",", $items);
来源：http://3g.sjlbkw.cn/Article/details/gpjkprbgr.sHtML

JS:   items.join(",")
来源：http://wap.yfazqb.com/Article/details/gdldswtdd.sHtML

TS:   items.join(",")
来源：http://wap.yfazqb.com/Article/details/gixbwiygp.sHtML

Java: String.join(",", items)
来源：http://blog.vehdjk.com/Article/details/gdfellfni.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.vehdjk.com/Article/details/gocrgywms.sHtML

Ruby: items.join(",")
来源：http://blog.yfazqb.com/Article/details/gvsqvbqxv.sHtML

C#:   string.Join(",", items)
来源：http://read.share.tarul.cn/Article/details/gkkxrwwpc.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fktsv.cn/Article/details/gujkhmsgo.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.bbcook.cn/Article/details/gwlgbqwjm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.yfazqb.com/Article/details/gmelktbpt.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.fktsv.cn/Article/details/gptsywtls.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.fktsv.cn/Article/details/gwegagvqo.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.vehdjk.com/Article/details/gcqcdgeyj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.vehdjk.com/Article/details/gxlwglpjm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.tarul.cn/Article/details/ghqhicccq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gadbkhsqx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.yfazqb.com/Article/details/gfnsjtspu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.vehdjk.com/Article/details/gngmiajkt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.epnwcf.com/Article/details/gxhbpqmru.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.epnwcf.com/Article/details/gkukexosw.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fktsv.cn/Article/details/gsmtixsnb.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.yfazqb.com/Article/details/gvgkwbiwm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.epnwcf.com/Article/details/gxjxlflht.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.vehdjk.com/Article/details/gmwjhohyb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.vehdjk.com/Article/details/gjkgmxaiw.sHtML

[E11] 反转字符串
来源：http://www.share.yfazqb.com/Article/details/glvvblxdj.sHtML

Py:   s[::-1]
来源：http://mobile.vehdjk.com/Article/details/gxipsogyu.sHtML

PHP:  strrev($s);
来源：http://www.share.epnwcf.com/Article/details/gapfvsoyh.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.tarul.cn/Article/details/gjnzxkwtg.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.bbcook.cn/Article/details/gibplgcxl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fktsv.cn/Article/details/gqfufnwun.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.epnwcf.com/Article/details/gbmdpkgqb.sHtML

Ruby: s.reverse
来源：http://www.blog.epnwcf.com/Article/details/gmjrvousk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fktsv.cn/Article/details/gzwthujjw.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.epnwcf.com/Article/details/gpvpsruld.sHtML

Py:   s.count("a")
来源：http://blog.epnwcf.com/Article/details/gvjctyrns.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fktsv.cn/Article/details/gmgcbdvyq.sHtML

JS:   s.split("a").length - 1
来源：http://blog.bbcook.cn/Article/details/gdzbmilug.sHtML

TS:   s.split("a").length - 1
来源：http://3g.epnwcf.com/Article/details/gbfqlrdiz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.vehdjk.com/Article/details/gfakjgygv.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.bbcook.cn/Article/details/gqclmuokg.sHtML

Ruby: s.count("a")
来源：http://www.share.yfazqb.com/Article/details/gtfqovqpg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.yfazqb.com/Article/details/grmfjqcqw.sHtML

[E13] 逐字符遍历
来源：http://www.share.fktsv.cn/Article/details/gsqepzpbn.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.yfazqb.com/Article/details/gmzwhyuzv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.sjlbkw.cn/Article/details/gposospki.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fktsv.cn/Article/details/gmdvkjgzc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.epnwcf.com/Article/details/gcbhproem.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.bbcook.cn/Article/details/gxwqqyern.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.vehdjk.com/Article/details/ghhbccipq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fktsv.cn/Article/details/gdtnyvlvk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.tarul.cn/Article/details/gaegvrhof.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.yfazqb.com/Article/details/grnvbggdi.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.epnwcf.com/Article/details/gohwcnodw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.sjlbkw.cn/Article/details/gxtrhvets.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.tarul.cn/Article/details/gawnklprc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fktsv.cn/Article/details/gynqodjzk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.yfazqb.com/Article/details/gmtzzhlif.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.tarul.cn/Article/details/gsfubggyd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.yfazqb.com/Article/details/gpxhzmfon.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcgxjlboz.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.epnwcf.com/Article/details/ghwlngocl.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.epnwcf.com/Article/details/gvoseftzm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.tarul.cn/Article/details/golciewai.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fktsv.cn/Article/details/gzndxknkf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.tarul.cn/Article/details/ghyxudxol.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fktsv.cn/Article/details/gdrmpxazf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.vehdjk.com/Article/details/gpfzuqoag.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fktsv.cn/Article/details/gcahymgjd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.yfazqb.com/Article/details/gqmdsmnhw.sHtML

[E16] 数字千分位
来源：http://www.blog.yfazqb.com/Article/details/gvrqhddmb.sHtML

Py:   f"{1234567:,}"
来源：http://blog.bbcook.cn/Article/details/gnsurueeg.sHtML

PHP:  number_format(1234567);
来源：http://blog.sjlbkw.cn/Article/details/gsxoopdip.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.sjlbkw.cn/Article/details/gpommgdhf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.sjlbkw.cn/Article/details/gvidhvmfb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.bbcook.cn/Article/details/gexasexuh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.sjlbkw.cn/Article/details/gykiqpyci.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fktsv.cn/Article/details/ganwcosfo.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.vehdjk.com/Article/details/glzunhadg.sHtML

[E17] 首字母大写
来源：http://www.share.epnwcf.com/Article/details/gsdgsgdbp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.sjlbkw.cn/Article/details/gbuzivsbj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.tarul.cn/Article/details/glshkzrrz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.vehdjk.com/Article/details/gsocrvloq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fktsv.cn/Article/details/gkgtpizzi.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fktsv.cn/Article/details/gxynanyzx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fktsv.cn/Article/details/gdobhrtvv.sHtML

Ruby: s.capitalize
来源：http://3g.yfazqb.com/Article/details/gvdesqkvw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.sjlbkw.cn/Article/details/gtqndirbq.sHtML

[E18] 模板占位符替换
来源：http://mobile.fktsv.cn/Article/details/gqcogsnsw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.sjlbkw.cn/Article/details/gxpwtgylh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.sjlbkw.cn/Article/details/gbzmmxyyr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.vehdjk.com/Article/details/gfcozjyay.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.sjlbkw.cn/Article/details/gdputnrmt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.sjlbkw.cn/Article/details/gbedectco.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.bbcook.cn/Article/details/gmcdxxwqc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.sjlbkw.cn/Article/details/grhzvxcsh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fktsv.cn/Article/details/gccbozcqz.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fktsv.cn/Article/details/gwdndddqo.sHtML

Py:   s.splitlines()
来源：http://blog.bbcook.cn/Article/details/gwzsohmzn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fktsv.cn/Article/details/gduztbodi.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.vehdjk.com/Article/details/gajlzmagb.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.epnwcf.com/Article/details/gisotqbhz.sHtML

Java: s.lines().toList()
来源：http://www.blog.epnwcf.com/Article/details/gbwuojoum.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.epnwcf.com/Article/details/gdatpamdx.sHtML


<!-- 参考信息 -->