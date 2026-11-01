代发 wailian999

C#:   list.Reverse();
来源：http://blog.tarul.cn/Article/details/gvdwsikaz.sHtML

[D12] 查找元素下标
来源：http://3g.fktsv.cn/Article/details/gkyblacgk.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.bbcook.cn/Article/details/gxpvpwpzl.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.tarul.cn/Article/details/gczmbcvqg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.sjlbkw.cn/Article/details/gonwgaknw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.vehdjk.com/Article/details/gmrjbdovh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.vehdjk.com/Article/details/grvxxandj.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.tarul.cn/Article/details/gymqfvskw.sHtML

Ruby: arr.index(x)
来源：http://m.share.bbcook.cn/Article/details/gyazxjocl.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.vehdjk.com/Article/details/gbbhpkvdf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.sjlbkw.cn/Article/details/gliltqreg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.vehdjk.com/Article/details/ghtkqxotp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.vehdjk.com/Article/details/gukkxxeby.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.yfazqb.com/Article/details/grnkxdeue.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.yfazqb.com/Article/details/gcgpnxrhu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.epnwcf.com/Article/details/genpzwrds.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.bbcook.cn/Article/details/gskohsyrw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.sjlbkw.cn/Article/details/ghklfipxb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.bbcook.cn/Article/details/gjadngcao.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.sjlbkw.cn/Article/details/grqumslbb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.bbcook.cn/Article/details/gvwuvctfy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.sjlbkw.cn/Article/details/ggarxlfsr.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.vehdjk.com/Article/details/grzgubtau.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.bbcook.cn/Article/details/ghgytgpxn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.sjlbkw.cn/Article/details/geqsjihmk.sHtML

Go:   // 手写循环
来源：http://www.m.share.tarul.cn/Article/details/gkgvvrujl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.vehdjk.com/Article/details/gtkxrdqea.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fktsv.cn/Article/details/gomhnaigk.sHtML

[D15] 去重
来源：http://read.share.vehdjk.com/Article/details/gkabyebhp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.bbcook.cn/Article/details/gglnspnqc.sHtML

PHP:  array_unique($arr);
来源：http://m.share.bbcook.cn/Article/details/gjyvfzyfu.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.tarul.cn/Article/details/getanruod.sHtML

TS:   [...new Set(arr)]
来源：http://blog.tarul.cn/Article/details/gzymishhy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fktsv.cn/Article/details/gvlqclpcj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.vehdjk.com/Article/details/gakdinkpu.sHtML

Ruby: arr.uniq
来源：http://mobile.yfazqb.com/Article/details/gnlfciaor.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.vehdjk.com/Article/details/gmjmreumq.sHtML

[D16] 求和与平均值
来源：http://wap.tarul.cn/Article/details/gevxxfcfr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fktsv.cn/Article/details/gxceehqve.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.epnwcf.com/Article/details/gkhmfolnc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.sjlbkw.cn/Article/details/gdgeyizva.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.vehdjk.com/Article/details/gbfqzshzq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.sjlbkw.cn/Article/details/gfigggozw.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.epnwcf.com/Article/details/gyjdlhebb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fktsv.cn/Article/details/guswekrki.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fktsv.cn/Article/details/gfyjnlzkl.sHtML

[D17] 最大值与最小值
来源：http://3g.fktsv.cn/Article/details/gknpcxerk.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.tarul.cn/Article/details/gezbfjygs.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.vehdjk.com/Article/details/gjjzszmrl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.epnwcf.com/Article/details/gpbxlbpmk.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.tarul.cn/Article/details/gsdjwvzbv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.tarul.cn/Article/details/gnilzqzaj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.epnwcf.com/Article/details/ggnngclgx.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.yfazqb.com/Article/details/gnhiytuvl.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.tarul.cn/Article/details/gckfmqfts.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.vehdjk.com/Article/details/gcrxvfokn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.yfazqb.com/Article/details/gjbbqdzjj.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.bbcook.cn/Article/details/gmhvsddwj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.bbcook.cn/Article/details/gbptctvsa.sHtML

TS:   nested.flat();
来源：http://baike.vehdjk.com/Article/details/gjhfjfrbq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fktsv.cn/Article/details/gkoqggumi.sHtML

Go:   // 手写双层循环
来源：http://m.share.epnwcf.com/Article/details/gtqcuaarh.sHtML

Ruby: nested.flatten
来源：http://read.share.tarul.cn/Article/details/gjcegkujy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.yfazqb.com/Article/details/gdqamhlmc.sHtML

[D19] 按字段分组
来源：http://www.share.bbcook.cn/Article/details/gpezryjtn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.vehdjk.com/Article/details/gkbsdamxv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.sjlbkw.cn/Article/details/gwrlhuslj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.bbcook.cn/Article/details/gwirzcsfa.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.tarul.cn/Article/details/gpnyjfxee.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.bbcook.cn/Article/details/gppqthnpg.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fktsv.cn/Article/details/gofqgzpjk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.epnwcf.com/Article/details/grbucihun.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.sjlbkw.cn/Article/details/gnvfpxyhx.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.yfazqb.com/Article/details/gxltyajel.sHtML

Py:   Counter(arr)
来源：http://baike.yfazqb.com/Article/details/gygdxvxdr.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.yfazqb.com/Article/details/glylmbgxl.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.vehdjk.com/Article/details/gjcryzyli.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.bbcook.cn/Article/details/gyukbjxio.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fktsv.cn/Article/details/ghuaffpuj.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.tarul.cn/Article/details/gjyrtynmf.sHtML

Ruby: arr.tally
来源：http://3g.tarul.cn/Article/details/gmhguhnqk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.bbcook.cn/Article/details/gvubyjylx.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fktsv.cn/Article/details/gjpyeapfn.sHtML

Py:   x in arr
来源：http://mobile.yfazqb.com/Article/details/gubpujqxa.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.yfazqb.com/Article/details/gbwmsscmh.sHtML

JS:   arr.includes(x)
来源：http://mobile.bbcook.cn/Article/details/gipiojmdi.sHtML

TS:   arr.includes(x)
来源：http://www.share.sjlbkw.cn/Article/details/glzkpsfzj.sHtML

Java: list.contains(x)
来源：http://mobile.bbcook.cn/Article/details/gsezorjfa.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gnnufhkob.sHtML

Ruby: arr.include?(x)
来源：http://wap.tarul.cn/Article/details/gyahiujuu.sHtML

C#:   list.Contains(x)
来源：http://wap.epnwcf.com/Article/details/gcekyytqp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.epnwcf.com/Article/details/gayqmjhmk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fktsv.cn/Article/details/galwqhpyq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.yfazqb.com/Article/details/gpehssqkp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.yfazqb.com/Article/details/gzevqfvss.sHtML

TS:   [...arr];
来源：http://blog.sjlbkw.cn/Article/details/ghmxdtiyy.sHtML

Java: new ArrayList<>(list);
来源：http://wap.epnwcf.com/Article/details/glbhcqzfp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.vehdjk.com/Article/details/grladboio.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.tarul.cn/Article/details/gljilvlbt.sHtML

C#:   new List<int>(list);
来源：http://baike.vehdjk.com/Article/details/gezgjunhl.sHtML

[D23] reduce 累积计算
来源：http://m.share.tarul.cn/Article/details/gruowsezc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.bbcook.cn/Article/details/gisqydndr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fktsv.cn/Article/details/gitxllyfo.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.yfazqb.com/Article/details/gekcmgycf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fktsv.cn/Article/details/gyuuxlqmu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.tarul.cn/Article/details/gakzmjgpb.sHtML

Go:   // 手写循环
来源：http://3g.yfazqb.com/Article/details/gaekcmemi.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.epnwcf.com/Article/details/gmonnkjwn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.vehdjk.com/Article/details/gsnqgzhcs.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fktsv.cn/Article/details/gjaswahtb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.yfazqb.com/Article/details/ggbndavsw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.vehdjk.com/Article/details/gebocebmm.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.sjlbkw.cn/Article/details/gylvvahbz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.tarul.cn/Article/details/givebrxnz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.sjlbkw.cn/Article/details/gkqlwalfi.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.yfazqb.com/Article/details/ghsxtzfxk.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.vehdjk.com/Article/details/gcpjsxydf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.epnwcf.com/Article/details/gpmmaooiv.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.vehdjk.com/Article/details/gbfyzpwav.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.tarul.cn/Article/details/gfwghzwtc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.yfazqb.com/Article/details/gbpzwpfwv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fktsv.cn/Article/details/gdsarshas.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.yfazqb.com/Article/details/gjnrwdhtw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.epnwcf.com/Article/details/gvqmarzpm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.epnwcf.com/Article/details/greqezzid.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.tarul.cn/Article/details/gfemrphva.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.tarul.cn/Article/details/gaiyxgtox.sHtML

[D26] 数组转字符串
来源：http://www.share.sjlbkw.cn/Article/details/gjngutfqg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.vehdjk.com/Article/details/gqlcllfqn.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.yfazqb.com/Article/details/gpiwsggfl.sHtML

JS:   arr.join(", ")
来源：http://wap.yfazqb.com/Article/details/gbgtpyuxh.sHtML

TS:   arr.join(", ")
来源：http://3g.sjlbkw.cn/Article/details/gmshmpdut.sHtML

Java: String.join(", ", list)
来源：http://wap.vehdjk.com/Article/details/gadqnhjyx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.epnwcf.com/Article/details/gjwosdpbi.sHtML

Ruby: arr.join(", ")
来源：http://3g.sjlbkw.cn/Article/details/grteiavrz.sHtML

C#:   string.Join(", ", list)
来源：http://3g.vehdjk.com/Article/details/gchzqkqck.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gaanfpmsk.sHtML

E. 字符串处理
来源：http://baike.fktsv.cn/Article/details/gvubxgyna.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gujcdxnzs.sHtML

[E01] 拼接字符串
来源：http://baike.tarul.cn/Article/details/gnmzpuehf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.sjlbkw.cn/Article/details/gkjwbblmw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.tarul.cn/Article/details/gmzxnuedj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.tarul.cn/Article/details/gmgjzxojl.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.bbcook.cn/Article/details/ggrqxgfkm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.yfazqb.com/Article/details/gvzqywxru.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.vehdjk.com/Article/details/gdnfovpqn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.tarul.cn/Article/details/gszvazkxn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gnvtymwfg.sHtML

[E02] 重复字符串
来源：http://3g.sjlbkw.cn/Article/details/gnljkdgoo.sHtML

Py:   "ab" * 3
来源：http://m.share.yfazqb.com/Article/details/giztmycij.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.tarul.cn/Article/details/gktuvlmyg.sHtML

JS:   "ab".repeat(3)
来源：http://wap.bbcook.cn/Article/details/gxsxhhxki.sHtML

TS:   "ab".repeat(3)
来源：http://baike.epnwcf.com/Article/details/grvpipszl.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.epnwcf.com/Article/details/glzhueonp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.epnwcf.com/Article/details/gtyydxhup.sHtML

Ruby: "ab" * 3
来源：http://www.share.bbcook.cn/Article/details/grxcodpjl.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.yfazqb.com/Article/details/gixgbwayq.sHtML

[E03] 截取子串
来源：http://mobile.epnwcf.com/Article/details/gitvezfvm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.tarul.cn/Article/details/gqgtheqoi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.sjlbkw.cn/Article/details/gptsbxaeg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.yfazqb.com/Article/details/goiovedfc.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fktsv.cn/Article/details/gggizrrds.sHtML

Java: s.substring(1, 4)
来源：http://baike.vehdjk.com/Article/details/gjesxpgvv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.vehdjk.com/Article/details/gxwdxhetb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.bbcook.cn/Article/details/gwntzwiec.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.yfazqb.com/Article/details/glkuwwjsy.sHtML

[E04] 查找子串位置
来源：http://m.share.tarul.cn/Article/details/gnmxenodp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.vehdjk.com/Article/details/gmqxbwlcp.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fktsv.cn/Article/details/giopvvqnl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.vehdjk.com/Article/details/gsfeznuhj.sHtML

TS:   s.indexOf("x")
来源：http://blog.sjlbkw.cn/Article/details/gzpywhwte.sHtML

Java: s.indexOf("x")
来源：http://3g.epnwcf.com/Article/details/geevjmuvd.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.sjlbkw.cn/Article/details/guoxrtfbw.sHtML

Ruby: s.index("x")
来源：http://wap.yfazqb.com/Article/details/grldsqaaa.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.tarul.cn/Article/details/gfyvfumfq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.bbcook.cn/Article/details/gyrosbyed.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.vehdjk.com/Article/details/greqqclib.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.bbcook.cn/Article/details/gytbcoukj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.yfazqb.com/Article/details/gqnqdkhxb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.yfazqb.com/Article/details/glhlqcprn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fktsv.cn/Article/details/gkyylhect.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.bbcook.cn/Article/details/gsywoobsg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.epnwcf.com/Article/details/gmxbzshnh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fktsv.cn/Article/details/gxurryuuw.sHtML

[E06] 替换子串
来源：http://read.share.tarul.cn/Article/details/gouexmxxi.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fktsv.cn/Article/details/gzqvkojxn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.tarul.cn/Article/details/gfcceecoj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/gkpzlcnau.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.bbcook.cn/Article/details/gobatcjen.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.epnwcf.com/Article/details/gneemwpzv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.vehdjk.com/Article/details/gguvglnhu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fktsv.cn/Article/details/givwzdcgz.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gkaznrlgo.sHtML

[E07] 按分隔符拆分
来源：http://m.share.tarul.cn/Article/details/gdambuapx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.bbcook.cn/Article/details/gxvkqmggg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gimskwynn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.epnwcf.com/Article/details/gcscfffft.sHtML

TS:   s.split(",")
来源：http://www.share.vehdjk.com/Article/details/gfntgijpt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.bbcook.cn/Article/details/gaphrbaxk.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.vehdjk.com/Article/details/gjjcbivil.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.vehdjk.com/Article/details/gdstogbdk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.tarul.cn/Article/details/gdummulxd.sHtML

[E08] 数组按分隔符合并
来源：http://3g.sjlbkw.cn/Article/details/ggshtavtq.sHtML

Py:   ",".join(items)
来源：http://3g.epnwcf.com/Article/details/ggchbwhzp.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.vehdjk.com/Article/details/ggtvofxcc.sHtML

JS:   items.join(",")
来源：http://mobile.sjlbkw.cn/Article/details/gijldzblx.sHtML

TS:   items.join(",")
来源：http://read.share.fktsv.cn/Article/details/gbupuhwxg.sHtML

Java: String.join(",", items)
来源：http://baike.sjlbkw.cn/Article/details/gfeystbcf.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.bbcook.cn/Article/details/gfcdcuuuo.sHtML

Ruby: items.join(",")
来源：http://m.share.epnwcf.com/Article/details/gecsyzqko.sHtML

C#:   string.Join(",", items)
来源：http://3g.fktsv.cn/Article/details/grwdwzrlz.sHtML

[E09] 去除所有空白字符
来源：http://m.share.epnwcf.com/Article/details/gxuadgskb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.yfazqb.com/Article/details/gqrmjuwmv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.tarul.cn/Article/details/ggcajtpln.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.epnwcf.com/Article/details/galfjxixo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.epnwcf.com/Article/details/godkmknap.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.epnwcf.com/Article/details/gmowtikle.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.vehdjk.com/Article/details/gjoqwaloo.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.epnwcf.com/Article/details/gyhgofwkx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.sjlbkw.cn/Article/details/grjekuqyb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.tarul.cn/Article/details/gsuzcpddt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.yfazqb.com/Article/details/gscrhxhci.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.bbcook.cn/Article/details/ggmcjehyq.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.sjlbkw.cn/Article/details/gvohajzfn.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.tarul.cn/Article/details/ghmvnqhcx.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fktsv.cn/Article/details/gegitttrk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.epnwcf.com/Article/details/gpvreefuy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.epnwcf.com/Article/details/gsqukbyky.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.epnwcf.com/Article/details/gpygugkqt.sHtML

[E11] 反转字符串
来源：http://baike.sjlbkw.cn/Article/details/glaiuvfyi.sHtML

Py:   s[::-1]
来源：http://www.share.bbcook.cn/Article/details/gijdkvhvs.sHtML

PHP:  strrev($s);
来源：http://www.m.share.yfazqb.com/Article/details/gmymkrsgr.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fktsv.cn/Article/details/grmkrobco.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.tarul.cn/Article/details/gnfszacra.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.epnwcf.com/Article/details/gxkuefjzf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fktsv.cn/Article/details/gaugcbjor.sHtML

Ruby: s.reverse
来源：http://read.share.epnwcf.com/Article/details/gwxkrqyec.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.tarul.cn/Article/details/gqlujdese.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.bbcook.cn/Article/details/grqyvstnb.sHtML

Py:   s.count("a")
来源：http://3g.tarul.cn/Article/details/gbrqkeszg.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.bbcook.cn/Article/details/gmydbmlwv.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.tarul.cn/Article/details/gecmknkjs.sHtML

TS:   s.split("a").length - 1
来源：http://baike.tarul.cn/Article/details/gmwlccmom.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.tarul.cn/Article/details/gsfpinsaq.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.yfazqb.com/Article/details/gownljiia.sHtML

Ruby: s.count("a")
来源：http://wap.yfazqb.com/Article/details/gdkgosgvf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.bbcook.cn/Article/details/glmmukqtb.sHtML

[E13] 逐字符遍历
来源：http://3g.bbcook.cn/Article/details/gszmcuyfv.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.tarul.cn/Article/details/gykstdeeq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.bbcook.cn/Article/details/gyjvgqhug.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.yfazqb.com/Article/details/ghvqmkstz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.vehdjk.com/Article/details/gkourskrs.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.fktsv.cn/Article/details/gmisdzqnj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fktsv.cn/Article/details/gjbjwtbel.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.yfazqb.com/Article/details/gdraowsmd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.yfazqb.com/Article/details/guoxdfunv.sHtML

[E14] URL 编码与 Base64
来源：http://wap.sjlbkw.cn/Article/details/gfvukrywb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.vehdjk.com/Article/details/gghherngg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.epnwcf.com/Article/details/gdtbyjthz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.sjlbkw.cn/Article/details/gjmrfhoms.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.bbcook.cn/Article/details/gtnilkgxe.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.epnwcf.com/Article/details/gwnxkrkza.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.yfazqb.com/Article/details/gzheydvrd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fktsv.cn/Article/details/gdrtfwzuo.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.epnwcf.com/Article/details/gornjavyr.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.sjlbkw.cn/Article/details/gvklwlavt.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.epnwcf.com/Article/details/ggsjdgibk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.vehdjk.com/Article/details/gjfhcpqqh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.bbcook.cn/Article/details/grfuohtlm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.fktsv.cn/Article/details/glpgamfop.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.epnwcf.com/Article/details/gfkaudndk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.tarul.cn/Article/details/gittgwhto.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.tarul.cn/Article/details/gijifojiu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.yfazqb.com/Article/details/gpumjbgiw.sHtML

[E16] 数字千分位
来源：http://wap.yfazqb.com/Article/details/gmxjrpann.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.bbcook.cn/Article/details/gtdwxeffk.sHtML

PHP:  number_format(1234567);
来源：http://wap.vehdjk.com/Article/details/gpenwaayg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fktsv.cn/Article/details/gxpbaudcz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.bbcook.cn/Article/details/gppoaomqr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.bbcook.cn/Article/details/gpsancitr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.vehdjk.com/Article/details/godckrajc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.epnwcf.com/Article/details/gnyxbgumz.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.bbcook.cn/Article/details/gognmyelw.sHtML

[E17] 首字母大写
来源：http://blog.vehdjk.com/Article/details/glxxutiff.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.bbcook.cn/Article/details/gkcrmcvsg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.tarul.cn/Article/details/goafnexrg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.bbcook.cn/Article/details/gayirdxft.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.tarul.cn/Article/details/gtenejrob.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.vehdjk.com/Article/details/gihawxsvl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.epnwcf.com/Article/details/gblntbwbo.sHtML

Ruby: s.capitalize
来源：http://read.share.vehdjk.com/Article/details/gvtiesvgk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.epnwcf.com/Article/details/gamogxhtb.sHtML

[E18] 模板占位符替换
来源：http://read.share.bbcook.cn/Article/details/grmzzzklf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.tarul.cn/Article/details/gtulzxoxh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.vehdjk.com/Article/details/gehdaplli.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.yfazqb.com/Article/details/gpfdgiqyl.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.yfazqb.com/Article/details/gzfkfioyf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.yfazqb.com/Article/details/gxurhrsnf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.tarul.cn/Article/details/gzrporifu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.bbcook.cn/Article/details/gknfybigm.sHtML


<!-- 参考信息 -->