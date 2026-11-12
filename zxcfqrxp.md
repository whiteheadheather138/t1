代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://bpt.yangfankeji.com

TS:   [1, 2, 3].includes(x)
来源：http://pww.fktsv.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://prk.cucudq.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dhu.jinyuanbaomall.cn

Ruby: [1, 2, 3].include?(x)
来源：http://rpy.fanxiaobao.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dwg.yj20258888.top

[B15] 布尔运算与取反
来源：http://boy.meibo888.top

Py:   a and b or not c
来源：http://mmv.sjlbkw.cn

PHP:  $a && $b || !$c
来源：http://kwa.ywan-chungtsiang.top

JS:   a && b || !c
来源：http://rsu.gotoacloud.top

TS:   a && b || !c
来源：http://xjm.chenlongwang.top

Java: a && b || !c
来源：http://mye.jlsjyb.cn

Go:   a && b || !c
来源：http://dhn.nanxuanxn.top

Ruby: a && b || !c
来源：http://cst.mhx1999.top

C#:   a && b || !c
来源：http://dmu.snrcjt.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xsz.zdqjudy.top

Py:   if not data: return
来源：http://vlc.0kj1m.cn

PHP:  if (!$data) { return; }
来源：http://yfq.yj20258.top

JS:   if (!data) return;
来源：http://upy.xuetiantiany.cn

TS:   if (!data) return;
来源：http://wje.uphjek.com

Java: if (data == null) return;
来源：http://vbe.jianghu66.top

Go:   if data == nil { return }
来源：http://xmd.hywenlv.cn

Ruby: return if data.nil?
来源：http://oyn.xinyue.icu

C#:   if (data == null) return;
来源：http://lwk.yfazqb.com

================================================================================
来源：http://lmw.yangfankeji.com

C. 函数与作用域
来源：http://gme.zhengqikj.top

================================================================================
来源：http://nsh.zhoulong.xyz

[C01] 定义函数
来源：http://bmn.jianghu66.top

Py:   def add(a, b): return a + b
来源：http://mja.hysaishi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://abq.jianghu66.top

JS:   function add(a, b) { return a + b; }
来源：http://awf.redwolf501.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fhm.vehdjk.com

Java: static int add(int a, int b) { return a + b; }
来源：http://muz.andypj.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://wqi.pycfn.com

Ruby: def add(a, b); a + b; end
来源：http://ohd.pycfn.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://oyj.nanxinkj.top

[C02] 默认参数
来源：http://ubb.xingfuxueyuan.xyz

Py:   def greet(name="World"): return name
来源：http://snc.uphjek.com

PHP:  function greet($name = "World") { return $name; }
来源：http://wyq.chenzaomai.com

JS:   function greet(name = "World") { return name; }
来源：http://boz.kuanghao11.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://oem.hywenlv.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://abo.316326.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ifc.jinqigfzy.top

Ruby: def greet(name = "World") = name
来源：http://eht.fktsv.cn

C#:   string Greet(string name = "World") => name;
来源：http://zak.vehdjk.com

[C03] 可变参数
来源：http://mub.daria6918.cn

Py:   def total(*args): return sum(args)
来源：http://zdh.shuidangran.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ywz.guowangkeji.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blr.dianchejie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://poa.yvedp.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mxv.aizwys.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wqh.nanxuanxn.top

Ruby: def total(*nums); nums.sum; end
来源：http://sjq.xuanzx.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nvz.uphjek.com

[C04] 命名参数 / 关键字参数
来源：http://bsi.zdqjudy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yno.yfazqb.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xxs.jinqigfzy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://scr.cheryme.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qqu.meibo888.top

Java: // 无：用 Builder 模式或 record
来源：http://tfd.gaohongyu789.top

Go:   // 无：用配置结构体参数
来源：http://dvc.dianchejie.cn

Ruby: f(a: 1, b: 2)
来源：http://ylj.yongpay.top

C#:   f(a: 1, b: 2)
来源：http://jug.yonumen.top

[C05] 返回多个值
来源：http://ocp.sjlbkw.cn

Py:   return a, b
来源：http://sgi.redwolf501.top

PHP:  return [$a, $b];
来源：http://esq.daria6918.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fds.daria6918.cn

TS:   return { a, b };
来源：http://nmk.jinqigfzy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rhh.fanxiaobao.xyz

Go:   return a, b
来源：http://gke.hammf.cn

Ruby: return a, b
来源：http://ncx.kuanghao11.cn

C#:   return (a, b);              // ValueTuple
来源：http://yrd.tanke756.top

[C06] 匿名函数 / lambda
来源：http://pct.havefunace.top

Py:   square = lambda x: x * x
来源：http://pkc.shangyingyoupin.top

PHP:  $square = fn($x) => $x * $x;
来源：http://hga.nwbrower.top

JS:   const square = x => x * x;
来源：http://gro.feifeiyinyue.top

TS:   const square = (x: number): number => x * x;
来源：http://ctu.jianghu66.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://keu.zdbjq.cn

Go:   sq := func(x int) int { return x * x }
来源：http://otz.yj20258.top

Ruby: square = ->(x) { x * x }
来源：http://tss.zdbjq.cn

C#:   Func<int, int> square = x => x * x;
来源：http://dgn.nwbrower.top

[C07] 把函数作为参数传入
来源：http://kan.yfazqb.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sug.shuidangran.top

PHP:  array_map("strtoupper", $arr);
来源：http://wib.sweek.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qti.shzxlz.cn

TS:   arr.map(String)
来源：http://zux.zycfv.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://phq.shangyingyoupin.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://okz.shanyushiyangkeji.top

Ruby: arr.map(&:upcase)
来源：http://cni.ehwqpu.com

C#:   arr.Select(s => s.ToUpper())
来源：http://fpn.ehwqpu.com

[C08] 闭包
来源：http://wqo.gotoacloud.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uou.zhiwuduotai.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rcg.birdmap.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kmf.zycfv.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://srk.yangfankeji.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xoo.xinyue.icu

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gbl.52xcode.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://erb.quarkkingdee.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xjs.jinghuilouyu.cn

[C09] 递归
来源：http://ajh.gaohongyu789.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wzm.sweek.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ibe.yuxming.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bno.chenjidiqi.icu

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://brr.ybcxt.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rap.ybcxt.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rew.fehbvm.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mbg.ybcxt.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qxa.guannengcc.top

[C10] 变量作用域
来源：http://ooh.hnqzz.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wmv.birdmap.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://aat.xuetiantiany.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fsa.fktsv.cn

TS:   同 JS
来源：http://mxn.andypj.xyz

Java: 方法内为块级作用域
来源：http://ayw.xinyue.icu

Go:   花括号块级作用域
来源：http://ixw.xinyue.icu

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zxj.fanxiaobao.xyz

C#:   块级作用域
来源：http://keb.fanxiaobao.xyz

[C11] 模块导入与导出
来源：http://kmf.xuetiantiany.cn

Py:   from module import func
来源：http://vjd.yonumen.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ydk.tian-w.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://moo.shangyingyoupin.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gsb.zhijiandao.cn

Java: import java.util.List;
来源：http://vmy.yj202588.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vim.dianchejie.cn

Ruby: require "json"; require_relative "./util"
来源：http://wgr.tarul.cn

C#:   using System.Text;
来源：http://uxf.cashguo.top

[C12] 立即执行函数 IIFE
来源：http://cyd.9152youxi.cn

Py:   (lambda: print("run"))()
来源：http://fwn.jinqigfzy.top

PHP:  (function () { echo "run"; })();
来源：http://mpb.zhixingplan.top

JS:   (() => { console.log("run"); })();
来源：http://chu.fehbvm.com

TS:   (() => { console.log("run"); })();
来源：http://dlx.jinghuilouyu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zpi.feifeiyinyue.top

Go:   func() { fmt.Println("run") }()
来源：http://esn.cdnleiting.top

Ruby: -> { puts "run" }.call
来源：http://waw.zycfv.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qbh.vehdjk.com

[C13] 类型声明 / 类型注解
来源：http://jwf.svipenyu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://iiz.feifeiyinyue.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://aiu.yueranfly.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ktp.xinyue.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://buj.ydjk.org.cn

Java: int add(int a, int b) { return a + b; }
来源：http://hyn.ydjk.org.cn

Go:   func add(a, b int) int
来源：http://pcl.aibaodan.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xpo.sxryk.cn

C#:   int Add(int a, int b) => a + b;
来源：http://yyg.yonumen.top

[C14] 泛型函数
来源：http://uqr.aibaodan.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://iir.xziqi.cn

PHP:  // 无泛型
来源：http://yzs.uphjek.com

JS:   // 无泛型
来源：http://wtm.pycfn.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://svg.ydjk.org.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://omu.316326.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://acn.ybcxt.top

Ruby: # 无泛型
来源：http://xmk.xylfe.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://eqg.sysykeji.top

[C15] 解构 / 展开参数
来源：http://afn.dianchejie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bdl.sufxvd.cn

PHP:  [$a, $b] = $pair;
来源：http://zvc.ydzc1.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pku.zdbjq.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xef.ydjk.org.cn

Java: // 无解构
来源：http://qip.jinqigfzy.top

Go:   // 无解构
来源：http://kpm.cashguo.top

Ruby: a, b = pair
来源：http://waz.jinghuilouyu.cn

C#:   var (a, b) = pair;
来源：http://dax.hammf.cn

[C16] 函数 / 方法重载
来源：http://bxe.jiagoushi.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://req.yj20258.top

PHP:  // 无重载
来源：http://mgj.gzhubu.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://imm.jyoumei.cn

TS:   // 用联合类型或重载签名声明
来源：http://pzh.pengpengdd.cyou

Java: void f(int a) {}  void f(String a) {}
来源：http://jyj.daxiang520.top

Go:   // 无重载：用不同函数名
来源：http://jxw.redwolf501.top

Ruby: # 无重载：靠动态参数
来源：http://fdo.mhx1999.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://tbs.jiagoushi.top

================================================================================
来源：http://phi.yj202588.top

D. 数组 / 列表 / 集合
来源：http://aff.jinqigfzy.top

================================================================================
来源：http://icf.shangyingyoupin.top

[D01] 创建数组 / 列表
来源：http://srt.zhixingplan.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://nkr.jinghuilouyu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mmn.ivvv.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dmv.hnqzz.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://fuy.ybcxt.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zga.sxryk.cn

Go:   arr := []int{1, 2, 3}
来源：http://wsc.xingfuxueyuan.xyz

Ruby: arr = [1, 2, 3]
来源：http://pqe.xuanzx.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ekb.hysaishi.cn

[D02] 追加元素到末尾
来源：http://sog.zhengqikj.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://avm.jinghuilouyu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lhg.yangfankeji.com

JS:   arr.push(4);
来源：http://ooa.yueranfly.top

TS:   arr.push(4);
来源：http://dlw.yuxming.cn

Java: list.add(4);
来源：http://ptc.feifeiyinyue.top

Go:   arr = append(arr, 4)
来源：http://tgi.tarul.cn

Ruby: arr << 4; arr.push(5)
来源：http://uga.andypj.xyz

C#:   list.Add(4);
来源：http://lgh.epnwcf.com

[D03] 在指定位置插入元素
来源：http://vse.mhx1999.top

Py:   arr.insert(0, 0)
来源：http://lth.redwolf501.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://isq.yangfankeji.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://odh.vehdjk.com

TS:   arr.splice(0, 0, 0);
来源：http://noh.daxiang520.top

Java: list.add(0, 0);
来源：http://plf.zhixingplan.top

Go:   arr = append([]int{0}, arr...)
来源：http://mgk.mhx1999.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zxv.xuetiantiany.cn

C#:   list.Insert(0, 0);
来源：http://jsg.cucudq.cn

[D04] 删除元素
来源：http://nji.havefunace.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nly.gaohongyu789.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mrq.9152youxi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kqs.shanyushiyangkeji.top

TS:   arr.splice(0, 1);
来源：http://nje.gotoacloud.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://alr.bjfxy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tuf.xingfuxueyuan.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qkp.feifeiyinyue.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qle.havefunace.top

[D05] 访问与修改元素
来源：http://ysu.jinqigufen.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gnk.zdbjq.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zpg.aizwys.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cut.hcnkem.com

TS:   arr[0]; arr.at(-1);
来源：http://abx.shuidangran.top

Java: list.get(0); list.set(0, 9);
来源：http://gxi.ppjwa.cn

Go:   arr[0]; arr[0] = 9
来源：http://bmm.yuxming.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zck.jqgfzy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hoc.fzhhl.top

[D06] 数组长度
来源：http://tts.tarul.cn

Py:   len(arr)
来源：http://yuk.daria6918.cn

PHP:  count($arr);
来源：http://fzg.hnxiangtu.top

JS:   arr.length
来源：http://tdb.havefunace.top

TS:   arr.length
来源：http://qkl.snrcjt.cn

Java: list.size();
来源：http://nwv.fktsv.cn

Go:   len(arr)
来源：http://alo.ctjpmb.com

Ruby: arr.length; arr.size
来源：http://mwa.tian-w.cn

C#:   list.Count;
来源：http://xyg.ehwqpu.com

[D07] 切片 / 取子数组
来源：http://win.meibo888.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pch.jqgufenzy.top

PHP:  array_slice($arr, 1, 3);
来源：http://tby.xinyue.icu

JS:   arr.slice(1, 4);
来源：http://hdq.xuetiantiany.cn

TS:   arr.slice(1, 4);
来源：http://lmb.hnqzz.top

Java: list.subList(1, 4);
来源：http://nfx.dashuyun.cn

Go:   arr[1:4]
来源：http://qzp.9152youxi.cn

Ruby: arr[1, 3]
来源：http://nmj.ctjpmb.com

C#:   list.GetRange(1, 3);
来源：http://gsm.zdqjudy.top

[D08] 合并两个数组
来源：http://erq.hammf.cn

Py:   a + b;  a.extend(b)
来源：http://pix.yj20258.top

PHP:  array_merge($a, $b);
来源：http://zyp.chenzaomai.com

JS:   [...a, ...b];  a.concat(b);
来源：http://pvc.yonumen.top

TS:   [...a, ...b];
来源：http://azd.fktsv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lov.ywan-chungtsiang.top

Go:   append(a, b...)
来源：http://oat.zhengqikj.top

Ruby: a + b;  a.concat(b)
来源：http://emb.fzhhl.top

C#:   a.Concat(b).ToList()
来源：http://jrl.cheryme.top

[D09] 排序（升序）
来源：http://wti.daria6918.cn

Py:   sorted(arr);  arr.sort()
来源：http://zkz.guowangkeji.top

PHP:  sort($arr);
来源：http://mlk.chenjidiqi.icu

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gxh.daria6918.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xcl.hcnkem.com

Java: Collections.sort(list);  list.sort(null);
来源：http://mwz.tanke756.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vbk.gogol.net.cn

Ruby: arr.sort
来源：http://wzn.zhixingplan.top

C#:   list.Sort();
来源：http://grg.bbcook.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://bso.sweek.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://edm.tarul.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://joh.yanxiufei.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://drx.xylfe.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qly.chenjidiqi.icu

Java: list.sort(Comparator.comparing(Person::age));
来源：http://byr.hcnkem.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ucw.yonumen.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://exl.xingfuxueyuan.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://knt.zhaomingkeji.xyz

[D11] 反转数组
来源：http://ixc.fanxiaobao.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://lpw.andypj.xyz

PHP:  array_reverse($arr);
来源：http://ddo.chenzaomai.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hoo.daria6918.cn

TS:   [...arr].reverse();
来源：http://gbs.hnxiangtu.top

Java: Collections.reverse(list);
来源：http://fey.gaohongyu789.top

Go:   slices.Reverse(arr)
来源：http://oln.jiagoushi.top

Ruby: arr.reverse
来源：http://ext.sweek.top

C#:   list.Reverse();
来源：http://bme.ppjwa.cn

[D12] 查找元素下标
来源：http://njh.aizwys.cn

Py:   arr.index(x);  x in arr
来源：http://kkg.ybcxt.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uau.sufxvd.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gxz.aibaodan.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zqo.nanxinkj.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cel.xylfe.cn

Go:   slices.Index(arr, x)
来源：http://tch.shzxlz.cn

Ruby: arr.index(x)
来源：http://atb.ivvv.top

C#:   list.IndexOf(x);
来源：http://ptf.yangfankeji.com

[D13] 过滤（保留满足条件的）
来源：http://obz.guowangkeji.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://alb.zycfv.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://axt.yj202588.top

JS:   arr.filter(x => x > 3)
来源：http://ylk.jinqigufen.top

TS:   arr.filter(x => x > 3)
来源：http://wlo.ydjk.org.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qwv.shanyushiyangtech.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fgz.jiagoushi.top

Ruby: arr.select { |x| x > 3 }
来源：http://pev.jinghuilouyu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ccw.sufxvd.cn

[D14] 映射转换（每个元素变形）
来源：http://bkd.ydjk.org.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://oeu.ydjk.org.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kyy.daxiang520.top

JS:   arr.map(x => x * 2)
来源：http://yzt.meibo888.top

TS:   arr.map(x => x * 2)
来源：http://sac.zycfv.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://iqk.iojbl.cn

Go:   // 手写循环
来源：http://bfw.zdbjq.cn

Ruby: arr.map { |x| x * 2 }
来源：http://zwk.nanxuanxn.top

C#:   list.Select(x => x * 2).ToList()
来源：http://yue.jlsjyb.cn


<!-- 参考信息 -->