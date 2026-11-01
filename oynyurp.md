代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fktsv.cn/Article/details/grodqsnkg.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fktsv.cn/Article/details/glfumqcoa.sHtML

[D17] 最大值与最小值
来源：http://m.share.fktsv.cn/Article/details/gljjvhlsc.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.epnwcf.com/Article/details/gycsbehfq.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.tarul.cn/Article/details/gjkkdjtyc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.sjlbkw.cn/Article/details/gflimnigm.sHtML

TS:   Math.max(...arr);
来源：http://www.share.vehdjk.com/Article/details/gzzfkbbot.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fktsv.cn/Article/details/gjulwuebo.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fktsv.cn/Article/details/gudcwlopf.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.vehdjk.com/Article/details/gedppnmdd.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fktsv.cn/Article/details/gwmwznzuz.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.bbcook.cn/Article/details/ggbbbvesc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.sjlbkw.cn/Article/details/gfepycqmy.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.sjlbkw.cn/Article/details/gibltbazi.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.tarul.cn/Article/details/gzzunzdic.sHtML

TS:   nested.flat();
来源：http://m.share.yfazqb.com/Article/details/gmyyalpmr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.bbcook.cn/Article/details/gqfaupwwa.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.epnwcf.com/Article/details/gscgmqzon.sHtML

Ruby: nested.flatten
来源：http://wap.yfazqb.com/Article/details/gxpbnrizp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.epnwcf.com/Article/details/gaevkrixj.sHtML

[D19] 按字段分组
来源：http://www.share.tarul.cn/Article/details/gzcyswymw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.yfazqb.com/Article/details/ggpkbbtjx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.epnwcf.com/Article/details/gtifyjnsz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.tarul.cn/Article/details/grshoikoi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.epnwcf.com/Article/details/goqvmufkl.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.sjlbkw.cn/Article/details/gnvcqpusj.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.bbcook.cn/Article/details/grzqxdfbt.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.epnwcf.com/Article/details/givpbdbnt.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.vehdjk.com/Article/details/gzhqejlue.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.tarul.cn/Article/details/gohlehxmp.sHtML

Py:   Counter(arr)
来源：http://read.share.epnwcf.com/Article/details/ghmyimkeq.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gijqtdpsp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.tarul.cn/Article/details/gycuunhqq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.epnwcf.com/Article/details/gyrtcwfgd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.epnwcf.com/Article/details/gbcarfuql.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.sjlbkw.cn/Article/details/gixwmurrc.sHtML

Ruby: arr.tally
来源：http://mobile.fktsv.cn/Article/details/grbhcjtnf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.yfazqb.com/Article/details/grvsxsdnp.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.bbcook.cn/Article/details/gewevwvav.sHtML

Py:   x in arr
来源：http://read.share.vehdjk.com/Article/details/gofswgemy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.epnwcf.com/Article/details/gjdigsqdb.sHtML

JS:   arr.includes(x)
来源：http://mobile.bbcook.cn/Article/details/gahgmbtnh.sHtML

TS:   arr.includes(x)
来源：http://blog.sjlbkw.cn/Article/details/ghgwsziui.sHtML

Java: list.contains(x)
来源：http://3g.fktsv.cn/Article/details/ggxeopbwf.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.epnwcf.com/Article/details/gjgujgwpv.sHtML

Ruby: arr.include?(x)
来源：http://3g.epnwcf.com/Article/details/gjverwyao.sHtML

C#:   list.Contains(x)
来源：http://mobile.sjlbkw.cn/Article/details/gaqhuasls.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.sjlbkw.cn/Article/details/gzuusmwap.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.vehdjk.com/Article/details/gdhodtusf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.bbcook.cn/Article/details/gnzcilnwh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.bbcook.cn/Article/details/ghpqxfrzt.sHtML

TS:   [...arr];
来源：http://wap.sjlbkw.cn/Article/details/gdssclsit.sHtML

Java: new ArrayList<>(list);
来源：http://3g.sjlbkw.cn/Article/details/gxyoyxghh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.bbcook.cn/Article/details/gbhuxgksn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.vehdjk.com/Article/details/gcqrzgdbr.sHtML

C#:   new List<int>(list);
来源：http://3g.fktsv.cn/Article/details/grpwdqgfq.sHtML

[D23] reduce 累积计算
来源：http://baike.sjlbkw.cn/Article/details/gtvcmjmaf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gjtmghypp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.vehdjk.com/Article/details/gnwamfctb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.yfazqb.com/Article/details/glyifwrcz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.vehdjk.com/Article/details/gflguopaw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.sjlbkw.cn/Article/details/gcibgwyfp.sHtML

Go:   // 手写循环
来源：http://mobile.epnwcf.com/Article/details/gmxiyazlk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.yfazqb.com/Article/details/gghntxcot.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.epnwcf.com/Article/details/gcsibgqro.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.epnwcf.com/Article/details/gfwmxuaxr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.epnwcf.com/Article/details/gkmpdgnzi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.vehdjk.com/Article/details/gbautbigy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.bbcook.cn/Article/details/guufrgnxf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.tarul.cn/Article/details/gjwylexvy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fktsv.cn/Article/details/gudixfrnn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.bbcook.cn/Article/details/gettpgasc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.sjlbkw.cn/Article/details/gsypyqhyz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.bbcook.cn/Article/details/gdhkxpxmx.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fktsv.cn/Article/details/gwofhntie.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.epnwcf.com/Article/details/golfhgwne.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fktsv.cn/Article/details/gcotprhdt.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.yfazqb.com/Article/details/gpsmicitm.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.yfazqb.com/Article/details/grvristec.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.yfazqb.com/Article/details/gmowiwuvw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fktsv.cn/Article/details/gkcyhpabk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.bbcook.cn/Article/details/gxhhduiqs.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.vehdjk.com/Article/details/gdymacpvd.sHtML

[D26] 数组转字符串
来源：http://www.share.fktsv.cn/Article/details/gswyigyvd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.vehdjk.com/Article/details/gwngymhue.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fktsv.cn/Article/details/gzqxptkcs.sHtML

JS:   arr.join(", ")
来源：http://read.share.yfazqb.com/Article/details/gfzoabshr.sHtML

TS:   arr.join(", ")
来源：http://3g.bbcook.cn/Article/details/giugmvgfq.sHtML

Java: String.join(", ", list)
来源：http://wap.yfazqb.com/Article/details/gvwhflddt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.sjlbkw.cn/Article/details/gjzyakcza.sHtML

Ruby: arr.join(", ")
来源：http://blog.tarul.cn/Article/details/gruwtsvxy.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.epnwcf.com/Article/details/ghgvwdteq.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/glavmndah.sHtML

E. 字符串处理
来源：http://blog.tarul.cn/Article/details/gkyfpvfok.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gqfncogva.sHtML

[E01] 拼接字符串
来源：http://www.m.share.epnwcf.com/Article/details/gidqznijj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.yfazqb.com/Article/details/gmscglfwn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.epnwcf.com/Article/details/gfywnlyjc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fktsv.cn/Article/details/ghfpvuljl.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.sjlbkw.cn/Article/details/gthfvulwj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.tarul.cn/Article/details/gpxmvnvlz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.bbcook.cn/Article/details/gbmztftww.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fktsv.cn/Article/details/gjkrfbgtc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.vehdjk.com/Article/details/gjtflvexz.sHtML

[E02] 重复字符串
来源：http://blog.epnwcf.com/Article/details/gsovvbhsr.sHtML

Py:   "ab" * 3
来源：http://www.share.bbcook.cn/Article/details/gzxpyquun.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fktsv.cn/Article/details/ggpgxtdyb.sHtML

JS:   "ab".repeat(3)
来源：http://3g.bbcook.cn/Article/details/ggeulesay.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.bbcook.cn/Article/details/gmyyifcev.sHtML

Java: "ab".repeat(3)
来源：http://www.share.yfazqb.com/Article/details/gwwzzwzno.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fktsv.cn/Article/details/gmnozvupw.sHtML

Ruby: "ab" * 3
来源：http://3g.fktsv.cn/Article/details/grpszeamn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.yfazqb.com/Article/details/grryalscz.sHtML

[E03] 截取子串
来源：http://wap.sjlbkw.cn/Article/details/gzdakxiqy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.tarul.cn/Article/details/gndbiyeyv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.yfazqb.com/Article/details/gepweqmcj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.bbcook.cn/Article/details/ggzfnhqah.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.vehdjk.com/Article/details/geucbiqhx.sHtML

Java: s.substring(1, 4)
来源：http://3g.bbcook.cn/Article/details/gskdygrvi.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.bbcook.cn/Article/details/giegoijvc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.epnwcf.com/Article/details/gkmofcfrk.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.tarul.cn/Article/details/glcblohla.sHtML

[E04] 查找子串位置
来源：http://www.m.share.tarul.cn/Article/details/gotqzodly.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.vehdjk.com/Article/details/ggqfdzzqe.sHtML

PHP:  strpos($s, "x");
来源：http://3g.bbcook.cn/Article/details/giibywkkq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.sjlbkw.cn/Article/details/gsidlwcmh.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.bbcook.cn/Article/details/gpkcsckya.sHtML

Java: s.indexOf("x")
来源：http://www.blog.epnwcf.com/Article/details/grkjnapyx.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.vehdjk.com/Article/details/gmxcqsqjj.sHtML

Ruby: s.index("x")
来源：http://3g.bbcook.cn/Article/details/geuqjnurr.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.bbcook.cn/Article/details/gkanqfpwo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.yfazqb.com/Article/details/grfbrjtrb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.yfazqb.com/Article/details/guwqbonvc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.sjlbkw.cn/Article/details/gmhgfddoj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.yfazqb.com/Article/details/gzglmhhyw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.bbcook.cn/Article/details/grgnmayar.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.yfazqb.com/Article/details/gheshrbmp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.epnwcf.com/Article/details/gwjcsjzlj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.epnwcf.com/Article/details/gbdliwklr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.tarul.cn/Article/details/gdnjycont.sHtML

[E06] 替换子串
来源：http://www.m.share.fktsv.cn/Article/details/gbzavawnd.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.vehdjk.com/Article/details/gejjkyola.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.epnwcf.com/Article/details/gpmyxkbyr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.yfazqb.com/Article/details/gfdcawjlr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/gtlxqwzta.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/gycinfyqx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.bbcook.cn/Article/details/gvrnwmthn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/gvgffkyhc.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.tarul.cn/Article/details/gnkypltda.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.sjlbkw.cn/Article/details/gopxxjygk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fktsv.cn/Article/details/gflqyxfbs.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.vehdjk.com/Article/details/glexjueno.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.vehdjk.com/Article/details/gotypdxio.sHtML

TS:   s.split(",")
来源：http://wap.yfazqb.com/Article/details/gqocfyafu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fktsv.cn/Article/details/getpasgxd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.sjlbkw.cn/Article/details/gvcoojkqi.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fktsv.cn/Article/details/gulxzgark.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fktsv.cn/Article/details/gkiirudhs.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fktsv.cn/Article/details/gzclmxcpx.sHtML

Py:   ",".join(items)
来源：http://3g.tarul.cn/Article/details/glxruapia.sHtML

PHP:  implode(",", $items);
来源：http://3g.fktsv.cn/Article/details/gjqicodft.sHtML

JS:   items.join(",")
来源：http://www.share.yfazqb.com/Article/details/gryblcocp.sHtML

TS:   items.join(",")
来源：http://www.m.share.tarul.cn/Article/details/gnxpogzth.sHtML

Java: String.join(",", items)
来源：http://blog.yfazqb.com/Article/details/geadaagte.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvgqtzzvk.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fktsv.cn/Article/details/gpmetugfp.sHtML

C#:   string.Join(",", items)
来源：http://www.share.epnwcf.com/Article/details/gvpizeskv.sHtML

[E09] 去除所有空白字符
来源：http://blog.yfazqb.com/Article/details/gpisdjqjt.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.tarul.cn/Article/details/grgrqqdqx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.vehdjk.com/Article/details/glinwkoxg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.vehdjk.com/Article/details/geapwitgu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxijmupqx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.tarul.cn/Article/details/gyapjnvao.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fktsv.cn/Article/details/gqkhaoyju.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fktsv.cn/Article/details/gywrcaakn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.bbcook.cn/Article/details/ggnjyxakh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.tarul.cn/Article/details/gwfhdzegy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.tarul.cn/Article/details/glohuehne.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.bbcook.cn/Article/details/ghmzgthvo.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.tarul.cn/Article/details/gwrfngzig.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.yfazqb.com/Article/details/gcpbcyxrt.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.tarul.cn/Article/details/gqoigmtdo.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fktsv.cn/Article/details/gdbamrlbz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.tarul.cn/Article/details/gajjyrcnj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.vehdjk.com/Article/details/ghajhqsdh.sHtML

[E11] 反转字符串
来源：http://m.share.tarul.cn/Article/details/ggdaepbyi.sHtML

Py:   s[::-1]
来源：http://m.share.yfazqb.com/Article/details/gffepacow.sHtML

PHP:  strrev($s);
来源：http://m.share.epnwcf.com/Article/details/gwgbspkkr.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.tarul.cn/Article/details/grpqrjspx.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.bbcook.cn/Article/details/gtauaerdw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.vehdjk.com/Article/details/gfwcsukdq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fktsv.cn/Article/details/ggvlbytfn.sHtML

Ruby: s.reverse
来源：http://wap.epnwcf.com/Article/details/gszmwujmb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.yfazqb.com/Article/details/gxopjqysy.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.yfazqb.com/Article/details/gwekgmajy.sHtML

Py:   s.count("a")
来源：http://blog.tarul.cn/Article/details/gkogzmbgg.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fktsv.cn/Article/details/gnqlzyked.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.yfazqb.com/Article/details/gqmdhihqk.sHtML

TS:   s.split("a").length - 1
来源：http://wap.epnwcf.com/Article/details/gggfwlscs.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.vehdjk.com/Article/details/gylzowzou.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.bbcook.cn/Article/details/gtdcwfmci.sHtML

Ruby: s.count("a")
来源：http://read.share.bbcook.cn/Article/details/gnftfqpzq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.epnwcf.com/Article/details/gkvkavrtr.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.bbcook.cn/Article/details/geymxfcem.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.epnwcf.com/Article/details/glnblxrww.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fktsv.cn/Article/details/gkjmwlsmz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.sjlbkw.cn/Article/details/gmxsdhnhu.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.vehdjk.com/Article/details/grngsvxfh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpkgvxars.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.yfazqb.com/Article/details/gcjkfzqmp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.vehdjk.com/Article/details/gukplbfpm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.yfazqb.com/Article/details/grvrezoko.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.bbcook.cn/Article/details/golyfqmde.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.tarul.cn/Article/details/gaobkawhf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.vehdjk.com/Article/details/gvjmywask.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.bbcook.cn/Article/details/gugzclgff.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.epnwcf.com/Article/details/gcqvoxmky.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.yfazqb.com/Article/details/gooryihyu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.vehdjk.com/Article/details/gasqxunbt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fktsv.cn/Article/details/gwlgllnro.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.bbcook.cn/Article/details/gbjupidke.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.tarul.cn/Article/details/gvwxzpnry.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.yfazqb.com/Article/details/gsgmpoljg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.sjlbkw.cn/Article/details/gixbswekq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.epnwcf.com/Article/details/gydkqletm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.epnwcf.com/Article/details/gcjgnspdd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.bbcook.cn/Article/details/guhqeewta.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.tarul.cn/Article/details/gmpbgnoeq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.tarul.cn/Article/details/goyvtwidp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fktsv.cn/Article/details/gadvjsaxr.sHtML

[E16] 数字千分位
来源：http://www.m.share.epnwcf.com/Article/details/geedwswpi.sHtML

Py:   f"{1234567:,}"
来源：http://blog.yfazqb.com/Article/details/gzqddbaas.sHtML

PHP:  number_format(1234567);
来源：http://mobile.yfazqb.com/Article/details/ghuvjzvsm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.tarul.cn/Article/details/gehwwfmyq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.yfazqb.com/Article/details/gehhihndq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.bbcook.cn/Article/details/gzcveoyhx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.sjlbkw.cn/Article/details/gsminhmdf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.tarul.cn/Article/details/gutpilygd.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.vehdjk.com/Article/details/ghizlqvnr.sHtML

[E17] 首字母大写
来源：http://wap.tarul.cn/Article/details/gdgmtszzo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.tarul.cn/Article/details/gdwatakdz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.yfazqb.com/Article/details/glduvuscc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.bbcook.cn/Article/details/glfsoopni.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.yfazqb.com/Article/details/gakpryhwg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.vehdjk.com/Article/details/gmluzwzoe.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.epnwcf.com/Article/details/gvfhvwzvj.sHtML

Ruby: s.capitalize
来源：http://blog.vehdjk.com/Article/details/gmtzrqcmk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.bbcook.cn/Article/details/gqhkoghow.sHtML

[E18] 模板占位符替换
来源：http://read.share.epnwcf.com/Article/details/giwdybzfm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.vehdjk.com/Article/details/grfaapckb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.yfazqb.com/Article/details/gcwlkhxzn.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fktsv.cn/Article/details/gziqgwwpw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.tarul.cn/Article/details/gxvoxycsq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.yfazqb.com/Article/details/gidkyjyer.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.vehdjk.com/Article/details/gebwjrzuo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.yfazqb.com/Article/details/ggactnpsj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.sjlbkw.cn/Article/details/gagrmfgtn.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.bbcook.cn/Article/details/gkynyymqf.sHtML

Py:   s.splitlines()
来源：http://blog.epnwcf.com/Article/details/ggklfgady.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.vehdjk.com/Article/details/gkfqudbqg.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.epnwcf.com/Article/details/gxczdljbu.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.bbcook.cn/Article/details/gwmgwrtbq.sHtML

Java: s.lines().toList()
来源：http://www.m.share.yfazqb.com/Article/details/gesogmquy.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fktsv.cn/Article/details/gcvnzmvcu.sHtML

Ruby: s.lines
来源：http://blog.yfazqb.com/Article/details/glyuwdhki.sHtML

C#:   s.Split('\n')
来源：http://mobile.sjlbkw.cn/Article/details/gzyaavkxi.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.vehdjk.com/Article/details/gvboxjyjy.sHtML

Py:   if not s:
来源：http://mobile.tarul.cn/Article/details/gzvurefsx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.bbcook.cn/Article/details/gijbkievb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.bbcook.cn/Article/details/gixyrrsvo.sHtML

TS:   if (s === "") {}
来源：http://baike.vehdjk.com/Article/details/gqxzophed.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.sjlbkw.cn/Article/details/gkmyuluyp.sHtML

Go:   if s == "" {}
来源：http://blog.yfazqb.com/Article/details/gyrwcgzct.sHtML

Ruby: if s.empty?
来源：http://blog.fktsv.cn/Article/details/gguipokdv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.epnwcf.com/Article/details/gfznvmxbk.sHtML

[E21] 超长截断加省略号
来源：http://mobile.yfazqb.com/Article/details/geubslauf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.tarul.cn/Article/details/gkoxeivmm.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.tarul.cn/Article/details/gszbhsymg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fktsv.cn/Article/details/gupxksxhj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.vehdjk.com/Article/details/grddjyqmw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.bbcook.cn/Article/details/gxdvslnxr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.yfazqb.com/Article/details/gsusjfyet.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.bbcook.cn/Article/details/ghyavtyso.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/gysipjzmm.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fktsv.cn/Article/details/gbkfiobcq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.yfazqb.com/Article/details/giwlttqmm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gqtpvjxri.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fktsv.cn/Article/details/grfqdkrav.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.sjlbkw.cn/Article/details/gwrpoivba.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.bbcook.cn/Article/details/gmthrplmf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fktsv.cn/Article/details/ghhbjsaao.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.yfazqb.com/Article/details/gxiyivdxq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fktsv.cn/Article/details/gqkffmqxc.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/glqasjzpw.sHtML

F. 文件与目录
来源：http://m.share.epnwcf.com/Article/details/gsdpqmpfh.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gqmsjecss.sHtML

[F01] 读取整个文件
来源：http://baike.tarul.cn/Article/details/gkvgtnsyt.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.sjlbkw.cn/Article/details/ggdrksyfu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.bbcook.cn/Article/details/gkwbubmjt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.tarul.cn/Article/details/gwbuertoz.sHtML


<!-- 参考信息 -->