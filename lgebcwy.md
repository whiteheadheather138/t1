代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.bbcook.cn/Article/details/gvoxhytue.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.yfazqb.com/Article/details/gymnkfxek.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.sjlbkw.cn/Article/details/gftzsljop.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.tarul.cn/Article/details/gzaxvewpa.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fktsv.cn/Article/details/goynrfplk.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fktsv.cn/Article/details/gftagrlfr.sHtML

Py:   Counter(arr)
来源：http://wap.bbcook.cn/Article/details/gcqcsicih.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.tarul.cn/Article/details/gcvfmkovi.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.tarul.cn/Article/details/gqajatxnd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fktsv.cn/Article/details/gmiwwpnjr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fktsv.cn/Article/details/ggydemknv.sHtML

Go:   // 手写 map[T]int
来源：http://blog.vehdjk.com/Article/details/gtxcnqlhp.sHtML

Ruby: arr.tally
来源：http://www.blog.tarul.cn/Article/details/govvvenae.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.bbcook.cn/Article/details/gdalafddz.sHtML

[D21] 判断是否包含某元素
来源：http://blog.vehdjk.com/Article/details/gwjkogspv.sHtML

Py:   x in arr
来源：http://blog.bbcook.cn/Article/details/gfcqpoiau.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.epnwcf.com/Article/details/ggeznhcca.sHtML

JS:   arr.includes(x)
来源：http://m.share.sjlbkw.cn/Article/details/gcpeksyoa.sHtML

TS:   arr.includes(x)
来源：http://3g.fktsv.cn/Article/details/geakayzrt.sHtML

Java: list.contains(x)
来源：http://www.blog.fktsv.cn/Article/details/ghlnkqpww.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gptvjzzev.sHtML

Ruby: arr.include?(x)
来源：http://wap.epnwcf.com/Article/details/ggkyxydnn.sHtML

C#:   list.Contains(x)
来源：http://3g.sjlbkw.cn/Article/details/gqqbpwrlk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.yfazqb.com/Article/details/gktmfgwfj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.bbcook.cn/Article/details/gczlascud.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.vehdjk.com/Article/details/gtnvvykzc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.vehdjk.com/Article/details/gfnzujujm.sHtML

TS:   [...arr];
来源：http://mobile.bbcook.cn/Article/details/gqksfayix.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fktsv.cn/Article/details/gpbmxfzjv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.tarul.cn/Article/details/gzegmzbnp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.bbcook.cn/Article/details/gncoutdea.sHtML

C#:   new List<int>(list);
来源：http://read.share.epnwcf.com/Article/details/gfrqagxcf.sHtML

[D23] reduce 累积计算
来源：http://wap.bbcook.cn/Article/details/gatmbjvmi.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fktsv.cn/Article/details/gpzaxyomu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fktsv.cn/Article/details/gixzcxjug.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.bbcook.cn/Article/details/ggtvqkkbi.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.tarul.cn/Article/details/gzscxycle.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.bbcook.cn/Article/details/guicvjcid.sHtML

Go:   // 手写循环
来源：http://www.blog.epnwcf.com/Article/details/guqpavdlh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.bbcook.cn/Article/details/gthwghbvw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.tarul.cn/Article/details/gsglajsau.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.vehdjk.com/Article/details/gmbvadkim.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.sjlbkw.cn/Article/details/gavgadqti.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.tarul.cn/Article/details/gyodtrtcq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fktsv.cn/Article/details/gjvrqfqhp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gludrmelx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fktsv.cn/Article/details/gaxrrrfeb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.tarul.cn/Article/details/gbzqxxgyp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.sjlbkw.cn/Article/details/gquhwykrb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.sjlbkw.cn/Article/details/grruizrzb.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.vehdjk.com/Article/details/gdjjqsejo.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.bbcook.cn/Article/details/gepgqzajv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.bbcook.cn/Article/details/gllhwagkl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fktsv.cn/Article/details/gfsbmslwe.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.bbcook.cn/Article/details/gyhzgjldv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.vehdjk.com/Article/details/gkhogfbbx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.tarul.cn/Article/details/gbagxzprh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.sjlbkw.cn/Article/details/gvosqukuj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fktsv.cn/Article/details/gjmjckdwd.sHtML

[D26] 数组转字符串
来源：http://3g.vehdjk.com/Article/details/gfmjqvslz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.sjlbkw.cn/Article/details/glgiibkwv.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.sjlbkw.cn/Article/details/gujklbpwx.sHtML

JS:   arr.join(", ")
来源：http://read.share.fktsv.cn/Article/details/ggrcaikiq.sHtML

TS:   arr.join(", ")
来源：http://wap.tarul.cn/Article/details/gepesacfr.sHtML

Java: String.join(", ", list)
来源：http://baike.yfazqb.com/Article/details/gvuzgwxpi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fktsv.cn/Article/details/gwzqjjhws.sHtML

Ruby: arr.join(", ")
来源：http://baike.vehdjk.com/Article/details/gejxpmfoc.sHtML

C#:   string.Join(", ", list)
来源：http://blog.epnwcf.com/Article/details/gszcwdzxh.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/giqegfsih.sHtML

E. 字符串处理
来源：http://www.blog.yfazqb.com/Article/details/gkciqljca.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gjesqecnl.sHtML

[E01] 拼接字符串
来源：http://baike.vehdjk.com/Article/details/glpykomcb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fktsv.cn/Article/details/gxostptgu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fktsv.cn/Article/details/gjocdwssw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fktsv.cn/Article/details/gbyrlnnrn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.bbcook.cn/Article/details/gvyzswzvf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.sjlbkw.cn/Article/details/gguprikyb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.sjlbkw.cn/Article/details/glzpjfgdw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.tarul.cn/Article/details/gvmmvtvig.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gsdzsyhtm.sHtML

[E02] 重复字符串
来源：http://m.share.vehdjk.com/Article/details/gtutukgtc.sHtML

Py:   "ab" * 3
来源：http://www.m.share.sjlbkw.cn/Article/details/gtcusswkl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.sjlbkw.cn/Article/details/grzjbwkkt.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.epnwcf.com/Article/details/gggvtnibk.sHtML

TS:   "ab".repeat(3)
来源：http://wap.vehdjk.com/Article/details/geitjzhox.sHtML

Java: "ab".repeat(3)
来源：http://read.share.sjlbkw.cn/Article/details/gajaehswb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.vehdjk.com/Article/details/gubyelbly.sHtML

Ruby: "ab" * 3
来源：http://baike.yfazqb.com/Article/details/gmeiuhowi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fktsv.cn/Article/details/gyhgbfmmg.sHtML

[E03] 截取子串
来源：http://m.share.epnwcf.com/Article/details/gwzakvljk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.fktsv.cn/Article/details/gqppfbniu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.vehdjk.com/Article/details/gubxwnlmy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fktsv.cn/Article/details/gylhirvam.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.vehdjk.com/Article/details/gsokghyxc.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fktsv.cn/Article/details/gutqmxdic.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.tarul.cn/Article/details/gnpqgklit.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fktsv.cn/Article/details/gsjyrctim.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.sjlbkw.cn/Article/details/gblljjfoy.sHtML

[E04] 查找子串位置
来源：http://m.share.vehdjk.com/Article/details/gmskmcxxx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.tarul.cn/Article/details/ghkdbginv.sHtML

PHP:  strpos($s, "x");
来源：http://3g.yfazqb.com/Article/details/gxdofrdff.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.tarul.cn/Article/details/gjlhnqatk.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.vehdjk.com/Article/details/gvycaqrra.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fktsv.cn/Article/details/gajfbkdio.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.tarul.cn/Article/details/gsowaorpj.sHtML

Ruby: s.index("x")
来源：http://m.share.epnwcf.com/Article/details/grqiclfhk.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fktsv.cn/Article/details/gfedjguyw.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.sjlbkw.cn/Article/details/grznbivcs.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.yfazqb.com/Article/details/glkvjbxos.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.vehdjk.com/Article/details/gpqqlzuht.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.yfazqb.com/Article/details/gtthmucli.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.fktsv.cn/Article/details/gisvhhzbh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.bbcook.cn/Article/details/gxkakkthz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.yfazqb.com/Article/details/gjsndvnsh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.bbcook.cn/Article/details/gkzeuvkhn.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.vehdjk.com/Article/details/gtwzbffku.sHtML

[E06] 替换子串
来源：http://www.blog.yfazqb.com/Article/details/gqjrqtxhz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.bbcook.cn/Article/details/gotwttahx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.vehdjk.com/Article/details/gsoatolor.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/gnbdgrlgj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gsgqokqgy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.vehdjk.com/Article/details/gcqlggydl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.sjlbkw.cn/Article/details/gejdyymkv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.vehdjk.com/Article/details/ggnmtbwwn.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/grwblrfex.sHtML

[E07] 按分隔符拆分
来源：http://3g.tarul.cn/Article/details/gmkagmnhh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fktsv.cn/Article/details/gkwcuhwcs.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fktsv.cn/Article/details/glxdyievs.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.epnwcf.com/Article/details/gsoknlqqd.sHtML

TS:   s.split(",")
来源：http://www.share.fktsv.cn/Article/details/gykoxzvfz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.bbcook.cn/Article/details/ghcdfujfy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.sjlbkw.cn/Article/details/gtljbmbmv.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.epnwcf.com/Article/details/gatpfibrp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.epnwcf.com/Article/details/gjjtakats.sHtML

[E08] 数组按分隔符合并
来源：http://blog.tarul.cn/Article/details/gcphmkyvq.sHtML

Py:   ",".join(items)
来源：http://m.share.bbcook.cn/Article/details/gwqvvqyoe.sHtML

PHP:  implode(",", $items);
来源：http://read.share.vehdjk.com/Article/details/gwznpuycx.sHtML

JS:   items.join(",")
来源：http://blog.epnwcf.com/Article/details/glbifvlff.sHtML

TS:   items.join(",")
来源：http://3g.sjlbkw.cn/Article/details/gfbpykxrd.sHtML

Java: String.join(",", items)
来源：http://www.share.tarul.cn/Article/details/ggennlait.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.vehdjk.com/Article/details/gaqlbgbqp.sHtML

Ruby: items.join(",")
来源：http://wap.bbcook.cn/Article/details/grvcvzxcq.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.tarul.cn/Article/details/gcjzwtvwr.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fktsv.cn/Article/details/gtydfqdgv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.epnwcf.com/Article/details/ggzktslbu.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.vehdjk.com/Article/details/gikkbtolg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.bbcook.cn/Article/details/gqegnhlye.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.bbcook.cn/Article/details/gogeouecg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.yfazqb.com/Article/details/goufsolgh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.vehdjk.com/Article/details/gxvdfgpfl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.epnwcf.com/Article/details/gopewuelv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.bbcook.cn/Article/details/gwbbmyljo.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.sjlbkw.cn/Article/details/gkuryaidl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.bbcook.cn/Article/details/gfxrqncni.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.yfazqb.com/Article/details/gkkltiaff.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.epnwcf.com/Article/details/gsclljjfs.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fktsv.cn/Article/details/gnuyxjdlv.sHtML

Java: String.format("%03d", 7)
来源：http://blog.bbcook.cn/Article/details/gafusunmd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.yfazqb.com/Article/details/gwzznjcuc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.yfazqb.com/Article/details/guurmduqu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.bbcook.cn/Article/details/gnapuldvd.sHtML

[E11] 反转字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gclhpydwq.sHtML

Py:   s[::-1]
来源：http://baike.fktsv.cn/Article/details/gtrzhnmnk.sHtML

PHP:  strrev($s);
来源：http://wap.yfazqb.com/Article/details/gtjgotdmw.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.yfazqb.com/Article/details/gyraatpge.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/gbwazpzco.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.sjlbkw.cn/Article/details/gvmeykngc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fktsv.cn/Article/details/grufkcydx.sHtML

Ruby: s.reverse
来源：http://www.m.share.sjlbkw.cn/Article/details/gutibcgbe.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.bbcook.cn/Article/details/gkzdzkdvn.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.bbcook.cn/Article/details/grgavnwmc.sHtML

Py:   s.count("a")
来源：http://www.blog.yfazqb.com/Article/details/getphybjg.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.epnwcf.com/Article/details/gpzvzbfnu.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.epnwcf.com/Article/details/gxruhnxmq.sHtML

TS:   s.split("a").length - 1
来源：http://baike.tarul.cn/Article/details/gvcxkhvpw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.epnwcf.com/Article/details/gmazxftij.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.yfazqb.com/Article/details/gicsafbcp.sHtML

Ruby: s.count("a")
来源：http://wap.yfazqb.com/Article/details/gfcszbxsh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.vehdjk.com/Article/details/gbihhpjru.sHtML

[E13] 逐字符遍历
来源：http://m.share.yfazqb.com/Article/details/gunvlhhji.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fktsv.cn/Article/details/geurynmyw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.epnwcf.com/Article/details/gsjwjaado.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.yfazqb.com/Article/details/guieynier.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.tarul.cn/Article/details/gmkptothf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.bbcook.cn/Article/details/gzohfqghi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.yfazqb.com/Article/details/gljsrdeha.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fktsv.cn/Article/details/gogczmheq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.epnwcf.com/Article/details/ggrlzdisc.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.bbcook.cn/Article/details/gegvmwjuw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.bbcook.cn/Article/details/geroinren.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.sjlbkw.cn/Article/details/gwvhzhlhr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.yfazqb.com/Article/details/gpftunpxv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.vehdjk.com/Article/details/gpbrjqvhn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.epnwcf.com/Article/details/gjrcsrvxt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.bbcook.cn/Article/details/glfutvcep.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.bbcook.cn/Article/details/gjnzhtgai.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.epnwcf.com/Article/details/gmhuctgqe.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.fktsv.cn/Article/details/gtwrerrpf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.yfazqb.com/Article/details/gejkdilya.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.sjlbkw.cn/Article/details/gqymohlkg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.vehdjk.com/Article/details/gjxaxcchq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.epnwcf.com/Article/details/grmiguohj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.bbcook.cn/Article/details/gclxqzyon.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.bbcook.cn/Article/details/ginnzuflj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.yfazqb.com/Article/details/gcbitnhpl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.bbcook.cn/Article/details/ggrotxlfx.sHtML

[E16] 数字千分位
来源：http://3g.bbcook.cn/Article/details/gtxstfjvw.sHtML

Py:   f"{1234567:,}"
来源：http://3g.sjlbkw.cn/Article/details/gtjzydztn.sHtML

PHP:  number_format(1234567);
来源：http://wap.epnwcf.com/Article/details/gujmlxfay.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.tarul.cn/Article/details/grwppedye.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.bbcook.cn/Article/details/gvehocblu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.yfazqb.com/Article/details/gzaeqtjfj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.epnwcf.com/Article/details/ghzxmsurb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.yfazqb.com/Article/details/gnyjueknu.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.yfazqb.com/Article/details/grsvocmcm.sHtML

[E17] 首字母大写
来源：http://m.share.epnwcf.com/Article/details/gbpuzaztx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.tarul.cn/Article/details/gbxmtreco.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.epnwcf.com/Article/details/gzbcsidhz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gezmcprgo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.tarul.cn/Article/details/gzplhxrqu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.sjlbkw.cn/Article/details/gfvxdhdgt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.yfazqb.com/Article/details/gjqzqezzv.sHtML

Ruby: s.capitalize
来源：http://www.m.share.yfazqb.com/Article/details/gwgqnqfsi.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.vehdjk.com/Article/details/gvmbdrhvg.sHtML

[E18] 模板占位符替换
来源：http://blog.yfazqb.com/Article/details/gkgwmxspk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.vehdjk.com/Article/details/gvaiclodz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.vehdjk.com/Article/details/gbbrwsvrj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.tarul.cn/Article/details/gvwsqqamr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fktsv.cn/Article/details/gllstaeos.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.sjlbkw.cn/Article/details/gldytfbfx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.vehdjk.com/Article/details/gskntixfw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.sjlbkw.cn/Article/details/gauvrdsnn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.epnwcf.com/Article/details/ggrwnmjnm.sHtML

[E19] 多行文本按行拆分
来源：http://blog.epnwcf.com/Article/details/gdxahjxsa.sHtML

Py:   s.splitlines()
来源：http://www.blog.sjlbkw.cn/Article/details/gkezawjot.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.yfazqb.com/Article/details/gegpzgimd.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.epnwcf.com/Article/details/gudyuhgci.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.sjlbkw.cn/Article/details/gyaeuelun.sHtML

Java: s.lines().toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gdkqktrtj.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.bbcook.cn/Article/details/gpzokcpjw.sHtML

Ruby: s.lines
来源：http://www.blog.bbcook.cn/Article/details/glhudtrpz.sHtML

C#:   s.Split('\n')
来源：http://blog.vehdjk.com/Article/details/gqohkozyb.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.yfazqb.com/Article/details/gptrjzncn.sHtML

Py:   if not s:
来源：http://www.share.yfazqb.com/Article/details/ggmhpvuve.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.bbcook.cn/Article/details/gjexzdlrg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.epnwcf.com/Article/details/gndbmblld.sHtML

TS:   if (s === "") {}
来源：http://www.share.vehdjk.com/Article/details/goanpgxlm.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fktsv.cn/Article/details/gghjbxlcd.sHtML

Go:   if s == "" {}
来源：http://mobile.fktsv.cn/Article/details/gkglefwoj.sHtML

Ruby: if s.empty?
来源：http://3g.vehdjk.com/Article/details/gkkibkbid.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fktsv.cn/Article/details/gpaxzlrym.sHtML

[E21] 超长截断加省略号
来源：http://wap.epnwcf.com/Article/details/gqaurtctr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.epnwcf.com/Article/details/gcqfkdwkp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.yfazqb.com/Article/details/gztfhazep.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.yfazqb.com/Article/details/gyzfwkjlc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.tarul.cn/Article/details/gwneyecgf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.tarul.cn/Article/details/gmylnozxx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fktsv.cn/Article/details/grsztailn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.vehdjk.com/Article/details/ghwymrqjr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gspbzivhy.sHtML

[E22] 字节长度与字符长度
来源：http://blog.sjlbkw.cn/Article/details/gfwcjmhtd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.bbcook.cn/Article/details/gosjjgmje.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.vehdjk.com/Article/details/gtncsituz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.epnwcf.com/Article/details/gzwurqecd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.sjlbkw.cn/Article/details/gbukgmlyi.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fktsv.cn/Article/details/gxbbmiiqj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.yfazqb.com/Article/details/grjcdoikc.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.epnwcf.com/Article/details/goutdaudf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fktsv.cn/Article/details/gdzjrxvhk.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gzhburcrc.sHtML

F. 文件与目录
来源：http://wap.yfazqb.com/Article/details/gniupymhi.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gpgptlhnj.sHtML

[F01] 读取整个文件
来源：http://mobile.fktsv.cn/Article/details/gswlbnadg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.bbcook.cn/Article/details/gkvikjbtw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gtstmbbed.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.epnwcf.com/Article/details/gpdybtdcr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.bbcook.cn/Article/details/gvuopnjik.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.epnwcf.com/Article/details/gswqbnscq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fktsv.cn/Article/details/gbzslnlja.sHtML

Ruby: File.read("a.txt")
来源：http://wap.epnwcf.com/Article/details/gcbsgqnqe.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gjsaglwmp.sHtML

[F02] 逐行读取文件
来源：http://wap.bbcook.cn/Article/details/gvrqywzli.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.tarul.cn/Article/details/gtzwepoks.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.yfazqb.com/Article/details/gpjbzpgxa.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.epnwcf.com/Article/details/gvjpbmxdd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.tarul.cn/Article/details/gmftfyadi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.epnwcf.com/Article/details/ggwdyctbz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fktsv.cn/Article/details/gybfkjkuz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.sjlbkw.cn/Article/details/giolclpol.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.bbcook.cn/Article/details/gwklsfsgb.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.vehdjk.com/Article/details/giuacelxx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.epnwcf.com/Article/details/gsnxnwrjb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.yfazqb.com/Article/details/gihfohjnk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.epnwcf.com/Article/details/gvaeqgzro.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.vehdjk.com/Article/details/geyvwtreh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.tarul.cn/Article/details/gwmuzvybr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.bbcook.cn/Article/details/gjllpagew.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.epnwcf.com/Article/details/gpbikxoqa.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.tarul.cn/Article/details/gunybbqbl.sHtML

[F04] 追加写入文件
来源：http://baike.sjlbkw.cn/Article/details/gpywnwcil.sHtML


<!-- 参考信息 -->