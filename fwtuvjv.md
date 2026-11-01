代发 wailian999

[D11] 反转数组
来源：http://baike.tarul.cn/Article/details/gqwbeqere.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.epnwcf.com/Article/details/gwkotkadu.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.vehdjk.com/Article/details/gjeavjtxv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fktsv.cn/Article/details/gxozjupba.sHtML

TS:   [...arr].reverse();
来源：http://read.share.bbcook.cn/Article/details/gotzvqqnv.sHtML

Java: Collections.reverse(list);
来源：http://read.share.bbcook.cn/Article/details/gjczyhjza.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.vehdjk.com/Article/details/gpnowqyav.sHtML

Ruby: arr.reverse
来源：http://read.share.yfazqb.com/Article/details/gizcpvugj.sHtML

C#:   list.Reverse();
来源：http://m.share.fktsv.cn/Article/details/gffziobbz.sHtML

[D12] 查找元素下标
来源：http://blog.sjlbkw.cn/Article/details/gxpqfojzg.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.sjlbkw.cn/Article/details/gwgugaibn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.sjlbkw.cn/Article/details/gluaswryl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.tarul.cn/Article/details/gbfydxazx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.vehdjk.com/Article/details/gejgepefz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.yfazqb.com/Article/details/gsgthlapy.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gustdrrxc.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.tarul.cn/Article/details/gmsoemsfh.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.vehdjk.com/Article/details/gwmavduxt.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fktsv.cn/Article/details/gdnhmukjn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.sjlbkw.cn/Article/details/gfsfidyoz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.tarul.cn/Article/details/gkyvtpnxv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fktsv.cn/Article/details/gyruktkhx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fktsv.cn/Article/details/gjpxwxufr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fktsv.cn/Article/details/gbkyboymz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fktsv.cn/Article/details/glxrqvanv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.bbcook.cn/Article/details/gbmcjyagb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.bbcook.cn/Article/details/gzoxhazkc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.tarul.cn/Article/details/grrnmvbgq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.tarul.cn/Article/details/gzpxibehj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.yfazqb.com/Article/details/ggqppcxys.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.vehdjk.com/Article/details/gjbhptwtf.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fktsv.cn/Article/details/gpjnuixsm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.tarul.cn/Article/details/gilpkzkng.sHtML

Go:   // 手写循环
来源：http://read.share.vehdjk.com/Article/details/gwftdtuap.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkimnqmpu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fktsv.cn/Article/details/gsrrmebln.sHtML

[D15] 去重
来源：http://3g.fktsv.cn/Article/details/gnwbnqbye.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.tarul.cn/Article/details/goxgilfub.sHtML

PHP:  array_unique($arr);
来源：http://read.share.yfazqb.com/Article/details/gwiebhhfw.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.vehdjk.com/Article/details/glwaosemm.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.vehdjk.com/Article/details/grpntmdvc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.tarul.cn/Article/details/gglcrdkyc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.bbcook.cn/Article/details/gnjbfzgyc.sHtML

Ruby: arr.uniq
来源：http://mobile.epnwcf.com/Article/details/glfierfmj.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.vehdjk.com/Article/details/gufwmwaad.sHtML

[D16] 求和与平均值
来源：http://read.share.yfazqb.com/Article/details/gfaavfmhz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.yfazqb.com/Article/details/gyzqzaufa.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.yfazqb.com/Article/details/gcvyauxrt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.tarul.cn/Article/details/grhteabla.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.epnwcf.com/Article/details/gvqmdtqel.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.bbcook.cn/Article/details/gdquzjqwr.sHtML

Go:   // 手写循环累加
来源：http://3g.bbcook.cn/Article/details/ggasenwaw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.bbcook.cn/Article/details/gcpedvcur.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fktsv.cn/Article/details/gtmnpncyu.sHtML

[D17] 最大值与最小值
来源：http://3g.fktsv.cn/Article/details/gwzambfsw.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.tarul.cn/Article/details/gjvypsdqt.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.bbcook.cn/Article/details/gbfohdouz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.epnwcf.com/Article/details/gnmkmchuj.sHtML

TS:   Math.max(...arr);
来源：http://blog.yfazqb.com/Article/details/gsmeclvzr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.tarul.cn/Article/details/gbmjgkelv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gsrintmsw.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.epnwcf.com/Article/details/gafpmpmvg.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fktsv.cn/Article/details/gfqvwqeqm.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.bbcook.cn/Article/details/gdkulzmbl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fktsv.cn/Article/details/gfuljedqa.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.yfazqb.com/Article/details/gbygxxhli.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fktsv.cn/Article/details/ggmeuidgi.sHtML

TS:   nested.flat();
来源：http://3g.sjlbkw.cn/Article/details/gseyvxypr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.vehdjk.com/Article/details/gwdltmtab.sHtML

Go:   // 手写双层循环
来源：http://blog.yfazqb.com/Article/details/gcaaorvil.sHtML

Ruby: nested.flatten
来源：http://www.blog.sjlbkw.cn/Article/details/gjllpegun.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.vehdjk.com/Article/details/gxywyyxko.sHtML

[D19] 按字段分组
来源：http://www.blog.sjlbkw.cn/Article/details/godnxlkfz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.epnwcf.com/Article/details/gnijhovyw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.tarul.cn/Article/details/gvpxntiyq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.yfazqb.com/Article/details/gvyulowrg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.vehdjk.com/Article/details/gsbchvpqv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.bbcook.cn/Article/details/gtnunhoyp.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.epnwcf.com/Article/details/gajwfikkd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.epnwcf.com/Article/details/gcyxrkgpn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.epnwcf.com/Article/details/gnvphtxnh.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.vehdjk.com/Article/details/gzsdambnu.sHtML

Py:   Counter(arr)
来源：http://m.share.epnwcf.com/Article/details/gtaqfuqcv.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.tarul.cn/Article/details/greodstpu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.tarul.cn/Article/details/ghvzmohze.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.yfazqb.com/Article/details/gzzhtbvrs.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.yfazqb.com/Article/details/gbrkudzbj.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.yfazqb.com/Article/details/ghhgezzbs.sHtML

Ruby: arr.tally
来源：http://m.share.tarul.cn/Article/details/gdyokqusy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.sjlbkw.cn/Article/details/gkwyrzqmj.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.vehdjk.com/Article/details/gyngwprhx.sHtML

Py:   x in arr
来源：http://blog.yfazqb.com/Article/details/gguowdise.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.vehdjk.com/Article/details/gybnayehq.sHtML

JS:   arr.includes(x)
来源：http://baike.vehdjk.com/Article/details/gkrfwrdcz.sHtML

TS:   arr.includes(x)
来源：http://mobile.tarul.cn/Article/details/gdfdsjovo.sHtML

Java: list.contains(x)
来源：http://www.blog.vehdjk.com/Article/details/gdbvvhvlj.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gtrqmadno.sHtML

Ruby: arr.include?(x)
来源：http://blog.fktsv.cn/Article/details/gurjqhkwv.sHtML

C#:   list.Contains(x)
来源：http://3g.epnwcf.com/Article/details/gjdvvogjf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.tarul.cn/Article/details/gaavinmeb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.epnwcf.com/Article/details/goeyggtpg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.vehdjk.com/Article/details/gknsxvshh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gvbwoclru.sHtML

TS:   [...arr];
来源：http://mobile.vehdjk.com/Article/details/gtpmltuke.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.tarul.cn/Article/details/gwromplqc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.vehdjk.com/Article/details/gelhrieuj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.sjlbkw.cn/Article/details/gppdljmsp.sHtML

C#:   new List<int>(list);
来源：http://3g.fktsv.cn/Article/details/gbkcmylgo.sHtML

[D23] reduce 累积计算
来源：http://blog.bbcook.cn/Article/details/ginjkortr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.yfazqb.com/Article/details/gthsawjdt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fktsv.cn/Article/details/glhayonuq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.sjlbkw.cn/Article/details/gjnwffhsg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.epnwcf.com/Article/details/gwapiqtrp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.sjlbkw.cn/Article/details/gpccwxzpt.sHtML

Go:   // 手写循环
来源：http://mobile.yfazqb.com/Article/details/gcerxnmim.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.vehdjk.com/Article/details/gsvllwfdu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.yfazqb.com/Article/details/gnhcbokeq.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.epnwcf.com/Article/details/gthvrnbao.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.yfazqb.com/Article/details/gjydzvpco.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.sjlbkw.cn/Article/details/grsekmikr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.yfazqb.com/Article/details/gxibqnypa.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gjochwqwt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.bbcook.cn/Article/details/gjebghwbq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.bbcook.cn/Article/details/gfknilowo.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.yfazqb.com/Article/details/gykdlziqn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.sjlbkw.cn/Article/details/gbewpbmjf.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fktsv.cn/Article/details/gkrlfwsve.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.vehdjk.com/Article/details/gemggkrcp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.bbcook.cn/Article/details/gmthydygn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.yfazqb.com/Article/details/gtfgoxayq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fktsv.cn/Article/details/glhkyqukb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.epnwcf.com/Article/details/gphggnxec.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.fktsv.cn/Article/details/gsjwqdvyo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.sjlbkw.cn/Article/details/gamnysxjb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.vehdjk.com/Article/details/gprjdotdb.sHtML

[D26] 数组转字符串
来源：http://blog.epnwcf.com/Article/details/gcxqxzluo.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.tarul.cn/Article/details/glfqwrzqc.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.yfazqb.com/Article/details/gpxvtplfi.sHtML

JS:   arr.join(", ")
来源：http://3g.fktsv.cn/Article/details/grcwkhxcj.sHtML

TS:   arr.join(", ")
来源：http://wap.vehdjk.com/Article/details/gixfwxlsr.sHtML

Java: String.join(", ", list)
来源：http://m.share.tarul.cn/Article/details/gyvqbgywf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.fktsv.cn/Article/details/gtasjgbuv.sHtML

Ruby: arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/gpeafrytr.sHtML

C#:   string.Join(", ", list)
来源：http://wap.epnwcf.com/Article/details/gmlsksowz.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gsynqoeuv.sHtML

E. 字符串处理
来源：http://m.share.tarul.cn/Article/details/gytvmjafx.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gteaasxcj.sHtML

[E01] 拼接字符串
来源：http://m.share.bbcook.cn/Article/details/gsrpzcfrx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.sjlbkw.cn/Article/details/gmthsmomt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fktsv.cn/Article/details/ghfgcrfoq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.yfazqb.com/Article/details/ggehassag.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.bbcook.cn/Article/details/grkilhxmg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.vehdjk.com/Article/details/gqgjctqsm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.tarul.cn/Article/details/grntlthcs.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.bbcook.cn/Article/details/givjkacwe.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.vehdjk.com/Article/details/gtxzkqvur.sHtML

[E02] 重复字符串
来源：http://baike.yfazqb.com/Article/details/golpureip.sHtML

Py:   "ab" * 3
来源：http://www.share.epnwcf.com/Article/details/gvgrwepeh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fktsv.cn/Article/details/gftkmyuub.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.vehdjk.com/Article/details/gtcymtvhh.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.bbcook.cn/Article/details/gisqynloq.sHtML

Java: "ab".repeat(3)
来源：http://read.share.epnwcf.com/Article/details/gtaamxlvg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.epnwcf.com/Article/details/gdillymea.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.tarul.cn/Article/details/gvseeqwoo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.epnwcf.com/Article/details/gkjcjqbie.sHtML

[E03] 截取子串
来源：http://mobile.sjlbkw.cn/Article/details/gxkpnxjlg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.epnwcf.com/Article/details/goareoval.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.sjlbkw.cn/Article/details/gjxrynlzu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.tarul.cn/Article/details/gnacxvwvc.sHtML

TS:   s.slice(1, 4)
来源：http://wap.yfazqb.com/Article/details/gtqvcaofd.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gihkvnure.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fktsv.cn/Article/details/gbkapqhiq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.epnwcf.com/Article/details/grruzgxiq.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.epnwcf.com/Article/details/gltswhqjn.sHtML

[E04] 查找子串位置
来源：http://wap.vehdjk.com/Article/details/gidqbepzo.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.vehdjk.com/Article/details/ghepmzcsh.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.yfazqb.com/Article/details/grwdbwxuk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.yfazqb.com/Article/details/gqsgxlydo.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.sjlbkw.cn/Article/details/gilhucxro.sHtML

Java: s.indexOf("x")
来源：http://www.share.tarul.cn/Article/details/gvebbcqbc.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.vehdjk.com/Article/details/gelnczkda.sHtML

Ruby: s.index("x")
来源：http://3g.tarul.cn/Article/details/gpjhwhsqv.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fktsv.cn/Article/details/gvvxnslpo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.sjlbkw.cn/Article/details/gflqcgxek.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.fktsv.cn/Article/details/gkfdqhjsd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.yfazqb.com/Article/details/gxfcspmlz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.sjlbkw.cn/Article/details/gxngbwqtt.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.yfazqb.com/Article/details/gzctjtifm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.epnwcf.com/Article/details/gynuhqwpd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.yfazqb.com/Article/details/gfsrslunj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.vehdjk.com/Article/details/gukkknznz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.tarul.cn/Article/details/gosozghdt.sHtML

[E06] 替换子串
来源：http://mobile.fktsv.cn/Article/details/gsezpdpcc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.sjlbkw.cn/Article/details/gptxoslhl.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.vehdjk.com/Article/details/gdlltwzpg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gapeeadiz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.epnwcf.com/Article/details/ghghgyngw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.yfazqb.com/Article/details/gaqtpjcde.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.epnwcf.com/Article/details/gtnxiekwd.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.tarul.cn/Article/details/gweokgqgq.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/girpncall.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fktsv.cn/Article/details/gkczwjmqz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.sjlbkw.cn/Article/details/ghxnavvyq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.epnwcf.com/Article/details/gthdyrczf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.sjlbkw.cn/Article/details/gfyedwfht.sHtML

TS:   s.split(",")
来源：http://blog.tarul.cn/Article/details/gmiihpfax.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.tarul.cn/Article/details/grreodgyb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.vehdjk.com/Article/details/gdtvgddfp.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.vehdjk.com/Article/details/gycgokqyp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fktsv.cn/Article/details/gwwaimdmi.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.sjlbkw.cn/Article/details/gcaqlppfg.sHtML

Py:   ",".join(items)
来源：http://www.share.fktsv.cn/Article/details/ggppmcocw.sHtML

PHP:  implode(",", $items);
来源：http://3g.yfazqb.com/Article/details/gccvejano.sHtML

JS:   items.join(",")
来源：http://m.share.fktsv.cn/Article/details/gbbqucbni.sHtML

TS:   items.join(",")
来源：http://m.share.vehdjk.com/Article/details/gibotuptb.sHtML

Java: String.join(",", items)
来源：http://3g.fktsv.cn/Article/details/gtfhgrqfz.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.bbcook.cn/Article/details/gwytjpjmf.sHtML

Ruby: items.join(",")
来源：http://m.share.epnwcf.com/Article/details/gicqsetau.sHtML

C#:   string.Join(",", items)
来源：http://mobile.epnwcf.com/Article/details/gfugmesiq.sHtML

[E09] 去除所有空白字符
来源：http://mobile.yfazqb.com/Article/details/gvsnbncap.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.tarul.cn/Article/details/gmgbjmvql.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fktsv.cn/Article/details/gjnreslrp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.yfazqb.com/Article/details/gjhpugtjv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.yfazqb.com/Article/details/gsujiqdvj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.bbcook.cn/Article/details/glpyfkrmz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fktsv.cn/Article/details/gltdpmmyi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.epnwcf.com/Article/details/gkuosgapa.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.fktsv.cn/Article/details/gyxgtgczm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.sjlbkw.cn/Article/details/ghjoqykss.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.vehdjk.com/Article/details/gwjmhtgzh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.vehdjk.com/Article/details/gftwktkpi.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.bbcook.cn/Article/details/giykwrjzq.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.bbcook.cn/Article/details/ghqnytzbo.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fktsv.cn/Article/details/gymnuezaf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.vehdjk.com/Article/details/gtbhdxwbt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.tarul.cn/Article/details/gyidkpedd.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.fktsv.cn/Article/details/gnfmwzzxx.sHtML

[E11] 反转字符串
来源：http://3g.yfazqb.com/Article/details/ggpdwkpmq.sHtML

Py:   s[::-1]
来源：http://www.blog.yfazqb.com/Article/details/gueopktzn.sHtML

PHP:  strrev($s);
来源：http://3g.fktsv.cn/Article/details/gnjtoqlnc.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/gosspwqeg.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.sjlbkw.cn/Article/details/gwzxzdqxq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.bbcook.cn/Article/details/guiohdwpl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.bbcook.cn/Article/details/gpuwwzysx.sHtML

Ruby: s.reverse
来源：http://www.blog.fktsv.cn/Article/details/gtrxhbbth.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.yfazqb.com/Article/details/gcgwtwapm.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.yfazqb.com/Article/details/gdefjiabc.sHtML

Py:   s.count("a")
来源：http://www.share.tarul.cn/Article/details/gnlsuhoxs.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.vehdjk.com/Article/details/gvojzqxhd.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.bbcook.cn/Article/details/gmwvqcbld.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fktsv.cn/Article/details/glaujwgmj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.vehdjk.com/Article/details/gfzrpbyvc.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.tarul.cn/Article/details/gwzkbbiyo.sHtML

Ruby: s.count("a")
来源：http://read.share.sjlbkw.cn/Article/details/gsaefxlsj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.tarul.cn/Article/details/gygsaxkyh.sHtML

[E13] 逐字符遍历
来源：http://3g.yfazqb.com/Article/details/gbdprfuim.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.tarul.cn/Article/details/gyzmgebyl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.vehdjk.com/Article/details/guvcsqsva.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fktsv.cn/Article/details/gbtfsyoma.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.sjlbkw.cn/Article/details/grvokcofi.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.vehdjk.com/Article/details/gackqkymt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.bbcook.cn/Article/details/gppzceajn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.sjlbkw.cn/Article/details/grqlaqijq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.epnwcf.com/Article/details/gizpmpvuq.sHtML

[E14] URL 编码与 Base64
来源：http://3g.epnwcf.com/Article/details/gdbeuxdvo.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.yfazqb.com/Article/details/gdhqmojvg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.bbcook.cn/Article/details/goalvlcgd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.tarul.cn/Article/details/glfmxvtfu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.tarul.cn/Article/details/gbkjvdxac.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fktsv.cn/Article/details/gndclbufn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.sjlbkw.cn/Article/details/gadqmmppx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.vehdjk.com/Article/details/gckcrpfkz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.tarul.cn/Article/details/grbwadfwj.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.epnwcf.com/Article/details/gnxzynqlf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fktsv.cn/Article/details/gyoptqxjt.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.tarul.cn/Article/details/gpsktvasb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.yfazqb.com/Article/details/gyybpcwgu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.bbcook.cn/Article/details/gpiwksyrr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.bbcook.cn/Article/details/gntmzdced.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fktsv.cn/Article/details/gidrecxrf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.bbcook.cn/Article/details/gwipuecra.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.yfazqb.com/Article/details/gupiokeyq.sHtML

[E16] 数字千分位
来源：http://www.share.sjlbkw.cn/Article/details/gkutyxnot.sHtML

Py:   f"{1234567:,}"
来源：http://baike.epnwcf.com/Article/details/gggcroxsf.sHtML

PHP:  number_format(1234567);
来源：http://baike.vehdjk.com/Article/details/gnwjhjfdo.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.epnwcf.com/Article/details/gyjsgkdxz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.bbcook.cn/Article/details/gipsejird.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.epnwcf.com/Article/details/gpxhhvucf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.tarul.cn/Article/details/gccajveuz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fktsv.cn/Article/details/gbquqwonj.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.yfazqb.com/Article/details/gkpliwmie.sHtML

[E17] 首字母大写
来源：http://www.blog.yfazqb.com/Article/details/gfijzgysd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.yfazqb.com/Article/details/ghycvejpp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.epnwcf.com/Article/details/ghffumjcg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.epnwcf.com/Article/details/grenmnbvc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.epnwcf.com/Article/details/gknrvyhcq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.bbcook.cn/Article/details/gkokywrwq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.yfazqb.com/Article/details/gfzqluwwl.sHtML

Ruby: s.capitalize
来源：http://mobile.bbcook.cn/Article/details/glrjdabcs.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.epnwcf.com/Article/details/gdvomoiyr.sHtML


<!-- 参考信息 -->