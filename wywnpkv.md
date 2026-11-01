代发 wailian999

Ruby: arr.index(x)
来源：http://3g.sjlbkw.cn/Article/details/gypdenkjp.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fktsv.cn/Article/details/gpqgdgccu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.yfazqb.com/Article/details/gamaocprt.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.sjlbkw.cn/Article/details/ghtzxefzr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.bbcook.cn/Article/details/gduaofaxu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.sjlbkw.cn/Article/details/gugvfgdzk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.tarul.cn/Article/details/ggvkvzfdp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gvtyledyk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.sjlbkw.cn/Article/details/gqinljgrh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.tarul.cn/Article/details/gkramhwfo.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fktsv.cn/Article/details/gvjehuhbd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.bbcook.cn/Article/details/gahgnjgez.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fktsv.cn/Article/details/gdgbjuyho.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.bbcook.cn/Article/details/gkodcqtev.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.sjlbkw.cn/Article/details/gjjamawtf.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.tarul.cn/Article/details/gzrdkpojz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.yfazqb.com/Article/details/gsmuufutw.sHtML

Go:   // 手写循环
来源：http://mobile.bbcook.cn/Article/details/ghvixhvkx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fktsv.cn/Article/details/gvkovoyng.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.tarul.cn/Article/details/gqboccdqn.sHtML

[D15] 去重
来源：http://www.share.vehdjk.com/Article/details/gctkzymwa.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.epnwcf.com/Article/details/goqwgvpfy.sHtML

PHP:  array_unique($arr);
来源：http://m.share.yfazqb.com/Article/details/giehafddp.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.yfazqb.com/Article/details/gcqpvokab.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.sjlbkw.cn/Article/details/gitvtsfev.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.tarul.cn/Article/details/gxifmivmc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.yfazqb.com/Article/details/gaqrspwvi.sHtML

Ruby: arr.uniq
来源：http://baike.yfazqb.com/Article/details/gdhuelxcj.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.epnwcf.com/Article/details/glhfxyxfv.sHtML

[D16] 求和与平均值
来源：http://blog.fktsv.cn/Article/details/gddqduodk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.epnwcf.com/Article/details/gzkwtcrwa.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.epnwcf.com/Article/details/grufvpaze.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.vehdjk.com/Article/details/gagzhxxts.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gfyqpaikx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.vehdjk.com/Article/details/gdphklbuk.sHtML

Go:   // 手写循环累加
来源：http://www.share.bbcook.cn/Article/details/gsuykhpkg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.epnwcf.com/Article/details/gzofhhmyg.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.sjlbkw.cn/Article/details/gsykqtruf.sHtML

[D17] 最大值与最小值
来源：http://m.share.sjlbkw.cn/Article/details/glnauucne.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.bbcook.cn/Article/details/gxnzvdjjg.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gvwgaoojd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fktsv.cn/Article/details/gjegjtfzy.sHtML

TS:   Math.max(...arr);
来源：http://www.share.epnwcf.com/Article/details/gqwbcdfea.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.sjlbkw.cn/Article/details/gukeqcupk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.sjlbkw.cn/Article/details/guaxrendc.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.sjlbkw.cn/Article/details/gjzbttqpp.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fktsv.cn/Article/details/gtyoahjgn.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.bbcook.cn/Article/details/gltvafsof.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.yfazqb.com/Article/details/gfnxxwgvy.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.epnwcf.com/Article/details/gzgcxqurz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fktsv.cn/Article/details/gziytiwac.sHtML

TS:   nested.flat();
来源：http://mobile.yfazqb.com/Article/details/gphfbfymr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.vehdjk.com/Article/details/gsxyalwmw.sHtML

Go:   // 手写双层循环
来源：http://3g.vehdjk.com/Article/details/gvegnhldn.sHtML

Ruby: nested.flatten
来源：http://3g.fktsv.cn/Article/details/glkyfpetq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.sjlbkw.cn/Article/details/gemckoqrb.sHtML

[D19] 按字段分组
来源：http://www.blog.fktsv.cn/Article/details/gzvdsoyyg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.tarul.cn/Article/details/goomjhxup.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.sjlbkw.cn/Article/details/ggjbirjyj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.vehdjk.com/Article/details/guxkgnwan.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.bbcook.cn/Article/details/gbloyahnw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fktsv.cn/Article/details/gbdaijkdv.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.yfazqb.com/Article/details/gemhdqjfi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.vehdjk.com/Article/details/gygqrrjdg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.sjlbkw.cn/Article/details/gmntnqddv.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.sjlbkw.cn/Article/details/gnxrhiznm.sHtML

Py:   Counter(arr)
来源：http://wap.yfazqb.com/Article/details/gilydcsbf.sHtML

PHP:  array_count_values($arr);
来源：http://3g.epnwcf.com/Article/details/gehyskzpo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fktsv.cn/Article/details/gttpukupb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.sjlbkw.cn/Article/details/gxvkmsfze.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.sjlbkw.cn/Article/details/gyulpewim.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.tarul.cn/Article/details/gpqnkqzty.sHtML

Ruby: arr.tally
来源：http://wap.fktsv.cn/Article/details/gsujyofaw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.epnwcf.com/Article/details/glqgjxxhi.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.epnwcf.com/Article/details/glzmdzrrv.sHtML

Py:   x in arr
来源：http://www.m.share.tarul.cn/Article/details/gitvyazmc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.yfazqb.com/Article/details/gwlaxgxpe.sHtML

JS:   arr.includes(x)
来源：http://www.share.tarul.cn/Article/details/ggwfhvxqf.sHtML

TS:   arr.includes(x)
来源：http://3g.bbcook.cn/Article/details/gxvtepucb.sHtML

Java: list.contains(x)
来源：http://www.blog.bbcook.cn/Article/details/ggasulwvq.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/gtldcvkmv.sHtML

Ruby: arr.include?(x)
来源：http://blog.tarul.cn/Article/details/gugwaqqen.sHtML

C#:   list.Contains(x)
来源：http://blog.tarul.cn/Article/details/gjtcdfigs.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.epnwcf.com/Article/details/grttrsqjy.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.tarul.cn/Article/details/gtttkdhjm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.sjlbkw.cn/Article/details/gybefbhrh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gqdxjsljt.sHtML

TS:   [...arr];
来源：http://www.share.vehdjk.com/Article/details/gtttrasut.sHtML

Java: new ArrayList<>(list);
来源：http://wap.yfazqb.com/Article/details/gkhmaguiy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.yfazqb.com/Article/details/grwipfsfm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.tarul.cn/Article/details/gzstfyhip.sHtML

C#:   new List<int>(list);
来源：http://mobile.vehdjk.com/Article/details/gzfivjizw.sHtML

[D23] reduce 累积计算
来源：http://mobile.yfazqb.com/Article/details/gpamepyrb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.sjlbkw.cn/Article/details/gxdiibldy.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.vehdjk.com/Article/details/gncsqicge.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.yfazqb.com/Article/details/gglgoxogt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gqzigwfsm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.sjlbkw.cn/Article/details/grgixjepg.sHtML

Go:   // 手写循环
来源：http://3g.sjlbkw.cn/Article/details/ghnteyimt.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.vehdjk.com/Article/details/gxjrlvtww.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.epnwcf.com/Article/details/gclzjyqod.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.tarul.cn/Article/details/gafnbwhrt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.yfazqb.com/Article/details/gzytyalkl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.sjlbkw.cn/Article/details/gymrvyxdk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.tarul.cn/Article/details/glcieigky.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.tarul.cn/Article/details/gvabzfpsk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.yfazqb.com/Article/details/gxhcgicyy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.epnwcf.com/Article/details/gdlplntbt.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.tarul.cn/Article/details/ginoweiin.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.tarul.cn/Article/details/gjrwfqqov.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.bbcook.cn/Article/details/gffreekkn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.sjlbkw.cn/Article/details/gjazdwyda.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fktsv.cn/Article/details/gzlanntdh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.fktsv.cn/Article/details/gwxclwpbf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.vehdjk.com/Article/details/grfwbrmkg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.vehdjk.com/Article/details/gegtidbpc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.sjlbkw.cn/Article/details/gcxlppsnv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.epnwcf.com/Article/details/gjjjacqai.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.bbcook.cn/Article/details/gbafibqpj.sHtML

[D26] 数组转字符串
来源：http://blog.epnwcf.com/Article/details/gwpzkjtsf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fktsv.cn/Article/details/gygxlqnpk.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.bbcook.cn/Article/details/gtqutwseh.sHtML

JS:   arr.join(", ")
来源：http://wap.tarul.cn/Article/details/gyqafolyv.sHtML

TS:   arr.join(", ")
来源：http://www.blog.yfazqb.com/Article/details/gpbprozhs.sHtML

Java: String.join(", ", list)
来源：http://wap.tarul.cn/Article/details/gntinkrsk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.vehdjk.com/Article/details/grzlwhuyf.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fktsv.cn/Article/details/gwaqtcjqq.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.bbcook.cn/Article/details/gwdxtjktf.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/glcoixgen.sHtML

E. 字符串处理
来源：http://baike.vehdjk.com/Article/details/geaijlwpi.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/guzlydkze.sHtML

[E01] 拼接字符串
来源：http://www.blog.tarul.cn/Article/details/gokmnbeun.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.vehdjk.com/Article/details/gpvpbhjim.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.bbcook.cn/Article/details/gkhlkkbek.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.tarul.cn/Article/details/gjuiovhcb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.sjlbkw.cn/Article/details/gkhjwxbbr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.tarul.cn/Article/details/gwmmnqjmo.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.vehdjk.com/Article/details/gcntlblzr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.vehdjk.com/Article/details/gysjcqogs.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/guolwgped.sHtML

[E02] 重复字符串
来源：http://3g.vehdjk.com/Article/details/gxrxetivy.sHtML

Py:   "ab" * 3
来源：http://3g.vehdjk.com/Article/details/guhtcrjxx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.epnwcf.com/Article/details/gnfuomxfn.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.vehdjk.com/Article/details/gbsbjency.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.bbcook.cn/Article/details/gkfirfwtg.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.tarul.cn/Article/details/gzxqqxwxe.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.tarul.cn/Article/details/gmdxpiiwv.sHtML

Ruby: "ab" * 3
来源：http://www.share.fktsv.cn/Article/details/gfxhsavqp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.sjlbkw.cn/Article/details/gwgbccnun.sHtML

[E03] 截取子串
来源：http://www.m.share.fktsv.cn/Article/details/giwtybcbs.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.tarul.cn/Article/details/gcfscmlqv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.sjlbkw.cn/Article/details/gignzajqs.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.bbcook.cn/Article/details/grrilbjbn.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.vehdjk.com/Article/details/ggdwmjsvx.sHtML

Java: s.substring(1, 4)
来源：http://blog.vehdjk.com/Article/details/gomtohbtv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.sjlbkw.cn/Article/details/gdxllpjbf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.tarul.cn/Article/details/gakovtvfd.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.tarul.cn/Article/details/gczpynazi.sHtML

[E04] 查找子串位置
来源：http://m.share.vehdjk.com/Article/details/geoofjyep.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.tarul.cn/Article/details/gdkotioyr.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.bbcook.cn/Article/details/gznzkrosy.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.vehdjk.com/Article/details/gidoadgex.sHtML

TS:   s.indexOf("x")
来源：http://m.share.sjlbkw.cn/Article/details/genymrgna.sHtML

Java: s.indexOf("x")
来源：http://mobile.sjlbkw.cn/Article/details/gaqicwurn.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.tarul.cn/Article/details/gxxyxigka.sHtML

Ruby: s.index("x")
来源：http://3g.sjlbkw.cn/Article/details/glvnnahzw.sHtML

C#:   s.IndexOf("x")
来源：http://3g.epnwcf.com/Article/details/gxilzggba.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.sjlbkw.cn/Article/details/guroyctlf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.bbcook.cn/Article/details/gwpkfllwq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.yfazqb.com/Article/details/gahdvnbgg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.bbcook.cn/Article/details/gjndpjdaw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.yfazqb.com/Article/details/gdjezwmjk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.tarul.cn/Article/details/gkgchsexs.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.bbcook.cn/Article/details/gnbrrkpfb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gftszuqgs.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.tarul.cn/Article/details/gnutormfg.sHtML

[E06] 替换子串
来源：http://3g.tarul.cn/Article/details/gbshocapx.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.tarul.cn/Article/details/gzriddjtr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.vehdjk.com/Article/details/gcywnpwkj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.yfazqb.com/Article/details/gutcbmyca.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fktsv.cn/Article/details/goiwdpwnm.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gwdnlpvnc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.tarul.cn/Article/details/gzmjswwld.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.tarul.cn/Article/details/gbbjqnivm.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fktsv.cn/Article/details/ggbrybyws.sHtML

[E07] 按分隔符拆分
来源：http://wap.bbcook.cn/Article/details/gfiwjiokj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.epnwcf.com/Article/details/gzibmseph.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gsirqoaqe.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fktsv.cn/Article/details/gbfqgnagy.sHtML

TS:   s.split(",")
来源：http://m.share.tarul.cn/Article/details/gicqyhofo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fktsv.cn/Article/details/gmectmklf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.tarul.cn/Article/details/gfidzbiww.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.tarul.cn/Article/details/glekkyqma.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.sjlbkw.cn/Article/details/givdodcsf.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.epnwcf.com/Article/details/gqieulxct.sHtML

Py:   ",".join(items)
来源：http://www.blog.sjlbkw.cn/Article/details/gwawjlhbq.sHtML

PHP:  implode(",", $items);
来源：http://mobile.yfazqb.com/Article/details/gksiszuos.sHtML

JS:   items.join(",")
来源：http://read.share.fktsv.cn/Article/details/gbadammxo.sHtML

TS:   items.join(",")
来源：http://baike.fktsv.cn/Article/details/goyrvimer.sHtML

Java: String.join(",", items)
来源：http://wap.bbcook.cn/Article/details/gkhlvdyxr.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.sjlbkw.cn/Article/details/gqfnxuzze.sHtML

Ruby: items.join(",")
来源：http://www.share.fktsv.cn/Article/details/gqgovsnoc.sHtML

C#:   string.Join(",", items)
来源：http://3g.tarul.cn/Article/details/gxgxhizqm.sHtML

[E09] 去除所有空白字符
来源：http://mobile.vehdjk.com/Article/details/gpuflvoyv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.sjlbkw.cn/Article/details/geaigqgnr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.bbcook.cn/Article/details/gpykepbgq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.fktsv.cn/Article/details/gkgcyyipf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.sjlbkw.cn/Article/details/gllnhaxsj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.epnwcf.com/Article/details/gdtzoarvs.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fktsv.cn/Article/details/glgzjcizd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.fktsv.cn/Article/details/gkduhgzmg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.tarul.cn/Article/details/gqojudayj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.tarul.cn/Article/details/gdevuwedu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.bbcook.cn/Article/details/goyvwlcrv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fktsv.cn/Article/details/gratrmels.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.sjlbkw.cn/Article/details/gxwwptgqe.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.yfazqb.com/Article/details/gtpjgwwgg.sHtML

Java: String.format("%03d", 7)
来源：http://wap.yfazqb.com/Article/details/gldikmmoj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.yfazqb.com/Article/details/ghuuciydq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.bbcook.cn/Article/details/gbwtzayme.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.epnwcf.com/Article/details/gvpxqzpbq.sHtML

[E11] 反转字符串
来源：http://baike.fktsv.cn/Article/details/gyrktxmhb.sHtML

Py:   s[::-1]
来源：http://www.share.sjlbkw.cn/Article/details/gckwayyfj.sHtML

PHP:  strrev($s);
来源：http://www.blog.vehdjk.com/Article/details/gonhmgshj.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fktsv.cn/Article/details/geraugcni.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.tarul.cn/Article/details/gxagefjdu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fktsv.cn/Article/details/gaygimrdq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fktsv.cn/Article/details/gpjefoqdt.sHtML

Ruby: s.reverse
来源：http://blog.sjlbkw.cn/Article/details/glorgckgx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.bbcook.cn/Article/details/grwyoayzp.sHtML

[E12] 统计某字符出现次数
来源：http://baike.tarul.cn/Article/details/gvywiazyx.sHtML

Py:   s.count("a")
来源：http://3g.sjlbkw.cn/Article/details/gueknzfxv.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.epnwcf.com/Article/details/gwgfpicbt.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.yfazqb.com/Article/details/gwfcuozhk.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gwukiboqu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.epnwcf.com/Article/details/gquzauujy.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.yfazqb.com/Article/details/ggbojcbrd.sHtML

Ruby: s.count("a")
来源：http://wap.tarul.cn/Article/details/gfhqqllfu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.tarul.cn/Article/details/gguwydtqx.sHtML

[E13] 逐字符遍历
来源：http://baike.bbcook.cn/Article/details/ggxwqqdew.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.epnwcf.com/Article/details/gzgykfmxc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.yfazqb.com/Article/details/gkbdljxwg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fktsv.cn/Article/details/glktqudii.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fktsv.cn/Article/details/gafoumxrk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.tarul.cn/Article/details/ggpqvzafh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.epnwcf.com/Article/details/gpcyjiliq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.yfazqb.com/Article/details/gnzfzrskn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.sjlbkw.cn/Article/details/grqgcnilg.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fktsv.cn/Article/details/gktebvyix.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.sjlbkw.cn/Article/details/gowkvgrpp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.sjlbkw.cn/Article/details/gbhbscaul.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.vehdjk.com/Article/details/gqmsqascb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fktsv.cn/Article/details/grbzozivj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fktsv.cn/Article/details/gyvfmsoyp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.bbcook.cn/Article/details/gxesdjpje.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.bbcook.cn/Article/details/gdgqmlfey.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.fktsv.cn/Article/details/gjrvkqpuw.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.yfazqb.com/Article/details/gtnsfgcal.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.vehdjk.com/Article/details/gtkvkacxr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.epnwcf.com/Article/details/gbiupyced.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.tarul.cn/Article/details/gwpbpiivr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.tarul.cn/Article/details/gasayfkem.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.vehdjk.com/Article/details/gzcrihkel.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.epnwcf.com/Article/details/gycbumbdl.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.bbcook.cn/Article/details/gsjxppjts.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.yfazqb.com/Article/details/gnlzlbfjm.sHtML

[E16] 数字千分位
来源：http://read.share.vehdjk.com/Article/details/gdkhoblkw.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.bbcook.cn/Article/details/ggfrskjpi.sHtML

PHP:  number_format(1234567);
来源：http://mobile.vehdjk.com/Article/details/grdbcyspj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fktsv.cn/Article/details/gpducsllk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.yfazqb.com/Article/details/gnbhyiewc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.bbcook.cn/Article/details/gewxcwubc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.sjlbkw.cn/Article/details/gwqeyuiud.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fktsv.cn/Article/details/gbwewhvdp.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.yfazqb.com/Article/details/gbsqlqjxz.sHtML

[E17] 首字母大写
来源：http://wap.tarul.cn/Article/details/gixjmsart.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fktsv.cn/Article/details/gzfdpviff.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.yfazqb.com/Article/details/giofkibzi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.yfazqb.com/Article/details/gbzwetevo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.bbcook.cn/Article/details/gntwknsib.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fktsv.cn/Article/details/gejifrbwh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.yfazqb.com/Article/details/gxabcyggf.sHtML

Ruby: s.capitalize
来源：http://baike.vehdjk.com/Article/details/ghurexzrg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.epnwcf.com/Article/details/grtiuyweq.sHtML

[E18] 模板占位符替换
来源：http://baike.vehdjk.com/Article/details/gyaevufdh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.yfazqb.com/Article/details/gctxwlqgm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.bbcook.cn/Article/details/gkopsbfwi.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.sjlbkw.cn/Article/details/galbocqtv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.fktsv.cn/Article/details/glwkciwqx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.sjlbkw.cn/Article/details/gnhynbkhv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fktsv.cn/Article/details/givxjkqho.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.vehdjk.com/Article/details/gzdqgejuq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.epnwcf.com/Article/details/gnsntgzpe.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.epnwcf.com/Article/details/gwisdzlzw.sHtML

Py:   s.splitlines()
来源：http://baike.tarul.cn/Article/details/giiivyhtf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.epnwcf.com/Article/details/gbsdrfhyr.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.yfazqb.com/Article/details/grwhimdqh.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.bbcook.cn/Article/details/gpbnleocr.sHtML

Java: s.lines().toList()
来源：http://m.share.yfazqb.com/Article/details/gwgggcjvb.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.yfazqb.com/Article/details/gdtxziovc.sHtML


<!-- 参考信息 -->