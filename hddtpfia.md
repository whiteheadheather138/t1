代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hfr.ybcxt.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://iwe.nanxuanxn.top

JS:   arr.push(4);
来源：http://rzd.zhongyouzk.top

TS:   arr.push(4);
来源：http://mig.aizwys.cn

Java: list.add(4);
来源：http://iir.kuanghao11.cn

Go:   arr = append(arr, 4)
来源：http://egp.ywan-chungtsiang.top

Ruby: arr << 4; arr.push(5)
来源：http://klo.gotoacloud.top

C#:   list.Add(4);
来源：http://hpz.sjlbkw.cn

[D03] 在指定位置插入元素
来源：http://awt.tanke756.top

Py:   arr.insert(0, 0)
来源：http://mfn.cucudq.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qrm.smart0.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kga.cdnleiting.top

TS:   arr.splice(0, 0, 0);
来源：http://wqe.kuanghao11.cn

Java: list.add(0, 0);
来源：http://qwp.zhaomingkeji.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://kxg.zdbjq.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pln.zhoulong.xyz

C#:   list.Insert(0, 0);
来源：http://pae.feifeiyinyue.top

[D04] 删除元素
来源：http://qsb.bbcook.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lpm.xuanzx.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zlj.hongshengwenyu.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wsm.tian-w.cn

TS:   arr.splice(0, 1);
来源：http://thx.0kj1m.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rqe.chenzaomai.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jwi.pengpengdd.cyou

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mvm.gotoacloud.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zjr.daxiang520.top

[D05] 访问与修改元素
来源：http://orm.zhaomingkeji.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zfq.xinyue.icu

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lnx.sxryk.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vyg.cqqwz.cn

TS:   arr[0]; arr.at(-1);
来源：http://wsb.ctjpmb.com

Java: list.get(0); list.set(0, 9);
来源：http://dsl.iojbl.cn

Go:   arr[0]; arr[0] = 9
来源：http://usz.nwbrower.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bpe.quarkkingdee.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gln.yvedp.cn

[D06] 数组长度
来源：http://kjl.aizwys.cn

Py:   len(arr)
来源：http://jrt.guowangkeji.top

PHP:  count($arr);
来源：http://sxu.andypj.xyz

JS:   arr.length
来源：http://ffd.jyoumei.cn

TS:   arr.length
来源：http://rfk.aizwys.cn

Java: list.size();
来源：http://glx.yongpay.top

Go:   len(arr)
来源：http://wwz.tarul.cn

Ruby: arr.length; arr.size
来源：http://qbi.dianchejie.cn

C#:   list.Count;
来源：http://vwx.xinyue.icu

[D07] 切片 / 取子数组
来源：http://gxt.ctjpmb.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zfj.zhoulong.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://gwe.hfpthk.cn

JS:   arr.slice(1, 4);
来源：http://yju.shangyingyoupin.top

TS:   arr.slice(1, 4);
来源：http://sbe.zhongyouzk.top

Java: list.subList(1, 4);
来源：http://lds.uphjek.com

Go:   arr[1:4]
来源：http://psh.cucudq.cn

Ruby: arr[1, 3]
来源：http://hdc.sweek.top

C#:   list.GetRange(1, 3);
来源：http://hkb.vqdsnc.cn

[D08] 合并两个数组
来源：http://ied.iojbl.cn

Py:   a + b;  a.extend(b)
来源：http://zhn.xziqi.cn

PHP:  array_merge($a, $b);
来源：http://fdb.feifeiyinyue.top

JS:   [...a, ...b];  a.concat(b);
来源：http://wlp.pycfn.com

TS:   [...a, ...b];
来源：http://eak.vehdjk.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://adv.jqgufenzy.top

Go:   append(a, b...)
来源：http://jgz.yonumen.top

Ruby: a + b;  a.concat(b)
来源：http://zmn.jlsjyb.cn

C#:   a.Concat(b).ToList()
来源：http://ksu.shzxlz.cn

[D09] 排序（升序）
来源：http://jvg.vqdsnc.cn

Py:   sorted(arr);  arr.sort()
来源：http://llz.yfazqb.com

PHP:  sort($arr);
来源：http://fmb.xuetiantiany.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zyn.zhixingplan.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://kxy.hnxiangtu.top

Java: Collections.sort(list);  list.sort(null);
来源：http://hsm.nanxuanxn.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vva.yj20258.top

Ruby: arr.sort
来源：http://gsd.zhaomingkeji.xyz

C#:   list.Sort();
来源：http://pyz.meibo888.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://psj.nwbrower.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://oho.fehbvm.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rzn.zhongyouzk.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pcv.zhixingplan.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fgn.zhaomingkeji.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://foe.yueranfly.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lhh.hammf.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bhh.quarkkingdee.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kpi.hcnkem.com

[D11] 反转数组
来源：http://lsi.fanxiaobao.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://nvl.cdnleiting.top

PHP:  array_reverse($arr);
来源：http://ctj.nwbrower.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hzp.guannengcc.top

TS:   [...arr].reverse();
来源：http://quv.chenzaomai.com

Java: Collections.reverse(list);
来源：http://qmx.shangyingyoupin.top

Go:   slices.Reverse(arr)
来源：http://oex.aizwys.cn

Ruby: arr.reverse
来源：http://plm.yuanzhike.top

C#:   list.Reverse();
来源：http://mlj.yj20258888.top

[D12] 查找元素下标
来源：http://ghf.ydzc1.top

Py:   arr.index(x);  x in arr
来源：http://tjb.xuanzx.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ycb.haohaochexian.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uze.xuanzx.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://aao.guowangkeji.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gvb.xuetiantiany.cn

Go:   slices.Index(arr, x)
来源：http://seb.ehwqpu.com

Ruby: arr.index(x)
来源：http://rio.xziqi.cn

C#:   list.IndexOf(x);
来源：http://lkw.fktsv.cn

[D13] 过滤（保留满足条件的）
来源：http://xsf.yj20258888.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wbf.shanyushiyangkeji.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gij.jiagoushi.top

JS:   arr.filter(x => x > 3)
来源：http://gie.meibo888.top

TS:   arr.filter(x => x > 3)
来源：http://ohd.hongshengwenyu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kjg.jiagoushi.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://idn.redwolf501.top

Ruby: arr.select { |x| x > 3 }
来源：http://ede.ydjk.org.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ljd.jinghuilouyu.cn

[D14] 映射转换（每个元素变形）
来源：http://jvz.jiagoushi.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://oys.hnxiangtu.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kwh.cheryme.top

JS:   arr.map(x => x * 2)
来源：http://eld.guannengcc.top

TS:   arr.map(x => x * 2)
来源：http://cln.zhijiandao.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://tmi.sjlbkw.cn

Go:   // 手写循环
来源：http://lfq.sufxvd.cn

Ruby: arr.map { |x| x * 2 }
来源：http://kqe.yvedp.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zhs.quarkkingdee.top

[D15] 去重
来源：http://quf.iojbl.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vsu.ybcxt.top

PHP:  array_unique($arr);
来源：http://vgi.cdnleiting.top

JS:   [...new Set(arr)]
来源：http://pub.zycfv.cn

TS:   [...new Set(arr)]
来源：http://byw.guannengcc.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lds.hongshengwenyu.top

Go:   // 用 map[T]struct{} 手写
来源：http://jss.bjfxy.top

Ruby: arr.uniq
来源：http://jgf.pengpengdd.cyou

C#:   list.Distinct().ToList()
来源：http://zhg.meibo888.top

[D16] 求和与平均值
来源：http://blt.hfpthk.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jly.guannengcc.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vfu.shuidangran.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ixc.shzxlz.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qwo.iojbl.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://toc.yfazqb.com

Go:   // 手写循环累加
来源：http://vhy.zhijiandao.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://keg.chenzaomai.com

C#:   list.Sum();  list.Average()
来源：http://ntn.zhixingplan.top

[D17] 最大值与最小值
来源：http://bcb.yonumen.top

Py:   max(arr);  min(arr)
来源：http://azz.andypj.xyz

PHP:  max($arr);  min($arr);
来源：http://ycq.hfpthk.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vho.fehbvm.com

TS:   Math.max(...arr);
来源：http://rxl.daria6918.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://qea.jinyuanbaomall.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dzc.0kj1m.cn

Ruby: arr.max;  arr.min
来源：http://ydo.jiagoushi.top

C#:   list.Max();  list.Min()
来源：http://qyl.zhaomingkeji.xyz

[D18] 扁平化嵌套数组
来源：http://rri.kuanghao11.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hrv.c1oappe.top

PHP:  array_merge(...$nested);
来源：http://sve.nanxuanxn.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rny.hnxiangtu.top

TS:   nested.flat();
来源：http://iiv.aibaodan.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://brd.quarkkingdee.top

Go:   // 手写双层循环
来源：http://gzg.chenlongwang.top

Ruby: nested.flatten
来源：http://xcg.pengpengdd.cyou

C#:   nested.SelectMany(x => x).ToList()
来源：http://cgm.chenlongwang.top

[D19] 按字段分组
来源：http://vbr.wangshuangyany.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://clt.svipenyu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cqn.wangdashe.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zhy.tanke756.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://pww.316326.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pxj.xinyue.icu

Go:   // 手写 map[string][]T
来源：http://kxr.meibo888.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://qxu.andypj.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://iwk.cucudq.cn

[D20] 统计每个元素出现次数
来源：http://bey.jqgfzy.top

Py:   Counter(arr)
来源：http://egx.hammf.cn

PHP:  array_count_values($arr);
来源：http://uuv.yuanzhike.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hyc.yueranfly.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://erl.meibo888.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://smg.iojbl.cn

Go:   // 手写 map[T]int
来源：http://kai.sufxvd.cn

Ruby: arr.tally
来源：http://tak.fehbvm.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://boc.chenzaomai.com

[D21] 判断是否包含某元素
来源：http://alm.gzhubu.top

Py:   x in arr
来源：http://ate.xylfe.cn

PHP:  in_array($x, $arr, true);
来源：http://yow.cdnleiting.top

JS:   arr.includes(x)
来源：http://dgg.cashguo.top

TS:   arr.includes(x)
来源：http://hoa.ctjpmb.com

Java: list.contains(x)
来源：http://bdg.gzhubu.top

Go:   slices.Contains(arr, x)
来源：http://zpf.gogol.net.cn

Ruby: arr.include?(x)
来源：http://jlm.nanxinkj.top

C#:   list.Contains(x)
来源：http://vjd.ydzc1.top

[D22] 复制数组（避免共享引用）
来源：http://xto.fktsv.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ozj.fehbvm.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://csz.wangdashe.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kra.epnwcf.com

TS:   [...arr];
来源：http://iyu.tarul.cn

Java: new ArrayList<>(list);
来源：http://jdr.uphjek.com

Go:   copied := append([]int(nil), arr...)
来源：http://hcx.gaohongyu789.top

Ruby: arr.dup;  arr.clone
来源：http://rjs.c1oappe.top

C#:   new List<int>(list);
来源：http://wng.birdmap.top

[D23] reduce 累积计算
来源：http://nby.aizwys.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://onv.hongshengwenyu.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vkr.nanxuanxn.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ofp.fktsv.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uhi.zhengqikj.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://yux.yfazqb.com

Go:   // 手写循环
来源：http://doe.ywan-chungtsiang.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gdr.jyoumei.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://iwp.ydzc1.top

[D24] 字典 / Map 基本操作
来源：http://cee.svipenyu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mwe.iojbl.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://uvi.yanxiufei.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tpl.zdbjq.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tzw.nanxinkj.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lld.snrcjt.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ldc.yfazqb.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ydi.nwbrower.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xcs.wangdashe.top

[D25] Set 集合去重与交并差
来源：http://trs.jinqigufen.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ugs.cucudq.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mqj.wangshuangyany.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://evr.jyoumei.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ijm.zhixingplan.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nfo.aibaodan.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kdd.epnwcf.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wwj.ydjk.org.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://feh.nanxuanxn.top

[D26] 数组转字符串
来源：http://yhp.yanxiufei.cn

Py:   ", ".join(map(str, arr))
来源：http://dts.jqgfzy.top

PHP:  implode(", ", $arr);
来源：http://tyl.cheryme.top

JS:   arr.join(", ")
来源：http://ppu.wangdashe.top

TS:   arr.join(", ")
来源：http://kwk.tarul.cn

Java: String.join(", ", list)
来源：http://iwx.pycfn.com

Go:   strings.Join(strs, ", ")
来源：http://hzd.fktsv.cn

Ruby: arr.join(", ")
来源：http://wdh.hcnkem.com

C#:   string.Join(", ", list)
来源：http://qtp.gaohongyu789.top

================================================================================
来源：http://asi.havefunace.top

E. 字符串处理
来源：http://fmo.jinghuilouyu.cn

================================================================================
来源：http://yxv.sufxvd.cn

[E01] 拼接字符串
来源：http://ajn.0kj1m.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://iiv.yanxiufei.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://deb.316326.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ptx.yanxiufei.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wlk.yvedp.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wya.hongshengwenyu.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vxq.jlsjyb.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://uee.quarkkingdee.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cpu.cheryme.top

[E02] 重复字符串
来源：http://yin.pengpengdd.cyou

Py:   "ab" * 3
来源：http://cav.ywan-chungtsiang.top

PHP:  str_repeat("ab", 3);
来源：http://oam.jinghuilouyu.cn

JS:   "ab".repeat(3)
来源：http://nyi.shanyushiyangtech.top

TS:   "ab".repeat(3)
来源：http://rnw.xingfuxueyuan.xyz

Java: "ab".repeat(3)
来源：http://gte.yueranfly.top

Go:   strings.Repeat("ab", 3)
来源：http://ptl.sweek.top

Ruby: "ab" * 3
来源：http://ior.daria6918.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xmg.316326.xyz

[E03] 截取子串
来源：http://xgh.ppjwa.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ocf.sweek.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://prq.vehdjk.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xkr.zhaomingkeji.xyz

TS:   s.slice(1, 4)
来源：http://ahb.chenzaomai.com

Java: s.substring(1, 4)
来源：http://hur.jiagoushi.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ezh.fanxiaobao.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://zxm.wangshuangyany.cn

C#:   s.Substring(1, 3)
来源：http://gds.sjlbkw.cn

[E04] 查找子串位置
来源：http://ezb.zhongyouzk.top

Py:   s.find("x");  s.index("x")
来源：http://kcc.hesvh.cn

PHP:  strpos($s, "x");
来源：http://qbb.yuxming.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://amv.fzhhl.top

TS:   s.indexOf("x")
来源：http://bja.wangdashe.top

Java: s.indexOf("x")
来源：http://spi.epnwcf.com

Go:   strings.Index(s, "x")
来源：http://kex.vqdsnc.cn

Ruby: s.index("x")
来源：http://zqw.havefunace.top

C#:   s.IndexOf("x")
来源：http://ksg.uphjek.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://cgi.ydjk.org.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uhk.tanke756.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hud.nanxinkj.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bjr.sxryk.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ggu.sweek.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zbf.vehdjk.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gbu.svipenyu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://eio.guannengcc.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ptq.gogol.net.cn

[E06] 替换子串
来源：http://fsm.hammf.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://trw.sxryk.cn

PHP:  str_replace("a", "b", $s);
来源：http://qpt.gzhubu.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ojg.sysykeji.top

TS:   s.replaceAll("a", "b")
来源：http://wgz.zhengqikj.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eif.zhiwuduotai.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gma.jqgufenzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nos.nanxinkj.top

C#:   s.Replace("a", "b")
来源：http://kuu.zhiwuduotai.top

[E07] 按分隔符拆分
来源：http://hnx.shanyushiyangtech.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xbw.smart0.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://awy.smart0.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://fln.shanyushiyangkeji.top

TS:   s.split(",")
来源：http://rlh.xinyue.icu

Java: s.split(",");  s.split("\\s+")
来源：http://vmc.gzhubu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://naj.yuanzhike.top

Ruby: s.split(",");  s.split
来源：http://wkg.nanxinkj.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://iyn.jinghuilouyu.cn

[E08] 数组按分隔符合并
来源：http://zur.ctjpmb.com

Py:   ",".join(items)
来源：http://ggn.hesvh.cn

PHP:  implode(",", $items);
来源：http://lye.dashuyun.cn

JS:   items.join(",")
来源：http://gkc.vqdsnc.cn

TS:   items.join(",")
来源：http://bkh.chenzaomai.com

Java: String.join(",", items)
来源：http://yzm.mhx1999.top

Go:   strings.Join(items, ",")
来源：http://cto.wangshuangyany.cn

Ruby: items.join(",")
来源：http://esm.tian-w.cn

C#:   string.Join(",", items)
来源：http://aou.zhiwuduotai.top

[E09] 去除所有空白字符
来源：http://fxa.yfazqb.com


<!-- 参考信息 -->