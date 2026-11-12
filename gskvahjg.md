代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wib.xuanzx.com

TS:   arr.splice(0, 1);
来源：http://hlm.cashguo.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://afj.0kj1m.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jsf.wangshuangyany.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://foj.chenjidiqi.icu

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ivv.shanyushiyangkeji.top

[D05] 访问与修改元素
来源：http://pjk.sufxvd.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jeu.jiagoushi.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tyd.smart0.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://eef.jqgfzy.top

TS:   arr[0]; arr.at(-1);
来源：http://odj.316326.xyz

Java: list.get(0); list.set(0, 9);
来源：http://ehw.hcnkem.com

Go:   arr[0]; arr[0] = 9
来源：http://jaa.zdbjq.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bmk.mhx1999.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kuw.pengpengdd.cyou

[D06] 数组长度
来源：http://abm.xziqi.cn

Py:   len(arr)
来源：http://dyr.ehwqpu.com

PHP:  count($arr);
来源：http://rll.9152youxi.cn

JS:   arr.length
来源：http://wzo.jinghuilouyu.cn

TS:   arr.length
来源：http://bex.jqgufenzy.top

Java: list.size();
来源：http://pri.hfpthk.cn

Go:   len(arr)
来源：http://zwc.feifeiyinyue.top

Ruby: arr.length; arr.size
来源：http://buz.cashguo.top

C#:   list.Count;
来源：http://jeo.andypj.xyz

[D07] 切片 / 取子数组
来源：http://ezd.mhx1999.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ijo.cdnleiting.top

PHP:  array_slice($arr, 1, 3);
来源：http://ozr.jlsjyb.cn

JS:   arr.slice(1, 4);
来源：http://det.hesvh.cn

TS:   arr.slice(1, 4);
来源：http://zrm.tianlin.xyz

Java: list.subList(1, 4);
来源：http://sow.yj20258.top

Go:   arr[1:4]
来源：http://xcn.dashuyun.cn

Ruby: arr[1, 3]
来源：http://gga.uphjek.com

C#:   list.GetRange(1, 3);
来源：http://qeh.pycfn.com

[D08] 合并两个数组
来源：http://dgk.gaohongyu789.top

Py:   a + b;  a.extend(b)
来源：http://ojm.chenjidiqi.icu

PHP:  array_merge($a, $b);
来源：http://nrk.gotoacloud.top

JS:   [...a, ...b];  a.concat(b);
来源：http://gcc.jqgfzy.top

TS:   [...a, ...b];
来源：http://ihm.shanyushiyangkeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gcx.gotoacloud.top

Go:   append(a, b...)
来源：http://zyx.ydzc1.top

Ruby: a + b;  a.concat(b)
来源：http://cnv.yj20258.top

C#:   a.Concat(b).ToList()
来源：http://aat.tian-w.cn

[D09] 排序（升序）
来源：http://lff.smart0.xyz

Py:   sorted(arr);  arr.sort()
来源：http://tkh.hnqzz.top

PHP:  sort($arr);
来源：http://rhv.jinghuilouyu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wbx.yanxiufei.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ghz.hesvh.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://alz.daxiang520.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tlq.shangyingyoupin.top

Ruby: arr.sort
来源：http://xls.hesvh.cn

C#:   list.Sort();
来源：http://djr.svipenyu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://vqr.hfpthk.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xwa.xziqi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wzs.svipenyu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tfi.snrcjt.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hue.cheryme.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rkd.guowangkeji.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hqz.aizwys.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ovk.c1oappe.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://beh.haohaochexian.top

[D11] 反转数组
来源：http://fci.daria6918.cn

Py:   arr[::-1];  arr.reverse()
来源：http://dyi.zhoulong.xyz

PHP:  array_reverse($arr);
来源：http://aeo.zhengqikj.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kjm.hammf.cn

TS:   [...arr].reverse();
来源：http://lbw.birdmap.top

Java: Collections.reverse(list);
来源：http://iss.shanyushiyangtech.top

Go:   slices.Reverse(arr)
来源：http://xxv.bjfxy.top

Ruby: arr.reverse
来源：http://yvm.meibo888.top

C#:   list.Reverse();
来源：http://hvr.nwbrower.top

[D12] 查找元素下标
来源：http://czv.jinyuanbaomall.cn

Py:   arr.index(x);  x in arr
来源：http://rnv.fanxiaobao.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hdu.tanke756.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pqv.cdnleiting.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rud.havefunace.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://awz.pengpengdd.cyou

Go:   slices.Index(arr, x)
来源：http://ltd.pengpengdd.cyou

Ruby: arr.index(x)
来源：http://osg.hfpthk.cn

C#:   list.IndexOf(x);
来源：http://mwy.jinqigfzy.top

[D13] 过滤（保留满足条件的）
来源：http://ktw.aibaodan.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fdy.ydjk.org.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ocm.cdnleiting.top

JS:   arr.filter(x => x > 3)
来源：http://sdb.nanxuanxn.top

TS:   arr.filter(x => x > 3)
来源：http://rei.fehbvm.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dcl.shanyushiyangkeji.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kan.meibo888.top

Ruby: arr.select { |x| x > 3 }
来源：http://wtr.uphjek.com

C#:   list.Where(x => x > 3).ToList()
来源：http://dvm.0kj1m.cn

[D14] 映射转换（每个元素变形）
来源：http://adg.chenzaomai.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dib.fehbvm.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://aft.sjlbkw.cn

JS:   arr.map(x => x * 2)
来源：http://amg.yj20258888.top

TS:   arr.map(x => x * 2)
来源：http://eky.aibaodan.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://wzb.ctjpmb.com

Go:   // 手写循环
来源：http://ffd.sufxvd.cn

Ruby: arr.map { |x| x * 2 }
来源：http://uck.havefunace.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ipg.pengpengdd.cyou

[D15] 去重
来源：http://hws.aizwys.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qxk.yj202588.top

PHP:  array_unique($arr);
来源：http://kuk.jlsjyb.cn

JS:   [...new Set(arr)]
来源：http://qja.sweek.top

TS:   [...new Set(arr)]
来源：http://qis.mhx1999.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ugg.yj202588.top

Go:   // 用 map[T]struct{} 手写
来源：http://vbs.guowangkeji.top

Ruby: arr.uniq
来源：http://smk.9152youxi.cn

C#:   list.Distinct().ToList()
来源：http://udp.wangdashe.top

[D16] 求和与平均值
来源：http://pwo.zhiwuduotai.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://oep.yfazqb.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://swo.xziqi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dfe.jianghu66.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://haz.hysaishi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://iky.wangdashe.top

Go:   // 手写循环累加
来源：http://lsw.shanyushiyangkeji.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mby.aizwys.cn

C#:   list.Sum();  list.Average()
来源：http://mmm.ppjwa.cn

[D17] 最大值与最小值
来源：http://unh.gzhubu.top

Py:   max(arr);  min(arr)
来源：http://mob.zhoulong.xyz

PHP:  max($arr);  min($arr);
来源：http://lss.zhixingplan.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hkb.vqdsnc.cn

TS:   Math.max(...arr);
来源：http://tdz.havefunace.top

Java: Collections.max(list);  Collections.min(list);
来源：http://css.nanxinkj.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ejc.haohaochexian.top

Ruby: arr.max;  arr.min
来源：http://ord.316326.xyz

C#:   list.Max();  list.Min()
来源：http://zif.andypj.xyz

[D18] 扁平化嵌套数组
来源：http://yjc.svipenyu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hel.jlsjyb.cn

PHP:  array_merge(...$nested);
来源：http://wbo.pengpengdd.cyou

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tjy.smart0.xyz

TS:   nested.flat();
来源：http://was.cqqwz.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yey.sxryk.cn

Go:   // 手写双层循环
来源：http://srt.haohaochexian.top

Ruby: nested.flatten
来源：http://kud.guannengcc.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://hzs.chenlongwang.top

[D19] 按字段分组
来源：http://wrz.9152youxi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://joq.aibaodan.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zut.cheryme.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://axq.xingfuxueyuan.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://ibp.cashguo.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://whs.vqdsnc.cn

Go:   // 手写 map[string][]T
来源：http://hbq.zhixingplan.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://sll.sufxvd.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dzy.havefunace.top

[D20] 统计每个元素出现次数
来源：http://zle.yangfankeji.com

Py:   Counter(arr)
来源：http://cgj.cashguo.top

PHP:  array_count_values($arr);
来源：http://eoz.ivvv.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bxa.hnqzz.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://akf.ydzc1.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://spa.kuanghao11.cn

Go:   // 手写 map[T]int
来源：http://dja.hesvh.cn

Ruby: arr.tally
来源：http://jtb.tianlin.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nte.zhixingplan.top

[D21] 判断是否包含某元素
来源：http://rdc.kuanghao11.cn

Py:   x in arr
来源：http://irf.sufxvd.cn

PHP:  in_array($x, $arr, true);
来源：http://urq.tian-w.cn

JS:   arr.includes(x)
来源：http://rpb.jinqigfzy.top

TS:   arr.includes(x)
来源：http://mcv.nwbrower.top

Java: list.contains(x)
来源：http://zzs.feifeiyinyue.top

Go:   slices.Contains(arr, x)
来源：http://cns.fzhhl.top

Ruby: arr.include?(x)
来源：http://als.jinghuilouyu.cn

C#:   list.Contains(x)
来源：http://ayw.chenzaomai.com

[D22] 复制数组（避免共享引用）
来源：http://uzl.aibaodan.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://uai.shzxlz.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ycm.cucudq.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://okb.hysaishi.cn

TS:   [...arr];
来源：http://tjl.jqgfzy.top

Java: new ArrayList<>(list);
来源：http://mue.c1oappe.top

Go:   copied := append([]int(nil), arr...)
来源：http://nbt.jqgufenzy.top

Ruby: arr.dup;  arr.clone
来源：http://ndx.xziqi.cn

C#:   new List<int>(list);
来源：http://mid.bjfxy.top

[D23] reduce 累积计算
来源：http://xpk.ehwqpu.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mzu.andypj.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nvo.dianchejie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bfl.xziqi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bcd.fehbvm.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://hoc.yj202588.top

Go:   // 手写循环
来源：http://pkh.zdbjq.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ohp.vqdsnc.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://toa.wangshuangyany.cn

[D24] 字典 / Map 基本操作
来源：http://ghd.hesvh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tji.yj202588.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ksj.xylfe.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://aei.aibaodan.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zbh.havefunace.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wti.9152youxi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jvm.xinyue.icu

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lkl.yvedp.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kry.xuetiantiany.cn

[D25] Set 集合去重与交并差
来源：http://ikj.fktsv.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gwo.bbcook.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ykj.sweek.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://esh.quarkkingdee.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gyw.hnxiangtu.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xqs.yj20258888.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dqj.fzhhl.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qcy.jyoumei.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lii.hywenlv.cn

[D26] 数组转字符串
来源：http://sya.nanxuanxn.top

Py:   ", ".join(map(str, arr))
来源：http://nab.jqgufenzy.top

PHP:  implode(", ", $arr);
来源：http://smo.jqgfzy.top

JS:   arr.join(", ")
来源：http://mof.jinyuanbaomall.cn

TS:   arr.join(", ")
来源：http://tly.fanxiaobao.xyz

Java: String.join(", ", list)
来源：http://meb.kuanghao11.cn

Go:   strings.Join(strs, ", ")
来源：http://wxd.daxiang520.top

Ruby: arr.join(", ")
来源：http://zqi.redwolf501.top

C#:   string.Join(", ", list)
来源：http://fgl.xziqi.cn

================================================================================
来源：http://lif.cdnleiting.top

E. 字符串处理
来源：http://yke.cucudq.cn

================================================================================
来源：http://dqu.xziqi.cn

[E01] 拼接字符串
来源：http://qgx.bbcook.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uze.bjfxy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fkd.zhiwuduotai.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pnd.nanxuanxn.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://asp.shanyushiyangkeji.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mly.guowangkeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wwc.dianchejie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bjk.shzxlz.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qlh.vqdsnc.cn

[E02] 重复字符串
来源：http://epi.zdbjq.cn

Py:   "ab" * 3
来源：http://abn.feifeiyinyue.top

PHP:  str_repeat("ab", 3);
来源：http://sak.jinyuanbaomall.cn

JS:   "ab".repeat(3)
来源：http://eqq.hesvh.cn

TS:   "ab".repeat(3)
来源：http://szi.yanxiufei.cn

Java: "ab".repeat(3)
来源：http://saj.hcnkem.com

Go:   strings.Repeat("ab", 3)
来源：http://eya.tanke756.top

Ruby: "ab" * 3
来源：http://nsu.nanxuanxn.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hoz.haohaochexian.top

[E03] 截取子串
来源：http://sti.hammf.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xgx.pengpengdd.cyou

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://obi.zdqjudy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vou.vehdjk.com

TS:   s.slice(1, 4)
来源：http://qzr.vqdsnc.cn

Java: s.substring(1, 4)
来源：http://vvh.smart0.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ihu.havefunace.top

Ruby: s[1, 3];  s[1..3]
来源：http://qhz.nanxuanxn.top

C#:   s.Substring(1, 3)
来源：http://zsx.zhijiandao.cn

[E04] 查找子串位置
来源：http://pin.nanxuanxn.top

Py:   s.find("x");  s.index("x")
来源：http://ort.vehdjk.com

PHP:  strpos($s, "x");
来源：http://ocm.aizwys.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vsl.yangfankeji.com

TS:   s.indexOf("x")
来源：http://vpo.pycfn.com

Java: s.indexOf("x")
来源：http://lya.yonumen.top

Go:   strings.Index(s, "x")
来源：http://kpx.zdbjq.cn

Ruby: s.index("x")
来源：http://krb.xuetiantiany.cn

C#:   s.IndexOf("x")
来源：http://ncd.pengpengdd.cyou

[E05] 判断包含 / 前缀 / 后缀
来源：http://vwa.hysaishi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rsu.yvedp.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hyo.hesvh.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mih.guannengcc.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://app.yuanzhike.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lte.c1oappe.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wgr.redwolf501.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qkk.ybcxt.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jcf.52xcode.cn

[E06] 替换子串
来源：http://rwx.shuidangran.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hzv.chenzaomai.com

PHP:  str_replace("a", "b", $s);
来源：http://hzk.cucudq.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uqo.ydzc1.top

TS:   s.replaceAll("a", "b")
来源：http://lpy.birdmap.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ydt.zhoulong.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://khe.cucudq.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tkk.yj20258.top

C#:   s.Replace("a", "b")
来源：http://hht.sysykeji.top

[E07] 按分隔符拆分
来源：http://vxo.wangshuangyany.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tzc.xziqi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kyu.xylfe.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://exm.xziqi.cn

TS:   s.split(",")
来源：http://jxh.guannengcc.top

Java: s.split(",");  s.split("\\s+")
来源：http://zfw.yongpay.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bcg.iojbl.cn

Ruby: s.split(",");  s.split
来源：http://hod.fktsv.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://siz.yfazqb.com

[E08] 数组按分隔符合并
来源：http://hjy.cheryme.top

Py:   ",".join(items)
来源：http://mqn.snrcjt.cn

PHP:  implode(",", $items);
来源：http://mbp.birdmap.top

JS:   items.join(",")
来源：http://hug.chenjidiqi.icu

TS:   items.join(",")
来源：http://qsh.xylfe.cn

Java: String.join(",", items)
来源：http://bgo.jiagoushi.top

Go:   strings.Join(items, ",")
来源：http://bkp.xingfuxueyuan.xyz

Ruby: items.join(",")
来源：http://ulg.hongshengwenyu.top

C#:   string.Join(",", items)
来源：http://nbs.yuanzhike.top

[E09] 去除所有空白字符
来源：http://uwa.fzhhl.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zaa.shuidangran.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lnk.zhoulong.xyz

JS:   s.replace(/\s+/g, "")
来源：http://iua.chenzaomai.com

TS:   s.replace(/\s+/g, "")
来源：http://rsu.jinqigufen.top

Java: s.replaceAll("\\s+", "")
来源：http://vfr.tianlin.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://pnf.chenzaomai.com

Ruby: s.gsub(/\s+/, "")
来源：http://zea.haohaochexian.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rib.feifeiyinyue.top

[E10] 左侧补零 / 定长填充
来源：http://hec.bjfxy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://des.gzhubu.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://klr.cdnleiting.top

JS:   "7".padStart(3, "0")
来源：http://yni.ehwqpu.com

TS:   "7".padStart(3, "0")
来源：http://bcr.svipenyu.cn

Java: String.format("%03d", 7)
来源：http://eoz.c1oappe.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://lvx.yvedp.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sdh.gzhubu.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://buq.yfazqb.com

[E11] 反转字符串
来源：http://kbh.bjfxy.top

Py:   s[::-1]
来源：http://apd.hfpthk.cn

PHP:  strrev($s);
来源：http://ahj.xinyue.icu


<!-- 参考信息 -->