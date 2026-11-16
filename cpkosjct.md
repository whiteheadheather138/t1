代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://zny.zhaomingkeji.xyz

TS:   [1, 2, 3].includes(x)
来源：http://yif.pycfn.com

Java: List.of(1, 2, 3).contains(x)
来源：http://brh.daria6918.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://oqg.gzhubu.top

Ruby: [1, 2, 3].include?(x)
来源：http://tlw.zhongyouzk.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://riz.yj20258888.top

[B15] 布尔运算与取反
来源：http://pvo.pengpengdd.cyou

Py:   a and b or not c
来源：http://wlo.shzxlz.cn

PHP:  $a && $b || !$c
来源：http://ysc.zhaomingkeji.xyz

JS:   a && b || !c
来源：http://wta.xuetiantiany.cn

TS:   a && b || !c
来源：http://znu.smart0.xyz

Java: a && b || !c
来源：http://vvn.hongshengwenyu.top

Go:   a && b || !c
来源：http://wct.redwolf501.top

Ruby: a && b || !c
来源：http://ccb.pycfn.com

C#:   a && b || !c
来源：http://bzq.guowangkeji.top

[B16] 卫语句：不满足条件提前返回
来源：http://isd.fehbvm.com

Py:   if not data: return
来源：http://pof.quarkkingdee.top

PHP:  if (!$data) { return; }
来源：http://ics.sjlbkw.cn

JS:   if (!data) return;
来源：http://ndt.fzhhl.top

TS:   if (!data) return;
来源：http://dsx.hcnkem.com

Java: if (data == null) return;
来源：http://ksz.hongshengwenyu.top

Go:   if data == nil { return }
来源：http://pjn.uphjek.com

Ruby: return if data.nil?
来源：http://trp.daxiang520.top

C#:   if (data == null) return;
来源：http://buj.aizwys.cn

================================================================================
来源：http://twr.jqgfzy.top

C. 函数与作用域
来源：http://soo.yj20258.top

================================================================================
来源：http://whi.hywenlv.cn

[C01] 定义函数
来源：http://qwk.zhiwuduotai.top

Py:   def add(a, b): return a + b
来源：http://bau.mhx1999.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eic.fzhhl.top

JS:   function add(a, b) { return a + b; }
来源：http://rqj.sufxvd.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rhr.fzhhl.top

Java: static int add(int a, int b) { return a + b; }
来源：http://hju.haohaochexian.top

Go:   func add(a, b int) int { return a + b }
来源：http://qau.tanke756.top

Ruby: def add(a, b); a + b; end
来源：http://paw.meibo888.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://axk.hnxiangtu.top

[C02] 默认参数
来源：http://ldg.yonumen.top

Py:   def greet(name="World"): return name
来源：http://udu.wangdashe.top

PHP:  function greet($name = "World") { return $name; }
来源：http://knv.yangfankeji.com

JS:   function greet(name = "World") { return name; }
来源：http://qcz.aibaodan.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://cag.9152youxi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vaw.tarul.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://efd.guowangkeji.top

Ruby: def greet(name = "World") = name
来源：http://xeo.gotoacloud.top

C#:   string Greet(string name = "World") => name;
来源：http://nsz.jinghuilouyu.cn

[C03] 可变参数
来源：http://xgl.haohaochexian.top

Py:   def total(*args): return sum(args)
来源：http://saa.dashuyun.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fdg.shanyushiyangtech.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zgw.havefunace.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yeb.jinghuilouyu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lwe.hysaishi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ypw.yueranfly.top

Ruby: def total(*nums); nums.sum; end
来源：http://orl.pengpengdd.cyou

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vsz.andypj.xyz

[C04] 命名参数 / 关键字参数
来源：http://skg.9152youxi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://umf.zycfv.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dyy.gaohongyu789.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://icb.shzxlz.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zvi.xuetiantiany.cn

Java: // 无：用 Builder 模式或 record
来源：http://eac.yanxiufei.cn

Go:   // 无：用配置结构体参数
来源：http://jjl.chenjidiqi.icu

Ruby: f(a: 1, b: 2)
来源：http://yae.vqdsnc.cn

C#:   f(a: 1, b: 2)
来源：http://yrj.c1oappe.top

[C05] 返回多个值
来源：http://kfu.fzhhl.top

Py:   return a, b
来源：http://dss.hnqzz.top

PHP:  return [$a, $b];
来源：http://smn.ybcxt.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://xst.dianchejie.cn

TS:   return { a, b };
来源：http://fkn.xuanzx.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://euc.shzxlz.cn

Go:   return a, b
来源：http://ubs.jyoumei.cn

Ruby: return a, b
来源：http://cbw.shangyingyoupin.top

C#:   return (a, b);              // ValueTuple
来源：http://bgg.shangyingyoupin.top

[C06] 匿名函数 / lambda
来源：http://nny.fktsv.cn

Py:   square = lambda x: x * x
来源：http://ycw.tanke756.top

PHP:  $square = fn($x) => $x * $x;
来源：http://pim.c1oappe.top

JS:   const square = x => x * x;
来源：http://nur.pengpengdd.cyou

TS:   const square = (x: number): number => x * x;
来源：http://hjh.snrcjt.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cma.xylfe.cn

Go:   sq := func(x int) int { return x * x }
来源：http://tls.daxiang520.top

Ruby: square = ->(x) { x * x }
来源：http://ftz.yonumen.top

C#:   Func<int, int> square = x => x * x;
来源：http://chw.quarkkingdee.top

[C07] 把函数作为参数传入
来源：http://fih.fanxiaobao.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tvq.fzhhl.top

PHP:  array_map("strtoupper", $arr);
来源：http://pdl.zhoulong.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ecx.sjlbkw.cn

TS:   arr.map(String)
来源：http://jkx.yj20258888.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fbf.tianlin.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hmb.wangdashe.top

Ruby: arr.map(&:upcase)
来源：http://amk.fengsongda.top

C#:   arr.Select(s => s.ToUpper())
来源：http://adv.yongpay.top

[C08] 闭包
来源：http://byl.zhaomingkeji.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yax.jinyuanbaomall.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cln.ppjwa.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://eca.xuanzx.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xal.daria6918.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dws.aibaodan.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cny.zhoulong.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yyy.dashuyun.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://keh.jianghu66.top

[C09] 递归
来源：http://iqh.gogol.net.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ihn.jianghu66.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://obl.zhijiandao.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://snz.ctjpmb.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wua.zhongyouzk.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fgx.havefunace.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ssz.jyoumei.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jpg.daxiang520.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cac.zhongyouzk.top

[C10] 变量作用域
来源：http://mjw.52xcode.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fqh.shanyushiyangtech.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vyo.hcnkem.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dcr.guowangkeji.top

TS:   同 JS
来源：http://ljr.hnqzz.top

Java: 方法内为块级作用域
来源：http://ghd.zhiwuduotai.top

Go:   花括号块级作用域
来源：http://fyu.ivvv.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bcc.sysykeji.top

C#:   块级作用域
来源：http://xbe.shzxlz.cn

[C11] 模块导入与导出
来源：http://gvi.fengsongda.top

Py:   from module import func
来源：http://tkq.vqdsnc.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://scw.yj202588.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://udu.yonumen.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hal.vehdjk.com

Java: import java.util.List;
来源：http://cqs.hysaishi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://uic.tarul.cn

Ruby: require "json"; require_relative "./util"
来源：http://cfk.zhixingplan.top

C#:   using System.Text;
来源：http://gjf.zhaomingkeji.xyz

[C12] 立即执行函数 IIFE
来源：http://fry.jlsjyb.cn

Py:   (lambda: print("run"))()
来源：http://ggs.sysykeji.top

PHP:  (function () { echo "run"; })();
来源：http://ktb.dianchejie.cn

JS:   (() => { console.log("run"); })();
来源：http://kje.9152youxi.cn

TS:   (() => { console.log("run"); })();
来源：http://hpo.hcnkem.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kip.nanxinkj.top

Go:   func() { fmt.Println("run") }()
来源：http://urd.fzhhl.top

Ruby: -> { puts "run" }.call
来源：http://rjp.zdqjudy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://wln.zhiwuduotai.top

[C13] 类型声明 / 类型注解
来源：http://heo.havefunace.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dfw.smart0.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lkt.aibaodan.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hzl.nanxinkj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xth.zhoulong.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://faq.shangyingyoupin.top

Go:   func add(a, b int) int
来源：http://tej.jqgfzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ngw.wangdashe.top

C#:   int Add(int a, int b) => a + b;
来源：http://zkm.jlsjyb.cn

[C14] 泛型函数
来源：http://ggf.zhiwuduotai.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dqd.xinyue.icu

PHP:  // 无泛型
来源：http://zbi.jiagoushi.top

JS:   // 无泛型
来源：http://wgv.yj20258888.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vif.jinqigufen.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zzt.hongshengwenyu.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zbm.birdmap.top

Ruby: # 无泛型
来源：http://slu.vehdjk.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tij.xuetiantiany.cn

[C15] 解构 / 展开参数
来源：http://lkr.yuanzhike.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://htn.bbcook.cn

PHP:  [$a, $b] = $pair;
来源：http://psv.guowangkeji.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xaz.316326.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hth.yj202588.top

Java: // 无解构
来源：http://bdo.jiagoushi.top

Go:   // 无解构
来源：http://frp.hysaishi.cn

Ruby: a, b = pair
来源：http://hiv.ywan-chungtsiang.top

C#:   var (a, b) = pair;
来源：http://svc.yj20258.top

[C16] 函数 / 方法重载
来源：http://eqw.redwolf501.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zat.bbcook.cn

PHP:  // 无重载
来源：http://nrs.xinyue.icu

JS:   // 无重载：靠 arguments.length 分支
来源：http://bbj.aizwys.cn

TS:   // 用联合类型或重载签名声明
来源：http://mcq.svipenyu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://nli.xinyue.icu

Go:   // 无重载：用不同函数名
来源：http://nyc.gotoacloud.top

Ruby: # 无重载：靠动态参数
来源：http://sss.zhaomingkeji.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://lul.jlsjyb.cn

================================================================================
来源：http://cnw.sxryk.cn

D. 数组 / 列表 / 集合
来源：http://czz.jinqigufen.top

================================================================================
来源：http://ikh.0kj1m.cn

[D01] 创建数组 / 列表
来源：http://ljq.redwolf501.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://upe.guowangkeji.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jyw.fanxiaobao.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://diu.daxiang520.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://slm.xingfuxueyuan.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qjh.yuxming.cn

Go:   arr := []int{1, 2, 3}
来源：http://kbt.yj20258888.top

Ruby: arr = [1, 2, 3]
来源：http://frt.guannengcc.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pyr.zhongyouzk.top

[D02] 追加元素到末尾
来源：http://qup.ppjwa.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mlb.haohaochexian.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fqr.ywan-chungtsiang.top

JS:   arr.push(4);
来源：http://fiw.jqgfzy.top

TS:   arr.push(4);
来源：http://rgn.meibo888.top

Java: list.add(4);
来源：http://gab.tanke756.top

Go:   arr = append(arr, 4)
来源：http://hsy.wangdashe.top

Ruby: arr << 4; arr.push(5)
来源：http://sdq.andypj.xyz

C#:   list.Add(4);
来源：http://hom.fehbvm.com

[D03] 在指定位置插入元素
来源：http://oqq.hnqzz.top

Py:   arr.insert(0, 0)
来源：http://jqz.tanke756.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dtz.bjfxy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qww.quarkkingdee.top

TS:   arr.splice(0, 0, 0);
来源：http://pox.pycfn.com

Java: list.add(0, 0);
来源：http://cye.epnwcf.com

Go:   arr = append([]int{0}, arr...)
来源：http://xkw.ctjpmb.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jtv.andypj.xyz

C#:   list.Insert(0, 0);
来源：http://bxe.zdqjudy.top

[D04] 删除元素
来源：http://pbv.jinqigufen.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bqk.zdqjudy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jgn.pycfn.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://skg.c1oappe.top

TS:   arr.splice(0, 1);
来源：http://ukp.hcnkem.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wji.nanxuanxn.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gki.smart0.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://woh.guannengcc.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jac.kuanghao11.cn

[D05] 访问与修改元素
来源：http://ijh.gaohongyu789.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jax.yanxiufei.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://knp.zycfv.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hdu.0kj1m.cn

TS:   arr[0]; arr.at(-1);
来源：http://pct.gaohongyu789.top

Java: list.get(0); list.set(0, 9);
来源：http://don.guannengcc.top

Go:   arr[0]; arr[0] = 9
来源：http://hmm.nwbrower.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://atc.wangshuangyany.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dag.fanxiaobao.xyz

[D06] 数组长度
来源：http://bkp.hfpthk.cn

Py:   len(arr)
来源：http://rli.jinghuilouyu.cn

PHP:  count($arr);
来源：http://aqb.cucudq.cn

JS:   arr.length
来源：http://dtf.bbcook.cn

TS:   arr.length
来源：http://wju.vqdsnc.cn

Java: list.size();
来源：http://ugz.hcnkem.com

Go:   len(arr)
来源：http://pkx.gzhubu.top

Ruby: arr.length; arr.size
来源：http://rvr.jqgfzy.top

C#:   list.Count;
来源：http://cwf.fengsongda.top

[D07] 切片 / 取子数组
来源：http://fsb.hnxiangtu.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://niv.guannengcc.top

PHP:  array_slice($arr, 1, 3);
来源：http://asa.ydjk.org.cn

JS:   arr.slice(1, 4);
来源：http://uks.tanke756.top

TS:   arr.slice(1, 4);
来源：http://upq.shuidangran.top

Java: list.subList(1, 4);
来源：http://ttk.jinghuilouyu.cn

Go:   arr[1:4]
来源：http://snd.iojbl.cn

Ruby: arr[1, 3]
来源：http://csv.hammf.cn

C#:   list.GetRange(1, 3);
来源：http://wkw.cucudq.cn

[D08] 合并两个数组
来源：http://wdo.meibo888.top

Py:   a + b;  a.extend(b)
来源：http://euk.meibo888.top

PHP:  array_merge($a, $b);
来源：http://vch.zhaomingkeji.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://vfh.hongshengwenyu.top

TS:   [...a, ...b];
来源：http://vjr.tanke756.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://txk.wangshuangyany.cn

Go:   append(a, b...)
来源：http://cza.zhengqikj.top

Ruby: a + b;  a.concat(b)
来源：http://yts.zhoulong.xyz

C#:   a.Concat(b).ToList()
来源：http://wht.meibo888.top

[D09] 排序（升序）
来源：http://vch.tanke756.top

Py:   sorted(arr);  arr.sort()
来源：http://duq.shzxlz.cn

PHP:  sort($arr);
来源：http://knc.aizwys.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vlq.shanyushiyangkeji.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://zzn.yj202588.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ipm.xinyue.icu

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://aew.nwbrower.top

Ruby: arr.sort
来源：http://znv.xingfuxueyuan.xyz

C#:   list.Sort();
来源：http://xcr.yangfankeji.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://ihr.tanke756.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fsx.cqqwz.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://umf.ydzc1.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://onk.ivvv.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gzk.sxryk.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qrn.yfazqb.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://itx.chenzaomai.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zpj.epnwcf.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qfr.jianghu66.top

[D11] 反转数组
来源：http://vkg.andypj.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://ckv.yj20258888.top

PHP:  array_reverse($arr);
来源：http://beq.jqgufenzy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mkt.gaohongyu789.top

TS:   [...arr].reverse();
来源：http://hok.mhx1999.top

Java: Collections.reverse(list);
来源：http://gke.jinyuanbaomall.cn

Go:   slices.Reverse(arr)
来源：http://hqz.shanyushiyangkeji.top

Ruby: arr.reverse
来源：http://dzy.yvedp.cn

C#:   list.Reverse();
来源：http://chb.aibaodan.cn

[D12] 查找元素下标
来源：http://nvb.vehdjk.com

Py:   arr.index(x);  x in arr
来源：http://npa.ivvv.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mnz.fanxiaobao.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://exr.pengpengdd.cyou

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gzq.xinyue.icu

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://iuk.smart0.xyz

Go:   slices.Index(arr, x)
来源：http://cog.shanyushiyangkeji.top

Ruby: arr.index(x)
来源：http://wse.ywan-chungtsiang.top

C#:   list.IndexOf(x);
来源：http://pwq.c1oappe.top

[D13] 过滤（保留满足条件的）
来源：http://hne.iojbl.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kfg.yj20258888.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fdi.zhixingplan.top

JS:   arr.filter(x => x > 3)
来源：http://jwf.gotoacloud.top

TS:   arr.filter(x => x > 3)
来源：http://ker.jyoumei.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zak.quarkkingdee.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kse.zhoulong.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://hji.nanxinkj.top

C#:   list.Where(x => x > 3).ToList()
来源：http://uot.316326.xyz

[D14] 映射转换（每个元素变形）
来源：http://lsc.cucudq.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://doy.daxiang520.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wqv.snrcjt.cn

JS:   arr.map(x => x * 2)
来源：http://jyr.zdqjudy.top

TS:   arr.map(x => x * 2)
来源：http://ffu.zhengqikj.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://rdz.pengpengdd.cyou

Go:   // 手写循环
来源：http://bih.wangshuangyany.cn

Ruby: arr.map { |x| x * 2 }
来源：http://cnd.cashguo.top

C#:   list.Select(x => x * 2).ToList()
来源：http://rmo.yanxiufei.cn


<!-- 参考信息 -->