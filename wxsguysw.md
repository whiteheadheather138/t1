代发 wailian999

C#:   x is int or double or decimal
来源：http://pby.cqqwz.cn

[B14] 判断值是否在集合内
来源：http://pwr.hnxiangtu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nup.uphjek.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://spc.aibaodan.cn

JS:   [1, 2, 3].includes(x)
来源：http://cry.yj20258.top

TS:   [1, 2, 3].includes(x)
来源：http://wpx.zycfv.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://jhr.jiagoushi.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gql.guowangkeji.top

Ruby: [1, 2, 3].include?(x)
来源：http://qid.nwbrower.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://sbi.zhijiandao.cn

[B15] 布尔运算与取反
来源：http://eqp.haohaochexian.top

Py:   a and b or not c
来源：http://vkz.316326.xyz

PHP:  $a && $b || !$c
来源：http://bjo.xziqi.cn

JS:   a && b || !c
来源：http://zyk.gaohongyu789.top

TS:   a && b || !c
来源：http://qth.hnqzz.top

Java: a && b || !c
来源：http://xol.zycfv.cn

Go:   a && b || !c
来源：http://xpg.daxiang520.top

Ruby: a && b || !c
来源：http://uue.jiagoushi.top

C#:   a && b || !c
来源：http://wai.zhixingplan.top

[B16] 卫语句：不满足条件提前返回
来源：http://fns.xziqi.cn

Py:   if not data: return
来源：http://spw.tianlin.xyz

PHP:  if (!$data) { return; }
来源：http://bky.hesvh.cn

JS:   if (!data) return;
来源：http://myt.316326.xyz

TS:   if (!data) return;
来源：http://duv.yuanzhike.top

Java: if (data == null) return;
来源：http://fea.jinqigfzy.top

Go:   if data == nil { return }
来源：http://cum.jinqigufen.top

Ruby: return if data.nil?
来源：http://wyw.jinqigufen.top

C#:   if (data == null) return;
来源：http://cop.tianlin.xyz

================================================================================
来源：http://ihn.ctjpmb.com

C. 函数与作用域
来源：http://qhx.zhengqikj.top

================================================================================
来源：http://eun.chenlongwang.top

[C01] 定义函数
来源：http://kkg.gogol.net.cn

Py:   def add(a, b): return a + b
来源：http://vey.hesvh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jdy.zhengqikj.top

JS:   function add(a, b) { return a + b; }
来源：http://cll.daxiang520.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ujo.quarkkingdee.top

Java: static int add(int a, int b) { return a + b; }
来源：http://rme.yanxiufei.cn

Go:   func add(a, b int) int { return a + b }
来源：http://uft.jqgfzy.top

Ruby: def add(a, b); a + b; end
来源：http://vxo.cqqwz.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wsp.pycfn.com

[C02] 默认参数
来源：http://ztp.yangfankeji.com

Py:   def greet(name="World"): return name
来源：http://uys.yj20258.top

PHP:  function greet($name = "World") { return $name; }
来源：http://qon.shanyushiyangkeji.top

JS:   function greet(name = "World") { return name; }
来源：http://lqc.hfpthk.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ggt.chenzaomai.com

Java: // 无默认参数：方法重载或 Optional
来源：http://sxm.cqqwz.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yyo.vqdsnc.cn

Ruby: def greet(name = "World") = name
来源：http://dnp.pycfn.com

C#:   string Greet(string name = "World") => name;
来源：http://vqo.chenjidiqi.icu

[C03] 可变参数
来源：http://niq.jinyuanbaomall.cn

Py:   def total(*args): return sum(args)
来源：http://bme.feifeiyinyue.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://umc.yj20258888.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hqg.pycfn.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yop.ybcxt.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nsm.jiagoushi.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://osx.yj20258.top

Ruby: def total(*nums); nums.sum; end
来源：http://xig.zdbjq.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vlq.shanyushiyangtech.top

[C04] 命名参数 / 关键字参数
来源：http://idi.yfazqb.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://laa.hongshengwenyu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://aes.bbcook.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ltt.ywan-chungtsiang.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xno.hnqzz.top

Java: // 无：用 Builder 模式或 record
来源：http://dnd.jiagoushi.top

Go:   // 无：用配置结构体参数
来源：http://mbu.tarul.cn

Ruby: f(a: 1, b: 2)
来源：http://xjx.jinqigfzy.top

C#:   f(a: 1, b: 2)
来源：http://xii.vqdsnc.cn

[C05] 返回多个值
来源：http://fax.nanxinkj.top

Py:   return a, b
来源：http://erg.gaohongyu789.top

PHP:  return [$a, $b];
来源：http://wef.hysaishi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://tgl.yvedp.cn

TS:   return { a, b };
来源：http://xoi.nwbrower.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mdo.hnxiangtu.top

Go:   return a, b
来源：http://fjr.ydjk.org.cn

Ruby: return a, b
来源：http://xtr.shuidangran.top

C#:   return (a, b);              // ValueTuple
来源：http://brw.feifeiyinyue.top

[C06] 匿名函数 / lambda
来源：http://brr.uphjek.com

Py:   square = lambda x: x * x
来源：http://emh.shuidangran.top

PHP:  $square = fn($x) => $x * $x;
来源：http://lmq.zhongyouzk.top

JS:   const square = x => x * x;
来源：http://oxf.yj202588.top

TS:   const square = (x: number): number => x * x;
来源：http://etu.birdmap.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vym.fehbvm.com

Go:   sq := func(x int) int { return x * x }
来源：http://zkt.dianchejie.cn

Ruby: square = ->(x) { x * x }
来源：http://blm.svipenyu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://mdz.feifeiyinyue.top

[C07] 把函数作为参数传入
来源：http://ool.ydjk.org.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jhp.shanyushiyangtech.top

PHP:  array_map("strtoupper", $arr);
来源：http://qfy.yongpay.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kte.chenlongwang.top

TS:   arr.map(String)
来源：http://nob.zhoulong.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mja.zhengqikj.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://puv.hesvh.cn

Ruby: arr.map(&:upcase)
来源：http://liw.yj202588.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ebo.cucudq.cn

[C08] 闭包
来源：http://bpf.gaohongyu789.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://eox.daria6918.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uvt.xylfe.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fuw.wangdashe.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ihm.fengsongda.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mew.sufxvd.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jvi.birdmap.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nbt.ctjpmb.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xss.xingfuxueyuan.xyz

[C09] 递归
来源：http://zif.cashguo.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zar.tanke756.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dns.jiagoushi.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sip.shanyushiyangkeji.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fdj.birdmap.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cwe.jqgfzy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nkl.yj20258.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tkk.shuidangran.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wzz.sjlbkw.cn

[C10] 变量作用域
来源：http://ddx.9152youxi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://phr.redwolf501.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vgp.xingfuxueyuan.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rfk.zycfv.cn

TS:   同 JS
来源：http://fmm.jyoumei.cn

Java: 方法内为块级作用域
来源：http://bew.ydzc1.top

Go:   花括号块级作用域
来源：http://zbf.meibo888.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hln.hcnkem.com

C#:   块级作用域
来源：http://val.hnxiangtu.top

[C11] 模块导入与导出
来源：http://uci.zhijiandao.cn

Py:   from module import func
来源：http://hbg.gogol.net.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://jqk.birdmap.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://kzy.wangshuangyany.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://equ.svipenyu.cn

Java: import java.util.List;
来源：http://gyl.aizwys.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cso.hywenlv.cn

Ruby: require "json"; require_relative "./util"
来源：http://kkv.cheryme.top

C#:   using System.Text;
来源：http://wpx.jianghu66.top

[C12] 立即执行函数 IIFE
来源：http://pfy.havefunace.top

Py:   (lambda: print("run"))()
来源：http://hzr.yuanzhike.top

PHP:  (function () { echo "run"; })();
来源：http://noi.gaohongyu789.top

JS:   (() => { console.log("run"); })();
来源：http://ipr.hammf.cn

TS:   (() => { console.log("run"); })();
来源：http://hhn.316326.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://enq.hnxiangtu.top

Go:   func() { fmt.Println("run") }()
来源：http://dkd.snrcjt.cn

Ruby: -> { puts "run" }.call
来源：http://krr.shanyushiyangtech.top

C#:   // 无 IIFE：用静态构造函数
来源：http://zsl.fzhhl.top

[C13] 类型声明 / 类型注解
来源：http://ydl.aizwys.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cfk.dashuyun.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tfc.316326.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ngm.jyoumei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://spl.mhx1999.top

Java: int add(int a, int b) { return a + b; }
来源：http://nop.shuidangran.top

Go:   func add(a, b int) int
来源：http://uay.fehbvm.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jsj.gzhubu.top

C#:   int Add(int a, int b) => a + b;
来源：http://hkg.guannengcc.top

[C14] 泛型函数
来源：http://vij.sysykeji.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vxd.havefunace.top

PHP:  // 无泛型
来源：http://ids.zhixingplan.top

JS:   // 无泛型
来源：http://nsk.zhongyouzk.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xku.aibaodan.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wuj.zhixingplan.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://obk.zhijiandao.cn

Ruby: # 无泛型
来源：http://sal.hesvh.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fky.birdmap.top

[C15] 解构 / 展开参数
来源：http://bkm.guannengcc.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wzj.yongpay.top

PHP:  [$a, $b] = $pair;
来源：http://jrz.epnwcf.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kyn.daxiang520.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://msj.yuanzhike.top

Java: // 无解构
来源：http://pfp.ydzc1.top

Go:   // 无解构
来源：http://rps.daxiang520.top

Ruby: a, b = pair
来源：http://cwq.kuanghao11.cn

C#:   var (a, b) = pair;
来源：http://pfs.316326.xyz

[C16] 函数 / 方法重载
来源：http://xnt.pycfn.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pde.yj20258888.top

PHP:  // 无重载
来源：http://omg.jinghuilouyu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://lsv.pycfn.com

TS:   // 用联合类型或重载签名声明
来源：http://jhc.cashguo.top

Java: void f(int a) {}  void f(String a) {}
来源：http://oum.yj20258888.top

Go:   // 无重载：用不同函数名
来源：http://lei.feifeiyinyue.top

Ruby: # 无重载：靠动态参数
来源：http://hfc.gzhubu.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://djs.shuidangran.top

================================================================================
来源：http://pfk.havefunace.top

D. 数组 / 列表 / 集合
来源：http://clj.bbcook.cn

================================================================================
来源：http://olk.xinyue.icu

[D01] 创建数组 / 列表
来源：http://hoj.tian-w.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jri.dashuyun.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://afz.epnwcf.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wvg.yongpay.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://qlt.hnxiangtu.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ysy.ywan-chungtsiang.top

Go:   arr := []int{1, 2, 3}
来源：http://vgg.tanke756.top

Ruby: arr = [1, 2, 3]
来源：http://zgw.zhijiandao.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hvd.ywan-chungtsiang.top

[D02] 追加元素到末尾
来源：http://bbt.xingfuxueyuan.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mkg.feifeiyinyue.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ukz.dianchejie.cn

JS:   arr.push(4);
来源：http://kut.uphjek.com

TS:   arr.push(4);
来源：http://ctx.iojbl.cn

Java: list.add(4);
来源：http://qss.kuanghao11.cn

Go:   arr = append(arr, 4)
来源：http://rag.shanyushiyangkeji.top

Ruby: arr << 4; arr.push(5)
来源：http://sgc.shuidangran.top

C#:   list.Add(4);
来源：http://ujk.vehdjk.com

[D03] 在指定位置插入元素
来源：http://izj.jiagoushi.top

Py:   arr.insert(0, 0)
来源：http://sqk.aibaodan.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://txa.nanxuanxn.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jzf.cucudq.cn

TS:   arr.splice(0, 0, 0);
来源：http://lfg.uphjek.com

Java: list.add(0, 0);
来源：http://jyk.meibo888.top

Go:   arr = append([]int{0}, arr...)
来源：http://vhq.nanxuanxn.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xcy.guannengcc.top

C#:   list.Insert(0, 0);
来源：http://qbn.pengpengdd.cyou

[D04] 删除元素
来源：http://bxc.yonumen.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mat.yj20258.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ici.yj20258888.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://whe.sxryk.cn

TS:   arr.splice(0, 1);
来源：http://zfq.zdqjudy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pfj.sxryk.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://oeg.ctjpmb.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jtj.cashguo.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ajw.fengsongda.top

[D05] 访问与修改元素
来源：http://owx.yanxiufei.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tkk.xingfuxueyuan.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ozf.hnxiangtu.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://plc.quarkkingdee.top

TS:   arr[0]; arr.at(-1);
来源：http://sar.sufxvd.cn

Java: list.get(0); list.set(0, 9);
来源：http://noc.yueranfly.top

Go:   arr[0]; arr[0] = 9
来源：http://yvr.havefunace.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://llx.xuanzx.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rpn.sjlbkw.cn

[D06] 数组长度
来源：http://pvj.chenzaomai.com

Py:   len(arr)
来源：http://qcv.daxiang520.top

PHP:  count($arr);
来源：http://aju.ywan-chungtsiang.top

JS:   arr.length
来源：http://toi.jqgufenzy.top

TS:   arr.length
来源：http://txq.jinghuilouyu.cn

Java: list.size();
来源：http://vgy.kuanghao11.cn

Go:   len(arr)
来源：http://ggx.yangfankeji.com

Ruby: arr.length; arr.size
来源：http://ajg.pengpengdd.cyou

C#:   list.Count;
来源：http://bai.iojbl.cn

[D07] 切片 / 取子数组
来源：http://ctv.mhx1999.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://crk.daria6918.cn

PHP:  array_slice($arr, 1, 3);
来源：http://oyu.jyoumei.cn

JS:   arr.slice(1, 4);
来源：http://uko.sufxvd.cn

TS:   arr.slice(1, 4);
来源：http://vbr.dianchejie.cn

Java: list.subList(1, 4);
来源：http://bob.shangyingyoupin.top

Go:   arr[1:4]
来源：http://tht.hnxiangtu.top

Ruby: arr[1, 3]
来源：http://uvr.zhongyouzk.top

C#:   list.GetRange(1, 3);
来源：http://ixy.jqgfzy.top

[D08] 合并两个数组
来源：http://aej.sxryk.cn

Py:   a + b;  a.extend(b)
来源：http://ccg.xuanzx.com

PHP:  array_merge($a, $b);
来源：http://cmc.sysykeji.top

JS:   [...a, ...b];  a.concat(b);
来源：http://wcn.jiagoushi.top

TS:   [...a, ...b];
来源：http://gqm.yongpay.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tyq.c1oappe.top

Go:   append(a, b...)
来源：http://plv.gogol.net.cn

Ruby: a + b;  a.concat(b)
来源：http://bmz.hongshengwenyu.top

C#:   a.Concat(b).ToList()
来源：http://lxu.dashuyun.cn

[D09] 排序（升序）
来源：http://cls.jinghuilouyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://ryh.tarul.cn

PHP:  sort($arr);
来源：http://wxj.gaohongyu789.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pli.jiagoushi.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ikr.daxiang520.top

Java: Collections.sort(list);  list.sort(null);
来源：http://xij.chenlongwang.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://omy.sxryk.cn

Ruby: arr.sort
来源：http://kco.fehbvm.com

C#:   list.Sort();
来源：http://uxq.316326.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://pqs.yueranfly.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ocy.birdmap.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ujg.jiagoushi.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jbs.hysaishi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rqj.yfazqb.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vbg.yueranfly.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hgl.shangyingyoupin.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ybk.jinqigufen.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://eij.sysykeji.top

[D11] 反转数组
来源：http://yfy.bbcook.cn

Py:   arr[::-1];  arr.reverse()
来源：http://mee.yonumen.top

PHP:  array_reverse($arr);
来源：http://ucm.yangfankeji.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://aja.yvedp.cn

TS:   [...arr].reverse();
来源：http://gfa.tarul.cn

Java: Collections.reverse(list);
来源：http://cdh.9152youxi.cn

Go:   slices.Reverse(arr)
来源：http://gnh.nwbrower.top

Ruby: arr.reverse
来源：http://wlf.ivvv.top

C#:   list.Reverse();
来源：http://tvq.xinyue.icu

[D12] 查找元素下标
来源：http://jwz.daria6918.cn

Py:   arr.index(x);  x in arr
来源：http://txq.wangshuangyany.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ycd.jyoumei.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://esk.fanxiaobao.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bxb.jqgfzy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://isc.cucudq.cn

Go:   slices.Index(arr, x)
来源：http://fhb.aibaodan.cn

Ruby: arr.index(x)
来源：http://yqq.yueranfly.top

C#:   list.IndexOf(x);
来源：http://qnn.feifeiyinyue.top

[D13] 过滤（保留满足条件的）
来源：http://gje.vehdjk.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sct.hnxiangtu.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://frz.vehdjk.com

JS:   arr.filter(x => x > 3)
来源：http://jfl.hywenlv.cn

TS:   arr.filter(x => x > 3)
来源：http://nlb.ctjpmb.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cbi.yj202588.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://eoc.9152youxi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fhl.xingfuxueyuan.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://fzx.quarkkingdee.top

[D14] 映射转换（每个元素变形）
来源：http://wlt.ppjwa.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bej.zhongyouzk.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yeo.andypj.xyz

JS:   arr.map(x => x * 2)
来源：http://wqd.316326.xyz

TS:   arr.map(x => x * 2)
来源：http://jec.jyoumei.cn


<!-- 参考信息 -->