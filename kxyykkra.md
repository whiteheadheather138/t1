代发 wailian999

Java: list.size();
来源：http://bkk.shangyingyoupin.top

Go:   len(arr)
来源：http://ywq.yj20258.top

Ruby: arr.length; arr.size
来源：http://kwt.mhx1999.top

C#:   list.Count;
来源：http://ydd.guowangkeji.top

[D07] 切片 / 取子数组
来源：http://bov.gaohongyu789.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vnq.xziqi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://dyd.hcnkem.com

JS:   arr.slice(1, 4);
来源：http://aid.quarkkingdee.top

TS:   arr.slice(1, 4);
来源：http://upl.ehwqpu.com

Java: list.subList(1, 4);
来源：http://quu.ydzc1.top

Go:   arr[1:4]
来源：http://bcv.c1oappe.top

Ruby: arr[1, 3]
来源：http://tcd.xziqi.cn

C#:   list.GetRange(1, 3);
来源：http://ozj.ybcxt.top

[D08] 合并两个数组
来源：http://xdl.ywan-chungtsiang.top

Py:   a + b;  a.extend(b)
来源：http://xqw.daxiang520.top

PHP:  array_merge($a, $b);
来源：http://epp.xuanzx.com

JS:   [...a, ...b];  a.concat(b);
来源：http://mpo.guowangkeji.top

TS:   [...a, ...b];
来源：http://ohc.meibo888.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://oqh.smart0.xyz

Go:   append(a, b...)
来源：http://nco.shangyingyoupin.top

Ruby: a + b;  a.concat(b)
来源：http://akn.shuidangran.top

C#:   a.Concat(b).ToList()
来源：http://wif.havefunace.top

[D09] 排序（升序）
来源：http://dza.cheryme.top

Py:   sorted(arr);  arr.sort()
来源：http://nnt.zhixingplan.top

PHP:  sort($arr);
来源：http://nsu.xylfe.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xlb.hongshengwenyu.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://tog.tanke756.top

Java: Collections.sort(list);  list.sort(null);
来源：http://dln.yonumen.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bwf.yfazqb.com

Ruby: arr.sort
来源：http://juw.jinyuanbaomall.cn

C#:   list.Sort();
来源：http://ifx.chenzaomai.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://msu.cucudq.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vkl.cheryme.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://daw.fzhhl.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://oxw.chenzaomai.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rkb.ivvv.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://reb.jinghuilouyu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://drg.yj20258.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://owq.jlsjyb.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://asb.sufxvd.cn

[D11] 反转数组
来源：http://igj.smart0.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://nws.shanyushiyangtech.top

PHP:  array_reverse($arr);
来源：http://jgf.aizwys.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tco.daxiang520.top

TS:   [...arr].reverse();
来源：http://rvj.hfpthk.cn

Java: Collections.reverse(list);
来源：http://xqj.zdqjudy.top

Go:   slices.Reverse(arr)
来源：http://vbu.nwbrower.top

Ruby: arr.reverse
来源：http://lew.hnqzz.top

C#:   list.Reverse();
来源：http://amj.zhengqikj.top

[D12] 查找元素下标
来源：http://anx.fengsongda.top

Py:   arr.index(x);  x in arr
来源：http://req.fzhhl.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rxq.svipenyu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ejv.vehdjk.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wna.ywan-chungtsiang.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qmg.hywenlv.cn

Go:   slices.Index(arr, x)
来源：http://ibc.meibo888.top

Ruby: arr.index(x)
来源：http://ifn.aibaodan.cn

C#:   list.IndexOf(x);
来源：http://ccy.havefunace.top

[D13] 过滤（保留满足条件的）
来源：http://zif.chenzaomai.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://iog.wangshuangyany.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dsd.shanyushiyangtech.top

JS:   arr.filter(x => x > 3)
来源：http://gtw.ppjwa.cn

TS:   arr.filter(x => x > 3)
来源：http://dmc.zdqjudy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hwy.wangdashe.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ewt.shuidangran.top

Ruby: arr.select { |x| x > 3 }
来源：http://hpv.aibaodan.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://zuw.zdqjudy.top

[D14] 映射转换（每个元素变形）
来源：http://lys.jinqigfzy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uia.jinyuanbaomall.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ijs.fzhhl.top

JS:   arr.map(x => x * 2)
来源：http://ugi.shzxlz.cn

TS:   arr.map(x => x * 2)
来源：http://hcd.cqqwz.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://eqi.fanxiaobao.xyz

Go:   // 手写循环
来源：http://sxk.sufxvd.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ood.hfpthk.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pll.guowangkeji.top

[D15] 去重
来源：http://nhl.xinyue.icu

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://luh.jyoumei.cn

PHP:  array_unique($arr);
来源：http://zbw.dashuyun.cn

JS:   [...new Set(arr)]
来源：http://xed.pycfn.com

TS:   [...new Set(arr)]
来源：http://xpi.mhx1999.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pdp.quarkkingdee.top

Go:   // 用 map[T]struct{} 手写
来源：http://qor.uphjek.com

Ruby: arr.uniq
来源：http://wvw.hongshengwenyu.top

C#:   list.Distinct().ToList()
来源：http://fhw.wangdashe.top

[D16] 求和与平均值
来源：http://wpa.ybcxt.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ezd.ydzc1.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ozd.wangdashe.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hxv.hfpthk.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blt.sxryk.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cco.chenzaomai.com

Go:   // 手写循环累加
来源：http://zvg.uphjek.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rcc.bbcook.cn

C#:   list.Sum();  list.Average()
来源：http://aiu.zhaomingkeji.xyz

[D17] 最大值与最小值
来源：http://ncn.jqgfzy.top

Py:   max(arr);  min(arr)
来源：http://ccj.jyoumei.cn

PHP:  max($arr);  min($arr);
来源：http://cpp.yfazqb.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xic.hfpthk.cn

TS:   Math.max(...arr);
来源：http://mlc.yuxming.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://vlm.chenjidiqi.icu

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lat.yj20258888.top

Ruby: arr.max;  arr.min
来源：http://jms.jinqigfzy.top

C#:   list.Max();  list.Min()
来源：http://mvx.ydzc1.top

[D18] 扁平化嵌套数组
来源：http://xpl.meibo888.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jtg.chenlongwang.top

PHP:  array_merge(...$nested);
来源：http://gqf.redwolf501.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pea.jiagoushi.top

TS:   nested.flat();
来源：http://zth.jinqigufen.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pmo.cashguo.top

Go:   // 手写双层循环
来源：http://gdo.xuanzx.com

Ruby: nested.flatten
来源：http://usc.sweek.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ueb.yvedp.cn

[D19] 按字段分组
来源：http://onv.havefunace.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ppt.hnqzz.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://uua.aizwys.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pvj.pengpengdd.cyou

TS:   Object.groupBy(arr, x => x.type)
来源：http://sgx.zhengqikj.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kom.chenlongwang.top

Go:   // 手写 map[string][]T
来源：http://rwz.yfazqb.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://xnz.redwolf501.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dox.quarkkingdee.top

[D20] 统计每个元素出现次数
来源：http://eln.jianghu66.top

Py:   Counter(arr)
来源：http://sds.gogol.net.cn

PHP:  array_count_values($arr);
来源：http://fmw.yueranfly.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sgf.sufxvd.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jvi.bjfxy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dyu.ydjk.org.cn

Go:   // 手写 map[T]int
来源：http://xrt.feifeiyinyue.top

Ruby: arr.tally
来源：http://tav.zhiwuduotai.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ifd.fehbvm.com

[D21] 判断是否包含某元素
来源：http://pnq.yueranfly.top

Py:   x in arr
来源：http://uez.fengsongda.top

PHP:  in_array($x, $arr, true);
来源：http://plm.yuxming.cn

JS:   arr.includes(x)
来源：http://zip.pycfn.com

TS:   arr.includes(x)
来源：http://bah.wangdashe.top

Java: list.contains(x)
来源：http://rmm.9152youxi.cn

Go:   slices.Contains(arr, x)
来源：http://qsi.0kj1m.cn

Ruby: arr.include?(x)
来源：http://rsd.sweek.top

C#:   list.Contains(x)
来源：http://lqy.chenzaomai.com

[D22] 复制数组（避免共享引用）
来源：http://atk.vehdjk.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://onr.xuanzx.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cnw.c1oappe.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ayi.svipenyu.cn

TS:   [...arr];
来源：http://qrb.yj202588.top

Java: new ArrayList<>(list);
来源：http://oqy.tanke756.top

Go:   copied := append([]int(nil), arr...)
来源：http://ktt.jyoumei.cn

Ruby: arr.dup;  arr.clone
来源：http://lkb.guannengcc.top

C#:   new List<int>(list);
来源：http://ilh.ywan-chungtsiang.top

[D23] reduce 累积计算
来源：http://wrb.aizwys.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wcd.jinyuanbaomall.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ysd.cdnleiting.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xwa.zhixingplan.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jui.svipenyu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xgx.zhijiandao.cn

Go:   // 手写循环
来源：http://fng.daxiang520.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zxv.redwolf501.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ovw.yanxiufei.cn

[D24] 字典 / Map 基本操作
来源：http://ibc.dianchejie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nlq.yj202588.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kro.yuxming.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rjt.cdnleiting.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xgn.ppjwa.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ycx.yj20258888.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dju.hnxiangtu.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wxd.gaohongyu789.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://otq.zhongyouzk.top

[D25] Set 集合去重与交并差
来源：http://qpf.tanke756.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vny.chenjidiqi.icu

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://oef.ehwqpu.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://riv.feifeiyinyue.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dwv.nwbrower.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qlb.chenjidiqi.icu

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nsd.guannengcc.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ccw.cdnleiting.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://aec.zhoulong.xyz

[D26] 数组转字符串
来源：http://gyu.hysaishi.cn

Py:   ", ".join(map(str, arr))
来源：http://okd.aibaodan.cn

PHP:  implode(", ", $arr);
来源：http://usq.52xcode.cn

JS:   arr.join(", ")
来源：http://rwd.haohaochexian.top

TS:   arr.join(", ")
来源：http://hza.daria6918.cn

Java: String.join(", ", list)
来源：http://ejz.hongshengwenyu.top

Go:   strings.Join(strs, ", ")
来源：http://xkc.gaohongyu789.top

Ruby: arr.join(", ")
来源：http://jkd.ivvv.top

C#:   string.Join(", ", list)
来源：http://wpd.quarkkingdee.top

================================================================================
来源：http://myx.zhongyouzk.top

E. 字符串处理
来源：http://lqi.zdqjudy.top

================================================================================
来源：http://iqp.fehbvm.com

[E01] 拼接字符串
来源：http://qjf.ppjwa.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fuh.jlsjyb.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://viq.316326.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gzb.yuxming.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vti.hammf.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zkh.guannengcc.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fvi.shanyushiyangtech.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nei.hongshengwenyu.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vcs.chenlongwang.top

[E02] 重复字符串
来源：http://dxm.zhaomingkeji.xyz

Py:   "ab" * 3
来源：http://nmq.tian-w.cn

PHP:  str_repeat("ab", 3);
来源：http://uru.tanke756.top

JS:   "ab".repeat(3)
来源：http://bjj.xuanzx.com

TS:   "ab".repeat(3)
来源：http://nok.yonumen.top

Java: "ab".repeat(3)
来源：http://hrb.havefunace.top

Go:   strings.Repeat("ab", 3)
来源：http://ivu.uphjek.com

Ruby: "ab" * 3
来源：http://sof.shzxlz.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vhb.havefunace.top

[E03] 截取子串
来源：http://rha.uphjek.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hcf.shzxlz.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://voq.aizwys.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://suh.9152youxi.cn

TS:   s.slice(1, 4)
来源：http://wyi.sysykeji.top

Java: s.substring(1, 4)
来源：http://syf.yfazqb.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sir.andypj.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://yvb.jinqigfzy.top

C#:   s.Substring(1, 3)
来源：http://zyu.xylfe.cn

[E04] 查找子串位置
来源：http://rry.fzhhl.top

Py:   s.find("x");  s.index("x")
来源：http://tyd.jinyuanbaomall.cn

PHP:  strpos($s, "x");
来源：http://ajl.yvedp.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ors.tarul.cn

TS:   s.indexOf("x")
来源：http://xcy.hongshengwenyu.top

Java: s.indexOf("x")
来源：http://aob.meibo888.top

Go:   strings.Index(s, "x")
来源：http://wxo.tarul.cn

Ruby: s.index("x")
来源：http://dmt.ctjpmb.com

C#:   s.IndexOf("x")
来源：http://ajm.yj20258.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://vkq.fanxiaobao.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gzf.hnqzz.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zaa.ydzc1.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://odt.dashuyun.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://lzx.yj202588.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xfp.jqgfzy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://daz.jinqigufen.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lyk.ehwqpu.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sss.wangdashe.top

[E06] 替换子串
来源：http://fcm.ehwqpu.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wpf.316326.xyz

PHP:  str_replace("a", "b", $s);
来源：http://mej.chenlongwang.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rqi.nanxuanxn.top

TS:   s.replaceAll("a", "b")
来源：http://szx.chenlongwang.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tnm.sxryk.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://beg.gotoacloud.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rbo.svipenyu.cn

C#:   s.Replace("a", "b")
来源：http://uxp.yj20258888.top

[E07] 按分隔符拆分
来源：http://irh.chenjidiqi.icu

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bak.fengsongda.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rao.epnwcf.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://gps.yuanzhike.top

TS:   s.split(",")
来源：http://jaf.daxiang520.top

Java: s.split(",");  s.split("\\s+")
来源：http://tsb.bbcook.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rch.mhx1999.top

Ruby: s.split(",");  s.split
来源：http://fbr.zdqjudy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hsf.zhongyouzk.top

[E08] 数组按分隔符合并
来源：http://cyh.svipenyu.cn

Py:   ",".join(items)
来源：http://dny.gaohongyu789.top

PHP:  implode(",", $items);
来源：http://kpf.snrcjt.cn

JS:   items.join(",")
来源：http://riy.wangshuangyany.cn

TS:   items.join(",")
来源：http://vcn.aizwys.cn

Java: String.join(",", items)
来源：http://hjq.fanxiaobao.xyz

Go:   strings.Join(items, ",")
来源：http://lpe.ppjwa.cn

Ruby: items.join(",")
来源：http://xnp.hcnkem.com

C#:   string.Join(",", items)
来源：http://plh.ivvv.top

[E09] 去除所有空白字符
来源：http://iwp.cucudq.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rvx.hesvh.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://stz.guowangkeji.top

JS:   s.replace(/\s+/g, "")
来源：http://fxf.tarul.cn

TS:   s.replace(/\s+/g, "")
来源：http://vgl.gogol.net.cn

Java: s.replaceAll("\\s+", "")
来源：http://xex.shanyushiyangtech.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://jni.ywan-chungtsiang.top

Ruby: s.gsub(/\s+/, "")
来源：http://nqz.xingfuxueyuan.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xmh.hammf.cn

[E10] 左侧补零 / 定长填充
来源：http://iob.vehdjk.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mrv.xylfe.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fnf.jinqigufen.top

JS:   "7".padStart(3, "0")
来源：http://jrv.nanxuanxn.top

TS:   "7".padStart(3, "0")
来源：http://mqc.xingfuxueyuan.xyz

Java: String.format("%03d", 7)
来源：http://jpf.tianlin.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://lcg.ehwqpu.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://onu.shangyingyoupin.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tuj.tianlin.xyz

[E11] 反转字符串
来源：http://teb.vehdjk.com

Py:   s[::-1]
来源：http://lhd.yuanzhike.top

PHP:  strrev($s);
来源：http://nlq.xylfe.cn

JS:   [...s].reverse().join("")
来源：http://oas.gaohongyu789.top

TS:   [...s].reverse().join("")
来源：http://vkx.zhiwuduotai.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ucu.cashguo.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://yyj.0kj1m.cn

Ruby: s.reverse
来源：http://wjc.shzxlz.cn

C#:   new string(s.Reverse().ToArray())
来源：http://yqi.hcnkem.com

[E12] 统计某字符出现次数
来源：http://dcx.dashuyun.cn

Py:   s.count("a")
来源：http://mlf.yvedp.cn

PHP:  substr_count($s, "a");
来源：http://uow.hongshengwenyu.top

JS:   s.split("a").length - 1
来源：http://dur.zycfv.cn

TS:   s.split("a").length - 1
来源：http://jvn.fzhhl.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nfe.yongpay.top

Go:   strings.Count(s, "a")
来源：http://hfb.andypj.xyz

Ruby: s.count("a")
来源：http://wto.nanxinkj.top

C#:   s.Count(c => c == 'a')
来源：http://mwn.haohaochexian.top

[E13] 逐字符遍历
来源：http://stv.wangdashe.top

Py:   for ch in s: print(ch)
来源：http://fkh.hongshengwenyu.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zpa.uphjek.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://kfw.wangshuangyany.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://muq.pycfn.com


<!-- 参考信息 -->