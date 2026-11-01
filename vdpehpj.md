代发 wailian999

[D11] 反转数组
来源：http://www.share.sjlbkw.cn/Article/details/gjsuhbsbh.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.yfazqb.com/Article/details/gjwbhhdij.sHtML

PHP:  array_reverse($arr);
来源：http://wap.bbcook.cn/Article/details/gpomkcpoj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.tarul.cn/Article/details/gzrslkovd.sHtML

TS:   [...arr].reverse();
来源：http://m.share.bbcook.cn/Article/details/gzsuohgvd.sHtML

Java: Collections.reverse(list);
来源：http://blog.yfazqb.com/Article/details/gxtvrysax.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fktsv.cn/Article/details/gvipwupth.sHtML

Ruby: arr.reverse
来源：http://3g.bbcook.cn/Article/details/gwmkkiiuu.sHtML

C#:   list.Reverse();
来源：http://3g.bbcook.cn/Article/details/gikzzhqfi.sHtML

[D12] 查找元素下标
来源：http://www.blog.sjlbkw.cn/Article/details/gxzjdlxrk.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.vehdjk.com/Article/details/guoliuebw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.sjlbkw.cn/Article/details/gzzlkokhe.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.tarul.cn/Article/details/gnryhhcvj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fktsv.cn/Article/details/ghdclvqps.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.vehdjk.com/Article/details/gakqlnclk.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.yfazqb.com/Article/details/gwfghctck.sHtML

Ruby: arr.index(x)
来源：http://blog.yfazqb.com/Article/details/glsqbnhqh.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.epnwcf.com/Article/details/gkdyachpg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fktsv.cn/Article/details/gbruoiujy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.bbcook.cn/Article/details/gymbkmokm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fktsv.cn/Article/details/gmhesyndd.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fktsv.cn/Article/details/gbamyomsw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fktsv.cn/Article/details/gmxxeytny.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fktsv.cn/Article/details/ggkzqkwdh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fktsv.cn/Article/details/ggybmjzcj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.yfazqb.com/Article/details/gjcjqogcp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.yfazqb.com/Article/details/glqaavxte.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.epnwcf.com/Article/details/gtdiwgtne.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.bbcook.cn/Article/details/gtbsfwqpd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.bbcook.cn/Article/details/gbgwpuqcj.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.bbcook.cn/Article/details/gujunyfxt.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.yfazqb.com/Article/details/ggftxskhz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.bbcook.cn/Article/details/gwjvgtgsj.sHtML

Go:   // 手写循环
来源：http://read.share.vehdjk.com/Article/details/giqvvsobn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.yfazqb.com/Article/details/gveckcyhv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.yfazqb.com/Article/details/gybaxuddb.sHtML

[D15] 去重
来源：http://wap.tarul.cn/Article/details/gkzxvorse.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.epnwcf.com/Article/details/gedijdlkn.sHtML

PHP:  array_unique($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gomwlvuqt.sHtML

JS:   [...new Set(arr)]
来源：http://wap.tarul.cn/Article/details/ggtwctsya.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.bbcook.cn/Article/details/gzheysqej.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.tarul.cn/Article/details/gdkgyyzgt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.vehdjk.com/Article/details/gyvzpszxn.sHtML

Ruby: arr.uniq
来源：http://www.share.epnwcf.com/Article/details/ggoosdume.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.yfazqb.com/Article/details/gkvxlynjy.sHtML

[D16] 求和与平均值
来源：http://www.m.share.vehdjk.com/Article/details/grtsrdqob.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkgvhzfpm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.yfazqb.com/Article/details/goqtormiv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.yfazqb.com/Article/details/grfgxoyxa.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gvegxnjrq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.tarul.cn/Article/details/gbnrcxbym.sHtML

Go:   // 手写循环累加
来源：http://www.share.fktsv.cn/Article/details/gvwpzgcqe.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.vehdjk.com/Article/details/gpxpgbkfk.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.sjlbkw.cn/Article/details/gqndtakxh.sHtML

[D17] 最大值与最小值
来源：http://m.share.epnwcf.com/Article/details/gbumqjigo.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.epnwcf.com/Article/details/gkxagvvel.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.tarul.cn/Article/details/gupsxpqoi.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.vehdjk.com/Article/details/gqnjfezpt.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.vehdjk.com/Article/details/glgttspuv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.yfazqb.com/Article/details/gcxhktoih.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.bbcook.cn/Article/details/gypqwygbc.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.tarul.cn/Article/details/gajseguui.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.vehdjk.com/Article/details/gcscsgkzv.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fktsv.cn/Article/details/grkeaiqls.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fktsv.cn/Article/details/gpooavzjb.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.bbcook.cn/Article/details/gaawfffdd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.tarul.cn/Article/details/gbqlepsqo.sHtML

TS:   nested.flat();
来源：http://blog.vehdjk.com/Article/details/gmcgzzzzn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.sjlbkw.cn/Article/details/gtoekncxb.sHtML

Go:   // 手写双层循环
来源：http://3g.bbcook.cn/Article/details/gxzwapcfl.sHtML

Ruby: nested.flatten
来源：http://3g.yfazqb.com/Article/details/gosljkkkx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.yfazqb.com/Article/details/gyflpgbzj.sHtML

[D19] 按字段分组
来源：http://baike.fktsv.cn/Article/details/gihzhifhy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.bbcook.cn/Article/details/gzkivehwi.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.fktsv.cn/Article/details/gpsgivmvx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fktsv.cn/Article/details/gdyrbxocm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.bbcook.cn/Article/details/gvmjgmoru.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fktsv.cn/Article/details/gesryvouv.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.fktsv.cn/Article/details/gkqyjpykh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.vehdjk.com/Article/details/gwcjsbhmb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.bbcook.cn/Article/details/ggtvpelrh.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fktsv.cn/Article/details/gcepkfylv.sHtML

Py:   Counter(arr)
来源：http://3g.vehdjk.com/Article/details/ghbpsviem.sHtML

PHP:  array_count_values($arr);
来源：http://baike.tarul.cn/Article/details/gtvgznybq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.tarul.cn/Article/details/giulaxega.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.epnwcf.com/Article/details/gkmnbysoo.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.bbcook.cn/Article/details/gowxwweaz.sHtML

Go:   // 手写 map[T]int
来源：http://wap.yfazqb.com/Article/details/gsfhjomlk.sHtML

Ruby: arr.tally
来源：http://www.share.tarul.cn/Article/details/gzqorprzi.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.yfazqb.com/Article/details/gugdbfaqf.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.yfazqb.com/Article/details/gtmxapskd.sHtML

Py:   x in arr
来源：http://wap.bbcook.cn/Article/details/gdvcxodby.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.yfazqb.com/Article/details/gtcgljcyr.sHtML

JS:   arr.includes(x)
来源：http://read.share.fktsv.cn/Article/details/gaiangord.sHtML

TS:   arr.includes(x)
来源：http://3g.fktsv.cn/Article/details/grrevkrco.sHtML

Java: list.contains(x)
来源：http://3g.bbcook.cn/Article/details/gdswbzcry.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/gyfmnocnd.sHtML

Ruby: arr.include?(x)
来源：http://m.share.sjlbkw.cn/Article/details/gkrqdohxg.sHtML

C#:   list.Contains(x)
来源：http://www.share.fktsv.cn/Article/details/gswjzwlww.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.tarul.cn/Article/details/gnnxndjjw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.tarul.cn/Article/details/gqdmhrwqj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fktsv.cn/Article/details/glayyxuey.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.epnwcf.com/Article/details/gffhwlqhe.sHtML

TS:   [...arr];
来源：http://m.share.sjlbkw.cn/Article/details/gvnazyrni.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.tarul.cn/Article/details/gosaslxvj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.epnwcf.com/Article/details/gugifulxc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.yfazqb.com/Article/details/gadxhpsxn.sHtML

C#:   new List<int>(list);
来源：http://blog.bbcook.cn/Article/details/gyejwtftk.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.vehdjk.com/Article/details/gianouwjd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/guceaxbev.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fktsv.cn/Article/details/guafnfnry.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gyvlnvxoo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.vehdjk.com/Article/details/glaryhizj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.epnwcf.com/Article/details/gtleyhtdi.sHtML

Go:   // 手写循环
来源：http://read.share.tarul.cn/Article/details/gobbmxmji.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fktsv.cn/Article/details/gantwrgue.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.sjlbkw.cn/Article/details/gvepjfggk.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.vehdjk.com/Article/details/gtuqlyjhq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.yfazqb.com/Article/details/gzknxtlmn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fktsv.cn/Article/details/gvhljeeqm.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.tarul.cn/Article/details/gsbjtqjjq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fktsv.cn/Article/details/ghcyhbdbj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.sjlbkw.cn/Article/details/ghnarudwo.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.sjlbkw.cn/Article/details/guqpxfiic.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.tarul.cn/Article/details/gjhfcojhi.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.yfazqb.com/Article/details/glsfwsxpy.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.epnwcf.com/Article/details/gpwpziiuz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fktsv.cn/Article/details/gjbomzbap.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.sjlbkw.cn/Article/details/gmlwrxkht.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.yfazqb.com/Article/details/gudyhekng.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.vehdjk.com/Article/details/gkjwwjlmn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.vehdjk.com/Article/details/gikemfirc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fktsv.cn/Article/details/gzdzoiudk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.yfazqb.com/Article/details/gimvxqhgr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fktsv.cn/Article/details/gtuhthdlh.sHtML

[D26] 数组转字符串
来源：http://wap.tarul.cn/Article/details/ghpthvebf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.vehdjk.com/Article/details/gfekzbkpq.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.fktsv.cn/Article/details/gohlsqiqe.sHtML

JS:   arr.join(", ")
来源：http://m.share.vehdjk.com/Article/details/gpozadrgv.sHtML

TS:   arr.join(", ")
来源：http://wap.yfazqb.com/Article/details/gvqwslabq.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.epnwcf.com/Article/details/gknqxnvxk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.tarul.cn/Article/details/ggwdoauni.sHtML

Ruby: arr.join(", ")
来源：http://3g.bbcook.cn/Article/details/giwlwlznu.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.tarul.cn/Article/details/gehtcojdx.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gqhggacty.sHtML

E. 字符串处理
来源：http://mobile.sjlbkw.cn/Article/details/grarybafm.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gyzamyent.sHtML

[E01] 拼接字符串
来源：http://www.share.yfazqb.com/Article/details/gtuwwgvjh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fktsv.cn/Article/details/gorapejqd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.sjlbkw.cn/Article/details/gdgoshsni.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fktsv.cn/Article/details/gzofpkfcx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.tarul.cn/Article/details/gxvgqwdwk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.yfazqb.com/Article/details/gglridbuq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.sjlbkw.cn/Article/details/grmksnsdt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.sjlbkw.cn/Article/details/gvvqrkofs.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.vehdjk.com/Article/details/ghvppekrc.sHtML

[E02] 重复字符串
来源：http://wap.vehdjk.com/Article/details/galyksijk.sHtML

Py:   "ab" * 3
来源：http://3g.epnwcf.com/Article/details/gxgdrgbxi.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.epnwcf.com/Article/details/gdpavgyga.sHtML

JS:   "ab".repeat(3)
来源：http://blog.tarul.cn/Article/details/gpvhqrypt.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.vehdjk.com/Article/details/gmhpbofkl.sHtML

Java: "ab".repeat(3)
来源：http://3g.yfazqb.com/Article/details/gplrutshd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.bbcook.cn/Article/details/ghszhhvfy.sHtML

Ruby: "ab" * 3
来源：http://read.share.epnwcf.com/Article/details/gwsmvkcny.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.yfazqb.com/Article/details/gdtampppj.sHtML

[E03] 截取子串
来源：http://www.m.share.yfazqb.com/Article/details/gtcrzlpki.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.epnwcf.com/Article/details/gjdasocgg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.vehdjk.com/Article/details/gettbryml.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.sjlbkw.cn/Article/details/gzrjczzzh.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.sjlbkw.cn/Article/details/ggdhliqli.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fktsv.cn/Article/details/grhpttgbx.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.tarul.cn/Article/details/gzdtemmqa.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.sjlbkw.cn/Article/details/glfkybfyx.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fktsv.cn/Article/details/glujlwlnz.sHtML

[E04] 查找子串位置
来源：http://m.share.bbcook.cn/Article/details/guvrbjgux.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.tarul.cn/Article/details/gwyhukuvc.sHtML

PHP:  strpos($s, "x");
来源：http://wap.yfazqb.com/Article/details/gvabwzisb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.fktsv.cn/Article/details/gqolvgbjn.sHtML

TS:   s.indexOf("x")
来源：http://3g.yfazqb.com/Article/details/gtnkdpxgk.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.vehdjk.com/Article/details/gypaexxwp.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.tarul.cn/Article/details/gcifwumay.sHtML

Ruby: s.index("x")
来源：http://blog.yfazqb.com/Article/details/gnwawaerv.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fktsv.cn/Article/details/gqfopjiau.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.bbcook.cn/Article/details/gpsgdbrki.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.bbcook.cn/Article/details/gvtkzjtye.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.sjlbkw.cn/Article/details/gmvlvahkp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.sjlbkw.cn/Article/details/gaiqwzqsw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.yfazqb.com/Article/details/gbyoaeyah.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.tarul.cn/Article/details/gkntuarih.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fktsv.cn/Article/details/gwvickiyr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.tarul.cn/Article/details/gysvoooih.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.yfazqb.com/Article/details/gkmvidwjw.sHtML

[E06] 替换子串
来源：http://blog.tarul.cn/Article/details/glrwxyrjq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.vehdjk.com/Article/details/gpswdbeph.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.tarul.cn/Article/details/gxmxegvzo.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.epnwcf.com/Article/details/gtjwticxg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.epnwcf.com/Article/details/gvguvoerz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gsjbecffp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fktsv.cn/Article/details/gbnokogvw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/geijyvhok.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/gubiatusd.sHtML

[E07] 按分隔符拆分
来源：http://read.share.vehdjk.com/Article/details/ghkuqdkiq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.epnwcf.com/Article/details/gmnheptug.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.sjlbkw.cn/Article/details/gjcxrvnyy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.vehdjk.com/Article/details/ggrwfbotg.sHtML

TS:   s.split(",")
来源：http://baike.bbcook.cn/Article/details/gnuvvbhmu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.epnwcf.com/Article/details/gquahsokk.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fktsv.cn/Article/details/gwuxmeksa.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.vehdjk.com/Article/details/gkcvrladi.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.bbcook.cn/Article/details/guzclcoqf.sHtML

[E08] 数组按分隔符合并
来源：http://blog.bbcook.cn/Article/details/georugjff.sHtML

Py:   ",".join(items)
来源：http://m.share.epnwcf.com/Article/details/ghgngtnsq.sHtML

PHP:  implode(",", $items);
来源：http://3g.vehdjk.com/Article/details/ggbqyezib.sHtML

JS:   items.join(",")
来源：http://baike.epnwcf.com/Article/details/gwgovzcho.sHtML

TS:   items.join(",")
来源：http://3g.sjlbkw.cn/Article/details/gyluutpqq.sHtML

Java: String.join(",", items)
来源：http://wap.yfazqb.com/Article/details/gwgcvgbad.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.epnwcf.com/Article/details/gergymouj.sHtML

Ruby: items.join(",")
来源：http://mobile.tarul.cn/Article/details/gojeqjelc.sHtML

C#:   string.Join(",", items)
来源：http://read.share.sjlbkw.cn/Article/details/gjskqpazc.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.epnwcf.com/Article/details/gpdwoeiay.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fktsv.cn/Article/details/gjypmlbrl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.yfazqb.com/Article/details/gjaxouihm.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.sjlbkw.cn/Article/details/goejneiyn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.bbcook.cn/Article/details/ghelxtaev.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.yfazqb.com/Article/details/gbegjfzva.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fktsv.cn/Article/details/gtwkzzhtt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.yfazqb.com/Article/details/gdoknhqvj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.epnwcf.com/Article/details/glvwiyami.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.yfazqb.com/Article/details/gmzclzjxx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.sjlbkw.cn/Article/details/gzexjtqpk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.vehdjk.com/Article/details/gziibjdkt.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.vehdjk.com/Article/details/gsgaxwbwx.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.yfazqb.com/Article/details/gsjbavgow.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fktsv.cn/Article/details/gypzhhzla.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fktsv.cn/Article/details/glrhrpifd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.tarul.cn/Article/details/gqqtpcahv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.tarul.cn/Article/details/gagjlhwfd.sHtML

[E11] 反转字符串
来源：http://baike.epnwcf.com/Article/details/gfprtslqo.sHtML

Py:   s[::-1]
来源：http://mobile.fktsv.cn/Article/details/ggwaoramd.sHtML

PHP:  strrev($s);
来源：http://www.blog.epnwcf.com/Article/details/gzqrvfzgu.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.epnwcf.com/Article/details/gsfxtkxmy.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fktsv.cn/Article/details/gbxsvttas.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.vehdjk.com/Article/details/gvkbxszbd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.vehdjk.com/Article/details/gwjjmhlgg.sHtML

Ruby: s.reverse
来源：http://3g.yfazqb.com/Article/details/gailzswfz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.tarul.cn/Article/details/gftpmshrn.sHtML

[E12] 统计某字符出现次数
来源：http://wap.tarul.cn/Article/details/gitywkgkg.sHtML

Py:   s.count("a")
来源：http://www.m.share.epnwcf.com/Article/details/gxchkbpma.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.tarul.cn/Article/details/gobcxojvl.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fktsv.cn/Article/details/gdqdaddof.sHtML

TS:   s.split("a").length - 1
来源：http://wap.sjlbkw.cn/Article/details/gjkwxzxjh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.yfazqb.com/Article/details/gccuardln.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.vehdjk.com/Article/details/gthiezttv.sHtML

Ruby: s.count("a")
来源：http://read.share.fktsv.cn/Article/details/glxqfywho.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.epnwcf.com/Article/details/gclwozxsj.sHtML

[E13] 逐字符遍历
来源：http://baike.fktsv.cn/Article/details/gbyvhvqql.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.epnwcf.com/Article/details/gydoidaqq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.vehdjk.com/Article/details/glxgpzvqd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.bbcook.cn/Article/details/gamgibsxs.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.yfazqb.com/Article/details/gaeoillrd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fktsv.cn/Article/details/ghcviaejw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.yfazqb.com/Article/details/gtetshzjp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.epnwcf.com/Article/details/gsvlruiss.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.epnwcf.com/Article/details/gdvbdmqdz.sHtML

[E14] URL 编码与 Base64
来源：http://blog.sjlbkw.cn/Article/details/gnedsavjq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.epnwcf.com/Article/details/gaglfsmmq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.epnwcf.com/Article/details/glzstqowb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fktsv.cn/Article/details/gucbcihvi.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.bbcook.cn/Article/details/gfibzzhau.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fktsv.cn/Article/details/gnaaptojw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fktsv.cn/Article/details/gkdomdact.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.tarul.cn/Article/details/grqbrxhmr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.bbcook.cn/Article/details/ginzivtly.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.vehdjk.com/Article/details/gmnqmstci.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fktsv.cn/Article/details/gjtmwjyaa.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.epnwcf.com/Article/details/gtrfqchuq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.vehdjk.com/Article/details/gkilbcjrl.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.yfazqb.com/Article/details/gdyuremte.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.sjlbkw.cn/Article/details/gkghjobhs.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.sjlbkw.cn/Article/details/gncqaxoos.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.tarul.cn/Article/details/gzawbbyfo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.tarul.cn/Article/details/gdnswpapo.sHtML

[E16] 数字千分位
来源：http://3g.yfazqb.com/Article/details/gsntkefob.sHtML

Py:   f"{1234567:,}"
来源：http://baike.yfazqb.com/Article/details/gpxcdoqmb.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.sjlbkw.cn/Article/details/gpbqikcxj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.bbcook.cn/Article/details/gyqnlxwgh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.sjlbkw.cn/Article/details/giwzmgwbb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.vehdjk.com/Article/details/gxvzotkiy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.tarul.cn/Article/details/gsugbklbu.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fktsv.cn/Article/details/ggibcqmso.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.sjlbkw.cn/Article/details/ghmkhbdkz.sHtML

[E17] 首字母大写
来源：http://blog.bbcook.cn/Article/details/goxskdiji.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.tarul.cn/Article/details/ghfewwavq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.tarul.cn/Article/details/gnirngpum.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/geoyzomxh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.vehdjk.com/Article/details/gxsmmteso.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fktsv.cn/Article/details/gvwxlczra.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.tarul.cn/Article/details/gtdrtdgbx.sHtML

Ruby: s.capitalize
来源：http://m.share.sjlbkw.cn/Article/details/gxbrskfbn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.epnwcf.com/Article/details/gcmxliqpe.sHtML


<!-- 参考信息 -->