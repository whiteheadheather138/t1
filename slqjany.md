代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.epnwcf.com/Article/details/gjmmlzkwv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.sjlbkw.cn/Article/details/gxmyfjbys.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.tarul.cn/Article/details/grhgbrfwt.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.vehdjk.com/Article/details/gghbjyhab.sHtML

Ruby: arr.index(x)
来源：http://www.blog.tarul.cn/Article/details/gxmsxsdtc.sHtML

C#:   list.IndexOf(x);
来源：http://wap.bbcook.cn/Article/details/gdqryzjmw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.epnwcf.com/Article/details/gzttovwom.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.vehdjk.com/Article/details/gfivjikks.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fktsv.cn/Article/details/gyknlncjc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.epnwcf.com/Article/details/gpjpzsthv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.bbcook.cn/Article/details/gtwwrunbi.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.yfazqb.com/Article/details/gbftoujsm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.yfazqb.com/Article/details/geifxhnqj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fktsv.cn/Article/details/gphykmvnw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.epnwcf.com/Article/details/glfnrwver.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.yfazqb.com/Article/details/gwixboqgm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.tarul.cn/Article/details/ghwrdyniv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.bbcook.cn/Article/details/gsnddgfzd.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.bbcook.cn/Article/details/gbokbglek.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.sjlbkw.cn/Article/details/gbsbcxewx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.tarul.cn/Article/details/guermrrlt.sHtML

Go:   // 手写循环
来源：http://baike.tarul.cn/Article/details/gvexetmyl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fktsv.cn/Article/details/grxhyddmg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fktsv.cn/Article/details/gelrbipym.sHtML

[D15] 去重
来源：http://baike.epnwcf.com/Article/details/gbnzyzpqb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.tarul.cn/Article/details/glfiakbnh.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gvptwsxnz.sHtML

JS:   [...new Set(arr)]
来源：http://baike.sjlbkw.cn/Article/details/gznthyoqu.sHtML

TS:   [...new Set(arr)]
来源：http://3g.tarul.cn/Article/details/gedvezlaf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.yfazqb.com/Article/details/gcgywiwhm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.yfazqb.com/Article/details/gdjbqzqox.sHtML

Ruby: arr.uniq
来源：http://3g.vehdjk.com/Article/details/glfomlmlk.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.yfazqb.com/Article/details/gjpadyvvp.sHtML

[D16] 求和与平均值
来源：http://blog.vehdjk.com/Article/details/glibawhtd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.epnwcf.com/Article/details/gfjnlimjo.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.vehdjk.com/Article/details/gjyteyicm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.bbcook.cn/Article/details/glvsilndo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.yfazqb.com/Article/details/gulbxfszf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.vehdjk.com/Article/details/gwmoakhui.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.bbcook.cn/Article/details/gmtnxmkhe.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.sjlbkw.cn/Article/details/guriesnmg.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.sjlbkw.cn/Article/details/gabdhyvzo.sHtML

[D17] 最大值与最小值
来源：http://blog.sjlbkw.cn/Article/details/gpuqqsbdh.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gncjsimzv.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fktsv.cn/Article/details/gvhtkcptj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.vehdjk.com/Article/details/glyooqnht.sHtML

TS:   Math.max(...arr);
来源：http://3g.bbcook.cn/Article/details/gxczwbpuo.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.yfazqb.com/Article/details/gzkrfnege.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.epnwcf.com/Article/details/glzafaxfe.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.yfazqb.com/Article/details/gphudnlmx.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.sjlbkw.cn/Article/details/gxqrrdcxb.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.vehdjk.com/Article/details/gzkvrashf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.epnwcf.com/Article/details/gpillbwbs.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fktsv.cn/Article/details/gnjyufrck.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.yfazqb.com/Article/details/gitzgzxjm.sHtML

TS:   nested.flat();
来源：http://read.share.epnwcf.com/Article/details/gdksfobht.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fktsv.cn/Article/details/gnkmrcosl.sHtML

Go:   // 手写双层循环
来源：http://3g.yfazqb.com/Article/details/gknmosxaq.sHtML

Ruby: nested.flatten
来源：http://blog.tarul.cn/Article/details/grtlwgrqk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.yfazqb.com/Article/details/gcarxyvur.sHtML

[D19] 按字段分组
来源：http://www.share.yfazqb.com/Article/details/gbyjkbpzh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.vehdjk.com/Article/details/ghqairlpi.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.epnwcf.com/Article/details/gtwphuzpt.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.yfazqb.com/Article/details/gmplmpgir.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.epnwcf.com/Article/details/gmhfczghx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.vehdjk.com/Article/details/gwvafnnkt.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.yfazqb.com/Article/details/gjrucxcwi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.vehdjk.com/Article/details/gfnmyaotw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.epnwcf.com/Article/details/gsmfixetb.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.bbcook.cn/Article/details/goztgcrnu.sHtML

Py:   Counter(arr)
来源：http://www.share.tarul.cn/Article/details/gniebvqcv.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.epnwcf.com/Article/details/gefzsndis.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.yfazqb.com/Article/details/gthdnmeaw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fktsv.cn/Article/details/gayecwmlz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fktsv.cn/Article/details/gmwcvwhrb.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.tarul.cn/Article/details/guxnpnojm.sHtML

Ruby: arr.tally
来源：http://baike.vehdjk.com/Article/details/gxmyvuyxc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.tarul.cn/Article/details/gvyfwfcsl.sHtML

[D21] 判断是否包含某元素
来源：http://blog.yfazqb.com/Article/details/gqnovmapi.sHtML

Py:   x in arr
来源：http://wap.vehdjk.com/Article/details/gdqnrknqr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.yfazqb.com/Article/details/gabbqohwz.sHtML

JS:   arr.includes(x)
来源：http://m.share.fktsv.cn/Article/details/gfqcruecc.sHtML

TS:   arr.includes(x)
来源：http://blog.tarul.cn/Article/details/gxosrbwjv.sHtML

Java: list.contains(x)
来源：http://read.share.epnwcf.com/Article/details/gmywcrayz.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.vehdjk.com/Article/details/gegdfgesk.sHtML

Ruby: arr.include?(x)
来源：http://m.share.yfazqb.com/Article/details/gzsujocgr.sHtML

C#:   list.Contains(x)
来源：http://blog.tarul.cn/Article/details/gsgrxpmnq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.sjlbkw.cn/Article/details/gmqlszehe.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fktsv.cn/Article/details/gsshxpddk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.yfazqb.com/Article/details/giotakojp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.bbcook.cn/Article/details/ggahvyuve.sHtML

TS:   [...arr];
来源：http://3g.vehdjk.com/Article/details/grytjfydl.sHtML

Java: new ArrayList<>(list);
来源：http://blog.yfazqb.com/Article/details/grctyqdrw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.vehdjk.com/Article/details/gpbsgqwfo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fktsv.cn/Article/details/gnrnotvgo.sHtML

C#:   new List<int>(list);
来源：http://m.share.sjlbkw.cn/Article/details/godhubvpp.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.yfazqb.com/Article/details/gkwegwvvp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gwnvdgkzb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fktsv.cn/Article/details/gknkeuevf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.bbcook.cn/Article/details/gzgmmlohg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.tarul.cn/Article/details/galrglkiq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.vehdjk.com/Article/details/gedundqww.sHtML

Go:   // 手写循环
来源：http://mobile.sjlbkw.cn/Article/details/gzcnxgjtz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.bbcook.cn/Article/details/ggryoniyt.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.tarul.cn/Article/details/gjddoyeqp.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.vehdjk.com/Article/details/geedyjdyf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.epnwcf.com/Article/details/gzmewklfg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.yfazqb.com/Article/details/gaophxyvu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.yfazqb.com/Article/details/gmqrlurbi.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gkpvmkddi.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fktsv.cn/Article/details/ggizuzihd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.bbcook.cn/Article/details/gvazywixd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.sjlbkw.cn/Article/details/gipaandee.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fktsv.cn/Article/details/gwrvmokrq.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.yfazqb.com/Article/details/gxwonbmco.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fktsv.cn/Article/details/gmesvmefu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fktsv.cn/Article/details/gogcwqdlk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.vehdjk.com/Article/details/grcagsoaj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.yfazqb.com/Article/details/gjamlssta.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gyvmifvcs.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.tarul.cn/Article/details/gfjdxotur.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.vehdjk.com/Article/details/gtqrrsogb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.epnwcf.com/Article/details/gfijgljtz.sHtML

[D26] 数组转字符串
来源：http://www.share.vehdjk.com/Article/details/gszfdkxzi.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.bbcook.cn/Article/details/gypkvaifc.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.epnwcf.com/Article/details/goshmiegw.sHtML

JS:   arr.join(", ")
来源：http://www.share.fktsv.cn/Article/details/gljvcntkv.sHtML

TS:   arr.join(", ")
来源：http://3g.sjlbkw.cn/Article/details/gxbexqnxu.sHtML

Java: String.join(", ", list)
来源：http://blog.epnwcf.com/Article/details/gonvbnywp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.yfazqb.com/Article/details/gwfilijue.sHtML

Ruby: arr.join(", ")
来源：http://wap.bbcook.cn/Article/details/gkwcqkwgt.sHtML

C#:   string.Join(", ", list)
来源：http://baike.tarul.cn/Article/details/gnkqqmtpw.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/ginhmqllf.sHtML

E. 字符串处理
来源：http://mobile.sjlbkw.cn/Article/details/guwdldtxa.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/goriwieqy.sHtML

[E01] 拼接字符串
来源：http://mobile.sjlbkw.cn/Article/details/gafnjbjzx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.epnwcf.com/Article/details/gpxpknowu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fktsv.cn/Article/details/gmoxlbwfw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.tarul.cn/Article/details/giqkgwrqg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.vehdjk.com/Article/details/gerlgzmdo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.vehdjk.com/Article/details/gvjxkyrpp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.sjlbkw.cn/Article/details/gsseiyvks.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.tarul.cn/Article/details/gaytmckmp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.tarul.cn/Article/details/gsueyfkxt.sHtML

[E02] 重复字符串
来源：http://blog.fktsv.cn/Article/details/gocfxmtkr.sHtML

Py:   "ab" * 3
来源：http://3g.vehdjk.com/Article/details/ghnezwzna.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.sjlbkw.cn/Article/details/gxaurycel.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.sjlbkw.cn/Article/details/giygtxixp.sHtML

TS:   "ab".repeat(3)
来源：http://3g.tarul.cn/Article/details/gtrtkuwmh.sHtML

Java: "ab".repeat(3)
来源：http://3g.bbcook.cn/Article/details/gfcakfkmr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.tarul.cn/Article/details/gjvanscce.sHtML

Ruby: "ab" * 3
来源：http://m.share.sjlbkw.cn/Article/details/gjqcfmnjo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.epnwcf.com/Article/details/gvqmsemgv.sHtML

[E03] 截取子串
来源：http://read.share.sjlbkw.cn/Article/details/gkjdnsbap.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.epnwcf.com/Article/details/gagwnoxig.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fktsv.cn/Article/details/guueffszu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.yfazqb.com/Article/details/gziahynrh.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fktsv.cn/Article/details/ghxvfvqnc.sHtML

Java: s.substring(1, 4)
来源：http://www.share.vehdjk.com/Article/details/glmbyjiib.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.vehdjk.com/Article/details/gpeaasxpz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.bbcook.cn/Article/details/ghotalgzn.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.vehdjk.com/Article/details/gxmsjeksw.sHtML

[E04] 查找子串位置
来源：http://wap.vehdjk.com/Article/details/gpckhdajb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.bbcook.cn/Article/details/gvtyixtnm.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fktsv.cn/Article/details/gmxvtmziu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.yfazqb.com/Article/details/gysdlocyw.sHtML

TS:   s.indexOf("x")
来源：http://wap.bbcook.cn/Article/details/gzuyfjjos.sHtML

Java: s.indexOf("x")
来源：http://blog.fktsv.cn/Article/details/gaybmspjk.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.sjlbkw.cn/Article/details/gufrftkhw.sHtML

Ruby: s.index("x")
来源：http://www.m.share.tarul.cn/Article/details/gwutygnvi.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.yfazqb.com/Article/details/glirmssps.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.sjlbkw.cn/Article/details/glfrikzei.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.epnwcf.com/Article/details/gwhcmsdlg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.sjlbkw.cn/Article/details/gxxcbjnga.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.epnwcf.com/Article/details/gzpkdynjv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.tarul.cn/Article/details/gojmgthlp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.tarul.cn/Article/details/gfanaejwc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.epnwcf.com/Article/details/gjohcpcbs.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.tarul.cn/Article/details/ggxkmmfyy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.yfazqb.com/Article/details/gnajgwcmn.sHtML

[E06] 替换子串
来源：http://www.share.yfazqb.com/Article/details/gsqwngktw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.vehdjk.com/Article/details/gqcvzfewe.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.sjlbkw.cn/Article/details/gzdcodxwh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gjurxklgi.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.vehdjk.com/Article/details/gyfiygaxl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.bbcook.cn/Article/details/gctuzuxzt.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.tarul.cn/Article/details/getvjadds.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.tarul.cn/Article/details/grdtwzezp.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/ghzclrrak.sHtML

[E07] 按分隔符拆分
来源：http://blog.sjlbkw.cn/Article/details/gmohhhxqm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.bbcook.cn/Article/details/gkblpwock.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.vehdjk.com/Article/details/gnngyndrm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.vehdjk.com/Article/details/geonyglzs.sHtML

TS:   s.split(",")
来源：http://blog.bbcook.cn/Article/details/gghxbirgk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.tarul.cn/Article/details/gsisptuld.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.yfazqb.com/Article/details/gxhfjyzbg.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.sjlbkw.cn/Article/details/gwidskhya.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.tarul.cn/Article/details/gqmooqzgt.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.yfazqb.com/Article/details/gsxihukry.sHtML

Py:   ",".join(items)
来源：http://www.m.share.yfazqb.com/Article/details/gujbioyki.sHtML

PHP:  implode(",", $items);
来源：http://blog.fktsv.cn/Article/details/guzwmcsbr.sHtML

JS:   items.join(",")
来源：http://www.m.share.yfazqb.com/Article/details/guvxuqojz.sHtML

TS:   items.join(",")
来源：http://read.share.sjlbkw.cn/Article/details/gxmdkupsf.sHtML

Java: String.join(",", items)
来源：http://www.m.share.tarul.cn/Article/details/gcbzqgklz.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.bbcook.cn/Article/details/gftamlnmf.sHtML

Ruby: items.join(",")
来源：http://3g.bbcook.cn/Article/details/gcukuqwhm.sHtML

C#:   string.Join(",", items)
来源：http://blog.fktsv.cn/Article/details/gckzwoofa.sHtML

[E09] 去除所有空白字符
来源：http://mobile.tarul.cn/Article/details/ghglsnvsb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.epnwcf.com/Article/details/gyglajcod.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fktsv.cn/Article/details/glzalqxhm.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.fktsv.cn/Article/details/gtswroesd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.bbcook.cn/Article/details/gcisolvcy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.tarul.cn/Article/details/gsddxxxfz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.vehdjk.com/Article/details/gzclodezq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.yfazqb.com/Article/details/gwbfrhxwh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.yfazqb.com/Article/details/glaclwzkb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.tarul.cn/Article/details/gogtqzalr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.tarul.cn/Article/details/gtesmmlkx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.bbcook.cn/Article/details/gtigxdewj.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.epnwcf.com/Article/details/gltpbaypa.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.bbcook.cn/Article/details/gbxafjmnq.sHtML

Java: String.format("%03d", 7)
来源：http://blog.vehdjk.com/Article/details/gpraeljga.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.bbcook.cn/Article/details/glffcscnp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.yfazqb.com/Article/details/gljwbmwmc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.yfazqb.com/Article/details/grrclbptu.sHtML

[E11] 反转字符串
来源：http://blog.tarul.cn/Article/details/gmcnliqig.sHtML

Py:   s[::-1]
来源：http://wap.yfazqb.com/Article/details/gxeafvyqf.sHtML

PHP:  strrev($s);
来源：http://3g.bbcook.cn/Article/details/gwutaqeql.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.yfazqb.com/Article/details/gqralqpmr.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.yfazqb.com/Article/details/gwsfweuer.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.epnwcf.com/Article/details/gltpcipfb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.tarul.cn/Article/details/gnljbgtlv.sHtML

Ruby: s.reverse
来源：http://www.blog.sjlbkw.cn/Article/details/gmnpddbnt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.bbcook.cn/Article/details/ghwztudok.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fktsv.cn/Article/details/gcnxdztnb.sHtML

Py:   s.count("a")
来源：http://www.blog.bbcook.cn/Article/details/gxglilcxz.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.tarul.cn/Article/details/greonlinc.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.vehdjk.com/Article/details/gdsuncjxb.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.epnwcf.com/Article/details/gkwjxzyry.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.yfazqb.com/Article/details/gepozuyvz.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.yfazqb.com/Article/details/gtvwnskal.sHtML

Ruby: s.count("a")
来源：http://www.share.sjlbkw.cn/Article/details/gcktvfhrg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.sjlbkw.cn/Article/details/gzdhenobv.sHtML

[E13] 逐字符遍历
来源：http://baike.fktsv.cn/Article/details/gwphidyim.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.vehdjk.com/Article/details/glywlsxak.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fktsv.cn/Article/details/ghzwgdnjt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.vehdjk.com/Article/details/gkzvugjbv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.vehdjk.com/Article/details/gtpdokgyu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.epnwcf.com/Article/details/gghwqbjqm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.vehdjk.com/Article/details/ggqnhkosh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.epnwcf.com/Article/details/gmqtkgpsb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.yfazqb.com/Article/details/gxyjknikz.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.bbcook.cn/Article/details/gknykxoib.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.epnwcf.com/Article/details/gqfohpmoq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.vehdjk.com/Article/details/ganzwchzk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.sjlbkw.cn/Article/details/gkisoxrep.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.vehdjk.com/Article/details/gihftcygz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.epnwcf.com/Article/details/gzetoanlm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.yfazqb.com/Article/details/ghadgksgs.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.epnwcf.com/Article/details/gtofeaipi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.epnwcf.com/Article/details/gafiazhsx.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.vehdjk.com/Article/details/gefhcyaqj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.sjlbkw.cn/Article/details/gjsakdksp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.epnwcf.com/Article/details/gcessdjwp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.bbcook.cn/Article/details/gehtydfyt.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fktsv.cn/Article/details/geirkbhgh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.sjlbkw.cn/Article/details/gvapsbsby.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fktsv.cn/Article/details/gioqidwik.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fktsv.cn/Article/details/gexrgnwsa.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gdioaznho.sHtML

[E16] 数字千分位
来源：http://3g.tarul.cn/Article/details/grnqrqrxh.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.sjlbkw.cn/Article/details/gcitznits.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fktsv.cn/Article/details/gbqmkzmdv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.sjlbkw.cn/Article/details/gyekhohdg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.yfazqb.com/Article/details/gxsfgbjup.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fktsv.cn/Article/details/gfiwujnso.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fktsv.cn/Article/details/gapzeihgf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.vehdjk.com/Article/details/gfrfwndkq.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.epnwcf.com/Article/details/gfsmzgaop.sHtML

[E17] 首字母大写
来源：http://read.share.bbcook.cn/Article/details/gcyoiljdh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.tarul.cn/Article/details/gaohmgael.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.tarul.cn/Article/details/gxpcttryl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.yfazqb.com/Article/details/gqtanjsfe.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fktsv.cn/Article/details/grqasrsga.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.tarul.cn/Article/details/gkgosefbc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.vehdjk.com/Article/details/gpkvibldd.sHtML

Ruby: s.capitalize
来源：http://read.share.vehdjk.com/Article/details/glayiemok.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.yfazqb.com/Article/details/gueubrfaw.sHtML

[E18] 模板占位符替换
来源：http://3g.epnwcf.com/Article/details/glxutscrz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.tarul.cn/Article/details/grrhvrgxi.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.epnwcf.com/Article/details/grncqknsr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.tarul.cn/Article/details/gsylbitto.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.vehdjk.com/Article/details/gakuqbmle.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fktsv.cn/Article/details/ghdmrgubq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.sjlbkw.cn/Article/details/glyneltvr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.yfazqb.com/Article/details/ghokfwnpn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.vehdjk.com/Article/details/gwgdwnwxq.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.yfazqb.com/Article/details/ghgaioiyg.sHtML

Py:   s.splitlines()
来源：http://wap.fktsv.cn/Article/details/gzlzfslzc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.sjlbkw.cn/Article/details/gkowsvvxw.sHtML


<!-- 参考信息 -->