代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.tarul.cn/Article/details/gkfvnsfag.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.vehdjk.com/Article/details/gtumxukrr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.yfazqb.com/Article/details/gyuhycvih.sHtML

Go:   // 手写循环累加
来源：http://www.share.epnwcf.com/Article/details/ghahafktu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.vehdjk.com/Article/details/grranltlh.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.vehdjk.com/Article/details/gftkgkdyo.sHtML

[D17] 最大值与最小值
来源：http://mobile.epnwcf.com/Article/details/gpifhgftg.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.tarul.cn/Article/details/gnxhfmcwu.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.vehdjk.com/Article/details/grxgrwcew.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.epnwcf.com/Article/details/gmfcfqxat.sHtML

TS:   Math.max(...arr);
来源：http://wap.epnwcf.com/Article/details/gfcqzxjvi.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.bbcook.cn/Article/details/ghiuxfton.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.epnwcf.com/Article/details/gzlggauii.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.vehdjk.com/Article/details/gyctkqyee.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.bbcook.cn/Article/details/glkqsthvp.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fktsv.cn/Article/details/gerjodaid.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.epnwcf.com/Article/details/gfhtyuvxh.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.yfazqb.com/Article/details/gsjjhsovc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.epnwcf.com/Article/details/glyedawcf.sHtML

TS:   nested.flat();
来源：http://3g.tarul.cn/Article/details/gclkjmkjt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.bbcook.cn/Article/details/gfftiwgpg.sHtML

Go:   // 手写双层循环
来源：http://www.share.tarul.cn/Article/details/gsriqcqqu.sHtML

Ruby: nested.flatten
来源：http://www.blog.bbcook.cn/Article/details/ggxdahjwo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.vehdjk.com/Article/details/gfvvrlpjp.sHtML

[D19] 按字段分组
来源：http://blog.sjlbkw.cn/Article/details/gxzyrepxr.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gjfglsajr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.tarul.cn/Article/details/gsyuhizxj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fktsv.cn/Article/details/glryujdgi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.tarul.cn/Article/details/gzgknawea.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.vehdjk.com/Article/details/gxfwesdlq.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fktsv.cn/Article/details/ghienpyyb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.bbcook.cn/Article/details/gkvddcwjh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fktsv.cn/Article/details/guubkchvf.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.vehdjk.com/Article/details/gdivotvzl.sHtML

Py:   Counter(arr)
来源：http://3g.yfazqb.com/Article/details/geginroot.sHtML

PHP:  array_count_values($arr);
来源：http://wap.yfazqb.com/Article/details/gqmevpitr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.bbcook.cn/Article/details/gdpzundli.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fktsv.cn/Article/details/ghvquchui.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.yfazqb.com/Article/details/gfqvnapeq.sHtML

Go:   // 手写 map[T]int
来源：http://3g.sjlbkw.cn/Article/details/gsibgvxjg.sHtML

Ruby: arr.tally
来源：http://www.m.share.tarul.cn/Article/details/gflcqrggu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.tarul.cn/Article/details/gcamajaig.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.bbcook.cn/Article/details/gzioumjcs.sHtML

Py:   x in arr
来源：http://baike.sjlbkw.cn/Article/details/gajhowzre.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.tarul.cn/Article/details/gxgujrige.sHtML

JS:   arr.includes(x)
来源：http://www.blog.bbcook.cn/Article/details/gefboeqdc.sHtML

TS:   arr.includes(x)
来源：http://baike.fktsv.cn/Article/details/gsinhpxdw.sHtML

Java: list.contains(x)
来源：http://m.share.sjlbkw.cn/Article/details/ghkeurrvx.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gjaulekgk.sHtML

Ruby: arr.include?(x)
来源：http://www.share.sjlbkw.cn/Article/details/gpxduxlww.sHtML

C#:   list.Contains(x)
来源：http://blog.fktsv.cn/Article/details/gfmwavyzt.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.vehdjk.com/Article/details/grbwywshk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.bbcook.cn/Article/details/gpzmekbbf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.tarul.cn/Article/details/guudxshpj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.vehdjk.com/Article/details/gguztxkon.sHtML

TS:   [...arr];
来源：http://www.m.share.fktsv.cn/Article/details/gmruqvgyi.sHtML

Java: new ArrayList<>(list);
来源：http://3g.sjlbkw.cn/Article/details/glivhuoou.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.tarul.cn/Article/details/gdnrlfgfh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.yfazqb.com/Article/details/gbavnejxb.sHtML

C#:   new List<int>(list);
来源：http://wap.vehdjk.com/Article/details/gyicfvovf.sHtML

[D23] reduce 累积计算
来源：http://baike.epnwcf.com/Article/details/gnrkanhtx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.tarul.cn/Article/details/guqpunvby.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.sjlbkw.cn/Article/details/gprtsfsac.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.epnwcf.com/Article/details/gcmunhaaj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.yfazqb.com/Article/details/gpiyunsum.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.yfazqb.com/Article/details/gidofyuwn.sHtML

Go:   // 手写循环
来源：http://baike.bbcook.cn/Article/details/gslxbwoxw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fktsv.cn/Article/details/gvusaptwu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.yfazqb.com/Article/details/gjqgfwlfx.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.vehdjk.com/Article/details/gsfkyjeua.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.tarul.cn/Article/details/gyaqwaqyz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fktsv.cn/Article/details/ggchbwgrr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.bbcook.cn/Article/details/gknwshjdf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.sjlbkw.cn/Article/details/gxuehnaem.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.epnwcf.com/Article/details/glbsfyaps.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.yfazqb.com/Article/details/giaowghlk.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.vehdjk.com/Article/details/giupzrmzd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.tarul.cn/Article/details/gzgriedtp.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.vehdjk.com/Article/details/gttpkrymg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fktsv.cn/Article/details/gnczwkhli.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.vehdjk.com/Article/details/gkmmwfock.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.bbcook.cn/Article/details/gpgsmfsmf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.vehdjk.com/Article/details/gznsbujil.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.bbcook.cn/Article/details/gcrsgxtqf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.bbcook.cn/Article/details/gakepttuu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.epnwcf.com/Article/details/gvqulyedf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.yfazqb.com/Article/details/gbfeegnew.sHtML

[D26] 数组转字符串
来源：http://blog.bbcook.cn/Article/details/gjeolneec.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.sjlbkw.cn/Article/details/gwfppaftp.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.yfazqb.com/Article/details/gfsetlewy.sHtML

JS:   arr.join(", ")
来源：http://read.share.epnwcf.com/Article/details/govhgdeez.sHtML

TS:   arr.join(", ")
来源：http://wap.sjlbkw.cn/Article/details/giyvollqd.sHtML

Java: String.join(", ", list)
来源：http://read.share.bbcook.cn/Article/details/gtidfffdi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.vehdjk.com/Article/details/goloolehh.sHtML

Ruby: arr.join(", ")
来源：http://3g.epnwcf.com/Article/details/glvkkvusz.sHtML

C#:   string.Join(", ", list)
来源：http://baike.tarul.cn/Article/details/guibojybq.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gofazjemj.sHtML

E. 字符串处理
来源：http://m.share.epnwcf.com/Article/details/gftpbtjyf.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gfsmdgopc.sHtML

[E01] 拼接字符串
来源：http://read.share.yfazqb.com/Article/details/giprnnqfj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.tarul.cn/Article/details/gdqaxcuba.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.epnwcf.com/Article/details/gwwwttlhh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.tarul.cn/Article/details/gtlsaxoin.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.tarul.cn/Article/details/gnlobfkod.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.yfazqb.com/Article/details/gcslbhlug.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.tarul.cn/Article/details/gomlpfocz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.yfazqb.com/Article/details/gdzvibqwu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gcaxcorbc.sHtML

[E02] 重复字符串
来源：http://www.share.tarul.cn/Article/details/gctfrrbdu.sHtML

Py:   "ab" * 3
来源：http://mobile.vehdjk.com/Article/details/gbxqmbtpa.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.sjlbkw.cn/Article/details/glfoehbcr.sHtML

JS:   "ab".repeat(3)
来源：http://blog.yfazqb.com/Article/details/gvroiybqo.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.vehdjk.com/Article/details/gfkfdkwol.sHtML

Java: "ab".repeat(3)
来源：http://3g.epnwcf.com/Article/details/ghysxxwzn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.tarul.cn/Article/details/gcqumeorn.sHtML

Ruby: "ab" * 3
来源：http://wap.vehdjk.com/Article/details/geekpaxak.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.yfazqb.com/Article/details/gxjlqzqdz.sHtML

[E03] 截取子串
来源：http://3g.bbcook.cn/Article/details/gouaasqjh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.yfazqb.com/Article/details/gtjdxlihl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.epnwcf.com/Article/details/gblzwhwgf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.epnwcf.com/Article/details/gwfcfmmzx.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.yfazqb.com/Article/details/glztoagst.sHtML

Java: s.substring(1, 4)
来源：http://mobile.tarul.cn/Article/details/gcatjusyb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.sjlbkw.cn/Article/details/gckzjehxc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.tarul.cn/Article/details/gujhalakb.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.tarul.cn/Article/details/gwrwmbfce.sHtML

[E04] 查找子串位置
来源：http://www.m.share.tarul.cn/Article/details/gvucvyjxn.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.sjlbkw.cn/Article/details/gxeiuguif.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.vehdjk.com/Article/details/gdcooqqkt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.yfazqb.com/Article/details/gxsieeqkk.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.vehdjk.com/Article/details/gtavlqfvi.sHtML

Java: s.indexOf("x")
来源：http://blog.bbcook.cn/Article/details/gfkpmppxe.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.bbcook.cn/Article/details/gzahfwfow.sHtML

Ruby: s.index("x")
来源：http://baike.fktsv.cn/Article/details/goyruouoq.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.epnwcf.com/Article/details/grzmybcah.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.yfazqb.com/Article/details/gtkcqeoei.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.yfazqb.com/Article/details/ghkchkvtg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.tarul.cn/Article/details/gvhlkhqfo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.tarul.cn/Article/details/gdysqeakl.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.vehdjk.com/Article/details/gwglsjuje.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.sjlbkw.cn/Article/details/gzuesmwdo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.yfazqb.com/Article/details/gjucenkcp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.tarul.cn/Article/details/gokkenmaq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.vehdjk.com/Article/details/gjjebwcgg.sHtML

[E06] 替换子串
来源：http://read.share.yfazqb.com/Article/details/ghvkrmhwo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.yfazqb.com/Article/details/grugehkho.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.sjlbkw.cn/Article/details/gwcbdmwcd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.vehdjk.com/Article/details/glbbdordr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.tarul.cn/Article/details/gehnqmfol.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gwfjsytkq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.epnwcf.com/Article/details/gfcjqigrl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gzjqaithd.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.epnwcf.com/Article/details/gzhboamzn.sHtML

[E07] 按分隔符拆分
来源：http://blog.vehdjk.com/Article/details/gqujcvwkp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fktsv.cn/Article/details/grntqkuxq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtfnaqpet.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.vehdjk.com/Article/details/gydshkeit.sHtML

TS:   s.split(",")
来源：http://www.m.share.vehdjk.com/Article/details/gtsbbzbsh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.tarul.cn/Article/details/gxhbaehjb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.yfazqb.com/Article/details/gslcvucae.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.sjlbkw.cn/Article/details/goheyfyuv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.tarul.cn/Article/details/gsufmbasl.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.sjlbkw.cn/Article/details/gvulacsse.sHtML

Py:   ",".join(items)
来源：http://mobile.epnwcf.com/Article/details/gjijcrswz.sHtML

PHP:  implode(",", $items);
来源：http://blog.bbcook.cn/Article/details/gfjjdpfla.sHtML

JS:   items.join(",")
来源：http://m.share.epnwcf.com/Article/details/gniicdrwo.sHtML

TS:   items.join(",")
来源：http://www.share.epnwcf.com/Article/details/gamgknbum.sHtML

Java: String.join(",", items)
来源：http://www.m.share.vehdjk.com/Article/details/gbkhduucc.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fktsv.cn/Article/details/ggslpoeyh.sHtML

Ruby: items.join(",")
来源：http://www.blog.tarul.cn/Article/details/gqaawfbvw.sHtML

C#:   string.Join(",", items)
来源：http://baike.sjlbkw.cn/Article/details/gzkhrnqay.sHtML

[E09] 去除所有空白字符
来源：http://m.share.sjlbkw.cn/Article/details/gfdleeasj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.tarul.cn/Article/details/gihwljmfw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.sjlbkw.cn/Article/details/ghhhrwoab.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.tarul.cn/Article/details/glntbtdyt.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.epnwcf.com/Article/details/gqohxkkhl.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.yfazqb.com/Article/details/gnjuduzcz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.sjlbkw.cn/Article/details/gkildphyd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.yfazqb.com/Article/details/glvyoqbzy.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fktsv.cn/Article/details/gjlrpgect.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.bbcook.cn/Article/details/gvnqojncf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.yfazqb.com/Article/details/guztzxxlt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.vehdjk.com/Article/details/gaejtelsu.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.sjlbkw.cn/Article/details/giiipqoou.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.bbcook.cn/Article/details/gbtgmdfkr.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.yfazqb.com/Article/details/guvtlpkmh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.vehdjk.com/Article/details/gpejmztot.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.yfazqb.com/Article/details/gprykxwsh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.vehdjk.com/Article/details/gyupldgao.sHtML

[E11] 反转字符串
来源：http://m.share.epnwcf.com/Article/details/gnadnuvkb.sHtML

Py:   s[::-1]
来源：http://3g.fktsv.cn/Article/details/gojynuler.sHtML

PHP:  strrev($s);
来源：http://www.m.share.epnwcf.com/Article/details/gthxnqatm.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fktsv.cn/Article/details/gunxrgwyw.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.fktsv.cn/Article/details/gwgafqgah.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.yfazqb.com/Article/details/ghzjeoaxf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.bbcook.cn/Article/details/gwgvkvhva.sHtML

Ruby: s.reverse
来源：http://mobile.fktsv.cn/Article/details/ghokbzgil.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.tarul.cn/Article/details/guooflsnx.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fktsv.cn/Article/details/gbtgeijzy.sHtML

Py:   s.count("a")
来源：http://m.share.sjlbkw.cn/Article/details/gbhyyswiy.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.bbcook.cn/Article/details/gabrrkkgm.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.tarul.cn/Article/details/gdbdydjwe.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.vehdjk.com/Article/details/gvobwjyix.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.sjlbkw.cn/Article/details/ghwiofijf.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.sjlbkw.cn/Article/details/gecpmhmiq.sHtML

Ruby: s.count("a")
来源：http://read.share.tarul.cn/Article/details/gvtwbrhun.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fktsv.cn/Article/details/gybseflbd.sHtML

[E13] 逐字符遍历
来源：http://www.blog.sjlbkw.cn/Article/details/grxktpdac.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.tarul.cn/Article/details/gjlftifet.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.sjlbkw.cn/Article/details/gyshkpndo.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.sjlbkw.cn/Article/details/gqhqnvkch.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.sjlbkw.cn/Article/details/gequldool.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.yfazqb.com/Article/details/gfukwirmn.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.yfazqb.com/Article/details/gqqzaulut.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.sjlbkw.cn/Article/details/gyunbymko.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.sjlbkw.cn/Article/details/gfdahobmg.sHtML

[E14] URL 编码与 Base64
来源：http://baike.yfazqb.com/Article/details/gaytmpyos.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.yfazqb.com/Article/details/ghvldhdmb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.epnwcf.com/Article/details/gdeofjkaq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.vehdjk.com/Article/details/gdplprepd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.tarul.cn/Article/details/gmybrxyxk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.yfazqb.com/Article/details/gvctgtyhb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.epnwcf.com/Article/details/gtxljexty.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.tarul.cn/Article/details/gteyaqoyd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.sjlbkw.cn/Article/details/gmdiilztg.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.bbcook.cn/Article/details/grualcvcn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.yfazqb.com/Article/details/geqabsvkb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.epnwcf.com/Article/details/gnqvwjgkr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.bbcook.cn/Article/details/gxserlaua.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.fktsv.cn/Article/details/gqfvtzgbq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.vehdjk.com/Article/details/gzcapuvnl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.yfazqb.com/Article/details/grmwgpwnv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.epnwcf.com/Article/details/gzupifgyg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fktsv.cn/Article/details/gcwljhmqq.sHtML

[E16] 数字千分位
来源：http://wap.tarul.cn/Article/details/gsafqatyn.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.sjlbkw.cn/Article/details/gfstqctpm.sHtML

PHP:  number_format(1234567);
来源：http://read.share.sjlbkw.cn/Article/details/grmdmwqqk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.epnwcf.com/Article/details/gjhxpufup.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.epnwcf.com/Article/details/gznndmptv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.epnwcf.com/Article/details/glbfvluxp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.bbcook.cn/Article/details/gajhmipsf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.bbcook.cn/Article/details/gugmeuwny.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.sjlbkw.cn/Article/details/gyysagbxz.sHtML

[E17] 首字母大写
来源：http://www.blog.bbcook.cn/Article/details/gmqbklsna.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.tarul.cn/Article/details/gmihtzfhl.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.epnwcf.com/Article/details/gvrppulpw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.tarul.cn/Article/details/gskcpltct.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.epnwcf.com/Article/details/ghbwiwzxj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.tarul.cn/Article/details/gydqrpadd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.sjlbkw.cn/Article/details/gotbmjyul.sHtML

Ruby: s.capitalize
来源：http://m.share.tarul.cn/Article/details/guxjzlvxp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fktsv.cn/Article/details/gqanvbept.sHtML

[E18] 模板占位符替换
来源：http://baike.fktsv.cn/Article/details/gzrcmvnaa.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.yfazqb.com/Article/details/gijomewwg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.vehdjk.com/Article/details/gkkvjgvjj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.sjlbkw.cn/Article/details/gphsrgmzo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.yfazqb.com/Article/details/gkeshphie.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.epnwcf.com/Article/details/gygefgxgm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.vehdjk.com/Article/details/gxhqcphrl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fktsv.cn/Article/details/gmkufxszw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.vehdjk.com/Article/details/gathexpwg.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fktsv.cn/Article/details/gdocbwrdf.sHtML

Py:   s.splitlines()
来源：http://blog.vehdjk.com/Article/details/gljczvlzl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.tarul.cn/Article/details/gpphpuqbd.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.bbcook.cn/Article/details/gezpnamex.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fktsv.cn/Article/details/gqhyxtahz.sHtML

Java: s.lines().toList()
来源：http://3g.fktsv.cn/Article/details/giqqfbkyw.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.epnwcf.com/Article/details/gribrfyrm.sHtML

Ruby: s.lines
来源：http://m.share.fktsv.cn/Article/details/gmwxwsemc.sHtML

C#:   s.Split('\n')
来源：http://mobile.sjlbkw.cn/Article/details/gehaqqllt.sHtML

[E20] 判断字符串是否为空
来源：http://wap.sjlbkw.cn/Article/details/gzzddstqx.sHtML

Py:   if not s:
来源：http://3g.tarul.cn/Article/details/gsbtvcgsq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.tarul.cn/Article/details/gxiydvmbk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.epnwcf.com/Article/details/gyfbknuya.sHtML

TS:   if (s === "") {}
来源：http://baike.vehdjk.com/Article/details/gbpniqizn.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.sjlbkw.cn/Article/details/gjbclqebr.sHtML

Go:   if s == "" {}
来源：http://www.blog.sjlbkw.cn/Article/details/gpsjvkpub.sHtML

Ruby: if s.empty?
来源：http://m.share.epnwcf.com/Article/details/gxwsbxzik.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.bbcook.cn/Article/details/gmqivszln.sHtML

[E21] 超长截断加省略号
来源：http://wap.bbcook.cn/Article/details/gygfhegix.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.fktsv.cn/Article/details/gxawwaonf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fktsv.cn/Article/details/gwqvjdgxk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/gkgyruztm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.yfazqb.com/Article/details/gynuzfxww.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fktsv.cn/Article/details/gggbgwido.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.epnwcf.com/Article/details/gmcgediij.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/gtmqyavos.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.bbcook.cn/Article/details/gashqxjwd.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.epnwcf.com/Article/details/gagjunboh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.yfazqb.com/Article/details/gsxmagyco.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.tarul.cn/Article/details/gtbtajnrr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.bbcook.cn/Article/details/grpwzcqmk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.sjlbkw.cn/Article/details/gfnogtclc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.sjlbkw.cn/Article/details/gjichalvq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.vehdjk.com/Article/details/gfskegtwp.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.sjlbkw.cn/Article/details/gkinlzacl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.bbcook.cn/Article/details/guqmyttad.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gvyolyxtq.sHtML

F. 文件与目录
来源：http://www.m.share.vehdjk.com/Article/details/glzpyawkv.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gfydybphl.sHtML


<!-- 参考信息 -->