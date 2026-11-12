代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://xkb.zhengqikj.top

C#:   using System.Text;
来源：http://idq.zycfv.cn

[C12] 立即执行函数 IIFE
来源：http://ahr.dianchejie.cn

Py:   (lambda: print("run"))()
来源：http://gak.yfazqb.com

PHP:  (function () { echo "run"; })();
来源：http://xyw.xingfuxueyuan.xyz

JS:   (() => { console.log("run"); })();
来源：http://fiz.gotoacloud.top

TS:   (() => { console.log("run"); })();
来源：http://jvw.ppjwa.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jtz.wangdashe.top

Go:   func() { fmt.Println("run") }()
来源：http://pcv.havefunace.top

Ruby: -> { puts "run" }.call
来源：http://nzg.tanke756.top

C#:   // 无 IIFE：用静态构造函数
来源：http://cws.jinghuilouyu.cn

[C13] 类型声明 / 类型注解
来源：http://lxh.ywan-chungtsiang.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zua.xuanzx.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sxn.ywan-chungtsiang.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://apl.jqgufenzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://svj.hnxiangtu.top

Java: int add(int a, int b) { return a + b; }
来源：http://pli.hcnkem.com

Go:   func add(a, b int) int
来源：http://egw.sufxvd.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mfq.guowangkeji.top

C#:   int Add(int a, int b) => a + b;
来源：http://ker.ppjwa.cn

[C14] 泛型函数
来源：http://pxk.yueranfly.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ydo.c1oappe.top

PHP:  // 无泛型
来源：http://rfx.aibaodan.cn

JS:   // 无泛型
来源：http://nup.jqgufenzy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vtk.ywan-chungtsiang.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qpp.fengsongda.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zvs.zhengqikj.top

Ruby: # 无泛型
来源：http://nsh.snrcjt.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fcr.snrcjt.cn

[C15] 解构 / 展开参数
来源：http://hmo.shanyushiyangkeji.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bfx.hesvh.cn

PHP:  [$a, $b] = $pair;
来源：http://htv.hongshengwenyu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uxj.yj20258.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fje.shanyushiyangtech.top

Java: // 无解构
来源：http://qil.kuanghao11.cn

Go:   // 无解构
来源：http://bty.svipenyu.cn

Ruby: a, b = pair
来源：http://tgp.bbcook.cn

C#:   var (a, b) = pair;
来源：http://eau.sufxvd.cn

[C16] 函数 / 方法重载
来源：http://xlj.bjfxy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bzq.wangdashe.top

PHP:  // 无重载
来源：http://gos.hnxiangtu.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://lcv.vehdjk.com

TS:   // 用联合类型或重载签名声明
来源：http://uvx.mhx1999.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ies.hesvh.cn

Go:   // 无重载：用不同函数名
来源：http://fxo.zdqjudy.top

Ruby: # 无重载：靠动态参数
来源：http://zki.cqqwz.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://yqg.mhx1999.top

================================================================================
来源：http://zbf.nanxuanxn.top

D. 数组 / 列表 / 集合
来源：http://gpp.xuanzx.com

================================================================================
来源：http://qcu.xylfe.cn

[D01] 创建数组 / 列表
来源：http://ijp.gotoacloud.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://rsi.cqqwz.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cyd.xziqi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qlh.shzxlz.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bgy.c1oappe.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jfn.pengpengdd.cyou

Go:   arr := []int{1, 2, 3}
来源：http://pbe.ctjpmb.com

Ruby: arr = [1, 2, 3]
来源：http://wzy.dianchejie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://erz.zhixingplan.top

[D02] 追加元素到末尾
来源：http://czl.cucudq.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yje.tanke756.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://okx.dashuyun.cn

JS:   arr.push(4);
来源：http://fyq.redwolf501.top

TS:   arr.push(4);
来源：http://ixe.ctjpmb.com

Java: list.add(4);
来源：http://ipt.xingfuxueyuan.xyz

Go:   arr = append(arr, 4)
来源：http://gxs.hongshengwenyu.top

Ruby: arr << 4; arr.push(5)
来源：http://fiq.ctjpmb.com

C#:   list.Add(4);
来源：http://all.dashuyun.cn

[D03] 在指定位置插入元素
来源：http://gez.yanxiufei.cn

Py:   arr.insert(0, 0)
来源：http://uju.zhaomingkeji.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ews.jqgfzy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hhr.andypj.xyz

TS:   arr.splice(0, 0, 0);
来源：http://toc.sxryk.cn

Java: list.add(0, 0);
来源：http://ilf.aizwys.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ywc.dianchejie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://siu.zdqjudy.top

C#:   list.Insert(0, 0);
来源：http://lrp.quarkkingdee.top

[D04] 删除元素
来源：http://jlo.pycfn.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qxz.hysaishi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ffv.yj202588.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dxu.jlsjyb.cn

TS:   arr.splice(0, 1);
来源：http://wbe.xuetiantiany.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yxv.cashguo.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vhz.gzhubu.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rcw.xingfuxueyuan.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wie.yueranfly.top

[D05] 访问与修改元素
来源：http://lqu.havefunace.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vvh.yueranfly.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mmo.wangdashe.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ntu.jianghu66.top

TS:   arr[0]; arr.at(-1);
来源：http://vib.ydzc1.top

Java: list.get(0); list.set(0, 9);
来源：http://uyp.vqdsnc.cn

Go:   arr[0]; arr[0] = 9
来源：http://vpd.ivvv.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gpg.tanke756.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zxd.fzhhl.top

[D06] 数组长度
来源：http://cyg.fzhhl.top

Py:   len(arr)
来源：http://adv.tian-w.cn

PHP:  count($arr);
来源：http://aru.bjfxy.top

JS:   arr.length
来源：http://ptd.chenjidiqi.icu

TS:   arr.length
来源：http://rzp.yongpay.top

Java: list.size();
来源：http://qah.zdbjq.cn

Go:   len(arr)
来源：http://dls.chenjidiqi.icu

Ruby: arr.length; arr.size
来源：http://coq.yonumen.top

C#:   list.Count;
来源：http://azf.chenlongwang.top

[D07] 切片 / 取子数组
来源：http://psq.feifeiyinyue.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fhs.gotoacloud.top

PHP:  array_slice($arr, 1, 3);
来源：http://eqs.ydjk.org.cn

JS:   arr.slice(1, 4);
来源：http://zzb.zhongyouzk.top

TS:   arr.slice(1, 4);
来源：http://gne.gotoacloud.top

Java: list.subList(1, 4);
来源：http://fnl.fktsv.cn

Go:   arr[1:4]
来源：http://zmq.epnwcf.com

Ruby: arr[1, 3]
来源：http://run.aibaodan.cn

C#:   list.GetRange(1, 3);
来源：http://pwc.jinghuilouyu.cn

[D08] 合并两个数组
来源：http://zmt.zdqjudy.top

Py:   a + b;  a.extend(b)
来源：http://cnw.yanxiufei.cn

PHP:  array_merge($a, $b);
来源：http://qfi.kuanghao11.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zoo.cucudq.cn

TS:   [...a, ...b];
来源：http://dab.redwolf501.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kze.hesvh.cn

Go:   append(a, b...)
来源：http://ogq.aizwys.cn

Ruby: a + b;  a.concat(b)
来源：http://vou.yj20258.top

C#:   a.Concat(b).ToList()
来源：http://ahd.nanxuanxn.top

[D09] 排序（升序）
来源：http://gbz.zhengqikj.top

Py:   sorted(arr);  arr.sort()
来源：http://lla.fzhhl.top

PHP:  sort($arr);
来源：http://rvg.jlsjyb.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tnq.hnqzz.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://kse.sxryk.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mos.zhijiandao.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ijd.hcnkem.com

Ruby: arr.sort
来源：http://yjt.mhx1999.top

C#:   list.Sort();
来源：http://aaf.zdqjudy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://emq.smart0.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fmg.xylfe.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hse.hnqzz.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xpi.xziqi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wky.tian-w.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sch.sjlbkw.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wez.yfazqb.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mbg.jiagoushi.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jbo.yanxiufei.cn

[D11] 反转数组
来源：http://mso.ctjpmb.com

Py:   arr[::-1];  arr.reverse()
来源：http://iey.havefunace.top

PHP:  array_reverse($arr);
来源：http://kyr.nanxinkj.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xsz.snrcjt.cn

TS:   [...arr].reverse();
来源：http://sev.gaohongyu789.top

Java: Collections.reverse(list);
来源：http://nll.shangyingyoupin.top

Go:   slices.Reverse(arr)
来源：http://gqo.hongshengwenyu.top

Ruby: arr.reverse
来源：http://xmn.yj20258888.top

C#:   list.Reverse();
来源：http://ipu.sysykeji.top

[D12] 查找元素下标
来源：http://xig.xinyue.icu

Py:   arr.index(x);  x in arr
来源：http://kei.jlsjyb.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gej.zhijiandao.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sog.hywenlv.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sob.hysaishi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qxu.aizwys.cn

Go:   slices.Index(arr, x)
来源：http://uza.ydzc1.top

Ruby: arr.index(x)
来源：http://itj.svipenyu.cn

C#:   list.IndexOf(x);
来源：http://jyw.svipenyu.cn

[D13] 过滤（保留满足条件的）
来源：http://ocu.chenjidiqi.icu

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fcy.jianghu66.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rbd.iojbl.cn

JS:   arr.filter(x => x > 3)
来源：http://wcw.epnwcf.com

TS:   arr.filter(x => x > 3)
来源：http://rpu.redwolf501.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mgz.gogol.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ykk.shuidangran.top

Ruby: arr.select { |x| x > 3 }
来源：http://tza.hysaishi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://szx.zycfv.cn

[D14] 映射转换（每个元素变形）
来源：http://hdv.iojbl.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tec.ehwqpu.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mtn.hnqzz.top

JS:   arr.map(x => x * 2)
来源：http://kjf.c1oappe.top

TS:   arr.map(x => x * 2)
来源：http://ydd.fengsongda.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://mbl.yongpay.top

Go:   // 手写循环
来源：http://rhw.haohaochexian.top

Ruby: arr.map { |x| x * 2 }
来源：http://viy.shanyushiyangtech.top

C#:   list.Select(x => x * 2).ToList()
来源：http://mav.gzhubu.top

[D15] 去重
来源：http://hyt.cucudq.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mlg.fktsv.cn

PHP:  array_unique($arr);
来源：http://jxh.pycfn.com

JS:   [...new Set(arr)]
来源：http://spx.yuanzhike.top

TS:   [...new Set(arr)]
来源：http://jeq.sufxvd.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zsp.yuxming.cn

Go:   // 用 map[T]struct{} 手写
来源：http://rve.iojbl.cn

Ruby: arr.uniq
来源：http://hsh.tarul.cn

C#:   list.Distinct().ToList()
来源：http://mfw.tianlin.xyz

[D16] 求和与平均值
来源：http://zds.yanxiufei.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://eqz.mhx1999.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yan.yuxming.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://arb.ehwqpu.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mnb.wangdashe.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zpu.aibaodan.cn

Go:   // 手写循环累加
来源：http://vap.hysaishi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hfk.jqgufenzy.top

C#:   list.Sum();  list.Average()
来源：http://rbw.xuanzx.com

[D17] 最大值与最小值
来源：http://uyw.sysykeji.top

Py:   max(arr);  min(arr)
来源：http://ifv.fehbvm.com

PHP:  max($arr);  min($arr);
来源：http://jaz.tanke756.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zhn.fktsv.cn

TS:   Math.max(...arr);
来源：http://lva.shuidangran.top

Java: Collections.max(list);  Collections.min(list);
来源：http://rbo.ybcxt.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vjx.shanyushiyangtech.top

Ruby: arr.max;  arr.min
来源：http://umq.0kj1m.cn

C#:   list.Max();  list.Min()
来源：http://enw.yvedp.cn

[D18] 扁平化嵌套数组
来源：http://mmn.fzhhl.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kzi.yueranfly.top

PHP:  array_merge(...$nested);
来源：http://bis.daxiang520.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hfc.tanke756.top

TS:   nested.flat();
来源：http://hyn.zhengqikj.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qqh.daxiang520.top

Go:   // 手写双层循环
来源：http://ouo.fehbvm.com

Ruby: nested.flatten
来源：http://mbu.sysykeji.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://wdj.vehdjk.com

[D19] 按字段分组
来源：http://ljh.yongpay.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qui.jinqigfzy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nir.shzxlz.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yfc.jlsjyb.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vjm.shanyushiyangkeji.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://enh.zhongyouzk.top

Go:   // 手写 map[string][]T
来源：http://xyo.zhongyouzk.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://zli.andypj.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uxe.zdqjudy.top

[D20] 统计每个元素出现次数
来源：http://cxj.birdmap.top

Py:   Counter(arr)
来源：http://jcg.hysaishi.cn

PHP:  array_count_values($arr);
来源：http://zcx.vehdjk.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ony.svipenyu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rkf.tian-w.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ukq.c1oappe.top

Go:   // 手写 map[T]int
来源：http://iqe.snrcjt.cn

Ruby: arr.tally
来源：http://gyb.aibaodan.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ohq.zhengqikj.top

[D21] 判断是否包含某元素
来源：http://sla.jinqigufen.top

Py:   x in arr
来源：http://yqm.dashuyun.cn

PHP:  in_array($x, $arr, true);
来源：http://ici.hammf.cn

JS:   arr.includes(x)
来源：http://lqy.hywenlv.cn

TS:   arr.includes(x)
来源：http://qgr.ppjwa.cn

Java: list.contains(x)
来源：http://cnl.gaohongyu789.top

Go:   slices.Contains(arr, x)
来源：http://nox.aibaodan.cn

Ruby: arr.include?(x)
来源：http://tcg.hnxiangtu.top

C#:   list.Contains(x)
来源：http://nwv.316326.xyz

[D22] 复制数组（避免共享引用）
来源：http://tpj.sweek.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rrg.gaohongyu789.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://szb.yuanzhike.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bnp.dianchejie.cn

TS:   [...arr];
来源：http://utt.nanxinkj.top

Java: new ArrayList<>(list);
来源：http://jyk.mhx1999.top

Go:   copied := append([]int(nil), arr...)
来源：http://khk.tianlin.xyz

Ruby: arr.dup;  arr.clone
来源：http://xym.sufxvd.cn

C#:   new List<int>(list);
来源：http://rdg.xuanzx.com

[D23] reduce 累积计算
来源：http://thv.meibo888.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://myn.nanxinkj.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xqp.shanyushiyangtech.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dru.iojbl.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ibe.hcnkem.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://pxw.xuanzx.com

Go:   // 手写循环
来源：http://wse.vehdjk.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://opi.ydzc1.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ivt.chenlongwang.top

[D24] 字典 / Map 基本操作
来源：http://lax.xingfuxueyuan.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cfl.pengpengdd.cyou

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://opt.yueranfly.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ulj.epnwcf.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jdi.yonumen.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nou.jyoumei.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qdv.zhengqikj.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qka.chenlongwang.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mzy.ivvv.top

[D25] Set 集合去重与交并差
来源：http://jpw.ydjk.org.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zfl.smart0.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ybm.shzxlz.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bqo.gogol.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nsa.gotoacloud.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xqe.xziqi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dwg.bjfxy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://spb.jqgfzy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fsa.zhengqikj.top

[D26] 数组转字符串
来源：http://cfj.hesvh.cn

Py:   ", ".join(map(str, arr))
来源：http://kzq.zdbjq.cn

PHP:  implode(", ", $arr);
来源：http://txx.shanyushiyangkeji.top

JS:   arr.join(", ")
来源：http://mrj.0kj1m.cn

TS:   arr.join(", ")
来源：http://wsf.zhoulong.xyz

Java: String.join(", ", list)
来源：http://xkf.guowangkeji.top

Go:   strings.Join(strs, ", ")
来源：http://iyo.yonumen.top

Ruby: arr.join(", ")
来源：http://yzp.nwbrower.top

C#:   string.Join(", ", list)
来源：http://hdb.aizwys.cn

================================================================================
来源：http://tjx.quarkkingdee.top

E. 字符串处理
来源：http://ksk.fanxiaobao.xyz

================================================================================
来源：http://ofo.fanxiaobao.xyz

[E01] 拼接字符串
来源：http://ccm.hnqzz.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qyw.ehwqpu.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://stb.jqgfzy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://roc.xziqi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cdz.zhengqikj.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zfb.svipenyu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yrc.yangfankeji.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zoc.xuetiantiany.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mrv.hnxiangtu.top

[E02] 重复字符串
来源：http://dje.birdmap.top

Py:   "ab" * 3
来源：http://uwf.ydzc1.top

PHP:  str_repeat("ab", 3);
来源：http://ejg.gogol.net.cn

JS:   "ab".repeat(3)
来源：http://izb.fehbvm.com


<!-- 参考信息 -->