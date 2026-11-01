代发 wailian999

PHP:  sort($arr);
来源：http://mobile.fktsv.cn/Article/details/gaehhkymn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.vehdjk.com/Article/details/gtvyhtprp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.epnwcf.com/Article/details/gaoygwfow.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.yfazqb.com/Article/details/giadfccwa.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.yfazqb.com/Article/details/gfjnecbxc.sHtML

Ruby: arr.sort
来源：http://blog.epnwcf.com/Article/details/gzaoljbhw.sHtML

C#:   list.Sort();
来源：http://mobile.sjlbkw.cn/Article/details/gnwzfbxcr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.yfazqb.com/Article/details/gyshwzrux.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.vehdjk.com/Article/details/gkhvgvkqr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.epnwcf.com/Article/details/gzepgpiny.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.tarul.cn/Article/details/gsjeusoqc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.yfazqb.com/Article/details/gwxalloke.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.yfazqb.com/Article/details/gstqfekvb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.vehdjk.com/Article/details/gxoyttvku.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.bbcook.cn/Article/details/gbdseuxnh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.bbcook.cn/Article/details/gayhghgoq.sHtML

[D11] 反转数组
来源：http://m.share.epnwcf.com/Article/details/gmnhdxdlx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.sjlbkw.cn/Article/details/gmqocklbm.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.tarul.cn/Article/details/ggymbyqzn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.epnwcf.com/Article/details/gqdqdvsoy.sHtML

TS:   [...arr].reverse();
来源：http://read.share.yfazqb.com/Article/details/gkaacchyx.sHtML

Java: Collections.reverse(list);
来源：http://3g.fktsv.cn/Article/details/gfwjupcqx.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.bbcook.cn/Article/details/gowlubqid.sHtML

Ruby: arr.reverse
来源：http://www.blog.tarul.cn/Article/details/gxgphoaez.sHtML

C#:   list.Reverse();
来源：http://m.share.bbcook.cn/Article/details/gtgyejjmw.sHtML

[D12] 查找元素下标
来源：http://mobile.yfazqb.com/Article/details/gpxkzfoaw.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.tarul.cn/Article/details/glidktcxu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fktsv.cn/Article/details/gshxfydll.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.yfazqb.com/Article/details/gqldqtved.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fktsv.cn/Article/details/gszlihwrs.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.epnwcf.com/Article/details/gejtmbons.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gegndjido.sHtML

Ruby: arr.index(x)
来源：http://mobile.tarul.cn/Article/details/gtpzoupgo.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.yfazqb.com/Article/details/giuiapcnv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.sjlbkw.cn/Article/details/ghpfblrbe.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.epnwcf.com/Article/details/gkkszwfpp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.vehdjk.com/Article/details/gmzipeusv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.epnwcf.com/Article/details/gznkfommk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fktsv.cn/Article/details/gyuruxbau.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fktsv.cn/Article/details/gebnktnfz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.vehdjk.com/Article/details/gyjeuphua.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.bbcook.cn/Article/details/gowgkinyr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.bbcook.cn/Article/details/grrczqqnf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fktsv.cn/Article/details/gscptpsyj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.tarul.cn/Article/details/gycxkbreh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.yfazqb.com/Article/details/gqjxnmhrp.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fktsv.cn/Article/details/gokdmasnr.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.vehdjk.com/Article/details/gdbyduwxn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.vehdjk.com/Article/details/gbpanlqfj.sHtML

Go:   // 手写循环
来源：http://wap.bbcook.cn/Article/details/gizyprzhl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.sjlbkw.cn/Article/details/grulqavqf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fktsv.cn/Article/details/gthfijeqk.sHtML

[D15] 去重
来源：http://3g.fktsv.cn/Article/details/gsjiezarj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fktsv.cn/Article/details/gmccuknfj.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fktsv.cn/Article/details/gfdcewgbt.sHtML

JS:   [...new Set(arr)]
来源：http://wap.yfazqb.com/Article/details/gvwxjsmcm.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.tarul.cn/Article/details/gxcgilrom.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.sjlbkw.cn/Article/details/gndoeihba.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.epnwcf.com/Article/details/ggdveebeq.sHtML

Ruby: arr.uniq
来源：http://wap.yfazqb.com/Article/details/gmswwdupj.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.bbcook.cn/Article/details/gpmmobtfy.sHtML

[D16] 求和与平均值
来源：http://www.m.share.sjlbkw.cn/Article/details/gfukhrjyk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.bbcook.cn/Article/details/gawekxcvz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.bbcook.cn/Article/details/gqbqutzej.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fktsv.cn/Article/details/gpuimpqfd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.tarul.cn/Article/details/gylwkcegn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.epnwcf.com/Article/details/gvmyamexr.sHtML

Go:   // 手写循环累加
来源：http://www.share.epnwcf.com/Article/details/gwnshzzrf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.sjlbkw.cn/Article/details/guafqqfhh.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.epnwcf.com/Article/details/grevfucgy.sHtML

[D17] 最大值与最小值
来源：http://www.blog.epnwcf.com/Article/details/gcespxobl.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.yfazqb.com/Article/details/gepjrqugd.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.yfazqb.com/Article/details/gzzfkzjfg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.bbcook.cn/Article/details/getorxgeg.sHtML

TS:   Math.max(...arr);
来源：http://blog.yfazqb.com/Article/details/gnzejdqxc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fktsv.cn/Article/details/gptooktdy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.tarul.cn/Article/details/gtgwdfllk.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.vehdjk.com/Article/details/gqcdihpvq.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.yfazqb.com/Article/details/golpepcpt.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.bbcook.cn/Article/details/gheefjlrz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.vehdjk.com/Article/details/gepujgcmp.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.yfazqb.com/Article/details/gejxixewn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.tarul.cn/Article/details/gqcdgwekw.sHtML

TS:   nested.flat();
来源：http://www.blog.fktsv.cn/Article/details/ghiwsjfjp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fktsv.cn/Article/details/ghefusrpf.sHtML

Go:   // 手写双层循环
来源：http://read.share.bbcook.cn/Article/details/gesnokcnt.sHtML

Ruby: nested.flatten
来源：http://www.m.share.yfazqb.com/Article/details/ggpqeypic.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.epnwcf.com/Article/details/gmuolplfg.sHtML

[D19] 按字段分组
来源：http://www.share.vehdjk.com/Article/details/gtemwlqtl.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fktsv.cn/Article/details/gzbythzld.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fktsv.cn/Article/details/gzupuzqvi.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.tarul.cn/Article/details/gfviawicy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fktsv.cn/Article/details/gqvqjthxs.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.bbcook.cn/Article/details/gdcbyrcie.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.epnwcf.com/Article/details/gmbtlprko.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.sjlbkw.cn/Article/details/gciipfhtt.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.yfazqb.com/Article/details/gflrtdxaw.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.bbcook.cn/Article/details/gqfmflogu.sHtML

Py:   Counter(arr)
来源：http://m.share.vehdjk.com/Article/details/gantmgtnp.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fktsv.cn/Article/details/gszoatyel.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.sjlbkw.cn/Article/details/gtlchhxlh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.vehdjk.com/Article/details/garkboxzk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.epnwcf.com/Article/details/gtaexbrfn.sHtML

Go:   // 手写 map[T]int
来源：http://wap.yfazqb.com/Article/details/gzgnckloa.sHtML

Ruby: arr.tally
来源：http://mobile.bbcook.cn/Article/details/gfnatokto.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.vehdjk.com/Article/details/guqjkxovx.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.epnwcf.com/Article/details/gajsshdvf.sHtML

Py:   x in arr
来源：http://baike.fktsv.cn/Article/details/gnwnwovss.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fktsv.cn/Article/details/gnqxzhmit.sHtML

JS:   arr.includes(x)
来源：http://www.share.sjlbkw.cn/Article/details/gqykmapbu.sHtML

TS:   arr.includes(x)
来源：http://m.share.tarul.cn/Article/details/gegjdekdc.sHtML

Java: list.contains(x)
来源：http://3g.vehdjk.com/Article/details/gypgzorpx.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gktiaoiwa.sHtML

Ruby: arr.include?(x)
来源：http://wap.sjlbkw.cn/Article/details/gealizkoi.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnambwsqk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.epnwcf.com/Article/details/gpbhsjxdf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.epnwcf.com/Article/details/gvgddcicr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.bbcook.cn/Article/details/gmzrknmct.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.epnwcf.com/Article/details/gsjpabhct.sHtML

TS:   [...arr];
来源：http://blog.fktsv.cn/Article/details/gabzobhmo.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.yfazqb.com/Article/details/ghofexfas.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.epnwcf.com/Article/details/gwrgqkfzt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.vehdjk.com/Article/details/geftnvgpc.sHtML

C#:   new List<int>(list);
来源：http://m.share.tarul.cn/Article/details/gfapvfrrn.sHtML

[D23] reduce 累积计算
来源：http://3g.vehdjk.com/Article/details/gslevosjl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.bbcook.cn/Article/details/gwdqytbrw.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.sjlbkw.cn/Article/details/gkxmurxrm.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gnnvxxieh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.yfazqb.com/Article/details/gopixhqlu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.tarul.cn/Article/details/gcdfrncpd.sHtML

Go:   // 手写循环
来源：http://3g.vehdjk.com/Article/details/gcdkykivr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.yfazqb.com/Article/details/gbawartcn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.vehdjk.com/Article/details/gnpsocfqb.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.bbcook.cn/Article/details/gbopbbhtx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.epnwcf.com/Article/details/ghodmpidn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.epnwcf.com/Article/details/gymvwpzjh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.sjlbkw.cn/Article/details/giqediwhh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.vehdjk.com/Article/details/givtjnnmo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fktsv.cn/Article/details/gponkklln.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.tarul.cn/Article/details/grybamiym.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fktsv.cn/Article/details/gerghfqzx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.sjlbkw.cn/Article/details/gglbjwurn.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.tarul.cn/Article/details/gijhjrjfe.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fktsv.cn/Article/details/gpscnhbwa.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.tarul.cn/Article/details/gygqpjocz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.epnwcf.com/Article/details/ggwimunvw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.epnwcf.com/Article/details/ggdjcegyi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.yfazqb.com/Article/details/ghvmuaxdg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.bbcook.cn/Article/details/gqsrntqdb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.epnwcf.com/Article/details/gxhhbusgb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.vehdjk.com/Article/details/gqznpnyzi.sHtML

[D26] 数组转字符串
来源：http://www.share.tarul.cn/Article/details/gkdkvzcsu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fktsv.cn/Article/details/gudmvjgum.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gccxikmkn.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fktsv.cn/Article/details/gwzyckkzz.sHtML

TS:   arr.join(", ")
来源：http://read.share.epnwcf.com/Article/details/gatvnslus.sHtML

Java: String.join(", ", list)
来源：http://m.share.bbcook.cn/Article/details/gywjzcnqo.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.epnwcf.com/Article/details/gggsdrkbb.sHtML

Ruby: arr.join(", ")
来源：http://mobile.tarul.cn/Article/details/gkqkxqzxn.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.tarul.cn/Article/details/gojnvewrl.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/grxejcswk.sHtML

E. 字符串处理
来源：http://blog.sjlbkw.cn/Article/details/glgyuduob.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gvidzcdbu.sHtML

[E01] 拼接字符串
来源：http://blog.sjlbkw.cn/Article/details/gzudzelgf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.bbcook.cn/Article/details/gqajvpeev.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.yfazqb.com/Article/details/geiigwnwi.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.vehdjk.com/Article/details/gptjtxnta.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.epnwcf.com/Article/details/grhvwzrpo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.epnwcf.com/Article/details/gqgbgynoa.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.epnwcf.com/Article/details/geznpytcl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.tarul.cn/Article/details/gkvwhildy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.epnwcf.com/Article/details/gqcrlhfej.sHtML

[E02] 重复字符串
来源：http://mobile.epnwcf.com/Article/details/gffwmbmvn.sHtML

Py:   "ab" * 3
来源：http://wap.yfazqb.com/Article/details/glppqxjlj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.sjlbkw.cn/Article/details/goaewyufe.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.yfazqb.com/Article/details/gtnjkmedv.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.yfazqb.com/Article/details/ggczkjdwf.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.bbcook.cn/Article/details/gnqorzkxa.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.bbcook.cn/Article/details/gvbyrrdkp.sHtML

Ruby: "ab" * 3
来源：http://mobile.sjlbkw.cn/Article/details/grjpnayhz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.epnwcf.com/Article/details/gozhxwfbv.sHtML

[E03] 截取子串
来源：http://www.share.epnwcf.com/Article/details/gumnbtmot.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.vehdjk.com/Article/details/gwnrbvokp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.yfazqb.com/Article/details/ggsxeryet.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.vehdjk.com/Article/details/gzfhjzkeh.sHtML

TS:   s.slice(1, 4)
来源：http://wap.tarul.cn/Article/details/guibynweb.sHtML

Java: s.substring(1, 4)
来源：http://wap.vehdjk.com/Article/details/gkdbehtrx.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.sjlbkw.cn/Article/details/gapnhjbrh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.vehdjk.com/Article/details/ghjtyfgom.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fktsv.cn/Article/details/gaurslkfe.sHtML

[E04] 查找子串位置
来源：http://wap.bbcook.cn/Article/details/gfdprclhi.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.yfazqb.com/Article/details/gsnymdxjs.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.sjlbkw.cn/Article/details/gwfewgwtd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fktsv.cn/Article/details/gozfpewoc.sHtML

TS:   s.indexOf("x")
来源：http://mobile.vehdjk.com/Article/details/gvgzclvrf.sHtML

Java: s.indexOf("x")
来源：http://3g.fktsv.cn/Article/details/gknufaxnv.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.epnwcf.com/Article/details/gzotxvbfc.sHtML

Ruby: s.index("x")
来源：http://m.share.tarul.cn/Article/details/gusxujghq.sHtML

C#:   s.IndexOf("x")
来源：http://blog.sjlbkw.cn/Article/details/giysenxyp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.tarul.cn/Article/details/gmoupkeri.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fktsv.cn/Article/details/gxpidxugm.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.yfazqb.com/Article/details/gekazrdfv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.vehdjk.com/Article/details/geowhixaz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.vehdjk.com/Article/details/gfewmsbis.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.tarul.cn/Article/details/gmcxfjkhk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.yfazqb.com/Article/details/gouuyoezw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.bbcook.cn/Article/details/grtmkhzwq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.bbcook.cn/Article/details/ggxlhvpfp.sHtML

[E06] 替换子串
来源：http://blog.fktsv.cn/Article/details/gzvtgefhj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.bbcook.cn/Article/details/grbontsty.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.bbcook.cn/Article/details/gomlfnurg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.yfazqb.com/Article/details/gvtmwcsea.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.tarul.cn/Article/details/gkpqcqerr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/gomzmrttp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.sjlbkw.cn/Article/details/ggxgvmqgn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gpxhpousj.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gogeqiide.sHtML

[E07] 按分隔符拆分
来源：http://baike.yfazqb.com/Article/details/gtokhbtdl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.sjlbkw.cn/Article/details/gosihvrfk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.sjlbkw.cn/Article/details/gjpwkcraz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fktsv.cn/Article/details/galbhkemk.sHtML

TS:   s.split(",")
来源：http://mobile.fktsv.cn/Article/details/gvaqysirv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.tarul.cn/Article/details/gfqbnfsmd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.yfazqb.com/Article/details/gkchvimki.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.epnwcf.com/Article/details/gtazgyapa.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.bbcook.cn/Article/details/gogmqxxhe.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fktsv.cn/Article/details/gxfzoyxwl.sHtML

Py:   ",".join(items)
来源：http://read.share.sjlbkw.cn/Article/details/gpakflctx.sHtML

PHP:  implode(",", $items);
来源：http://read.share.tarul.cn/Article/details/grdhsluzf.sHtML

JS:   items.join(",")
来源：http://baike.bbcook.cn/Article/details/gelpxicss.sHtML

TS:   items.join(",")
来源：http://www.blog.sjlbkw.cn/Article/details/gcjmxstwa.sHtML

Java: String.join(",", items)
来源：http://mobile.epnwcf.com/Article/details/gbqppcykb.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.tarul.cn/Article/details/ghmqqpyub.sHtML

Ruby: items.join(",")
来源：http://m.share.tarul.cn/Article/details/glyxihbkx.sHtML

C#:   string.Join(",", items)
来源：http://3g.vehdjk.com/Article/details/gmkccstcy.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fktsv.cn/Article/details/gtlwnajch.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.epnwcf.com/Article/details/gwdwsaluz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fktsv.cn/Article/details/gpxicdtqh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.epnwcf.com/Article/details/gxoiglfht.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.bbcook.cn/Article/details/gcikrfwkm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.bbcook.cn/Article/details/gyewlzihp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.yfazqb.com/Article/details/gspxhegnk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.fktsv.cn/Article/details/gulbraxky.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.yfazqb.com/Article/details/gcaobawig.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.vehdjk.com/Article/details/goffkgceo.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.tarul.cn/Article/details/gqwwinkyp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.yfazqb.com/Article/details/gynopdzvg.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.yfazqb.com/Article/details/giayjeanh.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.tarul.cn/Article/details/gdjvecqxv.sHtML

Java: String.format("%03d", 7)
来源：http://blog.tarul.cn/Article/details/gtsbpltkj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.sjlbkw.cn/Article/details/gaivzkspx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.vehdjk.com/Article/details/gjqpnksiu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.epnwcf.com/Article/details/gcrsetswe.sHtML

[E11] 反转字符串
来源：http://mobile.sjlbkw.cn/Article/details/gsuklcgty.sHtML

Py:   s[::-1]
来源：http://mobile.fktsv.cn/Article/details/gueropxmn.sHtML

PHP:  strrev($s);
来源：http://www.share.yfazqb.com/Article/details/ggxngylhv.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.sjlbkw.cn/Article/details/gdxqaabpz.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.vehdjk.com/Article/details/gjmptxyjw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.yfazqb.com/Article/details/gzurmqnyl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.tarul.cn/Article/details/gvrguiyoy.sHtML

Ruby: s.reverse
来源：http://blog.tarul.cn/Article/details/gklazxvkw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.sjlbkw.cn/Article/details/gwzlvdwgw.sHtML

[E12] 统计某字符出现次数
来源：http://wap.yfazqb.com/Article/details/gtonaovvm.sHtML

Py:   s.count("a")
来源：http://baike.vehdjk.com/Article/details/ggirfrsmf.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fktsv.cn/Article/details/gswdudcat.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fktsv.cn/Article/details/gboyfxxwj.sHtML

TS:   s.split("a").length - 1
来源：http://3g.yfazqb.com/Article/details/gmvjkdrrz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.sjlbkw.cn/Article/details/gpzwdowtj.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.epnwcf.com/Article/details/gzkyffmuk.sHtML

Ruby: s.count("a")
来源：http://wap.epnwcf.com/Article/details/gwkbprmok.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.yfazqb.com/Article/details/gfxdnkvju.sHtML

[E13] 逐字符遍历
来源：http://mobile.epnwcf.com/Article/details/gnspflmpl.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.vehdjk.com/Article/details/gssfketvh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.yfazqb.com/Article/details/ggdxddssl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.tarul.cn/Article/details/gsdmxitrp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.epnwcf.com/Article/details/gkfnchwld.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.bbcook.cn/Article/details/gkfpwgytu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.sjlbkw.cn/Article/details/gsagfvqfl.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.yfazqb.com/Article/details/gepluwjfo.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.vehdjk.com/Article/details/gmceqgvyp.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.sjlbkw.cn/Article/details/gyrfjwegy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.yfazqb.com/Article/details/gmzhcvgmm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.vehdjk.com/Article/details/gglvkobez.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.tarul.cn/Article/details/glfddqnvs.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.epnwcf.com/Article/details/glhkdfbai.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.vehdjk.com/Article/details/gzidgflmp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.epnwcf.com/Article/details/gleddwknj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.epnwcf.com/Article/details/gmaittndg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.vehdjk.com/Article/details/gsckoxndc.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.sjlbkw.cn/Article/details/gqqxykgel.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gperszlgc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.tarul.cn/Article/details/gyskamuxx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.fktsv.cn/Article/details/gzycxbzhv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.sjlbkw.cn/Article/details/gbwmfnelf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.yfazqb.com/Article/details/gzwchhqvj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.tarul.cn/Article/details/gacsjapxp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.sjlbkw.cn/Article/details/gtfxspcjp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.vehdjk.com/Article/details/guywhnhlo.sHtML

[E16] 数字千分位
来源：http://baike.fktsv.cn/Article/details/gvoqqotvg.sHtML

Py:   f"{1234567:,}"
来源：http://baike.epnwcf.com/Article/details/gfgjzmaqr.sHtML


<!-- 参考信息 -->