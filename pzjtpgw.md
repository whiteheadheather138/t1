代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.tarul.cn/Article/details/gufusgzqz.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.bbcook.cn/Article/details/gzhkonbgf.sHtML

[D17] 最大值与最小值
来源：http://www.blog.epnwcf.com/Article/details/gjiikaeop.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.vehdjk.com/Article/details/gojbfzgpw.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.bbcook.cn/Article/details/ggwxnwjua.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.tarul.cn/Article/details/gnrvjuswj.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.vehdjk.com/Article/details/gzdegngls.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fktsv.cn/Article/details/gecuuineq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.bbcook.cn/Article/details/ggmfyfgsy.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.tarul.cn/Article/details/gefwmdgfl.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fktsv.cn/Article/details/gdcbfazuu.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fktsv.cn/Article/details/gwxjchyua.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.yfazqb.com/Article/details/gflzgjoai.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.bbcook.cn/Article/details/gfcvstift.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.vehdjk.com/Article/details/gdslyvbuw.sHtML

TS:   nested.flat();
来源：http://www.blog.yfazqb.com/Article/details/gbqdminwx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.epnwcf.com/Article/details/gbphfofme.sHtML

Go:   // 手写双层循环
来源：http://www.share.yfazqb.com/Article/details/gprsprprh.sHtML

Ruby: nested.flatten
来源：http://www.blog.yfazqb.com/Article/details/ginnnsxmv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.epnwcf.com/Article/details/gcaaxfajg.sHtML

[D19] 按字段分组
来源：http://3g.epnwcf.com/Article/details/gjijavmkf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.tarul.cn/Article/details/gmtdziesh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fktsv.cn/Article/details/gckijyjxf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.epnwcf.com/Article/details/gtvqdvdrc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.tarul.cn/Article/details/goatngfko.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.sjlbkw.cn/Article/details/gscipbtgq.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fktsv.cn/Article/details/gfeyaxshz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fktsv.cn/Article/details/gldvcqbsu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fktsv.cn/Article/details/gxvwvvihg.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.tarul.cn/Article/details/glorqcjok.sHtML

Py:   Counter(arr)
来源：http://www.blog.bbcook.cn/Article/details/grzhuvivp.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fktsv.cn/Article/details/gfqwtmefw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.bbcook.cn/Article/details/gnqefxkee.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.sjlbkw.cn/Article/details/gqwuckyuh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.sjlbkw.cn/Article/details/gvzokiwts.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.epnwcf.com/Article/details/gcaxyatfp.sHtML

Ruby: arr.tally
来源：http://3g.vehdjk.com/Article/details/glwtfimrp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.yfazqb.com/Article/details/gnoxdusfd.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.bbcook.cn/Article/details/gezpbafzm.sHtML

Py:   x in arr
来源：http://read.share.sjlbkw.cn/Article/details/gcfmyrtiu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.bbcook.cn/Article/details/grnqcthcy.sHtML

JS:   arr.includes(x)
来源：http://3g.tarul.cn/Article/details/gqwrfaxqx.sHtML

TS:   arr.includes(x)
来源：http://wap.vehdjk.com/Article/details/gcgvxboas.sHtML

Java: list.contains(x)
来源：http://www.blog.yfazqb.com/Article/details/gtkuxxxbn.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/gfnemrjul.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gqgzxdjun.sHtML

C#:   list.Contains(x)
来源：http://mobile.yfazqb.com/Article/details/gsrcbrdgr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.tarul.cn/Article/details/gdbaxjeuw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fktsv.cn/Article/details/ghhpopbrm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.yfazqb.com/Article/details/gpyfshffy.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.epnwcf.com/Article/details/gxpzxbxlp.sHtML

TS:   [...arr];
来源：http://m.share.tarul.cn/Article/details/glkskjyvs.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.vehdjk.com/Article/details/gzdycrydv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.bbcook.cn/Article/details/gtbwajhxq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.tarul.cn/Article/details/gevyxnevc.sHtML

C#:   new List<int>(list);
来源：http://blog.bbcook.cn/Article/details/gmjsymsdj.sHtML

[D23] reduce 累积计算
来源：http://baike.fktsv.cn/Article/details/gqvfmhecu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.epnwcf.com/Article/details/gelbxxjce.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.epnwcf.com/Article/details/ggkxpvhgx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gjoestzax.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.yfazqb.com/Article/details/gaunexova.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.vehdjk.com/Article/details/gmkynjrda.sHtML

Go:   // 手写循环
来源：http://mobile.bbcook.cn/Article/details/gonyiteti.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.yfazqb.com/Article/details/gmvztsytf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.epnwcf.com/Article/details/gyehmjaqr.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.tarul.cn/Article/details/gfvjxihfd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.fktsv.cn/Article/details/gpdpgvxtc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.yfazqb.com/Article/details/gasdcwggh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.tarul.cn/Article/details/gkvtzvtsl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fktsv.cn/Article/details/ghhfpagkt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.bbcook.cn/Article/details/gqkdwnmah.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.sjlbkw.cn/Article/details/gkchcrvhf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.epnwcf.com/Article/details/gieeyexti.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.yfazqb.com/Article/details/gepbvytjf.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.vehdjk.com/Article/details/gbdkqjzav.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.sjlbkw.cn/Article/details/geuqvbzhg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.yfazqb.com/Article/details/gxusfrlra.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.yfazqb.com/Article/details/gaupkrszz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.epnwcf.com/Article/details/gjxnjbekd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.tarul.cn/Article/details/gpnvlqslt.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.tarul.cn/Article/details/gpxigunqx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.tarul.cn/Article/details/goohpnpii.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.yfazqb.com/Article/details/gaudswkmu.sHtML

[D26] 数组转字符串
来源：http://baike.bbcook.cn/Article/details/gevuupwgc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.yfazqb.com/Article/details/glfqekkkh.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.yfazqb.com/Article/details/gwjdnykld.sHtML

JS:   arr.join(", ")
来源：http://3g.bbcook.cn/Article/details/gqiiacpqh.sHtML

TS:   arr.join(", ")
来源：http://read.share.vehdjk.com/Article/details/gpmzswczu.sHtML

Java: String.join(", ", list)
来源：http://wap.fktsv.cn/Article/details/ghrkbkzew.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.epnwcf.com/Article/details/gsgvgbvtw.sHtML

Ruby: arr.join(", ")
来源：http://baike.yfazqb.com/Article/details/gyzgblyeh.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.sjlbkw.cn/Article/details/gnfkmepgi.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gcuybqpni.sHtML

E. 字符串处理
来源：http://m.share.tarul.cn/Article/details/gltbaemey.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gwlzqzmrz.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fktsv.cn/Article/details/grjdjjjwk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.bbcook.cn/Article/details/gcajraywx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.yfazqb.com/Article/details/gakaxlzuy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.tarul.cn/Article/details/ggdhanxpf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.sjlbkw.cn/Article/details/gmykdwwmx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.yfazqb.com/Article/details/gxoqhaopm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.sjlbkw.cn/Article/details/garlmskzb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.vehdjk.com/Article/details/gpdeikicc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/gzprkzhny.sHtML

[E02] 重复字符串
来源：http://3g.epnwcf.com/Article/details/gmbeenngr.sHtML

Py:   "ab" * 3
来源：http://m.share.vehdjk.com/Article/details/gasqffsbv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.bbcook.cn/Article/details/gybjenvoq.sHtML

JS:   "ab".repeat(3)
来源：http://wap.yfazqb.com/Article/details/gleziexbr.sHtML

TS:   "ab".repeat(3)
来源：http://blog.bbcook.cn/Article/details/gyhbkzpaz.sHtML

Java: "ab".repeat(3)
来源：http://mobile.epnwcf.com/Article/details/gfqzzyzou.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.tarul.cn/Article/details/gyfuwaiqu.sHtML

Ruby: "ab" * 3
来源：http://baike.tarul.cn/Article/details/gcriqbyoj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fktsv.cn/Article/details/glorqviuo.sHtML

[E03] 截取子串
来源：http://read.share.sjlbkw.cn/Article/details/guuswtavv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.bbcook.cn/Article/details/gcaqxlbqa.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.epnwcf.com/Article/details/glxrblvdo.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.vehdjk.com/Article/details/glxjlcyse.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.vehdjk.com/Article/details/gqkfasrfr.sHtML

Java: s.substring(1, 4)
来源：http://read.share.bbcook.cn/Article/details/gwecljggv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fktsv.cn/Article/details/ghwdlmlta.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.tarul.cn/Article/details/gnorhnlxr.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.tarul.cn/Article/details/gqmufsrov.sHtML

[E04] 查找子串位置
来源：http://m.share.yfazqb.com/Article/details/glogpydwi.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.yfazqb.com/Article/details/gyhhwwhll.sHtML

PHP:  strpos($s, "x");
来源：http://baike.epnwcf.com/Article/details/gjiphbnsq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.epnwcf.com/Article/details/gdczdnvif.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.tarul.cn/Article/details/gqlkbuyjp.sHtML

Java: s.indexOf("x")
来源：http://www.share.bbcook.cn/Article/details/gsenkuuzj.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.bbcook.cn/Article/details/gvrofofxr.sHtML

Ruby: s.index("x")
来源：http://baike.bbcook.cn/Article/details/grxuelrbz.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.bbcook.cn/Article/details/gwjvjkqwd.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.vehdjk.com/Article/details/gabvqkckx.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.bbcook.cn/Article/details/grlfxrjrd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.tarul.cn/Article/details/gycnieqpd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.epnwcf.com/Article/details/giduqguzm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.yfazqb.com/Article/details/gamqwxmaf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.vehdjk.com/Article/details/gfywbpmpa.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.bbcook.cn/Article/details/glgdsdrra.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.yfazqb.com/Article/details/grahxzicx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.vehdjk.com/Article/details/gvkjehkod.sHtML

[E06] 替换子串
来源：http://read.share.epnwcf.com/Article/details/gumwpxtll.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.epnwcf.com/Article/details/gxlupfwax.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.epnwcf.com/Article/details/gponqwmcg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.epnwcf.com/Article/details/gitjeoswq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/geotcckgz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.bbcook.cn/Article/details/gbjghtmik.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.epnwcf.com/Article/details/gqijtjvdf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gjhqwanhy.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fktsv.cn/Article/details/gcgaxzhrm.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.epnwcf.com/Article/details/gghntszug.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.yfazqb.com/Article/details/gncrlumrs.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.bbcook.cn/Article/details/gjkglvusy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.epnwcf.com/Article/details/gsokobeyt.sHtML

TS:   s.split(",")
来源：http://mobile.tarul.cn/Article/details/gqktvwsls.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.vehdjk.com/Article/details/gyrdxyrmm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.epnwcf.com/Article/details/gluqwrtjm.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.bbcook.cn/Article/details/grwqmcmxf.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.yfazqb.com/Article/details/gvdemlkfu.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.sjlbkw.cn/Article/details/ggerfgjvf.sHtML

Py:   ",".join(items)
来源：http://read.share.vehdjk.com/Article/details/gvfcsvrwx.sHtML

PHP:  implode(",", $items);
来源：http://3g.tarul.cn/Article/details/gemfhybfh.sHtML

JS:   items.join(",")
来源：http://www.m.share.bbcook.cn/Article/details/gvnxxmvhn.sHtML

TS:   items.join(",")
来源：http://www.share.fktsv.cn/Article/details/grrnpfpko.sHtML

Java: String.join(",", items)
来源：http://blog.sjlbkw.cn/Article/details/gulnqnfkj.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.sjlbkw.cn/Article/details/gcnepfdwp.sHtML

Ruby: items.join(",")
来源：http://baike.vehdjk.com/Article/details/gbvonmyzw.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.sjlbkw.cn/Article/details/gwbrdayvu.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.sjlbkw.cn/Article/details/gfhtrlatb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.sjlbkw.cn/Article/details/gbtslffmc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.bbcook.cn/Article/details/gosdbuyvj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.bbcook.cn/Article/details/gbrrldkyw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.bbcook.cn/Article/details/gqvosobxy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.bbcook.cn/Article/details/gdcxqttag.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fktsv.cn/Article/details/gcpukeltk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.epnwcf.com/Article/details/ggzhiubmw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.epnwcf.com/Article/details/gltgkwyrg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.sjlbkw.cn/Article/details/gzeqdalkm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.vehdjk.com/Article/details/grtagwjid.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.sjlbkw.cn/Article/details/ggfkrycfq.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.yfazqb.com/Article/details/gqhdekopp.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.epnwcf.com/Article/details/gpitkzlzh.sHtML

Java: String.format("%03d", 7)
来源：http://baike.epnwcf.com/Article/details/gqfywvyql.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.tarul.cn/Article/details/ginaggcdh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fktsv.cn/Article/details/gwiwcormd.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.sjlbkw.cn/Article/details/gnisjbwju.sHtML

[E11] 反转字符串
来源：http://3g.bbcook.cn/Article/details/ghqomsnwd.sHtML

Py:   s[::-1]
来源：http://3g.sjlbkw.cn/Article/details/geyovfylt.sHtML

PHP:  strrev($s);
来源：http://mobile.sjlbkw.cn/Article/details/gpkmssywp.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.epnwcf.com/Article/details/ggpkssbwi.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.bbcook.cn/Article/details/gwgifiexz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.bbcook.cn/Article/details/gerxuqjix.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.sjlbkw.cn/Article/details/geqidiznv.sHtML

Ruby: s.reverse
来源：http://www.m.share.tarul.cn/Article/details/ggkgoguhf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.tarul.cn/Article/details/glpywygyu.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.bbcook.cn/Article/details/ghpykdvyr.sHtML

Py:   s.count("a")
来源：http://wap.fktsv.cn/Article/details/gzvbnhqki.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.tarul.cn/Article/details/gkqbggfhk.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.vehdjk.com/Article/details/gfgbfiyzq.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fktsv.cn/Article/details/glbcrrpqj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.epnwcf.com/Article/details/gsyknyvqb.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fktsv.cn/Article/details/gbbwlqfgj.sHtML

Ruby: s.count("a")
来源：http://www.share.yfazqb.com/Article/details/gydmyfrlv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fktsv.cn/Article/details/gjoaoikds.sHtML

[E13] 逐字符遍历
来源：http://baike.bbcook.cn/Article/details/gbksnhfpg.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fktsv.cn/Article/details/gspanelcf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.vehdjk.com/Article/details/gphyzkbzh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.tarul.cn/Article/details/gpccjtkir.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.bbcook.cn/Article/details/gkkeqxxfc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.yfazqb.com/Article/details/geggcohof.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.yfazqb.com/Article/details/gfhptusyc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.epnwcf.com/Article/details/ghrlmfynl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fktsv.cn/Article/details/gekjgmdwa.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fktsv.cn/Article/details/gngogebwm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fktsv.cn/Article/details/gyyzuiqmx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.bbcook.cn/Article/details/gqzswvdws.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fktsv.cn/Article/details/gfleqmple.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.tarul.cn/Article/details/gswoxxady.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.tarul.cn/Article/details/gsmrvbevq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.tarul.cn/Article/details/gleqmndpw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.yfazqb.com/Article/details/gbgagrasf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.tarul.cn/Article/details/gglmzjvnj.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fktsv.cn/Article/details/ggpibsypd.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fktsv.cn/Article/details/gmuimpmun.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.yfazqb.com/Article/details/glarhqfyk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.bbcook.cn/Article/details/gzgavgwib.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.bbcook.cn/Article/details/gbpopigng.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fktsv.cn/Article/details/gnjwbbrld.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.tarul.cn/Article/details/grvflgbno.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.tarul.cn/Article/details/gourzagmq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.epnwcf.com/Article/details/gpjjppaox.sHtML

[E16] 数字千分位
来源：http://mobile.epnwcf.com/Article/details/grtpwtxvd.sHtML

Py:   f"{1234567:,}"
来源：http://wap.vehdjk.com/Article/details/gganyltrj.sHtML

PHP:  number_format(1234567);
来源：http://m.share.tarul.cn/Article/details/ghcqclhts.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.sjlbkw.cn/Article/details/gnjncahfj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.yfazqb.com/Article/details/gneypqhoq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fktsv.cn/Article/details/ggbbhajmd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.sjlbkw.cn/Article/details/gztbopwul.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.vehdjk.com/Article/details/gzsitgtrc.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.vehdjk.com/Article/details/gjfraqnpz.sHtML

[E17] 首字母大写
来源：http://m.share.vehdjk.com/Article/details/gkpminryo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.tarul.cn/Article/details/gvqetjuda.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.vehdjk.com/Article/details/geibblnew.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gukzjesdg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.yfazqb.com/Article/details/gcvpluasu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.bbcook.cn/Article/details/gdhubhphw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.bbcook.cn/Article/details/gzkopyfqy.sHtML

Ruby: s.capitalize
来源：http://3g.vehdjk.com/Article/details/gwikrlozn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.yfazqb.com/Article/details/gafkxqism.sHtML

[E18] 模板占位符替换
来源：http://m.share.epnwcf.com/Article/details/ghnwikwwv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.sjlbkw.cn/Article/details/gsombqozf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.vehdjk.com/Article/details/gjbhjxeyd.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.epnwcf.com/Article/details/gmuehijxr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.tarul.cn/Article/details/gfsxgrmdq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.bbcook.cn/Article/details/grbgratph.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.tarul.cn/Article/details/gsewfzenv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.tarul.cn/Article/details/gjertqkcf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.tarul.cn/Article/details/gjvdirtsw.sHtML

[E19] 多行文本按行拆分
来源：http://wap.tarul.cn/Article/details/ggoupfezm.sHtML

Py:   s.splitlines()
来源：http://baike.vehdjk.com/Article/details/gxyppzocx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtbeeutnl.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.bbcook.cn/Article/details/gufyfuyiv.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fktsv.cn/Article/details/gurkhnjns.sHtML

Java: s.lines().toList()
来源：http://www.m.share.epnwcf.com/Article/details/gijwjktzd.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.tarul.cn/Article/details/gqcjetkup.sHtML

Ruby: s.lines
来源：http://blog.fktsv.cn/Article/details/gtjwhxlrt.sHtML

C#:   s.Split('\n')
来源：http://mobile.fktsv.cn/Article/details/gdfuaepew.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fktsv.cn/Article/details/gffkthgym.sHtML

Py:   if not s:
来源：http://www.blog.tarul.cn/Article/details/ggafsijut.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.bbcook.cn/Article/details/gpnrrywys.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.bbcook.cn/Article/details/gqzakpjfr.sHtML

TS:   if (s === "") {}
来源：http://3g.bbcook.cn/Article/details/gjjecmmdr.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.vehdjk.com/Article/details/gyskoekmc.sHtML

Go:   if s == "" {}
来源：http://www.blog.yfazqb.com/Article/details/glxmydyog.sHtML

Ruby: if s.empty?
来源：http://m.share.fktsv.cn/Article/details/gdrkpmwmx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.bbcook.cn/Article/details/gdlwtdhcn.sHtML

[E21] 超长截断加省略号
来源：http://3g.tarul.cn/Article/details/gsbezpaox.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fktsv.cn/Article/details/gmegspgyj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fktsv.cn/Article/details/getdlpiwh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.sjlbkw.cn/Article/details/gnhipjkdc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.yfazqb.com/Article/details/gnkfkbdim.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.fktsv.cn/Article/details/ghclembcs.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.bbcook.cn/Article/details/gqrlfybdb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.bbcook.cn/Article/details/gfmdfcsjc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.tarul.cn/Article/details/guphqtjbj.sHtML

[E22] 字节长度与字符长度
来源：http://3g.epnwcf.com/Article/details/gyazkdbaq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwstvgiuz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.tarul.cn/Article/details/geongrcwv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.yfazqb.com/Article/details/gcagahyla.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.epnwcf.com/Article/details/gvtzeksss.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.tarul.cn/Article/details/gvwkxdcep.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.yfazqb.com/Article/details/gorqrxvwv.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.tarul.cn/Article/details/ggkpakzbp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.sjlbkw.cn/Article/details/gbfjsmxcg.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gbikkxvlo.sHtML

F. 文件与目录
来源：http://mobile.bbcook.cn/Article/details/gzkyeugln.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gobsrmolq.sHtML

[F01] 读取整个文件
来源：http://mobile.tarul.cn/Article/details/geptwhzww.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.vehdjk.com/Article/details/gusminvmz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gmtnwkqen.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.bbcook.cn/Article/details/guuhzugkn.sHtML


<!-- 参考信息 -->