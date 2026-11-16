代发 wailian999

D. 数组 / 列表 / 集合
来源：http://hmn.kuanghao11.cn

================================================================================
来源：http://oye.sufxvd.cn

[D01] 创建数组 / 列表
来源：http://ktv.shzxlz.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jcc.jyoumei.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zce.sjlbkw.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mkk.gzhubu.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://jim.jinqigfzy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qgv.aibaodan.cn

Go:   arr := []int{1, 2, 3}
来源：http://gxq.nanxuanxn.top

Ruby: arr = [1, 2, 3]
来源：http://xeb.andypj.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hau.wangshuangyany.cn

[D02] 追加元素到末尾
来源：http://zhs.fengsongda.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xib.zhoulong.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hcn.ydzc1.top

JS:   arr.push(4);
来源：http://uxm.hammf.cn

TS:   arr.push(4);
来源：http://dxz.sxryk.cn

Java: list.add(4);
来源：http://kca.aizwys.cn

Go:   arr = append(arr, 4)
来源：http://ieo.chenlongwang.top

Ruby: arr << 4; arr.push(5)
来源：http://cxc.ydjk.org.cn

C#:   list.Add(4);
来源：http://ivq.epnwcf.com

[D03] 在指定位置插入元素
来源：http://vng.ybcxt.top

Py:   arr.insert(0, 0)
来源：http://owk.xylfe.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zty.cheryme.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cma.jinyuanbaomall.cn

TS:   arr.splice(0, 0, 0);
来源：http://bxc.jiagoushi.top

Java: list.add(0, 0);
来源：http://rud.ctjpmb.com

Go:   arr = append([]int{0}, arr...)
来源：http://bdf.c1oappe.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zdf.zhiwuduotai.top

C#:   list.Insert(0, 0);
来源：http://hmw.gzhubu.top

[D04] 删除元素
来源：http://kzd.pengpengdd.cyou

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bmt.jinghuilouyu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pvv.jyoumei.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xln.fengsongda.top

TS:   arr.splice(0, 1);
来源：http://txg.yangfankeji.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nqx.wangshuangyany.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qnh.hcnkem.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://oxr.hammf.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fao.aizwys.cn

[D05] 访问与修改元素
来源：http://vim.gaohongyu789.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lzz.fanxiaobao.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tei.feifeiyinyue.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jcc.vehdjk.com

TS:   arr[0]; arr.at(-1);
来源：http://yto.pycfn.com

Java: list.get(0); list.set(0, 9);
来源：http://exx.vqdsnc.cn

Go:   arr[0]; arr[0] = 9
来源：http://aeg.wangdashe.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://peq.ehwqpu.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fji.xuetiantiany.cn

[D06] 数组长度
来源：http://hkl.wangshuangyany.cn

Py:   len(arr)
来源：http://oko.hywenlv.cn

PHP:  count($arr);
来源：http://dlg.nwbrower.top

JS:   arr.length
来源：http://fsu.zycfv.cn

TS:   arr.length
来源：http://ljz.quarkkingdee.top

Java: list.size();
来源：http://gcg.jyoumei.cn

Go:   len(arr)
来源：http://etz.xinyue.icu

Ruby: arr.length; arr.size
来源：http://cdd.smart0.xyz

C#:   list.Count;
来源：http://uup.haohaochexian.top

[D07] 切片 / 取子数组
来源：http://uyx.yfazqb.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fnm.smart0.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://yio.pengpengdd.cyou

JS:   arr.slice(1, 4);
来源：http://gvl.zhixingplan.top

TS:   arr.slice(1, 4);
来源：http://cxo.jianghu66.top

Java: list.subList(1, 4);
来源：http://zqp.hnxiangtu.top

Go:   arr[1:4]
来源：http://smr.zhijiandao.cn

Ruby: arr[1, 3]
来源：http://skg.tarul.cn

C#:   list.GetRange(1, 3);
来源：http://ves.hnxiangtu.top

[D08] 合并两个数组
来源：http://amf.pycfn.com

Py:   a + b;  a.extend(b)
来源：http://jqh.zycfv.cn

PHP:  array_merge($a, $b);
来源：http://dto.gotoacloud.top

JS:   [...a, ...b];  a.concat(b);
来源：http://prb.tian-w.cn

TS:   [...a, ...b];
来源：http://mvn.dashuyun.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wlj.fehbvm.com

Go:   append(a, b...)
来源：http://opw.zycfv.cn

Ruby: a + b;  a.concat(b)
来源：http://qve.zhongyouzk.top

C#:   a.Concat(b).ToList()
来源：http://fxk.haohaochexian.top

[D09] 排序（升序）
来源：http://nhs.xingfuxueyuan.xyz

Py:   sorted(arr);  arr.sort()
来源：http://pen.vqdsnc.cn

PHP:  sort($arr);
来源：http://qgi.ydzc1.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wma.yj20258888.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://yjl.smart0.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://zrd.yanxiufei.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://noa.ydzc1.top

Ruby: arr.sort
来源：http://mhp.nanxuanxn.top

C#:   list.Sort();
来源：http://ybt.yj20258888.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://qyx.zhaomingkeji.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kjk.guannengcc.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://alq.shuidangran.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://via.jinyuanbaomall.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mxg.c1oappe.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nqo.cashguo.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wgv.jinghuilouyu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fhg.tianlin.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pst.pycfn.com

[D11] 反转数组
来源：http://ufb.quarkkingdee.top

Py:   arr[::-1];  arr.reverse()
来源：http://epz.jinqigfzy.top

PHP:  array_reverse($arr);
来源：http://jzc.zhongyouzk.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://slu.hfpthk.cn

TS:   [...arr].reverse();
来源：http://gin.chenzaomai.com

Java: Collections.reverse(list);
来源：http://zaz.yongpay.top

Go:   slices.Reverse(arr)
来源：http://dbg.hysaishi.cn

Ruby: arr.reverse
来源：http://vir.fengsongda.top

C#:   list.Reverse();
来源：http://clq.hywenlv.cn

[D12] 查找元素下标
来源：http://kdk.hesvh.cn

Py:   arr.index(x);  x in arr
来源：http://asg.hnqzz.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mkd.ywan-chungtsiang.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kzf.zhoulong.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rwc.xuanzx.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nmi.zdqjudy.top

Go:   slices.Index(arr, x)
来源：http://eoo.meibo888.top

Ruby: arr.index(x)
来源：http://kpy.ppjwa.cn

C#:   list.IndexOf(x);
来源：http://ynu.cheryme.top

[D13] 过滤（保留满足条件的）
来源：http://otj.nanxinkj.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bap.wangshuangyany.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xsw.vqdsnc.cn

JS:   arr.filter(x => x > 3)
来源：http://kqc.fanxiaobao.xyz

TS:   arr.filter(x => x > 3)
来源：http://itg.cucudq.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ksm.kuanghao11.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hts.xuanzx.com

Ruby: arr.select { |x| x > 3 }
来源：http://nmw.zhijiandao.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://klc.cheryme.top

[D14] 映射转换（每个元素变形）
来源：http://ekj.nanxinkj.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sht.xinyue.icu

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://aqn.yuanzhike.top

JS:   arr.map(x => x * 2)
来源：http://eic.guannengcc.top

TS:   arr.map(x => x * 2)
来源：http://wev.cucudq.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://eto.cheryme.top

Go:   // 手写循环
来源：http://mhx.gogol.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://irn.quarkkingdee.top

C#:   list.Select(x => x * 2).ToList()
来源：http://vbc.ehwqpu.com

[D15] 去重
来源：http://rfn.hnqzz.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qcf.hesvh.cn

PHP:  array_unique($arr);
来源：http://fes.nanxuanxn.top

JS:   [...new Set(arr)]
来源：http://rdu.ctjpmb.com

TS:   [...new Set(arr)]
来源：http://nta.yangfankeji.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://enq.feifeiyinyue.top

Go:   // 用 map[T]struct{} 手写
来源：http://vip.svipenyu.cn

Ruby: arr.uniq
来源：http://zap.jinqigfzy.top

C#:   list.Distinct().ToList()
来源：http://lui.gogol.net.cn

[D16] 求和与平均值
来源：http://evh.chenjidiqi.icu

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xke.shuidangran.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://iqw.mhx1999.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vud.pengpengdd.cyou

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://atd.hammf.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://szm.ivvv.top

Go:   // 手写循环累加
来源：http://qvv.ydzc1.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jvl.yueranfly.top

C#:   list.Sum();  list.Average()
来源：http://pez.cqqwz.cn

[D17] 最大值与最小值
来源：http://wbc.shangyingyoupin.top

Py:   max(arr);  min(arr)
来源：http://uru.ywan-chungtsiang.top

PHP:  max($arr);  min($arr);
来源：http://rxf.fktsv.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fct.sjlbkw.cn

TS:   Math.max(...arr);
来源：http://gji.jlsjyb.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gga.svipenyu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://oyk.zdqjudy.top

Ruby: arr.max;  arr.min
来源：http://jqk.yj20258888.top

C#:   list.Max();  list.Min()
来源：http://yhp.zhiwuduotai.top

[D18] 扁平化嵌套数组
来源：http://lki.ppjwa.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lpx.sysykeji.top

PHP:  array_merge(...$nested);
来源：http://cus.tianlin.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mlb.hammf.cn

TS:   nested.flat();
来源：http://lpf.dashuyun.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mid.ydjk.org.cn

Go:   // 手写双层循环
来源：http://fws.daria6918.cn

Ruby: nested.flatten
来源：http://kzm.cucudq.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://rmr.jyoumei.cn

[D19] 按字段分组
来源：http://zpj.vehdjk.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fgr.shuidangran.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://irz.c1oappe.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kkl.quarkkingdee.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://grr.shanyushiyangtech.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fxa.tianlin.xyz

Go:   // 手写 map[string][]T
来源：http://dps.svipenyu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://duh.aizwys.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mow.zhongyouzk.top

[D20] 统计每个元素出现次数
来源：http://ycr.quarkkingdee.top

Py:   Counter(arr)
来源：http://fdp.xinyue.icu

PHP:  array_count_values($arr);
来源：http://usv.tian-w.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lrf.tianlin.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://you.ywan-chungtsiang.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wmn.shanyushiyangkeji.top

Go:   // 手写 map[T]int
来源：http://jjz.yvedp.cn

Ruby: arr.tally
来源：http://fdd.ydjk.org.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vxk.cheryme.top

[D21] 判断是否包含某元素
来源：http://hus.yonumen.top

Py:   x in arr
来源：http://chc.redwolf501.top

PHP:  in_array($x, $arr, true);
来源：http://xxf.pycfn.com

JS:   arr.includes(x)
来源：http://uxk.hywenlv.cn

TS:   arr.includes(x)
来源：http://idh.ctjpmb.com

Java: list.contains(x)
来源：http://iul.aizwys.cn

Go:   slices.Contains(arr, x)
来源：http://ndz.shanyushiyangtech.top

Ruby: arr.include?(x)
来源：http://kzi.hywenlv.cn

C#:   list.Contains(x)
来源：http://pjr.ydjk.org.cn

[D22] 复制数组（避免共享引用）
来源：http://leg.daxiang520.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vpr.cashguo.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ckt.zhiwuduotai.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jsx.smart0.xyz

TS:   [...arr];
来源：http://lfa.shanyushiyangtech.top

Java: new ArrayList<>(list);
来源：http://tvp.pengpengdd.cyou

Go:   copied := append([]int(nil), arr...)
来源：http://npj.hnxiangtu.top

Ruby: arr.dup;  arr.clone
来源：http://qup.ehwqpu.com

C#:   new List<int>(list);
来源：http://yro.xuetiantiany.cn

[D23] reduce 累积计算
来源：http://pbd.fehbvm.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://oxm.vehdjk.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jdm.jqgfzy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tcr.chenzaomai.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zrr.jqgufenzy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://lox.jinghuilouyu.cn

Go:   // 手写循环
来源：http://zze.sufxvd.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zgc.shzxlz.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xex.sxryk.cn

[D24] 字典 / Map 基本操作
来源：http://bml.hongshengwenyu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mse.smart0.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dle.jiagoushi.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cxi.shzxlz.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wky.sjlbkw.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://abs.yj20258.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://arm.vehdjk.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://asy.pycfn.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fkw.cashguo.top

[D25] Set 集合去重与交并差
来源：http://vpk.yonumen.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://poo.ctjpmb.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yyj.jinqigfzy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://oho.xylfe.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jos.gotoacloud.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://enj.ehwqpu.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://euf.bjfxy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cqx.cucudq.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://szz.yj20258888.top

[D26] 数组转字符串
来源：http://mbm.gogol.net.cn

Py:   ", ".join(map(str, arr))
来源：http://sgi.cqqwz.cn

PHP:  implode(", ", $arr);
来源：http://nwc.hongshengwenyu.top

JS:   arr.join(", ")
来源：http://grl.xylfe.cn

TS:   arr.join(", ")
来源：http://ujh.pengpengdd.cyou

Java: String.join(", ", list)
来源：http://gdt.ywan-chungtsiang.top

Go:   strings.Join(strs, ", ")
来源：http://syf.nwbrower.top

Ruby: arr.join(", ")
来源：http://lkj.svipenyu.cn

C#:   string.Join(", ", list)
来源：http://wjp.haohaochexian.top

================================================================================
来源：http://syg.yuanzhike.top

E. 字符串处理
来源：http://wuf.svipenyu.cn

================================================================================
来源：http://kvd.zhengqikj.top

[E01] 拼接字符串
来源：http://egd.aibaodan.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://eay.fengsongda.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lrq.yvedp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ngh.pycfn.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gdg.jlsjyb.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wcc.aizwys.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qvn.jinqigufen.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tvj.chenzaomai.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gur.svipenyu.cn

[E02] 重复字符串
来源：http://twn.hnqzz.top

Py:   "ab" * 3
来源：http://dqa.hnxiangtu.top

PHP:  str_repeat("ab", 3);
来源：http://hls.kuanghao11.cn

JS:   "ab".repeat(3)
来源：http://nei.yj20258.top

TS:   "ab".repeat(3)
来源：http://mwy.52xcode.cn

Java: "ab".repeat(3)
来源：http://bkm.yj20258888.top

Go:   strings.Repeat("ab", 3)
来源：http://stj.xuetiantiany.cn

Ruby: "ab" * 3
来源：http://tco.ppjwa.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fsq.gaohongyu789.top

[E03] 截取子串
来源：http://bxy.shuidangran.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://din.birdmap.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ihu.52xcode.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jor.hongshengwenyu.top

TS:   s.slice(1, 4)
来源：http://vck.aizwys.cn

Java: s.substring(1, 4)
来源：http://ldv.shzxlz.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pre.vehdjk.com

Ruby: s[1, 3];  s[1..3]
来源：http://kja.shanyushiyangkeji.top

C#:   s.Substring(1, 3)
来源：http://gwy.tianlin.xyz

[E04] 查找子串位置
来源：http://mfc.ydjk.org.cn

Py:   s.find("x");  s.index("x")
来源：http://sow.fanxiaobao.xyz

PHP:  strpos($s, "x");
来源：http://bdv.jinyuanbaomall.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mln.zhixingplan.top

TS:   s.indexOf("x")
来源：http://qmj.havefunace.top

Java: s.indexOf("x")
来源：http://bpk.meibo888.top

Go:   strings.Index(s, "x")
来源：http://fnh.tarul.cn

Ruby: s.index("x")
来源：http://qsg.jyoumei.cn

C#:   s.IndexOf("x")
来源：http://lwn.ybcxt.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://agy.snrcjt.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vwu.sjlbkw.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zpy.snrcjt.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hfp.sxryk.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://pua.fehbvm.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://aqb.xuetiantiany.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pbn.shuidangran.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jxn.dianchejie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vkq.chenzaomai.com

[E06] 替换子串
来源：http://hax.jianghu66.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qom.vehdjk.com

PHP:  str_replace("a", "b", $s);
来源：http://byk.jinyuanbaomall.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lyo.chenjidiqi.icu

TS:   s.replaceAll("a", "b")
来源：http://zem.yfazqb.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qqt.haohaochexian.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bzn.jiagoushi.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://khf.fehbvm.com

C#:   s.Replace("a", "b")
来源：http://cop.52xcode.cn

[E07] 按分隔符拆分
来源：http://bvt.jqgufenzy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kmu.nanxinkj.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tgm.shuidangran.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://zrz.fengsongda.top

TS:   s.split(",")
来源：http://hxx.fengsongda.top

Java: s.split(",");  s.split("\\s+")
来源：http://lnv.yuanzhike.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://umb.tarul.cn


<!-- 参考信息 -->