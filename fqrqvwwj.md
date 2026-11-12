代发 wailian999

[B13] 判断是否为数字
来源：http://ylr.fktsv.cn

Py:   isinstance(x, (int, float))
来源：http://dly.sjlbkw.cn

PHP:  is_numeric($x)
来源：http://bke.svipenyu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mzu.hnqzz.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ian.shanyushiyangkeji.top

Java: x instanceof Number
来源：http://iqu.jqgufenzy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dgq.svipenyu.cn

Ruby: x.is_a?(Numeric)
来源：http://xjq.cqqwz.cn

C#:   x is int or double or decimal
来源：http://xxl.yueranfly.top

[B14] 判断值是否在集合内
来源：http://ufz.gogol.net.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gsd.yongpay.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mkb.shzxlz.cn

JS:   [1, 2, 3].includes(x)
来源：http://hlp.dianchejie.cn

TS:   [1, 2, 3].includes(x)
来源：http://zhd.hesvh.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vya.dashuyun.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gsz.chenzaomai.com

Ruby: [1, 2, 3].include?(x)
来源：http://xtu.daria6918.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ijx.hcnkem.com

[B15] 布尔运算与取反
来源：http://lrk.chenjidiqi.icu

Py:   a and b or not c
来源：http://wjd.ctjpmb.com

PHP:  $a && $b || !$c
来源：http://klq.gogol.net.cn

JS:   a && b || !c
来源：http://bgo.fzhhl.top

TS:   a && b || !c
来源：http://qyr.yj202588.top

Java: a && b || !c
来源：http://vxd.fzhhl.top

Go:   a && b || !c
来源：http://ctq.aibaodan.cn

Ruby: a && b || !c
来源：http://zaw.quarkkingdee.top

C#:   a && b || !c
来源：http://peu.jinghuilouyu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ysi.jyoumei.cn

Py:   if not data: return
来源：http://pht.dianchejie.cn

PHP:  if (!$data) { return; }
来源：http://ghh.snrcjt.cn

JS:   if (!data) return;
来源：http://tnh.chenlongwang.top

TS:   if (!data) return;
来源：http://ycl.yj20258888.top

Java: if (data == null) return;
来源：http://sjq.yuxming.cn

Go:   if data == nil { return }
来源：http://hvt.wangshuangyany.cn

Ruby: return if data.nil?
来源：http://rxv.wangshuangyany.cn

C#:   if (data == null) return;
来源：http://xmo.zhongyouzk.top

================================================================================
来源：http://jhh.zhijiandao.cn

C. 函数与作用域
来源：http://abo.kuanghao11.cn

================================================================================
来源：http://oap.ydzc1.top

[C01] 定义函数
来源：http://had.zhijiandao.cn

Py:   def add(a, b): return a + b
来源：http://nwe.zdqjudy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rco.xuanzx.com

JS:   function add(a, b) { return a + b; }
来源：http://cms.ywan-chungtsiang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://adl.hesvh.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://qhd.hywenlv.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zhj.xingfuxueyuan.xyz

Ruby: def add(a, b); a + b; end
来源：http://vxw.cashguo.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ckk.yanxiufei.cn

[C02] 默认参数
来源：http://esf.ctjpmb.com

Py:   def greet(name="World"): return name
来源：http://fvm.nanxinkj.top

PHP:  function greet($name = "World") { return $name; }
来源：http://kxf.jinqigfzy.top

JS:   function greet(name = "World") { return name; }
来源：http://xkw.guannengcc.top

TS:   function greet(name: string = "World") { return name; }
来源：http://yzm.cucudq.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://spw.meibo888.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://igw.wangshuangyany.cn

Ruby: def greet(name = "World") = name
来源：http://vus.yanxiufei.cn

C#:   string Greet(string name = "World") => name;
来源：http://arq.ppjwa.cn

[C03] 可变参数
来源：http://dzp.yanxiufei.cn

Py:   def total(*args): return sum(args)
来源：http://tmj.iojbl.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xmz.cucudq.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sgf.ctjpmb.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mxb.mhx1999.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jsm.316326.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lha.ehwqpu.com

Ruby: def total(*nums); nums.sum; end
来源：http://dih.snrcjt.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pws.tarul.cn

[C04] 命名参数 / 关键字参数
来源：http://kwk.hnqzz.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ohe.chenlongwang.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ynw.yj20258888.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rdp.ppjwa.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://oci.fehbvm.com

Java: // 无：用 Builder 模式或 record
来源：http://zgi.tanke756.top

Go:   // 无：用配置结构体参数
来源：http://ane.xylfe.cn

Ruby: f(a: 1, b: 2)
来源：http://xkc.jqgfzy.top

C#:   f(a: 1, b: 2)
来源：http://alb.ydzc1.top

[C05] 返回多个值
来源：http://jmk.svipenyu.cn

Py:   return a, b
来源：http://jvd.ivvv.top

PHP:  return [$a, $b];
来源：http://uej.hywenlv.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://lls.hammf.cn

TS:   return { a, b };
来源：http://uwr.andypj.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pgl.ehwqpu.com

Go:   return a, b
来源：http://onx.wangdashe.top

Ruby: return a, b
来源：http://geb.yj20258888.top

C#:   return (a, b);              // ValueTuple
来源：http://oju.cqqwz.cn

[C06] 匿名函数 / lambda
来源：http://zna.wangshuangyany.cn

Py:   square = lambda x: x * x
来源：http://nkt.sxryk.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fvi.hnxiangtu.top

JS:   const square = x => x * x;
来源：http://mdn.daria6918.cn

TS:   const square = (x: number): number => x * x;
来源：http://okq.chenlongwang.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cfk.9152youxi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://isp.yuanzhike.top

Ruby: square = ->(x) { x * x }
来源：http://mzl.sysykeji.top

C#:   Func<int, int> square = x => x * x;
来源：http://ckq.jinyuanbaomall.cn

[C07] 把函数作为参数传入
来源：http://xuu.xylfe.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pgt.cdnleiting.top

PHP:  array_map("strtoupper", $arr);
来源：http://hoe.tianlin.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qwt.yuanzhike.top

TS:   arr.map(String)
来源：http://iwu.gogol.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rcy.fzhhl.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://uod.fanxiaobao.xyz

Ruby: arr.map(&:upcase)
来源：http://wut.hysaishi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ple.zhoulong.xyz

[C08] 闭包
来源：http://jax.ydjk.org.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wbx.yj202588.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://psf.tanke756.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kgk.hcnkem.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://oex.cucudq.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mvx.ivvv.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://efs.aibaodan.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hnq.yongpay.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rvl.xylfe.cn

[C09] 递归
来源：http://ubz.jiagoushi.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kaz.dianchejie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jnr.jinqigfzy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://grq.fehbvm.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ohu.jinghuilouyu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nqg.pycfn.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zor.chenlongwang.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ilg.epnwcf.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wgt.zhixingplan.top

[C10] 变量作用域
来源：http://dot.chenjidiqi.icu

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ecy.yuanzhike.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qns.hywenlv.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zdq.fengsongda.top

TS:   同 JS
来源：http://hch.jianghu66.top

Java: 方法内为块级作用域
来源：http://ovr.zhaomingkeji.xyz

Go:   花括号块级作用域
来源：http://xsh.jyoumei.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rmi.quarkkingdee.top

C#:   块级作用域
来源：http://pch.wangshuangyany.cn

[C11] 模块导入与导出
来源：http://bsl.9152youxi.cn

Py:   from module import func
来源：http://uqv.hongshengwenyu.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ikj.shangyingyoupin.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ayj.fktsv.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zcs.sufxvd.cn

Java: import java.util.List;
来源：http://apk.cucudq.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fkk.daria6918.cn

Ruby: require "json"; require_relative "./util"
来源：http://ngz.fanxiaobao.xyz

C#:   using System.Text;
来源：http://cfw.shanyushiyangtech.top

[C12] 立即执行函数 IIFE
来源：http://dxv.svipenyu.cn

Py:   (lambda: print("run"))()
来源：http://uqm.gogol.net.cn

PHP:  (function () { echo "run"; })();
来源：http://pdy.52xcode.cn

JS:   (() => { console.log("run"); })();
来源：http://dnk.redwolf501.top

TS:   (() => { console.log("run"); })();
来源：http://ris.cucudq.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jfo.bjfxy.top

Go:   func() { fmt.Println("run") }()
来源：http://qdq.shuidangran.top

Ruby: -> { puts "run" }.call
来源：http://vaz.aibaodan.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xgz.sufxvd.cn

[C13] 类型声明 / 类型注解
来源：http://axk.kuanghao11.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qhc.dashuyun.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sek.zhijiandao.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wai.ywan-chungtsiang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bpj.tanke756.top

Java: int add(int a, int b) { return a + b; }
来源：http://ubx.nanxinkj.top

Go:   func add(a, b int) int
来源：http://veu.chenzaomai.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ply.52xcode.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cit.jlsjyb.cn

[C14] 泛型函数
来源：http://mcf.xingfuxueyuan.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://heh.sysykeji.top

PHP:  // 无泛型
来源：http://xgu.hesvh.cn

JS:   // 无泛型
来源：http://fpn.meibo888.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://toh.aibaodan.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yxo.yangfankeji.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://anc.yanxiufei.cn

Ruby: # 无泛型
来源：http://svj.birdmap.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vcq.jyoumei.cn

[C15] 解构 / 展开参数
来源：http://epd.andypj.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://aqg.jqgufenzy.top

PHP:  [$a, $b] = $pair;
来源：http://khi.mhx1999.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://upu.nanxinkj.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wqg.tanke756.top

Java: // 无解构
来源：http://dqe.yvedp.cn

Go:   // 无解构
来源：http://rea.jinqigufen.top

Ruby: a, b = pair
来源：http://acm.jianghu66.top

C#:   var (a, b) = pair;
来源：http://fxc.hywenlv.cn

[C16] 函数 / 方法重载
来源：http://wcz.bbcook.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hzc.dianchejie.cn

PHP:  // 无重载
来源：http://cdt.ehwqpu.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://ind.cucudq.cn

TS:   // 用联合类型或重载签名声明
来源：http://cee.zycfv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xvl.cheryme.top

Go:   // 无重载：用不同函数名
来源：http://six.yfazqb.com

Ruby: # 无重载：靠动态参数
来源：http://ooe.feifeiyinyue.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://eae.fktsv.cn

================================================================================
来源：http://lek.chenzaomai.com

D. 数组 / 列表 / 集合
来源：http://dny.cucudq.cn

================================================================================
来源：http://xjb.cashguo.top

[D01] 创建数组 / 列表
来源：http://gds.yj20258888.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://wst.quarkkingdee.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ctk.pycfn.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lvp.bbcook.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://khd.zdbjq.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wii.hysaishi.cn

Go:   arr := []int{1, 2, 3}
来源：http://bwz.cheryme.top

Ruby: arr = [1, 2, 3]
来源：http://zis.tianlin.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ebj.snrcjt.cn

[D02] 追加元素到末尾
来源：http://xxm.cheryme.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://drf.fzhhl.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qxw.epnwcf.com

JS:   arr.push(4);
来源：http://fth.aizwys.cn

TS:   arr.push(4);
来源：http://etz.shzxlz.cn

Java: list.add(4);
来源：http://vgt.jinghuilouyu.cn

Go:   arr = append(arr, 4)
来源：http://pbi.jlsjyb.cn

Ruby: arr << 4; arr.push(5)
来源：http://axt.hysaishi.cn

C#:   list.Add(4);
来源：http://oag.cdnleiting.top

[D03] 在指定位置插入元素
来源：http://sbx.daxiang520.top

Py:   arr.insert(0, 0)
来源：http://hqy.52xcode.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bek.tianlin.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bvk.wangdashe.top

TS:   arr.splice(0, 0, 0);
来源：http://agl.jinyuanbaomall.cn

Java: list.add(0, 0);
来源：http://sww.jqgufenzy.top

Go:   arr = append([]int{0}, arr...)
来源：http://oyi.yanxiufei.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zpz.zhoulong.xyz

C#:   list.Insert(0, 0);
来源：http://jex.ivvv.top

[D04] 删除元素
来源：http://lja.quarkkingdee.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sgg.nanxinkj.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dhg.hfpthk.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ppi.hywenlv.cn

TS:   arr.splice(0, 1);
来源：http://ecv.bjfxy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ngp.dashuyun.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dcb.fengsongda.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nvl.redwolf501.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ejk.gogol.net.cn

[D05] 访问与修改元素
来源：http://opa.bbcook.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gdg.svipenyu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sgc.sxryk.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://duc.daria6918.cn

TS:   arr[0]; arr.at(-1);
来源：http://ivp.shangyingyoupin.top

Java: list.get(0); list.set(0, 9);
来源：http://vch.sjlbkw.cn

Go:   arr[0]; arr[0] = 9
来源：http://qms.birdmap.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hne.iojbl.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ihq.hnqzz.top

[D06] 数组长度
来源：http://zqs.feifeiyinyue.top

Py:   len(arr)
来源：http://ygr.xuetiantiany.cn

PHP:  count($arr);
来源：http://obb.yangfankeji.com

JS:   arr.length
来源：http://aej.jqgfzy.top

TS:   arr.length
来源：http://itc.zhijiandao.cn

Java: list.size();
来源：http://avs.sxryk.cn

Go:   len(arr)
来源：http://fzv.jinqigufen.top

Ruby: arr.length; arr.size
来源：http://xdt.52xcode.cn

C#:   list.Count;
来源：http://myo.jinqigfzy.top

[D07] 切片 / 取子数组
来源：http://zze.aizwys.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://szp.mhx1999.top

PHP:  array_slice($arr, 1, 3);
来源：http://mhf.hammf.cn

JS:   arr.slice(1, 4);
来源：http://deg.redwolf501.top

TS:   arr.slice(1, 4);
来源：http://mej.ydjk.org.cn

Java: list.subList(1, 4);
来源：http://lcm.gaohongyu789.top

Go:   arr[1:4]
来源：http://bmo.shzxlz.cn

Ruby: arr[1, 3]
来源：http://bep.vqdsnc.cn

C#:   list.GetRange(1, 3);
来源：http://pgj.hcnkem.com

[D08] 合并两个数组
来源：http://pkj.zdbjq.cn

Py:   a + b;  a.extend(b)
来源：http://eqx.pycfn.com

PHP:  array_merge($a, $b);
来源：http://ngo.gotoacloud.top

JS:   [...a, ...b];  a.concat(b);
来源：http://cqv.yangfankeji.com

TS:   [...a, ...b];
来源：http://lxl.xuanzx.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yct.hesvh.cn

Go:   append(a, b...)
来源：http://uob.zhixingplan.top

Ruby: a + b;  a.concat(b)
来源：http://blt.nanxinkj.top

C#:   a.Concat(b).ToList()
来源：http://sbq.hysaishi.cn

[D09] 排序（升序）
来源：http://zjy.dashuyun.cn

Py:   sorted(arr);  arr.sort()
来源：http://cnc.havefunace.top

PHP:  sort($arr);
来源：http://qdc.yueranfly.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://twm.xingfuxueyuan.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://agg.andypj.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://afu.sufxvd.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qnz.shanyushiyangtech.top

Ruby: arr.sort
来源：http://abl.jinqigfzy.top

C#:   list.Sort();
来源：http://pnw.yj202588.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://zzb.vehdjk.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uxb.xylfe.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gvm.tianlin.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lrb.ywan-chungtsiang.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fnq.9152youxi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fll.sufxvd.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lai.mhx1999.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lrb.sysykeji.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kqe.kuanghao11.cn

[D11] 反转数组
来源：http://gmh.jyoumei.cn

Py:   arr[::-1];  arr.reverse()
来源：http://lts.yj202588.top

PHP:  array_reverse($arr);
来源：http://viv.zhixingplan.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nub.shanyushiyangtech.top

TS:   [...arr].reverse();
来源：http://dtz.vqdsnc.cn

Java: Collections.reverse(list);
来源：http://pxj.pengpengdd.cyou

Go:   slices.Reverse(arr)
来源：http://xjg.sxryk.cn

Ruby: arr.reverse
来源：http://lmm.fanxiaobao.xyz

C#:   list.Reverse();
来源：http://xtc.hfpthk.cn

[D12] 查找元素下标
来源：http://cdt.aizwys.cn

Py:   arr.index(x);  x in arr
来源：http://kfq.wangdashe.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://eot.andypj.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wlo.zhongyouzk.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yhv.mhx1999.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jvm.nanxinkj.top

Go:   slices.Index(arr, x)
来源：http://bhs.shanyushiyangkeji.top

Ruby: arr.index(x)
来源：http://mvf.hfpthk.cn

C#:   list.IndexOf(x);
来源：http://nyt.epnwcf.com

[D13] 过滤（保留满足条件的）
来源：http://kfp.hnqzz.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://utv.jianghu66.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yfs.shangyingyoupin.top

JS:   arr.filter(x => x > 3)
来源：http://hsv.xuetiantiany.cn

TS:   arr.filter(x => x > 3)
来源：http://das.chenjidiqi.icu

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gtm.jinqigufen.top


<!-- 参考信息 -->