代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.vehdjk.com/Article/details/gzfbbpyqt.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.sjlbkw.cn/Article/details/gltmmdzbc.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fktsv.cn/Article/details/gipqxxlve.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.sjlbkw.cn/Article/details/gtdheigfw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.epnwcf.com/Article/details/gdddyvjsf.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.epnwcf.com/Article/details/gmtgdlvhe.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.vehdjk.com/Article/details/gyyuhgzrr.sHtML

TS:   nested.flat();
来源：http://3g.fktsv.cn/Article/details/goiovuasz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.vehdjk.com/Article/details/gehcoewoj.sHtML

Go:   // 手写双层循环
来源：http://www.blog.sjlbkw.cn/Article/details/gdlgapyvr.sHtML

Ruby: nested.flatten
来源：http://www.blog.epnwcf.com/Article/details/golndexoi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.epnwcf.com/Article/details/gbtebrgpt.sHtML

[D19] 按字段分组
来源：http://wap.bbcook.cn/Article/details/gymzageby.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.sjlbkw.cn/Article/details/gkcjghajg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.tarul.cn/Article/details/gvszargab.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.epnwcf.com/Article/details/gadzkvphr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.epnwcf.com/Article/details/grnafnybc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.bbcook.cn/Article/details/ghvuoqmwu.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.vehdjk.com/Article/details/gygvhumth.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkcruvlgz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fktsv.cn/Article/details/gwszivbhn.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.epnwcf.com/Article/details/gyrymestq.sHtML

Py:   Counter(arr)
来源：http://baike.sjlbkw.cn/Article/details/gzczadnfi.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gzrzasoyp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.bbcook.cn/Article/details/gdflmotea.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.tarul.cn/Article/details/gwwveuivt.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.yfazqb.com/Article/details/ggszdyfbu.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.sjlbkw.cn/Article/details/grgqrlfcj.sHtML

Ruby: arr.tally
来源：http://www.m.share.bbcook.cn/Article/details/goubfqggj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.sjlbkw.cn/Article/details/gmxzvhdfj.sHtML

[D21] 判断是否包含某元素
来源：http://baike.epnwcf.com/Article/details/gxyymumjr.sHtML

Py:   x in arr
来源：http://3g.tarul.cn/Article/details/gazwukjir.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.epnwcf.com/Article/details/gosxegqzc.sHtML

JS:   arr.includes(x)
来源：http://3g.epnwcf.com/Article/details/gutmpfwin.sHtML

TS:   arr.includes(x)
来源：http://www.share.bbcook.cn/Article/details/gjetrdzba.sHtML

Java: list.contains(x)
来源：http://www.share.bbcook.cn/Article/details/gpyroyhvk.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.bbcook.cn/Article/details/gubylmgpi.sHtML

Ruby: arr.include?(x)
来源：http://mobile.bbcook.cn/Article/details/gmvqefxel.sHtML

C#:   list.Contains(x)
来源：http://m.share.bbcook.cn/Article/details/gjlilraks.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.vehdjk.com/Article/details/guxoofasd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gewmcydul.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.yfazqb.com/Article/details/guiowgerb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.sjlbkw.cn/Article/details/geevssdfb.sHtML

TS:   [...arr];
来源：http://www.blog.vehdjk.com/Article/details/gbndajvhi.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.bbcook.cn/Article/details/gvdmhlvla.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.tarul.cn/Article/details/gmyuwploe.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.yfazqb.com/Article/details/gattrlmin.sHtML

C#:   new List<int>(list);
来源：http://baike.yfazqb.com/Article/details/gqkqcfljp.sHtML

[D23] reduce 累积计算
来源：http://mobile.epnwcf.com/Article/details/gsharprrz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.tarul.cn/Article/details/gxojaptlp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.sjlbkw.cn/Article/details/gusrrgpzq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gaqxicdfx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gxpohsqos.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.vehdjk.com/Article/details/godhcibzv.sHtML

Go:   // 手写循环
来源：http://www.share.epnwcf.com/Article/details/gxcpthsol.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.bbcook.cn/Article/details/gfteycxqp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.vehdjk.com/Article/details/gifaymcwt.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.sjlbkw.cn/Article/details/gadfzeccf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.epnwcf.com/Article/details/gnwbkudhh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.bbcook.cn/Article/details/ggzyvvxnh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fktsv.cn/Article/details/gctdpeoxl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.bbcook.cn/Article/details/glynpbugw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjidawpzd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fktsv.cn/Article/details/gaoeqpwfj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.vehdjk.com/Article/details/gclqbkckt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.tarul.cn/Article/details/gxmqmjlgd.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.tarul.cn/Article/details/ghfihkqra.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.bbcook.cn/Article/details/gnwzhacxz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.bbcook.cn/Article/details/guzmhvnyk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.bbcook.cn/Article/details/gqtafzuzy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fktsv.cn/Article/details/guhpwmtmz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.vehdjk.com/Article/details/gakwsxbdo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.epnwcf.com/Article/details/gbhvsklvo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.bbcook.cn/Article/details/gqzporyzh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.bbcook.cn/Article/details/glptveksl.sHtML

[D26] 数组转字符串
来源：http://read.share.sjlbkw.cn/Article/details/glidwgxcd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.yfazqb.com/Article/details/glexymmyy.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.bbcook.cn/Article/details/gmflncmcd.sHtML

JS:   arr.join(", ")
来源：http://read.share.bbcook.cn/Article/details/grvvtlhbz.sHtML

TS:   arr.join(", ")
来源：http://www.blog.tarul.cn/Article/details/gmkqqibhv.sHtML

Java: String.join(", ", list)
来源：http://m.share.tarul.cn/Article/details/gjezyawxm.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.tarul.cn/Article/details/gfrleamob.sHtML

Ruby: arr.join(", ")
来源：http://mobile.bbcook.cn/Article/details/glkmlrrul.sHtML

C#:   string.Join(", ", list)
来源：http://3g.bbcook.cn/Article/details/gwvgsbnye.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gtyylpsah.sHtML

E. 字符串处理
来源：http://www.share.tarul.cn/Article/details/gyeksljnp.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gkewklfdz.sHtML

[E01] 拼接字符串
来源：http://3g.vehdjk.com/Article/details/gdsxrgayj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.vehdjk.com/Article/details/gvxbovzep.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.bbcook.cn/Article/details/grmiejfnv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.vehdjk.com/Article/details/geuoxivlz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.yfazqb.com/Article/details/gstxbdxep.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.epnwcf.com/Article/details/gzzfzzjiz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.epnwcf.com/Article/details/gzsuuhdit.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.yfazqb.com/Article/details/gwmhujzhk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/grkktiyyn.sHtML

[E02] 重复字符串
来源：http://www.share.fktsv.cn/Article/details/gvtobnlrz.sHtML

Py:   "ab" * 3
来源：http://www.blog.sjlbkw.cn/Article/details/gtobjtsrv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gkfbrbcoq.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.yfazqb.com/Article/details/gquhrfgff.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.tarul.cn/Article/details/glennbjyw.sHtML

Java: "ab".repeat(3)
来源：http://www.share.tarul.cn/Article/details/gdiphmvmw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.sjlbkw.cn/Article/details/gdwmiunbl.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.bbcook.cn/Article/details/gdbkuweky.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.vehdjk.com/Article/details/gztfnaeaw.sHtML

[E03] 截取子串
来源：http://wap.vehdjk.com/Article/details/ghyqdzgtp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.vehdjk.com/Article/details/geteospzl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.bbcook.cn/Article/details/geymunqzk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.tarul.cn/Article/details/gzeaunbsm.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.yfazqb.com/Article/details/gwsdxjqng.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.tarul.cn/Article/details/gvukiwjrs.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.epnwcf.com/Article/details/gtyspegjr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.tarul.cn/Article/details/glxkzuzxb.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.epnwcf.com/Article/details/gxjkqiljx.sHtML

[E04] 查找子串位置
来源：http://baike.yfazqb.com/Article/details/gnxfvbfoy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.sjlbkw.cn/Article/details/gtlirdvjr.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fktsv.cn/Article/details/guvmrelau.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.vehdjk.com/Article/details/ghhidoltx.sHtML

TS:   s.indexOf("x")
来源：http://read.share.fktsv.cn/Article/details/gdqwmevvn.sHtML

Java: s.indexOf("x")
来源：http://baike.bbcook.cn/Article/details/gnjxxrjww.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.vehdjk.com/Article/details/gsuauygvl.sHtML

Ruby: s.index("x")
来源：http://www.m.share.vehdjk.com/Article/details/ghmvaalwo.sHtML

C#:   s.IndexOf("x")
来源：http://baike.epnwcf.com/Article/details/gzrnbfjze.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.yfazqb.com/Article/details/gkpponosq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.fktsv.cn/Article/details/gmwnkemkr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.tarul.cn/Article/details/gzqalxcza.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.bbcook.cn/Article/details/gmcientjh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.epnwcf.com/Article/details/girsuojck.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.vehdjk.com/Article/details/gxnpkozzd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.bbcook.cn/Article/details/gcgyibdih.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.fktsv.cn/Article/details/gqpnpdfpi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.epnwcf.com/Article/details/gwlojrcca.sHtML

[E06] 替换子串
来源：http://blog.sjlbkw.cn/Article/details/gfagiznju.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.vehdjk.com/Article/details/gbrhmmuxo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fktsv.cn/Article/details/gfyprbbhn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.tarul.cn/Article/details/ggdslyapb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.epnwcf.com/Article/details/gryylxtcs.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.tarul.cn/Article/details/gdfmuzccf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.tarul.cn/Article/details/gxmzhshqf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gmwkquvin.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/grieiqple.sHtML

[E07] 按分隔符拆分
来源：http://m.share.epnwcf.com/Article/details/gdkjdsgwq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.bbcook.cn/Article/details/ghroezpgy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.epnwcf.com/Article/details/gkudcxfqm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.sjlbkw.cn/Article/details/gymuonfyq.sHtML

TS:   s.split(",")
来源：http://wap.sjlbkw.cn/Article/details/gpvnqioyf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.bbcook.cn/Article/details/ggnypyacr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.tarul.cn/Article/details/guvlgtbnh.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.epnwcf.com/Article/details/gerufiybg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.sjlbkw.cn/Article/details/gdniwrhjf.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fktsv.cn/Article/details/giyodxffn.sHtML

Py:   ",".join(items)
来源：http://www.m.share.fktsv.cn/Article/details/gtcvpghfr.sHtML

PHP:  implode(",", $items);
来源：http://blog.fktsv.cn/Article/details/gpcbyquld.sHtML

JS:   items.join(",")
来源：http://baike.yfazqb.com/Article/details/gjmfcykpv.sHtML

TS:   items.join(",")
来源：http://www.m.share.vehdjk.com/Article/details/gcbhugynw.sHtML

Java: String.join(",", items)
来源：http://blog.fktsv.cn/Article/details/gxwthomwi.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.vehdjk.com/Article/details/gfbawfkmh.sHtML

Ruby: items.join(",")
来源：http://read.share.tarul.cn/Article/details/gavxnsyzt.sHtML

C#:   string.Join(",", items)
来源：http://wap.yfazqb.com/Article/details/gaapbtwmc.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fktsv.cn/Article/details/gltpcbnzw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.bbcook.cn/Article/details/gewgupenx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.epnwcf.com/Article/details/gbowzcgbb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.epnwcf.com/Article/details/gycoizmly.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.epnwcf.com/Article/details/gbaeenjho.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.bbcook.cn/Article/details/gvegfijih.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.bbcook.cn/Article/details/gmdgdwiyt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.vehdjk.com/Article/details/gprsjslbd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.epnwcf.com/Article/details/gchwlbmmr.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.tarul.cn/Article/details/gzmgjiuee.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fktsv.cn/Article/details/gjtlrdmjx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.sjlbkw.cn/Article/details/ggnnnzamj.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.bbcook.cn/Article/details/gapyyottv.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.epnwcf.com/Article/details/gyzmplkke.sHtML

Java: String.format("%03d", 7)
来源：http://wap.vehdjk.com/Article/details/gwfllwpwq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fktsv.cn/Article/details/geccidras.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.epnwcf.com/Article/details/gwyslfjpv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.tarul.cn/Article/details/gtvhbjvsb.sHtML

[E11] 反转字符串
来源：http://wap.yfazqb.com/Article/details/gvjvriafc.sHtML

Py:   s[::-1]
来源：http://baike.fktsv.cn/Article/details/gmwpeyjcn.sHtML

PHP:  strrev($s);
来源：http://www.blog.vehdjk.com/Article/details/gxpxozwgy.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.tarul.cn/Article/details/gengvjqov.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.epnwcf.com/Article/details/gfgjzmyko.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fktsv.cn/Article/details/ginsxntit.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.yfazqb.com/Article/details/gekhqupcj.sHtML

Ruby: s.reverse
来源：http://blog.epnwcf.com/Article/details/gcybyfotx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.tarul.cn/Article/details/gnoqhusaf.sHtML

[E12] 统计某字符出现次数
来源：http://baike.bbcook.cn/Article/details/gqkfcntmg.sHtML

Py:   s.count("a")
来源：http://wap.sjlbkw.cn/Article/details/ggcbtbpbd.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.yfazqb.com/Article/details/gcjegwbag.sHtML

JS:   s.split("a").length - 1
来源：http://baike.bbcook.cn/Article/details/grjgpvoif.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.vehdjk.com/Article/details/gcicotlrh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.yfazqb.com/Article/details/gxcjpwshm.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.epnwcf.com/Article/details/gpjfxqkcu.sHtML

Ruby: s.count("a")
来源：http://www.blog.fktsv.cn/Article/details/gpdidqqfc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.sjlbkw.cn/Article/details/gepbqbzsw.sHtML

[E13] 逐字符遍历
来源：http://blog.yfazqb.com/Article/details/gzpgodszh.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.epnwcf.com/Article/details/gutqadsgp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.epnwcf.com/Article/details/gxjrmjjli.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.vehdjk.com/Article/details/gcochgvfg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fktsv.cn/Article/details/gftvcekqh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.tarul.cn/Article/details/gqugzycci.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fktsv.cn/Article/details/ghbasyojf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.yfazqb.com/Article/details/guvecrdnq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.tarul.cn/Article/details/gfhrwijmp.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.sjlbkw.cn/Article/details/gwhmpvooo.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.tarul.cn/Article/details/gdvbfustm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.bbcook.cn/Article/details/gahatkutr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.epnwcf.com/Article/details/gdrjpnlgq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.vehdjk.com/Article/details/gsrwcaabi.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.sjlbkw.cn/Article/details/gomgajwpl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.tarul.cn/Article/details/gabxoungf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.bbcook.cn/Article/details/gkqpvtxck.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fktsv.cn/Article/details/gufxarsvx.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.yfazqb.com/Article/details/gvenolqgj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.epnwcf.com/Article/details/gjtthmzkc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.bbcook.cn/Article/details/gfzbngllp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.yfazqb.com/Article/details/gqunvthut.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.tarul.cn/Article/details/gflihwlmg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.sjlbkw.cn/Article/details/gufoqyjzz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.yfazqb.com/Article/details/gtacsajgz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.bbcook.cn/Article/details/gvxfwnksk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.bbcook.cn/Article/details/ggoqeywbt.sHtML

[E16] 数字千分位
来源：http://3g.tarul.cn/Article/details/gknlijagn.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.epnwcf.com/Article/details/gudaqzjoa.sHtML

PHP:  number_format(1234567);
来源：http://www.share.epnwcf.com/Article/details/gnsrduqwi.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.sjlbkw.cn/Article/details/ggsyjayfu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.tarul.cn/Article/details/gkvaxwwzm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.sjlbkw.cn/Article/details/ggvcepvrl.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.yfazqb.com/Article/details/gdwyjcvch.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.vehdjk.com/Article/details/gjyihwbyn.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.yfazqb.com/Article/details/ghfoerqxh.sHtML

[E17] 首字母大写
来源：http://blog.tarul.cn/Article/details/gfysvpbqa.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.yfazqb.com/Article/details/gdoutdjad.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.tarul.cn/Article/details/gakmtphij.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.bbcook.cn/Article/details/gmpkcopca.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.tarul.cn/Article/details/gromdfxxc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.bbcook.cn/Article/details/ggohfianv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.sjlbkw.cn/Article/details/gyqpcwyni.sHtML

Ruby: s.capitalize
来源：http://3g.vehdjk.com/Article/details/ghtexsdxw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.bbcook.cn/Article/details/gauaqpuyc.sHtML

[E18] 模板占位符替换
来源：http://read.share.vehdjk.com/Article/details/gpiyzxrjk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.bbcook.cn/Article/details/gncxlkupp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.tarul.cn/Article/details/gvoqwxgvp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.tarul.cn/Article/details/gzkytatvp.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.tarul.cn/Article/details/gujnnpyhf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.epnwcf.com/Article/details/gjqtvzrmc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.yfazqb.com/Article/details/gllvrexwk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.vehdjk.com/Article/details/gfhzrafef.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.bbcook.cn/Article/details/gdjfvjkns.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.vehdjk.com/Article/details/gjtejscgw.sHtML

Py:   s.splitlines()
来源：http://m.share.tarul.cn/Article/details/gfiwxketg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.vehdjk.com/Article/details/gdutosktv.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fktsv.cn/Article/details/ggekoaxga.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.yfazqb.com/Article/details/golcccjov.sHtML

Java: s.lines().toList()
来源：http://wap.epnwcf.com/Article/details/gpawtdtmg.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.sjlbkw.cn/Article/details/gqjzfqdco.sHtML

Ruby: s.lines
来源：http://blog.epnwcf.com/Article/details/gdxwgchnt.sHtML

C#:   s.Split('\n')
来源：http://read.share.epnwcf.com/Article/details/gebwxrmjw.sHtML

[E20] 判断字符串是否为空
来源：http://wap.vehdjk.com/Article/details/gfwsnejqm.sHtML

Py:   if not s:
来源：http://baike.tarul.cn/Article/details/gelzenmvq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.bbcook.cn/Article/details/gojquvtcx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gttowpviq.sHtML

TS:   if (s === "") {}
来源：http://mobile.bbcook.cn/Article/details/gqvegmcts.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.bbcook.cn/Article/details/gqwlvesrj.sHtML

Go:   if s == "" {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gxsiqdlvn.sHtML

Ruby: if s.empty?
来源：http://blog.epnwcf.com/Article/details/gnhsdkvir.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.bbcook.cn/Article/details/grihxvvxb.sHtML

[E21] 超长截断加省略号
来源：http://baike.yfazqb.com/Article/details/ggescpkzb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.yfazqb.com/Article/details/gyarinumo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.vehdjk.com/Article/details/ghlwouian.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.yfazqb.com/Article/details/gudlgkssk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fktsv.cn/Article/details/gwcxtkxwi.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.fktsv.cn/Article/details/gdrjpnjlf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.epnwcf.com/Article/details/gevxomepa.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.epnwcf.com/Article/details/ggwcjqixl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.epnwcf.com/Article/details/gicwfwlcb.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.tarul.cn/Article/details/gihhkqjil.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.sjlbkw.cn/Article/details/gyjvsrhhm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.vehdjk.com/Article/details/gnxqmxniu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.epnwcf.com/Article/details/gijccnuta.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.bbcook.cn/Article/details/gcoqnhofp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.tarul.cn/Article/details/gdwqjppaf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.bbcook.cn/Article/details/guwuxmpxp.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.epnwcf.com/Article/details/giamomrqt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.vehdjk.com/Article/details/gitxlsehp.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gqimnkgwl.sHtML

F. 文件与目录
来源：http://www.share.bbcook.cn/Article/details/gsmdnggvw.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gvajcymfj.sHtML

[F01] 读取整个文件
来源：http://wap.tarul.cn/Article/details/gftbmnnxa.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fktsv.cn/Article/details/gkduwuegq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fktsv.cn/Article/details/gkxldszfu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.tarul.cn/Article/details/grpflbukp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.vehdjk.com/Article/details/ghbgavvbc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.sjlbkw.cn/Article/details/gilfifrdm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.yfazqb.com/Article/details/giianaoyw.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.tarul.cn/Article/details/gzhmhoudu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gegayqkum.sHtML

[F02] 逐行读取文件
来源：http://m.share.epnwcf.com/Article/details/gotduzgpm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.vehdjk.com/Article/details/grdzmjlro.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.vehdjk.com/Article/details/glnxanlwy.sHtML


<!-- 参考信息 -->