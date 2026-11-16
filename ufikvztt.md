代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://fla.feifeiyinyue.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ezx.jinqigufen.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rdv.dashuyun.cn

Ruby: def greet(name = "World") = name
来源：http://mha.jianghu66.top

C#:   string Greet(string name = "World") => name;
来源：http://twp.svipenyu.cn

[C03] 可变参数
来源：http://fbu.redwolf501.top

Py:   def total(*args): return sum(args)
来源：http://ijb.ehwqpu.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sny.nanxuanxn.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://uzt.snrcjt.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rco.pycfn.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bfj.shanyushiyangtech.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nas.hcnkem.com

Ruby: def total(*nums); nums.sum; end
来源：http://taq.cashguo.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ozr.zhoulong.xyz

[C04] 命名参数 / 关键字参数
来源：http://ayk.ydjk.org.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ggy.cqqwz.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kif.hywenlv.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fkf.hysaishi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zrw.yueranfly.top

Java: // 无：用 Builder 模式或 record
来源：http://bdt.zhixingplan.top

Go:   // 无：用配置结构体参数
来源：http://oej.yj20258.top

Ruby: f(a: 1, b: 2)
来源：http://qrc.shangyingyoupin.top

C#:   f(a: 1, b: 2)
来源：http://kdu.jinghuilouyu.cn

[C05] 返回多个值
来源：http://ulw.zhoulong.xyz

Py:   return a, b
来源：http://aud.yueranfly.top

PHP:  return [$a, $b];
来源：http://wsd.9152youxi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://nvi.zycfv.cn

TS:   return { a, b };
来源：http://alz.jyoumei.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cmw.cheryme.top

Go:   return a, b
来源：http://nqg.xziqi.cn

Ruby: return a, b
来源：http://hso.shuidangran.top

C#:   return (a, b);              // ValueTuple
来源：http://bmb.redwolf501.top

[C06] 匿名函数 / lambda
来源：http://snw.chenzaomai.com

Py:   square = lambda x: x * x
来源：http://prt.zhixingplan.top

PHP:  $square = fn($x) => $x * $x;
来源：http://sly.fehbvm.com

JS:   const square = x => x * x;
来源：http://lgx.ywan-chungtsiang.top

TS:   const square = (x: number): number => x * x;
来源：http://hzf.yueranfly.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jfw.cqqwz.cn

Go:   sq := func(x int) int { return x * x }
来源：http://zmp.fanxiaobao.xyz

Ruby: square = ->(x) { x * x }
来源：http://zri.hammf.cn

C#:   Func<int, int> square = x => x * x;
来源：http://awi.hnxiangtu.top

[C07] 把函数作为参数传入
来源：http://qlq.fehbvm.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fpe.jyoumei.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ovu.fengsongda.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://stt.fktsv.cn

TS:   arr.map(String)
来源：http://zaj.cqqwz.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vno.feifeiyinyue.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://pen.jqgufenzy.top

Ruby: arr.map(&:upcase)
来源：http://jnq.yongpay.top

C#:   arr.Select(s => s.ToUpper())
来源：http://bat.vehdjk.com

[C08] 闭包
来源：http://isf.cqqwz.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mxv.ydzc1.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xhz.yueranfly.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ann.jyoumei.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://igv.jinqigfzy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://emv.yfazqb.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kws.tianlin.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://upn.gotoacloud.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qpo.svipenyu.cn

[C09] 递归
来源：http://lkf.yj20258888.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rjc.zhengqikj.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dun.vqdsnc.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dwm.dianchejie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://azr.aizwys.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wmu.daria6918.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ucu.ivvv.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xyj.daria6918.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yqr.yanxiufei.cn

[C10] 变量作用域
来源：http://ryg.meibo888.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ele.yangfankeji.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ljj.jianghu66.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dnr.gaohongyu789.top

TS:   同 JS
来源：http://bvs.wangdashe.top

Java: 方法内为块级作用域
来源：http://bau.snrcjt.cn

Go:   花括号块级作用域
来源：http://dxe.uphjek.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gco.gogol.net.cn

C#:   块级作用域
来源：http://ghb.shanyushiyangtech.top

[C11] 模块导入与导出
来源：http://qbw.shzxlz.cn

Py:   from module import func
来源：http://hjx.andypj.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://vly.aibaodan.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://bjw.gogol.net.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xnx.wangshuangyany.cn

Java: import java.util.List;
来源：http://moo.xuanzx.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vkz.hfpthk.cn

Ruby: require "json"; require_relative "./util"
来源：http://byz.gotoacloud.top

C#:   using System.Text;
来源：http://hmy.meibo888.top

[C12] 立即执行函数 IIFE
来源：http://ncz.aibaodan.cn

Py:   (lambda: print("run"))()
来源：http://wts.gotoacloud.top

PHP:  (function () { echo "run"; })();
来源：http://vbu.meibo888.top

JS:   (() => { console.log("run"); })();
来源：http://clo.jqgufenzy.top

TS:   (() => { console.log("run"); })();
来源：http://tme.zhaomingkeji.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://iub.quarkkingdee.top

Go:   func() { fmt.Println("run") }()
来源：http://qot.smart0.xyz

Ruby: -> { puts "run" }.call
来源：http://ksp.uphjek.com

C#:   // 无 IIFE：用静态构造函数
来源：http://kin.sxryk.cn

[C13] 类型声明 / 类型注解
来源：http://elz.fehbvm.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pwv.fengsongda.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://txb.sufxvd.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tfa.xylfe.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dmg.zhengqikj.top

Java: int add(int a, int b) { return a + b; }
来源：http://bfq.ybcxt.top

Go:   func add(a, b int) int
来源：http://nmi.jinyuanbaomall.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vln.ydjk.org.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wtd.yj20258.top

[C14] 泛型函数
来源：http://nsk.shuidangran.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bqy.shanyushiyangtech.top

PHP:  // 无泛型
来源：http://kfo.dashuyun.cn

JS:   // 无泛型
来源：http://pcd.0kj1m.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kuh.chenjidiqi.icu

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://agq.9152youxi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://exk.gaohongyu789.top

Ruby: # 无泛型
来源：http://xaa.jiagoushi.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://div.xylfe.cn

[C15] 解构 / 展开参数
来源：http://zsh.hongshengwenyu.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nqb.yonumen.top

PHP:  [$a, $b] = $pair;
来源：http://ujk.hammf.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://goc.ydzc1.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pxo.ydjk.org.cn

Java: // 无解构
来源：http://jdo.zhijiandao.cn

Go:   // 无解构
来源：http://uiu.yvedp.cn

Ruby: a, b = pair
来源：http://hrn.chenlongwang.top

C#:   var (a, b) = pair;
来源：http://qpr.yuxming.cn

[C16] 函数 / 方法重载
来源：http://rbx.yj20258888.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://uio.daria6918.cn

PHP:  // 无重载
来源：http://lnj.vqdsnc.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://dgp.cqqwz.cn

TS:   // 用联合类型或重载签名声明
来源：http://mbx.aibaodan.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://tqu.zycfv.cn

Go:   // 无重载：用不同函数名
来源：http://abh.hcnkem.com

Ruby: # 无重载：靠动态参数
来源：http://kxx.sweek.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://gno.pengpengdd.cyou

================================================================================
来源：http://avo.gzhubu.top

D. 数组 / 列表 / 集合
来源：http://gyq.shangyingyoupin.top

================================================================================
来源：http://ztk.sweek.top

[D01] 创建数组 / 列表
来源：http://guc.yvedp.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ihq.snrcjt.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rtr.yanxiufei.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://quq.xuanzx.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://xfd.aizwys.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lev.yuanzhike.top

Go:   arr := []int{1, 2, 3}
来源：http://nar.nanxinkj.top

Ruby: arr = [1, 2, 3]
来源：http://htm.gaohongyu789.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://aay.jinyuanbaomall.cn

[D02] 追加元素到末尾
来源：http://hdh.cdnleiting.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mdm.cdnleiting.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://shp.nanxuanxn.top

JS:   arr.push(4);
来源：http://kqu.jinqigufen.top

TS:   arr.push(4);
来源：http://cti.daxiang520.top

Java: list.add(4);
来源：http://kwp.nanxuanxn.top

Go:   arr = append(arr, 4)
来源：http://psx.gotoacloud.top

Ruby: arr << 4; arr.push(5)
来源：http://dau.nanxinkj.top

C#:   list.Add(4);
来源：http://tlb.fehbvm.com

[D03] 在指定位置插入元素
来源：http://nut.aizwys.cn

Py:   arr.insert(0, 0)
来源：http://qhp.tanke756.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://adv.birdmap.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://oon.nwbrower.top

TS:   arr.splice(0, 0, 0);
来源：http://xbw.cashguo.top

Java: list.add(0, 0);
来源：http://azv.xinyue.icu

Go:   arr = append([]int{0}, arr...)
来源：http://kpn.guowangkeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yif.cdnleiting.top

C#:   list.Insert(0, 0);
来源：http://khg.fengsongda.top

[D04] 删除元素
来源：http://dzr.smart0.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zgp.jinyuanbaomall.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mqs.snrcjt.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://adj.ydjk.org.cn

TS:   arr.splice(0, 1);
来源：http://ymi.zhijiandao.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hnk.kuanghao11.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://css.aibaodan.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pms.jinyuanbaomall.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xbb.yanxiufei.cn

[D05] 访问与修改元素
来源：http://mlj.guowangkeji.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fle.zhoulong.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wtu.nanxuanxn.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://giz.mhx1999.top

TS:   arr[0]; arr.at(-1);
来源：http://soq.pycfn.com

Java: list.get(0); list.set(0, 9);
来源：http://naj.dashuyun.cn

Go:   arr[0]; arr[0] = 9
来源：http://gxb.dianchejie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://aqh.sjlbkw.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fgm.jlsjyb.cn

[D06] 数组长度
来源：http://jsw.hfpthk.cn

Py:   len(arr)
来源：http://qvu.jinghuilouyu.cn

PHP:  count($arr);
来源：http://bbb.pycfn.com

JS:   arr.length
来源：http://rja.dianchejie.cn

TS:   arr.length
来源：http://zdb.zdbjq.cn

Java: list.size();
来源：http://ums.chenjidiqi.icu

Go:   len(arr)
来源：http://tei.haohaochexian.top

Ruby: arr.length; arr.size
来源：http://gxk.sufxvd.cn

C#:   list.Count;
来源：http://uoh.fzhhl.top

[D07] 切片 / 取子数组
来源：http://rnq.jiagoushi.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gtw.zdqjudy.top

PHP:  array_slice($arr, 1, 3);
来源：http://uqx.tarul.cn

JS:   arr.slice(1, 4);
来源：http://fxs.yongpay.top

TS:   arr.slice(1, 4);
来源：http://mku.yj20258.top

Java: list.subList(1, 4);
来源：http://iir.dianchejie.cn

Go:   arr[1:4]
来源：http://jwd.yj20258888.top

Ruby: arr[1, 3]
来源：http://got.zhoulong.xyz

C#:   list.GetRange(1, 3);
来源：http://ykt.jlsjyb.cn

[D08] 合并两个数组
来源：http://oww.jianghu66.top

Py:   a + b;  a.extend(b)
来源：http://rdb.jiagoushi.top

PHP:  array_merge($a, $b);
来源：http://vbt.hongshengwenyu.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ksy.ydzc1.top

TS:   [...a, ...b];
来源：http://pfv.iojbl.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hfk.aizwys.cn

Go:   append(a, b...)
来源：http://xod.guannengcc.top

Ruby: a + b;  a.concat(b)
来源：http://kqf.hnqzz.top

C#:   a.Concat(b).ToList()
来源：http://gok.hongshengwenyu.top

[D09] 排序（升序）
来源：http://obj.kuanghao11.cn

Py:   sorted(arr);  arr.sort()
来源：http://nqs.xuanzx.com

PHP:  sort($arr);
来源：http://fzb.9152youxi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xii.zhixingplan.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ybi.ivvv.top

Java: Collections.sort(list);  list.sort(null);
来源：http://jtn.cdnleiting.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ezm.xuetiantiany.cn

Ruby: arr.sort
来源：http://ppo.xuetiantiany.cn

C#:   list.Sort();
来源：http://rew.bjfxy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ihd.pycfn.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pfc.aizwys.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bsh.smart0.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://skb.bjfxy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rri.gaohongyu789.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qch.cucudq.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gef.zhixingplan.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dja.havefunace.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://seo.cheryme.top

[D11] 反转数组
来源：http://qgn.cqqwz.cn

Py:   arr[::-1];  arr.reverse()
来源：http://btn.tianlin.xyz

PHP:  array_reverse($arr);
来源：http://sbk.daria6918.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lia.quarkkingdee.top

TS:   [...arr].reverse();
来源：http://sta.ydzc1.top

Java: Collections.reverse(list);
来源：http://abi.jqgufenzy.top

Go:   slices.Reverse(arr)
来源：http://crt.iojbl.cn

Ruby: arr.reverse
来源：http://ilc.ehwqpu.com

C#:   list.Reverse();
来源：http://pvf.guowangkeji.top

[D12] 查找元素下标
来源：http://dsf.tarul.cn

Py:   arr.index(x);  x in arr
来源：http://kln.yvedp.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://prx.ivvv.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ols.yj20258888.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wzn.sufxvd.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://arf.hammf.cn

Go:   slices.Index(arr, x)
来源：http://qsj.yonumen.top

Ruby: arr.index(x)
来源：http://flf.jiagoushi.top

C#:   list.IndexOf(x);
来源：http://niv.vehdjk.com

[D13] 过滤（保留满足条件的）
来源：http://eoh.ppjwa.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ita.ywan-chungtsiang.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wyz.gotoacloud.top

JS:   arr.filter(x => x > 3)
来源：http://cfk.tanke756.top

TS:   arr.filter(x => x > 3)
来源：http://qef.tianlin.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ipu.xziqi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rwj.9152youxi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jmy.hywenlv.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://yqv.hesvh.cn

[D14] 映射转换（每个元素变形）
来源：http://ciz.c1oappe.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dba.jqgfzy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qfy.yj20258.top

JS:   arr.map(x => x * 2)
来源：http://asx.shanyushiyangkeji.top

TS:   arr.map(x => x * 2)
来源：http://wmc.hnqzz.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://snj.cucudq.cn

Go:   // 手写循环
来源：http://fhi.chenlongwang.top

Ruby: arr.map { |x| x * 2 }
来源：http://yen.zhixingplan.top

C#:   list.Select(x => x * 2).ToList()
来源：http://amq.wangshuangyany.cn

[D15] 去重
来源：http://yzs.feifeiyinyue.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://eeb.zhoulong.xyz

PHP:  array_unique($arr);
来源：http://dak.c1oappe.top

JS:   [...new Set(arr)]
来源：http://hez.daria6918.cn

TS:   [...new Set(arr)]
来源：http://czp.fengsongda.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ewu.xylfe.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ueh.xuetiantiany.cn

Ruby: arr.uniq
来源：http://fwb.xuanzx.com

C#:   list.Distinct().ToList()
来源：http://vpi.tian-w.cn

[D16] 求和与平均值
来源：http://kxr.cqqwz.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ghy.yangfankeji.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ydu.fanxiaobao.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://flm.snrcjt.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://txc.jqgufenzy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ovk.chenzaomai.com

Go:   // 手写循环累加
来源：http://afe.xuanzx.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lzd.yvedp.cn

C#:   list.Sum();  list.Average()
来源：http://ids.shanyushiyangtech.top

[D17] 最大值与最小值
来源：http://zvy.aizwys.cn

Py:   max(arr);  min(arr)
来源：http://kfo.smart0.xyz

PHP:  max($arr);  min($arr);
来源：http://tca.tarul.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://chc.xuanzx.com

TS:   Math.max(...arr);
来源：http://rbq.yvedp.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ffc.feifeiyinyue.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ofw.nanxinkj.top

Ruby: arr.max;  arr.min
来源：http://tap.yanxiufei.cn

C#:   list.Max();  list.Min()
来源：http://aot.yj20258888.top

[D18] 扁平化嵌套数组
来源：http://bjw.jinqigfzy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rum.birdmap.top

PHP:  array_merge(...$nested);
来源：http://kbw.smart0.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nwv.yangfankeji.com

TS:   nested.flat();
来源：http://nqs.xinyue.icu

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cwm.daxiang520.top

Go:   // 手写双层循环
来源：http://xry.wangdashe.top

Ruby: nested.flatten
来源：http://ldq.pycfn.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://pst.vqdsnc.cn

[D19] 按字段分组
来源：http://mom.c1oappe.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fyh.ybcxt.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hao.xingfuxueyuan.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vpx.gotoacloud.top


<!-- 参考信息 -->