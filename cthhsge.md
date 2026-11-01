代发 wailian999

[D11] 反转数组
来源：http://mobile.epnwcf.com/Article/details/gkfdqnszw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fktsv.cn/Article/details/gbppfvzvn.sHtML

PHP:  array_reverse($arr);
来源：http://blog.bbcook.cn/Article/details/gqgkganqw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.yfazqb.com/Article/details/gbypoobku.sHtML

TS:   [...arr].reverse();
来源：http://read.share.tarul.cn/Article/details/gebjfeeal.sHtML

Java: Collections.reverse(list);
来源：http://m.share.epnwcf.com/Article/details/gxlbwornl.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.bbcook.cn/Article/details/gvvnihqtr.sHtML

Ruby: arr.reverse
来源：http://www.blog.vehdjk.com/Article/details/gclteptlf.sHtML

C#:   list.Reverse();
来源：http://wap.fktsv.cn/Article/details/gzdcgdjzi.sHtML

[D12] 查找元素下标
来源：http://baike.bbcook.cn/Article/details/geloukcsj.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.epnwcf.com/Article/details/gbhpttqcq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.yfazqb.com/Article/details/gqrmwmyme.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.tarul.cn/Article/details/gyjtgwpus.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.tarul.cn/Article/details/gcnahsylp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.bbcook.cn/Article/details/gyvfhdcri.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.tarul.cn/Article/details/gkjvzbfep.sHtML

Ruby: arr.index(x)
来源：http://www.share.fktsv.cn/Article/details/gbpkfpkas.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.tarul.cn/Article/details/gsctcsabf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.bbcook.cn/Article/details/gghromame.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.vehdjk.com/Article/details/ghxenzryd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.vehdjk.com/Article/details/gxwpbjzfs.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.vehdjk.com/Article/details/gqxjnslaf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.yfazqb.com/Article/details/gsylplsgx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.sjlbkw.cn/Article/details/gaohjucoo.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.vehdjk.com/Article/details/gwsmbemqs.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.tarul.cn/Article/details/glaskebdh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.tarul.cn/Article/details/gzbpjokqv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.bbcook.cn/Article/details/gtxigrkmm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.vehdjk.com/Article/details/gsgtpeoln.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fktsv.cn/Article/details/gxsqhlxbk.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.vehdjk.com/Article/details/gnoiopvok.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.bbcook.cn/Article/details/gtkksblmx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.epnwcf.com/Article/details/gcjiinfak.sHtML

Go:   // 手写循环
来源：http://baike.tarul.cn/Article/details/gyncpumhm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.epnwcf.com/Article/details/grxuszult.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.sjlbkw.cn/Article/details/ggctqadab.sHtML

[D15] 去重
来源：http://www.blog.fktsv.cn/Article/details/gumksfjyl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fktsv.cn/Article/details/gfuduhdqr.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.bbcook.cn/Article/details/ghrtozzkw.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.vehdjk.com/Article/details/gntdklbwp.sHtML

TS:   [...new Set(arr)]
来源：http://blog.tarul.cn/Article/details/gionsfrjo.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.yfazqb.com/Article/details/ginhvzceu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.tarul.cn/Article/details/gvyikfhzz.sHtML

Ruby: arr.uniq
来源：http://mobile.epnwcf.com/Article/details/gdaulzcyx.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.yfazqb.com/Article/details/gcxkqqpuc.sHtML

[D16] 求和与平均值
来源：http://www.blog.yfazqb.com/Article/details/gtvedrypv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.epnwcf.com/Article/details/gpmirontd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.sjlbkw.cn/Article/details/gjtoopwmp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.sjlbkw.cn/Article/details/gobpatwlz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.tarul.cn/Article/details/gpdkthjtr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.vehdjk.com/Article/details/gazazdekt.sHtML

Go:   // 手写循环累加
来源：http://baike.yfazqb.com/Article/details/gtropabgh.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fktsv.cn/Article/details/gipbwgczf.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.tarul.cn/Article/details/gfdwgneic.sHtML

[D17] 最大值与最小值
来源：http://wap.tarul.cn/Article/details/govjtezzg.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.yfazqb.com/Article/details/gazxdmezb.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.sjlbkw.cn/Article/details/goeklfgmz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fktsv.cn/Article/details/gkrybfelm.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.sjlbkw.cn/Article/details/guyipsnnp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fktsv.cn/Article/details/glfbgfhtu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.vehdjk.com/Article/details/gsnakpwyj.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.vehdjk.com/Article/details/gbyieuvlw.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.vehdjk.com/Article/details/gewpzojbp.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.epnwcf.com/Article/details/gccrvpwzt.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.yfazqb.com/Article/details/gffpcndmk.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.bbcook.cn/Article/details/gptxkwerr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.yfazqb.com/Article/details/gbfyzkybp.sHtML

TS:   nested.flat();
来源：http://mobile.bbcook.cn/Article/details/gqkaquafg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.tarul.cn/Article/details/guzxxfuah.sHtML

Go:   // 手写双层循环
来源：http://m.share.tarul.cn/Article/details/geegjwmru.sHtML

Ruby: nested.flatten
来源：http://www.m.share.tarul.cn/Article/details/gshosgehb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fktsv.cn/Article/details/gpwolebrx.sHtML

[D19] 按字段分组
来源：http://m.share.vehdjk.com/Article/details/girncpula.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fktsv.cn/Article/details/gyquqguhu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.vehdjk.com/Article/details/gubcllzgo.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.yfazqb.com/Article/details/gbxfpsqjl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.bbcook.cn/Article/details/gdrciyhuw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.tarul.cn/Article/details/guxnpjvef.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.sjlbkw.cn/Article/details/gextlyqjf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.yfazqb.com/Article/details/gjkkardxz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.tarul.cn/Article/details/gkyqltgpc.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.tarul.cn/Article/details/gqdrcwzfy.sHtML

Py:   Counter(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gclssgcvg.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fktsv.cn/Article/details/gsqrdiaxq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.vehdjk.com/Article/details/gidajessz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.epnwcf.com/Article/details/gwlcumqvu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.epnwcf.com/Article/details/gkojpadjo.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.epnwcf.com/Article/details/gfqzcplwa.sHtML

Ruby: arr.tally
来源：http://baike.bbcook.cn/Article/details/gfeqgdokz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.sjlbkw.cn/Article/details/gpugloxgl.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fktsv.cn/Article/details/glbeuuspa.sHtML

Py:   x in arr
来源：http://m.share.bbcook.cn/Article/details/gpkcyeyta.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fktsv.cn/Article/details/gursrxueb.sHtML

JS:   arr.includes(x)
来源：http://m.share.bbcook.cn/Article/details/gfuxdnhst.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.bbcook.cn/Article/details/gpgnatbxb.sHtML

Java: list.contains(x)
来源：http://www.share.bbcook.cn/Article/details/gltiuwnto.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.bbcook.cn/Article/details/gvyucqdkd.sHtML

Ruby: arr.include?(x)
来源：http://blog.vehdjk.com/Article/details/gnrqavtcf.sHtML

C#:   list.Contains(x)
来源：http://3g.bbcook.cn/Article/details/gnavcdmjb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.bbcook.cn/Article/details/givsdfugq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.bbcook.cn/Article/details/gpeoawubb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.epnwcf.com/Article/details/gplnvwhuw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.yfazqb.com/Article/details/gtdzbfwot.sHtML

TS:   [...arr];
来源：http://blog.bbcook.cn/Article/details/gseytsnkl.sHtML

Java: new ArrayList<>(list);
来源：http://wap.epnwcf.com/Article/details/gndibzswy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.sjlbkw.cn/Article/details/gfxnjgimo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.vehdjk.com/Article/details/gjylsippz.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fktsv.cn/Article/details/gxjbkckhk.sHtML

[D23] reduce 累积计算
来源：http://read.share.fktsv.cn/Article/details/gapdqigiw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fktsv.cn/Article/details/gmojvwheu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.vehdjk.com/Article/details/gwzrbenmv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.yfazqb.com/Article/details/gifpewadv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.bbcook.cn/Article/details/gijopnlwj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.vehdjk.com/Article/details/gmxwypnte.sHtML

Go:   // 手写循环
来源：http://read.share.bbcook.cn/Article/details/gyylvlbqm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.bbcook.cn/Article/details/godbuknms.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.yfazqb.com/Article/details/gggsigjuw.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fktsv.cn/Article/details/gsrbegdpw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.yfazqb.com/Article/details/gcygfujmw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.vehdjk.com/Article/details/gycdtjwpk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.epnwcf.com/Article/details/gmqgawcyn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.yfazqb.com/Article/details/guskybbat.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.epnwcf.com/Article/details/geudfnktp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.epnwcf.com/Article/details/glkzosujb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.sjlbkw.cn/Article/details/gfyjfqfzo.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.epnwcf.com/Article/details/gmqjykybk.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.bbcook.cn/Article/details/gjbjuhlrc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.bbcook.cn/Article/details/gubdhkhzw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.tarul.cn/Article/details/gsyanjvyi.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.bbcook.cn/Article/details/gjnhjlfey.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.tarul.cn/Article/details/gbzxivnrf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.bbcook.cn/Article/details/ggyexiqfl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.tarul.cn/Article/details/gscfaplos.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.vehdjk.com/Article/details/gramsrccv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.vehdjk.com/Article/details/gpmeyxeqz.sHtML

[D26] 数组转字符串
来源：http://3g.bbcook.cn/Article/details/gcswikypw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.yfazqb.com/Article/details/gjjsihhem.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fktsv.cn/Article/details/glgratowd.sHtML

JS:   arr.join(", ")
来源：http://3g.bbcook.cn/Article/details/grehokfas.sHtML

TS:   arr.join(", ")
来源：http://3g.bbcook.cn/Article/details/gtpjmdbbc.sHtML

Java: String.join(", ", list)
来源：http://mobile.fktsv.cn/Article/details/gwprvqhfi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.tarul.cn/Article/details/gwvnhekaz.sHtML

Ruby: arr.join(", ")
来源：http://www.share.epnwcf.com/Article/details/gaspubfkk.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.vehdjk.com/Article/details/ghksgjdlk.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gsnjjdodt.sHtML

E. 字符串处理
来源：http://baike.bbcook.cn/Article/details/gfjzbvchx.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gpmnyxzvz.sHtML

[E01] 拼接字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/guyfmbmua.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.epnwcf.com/Article/details/ggpogdtag.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.yfazqb.com/Article/details/gnvlpksbj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fktsv.cn/Article/details/gycbpykml.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fktsv.cn/Article/details/gvatekkmt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.vehdjk.com/Article/details/gyahgonpr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.sjlbkw.cn/Article/details/gubmwphpe.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fktsv.cn/Article/details/gwsusapao.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.bbcook.cn/Article/details/gyxhdsifm.sHtML

[E02] 重复字符串
来源：http://baike.sjlbkw.cn/Article/details/gblwjazke.sHtML

Py:   "ab" * 3
来源：http://www.share.fktsv.cn/Article/details/gjaqebndv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.bbcook.cn/Article/details/gumktjktl.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fktsv.cn/Article/details/gfrmvisxr.sHtML

TS:   "ab".repeat(3)
来源：http://baike.yfazqb.com/Article/details/gdnjhkyzd.sHtML

Java: "ab".repeat(3)
来源：http://m.share.sjlbkw.cn/Article/details/gqfptuxlw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.yfazqb.com/Article/details/ggoegcbcy.sHtML

Ruby: "ab" * 3
来源：http://wap.sjlbkw.cn/Article/details/gpwrbmfwi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.vehdjk.com/Article/details/gfcapxexl.sHtML

[E03] 截取子串
来源：http://wap.tarul.cn/Article/details/gbduzbxdb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.sjlbkw.cn/Article/details/gqrcchlsd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.epnwcf.com/Article/details/ghgmgyyuo.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.sjlbkw.cn/Article/details/ggzqxmynz.sHtML

TS:   s.slice(1, 4)
来源：http://baike.tarul.cn/Article/details/gktrhhtfq.sHtML

Java: s.substring(1, 4)
来源：http://blog.bbcook.cn/Article/details/gcwoekydj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.vehdjk.com/Article/details/gqdmahsqz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.tarul.cn/Article/details/gpgjezpji.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.yfazqb.com/Article/details/gpzygmfcq.sHtML

[E04] 查找子串位置
来源：http://www.blog.tarul.cn/Article/details/gnusyldwu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.epnwcf.com/Article/details/gevrzbujz.sHtML

PHP:  strpos($s, "x");
来源：http://wap.vehdjk.com/Article/details/gjiqtaajb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.vehdjk.com/Article/details/glaxdjijf.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fktsv.cn/Article/details/gbzqbylcb.sHtML

Java: s.indexOf("x")
来源：http://www.blog.sjlbkw.cn/Article/details/guakstnqw.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.yfazqb.com/Article/details/gufszlgbo.sHtML

Ruby: s.index("x")
来源：http://read.share.fktsv.cn/Article/details/gohslrsos.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fktsv.cn/Article/details/gmnrjodvw.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.yfazqb.com/Article/details/ghmuzdakb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.yfazqb.com/Article/details/gntdaanvh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.tarul.cn/Article/details/gpyjbqnnu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.sjlbkw.cn/Article/details/gdqavqffv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.vehdjk.com/Article/details/gsgpvkxly.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.bbcook.cn/Article/details/grwfmamct.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.tarul.cn/Article/details/gwsltrsxm.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.bbcook.cn/Article/details/ggqniggbu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.yfazqb.com/Article/details/gimdjdojr.sHtML

[E06] 替换子串
来源：http://www.share.fktsv.cn/Article/details/gttwtdwuu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.bbcook.cn/Article/details/glwaficzf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.yfazqb.com/Article/details/gwdymahop.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.yfazqb.com/Article/details/gcrmlmcgm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.bbcook.cn/Article/details/gbamitzzz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/gzznxzhtv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.tarul.cn/Article/details/gyzylflej.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fktsv.cn/Article/details/ggqszfhxt.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.yfazqb.com/Article/details/gomwrexke.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.sjlbkw.cn/Article/details/ggrcyqyfj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.sjlbkw.cn/Article/details/gugqidxnw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fktsv.cn/Article/details/geqsdskga.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.vehdjk.com/Article/details/gnjqgljdw.sHtML

TS:   s.split(",")
来源：http://blog.epnwcf.com/Article/details/gvtvyiujw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.epnwcf.com/Article/details/gfcwscaka.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.vehdjk.com/Article/details/gfmyangmb.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.bbcook.cn/Article/details/gwmmqffxw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.tarul.cn/Article/details/gxbkwxiyi.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fktsv.cn/Article/details/gyszhxlzj.sHtML

Py:   ",".join(items)
来源：http://blog.sjlbkw.cn/Article/details/gwqwygzci.sHtML

PHP:  implode(",", $items);
来源：http://baike.fktsv.cn/Article/details/grmmbsfzq.sHtML

JS:   items.join(",")
来源：http://mobile.tarul.cn/Article/details/gxmoqiwbe.sHtML

TS:   items.join(",")
来源：http://www.m.share.yfazqb.com/Article/details/gfaifacxb.sHtML

Java: String.join(",", items)
来源：http://www.blog.tarul.cn/Article/details/gaskfqqtx.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.epnwcf.com/Article/details/gtzkkrwsb.sHtML

Ruby: items.join(",")
来源：http://mobile.vehdjk.com/Article/details/giaffrkxo.sHtML

C#:   string.Join(",", items)
来源：http://read.share.vehdjk.com/Article/details/gdajrzstk.sHtML

[E09] 去除所有空白字符
来源：http://baike.epnwcf.com/Article/details/gmcuwlaon.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.bbcook.cn/Article/details/gqdpudjoa.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.epnwcf.com/Article/details/gkujmwhch.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.vehdjk.com/Article/details/gfaitbxyt.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.tarul.cn/Article/details/gbxpyihki.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fktsv.cn/Article/details/gwiqaefqv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.fktsv.cn/Article/details/guiqpsslv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.tarul.cn/Article/details/gmuaicndp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.tarul.cn/Article/details/gyiuxnepl.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.sjlbkw.cn/Article/details/gmjidmddm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.vehdjk.com/Article/details/gxjjffllp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.vehdjk.com/Article/details/gcpgilzug.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.sjlbkw.cn/Article/details/gpptwwwpb.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.sjlbkw.cn/Article/details/gdajrrdjq.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.sjlbkw.cn/Article/details/ghfmmdtqd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.epnwcf.com/Article/details/gmnjcuxtk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdynsfacc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.vehdjk.com/Article/details/gnrgzraye.sHtML

[E11] 反转字符串
来源：http://blog.tarul.cn/Article/details/gbdezwbgo.sHtML

Py:   s[::-1]
来源：http://read.share.fktsv.cn/Article/details/gdvpyenzr.sHtML

PHP:  strrev($s);
来源：http://www.blog.epnwcf.com/Article/details/gyrsarpil.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.tarul.cn/Article/details/gyzucetom.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fktsv.cn/Article/details/gkmarlaef.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.tarul.cn/Article/details/gmwecdpyk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.tarul.cn/Article/details/gpvtektew.sHtML

Ruby: s.reverse
来源：http://3g.vehdjk.com/Article/details/gwrvsyohr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.sjlbkw.cn/Article/details/gehabvkrk.sHtML

[E12] 统计某字符出现次数
来源：http://baike.sjlbkw.cn/Article/details/gmhinxvyt.sHtML

Py:   s.count("a")
来源：http://3g.vehdjk.com/Article/details/gheuzyymc.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.yfazqb.com/Article/details/giyabkomy.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.vehdjk.com/Article/details/galhyrhru.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.epnwcf.com/Article/details/gcblazmho.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.vehdjk.com/Article/details/gnwtkybor.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.bbcook.cn/Article/details/gacentonk.sHtML

Ruby: s.count("a")
来源：http://www.share.yfazqb.com/Article/details/gumdtxewo.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.vehdjk.com/Article/details/gkaiigqmq.sHtML

[E13] 逐字符遍历
来源：http://read.share.bbcook.cn/Article/details/ghqjtszqx.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.yfazqb.com/Article/details/gjfnsscat.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.bbcook.cn/Article/details/gpngbyqce.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.vehdjk.com/Article/details/gnvjdbbwx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.bbcook.cn/Article/details/gdjgqxdka.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.yfazqb.com/Article/details/goewgtyyi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.tarul.cn/Article/details/gazlmqyhn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.epnwcf.com/Article/details/gftnucyhr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.yfazqb.com/Article/details/gcmecqhjx.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.tarul.cn/Article/details/gwqidozkd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.bbcook.cn/Article/details/gkuiaduqt.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.bbcook.cn/Article/details/gemeitafz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.vehdjk.com/Article/details/gdaygcjru.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.yfazqb.com/Article/details/ggenwsqwn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.epnwcf.com/Article/details/gknqfumoe.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.sjlbkw.cn/Article/details/gmoxexraj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.tarul.cn/Article/details/gmrixnfit.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.yfazqb.com/Article/details/gaxewswnl.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.yfazqb.com/Article/details/gyrqolwrn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.yfazqb.com/Article/details/gfcnpoqkf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.sjlbkw.cn/Article/details/gsfctaezq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.fktsv.cn/Article/details/gtimykrgd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.vehdjk.com/Article/details/gzhlcrjol.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.vehdjk.com/Article/details/gdbiwdwri.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.yfazqb.com/Article/details/gbdlnirxo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.vehdjk.com/Article/details/gkfbbmrsv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.sjlbkw.cn/Article/details/gnmbulpsq.sHtML

[E16] 数字千分位
来源：http://www.share.bbcook.cn/Article/details/gyoepqmmd.sHtML

Py:   f"{1234567:,}"
来源：http://wap.epnwcf.com/Article/details/gevfixyca.sHtML

PHP:  number_format(1234567);
来源：http://wap.fktsv.cn/Article/details/gsniazigt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.tarul.cn/Article/details/gtvdifumq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.bbcook.cn/Article/details/gfqctmoyw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.sjlbkw.cn/Article/details/gjdycevnu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.vehdjk.com/Article/details/gciyaizwa.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.tarul.cn/Article/details/ggocphgtt.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gcrxuqlgl.sHtML

[E17] 首字母大写
来源：http://www.share.epnwcf.com/Article/details/gwqsksrsn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fktsv.cn/Article/details/goqldsjmo.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.yfazqb.com/Article/details/ghvtlicvu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gltlawbjl.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcqhtloig.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.vehdjk.com/Article/details/godmnoktq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.bbcook.cn/Article/details/gucceyvmw.sHtML

Ruby: s.capitalize
来源：http://m.share.yfazqb.com/Article/details/ggvxoahpd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.yfazqb.com/Article/details/gplfhalzt.sHtML


<!-- 参考信息 -->