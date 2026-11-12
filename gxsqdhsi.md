代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://gyr.cqqwz.cn

JS:   (() => { console.log("run"); })();
来源：http://rfs.andypj.xyz

TS:   (() => { console.log("run"); })();
来源：http://gfj.svipenyu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xha.jianghu66.top

Go:   func() { fmt.Println("run") }()
来源：http://awf.316326.xyz

Ruby: -> { puts "run" }.call
来源：http://ukz.fanxiaobao.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://saa.hammf.cn

[C13] 类型声明 / 类型注解
来源：http://ive.yj20258888.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kpt.tarul.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gug.hfpthk.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ujb.hysaishi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bzp.zdbjq.cn

Java: int add(int a, int b) { return a + b; }
来源：http://saj.aizwys.cn

Go:   func add(a, b int) int
来源：http://vxv.daxiang520.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wex.aizwys.cn

C#:   int Add(int a, int b) => a + b;
来源：http://clv.wangdashe.top

[C14] 泛型函数
来源：http://vxd.zhiwuduotai.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bee.fktsv.cn

PHP:  // 无泛型
来源：http://jaq.nanxuanxn.top

JS:   // 无泛型
来源：http://vts.cashguo.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kwz.bjfxy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://upd.epnwcf.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://myz.zhiwuduotai.top

Ruby: # 无泛型
来源：http://kbp.dashuyun.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://agz.chenlongwang.top

[C15] 解构 / 展开参数
来源：http://bac.ydzc1.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kpa.wangdashe.top

PHP:  [$a, $b] = $pair;
来源：http://sys.yvedp.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://igm.fengsongda.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fcw.yj20258.top

Java: // 无解构
来源：http://fic.kuanghao11.cn

Go:   // 无解构
来源：http://ndm.9152youxi.cn

Ruby: a, b = pair
来源：http://ycv.smart0.xyz

C#:   var (a, b) = pair;
来源：http://hij.yj20258888.top

[C16] 函数 / 方法重载
来源：http://qvi.wangshuangyany.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xhu.pengpengdd.cyou

PHP:  // 无重载
来源：http://wba.wangdashe.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://abd.havefunace.top

TS:   // 用联合类型或重载签名声明
来源：http://agi.hfpthk.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://lmi.yangfankeji.com

Go:   // 无重载：用不同函数名
来源：http://afi.jqgufenzy.top

Ruby: # 无重载：靠动态参数
来源：http://bnq.xuetiantiany.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ngt.gogol.net.cn

================================================================================
来源：http://qjh.zhoulong.xyz

D. 数组 / 列表 / 集合
来源：http://pdd.jiagoushi.top

================================================================================
来源：http://azs.chenlongwang.top

[D01] 创建数组 / 列表
来源：http://hnl.hesvh.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ooa.xylfe.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://prk.sufxvd.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qcs.sufxvd.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xrl.cheryme.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bpy.ehwqpu.com

Go:   arr := []int{1, 2, 3}
来源：http://egy.zhixingplan.top

Ruby: arr = [1, 2, 3]
来源：http://eil.shangyingyoupin.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fqi.sysykeji.top

[D02] 追加元素到末尾
来源：http://bnn.guannengcc.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jyo.nanxinkj.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xob.shuidangran.top

JS:   arr.push(4);
来源：http://lnh.cqqwz.cn

TS:   arr.push(4);
来源：http://uhc.svipenyu.cn

Java: list.add(4);
来源：http://lkc.zhaomingkeji.xyz

Go:   arr = append(arr, 4)
来源：http://juy.meibo888.top

Ruby: arr << 4; arr.push(5)
来源：http://exq.aizwys.cn

C#:   list.Add(4);
来源：http://egl.cucudq.cn

[D03] 在指定位置插入元素
来源：http://hmn.yanxiufei.cn

Py:   arr.insert(0, 0)
来源：http://qqn.jqgfzy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mos.nanxinkj.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ngn.ydzc1.top

TS:   arr.splice(0, 0, 0);
来源：http://dei.tian-w.cn

Java: list.add(0, 0);
来源：http://ubo.havefunace.top

Go:   arr = append([]int{0}, arr...)
来源：http://mhp.yongpay.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://anf.havefunace.top

C#:   list.Insert(0, 0);
来源：http://qea.ppjwa.cn

[D04] 删除元素
来源：http://msw.ybcxt.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fdd.hongshengwenyu.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sfb.zhixingplan.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mtv.guannengcc.top

TS:   arr.splice(0, 1);
来源：http://ygh.dashuyun.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fcs.xylfe.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xgb.daria6918.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jxa.vehdjk.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nmd.wangshuangyany.cn

[D05] 访问与修改元素
来源：http://suu.chenlongwang.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bpr.fehbvm.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://epg.9152youxi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tqn.9152youxi.cn

TS:   arr[0]; arr.at(-1);
来源：http://wji.nanxinkj.top

Java: list.get(0); list.set(0, 9);
来源：http://dzy.tarul.cn

Go:   arr[0]; arr[0] = 9
来源：http://xgd.jiagoushi.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wyq.fzhhl.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fuf.hesvh.cn

[D06] 数组长度
来源：http://ecj.ppjwa.cn

Py:   len(arr)
来源：http://zme.svipenyu.cn

PHP:  count($arr);
来源：http://lms.jyoumei.cn

JS:   arr.length
来源：http://cao.jinghuilouyu.cn

TS:   arr.length
来源：http://zuy.iojbl.cn

Java: list.size();
来源：http://twm.zhiwuduotai.top

Go:   len(arr)
来源：http://lts.sweek.top

Ruby: arr.length; arr.size
来源：http://hbq.nanxuanxn.top

C#:   list.Count;
来源：http://crg.yj20258.top

[D07] 切片 / 取子数组
来源：http://mmd.ctjpmb.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ttl.gogol.net.cn

PHP:  array_slice($arr, 1, 3);
来源：http://mak.ctjpmb.com

JS:   arr.slice(1, 4);
来源：http://oec.shanyushiyangkeji.top

TS:   arr.slice(1, 4);
来源：http://srw.cashguo.top

Java: list.subList(1, 4);
来源：http://uka.jinyuanbaomall.cn

Go:   arr[1:4]
来源：http://ukg.tarul.cn

Ruby: arr[1, 3]
来源：http://dzu.yonumen.top

C#:   list.GetRange(1, 3);
来源：http://gsx.zhijiandao.cn

[D08] 合并两个数组
来源：http://iek.sufxvd.cn

Py:   a + b;  a.extend(b)
来源：http://qye.gzhubu.top

PHP:  array_merge($a, $b);
来源：http://bhj.yj202588.top

JS:   [...a, ...b];  a.concat(b);
来源：http://rpj.yj20258.top

TS:   [...a, ...b];
来源：http://uht.gaohongyu789.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ffc.redwolf501.top

Go:   append(a, b...)
来源：http://gmm.fehbvm.com

Ruby: a + b;  a.concat(b)
来源：http://cug.tanke756.top

C#:   a.Concat(b).ToList()
来源：http://oay.sxryk.cn

[D09] 排序（升序）
来源：http://cat.hnxiangtu.top

Py:   sorted(arr);  arr.sort()
来源：http://lzh.cheryme.top

PHP:  sort($arr);
来源：http://wiy.cqqwz.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rzy.bbcook.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://udx.cdnleiting.top

Java: Collections.sort(list);  list.sort(null);
来源：http://tzj.yuxming.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nuv.c1oappe.top

Ruby: arr.sort
来源：http://aar.xuetiantiany.cn

C#:   list.Sort();
来源：http://pka.meibo888.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ire.hywenlv.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pnw.chenjidiqi.icu

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dwr.zhijiandao.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nps.shanyushiyangtech.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fys.svipenyu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zdy.chenzaomai.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uwe.zhaomingkeji.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mvm.shangyingyoupin.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pbo.zhongyouzk.top

[D11] 反转数组
来源：http://tef.ybcxt.top

Py:   arr[::-1];  arr.reverse()
来源：http://ufu.yanxiufei.cn

PHP:  array_reverse($arr);
来源：http://sig.xylfe.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://flh.ehwqpu.com

TS:   [...arr].reverse();
来源：http://hfa.zdbjq.cn

Java: Collections.reverse(list);
来源：http://lbx.nanxinkj.top

Go:   slices.Reverse(arr)
来源：http://jbt.sweek.top

Ruby: arr.reverse
来源：http://gig.sufxvd.cn

C#:   list.Reverse();
来源：http://jnu.shangyingyoupin.top

[D12] 查找元素下标
来源：http://dzy.hnxiangtu.top

Py:   arr.index(x);  x in arr
来源：http://xrg.ywan-chungtsiang.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mwq.wangdashe.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vgk.fktsv.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ocf.hesvh.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nkn.jinghuilouyu.cn

Go:   slices.Index(arr, x)
来源：http://fzj.fengsongda.top

Ruby: arr.index(x)
来源：http://uap.cheryme.top

C#:   list.IndexOf(x);
来源：http://lsb.yuanzhike.top

[D13] 过滤（保留满足条件的）
来源：http://vkt.jinyuanbaomall.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sku.fanxiaobao.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ohf.yvedp.cn

JS:   arr.filter(x => x > 3)
来源：http://rhn.yj20258.top

TS:   arr.filter(x => x > 3)
来源：http://rig.tianlin.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ibj.yvedp.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://svi.nwbrower.top

Ruby: arr.select { |x| x > 3 }
来源：http://lis.meibo888.top

C#:   list.Where(x => x > 3).ToList()
来源：http://zej.fanxiaobao.xyz

[D14] 映射转换（每个元素变形）
来源：http://tmu.ydzc1.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://era.hammf.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dqq.yueranfly.top

JS:   arr.map(x => x * 2)
来源：http://ybt.fehbvm.com

TS:   arr.map(x => x * 2)
来源：http://jll.shangyingyoupin.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://aea.cdnleiting.top

Go:   // 手写循环
来源：http://aad.andypj.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://hyr.yvedp.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://sbt.cqqwz.cn

[D15] 去重
来源：http://quc.ehwqpu.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yej.tarul.cn

PHP:  array_unique($arr);
来源：http://rkk.vehdjk.com

JS:   [...new Set(arr)]
来源：http://vux.jqgfzy.top

TS:   [...new Set(arr)]
来源：http://jxo.zhaomingkeji.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ukh.gotoacloud.top

Go:   // 用 map[T]struct{} 手写
来源：http://vup.gzhubu.top

Ruby: arr.uniq
来源：http://znw.chenzaomai.com

C#:   list.Distinct().ToList()
来源：http://gly.daria6918.cn

[D16] 求和与平均值
来源：http://ouf.redwolf501.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fvz.jinqigfzy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vwk.sxryk.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zfv.uphjek.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dvp.vehdjk.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ofo.shzxlz.cn

Go:   // 手写循环累加
来源：http://mal.yangfankeji.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://iyx.chenzaomai.com

C#:   list.Sum();  list.Average()
来源：http://ild.fengsongda.top

[D17] 最大值与最小值
来源：http://yme.xuanzx.com

Py:   max(arr);  min(arr)
来源：http://kno.sysykeji.top

PHP:  max($arr);  min($arr);
来源：http://pyj.epnwcf.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mve.birdmap.top

TS:   Math.max(...arr);
来源：http://teg.chenlongwang.top

Java: Collections.max(list);  Collections.min(list);
来源：http://nuh.epnwcf.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jgz.yongpay.top

Ruby: arr.max;  arr.min
来源：http://zib.zycfv.cn

C#:   list.Max();  list.Min()
来源：http://mzs.tanke756.top

[D18] 扁平化嵌套数组
来源：http://chy.zhijiandao.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kfy.yueranfly.top

PHP:  array_merge(...$nested);
来源：http://jtj.nanxuanxn.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://soh.zdqjudy.top

TS:   nested.flat();
来源：http://zrp.xziqi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rts.zdqjudy.top

Go:   // 手写双层循环
来源：http://nhs.fktsv.cn

Ruby: nested.flatten
来源：http://jqg.hesvh.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://tpi.yongpay.top

[D19] 按字段分组
来源：http://lqh.kuanghao11.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dhd.sxryk.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ypz.jinyuanbaomall.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lgw.sxryk.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://dlx.aizwys.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ucw.ehwqpu.com

Go:   // 手写 map[string][]T
来源：http://xsk.ybcxt.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://spr.xuetiantiany.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lvo.hnqzz.top

[D20] 统计每个元素出现次数
来源：http://zbc.hywenlv.cn

Py:   Counter(arr)
来源：http://mqx.yangfankeji.com

PHP:  array_count_values($arr);
来源：http://geg.jinqigufen.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ezc.52xcode.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qie.hongshengwenyu.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://phs.shzxlz.cn

Go:   // 手写 map[T]int
来源：http://qtw.gaohongyu789.top

Ruby: arr.tally
来源：http://spw.aibaodan.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kus.xylfe.cn

[D21] 判断是否包含某元素
来源：http://bgp.yj20258.top

Py:   x in arr
来源：http://apt.dianchejie.cn

PHP:  in_array($x, $arr, true);
来源：http://izt.daxiang520.top

JS:   arr.includes(x)
来源：http://met.hongshengwenyu.top

TS:   arr.includes(x)
来源：http://eiz.yfazqb.com

Java: list.contains(x)
来源：http://uaa.gotoacloud.top

Go:   slices.Contains(arr, x)
来源：http://lla.feifeiyinyue.top

Ruby: arr.include?(x)
来源：http://etj.zycfv.cn

C#:   list.Contains(x)
来源：http://yjb.yvedp.cn

[D22] 复制数组（避免共享引用）
来源：http://zvo.svipenyu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://paa.cheryme.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cdv.cdnleiting.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uqk.ywan-chungtsiang.top

TS:   [...arr];
来源：http://hwm.xingfuxueyuan.xyz

Java: new ArrayList<>(list);
来源：http://qzl.hammf.cn

Go:   copied := append([]int(nil), arr...)
来源：http://siw.feifeiyinyue.top

Ruby: arr.dup;  arr.clone
来源：http://svo.pycfn.com

C#:   new List<int>(list);
来源：http://xxh.pycfn.com

[D23] reduce 累积计算
来源：http://tfn.cheryme.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://toq.zhiwuduotai.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vun.sjlbkw.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tty.gzhubu.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lmp.sjlbkw.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qfi.hongshengwenyu.top

Go:   // 手写循环
来源：http://ogs.yanxiufei.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://oxo.zdbjq.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uax.epnwcf.com

[D24] 字典 / Map 基本操作
来源：http://kak.hongshengwenyu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xsg.zhoulong.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dpx.aibaodan.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://agk.fzhhl.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://uhf.fzhhl.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://swn.hcnkem.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rok.gzhubu.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rnw.ybcxt.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vby.snrcjt.cn

[D25] Set 集合去重与交并差
来源：http://ttb.zdqjudy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://uvh.cheryme.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nmj.gaohongyu789.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rnt.daria6918.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rak.fzhhl.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://igq.zhongyouzk.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kam.jianghu66.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://llr.daria6918.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kij.sxryk.cn

[D26] 数组转字符串
来源：http://ddz.yvedp.cn

Py:   ", ".join(map(str, arr))
来源：http://mbk.zhixingplan.top

PHP:  implode(", ", $arr);
来源：http://qtf.jinghuilouyu.cn

JS:   arr.join(", ")
来源：http://gua.zhongyouzk.top

TS:   arr.join(", ")
来源：http://fkc.zdqjudy.top

Java: String.join(", ", list)
来源：http://xvd.yvedp.cn

Go:   strings.Join(strs, ", ")
来源：http://pvr.cashguo.top

Ruby: arr.join(", ")
来源：http://kiy.jlsjyb.cn

C#:   string.Join(", ", list)
来源：http://uzk.nwbrower.top

================================================================================
来源：http://grz.hesvh.cn

E. 字符串处理
来源：http://ymx.birdmap.top

================================================================================
来源：http://seg.yvedp.cn

[E01] 拼接字符串
来源：http://vyi.xuanzx.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fpj.hysaishi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ela.wangdashe.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ody.xingfuxueyuan.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://eex.vqdsnc.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pes.fzhhl.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rvj.zycfv.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ddn.zhengqikj.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yve.quarkkingdee.top

[E02] 重复字符串
来源：http://rmv.yangfankeji.com

Py:   "ab" * 3
来源：http://hmn.zhijiandao.cn

PHP:  str_repeat("ab", 3);
来源：http://gmk.smart0.xyz

JS:   "ab".repeat(3)
来源：http://hfd.nanxinkj.top

TS:   "ab".repeat(3)
来源：http://zfx.nanxuanxn.top

Java: "ab".repeat(3)
来源：http://ide.daxiang520.top

Go:   strings.Repeat("ab", 3)
来源：http://dlx.chenjidiqi.icu

Ruby: "ab" * 3
来源：http://jsm.zhoulong.xyz


<!-- 参考信息 -->