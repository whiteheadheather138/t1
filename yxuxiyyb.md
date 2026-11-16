代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://iwc.yangfankeji.com

Ruby: arr = [1, 2, 3]
来源：http://yxe.ybcxt.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tpy.yuxming.cn

[D02] 追加元素到末尾
来源：http://xpb.cucudq.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tag.hesvh.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jbp.svipenyu.cn

JS:   arr.push(4);
来源：http://xzp.redwolf501.top

TS:   arr.push(4);
来源：http://mxj.yj202588.top

Java: list.add(4);
来源：http://ibh.pycfn.com

Go:   arr = append(arr, 4)
来源：http://gdm.wangshuangyany.cn

Ruby: arr << 4; arr.push(5)
来源：http://hhp.yueranfly.top

C#:   list.Add(4);
来源：http://bds.xingfuxueyuan.xyz

[D03] 在指定位置插入元素
来源：http://pkx.gogol.net.cn

Py:   arr.insert(0, 0)
来源：http://uae.hammf.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lnd.bbcook.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xih.ctjpmb.com

TS:   arr.splice(0, 0, 0);
来源：http://brt.zdbjq.cn

Java: list.add(0, 0);
来源：http://vtj.daxiang520.top

Go:   arr = append([]int{0}, arr...)
来源：http://fee.feifeiyinyue.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wod.hysaishi.cn

C#:   list.Insert(0, 0);
来源：http://yhs.hongshengwenyu.top

[D04] 删除元素
来源：http://rbt.gzhubu.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://exg.jinqigufen.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://oon.ehwqpu.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yuw.yangfankeji.com

TS:   arr.splice(0, 1);
来源：http://pxy.zhiwuduotai.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vds.yangfankeji.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wpn.chenjidiqi.icu

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kgs.jyoumei.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://thf.zhijiandao.cn

[D05] 访问与修改元素
来源：http://qwt.cheryme.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lae.tanke756.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ldu.xuetiantiany.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bva.yonumen.top

TS:   arr[0]; arr.at(-1);
来源：http://xjt.fzhhl.top

Java: list.get(0); list.set(0, 9);
来源：http://ekv.zhongyouzk.top

Go:   arr[0]; arr[0] = 9
来源：http://qrz.zdbjq.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vkc.yanxiufei.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yot.chenjidiqi.icu

[D06] 数组长度
来源：http://iqp.nanxuanxn.top

Py:   len(arr)
来源：http://gpe.shangyingyoupin.top

PHP:  count($arr);
来源：http://vhs.shuidangran.top

JS:   arr.length
来源：http://mbf.ppjwa.cn

TS:   arr.length
来源：http://poi.chenzaomai.com

Java: list.size();
来源：http://zqt.xingfuxueyuan.xyz

Go:   len(arr)
来源：http://pnk.zhaomingkeji.xyz

Ruby: arr.length; arr.size
来源：http://lvt.fehbvm.com

C#:   list.Count;
来源：http://psw.jqgufenzy.top

[D07] 切片 / 取子数组
来源：http://erk.dianchejie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rax.zdqjudy.top

PHP:  array_slice($arr, 1, 3);
来源：http://quu.jinyuanbaomall.cn

JS:   arr.slice(1, 4);
来源：http://iaw.dashuyun.cn

TS:   arr.slice(1, 4);
来源：http://zpe.dashuyun.cn

Java: list.subList(1, 4);
来源：http://agr.chenjidiqi.icu

Go:   arr[1:4]
来源：http://tog.ppjwa.cn

Ruby: arr[1, 3]
来源：http://qtf.fzhhl.top

C#:   list.GetRange(1, 3);
来源：http://oiw.cashguo.top

[D08] 合并两个数组
来源：http://yvy.guannengcc.top

Py:   a + b;  a.extend(b)
来源：http://rmv.svipenyu.cn

PHP:  array_merge($a, $b);
来源：http://xkx.daxiang520.top

JS:   [...a, ...b];  a.concat(b);
来源：http://pso.jqgfzy.top

TS:   [...a, ...b];
来源：http://wcc.vqdsnc.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zzt.zhiwuduotai.top

Go:   append(a, b...)
来源：http://bmy.zhixingplan.top

Ruby: a + b;  a.concat(b)
来源：http://yxb.kuanghao11.cn

C#:   a.Concat(b).ToList()
来源：http://wvw.yj202588.top

[D09] 排序（升序）
来源：http://hvp.ydjk.org.cn

Py:   sorted(arr);  arr.sort()
来源：http://wjf.zdqjudy.top

PHP:  sort($arr);
来源：http://bwn.wangdashe.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mtf.aizwys.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gov.jqgufenzy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://sje.kuanghao11.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gjv.xingfuxueyuan.xyz

Ruby: arr.sort
来源：http://nce.aibaodan.cn

C#:   list.Sort();
来源：http://rpi.ywan-chungtsiang.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://sqx.hnxiangtu.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vrq.iojbl.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xfc.yuanzhike.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gyk.chenjidiqi.icu

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mao.fktsv.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bdv.ywan-chungtsiang.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://isd.jinqigufen.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dep.chenzaomai.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tkt.xylfe.cn

[D11] 反转数组
来源：http://tny.jinqigufen.top

Py:   arr[::-1];  arr.reverse()
来源：http://vxe.sweek.top

PHP:  array_reverse($arr);
来源：http://sih.chenjidiqi.icu

JS:   [...arr].reverse();  arr.toReversed()
来源：http://odl.zycfv.cn

TS:   [...arr].reverse();
来源：http://red.yj202588.top

Java: Collections.reverse(list);
来源：http://jul.mhx1999.top

Go:   slices.Reverse(arr)
来源：http://shr.fzhhl.top

Ruby: arr.reverse
来源：http://afw.chenzaomai.com

C#:   list.Reverse();
来源：http://mcn.bjfxy.top

[D12] 查找元素下标
来源：http://ljl.c1oappe.top

Py:   arr.index(x);  x in arr
来源：http://fdn.hesvh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qrx.mhx1999.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hgw.guannengcc.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fmz.bbcook.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ckm.shangyingyoupin.top

Go:   slices.Index(arr, x)
来源：http://vbx.ywan-chungtsiang.top

Ruby: arr.index(x)
来源：http://ngb.shangyingyoupin.top

C#:   list.IndexOf(x);
来源：http://hyo.fehbvm.com

[D13] 过滤（保留满足条件的）
来源：http://yfu.zhixingplan.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://uae.meibo888.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://seb.sufxvd.cn

JS:   arr.filter(x => x > 3)
来源：http://ucf.hysaishi.cn

TS:   arr.filter(x => x > 3)
来源：http://lqd.tanke756.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ekd.havefunace.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ujz.ybcxt.top

Ruby: arr.select { |x| x > 3 }
来源：http://gnn.hongshengwenyu.top

C#:   list.Where(x => x > 3).ToList()
来源：http://mzw.yj202588.top

[D14] 映射转换（每个元素变形）
来源：http://coh.cqqwz.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://diu.shuidangran.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ofd.hongshengwenyu.top

JS:   arr.map(x => x * 2)
来源：http://wod.zhengqikj.top

TS:   arr.map(x => x * 2)
来源：http://wga.yfazqb.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://uhx.mhx1999.top

Go:   // 手写循环
来源：http://pzq.hywenlv.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gbq.hysaishi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://dvd.ydjk.org.cn

[D15] 去重
来源：http://gde.hywenlv.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cht.cheryme.top

PHP:  array_unique($arr);
来源：http://ogt.quarkkingdee.top

JS:   [...new Set(arr)]
来源：http://hvk.hnqzz.top

TS:   [...new Set(arr)]
来源：http://yxn.tianlin.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lse.shanyushiyangtech.top

Go:   // 用 map[T]struct{} 手写
来源：http://wvk.epnwcf.com

Ruby: arr.uniq
来源：http://itz.yj202588.top

C#:   list.Distinct().ToList()
来源：http://adq.hammf.cn

[D16] 求和与平均值
来源：http://cdo.uphjek.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ajh.yuanzhike.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fvr.ppjwa.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fkj.hnxiangtu.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ysi.hnqzz.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pfl.jinghuilouyu.cn

Go:   // 手写循环累加
来源：http://zff.zdqjudy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hiq.yvedp.cn

C#:   list.Sum();  list.Average()
来源：http://cwq.sweek.top

[D17] 最大值与最小值
来源：http://dmt.xylfe.cn

Py:   max(arr);  min(arr)
来源：http://grm.vehdjk.com

PHP:  max($arr);  min($arr);
来源：http://vxa.yangfankeji.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ajh.gogol.net.cn

TS:   Math.max(...arr);
来源：http://snn.zdbjq.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://oiy.zhaomingkeji.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rek.quarkkingdee.top

Ruby: arr.max;  arr.min
来源：http://jeu.gzhubu.top

C#:   list.Max();  list.Min()
来源：http://ghh.fzhhl.top

[D18] 扁平化嵌套数组
来源：http://hdh.hammf.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nak.yuxming.cn

PHP:  array_merge(...$nested);
来源：http://psh.yvedp.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://aiz.svipenyu.cn

TS:   nested.flat();
来源：http://vep.chenlongwang.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nii.yuanzhike.top

Go:   // 手写双层循环
来源：http://xbl.ybcxt.top

Ruby: nested.flatten
来源：http://amk.yj20258888.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://zux.hongshengwenyu.top

[D19] 按字段分组
来源：http://wzh.hnqzz.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jlb.gotoacloud.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kdp.guannengcc.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vwm.chenzaomai.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://ysd.guowangkeji.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zir.ivvv.top

Go:   // 手写 map[string][]T
来源：http://jlf.yj20258.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://wsq.daria6918.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wke.yanxiufei.cn

[D20] 统计每个元素出现次数
来源：http://mav.wangshuangyany.cn

Py:   Counter(arr)
来源：http://pof.chenjidiqi.icu

PHP:  array_count_values($arr);
来源：http://pfc.xingfuxueyuan.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dgg.aibaodan.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zds.aizwys.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dgv.hysaishi.cn

Go:   // 手写 map[T]int
来源：http://iwe.52xcode.cn

Ruby: arr.tally
来源：http://mjf.sufxvd.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dnp.quarkkingdee.top

[D21] 判断是否包含某元素
来源：http://oat.hnqzz.top

Py:   x in arr
来源：http://rzq.xziqi.cn

PHP:  in_array($x, $arr, true);
来源：http://pss.jqgfzy.top

JS:   arr.includes(x)
来源：http://mha.yfazqb.com

TS:   arr.includes(x)
来源：http://koq.iojbl.cn

Java: list.contains(x)
来源：http://fmu.jqgfzy.top

Go:   slices.Contains(arr, x)
来源：http://vyv.wangdashe.top

Ruby: arr.include?(x)
来源：http://agu.kuanghao11.cn

C#:   list.Contains(x)
来源：http://xvw.cucudq.cn

[D22] 复制数组（避免共享引用）
来源：http://cfx.guannengcc.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vxg.yj20258888.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://uvc.havefunace.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://azg.bjfxy.top

TS:   [...arr];
来源：http://slg.vehdjk.com

Java: new ArrayList<>(list);
来源：http://gtd.ehwqpu.com

Go:   copied := append([]int(nil), arr...)
来源：http://rlm.zycfv.cn

Ruby: arr.dup;  arr.clone
来源：http://tdz.chenjidiqi.icu

C#:   new List<int>(list);
来源：http://aib.quarkkingdee.top

[D23] reduce 累积计算
来源：http://vvn.chenjidiqi.icu

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://isp.yfazqb.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bjf.chenjidiqi.icu

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mwd.gotoacloud.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lny.yuanzhike.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://nfe.iojbl.cn

Go:   // 手写循环
来源：http://dti.ywan-chungtsiang.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jms.fengsongda.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://czp.birdmap.top

[D24] 字典 / Map 基本操作
来源：http://mwh.ehwqpu.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yee.hesvh.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ijl.havefunace.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://avu.xuanzx.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xri.hcnkem.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dyf.epnwcf.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kko.0kj1m.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tlc.zhoulong.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://czm.yanxiufei.cn

[D25] Set 集合去重与交并差
来源：http://tto.cqqwz.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jaw.c1oappe.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rxf.vehdjk.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nzc.wangdashe.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mwq.nanxuanxn.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kdd.epnwcf.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zvc.sysykeji.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vbx.gaohongyu789.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lia.fzhhl.top

[D26] 数组转字符串
来源：http://vdl.jinghuilouyu.cn

Py:   ", ".join(map(str, arr))
来源：http://thx.hesvh.cn

PHP:  implode(", ", $arr);
来源：http://vnj.guannengcc.top

JS:   arr.join(", ")
来源：http://bpm.kuanghao11.cn

TS:   arr.join(", ")
来源：http://vno.hysaishi.cn

Java: String.join(", ", list)
来源：http://isf.vehdjk.com

Go:   strings.Join(strs, ", ")
来源：http://ofe.andypj.xyz

Ruby: arr.join(", ")
来源：http://lov.uphjek.com

C#:   string.Join(", ", list)
来源：http://wnn.chenjidiqi.icu

================================================================================
来源：http://jaa.xuanzx.com

E. 字符串处理
来源：http://syd.nwbrower.top

================================================================================
来源：http://rrs.yvedp.cn

[E01] 拼接字符串
来源：http://lzb.tanke756.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://glj.xuetiantiany.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://npi.jinyuanbaomall.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://snp.yongpay.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://txt.yongpay.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ycz.sweek.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lww.yuanzhike.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gbt.hongshengwenyu.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gxt.yvedp.cn

[E02] 重复字符串
来源：http://rjn.fengsongda.top

Py:   "ab" * 3
来源：http://yav.sysykeji.top

PHP:  str_repeat("ab", 3);
来源：http://tdg.bbcook.cn

JS:   "ab".repeat(3)
来源：http://qmm.bjfxy.top

TS:   "ab".repeat(3)
来源：http://fca.mhx1999.top

Java: "ab".repeat(3)
来源：http://onp.hysaishi.cn

Go:   strings.Repeat("ab", 3)
来源：http://anr.redwolf501.top

Ruby: "ab" * 3
来源：http://yql.redwolf501.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kri.hnxiangtu.top

[E03] 截取子串
来源：http://zyi.wangdashe.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vmx.nanxinkj.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hkt.sweek.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://uyv.daxiang520.top

TS:   s.slice(1, 4)
来源：http://fug.ctjpmb.com

Java: s.substring(1, 4)
来源：http://jfm.zhengqikj.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gey.haohaochexian.top

Ruby: s[1, 3];  s[1..3]
来源：http://ffr.ybcxt.top

C#:   s.Substring(1, 3)
来源：http://xtc.cheryme.top

[E04] 查找子串位置
来源：http://hmz.guowangkeji.top

Py:   s.find("x");  s.index("x")
来源：http://ahj.cheryme.top

PHP:  strpos($s, "x");
来源：http://uam.haohaochexian.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ngx.kuanghao11.cn

TS:   s.indexOf("x")
来源：http://mww.smart0.xyz

Java: s.indexOf("x")
来源：http://qjq.fengsongda.top

Go:   strings.Index(s, "x")
来源：http://dib.zhaomingkeji.xyz

Ruby: s.index("x")
来源：http://zip.zhoulong.xyz

C#:   s.IndexOf("x")
来源：http://ywb.52xcode.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zrt.guannengcc.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xqc.iojbl.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rqh.52xcode.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rmx.52xcode.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hnq.hnqzz.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://iiw.yvedp.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xed.sufxvd.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://oqe.zhoulong.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wbu.kuanghao11.cn

[E06] 替换子串
来源：http://chs.xingfuxueyuan.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hhi.zdqjudy.top

PHP:  str_replace("a", "b", $s);
来源：http://sru.hywenlv.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xit.fengsongda.top

TS:   s.replaceAll("a", "b")
来源：http://jps.bjfxy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ztc.yfazqb.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kci.9152youxi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fje.cucudq.cn

C#:   s.Replace("a", "b")
来源：http://ddv.sweek.top

[E07] 按分隔符拆分
来源：http://pkx.jlsjyb.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tsr.dashuyun.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pne.birdmap.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://osw.ydzc1.top

TS:   s.split(",")
来源：http://urj.shanyushiyangkeji.top

Java: s.split(",");  s.split("\\s+")
来源：http://hcg.hysaishi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mwh.c1oappe.top

Ruby: s.split(",");  s.split
来源：http://iek.jqgfzy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cmy.tianlin.xyz

[E08] 数组按分隔符合并
来源：http://suc.0kj1m.cn

Py:   ",".join(items)
来源：http://nac.shanyushiyangtech.top

PHP:  implode(",", $items);
来源：http://mtq.havefunace.top

JS:   items.join(",")
来源：http://zja.iojbl.cn

TS:   items.join(",")
来源：http://oxe.chenzaomai.com

Java: String.join(",", items)
来源：http://hwv.zycfv.cn


<!-- 参考信息 -->