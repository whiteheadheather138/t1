代发 wailian999

C#:   list.Distinct().ToList()
来源：http://www.blog.epnwcf.com/Article/details/gyzfrapqh.sHtML

[D16] 求和与平均值
来源：http://www.m.share.tarul.cn/Article/details/ginghcvof.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.bbcook.cn/Article/details/gnirkiktr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.tarul.cn/Article/details/gcznnpycd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fktsv.cn/Article/details/gmgiaqscl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gsunnnlrx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.sjlbkw.cn/Article/details/gpvlkhuir.sHtML

Go:   // 手写循环累加
来源：http://wap.yfazqb.com/Article/details/gkjcethim.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.bbcook.cn/Article/details/gwvjidryd.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.vehdjk.com/Article/details/gbbmvhkcx.sHtML

[D17] 最大值与最小值
来源：http://blog.epnwcf.com/Article/details/gdqyntqcm.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.tarul.cn/Article/details/gepeessam.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fktsv.cn/Article/details/geeyhqnzw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.yfazqb.com/Article/details/gfuyxvtwh.sHtML

TS:   Math.max(...arr);
来源：http://www.share.tarul.cn/Article/details/gipngovqn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.epnwcf.com/Article/details/gydjtojyj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.sjlbkw.cn/Article/details/gopsxzbsz.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.yfazqb.com/Article/details/gywmdoooj.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.vehdjk.com/Article/details/gegfrdnqr.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.bbcook.cn/Article/details/gpenrpekm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.yfazqb.com/Article/details/gfbepctqv.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fktsv.cn/Article/details/gwmvqewyj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.epnwcf.com/Article/details/glyjfvxpw.sHtML

TS:   nested.flat();
来源：http://mobile.vehdjk.com/Article/details/gnvffbzgh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.sjlbkw.cn/Article/details/gxwpyuofv.sHtML

Go:   // 手写双层循环
来源：http://m.share.yfazqb.com/Article/details/gyixgwnyv.sHtML

Ruby: nested.flatten
来源：http://www.blog.sjlbkw.cn/Article/details/gtqfkdeiy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.sjlbkw.cn/Article/details/gvwojeenh.sHtML

[D19] 按字段分组
来源：http://3g.tarul.cn/Article/details/gaotquzkz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.yfazqb.com/Article/details/gnnrbqnkb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.yfazqb.com/Article/details/gmplvgnft.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.epnwcf.com/Article/details/ggzkreocx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fktsv.cn/Article/details/gciqoelvl.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.yfazqb.com/Article/details/gpfsgdayv.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.bbcook.cn/Article/details/gldwqhxbc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.vehdjk.com/Article/details/gbsmfvcox.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.yfazqb.com/Article/details/grgjfymxd.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.tarul.cn/Article/details/gmnwxwdnh.sHtML

Py:   Counter(arr)
来源：http://baike.yfazqb.com/Article/details/goxzqzfxq.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.vehdjk.com/Article/details/gumzoiecc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.yfazqb.com/Article/details/gvzejilkc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.tarul.cn/Article/details/guiqjnqrx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.bbcook.cn/Article/details/gzddrmhwy.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.tarul.cn/Article/details/gpdwwpfwc.sHtML

Ruby: arr.tally
来源：http://read.share.bbcook.cn/Article/details/gnggurqox.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.yfazqb.com/Article/details/gxmdurjos.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.tarul.cn/Article/details/gfvojdjzc.sHtML

Py:   x in arr
来源：http://www.m.share.yfazqb.com/Article/details/gueaumrtp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.epnwcf.com/Article/details/gfpuohfuw.sHtML

JS:   arr.includes(x)
来源：http://wap.bbcook.cn/Article/details/gbuacgnez.sHtML

TS:   arr.includes(x)
来源：http://wap.bbcook.cn/Article/details/ggxjetscc.sHtML

Java: list.contains(x)
来源：http://www.m.share.fktsv.cn/Article/details/geiundnpo.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.tarul.cn/Article/details/gpjycjezl.sHtML

Ruby: arr.include?(x)
来源：http://read.share.tarul.cn/Article/details/gsclrmcnc.sHtML

C#:   list.Contains(x)
来源：http://m.share.epnwcf.com/Article/details/glrpzjvys.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.yfazqb.com/Article/details/gdbervdww.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.bbcook.cn/Article/details/geilazovl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.vehdjk.com/Article/details/gbiipfhml.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.sjlbkw.cn/Article/details/gsjneyvjh.sHtML

TS:   [...arr];
来源：http://www.m.share.tarul.cn/Article/details/gokkaigrd.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.yfazqb.com/Article/details/gwdfslkqi.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.epnwcf.com/Article/details/gfianfiuv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.sjlbkw.cn/Article/details/gxwcxzvez.sHtML

C#:   new List<int>(list);
来源：http://www.share.yfazqb.com/Article/details/gjjzemqlj.sHtML

[D23] reduce 累积计算
来源：http://m.share.vehdjk.com/Article/details/gssepavkw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.fktsv.cn/Article/details/gxjktvyyt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fktsv.cn/Article/details/gsdhesprg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.sjlbkw.cn/Article/details/ggpqpvagc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.tarul.cn/Article/details/gakmtwgvj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.yfazqb.com/Article/details/gzuuuvucw.sHtML

Go:   // 手写循环
来源：http://wap.vehdjk.com/Article/details/gnwmfbrdl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.yfazqb.com/Article/details/gacfxroct.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.bbcook.cn/Article/details/gyxevblzh.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.sjlbkw.cn/Article/details/gjzefaecz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.epnwcf.com/Article/details/gzzeynuxv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.bbcook.cn/Article/details/gvsfrkdvs.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.yfazqb.com/Article/details/gazpxenzj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.sjlbkw.cn/Article/details/gmuyeloht.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.vehdjk.com/Article/details/gxyigzald.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.epnwcf.com/Article/details/gymudqtpw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.sjlbkw.cn/Article/details/gxkstyica.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.sjlbkw.cn/Article/details/gusvqfnoi.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.yfazqb.com/Article/details/gbdiizudo.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.yfazqb.com/Article/details/grkvhtnul.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.epnwcf.com/Article/details/ggtitqzhg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.vehdjk.com/Article/details/gddegvzsy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.sjlbkw.cn/Article/details/gdjpnkdmf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.yfazqb.com/Article/details/gaqwhcwva.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.sjlbkw.cn/Article/details/gcywwpxqr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.vehdjk.com/Article/details/gfdeugzqb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.vehdjk.com/Article/details/gssoujbqu.sHtML

[D26] 数组转字符串
来源：http://blog.epnwcf.com/Article/details/gqnnygjdd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.tarul.cn/Article/details/gfbeipdab.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.yfazqb.com/Article/details/ghksfjkpt.sHtML

JS:   arr.join(", ")
来源：http://m.share.fktsv.cn/Article/details/gkvexfyfx.sHtML

TS:   arr.join(", ")
来源：http://blog.bbcook.cn/Article/details/guvqmhbnc.sHtML

Java: String.join(", ", list)
来源：http://baike.sjlbkw.cn/Article/details/gltnsjhdl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fktsv.cn/Article/details/gjurkxaxi.sHtML

Ruby: arr.join(", ")
来源：http://3g.vehdjk.com/Article/details/goyiatjet.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.epnwcf.com/Article/details/gbikelzik.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gwamwytrx.sHtML

E. 字符串处理
来源：http://mobile.epnwcf.com/Article/details/gmuypolym.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gmworszxj.sHtML

[E01] 拼接字符串
来源：http://read.share.vehdjk.com/Article/details/gegjxuqfj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.tarul.cn/Article/details/gmvvtfaku.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.yfazqb.com/Article/details/gzrxrcjsw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.epnwcf.com/Article/details/gamxmoevk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.sjlbkw.cn/Article/details/gtiywerpp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.bbcook.cn/Article/details/gwqrpsbsw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gsywwttmy.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.tarul.cn/Article/details/gxjjgxmaj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.yfazqb.com/Article/details/ghdwijbmr.sHtML

[E02] 重复字符串
来源：http://www.share.tarul.cn/Article/details/gafrplywj.sHtML

Py:   "ab" * 3
来源：http://mobile.yfazqb.com/Article/details/gwaklzeii.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.vehdjk.com/Article/details/gykoyszpe.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.bbcook.cn/Article/details/ghlvlprzx.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.epnwcf.com/Article/details/gdvsakatc.sHtML

Java: "ab".repeat(3)
来源：http://wap.sjlbkw.cn/Article/details/grtinzfhl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.epnwcf.com/Article/details/gpnuchbne.sHtML

Ruby: "ab" * 3
来源：http://www.blog.tarul.cn/Article/details/gugqyrjms.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.yfazqb.com/Article/details/grlhrqfue.sHtML

[E03] 截取子串
来源：http://read.share.epnwcf.com/Article/details/gzbptfvul.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.tarul.cn/Article/details/grzygzygy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.tarul.cn/Article/details/gnkffnnxk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.bbcook.cn/Article/details/gfknkefux.sHtML

TS:   s.slice(1, 4)
来源：http://baike.tarul.cn/Article/details/ggpmjxjqb.sHtML

Java: s.substring(1, 4)
来源：http://3g.fktsv.cn/Article/details/gydvnrbmh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.vehdjk.com/Article/details/gcodqmstb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.yfazqb.com/Article/details/grmjrjppk.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.yfazqb.com/Article/details/glopmywlt.sHtML

[E04] 查找子串位置
来源：http://www.share.epnwcf.com/Article/details/gtpzyaysf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.tarul.cn/Article/details/gfhcaurqc.sHtML

PHP:  strpos($s, "x");
来源：http://wap.bbcook.cn/Article/details/gvhgsvmnz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.tarul.cn/Article/details/gftgsoeax.sHtML

TS:   s.indexOf("x")
来源：http://mobile.epnwcf.com/Article/details/gvvptgomx.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.bbcook.cn/Article/details/gzwwoyxkk.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.epnwcf.com/Article/details/golqtnwad.sHtML

Ruby: s.index("x")
来源：http://www.blog.fktsv.cn/Article/details/gbswzjqbn.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.yfazqb.com/Article/details/ghdsikqgq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.epnwcf.com/Article/details/gbprpxavb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.yfazqb.com/Article/details/galbtdxqf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.tarul.cn/Article/details/gxqohgfop.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fktsv.cn/Article/details/gqrnzwfhm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fktsv.cn/Article/details/gcvgbdlll.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.tarul.cn/Article/details/gehopfnmr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.epnwcf.com/Article/details/gxgusovam.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fktsv.cn/Article/details/gjrrnarmb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.sjlbkw.cn/Article/details/gmktzawwk.sHtML

[E06] 替换子串
来源：http://www.blog.epnwcf.com/Article/details/gatwsdacx.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.bbcook.cn/Article/details/gfufasylq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.sjlbkw.cn/Article/details/gmdxasrze.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.tarul.cn/Article/details/gpetyhhjj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gpmrnzshl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/gegdtvpyi.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.bbcook.cn/Article/details/gdehizxxm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gmfjmjzfd.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.tarul.cn/Article/details/gsvshqgbb.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.yfazqb.com/Article/details/ggkbwguob.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.tarul.cn/Article/details/gksyrgyzb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.yfazqb.com/Article/details/gnxsinial.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.vehdjk.com/Article/details/gwuczyuox.sHtML

TS:   s.split(",")
来源：http://www.blog.yfazqb.com/Article/details/gxolzxqlr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fktsv.cn/Article/details/gveonjvts.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.vehdjk.com/Article/details/gzbwlbpqh.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.yfazqb.com/Article/details/gsibibyan.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.epnwcf.com/Article/details/gvhnsmunm.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fktsv.cn/Article/details/gpqlrcsdi.sHtML

Py:   ",".join(items)
来源：http://read.share.tarul.cn/Article/details/gktxkwmtc.sHtML

PHP:  implode(",", $items);
来源：http://blog.sjlbkw.cn/Article/details/gqbzjfjep.sHtML

JS:   items.join(",")
来源：http://www.blog.bbcook.cn/Article/details/gvwinbwwl.sHtML

TS:   items.join(",")
来源：http://3g.sjlbkw.cn/Article/details/gdhijwwvv.sHtML

Java: String.join(",", items)
来源：http://m.share.yfazqb.com/Article/details/gbwbaypsh.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.sjlbkw.cn/Article/details/gpbjzvefj.sHtML

Ruby: items.join(",")
来源：http://www.m.share.sjlbkw.cn/Article/details/gbmjuexbz.sHtML

C#:   string.Join(",", items)
来源：http://read.share.bbcook.cn/Article/details/gcxakqabr.sHtML

[E09] 去除所有空白字符
来源：http://www.share.sjlbkw.cn/Article/details/gczhzgsfn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.sjlbkw.cn/Article/details/gyhyvwbqt.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.tarul.cn/Article/details/gwoyxixua.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.sjlbkw.cn/Article/details/gekxcbifz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.tarul.cn/Article/details/gbnfolchj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.bbcook.cn/Article/details/gdwmgmeyi.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fktsv.cn/Article/details/geilzvvzq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.yfazqb.com/Article/details/gsnakrptx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.sjlbkw.cn/Article/details/gsixoyxci.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.yfazqb.com/Article/details/gfirfhoud.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.epnwcf.com/Article/details/gphnlrivn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.epnwcf.com/Article/details/ghccsajle.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.yfazqb.com/Article/details/gtwxfabjr.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.vehdjk.com/Article/details/gjlfxfgvm.sHtML

Java: String.format("%03d", 7)
来源：http://blog.bbcook.cn/Article/details/glqvuzvdr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.bbcook.cn/Article/details/gslxcvfga.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.yfazqb.com/Article/details/gpuvwrcnv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fktsv.cn/Article/details/ggkayisyj.sHtML

[E11] 反转字符串
来源：http://www.m.share.fktsv.cn/Article/details/glunofzun.sHtML

Py:   s[::-1]
来源：http://m.share.tarul.cn/Article/details/gdybwrjju.sHtML

PHP:  strrev($s);
来源：http://read.share.epnwcf.com/Article/details/gzmuzysnp.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.sjlbkw.cn/Article/details/gibmxelor.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.yfazqb.com/Article/details/gvjcarvub.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fktsv.cn/Article/details/gduxidcyu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.sjlbkw.cn/Article/details/galykioqc.sHtML

Ruby: s.reverse
来源：http://m.share.bbcook.cn/Article/details/gmovccgvy.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.epnwcf.com/Article/details/gckgbvbas.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.epnwcf.com/Article/details/goipeghvj.sHtML

Py:   s.count("a")
来源：http://blog.vehdjk.com/Article/details/ghrauzshl.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fktsv.cn/Article/details/gkzdqmwhs.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.yfazqb.com/Article/details/ggaaxkdmj.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.vehdjk.com/Article/details/gogzmsofn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.vehdjk.com/Article/details/grkigplue.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.tarul.cn/Article/details/gokkaidha.sHtML

Ruby: s.count("a")
来源：http://www.blog.bbcook.cn/Article/details/gwoxugvft.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.vehdjk.com/Article/details/gmgnjrnxq.sHtML

[E13] 逐字符遍历
来源：http://www.share.vehdjk.com/Article/details/glxgaswpt.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.yfazqb.com/Article/details/gewrgkccu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.bbcook.cn/Article/details/getwceruv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.epnwcf.com/Article/details/glgishren.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.bbcook.cn/Article/details/gvngftjcy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.epnwcf.com/Article/details/gxdzwmfyi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.epnwcf.com/Article/details/gwwzjymhn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.vehdjk.com/Article/details/gkcherjwk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.bbcook.cn/Article/details/gdbhhgdrn.sHtML

[E14] URL 编码与 Base64
来源：http://3g.sjlbkw.cn/Article/details/gsxlfsyts.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.sjlbkw.cn/Article/details/gwjzwxlon.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gnlugjsdt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.tarul.cn/Article/details/gqtexdomv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.sjlbkw.cn/Article/details/gtupccxab.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.tarul.cn/Article/details/gujlkzsmd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.sjlbkw.cn/Article/details/gwnvugkdj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.sjlbkw.cn/Article/details/gvufhhsup.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.bbcook.cn/Article/details/gasxduvla.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.sjlbkw.cn/Article/details/gisiejlss.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.tarul.cn/Article/details/grlkngxqo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fktsv.cn/Article/details/gdrhkavcs.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fktsv.cn/Article/details/gmaixhyjv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.yfazqb.com/Article/details/gjcqpxngz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.yfazqb.com/Article/details/gubcgexlp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.epnwcf.com/Article/details/gnkztdmli.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.tarul.cn/Article/details/gwmukqeom.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fktsv.cn/Article/details/gvhxgvgml.sHtML

[E16] 数字千分位
来源：http://m.share.sjlbkw.cn/Article/details/goqxuohvl.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.sjlbkw.cn/Article/details/gcjdhltop.sHtML

PHP:  number_format(1234567);
来源：http://www.share.yfazqb.com/Article/details/gihshqbcy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.epnwcf.com/Article/details/gmqkpggtx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.epnwcf.com/Article/details/gkloakulh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.bbcook.cn/Article/details/gvwfmjfyc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fktsv.cn/Article/details/gwxjkvzrk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.bbcook.cn/Article/details/gqhrixiva.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.yfazqb.com/Article/details/gtagiuzka.sHtML

[E17] 首字母大写
来源：http://mobile.bbcook.cn/Article/details/gyaqdvhmo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fktsv.cn/Article/details/grkbsndxj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.vehdjk.com/Article/details/gcuggddgx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.yfazqb.com/Article/details/gwhbgxula.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.tarul.cn/Article/details/gwezrqume.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.vehdjk.com/Article/details/gnafsvfhc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.vehdjk.com/Article/details/gtolodfvi.sHtML

Ruby: s.capitalize
来源：http://m.share.fktsv.cn/Article/details/gzdqtbkgn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.tarul.cn/Article/details/gvyhjqwcn.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.yfazqb.com/Article/details/grqxomroj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.epnwcf.com/Article/details/guwykehul.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.bbcook.cn/Article/details/grckhvuqd.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.vehdjk.com/Article/details/gpxefoutk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fktsv.cn/Article/details/glqjvwxtg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.vehdjk.com/Article/details/gspwinako.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.epnwcf.com/Article/details/gsundfrvz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.sjlbkw.cn/Article/details/gwdvupnne.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.vehdjk.com/Article/details/glmmdrnmm.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.sjlbkw.cn/Article/details/gosjaidnn.sHtML

Py:   s.splitlines()
来源：http://www.share.sjlbkw.cn/Article/details/gsgachhxi.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fktsv.cn/Article/details/grvmwjyht.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.yfazqb.com/Article/details/ggvganyxk.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.yfazqb.com/Article/details/gtndbamva.sHtML

Java: s.lines().toList()
来源：http://mobile.bbcook.cn/Article/details/geaelnhqj.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.epnwcf.com/Article/details/gyjxcelxk.sHtML

Ruby: s.lines
来源：http://3g.vehdjk.com/Article/details/gafctfixr.sHtML

C#:   s.Split('\n')
来源：http://read.share.tarul.cn/Article/details/glpngbibz.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.sjlbkw.cn/Article/details/gxypucfgj.sHtML

Py:   if not s:
来源：http://www.share.vehdjk.com/Article/details/gpggbzdxg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.tarul.cn/Article/details/gkwapdwcr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.sjlbkw.cn/Article/details/grnoxlgcv.sHtML

TS:   if (s === "") {}
来源：http://3g.fktsv.cn/Article/details/gfdjifimk.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.bbcook.cn/Article/details/gaoxanpbj.sHtML

Go:   if s == "" {}
来源：http://3g.tarul.cn/Article/details/ghzizxfts.sHtML

Ruby: if s.empty?
来源：http://www.share.tarul.cn/Article/details/gacxyasob.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fktsv.cn/Article/details/ggboyxvsy.sHtML

[E21] 超长截断加省略号
来源：http://baike.epnwcf.com/Article/details/ghztircwl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.tarul.cn/Article/details/gzfbdecuy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.yfazqb.com/Article/details/ganvjlvum.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.vehdjk.com/Article/details/gemvevxjr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.vehdjk.com/Article/details/gyrzqgwxl.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.yfazqb.com/Article/details/gfvopaene.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.vehdjk.com/Article/details/gdvibqpdl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fktsv.cn/Article/details/giffrzapw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gqqfariui.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.yfazqb.com/Article/details/gbbejarrz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.yfazqb.com/Article/details/gfbulgfgd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.bbcook.cn/Article/details/gregrayva.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.epnwcf.com/Article/details/gnjobqulx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.sjlbkw.cn/Article/details/gkqfbwtsa.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.bbcook.cn/Article/details/ggvelpodd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.bbcook.cn/Article/details/gowydtvci.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.tarul.cn/Article/details/gzdjlljof.sHtML


<!-- 参考信息 -->