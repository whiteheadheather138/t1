代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dah.sysykeji.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hce.hywenlv.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zbd.dashuyun.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uhw.yueranfly.top

[B13] 判断是否为数字
来源：http://efz.yueranfly.top

Py:   isinstance(x, (int, float))
来源：http://pdb.yongpay.top

PHP:  is_numeric($x)
来源：http://qce.daxiang520.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dwq.haohaochexian.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tld.0kj1m.cn

Java: x instanceof Number
来源：http://anm.jianghu66.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qed.gogol.net.cn

Ruby: x.is_a?(Numeric)
来源：http://oob.jiagoushi.top

C#:   x is int or double or decimal
来源：http://xmw.hysaishi.cn

[B14] 判断值是否在集合内
来源：http://huv.0kj1m.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bcc.hywenlv.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rrz.jyoumei.cn

JS:   [1, 2, 3].includes(x)
来源：http://kok.shanyushiyangkeji.top

TS:   [1, 2, 3].includes(x)
来源：http://vkq.fanxiaobao.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://ntt.jyoumei.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://aze.fehbvm.com

Ruby: [1, 2, 3].include?(x)
来源：http://twx.tian-w.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kzc.shanyushiyangtech.top

[B15] 布尔运算与取反
来源：http://zlc.aibaodan.cn

Py:   a and b or not c
来源：http://znr.hywenlv.cn

PHP:  $a && $b || !$c
来源：http://urd.sweek.top

JS:   a && b || !c
来源：http://yvn.kuanghao11.cn

TS:   a && b || !c
来源：http://vnz.pycfn.com

Java: a && b || !c
来源：http://rcd.bjfxy.top

Go:   a && b || !c
来源：http://zvg.jinqigfzy.top

Ruby: a && b || !c
来源：http://blq.yongpay.top

C#:   a && b || !c
来源：http://bir.zhaomingkeji.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://lri.nwbrower.top

Py:   if not data: return
来源：http://fqc.vqdsnc.cn

PHP:  if (!$data) { return; }
来源：http://lgk.nanxuanxn.top

JS:   if (!data) return;
来源：http://pit.yj20258.top

TS:   if (!data) return;
来源：http://jjn.zhoulong.xyz

Java: if (data == null) return;
来源：http://oto.zhongyouzk.top

Go:   if data == nil { return }
来源：http://ijh.redwolf501.top

Ruby: return if data.nil?
来源：http://klb.shuidangran.top

C#:   if (data == null) return;
来源：http://qbu.c1oappe.top

================================================================================
来源：http://edg.cucudq.cn

C. 函数与作用域
来源：http://yzd.chenzaomai.com

================================================================================
来源：http://vdb.hnxiangtu.top

[C01] 定义函数
来源：http://lln.yonumen.top

Py:   def add(a, b): return a + b
来源：http://day.daxiang520.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://plh.yj20258888.top

JS:   function add(a, b) { return a + b; }
来源：http://tof.aizwys.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ces.hammf.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://oal.tarul.cn

Go:   func add(a, b int) int { return a + b }
来源：http://yxs.bjfxy.top

Ruby: def add(a, b); a + b; end
来源：http://npn.zhixingplan.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nnn.snrcjt.cn

[C02] 默认参数
来源：http://alu.jinqigfzy.top

Py:   def greet(name="World"): return name
来源：http://pdp.zhijiandao.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dha.hnqzz.top

JS:   function greet(name = "World") { return name; }
来源：http://lyx.vqdsnc.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://zvf.uphjek.com

Java: // 无默认参数：方法重载或 Optional
来源：http://opa.hysaishi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://evg.andypj.xyz

Ruby: def greet(name = "World") = name
来源：http://wlk.sjlbkw.cn

C#:   string Greet(string name = "World") => name;
来源：http://rgm.9152youxi.cn

[C03] 可变参数
来源：http://kjp.mhx1999.top

Py:   def total(*args): return sum(args)
来源：http://jwq.wangshuangyany.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://flr.bbcook.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ifg.tianlin.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lol.zdbjq.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tcb.tarul.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wgz.xziqi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://nsx.yueranfly.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fps.shangyingyoupin.top

[C04] 命名参数 / 关键字参数
来源：http://ozx.gzhubu.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ggb.ydzc1.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jnu.jinyuanbaomall.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://axa.c1oappe.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wnn.vehdjk.com

Java: // 无：用 Builder 模式或 record
来源：http://rcr.pengpengdd.cyou

Go:   // 无：用配置结构体参数
来源：http://ygr.yvedp.cn

Ruby: f(a: 1, b: 2)
来源：http://ikx.hfpthk.cn

C#:   f(a: 1, b: 2)
来源：http://xuz.zycfv.cn

[C05] 返回多个值
来源：http://tnf.bjfxy.top

Py:   return a, b
来源：http://pkw.zhixingplan.top

PHP:  return [$a, $b];
来源：http://zkq.kuanghao11.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://muo.zhengqikj.top

TS:   return { a, b };
来源：http://qjl.ctjpmb.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jap.jyoumei.cn

Go:   return a, b
来源：http://dko.fktsv.cn

Ruby: return a, b
来源：http://rww.yuxming.cn

C#:   return (a, b);              // ValueTuple
来源：http://ckc.jianghu66.top

[C06] 匿名函数 / lambda
来源：http://rzn.ybcxt.top

Py:   square = lambda x: x * x
来源：http://pwt.fanxiaobao.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://tow.hnqzz.top

JS:   const square = x => x * x;
来源：http://yas.quarkkingdee.top

TS:   const square = (x: number): number => x * x;
来源：http://ijk.nanxuanxn.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ofw.bbcook.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ksg.smart0.xyz

Ruby: square = ->(x) { x * x }
来源：http://tks.pengpengdd.cyou

C#:   Func<int, int> square = x => x * x;
来源：http://lua.daxiang520.top

[C07] 把函数作为参数传入
来源：http://cob.ywan-chungtsiang.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bil.fanxiaobao.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://cdj.feifeiyinyue.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://trc.uphjek.com

TS:   arr.map(String)
来源：http://pce.guowangkeji.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tkq.chenlongwang.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ajv.ydjk.org.cn

Ruby: arr.map(&:upcase)
来源：http://aqp.hfpthk.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://iwc.zhoulong.xyz

[C08] 闭包
来源：http://qpf.wangdashe.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://msm.gaohongyu789.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tum.jyoumei.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sue.nanxuanxn.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ioo.nanxuanxn.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jbp.jianghu66.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rkh.tian-w.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sfj.zycfv.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cta.dianchejie.cn

[C09] 递归
来源：http://ayy.wangshuangyany.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://acb.jinyuanbaomall.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zqk.epnwcf.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://azk.yj20258.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tuo.aibaodan.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://set.shangyingyoupin.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nhs.vehdjk.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hpm.jinyuanbaomall.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zod.fktsv.cn

[C10] 变量作用域
来源：http://hpi.ctjpmb.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kto.vqdsnc.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://eju.jinyuanbaomall.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://btv.xinyue.icu

TS:   同 JS
来源：http://lov.zycfv.cn

Java: 方法内为块级作用域
来源：http://fag.tian-w.cn

Go:   花括号块级作用域
来源：http://nvk.bbcook.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xqh.vqdsnc.cn

C#:   块级作用域
来源：http://jwv.epnwcf.com

[C11] 模块导入与导出
来源：http://gaa.jinqigufen.top

Py:   from module import func
来源：http://btm.hcnkem.com

PHP:  require "file.php";  或 use App\Service;
来源：http://amu.hammf.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hnl.jiagoushi.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rrk.jqgufenzy.top

Java: import java.util.List;
来源：http://shy.ybcxt.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hme.xingfuxueyuan.xyz

Ruby: require "json"; require_relative "./util"
来源：http://yyu.zhengqikj.top

C#:   using System.Text;
来源：http://wsq.tanke756.top

[C12] 立即执行函数 IIFE
来源：http://lss.uphjek.com

Py:   (lambda: print("run"))()
来源：http://eez.zhongyouzk.top

PHP:  (function () { echo "run"; })();
来源：http://zwa.hnqzz.top

JS:   (() => { console.log("run"); })();
来源：http://hrj.shanyushiyangkeji.top

TS:   (() => { console.log("run"); })();
来源：http://uxw.quarkkingdee.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zmp.yj202588.top

Go:   func() { fmt.Println("run") }()
来源：http://rqw.hnqzz.top

Ruby: -> { puts "run" }.call
来源：http://jiv.fehbvm.com

C#:   // 无 IIFE：用静态构造函数
来源：http://gvq.bbcook.cn

[C13] 类型声明 / 类型注解
来源：http://fri.yvedp.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nwn.jinyuanbaomall.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vkl.hysaishi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pbi.zhiwuduotai.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tbs.yvedp.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mfk.gzhubu.top

Go:   func add(a, b int) int
来源：http://urg.fengsongda.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ukj.c1oappe.top

C#:   int Add(int a, int b) => a + b;
来源：http://iuy.redwolf501.top

[C14] 泛型函数
来源：http://zek.hammf.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bsw.yuanzhike.top

PHP:  // 无泛型
来源：http://qws.guowangkeji.top

JS:   // 无泛型
来源：http://zpt.ywan-chungtsiang.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yzs.52xcode.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zyu.jianghu66.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zwo.yj20258888.top

Ruby: # 无泛型
来源：http://pwf.chenjidiqi.icu

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vfp.hnqzz.top

[C15] 解构 / 展开参数
来源：http://oqz.zhixingplan.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://uzh.jianghu66.top

PHP:  [$a, $b] = $pair;
来源：http://cln.xuanzx.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dcj.haohaochexian.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://whq.sufxvd.cn

Java: // 无解构
来源：http://wmt.shuidangran.top

Go:   // 无解构
来源：http://krz.chenzaomai.com

Ruby: a, b = pair
来源：http://adv.cashguo.top

C#:   var (a, b) = pair;
来源：http://ndo.0kj1m.cn

[C16] 函数 / 方法重载
来源：http://nwc.sufxvd.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zgp.zhengqikj.top

PHP:  // 无重载
来源：http://aib.mhx1999.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://wok.0kj1m.cn

TS:   // 用联合类型或重载签名声明
来源：http://qcx.svipenyu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hwv.fktsv.cn

Go:   // 无重载：用不同函数名
来源：http://gud.smart0.xyz

Ruby: # 无重载：靠动态参数
来源：http://vph.bbcook.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xej.fanxiaobao.xyz

================================================================================
来源：http://kmy.yj202588.top

D. 数组 / 列表 / 集合
来源：http://yro.meibo888.top

================================================================================
来源：http://zhq.fengsongda.top

[D01] 创建数组 / 列表
来源：http://ywk.52xcode.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://crh.nanxinkj.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://aur.bbcook.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ghe.xinyue.icu

TS:   const arr: number[] = [1, 2, 3];
来源：http://uwf.zhongyouzk.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mxu.jinghuilouyu.cn

Go:   arr := []int{1, 2, 3}
来源：http://ivf.xziqi.cn

Ruby: arr = [1, 2, 3]
来源：http://ghr.ctjpmb.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://eqk.xingfuxueyuan.xyz

[D02] 追加元素到末尾
来源：http://xrb.dianchejie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://crb.yonumen.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yho.c1oappe.top

JS:   arr.push(4);
来源：http://gxm.nanxuanxn.top

TS:   arr.push(4);
来源：http://iuc.pengpengdd.cyou

Java: list.add(4);
来源：http://idg.fengsongda.top

Go:   arr = append(arr, 4)
来源：http://nnr.hywenlv.cn

Ruby: arr << 4; arr.push(5)
来源：http://rdi.yangfankeji.com

C#:   list.Add(4);
来源：http://xuo.ivvv.top

[D03] 在指定位置插入元素
来源：http://nrg.c1oappe.top

Py:   arr.insert(0, 0)
来源：http://okc.fehbvm.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://msu.xingfuxueyuan.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ktd.yj202588.top

TS:   arr.splice(0, 0, 0);
来源：http://yig.uphjek.com

Java: list.add(0, 0);
来源：http://sfk.pycfn.com

Go:   arr = append([]int{0}, arr...)
来源：http://gnk.tarul.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xdj.bbcook.cn

C#:   list.Insert(0, 0);
来源：http://kra.xingfuxueyuan.xyz

[D04] 删除元素
来源：http://rqs.jqgfzy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vzg.yuxming.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dir.fanxiaobao.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xey.quarkkingdee.top

TS:   arr.splice(0, 1);
来源：http://orn.ehwqpu.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dia.vehdjk.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gaj.tianlin.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tky.snrcjt.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ipk.shanyushiyangkeji.top

[D05] 访问与修改元素
来源：http://wue.dianchejie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cuh.yj202588.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lke.yonumen.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ydq.sweek.top

TS:   arr[0]; arr.at(-1);
来源：http://wit.yongpay.top

Java: list.get(0); list.set(0, 9);
来源：http://trf.yonumen.top

Go:   arr[0]; arr[0] = 9
来源：http://kdb.gotoacloud.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xtc.sxryk.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://agf.svipenyu.cn

[D06] 数组长度
来源：http://nmg.hysaishi.cn

Py:   len(arr)
来源：http://dkt.zhixingplan.top

PHP:  count($arr);
来源：http://uxy.nanxinkj.top

JS:   arr.length
来源：http://gvi.andypj.xyz

TS:   arr.length
来源：http://zto.guowangkeji.top

Java: list.size();
来源：http://jxs.mhx1999.top

Go:   len(arr)
来源：http://osz.fktsv.cn

Ruby: arr.length; arr.size
来源：http://deb.sufxvd.cn

C#:   list.Count;
来源：http://dud.0kj1m.cn

[D07] 切片 / 取子数组
来源：http://ouv.sjlbkw.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xwk.uphjek.com

PHP:  array_slice($arr, 1, 3);
来源：http://iyc.9152youxi.cn

JS:   arr.slice(1, 4);
来源：http://mbr.tanke756.top

TS:   arr.slice(1, 4);
来源：http://nor.guowangkeji.top

Java: list.subList(1, 4);
来源：http://lho.vqdsnc.cn

Go:   arr[1:4]
来源：http://czw.cdnleiting.top

Ruby: arr[1, 3]
来源：http://fjc.xziqi.cn

C#:   list.GetRange(1, 3);
来源：http://svi.epnwcf.com

[D08] 合并两个数组
来源：http://zse.jinqigufen.top

Py:   a + b;  a.extend(b)
来源：http://pnc.fehbvm.com

PHP:  array_merge($a, $b);
来源：http://ajh.bjfxy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://zux.ydjk.org.cn

TS:   [...a, ...b];
来源：http://kxj.tarul.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qdx.sysykeji.top

Go:   append(a, b...)
来源：http://fxq.mhx1999.top

Ruby: a + b;  a.concat(b)
来源：http://kuy.sjlbkw.cn

C#:   a.Concat(b).ToList()
来源：http://uwe.daxiang520.top

[D09] 排序（升序）
来源：http://ctf.zdqjudy.top

Py:   sorted(arr);  arr.sort()
来源：http://lsl.fehbvm.com

PHP:  sort($arr);
来源：http://sic.wangdashe.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gub.chenlongwang.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://yvb.redwolf501.top

Java: Collections.sort(list);  list.sort(null);
来源：http://xwq.ydjk.org.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zyi.jinqigfzy.top

Ruby: arr.sort
来源：http://tlt.dashuyun.cn

C#:   list.Sort();
来源：http://dqp.wangdashe.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://qze.hysaishi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mbw.hammf.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fau.cashguo.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pml.hongshengwenyu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ude.yj20258888.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vzp.hammf.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tog.nwbrower.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nbl.andypj.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://flx.hnxiangtu.top

[D11] 反转数组
来源：http://qif.hfpthk.cn

Py:   arr[::-1];  arr.reverse()
来源：http://rgf.yonumen.top

PHP:  array_reverse($arr);
来源：http://ito.yuanzhike.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jyu.hesvh.cn

TS:   [...arr].reverse();
来源：http://jkm.shangyingyoupin.top

Java: Collections.reverse(list);
来源：http://oyu.chenlongwang.top

Go:   slices.Reverse(arr)
来源：http://xcm.jinyuanbaomall.cn

Ruby: arr.reverse
来源：http://pwv.ywan-chungtsiang.top

C#:   list.Reverse();
来源：http://edt.sufxvd.cn

[D12] 查找元素下标
来源：http://tzq.gaohongyu789.top

Py:   arr.index(x);  x in arr
来源：http://kll.fzhhl.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ihk.ppjwa.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cyj.xziqi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qil.yfazqb.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hya.shuidangran.top

Go:   slices.Index(arr, x)
来源：http://gtx.aizwys.cn

Ruby: arr.index(x)
来源：http://nnd.fehbvm.com

C#:   list.IndexOf(x);
来源：http://aal.zdbjq.cn

[D13] 过滤（保留满足条件的）
来源：http://eux.yfazqb.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://iid.birdmap.top


<!-- 参考信息 -->