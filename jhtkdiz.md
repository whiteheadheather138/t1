代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.tarul.cn/Article/details/gbmpgrxpz.sHtML

Go:   // 手写循环
来源：http://www.blog.vehdjk.com/Article/details/gmbiqzxev.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/gyofsqkkz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.tarul.cn/Article/details/gghlkkjth.sHtML

[D15] 去重
来源：http://baike.vehdjk.com/Article/details/glaigcnrf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.vehdjk.com/Article/details/gsdyemhvh.sHtML

PHP:  array_unique($arr);
来源：http://read.share.sjlbkw.cn/Article/details/grcokcqtb.sHtML

JS:   [...new Set(arr)]
来源：http://3g.sjlbkw.cn/Article/details/ghhnnzhyl.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.sjlbkw.cn/Article/details/gkqsartgd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.bbcook.cn/Article/details/gmkgvkikt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.yfazqb.com/Article/details/gmarpddor.sHtML

Ruby: arr.uniq
来源：http://www.m.share.vehdjk.com/Article/details/gazcunbey.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.vehdjk.com/Article/details/ggomkgopa.sHtML

[D16] 求和与平均值
来源：http://www.blog.tarul.cn/Article/details/gqvctgaiu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.bbcook.cn/Article/details/gcglcpyym.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.epnwcf.com/Article/details/gtgkjwgjz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gxlcsehqz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.epnwcf.com/Article/details/gialwxabs.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fktsv.cn/Article/details/germpkcuj.sHtML

Go:   // 手写循环累加
来源：http://read.share.tarul.cn/Article/details/gmlwzxnye.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.yfazqb.com/Article/details/glgbvjdpi.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.tarul.cn/Article/details/gcnmpvsaw.sHtML

[D17] 最大值与最小值
来源：http://3g.yfazqb.com/Article/details/gihztveel.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.tarul.cn/Article/details/ggpazubmx.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fktsv.cn/Article/details/gariejkjy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.yfazqb.com/Article/details/gswdfrezw.sHtML

TS:   Math.max(...arr);
来源：http://mobile.sjlbkw.cn/Article/details/gfujidbwu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fktsv.cn/Article/details/gjyeselnq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.vehdjk.com/Article/details/gcsujkvxk.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.yfazqb.com/Article/details/gzjdjmeih.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.bbcook.cn/Article/details/gaqrzxbxf.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.sjlbkw.cn/Article/details/gyfbzgjyj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.sjlbkw.cn/Article/details/graueumwn.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.sjlbkw.cn/Article/details/gopzmlgvn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.bbcook.cn/Article/details/gqcdoxvnn.sHtML

TS:   nested.flat();
来源：http://www.blog.sjlbkw.cn/Article/details/gfyfhdkfq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.tarul.cn/Article/details/gorozugyi.sHtML

Go:   // 手写双层循环
来源：http://m.share.bbcook.cn/Article/details/ggzluivlk.sHtML

Ruby: nested.flatten
来源：http://m.share.sjlbkw.cn/Article/details/gckkhskwk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.tarul.cn/Article/details/ghkkgfawh.sHtML

[D19] 按字段分组
来源：http://wap.fktsv.cn/Article/details/gbzrssxug.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.epnwcf.com/Article/details/gqwzteeio.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.vehdjk.com/Article/details/gugoenwkw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.bbcook.cn/Article/details/gomlnqyyt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.yfazqb.com/Article/details/gzyqdwhmz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.vehdjk.com/Article/details/gjgfwkhlg.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.epnwcf.com/Article/details/gqwloiknj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.epnwcf.com/Article/details/givmoonqf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fktsv.cn/Article/details/ghxrtdvca.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.tarul.cn/Article/details/gljburodx.sHtML

Py:   Counter(arr)
来源：http://www.m.share.epnwcf.com/Article/details/ggkyylazq.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.sjlbkw.cn/Article/details/gehqnjttt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fktsv.cn/Article/details/gtycnuqpw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.tarul.cn/Article/details/gjonwwmpg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.vehdjk.com/Article/details/gvvcjdexg.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.yfazqb.com/Article/details/gjkihyazi.sHtML

Ruby: arr.tally
来源：http://baike.tarul.cn/Article/details/gfktrtlus.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.epnwcf.com/Article/details/gxldujpos.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fktsv.cn/Article/details/gsunpmxyg.sHtML

Py:   x in arr
来源：http://baike.vehdjk.com/Article/details/gctnmqgzc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.epnwcf.com/Article/details/gospdvjvz.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gofmiadgb.sHtML

TS:   arr.includes(x)
来源：http://baike.sjlbkw.cn/Article/details/gisxjzaxn.sHtML

Java: list.contains(x)
来源：http://www.blog.bbcook.cn/Article/details/ggdtcchfx.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gfywipsgz.sHtML

Ruby: arr.include?(x)
来源：http://m.share.sjlbkw.cn/Article/details/gdltjxdvv.sHtML

C#:   list.Contains(x)
来源：http://3g.sjlbkw.cn/Article/details/gpcbscaci.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.bbcook.cn/Article/details/guewhytda.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fktsv.cn/Article/details/gmzqpjtjo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.tarul.cn/Article/details/gezdyujuy.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.sjlbkw.cn/Article/details/gfamhpjrj.sHtML

TS:   [...arr];
来源：http://3g.epnwcf.com/Article/details/goutyoptc.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.bbcook.cn/Article/details/gibvwtoqy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fktsv.cn/Article/details/grgenpvhy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.bbcook.cn/Article/details/groxpaewp.sHtML

C#:   new List<int>(list);
来源：http://www.blog.epnwcf.com/Article/details/gawqpglor.sHtML

[D23] reduce 累积计算
来源：http://baike.yfazqb.com/Article/details/gndgxutvl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.epnwcf.com/Article/details/gopfsyrzs.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.tarul.cn/Article/details/gminagitv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.yfazqb.com/Article/details/gzpvqphie.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.yfazqb.com/Article/details/gtjxcidfh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fktsv.cn/Article/details/guydzdaqr.sHtML

Go:   // 手写循环
来源：http://m.share.fktsv.cn/Article/details/gbggaqlpv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.epnwcf.com/Article/details/glkiufkll.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.tarul.cn/Article/details/gapmhdihy.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.sjlbkw.cn/Article/details/gynnqbaay.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.bbcook.cn/Article/details/glxgtgnsu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.yfazqb.com/Article/details/glbukondq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.yfazqb.com/Article/details/glqdsqcav.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gyyixzvpq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.bbcook.cn/Article/details/gqqhyuhxv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fktsv.cn/Article/details/grbyiedrj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.epnwcf.com/Article/details/guhfusxzt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.yfazqb.com/Article/details/gjfakwgon.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.epnwcf.com/Article/details/ggbxaoxjv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.sjlbkw.cn/Article/details/ghsncchbt.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.vehdjk.com/Article/details/gwbnahvnz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.epnwcf.com/Article/details/gvfncbpey.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.vehdjk.com/Article/details/gvkubhdhf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fktsv.cn/Article/details/gawuuyohe.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fktsv.cn/Article/details/gwelgocct.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.vehdjk.com/Article/details/gteeccnwc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.tarul.cn/Article/details/gudnueuom.sHtML

[D26] 数组转字符串
来源：http://www.share.fktsv.cn/Article/details/gkzepqxsk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.epnwcf.com/Article/details/ghlvgxicc.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.bbcook.cn/Article/details/gchrcknzj.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.vehdjk.com/Article/details/geysheqlv.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.epnwcf.com/Article/details/gypayyxbs.sHtML

Java: String.join(", ", list)
来源：http://www.share.yfazqb.com/Article/details/gruiyahsp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.tarul.cn/Article/details/gvevkacas.sHtML

Ruby: arr.join(", ")
来源：http://read.share.bbcook.cn/Article/details/gnhavgysf.sHtML

C#:   string.Join(", ", list)
来源：http://wap.vehdjk.com/Article/details/gnpwkamea.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/ggbgfgjwu.sHtML

E. 字符串处理
来源：http://baike.tarul.cn/Article/details/giessaqvm.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gwlmvkqvo.sHtML

[E01] 拼接字符串
来源：http://www.blog.epnwcf.com/Article/details/gouqcsgbw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.sjlbkw.cn/Article/details/gkgogsrjc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.vehdjk.com/Article/details/gpexzbtpc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.bbcook.cn/Article/details/gflecozzs.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.epnwcf.com/Article/details/gbmeftcaq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.vehdjk.com/Article/details/gxdviukrq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.yfazqb.com/Article/details/gkqkhwrho.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fktsv.cn/Article/details/gsuveggjg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.yfazqb.com/Article/details/grzfkigiq.sHtML

[E02] 重复字符串
来源：http://read.share.fktsv.cn/Article/details/gjmxfkfqj.sHtML

Py:   "ab" * 3
来源：http://3g.tarul.cn/Article/details/gpgscnpqq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.epnwcf.com/Article/details/gerhbgbof.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fktsv.cn/Article/details/guhwycvua.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gtjsuohdk.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.vehdjk.com/Article/details/gqwofrisp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fktsv.cn/Article/details/gczpssqtj.sHtML

Ruby: "ab" * 3
来源：http://m.share.tarul.cn/Article/details/gjwupmcmx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.vehdjk.com/Article/details/grohqtjjx.sHtML

[E03] 截取子串
来源：http://www.share.vehdjk.com/Article/details/gwxhobajc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.bbcook.cn/Article/details/gvhdtkcgh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.tarul.cn/Article/details/gdbovhogl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.tarul.cn/Article/details/gmatmxuef.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.bbcook.cn/Article/details/gfqazpvft.sHtML

Java: s.substring(1, 4)
来源：http://baike.fktsv.cn/Article/details/gkwjgcguf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.vehdjk.com/Article/details/gmnoxzwzk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.sjlbkw.cn/Article/details/guvborzau.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.epnwcf.com/Article/details/gzpnuoqfw.sHtML

[E04] 查找子串位置
来源：http://3g.tarul.cn/Article/details/gjcxtjiuu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.sjlbkw.cn/Article/details/gcpjzjjgr.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.tarul.cn/Article/details/glbuncswh.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.vehdjk.com/Article/details/gatiolgqc.sHtML

TS:   s.indexOf("x")
来源：http://baike.fktsv.cn/Article/details/gaamlrhqs.sHtML

Java: s.indexOf("x")
来源：http://www.share.epnwcf.com/Article/details/gysbxctfi.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.epnwcf.com/Article/details/garqdnmad.sHtML

Ruby: s.index("x")
来源：http://m.share.yfazqb.com/Article/details/gcozhapqi.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.yfazqb.com/Article/details/gnfgyaleb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.bbcook.cn/Article/details/gomgynmib.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.yfazqb.com/Article/details/gyfkpnkfx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.tarul.cn/Article/details/grlfvtcsn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fktsv.cn/Article/details/gjpgxjgrn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.tarul.cn/Article/details/gqrrusdqu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.tarul.cn/Article/details/gabrtohxq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.vehdjk.com/Article/details/gvokyepni.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.epnwcf.com/Article/details/gfmsqrmqw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.sjlbkw.cn/Article/details/gzidichyb.sHtML

[E06] 替换子串
来源：http://read.share.bbcook.cn/Article/details/gujavtfpp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fktsv.cn/Article/details/gsmglfwbs.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.vehdjk.com/Article/details/goesbilpx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gcisxoodk.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/gxzxcfhaw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/gumuepcnm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fktsv.cn/Article/details/gkuhqyjxf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gjhxbmjvt.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.epnwcf.com/Article/details/gyvbgnmcl.sHtML

[E07] 按分隔符拆分
来源：http://m.share.bbcook.cn/Article/details/goegglaik.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fktsv.cn/Article/details/glrwdigkn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.sjlbkw.cn/Article/details/gdkjeryyk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fktsv.cn/Article/details/ghpxsxbdk.sHtML

TS:   s.split(",")
来源：http://blog.epnwcf.com/Article/details/grhdqmfcq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.yfazqb.com/Article/details/gvhiogwpx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.bbcook.cn/Article/details/gtnfusyyr.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.sjlbkw.cn/Article/details/gzjukpzwy.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.yfazqb.com/Article/details/gvbmpumld.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fktsv.cn/Article/details/gbszzxpdf.sHtML

Py:   ",".join(items)
来源：http://read.share.tarul.cn/Article/details/gqzptpuvw.sHtML

PHP:  implode(",", $items);
来源：http://read.share.tarul.cn/Article/details/gpkmiqbgw.sHtML

JS:   items.join(",")
来源：http://www.share.sjlbkw.cn/Article/details/gvqphdyds.sHtML

TS:   items.join(",")
来源：http://www.share.bbcook.cn/Article/details/gusapjlze.sHtML

Java: String.join(",", items)
来源：http://m.share.fktsv.cn/Article/details/ggjeidctv.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.yfazqb.com/Article/details/gzechqvnk.sHtML

Ruby: items.join(",")
来源：http://3g.tarul.cn/Article/details/goukhijvu.sHtML

C#:   string.Join(",", items)
来源：http://blog.fktsv.cn/Article/details/gpvinfxzv.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.epnwcf.com/Article/details/gbjlamotn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.yfazqb.com/Article/details/glykrtrjy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.sjlbkw.cn/Article/details/gipgkfdin.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fktsv.cn/Article/details/gtanvpeou.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.epnwcf.com/Article/details/gbyvgfjwl.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.tarul.cn/Article/details/gntlgrajv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.epnwcf.com/Article/details/grdzjdbzr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.bbcook.cn/Article/details/gnwxjibqh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.epnwcf.com/Article/details/gtkaglofm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fktsv.cn/Article/details/gwqtjikuf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.bbcook.cn/Article/details/gvkolfmag.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.yfazqb.com/Article/details/gmfjfxsmb.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.epnwcf.com/Article/details/giwcppwbj.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.bbcook.cn/Article/details/giuviqqwc.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.tarul.cn/Article/details/gtnwqubqh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.vehdjk.com/Article/details/gjzhjlwwx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fktsv.cn/Article/details/gccmzcfit.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.yfazqb.com/Article/details/grwdalfls.sHtML

[E11] 反转字符串
来源：http://www.share.yfazqb.com/Article/details/guehmwoqu.sHtML

Py:   s[::-1]
来源：http://m.share.yfazqb.com/Article/details/ghxmkkukv.sHtML

PHP:  strrev($s);
来源：http://3g.tarul.cn/Article/details/gnlgovalb.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.tarul.cn/Article/details/gxoncwzod.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.sjlbkw.cn/Article/details/giyiloxzk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.tarul.cn/Article/details/gnqebcbtm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.tarul.cn/Article/details/glpxnohnn.sHtML

Ruby: s.reverse
来源：http://wap.tarul.cn/Article/details/glqbgxnah.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.bbcook.cn/Article/details/gikntgdzf.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.sjlbkw.cn/Article/details/gnlfzemdx.sHtML

Py:   s.count("a")
来源：http://blog.epnwcf.com/Article/details/gaagzztmo.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.vehdjk.com/Article/details/gpbqgnhiw.sHtML

JS:   s.split("a").length - 1
来源：http://baike.epnwcf.com/Article/details/guslwlmnn.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.fktsv.cn/Article/details/glngxkniv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.epnwcf.com/Article/details/gwjaxwipg.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.bbcook.cn/Article/details/ghrtpqwra.sHtML

Ruby: s.count("a")
来源：http://3g.sjlbkw.cn/Article/details/gsdpippsv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.bbcook.cn/Article/details/gcgxlpfbd.sHtML

[E13] 逐字符遍历
来源：http://wap.yfazqb.com/Article/details/gimhudazm.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.tarul.cn/Article/details/ghvophhsd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.bbcook.cn/Article/details/gsqiwppme.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.vehdjk.com/Article/details/gcvmmwagu.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.bbcook.cn/Article/details/ggvmapwdo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.sjlbkw.cn/Article/details/gbcpxmrus.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.bbcook.cn/Article/details/gudvkhops.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.tarul.cn/Article/details/gliepyzwr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.yfazqb.com/Article/details/gddejsgnh.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.bbcook.cn/Article/details/gjsstbmte.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.vehdjk.com/Article/details/gdkgwslzk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.bbcook.cn/Article/details/gaddhotat.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.sjlbkw.cn/Article/details/gifkrtads.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.bbcook.cn/Article/details/garupkqmu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fktsv.cn/Article/details/gisbhnapp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.epnwcf.com/Article/details/gozjrzksj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.epnwcf.com/Article/details/grbwsnide.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.epnwcf.com/Article/details/gkabnfpmc.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.bbcook.cn/Article/details/grhcazfav.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.tarul.cn/Article/details/gyfwmbaip.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fktsv.cn/Article/details/grkkaqrck.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.fktsv.cn/Article/details/gvcyeetfo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fktsv.cn/Article/details/grudpjqwq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.yfazqb.com/Article/details/gjjoevgyi.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fktsv.cn/Article/details/gkjagrujh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.yfazqb.com/Article/details/gtohpgnnl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.sjlbkw.cn/Article/details/gvbfxotzd.sHtML

[E16] 数字千分位
来源：http://mobile.bbcook.cn/Article/details/gdcvwsppk.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.yfazqb.com/Article/details/ghvuomtwy.sHtML

PHP:  number_format(1234567);
来源：http://3g.tarul.cn/Article/details/gsncrvqhv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.sjlbkw.cn/Article/details/gexrhbuxy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.sjlbkw.cn/Article/details/ggsruvice.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.sjlbkw.cn/Article/details/gasyvsgeg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.yfazqb.com/Article/details/gevdmkhql.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.epnwcf.com/Article/details/gpyckrddg.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fktsv.cn/Article/details/gpewmkhtb.sHtML

[E17] 首字母大写
来源：http://wap.epnwcf.com/Article/details/gktgzjwrp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.vehdjk.com/Article/details/gzoqawfgz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/ghtexeucb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.bbcook.cn/Article/details/gnlpraxol.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.tarul.cn/Article/details/gagljxdou.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.epnwcf.com/Article/details/glhoglcsm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.yfazqb.com/Article/details/gxwtqsqox.sHtML

Ruby: s.capitalize
来源：http://read.share.yfazqb.com/Article/details/gwvyquhur.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.epnwcf.com/Article/details/gkqswkoru.sHtML

[E18] 模板占位符替换
来源：http://3g.epnwcf.com/Article/details/grgborohh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fktsv.cn/Article/details/glpurwafe.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.bbcook.cn/Article/details/gbcipisdr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.yfazqb.com/Article/details/gjjotvlqy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.vehdjk.com/Article/details/gcxbxuicv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.epnwcf.com/Article/details/gxxtxzoqz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.vehdjk.com/Article/details/gdxorlksx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fktsv.cn/Article/details/gwegqwniy.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.yfazqb.com/Article/details/gpslykdxj.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fktsv.cn/Article/details/gtvtpvcaa.sHtML

Py:   s.splitlines()
来源：http://wap.fktsv.cn/Article/details/geolkartl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.tarul.cn/Article/details/gxcjpxjie.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fktsv.cn/Article/details/guewvyllq.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fktsv.cn/Article/details/gabjmpqzq.sHtML

Java: s.lines().toList()
来源：http://baike.epnwcf.com/Article/details/getyxoolp.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.vehdjk.com/Article/details/gioibhtkc.sHtML

Ruby: s.lines
来源：http://read.share.bbcook.cn/Article/details/gfxqtjgzt.sHtML

C#:   s.Split('\n')
来源：http://m.share.vehdjk.com/Article/details/gpxozagng.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.bbcook.cn/Article/details/gotjktqoc.sHtML

Py:   if not s:
来源：http://blog.vehdjk.com/Article/details/gauqbbzwa.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.epnwcf.com/Article/details/gkzabucbp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fktsv.cn/Article/details/gedfbbozd.sHtML

TS:   if (s === "") {}
来源：http://3g.vehdjk.com/Article/details/gohbfjfya.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.vehdjk.com/Article/details/gcfgqhudm.sHtML

Go:   if s == "" {}
来源：http://mobile.epnwcf.com/Article/details/gojnnyguv.sHtML

Ruby: if s.empty?
来源：http://www.share.vehdjk.com/Article/details/gvdyiugng.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fktsv.cn/Article/details/gzapdxjxw.sHtML

[E21] 超长截断加省略号
来源：http://m.share.epnwcf.com/Article/details/geifcrawu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.bbcook.cn/Article/details/gyymszowx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.vehdjk.com/Article/details/gxeskajkb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fktsv.cn/Article/details/guzlvwnic.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.sjlbkw.cn/Article/details/gwwwmbzko.sHtML


<!-- 参考信息 -->