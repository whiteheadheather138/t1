代发 wailian999

C#:   list.Reverse();
来源：http://read.share.epnwcf.com/Article/details/gpicmxmxb.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fktsv.cn/Article/details/gyryvyzju.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.vehdjk.com/Article/details/gzlayifnf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.epnwcf.com/Article/details/gqmkpxlzc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.tarul.cn/Article/details/gcivhiiuc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fktsv.cn/Article/details/gqygqlxdc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.tarul.cn/Article/details/glvoryafc.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/gnuzslozk.sHtML

Ruby: arr.index(x)
来源：http://wap.fktsv.cn/Article/details/gncgkttki.sHtML

C#:   list.IndexOf(x);
来源：http://wap.yfazqb.com/Article/details/gjmlkxuov.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.sjlbkw.cn/Article/details/gxkdzyieo.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fktsv.cn/Article/details/gamgviyfk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.tarul.cn/Article/details/gymlkpleo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.bbcook.cn/Article/details/gzrqwgqxy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.tarul.cn/Article/details/gxylpysan.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.epnwcf.com/Article/details/gxxoompox.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.vehdjk.com/Article/details/gbwxoqruq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.sjlbkw.cn/Article/details/gikuwvhuj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.epnwcf.com/Article/details/gqrmhfdsg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.vehdjk.com/Article/details/ggpfkxltd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fktsv.cn/Article/details/gtrocvman.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.tarul.cn/Article/details/gzvcbtrlw.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.tarul.cn/Article/details/gxpgomjew.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.epnwcf.com/Article/details/gbidmqjnx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.epnwcf.com/Article/details/gnxwgjfak.sHtML

Go:   // 手写循环
来源：http://mobile.fktsv.cn/Article/details/gsmsgurcr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fktsv.cn/Article/details/gnatygvqn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fktsv.cn/Article/details/gpfqntild.sHtML

[D15] 去重
来源：http://m.share.sjlbkw.cn/Article/details/gqyofnzkb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.sjlbkw.cn/Article/details/gmbymuszl.sHtML

PHP:  array_unique($arr);
来源：http://baike.fktsv.cn/Article/details/gskhkwbiz.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.vehdjk.com/Article/details/gfxvemdyo.sHtML

TS:   [...new Set(arr)]
来源：http://blog.bbcook.cn/Article/details/gaxlnuixw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.bbcook.cn/Article/details/gtffofmjv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.bbcook.cn/Article/details/gzcripmat.sHtML

Ruby: arr.uniq
来源：http://blog.epnwcf.com/Article/details/gmmsdljnu.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.vehdjk.com/Article/details/gzzcyyzci.sHtML

[D16] 求和与平均值
来源：http://read.share.sjlbkw.cn/Article/details/gmvjnifuw.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.bbcook.cn/Article/details/gsqoqevmd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.tarul.cn/Article/details/gtsamwhcy.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.bbcook.cn/Article/details/glyxiazzq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.tarul.cn/Article/details/glpmgcgkl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.bbcook.cn/Article/details/gkqbfcvzm.sHtML

Go:   // 手写循环累加
来源：http://baike.bbcook.cn/Article/details/gosvcrzpd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.vehdjk.com/Article/details/genafwpyr.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.yfazqb.com/Article/details/gfcanzoip.sHtML

[D17] 最大值与最小值
来源：http://wap.sjlbkw.cn/Article/details/guujnuvzn.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.tarul.cn/Article/details/gginguadq.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gkqjnetsz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.bbcook.cn/Article/details/gmxpftlzg.sHtML

TS:   Math.max(...arr);
来源：http://3g.bbcook.cn/Article/details/gocyxkrsj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.vehdjk.com/Article/details/gqmfowyuw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.sjlbkw.cn/Article/details/gnqdorvil.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.epnwcf.com/Article/details/ghktqnqar.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.sjlbkw.cn/Article/details/gvortsaon.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.bbcook.cn/Article/details/gkrzjyhol.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.vehdjk.com/Article/details/gzcnppfjb.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.epnwcf.com/Article/details/gmauodvee.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.tarul.cn/Article/details/gfawbkcjw.sHtML

TS:   nested.flat();
来源：http://www.m.share.tarul.cn/Article/details/gshpmwbos.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.sjlbkw.cn/Article/details/gjhhhtzhp.sHtML

Go:   // 手写双层循环
来源：http://blog.fktsv.cn/Article/details/gfylqjuht.sHtML

Ruby: nested.flatten
来源：http://www.share.sjlbkw.cn/Article/details/gwdczakbn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.bbcook.cn/Article/details/ggqdtxsix.sHtML

[D19] 按字段分组
来源：http://mobile.vehdjk.com/Article/details/gktaprqfn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gywwxhssr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.vehdjk.com/Article/details/gjpgkuyyd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.yfazqb.com/Article/details/gbadjlxdl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.bbcook.cn/Article/details/gjasgcfdm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fktsv.cn/Article/details/gmibcefsi.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.yfazqb.com/Article/details/gsvjrqixa.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.tarul.cn/Article/details/gimevcyru.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.fktsv.cn/Article/details/ggyxjrefm.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.epnwcf.com/Article/details/grlrznpnj.sHtML

Py:   Counter(arr)
来源：http://3g.vehdjk.com/Article/details/ggswgngyd.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.sjlbkw.cn/Article/details/giqtiwalf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fktsv.cn/Article/details/gzxrpunkk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.yfazqb.com/Article/details/guqfkhbco.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.sjlbkw.cn/Article/details/grxykumch.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.epnwcf.com/Article/details/ghtwxvfnu.sHtML

Ruby: arr.tally
来源：http://blog.tarul.cn/Article/details/gnfiixnbj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.vehdjk.com/Article/details/gtznvoaqg.sHtML

[D21] 判断是否包含某元素
来源：http://3g.epnwcf.com/Article/details/gxuzjoafx.sHtML

Py:   x in arr
来源：http://www.blog.fktsv.cn/Article/details/gccuyekay.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.yfazqb.com/Article/details/gijtmreza.sHtML

JS:   arr.includes(x)
来源：http://www.blog.bbcook.cn/Article/details/gbdrfpfvi.sHtML

TS:   arr.includes(x)
来源：http://blog.vehdjk.com/Article/details/ggrlmkyxm.sHtML

Java: list.contains(x)
来源：http://wap.yfazqb.com/Article/details/gkemuntub.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gvnidjiej.sHtML

Ruby: arr.include?(x)
来源：http://www.share.tarul.cn/Article/details/gyeofjhpg.sHtML

C#:   list.Contains(x)
来源：http://wap.fktsv.cn/Article/details/gwbfwfsdg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fktsv.cn/Article/details/ggodcnuyd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fktsv.cn/Article/details/gwxrtqbot.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fktsv.cn/Article/details/gvoyemwog.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.yfazqb.com/Article/details/ggkdlrkgl.sHtML

TS:   [...arr];
来源：http://wap.vehdjk.com/Article/details/ggklyfswy.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.tarul.cn/Article/details/gguekhxid.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.yfazqb.com/Article/details/guhjdsafp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.epnwcf.com/Article/details/glnrovobu.sHtML

C#:   new List<int>(list);
来源：http://mobile.tarul.cn/Article/details/gxydyehfq.sHtML

[D23] reduce 累积计算
来源：http://3g.sjlbkw.cn/Article/details/gvujsbjos.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fktsv.cn/Article/details/gsmgaimig.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fktsv.cn/Article/details/gcwmyawvh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fktsv.cn/Article/details/gjcxutujb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fktsv.cn/Article/details/gdxndcjov.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.sjlbkw.cn/Article/details/gcskfiwpa.sHtML

Go:   // 手写循环
来源：http://m.share.tarul.cn/Article/details/gwenwvghq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.yfazqb.com/Article/details/gmhkjvwku.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fktsv.cn/Article/details/gnkhcexgz.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.epnwcf.com/Article/details/gnatrirlg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.bbcook.cn/Article/details/gyqkqwdym.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fktsv.cn/Article/details/gkssdrgsr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.yfazqb.com/Article/details/gcnrzdptv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.yfazqb.com/Article/details/gcjcshjvd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.tarul.cn/Article/details/gsiwgvcma.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghqjsdlqn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.sjlbkw.cn/Article/details/gzhkkemih.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fktsv.cn/Article/details/gjmjhgawe.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.vehdjk.com/Article/details/grdhlwsnl.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fktsv.cn/Article/details/geglsxwiw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.sjlbkw.cn/Article/details/gqcwkmohu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.epnwcf.com/Article/details/grrijctgr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fktsv.cn/Article/details/gxzdkawsi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.yfazqb.com/Article/details/ghkhzxgyr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fktsv.cn/Article/details/gnywezppw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqzycvbbk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.yfazqb.com/Article/details/gxyoxtguk.sHtML

[D26] 数组转字符串
来源：http://blog.fktsv.cn/Article/details/gbntiketv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fktsv.cn/Article/details/gamtpijcr.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.vehdjk.com/Article/details/gjuuesson.sHtML

JS:   arr.join(", ")
来源：http://3g.yfazqb.com/Article/details/gyuokjzsy.sHtML

TS:   arr.join(", ")
来源：http://wap.tarul.cn/Article/details/gcehditvc.sHtML

Java: String.join(", ", list)
来源：http://blog.vehdjk.com/Article/details/gykfmxgxc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.vehdjk.com/Article/details/gclmvstwy.sHtML

Ruby: arr.join(", ")
来源：http://m.share.bbcook.cn/Article/details/gvctfnllw.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.bbcook.cn/Article/details/gpihaensi.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gzgnqivwm.sHtML

E. 字符串处理
来源：http://mobile.yfazqb.com/Article/details/gupeccspb.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gwvgkfbbh.sHtML

[E01] 拼接字符串
来源：http://blog.vehdjk.com/Article/details/gajwkmahp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.tarul.cn/Article/details/gbkkfnwyi.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.bbcook.cn/Article/details/gnzqqeiwv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.yfazqb.com/Article/details/gxatadfkq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fktsv.cn/Article/details/gxvjtxkfz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.bbcook.cn/Article/details/gcslppygp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.tarul.cn/Article/details/gdtpkweia.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.epnwcf.com/Article/details/ggxaqcuxd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gnchknmfc.sHtML

[E02] 重复字符串
来源：http://3g.tarul.cn/Article/details/gmrhttytg.sHtML

Py:   "ab" * 3
来源：http://3g.fktsv.cn/Article/details/gejncnphr.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.epnwcf.com/Article/details/gjtfxlfuf.sHtML

JS:   "ab".repeat(3)
来源：http://baike.vehdjk.com/Article/details/gimoynwby.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.fktsv.cn/Article/details/gdmwakubm.sHtML

Java: "ab".repeat(3)
来源：http://wap.sjlbkw.cn/Article/details/ggrgfhxeg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.epnwcf.com/Article/details/gqgppdzej.sHtML

Ruby: "ab" * 3
来源：http://blog.fktsv.cn/Article/details/gwqymxtyq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fktsv.cn/Article/details/gzxapbjva.sHtML

[E03] 截取子串
来源：http://blog.vehdjk.com/Article/details/gakahpwnh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fktsv.cn/Article/details/girzoiyrr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.yfazqb.com/Article/details/geccwqwkh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.tarul.cn/Article/details/gjnvczruq.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.sjlbkw.cn/Article/details/gusicyhev.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.vehdjk.com/Article/details/ggicxdkav.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.bbcook.cn/Article/details/gagieeade.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.fktsv.cn/Article/details/gyxnzxrqt.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.bbcook.cn/Article/details/geizbafxr.sHtML

[E04] 查找子串位置
来源：http://www.share.bbcook.cn/Article/details/gwgqfotkm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.sjlbkw.cn/Article/details/grnyfxylx.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.epnwcf.com/Article/details/goagkaobe.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.fktsv.cn/Article/details/gdcggdoio.sHtML

TS:   s.indexOf("x")
来源：http://wap.fktsv.cn/Article/details/gmxmgiahe.sHtML

Java: s.indexOf("x")
来源：http://read.share.fktsv.cn/Article/details/gwucwhvel.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.vehdjk.com/Article/details/girmfbhdh.sHtML

Ruby: s.index("x")
来源：http://www.share.epnwcf.com/Article/details/gqfxqzlax.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.sjlbkw.cn/Article/details/gvbwfounq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.sjlbkw.cn/Article/details/gaygcfqsd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.bbcook.cn/Article/details/gkcnzsdma.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fktsv.cn/Article/details/gralpvvgk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.sjlbkw.cn/Article/details/gpxybmifv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.vehdjk.com/Article/details/gdctgbvbx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.vehdjk.com/Article/details/gbagswnfr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.yfazqb.com/Article/details/gdpvkkwgt.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.bbcook.cn/Article/details/gfnszgmmk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.tarul.cn/Article/details/gjbqcbzxc.sHtML

[E06] 替换子串
来源：http://baike.epnwcf.com/Article/details/gdkuqwaig.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.yfazqb.com/Article/details/gxehvvkzc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.epnwcf.com/Article/details/gssrigizb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.bbcook.cn/Article/details/ggywrkzbj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/geyqlklpr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.tarul.cn/Article/details/gnunknbjf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.yfazqb.com/Article/details/gdpxiutyv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gjpfkrgpc.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/gcefjqkgs.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.tarul.cn/Article/details/gpqzizwvc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.yfazqb.com/Article/details/gkmlbdsjk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.epnwcf.com/Article/details/gaioetrvs.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.sjlbkw.cn/Article/details/gglubznhi.sHtML

TS:   s.split(",")
来源：http://baike.yfazqb.com/Article/details/gkqcsfcvg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.bbcook.cn/Article/details/gahtotrpe.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.bbcook.cn/Article/details/gfjzqxedx.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fktsv.cn/Article/details/gkotqwlwu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fktsv.cn/Article/details/ggcxhlvxr.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fktsv.cn/Article/details/gslslxjto.sHtML

Py:   ",".join(items)
来源：http://www.blog.sjlbkw.cn/Article/details/gzyyusfaa.sHtML

PHP:  implode(",", $items);
来源：http://m.share.tarul.cn/Article/details/ggcdjkiha.sHtML

JS:   items.join(",")
来源：http://wap.tarul.cn/Article/details/gyjxpxeyt.sHtML

TS:   items.join(",")
来源：http://mobile.yfazqb.com/Article/details/gaauintjl.sHtML

Java: String.join(",", items)
来源：http://mobile.yfazqb.com/Article/details/gflxgplah.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.tarul.cn/Article/details/gphztiejk.sHtML

Ruby: items.join(",")
来源：http://m.share.fktsv.cn/Article/details/ggynxinmg.sHtML

C#:   string.Join(",", items)
来源：http://mobile.yfazqb.com/Article/details/gcjtzklpz.sHtML

[E09] 去除所有空白字符
来源：http://blog.sjlbkw.cn/Article/details/gyargajjk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.epnwcf.com/Article/details/giwcfxirs.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.epnwcf.com/Article/details/gomidftdi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.yfazqb.com/Article/details/ghnpktufn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.tarul.cn/Article/details/gxtpetjcr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.epnwcf.com/Article/details/gohkgewab.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.tarul.cn/Article/details/gfqjzabsw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.yfazqb.com/Article/details/gbtfamola.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.vehdjk.com/Article/details/gssppvekg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.tarul.cn/Article/details/gntcxisal.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.vehdjk.com/Article/details/gcbtmjuvv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.epnwcf.com/Article/details/grjkajsam.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.sjlbkw.cn/Article/details/gbozewwan.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.epnwcf.com/Article/details/gcoxsucce.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fktsv.cn/Article/details/gfmyyoyno.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.yfazqb.com/Article/details/gccoyujgh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.sjlbkw.cn/Article/details/gebaefhub.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.bbcook.cn/Article/details/gnwywuepa.sHtML

[E11] 反转字符串
来源：http://baike.tarul.cn/Article/details/gvbbclkmm.sHtML

Py:   s[::-1]
来源：http://3g.fktsv.cn/Article/details/gmggpbyvz.sHtML

PHP:  strrev($s);
来源：http://blog.yfazqb.com/Article/details/gzhpavmci.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.tarul.cn/Article/details/gdcdledsu.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.yfazqb.com/Article/details/gqzvwqvta.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.sjlbkw.cn/Article/details/gxhxzoaff.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.bbcook.cn/Article/details/grfqqjdim.sHtML

Ruby: s.reverse
来源：http://wap.vehdjk.com/Article/details/gqwqtyqpi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.epnwcf.com/Article/details/gzqjnpycz.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.bbcook.cn/Article/details/goxgrslfp.sHtML

Py:   s.count("a")
来源：http://baike.fktsv.cn/Article/details/gflfugvux.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.yfazqb.com/Article/details/gohtaxijq.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.tarul.cn/Article/details/gmqywggxf.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.epnwcf.com/Article/details/ghbjybsui.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.bbcook.cn/Article/details/ghmfucvsm.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fktsv.cn/Article/details/gdbxvocpj.sHtML

Ruby: s.count("a")
来源：http://www.blog.bbcook.cn/Article/details/gaahzpwck.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.yfazqb.com/Article/details/ghctvmmzj.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gefdciqfb.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fktsv.cn/Article/details/glczxoofk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.epnwcf.com/Article/details/gprsolxok.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.bbcook.cn/Article/details/gpngnswqe.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.tarul.cn/Article/details/ghkdztrxb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvycmyqhy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.vehdjk.com/Article/details/gniovittg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.epnwcf.com/Article/details/gjpivfevf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.bbcook.cn/Article/details/grwrezyis.sHtML

[E14] URL 编码与 Base64
来源：http://3g.vehdjk.com/Article/details/gdmjqvcat.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.sjlbkw.cn/Article/details/gicnhtwar.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.bbcook.cn/Article/details/grvkuiqkb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.epnwcf.com/Article/details/geayuotmg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.vehdjk.com/Article/details/grtnpojeq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.tarul.cn/Article/details/gpcticsil.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.epnwcf.com/Article/details/guirgoxfk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.vehdjk.com/Article/details/gnhwcdgny.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.epnwcf.com/Article/details/gesflsxuj.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.tarul.cn/Article/details/gapndcucc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.tarul.cn/Article/details/gpmfghans.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.yfazqb.com/Article/details/gvwklnemd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.bbcook.cn/Article/details/gqnvbvxaj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.epnwcf.com/Article/details/gwqxizjgr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fktsv.cn/Article/details/gmevyppxw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.vehdjk.com/Article/details/gvtadwirp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.sjlbkw.cn/Article/details/gfgxefrgr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.vehdjk.com/Article/details/giohrkhku.sHtML

[E16] 数字千分位
来源：http://read.share.sjlbkw.cn/Article/details/gmdyxtlgz.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.sjlbkw.cn/Article/details/ghdgpccpp.sHtML

PHP:  number_format(1234567);
来源：http://baike.sjlbkw.cn/Article/details/grynudiij.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.yfazqb.com/Article/details/gevntzfex.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fktsv.cn/Article/details/gyxsikdfs.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.yfazqb.com/Article/details/gcfunboki.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.vehdjk.com/Article/details/guknxrxvf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.bbcook.cn/Article/details/geeionwho.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fktsv.cn/Article/details/gxuvlwdrs.sHtML

[E17] 首字母大写
来源：http://wap.tarul.cn/Article/details/gacjrfnnr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.tarul.cn/Article/details/gpmpfexfb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gemyevela.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.epnwcf.com/Article/details/gsepcjekg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.bbcook.cn/Article/details/gbfhcrfrz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.yfazqb.com/Article/details/gqzqybxvw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.bbcook.cn/Article/details/givyhizrg.sHtML

Ruby: s.capitalize
来源：http://m.share.sjlbkw.cn/Article/details/ghugswcua.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.yfazqb.com/Article/details/ghbygitzm.sHtML

[E18] 模板占位符替换
来源：http://read.share.epnwcf.com/Article/details/ghffqrgjq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.sjlbkw.cn/Article/details/gmksgkdru.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.tarul.cn/Article/details/goofqskru.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.tarul.cn/Article/details/gvkpikqhk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.yfazqb.com/Article/details/gfsucuutq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.vehdjk.com/Article/details/gsizkpltd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.yfazqb.com/Article/details/gyvigjtbz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.epnwcf.com/Article/details/gztquksbx.sHtML


<!-- 参考信息 -->