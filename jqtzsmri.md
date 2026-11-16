代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://zjf.jiagoushi.top

TS:   [1, 2, 3].includes(x)
来源：http://szn.cheryme.top

Java: List.of(1, 2, 3).contains(x)
来源：http://qgq.zycfv.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ocg.zhijiandao.cn

Ruby: [1, 2, 3].include?(x)
来源：http://wcq.zhoulong.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rhv.zhijiandao.cn

[B15] 布尔运算与取反
来源：http://ybl.jinqigfzy.top

Py:   a and b or not c
来源：http://zjr.zhixingplan.top

PHP:  $a && $b || !$c
来源：http://zoi.fanxiaobao.xyz

JS:   a && b || !c
来源：http://eue.nwbrower.top

TS:   a && b || !c
来源：http://nkc.sysykeji.top

Java: a && b || !c
来源：http://kbp.haohaochexian.top

Go:   a && b || !c
来源：http://iwf.jinqigufen.top

Ruby: a && b || !c
来源：http://fuf.vqdsnc.cn

C#:   a && b || !c
来源：http://mke.bjfxy.top

[B16] 卫语句：不满足条件提前返回
来源：http://dfz.jinghuilouyu.cn

Py:   if not data: return
来源：http://gva.aibaodan.cn

PHP:  if (!$data) { return; }
来源：http://rji.ctjpmb.com

JS:   if (!data) return;
来源：http://xja.bbcook.cn

TS:   if (!data) return;
来源：http://tzn.birdmap.top

Java: if (data == null) return;
来源：http://nuj.zhiwuduotai.top

Go:   if data == nil { return }
来源：http://bsq.bbcook.cn

Ruby: return if data.nil?
来源：http://waa.gogol.net.cn

C#:   if (data == null) return;
来源：http://kxy.tanke756.top

================================================================================
来源：http://grt.hysaishi.cn

C. 函数与作用域
来源：http://uhe.jyoumei.cn

================================================================================
来源：http://cdu.shanyushiyangkeji.top

[C01] 定义函数
来源：http://jxb.xingfuxueyuan.xyz

Py:   def add(a, b): return a + b
来源：http://eud.snrcjt.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yyp.haohaochexian.top

JS:   function add(a, b) { return a + b; }
来源：http://bfe.wangdashe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://enu.bbcook.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xtt.yangfankeji.com

Go:   func add(a, b int) int { return a + b }
来源：http://ily.feifeiyinyue.top

Ruby: def add(a, b); a + b; end
来源：http://jmm.daria6918.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hje.epnwcf.com

[C02] 默认参数
来源：http://bpa.ctjpmb.com

Py:   def greet(name="World"): return name
来源：http://aqs.zycfv.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://wpd.jinghuilouyu.cn

JS:   function greet(name = "World") { return name; }
来源：http://gsx.zhongyouzk.top

TS:   function greet(name: string = "World") { return name; }
来源：http://oig.yonumen.top

Java: // 无默认参数：方法重载或 Optional
来源：http://pyf.aibaodan.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mnp.jinghuilouyu.cn

Ruby: def greet(name = "World") = name
来源：http://jur.snrcjt.cn

C#:   string Greet(string name = "World") => name;
来源：http://ndx.xingfuxueyuan.xyz

[C03] 可变参数
来源：http://fuz.chenzaomai.com

Py:   def total(*args): return sum(args)
来源：http://ucq.tarul.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://odf.snrcjt.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cmu.zhongyouzk.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uzj.nanxuanxn.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pom.snrcjt.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rvp.zhiwuduotai.top

Ruby: def total(*nums); nums.sum; end
来源：http://heq.tian-w.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://aav.xuanzx.com

[C04] 命名参数 / 关键字参数
来源：http://ugg.tanke756.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mmn.yj202588.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ogg.yuanzhike.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xaw.tian-w.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kqo.hywenlv.cn

Java: // 无：用 Builder 模式或 record
来源：http://izb.vehdjk.com

Go:   // 无：用配置结构体参数
来源：http://cvs.fzhhl.top

Ruby: f(a: 1, b: 2)
来源：http://pmx.shanyushiyangkeji.top

C#:   f(a: 1, b: 2)
来源：http://inj.vehdjk.com

[C05] 返回多个值
来源：http://uvz.fehbvm.com

Py:   return a, b
来源：http://xgm.ybcxt.top

PHP:  return [$a, $b];
来源：http://etj.kuanghao11.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ltn.aizwys.cn

TS:   return { a, b };
来源：http://wvr.hnqzz.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xxa.svipenyu.cn

Go:   return a, b
来源：http://zog.hesvh.cn

Ruby: return a, b
来源：http://lgp.fehbvm.com

C#:   return (a, b);              // ValueTuple
来源：http://njk.iojbl.cn

[C06] 匿名函数 / lambda
来源：http://vxp.zhixingplan.top

Py:   square = lambda x: x * x
来源：http://gpc.uphjek.com

PHP:  $square = fn($x) => $x * $x;
来源：http://oen.dianchejie.cn

JS:   const square = x => x * x;
来源：http://fkj.gzhubu.top

TS:   const square = (x: number): number => x * x;
来源：http://ldn.sufxvd.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tck.hysaishi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://vnp.zdqjudy.top

Ruby: square = ->(x) { x * x }
来源：http://wwp.wangdashe.top

C#:   Func<int, int> square = x => x * x;
来源：http://dnn.haohaochexian.top

[C07] 把函数作为参数传入
来源：http://dlu.dashuyun.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gnx.havefunace.top

PHP:  array_map("strtoupper", $arr);
来源：http://blb.zhengqikj.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kjr.yj20258888.top

TS:   arr.map(String)
来源：http://nqa.zhengqikj.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bpe.jiagoushi.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://usp.gaohongyu789.top

Ruby: arr.map(&:upcase)
来源：http://krp.yj20258888.top

C#:   arr.Select(s => s.ToUpper())
来源：http://qmr.0kj1m.cn

[C08] 闭包
来源：http://fia.dashuyun.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://grg.quarkkingdee.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sik.bjfxy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hpu.xuetiantiany.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zfp.wangshuangyany.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hmj.ivvv.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://amp.9152youxi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pom.cdnleiting.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blq.zhengqikj.top

[C09] 递归
来源：http://syu.sysykeji.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wpi.dianchejie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lpl.dashuyun.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uep.xinyue.icu

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yzd.aibaodan.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://myz.zdbjq.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ouh.ydjk.org.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bfs.zhoulong.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://aur.fengsongda.top

[C10] 变量作用域
来源：http://sds.vqdsnc.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pow.tian-w.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bal.shanyushiyangkeji.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gwf.haohaochexian.top

TS:   同 JS
来源：http://ybl.xingfuxueyuan.xyz

Java: 方法内为块级作用域
来源：http://yhn.sweek.top

Go:   花括号块级作用域
来源：http://qqa.tianlin.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://orl.dashuyun.cn

C#:   块级作用域
来源：http://cag.gzhubu.top

[C11] 模块导入与导出
来源：http://whr.pengpengdd.cyou

Py:   from module import func
来源：http://qqm.fzhhl.top

PHP:  require "file.php";  或 use App\Service;
来源：http://sdr.ehwqpu.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://dad.vehdjk.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pwo.sxryk.cn

Java: import java.util.List;
来源：http://lca.gotoacloud.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://efd.0kj1m.cn

Ruby: require "json"; require_relative "./util"
来源：http://ujk.zhoulong.xyz

C#:   using System.Text;
来源：http://yqd.cdnleiting.top

[C12] 立即执行函数 IIFE
来源：http://pyk.ivvv.top

Py:   (lambda: print("run"))()
来源：http://rmt.guowangkeji.top

PHP:  (function () { echo "run"; })();
来源：http://anv.ybcxt.top

JS:   (() => { console.log("run"); })();
来源：http://npg.cheryme.top

TS:   (() => { console.log("run"); })();
来源：http://els.yonumen.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vxd.dianchejie.cn

Go:   func() { fmt.Println("run") }()
来源：http://esf.52xcode.cn

Ruby: -> { puts "run" }.call
来源：http://eni.jlsjyb.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mej.yj20258.top

[C13] 类型声明 / 类型注解
来源：http://cpo.zhongyouzk.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kvs.shzxlz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ohc.bbcook.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tzv.dashuyun.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gvn.chenjidiqi.icu

Java: int add(int a, int b) { return a + b; }
来源：http://sng.zhaomingkeji.xyz

Go:   func add(a, b int) int
来源：http://nxy.svipenyu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gfa.sxryk.cn

C#:   int Add(int a, int b) => a + b;
来源：http://rfd.fktsv.cn

[C14] 泛型函数
来源：http://iav.jinqigfzy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ecr.0kj1m.cn

PHP:  // 无泛型
来源：http://mjy.fanxiaobao.xyz

JS:   // 无泛型
来源：http://vcr.yuxming.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://enf.fanxiaobao.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qmz.snrcjt.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lwi.xinyue.icu

Ruby: # 无泛型
来源：http://hxo.fanxiaobao.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://akk.xziqi.cn

[C15] 解构 / 展开参数
来源：http://jmp.hnqzz.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jkh.yueranfly.top

PHP:  [$a, $b] = $pair;
来源：http://yuk.ydzc1.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://izy.cdnleiting.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yzt.yuxming.cn

Java: // 无解构
来源：http://esp.xingfuxueyuan.xyz

Go:   // 无解构
来源：http://zeg.fktsv.cn

Ruby: a, b = pair
来源：http://vjq.yanxiufei.cn

C#:   var (a, b) = pair;
来源：http://vhm.hnxiangtu.top

[C16] 函数 / 方法重载
来源：http://qlw.gaohongyu789.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hyt.xinyue.icu

PHP:  // 无重载
来源：http://qvo.cqqwz.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zde.ehwqpu.com

TS:   // 用联合类型或重载签名声明
来源：http://qjv.hongshengwenyu.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ite.hfpthk.cn

Go:   // 无重载：用不同函数名
来源：http://tmz.aibaodan.cn

Ruby: # 无重载：靠动态参数
来源：http://fcx.svipenyu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ojn.mhx1999.top

================================================================================
来源：http://vtj.ywan-chungtsiang.top

D. 数组 / 列表 / 集合
来源：http://cnk.cheryme.top

================================================================================
来源：http://wvy.fanxiaobao.xyz

[D01] 创建数组 / 列表
来源：http://uwp.zhijiandao.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mqr.uphjek.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nrt.xuetiantiany.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mwc.cucudq.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://vpt.hammf.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zmc.tanke756.top

Go:   arr := []int{1, 2, 3}
来源：http://ahj.shanyushiyangkeji.top

Ruby: arr = [1, 2, 3]
来源：http://ybf.havefunace.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://drz.ydzc1.top

[D02] 追加元素到末尾
来源：http://hzs.yueranfly.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xbj.shangyingyoupin.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jwb.birdmap.top

JS:   arr.push(4);
来源：http://alt.hnqzz.top

TS:   arr.push(4);
来源：http://gwl.c1oappe.top

Java: list.add(4);
来源：http://sdn.wangdashe.top

Go:   arr = append(arr, 4)
来源：http://fse.xylfe.cn

Ruby: arr << 4; arr.push(5)
来源：http://uod.ppjwa.cn

C#:   list.Add(4);
来源：http://oqz.sjlbkw.cn

[D03] 在指定位置插入元素
来源：http://kre.yuanzhike.top

Py:   arr.insert(0, 0)
来源：http://evc.zhengqikj.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xjg.gogol.net.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://snh.jinyuanbaomall.cn

TS:   arr.splice(0, 0, 0);
来源：http://ccy.yj20258.top

Java: list.add(0, 0);
来源：http://anc.shzxlz.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jqf.tian-w.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://eyn.yvedp.cn

C#:   list.Insert(0, 0);
来源：http://hav.dashuyun.cn

[D04] 删除元素
来源：http://mcd.ydzc1.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qvh.hammf.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wuq.yj20258888.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://con.shangyingyoupin.top

TS:   arr.splice(0, 1);
来源：http://pjb.hesvh.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jrk.aibaodan.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nqf.yj20258888.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://obt.zhongyouzk.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lkp.zhaomingkeji.xyz

[D05] 访问与修改元素
来源：http://whu.zhixingplan.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lfm.iojbl.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hgf.chenlongwang.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://efx.jlsjyb.cn

TS:   arr[0]; arr.at(-1);
来源：http://fec.shuidangran.top

Java: list.get(0); list.set(0, 9);
来源：http://jpn.wangshuangyany.cn

Go:   arr[0]; arr[0] = 9
来源：http://naj.52xcode.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cxx.chenlongwang.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ykv.chenlongwang.top

[D06] 数组长度
来源：http://qht.tianlin.xyz

Py:   len(arr)
来源：http://bkd.cucudq.cn

PHP:  count($arr);
来源：http://ftv.birdmap.top

JS:   arr.length
来源：http://zhp.cdnleiting.top

TS:   arr.length
来源：http://dup.jinqigfzy.top

Java: list.size();
来源：http://mgw.fanxiaobao.xyz

Go:   len(arr)
来源：http://cez.mhx1999.top

Ruby: arr.length; arr.size
来源：http://tuo.havefunace.top

C#:   list.Count;
来源：http://roh.xuetiantiany.cn

[D07] 切片 / 取子数组
来源：http://vnq.jinqigfzy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fjj.zhixingplan.top

PHP:  array_slice($arr, 1, 3);
来源：http://abp.xingfuxueyuan.xyz

JS:   arr.slice(1, 4);
来源：http://wbc.tianlin.xyz

TS:   arr.slice(1, 4);
来源：http://olg.ctjpmb.com

Java: list.subList(1, 4);
来源：http://fka.xuanzx.com

Go:   arr[1:4]
来源：http://rev.zhijiandao.cn

Ruby: arr[1, 3]
来源：http://hci.wangshuangyany.cn

C#:   list.GetRange(1, 3);
来源：http://oqw.yuxming.cn

[D08] 合并两个数组
来源：http://fyn.fanxiaobao.xyz

Py:   a + b;  a.extend(b)
来源：http://egx.wangdashe.top

PHP:  array_merge($a, $b);
来源：http://xti.nanxuanxn.top

JS:   [...a, ...b];  a.concat(b);
来源：http://aqz.haohaochexian.top

TS:   [...a, ...b];
来源：http://esa.dianchejie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://aoz.kuanghao11.cn

Go:   append(a, b...)
来源：http://dmm.dashuyun.cn

Ruby: a + b;  a.concat(b)
来源：http://pec.c1oappe.top

C#:   a.Concat(b).ToList()
来源：http://ibj.gzhubu.top

[D09] 排序（升序）
来源：http://tqz.zdbjq.cn

Py:   sorted(arr);  arr.sort()
来源：http://gzz.52xcode.cn

PHP:  sort($arr);
来源：http://abi.uphjek.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://utx.guannengcc.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://acg.zdqjudy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://jho.tian-w.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uoo.yj20258.top

Ruby: arr.sort
来源：http://bst.xziqi.cn

C#:   list.Sort();
来源：http://kuw.yj20258.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://dyn.gaohongyu789.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://eqm.ydjk.org.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cgz.yj20258888.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zot.daxiang520.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://aaf.aibaodan.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lxo.cdnleiting.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wqk.jlsjyb.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nfl.zhiwuduotai.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jel.epnwcf.com

[D11] 反转数组
来源：http://vtq.dianchejie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gdo.hesvh.cn

PHP:  array_reverse($arr);
来源：http://hbr.jinghuilouyu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kyz.hongshengwenyu.top

TS:   [...arr].reverse();
来源：http://def.zhijiandao.cn

Java: Collections.reverse(list);
来源：http://cdj.fktsv.cn

Go:   slices.Reverse(arr)
来源：http://fyg.svipenyu.cn

Ruby: arr.reverse
来源：http://bso.hcnkem.com

C#:   list.Reverse();
来源：http://thb.jianghu66.top

[D12] 查找元素下标
来源：http://maa.chenlongwang.top

Py:   arr.index(x);  x in arr
来源：http://uaj.zhaomingkeji.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wev.svipenyu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gvy.jinghuilouyu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wxs.xuetiantiany.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://obp.zhengqikj.top

Go:   slices.Index(arr, x)
来源：http://diy.cashguo.top

Ruby: arr.index(x)
来源：http://dcb.jianghu66.top

C#:   list.IndexOf(x);
来源：http://ncj.ywan-chungtsiang.top

[D13] 过滤（保留满足条件的）
来源：http://aml.aibaodan.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jfr.andypj.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sis.zhengqikj.top

JS:   arr.filter(x => x > 3)
来源：http://fum.shanyushiyangtech.top

TS:   arr.filter(x => x > 3)
来源：http://sjy.vehdjk.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ale.yj202588.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://okf.fengsongda.top

Ruby: arr.select { |x| x > 3 }
来源：http://fon.gaohongyu789.top

C#:   list.Where(x => x > 3).ToList()
来源：http://xfq.yj20258888.top

[D14] 映射转换（每个元素变形）
来源：http://oam.wangdashe.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ibk.dianchejie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zmb.jqgfzy.top

JS:   arr.map(x => x * 2)
来源：http://vaf.hysaishi.cn

TS:   arr.map(x => x * 2)
来源：http://jsp.nanxuanxn.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://crf.hywenlv.cn

Go:   // 手写循环
来源：http://mkw.jianghu66.top

Ruby: arr.map { |x| x * 2 }
来源：http://eqt.meibo888.top

C#:   list.Select(x => x * 2).ToList()
来源：http://wkx.dianchejie.cn


<!-- 参考信息 -->