代发 wailian999

[D11] 反转数组
来源：http://www.m.share.sjlbkw.cn/Article/details/gjyqbavsf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.vehdjk.com/Article/details/gzihzfdhq.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fktsv.cn/Article/details/gjdskiasg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.tarul.cn/Article/details/glkxphauy.sHtML

TS:   [...arr].reverse();
来源：http://read.share.sjlbkw.cn/Article/details/gglobzwte.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fktsv.cn/Article/details/gserozuac.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gpocwsfms.sHtML

Ruby: arr.reverse
来源：http://www.share.bbcook.cn/Article/details/gwarqxjgw.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fktsv.cn/Article/details/gcefigqro.sHtML

[D12] 查找元素下标
来源：http://www.blog.fktsv.cn/Article/details/glhtmbkwq.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.bbcook.cn/Article/details/gaijnokcq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.bbcook.cn/Article/details/gsugrxmtr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.yfazqb.com/Article/details/gmcukuikg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fktsv.cn/Article/details/gyxbyucxd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.fktsv.cn/Article/details/gmvldfrzj.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.bbcook.cn/Article/details/gcurerwcf.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.tarul.cn/Article/details/gjklmopmv.sHtML

C#:   list.IndexOf(x);
来源：http://3g.sjlbkw.cn/Article/details/gvupgmlhx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fktsv.cn/Article/details/gfmbhzfem.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fktsv.cn/Article/details/gonhrohld.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.epnwcf.com/Article/details/gnzwrolgk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.tarul.cn/Article/details/gyuzsgyiz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.sjlbkw.cn/Article/details/gtedehffw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.epnwcf.com/Article/details/gqeimghnw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.bbcook.cn/Article/details/gjpyjhabn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fktsv.cn/Article/details/ggjsykxyd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/ghtqtztke.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.epnwcf.com/Article/details/gxvlvbxrr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.epnwcf.com/Article/details/gtkttlryq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.sjlbkw.cn/Article/details/gjgberqqt.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fktsv.cn/Article/details/ggzrnzowm.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.bbcook.cn/Article/details/gdxtqtkwh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.epnwcf.com/Article/details/gbkutqqru.sHtML

Go:   // 手写循环
来源：http://mobile.fktsv.cn/Article/details/gwzmaeioi.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.epnwcf.com/Article/details/guxhyyyrl.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.vehdjk.com/Article/details/grqkbfbku.sHtML

[D15] 去重
来源：http://wap.fktsv.cn/Article/details/gygdmodln.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.bbcook.cn/Article/details/gmvtmckin.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.epnwcf.com/Article/details/geqzlrdts.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fktsv.cn/Article/details/gsiznjijs.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.yfazqb.com/Article/details/guodrjsuf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.sjlbkw.cn/Article/details/gtkvfocah.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.epnwcf.com/Article/details/gipgwewpp.sHtML

Ruby: arr.uniq
来源：http://mobile.yfazqb.com/Article/details/giqpewqid.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.sjlbkw.cn/Article/details/guqakahvw.sHtML

[D16] 求和与平均值
来源：http://wap.epnwcf.com/Article/details/gvalqoqad.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fktsv.cn/Article/details/gwchnubrf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.bbcook.cn/Article/details/gmkkvxbbf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.yfazqb.com/Article/details/girtivkcy.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.bbcook.cn/Article/details/gfmxpgocp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.epnwcf.com/Article/details/gacibktlv.sHtML

Go:   // 手写循环累加
来源：http://read.share.vehdjk.com/Article/details/gelfblypb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.epnwcf.com/Article/details/gdtpswtep.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.vehdjk.com/Article/details/gnkipeyep.sHtML

[D17] 最大值与最小值
来源：http://mobile.tarul.cn/Article/details/grdlineyk.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.bbcook.cn/Article/details/gswuopwsy.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.tarul.cn/Article/details/glqyiiksg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.vehdjk.com/Article/details/gmszeiaue.sHtML

TS:   Math.max(...arr);
来源：http://www.share.vehdjk.com/Article/details/gsmwfcygn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.tarul.cn/Article/details/ggyasjdoz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.vehdjk.com/Article/details/guhxhusae.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.tarul.cn/Article/details/gbmajvtgv.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.epnwcf.com/Article/details/gfjguwsnt.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.sjlbkw.cn/Article/details/gfpginylt.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.tarul.cn/Article/details/gdokdrjuz.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.epnwcf.com/Article/details/gqqtlulnk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.vehdjk.com/Article/details/gahrzqssq.sHtML

TS:   nested.flat();
来源：http://www.blog.vehdjk.com/Article/details/gsdcbnfls.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.yfazqb.com/Article/details/glicndegm.sHtML

Go:   // 手写双层循环
来源：http://blog.fktsv.cn/Article/details/grcmrfeyy.sHtML

Ruby: nested.flatten
来源：http://m.share.epnwcf.com/Article/details/gjugoiqxs.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.bbcook.cn/Article/details/gvinxekrv.sHtML

[D19] 按字段分组
来源：http://www.blog.vehdjk.com/Article/details/gmdbwovln.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fktsv.cn/Article/details/gykbpdkrg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.bbcook.cn/Article/details/gdmejsqjs.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.bbcook.cn/Article/details/gvdlrccqa.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.epnwcf.com/Article/details/gipmkxhxv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.sjlbkw.cn/Article/details/gopgezzce.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fktsv.cn/Article/details/gtnucrmum.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.tarul.cn/Article/details/geuujxkii.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.vehdjk.com/Article/details/guizwcjwf.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.yfazqb.com/Article/details/gcixhyqqn.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gyktqzvwt.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gtmylighz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.epnwcf.com/Article/details/grkhdaapz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.epnwcf.com/Article/details/gehjgabpx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.vehdjk.com/Article/details/gketbthnm.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.tarul.cn/Article/details/gogorrsnr.sHtML

Ruby: arr.tally
来源：http://www.m.share.epnwcf.com/Article/details/gajimjcai.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fktsv.cn/Article/details/gcemrpfyx.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.vehdjk.com/Article/details/gmdbuyjmk.sHtML

Py:   x in arr
来源：http://www.share.epnwcf.com/Article/details/gynhixqmj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.tarul.cn/Article/details/gjdixvotn.sHtML

JS:   arr.includes(x)
来源：http://baike.vehdjk.com/Article/details/gloamuixa.sHtML

TS:   arr.includes(x)
来源：http://3g.vehdjk.com/Article/details/gjnhrspua.sHtML

Java: list.contains(x)
来源：http://www.blog.fktsv.cn/Article/details/gmrcowgcs.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/geznlnvfd.sHtML

Ruby: arr.include?(x)
来源：http://3g.epnwcf.com/Article/details/gqqxitpqp.sHtML

C#:   list.Contains(x)
来源：http://www.share.sjlbkw.cn/Article/details/gfgqnhggt.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.epnwcf.com/Article/details/gmurelzsk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.bbcook.cn/Article/details/gumipdihz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.tarul.cn/Article/details/gzvgqqnjt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.epnwcf.com/Article/details/ganznaecw.sHtML

TS:   [...arr];
来源：http://mobile.vehdjk.com/Article/details/gxzxvkqde.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.yfazqb.com/Article/details/gqtjunlfp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fktsv.cn/Article/details/gifugystr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.yfazqb.com/Article/details/gvgtsqtwa.sHtML

C#:   new List<int>(list);
来源：http://baike.yfazqb.com/Article/details/gklfgjiyu.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.vehdjk.com/Article/details/gqggjixui.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.epnwcf.com/Article/details/giltsavlg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fktsv.cn/Article/details/gujtjoaoa.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.yfazqb.com/Article/details/gcbnzhayo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gmxcusfcl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.epnwcf.com/Article/details/giyldhcpx.sHtML

Go:   // 手写循环
来源：http://baike.bbcook.cn/Article/details/gcdvylehm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.bbcook.cn/Article/details/grpzdpprb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.bbcook.cn/Article/details/gecdyxqly.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fktsv.cn/Article/details/gsoiodbko.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fktsv.cn/Article/details/gqvoxnmwe.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.epnwcf.com/Article/details/gnqndfjzv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.vehdjk.com/Article/details/godlhhzpt.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.tarul.cn/Article/details/ghovsaxbx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fktsv.cn/Article/details/grmmunqpf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fktsv.cn/Article/details/gvrbmcaya.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.epnwcf.com/Article/details/gupuiiphs.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.bbcook.cn/Article/details/gnkwquoaq.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.yfazqb.com/Article/details/gsmqhkqog.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.bbcook.cn/Article/details/glrypwqfa.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.sjlbkw.cn/Article/details/glauxylub.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.yfazqb.com/Article/details/gpjinqpco.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fktsv.cn/Article/details/gorvvoqsv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.vehdjk.com/Article/details/gqmtnvteo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.tarul.cn/Article/details/gluuewqea.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.bbcook.cn/Article/details/gzpxyvjfo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.vehdjk.com/Article/details/gnwimyapn.sHtML

[D26] 数组转字符串
来源：http://read.share.vehdjk.com/Article/details/guhtxeqel.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.tarul.cn/Article/details/gpbbcxewu.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.vehdjk.com/Article/details/gpueczvhm.sHtML

JS:   arr.join(", ")
来源：http://read.share.yfazqb.com/Article/details/garlsdhxw.sHtML

TS:   arr.join(", ")
来源：http://mobile.yfazqb.com/Article/details/guqqoefsb.sHtML

Java: String.join(", ", list)
来源：http://m.share.epnwcf.com/Article/details/gbqkkhers.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.tarul.cn/Article/details/giqwxmnqp.sHtML

Ruby: arr.join(", ")
来源：http://baike.vehdjk.com/Article/details/gldiaxfkn.sHtML

C#:   string.Join(", ", list)
来源：http://3g.tarul.cn/Article/details/ghzftnjcp.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gpnimrudh.sHtML

E. 字符串处理
来源：http://read.share.fktsv.cn/Article/details/gtksprhnf.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gvwmqmctt.sHtML

[E01] 拼接字符串
来源：http://wap.yfazqb.com/Article/details/grglpmhbt.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.bbcook.cn/Article/details/grygrxdtr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fktsv.cn/Article/details/gvabdkgip.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.tarul.cn/Article/details/gcnrukspi.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fktsv.cn/Article/details/gwifgiqvz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.epnwcf.com/Article/details/gpqsdjvhb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.epnwcf.com/Article/details/gysayfazw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.tarul.cn/Article/details/gdtfpssjx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.bbcook.cn/Article/details/ggayclfcu.sHtML

[E02] 重复字符串
来源：http://wap.tarul.cn/Article/details/gkxeddimp.sHtML

Py:   "ab" * 3
来源：http://wap.bbcook.cn/Article/details/gnnkrpqdc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.sjlbkw.cn/Article/details/gvxhdlifb.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwpnsblpu.sHtML

TS:   "ab".repeat(3)
来源：http://wap.yfazqb.com/Article/details/gzqgqibwt.sHtML

Java: "ab".repeat(3)
来源：http://baike.yfazqb.com/Article/details/gkveztxha.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.epnwcf.com/Article/details/gwqdskatu.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.epnwcf.com/Article/details/gnubrpnou.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.yfazqb.com/Article/details/gqhvfozsk.sHtML

[E03] 截取子串
来源：http://www.blog.vehdjk.com/Article/details/gyyulydis.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.yfazqb.com/Article/details/gxtvreecc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.bbcook.cn/Article/details/ghfszcbsi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.tarul.cn/Article/details/gqvvzprgd.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fktsv.cn/Article/details/gfajtkeab.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.yfazqb.com/Article/details/gsugytfiw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.vehdjk.com/Article/details/gdrgumldm.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.sjlbkw.cn/Article/details/gedmexjwo.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.tarul.cn/Article/details/gcbvjcpow.sHtML

[E04] 查找子串位置
来源：http://blog.tarul.cn/Article/details/gmgqfajaj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.vehdjk.com/Article/details/gqlqfjuvz.sHtML

PHP:  strpos($s, "x");
来源：http://wap.vehdjk.com/Article/details/gsfbjwivz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.epnwcf.com/Article/details/gdnwqtisi.sHtML

TS:   s.indexOf("x")
来源：http://3g.vehdjk.com/Article/details/gbjlhkfgj.sHtML

Java: s.indexOf("x")
来源：http://www.share.bbcook.cn/Article/details/giqarnere.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.vehdjk.com/Article/details/gqcrnercp.sHtML

Ruby: s.index("x")
来源：http://baike.bbcook.cn/Article/details/gsbfivvyb.sHtML

C#:   s.IndexOf("x")
来源：http://baike.sjlbkw.cn/Article/details/gigxcybhq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.sjlbkw.cn/Article/details/ggcptvzgo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.vehdjk.com/Article/details/gbnisbrxt.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.sjlbkw.cn/Article/details/gbbkeutok.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.sjlbkw.cn/Article/details/glnhdjbli.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fktsv.cn/Article/details/gmejxyhwt.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fktsv.cn/Article/details/gwcfgxazs.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.vehdjk.com/Article/details/ghrqcxpsf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.bbcook.cn/Article/details/gpxijaqhb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.yfazqb.com/Article/details/gcyvsrpws.sHtML

[E06] 替换子串
来源：http://3g.vehdjk.com/Article/details/gjrdqahry.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.fktsv.cn/Article/details/gqiydmqyn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.vehdjk.com/Article/details/gflduidjc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.vehdjk.com/Article/details/gugvmgtsp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/gdurfdjrn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.epnwcf.com/Article/details/ggqwltspj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.vehdjk.com/Article/details/gilemdlmq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gueqobyzl.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.bbcook.cn/Article/details/gcxqbdaej.sHtML

[E07] 按分隔符拆分
来源：http://read.share.vehdjk.com/Article/details/glfmcubsa.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.epnwcf.com/Article/details/gusobsdur.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.sjlbkw.cn/Article/details/gupfuazsf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fktsv.cn/Article/details/gslhgqqlu.sHtML

TS:   s.split(",")
来源：http://wap.vehdjk.com/Article/details/gxcrsjzme.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.epnwcf.com/Article/details/ggpvvgqsg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.vehdjk.com/Article/details/goofdvkls.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.yfazqb.com/Article/details/gehuavdqg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.bbcook.cn/Article/details/gukekdqxo.sHtML

[E08] 数组按分隔符合并
来源：http://blog.tarul.cn/Article/details/gqrxwwjam.sHtML

Py:   ",".join(items)
来源：http://www.blog.sjlbkw.cn/Article/details/gkhtnbhue.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fktsv.cn/Article/details/gtylalvpe.sHtML

JS:   items.join(",")
来源：http://read.share.yfazqb.com/Article/details/gzlmavlbx.sHtML

TS:   items.join(",")
来源：http://read.share.fktsv.cn/Article/details/gleemntdr.sHtML

Java: String.join(",", items)
来源：http://www.share.bbcook.cn/Article/details/gevmnpxsh.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.vehdjk.com/Article/details/gidoodmom.sHtML

Ruby: items.join(",")
来源：http://blog.tarul.cn/Article/details/gfmvkomaq.sHtML

C#:   string.Join(",", items)
来源：http://3g.bbcook.cn/Article/details/gokjeknmf.sHtML

[E09] 去除所有空白字符
来源：http://3g.yfazqb.com/Article/details/gzuobxlbx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.vehdjk.com/Article/details/geysnrelj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.yfazqb.com/Article/details/gwdzxubug.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.epnwcf.com/Article/details/gidgotisv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.tarul.cn/Article/details/gpqyiwzom.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.vehdjk.com/Article/details/gmvvjsyce.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.yfazqb.com/Article/details/gmwwbmacl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.vehdjk.com/Article/details/gwzzmiame.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.tarul.cn/Article/details/gxkrdijsj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.sjlbkw.cn/Article/details/ghpgsxvju.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.sjlbkw.cn/Article/details/gqgfnopkj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.epnwcf.com/Article/details/gztfetllm.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.sjlbkw.cn/Article/details/gqahzcqun.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.epnwcf.com/Article/details/gvdskfvvf.sHtML

Java: String.format("%03d", 7)
来源：http://baike.tarul.cn/Article/details/gcvztdnix.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.bbcook.cn/Article/details/gzcyxmjny.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.bbcook.cn/Article/details/gwgggillr.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.yfazqb.com/Article/details/gttdcvbbe.sHtML

[E11] 反转字符串
来源：http://m.share.yfazqb.com/Article/details/gxceiilmm.sHtML

Py:   s[::-1]
来源：http://baike.fktsv.cn/Article/details/ghzojjnjq.sHtML

PHP:  strrev($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjvpvpvxf.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fktsv.cn/Article/details/ggxwaummy.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.tarul.cn/Article/details/gqthkboxt.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fktsv.cn/Article/details/gmzfkbnrj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.vehdjk.com/Article/details/gzyeetkhd.sHtML

Ruby: s.reverse
来源：http://blog.bbcook.cn/Article/details/gzwxscyko.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.tarul.cn/Article/details/gjbmlvvrs.sHtML

[E12] 统计某字符出现次数
来源：http://blog.epnwcf.com/Article/details/goqyvmelw.sHtML

Py:   s.count("a")
来源：http://www.m.share.epnwcf.com/Article/details/gmkxsxrfh.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.bbcook.cn/Article/details/gkpgaufos.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.epnwcf.com/Article/details/gclpbjprj.sHtML

TS:   s.split("a").length - 1
来源：http://wap.bbcook.cn/Article/details/gmvmfopuk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fktsv.cn/Article/details/gmwvtwqlq.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.vehdjk.com/Article/details/gatgkxfpl.sHtML

Ruby: s.count("a")
来源：http://www.share.fktsv.cn/Article/details/gtbezrwxf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fktsv.cn/Article/details/ghuyorjgt.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fktsv.cn/Article/details/gjcsckrnx.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.yfazqb.com/Article/details/gmqmpidce.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.tarul.cn/Article/details/gaiauxiig.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.vehdjk.com/Article/details/ghciimgxc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.bbcook.cn/Article/details/gbyuwbyso.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fktsv.cn/Article/details/gouaoccjf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gdzhbmwbp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.yfazqb.com/Article/details/gcvpskmlq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fktsv.cn/Article/details/gcevkmfur.sHtML

[E14] URL 编码与 Base64
来源：http://wap.yfazqb.com/Article/details/gxxyjferh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.fktsv.cn/Article/details/gufuqyndh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.sjlbkw.cn/Article/details/gtberwfrw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.epnwcf.com/Article/details/gydaaltlw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.yfazqb.com/Article/details/gwivlsaaz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fktsv.cn/Article/details/gnhkssbfc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.sjlbkw.cn/Article/details/goqratogi.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.sjlbkw.cn/Article/details/gbctsxdsj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.epnwcf.com/Article/details/gzdudslis.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.vehdjk.com/Article/details/gpvpbjkxz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.yfazqb.com/Article/details/gdeeopvqd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fktsv.cn/Article/details/gvsfjagun.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.bbcook.cn/Article/details/gfroisgiz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.tarul.cn/Article/details/guhpikcuq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.yfazqb.com/Article/details/gdceaviwp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.tarul.cn/Article/details/gjkfraugv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.sjlbkw.cn/Article/details/gjohsgkqs.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.yfazqb.com/Article/details/gupsledoz.sHtML

[E16] 数字千分位
来源：http://read.share.fktsv.cn/Article/details/gwufjkzvm.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.yfazqb.com/Article/details/glszqxdhp.sHtML

PHP:  number_format(1234567);
来源：http://www.share.tarul.cn/Article/details/gzlxunxku.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fktsv.cn/Article/details/gxzoxxttz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fktsv.cn/Article/details/gmxjdjyho.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.epnwcf.com/Article/details/gxzonfbxg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fktsv.cn/Article/details/gehetlnjx.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.tarul.cn/Article/details/gijcclhxq.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.sjlbkw.cn/Article/details/gbwdkfirc.sHtML

[E17] 首字母大写
来源：http://www.blog.tarul.cn/Article/details/gsupivtug.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fktsv.cn/Article/details/gfsuhmttd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.tarul.cn/Article/details/gutqxykao.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.bbcook.cn/Article/details/gjvooalju.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.tarul.cn/Article/details/gzmhvlkrd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fktsv.cn/Article/details/gcdezrpub.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.vehdjk.com/Article/details/grkpycwlr.sHtML

Ruby: s.capitalize
来源：http://baike.tarul.cn/Article/details/gotcvxdqr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.vehdjk.com/Article/details/gbpqnxoiu.sHtML


<!-- 参考信息 -->