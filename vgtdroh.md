代发 wailian999

Ruby: arr.index(x)
来源：http://baike.yfazqb.com/Article/details/gcheidxbh.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.vehdjk.com/Article/details/gkgfejsjd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.epnwcf.com/Article/details/gbvfaifwq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fktsv.cn/Article/details/ghabznkib.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.sjlbkw.cn/Article/details/gawtqtsrb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.vehdjk.com/Article/details/gsrzgptan.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.epnwcf.com/Article/details/gnnkfqrov.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.epnwcf.com/Article/details/gvffkjpvi.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.vehdjk.com/Article/details/gcvstspjp.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.yfazqb.com/Article/details/gnwdbivaa.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.yfazqb.com/Article/details/guwvbatgr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.yfazqb.com/Article/details/gtaqlzbtw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.tarul.cn/Article/details/gmwwdkxeo.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.tarul.cn/Article/details/gyisdrhhw.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.epnwcf.com/Article/details/gzerygkcd.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.bbcook.cn/Article/details/gktqxlmwk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.vehdjk.com/Article/details/gfcgswgkp.sHtML

Go:   // 手写循环
来源：http://baike.vehdjk.com/Article/details/gcvjwkubo.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.yfazqb.com/Article/details/gnppmkekd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.sjlbkw.cn/Article/details/gsdqvinhp.sHtML

[D15] 去重
来源：http://3g.yfazqb.com/Article/details/gkqlsswry.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.sjlbkw.cn/Article/details/gwcckbgtc.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gckkiixjx.sHtML

JS:   [...new Set(arr)]
来源：http://3g.epnwcf.com/Article/details/gaaugoeus.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.sjlbkw.cn/Article/details/gwmonpusg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.epnwcf.com/Article/details/gcyenqhtp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.epnwcf.com/Article/details/gpolzretg.sHtML

Ruby: arr.uniq
来源：http://wap.epnwcf.com/Article/details/gqdkbpzih.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.yfazqb.com/Article/details/golgyqdyx.sHtML

[D16] 求和与平均值
来源：http://blog.epnwcf.com/Article/details/gxncxkrah.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.fktsv.cn/Article/details/gwrzdrfvh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.tarul.cn/Article/details/gwxmrsszc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.epnwcf.com/Article/details/gopvhqpdl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.bbcook.cn/Article/details/gmhhnrvpq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.yfazqb.com/Article/details/gthbygtsd.sHtML

Go:   // 手写循环累加
来源：http://www.share.yfazqb.com/Article/details/gvwxzgdlh.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.vehdjk.com/Article/details/gwmvyktlr.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.tarul.cn/Article/details/gohtwdkbg.sHtML

[D17] 最大值与最小值
来源：http://wap.sjlbkw.cn/Article/details/gkvmoyugi.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.epnwcf.com/Article/details/godyzblvs.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.vehdjk.com/Article/details/guaqmfflc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.tarul.cn/Article/details/gdgqelwxk.sHtML

TS:   Math.max(...arr);
来源：http://read.share.vehdjk.com/Article/details/glmyfbovk.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.bbcook.cn/Article/details/gvhnstcef.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.epnwcf.com/Article/details/gzuyejmgf.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fktsv.cn/Article/details/gzvebgbbt.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.epnwcf.com/Article/details/gyzdwijqk.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.sjlbkw.cn/Article/details/gqwygfity.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.vehdjk.com/Article/details/gbgxbsgzm.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.bbcook.cn/Article/details/ghmgrkjkc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.tarul.cn/Article/details/gloppgoxl.sHtML

TS:   nested.flat();
来源：http://m.share.yfazqb.com/Article/details/glcnhpcfs.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.sjlbkw.cn/Article/details/gyggymtbk.sHtML

Go:   // 手写双层循环
来源：http://baike.epnwcf.com/Article/details/gesynfpqq.sHtML

Ruby: nested.flatten
来源：http://read.share.bbcook.cn/Article/details/gtarnkwqm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.sjlbkw.cn/Article/details/gmamrlcdi.sHtML

[D19] 按字段分组
来源：http://baike.bbcook.cn/Article/details/ghamclsiv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.tarul.cn/Article/details/gyjalmhbr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.vehdjk.com/Article/details/gxansvyos.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.sjlbkw.cn/Article/details/gquegbazv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fktsv.cn/Article/details/gszrstwnj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.tarul.cn/Article/details/gyqatpbwk.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.yfazqb.com/Article/details/gxaotnvcp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fktsv.cn/Article/details/gavfewscb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.tarul.cn/Article/details/gfsqsmwhf.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.bbcook.cn/Article/details/ggwkyqerv.sHtML

Py:   Counter(arr)
来源：http://wap.vehdjk.com/Article/details/gxfswsgfl.sHtML

PHP:  array_count_values($arr);
来源：http://wap.sjlbkw.cn/Article/details/geojnmyun.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.yfazqb.com/Article/details/gfkhqnruj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.bbcook.cn/Article/details/ggjawojrh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.yfazqb.com/Article/details/ganatjivd.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.bbcook.cn/Article/details/gyeglmwlq.sHtML

Ruby: arr.tally
来源：http://www.share.sjlbkw.cn/Article/details/glhaqsubl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.sjlbkw.cn/Article/details/gdcgkmrny.sHtML

[D21] 判断是否包含某元素
来源：http://baike.vehdjk.com/Article/details/gczvrgzfp.sHtML

Py:   x in arr
来源：http://read.share.fktsv.cn/Article/details/glytfdirn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.vehdjk.com/Article/details/gzyhhwofe.sHtML

JS:   arr.includes(x)
来源：http://3g.vehdjk.com/Article/details/gbcgfrjfi.sHtML

TS:   arr.includes(x)
来源：http://mobile.bbcook.cn/Article/details/ghpattouo.sHtML

Java: list.contains(x)
来源：http://baike.epnwcf.com/Article/details/gasvuyryk.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.vehdjk.com/Article/details/gzlwkwvkq.sHtML

Ruby: arr.include?(x)
来源：http://wap.yfazqb.com/Article/details/goatfwaod.sHtML

C#:   list.Contains(x)
来源：http://baike.epnwcf.com/Article/details/ganddkdva.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.yfazqb.com/Article/details/glbzdtstc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.tarul.cn/Article/details/gueosvidm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.tarul.cn/Article/details/gchdjmcxd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fktsv.cn/Article/details/gfixfdhdp.sHtML

TS:   [...arr];
来源：http://www.m.share.yfazqb.com/Article/details/gguyuostv.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.bbcook.cn/Article/details/gbdqptsbs.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.tarul.cn/Article/details/gxrpmkoem.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.sjlbkw.cn/Article/details/gjgrzcgfj.sHtML

C#:   new List<int>(list);
来源：http://blog.tarul.cn/Article/details/gnxydxcmp.sHtML

[D23] reduce 累积计算
来源：http://mobile.sjlbkw.cn/Article/details/gmktkladx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.yfazqb.com/Article/details/gbfpsxizz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.sjlbkw.cn/Article/details/gazhcowzd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.sjlbkw.cn/Article/details/goquxqnpk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.tarul.cn/Article/details/gzikhnlgj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.epnwcf.com/Article/details/godhmcpfp.sHtML

Go:   // 手写循环
来源：http://read.share.yfazqb.com/Article/details/gbhyrpfmk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.yfazqb.com/Article/details/gepbqwylq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.vehdjk.com/Article/details/goggwoxsi.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.bbcook.cn/Article/details/gdbwpcbhk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.tarul.cn/Article/details/gmrhwktms.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fktsv.cn/Article/details/gfjwpqctr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.bbcook.cn/Article/details/gxqbpcunc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fktsv.cn/Article/details/gfwrhuhrv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.bbcook.cn/Article/details/gtkauuvxh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.tarul.cn/Article/details/gwtrdsrtm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.yfazqb.com/Article/details/gdgopkwxz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.tarul.cn/Article/details/gynsdzbgh.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fktsv.cn/Article/details/ggexueonb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.vehdjk.com/Article/details/gtcrhffpg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.yfazqb.com/Article/details/glwfagfec.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.fktsv.cn/Article/details/gewuszrcv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.epnwcf.com/Article/details/gxegmzyov.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.tarul.cn/Article/details/gafwkexdh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.sjlbkw.cn/Article/details/gxninlfxl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.epnwcf.com/Article/details/gytyslofs.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.tarul.cn/Article/details/gybzopeoe.sHtML

[D26] 数组转字符串
来源：http://blog.fktsv.cn/Article/details/ggszluayd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.tarul.cn/Article/details/gihsongyd.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.sjlbkw.cn/Article/details/gelhbjvwu.sHtML

JS:   arr.join(", ")
来源：http://www.share.yfazqb.com/Article/details/gsbzmywwd.sHtML

TS:   arr.join(", ")
来源：http://www.blog.tarul.cn/Article/details/glixektue.sHtML

Java: String.join(", ", list)
来源：http://blog.fktsv.cn/Article/details/ghkiagqbz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.vehdjk.com/Article/details/gwcxaevov.sHtML

Ruby: arr.join(", ")
来源：http://blog.vehdjk.com/Article/details/ghfzyxhuj.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.yfazqb.com/Article/details/ggbsniobe.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gbuychilc.sHtML

E. 字符串处理
来源：http://www.share.yfazqb.com/Article/details/gieaiybjq.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gihfcimgb.sHtML

[E01] 拼接字符串
来源：http://baike.tarul.cn/Article/details/gxfvvipjb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.tarul.cn/Article/details/gcrquolic.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.tarul.cn/Article/details/gpgdftcmg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.yfazqb.com/Article/details/gylblkqtw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fktsv.cn/Article/details/ggjklvwwf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.vehdjk.com/Article/details/gdbtbgvtu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.sjlbkw.cn/Article/details/gwblrfplg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.tarul.cn/Article/details/gzrzfditf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.tarul.cn/Article/details/giqqzgfyv.sHtML

[E02] 重复字符串
来源：http://www.blog.bbcook.cn/Article/details/gxscldupv.sHtML

Py:   "ab" * 3
来源：http://read.share.tarul.cn/Article/details/gaqmnctdf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fktsv.cn/Article/details/gkxzcqvun.sHtML

JS:   "ab".repeat(3)
来源：http://blog.tarul.cn/Article/details/goqyeobqm.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.tarul.cn/Article/details/gpnhaycnb.sHtML

Java: "ab".repeat(3)
来源：http://wap.fktsv.cn/Article/details/gggbrnikt.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.sjlbkw.cn/Article/details/gviqofamq.sHtML

Ruby: "ab" * 3
来源：http://baike.fktsv.cn/Article/details/glmzkqabw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.yfazqb.com/Article/details/gqionyirw.sHtML

[E03] 截取子串
来源：http://www.m.share.tarul.cn/Article/details/gafegccwo.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.yfazqb.com/Article/details/gpdcczgrr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.tarul.cn/Article/details/gjjixbzgo.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.yfazqb.com/Article/details/gxbfohcvj.sHtML

TS:   s.slice(1, 4)
来源：http://3g.bbcook.cn/Article/details/grleofzzw.sHtML

Java: s.substring(1, 4)
来源：http://www.share.sjlbkw.cn/Article/details/gprexgxdn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.epnwcf.com/Article/details/gnumvxbib.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fktsv.cn/Article/details/gqfdyswdm.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.yfazqb.com/Article/details/ghbpbwsaq.sHtML

[E04] 查找子串位置
来源：http://blog.sjlbkw.cn/Article/details/gumnkthmq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.sjlbkw.cn/Article/details/gbhurwccg.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fktsv.cn/Article/details/gyelwzfji.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.bbcook.cn/Article/details/geowabbvy.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.yfazqb.com/Article/details/gihxsgpna.sHtML

Java: s.indexOf("x")
来源：http://www.share.sjlbkw.cn/Article/details/gxpzoplhy.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.bbcook.cn/Article/details/gfioytlig.sHtML

Ruby: s.index("x")
来源：http://read.share.epnwcf.com/Article/details/gwudmqlaq.sHtML

C#:   s.IndexOf("x")
来源：http://wap.vehdjk.com/Article/details/georlxrvq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.tarul.cn/Article/details/ggnayfapx.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.tarul.cn/Article/details/ggtqkxaiw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fktsv.cn/Article/details/gstmtsmty.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fktsv.cn/Article/details/ggciyuduz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.tarul.cn/Article/details/gbvpouqiu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.vehdjk.com/Article/details/glocqfqdh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.bbcook.cn/Article/details/gcewipbjp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.sjlbkw.cn/Article/details/grakbdeku.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fktsv.cn/Article/details/gkmwunjop.sHtML

[E06] 替换子串
来源：http://3g.yfazqb.com/Article/details/guajouidt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.bbcook.cn/Article/details/gwpjltsqk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.vehdjk.com/Article/details/gbrperqkq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.tarul.cn/Article/details/gdrypwxtj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gyixcxndi.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.tarul.cn/Article/details/gguxzudmr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fktsv.cn/Article/details/gkltplflu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.vehdjk.com/Article/details/gnoxkeqxf.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gqszbjzfa.sHtML

[E07] 按分隔符拆分
来源：http://wap.tarul.cn/Article/details/gatkrczqr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.sjlbkw.cn/Article/details/gfbmlxodf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.sjlbkw.cn/Article/details/gcjpfsqqd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.vehdjk.com/Article/details/gfkvbkrlx.sHtML

TS:   s.split(",")
来源：http://blog.bbcook.cn/Article/details/gdutbnhku.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.yfazqb.com/Article/details/gofibkdms.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.fktsv.cn/Article/details/gxxsbxcqz.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.fktsv.cn/Article/details/glufwxjpr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fktsv.cn/Article/details/gppbjqyhn.sHtML

[E08] 数组按分隔符合并
来源：http://blog.sjlbkw.cn/Article/details/gkjrysoca.sHtML

Py:   ",".join(items)
来源：http://www.blog.tarul.cn/Article/details/giblbfzof.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fktsv.cn/Article/details/giwhxkoev.sHtML

JS:   items.join(",")
来源：http://www.m.share.epnwcf.com/Article/details/geetgfvmn.sHtML

TS:   items.join(",")
来源：http://www.blog.tarul.cn/Article/details/gjdhvvbmi.sHtML

Java: String.join(",", items)
来源：http://wap.bbcook.cn/Article/details/gauyznspu.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.bbcook.cn/Article/details/gcusvuapy.sHtML

Ruby: items.join(",")
来源：http://www.blog.yfazqb.com/Article/details/gplshekkb.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fktsv.cn/Article/details/gdvtfcnkn.sHtML

[E09] 去除所有空白字符
来源：http://www.share.bbcook.cn/Article/details/gmrxbrclp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.bbcook.cn/Article/details/gfnviltba.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.vehdjk.com/Article/details/gzqcszfpo.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.tarul.cn/Article/details/gorqqbzza.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.vehdjk.com/Article/details/gruxhjedv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.yfazqb.com/Article/details/gjscxkjrr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.bbcook.cn/Article/details/gxfpdvwzn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.vehdjk.com/Article/details/gwkuivqiu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.tarul.cn/Article/details/gpmnqffnz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.vehdjk.com/Article/details/gznlzyedy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.vehdjk.com/Article/details/gybknhbqp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.bbcook.cn/Article/details/gogssteav.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.bbcook.cn/Article/details/guvcuwgfw.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.yfazqb.com/Article/details/gqiplisaf.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.epnwcf.com/Article/details/gfavlwffd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.epnwcf.com/Article/details/gzmmsjqtw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.yfazqb.com/Article/details/gkyfogtdy.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fktsv.cn/Article/details/gwsqymrmf.sHtML

[E11] 反转字符串
来源：http://www.blog.vehdjk.com/Article/details/gpeiuklii.sHtML

Py:   s[::-1]
来源：http://wap.vehdjk.com/Article/details/glortinrr.sHtML

PHP:  strrev($s);
来源：http://3g.bbcook.cn/Article/details/gguarjqbf.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.tarul.cn/Article/details/gframvgkt.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.bbcook.cn/Article/details/gbkhmwfzd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.tarul.cn/Article/details/gybeytomg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.tarul.cn/Article/details/gjeyhbfhj.sHtML

Ruby: s.reverse
来源：http://mobile.yfazqb.com/Article/details/giwyhthki.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.epnwcf.com/Article/details/gphdalfpk.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fktsv.cn/Article/details/gqsbqixxo.sHtML

Py:   s.count("a")
来源：http://www.m.share.yfazqb.com/Article/details/gkfrvpjbj.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.yfazqb.com/Article/details/gzcnqcqft.sHtML

JS:   s.split("a").length - 1
来源：http://3g.epnwcf.com/Article/details/ggoqulpes.sHtML

TS:   s.split("a").length - 1
来源：http://wap.sjlbkw.cn/Article/details/gpfpelhxz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.yfazqb.com/Article/details/gayxxuvpi.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.tarul.cn/Article/details/gfhuptyrb.sHtML

Ruby: s.count("a")
来源：http://read.share.epnwcf.com/Article/details/gwenbkgfo.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.sjlbkw.cn/Article/details/gvmgbxwzd.sHtML

[E13] 逐字符遍历
来源：http://mobile.tarul.cn/Article/details/gfxdohzvo.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.yfazqb.com/Article/details/gmkrlnnta.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fktsv.cn/Article/details/grxbfoqpw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fktsv.cn/Article/details/gyfozyiee.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.bbcook.cn/Article/details/gvfeaqtka.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.sjlbkw.cn/Article/details/gemsdsqyy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.bbcook.cn/Article/details/gwvykalpc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.tarul.cn/Article/details/gzbzuawyb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.sjlbkw.cn/Article/details/gclbcgkuv.sHtML

[E14] URL 编码与 Base64
来源：http://baike.epnwcf.com/Article/details/govqddhlx.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.yfazqb.com/Article/details/gwowemajx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.tarul.cn/Article/details/gwukrtrew.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.sjlbkw.cn/Article/details/gqkksfcoy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.epnwcf.com/Article/details/gqahjnotf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.epnwcf.com/Article/details/gehrknyvt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.bbcook.cn/Article/details/gkenerffi.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.tarul.cn/Article/details/gandxjsgw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.epnwcf.com/Article/details/gblpccmmd.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.epnwcf.com/Article/details/gzxanrbym.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.yfazqb.com/Article/details/gxevntkhr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fktsv.cn/Article/details/gvazzqluz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.tarul.cn/Article/details/gikuiirjb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.epnwcf.com/Article/details/gfxeoolkz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.yfazqb.com/Article/details/gbxggsyjy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.vehdjk.com/Article/details/gsgkrvmsj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fktsv.cn/Article/details/gvnmpcamw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.bbcook.cn/Article/details/gfxegvykk.sHtML

[E16] 数字千分位
来源：http://www.blog.epnwcf.com/Article/details/geqzhnalo.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.tarul.cn/Article/details/gmefdqndx.sHtML

PHP:  number_format(1234567);
来源：http://www.share.sjlbkw.cn/Article/details/gpkgbgumo.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.sjlbkw.cn/Article/details/gybograls.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.yfazqb.com/Article/details/gkchayqho.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.sjlbkw.cn/Article/details/guilsuayt.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.yfazqb.com/Article/details/gryarawls.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.sjlbkw.cn/Article/details/gqfhlqyqr.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.epnwcf.com/Article/details/grcaqanxp.sHtML

[E17] 首字母大写
来源：http://wap.fktsv.cn/Article/details/gpnlismlx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.bbcook.cn/Article/details/gldytdygy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.epnwcf.com/Article/details/gmcmklovj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.tarul.cn/Article/details/gkmdhndek.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.sjlbkw.cn/Article/details/gpkvnzdyz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.sjlbkw.cn/Article/details/gtmehpxsq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.tarul.cn/Article/details/gmytojdhz.sHtML

Ruby: s.capitalize
来源：http://www.share.sjlbkw.cn/Article/details/gwcvoktze.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.yfazqb.com/Article/details/ggvitxxwm.sHtML

[E18] 模板占位符替换
来源：http://www.blog.bbcook.cn/Article/details/gvyucsgsk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.epnwcf.com/Article/details/gkpiimpvp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.sjlbkw.cn/Article/details/gjhjhalyy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.yfazqb.com/Article/details/gnturixpc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.fktsv.cn/Article/details/ggovuiejb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.yfazqb.com/Article/details/gtmjczgej.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.sjlbkw.cn/Article/details/guqekpjoc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.tarul.cn/Article/details/glyriwavh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.tarul.cn/Article/details/gzeaerwgk.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.tarul.cn/Article/details/ghubrfvnu.sHtML

Py:   s.splitlines()
来源：http://read.share.tarul.cn/Article/details/gqdfhvueo.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.yfazqb.com/Article/details/gqknqhzpv.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.vehdjk.com/Article/details/guvvsxyus.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fktsv.cn/Article/details/gtbmzenkh.sHtML

Java: s.lines().toList()
来源：http://m.share.epnwcf.com/Article/details/gacpjwdas.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.epnwcf.com/Article/details/gkcabpjuv.sHtML


<!-- 参考信息 -->