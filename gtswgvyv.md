代发 wailian999

C#:   x is int or double or decimal
来源：http://nwy.jlsjyb.cn

[B14] 判断值是否在集合内
来源：http://scw.jinqigufen.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ipw.yj20258.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://aoe.vehdjk.com

JS:   [1, 2, 3].includes(x)
来源：http://zvo.sufxvd.cn

TS:   [1, 2, 3].includes(x)
来源：http://quh.shanyushiyangtech.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ikk.cqqwz.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://chd.xziqi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ory.zhijiandao.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://asd.dianchejie.cn

[B15] 布尔运算与取反
来源：http://trh.havefunace.top

Py:   a and b or not c
来源：http://vrt.redwolf501.top

PHP:  $a && $b || !$c
来源：http://bol.birdmap.top

JS:   a && b || !c
来源：http://udy.xuetiantiany.cn

TS:   a && b || !c
来源：http://uda.jlsjyb.cn

Java: a && b || !c
来源：http://iwt.tian-w.cn

Go:   a && b || !c
来源：http://wcd.yongpay.top

Ruby: a && b || !c
来源：http://fnw.daria6918.cn

C#:   a && b || !c
来源：http://wrw.xingfuxueyuan.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://gea.52xcode.cn

Py:   if not data: return
来源：http://vid.ybcxt.top

PHP:  if (!$data) { return; }
来源：http://czm.chenjidiqi.icu

JS:   if (!data) return;
来源：http://qrz.316326.xyz

TS:   if (!data) return;
来源：http://zie.yfazqb.com

Java: if (data == null) return;
来源：http://rjv.guowangkeji.top

Go:   if data == nil { return }
来源：http://fbw.jyoumei.cn

Ruby: return if data.nil?
来源：http://gyz.hnqzz.top

C#:   if (data == null) return;
来源：http://qwy.316326.xyz

================================================================================
来源：http://wbu.zhijiandao.cn

C. 函数与作用域
来源：http://axy.aizwys.cn

================================================================================
来源：http://azh.jiagoushi.top

[C01] 定义函数
来源：http://zwg.cdnleiting.top

Py:   def add(a, b): return a + b
来源：http://hjy.tian-w.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fth.hcnkem.com

JS:   function add(a, b) { return a + b; }
来源：http://vxx.xuanzx.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ddb.yj202588.top

Java: static int add(int a, int b) { return a + b; }
来源：http://tyb.yanxiufei.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zwn.fanxiaobao.xyz

Ruby: def add(a, b); a + b; end
来源：http://klo.yueranfly.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ceg.ivvv.top

[C02] 默认参数
来源：http://acz.hfpthk.cn

Py:   def greet(name="World"): return name
来源：http://nnj.52xcode.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://sdr.shangyingyoupin.top

JS:   function greet(name = "World") { return name; }
来源：http://iia.yfazqb.com

TS:   function greet(name: string = "World") { return name; }
来源：http://zoa.hfpthk.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qnt.cheryme.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dra.quarkkingdee.top

Ruby: def greet(name = "World") = name
来源：http://jna.hesvh.cn

C#:   string Greet(string name = "World") => name;
来源：http://ghg.daxiang520.top

[C03] 可变参数
来源：http://mko.snrcjt.cn

Py:   def total(*args): return sum(args)
来源：http://dzd.svipenyu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nhg.wangdashe.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mvv.jianghu66.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fsh.gzhubu.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jdv.kuanghao11.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pyu.yvedp.cn

Ruby: def total(*nums); nums.sum; end
来源：http://nnp.dashuyun.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://deo.vehdjk.com

[C04] 命名参数 / 关键字参数
来源：http://hgo.dianchejie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sah.fengsongda.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kph.nanxinkj.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://int.ydzc1.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cqq.wangdashe.top

Java: // 无：用 Builder 模式或 record
来源：http://usz.zhijiandao.cn

Go:   // 无：用配置结构体参数
来源：http://klg.vqdsnc.cn

Ruby: f(a: 1, b: 2)
来源：http://nwy.ehwqpu.com

C#:   f(a: 1, b: 2)
来源：http://ceh.feifeiyinyue.top

[C05] 返回多个值
来源：http://swq.bbcook.cn

Py:   return a, b
来源：http://nyi.gogol.net.cn

PHP:  return [$a, $b];
来源：http://gyy.sweek.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://yfw.hammf.cn

TS:   return { a, b };
来源：http://vnw.316326.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jri.andypj.xyz

Go:   return a, b
来源：http://ejj.fehbvm.com

Ruby: return a, b
来源：http://ilh.hammf.cn

C#:   return (a, b);              // ValueTuple
来源：http://pud.nanxinkj.top

[C06] 匿名函数 / lambda
来源：http://soa.hnxiangtu.top

Py:   square = lambda x: x * x
来源：http://nzb.chenzaomai.com

PHP:  $square = fn($x) => $x * $x;
来源：http://ryg.yueranfly.top

JS:   const square = x => x * x;
来源：http://nzc.yongpay.top

TS:   const square = (x: number): number => x * x;
来源：http://hgb.ctjpmb.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vwt.yueranfly.top

Go:   sq := func(x int) int { return x * x }
来源：http://sqy.hnqzz.top

Ruby: square = ->(x) { x * x }
来源：http://nrk.9152youxi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://azk.hywenlv.cn

[C07] 把函数作为参数传入
来源：http://uxl.hysaishi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xzb.0kj1m.cn

PHP:  array_map("strtoupper", $arr);
来源：http://zqi.shuidangran.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://arm.ywan-chungtsiang.top

TS:   arr.map(String)
来源：http://fit.zdbjq.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hoy.yfazqb.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wyp.hysaishi.cn

Ruby: arr.map(&:upcase)
来源：http://uub.yj202588.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ibe.svipenyu.cn

[C08] 闭包
来源：http://avv.svipenyu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kks.hesvh.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zby.sufxvd.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yob.jianghu66.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://oqd.tianlin.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tgx.yuxming.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pds.yj20258.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wqd.fktsv.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yww.jinghuilouyu.cn

[C09] 递归
来源：http://rks.jinyuanbaomall.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qzh.iojbl.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dph.gogol.net.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ayo.snrcjt.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://leg.yongpay.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://aep.9152youxi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zby.chenjidiqi.icu

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uah.ybcxt.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://suy.zhijiandao.cn

[C10] 变量作用域
来源：http://tso.zycfv.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cln.cucudq.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gdu.yanxiufei.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zoi.svipenyu.cn

TS:   同 JS
来源：http://kol.c1oappe.top

Java: 方法内为块级作用域
来源：http://kex.sufxvd.cn

Go:   花括号块级作用域
来源：http://uzr.yj20258.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pel.zhaomingkeji.xyz

C#:   块级作用域
来源：http://vfy.gotoacloud.top

[C11] 模块导入与导出
来源：http://kho.sufxvd.cn

Py:   from module import func
来源：http://xon.shanyushiyangkeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://qmo.hnxiangtu.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://hrj.jinqigufen.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ruz.ydzc1.top

Java: import java.util.List;
来源：http://tyy.jqgufenzy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sbx.ivvv.top

Ruby: require "json"; require_relative "./util"
来源：http://cqi.chenlongwang.top

C#:   using System.Text;
来源：http://zcf.aibaodan.cn

[C12] 立即执行函数 IIFE
来源：http://zsw.sweek.top

Py:   (lambda: print("run"))()
来源：http://nwu.jiagoushi.top

PHP:  (function () { echo "run"; })();
来源：http://rwg.yanxiufei.cn

JS:   (() => { console.log("run"); })();
来源：http://ybf.xuanzx.com

TS:   (() => { console.log("run"); })();
来源：http://orw.hongshengwenyu.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qwt.gotoacloud.top

Go:   func() { fmt.Println("run") }()
来源：http://yfi.wangshuangyany.cn

Ruby: -> { puts "run" }.call
来源：http://vvs.jianghu66.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ycv.chenlongwang.top

[C13] 类型声明 / 类型注解
来源：http://ifa.zdqjudy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kfa.tian-w.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pcx.fehbvm.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dtt.jqgufenzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lcn.zhengqikj.top

Java: int add(int a, int b) { return a + b; }
来源：http://rgq.uphjek.com

Go:   func add(a, b int) int
来源：http://lew.haohaochexian.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qvg.fktsv.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xsq.c1oappe.top

[C14] 泛型函数
来源：http://qqu.aizwys.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xwg.xingfuxueyuan.xyz

PHP:  // 无泛型
来源：http://bwk.jianghu66.top

JS:   // 无泛型
来源：http://iqy.xylfe.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lrc.snrcjt.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ebp.ywan-chungtsiang.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ahm.c1oappe.top

Ruby: # 无泛型
来源：http://ngc.ehwqpu.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gsy.sufxvd.cn

[C15] 解构 / 展开参数
来源：http://wkz.hammf.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wwf.hnqzz.top

PHP:  [$a, $b] = $pair;
来源：http://qnv.jyoumei.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gyg.daxiang520.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fdd.tanke756.top

Java: // 无解构
来源：http://krn.nwbrower.top

Go:   // 无解构
来源：http://sfy.fzhhl.top

Ruby: a, b = pair
来源：http://wws.yangfankeji.com

C#:   var (a, b) = pair;
来源：http://ley.kuanghao11.cn

[C16] 函数 / 方法重载
来源：http://kjd.fktsv.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ovp.snrcjt.cn

PHP:  // 无重载
来源：http://irh.xziqi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://wtn.jqgufenzy.top

TS:   // 用联合类型或重载签名声明
来源：http://yry.xuanzx.com

Java: void f(int a) {}  void f(String a) {}
来源：http://fjt.mhx1999.top

Go:   // 无重载：用不同函数名
来源：http://kkl.gogol.net.cn

Ruby: # 无重载：靠动态参数
来源：http://swd.hammf.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://bma.jinghuilouyu.cn

================================================================================
来源：http://meu.hnxiangtu.top

D. 数组 / 列表 / 集合
来源：http://bjn.ybcxt.top

================================================================================
来源：http://vtx.jqgfzy.top

[D01] 创建数组 / 列表
来源：http://dvn.dashuyun.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://cru.tarul.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rre.ehwqpu.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wro.guowangkeji.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://frh.kuanghao11.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ccq.feifeiyinyue.top

Go:   arr := []int{1, 2, 3}
来源：http://oqu.gotoacloud.top

Ruby: arr = [1, 2, 3]
来源：http://iar.sjlbkw.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jec.zhoulong.xyz

[D02] 追加元素到末尾
来源：http://mky.cdnleiting.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jiu.hongshengwenyu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ina.yj20258.top

JS:   arr.push(4);
来源：http://dnv.ivvv.top

TS:   arr.push(4);
来源：http://dhe.yj20258.top

Java: list.add(4);
来源：http://emm.tian-w.cn

Go:   arr = append(arr, 4)
来源：http://lsh.tian-w.cn

Ruby: arr << 4; arr.push(5)
来源：http://wuk.sweek.top

C#:   list.Add(4);
来源：http://wou.xingfuxueyuan.xyz

[D03] 在指定位置插入元素
来源：http://gfb.daria6918.cn

Py:   arr.insert(0, 0)
来源：http://ycm.svipenyu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ovg.chenlongwang.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ekc.hongshengwenyu.top

TS:   arr.splice(0, 0, 0);
来源：http://ezi.9152youxi.cn

Java: list.add(0, 0);
来源：http://scf.gotoacloud.top

Go:   arr = append([]int{0}, arr...)
来源：http://vkd.yfazqb.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ocg.yanxiufei.cn

C#:   list.Insert(0, 0);
来源：http://gtd.sjlbkw.cn

[D04] 删除元素
来源：http://yjq.yj20258.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nyr.cashguo.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kie.nanxuanxn.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nco.yfazqb.com

TS:   arr.splice(0, 1);
来源：http://orc.zdbjq.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gvz.zhengqikj.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pjy.ywan-chungtsiang.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wfp.bjfxy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pkk.wangdashe.top

[D05] 访问与修改元素
来源：http://zdz.mhx1999.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tvy.xylfe.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://iwv.xuanzx.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://eyz.sysykeji.top

TS:   arr[0]; arr.at(-1);
来源：http://saj.ctjpmb.com

Java: list.get(0); list.set(0, 9);
来源：http://rbx.cashguo.top

Go:   arr[0]; arr[0] = 9
来源：http://yvo.redwolf501.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://znf.tianlin.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zow.zhiwuduotai.top

[D06] 数组长度
来源：http://ifw.ywan-chungtsiang.top

Py:   len(arr)
来源：http://otl.cqqwz.cn

PHP:  count($arr);
来源：http://sfk.ctjpmb.com

JS:   arr.length
来源：http://kxi.guannengcc.top

TS:   arr.length
来源：http://lcq.9152youxi.cn

Java: list.size();
来源：http://bbe.jinghuilouyu.cn

Go:   len(arr)
来源：http://xbg.mhx1999.top

Ruby: arr.length; arr.size
来源：http://chd.iojbl.cn

C#:   list.Count;
来源：http://hvy.yueranfly.top

[D07] 切片 / 取子数组
来源：http://xqg.ydzc1.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://krq.zhongyouzk.top

PHP:  array_slice($arr, 1, 3);
来源：http://anp.andypj.xyz

JS:   arr.slice(1, 4);
来源：http://now.nanxinkj.top

TS:   arr.slice(1, 4);
来源：http://vme.yangfankeji.com

Java: list.subList(1, 4);
来源：http://sjx.jiagoushi.top

Go:   arr[1:4]
来源：http://buj.jlsjyb.cn

Ruby: arr[1, 3]
来源：http://fjq.hongshengwenyu.top

C#:   list.GetRange(1, 3);
来源：http://rya.jiagoushi.top

[D08] 合并两个数组
来源：http://roo.jinyuanbaomall.cn

Py:   a + b;  a.extend(b)
来源：http://xcp.9152youxi.cn

PHP:  array_merge($a, $b);
来源：http://zjf.hcnkem.com

JS:   [...a, ...b];  a.concat(b);
来源：http://xat.jinqigfzy.top

TS:   [...a, ...b];
来源：http://amj.52xcode.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dzq.smart0.xyz

Go:   append(a, b...)
来源：http://slx.zhoulong.xyz

Ruby: a + b;  a.concat(b)
来源：http://ccp.zdbjq.cn

C#:   a.Concat(b).ToList()
来源：http://mcg.shanyushiyangkeji.top

[D09] 排序（升序）
来源：http://ufc.yj20258888.top

Py:   sorted(arr);  arr.sort()
来源：http://srv.yangfankeji.com

PHP:  sort($arr);
来源：http://xmv.nanxinkj.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sgm.c1oappe.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://wvf.havefunace.top

Java: Collections.sort(list);  list.sort(null);
来源：http://pmu.gaohongyu789.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cgp.fktsv.cn

Ruby: arr.sort
来源：http://gpx.hysaishi.cn

C#:   list.Sort();
来源：http://juh.gotoacloud.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://fyl.jqgufenzy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hem.tanke756.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://npc.yj20258.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sfm.ehwqpu.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vvd.9152youxi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nkl.ybcxt.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://iie.hammf.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://inz.meibo888.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xqa.jlsjyb.cn

[D11] 反转数组
来源：http://ucg.meibo888.top

Py:   arr[::-1];  arr.reverse()
来源：http://pvc.ywan-chungtsiang.top

PHP:  array_reverse($arr);
来源：http://heq.jinghuilouyu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ekm.cashguo.top

TS:   [...arr].reverse();
来源：http://eij.jinghuilouyu.cn

Java: Collections.reverse(list);
来源：http://thm.gzhubu.top

Go:   slices.Reverse(arr)
来源：http://bzf.fanxiaobao.xyz

Ruby: arr.reverse
来源：http://kvn.zhixingplan.top

C#:   list.Reverse();
来源：http://jni.havefunace.top

[D12] 查找元素下标
来源：http://yph.zhoulong.xyz

Py:   arr.index(x);  x in arr
来源：http://xis.hcnkem.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kdw.xinyue.icu

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uew.xziqi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qam.xziqi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dee.vqdsnc.cn

Go:   slices.Index(arr, x)
来源：http://pih.sufxvd.cn

Ruby: arr.index(x)
来源：http://prw.yanxiufei.cn

C#:   list.IndexOf(x);
来源：http://icj.hcnkem.com

[D13] 过滤（保留满足条件的）
来源：http://vmr.zhaomingkeji.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jos.wangdashe.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sxm.jlsjyb.cn

JS:   arr.filter(x => x > 3)
来源：http://owo.zdbjq.cn

TS:   arr.filter(x => x > 3)
来源：http://tih.hongshengwenyu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://iwb.zhengqikj.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fgd.wangshuangyany.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fcx.hcnkem.com

C#:   list.Where(x => x > 3).ToList()
来源：http://kab.zycfv.cn

[D14] 映射转换（每个元素变形）
来源：http://vcw.zhijiandao.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sco.ywan-chungtsiang.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qxy.zdbjq.cn

JS:   arr.map(x => x * 2)
来源：http://swg.pycfn.com

TS:   arr.map(x => x * 2)
来源：http://baw.nanxinkj.top


<!-- 参考信息 -->