代发 wailian999

C#:   x is int or double or decimal
来源：http://dcg.gogol.net.cn

[B14] 判断值是否在集合内
来源：http://csp.gogol.net.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://plh.kuanghao11.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://epm.52xcode.cn

JS:   [1, 2, 3].includes(x)
来源：http://wdk.jinghuilouyu.cn

TS:   [1, 2, 3].includes(x)
来源：http://lwx.aizwys.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://hil.jianghu66.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bzn.nanxuanxn.top

Ruby: [1, 2, 3].include?(x)
来源：http://bey.svipenyu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://glj.shuidangran.top

[B15] 布尔运算与取反
来源：http://eqz.xingfuxueyuan.xyz

Py:   a and b or not c
来源：http://oko.nwbrower.top

PHP:  $a && $b || !$c
来源：http://tmb.hnxiangtu.top

JS:   a && b || !c
来源：http://krv.dashuyun.cn

TS:   a && b || !c
来源：http://zjr.pycfn.com

Java: a && b || !c
来源：http://xwl.yj20258888.top

Go:   a && b || !c
来源：http://hew.jinqigufen.top

Ruby: a && b || !c
来源：http://lhx.andypj.xyz

C#:   a && b || !c
来源：http://rsx.chenjidiqi.icu

[B16] 卫语句：不满足条件提前返回
来源：http://yfl.52xcode.cn

Py:   if not data: return
来源：http://mca.sjlbkw.cn

PHP:  if (!$data) { return; }
来源：http://key.yangfankeji.com

JS:   if (!data) return;
来源：http://cas.gogol.net.cn

TS:   if (!data) return;
来源：http://dbz.316326.xyz

Java: if (data == null) return;
来源：http://rvy.xingfuxueyuan.xyz

Go:   if data == nil { return }
来源：http://rhf.tarul.cn

Ruby: return if data.nil?
来源：http://qik.ydzc1.top

C#:   if (data == null) return;
来源：http://dar.hesvh.cn

================================================================================
来源：http://hfs.yongpay.top

C. 函数与作用域
来源：http://ohn.xziqi.cn

================================================================================
来源：http://rkx.yuxming.cn

[C01] 定义函数
来源：http://ohg.fehbvm.com

Py:   def add(a, b): return a + b
来源：http://mdn.chenzaomai.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://auz.52xcode.cn

JS:   function add(a, b) { return a + b; }
来源：http://wpj.xuetiantiany.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tft.tianlin.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://wun.sufxvd.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hcf.c1oappe.top

Ruby: def add(a, b); a + b; end
来源：http://nqp.jinqigufen.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lrk.jianghu66.top

[C02] 默认参数
来源：http://mfa.xylfe.cn

Py:   def greet(name="World"): return name
来源：http://dvl.cucudq.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://awj.ydzc1.top

JS:   function greet(name = "World") { return name; }
来源：http://bfw.yongpay.top

TS:   function greet(name: string = "World") { return name; }
来源：http://bif.redwolf501.top

Java: // 无默认参数：方法重载或 Optional
来源：http://kby.aibaodan.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gwg.yvedp.cn

Ruby: def greet(name = "World") = name
来源：http://zap.ybcxt.top

C#:   string Greet(string name = "World") => name;
来源：http://qdt.fktsv.cn

[C03] 可变参数
来源：http://olj.gaohongyu789.top

Py:   def total(*args): return sum(args)
来源：http://cng.shzxlz.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tvu.bbcook.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qvv.zdqjudy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ycz.jinyuanbaomall.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hyw.aizwys.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ybe.xuanzx.com

Ruby: def total(*nums); nums.sum; end
来源：http://ios.yvedp.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mfq.hywenlv.cn

[C04] 命名参数 / 关键字参数
来源：http://qzk.mhx1999.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yao.birdmap.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hlv.sufxvd.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dfc.fzhhl.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fxl.jqgufenzy.top

Java: // 无：用 Builder 模式或 record
来源：http://iuc.aibaodan.cn

Go:   // 无：用配置结构体参数
来源：http://fiw.shzxlz.cn

Ruby: f(a: 1, b: 2)
来源：http://umw.jianghu66.top

C#:   f(a: 1, b: 2)
来源：http://esa.pengpengdd.cyou

[C05] 返回多个值
来源：http://dgb.uphjek.com

Py:   return a, b
来源：http://wni.xuetiantiany.cn

PHP:  return [$a, $b];
来源：http://adi.redwolf501.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://jdu.pycfn.com

TS:   return { a, b };
来源：http://mcs.c1oappe.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lqn.zdqjudy.top

Go:   return a, b
来源：http://pgr.pycfn.com

Ruby: return a, b
来源：http://riu.zhengqikj.top

C#:   return (a, b);              // ValueTuple
来源：http://otl.aizwys.cn

[C06] 匿名函数 / lambda
来源：http://bhq.tanke756.top

Py:   square = lambda x: x * x
来源：http://dcc.birdmap.top

PHP:  $square = fn($x) => $x * $x;
来源：http://hbc.epnwcf.com

JS:   const square = x => x * x;
来源：http://bsm.jqgufenzy.top

TS:   const square = (x: number): number => x * x;
来源：http://pjk.meibo888.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hpc.xinyue.icu

Go:   sq := func(x int) int { return x * x }
来源：http://opd.dashuyun.cn

Ruby: square = ->(x) { x * x }
来源：http://zjx.hysaishi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://lsf.ybcxt.top

[C07] 把函数作为参数传入
来源：http://zgh.feifeiyinyue.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cdd.mhx1999.top

PHP:  array_map("strtoupper", $arr);
来源：http://grn.daxiang520.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://txh.chenjidiqi.icu

TS:   arr.map(String)
来源：http://bev.316326.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gin.zhongyouzk.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://knv.guannengcc.top

Ruby: arr.map(&:upcase)
来源：http://hmf.jinqigfzy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://zfg.kuanghao11.cn

[C08] 闭包
来源：http://mpa.zycfv.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rqo.cucudq.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ihs.quarkkingdee.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cxn.cashguo.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kax.zhiwuduotai.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kij.nanxinkj.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xxv.yuanzhike.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wcb.wangdashe.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://scv.zhoulong.xyz

[C09] 递归
来源：http://ekd.gotoacloud.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mzk.jyoumei.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tgj.iojbl.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://smc.zhiwuduotai.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hxk.yvedp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qbe.jqgfzy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ers.chenlongwang.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rla.nwbrower.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ynm.tarul.cn

[C10] 变量作用域
来源：http://wwy.mhx1999.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wym.yuanzhike.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://adu.pengpengdd.cyou

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xad.nanxuanxn.top

TS:   同 JS
来源：http://xgd.9152youxi.cn

Java: 方法内为块级作用域
来源：http://aav.shzxlz.cn

Go:   花括号块级作用域
来源：http://lzu.guannengcc.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rgd.c1oappe.top

C#:   块级作用域
来源：http://ccx.yuxming.cn

[C11] 模块导入与导出
来源：http://twp.fktsv.cn

Py:   from module import func
来源：http://ofd.ydzc1.top

PHP:  require "file.php";  或 use App\Service;
来源：http://tec.fzhhl.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://yxg.zhixingplan.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rcx.birdmap.top

Java: import java.util.List;
来源：http://wdt.andypj.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xmo.zhoulong.xyz

Ruby: require "json"; require_relative "./util"
来源：http://jnz.fengsongda.top

C#:   using System.Text;
来源：http://hmx.uphjek.com

[C12] 立即执行函数 IIFE
来源：http://vxj.sufxvd.cn

Py:   (lambda: print("run"))()
来源：http://rzo.zdqjudy.top

PHP:  (function () { echo "run"; })();
来源：http://nvn.ywan-chungtsiang.top

JS:   (() => { console.log("run"); })();
来源：http://pjv.chenjidiqi.icu

TS:   (() => { console.log("run"); })();
来源：http://vrv.zhengqikj.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ung.zhiwuduotai.top

Go:   func() { fmt.Println("run") }()
来源：http://cej.shanyushiyangtech.top

Ruby: -> { puts "run" }.call
来源：http://ztv.jinqigfzy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://wdp.gogol.net.cn

[C13] 类型声明 / 类型注解
来源：http://vjc.yj20258888.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://npn.yuanzhike.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pku.yvedp.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qtm.fehbvm.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kye.ydjk.org.cn

Java: int add(int a, int b) { return a + b; }
来源：http://szx.ctjpmb.com

Go:   func add(a, b int) int
来源：http://rkm.redwolf501.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://uqf.jyoumei.cn

C#:   int Add(int a, int b) => a + b;
来源：http://awo.svipenyu.cn

[C14] 泛型函数
来源：http://evf.wangdashe.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lcu.316326.xyz

PHP:  // 无泛型
来源：http://ogf.zhaomingkeji.xyz

JS:   // 无泛型
来源：http://gmk.vehdjk.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ecp.shanyushiyangkeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://oec.tanke756.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dve.hnqzz.top

Ruby: # 无泛型
来源：http://hpx.yonumen.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nkj.tian-w.cn

[C15] 解构 / 展开参数
来源：http://fqp.hysaishi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://try.xuanzx.com

PHP:  [$a, $b] = $pair;
来源：http://poa.tian-w.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bib.zhongyouzk.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tkp.haohaochexian.top

Java: // 无解构
来源：http://oqf.daria6918.cn

Go:   // 无解构
来源：http://hts.yj20258888.top

Ruby: a, b = pair
来源：http://uup.ydzc1.top

C#:   var (a, b) = pair;
来源：http://gpj.tianlin.xyz

[C16] 函数 / 方法重载
来源：http://ivl.cashguo.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tgr.hammf.cn

PHP:  // 无重载
来源：http://lch.aizwys.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://imu.pycfn.com

TS:   // 用联合类型或重载签名声明
来源：http://fzc.fengsongda.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ucc.sjlbkw.cn

Go:   // 无重载：用不同函数名
来源：http://eun.mhx1999.top

Ruby: # 无重载：靠动态参数
来源：http://fon.yanxiufei.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ffl.yj20258888.top

================================================================================
来源：http://cea.havefunace.top

D. 数组 / 列表 / 集合
来源：http://yba.nanxuanxn.top

================================================================================
来源：http://fve.fzhhl.top

[D01] 创建数组 / 列表
来源：http://knz.xziqi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://arz.fzhhl.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xqu.aibaodan.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jkj.zhongyouzk.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://quk.wangshuangyany.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ipq.hnxiangtu.top

Go:   arr := []int{1, 2, 3}
来源：http://tgr.daxiang520.top

Ruby: arr = [1, 2, 3]
来源：http://hzr.xinyue.icu

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hnj.daria6918.cn

[D02] 追加元素到末尾
来源：http://tcp.ppjwa.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zhh.redwolf501.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ouv.yuanzhike.top

JS:   arr.push(4);
来源：http://uzp.daria6918.cn

TS:   arr.push(4);
来源：http://daz.zhijiandao.cn

Java: list.add(4);
来源：http://hhb.havefunace.top

Go:   arr = append(arr, 4)
来源：http://sge.nanxuanxn.top

Ruby: arr << 4; arr.push(5)
来源：http://ehz.52xcode.cn

C#:   list.Add(4);
来源：http://url.tarul.cn

[D03] 在指定位置插入元素
来源：http://xjp.tianlin.xyz

Py:   arr.insert(0, 0)
来源：http://kpy.xuetiantiany.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://khg.0kj1m.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://snt.c1oappe.top

TS:   arr.splice(0, 0, 0);
来源：http://nmo.zhongyouzk.top

Java: list.add(0, 0);
来源：http://wcp.gaohongyu789.top

Go:   arr = append([]int{0}, arr...)
来源：http://qqs.shangyingyoupin.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ojb.chenzaomai.com

C#:   list.Insert(0, 0);
来源：http://dvt.yongpay.top

[D04] 删除元素
来源：http://lxt.sufxvd.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cnx.fanxiaobao.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dwn.shuidangran.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yqd.jinyuanbaomall.cn

TS:   arr.splice(0, 1);
来源：http://whh.fanxiaobao.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wup.zhaomingkeji.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zvb.sjlbkw.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rid.chenzaomai.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zqt.cqqwz.cn

[D05] 访问与修改元素
来源：http://efb.c1oappe.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vkn.guowangkeji.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wvc.zhiwuduotai.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://oqn.xuanzx.com

TS:   arr[0]; arr.at(-1);
来源：http://rjr.zdqjudy.top

Java: list.get(0); list.set(0, 9);
来源：http://vdq.jqgufenzy.top

Go:   arr[0]; arr[0] = 9
来源：http://njb.shanyushiyangkeji.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ugx.kuanghao11.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://deu.xingfuxueyuan.xyz

[D06] 数组长度
来源：http://xjy.jiagoushi.top

Py:   len(arr)
来源：http://moz.jinqigfzy.top

PHP:  count($arr);
来源：http://aqu.fengsongda.top

JS:   arr.length
来源：http://gnt.zhijiandao.cn

TS:   arr.length
来源：http://eck.tian-w.cn

Java: list.size();
来源：http://yai.bbcook.cn

Go:   len(arr)
来源：http://pvt.guannengcc.top

Ruby: arr.length; arr.size
来源：http://cjq.pycfn.com

C#:   list.Count;
来源：http://zze.zdbjq.cn

[D07] 切片 / 取子数组
来源：http://aam.nwbrower.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jaq.nanxuanxn.top

PHP:  array_slice($arr, 1, 3);
来源：http://tqv.nwbrower.top

JS:   arr.slice(1, 4);
来源：http://jks.52xcode.cn

TS:   arr.slice(1, 4);
来源：http://lep.xylfe.cn

Java: list.subList(1, 4);
来源：http://tdo.zhongyouzk.top

Go:   arr[1:4]
来源：http://qea.yonumen.top

Ruby: arr[1, 3]
来源：http://oiq.hfpthk.cn

C#:   list.GetRange(1, 3);
来源：http://efn.vehdjk.com

[D08] 合并两个数组
来源：http://upf.bbcook.cn

Py:   a + b;  a.extend(b)
来源：http://vcj.ydjk.org.cn

PHP:  array_merge($a, $b);
来源：http://kua.hysaishi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://vau.chenjidiqi.icu

TS:   [...a, ...b];
来源：http://bvc.hywenlv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ujz.yfazqb.com

Go:   append(a, b...)
来源：http://czk.jqgufenzy.top

Ruby: a + b;  a.concat(b)
来源：http://oiz.yj202588.top

C#:   a.Concat(b).ToList()
来源：http://bsf.jinqigfzy.top

[D09] 排序（升序）
来源：http://cby.dashuyun.cn

Py:   sorted(arr);  arr.sort()
来源：http://nra.yueranfly.top

PHP:  sort($arr);
来源：http://jzc.yfazqb.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dja.zhongyouzk.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://atn.cheryme.top

Java: Collections.sort(list);  list.sort(null);
来源：http://cms.gogol.net.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tsa.pengpengdd.cyou

Ruby: arr.sort
来源：http://wxg.dashuyun.cn

C#:   list.Sort();
来源：http://vzg.yuxming.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://kmo.ctjpmb.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://eqw.quarkkingdee.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iht.zhongyouzk.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cfj.sjlbkw.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://olu.hysaishi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baq.aibaodan.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zwe.zhongyouzk.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ykn.ydjk.org.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hdn.sufxvd.cn

[D11] 反转数组
来源：http://ycw.tanke756.top

Py:   arr[::-1];  arr.reverse()
来源：http://jbv.yj20258.top

PHP:  array_reverse($arr);
来源：http://bdt.birdmap.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dts.tian-w.cn

TS:   [...arr].reverse();
来源：http://mnk.xuetiantiany.cn

Java: Collections.reverse(list);
来源：http://ans.zycfv.cn

Go:   slices.Reverse(arr)
来源：http://eob.cheryme.top

Ruby: arr.reverse
来源：http://lcp.meibo888.top

C#:   list.Reverse();
来源：http://rtb.shangyingyoupin.top

[D12] 查找元素下标
来源：http://bsa.52xcode.cn

Py:   arr.index(x);  x in arr
来源：http://qen.zycfv.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zyg.pengpengdd.cyou

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gnp.sysykeji.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lko.uphjek.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sjk.andypj.xyz

Go:   slices.Index(arr, x)
来源：http://jck.hammf.cn

Ruby: arr.index(x)
来源：http://fmh.ybcxt.top

C#:   list.IndexOf(x);
来源：http://hir.vqdsnc.cn

[D13] 过滤（保留满足条件的）
来源：http://qhn.shanyushiyangtech.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nla.jianghu66.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pzy.kuanghao11.cn

JS:   arr.filter(x => x > 3)
来源：http://jik.fehbvm.com

TS:   arr.filter(x => x > 3)
来源：http://dgz.bbcook.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://uig.feifeiyinyue.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gqg.chenlongwang.top

Ruby: arr.select { |x| x > 3 }
来源：http://bid.zhengqikj.top

C#:   list.Where(x => x > 3).ToList()
来源：http://txm.ctjpmb.com

[D14] 映射转换（每个元素变形）
来源：http://vak.jqgufenzy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sva.hcnkem.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zmc.jianghu66.top

JS:   arr.map(x => x * 2)
来源：http://kyd.hammf.cn

TS:   arr.map(x => x * 2)
来源：http://gnp.yj20258.top


<!-- 参考信息 -->