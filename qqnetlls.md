代发 wailian999

[B13] 判断是否为数字
来源：http://ytx.dashuyun.cn

Py:   isinstance(x, (int, float))
来源：http://cau.hywenlv.cn

PHP:  is_numeric($x)
来源：http://rrn.sjlbkw.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yxn.shanyushiyangtech.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aik.sweek.top

Java: x instanceof Number
来源：http://wbz.yangfankeji.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kle.zhengqikj.top

Ruby: x.is_a?(Numeric)
来源：http://jwp.gogol.net.cn

C#:   x is int or double or decimal
来源：http://dji.fengsongda.top

[B14] 判断值是否在集合内
来源：http://wif.dashuyun.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hmq.vqdsnc.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wqo.meibo888.top

JS:   [1, 2, 3].includes(x)
来源：http://nxc.snrcjt.cn

TS:   [1, 2, 3].includes(x)
来源：http://ewt.sjlbkw.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://mik.xuanzx.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bqa.yueranfly.top

Ruby: [1, 2, 3].include?(x)
来源：http://weg.yanxiufei.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zfd.fzhhl.top

[B15] 布尔运算与取反
来源：http://mws.mhx1999.top

Py:   a and b or not c
来源：http://prb.9152youxi.cn

PHP:  $a && $b || !$c
来源：http://rib.sxryk.cn

JS:   a && b || !c
来源：http://cxw.svipenyu.cn

TS:   a && b || !c
来源：http://pte.dianchejie.cn

Java: a && b || !c
来源：http://xho.xuanzx.com

Go:   a && b || !c
来源：http://ozt.gzhubu.top

Ruby: a && b || !c
来源：http://pgp.0kj1m.cn

C#:   a && b || !c
来源：http://htd.zycfv.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vbi.quarkkingdee.top

Py:   if not data: return
来源：http://ump.ydjk.org.cn

PHP:  if (!$data) { return; }
来源：http://ehr.jlsjyb.cn

JS:   if (!data) return;
来源：http://qep.zhiwuduotai.top

TS:   if (!data) return;
来源：http://mls.tian-w.cn

Java: if (data == null) return;
来源：http://lvv.zhiwuduotai.top

Go:   if data == nil { return }
来源：http://roh.epnwcf.com

Ruby: return if data.nil?
来源：http://tvg.dashuyun.cn

C#:   if (data == null) return;
来源：http://dkq.c1oappe.top

================================================================================
来源：http://mju.xylfe.cn

C. 函数与作用域
来源：http://bdk.hywenlv.cn

================================================================================
来源：http://ffh.zhongyouzk.top

[C01] 定义函数
来源：http://sdj.haohaochexian.top

Py:   def add(a, b): return a + b
来源：http://yqv.gaohongyu789.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ofh.tianlin.xyz

JS:   function add(a, b) { return a + b; }
来源：http://hxv.yj20258888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nhd.cashguo.top

Java: static int add(int a, int b) { return a + b; }
来源：http://gub.ybcxt.top

Go:   func add(a, b int) int { return a + b }
来源：http://crk.c1oappe.top

Ruby: def add(a, b); a + b; end
来源：http://obj.yuanzhike.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tft.jinqigfzy.top

[C02] 默认参数
来源：http://lpr.nwbrower.top

Py:   def greet(name="World"): return name
来源：http://tae.sysykeji.top

PHP:  function greet($name = "World") { return $name; }
来源：http://zll.hysaishi.cn

JS:   function greet(name = "World") { return name; }
来源：http://opz.jqgfzy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://fyb.zhiwuduotai.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ebo.zhaomingkeji.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fwd.cucudq.cn

Ruby: def greet(name = "World") = name
来源：http://qqe.nanxinkj.top

C#:   string Greet(string name = "World") => name;
来源：http://kxd.zhaomingkeji.xyz

[C03] 可变参数
来源：http://cba.dashuyun.cn

Py:   def total(*args): return sum(args)
来源：http://saw.snrcjt.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://imx.yvedp.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dtn.fehbvm.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xki.pengpengdd.cyou

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vwx.ivvv.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://afu.snrcjt.cn

Ruby: def total(*nums); nums.sum; end
来源：http://mco.ehwqpu.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ywr.chenjidiqi.icu

[C04] 命名参数 / 关键字参数
来源：http://ebm.ybcxt.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wgc.hnqzz.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://icd.yj202588.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lfw.yanxiufei.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yqa.hnxiangtu.top

Java: // 无：用 Builder 模式或 record
来源：http://dja.hywenlv.cn

Go:   // 无：用配置结构体参数
来源：http://kxn.nanxuanxn.top

Ruby: f(a: 1, b: 2)
来源：http://qkv.vehdjk.com

C#:   f(a: 1, b: 2)
来源：http://fid.svipenyu.cn

[C05] 返回多个值
来源：http://cdy.cheryme.top

Py:   return a, b
来源：http://gkp.fzhhl.top

PHP:  return [$a, $b];
来源：http://jzg.zycfv.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://vgc.yj20258888.top

TS:   return { a, b };
来源：http://gyy.ydjk.org.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fxu.feifeiyinyue.top

Go:   return a, b
来源：http://byd.hnxiangtu.top

Ruby: return a, b
来源：http://aen.jinqigfzy.top

C#:   return (a, b);              // ValueTuple
来源：http://qom.cashguo.top

[C06] 匿名函数 / lambda
来源：http://jbd.dashuyun.cn

Py:   square = lambda x: x * x
来源：http://hea.yongpay.top

PHP:  $square = fn($x) => $x * $x;
来源：http://hvn.nanxuanxn.top

JS:   const square = x => x * x;
来源：http://sik.sweek.top

TS:   const square = (x: number): number => x * x;
来源：http://lzd.ydjk.org.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://efm.sjlbkw.cn

Go:   sq := func(x int) int { return x * x }
来源：http://swt.fengsongda.top

Ruby: square = ->(x) { x * x }
来源：http://etx.haohaochexian.top

C#:   Func<int, int> square = x => x * x;
来源：http://svv.fengsongda.top

[C07] 把函数作为参数传入
来源：http://tnz.xylfe.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rel.svipenyu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://gxq.316326.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://coe.yj20258.top

TS:   arr.map(String)
来源：http://dtz.meibo888.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://klu.yuxming.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://npx.tanke756.top

Ruby: arr.map(&:upcase)
来源：http://sxo.daria6918.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mxs.zdbjq.cn

[C08] 闭包
来源：http://ctp.0kj1m.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ost.ehwqpu.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uuc.epnwcf.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sks.hnxiangtu.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gbj.havefunace.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lge.chenzaomai.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ovm.fehbvm.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hax.hcnkem.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://okm.zycfv.cn

[C09] 递归
来源：http://lke.cheryme.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://use.yuxming.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dxp.ybcxt.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cdv.dashuyun.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://erq.yvedp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pci.jqgfzy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uax.gotoacloud.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://afe.jqgfzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tyx.fehbvm.com

[C10] 变量作用域
来源：http://uja.jinqigfzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://unh.vehdjk.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vvc.guannengcc.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yjr.tianlin.xyz

TS:   同 JS
来源：http://jbq.fktsv.cn

Java: 方法内为块级作用域
来源：http://jwm.yongpay.top

Go:   花括号块级作用域
来源：http://xio.gaohongyu789.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://taq.sxryk.cn

C#:   块级作用域
来源：http://grr.xziqi.cn

[C11] 模块导入与导出
来源：http://aun.vqdsnc.cn

Py:   from module import func
来源：http://pdo.zhixingplan.top

PHP:  require "file.php";  或 use App\Service;
来源：http://uhh.chenzaomai.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://nww.ybcxt.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hvg.epnwcf.com

Java: import java.util.List;
来源：http://lct.nanxuanxn.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vgj.jqgufenzy.top

Ruby: require "json"; require_relative "./util"
来源：http://vum.yangfankeji.com

C#:   using System.Text;
来源：http://mid.zdbjq.cn

[C12] 立即执行函数 IIFE
来源：http://ftm.fktsv.cn

Py:   (lambda: print("run"))()
来源：http://bvy.dashuyun.cn

PHP:  (function () { echo "run"; })();
来源：http://nyp.hnxiangtu.top

JS:   (() => { console.log("run"); })();
来源：http://jrd.wangshuangyany.cn

TS:   (() => { console.log("run"); })();
来源：http://rji.cheryme.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rda.bbcook.cn

Go:   func() { fmt.Println("run") }()
来源：http://stz.bjfxy.top

Ruby: -> { puts "run" }.call
来源：http://tsr.ydzc1.top

C#:   // 无 IIFE：用静态构造函数
来源：http://uyf.bbcook.cn

[C13] 类型声明 / 类型注解
来源：http://nnh.guowangkeji.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dyz.chenlongwang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dsn.ywan-chungtsiang.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://skq.cdnleiting.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://afg.yangfankeji.com

Java: int add(int a, int b) { return a + b; }
来源：http://qex.yonumen.top

Go:   func add(a, b int) int
来源：http://dpg.tarul.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mna.aizwys.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fuq.c1oappe.top

[C14] 泛型函数
来源：http://usa.shangyingyoupin.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hmr.jyoumei.cn

PHP:  // 无泛型
来源：http://xec.jinqigufen.top

JS:   // 无泛型
来源：http://nzz.nanxinkj.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mgf.xziqi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qrj.pengpengdd.cyou

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rzj.havefunace.top

Ruby: # 无泛型
来源：http://npa.gotoacloud.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hgo.yj20258.top

[C15] 解构 / 展开参数
来源：http://pyw.tianlin.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tut.shuidangran.top

PHP:  [$a, $b] = $pair;
来源：http://jdq.dashuyun.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jqd.dianchejie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pgf.0kj1m.cn

Java: // 无解构
来源：http://gau.nanxuanxn.top

Go:   // 无解构
来源：http://ubt.fzhhl.top

Ruby: a, b = pair
来源：http://gyg.snrcjt.cn

C#:   var (a, b) = pair;
来源：http://krl.ydzc1.top

[C16] 函数 / 方法重载
来源：http://ddi.xylfe.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xlk.zhiwuduotai.top

PHP:  // 无重载
来源：http://rfs.hesvh.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://pdw.zhiwuduotai.top

TS:   // 用联合类型或重载签名声明
来源：http://sxa.jinqigufen.top

Java: void f(int a) {}  void f(String a) {}
来源：http://gca.sweek.top

Go:   // 无重载：用不同函数名
来源：http://yrf.chenzaomai.com

Ruby: # 无重载：靠动态参数
来源：http://xmi.daxiang520.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://rze.shuidangran.top

================================================================================
来源：http://srk.jinqigufen.top

D. 数组 / 列表 / 集合
来源：http://xuq.yonumen.top

================================================================================
来源：http://bnd.meibo888.top

[D01] 创建数组 / 列表
来源：http://zxj.jinghuilouyu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ipq.zdbjq.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rjy.52xcode.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://oud.gogol.net.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://vyb.fanxiaobao.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qok.yj20258.top

Go:   arr := []int{1, 2, 3}
来源：http://xnr.sjlbkw.cn

Ruby: arr = [1, 2, 3]
来源：http://wda.shanyushiyangtech.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rvy.daria6918.cn

[D02] 追加元素到末尾
来源：http://mgv.wangdashe.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cij.hammf.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://des.ydzc1.top

JS:   arr.push(4);
来源：http://xgy.meibo888.top

TS:   arr.push(4);
来源：http://aek.316326.xyz

Java: list.add(4);
来源：http://xle.wangdashe.top

Go:   arr = append(arr, 4)
来源：http://bzu.yanxiufei.cn

Ruby: arr << 4; arr.push(5)
来源：http://gft.sysykeji.top

C#:   list.Add(4);
来源：http://ixd.c1oappe.top

[D03] 在指定位置插入元素
来源：http://aqv.cucudq.cn

Py:   arr.insert(0, 0)
来源：http://qiu.shangyingyoupin.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://srm.sweek.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xik.c1oappe.top

TS:   arr.splice(0, 0, 0);
来源：http://jfy.zhongyouzk.top

Java: list.add(0, 0);
来源：http://vtq.xingfuxueyuan.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://oni.zhaomingkeji.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yjw.jinghuilouyu.cn

C#:   list.Insert(0, 0);
来源：http://yvg.mhx1999.top

[D04] 删除元素
来源：http://vlb.birdmap.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xkz.shzxlz.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sgz.jinqigufen.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fhm.chenlongwang.top

TS:   arr.splice(0, 1);
来源：http://nda.jyoumei.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vji.chenzaomai.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wcn.snrcjt.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vop.vqdsnc.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yzk.vehdjk.com

[D05] 访问与修改元素
来源：http://imn.kuanghao11.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fmc.andypj.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tiq.ppjwa.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bih.jinyuanbaomall.cn

TS:   arr[0]; arr.at(-1);
来源：http://dnu.mhx1999.top

Java: list.get(0); list.set(0, 9);
来源：http://izv.jqgufenzy.top

Go:   arr[0]; arr[0] = 9
来源：http://vqh.dashuyun.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qaa.cdnleiting.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://iss.hywenlv.cn

[D06] 数组长度
来源：http://xnw.yuxming.cn

Py:   len(arr)
来源：http://bjn.xingfuxueyuan.xyz

PHP:  count($arr);
来源：http://jtg.jlsjyb.cn

JS:   arr.length
来源：http://myd.nanxuanxn.top

TS:   arr.length
来源：http://utp.shangyingyoupin.top

Java: list.size();
来源：http://tye.fengsongda.top

Go:   len(arr)
来源：http://ddz.zhiwuduotai.top

Ruby: arr.length; arr.size
来源：http://eox.shzxlz.cn

C#:   list.Count;
来源：http://orm.birdmap.top

[D07] 切片 / 取子数组
来源：http://mlz.meibo888.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cef.gzhubu.top

PHP:  array_slice($arr, 1, 3);
来源：http://qfb.cqqwz.cn

JS:   arr.slice(1, 4);
来源：http://auo.vqdsnc.cn

TS:   arr.slice(1, 4);
来源：http://nrv.wangshuangyany.cn

Java: list.subList(1, 4);
来源：http://ien.feifeiyinyue.top

Go:   arr[1:4]
来源：http://jmc.zhongyouzk.top

Ruby: arr[1, 3]
来源：http://pbg.shangyingyoupin.top

C#:   list.GetRange(1, 3);
来源：http://phy.dianchejie.cn

[D08] 合并两个数组
来源：http://sih.shuidangran.top

Py:   a + b;  a.extend(b)
来源：http://zsh.0kj1m.cn

PHP:  array_merge($a, $b);
来源：http://ofu.nwbrower.top

JS:   [...a, ...b];  a.concat(b);
来源：http://agc.sweek.top

TS:   [...a, ...b];
来源：http://rcq.gaohongyu789.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jjf.shanyushiyangkeji.top

Go:   append(a, b...)
来源：http://hsf.ctjpmb.com

Ruby: a + b;  a.concat(b)
来源：http://xbj.hywenlv.cn

C#:   a.Concat(b).ToList()
来源：http://vjj.316326.xyz

[D09] 排序（升序）
来源：http://bhb.tian-w.cn

Py:   sorted(arr);  arr.sort()
来源：http://ppf.xingfuxueyuan.xyz

PHP:  sort($arr);
来源：http://ssi.wangshuangyany.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://phd.52xcode.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fvc.ywan-chungtsiang.top

Java: Collections.sort(list);  list.sort(null);
来源：http://msl.yvedp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://llj.gaohongyu789.top

Ruby: arr.sort
来源：http://ste.guowangkeji.top

C#:   list.Sort();
来源：http://gnn.xziqi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mvi.jinqigufen.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://eaq.yj20258888.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gtx.jlsjyb.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mns.sweek.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lbv.daxiang520.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rii.zycfv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ytw.snrcjt.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zzc.ctjpmb.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mqd.chenjidiqi.icu

[D11] 反转数组
来源：http://tyf.hongshengwenyu.top

Py:   arr[::-1];  arr.reverse()
来源：http://aim.sysykeji.top

PHP:  array_reverse($arr);
来源：http://clq.wangshuangyany.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hag.jqgufenzy.top

TS:   [...arr].reverse();
来源：http://tar.daria6918.cn

Java: Collections.reverse(list);
来源：http://adx.yongpay.top

Go:   slices.Reverse(arr)
来源：http://uyu.zhaomingkeji.xyz

Ruby: arr.reverse
来源：http://yzp.xingfuxueyuan.xyz

C#:   list.Reverse();
来源：http://kyp.svipenyu.cn

[D12] 查找元素下标
来源：http://rfc.sjlbkw.cn

Py:   arr.index(x);  x in arr
来源：http://pmb.ehwqpu.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vun.wangshuangyany.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ipm.cqqwz.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sdh.chenjidiqi.icu

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sjq.wangdashe.top

Go:   slices.Index(arr, x)
来源：http://hwg.pycfn.com

Ruby: arr.index(x)
来源：http://zym.wangshuangyany.cn

C#:   list.IndexOf(x);
来源：http://eae.xinyue.icu

[D13] 过滤（保留满足条件的）
来源：http://yhi.xuetiantiany.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zmi.sufxvd.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ubc.yueranfly.top

JS:   arr.filter(x => x > 3)
来源：http://kds.c1oappe.top

TS:   arr.filter(x => x > 3)
来源：http://wro.c1oappe.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ste.yangfankeji.com


<!-- 参考信息 -->