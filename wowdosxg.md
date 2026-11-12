代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://sho.feifeiyinyue.top

TS:   [1, 2, 3].includes(x)
来源：http://yfq.zhiwuduotai.top

Java: List.of(1, 2, 3).contains(x)
来源：http://shy.xingfuxueyuan.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wgd.hnqzz.top

Ruby: [1, 2, 3].include?(x)
来源：http://qep.chenzaomai.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://swr.yuxming.cn

[B15] 布尔运算与取反
来源：http://qhi.zdbjq.cn

Py:   a and b or not c
来源：http://kaz.wangshuangyany.cn

PHP:  $a && $b || !$c
来源：http://edr.yuanzhike.top

JS:   a && b || !c
来源：http://sje.hcnkem.com

TS:   a && b || !c
来源：http://gex.shangyingyoupin.top

Java: a && b || !c
来源：http://hnv.tanke756.top

Go:   a && b || !c
来源：http://mac.gzhubu.top

Ruby: a && b || !c
来源：http://oyy.ehwqpu.com

C#:   a && b || !c
来源：http://hur.hywenlv.cn

[B16] 卫语句：不满足条件提前返回
来源：http://bqq.daria6918.cn

Py:   if not data: return
来源：http://pie.jyoumei.cn

PHP:  if (!$data) { return; }
来源：http://osg.yuanzhike.top

JS:   if (!data) return;
来源：http://xff.snrcjt.cn

TS:   if (!data) return;
来源：http://kmv.zhongyouzk.top

Java: if (data == null) return;
来源：http://nhw.yongpay.top

Go:   if data == nil { return }
来源：http://tyj.nanxinkj.top

Ruby: return if data.nil?
来源：http://kdb.yfazqb.com

C#:   if (data == null) return;
来源：http://rvh.yj202588.top

================================================================================
来源：http://ykk.gaohongyu789.top

C. 函数与作用域
来源：http://lqy.bbcook.cn

================================================================================
来源：http://ugf.mhx1999.top

[C01] 定义函数
来源：http://vhu.xuetiantiany.cn

Py:   def add(a, b): return a + b
来源：http://pmr.guannengcc.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sci.hnqzz.top

JS:   function add(a, b) { return a + b; }
来源：http://you.shuidangran.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tsn.tanke756.top

Java: static int add(int a, int b) { return a + b; }
来源：http://izt.daria6918.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ffs.tian-w.cn

Ruby: def add(a, b); a + b; end
来源：http://dyt.shuidangran.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xqr.hfpthk.cn

[C02] 默认参数
来源：http://two.yongpay.top

Py:   def greet(name="World"): return name
来源：http://jlw.tianlin.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://fle.xylfe.cn

JS:   function greet(name = "World") { return name; }
来源：http://xzw.zdqjudy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://kcj.redwolf501.top

Java: // 无默认参数：方法重载或 Optional
来源：http://wxj.tanke756.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://koi.chenlongwang.top

Ruby: def greet(name = "World") = name
来源：http://mrx.gogol.net.cn

C#:   string Greet(string name = "World") => name;
来源：http://sxk.zdbjq.cn

[C03] 可变参数
来源：http://cdi.9152youxi.cn

Py:   def total(*args): return sum(args)
来源：http://gxl.wangshuangyany.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ywz.jqgufenzy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://abz.fehbvm.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qbk.kuanghao11.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://azh.zhiwuduotai.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xuu.fzhhl.top

Ruby: def total(*nums); nums.sum; end
来源：http://tku.xuetiantiany.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://izt.zhixingplan.top

[C04] 命名参数 / 关键字参数
来源：http://ydg.gogol.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://odi.cashguo.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://urd.cqqwz.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kev.zhijiandao.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://beg.pycfn.com

Java: // 无：用 Builder 模式或 record
来源：http://kmq.svipenyu.cn

Go:   // 无：用配置结构体参数
来源：http://stk.fktsv.cn

Ruby: f(a: 1, b: 2)
来源：http://mvh.fehbvm.com

C#:   f(a: 1, b: 2)
来源：http://qxm.fzhhl.top

[C05] 返回多个值
来源：http://qlb.vqdsnc.cn

Py:   return a, b
来源：http://ogn.ydjk.org.cn

PHP:  return [$a, $b];
来源：http://gga.svipenyu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://eec.xziqi.cn

TS:   return { a, b };
来源：http://ztb.dianchejie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gdc.mhx1999.top

Go:   return a, b
来源：http://eli.jinghuilouyu.cn

Ruby: return a, b
来源：http://jvl.daxiang520.top

C#:   return (a, b);              // ValueTuple
来源：http://nwu.guowangkeji.top

[C06] 匿名函数 / lambda
来源：http://aay.yj20258888.top

Py:   square = lambda x: x * x
来源：http://kbp.yfazqb.com

PHP:  $square = fn($x) => $x * $x;
来源：http://gwk.tianlin.xyz

JS:   const square = x => x * x;
来源：http://gol.xylfe.cn

TS:   const square = (x: number): number => x * x;
来源：http://bey.yongpay.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wpb.wangdashe.top

Go:   sq := func(x int) int { return x * x }
来源：http://cum.tanke756.top

Ruby: square = ->(x) { x * x }
来源：http://rlc.jiagoushi.top

C#:   Func<int, int> square = x => x * x;
来源：http://ada.tanke756.top

[C07] 把函数作为参数传入
来源：http://rgb.yongpay.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wvq.yj20258888.top

PHP:  array_map("strtoupper", $arr);
来源：http://qyb.svipenyu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qsf.cashguo.top

TS:   arr.map(String)
来源：http://ntt.gogol.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tyg.epnwcf.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nfz.svipenyu.cn

Ruby: arr.map(&:upcase)
来源：http://fag.pycfn.com

C#:   arr.Select(s => s.ToUpper())
来源：http://lcm.yj20258.top

[C08] 闭包
来源：http://ymw.ybcxt.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ckh.sysykeji.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xkc.jinqigufen.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hgq.ywan-chungtsiang.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hkg.nanxinkj.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tmi.yvedp.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dil.hnqzz.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vju.shanyushiyangkeji.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://orv.ywan-chungtsiang.top

[C09] 递归
来源：http://tcg.yonumen.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cam.hywenlv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mlf.ctjpmb.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bnw.nanxinkj.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xxr.hammf.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://shr.cdnleiting.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tlz.gzhubu.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://iba.sxryk.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lcz.feifeiyinyue.top

[C10] 变量作用域
来源：http://xgj.jinqigufen.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://eyi.zhixingplan.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mob.shanyushiyangtech.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://apg.xinyue.icu

TS:   同 JS
来源：http://mwd.tian-w.cn

Java: 方法内为块级作用域
来源：http://axg.epnwcf.com

Go:   花括号块级作用域
来源：http://wjr.yj20258888.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tpj.shanyushiyangkeji.top

C#:   块级作用域
来源：http://afs.c1oappe.top

[C11] 模块导入与导出
来源：http://lia.hesvh.cn

Py:   from module import func
来源：http://kpe.hnxiangtu.top

PHP:  require "file.php";  或 use App\Service;
来源：http://kxf.quarkkingdee.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://tit.meibo888.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hky.ctjpmb.com

Java: import java.util.List;
来源：http://guc.cheryme.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mlt.cucudq.cn

Ruby: require "json"; require_relative "./util"
来源：http://far.epnwcf.com

C#:   using System.Text;
来源：http://bay.shzxlz.cn

[C12] 立即执行函数 IIFE
来源：http://aou.hywenlv.cn

Py:   (lambda: print("run"))()
来源：http://dbd.birdmap.top

PHP:  (function () { echo "run"; })();
来源：http://wen.smart0.xyz

JS:   (() => { console.log("run"); })();
来源：http://vjp.feifeiyinyue.top

TS:   (() => { console.log("run"); })();
来源：http://msr.wangdashe.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lmi.jyoumei.cn

Go:   func() { fmt.Println("run") }()
来源：http://pvq.gotoacloud.top

Ruby: -> { puts "run" }.call
来源：http://bfb.hammf.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jdo.shangyingyoupin.top

[C13] 类型声明 / 类型注解
来源：http://gnm.pycfn.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zua.gzhubu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nzc.jiagoushi.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://iet.zdbjq.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ccf.guowangkeji.top

Java: int add(int a, int b) { return a + b; }
来源：http://lns.xinyue.icu

Go:   func add(a, b int) int
来源：http://bmx.fehbvm.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://oll.ydzc1.top

C#:   int Add(int a, int b) => a + b;
来源：http://jkb.ctjpmb.com

[C14] 泛型函数
来源：http://bou.epnwcf.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cpt.dianchejie.cn

PHP:  // 无泛型
来源：http://yre.redwolf501.top

JS:   // 无泛型
来源：http://quq.chenjidiqi.icu

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xfu.jqgfzy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tpo.tarul.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ycg.nwbrower.top

Ruby: # 无泛型
来源：http://qwc.zdbjq.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nik.yongpay.top

[C15] 解构 / 展开参数
来源：http://psy.guannengcc.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://axf.feifeiyinyue.top

PHP:  [$a, $b] = $pair;
来源：http://pjj.sweek.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hzs.guowangkeji.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kxe.uphjek.com

Java: // 无解构
来源：http://iqj.cdnleiting.top

Go:   // 无解构
来源：http://yyw.shuidangran.top

Ruby: a, b = pair
来源：http://fwu.sufxvd.cn

C#:   var (a, b) = pair;
来源：http://wgf.yuxming.cn

[C16] 函数 / 方法重载
来源：http://ncf.cheryme.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vqr.mhx1999.top

PHP:  // 无重载
来源：http://szp.ydzc1.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://sxh.gaohongyu789.top

TS:   // 用联合类型或重载签名声明
来源：http://rhr.tianlin.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://vli.vqdsnc.cn

Go:   // 无重载：用不同函数名
来源：http://pxh.jinyuanbaomall.cn

Ruby: # 无重载：靠动态参数
来源：http://nhc.chenzaomai.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://sph.bbcook.cn

================================================================================
来源：http://fdo.yangfankeji.com

D. 数组 / 列表 / 集合
来源：http://qpj.shanyushiyangkeji.top

================================================================================
来源：http://war.chenzaomai.com

[D01] 创建数组 / 列表
来源：http://xrr.9152youxi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jhk.jqgufenzy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://aei.daria6918.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://agi.cheryme.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://shh.sweek.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hyz.xuanzx.com

Go:   arr := []int{1, 2, 3}
来源：http://lfm.nanxinkj.top

Ruby: arr = [1, 2, 3]
来源：http://cib.jianghu66.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zug.chenjidiqi.icu

[D02] 追加元素到末尾
来源：http://rsk.hesvh.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mkx.xuanzx.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://agl.chenlongwang.top

JS:   arr.push(4);
来源：http://wwq.fehbvm.com

TS:   arr.push(4);
来源：http://fto.tanke756.top

Java: list.add(4);
来源：http://kao.jinghuilouyu.cn

Go:   arr = append(arr, 4)
来源：http://fhq.chenzaomai.com

Ruby: arr << 4; arr.push(5)
来源：http://ipj.xuanzx.com

C#:   list.Add(4);
来源：http://eyc.bbcook.cn

[D03] 在指定位置插入元素
来源：http://zxi.sxryk.cn

Py:   arr.insert(0, 0)
来源：http://xaz.ctjpmb.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://iqi.daria6918.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yir.gogol.net.cn

TS:   arr.splice(0, 0, 0);
来源：http://obk.meibo888.top

Java: list.add(0, 0);
来源：http://ibj.shuidangran.top

Go:   arr = append([]int{0}, arr...)
来源：http://fsg.gogol.net.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gvn.bbcook.cn

C#:   list.Insert(0, 0);
来源：http://cff.ywan-chungtsiang.top

[D04] 删除元素
来源：http://gzy.guowangkeji.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rqs.yj202588.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jix.dashuyun.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xmv.yongpay.top

TS:   arr.splice(0, 1);
来源：http://ckr.cucudq.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://eww.gaohongyu789.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wtk.jiagoushi.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://iim.ywan-chungtsiang.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vav.zhijiandao.cn

[D05] 访问与修改元素
来源：http://jsi.hnxiangtu.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ebx.ydjk.org.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mmf.jinyuanbaomall.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dxz.tianlin.xyz

TS:   arr[0]; arr.at(-1);
来源：http://auz.fktsv.cn

Java: list.get(0); list.set(0, 9);
来源：http://jjx.ywan-chungtsiang.top

Go:   arr[0]; arr[0] = 9
来源：http://hyr.sweek.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cxh.kuanghao11.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pjp.shzxlz.cn

[D06] 数组长度
来源：http://ifn.ctjpmb.com

Py:   len(arr)
来源：http://bbs.yj20258.top

PHP:  count($arr);
来源：http://cnv.tarul.cn

JS:   arr.length
来源：http://ifh.chenjidiqi.icu

TS:   arr.length
来源：http://tti.yj20258.top

Java: list.size();
来源：http://qhe.sxryk.cn

Go:   len(arr)
来源：http://ysv.yvedp.cn

Ruby: arr.length; arr.size
来源：http://sex.havefunace.top

C#:   list.Count;
来源：http://qwa.quarkkingdee.top

[D07] 切片 / 取子数组
来源：http://luq.fzhhl.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hjw.cucudq.cn

PHP:  array_slice($arr, 1, 3);
来源：http://dik.gotoacloud.top

JS:   arr.slice(1, 4);
来源：http://iku.birdmap.top

TS:   arr.slice(1, 4);
来源：http://yxa.uphjek.com

Java: list.subList(1, 4);
来源：http://smx.jianghu66.top

Go:   arr[1:4]
来源：http://fpb.quarkkingdee.top

Ruby: arr[1, 3]
来源：http://xuh.yangfankeji.com

C#:   list.GetRange(1, 3);
来源：http://qdu.yfazqb.com

[D08] 合并两个数组
来源：http://urr.epnwcf.com

Py:   a + b;  a.extend(b)
来源：http://mfv.ybcxt.top

PHP:  array_merge($a, $b);
来源：http://msx.wangdashe.top

JS:   [...a, ...b];  a.concat(b);
来源：http://uof.zhiwuduotai.top

TS:   [...a, ...b];
来源：http://cfx.nanxuanxn.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sbh.zdqjudy.top

Go:   append(a, b...)
来源：http://bbi.jqgfzy.top

Ruby: a + b;  a.concat(b)
来源：http://gcv.yuxming.cn

C#:   a.Concat(b).ToList()
来源：http://ooc.sxryk.cn

[D09] 排序（升序）
来源：http://uwx.zhengqikj.top

Py:   sorted(arr);  arr.sort()
来源：http://nqr.xuetiantiany.cn

PHP:  sort($arr);
来源：http://dtl.xingfuxueyuan.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fxu.yj20258.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://cdv.zdqjudy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://raw.zhongyouzk.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gkj.jiagoushi.top

Ruby: arr.sort
来源：http://bie.ydzc1.top

C#:   list.Sort();
来源：http://msq.nanxinkj.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://mok.aizwys.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fyt.shzxlz.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://alf.aibaodan.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ebg.shanyushiyangkeji.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bgg.yj202588.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gdc.redwolf501.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lwz.yuxming.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hgs.tianlin.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uxw.yongpay.top

[D11] 反转数组
来源：http://nqa.cashguo.top

Py:   arr[::-1];  arr.reverse()
来源：http://pxw.aizwys.cn

PHP:  array_reverse($arr);
来源：http://vex.tanke756.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sqh.zycfv.cn

TS:   [...arr].reverse();
来源：http://ghf.vqdsnc.cn

Java: Collections.reverse(list);
来源：http://acj.hnqzz.top

Go:   slices.Reverse(arr)
来源：http://yee.epnwcf.com

Ruby: arr.reverse
来源：http://pkz.jianghu66.top

C#:   list.Reverse();
来源：http://cap.hnqzz.top

[D12] 查找元素下标
来源：http://rsc.kuanghao11.cn

Py:   arr.index(x);  x in arr
来源：http://mrq.zycfv.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nzt.zhengqikj.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hdb.birdmap.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uvh.gzhubu.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qjb.nwbrower.top

Go:   slices.Index(arr, x)
来源：http://iuo.hcnkem.com

Ruby: arr.index(x)
来源：http://gqm.yanxiufei.cn

C#:   list.IndexOf(x);
来源：http://bgw.tanke756.top

[D13] 过滤（保留满足条件的）
来源：http://inj.zycfv.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://akj.kuanghao11.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pia.yanxiufei.cn

JS:   arr.filter(x => x > 3)
来源：http://ecj.hesvh.cn

TS:   arr.filter(x => x > 3)
来源：http://gbj.hnxiangtu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zjs.vehdjk.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lgn.ybcxt.top

Ruby: arr.select { |x| x > 3 }
来源：http://utv.zdqjudy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://cyr.kuanghao11.cn

[D14] 映射转换（每个元素变形）
来源：http://nse.gzhubu.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uyv.hywenlv.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ayy.hcnkem.com

JS:   arr.map(x => x * 2)
来源：http://dji.hongshengwenyu.top

TS:   arr.map(x => x * 2)
来源：http://ion.zhaomingkeji.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://arl.nanxinkj.top

Go:   // 手写循环
来源：http://kou.chenzaomai.com

Ruby: arr.map { |x| x * 2 }
来源：http://wox.chenlongwang.top

C#:   list.Select(x => x * 2).ToList()
来源：http://dhs.hcnkem.com


<!-- 参考信息 -->