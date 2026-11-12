代发 wailian999

Py:   len(arr)
来源：http://irq.xinyue.icu

PHP:  count($arr);
来源：http://sio.ybcxt.top

JS:   arr.length
来源：http://waz.chenzaomai.com

TS:   arr.length
来源：http://apq.ehwqpu.com

Java: list.size();
来源：http://uxe.vehdjk.com

Go:   len(arr)
来源：http://wcj.havefunace.top

Ruby: arr.length; arr.size
来源：http://tjh.ehwqpu.com

C#:   list.Count;
来源：http://ary.yvedp.cn

[D07] 切片 / 取子数组
来源：http://ypt.yonumen.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vqx.redwolf501.top

PHP:  array_slice($arr, 1, 3);
来源：http://jck.zycfv.cn

JS:   arr.slice(1, 4);
来源：http://hfg.mhx1999.top

TS:   arr.slice(1, 4);
来源：http://zwx.hongshengwenyu.top

Java: list.subList(1, 4);
来源：http://goj.cheryme.top

Go:   arr[1:4]
来源：http://jiu.0kj1m.cn

Ruby: arr[1, 3]
来源：http://osj.yanxiufei.cn

C#:   list.GetRange(1, 3);
来源：http://crv.hammf.cn

[D08] 合并两个数组
来源：http://ntv.fengsongda.top

Py:   a + b;  a.extend(b)
来源：http://jgm.gzhubu.top

PHP:  array_merge($a, $b);
来源：http://sqs.smart0.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://swn.vehdjk.com

TS:   [...a, ...b];
来源：http://ybg.yuxming.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vzz.sysykeji.top

Go:   append(a, b...)
来源：http://sek.xuetiantiany.cn

Ruby: a + b;  a.concat(b)
来源：http://rrm.vehdjk.com

C#:   a.Concat(b).ToList()
来源：http://ffw.yuanzhike.top

[D09] 排序（升序）
来源：http://kai.daria6918.cn

Py:   sorted(arr);  arr.sort()
来源：http://ylz.tarul.cn

PHP:  sort($arr);
来源：http://ywd.tian-w.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cyw.jinqigfzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://tsv.yonumen.top

Java: Collections.sort(list);  list.sort(null);
来源：http://gks.jinqigufen.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hng.sxryk.cn

Ruby: arr.sort
来源：http://gcq.zhiwuduotai.top

C#:   list.Sort();
来源：http://ota.guowangkeji.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://lpx.kuanghao11.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://evb.wangdashe.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hqt.wangshuangyany.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://smt.jinghuilouyu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bfa.cdnleiting.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zke.dashuyun.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://aji.9152youxi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qwq.ydjk.org.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bmq.ctjpmb.com

[D11] 反转数组
来源：http://dxx.sjlbkw.cn

Py:   arr[::-1];  arr.reverse()
来源：http://jix.sjlbkw.cn

PHP:  array_reverse($arr);
来源：http://wps.vehdjk.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ufu.bbcook.cn

TS:   [...arr].reverse();
来源：http://hnk.jyoumei.cn

Java: Collections.reverse(list);
来源：http://uyf.52xcode.cn

Go:   slices.Reverse(arr)
来源：http://xbt.yfazqb.com

Ruby: arr.reverse
来源：http://iyv.meibo888.top

C#:   list.Reverse();
来源：http://ysn.yueranfly.top

[D12] 查找元素下标
来源：http://cki.chenjidiqi.icu

Py:   arr.index(x);  x in arr
来源：http://gee.chenzaomai.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dax.jinghuilouyu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gld.cdnleiting.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://osx.xuetiantiany.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ujh.havefunace.top

Go:   slices.Index(arr, x)
来源：http://aho.tian-w.cn

Ruby: arr.index(x)
来源：http://iuk.nwbrower.top

C#:   list.IndexOf(x);
来源：http://mri.jinghuilouyu.cn

[D13] 过滤（保留满足条件的）
来源：http://jzw.jinyuanbaomall.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hjq.aibaodan.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jmt.yvedp.cn

JS:   arr.filter(x => x > 3)
来源：http://lry.jqgufenzy.top

TS:   arr.filter(x => x > 3)
来源：http://air.jianghu66.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nco.fktsv.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ucu.hcnkem.com

Ruby: arr.select { |x| x > 3 }
来源：http://grs.xinyue.icu

C#:   list.Where(x => x > 3).ToList()
来源：http://tep.quarkkingdee.top

[D14] 映射转换（每个元素变形）
来源：http://vku.yuxming.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kyg.cdnleiting.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zqs.hnxiangtu.top

JS:   arr.map(x => x * 2)
来源：http://wgp.pengpengdd.cyou

TS:   arr.map(x => x * 2)
来源：http://mkg.chenjidiqi.icu

Java: list.stream().map(x -> x * 2).toList()
来源：http://lpg.hywenlv.cn

Go:   // 手写循环
来源：http://adn.ydzc1.top

Ruby: arr.map { |x| x * 2 }
来源：http://dwk.zdbjq.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ile.zhaomingkeji.xyz

[D15] 去重
来源：http://trv.c1oappe.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ary.yanxiufei.cn

PHP:  array_unique($arr);
来源：http://ziq.yueranfly.top

JS:   [...new Set(arr)]
来源：http://pvs.uphjek.com

TS:   [...new Set(arr)]
来源：http://jbl.zhoulong.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fsh.sxryk.cn

Go:   // 用 map[T]struct{} 手写
来源：http://gyt.daria6918.cn

Ruby: arr.uniq
来源：http://zbr.jinghuilouyu.cn

C#:   list.Distinct().ToList()
来源：http://phy.cucudq.cn

[D16] 求和与平均值
来源：http://eiz.9152youxi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qar.nwbrower.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ptq.zhoulong.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vou.jyoumei.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sjq.smart0.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://meh.redwolf501.top

Go:   // 手写循环累加
来源：http://uge.xingfuxueyuan.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qvb.tianlin.xyz

C#:   list.Sum();  list.Average()
来源：http://kmq.zhaomingkeji.xyz

[D17] 最大值与最小值
来源：http://vnd.yvedp.cn

Py:   max(arr);  min(arr)
来源：http://uru.yongpay.top

PHP:  max($arr);  min($arr);
来源：http://nfu.yanxiufei.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gdb.shanyushiyangtech.top

TS:   Math.max(...arr);
来源：http://pwb.jlsjyb.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://pci.gaohongyu789.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yjw.andypj.xyz

Ruby: arr.max;  arr.min
来源：http://lia.tian-w.cn

C#:   list.Max();  list.Min()
来源：http://cec.aizwys.cn

[D18] 扁平化嵌套数组
来源：http://nim.pycfn.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://twe.tanke756.top

PHP:  array_merge(...$nested);
来源：http://llx.zhaomingkeji.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ojb.316326.xyz

TS:   nested.flat();
来源：http://zwa.ivvv.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tyg.ybcxt.top

Go:   // 手写双层循环
来源：http://xeq.gotoacloud.top

Ruby: nested.flatten
来源：http://mrd.yuxming.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ajp.cheryme.top

[D19] 按字段分组
来源：http://ecq.jianghu66.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jkp.gzhubu.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tgy.wangdashe.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://czn.wangdashe.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://gzc.epnwcf.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ryx.hammf.cn

Go:   // 手写 map[string][]T
来源：http://pjc.cucudq.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://bty.zdbjq.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://npq.hnxiangtu.top

[D20] 统计每个元素出现次数
来源：http://ijj.ctjpmb.com

Py:   Counter(arr)
来源：http://csg.tianlin.xyz

PHP:  array_count_values($arr);
来源：http://qni.chenjidiqi.icu

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sip.hywenlv.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xcl.kuanghao11.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://krs.jinghuilouyu.cn

Go:   // 手写 map[T]int
来源：http://imb.gogol.net.cn

Ruby: arr.tally
来源：http://jaj.ppjwa.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mnj.vqdsnc.cn

[D21] 判断是否包含某元素
来源：http://muw.yvedp.cn

Py:   x in arr
来源：http://uui.cashguo.top

PHP:  in_array($x, $arr, true);
来源：http://nwf.xingfuxueyuan.xyz

JS:   arr.includes(x)
来源：http://zhk.svipenyu.cn

TS:   arr.includes(x)
来源：http://upp.tanke756.top

Java: list.contains(x)
来源：http://bqo.jqgfzy.top

Go:   slices.Contains(arr, x)
来源：http://tlf.zhijiandao.cn

Ruby: arr.include?(x)
来源：http://ezz.xuanzx.com

C#:   list.Contains(x)
来源：http://tll.hfpthk.cn

[D22] 复制数组（避免共享引用）
来源：http://xmw.uphjek.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gpv.xylfe.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hvi.sufxvd.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vvd.gotoacloud.top

TS:   [...arr];
来源：http://zgm.zdbjq.cn

Java: new ArrayList<>(list);
来源：http://fsd.tian-w.cn

Go:   copied := append([]int(nil), arr...)
来源：http://hvy.jqgfzy.top

Ruby: arr.dup;  arr.clone
来源：http://ven.zhijiandao.cn

C#:   new List<int>(list);
来源：http://uoz.jyoumei.cn

[D23] reduce 累积计算
来源：http://xvr.svipenyu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fee.nanxuanxn.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://koe.ydzc1.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qlc.daxiang520.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://aow.cqqwz.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://oiu.ybcxt.top

Go:   // 手写循环
来源：http://del.zdqjudy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ekj.zdbjq.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://twf.ydzc1.top

[D24] 字典 / Map 基本操作
来源：http://bcn.jyoumei.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tbt.jqgufenzy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rrs.nwbrower.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sje.tian-w.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://oup.jianghu66.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://isr.hongshengwenyu.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://quc.bbcook.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rxg.jlsjyb.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dvf.hesvh.cn

[D25] Set 集合去重与交并差
来源：http://zon.cucudq.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yzz.316326.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://doi.jinyuanbaomall.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bdt.wangshuangyany.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lyv.dianchejie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://krp.bjfxy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nay.aizwys.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bbr.dashuyun.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zny.zhijiandao.cn

[D26] 数组转字符串
来源：http://gjq.birdmap.top

Py:   ", ".join(map(str, arr))
来源：http://caw.snrcjt.cn

PHP:  implode(", ", $arr);
来源：http://jte.zycfv.cn

JS:   arr.join(", ")
来源：http://oti.jinghuilouyu.cn

TS:   arr.join(", ")
来源：http://hfy.sufxvd.cn

Java: String.join(", ", list)
来源：http://hbt.fktsv.cn

Go:   strings.Join(strs, ", ")
来源：http://isf.yanxiufei.cn

Ruby: arr.join(", ")
来源：http://aix.sweek.top

C#:   string.Join(", ", list)
来源：http://yee.vqdsnc.cn

================================================================================
来源：http://xeu.ctjpmb.com

E. 字符串处理
来源：http://xoo.andypj.xyz

================================================================================
来源：http://qhp.xinyue.icu

[E01] 拼接字符串
来源：http://brm.shzxlz.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yrf.cdnleiting.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://waf.fehbvm.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qiu.yongpay.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kfl.ybcxt.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://iew.sweek.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pfw.zhoulong.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nva.hnqzz.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xec.zycfv.cn

[E02] 重复字符串
来源：http://qrl.vehdjk.com

Py:   "ab" * 3
来源：http://uad.vehdjk.com

PHP:  str_repeat("ab", 3);
来源：http://tiy.cqqwz.cn

JS:   "ab".repeat(3)
来源：http://iet.jianghu66.top

TS:   "ab".repeat(3)
来源：http://gtj.mhx1999.top

Java: "ab".repeat(3)
来源：http://nsp.svipenyu.cn

Go:   strings.Repeat("ab", 3)
来源：http://nsi.ydzc1.top

Ruby: "ab" * 3
来源：http://rvj.ydjk.org.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yjp.wangdashe.top

[E03] 截取子串
来源：http://rdq.cheryme.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kxx.hongshengwenyu.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ghm.jinqigfzy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tgf.yfazqb.com

TS:   s.slice(1, 4)
来源：http://rqx.hcnkem.com

Java: s.substring(1, 4)
来源：http://dfp.fktsv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://etb.c1oappe.top

Ruby: s[1, 3];  s[1..3]
来源：http://jak.fehbvm.com

C#:   s.Substring(1, 3)
来源：http://ffk.chenlongwang.top

[E04] 查找子串位置
来源：http://tvg.nanxinkj.top

Py:   s.find("x");  s.index("x")
来源：http://jve.andypj.xyz

PHP:  strpos($s, "x");
来源：http://xab.zdbjq.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mxg.0kj1m.cn

TS:   s.indexOf("x")
来源：http://lvo.kuanghao11.cn

Java: s.indexOf("x")
来源：http://hjp.meibo888.top

Go:   strings.Index(s, "x")
来源：http://hnh.kuanghao11.cn

Ruby: s.index("x")
来源：http://wiq.tianlin.xyz

C#:   s.IndexOf("x")
来源：http://eiz.jqgfzy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://pwd.iojbl.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fxp.zycfv.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bds.hammf.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sci.xylfe.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mti.yangfankeji.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://anj.jinghuilouyu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hzt.shanyushiyangkeji.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lky.shuidangran.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xjk.xuetiantiany.cn

[E06] 替换子串
来源：http://inv.yuanzhike.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://era.jlsjyb.cn

PHP:  str_replace("a", "b", $s);
来源：http://dvb.yuxming.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zmi.birdmap.top

TS:   s.replaceAll("a", "b")
来源：http://zvn.chenlongwang.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ttj.iojbl.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hfn.hongshengwenyu.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wed.aibaodan.cn

C#:   s.Replace("a", "b")
来源：http://bns.feifeiyinyue.top

[E07] 按分隔符拆分
来源：http://eec.cashguo.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fcy.daxiang520.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qkx.ybcxt.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://zhp.sysykeji.top

TS:   s.split(",")
来源：http://ids.sjlbkw.cn

Java: s.split(",");  s.split("\\s+")
来源：http://bbv.tarul.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://svn.316326.xyz

Ruby: s.split(",");  s.split
来源：http://ehc.redwolf501.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://puv.yuxming.cn

[E08] 数组按分隔符合并
来源：http://jas.zhaomingkeji.xyz

Py:   ",".join(items)
来源：http://wzq.haohaochexian.top

PHP:  implode(",", $items);
来源：http://mvc.fzhhl.top

JS:   items.join(",")
来源：http://xqm.kuanghao11.cn

TS:   items.join(",")
来源：http://wsc.chenlongwang.top

Java: String.join(",", items)
来源：http://ycc.tian-w.cn

Go:   strings.Join(items, ",")
来源：http://acn.jinqigufen.top

Ruby: items.join(",")
来源：http://atg.52xcode.cn

C#:   string.Join(",", items)
来源：http://prs.ctjpmb.com

[E09] 去除所有空白字符
来源：http://wgt.jianghu66.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tiw.zhengqikj.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nfw.kuanghao11.cn

JS:   s.replace(/\s+/g, "")
来源：http://pnp.xuetiantiany.cn

TS:   s.replace(/\s+/g, "")
来源：http://xbo.hywenlv.cn

Java: s.replaceAll("\\s+", "")
来源：http://oqb.jqgfzy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ltn.ppjwa.cn

Ruby: s.gsub(/\s+/, "")
来源：http://fag.svipenyu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kff.aibaodan.cn

[E10] 左侧补零 / 定长填充
来源：http://oeo.pycfn.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hsa.wangshuangyany.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lxm.yongpay.top

JS:   "7".padStart(3, "0")
来源：http://kbg.bjfxy.top

TS:   "7".padStart(3, "0")
来源：http://sis.sysykeji.top

Java: String.format("%03d", 7)
来源：http://nnd.uphjek.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://owe.chenlongwang.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pji.yuxming.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://oim.gogol.net.cn

[E11] 反转字符串
来源：http://cdi.wangshuangyany.cn

Py:   s[::-1]
来源：http://itn.ydzc1.top

PHP:  strrev($s);
来源：http://qpw.jianghu66.top

JS:   [...s].reverse().join("")
来源：http://eyg.tarul.cn

TS:   [...s].reverse().join("")
来源：http://nmk.yj202588.top

Java: new StringBuilder(s).reverse().toString()
来源：http://qxq.cucudq.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://dgj.hongshengwenyu.top

Ruby: s.reverse
来源：http://chv.dashuyun.cn

C#:   new string(s.Reverse().ToArray())
来源：http://bql.ppjwa.cn

[E12] 统计某字符出现次数
来源：http://fmq.hongshengwenyu.top

Py:   s.count("a")
来源：http://ooa.zhoulong.xyz

PHP:  substr_count($s, "a");
来源：http://rmn.xinyue.icu

JS:   s.split("a").length - 1
来源：http://kzj.birdmap.top

TS:   s.split("a").length - 1
来源：http://nps.snrcjt.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://uqy.sysykeji.top

Go:   strings.Count(s, "a")
来源：http://ezj.yuanzhike.top

Ruby: s.count("a")
来源：http://jdz.xylfe.cn

C#:   s.Count(c => c == 'a')
来源：http://jle.aizwys.cn

[E13] 逐字符遍历
来源：http://giw.vqdsnc.cn


<!-- 参考信息 -->