代发 wailian999

[B13] 判断是否为数字
来源：http://czb.jinghuilouyu.cn

Py:   isinstance(x, (int, float))
来源：http://ptt.cdnleiting.top

PHP:  is_numeric($x)
来源：http://ztc.zhongyouzk.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qty.zhengqikj.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vbt.tanke756.top

Java: x instanceof Number
来源：http://dwo.zdbjq.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hut.chenlongwang.top

Ruby: x.is_a?(Numeric)
来源：http://cai.xziqi.cn

C#:   x is int or double or decimal
来源：http://wyv.chenjidiqi.icu

[B14] 判断值是否在集合内
来源：http://bjo.ydjk.org.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dsx.tanke756.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cmt.xuanzx.com

JS:   [1, 2, 3].includes(x)
来源：http://vju.yangfankeji.com

TS:   [1, 2, 3].includes(x)
来源：http://job.sjlbkw.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://adq.xziqi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vyr.ydzc1.top

Ruby: [1, 2, 3].include?(x)
来源：http://cir.daxiang520.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uvf.ctjpmb.com

[B15] 布尔运算与取反
来源：http://lrt.yuanzhike.top

Py:   a and b or not c
来源：http://eca.zdbjq.cn

PHP:  $a && $b || !$c
来源：http://mrq.andypj.xyz

JS:   a && b || !c
来源：http://mip.xuanzx.com

TS:   a && b || !c
来源：http://rno.zhoulong.xyz

Java: a && b || !c
来源：http://icq.haohaochexian.top

Go:   a && b || !c
来源：http://awj.epnwcf.com

Ruby: a && b || !c
来源：http://ada.52xcode.cn

C#:   a && b || !c
来源：http://nxb.jqgufenzy.top

[B16] 卫语句：不满足条件提前返回
来源：http://cyr.feifeiyinyue.top

Py:   if not data: return
来源：http://myq.shangyingyoupin.top

PHP:  if (!$data) { return; }
来源：http://xla.redwolf501.top

JS:   if (!data) return;
来源：http://khn.tarul.cn

TS:   if (!data) return;
来源：http://vkp.yueranfly.top

Java: if (data == null) return;
来源：http://oii.dashuyun.cn

Go:   if data == nil { return }
来源：http://sfx.jinghuilouyu.cn

Ruby: return if data.nil?
来源：http://wgg.yuanzhike.top

C#:   if (data == null) return;
来源：http://fdh.bjfxy.top

================================================================================
来源：http://zcm.havefunace.top

C. 函数与作用域
来源：http://otc.yanxiufei.cn

================================================================================
来源：http://zle.guannengcc.top

[C01] 定义函数
来源：http://xbp.hcnkem.com

Py:   def add(a, b): return a + b
来源：http://zen.pengpengdd.cyou

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fcb.ivvv.top

JS:   function add(a, b) { return a + b; }
来源：http://vim.epnwcf.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rws.shanyushiyangtech.top

Java: static int add(int a, int b) { return a + b; }
来源：http://oya.zhengqikj.top

Go:   func add(a, b int) int { return a + b }
来源：http://kgx.fehbvm.com

Ruby: def add(a, b); a + b; end
来源：http://woo.chenlongwang.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ccp.xuetiantiany.cn

[C02] 默认参数
来源：http://coy.ctjpmb.com

Py:   def greet(name="World"): return name
来源：http://vqc.wangdashe.top

PHP:  function greet($name = "World") { return $name; }
来源：http://tft.cashguo.top

JS:   function greet(name = "World") { return name; }
来源：http://tsd.ehwqpu.com

TS:   function greet(name: string = "World") { return name; }
来源：http://wkb.shuidangran.top

Java: // 无默认参数：方法重载或 Optional
来源：http://bui.cucudq.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xft.bjfxy.top

Ruby: def greet(name = "World") = name
来源：http://qdm.xuetiantiany.cn

C#:   string Greet(string name = "World") => name;
来源：http://quw.tarul.cn

[C03] 可变参数
来源：http://hkf.zdbjq.cn

Py:   def total(*args): return sum(args)
来源：http://uyv.fktsv.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zip.hfpthk.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fje.zycfv.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cqs.quarkkingdee.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ikj.havefunace.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cyo.birdmap.top

Ruby: def total(*nums); nums.sum; end
来源：http://lnm.cdnleiting.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cna.aizwys.cn

[C04] 命名参数 / 关键字参数
来源：http://mnp.meibo888.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.jinqigfzy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://oss.yongpay.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bpv.jlsjyb.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://htt.ppjwa.cn

Java: // 无：用 Builder 模式或 record
来源：http://ceh.wangdashe.top

Go:   // 无：用配置结构体参数
来源：http://sqx.mhx1999.top

Ruby: f(a: 1, b: 2)
来源：http://zhp.sweek.top

C#:   f(a: 1, b: 2)
来源：http://uuv.yangfankeji.com

[C05] 返回多个值
来源：http://yup.zhongyouzk.top

Py:   return a, b
来源：http://vwm.yvedp.cn

PHP:  return [$a, $b];
来源：http://zrg.wangdashe.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://vnb.jqgfzy.top

TS:   return { a, b };
来源：http://lrh.wangshuangyany.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zcp.zdqjudy.top

Go:   return a, b
来源：http://lbh.aizwys.cn

Ruby: return a, b
来源：http://dqe.zdqjudy.top

C#:   return (a, b);              // ValueTuple
来源：http://kpv.hammf.cn

[C06] 匿名函数 / lambda
来源：http://aje.nanxuanxn.top

Py:   square = lambda x: x * x
来源：http://cgu.sufxvd.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://qau.yueranfly.top

JS:   const square = x => x * x;
来源：http://bgo.nanxinkj.top

TS:   const square = (x: number): number => x * x;
来源：http://zas.c1oappe.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ful.gaohongyu789.top

Go:   sq := func(x int) int { return x * x }
来源：http://nnz.hammf.cn

Ruby: square = ->(x) { x * x }
来源：http://grz.snrcjt.cn

C#:   Func<int, int> square = x => x * x;
来源：http://dkd.hywenlv.cn

[C07] 把函数作为参数传入
来源：http://hef.mhx1999.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://eae.cqqwz.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wnb.guannengcc.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hkq.hongshengwenyu.top

TS:   arr.map(String)
来源：http://ohp.zdbjq.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lfi.hywenlv.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qhq.yj202588.top

Ruby: arr.map(&:upcase)
来源：http://vkg.sufxvd.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ary.daxiang520.top

[C08] 闭包
来源：http://huc.shzxlz.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dhh.nanxinkj.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gcm.jlsjyb.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qzr.vehdjk.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fxc.hammf.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://udp.ctjpmb.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://eey.mhx1999.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jae.xuanzx.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tse.zhoulong.xyz

[C09] 递归
来源：http://elc.zhaomingkeji.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ywu.zhaomingkeji.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xsd.iojbl.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pjl.hysaishi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kqi.snrcjt.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mok.hfpthk.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ntk.tarul.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cmh.zhixingplan.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://umk.jinyuanbaomall.cn

[C10] 变量作用域
来源：http://tjw.sweek.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bla.yueranfly.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://aza.xuetiantiany.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bhl.xuanzx.com

TS:   同 JS
来源：http://gvv.smart0.xyz

Java: 方法内为块级作用域
来源：http://ukv.dashuyun.cn

Go:   花括号块级作用域
来源：http://gpk.sweek.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uci.chenzaomai.com

C#:   块级作用域
来源：http://xbe.haohaochexian.top

[C11] 模块导入与导出
来源：http://cbs.yangfankeji.com

Py:   from module import func
来源：http://lbz.zhijiandao.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://frf.tian-w.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://aet.ydzc1.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sln.vqdsnc.cn

Java: import java.util.List;
来源：http://phr.0kj1m.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hti.pycfn.com

Ruby: require "json"; require_relative "./util"
来源：http://txl.bjfxy.top

C#:   using System.Text;
来源：http://gps.jianghu66.top

[C12] 立即执行函数 IIFE
来源：http://rur.cqqwz.cn

Py:   (lambda: print("run"))()
来源：http://jpd.zhoulong.xyz

PHP:  (function () { echo "run"; })();
来源：http://esh.gzhubu.top

JS:   (() => { console.log("run"); })();
来源：http://nrm.gzhubu.top

TS:   (() => { console.log("run"); })();
来源：http://cak.zhiwuduotai.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xkv.yanxiufei.cn

Go:   func() { fmt.Println("run") }()
来源：http://ipl.tanke756.top

Ruby: -> { puts "run" }.call
来源：http://qzd.xinyue.icu

C#:   // 无 IIFE：用静态构造函数
来源：http://jge.yuanzhike.top

[C13] 类型声明 / 类型注解
来源：http://bsh.zhaomingkeji.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bje.zhiwuduotai.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kmp.fengsongda.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vrq.wangdashe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rbx.gaohongyu789.top

Java: int add(int a, int b) { return a + b; }
来源：http://rjl.yvedp.cn

Go:   func add(a, b int) int
来源：http://bcv.yongpay.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mkh.hesvh.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vbn.dashuyun.cn

[C14] 泛型函数
来源：http://yao.zhiwuduotai.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kpt.shanyushiyangtech.top

PHP:  // 无泛型
来源：http://dyi.sxryk.cn

JS:   // 无泛型
来源：http://rnj.hfpthk.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xyc.epnwcf.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hbs.zhaomingkeji.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vhd.shangyingyoupin.top

Ruby: # 无泛型
来源：http://ztu.yuanzhike.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tjm.jqgfzy.top

[C15] 解构 / 展开参数
来源：http://ulb.shzxlz.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ukm.chenlongwang.top

PHP:  [$a, $b] = $pair;
来源：http://acp.sysykeji.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://syt.yongpay.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vyi.feifeiyinyue.top

Java: // 无解构
来源：http://prc.svipenyu.cn

Go:   // 无解构
来源：http://xql.ppjwa.cn

Ruby: a, b = pair
来源：http://olp.jinyuanbaomall.cn

C#:   var (a, b) = pair;
来源：http://gnq.vehdjk.com

[C16] 函数 / 方法重载
来源：http://vmd.0kj1m.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://deg.bjfxy.top

PHP:  // 无重载
来源：http://huk.ehwqpu.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://bvj.chenlongwang.top

TS:   // 用联合类型或重载签名声明
来源：http://dxp.wangshuangyany.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hty.zhiwuduotai.top

Go:   // 无重载：用不同函数名
来源：http://dma.bbcook.cn

Ruby: # 无重载：靠动态参数
来源：http://mdt.ivvv.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://kjn.ehwqpu.com

================================================================================
来源：http://btj.daxiang520.top

D. 数组 / 列表 / 集合
来源：http://mbs.ivvv.top

================================================================================
来源：http://wrs.hnxiangtu.top

[D01] 创建数组 / 列表
来源：http://xym.tanke756.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ups.yangfankeji.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jrg.gotoacloud.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://evl.haohaochexian.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://lnh.zhixingplan.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jcb.zhixingplan.top

Go:   arr := []int{1, 2, 3}
来源：http://zpo.sufxvd.cn

Ruby: arr = [1, 2, 3]
来源：http://eqr.zdbjq.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ciy.haohaochexian.top

[D02] 追加元素到末尾
来源：http://jfv.xingfuxueyuan.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://byr.fengsongda.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ebh.nanxuanxn.top

JS:   arr.push(4);
来源：http://gvo.haohaochexian.top

TS:   arr.push(4);
来源：http://ilu.tianlin.xyz

Java: list.add(4);
来源：http://hpm.jlsjyb.cn

Go:   arr = append(arr, 4)
来源：http://csk.yj20258888.top

Ruby: arr << 4; arr.push(5)
来源：http://idi.ivvv.top

C#:   list.Add(4);
来源：http://caq.fzhhl.top

[D03] 在指定位置插入元素
来源：http://jfv.daxiang520.top

Py:   arr.insert(0, 0)
来源：http://dfb.wangdashe.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ozz.ydjk.org.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qag.hnxiangtu.top

TS:   arr.splice(0, 0, 0);
来源：http://ola.wangshuangyany.cn

Java: list.add(0, 0);
来源：http://wyg.chenjidiqi.icu

Go:   arr = append([]int{0}, arr...)
来源：http://kcx.uphjek.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ngf.ywan-chungtsiang.top

C#:   list.Insert(0, 0);
来源：http://abc.andypj.xyz

[D04] 删除元素
来源：http://tlz.jinqigufen.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wqt.ydjk.org.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fxb.vqdsnc.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ojj.mhx1999.top

TS:   arr.splice(0, 1);
来源：http://kjf.zhaomingkeji.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zvp.cdnleiting.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ejx.nwbrower.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hvh.ywan-chungtsiang.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://onc.nanxuanxn.top

[D05] 访问与修改元素
来源：http://lgd.andypj.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bqe.yonumen.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nuz.zhiwuduotai.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bvr.kuanghao11.cn

TS:   arr[0]; arr.at(-1);
来源：http://ljv.cashguo.top

Java: list.get(0); list.set(0, 9);
来源：http://ikj.jinqigfzy.top

Go:   arr[0]; arr[0] = 9
来源：http://atj.aizwys.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hqo.ctjpmb.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ega.zhongyouzk.top

[D06] 数组长度
来源：http://rzu.jiagoushi.top

Py:   len(arr)
来源：http://wvo.snrcjt.cn

PHP:  count($arr);
来源：http://udk.zhongyouzk.top

JS:   arr.length
来源：http://ejk.yj202588.top

TS:   arr.length
来源：http://wyf.ctjpmb.com

Java: list.size();
来源：http://fmk.yuxming.cn

Go:   len(arr)
来源：http://fro.jinyuanbaomall.cn

Ruby: arr.length; arr.size
来源：http://ujh.yongpay.top

C#:   list.Count;
来源：http://ddp.sweek.top

[D07] 切片 / 取子数组
来源：http://vfw.birdmap.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://uqj.ydzc1.top

PHP:  array_slice($arr, 1, 3);
来源：http://lds.zhiwuduotai.top

JS:   arr.slice(1, 4);
来源：http://evv.hysaishi.cn

TS:   arr.slice(1, 4);
来源：http://bod.iojbl.cn

Java: list.subList(1, 4);
来源：http://roj.jinqigfzy.top

Go:   arr[1:4]
来源：http://xbm.hywenlv.cn

Ruby: arr[1, 3]
来源：http://cxk.zdbjq.cn

C#:   list.GetRange(1, 3);
来源：http://yim.yueranfly.top

[D08] 合并两个数组
来源：http://oti.uphjek.com

Py:   a + b;  a.extend(b)
来源：http://oen.smart0.xyz

PHP:  array_merge($a, $b);
来源：http://ejk.sysykeji.top

JS:   [...a, ...b];  a.concat(b);
来源：http://civ.bjfxy.top

TS:   [...a, ...b];
来源：http://ali.svipenyu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bce.shzxlz.cn

Go:   append(a, b...)
来源：http://mpv.sweek.top

Ruby: a + b;  a.concat(b)
来源：http://jml.fzhhl.top

C#:   a.Concat(b).ToList()
来源：http://ygp.vqdsnc.cn

[D09] 排序（升序）
来源：http://dor.wangshuangyany.cn

Py:   sorted(arr);  arr.sort()
来源：http://vzs.guannengcc.top

PHP:  sort($arr);
来源：http://plt.yj202588.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nem.birdmap.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://kth.daxiang520.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ija.ctjpmb.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://khl.fzhhl.top

Ruby: arr.sort
来源：http://eoc.zhixingplan.top

C#:   list.Sort();
来源：http://cnx.ybcxt.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://jtp.hywenlv.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lrd.zhoulong.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xfk.bjfxy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tly.tian-w.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mde.tianlin.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dzt.mhx1999.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xyx.jiagoushi.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://iwc.guannengcc.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nlf.hnxiangtu.top

[D11] 反转数组
来源：http://syz.shangyingyoupin.top

Py:   arr[::-1];  arr.reverse()
来源：http://kuo.9152youxi.cn

PHP:  array_reverse($arr);
来源：http://fvi.jinyuanbaomall.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ysv.hysaishi.cn

TS:   [...arr].reverse();
来源：http://qdj.mhx1999.top

Java: Collections.reverse(list);
来源：http://sgu.jinqigufen.top

Go:   slices.Reverse(arr)
来源：http://due.hesvh.cn

Ruby: arr.reverse
来源：http://lfe.aizwys.cn

C#:   list.Reverse();
来源：http://fpj.sufxvd.cn

[D12] 查找元素下标
来源：http://kdw.kuanghao11.cn

Py:   arr.index(x);  x in arr
来源：http://kyn.tianlin.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nhb.shanyushiyangkeji.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rcz.ywan-chungtsiang.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xpo.jinqigfzy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mpz.xinyue.icu

Go:   slices.Index(arr, x)
来源：http://dyo.cheryme.top

Ruby: arr.index(x)
来源：http://jjs.nanxuanxn.top

C#:   list.IndexOf(x);
来源：http://doh.shangyingyoupin.top

[D13] 过滤（保留满足条件的）
来源：http://mdn.aizwys.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://knm.birdmap.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://msi.jqgfzy.top

JS:   arr.filter(x => x > 3)
来源：http://oei.shanyushiyangkeji.top

TS:   arr.filter(x => x > 3)
来源：http://ipp.ywan-chungtsiang.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fto.yanxiufei.cn


<!-- 参考信息 -->