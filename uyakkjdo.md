代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://ahp.tarul.cn

TS:   [1, 2, 3].includes(x)
来源：http://yxr.havefunace.top

Java: List.of(1, 2, 3).contains(x)
来源：http://bui.nanxinkj.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://oqy.cheryme.top

Ruby: [1, 2, 3].include?(x)
来源：http://ibm.ybcxt.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vmf.bjfxy.top

[B15] 布尔运算与取反
来源：http://qto.316326.xyz

Py:   a and b or not c
来源：http://lho.jinyuanbaomall.cn

PHP:  $a && $b || !$c
来源：http://jee.ywan-chungtsiang.top

JS:   a && b || !c
来源：http://xkn.meibo888.top

TS:   a && b || !c
来源：http://qrf.tarul.cn

Java: a && b || !c
来源：http://hyq.hysaishi.cn

Go:   a && b || !c
来源：http://pxu.gzhubu.top

Ruby: a && b || !c
来源：http://sne.sweek.top

C#:   a && b || !c
来源：http://ayh.chenlongwang.top

[B16] 卫语句：不满足条件提前返回
来源：http://dfk.hnqzz.top

Py:   if not data: return
来源：http://arv.ywan-chungtsiang.top

PHP:  if (!$data) { return; }
来源：http://ryf.hesvh.cn

JS:   if (!data) return;
来源：http://tkq.cheryme.top

TS:   if (!data) return;
来源：http://yod.zdbjq.cn

Java: if (data == null) return;
来源：http://hqk.jinghuilouyu.cn

Go:   if data == nil { return }
来源：http://mel.sxryk.cn

Ruby: return if data.nil?
来源：http://ebp.hongshengwenyu.top

C#:   if (data == null) return;
来源：http://usg.xingfuxueyuan.xyz

================================================================================
来源：http://sre.shuidangran.top

C. 函数与作用域
来源：http://pgo.fehbvm.com

================================================================================
来源：http://ehc.tian-w.cn

[C01] 定义函数
来源：http://yuz.fzhhl.top

Py:   def add(a, b): return a + b
来源：http://mri.yangfankeji.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://umb.chenzaomai.com

JS:   function add(a, b) { return a + b; }
来源：http://yzl.redwolf501.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xry.hfpthk.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xxf.ivvv.top

Go:   func add(a, b int) int { return a + b }
来源：http://fgj.xylfe.cn

Ruby: def add(a, b); a + b; end
来源：http://pxl.jiagoushi.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kss.jianghu66.top

[C02] 默认参数
来源：http://ozk.jqgfzy.top

Py:   def greet(name="World"): return name
来源：http://xzv.jiagoushi.top

PHP:  function greet($name = "World") { return $name; }
来源：http://prg.jlsjyb.cn

JS:   function greet(name = "World") { return name; }
来源：http://cry.ppjwa.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://grv.hammf.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://lou.cqqwz.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zmn.xziqi.cn

Ruby: def greet(name = "World") = name
来源：http://rtj.aibaodan.cn

C#:   string Greet(string name = "World") => name;
来源：http://uhe.yanxiufei.cn

[C03] 可变参数
来源：http://bnk.chenjidiqi.icu

Py:   def total(*args): return sum(args)
来源：http://ztw.sweek.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xjo.xuanzx.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sez.tian-w.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://clm.yanxiufei.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qte.epnwcf.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mjw.hywenlv.cn

Ruby: def total(*nums); nums.sum; end
来源：http://css.vqdsnc.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ram.jinyuanbaomall.cn

[C04] 命名参数 / 关键字参数
来源：http://srx.zhaomingkeji.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uww.jinqigufen.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kro.svipenyu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qho.zdqjudy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wcj.tanke756.top

Java: // 无：用 Builder 模式或 record
来源：http://ekr.pycfn.com

Go:   // 无：用配置结构体参数
来源：http://nwp.redwolf501.top

Ruby: f(a: 1, b: 2)
来源：http://dmd.hammf.cn

C#:   f(a: 1, b: 2)
来源：http://ugp.tian-w.cn

[C05] 返回多个值
来源：http://yei.daria6918.cn

Py:   return a, b
来源：http://qep.ydzc1.top

PHP:  return [$a, $b];
来源：http://uoj.chenlongwang.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://esf.yuxming.cn

TS:   return { a, b };
来源：http://grz.gotoacloud.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mtp.feifeiyinyue.top

Go:   return a, b
来源：http://tvy.chenjidiqi.icu

Ruby: return a, b
来源：http://lex.ybcxt.top

C#:   return (a, b);              // ValueTuple
来源：http://omw.yj20258.top

[C06] 匿名函数 / lambda
来源：http://wme.hnqzz.top

Py:   square = lambda x: x * x
来源：http://apz.zhixingplan.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ovu.meibo888.top

JS:   const square = x => x * x;
来源：http://ajl.zhaomingkeji.xyz

TS:   const square = (x: number): number => x * x;
来源：http://qjo.hnqzz.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://moi.smart0.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://zny.tarul.cn

Ruby: square = ->(x) { x * x }
来源：http://adt.shanyushiyangkeji.top

C#:   Func<int, int> square = x => x * x;
来源：http://ldx.zhixingplan.top

[C07] 把函数作为参数传入
来源：http://oae.jinyuanbaomall.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wsh.fzhhl.top

PHP:  array_map("strtoupper", $arr);
来源：http://ofw.chenzaomai.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gid.xuetiantiany.cn

TS:   arr.map(String)
来源：http://cwb.yj20258888.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lwy.zhijiandao.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zvb.yangfankeji.com

Ruby: arr.map(&:upcase)
来源：http://ttb.sysykeji.top

C#:   arr.Select(s => s.ToUpper())
来源：http://rlc.hywenlv.cn

[C08] 闭包
来源：http://lrn.dashuyun.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gag.hammf.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wvb.yangfankeji.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://quw.shangyingyoupin.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fno.birdmap.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sem.dashuyun.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://avx.gzhubu.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wlc.gotoacloud.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://msl.jinqigfzy.top

[C09] 递归
来源：http://yxl.zhengqikj.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://guh.tarul.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dof.yj20258.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tqh.jinyuanbaomall.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oxp.ydjk.org.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://twt.zdqjudy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jll.zhaomingkeji.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://irc.xylfe.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hbk.ydjk.org.cn

[C10] 变量作用域
来源：http://wwb.dianchejie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://djj.c1oappe.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vpp.hnqzz.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zni.jyoumei.cn

TS:   同 JS
来源：http://nxk.yuanzhike.top

Java: 方法内为块级作用域
来源：http://iuh.zhoulong.xyz

Go:   花括号块级作用域
来源：http://qpa.sufxvd.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wod.gaohongyu789.top

C#:   块级作用域
来源：http://ziw.xinyue.icu

[C11] 模块导入与导出
来源：http://iiw.zhaomingkeji.xyz

Py:   from module import func
来源：http://ewt.smart0.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://das.zhijiandao.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://tux.svipenyu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://djl.jinqigfzy.top

Java: import java.util.List;
来源：http://ehm.c1oappe.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jpv.gaohongyu789.top

Ruby: require "json"; require_relative "./util"
来源：http://owq.bbcook.cn

C#:   using System.Text;
来源：http://npl.cqqwz.cn

[C12] 立即执行函数 IIFE
来源：http://jat.redwolf501.top

Py:   (lambda: print("run"))()
来源：http://jvv.quarkkingdee.top

PHP:  (function () { echo "run"; })();
来源：http://dde.chenlongwang.top

JS:   (() => { console.log("run"); })();
来源：http://sst.fzhhl.top

TS:   (() => { console.log("run"); })();
来源：http://ysr.nanxuanxn.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gss.cdnleiting.top

Go:   func() { fmt.Println("run") }()
来源：http://aak.hongshengwenyu.top

Ruby: -> { puts "run" }.call
来源：http://vws.dianchejie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://uwc.chenjidiqi.icu

[C13] 类型声明 / 类型注解
来源：http://lbk.iojbl.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fmi.c1oappe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kyr.andypj.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hcf.zhoulong.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ihd.xuetiantiany.cn

Java: int add(int a, int b) { return a + b; }
来源：http://gmc.xingfuxueyuan.xyz

Go:   func add(a, b int) int
来源：http://tfw.wangshuangyany.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tzg.jinghuilouyu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://gqb.vqdsnc.cn

[C14] 泛型函数
来源：http://wrd.nwbrower.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vbf.kuanghao11.cn

PHP:  // 无泛型
来源：http://wcc.zhijiandao.cn

JS:   // 无泛型
来源：http://tcd.ywan-chungtsiang.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mrl.cucudq.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xwe.sxryk.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ccq.9152youxi.cn

Ruby: # 无泛型
来源：http://zmm.bbcook.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bnr.jqgufenzy.top

[C15] 解构 / 展开参数
来源：http://adq.52xcode.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yss.bjfxy.top

PHP:  [$a, $b] = $pair;
来源：http://frx.hysaishi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kfr.yuanzhike.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ziy.tarul.cn

Java: // 无解构
来源：http://tis.wangdashe.top

Go:   // 无解构
来源：http://vjq.nwbrower.top

Ruby: a, b = pair
来源：http://ttt.vqdsnc.cn

C#:   var (a, b) = pair;
来源：http://sgc.cheryme.top

[C16] 函数 / 方法重载
来源：http://pot.jiagoushi.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jcx.svipenyu.cn

PHP:  // 无重载
来源：http://vwn.feifeiyinyue.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://tnd.xingfuxueyuan.xyz

TS:   // 用联合类型或重载签名声明
来源：http://jek.hnqzz.top

Java: void f(int a) {}  void f(String a) {}
来源：http://hib.feifeiyinyue.top

Go:   // 无重载：用不同函数名
来源：http://rdt.haohaochexian.top

Ruby: # 无重载：靠动态参数
来源：http://hif.xziqi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://jpr.cucudq.cn

================================================================================
来源：http://juk.jianghu66.top

D. 数组 / 列表 / 集合
来源：http://kfm.aizwys.cn

================================================================================
来源：http://nez.ydzc1.top

[D01] 创建数组 / 列表
来源：http://rsm.vehdjk.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://yfg.shangyingyoupin.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gzo.shuidangran.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://djd.chenlongwang.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://rjx.epnwcf.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wcg.zdqjudy.top

Go:   arr := []int{1, 2, 3}
来源：http://mkc.cashguo.top

Ruby: arr = [1, 2, 3]
来源：http://sef.chenjidiqi.icu

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tcs.jlsjyb.cn

[D02] 追加元素到末尾
来源：http://xtv.jianghu66.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ojv.cdnleiting.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cdl.mhx1999.top

JS:   arr.push(4);
来源：http://uak.ywan-chungtsiang.top

TS:   arr.push(4);
来源：http://fel.sjlbkw.cn

Java: list.add(4);
来源：http://ieu.yvedp.cn

Go:   arr = append(arr, 4)
来源：http://txh.havefunace.top

Ruby: arr << 4; arr.push(5)
来源：http://qwd.kuanghao11.cn

C#:   list.Add(4);
来源：http://lxv.jqgfzy.top

[D03] 在指定位置插入元素
来源：http://skd.jqgfzy.top

Py:   arr.insert(0, 0)
来源：http://sok.zhijiandao.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mmi.guannengcc.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ldz.aibaodan.cn

TS:   arr.splice(0, 0, 0);
来源：http://jak.zycfv.cn

Java: list.add(0, 0);
来源：http://zna.zhixingplan.top

Go:   arr = append([]int{0}, arr...)
来源：http://wlw.vqdsnc.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://eos.gogol.net.cn

C#:   list.Insert(0, 0);
来源：http://acn.cqqwz.cn

[D04] 删除元素
来源：http://xrm.sufxvd.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qsf.iojbl.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yzy.zhixingplan.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://noc.hysaishi.cn

TS:   arr.splice(0, 1);
来源：http://txr.ywan-chungtsiang.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mjx.shangyingyoupin.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://thn.cdnleiting.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://eiz.gotoacloud.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ytu.zhiwuduotai.top

[D05] 访问与修改元素
来源：http://pea.smart0.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yqo.vqdsnc.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jtm.birdmap.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ebx.fktsv.cn

TS:   arr[0]; arr.at(-1);
来源：http://avm.vehdjk.com

Java: list.get(0); list.set(0, 9);
来源：http://unp.cucudq.cn

Go:   arr[0]; arr[0] = 9
来源：http://ato.cashguo.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rix.sufxvd.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://erx.wangdashe.top

[D06] 数组长度
来源：http://nlx.sjlbkw.cn

Py:   len(arr)
来源：http://cqx.cqqwz.cn

PHP:  count($arr);
来源：http://jvi.chenzaomai.com

JS:   arr.length
来源：http://jyt.yongpay.top

TS:   arr.length
来源：http://quc.yanxiufei.cn

Java: list.size();
来源：http://vak.jlsjyb.cn

Go:   len(arr)
来源：http://zwi.cqqwz.cn

Ruby: arr.length; arr.size
来源：http://bfe.yj20258888.top

C#:   list.Count;
来源：http://rni.yanxiufei.cn

[D07] 切片 / 取子数组
来源：http://vjo.fengsongda.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vue.zdqjudy.top

PHP:  array_slice($arr, 1, 3);
来源：http://ssz.xingfuxueyuan.xyz

JS:   arr.slice(1, 4);
来源：http://sdw.fengsongda.top

TS:   arr.slice(1, 4);
来源：http://rgf.hnxiangtu.top

Java: list.subList(1, 4);
来源：http://ype.hywenlv.cn

Go:   arr[1:4]
来源：http://meq.bbcook.cn

Ruby: arr[1, 3]
来源：http://yfr.xuanzx.com

C#:   list.GetRange(1, 3);
来源：http://rjk.9152youxi.cn

[D08] 合并两个数组
来源：http://jwh.zycfv.cn

Py:   a + b;  a.extend(b)
来源：http://yrd.gogol.net.cn

PHP:  array_merge($a, $b);
来源：http://xmh.pengpengdd.cyou

JS:   [...a, ...b];  a.concat(b);
来源：http://opo.yfazqb.com

TS:   [...a, ...b];
来源：http://cjr.jinqigufen.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yga.nanxuanxn.top

Go:   append(a, b...)
来源：http://cuq.cheryme.top

Ruby: a + b;  a.concat(b)
来源：http://mhf.jianghu66.top

C#:   a.Concat(b).ToList()
来源：http://hqg.hnxiangtu.top

[D09] 排序（升序）
来源：http://ube.smart0.xyz

Py:   sorted(arr);  arr.sort()
来源：http://xyr.sjlbkw.cn

PHP:  sort($arr);
来源：http://eef.zdbjq.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zll.zhixingplan.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://vzk.andypj.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://ypy.xingfuxueyuan.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ldh.shanyushiyangtech.top

Ruby: arr.sort
来源：http://mhh.iojbl.cn

C#:   list.Sort();
来源：http://bmy.hammf.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ylh.hnxiangtu.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ghn.zhijiandao.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ekw.sysykeji.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kmb.zhengqikj.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://feo.dianchejie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ewm.hammf.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mbz.snrcjt.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cpv.uphjek.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://abu.epnwcf.com

[D11] 反转数组
来源：http://emt.ydjk.org.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wnu.zhengqikj.top

PHP:  array_reverse($arr);
来源：http://zwp.aibaodan.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wqg.shangyingyoupin.top

TS:   [...arr].reverse();
来源：http://ney.sjlbkw.cn

Java: Collections.reverse(list);
来源：http://ifa.yangfankeji.com

Go:   slices.Reverse(arr)
来源：http://awo.fktsv.cn

Ruby: arr.reverse
来源：http://qey.vehdjk.com

C#:   list.Reverse();
来源：http://dvk.ydjk.org.cn

[D12] 查找元素下标
来源：http://mvb.nwbrower.top

Py:   arr.index(x);  x in arr
来源：http://onm.epnwcf.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cpu.nanxinkj.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cmr.9152youxi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zae.zhongyouzk.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ldh.sufxvd.cn

Go:   slices.Index(arr, x)
来源：http://thn.52xcode.cn

Ruby: arr.index(x)
来源：http://qfy.hysaishi.cn

C#:   list.IndexOf(x);
来源：http://ncl.yuanzhike.top

[D13] 过滤（保留满足条件的）
来源：http://fym.guowangkeji.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lel.316326.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fwi.ywan-chungtsiang.top

JS:   arr.filter(x => x > 3)
来源：http://xsf.iojbl.cn

TS:   arr.filter(x => x > 3)
来源：http://ulk.guannengcc.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zpe.bbcook.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pqq.jinqigfzy.top

Ruby: arr.select { |x| x > 3 }
来源：http://vbb.jinghuilouyu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://upz.yuxming.cn

[D14] 映射转换（每个元素变形）
来源：http://sdm.zhixingplan.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ahv.9152youxi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xen.jinqigufen.top

JS:   arr.map(x => x * 2)
来源：http://nph.wangshuangyany.cn

TS:   arr.map(x => x * 2)
来源：http://wwy.xinyue.icu

Java: list.stream().map(x -> x * 2).toList()
来源：http://bhi.bbcook.cn

Go:   // 手写循环
来源：http://pzw.sjlbkw.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fgu.fktsv.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://vbv.aibaodan.cn


<!-- 参考信息 -->