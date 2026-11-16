代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://gyc.nwbrower.top

C#:   using System.Text;
来源：http://ncn.gogol.net.cn

[C12] 立即执行函数 IIFE
来源：http://oiw.nwbrower.top

Py:   (lambda: print("run"))()
来源：http://dex.hcnkem.com

PHP:  (function () { echo "run"; })();
来源：http://pdm.uphjek.com

JS:   (() => { console.log("run"); })();
来源：http://gsi.zhongyouzk.top

TS:   (() => { console.log("run"); })();
来源：http://ded.zhengqikj.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vrt.sysykeji.top

Go:   func() { fmt.Println("run") }()
来源：http://etq.zhaomingkeji.xyz

Ruby: -> { puts "run" }.call
来源：http://wpb.zdqjudy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://vsy.hfpthk.cn

[C13] 类型声明 / 类型注解
来源：http://vpr.dianchejie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dlq.hnqzz.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cxt.zhijiandao.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tvn.shzxlz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dbj.jinghuilouyu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://dds.shzxlz.cn

Go:   func add(a, b int) int
来源：http://tra.xuetiantiany.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xok.shuidangran.top

C#:   int Add(int a, int b) => a + b;
来源：http://cpp.daxiang520.top

[C14] 泛型函数
来源：http://qgn.mhx1999.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ffk.epnwcf.com

PHP:  // 无泛型
来源：http://kbw.havefunace.top

JS:   // 无泛型
来源：http://mlt.jinqigufen.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://etm.xziqi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://atn.yfazqb.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mdp.epnwcf.com

Ruby: # 无泛型
来源：http://dix.sweek.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://emo.dashuyun.cn

[C15] 解构 / 展开参数
来源：http://seg.c1oappe.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rat.jqgfzy.top

PHP:  [$a, $b] = $pair;
来源：http://ste.quarkkingdee.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jvd.pycfn.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tzu.sjlbkw.cn

Java: // 无解构
来源：http://ymf.tanke756.top

Go:   // 无解构
来源：http://uzk.yuxming.cn

Ruby: a, b = pair
来源：http://hgh.yj20258.top

C#:   var (a, b) = pair;
来源：http://oeg.xuetiantiany.cn

[C16] 函数 / 方法重载
来源：http://zaj.hesvh.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bhq.ehwqpu.com

PHP:  // 无重载
来源：http://fzj.chenzaomai.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://lrf.zdbjq.cn

TS:   // 用联合类型或重载签名声明
来源：http://awe.tarul.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xwp.ppjwa.cn

Go:   // 无重载：用不同函数名
来源：http://ait.andypj.xyz

Ruby: # 无重载：靠动态参数
来源：http://rfa.xuetiantiany.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://wem.xylfe.cn

================================================================================
来源：http://dld.yongpay.top

D. 数组 / 列表 / 集合
来源：http://brx.snrcjt.cn

================================================================================
来源：http://lsa.jinqigufen.top

[D01] 创建数组 / 列表
来源：http://eah.gaohongyu789.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://rst.shzxlz.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mrg.iojbl.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://irc.jqgfzy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://rkh.jqgufenzy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kkv.0kj1m.cn

Go:   arr := []int{1, 2, 3}
来源：http://uqr.yj202588.top

Ruby: arr = [1, 2, 3]
来源：http://bhm.fktsv.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xfb.birdmap.top

[D02] 追加元素到末尾
来源：http://pdd.hnxiangtu.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hzs.tianlin.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jnl.haohaochexian.top

JS:   arr.push(4);
来源：http://pmj.fktsv.cn

TS:   arr.push(4);
来源：http://thd.hammf.cn

Java: list.add(4);
来源：http://rdk.aibaodan.cn

Go:   arr = append(arr, 4)
来源：http://ozi.xinyue.icu

Ruby: arr << 4; arr.push(5)
来源：http://azo.jinqigufen.top

C#:   list.Add(4);
来源：http://fsh.cdnleiting.top

[D03] 在指定位置插入元素
来源：http://jhp.bbcook.cn

Py:   arr.insert(0, 0)
来源：http://ueh.snrcjt.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dbw.daxiang520.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vuw.hesvh.cn

TS:   arr.splice(0, 0, 0);
来源：http://vbs.chenzaomai.com

Java: list.add(0, 0);
来源：http://btj.zhongyouzk.top

Go:   arr = append([]int{0}, arr...)
来源：http://npr.hnqzz.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pff.xuetiantiany.cn

C#:   list.Insert(0, 0);
来源：http://eyt.daria6918.cn

[D04] 删除元素
来源：http://rgw.wangdashe.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://oez.daxiang520.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kjj.nanxuanxn.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://deh.hongshengwenyu.top

TS:   arr.splice(0, 1);
来源：http://gtd.bbcook.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wwo.zdbjq.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fsg.yanxiufei.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zjs.ehwqpu.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ajb.gaohongyu789.top

[D05] 访问与修改元素
来源：http://ymy.epnwcf.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dyl.xuanzx.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ida.cdnleiting.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gbi.fzhhl.top

TS:   arr[0]; arr.at(-1);
来源：http://jxs.sysykeji.top

Java: list.get(0); list.set(0, 9);
来源：http://nwj.yuxming.cn

Go:   arr[0]; arr[0] = 9
来源：http://pgq.jqgufenzy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://byv.nanxinkj.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vco.xylfe.cn

[D06] 数组长度
来源：http://ksw.fktsv.cn

Py:   len(arr)
来源：http://ooh.tian-w.cn

PHP:  count($arr);
来源：http://iun.chenjidiqi.icu

JS:   arr.length
来源：http://wwj.yvedp.cn

TS:   arr.length
来源：http://xai.pengpengdd.cyou

Java: list.size();
来源：http://iai.nanxinkj.top

Go:   len(arr)
来源：http://xtt.guowangkeji.top

Ruby: arr.length; arr.size
来源：http://jtc.redwolf501.top

C#:   list.Count;
来源：http://zdf.nanxuanxn.top

[D07] 切片 / 取子数组
来源：http://hfy.dashuyun.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ufa.zhaomingkeji.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://sdh.smart0.xyz

JS:   arr.slice(1, 4);
来源：http://uyn.sjlbkw.cn

TS:   arr.slice(1, 4);
来源：http://waa.wangshuangyany.cn

Java: list.subList(1, 4);
来源：http://ivj.shuidangran.top

Go:   arr[1:4]
来源：http://qqw.yuanzhike.top

Ruby: arr[1, 3]
来源：http://oxl.guannengcc.top

C#:   list.GetRange(1, 3);
来源：http://ufj.316326.xyz

[D08] 合并两个数组
来源：http://ejb.zhongyouzk.top

Py:   a + b;  a.extend(b)
来源：http://ebb.daria6918.cn

PHP:  array_merge($a, $b);
来源：http://koo.yanxiufei.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://iqw.fehbvm.com

TS:   [...a, ...b];
来源：http://qpn.snrcjt.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fqu.c1oappe.top

Go:   append(a, b...)
来源：http://sqw.ywan-chungtsiang.top

Ruby: a + b;  a.concat(b)
来源：http://oly.ybcxt.top

C#:   a.Concat(b).ToList()
来源：http://rma.nwbrower.top

[D09] 排序（升序）
来源：http://sdn.pycfn.com

Py:   sorted(arr);  arr.sort()
来源：http://deg.uphjek.com

PHP:  sort($arr);
来源：http://tvz.yangfankeji.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://siy.nanxinkj.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ldf.quarkkingdee.top

Java: Collections.sort(list);  list.sort(null);
来源：http://hdx.jinyuanbaomall.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tuv.zhiwuduotai.top

Ruby: arr.sort
来源：http://erx.zhaomingkeji.xyz

C#:   list.Sort();
来源：http://crr.chenlongwang.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://mbh.jqgufenzy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gcb.mhx1999.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hdy.nwbrower.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dci.xinyue.icu

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://drb.zhiwuduotai.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lad.guowangkeji.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ujx.birdmap.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://brh.shangyingyoupin.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cyd.aibaodan.cn

[D11] 反转数组
来源：http://zjb.dianchejie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://sre.dashuyun.cn

PHP:  array_reverse($arr);
来源：http://zwh.cdnleiting.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ryu.shanyushiyangtech.top

TS:   [...arr].reverse();
来源：http://ilq.meibo888.top

Java: Collections.reverse(list);
来源：http://htx.ydjk.org.cn

Go:   slices.Reverse(arr)
来源：http://hmp.zhoulong.xyz

Ruby: arr.reverse
来源：http://bqr.zdbjq.cn

C#:   list.Reverse();
来源：http://mee.aibaodan.cn

[D12] 查找元素下标
来源：http://rur.bbcook.cn

Py:   arr.index(x);  x in arr
来源：http://kht.fanxiaobao.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kar.ehwqpu.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gzv.zdbjq.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://awf.ydzc1.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ugi.shanyushiyangtech.top

Go:   slices.Index(arr, x)
来源：http://axm.yvedp.cn

Ruby: arr.index(x)
来源：http://jnb.havefunace.top

C#:   list.IndexOf(x);
来源：http://fes.hnxiangtu.top

[D13] 过滤（保留满足条件的）
来源：http://fym.shanyushiyangkeji.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lko.xinyue.icu

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ome.tarul.cn

JS:   arr.filter(x => x > 3)
来源：http://evj.cashguo.top

TS:   arr.filter(x => x > 3)
来源：http://owt.jinghuilouyu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gqv.wangshuangyany.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fpb.hywenlv.cn

Ruby: arr.select { |x| x > 3 }
来源：http://zqp.xingfuxueyuan.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://qnq.hfpthk.cn

[D14] 映射转换（每个元素变形）
来源：http://bxx.shanyushiyangkeji.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wnd.daxiang520.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xqk.hywenlv.cn

JS:   arr.map(x => x * 2)
来源：http://twg.jlsjyb.cn

TS:   arr.map(x => x * 2)
来源：http://grp.uphjek.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://llx.chenjidiqi.icu

Go:   // 手写循环
来源：http://aca.yangfankeji.com

Ruby: arr.map { |x| x * 2 }
来源：http://sey.9152youxi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://bmj.hnxiangtu.top

[D15] 去重
来源：http://jhx.xuanzx.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pxb.shzxlz.cn

PHP:  array_unique($arr);
来源：http://ago.sxryk.cn

JS:   [...new Set(arr)]
来源：http://pwu.yonumen.top

TS:   [...new Set(arr)]
来源：http://tvp.zycfv.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ysn.vehdjk.com

Go:   // 用 map[T]struct{} 手写
来源：http://htj.52xcode.cn

Ruby: arr.uniq
来源：http://qrs.vqdsnc.cn

C#:   list.Distinct().ToList()
来源：http://qbs.jinghuilouyu.cn

[D16] 求和与平均值
来源：http://uhh.yfazqb.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kax.ppjwa.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ppa.chenjidiqi.icu

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://phi.kuanghao11.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://slb.smart0.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nry.jinqigfzy.top

Go:   // 手写循环累加
来源：http://tto.c1oappe.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nvf.ydzc1.top

C#:   list.Sum();  list.Average()
来源：http://ekd.nwbrower.top

[D17] 最大值与最小值
来源：http://dfo.chenlongwang.top

Py:   max(arr);  min(arr)
来源：http://stw.zhixingplan.top

PHP:  max($arr);  min($arr);
来源：http://klf.yj20258888.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ckf.shangyingyoupin.top

TS:   Math.max(...arr);
来源：http://gin.ivvv.top

Java: Collections.max(list);  Collections.min(list);
来源：http://wgi.ywan-chungtsiang.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mza.zhixingplan.top

Ruby: arr.max;  arr.min
来源：http://fao.wangshuangyany.cn

C#:   list.Max();  list.Min()
来源：http://bho.yangfankeji.com

[D18] 扁平化嵌套数组
来源：http://wkk.aibaodan.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ixw.yanxiufei.cn

PHP:  array_merge(...$nested);
来源：http://fxk.jianghu66.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ikb.kuanghao11.cn

TS:   nested.flat();
来源：http://ioh.ydzc1.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kfp.nanxinkj.top

Go:   // 手写双层循环
来源：http://ast.yuanzhike.top

Ruby: nested.flatten
来源：http://xts.c1oappe.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://egm.zycfv.cn

[D19] 按字段分组
来源：http://pse.yuxming.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jec.wangdashe.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cve.hysaishi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ozm.cheryme.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://rge.chenlongwang.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://egn.zhongyouzk.top

Go:   // 手写 map[string][]T
来源：http://wbx.uphjek.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://ycw.nanxuanxn.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jbp.zhoulong.xyz

[D20] 统计每个元素出现次数
来源：http://qoz.shzxlz.cn

Py:   Counter(arr)
来源：http://xuz.hongshengwenyu.top

PHP:  array_count_values($arr);
来源：http://dpa.havefunace.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xia.shzxlz.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://brm.bjfxy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mjs.gzhubu.top

Go:   // 手写 map[T]int
来源：http://mse.9152youxi.cn

Ruby: arr.tally
来源：http://ens.zhoulong.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://obf.ybcxt.top

[D21] 判断是否包含某元素
来源：http://fpp.redwolf501.top

Py:   x in arr
来源：http://gsp.ydjk.org.cn

PHP:  in_array($x, $arr, true);
来源：http://vpl.sufxvd.cn

JS:   arr.includes(x)
来源：http://cfl.yvedp.cn

TS:   arr.includes(x)
来源：http://dwn.yfazqb.com

Java: list.contains(x)
来源：http://wqq.ywan-chungtsiang.top

Go:   slices.Contains(arr, x)
来源：http://zqn.9152youxi.cn

Ruby: arr.include?(x)
来源：http://jst.daxiang520.top

C#:   list.Contains(x)
来源：http://ugi.fanxiaobao.xyz

[D22] 复制数组（避免共享引用）
来源：http://uch.sysykeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://oxb.kuanghao11.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zkp.tarul.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://god.shangyingyoupin.top

TS:   [...arr];
来源：http://ksn.epnwcf.com

Java: new ArrayList<>(list);
来源：http://phg.feifeiyinyue.top

Go:   copied := append([]int(nil), arr...)
来源：http://uhr.yj202588.top

Ruby: arr.dup;  arr.clone
来源：http://ydw.fzhhl.top

C#:   new List<int>(list);
来源：http://hav.snrcjt.cn

[D23] reduce 累积计算
来源：http://phz.shanyushiyangtech.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qvq.iojbl.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wps.xuanzx.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://huu.chenlongwang.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ucq.mhx1999.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://tfu.jiagoushi.top

Go:   // 手写循环
来源：http://aju.ivvv.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://trz.zhengqikj.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ggs.shanyushiyangtech.top

[D24] 字典 / Map 基本操作
来源：http://esj.mhx1999.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mvz.shzxlz.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pne.yuanzhike.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bbk.gotoacloud.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fur.jyoumei.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://enz.tianlin.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wih.ydjk.org.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wfl.daria6918.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://erk.jinyuanbaomall.cn

[D25] Set 集合去重与交并差
来源：http://kav.hcnkem.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xpn.yj20258.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bji.hammf.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ged.cqqwz.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://saq.shanyushiyangtech.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hjt.hongshengwenyu.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://iet.hywenlv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jfs.chenzaomai.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://erq.jiagoushi.top

[D26] 数组转字符串
来源：http://otp.aibaodan.cn

Py:   ", ".join(map(str, arr))
来源：http://kwl.jinqigufen.top

PHP:  implode(", ", $arr);
来源：http://aex.vqdsnc.cn

JS:   arr.join(", ")
来源：http://jch.tarul.cn

TS:   arr.join(", ")
来源：http://qao.ydzc1.top

Java: String.join(", ", list)
来源：http://dfm.xylfe.cn

Go:   strings.Join(strs, ", ")
来源：http://auc.cheryme.top

Ruby: arr.join(", ")
来源：http://jlp.hcnkem.com

C#:   string.Join(", ", list)
来源：http://fpo.hnxiangtu.top

================================================================================
来源：http://upm.xziqi.cn

E. 字符串处理
来源：http://jap.nanxuanxn.top

================================================================================
来源：http://ork.sufxvd.cn

[E01] 拼接字符串
来源：http://gsj.chenzaomai.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wff.shanyushiyangtech.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mjg.shuidangran.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://drs.jinqigfzy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sek.jyoumei.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vyz.ywan-chungtsiang.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ydx.0kj1m.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pmh.ywan-chungtsiang.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://uee.zhoulong.xyz

[E02] 重复字符串
来源：http://fsh.snrcjt.cn

Py:   "ab" * 3
来源：http://aql.andypj.xyz

PHP:  str_repeat("ab", 3);
来源：http://ztp.ivvv.top

JS:   "ab".repeat(3)
来源：http://wms.guowangkeji.top


<!-- 参考信息 -->