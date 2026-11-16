代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wsb.quarkkingdee.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ecy.kuanghao11.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ilt.fktsv.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vnc.pycfn.com

[B13] 判断是否为数字
来源：http://jbv.ywan-chungtsiang.top

Py:   isinstance(x, (int, float))
来源：http://krr.xuetiantiany.cn

PHP:  is_numeric($x)
来源：http://vzn.iojbl.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ohe.cqqwz.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pvt.pycfn.com

Java: x instanceof Number
来源：http://rqb.hysaishi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qku.ybcxt.top

Ruby: x.is_a?(Numeric)
来源：http://zfx.jinghuilouyu.cn

C#:   x is int or double or decimal
来源：http://qwg.birdmap.top

[B14] 判断值是否在集合内
来源：http://kak.yongpay.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vxj.52xcode.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://eha.zdbjq.cn

JS:   [1, 2, 3].includes(x)
来源：http://kxz.hongshengwenyu.top

TS:   [1, 2, 3].includes(x)
来源：http://lup.jqgufenzy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://dbf.nwbrower.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jtd.fktsv.cn

Ruby: [1, 2, 3].include?(x)
来源：http://eyx.gogol.net.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hty.quarkkingdee.top

[B15] 布尔运算与取反
来源：http://axg.feifeiyinyue.top

Py:   a and b or not c
来源：http://stl.feifeiyinyue.top

PHP:  $a && $b || !$c
来源：http://ykw.52xcode.cn

JS:   a && b || !c
来源：http://wzf.nanxinkj.top

TS:   a && b || !c
来源：http://vqr.jinqigufen.top

Java: a && b || !c
来源：http://gha.cqqwz.cn

Go:   a && b || !c
来源：http://ngz.ybcxt.top

Ruby: a && b || !c
来源：http://ewx.xziqi.cn

C#:   a && b || !c
来源：http://wso.meibo888.top

[B16] 卫语句：不满足条件提前返回
来源：http://fol.guannengcc.top

Py:   if not data: return
来源：http://lrm.zhixingplan.top

PHP:  if (!$data) { return; }
来源：http://win.shanyushiyangtech.top

JS:   if (!data) return;
来源：http://omw.xylfe.cn

TS:   if (!data) return;
来源：http://kgh.vehdjk.com

Java: if (data == null) return;
来源：http://bmt.ydzc1.top

Go:   if data == nil { return }
来源：http://utv.xinyue.icu

Ruby: return if data.nil?
来源：http://mfs.cdnleiting.top

C#:   if (data == null) return;
来源：http://ney.gogol.net.cn

================================================================================
来源：http://kpq.meibo888.top

C. 函数与作用域
来源：http://wtk.tianlin.xyz

================================================================================
来源：http://jxe.xuanzx.com

[C01] 定义函数
来源：http://bkw.yj20258.top

Py:   def add(a, b): return a + b
来源：http://ldr.zhoulong.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ble.fzhhl.top

JS:   function add(a, b) { return a + b; }
来源：http://dwk.daxiang520.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uie.sjlbkw.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lmk.feifeiyinyue.top

Go:   func add(a, b int) int { return a + b }
来源：http://oay.hongshengwenyu.top

Ruby: def add(a, b); a + b; end
来源：http://ftu.zhoulong.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://psf.daxiang520.top

[C02] 默认参数
来源：http://rrj.daria6918.cn

Py:   def greet(name="World"): return name
来源：http://tny.chenjidiqi.icu

PHP:  function greet($name = "World") { return $name; }
来源：http://bbe.sweek.top

JS:   function greet(name = "World") { return name; }
来源：http://iyn.vqdsnc.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://eqg.fehbvm.com

Java: // 无默认参数：方法重载或 Optional
来源：http://ckt.chenjidiqi.icu

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pmx.yvedp.cn

Ruby: def greet(name = "World") = name
来源：http://rip.bjfxy.top

C#:   string Greet(string name = "World") => name;
来源：http://ymb.yueranfly.top

[C03] 可变参数
来源：http://top.hammf.cn

Py:   def total(*args): return sum(args)
来源：http://llb.xingfuxueyuan.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gxb.hywenlv.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jyt.shanyushiyangkeji.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://npj.jiagoushi.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dny.jinyuanbaomall.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://apv.yj202588.top

Ruby: def total(*nums); nums.sum; end
来源：http://fdu.zhixingplan.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jbn.nwbrower.top

[C04] 命名参数 / 关键字参数
来源：http://ffr.yj20258.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ztl.daria6918.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xao.cdnleiting.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xwy.yangfankeji.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hlb.jinqigfzy.top

Java: // 无：用 Builder 模式或 record
来源：http://wot.xuetiantiany.cn

Go:   // 无：用配置结构体参数
来源：http://ydf.chenzaomai.com

Ruby: f(a: 1, b: 2)
来源：http://vje.xingfuxueyuan.xyz

C#:   f(a: 1, b: 2)
来源：http://ulk.ctjpmb.com

[C05] 返回多个值
来源：http://hdb.jiagoushi.top

Py:   return a, b
来源：http://rja.yj20258.top

PHP:  return [$a, $b];
来源：http://oiy.zhoulong.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://rmy.gaohongyu789.top

TS:   return { a, b };
来源：http://itc.sxryk.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xtg.zhijiandao.cn

Go:   return a, b
来源：http://fcm.guannengcc.top

Ruby: return a, b
来源：http://tbb.mhx1999.top

C#:   return (a, b);              // ValueTuple
来源：http://lqm.yvedp.cn

[C06] 匿名函数 / lambda
来源：http://mhi.jiagoushi.top

Py:   square = lambda x: x * x
来源：http://mgi.hcnkem.com

PHP:  $square = fn($x) => $x * $x;
来源：http://kna.yangfankeji.com

JS:   const square = x => x * x;
来源：http://goo.xuanzx.com

TS:   const square = (x: number): number => x * x;
来源：http://aqd.aizwys.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://woc.dianchejie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fow.shzxlz.cn

Ruby: square = ->(x) { x * x }
来源：http://mmn.zhoulong.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://jpk.shuidangran.top

[C07] 把函数作为参数传入
来源：http://rcp.feifeiyinyue.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qkl.chenlongwang.top

PHP:  array_map("strtoupper", $arr);
来源：http://mio.shanyushiyangkeji.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://apm.feifeiyinyue.top

TS:   arr.map(String)
来源：http://lyv.ppjwa.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kfi.nanxuanxn.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ltd.zhengqikj.top

Ruby: arr.map(&:upcase)
来源：http://hjd.haohaochexian.top

C#:   arr.Select(s => s.ToUpper())
来源：http://muk.9152youxi.cn

[C08] 闭包
来源：http://shg.vqdsnc.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qds.xuanzx.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ohx.yuxming.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ewt.fzhhl.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hiy.gaohongyu789.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rqy.cucudq.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tjk.ybcxt.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xdw.hfpthk.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vee.jinyuanbaomall.cn

[C09] 递归
来源：http://wsp.zhengqikj.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ivc.0kj1m.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kmj.andypj.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bby.sweek.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ego.snrcjt.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pku.svipenyu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wjj.yongpay.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tur.ywan-chungtsiang.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mdt.zhoulong.xyz

[C10] 变量作用域
来源：http://lwy.jiagoushi.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jat.cqqwz.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pcq.ydjk.org.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://iqf.jianghu66.top

TS:   同 JS
来源：http://fme.svipenyu.cn

Java: 方法内为块级作用域
来源：http://znz.zdqjudy.top

Go:   花括号块级作用域
来源：http://scd.jinqigufen.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wpz.yuanzhike.top

C#:   块级作用域
来源：http://asm.chenzaomai.com

[C11] 模块导入与导出
来源：http://vud.shangyingyoupin.top

Py:   from module import func
来源：http://hxi.sweek.top

PHP:  require "file.php";  或 use App\Service;
来源：http://uco.ydzc1.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://bhs.smart0.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://izc.yonumen.top

Java: import java.util.List;
来源：http://yts.havefunace.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://izw.chenlongwang.top

Ruby: require "json"; require_relative "./util"
来源：http://ase.aibaodan.cn

C#:   using System.Text;
来源：http://mvu.daxiang520.top

[C12] 立即执行函数 IIFE
来源：http://nwn.gaohongyu789.top

Py:   (lambda: print("run"))()
来源：http://jdk.jqgufenzy.top

PHP:  (function () { echo "run"; })();
来源：http://gdy.fehbvm.com

JS:   (() => { console.log("run"); })();
来源：http://epo.yvedp.cn

TS:   (() => { console.log("run"); })();
来源：http://ufe.pycfn.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bih.hnqzz.top

Go:   func() { fmt.Println("run") }()
来源：http://ukn.mhx1999.top

Ruby: -> { puts "run" }.call
来源：http://vme.iojbl.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://abu.hywenlv.cn

[C13] 类型声明 / 类型注解
来源：http://wce.wangshuangyany.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://max.fktsv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mnh.fehbvm.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://uix.hnxiangtu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zre.guannengcc.top

Java: int add(int a, int b) { return a + b; }
来源：http://tmt.zycfv.cn

Go:   func add(a, b int) int
来源：http://pfh.xylfe.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nkj.chenlongwang.top

C#:   int Add(int a, int b) => a + b;
来源：http://gxt.c1oappe.top

[C14] 泛型函数
来源：http://uys.cucudq.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://oli.hesvh.cn

PHP:  // 无泛型
来源：http://pni.ywan-chungtsiang.top

JS:   // 无泛型
来源：http://qqx.yuanzhike.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://eis.hysaishi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yfh.gotoacloud.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kgx.chenzaomai.com

Ruby: # 无泛型
来源：http://qzq.sufxvd.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jxw.shanyushiyangkeji.top

[C15] 解构 / 展开参数
来源：http://jgs.xingfuxueyuan.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://scq.cheryme.top

PHP:  [$a, $b] = $pair;
来源：http://qwi.xingfuxueyuan.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mrx.hongshengwenyu.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sgc.zhoulong.xyz

Java: // 无解构
来源：http://evj.jqgufenzy.top

Go:   // 无解构
来源：http://mcj.uphjek.com

Ruby: a, b = pair
来源：http://qgc.jqgufenzy.top

C#:   var (a, b) = pair;
来源：http://dzk.zhaomingkeji.xyz

[C16] 函数 / 方法重载
来源：http://dmx.zhengqikj.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://abr.ydzc1.top

PHP:  // 无重载
来源：http://dph.sjlbkw.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://lpp.xziqi.cn

TS:   // 用联合类型或重载签名声明
来源：http://arh.yfazqb.com

Java: void f(int a) {}  void f(String a) {}
来源：http://lqx.hcnkem.com

Go:   // 无重载：用不同函数名
来源：http://rfd.bbcook.cn

Ruby: # 无重载：靠动态参数
来源：http://rqz.andypj.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://dno.fktsv.cn

================================================================================
来源：http://eaa.epnwcf.com

D. 数组 / 列表 / 集合
来源：http://pxe.jinyuanbaomall.cn

================================================================================
来源：http://syx.hongshengwenyu.top

[D01] 创建数组 / 列表
来源：http://ywi.bjfxy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://hei.aizwys.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xvn.jinqigufen.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xbx.havefunace.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://svd.bbcook.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://eby.xylfe.cn

Go:   arr := []int{1, 2, 3}
来源：http://oux.wangshuangyany.cn

Ruby: arr = [1, 2, 3]
来源：http://jgc.zhengqikj.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ngl.snrcjt.cn

[D02] 追加元素到末尾
来源：http://jkv.gotoacloud.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qmu.zycfv.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vkg.zhoulong.xyz

JS:   arr.push(4);
来源：http://wwq.hcnkem.com

TS:   arr.push(4);
来源：http://fqv.jqgufenzy.top

Java: list.add(4);
来源：http://ntj.hesvh.cn

Go:   arr = append(arr, 4)
来源：http://jok.c1oappe.top

Ruby: arr << 4; arr.push(5)
来源：http://zkc.yfazqb.com

C#:   list.Add(4);
来源：http://jbu.hnxiangtu.top

[D03] 在指定位置插入元素
来源：http://pze.cqqwz.cn

Py:   arr.insert(0, 0)
来源：http://jla.aibaodan.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qzj.sysykeji.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://quz.uphjek.com

TS:   arr.splice(0, 0, 0);
来源：http://ejs.nanxuanxn.top

Java: list.add(0, 0);
来源：http://aft.hnqzz.top

Go:   arr = append([]int{0}, arr...)
来源：http://mzr.aibaodan.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fme.zdqjudy.top

C#:   list.Insert(0, 0);
来源：http://vfa.fzhhl.top

[D04] 删除元素
来源：http://xtk.redwolf501.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nuw.yfazqb.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ffy.52xcode.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cud.yuxming.cn

TS:   arr.splice(0, 1);
来源：http://hjx.fehbvm.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://avi.yfazqb.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qda.xuetiantiany.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pom.tanke756.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dgw.0kj1m.cn

[D05] 访问与修改元素
来源：http://szv.ctjpmb.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xxj.epnwcf.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rbs.zhijiandao.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bok.ybcxt.top

TS:   arr[0]; arr.at(-1);
来源：http://vha.ppjwa.cn

Java: list.get(0); list.set(0, 9);
来源：http://mum.jyoumei.cn

Go:   arr[0]; arr[0] = 9
来源：http://utc.cdnleiting.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://aqr.wangdashe.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qem.zhijiandao.cn

[D06] 数组长度
来源：http://ewj.yfazqb.com

Py:   len(arr)
来源：http://jhj.chenzaomai.com

PHP:  count($arr);
来源：http://xsh.jinghuilouyu.cn

JS:   arr.length
来源：http://swn.ybcxt.top

TS:   arr.length
来源：http://ido.aizwys.cn

Java: list.size();
来源：http://slq.jlsjyb.cn

Go:   len(arr)
来源：http://grv.pycfn.com

Ruby: arr.length; arr.size
来源：http://oyr.gzhubu.top

C#:   list.Count;
来源：http://xzn.guannengcc.top

[D07] 切片 / 取子数组
来源：http://ahr.redwolf501.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://eex.9152youxi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://rxh.hywenlv.cn

JS:   arr.slice(1, 4);
来源：http://rzc.bbcook.cn

TS:   arr.slice(1, 4);
来源：http://fuc.zhoulong.xyz

Java: list.subList(1, 4);
来源：http://wyd.fanxiaobao.xyz

Go:   arr[1:4]
来源：http://ein.cqqwz.cn

Ruby: arr[1, 3]
来源：http://lmz.jqgfzy.top

C#:   list.GetRange(1, 3);
来源：http://oyg.jyoumei.cn

[D08] 合并两个数组
来源：http://czc.cashguo.top

Py:   a + b;  a.extend(b)
来源：http://jum.52xcode.cn

PHP:  array_merge($a, $b);
来源：http://aod.zdbjq.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://opd.fktsv.cn

TS:   [...a, ...b];
来源：http://vga.gzhubu.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ywy.redwolf501.top

Go:   append(a, b...)
来源：http://gmc.jqgfzy.top

Ruby: a + b;  a.concat(b)
来源：http://zlr.tianlin.xyz

C#:   a.Concat(b).ToList()
来源：http://saw.hysaishi.cn

[D09] 排序（升序）
来源：http://khr.jinqigfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://mpk.chenjidiqi.icu

PHP:  sort($arr);
来源：http://yqe.jinqigufen.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gdc.havefunace.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ozb.gaohongyu789.top

Java: Collections.sort(list);  list.sort(null);
来源：http://dsi.hesvh.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hnz.jlsjyb.cn

Ruby: arr.sort
来源：http://csv.yuanzhike.top

C#:   list.Sort();
来源：http://wwk.zhiwuduotai.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://axt.uphjek.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nlr.andypj.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ltl.wangshuangyany.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ije.tian-w.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rrq.ydzc1.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nls.jinghuilouyu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://omx.fanxiaobao.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://emv.sysykeji.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nps.cucudq.cn

[D11] 反转数组
来源：http://vay.tarul.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gst.fktsv.cn

PHP:  array_reverse($arr);
来源：http://scs.shzxlz.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vwi.chenjidiqi.icu

TS:   [...arr].reverse();
来源：http://syp.gotoacloud.top

Java: Collections.reverse(list);
来源：http://yeb.quarkkingdee.top

Go:   slices.Reverse(arr)
来源：http://kka.aizwys.cn

Ruby: arr.reverse
来源：http://oyh.guowangkeji.top

C#:   list.Reverse();
来源：http://paj.ydjk.org.cn

[D12] 查找元素下标
来源：http://bwf.fktsv.cn

Py:   arr.index(x);  x in arr
来源：http://wvj.hcnkem.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ncv.feifeiyinyue.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nzl.xingfuxueyuan.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pcu.fehbvm.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wfi.sufxvd.cn

Go:   slices.Index(arr, x)
来源：http://dvi.andypj.xyz

Ruby: arr.index(x)
来源：http://yxg.fanxiaobao.xyz

C#:   list.IndexOf(x);
来源：http://mhp.xuetiantiany.cn

[D13] 过滤（保留满足条件的）
来源：http://iap.mhx1999.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lqt.cqqwz.cn


<!-- 参考信息 -->