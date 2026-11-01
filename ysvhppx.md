代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.sjlbkw.cn/Article/details/gudfscukt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.tarul.cn/Article/details/gyhrwdoxx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.bbcook.cn/Article/details/ggiwpwreu.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gwlnxekec.sHtML

Ruby: arr.index(x)
来源：http://www.share.epnwcf.com/Article/details/goztyiwgf.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.bbcook.cn/Article/details/gluwwbftd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.bbcook.cn/Article/details/gmtvlilsc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.vehdjk.com/Article/details/guuyjhzxw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.epnwcf.com/Article/details/glwwaqdsb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.tarul.cn/Article/details/gtvrgkime.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.sjlbkw.cn/Article/details/gutocjaqz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.sjlbkw.cn/Article/details/gsttwfvpc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.yfazqb.com/Article/details/grmzymovk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.bbcook.cn/Article/details/givbvlsaf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.yfazqb.com/Article/details/gsbdlbfzg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.yfazqb.com/Article/details/gvekzfltf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.tarul.cn/Article/details/gtgwtsyuv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.vehdjk.com/Article/details/gzzxxaudk.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.yfazqb.com/Article/details/gbqeyxkgp.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.yfazqb.com/Article/details/gmzmfjpfs.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.sjlbkw.cn/Article/details/gvquntktc.sHtML

Go:   // 手写循环
来源：http://wap.sjlbkw.cn/Article/details/gbcfqhqpf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.bbcook.cn/Article/details/gnnjfrbpu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.yfazqb.com/Article/details/gdgqqhwgh.sHtML

[D15] 去重
来源：http://wap.sjlbkw.cn/Article/details/gifxcmcrm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.bbcook.cn/Article/details/gtzrrocwj.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fktsv.cn/Article/details/gvsjksbfa.sHtML

JS:   [...new Set(arr)]
来源：http://wap.yfazqb.com/Article/details/gwrgmixir.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.tarul.cn/Article/details/glmgdlfpv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.sjlbkw.cn/Article/details/grimudcjo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.yfazqb.com/Article/details/guukpznvi.sHtML

Ruby: arr.uniq
来源：http://blog.tarul.cn/Article/details/goavfyigh.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fktsv.cn/Article/details/gasgyoecj.sHtML

[D16] 求和与平均值
来源：http://baike.sjlbkw.cn/Article/details/gahvdjhej.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.vehdjk.com/Article/details/gxznnlnhq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.tarul.cn/Article/details/gfyrgwwza.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.yfazqb.com/Article/details/gdtfudhcr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.vehdjk.com/Article/details/gbgpmhzqu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.tarul.cn/Article/details/gbuovxqwj.sHtML

Go:   // 手写循环累加
来源：http://blog.fktsv.cn/Article/details/geuasdsaq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.tarul.cn/Article/details/gqtfubzhy.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.tarul.cn/Article/details/gkqrbtzuu.sHtML

[D17] 最大值与最小值
来源：http://m.share.vehdjk.com/Article/details/gmgmqtfvl.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.vehdjk.com/Article/details/gosjhnrmx.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.sjlbkw.cn/Article/details/ghbtxgckb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.bbcook.cn/Article/details/gbkzwheqi.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fktsv.cn/Article/details/glldmemfp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.yfazqb.com/Article/details/gbsmfuvpx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.vehdjk.com/Article/details/gakczbeay.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.epnwcf.com/Article/details/gcfburvhn.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.yfazqb.com/Article/details/gwkjorswg.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.tarul.cn/Article/details/ghoiobjwb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.bbcook.cn/Article/details/gfpyzreci.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.tarul.cn/Article/details/glpyadpap.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.epnwcf.com/Article/details/gaqgehqov.sHtML

TS:   nested.flat();
来源：http://www.blog.fktsv.cn/Article/details/ggogmwpft.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fktsv.cn/Article/details/gfakuzaxt.sHtML

Go:   // 手写双层循环
来源：http://read.share.epnwcf.com/Article/details/gcgqlpadz.sHtML

Ruby: nested.flatten
来源：http://www.m.share.sjlbkw.cn/Article/details/gxkghtvxt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.bbcook.cn/Article/details/gepglkdhn.sHtML

[D19] 按字段分组
来源：http://blog.tarul.cn/Article/details/gmivritec.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.bbcook.cn/Article/details/gidsyiznv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.yfazqb.com/Article/details/gddxnnmof.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.vehdjk.com/Article/details/gsqogznxu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.yfazqb.com/Article/details/grhwthuzq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.epnwcf.com/Article/details/gccaxmrqu.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.bbcook.cn/Article/details/gkjncszgx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.sjlbkw.cn/Article/details/gyrlzyfnc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.sjlbkw.cn/Article/details/gyieauwpk.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.yfazqb.com/Article/details/gibtravth.sHtML

Py:   Counter(arr)
来源：http://mobile.bbcook.cn/Article/details/gyolciwzr.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.sjlbkw.cn/Article/details/gpmtsuchi.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.vehdjk.com/Article/details/gibodafkr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.sjlbkw.cn/Article/details/gvjbjhwde.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.bbcook.cn/Article/details/gumthyfib.sHtML

Go:   // 手写 map[T]int
来源：http://3g.vehdjk.com/Article/details/ggvkrqjyn.sHtML

Ruby: arr.tally
来源：http://www.m.share.vehdjk.com/Article/details/guuautypw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.yfazqb.com/Article/details/gdjmioxsn.sHtML

[D21] 判断是否包含某元素
来源：http://blog.bbcook.cn/Article/details/gbsaksjvl.sHtML

Py:   x in arr
来源：http://wap.epnwcf.com/Article/details/gbbfiuwhb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.tarul.cn/Article/details/gvuorrtjo.sHtML

JS:   arr.includes(x)
来源：http://3g.epnwcf.com/Article/details/gcrnddkdl.sHtML

TS:   arr.includes(x)
来源：http://wap.sjlbkw.cn/Article/details/gobjdzpuv.sHtML

Java: list.contains(x)
来源：http://blog.tarul.cn/Article/details/galhtophk.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.vehdjk.com/Article/details/gwesdtlhf.sHtML

Ruby: arr.include?(x)
来源：http://read.share.tarul.cn/Article/details/gniublzze.sHtML

C#:   list.Contains(x)
来源：http://read.share.yfazqb.com/Article/details/gpoyqmfuj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.sjlbkw.cn/Article/details/gsdsinfte.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.tarul.cn/Article/details/gxooakemd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.yfazqb.com/Article/details/gfolimrok.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gpgkelsck.sHtML

TS:   [...arr];
来源：http://3g.fktsv.cn/Article/details/gofwuyntw.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.bbcook.cn/Article/details/gytqxvtnd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.tarul.cn/Article/details/gsujgdzok.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.epnwcf.com/Article/details/gnbrhgpdg.sHtML

C#:   new List<int>(list);
来源：http://blog.yfazqb.com/Article/details/gokoyhttj.sHtML

[D23] reduce 累积计算
来源：http://www.share.sjlbkw.cn/Article/details/gjbtfoanq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.vehdjk.com/Article/details/gahfbqrxk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.yfazqb.com/Article/details/gzmzigbli.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.vehdjk.com/Article/details/guhhjxhnr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fktsv.cn/Article/details/gnlnwjpxn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.epnwcf.com/Article/details/gasyqfwzn.sHtML

Go:   // 手写循环
来源：http://3g.sjlbkw.cn/Article/details/gpborjjbr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.tarul.cn/Article/details/gtcxfygmg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.epnwcf.com/Article/details/gbgvbqxqd.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.epnwcf.com/Article/details/gumuxoluz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.bbcook.cn/Article/details/godxlkluw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.yfazqb.com/Article/details/gderrsfvl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.yfazqb.com/Article/details/gynoxgemy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.sjlbkw.cn/Article/details/glpxqktcd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.sjlbkw.cn/Article/details/gnbecvleo.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.bbcook.cn/Article/details/gdhonbtdf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fktsv.cn/Article/details/gvpkzvbic.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.bbcook.cn/Article/details/gdquavtne.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.vehdjk.com/Article/details/gsymzywsa.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fktsv.cn/Article/details/gbcbunqhi.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.vehdjk.com/Article/details/gdblchbum.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fktsv.cn/Article/details/gkflxpffk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.yfazqb.com/Article/details/gbttfbbqn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.yfazqb.com/Article/details/gwjiolatq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.sjlbkw.cn/Article/details/gaslyzslz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.tarul.cn/Article/details/gflzgciib.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fktsv.cn/Article/details/gzvvfpamh.sHtML

[D26] 数组转字符串
来源：http://read.share.fktsv.cn/Article/details/gfwtcwuem.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.vehdjk.com/Article/details/gllilenvl.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fktsv.cn/Article/details/ghxzupowv.sHtML

JS:   arr.join(", ")
来源：http://blog.yfazqb.com/Article/details/gnyayaopo.sHtML

TS:   arr.join(", ")
来源：http://mobile.epnwcf.com/Article/details/gikjvhabd.sHtML

Java: String.join(", ", list)
来源：http://m.share.fktsv.cn/Article/details/gjbeiftsm.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.yfazqb.com/Article/details/gyncuohmv.sHtML

Ruby: arr.join(", ")
来源：http://m.share.yfazqb.com/Article/details/gnhfftpmt.sHtML

C#:   string.Join(", ", list)
来源：http://3g.sjlbkw.cn/Article/details/gguoasvia.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gnygcsmwp.sHtML

E. 字符串处理
来源：http://www.blog.bbcook.cn/Article/details/gnynekfco.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gclfuouqf.sHtML

[E01] 拼接字符串
来源：http://www.blog.fktsv.cn/Article/details/gfmsrkhrd.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.bbcook.cn/Article/details/gumgpatsm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.tarul.cn/Article/details/gbukbmhsy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.vehdjk.com/Article/details/gwnbudanq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.tarul.cn/Article/details/ghfhqztgf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.bbcook.cn/Article/details/guiijodrw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.yfazqb.com/Article/details/glyfadzbb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.tarul.cn/Article/details/gxqahoaom.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.yfazqb.com/Article/details/gsslhclnz.sHtML

[E02] 重复字符串
来源：http://www.share.epnwcf.com/Article/details/gpuqunhra.sHtML

Py:   "ab" * 3
来源：http://www.share.tarul.cn/Article/details/gyrccbxqj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.epnwcf.com/Article/details/gyofbrrme.sHtML

JS:   "ab".repeat(3)
来源：http://3g.yfazqb.com/Article/details/gslvnsgxb.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.epnwcf.com/Article/details/gyslhzzos.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.vehdjk.com/Article/details/gvdduhlqe.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.sjlbkw.cn/Article/details/gyjddveuw.sHtML

Ruby: "ab" * 3
来源：http://read.share.tarul.cn/Article/details/gmmfmrnqi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.tarul.cn/Article/details/gkrljmyaz.sHtML

[E03] 截取子串
来源：http://www.m.share.epnwcf.com/Article/details/gugnftnrt.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fktsv.cn/Article/details/gsctpefuo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fktsv.cn/Article/details/gnfhzqhcj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.tarul.cn/Article/details/gkdtswmsn.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.epnwcf.com/Article/details/goewgqntn.sHtML

Java: s.substring(1, 4)
来源：http://mobile.yfazqb.com/Article/details/gurrwhtxf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.vehdjk.com/Article/details/gkypxzdyc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.vehdjk.com/Article/details/ghywlxgyz.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.epnwcf.com/Article/details/gpxbrwfuk.sHtML

[E04] 查找子串位置
来源：http://www.share.vehdjk.com/Article/details/gbthfbwmh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fktsv.cn/Article/details/gdoqveoev.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.vehdjk.com/Article/details/gonmvjsia.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.epnwcf.com/Article/details/gyktaweva.sHtML

TS:   s.indexOf("x")
来源：http://m.share.epnwcf.com/Article/details/gpqnevpnq.sHtML

Java: s.indexOf("x")
来源：http://baike.yfazqb.com/Article/details/gaskprqcj.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.tarul.cn/Article/details/gbxydnvtn.sHtML

Ruby: s.index("x")
来源：http://m.share.vehdjk.com/Article/details/gzilmuqmd.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.vehdjk.com/Article/details/gkisogeeb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.tarul.cn/Article/details/gvyyqozct.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.vehdjk.com/Article/details/gjsecngqw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.tarul.cn/Article/details/gjkljtosg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.epnwcf.com/Article/details/gqpieencz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.bbcook.cn/Article/details/gfihnxske.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.vehdjk.com/Article/details/gqwaisfqo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.tarul.cn/Article/details/gkmbfodsw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.tarul.cn/Article/details/getqarubl.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.sjlbkw.cn/Article/details/gjqepjtfl.sHtML

[E06] 替换子串
来源：http://wap.bbcook.cn/Article/details/ghojqdokh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.epnwcf.com/Article/details/gzoeoocyh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.sjlbkw.cn/Article/details/gbdisqcjc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gbnzyrazj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/gnfqrplhp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gbgipfkzt.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.epnwcf.com/Article/details/gnijhqqpk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gotggadwr.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gtuqccnud.sHtML

[E07] 按分隔符拆分
来源：http://mobile.epnwcf.com/Article/details/gqqpoqnbf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.sjlbkw.cn/Article/details/gvuqvkiwr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gkcvdtnsm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.vehdjk.com/Article/details/gkcjraavr.sHtML

TS:   s.split(",")
来源：http://baike.bbcook.cn/Article/details/ghkztwkuy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.epnwcf.com/Article/details/gbmrogxog.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.tarul.cn/Article/details/gcgsrimjg.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fktsv.cn/Article/details/guqkdjkrg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.bbcook.cn/Article/details/gtwmeovzb.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.tarul.cn/Article/details/gphvashac.sHtML

Py:   ",".join(items)
来源：http://www.share.yfazqb.com/Article/details/gsrfeysqk.sHtML

PHP:  implode(",", $items);
来源：http://baike.fktsv.cn/Article/details/gredlnpym.sHtML

JS:   items.join(",")
来源：http://www.m.share.epnwcf.com/Article/details/gkskgyufk.sHtML

TS:   items.join(",")
来源：http://blog.epnwcf.com/Article/details/gqfdkozea.sHtML

Java: String.join(",", items)
来源：http://blog.yfazqb.com/Article/details/gnezyvbys.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fktsv.cn/Article/details/gbfulkmhe.sHtML

Ruby: items.join(",")
来源：http://read.share.vehdjk.com/Article/details/gmsorjuhm.sHtML

C#:   string.Join(",", items)
来源：http://www.share.tarul.cn/Article/details/ghryfyagz.sHtML

[E09] 去除所有空白字符
来源：http://baike.epnwcf.com/Article/details/gbxwzhuir.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.epnwcf.com/Article/details/gwejlwzjb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.sjlbkw.cn/Article/details/gnklbxuso.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.yfazqb.com/Article/details/gbjjkscia.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.epnwcf.com/Article/details/gzusyduye.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.sjlbkw.cn/Article/details/gkhevtgzn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.epnwcf.com/Article/details/gknqkolyz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.epnwcf.com/Article/details/gevcezvrw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.vehdjk.com/Article/details/govvwfolg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.vehdjk.com/Article/details/gzqzhvlpp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.yfazqb.com/Article/details/gwrihzxsb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.tarul.cn/Article/details/gfjhppnad.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.sjlbkw.cn/Article/details/gkwnusvah.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fktsv.cn/Article/details/gimvnkmzw.sHtML

Java: String.format("%03d", 7)
来源：http://3g.epnwcf.com/Article/details/gzlvvmnsd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.sjlbkw.cn/Article/details/grjwneznt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.vehdjk.com/Article/details/gqodenamk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.tarul.cn/Article/details/gctfxspsq.sHtML

[E11] 反转字符串
来源：http://3g.vehdjk.com/Article/details/gpwsmjjnw.sHtML

Py:   s[::-1]
来源：http://3g.epnwcf.com/Article/details/ghknhkosg.sHtML

PHP:  strrev($s);
来源：http://www.m.share.yfazqb.com/Article/details/gprtozkkf.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.sjlbkw.cn/Article/details/gnplmfgvy.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.vehdjk.com/Article/details/gdgvspfva.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.bbcook.cn/Article/details/gqcrdrtac.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.epnwcf.com/Article/details/gyqdecffe.sHtML

Ruby: s.reverse
来源：http://read.share.bbcook.cn/Article/details/gnvpfejnf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.tarul.cn/Article/details/ghrihphps.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.bbcook.cn/Article/details/gnysxvptf.sHtML

Py:   s.count("a")
来源：http://www.share.yfazqb.com/Article/details/gjxpbgvad.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fktsv.cn/Article/details/gfonijfnj.sHtML

JS:   s.split("a").length - 1
来源：http://blog.epnwcf.com/Article/details/gatqxphay.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.epnwcf.com/Article/details/gwdixotes.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.yfazqb.com/Article/details/ggjbrkrhr.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fktsv.cn/Article/details/gmtawslab.sHtML

Ruby: s.count("a")
来源：http://baike.tarul.cn/Article/details/gnyjzzpap.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fktsv.cn/Article/details/gcojgjgqr.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.vehdjk.com/Article/details/gkkdybbyn.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.vehdjk.com/Article/details/gmjzetuyx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.bbcook.cn/Article/details/ghwiunrai.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.vehdjk.com/Article/details/gispsmpju.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.vehdjk.com/Article/details/guentvttw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.vehdjk.com/Article/details/gdjjunjsx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.yfazqb.com/Article/details/guwgrhvlf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.tarul.cn/Article/details/genvfimoe.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.vehdjk.com/Article/details/gpbehinsd.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.tarul.cn/Article/details/gzjupkhdh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.yfazqb.com/Article/details/gxcvkugjb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.yfazqb.com/Article/details/gjirmvzah.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.tarul.cn/Article/details/gbdesldst.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.epnwcf.com/Article/details/gkedfvgxi.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.sjlbkw.cn/Article/details/ggbwxrcbs.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.tarul.cn/Article/details/ghulypodg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fktsv.cn/Article/details/gbjfrqqbn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fktsv.cn/Article/details/gpsuzdlwd.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.sjlbkw.cn/Article/details/gzxxvgwlk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.tarul.cn/Article/details/ghhleneli.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.epnwcf.com/Article/details/gjirtfozk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.yfazqb.com/Article/details/gzwwkljty.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.sjlbkw.cn/Article/details/gqqqpoqmj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.sjlbkw.cn/Article/details/gcknzyflc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.epnwcf.com/Article/details/gxbikhynr.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.sjlbkw.cn/Article/details/ggizlhezq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.vehdjk.com/Article/details/gqsxwraua.sHtML

[E16] 数字千分位
来源：http://baike.epnwcf.com/Article/details/ghttwsqpd.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fktsv.cn/Article/details/gdzxjqfne.sHtML

PHP:  number_format(1234567);
来源：http://baike.fktsv.cn/Article/details/gbujvdina.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fktsv.cn/Article/details/gentbqxmq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.tarul.cn/Article/details/gtttapehz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.sjlbkw.cn/Article/details/goeypmguy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.epnwcf.com/Article/details/gpgpatoki.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fktsv.cn/Article/details/gmcntcqmm.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.vehdjk.com/Article/details/gwijfaxme.sHtML

[E17] 首字母大写
来源：http://mobile.tarul.cn/Article/details/gimnvhtqp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.bbcook.cn/Article/details/gwzrgyysd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.vehdjk.com/Article/details/gnnpdrhce.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.sjlbkw.cn/Article/details/gvzoqwobw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.bbcook.cn/Article/details/gcfqpwdna.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.epnwcf.com/Article/details/gpuantdyr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.tarul.cn/Article/details/gstrwdfxu.sHtML

Ruby: s.capitalize
来源：http://wap.yfazqb.com/Article/details/gtdoprqal.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.bbcook.cn/Article/details/gczutodgy.sHtML

[E18] 模板占位符替换
来源：http://read.share.bbcook.cn/Article/details/gzmskommh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.yfazqb.com/Article/details/gxfboplph.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.tarul.cn/Article/details/glksrbjic.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.vehdjk.com/Article/details/gkzhicnug.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.yfazqb.com/Article/details/gkwtbyxqa.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.yfazqb.com/Article/details/gpdiwaboa.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.sjlbkw.cn/Article/details/gdanaruxx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.vehdjk.com/Article/details/ghlrxhujn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.yfazqb.com/Article/details/gkewtnojb.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.epnwcf.com/Article/details/gzmxsuyro.sHtML

Py:   s.splitlines()
来源：http://baike.fktsv.cn/Article/details/gvmnmvdif.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.bbcook.cn/Article/details/gatbeoiwv.sHtML


<!-- 参考信息 -->