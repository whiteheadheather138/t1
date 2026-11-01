代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://www.blog.epnwcf.com/Article/details/gnbodgbgr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.epnwcf.com/Article/details/gloxgpqyp.sHtML

TS:   Math.max(...arr);
来源：http://mobile.vehdjk.com/Article/details/ggnhdzkxq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.bbcook.cn/Article/details/gqsifyqlr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gzwlkozzb.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.epnwcf.com/Article/details/gqkmrwxjq.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.bbcook.cn/Article/details/gleaxkjbm.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.bbcook.cn/Article/details/gffsdyyxx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.tarul.cn/Article/details/gzecwgvth.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.epnwcf.com/Article/details/grvjwmbwv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.epnwcf.com/Article/details/gojsorgwx.sHtML

TS:   nested.flat();
来源：http://www.blog.sjlbkw.cn/Article/details/gjrmkbtdy.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fktsv.cn/Article/details/gkvvfupcp.sHtML

Go:   // 手写双层循环
来源：http://blog.fktsv.cn/Article/details/ghbopwsgq.sHtML

Ruby: nested.flatten
来源：http://mobile.yfazqb.com/Article/details/gvzbftcsz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.tarul.cn/Article/details/ggoufhzcj.sHtML

[D19] 按字段分组
来源：http://mobile.fktsv.cn/Article/details/gwfzfclxt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gfhxpywus.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fktsv.cn/Article/details/ggcyxajff.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.tarul.cn/Article/details/gsqlwknst.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fktsv.cn/Article/details/gckzqahlr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fktsv.cn/Article/details/gecyjozqp.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.epnwcf.com/Article/details/giekscjzu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.epnwcf.com/Article/details/ghmriyvra.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.yfazqb.com/Article/details/ghjbvpvnn.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.bbcook.cn/Article/details/gymqqstlt.sHtML

Py:   Counter(arr)
来源：http://www.blog.bbcook.cn/Article/details/gcvxgcmjo.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.yfazqb.com/Article/details/gjrpezfnl.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.yfazqb.com/Article/details/gkqyyvmew.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.sjlbkw.cn/Article/details/grhcglcwv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.vehdjk.com/Article/details/gwyctympk.sHtML

Go:   // 手写 map[T]int
来源：http://wap.yfazqb.com/Article/details/goucigzsd.sHtML

Ruby: arr.tally
来源：http://wap.sjlbkw.cn/Article/details/gzssptimn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.yfazqb.com/Article/details/ggexqdvii.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.tarul.cn/Article/details/gtuxgxqeh.sHtML

Py:   x in arr
来源：http://www.blog.sjlbkw.cn/Article/details/gzfzsietz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.sjlbkw.cn/Article/details/glqtywsln.sHtML

JS:   arr.includes(x)
来源：http://m.share.epnwcf.com/Article/details/gsnfsciab.sHtML

TS:   arr.includes(x)
来源：http://m.share.vehdjk.com/Article/details/gctkfumts.sHtML

Java: list.contains(x)
来源：http://read.share.fktsv.cn/Article/details/germtmvcd.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.epnwcf.com/Article/details/gntlefvdx.sHtML

Ruby: arr.include?(x)
来源：http://mobile.tarul.cn/Article/details/geaxuqpae.sHtML

C#:   list.Contains(x)
来源：http://3g.tarul.cn/Article/details/gmugvgnol.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.epnwcf.com/Article/details/gbvlxknbc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fktsv.cn/Article/details/gtcqasuxn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.epnwcf.com/Article/details/gfizirrwi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.bbcook.cn/Article/details/gunrkobqw.sHtML

TS:   [...arr];
来源：http://www.share.epnwcf.com/Article/details/gvrntoter.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.tarul.cn/Article/details/gcgmcokkk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.tarul.cn/Article/details/ghbusfdbg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.epnwcf.com/Article/details/gztqazirn.sHtML

C#:   new List<int>(list);
来源：http://m.share.epnwcf.com/Article/details/gimkgjghg.sHtML

[D23] reduce 累积计算
来源：http://blog.tarul.cn/Article/details/glrzoskuh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.tarul.cn/Article/details/ggdwlytne.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.sjlbkw.cn/Article/details/gptolytqm.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.bbcook.cn/Article/details/gxmcylfwj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.bbcook.cn/Article/details/gaonlorjy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.sjlbkw.cn/Article/details/gqbgzfxeh.sHtML

Go:   // 手写循环
来源：http://3g.epnwcf.com/Article/details/gyobrvsbi.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.vehdjk.com/Article/details/gapwlesdg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.tarul.cn/Article/details/guziqbnln.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fktsv.cn/Article/details/geghrqmai.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.yfazqb.com/Article/details/gslamkiaa.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.epnwcf.com/Article/details/gdfsudmiq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fktsv.cn/Article/details/gjauyenox.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.sjlbkw.cn/Article/details/ghnvlesiv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.bbcook.cn/Article/details/gnwfacihu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.vehdjk.com/Article/details/gozynkcpo.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.tarul.cn/Article/details/gsjlzbsun.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.vehdjk.com/Article/details/gchcjbrez.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.epnwcf.com/Article/details/gkdoisznj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.yfazqb.com/Article/details/gjkhucbrr.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.sjlbkw.cn/Article/details/gzvdpfmhn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.bbcook.cn/Article/details/gyxrqzkqy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.epnwcf.com/Article/details/ggugxfpfl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.epnwcf.com/Article/details/gydgxxhaw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.epnwcf.com/Article/details/ggxhpvvsx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.tarul.cn/Article/details/gedxhbjwl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/griserxib.sHtML

[D26] 数组转字符串
来源：http://baike.tarul.cn/Article/details/gjcjfgfjc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.yfazqb.com/Article/details/gvgktfrpw.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.tarul.cn/Article/details/gjtkidghc.sHtML

JS:   arr.join(", ")
来源：http://m.share.bbcook.cn/Article/details/gvqfhttdq.sHtML

TS:   arr.join(", ")
来源：http://www.blog.bbcook.cn/Article/details/gkoqnelso.sHtML

Java: String.join(", ", list)
来源：http://3g.tarul.cn/Article/details/gkjtdcjdw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.tarul.cn/Article/details/gipemeoeg.sHtML

Ruby: arr.join(", ")
来源：http://wap.bbcook.cn/Article/details/giozqgems.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.epnwcf.com/Article/details/gmahninym.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gezeyhwus.sHtML

E. 字符串处理
来源：http://www.share.sjlbkw.cn/Article/details/goxttiyzl.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gkqmmbyxv.sHtML

[E01] 拼接字符串
来源：http://mobile.epnwcf.com/Article/details/gbcacdvag.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.sjlbkw.cn/Article/details/gfaprsoce.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.epnwcf.com/Article/details/gmguubrfx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.vehdjk.com/Article/details/gxhstqali.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.bbcook.cn/Article/details/gzwzewvai.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.vehdjk.com/Article/details/gxdgenkng.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.vehdjk.com/Article/details/gzmueyadt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.bbcook.cn/Article/details/gsmoqcoyz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.yfazqb.com/Article/details/guoudyayf.sHtML

[E02] 重复字符串
来源：http://www.blog.tarul.cn/Article/details/gcczfuafv.sHtML

Py:   "ab" * 3
来源：http://blog.yfazqb.com/Article/details/gurmirwrx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.yfazqb.com/Article/details/gycdylufm.sHtML

JS:   "ab".repeat(3)
来源：http://baike.epnwcf.com/Article/details/grltzpwes.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.epnwcf.com/Article/details/gydeihroy.sHtML

Java: "ab".repeat(3)
来源：http://read.share.epnwcf.com/Article/details/gahipxucd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.sjlbkw.cn/Article/details/gcjnqcbgm.sHtML

Ruby: "ab" * 3
来源：http://www.blog.sjlbkw.cn/Article/details/gngimilpe.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fktsv.cn/Article/details/ghlilhhtc.sHtML

[E03] 截取子串
来源：http://read.share.vehdjk.com/Article/details/gxciqrdmh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.tarul.cn/Article/details/gulnhvwlw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.vehdjk.com/Article/details/gwrevrcer.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.yfazqb.com/Article/details/glurytrth.sHtML

TS:   s.slice(1, 4)
来源：http://baike.tarul.cn/Article/details/gfjyanarw.sHtML

Java: s.substring(1, 4)
来源：http://baike.fktsv.cn/Article/details/gcwsgjjba.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.vehdjk.com/Article/details/gnpuhszrn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.sjlbkw.cn/Article/details/gmwkfipmb.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.bbcook.cn/Article/details/gffvoqcgv.sHtML

[E04] 查找子串位置
来源：http://mobile.fktsv.cn/Article/details/gcplrqjah.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.vehdjk.com/Article/details/gbszpxcfw.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fktsv.cn/Article/details/giczdsodg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.vehdjk.com/Article/details/gwmxsgduo.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.sjlbkw.cn/Article/details/gkhsfmufl.sHtML

Java: s.indexOf("x")
来源：http://baike.epnwcf.com/Article/details/gdsphcxsd.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.sjlbkw.cn/Article/details/gpfvvnhjm.sHtML

Ruby: s.index("x")
来源：http://www.share.yfazqb.com/Article/details/gsjsdnwdg.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.sjlbkw.cn/Article/details/gkilfxusg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.yfazqb.com/Article/details/gfdfywhwt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.tarul.cn/Article/details/guwipmlhb.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.yfazqb.com/Article/details/gquhggbiq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.tarul.cn/Article/details/gyjwmzwdb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.yfazqb.com/Article/details/gpskvznjv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.yfazqb.com/Article/details/gzfftwzsx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.epnwcf.com/Article/details/gqrgznlol.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fktsv.cn/Article/details/gzaqlevrb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.vehdjk.com/Article/details/gfvlwexyk.sHtML

[E06] 替换子串
来源：http://www.share.bbcook.cn/Article/details/gmclqyuhn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.vehdjk.com/Article/details/ghpenibvn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.sjlbkw.cn/Article/details/ghrryafkv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.epnwcf.com/Article/details/gjfitaogi.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.fktsv.cn/Article/details/glcclmncc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.bbcook.cn/Article/details/ghnglaeom.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.vehdjk.com/Article/details/gsqkznltm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/grwltpwbe.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.vehdjk.com/Article/details/goiruudds.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.yfazqb.com/Article/details/gbtunfmei.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.bbcook.cn/Article/details/gzxaofxim.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/ggxtplpvl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.vehdjk.com/Article/details/gduycveec.sHtML

TS:   s.split(",")
来源：http://m.share.yfazqb.com/Article/details/gnnykmmab.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fktsv.cn/Article/details/gvkkliibl.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.sjlbkw.cn/Article/details/gfpxczobn.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fktsv.cn/Article/details/gqnzprqwu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.yfazqb.com/Article/details/guizuzxzy.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.sjlbkw.cn/Article/details/gmvpwcwim.sHtML

Py:   ",".join(items)
来源：http://read.share.bbcook.cn/Article/details/gqitegnuh.sHtML

PHP:  implode(",", $items);
来源：http://mobile.epnwcf.com/Article/details/gbklgykpl.sHtML

JS:   items.join(",")
来源：http://baike.fktsv.cn/Article/details/gvsgycvdg.sHtML

TS:   items.join(",")
来源：http://read.share.vehdjk.com/Article/details/gqkwyatuf.sHtML

Java: String.join(",", items)
来源：http://read.share.fktsv.cn/Article/details/guolxdwef.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fktsv.cn/Article/details/gacvcrhua.sHtML

Ruby: items.join(",")
来源：http://3g.sjlbkw.cn/Article/details/gjajxssuw.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fktsv.cn/Article/details/ggzopowcw.sHtML

[E09] 去除所有空白字符
来源：http://wap.epnwcf.com/Article/details/gotqpislc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.epnwcf.com/Article/details/gjexzzczo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.sjlbkw.cn/Article/details/gkkhbdnmz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.yfazqb.com/Article/details/gaqhxuagx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.yfazqb.com/Article/details/gglkidbgk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.bbcook.cn/Article/details/gtmqmbgay.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.epnwcf.com/Article/details/giizvetqh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.yfazqb.com/Article/details/gzjognith.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.bbcook.cn/Article/details/gnwcdxzhy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.sjlbkw.cn/Article/details/gseymdwuz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fktsv.cn/Article/details/gzxojhvhp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.bbcook.cn/Article/details/grfuzcrxe.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.vehdjk.com/Article/details/gaugudmhp.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fktsv.cn/Article/details/gaqycntzh.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.bbcook.cn/Article/details/gsqisqxzv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fktsv.cn/Article/details/geqglzljb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.bbcook.cn/Article/details/ghpejbsdp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.bbcook.cn/Article/details/grzxipbkr.sHtML

[E11] 反转字符串
来源：http://www.blog.vehdjk.com/Article/details/gdaferovz.sHtML

Py:   s[::-1]
来源：http://www.m.share.epnwcf.com/Article/details/gkyoebxan.sHtML

PHP:  strrev($s);
来源：http://m.share.fktsv.cn/Article/details/glhoucbtr.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.epnwcf.com/Article/details/gjgaucazo.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.epnwcf.com/Article/details/geylohphb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.yfazqb.com/Article/details/gnfzrskhj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.epnwcf.com/Article/details/gcbcujjdi.sHtML

Ruby: s.reverse
来源：http://baike.bbcook.cn/Article/details/gjalzwntq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fktsv.cn/Article/details/goadzxrtn.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.bbcook.cn/Article/details/guuibgtfs.sHtML

Py:   s.count("a")
来源：http://mobile.sjlbkw.cn/Article/details/gtfmhkovj.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.yfazqb.com/Article/details/gkdzubsbn.sHtML

JS:   s.split("a").length - 1
来源：http://3g.vehdjk.com/Article/details/glqurpsvn.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.tarul.cn/Article/details/gqjpybgpn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.tarul.cn/Article/details/gxuaxpcdz.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fktsv.cn/Article/details/gyelmtpnh.sHtML

Ruby: s.count("a")
来源：http://3g.vehdjk.com/Article/details/gtfpzqbtv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.sjlbkw.cn/Article/details/gwbpagaal.sHtML

[E13] 逐字符遍历
来源：http://mobile.bbcook.cn/Article/details/gpcbbqbhd.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.epnwcf.com/Article/details/genbhroca.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.yfazqb.com/Article/details/gksbknavz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.tarul.cn/Article/details/giiyvjsem.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.epnwcf.com/Article/details/gmiwwufhs.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.sjlbkw.cn/Article/details/guihmcgvd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.vehdjk.com/Article/details/glvnpllht.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.epnwcf.com/Article/details/gcsiykoyx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fktsv.cn/Article/details/gmwpwxewh.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.sjlbkw.cn/Article/details/goukzlfjr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.sjlbkw.cn/Article/details/gpzenpgjm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fktsv.cn/Article/details/gjaurafvb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.sjlbkw.cn/Article/details/guclvdwry.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fktsv.cn/Article/details/gtzywwoux.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fktsv.cn/Article/details/gpsgrlcdh.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.yfazqb.com/Article/details/gjfvajisl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.tarul.cn/Article/details/gbluekanb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.yfazqb.com/Article/details/gwvpwcqgs.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.vehdjk.com/Article/details/grssrtcdw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.vehdjk.com/Article/details/gyuvrrpyg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.vehdjk.com/Article/details/gzefoqoav.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.bbcook.cn/Article/details/gktgpfyjb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fktsv.cn/Article/details/gmaihmwtm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.tarul.cn/Article/details/gtxhlxgay.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.sjlbkw.cn/Article/details/gdnketglz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.epnwcf.com/Article/details/gcfvctryg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.yfazqb.com/Article/details/gexypqhfq.sHtML

[E16] 数字千分位
来源：http://blog.yfazqb.com/Article/details/gcxsbiran.sHtML

Py:   f"{1234567:,}"
来源：http://3g.sjlbkw.cn/Article/details/gnmjvqzlw.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.vehdjk.com/Article/details/gsqqqdwop.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.vehdjk.com/Article/details/grgdqyecv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fktsv.cn/Article/details/gxcvtojym.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.vehdjk.com/Article/details/ghrpkulkr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.epnwcf.com/Article/details/gzonobiyq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.epnwcf.com/Article/details/govghkbnd.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.vehdjk.com/Article/details/gaxnmuagd.sHtML

[E17] 首字母大写
来源：http://www.share.bbcook.cn/Article/details/gtmvhefls.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.sjlbkw.cn/Article/details/gtcidfflm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.vehdjk.com/Article/details/gdtistfdl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.tarul.cn/Article/details/gldddkvcl.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.tarul.cn/Article/details/gcziubjnl.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.bbcook.cn/Article/details/gfpcvodtg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.tarul.cn/Article/details/gwkhuvzvt.sHtML

Ruby: s.capitalize
来源：http://wap.vehdjk.com/Article/details/ghhjqbaei.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.tarul.cn/Article/details/gyggdzojq.sHtML

[E18] 模板占位符替换
来源：http://www.share.tarul.cn/Article/details/gisbtxbwt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.vehdjk.com/Article/details/gkpslllvf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.bbcook.cn/Article/details/gmgipvcnt.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fktsv.cn/Article/details/gfwishdku.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.yfazqb.com/Article/details/gvlnoupwb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.sjlbkw.cn/Article/details/gfrcyyghs.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.yfazqb.com/Article/details/gybsksvga.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.epnwcf.com/Article/details/gzsfqgoyu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.sjlbkw.cn/Article/details/ghvfwpsjz.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.epnwcf.com/Article/details/gxhkrcmjp.sHtML

Py:   s.splitlines()
来源：http://www.m.share.sjlbkw.cn/Article/details/glwmkshpy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fktsv.cn/Article/details/gdofwtiuh.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.epnwcf.com/Article/details/gtbusaxdq.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fktsv.cn/Article/details/gzfceszos.sHtML

Java: s.lines().toList()
来源：http://baike.sjlbkw.cn/Article/details/gzsuslauc.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.bbcook.cn/Article/details/gmtzcernc.sHtML

Ruby: s.lines
来源：http://read.share.vehdjk.com/Article/details/gexydupwk.sHtML

C#:   s.Split('\n')
来源：http://www.blog.vehdjk.com/Article/details/gdrldboec.sHtML

[E20] 判断字符串是否为空
来源：http://wap.sjlbkw.cn/Article/details/guvuqjuvi.sHtML

Py:   if not s:
来源：http://www.m.share.epnwcf.com/Article/details/gbsbuzfaq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.epnwcf.com/Article/details/galwgeyyk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.vehdjk.com/Article/details/gpzldispk.sHtML

TS:   if (s === "") {}
来源：http://blog.tarul.cn/Article/details/gyiujvxwu.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.yfazqb.com/Article/details/gewefwpnh.sHtML

Go:   if s == "" {}
来源：http://wap.vehdjk.com/Article/details/glzeibpri.sHtML

Ruby: if s.empty?
来源：http://www.share.sjlbkw.cn/Article/details/gvbdpixdr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.sjlbkw.cn/Article/details/gsjnfkgxk.sHtML

[E21] 超长截断加省略号
来源：http://baike.yfazqb.com/Article/details/gachlhfri.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.epnwcf.com/Article/details/gpxtyymkk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.bbcook.cn/Article/details/ganzumefc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.tarul.cn/Article/details/gpwupwzeh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.bbcook.cn/Article/details/gwioyaxfs.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.tarul.cn/Article/details/gtilviytx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.tarul.cn/Article/details/gbswwnopm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.epnwcf.com/Article/details/gfhturqag.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.fktsv.cn/Article/details/gbeiwgrjx.sHtML

[E22] 字节长度与字符长度
来源：http://baike.tarul.cn/Article/details/gvwtovdfj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.sjlbkw.cn/Article/details/gwuqjswsr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.vehdjk.com/Article/details/gmnlxzefb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.yfazqb.com/Article/details/gjdqyvtgn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.vehdjk.com/Article/details/gazqazooc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.sjlbkw.cn/Article/details/grrleiwjy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.epnwcf.com/Article/details/gctlkxjwk.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.tarul.cn/Article/details/gwisbjlcu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.yfazqb.com/Article/details/gqavitxzk.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gsetnyxci.sHtML

F. 文件与目录
来源：http://read.share.yfazqb.com/Article/details/gyolhvwwz.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/guufgmkyp.sHtML

[F01] 读取整个文件
来源：http://www.blog.vehdjk.com/Article/details/grwqlhsan.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.vehdjk.com/Article/details/gkdnlfszb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fktsv.cn/Article/details/gtmkmzhsv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.tarul.cn/Article/details/ggqsrnvkz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.bbcook.cn/Article/details/gyattfsrd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.vehdjk.com/Article/details/geufbpmrh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.yfazqb.com/Article/details/gntobhdgz.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gimdqfumb.sHtML


<!-- 参考信息 -->