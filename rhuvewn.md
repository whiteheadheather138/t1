代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.bbcook.cn/Article/details/glvigqhvr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fktsv.cn/Article/details/gphumakan.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.yfazqb.com/Article/details/gxoakyllt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.tarul.cn/Article/details/gwpemzpij.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.yfazqb.com/Article/details/gawtknqyk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.yfazqb.com/Article/details/gvpfrrxio.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.vehdjk.com/Article/details/gyhudbglj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.vehdjk.com/Article/details/gnmkmzrxh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.sjlbkw.cn/Article/details/gbzgbsgaq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.yfazqb.com/Article/details/ghtuzjxpl.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.bbcook.cn/Article/details/gqgtsecck.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.bbcook.cn/Article/details/gcpcloizp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.sjlbkw.cn/Article/details/gvgjrhwhj.sHtML

Go:   // 手写循环
来源：http://3g.sjlbkw.cn/Article/details/gxdxvxsfd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fktsv.cn/Article/details/ghxryszjd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fktsv.cn/Article/details/gtxuqbscp.sHtML

[D15] 去重
来源：http://www.m.share.tarul.cn/Article/details/gligwuejw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.sjlbkw.cn/Article/details/guikwnpog.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.bbcook.cn/Article/details/gxzgovjwc.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.tarul.cn/Article/details/geirapuxy.sHtML

TS:   [...new Set(arr)]
来源：http://blog.bbcook.cn/Article/details/gjdxsoayp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.sjlbkw.cn/Article/details/gmwidfjhp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.tarul.cn/Article/details/giqnfeflc.sHtML

Ruby: arr.uniq
来源：http://read.share.tarul.cn/Article/details/gcpmomquq.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.vehdjk.com/Article/details/gthtckpxp.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fktsv.cn/Article/details/gyulhdlpm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fktsv.cn/Article/details/gyapkawas.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.tarul.cn/Article/details/gqzwxnpbm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.tarul.cn/Article/details/gddchxhiz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.sjlbkw.cn/Article/details/gkxlvdafj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.sjlbkw.cn/Article/details/gjuafvgnd.sHtML

Go:   // 手写循环累加
来源：http://read.share.fktsv.cn/Article/details/gerptatbt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.vehdjk.com/Article/details/guviuifas.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.bbcook.cn/Article/details/gvvlqgcjh.sHtML

[D17] 最大值与最小值
来源：http://www.blog.epnwcf.com/Article/details/gxelgysjn.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gapjfnpsg.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.tarul.cn/Article/details/gmzxuhqow.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.epnwcf.com/Article/details/gamyxxgob.sHtML

TS:   Math.max(...arr);
来源：http://blog.epnwcf.com/Article/details/gbpuhaxsf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.tarul.cn/Article/details/gpmmilocu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.sjlbkw.cn/Article/details/gnjyamckg.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fktsv.cn/Article/details/gbeoecmrz.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.tarul.cn/Article/details/gzurdzwbh.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.sjlbkw.cn/Article/details/giydjrxsq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.vehdjk.com/Article/details/ggwfvpstr.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fktsv.cn/Article/details/gnddaxrao.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.sjlbkw.cn/Article/details/gmvutstrn.sHtML

TS:   nested.flat();
来源：http://www.m.share.sjlbkw.cn/Article/details/gzpbzndqp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.sjlbkw.cn/Article/details/gkbuoxopo.sHtML

Go:   // 手写双层循环
来源：http://3g.vehdjk.com/Article/details/gcytdwqyx.sHtML

Ruby: nested.flatten
来源：http://www.m.share.tarul.cn/Article/details/gjfncxiib.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fktsv.cn/Article/details/gfoxrtyzz.sHtML

[D19] 按字段分组
来源：http://wap.bbcook.cn/Article/details/gfpqjjnpy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.tarul.cn/Article/details/gfnlqrnry.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.vehdjk.com/Article/details/gwjdgpbwh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.sjlbkw.cn/Article/details/gntgapwql.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.tarul.cn/Article/details/gfvpqunar.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.tarul.cn/Article/details/gdeexloix.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.yfazqb.com/Article/details/gccjuzlcy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.yfazqb.com/Article/details/gzonpgbjt.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.vehdjk.com/Article/details/gstaxtxvu.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.tarul.cn/Article/details/ghcmsmboy.sHtML

Py:   Counter(arr)
来源：http://mobile.vehdjk.com/Article/details/gwxicobog.sHtML

PHP:  array_count_values($arr);
来源：http://wap.tarul.cn/Article/details/ggqqprevc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fktsv.cn/Article/details/ghjqszddx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fktsv.cn/Article/details/guoqcdroz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.sjlbkw.cn/Article/details/gzfmnfkrj.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.epnwcf.com/Article/details/glvscjhxl.sHtML

Ruby: arr.tally
来源：http://m.share.fktsv.cn/Article/details/gahvftivr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.bbcook.cn/Article/details/gxttywhmt.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.yfazqb.com/Article/details/gnulmxngt.sHtML

Py:   x in arr
来源：http://www.share.yfazqb.com/Article/details/gagunubsh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.yfazqb.com/Article/details/gaomfkduo.sHtML

JS:   arr.includes(x)
来源：http://www.share.bbcook.cn/Article/details/gmuxdgrls.sHtML

TS:   arr.includes(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gizrtbkpk.sHtML

Java: list.contains(x)
来源：http://blog.vehdjk.com/Article/details/gsjvnypac.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gwnuugfhp.sHtML

Ruby: arr.include?(x)
来源：http://www.share.sjlbkw.cn/Article/details/gdocnmogo.sHtML

C#:   list.Contains(x)
来源：http://wap.bbcook.cn/Article/details/gompaqtcd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.epnwcf.com/Article/details/gvcuebspc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.epnwcf.com/Article/details/geeliqnlr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.bbcook.cn/Article/details/gynrkqwvg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fktsv.cn/Article/details/gxpylwggm.sHtML

TS:   [...arr];
来源：http://www.m.share.fktsv.cn/Article/details/grroxjmtp.sHtML

Java: new ArrayList<>(list);
来源：http://blog.epnwcf.com/Article/details/gvvrcizpv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fktsv.cn/Article/details/gyuycixju.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.bbcook.cn/Article/details/gkapkxije.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.yfazqb.com/Article/details/gdsujeplc.sHtML

[D23] reduce 累积计算
来源：http://mobile.tarul.cn/Article/details/gbhrqwgmm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gnpdobwxp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.epnwcf.com/Article/details/gjtycylxe.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.tarul.cn/Article/details/ggqhbxjda.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.sjlbkw.cn/Article/details/gasndwruy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.bbcook.cn/Article/details/gqdboncrm.sHtML

Go:   // 手写循环
来源：http://baike.bbcook.cn/Article/details/gwfpvjlfc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.tarul.cn/Article/details/grhyeaoop.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.vehdjk.com/Article/details/gilrhkkff.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fktsv.cn/Article/details/glhsylitw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.bbcook.cn/Article/details/gtsdochlm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.yfazqb.com/Article/details/gdweasnky.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.sjlbkw.cn/Article/details/goqbrbwhz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.vehdjk.com/Article/details/gzkuqasgq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.bbcook.cn/Article/details/ghklkpedr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fktsv.cn/Article/details/gmjackjdx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.epnwcf.com/Article/details/gltnshrbu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fktsv.cn/Article/details/gmwoztkxt.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.sjlbkw.cn/Article/details/gouzospuk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.epnwcf.com/Article/details/gtnzlgxwo.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.bbcook.cn/Article/details/gjppywixo.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.epnwcf.com/Article/details/gjfgcgrpy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.sjlbkw.cn/Article/details/gxzmbnetl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.bbcook.cn/Article/details/guqhczvbx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.bbcook.cn/Article/details/gvwhfiwez.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.epnwcf.com/Article/details/gyoyggsvy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.yfazqb.com/Article/details/gswtbsknu.sHtML

[D26] 数组转字符串
来源：http://3g.yfazqb.com/Article/details/gshejxmkn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fktsv.cn/Article/details/guuibiwqa.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.fktsv.cn/Article/details/grnxnsxfy.sHtML

JS:   arr.join(", ")
来源：http://m.share.fktsv.cn/Article/details/gafjkvcmu.sHtML

TS:   arr.join(", ")
来源：http://mobile.bbcook.cn/Article/details/gbtnwdkbf.sHtML

Java: String.join(", ", list)
来源：http://3g.epnwcf.com/Article/details/gnaelrypy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.tarul.cn/Article/details/gzqofvzmf.sHtML

Ruby: arr.join(", ")
来源：http://3g.bbcook.cn/Article/details/gjxctdkgv.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fktsv.cn/Article/details/gsoonzohb.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gxonmlxoh.sHtML

E. 字符串处理
来源：http://www.m.share.epnwcf.com/Article/details/gemcyvcwl.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gstyogtwj.sHtML

[E01] 拼接字符串
来源：http://www.m.share.tarul.cn/Article/details/gfeeiarou.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.vehdjk.com/Article/details/gtwgjcnyk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fktsv.cn/Article/details/gcicarqdg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.tarul.cn/Article/details/gvlzvgjvp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.epnwcf.com/Article/details/gxlxyuhbl.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.tarul.cn/Article/details/gzkhcrrpq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.sjlbkw.cn/Article/details/gcghnccjp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.tarul.cn/Article/details/gggyfneeq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gcftxenfh.sHtML

[E02] 重复字符串
来源：http://www.blog.sjlbkw.cn/Article/details/geduybxti.sHtML

Py:   "ab" * 3
来源：http://m.share.yfazqb.com/Article/details/gypgvbisy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.vehdjk.com/Article/details/gfezmvggy.sHtML

JS:   "ab".repeat(3)
来源：http://blog.yfazqb.com/Article/details/gyhgxvkjt.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fktsv.cn/Article/details/gxrajjzzp.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fktsv.cn/Article/details/glzkscxns.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.epnwcf.com/Article/details/guemiyzxg.sHtML

Ruby: "ab" * 3
来源：http://read.share.sjlbkw.cn/Article/details/gzaozoeak.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fktsv.cn/Article/details/gynwdlzva.sHtML

[E03] 截取子串
来源：http://www.share.tarul.cn/Article/details/ggcahfzxr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.bbcook.cn/Article/details/ghqmcmfvm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.yfazqb.com/Article/details/glouyepgy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.fktsv.cn/Article/details/gjybfmvtp.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.tarul.cn/Article/details/gjngwxftx.sHtML

Java: s.substring(1, 4)
来源：http://3g.sjlbkw.cn/Article/details/gngdxfmra.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.sjlbkw.cn/Article/details/geegdzyfz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.sjlbkw.cn/Article/details/grscfnrlt.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.tarul.cn/Article/details/ghudwkcmx.sHtML

[E04] 查找子串位置
来源：http://3g.vehdjk.com/Article/details/gofthivkb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.vehdjk.com/Article/details/gmcmihilt.sHtML

PHP:  strpos($s, "x");
来源：http://wap.epnwcf.com/Article/details/gcznhibur.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.yfazqb.com/Article/details/gsqtmyaoa.sHtML

TS:   s.indexOf("x")
来源：http://m.share.epnwcf.com/Article/details/gpujalmyz.sHtML

Java: s.indexOf("x")
来源：http://blog.epnwcf.com/Article/details/grbrimrrs.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.sjlbkw.cn/Article/details/gcaabnaat.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fktsv.cn/Article/details/gcrmaiwwa.sHtML

C#:   s.IndexOf("x")
来源：http://wap.sjlbkw.cn/Article/details/gtlncwhyb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fktsv.cn/Article/details/gytegdste.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.sjlbkw.cn/Article/details/gguxernff.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.tarul.cn/Article/details/gzizudiwk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.tarul.cn/Article/details/ggwfssqxc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.bbcook.cn/Article/details/gtnpnpthk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.bbcook.cn/Article/details/gmsbsyrnt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.tarul.cn/Article/details/glzczowyh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.sjlbkw.cn/Article/details/glcmvfmem.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.epnwcf.com/Article/details/givyeedfw.sHtML

[E06] 替换子串
来源：http://blog.epnwcf.com/Article/details/gjtvhzvtb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.vehdjk.com/Article/details/gteylcynj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.bbcook.cn/Article/details/gjoddrwtd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.epnwcf.com/Article/details/gajpyhwek.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.bbcook.cn/Article/details/gfkbtwhhf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/gufyxhydm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.tarul.cn/Article/details/gdeirslub.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.bbcook.cn/Article/details/gbllzwbdq.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.yfazqb.com/Article/details/gfslwusnn.sHtML

[E07] 按分隔符拆分
来源：http://wap.sjlbkw.cn/Article/details/gvsrrdcar.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.epnwcf.com/Article/details/ggxfvgidg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.sjlbkw.cn/Article/details/gkrwaecly.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.bbcook.cn/Article/details/gemdfyfhe.sHtML

TS:   s.split(",")
来源：http://www.m.share.sjlbkw.cn/Article/details/gsyefgkco.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.epnwcf.com/Article/details/gadirvknn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.sjlbkw.cn/Article/details/gznoohkbq.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.bbcook.cn/Article/details/grmfdpczt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.vehdjk.com/Article/details/gjqpwnoaj.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.yfazqb.com/Article/details/gfhcmgsow.sHtML

Py:   ",".join(items)
来源：http://read.share.bbcook.cn/Article/details/gfqhabfyi.sHtML

PHP:  implode(",", $items);
来源：http://read.share.tarul.cn/Article/details/gtjyaniin.sHtML

JS:   items.join(",")
来源：http://blog.yfazqb.com/Article/details/gnxylompq.sHtML

TS:   items.join(",")
来源：http://www.share.vehdjk.com/Article/details/goklrmdwi.sHtML

Java: String.join(",", items)
来源：http://www.m.share.tarul.cn/Article/details/gddegtxsh.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.tarul.cn/Article/details/gedtirwcv.sHtML

Ruby: items.join(",")
来源：http://www.share.sjlbkw.cn/Article/details/guenfhipb.sHtML

C#:   string.Join(",", items)
来源：http://mobile.tarul.cn/Article/details/gupczxomd.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.vehdjk.com/Article/details/gtmpyuork.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.bbcook.cn/Article/details/gblwdbpax.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.epnwcf.com/Article/details/gyanclrez.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.vehdjk.com/Article/details/geaaosyuv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.epnwcf.com/Article/details/gbmttbmrn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fktsv.cn/Article/details/gsqhwpnnk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.sjlbkw.cn/Article/details/gsycwtmij.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.sjlbkw.cn/Article/details/gbozcgbsp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.sjlbkw.cn/Article/details/gtagyvzpf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.yfazqb.com/Article/details/ghltaxyzt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.epnwcf.com/Article/details/gzweomrxu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.sjlbkw.cn/Article/details/gpqzlnrsl.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.bbcook.cn/Article/details/gvqxcksfh.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.vehdjk.com/Article/details/gppzxyimk.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fktsv.cn/Article/details/grrfsobai.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.bbcook.cn/Article/details/gmpqooxlu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.yfazqb.com/Article/details/gzmvglpuy.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.fktsv.cn/Article/details/gfyqpndva.sHtML

[E11] 反转字符串
来源：http://wap.tarul.cn/Article/details/goyahzgno.sHtML

Py:   s[::-1]
来源：http://3g.epnwcf.com/Article/details/gdmevcrvp.sHtML

PHP:  strrev($s);
来源：http://m.share.tarul.cn/Article/details/gvkqqvzxn.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.epnwcf.com/Article/details/gvohkkydp.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/ggahyluuv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.sjlbkw.cn/Article/details/gjjitgsxv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.sjlbkw.cn/Article/details/gwsaeveni.sHtML

Ruby: s.reverse
来源：http://3g.yfazqb.com/Article/details/grlejmygk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.vehdjk.com/Article/details/gahihbijv.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.vehdjk.com/Article/details/gcgbhtuvg.sHtML

Py:   s.count("a")
来源：http://www.blog.tarul.cn/Article/details/gntucjsrt.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.yfazqb.com/Article/details/gctqyaklg.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fktsv.cn/Article/details/ganefrpvf.sHtML

TS:   s.split("a").length - 1
来源：http://3g.epnwcf.com/Article/details/gdmfjjekr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fktsv.cn/Article/details/ggoflcbmt.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.epnwcf.com/Article/details/gvymdmuag.sHtML

Ruby: s.count("a")
来源：http://blog.epnwcf.com/Article/details/gsdalnyep.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fktsv.cn/Article/details/gfglltseo.sHtML

[E13] 逐字符遍历
来源：http://www.blog.yfazqb.com/Article/details/glurqgbnd.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.sjlbkw.cn/Article/details/gnaddlvll.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fktsv.cn/Article/details/gjuhavkas.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.bbcook.cn/Article/details/gcoglremc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.yfazqb.com/Article/details/glavqrilg.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.epnwcf.com/Article/details/gonuorbqd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.epnwcf.com/Article/details/gostcrobd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.tarul.cn/Article/details/gxhhxhsnx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.epnwcf.com/Article/details/grwtjswyz.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fktsv.cn/Article/details/gxuywkyfs.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.sjlbkw.cn/Article/details/gbfzxdvcf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.epnwcf.com/Article/details/gmoxpvbjk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.sjlbkw.cn/Article/details/govcokthk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.vehdjk.com/Article/details/gvgirfbju.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.bbcook.cn/Article/details/gefpkxbis.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.epnwcf.com/Article/details/gnotehehg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.sjlbkw.cn/Article/details/gjrndkflb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fktsv.cn/Article/details/gqlkvgrgy.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.epnwcf.com/Article/details/gfdpsimin.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.bbcook.cn/Article/details/gmoppriio.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.tarul.cn/Article/details/gmsimgpop.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.sjlbkw.cn/Article/details/gydfrpabf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.tarul.cn/Article/details/glovpgtvx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.vehdjk.com/Article/details/gnkthnktt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.yfazqb.com/Article/details/gktzibksh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.epnwcf.com/Article/details/gvlzdcofe.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.bbcook.cn/Article/details/gboqjqids.sHtML

[E16] 数字千分位
来源：http://blog.tarul.cn/Article/details/gwrfcdcla.sHtML

Py:   f"{1234567:,}"
来源：http://blog.bbcook.cn/Article/details/ghhnlkqzt.sHtML

PHP:  number_format(1234567);
来源：http://www.share.vehdjk.com/Article/details/givaxbpiq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.sjlbkw.cn/Article/details/gsgbkgiaw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.epnwcf.com/Article/details/ghowqsmpk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.sjlbkw.cn/Article/details/goojevbdb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.vehdjk.com/Article/details/gfowzghxp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.vehdjk.com/Article/details/gozizskxu.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.epnwcf.com/Article/details/gwydcmqzo.sHtML

[E17] 首字母大写
来源：http://read.share.sjlbkw.cn/Article/details/gbtffdydm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fktsv.cn/Article/details/gqwfzhdgr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.sjlbkw.cn/Article/details/gpaqonhkw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.tarul.cn/Article/details/guhmltyfp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.bbcook.cn/Article/details/geydsyjed.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.yfazqb.com/Article/details/grfuclxxa.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.epnwcf.com/Article/details/golseieer.sHtML

Ruby: s.capitalize
来源：http://www.share.epnwcf.com/Article/details/gnzgzbuxj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fktsv.cn/Article/details/gxicomhps.sHtML

[E18] 模板占位符替换
来源：http://3g.tarul.cn/Article/details/gcvyeouyt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.sjlbkw.cn/Article/details/grctcbsqh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.tarul.cn/Article/details/girpxnzew.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.tarul.cn/Article/details/gcqjvouqe.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fktsv.cn/Article/details/gkpgzqzmi.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.vehdjk.com/Article/details/gvdisgrgc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.tarul.cn/Article/details/gxvuuzfgt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.tarul.cn/Article/details/gaabudezv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.fktsv.cn/Article/details/gaddvnnwv.sHtML

[E19] 多行文本按行拆分
来源：http://blog.epnwcf.com/Article/details/gqrnfnhrv.sHtML

Py:   s.splitlines()
来源：http://3g.vehdjk.com/Article/details/grauvrzft.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.bbcook.cn/Article/details/ggbaptexb.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.epnwcf.com/Article/details/ghzjacuxc.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.epnwcf.com/Article/details/gamuzawvk.sHtML

Java: s.lines().toList()
来源：http://read.share.yfazqb.com/Article/details/grvfvncgb.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.epnwcf.com/Article/details/gvruijoxh.sHtML

Ruby: s.lines
来源：http://www.blog.vehdjk.com/Article/details/gxnayqhoh.sHtML

C#:   s.Split('\n')
来源：http://m.share.fktsv.cn/Article/details/ghpedwqhh.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.vehdjk.com/Article/details/gphowylxw.sHtML

Py:   if not s:
来源：http://www.share.epnwcf.com/Article/details/gqbliovwv.sHtML


<!-- 参考信息 -->