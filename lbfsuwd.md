代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.sjlbkw.cn/Article/details/gcxoeixhz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.bbcook.cn/Article/details/gxbausvdl.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.tarul.cn/Article/details/gyubtkmrb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fktsv.cn/Article/details/gbajlhjnx.sHtML

[D11] 反转数组
来源：http://baike.tarul.cn/Article/details/ghjbaosxe.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.tarul.cn/Article/details/gabihwytq.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gymgyqoce.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.bbcook.cn/Article/details/ggeriovgp.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fktsv.cn/Article/details/gsijtfuce.sHtML

Java: Collections.reverse(list);
来源：http://baike.fktsv.cn/Article/details/gejiwmmbn.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.epnwcf.com/Article/details/gtbxhmtdf.sHtML

Ruby: arr.reverse
来源：http://blog.tarul.cn/Article/details/gtcnusjkl.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fktsv.cn/Article/details/gpqdftehe.sHtML

[D12] 查找元素下标
来源：http://blog.vehdjk.com/Article/details/gbawoncdc.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.yfazqb.com/Article/details/grcstbcns.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.bbcook.cn/Article/details/gakkfhssp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.yfazqb.com/Article/details/gowzpjvyd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.vehdjk.com/Article/details/ghoxntwit.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.tarul.cn/Article/details/gucsyyudh.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.vehdjk.com/Article/details/ghgbwxbqw.sHtML

Ruby: arr.index(x)
来源：http://m.share.yfazqb.com/Article/details/gsryznogd.sHtML

C#:   list.IndexOf(x);
来源：http://wap.epnwcf.com/Article/details/grtrzkgub.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fktsv.cn/Article/details/gtvhflyrt.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.epnwcf.com/Article/details/gmklrfxzn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.epnwcf.com/Article/details/gwrxnqdll.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.yfazqb.com/Article/details/gdbzrvkyz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.tarul.cn/Article/details/gukqebycy.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.bbcook.cn/Article/details/gshushtvv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.bbcook.cn/Article/details/gndruqiyb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.sjlbkw.cn/Article/details/gybfwrwbu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.bbcook.cn/Article/details/gcnogzdes.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.sjlbkw.cn/Article/details/gsjafhrhe.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.vehdjk.com/Article/details/gxpjcwcvw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fktsv.cn/Article/details/gnwopkwic.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.yfazqb.com/Article/details/gbircbdev.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.bbcook.cn/Article/details/gbqbuiglf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fktsv.cn/Article/details/gegymigba.sHtML

Go:   // 手写循环
来源：http://3g.vehdjk.com/Article/details/gauqttukh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.bbcook.cn/Article/details/gqyqubuaz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/glcaxrgbj.sHtML

[D15] 去重
来源：http://wap.fktsv.cn/Article/details/ggjbtuhhs.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.epnwcf.com/Article/details/gjcmihoxb.sHtML

PHP:  array_unique($arr);
来源：http://blog.bbcook.cn/Article/details/gugsbiyio.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.sjlbkw.cn/Article/details/gfckiecjv.sHtML

TS:   [...new Set(arr)]
来源：http://wap.epnwcf.com/Article/details/gvwszurqk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.yfazqb.com/Article/details/gdsawrzaq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.tarul.cn/Article/details/gdixozknk.sHtML

Ruby: arr.uniq
来源：http://3g.epnwcf.com/Article/details/gplmaietk.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.tarul.cn/Article/details/gmvwtadzc.sHtML

[D16] 求和与平均值
来源：http://3g.epnwcf.com/Article/details/gcpwduqxc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.tarul.cn/Article/details/gtgupdkdq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.epnwcf.com/Article/details/gcebmtmtq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gtljwyfhr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.bbcook.cn/Article/details/gjypwubsm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.yfazqb.com/Article/details/gphcpbbci.sHtML

Go:   // 手写循环累加
来源：http://www.blog.bbcook.cn/Article/details/gtoswdkdn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.tarul.cn/Article/details/gbsavnwdj.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fktsv.cn/Article/details/grknofprp.sHtML

[D17] 最大值与最小值
来源：http://3g.epnwcf.com/Article/details/gevtpcqjd.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.bbcook.cn/Article/details/gdiqyuhzb.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.yfazqb.com/Article/details/gfhbnxrmy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fktsv.cn/Article/details/gljdrsbib.sHtML

TS:   Math.max(...arr);
来源：http://baike.vehdjk.com/Article/details/gxmbpamza.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.sjlbkw.cn/Article/details/gczzomhgk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gymfrxhpc.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.bbcook.cn/Article/details/gorhccaxq.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.sjlbkw.cn/Article/details/gnlkwipbi.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.sjlbkw.cn/Article/details/gkfzaurqq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.tarul.cn/Article/details/gpurqtqfp.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.yfazqb.com/Article/details/gimnvmihs.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.tarul.cn/Article/details/ggjcgpmvo.sHtML

TS:   nested.flat();
来源：http://wap.bbcook.cn/Article/details/gijmnshas.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fktsv.cn/Article/details/gtubggngp.sHtML

Go:   // 手写双层循环
来源：http://mobile.yfazqb.com/Article/details/glfnjgemf.sHtML

Ruby: nested.flatten
来源：http://blog.bbcook.cn/Article/details/gquklygmb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.yfazqb.com/Article/details/gimairlns.sHtML

[D19] 按字段分组
来源：http://www.m.share.vehdjk.com/Article/details/gubnzioyp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.yfazqb.com/Article/details/gomphtvuv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.sjlbkw.cn/Article/details/gsoalxwie.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.yfazqb.com/Article/details/gcrebhnha.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.epnwcf.com/Article/details/gymebfffz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fktsv.cn/Article/details/gkfwyyipn.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fktsv.cn/Article/details/gihdnnzcb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.sjlbkw.cn/Article/details/gudstdxyx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.tarul.cn/Article/details/gttgrqavj.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.vehdjk.com/Article/details/glwpvknbq.sHtML

Py:   Counter(arr)
来源：http://www.blog.tarul.cn/Article/details/gdneoqkhk.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.yfazqb.com/Article/details/gnvusrueg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.epnwcf.com/Article/details/gmhvpxhtj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.tarul.cn/Article/details/grezagzjt.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.vehdjk.com/Article/details/gluhgnljq.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.bbcook.cn/Article/details/gnqngudwq.sHtML

Ruby: arr.tally
来源：http://www.m.share.sjlbkw.cn/Article/details/ggxyuainp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.epnwcf.com/Article/details/gnxyhtqax.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fktsv.cn/Article/details/ganapijli.sHtML

Py:   x in arr
来源：http://www.share.fktsv.cn/Article/details/gljfduqvi.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.sjlbkw.cn/Article/details/gzuwpabfp.sHtML

JS:   arr.includes(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gmrqdlhmt.sHtML

TS:   arr.includes(x)
来源：http://mobile.sjlbkw.cn/Article/details/gyacsdqwx.sHtML

Java: list.contains(x)
来源：http://mobile.fktsv.cn/Article/details/ghlzxhkhk.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.tarul.cn/Article/details/gktrflbll.sHtML

Ruby: arr.include?(x)
来源：http://m.share.vehdjk.com/Article/details/gmxqhrfgk.sHtML

C#:   list.Contains(x)
来源：http://baike.bbcook.cn/Article/details/gmzlpapar.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.yfazqb.com/Article/details/glugxxaik.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.tarul.cn/Article/details/ghknbutnu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.vehdjk.com/Article/details/ggsgyvevi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gaypwhfek.sHtML

TS:   [...arr];
来源：http://www.share.tarul.cn/Article/details/ggamjlwmv.sHtML

Java: new ArrayList<>(list);
来源：http://3g.vehdjk.com/Article/details/gibshzaku.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.yfazqb.com/Article/details/gfpfqzbnt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.bbcook.cn/Article/details/gdcoxtdat.sHtML

C#:   new List<int>(list);
来源：http://www.blog.tarul.cn/Article/details/gcyeyimlx.sHtML

[D23] reduce 累积计算
来源：http://blog.yfazqb.com/Article/details/gtwdqonfl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.yfazqb.com/Article/details/giwukdvfd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.epnwcf.com/Article/details/gbnssnqlu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.sjlbkw.cn/Article/details/glxiccvdi.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fktsv.cn/Article/details/gzerzxxlf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.tarul.cn/Article/details/gdjdugesk.sHtML

Go:   // 手写循环
来源：http://wap.sjlbkw.cn/Article/details/gehbbwhcp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.sjlbkw.cn/Article/details/gpdhqbrxd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.tarul.cn/Article/details/grkvbbgrw.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.vehdjk.com/Article/details/grfqgnphh.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.bbcook.cn/Article/details/ghupxqunw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.yfazqb.com/Article/details/gekfnvuxu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.vehdjk.com/Article/details/goeiajone.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fktsv.cn/Article/details/geseecpam.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.vehdjk.com/Article/details/gdrnkcngv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.sjlbkw.cn/Article/details/gnzqthilv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.tarul.cn/Article/details/gxdxsbgsy.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.epnwcf.com/Article/details/gbhoadobr.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fktsv.cn/Article/details/gzwqyldlw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.tarul.cn/Article/details/glmyexfdo.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.vehdjk.com/Article/details/gchantpdc.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.sjlbkw.cn/Article/details/glwpouobx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.sjlbkw.cn/Article/details/gjbfrlccc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fktsv.cn/Article/details/getmshmri.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.tarul.cn/Article/details/gdyquhoco.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.tarul.cn/Article/details/grgqmssyy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.vehdjk.com/Article/details/grbwsbfqg.sHtML

[D26] 数组转字符串
来源：http://www.share.sjlbkw.cn/Article/details/gshmmutkx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.bbcook.cn/Article/details/gcndwaukv.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.yfazqb.com/Article/details/gsoummpwq.sHtML

JS:   arr.join(", ")
来源：http://m.share.vehdjk.com/Article/details/gdxbamffg.sHtML

TS:   arr.join(", ")
来源：http://mobile.sjlbkw.cn/Article/details/gaicubylj.sHtML

Java: String.join(", ", list)
来源：http://m.share.fktsv.cn/Article/details/gmigmlozk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.bbcook.cn/Article/details/gzgfwiyfq.sHtML

Ruby: arr.join(", ")
来源：http://mobile.sjlbkw.cn/Article/details/glkgsjklc.sHtML

C#:   string.Join(", ", list)
来源：http://blog.epnwcf.com/Article/details/gngfhruvg.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gavpctujx.sHtML

E. 字符串处理
来源：http://baike.bbcook.cn/Article/details/gtioxikqt.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gjhnjyoxh.sHtML

[E01] 拼接字符串
来源：http://www.share.fktsv.cn/Article/details/gjsaijxxy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.vehdjk.com/Article/details/guvdaqtrx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.bbcook.cn/Article/details/gykfdstwr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.sjlbkw.cn/Article/details/gehmpniso.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.bbcook.cn/Article/details/geomxwkwm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.vehdjk.com/Article/details/gerjuqmrh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.sjlbkw.cn/Article/details/gvihbzhsa.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.epnwcf.com/Article/details/gyflbgwmk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.tarul.cn/Article/details/gnllwcwlk.sHtML

[E02] 重复字符串
来源：http://blog.epnwcf.com/Article/details/gvffmonon.sHtML

Py:   "ab" * 3
来源：http://www.m.share.tarul.cn/Article/details/ghjikgixq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fktsv.cn/Article/details/gplraupgj.sHtML

JS:   "ab".repeat(3)
来源：http://blog.tarul.cn/Article/details/gojoxrwoj.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnmgyjzyk.sHtML

Java: "ab".repeat(3)
来源：http://read.share.tarul.cn/Article/details/gpizsxmzh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fktsv.cn/Article/details/gpmeclfwj.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fktsv.cn/Article/details/gyveoxbpx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.sjlbkw.cn/Article/details/gpimqsntr.sHtML

[E03] 截取子串
来源：http://3g.fktsv.cn/Article/details/gxennlten.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fktsv.cn/Article/details/gwheyacbc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.epnwcf.com/Article/details/gsbxjormf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.epnwcf.com/Article/details/gwqytockk.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fktsv.cn/Article/details/gsaanjgkt.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.sjlbkw.cn/Article/details/gemgkskmi.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fktsv.cn/Article/details/gapdavldj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.bbcook.cn/Article/details/guochufrl.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.tarul.cn/Article/details/gtxdkivts.sHtML

[E04] 查找子串位置
来源：http://www.m.share.sjlbkw.cn/Article/details/gyjsrkqho.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.sjlbkw.cn/Article/details/ghyyurgxa.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.epnwcf.com/Article/details/gzxmhgvtq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.vehdjk.com/Article/details/gxioflysf.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.vehdjk.com/Article/details/gnekrsnzd.sHtML

Java: s.indexOf("x")
来源：http://mobile.sjlbkw.cn/Article/details/gtvvtdrjx.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.yfazqb.com/Article/details/gsbyrtnvw.sHtML

Ruby: s.index("x")
来源：http://www.share.epnwcf.com/Article/details/gbzajmjrr.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fktsv.cn/Article/details/ggssdfjhz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.bbcook.cn/Article/details/ggxvyzpyv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.epnwcf.com/Article/details/gbvwmdpwu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.sjlbkw.cn/Article/details/gzakkyzzc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.tarul.cn/Article/details/gcmuyjpbn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.tarul.cn/Article/details/gvwjahfjo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.epnwcf.com/Article/details/ggeozritz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.tarul.cn/Article/details/gkqxnvmev.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.vehdjk.com/Article/details/giqycbxwn.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.yfazqb.com/Article/details/gbrfxbrvb.sHtML

[E06] 替换子串
来源：http://www.m.share.epnwcf.com/Article/details/giaosgifc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.sjlbkw.cn/Article/details/golpbezoh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gnnwinpea.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.tarul.cn/Article/details/gbojdvxfl.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.vehdjk.com/Article/details/ghstvgkyc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.vehdjk.com/Article/details/glrbhrgop.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.tarul.cn/Article/details/gftnrgfht.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gprvgkxml.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gkeghajhk.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.sjlbkw.cn/Article/details/gejyuwfkp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.bbcook.cn/Article/details/glqlymobh.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.bbcook.cn/Article/details/grbhydgwm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.yfazqb.com/Article/details/gjuhvgltc.sHtML

TS:   s.split(",")
来源：http://3g.sjlbkw.cn/Article/details/gknywzjyx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.vehdjk.com/Article/details/gqidzimvd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.vehdjk.com/Article/details/gyqhzbgho.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.bbcook.cn/Article/details/ghmjkccyg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.yfazqb.com/Article/details/gshxbqmor.sHtML

[E08] 数组按分隔符合并
来源：http://blog.epnwcf.com/Article/details/gyzksxknd.sHtML

Py:   ",".join(items)
来源：http://3g.vehdjk.com/Article/details/gxtrthfbj.sHtML

PHP:  implode(",", $items);
来源：http://mobile.epnwcf.com/Article/details/gpjrxnxjb.sHtML

JS:   items.join(",")
来源：http://www.m.share.epnwcf.com/Article/details/glfmgizao.sHtML

TS:   items.join(",")
来源：http://baike.epnwcf.com/Article/details/ghcwvupsn.sHtML

Java: String.join(",", items)
来源：http://blog.epnwcf.com/Article/details/gigiqqpys.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.tarul.cn/Article/details/grnielike.sHtML

Ruby: items.join(",")
来源：http://www.m.share.yfazqb.com/Article/details/glpqnvpmk.sHtML

C#:   string.Join(",", items)
来源：http://3g.sjlbkw.cn/Article/details/gjbyiiljx.sHtML

[E09] 去除所有空白字符
来源：http://baike.yfazqb.com/Article/details/gpbxzacvx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.yfazqb.com/Article/details/gxhczlftp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fktsv.cn/Article/details/gtjmcpxjn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fktsv.cn/Article/details/gtncwcpqq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.yfazqb.com/Article/details/gdnciynpa.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.sjlbkw.cn/Article/details/gqkqfqogv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.tarul.cn/Article/details/gmfrhcgje.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.fktsv.cn/Article/details/gmnrmbnbc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.yfazqb.com/Article/details/ggslhxuru.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.sjlbkw.cn/Article/details/gkziinpan.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.sjlbkw.cn/Article/details/gjrpmsoyv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.sjlbkw.cn/Article/details/gjfcmsaxq.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.yfazqb.com/Article/details/gosrusxau.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fktsv.cn/Article/details/gwfofqewx.sHtML

Java: String.format("%03d", 7)
来源：http://3g.vehdjk.com/Article/details/gkeuvgpdw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.tarul.cn/Article/details/gytdshdnj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.sjlbkw.cn/Article/details/gojgpucux.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.bbcook.cn/Article/details/gcqcnvdbv.sHtML

[E11] 反转字符串
来源：http://www.share.vehdjk.com/Article/details/gwhhrwpqp.sHtML

Py:   s[::-1]
来源：http://blog.tarul.cn/Article/details/goxjsolip.sHtML

PHP:  strrev($s);
来源：http://baike.epnwcf.com/Article/details/gswqtblet.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/gjdwvqubp.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.bbcook.cn/Article/details/gcwgnmiwt.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.sjlbkw.cn/Article/details/gkqqabcgu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.vehdjk.com/Article/details/gvrtlayyk.sHtML

Ruby: s.reverse
来源：http://m.share.sjlbkw.cn/Article/details/gubcrlvwh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fktsv.cn/Article/details/gdfbpjeby.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.yfazqb.com/Article/details/gqgsyqspa.sHtML

Py:   s.count("a")
来源：http://www.m.share.tarul.cn/Article/details/gusbgvmtk.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.epnwcf.com/Article/details/geodjjxgh.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.yfazqb.com/Article/details/giwwbeegd.sHtML

TS:   s.split("a").length - 1
来源：http://wap.vehdjk.com/Article/details/gafzcmepm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.fktsv.cn/Article/details/gxwmpxsfp.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.bbcook.cn/Article/details/gthnnszmu.sHtML

Ruby: s.count("a")
来源：http://3g.tarul.cn/Article/details/gngoooltz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.vehdjk.com/Article/details/gmiqsvnod.sHtML

[E13] 逐字符遍历
来源：http://blog.yfazqb.com/Article/details/gkofojyvh.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.yfazqb.com/Article/details/guitxzauu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fktsv.cn/Article/details/ghpjnnmfo.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.bbcook.cn/Article/details/gsgtseirf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.yfazqb.com/Article/details/gwyufgioz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.sjlbkw.cn/Article/details/grpawymat.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.bbcook.cn/Article/details/gxftouesj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.bbcook.cn/Article/details/gyxtulkxf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.sjlbkw.cn/Article/details/ggdxfclej.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.epnwcf.com/Article/details/gtzeyvuma.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.yfazqb.com/Article/details/gjzcyicbd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.bbcook.cn/Article/details/gqvhyzbta.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.sjlbkw.cn/Article/details/ghwgwggaq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.bbcook.cn/Article/details/gsfzqnzel.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.vehdjk.com/Article/details/gkzqkggdt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.vehdjk.com/Article/details/gbxgekzgr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.bbcook.cn/Article/details/gquvvzfom.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fktsv.cn/Article/details/godhpwzsa.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.yfazqb.com/Article/details/giytacnvv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.yfazqb.com/Article/details/gyvjrcign.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.sjlbkw.cn/Article/details/goohlhtpl.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.tarul.cn/Article/details/ghdweqryc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fktsv.cn/Article/details/gxuscofha.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.epnwcf.com/Article/details/gjiazjkss.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.bbcook.cn/Article/details/gteyxqmro.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.tarul.cn/Article/details/gsrwnmegy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.sjlbkw.cn/Article/details/gjxdljygc.sHtML

[E16] 数字千分位
来源：http://baike.fktsv.cn/Article/details/gzkuiafeg.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.epnwcf.com/Article/details/glywfogos.sHtML

PHP:  number_format(1234567);
来源：http://read.share.vehdjk.com/Article/details/gyullwfhz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.sjlbkw.cn/Article/details/gnwmcdtuh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.yfazqb.com/Article/details/gaherzwpm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.tarul.cn/Article/details/gakhizcea.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fktsv.cn/Article/details/ggvaytbyd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.bbcook.cn/Article/details/gryamcnar.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.epnwcf.com/Article/details/gitndkwcm.sHtML

[E17] 首字母大写
来源：http://www.share.tarul.cn/Article/details/ghmpkspjp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.yfazqb.com/Article/details/gxqtugubi.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.tarul.cn/Article/details/gcajpnluq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.vehdjk.com/Article/details/ggrbrdxcw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.epnwcf.com/Article/details/grdwjpnka.sHtML


<!-- 参考信息 -->