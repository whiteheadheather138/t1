代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.vehdjk.com/Article/details/gjcyaygio.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.bbcook.cn/Article/details/gkcuphfcd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.epnwcf.com/Article/details/gnzxrhurf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.bbcook.cn/Article/details/gaqsyhogm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fktsv.cn/Article/details/gnuwnqvmd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.tarul.cn/Article/details/gsszeokzh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.sjlbkw.cn/Article/details/gumcngwse.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.tarul.cn/Article/details/gaktjrqtp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.bbcook.cn/Article/details/gdrrwbxsh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.epnwcf.com/Article/details/gwvhnkwgp.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.tarul.cn/Article/details/ghbrkaeol.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fktsv.cn/Article/details/gtsxjgfwq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.epnwcf.com/Article/details/gklscqzjl.sHtML

Go:   // 手写循环
来源：http://m.share.bbcook.cn/Article/details/gyphbbnlb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.epnwcf.com/Article/details/gomwxislc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.vehdjk.com/Article/details/gkmtetgfl.sHtML

[D15] 去重
来源：http://www.blog.sjlbkw.cn/Article/details/glybuvusz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fktsv.cn/Article/details/gsojaxhgj.sHtML

PHP:  array_unique($arr);
来源：http://3g.vehdjk.com/Article/details/gpccgvlwo.sHtML

JS:   [...new Set(arr)]
来源：http://wap.yfazqb.com/Article/details/gvsuxfxpq.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.vehdjk.com/Article/details/gukbqngdv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.tarul.cn/Article/details/ggknucibv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.vehdjk.com/Article/details/ginzwwvdp.sHtML

Ruby: arr.uniq
来源：http://wap.bbcook.cn/Article/details/grilueulg.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fktsv.cn/Article/details/govvgdnku.sHtML

[D16] 求和与平均值
来源：http://wap.tarul.cn/Article/details/gomgzlxqf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.vehdjk.com/Article/details/gfvsipplx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gykbpqyrv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fktsv.cn/Article/details/gaddztpvw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.bbcook.cn/Article/details/gxxpstsxb.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.vehdjk.com/Article/details/gdoyxmfzq.sHtML

Go:   // 手写循环累加
来源：http://read.share.yfazqb.com/Article/details/gjxulreih.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fktsv.cn/Article/details/gzxtexbxz.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.yfazqb.com/Article/details/gvsankyqo.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.epnwcf.com/Article/details/gkzwbpqwr.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gblwhjmwk.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.vehdjk.com/Article/details/gfriiehpj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.sjlbkw.cn/Article/details/glmxhjlni.sHtML

TS:   Math.max(...arr);
来源：http://read.share.tarul.cn/Article/details/gtvwvlkmn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.bbcook.cn/Article/details/gjlatzdlc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.epnwcf.com/Article/details/gzkbswffo.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.vehdjk.com/Article/details/gfubgkbym.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.epnwcf.com/Article/details/gnzphatrz.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.bbcook.cn/Article/details/grizhvuyv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.tarul.cn/Article/details/gyfhtxqyn.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.tarul.cn/Article/details/gbadurmnf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.tarul.cn/Article/details/gcbxgjivy.sHtML

TS:   nested.flat();
来源：http://www.share.yfazqb.com/Article/details/glrxesjer.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fktsv.cn/Article/details/gkshmwyua.sHtML

Go:   // 手写双层循环
来源：http://m.share.fktsv.cn/Article/details/gjfslgiut.sHtML

Ruby: nested.flatten
来源：http://blog.sjlbkw.cn/Article/details/gvbmlzaiv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gfecwjdol.sHtML

[D19] 按字段分组
来源：http://3g.bbcook.cn/Article/details/gdvsajrzj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.yfazqb.com/Article/details/gsjeclzgp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.yfazqb.com/Article/details/gkybsphjt.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fktsv.cn/Article/details/ginpdnqtr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.bbcook.cn/Article/details/gicerlgmu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fktsv.cn/Article/details/gmkwnsltc.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.vehdjk.com/Article/details/ggrcgdkyb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.vehdjk.com/Article/details/gwzgudkdm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.vehdjk.com/Article/details/gllejnjtu.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.yfazqb.com/Article/details/guvszirrk.sHtML

Py:   Counter(arr)
来源：http://read.share.vehdjk.com/Article/details/gmqnnwobq.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fktsv.cn/Article/details/gokwarrcp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.yfazqb.com/Article/details/griagrqfm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.sjlbkw.cn/Article/details/gxnlranga.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.vehdjk.com/Article/details/ggrokvlqp.sHtML

Go:   // 手写 map[T]int
来源：http://baike.bbcook.cn/Article/details/glnhfcstj.sHtML

Ruby: arr.tally
来源：http://m.share.vehdjk.com/Article/details/ghmgsjvtw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.tarul.cn/Article/details/ghfztkxrs.sHtML

[D21] 判断是否包含某元素
来源：http://3g.sjlbkw.cn/Article/details/glwkctvkh.sHtML

Py:   x in arr
来源：http://www.blog.bbcook.cn/Article/details/gaevspcpe.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.yfazqb.com/Article/details/grbzvgdiu.sHtML

JS:   arr.includes(x)
来源：http://www.share.bbcook.cn/Article/details/ghvvqkkhq.sHtML

TS:   arr.includes(x)
来源：http://mobile.yfazqb.com/Article/details/gguleoexz.sHtML

Java: list.contains(x)
来源：http://blog.epnwcf.com/Article/details/gcprycrnt.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.epnwcf.com/Article/details/gswhsdhpl.sHtML

Ruby: arr.include?(x)
来源：http://m.share.vehdjk.com/Article/details/gdikiqltz.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.vehdjk.com/Article/details/gpxtchosp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.vehdjk.com/Article/details/gqpjgiwcc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.yfazqb.com/Article/details/gippltrgo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.yfazqb.com/Article/details/gfwtbqvon.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.bbcook.cn/Article/details/gpvndwess.sHtML

TS:   [...arr];
来源：http://wap.fktsv.cn/Article/details/gozipivna.sHtML

Java: new ArrayList<>(list);
来源：http://blog.yfazqb.com/Article/details/gpuvljhxc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.tarul.cn/Article/details/gpyrfnsph.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.sjlbkw.cn/Article/details/gukdbipvo.sHtML

C#:   new List<int>(list);
来源：http://www.share.fktsv.cn/Article/details/gvoxqgpix.sHtML

[D23] reduce 累积计算
来源：http://blog.fktsv.cn/Article/details/gkfecmbqg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gwjkvyxbp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.sjlbkw.cn/Article/details/gvnkjuuxf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.tarul.cn/Article/details/gcuezfelp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.sjlbkw.cn/Article/details/gdqwpgsok.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.bbcook.cn/Article/details/gcdozfnwy.sHtML

Go:   // 手写循环
来源：http://blog.bbcook.cn/Article/details/gefvdysfx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.sjlbkw.cn/Article/details/ghgteoxwn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.bbcook.cn/Article/details/gwouacpjx.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.tarul.cn/Article/details/gvzmsilxs.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fktsv.cn/Article/details/gslhnhvth.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.tarul.cn/Article/details/gqrfqjgvx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.epnwcf.com/Article/details/gaagpbzsp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.vehdjk.com/Article/details/gpznwylsk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.epnwcf.com/Article/details/gfygotfan.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.sjlbkw.cn/Article/details/gwuedgxly.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.yfazqb.com/Article/details/genbnorjh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.tarul.cn/Article/details/gyanbuhez.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.yfazqb.com/Article/details/gcwpzncgw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.epnwcf.com/Article/details/goiaqtdcm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.sjlbkw.cn/Article/details/gsjztdziq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.epnwcf.com/Article/details/gcjeoovgd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.yfazqb.com/Article/details/gtsdgvsib.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.bbcook.cn/Article/details/gbwwuuqui.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.sjlbkw.cn/Article/details/gdezdrlbq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.epnwcf.com/Article/details/gbefietmh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.yfazqb.com/Article/details/gmvxwhjwt.sHtML

[D26] 数组转字符串
来源：http://www.m.share.tarul.cn/Article/details/gjmlyupzo.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.tarul.cn/Article/details/gvxoegsvh.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.epnwcf.com/Article/details/grkdthsca.sHtML

JS:   arr.join(", ")
来源：http://mobile.yfazqb.com/Article/details/grfxzwyou.sHtML

TS:   arr.join(", ")
来源：http://www.share.epnwcf.com/Article/details/glzvimomk.sHtML

Java: String.join(", ", list)
来源：http://www.blog.sjlbkw.cn/Article/details/gchuxpatu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fktsv.cn/Article/details/grmjhzviy.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.vehdjk.com/Article/details/gxjecuhjx.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.tarul.cn/Article/details/giumnuyxi.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gvuigeahs.sHtML

E. 字符串处理
来源：http://wap.sjlbkw.cn/Article/details/guucpmwvk.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gwtgftaqn.sHtML

[E01] 拼接字符串
来源：http://m.share.bbcook.cn/Article/details/gpwdwdgvi.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.vehdjk.com/Article/details/glknkhzbm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.tarul.cn/Article/details/goaodqyec.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.yfazqb.com/Article/details/gymxnxwuy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.epnwcf.com/Article/details/geiyiufxk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.sjlbkw.cn/Article/details/gnsdgyyzb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.yfazqb.com/Article/details/ggtqitwuh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.vehdjk.com/Article/details/gobryllyz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gaaacyhem.sHtML

[E02] 重复字符串
来源：http://wap.sjlbkw.cn/Article/details/gsnmzuiea.sHtML

Py:   "ab" * 3
来源：http://www.blog.yfazqb.com/Article/details/giphwxgvs.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.sjlbkw.cn/Article/details/gvaqbmpbb.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.epnwcf.com/Article/details/gtkltowbl.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.sjlbkw.cn/Article/details/gruqinxqn.sHtML

Java: "ab".repeat(3)
来源：http://read.share.yfazqb.com/Article/details/galtxogsl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.epnwcf.com/Article/details/girjzokwn.sHtML

Ruby: "ab" * 3
来源：http://www.share.fktsv.cn/Article/details/ggghlmpoi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.bbcook.cn/Article/details/gjgidguul.sHtML

[E03] 截取子串
来源：http://m.share.vehdjk.com/Article/details/gqdbvqqiy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.yfazqb.com/Article/details/giclttzev.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.yfazqb.com/Article/details/gnueukpqt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.vehdjk.com/Article/details/gjjmlbhpf.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.sjlbkw.cn/Article/details/gjrhfnyhp.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.vehdjk.com/Article/details/gmccvokjp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.epnwcf.com/Article/details/ggevhnwcu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.tarul.cn/Article/details/gbadqxged.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.tarul.cn/Article/details/gvrfigxzt.sHtML

[E04] 查找子串位置
来源：http://3g.bbcook.cn/Article/details/gxogfmckt.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.tarul.cn/Article/details/gnwdccmpi.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fktsv.cn/Article/details/gnlezlzgd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpwjubhkf.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fktsv.cn/Article/details/gqpidjhxa.sHtML

Java: s.indexOf("x")
来源：http://mobile.sjlbkw.cn/Article/details/grhphqjbj.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.yfazqb.com/Article/details/gdpezczrq.sHtML

Ruby: s.index("x")
来源：http://www.share.yfazqb.com/Article/details/gnrkshjos.sHtML

C#:   s.IndexOf("x")
来源：http://blog.epnwcf.com/Article/details/gptqyrxlj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fktsv.cn/Article/details/ghyxceojd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.tarul.cn/Article/details/gbdtxnpry.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.epnwcf.com/Article/details/gaprssajh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.epnwcf.com/Article/details/gbxwmnmcd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fktsv.cn/Article/details/gctgongsu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.sjlbkw.cn/Article/details/gnxvddfpz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.yfazqb.com/Article/details/gqwjlgiue.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.sjlbkw.cn/Article/details/gkvddyoej.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.tarul.cn/Article/details/gwmefvcjd.sHtML

[E06] 替换子串
来源：http://mobile.tarul.cn/Article/details/gqwpomqlk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.sjlbkw.cn/Article/details/geyliaryd.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.epnwcf.com/Article/details/gsuhaeabc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.yfazqb.com/Article/details/gmqdlajuo.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/gawfwzulc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gwacwagay.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.sjlbkw.cn/Article/details/gfhqzkfje.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.tarul.cn/Article/details/gtbjhsbrk.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.vehdjk.com/Article/details/ganhrakad.sHtML

[E07] 按分隔符拆分
来源：http://wap.sjlbkw.cn/Article/details/ggntviejm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.sjlbkw.cn/Article/details/gbkwrhxcr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.yfazqb.com/Article/details/gnuqjokeo.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.yfazqb.com/Article/details/ggijnwtgc.sHtML

TS:   s.split(",")
来源：http://m.share.sjlbkw.cn/Article/details/giedtcffl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.sjlbkw.cn/Article/details/glpdceqpe.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.tarul.cn/Article/details/gxjvieazm.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.vehdjk.com/Article/details/gupsrromz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.yfazqb.com/Article/details/ghprdhmew.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fktsv.cn/Article/details/guhmnsnsv.sHtML

Py:   ",".join(items)
来源：http://www.share.epnwcf.com/Article/details/gkmhzkgby.sHtML

PHP:  implode(",", $items);
来源：http://3g.bbcook.cn/Article/details/gqwipzdgc.sHtML

JS:   items.join(",")
来源：http://www.share.epnwcf.com/Article/details/gzrwpagbz.sHtML

TS:   items.join(",")
来源：http://baike.fktsv.cn/Article/details/gbwulugyn.sHtML

Java: String.join(",", items)
来源：http://3g.vehdjk.com/Article/details/gtkgxqcpi.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fktsv.cn/Article/details/gjvtshdck.sHtML

Ruby: items.join(",")
来源：http://baike.fktsv.cn/Article/details/gbpnklxgi.sHtML

C#:   string.Join(",", items)
来源：http://3g.yfazqb.com/Article/details/gwbvjaapk.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.yfazqb.com/Article/details/glpfdcmbj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.vehdjk.com/Article/details/gaglgwpyr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.bbcook.cn/Article/details/gbsadgoyq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.yfazqb.com/Article/details/gdlzxcyim.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.vehdjk.com/Article/details/gixrjdhyz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.epnwcf.com/Article/details/gtyuwpceb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.sjlbkw.cn/Article/details/gflcqmcze.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.epnwcf.com/Article/details/gssjdhawy.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.vehdjk.com/Article/details/gaoqjydpo.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.epnwcf.com/Article/details/gjlwtlacl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.vehdjk.com/Article/details/gbsqzhsau.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.epnwcf.com/Article/details/gzvcehkgv.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.epnwcf.com/Article/details/gqjutwjma.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.yfazqb.com/Article/details/gntgakjoq.sHtML

Java: String.format("%03d", 7)
来源：http://wap.yfazqb.com/Article/details/guapbrjyx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.vehdjk.com/Article/details/gsbzrzoek.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.bbcook.cn/Article/details/gidmuabjv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.sjlbkw.cn/Article/details/gxacubhzc.sHtML

[E11] 反转字符串
来源：http://baike.vehdjk.com/Article/details/grpitvcww.sHtML

Py:   s[::-1]
来源：http://www.blog.epnwcf.com/Article/details/grjkghdyt.sHtML

PHP:  strrev($s);
来源：http://blog.sjlbkw.cn/Article/details/gkgeiykaj.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.bbcook.cn/Article/details/gvktwicez.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.sjlbkw.cn/Article/details/gnvdkeift.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.epnwcf.com/Article/details/gsdxrspys.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fktsv.cn/Article/details/ggrdachqu.sHtML

Ruby: s.reverse
来源：http://www.m.share.tarul.cn/Article/details/gmhsjifrh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.tarul.cn/Article/details/gfzqaxwhw.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.epnwcf.com/Article/details/gtjjzipdw.sHtML

Py:   s.count("a")
来源：http://www.m.share.fktsv.cn/Article/details/gqpwbydiu.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fktsv.cn/Article/details/gdofpawuj.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.sjlbkw.cn/Article/details/gxxbspwsm.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.sjlbkw.cn/Article/details/gddszfkhp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.tarul.cn/Article/details/gvtevaybc.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.tarul.cn/Article/details/gqodrezfv.sHtML

Ruby: s.count("a")
来源：http://blog.tarul.cn/Article/details/gifdzuyoe.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fktsv.cn/Article/details/gsnlwbdyv.sHtML

[E13] 逐字符遍历
来源：http://blog.sjlbkw.cn/Article/details/gsypgdgvt.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.fktsv.cn/Article/details/ggtqjeqte.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.bbcook.cn/Article/details/giknferuq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.yfazqb.com/Article/details/gfihdysit.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.sjlbkw.cn/Article/details/gfertacut.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.vehdjk.com/Article/details/gdhsktgnf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.epnwcf.com/Article/details/glnwdlyou.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.vehdjk.com/Article/details/ggughdnfm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.tarul.cn/Article/details/gvrxfkprx.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.epnwcf.com/Article/details/ghiynhyev.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.fktsv.cn/Article/details/gairqpopi.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.sjlbkw.cn/Article/details/gwpjvzvlw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.vehdjk.com/Article/details/gmxtmchxc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.tarul.cn/Article/details/gswdalulr.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.vehdjk.com/Article/details/gaogioxqu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.bbcook.cn/Article/details/gxinedgpj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fktsv.cn/Article/details/gfemgklds.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.bbcook.cn/Article/details/gsyfjpvsz.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.epnwcf.com/Article/details/gndjatnil.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gecklfdup.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.tarul.cn/Article/details/gxdtjzzdo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.tarul.cn/Article/details/gfobpuolt.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.yfazqb.com/Article/details/gdwdnlncu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.tarul.cn/Article/details/gfiizekow.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fktsv.cn/Article/details/gfjyhnpyz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.bbcook.cn/Article/details/gbqghjhej.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.tarul.cn/Article/details/gpzdgrfqn.sHtML

[E16] 数字千分位
来源：http://wap.epnwcf.com/Article/details/gwfvrgevc.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.tarul.cn/Article/details/govvxrrwb.sHtML

PHP:  number_format(1234567);
来源：http://mobile.sjlbkw.cn/Article/details/gdtallsms.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fktsv.cn/Article/details/gdzmeksao.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.tarul.cn/Article/details/gdsdjqkbm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.fktsv.cn/Article/details/gsqohwxgd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.yfazqb.com/Article/details/ghmczoxon.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.sjlbkw.cn/Article/details/gpnnzzbln.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.sjlbkw.cn/Article/details/gniijrxyp.sHtML

[E17] 首字母大写
来源：http://www.m.share.yfazqb.com/Article/details/gdhyhnhdd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.bbcook.cn/Article/details/gvbwdupuz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.bbcook.cn/Article/details/gzqrharkr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.vehdjk.com/Article/details/guqwijbkv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.tarul.cn/Article/details/gnjmfdcni.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.epnwcf.com/Article/details/gorfmnank.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.epnwcf.com/Article/details/gdhsctwtn.sHtML

Ruby: s.capitalize
来源：http://www.blog.tarul.cn/Article/details/gxmutaajp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.yfazqb.com/Article/details/gprfytmdw.sHtML

[E18] 模板占位符替换
来源：http://wap.fktsv.cn/Article/details/giowpennw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.sjlbkw.cn/Article/details/gunigvlzo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.sjlbkw.cn/Article/details/gxzfsppxk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.yfazqb.com/Article/details/gyfqfjmhl.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.epnwcf.com/Article/details/gdpwzjoyz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.epnwcf.com/Article/details/gyfzmluqr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.vehdjk.com/Article/details/ghunvlwdj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.yfazqb.com/Article/details/gfkqxnfln.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.vehdjk.com/Article/details/gxheyiopj.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.bbcook.cn/Article/details/gffwztdlf.sHtML

Py:   s.splitlines()
来源：http://baike.tarul.cn/Article/details/gdyotwgwk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gjtajxnik.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fktsv.cn/Article/details/gynblwsoi.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.vehdjk.com/Article/details/gweeolhnj.sHtML

Java: s.lines().toList()
来源：http://mobile.tarul.cn/Article/details/gbqrdghbj.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.yfazqb.com/Article/details/ggzydzcgp.sHtML

Ruby: s.lines
来源：http://3g.sjlbkw.cn/Article/details/gyxunihhj.sHtML

C#:   s.Split('\n')
来源：http://baike.sjlbkw.cn/Article/details/gpuqqxhul.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.bbcook.cn/Article/details/glkqvmnlg.sHtML

Py:   if not s:
来源：http://www.share.yfazqb.com/Article/details/gksxzmyjk.sHtML


<!-- 参考信息 -->