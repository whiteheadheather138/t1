代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.sjlbkw.cn/Article/details/ggykjscnd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.sjlbkw.cn/Article/details/gebeexwtf.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.vehdjk.com/Article/details/gpmismtxp.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.yfazqb.com/Article/details/glivuqwan.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.yfazqb.com/Article/details/gamrqwarl.sHtML

Go:   // 手写循环
来源：http://baike.fktsv.cn/Article/details/gpwtcgrau.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fktsv.cn/Article/details/gkasqznic.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.sjlbkw.cn/Article/details/gdbhbrtay.sHtML

[D15] 去重
来源：http://read.share.bbcook.cn/Article/details/gppzztjqp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.sjlbkw.cn/Article/details/gegbhinir.sHtML

PHP:  array_unique($arr);
来源：http://mobile.vehdjk.com/Article/details/grihtgroy.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.yfazqb.com/Article/details/gnaojzqzd.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fktsv.cn/Article/details/gdhkafbkn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.vehdjk.com/Article/details/grcltcjmu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fktsv.cn/Article/details/ggctucuxr.sHtML

Ruby: arr.uniq
来源：http://www.blog.fktsv.cn/Article/details/gifmxjkno.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.bbcook.cn/Article/details/gksggtyvn.sHtML

[D16] 求和与平均值
来源：http://read.share.epnwcf.com/Article/details/glkfjfcnt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.bbcook.cn/Article/details/gukzoypbb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.yfazqb.com/Article/details/gdjuijvkz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.tarul.cn/Article/details/grkkuzaux.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.yfazqb.com/Article/details/gywojaxdp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.vehdjk.com/Article/details/gljonnxcm.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.sjlbkw.cn/Article/details/gnagmyquj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.sjlbkw.cn/Article/details/grdwwvmxs.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.vehdjk.com/Article/details/gelnudeqs.sHtML

[D17] 最大值与最小值
来源：http://baike.bbcook.cn/Article/details/gkkysnjtw.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.epnwcf.com/Article/details/gepsdxhgb.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fktsv.cn/Article/details/gzaubdosu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.sjlbkw.cn/Article/details/gzvzmfwum.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.bbcook.cn/Article/details/gojvdffcc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.epnwcf.com/Article/details/gibetiwkq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.tarul.cn/Article/details/gcmskehbu.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.sjlbkw.cn/Article/details/glhdovpwb.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.bbcook.cn/Article/details/gwzrtuukr.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fktsv.cn/Article/details/gytcxkbjm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.tarul.cn/Article/details/gttlsgezu.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.sjlbkw.cn/Article/details/grjrwkfbx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.tarul.cn/Article/details/gssfqzqlf.sHtML

TS:   nested.flat();
来源：http://www.m.share.sjlbkw.cn/Article/details/giapcpmmp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.tarul.cn/Article/details/giyhvvynm.sHtML

Go:   // 手写双层循环
来源：http://3g.epnwcf.com/Article/details/gpfbbtbsh.sHtML

Ruby: nested.flatten
来源：http://www.blog.sjlbkw.cn/Article/details/gpodvrywz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.yfazqb.com/Article/details/giprypixm.sHtML

[D19] 按字段分组
来源：http://m.share.fktsv.cn/Article/details/gjtsjfqtd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.bbcook.cn/Article/details/gnpvibpxa.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.vehdjk.com/Article/details/gqbbcqhmw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fktsv.cn/Article/details/glljvcnsb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.yfazqb.com/Article/details/getizodql.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.epnwcf.com/Article/details/gaayesgec.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.tarul.cn/Article/details/gbchdlaxl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fktsv.cn/Article/details/gozxygvvk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.yfazqb.com/Article/details/gixxyirxj.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.sjlbkw.cn/Article/details/gohinzxxt.sHtML

Py:   Counter(arr)
来源：http://m.share.yfazqb.com/Article/details/gllcyvzav.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.vehdjk.com/Article/details/ggksrchcz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.epnwcf.com/Article/details/ggvlssqvo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.sjlbkw.cn/Article/details/gwzdsuzfd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.vehdjk.com/Article/details/gkfphsexa.sHtML

Go:   // 手写 map[T]int
来源：http://wap.yfazqb.com/Article/details/gxhcqfwix.sHtML

Ruby: arr.tally
来源：http://www.blog.sjlbkw.cn/Article/details/gnmhlqvyw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.vehdjk.com/Article/details/gbsaunomz.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.yfazqb.com/Article/details/gyivqllbv.sHtML

Py:   x in arr
来源：http://www.share.yfazqb.com/Article/details/ggoqutano.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.tarul.cn/Article/details/guywjsxmo.sHtML

JS:   arr.includes(x)
来源：http://m.share.sjlbkw.cn/Article/details/ghryfinga.sHtML

TS:   arr.includes(x)
来源：http://blog.sjlbkw.cn/Article/details/gettcjhlp.sHtML

Java: list.contains(x)
来源：http://mobile.epnwcf.com/Article/details/gsnjlgydq.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.tarul.cn/Article/details/gghnhrkel.sHtML

Ruby: arr.include?(x)
来源：http://3g.sjlbkw.cn/Article/details/gsifbyrrt.sHtML

C#:   list.Contains(x)
来源：http://blog.sjlbkw.cn/Article/details/gimnviuda.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.sjlbkw.cn/Article/details/glleirhrt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fktsv.cn/Article/details/gmmwntiud.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.bbcook.cn/Article/details/gwwgwhgsp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.vehdjk.com/Article/details/gtjyhnhqh.sHtML

TS:   [...arr];
来源：http://3g.bbcook.cn/Article/details/gazwbhurl.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fktsv.cn/Article/details/gssknqfru.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fktsv.cn/Article/details/gonmahfou.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.bbcook.cn/Article/details/gvmqrdxxt.sHtML

C#:   new List<int>(list);
来源：http://m.share.fktsv.cn/Article/details/gdwiqiqsy.sHtML

[D23] reduce 累积计算
来源：http://3g.epnwcf.com/Article/details/ghgiqyhzq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.vehdjk.com/Article/details/gghlicfai.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.yfazqb.com/Article/details/gmcsfeafh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fktsv.cn/Article/details/gzgvmdtpk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gdzqorqpa.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.epnwcf.com/Article/details/gnjfqihra.sHtML

Go:   // 手写循环
来源：http://blog.bbcook.cn/Article/details/gcqdxdmwa.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.epnwcf.com/Article/details/gkukmclqu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.tarul.cn/Article/details/grwqzytpd.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fktsv.cn/Article/details/ggusuwufp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.sjlbkw.cn/Article/details/gfhyqflre.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.sjlbkw.cn/Article/details/gzsiiejfh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.vehdjk.com/Article/details/gklgtaraa.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.epnwcf.com/Article/details/gxjxaotqr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.tarul.cn/Article/details/gnrowazyv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.epnwcf.com/Article/details/gaydgomru.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.sjlbkw.cn/Article/details/gcskisetx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.bbcook.cn/Article/details/gsadujtfu.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.yfazqb.com/Article/details/gwriosuta.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.yfazqb.com/Article/details/gadwztaqx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.sjlbkw.cn/Article/details/gvzwzhald.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.sjlbkw.cn/Article/details/gtchvffwo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.sjlbkw.cn/Article/details/gjnnnhdyg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.epnwcf.com/Article/details/gkvtneunr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.epnwcf.com/Article/details/gjtjuwcrx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fktsv.cn/Article/details/ghbhjbsdz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.bbcook.cn/Article/details/ggkgwrzhw.sHtML

[D26] 数组转字符串
来源：http://baike.sjlbkw.cn/Article/details/gnnpilfql.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.vehdjk.com/Article/details/gsrxbjqgv.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.yfazqb.com/Article/details/ggngrbnom.sHtML

JS:   arr.join(", ")
来源：http://3g.yfazqb.com/Article/details/gybygwgxh.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.tarul.cn/Article/details/gncxpafdb.sHtML

Java: String.join(", ", list)
来源：http://mobile.tarul.cn/Article/details/gacrnrsqv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.bbcook.cn/Article/details/gxbxvzzzg.sHtML

Ruby: arr.join(", ")
来源：http://m.share.epnwcf.com/Article/details/ghobpqksn.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.epnwcf.com/Article/details/gcndpthgv.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gcrrspivf.sHtML

E. 字符串处理
来源：http://baike.fktsv.cn/Article/details/gjsmaeygd.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gpevezwnf.sHtML

[E01] 拼接字符串
来源：http://baike.sjlbkw.cn/Article/details/gksrwepdt.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.epnwcf.com/Article/details/gacznxyea.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.bbcook.cn/Article/details/gnxhazjqj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.tarul.cn/Article/details/glxprrqxy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fktsv.cn/Article/details/gcjydrqrj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.yfazqb.com/Article/details/gphphvvzz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.bbcook.cn/Article/details/gxcdazbfv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.vehdjk.com/Article/details/gcbpfaeiy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.bbcook.cn/Article/details/gtbzuymkj.sHtML

[E02] 重复字符串
来源：http://mobile.bbcook.cn/Article/details/gmkwagjwo.sHtML

Py:   "ab" * 3
来源：http://blog.vehdjk.com/Article/details/gptsthabf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.yfazqb.com/Article/details/ggidvravs.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.tarul.cn/Article/details/gisjewqch.sHtML

TS:   "ab".repeat(3)
来源：http://wap.epnwcf.com/Article/details/guobbvyhh.sHtML

Java: "ab".repeat(3)
来源：http://baike.tarul.cn/Article/details/grkomihms.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.vehdjk.com/Article/details/glewmsgfp.sHtML

Ruby: "ab" * 3
来源：http://wap.epnwcf.com/Article/details/gkvppeyts.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.sjlbkw.cn/Article/details/gaxmzgccj.sHtML

[E03] 截取子串
来源：http://www.m.share.bbcook.cn/Article/details/gfnezhtkk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.vehdjk.com/Article/details/gtylyoebq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.vehdjk.com/Article/details/gowggovzs.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.epnwcf.com/Article/details/gxriplqwe.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fktsv.cn/Article/details/gqnhtybox.sHtML

Java: s.substring(1, 4)
来源：http://read.share.yfazqb.com/Article/details/gactrjnta.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.epnwcf.com/Article/details/gqafchcaz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fktsv.cn/Article/details/gmynsxuiy.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.tarul.cn/Article/details/gqcxrtfrw.sHtML

[E04] 查找子串位置
来源：http://m.share.vehdjk.com/Article/details/gflzdzblq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.fktsv.cn/Article/details/guroesspw.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.yfazqb.com/Article/details/gjkcsslvo.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.epnwcf.com/Article/details/gnnqydwwh.sHtML

TS:   s.indexOf("x")
来源：http://3g.yfazqb.com/Article/details/gtaqlczco.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.bbcook.cn/Article/details/gtinmkamt.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.yfazqb.com/Article/details/gjiqegxfu.sHtML

Ruby: s.index("x")
来源：http://www.m.share.vehdjk.com/Article/details/gkzjeymhh.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.bbcook.cn/Article/details/gxcnbscen.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fktsv.cn/Article/details/gzpqjzzao.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.vehdjk.com/Article/details/gjcvyjpai.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.yfazqb.com/Article/details/gkzdlynkm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fktsv.cn/Article/details/gddpxrqin.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.bbcook.cn/Article/details/ggdplfzfk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.sjlbkw.cn/Article/details/gkyyixflb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.tarul.cn/Article/details/guyuxgelj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fktsv.cn/Article/details/gggjowjib.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.tarul.cn/Article/details/giudaaxie.sHtML

[E06] 替换子串
来源：http://read.share.bbcook.cn/Article/details/gshoimogm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.epnwcf.com/Article/details/gmusxswqn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.tarul.cn/Article/details/guzosbiti.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.epnwcf.com/Article/details/gsjjnryby.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/grsaziqep.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.bbcook.cn/Article/details/gpibrjacy.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.epnwcf.com/Article/details/gllwaoejq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.tarul.cn/Article/details/gclemuyfy.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.tarul.cn/Article/details/gxrywxjmr.sHtML

[E07] 按分隔符拆分
来源：http://www.share.tarul.cn/Article/details/gvhoesxly.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.epnwcf.com/Article/details/ggionfrwh.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fktsv.cn/Article/details/gnelgxrsy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.vehdjk.com/Article/details/gqtnqxjhx.sHtML

TS:   s.split(",")
来源：http://baike.fktsv.cn/Article/details/gjliwwfkr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fktsv.cn/Article/details/gbrggbcrk.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.epnwcf.com/Article/details/gvvynalln.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.yfazqb.com/Article/details/guqftlqjp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fktsv.cn/Article/details/ghtvkkgbj.sHtML

[E08] 数组按分隔符合并
来源：http://blog.tarul.cn/Article/details/gwgyjdblk.sHtML

Py:   ",".join(items)
来源：http://baike.bbcook.cn/Article/details/gvfcdnbms.sHtML

PHP:  implode(",", $items);
来源：http://blog.tarul.cn/Article/details/glkkzvzal.sHtML

JS:   items.join(",")
来源：http://3g.yfazqb.com/Article/details/gmgyhtihj.sHtML

TS:   items.join(",")
来源：http://baike.yfazqb.com/Article/details/gwkkskaeu.sHtML

Java: String.join(",", items)
来源：http://m.share.fktsv.cn/Article/details/ggeutlarn.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.vehdjk.com/Article/details/gkjbgcuac.sHtML

Ruby: items.join(",")
来源：http://read.share.bbcook.cn/Article/details/gbzkfjwyq.sHtML

C#:   string.Join(",", items)
来源：http://m.share.yfazqb.com/Article/details/gidcyruax.sHtML

[E09] 去除所有空白字符
来源：http://3g.yfazqb.com/Article/details/gaxdmkvwb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.sjlbkw.cn/Article/details/grbmddlvg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.sjlbkw.cn/Article/details/gvtsrvbyf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.vehdjk.com/Article/details/gutfpwqgt.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.bbcook.cn/Article/details/goqdeusyi.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.yfazqb.com/Article/details/gmtvjorzf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.vehdjk.com/Article/details/gzhlgjoex.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.epnwcf.com/Article/details/gakzctagu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.tarul.cn/Article/details/gbbhasjdd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.yfazqb.com/Article/details/gjvvvjnfb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.bbcook.cn/Article/details/godpbzexm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.vehdjk.com/Article/details/gjjfnskef.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.tarul.cn/Article/details/gmozcfnlu.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.vehdjk.com/Article/details/gyspowzoe.sHtML

Java: String.format("%03d", 7)
来源：http://wap.sjlbkw.cn/Article/details/gznlhrxme.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.yfazqb.com/Article/details/gjkepljnu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.sjlbkw.cn/Article/details/gdahrwtxc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.epnwcf.com/Article/details/gafqqdqfv.sHtML

[E11] 反转字符串
来源：http://3g.tarul.cn/Article/details/gzhpdnqaz.sHtML

Py:   s[::-1]
来源：http://www.share.sjlbkw.cn/Article/details/gqceagzjd.sHtML

PHP:  strrev($s);
来源：http://baike.fktsv.cn/Article/details/gfgvhvyrc.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fktsv.cn/Article/details/gvywwnodb.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.yfazqb.com/Article/details/gkomdihhv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.bbcook.cn/Article/details/gdgvdjntq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.tarul.cn/Article/details/gihpoyeux.sHtML

Ruby: s.reverse
来源：http://read.share.tarul.cn/Article/details/gkrxtpokg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fktsv.cn/Article/details/gbqotlmgn.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.epnwcf.com/Article/details/gxpzbeukk.sHtML

Py:   s.count("a")
来源：http://baike.tarul.cn/Article/details/gbuxucqyo.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.yfazqb.com/Article/details/ghyhzndnh.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.tarul.cn/Article/details/gehqoysgg.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.vehdjk.com/Article/details/gcvnuxoua.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fktsv.cn/Article/details/gxemakyns.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fktsv.cn/Article/details/gynoupzrd.sHtML

Ruby: s.count("a")
来源：http://mobile.sjlbkw.cn/Article/details/gndhdchae.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.tarul.cn/Article/details/glevupnhx.sHtML

[E13] 逐字符遍历
来源：http://mobile.fktsv.cn/Article/details/glfbfnvpf.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.vehdjk.com/Article/details/gqzsaxmlo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.sjlbkw.cn/Article/details/gcezhjrgn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.sjlbkw.cn/Article/details/gllbwqihg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.sjlbkw.cn/Article/details/gkldylryb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.epnwcf.com/Article/details/gjjzegcid.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.sjlbkw.cn/Article/details/ghfolrrgf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.sjlbkw.cn/Article/details/ggrzrjugz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.bbcook.cn/Article/details/gfnlweefv.sHtML

[E14] URL 编码与 Base64
来源：http://3g.epnwcf.com/Article/details/gdoutnanl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.bbcook.cn/Article/details/gxuowoyfz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.tarul.cn/Article/details/gvcofulsv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fktsv.cn/Article/details/gbtiiyqjl.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghsvnqamy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.tarul.cn/Article/details/grirbntet.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.yfazqb.com/Article/details/grqnvjjmu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.bbcook.cn/Article/details/gvlpcocaa.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fktsv.cn/Article/details/gworkhcje.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.sjlbkw.cn/Article/details/gmrpdvknt.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fktsv.cn/Article/details/girvxjwfc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.bbcook.cn/Article/details/gwdgwqccc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.vehdjk.com/Article/details/gjaxndckh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.bbcook.cn/Article/details/gqtldhfvh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.sjlbkw.cn/Article/details/gujdieeff.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.vehdjk.com/Article/details/gzfkvtlqg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fktsv.cn/Article/details/gfutujdou.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fktsv.cn/Article/details/goefsemah.sHtML

[E16] 数字千分位
来源：http://blog.sjlbkw.cn/Article/details/gqiuddqfn.sHtML

Py:   f"{1234567:,}"
来源：http://baike.bbcook.cn/Article/details/ggoaabgkb.sHtML

PHP:  number_format(1234567);
来源：http://wap.fktsv.cn/Article/details/gnbimemar.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.yfazqb.com/Article/details/gdewnouea.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.tarul.cn/Article/details/gdhoytrgk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.bbcook.cn/Article/details/gffgrocfh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fktsv.cn/Article/details/gktnwbuzj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.tarul.cn/Article/details/gmziuilqw.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.epnwcf.com/Article/details/gpfxummyb.sHtML

[E17] 首字母大写
来源：http://www.m.share.bbcook.cn/Article/details/gnfmxxbrw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.yfazqb.com/Article/details/gojanzgry.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.vehdjk.com/Article/details/gjrpthqiy.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.vehdjk.com/Article/details/gfcxnvsby.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.bbcook.cn/Article/details/ghexyunzj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.sjlbkw.cn/Article/details/gjgqcgnyf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fktsv.cn/Article/details/geppvkcfq.sHtML

Ruby: s.capitalize
来源：http://www.blog.tarul.cn/Article/details/gpvupqfgt.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fktsv.cn/Article/details/gmxhfmrzz.sHtML

[E18] 模板占位符替换
来源：http://www.blog.vehdjk.com/Article/details/giestsicj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fktsv.cn/Article/details/ghnjmccir.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.tarul.cn/Article/details/gljpdlfqe.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.sjlbkw.cn/Article/details/goyunuwnw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.vehdjk.com/Article/details/gdydtibmv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.vehdjk.com/Article/details/gwssehwnr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.tarul.cn/Article/details/ggcyolxji.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.vehdjk.com/Article/details/gvovogjwv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.yfazqb.com/Article/details/gzeeswtxl.sHtML

[E19] 多行文本按行拆分
来源：http://baike.tarul.cn/Article/details/grqxsxfqe.sHtML

Py:   s.splitlines()
来源：http://www.blog.epnwcf.com/Article/details/gjujqxbgm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gzttlxvee.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.tarul.cn/Article/details/glgyyaknj.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.vehdjk.com/Article/details/gvpmfrvpy.sHtML

Java: s.lines().toList()
来源：http://www.share.fktsv.cn/Article/details/gdwavprqy.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.epnwcf.com/Article/details/gggkkiawj.sHtML

Ruby: s.lines
来源：http://m.share.yfazqb.com/Article/details/gewuulmkq.sHtML

C#:   s.Split('\n')
来源：http://mobile.bbcook.cn/Article/details/gkqpivrcy.sHtML

[E20] 判断字符串是否为空
来源：http://3g.vehdjk.com/Article/details/gyhgqphpc.sHtML

Py:   if not s:
来源：http://m.share.sjlbkw.cn/Article/details/gebffnnhy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.vehdjk.com/Article/details/gtdszvwcx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.yfazqb.com/Article/details/gnsmmmuqg.sHtML

TS:   if (s === "") {}
来源：http://baike.fktsv.cn/Article/details/grgjdnhhr.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.epnwcf.com/Article/details/gmbgbxznd.sHtML

Go:   if s == "" {}
来源：http://m.share.fktsv.cn/Article/details/gpnaqwljc.sHtML

Ruby: if s.empty?
来源：http://3g.epnwcf.com/Article/details/giztcptos.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.tarul.cn/Article/details/gmqmupufa.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.epnwcf.com/Article/details/glbqqtbxo.sHtML


<!-- 参考信息 -->