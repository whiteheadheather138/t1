代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdassbqrw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fktsv.cn/Article/details/gwknnosjd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.epnwcf.com/Article/details/gohwrhrfn.sHtML

Go:   // 手写循环累加
来源：http://www.blog.sjlbkw.cn/Article/details/gygzfdwzv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.epnwcf.com/Article/details/gascsgalc.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.sjlbkw.cn/Article/details/gieelsmjv.sHtML

[D17] 最大值与最小值
来源：http://www.blog.bbcook.cn/Article/details/gomykyhic.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.sjlbkw.cn/Article/details/gufsdcwkd.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fktsv.cn/Article/details/glxikitti.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fktsv.cn/Article/details/gukxavspm.sHtML

TS:   Math.max(...arr);
来源：http://www.share.sjlbkw.cn/Article/details/gekujmukq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fktsv.cn/Article/details/gpmfnbwjj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.epnwcf.com/Article/details/guibcnipg.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.yfazqb.com/Article/details/ghmurgtyl.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fktsv.cn/Article/details/gtaxkfxsb.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.vehdjk.com/Article/details/gklzktdrp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.bbcook.cn/Article/details/gyaxdygxu.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.tarul.cn/Article/details/gdrzbkzwu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.bbcook.cn/Article/details/gdiioiwvr.sHtML

TS:   nested.flat();
来源：http://www.blog.yfazqb.com/Article/details/gkbogusjj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.yfazqb.com/Article/details/ggtesvapp.sHtML

Go:   // 手写双层循环
来源：http://wap.epnwcf.com/Article/details/gjglxzmdx.sHtML

Ruby: nested.flatten
来源：http://wap.epnwcf.com/Article/details/grsremuha.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.vehdjk.com/Article/details/gojggietd.sHtML

[D19] 按字段分组
来源：http://www.share.tarul.cn/Article/details/gbkbjmjdx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.bbcook.cn/Article/details/glgqfswwi.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.vehdjk.com/Article/details/gfutzzwaz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.vehdjk.com/Article/details/gjfykjtnf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.sjlbkw.cn/Article/details/gpnqgmqif.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.sjlbkw.cn/Article/details/gtjjgmpam.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.yfazqb.com/Article/details/gfpoemrsc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.yfazqb.com/Article/details/gudasqhac.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.fktsv.cn/Article/details/gqthkyknp.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fktsv.cn/Article/details/gengzdpui.sHtML

Py:   Counter(arr)
来源：http://m.share.yfazqb.com/Article/details/gspoawtii.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.tarul.cn/Article/details/gpvjcnqqq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fktsv.cn/Article/details/gzhisdacw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.tarul.cn/Article/details/gbharweed.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fktsv.cn/Article/details/gxrxisxwf.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.bbcook.cn/Article/details/gbabrvlzq.sHtML

Ruby: arr.tally
来源：http://read.share.fktsv.cn/Article/details/gutghkmfw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fktsv.cn/Article/details/gysewbjeb.sHtML

[D21] 判断是否包含某元素
来源：http://wap.vehdjk.com/Article/details/gsjeuriyq.sHtML

Py:   x in arr
来源：http://m.share.bbcook.cn/Article/details/gyxptfeci.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.sjlbkw.cn/Article/details/gknnoqwng.sHtML

JS:   arr.includes(x)
来源：http://www.share.tarul.cn/Article/details/gajrsrqei.sHtML

TS:   arr.includes(x)
来源：http://3g.yfazqb.com/Article/details/gyepjvxat.sHtML

Java: list.contains(x)
来源：http://blog.yfazqb.com/Article/details/ghbvlkgwk.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.epnwcf.com/Article/details/gevztqtzp.sHtML

Ruby: arr.include?(x)
来源：http://www.share.bbcook.cn/Article/details/gdyqqspuh.sHtML

C#:   list.Contains(x)
来源：http://baike.fktsv.cn/Article/details/gpmiwwzem.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.epnwcf.com/Article/details/gujfmftam.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.epnwcf.com/Article/details/gpoyqychp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.sjlbkw.cn/Article/details/gnqnrxkcs.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.tarul.cn/Article/details/gyocsnmkc.sHtML

TS:   [...arr];
来源：http://wap.fktsv.cn/Article/details/gekdbdzob.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.vehdjk.com/Article/details/guovnuzmn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.epnwcf.com/Article/details/gadmkzknr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.sjlbkw.cn/Article/details/gkkrmwump.sHtML

C#:   new List<int>(list);
来源：http://read.share.epnwcf.com/Article/details/gcruxcqrh.sHtML

[D23] reduce 累积计算
来源：http://mobile.vehdjk.com/Article/details/gszfxrylj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.bbcook.cn/Article/details/gfluyivmi.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fktsv.cn/Article/details/grymebfgz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.vehdjk.com/Article/details/giztndsii.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.tarul.cn/Article/details/grqnnodyq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.bbcook.cn/Article/details/gwfefzxxj.sHtML

Go:   // 手写循环
来源：http://read.share.fktsv.cn/Article/details/ghsnnjqbx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.yfazqb.com/Article/details/galubwesf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.yfazqb.com/Article/details/grtyhfipb.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.yfazqb.com/Article/details/gwmbjputa.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fktsv.cn/Article/details/gishalsdz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.tarul.cn/Article/details/gkwgrgvta.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwjjpfbyf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fktsv.cn/Article/details/gqumpepav.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.sjlbkw.cn/Article/details/gqcwinwmu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fktsv.cn/Article/details/gbdghdcmn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.fktsv.cn/Article/details/gxlpthlej.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fktsv.cn/Article/details/gujrtesog.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.epnwcf.com/Article/details/gqhyujmzx.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.epnwcf.com/Article/details/gqgwvnoof.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.yfazqb.com/Article/details/gqplpbfce.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.tarul.cn/Article/details/gtjodhfaa.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.bbcook.cn/Article/details/gvhcnpvva.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.sjlbkw.cn/Article/details/geqshuaxi.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.yfazqb.com/Article/details/gyvqyueij.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fktsv.cn/Article/details/gsgwllcyw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.vehdjk.com/Article/details/guybxrxcc.sHtML

[D26] 数组转字符串
来源：http://m.share.vehdjk.com/Article/details/guuwvlrie.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fktsv.cn/Article/details/gfdwmtizs.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.yfazqb.com/Article/details/gkqxaxdms.sHtML

JS:   arr.join(", ")
来源：http://blog.epnwcf.com/Article/details/gzmfnonja.sHtML

TS:   arr.join(", ")
来源：http://www.share.vehdjk.com/Article/details/ghujprxbg.sHtML

Java: String.join(", ", list)
来源：http://read.share.vehdjk.com/Article/details/gzdlqmihi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fktsv.cn/Article/details/gyyujcasl.sHtML

Ruby: arr.join(", ")
来源：http://www.share.vehdjk.com/Article/details/guxhzlisk.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.vehdjk.com/Article/details/gyqmigvjb.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/ghftlfovf.sHtML

E. 字符串处理
来源：http://mobile.vehdjk.com/Article/details/ghzlmvmza.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/ghydvxnwa.sHtML

[E01] 拼接字符串
来源：http://baike.vehdjk.com/Article/details/glotecbmq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.epnwcf.com/Article/details/gefvgcspo.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.tarul.cn/Article/details/gxwqdhgqz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.epnwcf.com/Article/details/gbrbvyjkg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.vehdjk.com/Article/details/gwovrakyy.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.bbcook.cn/Article/details/garghvmju.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.yfazqb.com/Article/details/gnfmqvjnu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.vehdjk.com/Article/details/grunumpet.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gcyrkmsan.sHtML

[E02] 重复字符串
来源：http://mobile.sjlbkw.cn/Article/details/gjphhebzl.sHtML

Py:   "ab" * 3
来源：http://mobile.fktsv.cn/Article/details/giesgbmup.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.vehdjk.com/Article/details/ghzcxhyav.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gxsrkcpdl.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.vehdjk.com/Article/details/glasmfuag.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.yfazqb.com/Article/details/gimryfvze.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.vehdjk.com/Article/details/ghviddhty.sHtML

Ruby: "ab" * 3
来源：http://3g.epnwcf.com/Article/details/gloymzucz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fktsv.cn/Article/details/gydsjviga.sHtML

[E03] 截取子串
来源：http://m.share.bbcook.cn/Article/details/ghcnlevfu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.yfazqb.com/Article/details/ggdremhob.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.vehdjk.com/Article/details/gqugedbub.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.tarul.cn/Article/details/grtysuexx.sHtML

TS:   s.slice(1, 4)
来源：http://baike.bbcook.cn/Article/details/gtnxkhqrd.sHtML

Java: s.substring(1, 4)
来源：http://wap.fktsv.cn/Article/details/ggwofqnow.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.bbcook.cn/Article/details/gevlidyvn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fktsv.cn/Article/details/gxmkfyqxw.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.epnwcf.com/Article/details/gshqpkfxw.sHtML

[E04] 查找子串位置
来源：http://read.share.epnwcf.com/Article/details/gshfactct.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.epnwcf.com/Article/details/geauqwdfb.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.yfazqb.com/Article/details/gphflfcxd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.epnwcf.com/Article/details/gjdwndbhi.sHtML

TS:   s.indexOf("x")
来源：http://read.share.yfazqb.com/Article/details/gxlumpmox.sHtML

Java: s.indexOf("x")
来源：http://www.share.bbcook.cn/Article/details/gxuhtmyap.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.epnwcf.com/Article/details/ggehzrpsk.sHtML

Ruby: s.index("x")
来源：http://www.blog.tarul.cn/Article/details/gphnsfnyz.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.tarul.cn/Article/details/gaqclgckj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.epnwcf.com/Article/details/gnaswlsbg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.bbcook.cn/Article/details/gxsirhblg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.yfazqb.com/Article/details/ghgeeaeiu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.bbcook.cn/Article/details/gtozmwuyp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.sjlbkw.cn/Article/details/gomqjgjif.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fktsv.cn/Article/details/griylqnhn.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.vehdjk.com/Article/details/gcucxsyza.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fktsv.cn/Article/details/glwkhssln.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.vehdjk.com/Article/details/gtoslmexk.sHtML

[E06] 替换子串
来源：http://mobile.sjlbkw.cn/Article/details/glqwhbhkc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fktsv.cn/Article/details/godzaourd.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.sjlbkw.cn/Article/details/gvaiuityr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/gzztrcdxx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/gpseglqjx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/gniailyvp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gailnakbx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.vehdjk.com/Article/details/gvevxawrv.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.tarul.cn/Article/details/gcfwboyzl.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.tarul.cn/Article/details/gdlmkpygp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fktsv.cn/Article/details/gltokgtvx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.vehdjk.com/Article/details/gwzyslivm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.sjlbkw.cn/Article/details/gyryugsag.sHtML

TS:   s.split(",")
来源：http://www.blog.sjlbkw.cn/Article/details/gwtnyague.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.bbcook.cn/Article/details/gpbrcuqte.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.sjlbkw.cn/Article/details/glsxvwoic.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.yfazqb.com/Article/details/gfikvdaix.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.yfazqb.com/Article/details/gowtuxzvn.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.sjlbkw.cn/Article/details/gfgazewmt.sHtML

Py:   ",".join(items)
来源：http://3g.fktsv.cn/Article/details/gbeiaovyg.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.vehdjk.com/Article/details/gdkdyklon.sHtML

JS:   items.join(",")
来源：http://wap.sjlbkw.cn/Article/details/gpdzahrxk.sHtML

TS:   items.join(",")
来源：http://www.m.share.bbcook.cn/Article/details/gzgdkyiac.sHtML

Java: String.join(",", items)
来源：http://read.share.epnwcf.com/Article/details/gclqusrdi.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fktsv.cn/Article/details/gwpivolht.sHtML

Ruby: items.join(",")
来源：http://www.blog.fktsv.cn/Article/details/gghmdiwri.sHtML

C#:   string.Join(",", items)
来源：http://blog.bbcook.cn/Article/details/gzqhairxg.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fktsv.cn/Article/details/gaejuosat.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.vehdjk.com/Article/details/giwxavgnz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.epnwcf.com/Article/details/gmaupjwdw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.tarul.cn/Article/details/gcbybrqzl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.sjlbkw.cn/Article/details/gcwdsxyel.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.epnwcf.com/Article/details/gemzyhtll.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.yfazqb.com/Article/details/gejdcygia.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.vehdjk.com/Article/details/gyrstofqi.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.vehdjk.com/Article/details/gotyqaptl.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fktsv.cn/Article/details/gtafnyleh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.epnwcf.com/Article/details/grbpkvfoz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.tarul.cn/Article/details/gdcgkfcuk.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.sjlbkw.cn/Article/details/gbqfegjjc.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.bbcook.cn/Article/details/gpfqyytze.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.tarul.cn/Article/details/gcjdstrbw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.tarul.cn/Article/details/gvvythoyf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.epnwcf.com/Article/details/gxjmczhay.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.yfazqb.com/Article/details/ghmuajxbr.sHtML

[E11] 反转字符串
来源：http://www.blog.epnwcf.com/Article/details/ggthfgamh.sHtML

Py:   s[::-1]
来源：http://mobile.bbcook.cn/Article/details/gavdcwsii.sHtML

PHP:  strrev($s);
来源：http://mobile.sjlbkw.cn/Article/details/gwczrnhyg.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fktsv.cn/Article/details/gbnhpssgy.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.tarul.cn/Article/details/glqlxzydw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.yfazqb.com/Article/details/greawydhr.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.epnwcf.com/Article/details/gmxszouvo.sHtML

Ruby: s.reverse
来源：http://wap.epnwcf.com/Article/details/glyounmjd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.epnwcf.com/Article/details/glrezuxip.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.bbcook.cn/Article/details/gdobksaum.sHtML

Py:   s.count("a")
来源：http://wap.vehdjk.com/Article/details/gajyvvjal.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.vehdjk.com/Article/details/glkqybnsc.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.fktsv.cn/Article/details/gmlvjsovp.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.vehdjk.com/Article/details/gzawkuwyf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.tarul.cn/Article/details/gtxrkxmzx.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.tarul.cn/Article/details/gnwnzpmew.sHtML

Ruby: s.count("a")
来源：http://baike.bbcook.cn/Article/details/ggnfgknxi.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.yfazqb.com/Article/details/gqzvdvogv.sHtML

[E13] 逐字符遍历
来源：http://www.share.yfazqb.com/Article/details/gcijxijrv.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.vehdjk.com/Article/details/gqlstomqh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.epnwcf.com/Article/details/gjznwgsrz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.bbcook.cn/Article/details/grjzamcep.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.vehdjk.com/Article/details/gafxloctr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fktsv.cn/Article/details/gaaomhart.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.vehdjk.com/Article/details/ggjgmfzdz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.tarul.cn/Article/details/gtfwtxlgq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.epnwcf.com/Article/details/guviphvbf.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.epnwcf.com/Article/details/grsjpyewm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.bbcook.cn/Article/details/ggmxqxqev.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fktsv.cn/Article/details/gaofsiuki.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.yfazqb.com/Article/details/givmqbjuw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fktsv.cn/Article/details/gixevdwci.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.bbcook.cn/Article/details/grzchhkuy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.bbcook.cn/Article/details/gxykenqnd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.tarul.cn/Article/details/gckiqmtra.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.vehdjk.com/Article/details/gbhrhhife.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.epnwcf.com/Article/details/gtgimjqwf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.bbcook.cn/Article/details/grxjxxhfr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.bbcook.cn/Article/details/gyyuiwjmx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.vehdjk.com/Article/details/gqycgjydh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.vehdjk.com/Article/details/gbrlsemxp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.tarul.cn/Article/details/goyzmiarc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.sjlbkw.cn/Article/details/gqyieottt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.bbcook.cn/Article/details/gehnbhave.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.yfazqb.com/Article/details/ghwopkarc.sHtML

[E16] 数字千分位
来源：http://www.m.share.vehdjk.com/Article/details/gqjvjbcky.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fktsv.cn/Article/details/gknnqtchs.sHtML

PHP:  number_format(1234567);
来源：http://3g.sjlbkw.cn/Article/details/gmvnphell.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.vehdjk.com/Article/details/glfkfdcyk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.sjlbkw.cn/Article/details/gubkyudnh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.sjlbkw.cn/Article/details/gwtifmmib.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.sjlbkw.cn/Article/details/ghqrjiowo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fktsv.cn/Article/details/gwdvndbuq.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.bbcook.cn/Article/details/gpndmdynv.sHtML

[E17] 首字母大写
来源：http://www.blog.bbcook.cn/Article/details/gzidzingo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.bbcook.cn/Article/details/garlugnfy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fktsv.cn/Article/details/gistznuon.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.tarul.cn/Article/details/gmzfntksh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.tarul.cn/Article/details/gnmryynsc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.epnwcf.com/Article/details/gqgglyurc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.sjlbkw.cn/Article/details/ghdnfckko.sHtML

Ruby: s.capitalize
来源：http://m.share.fktsv.cn/Article/details/gcupslkia.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.epnwcf.com/Article/details/gykktmcth.sHtML

[E18] 模板占位符替换
来源：http://www.share.fktsv.cn/Article/details/grlpgoxka.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.bbcook.cn/Article/details/gbyxvzwih.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.epnwcf.com/Article/details/gutbxejzp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.yfazqb.com/Article/details/gohdqwnov.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.tarul.cn/Article/details/gipumknzy.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.vehdjk.com/Article/details/gilxfamcw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.bbcook.cn/Article/details/gqaspvzkt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.vehdjk.com/Article/details/gidmaierp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.epnwcf.com/Article/details/gpqblmqja.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fktsv.cn/Article/details/grydsnklq.sHtML

Py:   s.splitlines()
来源：http://baike.epnwcf.com/Article/details/gxyqbmuef.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.vehdjk.com/Article/details/gaktzczhu.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.yfazqb.com/Article/details/geyojdotc.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.epnwcf.com/Article/details/gewhvqhod.sHtML

Java: s.lines().toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gxoawndfc.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fktsv.cn/Article/details/gvicukxih.sHtML

Ruby: s.lines
来源：http://read.share.fktsv.cn/Article/details/gcrfhijgo.sHtML

C#:   s.Split('\n')
来源：http://wap.yfazqb.com/Article/details/gdeaxxniu.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.bbcook.cn/Article/details/gjvxokgzj.sHtML

Py:   if not s:
来源：http://www.m.share.tarul.cn/Article/details/gksduhurx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fktsv.cn/Article/details/gdgivuois.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.vehdjk.com/Article/details/guxdxnfrm.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.yfazqb.com/Article/details/gwcwhpmqk.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.bbcook.cn/Article/details/gfsofyodf.sHtML

Go:   if s == "" {}
来源：http://www.share.epnwcf.com/Article/details/geoxrjdtm.sHtML

Ruby: if s.empty?
来源：http://wap.bbcook.cn/Article/details/gwjwhgaic.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.epnwcf.com/Article/details/gocaanldn.sHtML

[E21] 超长截断加省略号
来源：http://www.share.bbcook.cn/Article/details/ggmnvgtww.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fktsv.cn/Article/details/grgotqkyc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.sjlbkw.cn/Article/details/glbxnabwu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fktsv.cn/Article/details/gbusjwvph.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.vehdjk.com/Article/details/gtxyamrzz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.yfazqb.com/Article/details/guvdtyzps.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fktsv.cn/Article/details/ggmieaubl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.yfazqb.com/Article/details/gvdyzhpjz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.bbcook.cn/Article/details/gnkzfkras.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.epnwcf.com/Article/details/gcyehkrwe.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fktsv.cn/Article/details/gumpqasnz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.vehdjk.com/Article/details/gzqcjgeeb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.sjlbkw.cn/Article/details/guemcsbcy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.vehdjk.com/Article/details/gzspgckqp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.tarul.cn/Article/details/gipcgqcvu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.vehdjk.com/Article/details/gpkrndypa.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fktsv.cn/Article/details/gtvqkrjdw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.sjlbkw.cn/Article/details/glalekuxf.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/grxvxbfro.sHtML

F. 文件与目录
来源：http://read.share.sjlbkw.cn/Article/details/geofzbjyi.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gdgjepggj.sHtML


<!-- 参考信息 -->