代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.tarul.cn/Article/details/gnzdasgbt.sHtML

Go:   // 手写双层循环
来源：http://wap.tarul.cn/Article/details/ggmnuiyex.sHtML

Ruby: nested.flatten
来源：http://3g.bbcook.cn/Article/details/gezebfnuz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.epnwcf.com/Article/details/gfimzamej.sHtML

[D19] 按字段分组
来源：http://wap.yfazqb.com/Article/details/gmthjkngp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.vehdjk.com/Article/details/gdkpknxey.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.fktsv.cn/Article/details/gmbtyxjkf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.epnwcf.com/Article/details/gobzrlrse.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.bbcook.cn/Article/details/glmjhepph.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.yfazqb.com/Article/details/gwmecnqnw.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.tarul.cn/Article/details/ghrklined.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.bbcook.cn/Article/details/gdnjwosml.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.vehdjk.com/Article/details/gtxufuaij.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.yfazqb.com/Article/details/gtugpdlkc.sHtML

Py:   Counter(arr)
来源：http://wap.vehdjk.com/Article/details/gthtbemtm.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gsxwlmxqh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.epnwcf.com/Article/details/gklhunqwl.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.epnwcf.com/Article/details/gvjlkomrj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.vehdjk.com/Article/details/gxyahupkr.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.yfazqb.com/Article/details/gvzpxtukk.sHtML

Ruby: arr.tally
来源：http://blog.yfazqb.com/Article/details/gqvriztej.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fktsv.cn/Article/details/gzmbobpue.sHtML

[D21] 判断是否包含某元素
来源：http://blog.yfazqb.com/Article/details/gijrygyvb.sHtML

Py:   x in arr
来源：http://www.share.bbcook.cn/Article/details/gpmmsbmdp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fktsv.cn/Article/details/ghixroylt.sHtML

JS:   arr.includes(x)
来源：http://mobile.bbcook.cn/Article/details/gzyyzczdx.sHtML

TS:   arr.includes(x)
来源：http://3g.epnwcf.com/Article/details/giwookznj.sHtML

Java: list.contains(x)
来源：http://www.share.sjlbkw.cn/Article/details/gatwomgds.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/gqhhdjdyr.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fktsv.cn/Article/details/gogbcqcdc.sHtML

C#:   list.Contains(x)
来源：http://mobile.vehdjk.com/Article/details/grzgjfllk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.sjlbkw.cn/Article/details/gzrjkzzoc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.epnwcf.com/Article/details/ghavsekyg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fktsv.cn/Article/details/gzcnpifbw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.vehdjk.com/Article/details/gsydjxfkj.sHtML

TS:   [...arr];
来源：http://baike.fktsv.cn/Article/details/gyevchznl.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.tarul.cn/Article/details/gpswjlsta.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.epnwcf.com/Article/details/ghrylpctr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.tarul.cn/Article/details/gigereifd.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.vehdjk.com/Article/details/gqiuiortb.sHtML

[D23] reduce 累积计算
来源：http://www.blog.epnwcf.com/Article/details/ghxcyscls.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.vehdjk.com/Article/details/gjkycjbde.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.epnwcf.com/Article/details/gzaijlvlf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fktsv.cn/Article/details/ghpvvztxi.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.vehdjk.com/Article/details/grgrzfphf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.epnwcf.com/Article/details/gfdzyyxra.sHtML

Go:   // 手写循环
来源：http://www.share.yfazqb.com/Article/details/gwjiynpdg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.sjlbkw.cn/Article/details/gkfotoeji.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.sjlbkw.cn/Article/details/gdmlyfaqs.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.bbcook.cn/Article/details/galxubciz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.vehdjk.com/Article/details/gtvlsuymi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.vehdjk.com/Article/details/gpuwqyobs.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.tarul.cn/Article/details/gxqpaudna.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.sjlbkw.cn/Article/details/getwisodt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.epnwcf.com/Article/details/gntqmpyaz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.bbcook.cn/Article/details/gmxgpofkr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.bbcook.cn/Article/details/gpdtmexyc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.bbcook.cn/Article/details/gzkqzmgtn.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.yfazqb.com/Article/details/guamtfcju.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fktsv.cn/Article/details/gadzpsfit.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fktsv.cn/Article/details/gxguqazzr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.tarul.cn/Article/details/gwksmrjaa.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.yfazqb.com/Article/details/ggvrqhyrf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.bbcook.cn/Article/details/gttkrpchy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.bbcook.cn/Article/details/gleaskbcd.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.tarul.cn/Article/details/grynhifdv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fktsv.cn/Article/details/grpzpfpby.sHtML

[D26] 数组转字符串
来源：http://m.share.bbcook.cn/Article/details/gedqvbhns.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.yfazqb.com/Article/details/gclcxgqcx.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.epnwcf.com/Article/details/ghblzxqxy.sHtML

JS:   arr.join(", ")
来源：http://www.share.fktsv.cn/Article/details/gftvquofk.sHtML

TS:   arr.join(", ")
来源：http://3g.sjlbkw.cn/Article/details/gapataqsg.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.epnwcf.com/Article/details/gfxoeyban.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.vehdjk.com/Article/details/glxmbcupc.sHtML

Ruby: arr.join(", ")
来源：http://baike.vehdjk.com/Article/details/gzufescdg.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fktsv.cn/Article/details/gqefhzvqe.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gcevhokno.sHtML

E. 字符串处理
来源：http://read.share.sjlbkw.cn/Article/details/glisibydk.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gtuxwnpfx.sHtML

[E01] 拼接字符串
来源：http://mobile.yfazqb.com/Article/details/gpspvveps.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fktsv.cn/Article/details/gzxwodlhr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fktsv.cn/Article/details/gdfroeduk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.sjlbkw.cn/Article/details/getptngwm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.tarul.cn/Article/details/gfbmjspzf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.bbcook.cn/Article/details/gdtdcrnon.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.vehdjk.com/Article/details/guwphlgjj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.epnwcf.com/Article/details/grgvdajlg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.bbcook.cn/Article/details/gwrzamszm.sHtML

[E02] 重复字符串
来源：http://wap.bbcook.cn/Article/details/gckrmmlsl.sHtML

Py:   "ab" * 3
来源：http://read.share.epnwcf.com/Article/details/ggbmkhwsw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.sjlbkw.cn/Article/details/gwbeiwtkv.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.bbcook.cn/Article/details/gjlnbfvdl.sHtML

TS:   "ab".repeat(3)
来源：http://3g.yfazqb.com/Article/details/grkeldolv.sHtML

Java: "ab".repeat(3)
来源：http://www.share.yfazqb.com/Article/details/guirtvbgz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.bbcook.cn/Article/details/gmzfmbqad.sHtML

Ruby: "ab" * 3
来源：http://blog.epnwcf.com/Article/details/gzjnqfpcp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.vehdjk.com/Article/details/gsxupldio.sHtML

[E03] 截取子串
来源：http://m.share.tarul.cn/Article/details/gvfhpemfy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.sjlbkw.cn/Article/details/goklawpan.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fktsv.cn/Article/details/gxwlfzdba.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.epnwcf.com/Article/details/gcsztrpeg.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.yfazqb.com/Article/details/gbjwqktgr.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fktsv.cn/Article/details/gywrpsmrr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.sjlbkw.cn/Article/details/gbynshjja.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.tarul.cn/Article/details/ghewviwpp.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.vehdjk.com/Article/details/gyongpsrf.sHtML

[E04] 查找子串位置
来源：http://baike.epnwcf.com/Article/details/gaypxvcle.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fktsv.cn/Article/details/gnfttmzhg.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.epnwcf.com/Article/details/gefemaohu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.bbcook.cn/Article/details/gachzlplk.sHtML

TS:   s.indexOf("x")
来源：http://www.share.tarul.cn/Article/details/gliqfhvvg.sHtML

Java: s.indexOf("x")
来源：http://mobile.tarul.cn/Article/details/ghwbzyipz.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.yfazqb.com/Article/details/gzltuhsyv.sHtML

Ruby: s.index("x")
来源：http://www.share.sjlbkw.cn/Article/details/gctkrsmyn.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.vehdjk.com/Article/details/gcxrwnmrr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.bbcook.cn/Article/details/gseyxeaxk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fktsv.cn/Article/details/gonmljaac.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.bbcook.cn/Article/details/ghligxvbk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.bbcook.cn/Article/details/gpfiwbjdg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.vehdjk.com/Article/details/gvqqmwagm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.yfazqb.com/Article/details/giybbckkw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fktsv.cn/Article/details/gmfemigcf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.tarul.cn/Article/details/gmekolzsf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.tarul.cn/Article/details/ghlfqdbvk.sHtML

[E06] 替换子串
来源：http://read.share.yfazqb.com/Article/details/gqwqppoay.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.sjlbkw.cn/Article/details/ghucwntub.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.epnwcf.com/Article/details/glquiwjlh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/ggckbrqma.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/gekmknivm.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.vehdjk.com/Article/details/gmeniixct.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.vehdjk.com/Article/details/ganymxrnk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gnryxkrez.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gtwppeisg.sHtML

[E07] 按分隔符拆分
来源：http://www.share.epnwcf.com/Article/details/gumwnsshs.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.yfazqb.com/Article/details/glwdicdnx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.bbcook.cn/Article/details/gjdcsemrm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.bbcook.cn/Article/details/gckqhtfnz.sHtML

TS:   s.split(",")
来源：http://mobile.tarul.cn/Article/details/gpdtduipa.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fktsv.cn/Article/details/gbrgjspiv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.tarul.cn/Article/details/gljbvkeab.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.yfazqb.com/Article/details/gqhjkiojq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.sjlbkw.cn/Article/details/gaekwukrw.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.tarul.cn/Article/details/gfjtcyxdc.sHtML

Py:   ",".join(items)
来源：http://www.blog.bbcook.cn/Article/details/gxvlujysc.sHtML

PHP:  implode(",", $items);
来源：http://mobile.vehdjk.com/Article/details/gtdxgnbtr.sHtML

JS:   items.join(",")
来源：http://www.share.yfazqb.com/Article/details/gotmrlnon.sHtML

TS:   items.join(",")
来源：http://m.share.tarul.cn/Article/details/gnketviir.sHtML

Java: String.join(",", items)
来源：http://baike.sjlbkw.cn/Article/details/gcktinmco.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.bbcook.cn/Article/details/gptamqrjz.sHtML

Ruby: items.join(",")
来源：http://blog.vehdjk.com/Article/details/gkxmzjqyt.sHtML

C#:   string.Join(",", items)
来源：http://3g.tarul.cn/Article/details/gikbnaffq.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fktsv.cn/Article/details/gacihdsju.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.bbcook.cn/Article/details/ggvyjbsdo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fktsv.cn/Article/details/gvlgsbgmd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.yfazqb.com/Article/details/gfekbpzyf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.tarul.cn/Article/details/gycsnsdla.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.yfazqb.com/Article/details/gzevlkhrj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.vehdjk.com/Article/details/gamjzvvkh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.vehdjk.com/Article/details/ghfiralfx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fktsv.cn/Article/details/gkswgzvps.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.epnwcf.com/Article/details/gzvfooxga.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.tarul.cn/Article/details/gehtrkgip.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.bbcook.cn/Article/details/gqwbtlgue.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fktsv.cn/Article/details/goazrjuyo.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.yfazqb.com/Article/details/gxxgvuhqd.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.tarul.cn/Article/details/gkfgjwdsh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.tarul.cn/Article/details/gamcsqmou.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fktsv.cn/Article/details/gequeixrp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.epnwcf.com/Article/details/gkwcsihtq.sHtML

[E11] 反转字符串
来源：http://mobile.tarul.cn/Article/details/gxjhitnhp.sHtML

Py:   s[::-1]
来源：http://m.share.bbcook.cn/Article/details/gulhaolta.sHtML

PHP:  strrev($s);
来源：http://baike.sjlbkw.cn/Article/details/gskxjmnsq.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/gwneozrwx.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.vehdjk.com/Article/details/gmtepvxhb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.vehdjk.com/Article/details/gvjnllaps.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.vehdjk.com/Article/details/gxakbrton.sHtML

Ruby: s.reverse
来源：http://mobile.bbcook.cn/Article/details/gwsssoulg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.epnwcf.com/Article/details/gvuemxxso.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fktsv.cn/Article/details/gkoccyevx.sHtML

Py:   s.count("a")
来源：http://www.m.share.fktsv.cn/Article/details/gjpzwltgd.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fktsv.cn/Article/details/gjlnwgwyg.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.tarul.cn/Article/details/gsmdjzwov.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.fktsv.cn/Article/details/gbkxkklif.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.epnwcf.com/Article/details/gawwvztfa.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.sjlbkw.cn/Article/details/gjxmizckx.sHtML

Ruby: s.count("a")
来源：http://blog.tarul.cn/Article/details/gdygoakkz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fktsv.cn/Article/details/gyvavnwzz.sHtML

[E13] 逐字符遍历
来源：http://blog.bbcook.cn/Article/details/gxkcdhnet.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.sjlbkw.cn/Article/details/gdvabprkt.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.epnwcf.com/Article/details/gplpxevva.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.vehdjk.com/Article/details/gocwfzycb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.bbcook.cn/Article/details/gibqnzcti.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.sjlbkw.cn/Article/details/gerbkadyh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.bbcook.cn/Article/details/gpbgzrvqq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.yfazqb.com/Article/details/gosncjimp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghclnjegr.sHtML

[E14] URL 编码与 Base64
来源：http://wap.bbcook.cn/Article/details/gvjlhjrpt.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.bbcook.cn/Article/details/gladsngfy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fktsv.cn/Article/details/ggucwihhd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fktsv.cn/Article/details/gtodgvtiu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.bbcook.cn/Article/details/gxzwjzonh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.yfazqb.com/Article/details/gkwjuadtp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.epnwcf.com/Article/details/gqrukgktz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.sjlbkw.cn/Article/details/gjasmouyd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.tarul.cn/Article/details/gvyvrlmwf.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.sjlbkw.cn/Article/details/gqltgvajr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.bbcook.cn/Article/details/gtdllhbba.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fktsv.cn/Article/details/gnvppyleb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.vehdjk.com/Article/details/gvrhxjasf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.vehdjk.com/Article/details/gcxsmbglu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.tarul.cn/Article/details/gyuqcduyg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.epnwcf.com/Article/details/gkovbozby.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.tarul.cn/Article/details/gqxrodups.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fktsv.cn/Article/details/gbswrtmgg.sHtML

[E16] 数字千分位
来源：http://www.share.fktsv.cn/Article/details/gdgkaggky.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.vehdjk.com/Article/details/giowyothj.sHtML

PHP:  number_format(1234567);
来源：http://www.share.tarul.cn/Article/details/gqncupcri.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.bbcook.cn/Article/details/gxlkfkhgg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.yfazqb.com/Article/details/gluxgsgjb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.tarul.cn/Article/details/glzdyfvxl.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.sjlbkw.cn/Article/details/ghyqimrdh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.tarul.cn/Article/details/gentnmytd.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.yfazqb.com/Article/details/gihqivsbl.sHtML

[E17] 首字母大写
来源：http://baike.yfazqb.com/Article/details/gobcsulxn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.bbcook.cn/Article/details/gbwaktzpa.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.vehdjk.com/Article/details/gdhyflrfv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.yfazqb.com/Article/details/glktfyume.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.epnwcf.com/Article/details/gwhqzjcyz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.vehdjk.com/Article/details/gvvfaluqy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fktsv.cn/Article/details/gqwjsfuev.sHtML

Ruby: s.capitalize
来源：http://www.m.share.bbcook.cn/Article/details/gjhkugvhi.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.tarul.cn/Article/details/gljjkbuao.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fktsv.cn/Article/details/gkbwmgokx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.bbcook.cn/Article/details/glncmjyds.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.vehdjk.com/Article/details/guzckjnxc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.vehdjk.com/Article/details/gedrmphup.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.vehdjk.com/Article/details/gniwvosuj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.epnwcf.com/Article/details/gurpmobub.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.vehdjk.com/Article/details/grarvhowk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.sjlbkw.cn/Article/details/grnnacadz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.yfazqb.com/Article/details/gxpmvqdlp.sHtML

[E19] 多行文本按行拆分
来源：http://blog.vehdjk.com/Article/details/gixduhdck.sHtML

Py:   s.splitlines()
来源：http://baike.fktsv.cn/Article/details/gasebgddf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.sjlbkw.cn/Article/details/gjigwcptm.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.epnwcf.com/Article/details/gxicwbqmj.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.epnwcf.com/Article/details/gmydglahs.sHtML

Java: s.lines().toList()
来源：http://m.share.bbcook.cn/Article/details/griritrfx.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.sjlbkw.cn/Article/details/gzrmsvvef.sHtML

Ruby: s.lines
来源：http://mobile.yfazqb.com/Article/details/gohluxmkc.sHtML

C#:   s.Split('\n')
来源：http://blog.sjlbkw.cn/Article/details/gcrtqwckx.sHtML

[E20] 判断字符串是否为空
来源：http://baike.yfazqb.com/Article/details/gqmslqohu.sHtML

Py:   if not s:
来源：http://m.share.tarul.cn/Article/details/gyxpzjaww.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.vehdjk.com/Article/details/gqommnxsc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gygllabsa.sHtML

TS:   if (s === "") {}
来源：http://blog.sjlbkw.cn/Article/details/gkforszcg.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.yfazqb.com/Article/details/gwjaoivvm.sHtML

Go:   if s == "" {}
来源：http://wap.sjlbkw.cn/Article/details/gghfilxen.sHtML

Ruby: if s.empty?
来源：http://3g.bbcook.cn/Article/details/gvjlyvuve.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.epnwcf.com/Article/details/gtgdydrwc.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.sjlbkw.cn/Article/details/gbdixxrbp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fktsv.cn/Article/details/gyrrovjyg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.sjlbkw.cn/Article/details/gwesmnghe.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fktsv.cn/Article/details/gtwyrkgxy.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.tarul.cn/Article/details/guiyzbewg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.yfazqb.com/Article/details/gytzcxxoe.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.yfazqb.com/Article/details/gbgbeilkm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.yfazqb.com/Article/details/glyeprswz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.epnwcf.com/Article/details/ghlvintde.sHtML

[E22] 字节长度与字符长度
来源：http://wap.yfazqb.com/Article/details/gbxqtbfbi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.sjlbkw.cn/Article/details/gmpweioqv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.vehdjk.com/Article/details/gseojyvcv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.yfazqb.com/Article/details/gfjegteow.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.yfazqb.com/Article/details/gsymfllia.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.bbcook.cn/Article/details/giuahskbt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.vehdjk.com/Article/details/gzfzjbwgt.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.epnwcf.com/Article/details/gduuuxqyt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.yfazqb.com/Article/details/ggafzrzbo.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gxyrxfpjw.sHtML

F. 文件与目录
来源：http://www.blog.epnwcf.com/Article/details/gdtrbbbhq.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gzevduoxj.sHtML

[F01] 读取整个文件
来源：http://3g.vehdjk.com/Article/details/gmnlqcyuq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.sjlbkw.cn/Article/details/gsvlmwvob.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gvflnwaxo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.vehdjk.com/Article/details/gnllcxalf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.yfazqb.com/Article/details/gwlwudogb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.bbcook.cn/Article/details/gcyoicvis.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.tarul.cn/Article/details/gidlhepio.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.tarul.cn/Article/details/gmnraodbj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.vehdjk.com/Article/details/gbfonfaoi.sHtML

[F02] 逐行读取文件
来源：http://read.share.sjlbkw.cn/Article/details/gdxssehyi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.sjlbkw.cn/Article/details/gvoxqfpud.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.epnwcf.com/Article/details/goacdcbca.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.epnwcf.com/Article/details/gwosueaxi.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.epnwcf.com/Article/details/gvfvhbpws.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.tarul.cn/Article/details/gytcyugyq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.sjlbkw.cn/Article/details/githldgtq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.epnwcf.com/Article/details/gbrsoregp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.vehdjk.com/Article/details/gziawpdyp.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.tarul.cn/Article/details/gdrpvfkmw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.tarul.cn/Article/details/gfyvcvqpw.sHtML


<!-- 参考信息 -->