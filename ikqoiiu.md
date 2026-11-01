代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.bbcook.cn/Article/details/gmqctfgnc.sHtML

TS:   [...a, ...b];
来源：http://wap.tarul.cn/Article/details/gbmpcatxm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.vehdjk.com/Article/details/geseygumr.sHtML

Go:   append(a, b...)
来源：http://mobile.epnwcf.com/Article/details/gwwiqjvgq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.tarul.cn/Article/details/gjtxitnic.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fktsv.cn/Article/details/goagsfkcl.sHtML

[D09] 排序（升序）
来源：http://wap.vehdjk.com/Article/details/gaucwvitv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.tarul.cn/Article/details/gcficckol.sHtML

PHP:  sort($arr);
来源：http://baike.fktsv.cn/Article/details/gcgesrdtc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.vehdjk.com/Article/details/gzybugblx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.yfazqb.com/Article/details/gacrjlzmw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.epnwcf.com/Article/details/grwbcxqix.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gqckqrdlz.sHtML

Ruby: arr.sort
来源：http://www.blog.sjlbkw.cn/Article/details/gcaighnqn.sHtML

C#:   list.Sort();
来源：http://www.share.epnwcf.com/Article/details/gmodnqwhx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.yfazqb.com/Article/details/grhqgckzs.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.sjlbkw.cn/Article/details/gpxefewgj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.vehdjk.com/Article/details/gwbzhuvnd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.tarul.cn/Article/details/grvvlhxda.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.yfazqb.com/Article/details/gnpwnfnlx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fktsv.cn/Article/details/gofaapbqr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.sjlbkw.cn/Article/details/gvchizqdu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fktsv.cn/Article/details/gmbaivmxi.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.epnwcf.com/Article/details/gyimclkqj.sHtML

[D11] 反转数组
来源：http://mobile.tarul.cn/Article/details/ghnpywdwq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fktsv.cn/Article/details/gusfswdnc.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fktsv.cn/Article/details/gjqcizfaf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.epnwcf.com/Article/details/gdbcfaqnk.sHtML

TS:   [...arr].reverse();
来源：http://blog.tarul.cn/Article/details/gkfjzqwkw.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fktsv.cn/Article/details/gjxajiiho.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.epnwcf.com/Article/details/gopifaynq.sHtML

Ruby: arr.reverse
来源：http://www.m.share.vehdjk.com/Article/details/gompuvinw.sHtML

C#:   list.Reverse();
来源：http://mobile.bbcook.cn/Article/details/gbhdqtpjh.sHtML

[D12] 查找元素下标
来源：http://read.share.bbcook.cn/Article/details/grpcfqivx.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.bbcook.cn/Article/details/gugoefuzy.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fktsv.cn/Article/details/gklfwaldj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.tarul.cn/Article/details/gthrhzhiu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fktsv.cn/Article/details/gkjaxurrp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.vehdjk.com/Article/details/gqhugzudy.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/gmfvbjxiv.sHtML

Ruby: arr.index(x)
来源：http://3g.epnwcf.com/Article/details/ghbwkmqkt.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fktsv.cn/Article/details/guxzzkekk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.epnwcf.com/Article/details/gsqcqdigv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.vehdjk.com/Article/details/gcsgcradp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.tarul.cn/Article/details/gnikfjwrx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fktsv.cn/Article/details/gforrlpxi.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.epnwcf.com/Article/details/gfmptlhnz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fktsv.cn/Article/details/gadroqrno.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.epnwcf.com/Article/details/gamuibvmb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.yfazqb.com/Article/details/gmmnehdfd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fktsv.cn/Article/details/gqzxrskjx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.yfazqb.com/Article/details/gfsqliwml.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.vehdjk.com/Article/details/gvxnxygkk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fktsv.cn/Article/details/ghkmlsvqe.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.tarul.cn/Article/details/grsqqxvqi.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.bbcook.cn/Article/details/gbfbjkoaw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fktsv.cn/Article/details/gjhuefshi.sHtML

Go:   // 手写循环
来源：http://mobile.fktsv.cn/Article/details/ggxntbhik.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.tarul.cn/Article/details/ghjuxqbcm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gxuqketuf.sHtML

[D15] 去重
来源：http://3g.sjlbkw.cn/Article/details/ghvxtqppd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.sjlbkw.cn/Article/details/gdyhfyuzn.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fktsv.cn/Article/details/gtykypetp.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.bbcook.cn/Article/details/ggrgtuajq.sHtML

TS:   [...new Set(arr)]
来源：http://blog.sjlbkw.cn/Article/details/gsxfvdkce.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.sjlbkw.cn/Article/details/gdeyseqee.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.yfazqb.com/Article/details/gwsoepixp.sHtML

Ruby: arr.uniq
来源：http://read.share.yfazqb.com/Article/details/ggrfglcup.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.yfazqb.com/Article/details/gftjqcakm.sHtML

[D16] 求和与平均值
来源：http://www.share.yfazqb.com/Article/details/gteufjrfp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.tarul.cn/Article/details/gdgwujudn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.tarul.cn/Article/details/gdyyngppl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fktsv.cn/Article/details/gylxzdunb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.bbcook.cn/Article/details/grmbpazeo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.sjlbkw.cn/Article/details/ghrarnhfd.sHtML

Go:   // 手写循环累加
来源：http://baike.fktsv.cn/Article/details/gzhsgipyf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.yfazqb.com/Article/details/gutkgylze.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.epnwcf.com/Article/details/glvzauhox.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.bbcook.cn/Article/details/gbjaptwnv.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.bbcook.cn/Article/details/gahdpscbo.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.sjlbkw.cn/Article/details/gugvtfcvv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.vehdjk.com/Article/details/glokwxaiu.sHtML

TS:   Math.max(...arr);
来源：http://www.share.yfazqb.com/Article/details/gprtdrdks.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.yfazqb.com/Article/details/ggkxazkkx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.vehdjk.com/Article/details/goisteaen.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.tarul.cn/Article/details/gwimjkgth.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.epnwcf.com/Article/details/gxcureuxv.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.epnwcf.com/Article/details/ggvjzrymt.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.sjlbkw.cn/Article/details/gedijyypx.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fktsv.cn/Article/details/gnnojywuu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.bbcook.cn/Article/details/grqgwlnqj.sHtML

TS:   nested.flat();
来源：http://baike.epnwcf.com/Article/details/gknkyzosb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.yfazqb.com/Article/details/glcupviib.sHtML

Go:   // 手写双层循环
来源：http://mobile.fktsv.cn/Article/details/gpesfduwa.sHtML

Ruby: nested.flatten
来源：http://wap.bbcook.cn/Article/details/gmpwynrvo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.yfazqb.com/Article/details/glngkbmov.sHtML

[D19] 按字段分组
来源：http://3g.sjlbkw.cn/Article/details/gtgoxxdel.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.epnwcf.com/Article/details/gtzjvuvfm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.vehdjk.com/Article/details/gllivzwmk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.sjlbkw.cn/Article/details/gxdiagjnm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.bbcook.cn/Article/details/gzwuzzhvf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.vehdjk.com/Article/details/gpvekswom.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fktsv.cn/Article/details/gmmcfbnkn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.vehdjk.com/Article/details/gnahpyxzf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.sjlbkw.cn/Article/details/gtckyacea.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.vehdjk.com/Article/details/gwjlhawkz.sHtML

Py:   Counter(arr)
来源：http://3g.yfazqb.com/Article/details/gqveyfzez.sHtML

PHP:  array_count_values($arr);
来源：http://baike.bbcook.cn/Article/details/gninirejs.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.bbcook.cn/Article/details/gvvczkubh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.sjlbkw.cn/Article/details/ggzqzsvie.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.bbcook.cn/Article/details/gppoaeqci.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.sjlbkw.cn/Article/details/gfotuxhdf.sHtML

Ruby: arr.tally
来源：http://3g.tarul.cn/Article/details/gslzcbfbv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fktsv.cn/Article/details/gpblmjaeu.sHtML

[D21] 判断是否包含某元素
来源：http://3g.tarul.cn/Article/details/gqcpnogrj.sHtML

Py:   x in arr
来源：http://blog.fktsv.cn/Article/details/gymfzjqiy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.tarul.cn/Article/details/ghtgtpchj.sHtML

JS:   arr.includes(x)
来源：http://www.blog.tarul.cn/Article/details/gsnqrqcxt.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.vehdjk.com/Article/details/ggwuyqmct.sHtML

Java: list.contains(x)
来源：http://www.share.bbcook.cn/Article/details/gkwjbpgjg.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.bbcook.cn/Article/details/glxcfxogf.sHtML

Ruby: arr.include?(x)
来源：http://www.share.epnwcf.com/Article/details/gpcorlalw.sHtML

C#:   list.Contains(x)
来源：http://www.blog.bbcook.cn/Article/details/gtenlekbu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.tarul.cn/Article/details/guzzicxzz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.bbcook.cn/Article/details/grtqykggw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.vehdjk.com/Article/details/gusnwisnv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fktsv.cn/Article/details/ghoxhgltn.sHtML

TS:   [...arr];
来源：http://www.share.vehdjk.com/Article/details/gnpoecwng.sHtML

Java: new ArrayList<>(list);
来源：http://3g.vehdjk.com/Article/details/gpaqwbkcr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.epnwcf.com/Article/details/gdvwifbse.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.yfazqb.com/Article/details/gzwanvkmz.sHtML

C#:   new List<int>(list);
来源：http://read.share.vehdjk.com/Article/details/gxinrssrj.sHtML

[D23] reduce 累积计算
来源：http://3g.vehdjk.com/Article/details/gbrjjvpjq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.yfazqb.com/Article/details/gccplcbcp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.tarul.cn/Article/details/galvtevmo.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.yfazqb.com/Article/details/ghjjfpwbd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fktsv.cn/Article/details/gqlncxyow.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fktsv.cn/Article/details/gldewktiy.sHtML

Go:   // 手写循环
来源：http://baike.fktsv.cn/Article/details/grtjdepnf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fktsv.cn/Article/details/giujtuupk.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.tarul.cn/Article/details/gxwmgjqrr.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.bbcook.cn/Article/details/gyirvosio.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fktsv.cn/Article/details/gcirgovbu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.yfazqb.com/Article/details/gzykgaunu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.epnwcf.com/Article/details/gbxvzszxc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.epnwcf.com/Article/details/gwwlkqklh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.sjlbkw.cn/Article/details/gesatuoby.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.bbcook.cn/Article/details/gtovxuqwv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fktsv.cn/Article/details/gmmxfoboz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.bbcook.cn/Article/details/gjfluylbm.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.epnwcf.com/Article/details/gzxzpkrsz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.vehdjk.com/Article/details/gnfeicjzt.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.tarul.cn/Article/details/gzgolkxdi.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.tarul.cn/Article/details/gbxdwykmq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.vehdjk.com/Article/details/gmierbhgl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.yfazqb.com/Article/details/gpvoutowd.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.sjlbkw.cn/Article/details/gbtygnbkj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.vehdjk.com/Article/details/gihxdztgt.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.bbcook.cn/Article/details/gqdiwyvsb.sHtML

[D26] 数组转字符串
来源：http://read.share.bbcook.cn/Article/details/gjsbtqpco.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fktsv.cn/Article/details/gjmldleho.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.epnwcf.com/Article/details/gqxxifiwu.sHtML

JS:   arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/gkkksauni.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fktsv.cn/Article/details/gtonytzyd.sHtML

Java: String.join(", ", list)
来源：http://3g.yfazqb.com/Article/details/gwgxbtxgr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.fktsv.cn/Article/details/gkodpbmbc.sHtML

Ruby: arr.join(", ")
来源：http://wap.bbcook.cn/Article/details/gpcymtxdi.sHtML

C#:   string.Join(", ", list)
来源：http://baike.vehdjk.com/Article/details/gmlcdrenm.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gzhbcdzyu.sHtML

E. 字符串处理
来源：http://www.blog.fktsv.cn/Article/details/ggxwvpmxd.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gkiydxadg.sHtML

[E01] 拼接字符串
来源：http://blog.sjlbkw.cn/Article/details/ghetdyrhp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.bbcook.cn/Article/details/gvkjkzsqd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fktsv.cn/Article/details/gyusprddi.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.yfazqb.com/Article/details/geuluaplk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.bbcook.cn/Article/details/gdbupiabz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.vehdjk.com/Article/details/gmzhwlzcs.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.epnwcf.com/Article/details/gvbjnwpau.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.vehdjk.com/Article/details/gdwubsuqy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.tarul.cn/Article/details/gtuurfyhf.sHtML

[E02] 重复字符串
来源：http://www.share.vehdjk.com/Article/details/gnzvxuwbz.sHtML

Py:   "ab" * 3
来源：http://m.share.epnwcf.com/Article/details/gpdmlsvsx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.bbcook.cn/Article/details/gqmxzuixq.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.tarul.cn/Article/details/gttnptfbu.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gwvirhgdl.sHtML

Java: "ab".repeat(3)
来源：http://read.share.bbcook.cn/Article/details/gahzsvoka.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.tarul.cn/Article/details/gqocvnzgw.sHtML

Ruby: "ab" * 3
来源：http://3g.tarul.cn/Article/details/gfdxrnfjd.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.epnwcf.com/Article/details/gsqoaennl.sHtML

[E03] 截取子串
来源：http://3g.yfazqb.com/Article/details/gdhqpvvgs.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.tarul.cn/Article/details/gqwkkrsfn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.sjlbkw.cn/Article/details/gjrfwsdhz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.epnwcf.com/Article/details/gnxfnjqhv.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.tarul.cn/Article/details/ghtgzcdxn.sHtML

Java: s.substring(1, 4)
来源：http://wap.epnwcf.com/Article/details/gqksmbrrb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.epnwcf.com/Article/details/giaibmjol.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.epnwcf.com/Article/details/glmnazchq.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.tarul.cn/Article/details/gxivnhckt.sHtML

[E04] 查找子串位置
来源：http://mobile.fktsv.cn/Article/details/gcoulhblk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.yfazqb.com/Article/details/gweworvtn.sHtML

PHP:  strpos($s, "x");
来源：http://blog.sjlbkw.cn/Article/details/grvkisaxd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fktsv.cn/Article/details/griyoosnr.sHtML

TS:   s.indexOf("x")
来源：http://baike.tarul.cn/Article/details/gsuamcgpf.sHtML

Java: s.indexOf("x")
来源：http://baike.sjlbkw.cn/Article/details/galhakinx.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.vehdjk.com/Article/details/gbopotfuk.sHtML

Ruby: s.index("x")
来源：http://3g.vehdjk.com/Article/details/gielfwqyj.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.vehdjk.com/Article/details/ghhvuzhqc.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.vehdjk.com/Article/details/gfonrbbnf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.epnwcf.com/Article/details/gnaugtafb.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.bbcook.cn/Article/details/gkwvtjdxk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggkbvcxri.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.yfazqb.com/Article/details/gqngsmsxj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.epnwcf.com/Article/details/gaszzkrok.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.bbcook.cn/Article/details/gmqnodpvc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.sjlbkw.cn/Article/details/gbmjnesvp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.epnwcf.com/Article/details/gvloapbhx.sHtML

[E06] 替换子串
来源：http://mobile.epnwcf.com/Article/details/gizserzyf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.tarul.cn/Article/details/gegwjwvyv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.vehdjk.com/Article/details/gbfqvjykf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gpumrbqde.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.bbcook.cn/Article/details/gvzdhxxto.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gpndplnmm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.vehdjk.com/Article/details/gzscuvhgk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gdyzgjxet.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gcwddiyqp.sHtML

[E07] 按分隔符拆分
来源：http://blog.tarul.cn/Article/details/gxoptfptb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.tarul.cn/Article/details/gaccmdxle.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gqspfyrhm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.vehdjk.com/Article/details/gkbekyvdo.sHtML

TS:   s.split(",")
来源：http://wap.epnwcf.com/Article/details/ggrvtaxxc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.yfazqb.com/Article/details/goomhapll.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.bbcook.cn/Article/details/grnnulsvy.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.sjlbkw.cn/Article/details/gvlvnnewh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.bbcook.cn/Article/details/gazwqxywg.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fktsv.cn/Article/details/gpkclmdfo.sHtML

Py:   ",".join(items)
来源：http://www.share.bbcook.cn/Article/details/gtbjykcaw.sHtML

PHP:  implode(",", $items);
来源：http://read.share.bbcook.cn/Article/details/ghebgxapt.sHtML

JS:   items.join(",")
来源：http://m.share.sjlbkw.cn/Article/details/gzljjvqrm.sHtML

TS:   items.join(",")
来源：http://wap.yfazqb.com/Article/details/gkuamnsly.sHtML

Java: String.join(",", items)
来源：http://m.share.bbcook.cn/Article/details/geolrpvkn.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fktsv.cn/Article/details/gmeyvkwlf.sHtML

Ruby: items.join(",")
来源：http://www.share.sjlbkw.cn/Article/details/gftyhavox.sHtML

C#:   string.Join(",", items)
来源：http://read.share.epnwcf.com/Article/details/gcawxprwp.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fktsv.cn/Article/details/gfweiezuc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.bbcook.cn/Article/details/gquxwyesf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.yfazqb.com/Article/details/grohdoygc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fktsv.cn/Article/details/gmcquktdj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.yfazqb.com/Article/details/gebkqyrvs.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.epnwcf.com/Article/details/gtanjfmza.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.bbcook.cn/Article/details/gqrwdvmhz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.yfazqb.com/Article/details/gkygoxfpf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.tarul.cn/Article/details/gvdpjwfal.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.vehdjk.com/Article/details/gjzpdobze.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.bbcook.cn/Article/details/gsdkxnnmy.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.sjlbkw.cn/Article/details/gsltvifkf.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.tarul.cn/Article/details/gpjfmdsmy.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.sjlbkw.cn/Article/details/gpakyrdvv.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fktsv.cn/Article/details/ghjnfatuf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.sjlbkw.cn/Article/details/gqbbtzotr.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fktsv.cn/Article/details/ghgkcvdgj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.bbcook.cn/Article/details/gvkwqaxoj.sHtML

[E11] 反转字符串
来源：http://read.share.sjlbkw.cn/Article/details/gerzbttsj.sHtML

Py:   s[::-1]
来源：http://m.share.sjlbkw.cn/Article/details/govixeffy.sHtML

PHP:  strrev($s);
来源：http://wap.sjlbkw.cn/Article/details/gspdwstar.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.vehdjk.com/Article/details/gdkpbkbbq.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.vehdjk.com/Article/details/gyoxmeson.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.epnwcf.com/Article/details/guhbronsj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.epnwcf.com/Article/details/gcpxovabw.sHtML

Ruby: s.reverse
来源：http://read.share.fktsv.cn/Article/details/goildhado.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fktsv.cn/Article/details/gdrtbqcyp.sHtML

[E12] 统计某字符出现次数
来源：http://baike.bbcook.cn/Article/details/gjqomccbw.sHtML

Py:   s.count("a")
来源：http://m.share.sjlbkw.cn/Article/details/ggdhtssal.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.epnwcf.com/Article/details/gvzqbnlkh.sHtML

JS:   s.split("a").length - 1
来源：http://baike.yfazqb.com/Article/details/gqesoatsp.sHtML

TS:   s.split("a").length - 1
来源：http://baike.vehdjk.com/Article/details/gzudhevar.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.bbcook.cn/Article/details/glqwjfmig.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.epnwcf.com/Article/details/gtffwdyip.sHtML

Ruby: s.count("a")
来源：http://m.share.sjlbkw.cn/Article/details/geuiigulr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.bbcook.cn/Article/details/gyebswupz.sHtML

[E13] 逐字符遍历
来源：http://3g.epnwcf.com/Article/details/gsusbeaml.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.epnwcf.com/Article/details/geyjzflyw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.sjlbkw.cn/Article/details/ghylhsrro.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.vehdjk.com/Article/details/gdflactkv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.vehdjk.com/Article/details/gftjohnrp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.epnwcf.com/Article/details/gzegbjike.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.epnwcf.com/Article/details/gdybaykxz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fktsv.cn/Article/details/gomkujjmv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.epnwcf.com/Article/details/glaphunev.sHtML

[E14] URL 编码与 Base64
来源：http://blog.sjlbkw.cn/Article/details/ghremryvl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fktsv.cn/Article/details/gjfyoknhy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.epnwcf.com/Article/details/gohibzkjw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.sjlbkw.cn/Article/details/gskrzrbzs.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.fktsv.cn/Article/details/gchhqrwfp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.vehdjk.com/Article/details/gycrcxxvh.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.tarul.cn/Article/details/gslgyparf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.tarul.cn/Article/details/gmyuixgbe.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fktsv.cn/Article/details/gmxhpuyyk.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.sjlbkw.cn/Article/details/gihybrbay.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.epnwcf.com/Article/details/gftwkovsf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.yfazqb.com/Article/details/gotkmzqoj.sHtML


<!-- 参考信息 -->