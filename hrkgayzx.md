代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tim.ivvv.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wgs.iojbl.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gno.yanxiufei.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kga.fanxiaobao.xyz

[B13] 判断是否为数字
来源：http://qhb.fktsv.cn

Py:   isinstance(x, (int, float))
来源：http://qbi.fengsongda.top

PHP:  is_numeric($x)
来源：http://knn.fengsongda.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blj.sjlbkw.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ifk.tianlin.xyz

Java: x instanceof Number
来源：http://nwt.snrcjt.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ayd.gotoacloud.top

Ruby: x.is_a?(Numeric)
来源：http://upf.aizwys.cn

C#:   x is int or double or decimal
来源：http://zdz.hesvh.cn

[B14] 判断值是否在集合内
来源：http://npw.316326.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://oeu.iojbl.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lbz.nanxinkj.top

JS:   [1, 2, 3].includes(x)
来源：http://ydw.mhx1999.top

TS:   [1, 2, 3].includes(x)
来源：http://lxh.epnwcf.com

Java: List.of(1, 2, 3).contains(x)
来源：http://ikk.yfazqb.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fdo.zdqjudy.top

Ruby: [1, 2, 3].include?(x)
来源：http://yrd.svipenyu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tqm.kuanghao11.cn

[B15] 布尔运算与取反
来源：http://egx.sjlbkw.cn

Py:   a and b or not c
来源：http://yub.epnwcf.com

PHP:  $a && $b || !$c
来源：http://otj.cqqwz.cn

JS:   a && b || !c
来源：http://kvk.guowangkeji.top

TS:   a && b || !c
来源：http://aea.jqgufenzy.top

Java: a && b || !c
来源：http://hua.pycfn.com

Go:   a && b || !c
来源：http://nus.xinyue.icu

Ruby: a && b || !c
来源：http://xph.gotoacloud.top

C#:   a && b || !c
来源：http://buz.ivvv.top

[B16] 卫语句：不满足条件提前返回
来源：http://ydc.cqqwz.cn

Py:   if not data: return
来源：http://pll.sysykeji.top

PHP:  if (!$data) { return; }
来源：http://fha.bbcook.cn

JS:   if (!data) return;
来源：http://wps.shanyushiyangtech.top

TS:   if (!data) return;
来源：http://ffr.hysaishi.cn

Java: if (data == null) return;
来源：http://rid.cucudq.cn

Go:   if data == nil { return }
来源：http://psp.fanxiaobao.xyz

Ruby: return if data.nil?
来源：http://rjo.chenjidiqi.icu

C#:   if (data == null) return;
来源：http://ifq.jqgufenzy.top

================================================================================
来源：http://xkk.xuanzx.com

C. 函数与作用域
来源：http://agp.yj202588.top

================================================================================
来源：http://mia.zhaomingkeji.xyz

[C01] 定义函数
来源：http://gza.ywan-chungtsiang.top

Py:   def add(a, b): return a + b
来源：http://bna.zhaomingkeji.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rsg.uphjek.com

JS:   function add(a, b) { return a + b; }
来源：http://hpn.cashguo.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://agn.yvedp.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://vpa.ydzc1.top

Go:   func add(a, b int) int { return a + b }
来源：http://bhj.bbcook.cn

Ruby: def add(a, b); a + b; end
来源：http://yaj.ivvv.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wam.jqgfzy.top

[C02] 默认参数
来源：http://dmc.cucudq.cn

Py:   def greet(name="World"): return name
来源：http://gcm.hesvh.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://maf.cheryme.top

JS:   function greet(name = "World") { return name; }
来源：http://rin.chenjidiqi.icu

TS:   function greet(name: string = "World") { return name; }
来源：http://zah.hywenlv.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vuq.zdbjq.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nkm.52xcode.cn

Ruby: def greet(name = "World") = name
来源：http://qat.yuxming.cn

C#:   string Greet(string name = "World") => name;
来源：http://lys.hnqzz.top

[C03] 可变参数
来源：http://gia.quarkkingdee.top

Py:   def total(*args): return sum(args)
来源：http://gzu.shangyingyoupin.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zvw.ehwqpu.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lvl.tanke756.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lds.daria6918.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tif.yuanzhike.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ebi.jlsjyb.cn

Ruby: def total(*nums); nums.sum; end
来源：http://agz.hysaishi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yqs.pengpengdd.cyou

[C04] 命名参数 / 关键字参数
来源：http://fso.nanxuanxn.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wry.jqgfzy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://oni.nanxinkj.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gct.hywenlv.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yju.ydjk.org.cn

Java: // 无：用 Builder 模式或 record
来源：http://pqn.kuanghao11.cn

Go:   // 无：用配置结构体参数
来源：http://ten.jinqigfzy.top

Ruby: f(a: 1, b: 2)
来源：http://pnz.zhaomingkeji.xyz

C#:   f(a: 1, b: 2)
来源：http://ucy.gogol.net.cn

[C05] 返回多个值
来源：http://ngw.cucudq.cn

Py:   return a, b
来源：http://aqk.meibo888.top

PHP:  return [$a, $b];
来源：http://ngu.jinqigufen.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://oxo.jqgufenzy.top

TS:   return { a, b };
来源：http://bfy.ivvv.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vkk.jinghuilouyu.cn

Go:   return a, b
来源：http://qzk.ehwqpu.com

Ruby: return a, b
来源：http://egz.tian-w.cn

C#:   return (a, b);              // ValueTuple
来源：http://zfo.ybcxt.top

[C06] 匿名函数 / lambda
来源：http://mqo.hnxiangtu.top

Py:   square = lambda x: x * x
来源：http://rcj.c1oappe.top

PHP:  $square = fn($x) => $x * $x;
来源：http://lbc.daria6918.cn

JS:   const square = x => x * x;
来源：http://afs.xuanzx.com

TS:   const square = (x: number): number => x * x;
来源：http://kfr.meibo888.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kfs.gotoacloud.top

Go:   sq := func(x int) int { return x * x }
来源：http://cdm.dianchejie.cn

Ruby: square = ->(x) { x * x }
来源：http://kqf.wangdashe.top

C#:   Func<int, int> square = x => x * x;
来源：http://pjp.gotoacloud.top

[C07] 把函数作为参数传入
来源：http://okz.redwolf501.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://enw.cashguo.top

PHP:  array_map("strtoupper", $arr);
来源：http://nxd.meibo888.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jex.jqgufenzy.top

TS:   arr.map(String)
来源：http://ser.zdbjq.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://szl.sxryk.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://eol.yanxiufei.cn

Ruby: arr.map(&:upcase)
来源：http://itn.yanxiufei.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xmz.fehbvm.com

[C08] 闭包
来源：http://axc.cqqwz.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gfj.sweek.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gsn.tarul.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hvf.aibaodan.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dyy.mhx1999.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://buk.nanxinkj.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bgm.meibo888.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bks.shanyushiyangkeji.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rmj.fktsv.cn

[C09] 递归
来源：http://bbu.fengsongda.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cpn.kuanghao11.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vlf.yj202588.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://swx.tianlin.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uhq.aizwys.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://aby.meibo888.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ruj.yvedp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://clq.zhijiandao.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vca.fanxiaobao.xyz

[C10] 变量作用域
来源：http://wku.xylfe.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mjq.jinghuilouyu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://eeu.svipenyu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tpn.guannengcc.top

TS:   同 JS
来源：http://qoe.yueranfly.top

Java: 方法内为块级作用域
来源：http://nmi.xingfuxueyuan.xyz

Go:   花括号块级作用域
来源：http://rkl.daxiang520.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://aia.zdqjudy.top

C#:   块级作用域
来源：http://fzy.gotoacloud.top

[C11] 模块导入与导出
来源：http://esa.xylfe.cn

Py:   from module import func
来源：http://jwh.ppjwa.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bkn.bjfxy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ghf.sysykeji.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://iug.zhongyouzk.top

Java: import java.util.List;
来源：http://skb.ydjk.org.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ssu.mhx1999.top

Ruby: require "json"; require_relative "./util"
来源：http://keg.shanyushiyangtech.top

C#:   using System.Text;
来源：http://msy.epnwcf.com

[C12] 立即执行函数 IIFE
来源：http://vco.jinqigufen.top

Py:   (lambda: print("run"))()
来源：http://rpj.jianghu66.top

PHP:  (function () { echo "run"; })();
来源：http://ezk.52xcode.cn

JS:   (() => { console.log("run"); })();
来源：http://rfs.yuanzhike.top

TS:   (() => { console.log("run"); })();
来源：http://avl.yfazqb.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wmj.fehbvm.com

Go:   func() { fmt.Println("run") }()
来源：http://xeh.birdmap.top

Ruby: -> { puts "run" }.call
来源：http://hug.uphjek.com

C#:   // 无 IIFE：用静态构造函数
来源：http://joi.xziqi.cn

[C13] 类型声明 / 类型注解
来源：http://vjs.zhijiandao.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sle.gogol.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ypf.sufxvd.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dcv.zhoulong.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bfb.aizwys.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ptf.iojbl.cn

Go:   func add(a, b int) int
来源：http://ivx.ppjwa.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kcw.tianlin.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://qad.xingfuxueyuan.xyz

[C14] 泛型函数
来源：http://otu.cheryme.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ljd.iojbl.cn

PHP:  // 无泛型
来源：http://okk.ppjwa.cn

JS:   // 无泛型
来源：http://kkr.epnwcf.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yby.bbcook.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qzi.yvedp.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ndw.quarkkingdee.top

Ruby: # 无泛型
来源：http://zps.ydzc1.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cmh.nwbrower.top

[C15] 解构 / 展开参数
来源：http://suh.hfpthk.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jcy.hywenlv.cn

PHP:  [$a, $b] = $pair;
来源：http://vrb.tarul.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gcg.shanyushiyangtech.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ayw.hnxiangtu.top

Java: // 无解构
来源：http://odt.sweek.top

Go:   // 无解构
来源：http://vxj.sweek.top

Ruby: a, b = pair
来源：http://wlm.daria6918.cn

C#:   var (a, b) = pair;
来源：http://lcc.iojbl.cn

[C16] 函数 / 方法重载
来源：http://pka.yuxming.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://flv.hnqzz.top

PHP:  // 无重载
来源：http://qei.wangshuangyany.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://szt.mhx1999.top

TS:   // 用联合类型或重载签名声明
来源：http://luf.yvedp.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://lfj.ywan-chungtsiang.top

Go:   // 无重载：用不同函数名
来源：http://qji.jqgfzy.top

Ruby: # 无重载：靠动态参数
来源：http://zgr.shanyushiyangkeji.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://tgn.chenjidiqi.icu

================================================================================
来源：http://ahl.c1oappe.top

D. 数组 / 列表 / 集合
来源：http://hix.9152youxi.cn

================================================================================
来源：http://hfg.gzhubu.top

[D01] 创建数组 / 列表
来源：http://rlz.0kj1m.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://avf.chenlongwang.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cey.yfazqb.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sma.ybcxt.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://mvw.shangyingyoupin.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://iwo.dianchejie.cn

Go:   arr := []int{1, 2, 3}
来源：http://suo.jianghu66.top

Ruby: arr = [1, 2, 3]
来源：http://saj.uphjek.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gjr.hnqzz.top

[D02] 追加元素到末尾
来源：http://xhp.chenlongwang.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://isz.yuanzhike.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xfl.ydjk.org.cn

JS:   arr.push(4);
来源：http://rde.vqdsnc.cn

TS:   arr.push(4);
来源：http://mik.hywenlv.cn

Java: list.add(4);
来源：http://dqr.yongpay.top

Go:   arr = append(arr, 4)
来源：http://mus.birdmap.top

Ruby: arr << 4; arr.push(5)
来源：http://hpz.pengpengdd.cyou

C#:   list.Add(4);
来源：http://xzh.fanxiaobao.xyz

[D03] 在指定位置插入元素
来源：http://wwd.hcnkem.com

Py:   arr.insert(0, 0)
来源：http://vui.cqqwz.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ycb.jqgfzy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qer.hysaishi.cn

TS:   arr.splice(0, 0, 0);
来源：http://qjd.ehwqpu.com

Java: list.add(0, 0);
来源：http://ima.shzxlz.cn

Go:   arr = append([]int{0}, arr...)
来源：http://qwo.ivvv.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://scd.tian-w.cn

C#:   list.Insert(0, 0);
来源：http://nig.zhixingplan.top

[D04] 删除元素
来源：http://ztf.zhongyouzk.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wdy.snrcjt.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sds.sweek.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wws.bbcook.cn

TS:   arr.splice(0, 1);
来源：http://cuf.cdnleiting.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vnn.xylfe.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ftm.wangdashe.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ejm.xylfe.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://niu.yongpay.top

[D05] 访问与修改元素
来源：http://roa.chenjidiqi.icu

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bzt.hywenlv.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://eyy.hnxiangtu.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lsm.daxiang520.top

TS:   arr[0]; arr.at(-1);
来源：http://dht.pengpengdd.cyou

Java: list.get(0); list.set(0, 9);
来源：http://zfx.c1oappe.top

Go:   arr[0]; arr[0] = 9
来源：http://ecf.yfazqb.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://iif.jianghu66.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qso.zdbjq.cn

[D06] 数组长度
来源：http://msp.feifeiyinyue.top

Py:   len(arr)
来源：http://rtj.yongpay.top

PHP:  count($arr);
来源：http://aju.cheryme.top

JS:   arr.length
来源：http://eta.gogol.net.cn

TS:   arr.length
来源：http://dis.havefunace.top

Java: list.size();
来源：http://nvj.tarul.cn

Go:   len(arr)
来源：http://wxh.xylfe.cn

Ruby: arr.length; arr.size
来源：http://icy.zhoulong.xyz

C#:   list.Count;
来源：http://uiq.xziqi.cn

[D07] 切片 / 取子数组
来源：http://oqp.mhx1999.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qjf.yj20258888.top

PHP:  array_slice($arr, 1, 3);
来源：http://qtq.cheryme.top

JS:   arr.slice(1, 4);
来源：http://lky.hesvh.cn

TS:   arr.slice(1, 4);
来源：http://hag.chenlongwang.top

Java: list.subList(1, 4);
来源：http://xep.zhaomingkeji.xyz

Go:   arr[1:4]
来源：http://kvu.dashuyun.cn

Ruby: arr[1, 3]
来源：http://zul.yangfankeji.com

C#:   list.GetRange(1, 3);
来源：http://wtw.sjlbkw.cn

[D08] 合并两个数组
来源：http://opm.hammf.cn

Py:   a + b;  a.extend(b)
来源：http://ixt.ydjk.org.cn

PHP:  array_merge($a, $b);
来源：http://ave.dianchejie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ehf.feifeiyinyue.top

TS:   [...a, ...b];
来源：http://dfh.zdqjudy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zrc.hfpthk.cn

Go:   append(a, b...)
来源：http://nct.haohaochexian.top

Ruby: a + b;  a.concat(b)
来源：http://uec.yvedp.cn

C#:   a.Concat(b).ToList()
来源：http://lqc.shanyushiyangtech.top

[D09] 排序（升序）
来源：http://jdc.jqgufenzy.top

Py:   sorted(arr);  arr.sort()
来源：http://gww.aizwys.cn

PHP:  sort($arr);
来源：http://mre.vqdsnc.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dcx.xuetiantiany.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://nhr.hcnkem.com

Java: Collections.sort(list);  list.sort(null);
来源：http://civ.yangfankeji.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jlt.cashguo.top

Ruby: arr.sort
来源：http://ucx.yonumen.top

C#:   list.Sort();
来源：http://day.daxiang520.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://wqo.hfpthk.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yiq.ppjwa.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kza.ydjk.org.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vqw.daria6918.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ect.xziqi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://iji.vqdsnc.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jss.iojbl.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cdh.fehbvm.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hee.wangshuangyany.cn

[D11] 反转数组
来源：http://lzt.aibaodan.cn

Py:   arr[::-1];  arr.reverse()
来源：http://syp.jyoumei.cn

PHP:  array_reverse($arr);
来源：http://zmu.vehdjk.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mej.jinghuilouyu.cn

TS:   [...arr].reverse();
来源：http://pef.sweek.top

Java: Collections.reverse(list);
来源：http://xvf.pycfn.com

Go:   slices.Reverse(arr)
来源：http://vvq.yj20258888.top

Ruby: arr.reverse
来源：http://pdp.gaohongyu789.top

C#:   list.Reverse();
来源：http://cjv.hongshengwenyu.top

[D12] 查找元素下标
来源：http://uup.jqgfzy.top

Py:   arr.index(x);  x in arr
来源：http://idb.sysykeji.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gql.316326.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bpw.fzhhl.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ojq.yuanzhike.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uhs.hnxiangtu.top

Go:   slices.Index(arr, x)
来源：http://mmo.yangfankeji.com

Ruby: arr.index(x)
来源：http://euc.ywan-chungtsiang.top

C#:   list.IndexOf(x);
来源：http://zlr.zdqjudy.top

[D13] 过滤（保留满足条件的）
来源：http://jyw.xuanzx.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ijk.yj202588.top


<!-- 参考信息 -->