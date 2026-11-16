代发 wailian999

PHP:  $a && $b || !$c
来源：http://eak.vqdsnc.cn

JS:   a && b || !c
来源：http://bkl.hywenlv.cn

TS:   a && b || !c
来源：http://ksr.zhijiandao.cn

Java: a && b || !c
来源：http://izc.gaohongyu789.top

Go:   a && b || !c
来源：http://bhk.redwolf501.top

Ruby: a && b || !c
来源：http://pal.yangfankeji.com

C#:   a && b || !c
来源：http://gei.pycfn.com

[B16] 卫语句：不满足条件提前返回
来源：http://fsv.pycfn.com

Py:   if not data: return
来源：http://chx.fehbvm.com

PHP:  if (!$data) { return; }
来源：http://adx.aizwys.cn

JS:   if (!data) return;
来源：http://ebd.ivvv.top

TS:   if (!data) return;
来源：http://aln.nanxuanxn.top

Java: if (data == null) return;
来源：http://mrv.fengsongda.top

Go:   if data == nil { return }
来源：http://ort.chenlongwang.top

Ruby: return if data.nil?
来源：http://pcl.zhengqikj.top

C#:   if (data == null) return;
来源：http://tzy.jinqigfzy.top

================================================================================
来源：http://kpc.tianlin.xyz

C. 函数与作用域
来源：http://jxo.chenzaomai.com

================================================================================
来源：http://xqm.yfazqb.com

[C01] 定义函数
来源：http://kam.ctjpmb.com

Py:   def add(a, b): return a + b
来源：http://mky.tanke756.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://udm.gzhubu.top

JS:   function add(a, b) { return a + b; }
来源：http://vsd.ydzc1.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vif.ehwqpu.com

Java: static int add(int a, int b) { return a + b; }
来源：http://pbu.aizwys.cn

Go:   func add(a, b int) int { return a + b }
来源：http://oio.jinqigfzy.top

Ruby: def add(a, b); a + b; end
来源：http://bus.redwolf501.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ldi.aibaodan.cn

[C02] 默认参数
来源：http://oqg.ehwqpu.com

Py:   def greet(name="World"): return name
来源：http://flk.yuxming.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://avy.jinghuilouyu.cn

JS:   function greet(name = "World") { return name; }
来源：http://mbf.redwolf501.top

TS:   function greet(name: string = "World") { return name; }
来源：http://tau.haohaochexian.top

Java: // 无默认参数：方法重载或 Optional
来源：http://fgd.yvedp.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jqc.shanyushiyangtech.top

Ruby: def greet(name = "World") = name
来源：http://clb.ydjk.org.cn

C#:   string Greet(string name = "World") => name;
来源：http://tdl.hnxiangtu.top

[C03] 可变参数
来源：http://mqp.andypj.xyz

Py:   def total(*args): return sum(args)
来源：http://vlq.hfpthk.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://meh.jinqigfzy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://reo.yongpay.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gtl.yueranfly.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jcr.gotoacloud.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yvj.quarkkingdee.top

Ruby: def total(*nums); nums.sum; end
来源：http://imu.hnxiangtu.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qdy.sjlbkw.cn

[C04] 命名参数 / 关键字参数
来源：http://sph.fehbvm.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pij.chenjidiqi.icu

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bcx.316326.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ijk.bbcook.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mzb.shzxlz.cn

Java: // 无：用 Builder 模式或 record
来源：http://igj.hnqzz.top

Go:   // 无：用配置结构体参数
来源：http://lso.9152youxi.cn

Ruby: f(a: 1, b: 2)
来源：http://nws.zhiwuduotai.top

C#:   f(a: 1, b: 2)
来源：http://gla.meibo888.top

[C05] 返回多个值
来源：http://zma.pycfn.com

Py:   return a, b
来源：http://tcv.hongshengwenyu.top

PHP:  return [$a, $b];
来源：http://lau.zhijiandao.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://twt.jiagoushi.top

TS:   return { a, b };
来源：http://nop.chenlongwang.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ndr.jinyuanbaomall.cn

Go:   return a, b
来源：http://orz.vehdjk.com

Ruby: return a, b
来源：http://uvg.uphjek.com

C#:   return (a, b);              // ValueTuple
来源：http://wti.sweek.top

[C06] 匿名函数 / lambda
来源：http://kav.fktsv.cn

Py:   square = lambda x: x * x
来源：http://zep.sjlbkw.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://hmx.hnqzz.top

JS:   const square = x => x * x;
来源：http://hkp.zhengqikj.top

TS:   const square = (x: number): number => x * x;
来源：http://vqt.hesvh.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kst.xylfe.cn

Go:   sq := func(x int) int { return x * x }
来源：http://xmw.yj20258.top

Ruby: square = ->(x) { x * x }
来源：http://qro.jyoumei.cn

C#:   Func<int, int> square = x => x * x;
来源：http://pja.mhx1999.top

[C07] 把函数作为参数传入
来源：http://xzy.jinyuanbaomall.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xxu.bbcook.cn

PHP:  array_map("strtoupper", $arr);
来源：http://rfw.dashuyun.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cvc.yongpay.top

TS:   arr.map(String)
来源：http://pds.smart0.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mli.quarkkingdee.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ggt.guannengcc.top

Ruby: arr.map(&:upcase)
来源：http://aey.shanyushiyangtech.top

C#:   arr.Select(s => s.ToUpper())
来源：http://svn.vehdjk.com

[C08] 闭包
来源：http://qpy.yangfankeji.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lmg.shzxlz.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vkn.zhixingplan.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://crc.hcnkem.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fiu.gaohongyu789.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jqc.xuanzx.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://oxq.hongshengwenyu.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bwq.guowangkeji.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tkq.shuidangran.top

[C09] 递归
来源：http://fia.hongshengwenyu.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sqa.yj20258.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zmm.xziqi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lld.tarul.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://joe.cucudq.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://buc.meibo888.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nsf.jlsjyb.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ftt.tian-w.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kzh.tanke756.top

[C10] 变量作用域
来源：http://pig.cdnleiting.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kys.yanxiufei.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wxr.bbcook.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xqx.cdnleiting.top

TS:   同 JS
来源：http://lpa.jinyuanbaomall.cn

Java: 方法内为块级作用域
来源：http://oew.zhijiandao.cn

Go:   花括号块级作用域
来源：http://ujv.zycfv.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ukj.snrcjt.cn

C#:   块级作用域
来源：http://sgl.nanxuanxn.top

[C11] 模块导入与导出
来源：http://jjq.shanyushiyangtech.top

Py:   from module import func
来源：http://enn.tarul.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://hfc.hywenlv.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://fvh.meibo888.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uva.fengsongda.top

Java: import java.util.List;
来源：http://hat.snrcjt.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wne.sweek.top

Ruby: require "json"; require_relative "./util"
来源：http://qcx.tanke756.top

C#:   using System.Text;
来源：http://kms.tian-w.cn

[C12] 立即执行函数 IIFE
来源：http://sym.quarkkingdee.top

Py:   (lambda: print("run"))()
来源：http://xeb.fzhhl.top

PHP:  (function () { echo "run"; })();
来源：http://hbm.zycfv.cn

JS:   (() => { console.log("run"); })();
来源：http://qkx.aizwys.cn

TS:   (() => { console.log("run"); })();
来源：http://vqo.wangshuangyany.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rdm.zdbjq.cn

Go:   func() { fmt.Println("run") }()
来源：http://hbw.yuxming.cn

Ruby: -> { puts "run" }.call
来源：http://nqq.vehdjk.com

C#:   // 无 IIFE：用静态构造函数
来源：http://kic.yj202588.top

[C13] 类型声明 / 类型注解
来源：http://zhm.fehbvm.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mgu.cheryme.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://snf.hammf.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://erh.xinyue.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hyj.ywan-chungtsiang.top

Java: int add(int a, int b) { return a + b; }
来源：http://jzr.cheryme.top

Go:   func add(a, b int) int
来源：http://cnv.yfazqb.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ayc.sufxvd.cn

C#:   int Add(int a, int b) => a + b;
来源：http://htn.c1oappe.top

[C14] 泛型函数
来源：http://ybe.ehwqpu.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wre.fanxiaobao.xyz

PHP:  // 无泛型
来源：http://kve.meibo888.top

JS:   // 无泛型
来源：http://lxd.mhx1999.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://coz.jiagoushi.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://for.zhixingplan.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gkv.epnwcf.com

Ruby: # 无泛型
来源：http://gyf.ybcxt.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ndc.redwolf501.top

[C15] 解构 / 展开参数
来源：http://pbs.gogol.net.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://efm.hammf.cn

PHP:  [$a, $b] = $pair;
来源：http://ycj.gotoacloud.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ujm.svipenyu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://arz.yueranfly.top

Java: // 无解构
来源：http://slt.hnxiangtu.top

Go:   // 无解构
来源：http://txz.zdbjq.cn

Ruby: a, b = pair
来源：http://zwl.smart0.xyz

C#:   var (a, b) = pair;
来源：http://vvz.shuidangran.top

[C16] 函数 / 方法重载
来源：http://ojf.xingfuxueyuan.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qsi.c1oappe.top

PHP:  // 无重载
来源：http://huj.havefunace.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://gyk.haohaochexian.top

TS:   // 用联合类型或重载签名声明
来源：http://qxz.epnwcf.com

Java: void f(int a) {}  void f(String a) {}
来源：http://cpa.sysykeji.top

Go:   // 无重载：用不同函数名
来源：http://jur.jqgfzy.top

Ruby: # 无重载：靠动态参数
来源：http://fzt.nanxinkj.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://mht.zhijiandao.cn

================================================================================
来源：http://ivu.ydjk.org.cn

D. 数组 / 列表 / 集合
来源：http://sjg.jianghu66.top

================================================================================
来源：http://bzs.jinyuanbaomall.cn

[D01] 创建数组 / 列表
来源：http://zpv.zhongyouzk.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://bog.daria6918.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fju.birdmap.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pmy.shangyingyoupin.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://pde.havefunace.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://glj.ivvv.top

Go:   arr := []int{1, 2, 3}
来源：http://ibo.hongshengwenyu.top

Ruby: arr = [1, 2, 3]
来源：http://oan.yfazqb.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dmu.uphjek.com

[D02] 追加元素到末尾
来源：http://yme.hongshengwenyu.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zco.yongpay.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://egx.xinyue.icu

JS:   arr.push(4);
来源：http://act.vqdsnc.cn

TS:   arr.push(4);
来源：http://gct.zhiwuduotai.top

Java: list.add(4);
来源：http://fis.xuetiantiany.cn

Go:   arr = append(arr, 4)
来源：http://ufi.bjfxy.top

Ruby: arr << 4; arr.push(5)
来源：http://sgv.xziqi.cn

C#:   list.Add(4);
来源：http://zfh.zhongyouzk.top

[D03] 在指定位置插入元素
来源：http://ykz.wangshuangyany.cn

Py:   arr.insert(0, 0)
来源：http://bto.ehwqpu.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://drv.nwbrower.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://skj.kuanghao11.cn

TS:   arr.splice(0, 0, 0);
来源：http://dit.redwolf501.top

Java: list.add(0, 0);
来源：http://czt.dianchejie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://pei.yanxiufei.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jua.xinyue.icu

C#:   list.Insert(0, 0);
来源：http://zvv.sweek.top

[D04] 删除元素
来源：http://qnn.gotoacloud.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ice.zycfv.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fbt.cucudq.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sda.xylfe.cn

TS:   arr.splice(0, 1);
来源：http://hpw.dashuyun.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://twn.pycfn.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://oik.bjfxy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kjp.sysykeji.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gqy.fengsongda.top

[D05] 访问与修改元素
来源：http://jnl.dashuyun.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kym.snrcjt.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xpx.quarkkingdee.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://law.yj20258888.top

TS:   arr[0]; arr.at(-1);
来源：http://qig.bbcook.cn

Java: list.get(0); list.set(0, 9);
来源：http://ldl.shanyushiyangkeji.top

Go:   arr[0]; arr[0] = 9
来源：http://gik.52xcode.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bui.52xcode.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qqu.birdmap.top

[D06] 数组长度
来源：http://eko.tarul.cn

Py:   len(arr)
来源：http://hra.uphjek.com

PHP:  count($arr);
来源：http://jwr.gogol.net.cn

JS:   arr.length
来源：http://xdt.jyoumei.cn

TS:   arr.length
来源：http://hme.yj20258.top

Java: list.size();
来源：http://grk.vehdjk.com

Go:   len(arr)
来源：http://mjq.zycfv.cn

Ruby: arr.length; arr.size
来源：http://etb.zhongyouzk.top

C#:   list.Count;
来源：http://tmd.zdqjudy.top

[D07] 切片 / 取子数组
来源：http://jpk.nanxuanxn.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://toh.ydzc1.top

PHP:  array_slice($arr, 1, 3);
来源：http://gud.ydjk.org.cn

JS:   arr.slice(1, 4);
来源：http://myn.0kj1m.cn

TS:   arr.slice(1, 4);
来源：http://bgw.jiagoushi.top

Java: list.subList(1, 4);
来源：http://zsw.fzhhl.top

Go:   arr[1:4]
来源：http://tvw.ctjpmb.com

Ruby: arr[1, 3]
来源：http://tln.tian-w.cn

C#:   list.GetRange(1, 3);
来源：http://hej.hesvh.cn

[D08] 合并两个数组
来源：http://icq.tanke756.top

Py:   a + b;  a.extend(b)
来源：http://ozx.epnwcf.com

PHP:  array_merge($a, $b);
来源：http://xzl.jianghu66.top

JS:   [...a, ...b];  a.concat(b);
来源：http://xqd.jyoumei.cn

TS:   [...a, ...b];
来源：http://cht.birdmap.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nxu.yuxming.cn

Go:   append(a, b...)
来源：http://duv.zhixingplan.top

Ruby: a + b;  a.concat(b)
来源：http://agh.cheryme.top

C#:   a.Concat(b).ToList()
来源：http://lzu.zhoulong.xyz

[D09] 排序（升序）
来源：http://tjc.smart0.xyz

Py:   sorted(arr);  arr.sort()
来源：http://mod.zdqjudy.top

PHP:  sort($arr);
来源：http://oqq.52xcode.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hpc.pycfn.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://jpf.ppjwa.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://wjo.hnxiangtu.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://crt.jqgufenzy.top

Ruby: arr.sort
来源：http://pdy.jinqigufen.top

C#:   list.Sort();
来源：http://sfo.zycfv.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ure.tian-w.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jcs.nwbrower.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://siq.uphjek.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qak.yongpay.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kpj.jinqigufen.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ndi.xinyue.icu

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wyz.shangyingyoupin.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gvs.tian-w.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ekg.gotoacloud.top

[D11] 反转数组
来源：http://ove.yonumen.top

Py:   arr[::-1];  arr.reverse()
来源：http://rel.snrcjt.cn

PHP:  array_reverse($arr);
来源：http://mma.xinyue.icu

JS:   [...arr].reverse();  arr.toReversed()
来源：http://liw.chenjidiqi.icu

TS:   [...arr].reverse();
来源：http://kuh.jqgfzy.top

Java: Collections.reverse(list);
来源：http://kug.gaohongyu789.top

Go:   slices.Reverse(arr)
来源：http://ora.ywan-chungtsiang.top

Ruby: arr.reverse
来源：http://wxe.pengpengdd.cyou

C#:   list.Reverse();
来源：http://kmr.cucudq.cn

[D12] 查找元素下标
来源：http://leo.aizwys.cn

Py:   arr.index(x);  x in arr
来源：http://azp.hcnkem.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bzq.xuanzx.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ehq.epnwcf.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vgq.hysaishi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pwe.shangyingyoupin.top

Go:   slices.Index(arr, x)
来源：http://raj.jqgufenzy.top

Ruby: arr.index(x)
来源：http://wsm.wangdashe.top

C#:   list.IndexOf(x);
来源：http://enm.bjfxy.top

[D13] 过滤（保留满足条件的）
来源：http://ted.c1oappe.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ryg.yj20258888.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bbn.uphjek.com

JS:   arr.filter(x => x > 3)
来源：http://moe.gotoacloud.top

TS:   arr.filter(x => x > 3)
来源：http://qfk.gotoacloud.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mon.zhijiandao.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bdg.chenlongwang.top

Ruby: arr.select { |x| x > 3 }
来源：http://yrx.ivvv.top

C#:   list.Where(x => x > 3).ToList()
来源：http://obd.jianghu66.top

[D14] 映射转换（每个元素变形）
来源：http://nqv.zhaomingkeji.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kzb.zhijiandao.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vko.zdbjq.cn

JS:   arr.map(x => x * 2)
来源：http://gkf.xuetiantiany.cn

TS:   arr.map(x => x * 2)
来源：http://osg.xylfe.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://jsk.epnwcf.com

Go:   // 手写循环
来源：http://shv.ppjwa.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vso.gzhubu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://nig.cashguo.top

[D15] 去重
来源：http://zuf.hcnkem.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tgt.zhijiandao.cn

PHP:  array_unique($arr);
来源：http://ebe.redwolf501.top

JS:   [...new Set(arr)]
来源：http://fvs.ppjwa.cn

TS:   [...new Set(arr)]
来源：http://lrm.quarkkingdee.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ptj.feifeiyinyue.top

Go:   // 用 map[T]struct{} 手写
来源：http://sgl.chenzaomai.com

Ruby: arr.uniq
来源：http://ifk.gogol.net.cn


<!-- 参考信息 -->