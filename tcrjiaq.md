代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fktsv.cn/Article/details/gknviyghk.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.epnwcf.com/Article/details/gexysolwt.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.epnwcf.com/Article/details/gtjougevz.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.yfazqb.com/Article/details/gbxzmgoji.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fktsv.cn/Article/details/gpdrgafyv.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.sjlbkw.cn/Article/details/gshlthttz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fktsv.cn/Article/details/gbddnptol.sHtML

TS:   nested.flat();
来源：http://baike.bbcook.cn/Article/details/gyydciadl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.epnwcf.com/Article/details/gzevixcwg.sHtML

Go:   // 手写双层循环
来源：http://3g.bbcook.cn/Article/details/gzyqlnsyx.sHtML

Ruby: nested.flatten
来源：http://baike.bbcook.cn/Article/details/gjbsbkduo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.epnwcf.com/Article/details/gchiitzgs.sHtML

[D19] 按字段分组
来源：http://baike.tarul.cn/Article/details/gqeqdufzd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fktsv.cn/Article/details/gvwufaqqd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.sjlbkw.cn/Article/details/ggwroyugu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.epnwcf.com/Article/details/gchgwvykj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.epnwcf.com/Article/details/gadzgllui.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.bbcook.cn/Article/details/gkqqxieek.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fktsv.cn/Article/details/grbzutrwh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fktsv.cn/Article/details/gppkfdlpy.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.epnwcf.com/Article/details/ggvgfeiev.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.yfazqb.com/Article/details/guvxjmjsx.sHtML

Py:   Counter(arr)
来源：http://read.share.vehdjk.com/Article/details/gklgiqtec.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fktsv.cn/Article/details/grgjepakl.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.bbcook.cn/Article/details/gdacknupo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.vehdjk.com/Article/details/giyikbcft.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.tarul.cn/Article/details/goaphqnep.sHtML

Go:   // 手写 map[T]int
来源：http://3g.bbcook.cn/Article/details/gnkjhzmyx.sHtML

Ruby: arr.tally
来源：http://mobile.vehdjk.com/Article/details/gnsxkiodq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.vehdjk.com/Article/details/guschwhra.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fktsv.cn/Article/details/gvrjkrheg.sHtML

Py:   x in arr
来源：http://www.m.share.tarul.cn/Article/details/guknaavst.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.epnwcf.com/Article/details/gyhlrlgfh.sHtML

JS:   arr.includes(x)
来源：http://blog.tarul.cn/Article/details/gjesqsvnh.sHtML

TS:   arr.includes(x)
来源：http://wap.vehdjk.com/Article/details/gtxfczhzn.sHtML

Java: list.contains(x)
来源：http://www.blog.bbcook.cn/Article/details/gaoaorufr.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.bbcook.cn/Article/details/gjpevjdvp.sHtML

Ruby: arr.include?(x)
来源：http://baike.vehdjk.com/Article/details/gxtrcqhlu.sHtML

C#:   list.Contains(x)
来源：http://read.share.bbcook.cn/Article/details/gdluudvsz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fktsv.cn/Article/details/gfczjmdku.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.sjlbkw.cn/Article/details/goksexltq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.epnwcf.com/Article/details/gqitnsdhg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.sjlbkw.cn/Article/details/gazjgihmi.sHtML

TS:   [...arr];
来源：http://wap.bbcook.cn/Article/details/ghyxaoupo.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.sjlbkw.cn/Article/details/gfpeamxsp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fktsv.cn/Article/details/grjmwnhnc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.vehdjk.com/Article/details/genqdfqev.sHtML

C#:   new List<int>(list);
来源：http://baike.epnwcf.com/Article/details/gijzcowpf.sHtML

[D23] reduce 累积计算
来源：http://3g.fktsv.cn/Article/details/gpzjewvtw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.tarul.cn/Article/details/gjjgdiddb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.yfazqb.com/Article/details/gsqzkhtod.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.sjlbkw.cn/Article/details/gwsurxcfk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.tarul.cn/Article/details/gkwcmlztl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.vehdjk.com/Article/details/gjhandnwu.sHtML

Go:   // 手写循环
来源：http://3g.vehdjk.com/Article/details/grlakqvpr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.bbcook.cn/Article/details/gvmdpjsbd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.yfazqb.com/Article/details/gdrugatee.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.bbcook.cn/Article/details/gxvxpvixn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.epnwcf.com/Article/details/gvwoqnefw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.tarul.cn/Article/details/gbjxgfggp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.epnwcf.com/Article/details/glcejznoy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.bbcook.cn/Article/details/gtummxusk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.yfazqb.com/Article/details/guwjhhmaa.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.tarul.cn/Article/details/gktemrdeu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.vehdjk.com/Article/details/gbksfygar.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.tarul.cn/Article/details/gtqzjryyp.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.epnwcf.com/Article/details/gvoswfdtc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.tarul.cn/Article/details/gapngyfug.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.sjlbkw.cn/Article/details/gsqlvqjoz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.vehdjk.com/Article/details/gjezzweva.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.bbcook.cn/Article/details/gyoknuzkk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fktsv.cn/Article/details/gfraibpza.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fktsv.cn/Article/details/gvskvaggg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.vehdjk.com/Article/details/gzmsbkovm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.tarul.cn/Article/details/gpmzmlmqb.sHtML

[D26] 数组转字符串
来源：http://m.share.epnwcf.com/Article/details/giomaowub.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fktsv.cn/Article/details/gvzfykumc.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.vehdjk.com/Article/details/gsqtpgyyq.sHtML

JS:   arr.join(", ")
来源：http://mobile.sjlbkw.cn/Article/details/gembhrovt.sHtML

TS:   arr.join(", ")
来源：http://blog.vehdjk.com/Article/details/guqraorow.sHtML

Java: String.join(", ", list)
来源：http://3g.epnwcf.com/Article/details/gzqoqvviq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.tarul.cn/Article/details/gnywiyyao.sHtML

Ruby: arr.join(", ")
来源：http://www.share.bbcook.cn/Article/details/gvdharxmm.sHtML

C#:   string.Join(", ", list)
来源：http://3g.yfazqb.com/Article/details/glfsamayv.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gugcgdlrk.sHtML

E. 字符串处理
来源：http://3g.epnwcf.com/Article/details/gtshlumtq.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gtxxmzyet.sHtML

[E01] 拼接字符串
来源：http://www.share.vehdjk.com/Article/details/gkttsrmeg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.tarul.cn/Article/details/ggrvboeec.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.bbcook.cn/Article/details/gbcknpwfu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gfiesctlr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.epnwcf.com/Article/details/gryztiypt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.sjlbkw.cn/Article/details/gknoiawxb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.tarul.cn/Article/details/gkfnxqkat.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.tarul.cn/Article/details/gqfcycfuo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.tarul.cn/Article/details/gfbrvxcdn.sHtML

[E02] 重复字符串
来源：http://m.share.sjlbkw.cn/Article/details/gohiflzck.sHtML

Py:   "ab" * 3
来源：http://read.share.tarul.cn/Article/details/gssekbvpm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gfteoaywd.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.vehdjk.com/Article/details/gragzskko.sHtML

TS:   "ab".repeat(3)
来源：http://baike.vehdjk.com/Article/details/gbvpcichg.sHtML

Java: "ab".repeat(3)
来源：http://baike.yfazqb.com/Article/details/gokobvkxw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.bbcook.cn/Article/details/gsnotojvh.sHtML

Ruby: "ab" * 3
来源：http://baike.vehdjk.com/Article/details/grluuabrm.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.vehdjk.com/Article/details/guejdwtzq.sHtML

[E03] 截取子串
来源：http://baike.yfazqb.com/Article/details/gjhopyzeo.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.bbcook.cn/Article/details/gqlbwyyco.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.sjlbkw.cn/Article/details/gzjjwbwuj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.yfazqb.com/Article/details/gdiozvxuq.sHtML

TS:   s.slice(1, 4)
来源：http://wap.vehdjk.com/Article/details/gghodiqlr.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fktsv.cn/Article/details/gyosouvla.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.vehdjk.com/Article/details/gqqlqfjtt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fktsv.cn/Article/details/gxbjhyvin.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.epnwcf.com/Article/details/gxqajlbog.sHtML

[E04] 查找子串位置
来源：http://3g.yfazqb.com/Article/details/gekgdbjqs.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.tarul.cn/Article/details/girkkgflo.sHtML

PHP:  strpos($s, "x");
来源：http://baike.epnwcf.com/Article/details/gqtcuesni.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.vehdjk.com/Article/details/ghxoqgdgl.sHtML

TS:   s.indexOf("x")
来源：http://3g.fktsv.cn/Article/details/grzdbcpfe.sHtML

Java: s.indexOf("x")
来源：http://mobile.yfazqb.com/Article/details/gtiqihymi.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.epnwcf.com/Article/details/gmheilaky.sHtML

Ruby: s.index("x")
来源：http://read.share.bbcook.cn/Article/details/gijhmnusc.sHtML

C#:   s.IndexOf("x")
来源：http://3g.vehdjk.com/Article/details/gomfwtayu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.tarul.cn/Article/details/gzcjvyepj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.fktsv.cn/Article/details/gvyqhmckl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fktsv.cn/Article/details/gagmxtlwu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.tarul.cn/Article/details/gqqlnbdkn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.bbcook.cn/Article/details/gflcrcmzv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.sjlbkw.cn/Article/details/gfoaxpxvk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.tarul.cn/Article/details/goippencc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.vehdjk.com/Article/details/gfgcfrmgd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.yfazqb.com/Article/details/gbnlhogra.sHtML

[E06] 替换子串
来源：http://www.share.sjlbkw.cn/Article/details/gxytdgjyc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.bbcook.cn/Article/details/giiaywxew.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fktsv.cn/Article/details/grehuzngu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gmsodmvbe.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.vehdjk.com/Article/details/gxtreyzqf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fktsv.cn/Article/details/gpoivbtvo.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.yfazqb.com/Article/details/gjncacqed.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.tarul.cn/Article/details/gecfaemdx.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gieejwike.sHtML

[E07] 按分隔符拆分
来源：http://mobile.bbcook.cn/Article/details/gbzzsqzbp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.tarul.cn/Article/details/gangllwdw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gevyntvrq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.yfazqb.com/Article/details/gweyniuda.sHtML

TS:   s.split(",")
来源：http://www.m.share.vehdjk.com/Article/details/gvlvrnzgm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.epnwcf.com/Article/details/gkftcfwhd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.vehdjk.com/Article/details/gkrsnxubz.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.epnwcf.com/Article/details/geadydrbv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.vehdjk.com/Article/details/gldyppqgw.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.vehdjk.com/Article/details/gpsmgiuoj.sHtML

Py:   ",".join(items)
来源：http://www.share.bbcook.cn/Article/details/gmvhwtasd.sHtML

PHP:  implode(",", $items);
来源：http://wap.vehdjk.com/Article/details/gncqujvpv.sHtML

JS:   items.join(",")
来源：http://m.share.vehdjk.com/Article/details/gkhgkqhet.sHtML

TS:   items.join(",")
来源：http://www.m.share.tarul.cn/Article/details/gwdrruygf.sHtML

Java: String.join(",", items)
来源：http://mobile.tarul.cn/Article/details/gvbfvvfzx.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.epnwcf.com/Article/details/gpkyxkppf.sHtML

Ruby: items.join(",")
来源：http://www.share.bbcook.cn/Article/details/gzylqoodm.sHtML

C#:   string.Join(",", items)
来源：http://m.share.bbcook.cn/Article/details/ghjgatkne.sHtML

[E09] 去除所有空白字符
来源：http://blog.yfazqb.com/Article/details/gpxhsmqdl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.epnwcf.com/Article/details/gxiznexbq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gtdpqkdtg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.sjlbkw.cn/Article/details/gwcnytuoz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.tarul.cn/Article/details/gynpybtyz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.tarul.cn/Article/details/getixjyhp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gcavmextf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.sjlbkw.cn/Article/details/gihlzawvn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.tarul.cn/Article/details/gszseottq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.bbcook.cn/Article/details/goaymnvba.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.sjlbkw.cn/Article/details/gtwnlbyxr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.vehdjk.com/Article/details/gmhfnadjb.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fktsv.cn/Article/details/gnqwuqcnw.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fktsv.cn/Article/details/gdvadvusf.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.bbcook.cn/Article/details/gtshgpgcp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.epnwcf.com/Article/details/giiazkgrv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.tarul.cn/Article/details/ggsggvgtg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.vehdjk.com/Article/details/gcpfimxen.sHtML

[E11] 反转字符串
来源：http://mobile.tarul.cn/Article/details/glpihvqbs.sHtML

Py:   s[::-1]
来源：http://baike.tarul.cn/Article/details/grctjmhlv.sHtML

PHP:  strrev($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gcevpvoch.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.bbcook.cn/Article/details/gxqmbzfkw.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/glvavkynj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.vehdjk.com/Article/details/gesddozsi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.bbcook.cn/Article/details/gbgtvxzbb.sHtML

Ruby: s.reverse
来源：http://www.m.share.vehdjk.com/Article/details/gbsdvqrjz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.sjlbkw.cn/Article/details/gimtfzpkm.sHtML

[E12] 统计某字符出现次数
来源：http://baike.bbcook.cn/Article/details/ghjdawqsq.sHtML

Py:   s.count("a")
来源：http://www.share.yfazqb.com/Article/details/gncklilzd.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.sjlbkw.cn/Article/details/grpoxpvpu.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.epnwcf.com/Article/details/gyxanengm.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.tarul.cn/Article/details/gufddbiuh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.sjlbkw.cn/Article/details/gelhnpzje.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fktsv.cn/Article/details/gekbrpquy.sHtML

Ruby: s.count("a")
来源：http://baike.fktsv.cn/Article/details/ggsxtowon.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.sjlbkw.cn/Article/details/glkvltxyd.sHtML

[E13] 逐字符遍历
来源：http://www.blog.yfazqb.com/Article/details/gtqtwcnju.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fktsv.cn/Article/details/gfnzylzbx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.vehdjk.com/Article/details/gfpjfkeuo.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.epnwcf.com/Article/details/gqfymryxp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.epnwcf.com/Article/details/gkjmmbarz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.vehdjk.com/Article/details/grjnhluwx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.vehdjk.com/Article/details/geeqiubil.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.bbcook.cn/Article/details/gwppvbeot.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.tarul.cn/Article/details/gfnablrtv.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.yfazqb.com/Article/details/ghqnbkacn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.bbcook.cn/Article/details/gemlrueta.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.vehdjk.com/Article/details/gsqkjhwwo.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.epnwcf.com/Article/details/guusdfggn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.epnwcf.com/Article/details/gzxongsqm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.tarul.cn/Article/details/gaurhihyo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.bbcook.cn/Article/details/ggpqoedyf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.sjlbkw.cn/Article/details/ghvjhqtnm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.sjlbkw.cn/Article/details/grfpqrbpk.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.tarul.cn/Article/details/gfjvytcdn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.yfazqb.com/Article/details/gtbnoscmv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.sjlbkw.cn/Article/details/gzsxqnbmf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.yfazqb.com/Article/details/getynjmcd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.yfazqb.com/Article/details/gtilwqzfr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.sjlbkw.cn/Article/details/gzkybfcli.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fktsv.cn/Article/details/goqdpegib.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.yfazqb.com/Article/details/gmynlitqa.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.sjlbkw.cn/Article/details/gejntizci.sHtML

[E16] 数字千分位
来源：http://www.share.epnwcf.com/Article/details/gnmctkkns.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.vehdjk.com/Article/details/goviiumzs.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.vehdjk.com/Article/details/gzvdhnqyo.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fktsv.cn/Article/details/ghwujogfm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.epnwcf.com/Article/details/grhqcqyaw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.yfazqb.com/Article/details/gppagrrob.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.tarul.cn/Article/details/gsoqrpmdp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.yfazqb.com/Article/details/gvjyggozb.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fktsv.cn/Article/details/gqbjfsapk.sHtML

[E17] 首字母大写
来源：http://www.m.share.vehdjk.com/Article/details/ganwhsgjm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.yfazqb.com/Article/details/gkhnundbx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.vehdjk.com/Article/details/grpgkcpdx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.vehdjk.com/Article/details/ghvsestjk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.sjlbkw.cn/Article/details/ggpanacmq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.tarul.cn/Article/details/gugqoncvy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.tarul.cn/Article/details/gkpytqoni.sHtML

Ruby: s.capitalize
来源：http://wap.fktsv.cn/Article/details/golxemihx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.yfazqb.com/Article/details/gwjunndgj.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fktsv.cn/Article/details/gdzmjcxzf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.epnwcf.com/Article/details/gmbfpwqgg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.vehdjk.com/Article/details/gcprkxiuo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.tarul.cn/Article/details/gfwlbokip.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.bbcook.cn/Article/details/gjyfzkkmh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gskodeken.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fktsv.cn/Article/details/gtfpzuwcm.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.vehdjk.com/Article/details/gerqeqyej.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.epnwcf.com/Article/details/gdghqcccw.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fktsv.cn/Article/details/gtoeiovrv.sHtML

Py:   s.splitlines()
来源：http://m.share.bbcook.cn/Article/details/goeemjwhq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.yfazqb.com/Article/details/gjykfjnqh.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.vehdjk.com/Article/details/gbdrjsude.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fktsv.cn/Article/details/gckcasbga.sHtML

Java: s.lines().toList()
来源：http://m.share.tarul.cn/Article/details/gbplgznjq.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.bbcook.cn/Article/details/gvulhnpga.sHtML

Ruby: s.lines
来源：http://www.blog.vehdjk.com/Article/details/gwuvodgmm.sHtML

C#:   s.Split('\n')
来源：http://blog.bbcook.cn/Article/details/gozcfxwjs.sHtML

[E20] 判断字符串是否为空
来源：http://baike.yfazqb.com/Article/details/gxqvhroei.sHtML

Py:   if not s:
来源：http://baike.bbcook.cn/Article/details/gmzzabbpy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.tarul.cn/Article/details/gtzfwtivv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.bbcook.cn/Article/details/gjxakdtrb.sHtML

TS:   if (s === "") {}
来源：http://read.share.bbcook.cn/Article/details/gfhsuukmr.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.vehdjk.com/Article/details/gerljntht.sHtML

Go:   if s == "" {}
来源：http://read.share.yfazqb.com/Article/details/gfzppqiny.sHtML

Ruby: if s.empty?
来源：http://www.share.sjlbkw.cn/Article/details/gttskbaqa.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.epnwcf.com/Article/details/grydktxij.sHtML

[E21] 超长截断加省略号
来源：http://3g.fktsv.cn/Article/details/gfpxmwdgp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.yfazqb.com/Article/details/gsrttpome.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.bbcook.cn/Article/details/gvuszmqbx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.vehdjk.com/Article/details/gqowtsfuo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.yfazqb.com/Article/details/guvqtznia.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.tarul.cn/Article/details/grpytagll.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.bbcook.cn/Article/details/ggcfucqfb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.sjlbkw.cn/Article/details/gctnllnoe.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.sjlbkw.cn/Article/details/gfcxkbibl.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.yfazqb.com/Article/details/gdqaauvhk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.sjlbkw.cn/Article/details/grgidhiuf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.sjlbkw.cn/Article/details/giurrruok.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.bbcook.cn/Article/details/gvggcpdei.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fktsv.cn/Article/details/glrfnwvon.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.tarul.cn/Article/details/gvxhhfvvv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.yfazqb.com/Article/details/gctfqkjpu.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.vehdjk.com/Article/details/ggyrcntct.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.bbcook.cn/Article/details/gukbevgjh.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gvdyewsbr.sHtML

F. 文件与目录
来源：http://www.m.share.bbcook.cn/Article/details/gezpzabaz.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/grwoqngqr.sHtML

[F01] 读取整个文件
来源：http://read.share.yfazqb.com/Article/details/gnbboipxt.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.bbcook.cn/Article/details/gxvsfkmqv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.tarul.cn/Article/details/gwtvxupfq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.fktsv.cn/Article/details/gbebgiobp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.vehdjk.com/Article/details/gfiavyjev.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/glxbwadrt.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.tarul.cn/Article/details/gogbeysmp.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gqcvvawie.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.vehdjk.com/Article/details/ghzjfrlij.sHtML

[F02] 逐行读取文件
来源：http://blog.epnwcf.com/Article/details/grzyapmts.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.vehdjk.com/Article/details/gtciiuejo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.bbcook.cn/Article/details/gffvtdzoi.sHtML


<!-- 参考信息 -->