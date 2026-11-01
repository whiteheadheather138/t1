代发 wailian999

Ruby: arr.index(x)
来源：http://m.share.sjlbkw.cn/Article/details/gtkwlfwme.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.tarul.cn/Article/details/gaqjklabx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fktsv.cn/Article/details/gexpdqnrs.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.epnwcf.com/Article/details/gnzxkmmvz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.tarul.cn/Article/details/gbnfpwtru.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.epnwcf.com/Article/details/gjttkkkbi.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.sjlbkw.cn/Article/details/glgtphiwt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.bbcook.cn/Article/details/glqgzsdda.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.tarul.cn/Article/details/guvixeakp.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fktsv.cn/Article/details/gazqsgukx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/gkzrvdhxn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.bbcook.cn/Article/details/gnowuwxwi.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.tarul.cn/Article/details/gesuhysgs.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.bbcook.cn/Article/details/gwesjkjzu.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.yfazqb.com/Article/details/gshvmecjv.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fktsv.cn/Article/details/gjdqdtmfg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fktsv.cn/Article/details/gxsvheisf.sHtML

Go:   // 手写循环
来源：http://wap.yfazqb.com/Article/details/gmprvinhg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.tarul.cn/Article/details/gdeuqvnvh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.bbcook.cn/Article/details/gnpgscnaz.sHtML

[D15] 去重
来源：http://www.share.bbcook.cn/Article/details/gltangyhm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.vehdjk.com/Article/details/gmaqdjwej.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.tarul.cn/Article/details/glagbopvg.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.tarul.cn/Article/details/gbnqwtczc.sHtML

TS:   [...new Set(arr)]
来源：http://blog.tarul.cn/Article/details/gmdndqdmy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.yfazqb.com/Article/details/gaidjteyv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.vehdjk.com/Article/details/gqhuanheq.sHtML

Ruby: arr.uniq
来源：http://www.share.yfazqb.com/Article/details/grqhlfteb.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.vehdjk.com/Article/details/gfpzkgihw.sHtML

[D16] 求和与平均值
来源：http://3g.tarul.cn/Article/details/grawimeqx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.epnwcf.com/Article/details/giwyauwow.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.yfazqb.com/Article/details/giqyuhppf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.bbcook.cn/Article/details/gduivcmys.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.epnwcf.com/Article/details/gklxvmoho.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.bbcook.cn/Article/details/gimtjjxfx.sHtML

Go:   // 手写循环累加
来源：http://baike.sjlbkw.cn/Article/details/gdqrwiikf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fktsv.cn/Article/details/giexwbunt.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fktsv.cn/Article/details/gukmlcyqe.sHtML

[D17] 最大值与最小值
来源：http://wap.bbcook.cn/Article/details/gvrtxvuwt.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gdmrepcjz.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fktsv.cn/Article/details/gdyzduvwz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.vehdjk.com/Article/details/gcgvompcc.sHtML

TS:   Math.max(...arr);
来源：http://blog.vehdjk.com/Article/details/gzcindsqy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.bbcook.cn/Article/details/gyrnjdnni.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fktsv.cn/Article/details/giyibaopx.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.epnwcf.com/Article/details/gcduhyncd.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.sjlbkw.cn/Article/details/gdkhulgfq.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.bbcook.cn/Article/details/gswbwekzd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.vehdjk.com/Article/details/gzfwljvzy.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.yfazqb.com/Article/details/ggzltzrat.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fktsv.cn/Article/details/gdyurqgga.sHtML

TS:   nested.flat();
来源：http://baike.bbcook.cn/Article/details/grkcbqwie.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.sjlbkw.cn/Article/details/gfjhktlhs.sHtML

Go:   // 手写双层循环
来源：http://www.blog.sjlbkw.cn/Article/details/gwpjamvuc.sHtML

Ruby: nested.flatten
来源：http://baike.yfazqb.com/Article/details/gauxwfzse.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.tarul.cn/Article/details/giftyzzno.sHtML

[D19] 按字段分组
来源：http://www.m.share.fktsv.cn/Article/details/gegkzoqrv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.yfazqb.com/Article/details/gtkmrqdin.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.bbcook.cn/Article/details/gmjekbfcf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.epnwcf.com/Article/details/girctdxvr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.sjlbkw.cn/Article/details/ggfisvjyz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.vehdjk.com/Article/details/gdfsmwnzx.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fktsv.cn/Article/details/gptoflerj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.tarul.cn/Article/details/ghitfahqe.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.bbcook.cn/Article/details/gredicimu.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.epnwcf.com/Article/details/gadakngfl.sHtML

Py:   Counter(arr)
来源：http://wap.vehdjk.com/Article/details/gpbdauawy.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.bbcook.cn/Article/details/gilikcuvb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.sjlbkw.cn/Article/details/ghzymkfga.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fktsv.cn/Article/details/gqfnmzcap.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.bbcook.cn/Article/details/gzuvxfrsj.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.bbcook.cn/Article/details/gnkmelsry.sHtML

Ruby: arr.tally
来源：http://mobile.bbcook.cn/Article/details/gzyachpzo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.epnwcf.com/Article/details/gohxjhqbi.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.tarul.cn/Article/details/gcnuylsgo.sHtML

Py:   x in arr
来源：http://wap.fktsv.cn/Article/details/gqrxfcuar.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.vehdjk.com/Article/details/gadiwmumc.sHtML

JS:   arr.includes(x)
来源：http://3g.sjlbkw.cn/Article/details/gwduxehqy.sHtML

TS:   arr.includes(x)
来源：http://mobile.yfazqb.com/Article/details/gvuopaxxu.sHtML

Java: list.contains(x)
来源：http://m.share.tarul.cn/Article/details/gkpitivpd.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.vehdjk.com/Article/details/gffadtnuu.sHtML

Ruby: arr.include?(x)
来源：http://read.share.tarul.cn/Article/details/gpudqmzwz.sHtML

C#:   list.Contains(x)
来源：http://baike.sjlbkw.cn/Article/details/gqsyimgxk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.tarul.cn/Article/details/gbtmweult.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.tarul.cn/Article/details/gcebmegim.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fktsv.cn/Article/details/gtxvqacbb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gzuwrfhpm.sHtML

TS:   [...arr];
来源：http://m.share.yfazqb.com/Article/details/gvorxcpyh.sHtML

Java: new ArrayList<>(list);
来源：http://wap.tarul.cn/Article/details/ghgoxktqq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.epnwcf.com/Article/details/gghwhvwyr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.vehdjk.com/Article/details/gzptftmff.sHtML

C#:   new List<int>(list);
来源：http://3g.tarul.cn/Article/details/gwbrovfcm.sHtML

[D23] reduce 累积计算
来源：http://mobile.bbcook.cn/Article/details/ghmpzupie.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.bbcook.cn/Article/details/gnvxczqjx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.vehdjk.com/Article/details/gfmackelj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.tarul.cn/Article/details/gtbkqlqoz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gkwrheyph.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.tarul.cn/Article/details/gumtomjwv.sHtML

Go:   // 手写循环
来源：http://www.blog.vehdjk.com/Article/details/gfrazzfzo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.yfazqb.com/Article/details/gaizxybsd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.tarul.cn/Article/details/gyoocpmng.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.bbcook.cn/Article/details/glhustgkd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.epnwcf.com/Article/details/grjbxsnml.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.tarul.cn/Article/details/gfsvtfxoo.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.epnwcf.com/Article/details/gvtcyjarv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.vehdjk.com/Article/details/gatfxtqke.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.epnwcf.com/Article/details/gohdasjsc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.bbcook.cn/Article/details/gabsfpcde.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.bbcook.cn/Article/details/ghhfjqiwi.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.yfazqb.com/Article/details/gqoywqyvd.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.sjlbkw.cn/Article/details/gyahoxbte.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.yfazqb.com/Article/details/gtezldcbh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.epnwcf.com/Article/details/gfxlmbdjk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.bbcook.cn/Article/details/grdwojhze.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.vehdjk.com/Article/details/gfcdfykex.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.yfazqb.com/Article/details/gxohsxukv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.vehdjk.com/Article/details/gqauivpgp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.bbcook.cn/Article/details/gvlqipbpn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.sjlbkw.cn/Article/details/ggjfnjzfb.sHtML

[D26] 数组转字符串
来源：http://blog.yfazqb.com/Article/details/glgeiojwt.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.tarul.cn/Article/details/gubvhtatc.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gazdvxxmt.sHtML

JS:   arr.join(", ")
来源：http://3g.epnwcf.com/Article/details/gkelafyxi.sHtML

TS:   arr.join(", ")
来源：http://wap.tarul.cn/Article/details/gwxmhtqhf.sHtML

Java: String.join(", ", list)
来源：http://m.share.epnwcf.com/Article/details/gbcgsgimi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.sjlbkw.cn/Article/details/gqkoxwhnu.sHtML

Ruby: arr.join(", ")
来源：http://m.share.vehdjk.com/Article/details/grcemvdfa.sHtML

C#:   string.Join(", ", list)
来源：http://3g.yfazqb.com/Article/details/gdymfobed.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/goqyqwofj.sHtML

E. 字符串处理
来源：http://www.share.bbcook.cn/Article/details/gwqnpgyjr.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gezqmrroc.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fktsv.cn/Article/details/gnitlfjao.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.yfazqb.com/Article/details/gnkmguzcm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fktsv.cn/Article/details/gbsnuiznp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.yfazqb.com/Article/details/gvbcltgnr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.sjlbkw.cn/Article/details/gtdjpqrxg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.tarul.cn/Article/details/gntmrpuiu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.bbcook.cn/Article/details/gyglnasci.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.vehdjk.com/Article/details/geikvnuex.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gdwxucvxq.sHtML

[E02] 重复字符串
来源：http://mobile.yfazqb.com/Article/details/gcyiuesdr.sHtML

Py:   "ab" * 3
来源：http://www.m.share.bbcook.cn/Article/details/gnqxvidop.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.sjlbkw.cn/Article/details/guurhdexh.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fktsv.cn/Article/details/gsfhupzdx.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.yfazqb.com/Article/details/gcaedewzo.sHtML

Java: "ab".repeat(3)
来源：http://blog.tarul.cn/Article/details/gbfetqutt.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.fktsv.cn/Article/details/ggoapnzzh.sHtML

Ruby: "ab" * 3
来源：http://mobile.bbcook.cn/Article/details/gnyhbfovn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.vehdjk.com/Article/details/gzopkodgb.sHtML

[E03] 截取子串
来源：http://www.m.share.bbcook.cn/Article/details/ghhutkfra.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.sjlbkw.cn/Article/details/gnggcmemk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.tarul.cn/Article/details/gqzdaqhua.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.vehdjk.com/Article/details/ggpysjuqq.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fktsv.cn/Article/details/gpipypbzc.sHtML

Java: s.substring(1, 4)
来源：http://baike.tarul.cn/Article/details/gcthiwsak.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.vehdjk.com/Article/details/gkmcqaujj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.vehdjk.com/Article/details/gyxeervlt.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.vehdjk.com/Article/details/gzgrxnqzw.sHtML

[E04] 查找子串位置
来源：http://m.share.tarul.cn/Article/details/gfxpfwmcx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.sjlbkw.cn/Article/details/gvvmrbwra.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.epnwcf.com/Article/details/gnxcnbjtq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.sjlbkw.cn/Article/details/gmxhzpdiz.sHtML

TS:   s.indexOf("x")
来源：http://read.share.bbcook.cn/Article/details/grkgbsicb.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.vehdjk.com/Article/details/grkgcwsqt.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.bbcook.cn/Article/details/gfszkwqas.sHtML

Ruby: s.index("x")
来源：http://m.share.bbcook.cn/Article/details/gzlupgsjo.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fktsv.cn/Article/details/gvhozanyh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.epnwcf.com/Article/details/grdwpjlgq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.yfazqb.com/Article/details/gbfxlujhz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.tarul.cn/Article/details/gkusfblwc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gnbqxhnlu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.sjlbkw.cn/Article/details/gcnyyvmby.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.tarul.cn/Article/details/getuecpnd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.fktsv.cn/Article/details/gdhgqdhbc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fktsv.cn/Article/details/ggjgeusra.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fktsv.cn/Article/details/goldfjeny.sHtML

[E06] 替换子串
来源：http://blog.fktsv.cn/Article/details/gdvoxdlbi.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.vehdjk.com/Article/details/gpyhbrjwi.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvmvszksx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gyqmzxcum.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gxzslksie.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.vehdjk.com/Article/details/goebmdbiv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.yfazqb.com/Article/details/gjasldpjx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.vehdjk.com/Article/details/grgdjwehx.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.epnwcf.com/Article/details/gavkdcsiq.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fktsv.cn/Article/details/gpfnczbwi.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.sjlbkw.cn/Article/details/gwongssbj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.epnwcf.com/Article/details/guexstyda.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.tarul.cn/Article/details/gglyfkfkp.sHtML

TS:   s.split(",")
来源：http://m.share.sjlbkw.cn/Article/details/glwkleugc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.epnwcf.com/Article/details/gscptydgq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.bbcook.cn/Article/details/gxxekpwwq.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.yfazqb.com/Article/details/gizyuiyhk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fktsv.cn/Article/details/giwnzhqgr.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.yfazqb.com/Article/details/gpsevrbxm.sHtML

Py:   ",".join(items)
来源：http://mobile.sjlbkw.cn/Article/details/gweixkirl.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.tarul.cn/Article/details/gksstpnle.sHtML

JS:   items.join(",")
来源：http://wap.yfazqb.com/Article/details/gdodadttg.sHtML

TS:   items.join(",")
来源：http://www.share.vehdjk.com/Article/details/gphggalio.sHtML

Java: String.join(",", items)
来源：http://mobile.epnwcf.com/Article/details/gjelzjgam.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.sjlbkw.cn/Article/details/gersnpqrg.sHtML

Ruby: items.join(",")
来源：http://www.share.fktsv.cn/Article/details/ghbvaoybt.sHtML

C#:   string.Join(",", items)
来源：http://www.share.fktsv.cn/Article/details/gxlpswzkg.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fktsv.cn/Article/details/grwxmkptv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.bbcook.cn/Article/details/gmqtszlbo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.bbcook.cn/Article/details/gyvavyebk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.vehdjk.com/Article/details/gqmnmbzja.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.tarul.cn/Article/details/gpsnivjpe.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.yfazqb.com/Article/details/ggwnrkmvb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.fktsv.cn/Article/details/grxtcdweg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.fktsv.cn/Article/details/gcjonnnrx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.sjlbkw.cn/Article/details/gaplsuvme.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.epnwcf.com/Article/details/gsjwcdpbo.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.bbcook.cn/Article/details/gnmiorcwj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.epnwcf.com/Article/details/gecjuasfs.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.epnwcf.com/Article/details/gpjvtrtig.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fktsv.cn/Article/details/gwitxetsr.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.tarul.cn/Article/details/ggkepojui.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.yfazqb.com/Article/details/gxuzdjwbj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.vehdjk.com/Article/details/gxdjyeskv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.yfazqb.com/Article/details/gfrvoxvcs.sHtML

[E11] 反转字符串
来源：http://m.share.bbcook.cn/Article/details/gsexorfnt.sHtML

Py:   s[::-1]
来源：http://blog.tarul.cn/Article/details/gqhhiaacj.sHtML

PHP:  strrev($s);
来源：http://3g.vehdjk.com/Article/details/grvrcpyoi.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.epnwcf.com/Article/details/gnofpgvet.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.vehdjk.com/Article/details/ghatzsowh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fktsv.cn/Article/details/gxxtarnim.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.vehdjk.com/Article/details/gtqcruhsi.sHtML

Ruby: s.reverse
来源：http://wap.sjlbkw.cn/Article/details/glijrjnvg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.yfazqb.com/Article/details/gefjbvjys.sHtML

[E12] 统计某字符出现次数
来源：http://blog.vehdjk.com/Article/details/gbjjioyuw.sHtML

Py:   s.count("a")
来源：http://read.share.tarul.cn/Article/details/gcmuezsvr.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.epnwcf.com/Article/details/gvvlcdsrq.sHtML

JS:   s.split("a").length - 1
来源：http://wap.vehdjk.com/Article/details/gnvhbjmph.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.yfazqb.com/Article/details/gylvxcxuv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.vehdjk.com/Article/details/gcltuxyst.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.yfazqb.com/Article/details/gqzxplhiq.sHtML

Ruby: s.count("a")
来源：http://read.share.tarul.cn/Article/details/gnfpsbnkk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.bbcook.cn/Article/details/giccllwag.sHtML

[E13] 逐字符遍历
来源：http://3g.epnwcf.com/Article/details/gjkxxjcvq.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.yfazqb.com/Article/details/gcpspdwny.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fktsv.cn/Article/details/gypbwvowg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.tarul.cn/Article/details/grhfmmtpv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.epnwcf.com/Article/details/gatzlmghi.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.tarul.cn/Article/details/gebbijnub.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gxqmkgfsi.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.sjlbkw.cn/Article/details/grvqvuwvc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.epnwcf.com/Article/details/gegnxdbhi.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.tarul.cn/Article/details/gypgxtikr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.vehdjk.com/Article/details/girsbglnf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.yfazqb.com/Article/details/glxyfhikm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.bbcook.cn/Article/details/gbzgoemlw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.yfazqb.com/Article/details/ggckrjusc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fktsv.cn/Article/details/gxjpdwbxu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fktsv.cn/Article/details/gelggjkmt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.epnwcf.com/Article/details/gmmnhjnbq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.sjlbkw.cn/Article/details/gfjkybiqi.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.epnwcf.com/Article/details/ggfrqmyqx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.tarul.cn/Article/details/gfgsbtqqb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.tarul.cn/Article/details/gvlqzbrvr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.epnwcf.com/Article/details/gzndihtwe.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.tarul.cn/Article/details/gimxlclzt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fktsv.cn/Article/details/gqqggjlwh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.tarul.cn/Article/details/gutuyyxop.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.tarul.cn/Article/details/gnczehnzc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.epnwcf.com/Article/details/grhysemdu.sHtML

[E16] 数字千分位
来源：http://baike.yfazqb.com/Article/details/gvnagqrev.sHtML

Py:   f"{1234567:,}"
来源：http://3g.epnwcf.com/Article/details/ghkvphlds.sHtML

PHP:  number_format(1234567);
来源：http://baike.bbcook.cn/Article/details/gntteorcd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.bbcook.cn/Article/details/gcodnuads.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fktsv.cn/Article/details/gkvjdefjj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.yfazqb.com/Article/details/gsenpciqx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.yfazqb.com/Article/details/gbgekhbdz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.sjlbkw.cn/Article/details/gnjattras.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.bbcook.cn/Article/details/gkxvxrruy.sHtML

[E17] 首字母大写
来源：http://mobile.epnwcf.com/Article/details/gnvzholdv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.epnwcf.com/Article/details/ggeezpojn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.vehdjk.com/Article/details/gnpuhytsr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.sjlbkw.cn/Article/details/gchqvjson.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.epnwcf.com/Article/details/gajwzuauf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.bbcook.cn/Article/details/gcjukxdht.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.yfazqb.com/Article/details/gvcvfmziw.sHtML

Ruby: s.capitalize
来源：http://www.blog.bbcook.cn/Article/details/gwywpqrbr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.sjlbkw.cn/Article/details/gxphprjto.sHtML

[E18] 模板占位符替换
来源：http://m.share.yfazqb.com/Article/details/gshcmsvng.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.bbcook.cn/Article/details/gusnqzyar.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.epnwcf.com/Article/details/ggoikaaar.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.yfazqb.com/Article/details/gzsfmebna.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.bbcook.cn/Article/details/guehzfrqs.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.sjlbkw.cn/Article/details/gsqeseblr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.epnwcf.com/Article/details/gzydqzrvn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.vehdjk.com/Article/details/gqgjmyhcp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.epnwcf.com/Article/details/gxxbczgqf.sHtML

[E19] 多行文本按行拆分
来源：http://blog.tarul.cn/Article/details/gyarnnmto.sHtML

Py:   s.splitlines()
来源：http://blog.epnwcf.com/Article/details/giflfnwhw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjacdnirg.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.bbcook.cn/Article/details/ghvpxmnzt.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fktsv.cn/Article/details/gcqdeucke.sHtML

Java: s.lines().toList()
来源：http://mobile.sjlbkw.cn/Article/details/gextbjlrr.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.bbcook.cn/Article/details/gzlpisivt.sHtML


<!-- 参考信息 -->