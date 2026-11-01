代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.tarul.cn/Article/details/geiwfwsfb.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.yfazqb.com/Article/details/gomgfblij.sHtML

[D09] 排序（升序）
来源：http://baike.bbcook.cn/Article/details/gqworjpyc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.epnwcf.com/Article/details/goqzerquq.sHtML

PHP:  sort($arr);
来源：http://www.blog.fktsv.cn/Article/details/gyggeamuk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.sjlbkw.cn/Article/details/grknlkvqk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.yfazqb.com/Article/details/gehlszxcn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.sjlbkw.cn/Article/details/gorsqmevt.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.bbcook.cn/Article/details/ghwohldnm.sHtML

Ruby: arr.sort
来源：http://mobile.epnwcf.com/Article/details/gqsrzneyq.sHtML

C#:   list.Sort();
来源：http://read.share.vehdjk.com/Article/details/gvnnaobfz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.bbcook.cn/Article/details/gbsgiorjh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.epnwcf.com/Article/details/ggnwdogbb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.sjlbkw.cn/Article/details/gvzohdqwh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.yfazqb.com/Article/details/gcbcfjalz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.vehdjk.com/Article/details/gemqgifll.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fktsv.cn/Article/details/gcnybrhsn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.tarul.cn/Article/details/ghzeiizbx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.yfazqb.com/Article/details/gjdflcsrh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.sjlbkw.cn/Article/details/gkhcuxqfb.sHtML

[D11] 反转数组
来源：http://www.m.share.yfazqb.com/Article/details/gyzrlxial.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.sjlbkw.cn/Article/details/gcmputxun.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.tarul.cn/Article/details/gvmghuujs.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.vehdjk.com/Article/details/gcxwldwjq.sHtML

TS:   [...arr].reverse();
来源：http://m.share.sjlbkw.cn/Article/details/gyxsapvsl.sHtML

Java: Collections.reverse(list);
来源：http://m.share.epnwcf.com/Article/details/gpaaegvsw.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.vehdjk.com/Article/details/gyubrgfys.sHtML

Ruby: arr.reverse
来源：http://3g.bbcook.cn/Article/details/gekwmypvr.sHtML

C#:   list.Reverse();
来源：http://read.share.fktsv.cn/Article/details/gvcqfiwiu.sHtML

[D12] 查找元素下标
来源：http://baike.sjlbkw.cn/Article/details/gsssrluly.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.epnwcf.com/Article/details/gykksvyvj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.tarul.cn/Article/details/gmhjriuet.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.yfazqb.com/Article/details/gbewwceyw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fktsv.cn/Article/details/gllouyyel.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fktsv.cn/Article/details/gwfdhlime.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.vehdjk.com/Article/details/gabcjkwle.sHtML

Ruby: arr.index(x)
来源：http://m.share.bbcook.cn/Article/details/geryhbsuz.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.bbcook.cn/Article/details/ggpunqzef.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.sjlbkw.cn/Article/details/gkwfzsheg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.tarul.cn/Article/details/gfcdyekwb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.bbcook.cn/Article/details/gvsfzbjur.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.yfazqb.com/Article/details/gxrjpvgpy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.vehdjk.com/Article/details/grswciana.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.vehdjk.com/Article/details/gzhgppqpl.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.sjlbkw.cn/Article/details/gfvunpter.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.epnwcf.com/Article/details/grxxupfmf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.yfazqb.com/Article/details/glfykoirm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.sjlbkw.cn/Article/details/gmyencnsj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fktsv.cn/Article/details/ggtvxekch.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.yfazqb.com/Article/details/gvpnatyrm.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.yfazqb.com/Article/details/gkngvxrjx.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.bbcook.cn/Article/details/gbdtmrijm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.vehdjk.com/Article/details/gcqckibsf.sHtML

Go:   // 手写循环
来源：http://blog.vehdjk.com/Article/details/gthifmiyl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.yfazqb.com/Article/details/gckgdyatt.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.sjlbkw.cn/Article/details/gvzptvmrn.sHtML

[D15] 去重
来源：http://www.share.bbcook.cn/Article/details/govlaokta.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fktsv.cn/Article/details/gbczvvscl.sHtML

PHP:  array_unique($arr);
来源：http://wap.epnwcf.com/Article/details/gvnqimtxr.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fktsv.cn/Article/details/goagbjgml.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.tarul.cn/Article/details/gficyxjcb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.yfazqb.com/Article/details/grygmkymh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.yfazqb.com/Article/details/gmoezuiev.sHtML

Ruby: arr.uniq
来源：http://m.share.sjlbkw.cn/Article/details/gwyfycdlo.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.vehdjk.com/Article/details/gtxptfoii.sHtML

[D16] 求和与平均值
来源：http://www.blog.fktsv.cn/Article/details/gmrwhkeor.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fktsv.cn/Article/details/gegxgztuw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gubswodiz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.tarul.cn/Article/details/gnwcgawlq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gwvsqepkq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.bbcook.cn/Article/details/gnnfezute.sHtML

Go:   // 手写循环累加
来源：http://blog.sjlbkw.cn/Article/details/gdsvvtwpy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.epnwcf.com/Article/details/gojwxlpwe.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.sjlbkw.cn/Article/details/ghxcvwhum.sHtML

[D17] 最大值与最小值
来源：http://wap.sjlbkw.cn/Article/details/gcjzhdmcj.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.epnwcf.com/Article/details/gdxaymmai.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.sjlbkw.cn/Article/details/gpqpjibfg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.epnwcf.com/Article/details/gcjkugwxt.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fktsv.cn/Article/details/gznxxiuwe.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fktsv.cn/Article/details/gcwfyvcdo.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.bbcook.cn/Article/details/gahisnqtz.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.bbcook.cn/Article/details/gjjzhfavb.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fktsv.cn/Article/details/gbobfvmtg.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.vehdjk.com/Article/details/gybqbdpzu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.epnwcf.com/Article/details/gmbhkbptv.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.epnwcf.com/Article/details/ggckbvifi.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.yfazqb.com/Article/details/gsiislthp.sHtML

TS:   nested.flat();
来源：http://blog.bbcook.cn/Article/details/guhjkimms.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fktsv.cn/Article/details/gdyidgile.sHtML

Go:   // 手写双层循环
来源：http://wap.tarul.cn/Article/details/govvrcrgq.sHtML

Ruby: nested.flatten
来源：http://www.m.share.bbcook.cn/Article/details/gfkkkonze.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.yfazqb.com/Article/details/gejyrewcj.sHtML

[D19] 按字段分组
来源：http://www.m.share.fktsv.cn/Article/details/gonanhifa.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.tarul.cn/Article/details/gatypvrra.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.bbcook.cn/Article/details/gynnkxgpp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.sjlbkw.cn/Article/details/gzafedsrl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.bbcook.cn/Article/details/glhenqtpo.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.yfazqb.com/Article/details/gonifjxnw.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.sjlbkw.cn/Article/details/gsvuezccr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.sjlbkw.cn/Article/details/gxvdtlpxx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.yfazqb.com/Article/details/gzqzkzpsz.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fktsv.cn/Article/details/gknaqfbjq.sHtML

Py:   Counter(arr)
来源：http://baike.tarul.cn/Article/details/gqliqoeuk.sHtML

PHP:  array_count_values($arr);
来源：http://blog.bbcook.cn/Article/details/gkovxrjqg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fktsv.cn/Article/details/gkmnnxzbh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fktsv.cn/Article/details/ghkmniaym.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.epnwcf.com/Article/details/gkbmuocxt.sHtML

Go:   // 手写 map[T]int
来源：http://baike.sjlbkw.cn/Article/details/gdplzdzcp.sHtML

Ruby: arr.tally
来源：http://www.share.bbcook.cn/Article/details/gemnrqjkj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.vehdjk.com/Article/details/ghzaasecf.sHtML

[D21] 判断是否包含某元素
来源：http://3g.epnwcf.com/Article/details/gccdkugsx.sHtML

Py:   x in arr
来源：http://www.share.sjlbkw.cn/Article/details/gvzkdtyxj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.sjlbkw.cn/Article/details/gzwhkkbdl.sHtML

JS:   arr.includes(x)
来源：http://blog.yfazqb.com/Article/details/gqbxnpdca.sHtML

TS:   arr.includes(x)
来源：http://m.share.tarul.cn/Article/details/gevgupelc.sHtML

Java: list.contains(x)
来源：http://baike.vehdjk.com/Article/details/gvgumszfk.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.epnwcf.com/Article/details/grkougcsj.sHtML

Ruby: arr.include?(x)
来源：http://read.share.sjlbkw.cn/Article/details/gwhwwvffq.sHtML

C#:   list.Contains(x)
来源：http://m.share.fktsv.cn/Article/details/gqwlwkfbf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.bbcook.cn/Article/details/gojpbplhj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.bbcook.cn/Article/details/gibyjcsff.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.bbcook.cn/Article/details/gfyvnnjyn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.epnwcf.com/Article/details/gjjjwhese.sHtML

TS:   [...arr];
来源：http://www.m.share.yfazqb.com/Article/details/gwnuxwtih.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.yfazqb.com/Article/details/gktcghedy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.vehdjk.com/Article/details/gtzgktieg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.yfazqb.com/Article/details/gxcbmhjrv.sHtML

C#:   new List<int>(list);
来源：http://mobile.vehdjk.com/Article/details/gnuyddtmm.sHtML

[D23] reduce 累积计算
来源：http://mobile.fktsv.cn/Article/details/gegjjxvlu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.yfazqb.com/Article/details/gheoqmxpf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.tarul.cn/Article/details/gknhhojju.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.bbcook.cn/Article/details/gahakscuz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.sjlbkw.cn/Article/details/ghcjtcjno.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.bbcook.cn/Article/details/gkypwhzxx.sHtML

Go:   // 手写循环
来源：http://www.share.fktsv.cn/Article/details/gynjvqglj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fktsv.cn/Article/details/gbhewkdqe.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fktsv.cn/Article/details/gphnvrwpm.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.tarul.cn/Article/details/guelcxqlo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.sjlbkw.cn/Article/details/gluzxlein.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.yfazqb.com/Article/details/giaqmjevg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.yfazqb.com/Article/details/gtyclzebq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.sjlbkw.cn/Article/details/gqgedjkyu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.epnwcf.com/Article/details/gkzmxdnys.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fktsv.cn/Article/details/gkckvxkwe.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.tarul.cn/Article/details/gxuiubdjv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.yfazqb.com/Article/details/grpgrdssk.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.sjlbkw.cn/Article/details/gyqbiutmf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fktsv.cn/Article/details/gmxsfgsjv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.tarul.cn/Article/details/gtykslizp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.tarul.cn/Article/details/gsfmknriw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.bbcook.cn/Article/details/gasydqyli.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fktsv.cn/Article/details/ggpwzjjut.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.vehdjk.com/Article/details/gxnyyyutg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.vehdjk.com/Article/details/gukwyqacu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.vehdjk.com/Article/details/gveacdisx.sHtML

[D26] 数组转字符串
来源：http://3g.yfazqb.com/Article/details/gbrascgwj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.epnwcf.com/Article/details/grvfeatla.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.yfazqb.com/Article/details/grrtkamqx.sHtML

JS:   arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/gnhlwcygc.sHtML

TS:   arr.join(", ")
来源：http://mobile.sjlbkw.cn/Article/details/gacsrzneo.sHtML

Java: String.join(", ", list)
来源：http://read.share.vehdjk.com/Article/details/gdoyazeak.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.bbcook.cn/Article/details/gdxskggdb.sHtML

Ruby: arr.join(", ")
来源：http://www.share.bbcook.cn/Article/details/gsaqjgofu.sHtML

C#:   string.Join(", ", list)
来源：http://baike.epnwcf.com/Article/details/gjxeznwnp.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gsgozivti.sHtML

E. 字符串处理
来源：http://baike.yfazqb.com/Article/details/goxcnvadw.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gchliqurh.sHtML

[E01] 拼接字符串
来源：http://www.share.bbcook.cn/Article/details/govlxbjtk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fktsv.cn/Article/details/geslzousn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fktsv.cn/Article/details/geflsxhiq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.yfazqb.com/Article/details/gkqjkiucl.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.sjlbkw.cn/Article/details/ghdcsguaw.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.yfazqb.com/Article/details/gxlyhacem.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.tarul.cn/Article/details/gwrbpyqfg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fktsv.cn/Article/details/gxkctouyq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.yfazqb.com/Article/details/gfspmcujw.sHtML

[E02] 重复字符串
来源：http://blog.fktsv.cn/Article/details/ghsuszrgl.sHtML

Py:   "ab" * 3
来源：http://www.m.share.vehdjk.com/Article/details/gweizwyri.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fktsv.cn/Article/details/gausvuklm.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.bbcook.cn/Article/details/gmgkqbcux.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fktsv.cn/Article/details/gaubuklez.sHtML

Java: "ab".repeat(3)
来源：http://read.share.bbcook.cn/Article/details/gxupowuve.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.tarul.cn/Article/details/gsufziwyl.sHtML

Ruby: "ab" * 3
来源：http://3g.bbcook.cn/Article/details/gqvqdnrms.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.tarul.cn/Article/details/ggepfzroj.sHtML

[E03] 截取子串
来源：http://read.share.tarul.cn/Article/details/grnfpkztk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fktsv.cn/Article/details/gyhcktklg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.bbcook.cn/Article/details/gyukvocpn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.tarul.cn/Article/details/giktkitbn.sHtML

TS:   s.slice(1, 4)
来源：http://blog.vehdjk.com/Article/details/gaegbwuah.sHtML

Java: s.substring(1, 4)
来源：http://baike.tarul.cn/Article/details/gffyehfuk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fktsv.cn/Article/details/gkhiwslfc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.tarul.cn/Article/details/gotypmush.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.yfazqb.com/Article/details/gqgiypkex.sHtML

[E04] 查找子串位置
来源：http://www.share.sjlbkw.cn/Article/details/gjrabomww.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.sjlbkw.cn/Article/details/gdhtwpwfe.sHtML

PHP:  strpos($s, "x");
来源：http://3g.vehdjk.com/Article/details/gwtebvvli.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fktsv.cn/Article/details/gueddqpau.sHtML

TS:   s.indexOf("x")
来源：http://wap.bbcook.cn/Article/details/gngvcrxau.sHtML

Java: s.indexOf("x")
来源：http://www.share.vehdjk.com/Article/details/gbllbtlqj.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.bbcook.cn/Article/details/gskypuvmb.sHtML

Ruby: s.index("x")
来源：http://www.m.share.vehdjk.com/Article/details/glbgtpvkv.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.tarul.cn/Article/details/gyhxkulpz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.vehdjk.com/Article/details/ghplbvrcj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.sjlbkw.cn/Article/details/gmtytsntq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.yfazqb.com/Article/details/gtqwfsldh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.bbcook.cn/Article/details/gbrxpeqhu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.vehdjk.com/Article/details/gmurmpzqq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fktsv.cn/Article/details/gvhqppgtr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.fktsv.cn/Article/details/gfhdwkknr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fktsv.cn/Article/details/gjdcybxdt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.tarul.cn/Article/details/gpmqyxvoq.sHtML

[E06] 替换子串
来源：http://www.m.share.tarul.cn/Article/details/gndjvyzyt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.tarul.cn/Article/details/gwgcgxksy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.yfazqb.com/Article/details/gwffrxhfp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.vehdjk.com/Article/details/gyfgapehw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/ggmvqbbsw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gusaqtraq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.bbcook.cn/Article/details/gsxnekdot.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gmylcgclw.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fktsv.cn/Article/details/gvhffykjq.sHtML

[E07] 按分隔符拆分
来源：http://blog.sjlbkw.cn/Article/details/grzqusdrd.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.sjlbkw.cn/Article/details/gsuipmcjl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fktsv.cn/Article/details/grkgsmwku.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fktsv.cn/Article/details/gxbbtbhlj.sHtML

TS:   s.split(",")
来源：http://mobile.vehdjk.com/Article/details/ghlsosxzx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.bbcook.cn/Article/details/ggcdyuxup.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fktsv.cn/Article/details/gbjqpjcvv.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.sjlbkw.cn/Article/details/gfbxpqwof.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.epnwcf.com/Article/details/gsgcqzvlb.sHtML

[E08] 数组按分隔符合并
来源：http://baike.epnwcf.com/Article/details/gvcrlgskk.sHtML

Py:   ",".join(items)
来源：http://wap.sjlbkw.cn/Article/details/gekddymdp.sHtML

PHP:  implode(",", $items);
来源：http://3g.fktsv.cn/Article/details/gpmxbvwbb.sHtML

JS:   items.join(",")
来源：http://3g.epnwcf.com/Article/details/gshpzjphd.sHtML

TS:   items.join(",")
来源：http://www.share.fktsv.cn/Article/details/grnbirwjs.sHtML

Java: String.join(",", items)
来源：http://www.blog.fktsv.cn/Article/details/ghpivymgy.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.sjlbkw.cn/Article/details/guxikzwfs.sHtML

Ruby: items.join(",")
来源：http://3g.sjlbkw.cn/Article/details/guecgcfxy.sHtML

C#:   string.Join(",", items)
来源：http://baike.yfazqb.com/Article/details/gysygivfi.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fktsv.cn/Article/details/gkilixamw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.yfazqb.com/Article/details/goiaxqwjy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fktsv.cn/Article/details/gvjlrclms.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fktsv.cn/Article/details/gwxnlgglb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fktsv.cn/Article/details/gmegglqaj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.sjlbkw.cn/Article/details/gtwdorwaw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.vehdjk.com/Article/details/gfoxmbphc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fktsv.cn/Article/details/gxwapeswb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.epnwcf.com/Article/details/gfqfhkxuh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.vehdjk.com/Article/details/gozfvxtvz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.yfazqb.com/Article/details/gmymbjtpt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.sjlbkw.cn/Article/details/gbbggpqex.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.vehdjk.com/Article/details/givkupndv.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.epnwcf.com/Article/details/gypgvtyqx.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.bbcook.cn/Article/details/gqyqxdsdj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.bbcook.cn/Article/details/gurbyzxqz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.yfazqb.com/Article/details/gkanntoaq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.yfazqb.com/Article/details/gvlxncyna.sHtML

[E11] 反转字符串
来源：http://blog.epnwcf.com/Article/details/gmbdhyguu.sHtML

Py:   s[::-1]
来源：http://m.share.tarul.cn/Article/details/ggfvfbojq.sHtML

PHP:  strrev($s);
来源：http://read.share.yfazqb.com/Article/details/gznoowjnb.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.sjlbkw.cn/Article/details/gsketucjx.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.epnwcf.com/Article/details/gvtnmlwkr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.vehdjk.com/Article/details/gvywlnjig.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.bbcook.cn/Article/details/gxlhmmzrl.sHtML

Ruby: s.reverse
来源：http://mobile.bbcook.cn/Article/details/groikiyrx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.tarul.cn/Article/details/gqkvsbcgl.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.sjlbkw.cn/Article/details/ggwbsvkyf.sHtML

Py:   s.count("a")
来源：http://blog.vehdjk.com/Article/details/gsarotetc.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.yfazqb.com/Article/details/gpkfkosby.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.tarul.cn/Article/details/gnbdcchso.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fktsv.cn/Article/details/gqkedmbcs.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.tarul.cn/Article/details/gegieputj.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.bbcook.cn/Article/details/gsagyucgv.sHtML

Ruby: s.count("a")
来源：http://mobile.vehdjk.com/Article/details/gxkedocqg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.bbcook.cn/Article/details/gtbcjcrby.sHtML

[E13] 逐字符遍历
来源：http://m.share.vehdjk.com/Article/details/gybcupxfo.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fktsv.cn/Article/details/gxiockrsb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fktsv.cn/Article/details/gevctxclr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.sjlbkw.cn/Article/details/gmvjvjhdq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.bbcook.cn/Article/details/gkuznclck.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.vehdjk.com/Article/details/gouwjhhjt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.epnwcf.com/Article/details/gwlnjkzcb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.sjlbkw.cn/Article/details/gtwagmfil.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.sjlbkw.cn/Article/details/geuzgoofk.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.sjlbkw.cn/Article/details/gbxhgpmlk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fktsv.cn/Article/details/gpgqunqas.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.bbcook.cn/Article/details/gpggjptvj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.bbcook.cn/Article/details/gdufdzozx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fktsv.cn/Article/details/gapijzqkg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.vehdjk.com/Article/details/gniykdjka.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.epnwcf.com/Article/details/glghkejjh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.epnwcf.com/Article/details/gskqtdhha.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.epnwcf.com/Article/details/gnfshmkro.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.epnwcf.com/Article/details/grshaqqrw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.sjlbkw.cn/Article/details/gncihwdzo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.bbcook.cn/Article/details/gpdwzyxmv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.bbcook.cn/Article/details/ggjjdstmz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.sjlbkw.cn/Article/details/gaeszjzyj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.vehdjk.com/Article/details/ghvrbakma.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fktsv.cn/Article/details/gqzyigmdv.sHtML


<!-- 参考信息 -->