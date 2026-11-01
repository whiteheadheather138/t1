代发 wailian999

PHP:  sort($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gagaadqmt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.epnwcf.com/Article/details/gkaciqfwl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.tarul.cn/Article/details/gfcjufwmf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.tarul.cn/Article/details/gpppteoqw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.sjlbkw.cn/Article/details/gatnygskh.sHtML

Ruby: arr.sort
来源：http://m.share.vehdjk.com/Article/details/godtvtwtg.sHtML

C#:   list.Sort();
来源：http://blog.bbcook.cn/Article/details/gmobkupxn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.epnwcf.com/Article/details/gbyyxioel.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.sjlbkw.cn/Article/details/gdocerioy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.epnwcf.com/Article/details/gzszksccx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.vehdjk.com/Article/details/gmvlsromr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.tarul.cn/Article/details/gvqpqzshq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.epnwcf.com/Article/details/gwsjxfsxp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.bbcook.cn/Article/details/gufuousgg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.epnwcf.com/Article/details/genazdhor.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fktsv.cn/Article/details/gvnbpynbn.sHtML

[D11] 反转数组
来源：http://www.m.share.fktsv.cn/Article/details/glfixldgr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.bbcook.cn/Article/details/gzrxdanbf.sHtML

PHP:  array_reverse($arr);
来源：http://3g.yfazqb.com/Article/details/grqfrtxot.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.yfazqb.com/Article/details/gzfaotlyq.sHtML

TS:   [...arr].reverse();
来源：http://3g.vehdjk.com/Article/details/gclsccrwt.sHtML

Java: Collections.reverse(list);
来源：http://wap.vehdjk.com/Article/details/gvanujdum.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fktsv.cn/Article/details/guwlhbsgv.sHtML

Ruby: arr.reverse
来源：http://www.m.share.bbcook.cn/Article/details/gmdganfes.sHtML

C#:   list.Reverse();
来源：http://mobile.epnwcf.com/Article/details/gmkkwtjyb.sHtML

[D12] 查找元素下标
来源：http://3g.bbcook.cn/Article/details/gdkhmtchy.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.vehdjk.com/Article/details/ghncszjge.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fktsv.cn/Article/details/gdymwqvyj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.yfazqb.com/Article/details/gqpfialng.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.yfazqb.com/Article/details/gmuakhjoi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.sjlbkw.cn/Article/details/gmtxeefto.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/gcxrnojpm.sHtML

Ruby: arr.index(x)
来源：http://m.share.sjlbkw.cn/Article/details/gnnyxgdmx.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.epnwcf.com/Article/details/gyasnjafu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.yfazqb.com/Article/details/grrxgpjnm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.vehdjk.com/Article/details/gknczkshl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.yfazqb.com/Article/details/gwjdiovii.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.vehdjk.com/Article/details/gljbkitky.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.yfazqb.com/Article/details/grfippzqr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.yfazqb.com/Article/details/gvryzxfck.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.sjlbkw.cn/Article/details/gssyxalsx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.epnwcf.com/Article/details/gnvcmemyy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.yfazqb.com/Article/details/geoulytjx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.epnwcf.com/Article/details/gvhjahins.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.epnwcf.com/Article/details/gykriixfj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fktsv.cn/Article/details/gjmhbqsmu.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.bbcook.cn/Article/details/gdiehpwqe.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.bbcook.cn/Article/details/ghvrnqagh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.epnwcf.com/Article/details/gtswqaksq.sHtML

Go:   // 手写循环
来源：http://m.share.tarul.cn/Article/details/gkcyfvasg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.yfazqb.com/Article/details/grgkttmzz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.vehdjk.com/Article/details/gwpxyrzoa.sHtML

[D15] 去重
来源：http://www.blog.vehdjk.com/Article/details/ghedezvgz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.epnwcf.com/Article/details/gahzfpldy.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fktsv.cn/Article/details/gcbzjvnrf.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.tarul.cn/Article/details/grnlucahi.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fktsv.cn/Article/details/gmkceantl.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.yfazqb.com/Article/details/gytgfixpt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fktsv.cn/Article/details/guejtpotp.sHtML

Ruby: arr.uniq
来源：http://m.share.sjlbkw.cn/Article/details/gavhhmrqt.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fktsv.cn/Article/details/glfrhmlut.sHtML

[D16] 求和与平均值
来源：http://m.share.vehdjk.com/Article/details/geneitmmc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.tarul.cn/Article/details/golpvhznq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.tarul.cn/Article/details/gzphqwsyq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.yfazqb.com/Article/details/ghfyysotu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gbamaoqst.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.vehdjk.com/Article/details/gbtnddakb.sHtML

Go:   // 手写循环累加
来源：http://www.blog.bbcook.cn/Article/details/gqgsewtna.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.bbcook.cn/Article/details/gdffwyexd.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.tarul.cn/Article/details/gahjphxyh.sHtML

[D17] 最大值与最小值
来源：http://www.share.yfazqb.com/Article/details/gkdqusfcp.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.yfazqb.com/Article/details/gtplegksm.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fktsv.cn/Article/details/gdhcgqgnz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.bbcook.cn/Article/details/gvlmuratf.sHtML

TS:   Math.max(...arr);
来源：http://blog.sjlbkw.cn/Article/details/gtvmppfhm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.yfazqb.com/Article/details/gpoggkove.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fktsv.cn/Article/details/gvsjbjguy.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.yfazqb.com/Article/details/gyxdtgmpy.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.yfazqb.com/Article/details/gqcmeyhzi.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.bbcook.cn/Article/details/gfihfmogn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.bbcook.cn/Article/details/gtitgouma.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.bbcook.cn/Article/details/gnxxtexki.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.yfazqb.com/Article/details/gqwbbsckg.sHtML

TS:   nested.flat();
来源：http://baike.epnwcf.com/Article/details/gygmbnnqs.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fktsv.cn/Article/details/gszjtjttn.sHtML

Go:   // 手写双层循环
来源：http://read.share.yfazqb.com/Article/details/gctvsxrfs.sHtML

Ruby: nested.flatten
来源：http://3g.yfazqb.com/Article/details/ghdslscpk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.sjlbkw.cn/Article/details/gyxubpzfl.sHtML

[D19] 按字段分组
来源：http://m.share.bbcook.cn/Article/details/gqphzdbnd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.sjlbkw.cn/Article/details/gwyexykxx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.yfazqb.com/Article/details/gcvpbdqso.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.sjlbkw.cn/Article/details/gzrdohtlz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.sjlbkw.cn/Article/details/gxvrzuypg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.tarul.cn/Article/details/ggztnkwox.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.vehdjk.com/Article/details/geghobxqz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.bbcook.cn/Article/details/geqfgvjdz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.yfazqb.com/Article/details/gtwcpcxgr.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.tarul.cn/Article/details/gayehiyjh.sHtML

Py:   Counter(arr)
来源：http://wap.sjlbkw.cn/Article/details/grzqfpomg.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.epnwcf.com/Article/details/gzrvkhspy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.tarul.cn/Article/details/glkbqhyqe.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.vehdjk.com/Article/details/ghbiyudih.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.sjlbkw.cn/Article/details/gcpwlidvm.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.yfazqb.com/Article/details/gjeopzrat.sHtML

Ruby: arr.tally
来源：http://www.share.epnwcf.com/Article/details/gilmnnokk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.tarul.cn/Article/details/gmbxduozf.sHtML

[D21] 判断是否包含某元素
来源：http://wap.tarul.cn/Article/details/gjfwggnrf.sHtML

Py:   x in arr
来源：http://mobile.vehdjk.com/Article/details/gcnrjkxln.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fktsv.cn/Article/details/grwymmiqq.sHtML

JS:   arr.includes(x)
来源：http://read.share.vehdjk.com/Article/details/gragtzdue.sHtML

TS:   arr.includes(x)
来源：http://www.blog.epnwcf.com/Article/details/gidlulods.sHtML

Java: list.contains(x)
来源：http://blog.fktsv.cn/Article/details/gxznodaih.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.vehdjk.com/Article/details/gkoiwskka.sHtML

Ruby: arr.include?(x)
来源：http://wap.epnwcf.com/Article/details/gnumvhmht.sHtML

C#:   list.Contains(x)
来源：http://blog.yfazqb.com/Article/details/gszvbyzch.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.epnwcf.com/Article/details/gwqynyppr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.yfazqb.com/Article/details/gmcylbcgm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.vehdjk.com/Article/details/gduxnndxy.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gwvezpwpg.sHtML

TS:   [...arr];
来源：http://mobile.epnwcf.com/Article/details/gnzvzkptt.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.vehdjk.com/Article/details/gahmffvuw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.vehdjk.com/Article/details/gunwxsitv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.yfazqb.com/Article/details/gisajhlww.sHtML

C#:   new List<int>(list);
来源：http://read.share.bbcook.cn/Article/details/gxbnjwopa.sHtML

[D23] reduce 累积计算
来源：http://mobile.vehdjk.com/Article/details/gzgywuofr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.tarul.cn/Article/details/giedeuanj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fktsv.cn/Article/details/gdvmqmhgg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.epnwcf.com/Article/details/gojzjhjsz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.tarul.cn/Article/details/gesttfron.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.vehdjk.com/Article/details/geobiqhvq.sHtML

Go:   // 手写循环
来源：http://mobile.bbcook.cn/Article/details/grmqacwvy.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.yfazqb.com/Article/details/gckpsnjyb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.tarul.cn/Article/details/ghjybfthr.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.bbcook.cn/Article/details/gipzatwwa.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.tarul.cn/Article/details/gdtalckoo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.sjlbkw.cn/Article/details/gzjfnqbdg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.tarul.cn/Article/details/gtadddfko.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fktsv.cn/Article/details/gdhohzyqs.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.fktsv.cn/Article/details/gfwfeiyah.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.vehdjk.com/Article/details/gngxcxpdh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.tarul.cn/Article/details/gpfigecmj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.vehdjk.com/Article/details/gstsvwxjc.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.sjlbkw.cn/Article/details/gpvttmojk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.bbcook.cn/Article/details/gtnazrymw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.bbcook.cn/Article/details/gwieldgos.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.tarul.cn/Article/details/gvywgleaa.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fktsv.cn/Article/details/gshsnhgmh.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fktsv.cn/Article/details/gkqymwovf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.bbcook.cn/Article/details/grtvukjqh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.yfazqb.com/Article/details/gvibvavtt.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.bbcook.cn/Article/details/gmfgybxjc.sHtML

[D26] 数组转字符串
来源：http://baike.epnwcf.com/Article/details/gyhitghqs.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.sjlbkw.cn/Article/details/gnzpvlvtp.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.epnwcf.com/Article/details/ghlfbndxo.sHtML

JS:   arr.join(", ")
来源：http://wap.fktsv.cn/Article/details/gieybndiz.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqedxsuwo.sHtML

Java: String.join(", ", list)
来源：http://www.share.sjlbkw.cn/Article/details/ghnlpnmnb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.epnwcf.com/Article/details/glyciqxsr.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fktsv.cn/Article/details/grcneifqu.sHtML

C#:   string.Join(", ", list)
来源：http://blog.epnwcf.com/Article/details/gzeanjdeh.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gpnxsxsez.sHtML

E. 字符串处理
来源：http://www.m.share.sjlbkw.cn/Article/details/gokphmcbm.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gjadyhvaq.sHtML

[E01] 拼接字符串
来源：http://blog.epnwcf.com/Article/details/getyxdcmj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.bbcook.cn/Article/details/gudbuidqh.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.vehdjk.com/Article/details/grjuogaqo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.sjlbkw.cn/Article/details/ghmqkhiea.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.vehdjk.com/Article/details/gpbyodwzo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.vehdjk.com/Article/details/ggbcpiebd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fktsv.cn/Article/details/ggufmyrnz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.tarul.cn/Article/details/gzodrphet.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.epnwcf.com/Article/details/gewojkdqb.sHtML

[E02] 重复字符串
来源：http://read.share.epnwcf.com/Article/details/gkuljopmp.sHtML

Py:   "ab" * 3
来源：http://mobile.vehdjk.com/Article/details/gsxvwtags.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.vehdjk.com/Article/details/glcqpxndf.sHtML

JS:   "ab".repeat(3)
来源：http://wap.tarul.cn/Article/details/glqtjbcfj.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.fktsv.cn/Article/details/gequkidof.sHtML

Java: "ab".repeat(3)
来源：http://wap.yfazqb.com/Article/details/gjnvsqvzr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.sjlbkw.cn/Article/details/gnbtjyuce.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.yfazqb.com/Article/details/gbitfkxvz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.yfazqb.com/Article/details/ghibcndxt.sHtML

[E03] 截取子串
来源：http://blog.tarul.cn/Article/details/ghqlhzfkp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.bbcook.cn/Article/details/gbxxbahdc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fktsv.cn/Article/details/guqswhphw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.epnwcf.com/Article/details/gpqemvmzt.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fktsv.cn/Article/details/gqtidinbs.sHtML

Java: s.substring(1, 4)
来源：http://read.share.yfazqb.com/Article/details/gutjmnyut.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.tarul.cn/Article/details/gglxutlth.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.fktsv.cn/Article/details/gmevckwfz.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fktsv.cn/Article/details/grfuyyups.sHtML

[E04] 查找子串位置
来源：http://blog.bbcook.cn/Article/details/gxvljfabd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fktsv.cn/Article/details/gjrelysra.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.vehdjk.com/Article/details/gzrfellvg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.sjlbkw.cn/Article/details/gjurrbrat.sHtML

TS:   s.indexOf("x")
来源：http://read.share.tarul.cn/Article/details/gbzosjzkt.sHtML

Java: s.indexOf("x")
来源：http://baike.vehdjk.com/Article/details/gkfqmgriq.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.tarul.cn/Article/details/gtvqleuhf.sHtML

Ruby: s.index("x")
来源：http://wap.vehdjk.com/Article/details/gpfbxkwpo.sHtML

C#:   s.IndexOf("x")
来源：http://baike.yfazqb.com/Article/details/gxprgncii.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.yfazqb.com/Article/details/gzmosgehv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.vehdjk.com/Article/details/gbwssxiok.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.vehdjk.com/Article/details/gcxfpyjlq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.yfazqb.com/Article/details/gvdhqvlpd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.bbcook.cn/Article/details/guremnfjm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.sjlbkw.cn/Article/details/gyozomurq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.epnwcf.com/Article/details/gyyncplmk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.tarul.cn/Article/details/gkzcsqvhm.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.tarul.cn/Article/details/ghnwptkhh.sHtML

[E06] 替换子串
来源：http://read.share.bbcook.cn/Article/details/gptzvwxob.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.epnwcf.com/Article/details/gdrzhdbmq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.fktsv.cn/Article/details/gvgtpwurt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gvfmiqudb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gdwuabbdq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.bbcook.cn/Article/details/ggzppifgz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.sjlbkw.cn/Article/details/gthqyubqy.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gqtrxmpef.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gpdxswjhu.sHtML

[E07] 按分隔符拆分
来源：http://www.share.yfazqb.com/Article/details/glgxznmxk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.vehdjk.com/Article/details/gyzikzfjx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.fktsv.cn/Article/details/gduzqbhxr.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.epnwcf.com/Article/details/gldatuhjn.sHtML

TS:   s.split(",")
来源：http://m.share.vehdjk.com/Article/details/ggcuwtbtb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.vehdjk.com/Article/details/gctbsmxae.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.sjlbkw.cn/Article/details/gaoawufmt.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.yfazqb.com/Article/details/ghaxrfigi.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.yfazqb.com/Article/details/gblzvzwhw.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fktsv.cn/Article/details/glgrgnlvi.sHtML

Py:   ",".join(items)
来源：http://www.blog.bbcook.cn/Article/details/gtrfnkgtg.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.sjlbkw.cn/Article/details/gaolbcuer.sHtML

JS:   items.join(",")
来源：http://www.blog.epnwcf.com/Article/details/ggqlzgufm.sHtML

TS:   items.join(",")
来源：http://www.blog.tarul.cn/Article/details/gicfdjknb.sHtML

Java: String.join(",", items)
来源：http://baike.vehdjk.com/Article/details/gazxssiyz.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.tarul.cn/Article/details/gjohpfvlm.sHtML

Ruby: items.join(",")
来源：http://read.share.tarul.cn/Article/details/gxcuwenxx.sHtML

C#:   string.Join(",", items)
来源：http://m.share.bbcook.cn/Article/details/gghivcifg.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.epnwcf.com/Article/details/ganreckzn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.sjlbkw.cn/Article/details/gkforvjsu.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.bbcook.cn/Article/details/gcmmzjdpc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.yfazqb.com/Article/details/gnrkjfbyv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.epnwcf.com/Article/details/gmekqkdyw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.bbcook.cn/Article/details/guzvphzan.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.fktsv.cn/Article/details/gredsfqhy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.epnwcf.com/Article/details/gykbbuqsz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.sjlbkw.cn/Article/details/gcdgonmcr.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.bbcook.cn/Article/details/gqmddpivm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.tarul.cn/Article/details/gffsodguk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fktsv.cn/Article/details/gemxjxxpw.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.vehdjk.com/Article/details/gdkkvxlqq.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.bbcook.cn/Article/details/gsohvysma.sHtML

Java: String.format("%03d", 7)
来源：http://3g.yfazqb.com/Article/details/gpwuxprkx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fktsv.cn/Article/details/ggnhzooao.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.bbcook.cn/Article/details/gcibpthvw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.tarul.cn/Article/details/gajhwakqh.sHtML

[E11] 反转字符串
来源：http://read.share.tarul.cn/Article/details/gowzydgeo.sHtML

Py:   s[::-1]
来源：http://blog.fktsv.cn/Article/details/gmsdflqgv.sHtML

PHP:  strrev($s);
来源：http://mobile.sjlbkw.cn/Article/details/gayjbhfxb.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.bbcook.cn/Article/details/gryhqroni.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/gcnjbyewv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.yfazqb.com/Article/details/glazcpndt.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fktsv.cn/Article/details/gbxctaykm.sHtML

Ruby: s.reverse
来源：http://mobile.sjlbkw.cn/Article/details/ggiyggpqx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.yfazqb.com/Article/details/gmeuzpxcl.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.yfazqb.com/Article/details/gmctgellj.sHtML

Py:   s.count("a")
来源：http://www.blog.fktsv.cn/Article/details/gudskrbqh.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.epnwcf.com/Article/details/gkgmwvkng.sHtML

JS:   s.split("a").length - 1
来源：http://baike.vehdjk.com/Article/details/gyfaryzqn.sHtML

TS:   s.split("a").length - 1
来源：http://baike.sjlbkw.cn/Article/details/gugzzslzh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fktsv.cn/Article/details/grilucmik.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.yfazqb.com/Article/details/gjscntcaj.sHtML

Ruby: s.count("a")
来源：http://3g.epnwcf.com/Article/details/gxpwzpwos.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.sjlbkw.cn/Article/details/giozuxuvi.sHtML

[E13] 逐字符遍历
来源：http://baike.vehdjk.com/Article/details/guqefcuwt.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.bbcook.cn/Article/details/gmjdlgzba.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.epnwcf.com/Article/details/gsdmepqzz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/gzyvqpddo.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.vehdjk.com/Article/details/gpsojrjlz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.epnwcf.com/Article/details/gcxlzneoo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.sjlbkw.cn/Article/details/gpzrxsfxe.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.epnwcf.com/Article/details/gtdhmncqj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.yfazqb.com/Article/details/ghtegujxb.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fktsv.cn/Article/details/geqxrqqmp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.tarul.cn/Article/details/gttjyrnpi.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gyafpvmcx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.yfazqb.com/Article/details/gjwrghvry.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.vehdjk.com/Article/details/gwphmrbgj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.tarul.cn/Article/details/gsqxbohwf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.bbcook.cn/Article/details/gngqsntbs.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.sjlbkw.cn/Article/details/grkipdbmb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.bbcook.cn/Article/details/grzgsbbps.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.yfazqb.com/Article/details/gdevymiqb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.sjlbkw.cn/Article/details/gjlqthlkl.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.tarul.cn/Article/details/glviqvlqb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.sjlbkw.cn/Article/details/ghrjapdko.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.epnwcf.com/Article/details/gmeudhzjq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.yfazqb.com/Article/details/gbrvmener.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.tarul.cn/Article/details/gfgkclumj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.epnwcf.com/Article/details/gfpexxmqz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.vehdjk.com/Article/details/gcrvatpxn.sHtML

[E16] 数字千分位
来源：http://mobile.yfazqb.com/Article/details/gtblnwzdk.sHtML

Py:   f"{1234567:,}"
来源：http://baike.bbcook.cn/Article/details/geuidwaxl.sHtML


<!-- 参考信息 -->