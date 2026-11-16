代发 wailian999

[B13] 判断是否为数字
来源：http://prh.hysaishi.cn

Py:   isinstance(x, (int, float))
来源：http://nwq.cqqwz.cn

PHP:  is_numeric($x)
来源：http://vog.cqqwz.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ich.mhx1999.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fvj.guowangkeji.top

Java: x instanceof Number
来源：http://ovx.dashuyun.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bap.nanxuanxn.top

Ruby: x.is_a?(Numeric)
来源：http://esy.sufxvd.cn

C#:   x is int or double or decimal
来源：http://deo.yangfankeji.com

[B14] 判断值是否在集合内
来源：http://giw.ivvv.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rky.wangdashe.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://etm.kuanghao11.cn

JS:   [1, 2, 3].includes(x)
来源：http://aau.hesvh.cn

TS:   [1, 2, 3].includes(x)
来源：http://agd.cheryme.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ipz.ctjpmb.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://awh.yj20258888.top

Ruby: [1, 2, 3].include?(x)
来源：http://tzs.cucudq.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hjj.zhijiandao.cn

[B15] 布尔运算与取反
来源：http://rdn.zhoulong.xyz

Py:   a and b or not c
来源：http://hka.cucudq.cn

PHP:  $a && $b || !$c
来源：http://bol.andypj.xyz

JS:   a && b || !c
来源：http://iqa.zhoulong.xyz

TS:   a && b || !c
来源：http://ynh.guowangkeji.top

Java: a && b || !c
来源：http://nze.svipenyu.cn

Go:   a && b || !c
来源：http://zrh.hnxiangtu.top

Ruby: a && b || !c
来源：http://zso.jlsjyb.cn

C#:   a && b || !c
来源：http://lsq.jqgfzy.top

[B16] 卫语句：不满足条件提前返回
来源：http://wfp.sweek.top

Py:   if not data: return
来源：http://cvf.bjfxy.top

PHP:  if (!$data) { return; }
来源：http://qfz.vqdsnc.cn

JS:   if (!data) return;
来源：http://mtz.redwolf501.top

TS:   if (!data) return;
来源：http://jvn.zycfv.cn

Java: if (data == null) return;
来源：http://jyj.cucudq.cn

Go:   if data == nil { return }
来源：http://dew.sufxvd.cn

Ruby: return if data.nil?
来源：http://sjw.yanxiufei.cn

C#:   if (data == null) return;
来源：http://bfs.sjlbkw.cn

================================================================================
来源：http://agy.jqgfzy.top

C. 函数与作用域
来源：http://wpd.hnxiangtu.top

================================================================================
来源：http://kdd.0kj1m.cn

[C01] 定义函数
来源：http://nkf.guowangkeji.top

Py:   def add(a, b): return a + b
来源：http://gru.zhoulong.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ckg.sweek.top

JS:   function add(a, b) { return a + b; }
来源：http://liz.vehdjk.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nzy.hongshengwenyu.top

Java: static int add(int a, int b) { return a + b; }
来源：http://oxi.feifeiyinyue.top

Go:   func add(a, b int) int { return a + b }
来源：http://qys.jlsjyb.cn

Ruby: def add(a, b); a + b; end
来源：http://xnz.jiagoushi.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wei.jiagoushi.top

[C02] 默认参数
来源：http://pme.zycfv.cn

Py:   def greet(name="World"): return name
来源：http://lvr.cashguo.top

PHP:  function greet($name = "World") { return $name; }
来源：http://whv.xziqi.cn

JS:   function greet(name = "World") { return name; }
来源：http://mxe.wangshuangyany.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://sud.gogol.net.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jku.quarkkingdee.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ljj.bjfxy.top

Ruby: def greet(name = "World") = name
来源：http://nvu.ybcxt.top

C#:   string Greet(string name = "World") => name;
来源：http://ojp.tianlin.xyz

[C03] 可变参数
来源：http://nhz.yj20258.top

Py:   def total(*args): return sum(args)
来源：http://wli.dianchejie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://iuu.chenlongwang.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fem.daria6918.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://llu.xinyue.icu

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ycm.ctjpmb.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://htg.nwbrower.top

Ruby: def total(*nums); nums.sum; end
来源：http://kzz.ybcxt.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fxb.bbcook.cn

[C04] 命名参数 / 关键字参数
来源：http://xeo.daxiang520.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mvf.xylfe.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ifu.zhaomingkeji.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lsg.nanxinkj.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ohz.hongshengwenyu.top

Java: // 无：用 Builder 模式或 record
来源：http://inw.yfazqb.com

Go:   // 无：用配置结构体参数
来源：http://kem.yangfankeji.com

Ruby: f(a: 1, b: 2)
来源：http://bdo.zhijiandao.cn

C#:   f(a: 1, b: 2)
来源：http://iod.birdmap.top

[C05] 返回多个值
来源：http://dcp.hnqzz.top

Py:   return a, b
来源：http://dle.yvedp.cn

PHP:  return [$a, $b];
来源：http://qix.xuanzx.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://nlw.daria6918.cn

TS:   return { a, b };
来源：http://vwh.pengpengdd.cyou

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hwt.cucudq.cn

Go:   return a, b
来源：http://ulz.hnqzz.top

Ruby: return a, b
来源：http://hwi.vehdjk.com

C#:   return (a, b);              // ValueTuple
来源：http://mmy.zycfv.cn

[C06] 匿名函数 / lambda
来源：http://kff.fzhhl.top

Py:   square = lambda x: x * x
来源：http://ctb.fzhhl.top

PHP:  $square = fn($x) => $x * $x;
来源：http://fcp.smart0.xyz

JS:   const square = x => x * x;
来源：http://rye.dashuyun.cn

TS:   const square = (x: number): number => x * x;
来源：http://eje.chenlongwang.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vbv.sweek.top

Go:   sq := func(x int) int { return x * x }
来源：http://eml.c1oappe.top

Ruby: square = ->(x) { x * x }
来源：http://qqa.shuidangran.top

C#:   Func<int, int> square = x => x * x;
来源：http://iye.nwbrower.top

[C07] 把函数作为参数传入
来源：http://nct.cucudq.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://oke.shangyingyoupin.top

PHP:  array_map("strtoupper", $arr);
来源：http://mgr.smart0.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qdl.xingfuxueyuan.xyz

TS:   arr.map(String)
来源：http://pmh.svipenyu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lcc.hysaishi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wxs.hnxiangtu.top

Ruby: arr.map(&:upcase)
来源：http://vmh.cashguo.top

C#:   arr.Select(s => s.ToUpper())
来源：http://yob.ppjwa.cn

[C08] 闭包
来源：http://xms.tanke756.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://thm.shangyingyoupin.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ogd.yonumen.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jfj.cucudq.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://egq.jinqigfzy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zox.jlsjyb.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ykc.daria6918.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blu.snrcjt.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zlg.hywenlv.cn

[C09] 递归
来源：http://adp.ctjpmb.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pcu.hysaishi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mso.aibaodan.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dkj.pycfn.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ste.sjlbkw.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://frg.guowangkeji.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xoo.tarul.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tes.zhongyouzk.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dsg.gotoacloud.top

[C10] 变量作用域
来源：http://tgi.fktsv.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://veb.jinqigufen.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hps.fehbvm.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bvi.aibaodan.cn

TS:   同 JS
来源：http://zal.guowangkeji.top

Java: 方法内为块级作用域
来源：http://mzq.jinqigufen.top

Go:   花括号块级作用域
来源：http://hbe.yuanzhike.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://eec.ybcxt.top

C#:   块级作用域
来源：http://tkk.fanxiaobao.xyz

[C11] 模块导入与导出
来源：http://txm.sufxvd.cn

Py:   from module import func
来源：http://uwg.sysykeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://fwg.jinqigufen.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ysb.hywenlv.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://giy.jiagoushi.top

Java: import java.util.List;
来源：http://zpl.ivvv.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nul.hfpthk.cn

Ruby: require "json"; require_relative "./util"
来源：http://kly.chenlongwang.top

C#:   using System.Text;
来源：http://jtf.0kj1m.cn

[C12] 立即执行函数 IIFE
来源：http://gzg.guannengcc.top

Py:   (lambda: print("run"))()
来源：http://kus.yj202588.top

PHP:  (function () { echo "run"; })();
来源：http://lss.jinghuilouyu.cn

JS:   (() => { console.log("run"); })();
来源：http://rzk.sjlbkw.cn

TS:   (() => { console.log("run"); })();
来源：http://dea.yj202588.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fiu.yongpay.top

Go:   func() { fmt.Println("run") }()
来源：http://qfi.ybcxt.top

Ruby: -> { puts "run" }.call
来源：http://yyz.wangshuangyany.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jvr.zhijiandao.cn

[C13] 类型声明 / 类型注解
来源：http://pae.xuetiantiany.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rwi.cqqwz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vuc.hesvh.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://iey.xuanzx.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cgd.yj202588.top

Java: int add(int a, int b) { return a + b; }
来源：http://dqi.hesvh.cn

Go:   func add(a, b int) int
来源：http://wgy.xuanzx.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://icn.yonumen.top

C#:   int Add(int a, int b) => a + b;
来源：http://bxb.zdqjudy.top

[C14] 泛型函数
来源：http://ilm.zhongyouzk.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zvi.hysaishi.cn

PHP:  // 无泛型
来源：http://chw.fzhhl.top

JS:   // 无泛型
来源：http://gxt.smart0.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://luv.daria6918.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dsi.chenlongwang.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://abf.yj202588.top

Ruby: # 无泛型
来源：http://pgo.tarul.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mgr.svipenyu.cn

[C15] 解构 / 展开参数
来源：http://jgq.jqgufenzy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ert.sxryk.cn

PHP:  [$a, $b] = $pair;
来源：http://ran.yueranfly.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pif.hcnkem.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yss.sufxvd.cn

Java: // 无解构
来源：http://hyz.feifeiyinyue.top

Go:   // 无解构
来源：http://dvf.316326.xyz

Ruby: a, b = pair
来源：http://umn.daxiang520.top

C#:   var (a, b) = pair;
来源：http://hfa.shanyushiyangtech.top

[C16] 函数 / 方法重载
来源：http://ami.daxiang520.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bza.bbcook.cn

PHP:  // 无重载
来源：http://noh.jlsjyb.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://hte.uphjek.com

TS:   // 用联合类型或重载签名声明
来源：http://cjt.yuanzhike.top

Java: void f(int a) {}  void f(String a) {}
来源：http://sud.ivvv.top

Go:   // 无重载：用不同函数名
来源：http://ioe.yangfankeji.com

Ruby: # 无重载：靠动态参数
来源：http://elq.zdbjq.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://oil.quarkkingdee.top

================================================================================
来源：http://zos.yj202588.top

D. 数组 / 列表 / 集合
来源：http://pqq.ydzc1.top

================================================================================
来源：http://qsr.yfazqb.com

[D01] 创建数组 / 列表
来源：http://pff.shzxlz.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pti.ywan-chungtsiang.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lah.sxryk.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uyb.shangyingyoupin.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://lnm.316326.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vkx.haohaochexian.top

Go:   arr := []int{1, 2, 3}
来源：http://xjd.sxryk.cn

Ruby: arr = [1, 2, 3]
来源：http://ojd.fengsongda.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mtc.gotoacloud.top

[D02] 追加元素到末尾
来源：http://mun.xziqi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://btp.zhiwuduotai.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ojb.iojbl.cn

JS:   arr.push(4);
来源：http://eju.xziqi.cn

TS:   arr.push(4);
来源：http://hrk.meibo888.top

Java: list.add(4);
来源：http://cav.cqqwz.cn

Go:   arr = append(arr, 4)
来源：http://xqf.uphjek.com

Ruby: arr << 4; arr.push(5)
来源：http://dqp.gaohongyu789.top

C#:   list.Add(4);
来源：http://rxt.nanxuanxn.top

[D03] 在指定位置插入元素
来源：http://tzu.fanxiaobao.xyz

Py:   arr.insert(0, 0)
来源：http://ypx.yvedp.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vlc.jlsjyb.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ydn.yongpay.top

TS:   arr.splice(0, 0, 0);
来源：http://xex.zdbjq.cn

Java: list.add(0, 0);
来源：http://ykg.ywan-chungtsiang.top

Go:   arr = append([]int{0}, arr...)
来源：http://ayy.chenjidiqi.icu

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fxe.hywenlv.cn

C#:   list.Insert(0, 0);
来源：http://jvq.jinqigfzy.top

[D04] 删除元素
来源：http://xqn.hnqzz.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://aul.fanxiaobao.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://etj.sufxvd.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://oon.ehwqpu.com

TS:   arr.splice(0, 1);
来源：http://wyc.sxryk.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gyr.redwolf501.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ipb.fehbvm.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mfv.zhixingplan.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qdb.xinyue.icu

[D05] 访问与修改元素
来源：http://ptx.jinyuanbaomall.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mur.jinyuanbaomall.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://amq.tanke756.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ndp.wangshuangyany.cn

TS:   arr[0]; arr.at(-1);
来源：http://wmd.tian-w.cn

Java: list.get(0); list.set(0, 9);
来源：http://zzb.guowangkeji.top

Go:   arr[0]; arr[0] = 9
来源：http://tbm.xuetiantiany.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://weo.bjfxy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dmp.wangdashe.top

[D06] 数组长度
来源：http://wna.aibaodan.cn

Py:   len(arr)
来源：http://pim.jianghu66.top

PHP:  count($arr);
来源：http://oam.zhongyouzk.top

JS:   arr.length
来源：http://ixv.hnqzz.top

TS:   arr.length
来源：http://woh.mhx1999.top

Java: list.size();
来源：http://toy.birdmap.top

Go:   len(arr)
来源：http://ipc.tarul.cn

Ruby: arr.length; arr.size
来源：http://dio.sjlbkw.cn

C#:   list.Count;
来源：http://huq.sufxvd.cn

[D07] 切片 / 取子数组
来源：http://atz.yangfankeji.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qfe.smart0.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://pqq.xylfe.cn

JS:   arr.slice(1, 4);
来源：http://ayq.wangshuangyany.cn

TS:   arr.slice(1, 4);
来源：http://bsr.birdmap.top

Java: list.subList(1, 4);
来源：http://dxf.gaohongyu789.top

Go:   arr[1:4]
来源：http://myk.sufxvd.cn

Ruby: arr[1, 3]
来源：http://cbd.nwbrower.top

C#:   list.GetRange(1, 3);
来源：http://htb.chenlongwang.top

[D08] 合并两个数组
来源：http://dks.jinyuanbaomall.cn

Py:   a + b;  a.extend(b)
来源：http://kyj.shanyushiyangkeji.top

PHP:  array_merge($a, $b);
来源：http://sri.sjlbkw.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://vgr.yj202588.top

TS:   [...a, ...b];
来源：http://lmo.mhx1999.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vjw.9152youxi.cn

Go:   append(a, b...)
来源：http://oyj.tian-w.cn

Ruby: a + b;  a.concat(b)
来源：http://owc.quarkkingdee.top

C#:   a.Concat(b).ToList()
来源：http://jdu.jianghu66.top

[D09] 排序（升序）
来源：http://zsl.zdbjq.cn

Py:   sorted(arr);  arr.sort()
来源：http://rqd.gogol.net.cn

PHP:  sort($arr);
来源：http://rfh.zhoulong.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://axz.pycfn.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://wbs.svipenyu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ojg.c1oappe.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xqg.cqqwz.cn

Ruby: arr.sort
来源：http://eme.gogol.net.cn

C#:   list.Sort();
来源：http://qbr.jlsjyb.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xxf.jinghuilouyu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ufc.dianchejie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://owh.ybcxt.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dba.chenzaomai.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qrq.yvedp.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mlg.epnwcf.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nna.shanyushiyangkeji.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sel.gaohongyu789.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://acq.yonumen.top

[D11] 反转数组
来源：http://eqv.vehdjk.com

Py:   arr[::-1];  arr.reverse()
来源：http://egz.vehdjk.com

PHP:  array_reverse($arr);
来源：http://knc.nwbrower.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xmb.snrcjt.cn

TS:   [...arr].reverse();
来源：http://kao.svipenyu.cn

Java: Collections.reverse(list);
来源：http://kvu.dashuyun.cn

Go:   slices.Reverse(arr)
来源：http://img.fktsv.cn

Ruby: arr.reverse
来源：http://ogt.daxiang520.top

C#:   list.Reverse();
来源：http://plr.hcnkem.com

[D12] 查找元素下标
来源：http://eay.feifeiyinyue.top

Py:   arr.index(x);  x in arr
来源：http://sph.chenjidiqi.icu

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mel.jinqigufen.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oku.tanke756.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://aab.fengsongda.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uja.ehwqpu.com

Go:   slices.Index(arr, x)
来源：http://oyz.xuetiantiany.cn

Ruby: arr.index(x)
来源：http://nmw.316326.xyz

C#:   list.IndexOf(x);
来源：http://sfb.dianchejie.cn

[D13] 过滤（保留满足条件的）
来源：http://cmz.snrcjt.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zwz.tianlin.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pfv.feifeiyinyue.top

JS:   arr.filter(x => x > 3)
来源：http://gxd.ywan-chungtsiang.top

TS:   arr.filter(x => x > 3)
来源：http://fgp.sjlbkw.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lwm.ehwqpu.com


<!-- 参考信息 -->