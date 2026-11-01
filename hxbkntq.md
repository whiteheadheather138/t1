代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.vehdjk.com/Article/details/gcahzhidi.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.vehdjk.com/Article/details/gwmmrkgqj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fktsv.cn/Article/details/gxdtsluzu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.tarul.cn/Article/details/gvctagijy.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.tarul.cn/Article/details/gmapneher.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.bbcook.cn/Article/details/gfrolmjoy.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gcgosqipy.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.epnwcf.com/Article/details/glsubqyqf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.epnwcf.com/Article/details/gpggogoxh.sHtML

Go:   // 手写循环
来源：http://www.blog.fktsv.cn/Article/details/gwwdfgboe.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.bbcook.cn/Article/details/gpbskykto.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.sjlbkw.cn/Article/details/gunllouut.sHtML

[D15] 去重
来源：http://blog.yfazqb.com/Article/details/gikpyvnxx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.yfazqb.com/Article/details/gimgmxure.sHtML

PHP:  array_unique($arr);
来源：http://baike.epnwcf.com/Article/details/gutudywsx.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fktsv.cn/Article/details/gsbvpquvc.sHtML

TS:   [...new Set(arr)]
来源：http://baike.yfazqb.com/Article/details/gikocifhr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.epnwcf.com/Article/details/gnjrdxdza.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.yfazqb.com/Article/details/grtqirfjh.sHtML

Ruby: arr.uniq
来源：http://read.share.bbcook.cn/Article/details/gvudueafo.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.sjlbkw.cn/Article/details/ghdnxrjpp.sHtML

[D16] 求和与平均值
来源：http://m.share.epnwcf.com/Article/details/gqxcifsmi.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.bbcook.cn/Article/details/gijvttyjm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.bbcook.cn/Article/details/gptclvcrt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.vehdjk.com/Article/details/gumzleetk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fktsv.cn/Article/details/gheojhuyz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.sjlbkw.cn/Article/details/grlwcanjy.sHtML

Go:   // 手写循环累加
来源：http://blog.tarul.cn/Article/details/gqielaics.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.yfazqb.com/Article/details/gwemmcnys.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.tarul.cn/Article/details/gygqarskf.sHtML

[D17] 最大值与最小值
来源：http://baike.epnwcf.com/Article/details/guafgfcyf.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.vehdjk.com/Article/details/gjglwnuqs.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fktsv.cn/Article/details/gkxabhpzb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.epnwcf.com/Article/details/givrnbgbj.sHtML

TS:   Math.max(...arr);
来源：http://m.share.vehdjk.com/Article/details/gdfhvjjbx.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.vehdjk.com/Article/details/gdcvhnfqm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fktsv.cn/Article/details/gnsnyfaly.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.yfazqb.com/Article/details/grosevksa.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.vehdjk.com/Article/details/geuqpxztx.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.sjlbkw.cn/Article/details/gusmacwcd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.bbcook.cn/Article/details/gmrmutafq.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.bbcook.cn/Article/details/gpevxpodr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.bbcook.cn/Article/details/gumrgohkx.sHtML

TS:   nested.flat();
来源：http://mobile.bbcook.cn/Article/details/gzqimtjfv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.yfazqb.com/Article/details/guihxseep.sHtML

Go:   // 手写双层循环
来源：http://read.share.sjlbkw.cn/Article/details/gykcdgzkn.sHtML

Ruby: nested.flatten
来源：http://3g.sjlbkw.cn/Article/details/gochuluve.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.epnwcf.com/Article/details/gejnywatn.sHtML

[D19] 按字段分组
来源：http://www.m.share.fktsv.cn/Article/details/gbwxdbgex.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fktsv.cn/Article/details/gswxxlrmf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.yfazqb.com/Article/details/guhxwfccl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.epnwcf.com/Article/details/gnumlwgfj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.bbcook.cn/Article/details/glsrlehik.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.bbcook.cn/Article/details/gzckfhaug.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.sjlbkw.cn/Article/details/ggkukkdll.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fktsv.cn/Article/details/gtmjvbnvq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fktsv.cn/Article/details/gyjfnlzid.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.tarul.cn/Article/details/gtsvrafsh.sHtML

Py:   Counter(arr)
来源：http://wap.yfazqb.com/Article/details/gxkbhcqwc.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.tarul.cn/Article/details/gjupnakwr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.vehdjk.com/Article/details/golorvxuz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.bbcook.cn/Article/details/gwxwbnica.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.yfazqb.com/Article/details/gqokltxxf.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.tarul.cn/Article/details/gwbnnnrlm.sHtML

Ruby: arr.tally
来源：http://blog.bbcook.cn/Article/details/gxnzybjua.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.yfazqb.com/Article/details/gxtbquxms.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.vehdjk.com/Article/details/gelqljtru.sHtML

Py:   x in arr
来源：http://3g.fktsv.cn/Article/details/ghsuqgynj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.sjlbkw.cn/Article/details/gwxcvlfdt.sHtML

JS:   arr.includes(x)
来源：http://wap.vehdjk.com/Article/details/gkcqoygxa.sHtML

TS:   arr.includes(x)
来源：http://baike.sjlbkw.cn/Article/details/gallvanli.sHtML

Java: list.contains(x)
来源：http://mobile.tarul.cn/Article/details/gzscqamyg.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.vehdjk.com/Article/details/gsszfjlkt.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fktsv.cn/Article/details/gtctlxzcy.sHtML

C#:   list.Contains(x)
来源：http://m.share.vehdjk.com/Article/details/gjqsfnlin.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.bbcook.cn/Article/details/gindgkjus.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.vehdjk.com/Article/details/gihqtfgpc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.yfazqb.com/Article/details/gbwkivbgi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.sjlbkw.cn/Article/details/gsgzqizbn.sHtML

TS:   [...arr];
来源：http://read.share.vehdjk.com/Article/details/gceaiifxo.sHtML

Java: new ArrayList<>(list);
来源：http://baike.vehdjk.com/Article/details/gjkfqxbvo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.tarul.cn/Article/details/gbnvynyvc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fktsv.cn/Article/details/ghetqthxo.sHtML

C#:   new List<int>(list);
来源：http://wap.vehdjk.com/Article/details/gukmuqxut.sHtML

[D23] reduce 累积计算
来源：http://wap.yfazqb.com/Article/details/gevwmsqxa.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.sjlbkw.cn/Article/details/gokcfvjvo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fktsv.cn/Article/details/gqtxifgme.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.vehdjk.com/Article/details/gxsuyqlhr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.epnwcf.com/Article/details/gwnzczcul.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.bbcook.cn/Article/details/gwdgsqbpz.sHtML

Go:   // 手写循环
来源：http://3g.fktsv.cn/Article/details/gyyfvtsks.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.bbcook.cn/Article/details/gvqxvqwkm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fktsv.cn/Article/details/gjkjmhgct.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.sjlbkw.cn/Article/details/gntvuosdp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.epnwcf.com/Article/details/gunsftvha.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.sjlbkw.cn/Article/details/guzqlyovi.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.vehdjk.com/Article/details/gghewriqi.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.sjlbkw.cn/Article/details/gefhvgtvf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.sjlbkw.cn/Article/details/geziobcjj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.bbcook.cn/Article/details/gjefbxtin.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.tarul.cn/Article/details/ghvqffmtq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.bbcook.cn/Article/details/ggqjwrzbi.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.bbcook.cn/Article/details/gjopuqqhp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.yfazqb.com/Article/details/gfxoxkoyu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.fktsv.cn/Article/details/gvlziijko.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.fktsv.cn/Article/details/gxrmzhihr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.vehdjk.com/Article/details/gavnpollk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.bbcook.cn/Article/details/gbqjdgzps.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.bbcook.cn/Article/details/gvtliaink.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.tarul.cn/Article/details/gqzzdpffr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.sjlbkw.cn/Article/details/gdpsrrnzy.sHtML

[D26] 数组转字符串
来源：http://3g.vehdjk.com/Article/details/gblogwuhe.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fktsv.cn/Article/details/gcfxtaiyv.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.vehdjk.com/Article/details/gvpnpwwsv.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.epnwcf.com/Article/details/gbycvrybk.sHtML

TS:   arr.join(", ")
来源：http://wap.yfazqb.com/Article/details/gatcrkmcm.sHtML

Java: String.join(", ", list)
来源：http://3g.tarul.cn/Article/details/gezrkeynr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.sjlbkw.cn/Article/details/gpkkyfizz.sHtML

Ruby: arr.join(", ")
来源：http://blog.bbcook.cn/Article/details/gvwrigppj.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.vehdjk.com/Article/details/gsvalflqq.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gsyuvuhbl.sHtML

E. 字符串处理
来源：http://mobile.epnwcf.com/Article/details/gpsunhgdf.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gdjzrqhps.sHtML

[E01] 拼接字符串
来源：http://mobile.fktsv.cn/Article/details/gnptbfjwm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.tarul.cn/Article/details/gmuckesmd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.vehdjk.com/Article/details/gsyggjdpn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.bbcook.cn/Article/details/gwlkplenk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.vehdjk.com/Article/details/gbmslafjx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.tarul.cn/Article/details/gcecydwxb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.sjlbkw.cn/Article/details/grnskhyrg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.epnwcf.com/Article/details/gspdqqslm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gvtzwnmqh.sHtML

[E02] 重复字符串
来源：http://www.m.share.fktsv.cn/Article/details/ggodngnmc.sHtML

Py:   "ab" * 3
来源：http://3g.sjlbkw.cn/Article/details/gljhhtnkg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.vehdjk.com/Article/details/gctmzlvkd.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjwirkzpp.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.epnwcf.com/Article/details/gwweuswhb.sHtML

Java: "ab".repeat(3)
来源：http://baike.yfazqb.com/Article/details/goqcotmxc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.vehdjk.com/Article/details/gzaydpzcs.sHtML

Ruby: "ab" * 3
来源：http://www.share.bbcook.cn/Article/details/gnwodhzeu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.tarul.cn/Article/details/ggqamvrxl.sHtML

[E03] 截取子串
来源：http://mobile.sjlbkw.cn/Article/details/gbqbkxlfi.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.bbcook.cn/Article/details/gfmoanpdz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.tarul.cn/Article/details/gtipzzlkq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.bbcook.cn/Article/details/ggvjamjxq.sHtML

TS:   s.slice(1, 4)
来源：http://wap.bbcook.cn/Article/details/gmfljkfax.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fktsv.cn/Article/details/gcrichyww.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.sjlbkw.cn/Article/details/ghvhzucjp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.epnwcf.com/Article/details/govatckhf.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.fktsv.cn/Article/details/ggzjjpgfe.sHtML

[E04] 查找子串位置
来源：http://www.share.yfazqb.com/Article/details/gjawcxjcl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.epnwcf.com/Article/details/gljydcgqn.sHtML

PHP:  strpos($s, "x");
来源：http://baike.yfazqb.com/Article/details/gybouggrw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.vehdjk.com/Article/details/gewtqhwtk.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.sjlbkw.cn/Article/details/gpzjdwlpx.sHtML

Java: s.indexOf("x")
来源：http://www.share.sjlbkw.cn/Article/details/gdwvmzutw.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.vehdjk.com/Article/details/gptzcvdka.sHtML

Ruby: s.index("x")
来源：http://mobile.vehdjk.com/Article/details/ghczfgpbk.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.bbcook.cn/Article/details/gktscbqdl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.bbcook.cn/Article/details/goaxefnlm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.fktsv.cn/Article/details/giirvucoz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.epnwcf.com/Article/details/gzyauxdsv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.bbcook.cn/Article/details/gcfxvuuvc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.yfazqb.com/Article/details/gphhqefle.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.tarul.cn/Article/details/glhwsgeln.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.sjlbkw.cn/Article/details/gjtyqvrjk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.bbcook.cn/Article/details/gbeyavnnu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.vehdjk.com/Article/details/geanukdzo.sHtML

[E06] 替换子串
来源：http://m.share.tarul.cn/Article/details/gbmblwuad.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.vehdjk.com/Article/details/gskviuhbr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.bbcook.cn/Article/details/gbtrljjvg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fktsv.cn/Article/details/gicshtkpp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/gpcbpnynh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/gylfmtlvp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.tarul.cn/Article/details/gekfndfxw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.tarul.cn/Article/details/ggndsmerz.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gmzoubcqm.sHtML

[E07] 按分隔符拆分
来源：http://www.share.tarul.cn/Article/details/gsngeofoi.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.sjlbkw.cn/Article/details/gvqdmheeb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fktsv.cn/Article/details/glzpzpgem.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.epnwcf.com/Article/details/gnkuponhn.sHtML

TS:   s.split(",")
来源：http://blog.fktsv.cn/Article/details/ggqwstvie.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fktsv.cn/Article/details/gyauddyql.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.epnwcf.com/Article/details/gigrootdo.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.epnwcf.com/Article/details/gmhewtaak.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.epnwcf.com/Article/details/gshlyzmac.sHtML

[E08] 数组按分隔符合并
来源：http://3g.tarul.cn/Article/details/gvkikcwnj.sHtML

Py:   ",".join(items)
来源：http://mobile.fktsv.cn/Article/details/ghdiytlph.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.yfazqb.com/Article/details/grmuombhx.sHtML

JS:   items.join(",")
来源：http://read.share.vehdjk.com/Article/details/gjkrqzbdg.sHtML

TS:   items.join(",")
来源：http://baike.sjlbkw.cn/Article/details/grjgtdaty.sHtML

Java: String.join(",", items)
来源：http://read.share.sjlbkw.cn/Article/details/gzmgxkamv.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.epnwcf.com/Article/details/ginmdspzh.sHtML

Ruby: items.join(",")
来源：http://baike.sjlbkw.cn/Article/details/gszrcrjnp.sHtML

C#:   string.Join(",", items)
来源：http://mobile.yfazqb.com/Article/details/gwmrtflid.sHtML

[E09] 去除所有空白字符
来源：http://mobile.bbcook.cn/Article/details/gkgtuvrwv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.bbcook.cn/Article/details/gwrzojucq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.yfazqb.com/Article/details/gmnxkdpej.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.bbcook.cn/Article/details/gxpluamet.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.epnwcf.com/Article/details/gdzvfnhxu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.sjlbkw.cn/Article/details/gofcuvtpt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.tarul.cn/Article/details/gtcdayepq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.tarul.cn/Article/details/gppzznpdj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.vehdjk.com/Article/details/gcegokaah.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.bbcook.cn/Article/details/gqsrtwxii.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fktsv.cn/Article/details/gnjqayvrf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.epnwcf.com/Article/details/gquolskab.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.bbcook.cn/Article/details/gxrvngunb.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.vehdjk.com/Article/details/gxqkglrdi.sHtML

Java: String.format("%03d", 7)
来源：http://3g.epnwcf.com/Article/details/gpaufyigs.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fktsv.cn/Article/details/gyfnumfbk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.epnwcf.com/Article/details/ghbewbjdu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fktsv.cn/Article/details/gjppgugjp.sHtML

[E11] 反转字符串
来源：http://3g.tarul.cn/Article/details/guoahjwui.sHtML

Py:   s[::-1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gxfdnxsot.sHtML

PHP:  strrev($s);
来源：http://3g.fktsv.cn/Article/details/glqgysmvc.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.bbcook.cn/Article/details/gmtaghvxb.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.epnwcf.com/Article/details/gdeqewmvt.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.tarul.cn/Article/details/ggkubzokw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.epnwcf.com/Article/details/gsxkzlipj.sHtML

Ruby: s.reverse
来源：http://www.blog.vehdjk.com/Article/details/gfeunaelt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.bbcook.cn/Article/details/ghiwyfdmt.sHtML

[E12] 统计某字符出现次数
来源：http://wap.vehdjk.com/Article/details/gsyfrtxzb.sHtML

Py:   s.count("a")
来源：http://www.share.yfazqb.com/Article/details/gaeltyius.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.epnwcf.com/Article/details/gwlfbfqvf.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.vehdjk.com/Article/details/gfmcgidka.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.bbcook.cn/Article/details/ggsdzpudy.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.tarul.cn/Article/details/gflvoduaa.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.yfazqb.com/Article/details/ggpwabopy.sHtML

Ruby: s.count("a")
来源：http://baike.vehdjk.com/Article/details/gskqwtqrk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.tarul.cn/Article/details/gbosabcvf.sHtML

[E13] 逐字符遍历
来源：http://www.blog.epnwcf.com/Article/details/gqhretfvj.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.sjlbkw.cn/Article/details/gdsjrgnkv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.bbcook.cn/Article/details/gttnoixin.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fktsv.cn/Article/details/gvgiqsvaz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.bbcook.cn/Article/details/gnebfvcdu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.tarul.cn/Article/details/grjkbagdp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.sjlbkw.cn/Article/details/gwvnkshti.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.epnwcf.com/Article/details/gmrslwowy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gteqbjern.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.bbcook.cn/Article/details/gqaakvhro.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fktsv.cn/Article/details/gvseigpsj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fktsv.cn/Article/details/gmqvsawbx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.tarul.cn/Article/details/gulmmnaqw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fktsv.cn/Article/details/gzvuciihc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fktsv.cn/Article/details/gdiwopxqr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.sjlbkw.cn/Article/details/gjhqjiggu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fktsv.cn/Article/details/ghbfdillq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.yfazqb.com/Article/details/gyhtctdah.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.yfazqb.com/Article/details/gseujanpe.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.yfazqb.com/Article/details/gwgsaxmep.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.bbcook.cn/Article/details/guekbfinv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.vehdjk.com/Article/details/gzdnwocmq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.bbcook.cn/Article/details/glysvonuo.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fktsv.cn/Article/details/gelgutuht.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fktsv.cn/Article/details/gttxaucuq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.tarul.cn/Article/details/gqyjwpddq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fktsv.cn/Article/details/grxhqbczv.sHtML

[E16] 数字千分位
来源：http://3g.tarul.cn/Article/details/ghbqgxora.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.epnwcf.com/Article/details/gaapolbby.sHtML

PHP:  number_format(1234567);
来源：http://baike.vehdjk.com/Article/details/gjtsksjdx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fktsv.cn/Article/details/gdbhzeazp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.yfazqb.com/Article/details/gvixddtnt.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.vehdjk.com/Article/details/gkprsflcd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.bbcook.cn/Article/details/gfbbumedf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.tarul.cn/Article/details/gkuppenop.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.epnwcf.com/Article/details/gbwstjfbi.sHtML

[E17] 首字母大写
来源：http://www.share.epnwcf.com/Article/details/guvpxfwep.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.tarul.cn/Article/details/gpwfiebum.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fktsv.cn/Article/details/gyspoagsy.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.vehdjk.com/Article/details/guhcsbqtr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.vehdjk.com/Article/details/ghadzlzdy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.sjlbkw.cn/Article/details/gikjfstfu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fktsv.cn/Article/details/geftjbfni.sHtML

Ruby: s.capitalize
来源：http://read.share.yfazqb.com/Article/details/gkvcngakr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.tarul.cn/Article/details/gbqnzzisk.sHtML

[E18] 模板占位符替换
来源：http://blog.fktsv.cn/Article/details/gprnocfuk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.bbcook.cn/Article/details/gkkxanafh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.tarul.cn/Article/details/gnhqomqtl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.vehdjk.com/Article/details/gaewfnsfa.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.sjlbkw.cn/Article/details/gwdvfgidf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.tarul.cn/Article/details/gsrwjbkwn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.tarul.cn/Article/details/ggxwpwoxl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.bbcook.cn/Article/details/gloqdszwf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.fktsv.cn/Article/details/gxcryvhod.sHtML

[E19] 多行文本按行拆分
来源：http://baike.epnwcf.com/Article/details/gqbinylzr.sHtML

Py:   s.splitlines()
来源：http://baike.fktsv.cn/Article/details/gmemsmfdy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.vehdjk.com/Article/details/gtywkmrrk.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.vehdjk.com/Article/details/gziqhlthw.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.bbcook.cn/Article/details/gccqhdjwt.sHtML

Java: s.lines().toList()
来源：http://m.share.bbcook.cn/Article/details/geayckgjx.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.tarul.cn/Article/details/gunpbawju.sHtML

Ruby: s.lines
来源：http://mobile.yfazqb.com/Article/details/gcmxjtsod.sHtML

C#:   s.Split('\n')
来源：http://m.share.fktsv.cn/Article/details/gzcjfvnsf.sHtML

[E20] 判断字符串是否为空
来源：http://wap.vehdjk.com/Article/details/ghduslnup.sHtML

Py:   if not s:
来源：http://www.share.tarul.cn/Article/details/gnughzvew.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.sjlbkw.cn/Article/details/gprjunpol.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.epnwcf.com/Article/details/gaeuazxrm.sHtML

TS:   if (s === "") {}
来源：http://baike.yfazqb.com/Article/details/glknkuzjl.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.epnwcf.com/Article/details/gvlqwofbg.sHtML


<!-- 参考信息 -->