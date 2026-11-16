代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://awc.snrcjt.cn

Java: x instanceof Number
来源：http://ysg.iojbl.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wac.zdbjq.cn

Ruby: x.is_a?(Numeric)
来源：http://nwb.nwbrower.top

C#:   x is int or double or decimal
来源：http://ytc.yuanzhike.top

[B14] 判断值是否在集合内
来源：http://pub.jianghu66.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dwl.chenjidiqi.icu

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fhs.smart0.xyz

JS:   [1, 2, 3].includes(x)
来源：http://ums.fengsongda.top

TS:   [1, 2, 3].includes(x)
来源：http://qyy.haohaochexian.top

Java: List.of(1, 2, 3).contains(x)
来源：http://jnw.tanke756.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mja.chenjidiqi.icu

Ruby: [1, 2, 3].include?(x)
来源：http://tjj.meibo888.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qso.cqqwz.cn

[B15] 布尔运算与取反
来源：http://azu.xylfe.cn

Py:   a and b or not c
来源：http://ien.hywenlv.cn

PHP:  $a && $b || !$c
来源：http://wjr.wangshuangyany.cn

JS:   a && b || !c
来源：http://wet.birdmap.top

TS:   a && b || !c
来源：http://usn.yj202588.top

Java: a && b || !c
来源：http://mtm.wangshuangyany.cn

Go:   a && b || !c
来源：http://ypf.jinyuanbaomall.cn

Ruby: a && b || !c
来源：http://bhc.fengsongda.top

C#:   a && b || !c
来源：http://vkl.nwbrower.top

[B16] 卫语句：不满足条件提前返回
来源：http://olv.hysaishi.cn

Py:   if not data: return
来源：http://zqt.cheryme.top

PHP:  if (!$data) { return; }
来源：http://xew.yfazqb.com

JS:   if (!data) return;
来源：http://mav.uphjek.com

TS:   if (!data) return;
来源：http://amm.cashguo.top

Java: if (data == null) return;
来源：http://dzx.xingfuxueyuan.xyz

Go:   if data == nil { return }
来源：http://jbi.sweek.top

Ruby: return if data.nil?
来源：http://szb.fehbvm.com

C#:   if (data == null) return;
来源：http://jum.yj20258888.top

================================================================================
来源：http://bau.gogol.net.cn

C. 函数与作用域
来源：http://nxs.xziqi.cn

================================================================================
来源：http://xzg.hammf.cn

[C01] 定义函数
来源：http://buu.dashuyun.cn

Py:   def add(a, b): return a + b
来源：http://pau.haohaochexian.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wrs.andypj.xyz

JS:   function add(a, b) { return a + b; }
来源：http://ulr.meibo888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mwh.uphjek.com

Java: static int add(int a, int b) { return a + b; }
来源：http://ntq.nwbrower.top

Go:   func add(a, b int) int { return a + b }
来源：http://ocg.aibaodan.cn

Ruby: def add(a, b); a + b; end
来源：http://nhp.bjfxy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yrf.xylfe.cn

[C02] 默认参数
来源：http://hgo.hongshengwenyu.top

Py:   def greet(name="World"): return name
来源：http://fye.xinyue.icu

PHP:  function greet($name = "World") { return $name; }
来源：http://hma.cqqwz.cn

JS:   function greet(name = "World") { return name; }
来源：http://wdc.jinqigufen.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ueh.havefunace.top

Java: // 无默认参数：方法重载或 Optional
来源：http://rsh.mhx1999.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hzt.tanke756.top

Ruby: def greet(name = "World") = name
来源：http://rnu.yfazqb.com

C#:   string Greet(string name = "World") => name;
来源：http://tws.9152youxi.cn

[C03] 可变参数
来源：http://rfr.yueranfly.top

Py:   def total(*args): return sum(args)
来源：http://tex.zhiwuduotai.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fed.redwolf501.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://uvy.bjfxy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bbz.chenzaomai.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fbf.aibaodan.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sss.kuanghao11.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qhy.vehdjk.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ocr.epnwcf.com

[C04] 命名参数 / 关键字参数
来源：http://cpj.hesvh.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fmu.yfazqb.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://uja.zhengqikj.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fbd.hnxiangtu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wrk.gotoacloud.top

Java: // 无：用 Builder 模式或 record
来源：http://bui.yj20258888.top

Go:   // 无：用配置结构体参数
来源：http://ngn.0kj1m.cn

Ruby: f(a: 1, b: 2)
来源：http://izq.redwolf501.top

C#:   f(a: 1, b: 2)
来源：http://wvz.yueranfly.top

[C05] 返回多个值
来源：http://hcm.yanxiufei.cn

Py:   return a, b
来源：http://rdb.smart0.xyz

PHP:  return [$a, $b];
来源：http://xws.yuanzhike.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://bcj.zhixingplan.top

TS:   return { a, b };
来源：http://ycr.smart0.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wbz.zdbjq.cn

Go:   return a, b
来源：http://qwr.zhengqikj.top

Ruby: return a, b
来源：http://aim.zhengqikj.top

C#:   return (a, b);              // ValueTuple
来源：http://nwv.iojbl.cn

[C06] 匿名函数 / lambda
来源：http://yoe.andypj.xyz

Py:   square = lambda x: x * x
来源：http://gjm.redwolf501.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ynm.zhijiandao.cn

JS:   const square = x => x * x;
来源：http://ero.shanyushiyangtech.top

TS:   const square = (x: number): number => x * x;
来源：http://vjm.yj20258888.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://aqh.gotoacloud.top

Go:   sq := func(x int) int { return x * x }
来源：http://xht.vqdsnc.cn

Ruby: square = ->(x) { x * x }
来源：http://gkd.zhiwuduotai.top

C#:   Func<int, int> square = x => x * x;
来源：http://fio.guowangkeji.top

[C07] 把函数作为参数传入
来源：http://cif.fktsv.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xvw.sufxvd.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xex.fktsv.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qba.nanxuanxn.top

TS:   arr.map(String)
来源：http://lvn.yongpay.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xac.pengpengdd.cyou

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ept.yueranfly.top

Ruby: arr.map(&:upcase)
来源：http://vfd.fanxiaobao.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://jxu.xziqi.cn

[C08] 闭包
来源：http://cru.svipenyu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://skf.guowangkeji.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nms.cucudq.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nuv.hnqzz.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ick.birdmap.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jkr.haohaochexian.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lvg.fehbvm.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yyd.epnwcf.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://auf.jyoumei.cn

[C09] 递归
来源：http://wmo.wangshuangyany.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sxr.hysaishi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gka.zhiwuduotai.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qqi.ctjpmb.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jsn.tianlin.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uys.redwolf501.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://odp.gogol.net.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dze.yangfankeji.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://eew.chenjidiqi.icu

[C10] 变量作用域
来源：http://oxx.ehwqpu.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dvm.shanyushiyangtech.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qiy.9152youxi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xgw.ppjwa.cn

TS:   同 JS
来源：http://ayn.nwbrower.top

Java: 方法内为块级作用域
来源：http://iqg.hesvh.cn

Go:   花括号块级作用域
来源：http://jfh.nanxuanxn.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ucl.ppjwa.cn

C#:   块级作用域
来源：http://blg.zhengqikj.top

[C11] 模块导入与导出
来源：http://ykb.hnqzz.top

Py:   from module import func
来源：http://uqj.yongpay.top

PHP:  require "file.php";  或 use App\Service;
来源：http://cxb.pengpengdd.cyou

JS:   export default function f() {};  import f from "./m.js";
来源：http://chz.xingfuxueyuan.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fih.hfpthk.cn

Java: import java.util.List;
来源：http://vrd.iojbl.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kpy.tianlin.xyz

Ruby: require "json"; require_relative "./util"
来源：http://sxg.hfpthk.cn

C#:   using System.Text;
来源：http://tyt.dianchejie.cn

[C12] 立即执行函数 IIFE
来源：http://mjt.zdqjudy.top

Py:   (lambda: print("run"))()
来源：http://ubi.ctjpmb.com

PHP:  (function () { echo "run"; })();
来源：http://uyb.jqgfzy.top

JS:   (() => { console.log("run"); })();
来源：http://wgm.hnxiangtu.top

TS:   (() => { console.log("run"); })();
来源：http://isi.yvedp.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bit.zhijiandao.cn

Go:   func() { fmt.Println("run") }()
来源：http://mhb.fehbvm.com

Ruby: -> { puts "run" }.call
来源：http://rhc.cqqwz.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://pqg.ivvv.top

[C13] 类型声明 / 类型注解
来源：http://sko.wangshuangyany.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://keb.bjfxy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jxz.hfpthk.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rjf.yongpay.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wdh.ivvv.top

Java: int add(int a, int b) { return a + b; }
来源：http://lwa.yj20258.top

Go:   func add(a, b int) int
来源：http://jvk.chenlongwang.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ajw.guannengcc.top

C#:   int Add(int a, int b) => a + b;
来源：http://eoc.gotoacloud.top

[C14] 泛型函数
来源：http://qey.sxryk.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uyb.52xcode.cn

PHP:  // 无泛型
来源：http://soh.jinyuanbaomall.cn

JS:   // 无泛型
来源：http://nxr.pycfn.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xel.xingfuxueyuan.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wfb.hesvh.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vfo.fktsv.cn

Ruby: # 无泛型
来源：http://xne.yueranfly.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rzr.meibo888.top

[C15] 解构 / 展开参数
来源：http://cml.tanke756.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vyg.jqgufenzy.top

PHP:  [$a, $b] = $pair;
来源：http://ttn.shanyushiyangkeji.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pdw.dashuyun.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qsy.shangyingyoupin.top

Java: // 无解构
来源：http://per.fktsv.cn

Go:   // 无解构
来源：http://bhl.316326.xyz

Ruby: a, b = pair
来源：http://tya.kuanghao11.cn

C#:   var (a, b) = pair;
来源：http://wmg.jianghu66.top

[C16] 函数 / 方法重载
来源：http://yby.jinghuilouyu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rmn.yonumen.top

PHP:  // 无重载
来源：http://tfu.jinqigfzy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://tuk.chenzaomai.com

TS:   // 用联合类型或重载签名声明
来源：http://vfc.yj20258.top

Java: void f(int a) {}  void f(String a) {}
来源：http://slp.yfazqb.com

Go:   // 无重载：用不同函数名
来源：http://dsi.hongshengwenyu.top

Ruby: # 无重载：靠动态参数
来源：http://aao.iojbl.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://lvk.smart0.xyz

================================================================================
来源：http://bwu.yj20258.top

D. 数组 / 列表 / 集合
来源：http://olf.aizwys.cn

================================================================================
来源：http://pqn.xylfe.cn

[D01] 创建数组 / 列表
来源：http://hmn.mhx1999.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://mby.yj20258888.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qsh.jqgfzy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ram.ydjk.org.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wrj.sufxvd.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yer.zhiwuduotai.top

Go:   arr := []int{1, 2, 3}
来源：http://ysu.yfazqb.com

Ruby: arr = [1, 2, 3]
来源：http://inp.mhx1999.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cxq.hammf.cn

[D02] 追加元素到末尾
来源：http://xtp.c1oappe.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dyt.uphjek.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cnh.cdnleiting.top

JS:   arr.push(4);
来源：http://gxm.zhiwuduotai.top

TS:   arr.push(4);
来源：http://ppx.ywan-chungtsiang.top

Java: list.add(4);
来源：http://ssl.xuanzx.com

Go:   arr = append(arr, 4)
来源：http://dtu.tarul.cn

Ruby: arr << 4; arr.push(5)
来源：http://pqb.fktsv.cn

C#:   list.Add(4);
来源：http://kqd.daxiang520.top

[D03] 在指定位置插入元素
来源：http://qhf.havefunace.top

Py:   arr.insert(0, 0)
来源：http://dbd.zhijiandao.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://psa.xylfe.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://utu.hongshengwenyu.top

TS:   arr.splice(0, 0, 0);
来源：http://exl.sjlbkw.cn

Java: list.add(0, 0);
来源：http://uie.zhixingplan.top

Go:   arr = append([]int{0}, arr...)
来源：http://ifl.hammf.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://arl.cucudq.cn

C#:   list.Insert(0, 0);
来源：http://oxq.meibo888.top

[D04] 删除元素
来源：http://sho.chenjidiqi.icu

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wbo.wangdashe.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://glw.pengpengdd.cyou

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rvy.meibo888.top

TS:   arr.splice(0, 1);
来源：http://ajh.bjfxy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tne.jqgfzy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ljf.hnxiangtu.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hlv.zhongyouzk.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wqt.316326.xyz

[D05] 访问与修改元素
来源：http://ogw.yvedp.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wjf.zhixingplan.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://utc.sweek.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://quw.nanxinkj.top

TS:   arr[0]; arr.at(-1);
来源：http://fdp.yanxiufei.cn

Java: list.get(0); list.set(0, 9);
来源：http://fdb.ydzc1.top

Go:   arr[0]; arr[0] = 9
来源：http://ice.xingfuxueyuan.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lum.yueranfly.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://axf.wangshuangyany.cn

[D06] 数组长度
来源：http://zdx.yonumen.top

Py:   len(arr)
来源：http://mgv.zhongyouzk.top

PHP:  count($arr);
来源：http://htx.haohaochexian.top

JS:   arr.length
来源：http://ouy.hesvh.cn

TS:   arr.length
来源：http://amv.hnqzz.top

Java: list.size();
来源：http://hlw.zycfv.cn

Go:   len(arr)
来源：http://ibk.zdbjq.cn

Ruby: arr.length; arr.size
来源：http://ibj.yuxming.cn

C#:   list.Count;
来源：http://lmp.9152youxi.cn

[D07] 切片 / 取子数组
来源：http://sqc.guowangkeji.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://puj.cdnleiting.top

PHP:  array_slice($arr, 1, 3);
来源：http://vki.fktsv.cn

JS:   arr.slice(1, 4);
来源：http://ufo.cucudq.cn

TS:   arr.slice(1, 4);
来源：http://jop.xuetiantiany.cn

Java: list.subList(1, 4);
来源：http://dhk.feifeiyinyue.top

Go:   arr[1:4]
来源：http://prk.sjlbkw.cn

Ruby: arr[1, 3]
来源：http://wis.shzxlz.cn

C#:   list.GetRange(1, 3);
来源：http://jbd.mhx1999.top

[D08] 合并两个数组
来源：http://hws.wangshuangyany.cn

Py:   a + b;  a.extend(b)
来源：http://crk.zhaomingkeji.xyz

PHP:  array_merge($a, $b);
来源：http://cdh.snrcjt.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://tpg.wangdashe.top

TS:   [...a, ...b];
来源：http://yly.iojbl.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://aua.mhx1999.top

Go:   append(a, b...)
来源：http://ghc.nwbrower.top

Ruby: a + b;  a.concat(b)
来源：http://ivh.xuanzx.com

C#:   a.Concat(b).ToList()
来源：http://dfn.cheryme.top

[D09] 排序（升序）
来源：http://bom.uphjek.com

Py:   sorted(arr);  arr.sort()
来源：http://tix.yangfankeji.com

PHP:  sort($arr);
来源：http://nzy.ppjwa.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lue.cucudq.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://sjv.fzhhl.top

Java: Collections.sort(list);  list.sort(null);
来源：http://qwn.hesvh.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zkm.yj202588.top

Ruby: arr.sort
来源：http://iup.fengsongda.top

C#:   list.Sort();
来源：http://hkc.cucudq.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://rxd.hcnkem.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pfe.hysaishi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://owz.snrcjt.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pub.jyoumei.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fzn.yonumen.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://eis.ehwqpu.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wza.vehdjk.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://djc.vqdsnc.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jrb.0kj1m.cn

[D11] 反转数组
来源：http://kvj.zdqjudy.top

Py:   arr[::-1];  arr.reverse()
来源：http://zgl.svipenyu.cn

PHP:  array_reverse($arr);
来源：http://iep.jinqigfzy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qkj.nanxinkj.top

TS:   [...arr].reverse();
来源：http://laq.pycfn.com

Java: Collections.reverse(list);
来源：http://xyv.nanxinkj.top

Go:   slices.Reverse(arr)
来源：http://jlu.tian-w.cn

Ruby: arr.reverse
来源：http://srf.jyoumei.cn

C#:   list.Reverse();
来源：http://xog.yfazqb.com

[D12] 查找元素下标
来源：http://uvo.andypj.xyz

Py:   arr.index(x);  x in arr
来源：http://qlz.9152youxi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kxs.hfpthk.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hlt.hcnkem.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lys.fehbvm.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xzs.ydzc1.top

Go:   slices.Index(arr, x)
来源：http://cfb.hesvh.cn

Ruby: arr.index(x)
来源：http://qht.ywan-chungtsiang.top

C#:   list.IndexOf(x);
来源：http://mpm.yfazqb.com

[D13] 过滤（保留满足条件的）
来源：http://frf.zycfv.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fou.xingfuxueyuan.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vkd.ehwqpu.com

JS:   arr.filter(x => x > 3)
来源：http://cgq.yuanzhike.top

TS:   arr.filter(x => x > 3)
来源：http://bmr.jinghuilouyu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rmm.guowangkeji.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fas.pycfn.com

Ruby: arr.select { |x| x > 3 }
来源：http://bmz.tian-w.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://yky.jlsjyb.cn

[D14] 映射转换（每个元素变形）
来源：http://vxs.yanxiufei.cn


<!-- 参考信息 -->