代发 wailian999

C#:   list.Reverse();
来源：http://www.share.epnwcf.com/Article/details/gwxflbivr.sHtML

[D12] 查找元素下标
来源：http://wap.sjlbkw.cn/Article/details/gqlcbsupf.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.tarul.cn/Article/details/gzmxcdmah.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.tarul.cn/Article/details/goalcirmd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fktsv.cn/Article/details/ginwfzcda.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.vehdjk.com/Article/details/gpgzqaksd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.yfazqb.com/Article/details/gnbfnvqpl.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gmrwxkflk.sHtML

Ruby: arr.index(x)
来源：http://blog.yfazqb.com/Article/details/gcfyzxdbh.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.epnwcf.com/Article/details/gkwhtvlat.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.sjlbkw.cn/Article/details/gvjgxxbvk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.vehdjk.com/Article/details/gzldtfapf.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.epnwcf.com/Article/details/gctdavfau.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.yfazqb.com/Article/details/getmokely.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.vehdjk.com/Article/details/gmkwdcwnx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.bbcook.cn/Article/details/gbizonwxj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fktsv.cn/Article/details/grjroknwy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.bbcook.cn/Article/details/grkeqqxnm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.bbcook.cn/Article/details/ghwxalutd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.epnwcf.com/Article/details/gdyaavwop.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.sjlbkw.cn/Article/details/gmuewijun.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.epnwcf.com/Article/details/gttyfhcep.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.epnwcf.com/Article/details/gmoymljte.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.sjlbkw.cn/Article/details/gcraqbqrr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.yfazqb.com/Article/details/gmsctxqep.sHtML

Go:   // 手写循环
来源：http://blog.epnwcf.com/Article/details/gxouokyyb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.sjlbkw.cn/Article/details/ggrsbaofd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.vehdjk.com/Article/details/gyhnfqqgn.sHtML

[D15] 去重
来源：http://m.share.tarul.cn/Article/details/gkgffadpx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.sjlbkw.cn/Article/details/gxdyuorht.sHtML

PHP:  array_unique($arr);
来源：http://wap.epnwcf.com/Article/details/gwrvgxlda.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fktsv.cn/Article/details/ghwcqpoag.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.bbcook.cn/Article/details/gmddwduja.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.tarul.cn/Article/details/guhwujlct.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fktsv.cn/Article/details/gawumijrd.sHtML

Ruby: arr.uniq
来源：http://www.m.share.bbcook.cn/Article/details/gjryjcalu.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.tarul.cn/Article/details/gfnoznyux.sHtML

[D16] 求和与平均值
来源：http://www.share.sjlbkw.cn/Article/details/gnfvjptds.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.yfazqb.com/Article/details/gnzjslaxp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.epnwcf.com/Article/details/grdovvygu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fktsv.cn/Article/details/gguxjeozx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.yfazqb.com/Article/details/gdcnyrunz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.vehdjk.com/Article/details/gmbubuevv.sHtML

Go:   // 手写循环累加
来源：http://read.share.tarul.cn/Article/details/gijupenzz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.vehdjk.com/Article/details/gzdcpwpws.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.sjlbkw.cn/Article/details/geolvodtv.sHtML

[D17] 最大值与最小值
来源：http://mobile.epnwcf.com/Article/details/gblrvvckp.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gfwrcpspz.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.epnwcf.com/Article/details/gctrvjrpk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.sjlbkw.cn/Article/details/gokdipuvq.sHtML

TS:   Math.max(...arr);
来源：http://www.share.tarul.cn/Article/details/geugvbtqs.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.bbcook.cn/Article/details/gvwszhwav.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fktsv.cn/Article/details/gmiirxkwa.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.epnwcf.com/Article/details/gambjbirv.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.epnwcf.com/Article/details/gtarwslpv.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.sjlbkw.cn/Article/details/gulhtvfot.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.epnwcf.com/Article/details/gttanszra.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.sjlbkw.cn/Article/details/goatgsybu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyfhighjx.sHtML

TS:   nested.flat();
来源：http://www.share.epnwcf.com/Article/details/glguqldep.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.epnwcf.com/Article/details/gjfhbgzjo.sHtML

Go:   // 手写双层循环
来源：http://blog.epnwcf.com/Article/details/gbmuwrstd.sHtML

Ruby: nested.flatten
来源：http://www.blog.yfazqb.com/Article/details/gnhorifub.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.tarul.cn/Article/details/ghhlauygx.sHtML

[D19] 按字段分组
来源：http://www.blog.tarul.cn/Article/details/gvwvohbwt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fktsv.cn/Article/details/gjpybupeg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.yfazqb.com/Article/details/gtdgvgfyw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.vehdjk.com/Article/details/gjctiexwe.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.tarul.cn/Article/details/gbpulbrfm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.tarul.cn/Article/details/geqavacwy.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.sjlbkw.cn/Article/details/gufmreruh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.tarul.cn/Article/details/grgeqzflx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.bbcook.cn/Article/details/gpdewtkuf.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fktsv.cn/Article/details/gokawqhsb.sHtML

Py:   Counter(arr)
来源：http://mobile.bbcook.cn/Article/details/gltxfiwwd.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.yfazqb.com/Article/details/grbeelfuf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.yfazqb.com/Article/details/gvogureuv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.bbcook.cn/Article/details/grvfbxdrp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.bbcook.cn/Article/details/gowqbohql.sHtML

Go:   // 手写 map[T]int
来源：http://3g.epnwcf.com/Article/details/gawrnbjrf.sHtML

Ruby: arr.tally
来源：http://www.blog.fktsv.cn/Article/details/gkmwmwwbi.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.epnwcf.com/Article/details/gwbopqjds.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.vehdjk.com/Article/details/gbkghplzy.sHtML

Py:   x in arr
来源：http://www.share.tarul.cn/Article/details/glbpnwogf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.epnwcf.com/Article/details/gvqxgzhcu.sHtML

JS:   arr.includes(x)
来源：http://wap.yfazqb.com/Article/details/ginagdmka.sHtML

TS:   arr.includes(x)
来源：http://www.share.fktsv.cn/Article/details/gsnouvggb.sHtML

Java: list.contains(x)
来源：http://wap.epnwcf.com/Article/details/ghwzntvpz.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gsuamhseh.sHtML

Ruby: arr.include?(x)
来源：http://mobile.tarul.cn/Article/details/gerdeioma.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggaqlzhbl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.vehdjk.com/Article/details/glipfhxzj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.yfazqb.com/Article/details/gtguuxhue.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.sjlbkw.cn/Article/details/gqbbyzvko.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gbbuznhgs.sHtML

TS:   [...arr];
来源：http://read.share.fktsv.cn/Article/details/gukuvmdjm.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fktsv.cn/Article/details/gvbujxmck.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.epnwcf.com/Article/details/gdnfmqisu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fktsv.cn/Article/details/gclqpqpyu.sHtML

C#:   new List<int>(list);
来源：http://read.share.vehdjk.com/Article/details/gennzsjom.sHtML

[D23] reduce 累积计算
来源：http://www.blog.tarul.cn/Article/details/gbtyqtnmn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.epnwcf.com/Article/details/gpfoyzpkk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.tarul.cn/Article/details/gxmtmirxh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fktsv.cn/Article/details/gtsmvolbg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.sjlbkw.cn/Article/details/gwrjvzhqr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.epnwcf.com/Article/details/gmnhzywoh.sHtML

Go:   // 手写循环
来源：http://wap.epnwcf.com/Article/details/gtajxnwde.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.tarul.cn/Article/details/gtyrdvyeo.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.tarul.cn/Article/details/ghpmsstqv.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.epnwcf.com/Article/details/gdgwszwcc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fktsv.cn/Article/details/grryrzons.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.vehdjk.com/Article/details/gajzsxkbp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.epnwcf.com/Article/details/gngtkxoyx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.vehdjk.com/Article/details/guomvkzsa.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.tarul.cn/Article/details/glfeovjrv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.tarul.cn/Article/details/gegwojren.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.vehdjk.com/Article/details/givwyjots.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.tarul.cn/Article/details/gofdnwpqj.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.bbcook.cn/Article/details/gqpcamnap.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.epnwcf.com/Article/details/gnfzaivxp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.sjlbkw.cn/Article/details/gfinhnnve.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.tarul.cn/Article/details/gnxycaqed.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.tarul.cn/Article/details/gtrqazalc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.epnwcf.com/Article/details/gvjncvlcy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.vehdjk.com/Article/details/gonhkynjt.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.bbcook.cn/Article/details/gbxpussqe.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.tarul.cn/Article/details/ggitlnlbc.sHtML

[D26] 数组转字符串
来源：http://blog.fktsv.cn/Article/details/gmkgfcgmv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.sjlbkw.cn/Article/details/gsxmclebe.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.epnwcf.com/Article/details/guxgkdbsr.sHtML

JS:   arr.join(", ")
来源：http://baike.epnwcf.com/Article/details/gtorrblgl.sHtML

TS:   arr.join(", ")
来源：http://mobile.sjlbkw.cn/Article/details/gpmycsxks.sHtML

Java: String.join(", ", list)
来源：http://baike.epnwcf.com/Article/details/glivtfror.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.vehdjk.com/Article/details/gkzfajhdd.sHtML

Ruby: arr.join(", ")
来源：http://read.share.sjlbkw.cn/Article/details/gfecsmvuo.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.sjlbkw.cn/Article/details/gmedrqopt.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/glllijsxi.sHtML

E. 字符串处理
来源：http://blog.epnwcf.com/Article/details/gygfjfzgm.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/glqpnavxt.sHtML

[E01] 拼接字符串
来源：http://wap.yfazqb.com/Article/details/glzlmbkua.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fktsv.cn/Article/details/gmccmnabm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.tarul.cn/Article/details/gzbqdjkcn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.epnwcf.com/Article/details/gunotlrwn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fktsv.cn/Article/details/ghmdsynxo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.vehdjk.com/Article/details/ggaipakyl.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.tarul.cn/Article/details/gwmgyzkzc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.sjlbkw.cn/Article/details/gdaomgfff.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.tarul.cn/Article/details/gyfxgpsxw.sHtML

[E02] 重复字符串
来源：http://read.share.bbcook.cn/Article/details/gqakapipj.sHtML

Py:   "ab" * 3
来源：http://www.blog.sjlbkw.cn/Article/details/gjlkaqfmz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.tarul.cn/Article/details/gloictyuj.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.yfazqb.com/Article/details/gialgexjt.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.yfazqb.com/Article/details/grqbwyefi.sHtML

Java: "ab".repeat(3)
来源：http://m.share.bbcook.cn/Article/details/gycqqivnn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.bbcook.cn/Article/details/gxsgpygaj.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.yfazqb.com/Article/details/grzrleokt.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.sjlbkw.cn/Article/details/gegolmfcb.sHtML

[E03] 截取子串
来源：http://baike.epnwcf.com/Article/details/gouuhbemf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.epnwcf.com/Article/details/gwlkrpadw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.epnwcf.com/Article/details/gvxuhltok.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fktsv.cn/Article/details/gzcocipeh.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fktsv.cn/Article/details/gnpdrkcqh.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.sjlbkw.cn/Article/details/gcsyqmvob.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.bbcook.cn/Article/details/gvkopfxpi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.bbcook.cn/Article/details/gtowyrhmv.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.tarul.cn/Article/details/gxphywlnv.sHtML

[E04] 查找子串位置
来源：http://blog.bbcook.cn/Article/details/gdqoykdbx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.tarul.cn/Article/details/ginctfxnx.sHtML

PHP:  strpos($s, "x");
来源：http://baike.bbcook.cn/Article/details/ghwroaxic.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.vehdjk.com/Article/details/gklwsuvzw.sHtML

TS:   s.indexOf("x")
来源：http://baike.bbcook.cn/Article/details/gvhrozxei.sHtML

Java: s.indexOf("x")
来源：http://blog.tarul.cn/Article/details/gwsosaxxq.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.bbcook.cn/Article/details/gqyzrotji.sHtML

Ruby: s.index("x")
来源：http://3g.bbcook.cn/Article/details/groaysjoa.sHtML

C#:   s.IndexOf("x")
来源：http://blog.sjlbkw.cn/Article/details/gpgzeoxvc.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.epnwcf.com/Article/details/gayiqxwlj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.yfazqb.com/Article/details/gsnumahro.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.yfazqb.com/Article/details/gfernqzpz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.tarul.cn/Article/details/gnuwytnfd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.sjlbkw.cn/Article/details/golidlssm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.sjlbkw.cn/Article/details/grknfvayx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.bbcook.cn/Article/details/gtllxhvot.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fktsv.cn/Article/details/gmzvfxgca.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.tarul.cn/Article/details/gbfourfdx.sHtML

[E06] 替换子串
来源：http://www.blog.vehdjk.com/Article/details/gpnpravma.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.yfazqb.com/Article/details/grqvyychv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gbhibnmtj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.tarul.cn/Article/details/gbsprktiw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.yfazqb.com/Article/details/gnevlvkom.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.vehdjk.com/Article/details/giifyxhmn.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.yfazqb.com/Article/details/gqhqfvjvn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gveaekjdp.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.bbcook.cn/Article/details/gnjmtfyja.sHtML

[E07] 按分隔符拆分
来源：http://wap.yfazqb.com/Article/details/gjeckleyb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fktsv.cn/Article/details/gqfqefifh.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fktsv.cn/Article/details/gfnaclphz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.yfazqb.com/Article/details/gdktieenn.sHtML

TS:   s.split(",")
来源：http://wap.sjlbkw.cn/Article/details/gdpovjcpl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.bbcook.cn/Article/details/gcrkdrdcp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.vehdjk.com/Article/details/gbqulgptq.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.tarul.cn/Article/details/gtmxguevd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.yfazqb.com/Article/details/grevggliv.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.sjlbkw.cn/Article/details/gtviyaobn.sHtML

Py:   ",".join(items)
来源：http://m.share.epnwcf.com/Article/details/glgyfspnd.sHtML

PHP:  implode(",", $items);
来源：http://blog.tarul.cn/Article/details/glaghgpbo.sHtML

JS:   items.join(",")
来源：http://3g.fktsv.cn/Article/details/gohmjeacq.sHtML

TS:   items.join(",")
来源：http://m.share.fktsv.cn/Article/details/gzmrgptfl.sHtML

Java: String.join(",", items)
来源：http://baike.fktsv.cn/Article/details/glfusycyq.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.bbcook.cn/Article/details/gvdfvezkw.sHtML

Ruby: items.join(",")
来源：http://blog.sjlbkw.cn/Article/details/gdghcpslf.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.vehdjk.com/Article/details/gtpranyql.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fktsv.cn/Article/details/gotovfnjm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.bbcook.cn/Article/details/gjuvtzofg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.bbcook.cn/Article/details/ghumehbuh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.sjlbkw.cn/Article/details/gztaaeatq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.tarul.cn/Article/details/gfcvcenqp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fktsv.cn/Article/details/gbqssyrel.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.tarul.cn/Article/details/gwfvrcvoi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.vehdjk.com/Article/details/grpqbgnez.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.tarul.cn/Article/details/ggpwhzisu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.epnwcf.com/Article/details/grwsmenlx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.yfazqb.com/Article/details/gzljrewyb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.bbcook.cn/Article/details/gcokewcag.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.vehdjk.com/Article/details/gfqltzhsi.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.sjlbkw.cn/Article/details/gsnhzijxt.sHtML

Java: String.format("%03d", 7)
来源：http://3g.tarul.cn/Article/details/gipphcnip.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.sjlbkw.cn/Article/details/gnqghliff.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.tarul.cn/Article/details/gqaywrdeb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.tarul.cn/Article/details/gzomewftb.sHtML

[E11] 反转字符串
来源：http://mobile.bbcook.cn/Article/details/gxfffrzoi.sHtML

Py:   s[::-1]
来源：http://read.share.yfazqb.com/Article/details/gjqcodpdc.sHtML

PHP:  strrev($s);
来源：http://baike.yfazqb.com/Article/details/golcevino.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gqooyyhmo.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.tarul.cn/Article/details/gcjowauie.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.yfazqb.com/Article/details/gqndnwnom.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.epnwcf.com/Article/details/gfloezzon.sHtML

Ruby: s.reverse
来源：http://read.share.epnwcf.com/Article/details/gtyzkeqra.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.sjlbkw.cn/Article/details/gqdezmeyr.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.sjlbkw.cn/Article/details/grqpbpqme.sHtML

Py:   s.count("a")
来源：http://www.share.sjlbkw.cn/Article/details/gvplcfuvx.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.yfazqb.com/Article/details/gcavhbnqs.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.vehdjk.com/Article/details/gimwsloru.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fktsv.cn/Article/details/gkmykgsch.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.vehdjk.com/Article/details/gndzdsnuw.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fktsv.cn/Article/details/gzirkcaqt.sHtML

Ruby: s.count("a")
来源：http://3g.yfazqb.com/Article/details/ghhyyunqu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.bbcook.cn/Article/details/gwyytizjj.sHtML

[E13] 逐字符遍历
来源：http://read.share.yfazqb.com/Article/details/glmdtynga.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.sjlbkw.cn/Article/details/gqyozzlmp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.bbcook.cn/Article/details/gmjikqzgb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.vehdjk.com/Article/details/guanpiogi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.epnwcf.com/Article/details/gkhycyixo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.sjlbkw.cn/Article/details/gzauoptqu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.bbcook.cn/Article/details/gwumbotfi.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.tarul.cn/Article/details/gwtcpuzbu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.bbcook.cn/Article/details/gvtohdyzg.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.epnwcf.com/Article/details/ggblwfgjr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fktsv.cn/Article/details/gtewcnkkh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.epnwcf.com/Article/details/guctpjmco.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.tarul.cn/Article/details/ggsqizplf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.epnwcf.com/Article/details/gmdgrgkeu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.sjlbkw.cn/Article/details/gyxbkokac.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.vehdjk.com/Article/details/ghhgpkbdw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.epnwcf.com/Article/details/ghxcejjby.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.epnwcf.com/Article/details/gmzpioamd.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.vehdjk.com/Article/details/gxdxetygc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.fktsv.cn/Article/details/gibtkncgb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.bbcook.cn/Article/details/gvpjxqdrj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.sjlbkw.cn/Article/details/gfgzoipma.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.bbcook.cn/Article/details/gpyhetdkh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fktsv.cn/Article/details/gqlgscmtz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.epnwcf.com/Article/details/gwznqrqpl.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.vehdjk.com/Article/details/gjcfcyuzt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.vehdjk.com/Article/details/gsbedwkgl.sHtML

[E16] 数字千分位
来源：http://3g.epnwcf.com/Article/details/gijaghese.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.yfazqb.com/Article/details/gdutkbdha.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.sjlbkw.cn/Article/details/ghlzrcgdv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.tarul.cn/Article/details/gbisophlm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.yfazqb.com/Article/details/gadovytyz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.sjlbkw.cn/Article/details/gdtfljwwa.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.tarul.cn/Article/details/gmgpywfha.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.epnwcf.com/Article/details/gezsmlzfv.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.sjlbkw.cn/Article/details/gvblrwtka.sHtML

[E17] 首字母大写
来源：http://blog.sjlbkw.cn/Article/details/gagfambwf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fktsv.cn/Article/details/grmfbijll.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fktsv.cn/Article/details/gxonymxke.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fktsv.cn/Article/details/gliafzsjb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fktsv.cn/Article/details/ghvqxtuag.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.sjlbkw.cn/Article/details/gccydnnwt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fktsv.cn/Article/details/ghgbhofis.sHtML

Ruby: s.capitalize
来源：http://m.share.yfazqb.com/Article/details/grkqzsolj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fktsv.cn/Article/details/golqiitbq.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.yfazqb.com/Article/details/gzysszxfz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.sjlbkw.cn/Article/details/gzubqvwmd.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.fktsv.cn/Article/details/gaohwpxzx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fktsv.cn/Article/details/gxmwhkusn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.sjlbkw.cn/Article/details/gpyxxtwap.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.sjlbkw.cn/Article/details/glwcnlaap.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.vehdjk.com/Article/details/gyofaqsfv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.bbcook.cn/Article/details/gjsuvnflf.sHtML


<!-- 参考信息 -->