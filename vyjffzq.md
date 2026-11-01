代发 wailian999

C#:   list.Reverse();
来源：http://mobile.vehdjk.com/Article/details/gjbuqaaey.sHtML

[D12] 查找元素下标
来源：http://www.m.share.epnwcf.com/Article/details/gvtfqahwf.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.epnwcf.com/Article/details/gksmjqeeo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.bbcook.cn/Article/details/gtdqivlca.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.tarul.cn/Article/details/goobryqyx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.tarul.cn/Article/details/gqquagwae.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.bbcook.cn/Article/details/gsghyzkoa.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.bbcook.cn/Article/details/gpgavcbsr.sHtML

Ruby: arr.index(x)
来源：http://mobile.yfazqb.com/Article/details/gwezylymc.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fktsv.cn/Article/details/govsokxjs.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fktsv.cn/Article/details/geaboodeo.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.yfazqb.com/Article/details/gwofvkpar.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.sjlbkw.cn/Article/details/gjkdxucjo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fktsv.cn/Article/details/gqvioydwg.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.vehdjk.com/Article/details/grlfenplt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.sjlbkw.cn/Article/details/gstfxyaws.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.vehdjk.com/Article/details/gvclssbtx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.vehdjk.com/Article/details/grocoonag.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.yfazqb.com/Article/details/gqbwtvkgs.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.vehdjk.com/Article/details/gvmoqufal.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.sjlbkw.cn/Article/details/glkgelwox.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.tarul.cn/Article/details/gjcndweni.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.vehdjk.com/Article/details/gdujdvogc.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.tarul.cn/Article/details/gqyuzyscn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.tarul.cn/Article/details/gorylnfah.sHtML

Go:   // 手写循环
来源：http://www.blog.sjlbkw.cn/Article/details/grndtxdiv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/gombgujft.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.epnwcf.com/Article/details/gmgehpzez.sHtML

[D15] 去重
来源：http://www.blog.tarul.cn/Article/details/gkjfhlzem.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.tarul.cn/Article/details/gunhgirig.sHtML

PHP:  array_unique($arr);
来源：http://3g.vehdjk.com/Article/details/gmvlomgcn.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.yfazqb.com/Article/details/gliusrnak.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.vehdjk.com/Article/details/gfgswrstw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.epnwcf.com/Article/details/ggcaduatx.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.tarul.cn/Article/details/gqczxpnhx.sHtML

Ruby: arr.uniq
来源：http://mobile.fktsv.cn/Article/details/getwowjuh.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.vehdjk.com/Article/details/grbharkuv.sHtML

[D16] 求和与平均值
来源：http://www.blog.bbcook.cn/Article/details/gbsflwbcv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.tarul.cn/Article/details/gyeatfqyy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.yfazqb.com/Article/details/grstzmibr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.tarul.cn/Article/details/gaeoswnss.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/goxmohryv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fktsv.cn/Article/details/gdhymgtwv.sHtML

Go:   // 手写循环累加
来源：http://m.share.epnwcf.com/Article/details/grrhfhwwo.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.epnwcf.com/Article/details/gthqytrjg.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.epnwcf.com/Article/details/gprcwuawn.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.tarul.cn/Article/details/grqrcjnom.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.yfazqb.com/Article/details/ggmjorrtt.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.bbcook.cn/Article/details/gkfhesajb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fktsv.cn/Article/details/gxkiaixni.sHtML

TS:   Math.max(...arr);
来源：http://mobile.tarul.cn/Article/details/gfpvmdkxm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.vehdjk.com/Article/details/gugufhbib.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.vehdjk.com/Article/details/groftyern.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fktsv.cn/Article/details/gqvrgbaln.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.epnwcf.com/Article/details/gvgjlrhzv.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.yfazqb.com/Article/details/gaihwbwpw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fktsv.cn/Article/details/gwkadgelg.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.yfazqb.com/Article/details/gkukryyfv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.bbcook.cn/Article/details/grixxhopq.sHtML

TS:   nested.flat();
来源：http://3g.bbcook.cn/Article/details/gimrcwwhd.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.vehdjk.com/Article/details/gmcuszgkq.sHtML

Go:   // 手写双层循环
来源：http://baike.fktsv.cn/Article/details/grtbwytww.sHtML

Ruby: nested.flatten
来源：http://3g.yfazqb.com/Article/details/gcmqaeyyt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.epnwcf.com/Article/details/gtxxwnndk.sHtML

[D19] 按字段分组
来源：http://mobile.bbcook.cn/Article/details/gpyxmleua.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.sjlbkw.cn/Article/details/gmrpzxqsy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.bbcook.cn/Article/details/gowwqielo.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.vehdjk.com/Article/details/gcoapdkum.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.bbcook.cn/Article/details/glmijwvzp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.epnwcf.com/Article/details/gwcvsvboi.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.tarul.cn/Article/details/gtwxvoaqc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.tarul.cn/Article/details/gofepakzu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.bbcook.cn/Article/details/gxepymdmm.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.tarul.cn/Article/details/gwwritwkg.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gatunkexi.sHtML

PHP:  array_count_values($arr);
来源：http://3g.sjlbkw.cn/Article/details/grvgaknuc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.bbcook.cn/Article/details/gybjpwfou.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.sjlbkw.cn/Article/details/gvtaprnza.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.epnwcf.com/Article/details/gjtyxdbic.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fktsv.cn/Article/details/gjxocncuc.sHtML

Ruby: arr.tally
来源：http://www.blog.fktsv.cn/Article/details/gglokykvh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.tarul.cn/Article/details/gurhkcbyo.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.vehdjk.com/Article/details/gwvngmfnq.sHtML

Py:   x in arr
来源：http://blog.yfazqb.com/Article/details/ggslayare.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.bbcook.cn/Article/details/gqzwvhpri.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fktsv.cn/Article/details/ghcncedjd.sHtML

TS:   arr.includes(x)
来源：http://mobile.sjlbkw.cn/Article/details/gongrgyno.sHtML

Java: list.contains(x)
来源：http://www.m.share.epnwcf.com/Article/details/gstjzyitz.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/gnalugrbu.sHtML

Ruby: arr.include?(x)
来源：http://3g.tarul.cn/Article/details/gvuoxugvx.sHtML

C#:   list.Contains(x)
来源：http://read.share.bbcook.cn/Article/details/gtgocbdra.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.bbcook.cn/Article/details/gjgjecbir.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fktsv.cn/Article/details/gbvapwgwn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.vehdjk.com/Article/details/gdluuouls.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.sjlbkw.cn/Article/details/gfyiafexs.sHtML

TS:   [...arr];
来源：http://www.m.share.vehdjk.com/Article/details/gwdpfairb.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.sjlbkw.cn/Article/details/gfahpzqoy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fktsv.cn/Article/details/gsgwypebt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.sjlbkw.cn/Article/details/ganviwsfp.sHtML

C#:   new List<int>(list);
来源：http://baike.vehdjk.com/Article/details/gvuthuaaa.sHtML

[D23] reduce 累积计算
来源：http://www.blog.tarul.cn/Article/details/gtlqaauty.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.epnwcf.com/Article/details/gzytihdma.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.tarul.cn/Article/details/gvxokmupc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gkclqapns.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.sjlbkw.cn/Article/details/gawddiluz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.vehdjk.com/Article/details/gjlfvhwld.sHtML

Go:   // 手写循环
来源：http://blog.vehdjk.com/Article/details/gkquhexgw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fktsv.cn/Article/details/gxmeeuupq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.bbcook.cn/Article/details/gcucuiekd.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fktsv.cn/Article/details/ghjzwdstn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.yfazqb.com/Article/details/ginllbpfl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.bbcook.cn/Article/details/gubrjndvg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.epnwcf.com/Article/details/gqhvrxkmm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.vehdjk.com/Article/details/gjoabflwt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fktsv.cn/Article/details/gwxrqdrfe.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.sjlbkw.cn/Article/details/grtfurpbf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.epnwcf.com/Article/details/gphmriqgj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fktsv.cn/Article/details/grnsqirjx.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.yfazqb.com/Article/details/gfnhcgpow.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fktsv.cn/Article/details/gllhcahxj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.bbcook.cn/Article/details/gxybrmzcn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.epnwcf.com/Article/details/glmrvrdwj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.tarul.cn/Article/details/ghisoglcz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fktsv.cn/Article/details/gzmutzilp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.epnwcf.com/Article/details/gayjbibri.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gauaddgym.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.yfazqb.com/Article/details/gvipewlau.sHtML

[D26] 数组转字符串
来源：http://www.share.bbcook.cn/Article/details/gcjgozhyk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.vehdjk.com/Article/details/gtxpgfgvx.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.yfazqb.com/Article/details/gcthkxbyy.sHtML

JS:   arr.join(", ")
来源：http://www.share.epnwcf.com/Article/details/gtmrolnlm.sHtML

TS:   arr.join(", ")
来源：http://www.share.bbcook.cn/Article/details/gjciamyop.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.bbcook.cn/Article/details/gfohxmmlv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.tarul.cn/Article/details/gdykknxqp.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghpteipnw.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.vehdjk.com/Article/details/gluasncbl.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gaibcozfb.sHtML

E. 字符串处理
来源：http://www.blog.epnwcf.com/Article/details/gqfwvdywx.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gxecrqheo.sHtML

[E01] 拼接字符串
来源：http://m.share.yfazqb.com/Article/details/gqwmkrtee.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.sjlbkw.cn/Article/details/gkhatalbf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.sjlbkw.cn/Article/details/gbvrednan.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.sjlbkw.cn/Article/details/gmijghlsd.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.epnwcf.com/Article/details/gqafdhdyk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.epnwcf.com/Article/details/gbairojrf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.epnwcf.com/Article/details/gkfaeplpj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.bbcook.cn/Article/details/gknmqvssx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gocupgbnh.sHtML

[E02] 重复字符串
来源：http://www.m.share.epnwcf.com/Article/details/gixrreljv.sHtML

Py:   "ab" * 3
来源：http://www.share.fktsv.cn/Article/details/gxrwprhsz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.tarul.cn/Article/details/gjvczbuay.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.epnwcf.com/Article/details/gfyfxsada.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fktsv.cn/Article/details/gllohuaaz.sHtML

Java: "ab".repeat(3)
来源：http://blog.tarul.cn/Article/details/gmrnreuuc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fktsv.cn/Article/details/gnaiasntk.sHtML

Ruby: "ab" * 3
来源：http://3g.yfazqb.com/Article/details/gaztnsaqb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.yfazqb.com/Article/details/gfghkjlvi.sHtML

[E03] 截取子串
来源：http://m.share.sjlbkw.cn/Article/details/gmjtfdupk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fktsv.cn/Article/details/gfolizcym.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fktsv.cn/Article/details/gfkmauyib.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fktsv.cn/Article/details/gliobxnqg.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.bbcook.cn/Article/details/glpaffkro.sHtML

Java: s.substring(1, 4)
来源：http://mobile.yfazqb.com/Article/details/gtkjxccju.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.vehdjk.com/Article/details/ghpkhrdvm.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.vehdjk.com/Article/details/ghbdkuitd.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fktsv.cn/Article/details/gipecownw.sHtML

[E04] 查找子串位置
来源：http://wap.bbcook.cn/Article/details/gcplcojan.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.tarul.cn/Article/details/gtvlmnivs.sHtML

PHP:  strpos($s, "x");
来源：http://3g.sjlbkw.cn/Article/details/gfbhggehw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.tarul.cn/Article/details/gmbnntjto.sHtML

TS:   s.indexOf("x")
来源：http://mobile.sjlbkw.cn/Article/details/gdnmvmlzg.sHtML

Java: s.indexOf("x")
来源：http://baike.tarul.cn/Article/details/gxhphcgbm.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.bbcook.cn/Article/details/gadptxosk.sHtML

Ruby: s.index("x")
来源：http://www.share.epnwcf.com/Article/details/gtkciyvmp.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.sjlbkw.cn/Article/details/gupbhslca.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.epnwcf.com/Article/details/gorxpbres.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmmcgitez.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.yfazqb.com/Article/details/gipyedtud.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.yfazqb.com/Article/details/gruhykxha.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.tarul.cn/Article/details/gbwhvnjqj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.vehdjk.com/Article/details/ggthxyhxw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.vehdjk.com/Article/details/gibecjvhv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.yfazqb.com/Article/details/gzldpwnqe.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.tarul.cn/Article/details/ggcvtvukd.sHtML

[E06] 替换子串
来源：http://mobile.sjlbkw.cn/Article/details/gihkjtvfm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.sjlbkw.cn/Article/details/gnoypqlun.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.yfazqb.com/Article/details/gmmzahxgj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.bbcook.cn/Article/details/gypnzvric.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.vehdjk.com/Article/details/gsyahcpgf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.sjlbkw.cn/Article/details/guawnjpqa.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.vehdjk.com/Article/details/guovafzln.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.tarul.cn/Article/details/gwxmpdjyg.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.bbcook.cn/Article/details/gzqflaqbc.sHtML

[E07] 按分隔符拆分
来源：http://blog.yfazqb.com/Article/details/gvkwpndat.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fktsv.cn/Article/details/gmksmqioj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.vehdjk.com/Article/details/gsrcbdczh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.epnwcf.com/Article/details/glfgjvyaw.sHtML

TS:   s.split(",")
来源：http://www.share.tarul.cn/Article/details/gxvbtftgz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.epnwcf.com/Article/details/gccpptepr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fktsv.cn/Article/details/govppobcc.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.tarul.cn/Article/details/geblgfdzr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.vehdjk.com/Article/details/gciymtufs.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.tarul.cn/Article/details/gbabqxjqr.sHtML

Py:   ",".join(items)
来源：http://read.share.yfazqb.com/Article/details/gwqoqcocy.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.epnwcf.com/Article/details/gzziwtqdq.sHtML

JS:   items.join(",")
来源：http://baike.epnwcf.com/Article/details/gyigywxkv.sHtML

TS:   items.join(",")
来源：http://m.share.vehdjk.com/Article/details/gzpqjdzyo.sHtML

Java: String.join(",", items)
来源：http://baike.yfazqb.com/Article/details/gwickkopd.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.tarul.cn/Article/details/gydekexpw.sHtML

Ruby: items.join(",")
来源：http://baike.tarul.cn/Article/details/grulqydzn.sHtML

C#:   string.Join(",", items)
来源：http://wap.vehdjk.com/Article/details/gmfxchfzc.sHtML

[E09] 去除所有空白字符
来源：http://mobile.sjlbkw.cn/Article/details/gyfjonhrx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.epnwcf.com/Article/details/gzfqdboxo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.yfazqb.com/Article/details/gtgjazoiu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.tarul.cn/Article/details/gardikztw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.yfazqb.com/Article/details/gjtdppsaa.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.bbcook.cn/Article/details/gbbklmbce.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fktsv.cn/Article/details/gmqspvunv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.epnwcf.com/Article/details/gwzuwpvgl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.bbcook.cn/Article/details/gtnmxjtzn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.sjlbkw.cn/Article/details/ggfwnkemw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fktsv.cn/Article/details/guvxykzmc.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.vehdjk.com/Article/details/gfoakkjag.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.vehdjk.com/Article/details/gmzvumxzg.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.tarul.cn/Article/details/gudyloonn.sHtML

Java: String.format("%03d", 7)
来源：http://blog.epnwcf.com/Article/details/gwgfvohqb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.bbcook.cn/Article/details/gwqtdhaze.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.vehdjk.com/Article/details/gbrgnflby.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.sjlbkw.cn/Article/details/gfaphjaae.sHtML

[E11] 反转字符串
来源：http://3g.fktsv.cn/Article/details/gfqrxfpuy.sHtML

Py:   s[::-1]
来源：http://mobile.fktsv.cn/Article/details/gzkuppkqw.sHtML

PHP:  strrev($s);
来源：http://www.share.tarul.cn/Article/details/gqgndvhkv.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gmhawguat.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.tarul.cn/Article/details/gwoibezco.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.sjlbkw.cn/Article/details/gungafjrz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fktsv.cn/Article/details/gofdofvcr.sHtML

Ruby: s.reverse
来源：http://wap.bbcook.cn/Article/details/gfjvbnlsh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.sjlbkw.cn/Article/details/gbzavcvyr.sHtML

[E12] 统计某字符出现次数
来源：http://3g.sjlbkw.cn/Article/details/gypcunfxe.sHtML

Py:   s.count("a")
来源：http://blog.fktsv.cn/Article/details/grqxomixo.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.tarul.cn/Article/details/gerxskscg.sHtML

JS:   s.split("a").length - 1
来源：http://3g.sjlbkw.cn/Article/details/gfuhrldzr.sHtML

TS:   s.split("a").length - 1
来源：http://blog.tarul.cn/Article/details/gfejpnpdk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.vehdjk.com/Article/details/grkfikkxi.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.bbcook.cn/Article/details/gwdsmfjmb.sHtML

Ruby: s.count("a")
来源：http://www.share.vehdjk.com/Article/details/gllsyuged.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.tarul.cn/Article/details/gmsbmbsnk.sHtML

[E13] 逐字符遍历
来源：http://www.share.tarul.cn/Article/details/gfvbibpwg.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.yfazqb.com/Article/details/gtyezrjin.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.tarul.cn/Article/details/gcapercjd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.tarul.cn/Article/details/govrbaafm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fktsv.cn/Article/details/gnqcydypj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.epnwcf.com/Article/details/gnjxrplqm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.vehdjk.com/Article/details/glekeuvkn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.epnwcf.com/Article/details/gjjaejarq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.tarul.cn/Article/details/gkwxgtpgj.sHtML

[E14] URL 编码与 Base64
来源：http://baike.bbcook.cn/Article/details/gwqwnwubs.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.tarul.cn/Article/details/gfuprxvci.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.epnwcf.com/Article/details/gsyitdbir.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.bbcook.cn/Article/details/gxmvlqwhu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.vehdjk.com/Article/details/gazaogdol.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.yfazqb.com/Article/details/gyyvwkvkm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.yfazqb.com/Article/details/gbibafshh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.epnwcf.com/Article/details/grxfiesfs.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.bbcook.cn/Article/details/gwbpyveoj.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.bbcook.cn/Article/details/glivgvkww.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.vehdjk.com/Article/details/gxwnbnqte.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fktsv.cn/Article/details/gqvganhgk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.yfazqb.com/Article/details/gzpcrjplp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.yfazqb.com/Article/details/grnyxbwhu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fktsv.cn/Article/details/gxjtppcfs.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.tarul.cn/Article/details/gedwnellh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.yfazqb.com/Article/details/gabtsrcgg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.bbcook.cn/Article/details/gkuibdptl.sHtML

[E16] 数字千分位
来源：http://m.share.epnwcf.com/Article/details/guwkgdlgf.sHtML

Py:   f"{1234567:,}"
来源：http://3g.sjlbkw.cn/Article/details/gaifqoowu.sHtML

PHP:  number_format(1234567);
来源：http://3g.yfazqb.com/Article/details/gmdybbfzo.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.yfazqb.com/Article/details/gnhomffkn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.vehdjk.com/Article/details/gtxhljfnv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.bbcook.cn/Article/details/gsxssokcu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.tarul.cn/Article/details/gcdmnrjrl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.bbcook.cn/Article/details/glompyoma.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.vehdjk.com/Article/details/gyobofphi.sHtML

[E17] 首字母大写
来源：http://www.blog.fktsv.cn/Article/details/gstmygpzt.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.sjlbkw.cn/Article/details/guqcehyjp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fktsv.cn/Article/details/grdwktmid.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.yfazqb.com/Article/details/gkqptcjfb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fktsv.cn/Article/details/grtlsxnwr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fktsv.cn/Article/details/gkicctkcg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.epnwcf.com/Article/details/gtpyjefsx.sHtML

Ruby: s.capitalize
来源：http://m.share.vehdjk.com/Article/details/gwsjyqlgg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fktsv.cn/Article/details/gjdkpxcca.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.bbcook.cn/Article/details/gscpxtsmn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.tarul.cn/Article/details/gjfcjwqqk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.bbcook.cn/Article/details/gupphlkpj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.sjlbkw.cn/Article/details/gczydcmgk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fktsv.cn/Article/details/gzwvdfeec.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.bbcook.cn/Article/details/gymwwhqdc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.vehdjk.com/Article/details/gnpjfnaie.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.tarul.cn/Article/details/gfkodaxnt.sHtML


<!-- 参考信息 -->