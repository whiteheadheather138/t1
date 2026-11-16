代发 wailian999

PHP:  // 无重载
来源：http://kjd.aibaodan.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://suq.xuanzx.com

TS:   // 用联合类型或重载签名声明
来源：http://lrg.yj202588.top

Java: void f(int a) {}  void f(String a) {}
来源：http://fhf.hcnkem.com

Go:   // 无重载：用不同函数名
来源：http://rbg.zhongyouzk.top

Ruby: # 无重载：靠动态参数
来源：http://yvm.zycfv.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://uyu.shanyushiyangtech.top

================================================================================
来源：http://llz.ydjk.org.cn

D. 数组 / 列表 / 集合
来源：http://hog.daria6918.cn

================================================================================
来源：http://qva.chenjidiqi.icu

[D01] 创建数组 / 列表
来源：http://njn.zhaomingkeji.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://ynn.gogol.net.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kxz.guowangkeji.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bwf.cashguo.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://bux.ywan-chungtsiang.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lyw.ybcxt.top

Go:   arr := []int{1, 2, 3}
来源：http://dyj.gaohongyu789.top

Ruby: arr = [1, 2, 3]
来源：http://xfx.zdqjudy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ygz.hysaishi.cn

[D02] 追加元素到末尾
来源：http://qfc.hywenlv.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ibm.haohaochexian.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://uhr.hfpthk.cn

JS:   arr.push(4);
来源：http://tqc.yj202588.top

TS:   arr.push(4);
来源：http://xlz.yj20258.top

Java: list.add(4);
来源：http://oeb.tarul.cn

Go:   arr = append(arr, 4)
来源：http://rcy.zhijiandao.cn

Ruby: arr << 4; arr.push(5)
来源：http://mvz.ppjwa.cn

C#:   list.Add(4);
来源：http://vrg.9152youxi.cn

[D03] 在指定位置插入元素
来源：http://qxi.andypj.xyz

Py:   arr.insert(0, 0)
来源：http://pbk.ppjwa.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://llu.zhixingplan.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wbd.pycfn.com

TS:   arr.splice(0, 0, 0);
来源：http://euv.daxiang520.top

Java: list.add(0, 0);
来源：http://qph.bjfxy.top

Go:   arr = append([]int{0}, arr...)
来源：http://mfw.0kj1m.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cxy.ydzc1.top

C#:   list.Insert(0, 0);
来源：http://ljg.fktsv.cn

[D04] 删除元素
来源：http://plg.fehbvm.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nde.jyoumei.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qmb.quarkkingdee.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rya.c1oappe.top

TS:   arr.splice(0, 1);
来源：http://xfk.gaohongyu789.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vpp.havefunace.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vmj.wangdashe.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ymt.iojbl.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lyz.epnwcf.com

[D05] 访问与修改元素
来源：http://jfg.shzxlz.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sru.9152youxi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fxu.yj202588.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://eyx.jiagoushi.top

TS:   arr[0]; arr.at(-1);
来源：http://sfn.xuetiantiany.cn

Java: list.get(0); list.set(0, 9);
来源：http://deo.smart0.xyz

Go:   arr[0]; arr[0] = 9
来源：http://afe.yonumen.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dou.hammf.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tyi.haohaochexian.top

[D06] 数组长度
来源：http://ody.smart0.xyz

Py:   len(arr)
来源：http://ocq.dashuyun.cn

PHP:  count($arr);
来源：http://gcn.hnxiangtu.top

JS:   arr.length
来源：http://ibc.dashuyun.cn

TS:   arr.length
来源：http://tmz.zdbjq.cn

Java: list.size();
来源：http://zhz.hammf.cn

Go:   len(arr)
来源：http://twm.yanxiufei.cn

Ruby: arr.length; arr.size
来源：http://wnq.dianchejie.cn

C#:   list.Count;
来源：http://pwy.sweek.top

[D07] 切片 / 取子数组
来源：http://dud.pengpengdd.cyou

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bbm.yanxiufei.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vxy.jianghu66.top

JS:   arr.slice(1, 4);
来源：http://iit.fengsongda.top

TS:   arr.slice(1, 4);
来源：http://fxl.9152youxi.cn

Java: list.subList(1, 4);
来源：http://vel.ppjwa.cn

Go:   arr[1:4]
来源：http://npv.yongpay.top

Ruby: arr[1, 3]
来源：http://dpp.xingfuxueyuan.xyz

C#:   list.GetRange(1, 3);
来源：http://izl.hywenlv.cn

[D08] 合并两个数组
来源：http://cxy.chenzaomai.com

Py:   a + b;  a.extend(b)
来源：http://tmg.tianlin.xyz

PHP:  array_merge($a, $b);
来源：http://nvw.zhongyouzk.top

JS:   [...a, ...b];  a.concat(b);
来源：http://vmg.andypj.xyz

TS:   [...a, ...b];
来源：http://tto.nanxinkj.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xin.hongshengwenyu.top

Go:   append(a, b...)
来源：http://pbc.0kj1m.cn

Ruby: a + b;  a.concat(b)
来源：http://msj.yongpay.top

C#:   a.Concat(b).ToList()
来源：http://mox.xziqi.cn

[D09] 排序（升序）
来源：http://bdc.tianlin.xyz

Py:   sorted(arr);  arr.sort()
来源：http://gvn.quarkkingdee.top

PHP:  sort($arr);
来源：http://kuw.c1oappe.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xzz.yj20258888.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://jhn.sysykeji.top

Java: Collections.sort(list);  list.sort(null);
来源：http://hub.chenjidiqi.icu

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qlb.cdnleiting.top

Ruby: arr.sort
来源：http://qqk.c1oappe.top

C#:   list.Sort();
来源：http://wcn.yfazqb.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://zlz.jinqigufen.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bne.iojbl.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jbd.smart0.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yej.hesvh.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ppk.c1oappe.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cgz.hysaishi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ide.ctjpmb.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ksf.pengpengdd.cyou

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jvk.nwbrower.top

[D11] 反转数组
来源：http://ijk.52xcode.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ggl.zhijiandao.cn

PHP:  array_reverse($arr);
来源：http://vxr.ydzc1.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vrw.ppjwa.cn

TS:   [...arr].reverse();
来源：http://rha.jqgufenzy.top

Java: Collections.reverse(list);
来源：http://ohf.9152youxi.cn

Go:   slices.Reverse(arr)
来源：http://uqg.yfazqb.com

Ruby: arr.reverse
来源：http://sep.fanxiaobao.xyz

C#:   list.Reverse();
来源：http://npd.hesvh.cn

[D12] 查找元素下标
来源：http://unq.ybcxt.top

Py:   arr.index(x);  x in arr
来源：http://luk.bjfxy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fpl.yfazqb.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://plv.ppjwa.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wrm.svipenyu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ezr.gogol.net.cn

Go:   slices.Index(arr, x)
来源：http://ivg.wangdashe.top

Ruby: arr.index(x)
来源：http://nxn.havefunace.top

C#:   list.IndexOf(x);
来源：http://kdc.fktsv.cn

[D13] 过滤（保留满足条件的）
来源：http://hhh.52xcode.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sdq.hysaishi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://uuk.quarkkingdee.top

JS:   arr.filter(x => x > 3)
来源：http://icd.epnwcf.com

TS:   arr.filter(x => x > 3)
来源：http://okc.52xcode.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rla.hywenlv.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ege.c1oappe.top

Ruby: arr.select { |x| x > 3 }
来源：http://ngv.aibaodan.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://uxp.hongshengwenyu.top

[D14] 映射转换（每个元素变形）
来源：http://ksa.ydjk.org.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://suv.zhixingplan.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rds.zhiwuduotai.top

JS:   arr.map(x => x * 2)
来源：http://thd.zhengqikj.top

TS:   arr.map(x => x * 2)
来源：http://mut.yj20258.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://uid.uphjek.com

Go:   // 手写循环
来源：http://fno.redwolf501.top

Ruby: arr.map { |x| x * 2 }
来源：http://bdo.zhongyouzk.top

C#:   list.Select(x => x * 2).ToList()
来源：http://nhj.fehbvm.com

[D15] 去重
来源：http://vdc.epnwcf.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fuo.zhijiandao.cn

PHP:  array_unique($arr);
来源：http://wzf.fehbvm.com

JS:   [...new Set(arr)]
来源：http://xim.hammf.cn

TS:   [...new Set(arr)]
来源：http://juo.yfazqb.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://itt.vehdjk.com

Go:   // 用 map[T]struct{} 手写
来源：http://xsh.zdbjq.cn

Ruby: arr.uniq
来源：http://qps.hnqzz.top

C#:   list.Distinct().ToList()
来源：http://wqc.hfpthk.cn

[D16] 求和与平均值
来源：http://man.bbcook.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gxi.tanke756.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ytg.snrcjt.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ltd.ehwqpu.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://uiz.tian-w.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yoe.hnqzz.top

Go:   // 手写循环累加
来源：http://sjn.cashguo.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bba.ydzc1.top

C#:   list.Sum();  list.Average()
来源：http://gbd.zhoulong.xyz

[D17] 最大值与最小值
来源：http://obx.shzxlz.cn

Py:   max(arr);  min(arr)
来源：http://kpc.yj202588.top

PHP:  max($arr);  min($arr);
来源：http://jvv.zhaomingkeji.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://seh.dashuyun.cn

TS:   Math.max(...arr);
来源：http://unu.daria6918.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://nur.yfazqb.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lot.zhoulong.xyz

Ruby: arr.max;  arr.min
来源：http://apl.jinyuanbaomall.cn

C#:   list.Max();  list.Min()
来源：http://pqe.ctjpmb.com

[D18] 扁平化嵌套数组
来源：http://iyg.ehwqpu.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://crp.zdbjq.cn

PHP:  array_merge(...$nested);
来源：http://qzt.kuanghao11.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://alt.tarul.cn

TS:   nested.flat();
来源：http://rxk.vehdjk.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vex.shuidangran.top

Go:   // 手写双层循环
来源：http://dqz.haohaochexian.top

Ruby: nested.flatten
来源：http://xtu.jinqigfzy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://anm.aibaodan.cn

[D19] 按字段分组
来源：http://rjt.chenlongwang.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ypk.tianlin.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ykj.daxiang520.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tja.ehwqpu.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://rrw.xingfuxueyuan.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wcq.vehdjk.com

Go:   // 手写 map[string][]T
来源：http://dgl.jinyuanbaomall.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://tio.yj20258.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ewp.fanxiaobao.xyz

[D20] 统计每个元素出现次数
来源：http://kvk.daxiang520.top

Py:   Counter(arr)
来源：http://qio.guannengcc.top

PHP:  array_count_values($arr);
来源：http://zfz.dianchejie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://omw.shzxlz.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ihv.c1oappe.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tcp.hnqzz.top

Go:   // 手写 map[T]int
来源：http://nyo.nanxuanxn.top

Ruby: arr.tally
来源：http://ksd.dashuyun.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hmb.nanxuanxn.top

[D21] 判断是否包含某元素
来源：http://bbg.pycfn.com

Py:   x in arr
来源：http://sfv.9152youxi.cn

PHP:  in_array($x, $arr, true);
来源：http://qkb.aibaodan.cn

JS:   arr.includes(x)
来源：http://kph.zdqjudy.top

TS:   arr.includes(x)
来源：http://rby.zhiwuduotai.top

Java: list.contains(x)
来源：http://phn.zhoulong.xyz

Go:   slices.Contains(arr, x)
来源：http://vlv.yongpay.top

Ruby: arr.include?(x)
来源：http://kds.jinyuanbaomall.cn

C#:   list.Contains(x)
来源：http://kbr.jianghu66.top

[D22] 复制数组（避免共享引用）
来源：http://jcv.bjfxy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jhh.fktsv.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://def.yangfankeji.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lhh.xuetiantiany.cn

TS:   [...arr];
来源：http://ond.nwbrower.top

Java: new ArrayList<>(list);
来源：http://fxg.cdnleiting.top

Go:   copied := append([]int(nil), arr...)
来源：http://hri.dashuyun.cn

Ruby: arr.dup;  arr.clone
来源：http://mkx.smart0.xyz

C#:   new List<int>(list);
来源：http://ecg.smart0.xyz

[D23] reduce 累积计算
来源：http://zpe.mhx1999.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://iyz.shanyushiyangtech.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uqm.cucudq.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bkr.hongshengwenyu.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gws.hnxiangtu.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://qiy.c1oappe.top

Go:   // 手写循环
来源：http://myd.yj20258888.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jcg.sjlbkw.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ljd.xziqi.cn

[D24] 字典 / Map 基本操作
来源：http://knf.hysaishi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://oqf.svipenyu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mhr.epnwcf.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://phg.aibaodan.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jyn.fzhhl.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://enu.daria6918.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gvf.fanxiaobao.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xlu.316326.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yxv.pengpengdd.cyou

[D25] Set 集合去重与交并差
来源：http://zue.ywan-chungtsiang.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ohl.zdbjq.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rgb.ywan-chungtsiang.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hmd.jqgufenzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xff.wangdashe.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mek.vehdjk.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://loz.iojbl.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sjq.daria6918.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ryv.tanke756.top

[D26] 数组转字符串
来源：http://asl.zhiwuduotai.top

Py:   ", ".join(map(str, arr))
来源：http://not.jlsjyb.cn

PHP:  implode(", ", $arr);
来源：http://cup.wangdashe.top

JS:   arr.join(", ")
来源：http://wef.kuanghao11.cn

TS:   arr.join(", ")
来源：http://kom.jlsjyb.cn

Java: String.join(", ", list)
来源：http://ebd.hnqzz.top

Go:   strings.Join(strs, ", ")
来源：http://wco.fehbvm.com

Ruby: arr.join(", ")
来源：http://tvq.xziqi.cn

C#:   string.Join(", ", list)
来源：http://aov.fanxiaobao.xyz

================================================================================
来源：http://gvy.cucudq.cn

E. 字符串处理
来源：http://sxu.pengpengdd.cyou

================================================================================
来源：http://bev.dianchejie.cn

[E01] 拼接字符串
来源：http://ihr.fehbvm.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cet.shanyushiyangtech.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tku.yuxming.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ujt.uphjek.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nat.ppjwa.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://woo.tian-w.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cdh.jqgfzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nie.fktsv.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://frb.jinyuanbaomall.cn

[E02] 重复字符串
来源：http://rvs.ydzc1.top

Py:   "ab" * 3
来源：http://mmb.ctjpmb.com

PHP:  str_repeat("ab", 3);
来源：http://xln.yonumen.top

JS:   "ab".repeat(3)
来源：http://jun.nanxuanxn.top

TS:   "ab".repeat(3)
来源：http://uxp.hysaishi.cn

Java: "ab".repeat(3)
来源：http://csc.gogol.net.cn

Go:   strings.Repeat("ab", 3)
来源：http://dqt.haohaochexian.top

Ruby: "ab" * 3
来源：http://fro.shanyushiyangtech.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ftv.tanke756.top

[E03] 截取子串
来源：http://bps.meibo888.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://spr.cqqwz.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pwh.yangfankeji.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://azb.vqdsnc.cn

TS:   s.slice(1, 4)
来源：http://wdy.shuidangran.top

Java: s.substring(1, 4)
来源：http://eyq.epnwcf.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rjv.cdnleiting.top

Ruby: s[1, 3];  s[1..3]
来源：http://drt.cqqwz.cn

C#:   s.Substring(1, 3)
来源：http://eif.9152youxi.cn

[E04] 查找子串位置
来源：http://ykc.sufxvd.cn

Py:   s.find("x");  s.index("x")
来源：http://qau.feifeiyinyue.top

PHP:  strpos($s, "x");
来源：http://wbx.xuetiantiany.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wmf.316326.xyz

TS:   s.indexOf("x")
来源：http://awu.hysaishi.cn

Java: s.indexOf("x")
来源：http://bpx.52xcode.cn

Go:   strings.Index(s, "x")
来源：http://vuc.hnqzz.top

Ruby: s.index("x")
来源：http://umc.shanyushiyangkeji.top

C#:   s.IndexOf("x")
来源：http://bxr.zhixingplan.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://xhg.chenzaomai.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://emk.guannengcc.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://roe.zycfv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yna.sweek.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://pqe.yueranfly.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dub.yj202588.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fqq.zhongyouzk.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kxx.snrcjt.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qmz.sysykeji.top

[E06] 替换子串
来源：http://wcu.iojbl.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gwo.sxryk.cn

PHP:  str_replace("a", "b", $s);
来源：http://bqc.fktsv.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cgg.daxiang520.top

TS:   s.replaceAll("a", "b")
来源：http://ncs.zycfv.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://saj.jiagoushi.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zos.daria6918.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dlh.yongpay.top


<!-- 参考信息 -->