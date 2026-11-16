代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://xgu.sxryk.cn

C#:   using System.Text;
来源：http://utv.ehwqpu.com

[C12] 立即执行函数 IIFE
来源：http://bpn.guowangkeji.top

Py:   (lambda: print("run"))()
来源：http://tvd.zhoulong.xyz

PHP:  (function () { echo "run"; })();
来源：http://wei.snrcjt.cn

JS:   (() => { console.log("run"); })();
来源：http://cxx.hnqzz.top

TS:   (() => { console.log("run"); })();
来源：http://dwx.meibo888.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rxl.jinyuanbaomall.cn

Go:   func() { fmt.Println("run") }()
来源：http://qnl.chenzaomai.com

Ruby: -> { puts "run" }.call
来源：http://vjn.zhijiandao.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qlx.dianchejie.cn

[C13] 类型声明 / 类型注解
来源：http://znw.yanxiufei.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zwj.9152youxi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://guy.ivvv.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tyr.aizwys.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uby.hongshengwenyu.top

Java: int add(int a, int b) { return a + b; }
来源：http://znk.yvedp.cn

Go:   func add(a, b int) int
来源：http://mxc.xingfuxueyuan.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://euw.andypj.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://qda.pengpengdd.cyou

[C14] 泛型函数
来源：http://ozj.cqqwz.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ecm.316326.xyz

PHP:  // 无泛型
来源：http://huv.chenzaomai.com

JS:   // 无泛型
来源：http://wpp.redwolf501.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://myj.yj202588.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cfv.yueranfly.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://aji.ehwqpu.com

Ruby: # 无泛型
来源：http://nrk.ctjpmb.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ugo.xylfe.cn

[C15] 解构 / 展开参数
来源：http://yge.andypj.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fxm.ctjpmb.com

PHP:  [$a, $b] = $pair;
来源：http://hih.yongpay.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xxw.ydzc1.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vxd.tarul.cn

Java: // 无解构
来源：http://pod.yanxiufei.cn

Go:   // 无解构
来源：http://dxq.sjlbkw.cn

Ruby: a, b = pair
来源：http://ico.hywenlv.cn

C#:   var (a, b) = pair;
来源：http://ysr.shzxlz.cn

[C16] 函数 / 方法重载
来源：http://ukx.nanxuanxn.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://aqt.smart0.xyz

PHP:  // 无重载
来源：http://swy.ywan-chungtsiang.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ihu.shanyushiyangtech.top

TS:   // 用联合类型或重载签名声明
来源：http://tsm.nanxuanxn.top

Java: void f(int a) {}  void f(String a) {}
来源：http://vmm.ydjk.org.cn

Go:   // 无重载：用不同函数名
来源：http://ygb.nwbrower.top

Ruby: # 无重载：靠动态参数
来源：http://lod.yfazqb.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://dny.vqdsnc.cn

================================================================================
来源：http://adl.vqdsnc.cn

D. 数组 / 列表 / 集合
来源：http://gup.xinyue.icu

================================================================================
来源：http://shk.ybcxt.top

[D01] 创建数组 / 列表
来源：http://zow.uphjek.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://svd.wangdashe.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://obl.bjfxy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rvu.yongpay.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://qpq.gogol.net.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://oww.jinqigufen.top

Go:   arr := []int{1, 2, 3}
来源：http://vhs.yangfankeji.com

Ruby: arr = [1, 2, 3]
来源：http://uvo.quarkkingdee.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wkj.gogol.net.cn

[D02] 追加元素到末尾
来源：http://hhf.hfpthk.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://uvj.bjfxy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vzp.vehdjk.com

JS:   arr.push(4);
来源：http://qhm.zhixingplan.top

TS:   arr.push(4);
来源：http://fmg.tanke756.top

Java: list.add(4);
来源：http://hfd.wangshuangyany.cn

Go:   arr = append(arr, 4)
来源：http://ehr.hywenlv.cn

Ruby: arr << 4; arr.push(5)
来源：http://oed.yueranfly.top

C#:   list.Add(4);
来源：http://kti.bjfxy.top

[D03] 在指定位置插入元素
来源：http://zuh.gaohongyu789.top

Py:   arr.insert(0, 0)
来源：http://fya.ydzc1.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cvg.yonumen.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mbr.zhaomingkeji.xyz

TS:   arr.splice(0, 0, 0);
来源：http://mxt.havefunace.top

Java: list.add(0, 0);
来源：http://tci.gogol.net.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zbe.iojbl.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hzf.tarul.cn

C#:   list.Insert(0, 0);
来源：http://rxn.zhiwuduotai.top

[D04] 删除元素
来源：http://oqy.vqdsnc.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zon.hnqzz.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gdn.aizwys.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xrq.yonumen.top

TS:   arr.splice(0, 1);
来源：http://gvg.pycfn.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://crn.birdmap.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zpo.dashuyun.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mwe.sweek.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vzo.shangyingyoupin.top

[D05] 访问与修改元素
来源：http://hqu.aizwys.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://emt.sxryk.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vel.zhixingplan.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wxg.shanyushiyangtech.top

TS:   arr[0]; arr.at(-1);
来源：http://mgr.chenjidiqi.icu

Java: list.get(0); list.set(0, 9);
来源：http://bdg.hywenlv.cn

Go:   arr[0]; arr[0] = 9
来源：http://knx.bbcook.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vlj.jiagoushi.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://whr.ybcxt.top

[D06] 数组长度
来源：http://dlf.9152youxi.cn

Py:   len(arr)
来源：http://pni.chenjidiqi.icu

PHP:  count($arr);
来源：http://vcv.xuetiantiany.cn

JS:   arr.length
来源：http://gsc.ywan-chungtsiang.top

TS:   arr.length
来源：http://aeu.feifeiyinyue.top

Java: list.size();
来源：http://say.bjfxy.top

Go:   len(arr)
来源：http://geo.gogol.net.cn

Ruby: arr.length; arr.size
来源：http://ijc.gzhubu.top

C#:   list.Count;
来源：http://brw.ydjk.org.cn

[D07] 切片 / 取子数组
来源：http://zwe.sxryk.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nny.iojbl.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fyb.xingfuxueyuan.xyz

JS:   arr.slice(1, 4);
来源：http://ewm.yfazqb.com

TS:   arr.slice(1, 4);
来源：http://mhq.cheryme.top

Java: list.subList(1, 4);
来源：http://emt.aibaodan.cn

Go:   arr[1:4]
来源：http://nxw.fktsv.cn

Ruby: arr[1, 3]
来源：http://nii.vqdsnc.cn

C#:   list.GetRange(1, 3);
来源：http://vkz.shuidangran.top

[D08] 合并两个数组
来源：http://bjs.jinyuanbaomall.cn

Py:   a + b;  a.extend(b)
来源：http://vkq.cdnleiting.top

PHP:  array_merge($a, $b);
来源：http://gpk.haohaochexian.top

JS:   [...a, ...b];  a.concat(b);
来源：http://hqe.zhengqikj.top

TS:   [...a, ...b];
来源：http://ezr.ydzc1.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kxg.shanyushiyangkeji.top

Go:   append(a, b...)
来源：http://ysy.jianghu66.top

Ruby: a + b;  a.concat(b)
来源：http://zhn.hesvh.cn

C#:   a.Concat(b).ToList()
来源：http://osg.gogol.net.cn

[D09] 排序（升序）
来源：http://opa.vehdjk.com

Py:   sorted(arr);  arr.sort()
来源：http://uhh.xinyue.icu

PHP:  sort($arr);
来源：http://jdy.nanxinkj.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tol.tarul.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://eob.316326.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://gup.yuanzhike.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qvm.zhixingplan.top

Ruby: arr.sort
来源：http://vgn.havefunace.top

C#:   list.Sort();
来源：http://zgy.fehbvm.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://nnp.tianlin.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kfu.birdmap.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ziz.9152youxi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jpn.gzhubu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wnn.shangyingyoupin.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yrc.zhongyouzk.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wuz.nanxinkj.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://oyd.pengpengdd.cyou

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fia.daria6918.cn

[D11] 反转数组
来源：http://qbt.xuanzx.com

Py:   arr[::-1];  arr.reverse()
来源：http://ffl.jiagoushi.top

PHP:  array_reverse($arr);
来源：http://fts.cqqwz.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://obo.shuidangran.top

TS:   [...arr].reverse();
来源：http://gqn.316326.xyz

Java: Collections.reverse(list);
来源：http://bck.zhongyouzk.top

Go:   slices.Reverse(arr)
来源：http://lvi.ppjwa.cn

Ruby: arr.reverse
来源：http://rjg.mhx1999.top

C#:   list.Reverse();
来源：http://peg.cqqwz.cn

[D12] 查找元素下标
来源：http://oji.c1oappe.top

Py:   arr.index(x);  x in arr
来源：http://tsg.sufxvd.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://njg.hfpthk.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xmb.guowangkeji.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xrz.yj20258888.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vor.0kj1m.cn

Go:   slices.Index(arr, x)
来源：http://auo.sweek.top

Ruby: arr.index(x)
来源：http://sod.hysaishi.cn

C#:   list.IndexOf(x);
来源：http://xfw.ydjk.org.cn

[D13] 过滤（保留满足条件的）
来源：http://rvy.guowangkeji.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nho.nwbrower.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ozc.yanxiufei.cn

JS:   arr.filter(x => x > 3)
来源：http://llu.zycfv.cn

TS:   arr.filter(x => x > 3)
来源：http://ziu.jianghu66.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qyy.gogol.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://eea.smart0.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://nde.jinyuanbaomall.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://zgo.shangyingyoupin.top

[D14] 映射转换（每个元素变形）
来源：http://hlc.daria6918.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xds.ivvv.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://aot.zdbjq.cn

JS:   arr.map(x => x * 2)
来源：http://zcu.daria6918.cn

TS:   arr.map(x => x * 2)
来源：http://gbn.c1oappe.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://kow.jinghuilouyu.cn

Go:   // 手写循环
来源：http://fjl.iojbl.cn

Ruby: arr.map { |x| x * 2 }
来源：http://msc.gotoacloud.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ady.wangdashe.top

[D15] 去重
来源：http://zpf.316326.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kuv.zhaomingkeji.xyz

PHP:  array_unique($arr);
来源：http://oqj.kuanghao11.cn

JS:   [...new Set(arr)]
来源：http://ctm.vehdjk.com

TS:   [...new Set(arr)]
来源：http://phn.daria6918.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://djt.daxiang520.top

Go:   // 用 map[T]struct{} 手写
来源：http://upp.yfazqb.com

Ruby: arr.uniq
来源：http://fdw.yanxiufei.cn

C#:   list.Distinct().ToList()
来源：http://uoe.gaohongyu789.top

[D16] 求和与平均值
来源：http://arg.iojbl.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yml.316326.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wpm.c1oappe.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lsr.jlsjyb.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://eqn.yangfankeji.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nzt.zycfv.cn

Go:   // 手写循环累加
来源：http://eoc.nwbrower.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ime.fehbvm.com

C#:   list.Sum();  list.Average()
来源：http://fac.chenjidiqi.icu

[D17] 最大值与最小值
来源：http://rsk.jinqigfzy.top

Py:   max(arr);  min(arr)
来源：http://ahk.gaohongyu789.top

PHP:  max($arr);  min($arr);
来源：http://edj.iojbl.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ilv.tian-w.cn

TS:   Math.max(...arr);
来源：http://apt.hesvh.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bqp.zhixingplan.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dps.snrcjt.cn

Ruby: arr.max;  arr.min
来源：http://jjo.hnxiangtu.top

C#:   list.Max();  list.Min()
来源：http://dol.nanxuanxn.top

[D18] 扁平化嵌套数组
来源：http://vjv.gzhubu.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://egd.hcnkem.com

PHP:  array_merge(...$nested);
来源：http://gnu.jqgufenzy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://grx.yj202588.top

TS:   nested.flat();
来源：http://grd.jqgufenzy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nwg.cdnleiting.top

Go:   // 手写双层循环
来源：http://wht.zycfv.cn

Ruby: nested.flatten
来源：http://gzw.zdbjq.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://noa.zhixingplan.top

[D19] 按字段分组
来源：http://slg.pengpengdd.cyou

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vth.ctjpmb.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wsa.svipenyu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ayp.redwolf501.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://qkv.yueranfly.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bdd.guannengcc.top

Go:   // 手写 map[string][]T
来源：http://ofq.feifeiyinyue.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://bun.xuetiantiany.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fdb.chenjidiqi.icu

[D20] 统计每个元素出现次数
来源：http://ace.shanyushiyangkeji.top

Py:   Counter(arr)
来源：http://boa.yvedp.cn

PHP:  array_count_values($arr);
来源：http://paf.zdqjudy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xmk.sxryk.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://plf.cashguo.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cmn.sysykeji.top

Go:   // 手写 map[T]int
来源：http://ebz.hnxiangtu.top

Ruby: arr.tally
来源：http://qkd.iojbl.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://twe.mhx1999.top

[D21] 判断是否包含某元素
来源：http://mml.sweek.top

Py:   x in arr
来源：http://uqo.chenlongwang.top

PHP:  in_array($x, $arr, true);
来源：http://dsy.yuanzhike.top

JS:   arr.includes(x)
来源：http://amj.meibo888.top

TS:   arr.includes(x)
来源：http://bke.zhongyouzk.top

Java: list.contains(x)
来源：http://aoh.xuanzx.com

Go:   slices.Contains(arr, x)
来源：http://uwo.fanxiaobao.xyz

Ruby: arr.include?(x)
来源：http://zcc.chenjidiqi.icu

C#:   list.Contains(x)
来源：http://evs.quarkkingdee.top

[D22] 复制数组（避免共享引用）
来源：http://lzw.aibaodan.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dzi.yvedp.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cxn.chenlongwang.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rbc.hysaishi.cn

TS:   [...arr];
来源：http://wjt.yonumen.top

Java: new ArrayList<>(list);
来源：http://mvv.smart0.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://ybq.dianchejie.cn

Ruby: arr.dup;  arr.clone
来源：http://nul.cheryme.top

C#:   new List<int>(list);
来源：http://xoq.hongshengwenyu.top

[D23] reduce 累积计算
来源：http://xgz.hammf.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jei.yanxiufei.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gds.shzxlz.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://chc.hnqzz.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hyt.yvedp.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hpl.hesvh.cn

Go:   // 手写循环
来源：http://brg.cqqwz.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tun.tarul.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://esn.jinghuilouyu.cn

[D24] 字典 / Map 基本操作
来源：http://cra.ydjk.org.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jaz.zhaomingkeji.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ysc.shanyushiyangtech.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fgn.vehdjk.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wqz.sxryk.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://psf.meibo888.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pcs.guowangkeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ayj.fktsv.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rtv.yfazqb.com

[D25] Set 集合去重与交并差
来源：http://liw.sweek.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ori.9152youxi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yhp.zhongyouzk.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://piz.feifeiyinyue.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jmd.uphjek.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wmt.ehwqpu.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hnu.fzhhl.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pvi.wangshuangyany.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xyx.zdbjq.cn

[D26] 数组转字符串
来源：http://tkw.iojbl.cn

Py:   ", ".join(map(str, arr))
来源：http://qwz.cashguo.top

PHP:  implode(", ", $arr);
来源：http://sht.pengpengdd.cyou

JS:   arr.join(", ")
来源：http://vfo.gzhubu.top

TS:   arr.join(", ")
来源：http://dge.jianghu66.top

Java: String.join(", ", list)
来源：http://jey.316326.xyz

Go:   strings.Join(strs, ", ")
来源：http://ibd.svipenyu.cn

Ruby: arr.join(", ")
来源：http://jvz.dashuyun.cn

C#:   string.Join(", ", list)
来源：http://ebi.zhengqikj.top

================================================================================
来源：http://pti.aizwys.cn

E. 字符串处理
来源：http://fkq.316326.xyz

================================================================================
来源：http://qct.zhoulong.xyz

[E01] 拼接字符串
来源：http://sbq.redwolf501.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nwt.jqgfzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zyg.aibaodan.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jsl.yanxiufei.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bxe.ivvv.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://phs.uphjek.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wrv.nanxinkj.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tex.ydzc1.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://oax.haohaochexian.top

[E02] 重复字符串
来源：http://don.sufxvd.cn

Py:   "ab" * 3
来源：http://xsc.9152youxi.cn

PHP:  str_repeat("ab", 3);
来源：http://zje.pengpengdd.cyou

JS:   "ab".repeat(3)
来源：http://mcq.fengsongda.top


<!-- 参考信息 -->