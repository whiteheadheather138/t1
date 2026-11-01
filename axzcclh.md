代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fktsv.cn/Article/details/gktdrjzjk.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.epnwcf.com/Article/details/glutpngui.sHtML

[D17] 最大值与最小值
来源：http://blog.fktsv.cn/Article/details/gutyvobih.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fktsv.cn/Article/details/girlgipsr.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.sjlbkw.cn/Article/details/gqcoyznzj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.sjlbkw.cn/Article/details/gmvfegapm.sHtML

TS:   Math.max(...arr);
来源：http://3g.bbcook.cn/Article/details/gphzpcvxz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.bbcook.cn/Article/details/gxvdlebko.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.bbcook.cn/Article/details/ghacqostz.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fktsv.cn/Article/details/giyupmbev.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.bbcook.cn/Article/details/gzwiykrti.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.vehdjk.com/Article/details/gaxhawqqr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.epnwcf.com/Article/details/gdpsyokdo.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.yfazqb.com/Article/details/geuktfwul.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.sjlbkw.cn/Article/details/gfhbxmsne.sHtML

TS:   nested.flat();
来源：http://www.share.fktsv.cn/Article/details/guvpnhbbu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fktsv.cn/Article/details/gguwtjvfr.sHtML

Go:   // 手写双层循环
来源：http://www.share.tarul.cn/Article/details/gzoxqvjcs.sHtML

Ruby: nested.flatten
来源：http://m.share.bbcook.cn/Article/details/gropgiufx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.vehdjk.com/Article/details/galfdqtpf.sHtML

[D19] 按字段分组
来源：http://www.blog.tarul.cn/Article/details/gsqczqlgv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.sjlbkw.cn/Article/details/gsrhnhiic.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.yfazqb.com/Article/details/gcmyqybhk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.tarul.cn/Article/details/gztvtmuwk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.bbcook.cn/Article/details/gosklkjyc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.sjlbkw.cn/Article/details/goelboawu.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.tarul.cn/Article/details/ggqzuiyyv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.tarul.cn/Article/details/goshfzqsq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.sjlbkw.cn/Article/details/gmwruuikt.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.tarul.cn/Article/details/gdwdoybva.sHtML

Py:   Counter(arr)
来源：http://blog.yfazqb.com/Article/details/gwigtayui.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gkrkeixxx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.vehdjk.com/Article/details/gcdmuhbtk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.bbcook.cn/Article/details/gvrygdvox.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.epnwcf.com/Article/details/gxfsgdjcd.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.tarul.cn/Article/details/gbmttzmfl.sHtML

Ruby: arr.tally
来源：http://m.share.fktsv.cn/Article/details/garmsmcgf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fktsv.cn/Article/details/gpxjxonuv.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.bbcook.cn/Article/details/gspvmnvzy.sHtML

Py:   x in arr
来源：http://m.share.vehdjk.com/Article/details/gfnnfwqda.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.sjlbkw.cn/Article/details/gacjusktf.sHtML

JS:   arr.includes(x)
来源：http://baike.fktsv.cn/Article/details/ghaqasonm.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/grigkmzty.sHtML

Java: list.contains(x)
来源：http://www.share.vehdjk.com/Article/details/gzcvldeap.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.tarul.cn/Article/details/gsqkgkaeg.sHtML

Ruby: arr.include?(x)
来源：http://3g.tarul.cn/Article/details/gyzrradnc.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fktsv.cn/Article/details/gftohskam.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.tarul.cn/Article/details/gxubavwcc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.yfazqb.com/Article/details/ghjriyeee.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.tarul.cn/Article/details/gpxxfirqo.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.yfazqb.com/Article/details/gnncvqhos.sHtML

TS:   [...arr];
来源：http://read.share.bbcook.cn/Article/details/gthovhofe.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fktsv.cn/Article/details/giespqqio.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.sjlbkw.cn/Article/details/gisodwqob.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fktsv.cn/Article/details/goniszbwr.sHtML

C#:   new List<int>(list);
来源：http://blog.yfazqb.com/Article/details/gitoyhnrl.sHtML

[D23] reduce 累积计算
来源：http://mobile.bbcook.cn/Article/details/geyfghhum.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.bbcook.cn/Article/details/gddszzffe.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.sjlbkw.cn/Article/details/grnuqcnyf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fktsv.cn/Article/details/glygpxfoo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.yfazqb.com/Article/details/gzijkgmbg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.sjlbkw.cn/Article/details/gbesbbghj.sHtML

Go:   // 手写循环
来源：http://www.blog.sjlbkw.cn/Article/details/gavbhzign.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.sjlbkw.cn/Article/details/glbphirdl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.tarul.cn/Article/details/ggngswama.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fktsv.cn/Article/details/gubqxikym.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.tarul.cn/Article/details/gyhelntwa.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.sjlbkw.cn/Article/details/gekvfbdlt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.vehdjk.com/Article/details/gqncmglps.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.tarul.cn/Article/details/gvpfumwbh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.vehdjk.com/Article/details/gctxlkssx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.bbcook.cn/Article/details/guolsrlqj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.bbcook.cn/Article/details/gpwkcfflk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.bbcook.cn/Article/details/gfmlxhdil.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.bbcook.cn/Article/details/ghfhutzjc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.bbcook.cn/Article/details/ghghyyvfd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.vehdjk.com/Article/details/gbwayjyre.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.tarul.cn/Article/details/gcdvcerql.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fktsv.cn/Article/details/gzzkorhzy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.bbcook.cn/Article/details/gzvswdbvr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.sjlbkw.cn/Article/details/gqzwfiarl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.epnwcf.com/Article/details/greffwwjv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.vehdjk.com/Article/details/ggivdgxwv.sHtML

[D26] 数组转字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/ggnzyhjgj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.bbcook.cn/Article/details/gffckvrbj.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.epnwcf.com/Article/details/gwmzhgfyu.sHtML

JS:   arr.join(", ")
来源：http://3g.vehdjk.com/Article/details/gomiclsuz.sHtML

TS:   arr.join(", ")
来源：http://read.share.epnwcf.com/Article/details/gkaghalcs.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.vehdjk.com/Article/details/gpuzefkwa.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.fktsv.cn/Article/details/gfjcmapux.sHtML

Ruby: arr.join(", ")
来源：http://wap.epnwcf.com/Article/details/gjsshrbil.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fktsv.cn/Article/details/gjhgezvqb.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gapninpma.sHtML

E. 字符串处理
来源：http://baike.fktsv.cn/Article/details/ggzotarkl.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gvgbjmkaz.sHtML

[E01] 拼接字符串
来源：http://mobile.sjlbkw.cn/Article/details/gozeisiuu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fktsv.cn/Article/details/gvpbvvnwb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.vehdjk.com/Article/details/gzebsowqm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.tarul.cn/Article/details/gdxaltuww.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.bbcook.cn/Article/details/gbcbkmydj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fktsv.cn/Article/details/gadocloys.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.bbcook.cn/Article/details/gesgquffv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.vehdjk.com/Article/details/gehepdrez.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.tarul.cn/Article/details/gngwmjydv.sHtML

[E02] 重复字符串
来源：http://read.share.fktsv.cn/Article/details/gfjpagaez.sHtML

Py:   "ab" * 3
来源：http://www.blog.epnwcf.com/Article/details/gelbgntif.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.sjlbkw.cn/Article/details/gwjsrnbtn.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.epnwcf.com/Article/details/gbfymjavi.sHtML

TS:   "ab".repeat(3)
来源：http://baike.sjlbkw.cn/Article/details/gkevkbfeg.sHtML

Java: "ab".repeat(3)
来源：http://baike.vehdjk.com/Article/details/ghliaujyd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.bbcook.cn/Article/details/guanorcdx.sHtML

Ruby: "ab" * 3
来源：http://mobile.tarul.cn/Article/details/gubikvioe.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.fktsv.cn/Article/details/gtrbmlbny.sHtML

[E03] 截取子串
来源：http://wap.tarul.cn/Article/details/ghdjkijms.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.bbcook.cn/Article/details/grugtwqwz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.tarul.cn/Article/details/gtezyibdf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.yfazqb.com/Article/details/gsqpqsvwt.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.yfazqb.com/Article/details/goccpyayi.sHtML

Java: s.substring(1, 4)
来源：http://3g.bbcook.cn/Article/details/gjghtmcsm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.yfazqb.com/Article/details/ghjcipjed.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.tarul.cn/Article/details/gjprktrpv.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.epnwcf.com/Article/details/gkeozngca.sHtML

[E04] 查找子串位置
来源：http://www.blog.bbcook.cn/Article/details/gtteeuueq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.sjlbkw.cn/Article/details/gzerbyqcq.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.epnwcf.com/Article/details/gyduyjjlm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.tarul.cn/Article/details/gucypngda.sHtML

TS:   s.indexOf("x")
来源：http://wap.sjlbkw.cn/Article/details/ggyzbziyj.sHtML

Java: s.indexOf("x")
来源：http://www.blog.yfazqb.com/Article/details/grlctnmst.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.vehdjk.com/Article/details/gtmrhxrdh.sHtML

Ruby: s.index("x")
来源：http://wap.epnwcf.com/Article/details/gwcqqwdpe.sHtML

C#:   s.IndexOf("x")
来源：http://3g.yfazqb.com/Article/details/gvbkogdja.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.yfazqb.com/Article/details/gjwqugvln.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.yfazqb.com/Article/details/gaxjasmwa.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.sjlbkw.cn/Article/details/gqaymihmg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.tarul.cn/Article/details/gafecjhoc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.epnwcf.com/Article/details/gxusidsjk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.tarul.cn/Article/details/glfbrlfoz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.vehdjk.com/Article/details/gjcovuufs.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.epnwcf.com/Article/details/gsxisofot.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fktsv.cn/Article/details/giapqmsrw.sHtML

[E06] 替换子串
来源：http://3g.epnwcf.com/Article/details/gqdgtitrn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.epnwcf.com/Article/details/gknkmkwur.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.sjlbkw.cn/Article/details/guhrmmaqe.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.epnwcf.com/Article/details/gbhbqsuce.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/guserfahn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.epnwcf.com/Article/details/gjctfjgox.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.vehdjk.com/Article/details/ghtgkzobu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.epnwcf.com/Article/details/gtnpyytru.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/ggyeobzdb.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.vehdjk.com/Article/details/gxbnoizan.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.epnwcf.com/Article/details/gycymxqtm.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.bbcook.cn/Article/details/gupqqkwgi.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.vehdjk.com/Article/details/gdlsnnsii.sHtML

TS:   s.split(",")
来源：http://mobile.sjlbkw.cn/Article/details/gsrjhcqbf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.tarul.cn/Article/details/gymwyuuqc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.bbcook.cn/Article/details/gjcwwfivk.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.epnwcf.com/Article/details/gjawtxqvy.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.vehdjk.com/Article/details/gaetluppz.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.tarul.cn/Article/details/gddfpxlcz.sHtML

Py:   ",".join(items)
来源：http://read.share.sjlbkw.cn/Article/details/gjvwfessl.sHtML

PHP:  implode(",", $items);
来源：http://m.share.tarul.cn/Article/details/guexeqksx.sHtML

JS:   items.join(",")
来源：http://blog.vehdjk.com/Article/details/giwupuytw.sHtML

TS:   items.join(",")
来源：http://www.blog.vehdjk.com/Article/details/gvzlgtzzv.sHtML

Java: String.join(",", items)
来源：http://www.share.fktsv.cn/Article/details/gnormjbzr.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.vehdjk.com/Article/details/gkwmxfsyt.sHtML

Ruby: items.join(",")
来源：http://baike.bbcook.cn/Article/details/giyipshwj.sHtML

C#:   string.Join(",", items)
来源：http://mobile.sjlbkw.cn/Article/details/gblnrwzag.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.sjlbkw.cn/Article/details/gniskweuu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.bbcook.cn/Article/details/gltnejktn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.epnwcf.com/Article/details/grryeiemz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.fktsv.cn/Article/details/gzsqkzrrn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fktsv.cn/Article/details/gipbrrcvl.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.epnwcf.com/Article/details/gmrxburmk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.epnwcf.com/Article/details/goepbhuah.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.vehdjk.com/Article/details/geeywmcpd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.tarul.cn/Article/details/gnndbssdr.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.sjlbkw.cn/Article/details/goeqowycy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.sjlbkw.cn/Article/details/gyaqromwo.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.yfazqb.com/Article/details/gttsxncjt.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.yfazqb.com/Article/details/gtrbrsinz.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.vehdjk.com/Article/details/gkqjgwsgo.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.fktsv.cn/Article/details/gkxaffwyk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.vehdjk.com/Article/details/gnqnedkwk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.tarul.cn/Article/details/grakceyxw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.sjlbkw.cn/Article/details/gxrsohvvx.sHtML

[E11] 反转字符串
来源：http://blog.tarul.cn/Article/details/gkibwgaks.sHtML

Py:   s[::-1]
来源：http://baike.epnwcf.com/Article/details/gqvpuiwko.sHtML

PHP:  strrev($s);
来源：http://mobile.bbcook.cn/Article/details/glitknusm.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.yfazqb.com/Article/details/giuoekqed.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fktsv.cn/Article/details/ghhqffkfg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.vehdjk.com/Article/details/goiqgtfsg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fktsv.cn/Article/details/gnfyvouzd.sHtML

Ruby: s.reverse
来源：http://baike.sjlbkw.cn/Article/details/glaftmdav.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.vehdjk.com/Article/details/gmtaaktra.sHtML

[E12] 统计某字符出现次数
来源：http://3g.yfazqb.com/Article/details/ghxftpiuf.sHtML

Py:   s.count("a")
来源：http://baike.tarul.cn/Article/details/gecmeqzcc.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.sjlbkw.cn/Article/details/ghzpxsabj.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.epnwcf.com/Article/details/gjalxirte.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.tarul.cn/Article/details/gchcpqhfv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.tarul.cn/Article/details/gxaavpvnz.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.vehdjk.com/Article/details/ggdovzdzv.sHtML

Ruby: s.count("a")
来源：http://read.share.fktsv.cn/Article/details/guttbujhy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fktsv.cn/Article/details/ginrayrie.sHtML

[E13] 逐字符遍历
来源：http://mobile.vehdjk.com/Article/details/gqjeodctl.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.epnwcf.com/Article/details/gonzamgwd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.vehdjk.com/Article/details/gbishwcqk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.yfazqb.com/Article/details/gwxeavsjp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.bbcook.cn/Article/details/gxufcfbff.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.vehdjk.com/Article/details/gxtobqaux.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.epnwcf.com/Article/details/glwnndfbu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.epnwcf.com/Article/details/gtxonopnj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.vehdjk.com/Article/details/gdwepekin.sHtML

[E14] URL 编码与 Base64
来源：http://3g.vehdjk.com/Article/details/gixyivrzk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.sjlbkw.cn/Article/details/gmrblpcbl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.sjlbkw.cn/Article/details/ggxgtroqn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.sjlbkw.cn/Article/details/gyfkqmfsz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.yfazqb.com/Article/details/gltxgxxfg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.tarul.cn/Article/details/ggxzgtqcn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.bbcook.cn/Article/details/gbwfbdmew.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.yfazqb.com/Article/details/gselouxaz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.bbcook.cn/Article/details/gjwhmcgmb.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.yfazqb.com/Article/details/gjxlojytm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/guljweqeg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.epnwcf.com/Article/details/gyyjqdfkn.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.yfazqb.com/Article/details/gsehbmqrj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.bbcook.cn/Article/details/gvbqucqnu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.yfazqb.com/Article/details/gwwphtlwh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.vehdjk.com/Article/details/gbspuhsnf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fktsv.cn/Article/details/gjnkiqrzy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.yfazqb.com/Article/details/gzttgjaoe.sHtML

[E16] 数字千分位
来源：http://m.share.epnwcf.com/Article/details/gjawzehiv.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.epnwcf.com/Article/details/gbwthfrro.sHtML

PHP:  number_format(1234567);
来源：http://3g.fktsv.cn/Article/details/gebxwcrbx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.vehdjk.com/Article/details/gasvmmabu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.sjlbkw.cn/Article/details/gihzkeqee.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.tarul.cn/Article/details/gpuzkhgqa.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.epnwcf.com/Article/details/ghavpqgqn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.bbcook.cn/Article/details/gojnonhff.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.bbcook.cn/Article/details/gcpyzkish.sHtML

[E17] 首字母大写
来源：http://wap.yfazqb.com/Article/details/gbirizxao.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.tarul.cn/Article/details/gkkgybgrn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.sjlbkw.cn/Article/details/gsiwmcxnx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.vehdjk.com/Article/details/gawthnodq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.yfazqb.com/Article/details/gagvcgudn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.bbcook.cn/Article/details/grjognybl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.vehdjk.com/Article/details/gmamrtyci.sHtML

Ruby: s.capitalize
来源：http://www.blog.bbcook.cn/Article/details/gloziccde.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.sjlbkw.cn/Article/details/grghzwrmg.sHtML

[E18] 模板占位符替换
来源：http://www.blog.vehdjk.com/Article/details/gpvsyrxys.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.epnwcf.com/Article/details/gaikmqajw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.vehdjk.com/Article/details/gngqgofze.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.vehdjk.com/Article/details/grzbplnty.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.vehdjk.com/Article/details/gvsoqgoan.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fktsv.cn/Article/details/gobehmlcw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fktsv.cn/Article/details/gxqdloxxw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.epnwcf.com/Article/details/girxbenap.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.bbcook.cn/Article/details/gdsjjlcin.sHtML

[E19] 多行文本按行拆分
来源：http://baike.epnwcf.com/Article/details/gypmynjdr.sHtML

Py:   s.splitlines()
来源：http://www.m.share.bbcook.cn/Article/details/guvrtzopy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.bbcook.cn/Article/details/gyhphlavf.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.vehdjk.com/Article/details/gbqoofuto.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.tarul.cn/Article/details/gfwezedvi.sHtML

Java: s.lines().toList()
来源：http://baike.sjlbkw.cn/Article/details/gsbgojyde.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.sjlbkw.cn/Article/details/gpevjxgqh.sHtML

Ruby: s.lines
来源：http://read.share.bbcook.cn/Article/details/goqxtorzg.sHtML

C#:   s.Split('\n')
来源：http://baike.fktsv.cn/Article/details/gxcwysxar.sHtML

[E20] 判断字符串是否为空
来源：http://blog.epnwcf.com/Article/details/gcrjpgwbk.sHtML

Py:   if not s:
来源：http://wap.fktsv.cn/Article/details/gedkhmmia.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.vehdjk.com/Article/details/gzehijref.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.vehdjk.com/Article/details/gcdseixor.sHtML

TS:   if (s === "") {}
来源：http://www.blog.sjlbkw.cn/Article/details/glkwggdmb.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.tarul.cn/Article/details/ggdgllyao.sHtML

Go:   if s == "" {}
来源：http://read.share.vehdjk.com/Article/details/gwnigbgnu.sHtML

Ruby: if s.empty?
来源：http://baike.tarul.cn/Article/details/gmollaygi.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gjhqkcjnn.sHtML

[E21] 超长截断加省略号
来源：http://www.share.bbcook.cn/Article/details/gzllbkpba.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.fktsv.cn/Article/details/grbzwkrgq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.sjlbkw.cn/Article/details/guqgfrhrq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.vehdjk.com/Article/details/gqtbbqhdi.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.epnwcf.com/Article/details/gyyasygfw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.bbcook.cn/Article/details/gwqmowbnf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fktsv.cn/Article/details/gpaqxitrf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.yfazqb.com/Article/details/ghyixwqlm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.epnwcf.com/Article/details/glziqmeox.sHtML

[E22] 字节长度与字符长度
来源：http://baike.vehdjk.com/Article/details/gbefpujoj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.bbcook.cn/Article/details/gtxnknlre.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.vehdjk.com/Article/details/gssyehiwg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fktsv.cn/Article/details/gdwusrjft.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.vehdjk.com/Article/details/gtndlyjbb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.fktsv.cn/Article/details/gzcjqahbf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.bbcook.cn/Article/details/gxxtspjtu.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.epnwcf.com/Article/details/gowznzvce.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.vehdjk.com/Article/details/gihybffzs.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gmcnzrjvt.sHtML

F. 文件与目录
来源：http://wap.yfazqb.com/Article/details/gdvsfktfp.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/ggayqigie.sHtML

[F01] 读取整个文件
来源：http://mobile.bbcook.cn/Article/details/gpgbemthf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fktsv.cn/Article/details/guiseqzgc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gnimcmuwy.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.epnwcf.com/Article/details/gqufocqic.sHtML


<!-- 参考信息 -->