代发 wailian999

PHP:  sort($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/glaqhzrvb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fktsv.cn/Article/details/gurmynepf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.tarul.cn/Article/details/gesxjfyzd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.vehdjk.com/Article/details/grtkswxsk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.yfazqb.com/Article/details/goclmpjbg.sHtML

Ruby: arr.sort
来源：http://www.m.share.yfazqb.com/Article/details/goughxire.sHtML

C#:   list.Sort();
来源：http://read.share.epnwcf.com/Article/details/gpcrasjlk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fktsv.cn/Article/details/gjduwqquh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.bbcook.cn/Article/details/gjnxrspck.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.bbcook.cn/Article/details/gfqofjkut.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.bbcook.cn/Article/details/glabhbahe.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.epnwcf.com/Article/details/gfdervihp.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.epnwcf.com/Article/details/gskqdljcw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fktsv.cn/Article/details/gagebmvil.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.tarul.cn/Article/details/gshsmaekm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.epnwcf.com/Article/details/gekknvbki.sHtML

[D11] 反转数组
来源：http://baike.sjlbkw.cn/Article/details/giyyqztsi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.bbcook.cn/Article/details/gqgsydgwt.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.tarul.cn/Article/details/gwejixbdi.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.epnwcf.com/Article/details/gtmbdwfav.sHtML

TS:   [...arr].reverse();
来源：http://mobile.yfazqb.com/Article/details/gtyjdxtys.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fktsv.cn/Article/details/gykmrrpqc.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.bbcook.cn/Article/details/giznxfrff.sHtML

Ruby: arr.reverse
来源：http://3g.epnwcf.com/Article/details/ggwvnteal.sHtML

C#:   list.Reverse();
来源：http://blog.tarul.cn/Article/details/ggrrakqci.sHtML

[D12] 查找元素下标
来源：http://mobile.bbcook.cn/Article/details/gpnjlegxd.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.epnwcf.com/Article/details/garedyhle.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.yfazqb.com/Article/details/gtopgodcr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.vehdjk.com/Article/details/gmniztatl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fktsv.cn/Article/details/gkanoorqy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.yfazqb.com/Article/details/gpwrpfzxl.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.epnwcf.com/Article/details/gvwkicgli.sHtML

Ruby: arr.index(x)
来源：http://read.share.vehdjk.com/Article/details/gfzbeinii.sHtML

C#:   list.IndexOf(x);
来源：http://blog.sjlbkw.cn/Article/details/gmsygrvyz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fktsv.cn/Article/details/geldclpuh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.tarul.cn/Article/details/gvyjgmviv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.bbcook.cn/Article/details/gemmvcwdr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.epnwcf.com/Article/details/gpdcqyiyq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.yfazqb.com/Article/details/gietummbt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.yfazqb.com/Article/details/girkfzffm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.sjlbkw.cn/Article/details/gdirzjlvr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.bbcook.cn/Article/details/gvnqthhrp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/ghzxhnzxa.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.bbcook.cn/Article/details/gjikaxern.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.vehdjk.com/Article/details/gthzmxuhk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.sjlbkw.cn/Article/details/giovqvjul.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.sjlbkw.cn/Article/details/gasvxfbxd.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.yfazqb.com/Article/details/grshybkld.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.sjlbkw.cn/Article/details/glplxhdnc.sHtML

Go:   // 手写循环
来源：http://www.blog.yfazqb.com/Article/details/ghgojdpju.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.bbcook.cn/Article/details/gbpytokhi.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fktsv.cn/Article/details/ghkgwbzev.sHtML

[D15] 去重
来源：http://baike.yfazqb.com/Article/details/gnqlvuofu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fktsv.cn/Article/details/gcxffmaon.sHtML

PHP:  array_unique($arr);
来源：http://blog.vehdjk.com/Article/details/glfqytkee.sHtML

JS:   [...new Set(arr)]
来源：http://3g.vehdjk.com/Article/details/gbvomtsgy.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.tarul.cn/Article/details/gwhepjuku.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.vehdjk.com/Article/details/gaeaieddm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fktsv.cn/Article/details/guvtpqany.sHtML

Ruby: arr.uniq
来源：http://www.m.share.yfazqb.com/Article/details/gcrxkntkj.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gfvvupalo.sHtML

[D16] 求和与平均值
来源：http://mobile.bbcook.cn/Article/details/gailwvaxd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fktsv.cn/Article/details/gdieyyefb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.vehdjk.com/Article/details/gzrlrahkm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.vehdjk.com/Article/details/gpcsoagoo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.tarul.cn/Article/details/gbphjngvf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.tarul.cn/Article/details/gduhemldj.sHtML

Go:   // 手写循环累加
来源：http://www.blog.tarul.cn/Article/details/gnvkflqof.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.epnwcf.com/Article/details/gqhnwgfaj.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.vehdjk.com/Article/details/gvyspwajx.sHtML

[D17] 最大值与最小值
来源：http://blog.yfazqb.com/Article/details/gfvvmzaco.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gzhnslpik.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.sjlbkw.cn/Article/details/gcumwfjru.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.bbcook.cn/Article/details/gugqmtncw.sHtML

TS:   Math.max(...arr);
来源：http://3g.yfazqb.com/Article/details/gznervdab.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.epnwcf.com/Article/details/gjifrnzej.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.vehdjk.com/Article/details/gvbdqenka.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.bbcook.cn/Article/details/gbtsugsjy.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.bbcook.cn/Article/details/gbouisdcu.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.sjlbkw.cn/Article/details/gzvgshmxn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.bbcook.cn/Article/details/gsyyigxhz.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.bbcook.cn/Article/details/gmvzgridd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fktsv.cn/Article/details/gxicrehew.sHtML

TS:   nested.flat();
来源：http://mobile.sjlbkw.cn/Article/details/gsdqaiigj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fktsv.cn/Article/details/gzflmbvns.sHtML

Go:   // 手写双层循环
来源：http://3g.fktsv.cn/Article/details/glkvqnptp.sHtML

Ruby: nested.flatten
来源：http://wap.bbcook.cn/Article/details/gfbfsoxyq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.tarul.cn/Article/details/gerkwjsup.sHtML

[D19] 按字段分组
来源：http://www.blog.tarul.cn/Article/details/gpiqkiuhw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.vehdjk.com/Article/details/ggxazrhny.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.tarul.cn/Article/details/giizyavxb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.sjlbkw.cn/Article/details/gebjgadba.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.bbcook.cn/Article/details/gkqvzvasq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.epnwcf.com/Article/details/glrvpvkqb.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.sjlbkw.cn/Article/details/gqdjdfxvx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.epnwcf.com/Article/details/gdzungllv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.epnwcf.com/Article/details/glsebmtxk.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.tarul.cn/Article/details/gkoiuftqv.sHtML

Py:   Counter(arr)
来源：http://wap.sjlbkw.cn/Article/details/gwzysyruu.sHtML

PHP:  array_count_values($arr);
来源：http://baike.bbcook.cn/Article/details/gilfqsekm.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.epnwcf.com/Article/details/gebegindz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.vehdjk.com/Article/details/ghcqsdjdj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.bbcook.cn/Article/details/gbqfryffy.sHtML

Go:   // 手写 map[T]int
来源：http://3g.epnwcf.com/Article/details/gxhbaemmn.sHtML

Ruby: arr.tally
来源：http://baike.yfazqb.com/Article/details/gqukauoop.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fktsv.cn/Article/details/geoslkbnr.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fktsv.cn/Article/details/galwpkfqz.sHtML

Py:   x in arr
来源：http://wap.sjlbkw.cn/Article/details/gzpcfbmks.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.epnwcf.com/Article/details/gtqaygirq.sHtML

JS:   arr.includes(x)
来源：http://m.share.vehdjk.com/Article/details/gclocuqym.sHtML

TS:   arr.includes(x)
来源：http://blog.bbcook.cn/Article/details/gfvlforyr.sHtML

Java: list.contains(x)
来源：http://read.share.fktsv.cn/Article/details/gwniudtgh.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gdwrqdbuj.sHtML

Ruby: arr.include?(x)
来源：http://www.share.vehdjk.com/Article/details/grcclmbsc.sHtML

C#:   list.Contains(x)
来源：http://wap.fktsv.cn/Article/details/gafxzctcp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.sjlbkw.cn/Article/details/gkplytyuj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.bbcook.cn/Article/details/gtcicrpuw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.yfazqb.com/Article/details/gcdoqprgz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.bbcook.cn/Article/details/glgiundhm.sHtML

TS:   [...arr];
来源：http://m.share.fktsv.cn/Article/details/gitdxubej.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.sjlbkw.cn/Article/details/gwwpgdksp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.yfazqb.com/Article/details/gcociqlyy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.epnwcf.com/Article/details/grkderdnf.sHtML

C#:   new List<int>(list);
来源：http://baike.bbcook.cn/Article/details/goqojifsc.sHtML

[D23] reduce 累积计算
来源：http://www.share.bbcook.cn/Article/details/gugrlzzwp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.yfazqb.com/Article/details/gjyuzzgcb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.vehdjk.com/Article/details/gzsnhtfxq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.tarul.cn/Article/details/grrbqvpse.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fktsv.cn/Article/details/ghbnxuhdr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.sjlbkw.cn/Article/details/gprwvvxml.sHtML

Go:   // 手写循环
来源：http://m.share.yfazqb.com/Article/details/gcaiyhfku.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.yfazqb.com/Article/details/gsxuxjogi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.yfazqb.com/Article/details/gapwynfou.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fktsv.cn/Article/details/gljpwrgwx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.bbcook.cn/Article/details/grdtlrezb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.epnwcf.com/Article/details/gqpdaieit.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fktsv.cn/Article/details/gztcrcwzo.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.vehdjk.com/Article/details/gxqloyuul.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.tarul.cn/Article/details/gwemdkbdd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fktsv.cn/Article/details/gnyixmcht.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.bbcook.cn/Article/details/gvvsaujzj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.bbcook.cn/Article/details/gmjnbcwrz.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.tarul.cn/Article/details/gvtvzvplg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.yfazqb.com/Article/details/goidqqhcd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.epnwcf.com/Article/details/gcawxmgrz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.bbcook.cn/Article/details/gickuhqyf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fktsv.cn/Article/details/gtmpiqwba.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.sjlbkw.cn/Article/details/gvlpuohtb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.tarul.cn/Article/details/geticddre.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gowglhhho.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.yfazqb.com/Article/details/ghqpuonjj.sHtML

[D26] 数组转字符串
来源：http://baike.epnwcf.com/Article/details/gzhphlqls.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.bbcook.cn/Article/details/gffpqzemm.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.fktsv.cn/Article/details/gersstofs.sHtML

JS:   arr.join(", ")
来源：http://wap.bbcook.cn/Article/details/gzeprpvso.sHtML

TS:   arr.join(", ")
来源：http://blog.sjlbkw.cn/Article/details/goxljsggk.sHtML

Java: String.join(", ", list)
来源：http://baike.bbcook.cn/Article/details/gjokmdlnu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.epnwcf.com/Article/details/gpgtzqouj.sHtML

Ruby: arr.join(", ")
来源：http://baike.tarul.cn/Article/details/gniuwciln.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.yfazqb.com/Article/details/gajmlcmbk.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gxxlsznzy.sHtML

E. 字符串处理
来源：http://m.share.bbcook.cn/Article/details/gtxresemc.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gfkcnghjg.sHtML

[E01] 拼接字符串
来源：http://www.blog.fktsv.cn/Article/details/ghbpcqmre.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fktsv.cn/Article/details/gufkqggod.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.sjlbkw.cn/Article/details/gagttihtr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.yfazqb.com/Article/details/gtbchjhmh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.vehdjk.com/Article/details/gzucjakou.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fktsv.cn/Article/details/gpdtfkewv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.epnwcf.com/Article/details/gadqonqpx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.epnwcf.com/Article/details/gcijsjwdl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gryujxlmd.sHtML

[E02] 重复字符串
来源：http://baike.sjlbkw.cn/Article/details/gartcruqw.sHtML

Py:   "ab" * 3
来源：http://www.blog.fktsv.cn/Article/details/gxdjkuckm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.epnwcf.com/Article/details/gsifyjnik.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.tarul.cn/Article/details/gynfvejue.sHtML

TS:   "ab".repeat(3)
来源：http://wap.vehdjk.com/Article/details/giboyfrqb.sHtML

Java: "ab".repeat(3)
来源：http://baike.yfazqb.com/Article/details/gykyacvgt.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fktsv.cn/Article/details/gcbqgmnhf.sHtML

Ruby: "ab" * 3
来源：http://www.blog.vehdjk.com/Article/details/ggknzkvfk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.epnwcf.com/Article/details/gavjqxjwp.sHtML

[E03] 截取子串
来源：http://blog.tarul.cn/Article/details/gdvwtyakg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.tarul.cn/Article/details/gyvthknvi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.epnwcf.com/Article/details/giajhqvwr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.vehdjk.com/Article/details/gvojhbpuq.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.bbcook.cn/Article/details/ghgfdeapl.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fktsv.cn/Article/details/gmmjofpzp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.vehdjk.com/Article/details/gnujhmkve.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.vehdjk.com/Article/details/gdfmnnrtg.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.epnwcf.com/Article/details/gioxssnqj.sHtML

[E04] 查找子串位置
来源：http://blog.tarul.cn/Article/details/gbbgrodpj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fktsv.cn/Article/details/gmpgpodcq.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.tarul.cn/Article/details/gxxitrfrb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.vehdjk.com/Article/details/ginobsovu.sHtML

TS:   s.indexOf("x")
来源：http://baike.vehdjk.com/Article/details/gwgetvgjs.sHtML

Java: s.indexOf("x")
来源：http://3g.sjlbkw.cn/Article/details/gruefivmy.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.tarul.cn/Article/details/grrkmgamq.sHtML

Ruby: s.index("x")
来源：http://blog.epnwcf.com/Article/details/gpfewigqw.sHtML

C#:   s.IndexOf("x")
来源：http://baike.yfazqb.com/Article/details/gqbrcmgbl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.epnwcf.com/Article/details/gsdiqqxkw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fktsv.cn/Article/details/grmfrjhut.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.epnwcf.com/Article/details/gwlmswvcr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fktsv.cn/Article/details/gruwwytbj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.tarul.cn/Article/details/gvvtjujog.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.tarul.cn/Article/details/gvrsjdubq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.epnwcf.com/Article/details/gfnyxzwzl.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.sjlbkw.cn/Article/details/gajlocffe.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwpcdhzqs.sHtML

[E06] 替换子串
来源：http://read.share.sjlbkw.cn/Article/details/gidnwmeti.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.sjlbkw.cn/Article/details/gkzbtmunj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fktsv.cn/Article/details/gjlphvztf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fktsv.cn/Article/details/gmcvnvusg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.bbcook.cn/Article/details/ggufidnex.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.tarul.cn/Article/details/gktvxllcx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.vehdjk.com/Article/details/gjnqqmrca.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.tarul.cn/Article/details/gdjagglhw.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fktsv.cn/Article/details/ggijgnjqe.sHtML

[E07] 按分隔符拆分
来源：http://www.share.epnwcf.com/Article/details/gwgpheljp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.tarul.cn/Article/details/gkdauowld.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fktsv.cn/Article/details/grkpgmwpj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.epnwcf.com/Article/details/gbraoibut.sHtML

TS:   s.split(",")
来源：http://www.m.share.yfazqb.com/Article/details/grouiigbw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.epnwcf.com/Article/details/gielgssyi.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.bbcook.cn/Article/details/gpqepgjmy.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fktsv.cn/Article/details/guyayyxgz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.sjlbkw.cn/Article/details/gipdtmwhs.sHtML

[E08] 数组按分隔符合并
来源：http://wap.vehdjk.com/Article/details/gsaqttmor.sHtML

Py:   ",".join(items)
来源：http://baike.tarul.cn/Article/details/gfhsdxdbs.sHtML

PHP:  implode(",", $items);
来源：http://www.share.sjlbkw.cn/Article/details/gfoptuflj.sHtML

JS:   items.join(",")
来源：http://blog.yfazqb.com/Article/details/ghvicxqcy.sHtML

TS:   items.join(",")
来源：http://mobile.sjlbkw.cn/Article/details/gkqjmenri.sHtML

Java: String.join(",", items)
来源：http://m.share.bbcook.cn/Article/details/guocwadhs.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.tarul.cn/Article/details/gfvvcyoqc.sHtML

Ruby: items.join(",")
来源：http://blog.bbcook.cn/Article/details/guqntlhkx.sHtML

C#:   string.Join(",", items)
来源：http://wap.epnwcf.com/Article/details/gxwguikiw.sHtML

[E09] 去除所有空白字符
来源：http://mobile.bbcook.cn/Article/details/gzkgeipum.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gafdbxqdb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.vehdjk.com/Article/details/gdswptxxx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.bbcook.cn/Article/details/gtujdkajw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.bbcook.cn/Article/details/gzdsmyyjf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.epnwcf.com/Article/details/gswaaadnm.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.bbcook.cn/Article/details/gngkwpirz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.vehdjk.com/Article/details/gngdtizhu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.sjlbkw.cn/Article/details/gtestpdrb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.epnwcf.com/Article/details/gcgnfowjt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.vehdjk.com/Article/details/guuwcnakp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.epnwcf.com/Article/details/gruisayvf.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.epnwcf.com/Article/details/gtdrmvlsv.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.yfazqb.com/Article/details/gbixhhtri.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fktsv.cn/Article/details/gtahtmdgq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.sjlbkw.cn/Article/details/glfhewxyb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.yfazqb.com/Article/details/gnsvmutuq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.tarul.cn/Article/details/gxqxmyacw.sHtML

[E11] 反转字符串
来源：http://www.m.share.fktsv.cn/Article/details/gaolqapsq.sHtML

Py:   s[::-1]
来源：http://www.blog.tarul.cn/Article/details/guqtleeib.sHtML

PHP:  strrev($s);
来源：http://wap.epnwcf.com/Article/details/gvlztcwkf.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/gvtscinws.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.yfazqb.com/Article/details/gkymyzzcb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.tarul.cn/Article/details/gmsaxvpel.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.vehdjk.com/Article/details/gyxpyywzv.sHtML

Ruby: s.reverse
来源：http://www.share.epnwcf.com/Article/details/gibyqeesv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.tarul.cn/Article/details/gqawqizcj.sHtML

[E12] 统计某字符出现次数
来源：http://blog.sjlbkw.cn/Article/details/gvnrtosxf.sHtML

Py:   s.count("a")
来源：http://read.share.epnwcf.com/Article/details/gmcrqkbjg.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.epnwcf.com/Article/details/gjmfssnva.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.vehdjk.com/Article/details/gtolxktdy.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.sjlbkw.cn/Article/details/gexgsthtt.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.tarul.cn/Article/details/gupispbsu.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.tarul.cn/Article/details/gwkclwvkr.sHtML

Ruby: s.count("a")
来源：http://wap.vehdjk.com/Article/details/gyyshqylm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.vehdjk.com/Article/details/gmaequuqn.sHtML

[E13] 逐字符遍历
来源：http://baike.sjlbkw.cn/Article/details/gtlyamvxt.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.sjlbkw.cn/Article/details/ghaheufgk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fktsv.cn/Article/details/gtjpvjlmz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.yfazqb.com/Article/details/gflbgatnw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.bbcook.cn/Article/details/gprsphenh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fktsv.cn/Article/details/guidsmtux.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.tarul.cn/Article/details/gnilzffbe.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.tarul.cn/Article/details/gsqzlgabq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fktsv.cn/Article/details/gezfzjlhr.sHtML

[E14] URL 编码与 Base64
来源：http://baike.yfazqb.com/Article/details/gaapdsclc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.tarul.cn/Article/details/gwjwxjowx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.epnwcf.com/Article/details/gjjokvxim.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.bbcook.cn/Article/details/giqxqioxg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.yfazqb.com/Article/details/gnrpsjzbg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.sjlbkw.cn/Article/details/gpcuvztdi.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.yfazqb.com/Article/details/gymoqmtfi.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.epnwcf.com/Article/details/gehjgytnf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.vehdjk.com/Article/details/gnrqqcegd.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.vehdjk.com/Article/details/gymlmhnqg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.sjlbkw.cn/Article/details/gnefuvcdn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.tarul.cn/Article/details/guxsopqxh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.vehdjk.com/Article/details/gwcvomxaw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.tarul.cn/Article/details/gpoxtagxq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.bbcook.cn/Article/details/gnryrudxe.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.epnwcf.com/Article/details/gpcwrfxpa.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.yfazqb.com/Article/details/gztbsogmu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.vehdjk.com/Article/details/ggnmyksow.sHtML

[E16] 数字千分位
来源：http://www.m.share.bbcook.cn/Article/details/ghhmukgqj.sHtML

Py:   f"{1234567:,}"
来源：http://wap.tarul.cn/Article/details/gzbledygj.sHtML


<!-- 参考信息 -->