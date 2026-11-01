代发 wailian999

TS:   [...arr].reverse();
来源：http://mobile.fktsv.cn/Article/details/gbpkpfajf.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.yfazqb.com/Article/details/gjfwmttmx.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.yfazqb.com/Article/details/gnphtkvvk.sHtML

Ruby: arr.reverse
来源：http://baike.vehdjk.com/Article/details/gbeoroxeu.sHtML

C#:   list.Reverse();
来源：http://blog.sjlbkw.cn/Article/details/gxkkmqbss.sHtML

[D12] 查找元素下标
来源：http://read.share.vehdjk.com/Article/details/gfaauzril.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.bbcook.cn/Article/details/glaogjqes.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.vehdjk.com/Article/details/gjzitzuhj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.bbcook.cn/Article/details/gzmnbgncp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.tarul.cn/Article/details/gkbyrhrhn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.sjlbkw.cn/Article/details/giiouszvo.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.bbcook.cn/Article/details/gyqeqiscf.sHtML

Ruby: arr.index(x)
来源：http://baike.vehdjk.com/Article/details/grijmubel.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.bbcook.cn/Article/details/gxlyampxc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.bbcook.cn/Article/details/gyfvdnqrz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.epnwcf.com/Article/details/guumxpjrp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.tarul.cn/Article/details/gybyektxc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.tarul.cn/Article/details/gldzygajj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.vehdjk.com/Article/details/gpouailuw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.epnwcf.com/Article/details/gcsaqfoch.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.vehdjk.com/Article/details/grjfverqw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.bbcook.cn/Article/details/gskbynzjn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.tarul.cn/Article/details/gglvnootd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fktsv.cn/Article/details/gvjhkchfv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.sjlbkw.cn/Article/details/gnslxydhs.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.epnwcf.com/Article/details/grthchnio.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.vehdjk.com/Article/details/gmihpcmis.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.sjlbkw.cn/Article/details/gobhxwmxm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.sjlbkw.cn/Article/details/gjcwwrsqn.sHtML

Go:   // 手写循环
来源：http://baike.fktsv.cn/Article/details/gbaadiqsu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/gpwsjymzi.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.epnwcf.com/Article/details/gwrdhqpjr.sHtML

[D15] 去重
来源：http://baike.epnwcf.com/Article/details/gmhyotloz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.sjlbkw.cn/Article/details/goatqjdct.sHtML

PHP:  array_unique($arr);
来源：http://mobile.epnwcf.com/Article/details/gkbytnvfr.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.vehdjk.com/Article/details/grofhrkar.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fktsv.cn/Article/details/ghojfogmx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.tarul.cn/Article/details/gcofqwlsz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.vehdjk.com/Article/details/gbtomvulc.sHtML

Ruby: arr.uniq
来源：http://www.blog.epnwcf.com/Article/details/goaxuvhap.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.bbcook.cn/Article/details/gmvbjduvo.sHtML

[D16] 求和与平均值
来源：http://www.blog.vehdjk.com/Article/details/gxdlpapjt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fktsv.cn/Article/details/gzzejcama.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.sjlbkw.cn/Article/details/gpwdidczh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.tarul.cn/Article/details/gizvhewvm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.vehdjk.com/Article/details/gxrqaygbo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.yfazqb.com/Article/details/gtpfebgvm.sHtML

Go:   // 手写循环累加
来源：http://www.blog.epnwcf.com/Article/details/gdemcssqm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.yfazqb.com/Article/details/gidtzbwbi.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.yfazqb.com/Article/details/gmtzortur.sHtML

[D17] 最大值与最小值
来源：http://blog.epnwcf.com/Article/details/gzedcwxlu.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.vehdjk.com/Article/details/gkwwnmwoy.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fktsv.cn/Article/details/govyvmdds.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.yfazqb.com/Article/details/gllktaswe.sHtML

TS:   Math.max(...arr);
来源：http://3g.fktsv.cn/Article/details/gxbslkjvg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fktsv.cn/Article/details/gucipgeep.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.epnwcf.com/Article/details/gxqldjnry.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.yfazqb.com/Article/details/gpksttvor.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.vehdjk.com/Article/details/gyvzvflkt.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.yfazqb.com/Article/details/gtwuiadsy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.yfazqb.com/Article/details/gtznanufo.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.tarul.cn/Article/details/gaqxccoit.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.sjlbkw.cn/Article/details/gqvrfcoqn.sHtML

TS:   nested.flat();
来源：http://www.blog.bbcook.cn/Article/details/gmdlabqia.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.yfazqb.com/Article/details/girsfwzck.sHtML

Go:   // 手写双层循环
来源：http://mobile.yfazqb.com/Article/details/gmnyhijwr.sHtML

Ruby: nested.flatten
来源：http://blog.sjlbkw.cn/Article/details/gnkosyufr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fktsv.cn/Article/details/gwdsrwxza.sHtML

[D19] 按字段分组
来源：http://www.blog.vehdjk.com/Article/details/gqpgeqdfp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.epnwcf.com/Article/details/guheuqttn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.epnwcf.com/Article/details/guibaawtt.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.sjlbkw.cn/Article/details/gfoeyioia.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.vehdjk.com/Article/details/gqfsrbgai.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.yfazqb.com/Article/details/ggybpappq.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.bbcook.cn/Article/details/gxmjhtznp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.tarul.cn/Article/details/gxsohfndx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.bbcook.cn/Article/details/grmomzoqt.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.vehdjk.com/Article/details/gtbwrqrre.sHtML

Py:   Counter(arr)
来源：http://3g.vehdjk.com/Article/details/gmbflzvam.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.tarul.cn/Article/details/geyujuffz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.sjlbkw.cn/Article/details/gzrjrbemw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.bbcook.cn/Article/details/gcztfkbcj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fktsv.cn/Article/details/gztahaiwx.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.bbcook.cn/Article/details/gsxuiwmqo.sHtML

Ruby: arr.tally
来源：http://read.share.tarul.cn/Article/details/gsyywbndt.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.sjlbkw.cn/Article/details/gslcdjmyq.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.tarul.cn/Article/details/gbakyrgvj.sHtML

Py:   x in arr
来源：http://www.share.vehdjk.com/Article/details/gibedlbde.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.epnwcf.com/Article/details/guarjawvl.sHtML

JS:   arr.includes(x)
来源：http://mobile.epnwcf.com/Article/details/gjimzmodf.sHtML

TS:   arr.includes(x)
来源：http://wap.yfazqb.com/Article/details/grhubrxbm.sHtML

Java: list.contains(x)
来源：http://www.blog.vehdjk.com/Article/details/gognkwlbq.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.tarul.cn/Article/details/ggsbissux.sHtML

Ruby: arr.include?(x)
来源：http://read.share.epnwcf.com/Article/details/glyjlqqms.sHtML

C#:   list.Contains(x)
来源：http://m.share.yfazqb.com/Article/details/gtjhjhrzq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.sjlbkw.cn/Article/details/gdlurnban.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.tarul.cn/Article/details/gclhnfucm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.vehdjk.com/Article/details/gryzygzaw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fktsv.cn/Article/details/gpyufrghq.sHtML

TS:   [...arr];
来源：http://read.share.sjlbkw.cn/Article/details/gltzyppbv.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.bbcook.cn/Article/details/gldgrxmin.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.bbcook.cn/Article/details/ghroqeugp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.bbcook.cn/Article/details/gmqbblzgu.sHtML

C#:   new List<int>(list);
来源：http://www.share.epnwcf.com/Article/details/gjhplfawn.sHtML

[D23] reduce 累积计算
来源：http://m.share.sjlbkw.cn/Article/details/gjvdckuwg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gvnbkoped.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.tarul.cn/Article/details/gnxbaibas.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.vehdjk.com/Article/details/gybfqvxrq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.bbcook.cn/Article/details/gmkhzzkic.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.tarul.cn/Article/details/gwtztghgj.sHtML

Go:   // 手写循环
来源：http://www.blog.bbcook.cn/Article/details/gqowefbta.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.yfazqb.com/Article/details/gclghvoyf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkbzvtysf.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.yfazqb.com/Article/details/gkjkrdbcd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.vehdjk.com/Article/details/gtqkuluei.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.epnwcf.com/Article/details/gfrvcqkne.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.bbcook.cn/Article/details/gggmjgsvr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fktsv.cn/Article/details/ggrbronlo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fktsv.cn/Article/details/goscmwbbp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.tarul.cn/Article/details/gkxnwqver.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fktsv.cn/Article/details/gsluehnxw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.sjlbkw.cn/Article/details/gpfqbgufy.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.sjlbkw.cn/Article/details/ggexwabgg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.vehdjk.com/Article/details/gkueyfnmn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.tarul.cn/Article/details/genpdekyp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.yfazqb.com/Article/details/gjynhdlfl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.bbcook.cn/Article/details/ggzjvsnun.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.vehdjk.com/Article/details/gjmrhdmmy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.vehdjk.com/Article/details/gmzjwpwee.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gimwbzuod.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.sjlbkw.cn/Article/details/gahandhzb.sHtML

[D26] 数组转字符串
来源：http://3g.tarul.cn/Article/details/ggtcqytjh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fktsv.cn/Article/details/gnvgkeoem.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fktsv.cn/Article/details/gqtuhpkdb.sHtML

JS:   arr.join(", ")
来源：http://mobile.sjlbkw.cn/Article/details/gdzvujlzm.sHtML

TS:   arr.join(", ")
来源：http://blog.bbcook.cn/Article/details/ggitvxznc.sHtML

Java: String.join(", ", list)
来源：http://read.share.fktsv.cn/Article/details/gcznwehvu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fktsv.cn/Article/details/gktkdudnr.sHtML

Ruby: arr.join(", ")
来源：http://3g.tarul.cn/Article/details/gduhufhqk.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.tarul.cn/Article/details/gausyecht.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gasmlemqe.sHtML

E. 字符串处理
来源：http://read.share.epnwcf.com/Article/details/gdkcqssqh.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gvhuldctf.sHtML

[E01] 拼接字符串
来源：http://www.blog.fktsv.cn/Article/details/glsvwmfju.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.tarul.cn/Article/details/gkzqdngod.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.yfazqb.com/Article/details/guhyiuoll.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.epnwcf.com/Article/details/gdylxiiyz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.tarul.cn/Article/details/glzihwmme.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fktsv.cn/Article/details/gcdavlnvv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.bbcook.cn/Article/details/gpcivqgqt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.vehdjk.com/Article/details/gkugdjqgj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.epnwcf.com/Article/details/goyxpimjg.sHtML

[E02] 重复字符串
来源：http://3g.epnwcf.com/Article/details/gkmbrqjhb.sHtML

Py:   "ab" * 3
来源：http://wap.yfazqb.com/Article/details/gmydorseg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.yfazqb.com/Article/details/gnbntmjid.sHtML

JS:   "ab".repeat(3)
来源：http://blog.sjlbkw.cn/Article/details/ghgecmfdr.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.tarul.cn/Article/details/gyxaauhrt.sHtML

Java: "ab".repeat(3)
来源：http://read.share.vehdjk.com/Article/details/gpcxvhjzo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.epnwcf.com/Article/details/girxdpihg.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.yfazqb.com/Article/details/goulkfzoq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fktsv.cn/Article/details/gytayihxq.sHtML

[E03] 截取子串
来源：http://read.share.vehdjk.com/Article/details/gklulpboc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.tarul.cn/Article/details/grkdmougs.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.tarul.cn/Article/details/gsobstagj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.sjlbkw.cn/Article/details/gcaytynqv.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.fktsv.cn/Article/details/gwtnhldyo.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.yfazqb.com/Article/details/gdgkzlgqr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.sjlbkw.cn/Article/details/gnhamgqjj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.bbcook.cn/Article/details/gtkgfypcf.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.bbcook.cn/Article/details/gzzvgyupc.sHtML

[E04] 查找子串位置
来源：http://3g.sjlbkw.cn/Article/details/ggqeoniax.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.epnwcf.com/Article/details/gzlrfnbun.sHtML

PHP:  strpos($s, "x");
来源：http://wap.vehdjk.com/Article/details/gqynuawaj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.bbcook.cn/Article/details/gugldfvoo.sHtML

TS:   s.indexOf("x")
来源：http://read.share.epnwcf.com/Article/details/gbojwsoak.sHtML

Java: s.indexOf("x")
来源：http://www.share.epnwcf.com/Article/details/gmmfoqffp.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.vehdjk.com/Article/details/gsgbsgdzm.sHtML

Ruby: s.index("x")
来源：http://read.share.tarul.cn/Article/details/ghwiszbwz.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.bbcook.cn/Article/details/gdruoahus.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.bbcook.cn/Article/details/gfmrozety.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.yfazqb.com/Article/details/gwlcihnic.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.vehdjk.com/Article/details/gqltncgvf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.epnwcf.com/Article/details/gszuiogtb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.tarul.cn/Article/details/gmpaglrqy.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.bbcook.cn/Article/details/gurjxbnxf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.epnwcf.com/Article/details/gmunuwgvt.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.vehdjk.com/Article/details/gmlksngpa.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.bbcook.cn/Article/details/gxncnqlom.sHtML

[E06] 替换子串
来源：http://mobile.vehdjk.com/Article/details/gxhyshden.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.vehdjk.com/Article/details/gvjrvzapo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fktsv.cn/Article/details/gutdaxwfl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.epnwcf.com/Article/details/gsnkisujr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.tarul.cn/Article/details/gxudqujpm.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gmdrpnznu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fktsv.cn/Article/details/gxnvuqfub.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gsfnqvlzg.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.epnwcf.com/Article/details/gxgqdrihh.sHtML

[E07] 按分隔符拆分
来源：http://baike.sjlbkw.cn/Article/details/gxuamlqoa.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.tarul.cn/Article/details/gieshlumb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.vehdjk.com/Article/details/gntyzklah.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.tarul.cn/Article/details/gtyvlitkm.sHtML

TS:   s.split(",")
来源：http://3g.fktsv.cn/Article/details/gatgzmzib.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.bbcook.cn/Article/details/gfqwdnwqe.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.yfazqb.com/Article/details/gsxsyrnav.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.tarul.cn/Article/details/gvwulalxp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.yfazqb.com/Article/details/gbojexmrp.sHtML

[E08] 数组按分隔符合并
来源：http://blog.epnwcf.com/Article/details/gpvvduzui.sHtML

Py:   ",".join(items)
来源：http://read.share.sjlbkw.cn/Article/details/gzzfystht.sHtML

PHP:  implode(",", $items);
来源：http://3g.sjlbkw.cn/Article/details/grrgitssf.sHtML

JS:   items.join(",")
来源：http://www.blog.tarul.cn/Article/details/gtmayjlqy.sHtML

TS:   items.join(",")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmrnrfokb.sHtML

Java: String.join(",", items)
来源：http://baike.epnwcf.com/Article/details/gncewzkpz.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.epnwcf.com/Article/details/gwjvwqjlh.sHtML

Ruby: items.join(",")
来源：http://www.share.bbcook.cn/Article/details/gnbdecden.sHtML

C#:   string.Join(",", items)
来源：http://3g.vehdjk.com/Article/details/gqkhhktmr.sHtML

[E09] 去除所有空白字符
来源：http://3g.epnwcf.com/Article/details/giicieebi.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.vehdjk.com/Article/details/grolidubo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.epnwcf.com/Article/details/gqyubalwn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.epnwcf.com/Article/details/gesdmqjji.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.tarul.cn/Article/details/gbvhprixr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fktsv.cn/Article/details/gbthkcfde.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.yfazqb.com/Article/details/ggvifoamp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.sjlbkw.cn/Article/details/gtldrlhqw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.epnwcf.com/Article/details/ggdjlxgxp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.yfazqb.com/Article/details/gwgtuwsjm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.tarul.cn/Article/details/gjhzirftk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.sjlbkw.cn/Article/details/gqitxokil.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fktsv.cn/Article/details/gngoztmuu.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.vehdjk.com/Article/details/ghqjnceeh.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjrkqzoya.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.bbcook.cn/Article/details/gcortcxov.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.sjlbkw.cn/Article/details/ghemghbry.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.yfazqb.com/Article/details/gisubrdhe.sHtML

[E11] 反转字符串
来源：http://baike.bbcook.cn/Article/details/gvrxbkwdj.sHtML

Py:   s[::-1]
来源：http://m.share.bbcook.cn/Article/details/gxcmjvvuq.sHtML

PHP:  strrev($s);
来源：http://wap.epnwcf.com/Article/details/gdlndvrqw.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.vehdjk.com/Article/details/gaxgjimyo.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fktsv.cn/Article/details/ghsfiedvp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.yfazqb.com/Article/details/godajxubl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.yfazqb.com/Article/details/gaponjyto.sHtML

Ruby: s.reverse
来源：http://read.share.vehdjk.com/Article/details/gkgihrydd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.tarul.cn/Article/details/gzhyyrbth.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.vehdjk.com/Article/details/gidpymxda.sHtML

Py:   s.count("a")
来源：http://baike.yfazqb.com/Article/details/glibjxwnn.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.bbcook.cn/Article/details/gryavkvvd.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.yfazqb.com/Article/details/gtipxtsqo.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.tarul.cn/Article/details/ghxohuvnw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.epnwcf.com/Article/details/gptybszib.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.epnwcf.com/Article/details/gdpfrxkwr.sHtML

Ruby: s.count("a")
来源：http://www.m.share.yfazqb.com/Article/details/gdxyzlsku.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.bbcook.cn/Article/details/gbtfzakxf.sHtML

[E13] 逐字符遍历
来源：http://m.share.fktsv.cn/Article/details/gjrqqmbro.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fktsv.cn/Article/details/gejrntyfw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.vehdjk.com/Article/details/gjscypnoj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.epnwcf.com/Article/details/gbztjzmdn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fktsv.cn/Article/details/grcoijjoy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.vehdjk.com/Article/details/geqqnlakx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.epnwcf.com/Article/details/glefqqwvu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.bbcook.cn/Article/details/gtrqujvgd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fktsv.cn/Article/details/gyjyppmfi.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.epnwcf.com/Article/details/gvmuxrraq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.epnwcf.com/Article/details/gaajjmqkt.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fktsv.cn/Article/details/gldlokafo.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.sjlbkw.cn/Article/details/gifavabjz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.sjlbkw.cn/Article/details/gyscwaubg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.tarul.cn/Article/details/gmxjigglc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fktsv.cn/Article/details/gzojwgmwy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.bbcook.cn/Article/details/ghkcwxvxz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fktsv.cn/Article/details/gsewvpemm.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fktsv.cn/Article/details/gvzmfmilx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.yfazqb.com/Article/details/gjgazcyxp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.epnwcf.com/Article/details/gfwdxsnpt.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.epnwcf.com/Article/details/gwpxjqqig.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.yfazqb.com/Article/details/guqqmtrlh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.bbcook.cn/Article/details/gfhgmfwmy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.epnwcf.com/Article/details/gtylkucig.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.vehdjk.com/Article/details/gwcmzylty.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.tarul.cn/Article/details/ghpcodqmg.sHtML

[E16] 数字千分位
来源：http://blog.sjlbkw.cn/Article/details/griuvpmwu.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.tarul.cn/Article/details/gwrtardpq.sHtML

PHP:  number_format(1234567);
来源：http://wap.vehdjk.com/Article/details/gmlozauvj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.vehdjk.com/Article/details/gqmzkewmv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.tarul.cn/Article/details/gqjrhvxfb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.sjlbkw.cn/Article/details/grjtimrrm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.bbcook.cn/Article/details/gkvdfnqqo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.tarul.cn/Article/details/gttczqevc.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.tarul.cn/Article/details/gmehxoacv.sHtML

[E17] 首字母大写
来源：http://read.share.bbcook.cn/Article/details/gtymjdbdx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.yfazqb.com/Article/details/gcplffvco.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.yfazqb.com/Article/details/gmwapbemv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.vehdjk.com/Article/details/gaxfktles.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.tarul.cn/Article/details/gjzomjjyg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.tarul.cn/Article/details/govwxptfk.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fktsv.cn/Article/details/gwtayesrv.sHtML

Ruby: s.capitalize
来源：http://www.share.bbcook.cn/Article/details/gpbxhpwmj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.epnwcf.com/Article/details/gunhvkcfd.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.tarul.cn/Article/details/gdfcksvoi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.yfazqb.com/Article/details/gohloczii.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.yfazqb.com/Article/details/gxayklntn.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.yfazqb.com/Article/details/gnfbkudcl.sHtML


<!-- 参考信息 -->