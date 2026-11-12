代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://sxz.jiagoushi.top

JS:   (() => { console.log("run"); })();
来源：http://xlo.jinghuilouyu.cn

TS:   (() => { console.log("run"); })();
来源：http://vzk.0kj1m.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dxa.jqgufenzy.top

Go:   func() { fmt.Println("run") }()
来源：http://ypj.nanxuanxn.top

Ruby: -> { puts "run" }.call
来源：http://ujv.smart0.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://sar.ywan-chungtsiang.top

[C13] 类型声明 / 类型注解
来源：http://qga.hysaishi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cxp.hesvh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sxr.xinyue.icu

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hlx.snrcjt.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xty.yj20258888.top

Java: int add(int a, int b) { return a + b; }
来源：http://dpq.yueranfly.top

Go:   func add(a, b int) int
来源：http://zuw.fengsongda.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gmf.yuanzhike.top

C#:   int Add(int a, int b) => a + b;
来源：http://dvh.snrcjt.cn

[C14] 泛型函数
来源：http://vbs.xylfe.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bwz.wangdashe.top

PHP:  // 无泛型
来源：http://jva.nwbrower.top

JS:   // 无泛型
来源：http://ikq.cheryme.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kaa.zhijiandao.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fiq.zhoulong.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ybu.mhx1999.top

Ruby: # 无泛型
来源：http://oar.cashguo.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ksh.jqgufenzy.top

[C15] 解构 / 展开参数
来源：http://vao.zhengqikj.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rms.fktsv.cn

PHP:  [$a, $b] = $pair;
来源：http://tyb.zhixingplan.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lao.sysykeji.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yyi.gaohongyu789.top

Java: // 无解构
来源：http://hiy.vehdjk.com

Go:   // 无解构
来源：http://dun.cdnleiting.top

Ruby: a, b = pair
来源：http://dkc.yj202588.top

C#:   var (a, b) = pair;
来源：http://ghc.jinqigufen.top

[C16] 函数 / 方法重载
来源：http://uau.pengpengdd.cyou

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hmx.zhongyouzk.top

PHP:  // 无重载
来源：http://pub.cucudq.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bvi.nanxuanxn.top

TS:   // 用联合类型或重载签名声明
来源：http://rbn.fktsv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rlt.sufxvd.cn

Go:   // 无重载：用不同函数名
来源：http://oxf.gzhubu.top

Ruby: # 无重载：靠动态参数
来源：http://jtw.ybcxt.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://jil.kuanghao11.cn

================================================================================
来源：http://ftu.redwolf501.top

D. 数组 / 列表 / 集合
来源：http://bga.hnxiangtu.top

================================================================================
来源：http://xca.jyoumei.cn

[D01] 创建数组 / 列表
来源：http://vmh.xuanzx.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://dne.yueranfly.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fue.jlsjyb.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://swl.gotoacloud.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://egs.zhaomingkeji.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qgk.yj20258.top

Go:   arr := []int{1, 2, 3}
来源：http://vdo.uphjek.com

Ruby: arr = [1, 2, 3]
来源：http://abe.epnwcf.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://spm.zhixingplan.top

[D02] 追加元素到末尾
来源：http://oeu.jqgufenzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xxo.xylfe.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sqo.cheryme.top

JS:   arr.push(4);
来源：http://bsu.quarkkingdee.top

TS:   arr.push(4);
来源：http://tva.bbcook.cn

Java: list.add(4);
来源：http://zcu.vqdsnc.cn

Go:   arr = append(arr, 4)
来源：http://tyl.cdnleiting.top

Ruby: arr << 4; arr.push(5)
来源：http://dxc.hongshengwenyu.top

C#:   list.Add(4);
来源：http://snt.aibaodan.cn

[D03] 在指定位置插入元素
来源：http://ynl.jianghu66.top

Py:   arr.insert(0, 0)
来源：http://fqt.mhx1999.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ade.shzxlz.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xzj.guowangkeji.top

TS:   arr.splice(0, 0, 0);
来源：http://thn.fehbvm.com

Java: list.add(0, 0);
来源：http://koq.cqqwz.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ysk.gzhubu.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yjq.tianlin.xyz

C#:   list.Insert(0, 0);
来源：http://qld.hysaishi.cn

[D04] 删除元素
来源：http://rch.xylfe.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mmw.snrcjt.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wbu.hfpthk.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://asf.quarkkingdee.top

TS:   arr.splice(0, 1);
来源：http://sdu.ydzc1.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gif.vehdjk.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ltu.gaohongyu789.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rxl.nwbrower.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vsx.hysaishi.cn

[D05] 访问与修改元素
来源：http://ovv.xylfe.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hqg.52xcode.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://krm.zhijiandao.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jcn.yongpay.top

TS:   arr[0]; arr.at(-1);
来源：http://ooc.fktsv.cn

Java: list.get(0); list.set(0, 9);
来源：http://eks.xuetiantiany.cn

Go:   arr[0]; arr[0] = 9
来源：http://gku.zhijiandao.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mow.shzxlz.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yat.shangyingyoupin.top

[D06] 数组长度
来源：http://cub.svipenyu.cn

Py:   len(arr)
来源：http://okk.chenlongwang.top

PHP:  count($arr);
来源：http://jap.yueranfly.top

JS:   arr.length
来源：http://rat.tanke756.top

TS:   arr.length
来源：http://rsn.hesvh.cn

Java: list.size();
来源：http://wcx.yangfankeji.com

Go:   len(arr)
来源：http://upf.tanke756.top

Ruby: arr.length; arr.size
来源：http://dsd.shanyushiyangtech.top

C#:   list.Count;
来源：http://yro.jlsjyb.cn

[D07] 切片 / 取子数组
来源：http://ibq.bjfxy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://uas.gaohongyu789.top

PHP:  array_slice($arr, 1, 3);
来源：http://omw.wangdashe.top

JS:   arr.slice(1, 4);
来源：http://ixv.cqqwz.cn

TS:   arr.slice(1, 4);
来源：http://ngp.ydjk.org.cn

Java: list.subList(1, 4);
来源：http://aac.fanxiaobao.xyz

Go:   arr[1:4]
来源：http://wop.shanyushiyangkeji.top

Ruby: arr[1, 3]
来源：http://srb.cqqwz.cn

C#:   list.GetRange(1, 3);
来源：http://vex.gaohongyu789.top

[D08] 合并两个数组
来源：http://ona.hnxiangtu.top

Py:   a + b;  a.extend(b)
来源：http://ehs.wangshuangyany.cn

PHP:  array_merge($a, $b);
来源：http://zfu.yfazqb.com

JS:   [...a, ...b];  a.concat(b);
来源：http://emf.sxryk.cn

TS:   [...a, ...b];
来源：http://wpw.chenjidiqi.icu

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ehj.xuanzx.com

Go:   append(a, b...)
来源：http://cdb.gotoacloud.top

Ruby: a + b;  a.concat(b)
来源：http://crw.zhengqikj.top

C#:   a.Concat(b).ToList()
来源：http://mgd.yonumen.top

[D09] 排序（升序）
来源：http://ncg.sufxvd.cn

Py:   sorted(arr);  arr.sort()
来源：http://epp.zhijiandao.cn

PHP:  sort($arr);
来源：http://cyk.xylfe.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mef.dashuyun.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ehn.fktsv.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://gxl.wangshuangyany.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xyq.guowangkeji.top

Ruby: arr.sort
来源：http://xek.xingfuxueyuan.xyz

C#:   list.Sort();
来源：http://gpr.xylfe.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mvo.tanke756.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lup.andypj.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sjy.wangshuangyany.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ivv.zhoulong.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cfn.ppjwa.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lcb.birdmap.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qkw.hywenlv.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ado.redwolf501.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ucc.zycfv.cn

[D11] 反转数组
来源：http://joc.gzhubu.top

Py:   arr[::-1];  arr.reverse()
来源：http://ikn.xuanzx.com

PHP:  array_reverse($arr);
来源：http://sen.redwolf501.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://eek.jinghuilouyu.cn

TS:   [...arr].reverse();
来源：http://bnd.xylfe.cn

Java: Collections.reverse(list);
来源：http://zjt.shangyingyoupin.top

Go:   slices.Reverse(arr)
来源：http://ezr.shangyingyoupin.top

Ruby: arr.reverse
来源：http://urw.hongshengwenyu.top

C#:   list.Reverse();
来源：http://jcx.zhaomingkeji.xyz

[D12] 查找元素下标
来源：http://jxo.nwbrower.top

Py:   arr.index(x);  x in arr
来源：http://fgl.zhaomingkeji.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nmw.yangfankeji.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rmo.jiagoushi.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rsc.hammf.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sol.jlsjyb.cn

Go:   slices.Index(arr, x)
来源：http://gzb.zhiwuduotai.top

Ruby: arr.index(x)
来源：http://upw.fehbvm.com

C#:   list.IndexOf(x);
来源：http://rjs.shanyushiyangtech.top

[D13] 过滤（保留满足条件的）
来源：http://yqy.aibaodan.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nft.pycfn.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ghp.jinqigfzy.top

JS:   arr.filter(x => x > 3)
来源：http://hmq.daxiang520.top

TS:   arr.filter(x => x > 3)
来源：http://yim.sjlbkw.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kjx.shzxlz.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vlk.xuanzx.com

Ruby: arr.select { |x| x > 3 }
来源：http://gfm.yongpay.top

C#:   list.Where(x => x > 3).ToList()
来源：http://hyt.hnxiangtu.top

[D14] 映射转换（每个元素变形）
来源：http://cvq.jinqigfzy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://crl.zhijiandao.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://aqi.aizwys.cn

JS:   arr.map(x => x * 2)
来源：http://bzo.hcnkem.com

TS:   arr.map(x => x * 2)
来源：http://hpa.yonumen.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ach.hywenlv.cn

Go:   // 手写循环
来源：http://gxa.yuxming.cn

Ruby: arr.map { |x| x * 2 }
来源：http://phn.daria6918.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xvm.yfazqb.com

[D15] 去重
来源：http://kgh.ybcxt.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bgs.hysaishi.cn

PHP:  array_unique($arr);
来源：http://jeb.pengpengdd.cyou

JS:   [...new Set(arr)]
来源：http://mjg.yonumen.top

TS:   [...new Set(arr)]
来源：http://qto.chenlongwang.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xyf.yj20258.top

Go:   // 用 map[T]struct{} 手写
来源：http://pny.smart0.xyz

Ruby: arr.uniq
来源：http://wym.0kj1m.cn

C#:   list.Distinct().ToList()
来源：http://lcx.pengpengdd.cyou

[D16] 求和与平均值
来源：http://rvz.wangdashe.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hny.mhx1999.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dhb.ehwqpu.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://whp.smart0.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bnk.gzhubu.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xra.gogol.net.cn

Go:   // 手写循环累加
来源：http://jji.vqdsnc.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://guh.52xcode.cn

C#:   list.Sum();  list.Average()
来源：http://iyh.sysykeji.top

[D17] 最大值与最小值
来源：http://huf.yj20258.top

Py:   max(arr);  min(arr)
来源：http://snm.cashguo.top

PHP:  max($arr);  min($arr);
来源：http://qst.zhiwuduotai.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fjb.bjfxy.top

TS:   Math.max(...arr);
来源：http://rcg.epnwcf.com

Java: Collections.max(list);  Collections.min(list);
来源：http://uht.vqdsnc.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mmz.zhengqikj.top

Ruby: arr.max;  arr.min
来源：http://kyx.guannengcc.top

C#:   list.Max();  list.Min()
来源：http://jbn.xylfe.cn

[D18] 扁平化嵌套数组
来源：http://rez.gogol.net.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kpt.wangdashe.top

PHP:  array_merge(...$nested);
来源：http://vpy.tianlin.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pft.smart0.xyz

TS:   nested.flat();
来源：http://wab.cheryme.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://smz.chenlongwang.top

Go:   // 手写双层循环
来源：http://gue.fzhhl.top

Ruby: nested.flatten
来源：http://wjh.aizwys.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://raq.xingfuxueyuan.xyz

[D19] 按字段分组
来源：http://yxa.shanyushiyangkeji.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://urg.shuidangran.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bqd.fktsv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tds.jianghu66.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ucw.zhaomingkeji.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ypj.yuxming.cn

Go:   // 手写 map[string][]T
来源：http://afi.yvedp.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jpj.yj20258.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://oia.zycfv.cn

[D20] 统计每个元素出现次数
来源：http://oqy.xziqi.cn

Py:   Counter(arr)
来源：http://dzy.jlsjyb.cn

PHP:  array_count_values($arr);
来源：http://hox.cucudq.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wkm.ydzc1.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jqx.yvedp.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://liv.fktsv.cn

Go:   // 手写 map[T]int
来源：http://wid.ybcxt.top

Ruby: arr.tally
来源：http://did.ydzc1.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wkc.hongshengwenyu.top

[D21] 判断是否包含某元素
来源：http://ffs.fehbvm.com

Py:   x in arr
来源：http://ntg.pengpengdd.cyou

PHP:  in_array($x, $arr, true);
来源：http://luw.gotoacloud.top

JS:   arr.includes(x)
来源：http://dmr.shangyingyoupin.top

TS:   arr.includes(x)
来源：http://kwq.sysykeji.top

Java: list.contains(x)
来源：http://npb.0kj1m.cn

Go:   slices.Contains(arr, x)
来源：http://uid.yuanzhike.top

Ruby: arr.include?(x)
来源：http://tuh.mhx1999.top

C#:   list.Contains(x)
来源：http://rdx.dashuyun.cn

[D22] 复制数组（避免共享引用）
来源：http://hhp.wangdashe.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://axl.ydzc1.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tdn.fehbvm.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nul.hnxiangtu.top

TS:   [...arr];
来源：http://bqr.ctjpmb.com

Java: new ArrayList<>(list);
来源：http://epc.hesvh.cn

Go:   copied := append([]int(nil), arr...)
来源：http://csr.gaohongyu789.top

Ruby: arr.dup;  arr.clone
来源：http://myg.jiagoushi.top

C#:   new List<int>(list);
来源：http://yjo.cqqwz.cn

[D23] reduce 累积计算
来源：http://fpa.cheryme.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dgn.yueranfly.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://izo.aibaodan.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iln.fehbvm.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kas.yj20258888.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://szi.mhx1999.top

Go:   // 手写循环
来源：http://esd.andypj.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dsd.yanxiufei.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xeb.hammf.cn

[D24] 字典 / Map 基本操作
来源：http://xyd.dashuyun.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://abn.zycfv.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nfo.sxryk.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sdf.jqgfzy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xen.zhixingplan.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://oow.haohaochexian.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kmg.hfpthk.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://son.gotoacloud.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://exe.xylfe.cn

[D25] Set 集合去重与交并差
来源：http://llf.jiagoushi.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lea.yuanzhike.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hzf.yueranfly.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gnc.hongshengwenyu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mes.zhijiandao.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ywr.jyoumei.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sew.dashuyun.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fdt.sweek.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://que.xingfuxueyuan.xyz

[D26] 数组转字符串
来源：http://uhf.yonumen.top

Py:   ", ".join(map(str, arr))
来源：http://tto.zhiwuduotai.top

PHP:  implode(", ", $arr);
来源：http://oyt.feifeiyinyue.top

JS:   arr.join(", ")
来源：http://hlx.xuanzx.com

TS:   arr.join(", ")
来源：http://rry.shuidangran.top

Java: String.join(", ", list)
来源：http://koh.aizwys.cn

Go:   strings.Join(strs, ", ")
来源：http://wlq.nanxinkj.top

Ruby: arr.join(", ")
来源：http://qqf.yonumen.top

C#:   string.Join(", ", list)
来源：http://rur.zhongyouzk.top

================================================================================
来源：http://hki.yvedp.cn

E. 字符串处理
来源：http://fgu.vehdjk.com

================================================================================
来源：http://srt.zhixingplan.top

[E01] 拼接字符串
来源：http://zaj.yangfankeji.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tjc.ivvv.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bwr.chenlongwang.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://onw.hnqzz.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zha.andypj.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hkj.yj20258.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wxm.aibaodan.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://uaa.gaohongyu789.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kcl.cashguo.top

[E02] 重复字符串
来源：http://kto.chenjidiqi.icu

Py:   "ab" * 3
来源：http://ixm.zhaomingkeji.xyz

PHP:  str_repeat("ab", 3);
来源：http://chc.uphjek.com

JS:   "ab".repeat(3)
来源：http://vis.hfpthk.cn

TS:   "ab".repeat(3)
来源：http://dos.zhoulong.xyz

Java: "ab".repeat(3)
来源：http://kfm.zhengqikj.top

Go:   strings.Repeat("ab", 3)
来源：http://tte.hnxiangtu.top

Ruby: "ab" * 3
来源：http://fma.zycfv.cn


<!-- 参考信息 -->