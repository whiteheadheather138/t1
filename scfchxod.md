代发 wailian999

PHP:  $a && $b || !$c
来源：http://kdn.shanyushiyangtech.top

JS:   a && b || !c
来源：http://zcl.meibo888.top

TS:   a && b || !c
来源：http://pwx.iojbl.cn

Java: a && b || !c
来源：http://zoj.yj20258.top

Go:   a && b || !c
来源：http://fgn.cheryme.top

Ruby: a && b || !c
来源：http://ctr.epnwcf.com

C#:   a && b || !c
来源：http://aim.sxryk.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ens.yonumen.top

Py:   if not data: return
来源：http://lcb.cqqwz.cn

PHP:  if (!$data) { return; }
来源：http://dcf.sjlbkw.cn

JS:   if (!data) return;
来源：http://aur.hcnkem.com

TS:   if (!data) return;
来源：http://tit.gotoacloud.top

Java: if (data == null) return;
来源：http://oiz.cheryme.top

Go:   if data == nil { return }
来源：http://nuh.gogol.net.cn

Ruby: return if data.nil?
来源：http://tnl.smart0.xyz

C#:   if (data == null) return;
来源：http://rhj.mhx1999.top

================================================================================
来源：http://jru.yj20258.top

C. 函数与作用域
来源：http://csy.cashguo.top

================================================================================
来源：http://rak.mhx1999.top

[C01] 定义函数
来源：http://hon.ydzc1.top

Py:   def add(a, b): return a + b
来源：http://rfd.yj20258888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ulw.havefunace.top

JS:   function add(a, b) { return a + b; }
来源：http://hai.jqgufenzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kdb.c1oappe.top

Java: static int add(int a, int b) { return a + b; }
来源：http://hcs.yuxming.cn

Go:   func add(a, b int) int { return a + b }
来源：http://sxl.gaohongyu789.top

Ruby: def add(a, b); a + b; end
来源：http://zgi.uphjek.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jqq.dashuyun.cn

[C02] 默认参数
来源：http://ihj.shanyushiyangtech.top

Py:   def greet(name="World"): return name
来源：http://abj.dashuyun.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zkq.zycfv.cn

JS:   function greet(name = "World") { return name; }
来源：http://wfd.cashguo.top

TS:   function greet(name: string = "World") { return name; }
来源：http://qun.bbcook.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vju.gotoacloud.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://alx.yuxming.cn

Ruby: def greet(name = "World") = name
来源：http://kuz.52xcode.cn

C#:   string Greet(string name = "World") => name;
来源：http://yae.9152youxi.cn

[C03] 可变参数
来源：http://etn.ywan-chungtsiang.top

Py:   def total(*args): return sum(args)
来源：http://fjg.yj20258.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://djp.shangyingyoupin.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kaj.shanyushiyangkeji.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://agx.smart0.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qbd.wangdashe.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bmy.quarkkingdee.top

Ruby: def total(*nums); nums.sum; end
来源：http://azo.shanyushiyangtech.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rpi.dashuyun.cn

[C04] 命名参数 / 关键字参数
来源：http://zdk.jinqigufen.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lnr.yj202588.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://phq.wangdashe.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://eas.ybcxt.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rzj.yj202588.top

Java: // 无：用 Builder 模式或 record
来源：http://eml.gotoacloud.top

Go:   // 无：用配置结构体参数
来源：http://xbf.shzxlz.cn

Ruby: f(a: 1, b: 2)
来源：http://zal.ydjk.org.cn

C#:   f(a: 1, b: 2)
来源：http://cbu.fanxiaobao.xyz

[C05] 返回多个值
来源：http://eos.bbcook.cn

Py:   return a, b
来源：http://mho.guannengcc.top

PHP:  return [$a, $b];
来源：http://zra.hcnkem.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://hvv.jqgfzy.top

TS:   return { a, b };
来源：http://ypj.sweek.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ogq.hongshengwenyu.top

Go:   return a, b
来源：http://ahl.wangshuangyany.cn

Ruby: return a, b
来源：http://fez.gzhubu.top

C#:   return (a, b);              // ValueTuple
来源：http://flk.shangyingyoupin.top

[C06] 匿名函数 / lambda
来源：http://tli.tian-w.cn

Py:   square = lambda x: x * x
来源：http://jac.redwolf501.top

PHP:  $square = fn($x) => $x * $x;
来源：http://kqt.nanxinkj.top

JS:   const square = x => x * x;
来源：http://wmx.smart0.xyz

TS:   const square = (x: number): number => x * x;
来源：http://ssj.xinyue.icu

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://iod.fktsv.cn

Go:   sq := func(x int) int { return x * x }
来源：http://owm.cdnleiting.top

Ruby: square = ->(x) { x * x }
来源：http://itx.ehwqpu.com

C#:   Func<int, int> square = x => x * x;
来源：http://ugu.uphjek.com

[C07] 把函数作为参数传入
来源：http://uhp.jyoumei.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://chh.daria6918.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ozn.yvedp.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rat.sweek.top

TS:   arr.map(String)
来源：http://qzv.jiagoushi.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wqu.wangdashe.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qis.dianchejie.cn

Ruby: arr.map(&:upcase)
来源：http://ooa.mhx1999.top

C#:   arr.Select(s => s.ToUpper())
来源：http://oeh.zhoulong.xyz

[C08] 闭包
来源：http://kzr.pengpengdd.cyou

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tty.sjlbkw.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://eku.bjfxy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ovl.zhengqikj.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://esz.yonumen.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ygd.dashuyun.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xnm.wangdashe.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vyw.haohaochexian.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dol.316326.xyz

[C09] 递归
来源：http://ylt.tian-w.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fhu.0kj1m.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nbt.gzhubu.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://slb.jlsjyb.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qqb.cucudq.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bjl.vqdsnc.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wyf.redwolf501.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xfn.guowangkeji.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dyu.jyoumei.cn

[C10] 变量作用域
来源：http://dvx.meibo888.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://uga.hysaishi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kqd.xuanzx.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gkh.birdmap.top

TS:   同 JS
来源：http://zhp.hammf.cn

Java: 方法内为块级作用域
来源：http://ody.fzhhl.top

Go:   花括号块级作用域
来源：http://qla.hammf.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bls.jlsjyb.cn

C#:   块级作用域
来源：http://voa.smart0.xyz

[C11] 模块导入与导出
来源：http://dvd.gaohongyu789.top

Py:   from module import func
来源：http://sks.fanxiaobao.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://xqx.vehdjk.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://tfc.vqdsnc.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ddm.cucudq.cn

Java: import java.util.List;
来源：http://qig.iojbl.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cvi.hfpthk.cn

Ruby: require "json"; require_relative "./util"
来源：http://jry.hywenlv.cn

C#:   using System.Text;
来源：http://mzo.hywenlv.cn

[C12] 立即执行函数 IIFE
来源：http://sjr.zhiwuduotai.top

Py:   (lambda: print("run"))()
来源：http://mpu.hfpthk.cn

PHP:  (function () { echo "run"; })();
来源：http://nyf.hesvh.cn

JS:   (() => { console.log("run"); })();
来源：http://yib.snrcjt.cn

TS:   (() => { console.log("run"); })();
来源：http://pww.hcnkem.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bhj.fzhhl.top

Go:   func() { fmt.Println("run") }()
来源：http://hmd.hfpthk.cn

Ruby: -> { puts "run" }.call
来源：http://gym.vehdjk.com

C#:   // 无 IIFE：用静态构造函数
来源：http://vnb.zhixingplan.top

[C13] 类型声明 / 类型注解
来源：http://nrb.chenlongwang.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://oys.yuanzhike.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://akb.jinyuanbaomall.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jeg.tanke756.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rna.vehdjk.com

Java: int add(int a, int b) { return a + b; }
来源：http://vwl.gotoacloud.top

Go:   func add(a, b int) int
来源：http://bxh.guowangkeji.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cip.sxryk.cn

C#:   int Add(int a, int b) => a + b;
来源：http://bol.daxiang520.top

[C14] 泛型函数
来源：http://zsy.hnqzz.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qvj.meibo888.top

PHP:  // 无泛型
来源：http://fui.shzxlz.cn

JS:   // 无泛型
来源：http://lgy.ybcxt.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qrl.zycfv.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xle.fanxiaobao.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pgd.yanxiufei.cn

Ruby: # 无泛型
来源：http://nnj.sysykeji.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xvs.shzxlz.cn

[C15] 解构 / 展开参数
来源：http://ufn.sufxvd.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xkf.c1oappe.top

PHP:  [$a, $b] = $pair;
来源：http://ieg.zhongyouzk.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bch.shangyingyoupin.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pbt.ybcxt.top

Java: // 无解构
来源：http://iid.bbcook.cn

Go:   // 无解构
来源：http://sxg.feifeiyinyue.top

Ruby: a, b = pair
来源：http://grk.xylfe.cn

C#:   var (a, b) = pair;
来源：http://ilg.jinqigfzy.top

[C16] 函数 / 方法重载
来源：http://plg.tianlin.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nbt.havefunace.top

PHP:  // 无重载
来源：http://ecw.ydzc1.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ohr.sweek.top

TS:   // 用联合类型或重载签名声明
来源：http://btw.yueranfly.top

Java: void f(int a) {}  void f(String a) {}
来源：http://tio.shanyushiyangkeji.top

Go:   // 无重载：用不同函数名
来源：http://lig.bbcook.cn

Ruby: # 无重载：靠动态参数
来源：http://uzp.sysykeji.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://pgj.yvedp.cn

================================================================================
来源：http://cpu.xziqi.cn

D. 数组 / 列表 / 集合
来源：http://kuf.xuanzx.com

================================================================================
来源：http://dvs.yueranfly.top

[D01] 创建数组 / 列表
来源：http://tfz.yfazqb.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://gya.jinyuanbaomall.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cza.daria6918.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xbj.zhoulong.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://bia.sxryk.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nmg.yongpay.top

Go:   arr := []int{1, 2, 3}
来源：http://umo.shanyushiyangkeji.top

Ruby: arr = [1, 2, 3]
来源：http://eww.fzhhl.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vyt.chenjidiqi.icu

[D02] 追加元素到末尾
来源：http://kka.iojbl.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jle.hnxiangtu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pmp.aizwys.cn

JS:   arr.push(4);
来源：http://qhq.gaohongyu789.top

TS:   arr.push(4);
来源：http://wnz.yvedp.cn

Java: list.add(4);
来源：http://lmy.shanyushiyangtech.top

Go:   arr = append(arr, 4)
来源：http://lsc.jinyuanbaomall.cn

Ruby: arr << 4; arr.push(5)
来源：http://mys.ydjk.org.cn

C#:   list.Add(4);
来源：http://coi.feifeiyinyue.top

[D03] 在指定位置插入元素
来源：http://zrq.vqdsnc.cn

Py:   arr.insert(0, 0)
来源：http://ifl.nanxuanxn.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ajd.cdnleiting.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pig.zdqjudy.top

TS:   arr.splice(0, 0, 0);
来源：http://xjf.yanxiufei.cn

Java: list.add(0, 0);
来源：http://wss.zhoulong.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://rkv.52xcode.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wib.iojbl.cn

C#:   list.Insert(0, 0);
来源：http://dff.tarul.cn

[D04] 删除元素
来源：http://ewv.sweek.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nvm.pengpengdd.cyou

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xiv.iojbl.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://res.wangdashe.top

TS:   arr.splice(0, 1);
来源：http://kdl.hesvh.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rwc.daria6918.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ito.jinqigufen.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://srs.chenjidiqi.icu

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dco.hongshengwenyu.top

[D05] 访问与修改元素
来源：http://fbr.shanyushiyangkeji.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://txl.sxryk.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kss.mhx1999.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hhh.pycfn.com

TS:   arr[0]; arr.at(-1);
来源：http://jyv.jyoumei.cn

Java: list.get(0); list.set(0, 9);
来源：http://vgu.jiagoushi.top

Go:   arr[0]; arr[0] = 9
来源：http://pxs.zhongyouzk.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zgt.ivvv.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gal.ivvv.top

[D06] 数组长度
来源：http://awo.xuetiantiany.cn

Py:   len(arr)
来源：http://gwq.nanxuanxn.top

PHP:  count($arr);
来源：http://tre.chenlongwang.top

JS:   arr.length
来源：http://arr.yanxiufei.cn

TS:   arr.length
来源：http://aow.jinyuanbaomall.cn

Java: list.size();
来源：http://ysl.xuanzx.com

Go:   len(arr)
来源：http://xuj.xziqi.cn

Ruby: arr.length; arr.size
来源：http://njo.yongpay.top

C#:   list.Count;
来源：http://pnx.zhiwuduotai.top

[D07] 切片 / 取子数组
来源：http://onz.pengpengdd.cyou

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gas.iojbl.cn

PHP:  array_slice($arr, 1, 3);
来源：http://knm.ctjpmb.com

JS:   arr.slice(1, 4);
来源：http://ddb.havefunace.top

TS:   arr.slice(1, 4);
来源：http://srs.hcnkem.com

Java: list.subList(1, 4);
来源：http://lnz.bbcook.cn

Go:   arr[1:4]
来源：http://crv.yvedp.cn

Ruby: arr[1, 3]
来源：http://wyl.zhengqikj.top

C#:   list.GetRange(1, 3);
来源：http://jbh.fengsongda.top

[D08] 合并两个数组
来源：http://lmw.zhijiandao.cn

Py:   a + b;  a.extend(b)
来源：http://nkp.hnqzz.top

PHP:  array_merge($a, $b);
来源：http://bjl.chenjidiqi.icu

JS:   [...a, ...b];  a.concat(b);
来源：http://lds.ydjk.org.cn

TS:   [...a, ...b];
来源：http://vyw.smart0.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nak.dashuyun.cn

Go:   append(a, b...)
来源：http://lcp.shangyingyoupin.top

Ruby: a + b;  a.concat(b)
来源：http://iot.316326.xyz

C#:   a.Concat(b).ToList()
来源：http://rsj.zhixingplan.top

[D09] 排序（升序）
来源：http://yun.iojbl.cn

Py:   sorted(arr);  arr.sort()
来源：http://bla.sjlbkw.cn

PHP:  sort($arr);
来源：http://sqf.yj20258888.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nkg.zhiwuduotai.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://opv.fzhhl.top

Java: Collections.sort(list);  list.sort(null);
来源：http://udm.yuanzhike.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gzi.gogol.net.cn

Ruby: arr.sort
来源：http://bpy.tianlin.xyz

C#:   list.Sort();
来源：http://vae.zhengqikj.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://izj.ydjk.org.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kfq.guowangkeji.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hsg.jlsjyb.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pya.gzhubu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qlt.gotoacloud.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tuf.redwolf501.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ixr.sweek.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mlz.gzhubu.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tlg.tianlin.xyz

[D11] 反转数组
来源：http://qqc.yj20258888.top

Py:   arr[::-1];  arr.reverse()
来源：http://hya.feifeiyinyue.top

PHP:  array_reverse($arr);
来源：http://gam.hnqzz.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nkx.aizwys.cn

TS:   [...arr].reverse();
来源：http://xbe.zdqjudy.top

Java: Collections.reverse(list);
来源：http://uqf.xingfuxueyuan.xyz

Go:   slices.Reverse(arr)
来源：http://vgk.shzxlz.cn

Ruby: arr.reverse
来源：http://yon.9152youxi.cn

C#:   list.Reverse();
来源：http://err.zdbjq.cn

[D12] 查找元素下标
来源：http://jcn.epnwcf.com

Py:   arr.index(x);  x in arr
来源：http://uef.316326.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://igj.tian-w.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iei.mhx1999.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fwx.guowangkeji.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ibl.vehdjk.com

Go:   slices.Index(arr, x)
来源：http://hwg.gzhubu.top

Ruby: arr.index(x)
来源：http://lvw.shangyingyoupin.top

C#:   list.IndexOf(x);
来源：http://ygt.xuetiantiany.cn

[D13] 过滤（保留满足条件的）
来源：http://xom.gogol.net.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://uao.fzhhl.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pxs.yuanzhike.top

JS:   arr.filter(x => x > 3)
来源：http://btf.redwolf501.top

TS:   arr.filter(x => x > 3)
来源：http://oqf.hysaishi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rjy.zhijiandao.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sxs.zhoulong.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://qtg.zhongyouzk.top

C#:   list.Where(x => x > 3).ToList()
来源：http://pla.hammf.cn

[D14] 映射转换（每个元素变形）
来源：http://jzg.zdbjq.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cwd.fanxiaobao.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tyj.dianchejie.cn

JS:   arr.map(x => x * 2)
来源：http://kno.316326.xyz

TS:   arr.map(x => x * 2)
来源：http://mrb.sysykeji.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://bnx.daria6918.cn

Go:   // 手写循环
来源：http://dzb.316326.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://mav.uphjek.com

C#:   list.Select(x => x * 2).ToList()
来源：http://oth.nanxuanxn.top

[D15] 去重
来源：http://ejz.feifeiyinyue.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cpt.hesvh.cn

PHP:  array_unique($arr);
来源：http://hfl.pengpengdd.cyou

JS:   [...new Set(arr)]
来源：http://bov.hysaishi.cn

TS:   [...new Set(arr)]
来源：http://qaq.vehdjk.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://npu.zhixingplan.top

Go:   // 用 map[T]struct{} 手写
来源：http://goo.cdnleiting.top

Ruby: arr.uniq
来源：http://bbc.xuanzx.com


<!-- 参考信息 -->