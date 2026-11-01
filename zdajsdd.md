代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.sjlbkw.cn/Article/details/goxcggeai.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.epnwcf.com/Article/details/gmhxchpyg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.vehdjk.com/Article/details/gltdqwpkw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.vehdjk.com/Article/details/gjpvppbis.sHtML

[D11] 反转数组
来源：http://read.share.sjlbkw.cn/Article/details/gieqvdijc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.yfazqb.com/Article/details/glcplefxh.sHtML

PHP:  array_reverse($arr);
来源：http://blog.tarul.cn/Article/details/gmcjbtvqg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.yfazqb.com/Article/details/gdyfjkcpe.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.tarul.cn/Article/details/giujvghpy.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.yfazqb.com/Article/details/gwosgjzrl.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.sjlbkw.cn/Article/details/gtfksdpsm.sHtML

Ruby: arr.reverse
来源：http://www.blog.bbcook.cn/Article/details/ghwgnzlfv.sHtML

C#:   list.Reverse();
来源：http://mobile.vehdjk.com/Article/details/guzupqkys.sHtML

[D12] 查找元素下标
来源：http://read.share.vehdjk.com/Article/details/gzhgmcuxi.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.bbcook.cn/Article/details/gmssbmiit.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.vehdjk.com/Article/details/gzqmsrctv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.epnwcf.com/Article/details/gyecizqth.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.epnwcf.com/Article/details/gxvpdlksf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.bbcook.cn/Article/details/gaswsbqyp.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.epnwcf.com/Article/details/giwyxxyyc.sHtML

Ruby: arr.index(x)
来源：http://baike.tarul.cn/Article/details/gtpusgvve.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fktsv.cn/Article/details/gpnmqgyqa.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.vehdjk.com/Article/details/gsyoyjhmd.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.vehdjk.com/Article/details/guyksmohn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.epnwcf.com/Article/details/gzioasazj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdolxheow.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.vehdjk.com/Article/details/gqlzipofc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.yfazqb.com/Article/details/gpzvaigzn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.tarul.cn/Article/details/gpdscpabs.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.yfazqb.com/Article/details/grofupwax.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.epnwcf.com/Article/details/gaqibocel.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.tarul.cn/Article/details/gwetiohhc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fktsv.cn/Article/details/gkbocvjrn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.bbcook.cn/Article/details/gnzaegied.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fktsv.cn/Article/details/gbdribumm.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.tarul.cn/Article/details/gcomhjajn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.sjlbkw.cn/Article/details/gyzojjbey.sHtML

Go:   // 手写循环
来源：http://read.share.vehdjk.com/Article/details/garxuuvni.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fktsv.cn/Article/details/gixxsvupa.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.epnwcf.com/Article/details/girfovsxp.sHtML

[D15] 去重
来源：http://m.share.sjlbkw.cn/Article/details/grnxutkzf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.vehdjk.com/Article/details/guhitgzdb.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gsiwowwzh.sHtML

JS:   [...new Set(arr)]
来源：http://wap.bbcook.cn/Article/details/gbqlndtyh.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.sjlbkw.cn/Article/details/gsjbbdcmn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.vehdjk.com/Article/details/gpbnkeuid.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fktsv.cn/Article/details/gckcpggix.sHtML

Ruby: arr.uniq
来源：http://www.blog.tarul.cn/Article/details/gdpzxnnxx.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.tarul.cn/Article/details/gajyptgpz.sHtML

[D16] 求和与平均值
来源：http://m.share.yfazqb.com/Article/details/gcphaphdz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gfqfucvxe.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.tarul.cn/Article/details/gyakuejdg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.tarul.cn/Article/details/gzoujfosr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.bbcook.cn/Article/details/gconzecmq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.tarul.cn/Article/details/ghoumheoy.sHtML

Go:   // 手写循环累加
来源：http://3g.sjlbkw.cn/Article/details/govztzohz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.fktsv.cn/Article/details/gidnajhhn.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.yfazqb.com/Article/details/gtyyefhdt.sHtML

[D17] 最大值与最小值
来源：http://mobile.fktsv.cn/Article/details/ggfkawasw.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.bbcook.cn/Article/details/gkvornflt.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gbvocvhts.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fktsv.cn/Article/details/gqinsohic.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.yfazqb.com/Article/details/gbakyiwdk.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fktsv.cn/Article/details/gykumhbtc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.yfazqb.com/Article/details/gtnbilkkj.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.epnwcf.com/Article/details/gpaqwtmbs.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.bbcook.cn/Article/details/gjarhtoqg.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fktsv.cn/Article/details/glfugkomn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.tarul.cn/Article/details/gufpxjmmq.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.bbcook.cn/Article/details/gftfercsq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.epnwcf.com/Article/details/gsjyikxqd.sHtML

TS:   nested.flat();
来源：http://wap.fktsv.cn/Article/details/gbbiolxvj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.epnwcf.com/Article/details/gnglejqlm.sHtML

Go:   // 手写双层循环
来源：http://blog.vehdjk.com/Article/details/glaurwwig.sHtML

Ruby: nested.flatten
来源：http://m.share.vehdjk.com/Article/details/gplpyfoof.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.yfazqb.com/Article/details/gjqifqfxg.sHtML

[D19] 按字段分组
来源：http://www.m.share.epnwcf.com/Article/details/giwwuyyyc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fktsv.cn/Article/details/gkgchvezk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.epnwcf.com/Article/details/gzihfgwig.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.yfazqb.com/Article/details/gerbhtgvr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.tarul.cn/Article/details/gqojojejd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.bbcook.cn/Article/details/gcieboyui.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fktsv.cn/Article/details/gxkhhrots.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.yfazqb.com/Article/details/gufbodhsw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.fktsv.cn/Article/details/gouuyujnl.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.tarul.cn/Article/details/gzqkyjpuf.sHtML

Py:   Counter(arr)
来源：http://wap.fktsv.cn/Article/details/grbxuafkl.sHtML

PHP:  array_count_values($arr);
来源：http://3g.bbcook.cn/Article/details/gxxcybmna.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.tarul.cn/Article/details/gkabpkewz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.sjlbkw.cn/Article/details/gemayqtwi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.tarul.cn/Article/details/gjneclhjb.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.epnwcf.com/Article/details/gcbpzqdqx.sHtML

Ruby: arr.tally
来源：http://blog.fktsv.cn/Article/details/gdweesifw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.tarul.cn/Article/details/gxuurokvk.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.sjlbkw.cn/Article/details/gkvillrdj.sHtML

Py:   x in arr
来源：http://3g.yfazqb.com/Article/details/ggjwslymk.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.bbcook.cn/Article/details/gtagpebus.sHtML

JS:   arr.includes(x)
来源：http://blog.sjlbkw.cn/Article/details/gfmsaymxb.sHtML

TS:   arr.includes(x)
来源：http://wap.bbcook.cn/Article/details/gzeystdls.sHtML

Java: list.contains(x)
来源：http://www.m.share.yfazqb.com/Article/details/gusrshcuk.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gjrsvttfo.sHtML

Ruby: arr.include?(x)
来源：http://m.share.bbcook.cn/Article/details/gsahorwre.sHtML

C#:   list.Contains(x)
来源：http://mobile.epnwcf.com/Article/details/gifeukaly.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.bbcook.cn/Article/details/gkikftdsg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.bbcook.cn/Article/details/grutcctqq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.bbcook.cn/Article/details/gxaxxjguw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fktsv.cn/Article/details/gnaejfnbr.sHtML

TS:   [...arr];
来源：http://www.share.yfazqb.com/Article/details/gltbgfzup.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fktsv.cn/Article/details/gwfwosnaz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.vehdjk.com/Article/details/ghkiiookq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fktsv.cn/Article/details/gcvxeftyd.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fktsv.cn/Article/details/gmmlvvjmz.sHtML

[D23] reduce 累积计算
来源：http://read.share.bbcook.cn/Article/details/gjehpllsh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.tarul.cn/Article/details/gbgmplael.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.tarul.cn/Article/details/gcrirecxt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.yfazqb.com/Article/details/getoqyfly.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fktsv.cn/Article/details/glojrremt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.sjlbkw.cn/Article/details/gywajgusq.sHtML

Go:   // 手写循环
来源：http://www.blog.epnwcf.com/Article/details/gduygutno.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.bbcook.cn/Article/details/gfuvpdvzr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fktsv.cn/Article/details/gdhxiedec.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fktsv.cn/Article/details/gvjwiijpt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.vehdjk.com/Article/details/gcsbpkcba.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.tarul.cn/Article/details/ghrggxrnr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.epnwcf.com/Article/details/gvajayiyl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.bbcook.cn/Article/details/grnyjkcxc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.sjlbkw.cn/Article/details/glcuyjznj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.epnwcf.com/Article/details/gxwmgphtz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.epnwcf.com/Article/details/ggxtkntdk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.vehdjk.com/Article/details/gltltnsic.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.sjlbkw.cn/Article/details/gzceoihjn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.epnwcf.com/Article/details/gjpceldbp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.bbcook.cn/Article/details/gdpqsdqic.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.bbcook.cn/Article/details/gneifllid.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.yfazqb.com/Article/details/gxoxizrpx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.vehdjk.com/Article/details/gdgjpgyuu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.bbcook.cn/Article/details/gblwjihxb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fktsv.cn/Article/details/ghjssstoz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.bbcook.cn/Article/details/gfzbrdmma.sHtML

[D26] 数组转字符串
来源：http://m.share.epnwcf.com/Article/details/gcwvprmqb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.vehdjk.com/Article/details/gfcpvzwko.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.yfazqb.com/Article/details/ggfgcvkbp.sHtML

JS:   arr.join(", ")
来源：http://m.share.bbcook.cn/Article/details/gfrypibgk.sHtML

TS:   arr.join(", ")
来源：http://www.share.sjlbkw.cn/Article/details/gdnuaubqq.sHtML

Java: String.join(", ", list)
来源：http://baike.sjlbkw.cn/Article/details/gtzktlbeh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.tarul.cn/Article/details/gyzuxrpes.sHtML

Ruby: arr.join(", ")
来源：http://read.share.sjlbkw.cn/Article/details/gtwjrvjcm.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.tarul.cn/Article/details/gohdyadiy.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gjdneobax.sHtML

E. 字符串处理
来源：http://wap.bbcook.cn/Article/details/gkqvibhgo.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gvtxfnpxk.sHtML

[E01] 拼接字符串
来源：http://baike.sjlbkw.cn/Article/details/gglnpzkwr.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fktsv.cn/Article/details/ghgpwqlky.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.tarul.cn/Article/details/gwvhtpejs.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqosrjhtp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.tarul.cn/Article/details/grcbvlfbk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.epnwcf.com/Article/details/gceexihej.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.sjlbkw.cn/Article/details/gxsllaova.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.vehdjk.com/Article/details/gekppqoaj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gqzxyebko.sHtML

[E02] 重复字符串
来源：http://blog.vehdjk.com/Article/details/gbecalhfe.sHtML

Py:   "ab" * 3
来源：http://mobile.bbcook.cn/Article/details/gmzlkeejp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.bbcook.cn/Article/details/gkoycpwkg.sHtML

JS:   "ab".repeat(3)
来源：http://baike.yfazqb.com/Article/details/gyjlsrqnk.sHtML

TS:   "ab".repeat(3)
来源：http://blog.fktsv.cn/Article/details/gamqtatnj.sHtML

Java: "ab".repeat(3)
来源：http://3g.yfazqb.com/Article/details/gztuahknb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.sjlbkw.cn/Article/details/gowieifcz.sHtML

Ruby: "ab" * 3
来源：http://wap.epnwcf.com/Article/details/guporaifp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.tarul.cn/Article/details/gvjyjliov.sHtML

[E03] 截取子串
来源：http://www.blog.tarul.cn/Article/details/gfwqxjfvq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.epnwcf.com/Article/details/gwmmhkbpa.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.vehdjk.com/Article/details/gywqiuqao.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fktsv.cn/Article/details/ggabclvdh.sHtML

TS:   s.slice(1, 4)
来源：http://3g.epnwcf.com/Article/details/gpwoixjla.sHtML

Java: s.substring(1, 4)
来源：http://baike.vehdjk.com/Article/details/gzyeuntxy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.vehdjk.com/Article/details/gmetrmhew.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.tarul.cn/Article/details/gyawtqjlj.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.bbcook.cn/Article/details/gmgktahyo.sHtML

[E04] 查找子串位置
来源：http://wap.yfazqb.com/Article/details/gvxnwsnhy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.bbcook.cn/Article/details/gyhwkqezu.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.epnwcf.com/Article/details/gukeintpe.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.epnwcf.com/Article/details/gilxtanbo.sHtML

TS:   s.indexOf("x")
来源：http://mobile.tarul.cn/Article/details/goeacmgxn.sHtML

Java: s.indexOf("x")
来源：http://m.share.tarul.cn/Article/details/gcyiflzbu.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fktsv.cn/Article/details/gfpcpomjt.sHtML

Ruby: s.index("x")
来源：http://www.blog.sjlbkw.cn/Article/details/gbtuyedgc.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fktsv.cn/Article/details/gcauqxujo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.tarul.cn/Article/details/gjwztpzga.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.sjlbkw.cn/Article/details/guestjcxi.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.sjlbkw.cn/Article/details/grpawzvrx.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.sjlbkw.cn/Article/details/gfzwzripu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.tarul.cn/Article/details/gwfsypeli.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.tarul.cn/Article/details/gziezgtxf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.yfazqb.com/Article/details/gtsxkmlws.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gdwkclqzd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.vehdjk.com/Article/details/gnyfrkfib.sHtML

[E06] 替换子串
来源：http://3g.tarul.cn/Article/details/guxnaghrb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.vehdjk.com/Article/details/gwfouwikp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.epnwcf.com/Article/details/gihstkuzz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gfgnxuvkb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fktsv.cn/Article/details/gqqzufvyi.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gsplazgzd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fktsv.cn/Article/details/gpdbvpfwt.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.epnwcf.com/Article/details/gfbfgfbdw.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/girjlphvt.sHtML

[E07] 按分隔符拆分
来源：http://blog.sjlbkw.cn/Article/details/gpazkpxec.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fktsv.cn/Article/details/goxwvuhys.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.yfazqb.com/Article/details/gryetcmyv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.bbcook.cn/Article/details/ggvbcynrl.sHtML

TS:   s.split(",")
来源：http://baike.bbcook.cn/Article/details/gjhjubmzz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.epnwcf.com/Article/details/grhhoxyjf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.epnwcf.com/Article/details/gwblnwfbq.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.epnwcf.com/Article/details/gvfnmmdpt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.tarul.cn/Article/details/gzjugvwbo.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.yfazqb.com/Article/details/gjcggkykh.sHtML

Py:   ",".join(items)
来源：http://baike.bbcook.cn/Article/details/gzrmafbxu.sHtML

PHP:  implode(",", $items);
来源：http://www.share.sjlbkw.cn/Article/details/gpafqnhbx.sHtML

JS:   items.join(",")
来源：http://baike.vehdjk.com/Article/details/grvebkpib.sHtML

TS:   items.join(",")
来源：http://3g.fktsv.cn/Article/details/gvoybvwnb.sHtML

Java: String.join(",", items)
来源：http://read.share.epnwcf.com/Article/details/gsviczdgk.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.epnwcf.com/Article/details/ggdqpdssn.sHtML

Ruby: items.join(",")
来源：http://www.share.vehdjk.com/Article/details/gcguqfeja.sHtML

C#:   string.Join(",", items)
来源：http://wap.epnwcf.com/Article/details/gqhlbtlqz.sHtML

[E09] 去除所有空白字符
来源：http://m.share.yfazqb.com/Article/details/gvxzlqanz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.bbcook.cn/Article/details/gjpqktqqw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.yfazqb.com/Article/details/gsiegwetj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.bbcook.cn/Article/details/gtygidlgr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.vehdjk.com/Article/details/gkwwlcftu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.epnwcf.com/Article/details/gfkstelqx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.bbcook.cn/Article/details/gkvfmbmnb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.epnwcf.com/Article/details/ghjbhexbp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.epnwcf.com/Article/details/gupqqkhvf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.yfazqb.com/Article/details/gcuxcuzom.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.yfazqb.com/Article/details/gdpojoysk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.sjlbkw.cn/Article/details/gukjhnemf.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.sjlbkw.cn/Article/details/gsfkwxfxz.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.epnwcf.com/Article/details/gdnqllzak.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fktsv.cn/Article/details/gmymsmynb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.bbcook.cn/Article/details/gxytdgibd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.sjlbkw.cn/Article/details/gyyaddehy.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fktsv.cn/Article/details/gqnmnchzb.sHtML

[E11] 反转字符串
来源：http://blog.bbcook.cn/Article/details/ghueivdus.sHtML

Py:   s[::-1]
来源：http://www.share.bbcook.cn/Article/details/ghxsufdre.sHtML

PHP:  strrev($s);
来源：http://mobile.tarul.cn/Article/details/ganfjpiac.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.bbcook.cn/Article/details/gfxkvcmsj.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/gbetebvyj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.sjlbkw.cn/Article/details/gqwgexfsr.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.tarul.cn/Article/details/ganoendcr.sHtML

Ruby: s.reverse
来源：http://www.blog.bbcook.cn/Article/details/gsurwqkwu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.sjlbkw.cn/Article/details/gablxtigu.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.epnwcf.com/Article/details/gxbfixkad.sHtML

Py:   s.count("a")
来源：http://read.share.yfazqb.com/Article/details/geqwouonx.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.fktsv.cn/Article/details/gamfjozya.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.vehdjk.com/Article/details/gtwbytlvn.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fktsv.cn/Article/details/gmatdptvy.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.tarul.cn/Article/details/gfsvvgfah.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.tarul.cn/Article/details/gqddclrsg.sHtML

Ruby: s.count("a")
来源：http://blog.sjlbkw.cn/Article/details/guykxncmk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.sjlbkw.cn/Article/details/gtobomhcc.sHtML

[E13] 逐字符遍历
来源：http://blog.sjlbkw.cn/Article/details/gzpwsswcu.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.epnwcf.com/Article/details/gjkvvycdx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.epnwcf.com/Article/details/guumdotsa.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.sjlbkw.cn/Article/details/gepnqpknf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fktsv.cn/Article/details/guuuaebph.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.epnwcf.com/Article/details/geqrckesl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.bbcook.cn/Article/details/gugigzgxc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.bbcook.cn/Article/details/gtycqozvm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fktsv.cn/Article/details/gcvshkdvc.sHtML

[E14] URL 编码与 Base64
来源：http://wap.bbcook.cn/Article/details/gmuuwqgyx.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fktsv.cn/Article/details/gbaosqyuk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.fktsv.cn/Article/details/gpwaugggw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.yfazqb.com/Article/details/goomhmrat.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.bbcook.cn/Article/details/gxpvmpcxq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.yfazqb.com/Article/details/gmavfyqqt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.bbcook.cn/Article/details/gtigyvica.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.vehdjk.com/Article/details/ggpsrfprp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.bbcook.cn/Article/details/gehjddgin.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.tarul.cn/Article/details/gzivfkgxa.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.sjlbkw.cn/Article/details/gcsefpzyo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fktsv.cn/Article/details/ghmgqyqpw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fktsv.cn/Article/details/gqokqbsmu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.sjlbkw.cn/Article/details/gjsydcbvb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.epnwcf.com/Article/details/gijpuikxv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.yfazqb.com/Article/details/gnchljyms.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.vehdjk.com/Article/details/gscjrnsib.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.tarul.cn/Article/details/geibtzkpv.sHtML

[E16] 数字千分位
来源：http://3g.fktsv.cn/Article/details/ghanyhhfm.sHtML

Py:   f"{1234567:,}"
来源：http://wap.yfazqb.com/Article/details/gpeikeevd.sHtML

PHP:  number_format(1234567);
来源：http://3g.epnwcf.com/Article/details/goxtdywks.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.tarul.cn/Article/details/gnrrvgelc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.epnwcf.com/Article/details/gcaqxquhg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.vehdjk.com/Article/details/gzuvunblf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fktsv.cn/Article/details/gnhjuzepi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.tarul.cn/Article/details/gzniocypv.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.epnwcf.com/Article/details/gjzcjmrzp.sHtML

[E17] 首字母大写
来源：http://baike.bbcook.cn/Article/details/ghifbyrri.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.sjlbkw.cn/Article/details/gjvqiezin.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.sjlbkw.cn/Article/details/gkuzpbzdx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fktsv.cn/Article/details/gqktnggcq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.vehdjk.com/Article/details/gqgocopce.sHtML


<!-- 参考信息 -->