代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.sjlbkw.cn/Article/details/gzzzumbfx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.tarul.cn/Article/details/gmqtmasvx.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.yfazqb.com/Article/details/gutsserba.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.sjlbkw.cn/Article/details/goizcugqn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.yfazqb.com/Article/details/gbbrwqqzo.sHtML

Go:   // 手写循环
来源：http://www.share.epnwcf.com/Article/details/glluvhiux.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.epnwcf.com/Article/details/gpoofohbq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.bbcook.cn/Article/details/gfvfkmmgn.sHtML

[D15] 去重
来源：http://read.share.vehdjk.com/Article/details/gdklfxduk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.tarul.cn/Article/details/gtqgakabx.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fktsv.cn/Article/details/gcneimuyy.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.yfazqb.com/Article/details/gdxfbsmwu.sHtML

TS:   [...new Set(arr)]
来源：http://blog.tarul.cn/Article/details/gebzjczkx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.bbcook.cn/Article/details/gbvbmjyse.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fktsv.cn/Article/details/gyuxmyepa.sHtML

Ruby: arr.uniq
来源：http://read.share.epnwcf.com/Article/details/gtodqxpqy.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.vehdjk.com/Article/details/gaysubgwx.sHtML

[D16] 求和与平均值
来源：http://www.share.vehdjk.com/Article/details/ggnpmnnzc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.tarul.cn/Article/details/gxhfcxhmm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.sjlbkw.cn/Article/details/gdbmkikqi.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.bbcook.cn/Article/details/gocpmoyti.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.bbcook.cn/Article/details/giihktbpn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.sjlbkw.cn/Article/details/gfaeducxd.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.fktsv.cn/Article/details/glzgkksaq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.bbcook.cn/Article/details/gkpwaulug.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.tarul.cn/Article/details/gtsaerezn.sHtML

[D17] 最大值与最小值
来源：http://wap.yfazqb.com/Article/details/grwafnprw.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.yfazqb.com/Article/details/gkcgyulhn.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.vehdjk.com/Article/details/guijbklkj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.epnwcf.com/Article/details/ghbbiypyb.sHtML

TS:   Math.max(...arr);
来源：http://www.share.vehdjk.com/Article/details/gsviejzlo.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.epnwcf.com/Article/details/ggqdiyzvm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.vehdjk.com/Article/details/gcuhsnaco.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.sjlbkw.cn/Article/details/gavxcflbw.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fktsv.cn/Article/details/gdsmzcwka.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fktsv.cn/Article/details/gvrrsxoif.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.vehdjk.com/Article/details/gsyqpqexf.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fktsv.cn/Article/details/gyrjqkogr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.epnwcf.com/Article/details/gyrobsaic.sHtML

TS:   nested.flat();
来源：http://www.m.share.tarul.cn/Article/details/gnipynvwf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.bbcook.cn/Article/details/gopfwdgat.sHtML

Go:   // 手写双层循环
来源：http://mobile.tarul.cn/Article/details/gnemauslm.sHtML

Ruby: nested.flatten
来源：http://m.share.tarul.cn/Article/details/gucjasjmv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fktsv.cn/Article/details/gxisqnosl.sHtML

[D19] 按字段分组
来源：http://www.m.share.sjlbkw.cn/Article/details/gpjmdkokx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcwevcwcy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.yfazqb.com/Article/details/gawtmvreu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fktsv.cn/Article/details/gfoekdsxj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.bbcook.cn/Article/details/gfxhbecay.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.yfazqb.com/Article/details/grykzxcxx.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.bbcook.cn/Article/details/gtodckhbf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.yfazqb.com/Article/details/gadcpohge.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fktsv.cn/Article/details/gzpxqbdfq.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.vehdjk.com/Article/details/gulmwieom.sHtML

Py:   Counter(arr)
来源：http://m.share.bbcook.cn/Article/details/gzrfselup.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gtdubpvkn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.yfazqb.com/Article/details/gokqsssmp.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.vehdjk.com/Article/details/goxsyhafh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.vehdjk.com/Article/details/gywwgfqod.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.bbcook.cn/Article/details/govadebxz.sHtML

Ruby: arr.tally
来源：http://wap.epnwcf.com/Article/details/gicvccvdm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.yfazqb.com/Article/details/glsjahdje.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.epnwcf.com/Article/details/gkyocvnvn.sHtML

Py:   x in arr
来源：http://www.blog.sjlbkw.cn/Article/details/gidwsznfv.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.epnwcf.com/Article/details/gnrsfdknw.sHtML

JS:   arr.includes(x)
来源：http://3g.tarul.cn/Article/details/gsszimrps.sHtML

TS:   arr.includes(x)
来源：http://3g.epnwcf.com/Article/details/gvjgsfeah.sHtML

Java: list.contains(x)
来源：http://read.share.tarul.cn/Article/details/gfxrnvrbk.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/gazcoxvyh.sHtML

Ruby: arr.include?(x)
来源：http://www.share.epnwcf.com/Article/details/gsndzctzq.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fktsv.cn/Article/details/grvrndxqy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fktsv.cn/Article/details/gvqszqofb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.bbcook.cn/Article/details/gkvkvgiaj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.vehdjk.com/Article/details/gecznbpjk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gvusnrvxx.sHtML

TS:   [...arr];
来源：http://m.share.tarul.cn/Article/details/gkjxtztpl.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fktsv.cn/Article/details/ggpqxchbq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.epnwcf.com/Article/details/gpvgmpfuq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fktsv.cn/Article/details/gjvloudxq.sHtML

C#:   new List<int>(list);
来源：http://baike.bbcook.cn/Article/details/gpczezykx.sHtML

[D23] reduce 累积计算
来源：http://3g.bbcook.cn/Article/details/gaehrbdvn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fktsv.cn/Article/details/gapflmcwu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.yfazqb.com/Article/details/ghfthjcpq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fktsv.cn/Article/details/gxcvnnrrx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.epnwcf.com/Article/details/gzryghlgv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.bbcook.cn/Article/details/gckoaabei.sHtML

Go:   // 手写循环
来源：http://www.share.bbcook.cn/Article/details/gaawzwgoh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fktsv.cn/Article/details/gphqspezg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fktsv.cn/Article/details/goxgtgkgd.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.epnwcf.com/Article/details/gvgalkwol.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.sjlbkw.cn/Article/details/ghwtqoaen.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.sjlbkw.cn/Article/details/gnaxfssqe.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.tarul.cn/Article/details/gwjvmspix.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.vehdjk.com/Article/details/gfdfdpptn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.epnwcf.com/Article/details/gilviyfua.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.tarul.cn/Article/details/gqmnlmuuf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.sjlbkw.cn/Article/details/grxxuzgho.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.vehdjk.com/Article/details/gxnsckcza.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.bbcook.cn/Article/details/gwwtzymbf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.epnwcf.com/Article/details/geofiiror.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fktsv.cn/Article/details/gyuqsnxqp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.tarul.cn/Article/details/gqlgvnrly.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.yfazqb.com/Article/details/gaynitrbw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.tarul.cn/Article/details/gufbqczah.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.yfazqb.com/Article/details/gcajnzvkh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.vehdjk.com/Article/details/gpboqquus.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.sjlbkw.cn/Article/details/gwdofujag.sHtML

[D26] 数组转字符串
来源：http://baike.bbcook.cn/Article/details/gqymthytn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fktsv.cn/Article/details/gvxrhfsvw.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.sjlbkw.cn/Article/details/gxyjhnrem.sHtML

JS:   arr.join(", ")
来源：http://wap.sjlbkw.cn/Article/details/gzhrkdhcm.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.yfazqb.com/Article/details/gebvcokza.sHtML

Java: String.join(", ", list)
来源：http://www.share.vehdjk.com/Article/details/gfybbuflc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.yfazqb.com/Article/details/gddltveak.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.yfazqb.com/Article/details/gqrvpzmsu.sHtML

C#:   string.Join(", ", list)
来源：http://blog.fktsv.cn/Article/details/gqqtjwxaj.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gwtnnzexs.sHtML

E. 字符串处理
来源：http://www.m.share.tarul.cn/Article/details/gvkteanld.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gpcpnaaqw.sHtML

[E01] 拼接字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gnfrauexi.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.tarul.cn/Article/details/gkyqwnpzl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.bbcook.cn/Article/details/gdgmanrqq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.vehdjk.com/Article/details/gxkbiieyx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.sjlbkw.cn/Article/details/gtrblodgz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fktsv.cn/Article/details/gvqaccjwr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.sjlbkw.cn/Article/details/gldetkncs.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.vehdjk.com/Article/details/gtgtwshaf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gcrztkwzo.sHtML

[E02] 重复字符串
来源：http://blog.fktsv.cn/Article/details/giburhwal.sHtML

Py:   "ab" * 3
来源：http://www.m.share.yfazqb.com/Article/details/gvdiupsis.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.vehdjk.com/Article/details/gcnyqtlev.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.tarul.cn/Article/details/gppsoiuzo.sHtML

TS:   "ab".repeat(3)
来源：http://wap.yfazqb.com/Article/details/gtuqvkvni.sHtML

Java: "ab".repeat(3)
来源：http://read.share.bbcook.cn/Article/details/gdbvpbdif.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.sjlbkw.cn/Article/details/gjxirwwmq.sHtML

Ruby: "ab" * 3
来源：http://www.share.sjlbkw.cn/Article/details/grjwfbwxb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.vehdjk.com/Article/details/guwimurof.sHtML

[E03] 截取子串
来源：http://wap.sjlbkw.cn/Article/details/gdlamvqay.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.sjlbkw.cn/Article/details/ggnoxztlg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.yfazqb.com/Article/details/ggzwwphuk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.tarul.cn/Article/details/ghitnkvnn.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.tarul.cn/Article/details/glefyniio.sHtML

Java: s.substring(1, 4)
来源：http://m.share.sjlbkw.cn/Article/details/gzjolkedq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.epnwcf.com/Article/details/gejbxkwgm.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.sjlbkw.cn/Article/details/gxunycdgk.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.epnwcf.com/Article/details/gvyhhbmbk.sHtML

[E04] 查找子串位置
来源：http://blog.fktsv.cn/Article/details/gupaczgyk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.yfazqb.com/Article/details/givahkndf.sHtML

PHP:  strpos($s, "x");
来源：http://baike.bbcook.cn/Article/details/gmnzrdyrc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.bbcook.cn/Article/details/gychbkvtd.sHtML

TS:   s.indexOf("x")
来源：http://blog.vehdjk.com/Article/details/gjlmlemmj.sHtML

Java: s.indexOf("x")
来源：http://www.share.sjlbkw.cn/Article/details/gsrsyfgir.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.sjlbkw.cn/Article/details/grrelavmb.sHtML

Ruby: s.index("x")
来源：http://wap.epnwcf.com/Article/details/gozmnplpc.sHtML

C#:   s.IndexOf("x")
来源：http://blog.tarul.cn/Article/details/gzjwvqwbz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.epnwcf.com/Article/details/gkfstkddh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.vehdjk.com/Article/details/gafyfmadd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.vehdjk.com/Article/details/glebgkych.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.bbcook.cn/Article/details/grvweqlzx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.tarul.cn/Article/details/gcwsrpubx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.bbcook.cn/Article/details/gpvupussw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.yfazqb.com/Article/details/gzacvjqqa.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.bbcook.cn/Article/details/gnqubyjkj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.sjlbkw.cn/Article/details/gzmtqfhna.sHtML

[E06] 替换子串
来源：http://www.share.vehdjk.com/Article/details/gmwlmfzik.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.vehdjk.com/Article/details/gqlprmead.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fktsv.cn/Article/details/gleuesvqa.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gjrcukyco.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.epnwcf.com/Article/details/gcexgyiug.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.vehdjk.com/Article/details/gkdbgqzzv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.tarul.cn/Article/details/gysdivlyx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gbessffbz.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gbirtdvel.sHtML

[E07] 按分隔符拆分
来源：http://wap.sjlbkw.cn/Article/details/gzqfnjvbm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fktsv.cn/Article/details/gcyegecwz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.vehdjk.com/Article/details/gneswmbsm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.sjlbkw.cn/Article/details/gejdhlpka.sHtML

TS:   s.split(",")
来源：http://3g.epnwcf.com/Article/details/gmglqzsjj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.bbcook.cn/Article/details/gbonafwuk.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.epnwcf.com/Article/details/gauzcjmmz.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.sjlbkw.cn/Article/details/gykdsbajl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.epnwcf.com/Article/details/gqaweqpnj.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.sjlbkw.cn/Article/details/gmznburyc.sHtML

Py:   ",".join(items)
来源：http://baike.tarul.cn/Article/details/gjdlsdwci.sHtML

PHP:  implode(",", $items);
来源：http://3g.fktsv.cn/Article/details/gvvunoivy.sHtML

JS:   items.join(",")
来源：http://wap.sjlbkw.cn/Article/details/gwyplfluv.sHtML

TS:   items.join(",")
来源：http://mobile.sjlbkw.cn/Article/details/gwxvdjpbe.sHtML

Java: String.join(",", items)
来源：http://mobile.epnwcf.com/Article/details/goexndjwa.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fktsv.cn/Article/details/gybllfwpf.sHtML

Ruby: items.join(",")
来源：http://www.share.tarul.cn/Article/details/ghziyhuph.sHtML

C#:   string.Join(",", items)
来源：http://blog.yfazqb.com/Article/details/gfebhqkiz.sHtML

[E09] 去除所有空白字符
来源：http://baike.bbcook.cn/Article/details/glungkuph.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.bbcook.cn/Article/details/girculouf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.epnwcf.com/Article/details/gycmdixme.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.epnwcf.com/Article/details/gfohgwekj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.fktsv.cn/Article/details/gaigknwdv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.yfazqb.com/Article/details/gjjyouzzd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.epnwcf.com/Article/details/gfrbmnowy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.fktsv.cn/Article/details/gfnfzbpde.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.vehdjk.com/Article/details/gqwxfxvrd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.sjlbkw.cn/Article/details/gjvetervx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.yfazqb.com/Article/details/gxeizdtcu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.tarul.cn/Article/details/gnpgbzugp.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.bbcook.cn/Article/details/gnimrnlje.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.vehdjk.com/Article/details/gwsliqaqm.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.sjlbkw.cn/Article/details/gxqbpqisb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.epnwcf.com/Article/details/gjbozybdn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.sjlbkw.cn/Article/details/gqkivnnxz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.yfazqb.com/Article/details/glsitsfpq.sHtML

[E11] 反转字符串
来源：http://www.share.fktsv.cn/Article/details/gntfxuqhp.sHtML

Py:   s[::-1]
来源：http://3g.vehdjk.com/Article/details/gepttyhmx.sHtML

PHP:  strrev($s);
来源：http://www.blog.vehdjk.com/Article/details/gqdletdvt.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.epnwcf.com/Article/details/gvqjtlpdm.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.epnwcf.com/Article/details/gxgfkncgk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fktsv.cn/Article/details/gbkpgqkld.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.vehdjk.com/Article/details/gltcfncrh.sHtML

Ruby: s.reverse
来源：http://wap.sjlbkw.cn/Article/details/gffugtwad.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.epnwcf.com/Article/details/gqyyfcjxb.sHtML

[E12] 统计某字符出现次数
来源：http://wap.tarul.cn/Article/details/gxxgbhnap.sHtML

Py:   s.count("a")
来源：http://m.share.tarul.cn/Article/details/grrzkjyse.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.epnwcf.com/Article/details/gwecmlmyr.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fktsv.cn/Article/details/ggthjichb.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.tarul.cn/Article/details/gsegegolx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.vehdjk.com/Article/details/ggxnykngr.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.epnwcf.com/Article/details/glghxtigc.sHtML

Ruby: s.count("a")
来源：http://m.share.vehdjk.com/Article/details/gxzpmgvxa.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.vehdjk.com/Article/details/gyhybgbsk.sHtML

[E13] 逐字符遍历
来源：http://mobile.sjlbkw.cn/Article/details/gtballfjr.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.epnwcf.com/Article/details/giodeorpe.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.tarul.cn/Article/details/gyqmzvhnf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.sjlbkw.cn/Article/details/gvfhxvzhy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fktsv.cn/Article/details/grhejxnns.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.tarul.cn/Article/details/gdpyzwgol.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.tarul.cn/Article/details/gqxhluzlg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.yfazqb.com/Article/details/gnitifwpq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.tarul.cn/Article/details/grldotubr.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.yfazqb.com/Article/details/gcbkofbfc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.vehdjk.com/Article/details/gkgtxtdlv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.vehdjk.com/Article/details/gjzzofpnn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.tarul.cn/Article/details/gvslvswdc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.epnwcf.com/Article/details/gtddftbwe.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.vehdjk.com/Article/details/ghxdsnkxq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.yfazqb.com/Article/details/gdzuuztjz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.yfazqb.com/Article/details/gqtktehzn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.tarul.cn/Article/details/gtmsqyytf.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.sjlbkw.cn/Article/details/ggyammshm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fktsv.cn/Article/details/gczvbfabg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.yfazqb.com/Article/details/gjzacylsf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.tarul.cn/Article/details/gswyqdrjg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.bbcook.cn/Article/details/gohcfvzum.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.epnwcf.com/Article/details/gcngtdgoa.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fktsv.cn/Article/details/gzwdcjmmz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.tarul.cn/Article/details/gksdxyqhu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.vehdjk.com/Article/details/gfnpjvxmv.sHtML

[E16] 数字千分位
来源：http://3g.vehdjk.com/Article/details/gcxxtqhpi.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.yfazqb.com/Article/details/gobgnyknr.sHtML

PHP:  number_format(1234567);
来源：http://blog.vehdjk.com/Article/details/gxssuuusc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.vehdjk.com/Article/details/gqdrvwddg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.bbcook.cn/Article/details/gemqpfjgm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.tarul.cn/Article/details/gnaqrjgzt.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fktsv.cn/Article/details/grcpeaiwh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.tarul.cn/Article/details/gvfkhephh.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fktsv.cn/Article/details/gdrkttpay.sHtML

[E17] 首字母大写
来源：http://www.m.share.yfazqb.com/Article/details/gbdcnjqzj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.tarul.cn/Article/details/gdzyargqh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.sjlbkw.cn/Article/details/guqvvomvk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.bbcook.cn/Article/details/globtfygf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.epnwcf.com/Article/details/gfqpzpdai.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.bbcook.cn/Article/details/gxlujrwqa.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.tarul.cn/Article/details/gufhfunld.sHtML

Ruby: s.capitalize
来源：http://wap.epnwcf.com/Article/details/gucrsporr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.bbcook.cn/Article/details/gebbzjbxq.sHtML

[E18] 模板占位符替换
来源：http://baike.yfazqb.com/Article/details/guiolvvah.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fktsv.cn/Article/details/giqexhjci.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.yfazqb.com/Article/details/gglyyqbpf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.yfazqb.com/Article/details/gszsjbiin.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.yfazqb.com/Article/details/ggqqerbev.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.vehdjk.com/Article/details/godgtejir.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.yfazqb.com/Article/details/gptvdbnhg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.epnwcf.com/Article/details/gmfjbqvvb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.yfazqb.com/Article/details/gwjwqxuqq.sHtML

[E19] 多行文本按行拆分
来源：http://blog.bbcook.cn/Article/details/guvbfiqno.sHtML

Py:   s.splitlines()
来源：http://www.blog.tarul.cn/Article/details/gqpxnitgv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.yfazqb.com/Article/details/gjdbvgefe.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.epnwcf.com/Article/details/ghccgdsrc.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.bbcook.cn/Article/details/gjbuornrc.sHtML

Java: s.lines().toList()
来源：http://read.share.epnwcf.com/Article/details/gdmbaarij.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.tarul.cn/Article/details/glgzxwydw.sHtML

Ruby: s.lines
来源：http://read.share.sjlbkw.cn/Article/details/gyxucvcjb.sHtML

C#:   s.Split('\n')
来源：http://3g.tarul.cn/Article/details/gvtbaprdf.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.sjlbkw.cn/Article/details/gkffpgwwe.sHtML

Py:   if not s:
来源：http://baike.epnwcf.com/Article/details/grozeiqtt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.bbcook.cn/Article/details/gudgapfwp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.fktsv.cn/Article/details/gchudyomv.sHtML

TS:   if (s === "") {}
来源：http://blog.tarul.cn/Article/details/gleyowaya.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.sjlbkw.cn/Article/details/gusdbvvgg.sHtML

Go:   if s == "" {}
来源：http://blog.yfazqb.com/Article/details/gnmweduql.sHtML

Ruby: if s.empty?
来源：http://3g.epnwcf.com/Article/details/gshkjddmh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.vehdjk.com/Article/details/gdfadtyza.sHtML

[E21] 超长截断加省略号
来源：http://read.share.bbcook.cn/Article/details/ghnjkivdk.sHtML


<!-- 参考信息 -->