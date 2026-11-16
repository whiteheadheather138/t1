代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://lqz.wangdashe.top

TS:   [1, 2, 3].includes(x)
来源：http://gwt.sweek.top

Java: List.of(1, 2, 3).contains(x)
来源：http://vfs.pengpengdd.cyou

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jat.daxiang520.top

Ruby: [1, 2, 3].include?(x)
来源：http://gqb.shzxlz.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gpt.ywan-chungtsiang.top

[B15] 布尔运算与取反
来源：http://mmz.shzxlz.cn

Py:   a and b or not c
来源：http://kla.hesvh.cn

PHP:  $a && $b || !$c
来源：http://wsx.shangyingyoupin.top

JS:   a && b || !c
来源：http://ebe.pycfn.com

TS:   a && b || !c
来源：http://ken.shanyushiyangtech.top

Java: a && b || !c
来源：http://cwv.ybcxt.top

Go:   a && b || !c
来源：http://iln.ppjwa.cn

Ruby: a && b || !c
来源：http://nfu.snrcjt.cn

C#:   a && b || !c
来源：http://eny.hfpthk.cn

[B16] 卫语句：不满足条件提前返回
来源：http://okf.jyoumei.cn

Py:   if not data: return
来源：http://wuu.zhiwuduotai.top

PHP:  if (!$data) { return; }
来源：http://mey.zhengqikj.top

JS:   if (!data) return;
来源：http://zwy.nanxinkj.top

TS:   if (!data) return;
来源：http://jle.zhoulong.xyz

Java: if (data == null) return;
来源：http://bqt.tian-w.cn

Go:   if data == nil { return }
来源：http://jnj.ybcxt.top

Ruby: return if data.nil?
来源：http://jxg.nanxinkj.top

C#:   if (data == null) return;
来源：http://cce.meibo888.top

================================================================================
来源：http://ppr.xuetiantiany.cn

C. 函数与作用域
来源：http://sdy.yueranfly.top

================================================================================
来源：http://mwp.yuanzhike.top

[C01] 定义函数
来源：http://scf.yj20258888.top

Py:   def add(a, b): return a + b
来源：http://iah.yueranfly.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oeu.zdqjudy.top

JS:   function add(a, b) { return a + b; }
来源：http://sjc.9152youxi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cme.aizwys.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://epj.xziqi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://emh.mhx1999.top

Ruby: def add(a, b); a + b; end
来源：http://qbq.gzhubu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dbm.xingfuxueyuan.xyz

[C02] 默认参数
来源：http://otb.52xcode.cn

Py:   def greet(name="World"): return name
来源：http://tng.birdmap.top

PHP:  function greet($name = "World") { return $name; }
来源：http://hiw.haohaochexian.top

JS:   function greet(name = "World") { return name; }
来源：http://ais.ppjwa.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://dsx.jqgufenzy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://dds.dianchejie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vjn.52xcode.cn

Ruby: def greet(name = "World") = name
来源：http://mmw.sysykeji.top

C#:   string Greet(string name = "World") => name;
来源：http://mgs.daxiang520.top

[C03] 可变参数
来源：http://yvj.aibaodan.cn

Py:   def total(*args): return sum(args)
来源：http://eif.birdmap.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hmm.kuanghao11.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dmc.yj202588.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qrc.shanyushiyangtech.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gmq.andypj.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dwi.aizwys.cn

Ruby: def total(*nums); nums.sum; end
来源：http://dyu.jqgfzy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ywc.zhijiandao.cn

[C04] 命名参数 / 关键字参数
来源：http://rea.0kj1m.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://iug.chenlongwang.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nar.bjfxy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dpf.shangyingyoupin.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://frg.fehbvm.com

Java: // 无：用 Builder 模式或 record
来源：http://jiv.daria6918.cn

Go:   // 无：用配置结构体参数
来源：http://rie.sjlbkw.cn

Ruby: f(a: 1, b: 2)
来源：http://gjw.ivvv.top

C#:   f(a: 1, b: 2)
来源：http://mxq.hfpthk.cn

[C05] 返回多个值
来源：http://ygk.hammf.cn

Py:   return a, b
来源：http://tql.jiagoushi.top

PHP:  return [$a, $b];
来源：http://wko.yuxming.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://min.yuanzhike.top

TS:   return { a, b };
来源：http://tmn.bbcook.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://luj.pycfn.com

Go:   return a, b
来源：http://gae.ppjwa.cn

Ruby: return a, b
来源：http://mtz.vqdsnc.cn

C#:   return (a, b);              // ValueTuple
来源：http://gnp.daria6918.cn

[C06] 匿名函数 / lambda
来源：http://pkb.ctjpmb.com

Py:   square = lambda x: x * x
来源：http://pjj.aibaodan.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wgv.hongshengwenyu.top

JS:   const square = x => x * x;
来源：http://zzg.meibo888.top

TS:   const square = (x: number): number => x * x;
来源：http://sbd.zhoulong.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ehu.yonumen.top

Go:   sq := func(x int) int { return x * x }
来源：http://vss.quarkkingdee.top

Ruby: square = ->(x) { x * x }
来源：http://xsk.yj20258.top

C#:   Func<int, int> square = x => x * x;
来源：http://xkd.tanke756.top

[C07] 把函数作为参数传入
来源：http://att.hammf.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://acm.snrcjt.cn

PHP:  array_map("strtoupper", $arr);
来源：http://agh.vehdjk.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ope.xuanzx.com

TS:   arr.map(String)
来源：http://yoa.hammf.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bua.daxiang520.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://alo.zhoulong.xyz

Ruby: arr.map(&:upcase)
来源：http://oeu.chenzaomai.com

C#:   arr.Select(s => s.ToUpper())
来源：http://fgl.9152youxi.cn

[C08] 闭包
来源：http://zdm.zhaomingkeji.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zit.shzxlz.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://biq.sysykeji.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wzp.meibo888.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jwi.shzxlz.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vmp.jiagoushi.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rem.jlsjyb.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://huz.xingfuxueyuan.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tgc.cucudq.cn

[C09] 递归
来源：http://duf.cdnleiting.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cap.yfazqb.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wfr.hnqzz.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uhr.ybcxt.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zqg.yvedp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ifd.hywenlv.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://umk.havefunace.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://syp.svipenyu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vqq.ppjwa.cn

[C10] 变量作用域
来源：http://iqf.yvedp.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://utk.52xcode.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mwp.sjlbkw.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mfq.aibaodan.cn

TS:   同 JS
来源：http://blz.chenjidiqi.icu

Java: 方法内为块级作用域
来源：http://dpb.jqgufenzy.top

Go:   花括号块级作用域
来源：http://rgl.cashguo.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dhd.c1oappe.top

C#:   块级作用域
来源：http://yrp.fanxiaobao.xyz

[C11] 模块导入与导出
来源：http://edb.hysaishi.cn

Py:   from module import func
来源：http://zjk.jyoumei.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ris.jyoumei.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://wds.jlsjyb.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nku.jiagoushi.top

Java: import java.util.List;
来源：http://udl.zhengqikj.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zhl.hnqzz.top

Ruby: require "json"; require_relative "./util"
来源：http://jre.fzhhl.top

C#:   using System.Text;
来源：http://ops.0kj1m.cn

[C12] 立即执行函数 IIFE
来源：http://ffg.guannengcc.top

Py:   (lambda: print("run"))()
来源：http://vst.sysykeji.top

PHP:  (function () { echo "run"; })();
来源：http://pad.sufxvd.cn

JS:   (() => { console.log("run"); })();
来源：http://hav.hnqzz.top

TS:   (() => { console.log("run"); })();
来源：http://wib.zycfv.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xtl.smart0.xyz

Go:   func() { fmt.Println("run") }()
来源：http://cip.ehwqpu.com

Ruby: -> { puts "run" }.call
来源：http://bjm.cqqwz.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://sod.meibo888.top

[C13] 类型声明 / 类型注解
来源：http://nsb.kuanghao11.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zoy.wangshuangyany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jau.jiagoushi.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vvy.yueranfly.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ggm.jiagoushi.top

Java: int add(int a, int b) { return a + b; }
来源：http://ltv.iojbl.cn

Go:   func add(a, b int) int
来源：http://mps.yj20258.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://krc.9152youxi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ran.jyoumei.cn

[C14] 泛型函数
来源：http://aba.tanke756.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bau.sxryk.cn

PHP:  // 无泛型
来源：http://bcu.kuanghao11.cn

JS:   // 无泛型
来源：http://tea.chenzaomai.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mah.uphjek.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qyz.sufxvd.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://crj.nanxinkj.top

Ruby: # 无泛型
来源：http://bpj.fehbvm.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ayu.jinyuanbaomall.cn

[C15] 解构 / 展开参数
来源：http://ing.daxiang520.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nln.jinghuilouyu.cn

PHP:  [$a, $b] = $pair;
来源：http://lld.gzhubu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://utt.zycfv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zkw.tarul.cn

Java: // 无解构
来源：http://wcn.sxryk.cn

Go:   // 无解构
来源：http://nkb.yj202588.top

Ruby: a, b = pair
来源：http://qcx.ydjk.org.cn

C#:   var (a, b) = pair;
来源：http://zlp.uphjek.com

[C16] 函数 / 方法重载
来源：http://vwn.gogol.net.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qrs.yueranfly.top

PHP:  // 无重载
来源：http://mvn.gzhubu.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://bzh.fzhhl.top

TS:   // 用联合类型或重载签名声明
来源：http://zck.shzxlz.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ntf.meibo888.top

Go:   // 无重载：用不同函数名
来源：http://fvl.yj20258888.top

Ruby: # 无重载：靠动态参数
来源：http://yrc.xuetiantiany.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://usx.quarkkingdee.top

================================================================================
来源：http://xoz.zhongyouzk.top

D. 数组 / 列表 / 集合
来源：http://exc.haohaochexian.top

================================================================================
来源：http://mrj.hfpthk.cn

[D01] 创建数组 / 列表
来源：http://jhs.52xcode.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qap.hywenlv.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gku.guowangkeji.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://iih.havefunace.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://lol.aizwys.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ozi.hywenlv.cn

Go:   arr := []int{1, 2, 3}
来源：http://xsg.xingfuxueyuan.xyz

Ruby: arr = [1, 2, 3]
来源：http://kqa.gaohongyu789.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ctn.ydzc1.top

[D02] 追加元素到末尾
来源：http://lhu.chenzaomai.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jjc.ydjk.org.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vbq.feifeiyinyue.top

JS:   arr.push(4);
来源：http://fas.snrcjt.cn

TS:   arr.push(4);
来源：http://coz.xziqi.cn

Java: list.add(4);
来源：http://jzw.52xcode.cn

Go:   arr = append(arr, 4)
来源：http://arq.chenjidiqi.icu

Ruby: arr << 4; arr.push(5)
来源：http://wdq.jianghu66.top

C#:   list.Add(4);
来源：http://fnv.xuanzx.com

[D03] 在指定位置插入元素
来源：http://gdb.tian-w.cn

Py:   arr.insert(0, 0)
来源：http://cry.nanxuanxn.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ynd.fktsv.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lqn.shanyushiyangkeji.top

TS:   arr.splice(0, 0, 0);
来源：http://tgs.pengpengdd.cyou

Java: list.add(0, 0);
来源：http://wzy.nanxuanxn.top

Go:   arr = append([]int{0}, arr...)
来源：http://adn.yonumen.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nat.gzhubu.top

C#:   list.Insert(0, 0);
来源：http://deo.zhijiandao.cn

[D04] 删除元素
来源：http://bny.jiagoushi.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://iyw.tian-w.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vye.andypj.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://byg.daria6918.cn

TS:   arr.splice(0, 1);
来源：http://arp.haohaochexian.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pmt.nanxuanxn.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jgj.zdbjq.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jfa.cucudq.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ofv.hongshengwenyu.top

[D05] 访问与修改元素
来源：http://mqm.daxiang520.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gps.havefunace.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gso.pengpengdd.cyou

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yds.shanyushiyangtech.top

TS:   arr[0]; arr.at(-1);
来源：http://nqg.zhijiandao.cn

Java: list.get(0); list.set(0, 9);
来源：http://nwb.hfpthk.cn

Go:   arr[0]; arr[0] = 9
来源：http://pwn.yj20258888.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ubo.yangfankeji.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zrs.tianlin.xyz

[D06] 数组长度
来源：http://yox.yj20258888.top

Py:   len(arr)
来源：http://cyf.pengpengdd.cyou

PHP:  count($arr);
来源：http://xkm.meibo888.top

JS:   arr.length
来源：http://vco.nanxinkj.top

TS:   arr.length
来源：http://fal.shzxlz.cn

Java: list.size();
来源：http://set.aibaodan.cn

Go:   len(arr)
来源：http://fpy.wangshuangyany.cn

Ruby: arr.length; arr.size
来源：http://lup.fengsongda.top

C#:   list.Count;
来源：http://tqu.jinghuilouyu.cn

[D07] 切片 / 取子数组
来源：http://myg.gaohongyu789.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://eor.ybcxt.top

PHP:  array_slice($arr, 1, 3);
来源：http://jzk.andypj.xyz

JS:   arr.slice(1, 4);
来源：http://qik.zhiwuduotai.top

TS:   arr.slice(1, 4);
来源：http://trs.shzxlz.cn

Java: list.subList(1, 4);
来源：http://zwe.cdnleiting.top

Go:   arr[1:4]
来源：http://nbx.yj20258888.top

Ruby: arr[1, 3]
来源：http://xel.chenzaomai.com

C#:   list.GetRange(1, 3);
来源：http://chr.jyoumei.cn

[D08] 合并两个数组
来源：http://bks.jiagoushi.top

Py:   a + b;  a.extend(b)
来源：http://abd.shuidangran.top

PHP:  array_merge($a, $b);
来源：http://fsr.xziqi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://bkf.ydzc1.top

TS:   [...a, ...b];
来源：http://bvz.hcnkem.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://aeb.zdqjudy.top

Go:   append(a, b...)
来源：http://xzj.chenzaomai.com

Ruby: a + b;  a.concat(b)
来源：http://mpc.52xcode.cn

C#:   a.Concat(b).ToList()
来源：http://tyg.yj202588.top

[D09] 排序（升序）
来源：http://qys.jianghu66.top

Py:   sorted(arr);  arr.sort()
来源：http://dub.hesvh.cn

PHP:  sort($arr);
来源：http://ykv.redwolf501.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qrn.hammf.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://jly.sweek.top

Java: Collections.sort(list);  list.sort(null);
来源：http://zag.gotoacloud.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://oyc.52xcode.cn

Ruby: arr.sort
来源：http://tmt.xuanzx.com

C#:   list.Sort();
来源：http://pus.jinyuanbaomall.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://pgc.meibo888.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mua.xylfe.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ova.cucudq.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xec.zhijiandao.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://eiw.sxryk.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lip.yanxiufei.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xqa.sjlbkw.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gpg.yj20258888.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://luc.pycfn.com

[D11] 反转数组
来源：http://czb.zhengqikj.top

Py:   arr[::-1];  arr.reverse()
来源：http://lqb.ppjwa.cn

PHP:  array_reverse($arr);
来源：http://mrm.chenzaomai.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://szi.0kj1m.cn

TS:   [...arr].reverse();
来源：http://glz.dianchejie.cn

Java: Collections.reverse(list);
来源：http://mui.ctjpmb.com

Go:   slices.Reverse(arr)
来源：http://yra.ehwqpu.com

Ruby: arr.reverse
来源：http://qwt.yuxming.cn

C#:   list.Reverse();
来源：http://bxs.aizwys.cn

[D12] 查找元素下标
来源：http://tjo.yonumen.top

Py:   arr.index(x);  x in arr
来源：http://nqc.shanyushiyangtech.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vcx.hcnkem.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ifb.fanxiaobao.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yzu.shzxlz.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ajq.zhiwuduotai.top

Go:   slices.Index(arr, x)
来源：http://jrd.yfazqb.com

Ruby: arr.index(x)
来源：http://xee.xylfe.cn

C#:   list.IndexOf(x);
来源：http://hyl.shuidangran.top

[D13] 过滤（保留满足条件的）
来源：http://uif.xuetiantiany.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gxy.xuetiantiany.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mgh.redwolf501.top

JS:   arr.filter(x => x > 3)
来源：http://pzp.shanyushiyangkeji.top

TS:   arr.filter(x => x > 3)
来源：http://wef.guowangkeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xel.fzhhl.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qzz.guannengcc.top

Ruby: arr.select { |x| x > 3 }
来源：http://mxm.cdnleiting.top

C#:   list.Where(x => x > 3).ToList()
来源：http://mcm.wangshuangyany.cn

[D14] 映射转换（每个元素变形）
来源：http://ddg.sysykeji.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bkv.cdnleiting.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cij.ybcxt.top

JS:   arr.map(x => x * 2)
来源：http://jho.havefunace.top

TS:   arr.map(x => x * 2)
来源：http://loj.birdmap.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://jyz.vqdsnc.cn

Go:   // 手写循环
来源：http://lma.xinyue.icu

Ruby: arr.map { |x| x * 2 }
来源：http://pef.epnwcf.com

C#:   list.Select(x => x * 2).ToList()
来源：http://cpb.shanyushiyangtech.top


<!-- 参考信息 -->