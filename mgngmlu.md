代发 wailian999

C#:   list.Reverse();
来源：http://wap.bbcook.cn/Article/details/gejwbteds.sHtML

[D12] 查找元素下标
来源：http://www.blog.sjlbkw.cn/Article/details/goguswlcx.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.sjlbkw.cn/Article/details/gktxpntiu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.sjlbkw.cn/Article/details/gmeragiff.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.sjlbkw.cn/Article/details/gndjcnzbc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.vehdjk.com/Article/details/gslycqcvc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.sjlbkw.cn/Article/details/guwodfhaz.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.vehdjk.com/Article/details/guzaipooe.sHtML

Ruby: arr.index(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gxgupyhlj.sHtML

C#:   list.IndexOf(x);
来源：http://3g.bbcook.cn/Article/details/gmvzmfwgb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.yfazqb.com/Article/details/gmwxyqxsv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.yfazqb.com/Article/details/gbenpiqfo.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.yfazqb.com/Article/details/gijyoutzt.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.vehdjk.com/Article/details/gfrkfiiux.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.bbcook.cn/Article/details/greeagtdk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.sjlbkw.cn/Article/details/gunuhyhfe.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.vehdjk.com/Article/details/gqoipuvgf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.vehdjk.com/Article/details/gjealvjjq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.bbcook.cn/Article/details/gvlywyxqc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fktsv.cn/Article/details/gnwfuocgv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fktsv.cn/Article/details/gihqfpnbs.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.bbcook.cn/Article/details/gstdrilnf.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.vehdjk.com/Article/details/gdndqyoxh.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.vehdjk.com/Article/details/galzpbkcv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.tarul.cn/Article/details/gpcjkafuj.sHtML

Go:   // 手写循环
来源：http://www.blog.tarul.cn/Article/details/geghjflol.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fktsv.cn/Article/details/gpfbcaitp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.yfazqb.com/Article/details/gjiuuhnby.sHtML

[D15] 去重
来源：http://wap.epnwcf.com/Article/details/gxlqwvtzp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.tarul.cn/Article/details/gyftdnvqo.sHtML

PHP:  array_unique($arr);
来源：http://baike.sjlbkw.cn/Article/details/glqrcbnib.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.vehdjk.com/Article/details/gkidnxgpo.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.yfazqb.com/Article/details/gdcnfshag.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fktsv.cn/Article/details/ghsyarppx.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.bbcook.cn/Article/details/gnpuwhowb.sHtML

Ruby: arr.uniq
来源：http://www.m.share.tarul.cn/Article/details/gnrmbjpsz.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.epnwcf.com/Article/details/gixzblkgf.sHtML

[D16] 求和与平均值
来源：http://blog.bbcook.cn/Article/details/gimohuyoo.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.yfazqb.com/Article/details/gczapparv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fktsv.cn/Article/details/gfxwgkvwm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gnolkolut.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.epnwcf.com/Article/details/glkriirzi.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.bbcook.cn/Article/details/gvcciuiek.sHtML

Go:   // 手写循环累加
来源：http://3g.tarul.cn/Article/details/gtrvhigwc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.sjlbkw.cn/Article/details/gyanfqlnv.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fktsv.cn/Article/details/gjhzxdkxw.sHtML

[D17] 最大值与最小值
来源：http://www.share.sjlbkw.cn/Article/details/glopqufar.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.tarul.cn/Article/details/gjzefupnt.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fktsv.cn/Article/details/gbiazzfvn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.tarul.cn/Article/details/gvjwnlmvr.sHtML

TS:   Math.max(...arr);
来源：http://read.share.yfazqb.com/Article/details/goqtsglib.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.bbcook.cn/Article/details/gpcnkvnow.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.epnwcf.com/Article/details/gzvimswxs.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.yfazqb.com/Article/details/gjgbfihqo.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.epnwcf.com/Article/details/gxmbuykuw.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.vehdjk.com/Article/details/gmdkiaoxg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.tarul.cn/Article/details/giboovczx.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.vehdjk.com/Article/details/gfhegzkgl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.sjlbkw.cn/Article/details/gjbtvefdy.sHtML

TS:   nested.flat();
来源：http://3g.vehdjk.com/Article/details/grifzgqom.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.bbcook.cn/Article/details/gabfkhthe.sHtML

Go:   // 手写双层循环
来源：http://m.share.vehdjk.com/Article/details/gdollkfpl.sHtML

Ruby: nested.flatten
来源：http://m.share.fktsv.cn/Article/details/godkwflju.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.epnwcf.com/Article/details/gayalgxtg.sHtML

[D19] 按字段分组
来源：http://mobile.vehdjk.com/Article/details/gdphiobhc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.tarul.cn/Article/details/gykmyrghm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.sjlbkw.cn/Article/details/godleehzx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.sjlbkw.cn/Article/details/gsxamapef.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.tarul.cn/Article/details/grdgppoxb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.sjlbkw.cn/Article/details/ghjrzqytn.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.vehdjk.com/Article/details/gohuadcpi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fktsv.cn/Article/details/ggzcrrxky.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.vehdjk.com/Article/details/greklvhio.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.tarul.cn/Article/details/gsuevlewb.sHtML

Py:   Counter(arr)
来源：http://wap.yfazqb.com/Article/details/gjqeoafib.sHtML

PHP:  array_count_values($arr);
来源：http://baike.yfazqb.com/Article/details/gypthvazd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.tarul.cn/Article/details/ggwxvgjrr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.bbcook.cn/Article/details/goxkiqpgt.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.bbcook.cn/Article/details/gavoglsis.sHtML

Go:   // 手写 map[T]int
来源：http://baike.tarul.cn/Article/details/gryrbtubi.sHtML

Ruby: arr.tally
来源：http://baike.vehdjk.com/Article/details/grkvopdzt.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.epnwcf.com/Article/details/gfpfkdzze.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.vehdjk.com/Article/details/gdmgdjiqy.sHtML

Py:   x in arr
来源：http://3g.vehdjk.com/Article/details/gwmbsmixc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.yfazqb.com/Article/details/gzeybpjzh.sHtML

JS:   arr.includes(x)
来源：http://m.share.tarul.cn/Article/details/gfakkmhmj.sHtML

TS:   arr.includes(x)
来源：http://3g.tarul.cn/Article/details/gbagwwjwx.sHtML

Java: list.contains(x)
来源：http://blog.sjlbkw.cn/Article/details/gzbwekeot.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/gddckgyub.sHtML

Ruby: arr.include?(x)
来源：http://m.share.epnwcf.com/Article/details/girdwomvx.sHtML

C#:   list.Contains(x)
来源：http://www.blog.bbcook.cn/Article/details/gnzxuentf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.vehdjk.com/Article/details/grvywpsho.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.yfazqb.com/Article/details/gubrghgwu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.vehdjk.com/Article/details/ghlbhlplf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gcfcxryob.sHtML

TS:   [...arr];
来源：http://www.blog.epnwcf.com/Article/details/gsjupatew.sHtML

Java: new ArrayList<>(list);
来源：http://wap.sjlbkw.cn/Article/details/gwfoacysr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fktsv.cn/Article/details/ggsbzkige.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fktsv.cn/Article/details/gwhxgdalz.sHtML

C#:   new List<int>(list);
来源：http://baike.fktsv.cn/Article/details/gypknxtaz.sHtML

[D23] reduce 累积计算
来源：http://wap.bbcook.cn/Article/details/gxanaofrw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.epnwcf.com/Article/details/gtvwmikud.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.sjlbkw.cn/Article/details/guwoxebvt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.tarul.cn/Article/details/gqhxmdjeb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.tarul.cn/Article/details/gbkzpkmds.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.yfazqb.com/Article/details/gijsppram.sHtML

Go:   // 手写循环
来源：http://wap.yfazqb.com/Article/details/ggychrpdu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.yfazqb.com/Article/details/glflmylmo.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.bbcook.cn/Article/details/gamwhuceu.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.yfazqb.com/Article/details/gejfhxudp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.sjlbkw.cn/Article/details/gmlmykbhj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.epnwcf.com/Article/details/gzxlzclwb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.bbcook.cn/Article/details/gwtbdvfat.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fktsv.cn/Article/details/gflanebgj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.tarul.cn/Article/details/gosmxteup.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.bbcook.cn/Article/details/ghmnuhlbc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.tarul.cn/Article/details/gnjlmcyoh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.sjlbkw.cn/Article/details/gtkbwmjjt.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.epnwcf.com/Article/details/gfgcpaydi.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.yfazqb.com/Article/details/gucxibecw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.epnwcf.com/Article/details/ggpydnale.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.yfazqb.com/Article/details/gopopohqw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.bbcook.cn/Article/details/gjvihplrt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.yfazqb.com/Article/details/gkpkrzfhl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.epnwcf.com/Article/details/glzkrqqkl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.sjlbkw.cn/Article/details/gizixnbok.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.tarul.cn/Article/details/gvubvgykv.sHtML

[D26] 数组转字符串
来源：http://m.share.sjlbkw.cn/Article/details/gppuwaemk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.epnwcf.com/Article/details/gyxddieuv.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.sjlbkw.cn/Article/details/gswunddnj.sHtML

JS:   arr.join(", ")
来源：http://3g.yfazqb.com/Article/details/gobkmrhnk.sHtML

TS:   arr.join(", ")
来源：http://blog.bbcook.cn/Article/details/goxuecpdv.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.bbcook.cn/Article/details/gkcfpsfke.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.yfazqb.com/Article/details/gwpanplip.sHtML

Ruby: arr.join(", ")
来源：http://baike.bbcook.cn/Article/details/gsguecrfq.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.epnwcf.com/Article/details/gudknylov.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/ggqkaerir.sHtML

E. 字符串处理
来源：http://mobile.epnwcf.com/Article/details/gfxdeyspk.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gbctllopf.sHtML

[E01] 拼接字符串
来源：http://baike.fktsv.cn/Article/details/gzvtwxnva.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.tarul.cn/Article/details/gnhqeduwt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.tarul.cn/Article/details/gxbgvpuec.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.vehdjk.com/Article/details/gxxkwepkh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.epnwcf.com/Article/details/gedsbarnh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.epnwcf.com/Article/details/glyrndhce.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fktsv.cn/Article/details/ghkollagi.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.sjlbkw.cn/Article/details/gbtyytfrt.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fktsv.cn/Article/details/gfvtsptis.sHtML

[E02] 重复字符串
来源：http://wap.sjlbkw.cn/Article/details/guomjbwbs.sHtML

Py:   "ab" * 3
来源：http://3g.yfazqb.com/Article/details/gpgxknjrk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.vehdjk.com/Article/details/gilmuoybn.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.tarul.cn/Article/details/gxluyzvdc.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.tarul.cn/Article/details/gorxtukcz.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.tarul.cn/Article/details/gpadtdkpu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.sjlbkw.cn/Article/details/gcyicnpdx.sHtML

Ruby: "ab" * 3
来源：http://www.blog.tarul.cn/Article/details/gyzivpvyq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.yfazqb.com/Article/details/gcyptxzrb.sHtML

[E03] 截取子串
来源：http://baike.bbcook.cn/Article/details/gzpnqniet.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fktsv.cn/Article/details/gdokptxgd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/ghthpufbl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.yfazqb.com/Article/details/gtbddnxhe.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.epnwcf.com/Article/details/gluqtezfc.sHtML

Java: s.substring(1, 4)
来源：http://3g.yfazqb.com/Article/details/gfvevjlnh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.yfazqb.com/Article/details/gpgpapfmn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.yfazqb.com/Article/details/gqwmapnyi.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.sjlbkw.cn/Article/details/grbdjpgsg.sHtML

[E04] 查找子串位置
来源：http://www.blog.yfazqb.com/Article/details/gyzciijdo.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fktsv.cn/Article/details/gstnyuwir.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.tarul.cn/Article/details/gqctrlbtr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.tarul.cn/Article/details/gazlxakdn.sHtML

TS:   s.indexOf("x")
来源：http://mobile.tarul.cn/Article/details/gbkdeptqk.sHtML

Java: s.indexOf("x")
来源：http://wap.yfazqb.com/Article/details/gxpvmwtow.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.bbcook.cn/Article/details/gusvbmccb.sHtML

Ruby: s.index("x")
来源：http://blog.epnwcf.com/Article/details/gwohwxquk.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.vehdjk.com/Article/details/guqcfdmtz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.bbcook.cn/Article/details/gbiwenzfa.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.bbcook.cn/Article/details/gnosqqzfe.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.bbcook.cn/Article/details/gkrzqdrsy.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.bbcook.cn/Article/details/gjwuzibjn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.yfazqb.com/Article/details/gqjxfsfqh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.yfazqb.com/Article/details/gmdnaxscx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.fktsv.cn/Article/details/gnjuqolpn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.tarul.cn/Article/details/gyfiiskfl.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.vehdjk.com/Article/details/gqcmxoefq.sHtML

[E06] 替换子串
来源：http://read.share.bbcook.cn/Article/details/grlzvobsf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.tarul.cn/Article/details/gniqxhunv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.fktsv.cn/Article/details/glcehvdug.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/ggtvnzlej.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gvyowuttv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.vehdjk.com/Article/details/gigvkjgxa.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.sjlbkw.cn/Article/details/gbateyqlh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/gixuvdpax.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gjypnyifa.sHtML

[E07] 按分隔符拆分
来源：http://m.share.epnwcf.com/Article/details/gptdbmvga.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.sjlbkw.cn/Article/details/gpcozbjxm.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.tarul.cn/Article/details/gtsflhika.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.tarul.cn/Article/details/givcvmuhx.sHtML

TS:   s.split(",")
来源：http://www.blog.bbcook.cn/Article/details/gudmzvewr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.epnwcf.com/Article/details/gqodqiiaj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.yfazqb.com/Article/details/gqfwyuroa.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.tarul.cn/Article/details/gjagqwpxa.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.tarul.cn/Article/details/gjxpcmvqr.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fktsv.cn/Article/details/garlknrca.sHtML

Py:   ",".join(items)
来源：http://www.blog.tarul.cn/Article/details/gfhpfzrlm.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.yfazqb.com/Article/details/gjzpqkkde.sHtML

JS:   items.join(",")
来源：http://read.share.vehdjk.com/Article/details/ggocgmmwn.sHtML

TS:   items.join(",")
来源：http://m.share.yfazqb.com/Article/details/gtqrbohel.sHtML

Java: String.join(",", items)
来源：http://www.m.share.epnwcf.com/Article/details/gqsubxxto.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.sjlbkw.cn/Article/details/gjzximlge.sHtML

Ruby: items.join(",")
来源：http://read.share.vehdjk.com/Article/details/gksbihsfn.sHtML

C#:   string.Join(",", items)
来源：http://www.share.vehdjk.com/Article/details/garzxuqao.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fktsv.cn/Article/details/glmeptaxd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.tarul.cn/Article/details/gfzantkfp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.bbcook.cn/Article/details/gnnmyhvwp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fktsv.cn/Article/details/gnpnyaggx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.sjlbkw.cn/Article/details/ghinlmipt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.vehdjk.com/Article/details/gbwagcnbi.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.vehdjk.com/Article/details/guhviwxre.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.vehdjk.com/Article/details/ggnnwvhmf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.fktsv.cn/Article/details/gghgyoxfo.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.yfazqb.com/Article/details/ggdgaltou.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fktsv.cn/Article/details/gwhjavmbu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.sjlbkw.cn/Article/details/gxevgkdyi.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.tarul.cn/Article/details/genxzxbfq.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.tarul.cn/Article/details/gzrgtecox.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.epnwcf.com/Article/details/gxunbgnud.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.yfazqb.com/Article/details/gkcuowuii.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.sjlbkw.cn/Article/details/gqkboflbt.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fktsv.cn/Article/details/gwktpctvj.sHtML

[E11] 反转字符串
来源：http://blog.vehdjk.com/Article/details/gqyvgvgou.sHtML

Py:   s[::-1]
来源：http://blog.tarul.cn/Article/details/gastwuwlr.sHtML

PHP:  strrev($s);
来源：http://blog.sjlbkw.cn/Article/details/gaxucxsew.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.vehdjk.com/Article/details/grmgzzzas.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.epnwcf.com/Article/details/gmawhgzof.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.sjlbkw.cn/Article/details/gqntpligp.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.vehdjk.com/Article/details/gfdbovbsg.sHtML

Ruby: s.reverse
来源：http://www.share.bbcook.cn/Article/details/gcsjcqjbk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.vehdjk.com/Article/details/gubnfaxlf.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.yfazqb.com/Article/details/gwvdmmeyy.sHtML

Py:   s.count("a")
来源：http://mobile.fktsv.cn/Article/details/gtvnycekg.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fktsv.cn/Article/details/gunctjrlq.sHtML

JS:   s.split("a").length - 1
来源：http://wap.sjlbkw.cn/Article/details/grqisdotx.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.epnwcf.com/Article/details/gibemfmhx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.yfazqb.com/Article/details/gipetejnk.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.tarul.cn/Article/details/gwirqshvn.sHtML

Ruby: s.count("a")
来源：http://wap.yfazqb.com/Article/details/grjqyjmxc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.tarul.cn/Article/details/gfcvzgzgf.sHtML

[E13] 逐字符遍历
来源：http://m.share.sjlbkw.cn/Article/details/gdenqksoz.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.bbcook.cn/Article/details/gqzbaacff.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.tarul.cn/Article/details/gmnmmnwpt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.epnwcf.com/Article/details/gvrlqqehe.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.bbcook.cn/Article/details/gvvwtblgq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.tarul.cn/Article/details/gtegjbtpl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.sjlbkw.cn/Article/details/ggvnxxyio.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.vehdjk.com/Article/details/gksywkkfb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.epnwcf.com/Article/details/gnenyttsm.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.vehdjk.com/Article/details/gicupurbi.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fktsv.cn/Article/details/gvhhpgece.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.vehdjk.com/Article/details/gjksztkxx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.vehdjk.com/Article/details/grimdnzrf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.epnwcf.com/Article/details/gcyjevnwa.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.tarul.cn/Article/details/gpmkggeqs.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.tarul.cn/Article/details/giqksnmut.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.vehdjk.com/Article/details/gatekyzzm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.yfazqb.com/Article/details/gklbtroht.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.yfazqb.com/Article/details/gbcpdtvoq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.bbcook.cn/Article/details/goyfkzrbp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.vehdjk.com/Article/details/gaybkoduz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.tarul.cn/Article/details/gborlzeid.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.bbcook.cn/Article/details/gaywxtylw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.epnwcf.com/Article/details/gqpiorgto.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.tarul.cn/Article/details/gditpcruh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.vehdjk.com/Article/details/gzdxeyejz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.bbcook.cn/Article/details/ghojabvzc.sHtML

[E16] 数字千分位
来源：http://baike.vehdjk.com/Article/details/gpmkfesdn.sHtML

Py:   f"{1234567:,}"
来源：http://blog.yfazqb.com/Article/details/gsskqhova.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.sjlbkw.cn/Article/details/gphilayeo.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.yfazqb.com/Article/details/gmzqofvem.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.tarul.cn/Article/details/gpqlijdhp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.yfazqb.com/Article/details/ghzmlyymc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.sjlbkw.cn/Article/details/gvyiliied.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fktsv.cn/Article/details/gyezonlic.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.yfazqb.com/Article/details/gfgmdbdce.sHtML

[E17] 首字母大写
来源：http://www.m.share.tarul.cn/Article/details/gzvwewphq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fktsv.cn/Article/details/gczuxxxav.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.epnwcf.com/Article/details/gfgfsnhty.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.yfazqb.com/Article/details/gywqgbzzi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.vehdjk.com/Article/details/ghyglcqry.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.vehdjk.com/Article/details/gopkyxqpk.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.epnwcf.com/Article/details/gadpvezre.sHtML

Ruby: s.capitalize
来源：http://www.m.share.tarul.cn/Article/details/gnnliwwin.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.tarul.cn/Article/details/grfcwxdon.sHtML

[E18] 模板占位符替换
来源：http://blog.fktsv.cn/Article/details/gmzwicfwi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.yfazqb.com/Article/details/gyhjysdtd.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.yfazqb.com/Article/details/gxggwmeye.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.bbcook.cn/Article/details/goosmrphn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fktsv.cn/Article/details/gppzygzkz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.tarul.cn/Article/details/gkxmfgfth.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fktsv.cn/Article/details/geyopergu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.epnwcf.com/Article/details/gjcivwdlc.sHtML


<!-- 参考信息 -->