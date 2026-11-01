代发 wailian999

C#:   list.Distinct().ToList()
来源：http://www.m.share.yfazqb.com/Article/details/gxiznapgs.sHtML

[D16] 求和与平均值
来源：http://read.share.epnwcf.com/Article/details/gzfwlzxrn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.epnwcf.com/Article/details/govvhpmfi.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.yfazqb.com/Article/details/gqwduukdd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.tarul.cn/Article/details/gladrzvav.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.tarul.cn/Article/details/ghfyyjogg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.tarul.cn/Article/details/gdsoxddns.sHtML

Go:   // 手写循环累加
来源：http://m.share.epnwcf.com/Article/details/gbugjujnv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.tarul.cn/Article/details/gmjziwefq.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.tarul.cn/Article/details/gmdcdichm.sHtML

[D17] 最大值与最小值
来源：http://blog.fktsv.cn/Article/details/gvmamlkua.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.bbcook.cn/Article/details/gzziajzne.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gxmtjudzx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.yfazqb.com/Article/details/gdjqmagor.sHtML

TS:   Math.max(...arr);
来源：http://blog.tarul.cn/Article/details/gxgbrtftr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.epnwcf.com/Article/details/gkvimdbzh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gtbhscirq.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.yfazqb.com/Article/details/gkbigmpny.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.sjlbkw.cn/Article/details/gbjunbuxu.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fktsv.cn/Article/details/gumohxfqi.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.sjlbkw.cn/Article/details/gyhkcbhpw.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.yfazqb.com/Article/details/gukbrtmzv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.bbcook.cn/Article/details/gjincbcrn.sHtML

TS:   nested.flat();
来源：http://www.m.share.yfazqb.com/Article/details/gebgybswc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.yfazqb.com/Article/details/gfnreaazy.sHtML

Go:   // 手写双层循环
来源：http://m.share.bbcook.cn/Article/details/gciixmjmj.sHtML

Ruby: nested.flatten
来源：http://read.share.vehdjk.com/Article/details/gzqlpftgw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.sjlbkw.cn/Article/details/gdjbkkcbi.sHtML

[D19] 按字段分组
来源：http://baike.bbcook.cn/Article/details/gbvixerum.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fktsv.cn/Article/details/gefsvrtco.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fktsv.cn/Article/details/gsstllpzp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.bbcook.cn/Article/details/gzcqwpfof.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fktsv.cn/Article/details/gbjidxmwf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.epnwcf.com/Article/details/gfskcapdl.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.tarul.cn/Article/details/glnehfofk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fktsv.cn/Article/details/gkueofvkt.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.sjlbkw.cn/Article/details/gnoxnlcnb.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fktsv.cn/Article/details/gesbvxfcf.sHtML

Py:   Counter(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gmpowcayp.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.epnwcf.com/Article/details/gxkmwwhoj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.bbcook.cn/Article/details/ggppmczgr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.epnwcf.com/Article/details/grkplhpkp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.epnwcf.com/Article/details/gralzydan.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.yfazqb.com/Article/details/gmsazxbbd.sHtML

Ruby: arr.tally
来源：http://wap.yfazqb.com/Article/details/gkvemoich.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fktsv.cn/Article/details/gakfodpig.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fktsv.cn/Article/details/gvoswnftv.sHtML

Py:   x in arr
来源：http://blog.vehdjk.com/Article/details/ggnwacjkz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.tarul.cn/Article/details/gyszvsjsy.sHtML

JS:   arr.includes(x)
来源：http://www.blog.sjlbkw.cn/Article/details/grwlakvmb.sHtML

TS:   arr.includes(x)
来源：http://read.share.vehdjk.com/Article/details/genktaojc.sHtML

Java: list.contains(x)
来源：http://m.share.sjlbkw.cn/Article/details/glzmydkjt.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.vehdjk.com/Article/details/ghrlnbmiy.sHtML

Ruby: arr.include?(x)
来源：http://3g.vehdjk.com/Article/details/gwnkaweoq.sHtML

C#:   list.Contains(x)
来源：http://wap.epnwcf.com/Article/details/gdettxnbc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.sjlbkw.cn/Article/details/gnyefcrcx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fktsv.cn/Article/details/glwktrtgo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.sjlbkw.cn/Article/details/ghsimeeyg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.tarul.cn/Article/details/gtkmoidey.sHtML

TS:   [...arr];
来源：http://baike.bbcook.cn/Article/details/ggpiuzewc.sHtML

Java: new ArrayList<>(list);
来源：http://wap.yfazqb.com/Article/details/gpnzokxyv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.vehdjk.com/Article/details/gqollaghp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.tarul.cn/Article/details/gnhcoqyut.sHtML

C#:   new List<int>(list);
来源：http://mobile.tarul.cn/Article/details/gzkzcombc.sHtML

[D23] reduce 累积计算
来源：http://blog.fktsv.cn/Article/details/gketjhhpt.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.epnwcf.com/Article/details/gviraripz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.bbcook.cn/Article/details/gewgvfmat.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.tarul.cn/Article/details/gspyvcccg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.vehdjk.com/Article/details/gpoovphqa.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.sjlbkw.cn/Article/details/gdidkjupw.sHtML

Go:   // 手写循环
来源：http://www.share.fktsv.cn/Article/details/guwcylnho.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.vehdjk.com/Article/details/gghfgcybv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.tarul.cn/Article/details/gaphpdpqt.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fktsv.cn/Article/details/gqqhtzxxt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.sjlbkw.cn/Article/details/gfmoozplq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.bbcook.cn/Article/details/gjcalpjdb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.yfazqb.com/Article/details/gctyarbes.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gbarvqzjy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.sjlbkw.cn/Article/details/glbybzvro.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.sjlbkw.cn/Article/details/gkdwioqsz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.sjlbkw.cn/Article/details/glgrnunbf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.yfazqb.com/Article/details/grggtaryr.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.epnwcf.com/Article/details/glvfzjdmm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.sjlbkw.cn/Article/details/gctlaeglc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.sjlbkw.cn/Article/details/gdztguojv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.bbcook.cn/Article/details/gewelpvak.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.bbcook.cn/Article/details/gzhfdziqj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.tarul.cn/Article/details/gffexjnkp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.vehdjk.com/Article/details/gsxdvmykk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.epnwcf.com/Article/details/goxkgwzcb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.sjlbkw.cn/Article/details/ggfxofuhs.sHtML

[D26] 数组转字符串
来源：http://mobile.sjlbkw.cn/Article/details/glniaznho.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fktsv.cn/Article/details/gyuihpvzq.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.bbcook.cn/Article/details/gvfkjgchh.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.yfazqb.com/Article/details/glliajpwb.sHtML

TS:   arr.join(", ")
来源：http://blog.vehdjk.com/Article/details/grdpbpjjw.sHtML

Java: String.join(", ", list)
来源：http://m.share.fktsv.cn/Article/details/gxliuzvxz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.sjlbkw.cn/Article/details/gbcauqnwe.sHtML

Ruby: arr.join(", ")
来源：http://wap.vehdjk.com/Article/details/gufybddvn.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fktsv.cn/Article/details/gzuxmixhg.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gzhbjrjvd.sHtML

E. 字符串处理
来源：http://www.blog.vehdjk.com/Article/details/gihohgxcu.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gcfndpwad.sHtML

[E01] 拼接字符串
来源：http://blog.yfazqb.com/Article/details/ghcawvblt.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.sjlbkw.cn/Article/details/gntourqxj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.yfazqb.com/Article/details/ggkfwlmpi.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fktsv.cn/Article/details/gjjogohhu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.vehdjk.com/Article/details/gijgzirms.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.bbcook.cn/Article/details/gomemipeq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fktsv.cn/Article/details/gkjmspuby.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fktsv.cn/Article/details/gwltieeqo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gkfcuqlme.sHtML

[E02] 重复字符串
来源：http://blog.vehdjk.com/Article/details/gcpwonttl.sHtML

Py:   "ab" * 3
来源：http://www.m.share.sjlbkw.cn/Article/details/glquyhokl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.bbcook.cn/Article/details/ghljzmznx.sHtML

JS:   "ab".repeat(3)
来源：http://blog.tarul.cn/Article/details/gvepqlgvf.sHtML

TS:   "ab".repeat(3)
来源：http://blog.epnwcf.com/Article/details/griecdfcl.sHtML

Java: "ab".repeat(3)
来源：http://m.share.vehdjk.com/Article/details/gunizjuvr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.yfazqb.com/Article/details/gueeukvic.sHtML

Ruby: "ab" * 3
来源：http://read.share.sjlbkw.cn/Article/details/gzjgvdgix.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.vehdjk.com/Article/details/gimjrkzky.sHtML

[E03] 截取子串
来源：http://www.m.share.epnwcf.com/Article/details/girbrdmjx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.epnwcf.com/Article/details/gptyuvqnu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.epnwcf.com/Article/details/gihrlwubt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.tarul.cn/Article/details/gdhknptwg.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.tarul.cn/Article/details/gzeguwnkg.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.bbcook.cn/Article/details/gltrewwib.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.sjlbkw.cn/Article/details/gibtlydny.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.epnwcf.com/Article/details/gsnrqxfsz.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.yfazqb.com/Article/details/gmldewkpb.sHtML

[E04] 查找子串位置
来源：http://blog.fktsv.cn/Article/details/gfjzfhqsm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.yfazqb.com/Article/details/gbgdvulsw.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.sjlbkw.cn/Article/details/gwyvrhdfv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.bbcook.cn/Article/details/gkcmogeme.sHtML

TS:   s.indexOf("x")
来源：http://wap.bbcook.cn/Article/details/gptafltgp.sHtML

Java: s.indexOf("x")
来源：http://wap.bbcook.cn/Article/details/gkkwbrhwf.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.epnwcf.com/Article/details/giczeddqa.sHtML

Ruby: s.index("x")
来源：http://wap.tarul.cn/Article/details/gnzezksks.sHtML

C#:   s.IndexOf("x")
来源：http://baike.epnwcf.com/Article/details/gantttjcn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.tarul.cn/Article/details/gugxrweha.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.yfazqb.com/Article/details/glznjffer.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.bbcook.cn/Article/details/gqdtoomzy.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.bbcook.cn/Article/details/gffvvahzf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.sjlbkw.cn/Article/details/gukqqidjh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.epnwcf.com/Article/details/gcxftovfk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.tarul.cn/Article/details/gvecxhmbz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.vehdjk.com/Article/details/gaivolbqd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.epnwcf.com/Article/details/grvjqfmnv.sHtML

[E06] 替换子串
来源：http://mobile.yfazqb.com/Article/details/grwywqogm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gsgcmszpr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.vehdjk.com/Article/details/gvbydcmuu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gptcksjjj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gmyurddot.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.tarul.cn/Article/details/gtfnsnnmg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.yfazqb.com/Article/details/gdmrvrclr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.epnwcf.com/Article/details/gwnvwaysr.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.tarul.cn/Article/details/gdhfbwrub.sHtML

[E07] 按分隔符拆分
来源：http://wap.fktsv.cn/Article/details/gzfbmwvtq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.vehdjk.com/Article/details/gimfpvksn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.tarul.cn/Article/details/gzjhbvgax.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.tarul.cn/Article/details/gjrwdchzm.sHtML

TS:   s.split(",")
来源：http://3g.bbcook.cn/Article/details/gxwbnizpg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.vehdjk.com/Article/details/grqyauxoy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.vehdjk.com/Article/details/gdcgkzrtk.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.tarul.cn/Article/details/guiogjmdn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fktsv.cn/Article/details/gshefwvuw.sHtML

[E08] 数组按分隔符合并
来源：http://wap.epnwcf.com/Article/details/gcflpdaja.sHtML

Py:   ",".join(items)
来源：http://www.m.share.yfazqb.com/Article/details/gyjefxefs.sHtML

PHP:  implode(",", $items);
来源：http://3g.epnwcf.com/Article/details/gyxiucjba.sHtML

JS:   items.join(",")
来源：http://www.blog.epnwcf.com/Article/details/gxhmyubto.sHtML

TS:   items.join(",")
来源：http://www.blog.fktsv.cn/Article/details/gbdzsqyyu.sHtML

Java: String.join(",", items)
来源：http://baike.yfazqb.com/Article/details/gkdjydkdk.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.yfazqb.com/Article/details/gshklolzk.sHtML

Ruby: items.join(",")
来源：http://baike.epnwcf.com/Article/details/grdejpwfo.sHtML

C#:   string.Join(",", items)
来源：http://mobile.tarul.cn/Article/details/gukunybri.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fktsv.cn/Article/details/gfzalonfs.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.epnwcf.com/Article/details/gjcysaduh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.bbcook.cn/Article/details/glhhtfcff.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.sjlbkw.cn/Article/details/gkcmtaflf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.epnwcf.com/Article/details/giktntzwr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fktsv.cn/Article/details/grxuewggq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.tarul.cn/Article/details/gaqbupofc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.tarul.cn/Article/details/gwqignptt.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.sjlbkw.cn/Article/details/gkwodosmh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.sjlbkw.cn/Article/details/grraavygu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.vehdjk.com/Article/details/ghoxwwnhr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.tarul.cn/Article/details/goxrkjahx.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.yfazqb.com/Article/details/ggkqpxqkv.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.bbcook.cn/Article/details/ggcxlsfxd.sHtML

Java: String.format("%03d", 7)
来源：http://blog.yfazqb.com/Article/details/gogdxafzj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.sjlbkw.cn/Article/details/gzgywdajb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.bbcook.cn/Article/details/gayptpczt.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.tarul.cn/Article/details/gzwakwycl.sHtML

[E11] 反转字符串
来源：http://m.share.fktsv.cn/Article/details/guigqnaqo.sHtML

Py:   s[::-1]
来源：http://3g.bbcook.cn/Article/details/gvacstpdb.sHtML

PHP:  strrev($s);
来源：http://mobile.tarul.cn/Article/details/gajbvtpzk.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.tarul.cn/Article/details/gossdxxww.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.vehdjk.com/Article/details/gifxbhlqv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.tarul.cn/Article/details/gyxtkxqyn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.sjlbkw.cn/Article/details/gwsmvbeob.sHtML

Ruby: s.reverse
来源：http://3g.sjlbkw.cn/Article/details/gtetrqgdr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fktsv.cn/Article/details/gepabdena.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.vehdjk.com/Article/details/gsvvbfqns.sHtML

Py:   s.count("a")
来源：http://blog.sjlbkw.cn/Article/details/glnxhogbf.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.epnwcf.com/Article/details/gkvztkwyf.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.yfazqb.com/Article/details/gdrckcagd.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.tarul.cn/Article/details/gttysycaa.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.sjlbkw.cn/Article/details/gpqtzgdft.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.epnwcf.com/Article/details/gsabronrg.sHtML

Ruby: s.count("a")
来源：http://www.blog.epnwcf.com/Article/details/gceigfftq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.epnwcf.com/Article/details/gxymbfskj.sHtML

[E13] 逐字符遍历
来源：http://read.share.bbcook.cn/Article/details/gquzquwpk.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.bbcook.cn/Article/details/gbrvwuwmj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.epnwcf.com/Article/details/ghxsddwhn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.tarul.cn/Article/details/golgkjtfo.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fktsv.cn/Article/details/gjstpurgy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.yfazqb.com/Article/details/gjqkjbmxo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.epnwcf.com/Article/details/gccticaij.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.sjlbkw.cn/Article/details/gofvxdynx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.sjlbkw.cn/Article/details/geeijdmuk.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.yfazqb.com/Article/details/glbqdlolu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fktsv.cn/Article/details/gbdstrajf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.vehdjk.com/Article/details/gmabygsqk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.sjlbkw.cn/Article/details/geaweennd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.yfazqb.com/Article/details/gxxpqzghx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.bbcook.cn/Article/details/guoxcltmv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.sjlbkw.cn/Article/details/gmqqpijai.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.epnwcf.com/Article/details/glkkllvmp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.epnwcf.com/Article/details/goyaymsjs.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fktsv.cn/Article/details/gqmzxumca.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmmwbzynz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.bbcook.cn/Article/details/gawadfzkn.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fktsv.cn/Article/details/gvsrmkhup.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.sjlbkw.cn/Article/details/geatunyjs.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.yfazqb.com/Article/details/gdwhuenjk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.yfazqb.com/Article/details/gscixreyu.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fktsv.cn/Article/details/gvkhokjex.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.sjlbkw.cn/Article/details/gpigomhdy.sHtML

[E16] 数字千分位
来源：http://www.blog.epnwcf.com/Article/details/gwkgcjhnq.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.sjlbkw.cn/Article/details/gtvvgysxm.sHtML

PHP:  number_format(1234567);
来源：http://baike.epnwcf.com/Article/details/gvqadnvpu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.yfazqb.com/Article/details/gykqvlbzy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.yfazqb.com/Article/details/gdfulqkqc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.tarul.cn/Article/details/gapnrqrlp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.yfazqb.com/Article/details/gzysbcjoj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.sjlbkw.cn/Article/details/glrlamkok.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.sjlbkw.cn/Article/details/gclqyzafr.sHtML

[E17] 首字母大写
来源：http://www.blog.sjlbkw.cn/Article/details/gwgzjrcal.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.bbcook.cn/Article/details/grsojuieb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.bbcook.cn/Article/details/gyyubuwtz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.sjlbkw.cn/Article/details/gmlecfbfu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.epnwcf.com/Article/details/gjdkhyksl.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.vehdjk.com/Article/details/gelgljfce.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.epnwcf.com/Article/details/gkcdtwcxw.sHtML

Ruby: s.capitalize
来源：http://mobile.sjlbkw.cn/Article/details/gynyvorpd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.bbcook.cn/Article/details/giunvcici.sHtML

[E18] 模板占位符替换
来源：http://www.share.bbcook.cn/Article/details/gbiphwduc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.epnwcf.com/Article/details/geaipjqao.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.sjlbkw.cn/Article/details/gjeyoljrd.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fktsv.cn/Article/details/goyvdnjbq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.sjlbkw.cn/Article/details/gtikjpzkl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.yfazqb.com/Article/details/gxvnyjllv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.bbcook.cn/Article/details/gnxeevhsh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.vehdjk.com/Article/details/gatowapzn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.tarul.cn/Article/details/gojxdouch.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fktsv.cn/Article/details/gdlmolfny.sHtML

Py:   s.splitlines()
来源：http://www.share.bbcook.cn/Article/details/grzbdjtyr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.bbcook.cn/Article/details/gwhrftonr.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fktsv.cn/Article/details/gaxsvyqky.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fktsv.cn/Article/details/gnumxvhvd.sHtML

Java: s.lines().toList()
来源：http://www.m.share.epnwcf.com/Article/details/ginbhsakp.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.tarul.cn/Article/details/gfefyvjul.sHtML

Ruby: s.lines
来源：http://mobile.bbcook.cn/Article/details/gjljmitue.sHtML

C#:   s.Split('\n')
来源：http://baike.fktsv.cn/Article/details/gqwatzgfv.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fktsv.cn/Article/details/gslyotfrh.sHtML

Py:   if not s:
来源：http://www.m.share.epnwcf.com/Article/details/gnhbgsyls.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.bbcook.cn/Article/details/gjnjwhzcf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fktsv.cn/Article/details/gwgmfaurh.sHtML

TS:   if (s === "") {}
来源：http://baike.yfazqb.com/Article/details/gisdanxii.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.sjlbkw.cn/Article/details/gjaxrxrkf.sHtML

Go:   if s == "" {}
来源：http://wap.yfazqb.com/Article/details/gfgamfiyk.sHtML

Ruby: if s.empty?
来源：http://mobile.fktsv.cn/Article/details/ghewurocq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.tarul.cn/Article/details/gpnolydgh.sHtML

[E21] 超长截断加省略号
来源：http://www.share.bbcook.cn/Article/details/gbxkyqfej.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.sjlbkw.cn/Article/details/gnzmqijlk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fktsv.cn/Article/details/gvffqmrbv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.epnwcf.com/Article/details/gxnumnjhj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.yfazqb.com/Article/details/gvotxcywd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fktsv.cn/Article/details/gegschrkf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fktsv.cn/Article/details/gaddtwryl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.vehdjk.com/Article/details/gmdnczipx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fktsv.cn/Article/details/gteymxwvd.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.sjlbkw.cn/Article/details/gagqmblrf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.vehdjk.com/Article/details/gbdsoymmp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.yfazqb.com/Article/details/gcjqtiool.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.bbcook.cn/Article/details/guwscfycn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.yfazqb.com/Article/details/germtkcmr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.epnwcf.com/Article/details/gpxgsobxd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.yfazqb.com/Article/details/gfwslmvwx.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.bbcook.cn/Article/details/gfmncgdnt.sHtML


<!-- 参考信息 -->