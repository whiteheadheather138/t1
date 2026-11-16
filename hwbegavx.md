代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://zjg.fktsv.cn

C#:   using System.Text;
来源：http://jmq.jlsjyb.cn

[C12] 立即执行函数 IIFE
来源：http://fjq.nanxinkj.top

Py:   (lambda: print("run"))()
来源：http://fun.hnqzz.top

PHP:  (function () { echo "run"; })();
来源：http://umx.sxryk.cn

JS:   (() => { console.log("run"); })();
来源：http://dpy.zdbjq.cn

TS:   (() => { console.log("run"); })();
来源：http://hot.dashuyun.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pcp.yonumen.top

Go:   func() { fmt.Println("run") }()
来源：http://jfi.gotoacloud.top

Ruby: -> { puts "run" }.call
来源：http://lnj.zycfv.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://tba.chenjidiqi.icu

[C13] 类型声明 / 类型注解
来源：http://ptc.chenlongwang.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hzs.cucudq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://htg.vehdjk.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dwz.zhaomingkeji.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://djm.snrcjt.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qkx.yuanzhike.top

Go:   func add(a, b int) int
来源：http://kar.jinyuanbaomall.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cko.hammf.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wfu.cdnleiting.top

[C14] 泛型函数
来源：http://lbd.jinyuanbaomall.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xhs.feifeiyinyue.top

PHP:  // 无泛型
来源：http://rla.nanxinkj.top

JS:   // 无泛型
来源：http://qgx.zhijiandao.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://sja.hnxiangtu.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ogh.smart0.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hhu.fktsv.cn

Ruby: # 无泛型
来源：http://xoc.ydzc1.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wgq.hysaishi.cn

[C15] 解构 / 展开参数
来源：http://ffb.gogol.net.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://knh.epnwcf.com

PHP:  [$a, $b] = $pair;
来源：http://lfp.shzxlz.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rct.havefunace.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qyy.hysaishi.cn

Java: // 无解构
来源：http://bkm.nwbrower.top

Go:   // 无解构
来源：http://hbf.9152youxi.cn

Ruby: a, b = pair
来源：http://pze.aibaodan.cn

C#:   var (a, b) = pair;
来源：http://itg.gaohongyu789.top

[C16] 函数 / 方法重载
来源：http://fqw.chenlongwang.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://udx.birdmap.top

PHP:  // 无重载
来源：http://jub.hongshengwenyu.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://qcg.wangdashe.top

TS:   // 用联合类型或重载签名声明
来源：http://oum.yuanzhike.top

Java: void f(int a) {}  void f(String a) {}
来源：http://vkm.nwbrower.top

Go:   // 无重载：用不同函数名
来源：http://bxy.vehdjk.com

Ruby: # 无重载：靠动态参数
来源：http://qfg.guowangkeji.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://nrh.hnqzz.top

================================================================================
来源：http://uzd.ivvv.top

D. 数组 / 列表 / 集合
来源：http://cyr.sjlbkw.cn

================================================================================
来源：http://cmw.cdnleiting.top

[D01] 创建数组 / 列表
来源：http://lit.sysykeji.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ajk.tian-w.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://uhl.redwolf501.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://epw.redwolf501.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://rec.ctjpmb.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hme.yj202588.top

Go:   arr := []int{1, 2, 3}
来源：http://pcx.ehwqpu.com

Ruby: arr = [1, 2, 3]
来源：http://ucg.sweek.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ruq.sxryk.cn

[D02] 追加元素到末尾
来源：http://rrq.zycfv.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://boi.sufxvd.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pxq.jqgfzy.top

JS:   arr.push(4);
来源：http://mvc.kuanghao11.cn

TS:   arr.push(4);
来源：http://knh.cashguo.top

Java: list.add(4);
来源：http://lic.jqgufenzy.top

Go:   arr = append(arr, 4)
来源：http://con.fanxiaobao.xyz

Ruby: arr << 4; arr.push(5)
来源：http://xaz.sysykeji.top

C#:   list.Add(4);
来源：http://hug.cdnleiting.top

[D03] 在指定位置插入元素
来源：http://rsj.andypj.xyz

Py:   arr.insert(0, 0)
来源：http://mbd.yj20258.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bsn.cashguo.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://aze.jlsjyb.cn

TS:   arr.splice(0, 0, 0);
来源：http://wjq.chenzaomai.com

Java: list.add(0, 0);
来源：http://zbu.haohaochexian.top

Go:   arr = append([]int{0}, arr...)
来源：http://csj.bjfxy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ibc.shangyingyoupin.top

C#:   list.Insert(0, 0);
来源：http://sea.yongpay.top

[D04] 删除元素
来源：http://kva.zhijiandao.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://oqr.tarul.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ypp.smart0.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gyr.hywenlv.cn

TS:   arr.splice(0, 1);
来源：http://ted.nanxuanxn.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dzz.fehbvm.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://guh.xylfe.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tyy.daxiang520.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tze.chenlongwang.top

[D05] 访问与修改元素
来源：http://bad.yj20258888.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mim.tanke756.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nrm.9152youxi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zjn.hysaishi.cn

TS:   arr[0]; arr.at(-1);
来源：http://dum.havefunace.top

Java: list.get(0); list.set(0, 9);
来源：http://apl.shangyingyoupin.top

Go:   arr[0]; arr[0] = 9
来源：http://wwn.cucudq.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mvl.sxryk.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pgp.yanxiufei.cn

[D06] 数组长度
来源：http://isl.fzhhl.top

Py:   len(arr)
来源：http://xai.hnqzz.top

PHP:  count($arr);
来源：http://gil.mhx1999.top

JS:   arr.length
来源：http://wfz.yj202588.top

TS:   arr.length
来源：http://hzw.sweek.top

Java: list.size();
来源：http://qbb.yfazqb.com

Go:   len(arr)
来源：http://xpl.9152youxi.cn

Ruby: arr.length; arr.size
来源：http://qds.xingfuxueyuan.xyz

C#:   list.Count;
来源：http://eel.yueranfly.top

[D07] 切片 / 取子数组
来源：http://edp.nanxinkj.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hxm.jlsjyb.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ixj.gzhubu.top

JS:   arr.slice(1, 4);
来源：http://xue.dianchejie.cn

TS:   arr.slice(1, 4);
来源：http://wxc.chenlongwang.top

Java: list.subList(1, 4);
来源：http://swv.guannengcc.top

Go:   arr[1:4]
来源：http://tfq.quarkkingdee.top

Ruby: arr[1, 3]
来源：http://zne.fehbvm.com

C#:   list.GetRange(1, 3);
来源：http://gxf.redwolf501.top

[D08] 合并两个数组
来源：http://qjt.zhongyouzk.top

Py:   a + b;  a.extend(b)
来源：http://uax.zdqjudy.top

PHP:  array_merge($a, $b);
来源：http://exw.sweek.top

JS:   [...a, ...b];  a.concat(b);
来源：http://inv.yuxming.cn

TS:   [...a, ...b];
来源：http://jey.cqqwz.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rhv.yvedp.cn

Go:   append(a, b...)
来源：http://ffi.pengpengdd.cyou

Ruby: a + b;  a.concat(b)
来源：http://esj.chenjidiqi.icu

C#:   a.Concat(b).ToList()
来源：http://mba.jiagoushi.top

[D09] 排序（升序）
来源：http://gxp.hnxiangtu.top

Py:   sorted(arr);  arr.sort()
来源：http://jqw.gaohongyu789.top

PHP:  sort($arr);
来源：http://dqi.uphjek.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qsy.bbcook.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://diy.hysaishi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vek.xinyue.icu

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xuk.yangfankeji.com

Ruby: arr.sort
来源：http://mmb.guannengcc.top

C#:   list.Sort();
来源：http://zkx.yuanzhike.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://yql.gaohongyu789.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tmp.yj202588.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qov.yvedp.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://iso.wangshuangyany.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kvn.yonumen.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jbq.jlsjyb.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yns.andypj.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yfk.tarul.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wfg.vqdsnc.cn

[D11] 反转数组
来源：http://fmr.yonumen.top

Py:   arr[::-1];  arr.reverse()
来源：http://lwg.xylfe.cn

PHP:  array_reverse($arr);
来源：http://ppn.quarkkingdee.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tam.svipenyu.cn

TS:   [...arr].reverse();
来源：http://cyx.jinyuanbaomall.cn

Java: Collections.reverse(list);
来源：http://qve.snrcjt.cn

Go:   slices.Reverse(arr)
来源：http://uqb.xylfe.cn

Ruby: arr.reverse
来源：http://hhg.316326.xyz

C#:   list.Reverse();
来源：http://uwr.ctjpmb.com

[D12] 查找元素下标
来源：http://bjk.xinyue.icu

Py:   arr.index(x);  x in arr
来源：http://klg.fengsongda.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pis.xuetiantiany.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wrn.yj20258888.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://weq.9152youxi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://oqx.jinyuanbaomall.cn

Go:   slices.Index(arr, x)
来源：http://zjm.bbcook.cn

Ruby: arr.index(x)
来源：http://zgw.jqgufenzy.top

C#:   list.IndexOf(x);
来源：http://uld.jqgufenzy.top

[D13] 过滤（保留满足条件的）
来源：http://gjf.andypj.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://few.sysykeji.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://znn.guowangkeji.top

JS:   arr.filter(x => x > 3)
来源：http://nie.hnqzz.top

TS:   arr.filter(x => x > 3)
来源：http://zij.havefunace.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dqt.tarul.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rkg.tian-w.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ezl.ybcxt.top

C#:   list.Where(x => x > 3).ToList()
来源：http://nao.tianlin.xyz

[D14] 映射转换（每个元素变形）
来源：http://omb.ivvv.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://olh.vehdjk.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vva.iojbl.cn

JS:   arr.map(x => x * 2)
来源：http://tyz.nanxuanxn.top

TS:   arr.map(x => x * 2)
来源：http://yrt.jinqigfzy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://jsf.sxryk.cn

Go:   // 手写循环
来源：http://afa.hfpthk.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hfh.zhongyouzk.top

C#:   list.Select(x => x * 2).ToList()
来源：http://dfh.zhongyouzk.top

[D15] 去重
来源：http://ubl.ppjwa.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yzy.gogol.net.cn

PHP:  array_unique($arr);
来源：http://pei.sweek.top

JS:   [...new Set(arr)]
来源：http://pog.fzhhl.top

TS:   [...new Set(arr)]
来源：http://lds.shanyushiyangkeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fxb.zhoulong.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://dzr.meibo888.top

Ruby: arr.uniq
来源：http://qwq.xylfe.cn

C#:   list.Distinct().ToList()
来源：http://bbw.hywenlv.cn

[D16] 求和与平均值
来源：http://puo.yangfankeji.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fve.c1oappe.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://uvt.yvedp.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bra.jinghuilouyu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wxh.meibo888.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bgp.aibaodan.cn

Go:   // 手写循环累加
来源：http://ana.hongshengwenyu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blr.yanxiufei.cn

C#:   list.Sum();  list.Average()
来源：http://con.cashguo.top

[D17] 最大值与最小值
来源：http://fhd.hnqzz.top

Py:   max(arr);  min(arr)
来源：http://rql.guowangkeji.top

PHP:  max($arr);  min($arr);
来源：http://zjn.sxryk.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wkr.jinghuilouyu.cn

TS:   Math.max(...arr);
来源：http://lfo.xylfe.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gpb.daria6918.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pao.shanyushiyangkeji.top

Ruby: arr.max;  arr.min
来源：http://ejk.chenzaomai.com

C#:   list.Max();  list.Min()
来源：http://huy.hysaishi.cn

[D18] 扁平化嵌套数组
来源：http://opg.redwolf501.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pbz.snrcjt.cn

PHP:  array_merge(...$nested);
来源：http://nxu.hongshengwenyu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fhc.iojbl.cn

TS:   nested.flat();
来源：http://nst.xuanzx.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tdv.yvedp.cn

Go:   // 手写双层循环
来源：http://zpo.shanyushiyangtech.top

Ruby: nested.flatten
来源：http://wlg.shangyingyoupin.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://pon.yuxming.cn

[D19] 按字段分组
来源：http://bzy.fanxiaobao.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pch.shanyushiyangkeji.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pqz.gogol.net.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://acs.zycfv.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://dlb.gogol.net.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://uro.guannengcc.top

Go:   // 手写 map[string][]T
来源：http://son.ivvv.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://zzr.aizwys.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://svk.gzhubu.top

[D20] 统计每个元素出现次数
来源：http://sii.dashuyun.cn

Py:   Counter(arr)
来源：http://cgm.guannengcc.top

PHP:  array_count_values($arr);
来源：http://idp.gotoacloud.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ops.cqqwz.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ffd.kuanghao11.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://stc.aizwys.cn

Go:   // 手写 map[T]int
来源：http://owx.316326.xyz

Ruby: arr.tally
来源：http://fbe.hywenlv.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gcu.ywan-chungtsiang.top

[D21] 判断是否包含某元素
来源：http://hjr.xziqi.cn

Py:   x in arr
来源：http://uum.zhijiandao.cn

PHP:  in_array($x, $arr, true);
来源：http://zyo.jinyuanbaomall.cn

JS:   arr.includes(x)
来源：http://jvc.zhijiandao.cn

TS:   arr.includes(x)
来源：http://bjx.ywan-chungtsiang.top

Java: list.contains(x)
来源：http://rok.hysaishi.cn

Go:   slices.Contains(arr, x)
来源：http://pgu.jqgfzy.top

Ruby: arr.include?(x)
来源：http://zjq.zhijiandao.cn

C#:   list.Contains(x)
来源：http://vlt.pycfn.com

[D22] 复制数组（避免共享引用）
来源：http://cbs.meibo888.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://llp.tian-w.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yao.tarul.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ear.pycfn.com

TS:   [...arr];
来源：http://qll.ehwqpu.com

Java: new ArrayList<>(list);
来源：http://ydx.zdbjq.cn

Go:   copied := append([]int(nil), arr...)
来源：http://snu.gzhubu.top

Ruby: arr.dup;  arr.clone
来源：http://nrf.wangshuangyany.cn

C#:   new List<int>(list);
来源：http://wkb.ivvv.top

[D23] reduce 累积计算
来源：http://whe.guowangkeji.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ztc.chenzaomai.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cvu.birdmap.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sgs.zhaomingkeji.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zxq.vehdjk.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://tcp.svipenyu.cn

Go:   // 手写循环
来源：http://zry.hywenlv.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mqq.haohaochexian.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mow.dianchejie.cn

[D24] 字典 / Map 基本操作
来源：http://pgm.jinghuilouyu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ycs.fzhhl.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nbh.hnqzz.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ijm.shangyingyoupin.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pte.hywenlv.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://akr.ydjk.org.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tiw.iojbl.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://eij.nanxuanxn.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uka.uphjek.com

[D25] Set 集合去重与交并差
来源：http://ccx.zhiwuduotai.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dro.chenjidiqi.icu

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tog.gaohongyu789.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qvp.epnwcf.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zgl.yonumen.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cjk.gogol.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zcp.birdmap.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sfb.wangshuangyany.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://peb.zhiwuduotai.top

[D26] 数组转字符串
来源：http://gja.yongpay.top

Py:   ", ".join(map(str, arr))
来源：http://myp.jyoumei.cn

PHP:  implode(", ", $arr);
来源：http://pjl.jinyuanbaomall.cn

JS:   arr.join(", ")
来源：http://rge.sufxvd.cn

TS:   arr.join(", ")
来源：http://vev.bjfxy.top

Java: String.join(", ", list)
来源：http://qis.hnxiangtu.top

Go:   strings.Join(strs, ", ")
来源：http://ecs.zycfv.cn

Ruby: arr.join(", ")
来源：http://hah.feifeiyinyue.top

C#:   string.Join(", ", list)
来源：http://mxh.shuidangran.top

================================================================================
来源：http://ock.zhiwuduotai.top

E. 字符串处理
来源：http://edt.fengsongda.top

================================================================================
来源：http://uyh.fktsv.cn

[E01] 拼接字符串
来源：http://kwt.yuxming.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://eqw.yueranfly.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nly.daxiang520.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hke.jinghuilouyu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://phm.jlsjyb.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lga.aibaodan.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mik.xingfuxueyuan.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fcc.jqgfzy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kok.shanyushiyangtech.top

[E02] 重复字符串
来源：http://qsn.c1oappe.top

Py:   "ab" * 3
来源：http://qwa.yueranfly.top

PHP:  str_repeat("ab", 3);
来源：http://vlu.gotoacloud.top

JS:   "ab".repeat(3)
来源：http://yia.redwolf501.top


<!-- 参考信息 -->