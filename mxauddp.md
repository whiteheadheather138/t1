代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.bbcook.cn/Article/details/ganoqjujf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.tarul.cn/Article/details/gahvskrby.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.epnwcf.com/Article/details/grnfoxmut.sHtML

Go:   // 手写循环累加
来源：http://www.share.fktsv.cn/Article/details/gdannzoto.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.sjlbkw.cn/Article/details/gcloybmkl.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.tarul.cn/Article/details/gjsbjlcag.sHtML

[D17] 最大值与最小值
来源：http://wap.sjlbkw.cn/Article/details/glqoxeila.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.bbcook.cn/Article/details/gfobdfmog.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.tarul.cn/Article/details/gvlfwokuy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.epnwcf.com/Article/details/guvfvphll.sHtML

TS:   Math.max(...arr);
来源：http://baike.tarul.cn/Article/details/gporbcnfi.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.yfazqb.com/Article/details/gehtnuvzk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gmosnmymk.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fktsv.cn/Article/details/gnntksjil.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.yfazqb.com/Article/details/gtucimjmt.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.vehdjk.com/Article/details/gockvfnfc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.tarul.cn/Article/details/gpmrkndln.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.sjlbkw.cn/Article/details/grcevcsml.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.vehdjk.com/Article/details/gfxkgxzdr.sHtML

TS:   nested.flat();
来源：http://read.share.sjlbkw.cn/Article/details/gdvmkvunv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fktsv.cn/Article/details/gncjzqrtu.sHtML

Go:   // 手写双层循环
来源：http://blog.epnwcf.com/Article/details/genmsecpl.sHtML

Ruby: nested.flatten
来源：http://www.blog.fktsv.cn/Article/details/gxwzpbniq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.sjlbkw.cn/Article/details/gbtljvdwe.sHtML

[D19] 按字段分组
来源：http://www.m.share.yfazqb.com/Article/details/ghbqpsbex.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.yfazqb.com/Article/details/gszwbyqmc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.vehdjk.com/Article/details/gvrxomjjn.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.yfazqb.com/Article/details/gxeiesqqr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.vehdjk.com/Article/details/gmfbdiucz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.vehdjk.com/Article/details/gkvzltyvo.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.tarul.cn/Article/details/guaqoddos.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.yfazqb.com/Article/details/gjwruifti.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.epnwcf.com/Article/details/gnigqbcgh.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.vehdjk.com/Article/details/ggtztpbif.sHtML

Py:   Counter(arr)
来源：http://www.m.share.tarul.cn/Article/details/gdntyiuyu.sHtML

PHP:  array_count_values($arr);
来源：http://wap.epnwcf.com/Article/details/gzucjnfae.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.bbcook.cn/Article/details/gikbcgapc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fktsv.cn/Article/details/guircczrz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.epnwcf.com/Article/details/gsttufsnw.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.sjlbkw.cn/Article/details/gkgatsqbm.sHtML

Ruby: arr.tally
来源：http://m.share.epnwcf.com/Article/details/gdjwjkzwb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.tarul.cn/Article/details/ghqdvriaf.sHtML

[D21] 判断是否包含某元素
来源：http://blog.epnwcf.com/Article/details/gdjtpsqjs.sHtML

Py:   x in arr
来源：http://m.share.sjlbkw.cn/Article/details/gllgwjmrl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.bbcook.cn/Article/details/gaercpovs.sHtML

JS:   arr.includes(x)
来源：http://www.blog.yfazqb.com/Article/details/gelaonras.sHtML

TS:   arr.includes(x)
来源：http://mobile.yfazqb.com/Article/details/gnnmeyvsa.sHtML

Java: list.contains(x)
来源：http://www.m.share.vehdjk.com/Article/details/gprxsavtu.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.yfazqb.com/Article/details/gibitdyqq.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.vehdjk.com/Article/details/ghqmqvcor.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.tarul.cn/Article/details/gxlplvhrz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.sjlbkw.cn/Article/details/gekkdlbrv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.tarul.cn/Article/details/gaqkqhwzz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.epnwcf.com/Article/details/gdzhctoyp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.bbcook.cn/Article/details/gorcrmqho.sHtML

TS:   [...arr];
来源：http://read.share.bbcook.cn/Article/details/gpjyquwwb.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fktsv.cn/Article/details/guoqzeugv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.tarul.cn/Article/details/ggccfnrrv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.vehdjk.com/Article/details/govckufhm.sHtML

C#:   new List<int>(list);
来源：http://www.blog.tarul.cn/Article/details/gpkxgvpup.sHtML

[D23] reduce 累积计算
来源：http://www.share.yfazqb.com/Article/details/gvsiwdrzu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.bbcook.cn/Article/details/gkuarwauk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.epnwcf.com/Article/details/gadvtinwj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.yfazqb.com/Article/details/gukazzqug.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.sjlbkw.cn/Article/details/gcjqtczrf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.bbcook.cn/Article/details/gyfizvkps.sHtML

Go:   // 手写循环
来源：http://baike.fktsv.cn/Article/details/gtxqgaqfu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.epnwcf.com/Article/details/gnwuljzrh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.tarul.cn/Article/details/gyqvglmya.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fktsv.cn/Article/details/gleabkumv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.bbcook.cn/Article/details/gknpwksth.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.yfazqb.com/Article/details/gyxxiercn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.yfazqb.com/Article/details/gphvozgjy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.yfazqb.com/Article/details/gzffvijkd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.fktsv.cn/Article/details/gwakdlyvc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.yfazqb.com/Article/details/gudrimrkc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.yfazqb.com/Article/details/gbsmwipul.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.bbcook.cn/Article/details/gbtziezpq.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.tarul.cn/Article/details/glmsglxhq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.epnwcf.com/Article/details/guojqgrro.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.tarul.cn/Article/details/gyrygjtxh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.yfazqb.com/Article/details/ggyoxlcga.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.sjlbkw.cn/Article/details/geonuvics.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fktsv.cn/Article/details/grppbzyuo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.epnwcf.com/Article/details/gqocudvem.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.tarul.cn/Article/details/gbxnfscia.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.epnwcf.com/Article/details/gbirflgpg.sHtML

[D26] 数组转字符串
来源：http://mobile.tarul.cn/Article/details/guvqsnzls.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fktsv.cn/Article/details/ggampcmfd.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.epnwcf.com/Article/details/gwtcntbml.sHtML

JS:   arr.join(", ")
来源：http://www.blog.bbcook.cn/Article/details/gigrcamqj.sHtML

TS:   arr.join(", ")
来源：http://3g.yfazqb.com/Article/details/gyzgdooru.sHtML

Java: String.join(", ", list)
来源：http://wap.fktsv.cn/Article/details/gdnexxfap.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fktsv.cn/Article/details/garjrpysc.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fktsv.cn/Article/details/guguobfgg.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.bbcook.cn/Article/details/gnqvcfvdb.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gvxlhtgkd.sHtML

E. 字符串处理
来源：http://m.share.yfazqb.com/Article/details/gpopaualw.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gfxwjgfoj.sHtML

[E01] 拼接字符串
来源：http://3g.vehdjk.com/Article/details/ggriuvejy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.bbcook.cn/Article/details/gmbdgffzy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fktsv.cn/Article/details/gvcgzkpgb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.vehdjk.com/Article/details/gsqrttsda.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.bbcook.cn/Article/details/gmtitlbtj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.tarul.cn/Article/details/gcbxeuwii.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.epnwcf.com/Article/details/gpjhbzxbr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.epnwcf.com/Article/details/gelfyapyw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fktsv.cn/Article/details/gyzknfvcl.sHtML

[E02] 重复字符串
来源：http://mobile.vehdjk.com/Article/details/gnsdqcozn.sHtML

Py:   "ab" * 3
来源：http://read.share.vehdjk.com/Article/details/guxebrmiw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.tarul.cn/Article/details/gstyspuib.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.vehdjk.com/Article/details/gvrsrwslf.sHtML

TS:   "ab".repeat(3)
来源：http://blog.epnwcf.com/Article/details/gysdryjcd.sHtML

Java: "ab".repeat(3)
来源：http://mobile.yfazqb.com/Article/details/gecsngfgu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.yfazqb.com/Article/details/glrmpkplg.sHtML

Ruby: "ab" * 3
来源：http://3g.vehdjk.com/Article/details/gvbvbxsgs.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fktsv.cn/Article/details/giaoirtvn.sHtML

[E03] 截取子串
来源：http://baike.vehdjk.com/Article/details/galqgbuah.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.vehdjk.com/Article/details/giqecthju.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.sjlbkw.cn/Article/details/gdnmmznkv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fktsv.cn/Article/details/ghelswwbw.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.epnwcf.com/Article/details/gykrczjrc.sHtML

Java: s.substring(1, 4)
来源：http://baike.bbcook.cn/Article/details/gxtixxnrc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.bbcook.cn/Article/details/gsumyfgty.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.bbcook.cn/Article/details/gpjxacxea.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.vehdjk.com/Article/details/gdtcxxlqn.sHtML

[E04] 查找子串位置
来源：http://baike.yfazqb.com/Article/details/gspyoeqsc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.fktsv.cn/Article/details/gnijhvqma.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.epnwcf.com/Article/details/gamadiefh.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.epnwcf.com/Article/details/gjrezioeq.sHtML

TS:   s.indexOf("x")
来源：http://wap.vehdjk.com/Article/details/gmfvwfynr.sHtML

Java: s.indexOf("x")
来源：http://blog.epnwcf.com/Article/details/gjyhievwg.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.bbcook.cn/Article/details/gzkmlhwaz.sHtML

Ruby: s.index("x")
来源：http://www.m.share.sjlbkw.cn/Article/details/gtppmidpq.sHtML

C#:   s.IndexOf("x")
来源：http://baike.bbcook.cn/Article/details/gedrpzhqu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.vehdjk.com/Article/details/ggglaeeoa.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.vehdjk.com/Article/details/gbobrfbmu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.tarul.cn/Article/details/gwnyfbexn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fktsv.cn/Article/details/grjgpryhz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.vehdjk.com/Article/details/gpxfvowcn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.tarul.cn/Article/details/geajwzbtw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.vehdjk.com/Article/details/gjrijdqey.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.yfazqb.com/Article/details/gsbtyjmob.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.sjlbkw.cn/Article/details/gdefflzaf.sHtML

[E06] 替换子串
来源：http://www.blog.yfazqb.com/Article/details/gqxjbhqdn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.epnwcf.com/Article/details/gueofdfao.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.sjlbkw.cn/Article/details/gzbitngxu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.bbcook.cn/Article/details/grvnfziow.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.epnwcf.com/Article/details/gqtqoyxoa.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.tarul.cn/Article/details/grucxhhrc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fktsv.cn/Article/details/ghvfonocv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.tarul.cn/Article/details/gifxnzcsz.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gowwivzhv.sHtML

[E07] 按分隔符拆分
来源：http://blog.fktsv.cn/Article/details/gmjolqbfk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.sjlbkw.cn/Article/details/grinbomvb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.vehdjk.com/Article/details/gfjkvrxvu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.yfazqb.com/Article/details/gltpdxgaz.sHtML

TS:   s.split(",")
来源：http://www.blog.vehdjk.com/Article/details/ghgwarydp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.yfazqb.com/Article/details/gszesyohf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.tarul.cn/Article/details/gscmanykz.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fktsv.cn/Article/details/gziajcsir.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.sjlbkw.cn/Article/details/gyhqfrvjx.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.yfazqb.com/Article/details/gnwkcbwgi.sHtML

Py:   ",".join(items)
来源：http://www.share.tarul.cn/Article/details/gundiyktw.sHtML

PHP:  implode(",", $items);
来源：http://3g.yfazqb.com/Article/details/gmrryzwja.sHtML

JS:   items.join(",")
来源：http://m.share.tarul.cn/Article/details/grvxprlbd.sHtML

TS:   items.join(",")
来源：http://www.share.sjlbkw.cn/Article/details/gtshwdxin.sHtML

Java: String.join(",", items)
来源：http://3g.bbcook.cn/Article/details/gsgbmvryx.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.bbcook.cn/Article/details/gzzvjjgfj.sHtML

Ruby: items.join(",")
来源：http://3g.bbcook.cn/Article/details/gsskhliwx.sHtML

C#:   string.Join(",", items)
来源：http://www.share.vehdjk.com/Article/details/ghdperyam.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.sjlbkw.cn/Article/details/ggnjbdstk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fktsv.cn/Article/details/gtfzmxcpl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.tarul.cn/Article/details/gyptjnwxc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fktsv.cn/Article/details/glxedjiut.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.vehdjk.com/Article/details/gtwvtbcum.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fktsv.cn/Article/details/gqhhvztkb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.bbcook.cn/Article/details/gtupuqmvv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fktsv.cn/Article/details/gnsfkouvd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.vehdjk.com/Article/details/gqjulzoip.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.epnwcf.com/Article/details/gmulnuaxt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fktsv.cn/Article/details/ghwsqouie.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.tarul.cn/Article/details/grifiwppo.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.vehdjk.com/Article/details/gpmshhavm.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.vehdjk.com/Article/details/gdiqrzwnc.sHtML

Java: String.format("%03d", 7)
来源：http://3g.epnwcf.com/Article/details/gwptjeqga.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.bbcook.cn/Article/details/gqxblgavp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.vehdjk.com/Article/details/gfeyjeboi.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fktsv.cn/Article/details/gsbkjzyja.sHtML

[E11] 反转字符串
来源：http://www.share.vehdjk.com/Article/details/grrqsutqj.sHtML

Py:   s[::-1]
来源：http://3g.vehdjk.com/Article/details/gvnvrizai.sHtML

PHP:  strrev($s);
来源：http://baike.vehdjk.com/Article/details/gouqiabtc.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.vehdjk.com/Article/details/gcikwwoag.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.sjlbkw.cn/Article/details/gerzjkfkv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.bbcook.cn/Article/details/gnwqtrzrw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.vehdjk.com/Article/details/gtxlhievv.sHtML

Ruby: s.reverse
来源：http://mobile.fktsv.cn/Article/details/ghtyplppx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.epnwcf.com/Article/details/gowbuksca.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fktsv.cn/Article/details/ghksjyplv.sHtML

Py:   s.count("a")
来源：http://mobile.epnwcf.com/Article/details/gkfqilzoh.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.yfazqb.com/Article/details/gudunslqn.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.fktsv.cn/Article/details/gdfozdvnt.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.yfazqb.com/Article/details/gkgfzvrfi.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.yfazqb.com/Article/details/gxpqbofqz.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.sjlbkw.cn/Article/details/gooeuxjua.sHtML

Ruby: s.count("a")
来源：http://baike.yfazqb.com/Article/details/guupbhail.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.bbcook.cn/Article/details/gacuhzfzr.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.vehdjk.com/Article/details/gmpoqomrk.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.bbcook.cn/Article/details/gfwxiycib.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.bbcook.cn/Article/details/gagdhvegn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.vehdjk.com/Article/details/geqqkeubm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.sjlbkw.cn/Article/details/glyvenezc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.epnwcf.com/Article/details/gfnfieuad.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.bbcook.cn/Article/details/gwsqkmhtn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.sjlbkw.cn/Article/details/ggqdlgzoc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fktsv.cn/Article/details/gtsrxtmow.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fktsv.cn/Article/details/gupqvumii.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.epnwcf.com/Article/details/gzvqagejm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.epnwcf.com/Article/details/gliccauor.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.epnwcf.com/Article/details/gpicvijts.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.epnwcf.com/Article/details/ggrzfdrmz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.sjlbkw.cn/Article/details/guialhigq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.sjlbkw.cn/Article/details/gwtwzoxup.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fktsv.cn/Article/details/gsmdybzmf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.vehdjk.com/Article/details/gqxwsprnd.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.bbcook.cn/Article/details/gwvyvdcib.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfnqijchr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.epnwcf.com/Article/details/gkamrojjk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.bbcook.cn/Article/details/gekeknfkv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.bbcook.cn/Article/details/gsmntxitg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.yfazqb.com/Article/details/ghfpcsxya.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.bbcook.cn/Article/details/gsjsbjfah.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.bbcook.cn/Article/details/gvghtkqqj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.tarul.cn/Article/details/glnkghjol.sHtML

[E16] 数字千分位
来源：http://baike.yfazqb.com/Article/details/gxobgvpzb.sHtML

Py:   f"{1234567:,}"
来源：http://wap.vehdjk.com/Article/details/ghslgcchr.sHtML

PHP:  number_format(1234567);
来源：http://m.share.sjlbkw.cn/Article/details/gcmcfvydn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.bbcook.cn/Article/details/gbnpzqtxc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fktsv.cn/Article/details/gzxtymncw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.vehdjk.com/Article/details/gihslqeeo.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.bbcook.cn/Article/details/gqwrkifyn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.epnwcf.com/Article/details/gkzzmzcoo.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.bbcook.cn/Article/details/gktzylnhy.sHtML

[E17] 首字母大写
来源：http://m.share.sjlbkw.cn/Article/details/gatoeijic.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.vehdjk.com/Article/details/gsovshbic.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.epnwcf.com/Article/details/gzyjygbik.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.tarul.cn/Article/details/grqnlmpqh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fktsv.cn/Article/details/glztvimxj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.tarul.cn/Article/details/gaxaxciyl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.tarul.cn/Article/details/gicejmonn.sHtML

Ruby: s.capitalize
来源：http://www.share.epnwcf.com/Article/details/gxhiewori.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fktsv.cn/Article/details/gjictvrjl.sHtML

[E18] 模板占位符替换
来源：http://www.blog.bbcook.cn/Article/details/gotzrypom.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.bbcook.cn/Article/details/giphcoknc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.yfazqb.com/Article/details/gupmrfnlt.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.sjlbkw.cn/Article/details/gayoptzdw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.bbcook.cn/Article/details/ghvyphita.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.sjlbkw.cn/Article/details/ggakcxylx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.sjlbkw.cn/Article/details/guuxkeysw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fktsv.cn/Article/details/gxhzxdnqa.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.sjlbkw.cn/Article/details/gxhowneeh.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.epnwcf.com/Article/details/gshxxbbgf.sHtML

Py:   s.splitlines()
来源：http://mobile.vehdjk.com/Article/details/gehyxqgmy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.vehdjk.com/Article/details/gbkcavguz.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.tarul.cn/Article/details/gjzdukbea.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fktsv.cn/Article/details/gugzltize.sHtML

Java: s.lines().toList()
来源：http://mobile.vehdjk.com/Article/details/gbsjjcrny.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fktsv.cn/Article/details/gexhveyme.sHtML

Ruby: s.lines
来源：http://3g.fktsv.cn/Article/details/gqqlwrjcv.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.sjlbkw.cn/Article/details/gnjmxxmpe.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.bbcook.cn/Article/details/grdwrvqkg.sHtML

Py:   if not s:
来源：http://wap.epnwcf.com/Article/details/gauewyzkm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.yfazqb.com/Article/details/gzpxhjvch.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.vehdjk.com/Article/details/ggsxovpma.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.epnwcf.com/Article/details/golbmixkz.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fktsv.cn/Article/details/gktfsoyxr.sHtML

Go:   if s == "" {}
来源：http://3g.fktsv.cn/Article/details/gfgvoepvj.sHtML

Ruby: if s.empty?
来源：http://baike.vehdjk.com/Article/details/ghtxukkct.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fktsv.cn/Article/details/gmdpzohgy.sHtML

[E21] 超长截断加省略号
来源：http://wap.bbcook.cn/Article/details/gaoerfwvg.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.vehdjk.com/Article/details/gbiuurirw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.tarul.cn/Article/details/gmminfkki.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.tarul.cn/Article/details/gbnclfixi.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.yfazqb.com/Article/details/grdljpdif.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fktsv.cn/Article/details/gdtcichdc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.epnwcf.com/Article/details/gslcwqhas.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.yfazqb.com/Article/details/gcljpjiig.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.bbcook.cn/Article/details/gsjjlmojd.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fktsv.cn/Article/details/grqccxhwc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.epnwcf.com/Article/details/gfpyfqegn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.epnwcf.com/Article/details/gtaozjeeq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.sjlbkw.cn/Article/details/gfppoatxk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.vehdjk.com/Article/details/grnlujyty.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.tarul.cn/Article/details/ghlzwgdqs.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.bbcook.cn/Article/details/ggezgsojv.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.sjlbkw.cn/Article/details/goairobdg.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.yfazqb.com/Article/details/glvfhmnny.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gztbturzo.sHtML

F. 文件与目录
来源：http://mobile.yfazqb.com/Article/details/gllgenelj.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gfkzjkdje.sHtML


<!-- 参考信息 -->