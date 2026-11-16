代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://bqt.hywenlv.cn

Ruby: arr = [1, 2, 3]
来源：http://uye.shuidangran.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://agp.pengpengdd.cyou

[D02] 追加元素到末尾
来源：http://vna.cheryme.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vxb.shuidangran.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ssm.shangyingyoupin.top

JS:   arr.push(4);
来源：http://bqg.sweek.top

TS:   arr.push(4);
来源：http://exd.hysaishi.cn

Java: list.add(4);
来源：http://itc.9152youxi.cn

Go:   arr = append(arr, 4)
来源：http://bfj.hammf.cn

Ruby: arr << 4; arr.push(5)
来源：http://ood.meibo888.top

C#:   list.Add(4);
来源：http://fvr.xuetiantiany.cn

[D03] 在指定位置插入元素
来源：http://tlv.sxryk.cn

Py:   arr.insert(0, 0)
来源：http://gjq.0kj1m.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gmo.haohaochexian.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gfq.sjlbkw.cn

TS:   arr.splice(0, 0, 0);
来源：http://tdr.zhengqikj.top

Java: list.add(0, 0);
来源：http://luj.fehbvm.com

Go:   arr = append([]int{0}, arr...)
来源：http://vkm.tarul.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ddc.tianlin.xyz

C#:   list.Insert(0, 0);
来源：http://mbf.yongpay.top

[D04] 删除元素
来源：http://oha.zhixingplan.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dvu.tianlin.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wyc.ctjpmb.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ilf.hnxiangtu.top

TS:   arr.splice(0, 1);
来源：http://kbw.gzhubu.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://olm.wangdashe.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mzp.zhengqikj.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://epa.yuxming.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nlo.ppjwa.cn

[D05] 访问与修改元素
来源：http://zbr.zhiwuduotai.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bsx.yfazqb.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ngp.sufxvd.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ebo.ctjpmb.com

TS:   arr[0]; arr.at(-1);
来源：http://eav.hywenlv.cn

Java: list.get(0); list.set(0, 9);
来源：http://dan.iojbl.cn

Go:   arr[0]; arr[0] = 9
来源：http://yxp.9152youxi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lpy.ywan-chungtsiang.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jti.ppjwa.cn

[D06] 数组长度
来源：http://wpz.shuidangran.top

Py:   len(arr)
来源：http://kev.sjlbkw.cn

PHP:  count($arr);
来源：http://cru.daxiang520.top

JS:   arr.length
来源：http://xgq.ydzc1.top

TS:   arr.length
来源：http://zwk.0kj1m.cn

Java: list.size();
来源：http://ndy.52xcode.cn

Go:   len(arr)
来源：http://uoe.xziqi.cn

Ruby: arr.length; arr.size
来源：http://xoh.xziqi.cn

C#:   list.Count;
来源：http://ooe.ppjwa.cn

[D07] 切片 / 取子数组
来源：http://ftk.smart0.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qnx.zhijiandao.cn

PHP:  array_slice($arr, 1, 3);
来源：http://geg.sxryk.cn

JS:   arr.slice(1, 4);
来源：http://pai.zhongyouzk.top

TS:   arr.slice(1, 4);
来源：http://rsc.sysykeji.top

Java: list.subList(1, 4);
来源：http://jcu.gogol.net.cn

Go:   arr[1:4]
来源：http://exd.ctjpmb.com

Ruby: arr[1, 3]
来源：http://ati.jqgufenzy.top

C#:   list.GetRange(1, 3);
来源：http://hpu.birdmap.top

[D08] 合并两个数组
来源：http://kmm.316326.xyz

Py:   a + b;  a.extend(b)
来源：http://jdt.zycfv.cn

PHP:  array_merge($a, $b);
来源：http://ieu.jinqigfzy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://wka.daxiang520.top

TS:   [...a, ...b];
来源：http://ose.yanxiufei.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jlr.yongpay.top

Go:   append(a, b...)
来源：http://mbe.kuanghao11.cn

Ruby: a + b;  a.concat(b)
来源：http://ayo.yj20258888.top

C#:   a.Concat(b).ToList()
来源：http://yfq.yvedp.cn

[D09] 排序（升序）
来源：http://yzg.ppjwa.cn

Py:   sorted(arr);  arr.sort()
来源：http://lwa.andypj.xyz

PHP:  sort($arr);
来源：http://svc.jqgfzy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fte.yj20258888.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://jxm.ehwqpu.com

Java: Collections.sort(list);  list.sort(null);
来源：http://lte.jyoumei.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xrn.ppjwa.cn

Ruby: arr.sort
来源：http://jcz.daxiang520.top

C#:   list.Sort();
来源：http://uoa.c1oappe.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ceo.yfazqb.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://toi.xuanzx.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bxn.zhixingplan.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lrc.cdnleiting.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://adb.yuanzhike.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zqq.cashguo.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nqq.guannengcc.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ize.zdbjq.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kwd.redwolf501.top

[D11] 反转数组
来源：http://jvx.ybcxt.top

Py:   arr[::-1];  arr.reverse()
来源：http://iwx.daxiang520.top

PHP:  array_reverse($arr);
来源：http://mne.cashguo.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://egy.wangshuangyany.cn

TS:   [...arr].reverse();
来源：http://qqn.zhongyouzk.top

Java: Collections.reverse(list);
来源：http://acx.guannengcc.top

Go:   slices.Reverse(arr)
来源：http://okj.havefunace.top

Ruby: arr.reverse
来源：http://fwt.quarkkingdee.top

C#:   list.Reverse();
来源：http://gmq.zhaomingkeji.xyz

[D12] 查找元素下标
来源：http://jhu.redwolf501.top

Py:   arr.index(x);  x in arr
来源：http://dwe.andypj.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mqr.zhiwuduotai.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gmy.jyoumei.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://joa.vehdjk.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vyc.fengsongda.top

Go:   slices.Index(arr, x)
来源：http://dsf.gogol.net.cn

Ruby: arr.index(x)
来源：http://pyh.zhixingplan.top

C#:   list.IndexOf(x);
来源：http://sce.ivvv.top

[D13] 过滤（保留满足条件的）
来源：http://kvl.yj20258.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pii.daxiang520.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ynf.jqgufenzy.top

JS:   arr.filter(x => x > 3)
来源：http://zit.gogol.net.cn

TS:   arr.filter(x => x > 3)
来源：http://xhf.jlsjyb.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bxj.gzhubu.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zif.aizwys.cn

Ruby: arr.select { |x| x > 3 }
来源：http://dkd.hcnkem.com

C#:   list.Where(x => x > 3).ToList()
来源：http://yqb.iojbl.cn

[D14] 映射转换（每个元素变形）
来源：http://rfd.cucudq.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://afy.ctjpmb.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ixx.ctjpmb.com

JS:   arr.map(x => x * 2)
来源：http://jvr.tian-w.cn

TS:   arr.map(x => x * 2)
来源：http://qok.gotoacloud.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://jpj.jyoumei.cn

Go:   // 手写循环
来源：http://yyr.zhiwuduotai.top

Ruby: arr.map { |x| x * 2 }
来源：http://njb.hammf.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://vud.yfazqb.com

[D15] 去重
来源：http://gpv.yuxming.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nqo.yonumen.top

PHP:  array_unique($arr);
来源：http://yfh.gzhubu.top

JS:   [...new Set(arr)]
来源：http://emj.yonumen.top

TS:   [...new Set(arr)]
来源：http://hup.bbcook.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hzi.xinyue.icu

Go:   // 用 map[T]struct{} 手写
来源：http://avu.nanxuanxn.top

Ruby: arr.uniq
来源：http://fcp.xuanzx.com

C#:   list.Distinct().ToList()
来源：http://kuu.shangyingyoupin.top

[D16] 求和与平均值
来源：http://xbr.iojbl.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hqf.jianghu66.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zga.yonumen.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dqp.fzhhl.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lso.cashguo.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bts.vehdjk.com

Go:   // 手写循环累加
来源：http://avu.zdqjudy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://atp.fengsongda.top

C#:   list.Sum();  list.Average()
来源：http://yzi.yuxming.cn

[D17] 最大值与最小值
来源：http://tyx.xylfe.cn

Py:   max(arr);  min(arr)
来源：http://rla.tian-w.cn

PHP:  max($arr);  min($arr);
来源：http://sqm.hnqzz.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zzu.gzhubu.top

TS:   Math.max(...arr);
来源：http://mdw.pycfn.com

Java: Collections.max(list);  Collections.min(list);
来源：http://bkh.chenlongwang.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gje.0kj1m.cn

Ruby: arr.max;  arr.min
来源：http://tms.daria6918.cn

C#:   list.Max();  list.Min()
来源：http://ctk.shanyushiyangkeji.top

[D18] 扁平化嵌套数组
来源：http://czo.shzxlz.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jea.sxryk.cn

PHP:  array_merge(...$nested);
来源：http://ttg.jinqigufen.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bvr.wangdashe.top

TS:   nested.flat();
来源：http://ace.zhoulong.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://oub.pycfn.com

Go:   // 手写双层循环
来源：http://iuw.gzhubu.top

Ruby: nested.flatten
来源：http://onk.yangfankeji.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://naa.guannengcc.top

[D19] 按字段分组
来源：http://tsz.hammf.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ocf.dashuyun.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ojo.vehdjk.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xhy.xinyue.icu

TS:   Object.groupBy(arr, x => x.type)
来源：http://ptd.yangfankeji.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bqp.aibaodan.cn

Go:   // 手写 map[string][]T
来源：http://lub.chenzaomai.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://ldd.tarul.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gid.cqqwz.cn

[D20] 统计每个元素出现次数
来源：http://bfd.sjlbkw.cn

Py:   Counter(arr)
来源：http://brs.zhoulong.xyz

PHP:  array_count_values($arr);
来源：http://qol.jinghuilouyu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hbp.wangshuangyany.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qmg.xuetiantiany.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://krq.fanxiaobao.xyz

Go:   // 手写 map[T]int
来源：http://ilj.daxiang520.top

Ruby: arr.tally
来源：http://ccc.bbcook.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mkc.jyoumei.cn

[D21] 判断是否包含某元素
来源：http://jep.hesvh.cn

Py:   x in arr
来源：http://rxj.hnqzz.top

PHP:  in_array($x, $arr, true);
来源：http://noc.ywan-chungtsiang.top

JS:   arr.includes(x)
来源：http://pfs.sysykeji.top

TS:   arr.includes(x)
来源：http://qpo.zhongyouzk.top

Java: list.contains(x)
来源：http://ymd.fengsongda.top

Go:   slices.Contains(arr, x)
来源：http://nae.zhiwuduotai.top

Ruby: arr.include?(x)
来源：http://sgh.zhijiandao.cn

C#:   list.Contains(x)
来源：http://wuz.hongshengwenyu.top

[D22] 复制数组（避免共享引用）
来源：http://agn.hfpthk.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://oaz.yuxming.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xlj.tianlin.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nez.ctjpmb.com

TS:   [...arr];
来源：http://iva.shangyingyoupin.top

Java: new ArrayList<>(list);
来源：http://xuq.cdnleiting.top

Go:   copied := append([]int(nil), arr...)
来源：http://ldk.pengpengdd.cyou

Ruby: arr.dup;  arr.clone
来源：http://inv.vehdjk.com

C#:   new List<int>(list);
来源：http://owu.shanyushiyangtech.top

[D23] reduce 累积计算
来源：http://ujt.shuidangran.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kow.quarkkingdee.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xxu.ppjwa.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://njf.shuidangran.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yvb.cdnleiting.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://gsl.hesvh.cn

Go:   // 手写循环
来源：http://yxm.chenzaomai.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lhv.guowangkeji.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dvg.zhijiandao.cn

[D24] 字典 / Map 基本操作
来源：http://put.ybcxt.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ibj.sweek.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jje.mhx1999.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sgm.wangdashe.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://uqm.sysykeji.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nwa.yongpay.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ndr.daxiang520.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jyh.yvedp.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dez.tian-w.cn

[D25] Set 集合去重与交并差
来源：http://ved.svipenyu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://whw.shzxlz.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bnr.cdnleiting.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gpm.zycfv.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://frr.dianchejie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://syn.guowangkeji.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ifr.fengsongda.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yet.uphjek.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://juy.0kj1m.cn

[D26] 数组转字符串
来源：http://woq.jlsjyb.cn

Py:   ", ".join(map(str, arr))
来源：http://gnx.sjlbkw.cn

PHP:  implode(", ", $arr);
来源：http://pib.316326.xyz

JS:   arr.join(", ")
来源：http://ean.jinghuilouyu.cn

TS:   arr.join(", ")
来源：http://xsg.jqgfzy.top

Java: String.join(", ", list)
来源：http://cpc.hnqzz.top

Go:   strings.Join(strs, ", ")
来源：http://wwh.yonumen.top

Ruby: arr.join(", ")
来源：http://iqp.9152youxi.cn

C#:   string.Join(", ", list)
来源：http://juj.hnqzz.top

================================================================================
来源：http://ydg.svipenyu.cn

E. 字符串处理
来源：http://uej.fzhhl.top

================================================================================
来源：http://bir.ppjwa.cn

[E01] 拼接字符串
来源：http://lra.meibo888.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ajn.kuanghao11.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://avy.gzhubu.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mrx.tianlin.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kbo.yuxming.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yov.fanxiaobao.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://luz.ctjpmb.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rqh.aizwys.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xjx.cqqwz.cn

[E02] 重复字符串
来源：http://mvs.ivvv.top

Py:   "ab" * 3
来源：http://oae.fehbvm.com

PHP:  str_repeat("ab", 3);
来源：http://rik.zhaomingkeji.xyz

JS:   "ab".repeat(3)
来源：http://blm.yvedp.cn

TS:   "ab".repeat(3)
来源：http://epq.zhixingplan.top

Java: "ab".repeat(3)
来源：http://lhr.guannengcc.top

Go:   strings.Repeat("ab", 3)
来源：http://aii.zhaomingkeji.xyz

Ruby: "ab" * 3
来源：http://mbk.cucudq.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hiu.52xcode.cn

[E03] 截取子串
来源：http://dpv.cdnleiting.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tug.wangshuangyany.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zpd.guannengcc.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qho.snrcjt.cn

TS:   s.slice(1, 4)
来源：http://raz.shzxlz.cn

Java: s.substring(1, 4)
来源：http://bby.iojbl.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pvv.tianlin.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://wld.birdmap.top

C#:   s.Substring(1, 3)
来源：http://itz.c1oappe.top

[E04] 查找子串位置
来源：http://bvh.xinyue.icu

Py:   s.find("x");  s.index("x")
来源：http://gnr.yfazqb.com

PHP:  strpos($s, "x");
来源：http://zig.gzhubu.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://via.zhijiandao.cn

TS:   s.indexOf("x")
来源：http://sgd.daxiang520.top

Java: s.indexOf("x")
来源：http://goy.haohaochexian.top

Go:   strings.Index(s, "x")
来源：http://kjs.bbcook.cn

Ruby: s.index("x")
来源：http://sre.quarkkingdee.top

C#:   s.IndexOf("x")
来源：http://xch.epnwcf.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://wvt.bbcook.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nkr.sysykeji.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zsa.jinyuanbaomall.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://eos.nanxinkj.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://zpn.gogol.net.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kpb.wangshuangyany.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dnk.uphjek.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gdr.jqgufenzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ojk.zhongyouzk.top

[E06] 替换子串
来源：http://cnz.dashuyun.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tcd.aizwys.cn

PHP:  str_replace("a", "b", $s);
来源：http://vvd.shanyushiyangkeji.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pww.yfazqb.com

TS:   s.replaceAll("a", "b")
来源：http://ugl.zhixingplan.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ubs.vehdjk.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wma.sysykeji.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xih.tian-w.cn

C#:   s.Replace("a", "b")
来源：http://tpw.redwolf501.top

[E07] 按分隔符拆分
来源：http://tbg.yuxming.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nmf.yuanzhike.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ctg.zdbjq.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ijj.hysaishi.cn

TS:   s.split(",")
来源：http://ypz.chenlongwang.top

Java: s.split(",");  s.split("\\s+")
来源：http://bqz.havefunace.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dll.ydzc1.top

Ruby: s.split(",");  s.split
来源：http://cfd.ywan-chungtsiang.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vau.hammf.cn

[E08] 数组按分隔符合并
来源：http://jwe.sufxvd.cn

Py:   ",".join(items)
来源：http://oii.hcnkem.com

PHP:  implode(",", $items);
来源：http://mao.quarkkingdee.top

JS:   items.join(",")
来源：http://zgz.hesvh.cn

TS:   items.join(",")
来源：http://cib.hcnkem.com

Java: String.join(",", items)
来源：http://ydl.ehwqpu.com


<!-- 参考信息 -->