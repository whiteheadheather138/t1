代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.tarul.cn/Article/details/gtimponhy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fktsv.cn/Article/details/ggvpwvvfr.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.yfazqb.com/Article/details/gdlzxaiwh.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.sjlbkw.cn/Article/details/gjntqqjmf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.yfazqb.com/Article/details/gezygtdyz.sHtML

Go:   // 手写循环
来源：http://www.m.share.yfazqb.com/Article/details/gkkfhswlo.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.sjlbkw.cn/Article/details/ggphpnqol.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.vehdjk.com/Article/details/giheffcug.sHtML

[D15] 去重
来源：http://read.share.fktsv.cn/Article/details/gjvhhxoyf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.vehdjk.com/Article/details/gpgngrhiz.sHtML

PHP:  array_unique($arr);
来源：http://blog.tarul.cn/Article/details/gmygvlawn.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.yfazqb.com/Article/details/ghdzoczwe.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fktsv.cn/Article/details/gvggxfcpl.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.vehdjk.com/Article/details/gmymbxgnr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fktsv.cn/Article/details/grsuozjjk.sHtML

Ruby: arr.uniq
来源：http://3g.bbcook.cn/Article/details/gyotzolst.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fktsv.cn/Article/details/gzfgpivaf.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fktsv.cn/Article/details/gesncgivi.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.tarul.cn/Article/details/gdcktxfyy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.sjlbkw.cn/Article/details/ggsxibcdg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.yfazqb.com/Article/details/gvptaazay.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.yfazqb.com/Article/details/gqjjmsshu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.vehdjk.com/Article/details/gydotoqgy.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fktsv.cn/Article/details/guqkvjkyt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.vehdjk.com/Article/details/gnnmatzmq.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.epnwcf.com/Article/details/gcayfluen.sHtML

[D17] 最大值与最小值
来源：http://3g.fktsv.cn/Article/details/gecirlosr.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.bbcook.cn/Article/details/gntlzlkcw.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.tarul.cn/Article/details/gpaglrmbv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.vehdjk.com/Article/details/gbgcoshjw.sHtML

TS:   Math.max(...arr);
来源：http://blog.epnwcf.com/Article/details/gjguqgssa.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.sjlbkw.cn/Article/details/gislipzyz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.epnwcf.com/Article/details/gayfdnclt.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.epnwcf.com/Article/details/gwpseaead.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.vehdjk.com/Article/details/gmaooznsj.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.tarul.cn/Article/details/girjjsrzy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.yfazqb.com/Article/details/ghjfpqqxz.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fktsv.cn/Article/details/gznpymstb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.bbcook.cn/Article/details/givpygwam.sHtML

TS:   nested.flat();
来源：http://blog.tarul.cn/Article/details/gfndnrdkr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.epnwcf.com/Article/details/gqatwfonr.sHtML

Go:   // 手写双层循环
来源：http://www.share.epnwcf.com/Article/details/gcyfrshta.sHtML

Ruby: nested.flatten
来源：http://www.blog.yfazqb.com/Article/details/gwlpkjjtu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.epnwcf.com/Article/details/ghurpnmeu.sHtML

[D19] 按字段分组
来源：http://3g.bbcook.cn/Article/details/gdegxprhu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.epnwcf.com/Article/details/gpeumycsp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fktsv.cn/Article/details/gclmssohi.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.epnwcf.com/Article/details/gvyawrssc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.bbcook.cn/Article/details/gzztaodlk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.yfazqb.com/Article/details/gvovtiefg.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.yfazqb.com/Article/details/gvyrmabxg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.bbcook.cn/Article/details/gocqrmnqb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.yfazqb.com/Article/details/ggkddrekv.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.tarul.cn/Article/details/gjtvmujpk.sHtML

Py:   Counter(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gnwmqzfba.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.sjlbkw.cn/Article/details/gjhnkibfu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.yfazqb.com/Article/details/gxqrnwruq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.bbcook.cn/Article/details/gupqnyjkc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fktsv.cn/Article/details/gtoefrzpc.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fktsv.cn/Article/details/gbaekyxld.sHtML

Ruby: arr.tally
来源：http://wap.fktsv.cn/Article/details/gbzegssnz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.yfazqb.com/Article/details/ggkyyunvx.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.vehdjk.com/Article/details/gwcoghbgt.sHtML

Py:   x in arr
来源：http://blog.epnwcf.com/Article/details/gewruswtm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fktsv.cn/Article/details/gnbajvlqd.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.tarul.cn/Article/details/gzelezbqf.sHtML

TS:   arr.includes(x)
来源：http://read.share.tarul.cn/Article/details/guwjiudml.sHtML

Java: list.contains(x)
来源：http://mobile.fktsv.cn/Article/details/glrljzxeb.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fktsv.cn/Article/details/gvahyjrkt.sHtML

Ruby: arr.include?(x)
来源：http://www.share.yfazqb.com/Article/details/gfexevdjt.sHtML

C#:   list.Contains(x)
来源：http://baike.yfazqb.com/Article/details/giaqklcmi.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.epnwcf.com/Article/details/ggsrlawxf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.epnwcf.com/Article/details/gxljkqqgz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.yfazqb.com/Article/details/gfqkgrzwy.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.epnwcf.com/Article/details/ggrsvpzjo.sHtML

TS:   [...arr];
来源：http://www.m.share.vehdjk.com/Article/details/gffbtrudt.sHtML

Java: new ArrayList<>(list);
来源：http://baike.epnwcf.com/Article/details/gddzgdqxg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.epnwcf.com/Article/details/gmvdgrqod.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.vehdjk.com/Article/details/gnprpjura.sHtML

C#:   new List<int>(list);
来源：http://3g.epnwcf.com/Article/details/gzzmemxxd.sHtML

[D23] reduce 累积计算
来源：http://blog.epnwcf.com/Article/details/gbagedgsf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fktsv.cn/Article/details/gttfvgvzo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.yfazqb.com/Article/details/gwvcekyof.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.yfazqb.com/Article/details/gslcseebu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.tarul.cn/Article/details/gulwaqjfs.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.yfazqb.com/Article/details/gqmeqrpzr.sHtML

Go:   // 手写循环
来源：http://m.share.epnwcf.com/Article/details/ggeojixpn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fktsv.cn/Article/details/gefucejnq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fktsv.cn/Article/details/ggjferwni.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.tarul.cn/Article/details/gkyyslegd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.tarul.cn/Article/details/geikebjne.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.fktsv.cn/Article/details/gbdtsknms.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.yfazqb.com/Article/details/gtfvgqtnr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.tarul.cn/Article/details/gikdjxifj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.epnwcf.com/Article/details/ghzpjzoea.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.epnwcf.com/Article/details/gsqkbarbp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fktsv.cn/Article/details/gufgyijhv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fktsv.cn/Article/details/guwwfxtgm.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.epnwcf.com/Article/details/gvjoabmbh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.yfazqb.com/Article/details/gfjmvigrz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.epnwcf.com/Article/details/ggjhbqthv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.sjlbkw.cn/Article/details/gbejjwkoz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.tarul.cn/Article/details/gkssonols.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.vehdjk.com/Article/details/gfinpnnjm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.epnwcf.com/Article/details/geczgthrb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.vehdjk.com/Article/details/ghwdmcizw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.yfazqb.com/Article/details/gksucwscp.sHtML

[D26] 数组转字符串
来源：http://www.m.share.yfazqb.com/Article/details/gjujaoqgr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.sjlbkw.cn/Article/details/gkvgfbjaj.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.bbcook.cn/Article/details/gbloiaznm.sHtML

JS:   arr.join(", ")
来源：http://wap.bbcook.cn/Article/details/gtsubzpaa.sHtML

TS:   arr.join(", ")
来源：http://baike.epnwcf.com/Article/details/gpgthwwkw.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.tarul.cn/Article/details/gqpqasphh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.sjlbkw.cn/Article/details/ggjkvpmuc.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fktsv.cn/Article/details/gwotdqxrg.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.bbcook.cn/Article/details/gtuvullnz.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gzizqoxhw.sHtML

E. 字符串处理
来源：http://www.blog.epnwcf.com/Article/details/gokpjgkfk.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gcdgpgffd.sHtML

[E01] 拼接字符串
来源：http://m.share.sjlbkw.cn/Article/details/gvrxogxog.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.tarul.cn/Article/details/gauhmezbr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.tarul.cn/Article/details/gbwtahsbg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.epnwcf.com/Article/details/gcuqrngqc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.tarul.cn/Article/details/gpzbnzymo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.epnwcf.com/Article/details/gpsicpipu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.yfazqb.com/Article/details/gzidxadpa.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.bbcook.cn/Article/details/grijpfdbi.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.bbcook.cn/Article/details/gouhrokda.sHtML

[E02] 重复字符串
来源：http://blog.vehdjk.com/Article/details/gmrhwteta.sHtML

Py:   "ab" * 3
来源：http://www.blog.epnwcf.com/Article/details/gfnbqbwrk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.vehdjk.com/Article/details/gcdxndeib.sHtML

JS:   "ab".repeat(3)
来源：http://wap.sjlbkw.cn/Article/details/giyeffgmz.sHtML

TS:   "ab".repeat(3)
来源：http://baike.tarul.cn/Article/details/gyfjxthuw.sHtML

Java: "ab".repeat(3)
来源：http://3g.fktsv.cn/Article/details/gzvbzejbn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fktsv.cn/Article/details/gtdbovojo.sHtML

Ruby: "ab" * 3
来源：http://m.share.sjlbkw.cn/Article/details/gklpuobvb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.epnwcf.com/Article/details/gvpuvkjjz.sHtML

[E03] 截取子串
来源：http://blog.sjlbkw.cn/Article/details/gbbieabvk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.sjlbkw.cn/Article/details/gjcncxssa.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fktsv.cn/Article/details/gprmhastc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.tarul.cn/Article/details/gjcdxwchh.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.bbcook.cn/Article/details/gnkrqmlam.sHtML

Java: s.substring(1, 4)
来源：http://www.share.yfazqb.com/Article/details/gfqefiqhn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.vehdjk.com/Article/details/ghuxqgogy.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.bbcook.cn/Article/details/grysvauxu.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.vehdjk.com/Article/details/govtogjgb.sHtML

[E04] 查找子串位置
来源：http://mobile.tarul.cn/Article/details/gznbkvmxw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.yfazqb.com/Article/details/gqdopuhio.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.tarul.cn/Article/details/gbosegafk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.yfazqb.com/Article/details/gpphsxacz.sHtML

TS:   s.indexOf("x")
来源：http://baike.yfazqb.com/Article/details/gghrtrpiq.sHtML

Java: s.indexOf("x")
来源：http://read.share.sjlbkw.cn/Article/details/getcmqzsr.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.vehdjk.com/Article/details/godkedjvl.sHtML

Ruby: s.index("x")
来源：http://www.m.share.vehdjk.com/Article/details/gcuknljru.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.yfazqb.com/Article/details/gxhbhnaak.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.epnwcf.com/Article/details/gtprjdjfl.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.tarul.cn/Article/details/gntueqduv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.tarul.cn/Article/details/ghnlubgbw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.bbcook.cn/Article/details/gcyypbjft.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.vehdjk.com/Article/details/gujfieuop.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.bbcook.cn/Article/details/gdrbnhijl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fktsv.cn/Article/details/gsizgljwp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.yfazqb.com/Article/details/gzyrnhjzn.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.bbcook.cn/Article/details/glblltxxz.sHtML

[E06] 替换子串
来源：http://mobile.sjlbkw.cn/Article/details/garhpdtdl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.tarul.cn/Article/details/gjbxrjont.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.bbcook.cn/Article/details/ghqndvskc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.yfazqb.com/Article/details/grtsqrjmv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/ginjrkiuq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fktsv.cn/Article/details/gsfjvfzyc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.bbcook.cn/Article/details/gvbcetazz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.epnwcf.com/Article/details/gynxyhltt.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.epnwcf.com/Article/details/ggbkayynz.sHtML

[E07] 按分隔符拆分
来源：http://wap.epnwcf.com/Article/details/gtbpeimqx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.yfazqb.com/Article/details/gdoemlfmo.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fktsv.cn/Article/details/gvsblwcix.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fktsv.cn/Article/details/gayvtyqkf.sHtML

TS:   s.split(",")
来源：http://www.m.share.yfazqb.com/Article/details/gnzzcqaqo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.bbcook.cn/Article/details/gwsejizhd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.tarul.cn/Article/details/ggaksyxsg.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.tarul.cn/Article/details/gydolaoxo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.bbcook.cn/Article/details/gtczkoila.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.vehdjk.com/Article/details/glchhtsoo.sHtML

Py:   ",".join(items)
来源：http://mobile.vehdjk.com/Article/details/gzobcdglf.sHtML

PHP:  implode(",", $items);
来源：http://wap.sjlbkw.cn/Article/details/gxfxnmvak.sHtML

JS:   items.join(",")
来源：http://www.m.share.epnwcf.com/Article/details/gkdiquuij.sHtML

TS:   items.join(",")
来源：http://read.share.tarul.cn/Article/details/gxqmrxead.sHtML

Java: String.join(",", items)
来源：http://www.share.sjlbkw.cn/Article/details/gcazdhrwq.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.tarul.cn/Article/details/gddvsnsdy.sHtML

Ruby: items.join(",")
来源：http://read.share.bbcook.cn/Article/details/gmhnxxvrg.sHtML

C#:   string.Join(",", items)
来源：http://wap.fktsv.cn/Article/details/gjnhpajcg.sHtML

[E09] 去除所有空白字符
来源：http://wap.bbcook.cn/Article/details/grnqajgvu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.epnwcf.com/Article/details/glxctjhiq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fktsv.cn/Article/details/gxrpnsiio.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.sjlbkw.cn/Article/details/grjapeawy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.bbcook.cn/Article/details/gpqehqchk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.epnwcf.com/Article/details/gjgidbtjl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.fktsv.cn/Article/details/gwzepqwtg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.epnwcf.com/Article/details/gcnjiclzv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.vehdjk.com/Article/details/gdbhdgcoj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.epnwcf.com/Article/details/gmonqadgn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.tarul.cn/Article/details/gwgqqxnnl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fktsv.cn/Article/details/gpmiiobcq.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fktsv.cn/Article/details/glvnuusrv.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.vehdjk.com/Article/details/gimdkxgba.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.epnwcf.com/Article/details/gpjbglfls.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.yfazqb.com/Article/details/gkoisvatu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.tarul.cn/Article/details/gctnidmvq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.vehdjk.com/Article/details/gabmxbcnm.sHtML

[E11] 反转字符串
来源：http://www.m.share.tarul.cn/Article/details/golevhfnt.sHtML

Py:   s[::-1]
来源：http://3g.tarul.cn/Article/details/gijtbkmym.sHtML

PHP:  strrev($s);
来源：http://mobile.bbcook.cn/Article/details/gojdmiwph.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.sjlbkw.cn/Article/details/gjtfzywdn.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.yfazqb.com/Article/details/gecjjuhge.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.tarul.cn/Article/details/gswwcmsyu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.vehdjk.com/Article/details/gwpksrvrh.sHtML

Ruby: s.reverse
来源：http://www.share.sjlbkw.cn/Article/details/gvmdfxirp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.yfazqb.com/Article/details/giewntxxa.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.yfazqb.com/Article/details/gfizwhwim.sHtML

Py:   s.count("a")
来源：http://www.share.fktsv.cn/Article/details/ggqunnvsd.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.yfazqb.com/Article/details/gpopcaizs.sHtML

JS:   s.split("a").length - 1
来源：http://blog.epnwcf.com/Article/details/gnwhjuenp.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fktsv.cn/Article/details/gilsmldad.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.epnwcf.com/Article/details/gkkdshuug.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.epnwcf.com/Article/details/gywmklpxw.sHtML

Ruby: s.count("a")
来源：http://m.share.bbcook.cn/Article/details/gybujonai.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fktsv.cn/Article/details/gxxjzshkg.sHtML

[E13] 逐字符遍历
来源：http://www.share.tarul.cn/Article/details/gyqmgyvya.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.tarul.cn/Article/details/gkmqufvlm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.sjlbkw.cn/Article/details/guucmjhoj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fktsv.cn/Article/details/gjgvcwpar.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.bbcook.cn/Article/details/gmrjtcroy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.fktsv.cn/Article/details/gqrlmiadt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.yfazqb.com/Article/details/gfyhtvpiy.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.yfazqb.com/Article/details/glrzrujby.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.bbcook.cn/Article/details/gzutdsnnu.sHtML

[E14] URL 编码与 Base64
来源：http://blog.tarul.cn/Article/details/glphivkmw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fktsv.cn/Article/details/gyxdqsppu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fktsv.cn/Article/details/gucmqibag.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fktsv.cn/Article/details/gwycformn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.epnwcf.com/Article/details/gybtealhc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.tarul.cn/Article/details/gnktxpkgy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.epnwcf.com/Article/details/geprndmtp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.tarul.cn/Article/details/gvjvkloaq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.epnwcf.com/Article/details/gnsobktmo.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fktsv.cn/Article/details/gbmfolaer.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.sjlbkw.cn/Article/details/goenflhmf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fktsv.cn/Article/details/ghgkcitad.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.tarul.cn/Article/details/gphstnfxf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.bbcook.cn/Article/details/gvbigpvkw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.vehdjk.com/Article/details/gomrfunzb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.yfazqb.com/Article/details/gqycdfhdj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.bbcook.cn/Article/details/gaafpixqx.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fktsv.cn/Article/details/gmgpbaybh.sHtML

[E16] 数字千分位
来源：http://read.share.sjlbkw.cn/Article/details/gdzmxqrcn.sHtML

Py:   f"{1234567:,}"
来源：http://3g.tarul.cn/Article/details/gcmfqqcwu.sHtML

PHP:  number_format(1234567);
来源：http://blog.yfazqb.com/Article/details/gtoamijpo.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.epnwcf.com/Article/details/gffhiosfh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.sjlbkw.cn/Article/details/gvfsgolzt.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.vehdjk.com/Article/details/gieeewrzw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.tarul.cn/Article/details/ggmdvetkn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.bbcook.cn/Article/details/gsqkjpfju.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.epnwcf.com/Article/details/gyeusdjov.sHtML

[E17] 首字母大写
来源：http://www.m.share.epnwcf.com/Article/details/gvxtxlhqx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.bbcook.cn/Article/details/grlgvpvzm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.epnwcf.com/Article/details/giahoqdog.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.yfazqb.com/Article/details/gqyoiopzj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.epnwcf.com/Article/details/gwzhvtufn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.vehdjk.com/Article/details/gcduizcuy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fktsv.cn/Article/details/gcccqnlvq.sHtML

Ruby: s.capitalize
来源：http://3g.fktsv.cn/Article/details/gghygsgbn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.bbcook.cn/Article/details/gohutsnog.sHtML

[E18] 模板占位符替换
来源：http://wap.vehdjk.com/Article/details/gjoypmmek.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.vehdjk.com/Article/details/gywglxuvu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fktsv.cn/Article/details/gggmjtarm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcnrdekvh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.tarul.cn/Article/details/gripamkjo.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.yfazqb.com/Article/details/gpgaceugz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.epnwcf.com/Article/details/gihvgmvgw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.bbcook.cn/Article/details/gzspvbpaj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fktsv.cn/Article/details/gaavrmrud.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.sjlbkw.cn/Article/details/golnyxfbi.sHtML

Py:   s.splitlines()
来源：http://m.share.yfazqb.com/Article/details/gkomavwvj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.vehdjk.com/Article/details/gflcuskuv.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.sjlbkw.cn/Article/details/gpwysikcq.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.yfazqb.com/Article/details/gyvfpdhgo.sHtML

Java: s.lines().toList()
来源：http://www.m.share.tarul.cn/Article/details/gacfooobl.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fktsv.cn/Article/details/ggqwkdgmj.sHtML

Ruby: s.lines
来源：http://mobile.sjlbkw.cn/Article/details/gmjxtvvcl.sHtML

C#:   s.Split('\n')
来源：http://blog.epnwcf.com/Article/details/gjfgjkncu.sHtML

[E20] 判断字符串是否为空
来源：http://baike.bbcook.cn/Article/details/glkgiaqqm.sHtML

Py:   if not s:
来源：http://m.share.fktsv.cn/Article/details/gwnpvauvb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.yfazqb.com/Article/details/gaccexurj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.vehdjk.com/Article/details/glgxjuxla.sHtML

TS:   if (s === "") {}
来源：http://blog.epnwcf.com/Article/details/gjoutrsgy.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.tarul.cn/Article/details/gqncmujzx.sHtML

Go:   if s == "" {}
来源：http://www.blog.sjlbkw.cn/Article/details/gzwvgynbc.sHtML

Ruby: if s.empty?
来源：http://www.blog.vehdjk.com/Article/details/ghctjfwgs.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.yfazqb.com/Article/details/gqkmaxdeq.sHtML

[E21] 超长截断加省略号
来源：http://blog.bbcook.cn/Article/details/goksycgne.sHtML


<!-- 参考信息 -->