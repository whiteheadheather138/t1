代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.tarul.cn/Article/details/gqclkhqbq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gngcqqfip.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.tarul.cn/Article/details/gfomfcmaa.sHtML

Go:   // 手写循环累加
来源：http://www.share.epnwcf.com/Article/details/gsdjhmbxm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.epnwcf.com/Article/details/gfwymcrrf.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.bbcook.cn/Article/details/glgqqhuzz.sHtML

[D17] 最大值与最小值
来源：http://mobile.vehdjk.com/Article/details/geuldmbwg.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.vehdjk.com/Article/details/giuthyhot.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gngsapovj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.yfazqb.com/Article/details/gcpapkhpk.sHtML

TS:   Math.max(...arr);
来源：http://www.share.bbcook.cn/Article/details/gcaflsaww.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.epnwcf.com/Article/details/gmwzktddw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.vehdjk.com/Article/details/gnujnlqpd.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fktsv.cn/Article/details/gzecdqqox.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.bbcook.cn/Article/details/gbuqsvium.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.bbcook.cn/Article/details/guihbrpyv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.epnwcf.com/Article/details/ggrjcqjcj.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fktsv.cn/Article/details/gfayzhupn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.yfazqb.com/Article/details/gvwtjfyfc.sHtML

TS:   nested.flat();
来源：http://3g.bbcook.cn/Article/details/gjmoogmka.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.epnwcf.com/Article/details/gncbtbsuh.sHtML

Go:   // 手写双层循环
来源：http://www.blog.yfazqb.com/Article/details/gfjkagtth.sHtML

Ruby: nested.flatten
来源：http://www.m.share.bbcook.cn/Article/details/ggpuatjdd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fktsv.cn/Article/details/gxjargvpq.sHtML

[D19] 按字段分组
来源：http://blog.yfazqb.com/Article/details/ghvncrzab.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.tarul.cn/Article/details/gxhstqoqi.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.vehdjk.com/Article/details/gjkbgoejf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.epnwcf.com/Article/details/gmvqroriy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.bbcook.cn/Article/details/ggbtpzfjj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.vehdjk.com/Article/details/gwewbxhum.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.bbcook.cn/Article/details/ghoddujki.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.sjlbkw.cn/Article/details/gkfjnuuhn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.epnwcf.com/Article/details/gfhsugxxe.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fktsv.cn/Article/details/ghxxcvbgf.sHtML

Py:   Counter(arr)
来源：http://baike.tarul.cn/Article/details/gjehbigvh.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fktsv.cn/Article/details/gmxtkfeev.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.epnwcf.com/Article/details/gaecyiowr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.tarul.cn/Article/details/gtbxieaju.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.vehdjk.com/Article/details/ggsoknasq.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.yfazqb.com/Article/details/gtzzbrluo.sHtML

Ruby: arr.tally
来源：http://m.share.epnwcf.com/Article/details/gyqvwxcxu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.epnwcf.com/Article/details/gfwoyuazk.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.bbcook.cn/Article/details/gxkjxdwox.sHtML

Py:   x in arr
来源：http://read.share.vehdjk.com/Article/details/gwpdddgzb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.tarul.cn/Article/details/gniqarwyr.sHtML

JS:   arr.includes(x)
来源：http://wap.yfazqb.com/Article/details/gtroutkdv.sHtML

TS:   arr.includes(x)
来源：http://mobile.sjlbkw.cn/Article/details/gggrydxfc.sHtML

Java: list.contains(x)
来源：http://www.share.tarul.cn/Article/details/getkafwwi.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gfybiwypz.sHtML

Ruby: arr.include?(x)
来源：http://baike.sjlbkw.cn/Article/details/gznuebntl.sHtML

C#:   list.Contains(x)
来源：http://baike.tarul.cn/Article/details/gpsberksd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.sjlbkw.cn/Article/details/gswxebagv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fktsv.cn/Article/details/gujblztmk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.bbcook.cn/Article/details/gljurijmt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.sjlbkw.cn/Article/details/gyfewsdda.sHtML

TS:   [...arr];
来源：http://mobile.fktsv.cn/Article/details/gvdcwcjvw.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.bbcook.cn/Article/details/gyrjaozri.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fktsv.cn/Article/details/geobqalvm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.yfazqb.com/Article/details/gsaruwghr.sHtML

C#:   new List<int>(list);
来源：http://www.blog.epnwcf.com/Article/details/gffzvmunf.sHtML

[D23] reduce 累积计算
来源：http://mobile.tarul.cn/Article/details/gwgcqgsrg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.tarul.cn/Article/details/ganfaxbjj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.tarul.cn/Article/details/gghcyzijm.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fktsv.cn/Article/details/gjyxslyfi.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fktsv.cn/Article/details/gtxguxqwi.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.yfazqb.com/Article/details/gfyytbeiw.sHtML

Go:   // 手写循环
来源：http://www.m.share.tarul.cn/Article/details/gvwvwrigy.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fktsv.cn/Article/details/guniiybbn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.tarul.cn/Article/details/glwxcefkx.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.bbcook.cn/Article/details/gbhjggpha.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.sjlbkw.cn/Article/details/gpqwlgkkf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.bbcook.cn/Article/details/gzleqrekq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.bbcook.cn/Article/details/grshssrzd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gisgcgxlo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.epnwcf.com/Article/details/gbloormit.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.tarul.cn/Article/details/gxzcmszwh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.yfazqb.com/Article/details/gpyvrvylu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.yfazqb.com/Article/details/goiwwoecj.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.yfazqb.com/Article/details/gkfhnnikk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.vehdjk.com/Article/details/gsvlwgqyw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.sjlbkw.cn/Article/details/ggobpxmph.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.yfazqb.com/Article/details/gkwuhtgjx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.yfazqb.com/Article/details/gujrshrjc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.epnwcf.com/Article/details/giazvxche.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.yfazqb.com/Article/details/gfxqtzvun.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fktsv.cn/Article/details/grqzmvufw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.bbcook.cn/Article/details/gudfgtuop.sHtML

[D26] 数组转字符串
来源：http://read.share.epnwcf.com/Article/details/gjuvrsooz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.yfazqb.com/Article/details/ghnarsnjh.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.yfazqb.com/Article/details/gpgqqpiei.sHtML

JS:   arr.join(", ")
来源：http://www.share.epnwcf.com/Article/details/gboaecekv.sHtML

TS:   arr.join(", ")
来源：http://www.blog.sjlbkw.cn/Article/details/gqihitijw.sHtML

Java: String.join(", ", list)
来源：http://baike.tarul.cn/Article/details/gaeyfzlzn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.vehdjk.com/Article/details/gfquthyuv.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fktsv.cn/Article/details/grmyrpwfy.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.sjlbkw.cn/Article/details/gahgoyndk.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gutizkwii.sHtML

E. 字符串处理
来源：http://www.share.vehdjk.com/Article/details/gbozaikqn.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gmcdapjff.sHtML

[E01] 拼接字符串
来源：http://m.share.sjlbkw.cn/Article/details/gpauvokaw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.vehdjk.com/Article/details/gkeccnkci.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.sjlbkw.cn/Article/details/gunlzyehx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.sjlbkw.cn/Article/details/gmtxunnid.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.tarul.cn/Article/details/gxewrthch.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.tarul.cn/Article/details/gvrtrygcw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.tarul.cn/Article/details/glgxhywbs.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.yfazqb.com/Article/details/gmokhldxk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.epnwcf.com/Article/details/gxwsmokzi.sHtML

[E02] 重复字符串
来源：http://blog.tarul.cn/Article/details/gvjlnnvec.sHtML

Py:   "ab" * 3
来源：http://m.share.fktsv.cn/Article/details/glshphema.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.yfazqb.com/Article/details/gcgtdijfn.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtbmmyrem.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fktsv.cn/Article/details/gcfydsiwj.sHtML

Java: "ab".repeat(3)
来源：http://m.share.yfazqb.com/Article/details/gvpizumlh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.tarul.cn/Article/details/gyvfltkrp.sHtML

Ruby: "ab" * 3
来源：http://www.share.bbcook.cn/Article/details/gbxvukdrq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.fktsv.cn/Article/details/gotusnfsx.sHtML

[E03] 截取子串
来源：http://www.blog.yfazqb.com/Article/details/gcpybklzv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.sjlbkw.cn/Article/details/gubmjleui.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/gcfbcyktl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.sjlbkw.cn/Article/details/gdsgsdhec.sHtML

TS:   s.slice(1, 4)
来源：http://3g.vehdjk.com/Article/details/glanppink.sHtML

Java: s.substring(1, 4)
来源：http://wap.fktsv.cn/Article/details/gpkzbpeem.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.yfazqb.com/Article/details/gkxzdfupr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.sjlbkw.cn/Article/details/gmihoypqs.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fktsv.cn/Article/details/gcjojlwxg.sHtML

[E04] 查找子串位置
来源：http://www.share.sjlbkw.cn/Article/details/gxcnqbzwy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fktsv.cn/Article/details/gtuaueufw.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.tarul.cn/Article/details/gvyfhffgm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.vehdjk.com/Article/details/gverjvewc.sHtML

TS:   s.indexOf("x")
来源：http://m.share.epnwcf.com/Article/details/gvemaaukl.sHtML

Java: s.indexOf("x")
来源：http://wap.fktsv.cn/Article/details/graliskxf.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.epnwcf.com/Article/details/gqczvovri.sHtML

Ruby: s.index("x")
来源：http://www.m.share.vehdjk.com/Article/details/gicpowghi.sHtML

C#:   s.IndexOf("x")
来源：http://wap.tarul.cn/Article/details/godhgazdc.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.epnwcf.com/Article/details/ggyrqfnik.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.vehdjk.com/Article/details/gygzrsydw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fktsv.cn/Article/details/gdfwnllnv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fktsv.cn/Article/details/gutagsksr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.bbcook.cn/Article/details/gpwjdpqaj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.bbcook.cn/Article/details/grtaxmjzd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.tarul.cn/Article/details/gafmvsbfc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.sjlbkw.cn/Article/details/grnjjchma.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.bbcook.cn/Article/details/gciwznhrw.sHtML

[E06] 替换子串
来源：http://www.share.yfazqb.com/Article/details/gnlthutwg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.epnwcf.com/Article/details/guyuntlhs.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.tarul.cn/Article/details/ghtdzmcod.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/gvqhcrjkg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.vehdjk.com/Article/details/gboipxmhj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gyjelgnlk.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.yfazqb.com/Article/details/gaerqofyj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gmiyyqvxi.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fktsv.cn/Article/details/gihfgavue.sHtML

[E07] 按分隔符拆分
来源：http://blog.sjlbkw.cn/Article/details/gygoyfnkl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fktsv.cn/Article/details/geiehbams.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.yfazqb.com/Article/details/gokgivndy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.tarul.cn/Article/details/gcpnhzlve.sHtML

TS:   s.split(",")
来源：http://m.share.bbcook.cn/Article/details/gfqvhiach.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqmqkfgtr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.yfazqb.com/Article/details/gjtrkiyeb.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.epnwcf.com/Article/details/gmqonukoz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.epnwcf.com/Article/details/gfjusmtzh.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.yfazqb.com/Article/details/gmevvbicd.sHtML

Py:   ",".join(items)
来源：http://mobile.tarul.cn/Article/details/glrujeidu.sHtML

PHP:  implode(",", $items);
来源：http://mobile.sjlbkw.cn/Article/details/gzdxlchzy.sHtML

JS:   items.join(",")
来源：http://3g.sjlbkw.cn/Article/details/gsnowrzfl.sHtML

TS:   items.join(",")
来源：http://www.blog.sjlbkw.cn/Article/details/gplgjqbus.sHtML

Java: String.join(",", items)
来源：http://www.m.share.vehdjk.com/Article/details/gwjzvmjhc.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fktsv.cn/Article/details/gceqmbqfx.sHtML

Ruby: items.join(",")
来源：http://www.m.share.vehdjk.com/Article/details/giajwpnzh.sHtML

C#:   string.Join(",", items)
来源：http://mobile.yfazqb.com/Article/details/gjxvzcdyk.sHtML

[E09] 去除所有空白字符
来源：http://3g.epnwcf.com/Article/details/gckcaiodg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.yfazqb.com/Article/details/ggcmwioka.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.vehdjk.com/Article/details/gmyjavrxa.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fktsv.cn/Article/details/gwyldejym.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.bbcook.cn/Article/details/gnbspiecn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.tarul.cn/Article/details/gngaucsvm.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.sjlbkw.cn/Article/details/giwnxycrs.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.fktsv.cn/Article/details/geulaukns.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.bbcook.cn/Article/details/gkegbzebq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.vehdjk.com/Article/details/gwmlpyvad.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.yfazqb.com/Article/details/gmjpmytbh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.bbcook.cn/Article/details/gjcdrsogd.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.epnwcf.com/Article/details/gooocqrpz.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fktsv.cn/Article/details/galtrasvp.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.tarul.cn/Article/details/gtcjukhsc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.bbcook.cn/Article/details/ggpfquzhg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.epnwcf.com/Article/details/gudukoijj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.yfazqb.com/Article/details/grfssbhoc.sHtML

[E11] 反转字符串
来源：http://blog.yfazqb.com/Article/details/gjissyvgt.sHtML

Py:   s[::-1]
来源：http://www.share.tarul.cn/Article/details/gjxxkubwd.sHtML

PHP:  strrev($s);
来源：http://baike.epnwcf.com/Article/details/gsqdiggnn.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.vehdjk.com/Article/details/gybjjtdqs.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.tarul.cn/Article/details/giahrtyyg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.epnwcf.com/Article/details/gkuxftrky.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.tarul.cn/Article/details/guyycuakl.sHtML

Ruby: s.reverse
来源：http://www.share.epnwcf.com/Article/details/gqqyofidq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fktsv.cn/Article/details/gxacxwngk.sHtML

[E12] 统计某字符出现次数
来源：http://3g.sjlbkw.cn/Article/details/gneaelinh.sHtML

Py:   s.count("a")
来源：http://wap.fktsv.cn/Article/details/gzmycvjzh.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.tarul.cn/Article/details/gwhawapyf.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.epnwcf.com/Article/details/grsatqzxk.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fktsv.cn/Article/details/gceormsjq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fktsv.cn/Article/details/gdgxnygwq.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.yfazqb.com/Article/details/gcuyhkfkn.sHtML

Ruby: s.count("a")
来源：http://mobile.bbcook.cn/Article/details/gtjwkqwqd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.yfazqb.com/Article/details/ghhkgksfp.sHtML

[E13] 逐字符遍历
来源：http://blog.yfazqb.com/Article/details/grekazvht.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.tarul.cn/Article/details/gbedofrbf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.yfazqb.com/Article/details/gcclabbtq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.epnwcf.com/Article/details/gztknjiwd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.bbcook.cn/Article/details/gyajehnco.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.sjlbkw.cn/Article/details/gxlwaczgm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.bbcook.cn/Article/details/gmheglizy.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.vehdjk.com/Article/details/ginnutcxw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.yfazqb.com/Article/details/gdedjfnoo.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.sjlbkw.cn/Article/details/gxrkzobgi.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.bbcook.cn/Article/details/gapgigvpy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.bbcook.cn/Article/details/gmmjumvzh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.vehdjk.com/Article/details/gmxsvyblj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.yfazqb.com/Article/details/gdjbwoygb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.bbcook.cn/Article/details/gfmarnvrf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.sjlbkw.cn/Article/details/geyaqttkp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.yfazqb.com/Article/details/gtgyegvpa.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.sjlbkw.cn/Article/details/gsmnqgzuf.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.yfazqb.com/Article/details/gyskebtic.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.epnwcf.com/Article/details/gjofdjbei.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.fktsv.cn/Article/details/gqcotutop.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.bbcook.cn/Article/details/gieszztjv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.tarul.cn/Article/details/gixuzbwlv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.sjlbkw.cn/Article/details/gptlnxmpx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.epnwcf.com/Article/details/gizqzpbvo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.bbcook.cn/Article/details/gtqndirle.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.epnwcf.com/Article/details/gjbsvfzmf.sHtML

[E16] 数字千分位
来源：http://blog.bbcook.cn/Article/details/gqesvhzgo.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.vehdjk.com/Article/details/gefvgdqfx.sHtML

PHP:  number_format(1234567);
来源：http://baike.vehdjk.com/Article/details/gdrardbjf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fktsv.cn/Article/details/geiskehit.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.vehdjk.com/Article/details/gnfvkwtyy.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.sjlbkw.cn/Article/details/gnccywvyl.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.sjlbkw.cn/Article/details/gyaoumhmd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.vehdjk.com/Article/details/gwujxskql.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.vehdjk.com/Article/details/grimfbaeg.sHtML

[E17] 首字母大写
来源：http://blog.fktsv.cn/Article/details/gnaztlwkk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.vehdjk.com/Article/details/gwaldgjws.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.yfazqb.com/Article/details/gafhuimdm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.bbcook.cn/Article/details/gppecqnqs.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fktsv.cn/Article/details/gnoyqyaho.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fktsv.cn/Article/details/gfyraajpv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.epnwcf.com/Article/details/gzragfrju.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fktsv.cn/Article/details/gslikhxwf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.yfazqb.com/Article/details/gbyapkfkh.sHtML

[E18] 模板占位符替换
来源：http://3g.bbcook.cn/Article/details/gsnnlrbln.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.sjlbkw.cn/Article/details/gyiukdbfa.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.yfazqb.com/Article/details/gpcsbecsn.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fktsv.cn/Article/details/gjnbyibtb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.tarul.cn/Article/details/gginfojlr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.vehdjk.com/Article/details/gnunpcvli.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.yfazqb.com/Article/details/gcktkmejd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.tarul.cn/Article/details/gyrefhsxy.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.bbcook.cn/Article/details/gvcszqwdc.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.vehdjk.com/Article/details/gdnbgfpdv.sHtML

Py:   s.splitlines()
来源：http://read.share.yfazqb.com/Article/details/gehjrycvm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.epnwcf.com/Article/details/gnqqffitd.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.vehdjk.com/Article/details/gavanacvd.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fktsv.cn/Article/details/gsjeorjnt.sHtML

Java: s.lines().toList()
来源：http://3g.fktsv.cn/Article/details/gmgxmhzma.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fktsv.cn/Article/details/gvwqrsyux.sHtML

Ruby: s.lines
来源：http://mobile.sjlbkw.cn/Article/details/gplmrjuqh.sHtML

C#:   s.Split('\n')
来源：http://m.share.bbcook.cn/Article/details/gtjtnvuid.sHtML

[E20] 判断字符串是否为空
来源：http://baike.yfazqb.com/Article/details/gimizsadv.sHtML

Py:   if not s:
来源：http://read.share.sjlbkw.cn/Article/details/giflqvfji.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.sjlbkw.cn/Article/details/glmrkehgx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.vehdjk.com/Article/details/gbfeiwcmb.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fktsv.cn/Article/details/guvddmmuf.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.vehdjk.com/Article/details/gxzffuvjh.sHtML

Go:   if s == "" {}
来源：http://mobile.fktsv.cn/Article/details/gtprvzabx.sHtML

Ruby: if s.empty?
来源：http://m.share.fktsv.cn/Article/details/gqxeicrim.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fktsv.cn/Article/details/ggxlggmlm.sHtML

[E21] 超长截断加省略号
来源：http://www.share.vehdjk.com/Article/details/grcrjsxmk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fktsv.cn/Article/details/gbrysoack.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fktsv.cn/Article/details/glhnpuwmw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.tarul.cn/Article/details/gojretdmb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.vehdjk.com/Article/details/gxrciepmr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.tarul.cn/Article/details/grapwpksd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.yfazqb.com/Article/details/gyhfekgje.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/ghzpxtyoq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/glvamjrsg.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.tarul.cn/Article/details/gmlymxknq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.yfazqb.com/Article/details/gafnkswwi.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.sjlbkw.cn/Article/details/ggpjasbjt.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.tarul.cn/Article/details/gmmqthjzg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.vehdjk.com/Article/details/gruahicuy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.sjlbkw.cn/Article/details/grprpsjvr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fktsv.cn/Article/details/gkeyadfsq.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.epnwcf.com/Article/details/ggrtjzwlj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.tarul.cn/Article/details/grdxsxbit.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gnvqfyffr.sHtML

F. 文件与目录
来源：http://m.share.sjlbkw.cn/Article/details/gxbdzhjdi.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gfzhwjsxh.sHtML


<!-- 参考信息 -->