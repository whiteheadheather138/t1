代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.epnwcf.com/Article/details/gpsfjdlqh.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.tarul.cn/Article/details/gjasketxd.sHtML

[D17] 最大值与最小值
来源：http://wap.fktsv.cn/Article/details/gmxqmtwbv.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.epnwcf.com/Article/details/gvyojesud.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.epnwcf.com/Article/details/gpwednfmd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fktsv.cn/Article/details/grbnfjfgj.sHtML

TS:   Math.max(...arr);
来源：http://3g.epnwcf.com/Article/details/gydanmlqm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvdtshomx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.yfazqb.com/Article/details/giblbmohm.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fktsv.cn/Article/details/gfileghqs.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.sjlbkw.cn/Article/details/gjgxkauja.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fktsv.cn/Article/details/gqaaqvipw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.bbcook.cn/Article/details/gugxaqqus.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fktsv.cn/Article/details/gmbqsfcak.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.bbcook.cn/Article/details/ggcejqega.sHtML

TS:   nested.flat();
来源：http://wap.sjlbkw.cn/Article/details/ggdxuvuhd.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gxlawfsdh.sHtML

Go:   // 手写双层循环
来源：http://www.blog.tarul.cn/Article/details/glyrnnrlr.sHtML

Ruby: nested.flatten
来源：http://3g.vehdjk.com/Article/details/gvznlvaib.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.yfazqb.com/Article/details/gvustghgm.sHtML

[D19] 按字段分组
来源：http://wap.epnwcf.com/Article/details/gbywbosry.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.sjlbkw.cn/Article/details/gzvbluwga.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.tarul.cn/Article/details/gabraobcl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.bbcook.cn/Article/details/gonzecyyg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.sjlbkw.cn/Article/details/gueqwnory.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.tarul.cn/Article/details/gsvkcvneh.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fktsv.cn/Article/details/gmjqhbazi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fktsv.cn/Article/details/glvfqwlzx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.sjlbkw.cn/Article/details/gvwxsfsli.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.tarul.cn/Article/details/glhfoombp.sHtML

Py:   Counter(arr)
来源：http://read.share.fktsv.cn/Article/details/gecjknozw.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.epnwcf.com/Article/details/gkxdsrslx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.bbcook.cn/Article/details/grhgoztpj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.sjlbkw.cn/Article/details/ghbjrxqvp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.vehdjk.com/Article/details/gmfebpvzr.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fktsv.cn/Article/details/gecjbtkvc.sHtML

Ruby: arr.tally
来源：http://blog.tarul.cn/Article/details/gaaksgdfk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.tarul.cn/Article/details/gmuhequpu.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.vehdjk.com/Article/details/gualwgcnd.sHtML

Py:   x in arr
来源：http://www.blog.fktsv.cn/Article/details/gfzzgcrei.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.yfazqb.com/Article/details/gsgjciwpa.sHtML

JS:   arr.includes(x)
来源：http://mobile.tarul.cn/Article/details/gcuzftnan.sHtML

TS:   arr.includes(x)
来源：http://3g.vehdjk.com/Article/details/gftbixxzr.sHtML

Java: list.contains(x)
来源：http://3g.bbcook.cn/Article/details/gzhlrqvji.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.fktsv.cn/Article/details/gbcmnybli.sHtML

Ruby: arr.include?(x)
来源：http://m.share.yfazqb.com/Article/details/ggaiizpxz.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.yfazqb.com/Article/details/gooaktqse.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fktsv.cn/Article/details/gumkysqmk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.epnwcf.com/Article/details/gabckiaue.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.tarul.cn/Article/details/gdaqwpfmi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.vehdjk.com/Article/details/glfzcstld.sHtML

TS:   [...arr];
来源：http://mobile.epnwcf.com/Article/details/ghqtcdjds.sHtML

Java: new ArrayList<>(list);
来源：http://blog.bbcook.cn/Article/details/ggvermqfh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.yfazqb.com/Article/details/gztzvkgfs.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.sjlbkw.cn/Article/details/gzdkujvkh.sHtML

C#:   new List<int>(list);
来源：http://wap.fktsv.cn/Article/details/gnafsdcmo.sHtML

[D23] reduce 累积计算
来源：http://www.blog.yfazqb.com/Article/details/gwcizjvvb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.epnwcf.com/Article/details/giclxkstu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.tarul.cn/Article/details/ggioazddg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.tarul.cn/Article/details/gcqzcatmj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.tarul.cn/Article/details/gruzpjrrw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.yfazqb.com/Article/details/glnynlwol.sHtML

Go:   // 手写循环
来源：http://read.share.yfazqb.com/Article/details/gefkcklrs.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.epnwcf.com/Article/details/gaievortu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fktsv.cn/Article/details/gudhqhtje.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.tarul.cn/Article/details/golboiphn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fktsv.cn/Article/details/gkiuihfwd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.yfazqb.com/Article/details/gikrjtouy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.sjlbkw.cn/Article/details/gpgscyuhb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.yfazqb.com/Article/details/guqrwxmwf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.epnwcf.com/Article/details/gguubxeox.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.epnwcf.com/Article/details/gbdfqugzi.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.epnwcf.com/Article/details/gddyqzitl.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.sjlbkw.cn/Article/details/gipqwunyi.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.sjlbkw.cn/Article/details/gurojevbq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.sjlbkw.cn/Article/details/gqumjxjuk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.vehdjk.com/Article/details/ghjecvvcu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.vehdjk.com/Article/details/gavtgcvvv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.tarul.cn/Article/details/gyslazfmu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.epnwcf.com/Article/details/ggwmsfccd.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.epnwcf.com/Article/details/gdnnnskug.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.tarul.cn/Article/details/gsdrqxeoj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.vehdjk.com/Article/details/gzwrhbddh.sHtML

[D26] 数组转字符串
来源：http://m.share.sjlbkw.cn/Article/details/gqorvronn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.vehdjk.com/Article/details/ghlanqtup.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.tarul.cn/Article/details/garxxmluh.sHtML

JS:   arr.join(", ")
来源：http://blog.yfazqb.com/Article/details/gfprffkvt.sHtML

TS:   arr.join(", ")
来源：http://baike.yfazqb.com/Article/details/gcxycthlo.sHtML

Java: String.join(", ", list)
来源：http://www.blog.tarul.cn/Article/details/gxzalchzl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fktsv.cn/Article/details/gymulxohu.sHtML

Ruby: arr.join(", ")
来源：http://mobile.epnwcf.com/Article/details/gydkikqzv.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fktsv.cn/Article/details/gasdxjsep.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gqsveocaj.sHtML

E. 字符串处理
来源：http://m.share.vehdjk.com/Article/details/gbbnmhzfp.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gbrobmpjc.sHtML

[E01] 拼接字符串
来源：http://baike.sjlbkw.cn/Article/details/gtgcatbdj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.bbcook.cn/Article/details/gjomyknhb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fktsv.cn/Article/details/gakylqaot.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fktsv.cn/Article/details/gitwzqzei.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.bbcook.cn/Article/details/gtjpftdmz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.vehdjk.com/Article/details/gsewgttpn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.epnwcf.com/Article/details/gsfxijyzx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.vehdjk.com/Article/details/gqnytwmbn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gsvcicdzz.sHtML

[E02] 重复字符串
来源：http://3g.yfazqb.com/Article/details/gwthorsob.sHtML

Py:   "ab" * 3
来源：http://www.m.share.epnwcf.com/Article/details/gugrfjgwg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.sjlbkw.cn/Article/details/gdeomgbxk.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.bbcook.cn/Article/details/gyqjcldnw.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gppdbafbx.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.bbcook.cn/Article/details/galmfsyfl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.epnwcf.com/Article/details/gejrkksmg.sHtML

Ruby: "ab" * 3
来源：http://read.share.epnwcf.com/Article/details/gxjojvjur.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.yfazqb.com/Article/details/gzmwmdfpc.sHtML

[E03] 截取子串
来源：http://www.m.share.epnwcf.com/Article/details/gywzmerbb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.tarul.cn/Article/details/gbopkgsqo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.epnwcf.com/Article/details/gyfzoazcy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.epnwcf.com/Article/details/gtwfpvpdp.sHtML

TS:   s.slice(1, 4)
来源：http://baike.bbcook.cn/Article/details/gzknwprno.sHtML

Java: s.substring(1, 4)
来源：http://blog.tarul.cn/Article/details/gzbazzaxv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.epnwcf.com/Article/details/gpvlieynt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.epnwcf.com/Article/details/gxumzobcj.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.vehdjk.com/Article/details/gazxwhfma.sHtML

[E04] 查找子串位置
来源：http://www.share.bbcook.cn/Article/details/gqbpqyjgv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.epnwcf.com/Article/details/glbqkcyfh.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.fktsv.cn/Article/details/gdyrtnkrf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.yfazqb.com/Article/details/gsehstinl.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fktsv.cn/Article/details/gagbpyuco.sHtML

Java: s.indexOf("x")
来源：http://www.blog.tarul.cn/Article/details/gpngpmwlj.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.bbcook.cn/Article/details/gskkkamvs.sHtML

Ruby: s.index("x")
来源：http://www.blog.epnwcf.com/Article/details/gzjoztqra.sHtML

C#:   s.IndexOf("x")
来源：http://blog.vehdjk.com/Article/details/gmuifnqeu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.vehdjk.com/Article/details/gsepaombb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.yfazqb.com/Article/details/ggsdquwap.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.vehdjk.com/Article/details/gdrseyxqo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.vehdjk.com/Article/details/gpbkbhwwk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fktsv.cn/Article/details/gwwoegpce.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.tarul.cn/Article/details/gkikippei.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.bbcook.cn/Article/details/gxdzsorze.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.yfazqb.com/Article/details/gpiqesdcg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.vehdjk.com/Article/details/gctizrbus.sHtML

[E06] 替换子串
来源：http://wap.fktsv.cn/Article/details/gcrlveicw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.yfazqb.com/Article/details/ghatydonn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.bbcook.cn/Article/details/ghcifrhue.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.epnwcf.com/Article/details/gcegtotmv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.bbcook.cn/Article/details/gfalgwvrn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gbgaufhji.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.epnwcf.com/Article/details/gqethixev.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/grgibikvf.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.bbcook.cn/Article/details/gvofsbrvd.sHtML

[E07] 按分隔符拆分
来源：http://blog.bbcook.cn/Article/details/gnsonbwwh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.sjlbkw.cn/Article/details/gqsyvyylw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.tarul.cn/Article/details/grsugkgpr.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fktsv.cn/Article/details/gpaoummna.sHtML

TS:   s.split(",")
来源：http://blog.sjlbkw.cn/Article/details/gwkssibib.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.yfazqb.com/Article/details/gxgzgwoqb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.sjlbkw.cn/Article/details/gyqpjmvjv.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.tarul.cn/Article/details/gytcrsmwk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.tarul.cn/Article/details/gzogfuday.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fktsv.cn/Article/details/guvhdtviq.sHtML

Py:   ",".join(items)
来源：http://m.share.yfazqb.com/Article/details/gxpzvkjxf.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.sjlbkw.cn/Article/details/gzrlnttyu.sHtML

JS:   items.join(",")
来源：http://mobile.bbcook.cn/Article/details/guqmblgvp.sHtML

TS:   items.join(",")
来源：http://m.share.yfazqb.com/Article/details/gokzylisu.sHtML

Java: String.join(",", items)
来源：http://blog.tarul.cn/Article/details/geqpxubcx.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.vehdjk.com/Article/details/gknhieizt.sHtML

Ruby: items.join(",")
来源：http://wap.yfazqb.com/Article/details/gxtglyppd.sHtML

C#:   string.Join(",", items)
来源：http://www.share.tarul.cn/Article/details/gzbuqjbqx.sHtML

[E09] 去除所有空白字符
来源：http://wap.vehdjk.com/Article/details/gwhpajhvw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.tarul.cn/Article/details/gglcqraht.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gjhpkfoxu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.sjlbkw.cn/Article/details/gjjmqbrgu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.vehdjk.com/Article/details/ganvhgram.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.epnwcf.com/Article/details/ggvvlcets.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fktsv.cn/Article/details/gicbzjstj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.sjlbkw.cn/Article/details/gxmpaobiq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.bbcook.cn/Article/details/gaydxrqaq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.sjlbkw.cn/Article/details/gvwxuigzp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.tarul.cn/Article/details/glzwuvvjx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.vehdjk.com/Article/details/gynbduurq.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.vehdjk.com/Article/details/gvcdsrzfm.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.tarul.cn/Article/details/gosiodgum.sHtML

Java: String.format("%03d", 7)
来源：http://blog.tarul.cn/Article/details/gjeuuyucc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.epnwcf.com/Article/details/gstrjnlis.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.epnwcf.com/Article/details/gingcctdi.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.yfazqb.com/Article/details/gkdhnurln.sHtML

[E11] 反转字符串
来源：http://wap.epnwcf.com/Article/details/garjizveh.sHtML

Py:   s[::-1]
来源：http://blog.fktsv.cn/Article/details/gxpaiiaae.sHtML

PHP:  strrev($s);
来源：http://m.share.fktsv.cn/Article/details/gsokvwfmo.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.vehdjk.com/Article/details/gjddixgly.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.yfazqb.com/Article/details/glaxbjdox.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.sjlbkw.cn/Article/details/gqqkkdtil.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.vehdjk.com/Article/details/govrjlrud.sHtML

Ruby: s.reverse
来源：http://www.share.yfazqb.com/Article/details/gyjjlsgcf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fktsv.cn/Article/details/gyvdqdswz.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fktsv.cn/Article/details/giwzosfeu.sHtML

Py:   s.count("a")
来源：http://blog.epnwcf.com/Article/details/gffodlvtk.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.tarul.cn/Article/details/gxgqgvzxy.sHtML

JS:   s.split("a").length - 1
来源：http://wap.vehdjk.com/Article/details/gbadzkxaz.sHtML

TS:   s.split("a").length - 1
来源：http://wap.epnwcf.com/Article/details/gexcztngf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.yfazqb.com/Article/details/glmwhwqzo.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.bbcook.cn/Article/details/gvmlffzms.sHtML

Ruby: s.count("a")
来源：http://www.m.share.vehdjk.com/Article/details/gmxmbgvcg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.vehdjk.com/Article/details/gsycafjgy.sHtML

[E13] 逐字符遍历
来源：http://wap.tarul.cn/Article/details/gagtuxteb.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.tarul.cn/Article/details/gaofpjpkn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.bbcook.cn/Article/details/gctdibjqn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.sjlbkw.cn/Article/details/gfuvkhmoo.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.sjlbkw.cn/Article/details/gdrhrhilc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.vehdjk.com/Article/details/guhjucowc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.vehdjk.com/Article/details/gvxojdnoj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.yfazqb.com/Article/details/gfblfrlbx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.bbcook.cn/Article/details/gmvqqcojb.sHtML

[E14] URL 编码与 Base64
来源：http://3g.yfazqb.com/Article/details/ggtyfnnzg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.vehdjk.com/Article/details/gmvsdemea.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.sjlbkw.cn/Article/details/golwstgom.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fktsv.cn/Article/details/gsskgjhzu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.yfazqb.com/Article/details/gypikvphn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.sjlbkw.cn/Article/details/gepvqpugi.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.epnwcf.com/Article/details/gudrvllcs.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.yfazqb.com/Article/details/gaevzuomm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.epnwcf.com/Article/details/gkyvndhau.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.tarul.cn/Article/details/gszakndbp.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.yfazqb.com/Article/details/grzndyoky.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fktsv.cn/Article/details/gbvhqaeoi.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.bbcook.cn/Article/details/gaitaxdci.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fktsv.cn/Article/details/gqurbzoij.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fktsv.cn/Article/details/gyeadghmk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.sjlbkw.cn/Article/details/ghbcsxddj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fktsv.cn/Article/details/giegqbgrl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.bbcook.cn/Article/details/gkiadgmym.sHtML

[E16] 数字千分位
来源：http://baike.epnwcf.com/Article/details/gjgnwwpjh.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fktsv.cn/Article/details/gzwpepkrs.sHtML

PHP:  number_format(1234567);
来源：http://read.share.tarul.cn/Article/details/gtpmfeitd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.bbcook.cn/Article/details/gpbijpmaq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.yfazqb.com/Article/details/gpahbiqwj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.yfazqb.com/Article/details/gwfmihrvv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.tarul.cn/Article/details/guovdmvkh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.vehdjk.com/Article/details/ghkgswhml.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.sjlbkw.cn/Article/details/gvcdekfyf.sHtML

[E17] 首字母大写
来源：http://3g.fktsv.cn/Article/details/goounvemm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.epnwcf.com/Article/details/ggrnjvzrs.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.sjlbkw.cn/Article/details/gacqthswp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.epnwcf.com/Article/details/guzixmyns.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.yfazqb.com/Article/details/gscsuurwi.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.vehdjk.com/Article/details/gkdfgetrd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.sjlbkw.cn/Article/details/gxjkvgaud.sHtML

Ruby: s.capitalize
来源：http://3g.epnwcf.com/Article/details/gsgypqshq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fktsv.cn/Article/details/gdjqvkxac.sHtML

[E18] 模板占位符替换
来源：http://baike.yfazqb.com/Article/details/gpninnsss.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.vehdjk.com/Article/details/gityqrnjv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.yfazqb.com/Article/details/gixrtyhne.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.sjlbkw.cn/Article/details/goeztqxzq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.epnwcf.com/Article/details/gzdrzctpu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.sjlbkw.cn/Article/details/gpjglwdjf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.yfazqb.com/Article/details/glzjqxguc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.yfazqb.com/Article/details/ginhpvxmv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fktsv.cn/Article/details/gcqqntrea.sHtML

[E19] 多行文本按行拆分
来源：http://wap.sjlbkw.cn/Article/details/gaajjuchi.sHtML

Py:   s.splitlines()
来源：http://wap.sjlbkw.cn/Article/details/ghvympndh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fktsv.cn/Article/details/gcvszheqs.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.yfazqb.com/Article/details/gbkbmpjbh.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.vehdjk.com/Article/details/gluaikpmb.sHtML

Java: s.lines().toList()
来源：http://www.share.vehdjk.com/Article/details/giclyouxw.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.tarul.cn/Article/details/gmvmmwovh.sHtML

Ruby: s.lines
来源：http://mobile.vehdjk.com/Article/details/gboejpixr.sHtML

C#:   s.Split('\n')
来源：http://www.blog.epnwcf.com/Article/details/ggzoykpce.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.vehdjk.com/Article/details/gmvecjwpc.sHtML

Py:   if not s:
来源：http://m.share.bbcook.cn/Article/details/gkwjpjrnz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.sjlbkw.cn/Article/details/gsgurqodl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.epnwcf.com/Article/details/gyjqtrhxb.sHtML

TS:   if (s === "") {}
来源：http://mobile.epnwcf.com/Article/details/gaqfroknc.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.yfazqb.com/Article/details/gtxcrblxe.sHtML

Go:   if s == "" {}
来源：http://www.blog.tarul.cn/Article/details/ghrzfbrhh.sHtML

Ruby: if s.empty?
来源：http://read.share.vehdjk.com/Article/details/getwpkajg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.bbcook.cn/Article/details/gskipuybc.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.epnwcf.com/Article/details/glrzywnyy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.epnwcf.com/Article/details/gkgiaxica.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.bbcook.cn/Article/details/grlehsceo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.vehdjk.com/Article/details/gluniehbr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.sjlbkw.cn/Article/details/gykrywgwg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.bbcook.cn/Article/details/gtesopvlu.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.epnwcf.com/Article/details/grdvnpzoi.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gkbkwggsp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.yfazqb.com/Article/details/gbrzmvnar.sHtML

[E22] 字节长度与字符长度
来源：http://blog.yfazqb.com/Article/details/goiuiwlxa.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.epnwcf.com/Article/details/gyrafjcir.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.vehdjk.com/Article/details/gtrevzdya.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.vehdjk.com/Article/details/gozwrrvky.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.epnwcf.com/Article/details/ghptwpthf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.bbcook.cn/Article/details/gxchirssl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fktsv.cn/Article/details/grirnkygw.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.bbcook.cn/Article/details/gkywcrwkc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.epnwcf.com/Article/details/gmtcyvbvb.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gojlgjwvv.sHtML

F. 文件与目录
来源：http://wap.bbcook.cn/Article/details/gkikmaygr.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gtujasofd.sHtML

[F01] 读取整个文件
来源：http://blog.vehdjk.com/Article/details/gfmdmrgvb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.yfazqb.com/Article/details/gdlmrximu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.vehdjk.com/Article/details/getosmilq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.vehdjk.com/Article/details/ggbqfwfew.sHtML


<!-- 参考信息 -->