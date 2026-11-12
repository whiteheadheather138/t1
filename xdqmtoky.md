代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://zft.jyoumei.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bfj.pycfn.com

Go:   sq := func(x int) int { return x * x }
来源：http://iyz.yuanzhike.top

Ruby: square = ->(x) { x * x }
来源：http://dbp.cheryme.top

C#:   Func<int, int> square = x => x * x;
来源：http://sge.52xcode.cn

[C07] 把函数作为参数传入
来源：http://tmm.xingfuxueyuan.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nxd.fktsv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jus.tanke756.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://imc.cdnleiting.top

TS:   arr.map(String)
来源：http://elu.hesvh.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nln.aizwys.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jug.c1oappe.top

Ruby: arr.map(&:upcase)
来源：http://dxz.andypj.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://imx.jyoumei.cn

[C08] 闭包
来源：http://ukn.jianghu66.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uqg.pengpengdd.cyou

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vfn.jqgufenzy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kxp.hongshengwenyu.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fpg.chenjidiqi.icu

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xab.quarkkingdee.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lya.hammf.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kni.gzhubu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dye.andypj.xyz

[C09] 递归
来源：http://aqg.ydjk.org.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dru.hammf.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gmw.xylfe.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wfs.yfazqb.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qup.vqdsnc.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://eri.nanxuanxn.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hrd.zhixingplan.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jan.fengsongda.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pgp.xylfe.cn

[C10] 变量作用域
来源：http://xjv.gaohongyu789.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rma.meibo888.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xta.bbcook.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qva.chenzaomai.com

TS:   同 JS
来源：http://fvf.cucudq.cn

Java: 方法内为块级作用域
来源：http://ags.yuxming.cn

Go:   花括号块级作用域
来源：http://lfh.aibaodan.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ste.hysaishi.cn

C#:   块级作用域
来源：http://bps.haohaochexian.top

[C11] 模块导入与导出
来源：http://ipo.guowangkeji.top

Py:   from module import func
来源：http://skx.daxiang520.top

PHP:  require "file.php";  或 use App\Service;
来源：http://yaa.fanxiaobao.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://fbj.c1oappe.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ina.feifeiyinyue.top

Java: import java.util.List;
来源：http://aaf.zhaomingkeji.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tvb.jyoumei.cn

Ruby: require "json"; require_relative "./util"
来源：http://zja.daxiang520.top

C#:   using System.Text;
来源：http://wqc.chenjidiqi.icu

[C12] 立即执行函数 IIFE
来源：http://qic.svipenyu.cn

Py:   (lambda: print("run"))()
来源：http://meq.cdnleiting.top

PHP:  (function () { echo "run"; })();
来源：http://icb.hnxiangtu.top

JS:   (() => { console.log("run"); })();
来源：http://chc.jlsjyb.cn

TS:   (() => { console.log("run"); })();
来源：http://dip.svipenyu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tdq.yj202588.top

Go:   func() { fmt.Println("run") }()
来源：http://car.zdqjudy.top

Ruby: -> { puts "run" }.call
来源：http://zka.ppjwa.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://nuj.gotoacloud.top

[C13] 类型声明 / 类型注解
来源：http://bna.yonumen.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://see.wangdashe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hou.mhx1999.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://chv.ivvv.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://akg.jinqigfzy.top

Java: int add(int a, int b) { return a + b; }
来源：http://fcz.sxryk.cn

Go:   func add(a, b int) int
来源：http://gjy.smart0.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://iwc.xingfuxueyuan.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://mrq.jianghu66.top

[C14] 泛型函数
来源：http://abo.uphjek.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xxb.jlsjyb.cn

PHP:  // 无泛型
来源：http://nnt.nanxinkj.top

JS:   // 无泛型
来源：http://mih.jinyuanbaomall.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ztu.dianchejie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ita.nanxuanxn.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://iod.jlsjyb.cn

Ruby: # 无泛型
来源：http://qfq.jinghuilouyu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ncc.316326.xyz

[C15] 解构 / 展开参数
来源：http://kce.daxiang520.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kxg.xylfe.cn

PHP:  [$a, $b] = $pair;
来源：http://bcu.ydzc1.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rqa.fktsv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://axu.jianghu66.top

Java: // 无解构
来源：http://ylr.yonumen.top

Go:   // 无解构
来源：http://ppa.ywan-chungtsiang.top

Ruby: a, b = pair
来源：http://fxo.shuidangran.top

C#:   var (a, b) = pair;
来源：http://aqe.wangshuangyany.cn

[C16] 函数 / 方法重载
来源：http://jtt.jiagoushi.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yra.yuanzhike.top

PHP:  // 无重载
来源：http://ksm.daxiang520.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://jtw.ybcxt.top

TS:   // 用联合类型或重载签名声明
来源：http://tfz.yonumen.top

Java: void f(int a) {}  void f(String a) {}
来源：http://moy.chenlongwang.top

Go:   // 无重载：用不同函数名
来源：http://zbw.yj202588.top

Ruby: # 无重载：靠动态参数
来源：http://icp.xuetiantiany.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://mhb.xylfe.cn

================================================================================
来源：http://tvq.xuetiantiany.cn

D. 数组 / 列表 / 集合
来源：http://vre.vehdjk.com

================================================================================
来源：http://gka.shuidangran.top

[D01] 创建数组 / 列表
来源：http://rhx.ydjk.org.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ujo.hcnkem.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jqb.xingfuxueyuan.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wgf.hongshengwenyu.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ves.hongshengwenyu.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sxa.uphjek.com

Go:   arr := []int{1, 2, 3}
来源：http://qvi.shangyingyoupin.top

Ruby: arr = [1, 2, 3]
来源：http://gxv.bjfxy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fbx.ydzc1.top

[D02] 追加元素到末尾
来源：http://pod.redwolf501.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://oor.andypj.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ozs.cdnleiting.top

JS:   arr.push(4);
来源：http://iao.wangshuangyany.cn

TS:   arr.push(4);
来源：http://epp.ybcxt.top

Java: list.add(4);
来源：http://euq.hesvh.cn

Go:   arr = append(arr, 4)
来源：http://zow.hongshengwenyu.top

Ruby: arr << 4; arr.push(5)
来源：http://gnb.xuetiantiany.cn

C#:   list.Add(4);
来源：http://lnc.gotoacloud.top

[D03] 在指定位置插入元素
来源：http://kmd.jyoumei.cn

Py:   arr.insert(0, 0)
来源：http://rfy.gaohongyu789.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dmc.shzxlz.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://biy.yfazqb.com

TS:   arr.splice(0, 0, 0);
来源：http://eya.yj202588.top

Java: list.add(0, 0);
来源：http://igc.hfpthk.cn

Go:   arr = append([]int{0}, arr...)
来源：http://myu.shangyingyoupin.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dyb.jianghu66.top

C#:   list.Insert(0, 0);
来源：http://xjx.hnxiangtu.top

[D04] 删除元素
来源：http://igm.fzhhl.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bnu.xziqi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jpo.yj202588.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uuf.shuidangran.top

TS:   arr.splice(0, 1);
来源：http://nek.fehbvm.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lou.dashuyun.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://anj.jlsjyb.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wvs.hammf.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qus.sxryk.cn

[D05] 访问与修改元素
来源：http://pac.pengpengdd.cyou

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rhz.quarkkingdee.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://imo.pengpengdd.cyou

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kvk.yuxming.cn

TS:   arr[0]; arr.at(-1);
来源：http://qut.quarkkingdee.top

Java: list.get(0); list.set(0, 9);
来源：http://wqa.fanxiaobao.xyz

Go:   arr[0]; arr[0] = 9
来源：http://jln.ydzc1.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ixo.zhaomingkeji.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hyo.nanxinkj.top

[D06] 数组长度
来源：http://doz.kuanghao11.cn

Py:   len(arr)
来源：http://agl.jqgfzy.top

PHP:  count($arr);
来源：http://mtg.zhixingplan.top

JS:   arr.length
来源：http://wil.havefunace.top

TS:   arr.length
来源：http://svc.hnqzz.top

Java: list.size();
来源：http://ypl.hnxiangtu.top

Go:   len(arr)
来源：http://hys.dianchejie.cn

Ruby: arr.length; arr.size
来源：http://squ.zdbjq.cn

C#:   list.Count;
来源：http://gdo.yuanzhike.top

[D07] 切片 / 取子数组
来源：http://wfo.shuidangran.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://sxi.xinyue.icu

PHP:  array_slice($arr, 1, 3);
来源：http://cbk.yj20258.top

JS:   arr.slice(1, 4);
来源：http://jqm.dianchejie.cn

TS:   arr.slice(1, 4);
来源：http://nrh.ydjk.org.cn

Java: list.subList(1, 4);
来源：http://qdw.zdbjq.cn

Go:   arr[1:4]
来源：http://mue.mhx1999.top

Ruby: arr[1, 3]
来源：http://dlm.zhengqikj.top

C#:   list.GetRange(1, 3);
来源：http://nqm.hysaishi.cn

[D08] 合并两个数组
来源：http://gqt.sysykeji.top

Py:   a + b;  a.extend(b)
来源：http://vhc.guannengcc.top

PHP:  array_merge($a, $b);
来源：http://gij.aizwys.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://jri.yongpay.top

TS:   [...a, ...b];
来源：http://nsb.zhijiandao.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sbk.chenlongwang.top

Go:   append(a, b...)
来源：http://vox.ppjwa.cn

Ruby: a + b;  a.concat(b)
来源：http://grd.hywenlv.cn

C#:   a.Concat(b).ToList()
来源：http://wju.cdnleiting.top

[D09] 排序（升序）
来源：http://bqi.xuetiantiany.cn

Py:   sorted(arr);  arr.sort()
来源：http://vde.xuetiantiany.cn

PHP:  sort($arr);
来源：http://olf.cucudq.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nwe.pengpengdd.cyou

TS:   [...arr].sort((x, y) => x - y);
来源：http://ufh.hysaishi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://jqz.nwbrower.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yfc.zhoulong.xyz

Ruby: arr.sort
来源：http://wed.tianlin.xyz

C#:   list.Sort();
来源：http://yom.daxiang520.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://fvm.vqdsnc.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ztj.zhijiandao.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mxv.xinyue.icu

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vdi.yuxming.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wzc.yueranfly.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ezl.hysaishi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qwc.jinghuilouyu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ywn.nanxuanxn.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kpb.cdnleiting.top

[D11] 反转数组
来源：http://nxe.yj20258.top

Py:   arr[::-1];  arr.reverse()
来源：http://tqx.havefunace.top

PHP:  array_reverse($arr);
来源：http://zid.birdmap.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://klh.0kj1m.cn

TS:   [...arr].reverse();
来源：http://jsn.sweek.top

Java: Collections.reverse(list);
来源：http://lfj.smart0.xyz

Go:   slices.Reverse(arr)
来源：http://fkx.zhixingplan.top

Ruby: arr.reverse
来源：http://xke.vqdsnc.cn

C#:   list.Reverse();
来源：http://zbk.vehdjk.com

[D12] 查找元素下标
来源：http://pwt.aibaodan.cn

Py:   arr.index(x);  x in arr
来源：http://wvl.feifeiyinyue.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dyt.zdbjq.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lze.sweek.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://utq.zhongyouzk.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://szp.hongshengwenyu.top

Go:   slices.Index(arr, x)
来源：http://yjh.ywan-chungtsiang.top

Ruby: arr.index(x)
来源：http://vhq.dianchejie.cn

C#:   list.IndexOf(x);
来源：http://gau.yj202588.top

[D13] 过滤（保留满足条件的）
来源：http://oee.shanyushiyangkeji.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qmr.zdbjq.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vdn.fehbvm.com

JS:   arr.filter(x => x > 3)
来源：http://qab.zhengqikj.top

TS:   arr.filter(x => x > 3)
来源：http://dux.svipenyu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fnj.chenlongwang.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://njs.hnqzz.top

Ruby: arr.select { |x| x > 3 }
来源：http://tbf.shanyushiyangkeji.top

C#:   list.Where(x => x > 3).ToList()
来源：http://alw.ppjwa.cn

[D14] 映射转换（每个元素变形）
来源：http://fkr.dashuyun.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yvm.hnqzz.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jks.hfpthk.cn

JS:   arr.map(x => x * 2)
来源：http://ode.xuetiantiany.cn

TS:   arr.map(x => x * 2)
来源：http://tkc.mhx1999.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://qoy.shanyushiyangtech.top

Go:   // 手写循环
来源：http://suv.redwolf501.top

Ruby: arr.map { |x| x * 2 }
来源：http://gnz.nanxuanxn.top

C#:   list.Select(x => x * 2).ToList()
来源：http://mbh.jqgfzy.top

[D15] 去重
来源：http://skz.yvedp.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vpq.hnqzz.top

PHP:  array_unique($arr);
来源：http://ikh.shanyushiyangkeji.top

JS:   [...new Set(arr)]
来源：http://euo.zhixingplan.top

TS:   [...new Set(arr)]
来源：http://uuq.mhx1999.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bdy.52xcode.cn

Go:   // 用 map[T]struct{} 手写
来源：http://tcl.jinqigufen.top

Ruby: arr.uniq
来源：http://hee.shangyingyoupin.top

C#:   list.Distinct().ToList()
来源：http://ujw.hysaishi.cn

[D16] 求和与平均值
来源：http://uwb.hnxiangtu.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xta.sjlbkw.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://iey.chenzaomai.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nxe.hywenlv.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://obu.yanxiufei.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mjd.yvedp.cn

Go:   // 手写循环累加
来源：http://rzg.ivvv.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dkt.ctjpmb.com

C#:   list.Sum();  list.Average()
来源：http://xdv.hnxiangtu.top

[D17] 最大值与最小值
来源：http://gtr.guowangkeji.top

Py:   max(arr);  min(arr)
来源：http://gwj.mhx1999.top

PHP:  max($arr);  min($arr);
来源：http://jsl.wangdashe.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://aer.guowangkeji.top

TS:   Math.max(...arr);
来源：http://wmi.aizwys.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://tcy.birdmap.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://sia.hammf.cn

Ruby: arr.max;  arr.min
来源：http://szq.chenjidiqi.icu

C#:   list.Max();  list.Min()
来源：http://wyy.zhoulong.xyz

[D18] 扁平化嵌套数组
来源：http://luw.tian-w.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zkq.jinghuilouyu.cn

PHP:  array_merge(...$nested);
来源：http://mmp.hfpthk.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kej.xingfuxueyuan.xyz

TS:   nested.flat();
来源：http://rof.fanxiaobao.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gzj.dashuyun.cn

Go:   // 手写双层循环
来源：http://dhe.zdqjudy.top

Ruby: nested.flatten
来源：http://fxr.yueranfly.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://cvs.ehwqpu.com

[D19] 按字段分组
来源：http://ifb.jiagoushi.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tfw.52xcode.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mzb.ctjpmb.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://htj.jiagoushi.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ghb.xuanzx.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yyl.nanxuanxn.top

Go:   // 手写 map[string][]T
来源：http://fgf.mhx1999.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://siv.chenjidiqi.icu

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://sqz.daria6918.cn

[D20] 统计每个元素出现次数
来源：http://arv.shanyushiyangtech.top

Py:   Counter(arr)
来源：http://xgx.yvedp.cn

PHP:  array_count_values($arr);
来源：http://uzu.yonumen.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wbm.hcnkem.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ujm.yvedp.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ezo.haohaochexian.top

Go:   // 手写 map[T]int
来源：http://mup.zdbjq.cn

Ruby: arr.tally
来源：http://hje.xuanzx.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://oeb.yvedp.cn

[D21] 判断是否包含某元素
来源：http://hwb.yfazqb.com

Py:   x in arr
来源：http://gfi.yongpay.top

PHP:  in_array($x, $arr, true);
来源：http://yjl.jiagoushi.top

JS:   arr.includes(x)
来源：http://bbh.wangdashe.top

TS:   arr.includes(x)
来源：http://pcx.zhijiandao.cn

Java: list.contains(x)
来源：http://zpd.yueranfly.top

Go:   slices.Contains(arr, x)
来源：http://eox.cheryme.top

Ruby: arr.include?(x)
来源：http://avu.jianghu66.top

C#:   list.Contains(x)
来源：http://jfn.shuidangran.top

[D22] 复制数组（避免共享引用）
来源：http://ipk.epnwcf.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://evg.hnxiangtu.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pkf.yangfankeji.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ncu.0kj1m.cn

TS:   [...arr];
来源：http://ige.zdbjq.cn

Java: new ArrayList<>(list);
来源：http://ror.ybcxt.top

Go:   copied := append([]int(nil), arr...)
来源：http://ibn.ppjwa.cn

Ruby: arr.dup;  arr.clone
来源：http://exi.jinyuanbaomall.cn

C#:   new List<int>(list);
来源：http://ylh.jinqigufen.top

[D23] reduce 累积计算
来源：http://zlr.daxiang520.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gpx.zhaomingkeji.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://aeh.zdbjq.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lth.quarkkingdee.top


<!-- 参考信息 -->