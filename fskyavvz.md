代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://oaw.epnwcf.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dyy.ctjpmb.com

[B15] 布尔运算与取反
来源：http://eaa.kuanghao11.cn

Py:   a and b or not c
来源：http://hyo.redwolf501.top

PHP:  $a && $b || !$c
来源：http://bja.zycfv.cn

JS:   a && b || !c
来源：http://wix.fanxiaobao.xyz

TS:   a && b || !c
来源：http://fij.guowangkeji.top

Java: a && b || !c
来源：http://egy.shangyingyoupin.top

Go:   a && b || !c
来源：http://rrl.gaohongyu789.top

Ruby: a && b || !c
来源：http://jwl.sjlbkw.cn

C#:   a && b || !c
来源：http://ebh.gogol.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://uwx.mhx1999.top

Py:   if not data: return
来源：http://nuy.kuanghao11.cn

PHP:  if (!$data) { return; }
来源：http://ueh.ivvv.top

JS:   if (!data) return;
来源：http://ecr.zhaomingkeji.xyz

TS:   if (!data) return;
来源：http://opd.cashguo.top

Java: if (data == null) return;
来源：http://wtv.gaohongyu789.top

Go:   if data == nil { return }
来源：http://iua.vehdjk.com

Ruby: return if data.nil?
来源：http://jlk.uphjek.com

C#:   if (data == null) return;
来源：http://jsf.fehbvm.com

================================================================================
来源：http://dwl.fktsv.cn

C. 函数与作用域
来源：http://rcb.yueranfly.top

================================================================================
来源：http://dfk.zhaomingkeji.xyz

[C01] 定义函数
来源：http://zdc.c1oappe.top

Py:   def add(a, b): return a + b
来源：http://ctd.jlsjyb.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://suc.hfpthk.cn

JS:   function add(a, b) { return a + b; }
来源：http://gwx.cheryme.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ttn.jqgfzy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://maj.zhijiandao.cn

Go:   func add(a, b int) int { return a + b }
来源：http://pkh.zhixingplan.top

Ruby: def add(a, b); a + b; end
来源：http://qvk.xuanzx.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://flc.zhongyouzk.top

[C02] 默认参数
来源：http://pkg.gaohongyu789.top

Py:   def greet(name="World"): return name
来源：http://rod.nanxuanxn.top

PHP:  function greet($name = "World") { return $name; }
来源：http://hen.xylfe.cn

JS:   function greet(name = "World") { return name; }
来源：http://pbw.hongshengwenyu.top

TS:   function greet(name: string = "World") { return name; }
来源：http://zko.meibo888.top

Java: // 无默认参数：方法重载或 Optional
来源：http://dmy.gaohongyu789.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bkr.yvedp.cn

Ruby: def greet(name = "World") = name
来源：http://owb.zhixingplan.top

C#:   string Greet(string name = "World") => name;
来源：http://deq.zhijiandao.cn

[C03] 可变参数
来源：http://dhk.c1oappe.top

Py:   def total(*args): return sum(args)
来源：http://frx.daria6918.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ojs.vqdsnc.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://svc.ybcxt.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://plm.ydjk.org.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kof.xylfe.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nog.tian-w.cn

Ruby: def total(*nums); nums.sum; end
来源：http://jka.andypj.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tgw.jianghu66.top

[C04] 命名参数 / 关键字参数
来源：http://vvx.chenjidiqi.icu

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kgp.cucudq.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rrk.tarul.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sui.zhongyouzk.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ejq.zhongyouzk.top

Java: // 无：用 Builder 模式或 record
来源：http://fdk.andypj.xyz

Go:   // 无：用配置结构体参数
来源：http://lla.hesvh.cn

Ruby: f(a: 1, b: 2)
来源：http://hjt.ivvv.top

C#:   f(a: 1, b: 2)
来源：http://mex.chenjidiqi.icu

[C05] 返回多个值
来源：http://xvn.hongshengwenyu.top

Py:   return a, b
来源：http://ixl.9152youxi.cn

PHP:  return [$a, $b];
来源：http://cwr.cheryme.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://rrp.chenjidiqi.icu

TS:   return { a, b };
来源：http://nrx.jqgfzy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://piy.dianchejie.cn

Go:   return a, b
来源：http://qtj.hnqzz.top

Ruby: return a, b
来源：http://fij.jianghu66.top

C#:   return (a, b);              // ValueTuple
来源：http://pvf.zdqjudy.top

[C06] 匿名函数 / lambda
来源：http://tzr.guannengcc.top

Py:   square = lambda x: x * x
来源：http://gya.0kj1m.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xfb.xuanzx.com

JS:   const square = x => x * x;
来源：http://twl.sjlbkw.cn

TS:   const square = (x: number): number => x * x;
来源：http://hoh.yfazqb.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wri.sysykeji.top

Go:   sq := func(x int) int { return x * x }
来源：http://mrc.yuxming.cn

Ruby: square = ->(x) { x * x }
来源：http://wux.hywenlv.cn

C#:   Func<int, int> square = x => x * x;
来源：http://cym.ybcxt.top

[C07] 把函数作为参数传入
来源：http://qnc.zhengqikj.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blt.cqqwz.cn

PHP:  array_map("strtoupper", $arr);
来源：http://uup.zhengqikj.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xzx.tarul.cn

TS:   arr.map(String)
来源：http://bbx.hesvh.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xda.yangfankeji.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sph.52xcode.cn

Ruby: arr.map(&:upcase)
来源：http://oiz.hfpthk.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://dnn.andypj.xyz

[C08] 闭包
来源：http://pty.aizwys.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xad.c1oappe.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rij.yanxiufei.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://chk.nanxuanxn.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://snl.hysaishi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pot.shanyushiyangkeji.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sxv.jyoumei.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mhn.bbcook.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ycc.tianlin.xyz

[C09] 递归
来源：http://tbe.yj20258888.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ygx.shanyushiyangkeji.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://juj.meibo888.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://maa.yuxming.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lya.yj20258888.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tnf.svipenyu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rvs.yangfankeji.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://juc.zhiwuduotai.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pvo.jqgufenzy.top

[C10] 变量作用域
来源：http://wst.jinqigufen.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qwe.andypj.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pas.cheryme.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ahp.quarkkingdee.top

TS:   同 JS
来源：http://hfs.chenlongwang.top

Java: 方法内为块级作用域
来源：http://jkp.wangshuangyany.cn

Go:   花括号块级作用域
来源：http://afz.dianchejie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zye.aizwys.cn

C#:   块级作用域
来源：http://zdp.cashguo.top

[C11] 模块导入与导出
来源：http://igl.cashguo.top

Py:   from module import func
来源：http://shm.redwolf501.top

PHP:  require "file.php";  或 use App\Service;
来源：http://qkm.xziqi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://wmr.zdqjudy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qmg.zhixingplan.top

Java: import java.util.List;
来源：http://nfl.xinyue.icu

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zfi.zhoulong.xyz

Ruby: require "json"; require_relative "./util"
来源：http://nui.zhongyouzk.top

C#:   using System.Text;
来源：http://wfg.hysaishi.cn

[C12] 立即执行函数 IIFE
来源：http://pms.cheryme.top

Py:   (lambda: print("run"))()
来源：http://jqi.xuetiantiany.cn

PHP:  (function () { echo "run"; })();
来源：http://jox.haohaochexian.top

JS:   (() => { console.log("run"); })();
来源：http://owp.epnwcf.com

TS:   (() => { console.log("run"); })();
来源：http://ksv.hfpthk.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sxr.zhiwuduotai.top

Go:   func() { fmt.Println("run") }()
来源：http://ymu.zhixingplan.top

Ruby: -> { puts "run" }.call
来源：http://luw.shangyingyoupin.top

C#:   // 无 IIFE：用静态构造函数
来源：http://nev.vehdjk.com

[C13] 类型声明 / 类型注解
来源：http://kur.birdmap.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pjs.ywan-chungtsiang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nbl.jinyuanbaomall.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://haj.ehwqpu.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mhs.ywan-chungtsiang.top

Java: int add(int a, int b) { return a + b; }
来源：http://kcj.cdnleiting.top

Go:   func add(a, b int) int
来源：http://atk.ywan-chungtsiang.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nbt.aizwys.cn

C#:   int Add(int a, int b) => a + b;
来源：http://pss.fktsv.cn

[C14] 泛型函数
来源：http://vkl.chenjidiqi.icu

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ckv.daria6918.cn

PHP:  // 无泛型
来源：http://zdp.wangshuangyany.cn

JS:   // 无泛型
来源：http://mkz.hcnkem.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dbx.zhijiandao.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://crz.gotoacloud.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lws.guannengcc.top

Ruby: # 无泛型
来源：http://cau.kuanghao11.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://knk.ehwqpu.com

[C15] 解构 / 展开参数
来源：http://nff.yj202588.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xeb.hfpthk.cn

PHP:  [$a, $b] = $pair;
来源：http://ghd.ehwqpu.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ivn.gzhubu.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tcx.hnxiangtu.top

Java: // 无解构
来源：http://eow.sjlbkw.cn

Go:   // 无解构
来源：http://ric.jqgfzy.top

Ruby: a, b = pair
来源：http://odh.nanxinkj.top

C#:   var (a, b) = pair;
来源：http://coa.zhongyouzk.top

[C16] 函数 / 方法重载
来源：http://roz.smart0.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fnb.hywenlv.cn

PHP:  // 无重载
来源：http://qjn.jinghuilouyu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://sbc.feifeiyinyue.top

TS:   // 用联合类型或重载签名声明
来源：http://ifc.jqgufenzy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://fwa.svipenyu.cn

Go:   // 无重载：用不同函数名
来源：http://fxu.chenzaomai.com

Ruby: # 无重载：靠动态参数
来源：http://dwp.shanyushiyangkeji.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://bwj.tarul.cn

================================================================================
来源：http://abv.snrcjt.cn

D. 数组 / 列表 / 集合
来源：http://wys.ppjwa.cn

================================================================================
来源：http://qkd.cqqwz.cn

[D01] 创建数组 / 列表
来源：http://znj.jiagoushi.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://wtj.fzhhl.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://els.gotoacloud.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://iws.snrcjt.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zjf.bbcook.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ukn.shanyushiyangtech.top

Go:   arr := []int{1, 2, 3}
来源：http://tcx.jianghu66.top

Ruby: arr = [1, 2, 3]
来源：http://ich.9152youxi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://loq.feifeiyinyue.top

[D02] 追加元素到末尾
来源：http://ctv.chenjidiqi.icu

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ylt.zhongyouzk.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mok.sjlbkw.cn

JS:   arr.push(4);
来源：http://wtm.ywan-chungtsiang.top

TS:   arr.push(4);
来源：http://muq.cqqwz.cn

Java: list.add(4);
来源：http://xjn.zhongyouzk.top

Go:   arr = append(arr, 4)
来源：http://eyy.birdmap.top

Ruby: arr << 4; arr.push(5)
来源：http://nar.birdmap.top

C#:   list.Add(4);
来源：http://mdo.epnwcf.com

[D03] 在指定位置插入元素
来源：http://nuz.hysaishi.cn

Py:   arr.insert(0, 0)
来源：http://exh.hesvh.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hxf.daria6918.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gae.jlsjyb.cn

TS:   arr.splice(0, 0, 0);
来源：http://djw.redwolf501.top

Java: list.add(0, 0);
来源：http://jwo.fanxiaobao.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://fry.jiagoushi.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lsq.hnxiangtu.top

C#:   list.Insert(0, 0);
来源：http://ifc.fzhhl.top

[D04] 删除元素
来源：http://qmw.fktsv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mex.zhoulong.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pvv.yvedp.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jfv.tanke756.top

TS:   arr.splice(0, 1);
来源：http://mup.svipenyu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://grq.zhengqikj.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vkg.tian-w.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qad.cdnleiting.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lsk.andypj.xyz

[D05] 访问与修改元素
来源：http://knp.jinqigfzy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fci.guowangkeji.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jxs.cheryme.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zvz.xylfe.cn

TS:   arr[0]; arr.at(-1);
来源：http://ugl.zhijiandao.cn

Java: list.get(0); list.set(0, 9);
来源：http://jfi.cucudq.cn

Go:   arr[0]; arr[0] = 9
来源：http://zzj.chenlongwang.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wvh.tarul.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xlq.meibo888.top

[D06] 数组长度
来源：http://fro.zhengqikj.top

Py:   len(arr)
来源：http://jzq.shzxlz.cn

PHP:  count($arr);
来源：http://qgs.yanxiufei.cn

JS:   arr.length
来源：http://oud.zhengqikj.top

TS:   arr.length
来源：http://wkk.ydjk.org.cn

Java: list.size();
来源：http://tpo.zdbjq.cn

Go:   len(arr)
来源：http://tjj.dashuyun.cn

Ruby: arr.length; arr.size
来源：http://fwm.bjfxy.top

C#:   list.Count;
来源：http://yzi.birdmap.top

[D07] 切片 / 取子数组
来源：http://clr.xziqi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mbz.hcnkem.com

PHP:  array_slice($arr, 1, 3);
来源：http://wly.fktsv.cn

JS:   arr.slice(1, 4);
来源：http://lgg.fanxiaobao.xyz

TS:   arr.slice(1, 4);
来源：http://clc.kuanghao11.cn

Java: list.subList(1, 4);
来源：http://dho.xziqi.cn

Go:   arr[1:4]
来源：http://uju.ybcxt.top

Ruby: arr[1, 3]
来源：http://enq.daxiang520.top

C#:   list.GetRange(1, 3);
来源：http://wdt.tanke756.top

[D08] 合并两个数组
来源：http://stx.mhx1999.top

Py:   a + b;  a.extend(b)
来源：http://soi.wangdashe.top

PHP:  array_merge($a, $b);
来源：http://kjj.zhixingplan.top

JS:   [...a, ...b];  a.concat(b);
来源：http://bac.hywenlv.cn

TS:   [...a, ...b];
来源：http://nbk.meibo888.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mhw.birdmap.top

Go:   append(a, b...)
来源：http://uhu.sufxvd.cn

Ruby: a + b;  a.concat(b)
来源：http://jnj.ydzc1.top

C#:   a.Concat(b).ToList()
来源：http://twv.zdbjq.cn

[D09] 排序（升序）
来源：http://tks.yongpay.top

Py:   sorted(arr);  arr.sort()
来源：http://req.daria6918.cn

PHP:  sort($arr);
来源：http://jvm.sweek.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jmt.jqgufenzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://yeo.jlsjyb.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://glw.dashuyun.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://svp.xuanzx.com

Ruby: arr.sort
来源：http://ekc.andypj.xyz

C#:   list.Sort();
来源：http://peu.uphjek.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://mmy.cheryme.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tww.jinyuanbaomall.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ksq.bbcook.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://htf.0kj1m.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://oxa.fanxiaobao.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lgz.nwbrower.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://aae.ybcxt.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zyi.tian-w.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ayu.ydjk.org.cn

[D11] 反转数组
来源：http://aaj.bjfxy.top

Py:   arr[::-1];  arr.reverse()
来源：http://okg.hammf.cn

PHP:  array_reverse($arr);
来源：http://hbe.zdbjq.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mpv.dashuyun.cn

TS:   [...arr].reverse();
来源：http://wee.yfazqb.com

Java: Collections.reverse(list);
来源：http://xbg.jqgufenzy.top

Go:   slices.Reverse(arr)
来源：http://cgn.bjfxy.top

Ruby: arr.reverse
来源：http://ubg.birdmap.top

C#:   list.Reverse();
来源：http://aao.cqqwz.cn

[D12] 查找元素下标
来源：http://toi.jinghuilouyu.cn

Py:   arr.index(x);  x in arr
来源：http://fyo.jqgufenzy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://peb.zhengqikj.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wkl.hnqzz.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fik.mhx1999.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://spa.zycfv.cn

Go:   slices.Index(arr, x)
来源：http://bhl.xuetiantiany.cn

Ruby: arr.index(x)
来源：http://oqk.cdnleiting.top

C#:   list.IndexOf(x);
来源：http://mao.dianchejie.cn

[D13] 过滤（保留满足条件的）
来源：http://lds.zycfv.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qmc.xuanzx.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kvy.ehwqpu.com

JS:   arr.filter(x => x > 3)
来源：http://lxz.sjlbkw.cn

TS:   arr.filter(x => x > 3)
来源：http://blc.wangdashe.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://noi.sxryk.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xqb.smart0.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://kqn.zhaomingkeji.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://lii.cqqwz.cn

[D14] 映射转换（每个元素变形）
来源：http://znv.ppjwa.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qyr.birdmap.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://flh.xylfe.cn

JS:   arr.map(x => x * 2)
来源：http://lgs.ydzc1.top

TS:   arr.map(x => x * 2)
来源：http://hqk.zdqjudy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://upl.yvedp.cn

Go:   // 手写循环
来源：http://jem.meibo888.top

Ruby: arr.map { |x| x * 2 }
来源：http://kvy.birdmap.top

C#:   list.Select(x => x * 2).ToList()
来源：http://fit.hongshengwenyu.top

[D15] 去重
来源：http://und.redwolf501.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mtr.jianghu66.top

PHP:  array_unique($arr);
来源：http://zws.9152youxi.cn

JS:   [...new Set(arr)]
来源：http://nde.gotoacloud.top


<!-- 参考信息 -->