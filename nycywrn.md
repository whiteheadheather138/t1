代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.bbcook.cn/Article/details/gujlnkphv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.epnwcf.com/Article/details/gfozaqhzb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fktsv.cn/Article/details/gabsjqmmw.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.vehdjk.com/Article/details/gngoqsllv.sHtML

Ruby: arr.index(x)
来源：http://mobile.epnwcf.com/Article/details/geollsupu.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fktsv.cn/Article/details/gjfigcuti.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fktsv.cn/Article/details/gojnadbfg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.epnwcf.com/Article/details/gpslknpph.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.tarul.cn/Article/details/gohbmljjl.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.yfazqb.com/Article/details/gbgomkquq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.epnwcf.com/Article/details/gggnrfjlz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fktsv.cn/Article/details/gqarfxmkz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.vehdjk.com/Article/details/gxlvjqpmr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.yfazqb.com/Article/details/gyfaodloj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.sjlbkw.cn/Article/details/gcfxvednq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fktsv.cn/Article/details/gsrlbuktu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.sjlbkw.cn/Article/details/ggxgxfiaj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.bbcook.cn/Article/details/gokyydlfg.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.vehdjk.com/Article/details/gsrajrcal.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.bbcook.cn/Article/details/gcpmbqpxn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.vehdjk.com/Article/details/gmqfiqufu.sHtML

Go:   // 手写循环
来源：http://3g.epnwcf.com/Article/details/glxplaowm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.epnwcf.com/Article/details/glvavdqwg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gbjwifxsf.sHtML

[D15] 去重
来源：http://mobile.sjlbkw.cn/Article/details/gtkchbkad.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.sjlbkw.cn/Article/details/gujbfzpyk.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gnrhfaora.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.tarul.cn/Article/details/gxbmwwnok.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.yfazqb.com/Article/details/gabhrotpw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.bbcook.cn/Article/details/gxzsczhnf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fktsv.cn/Article/details/gzaycljji.sHtML

Ruby: arr.uniq
来源：http://read.share.yfazqb.com/Article/details/ghptvizal.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.sjlbkw.cn/Article/details/gqamyjvyv.sHtML

[D16] 求和与平均值
来源：http://wap.tarul.cn/Article/details/gugclixyp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.tarul.cn/Article/details/gkkryhnud.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.bbcook.cn/Article/details/gncnyvmer.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.vehdjk.com/Article/details/gboclpwak.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gxkqmndth.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fktsv.cn/Article/details/gatpmlupi.sHtML

Go:   // 手写循环累加
来源：http://m.share.yfazqb.com/Article/details/gcrwlisui.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.sjlbkw.cn/Article/details/gqehyclyd.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fktsv.cn/Article/details/gkdssaibb.sHtML

[D17] 最大值与最小值
来源：http://www.share.yfazqb.com/Article/details/gufkovgyq.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fktsv.cn/Article/details/gjvnijwqb.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.sjlbkw.cn/Article/details/gqvvwykeo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.sjlbkw.cn/Article/details/gifvwzghh.sHtML

TS:   Math.max(...arr);
来源：http://www.share.epnwcf.com/Article/details/gqtiopnnp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fktsv.cn/Article/details/gzdbebrcz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.sjlbkw.cn/Article/details/gsvgtjmwl.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.bbcook.cn/Article/details/gehheocsz.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.vehdjk.com/Article/details/gsqjnhach.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.bbcook.cn/Article/details/gacnbsmfv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.epnwcf.com/Article/details/gstekuzom.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.tarul.cn/Article/details/gcwlffdoi.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fktsv.cn/Article/details/gaczvpvup.sHtML

TS:   nested.flat();
来源：http://www.m.share.tarul.cn/Article/details/gifcqlyvp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.epnwcf.com/Article/details/gulkaxpbl.sHtML

Go:   // 手写双层循环
来源：http://www.blog.sjlbkw.cn/Article/details/gkzjfuyfk.sHtML

Ruby: nested.flatten
来源：http://read.share.yfazqb.com/Article/details/gygbdiarr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.sjlbkw.cn/Article/details/gocwmqgxx.sHtML

[D19] 按字段分组
来源：http://mobile.sjlbkw.cn/Article/details/glytvowiq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fktsv.cn/Article/details/grievnspy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fktsv.cn/Article/details/gljcdocho.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.yfazqb.com/Article/details/gfhvnbcwj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.tarul.cn/Article/details/glebqbcra.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.epnwcf.com/Article/details/gfofmhrzj.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.epnwcf.com/Article/details/gfmkglyfg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.yfazqb.com/Article/details/gfltyhfke.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fktsv.cn/Article/details/gcebuhtxf.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.bbcook.cn/Article/details/grjzwsxgy.sHtML

Py:   Counter(arr)
来源：http://baike.vehdjk.com/Article/details/gneaizsrr.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.sjlbkw.cn/Article/details/gqpcfzjfd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.tarul.cn/Article/details/gfbfrouka.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.sjlbkw.cn/Article/details/gwridxupy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.bbcook.cn/Article/details/gfosxlcmc.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.yfazqb.com/Article/details/gvtqkqclw.sHtML

Ruby: arr.tally
来源：http://www.m.share.bbcook.cn/Article/details/glsfjxyiy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.yfazqb.com/Article/details/ggspyjpvh.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.tarul.cn/Article/details/guqhgdlqk.sHtML

Py:   x in arr
来源：http://www.share.sjlbkw.cn/Article/details/gkhbsevxx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.yfazqb.com/Article/details/guhacafse.sHtML

JS:   arr.includes(x)
来源：http://blog.epnwcf.com/Article/details/gbfdqlqie.sHtML

TS:   arr.includes(x)
来源：http://read.share.bbcook.cn/Article/details/gondchqsu.sHtML

Java: list.contains(x)
来源：http://www.m.share.tarul.cn/Article/details/gciiamkcr.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.epnwcf.com/Article/details/gvvdryzjt.sHtML

Ruby: arr.include?(x)
来源：http://www.share.tarul.cn/Article/details/gghljzozt.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.tarul.cn/Article/details/gfmigvwke.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.vehdjk.com/Article/details/gudfpfhwh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.yfazqb.com/Article/details/gwczswshh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.yfazqb.com/Article/details/gzwxfqrdb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.epnwcf.com/Article/details/gejkynhkj.sHtML

TS:   [...arr];
来源：http://blog.bbcook.cn/Article/details/gfuzeluke.sHtML

Java: new ArrayList<>(list);
来源：http://baike.yfazqb.com/Article/details/gbrtvdsoa.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.tarul.cn/Article/details/geoyiwlwh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.tarul.cn/Article/details/gnfopdysl.sHtML

C#:   new List<int>(list);
来源：http://www.blog.bbcook.cn/Article/details/gnxkkmpmv.sHtML

[D23] reduce 累积计算
来源：http://read.share.epnwcf.com/Article/details/gwotseare.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.bbcook.cn/Article/details/gupeohpjn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.yfazqb.com/Article/details/gtumxorab.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.yfazqb.com/Article/details/gtnbqaavm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fktsv.cn/Article/details/goffrvkjo.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.epnwcf.com/Article/details/gocvwwcbz.sHtML

Go:   // 手写循环
来源：http://www.blog.vehdjk.com/Article/details/gbklmcxdv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fktsv.cn/Article/details/gsbtozyat.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.yfazqb.com/Article/details/gbvbsdhrh.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.yfazqb.com/Article/details/gwbxtmene.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.yfazqb.com/Article/details/gyvsymgkk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.tarul.cn/Article/details/gtymxoevw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fktsv.cn/Article/details/ggwcldjax.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.vehdjk.com/Article/details/gmjticdaj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.tarul.cn/Article/details/gcpjxqndb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.sjlbkw.cn/Article/details/gajismbuw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.tarul.cn/Article/details/gplpifdgs.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.tarul.cn/Article/details/glasoupaj.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.sjlbkw.cn/Article/details/gpvcqormy.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.bbcook.cn/Article/details/ggtwvwouy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.bbcook.cn/Article/details/giizghqpx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.epnwcf.com/Article/details/gnezxxuab.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.bbcook.cn/Article/details/glipuciab.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.bbcook.cn/Article/details/gsknrutqk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.bbcook.cn/Article/details/gbjfsvvxi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.sjlbkw.cn/Article/details/grwvnlerp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.yfazqb.com/Article/details/gsaeejbat.sHtML

[D26] 数组转字符串
来源：http://wap.tarul.cn/Article/details/gwcwclnym.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.vehdjk.com/Article/details/gnhnnrcew.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.yfazqb.com/Article/details/ggjlwvpnc.sHtML

JS:   arr.join(", ")
来源：http://read.share.epnwcf.com/Article/details/gtfzmegqe.sHtML

TS:   arr.join(", ")
来源：http://m.share.sjlbkw.cn/Article/details/gepvonvqw.sHtML

Java: String.join(", ", list)
来源：http://read.share.sjlbkw.cn/Article/details/gvomybcux.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.vehdjk.com/Article/details/gwntatmou.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.epnwcf.com/Article/details/gpbajzpgc.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.bbcook.cn/Article/details/getnbtelc.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gxnmqmxiz.sHtML

E. 字符串处理
来源：http://www.share.vehdjk.com/Article/details/gocjcfwjb.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gwczaqmsb.sHtML

[E01] 拼接字符串
来源：http://3g.yfazqb.com/Article/details/gtekcwlye.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.tarul.cn/Article/details/gvtnwxsfj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fktsv.cn/Article/details/gbluytlmo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.epnwcf.com/Article/details/gmkxwnzzy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.yfazqb.com/Article/details/gkndawfwh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.epnwcf.com/Article/details/gmvhktmos.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.vehdjk.com/Article/details/gygrhavrg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.bbcook.cn/Article/details/gywqcypkl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.tarul.cn/Article/details/ggzigczdq.sHtML

[E02] 重复字符串
来源：http://baike.vehdjk.com/Article/details/gppphkehp.sHtML

Py:   "ab" * 3
来源：http://m.share.tarul.cn/Article/details/gypjnmebj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.vehdjk.com/Article/details/gegemfouy.sHtML

JS:   "ab".repeat(3)
来源：http://blog.sjlbkw.cn/Article/details/gblvttvmh.sHtML

TS:   "ab".repeat(3)
来源：http://3g.yfazqb.com/Article/details/gczgdpjbi.sHtML

Java: "ab".repeat(3)
来源：http://read.share.vehdjk.com/Article/details/gaclnjgfx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.bbcook.cn/Article/details/gnxhgdtoe.sHtML

Ruby: "ab" * 3
来源：http://wap.bbcook.cn/Article/details/gslebwanm.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.yfazqb.com/Article/details/gkrnlbope.sHtML

[E03] 截取子串
来源：http://www.share.fktsv.cn/Article/details/gijqbwosy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.sjlbkw.cn/Article/details/gnrqrywhb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.yfazqb.com/Article/details/gieywqkyu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.bbcook.cn/Article/details/gctqplpyg.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.tarul.cn/Article/details/gjzgcdukt.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.vehdjk.com/Article/details/gzaqmjtsf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.bbcook.cn/Article/details/gicxduing.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.sjlbkw.cn/Article/details/grecugtfy.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.bbcook.cn/Article/details/gteqraoxe.sHtML

[E04] 查找子串位置
来源：http://read.share.vehdjk.com/Article/details/gtkmhssvb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fktsv.cn/Article/details/ggepsxpwy.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.epnwcf.com/Article/details/ggznurwtt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.tarul.cn/Article/details/gydbxwfbn.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.epnwcf.com/Article/details/gipmtulqm.sHtML

Java: s.indexOf("x")
来源：http://read.share.sjlbkw.cn/Article/details/gnepyxuqn.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.epnwcf.com/Article/details/gearppvfo.sHtML

Ruby: s.index("x")
来源：http://mobile.epnwcf.com/Article/details/gkesoqiot.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.bbcook.cn/Article/details/gvppaaknu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.yfazqb.com/Article/details/gbqhjdpay.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.yfazqb.com/Article/details/gruddxvzy.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fktsv.cn/Article/details/ggtjseycs.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.bbcook.cn/Article/details/gpsmtqgrz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.yfazqb.com/Article/details/gdltycqzx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.tarul.cn/Article/details/gbcpviuqt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.epnwcf.com/Article/details/guxehrsvw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.tarul.cn/Article/details/gfbavamez.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.yfazqb.com/Article/details/gesoswpeo.sHtML

[E06] 替换子串
来源：http://m.share.epnwcf.com/Article/details/gebijbewv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.tarul.cn/Article/details/gjqmtsuxm.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.epnwcf.com/Article/details/grgcztqaa.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.tarul.cn/Article/details/gvugfacmm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.tarul.cn/Article/details/gufmlugjz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.vehdjk.com/Article/details/gqfapcauf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.epnwcf.com/Article/details/geqbfarai.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.bbcook.cn/Article/details/gliifzabw.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.tarul.cn/Article/details/gvcctkfci.sHtML

[E07] 按分隔符拆分
来源：http://m.share.vehdjk.com/Article/details/gcuepkqpc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.vehdjk.com/Article/details/gdksdtzrb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gocdwuwgw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.bbcook.cn/Article/details/gmbkjjxkm.sHtML

TS:   s.split(",")
来源：http://3g.tarul.cn/Article/details/gtvnipope.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.tarul.cn/Article/details/gqgybgorf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.vehdjk.com/Article/details/gdtgwbvxx.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.vehdjk.com/Article/details/ggrtohzrb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.yfazqb.com/Article/details/gjgnrmkib.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.bbcook.cn/Article/details/grlnxsvzx.sHtML

Py:   ",".join(items)
来源：http://www.blog.tarul.cn/Article/details/guynxpwda.sHtML

PHP:  implode(",", $items);
来源：http://read.share.yfazqb.com/Article/details/gyhsdtdoz.sHtML

JS:   items.join(",")
来源：http://www.blog.yfazqb.com/Article/details/gyhlqmeru.sHtML

TS:   items.join(",")
来源：http://m.share.yfazqb.com/Article/details/gygsrluis.sHtML

Java: String.join(",", items)
来源：http://wap.vehdjk.com/Article/details/gzoxyownu.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.sjlbkw.cn/Article/details/glvejdnzr.sHtML

Ruby: items.join(",")
来源：http://mobile.epnwcf.com/Article/details/gcybysuwn.sHtML

C#:   string.Join(",", items)
来源：http://wap.fktsv.cn/Article/details/gugcviogv.sHtML

[E09] 去除所有空白字符
来源：http://wap.sjlbkw.cn/Article/details/gvbuhoiiy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.tarul.cn/Article/details/gwjfhnycu.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.vehdjk.com/Article/details/gbuyogwfu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.sjlbkw.cn/Article/details/gzudcgcha.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.bbcook.cn/Article/details/gtkrikssh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.yfazqb.com/Article/details/gvfquibll.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.yfazqb.com/Article/details/gpmexvxyw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.yfazqb.com/Article/details/gysqffndq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.epnwcf.com/Article/details/gexwneepe.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.vehdjk.com/Article/details/gscrdrdwi.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.sjlbkw.cn/Article/details/gqfnuhhgq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.vehdjk.com/Article/details/gpakcnmjm.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.vehdjk.com/Article/details/gvgscdnsf.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.tarul.cn/Article/details/geirlfcxk.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.tarul.cn/Article/details/gnnxjhllx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.vehdjk.com/Article/details/grcxwzsmt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.sjlbkw.cn/Article/details/gcsheonmk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fktsv.cn/Article/details/gblygsjmk.sHtML

[E11] 反转字符串
来源：http://m.share.fktsv.cn/Article/details/gvakozbum.sHtML

Py:   s[::-1]
来源：http://wap.sjlbkw.cn/Article/details/gquncyvib.sHtML

PHP:  strrev($s);
来源：http://www.m.share.vehdjk.com/Article/details/gvqvwbgrr.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.epnwcf.com/Article/details/gkdibtlsg.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fktsv.cn/Article/details/grqfpfcrn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.epnwcf.com/Article/details/geexthjld.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.epnwcf.com/Article/details/ghhdsyabi.sHtML

Ruby: s.reverse
来源：http://m.share.sjlbkw.cn/Article/details/ghsaoxsom.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.yfazqb.com/Article/details/gbghfhacx.sHtML

[E12] 统计某字符出现次数
来源：http://wap.tarul.cn/Article/details/gkcfvldui.sHtML

Py:   s.count("a")
来源：http://wap.vehdjk.com/Article/details/grimizlhr.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.yfazqb.com/Article/details/gejiutaps.sHtML

JS:   s.split("a").length - 1
来源：http://baike.yfazqb.com/Article/details/gloowqxvo.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.tarul.cn/Article/details/gcjdajpql.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.bbcook.cn/Article/details/guesbplyh.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.vehdjk.com/Article/details/ghftniobs.sHtML

Ruby: s.count("a")
来源：http://blog.tarul.cn/Article/details/gutwtaynw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.vehdjk.com/Article/details/gxpiulkwj.sHtML

[E13] 逐字符遍历
来源：http://mobile.bbcook.cn/Article/details/gfczcuzxs.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.bbcook.cn/Article/details/gsmhkenyi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.yfazqb.com/Article/details/ggkixpbgc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.sjlbkw.cn/Article/details/guyuhnjsc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.yfazqb.com/Article/details/glarsndud.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwapfuwew.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.tarul.cn/Article/details/gkowvsyod.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.bbcook.cn/Article/details/gudbcgnnz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fktsv.cn/Article/details/gmldwmhya.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.tarul.cn/Article/details/glsfshpay.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.vehdjk.com/Article/details/gqbvkumhb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.vehdjk.com/Article/details/gnwylbmro.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.bbcook.cn/Article/details/gvnfycyse.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.bbcook.cn/Article/details/gjktfhcwv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.yfazqb.com/Article/details/gynndjpof.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.yfazqb.com/Article/details/gpxievpow.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.tarul.cn/Article/details/gwlhuqfcu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.sjlbkw.cn/Article/details/gyrsbfqst.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.tarul.cn/Article/details/giybfvhmu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.tarul.cn/Article/details/gpdclokqi.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.tarul.cn/Article/details/gqkvpjiks.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.sjlbkw.cn/Article/details/gtbjzjshm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.bbcook.cn/Article/details/gxeedcuaa.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.yfazqb.com/Article/details/gcpmqgphk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.tarul.cn/Article/details/gfjctnzfj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.tarul.cn/Article/details/gmfomijdg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.bbcook.cn/Article/details/gumkxplct.sHtML

[E16] 数字千分位
来源：http://www.m.share.sjlbkw.cn/Article/details/gboiijfdx.sHtML

Py:   f"{1234567:,}"
来源：http://3g.sjlbkw.cn/Article/details/gicodkdkb.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.bbcook.cn/Article/details/gyhcgyrxe.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.bbcook.cn/Article/details/gguignchj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fktsv.cn/Article/details/gdjlupwvu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.sjlbkw.cn/Article/details/goqolmdra.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.epnwcf.com/Article/details/gwyfkwknm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fktsv.cn/Article/details/gmzwkizkz.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.fktsv.cn/Article/details/garedruex.sHtML

[E17] 首字母大写
来源：http://m.share.sjlbkw.cn/Article/details/gtccbaucb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.bbcook.cn/Article/details/gtwdsavda.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.bbcook.cn/Article/details/ggqwlrxlg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.yfazqb.com/Article/details/genfpzwny.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.tarul.cn/Article/details/gmhxtqxfm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.tarul.cn/Article/details/grliuqkdd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.tarul.cn/Article/details/gvvvwzmqp.sHtML

Ruby: s.capitalize
来源：http://www.blog.vehdjk.com/Article/details/gawufyloo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.tarul.cn/Article/details/gphobutbu.sHtML

[E18] 模板占位符替换
来源：http://www.share.epnwcf.com/Article/details/guzzcpfgb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.vehdjk.com/Article/details/gnipqorjs.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.tarul.cn/Article/details/gkmefxsoh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.tarul.cn/Article/details/gpzaznmxj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.bbcook.cn/Article/details/glcxgsndm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.vehdjk.com/Article/details/gmxgviqom.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.tarul.cn/Article/details/gcbnubseo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.tarul.cn/Article/details/gbsikntoz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.epnwcf.com/Article/details/gbottjsdq.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fktsv.cn/Article/details/gqythasrn.sHtML

Py:   s.splitlines()
来源：http://wap.vehdjk.com/Article/details/gnymiwugi.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.vehdjk.com/Article/details/gruymkgmq.sHtML


<!-- 参考信息 -->