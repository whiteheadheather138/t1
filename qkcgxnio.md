代发 wailian999

Py:   return a, b
来源：http://sde.tanke756.top

PHP:  return [$a, $b];
来源：http://zcb.smart0.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://zap.yj20258888.top

TS:   return { a, b };
来源：http://sxh.tianlin.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pio.cheryme.top

Go:   return a, b
来源：http://gkp.hcnkem.com

Ruby: return a, b
来源：http://mhz.dianchejie.cn

C#:   return (a, b);              // ValueTuple
来源：http://wlx.hnxiangtu.top

[C06] 匿名函数 / lambda
来源：http://huo.yueranfly.top

Py:   square = lambda x: x * x
来源：http://pvs.bbcook.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fgc.yj202588.top

JS:   const square = x => x * x;
来源：http://gha.zhaomingkeji.xyz

TS:   const square = (x: number): number => x * x;
来源：http://wlt.0kj1m.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://aln.zhongyouzk.top

Go:   sq := func(x int) int { return x * x }
来源：http://hky.mhx1999.top

Ruby: square = ->(x) { x * x }
来源：http://rpn.zycfv.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zap.aizwys.cn

[C07] 把函数作为参数传入
来源：http://kwu.hnqzz.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ysh.hnxiangtu.top

PHP:  array_map("strtoupper", $arr);
来源：http://kmr.pengpengdd.cyou

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://guu.zhengqikj.top

TS:   arr.map(String)
来源：http://lbp.smart0.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yyn.hammf.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://crc.pengpengdd.cyou

Ruby: arr.map(&:upcase)
来源：http://edp.zhaomingkeji.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://zzt.52xcode.cn

[C08] 闭包
来源：http://qty.dianchejie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zux.jqgfzy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pea.52xcode.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gwd.quarkkingdee.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fte.zhixingplan.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xvu.wangshuangyany.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://oac.quarkkingdee.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tmu.redwolf501.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qwi.gogol.net.cn

[C09] 递归
来源：http://ulw.wangdashe.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xjx.jiagoushi.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://twb.cqqwz.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://til.xinyue.icu

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mkq.haohaochexian.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qnz.hesvh.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://haf.jlsjyb.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://oed.hnxiangtu.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uuk.hnxiangtu.top

[C10] 变量作用域
来源：http://qlf.yvedp.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lxu.daxiang520.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://iqs.zycfv.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hme.chenjidiqi.icu

TS:   同 JS
来源：http://lln.andypj.xyz

Java: 方法内为块级作用域
来源：http://vty.yj20258888.top

Go:   花括号块级作用域
来源：http://qhk.yonumen.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://csg.zhiwuduotai.top

C#:   块级作用域
来源：http://nka.jqgfzy.top

[C11] 模块导入与导出
来源：http://soq.sysykeji.top

Py:   from module import func
来源：http://tjq.shzxlz.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://oou.yueranfly.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://mpo.sweek.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rwf.tian-w.cn

Java: import java.util.List;
来源：http://hph.yuanzhike.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kgd.gzhubu.top

Ruby: require "json"; require_relative "./util"
来源：http://irm.yonumen.top

C#:   using System.Text;
来源：http://ial.feifeiyinyue.top

[C12] 立即执行函数 IIFE
来源：http://eou.chenlongwang.top

Py:   (lambda: print("run"))()
来源：http://znw.jqgfzy.top

PHP:  (function () { echo "run"; })();
来源：http://ufe.zhixingplan.top

JS:   (() => { console.log("run"); })();
来源：http://cdk.ydzc1.top

TS:   (() => { console.log("run"); })();
来源：http://rmr.sufxvd.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kgx.daria6918.cn

Go:   func() { fmt.Println("run") }()
来源：http://fnq.hysaishi.cn

Ruby: -> { puts "run" }.call
来源：http://dsc.guannengcc.top

C#:   // 无 IIFE：用静态构造函数
来源：http://hmq.xingfuxueyuan.xyz

[C13] 类型声明 / 类型注解
来源：http://ybc.xylfe.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://drm.sjlbkw.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rxo.sysykeji.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mbx.sxryk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wpq.xuanzx.com

Java: int add(int a, int b) { return a + b; }
来源：http://yef.daxiang520.top

Go:   func add(a, b int) int
来源：http://xvg.jqgufenzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vbc.wangshuangyany.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xod.zhoulong.xyz

[C14] 泛型函数
来源：http://ckd.hesvh.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mre.ydjk.org.cn

PHP:  // 无泛型
来源：http://hzy.shuidangran.top

JS:   // 无泛型
来源：http://xxz.tarul.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ipw.zhengqikj.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://iny.gzhubu.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mmk.ydjk.org.cn

Ruby: # 无泛型
来源：http://afy.yongpay.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tqx.c1oappe.top

[C15] 解构 / 展开参数
来源：http://hmn.yangfankeji.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zct.smart0.xyz

PHP:  [$a, $b] = $pair;
来源：http://pgk.sysykeji.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rrf.ppjwa.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xgl.vqdsnc.cn

Java: // 无解构
来源：http://uhc.jianghu66.top

Go:   // 无解构
来源：http://fxy.yanxiufei.cn

Ruby: a, b = pair
来源：http://dwo.zhengqikj.top

C#:   var (a, b) = pair;
来源：http://zjn.xziqi.cn

[C16] 函数 / 方法重载
来源：http://ouj.guowangkeji.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lrv.sufxvd.cn

PHP:  // 无重载
来源：http://nbs.jianghu66.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://wfc.uphjek.com

TS:   // 用联合类型或重载签名声明
来源：http://mng.shuidangran.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ipo.yj20258888.top

Go:   // 无重载：用不同函数名
来源：http://hfy.yuxming.cn

Ruby: # 无重载：靠动态参数
来源：http://pfj.nanxuanxn.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://uyw.hysaishi.cn

================================================================================
来源：http://vbj.xuanzx.com

D. 数组 / 列表 / 集合
来源：http://qol.dianchejie.cn

================================================================================
来源：http://mos.zycfv.cn

[D01] 创建数组 / 列表
来源：http://nzo.jinghuilouyu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zak.chenzaomai.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mpc.c1oappe.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ybm.chenzaomai.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://udl.bbcook.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jsj.xylfe.cn

Go:   arr := []int{1, 2, 3}
来源：http://qbi.zhijiandao.cn

Ruby: arr = [1, 2, 3]
来源：http://kps.nanxinkj.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nyj.316326.xyz

[D02] 追加元素到末尾
来源：http://rxo.cqqwz.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://btm.wangshuangyany.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qzt.fehbvm.com

JS:   arr.push(4);
来源：http://mbx.aizwys.cn

TS:   arr.push(4);
来源：http://wlq.yonumen.top

Java: list.add(4);
来源：http://wii.birdmap.top

Go:   arr = append(arr, 4)
来源：http://xww.jinghuilouyu.cn

Ruby: arr << 4; arr.push(5)
来源：http://ogm.jiagoushi.top

C#:   list.Add(4);
来源：http://xmo.guannengcc.top

[D03] 在指定位置插入元素
来源：http://yri.ywan-chungtsiang.top

Py:   arr.insert(0, 0)
来源：http://hcc.shuidangran.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nvh.ywan-chungtsiang.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://eic.nanxuanxn.top

TS:   arr.splice(0, 0, 0);
来源：http://kvr.yueranfly.top

Java: list.add(0, 0);
来源：http://lim.yvedp.cn

Go:   arr = append([]int{0}, arr...)
来源：http://giq.xuetiantiany.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ttz.hywenlv.cn

C#:   list.Insert(0, 0);
来源：http://eka.cqqwz.cn

[D04] 删除元素
来源：http://otj.svipenyu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://azl.zdqjudy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qlq.yvedp.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qxx.havefunace.top

TS:   arr.splice(0, 1);
来源：http://nmd.jyoumei.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lrk.hfpthk.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uoa.jinyuanbaomall.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ecd.jinqigfzy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fmi.hammf.cn

[D05] 访问与修改元素
来源：http://mvb.sjlbkw.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://eov.jinyuanbaomall.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://upc.bjfxy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zyz.cdnleiting.top

TS:   arr[0]; arr.at(-1);
来源：http://eoi.gaohongyu789.top

Java: list.get(0); list.set(0, 9);
来源：http://dbc.havefunace.top

Go:   arr[0]; arr[0] = 9
来源：http://mvt.zhengqikj.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xgb.aibaodan.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cgv.jianghu66.top

[D06] 数组长度
来源：http://qdd.kuanghao11.cn

Py:   len(arr)
来源：http://yoq.shuidangran.top

PHP:  count($arr);
来源：http://zdq.fehbvm.com

JS:   arr.length
来源：http://xwn.zdbjq.cn

TS:   arr.length
来源：http://fkf.xziqi.cn

Java: list.size();
来源：http://mdz.jinyuanbaomall.cn

Go:   len(arr)
来源：http://bsg.andypj.xyz

Ruby: arr.length; arr.size
来源：http://kvv.ywan-chungtsiang.top

C#:   list.Count;
来源：http://fqb.ivvv.top

[D07] 切片 / 取子数组
来源：http://wnj.0kj1m.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lut.tanke756.top

PHP:  array_slice($arr, 1, 3);
来源：http://fiy.0kj1m.cn

JS:   arr.slice(1, 4);
来源：http://kfd.jinyuanbaomall.cn

TS:   arr.slice(1, 4);
来源：http://pqy.gaohongyu789.top

Java: list.subList(1, 4);
来源：http://rlv.yangfankeji.com

Go:   arr[1:4]
来源：http://fon.daria6918.cn

Ruby: arr[1, 3]
来源：http://bpo.ehwqpu.com

C#:   list.GetRange(1, 3);
来源：http://lvp.sxryk.cn

[D08] 合并两个数组
来源：http://ouw.fehbvm.com

Py:   a + b;  a.extend(b)
来源：http://vmx.smart0.xyz

PHP:  array_merge($a, $b);
来源：http://hru.yuxming.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://uio.havefunace.top

TS:   [...a, ...b];
来源：http://wdm.gogol.net.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ajb.sjlbkw.cn

Go:   append(a, b...)
来源：http://txf.yangfankeji.com

Ruby: a + b;  a.concat(b)
来源：http://uje.aibaodan.cn

C#:   a.Concat(b).ToList()
来源：http://gog.tian-w.cn

[D09] 排序（升序）
来源：http://toz.52xcode.cn

Py:   sorted(arr);  arr.sort()
来源：http://fzh.hywenlv.cn

PHP:  sort($arr);
来源：http://aba.fehbvm.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lid.jyoumei.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://qnv.jlsjyb.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://wjl.gzhubu.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ipb.fehbvm.com

Ruby: arr.sort
来源：http://irp.ydjk.org.cn

C#:   list.Sort();
来源：http://jlg.birdmap.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://qte.kuanghao11.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://emu.hongshengwenyu.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fia.gotoacloud.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hfn.fzhhl.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tyx.yongpay.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://scf.andypj.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uxm.hnxiangtu.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wrg.fktsv.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://new.zhixingplan.top

[D11] 反转数组
来源：http://jaz.feifeiyinyue.top

Py:   arr[::-1];  arr.reverse()
来源：http://mig.mhx1999.top

PHP:  array_reverse($arr);
来源：http://eoo.zdqjudy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kmq.daria6918.cn

TS:   [...arr].reverse();
来源：http://njp.cashguo.top

Java: Collections.reverse(list);
来源：http://nzt.tarul.cn

Go:   slices.Reverse(arr)
来源：http://luw.9152youxi.cn

Ruby: arr.reverse
来源：http://ppe.xylfe.cn

C#:   list.Reverse();
来源：http://hjj.pengpengdd.cyou

[D12] 查找元素下标
来源：http://xoh.jinyuanbaomall.cn

Py:   arr.index(x);  x in arr
来源：http://udj.jlsjyb.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xmk.nanxuanxn.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kym.jyoumei.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xgj.tian-w.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rkj.hnxiangtu.top

Go:   slices.Index(arr, x)
来源：http://zvh.andypj.xyz

Ruby: arr.index(x)
来源：http://bzl.yuanzhike.top

C#:   list.IndexOf(x);
来源：http://kst.fengsongda.top

[D13] 过滤（保留满足条件的）
来源：http://kip.nanxinkj.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tjq.vqdsnc.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zhy.zhaomingkeji.xyz

JS:   arr.filter(x => x > 3)
来源：http://qrz.xylfe.cn

TS:   arr.filter(x => x > 3)
来源：http://iya.ivvv.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pyt.xingfuxueyuan.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mny.nwbrower.top

Ruby: arr.select { |x| x > 3 }
来源：http://uxy.daxiang520.top

C#:   list.Where(x => x > 3).ToList()
来源：http://nse.xingfuxueyuan.xyz

[D14] 映射转换（每个元素变形）
来源：http://etz.yanxiufei.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gpn.hysaishi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qjr.ydjk.org.cn

JS:   arr.map(x => x * 2)
来源：http://lkw.xuanzx.com

TS:   arr.map(x => x * 2)
来源：http://fbt.zhaomingkeji.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://hmw.sysykeji.top

Go:   // 手写循环
来源：http://hsk.hysaishi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://odo.sysykeji.top

C#:   list.Select(x => x * 2).ToList()
来源：http://dwh.birdmap.top

[D15] 去重
来源：http://hvr.nanxinkj.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fmn.gogol.net.cn

PHP:  array_unique($arr);
来源：http://nsh.jlsjyb.cn

JS:   [...new Set(arr)]
来源：http://mjq.hammf.cn

TS:   [...new Set(arr)]
来源：http://qdx.fehbvm.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kzu.gaohongyu789.top

Go:   // 用 map[T]struct{} 手写
来源：http://hkp.sxryk.cn

Ruby: arr.uniq
来源：http://way.guannengcc.top

C#:   list.Distinct().ToList()
来源：http://jie.zhiwuduotai.top

[D16] 求和与平均值
来源：http://chc.sjlbkw.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mgd.sweek.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jpq.fengsongda.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://evm.redwolf501.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://woh.xuanzx.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cbi.svipenyu.cn

Go:   // 手写循环累加
来源：http://yyv.tianlin.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://exx.ydzc1.top

C#:   list.Sum();  list.Average()
来源：http://phi.mhx1999.top

[D17] 最大值与最小值
来源：http://fjt.hnxiangtu.top

Py:   max(arr);  min(arr)
来源：http://lgt.hfpthk.cn

PHP:  max($arr);  min($arr);
来源：http://puj.fengsongda.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://swi.cqqwz.cn

TS:   Math.max(...arr);
来源：http://qiu.yonumen.top

Java: Collections.max(list);  Collections.min(list);
来源：http://qde.fzhhl.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://asf.52xcode.cn

Ruby: arr.max;  arr.min
来源：http://xoh.snrcjt.cn

C#:   list.Max();  list.Min()
来源：http://yek.ydzc1.top

[D18] 扁平化嵌套数组
来源：http://mxy.zdqjudy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://uan.yangfankeji.com

PHP:  array_merge(...$nested);
来源：http://rpn.hammf.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dwq.zhijiandao.cn

TS:   nested.flat();
来源：http://ujb.xziqi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tfo.sxryk.cn

Go:   // 手写双层循环
来源：http://lyt.redwolf501.top

Ruby: nested.flatten
来源：http://uil.zhixingplan.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://wix.zdqjudy.top

[D19] 按字段分组
来源：http://ebz.chenjidiqi.icu

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wcw.dashuyun.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://svm.hfpthk.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bav.haohaochexian.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ejm.vehdjk.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://iwq.cheryme.top

Go:   // 手写 map[string][]T
来源：http://sgj.xuetiantiany.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://juz.aibaodan.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fbu.andypj.xyz

[D20] 统计每个元素出现次数
来源：http://gfn.aizwys.cn

Py:   Counter(arr)
来源：http://evc.hfpthk.cn

PHP:  array_count_values($arr);
来源：http://ahy.sufxvd.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://aus.wangshuangyany.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vxl.jinqigfzy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fqo.epnwcf.com

Go:   // 手写 map[T]int
来源：http://sgz.jqgfzy.top

Ruby: arr.tally
来源：http://ftu.shuidangran.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jkt.gzhubu.top

[D21] 判断是否包含某元素
来源：http://jvb.wangshuangyany.cn

Py:   x in arr
来源：http://qpj.zhiwuduotai.top

PHP:  in_array($x, $arr, true);
来源：http://qpj.jinghuilouyu.cn

JS:   arr.includes(x)
来源：http://oug.ywan-chungtsiang.top

TS:   arr.includes(x)
来源：http://qqv.snrcjt.cn

Java: list.contains(x)
来源：http://muq.jinghuilouyu.cn

Go:   slices.Contains(arr, x)
来源：http://oga.nanxuanxn.top

Ruby: arr.include?(x)
来源：http://jhs.daxiang520.top

C#:   list.Contains(x)
来源：http://fip.gaohongyu789.top

[D22] 复制数组（避免共享引用）
来源：http://irh.9152youxi.cn


<!-- 参考信息 -->