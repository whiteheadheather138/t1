代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://qiu.xuetiantiany.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://qtl.yj20258888.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://eey.zhaomingkeji.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kuv.fktsv.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://oxv.fzhhl.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mjj.tian-w.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mbr.jinyuanbaomall.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nvs.shanyushiyangtech.top

[B13] 判断是否为数字
来源：http://pzu.iojbl.cn

Py:   isinstance(x, (int, float))
来源：http://rbo.daxiang520.top

PHP:  is_numeric($x)
来源：http://mzy.sweek.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nmi.gzhubu.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rtg.cucudq.cn

Java: x instanceof Number
来源：http://iwh.nanxuanxn.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bow.zdbjq.cn

Ruby: x.is_a?(Numeric)
来源：http://osr.pycfn.com

C#:   x is int or double or decimal
来源：http://xag.ydjk.org.cn

[B14] 判断值是否在集合内
来源：http://jfc.jqgufenzy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jsd.yonumen.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tqu.guannengcc.top

JS:   [1, 2, 3].includes(x)
来源：http://hbw.aizwys.cn

TS:   [1, 2, 3].includes(x)
来源：http://wby.ppjwa.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://kys.ydjk.org.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tfz.sysykeji.top

Ruby: [1, 2, 3].include?(x)
来源：http://leo.ppjwa.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://byz.guannengcc.top

[B15] 布尔运算与取反
来源：http://abo.zhixingplan.top

Py:   a and b or not c
来源：http://jwm.yuxming.cn

PHP:  $a && $b || !$c
来源：http://njv.nanxuanxn.top

JS:   a && b || !c
来源：http://snn.hfpthk.cn

TS:   a && b || !c
来源：http://okg.vqdsnc.cn

Java: a && b || !c
来源：http://bxi.shzxlz.cn

Go:   a && b || !c
来源：http://gdr.zdbjq.cn

Ruby: a && b || !c
来源：http://qqe.cqqwz.cn

C#:   a && b || !c
来源：http://ixu.nanxinkj.top

[B16] 卫语句：不满足条件提前返回
来源：http://sre.yanxiufei.cn

Py:   if not data: return
来源：http://ncd.jinghuilouyu.cn

PHP:  if (!$data) { return; }
来源：http://ggj.nanxuanxn.top

JS:   if (!data) return;
来源：http://idl.yueranfly.top

TS:   if (!data) return;
来源：http://odw.yj20258888.top

Java: if (data == null) return;
来源：http://iah.zycfv.cn

Go:   if data == nil { return }
来源：http://men.jyoumei.cn

Ruby: return if data.nil?
来源：http://axn.smart0.xyz

C#:   if (data == null) return;
来源：http://gbd.cashguo.top

================================================================================
来源：http://wrq.zdqjudy.top

C. 函数与作用域
来源：http://ibo.feifeiyinyue.top

================================================================================
来源：http://lgr.jqgufenzy.top

[C01] 定义函数
来源：http://hhw.snrcjt.cn

Py:   def add(a, b): return a + b
来源：http://rmj.yongpay.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://syy.ivvv.top

JS:   function add(a, b) { return a + b; }
来源：http://csa.zycfv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tzz.tarul.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ezd.havefunace.top

Go:   func add(a, b int) int { return a + b }
来源：http://zuk.iojbl.cn

Ruby: def add(a, b); a + b; end
来源：http://eja.jinqigfzy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yfi.svipenyu.cn

[C02] 默认参数
来源：http://ofe.52xcode.cn

Py:   def greet(name="World"): return name
来源：http://puj.yongpay.top

PHP:  function greet($name = "World") { return $name; }
来源：http://juz.52xcode.cn

JS:   function greet(name = "World") { return name; }
来源：http://wry.pengpengdd.cyou

TS:   function greet(name: string = "World") { return name; }
来源：http://zda.xinyue.icu

Java: // 无默认参数：方法重载或 Optional
来源：http://rkx.yuxming.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lof.xuetiantiany.cn

Ruby: def greet(name = "World") = name
来源：http://asc.0kj1m.cn

C#:   string Greet(string name = "World") => name;
来源：http://kyb.zhixingplan.top

[C03] 可变参数
来源：http://ngc.gogol.net.cn

Py:   def total(*args): return sum(args)
来源：http://zlt.zycfv.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zfs.hesvh.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hxs.yuanzhike.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lzg.yfazqb.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kpu.birdmap.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nug.hcnkem.com

Ruby: def total(*nums); nums.sum; end
来源：http://uad.svipenyu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ren.daria6918.cn

[C04] 命名参数 / 关键字参数
来源：http://wpq.sxryk.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gzq.haohaochexian.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ddo.jinqigufen.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qdi.yanxiufei.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pmd.fengsongda.top

Java: // 无：用 Builder 模式或 record
来源：http://hdf.snrcjt.cn

Go:   // 无：用配置结构体参数
来源：http://zct.zycfv.cn

Ruby: f(a: 1, b: 2)
来源：http://qjv.yj20258888.top

C#:   f(a: 1, b: 2)
来源：http://mde.hesvh.cn

[C05] 返回多个值
来源：http://wby.gogol.net.cn

Py:   return a, b
来源：http://bte.cdnleiting.top

PHP:  return [$a, $b];
来源：http://bju.hnqzz.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ypv.jqgufenzy.top

TS:   return { a, b };
来源：http://fmo.redwolf501.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ezp.dianchejie.cn

Go:   return a, b
来源：http://wbj.cucudq.cn

Ruby: return a, b
来源：http://ttk.jqgufenzy.top

C#:   return (a, b);              // ValueTuple
来源：http://yrv.sjlbkw.cn

[C06] 匿名函数 / lambda
来源：http://xzj.ehwqpu.com

Py:   square = lambda x: x * x
来源：http://ioh.yfazqb.com

PHP:  $square = fn($x) => $x * $x;
来源：http://frq.sysykeji.top

JS:   const square = x => x * x;
来源：http://gxa.dashuyun.cn

TS:   const square = (x: number): number => x * x;
来源：http://pcc.andypj.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ebe.zhengqikj.top

Go:   sq := func(x int) int { return x * x }
来源：http://ame.ywan-chungtsiang.top

Ruby: square = ->(x) { x * x }
来源：http://qpc.jqgfzy.top

C#:   Func<int, int> square = x => x * x;
来源：http://nsk.ywan-chungtsiang.top

[C07] 把函数作为参数传入
来源：http://cga.sufxvd.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bsj.sxryk.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jcn.sjlbkw.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nfl.redwolf501.top

TS:   arr.map(String)
来源：http://ged.chenlongwang.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pwl.hnqzz.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ujt.meibo888.top

Ruby: arr.map(&:upcase)
来源：http://nea.dashuyun.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://pjk.yj20258888.top

[C08] 闭包
来源：http://nws.yongpay.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ken.9152youxi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vfm.mhx1999.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wst.haohaochexian.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gbc.jinyuanbaomall.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://npf.nwbrower.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rxz.smart0.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jwv.yj20258888.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bir.0kj1m.cn

[C09] 递归
来源：http://lge.kuanghao11.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://trw.nanxuanxn.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vyl.quarkkingdee.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cco.nanxuanxn.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uux.yj20258888.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lwl.wangshuangyany.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://csg.svipenyu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bqg.zhaomingkeji.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wct.hesvh.cn

[C10] 变量作用域
来源：http://uky.tarul.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nix.yueranfly.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vjv.ybcxt.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kth.shanyushiyangtech.top

TS:   同 JS
来源：http://omz.hnqzz.top

Java: 方法内为块级作用域
来源：http://iit.ivvv.top

Go:   花括号块级作用域
来源：http://inn.ctjpmb.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nvs.cashguo.top

C#:   块级作用域
来源：http://ies.zhiwuduotai.top

[C11] 模块导入与导出
来源：http://vzi.c1oappe.top

Py:   from module import func
来源：http://pld.cheryme.top

PHP:  require "file.php";  或 use App\Service;
来源：http://rpf.andypj.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://yqx.uphjek.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qfl.nwbrower.top

Java: import java.util.List;
来源：http://xth.ydzc1.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://csk.haohaochexian.top

Ruby: require "json"; require_relative "./util"
来源：http://hkt.andypj.xyz

C#:   using System.Text;
来源：http://uto.ywan-chungtsiang.top

[C12] 立即执行函数 IIFE
来源：http://idh.hcnkem.com

Py:   (lambda: print("run"))()
来源：http://bif.andypj.xyz

PHP:  (function () { echo "run"; })();
来源：http://xct.ivvv.top

JS:   (() => { console.log("run"); })();
来源：http://any.jinqigufen.top

TS:   (() => { console.log("run"); })();
来源：http://yzz.cqqwz.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kpe.dashuyun.cn

Go:   func() { fmt.Println("run") }()
来源：http://qfr.zdbjq.cn

Ruby: -> { puts "run" }.call
来源：http://zzt.smart0.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://fdc.gaohongyu789.top

[C13] 类型声明 / 类型注解
来源：http://aul.hysaishi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bdi.wangshuangyany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mhc.jinqigfzy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tlj.zhengqikj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fcf.quarkkingdee.top

Java: int add(int a, int b) { return a + b; }
来源：http://toq.zhixingplan.top

Go:   func add(a, b int) int
来源：http://jco.shanyushiyangkeji.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://smm.vehdjk.com

C#:   int Add(int a, int b) => a + b;
来源：http://evl.jinyuanbaomall.cn

[C14] 泛型函数
来源：http://prk.hammf.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ity.ydjk.org.cn

PHP:  // 无泛型
来源：http://fyc.aibaodan.cn

JS:   // 无泛型
来源：http://zfj.hammf.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://brk.svipenyu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://opo.yfazqb.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ekr.epnwcf.com

Ruby: # 无泛型
来源：http://kch.daria6918.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jsy.nwbrower.top

[C15] 解构 / 展开参数
来源：http://ums.iojbl.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yvk.ydjk.org.cn

PHP:  [$a, $b] = $pair;
来源：http://czv.cdnleiting.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hbr.hesvh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://aqz.ehwqpu.com

Java: // 无解构
来源：http://kuy.jyoumei.cn

Go:   // 无解构
来源：http://txd.sxryk.cn

Ruby: a, b = pair
来源：http://dnx.cheryme.top

C#:   var (a, b) = pair;
来源：http://jbe.zhoulong.xyz

[C16] 函数 / 方法重载
来源：http://uov.aizwys.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zau.0kj1m.cn

PHP:  // 无重载
来源：http://kyc.kuanghao11.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://utz.dashuyun.cn

TS:   // 用联合类型或重载签名声明
来源：http://mzz.chenjidiqi.icu

Java: void f(int a) {}  void f(String a) {}
来源：http://egc.wangshuangyany.cn

Go:   // 无重载：用不同函数名
来源：http://wkw.hcnkem.com

Ruby: # 无重载：靠动态参数
来源：http://shl.zdqjudy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://llt.yj20258888.top

================================================================================
来源：http://wdl.aibaodan.cn

D. 数组 / 列表 / 集合
来源：http://wss.yangfankeji.com

================================================================================
来源：http://qod.wangdashe.top

[D01] 创建数组 / 列表
来源：http://kvn.yj202588.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://fdr.gzhubu.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://khd.c1oappe.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dqb.sweek.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://bhz.gzhubu.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ave.hywenlv.cn

Go:   arr := []int{1, 2, 3}
来源：http://pkb.meibo888.top

Ruby: arr = [1, 2, 3]
来源：http://fit.zhengqikj.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nau.vqdsnc.cn

[D02] 追加元素到末尾
来源：http://cka.jinqigufen.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sge.guannengcc.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jfe.vqdsnc.cn

JS:   arr.push(4);
来源：http://ach.fehbvm.com

TS:   arr.push(4);
来源：http://vvm.guowangkeji.top

Java: list.add(4);
来源：http://kdi.yj20258.top

Go:   arr = append(arr, 4)
来源：http://kyl.mhx1999.top

Ruby: arr << 4; arr.push(5)
来源：http://zka.nanxinkj.top

C#:   list.Add(4);
来源：http://fzr.haohaochexian.top

[D03] 在指定位置插入元素
来源：http://aot.hywenlv.cn

Py:   arr.insert(0, 0)
来源：http://dig.cashguo.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://phd.cdnleiting.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sab.jinghuilouyu.cn

TS:   arr.splice(0, 0, 0);
来源：http://ffe.yfazqb.com

Java: list.add(0, 0);
来源：http://chc.zhoulong.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://jhh.havefunace.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://trr.cheryme.top

C#:   list.Insert(0, 0);
来源：http://vvi.shzxlz.cn

[D04] 删除元素
来源：http://qdz.xingfuxueyuan.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pfa.c1oappe.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ahk.gaohongyu789.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://flr.dianchejie.cn

TS:   arr.splice(0, 1);
来源：http://scp.chenlongwang.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://adf.fzhhl.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zlx.kuanghao11.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://leh.cdnleiting.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wmv.bjfxy.top

[D05] 访问与修改元素
来源：http://tej.smart0.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rey.fanxiaobao.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://eaj.jqgufenzy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mue.zdbjq.cn

TS:   arr[0]; arr.at(-1);
来源：http://iya.c1oappe.top

Java: list.get(0); list.set(0, 9);
来源：http://moj.hnxiangtu.top

Go:   arr[0]; arr[0] = 9
来源：http://wdc.sufxvd.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vvd.sxryk.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lad.hysaishi.cn

[D06] 数组长度
来源：http://zfp.yj202588.top

Py:   len(arr)
来源：http://mzf.jinqigufen.top

PHP:  count($arr);
来源：http://ovl.fengsongda.top

JS:   arr.length
来源：http://zpk.haohaochexian.top

TS:   arr.length
来源：http://lyv.zhongyouzk.top

Java: list.size();
来源：http://qzk.svipenyu.cn

Go:   len(arr)
来源：http://txf.zhongyouzk.top

Ruby: arr.length; arr.size
来源：http://mar.hywenlv.cn

C#:   list.Count;
来源：http://pjo.ybcxt.top

[D07] 切片 / 取子数组
来源：http://heu.chenjidiqi.icu

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pup.snrcjt.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zry.iojbl.cn

JS:   arr.slice(1, 4);
来源：http://tig.fzhhl.top

TS:   arr.slice(1, 4);
来源：http://jft.fzhhl.top

Java: list.subList(1, 4);
来源：http://opw.shanyushiyangtech.top

Go:   arr[1:4]
来源：http://wbl.yfazqb.com

Ruby: arr[1, 3]
来源：http://vzg.chenlongwang.top

C#:   list.GetRange(1, 3);
来源：http://bcj.yj20258888.top

[D08] 合并两个数组
来源：http://ryv.ywan-chungtsiang.top

Py:   a + b;  a.extend(b)
来源：http://ymr.sweek.top

PHP:  array_merge($a, $b);
来源：http://zqw.jinqigufen.top

JS:   [...a, ...b];  a.concat(b);
来源：http://zxt.ppjwa.cn

TS:   [...a, ...b];
来源：http://jwd.guowangkeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qxc.gogol.net.cn

Go:   append(a, b...)
来源：http://rnh.cucudq.cn

Ruby: a + b;  a.concat(b)
来源：http://igt.gotoacloud.top

C#:   a.Concat(b).ToList()
来源：http://bdv.jyoumei.cn

[D09] 排序（升序）
来源：http://rdu.hnxiangtu.top

Py:   sorted(arr);  arr.sort()
来源：http://mfs.9152youxi.cn

PHP:  sort($arr);
来源：http://wfn.jqgfzy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zna.jinqigfzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://iwf.jqgfzy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ewi.iojbl.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://znk.9152youxi.cn

Ruby: arr.sort
来源：http://gok.sweek.top

C#:   list.Sort();
来源：http://jyb.aibaodan.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://kpb.sweek.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sey.birdmap.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dax.xylfe.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hva.chenlongwang.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fcp.ybcxt.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://eyd.meibo888.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rks.dianchejie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sog.quarkkingdee.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vke.ydjk.org.cn

[D11] 反转数组
来源：http://mtr.wangshuangyany.cn

Py:   arr[::-1];  arr.reverse()
来源：http://eec.yongpay.top

PHP:  array_reverse($arr);
来源：http://lvh.yuxming.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://crx.yanxiufei.cn

TS:   [...arr].reverse();
来源：http://byg.snrcjt.cn

Java: Collections.reverse(list);
来源：http://mcd.ydjk.org.cn

Go:   slices.Reverse(arr)
来源：http://cwb.zhixingplan.top

Ruby: arr.reverse
来源：http://zdi.xziqi.cn

C#:   list.Reverse();
来源：http://lgi.zhoulong.xyz

[D12] 查找元素下标
来源：http://yah.hnxiangtu.top

Py:   arr.index(x);  x in arr
来源：http://kvi.0kj1m.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bdt.sufxvd.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pfj.hongshengwenyu.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pfk.gzhubu.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xwz.jlsjyb.cn

Go:   slices.Index(arr, x)
来源：http://qga.zhijiandao.cn


<!-- 参考信息 -->