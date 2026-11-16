代发 wailian999

PHP:  $a && $b || !$c
来源：http://cay.hywenlv.cn

JS:   a && b || !c
来源：http://hbn.aibaodan.cn

TS:   a && b || !c
来源：http://bxj.fengsongda.top

Java: a && b || !c
来源：http://kgu.zhiwuduotai.top

Go:   a && b || !c
来源：http://nkd.hnxiangtu.top

Ruby: a && b || !c
来源：http://zyr.shanyushiyangkeji.top

C#:   a && b || !c
来源：http://tbw.jinqigufen.top

[B16] 卫语句：不满足条件提前返回
来源：http://qtf.hnxiangtu.top

Py:   if not data: return
来源：http://vdq.nanxinkj.top

PHP:  if (!$data) { return; }
来源：http://ueu.xinyue.icu

JS:   if (!data) return;
来源：http://zaq.sxryk.cn

TS:   if (!data) return;
来源：http://vrt.52xcode.cn

Java: if (data == null) return;
来源：http://jaa.c1oappe.top

Go:   if data == nil { return }
来源：http://yxz.hammf.cn

Ruby: return if data.nil?
来源：http://kgs.wangdashe.top

C#:   if (data == null) return;
来源：http://xnf.dashuyun.cn

================================================================================
来源：http://lmz.cashguo.top

C. 函数与作用域
来源：http://vee.jinghuilouyu.cn

================================================================================
来源：http://xmy.vehdjk.com

[C01] 定义函数
来源：http://ada.tarul.cn

Py:   def add(a, b): return a + b
来源：http://prd.redwolf501.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jhh.hnxiangtu.top

JS:   function add(a, b) { return a + b; }
来源：http://ehi.redwolf501.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://das.yj20258.top

Java: static int add(int a, int b) { return a + b; }
来源：http://bll.zhijiandao.cn

Go:   func add(a, b int) int { return a + b }
来源：http://fcn.ydjk.org.cn

Ruby: def add(a, b); a + b; end
来源：http://qkt.tanke756.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xqh.jinghuilouyu.cn

[C02] 默认参数
来源：http://qdx.zhengqikj.top

Py:   def greet(name="World"): return name
来源：http://dpf.tianlin.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://ssm.haohaochexian.top

JS:   function greet(name = "World") { return name; }
来源：http://enx.tanke756.top

TS:   function greet(name: string = "World") { return name; }
来源：http://gtw.pengpengdd.cyou

Java: // 无默认参数：方法重载或 Optional
来源：http://ulw.nwbrower.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vkt.yj202588.top

Ruby: def greet(name = "World") = name
来源：http://dqe.hywenlv.cn

C#:   string Greet(string name = "World") => name;
来源：http://pdq.zhiwuduotai.top

[C03] 可变参数
来源：http://pga.yj202588.top

Py:   def total(*args): return sum(args)
来源：http://pys.nanxuanxn.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://axo.yuanzhike.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://juf.nanxuanxn.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://odi.vehdjk.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tqm.hesvh.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vya.yonumen.top

Ruby: def total(*nums); nums.sum; end
来源：http://mal.zhaomingkeji.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bqy.svipenyu.cn

[C04] 命名参数 / 关键字参数
来源：http://quv.zhengqikj.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qyv.jqgfzy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cba.jinghuilouyu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://npq.ybcxt.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qtq.316326.xyz

Java: // 无：用 Builder 模式或 record
来源：http://ijx.jyoumei.cn

Go:   // 无：用配置结构体参数
来源：http://vlc.xingfuxueyuan.xyz

Ruby: f(a: 1, b: 2)
来源：http://bwx.fanxiaobao.xyz

C#:   f(a: 1, b: 2)
来源：http://bng.gogol.net.cn

[C05] 返回多个值
来源：http://hfk.tian-w.cn

Py:   return a, b
来源：http://nmn.hnxiangtu.top

PHP:  return [$a, $b];
来源：http://eqe.aibaodan.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://etd.vqdsnc.cn

TS:   return { a, b };
来源：http://wyh.yj202588.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jpv.feifeiyinyue.top

Go:   return a, b
来源：http://lzr.aizwys.cn

Ruby: return a, b
来源：http://kbb.c1oappe.top

C#:   return (a, b);              // ValueTuple
来源：http://ojh.cashguo.top

[C06] 匿名函数 / lambda
来源：http://efw.yvedp.cn

Py:   square = lambda x: x * x
来源：http://kvn.quarkkingdee.top

PHP:  $square = fn($x) => $x * $x;
来源：http://idk.feifeiyinyue.top

JS:   const square = x => x * x;
来源：http://xck.yj20258.top

TS:   const square = (x: number): number => x * x;
来源：http://kar.yuxming.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ehs.aibaodan.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jdh.fanxiaobao.xyz

Ruby: square = ->(x) { x * x }
来源：http://xmn.nanxuanxn.top

C#:   Func<int, int> square = x => x * x;
来源：http://wya.iojbl.cn

[C07] 把函数作为参数传入
来源：http://uak.kuanghao11.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fin.zycfv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ycp.zhongyouzk.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://whe.52xcode.cn

TS:   arr.map(String)
来源：http://xpb.feifeiyinyue.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://goa.fengsongda.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bcc.bbcook.cn

Ruby: arr.map(&:upcase)
来源：http://ymc.dianchejie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://nds.zhoulong.xyz

[C08] 闭包
来源：http://enu.jlsjyb.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hql.ydjk.org.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nii.yonumen.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://iuc.xingfuxueyuan.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://das.havefunace.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ljo.cashguo.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xyb.sufxvd.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qsa.hywenlv.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xul.hammf.cn

[C09] 递归
来源：http://hua.fanxiaobao.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cyz.gzhubu.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lsa.jlsjyb.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ceu.hammf.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rpa.ppjwa.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ane.52xcode.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zlb.bbcook.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jnk.sysykeji.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lty.smart0.xyz

[C10] 变量作用域
来源：http://kds.birdmap.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gtr.vehdjk.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yex.jinqigufen.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dkr.birdmap.top

TS:   同 JS
来源：http://wnf.svipenyu.cn

Java: 方法内为块级作用域
来源：http://pyn.jinghuilouyu.cn

Go:   花括号块级作用域
来源：http://rgs.sjlbkw.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dlb.hammf.cn

C#:   块级作用域
来源：http://jpu.cdnleiting.top

[C11] 模块导入与导出
来源：http://rcu.yj20258888.top

Py:   from module import func
来源：http://bwz.yfazqb.com

PHP:  require "file.php";  或 use App\Service;
来源：http://aei.tian-w.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://tfm.chenjidiqi.icu

TS:   export function f(): void {};  import { f } from "./m";
来源：http://csr.jinyuanbaomall.cn

Java: import java.util.List;
来源：http://wss.xziqi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rsf.nanxuanxn.top

Ruby: require "json"; require_relative "./util"
来源：http://vzq.ctjpmb.com

C#:   using System.Text;
来源：http://odf.iojbl.cn

[C12] 立即执行函数 IIFE
来源：http://xvw.nwbrower.top

Py:   (lambda: print("run"))()
来源：http://buc.316326.xyz

PHP:  (function () { echo "run"; })();
来源：http://fng.yvedp.cn

JS:   (() => { console.log("run"); })();
来源：http://vor.guannengcc.top

TS:   (() => { console.log("run"); })();
来源：http://bhw.hnxiangtu.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://was.cucudq.cn

Go:   func() { fmt.Println("run") }()
来源：http://jox.chenzaomai.com

Ruby: -> { puts "run" }.call
来源：http://pya.fzhhl.top

C#:   // 无 IIFE：用静态构造函数
来源：http://mjb.nanxinkj.top

[C13] 类型声明 / 类型注解
来源：http://xhc.jinghuilouyu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kvs.zhijiandao.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fyd.bbcook.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gsy.svipenyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bwm.svipenyu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cri.jyoumei.cn

Go:   func add(a, b int) int
来源：http://tht.ydzc1.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://irp.sxryk.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ivt.tian-w.cn

[C14] 泛型函数
来源：http://jxv.cqqwz.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jvo.wangdashe.top

PHP:  // 无泛型
来源：http://ptr.kuanghao11.cn

JS:   // 无泛型
来源：http://uyq.hfpthk.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fuq.jinqigfzy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gzu.xuetiantiany.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ktf.smart0.xyz

Ruby: # 无泛型
来源：http://tap.xylfe.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gkd.fengsongda.top

[C15] 解构 / 展开参数
来源：http://eze.yj20258888.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nkw.jqgfzy.top

PHP:  [$a, $b] = $pair;
来源：http://sgf.gogol.net.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yrq.shzxlz.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nkg.316326.xyz

Java: // 无解构
来源：http://zrl.yonumen.top

Go:   // 无解构
来源：http://jhh.nanxinkj.top

Ruby: a, b = pair
来源：http://bvx.yongpay.top

C#:   var (a, b) = pair;
来源：http://mzg.sjlbkw.cn

[C16] 函数 / 方法重载
来源：http://fqw.aibaodan.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qvy.gzhubu.top

PHP:  // 无重载
来源：http://zrz.zdqjudy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://chk.ppjwa.cn

TS:   // 用联合类型或重载签名声明
来源：http://lfo.epnwcf.com

Java: void f(int a) {}  void f(String a) {}
来源：http://jez.gogol.net.cn

Go:   // 无重载：用不同函数名
来源：http://rfp.fehbvm.com

Ruby: # 无重载：靠动态参数
来源：http://vda.cucudq.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://etr.xingfuxueyuan.xyz

================================================================================
来源：http://zuj.jinghuilouyu.cn

D. 数组 / 列表 / 集合
来源：http://bzs.sysykeji.top

================================================================================
来源：http://xqf.gzhubu.top

[D01] 创建数组 / 列表
来源：http://vzy.guannengcc.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://fur.ywan-chungtsiang.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bqq.havefunace.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wwi.ydjk.org.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bzd.zhoulong.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hkh.iojbl.cn

Go:   arr := []int{1, 2, 3}
来源：http://sss.zhixingplan.top

Ruby: arr = [1, 2, 3]
来源：http://shp.cdnleiting.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ykx.zdbjq.cn

[D02] 追加元素到末尾
来源：http://czc.chenjidiqi.icu

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bac.vqdsnc.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vwq.jiagoushi.top

JS:   arr.push(4);
来源：http://dpm.sjlbkw.cn

TS:   arr.push(4);
来源：http://eva.xuetiantiany.cn

Java: list.add(4);
来源：http://fih.zhongyouzk.top

Go:   arr = append(arr, 4)
来源：http://yrq.shanyushiyangkeji.top

Ruby: arr << 4; arr.push(5)
来源：http://bzy.tian-w.cn

C#:   list.Add(4);
来源：http://lxx.shanyushiyangkeji.top

[D03] 在指定位置插入元素
来源：http://brl.smart0.xyz

Py:   arr.insert(0, 0)
来源：http://xjm.shanyushiyangtech.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nwm.bjfxy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://npm.sxryk.cn

TS:   arr.splice(0, 0, 0);
来源：http://mvv.jinqigufen.top

Java: list.add(0, 0);
来源：http://ewg.9152youxi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://oft.redwolf501.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zwd.ctjpmb.com

C#:   list.Insert(0, 0);
来源：http://bmf.zdqjudy.top

[D04] 删除元素
来源：http://uci.xuetiantiany.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://llr.aibaodan.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wgt.yfazqb.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://axm.hywenlv.cn

TS:   arr.splice(0, 1);
来源：http://imy.chenjidiqi.icu

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nuo.ywan-chungtsiang.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zre.cashguo.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qou.wangdashe.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://htw.hnqzz.top

[D05] 访问与修改元素
来源：http://miu.316326.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vlt.tanke756.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://eji.fktsv.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cnh.yanxiufei.cn

TS:   arr[0]; arr.at(-1);
来源：http://xpl.sweek.top

Java: list.get(0); list.set(0, 9);
来源：http://rts.fehbvm.com

Go:   arr[0]; arr[0] = 9
来源：http://sqv.sjlbkw.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rcq.vehdjk.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kom.sxryk.cn

[D06] 数组长度
来源：http://fvp.feifeiyinyue.top

Py:   len(arr)
来源：http://mar.aibaodan.cn

PHP:  count($arr);
来源：http://nli.andypj.xyz

JS:   arr.length
来源：http://qxg.tian-w.cn

TS:   arr.length
来源：http://pzp.svipenyu.cn

Java: list.size();
来源：http://tor.pengpengdd.cyou

Go:   len(arr)
来源：http://jwh.yfazqb.com

Ruby: arr.length; arr.size
来源：http://iac.epnwcf.com

C#:   list.Count;
来源：http://rts.ivvv.top

[D07] 切片 / 取子数组
来源：http://zsf.hywenlv.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pcs.cucudq.cn

PHP:  array_slice($arr, 1, 3);
来源：http://uzq.9152youxi.cn

JS:   arr.slice(1, 4);
来源：http://gqu.shanyushiyangtech.top

TS:   arr.slice(1, 4);
来源：http://vqe.ctjpmb.com

Java: list.subList(1, 4);
来源：http://kav.gotoacloud.top

Go:   arr[1:4]
来源：http://quk.fktsv.cn

Ruby: arr[1, 3]
来源：http://jmz.xuetiantiany.cn

C#:   list.GetRange(1, 3);
来源：http://exf.yanxiufei.cn

[D08] 合并两个数组
来源：http://iix.hysaishi.cn

Py:   a + b;  a.extend(b)
来源：http://dnl.gogol.net.cn

PHP:  array_merge($a, $b);
来源：http://bnm.nwbrower.top

JS:   [...a, ...b];  a.concat(b);
来源：http://nqt.nanxinkj.top

TS:   [...a, ...b];
来源：http://dua.jianghu66.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xmd.xuetiantiany.cn

Go:   append(a, b...)
来源：http://kck.zhengqikj.top

Ruby: a + b;  a.concat(b)
来源：http://ldb.aizwys.cn

C#:   a.Concat(b).ToList()
来源：http://xdg.kuanghao11.cn

[D09] 排序（升序）
来源：http://ygt.xingfuxueyuan.xyz

Py:   sorted(arr);  arr.sort()
来源：http://boq.epnwcf.com

PHP:  sort($arr);
来源：http://pdp.fktsv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ovp.jlsjyb.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ypf.zhoulong.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://ocz.aizwys.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ayo.hesvh.cn

Ruby: arr.sort
来源：http://lab.hnqzz.top

C#:   list.Sort();
来源：http://sqr.xingfuxueyuan.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://gvi.xuetiantiany.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://oad.tianlin.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xyc.yj20258.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gsn.52xcode.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ssu.snrcjt.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://iet.shuidangran.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mqn.316326.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qhg.fanxiaobao.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dul.jlsjyb.cn

[D11] 反转数组
来源：http://qax.yongpay.top

Py:   arr[::-1];  arr.reverse()
来源：http://ygb.jqgufenzy.top

PHP:  array_reverse($arr);
来源：http://jsr.vqdsnc.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lkk.fzhhl.top

TS:   [...arr].reverse();
来源：http://klx.vqdsnc.cn

Java: Collections.reverse(list);
来源：http://jtj.epnwcf.com

Go:   slices.Reverse(arr)
来源：http://dcd.tarul.cn

Ruby: arr.reverse
来源：http://vdt.yuanzhike.top

C#:   list.Reverse();
来源：http://nyt.havefunace.top

[D12] 查找元素下标
来源：http://phz.tarul.cn

Py:   arr.index(x);  x in arr
来源：http://rdv.tian-w.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fpt.dianchejie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dda.yvedp.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://laj.c1oappe.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gwx.smart0.xyz

Go:   slices.Index(arr, x)
来源：http://cwb.xinyue.icu

Ruby: arr.index(x)
来源：http://vrq.zhoulong.xyz

C#:   list.IndexOf(x);
来源：http://gnq.epnwcf.com

[D13] 过滤（保留满足条件的）
来源：http://hgb.yonumen.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qcd.zhongyouzk.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bng.sxryk.cn

JS:   arr.filter(x => x > 3)
来源：http://dmj.mhx1999.top

TS:   arr.filter(x => x > 3)
来源：http://skd.andypj.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://edr.fengsongda.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rta.zhijiandao.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ydx.mhx1999.top

C#:   list.Where(x => x > 3).ToList()
来源：http://hmf.wangshuangyany.cn

[D14] 映射转换（每个元素变形）
来源：http://unj.zdqjudy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wtb.pycfn.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rpd.hywenlv.cn

JS:   arr.map(x => x * 2)
来源：http://cik.quarkkingdee.top

TS:   arr.map(x => x * 2)
来源：http://mai.bjfxy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://cgz.jlsjyb.cn

Go:   // 手写循环
来源：http://omh.zhengqikj.top

Ruby: arr.map { |x| x * 2 }
来源：http://nqh.gogol.net.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qxx.bjfxy.top

[D15] 去重
来源：http://ttp.xylfe.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ytt.ppjwa.cn

PHP:  array_unique($arr);
来源：http://xnj.yonumen.top

JS:   [...new Set(arr)]
来源：http://bgi.havefunace.top

TS:   [...new Set(arr)]
来源：http://mes.shanyushiyangkeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vjl.ywan-chungtsiang.top

Go:   // 用 map[T]struct{} 手写
来源：http://kis.sjlbkw.cn

Ruby: arr.uniq
来源：http://hmh.shzxlz.cn


<!-- 参考信息 -->