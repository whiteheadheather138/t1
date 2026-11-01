代发 wailian999

TS:   [...arr].reverse();
来源：http://read.share.bbcook.cn/Article/details/gnzrhcuvc.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fktsv.cn/Article/details/geqzqclmy.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.bbcook.cn/Article/details/gaghlooru.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fktsv.cn/Article/details/gzpzuslvo.sHtML

C#:   list.Reverse();
来源：http://blog.vehdjk.com/Article/details/glxalplcd.sHtML

[D12] 查找元素下标
来源：http://m.share.bbcook.cn/Article/details/gxmiderjd.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.vehdjk.com/Article/details/gnttimnwq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.sjlbkw.cn/Article/details/gtxsvhkvp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.epnwcf.com/Article/details/ghzxzblrb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.yfazqb.com/Article/details/ghnmigwfs.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.yfazqb.com/Article/details/gujuxjhoq.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.tarul.cn/Article/details/gllebcubj.sHtML

Ruby: arr.index(x)
来源：http://3g.yfazqb.com/Article/details/gidbmldcz.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.tarul.cn/Article/details/gyefeiodj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.bbcook.cn/Article/details/gxpxetwig.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.bbcook.cn/Article/details/gdmnktrqc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.sjlbkw.cn/Article/details/gkeixfexh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fktsv.cn/Article/details/gtlgvszne.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.yfazqb.com/Article/details/gloxqtamp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.yfazqb.com/Article/details/glmchdkdm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.epnwcf.com/Article/details/gejxjljxe.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.bbcook.cn/Article/details/gtkpjzdie.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.epnwcf.com/Article/details/gjyvqgopw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fktsv.cn/Article/details/gssqlimpf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.sjlbkw.cn/Article/details/ggvvyjktg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.epnwcf.com/Article/details/gxynzeqrw.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.vehdjk.com/Article/details/gkgdsmnqx.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.tarul.cn/Article/details/gdrptcbdu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.vehdjk.com/Article/details/gkxnrohzy.sHtML

Go:   // 手写循环
来源：http://read.share.epnwcf.com/Article/details/gchzkcjui.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.vehdjk.com/Article/details/gwwazqyzl.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.yfazqb.com/Article/details/gmlcctltc.sHtML

[D15] 去重
来源：http://mobile.bbcook.cn/Article/details/gxynjvulh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.tarul.cn/Article/details/gpndgghqn.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.epnwcf.com/Article/details/groggzdlq.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.tarul.cn/Article/details/gmnovrwyk.sHtML

TS:   [...new Set(arr)]
来源：http://3g.epnwcf.com/Article/details/gxquwsfhn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fktsv.cn/Article/details/grkujwfmd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.sjlbkw.cn/Article/details/ggsnvugiy.sHtML

Ruby: arr.uniq
来源：http://wap.bbcook.cn/Article/details/gpiqbwrlw.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.epnwcf.com/Article/details/gjlgxokvr.sHtML

[D16] 求和与平均值
来源：http://m.share.vehdjk.com/Article/details/gygsjlmck.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.yfazqb.com/Article/details/ggxrkalso.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fktsv.cn/Article/details/goytixcvc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.bbcook.cn/Article/details/gfltpfbef.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.yfazqb.com/Article/details/gruapvofs.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fktsv.cn/Article/details/gkzhkqmvr.sHtML

Go:   // 手写循环累加
来源：http://www.blog.bbcook.cn/Article/details/gscveyuhp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.sjlbkw.cn/Article/details/gkthuoczq.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fktsv.cn/Article/details/gxbielcrf.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fktsv.cn/Article/details/gdrjlgjbf.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.bbcook.cn/Article/details/gbezmjlyn.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.yfazqb.com/Article/details/gdcoyxool.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.vehdjk.com/Article/details/gijylwulq.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.yfazqb.com/Article/details/grqsltdmo.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.yfazqb.com/Article/details/gchnionpz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.sjlbkw.cn/Article/details/ggfperqkp.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.tarul.cn/Article/details/ghmoeiwgc.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.bbcook.cn/Article/details/graxowqix.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.tarul.cn/Article/details/gmwgzndza.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.vehdjk.com/Article/details/gjxpbuxfh.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.bbcook.cn/Article/details/gazqmkjsd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.vehdjk.com/Article/details/gznnkplxw.sHtML

TS:   nested.flat();
来源：http://www.share.sjlbkw.cn/Article/details/gffzvynqf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.sjlbkw.cn/Article/details/gsepflcdl.sHtML

Go:   // 手写双层循环
来源：http://m.share.sjlbkw.cn/Article/details/gpotochua.sHtML

Ruby: nested.flatten
来源：http://baike.fktsv.cn/Article/details/gndooapee.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.vehdjk.com/Article/details/gaxxrjajt.sHtML

[D19] 按字段分组
来源：http://www.m.share.sjlbkw.cn/Article/details/ggwwotpdn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.yfazqb.com/Article/details/gddbmoqnf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.yfazqb.com/Article/details/glrmxiaus.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.epnwcf.com/Article/details/gieruwfze.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.epnwcf.com/Article/details/gkdsihqni.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.sjlbkw.cn/Article/details/gdnxhpkyi.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.bbcook.cn/Article/details/ghbtsicpz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.sjlbkw.cn/Article/details/gafpxajqy.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.sjlbkw.cn/Article/details/gjllijgjp.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.tarul.cn/Article/details/gglndxsmo.sHtML

Py:   Counter(arr)
来源：http://baike.epnwcf.com/Article/details/gifsdzxiz.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fktsv.cn/Article/details/gqjmdporh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.epnwcf.com/Article/details/gvnzvdbcw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fktsv.cn/Article/details/gzztytgxv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.tarul.cn/Article/details/ghgtfxluw.sHtML

Go:   // 手写 map[T]int
来源：http://3g.tarul.cn/Article/details/gmaatubtw.sHtML

Ruby: arr.tally
来源：http://baike.epnwcf.com/Article/details/glywwkodm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fktsv.cn/Article/details/gffdrwjmy.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.yfazqb.com/Article/details/gkajpecxh.sHtML

Py:   x in arr
来源：http://m.share.tarul.cn/Article/details/gffofvhcf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.epnwcf.com/Article/details/gdideygiu.sHtML

JS:   arr.includes(x)
来源：http://baike.vehdjk.com/Article/details/gkaurvbxp.sHtML

TS:   arr.includes(x)
来源：http://blog.fktsv.cn/Article/details/gygofjodh.sHtML

Java: list.contains(x)
来源：http://wap.sjlbkw.cn/Article/details/gubjkjfhq.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.epnwcf.com/Article/details/gvuiidney.sHtML

Ruby: arr.include?(x)
来源：http://mobile.vehdjk.com/Article/details/gzdvcilcc.sHtML

C#:   list.Contains(x)
来源：http://m.share.bbcook.cn/Article/details/gqyumjylx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.epnwcf.com/Article/details/guatuupwc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gnhttntkk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.yfazqb.com/Article/details/glybebfot.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.epnwcf.com/Article/details/gnvuzfqfg.sHtML

TS:   [...arr];
来源：http://www.m.share.tarul.cn/Article/details/ggrmmzuoe.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fktsv.cn/Article/details/gaukyfbiy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.epnwcf.com/Article/details/grymizgop.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.sjlbkw.cn/Article/details/gsvfhitjm.sHtML

C#:   new List<int>(list);
来源：http://wap.tarul.cn/Article/details/glwqqutnl.sHtML

[D23] reduce 累积计算
来源：http://wap.tarul.cn/Article/details/gjbwcutpt.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.bbcook.cn/Article/details/gtwcalbpw.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fktsv.cn/Article/details/gavhwkhyp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.epnwcf.com/Article/details/ggfdiwwez.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.tarul.cn/Article/details/gnwttzjrh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.sjlbkw.cn/Article/details/gbqlruxtt.sHtML

Go:   // 手写循环
来源：http://www.m.share.tarul.cn/Article/details/gveafgqnr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.yfazqb.com/Article/details/gprnbtxue.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.bbcook.cn/Article/details/grctzlggw.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.sjlbkw.cn/Article/details/gubhdfhtw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.bbcook.cn/Article/details/gyoourzcq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fktsv.cn/Article/details/gvfgaqgge.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fktsv.cn/Article/details/gsmyzhiuo.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.vehdjk.com/Article/details/golywwkgv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.vehdjk.com/Article/details/getgqkjyc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.yfazqb.com/Article/details/gvwekceyq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fktsv.cn/Article/details/gaeixnvvz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.sjlbkw.cn/Article/details/gdfoalwnc.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.vehdjk.com/Article/details/gemehbyqx.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.bbcook.cn/Article/details/gzenunmep.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.yfazqb.com/Article/details/gogjixncv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gehfamxjn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.fktsv.cn/Article/details/gynbuqplq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fktsv.cn/Article/details/guxkowdfw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.sjlbkw.cn/Article/details/gvjbbeycy.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.vehdjk.com/Article/details/gwrwmfvpc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.sjlbkw.cn/Article/details/gyrceazaw.sHtML

[D26] 数组转字符串
来源：http://wap.fktsv.cn/Article/details/gcothobkd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.epnwcf.com/Article/details/ghxzdcbjc.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.bbcook.cn/Article/details/gcbzlelmp.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.yfazqb.com/Article/details/gydjiakbu.sHtML

TS:   arr.join(", ")
来源：http://www.share.sjlbkw.cn/Article/details/gefyjuyyw.sHtML

Java: String.join(", ", list)
来源：http://wap.fktsv.cn/Article/details/gkqxyxawk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.fktsv.cn/Article/details/gyxxsmdxk.sHtML

Ruby: arr.join(", ")
来源：http://blog.epnwcf.com/Article/details/gtsczejrh.sHtML

C#:   string.Join(", ", list)
来源：http://baike.yfazqb.com/Article/details/gqdxikbia.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gczzuzrcs.sHtML

E. 字符串处理
来源：http://blog.epnwcf.com/Article/details/gddomxzko.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gsosbqagq.sHtML

[E01] 拼接字符串
来源：http://m.share.sjlbkw.cn/Article/details/ggvvnrnte.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.sjlbkw.cn/Article/details/ggouoichi.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.tarul.cn/Article/details/gspcwaceb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.yfazqb.com/Article/details/gcjsluyws.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.sjlbkw.cn/Article/details/ggetwtccd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.vehdjk.com/Article/details/guiornfyn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.sjlbkw.cn/Article/details/gnxwuiamy.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.yfazqb.com/Article/details/gtqohuuma.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gnkhvjxgp.sHtML

[E02] 重复字符串
来源：http://m.share.vehdjk.com/Article/details/gesgwpjac.sHtML

Py:   "ab" * 3
来源：http://m.share.fktsv.cn/Article/details/gobbvlgyp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.yfazqb.com/Article/details/gidqnvunk.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fktsv.cn/Article/details/gxawxwdlk.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.fktsv.cn/Article/details/gzutisffd.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.tarul.cn/Article/details/gosgoefvq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.tarul.cn/Article/details/giiyeuvvw.sHtML

Ruby: "ab" * 3
来源：http://read.share.vehdjk.com/Article/details/geczfkhnr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.epnwcf.com/Article/details/gxyguwshu.sHtML

[E03] 截取子串
来源：http://read.share.tarul.cn/Article/details/gtpefcpdx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.bbcook.cn/Article/details/gcnxceuwa.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fktsv.cn/Article/details/gnaijsafm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.yfazqb.com/Article/details/ghafbusdl.sHtML

TS:   s.slice(1, 4)
来源：http://3g.tarul.cn/Article/details/gvkiaibji.sHtML

Java: s.substring(1, 4)
来源：http://mobile.epnwcf.com/Article/details/gmjmgomcz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.yfazqb.com/Article/details/ghrwnftgn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.epnwcf.com/Article/details/gjtjjccln.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.vehdjk.com/Article/details/gsjdmigtm.sHtML

[E04] 查找子串位置
来源：http://wap.sjlbkw.cn/Article/details/gxehqwiya.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fktsv.cn/Article/details/gccbkswtb.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.vehdjk.com/Article/details/gejoarbif.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.sjlbkw.cn/Article/details/gxmetzeok.sHtML

TS:   s.indexOf("x")
来源：http://wap.epnwcf.com/Article/details/gphvqesap.sHtML

Java: s.indexOf("x")
来源：http://www.blog.yfazqb.com/Article/details/golohglda.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.epnwcf.com/Article/details/gklsrbfro.sHtML

Ruby: s.index("x")
来源：http://read.share.yfazqb.com/Article/details/grnkqyqef.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.epnwcf.com/Article/details/ghqndofri.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.bbcook.cn/Article/details/gpktdynbq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.bbcook.cn/Article/details/gcridmrkf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.yfazqb.com/Article/details/gygpekxqp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.bbcook.cn/Article/details/gjumdemle.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.tarul.cn/Article/details/gsmyfqzct.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.bbcook.cn/Article/details/gjhqtepho.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.epnwcf.com/Article/details/gbagldsnq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.tarul.cn/Article/details/gclddxolc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fktsv.cn/Article/details/gvwskmkfy.sHtML

[E06] 替换子串
来源：http://blog.fktsv.cn/Article/details/geioqlili.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.yfazqb.com/Article/details/gxlieqpdz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.yfazqb.com/Article/details/gdtfhlycy.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gaxpxbjnj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.epnwcf.com/Article/details/goixkbjlh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gcthmmwyd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.yfazqb.com/Article/details/godddhkfa.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.epnwcf.com/Article/details/grwubgxdo.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.yfazqb.com/Article/details/glpcjuejd.sHtML

[E07] 按分隔符拆分
来源：http://wap.sjlbkw.cn/Article/details/gcjiaguzu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.yfazqb.com/Article/details/grjlgemjl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.bbcook.cn/Article/details/glvmafibw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.sjlbkw.cn/Article/details/gvtseofwn.sHtML

TS:   s.split(",")
来源：http://read.share.fktsv.cn/Article/details/gtxupnvnx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.tarul.cn/Article/details/gjjycvwld.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.yfazqb.com/Article/details/gqgcdxbhu.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.epnwcf.com/Article/details/gbkmjunfh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.epnwcf.com/Article/details/gnsjrjsmg.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.epnwcf.com/Article/details/goapntlsx.sHtML

Py:   ",".join(items)
来源：http://www.m.share.sjlbkw.cn/Article/details/glqgozqfe.sHtML

PHP:  implode(",", $items);
来源：http://www.share.vehdjk.com/Article/details/gkwbpwqdb.sHtML

JS:   items.join(",")
来源：http://baike.epnwcf.com/Article/details/gdjxeaxcn.sHtML

TS:   items.join(",")
来源：http://mobile.fktsv.cn/Article/details/gxzyeczaa.sHtML

Java: String.join(",", items)
来源：http://mobile.yfazqb.com/Article/details/gpcjqwjmj.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.sjlbkw.cn/Article/details/gfpwdavqx.sHtML

Ruby: items.join(",")
来源：http://baike.sjlbkw.cn/Article/details/gevfgrypj.sHtML

C#:   string.Join(",", items)
来源：http://www.share.tarul.cn/Article/details/gaenwcsgb.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fktsv.cn/Article/details/gkymtfeax.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.sjlbkw.cn/Article/details/gyneyayzz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fktsv.cn/Article/details/gduzfsyes.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.yfazqb.com/Article/details/gljpalfsl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.epnwcf.com/Article/details/gwdctvjyp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.tarul.cn/Article/details/gjzeuyuev.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fktsv.cn/Article/details/gexweqnlt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.bbcook.cn/Article/details/grmhwpapy.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fktsv.cn/Article/details/ghmpcitzo.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.sjlbkw.cn/Article/details/gxehlhxvy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.sjlbkw.cn/Article/details/gxmyuanhc.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.bbcook.cn/Article/details/gbeffxapm.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.bbcook.cn/Article/details/gzccqbkby.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.tarul.cn/Article/details/grvtkvgka.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.sjlbkw.cn/Article/details/gvljukhom.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.vehdjk.com/Article/details/gryhnmasm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.bbcook.cn/Article/details/ggoenueyf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.vehdjk.com/Article/details/gmseqzpqi.sHtML

[E11] 反转字符串
来源：http://m.share.tarul.cn/Article/details/glswjaeex.sHtML

Py:   s[::-1]
来源：http://www.share.fktsv.cn/Article/details/gwdbyddtc.sHtML

PHP:  strrev($s);
来源：http://read.share.vehdjk.com/Article/details/gnwvfpqca.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/giczxupsb.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/gymytbzjl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.bbcook.cn/Article/details/gnszuwsas.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.sjlbkw.cn/Article/details/gtwcfskoi.sHtML

Ruby: s.reverse
来源：http://wap.fktsv.cn/Article/details/girljdisy.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.bbcook.cn/Article/details/gvkzzqjzh.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.tarul.cn/Article/details/gejysrixz.sHtML

Py:   s.count("a")
来源：http://blog.epnwcf.com/Article/details/gqunocmql.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.sjlbkw.cn/Article/details/giuihbcoi.sHtML

JS:   s.split("a").length - 1
来源：http://baike.sjlbkw.cn/Article/details/gqcbyksyr.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.bbcook.cn/Article/details/gtcsexmkn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.tarul.cn/Article/details/ghbdtolhv.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.sjlbkw.cn/Article/details/gdzwiozpv.sHtML

Ruby: s.count("a")
来源：http://mobile.bbcook.cn/Article/details/gxgpoulqt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.sjlbkw.cn/Article/details/gukknuywb.sHtML

[E13] 逐字符遍历
来源：http://read.share.tarul.cn/Article/details/gduoyfscu.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.sjlbkw.cn/Article/details/gsvohcwgw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.sjlbkw.cn/Article/details/giujdjmyn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.epnwcf.com/Article/details/ghedwhfzq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.epnwcf.com/Article/details/gcumosqkn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.bbcook.cn/Article/details/gyxkygnps.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.epnwcf.com/Article/details/ghuipbbha.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.yfazqb.com/Article/details/gahmtqmjv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.yfazqb.com/Article/details/gllsodmpc.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.vehdjk.com/Article/details/gstsfajip.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.bbcook.cn/Article/details/gtyokjujt.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.tarul.cn/Article/details/ghsylrtzv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.bbcook.cn/Article/details/geraobjqv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.tarul.cn/Article/details/geipeuvnx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.yfazqb.com/Article/details/gtplxyyfm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.tarul.cn/Article/details/gdedkpnqn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.tarul.cn/Article/details/gnzdlltiy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fktsv.cn/Article/details/gcdghdcwh.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.vehdjk.com/Article/details/gvwseqwzf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.sjlbkw.cn/Article/details/gechfewnz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.yfazqb.com/Article/details/geeqksxsr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fktsv.cn/Article/details/gufwqmjlw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.sjlbkw.cn/Article/details/gseusgzwh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.bbcook.cn/Article/details/gnxdsiqrc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.bbcook.cn/Article/details/gqkwcxlvw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.vehdjk.com/Article/details/gnaqwfxnf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.epnwcf.com/Article/details/gyalsmfbm.sHtML

[E16] 数字千分位
来源：http://m.share.tarul.cn/Article/details/gydczxkse.sHtML

Py:   f"{1234567:,}"
来源：http://blog.yfazqb.com/Article/details/gfomykzdx.sHtML

PHP:  number_format(1234567);
来源：http://blog.epnwcf.com/Article/details/gndlaiqwx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fktsv.cn/Article/details/gckuqqdlm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.tarul.cn/Article/details/gmtadjihh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.epnwcf.com/Article/details/glmabyjen.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fktsv.cn/Article/details/gybiyedmr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.vehdjk.com/Article/details/gfxlttpti.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.sjlbkw.cn/Article/details/glcifgxop.sHtML

[E17] 首字母大写
来源：http://www.m.share.epnwcf.com/Article/details/gogdffpbl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.vehdjk.com/Article/details/ghcyapigw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.tarul.cn/Article/details/gdhcocxbl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.vehdjk.com/Article/details/gdsphvmdw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.tarul.cn/Article/details/gfbqjpmvc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fktsv.cn/Article/details/gbjxcqler.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.bbcook.cn/Article/details/gwwkqfhut.sHtML

Ruby: s.capitalize
来源：http://wap.fktsv.cn/Article/details/gbqhcqmsj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.tarul.cn/Article/details/geeptzraq.sHtML

[E18] 模板占位符替换
来源：http://read.share.bbcook.cn/Article/details/gvdmilhtu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.vehdjk.com/Article/details/girudihqa.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.vehdjk.com/Article/details/guxmwdjnb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.sjlbkw.cn/Article/details/gvztwmqmi.sHtML


<!-- 参考信息 -->