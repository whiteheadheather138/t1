代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fktsv.cn/Article/details/gwevdlyvk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.bbcook.cn/Article/details/gohlqxqly.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fktsv.cn/Article/details/gyqsxygbw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.bbcook.cn/Article/details/gmdbwnvyd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.epnwcf.com/Article/details/gxuyomeei.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fktsv.cn/Article/details/gbfuumojm.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.sjlbkw.cn/Article/details/gxfjnxboz.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.bbcook.cn/Article/details/gnivzbgth.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.epnwcf.com/Article/details/gasahogwe.sHtML

Go:   // 手写循环
来源：http://read.share.bbcook.cn/Article/details/gdqgiagzh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.epnwcf.com/Article/details/gfxdogpca.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.yfazqb.com/Article/details/ggfvyslxe.sHtML

[D15] 去重
来源：http://www.blog.fktsv.cn/Article/details/gcynkfbws.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fktsv.cn/Article/details/gqsfthgpc.sHtML

PHP:  array_unique($arr);
来源：http://m.share.vehdjk.com/Article/details/gsviugckm.sHtML

JS:   [...new Set(arr)]
来源：http://baike.bbcook.cn/Article/details/gdilrhpvy.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.vehdjk.com/Article/details/gnwhrfgvd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fktsv.cn/Article/details/gkxhwpsba.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.vehdjk.com/Article/details/ggsrqhxsu.sHtML

Ruby: arr.uniq
来源：http://www.share.vehdjk.com/Article/details/gbadiovlb.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.tarul.cn/Article/details/gkrvsrmip.sHtML

[D16] 求和与平均值
来源：http://www.share.sjlbkw.cn/Article/details/gyczyxdtr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fktsv.cn/Article/details/guvfwzvoy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.vehdjk.com/Article/details/gkkargild.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.yfazqb.com/Article/details/guooqqyxi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.sjlbkw.cn/Article/details/ggodssftw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.sjlbkw.cn/Article/details/ggtfkesll.sHtML

Go:   // 手写循环累加
来源：http://www.share.bbcook.cn/Article/details/gqxqderis.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.epnwcf.com/Article/details/gtyqgynkc.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.tarul.cn/Article/details/gvzfwkrtd.sHtML

[D17] 最大值与最小值
来源：http://read.share.fktsv.cn/Article/details/gadiuxxgu.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.sjlbkw.cn/Article/details/gigenemog.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.yfazqb.com/Article/details/gbvvvyuar.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.yfazqb.com/Article/details/gkxbefxak.sHtML

TS:   Math.max(...arr);
来源：http://blog.vehdjk.com/Article/details/ggliaeiko.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.bbcook.cn/Article/details/gbujwebqt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.epnwcf.com/Article/details/gnzudnsgn.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.yfazqb.com/Article/details/gxbpqgozh.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.tarul.cn/Article/details/ghquxnlsm.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.yfazqb.com/Article/details/gztepbfgw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.bbcook.cn/Article/details/gzvrvbgrl.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.bbcook.cn/Article/details/geiiohykk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.bbcook.cn/Article/details/gevgherrn.sHtML

TS:   nested.flat();
来源：http://www.share.yfazqb.com/Article/details/glmmonpue.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.tarul.cn/Article/details/gbqlsqhse.sHtML

Go:   // 手写双层循环
来源：http://read.share.sjlbkw.cn/Article/details/gaeubycyo.sHtML

Ruby: nested.flatten
来源：http://www.m.share.bbcook.cn/Article/details/gwpjtwxyx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fktsv.cn/Article/details/ghlhjcvxa.sHtML

[D19] 按字段分组
来源：http://read.share.bbcook.cn/Article/details/gifjqzvtz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.tarul.cn/Article/details/giuxrvzfe.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.epnwcf.com/Article/details/gtmspqayb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.bbcook.cn/Article/details/gejfxcsgf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.epnwcf.com/Article/details/gnqoqftfk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.epnwcf.com/Article/details/gskcwixnt.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fktsv.cn/Article/details/gxpaltmga.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fktsv.cn/Article/details/gkrsfeaes.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.tarul.cn/Article/details/gaxqgfsna.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.tarul.cn/Article/details/guowxtxyi.sHtML

Py:   Counter(arr)
来源：http://read.share.yfazqb.com/Article/details/gutbousos.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.epnwcf.com/Article/details/gctnrlzbw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.epnwcf.com/Article/details/ghrmfgjjc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.yfazqb.com/Article/details/gybclwppr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.epnwcf.com/Article/details/gvkeblese.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fktsv.cn/Article/details/gmnmmbjcu.sHtML

Ruby: arr.tally
来源：http://www.share.yfazqb.com/Article/details/goojnfxsa.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.bbcook.cn/Article/details/ggjhrxcgx.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.vehdjk.com/Article/details/gpeoyayxb.sHtML

Py:   x in arr
来源：http://3g.tarul.cn/Article/details/gtqkptsga.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.bbcook.cn/Article/details/gqzehpznq.sHtML

JS:   arr.includes(x)
来源：http://read.share.bbcook.cn/Article/details/grmujskym.sHtML

TS:   arr.includes(x)
来源：http://mobile.fktsv.cn/Article/details/glatnojhg.sHtML

Java: list.contains(x)
来源：http://mobile.tarul.cn/Article/details/gwtsmdspe.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gsxfogpjo.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.vehdjk.com/Article/details/goycdfhvh.sHtML

C#:   list.Contains(x)
来源：http://baike.fktsv.cn/Article/details/gbmddjarc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fktsv.cn/Article/details/gznoimkjs.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fktsv.cn/Article/details/grcgpfayp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fktsv.cn/Article/details/ggfqdkdqt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fktsv.cn/Article/details/gnrbvspmw.sHtML

TS:   [...arr];
来源：http://www.blog.yfazqb.com/Article/details/gsrszvddv.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.yfazqb.com/Article/details/goowhlpbg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.vehdjk.com/Article/details/gqneefclx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.sjlbkw.cn/Article/details/gfbqsygvd.sHtML

C#:   new List<int>(list);
来源：http://wap.tarul.cn/Article/details/gcxqjaziu.sHtML

[D23] reduce 累积计算
来源：http://read.share.tarul.cn/Article/details/gfggpwdpq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.bbcook.cn/Article/details/gbvyjjrmd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.sjlbkw.cn/Article/details/ggekdaxux.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.yfazqb.com/Article/details/gjbmhinqg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.bbcook.cn/Article/details/geknwcfoh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.vehdjk.com/Article/details/giddpferd.sHtML

Go:   // 手写循环
来源：http://read.share.epnwcf.com/Article/details/gehcwxfft.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.epnwcf.com/Article/details/gusikmqjq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.tarul.cn/Article/details/gsxjrmtuu.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.sjlbkw.cn/Article/details/gmnetsuvo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.vehdjk.com/Article/details/gamjbrjwh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.sjlbkw.cn/Article/details/gxdqplbfj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.vehdjk.com/Article/details/gbqmwkzop.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.tarul.cn/Article/details/ghzvdozfc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fktsv.cn/Article/details/gsttadyrs.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.sjlbkw.cn/Article/details/gugzhplzl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.yfazqb.com/Article/details/gxwqyhrei.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.tarul.cn/Article/details/grkjrfwbh.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.tarul.cn/Article/details/gluxxoqoe.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.epnwcf.com/Article/details/guigmyurv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.fktsv.cn/Article/details/gmyuskofu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.epnwcf.com/Article/details/gklllhuyp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.bbcook.cn/Article/details/gzbqseidw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.sjlbkw.cn/Article/details/gzeiiqzgd.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.yfazqb.com/Article/details/gnasmxkxk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.tarul.cn/Article/details/gtixnlhug.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fktsv.cn/Article/details/grplhknul.sHtML

[D26] 数组转字符串
来源：http://m.share.fktsv.cn/Article/details/gsovcavss.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.bbcook.cn/Article/details/gerrarcea.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.tarul.cn/Article/details/grfjegdtp.sHtML

JS:   arr.join(", ")
来源：http://www.blog.yfazqb.com/Article/details/gitdiglhj.sHtML

TS:   arr.join(", ")
来源：http://m.share.epnwcf.com/Article/details/gkkizicug.sHtML

Java: String.join(", ", list)
来源：http://mobile.tarul.cn/Article/details/gfcenrctq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.vehdjk.com/Article/details/gheudcrbz.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.sjlbkw.cn/Article/details/gohalinxm.sHtML

C#:   string.Join(", ", list)
来源：http://blog.tarul.cn/Article/details/gkicsznks.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gsxnbebwi.sHtML

E. 字符串处理
来源：http://baike.yfazqb.com/Article/details/gbxltyvnz.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gppehrjer.sHtML

[E01] 拼接字符串
来源：http://blog.tarul.cn/Article/details/goqgqljhv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.tarul.cn/Article/details/gknwmwmmx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.epnwcf.com/Article/details/gfzncrdrt.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.epnwcf.com/Article/details/gtoxstwlr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.yfazqb.com/Article/details/gqzrdtwsc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.yfazqb.com/Article/details/gpxwbodzm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.vehdjk.com/Article/details/glqkvnybq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.bbcook.cn/Article/details/ggsrvfftb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.vehdjk.com/Article/details/gipwjvyro.sHtML

[E02] 重复字符串
来源：http://www.share.fktsv.cn/Article/details/gfyglaanj.sHtML

Py:   "ab" * 3
来源：http://www.share.fktsv.cn/Article/details/gwnkcjsgf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.bbcook.cn/Article/details/gazzqshmf.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.tarul.cn/Article/details/gtuebbqqg.sHtML

TS:   "ab".repeat(3)
来源：http://blog.yfazqb.com/Article/details/gpjbkqvqo.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fktsv.cn/Article/details/ghdzrncwo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fktsv.cn/Article/details/ggtbnlpjf.sHtML

Ruby: "ab" * 3
来源：http://blog.bbcook.cn/Article/details/gmncsgzja.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.epnwcf.com/Article/details/gxyhbqbyo.sHtML

[E03] 截取子串
来源：http://3g.fktsv.cn/Article/details/gjfpnckmm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fktsv.cn/Article/details/gwoxifkhd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/gpcccjtrj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.vehdjk.com/Article/details/gvhhvrkdp.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.epnwcf.com/Article/details/gmojvtexc.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.bbcook.cn/Article/details/glnubneye.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fktsv.cn/Article/details/gkcreqiax.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.epnwcf.com/Article/details/geitouylv.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.epnwcf.com/Article/details/gyqavhowk.sHtML

[E04] 查找子串位置
来源：http://www.share.fktsv.cn/Article/details/gncxyhgly.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.epnwcf.com/Article/details/gwxtuxzsg.sHtML

PHP:  strpos($s, "x");
来源：http://blog.tarul.cn/Article/details/gzmdnomqa.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.vehdjk.com/Article/details/gscgqzxyl.sHtML

TS:   s.indexOf("x")
来源：http://www.share.epnwcf.com/Article/details/ghbfzzmjx.sHtML

Java: s.indexOf("x")
来源：http://blog.tarul.cn/Article/details/gcoaocaht.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fktsv.cn/Article/details/gzvghjbow.sHtML

Ruby: s.index("x")
来源：http://www.share.fktsv.cn/Article/details/gwgfweyal.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.tarul.cn/Article/details/gkenlromb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.sjlbkw.cn/Article/details/gsvsaiwib.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.yfazqb.com/Article/details/gfoiprhjf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.tarul.cn/Article/details/gvyeqcetd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.bbcook.cn/Article/details/gvniygmsv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.epnwcf.com/Article/details/gtidytcnl.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.epnwcf.com/Article/details/gmsllgcjz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fktsv.cn/Article/details/gtmnpvrmx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.vehdjk.com/Article/details/gmlxnixow.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fktsv.cn/Article/details/gmfchtaqk.sHtML

[E06] 替换子串
来源：http://blog.vehdjk.com/Article/details/glqbqnbci.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.tarul.cn/Article/details/gklwhplbg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.yfazqb.com/Article/details/ghubhgxos.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gbismkcgm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.tarul.cn/Article/details/gimrqrkij.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.tarul.cn/Article/details/gdgdqdief.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.bbcook.cn/Article/details/givlkbmzw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.bbcook.cn/Article/details/gizpeudah.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.yfazqb.com/Article/details/gkkdhkame.sHtML

[E07] 按分隔符拆分
来源：http://m.share.epnwcf.com/Article/details/ggoeapgim.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.sjlbkw.cn/Article/details/gvfvcnxqi.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.vehdjk.com/Article/details/gzaobdlgq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.tarul.cn/Article/details/ghwbylapr.sHtML

TS:   s.split(",")
来源：http://blog.fktsv.cn/Article/details/glebmyrdd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fktsv.cn/Article/details/gdjyvieiu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.epnwcf.com/Article/details/gtiljdfcl.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fktsv.cn/Article/details/gwkmokpcd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.tarul.cn/Article/details/gyeibwzty.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.tarul.cn/Article/details/gohpazdmv.sHtML

Py:   ",".join(items)
来源：http://m.share.sjlbkw.cn/Article/details/grzyafwhq.sHtML

PHP:  implode(",", $items);
来源：http://m.share.yfazqb.com/Article/details/gohwcsprn.sHtML

JS:   items.join(",")
来源：http://read.share.bbcook.cn/Article/details/gexfmayyo.sHtML

TS:   items.join(",")
来源：http://www.blog.epnwcf.com/Article/details/gcflqpvvs.sHtML

Java: String.join(",", items)
来源：http://www.blog.yfazqb.com/Article/details/gplkmhubu.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.yfazqb.com/Article/details/gchqpdsqa.sHtML

Ruby: items.join(",")
来源：http://mobile.yfazqb.com/Article/details/gowybsryr.sHtML

C#:   string.Join(",", items)
来源：http://m.share.epnwcf.com/Article/details/gjukfsiik.sHtML

[E09] 去除所有空白字符
来源：http://baike.fktsv.cn/Article/details/gbihjckqy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.epnwcf.com/Article/details/grlyllkzq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.tarul.cn/Article/details/gjryzzmft.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.tarul.cn/Article/details/gdkhbduzs.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.yfazqb.com/Article/details/ghtggyidq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.bbcook.cn/Article/details/gvevxgldb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.vehdjk.com/Article/details/gllgipfiw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.bbcook.cn/Article/details/gvcmljuba.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.yfazqb.com/Article/details/gsblxchyc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.tarul.cn/Article/details/glyjjtqdm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.tarul.cn/Article/details/gmzoiewsu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.sjlbkw.cn/Article/details/gpypimaui.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.vehdjk.com/Article/details/gnnqsspou.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.tarul.cn/Article/details/gvmtcqceg.sHtML

Java: String.format("%03d", 7)
来源：http://baike.yfazqb.com/Article/details/gedbeschd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.sjlbkw.cn/Article/details/guaunpcbh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.sjlbkw.cn/Article/details/gqbryjnyv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.epnwcf.com/Article/details/gvdzxqqsy.sHtML

[E11] 反转字符串
来源：http://blog.epnwcf.com/Article/details/gwxvcdizt.sHtML

Py:   s[::-1]
来源：http://baike.yfazqb.com/Article/details/gyabaejeg.sHtML

PHP:  strrev($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/glrhkvlog.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.sjlbkw.cn/Article/details/gvuynkieq.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.epnwcf.com/Article/details/gkoajcnhl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.tarul.cn/Article/details/gceedgqmn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.bbcook.cn/Article/details/gsvrnfwvu.sHtML

Ruby: s.reverse
来源：http://m.share.sjlbkw.cn/Article/details/gapwqrkyn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.sjlbkw.cn/Article/details/gbjwpkktm.sHtML

[E12] 统计某字符出现次数
来源：http://baike.sjlbkw.cn/Article/details/gobmpiigw.sHtML

Py:   s.count("a")
来源：http://baike.fktsv.cn/Article/details/gwxwetmns.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.sjlbkw.cn/Article/details/gnvswhngp.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.bbcook.cn/Article/details/ggcsvpmul.sHtML

TS:   s.split("a").length - 1
来源：http://wap.epnwcf.com/Article/details/gwoyfggyg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.yfazqb.com/Article/details/gtzemnpgt.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.vehdjk.com/Article/details/gaaqgmqiz.sHtML

Ruby: s.count("a")
来源：http://3g.yfazqb.com/Article/details/gsdztxazh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.sjlbkw.cn/Article/details/gpzwfexsb.sHtML

[E13] 逐字符遍历
来源：http://blog.fktsv.cn/Article/details/giwptzyfw.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.tarul.cn/Article/details/ggrqmlsni.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.bbcook.cn/Article/details/gdgozwngg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.epnwcf.com/Article/details/gfpjaadwh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/gdoqqknqo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fktsv.cn/Article/details/gkwfrzphq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.sjlbkw.cn/Article/details/gaqlolvff.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.vehdjk.com/Article/details/gnmlacbpp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.bbcook.cn/Article/details/gtaujhxhs.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.tarul.cn/Article/details/gsizguvok.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.epnwcf.com/Article/details/gdhzbomgw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.tarul.cn/Article/details/gjiilmtdp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.bbcook.cn/Article/details/ghgzsmcxy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.epnwcf.com/Article/details/gxwficmsx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.vehdjk.com/Article/details/gesnnvcai.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.sjlbkw.cn/Article/details/goawkhwfk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.bbcook.cn/Article/details/ghxghxffh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.sjlbkw.cn/Article/details/gioavucot.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.sjlbkw.cn/Article/details/gvfvpuigx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.bbcook.cn/Article/details/gzkglbvcy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gihesajfk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.sjlbkw.cn/Article/details/gtmhvepxa.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.epnwcf.com/Article/details/gnqdbhfrf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.vehdjk.com/Article/details/gdjmqpgfz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.tarul.cn/Article/details/gwhipcxid.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.vehdjk.com/Article/details/gkozrkzez.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.tarul.cn/Article/details/gqjvmdejl.sHtML

[E16] 数字千分位
来源：http://3g.sjlbkw.cn/Article/details/gfzgixavf.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.yfazqb.com/Article/details/gsojmsvsj.sHtML

PHP:  number_format(1234567);
来源：http://blog.sjlbkw.cn/Article/details/gifqckvyu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.vehdjk.com/Article/details/gmytjovcq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fktsv.cn/Article/details/gwtkpueif.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.sjlbkw.cn/Article/details/geawlnkwp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.vehdjk.com/Article/details/gfpkclxcf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fktsv.cn/Article/details/grevkptpa.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.vehdjk.com/Article/details/guytugmwb.sHtML

[E17] 首字母大写
来源：http://www.share.fktsv.cn/Article/details/gjytryobc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.yfazqb.com/Article/details/gcmxnadqq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fktsv.cn/Article/details/gabqndena.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.sjlbkw.cn/Article/details/gpjsfhdqj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.bbcook.cn/Article/details/gtzhftdqc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.sjlbkw.cn/Article/details/grytoekdj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.sjlbkw.cn/Article/details/gmbfjfzze.sHtML

Ruby: s.capitalize
来源：http://baike.epnwcf.com/Article/details/giwhiwqcd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fktsv.cn/Article/details/grxxcqwaa.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gupkfavzj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.sjlbkw.cn/Article/details/gfrxhdwcp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.yfazqb.com/Article/details/gqdmbkibx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.tarul.cn/Article/details/gukjibjqj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.epnwcf.com/Article/details/gwoiodesc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.yfazqb.com/Article/details/gzpjlugqx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.epnwcf.com/Article/details/gylyszekw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.yfazqb.com/Article/details/gbzsradbp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.yfazqb.com/Article/details/gadjbkntz.sHtML

[E19] 多行文本按行拆分
来源：http://blog.vehdjk.com/Article/details/gohhkjrhg.sHtML

Py:   s.splitlines()
来源：http://www.blog.vehdjk.com/Article/details/gelerrnoz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.tarul.cn/Article/details/gpkupthyh.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.tarul.cn/Article/details/gqoruoktf.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.yfazqb.com/Article/details/ghpoxedtg.sHtML

Java: s.lines().toList()
来源：http://www.m.share.bbcook.cn/Article/details/gfqrmdjap.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.vehdjk.com/Article/details/gabezrckg.sHtML

Ruby: s.lines
来源：http://3g.tarul.cn/Article/details/gvogddunz.sHtML

C#:   s.Split('\n')
来源：http://blog.vehdjk.com/Article/details/gkwwnhaqo.sHtML

[E20] 判断字符串是否为空
来源：http://wap.epnwcf.com/Article/details/gxcutgyih.sHtML

Py:   if not s:
来源：http://read.share.yfazqb.com/Article/details/getzymewp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.yfazqb.com/Article/details/gqiskyorr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.yfazqb.com/Article/details/gzladzxwe.sHtML

TS:   if (s === "") {}
来源：http://www.share.bbcook.cn/Article/details/grfjiibmn.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fktsv.cn/Article/details/gozqgjgbt.sHtML


<!-- 参考信息 -->