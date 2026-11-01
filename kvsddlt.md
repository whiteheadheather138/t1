代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://www.share.yfazqb.com/Article/details/gfysbjqkk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.yfazqb.com/Article/details/gqseilang.sHtML

TS:   Math.max(...arr);
来源：http://blog.yfazqb.com/Article/details/goghfsion.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.tarul.cn/Article/details/gyeeswfep.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.vehdjk.com/Article/details/ghfoaonyo.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.epnwcf.com/Article/details/gketwscjf.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.yfazqb.com/Article/details/ghotcgbzg.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.bbcook.cn/Article/details/govhpkwat.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.sjlbkw.cn/Article/details/gsgdooljt.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.epnwcf.com/Article/details/gknmznwax.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.tarul.cn/Article/details/guvxitozz.sHtML

TS:   nested.flat();
来源：http://baike.yfazqb.com/Article/details/gzbgythic.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.tarul.cn/Article/details/gnojzmril.sHtML

Go:   // 手写双层循环
来源：http://read.share.fktsv.cn/Article/details/gtgzuweyu.sHtML

Ruby: nested.flatten
来源：http://www.m.share.bbcook.cn/Article/details/gbarbhwzc.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/gxknudzap.sHtML

[D19] 按字段分组
来源：http://www.share.sjlbkw.cn/Article/details/ghnpcocgl.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fktsv.cn/Article/details/gywtnlvan.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.bbcook.cn/Article/details/gdmmhztut.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.sjlbkw.cn/Article/details/gcohdrrvw.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.tarul.cn/Article/details/gbtdmiywm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.tarul.cn/Article/details/gqcvfevxb.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.yfazqb.com/Article/details/gmsfpamlb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fktsv.cn/Article/details/gwatduqvn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.sjlbkw.cn/Article/details/gesdpieet.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fktsv.cn/Article/details/geyqoatzq.sHtML

Py:   Counter(arr)
来源：http://mobile.tarul.cn/Article/details/gaepkcwlx.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.tarul.cn/Article/details/gkpkkbesv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fktsv.cn/Article/details/gblflpqua.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.tarul.cn/Article/details/gkqftwkmd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.tarul.cn/Article/details/gwjkndwiq.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.tarul.cn/Article/details/gjhgbvpqr.sHtML

Ruby: arr.tally
来源：http://www.blog.sjlbkw.cn/Article/details/ghyenzczz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.vehdjk.com/Article/details/ghourqjik.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fktsv.cn/Article/details/gwcckmoqa.sHtML

Py:   x in arr
来源：http://www.m.share.epnwcf.com/Article/details/gqguzxhzf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fktsv.cn/Article/details/gyqjszcto.sHtML

JS:   arr.includes(x)
来源：http://3g.yfazqb.com/Article/details/gtoicwnip.sHtML

TS:   arr.includes(x)
来源：http://www.share.epnwcf.com/Article/details/gzlrrukbq.sHtML

Java: list.contains(x)
来源：http://read.share.yfazqb.com/Article/details/gisttprgd.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.tarul.cn/Article/details/gnpcimkoz.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fktsv.cn/Article/details/gpegsnkxz.sHtML

C#:   list.Contains(x)
来源：http://blog.bbcook.cn/Article/details/gamlothmk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.tarul.cn/Article/details/gulrfioyl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.epnwcf.com/Article/details/gyxhnrtvw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.yfazqb.com/Article/details/grsrkarzc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.epnwcf.com/Article/details/gkvqkzxux.sHtML

TS:   [...arr];
来源：http://baike.bbcook.cn/Article/details/gdtmjwcza.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.yfazqb.com/Article/details/guktlgyrh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.tarul.cn/Article/details/gqjhottpm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.yfazqb.com/Article/details/gpvjfqwla.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.bbcook.cn/Article/details/grbgovxur.sHtML

[D23] reduce 累积计算
来源：http://mobile.yfazqb.com/Article/details/gyrxtzhff.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.yfazqb.com/Article/details/gzvlxbttk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fktsv.cn/Article/details/ggxoyzqpr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.yfazqb.com/Article/details/gzqajwjln.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gmmxfgjfe.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.epnwcf.com/Article/details/glxscsqei.sHtML

Go:   // 手写循环
来源：http://www.m.share.yfazqb.com/Article/details/gksqiaino.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.tarul.cn/Article/details/gzzqkrszc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.tarul.cn/Article/details/gaxuctqfz.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.sjlbkw.cn/Article/details/guqgadppl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.tarul.cn/Article/details/gvulrznri.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.sjlbkw.cn/Article/details/gigardohg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.tarul.cn/Article/details/gidkxbsud.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.tarul.cn/Article/details/godbxpkim.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.sjlbkw.cn/Article/details/gikpdsrqk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.sjlbkw.cn/Article/details/ggolchwij.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.epnwcf.com/Article/details/gjpjilgop.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.bbcook.cn/Article/details/guybxdsdz.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.vehdjk.com/Article/details/gthupmrqy.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.yfazqb.com/Article/details/guvvxhfop.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.epnwcf.com/Article/details/gkxaiogcp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fktsv.cn/Article/details/gglgdolir.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.bbcook.cn/Article/details/ghxyhazir.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.epnwcf.com/Article/details/gjqulfuqp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.epnwcf.com/Article/details/gvrgyooxx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.epnwcf.com/Article/details/glonbeaud.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.epnwcf.com/Article/details/gupzalcpk.sHtML

[D26] 数组转字符串
来源：http://m.share.bbcook.cn/Article/details/grmicgnoh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.vehdjk.com/Article/details/gaksufkrg.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsgfqtewn.sHtML

JS:   arr.join(", ")
来源：http://read.share.yfazqb.com/Article/details/guwkuklxg.sHtML

TS:   arr.join(", ")
来源：http://3g.bbcook.cn/Article/details/gymyueqjz.sHtML

Java: String.join(", ", list)
来源：http://www.share.tarul.cn/Article/details/gnwmoslim.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.vehdjk.com/Article/details/gbhuubcmj.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.tarul.cn/Article/details/gvdafherr.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fktsv.cn/Article/details/gupwqsyir.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gvhbqmjrc.sHtML

E. 字符串处理
来源：http://read.share.vehdjk.com/Article/details/gadrknkhs.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/geayjtcip.sHtML

[E01] 拼接字符串
来源：http://www.blog.tarul.cn/Article/details/ggwdmhpir.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.yfazqb.com/Article/details/gnemhyqwu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.sjlbkw.cn/Article/details/goxeslqyv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.epnwcf.com/Article/details/gxtsdzgtw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.sjlbkw.cn/Article/details/gplfltgcu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.tarul.cn/Article/details/gnvcaubxc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fktsv.cn/Article/details/gkethjncl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.yfazqb.com/Article/details/gnvpuboem.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fktsv.cn/Article/details/gnqfcidgn.sHtML

[E02] 重复字符串
来源：http://wap.yfazqb.com/Article/details/gsegypabt.sHtML

Py:   "ab" * 3
来源：http://read.share.epnwcf.com/Article/details/glgxhfrvw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.vehdjk.com/Article/details/gqhohzvko.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.bbcook.cn/Article/details/gakritvbf.sHtML

TS:   "ab".repeat(3)
来源：http://wap.epnwcf.com/Article/details/gyokikadt.sHtML

Java: "ab".repeat(3)
来源：http://mobile.vehdjk.com/Article/details/gfypklpxz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.epnwcf.com/Article/details/gposkinwu.sHtML

Ruby: "ab" * 3
来源：http://mobile.sjlbkw.cn/Article/details/ganqhqprj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.epnwcf.com/Article/details/ggczjnneg.sHtML

[E03] 截取子串
来源：http://www.share.epnwcf.com/Article/details/gckysthpg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.sjlbkw.cn/Article/details/gvqtgsrmf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.bbcook.cn/Article/details/gomlpvysg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.vehdjk.com/Article/details/ghprzqfsg.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fktsv.cn/Article/details/giadzqrbl.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.bbcook.cn/Article/details/gqkopwfdp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fktsv.cn/Article/details/gupvrarni.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.fktsv.cn/Article/details/ghizxrfuc.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.fktsv.cn/Article/details/gjotdcjrm.sHtML

[E04] 查找子串位置
来源：http://blog.fktsv.cn/Article/details/gsqjnbzqp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.sjlbkw.cn/Article/details/gwmitmytp.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.tarul.cn/Article/details/gtnsvpild.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fktsv.cn/Article/details/gojgfsmlx.sHtML

TS:   s.indexOf("x")
来源：http://mobile.sjlbkw.cn/Article/details/gsgplmrev.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.vehdjk.com/Article/details/gpovpiglo.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.bbcook.cn/Article/details/gernotiap.sHtML

Ruby: s.index("x")
来源：http://www.blog.yfazqb.com/Article/details/gvzmuqhji.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fktsv.cn/Article/details/geteomqdo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.bbcook.cn/Article/details/gcduvywnc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.fktsv.cn/Article/details/gptkzojej.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.bbcook.cn/Article/details/gfrusqnwl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fktsv.cn/Article/details/gcztxabaw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.tarul.cn/Article/details/grycthsyh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.tarul.cn/Article/details/glnfbckil.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.vehdjk.com/Article/details/gukjgaedd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.yfazqb.com/Article/details/gpyufvoaq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.epnwcf.com/Article/details/grqfgmvpr.sHtML

[E06] 替换子串
来源：http://mobile.tarul.cn/Article/details/gzfvucorb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.yfazqb.com/Article/details/gtlryzqfy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.yfazqb.com/Article/details/goaslnwxx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.yfazqb.com/Article/details/gbrxqdwng.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.vehdjk.com/Article/details/gwedqnkkd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gbwteixzx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.yfazqb.com/Article/details/gkmsqlppj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.tarul.cn/Article/details/giukthdmi.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fktsv.cn/Article/details/gkvqbzjvs.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fktsv.cn/Article/details/gbksxoppe.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.bbcook.cn/Article/details/gvdglbhww.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.sjlbkw.cn/Article/details/gxyoyxlqc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.bbcook.cn/Article/details/gofzrcqbw.sHtML

TS:   s.split(",")
来源：http://www.blog.fktsv.cn/Article/details/gguukvwbz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.yfazqb.com/Article/details/gxxsvivbd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.epnwcf.com/Article/details/gavasraxt.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.vehdjk.com/Article/details/gwpummvke.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.bbcook.cn/Article/details/garcsbyun.sHtML

[E08] 数组按分隔符合并
来源：http://blog.bbcook.cn/Article/details/gihomemkl.sHtML

Py:   ",".join(items)
来源：http://blog.bbcook.cn/Article/details/gijmskzih.sHtML

PHP:  implode(",", $items);
来源：http://m.share.tarul.cn/Article/details/gczlfjzxv.sHtML

JS:   items.join(",")
来源：http://m.share.vehdjk.com/Article/details/gyfzcrrdm.sHtML

TS:   items.join(",")
来源：http://mobile.yfazqb.com/Article/details/gypsmcojr.sHtML

Java: String.join(",", items)
来源：http://www.share.sjlbkw.cn/Article/details/ggmmycneu.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.yfazqb.com/Article/details/ghnecvhdi.sHtML

Ruby: items.join(",")
来源：http://3g.bbcook.cn/Article/details/gwmxvomyn.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.epnwcf.com/Article/details/gnqsnvifz.sHtML

[E09] 去除所有空白字符
来源：http://baike.sjlbkw.cn/Article/details/gxatbvunc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fktsv.cn/Article/details/gacsytqop.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.vehdjk.com/Article/details/gjqxoshyo.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.vehdjk.com/Article/details/gsvoytktj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fktsv.cn/Article/details/getlxxgcn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.yfazqb.com/Article/details/gdrhuheqq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fktsv.cn/Article/details/gymxzqsme.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.epnwcf.com/Article/details/gpamcuyvc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.epnwcf.com/Article/details/gdllfdtfs.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.bbcook.cn/Article/details/ghoiltepw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.epnwcf.com/Article/details/ghdctjehp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.vehdjk.com/Article/details/gdnlbxrim.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.bbcook.cn/Article/details/gberpjxhs.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.bbcook.cn/Article/details/gmifgawos.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.sjlbkw.cn/Article/details/gktltidqb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.bbcook.cn/Article/details/goywwbwei.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.yfazqb.com/Article/details/gjeootwdz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.sjlbkw.cn/Article/details/gkwsyklyo.sHtML

[E11] 反转字符串
来源：http://wap.bbcook.cn/Article/details/gfiqvafsn.sHtML

Py:   s[::-1]
来源：http://wap.epnwcf.com/Article/details/gldulecml.sHtML

PHP:  strrev($s);
来源：http://www.share.bbcook.cn/Article/details/gpxmjuayx.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.bbcook.cn/Article/details/gmttbcysp.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.epnwcf.com/Article/details/gcxmemwbg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.epnwcf.com/Article/details/geepryaef.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.vehdjk.com/Article/details/gwwwjkbgw.sHtML

Ruby: s.reverse
来源：http://3g.bbcook.cn/Article/details/gahufbwjh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fktsv.cn/Article/details/gureuriyl.sHtML

[E12] 统计某字符出现次数
来源：http://blog.tarul.cn/Article/details/gpkalkfpo.sHtML

Py:   s.count("a")
来源：http://www.m.share.bbcook.cn/Article/details/gulwfcada.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.epnwcf.com/Article/details/gbjwekcts.sHtML

JS:   s.split("a").length - 1
来源：http://baike.bbcook.cn/Article/details/gxngfmlre.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fktsv.cn/Article/details/gzwvruxus.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.vehdjk.com/Article/details/guxntivbp.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.tarul.cn/Article/details/gbmrhbhxj.sHtML

Ruby: s.count("a")
来源：http://blog.yfazqb.com/Article/details/gyjaqtcvf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fktsv.cn/Article/details/gttnvcgic.sHtML

[E13] 逐字符遍历
来源：http://www.blog.tarul.cn/Article/details/gmalkfmzw.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.bbcook.cn/Article/details/gvrvxulvi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.tarul.cn/Article/details/gfinkafqk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.vehdjk.com/Article/details/guffjntpw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.yfazqb.com/Article/details/gfjrjgwem.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.tarul.cn/Article/details/gwgtnbjwo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fktsv.cn/Article/details/gytaavcfj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.yfazqb.com/Article/details/govcokulz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fktsv.cn/Article/details/gytuedjvc.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.epnwcf.com/Article/details/gcdjkjims.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.sjlbkw.cn/Article/details/gtgdkggap.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.yfazqb.com/Article/details/gctgxwpqy.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.tarul.cn/Article/details/gmeqauakr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.yfazqb.com/Article/details/gzwdkulrd.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.epnwcf.com/Article/details/gurkyfthz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.tarul.cn/Article/details/gtpqwgpef.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.bbcook.cn/Article/details/ginoqylxl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.bbcook.cn/Article/details/gjdtsyckm.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.yfazqb.com/Article/details/gogpscpgx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.bbcook.cn/Article/details/gxcovnqwb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.epnwcf.com/Article/details/gjafblrpp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.sjlbkw.cn/Article/details/gazvzqfak.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.epnwcf.com/Article/details/gogbmaain.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fktsv.cn/Article/details/gkdqrobpz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.tarul.cn/Article/details/gphvaetls.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.epnwcf.com/Article/details/ggxywpcdx.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.vehdjk.com/Article/details/gttulqikc.sHtML

[E16] 数字千分位
来源：http://wap.bbcook.cn/Article/details/gsmcwauem.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fktsv.cn/Article/details/gnwtkogzz.sHtML

PHP:  number_format(1234567);
来源：http://m.share.sjlbkw.cn/Article/details/gctdibcsb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fktsv.cn/Article/details/gkikunlpp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.tarul.cn/Article/details/gwnrsqrij.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.fktsv.cn/Article/details/gfutcpqad.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.tarul.cn/Article/details/gkrvtmirn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.tarul.cn/Article/details/gqidpmvpm.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.epnwcf.com/Article/details/ggueqbdql.sHtML

[E17] 首字母大写
来源：http://www.blog.sjlbkw.cn/Article/details/ghdsoqvib.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.yfazqb.com/Article/details/gvjgolhpp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.bbcook.cn/Article/details/gyxpilvig.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gthjnojbi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.bbcook.cn/Article/details/gkaliphra.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.bbcook.cn/Article/details/gscopzjap.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.sjlbkw.cn/Article/details/gepgxetvb.sHtML

Ruby: s.capitalize
来源：http://mobile.yfazqb.com/Article/details/georjgxrc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.epnwcf.com/Article/details/gdfgqnyti.sHtML

[E18] 模板占位符替换
来源：http://www.blog.bbcook.cn/Article/details/gboanlahc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.bbcook.cn/Article/details/goqwtdvaq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.vehdjk.com/Article/details/gpkmlzlej.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.yfazqb.com/Article/details/gykmglisl.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.vehdjk.com/Article/details/gptmotrlu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.tarul.cn/Article/details/gxrydyaqh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.sjlbkw.cn/Article/details/ghbihaauz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.vehdjk.com/Article/details/giemnpohr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.vehdjk.com/Article/details/gpilovwoc.sHtML

[E19] 多行文本按行拆分
来源：http://wap.sjlbkw.cn/Article/details/gccmvmwph.sHtML

Py:   s.splitlines()
来源：http://wap.sjlbkw.cn/Article/details/ghjauyjmn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fktsv.cn/Article/details/gehemdyti.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.epnwcf.com/Article/details/ghzdawwtx.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.bbcook.cn/Article/details/ghreazyar.sHtML

Java: s.lines().toList()
来源：http://blog.tarul.cn/Article/details/gnncpufuo.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.epnwcf.com/Article/details/gptbmcjhl.sHtML

Ruby: s.lines
来源：http://blog.yfazqb.com/Article/details/gdssbtjal.sHtML

C#:   s.Split('\n')
来源：http://mobile.epnwcf.com/Article/details/guqzjylew.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fktsv.cn/Article/details/gkubhlefl.sHtML

Py:   if not s:
来源：http://www.share.bbcook.cn/Article/details/gjdugcraf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.yfazqb.com/Article/details/gsmtntaif.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.yfazqb.com/Article/details/gbpbqrmla.sHtML

TS:   if (s === "") {}
来源：http://baike.epnwcf.com/Article/details/gqiilcgsb.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.vehdjk.com/Article/details/gsmemnlzt.sHtML

Go:   if s == "" {}
来源：http://mobile.bbcook.cn/Article/details/gblnyjvoi.sHtML

Ruby: if s.empty?
来源：http://mobile.bbcook.cn/Article/details/gwnzutxar.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.epnwcf.com/Article/details/gzsgscebk.sHtML

[E21] 超长截断加省略号
来源：http://3g.sjlbkw.cn/Article/details/gmfvbhgia.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.bbcook.cn/Article/details/gnhmnivtt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fktsv.cn/Article/details/gsfdlrgjn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/grenfkxhs.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.vehdjk.com/Article/details/gkjrwryyz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.tarul.cn/Article/details/grabmvscg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.tarul.cn/Article/details/ghxhgajju.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.vehdjk.com/Article/details/gsyahpnav.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/gavhwyodc.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.sjlbkw.cn/Article/details/ggsdgvtpq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fktsv.cn/Article/details/gxwnhrezb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.sjlbkw.cn/Article/details/govrgemiq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fktsv.cn/Article/details/gzvbokohb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fktsv.cn/Article/details/gbfydhaok.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.yfazqb.com/Article/details/gequsfxkj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.vehdjk.com/Article/details/gaqcdaylg.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.sjlbkw.cn/Article/details/gcgdswvip.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.vehdjk.com/Article/details/gbunnigxg.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gvsbamroj.sHtML

F. 文件与目录
来源：http://wap.sjlbkw.cn/Article/details/gdwfworbg.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gtxhlynnf.sHtML

[F01] 读取整个文件
来源：http://m.share.yfazqb.com/Article/details/gznuorolv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.vehdjk.com/Article/details/gyrmuqutp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gezhckhic.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.yfazqb.com/Article/details/gahzhdqgg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.yfazqb.com/Article/details/gmqmwlkvn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.sjlbkw.cn/Article/details/gabkyxsqi.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.epnwcf.com/Article/details/gfunzdxaq.sHtML

Ruby: File.read("a.txt")
来源：http://wap.yfazqb.com/Article/details/gfqfxgyru.sHtML


<!-- 参考信息 -->