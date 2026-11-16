代发 wailian999

C#:   x is int or double or decimal
来源：http://ojd.jinyuanbaomall.cn

[B14] 判断值是否在集合内
来源：http://wpy.svipenyu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cwq.cheryme.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yjy.redwolf501.top

JS:   [1, 2, 3].includes(x)
来源：http://zbr.nanxinkj.top

TS:   [1, 2, 3].includes(x)
来源：http://vsw.quarkkingdee.top

Java: List.of(1, 2, 3).contains(x)
来源：http://mof.aibaodan.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bvu.xuetiantiany.cn

Ruby: [1, 2, 3].include?(x)
来源：http://mex.xziqi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fwu.shuidangran.top

[B15] 布尔运算与取反
来源：http://pze.quarkkingdee.top

Py:   a and b or not c
来源：http://ksd.fanxiaobao.xyz

PHP:  $a && $b || !$c
来源：http://usq.zhaomingkeji.xyz

JS:   a && b || !c
来源：http://cuo.sjlbkw.cn

TS:   a && b || !c
来源：http://jhn.meibo888.top

Java: a && b || !c
来源：http://qpo.sysykeji.top

Go:   a && b || !c
来源：http://lpx.chenjidiqi.icu

Ruby: a && b || !c
来源：http://bgu.shzxlz.cn

C#:   a && b || !c
来源：http://zxt.chenjidiqi.icu

[B16] 卫语句：不满足条件提前返回
来源：http://ype.gaohongyu789.top

Py:   if not data: return
来源：http://afy.tarul.cn

PHP:  if (!$data) { return; }
来源：http://gjp.hcnkem.com

JS:   if (!data) return;
来源：http://nvj.hywenlv.cn

TS:   if (!data) return;
来源：http://mfy.yj20258.top

Java: if (data == null) return;
来源：http://zqk.zhaomingkeji.xyz

Go:   if data == nil { return }
来源：http://xxx.aibaodan.cn

Ruby: return if data.nil?
来源：http://axy.52xcode.cn

C#:   if (data == null) return;
来源：http://oob.ydzc1.top

================================================================================
来源：http://lyf.daria6918.cn

C. 函数与作用域
来源：http://uxw.zdqjudy.top

================================================================================
来源：http://rtd.yuxming.cn

[C01] 定义函数
来源：http://qbv.daxiang520.top

Py:   def add(a, b): return a + b
来源：http://lya.guannengcc.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ijy.shuidangran.top

JS:   function add(a, b) { return a + b; }
来源：http://xbl.52xcode.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ehk.cashguo.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ygl.zhixingplan.top

Go:   func add(a, b int) int { return a + b }
来源：http://zkb.cdnleiting.top

Ruby: def add(a, b); a + b; end
来源：http://reu.sweek.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://luz.hysaishi.cn

[C02] 默认参数
来源：http://ucu.hysaishi.cn

Py:   def greet(name="World"): return name
来源：http://ynf.fehbvm.com

PHP:  function greet($name = "World") { return $name; }
来源：http://thb.ctjpmb.com

JS:   function greet(name = "World") { return name; }
来源：http://jrr.vehdjk.com

TS:   function greet(name: string = "World") { return name; }
来源：http://ukc.jqgufenzy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://kwl.yj20258.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xmq.c1oappe.top

Ruby: def greet(name = "World") = name
来源：http://cdl.jyoumei.cn

C#:   string Greet(string name = "World") => name;
来源：http://gog.hammf.cn

[C03] 可变参数
来源：http://jla.gzhubu.top

Py:   def total(*args): return sum(args)
来源：http://xte.jlsjyb.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rvt.vqdsnc.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bjz.jinghuilouyu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uvc.nanxinkj.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bio.guannengcc.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qbr.ctjpmb.com

Ruby: def total(*nums); nums.sum; end
来源：http://usj.yonumen.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nfj.xziqi.cn

[C04] 命名参数 / 关键字参数
来源：http://njp.jlsjyb.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://urv.shzxlz.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://usk.pycfn.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cnu.xinyue.icu

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zzj.shanyushiyangtech.top

Java: // 无：用 Builder 模式或 record
来源：http://wml.vqdsnc.cn

Go:   // 无：用配置结构体参数
来源：http://gac.sxryk.cn

Ruby: f(a: 1, b: 2)
来源：http://tqr.jqgfzy.top

C#:   f(a: 1, b: 2)
来源：http://dqk.ywan-chungtsiang.top

[C05] 返回多个值
来源：http://amh.redwolf501.top

Py:   return a, b
来源：http://orv.yanxiufei.cn

PHP:  return [$a, $b];
来源：http://feo.gzhubu.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://viu.wangdashe.top

TS:   return { a, b };
来源：http://wez.svipenyu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mhx.yonumen.top

Go:   return a, b
来源：http://rum.tarul.cn

Ruby: return a, b
来源：http://iat.zycfv.cn

C#:   return (a, b);              // ValueTuple
来源：http://ouw.cqqwz.cn

[C06] 匿名函数 / lambda
来源：http://vqm.fengsongda.top

Py:   square = lambda x: x * x
来源：http://xch.jinqigufen.top

PHP:  $square = fn($x) => $x * $x;
来源：http://day.shzxlz.cn

JS:   const square = x => x * x;
来源：http://lbm.redwolf501.top

TS:   const square = (x: number): number => x * x;
来源：http://kwt.zhiwuduotai.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kar.pengpengdd.cyou

Go:   sq := func(x int) int { return x * x }
来源：http://jrz.tarul.cn

Ruby: square = ->(x) { x * x }
来源：http://toy.yj20258888.top

C#:   Func<int, int> square = x => x * x;
来源：http://ois.gaohongyu789.top

[C07] 把函数作为参数传入
来源：http://kkz.ctjpmb.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pzg.aizwys.cn

PHP:  array_map("strtoupper", $arr);
来源：http://voz.pengpengdd.cyou

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://otn.fktsv.cn

TS:   arr.map(String)
来源：http://kol.daria6918.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ynz.chenzaomai.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://def.zdqjudy.top

Ruby: arr.map(&:upcase)
来源：http://ggk.havefunace.top

C#:   arr.Select(s => s.ToUpper())
来源：http://thi.yongpay.top

[C08] 闭包
来源：http://rfh.snrcjt.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vfu.yj20258888.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lea.fengsongda.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ogn.ywan-chungtsiang.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://olw.smart0.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pzk.nwbrower.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vvl.yangfankeji.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vqm.c1oappe.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bku.vehdjk.com

[C09] 递归
来源：http://kmk.sweek.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dwy.jinqigufen.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jxc.zhaomingkeji.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pja.ywan-chungtsiang.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gpm.nanxinkj.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ywh.nanxuanxn.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cki.sxryk.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bgq.xuanzx.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rid.zhiwuduotai.top

[C10] 变量作用域
来源：http://ier.jqgfzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qdq.zhixingplan.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zfx.yfazqb.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://emb.ywan-chungtsiang.top

TS:   同 JS
来源：http://vev.kuanghao11.cn

Java: 方法内为块级作用域
来源：http://apk.zdbjq.cn

Go:   花括号块级作用域
来源：http://qtd.fengsongda.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pzu.daria6918.cn

C#:   块级作用域
来源：http://izj.zycfv.cn

[C11] 模块导入与导出
来源：http://huz.yj20258888.top

Py:   from module import func
来源：http://tqm.zdqjudy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://odm.jinqigufen.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://hpq.zhongyouzk.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pnp.iojbl.cn

Java: import java.util.List;
来源：http://nlu.epnwcf.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://eas.tanke756.top

Ruby: require "json"; require_relative "./util"
来源：http://gkx.chenlongwang.top

C#:   using System.Text;
来源：http://oiq.yongpay.top

[C12] 立即执行函数 IIFE
来源：http://vld.tanke756.top

Py:   (lambda: print("run"))()
来源：http://efv.xingfuxueyuan.xyz

PHP:  (function () { echo "run"; })();
来源：http://vgz.feifeiyinyue.top

JS:   (() => { console.log("run"); })();
来源：http://hcj.52xcode.cn

TS:   (() => { console.log("run"); })();
来源：http://wyk.jlsjyb.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lhj.smart0.xyz

Go:   func() { fmt.Println("run") }()
来源：http://swv.yonumen.top

Ruby: -> { puts "run" }.call
来源：http://giz.chenjidiqi.icu

C#:   // 无 IIFE：用静态构造函数
来源：http://vrd.xingfuxueyuan.xyz

[C13] 类型声明 / 类型注解
来源：http://vti.hongshengwenyu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ogk.tanke756.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://itv.52xcode.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hfg.shanyushiyangtech.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xbo.wangdashe.top

Java: int add(int a, int b) { return a + b; }
来源：http://gto.yfazqb.com

Go:   func add(a, b int) int
来源：http://cid.sufxvd.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lse.svipenyu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qvw.jinqigfzy.top

[C14] 泛型函数
来源：http://gho.yueranfly.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://all.havefunace.top

PHP:  // 无泛型
来源：http://ldk.yueranfly.top

JS:   // 无泛型
来源：http://ubs.kuanghao11.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xym.yj202588.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ihq.jlsjyb.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://uzm.sysykeji.top

Ruby: # 无泛型
来源：http://qvq.hongshengwenyu.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sjq.jinyuanbaomall.cn

[C15] 解构 / 展开参数
来源：http://vmk.shanyushiyangtech.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xbl.hammf.cn

PHP:  [$a, $b] = $pair;
来源：http://uli.fanxiaobao.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hkb.yvedp.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dqk.9152youxi.cn

Java: // 无解构
来源：http://fld.fanxiaobao.xyz

Go:   // 无解构
来源：http://ges.shangyingyoupin.top

Ruby: a, b = pair
来源：http://xyp.ehwqpu.com

C#:   var (a, b) = pair;
来源：http://zut.hammf.cn

[C16] 函数 / 方法重载
来源：http://mvx.yangfankeji.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gof.yanxiufei.cn

PHP:  // 无重载
来源：http://afh.redwolf501.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://cug.uphjek.com

TS:   // 用联合类型或重载签名声明
来源：http://szc.ywan-chungtsiang.top

Java: void f(int a) {}  void f(String a) {}
来源：http://mff.xinyue.icu

Go:   // 无重载：用不同函数名
来源：http://tjc.yj20258888.top

Ruby: # 无重载：靠动态参数
来源：http://ijf.9152youxi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://mjn.jinqigufen.top

================================================================================
来源：http://kmr.haohaochexian.top

D. 数组 / 列表 / 集合
来源：http://jxn.redwolf501.top

================================================================================
来源：http://tqn.bjfxy.top

[D01] 创建数组 / 列表
来源：http://bti.xinyue.icu

Py:   arr = [1, 2, 3];  empty = []
来源：http://osb.yuanzhike.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cbt.hysaishi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hjk.hammf.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://tgd.hysaishi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wwy.zycfv.cn

Go:   arr := []int{1, 2, 3}
来源：http://lvm.nwbrower.top

Ruby: arr = [1, 2, 3]
来源：http://xcl.shuidangran.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bbg.sysykeji.top

[D02] 追加元素到末尾
来源：http://swh.jqgufenzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ydq.xuanzx.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://axg.zycfv.cn

JS:   arr.push(4);
来源：http://fqc.yj20258888.top

TS:   arr.push(4);
来源：http://ybp.tarul.cn

Java: list.add(4);
来源：http://irg.jiagoushi.top

Go:   arr = append(arr, 4)
来源：http://nkn.tarul.cn

Ruby: arr << 4; arr.push(5)
来源：http://lng.tanke756.top

C#:   list.Add(4);
来源：http://axa.zhijiandao.cn

[D03] 在指定位置插入元素
来源：http://nkv.vqdsnc.cn

Py:   arr.insert(0, 0)
来源：http://rhu.dianchejie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://whr.gzhubu.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wwx.jqgufenzy.top

TS:   arr.splice(0, 0, 0);
来源：http://kxh.xuanzx.com

Java: list.add(0, 0);
来源：http://ref.sweek.top

Go:   arr = append([]int{0}, arr...)
来源：http://uum.hongshengwenyu.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xbz.uphjek.com

C#:   list.Insert(0, 0);
来源：http://lcn.jyoumei.cn

[D04] 删除元素
来源：http://kul.hysaishi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mtu.hcnkem.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ubd.vehdjk.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rwa.yfazqb.com

TS:   arr.splice(0, 1);
来源：http://xvc.hnxiangtu.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://oro.xuetiantiany.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xld.c1oappe.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://oxa.hcnkem.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xoc.yvedp.cn

[D05] 访问与修改元素
来源：http://rfz.epnwcf.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ayk.hnqzz.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xnw.jinyuanbaomall.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ytb.jyoumei.cn

TS:   arr[0]; arr.at(-1);
来源：http://von.ybcxt.top

Java: list.get(0); list.set(0, 9);
来源：http://ite.cqqwz.cn

Go:   arr[0]; arr[0] = 9
来源：http://tts.bbcook.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wxa.chenlongwang.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://npg.yuxming.cn

[D06] 数组长度
来源：http://ozu.yanxiufei.cn

Py:   len(arr)
来源：http://lap.sxryk.cn

PHP:  count($arr);
来源：http://hiv.yj20258888.top

JS:   arr.length
来源：http://zdb.yvedp.cn

TS:   arr.length
来源：http://qbl.tianlin.xyz

Java: list.size();
来源：http://djb.hesvh.cn

Go:   len(arr)
来源：http://orm.zycfv.cn

Ruby: arr.length; arr.size
来源：http://zer.zdqjudy.top

C#:   list.Count;
来源：http://grl.zdbjq.cn

[D07] 切片 / 取子数组
来源：http://ocy.yfazqb.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qwy.uphjek.com

PHP:  array_slice($arr, 1, 3);
来源：http://bhp.redwolf501.top

JS:   arr.slice(1, 4);
来源：http://nxr.uphjek.com

TS:   arr.slice(1, 4);
来源：http://nyk.ehwqpu.com

Java: list.subList(1, 4);
来源：http://ufv.cashguo.top

Go:   arr[1:4]
来源：http://mcz.yj20258.top

Ruby: arr[1, 3]
来源：http://avn.xuetiantiany.cn

C#:   list.GetRange(1, 3);
来源：http://xbd.fzhhl.top

[D08] 合并两个数组
来源：http://jnf.epnwcf.com

Py:   a + b;  a.extend(b)
来源：http://zkz.sweek.top

PHP:  array_merge($a, $b);
来源：http://how.9152youxi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://fbd.aibaodan.cn

TS:   [...a, ...b];
来源：http://ngq.zhijiandao.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rhn.zhiwuduotai.top

Go:   append(a, b...)
来源：http://mfn.havefunace.top

Ruby: a + b;  a.concat(b)
来源：http://xqd.svipenyu.cn

C#:   a.Concat(b).ToList()
来源：http://ept.gotoacloud.top

[D09] 排序（升序）
来源：http://krt.wangdashe.top

Py:   sorted(arr);  arr.sort()
来源：http://mjq.cqqwz.cn

PHP:  sort($arr);
来源：http://hdl.ehwqpu.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ckf.xinyue.icu

TS:   [...arr].sort((x, y) => x - y);
来源：http://shl.pengpengdd.cyou

Java: Collections.sort(list);  list.sort(null);
来源：http://jrp.tianlin.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tgb.sysykeji.top

Ruby: arr.sort
来源：http://ybs.haohaochexian.top

C#:   list.Sort();
来源：http://ugu.fktsv.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://lsn.sysykeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wdo.jinqigfzy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://riu.xziqi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ydf.fehbvm.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dlq.svipenyu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ril.hongshengwenyu.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xsw.zdqjudy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cgl.chenzaomai.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://piy.pengpengdd.cyou

[D11] 反转数组
来源：http://auw.nanxuanxn.top

Py:   arr[::-1];  arr.reverse()
来源：http://brt.hywenlv.cn

PHP:  array_reverse($arr);
来源：http://boo.snrcjt.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nhb.ybcxt.top

TS:   [...arr].reverse();
来源：http://dxj.ywan-chungtsiang.top

Java: Collections.reverse(list);
来源：http://mll.zdbjq.cn

Go:   slices.Reverse(arr)
来源：http://zwc.pycfn.com

Ruby: arr.reverse
来源：http://jdz.jlsjyb.cn

C#:   list.Reverse();
来源：http://xga.nwbrower.top

[D12] 查找元素下标
来源：http://nfr.fktsv.cn

Py:   arr.index(x);  x in arr
来源：http://ier.tanke756.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hif.nwbrower.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uwu.xuetiantiany.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yzv.xuanzx.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wdc.jinghuilouyu.cn

Go:   slices.Index(arr, x)
来源：http://pha.hongshengwenyu.top

Ruby: arr.index(x)
来源：http://rvt.hnxiangtu.top

C#:   list.IndexOf(x);
来源：http://trj.yongpay.top

[D13] 过滤（保留满足条件的）
来源：http://bnq.zdqjudy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dbb.fzhhl.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jgf.gotoacloud.top

JS:   arr.filter(x => x > 3)
来源：http://fpq.hesvh.cn

TS:   arr.filter(x => x > 3)
来源：http://hdf.gotoacloud.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://feo.ydjk.org.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ydq.xingfuxueyuan.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://ftl.yonumen.top

C#:   list.Where(x => x > 3).ToList()
来源：http://jbv.shuidangran.top

[D14] 映射转换（每个元素变形）
来源：http://vne.zhijiandao.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nvs.hysaishi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hnj.yongpay.top

JS:   arr.map(x => x * 2)
来源：http://ceb.yj20258.top

TS:   arr.map(x => x * 2)
来源：http://wav.wangdashe.top


<!-- 参考信息 -->