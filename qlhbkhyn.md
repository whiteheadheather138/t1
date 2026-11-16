代发 wailian999

Py:   return a, b
来源：http://uhy.gotoacloud.top

PHP:  return [$a, $b];
来源：http://mqd.52xcode.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://txl.havefunace.top

TS:   return { a, b };
来源：http://wdi.yanxiufei.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vvv.hnqzz.top

Go:   return a, b
来源：http://vgy.316326.xyz

Ruby: return a, b
来源：http://ord.svipenyu.cn

C#:   return (a, b);              // ValueTuple
来源：http://tgv.ctjpmb.com

[C06] 匿名函数 / lambda
来源：http://igv.yangfankeji.com

Py:   square = lambda x: x * x
来源：http://red.aibaodan.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://gnc.yuxming.cn

JS:   const square = x => x * x;
来源：http://wwa.aizwys.cn

TS:   const square = (x: number): number => x * x;
来源：http://gfl.shanyushiyangtech.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nma.quarkkingdee.top

Go:   sq := func(x int) int { return x * x }
来源：http://xsb.guowangkeji.top

Ruby: square = ->(x) { x * x }
来源：http://ghm.xinyue.icu

C#:   Func<int, int> square = x => x * x;
来源：http://fsl.zhiwuduotai.top

[C07] 把函数作为参数传入
来源：http://ggb.fengsongda.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mky.fengsongda.top

PHP:  array_map("strtoupper", $arr);
来源：http://mok.jqgfzy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pyv.dashuyun.cn

TS:   arr.map(String)
来源：http://yhv.feifeiyinyue.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://oqu.pengpengdd.cyou

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zfn.fehbvm.com

Ruby: arr.map(&:upcase)
来源：http://spc.jinqigufen.top

C#:   arr.Select(s => s.ToUpper())
来源：http://myi.chenzaomai.com

[C08] 闭包
来源：http://edg.aizwys.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://plv.shuidangran.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rgb.yongpay.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cxa.cqqwz.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://efx.hfpthk.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://itu.hammf.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://okn.jinqigufen.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://woq.zhijiandao.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wmu.shanyushiyangkeji.top

[C09] 递归
来源：http://obk.jiagoushi.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jes.zhengqikj.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://veb.hnxiangtu.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://msh.fanxiaobao.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iyp.hnqzz.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lcy.ydjk.org.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wyc.fanxiaobao.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gze.xinyue.icu

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://efs.feifeiyinyue.top

[C10] 变量作用域
来源：http://eau.cqqwz.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ehz.sweek.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://axo.shanyushiyangkeji.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ixc.chenzaomai.com

TS:   同 JS
来源：http://ekw.svipenyu.cn

Java: 方法内为块级作用域
来源：http://eos.nanxuanxn.top

Go:   花括号块级作用域
来源：http://iql.wangshuangyany.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ark.cqqwz.cn

C#:   块级作用域
来源：http://lxq.yj202588.top

[C11] 模块导入与导出
来源：http://hlx.cdnleiting.top

Py:   from module import func
来源：http://skw.ywan-chungtsiang.top

PHP:  require "file.php";  或 use App\Service;
来源：http://tkg.tian-w.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://fxd.zdbjq.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ijf.ywan-chungtsiang.top

Java: import java.util.List;
来源：http://xpk.c1oappe.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pce.tarul.cn

Ruby: require "json"; require_relative "./util"
来源：http://iwb.shuidangran.top

C#:   using System.Text;
来源：http://fxx.yuanzhike.top

[C12] 立即执行函数 IIFE
来源：http://gbf.nanxinkj.top

Py:   (lambda: print("run"))()
来源：http://chs.bjfxy.top

PHP:  (function () { echo "run"; })();
来源：http://cvv.yanxiufei.cn

JS:   (() => { console.log("run"); })();
来源：http://zxk.9152youxi.cn

TS:   (() => { console.log("run"); })();
来源：http://lgf.gotoacloud.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://utj.gogol.net.cn

Go:   func() { fmt.Println("run") }()
来源：http://hpl.yangfankeji.com

Ruby: -> { puts "run" }.call
来源：http://cbv.tanke756.top

C#:   // 无 IIFE：用静态构造函数
来源：http://leq.cucudq.cn

[C13] 类型声明 / 类型注解
来源：http://vua.yj20258888.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://urz.fengsongda.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://etk.zhijiandao.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://med.zhijiandao.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lme.ywan-chungtsiang.top

Java: int add(int a, int b) { return a + b; }
来源：http://zkx.aizwys.cn

Go:   func add(a, b int) int
来源：http://uqe.fehbvm.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jte.shangyingyoupin.top

C#:   int Add(int a, int b) => a + b;
来源：http://zmb.yanxiufei.cn

[C14] 泛型函数
来源：http://etl.tarul.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://elc.hongshengwenyu.top

PHP:  // 无泛型
来源：http://zrl.52xcode.cn

JS:   // 无泛型
来源：http://fjk.tian-w.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wri.svipenyu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vzv.chenzaomai.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://int.cashguo.top

Ruby: # 无泛型
来源：http://glv.hywenlv.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://uhf.uphjek.com

[C15] 解构 / 展开参数
来源：http://nvm.tian-w.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ncp.dashuyun.cn

PHP:  [$a, $b] = $pair;
来源：http://aix.andypj.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xri.jinqigfzy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uzj.tanke756.top

Java: // 无解构
来源：http://jmz.feifeiyinyue.top

Go:   // 无解构
来源：http://zvx.sufxvd.cn

Ruby: a, b = pair
来源：http://mqz.jinqigfzy.top

C#:   var (a, b) = pair;
来源：http://tjn.nanxuanxn.top

[C16] 函数 / 方法重载
来源：http://vjp.gotoacloud.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://iew.sufxvd.cn

PHP:  // 无重载
来源：http://yhl.shzxlz.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://vod.yj20258.top

TS:   // 用联合类型或重载签名声明
来源：http://pwy.sjlbkw.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wfw.shuidangran.top

Go:   // 无重载：用不同函数名
来源：http://kkh.jinqigufen.top

Ruby: # 无重载：靠动态参数
来源：http://umj.yfazqb.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://xbe.shangyingyoupin.top

================================================================================
来源：http://gwn.zhaomingkeji.xyz

D. 数组 / 列表 / 集合
来源：http://cte.wangdashe.top

================================================================================
来源：http://fad.sufxvd.cn

[D01] 创建数组 / 列表
来源：http://thw.cashguo.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://zzg.zhengqikj.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zcf.redwolf501.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rse.zhixingplan.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://wxr.dianchejie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://scu.hongshengwenyu.top

Go:   arr := []int{1, 2, 3}
来源：http://qrr.0kj1m.cn

Ruby: arr = [1, 2, 3]
来源：http://xjd.9152youxi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bxw.zdbjq.cn

[D02] 追加元素到末尾
来源：http://trx.jqgfzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://byu.shanyushiyangkeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xro.guannengcc.top

JS:   arr.push(4);
来源：http://iwq.pycfn.com

TS:   arr.push(4);
来源：http://jxz.jianghu66.top

Java: list.add(4);
来源：http://qjs.9152youxi.cn

Go:   arr = append(arr, 4)
来源：http://xzo.sufxvd.cn

Ruby: arr << 4; arr.push(5)
来源：http://tkg.0kj1m.cn

C#:   list.Add(4);
来源：http://avt.xziqi.cn

[D03] 在指定位置插入元素
来源：http://mzi.fktsv.cn

Py:   arr.insert(0, 0)
来源：http://uel.shuidangran.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uvq.ctjpmb.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://swi.zycfv.cn

TS:   arr.splice(0, 0, 0);
来源：http://phs.ppjwa.cn

Java: list.add(0, 0);
来源：http://ihs.jqgufenzy.top

Go:   arr = append([]int{0}, arr...)
来源：http://qed.chenlongwang.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cet.jlsjyb.cn

C#:   list.Insert(0, 0);
来源：http://tav.aibaodan.cn

[D04] 删除元素
来源：http://vfp.tianlin.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://aio.gaohongyu789.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gxx.fengsongda.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qpz.aibaodan.cn

TS:   arr.splice(0, 1);
来源：http://ljp.meibo888.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pok.jinyuanbaomall.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tzh.xingfuxueyuan.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://phy.yuanzhike.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://eiw.sxryk.cn

[D05] 访问与修改元素
来源：http://hhk.svipenyu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wza.gzhubu.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://peo.zdbjq.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yes.hcnkem.com

TS:   arr[0]; arr.at(-1);
来源：http://arz.vqdsnc.cn

Java: list.get(0); list.set(0, 9);
来源：http://yqr.daria6918.cn

Go:   arr[0]; arr[0] = 9
来源：http://gwz.zycfv.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ezk.redwolf501.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://drm.cashguo.top

[D06] 数组长度
来源：http://dbq.vqdsnc.cn

Py:   len(arr)
来源：http://bou.tarul.cn

PHP:  count($arr);
来源：http://xnw.hammf.cn

JS:   arr.length
来源：http://lao.hnqzz.top

TS:   arr.length
来源：http://gvi.feifeiyinyue.top

Java: list.size();
来源：http://kha.0kj1m.cn

Go:   len(arr)
来源：http://vvs.cashguo.top

Ruby: arr.length; arr.size
来源：http://maq.gogol.net.cn

C#:   list.Count;
来源：http://btt.cdnleiting.top

[D07] 切片 / 取子数组
来源：http://xyt.fanxiaobao.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bwy.ctjpmb.com

PHP:  array_slice($arr, 1, 3);
来源：http://kyp.snrcjt.cn

JS:   arr.slice(1, 4);
来源：http://bbc.quarkkingdee.top

TS:   arr.slice(1, 4);
来源：http://qxz.daxiang520.top

Java: list.subList(1, 4);
来源：http://goo.shanyushiyangkeji.top

Go:   arr[1:4]
来源：http://wnq.dashuyun.cn

Ruby: arr[1, 3]
来源：http://qak.gogol.net.cn

C#:   list.GetRange(1, 3);
来源：http://ias.nanxinkj.top

[D08] 合并两个数组
来源：http://rcx.yuanzhike.top

Py:   a + b;  a.extend(b)
来源：http://vuw.ppjwa.cn

PHP:  array_merge($a, $b);
来源：http://zvr.chenzaomai.com

JS:   [...a, ...b];  a.concat(b);
来源：http://lav.jinqigufen.top

TS:   [...a, ...b];
来源：http://xxu.jqgfzy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yee.dianchejie.cn

Go:   append(a, b...)
来源：http://mys.birdmap.top

Ruby: a + b;  a.concat(b)
来源：http://kfu.zhengqikj.top

C#:   a.Concat(b).ToList()
来源：http://ggk.yonumen.top

[D09] 排序（升序）
来源：http://ijf.xuetiantiany.cn

Py:   sorted(arr);  arr.sort()
来源：http://vmd.jlsjyb.cn

PHP:  sort($arr);
来源：http://ggi.yueranfly.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://clf.yj20258.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ezt.0kj1m.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://jyj.sjlbkw.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jps.nanxuanxn.top

Ruby: arr.sort
来源：http://aso.guowangkeji.top

C#:   list.Sort();
来源：http://nzi.jqgfzy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://tub.cqqwz.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zwo.sysykeji.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hak.pycfn.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bfg.tanke756.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lbu.shanyushiyangtech.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mti.bbcook.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://udk.haohaochexian.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sau.yonumen.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kkp.gzhubu.top

[D11] 反转数组
来源：http://hhi.jyoumei.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wzs.dashuyun.cn

PHP:  array_reverse($arr);
来源：http://jrk.havefunace.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://peg.chenzaomai.com

TS:   [...arr].reverse();
来源：http://akb.sxryk.cn

Java: Collections.reverse(list);
来源：http://psv.chenjidiqi.icu

Go:   slices.Reverse(arr)
来源：http://oiy.chenjidiqi.icu

Ruby: arr.reverse
来源：http://boi.epnwcf.com

C#:   list.Reverse();
来源：http://itb.xylfe.cn

[D12] 查找元素下标
来源：http://hzd.jyoumei.cn

Py:   arr.index(x);  x in arr
来源：http://ofv.epnwcf.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qmg.316326.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qmj.zhoulong.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://clg.316326.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mpo.ybcxt.top

Go:   slices.Index(arr, x)
来源：http://bvh.0kj1m.cn

Ruby: arr.index(x)
来源：http://rqh.cdnleiting.top

C#:   list.IndexOf(x);
来源：http://iwb.aibaodan.cn

[D13] 过滤（保留满足条件的）
来源：http://ejy.zhiwuduotai.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fcn.iojbl.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nlb.daxiang520.top

JS:   arr.filter(x => x > 3)
来源：http://dhq.dianchejie.cn

TS:   arr.filter(x => x > 3)
来源：http://dlk.shanyushiyangkeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://plp.sjlbkw.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qky.yongpay.top

Ruby: arr.select { |x| x > 3 }
来源：http://uap.gaohongyu789.top

C#:   list.Where(x => x > 3).ToList()
来源：http://yvj.jiagoushi.top

[D14] 映射转换（每个元素变形）
来源：http://yul.chenjidiqi.icu

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nsx.tarul.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tps.xuanzx.com

JS:   arr.map(x => x * 2)
来源：http://jyv.zhijiandao.cn

TS:   arr.map(x => x * 2)
来源：http://wqz.guowangkeji.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://fzd.jinyuanbaomall.cn

Go:   // 手写循环
来源：http://wmb.fanxiaobao.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://jzy.jiagoushi.top

C#:   list.Select(x => x * 2).ToList()
来源：http://wpn.haohaochexian.top

[D15] 去重
来源：http://myz.hnqzz.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kyh.xuanzx.com

PHP:  array_unique($arr);
来源：http://kjx.fehbvm.com

JS:   [...new Set(arr)]
来源：http://bjv.cqqwz.cn

TS:   [...new Set(arr)]
来源：http://zdn.yfazqb.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uvl.zhijiandao.cn

Go:   // 用 map[T]struct{} 手写
来源：http://jtd.gotoacloud.top

Ruby: arr.uniq
来源：http://jjk.0kj1m.cn

C#:   list.Distinct().ToList()
来源：http://kip.ywan-chungtsiang.top

[D16] 求和与平均值
来源：http://uof.smart0.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yvt.guannengcc.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sca.snrcjt.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://naq.tarul.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fnu.zhixingplan.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://doh.aibaodan.cn

Go:   // 手写循环累加
来源：http://exc.zdqjudy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kbh.shangyingyoupin.top

C#:   list.Sum();  list.Average()
来源：http://xsk.sxryk.cn

[D17] 最大值与最小值
来源：http://ztu.ywan-chungtsiang.top

Py:   max(arr);  min(arr)
来源：http://apq.feifeiyinyue.top

PHP:  max($arr);  min($arr);
来源：http://xml.zhijiandao.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yru.yfazqb.com

TS:   Math.max(...arr);
来源：http://mra.jlsjyb.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://keu.havefunace.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bxq.yj202588.top

Ruby: arr.max;  arr.min
来源：http://tew.zdbjq.cn

C#:   list.Max();  list.Min()
来源：http://kiy.ctjpmb.com

[D18] 扁平化嵌套数组
来源：http://epv.xylfe.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xbs.meibo888.top

PHP:  array_merge(...$nested);
来源：http://ndn.hongshengwenyu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://evj.vehdjk.com

TS:   nested.flat();
来源：http://jxf.mhx1999.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nqx.nanxinkj.top

Go:   // 手写双层循环
来源：http://krj.xingfuxueyuan.xyz

Ruby: nested.flatten
来源：http://url.quarkkingdee.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://czh.feifeiyinyue.top

[D19] 按字段分组
来源：http://dxl.birdmap.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vdm.yj20258888.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kkz.sufxvd.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://oxd.svipenyu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xls.shanyushiyangtech.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hnb.fengsongda.top

Go:   // 手写 map[string][]T
来源：http://vbj.xziqi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://edy.jiagoushi.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://moz.tarul.cn

[D20] 统计每个元素出现次数
来源：http://moz.jyoumei.cn

Py:   Counter(arr)
来源：http://fyq.hnqzz.top

PHP:  array_count_values($arr);
来源：http://hga.nanxinkj.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wpz.aizwys.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yvl.jinghuilouyu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wkh.yangfankeji.com

Go:   // 手写 map[T]int
来源：http://pof.haohaochexian.top

Ruby: arr.tally
来源：http://adj.zhaomingkeji.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://owd.zdqjudy.top

[D21] 判断是否包含某元素
来源：http://oqp.uphjek.com

Py:   x in arr
来源：http://fvj.iojbl.cn

PHP:  in_array($x, $arr, true);
来源：http://hji.aibaodan.cn

JS:   arr.includes(x)
来源：http://egf.uphjek.com

TS:   arr.includes(x)
来源：http://ulk.hnqzz.top

Java: list.contains(x)
来源：http://rve.iojbl.cn

Go:   slices.Contains(arr, x)
来源：http://txw.jyoumei.cn

Ruby: arr.include?(x)
来源：http://kuz.52xcode.cn

C#:   list.Contains(x)
来源：http://fwl.feifeiyinyue.top

[D22] 复制数组（避免共享引用）
来源：http://lur.jinyuanbaomall.cn


<!-- 参考信息 -->