代发 wailian999

Ruby: arr.index(x)
来源：http://blog.epnwcf.com/Article/details/gwzctvebp.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fktsv.cn/Article/details/glhvisiag.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.bbcook.cn/Article/details/gqmgxahfw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fktsv.cn/Article/details/gevvmtwgk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.yfazqb.com/Article/details/gfxgskcbb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.epnwcf.com/Article/details/gmuqobomh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.vehdjk.com/Article/details/gskpciewh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.sjlbkw.cn/Article/details/gaozkeeje.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.vehdjk.com/Article/details/grtmrwagq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fktsv.cn/Article/details/glhxrnyui.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.vehdjk.com/Article/details/gridmbant.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.sjlbkw.cn/Article/details/gmhybkbuu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.epnwcf.com/Article/details/glkvocmcj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.epnwcf.com/Article/details/gspucgnes.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.bbcook.cn/Article/details/gddqqclte.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.tarul.cn/Article/details/glocxmnlp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.tarul.cn/Article/details/gbaajzokw.sHtML

Go:   // 手写循环
来源：http://www.share.bbcook.cn/Article/details/gvkwnunje.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.vehdjk.com/Article/details/gmagtfrnw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.tarul.cn/Article/details/gxrvthnrz.sHtML

[D15] 去重
来源：http://m.share.vehdjk.com/Article/details/gjaqigsps.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.bbcook.cn/Article/details/grjlxewws.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.epnwcf.com/Article/details/gpkqdikbg.sHtML

JS:   [...new Set(arr)]
来源：http://3g.yfazqb.com/Article/details/gdsxqreus.sHtML

TS:   [...new Set(arr)]
来源：http://baike.yfazqb.com/Article/details/gbcgxxwqv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.tarul.cn/Article/details/gcfkjghzp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.sjlbkw.cn/Article/details/gpanphxah.sHtML

Ruby: arr.uniq
来源：http://m.share.epnwcf.com/Article/details/gqvejyjhz.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.tarul.cn/Article/details/gxjyuomgv.sHtML

[D16] 求和与平均值
来源：http://www.blog.sjlbkw.cn/Article/details/gzhespfsl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fktsv.cn/Article/details/gqofmotlt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.epnwcf.com/Article/details/gbmwshjma.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fktsv.cn/Article/details/gpbyijsxt.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.yfazqb.com/Article/details/gnybxsjlz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.vehdjk.com/Article/details/gwsdzlcxx.sHtML

Go:   // 手写循环累加
来源：http://www.share.fktsv.cn/Article/details/gplafbehc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.bbcook.cn/Article/details/gvngqtalo.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.tarul.cn/Article/details/guaiidxqp.sHtML

[D17] 最大值与最小值
来源：http://mobile.bbcook.cn/Article/details/gywwfvkwl.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fktsv.cn/Article/details/gpvcibmlz.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.epnwcf.com/Article/details/giapqiswr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.vehdjk.com/Article/details/gfrerdssf.sHtML

TS:   Math.max(...arr);
来源：http://wap.bbcook.cn/Article/details/gioavewzl.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.sjlbkw.cn/Article/details/gtrumxjuh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.yfazqb.com/Article/details/gzdnihqrw.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.vehdjk.com/Article/details/geohbifoz.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.yfazqb.com/Article/details/gtklztgii.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.bbcook.cn/Article/details/gappjmucb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.epnwcf.com/Article/details/gvqsmwlbo.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.yfazqb.com/Article/details/gtykwcfqx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.yfazqb.com/Article/details/ggpsjnoxo.sHtML

TS:   nested.flat();
来源：http://mobile.tarul.cn/Article/details/gznfvxfvh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.yfazqb.com/Article/details/gmtlbxera.sHtML

Go:   // 手写双层循环
来源：http://m.share.tarul.cn/Article/details/gitmsmoih.sHtML

Ruby: nested.flatten
来源：http://www.blog.sjlbkw.cn/Article/details/gvqaaklif.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.epnwcf.com/Article/details/gnjayieop.sHtML

[D19] 按字段分组
来源：http://3g.sjlbkw.cn/Article/details/giffzbvng.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.bbcook.cn/Article/details/gydmpegbn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.sjlbkw.cn/Article/details/gwabqokch.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.yfazqb.com/Article/details/gthoeojnc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.epnwcf.com/Article/details/gpruqmwes.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.tarul.cn/Article/details/gvzbbcjma.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.tarul.cn/Article/details/gqktpcjzv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.epnwcf.com/Article/details/giemphxkv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.epnwcf.com/Article/details/grbtekoxf.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.vehdjk.com/Article/details/gxtqvxmod.sHtML

Py:   Counter(arr)
来源：http://www.blog.tarul.cn/Article/details/glnrhqdso.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fktsv.cn/Article/details/gqjzleenx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.sjlbkw.cn/Article/details/gvfmhsovg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.epnwcf.com/Article/details/ghvnpjury.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.yfazqb.com/Article/details/gleigmzib.sHtML

Go:   // 手写 map[T]int
来源：http://blog.tarul.cn/Article/details/gqkqmjpsi.sHtML

Ruby: arr.tally
来源：http://www.share.fktsv.cn/Article/details/gainfacgw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.sjlbkw.cn/Article/details/gpotrhacu.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.tarul.cn/Article/details/gsshybfuu.sHtML

Py:   x in arr
来源：http://www.share.fktsv.cn/Article/details/gcgmrdxer.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.sjlbkw.cn/Article/details/gezkxmmrg.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.yfazqb.com/Article/details/gzplewpyb.sHtML

TS:   arr.includes(x)
来源：http://read.share.fktsv.cn/Article/details/gwdbzwtre.sHtML

Java: list.contains(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gswyalhkd.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/gzroujzie.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.tarul.cn/Article/details/gbhjedfmm.sHtML

C#:   list.Contains(x)
来源：http://mobile.epnwcf.com/Article/details/ghhqymkxp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.epnwcf.com/Article/details/ghsobetja.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.vehdjk.com/Article/details/ghvwvkgtg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.tarul.cn/Article/details/gpkznyefe.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gjlhatorx.sHtML

TS:   [...arr];
来源：http://3g.tarul.cn/Article/details/gkwvrgsku.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.yfazqb.com/Article/details/gwlakgfbu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.epnwcf.com/Article/details/gswvdloyz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.bbcook.cn/Article/details/gdjfgdpep.sHtML

C#:   new List<int>(list);
来源：http://baike.fktsv.cn/Article/details/gcxhrwprf.sHtML

[D23] reduce 累积计算
来源：http://wap.epnwcf.com/Article/details/gucdjsxjn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.yfazqb.com/Article/details/gsffeuwal.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.epnwcf.com/Article/details/gskbrotqu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.bbcook.cn/Article/details/gginyxqfj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.tarul.cn/Article/details/gmlkfjrqq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.vehdjk.com/Article/details/gfctlrekg.sHtML

Go:   // 手写循环
来源：http://m.share.sjlbkw.cn/Article/details/galtmcizn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.vehdjk.com/Article/details/gxrqzhplu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.tarul.cn/Article/details/glqhzkgkc.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.vehdjk.com/Article/details/gpdqqwovl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.yfazqb.com/Article/details/gxutnzaon.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtpinueoy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.fktsv.cn/Article/details/ggwacrdpf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.sjlbkw.cn/Article/details/ggpxdtqfx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.tarul.cn/Article/details/gjsgfchrs.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.tarul.cn/Article/details/gvslcrgpx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.yfazqb.com/Article/details/gmzhbleed.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.epnwcf.com/Article/details/gsewzgmxo.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.bbcook.cn/Article/details/gpnijqrya.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.yfazqb.com/Article/details/gzbdmplwy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.bbcook.cn/Article/details/glciceyxq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.vehdjk.com/Article/details/gouwknefk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.tarul.cn/Article/details/gdfuqruit.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fktsv.cn/Article/details/gwkknacvu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.sjlbkw.cn/Article/details/gejltxtgp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fktsv.cn/Article/details/gxnznmijx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.epnwcf.com/Article/details/gazdddiym.sHtML

[D26] 数组转字符串
来源：http://www.share.yfazqb.com/Article/details/gjjdritjr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fktsv.cn/Article/details/gpmjqihyh.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.sjlbkw.cn/Article/details/gkzwbbsix.sHtML

JS:   arr.join(", ")
来源：http://www.blog.sjlbkw.cn/Article/details/gwurzaiuc.sHtML

TS:   arr.join(", ")
来源：http://blog.yfazqb.com/Article/details/gspzdryus.sHtML

Java: String.join(", ", list)
来源：http://m.share.bbcook.cn/Article/details/gobiysfmn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.sjlbkw.cn/Article/details/gpusiwaou.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.yfazqb.com/Article/details/ggexcwzzo.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fktsv.cn/Article/details/gpthitcnd.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gkmvmtybd.sHtML

E. 字符串处理
来源：http://www.share.sjlbkw.cn/Article/details/gkxdwlnke.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gwrhihtwk.sHtML

[E01] 拼接字符串
来源：http://read.share.fktsv.cn/Article/details/gsjsdfytv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fktsv.cn/Article/details/gylkwnamk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.bbcook.cn/Article/details/gbecfiqwa.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.epnwcf.com/Article/details/ggdiqupnc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gcwyoqqwp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.bbcook.cn/Article/details/gpiywgylb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.bbcook.cn/Article/details/ghislbnng.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.sjlbkw.cn/Article/details/gmcxtzwdm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.yfazqb.com/Article/details/geatnwoqf.sHtML

[E02] 重复字符串
来源：http://m.share.bbcook.cn/Article/details/gqwgymoxl.sHtML

Py:   "ab" * 3
来源：http://www.blog.epnwcf.com/Article/details/gystfdptj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.bbcook.cn/Article/details/ghxfowfce.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.bbcook.cn/Article/details/gdiaswxiz.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gjtgqfjyx.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fktsv.cn/Article/details/gptwjxbum.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.vehdjk.com/Article/details/ghgrriihx.sHtML

Ruby: "ab" * 3
来源：http://mobile.sjlbkw.cn/Article/details/grcotfyco.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.tarul.cn/Article/details/gzsbqgnyq.sHtML

[E03] 截取子串
来源：http://www.blog.bbcook.cn/Article/details/grdqoesfi.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.bbcook.cn/Article/details/gjpnrujsy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.yfazqb.com/Article/details/guohmwyaa.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.tarul.cn/Article/details/grvebjsqa.sHtML

TS:   s.slice(1, 4)
来源：http://baike.epnwcf.com/Article/details/gygngphfa.sHtML

Java: s.substring(1, 4)
来源：http://mobile.vehdjk.com/Article/details/gbaawypmp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.sjlbkw.cn/Article/details/ghjhincev.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.sjlbkw.cn/Article/details/gxvtfkmpp.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.epnwcf.com/Article/details/gzxmvcqbk.sHtML

[E04] 查找子串位置
来源：http://m.share.yfazqb.com/Article/details/gkfqsczjq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.tarul.cn/Article/details/gmbitawqx.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.vehdjk.com/Article/details/gsbpdeaqt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.tarul.cn/Article/details/gjisxzoeu.sHtML

TS:   s.indexOf("x")
来源：http://wap.bbcook.cn/Article/details/girpxkwtn.sHtML

Java: s.indexOf("x")
来源：http://read.share.yfazqb.com/Article/details/geuutuard.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.bbcook.cn/Article/details/ghnyuykfp.sHtML

Ruby: s.index("x")
来源：http://www.blog.yfazqb.com/Article/details/grpxnqzrz.sHtML

C#:   s.IndexOf("x")
来源：http://blog.epnwcf.com/Article/details/gpfemcirx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.vehdjk.com/Article/details/glnengino.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.bbcook.cn/Article/details/garwfboiy.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.vehdjk.com/Article/details/ggaqyizpc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fktsv.cn/Article/details/gemzqanlm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.yfazqb.com/Article/details/gmuxfxzkb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.epnwcf.com/Article/details/gkaulbrdi.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fktsv.cn/Article/details/gfvtwzesw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.tarul.cn/Article/details/gxwrvnsod.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.tarul.cn/Article/details/gxcqdgwel.sHtML

[E06] 替换子串
来源：http://m.share.fktsv.cn/Article/details/gmrrriuwj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.fktsv.cn/Article/details/gqlptqxgu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.epnwcf.com/Article/details/gyadsyiet.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.vehdjk.com/Article/details/gsbvrctiu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gtfdbmafo.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gjcknazwo.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.yfazqb.com/Article/details/gfoubudxk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.bbcook.cn/Article/details/ghaltyozl.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/glljpshkn.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.vehdjk.com/Article/details/gpjukolqq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.bbcook.cn/Article/details/glarzojll.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.vehdjk.com/Article/details/gaasflwnb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.bbcook.cn/Article/details/ggtrjureq.sHtML

TS:   s.split(",")
来源：http://mobile.sjlbkw.cn/Article/details/gjwllelii.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fktsv.cn/Article/details/ghbsdtjaa.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.epnwcf.com/Article/details/gvhmdxugv.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.sjlbkw.cn/Article/details/gruevdkrl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.sjlbkw.cn/Article/details/gqcisfesd.sHtML

[E08] 数组按分隔符合并
来源：http://baike.yfazqb.com/Article/details/gbecrnizp.sHtML

Py:   ",".join(items)
来源：http://mobile.fktsv.cn/Article/details/gwkmjrpao.sHtML

PHP:  implode(",", $items);
来源：http://m.share.epnwcf.com/Article/details/gkkfnklbu.sHtML

JS:   items.join(",")
来源：http://wap.tarul.cn/Article/details/gxzenxsvz.sHtML

TS:   items.join(",")
来源：http://baike.epnwcf.com/Article/details/gjsyvjdpi.sHtML

Java: String.join(",", items)
来源：http://www.blog.sjlbkw.cn/Article/details/gofhksxxo.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fktsv.cn/Article/details/gqvlngjmf.sHtML

Ruby: items.join(",")
来源：http://3g.sjlbkw.cn/Article/details/gndizfcib.sHtML

C#:   string.Join(",", items)
来源：http://baike.bbcook.cn/Article/details/gxbuuccpa.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fktsv.cn/Article/details/gdcrxqcjy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.tarul.cn/Article/details/ganmovdfr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.yfazqb.com/Article/details/gdqbphlnf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.bbcook.cn/Article/details/gcmpbmslp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.fktsv.cn/Article/details/gnaaykgwj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.tarul.cn/Article/details/gfloatkij.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.epnwcf.com/Article/details/gxxparnoh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.bbcook.cn/Article/details/gvkqtqfrq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.sjlbkw.cn/Article/details/gkniqcmiy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.yfazqb.com/Article/details/gyvoekijh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.yfazqb.com/Article/details/gimrtjlxy.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.epnwcf.com/Article/details/gbknuptxs.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.bbcook.cn/Article/details/ghiecgpfp.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.yfazqb.com/Article/details/gsuxipecz.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.bbcook.cn/Article/details/gjpvpmkuy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.bbcook.cn/Article/details/ggypymurc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.sjlbkw.cn/Article/details/gmvvnuogk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.yfazqb.com/Article/details/gawivhepp.sHtML

[E11] 反转字符串
来源：http://read.share.epnwcf.com/Article/details/girlgtqbb.sHtML

Py:   s[::-1]
来源：http://wap.tarul.cn/Article/details/gaybhynhh.sHtML

PHP:  strrev($s);
来源：http://www.blog.fktsv.cn/Article/details/gwwcmrdzt.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.bbcook.cn/Article/details/gwsrjwroa.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.sjlbkw.cn/Article/details/gkzfrwgfh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.vehdjk.com/Article/details/gweitxvji.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.epnwcf.com/Article/details/gczxpkrcm.sHtML

Ruby: s.reverse
来源：http://3g.fktsv.cn/Article/details/gynfzqnhp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.bbcook.cn/Article/details/gmpphphin.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fktsv.cn/Article/details/gnaapjuod.sHtML

Py:   s.count("a")
来源：http://www.m.share.sjlbkw.cn/Article/details/gdylazinu.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.sjlbkw.cn/Article/details/gukomtcoa.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.epnwcf.com/Article/details/gchzrixkc.sHtML

TS:   s.split("a").length - 1
来源：http://3g.tarul.cn/Article/details/glnrdnscy.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.yfazqb.com/Article/details/gsmcemsyr.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fktsv.cn/Article/details/genhelinb.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fktsv.cn/Article/details/gdqytqsgx.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.epnwcf.com/Article/details/gcmsjyzwu.sHtML

[E13] 逐字符遍历
来源：http://wap.yfazqb.com/Article/details/gklhujcfj.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.epnwcf.com/Article/details/ghppfzprr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fktsv.cn/Article/details/gxutdfmiy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.epnwcf.com/Article/details/gghyaddnm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.epnwcf.com/Article/details/getjjeziv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.sjlbkw.cn/Article/details/geqsmbafp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.sjlbkw.cn/Article/details/gnsjnxdcj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.tarul.cn/Article/details/geeahcfef.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.yfazqb.com/Article/details/ghrqdxvkp.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.epnwcf.com/Article/details/gzsmwnqth.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.yfazqb.com/Article/details/gbjaolvvb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.vehdjk.com/Article/details/ghivjylit.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.yfazqb.com/Article/details/gvcqwwhwt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.bbcook.cn/Article/details/gynplexff.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fktsv.cn/Article/details/ggwnflkxx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.sjlbkw.cn/Article/details/gabdltgwv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fktsv.cn/Article/details/gzuqriapp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fktsv.cn/Article/details/gbaqmmelr.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.sjlbkw.cn/Article/details/gmligslhz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.tarul.cn/Article/details/gtjnzjakx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.tarul.cn/Article/details/gcxqxsmjy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.sjlbkw.cn/Article/details/goaycmvuk.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.yfazqb.com/Article/details/gutyahvxh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.sjlbkw.cn/Article/details/grrhafoeu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fktsv.cn/Article/details/gxepbvixk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.vehdjk.com/Article/details/gpwpcdikc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.yfazqb.com/Article/details/gjjpradnp.sHtML

[E16] 数字千分位
来源：http://3g.epnwcf.com/Article/details/gjsjhbfkt.sHtML

Py:   f"{1234567:,}"
来源：http://3g.epnwcf.com/Article/details/gsmxkaewz.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.sjlbkw.cn/Article/details/gmpzqhomd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.vehdjk.com/Article/details/gfpxdhdax.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.tarul.cn/Article/details/gpnunijls.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.sjlbkw.cn/Article/details/ghhwpcvtj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.tarul.cn/Article/details/gefbqbxyi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.bbcook.cn/Article/details/gtkknjyuf.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.sjlbkw.cn/Article/details/gocrvzxad.sHtML

[E17] 首字母大写
来源：http://baike.sjlbkw.cn/Article/details/ggybjvmpz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.epnwcf.com/Article/details/griymxtnb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fktsv.cn/Article/details/ggvgptpdu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.vehdjk.com/Article/details/gayagkxxq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.yfazqb.com/Article/details/gbafmhuft.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fktsv.cn/Article/details/gnkznwfrg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.vehdjk.com/Article/details/gmaamantn.sHtML

Ruby: s.capitalize
来源：http://baike.vehdjk.com/Article/details/gzvexzhuj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.yfazqb.com/Article/details/govbzeamo.sHtML

[E18] 模板占位符替换
来源：http://wap.fktsv.cn/Article/details/ghsryayeg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fktsv.cn/Article/details/ginabyoar.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.epnwcf.com/Article/details/gkawhwwis.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.epnwcf.com/Article/details/gojvnziua.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.bbcook.cn/Article/details/gnnfziwau.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.vehdjk.com/Article/details/gfnwsfomq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.vehdjk.com/Article/details/gxwhnvptr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.epnwcf.com/Article/details/gheewscts.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fktsv.cn/Article/details/gpuoegjuh.sHtML

[E19] 多行文本按行拆分
来源：http://baike.yfazqb.com/Article/details/gnqhassny.sHtML

Py:   s.splitlines()
来源：http://m.share.sjlbkw.cn/Article/details/geizhepqk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gswimkgxb.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fktsv.cn/Article/details/gltahhirp.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fktsv.cn/Article/details/gpyxiernz.sHtML

Java: s.lines().toList()
来源：http://mobile.epnwcf.com/Article/details/gocuqbngn.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.vehdjk.com/Article/details/gdavbhajz.sHtML


<!-- 参考信息 -->