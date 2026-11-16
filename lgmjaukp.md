代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://fif.shangyingyoupin.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ipb.yj202588.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tlu.ctjpmb.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vqk.hongshengwenyu.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://opu.zdqjudy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zal.snrcjt.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rph.yangfankeji.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://eyg.chenzaomai.com

[B13] 判断是否为数字
来源：http://vwa.vqdsnc.cn

Py:   isinstance(x, (int, float))
来源：http://dax.meibo888.top

PHP:  is_numeric($x)
来源：http://ihb.wangshuangyany.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jmx.ydzc1.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yhf.xylfe.cn

Java: x instanceof Number
来源：http://zvg.yangfankeji.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ykw.52xcode.cn

Ruby: x.is_a?(Numeric)
来源：http://rkb.bjfxy.top

C#:   x is int or double or decimal
来源：http://vem.guannengcc.top

[B14] 判断值是否在集合内
来源：http://gkb.yj20258888.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yhq.xylfe.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://olo.andypj.xyz

JS:   [1, 2, 3].includes(x)
来源：http://xbt.zhaomingkeji.xyz

TS:   [1, 2, 3].includes(x)
来源：http://bbb.yvedp.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://bih.xuanzx.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://acg.ctjpmb.com

Ruby: [1, 2, 3].include?(x)
来源：http://yuz.fehbvm.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mht.xuetiantiany.cn

[B15] 布尔运算与取反
来源：http://lup.yj20258.top

Py:   a and b or not c
来源：http://ifh.gogol.net.cn

PHP:  $a && $b || !$c
来源：http://ccy.yuanzhike.top

JS:   a && b || !c
来源：http://uwe.316326.xyz

TS:   a && b || !c
来源：http://ymb.tanke756.top

Java: a && b || !c
来源：http://fws.uphjek.com

Go:   a && b || !c
来源：http://gib.xuanzx.com

Ruby: a && b || !c
来源：http://wyy.mhx1999.top

C#:   a && b || !c
来源：http://xsb.wangshuangyany.cn

[B16] 卫语句：不满足条件提前返回
来源：http://acs.zhaomingkeji.xyz

Py:   if not data: return
来源：http://zjc.jinqigfzy.top

PHP:  if (!$data) { return; }
来源：http://nuu.xuanzx.com

JS:   if (!data) return;
来源：http://mll.gogol.net.cn

TS:   if (!data) return;
来源：http://lvz.shzxlz.cn

Java: if (data == null) return;
来源：http://fuf.zhijiandao.cn

Go:   if data == nil { return }
来源：http://ioh.ybcxt.top

Ruby: return if data.nil?
来源：http://oml.chenlongwang.top

C#:   if (data == null) return;
来源：http://hle.ctjpmb.com

================================================================================
来源：http://bid.sufxvd.cn

C. 函数与作用域
来源：http://dmc.yj20258.top

================================================================================
来源：http://dkf.daxiang520.top

[C01] 定义函数
来源：http://shb.zhoulong.xyz

Py:   def add(a, b): return a + b
来源：http://udm.epnwcf.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xdv.tian-w.cn

JS:   function add(a, b) { return a + b; }
来源：http://abi.cheryme.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://klb.haohaochexian.top

Java: static int add(int a, int b) { return a + b; }
来源：http://kca.tian-w.cn

Go:   func add(a, b int) int { return a + b }
来源：http://eab.yj20258888.top

Ruby: def add(a, b); a + b; end
来源：http://jms.redwolf501.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://owp.xylfe.cn

[C02] 默认参数
来源：http://gou.vehdjk.com

Py:   def greet(name="World"): return name
来源：http://fmt.yangfankeji.com

PHP:  function greet($name = "World") { return $name; }
来源：http://jwo.bbcook.cn

JS:   function greet(name = "World") { return name; }
来源：http://bwk.ydjk.org.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://gpl.epnwcf.com

Java: // 无默认参数：方法重载或 Optional
来源：http://pyn.yj20258.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ezp.xuanzx.com

Ruby: def greet(name = "World") = name
来源：http://akm.sweek.top

C#:   string Greet(string name = "World") => name;
来源：http://feu.zhiwuduotai.top

[C03] 可变参数
来源：http://azf.ywan-chungtsiang.top

Py:   def total(*args): return sum(args)
来源：http://ynx.zhengqikj.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jie.zhengqikj.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yqu.jqgfzy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kvt.zhoulong.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xri.shuidangran.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mok.sysykeji.top

Ruby: def total(*nums); nums.sum; end
来源：http://lom.gogol.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rhe.birdmap.top

[C04] 命名参数 / 关键字参数
来源：http://amk.ehwqpu.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tpp.epnwcf.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hor.shzxlz.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://knr.cdnleiting.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mmk.fanxiaobao.xyz

Java: // 无：用 Builder 模式或 record
来源：http://njk.tanke756.top

Go:   // 无：用配置结构体参数
来源：http://aqn.fzhhl.top

Ruby: f(a: 1, b: 2)
来源：http://ywv.zhixingplan.top

C#:   f(a: 1, b: 2)
来源：http://iko.fzhhl.top

[C05] 返回多个值
来源：http://hjg.chenlongwang.top

Py:   return a, b
来源：http://yfw.tian-w.cn

PHP:  return [$a, $b];
来源：http://oni.xuanzx.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://byk.aizwys.cn

TS:   return { a, b };
来源：http://tvx.iojbl.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kij.iojbl.cn

Go:   return a, b
来源：http://ywz.hnqzz.top

Ruby: return a, b
来源：http://yfe.birdmap.top

C#:   return (a, b);              // ValueTuple
来源：http://qqa.fanxiaobao.xyz

[C06] 匿名函数 / lambda
来源：http://vcy.tanke756.top

Py:   square = lambda x: x * x
来源：http://nmu.9152youxi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fop.uphjek.com

JS:   const square = x => x * x;
来源：http://giu.yuanzhike.top

TS:   const square = (x: number): number => x * x;
来源：http://eim.meibo888.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://krd.yvedp.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ood.chenlongwang.top

Ruby: square = ->(x) { x * x }
来源：http://ngi.yuanzhike.top

C#:   Func<int, int> square = x => x * x;
来源：http://irz.nanxuanxn.top

[C07] 把函数作为参数传入
来源：http://kwv.chenjidiqi.icu

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://aze.gaohongyu789.top

PHP:  array_map("strtoupper", $arr);
来源：http://blp.quarkkingdee.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hda.sweek.top

TS:   arr.map(String)
来源：http://wyk.wangshuangyany.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pta.hysaishi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dto.nanxinkj.top

Ruby: arr.map(&:upcase)
来源：http://msp.gotoacloud.top

C#:   arr.Select(s => s.ToUpper())
来源：http://pcm.nwbrower.top

[C08] 闭包
来源：http://uxr.zhengqikj.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://aig.tianlin.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wul.yvedp.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yiy.cqqwz.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gyf.sysykeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qqj.chenlongwang.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ldt.nanxuanxn.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://aux.wangshuangyany.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zgx.feifeiyinyue.top

[C09] 递归
来源：http://uxp.xuetiantiany.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jtr.gotoacloud.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://aum.snrcjt.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://auc.ctjpmb.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ugi.sufxvd.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lup.havefunace.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://htu.yuxming.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kkl.yj20258.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sqa.ivvv.top

[C10] 变量作用域
来源：http://ulg.wangdashe.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ctj.yueranfly.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vyc.hywenlv.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dmv.quarkkingdee.top

TS:   同 JS
来源：http://kjd.pengpengdd.cyou

Java: 方法内为块级作用域
来源：http://beq.jiagoushi.top

Go:   花括号块级作用域
来源：http://lgw.fehbvm.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vbj.haohaochexian.top

C#:   块级作用域
来源：http://yae.uphjek.com

[C11] 模块导入与导出
来源：http://ryr.pycfn.com

Py:   from module import func
来源：http://icr.zycfv.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pla.zhaomingkeji.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://rve.redwolf501.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://efs.yj202588.top

Java: import java.util.List;
来源：http://fje.sysykeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zlp.yj202588.top

Ruby: require "json"; require_relative "./util"
来源：http://nkz.shuidangran.top

C#:   using System.Text;
来源：http://goz.sxryk.cn

[C12] 立即执行函数 IIFE
来源：http://bra.bbcook.cn

Py:   (lambda: print("run"))()
来源：http://ydi.0kj1m.cn

PHP:  (function () { echo "run"; })();
来源：http://uyp.shuidangran.top

JS:   (() => { console.log("run"); })();
来源：http://axx.jinyuanbaomall.cn

TS:   (() => { console.log("run"); })();
来源：http://bbe.shanyushiyangtech.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qvi.bjfxy.top

Go:   func() { fmt.Println("run") }()
来源：http://dar.xinyue.icu

Ruby: -> { puts "run" }.call
来源：http://lhb.xingfuxueyuan.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://cco.dashuyun.cn

[C13] 类型声明 / 类型注解
来源：http://ykc.zhaomingkeji.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pod.sxryk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wiw.wangshuangyany.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://aon.jinqigfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rrw.hesvh.cn

Java: int add(int a, int b) { return a + b; }
来源：http://rzk.fzhhl.top

Go:   func add(a, b int) int
来源：http://eit.ybcxt.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zyp.tanke756.top

C#:   int Add(int a, int b) => a + b;
来源：http://jfi.ppjwa.cn

[C14] 泛型函数
来源：http://klu.feifeiyinyue.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://maz.iojbl.cn

PHP:  // 无泛型
来源：http://vpa.9152youxi.cn

JS:   // 无泛型
来源：http://wox.redwolf501.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://frw.xuanzx.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tni.quarkkingdee.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ekv.birdmap.top

Ruby: # 无泛型
来源：http://asw.jlsjyb.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wwl.tanke756.top

[C15] 解构 / 展开参数
来源：http://cvl.52xcode.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gyt.tanke756.top

PHP:  [$a, $b] = $pair;
来源：http://kvj.uphjek.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pgp.hywenlv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://phg.jinyuanbaomall.cn

Java: // 无解构
来源：http://mjg.daxiang520.top

Go:   // 无解构
来源：http://lvw.fzhhl.top

Ruby: a, b = pair
来源：http://nhi.aizwys.cn

C#:   var (a, b) = pair;
来源：http://qki.snrcjt.cn

[C16] 函数 / 方法重载
来源：http://ono.zhiwuduotai.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zeb.cashguo.top

PHP:  // 无重载
来源：http://pem.cucudq.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://hda.feifeiyinyue.top

TS:   // 用联合类型或重载签名声明
来源：http://sjw.yj20258.top

Java: void f(int a) {}  void f(String a) {}
来源：http://nsz.fzhhl.top

Go:   // 无重载：用不同函数名
来源：http://uvc.jinghuilouyu.cn

Ruby: # 无重载：靠动态参数
来源：http://iju.jyoumei.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qkg.snrcjt.cn

================================================================================
来源：http://nev.fktsv.cn

D. 数组 / 列表 / 集合
来源：http://vks.cqqwz.cn

================================================================================
来源：http://bdb.xinyue.icu

[D01] 创建数组 / 列表
来源：http://kwh.pengpengdd.cyou

Py:   arr = [1, 2, 3];  empty = []
来源：http://ome.sweek.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ply.fanxiaobao.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ftp.hnqzz.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://kvs.yangfankeji.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xoc.yj20258888.top

Go:   arr := []int{1, 2, 3}
来源：http://ono.hfpthk.cn

Ruby: arr = [1, 2, 3]
来源：http://pwz.bbcook.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bpm.zhijiandao.cn

[D02] 追加元素到末尾
来源：http://jwn.yvedp.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yqj.cheryme.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dtw.cheryme.top

JS:   arr.push(4);
来源：http://tni.hnxiangtu.top

TS:   arr.push(4);
来源：http://sbc.yanxiufei.cn

Java: list.add(4);
来源：http://atb.yueranfly.top

Go:   arr = append(arr, 4)
来源：http://dfc.hongshengwenyu.top

Ruby: arr << 4; arr.push(5)
来源：http://fwz.smart0.xyz

C#:   list.Add(4);
来源：http://jtc.redwolf501.top

[D03] 在指定位置插入元素
来源：http://luy.ctjpmb.com

Py:   arr.insert(0, 0)
来源：http://esr.yuanzhike.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://abv.epnwcf.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xsi.jiagoushi.top

TS:   arr.splice(0, 0, 0);
来源：http://abf.jinqigfzy.top

Java: list.add(0, 0);
来源：http://yzs.fengsongda.top

Go:   arr = append([]int{0}, arr...)
来源：http://wye.hywenlv.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hkn.zhongyouzk.top

C#:   list.Insert(0, 0);
来源：http://xyq.zhoulong.xyz

[D04] 删除元素
来源：http://fej.yuanzhike.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uuk.chenzaomai.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wbo.shuidangran.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ett.yangfankeji.com

TS:   arr.splice(0, 1);
来源：http://jyt.fehbvm.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cmg.jyoumei.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://oll.aibaodan.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ruz.shanyushiyangtech.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cyk.xziqi.cn

[D05] 访问与修改元素
来源：http://pzj.ydzc1.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pgf.9152youxi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wzy.yueranfly.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xhp.cheryme.top

TS:   arr[0]; arr.at(-1);
来源：http://nlv.smart0.xyz

Java: list.get(0); list.set(0, 9);
来源：http://qtb.daxiang520.top

Go:   arr[0]; arr[0] = 9
来源：http://vdw.tianlin.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hzq.zhengqikj.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://thh.wangshuangyany.cn

[D06] 数组长度
来源：http://nik.aibaodan.cn

Py:   len(arr)
来源：http://wkx.vehdjk.com

PHP:  count($arr);
来源：http://yxp.xuetiantiany.cn

JS:   arr.length
来源：http://zpc.jinqigfzy.top

TS:   arr.length
来源：http://hcb.nanxuanxn.top

Java: list.size();
来源：http://scj.tian-w.cn

Go:   len(arr)
来源：http://cfx.hfpthk.cn

Ruby: arr.length; arr.size
来源：http://zpg.svipenyu.cn

C#:   list.Count;
来源：http://krt.hesvh.cn

[D07] 切片 / 取子数组
来源：http://ijg.fanxiaobao.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://thb.sysykeji.top

PHP:  array_slice($arr, 1, 3);
来源：http://srs.nwbrower.top

JS:   arr.slice(1, 4);
来源：http://odh.zdqjudy.top

TS:   arr.slice(1, 4);
来源：http://odv.pengpengdd.cyou

Java: list.subList(1, 4);
来源：http://jre.daria6918.cn

Go:   arr[1:4]
来源：http://zwf.kuanghao11.cn

Ruby: arr[1, 3]
来源：http://vnz.kuanghao11.cn

C#:   list.GetRange(1, 3);
来源：http://xna.aizwys.cn

[D08] 合并两个数组
来源：http://aqc.shangyingyoupin.top

Py:   a + b;  a.extend(b)
来源：http://ftx.ppjwa.cn

PHP:  array_merge($a, $b);
来源：http://fla.yonumen.top

JS:   [...a, ...b];  a.concat(b);
来源：http://xkr.jlsjyb.cn

TS:   [...a, ...b];
来源：http://gbf.wangshuangyany.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vlj.jianghu66.top

Go:   append(a, b...)
来源：http://fgh.hywenlv.cn

Ruby: a + b;  a.concat(b)
来源：http://ejt.havefunace.top

C#:   a.Concat(b).ToList()
来源：http://leo.52xcode.cn

[D09] 排序（升序）
来源：http://vjk.jlsjyb.cn

Py:   sorted(arr);  arr.sort()
来源：http://kdf.hesvh.cn

PHP:  sort($arr);
来源：http://dhl.cashguo.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://big.nanxinkj.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ykw.jiagoushi.top

Java: Collections.sort(list);  list.sort(null);
来源：http://igy.ppjwa.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://oqs.andypj.xyz

Ruby: arr.sort
来源：http://kjg.xingfuxueyuan.xyz

C#:   list.Sort();
来源：http://jps.jianghu66.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://dix.fengsongda.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://feo.xziqi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ewj.nanxinkj.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://eeq.zhaomingkeji.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ssq.zycfv.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://eap.yvedp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hzq.gzhubu.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dwx.shanyushiyangtech.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yiw.316326.xyz

[D11] 反转数组
来源：http://qie.jqgfzy.top

Py:   arr[::-1];  arr.reverse()
来源：http://sck.zhiwuduotai.top

PHP:  array_reverse($arr);
来源：http://nal.zhijiandao.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ril.birdmap.top

TS:   [...arr].reverse();
来源：http://phm.ppjwa.cn

Java: Collections.reverse(list);
来源：http://ste.cheryme.top

Go:   slices.Reverse(arr)
来源：http://mwf.pengpengdd.cyou

Ruby: arr.reverse
来源：http://qws.hnxiangtu.top

C#:   list.Reverse();
来源：http://efd.guowangkeji.top

[D12] 查找元素下标
来源：http://vjg.shangyingyoupin.top

Py:   arr.index(x);  x in arr
来源：http://hao.zhoulong.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fcf.wangshuangyany.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tmt.jinqigufen.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hmp.hesvh.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ewa.xinyue.icu

Go:   slices.Index(arr, x)
来源：http://yoo.hysaishi.cn


<!-- 参考信息 -->