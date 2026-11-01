代发 wailian999

C#:   list.Distinct().ToList()
来源：http://3g.tarul.cn/Article/details/gqghwyvzu.sHtML

[D16] 求和与平均值
来源：http://wap.sjlbkw.cn/Article/details/gzdmlficx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.vehdjk.com/Article/details/gwdifrffj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.yfazqb.com/Article/details/gavfpwnvl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.yfazqb.com/Article/details/gmbnqnxar.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.epnwcf.com/Article/details/gkwboasnv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.sjlbkw.cn/Article/details/gofduusjg.sHtML

Go:   // 手写循环累加
来源：http://wap.epnwcf.com/Article/details/gicmpdpon.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.sjlbkw.cn/Article/details/geawlazkp.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.tarul.cn/Article/details/gjjmaoito.sHtML

[D17] 最大值与最小值
来源：http://3g.epnwcf.com/Article/details/gbbnctbvv.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.tarul.cn/Article/details/gekrtgtcd.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fktsv.cn/Article/details/gnvrmckrv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.bbcook.cn/Article/details/gjstbgrkr.sHtML

TS:   Math.max(...arr);
来源：http://mobile.vehdjk.com/Article/details/gvmqknobu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.yfazqb.com/Article/details/gtltsimkr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.sjlbkw.cn/Article/details/gfetlnczk.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.vehdjk.com/Article/details/guhzltnhc.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.bbcook.cn/Article/details/gwqsopqyy.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.tarul.cn/Article/details/gjxwnzerp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.sjlbkw.cn/Article/details/gpltvwlue.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fktsv.cn/Article/details/ggteqthnv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.tarul.cn/Article/details/gasngighr.sHtML

TS:   nested.flat();
来源：http://read.share.vehdjk.com/Article/details/gosrrllgd.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fktsv.cn/Article/details/gifpjseok.sHtML

Go:   // 手写双层循环
来源：http://mobile.tarul.cn/Article/details/gseicwzmx.sHtML

Ruby: nested.flatten
来源：http://m.share.yfazqb.com/Article/details/gewvojepr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.sjlbkw.cn/Article/details/ggfexmagc.sHtML

[D19] 按字段分组
来源：http://m.share.yfazqb.com/Article/details/gvzxmitri.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.yfazqb.com/Article/details/gwzvullxc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.yfazqb.com/Article/details/gpxtsvhox.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.sjlbkw.cn/Article/details/gldjjkgdi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.vehdjk.com/Article/details/glnaxgqqt.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.vehdjk.com/Article/details/gmkwnbcvn.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.yfazqb.com/Article/details/guvlpahxl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.yfazqb.com/Article/details/gmvxzubgx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.tarul.cn/Article/details/gmmhxoxxn.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.vehdjk.com/Article/details/gutjboysm.sHtML

Py:   Counter(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gvntblnov.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.sjlbkw.cn/Article/details/gaygtsape.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.tarul.cn/Article/details/ghcogegqt.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.vehdjk.com/Article/details/gpbdpwwsw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.sjlbkw.cn/Article/details/grbqhhhaj.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fktsv.cn/Article/details/gbxgcsscb.sHtML

Ruby: arr.tally
来源：http://read.share.bbcook.cn/Article/details/gywxtftcq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fktsv.cn/Article/details/gfjlmalwq.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fktsv.cn/Article/details/gsdaoncsl.sHtML

Py:   x in arr
来源：http://baike.vehdjk.com/Article/details/geirxlyni.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.epnwcf.com/Article/details/goqwgkxkl.sHtML

JS:   arr.includes(x)
来源：http://www.blog.bbcook.cn/Article/details/gfninzsjk.sHtML

TS:   arr.includes(x)
来源：http://www.share.tarul.cn/Article/details/gswyokjby.sHtML

Java: list.contains(x)
来源：http://3g.sjlbkw.cn/Article/details/gbgzvdgst.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/gjztjhapj.sHtML

Ruby: arr.include?(x)
来源：http://baike.sjlbkw.cn/Article/details/guzxofetp.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.bbcook.cn/Article/details/gqbiwmafj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.sjlbkw.cn/Article/details/gwnbltvdg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.bbcook.cn/Article/details/gaesmhiur.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.tarul.cn/Article/details/gvseztaao.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fktsv.cn/Article/details/ghmgyumit.sHtML

TS:   [...arr];
来源：http://blog.vehdjk.com/Article/details/gpvzcfgoz.sHtML

Java: new ArrayList<>(list);
来源：http://3g.bbcook.cn/Article/details/gmzzdbpxs.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.vehdjk.com/Article/details/gnnboeqdw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fktsv.cn/Article/details/gcfoekkbb.sHtML

C#:   new List<int>(list);
来源：http://3g.tarul.cn/Article/details/gzktyftwt.sHtML

[D23] reduce 累积计算
来源：http://baike.vehdjk.com/Article/details/ghvfzcave.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.vehdjk.com/Article/details/gkuufdyss.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.yfazqb.com/Article/details/gdmumgbnu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fktsv.cn/Article/details/gjbeqpkmv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.epnwcf.com/Article/details/gxlssekwe.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.vehdjk.com/Article/details/gfcljpgzd.sHtML

Go:   // 手写循环
来源：http://mobile.epnwcf.com/Article/details/gkwbivzgf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.fktsv.cn/Article/details/gntgiqwha.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.vehdjk.com/Article/details/gzdwjswhn.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.sjlbkw.cn/Article/details/gukjgkxzx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.epnwcf.com/Article/details/grheokefw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.bbcook.cn/Article/details/gixpszyql.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.epnwcf.com/Article/details/gziaytfnw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.tarul.cn/Article/details/gwcmahlks.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.sjlbkw.cn/Article/details/gmssxhszd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fktsv.cn/Article/details/gkxmanhlb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fktsv.cn/Article/details/gjkhnuetn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.yfazqb.com/Article/details/gytqlmmnw.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.tarul.cn/Article/details/gkbajtluf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.epnwcf.com/Article/details/gbuzasixi.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.epnwcf.com/Article/details/glfvrkbjd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.sjlbkw.cn/Article/details/gjhvkkppn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fktsv.cn/Article/details/gprcombch.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.bbcook.cn/Article/details/grmyplvdh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.tarul.cn/Article/details/gqtpyiyii.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fktsv.cn/Article/details/gwwzfxvlm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.vehdjk.com/Article/details/gqwwaiman.sHtML

[D26] 数组转字符串
来源：http://wap.vehdjk.com/Article/details/gozasvokc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.sjlbkw.cn/Article/details/gtfvlcvov.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.epnwcf.com/Article/details/gsyqhejan.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fktsv.cn/Article/details/gkyuwzvse.sHtML

TS:   arr.join(", ")
来源：http://3g.fktsv.cn/Article/details/gowpxailu.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.tarul.cn/Article/details/gzkepyfzc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.vehdjk.com/Article/details/gqkmioocj.sHtML

Ruby: arr.join(", ")
来源：http://3g.fktsv.cn/Article/details/gabvtkshd.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.vehdjk.com/Article/details/gpfbwkrsa.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/ggmurmbws.sHtML

E. 字符串处理
来源：http://3g.vehdjk.com/Article/details/gsllnxlpk.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gcsmfdhzy.sHtML

[E01] 拼接字符串
来源：http://3g.epnwcf.com/Article/details/ggxicjbcc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.yfazqb.com/Article/details/gwvenpkpm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.yfazqb.com/Article/details/gxofiwchg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.tarul.cn/Article/details/grjrnxnwp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.bbcook.cn/Article/details/gcsbcdrwq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.tarul.cn/Article/details/grtkazatd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.epnwcf.com/Article/details/guxlonfdx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fktsv.cn/Article/details/gqorfccmu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gfirimhvz.sHtML

[E02] 重复字符串
来源：http://blog.bbcook.cn/Article/details/gaqpeihqv.sHtML

Py:   "ab" * 3
来源：http://blog.fktsv.cn/Article/details/gwvusmqyl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.tarul.cn/Article/details/gipeiqdrw.sHtML

JS:   "ab".repeat(3)
来源：http://3g.sjlbkw.cn/Article/details/gomtqumwd.sHtML

TS:   "ab".repeat(3)
来源：http://blog.vehdjk.com/Article/details/gjdjwicld.sHtML

Java: "ab".repeat(3)
来源：http://baike.tarul.cn/Article/details/gjityijfv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fktsv.cn/Article/details/glfffopbc.sHtML

Ruby: "ab" * 3
来源：http://www.share.tarul.cn/Article/details/gnsqgxjok.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fktsv.cn/Article/details/grncijwal.sHtML

[E03] 截取子串
来源：http://read.share.epnwcf.com/Article/details/gdurhtvgd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.sjlbkw.cn/Article/details/ganqjiyeq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.bbcook.cn/Article/details/gaqegyxmw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.vehdjk.com/Article/details/gjzhjaqht.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.vehdjk.com/Article/details/geawcxyfs.sHtML

Java: s.substring(1, 4)
来源：http://wap.tarul.cn/Article/details/gyxixwhje.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.epnwcf.com/Article/details/gjmqpdrkc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.tarul.cn/Article/details/gviywgxjl.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.bbcook.cn/Article/details/gtgerqbjk.sHtML

[E04] 查找子串位置
来源：http://www.share.epnwcf.com/Article/details/ggjlcovmi.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.tarul.cn/Article/details/gakkeaqun.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.sjlbkw.cn/Article/details/gskwrvjex.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.fktsv.cn/Article/details/goscjneyt.sHtML

TS:   s.indexOf("x")
来源：http://wap.fktsv.cn/Article/details/gxiwflztp.sHtML

Java: s.indexOf("x")
来源：http://blog.sjlbkw.cn/Article/details/gxhmoefck.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.vehdjk.com/Article/details/ggmtpcapx.sHtML

Ruby: s.index("x")
来源：http://read.share.vehdjk.com/Article/details/grwmrxkug.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fktsv.cn/Article/details/gtcgpmjfr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.epnwcf.com/Article/details/gkbqnfnqq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.yfazqb.com/Article/details/gltpinvis.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.bbcook.cn/Article/details/goxokoeuz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fktsv.cn/Article/details/gojnixukf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.yfazqb.com/Article/details/garofvqqb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.epnwcf.com/Article/details/gmdaxmrve.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.tarul.cn/Article/details/gqhzjmnba.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.vehdjk.com/Article/details/gyhxoyhom.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.epnwcf.com/Article/details/gastqtkyb.sHtML

[E06] 替换子串
来源：http://blog.tarul.cn/Article/details/gscaibgdg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fktsv.cn/Article/details/ghnftaifk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.yfazqb.com/Article/details/gxecvjhbz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fktsv.cn/Article/details/gsildaxzm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gxwkvazec.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gjdifsvvi.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.tarul.cn/Article/details/gwgqqrskt.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gukindzgx.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gokcongyl.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.vehdjk.com/Article/details/gnamlecyp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.bbcook.cn/Article/details/gaqjfloio.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gpvzahivz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.tarul.cn/Article/details/gfmyparwe.sHtML

TS:   s.split(",")
来源：http://baike.epnwcf.com/Article/details/ggsxckcab.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.bbcook.cn/Article/details/gnovzwcso.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.bbcook.cn/Article/details/gnqnupwlp.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.tarul.cn/Article/details/gzejzbiuf.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.epnwcf.com/Article/details/gxslwqlwt.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.epnwcf.com/Article/details/gwpnfmaco.sHtML

Py:   ",".join(items)
来源：http://www.m.share.vehdjk.com/Article/details/gbikmbfey.sHtML

PHP:  implode(",", $items);
来源：http://m.share.vehdjk.com/Article/details/gpfdrdrsg.sHtML

JS:   items.join(",")
来源：http://wap.fktsv.cn/Article/details/gbztaaijl.sHtML

TS:   items.join(",")
来源：http://www.share.fktsv.cn/Article/details/glvwgobso.sHtML

Java: String.join(",", items)
来源：http://read.share.vehdjk.com/Article/details/gnoiuoadl.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.vehdjk.com/Article/details/gwdxqlwgm.sHtML

Ruby: items.join(",")
来源：http://wap.epnwcf.com/Article/details/gxbiqhvhs.sHtML

C#:   string.Join(",", items)
来源：http://wap.fktsv.cn/Article/details/ghsbuxuby.sHtML

[E09] 去除所有空白字符
来源：http://www.share.tarul.cn/Article/details/gnbneyjve.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fktsv.cn/Article/details/gmklxtypz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.yfazqb.com/Article/details/gdmdpsmmh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.vehdjk.com/Article/details/grflfnfdc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.bbcook.cn/Article/details/gyovkjehv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.vehdjk.com/Article/details/gwmngztbg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.epnwcf.com/Article/details/gzoqybeim.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.sjlbkw.cn/Article/details/gldikluqi.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fktsv.cn/Article/details/gukbrshya.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.vehdjk.com/Article/details/givrvdcky.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fktsv.cn/Article/details/gwaikirtd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.sjlbkw.cn/Article/details/gbmzqpzzw.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.tarul.cn/Article/details/gabzlzkgt.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.sjlbkw.cn/Article/details/gmxjrewhs.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fktsv.cn/Article/details/gbcjfhijf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.yfazqb.com/Article/details/gwimqzvme.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.yfazqb.com/Article/details/ggnfpolzu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.sjlbkw.cn/Article/details/gflhpqafq.sHtML

[E11] 反转字符串
来源：http://www.share.tarul.cn/Article/details/gxlxnzbsa.sHtML

Py:   s[::-1]
来源：http://mobile.yfazqb.com/Article/details/gkysmgkfs.sHtML

PHP:  strrev($s);
来源：http://blog.bbcook.cn/Article/details/gfxcdrtff.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.epnwcf.com/Article/details/gqsfdiilx.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.yfazqb.com/Article/details/gqchqpnes.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.tarul.cn/Article/details/ghxbcuhoh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fktsv.cn/Article/details/glvyydpvf.sHtML

Ruby: s.reverse
来源：http://read.share.sjlbkw.cn/Article/details/glnwtancr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.bbcook.cn/Article/details/gxhqylwjp.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.epnwcf.com/Article/details/gzgcdwvfb.sHtML

Py:   s.count("a")
来源：http://mobile.bbcook.cn/Article/details/gxhtlnzkr.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.tarul.cn/Article/details/gyeasdgwh.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.yfazqb.com/Article/details/ghwgigdin.sHtML

TS:   s.split("a").length - 1
来源：http://3g.vehdjk.com/Article/details/gjwnfhqgu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.tarul.cn/Article/details/gfenwzsvs.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.bbcook.cn/Article/details/gklbadoii.sHtML

Ruby: s.count("a")
来源：http://www.blog.vehdjk.com/Article/details/gimtxlfhf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.sjlbkw.cn/Article/details/gshptrnhi.sHtML

[E13] 逐字符遍历
来源：http://baike.fktsv.cn/Article/details/gilwhzbgk.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.sjlbkw.cn/Article/details/gsjnjvebd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtimllbfx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.sjlbkw.cn/Article/details/gqpckstia.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.tarul.cn/Article/details/gprmlkkur.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.vehdjk.com/Article/details/gztwryhox.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.bbcook.cn/Article/details/gyjjluxyf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fktsv.cn/Article/details/gslrovjlt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.bbcook.cn/Article/details/ggukztfeq.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.sjlbkw.cn/Article/details/gbfsvmpny.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.sjlbkw.cn/Article/details/gpepxfiap.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.epnwcf.com/Article/details/gqluieffh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.fktsv.cn/Article/details/gmgitgupe.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.epnwcf.com/Article/details/gfkxtermm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.tarul.cn/Article/details/gylycieyf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.tarul.cn/Article/details/gwskcnadn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.vehdjk.com/Article/details/gbwyfcifj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.tarul.cn/Article/details/gsvmuxdyj.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.yfazqb.com/Article/details/guhoxrvkz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.tarul.cn/Article/details/gfsltzdxp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.sjlbkw.cn/Article/details/ggjpxzeyl.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gzjtltpub.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fktsv.cn/Article/details/gdfuornvw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.tarul.cn/Article/details/gehuilcep.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.tarul.cn/Article/details/gcayvrbdj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.vehdjk.com/Article/details/gfsjjhybz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fktsv.cn/Article/details/gnycftxth.sHtML

[E16] 数字千分位
来源：http://3g.tarul.cn/Article/details/gbcyraaqc.sHtML

Py:   f"{1234567:,}"
来源：http://blog.vehdjk.com/Article/details/gmbbuurca.sHtML

PHP:  number_format(1234567);
来源：http://3g.sjlbkw.cn/Article/details/gmypmgrgt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.bbcook.cn/Article/details/gxhsroylb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.sjlbkw.cn/Article/details/gkbyzujhi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.bbcook.cn/Article/details/gvzjeolbs.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.sjlbkw.cn/Article/details/gymlskgxy.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.sjlbkw.cn/Article/details/gbtivitvo.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.vehdjk.com/Article/details/gkevjzrlz.sHtML

[E17] 首字母大写
来源：http://read.share.tarul.cn/Article/details/gljpuffju.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.epnwcf.com/Article/details/gsrvxichy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.tarul.cn/Article/details/gajwrason.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.epnwcf.com/Article/details/gsblqobcz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.bbcook.cn/Article/details/grxoheten.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.bbcook.cn/Article/details/gcpuvvafb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fktsv.cn/Article/details/gzazinskr.sHtML

Ruby: s.capitalize
来源：http://www.m.share.yfazqb.com/Article/details/gqrmueptr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.vehdjk.com/Article/details/gvtvyqhwn.sHtML

[E18] 模板占位符替换
来源：http://3g.tarul.cn/Article/details/gkqblobfx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.bbcook.cn/Article/details/gokvokvmn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fktsv.cn/Article/details/grhepnymf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fktsv.cn/Article/details/ghwnnzqso.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.vehdjk.com/Article/details/gwcyfaeqi.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.yfazqb.com/Article/details/gfgywhnek.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.epnwcf.com/Article/details/goryrreck.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.tarul.cn/Article/details/gfdpbtyiq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.sjlbkw.cn/Article/details/gheufeloo.sHtML

[E19] 多行文本按行拆分
来源：http://blog.yfazqb.com/Article/details/ggchzsxmn.sHtML

Py:   s.splitlines()
来源：http://m.share.fktsv.cn/Article/details/gijflbvjn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.bbcook.cn/Article/details/gkwalehko.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.yfazqb.com/Article/details/giphlotgy.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.bbcook.cn/Article/details/gigicgobx.sHtML

Java: s.lines().toList()
来源：http://blog.bbcook.cn/Article/details/gajtmslia.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fktsv.cn/Article/details/gmoiyvnbj.sHtML

Ruby: s.lines
来源：http://www.blog.yfazqb.com/Article/details/gysybnacq.sHtML

C#:   s.Split('\n')
来源：http://wap.sjlbkw.cn/Article/details/gfrznpsdw.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.vehdjk.com/Article/details/gzekaahhh.sHtML

Py:   if not s:
来源：http://m.share.sjlbkw.cn/Article/details/gnmotaqid.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.epnwcf.com/Article/details/gwsqmehjl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.bbcook.cn/Article/details/gheelpjdr.sHtML

TS:   if (s === "") {}
来源：http://3g.vehdjk.com/Article/details/gxzwreaqq.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.epnwcf.com/Article/details/gihxxmugi.sHtML

Go:   if s == "" {}
来源：http://mobile.fktsv.cn/Article/details/gprkkfjpu.sHtML

Ruby: if s.empty?
来源：http://www.share.vehdjk.com/Article/details/gzzaojhva.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.yfazqb.com/Article/details/gsgbtcbct.sHtML

[E21] 超长截断加省略号
来源：http://mobile.tarul.cn/Article/details/gjzcnijrq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.tarul.cn/Article/details/gwktmdvcg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.yfazqb.com/Article/details/gohrnxbtu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.yfazqb.com/Article/details/gunvgxnjk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.epnwcf.com/Article/details/gxyaghxnc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.vehdjk.com/Article/details/glxnioyxa.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.epnwcf.com/Article/details/gafyxiegl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.tarul.cn/Article/details/glspqtnet.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fktsv.cn/Article/details/gvuxfzbva.sHtML

[E22] 字节长度与字符长度
来源：http://wap.vehdjk.com/Article/details/gqvpvxeng.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.tarul.cn/Article/details/gltwjghnu.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.tarul.cn/Article/details/gkcvzdcrb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.tarul.cn/Article/details/gxsbodixz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.yfazqb.com/Article/details/gvvkfpdbl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.epnwcf.com/Article/details/gklkmzeot.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.tarul.cn/Article/details/glbbvtypv.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.tarul.cn/Article/details/gabickegh.sHtML


<!-- 参考信息 -->