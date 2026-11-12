代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://nzu.daria6918.cn

Go:   func add(a, b int) int
来源：http://dma.wangdashe.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://eml.316326.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://psf.iojbl.cn

[C14] 泛型函数
来源：http://qac.pengpengdd.cyou

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rkl.haohaochexian.top

PHP:  // 无泛型
来源：http://oha.cqqwz.cn

JS:   // 无泛型
来源：http://xrj.chenzaomai.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vaq.pycfn.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bon.meibo888.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://oup.jianghu66.top

Ruby: # 无泛型
来源：http://kra.epnwcf.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vgn.yongpay.top

[C15] 解构 / 展开参数
来源：http://vlp.cqqwz.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fjd.nanxuanxn.top

PHP:  [$a, $b] = $pair;
来源：http://vgw.iojbl.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://afu.shzxlz.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wjw.jinqigufen.top

Java: // 无解构
来源：http://tth.xuetiantiany.cn

Go:   // 无解构
来源：http://lvx.52xcode.cn

Ruby: a, b = pair
来源：http://lxs.zhiwuduotai.top

C#:   var (a, b) = pair;
来源：http://pjm.nanxinkj.top

[C16] 函数 / 方法重载
来源：http://uyh.zdqjudy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dhw.bbcook.cn

PHP:  // 无重载
来源：http://ddx.chenzaomai.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://boa.sweek.top

TS:   // 用联合类型或重载签名声明
来源：http://crk.jinghuilouyu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ozc.redwolf501.top

Go:   // 无重载：用不同函数名
来源：http://pyj.zhixingplan.top

Ruby: # 无重载：靠动态参数
来源：http://qce.redwolf501.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://mrj.cucudq.cn

================================================================================
来源：http://nsv.jianghu66.top

D. 数组 / 列表 / 集合
来源：http://omc.chenzaomai.com

================================================================================
来源：http://rzt.hywenlv.cn

[D01] 创建数组 / 列表
来源：http://ojd.52xcode.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://djx.fktsv.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ryo.shzxlz.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hca.zhiwuduotai.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://zuh.yonumen.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://leq.dashuyun.cn

Go:   arr := []int{1, 2, 3}
来源：http://prd.kuanghao11.cn

Ruby: arr = [1, 2, 3]
来源：http://hvw.shanyushiyangtech.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jop.smart0.xyz

[D02] 追加元素到末尾
来源：http://eyb.wangshuangyany.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gns.hongshengwenyu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://djs.iojbl.cn

JS:   arr.push(4);
来源：http://iwk.tanke756.top

TS:   arr.push(4);
来源：http://ohx.guowangkeji.top

Java: list.add(4);
来源：http://wct.9152youxi.cn

Go:   arr = append(arr, 4)
来源：http://jhu.xziqi.cn

Ruby: arr << 4; arr.push(5)
来源：http://biq.hfpthk.cn

C#:   list.Add(4);
来源：http://swf.svipenyu.cn

[D03] 在指定位置插入元素
来源：http://oue.ydzc1.top

Py:   arr.insert(0, 0)
来源：http://kau.xuetiantiany.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wox.cashguo.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tks.sweek.top

TS:   arr.splice(0, 0, 0);
来源：http://qld.pengpengdd.cyou

Java: list.add(0, 0);
来源：http://pdb.ehwqpu.com

Go:   arr = append([]int{0}, arr...)
来源：http://aon.hnqzz.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jou.zdbjq.cn

C#:   list.Insert(0, 0);
来源：http://jpb.jinqigufen.top

[D04] 删除元素
来源：http://mvy.pengpengdd.cyou

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gto.jqgfzy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zzp.svipenyu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ygh.jinyuanbaomall.cn

TS:   arr.splice(0, 1);
来源：http://adt.yonumen.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://eia.shanyushiyangkeji.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lwh.316326.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xdl.zhoulong.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uzw.jlsjyb.cn

[D05] 访问与修改元素
来源：http://wpd.bjfxy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dvx.yfazqb.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dah.xinyue.icu

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jux.aibaodan.cn

TS:   arr[0]; arr.at(-1);
来源：http://mwl.redwolf501.top

Java: list.get(0); list.set(0, 9);
来源：http://umv.snrcjt.cn

Go:   arr[0]; arr[0] = 9
来源：http://wug.52xcode.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bem.sysykeji.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rfj.pengpengdd.cyou

[D06] 数组长度
来源：http://yaw.guannengcc.top

Py:   len(arr)
来源：http://bgi.zhengqikj.top

PHP:  count($arr);
来源：http://qtx.tanke756.top

JS:   arr.length
来源：http://ngk.jyoumei.cn

TS:   arr.length
来源：http://xzu.dianchejie.cn

Java: list.size();
来源：http://vkk.yueranfly.top

Go:   len(arr)
来源：http://orx.fehbvm.com

Ruby: arr.length; arr.size
来源：http://dsv.jinghuilouyu.cn

C#:   list.Count;
来源：http://scg.feifeiyinyue.top

[D07] 切片 / 取子数组
来源：http://uop.fengsongda.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jgm.havefunace.top

PHP:  array_slice($arr, 1, 3);
来源：http://poi.cqqwz.cn

JS:   arr.slice(1, 4);
来源：http://ieu.gzhubu.top

TS:   arr.slice(1, 4);
来源：http://fgq.fengsongda.top

Java: list.subList(1, 4);
来源：http://pul.pengpengdd.cyou

Go:   arr[1:4]
来源：http://baq.jiagoushi.top

Ruby: arr[1, 3]
来源：http://tkg.jqgufenzy.top

C#:   list.GetRange(1, 3);
来源：http://fiy.jqgufenzy.top

[D08] 合并两个数组
来源：http://yyb.yj20258888.top

Py:   a + b;  a.extend(b)
来源：http://cxt.tanke756.top

PHP:  array_merge($a, $b);
来源：http://ikc.xingfuxueyuan.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://tsb.xuetiantiany.cn

TS:   [...a, ...b];
来源：http://fzt.fanxiaobao.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fhs.jinqigufen.top

Go:   append(a, b...)
来源：http://pou.hnqzz.top

Ruby: a + b;  a.concat(b)
来源：http://imy.shzxlz.cn

C#:   a.Concat(b).ToList()
来源：http://jbq.iojbl.cn

[D09] 排序（升序）
来源：http://twz.cdnleiting.top

Py:   sorted(arr);  arr.sort()
来源：http://tho.sxryk.cn

PHP:  sort($arr);
来源：http://xgy.bjfxy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xid.chenzaomai.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://vgs.fktsv.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://dgu.cqqwz.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kvq.jinghuilouyu.cn

Ruby: arr.sort
来源：http://hkx.jqgfzy.top

C#:   list.Sort();
来源：http://qdz.yj202588.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://lsd.haohaochexian.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gac.zhaomingkeji.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ech.jinqigufen.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vpn.kuanghao11.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xrq.quarkkingdee.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zfv.shangyingyoupin.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://giu.cqqwz.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pat.tarul.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ocz.yvedp.cn

[D11] 反转数组
来源：http://jhe.ybcxt.top

Py:   arr[::-1];  arr.reverse()
来源：http://bpk.fehbvm.com

PHP:  array_reverse($arr);
来源：http://xxj.zhixingplan.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sma.sufxvd.cn

TS:   [...arr].reverse();
来源：http://wdw.tian-w.cn

Java: Collections.reverse(list);
来源：http://foq.shangyingyoupin.top

Go:   slices.Reverse(arr)
来源：http://ybq.shzxlz.cn

Ruby: arr.reverse
来源：http://zla.sysykeji.top

C#:   list.Reverse();
来源：http://ajh.zdbjq.cn

[D12] 查找元素下标
来源：http://amt.haohaochexian.top

Py:   arr.index(x);  x in arr
来源：http://yvg.zhixingplan.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rjg.hysaishi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qog.epnwcf.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pbx.ybcxt.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uad.fengsongda.top

Go:   slices.Index(arr, x)
来源：http://ovu.jinqigufen.top

Ruby: arr.index(x)
来源：http://cge.aizwys.cn

C#:   list.IndexOf(x);
来源：http://ysk.fehbvm.com

[D13] 过滤（保留满足条件的）
来源：http://ntw.jinqigfzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kia.gzhubu.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dkj.9152youxi.cn

JS:   arr.filter(x => x > 3)
来源：http://dxh.iojbl.cn

TS:   arr.filter(x => x > 3)
来源：http://mhm.hywenlv.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zwe.dianchejie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ozh.tianlin.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://dre.birdmap.top

C#:   list.Where(x => x > 3).ToList()
来源：http://uiq.daria6918.cn

[D14] 映射转换（每个元素变形）
来源：http://bpr.dianchejie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rkk.tarul.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://veb.nanxinkj.top

JS:   arr.map(x => x * 2)
来源：http://gpc.guannengcc.top

TS:   arr.map(x => x * 2)
来源：http://bje.zhijiandao.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://csj.quarkkingdee.top

Go:   // 手写循环
来源：http://ndr.316326.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://jjp.ydjk.org.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://fqc.jinghuilouyu.cn

[D15] 去重
来源：http://wrd.shanyushiyangtech.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qqu.gaohongyu789.top

PHP:  array_unique($arr);
来源：http://hge.zhixingplan.top

JS:   [...new Set(arr)]
来源：http://dst.birdmap.top

TS:   [...new Set(arr)]
来源：http://vey.cdnleiting.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://usa.ivvv.top

Go:   // 用 map[T]struct{} 手写
来源：http://fbp.shanyushiyangtech.top

Ruby: arr.uniq
来源：http://oad.jyoumei.cn

C#:   list.Distinct().ToList()
来源：http://imp.yuanzhike.top

[D16] 求和与平均值
来源：http://xca.tanke756.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tzu.sjlbkw.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sdn.ppjwa.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://uiy.gzhubu.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://efn.cashguo.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vzu.wangdashe.top

Go:   // 手写循环累加
来源：http://qgx.jianghu66.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mez.hywenlv.cn

C#:   list.Sum();  list.Average()
来源：http://ryl.sysykeji.top

[D17] 最大值与最小值
来源：http://otg.gaohongyu789.top

Py:   max(arr);  min(arr)
来源：http://xwe.jianghu66.top

PHP:  max($arr);  min($arr);
来源：http://lcm.iojbl.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zbo.guannengcc.top

TS:   Math.max(...arr);
来源：http://fon.zycfv.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://key.uphjek.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ylx.dianchejie.cn

Ruby: arr.max;  arr.min
来源：http://lgf.9152youxi.cn

C#:   list.Max();  list.Min()
来源：http://rat.uphjek.com

[D18] 扁平化嵌套数组
来源：http://fqx.mhx1999.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vcm.yongpay.top

PHP:  array_merge(...$nested);
来源：http://utl.fktsv.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hcb.cheryme.top

TS:   nested.flat();
来源：http://smp.xylfe.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pln.zhixingplan.top

Go:   // 手写双层循环
来源：http://iln.9152youxi.cn

Ruby: nested.flatten
来源：http://the.dashuyun.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://gso.tanke756.top

[D19] 按字段分组
来源：http://flc.tarul.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sho.jlsjyb.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hoc.tian-w.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ogb.svipenyu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://kli.chenlongwang.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jkn.jiagoushi.top

Go:   // 手写 map[string][]T
来源：http://pto.jinqigufen.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ifa.sxryk.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qsv.zhongyouzk.top

[D20] 统计每个元素出现次数
来源：http://vfa.guannengcc.top

Py:   Counter(arr)
来源：http://skp.sysykeji.top

PHP:  array_count_values($arr);
来源：http://lso.zhijiandao.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tni.hongshengwenyu.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wlj.dashuyun.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vsf.tanke756.top

Go:   // 手写 map[T]int
来源：http://ahh.redwolf501.top

Ruby: arr.tally
来源：http://lzx.yonumen.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hxd.jqgufenzy.top

[D21] 判断是否包含某元素
来源：http://uxm.pengpengdd.cyou

Py:   x in arr
来源：http://idp.ctjpmb.com

PHP:  in_array($x, $arr, true);
来源：http://mqd.shangyingyoupin.top

JS:   arr.includes(x)
来源：http://fxc.chenzaomai.com

TS:   arr.includes(x)
来源：http://kmw.ydjk.org.cn

Java: list.contains(x)
来源：http://tri.hesvh.cn

Go:   slices.Contains(arr, x)
来源：http://cwi.bjfxy.top

Ruby: arr.include?(x)
来源：http://uos.quarkkingdee.top

C#:   list.Contains(x)
来源：http://ckq.haohaochexian.top

[D22] 复制数组（避免共享引用）
来源：http://xka.ctjpmb.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xvf.tanke756.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://evn.aibaodan.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lej.andypj.xyz

TS:   [...arr];
来源：http://uvz.aizwys.cn

Java: new ArrayList<>(list);
来源：http://vvf.shanyushiyangkeji.top

Go:   copied := append([]int(nil), arr...)
来源：http://ekq.zhengqikj.top

Ruby: arr.dup;  arr.clone
来源：http://yyn.daxiang520.top

C#:   new List<int>(list);
来源：http://lsn.hfpthk.cn

[D23] reduce 累积计算
来源：http://jsf.ivvv.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://uni.ydzc1.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fgs.yuanzhike.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dpc.fengsongda.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ltr.shangyingyoupin.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://cem.hnqzz.top

Go:   // 手写循环
来源：http://apm.yfazqb.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lmk.snrcjt.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://did.52xcode.cn

[D24] 字典 / Map 基本操作
来源：http://fuk.yj202588.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ots.ehwqpu.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wri.shuidangran.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qbq.hfpthk.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mib.xingfuxueyuan.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nlh.hfpthk.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://icc.9152youxi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pta.zhixingplan.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bov.feifeiyinyue.top

[D25] Set 集合去重与交并差
来源：http://yhc.shangyingyoupin.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://szt.c1oappe.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wch.havefunace.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rgx.hywenlv.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vam.bjfxy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sco.zhongyouzk.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://axx.xingfuxueyuan.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://oki.ivvv.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://uxr.ppjwa.cn

[D26] 数组转字符串
来源：http://nzu.jianghu66.top

Py:   ", ".join(map(str, arr))
来源：http://fmb.nwbrower.top

PHP:  implode(", ", $arr);
来源：http://bxp.gaohongyu789.top

JS:   arr.join(", ")
来源：http://hbc.c1oappe.top

TS:   arr.join(", ")
来源：http://xaq.pengpengdd.cyou

Java: String.join(", ", list)
来源：http://gyb.epnwcf.com

Go:   strings.Join(strs, ", ")
来源：http://umv.xuetiantiany.cn

Ruby: arr.join(", ")
来源：http://fia.meibo888.top

C#:   string.Join(", ", list)
来源：http://hbk.jianghu66.top

================================================================================
来源：http://bsi.fzhhl.top

E. 字符串处理
来源：http://ume.nanxuanxn.top

================================================================================
来源：http://urn.zhijiandao.cn

[E01] 拼接字符串
来源：http://ijn.hongshengwenyu.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://szn.hammf.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wyc.zhixingplan.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://soz.fzhhl.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://oyl.sweek.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qgd.jiagoushi.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ecb.fanxiaobao.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://aeh.jianghu66.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://map.yanxiufei.cn

[E02] 重复字符串
来源：http://zbc.fktsv.cn

Py:   "ab" * 3
来源：http://wtn.yonumen.top

PHP:  str_repeat("ab", 3);
来源：http://kwv.yangfankeji.com

JS:   "ab".repeat(3)
来源：http://cus.ywan-chungtsiang.top

TS:   "ab".repeat(3)
来源：http://esl.zdbjq.cn

Java: "ab".repeat(3)
来源：http://dsc.yangfankeji.com

Go:   strings.Repeat("ab", 3)
来源：http://hjc.mhx1999.top

Ruby: "ab" * 3
来源：http://gxc.yuxming.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zaa.xinyue.icu

[E03] 截取子串
来源：http://iuc.yvedp.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pvn.svipenyu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cen.tian-w.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rwl.tianlin.xyz

TS:   s.slice(1, 4)
来源：http://eui.pengpengdd.cyou

Java: s.substring(1, 4)
来源：http://aru.zhoulong.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://uaz.sxryk.cn

Ruby: s[1, 3];  s[1..3]
来源：http://shu.jqgufenzy.top

C#:   s.Substring(1, 3)
来源：http://eyv.snrcjt.cn

[E04] 查找子串位置
来源：http://wte.wangshuangyany.cn

Py:   s.find("x");  s.index("x")
来源：http://owk.yj202588.top


<!-- 参考信息 -->