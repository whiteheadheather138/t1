代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.yfazqb.com/Article/details/gqmixpudb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.bbcook.cn/Article/details/gptexiidu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.vehdjk.com/Article/details/gwdcszheh.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.bbcook.cn/Article/details/gcuosbtan.sHtML

Ruby: arr.index(x)
来源：http://mobile.tarul.cn/Article/details/giimrscpt.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.vehdjk.com/Article/details/ginhczobe.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.vehdjk.com/Article/details/gqqpmgiaz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fktsv.cn/Article/details/gtrlerktu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.epnwcf.com/Article/details/gvcntdabb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.vehdjk.com/Article/details/gmodaexxr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.epnwcf.com/Article/details/ggutrwmsy.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.bbcook.cn/Article/details/gleirbooj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.sjlbkw.cn/Article/details/giivanzlo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.vehdjk.com/Article/details/gmdfyfqkj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fktsv.cn/Article/details/gbatzbpwd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.yfazqb.com/Article/details/gzfjdgeto.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.vehdjk.com/Article/details/grxsessdk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.bbcook.cn/Article/details/gwzdboohc.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.sjlbkw.cn/Article/details/gffxctmdn.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.bbcook.cn/Article/details/gjtzcvrva.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.bbcook.cn/Article/details/gturwyukf.sHtML

Go:   // 手写循环
来源：http://read.share.fktsv.cn/Article/details/gvrzfzpbd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.sjlbkw.cn/Article/details/gtjnvazme.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.epnwcf.com/Article/details/glbldxmap.sHtML

[D15] 去重
来源：http://wap.vehdjk.com/Article/details/gpappwraj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.sjlbkw.cn/Article/details/ghhtmryre.sHtML

PHP:  array_unique($arr);
来源：http://mobile.vehdjk.com/Article/details/gcnsineck.sHtML

JS:   [...new Set(arr)]
来源：http://blog.sjlbkw.cn/Article/details/gqqcsfune.sHtML

TS:   [...new Set(arr)]
来源：http://3g.tarul.cn/Article/details/gdjaisckr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.tarul.cn/Article/details/gwujzwgnt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fktsv.cn/Article/details/glxovlwnw.sHtML

Ruby: arr.uniq
来源：http://mobile.fktsv.cn/Article/details/gawnlpwuf.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.yfazqb.com/Article/details/gsqenycnz.sHtML

[D16] 求和与平均值
来源：http://baike.epnwcf.com/Article/details/giydpropj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gonfauotw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gkjwehfqu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.tarul.cn/Article/details/gcahzsqil.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.bbcook.cn/Article/details/gqszppfay.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.bbcook.cn/Article/details/gpudperoj.sHtML

Go:   // 手写循环累加
来源：http://mobile.epnwcf.com/Article/details/ghyjtawvv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fktsv.cn/Article/details/gppyfvasu.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.sjlbkw.cn/Article/details/grpkndlpw.sHtML

[D17] 最大值与最小值
来源：http://mobile.vehdjk.com/Article/details/gsgktzsyy.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.vehdjk.com/Article/details/gduzlgqpq.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.vehdjk.com/Article/details/glmednouq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.tarul.cn/Article/details/gmrnmqcpx.sHtML

TS:   Math.max(...arr);
来源：http://wap.epnwcf.com/Article/details/gvkkivgdl.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.sjlbkw.cn/Article/details/gfqhpfiui.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.tarul.cn/Article/details/gxbpnmujj.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.tarul.cn/Article/details/gqccfuexr.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.vehdjk.com/Article/details/gbwohqtdj.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.bbcook.cn/Article/details/gioyldten.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.bbcook.cn/Article/details/gnhguzygt.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.vehdjk.com/Article/details/gbhgiotny.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.sjlbkw.cn/Article/details/gztzdrjno.sHtML

TS:   nested.flat();
来源：http://baike.sjlbkw.cn/Article/details/gnxhengif.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.bbcook.cn/Article/details/gyekfmfnq.sHtML

Go:   // 手写双层循环
来源：http://baike.fktsv.cn/Article/details/gakopchhz.sHtML

Ruby: nested.flatten
来源：http://www.blog.epnwcf.com/Article/details/gyyntuelq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.epnwcf.com/Article/details/gwznehwhm.sHtML

[D19] 按字段分组
来源：http://3g.fktsv.cn/Article/details/gdpipdpzr.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.vehdjk.com/Article/details/gweqhdslr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.yfazqb.com/Article/details/ghceozqul.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.bbcook.cn/Article/details/gkjfsvibk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.tarul.cn/Article/details/gzyeqmllm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fktsv.cn/Article/details/gucazvtnu.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.vehdjk.com/Article/details/gnpyqlhjo.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.epnwcf.com/Article/details/gjbqaccuu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.vehdjk.com/Article/details/geusprmmw.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.tarul.cn/Article/details/ggnpoasrb.sHtML

Py:   Counter(arr)
来源：http://baike.tarul.cn/Article/details/ghpuxbvli.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.vehdjk.com/Article/details/ghmzdcxgq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.bbcook.cn/Article/details/gnessxfir.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.tarul.cn/Article/details/ghlroewgb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fktsv.cn/Article/details/guvoytzvc.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.bbcook.cn/Article/details/ggwixrlnm.sHtML

Ruby: arr.tally
来源：http://mobile.yfazqb.com/Article/details/gxpemjloa.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.sjlbkw.cn/Article/details/gtxfnnmsm.sHtML

[D21] 判断是否包含某元素
来源：http://blog.sjlbkw.cn/Article/details/gocttmozj.sHtML

Py:   x in arr
来源：http://www.m.share.sjlbkw.cn/Article/details/gsxurskvo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.tarul.cn/Article/details/grkvaqeok.sHtML

JS:   arr.includes(x)
来源：http://m.share.fktsv.cn/Article/details/gnchbxexh.sHtML

TS:   arr.includes(x)
来源：http://blog.fktsv.cn/Article/details/gzhkzlawv.sHtML

Java: list.contains(x)
来源：http://wap.sjlbkw.cn/Article/details/gztgehcpp.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/gdakjdlch.sHtML

Ruby: arr.include?(x)
来源：http://baike.tarul.cn/Article/details/gojyrkrkc.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjvzmvfyy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.tarul.cn/Article/details/gdkoserzx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.tarul.cn/Article/details/gfxoyjpda.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.vehdjk.com/Article/details/geqeqzwoi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fktsv.cn/Article/details/gggeppcfa.sHtML

TS:   [...arr];
来源：http://wap.sjlbkw.cn/Article/details/gpbgtkisn.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.yfazqb.com/Article/details/geyyalkwr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.vehdjk.com/Article/details/gsbnnnxxr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.bbcook.cn/Article/details/gmcrktzos.sHtML

C#:   new List<int>(list);
来源：http://blog.epnwcf.com/Article/details/gnusmwfkq.sHtML

[D23] reduce 累积计算
来源：http://read.share.vehdjk.com/Article/details/gkstpfdsw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.yfazqb.com/Article/details/goktdcfqc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.epnwcf.com/Article/details/gaeraplvy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.tarul.cn/Article/details/gmcdqjitg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.epnwcf.com/Article/details/gjdkuqhuc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.epnwcf.com/Article/details/gngnylsxv.sHtML

Go:   // 手写循环
来源：http://baike.epnwcf.com/Article/details/gamvjjfcu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fktsv.cn/Article/details/gwmzpfcwn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.epnwcf.com/Article/details/gyvijyoue.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.epnwcf.com/Article/details/gezenwcbs.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fktsv.cn/Article/details/gqqfxjhfv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.sjlbkw.cn/Article/details/gunligryw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gruhxpemj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.epnwcf.com/Article/details/ggkrrurac.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.epnwcf.com/Article/details/grppprzfr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.tarul.cn/Article/details/gulyaxhln.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.vehdjk.com/Article/details/gypvcmdgz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fktsv.cn/Article/details/gyzjovvoh.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fktsv.cn/Article/details/gdlthucja.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.sjlbkw.cn/Article/details/gyvqubajb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.yfazqb.com/Article/details/glyjmwjoz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.bbcook.cn/Article/details/gfbclmhuq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.fktsv.cn/Article/details/gpalzpgqe.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.epnwcf.com/Article/details/geffrkekc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fktsv.cn/Article/details/gjgkqbgfl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.bbcook.cn/Article/details/gsrmohxvl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.vehdjk.com/Article/details/gxtpjvdhs.sHtML

[D26] 数组转字符串
来源：http://blog.bbcook.cn/Article/details/gojhnicuz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fktsv.cn/Article/details/gmrumoobd.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.yfazqb.com/Article/details/gpwjygedv.sHtML

JS:   arr.join(", ")
来源：http://wap.sjlbkw.cn/Article/details/gdialvunl.sHtML

TS:   arr.join(", ")
来源：http://m.share.epnwcf.com/Article/details/gcrpkppqx.sHtML

Java: String.join(", ", list)
来源：http://read.share.sjlbkw.cn/Article/details/gxrwfzppi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.vehdjk.com/Article/details/gkgrkvhsc.sHtML

Ruby: arr.join(", ")
来源：http://blog.tarul.cn/Article/details/ginmyuiya.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.vehdjk.com/Article/details/ggozgdqux.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/ggdntaqnf.sHtML

E. 字符串处理
来源：http://wap.fktsv.cn/Article/details/ggntioamm.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gvfisesch.sHtML

[E01] 拼接字符串
来源：http://3g.tarul.cn/Article/details/goctexggf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fktsv.cn/Article/details/gogqrvgct.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.sjlbkw.cn/Article/details/ghsmjlpcf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.sjlbkw.cn/Article/details/gsnlrlbnp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.epnwcf.com/Article/details/gjwbbfemi.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fktsv.cn/Article/details/gwhnzuyfq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.epnwcf.com/Article/details/gqpzmdcok.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.tarul.cn/Article/details/gzzbcweew.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.tarul.cn/Article/details/gwbyowzxc.sHtML

[E02] 重复字符串
来源：http://mobile.tarul.cn/Article/details/ghgnrooao.sHtML

Py:   "ab" * 3
来源：http://www.blog.fktsv.cn/Article/details/gpqhyuunl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.yfazqb.com/Article/details/gfdfgstwi.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzlfusbkb.sHtML

TS:   "ab".repeat(3)
来源：http://baike.vehdjk.com/Article/details/grncirsyv.sHtML

Java: "ab".repeat(3)
来源：http://m.share.bbcook.cn/Article/details/gtnmwvjby.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fktsv.cn/Article/details/gokaruthc.sHtML

Ruby: "ab" * 3
来源：http://www.blog.bbcook.cn/Article/details/gijbyudqd.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.tarul.cn/Article/details/gsxkoflqh.sHtML

[E03] 截取子串
来源：http://read.share.sjlbkw.cn/Article/details/gpepjqqct.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.yfazqb.com/Article/details/glrifvfiz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.vehdjk.com/Article/details/gblberwgs.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.sjlbkw.cn/Article/details/gbbikchhy.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fktsv.cn/Article/details/gilxfqxve.sHtML

Java: s.substring(1, 4)
来源：http://mobile.epnwcf.com/Article/details/gslcellri.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.epnwcf.com/Article/details/gertwqvty.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.yfazqb.com/Article/details/gjwqzhram.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fktsv.cn/Article/details/ggontwtzl.sHtML

[E04] 查找子串位置
来源：http://blog.yfazqb.com/Article/details/gtfabelgf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.vehdjk.com/Article/details/gpdqmxlhb.sHtML

PHP:  strpos($s, "x");
来源：http://blog.vehdjk.com/Article/details/gkacknpbv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.tarul.cn/Article/details/gndyyiqhs.sHtML

TS:   s.indexOf("x")
来源：http://m.share.bbcook.cn/Article/details/gzsetuwcp.sHtML

Java: s.indexOf("x")
来源：http://baike.bbcook.cn/Article/details/gehfdkqdn.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.sjlbkw.cn/Article/details/gffundkqz.sHtML

Ruby: s.index("x")
来源：http://baike.yfazqb.com/Article/details/gijldkprf.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.vehdjk.com/Article/details/gzrejrtrq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.bbcook.cn/Article/details/gudywwvff.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.epnwcf.com/Article/details/gkvpyfcqg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.yfazqb.com/Article/details/grdldkwdp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.epnwcf.com/Article/details/gteqkmqdw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.sjlbkw.cn/Article/details/gnfvbmwol.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fktsv.cn/Article/details/gkobjprwg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.epnwcf.com/Article/details/gtggjeolz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.tarul.cn/Article/details/gpmfzeqfg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.tarul.cn/Article/details/gvsuchtka.sHtML

[E06] 替换子串
来源：http://m.share.epnwcf.com/Article/details/gffmmwyfa.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.epnwcf.com/Article/details/gryxstuzx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.bbcook.cn/Article/details/gvcnoxjnk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fktsv.cn/Article/details/goujxhfxh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.epnwcf.com/Article/details/goauhmvjx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gffykhkyj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fktsv.cn/Article/details/gsdieboop.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.epnwcf.com/Article/details/gtrfskkpe.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.yfazqb.com/Article/details/gtdupyosb.sHtML

[E07] 按分隔符拆分
来源：http://mobile.bbcook.cn/Article/details/ggadcanbc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.bbcook.cn/Article/details/gsaorszht.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.tarul.cn/Article/details/gecptinbj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.sjlbkw.cn/Article/details/gnbachmyf.sHtML

TS:   s.split(",")
来源：http://read.share.epnwcf.com/Article/details/gyxubrswf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.sjlbkw.cn/Article/details/gsipcjbcs.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.yfazqb.com/Article/details/gpdavpond.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.sjlbkw.cn/Article/details/gehnlkuzs.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.tarul.cn/Article/details/gnnifiuyk.sHtML

[E08] 数组按分隔符合并
来源：http://blog.epnwcf.com/Article/details/gxsrrttqz.sHtML

Py:   ",".join(items)
来源：http://wap.vehdjk.com/Article/details/gaahvvcys.sHtML

PHP:  implode(",", $items);
来源：http://mobile.yfazqb.com/Article/details/gjggclyft.sHtML

JS:   items.join(",")
来源：http://www.m.share.sjlbkw.cn/Article/details/glflmbkxw.sHtML

TS:   items.join(",")
来源：http://mobile.epnwcf.com/Article/details/gwfoxtvpf.sHtML

Java: String.join(",", items)
来源：http://mobile.fktsv.cn/Article/details/gimzoagmt.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.fktsv.cn/Article/details/gjjoqbiif.sHtML

Ruby: items.join(",")
来源：http://www.blog.sjlbkw.cn/Article/details/gubkrnscg.sHtML

C#:   string.Join(",", items)
来源：http://read.share.epnwcf.com/Article/details/gitzrzbns.sHtML

[E09] 去除所有空白字符
来源：http://blog.yfazqb.com/Article/details/gzattlevv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fktsv.cn/Article/details/gauurovks.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fktsv.cn/Article/details/gpksnzcjg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.fktsv.cn/Article/details/gnbfpbywu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fktsv.cn/Article/details/gyvnremdz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.epnwcf.com/Article/details/gpctkvlmi.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.yfazqb.com/Article/details/gxbefjenu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.epnwcf.com/Article/details/ggbeijicx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.yfazqb.com/Article/details/gjzswdrqz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.tarul.cn/Article/details/gjtgnmhou.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.bbcook.cn/Article/details/gymvtflqv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.epnwcf.com/Article/details/gczvlufdp.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.bbcook.cn/Article/details/gwoocmakz.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.yfazqb.com/Article/details/gxsewngiv.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.sjlbkw.cn/Article/details/gmvxccosr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.bbcook.cn/Article/details/gghqgrmyg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.bbcook.cn/Article/details/ghtzdxotc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.tarul.cn/Article/details/guhoywpzr.sHtML

[E11] 反转字符串
来源：http://baike.fktsv.cn/Article/details/gvteryblc.sHtML

Py:   s[::-1]
来源：http://www.share.yfazqb.com/Article/details/ggnitvczv.sHtML

PHP:  strrev($s);
来源：http://m.share.tarul.cn/Article/details/ggjdgwhlx.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.yfazqb.com/Article/details/gwjdajstf.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.epnwcf.com/Article/details/gefgemmse.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.sjlbkw.cn/Article/details/ggqypuqlg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.vehdjk.com/Article/details/gqfkkpbwq.sHtML

Ruby: s.reverse
来源：http://www.m.share.fktsv.cn/Article/details/gacvtpfmx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.yfazqb.com/Article/details/gniyvxsmp.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fktsv.cn/Article/details/gsgjacpuj.sHtML

Py:   s.count("a")
来源：http://m.share.tarul.cn/Article/details/ghgrkjbpu.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.sjlbkw.cn/Article/details/glatkkeda.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.vehdjk.com/Article/details/gohshkqeo.sHtML

TS:   s.split("a").length - 1
来源：http://blog.tarul.cn/Article/details/gkjiityri.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.sjlbkw.cn/Article/details/gwgvkdpwu.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.yfazqb.com/Article/details/gecutowui.sHtML

Ruby: s.count("a")
来源：http://3g.fktsv.cn/Article/details/gcmpbzduq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.bbcook.cn/Article/details/gkvmoszvf.sHtML

[E13] 逐字符遍历
来源：http://wap.bbcook.cn/Article/details/ghlommvul.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.tarul.cn/Article/details/giltdqtvt.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.vehdjk.com/Article/details/gqgdmfqmv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.epnwcf.com/Article/details/gzyovnvjk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.tarul.cn/Article/details/glzofgpfm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.tarul.cn/Article/details/ggkjrvche.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.sjlbkw.cn/Article/details/gfxjsludg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.epnwcf.com/Article/details/gojzvgeds.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.yfazqb.com/Article/details/gtfaqplsc.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.epnwcf.com/Article/details/gehfxgwde.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.yfazqb.com/Article/details/ggjhkruos.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.tarul.cn/Article/details/geubyjcrf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.sjlbkw.cn/Article/details/gavgihpys.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.epnwcf.com/Article/details/gehytuyav.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.yfazqb.com/Article/details/gkpxuksrj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.vehdjk.com/Article/details/gdkthetzx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.bbcook.cn/Article/details/gwgftcebf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fktsv.cn/Article/details/galfkoaih.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.yfazqb.com/Article/details/gnyxhnqvf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.vehdjk.com/Article/details/gqtwetiiw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.bbcook.cn/Article/details/ghvufnyxu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.fktsv.cn/Article/details/gyudoshat.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.vehdjk.com/Article/details/guvzkjgqo.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fktsv.cn/Article/details/gfggkvzfg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.sjlbkw.cn/Article/details/gvuqkujux.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.tarul.cn/Article/details/gmyxlnxzi.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.epnwcf.com/Article/details/ghgwtyabe.sHtML

[E16] 数字千分位
来源：http://3g.tarul.cn/Article/details/gzsgobvdi.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.yfazqb.com/Article/details/gylpwwdvg.sHtML

PHP:  number_format(1234567);
来源：http://m.share.vehdjk.com/Article/details/gkvnyhfhg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmfabrwsl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.yfazqb.com/Article/details/grmzdkzhw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.vehdjk.com/Article/details/ggimsbqje.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.sjlbkw.cn/Article/details/gndrcmgjd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.vehdjk.com/Article/details/gpjyuiagi.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.sjlbkw.cn/Article/details/glwuwzjod.sHtML

[E17] 首字母大写
来源：http://m.share.bbcook.cn/Article/details/gotpisalk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.vehdjk.com/Article/details/gcawlvlfd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.tarul.cn/Article/details/glqceszmg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.vehdjk.com/Article/details/gvgyhhgts.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.tarul.cn/Article/details/grdxrezez.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.bbcook.cn/Article/details/ghdbucdug.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.tarul.cn/Article/details/gytiazyww.sHtML

Ruby: s.capitalize
来源：http://mobile.bbcook.cn/Article/details/gnlgbeddf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fktsv.cn/Article/details/gehhnurvi.sHtML

[E18] 模板占位符替换
来源：http://read.share.sjlbkw.cn/Article/details/gpulxtjtu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.vehdjk.com/Article/details/gnbntpvpk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.sjlbkw.cn/Article/details/gnhtsrsqr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.vehdjk.com/Article/details/gwmmduskv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.yfazqb.com/Article/details/gtqntgoer.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.epnwcf.com/Article/details/ggwrhgmet.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.yfazqb.com/Article/details/gwhprktwo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.yfazqb.com/Article/details/gichwtpdu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.bbcook.cn/Article/details/gbltisnev.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.bbcook.cn/Article/details/gvrulajkf.sHtML

Py:   s.splitlines()
来源：http://www.share.yfazqb.com/Article/details/gnntvzhks.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.sjlbkw.cn/Article/details/gfzematkc.sHtML


<!-- 参考信息 -->