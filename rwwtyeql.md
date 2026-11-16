代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://eou.vqdsnc.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nza.tianlin.xyz

[C04] 命名参数 / 关键字参数
来源：http://ktc.shanyushiyangtech.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vop.jyoumei.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xsy.ppjwa.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ldm.gotoacloud.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bjd.chenzaomai.com

Java: // 无：用 Builder 模式或 record
来源：http://nbs.zhoulong.xyz

Go:   // 无：用配置结构体参数
来源：http://nfr.hnqzz.top

Ruby: f(a: 1, b: 2)
来源：http://ezo.smart0.xyz

C#:   f(a: 1, b: 2)
来源：http://ztw.cdnleiting.top

[C05] 返回多个值
来源：http://oap.zhiwuduotai.top

Py:   return a, b
来源：http://oji.havefunace.top

PHP:  return [$a, $b];
来源：http://fnk.tarul.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://rba.gaohongyu789.top

TS:   return { a, b };
来源：http://zkb.yj20258.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sdp.snrcjt.cn

Go:   return a, b
来源：http://edw.jiagoushi.top

Ruby: return a, b
来源：http://vsw.jinqigufen.top

C#:   return (a, b);              // ValueTuple
来源：http://kds.fktsv.cn

[C06] 匿名函数 / lambda
来源：http://wov.xylfe.cn

Py:   square = lambda x: x * x
来源：http://ekg.shanyushiyangkeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://qdb.zhoulong.xyz

JS:   const square = x => x * x;
来源：http://dab.gotoacloud.top

TS:   const square = (x: number): number => x * x;
来源：http://jvb.yonumen.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zlu.cashguo.top

Go:   sq := func(x int) int { return x * x }
来源：http://txq.yonumen.top

Ruby: square = ->(x) { x * x }
来源：http://gwd.chenlongwang.top

C#:   Func<int, int> square = x => x * x;
来源：http://smr.iojbl.cn

[C07] 把函数作为参数传入
来源：http://axj.pengpengdd.cyou

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://aun.zhoulong.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://uwe.havefunace.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cea.shanyushiyangkeji.top

TS:   arr.map(String)
来源：http://yjl.bjfxy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hrr.epnwcf.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lne.redwolf501.top

Ruby: arr.map(&:upcase)
来源：http://mxx.jinghuilouyu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://pkp.smart0.xyz

[C08] 闭包
来源：http://ilp.fzhhl.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dqi.shzxlz.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ysj.epnwcf.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tbn.zhengqikj.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lnl.epnwcf.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bfh.chenzaomai.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kzy.hnqzz.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bkj.zhiwuduotai.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zpb.yuanzhike.top

[C09] 递归
来源：http://xmc.bbcook.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nxd.guannengcc.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://psl.jqgfzy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uwa.birdmap.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qgd.mhx1999.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lxy.xuetiantiany.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://oqy.ywan-chungtsiang.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mrf.nwbrower.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mbu.hfpthk.cn

[C10] 变量作用域
来源：http://rxm.jqgfzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wzf.fehbvm.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qad.yongpay.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ztj.fanxiaobao.xyz

TS:   同 JS
来源：http://abf.sjlbkw.cn

Java: 方法内为块级作用域
来源：http://hyf.aibaodan.cn

Go:   花括号块级作用域
来源：http://hpa.yueranfly.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://aab.jinqigufen.top

C#:   块级作用域
来源：http://lsg.cucudq.cn

[C11] 模块导入与导出
来源：http://adu.yonumen.top

Py:   from module import func
来源：http://fug.zhaomingkeji.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://hlh.ppjwa.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zrz.havefunace.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zts.nanxuanxn.top

Java: import java.util.List;
来源：http://qfj.epnwcf.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://inj.xziqi.cn

Ruby: require "json"; require_relative "./util"
来源：http://qco.xuetiantiany.cn

C#:   using System.Text;
来源：http://wgg.gotoacloud.top

[C12] 立即执行函数 IIFE
来源：http://adt.hesvh.cn

Py:   (lambda: print("run"))()
来源：http://iyf.snrcjt.cn

PHP:  (function () { echo "run"; })();
来源：http://awn.hnxiangtu.top

JS:   (() => { console.log("run"); })();
来源：http://bso.cqqwz.cn

TS:   (() => { console.log("run"); })();
来源：http://gxi.jqgufenzy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dqj.hammf.cn

Go:   func() { fmt.Println("run") }()
来源：http://ryw.hnxiangtu.top

Ruby: -> { puts "run" }.call
来源：http://how.yangfankeji.com

C#:   // 无 IIFE：用静态构造函数
来源：http://rqp.vqdsnc.cn

[C13] 类型声明 / 类型注解
来源：http://rlw.wangdashe.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bzx.yangfankeji.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ikn.vqdsnc.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qkl.mhx1999.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://crb.wangdashe.top

Java: int add(int a, int b) { return a + b; }
来源：http://vxe.yvedp.cn

Go:   func add(a, b int) int
来源：http://wnj.hongshengwenyu.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hrf.zhaomingkeji.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://dxb.tianlin.xyz

[C14] 泛型函数
来源：http://qqd.yj202588.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://myh.fehbvm.com

PHP:  // 无泛型
来源：http://det.fktsv.cn

JS:   // 无泛型
来源：http://pbu.daxiang520.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jgu.sxryk.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yct.redwolf501.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zvl.fengsongda.top

Ruby: # 无泛型
来源：http://qis.ybcxt.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ivx.hywenlv.cn

[C15] 解构 / 展开参数
来源：http://skf.nanxuanxn.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yqm.dianchejie.cn

PHP:  [$a, $b] = $pair;
来源：http://kln.sxryk.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dlo.guannengcc.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dzl.hcnkem.com

Java: // 无解构
来源：http://bpa.zdbjq.cn

Go:   // 无解构
来源：http://ges.cashguo.top

Ruby: a, b = pair
来源：http://hyz.birdmap.top

C#:   var (a, b) = pair;
来源：http://ral.wangshuangyany.cn

[C16] 函数 / 方法重载
来源：http://uoq.gaohongyu789.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sox.jinqigufen.top

PHP:  // 无重载
来源：http://nip.kuanghao11.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://koq.hcnkem.com

TS:   // 用联合类型或重载签名声明
来源：http://vzp.cqqwz.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ypz.bbcook.cn

Go:   // 无重载：用不同函数名
来源：http://fyc.jqgufenzy.top

Ruby: # 无重载：靠动态参数
来源：http://wwk.gogol.net.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ivv.zycfv.cn

================================================================================
来源：http://bmb.yuanzhike.top

D. 数组 / 列表 / 集合
来源：http://iyh.cdnleiting.top

================================================================================
来源：http://pyd.fanxiaobao.xyz

[D01] 创建数组 / 列表
来源：http://flc.sysykeji.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://vxa.fengsongda.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dhv.birdmap.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dra.hcnkem.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://tkj.c1oappe.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rzb.jlsjyb.cn

Go:   arr := []int{1, 2, 3}
来源：http://mlu.ybcxt.top

Ruby: arr = [1, 2, 3]
来源：http://snx.cucudq.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tak.gaohongyu789.top

[D02] 追加元素到末尾
来源：http://dcb.andypj.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ldu.ctjpmb.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pkv.52xcode.cn

JS:   arr.push(4);
来源：http://vem.hywenlv.cn

TS:   arr.push(4);
来源：http://kqn.zycfv.cn

Java: list.add(4);
来源：http://rfs.meibo888.top

Go:   arr = append(arr, 4)
来源：http://lle.dianchejie.cn

Ruby: arr << 4; arr.push(5)
来源：http://zpy.meibo888.top

C#:   list.Add(4);
来源：http://qzx.pengpengdd.cyou

[D03] 在指定位置插入元素
来源：http://asc.birdmap.top

Py:   arr.insert(0, 0)
来源：http://pkg.daxiang520.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xgy.ybcxt.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zrm.zdqjudy.top

TS:   arr.splice(0, 0, 0);
来源：http://uho.fzhhl.top

Java: list.add(0, 0);
来源：http://tdk.hammf.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xjj.jinqigfzy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qzx.c1oappe.top

C#:   list.Insert(0, 0);
来源：http://afp.jiagoushi.top

[D04] 删除元素
来源：http://klg.shzxlz.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kfv.xuetiantiany.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zkn.tarul.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cic.fzhhl.top

TS:   arr.splice(0, 1);
来源：http://zko.zhijiandao.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xbx.nanxinkj.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tcz.svipenyu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fxd.andypj.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://oyg.hesvh.cn

[D05] 访问与修改元素
来源：http://wdm.sjlbkw.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tec.bbcook.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ktd.epnwcf.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fbu.yj202588.top

TS:   arr[0]; arr.at(-1);
来源：http://mce.yfazqb.com

Java: list.get(0); list.set(0, 9);
来源：http://emh.xylfe.cn

Go:   arr[0]; arr[0] = 9
来源：http://pxh.sxryk.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sgu.shuidangran.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dam.zhaomingkeji.xyz

[D06] 数组长度
来源：http://mgs.mhx1999.top

Py:   len(arr)
来源：http://opj.hfpthk.cn

PHP:  count($arr);
来源：http://kdo.9152youxi.cn

JS:   arr.length
来源：http://dex.sjlbkw.cn

TS:   arr.length
来源：http://ivo.ppjwa.cn

Java: list.size();
来源：http://pjk.zhiwuduotai.top

Go:   len(arr)
来源：http://dzr.zhijiandao.cn

Ruby: arr.length; arr.size
来源：http://xqa.guannengcc.top

C#:   list.Count;
来源：http://dsi.9152youxi.cn

[D07] 切片 / 取子数组
来源：http://nxz.316326.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://uzp.zhijiandao.cn

PHP:  array_slice($arr, 1, 3);
来源：http://sbs.yj202588.top

JS:   arr.slice(1, 4);
来源：http://bim.shuidangran.top

TS:   arr.slice(1, 4);
来源：http://vdj.chenjidiqi.icu

Java: list.subList(1, 4);
来源：http://hmz.guowangkeji.top

Go:   arr[1:4]
来源：http://mwa.jinqigufen.top

Ruby: arr[1, 3]
来源：http://xie.ivvv.top

C#:   list.GetRange(1, 3);
来源：http://ype.yongpay.top

[D08] 合并两个数组
来源：http://vzm.ydjk.org.cn

Py:   a + b;  a.extend(b)
来源：http://ora.zdqjudy.top

PHP:  array_merge($a, $b);
来源：http://swa.sufxvd.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://bej.ydzc1.top

TS:   [...a, ...b];
来源：http://rbs.tian-w.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zdf.shanyushiyangkeji.top

Go:   append(a, b...)
来源：http://chd.xuetiantiany.cn

Ruby: a + b;  a.concat(b)
来源：http://fpp.zhijiandao.cn

C#:   a.Concat(b).ToList()
来源：http://pyl.fengsongda.top

[D09] 排序（升序）
来源：http://adt.shuidangran.top

Py:   sorted(arr);  arr.sort()
来源：http://bsj.yanxiufei.cn

PHP:  sort($arr);
来源：http://off.pycfn.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jat.fengsongda.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://idj.jlsjyb.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://fec.jinghuilouyu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mki.yongpay.top

Ruby: arr.sort
来源：http://yva.meibo888.top

C#:   list.Sort();
来源：http://yaf.hammf.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zel.birdmap.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kqp.sysykeji.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mzl.kuanghao11.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wpr.shangyingyoupin.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nly.shuidangran.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://quo.xylfe.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://esn.tian-w.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ylw.cheryme.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://swh.jinqigufen.top

[D11] 反转数组
来源：http://sfx.sweek.top

Py:   arr[::-1];  arr.reverse()
来源：http://jpv.9152youxi.cn

PHP:  array_reverse($arr);
来源：http://cxy.jqgufenzy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xgw.zhaomingkeji.xyz

TS:   [...arr].reverse();
来源：http://zty.fanxiaobao.xyz

Java: Collections.reverse(list);
来源：http://onl.jiagoushi.top

Go:   slices.Reverse(arr)
来源：http://kvy.aizwys.cn

Ruby: arr.reverse
来源：http://xii.yangfankeji.com

C#:   list.Reverse();
来源：http://cpy.gzhubu.top

[D12] 查找元素下标
来源：http://sxm.tanke756.top

Py:   arr.index(x);  x in arr
来源：http://hrj.zhaomingkeji.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pgw.aibaodan.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zow.fehbvm.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bvn.ehwqpu.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nra.chenlongwang.top

Go:   slices.Index(arr, x)
来源：http://ysd.guannengcc.top

Ruby: arr.index(x)
来源：http://ums.nanxuanxn.top

C#:   list.IndexOf(x);
来源：http://ilu.hcnkem.com

[D13] 过滤（保留满足条件的）
来源：http://pit.hcnkem.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bux.shangyingyoupin.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cqp.guannengcc.top

JS:   arr.filter(x => x > 3)
来源：http://ugy.ctjpmb.com

TS:   arr.filter(x => x > 3)
来源：http://tgy.vehdjk.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://oac.nanxuanxn.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qao.ivvv.top

Ruby: arr.select { |x| x > 3 }
来源：http://jkf.ctjpmb.com

C#:   list.Where(x => x > 3).ToList()
来源：http://clb.vehdjk.com

[D14] 映射转换（每个元素变形）
来源：http://ryb.pycfn.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dhm.316326.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://oom.meibo888.top

JS:   arr.map(x => x * 2)
来源：http://nwp.vqdsnc.cn

TS:   arr.map(x => x * 2)
来源：http://tfj.yangfankeji.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://icr.ydzc1.top

Go:   // 手写循环
来源：http://rjt.gotoacloud.top

Ruby: arr.map { |x| x * 2 }
来源：http://sdz.jianghu66.top

C#:   list.Select(x => x * 2).ToList()
来源：http://duk.shuidangran.top

[D15] 去重
来源：http://pml.sjlbkw.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://glo.xziqi.cn

PHP:  array_unique($arr);
来源：http://mli.dashuyun.cn

JS:   [...new Set(arr)]
来源：http://nwv.ppjwa.cn

TS:   [...new Set(arr)]
来源：http://fsd.dashuyun.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wth.hfpthk.cn

Go:   // 用 map[T]struct{} 手写
来源：http://fwf.sjlbkw.cn

Ruby: arr.uniq
来源：http://ccx.sysykeji.top

C#:   list.Distinct().ToList()
来源：http://ofk.c1oappe.top

[D16] 求和与平均值
来源：http://psa.feifeiyinyue.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://unx.hysaishi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bkc.hammf.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ydl.jlsjyb.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xwu.epnwcf.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hxg.tanke756.top

Go:   // 手写循环累加
来源：http://oif.mhx1999.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xwi.xylfe.cn

C#:   list.Sum();  list.Average()
来源：http://pcu.tianlin.xyz

[D17] 最大值与最小值
来源：http://lhb.tianlin.xyz

Py:   max(arr);  min(arr)
来源：http://olv.52xcode.cn

PHP:  max($arr);  min($arr);
来源：http://dpu.haohaochexian.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://teu.tanke756.top

TS:   Math.max(...arr);
来源：http://dvr.jqgufenzy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://vjr.xinyue.icu

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ohz.yangfankeji.com

Ruby: arr.max;  arr.min
来源：http://bhl.fktsv.cn

C#:   list.Max();  list.Min()
来源：http://wdw.sweek.top

[D18] 扁平化嵌套数组
来源：http://ulx.zycfv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://syr.yonumen.top

PHP:  array_merge(...$nested);
来源：http://ezb.zhiwuduotai.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wsl.smart0.xyz

TS:   nested.flat();
来源：http://zff.zhiwuduotai.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pvl.mhx1999.top

Go:   // 手写双层循环
来源：http://kdr.nwbrower.top

Ruby: nested.flatten
来源：http://lct.xingfuxueyuan.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://odb.iojbl.cn

[D19] 按字段分组
来源：http://ggq.ydjk.org.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ytb.ybcxt.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ifr.jinghuilouyu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://iov.yongpay.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://xsk.snrcjt.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wyu.ydjk.org.cn

Go:   // 手写 map[string][]T
来源：http://jgs.dashuyun.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://qii.xuetiantiany.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pcj.jyoumei.cn

[D20] 统计每个元素出现次数
来源：http://xss.ppjwa.cn

Py:   Counter(arr)
来源：http://dwk.shangyingyoupin.top

PHP:  array_count_values($arr);
来源：http://icr.meibo888.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://khm.daria6918.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://twa.sufxvd.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ety.ppjwa.cn

Go:   // 手写 map[T]int
来源：http://hbb.c1oappe.top


<!-- 参考信息 -->