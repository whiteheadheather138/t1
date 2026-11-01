代发 wailian999

[D07] 切片 / 取子数组
来源：http://www.m.share.vehdjk.com/Article/details/gjgclxghg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.sjlbkw.cn/Article/details/gxdquatwt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.tarul.cn/Article/details/gkcfyoywn.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.bbcook.cn/Article/details/ggafnzcle.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.tarul.cn/Article/details/glsajjysm.sHtML

Java: list.subList(1, 4);
来源：http://m.share.bbcook.cn/Article/details/getmhakkd.sHtML

Go:   arr[1:4]
来源：http://baike.bbcook.cn/Article/details/grrumrodc.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fktsv.cn/Article/details/gsjgihjdl.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.fktsv.cn/Article/details/ggfqgzlkd.sHtML

[D08] 合并两个数组
来源：http://www.m.share.tarul.cn/Article/details/gxjtaxuly.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.vehdjk.com/Article/details/gkkibjvxz.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.bbcook.cn/Article/details/gravhjuaq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.epnwcf.com/Article/details/gdogznqfc.sHtML

TS:   [...a, ...b];
来源：http://3g.sjlbkw.cn/Article/details/gbsvjjunt.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.vehdjk.com/Article/details/gtymmxkif.sHtML

Go:   append(a, b...)
来源：http://mobile.yfazqb.com/Article/details/gcxugabgh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.vehdjk.com/Article/details/grcntdotg.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.yfazqb.com/Article/details/gqiwoecpw.sHtML

[D09] 排序（升序）
来源：http://baike.bbcook.cn/Article/details/ggadomzvh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.epnwcf.com/Article/details/gsdepucwp.sHtML

PHP:  sort($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gyuoxbkcu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.epnwcf.com/Article/details/greyzpjab.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.vehdjk.com/Article/details/goblejeps.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.sjlbkw.cn/Article/details/gyegkxcxd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gloncvepj.sHtML

Ruby: arr.sort
来源：http://mobile.tarul.cn/Article/details/gahjkktmp.sHtML

C#:   list.Sort();
来源：http://wap.epnwcf.com/Article/details/giqaxeino.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.vehdjk.com/Article/details/ggaqjlrsi.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.tarul.cn/Article/details/gjrwwhbhq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.epnwcf.com/Article/details/gwtbtosuc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.epnwcf.com/Article/details/gruqkvbga.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.vehdjk.com/Article/details/gtcpauine.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.tarul.cn/Article/details/gwwmhnmvh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.sjlbkw.cn/Article/details/gerhkysuo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.sjlbkw.cn/Article/details/gluxquqqh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fktsv.cn/Article/details/gjobgsgmh.sHtML

[D11] 反转数组
来源：http://blog.epnwcf.com/Article/details/gbzpayxhv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.vehdjk.com/Article/details/gwcgthslt.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.tarul.cn/Article/details/ggggjqdxn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.tarul.cn/Article/details/gztgctvrp.sHtML

TS:   [...arr].reverse();
来源：http://baike.sjlbkw.cn/Article/details/ghxidqnlf.sHtML

Java: Collections.reverse(list);
来源：http://read.share.epnwcf.com/Article/details/grqprxvog.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gsswyhvxm.sHtML

Ruby: arr.reverse
来源：http://baike.vehdjk.com/Article/details/gcmytdjcg.sHtML

C#:   list.Reverse();
来源：http://3g.bbcook.cn/Article/details/gytwczube.sHtML

[D12] 查找元素下标
来源：http://baike.bbcook.cn/Article/details/glycgjmsa.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.sjlbkw.cn/Article/details/gmcbssypk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fktsv.cn/Article/details/gegdeulyy.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.yfazqb.com/Article/details/gjkirxobw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fktsv.cn/Article/details/gtvtkthnt.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.yfazqb.com/Article/details/grkwphwso.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.bbcook.cn/Article/details/ghemsrtha.sHtML

Ruby: arr.index(x)
来源：http://www.blog.vehdjk.com/Article/details/guamcpzds.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fktsv.cn/Article/details/grddgroor.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.epnwcf.com/Article/details/grkmtchuz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.yfazqb.com/Article/details/gydleheim.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.tarul.cn/Article/details/gnrowrlfl.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.epnwcf.com/Article/details/gwtkhfhpx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.vehdjk.com/Article/details/ggypoapfw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.sjlbkw.cn/Article/details/gxpckdwsg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.bbcook.cn/Article/details/gvgevmfuo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.vehdjk.com/Article/details/ghjipbihd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fktsv.cn/Article/details/gimnvdxku.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fktsv.cn/Article/details/gumjlrrfx.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fktsv.cn/Article/details/ggcjemdlm.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.yfazqb.com/Article/details/gtgllfegl.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.sjlbkw.cn/Article/details/gdygfnacz.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.yfazqb.com/Article/details/ggsixldik.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.tarul.cn/Article/details/gokxhwscx.sHtML

Go:   // 手写循环
来源：http://www.blog.bbcook.cn/Article/details/ghvfizxaq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.tarul.cn/Article/details/guxaveipl.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.tarul.cn/Article/details/gophicpls.sHtML

[D15] 去重
来源：http://mobile.fktsv.cn/Article/details/gxzytsprq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.tarul.cn/Article/details/gwhudyhbm.sHtML

PHP:  array_unique($arr);
来源：http://blog.sjlbkw.cn/Article/details/gmjtrnofz.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fktsv.cn/Article/details/grvrbwbez.sHtML

TS:   [...new Set(arr)]
来源：http://wap.epnwcf.com/Article/details/gdeodbvha.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.yfazqb.com/Article/details/ghhhqjeem.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.epnwcf.com/Article/details/goothtqug.sHtML

Ruby: arr.uniq
来源：http://wap.sjlbkw.cn/Article/details/ghsswtvdt.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.vehdjk.com/Article/details/gyevmmcie.sHtML

[D16] 求和与平均值
来源：http://wap.yfazqb.com/Article/details/gzetumozm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.epnwcf.com/Article/details/gtjihmevj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gqwxonwds.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gltpumhdc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.epnwcf.com/Article/details/gwsbwmycr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.sjlbkw.cn/Article/details/gqcwwomwx.sHtML

Go:   // 手写循环累加
来源：http://3g.epnwcf.com/Article/details/gwssezgxd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.yfazqb.com/Article/details/gncliemey.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.yfazqb.com/Article/details/gproicumb.sHtML

[D17] 最大值与最小值
来源：http://baike.bbcook.cn/Article/details/gfmxdxgli.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.epnwcf.com/Article/details/gvqbqmtpn.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.tarul.cn/Article/details/gsqedatbc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.sjlbkw.cn/Article/details/gqxejlamz.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fktsv.cn/Article/details/gfokwtylq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.sjlbkw.cn/Article/details/gxbjwokuz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyupxwtyt.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.vehdjk.com/Article/details/gtrdazqiv.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.tarul.cn/Article/details/ghzaqrjly.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.vehdjk.com/Article/details/gqvffbnae.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.yfazqb.com/Article/details/gznprtuov.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.epnwcf.com/Article/details/gjxgxfbxs.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.epnwcf.com/Article/details/grxaaqzcc.sHtML

TS:   nested.flat();
来源：http://www.blog.tarul.cn/Article/details/gbjrmpexv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.sjlbkw.cn/Article/details/gqxndjhye.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.epnwcf.com/Article/details/ggwraueeu.sHtML

Ruby: nested.flatten
来源：http://mobile.sjlbkw.cn/Article/details/gosiknlbr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.bbcook.cn/Article/details/gutxhjavb.sHtML

[D19] 按字段分组
来源：http://3g.fktsv.cn/Article/details/gbvihmmrj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.sjlbkw.cn/Article/details/grljatueu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fktsv.cn/Article/details/guccskija.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.yfazqb.com/Article/details/gqfhalcog.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.yfazqb.com/Article/details/gemyowwrd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fktsv.cn/Article/details/gzgivjyic.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.vehdjk.com/Article/details/gpnfkbvbm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.vehdjk.com/Article/details/gxtsaglsz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.epnwcf.com/Article/details/gqyxtynxw.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.epnwcf.com/Article/details/grqdvwnox.sHtML

Py:   Counter(arr)
来源：http://blog.bbcook.cn/Article/details/gtouvhvfs.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.vehdjk.com/Article/details/gwpnhbwii.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.bbcook.cn/Article/details/gegulcejo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.yfazqb.com/Article/details/gecpsmqxh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.yfazqb.com/Article/details/gelypaqtu.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.vehdjk.com/Article/details/gkazcaxhj.sHtML

Ruby: arr.tally
来源：http://www.share.epnwcf.com/Article/details/gfytseuah.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.yfazqb.com/Article/details/gvhnzgxpp.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fktsv.cn/Article/details/gtleqaazy.sHtML

Py:   x in arr
来源：http://blog.tarul.cn/Article/details/gdweahxro.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.bbcook.cn/Article/details/gjhetfdox.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.vehdjk.com/Article/details/gxiaipifc.sHtML

TS:   arr.includes(x)
来源：http://3g.vehdjk.com/Article/details/gyztinbqc.sHtML

Java: list.contains(x)
来源：http://www.m.share.epnwcf.com/Article/details/gyxfbsdys.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gnveoudur.sHtML

Ruby: arr.include?(x)
来源：http://read.share.yfazqb.com/Article/details/ggqkgwljv.sHtML

C#:   list.Contains(x)
来源：http://read.share.tarul.cn/Article/details/gfojbftfz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.yfazqb.com/Article/details/gkzerotcm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.yfazqb.com/Article/details/gfnuvoapm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.tarul.cn/Article/details/ggxmpzlgo.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.epnwcf.com/Article/details/gtzwiyhnd.sHtML

TS:   [...arr];
来源：http://3g.sjlbkw.cn/Article/details/gflkzfpwe.sHtML

Java: new ArrayList<>(list);
来源：http://wap.tarul.cn/Article/details/gckvwumgb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.yfazqb.com/Article/details/ggzrnxcsy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.epnwcf.com/Article/details/gqmrpopng.sHtML

C#:   new List<int>(list);
来源：http://wap.sjlbkw.cn/Article/details/gbpyuvblj.sHtML

[D23] reduce 累积计算
来源：http://mobile.tarul.cn/Article/details/ggjfmmxfq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.bbcook.cn/Article/details/grmxcmveq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.epnwcf.com/Article/details/gesjmzdek.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.tarul.cn/Article/details/ggohdngxt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.tarul.cn/Article/details/gshlaueqp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.sjlbkw.cn/Article/details/gsvcyrthk.sHtML

Go:   // 手写循环
来源：http://blog.bbcook.cn/Article/details/gbysndsli.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.vehdjk.com/Article/details/gszsekhhp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.sjlbkw.cn/Article/details/gbxzujlwa.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.epnwcf.com/Article/details/gxvtveuwv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fktsv.cn/Article/details/gnkdlquhu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.epnwcf.com/Article/details/gifjzxiil.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.bbcook.cn/Article/details/gfpumljau.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.yfazqb.com/Article/details/gjzswbrpd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.bbcook.cn/Article/details/gaefbmteb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.tarul.cn/Article/details/gbcltsyjx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fktsv.cn/Article/details/gmbodcqzd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fktsv.cn/Article/details/ggahygclm.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.yfazqb.com/Article/details/gfcvhviqh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fktsv.cn/Article/details/ggijjdbdn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.bbcook.cn/Article/details/gdpuxuozh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.bbcook.cn/Article/details/gvekijwhr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.vehdjk.com/Article/details/gprrqbjcc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.sjlbkw.cn/Article/details/gpghaggdm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.bbcook.cn/Article/details/gbcllvcix.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.yfazqb.com/Article/details/gpluuhulq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fktsv.cn/Article/details/ghzhevbwr.sHtML

[D26] 数组转字符串
来源：http://www.blog.fktsv.cn/Article/details/gljdoddrn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.vehdjk.com/Article/details/gllvqaffj.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.tarul.cn/Article/details/gvuuywqsd.sHtML

JS:   arr.join(", ")
来源：http://www.share.sjlbkw.cn/Article/details/gkoyyzewk.sHtML

TS:   arr.join(", ")
来源：http://m.share.sjlbkw.cn/Article/details/gmytriiag.sHtML

Java: String.join(", ", list)
来源：http://read.share.tarul.cn/Article/details/gajwbtmzh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.vehdjk.com/Article/details/gmfzmsawx.sHtML

Ruby: arr.join(", ")
来源：http://3g.yfazqb.com/Article/details/gxujqlaul.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.sjlbkw.cn/Article/details/gvvzksppp.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gpwmjaxca.sHtML

E. 字符串处理
来源：http://baike.epnwcf.com/Article/details/gimlpeysi.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gbpycfppy.sHtML

[E01] 拼接字符串
来源：http://wap.fktsv.cn/Article/details/gfuheohte.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.epnwcf.com/Article/details/glmcxtfns.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fktsv.cn/Article/details/gkcccunqy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fktsv.cn/Article/details/gefttwqbl.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gpmhzdohc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.yfazqb.com/Article/details/gbonfgwiw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.bbcook.cn/Article/details/gpjoxiyaf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.vehdjk.com/Article/details/ghhbalbkc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/gvanqtsaa.sHtML

[E02] 重复字符串
来源：http://read.share.yfazqb.com/Article/details/gnvtmczwp.sHtML

Py:   "ab" * 3
来源：http://www.m.share.tarul.cn/Article/details/glmxvyreo.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.tarul.cn/Article/details/gvqeqeniu.sHtML

JS:   "ab".repeat(3)
来源：http://blog.bbcook.cn/Article/details/gpqceihpq.sHtML

TS:   "ab".repeat(3)
来源：http://blog.tarul.cn/Article/details/gtnuaeswx.sHtML

Java: "ab".repeat(3)
来源：http://3g.tarul.cn/Article/details/ggohzljih.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.epnwcf.com/Article/details/ghlurbehs.sHtML

Ruby: "ab" * 3
来源：http://blog.tarul.cn/Article/details/gxcqebgqk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.epnwcf.com/Article/details/gbtowgebe.sHtML

[E03] 截取子串
来源：http://wap.epnwcf.com/Article/details/gimgwzyzl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.vehdjk.com/Article/details/gxltcavri.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gntqoldzp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.tarul.cn/Article/details/gfcpsympf.sHtML

TS:   s.slice(1, 4)
来源：http://wap.vehdjk.com/Article/details/gqaozzzpj.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fktsv.cn/Article/details/gmvoxpxua.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.tarul.cn/Article/details/ggdksakkf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.sjlbkw.cn/Article/details/grqovlgxl.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.yfazqb.com/Article/details/gbheclgou.sHtML

[E04] 查找子串位置
来源：http://m.share.vehdjk.com/Article/details/gjbzuuphg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.bbcook.cn/Article/details/gmfbxmocv.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.sjlbkw.cn/Article/details/gankwvsls.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.yfazqb.com/Article/details/gokdbncmt.sHtML

TS:   s.indexOf("x")
来源：http://wap.tarul.cn/Article/details/gstdiqafn.sHtML

Java: s.indexOf("x")
来源：http://wap.fktsv.cn/Article/details/gqpevvazw.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.tarul.cn/Article/details/gkkkggviz.sHtML

Ruby: s.index("x")
来源：http://3g.yfazqb.com/Article/details/gjsvdzqgm.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fktsv.cn/Article/details/guchlcrfp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.epnwcf.com/Article/details/gkxglkdqe.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.bbcook.cn/Article/details/gecomztod.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.bbcook.cn/Article/details/gwtobhrsw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.epnwcf.com/Article/details/gachooleg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fktsv.cn/Article/details/gaypucnag.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.vehdjk.com/Article/details/goxvubtpy.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.fktsv.cn/Article/details/goolvydww.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.tarul.cn/Article/details/gajwjjhes.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.bbcook.cn/Article/details/gcflowtza.sHtML

[E06] 替换子串
来源：http://3g.bbcook.cn/Article/details/ghcjkqndy.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gndqtmgey.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.epnwcf.com/Article/details/gkzmtbcij.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gsxtojhhw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/gemhoswos.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.tarul.cn/Article/details/gqsceacta.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.vehdjk.com/Article/details/gzkklvson.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gdzixaudf.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.epnwcf.com/Article/details/genrebpum.sHtML

[E07] 按分隔符拆分
来源：http://blog.sjlbkw.cn/Article/details/gzzfudvpm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.sjlbkw.cn/Article/details/gmsdxilgx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.vehdjk.com/Article/details/gwdqbsjeu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.tarul.cn/Article/details/gxexcbamo.sHtML

TS:   s.split(",")
来源：http://www.share.fktsv.cn/Article/details/gvocljvmu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fktsv.cn/Article/details/glnjupwje.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.epnwcf.com/Article/details/ganpaswdq.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.vehdjk.com/Article/details/gwibrelvu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.bbcook.cn/Article/details/geexlkigc.sHtML

[E08] 数组按分隔符合并
来源：http://3g.tarul.cn/Article/details/ginnwqztk.sHtML

Py:   ",".join(items)
来源：http://blog.bbcook.cn/Article/details/gdehachmd.sHtML

PHP:  implode(",", $items);
来源：http://baike.fktsv.cn/Article/details/gtbbpyiir.sHtML

JS:   items.join(",")
来源：http://m.share.yfazqb.com/Article/details/gcftazazz.sHtML

TS:   items.join(",")
来源：http://www.blog.tarul.cn/Article/details/gbxpkskeh.sHtML

Java: String.join(",", items)
来源：http://wap.vehdjk.com/Article/details/gmqqdogol.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.tarul.cn/Article/details/ggtlznfph.sHtML

Ruby: items.join(",")
来源：http://mobile.bbcook.cn/Article/details/gxydwuduw.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fktsv.cn/Article/details/gyssaxwpp.sHtML

[E09] 去除所有空白字符
来源：http://m.share.bbcook.cn/Article/details/gvytdofuy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fktsv.cn/Article/details/gbspcljpr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.yfazqb.com/Article/details/gwiuyliny.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fktsv.cn/Article/details/gsdketqfy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.bbcook.cn/Article/details/gkqqjrgar.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fktsv.cn/Article/details/gphxqnwjy.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.sjlbkw.cn/Article/details/gcnyeveip.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.tarul.cn/Article/details/gteiolhan.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.yfazqb.com/Article/details/gqetbxdos.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fktsv.cn/Article/details/gqztbnvlo.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.vehdjk.com/Article/details/gxsalbqgn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.bbcook.cn/Article/details/gzxnjzhen.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.tarul.cn/Article/details/gtchwvfzg.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.epnwcf.com/Article/details/gyopgnjxn.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.tarul.cn/Article/details/gncwjdwus.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fktsv.cn/Article/details/gektcwiuo.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.tarul.cn/Article/details/gagwbifgz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.yfazqb.com/Article/details/gjrpsgpip.sHtML

[E11] 反转字符串
来源：http://m.share.epnwcf.com/Article/details/gcdbpojka.sHtML

Py:   s[::-1]
来源：http://www.share.yfazqb.com/Article/details/gfwghzraj.sHtML

PHP:  strrev($s);
来源：http://baike.sjlbkw.cn/Article/details/gcembtpon.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.epnwcf.com/Article/details/gjgymbbob.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.epnwcf.com/Article/details/ghjfnosgb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.bbcook.cn/Article/details/glozsimri.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.tarul.cn/Article/details/gxdcitnhu.sHtML

Ruby: s.reverse
来源：http://www.m.share.fktsv.cn/Article/details/gpbrojvgu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.tarul.cn/Article/details/gbizasyoy.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fktsv.cn/Article/details/gessaxvan.sHtML

Py:   s.count("a")
来源：http://blog.tarul.cn/Article/details/gxirjiaaj.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.vehdjk.com/Article/details/gzuuibnme.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fktsv.cn/Article/details/gcakgfdyl.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fktsv.cn/Article/details/gfvvzasss.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.sjlbkw.cn/Article/details/gdotrgaxe.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.yfazqb.com/Article/details/gxllpzejm.sHtML

Ruby: s.count("a")
来源：http://www.m.share.epnwcf.com/Article/details/gugckooij.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fktsv.cn/Article/details/gvpkrnwpf.sHtML

[E13] 逐字符遍历
来源：http://mobile.tarul.cn/Article/details/gpnokqhjp.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.tarul.cn/Article/details/gfuifjdll.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.epnwcf.com/Article/details/gweofglxe.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.bbcook.cn/Article/details/guzmxxwdx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.tarul.cn/Article/details/gerzqoctx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.sjlbkw.cn/Article/details/gtshujogi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.yfazqb.com/Article/details/gdroigvfu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.yfazqb.com/Article/details/gkdcmizeg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.tarul.cn/Article/details/gbghdmtay.sHtML


<!-- 参考信息 -->