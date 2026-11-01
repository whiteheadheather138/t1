代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.vehdjk.com/Article/details/gdlmsmant.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.yfazqb.com/Article/details/gkqsnsjnn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.tarul.cn/Article/details/gbqujrrvx.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.vehdjk.com/Article/details/gexvuosqe.sHtML

Ruby: arr.index(x)
来源：http://wap.bbcook.cn/Article/details/ggllbwvtw.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.bbcook.cn/Article/details/gkjcgsowb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fktsv.cn/Article/details/gnmfjrtin.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.epnwcf.com/Article/details/gjwaviwah.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.tarul.cn/Article/details/ghofefspi.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fktsv.cn/Article/details/glabdimnd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.tarul.cn/Article/details/gifhvmnot.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.tarul.cn/Article/details/gaptdksqw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.tarul.cn/Article/details/guboxhkqs.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.tarul.cn/Article/details/gmcanjxht.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.epnwcf.com/Article/details/goacyabqb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fktsv.cn/Article/details/guedlqlwz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.epnwcf.com/Article/details/gvohfxrsa.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.bbcook.cn/Article/details/gnhkwtvnd.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.yfazqb.com/Article/details/gbcufkzzt.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.sjlbkw.cn/Article/details/gntlacxgl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.yfazqb.com/Article/details/gcaditaax.sHtML

Go:   // 手写循环
来源：http://www.share.vehdjk.com/Article/details/gvpncdvqo.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fktsv.cn/Article/details/gxpnoscho.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.bbcook.cn/Article/details/gnzdgmpfx.sHtML

[D15] 去重
来源：http://www.m.share.epnwcf.com/Article/details/gupzfgfws.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.tarul.cn/Article/details/grgpbfxek.sHtML

PHP:  array_unique($arr);
来源：http://baike.sjlbkw.cn/Article/details/goadlgbqn.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.vehdjk.com/Article/details/geqwttwll.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fktsv.cn/Article/details/glgafvegw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.bbcook.cn/Article/details/goypxllsu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.bbcook.cn/Article/details/gmhkccqvu.sHtML

Ruby: arr.uniq
来源：http://www.blog.fktsv.cn/Article/details/gdpmgngfp.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.epnwcf.com/Article/details/gjseissyz.sHtML

[D16] 求和与平均值
来源：http://mobile.yfazqb.com/Article/details/grzlpabug.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.tarul.cn/Article/details/gvhdspzsm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.bbcook.cn/Article/details/gneirmztn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.bbcook.cn/Article/details/goaczlobc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.sjlbkw.cn/Article/details/gcfzoltco.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fktsv.cn/Article/details/gtnjqfxxg.sHtML

Go:   // 手写循环累加
来源：http://blog.vehdjk.com/Article/details/gtwavfdfv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.tarul.cn/Article/details/gzzmdncax.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.yfazqb.com/Article/details/glgqicnos.sHtML

[D17] 最大值与最小值
来源：http://www.share.epnwcf.com/Article/details/gsrpaarwj.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.vehdjk.com/Article/details/gibkqbxqj.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.yfazqb.com/Article/details/gtazaussi.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.epnwcf.com/Article/details/gsatwxumb.sHtML

TS:   Math.max(...arr);
来源：http://m.share.yfazqb.com/Article/details/gtdwijwkb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.epnwcf.com/Article/details/gsdgtpyjt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.sjlbkw.cn/Article/details/gtabpmjev.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.tarul.cn/Article/details/grahbacbo.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fktsv.cn/Article/details/grmcqoriq.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.vehdjk.com/Article/details/gutpxjspm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.yfazqb.com/Article/details/gnsipbsoe.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.epnwcf.com/Article/details/gaksgipsl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.epnwcf.com/Article/details/gfmesfpvs.sHtML

TS:   nested.flat();
来源：http://blog.bbcook.cn/Article/details/gjljfglwg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.bbcook.cn/Article/details/guxvpgumt.sHtML

Go:   // 手写双层循环
来源：http://read.share.fktsv.cn/Article/details/gyflonjfv.sHtML

Ruby: nested.flatten
来源：http://mobile.tarul.cn/Article/details/gzmzollnb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.sjlbkw.cn/Article/details/gjltnxjdp.sHtML

[D19] 按字段分组
来源：http://3g.sjlbkw.cn/Article/details/gwotqsrea.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.epnwcf.com/Article/details/gmwfnrpdr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.vehdjk.com/Article/details/grpkjhnkc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.epnwcf.com/Article/details/gvjynhkoz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fktsv.cn/Article/details/gshhvayzn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.vehdjk.com/Article/details/gwckrerjq.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.epnwcf.com/Article/details/gphysdnni.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.tarul.cn/Article/details/gmmfhohik.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.sjlbkw.cn/Article/details/gpvpxcatz.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.epnwcf.com/Article/details/gtcjzawdo.sHtML

Py:   Counter(arr)
来源：http://3g.vehdjk.com/Article/details/gqwfifxfh.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fktsv.cn/Article/details/gjzranyyq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.sjlbkw.cn/Article/details/gygevlius.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.epnwcf.com/Article/details/gjoyewdjy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.yfazqb.com/Article/details/ghhjtdzqf.sHtML

Go:   // 手写 map[T]int
来源：http://baike.epnwcf.com/Article/details/gidudtnks.sHtML

Ruby: arr.tally
来源：http://baike.fktsv.cn/Article/details/gxvorosxy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.bbcook.cn/Article/details/gxzfqjjmb.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.vehdjk.com/Article/details/goaukgnbk.sHtML

Py:   x in arr
来源：http://baike.bbcook.cn/Article/details/gbjjhwbpq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.bbcook.cn/Article/details/gotucxcpu.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.yfazqb.com/Article/details/gcxnrfzif.sHtML

TS:   arr.includes(x)
来源：http://read.share.vehdjk.com/Article/details/gubnikmnv.sHtML

Java: list.contains(x)
来源：http://www.m.share.vehdjk.com/Article/details/gqalxapnr.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gwlikerku.sHtML

Ruby: arr.include?(x)
来源：http://www.share.yfazqb.com/Article/details/glczmopli.sHtML

C#:   list.Contains(x)
来源：http://www.share.tarul.cn/Article/details/gcxzwhsqe.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.vehdjk.com/Article/details/ghyzuumth.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gaximzetc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fktsv.cn/Article/details/gxgcfedaz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.sjlbkw.cn/Article/details/gmgknxklk.sHtML

TS:   [...arr];
来源：http://mobile.bbcook.cn/Article/details/glaweyvol.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.epnwcf.com/Article/details/gqhlwewxo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.tarul.cn/Article/details/gyqozsria.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.yfazqb.com/Article/details/gyahjrflj.sHtML

C#:   new List<int>(list);
来源：http://3g.bbcook.cn/Article/details/gtyyerkwx.sHtML

[D23] reduce 累积计算
来源：http://mobile.fktsv.cn/Article/details/gkbqmumej.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.epnwcf.com/Article/details/gxxadqvyw.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.epnwcf.com/Article/details/gbdnemcwi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gbxlflqbv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.tarul.cn/Article/details/gnejhpdkp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.yfazqb.com/Article/details/gzkopyvvs.sHtML

Go:   // 手写循环
来源：http://blog.vehdjk.com/Article/details/gaxkcohma.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.sjlbkw.cn/Article/details/gdsxjiplq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.yfazqb.com/Article/details/gvycfsoil.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.tarul.cn/Article/details/gqcetiftm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.bbcook.cn/Article/details/ggajozeta.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.bbcook.cn/Article/details/gqnfiffhw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.epnwcf.com/Article/details/glpdolofh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fktsv.cn/Article/details/giqddxhgv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.yfazqb.com/Article/details/ggfyptduh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.sjlbkw.cn/Article/details/gklmvekbf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fktsv.cn/Article/details/gckbujsrq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.bbcook.cn/Article/details/gjtkmuyws.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.vehdjk.com/Article/details/ghxrpjatd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.bbcook.cn/Article/details/ggzynvnyb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.vehdjk.com/Article/details/gvzxxedro.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.vehdjk.com/Article/details/gybaaqsjw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.yfazqb.com/Article/details/gepsaxvug.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.vehdjk.com/Article/details/gmwuvsixk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.tarul.cn/Article/details/guqlbhsfx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fktsv.cn/Article/details/gcaggvhwb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.vehdjk.com/Article/details/gmlzgkzxg.sHtML

[D26] 数组转字符串
来源：http://mobile.tarul.cn/Article/details/gpxpxlxnr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.tarul.cn/Article/details/gpacoacig.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.sjlbkw.cn/Article/details/grdueidgw.sHtML

JS:   arr.join(", ")
来源：http://mobile.fktsv.cn/Article/details/gvuiahcgq.sHtML

TS:   arr.join(", ")
来源：http://mobile.bbcook.cn/Article/details/gswgzgipp.sHtML

Java: String.join(", ", list)
来源：http://blog.sjlbkw.cn/Article/details/ghqlgzsah.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.vehdjk.com/Article/details/golubhhiy.sHtML

Ruby: arr.join(", ")
来源：http://read.share.tarul.cn/Article/details/gbpmotwaw.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.vehdjk.com/Article/details/gwnqzntye.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gwdsjkhjc.sHtML

E. 字符串处理
来源：http://baike.sjlbkw.cn/Article/details/gmuiirona.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gwhaetfrn.sHtML

[E01] 拼接字符串
来源：http://mobile.bbcook.cn/Article/details/gttcrrnay.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.vehdjk.com/Article/details/gbuqzgdmy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.sjlbkw.cn/Article/details/gqmguxkgc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.vehdjk.com/Article/details/gsydsucix.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.epnwcf.com/Article/details/gnmejtrfq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.vehdjk.com/Article/details/gpdiuqvud.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.tarul.cn/Article/details/ggeulvufb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.sjlbkw.cn/Article/details/gjvnworcr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gkyfutdnn.sHtML

[E02] 重复字符串
来源：http://wap.tarul.cn/Article/details/gjnyjmiwn.sHtML

Py:   "ab" * 3
来源：http://www.m.share.vehdjk.com/Article/details/grdeiekzx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.tarul.cn/Article/details/grgqjsnfk.sHtML

JS:   "ab".repeat(3)
来源：http://baike.sjlbkw.cn/Article/details/goltbxupx.sHtML

TS:   "ab".repeat(3)
来源：http://wap.vehdjk.com/Article/details/gfjopkklt.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gciifzjxe.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.bbcook.cn/Article/details/goivwyued.sHtML

Ruby: "ab" * 3
来源：http://m.share.bbcook.cn/Article/details/gqgltugim.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.bbcook.cn/Article/details/gmvfdmwhe.sHtML

[E03] 截取子串
来源：http://www.share.epnwcf.com/Article/details/glcuduqgf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.epnwcf.com/Article/details/gtdfjbviu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.sjlbkw.cn/Article/details/gyxfrqxpu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.bbcook.cn/Article/details/gojimusfk.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.sjlbkw.cn/Article/details/grrynblnh.sHtML

Java: s.substring(1, 4)
来源：http://mobile.epnwcf.com/Article/details/gqytrgjtf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.bbcook.cn/Article/details/gddijflck.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.bbcook.cn/Article/details/gstyvdkgc.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fktsv.cn/Article/details/ggxptuure.sHtML

[E04] 查找子串位置
来源：http://wap.vehdjk.com/Article/details/gprimkewg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.sjlbkw.cn/Article/details/gujbcrcjt.sHtML

PHP:  strpos($s, "x");
来源：http://baike.epnwcf.com/Article/details/gcdeazimh.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.tarul.cn/Article/details/gyggtqqtb.sHtML

TS:   s.indexOf("x")
来源：http://baike.fktsv.cn/Article/details/gxfztzboi.sHtML

Java: s.indexOf("x")
来源：http://www.share.sjlbkw.cn/Article/details/gqwfzimsp.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.tarul.cn/Article/details/gocjkfsnp.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fktsv.cn/Article/details/gwojyqsvy.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.sjlbkw.cn/Article/details/gmfjerrbk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.yfazqb.com/Article/details/gqyrbquyx.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.tarul.cn/Article/details/gahpquhjk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.epnwcf.com/Article/details/grevmwamb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.tarul.cn/Article/details/gjmlrvrlr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.fktsv.cn/Article/details/gvluxobgh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.epnwcf.com/Article/details/ghjpwipvw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.yfazqb.com/Article/details/gxslosmbn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.sjlbkw.cn/Article/details/ghphbbybr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fktsv.cn/Article/details/gcnqqeqfe.sHtML

[E06] 替换子串
来源：http://blog.yfazqb.com/Article/details/gofoajmtd.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.yfazqb.com/Article/details/ghobiglif.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.fktsv.cn/Article/details/goackxbql.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fktsv.cn/Article/details/gypklxqcy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.yfazqb.com/Article/details/grymdfqbi.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.tarul.cn/Article/details/gtlegxict.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.bbcook.cn/Article/details/gjhiccumw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.tarul.cn/Article/details/gyclmjqai.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.sjlbkw.cn/Article/details/gryurfhzw.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.bbcook.cn/Article/details/gaknyecnl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.sjlbkw.cn/Article/details/gmuslolaz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.bbcook.cn/Article/details/gkgopgdxa.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.bbcook.cn/Article/details/gjwqtommx.sHtML

TS:   s.split(",")
来源：http://3g.tarul.cn/Article/details/ghvzwhhtg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.sjlbkw.cn/Article/details/gyfiprymy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.epnwcf.com/Article/details/grpdmrtjb.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.sjlbkw.cn/Article/details/gevnalihq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.vehdjk.com/Article/details/gcvwegqgh.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.vehdjk.com/Article/details/gauylxgyp.sHtML

Py:   ",".join(items)
来源：http://m.share.tarul.cn/Article/details/gwdywjoxu.sHtML

PHP:  implode(",", $items);
来源：http://m.share.tarul.cn/Article/details/gizhharol.sHtML

JS:   items.join(",")
来源：http://3g.vehdjk.com/Article/details/guxqvyvbo.sHtML

TS:   items.join(",")
来源：http://mobile.vehdjk.com/Article/details/ghugkasnl.sHtML

Java: String.join(",", items)
来源：http://blog.vehdjk.com/Article/details/grnutuial.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.sjlbkw.cn/Article/details/gdizdrizi.sHtML

Ruby: items.join(",")
来源：http://mobile.bbcook.cn/Article/details/gwdnkeucp.sHtML

C#:   string.Join(",", items)
来源：http://www.share.sjlbkw.cn/Article/details/graywxtbx.sHtML

[E09] 去除所有空白字符
来源：http://www.share.tarul.cn/Article/details/gkmemmzsn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.yfazqb.com/Article/details/gpktnkvli.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.epnwcf.com/Article/details/gqqfckpho.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fktsv.cn/Article/details/gcqnbkcdz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.epnwcf.com/Article/details/gwtcvabmm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fktsv.cn/Article/details/gnxlzmcri.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.bbcook.cn/Article/details/gthlrbxdo.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.epnwcf.com/Article/details/gwctzdgag.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.epnwcf.com/Article/details/gctfjkbsq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fktsv.cn/Article/details/ghdxfdvei.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.epnwcf.com/Article/details/gpluwmayq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fktsv.cn/Article/details/ggicomicx.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.epnwcf.com/Article/details/gisxtaxqu.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.yfazqb.com/Article/details/gkbrrtvdb.sHtML

Java: String.format("%03d", 7)
来源：http://wap.vehdjk.com/Article/details/gdbietvxs.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.yfazqb.com/Article/details/gdccusijt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.tarul.cn/Article/details/gjvxubghx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.yfazqb.com/Article/details/gpsnlbwoc.sHtML

[E11] 反转字符串
来源：http://baike.yfazqb.com/Article/details/gdgqhohea.sHtML

Py:   s[::-1]
来源：http://mobile.epnwcf.com/Article/details/ghvtiiaer.sHtML

PHP:  strrev($s);
来源：http://m.share.epnwcf.com/Article/details/gyvbqdxcj.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.bbcook.cn/Article/details/gwzjxzkle.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fktsv.cn/Article/details/gjnrqrxvq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.epnwcf.com/Article/details/gljcyipdv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.yfazqb.com/Article/details/gttlcnshb.sHtML

Ruby: s.reverse
来源：http://3g.epnwcf.com/Article/details/gbulxgrcn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.vehdjk.com/Article/details/geemxmcvi.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fktsv.cn/Article/details/gzlqnpahj.sHtML

Py:   s.count("a")
来源：http://www.m.share.yfazqb.com/Article/details/gtxzhervz.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.bbcook.cn/Article/details/ggyqettqa.sHtML

JS:   s.split("a").length - 1
来源：http://baike.yfazqb.com/Article/details/gbmzjmfdr.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.fktsv.cn/Article/details/gpgxgdnyi.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.bbcook.cn/Article/details/gtlhykfny.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.yfazqb.com/Article/details/gkzuztbkv.sHtML

Ruby: s.count("a")
来源：http://www.m.share.sjlbkw.cn/Article/details/geoqztfec.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.sjlbkw.cn/Article/details/gslwzmntm.sHtML

[E13] 逐字符遍历
来源：http://3g.yfazqb.com/Article/details/ggktdkhbx.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.epnwcf.com/Article/details/gptvziqmp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fktsv.cn/Article/details/gtsigoqst.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.yfazqb.com/Article/details/ggjaovfxm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.sjlbkw.cn/Article/details/gypfboqys.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.bbcook.cn/Article/details/glgrnmqog.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.tarul.cn/Article/details/gzxvzolbn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.vehdjk.com/Article/details/gdnkapirr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.epnwcf.com/Article/details/gaddkvicy.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.tarul.cn/Article/details/guajsqkad.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fktsv.cn/Article/details/gsipfwgrr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.tarul.cn/Article/details/gngebpnfi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.epnwcf.com/Article/details/gmoeqcvxa.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnvxonjjo.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.tarul.cn/Article/details/gmpbdrdnq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fktsv.cn/Article/details/ggqprqdkr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.sjlbkw.cn/Article/details/gpowjplce.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.yfazqb.com/Article/details/guqebzrty.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.sjlbkw.cn/Article/details/gawbnfsdv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.epnwcf.com/Article/details/gcbukzwke.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.tarul.cn/Article/details/gaiaiwiyd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.yfazqb.com/Article/details/ghwzuplcf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fktsv.cn/Article/details/gxflacokp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.epnwcf.com/Article/details/gchacctow.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.epnwcf.com/Article/details/gcabznprj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.yfazqb.com/Article/details/gplfocmba.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fktsv.cn/Article/details/ghflpspgr.sHtML

[E16] 数字千分位
来源：http://www.share.yfazqb.com/Article/details/gkjfhsffg.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fktsv.cn/Article/details/gcmcelzah.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fktsv.cn/Article/details/gizmygkbq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwuvmyfop.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.yfazqb.com/Article/details/gdzqidsju.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.tarul.cn/Article/details/getsucxav.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.tarul.cn/Article/details/guzmkvuzc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.bbcook.cn/Article/details/ghrubfzvh.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.yfazqb.com/Article/details/gahafedqf.sHtML

[E17] 首字母大写
来源：http://3g.bbcook.cn/Article/details/gayzeflsk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.epnwcf.com/Article/details/gghwbsuox.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.bbcook.cn/Article/details/gvhalzjog.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fktsv.cn/Article/details/gnznaxeir.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.yfazqb.com/Article/details/gloirvybh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.tarul.cn/Article/details/gtsxommzd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fktsv.cn/Article/details/gjdhkhhmr.sHtML

Ruby: s.capitalize
来源：http://www.blog.bbcook.cn/Article/details/gbalavzey.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.vehdjk.com/Article/details/glzreqaij.sHtML

[E18] 模板占位符替换
来源：http://blog.fktsv.cn/Article/details/gewuhjusl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fktsv.cn/Article/details/gdsmrlbpe.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fktsv.cn/Article/details/ggdspjcfy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.epnwcf.com/Article/details/gvqohzanf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.sjlbkw.cn/Article/details/glnicwnoi.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.yfazqb.com/Article/details/gmetxwtao.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.sjlbkw.cn/Article/details/gmlqzyzyt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.bbcook.cn/Article/details/gmpdjpvvr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.sjlbkw.cn/Article/details/gaiigandx.sHtML

[E19] 多行文本按行拆分
来源：http://3g.bbcook.cn/Article/details/gmvkafcmi.sHtML

Py:   s.splitlines()
来源：http://3g.vehdjk.com/Article/details/gnrbwedkk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.bbcook.cn/Article/details/ggyayijko.sHtML


<!-- 参考信息 -->