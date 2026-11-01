代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.bbcook.cn/Article/details/gkotrpyzd.sHtML

Go:   // 手写循环
来源：http://baike.bbcook.cn/Article/details/getuqbbty.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fktsv.cn/Article/details/guyodgksf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.vehdjk.com/Article/details/gjsndjzad.sHtML

[D15] 去重
来源：http://wap.sjlbkw.cn/Article/details/gjiwxceky.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.yfazqb.com/Article/details/ggwoqnvaa.sHtML

PHP:  array_unique($arr);
来源：http://3g.tarul.cn/Article/details/gzbhyzcpo.sHtML

JS:   [...new Set(arr)]
来源：http://wap.bbcook.cn/Article/details/gzmrcivvi.sHtML

TS:   [...new Set(arr)]
来源：http://3g.tarul.cn/Article/details/gmpvxpzct.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.tarul.cn/Article/details/gktgsvixr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fktsv.cn/Article/details/gfnxrzbql.sHtML

Ruby: arr.uniq
来源：http://read.share.sjlbkw.cn/Article/details/ggqgqjkob.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.tarul.cn/Article/details/gkmfozawp.sHtML

[D16] 求和与平均值
来源：http://3g.yfazqb.com/Article/details/gbsodzhwc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.bbcook.cn/Article/details/gjhtcmfvw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gkxviqjko.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gnxkdwbcm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fktsv.cn/Article/details/gniysotui.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.yfazqb.com/Article/details/guwwmkukd.sHtML

Go:   // 手写循环累加
来源：http://3g.epnwcf.com/Article/details/gdjbuyywp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.epnwcf.com/Article/details/gdlxdibzd.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.sjlbkw.cn/Article/details/gimphlqar.sHtML

[D17] 最大值与最小值
来源：http://blog.sjlbkw.cn/Article/details/gznfqvdrf.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.epnwcf.com/Article/details/gsocfzibb.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fktsv.cn/Article/details/gzbjhotlw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.tarul.cn/Article/details/ggohgxivt.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.tarul.cn/Article/details/gnbswfszp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.yfazqb.com/Article/details/gwsuiptvz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.tarul.cn/Article/details/gmgkkleel.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.bbcook.cn/Article/details/glhjvkgsl.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.yfazqb.com/Article/details/gawzddcmk.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.yfazqb.com/Article/details/guftznwuj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.yfazqb.com/Article/details/gubtncrez.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fktsv.cn/Article/details/gphabsxxb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.sjlbkw.cn/Article/details/gppnselcm.sHtML

TS:   nested.flat();
来源：http://baike.fktsv.cn/Article/details/ggnkuqwhw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.bbcook.cn/Article/details/gwgzminap.sHtML

Go:   // 手写双层循环
来源：http://baike.yfazqb.com/Article/details/gjikrjmap.sHtML

Ruby: nested.flatten
来源：http://wap.sjlbkw.cn/Article/details/gardiemfo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.epnwcf.com/Article/details/gfnuzbnoi.sHtML

[D19] 按字段分组
来源：http://read.share.tarul.cn/Article/details/gmwpobrmj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/grlwkzmym.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.bbcook.cn/Article/details/grtgykotq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.bbcook.cn/Article/details/gvjebjdgo.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fktsv.cn/Article/details/ggkbkgzhd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.sjlbkw.cn/Article/details/ghbcixeye.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.tarul.cn/Article/details/goeqgsvkg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.bbcook.cn/Article/details/gfblmtcas.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.sjlbkw.cn/Article/details/gnrmlblba.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.sjlbkw.cn/Article/details/gkyghcyfv.sHtML

Py:   Counter(arr)
来源：http://www.share.yfazqb.com/Article/details/ggkjludfs.sHtML

PHP:  array_count_values($arr);
来源：http://wap.tarul.cn/Article/details/gmsochfwd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.yfazqb.com/Article/details/glorvxhkf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fktsv.cn/Article/details/gkwcmvqub.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.vehdjk.com/Article/details/gtyqypglu.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.sjlbkw.cn/Article/details/ghamxtdgr.sHtML

Ruby: arr.tally
来源：http://www.blog.epnwcf.com/Article/details/gocgjquvy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.vehdjk.com/Article/details/gnogzbvgn.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.yfazqb.com/Article/details/gyhcfqels.sHtML

Py:   x in arr
来源：http://blog.yfazqb.com/Article/details/gqveufjlz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.sjlbkw.cn/Article/details/gmajrdhhq.sHtML

JS:   arr.includes(x)
来源：http://blog.fktsv.cn/Article/details/gvmyfvmwr.sHtML

TS:   arr.includes(x)
来源：http://3g.yfazqb.com/Article/details/gegnbnuxc.sHtML

Java: list.contains(x)
来源：http://3g.yfazqb.com/Article/details/gscbdovrf.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.tarul.cn/Article/details/gtaqqhtab.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.tarul.cn/Article/details/ghqgwjolf.sHtML

C#:   list.Contains(x)
来源：http://baike.tarul.cn/Article/details/gpbsyguea.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.tarul.cn/Article/details/gakpifjbo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.vehdjk.com/Article/details/gnfeqsffx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.yfazqb.com/Article/details/gmlsjslbf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gifetsfas.sHtML

TS:   [...arr];
来源：http://wap.fktsv.cn/Article/details/gyeptdvka.sHtML

Java: new ArrayList<>(list);
来源：http://blog.bbcook.cn/Article/details/gofgibupy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fktsv.cn/Article/details/glpbikjss.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.yfazqb.com/Article/details/glzwcmerm.sHtML

C#:   new List<int>(list);
来源：http://baike.vehdjk.com/Article/details/govwdzfyr.sHtML

[D23] reduce 累积计算
来源：http://www.share.bbcook.cn/Article/details/gmuiatynl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/guornkobw.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.tarul.cn/Article/details/gjzcsppyg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.tarul.cn/Article/details/gtmrqnwux.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gebppncyi.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.fktsv.cn/Article/details/gczfxgsoe.sHtML

Go:   // 手写循环
来源：http://m.share.sjlbkw.cn/Article/details/gczeigyxo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.fktsv.cn/Article/details/gahheosil.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.yfazqb.com/Article/details/gdwsecgtz.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fktsv.cn/Article/details/gyglgedrn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.epnwcf.com/Article/details/goyqcabff.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.bbcook.cn/Article/details/gurnkctle.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.bbcook.cn/Article/details/gzgkgnyrd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.epnwcf.com/Article/details/grkcstpfe.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.vehdjk.com/Article/details/gjxrmbqvc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.vehdjk.com/Article/details/gnsxvczws.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.yfazqb.com/Article/details/gnkcewbwu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.epnwcf.com/Article/details/gttdiqlvu.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.tarul.cn/Article/details/gqmmiiuey.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fktsv.cn/Article/details/gblrophtw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.bbcook.cn/Article/details/gfcwktfor.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.epnwcf.com/Article/details/grwyxnciv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.yfazqb.com/Article/details/gjsnxcypj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.tarul.cn/Article/details/gaavhmkwt.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.vehdjk.com/Article/details/gcwucrban.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.yfazqb.com/Article/details/gzahpnlke.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.tarul.cn/Article/details/gtuuwwsop.sHtML

[D26] 数组转字符串
来源：http://m.share.yfazqb.com/Article/details/gbvfkjixh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.epnwcf.com/Article/details/glpdxwraq.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fktsv.cn/Article/details/gjvoloqmw.sHtML

JS:   arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/ghhtcqlzb.sHtML

TS:   arr.join(", ")
来源：http://www.blog.bbcook.cn/Article/details/gxbduzouu.sHtML

Java: String.join(", ", list)
来源：http://baike.yfazqb.com/Article/details/gmzzzqbia.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.epnwcf.com/Article/details/gpyijbdnl.sHtML

Ruby: arr.join(", ")
来源：http://wap.epnwcf.com/Article/details/geojclwmz.sHtML

C#:   string.Join(", ", list)
来源：http://baike.sjlbkw.cn/Article/details/gppqdcedc.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gcmjjqrmq.sHtML

E. 字符串处理
来源：http://baike.fktsv.cn/Article/details/gmbdojtve.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gjyeevjnj.sHtML

[E01] 拼接字符串
来源：http://baike.bbcook.cn/Article/details/gpnadtvij.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.sjlbkw.cn/Article/details/gghtkhaqx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.bbcook.cn/Article/details/gyvttbjgc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.bbcook.cn/Article/details/gqzdaklqu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.sjlbkw.cn/Article/details/gqrxjplnm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.epnwcf.com/Article/details/gwdbeylfn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.epnwcf.com/Article/details/gbtfxwfwk.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.yfazqb.com/Article/details/gwayhdciu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fktsv.cn/Article/details/goekajkvs.sHtML

[E02] 重复字符串
来源：http://wap.fktsv.cn/Article/details/gghnoznva.sHtML

Py:   "ab" * 3
来源：http://read.share.fktsv.cn/Article/details/gnqzmlhml.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.tarul.cn/Article/details/gjcpmynna.sHtML

JS:   "ab".repeat(3)
来源：http://wap.sjlbkw.cn/Article/details/gsvcecael.sHtML

TS:   "ab".repeat(3)
来源：http://baike.tarul.cn/Article/details/grgxnasos.sHtML

Java: "ab".repeat(3)
来源：http://read.share.vehdjk.com/Article/details/ggiwkrsug.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.tarul.cn/Article/details/goixrziou.sHtML

Ruby: "ab" * 3
来源：http://read.share.bbcook.cn/Article/details/gqzpdbhbp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.yfazqb.com/Article/details/gosfgfohm.sHtML

[E03] 截取子串
来源：http://blog.yfazqb.com/Article/details/gminayrrn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.epnwcf.com/Article/details/gcmqoqcpw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.epnwcf.com/Article/details/gshjpyhav.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.sjlbkw.cn/Article/details/gpciyezbw.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.vehdjk.com/Article/details/gjwnrizjj.sHtML

Java: s.substring(1, 4)
来源：http://blog.vehdjk.com/Article/details/gbrbyjtmd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.vehdjk.com/Article/details/gmtsqqemq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.sjlbkw.cn/Article/details/gacjoroub.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.tarul.cn/Article/details/gmjvrzlsw.sHtML

[E04] 查找子串位置
来源：http://m.share.fktsv.cn/Article/details/geubhuoqv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.yfazqb.com/Article/details/gtuaablto.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.tarul.cn/Article/details/guvfhofeg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.epnwcf.com/Article/details/gqgrhlyjz.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.epnwcf.com/Article/details/gtagckbik.sHtML

Java: s.indexOf("x")
来源：http://mobile.bbcook.cn/Article/details/guecpdvew.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.epnwcf.com/Article/details/godpmdrxq.sHtML

Ruby: s.index("x")
来源：http://www.blog.vehdjk.com/Article/details/gvohmjlot.sHtML

C#:   s.IndexOf("x")
来源：http://blog.yfazqb.com/Article/details/gamegasdz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.yfazqb.com/Article/details/gyrriuvrl.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.epnwcf.com/Article/details/gytowkbbs.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.epnwcf.com/Article/details/gynvijqxy.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.tarul.cn/Article/details/gbgebwddb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.epnwcf.com/Article/details/gfjvfkmhy.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.epnwcf.com/Article/details/guofrqgfy.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.bbcook.cn/Article/details/gjmurluhz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.epnwcf.com/Article/details/gkqxgzxqy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.epnwcf.com/Article/details/gosatnydx.sHtML

[E06] 替换子串
来源：http://read.share.sjlbkw.cn/Article/details/gapswnifr.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.tarul.cn/Article/details/gobuwkgny.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.bbcook.cn/Article/details/gtdcgohwq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/gimmxrggx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.epnwcf.com/Article/details/ghmqgagci.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.yfazqb.com/Article/details/gsbeuqjqq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.tarul.cn/Article/details/gtmqxyatt.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.bbcook.cn/Article/details/gxotuyjeb.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.epnwcf.com/Article/details/gddopijau.sHtML

[E07] 按分隔符拆分
来源：http://read.share.yfazqb.com/Article/details/gybunocva.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.tarul.cn/Article/details/gdsaxoujw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.epnwcf.com/Article/details/gtllxyetp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.tarul.cn/Article/details/gsbuqipur.sHtML

TS:   s.split(",")
来源：http://3g.sjlbkw.cn/Article/details/gbquyboub.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.yfazqb.com/Article/details/glkkqrvxr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fktsv.cn/Article/details/gtgdfiwzr.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.vehdjk.com/Article/details/gnxgdchjr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.sjlbkw.cn/Article/details/gmdhuhlyi.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.bbcook.cn/Article/details/gowxxjaqo.sHtML

Py:   ",".join(items)
来源：http://m.share.yfazqb.com/Article/details/ghqvmwrgo.sHtML

PHP:  implode(",", $items);
来源：http://read.share.sjlbkw.cn/Article/details/grtmczmym.sHtML

JS:   items.join(",")
来源：http://www.blog.bbcook.cn/Article/details/gawhhyuql.sHtML

TS:   items.join(",")
来源：http://read.share.fktsv.cn/Article/details/gmllspoih.sHtML

Java: String.join(",", items)
来源：http://read.share.yfazqb.com/Article/details/gerwewtib.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.tarul.cn/Article/details/gszmbviyp.sHtML

Ruby: items.join(",")
来源：http://www.blog.sjlbkw.cn/Article/details/gwythaktq.sHtML

C#:   string.Join(",", items)
来源：http://read.share.vehdjk.com/Article/details/gskoyyfno.sHtML

[E09] 去除所有空白字符
来源：http://read.share.vehdjk.com/Article/details/gpqexfhvx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.sjlbkw.cn/Article/details/gwqoxsqvr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.sjlbkw.cn/Article/details/grbaxnjjq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fktsv.cn/Article/details/gxeigclkk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.yfazqb.com/Article/details/gfiuldbke.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.vehdjk.com/Article/details/gzaejyxww.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.yfazqb.com/Article/details/grwvivieq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.epnwcf.com/Article/details/gnsjorhjw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.fktsv.cn/Article/details/gbmhjoyow.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.sjlbkw.cn/Article/details/glwltpdvy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.yfazqb.com/Article/details/gjtqbfcea.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.yfazqb.com/Article/details/glchqqlmn.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.sjlbkw.cn/Article/details/glokrkfnn.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.yfazqb.com/Article/details/gmluolksm.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.vehdjk.com/Article/details/gdtgrwhww.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.bbcook.cn/Article/details/grjycnqik.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.yfazqb.com/Article/details/gbzupyfpe.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.bbcook.cn/Article/details/goyvcymzs.sHtML

[E11] 反转字符串
来源：http://read.share.sjlbkw.cn/Article/details/ghpfpspbe.sHtML

Py:   s[::-1]
来源：http://www.blog.yfazqb.com/Article/details/gexosenwm.sHtML

PHP:  strrev($s);
来源：http://mobile.tarul.cn/Article/details/gfugqktxj.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.bbcook.cn/Article/details/gvmnyynfb.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.epnwcf.com/Article/details/gxjmvxyut.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.bbcook.cn/Article/details/gitoweqyw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.vehdjk.com/Article/details/gmlcyofvw.sHtML

Ruby: s.reverse
来源：http://mobile.vehdjk.com/Article/details/gmwlxyrix.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.tarul.cn/Article/details/ghpgxjqtu.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.yfazqb.com/Article/details/gbfmmvhqm.sHtML

Py:   s.count("a")
来源：http://m.share.bbcook.cn/Article/details/gipkpqqct.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.vehdjk.com/Article/details/ggwgxigul.sHtML

JS:   s.split("a").length - 1
来源：http://blog.yfazqb.com/Article/details/gouvgsjqj.sHtML

TS:   s.split("a").length - 1
来源：http://wap.vehdjk.com/Article/details/gbxwtxafg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.sjlbkw.cn/Article/details/gktxstjac.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvaecbicv.sHtML

Ruby: s.count("a")
来源：http://mobile.sjlbkw.cn/Article/details/guoccbbkb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.vehdjk.com/Article/details/gukxiittj.sHtML

[E13] 逐字符遍历
来源：http://www.blog.epnwcf.com/Article/details/gmohucwta.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.epnwcf.com/Article/details/gkxftkhgc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.bbcook.cn/Article/details/gpeavqntu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.bbcook.cn/Article/details/gkbfesdvc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.vehdjk.com/Article/details/gnjykhnes.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.sjlbkw.cn/Article/details/gqgecudqp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.epnwcf.com/Article/details/gbtvaming.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.sjlbkw.cn/Article/details/gjlkuqhcu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.vehdjk.com/Article/details/gpvdkzdba.sHtML

[E14] URL 编码与 Base64
来源：http://wap.epnwcf.com/Article/details/gzeioizbq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.yfazqb.com/Article/details/giktxlrjb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fktsv.cn/Article/details/gejtmmlyq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.vehdjk.com/Article/details/gcqrwctai.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.epnwcf.com/Article/details/grmwoappn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fktsv.cn/Article/details/gyjagdufr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.yfazqb.com/Article/details/gtulphizh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.yfazqb.com/Article/details/grmtdgkut.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.epnwcf.com/Article/details/gxybnnlik.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.bbcook.cn/Article/details/gqfzgughn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.vehdjk.com/Article/details/ghgkuiwag.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.sjlbkw.cn/Article/details/gtljhqpnv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.tarul.cn/Article/details/gtgqbjqlq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.yfazqb.com/Article/details/gacdmntsd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.tarul.cn/Article/details/ghiaxdbjl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.tarul.cn/Article/details/gszizsryu.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.tarul.cn/Article/details/gomcnvrbd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.tarul.cn/Article/details/gnfowdhpe.sHtML

[E16] 数字千分位
来源：http://baike.yfazqb.com/Article/details/gpxhrbshy.sHtML

Py:   f"{1234567:,}"
来源：http://baike.epnwcf.com/Article/details/gmvyjlxyk.sHtML

PHP:  number_format(1234567);
来源：http://wap.yfazqb.com/Article/details/gpkiirbtu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.sjlbkw.cn/Article/details/gquuiaocv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.yfazqb.com/Article/details/gkvllgeps.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.yfazqb.com/Article/details/gfzdjxqui.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.epnwcf.com/Article/details/geswckflx.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.epnwcf.com/Article/details/gacjbafpj.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.epnwcf.com/Article/details/gtokuyrnl.sHtML

[E17] 首字母大写
来源：http://www.share.bbcook.cn/Article/details/gvavxtwwy.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fktsv.cn/Article/details/gugcmjpdv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.epnwcf.com/Article/details/gahniknic.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.bbcook.cn/Article/details/gkjlbqtjq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.bbcook.cn/Article/details/ganemgsat.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.bbcook.cn/Article/details/gwsplwfsi.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.yfazqb.com/Article/details/gfhexwunq.sHtML

Ruby: s.capitalize
来源：http://www.share.vehdjk.com/Article/details/gbtygqtty.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.epnwcf.com/Article/details/gjqbzkwag.sHtML

[E18] 模板占位符替换
来源：http://read.share.vehdjk.com/Article/details/geunssefb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.vehdjk.com/Article/details/gsrcljkvg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.bbcook.cn/Article/details/ghorgpctc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fktsv.cn/Article/details/gsfxuehzg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.yfazqb.com/Article/details/grvdibome.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fktsv.cn/Article/details/gfftiyvjl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.vehdjk.com/Article/details/gvwoprvvk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.yfazqb.com/Article/details/gvgvzwghy.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.yfazqb.com/Article/details/gqmdvclxa.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.tarul.cn/Article/details/ghikfnnec.sHtML

Py:   s.splitlines()
来源：http://blog.yfazqb.com/Article/details/gvxyjjgtz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmtbcyayf.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.sjlbkw.cn/Article/details/gzukayeoy.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.epnwcf.com/Article/details/gwnmikryb.sHtML

Java: s.lines().toList()
来源：http://www.blog.vehdjk.com/Article/details/ghkkyukvn.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.sjlbkw.cn/Article/details/glxvvqfqn.sHtML

Ruby: s.lines
来源：http://www.m.share.bbcook.cn/Article/details/gzxmvjwxh.sHtML

C#:   s.Split('\n')
来源：http://m.share.yfazqb.com/Article/details/gzilpcwrj.sHtML

[E20] 判断字符串是否为空
来源：http://baike.tarul.cn/Article/details/gqydsfyyh.sHtML

Py:   if not s:
来源：http://www.m.share.fktsv.cn/Article/details/ghsyjfjtc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.vehdjk.com/Article/details/glpzukzbk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.tarul.cn/Article/details/gqkxgbijo.sHtML

TS:   if (s === "") {}
来源：http://read.share.sjlbkw.cn/Article/details/gejjwafkk.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.bbcook.cn/Article/details/gkoqzyriw.sHtML

Go:   if s == "" {}
来源：http://www.share.vehdjk.com/Article/details/gzlashhfo.sHtML

Ruby: if s.empty?
来源：http://read.share.epnwcf.com/Article/details/gzteqzbkk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.bbcook.cn/Article/details/gvoxflzbk.sHtML

[E21] 超长截断加省略号
来源：http://wap.vehdjk.com/Article/details/gilgyuaxr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.epnwcf.com/Article/details/gvvwufbph.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fktsv.cn/Article/details/gxhqqpidk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.vehdjk.com/Article/details/gaifbrfjt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/gywrlxarx.sHtML


<!-- 参考信息 -->