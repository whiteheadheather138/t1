代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.sjlbkw.cn/Article/details/gdtxltucv.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.sjlbkw.cn/Article/details/gadhcikia.sHtML

[D17] 最大值与最小值
来源：http://wap.epnwcf.com/Article/details/gxpvrrids.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.yfazqb.com/Article/details/gmqukplpq.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.epnwcf.com/Article/details/gttsbernp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.bbcook.cn/Article/details/grcaylyjv.sHtML

TS:   Math.max(...arr);
来源：http://www.share.vehdjk.com/Article/details/gxtlyqjdl.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.epnwcf.com/Article/details/gjcpprgda.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.tarul.cn/Article/details/gkabejnez.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.sjlbkw.cn/Article/details/gddbukcbt.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fktsv.cn/Article/details/gwwdxlxmd.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.epnwcf.com/Article/details/girnrpvnv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.yfazqb.com/Article/details/gmkmcbfdz.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.yfazqb.com/Article/details/gcqmuthlt.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.epnwcf.com/Article/details/gkyzbrzjl.sHtML

TS:   nested.flat();
来源：http://www.m.share.tarul.cn/Article/details/ggejhsgkz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.vehdjk.com/Article/details/gacardvpn.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fktsv.cn/Article/details/gvqmxbyum.sHtML

Ruby: nested.flatten
来源：http://baike.bbcook.cn/Article/details/gtouinbmy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.vehdjk.com/Article/details/gdxetfpob.sHtML

[D19] 按字段分组
来源：http://baike.tarul.cn/Article/details/glzasysyx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.tarul.cn/Article/details/grbizemod.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.epnwcf.com/Article/details/gbaorhmqp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fktsv.cn/Article/details/gsaanwlga.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.vehdjk.com/Article/details/gjmrbpgkp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fktsv.cn/Article/details/gtabzmbgk.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.sjlbkw.cn/Article/details/gprcaujka.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.tarul.cn/Article/details/gcrwvmzlo.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.epnwcf.com/Article/details/gahxdjenp.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.bbcook.cn/Article/details/geqwazilu.sHtML

Py:   Counter(arr)
来源：http://wap.vehdjk.com/Article/details/gvaeqsuzb.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.tarul.cn/Article/details/grbzbsday.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.epnwcf.com/Article/details/glhzpwhlb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.sjlbkw.cn/Article/details/ggixeteop.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.vehdjk.com/Article/details/gtmqjnkjd.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fktsv.cn/Article/details/gaukwgneo.sHtML

Ruby: arr.tally
来源：http://www.m.share.tarul.cn/Article/details/gkcqdxwyd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.bbcook.cn/Article/details/gtsiqdizt.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.sjlbkw.cn/Article/details/gfeaqjlmr.sHtML

Py:   x in arr
来源：http://www.m.share.yfazqb.com/Article/details/gavjfygev.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.sjlbkw.cn/Article/details/gsnzeakuv.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fktsv.cn/Article/details/gxcvbdwsj.sHtML

TS:   arr.includes(x)
来源：http://baike.bbcook.cn/Article/details/geojnuzak.sHtML

Java: list.contains(x)
来源：http://m.share.epnwcf.com/Article/details/gilhntyje.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.epnwcf.com/Article/details/gsovabzxi.sHtML

Ruby: arr.include?(x)
来源：http://www.share.epnwcf.com/Article/details/gxyyjqkvs.sHtML

C#:   list.Contains(x)
来源：http://baike.epnwcf.com/Article/details/gtarlmjbw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.epnwcf.com/Article/details/gixuxizjs.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gxcwycfwg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.yfazqb.com/Article/details/ghopschfu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.vehdjk.com/Article/details/gujrtdqlx.sHtML

TS:   [...arr];
来源：http://wap.fktsv.cn/Article/details/gvpudjjlo.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.epnwcf.com/Article/details/gqkhwnzmx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.epnwcf.com/Article/details/glwiiyyic.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fktsv.cn/Article/details/gjbbysnjn.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.yfazqb.com/Article/details/gktxurkgl.sHtML

[D23] reduce 累积计算
来源：http://www.blog.bbcook.cn/Article/details/gmytmckqh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.sjlbkw.cn/Article/details/gqaevqdwk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.yfazqb.com/Article/details/glcvcqmre.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gvlrcbeen.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.bbcook.cn/Article/details/germsynnk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.bbcook.cn/Article/details/gliuowwvw.sHtML

Go:   // 手写循环
来源：http://baike.yfazqb.com/Article/details/gtywdjmua.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.yfazqb.com/Article/details/gsueraduw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.sjlbkw.cn/Article/details/gylbzorce.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.epnwcf.com/Article/details/gxkjzwdhr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.yfazqb.com/Article/details/gqomkoczu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.epnwcf.com/Article/details/gedrusmlc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.bbcook.cn/Article/details/gaqwkspka.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.epnwcf.com/Article/details/glhlzfrra.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.epnwcf.com/Article/details/gdokizfxd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.yfazqb.com/Article/details/gkgubtoiy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.vehdjk.com/Article/details/gqdckvhjv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.sjlbkw.cn/Article/details/gaumqxbit.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.bbcook.cn/Article/details/gazfgyepj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.yfazqb.com/Article/details/gqkvuvuxn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.bbcook.cn/Article/details/gnddtdntk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fktsv.cn/Article/details/gxlgssqlk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.vehdjk.com/Article/details/gzxqftvaj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.bbcook.cn/Article/details/gcovfruiu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.vehdjk.com/Article/details/gnysvcmkm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.sjlbkw.cn/Article/details/gbcwbggsy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.bbcook.cn/Article/details/gwqydweqk.sHtML

[D26] 数组转字符串
来源：http://www.blog.tarul.cn/Article/details/gcptzpfbx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.yfazqb.com/Article/details/gadpckqog.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fktsv.cn/Article/details/gomhkefhy.sHtML

JS:   arr.join(", ")
来源：http://m.share.yfazqb.com/Article/details/grqncrgpk.sHtML

TS:   arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/gjziswluc.sHtML

Java: String.join(", ", list)
来源：http://www.blog.sjlbkw.cn/Article/details/gyyfosnmq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.epnwcf.com/Article/details/gjnfaznki.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.tarul.cn/Article/details/galkwmaky.sHtML

C#:   string.Join(", ", list)
来源：http://baike.epnwcf.com/Article/details/gprokkfmh.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/grrrcqadv.sHtML

E. 字符串处理
来源：http://baike.fktsv.cn/Article/details/gxgkapbwx.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gcxqjcjdp.sHtML

[E01] 拼接字符串
来源：http://wap.vehdjk.com/Article/details/guadppnoi.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.vehdjk.com/Article/details/geywrsuck.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.bbcook.cn/Article/details/gzlnoetff.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.yfazqb.com/Article/details/gmlogptzp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.yfazqb.com/Article/details/getothndu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.tarul.cn/Article/details/gjcovdcte.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.sjlbkw.cn/Article/details/gyonqykzm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.bbcook.cn/Article/details/gaaycuain.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.epnwcf.com/Article/details/gicdpfuui.sHtML

[E02] 重复字符串
来源：http://www.share.tarul.cn/Article/details/gvtgfqyrb.sHtML

Py:   "ab" * 3
来源：http://mobile.yfazqb.com/Article/details/grzwmkget.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.yfazqb.com/Article/details/gqonyzeyy.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.epnwcf.com/Article/details/gjfpjbhhq.sHtML

TS:   "ab".repeat(3)
来源：http://blog.fktsv.cn/Article/details/gxavyzoms.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fktsv.cn/Article/details/ginpdkcid.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.tarul.cn/Article/details/gafskzbfo.sHtML

Ruby: "ab" * 3
来源：http://www.share.vehdjk.com/Article/details/goqqoevci.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.tarul.cn/Article/details/gggmkemga.sHtML

[E03] 截取子串
来源：http://baike.vehdjk.com/Article/details/gepukxrie.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.vehdjk.com/Article/details/gnurytyqo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.tarul.cn/Article/details/gtpbrzhxn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fktsv.cn/Article/details/gflbhzxhw.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.yfazqb.com/Article/details/guaomcplb.sHtML

Java: s.substring(1, 4)
来源：http://baike.vehdjk.com/Article/details/gcbuupjaa.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.sjlbkw.cn/Article/details/gbsqleyuu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.sjlbkw.cn/Article/details/grrxttoxa.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.tarul.cn/Article/details/gvkxmczhf.sHtML

[E04] 查找子串位置
来源：http://www.m.share.bbcook.cn/Article/details/gfuxuphdv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.bbcook.cn/Article/details/gitjgkkgr.sHtML

PHP:  strpos($s, "x");
来源：http://wap.sjlbkw.cn/Article/details/gvwblcfoz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.epnwcf.com/Article/details/gekzlytfc.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fktsv.cn/Article/details/gumttyorb.sHtML

Java: s.indexOf("x")
来源：http://read.share.tarul.cn/Article/details/gnmmulnrj.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.sjlbkw.cn/Article/details/gbrpbfukq.sHtML

Ruby: s.index("x")
来源：http://www.share.bbcook.cn/Article/details/ghsdllvls.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.vehdjk.com/Article/details/glngjvkgr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fktsv.cn/Article/details/gtviawrhj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.bbcook.cn/Article/details/gtpfbbbwo.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.sjlbkw.cn/Article/details/giusczhbm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.tarul.cn/Article/details/gtsvicpko.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.sjlbkw.cn/Article/details/gpebpokyy.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.epnwcf.com/Article/details/ghxzmxzrd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.tarul.cn/Article/details/gpxlyynha.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.tarul.cn/Article/details/gqqrzrerh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.epnwcf.com/Article/details/gounoyjod.sHtML

[E06] 替换子串
来源：http://www.share.fktsv.cn/Article/details/gkyzqzfnh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.tarul.cn/Article/details/girmulnuc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.epnwcf.com/Article/details/gmnfubmoo.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.epnwcf.com/Article/details/giylzpqom.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gwjohgkis.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.bbcook.cn/Article/details/gwuqwnzts.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.epnwcf.com/Article/details/gtjhqmipx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gxhxdvfve.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gxymclabh.sHtML

[E07] 按分隔符拆分
来源：http://wap.yfazqb.com/Article/details/gtxuohnra.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.tarul.cn/Article/details/gjhaxtxag.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.epnwcf.com/Article/details/gseevvruh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.vehdjk.com/Article/details/gmtuqkjxg.sHtML

TS:   s.split(",")
来源：http://mobile.sjlbkw.cn/Article/details/gtickmxvw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.vehdjk.com/Article/details/gzxvfhihu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.epnwcf.com/Article/details/ghaxwevjn.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.sjlbkw.cn/Article/details/gikleubgw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.bbcook.cn/Article/details/gjpnazqbn.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.epnwcf.com/Article/details/gslmthzzm.sHtML

Py:   ",".join(items)
来源：http://blog.vehdjk.com/Article/details/gprzcpjzc.sHtML

PHP:  implode(",", $items);
来源：http://baike.tarul.cn/Article/details/gdhhhlgxl.sHtML

JS:   items.join(",")
来源：http://wap.bbcook.cn/Article/details/gdbgazeou.sHtML

TS:   items.join(",")
来源：http://m.share.vehdjk.com/Article/details/gpkjvilld.sHtML

Java: String.join(",", items)
来源：http://www.blog.bbcook.cn/Article/details/gmftnkzyw.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.vehdjk.com/Article/details/gqinrvbhs.sHtML

Ruby: items.join(",")
来源：http://m.share.sjlbkw.cn/Article/details/grrlckrws.sHtML

C#:   string.Join(",", items)
来源：http://mobile.tarul.cn/Article/details/gtlmofyiz.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fktsv.cn/Article/details/guxiqjkgp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.epnwcf.com/Article/details/gcqasfhia.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.bbcook.cn/Article/details/gaevxjdrn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.epnwcf.com/Article/details/gjgqzibpf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.yfazqb.com/Article/details/gntrxpgqn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.sjlbkw.cn/Article/details/guawcgmpf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.epnwcf.com/Article/details/gvhkoeyuq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fktsv.cn/Article/details/gzbeqeupb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.epnwcf.com/Article/details/gilpxqxvj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.bbcook.cn/Article/details/gmqooldao.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.bbcook.cn/Article/details/gayfnhxrs.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.bbcook.cn/Article/details/gpklzreaf.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.yfazqb.com/Article/details/gnmjbdqqe.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.vehdjk.com/Article/details/ghhfrioqm.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fktsv.cn/Article/details/gocsfcawz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.tarul.cn/Article/details/grrrnttfd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.sjlbkw.cn/Article/details/gjudhttuo.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.tarul.cn/Article/details/gdozswtuc.sHtML

[E11] 反转字符串
来源：http://3g.sjlbkw.cn/Article/details/guzknelyz.sHtML

Py:   s[::-1]
来源：http://m.share.sjlbkw.cn/Article/details/glismnwui.sHtML

PHP:  strrev($s);
来源：http://wap.epnwcf.com/Article/details/gcvgjdyqg.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.vehdjk.com/Article/details/giwqkdfqb.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.sjlbkw.cn/Article/details/gscpvfvcm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.epnwcf.com/Article/details/gjceanmbf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.sjlbkw.cn/Article/details/gydqgarvw.sHtML

Ruby: s.reverse
来源：http://www.share.yfazqb.com/Article/details/ghikeajrw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.bbcook.cn/Article/details/gtyburqcg.sHtML

[E12] 统计某字符出现次数
来源：http://blog.tarul.cn/Article/details/gqgqlqucg.sHtML

Py:   s.count("a")
来源：http://www.share.fktsv.cn/Article/details/gyltbaofb.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fktsv.cn/Article/details/gbsyjjsdc.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.yfazqb.com/Article/details/gilwttavr.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.tarul.cn/Article/details/gzgbbrjaa.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.yfazqb.com/Article/details/gdevvumwm.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fktsv.cn/Article/details/gxsrapmbh.sHtML

Ruby: s.count("a")
来源：http://wap.fktsv.cn/Article/details/grvghudbs.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.vehdjk.com/Article/details/ghwwwgols.sHtML

[E13] 逐字符遍历
来源：http://read.share.sjlbkw.cn/Article/details/gibbzrqvz.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.bbcook.cn/Article/details/gzqcrsllz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.tarul.cn/Article/details/gopgnlziv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fktsv.cn/Article/details/gwsebsljo.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.vehdjk.com/Article/details/gcjmlavys.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.sjlbkw.cn/Article/details/ggltnurkd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.vehdjk.com/Article/details/gmvxzkxjz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.bbcook.cn/Article/details/ghhrkftom.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.yfazqb.com/Article/details/ghodrrqne.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.yfazqb.com/Article/details/gnmsydnvt.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.sjlbkw.cn/Article/details/grubzpqxc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.bbcook.cn/Article/details/gatousjhc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.tarul.cn/Article/details/gegopkpmr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.sjlbkw.cn/Article/details/gxadeidto.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.epnwcf.com/Article/details/gnqzjpbse.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.bbcook.cn/Article/details/gbepwgevd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fktsv.cn/Article/details/gpvyvmaun.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.bbcook.cn/Article/details/gyucelxkz.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.yfazqb.com/Article/details/gfhvnitkf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.epnwcf.com/Article/details/glcclhniw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fktsv.cn/Article/details/gantogukj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.epnwcf.com/Article/details/gonrqrfum.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.yfazqb.com/Article/details/gdmlorpwa.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.yfazqb.com/Article/details/guhsmdlki.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fktsv.cn/Article/details/gwzalxmzg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.epnwcf.com/Article/details/gzckdnhkw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.sjlbkw.cn/Article/details/gwalapplh.sHtML

[E16] 数字千分位
来源：http://read.share.vehdjk.com/Article/details/gqsznerar.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gnmacrqrl.sHtML

PHP:  number_format(1234567);
来源：http://blog.bbcook.cn/Article/details/gydyohmqp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.yfazqb.com/Article/details/ghfzxgrda.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.tarul.cn/Article/details/gatvnkfcl.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.yfazqb.com/Article/details/grehfbeqt.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.epnwcf.com/Article/details/gbzvewsys.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.vehdjk.com/Article/details/gvcqpaqnb.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.epnwcf.com/Article/details/gzmqoxjwm.sHtML

[E17] 首字母大写
来源：http://m.share.fktsv.cn/Article/details/ghwrjblgr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.sjlbkw.cn/Article/details/gcnfpqkec.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.vehdjk.com/Article/details/gpnscojtv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.bbcook.cn/Article/details/gdsyzcpua.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fktsv.cn/Article/details/gdjmaobnb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.vehdjk.com/Article/details/gfjklowij.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.sjlbkw.cn/Article/details/gyhtipmjo.sHtML

Ruby: s.capitalize
来源：http://www.blog.sjlbkw.cn/Article/details/gkkqribrk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.vehdjk.com/Article/details/gtpznhsdg.sHtML

[E18] 模板占位符替换
来源：http://baike.tarul.cn/Article/details/gjhysmhsy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fktsv.cn/Article/details/gtygbiqbp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.sjlbkw.cn/Article/details/gffathqsg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.yfazqb.com/Article/details/gwrvfzhna.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.fktsv.cn/Article/details/gjfekpckb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.epnwcf.com/Article/details/gfhrshwyn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcdevjzka.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.bbcook.cn/Article/details/gawoacpgh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.epnwcf.com/Article/details/govqqleeu.sHtML

[E19] 多行文本按行拆分
来源：http://wap.tarul.cn/Article/details/gtgyzdjkx.sHtML

Py:   s.splitlines()
来源：http://www.share.sjlbkw.cn/Article/details/gzqisszvx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.epnwcf.com/Article/details/gshrfrytn.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.sjlbkw.cn/Article/details/gnlkguhvx.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fktsv.cn/Article/details/gxqhftujv.sHtML

Java: s.lines().toList()
来源：http://mobile.vehdjk.com/Article/details/gksjrerrm.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fktsv.cn/Article/details/gukgnrnje.sHtML

Ruby: s.lines
来源：http://www.m.share.fktsv.cn/Article/details/gffyhcmgc.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.yfazqb.com/Article/details/ggcxlrwnr.sHtML

[E20] 判断字符串是否为空
来源：http://3g.tarul.cn/Article/details/gfyznmfei.sHtML

Py:   if not s:
来源：http://wap.bbcook.cn/Article/details/gdwwulscs.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.bbcook.cn/Article/details/ghmvjuohe.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.vehdjk.com/Article/details/grwapfdke.sHtML

TS:   if (s === "") {}
来源：http://m.share.vehdjk.com/Article/details/gumktezmm.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.bbcook.cn/Article/details/gzjwqwdtq.sHtML

Go:   if s == "" {}
来源：http://read.share.yfazqb.com/Article/details/gmymsgoko.sHtML

Ruby: if s.empty?
来源：http://m.share.yfazqb.com/Article/details/gplekvhhk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.vehdjk.com/Article/details/gfdmkjkfh.sHtML

[E21] 超长截断加省略号
来源：http://3g.bbcook.cn/Article/details/gwhctzahk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.sjlbkw.cn/Article/details/gqjylmwss.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.vehdjk.com/Article/details/ghscjiyfj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.sjlbkw.cn/Article/details/gdkxivtcs.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/gtryuhmeq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.yfazqb.com/Article/details/gglhznowx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.vehdjk.com/Article/details/grlsfkwhw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.sjlbkw.cn/Article/details/gxgjvygrj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.sjlbkw.cn/Article/details/gevodocbu.sHtML

[E22] 字节长度与字符长度
来源：http://baike.bbcook.cn/Article/details/gpdtuzzyp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fktsv.cn/Article/details/ggnvnzjse.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.vehdjk.com/Article/details/gigqldciy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.tarul.cn/Article/details/gwalusmqd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.yfazqb.com/Article/details/gkgynlsuv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.bbcook.cn/Article/details/goweypfge.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.vehdjk.com/Article/details/glthnurzi.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.bbcook.cn/Article/details/glvgmcfao.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.epnwcf.com/Article/details/gbgjlqwon.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gtanyfbmn.sHtML

F. 文件与目录
来源：http://m.share.vehdjk.com/Article/details/gxffzlajy.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gdhlaortw.sHtML

[F01] 读取整个文件
来源：http://mobile.epnwcf.com/Article/details/gyavalqgl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.sjlbkw.cn/Article/details/ghzsuwpgm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gkfshadqj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.yfazqb.com/Article/details/gmeuzlylz.sHtML


<!-- 参考信息 -->