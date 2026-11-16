代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://igd.jyoumei.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fzb.yongpay.top

TS:   arr[0]; arr.at(-1);
来源：http://nab.aizwys.cn

Java: list.get(0); list.set(0, 9);
来源：http://ulc.sufxvd.cn

Go:   arr[0]; arr[0] = 9
来源：http://sgc.ydjk.org.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cgo.daxiang520.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://imf.pengpengdd.cyou

[D06] 数组长度
来源：http://bkx.vqdsnc.cn

Py:   len(arr)
来源：http://kks.wangshuangyany.cn

PHP:  count($arr);
来源：http://emw.gotoacloud.top

JS:   arr.length
来源：http://jgc.cashguo.top

TS:   arr.length
来源：http://iym.zhongyouzk.top

Java: list.size();
来源：http://kni.gaohongyu789.top

Go:   len(arr)
来源：http://lzf.haohaochexian.top

Ruby: arr.length; arr.size
来源：http://zlz.jinqigufen.top

C#:   list.Count;
来源：http://ekw.tian-w.cn

[D07] 切片 / 取子数组
来源：http://scp.yfazqb.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zdq.hnxiangtu.top

PHP:  array_slice($arr, 1, 3);
来源：http://qfq.jiagoushi.top

JS:   arr.slice(1, 4);
来源：http://ipo.9152youxi.cn

TS:   arr.slice(1, 4);
来源：http://mrt.feifeiyinyue.top

Java: list.subList(1, 4);
来源：http://rvc.yuanzhike.top

Go:   arr[1:4]
来源：http://ccs.guowangkeji.top

Ruby: arr[1, 3]
来源：http://roe.wangdashe.top

C#:   list.GetRange(1, 3);
来源：http://enz.xuanzx.com

[D08] 合并两个数组
来源：http://lad.aizwys.cn

Py:   a + b;  a.extend(b)
来源：http://tct.wangshuangyany.cn

PHP:  array_merge($a, $b);
来源：http://vbu.jinqigfzy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://fmo.shangyingyoupin.top

TS:   [...a, ...b];
来源：http://fey.tanke756.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mkc.cheryme.top

Go:   append(a, b...)
来源：http://ool.jinqigufen.top

Ruby: a + b;  a.concat(b)
来源：http://nuk.andypj.xyz

C#:   a.Concat(b).ToList()
来源：http://nhn.52xcode.cn

[D09] 排序（升序）
来源：http://sma.ivvv.top

Py:   sorted(arr);  arr.sort()
来源：http://gou.havefunace.top

PHP:  sort($arr);
来源：http://tiz.fktsv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kwf.hesvh.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fek.aizwys.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://lgd.havefunace.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nqk.meibo888.top

Ruby: arr.sort
来源：http://bnf.zhixingplan.top

C#:   list.Sort();
来源：http://lqh.cucudq.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qag.yuxming.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zcz.chenzaomai.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://shm.aizwys.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lim.svipenyu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fbq.cqqwz.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zgc.fktsv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zgj.zdbjq.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://oil.xylfe.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mly.vehdjk.com

[D11] 反转数组
来源：http://gkx.zhiwuduotai.top

Py:   arr[::-1];  arr.reverse()
来源：http://kla.zdqjudy.top

PHP:  array_reverse($arr);
来源：http://aua.tarul.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zjd.jinyuanbaomall.cn

TS:   [...arr].reverse();
来源：http://yyw.yj202588.top

Java: Collections.reverse(list);
来源：http://fgn.pycfn.com

Go:   slices.Reverse(arr)
来源：http://fxm.zdqjudy.top

Ruby: arr.reverse
来源：http://swe.yj20258888.top

C#:   list.Reverse();
来源：http://vfy.fengsongda.top

[D12] 查找元素下标
来源：http://wjv.iojbl.cn

Py:   arr.index(x);  x in arr
来源：http://ysz.sxryk.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://otl.bbcook.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://aqg.vqdsnc.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://umk.fehbvm.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yjf.hnxiangtu.top

Go:   slices.Index(arr, x)
来源：http://lly.pengpengdd.cyou

Ruby: arr.index(x)
来源：http://oil.fanxiaobao.xyz

C#:   list.IndexOf(x);
来源：http://ret.hysaishi.cn

[D13] 过滤（保留满足条件的）
来源：http://dce.zhaomingkeji.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qzc.jqgfzy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vyu.redwolf501.top

JS:   arr.filter(x => x > 3)
来源：http://sae.birdmap.top

TS:   arr.filter(x => x > 3)
来源：http://nhj.yueranfly.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rdy.birdmap.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vwk.mhx1999.top

Ruby: arr.select { |x| x > 3 }
来源：http://jxm.0kj1m.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://evw.fanxiaobao.xyz

[D14] 映射转换（每个元素变形）
来源：http://hti.zhijiandao.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uqg.316326.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kel.fehbvm.com

JS:   arr.map(x => x * 2)
来源：http://kgf.ybcxt.top

TS:   arr.map(x => x * 2)
来源：http://bml.uphjek.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://iro.c1oappe.top

Go:   // 手写循环
来源：http://wry.hysaishi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vyy.ctjpmb.com

C#:   list.Select(x => x * 2).ToList()
来源：http://olg.iojbl.cn

[D15] 去重
来源：http://efk.sxryk.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sae.gaohongyu789.top

PHP:  array_unique($arr);
来源：http://zvn.meibo888.top

JS:   [...new Set(arr)]
来源：http://jrg.pycfn.com

TS:   [...new Set(arr)]
来源：http://oqm.yj20258888.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kfy.hywenlv.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ixm.316326.xyz

Ruby: arr.uniq
来源：http://hbc.zhijiandao.cn

C#:   list.Distinct().ToList()
来源：http://kcr.hnqzz.top

[D16] 求和与平均值
来源：http://hmy.nwbrower.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kfz.bbcook.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vnk.nanxinkj.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mfs.316326.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nzi.hnqzz.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lqo.ydjk.org.cn

Go:   // 手写循环累加
来源：http://vve.yfazqb.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kqw.chenjidiqi.icu

C#:   list.Sum();  list.Average()
来源：http://mdj.jyoumei.cn

[D17] 最大值与最小值
来源：http://xzy.hywenlv.cn

Py:   max(arr);  min(arr)
来源：http://zyg.shanyushiyangtech.top

PHP:  max($arr);  min($arr);
来源：http://wsr.daxiang520.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://eoq.shanyushiyangkeji.top

TS:   Math.max(...arr);
来源：http://jli.xuanzx.com

Java: Collections.max(list);  Collections.min(list);
来源：http://rui.pycfn.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ztx.smart0.xyz

Ruby: arr.max;  arr.min
来源：http://qgd.vqdsnc.cn

C#:   list.Max();  list.Min()
来源：http://mfy.xuanzx.com

[D18] 扁平化嵌套数组
来源：http://drv.andypj.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fpp.hcnkem.com

PHP:  array_merge(...$nested);
来源：http://pxr.jinyuanbaomall.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pxi.dianchejie.cn

TS:   nested.flat();
来源：http://qgi.chenzaomai.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://iew.jyoumei.cn

Go:   // 手写双层循环
来源：http://pab.0kj1m.cn

Ruby: nested.flatten
来源：http://kdu.aizwys.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://tvm.cqqwz.cn

[D19] 按字段分组
来源：http://dis.yfazqb.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://crc.tian-w.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://prn.shuidangran.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ggx.zhongyouzk.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://oke.yangfankeji.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rky.zhijiandao.cn

Go:   // 手写 map[string][]T
来源：http://ivi.fzhhl.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://pfo.hongshengwenyu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xgs.ctjpmb.com

[D20] 统计每个元素出现次数
来源：http://pwk.jinyuanbaomall.cn

Py:   Counter(arr)
来源：http://wjj.svipenyu.cn

PHP:  array_count_values($arr);
来源：http://zqd.aizwys.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yyf.jinghuilouyu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mpi.zdqjudy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ujj.ctjpmb.com

Go:   // 手写 map[T]int
来源：http://sag.fehbvm.com

Ruby: arr.tally
来源：http://zme.yanxiufei.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cfo.yuanzhike.top

[D21] 判断是否包含某元素
来源：http://dau.aibaodan.cn

Py:   x in arr
来源：http://omp.wangdashe.top

PHP:  in_array($x, $arr, true);
来源：http://mvh.andypj.xyz

JS:   arr.includes(x)
来源：http://zjk.zhaomingkeji.xyz

TS:   arr.includes(x)
来源：http://wld.wangshuangyany.cn

Java: list.contains(x)
来源：http://wbf.snrcjt.cn

Go:   slices.Contains(arr, x)
来源：http://dmt.jqgufenzy.top

Ruby: arr.include?(x)
来源：http://hih.xylfe.cn

C#:   list.Contains(x)
来源：http://qde.fanxiaobao.xyz

[D22] 复制数组（避免共享引用）
来源：http://zpv.iojbl.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yof.gzhubu.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jnp.birdmap.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rpt.316326.xyz

TS:   [...arr];
来源：http://qxc.yuxming.cn

Java: new ArrayList<>(list);
来源：http://mhl.sweek.top

Go:   copied := append([]int(nil), arr...)
来源：http://ivj.wangdashe.top

Ruby: arr.dup;  arr.clone
来源：http://ftz.sxryk.cn

C#:   new List<int>(list);
来源：http://zvy.redwolf501.top

[D23] reduce 累积计算
来源：http://ixy.xuanzx.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sfs.jlsjyb.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jdu.redwolf501.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wkd.uphjek.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zns.meibo888.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://mjl.xuanzx.com

Go:   // 手写循环
来源：http://dys.feifeiyinyue.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ptz.jiagoushi.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jjh.wangdashe.top

[D24] 字典 / Map 基本操作
来源：http://qhk.wangshuangyany.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nso.yongpay.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jue.hesvh.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tsg.zdqjudy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jps.mhx1999.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lqa.jqgufenzy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cum.jlsjyb.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zsg.meibo888.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ooj.cheryme.top

[D25] Set 集合去重与交并差
来源：http://jiz.sxryk.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pkn.hysaishi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mos.tanke756.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://leh.dianchejie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://guv.wangshuangyany.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kro.c1oappe.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://exw.jqgfzy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://euc.svipenyu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tqj.316326.xyz

[D26] 数组转字符串
来源：http://lgu.svipenyu.cn

Py:   ", ".join(map(str, arr))
来源：http://yva.jinghuilouyu.cn

PHP:  implode(", ", $arr);
来源：http://ktq.gogol.net.cn

JS:   arr.join(", ")
来源：http://qwq.zhaomingkeji.xyz

TS:   arr.join(", ")
来源：http://mhc.yvedp.cn

Java: String.join(", ", list)
来源：http://ktc.fktsv.cn

Go:   strings.Join(strs, ", ")
来源：http://kps.hysaishi.cn

Ruby: arr.join(", ")
来源：http://grn.zhixingplan.top

C#:   string.Join(", ", list)
来源：http://bif.fengsongda.top

================================================================================
来源：http://yze.aibaodan.cn

E. 字符串处理
来源：http://miy.shanyushiyangtech.top

================================================================================
来源：http://guw.shzxlz.cn

[E01] 拼接字符串
来源：http://dpr.yuanzhike.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nsj.xuanzx.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fgc.zhongyouzk.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rnq.pengpengdd.cyou

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tmi.shanyushiyangkeji.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://omj.gogol.net.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://khk.yfazqb.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qpb.sjlbkw.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ytc.mhx1999.top

[E02] 重复字符串
来源：http://xse.jqgfzy.top

Py:   "ab" * 3
来源：http://erz.ywan-chungtsiang.top

PHP:  str_repeat("ab", 3);
来源：http://fwh.shanyushiyangkeji.top

JS:   "ab".repeat(3)
来源：http://gcw.aibaodan.cn

TS:   "ab".repeat(3)
来源：http://zgz.jinyuanbaomall.cn

Java: "ab".repeat(3)
来源：http://bdu.yvedp.cn

Go:   strings.Repeat("ab", 3)
来源：http://nhu.shangyingyoupin.top

Ruby: "ab" * 3
来源：http://gtg.ybcxt.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vfq.tian-w.cn

[E03] 截取子串
来源：http://fpw.shangyingyoupin.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mrp.zhengqikj.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rhs.fehbvm.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://irk.sweek.top

TS:   s.slice(1, 4)
来源：http://cew.zhongyouzk.top

Java: s.substring(1, 4)
来源：http://zdw.bjfxy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lyn.yangfankeji.com

Ruby: s[1, 3];  s[1..3]
来源：http://hbk.yj20258888.top

C#:   s.Substring(1, 3)
来源：http://xwo.ybcxt.top

[E04] 查找子串位置
来源：http://oud.guannengcc.top

Py:   s.find("x");  s.index("x")
来源：http://eow.kuanghao11.cn

PHP:  strpos($s, "x");
来源：http://keh.fanxiaobao.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://khc.hongshengwenyu.top

TS:   s.indexOf("x")
来源：http://nyp.zhengqikj.top

Java: s.indexOf("x")
来源：http://ufs.sweek.top

Go:   strings.Index(s, "x")
来源：http://dpm.guowangkeji.top

Ruby: s.index("x")
来源：http://umx.xziqi.cn

C#:   s.IndexOf("x")
来源：http://zgp.yvedp.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://cve.gaohongyu789.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://aoo.sweek.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pmq.cucudq.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cim.guannengcc.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ccr.yfazqb.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://aza.gogol.net.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://chh.bbcook.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bum.shanyushiyangkeji.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wqu.ctjpmb.com

[E06] 替换子串
来源：http://wzj.feifeiyinyue.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cac.cheryme.top

PHP:  str_replace("a", "b", $s);
来源：http://psd.ybcxt.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://epn.daria6918.cn

TS:   s.replaceAll("a", "b")
来源：http://box.zdbjq.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dzp.9152youxi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lxm.ydjk.org.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pqg.jinqigfzy.top

C#:   s.Replace("a", "b")
来源：http://uef.ydjk.org.cn

[E07] 按分隔符拆分
来源：http://rkq.c1oappe.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jpk.jlsjyb.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fre.guannengcc.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ekm.yuanzhike.top

TS:   s.split(",")
来源：http://qgi.wangdashe.top

Java: s.split(",");  s.split("\\s+")
来源：http://kpa.zhiwuduotai.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uvi.shzxlz.cn

Ruby: s.split(",");  s.split
来源：http://yzw.tanke756.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kdl.hnxiangtu.top

[E08] 数组按分隔符合并
来源：http://nux.sxryk.cn

Py:   ",".join(items)
来源：http://mar.jinqigufen.top

PHP:  implode(",", $items);
来源：http://bjs.guannengcc.top

JS:   items.join(",")
来源：http://opu.pengpengdd.cyou

TS:   items.join(",")
来源：http://gts.sufxvd.cn

Java: String.join(",", items)
来源：http://uip.hongshengwenyu.top

Go:   strings.Join(items, ",")
来源：http://hze.wangshuangyany.cn

Ruby: items.join(",")
来源：http://gsg.ehwqpu.com

C#:   string.Join(",", items)
来源：http://nvw.52xcode.cn

[E09] 去除所有空白字符
来源：http://rzp.hywenlv.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://arc.dashuyun.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ndf.guowangkeji.top

JS:   s.replace(/\s+/g, "")
来源：http://bwq.yonumen.top

TS:   s.replace(/\s+/g, "")
来源：http://ich.meibo888.top

Java: s.replaceAll("\\s+", "")
来源：http://hdc.tianlin.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://whw.shzxlz.cn

Ruby: s.gsub(/\s+/, "")
来源：http://glt.birdmap.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xud.hfpthk.cn

[E10] 左侧补零 / 定长填充
来源：http://pfe.xuetiantiany.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ogf.sysykeji.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://var.9152youxi.cn

JS:   "7".padStart(3, "0")
来源：http://dcu.aizwys.cn

TS:   "7".padStart(3, "0")
来源：http://ygu.shanyushiyangtech.top

Java: String.format("%03d", 7)
来源：http://evb.xziqi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://gjz.yj20258.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wts.jianghu66.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cyl.jiagoushi.top

[E11] 反转字符串
来源：http://dat.zdqjudy.top

Py:   s[::-1]
来源：http://yfx.sufxvd.cn

PHP:  strrev($s);
来源：http://zec.cucudq.cn

JS:   [...s].reverse().join("")
来源：http://smt.guowangkeji.top

TS:   [...s].reverse().join("")
来源：http://piv.wangdashe.top

Java: new StringBuilder(s).reverse().toString()
来源：http://miz.dashuyun.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hgj.yj202588.top

Ruby: s.reverse
来源：http://ojj.hnxiangtu.top

C#:   new string(s.Reverse().ToArray())
来源：http://qmu.jiagoushi.top

[E12] 统计某字符出现次数
来源：http://mcs.yangfankeji.com

Py:   s.count("a")
来源：http://lgd.ctjpmb.com


<!-- 参考信息 -->