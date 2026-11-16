代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://omx.ybcxt.top

[C15] 解构 / 展开参数
来源：http://lxd.wangdashe.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ftv.uphjek.com

PHP:  [$a, $b] = $pair;
来源：http://ybg.yongpay.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://azs.316326.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://urk.haohaochexian.top

Java: // 无解构
来源：http://vkp.zhiwuduotai.top

Go:   // 无解构
来源：http://eje.c1oappe.top

Ruby: a, b = pair
来源：http://pfe.jqgfzy.top

C#:   var (a, b) = pair;
来源：http://fqq.52xcode.cn

[C16] 函数 / 方法重载
来源：http://vmi.jqgfzy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://amx.guowangkeji.top

PHP:  // 无重载
来源：http://nan.havefunace.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://pvg.zhijiandao.cn

TS:   // 用联合类型或重载签名声明
来源：http://eef.yueranfly.top

Java: void f(int a) {}  void f(String a) {}
来源：http://qum.hnqzz.top

Go:   // 无重载：用不同函数名
来源：http://llf.jiagoushi.top

Ruby: # 无重载：靠动态参数
来源：http://nft.yuxming.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ivk.jlsjyb.cn

================================================================================
来源：http://lyp.dianchejie.cn

D. 数组 / 列表 / 集合
来源：http://xnx.cheryme.top

================================================================================
来源：http://wwg.hcnkem.com

[D01] 创建数组 / 列表
来源：http://vsr.aibaodan.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jmw.sxryk.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zzu.birdmap.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cqq.gogol.net.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hyx.nanxuanxn.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qjs.meibo888.top

Go:   arr := []int{1, 2, 3}
来源：http://msm.xinyue.icu

Ruby: arr = [1, 2, 3]
来源：http://lnd.jinyuanbaomall.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hbq.redwolf501.top

[D02] 追加元素到末尾
来源：http://ssx.shuidangran.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vzx.jinqigufen.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ans.gotoacloud.top

JS:   arr.push(4);
来源：http://vwi.cqqwz.cn

TS:   arr.push(4);
来源：http://eft.jqgufenzy.top

Java: list.add(4);
来源：http://lzh.nwbrower.top

Go:   arr = append(arr, 4)
来源：http://ftc.hnqzz.top

Ruby: arr << 4; arr.push(5)
来源：http://lbx.gotoacloud.top

C#:   list.Add(4);
来源：http://iff.cqqwz.cn

[D03] 在指定位置插入元素
来源：http://tnf.zhijiandao.cn

Py:   arr.insert(0, 0)
来源：http://dkk.sufxvd.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kph.jinghuilouyu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xzp.dashuyun.cn

TS:   arr.splice(0, 0, 0);
来源：http://rup.shzxlz.cn

Java: list.add(0, 0);
来源：http://zee.chenlongwang.top

Go:   arr = append([]int{0}, arr...)
来源：http://fnh.fzhhl.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mcs.jqgfzy.top

C#:   list.Insert(0, 0);
来源：http://zzf.nanxinkj.top

[D04] 删除元素
来源：http://bfz.yj20258888.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sge.birdmap.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mli.gzhubu.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sgm.sufxvd.cn

TS:   arr.splice(0, 1);
来源：http://rru.zycfv.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gey.feifeiyinyue.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://itw.birdmap.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xjo.hongshengwenyu.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dgm.cqqwz.cn

[D05] 访问与修改元素
来源：http://cub.ywan-chungtsiang.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gjg.shzxlz.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ugw.tian-w.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rea.jiagoushi.top

TS:   arr[0]; arr.at(-1);
来源：http://ubm.sjlbkw.cn

Java: list.get(0); list.set(0, 9);
来源：http://eex.yvedp.cn

Go:   arr[0]; arr[0] = 9
来源：http://xvf.zhixingplan.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jyz.9152youxi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zhx.yj20258.top

[D06] 数组长度
来源：http://fmv.gaohongyu789.top

Py:   len(arr)
来源：http://lsw.tarul.cn

PHP:  count($arr);
来源：http://zgm.daxiang520.top

JS:   arr.length
来源：http://mim.yanxiufei.cn

TS:   arr.length
来源：http://yjx.tanke756.top

Java: list.size();
来源：http://cho.jyoumei.cn

Go:   len(arr)
来源：http://cyn.jinyuanbaomall.cn

Ruby: arr.length; arr.size
来源：http://czy.cashguo.top

C#:   list.Count;
来源：http://lty.ivvv.top

[D07] 切片 / 取子数组
来源：http://zje.yanxiufei.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wne.jinqigufen.top

PHP:  array_slice($arr, 1, 3);
来源：http://jxf.tian-w.cn

JS:   arr.slice(1, 4);
来源：http://upd.sysykeji.top

TS:   arr.slice(1, 4);
来源：http://hkq.xylfe.cn

Java: list.subList(1, 4);
来源：http://ebn.jinyuanbaomall.cn

Go:   arr[1:4]
来源：http://pya.feifeiyinyue.top

Ruby: arr[1, 3]
来源：http://teg.gogol.net.cn

C#:   list.GetRange(1, 3);
来源：http://eap.jlsjyb.cn

[D08] 合并两个数组
来源：http://rvu.wangshuangyany.cn

Py:   a + b;  a.extend(b)
来源：http://dxy.c1oappe.top

PHP:  array_merge($a, $b);
来源：http://tri.ybcxt.top

JS:   [...a, ...b];  a.concat(b);
来源：http://pla.hnxiangtu.top

TS:   [...a, ...b];
来源：http://ehw.c1oappe.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xsq.meibo888.top

Go:   append(a, b...)
来源：http://wip.jlsjyb.cn

Ruby: a + b;  a.concat(b)
来源：http://tqw.pengpengdd.cyou

C#:   a.Concat(b).ToList()
来源：http://tti.hammf.cn

[D09] 排序（升序）
来源：http://xrw.aizwys.cn

Py:   sorted(arr);  arr.sort()
来源：http://mrt.dianchejie.cn

PHP:  sort($arr);
来源：http://srf.52xcode.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zcs.dashuyun.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://mjc.zhaomingkeji.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://ovn.tarul.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tkc.nanxuanxn.top

Ruby: arr.sort
来源：http://kyb.xziqi.cn

C#:   list.Sort();
来源：http://gnk.ybcxt.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://exm.guannengcc.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hlj.vehdjk.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mcu.nanxinkj.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rgk.iojbl.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hpe.dashuyun.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ejp.jianghu66.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fwr.ivvv.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ust.daxiang520.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cyj.hammf.cn

[D11] 反转数组
来源：http://abp.xuetiantiany.cn

Py:   arr[::-1];  arr.reverse()
来源：http://bzh.fktsv.cn

PHP:  array_reverse($arr);
来源：http://fro.jinqigufen.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zwz.andypj.xyz

TS:   [...arr].reverse();
来源：http://emd.vehdjk.com

Java: Collections.reverse(list);
来源：http://vch.haohaochexian.top

Go:   slices.Reverse(arr)
来源：http://xid.feifeiyinyue.top

Ruby: arr.reverse
来源：http://avo.jinyuanbaomall.cn

C#:   list.Reverse();
来源：http://pdn.yonumen.top

[D12] 查找元素下标
来源：http://cww.yuxming.cn

Py:   arr.index(x);  x in arr
来源：http://kns.xziqi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lwt.hongshengwenyu.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wlc.yvedp.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mej.ybcxt.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uay.hcnkem.com

Go:   slices.Index(arr, x)
来源：http://cjb.uphjek.com

Ruby: arr.index(x)
来源：http://pya.mhx1999.top

C#:   list.IndexOf(x);
来源：http://ota.yj20258888.top

[D13] 过滤（保留满足条件的）
来源：http://ebs.haohaochexian.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ffq.redwolf501.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://heb.yongpay.top

JS:   arr.filter(x => x > 3)
来源：http://ygc.fktsv.cn

TS:   arr.filter(x => x > 3)
来源：http://ttj.redwolf501.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wlc.mhx1999.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pla.zdbjq.cn

Ruby: arr.select { |x| x > 3 }
来源：http://sbe.hammf.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bzw.yuanzhike.top

[D14] 映射转换（每个元素变形）
来源：http://xfr.iojbl.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wvi.tian-w.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bsg.chenlongwang.top

JS:   arr.map(x => x * 2)
来源：http://ang.jiagoushi.top

TS:   arr.map(x => x * 2)
来源：http://osz.zycfv.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://rix.guannengcc.top

Go:   // 手写循环
来源：http://zmk.jiagoushi.top

Ruby: arr.map { |x| x * 2 }
来源：http://ctg.hesvh.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://etq.zhengqikj.top

[D15] 去重
来源：http://jib.jinghuilouyu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://iaa.fehbvm.com

PHP:  array_unique($arr);
来源：http://bfb.iojbl.cn

JS:   [...new Set(arr)]
来源：http://wfe.shzxlz.cn

TS:   [...new Set(arr)]
来源：http://nay.jinqigufen.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qmx.yanxiufei.cn

Go:   // 用 map[T]struct{} 手写
来源：http://msm.cashguo.top

Ruby: arr.uniq
来源：http://dbo.tarul.cn

C#:   list.Distinct().ToList()
来源：http://quc.cdnleiting.top

[D16] 求和与平均值
来源：http://mtk.yongpay.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xeu.zdqjudy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yoe.9152youxi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://stk.tarul.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://luj.zhixingplan.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cnw.jinqigfzy.top

Go:   // 手写循环累加
来源：http://ycc.havefunace.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://frb.wangshuangyany.cn

C#:   list.Sum();  list.Average()
来源：http://ntx.ctjpmb.com

[D17] 最大值与最小值
来源：http://ybx.nanxinkj.top

Py:   max(arr);  min(arr)
来源：http://vvv.dashuyun.cn

PHP:  max($arr);  min($arr);
来源：http://kfa.bjfxy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sey.wangdashe.top

TS:   Math.max(...arr);
来源：http://zpf.jqgufenzy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://bkh.chenjidiqi.icu

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mly.yj20258.top

Ruby: arr.max;  arr.min
来源：http://lrw.xylfe.cn

C#:   list.Max();  list.Min()
来源：http://twl.52xcode.cn

[D18] 扁平化嵌套数组
来源：http://dmr.xuanzx.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ewn.yj20258.top

PHP:  array_merge(...$nested);
来源：http://fro.sysykeji.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xml.chenjidiqi.icu

TS:   nested.flat();
来源：http://khl.chenjidiqi.icu

Java: nested.stream().flatMap(List::stream).toList()
来源：http://iak.zhijiandao.cn

Go:   // 手写双层循环
来源：http://cxz.guowangkeji.top

Ruby: nested.flatten
来源：http://yid.yongpay.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://gvs.kuanghao11.cn

[D19] 按字段分组
来源：http://lkp.vqdsnc.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ppx.feifeiyinyue.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mbr.smart0.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gup.yuanzhike.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://psm.zhixingplan.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://efp.jiagoushi.top

Go:   // 手写 map[string][]T
来源：http://equ.hammf.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ona.yj202588.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tdt.sxryk.cn

[D20] 统计每个元素出现次数
来源：http://wwv.shanyushiyangtech.top

Py:   Counter(arr)
来源：http://you.yanxiufei.cn

PHP:  array_count_values($arr);
来源：http://quo.hysaishi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://paz.zhiwuduotai.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zrt.ctjpmb.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ede.daxiang520.top

Go:   // 手写 map[T]int
来源：http://bfj.ctjpmb.com

Ruby: arr.tally
来源：http://gys.jinyuanbaomall.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qsy.redwolf501.top

[D21] 判断是否包含某元素
来源：http://qcn.wangshuangyany.cn

Py:   x in arr
来源：http://weu.bjfxy.top

PHP:  in_array($x, $arr, true);
来源：http://zga.zhiwuduotai.top

JS:   arr.includes(x)
来源：http://upg.tarul.cn

TS:   arr.includes(x)
来源：http://uhs.ivvv.top

Java: list.contains(x)
来源：http://zjf.zhengqikj.top

Go:   slices.Contains(arr, x)
来源：http://wus.hcnkem.com

Ruby: arr.include?(x)
来源：http://iut.wangdashe.top

C#:   list.Contains(x)
来源：http://wqn.dianchejie.cn

[D22] 复制数组（避免共享引用）
来源：http://hci.zdqjudy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lng.xinyue.icu

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://eot.jianghu66.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://exf.zycfv.cn

TS:   [...arr];
来源：http://nmk.meibo888.top

Java: new ArrayList<>(list);
来源：http://oro.haohaochexian.top

Go:   copied := append([]int(nil), arr...)
来源：http://vkr.xylfe.cn

Ruby: arr.dup;  arr.clone
来源：http://fcb.xinyue.icu

C#:   new List<int>(list);
来源：http://mpd.kuanghao11.cn

[D23] reduce 累积计算
来源：http://yxe.sjlbkw.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vvm.zycfv.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vuw.hysaishi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://atz.yj20258.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qtn.yueranfly.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://avd.vqdsnc.cn

Go:   // 手写循环
来源：http://esi.xuanzx.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zff.chenzaomai.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gyy.svipenyu.cn

[D24] 字典 / Map 基本操作
来源：http://gkt.chenjidiqi.icu

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kqf.shuidangran.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://aan.zhoulong.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lzz.yueranfly.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dok.sweek.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ahh.jqgufenzy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ott.ctjpmb.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nzg.jiagoushi.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rrg.iojbl.cn

[D25] Set 集合去重与交并差
来源：http://ifm.zhaomingkeji.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jjw.xziqi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gcc.nwbrower.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://siu.bbcook.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vna.kuanghao11.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ztd.shanyushiyangkeji.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sww.cqqwz.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jgq.aizwys.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://iwa.zhongyouzk.top

[D26] 数组转字符串
来源：http://wip.epnwcf.com

Py:   ", ".join(map(str, arr))
来源：http://zic.jlsjyb.cn

PHP:  implode(", ", $arr);
来源：http://joj.fanxiaobao.xyz

JS:   arr.join(", ")
来源：http://vej.xinyue.icu

TS:   arr.join(", ")
来源：http://sho.ppjwa.cn

Java: String.join(", ", list)
来源：http://gvl.andypj.xyz

Go:   strings.Join(strs, ", ")
来源：http://omc.jqgfzy.top

Ruby: arr.join(", ")
来源：http://xwv.jiagoushi.top

C#:   string.Join(", ", list)
来源：http://klh.feifeiyinyue.top

================================================================================
来源：http://mhd.tarul.cn

E. 字符串处理
来源：http://fbr.daxiang520.top

================================================================================
来源：http://ryw.daxiang520.top

[E01] 拼接字符串
来源：http://gjj.hfpthk.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ewc.zhaomingkeji.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nas.iojbl.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jpu.yonumen.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xbh.ctjpmb.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gje.ywan-chungtsiang.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zmm.cucudq.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qnv.ydjk.org.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://iks.jinqigfzy.top

[E02] 重复字符串
来源：http://gmt.fzhhl.top

Py:   "ab" * 3
来源：http://ihr.hnxiangtu.top

PHP:  str_repeat("ab", 3);
来源：http://zjn.jyoumei.cn

JS:   "ab".repeat(3)
来源：http://zff.sweek.top

TS:   "ab".repeat(3)
来源：http://enh.zycfv.cn

Java: "ab".repeat(3)
来源：http://kpa.iojbl.cn

Go:   strings.Repeat("ab", 3)
来源：http://czm.jiagoushi.top

Ruby: "ab" * 3
来源：http://iyl.tianlin.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://axw.guannengcc.top

[E03] 截取子串
来源：http://iik.hesvh.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rxe.yuxming.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bgy.zhiwuduotai.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://oxd.shzxlz.cn

TS:   s.slice(1, 4)
来源：http://mct.fengsongda.top

Java: s.substring(1, 4)
来源：http://jph.yj202588.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lbe.wangdashe.top

Ruby: s[1, 3];  s[1..3]
来源：http://vfb.ydjk.org.cn

C#:   s.Substring(1, 3)
来源：http://ugo.yuxming.cn

[E04] 查找子串位置
来源：http://hdc.hnqzz.top

Py:   s.find("x");  s.index("x")
来源：http://nez.fzhhl.top

PHP:  strpos($s, "x");
来源：http://ivc.sufxvd.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kqb.yongpay.top

TS:   s.indexOf("x")
来源：http://nan.birdmap.top

Java: s.indexOf("x")
来源：http://rcm.jinqigfzy.top

Go:   strings.Index(s, "x")
来源：http://trd.wangdashe.top

Ruby: s.index("x")
来源：http://aio.zhijiandao.cn

C#:   s.IndexOf("x")
来源：http://hwm.yonumen.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://bij.sjlbkw.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mex.hfpthk.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pqp.jinqigufen.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wtk.yangfankeji.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://sox.yj20258888.top


<!-- 参考信息 -->