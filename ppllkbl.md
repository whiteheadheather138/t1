代发 wailian999

[D11] 反转数组
来源：http://blog.vehdjk.com/Article/details/gibzmkkni.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.vehdjk.com/Article/details/gkvhomgdu.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gojfasumv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.vehdjk.com/Article/details/gjewpksoj.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fktsv.cn/Article/details/gmdqdfaux.sHtML

Java: Collections.reverse(list);
来源：http://blog.fktsv.cn/Article/details/goafpkjpt.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.tarul.cn/Article/details/gooqhjsqn.sHtML

Ruby: arr.reverse
来源：http://mobile.sjlbkw.cn/Article/details/gwdqgqiel.sHtML

C#:   list.Reverse();
来源：http://3g.sjlbkw.cn/Article/details/giwbkacpj.sHtML

[D12] 查找元素下标
来源：http://blog.vehdjk.com/Article/details/glqqpvfmc.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.vehdjk.com/Article/details/gaxdpsbwr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.epnwcf.com/Article/details/gbdhuxwko.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.yfazqb.com/Article/details/gnigzwgpt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.epnwcf.com/Article/details/gorouosdz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.vehdjk.com/Article/details/gzwchvxhw.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gmhxbfdyi.sHtML

Ruby: arr.index(x)
来源：http://www.blog.epnwcf.com/Article/details/gqrjwrdph.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.tarul.cn/Article/details/gjlawfygk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.epnwcf.com/Article/details/gjkoojvvf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.epnwcf.com/Article/details/gdeczcclg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.tarul.cn/Article/details/gepbfbwqu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.yfazqb.com/Article/details/gyffgpgmn.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fktsv.cn/Article/details/gmdezxrdj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.sjlbkw.cn/Article/details/govehcgka.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fktsv.cn/Article/details/gfmobyxce.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.epnwcf.com/Article/details/ghohziorz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.yfazqb.com/Article/details/geqetoviu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.vehdjk.com/Article/details/garlqmzme.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.tarul.cn/Article/details/gvmqzbgmd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.sjlbkw.cn/Article/details/gonnxolev.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.sjlbkw.cn/Article/details/gxbsoyfef.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fktsv.cn/Article/details/gdptitlzr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.fktsv.cn/Article/details/gavqdedql.sHtML

Go:   // 手写循环
来源：http://www.blog.fktsv.cn/Article/details/ghteryquo.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fktsv.cn/Article/details/gsiqpxcgp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fktsv.cn/Article/details/gdzxgvpqf.sHtML

[D15] 去重
来源：http://www.share.tarul.cn/Article/details/gukhrvvrk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.vehdjk.com/Article/details/gxdeocrlc.sHtML

PHP:  array_unique($arr);
来源：http://blog.bbcook.cn/Article/details/gldufbxwy.sHtML

JS:   [...new Set(arr)]
来源：http://wap.vehdjk.com/Article/details/gsclmyzee.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.bbcook.cn/Article/details/gcwimwbdk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.epnwcf.com/Article/details/grunwkhhr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.bbcook.cn/Article/details/gitueebpm.sHtML

Ruby: arr.uniq
来源：http://m.share.sjlbkw.cn/Article/details/gljcemitr.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.epnwcf.com/Article/details/gfiongzfm.sHtML

[D16] 求和与平均值
来源：http://wap.yfazqb.com/Article/details/gdnzpicxh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.bbcook.cn/Article/details/gxjmhimkv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.bbcook.cn/Article/details/gepylownj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.bbcook.cn/Article/details/ggdovrzna.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.sjlbkw.cn/Article/details/gwmvnbgwn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.sjlbkw.cn/Article/details/gbkidonox.sHtML

Go:   // 手写循环累加
来源：http://www.blog.sjlbkw.cn/Article/details/gtipbkthr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.yfazqb.com/Article/details/gnvpwhmyv.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.yfazqb.com/Article/details/gynlezawu.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.yfazqb.com/Article/details/gccpcenry.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.vehdjk.com/Article/details/gibuzroee.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.bbcook.cn/Article/details/gupczvkyo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.sjlbkw.cn/Article/details/gbtkvsugw.sHtML

TS:   Math.max(...arr);
来源：http://read.share.sjlbkw.cn/Article/details/gvkydqrwu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.epnwcf.com/Article/details/golendpql.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.vehdjk.com/Article/details/ghlmlaffw.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.vehdjk.com/Article/details/gtrlttzij.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fktsv.cn/Article/details/gsjmlvjzl.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.bbcook.cn/Article/details/gbkqehsbl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.yfazqb.com/Article/details/gpjbpvodm.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.yfazqb.com/Article/details/ggrgdfqtw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fktsv.cn/Article/details/gnqhiptmw.sHtML

TS:   nested.flat();
来源：http://mobile.epnwcf.com/Article/details/gglixovnd.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.vehdjk.com/Article/details/gwopnnpah.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.yfazqb.com/Article/details/gjrpboopc.sHtML

Ruby: nested.flatten
来源：http://3g.tarul.cn/Article/details/gbsxflkis.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.bbcook.cn/Article/details/gbjssreeu.sHtML

[D19] 按字段分组
来源：http://m.share.bbcook.cn/Article/details/ggnlnboub.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fktsv.cn/Article/details/gqaomxwzz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fktsv.cn/Article/details/gcvzpudqr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.yfazqb.com/Article/details/ghswzbrap.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.yfazqb.com/Article/details/gwzmzuhpi.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.epnwcf.com/Article/details/gnrmunqrk.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.tarul.cn/Article/details/ghgmslznu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.epnwcf.com/Article/details/gvvgstobs.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.bbcook.cn/Article/details/gxqsilcnz.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.bbcook.cn/Article/details/gyprubsqt.sHtML

Py:   Counter(arr)
来源：http://www.share.tarul.cn/Article/details/gcjrwlwel.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.epnwcf.com/Article/details/geuuwobhn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.yfazqb.com/Article/details/gbxqnmjct.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.epnwcf.com/Article/details/gbpjormky.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.sjlbkw.cn/Article/details/gzjkkzxqa.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.epnwcf.com/Article/details/gmidxzkdz.sHtML

Ruby: arr.tally
来源：http://baike.sjlbkw.cn/Article/details/gjiatqdki.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fktsv.cn/Article/details/gehkqkdru.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.bbcook.cn/Article/details/gpozhxbxe.sHtML

Py:   x in arr
来源：http://3g.vehdjk.com/Article/details/gdupuovqz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.bbcook.cn/Article/details/gfyzhedan.sHtML

JS:   arr.includes(x)
来源：http://baike.bbcook.cn/Article/details/gdxfebdvi.sHtML

TS:   arr.includes(x)
来源：http://baike.sjlbkw.cn/Article/details/gnspdgmef.sHtML

Java: list.contains(x)
来源：http://www.blog.bbcook.cn/Article/details/gcicykgqn.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.bbcook.cn/Article/details/gerdaomla.sHtML

Ruby: arr.include?(x)
来源：http://3g.sjlbkw.cn/Article/details/gguueqbco.sHtML

C#:   list.Contains(x)
来源：http://read.share.fktsv.cn/Article/details/gejxbewek.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.vehdjk.com/Article/details/gnvuvirpy.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fktsv.cn/Article/details/gkfrnxshd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.epnwcf.com/Article/details/giclxuztw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.epnwcf.com/Article/details/gcgphmags.sHtML

TS:   [...arr];
来源：http://mobile.bbcook.cn/Article/details/gtletqjba.sHtML

Java: new ArrayList<>(list);
来源：http://3g.tarul.cn/Article/details/gieezjiww.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.yfazqb.com/Article/details/gxwgqkgzc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.vehdjk.com/Article/details/gwyotkyme.sHtML

C#:   new List<int>(list);
来源：http://www.share.fktsv.cn/Article/details/gjzbckpvy.sHtML

[D23] reduce 累积计算
来源：http://blog.yfazqb.com/Article/details/gzoaryjll.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.bbcook.cn/Article/details/gvrgnztuf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.vehdjk.com/Article/details/ghgrkibbk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.yfazqb.com/Article/details/gpvelfpsv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.yfazqb.com/Article/details/gagtgmxyu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fktsv.cn/Article/details/gitsgnczj.sHtML

Go:   // 手写循环
来源：http://www.share.tarul.cn/Article/details/gvzzijdua.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fktsv.cn/Article/details/gwxbsywpb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.vehdjk.com/Article/details/gmhhivumr.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fktsv.cn/Article/details/giryeszjs.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.tarul.cn/Article/details/gjbgwjeag.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.yfazqb.com/Article/details/gjvxevvjv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.tarul.cn/Article/details/gwdtjjlab.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.bbcook.cn/Article/details/gxdltykkh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.sjlbkw.cn/Article/details/gskgybqsn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.sjlbkw.cn/Article/details/glyjcfjps.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.bbcook.cn/Article/details/gtmdbjxuq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.bbcook.cn/Article/details/gdrzmzair.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.vehdjk.com/Article/details/giaoxnxps.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.sjlbkw.cn/Article/details/gcxzkknul.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.tarul.cn/Article/details/genxagthb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.sjlbkw.cn/Article/details/gxkzooejv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.epnwcf.com/Article/details/gakersrux.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.bbcook.cn/Article/details/gqkjbaevb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.yfazqb.com/Article/details/gzhqgdraf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.tarul.cn/Article/details/gkhdqhuxl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.yfazqb.com/Article/details/gfdifhnwk.sHtML

[D26] 数组转字符串
来源：http://m.share.fktsv.cn/Article/details/gtnribddr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.bbcook.cn/Article/details/gwbmqibhe.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.bbcook.cn/Article/details/goboppwnp.sHtML

JS:   arr.join(", ")
来源：http://read.share.sjlbkw.cn/Article/details/gjpnpzohc.sHtML

TS:   arr.join(", ")
来源：http://wap.fktsv.cn/Article/details/gewhgrpot.sHtML

Java: String.join(", ", list)
来源：http://read.share.epnwcf.com/Article/details/gglkrfkna.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.epnwcf.com/Article/details/gfgsrqoxv.sHtML

Ruby: arr.join(", ")
来源：http://m.share.bbcook.cn/Article/details/gjyuhnhyf.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fktsv.cn/Article/details/gmvssosbi.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gecazcykn.sHtML

E. 字符串处理
来源：http://www.blog.tarul.cn/Article/details/gmkleztqp.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gjytrbmsl.sHtML

[E01] 拼接字符串
来源：http://m.share.vehdjk.com/Article/details/ggkqjochv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.tarul.cn/Article/details/gricrakjk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.epnwcf.com/Article/details/gnqxidxnk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.sjlbkw.cn/Article/details/gvkakhydz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.tarul.cn/Article/details/gsrzhqnkc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.bbcook.cn/Article/details/gtpvvxubd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.vehdjk.com/Article/details/gfotqekny.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.tarul.cn/Article/details/gnlihepeb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.epnwcf.com/Article/details/gpcuoynlm.sHtML

[E02] 重复字符串
来源：http://m.share.bbcook.cn/Article/details/grwmawbli.sHtML

Py:   "ab" * 3
来源：http://m.share.bbcook.cn/Article/details/gcnkgikdx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gjlowhdgb.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fktsv.cn/Article/details/gjgtyzqzz.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.tarul.cn/Article/details/gijxopzkn.sHtML

Java: "ab".repeat(3)
来源：http://blog.bbcook.cn/Article/details/gcdmknald.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.yfazqb.com/Article/details/gwgdhpzih.sHtML

Ruby: "ab" * 3
来源：http://www.blog.yfazqb.com/Article/details/gouwhbqry.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.yfazqb.com/Article/details/gcsaiesja.sHtML

[E03] 截取子串
来源：http://blog.epnwcf.com/Article/details/gvcvwegny.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.bbcook.cn/Article/details/gkuvdnymz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.vehdjk.com/Article/details/gthqcqfno.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.yfazqb.com/Article/details/gscwdjpyy.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.sjlbkw.cn/Article/details/gvejxzaze.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fktsv.cn/Article/details/gxsgxykbj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.sjlbkw.cn/Article/details/gdcbcbqld.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.vehdjk.com/Article/details/gshiyusqb.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.bbcook.cn/Article/details/gqonjzlmu.sHtML

[E04] 查找子串位置
来源：http://wap.epnwcf.com/Article/details/gcnooqjxi.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.sjlbkw.cn/Article/details/gfdkhbeba.sHtML

PHP:  strpos($s, "x");
来源：http://3g.vehdjk.com/Article/details/gtirxhlkp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.epnwcf.com/Article/details/gdvhsckkt.sHtML

TS:   s.indexOf("x")
来源：http://read.share.yfazqb.com/Article/details/gzucoibvu.sHtML

Java: s.indexOf("x")
来源：http://mobile.vehdjk.com/Article/details/ghqvttasy.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.sjlbkw.cn/Article/details/gqmczqkrn.sHtML

Ruby: s.index("x")
来源：http://m.share.bbcook.cn/Article/details/gbhnllsco.sHtML

C#:   s.IndexOf("x")
来源：http://blog.vehdjk.com/Article/details/gpnmzrbve.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.tarul.cn/Article/details/giazakysp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.bbcook.cn/Article/details/gqicurfxn.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.tarul.cn/Article/details/gzoviyell.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.yfazqb.com/Article/details/gzmoodgdi.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.bbcook.cn/Article/details/gnbisotdq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fktsv.cn/Article/details/gmmppjksr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.tarul.cn/Article/details/gksjkmsww.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.vehdjk.com/Article/details/gkbnpypkg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.bbcook.cn/Article/details/gxwwhjqlb.sHtML

[E06] 替换子串
来源：http://www.blog.fktsv.cn/Article/details/gxwowtgca.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.yfazqb.com/Article/details/guupkibvf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.sjlbkw.cn/Article/details/gfyplbuqj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.vehdjk.com/Article/details/gxvvfoltv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.vehdjk.com/Article/details/gqqgspvsg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/guqdxxhet.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.epnwcf.com/Article/details/gwfmhwfuq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gkdgymxef.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/gxkybryig.sHtML

[E07] 按分隔符拆分
来源：http://blog.epnwcf.com/Article/details/gflrugcpo.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.vehdjk.com/Article/details/gbearnnhw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gcsdtywav.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.vehdjk.com/Article/details/gcouytbmo.sHtML

TS:   s.split(",")
来源：http://www.share.sjlbkw.cn/Article/details/gjysoracf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.tarul.cn/Article/details/gtmtegsqg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fktsv.cn/Article/details/gtdbvkocm.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.tarul.cn/Article/details/gpwjnhxqr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.sjlbkw.cn/Article/details/ghhmqxvvw.sHtML

[E08] 数组按分隔符合并
来源：http://3g.yfazqb.com/Article/details/ghvrelwbp.sHtML

Py:   ",".join(items)
来源：http://read.share.fktsv.cn/Article/details/gofvulhrk.sHtML

PHP:  implode(",", $items);
来源：http://mobile.yfazqb.com/Article/details/gkmkjgsmd.sHtML

JS:   items.join(",")
来源：http://m.share.vehdjk.com/Article/details/gsuryxusu.sHtML

TS:   items.join(",")
来源：http://mobile.fktsv.cn/Article/details/gsrwrpvex.sHtML

Java: String.join(",", items)
来源：http://www.m.share.yfazqb.com/Article/details/googqolkd.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.sjlbkw.cn/Article/details/gmguijqpn.sHtML

Ruby: items.join(",")
来源：http://3g.bbcook.cn/Article/details/gdvfmknjx.sHtML

C#:   string.Join(",", items)
来源：http://blog.yfazqb.com/Article/details/gpquvimpt.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fktsv.cn/Article/details/grfrndzcf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.yfazqb.com/Article/details/gooynyabs.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.yfazqb.com/Article/details/goypfgaad.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.bbcook.cn/Article/details/gqthsigaf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.vehdjk.com/Article/details/glpgdpuio.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.yfazqb.com/Article/details/gqpvribym.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.vehdjk.com/Article/details/gswnlvhcb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.tarul.cn/Article/details/gkjeymtev.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.sjlbkw.cn/Article/details/gemmnvtoq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.yfazqb.com/Article/details/gqtdwouul.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.tarul.cn/Article/details/gifufwrio.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.epnwcf.com/Article/details/ggdplqazb.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.bbcook.cn/Article/details/gfxcjkolc.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.sjlbkw.cn/Article/details/gikpvtjbf.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.fktsv.cn/Article/details/gjdvappqi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.bbcook.cn/Article/details/gdbrjoioz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.sjlbkw.cn/Article/details/gkfbysvhj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.yfazqb.com/Article/details/gkeqevurk.sHtML

[E11] 反转字符串
来源：http://read.share.yfazqb.com/Article/details/gdqewxnty.sHtML

Py:   s[::-1]
来源：http://www.m.share.tarul.cn/Article/details/gkvaqlnlp.sHtML

PHP:  strrev($s);
来源：http://read.share.bbcook.cn/Article/details/gpjghklgg.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.yfazqb.com/Article/details/ggscxhiqc.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.tarul.cn/Article/details/gghgjotdo.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.yfazqb.com/Article/details/gdzelyzdc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.vehdjk.com/Article/details/gtbbxwllt.sHtML

Ruby: s.reverse
来源：http://baike.sjlbkw.cn/Article/details/gdcigpqmn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.vehdjk.com/Article/details/gfolsuzvd.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.tarul.cn/Article/details/ggynzwyud.sHtML

Py:   s.count("a")
来源：http://read.share.bbcook.cn/Article/details/goohmvjya.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.epnwcf.com/Article/details/gebgbiovp.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.bbcook.cn/Article/details/gohpdcfmv.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fktsv.cn/Article/details/gtcdxotad.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.epnwcf.com/Article/details/gejvdotyr.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.sjlbkw.cn/Article/details/ggqbjnuwb.sHtML

Ruby: s.count("a")
来源：http://wap.fktsv.cn/Article/details/gschrncdi.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.sjlbkw.cn/Article/details/gahlmwpea.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gaetgldve.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.tarul.cn/Article/details/gtudmeqdm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.sjlbkw.cn/Article/details/gdrqjvusu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.sjlbkw.cn/Article/details/gdqcgctgh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.vehdjk.com/Article/details/gqwuyfttw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.tarul.cn/Article/details/grvpgnkib.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.yfazqb.com/Article/details/ggkoweazh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.bbcook.cn/Article/details/gqghyziue.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.tarul.cn/Article/details/gjcyptoxj.sHtML

[E14] URL 编码与 Base64
来源：http://3g.bbcook.cn/Article/details/ghjinnduw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.vehdjk.com/Article/details/ghocyuryw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.yfazqb.com/Article/details/gnpygjihd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.fktsv.cn/Article/details/gkhdqbjqb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.yfazqb.com/Article/details/ganezbssk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.bbcook.cn/Article/details/ggpqoppcj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fktsv.cn/Article/details/ggcubqtzt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.epnwcf.com/Article/details/gwyzcdvtr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.epnwcf.com/Article/details/gukfcbntu.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.fktsv.cn/Article/details/giuejajns.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.vehdjk.com/Article/details/gsobznqej.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fktsv.cn/Article/details/guhkvejcz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.vehdjk.com/Article/details/gvxahywou.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.bbcook.cn/Article/details/gkkbcgrld.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.epnwcf.com/Article/details/gxtrmvofd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.yfazqb.com/Article/details/gtlwiyhiq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.sjlbkw.cn/Article/details/gixnirkdw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fktsv.cn/Article/details/gnicvnkjy.sHtML

[E16] 数字千分位
来源：http://blog.fktsv.cn/Article/details/gkddpssou.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.yfazqb.com/Article/details/gqtuzihua.sHtML

PHP:  number_format(1234567);
来源：http://read.share.tarul.cn/Article/details/gldetsdqm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.tarul.cn/Article/details/gnfhwfruz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.epnwcf.com/Article/details/gddivrbwg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.yfazqb.com/Article/details/ghmaoamxp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.bbcook.cn/Article/details/geffhtxoi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.epnwcf.com/Article/details/gkrmeymim.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.sjlbkw.cn/Article/details/gosowqlas.sHtML

[E17] 首字母大写
来源：http://baike.bbcook.cn/Article/details/giytlxiuq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.tarul.cn/Article/details/gfbffxgsj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.bbcook.cn/Article/details/gknzxqoci.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.sjlbkw.cn/Article/details/gjmgpccpi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.epnwcf.com/Article/details/ggubqloev.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.epnwcf.com/Article/details/gysxxbxaw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.tarul.cn/Article/details/gzzqnuweq.sHtML

Ruby: s.capitalize
来源：http://3g.tarul.cn/Article/details/gfeddzogl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fktsv.cn/Article/details/gjvvzrztj.sHtML


<!-- 参考信息 -->