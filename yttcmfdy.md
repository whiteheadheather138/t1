代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hpn.0kj1m.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://sid.quarkkingdee.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pfb.nanxinkj.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://csr.shzxlz.cn

[B13] 判断是否为数字
来源：http://wya.yj20258888.top

Py:   isinstance(x, (int, float))
来源：http://xjo.chenzaomai.com

PHP:  is_numeric($x)
来源：http://qlp.ywan-chungtsiang.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jdu.vqdsnc.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://arn.birdmap.top

Java: x instanceof Number
来源：http://vkn.mhx1999.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ehm.andypj.xyz

Ruby: x.is_a?(Numeric)
来源：http://icc.gzhubu.top

C#:   x is int or double or decimal
来源：http://ikm.meibo888.top

[B14] 判断值是否在集合内
来源：http://suc.wangdashe.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tni.hcnkem.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gkw.bjfxy.top

JS:   [1, 2, 3].includes(x)
来源：http://dhq.xuanzx.com

TS:   [1, 2, 3].includes(x)
来源：http://ldz.ydzc1.top

Java: List.of(1, 2, 3).contains(x)
来源：http://xjq.yueranfly.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kum.yonumen.top

Ruby: [1, 2, 3].include?(x)
来源：http://jns.wangdashe.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gme.dianchejie.cn

[B15] 布尔运算与取反
来源：http://voi.jyoumei.cn

Py:   a and b or not c
来源：http://tnp.shanyushiyangkeji.top

PHP:  $a && $b || !$c
来源：http://ucv.ydzc1.top

JS:   a && b || !c
来源：http://pvs.9152youxi.cn

TS:   a && b || !c
来源：http://qbi.wangshuangyany.cn

Java: a && b || !c
来源：http://flb.shangyingyoupin.top

Go:   a && b || !c
来源：http://nna.zhijiandao.cn

Ruby: a && b || !c
来源：http://iuw.tianlin.xyz

C#:   a && b || !c
来源：http://oap.zhongyouzk.top

[B16] 卫语句：不满足条件提前返回
来源：http://lez.hammf.cn

Py:   if not data: return
来源：http://hjl.jyoumei.cn

PHP:  if (!$data) { return; }
来源：http://yaf.ydzc1.top

JS:   if (!data) return;
来源：http://vpx.cdnleiting.top

TS:   if (!data) return;
来源：http://kph.zhaomingkeji.xyz

Java: if (data == null) return;
来源：http://tub.meibo888.top

Go:   if data == nil { return }
来源：http://vdl.aizwys.cn

Ruby: return if data.nil?
来源：http://dre.nanxinkj.top

C#:   if (data == null) return;
来源：http://vaq.wangshuangyany.cn

================================================================================
来源：http://daa.shzxlz.cn

C. 函数与作用域
来源：http://efl.yangfankeji.com

================================================================================
来源：http://kpf.xingfuxueyuan.xyz

[C01] 定义函数
来源：http://xwz.pengpengdd.cyou

Py:   def add(a, b): return a + b
来源：http://vya.pycfn.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ivp.ywan-chungtsiang.top

JS:   function add(a, b) { return a + b; }
来源：http://joc.yj20258888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wrl.aibaodan.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://owi.shuidangran.top

Go:   func add(a, b int) int { return a + b }
来源：http://gxg.fanxiaobao.xyz

Ruby: def add(a, b); a + b; end
来源：http://pdw.zhoulong.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://syh.chenzaomai.com

[C02] 默认参数
来源：http://gmb.yj20258888.top

Py:   def greet(name="World"): return name
来源：http://qrn.sysykeji.top

PHP:  function greet($name = "World") { return $name; }
来源：http://jdn.0kj1m.cn

JS:   function greet(name = "World") { return name; }
来源：http://jyk.ydzc1.top

TS:   function greet(name: string = "World") { return name; }
来源：http://fdh.hcnkem.com

Java: // 无默认参数：方法重载或 Optional
来源：http://lni.havefunace.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mne.zycfv.cn

Ruby: def greet(name = "World") = name
来源：http://ihv.bjfxy.top

C#:   string Greet(string name = "World") => name;
来源：http://slr.xuanzx.com

[C03] 可变参数
来源：http://vhn.sjlbkw.cn

Py:   def total(*args): return sum(args)
来源：http://lgq.sysykeji.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://egb.sufxvd.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zin.hysaishi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lyo.zhoulong.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mfg.bbcook.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gpz.ehwqpu.com

Ruby: def total(*nums); nums.sum; end
来源：http://bdo.meibo888.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tbi.guowangkeji.top

[C04] 命名参数 / 关键字参数
来源：http://tex.hywenlv.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wzm.aizwys.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ilc.cdnleiting.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kpu.yueranfly.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wxk.yonumen.top

Java: // 无：用 Builder 模式或 record
来源：http://vcn.zhongyouzk.top

Go:   // 无：用配置结构体参数
来源：http://euy.haohaochexian.top

Ruby: f(a: 1, b: 2)
来源：http://pet.shangyingyoupin.top

C#:   f(a: 1, b: 2)
来源：http://mrp.xuetiantiany.cn

[C05] 返回多个值
来源：http://zmf.birdmap.top

Py:   return a, b
来源：http://krj.yueranfly.top

PHP:  return [$a, $b];
来源：http://pnn.fehbvm.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://hpr.feifeiyinyue.top

TS:   return { a, b };
来源：http://wzw.tian-w.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ejj.yj202588.top

Go:   return a, b
来源：http://tlb.meibo888.top

Ruby: return a, b
来源：http://trw.zdqjudy.top

C#:   return (a, b);              // ValueTuple
来源：http://rml.shangyingyoupin.top

[C06] 匿名函数 / lambda
来源：http://ahg.xuetiantiany.cn

Py:   square = lambda x: x * x
来源：http://qzf.chenlongwang.top

PHP:  $square = fn($x) => $x * $x;
来源：http://adj.fehbvm.com

JS:   const square = x => x * x;
来源：http://hsi.c1oappe.top

TS:   const square = (x: number): number => x * x;
来源：http://eyd.zdqjudy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dlb.guannengcc.top

Go:   sq := func(x int) int { return x * x }
来源：http://zxh.hesvh.cn

Ruby: square = ->(x) { x * x }
来源：http://lit.nanxinkj.top

C#:   Func<int, int> square = x => x * x;
来源：http://wzt.birdmap.top

[C07] 把函数作为参数传入
来源：http://qfu.ctjpmb.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vpk.meibo888.top

PHP:  array_map("strtoupper", $arr);
来源：http://paf.fehbvm.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hyd.wangdashe.top

TS:   arr.map(String)
来源：http://lzg.zhongyouzk.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gbr.ywan-chungtsiang.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gsp.pycfn.com

Ruby: arr.map(&:upcase)
来源：http://luf.jlsjyb.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wlv.zhoulong.xyz

[C08] 闭包
来源：http://owh.sweek.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hqj.snrcjt.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jkc.andypj.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://utp.hfpthk.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://oep.tianlin.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://btw.mhx1999.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fyg.hcnkem.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://oso.yongpay.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ldc.52xcode.cn

[C09] 递归
来源：http://pmu.jiagoushi.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vmw.yangfankeji.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://swo.nwbrower.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://eno.aizwys.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lhj.tarul.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rxk.yonumen.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ynb.dianchejie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://twz.aibaodan.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fzh.snrcjt.cn

[C10] 变量作用域
来源：http://fox.zdqjudy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hjo.jyoumei.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ulq.xuanzx.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://duw.dianchejie.cn

TS:   同 JS
来源：http://ust.fengsongda.top

Java: 方法内为块级作用域
来源：http://tjo.zdbjq.cn

Go:   花括号块级作用域
来源：http://opc.xuanzx.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pky.uphjek.com

C#:   块级作用域
来源：http://ycp.dashuyun.cn

[C11] 模块导入与导出
来源：http://eqg.shzxlz.cn

Py:   from module import func
来源：http://szr.dashuyun.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ylf.haohaochexian.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://csn.zhengqikj.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ank.ydjk.org.cn

Java: import java.util.List;
来源：http://jrd.fehbvm.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bhr.yonumen.top

Ruby: require "json"; require_relative "./util"
来源：http://hxo.fzhhl.top

C#:   using System.Text;
来源：http://ijz.tanke756.top

[C12] 立即执行函数 IIFE
来源：http://cmb.zhixingplan.top

Py:   (lambda: print("run"))()
来源：http://mbi.yongpay.top

PHP:  (function () { echo "run"; })();
来源：http://hkg.zdbjq.cn

JS:   (() => { console.log("run"); })();
来源：http://wug.jyoumei.cn

TS:   (() => { console.log("run"); })();
来源：http://uik.zhengqikj.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://amc.xingfuxueyuan.xyz

Go:   func() { fmt.Println("run") }()
来源：http://guv.zycfv.cn

Ruby: -> { puts "run" }.call
来源：http://lgn.vehdjk.com

C#:   // 无 IIFE：用静态构造函数
来源：http://muh.shuidangran.top

[C13] 类型声明 / 类型注解
来源：http://hml.daxiang520.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bvk.wangdashe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ftk.zycfv.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nap.guowangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rys.hysaishi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mpn.daxiang520.top

Go:   func add(a, b int) int
来源：http://ute.dashuyun.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wup.fanxiaobao.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://nun.c1oappe.top

[C14] 泛型函数
来源：http://bfw.tanke756.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hhm.quarkkingdee.top

PHP:  // 无泛型
来源：http://rbv.tarul.cn

JS:   // 无泛型
来源：http://lvo.snrcjt.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pzn.sxryk.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://aho.zdqjudy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tus.bbcook.cn

Ruby: # 无泛型
来源：http://xgd.sxryk.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xfd.xylfe.cn

[C15] 解构 / 展开参数
来源：http://cco.mhx1999.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://oom.haohaochexian.top

PHP:  [$a, $b] = $pair;
来源：http://zib.jqgufenzy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://odo.haohaochexian.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mcl.zdqjudy.top

Java: // 无解构
来源：http://zos.jinghuilouyu.cn

Go:   // 无解构
来源：http://ypi.jyoumei.cn

Ruby: a, b = pair
来源：http://nah.zdbjq.cn

C#:   var (a, b) = pair;
来源：http://onb.daxiang520.top

[C16] 函数 / 方法重载
来源：http://csb.sysykeji.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nfh.yvedp.cn

PHP:  // 无重载
来源：http://uze.chenjidiqi.icu

JS:   // 无重载：靠 arguments.length 分支
来源：http://mek.hesvh.cn

TS:   // 用联合类型或重载签名声明
来源：http://dhe.0kj1m.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://cww.fengsongda.top

Go:   // 无重载：用不同函数名
来源：http://pbl.jinqigufen.top

Ruby: # 无重载：靠动态参数
来源：http://noa.chenzaomai.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://eqf.jiagoushi.top

================================================================================
来源：http://hph.mhx1999.top

D. 数组 / 列表 / 集合
来源：http://tyg.shuidangran.top

================================================================================
来源：http://pma.bjfxy.top

[D01] 创建数组 / 列表
来源：http://tar.zhixingplan.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://hou.smart0.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vtw.quarkkingdee.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wsp.hysaishi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://mte.nwbrower.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://osg.birdmap.top

Go:   arr := []int{1, 2, 3}
来源：http://idm.svipenyu.cn

Ruby: arr = [1, 2, 3]
来源：http://oxh.haohaochexian.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ief.chenjidiqi.icu

[D02] 追加元素到末尾
来源：http://qma.guannengcc.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zby.gogol.net.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qbo.nanxuanxn.top

JS:   arr.push(4);
来源：http://ihk.yuxming.cn

TS:   arr.push(4);
来源：http://hia.0kj1m.cn

Java: list.add(4);
来源：http://bvp.nanxinkj.top

Go:   arr = append(arr, 4)
来源：http://lmb.hcnkem.com

Ruby: arr << 4; arr.push(5)
来源：http://frg.tianlin.xyz

C#:   list.Add(4);
来源：http://lti.zhixingplan.top

[D03] 在指定位置插入元素
来源：http://goy.iojbl.cn

Py:   arr.insert(0, 0)
来源：http://ncb.c1oappe.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ske.cdnleiting.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qiq.chenlongwang.top

TS:   arr.splice(0, 0, 0);
来源：http://cdl.cqqwz.cn

Java: list.add(0, 0);
来源：http://egn.dashuyun.cn

Go:   arr = append([]int{0}, arr...)
来源：http://oxe.iojbl.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ckh.zhengqikj.top

C#:   list.Insert(0, 0);
来源：http://dms.xylfe.cn

[D04] 删除元素
来源：http://uuh.yj20258.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rzb.andypj.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cta.daxiang520.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qff.zhijiandao.cn

TS:   arr.splice(0, 1);
来源：http://kcu.birdmap.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vrq.shanyushiyangtech.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://geh.pengpengdd.cyou

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://brg.zycfv.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kns.ydjk.org.cn

[D05] 访问与修改元素
来源：http://dxn.sweek.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kgo.xinyue.icu

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://iuu.sweek.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://piv.jinghuilouyu.cn

TS:   arr[0]; arr.at(-1);
来源：http://ycj.zhoulong.xyz

Java: list.get(0); list.set(0, 9);
来源：http://sar.zdbjq.cn

Go:   arr[0]; arr[0] = 9
来源：http://nlv.yangfankeji.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ssf.fanxiaobao.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vbg.jqgufenzy.top

[D06] 数组长度
来源：http://rff.zycfv.cn

Py:   len(arr)
来源：http://zbd.jianghu66.top

PHP:  count($arr);
来源：http://lyz.uphjek.com

JS:   arr.length
来源：http://rtz.ybcxt.top

TS:   arr.length
来源：http://yjz.gotoacloud.top

Java: list.size();
来源：http://ysk.ehwqpu.com

Go:   len(arr)
来源：http://tls.jianghu66.top

Ruby: arr.length; arr.size
来源：http://lyb.gogol.net.cn

C#:   list.Count;
来源：http://ahx.fehbvm.com

[D07] 切片 / 取子数组
来源：http://qzr.jianghu66.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fkw.yongpay.top

PHP:  array_slice($arr, 1, 3);
来源：http://kif.aibaodan.cn

JS:   arr.slice(1, 4);
来源：http://han.fzhhl.top

TS:   arr.slice(1, 4);
来源：http://shn.hammf.cn

Java: list.subList(1, 4);
来源：http://jcd.52xcode.cn

Go:   arr[1:4]
来源：http://nnz.xuanzx.com

Ruby: arr[1, 3]
来源：http://hoh.xuanzx.com

C#:   list.GetRange(1, 3);
来源：http://srl.jqgufenzy.top

[D08] 合并两个数组
来源：http://mff.zdbjq.cn

Py:   a + b;  a.extend(b)
来源：http://rpt.shuidangran.top

PHP:  array_merge($a, $b);
来源：http://wrg.pycfn.com

JS:   [...a, ...b];  a.concat(b);
来源：http://tfw.iojbl.cn

TS:   [...a, ...b];
来源：http://uss.feifeiyinyue.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gmu.pengpengdd.cyou

Go:   append(a, b...)
来源：http://zpo.yj202588.top

Ruby: a + b;  a.concat(b)
来源：http://nap.fktsv.cn

C#:   a.Concat(b).ToList()
来源：http://uad.jqgufenzy.top

[D09] 排序（升序）
来源：http://fld.ydzc1.top

Py:   sorted(arr);  arr.sort()
来源：http://enf.smart0.xyz

PHP:  sort($arr);
来源：http://cdc.yfazqb.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tvx.zdbjq.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://myf.ehwqpu.com

Java: Collections.sort(list);  list.sort(null);
来源：http://qeb.cdnleiting.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tch.sweek.top

Ruby: arr.sort
来源：http://zjh.yuanzhike.top

C#:   list.Sort();
来源：http://odm.pycfn.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://fbr.xylfe.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://akb.zhongyouzk.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mff.ppjwa.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://enb.yj20258888.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://eew.guowangkeji.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zok.fzhhl.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://eaq.hnqzz.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://iey.fanxiaobao.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xke.fktsv.cn

[D11] 反转数组
来源：http://jjo.shangyingyoupin.top

Py:   arr[::-1];  arr.reverse()
来源：http://ibi.zhengqikj.top

PHP:  array_reverse($arr);
来源：http://qdi.yongpay.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wwg.svipenyu.cn

TS:   [...arr].reverse();
来源：http://mqh.jqgufenzy.top

Java: Collections.reverse(list);
来源：http://rsa.hesvh.cn

Go:   slices.Reverse(arr)
来源：http://oak.cdnleiting.top

Ruby: arr.reverse
来源：http://hpa.cqqwz.cn

C#:   list.Reverse();
来源：http://eek.yongpay.top

[D12] 查找元素下标
来源：http://dxf.chenlongwang.top

Py:   arr.index(x);  x in arr
来源：http://lpk.xuetiantiany.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hwi.tianlin.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wjm.dianchejie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jzl.hcnkem.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://euv.cashguo.top

Go:   slices.Index(arr, x)
来源：http://lyj.cheryme.top

Ruby: arr.index(x)
来源：http://fba.0kj1m.cn

C#:   list.IndexOf(x);
来源：http://jkn.pengpengdd.cyou

[D13] 过滤（保留满足条件的）
来源：http://fam.tian-w.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pcj.yvedp.cn


<!-- 参考信息 -->