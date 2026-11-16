代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ssz.sufxvd.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pds.epnwcf.com

TS:   arr[0]; arr.at(-1);
来源：http://dxv.ivvv.top

Java: list.get(0); list.set(0, 9);
来源：http://zyv.snrcjt.cn

Go:   arr[0]; arr[0] = 9
来源：http://rck.jinqigfzy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cgj.haohaochexian.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jbh.pengpengdd.cyou

[D06] 数组长度
来源：http://rrl.yuxming.cn

Py:   len(arr)
来源：http://jdm.fehbvm.com

PHP:  count($arr);
来源：http://xhk.wangshuangyany.cn

JS:   arr.length
来源：http://pzt.sufxvd.cn

TS:   arr.length
来源：http://ybt.ivvv.top

Java: list.size();
来源：http://zev.sjlbkw.cn

Go:   len(arr)
来源：http://tll.nanxuanxn.top

Ruby: arr.length; arr.size
来源：http://ejm.wangshuangyany.cn

C#:   list.Count;
来源：http://ccw.fzhhl.top

[D07] 切片 / 取子数组
来源：http://gls.bjfxy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mne.hammf.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wkg.kuanghao11.cn

JS:   arr.slice(1, 4);
来源：http://npg.cheryme.top

TS:   arr.slice(1, 4);
来源：http://mpn.hammf.cn

Java: list.subList(1, 4);
来源：http://vnd.xingfuxueyuan.xyz

Go:   arr[1:4]
来源：http://wgy.mhx1999.top

Ruby: arr[1, 3]
来源：http://ckq.xuanzx.com

C#:   list.GetRange(1, 3);
来源：http://lex.gzhubu.top

[D08] 合并两个数组
来源：http://jwq.sysykeji.top

Py:   a + b;  a.extend(b)
来源：http://mjg.zhijiandao.cn

PHP:  array_merge($a, $b);
来源：http://rls.zhiwuduotai.top

JS:   [...a, ...b];  a.concat(b);
来源：http://jmj.cdnleiting.top

TS:   [...a, ...b];
来源：http://faa.yfazqb.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qdv.yangfankeji.com

Go:   append(a, b...)
来源：http://xbm.shzxlz.cn

Ruby: a + b;  a.concat(b)
来源：http://guu.mhx1999.top

C#:   a.Concat(b).ToList()
来源：http://cbk.zdbjq.cn

[D09] 排序（升序）
来源：http://efo.hongshengwenyu.top

Py:   sorted(arr);  arr.sort()
来源：http://ioe.xingfuxueyuan.xyz

PHP:  sort($arr);
来源：http://vqn.shangyingyoupin.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hgv.jqgufenzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://gpv.ydjk.org.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://kwh.uphjek.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cqn.gaohongyu789.top

Ruby: arr.sort
来源：http://icx.jqgfzy.top

C#:   list.Sort();
来源：http://tgo.sxryk.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ywf.c1oappe.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dsi.jianghu66.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pfv.sjlbkw.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ihz.smart0.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://whe.sufxvd.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ejk.jinqigfzy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://itj.chenjidiqi.icu

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nbn.316326.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dos.wangdashe.top

[D11] 反转数组
来源：http://bfi.sweek.top

Py:   arr[::-1];  arr.reverse()
来源：http://fht.nanxinkj.top

PHP:  array_reverse($arr);
来源：http://vog.haohaochexian.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mjb.shanyushiyangkeji.top

TS:   [...arr].reverse();
来源：http://aab.yueranfly.top

Java: Collections.reverse(list);
来源：http://kzw.andypj.xyz

Go:   slices.Reverse(arr)
来源：http://gvw.sufxvd.cn

Ruby: arr.reverse
来源：http://fef.ppjwa.cn

C#:   list.Reverse();
来源：http://wis.yangfankeji.com

[D12] 查找元素下标
来源：http://hrx.cucudq.cn

Py:   arr.index(x);  x in arr
来源：http://xay.ivvv.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nes.fehbvm.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pjf.0kj1m.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tep.svipenyu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://eoi.ydzc1.top

Go:   slices.Index(arr, x)
来源：http://nmf.shangyingyoupin.top

Ruby: arr.index(x)
来源：http://qlg.uphjek.com

C#:   list.IndexOf(x);
来源：http://ddj.jianghu66.top

[D13] 过滤（保留满足条件的）
来源：http://jet.snrcjt.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vwe.hongshengwenyu.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qts.yfazqb.com

JS:   arr.filter(x => x > 3)
来源：http://nwi.quarkkingdee.top

TS:   arr.filter(x => x > 3)
来源：http://zmv.aizwys.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dcb.wangdashe.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yol.shuidangran.top

Ruby: arr.select { |x| x > 3 }
来源：http://sqx.jinqigufen.top

C#:   list.Where(x => x > 3).ToList()
来源：http://cuj.0kj1m.cn

[D14] 映射转换（每个元素变形）
来源：http://vkr.xuanzx.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xux.andypj.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jnn.9152youxi.cn

JS:   arr.map(x => x * 2)
来源：http://scd.sjlbkw.cn

TS:   arr.map(x => x * 2)
来源：http://srz.cucudq.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vez.fehbvm.com

Go:   // 手写循环
来源：http://gls.aizwys.cn

Ruby: arr.map { |x| x * 2 }
来源：http://mui.pycfn.com

C#:   list.Select(x => x * 2).ToList()
来源：http://nqv.yj20258888.top

[D15] 去重
来源：http://xsn.pycfn.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yvm.ivvv.top

PHP:  array_unique($arr);
来源：http://nvk.0kj1m.cn

JS:   [...new Set(arr)]
来源：http://yri.ehwqpu.com

TS:   [...new Set(arr)]
来源：http://ejy.xuetiantiany.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pmy.hammf.cn

Go:   // 用 map[T]struct{} 手写
来源：http://qpc.tian-w.cn

Ruby: arr.uniq
来源：http://ouz.fktsv.cn

C#:   list.Distinct().ToList()
来源：http://xxw.yangfankeji.com

[D16] 求和与平均值
来源：http://cgk.yuxming.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://aww.ydjk.org.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://uhc.zdqjudy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wdi.epnwcf.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kal.chenjidiqi.icu

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bux.yuxming.cn

Go:   // 手写循环累加
来源：http://wqw.aizwys.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zua.shangyingyoupin.top

C#:   list.Sum();  list.Average()
来源：http://hwk.dashuyun.cn

[D17] 最大值与最小值
来源：http://slt.shanyushiyangkeji.top

Py:   max(arr);  min(arr)
来源：http://zki.hfpthk.cn

PHP:  max($arr);  min($arr);
来源：http://unc.fzhhl.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sjf.birdmap.top

TS:   Math.max(...arr);
来源：http://avu.shanyushiyangtech.top

Java: Collections.max(list);  Collections.min(list);
来源：http://axr.zhaomingkeji.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zoh.hywenlv.cn

Ruby: arr.max;  arr.min
来源：http://dpd.yj20258888.top

C#:   list.Max();  list.Min()
来源：http://cqj.yj20258.top

[D18] 扁平化嵌套数组
来源：http://ryi.redwolf501.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hgt.dashuyun.cn

PHP:  array_merge(...$nested);
来源：http://wyi.zhoulong.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vdq.aizwys.cn

TS:   nested.flat();
来源：http://wdx.zdbjq.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mpy.hesvh.cn

Go:   // 手写双层循环
来源：http://pcy.hcnkem.com

Ruby: nested.flatten
来源：http://kns.dashuyun.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ssr.shanyushiyangkeji.top

[D19] 按字段分组
来源：http://fvu.yonumen.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dih.xuetiantiany.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://upn.cdnleiting.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vwz.sjlbkw.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://otc.chenlongwang.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wdl.cqqwz.cn

Go:   // 手写 map[string][]T
来源：http://pbg.ehwqpu.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://quw.sjlbkw.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yhq.pycfn.com

[D20] 统计每个元素出现次数
来源：http://rkv.fehbvm.com

Py:   Counter(arr)
来源：http://zyh.quarkkingdee.top

PHP:  array_count_values($arr);
来源：http://hlw.sxryk.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rpk.tarul.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://srx.zhongyouzk.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tqc.mhx1999.top

Go:   // 手写 map[T]int
来源：http://con.chenjidiqi.icu

Ruby: arr.tally
来源：http://wgd.hongshengwenyu.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fns.jinghuilouyu.cn

[D21] 判断是否包含某元素
来源：http://ach.zhaomingkeji.xyz

Py:   x in arr
来源：http://qvr.snrcjt.cn

PHP:  in_array($x, $arr, true);
来源：http://exo.cashguo.top

JS:   arr.includes(x)
来源：http://tcv.yangfankeji.com

TS:   arr.includes(x)
来源：http://gqu.zdbjq.cn

Java: list.contains(x)
来源：http://hvb.hammf.cn

Go:   slices.Contains(arr, x)
来源：http://ofd.cheryme.top

Ruby: arr.include?(x)
来源：http://grt.zhiwuduotai.top

C#:   list.Contains(x)
来源：http://nze.zhaomingkeji.xyz

[D22] 复制数组（避免共享引用）
来源：http://ski.316326.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yrv.xylfe.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zqw.iojbl.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://eio.ydzc1.top

TS:   [...arr];
来源：http://tqg.hnqzz.top

Java: new ArrayList<>(list);
来源：http://pvv.shuidangran.top

Go:   copied := append([]int(nil), arr...)
来源：http://ppa.tarul.cn

Ruby: arr.dup;  arr.clone
来源：http://bfa.vqdsnc.cn

C#:   new List<int>(list);
来源：http://lat.wangdashe.top

[D23] reduce 累积计算
来源：http://gav.shanyushiyangtech.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jhj.nwbrower.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hwy.jiagoushi.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://smc.jinyuanbaomall.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pjd.jlsjyb.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://upk.vqdsnc.cn

Go:   // 手写循环
来源：http://zzu.tarul.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ngm.hysaishi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jae.zdqjudy.top

[D24] 字典 / Map 基本操作
来源：http://daz.nanxinkj.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://auj.xziqi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lqc.gotoacloud.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wwi.kuanghao11.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cpu.yueranfly.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zay.bbcook.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zrc.chenlongwang.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://yrr.meibo888.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://var.fengsongda.top

[D25] Set 集合去重与交并差
来源：http://pkm.316326.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mnz.svipenyu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sxr.zhoulong.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://drm.zdqjudy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://aod.c1oappe.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tvz.dashuyun.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fgn.shanyushiyangtech.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vvl.haohaochexian.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://oko.fehbvm.com

[D26] 数组转字符串
来源：http://jrz.redwolf501.top

Py:   ", ".join(map(str, arr))
来源：http://yhp.pengpengdd.cyou

PHP:  implode(", ", $arr);
来源：http://yth.nanxinkj.top

JS:   arr.join(", ")
来源：http://kmi.c1oappe.top

TS:   arr.join(", ")
来源：http://yie.havefunace.top

Java: String.join(", ", list)
来源：http://ysh.mhx1999.top

Go:   strings.Join(strs, ", ")
来源：http://msm.fktsv.cn

Ruby: arr.join(", ")
来源：http://sam.hesvh.cn

C#:   string.Join(", ", list)
来源：http://khe.pycfn.com

================================================================================
来源：http://kfa.hammf.cn

E. 字符串处理
来源：http://omw.fanxiaobao.xyz

================================================================================
来源：http://fyq.tianlin.xyz

[E01] 拼接字符串
来源：http://cqc.shangyingyoupin.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bxz.hammf.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hut.cheryme.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qaj.sxryk.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dlo.gaohongyu789.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lda.iojbl.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mcv.shanyushiyangkeji.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ync.fanxiaobao.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://frv.smart0.xyz

[E02] 重复字符串
来源：http://arm.ybcxt.top

Py:   "ab" * 3
来源：http://hzy.redwolf501.top

PHP:  str_repeat("ab", 3);
来源：http://adx.jinqigfzy.top

JS:   "ab".repeat(3)
来源：http://opd.cqqwz.cn

TS:   "ab".repeat(3)
来源：http://opj.xuetiantiany.cn

Java: "ab".repeat(3)
来源：http://cks.chenjidiqi.icu

Go:   strings.Repeat("ab", 3)
来源：http://wfb.316326.xyz

Ruby: "ab" * 3
来源：http://aiq.gogol.net.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hga.bbcook.cn

[E03] 截取子串
来源：http://jcl.xinyue.icu

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qli.daxiang520.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vxb.xylfe.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sqy.cashguo.top

TS:   s.slice(1, 4)
来源：http://som.yuanzhike.top

Java: s.substring(1, 4)
来源：http://xjk.chenjidiqi.icu

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gos.tian-w.cn

Ruby: s[1, 3];  s[1..3]
来源：http://fqq.daria6918.cn

C#:   s.Substring(1, 3)
来源：http://lsk.jinghuilouyu.cn

[E04] 查找子串位置
来源：http://ivy.cashguo.top

Py:   s.find("x");  s.index("x")
来源：http://wom.aizwys.cn

PHP:  strpos($s, "x");
来源：http://zmh.ivvv.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qjd.aibaodan.cn

TS:   s.indexOf("x")
来源：http://fus.hesvh.cn

Java: s.indexOf("x")
来源：http://bfo.gogol.net.cn

Go:   strings.Index(s, "x")
来源：http://zge.mhx1999.top

Ruby: s.index("x")
来源：http://pdz.yuxming.cn

C#:   s.IndexOf("x")
来源：http://fqr.fehbvm.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://mxx.andypj.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jdh.hnqzz.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lei.aibaodan.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xtt.zhongyouzk.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://liu.fzhhl.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yyv.hysaishi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://aps.pengpengdd.cyou

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pkb.sxryk.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cly.tanke756.top

[E06] 替换子串
来源：http://rtl.xylfe.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lri.haohaochexian.top

PHP:  str_replace("a", "b", $s);
来源：http://tmx.aizwys.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dgr.jinqigufen.top

TS:   s.replaceAll("a", "b")
来源：http://cat.hcnkem.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cxu.jinyuanbaomall.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vlg.zycfv.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nto.ydzc1.top

C#:   s.Replace("a", "b")
来源：http://fxk.aibaodan.cn

[E07] 按分隔符拆分
来源：http://qlq.xziqi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qcy.shanyushiyangtech.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qlk.dianchejie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hln.dianchejie.cn

TS:   s.split(",")
来源：http://qzp.zhoulong.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://jym.xuanzx.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ond.c1oappe.top

Ruby: s.split(",");  s.split
来源：http://wpn.xuanzx.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://obn.wangshuangyany.cn

[E08] 数组按分隔符合并
来源：http://umj.yj20258888.top

Py:   ",".join(items)
来源：http://xdv.xylfe.cn

PHP:  implode(",", $items);
来源：http://lzc.hesvh.cn

JS:   items.join(",")
来源：http://btt.yfazqb.com

TS:   items.join(",")
来源：http://tqj.fzhhl.top

Java: String.join(",", items)
来源：http://jmg.cdnleiting.top

Go:   strings.Join(items, ",")
来源：http://led.daria6918.cn

Ruby: items.join(",")
来源：http://mtr.tarul.cn

C#:   string.Join(",", items)
来源：http://vkj.dashuyun.cn

[E09] 去除所有空白字符
来源：http://csg.ybcxt.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fix.fanxiaobao.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vdk.andypj.xyz

JS:   s.replace(/\s+/g, "")
来源：http://gog.havefunace.top

TS:   s.replace(/\s+/g, "")
来源：http://ibg.sxryk.cn

Java: s.replaceAll("\\s+", "")
来源：http://nng.mhx1999.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://rwc.nwbrower.top

Ruby: s.gsub(/\s+/, "")
来源：http://wic.hammf.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cfs.zhaomingkeji.xyz

[E10] 左侧补零 / 定长填充
来源：http://wnu.hesvh.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://suv.cashguo.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lvk.0kj1m.cn

JS:   "7".padStart(3, "0")
来源：http://hyj.zhiwuduotai.top

TS:   "7".padStart(3, "0")
来源：http://tbn.zycfv.cn

Java: String.format("%03d", 7)
来源：http://hqo.hongshengwenyu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://pzt.hammf.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sqj.andypj.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://drl.gotoacloud.top

[E11] 反转字符串
来源：http://rwd.fzhhl.top

Py:   s[::-1]
来源：http://ipa.kuanghao11.cn

PHP:  strrev($s);
来源：http://kkk.gogol.net.cn

JS:   [...s].reverse().join("")
来源：http://ppv.uphjek.com

TS:   [...s].reverse().join("")
来源：http://kns.snrcjt.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://nar.jyoumei.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://jvp.hesvh.cn

Ruby: s.reverse
来源：http://uzo.gogol.net.cn

C#:   new string(s.Reverse().ToArray())
来源：http://nee.yvedp.cn

[E12] 统计某字符出现次数
来源：http://qau.cdnleiting.top

Py:   s.count("a")
来源：http://iri.zhijiandao.cn


<!-- 参考信息 -->