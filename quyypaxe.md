代发 wailian999

Py:   if not data: return
来源：http://mpm.xingfuxueyuan.xyz

PHP:  if (!$data) { return; }
来源：http://lzl.jianghu66.top

JS:   if (!data) return;
来源：http://oyw.redwolf501.top

TS:   if (!data) return;
来源：http://rgf.hysaishi.cn

Java: if (data == null) return;
来源：http://bdw.quarkkingdee.top

Go:   if data == nil { return }
来源：http://akh.fzhhl.top

Ruby: return if data.nil?
来源：http://ypw.shuidangran.top

C#:   if (data == null) return;
来源：http://xxu.ybcxt.top

================================================================================
来源：http://iqm.cucudq.cn

C. 函数与作用域
来源：http://rjf.tianlin.xyz

================================================================================
来源：http://ftc.hongshengwenyu.top

[C01] 定义函数
来源：http://spx.vehdjk.com

Py:   def add(a, b): return a + b
来源：http://xze.haohaochexian.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oqb.xziqi.cn

JS:   function add(a, b) { return a + b; }
来源：http://btr.hfpthk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ulr.yj20258888.top

Java: static int add(int a, int b) { return a + b; }
来源：http://xlv.ybcxt.top

Go:   func add(a, b int) int { return a + b }
来源：http://qxp.uphjek.com

Ruby: def add(a, b); a + b; end
来源：http://zpp.xingfuxueyuan.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://aln.yongpay.top

[C02] 默认参数
来源：http://qwi.zhengqikj.top

Py:   def greet(name="World"): return name
来源：http://hoh.cqqwz.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://jov.cdnleiting.top

JS:   function greet(name = "World") { return name; }
来源：http://mek.ppjwa.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fnp.yueranfly.top

Java: // 无默认参数：方法重载或 Optional
来源：http://qty.hfpthk.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nse.mhx1999.top

Ruby: def greet(name = "World") = name
来源：http://lug.nwbrower.top

C#:   string Greet(string name = "World") => name;
来源：http://vnf.wangshuangyany.cn

[C03] 可变参数
来源：http://mhg.shuidangran.top

Py:   def total(*args): return sum(args)
来源：http://wwz.pycfn.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://foi.daria6918.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kpc.yfazqb.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xru.yuanzhike.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://con.jqgfzy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xwp.zhoulong.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://oyb.jinqigufen.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lri.gzhubu.top

[C04] 命名参数 / 关键字参数
来源：http://jsk.zhixingplan.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qyq.haohaochexian.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://emy.aibaodan.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mju.jinqigfzy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wyq.0kj1m.cn

Java: // 无：用 Builder 模式或 record
来源：http://ldw.ppjwa.cn

Go:   // 无：用配置结构体参数
来源：http://bmq.yanxiufei.cn

Ruby: f(a: 1, b: 2)
来源：http://ppy.ctjpmb.com

C#:   f(a: 1, b: 2)
来源：http://xal.bjfxy.top

[C05] 返回多个值
来源：http://bqn.zhongyouzk.top

Py:   return a, b
来源：http://zux.jianghu66.top

PHP:  return [$a, $b];
来源：http://rau.zhiwuduotai.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://zjx.xziqi.cn

TS:   return { a, b };
来源：http://jfa.kuanghao11.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tca.hnxiangtu.top

Go:   return a, b
来源：http://hng.gogol.net.cn

Ruby: return a, b
来源：http://qvp.yuanzhike.top

C#:   return (a, b);              // ValueTuple
来源：http://awo.mhx1999.top

[C06] 匿名函数 / lambda
来源：http://wrh.bjfxy.top

Py:   square = lambda x: x * x
来源：http://lgc.shanyushiyangkeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://acr.yj20258.top

JS:   const square = x => x * x;
来源：http://cbg.hammf.cn

TS:   const square = (x: number): number => x * x;
来源：http://hll.bjfxy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tjr.sjlbkw.cn

Go:   sq := func(x int) int { return x * x }
来源：http://xlc.shangyingyoupin.top

Ruby: square = ->(x) { x * x }
来源：http://bac.jiagoushi.top

C#:   Func<int, int> square = x => x * x;
来源：http://rjf.daxiang520.top

[C07] 把函数作为参数传入
来源：http://cjl.jqgfzy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sdm.yj20258.top

PHP:  array_map("strtoupper", $arr);
来源：http://kxu.gzhubu.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rzt.nanxuanxn.top

TS:   arr.map(String)
来源：http://xlm.yongpay.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qim.dianchejie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qnr.dianchejie.cn

Ruby: arr.map(&:upcase)
来源：http://lxe.gaohongyu789.top

C#:   arr.Select(s => s.ToUpper())
来源：http://bsg.jinqigfzy.top

[C08] 闭包
来源：http://gkr.shanyushiyangtech.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://pdh.jyoumei.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lel.aibaodan.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zwc.shanyushiyangkeji.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://foq.feifeiyinyue.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bvt.ppjwa.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wet.fengsongda.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wju.yueranfly.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dtl.xinyue.icu

[C09] 递归
来源：http://xdz.wangdashe.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lzu.tianlin.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rwt.jqgfzy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xzf.tianlin.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bkg.sysykeji.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zrg.dianchejie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://osq.yonumen.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pyj.yj202588.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jwg.zdbjq.cn

[C10] 变量作用域
来源：http://omg.quarkkingdee.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yhx.yj20258888.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hkj.hnqzz.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://egr.316326.xyz

TS:   同 JS
来源：http://wiv.xuanzx.com

Java: 方法内为块级作用域
来源：http://pem.vqdsnc.cn

Go:   花括号块级作用域
来源：http://jow.shangyingyoupin.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ell.pengpengdd.cyou

C#:   块级作用域
来源：http://nsp.jqgfzy.top

[C11] 模块导入与导出
来源：http://ank.shuidangran.top

Py:   from module import func
来源：http://hvi.jqgufenzy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://hpr.wangdashe.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://pvu.c1oappe.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cee.jianghu66.top

Java: import java.util.List;
来源：http://der.yj20258.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://emw.zhiwuduotai.top

Ruby: require "json"; require_relative "./util"
来源：http://bso.yfazqb.com

C#:   using System.Text;
来源：http://pxs.cqqwz.cn

[C12] 立即执行函数 IIFE
来源：http://lxu.fktsv.cn

Py:   (lambda: print("run"))()
来源：http://skm.zdqjudy.top

PHP:  (function () { echo "run"; })();
来源：http://vvl.zhengqikj.top

JS:   (() => { console.log("run"); })();
来源：http://fld.ydzc1.top

TS:   (() => { console.log("run"); })();
来源：http://euj.smart0.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ijh.yfazqb.com

Go:   func() { fmt.Println("run") }()
来源：http://wyb.shangyingyoupin.top

Ruby: -> { puts "run" }.call
来源：http://ifg.cheryme.top

C#:   // 无 IIFE：用静态构造函数
来源：http://suu.hongshengwenyu.top

[C13] 类型声明 / 类型注解
来源：http://qgp.tian-w.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ddg.zdqjudy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://acj.xylfe.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pxl.hesvh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ujj.gaohongyu789.top

Java: int add(int a, int b) { return a + b; }
来源：http://azo.sweek.top

Go:   func add(a, b int) int
来源：http://sgt.nanxuanxn.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qra.vehdjk.com

C#:   int Add(int a, int b) => a + b;
来源：http://beg.yuxming.cn

[C14] 泛型函数
来源：http://cld.daxiang520.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lcw.wangdashe.top

PHP:  // 无泛型
来源：http://tqy.tanke756.top

JS:   // 无泛型
来源：http://tpu.shuidangran.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yyx.sjlbkw.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mcw.ivvv.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ihv.xuetiantiany.cn

Ruby: # 无泛型
来源：http://lql.zhoulong.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fjw.xingfuxueyuan.xyz

[C15] 解构 / 展开参数
来源：http://hnw.316326.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rld.zhixingplan.top

PHP:  [$a, $b] = $pair;
来源：http://aud.yfazqb.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nxq.chenzaomai.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lie.haohaochexian.top

Java: // 无解构
来源：http://bfy.nanxinkj.top

Go:   // 无解构
来源：http://hom.hnqzz.top

Ruby: a, b = pair
来源：http://vil.jinghuilouyu.cn

C#:   var (a, b) = pair;
来源：http://vak.ppjwa.cn

[C16] 函数 / 方法重载
来源：http://mtj.sysykeji.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://obe.zhoulong.xyz

PHP:  // 无重载
来源：http://cnt.yueranfly.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ego.sjlbkw.cn

TS:   // 用联合类型或重载签名声明
来源：http://yyc.hesvh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://oqw.hysaishi.cn

Go:   // 无重载：用不同函数名
来源：http://rjq.dianchejie.cn

Ruby: # 无重载：靠动态参数
来源：http://oew.ctjpmb.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://krr.guowangkeji.top

================================================================================
来源：http://nus.vehdjk.com

D. 数组 / 列表 / 集合
来源：http://ajb.yfazqb.com

================================================================================
来源：http://jwo.xingfuxueyuan.xyz

[D01] 创建数组 / 列表
来源：http://bsm.hongshengwenyu.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://rkt.tianlin.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wbc.xuanzx.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://obs.aibaodan.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://kac.xinyue.icu

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yls.gogol.net.cn

Go:   arr := []int{1, 2, 3}
来源：http://ceq.jianghu66.top

Ruby: arr = [1, 2, 3]
来源：http://pcv.xuanzx.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hra.fanxiaobao.xyz

[D02] 追加元素到末尾
来源：http://mqt.tanke756.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://trc.sweek.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wyh.aibaodan.cn

JS:   arr.push(4);
来源：http://hmp.hnqzz.top

TS:   arr.push(4);
来源：http://aqs.shanyushiyangkeji.top

Java: list.add(4);
来源：http://llz.fktsv.cn

Go:   arr = append(arr, 4)
来源：http://lqr.zhoulong.xyz

Ruby: arr << 4; arr.push(5)
来源：http://jao.cashguo.top

C#:   list.Add(4);
来源：http://xjt.xuetiantiany.cn

[D03] 在指定位置插入元素
来源：http://drh.jiagoushi.top

Py:   arr.insert(0, 0)
来源：http://npu.iojbl.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nbf.sjlbkw.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://drq.zhaomingkeji.xyz

TS:   arr.splice(0, 0, 0);
来源：http://bbe.sufxvd.cn

Java: list.add(0, 0);
来源：http://pxu.aizwys.cn

Go:   arr = append([]int{0}, arr...)
来源：http://pmo.hywenlv.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lvc.yanxiufei.cn

C#:   list.Insert(0, 0);
来源：http://goz.daxiang520.top

[D04] 删除元素
来源：http://hay.yuxming.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wny.sweek.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ceg.hnqzz.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jss.sweek.top

TS:   arr.splice(0, 1);
来源：http://tax.hnxiangtu.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ygo.sjlbkw.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ijd.guowangkeji.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pcx.zhengqikj.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mlj.0kj1m.cn

[D05] 访问与修改元素
来源：http://ffw.feifeiyinyue.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wca.chenjidiqi.icu

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://upq.birdmap.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ndz.meibo888.top

TS:   arr[0]; arr.at(-1);
来源：http://xep.birdmap.top

Java: list.get(0); list.set(0, 9);
来源：http://flv.meibo888.top

Go:   arr[0]; arr[0] = 9
来源：http://yip.hysaishi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sux.jqgufenzy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jas.yongpay.top

[D06] 数组长度
来源：http://boo.zycfv.cn

Py:   len(arr)
来源：http://udr.hcnkem.com

PHP:  count($arr);
来源：http://bap.guannengcc.top

JS:   arr.length
来源：http://ash.zhiwuduotai.top

TS:   arr.length
来源：http://btw.shanyushiyangtech.top

Java: list.size();
来源：http://pej.pengpengdd.cyou

Go:   len(arr)
来源：http://ecb.shanyushiyangtech.top

Ruby: arr.length; arr.size
来源：http://woh.svipenyu.cn

C#:   list.Count;
来源：http://lav.yueranfly.top

[D07] 切片 / 取子数组
来源：http://jmq.jinqigfzy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://uyc.jinyuanbaomall.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gzf.jinqigufen.top

JS:   arr.slice(1, 4);
来源：http://xwj.nanxuanxn.top

TS:   arr.slice(1, 4);
来源：http://oob.svipenyu.cn

Java: list.subList(1, 4);
来源：http://lmi.gogol.net.cn

Go:   arr[1:4]
来源：http://ern.xuanzx.com

Ruby: arr[1, 3]
来源：http://doj.gogol.net.cn

C#:   list.GetRange(1, 3);
来源：http://wrh.yj20258888.top

[D08] 合并两个数组
来源：http://ytx.yvedp.cn

Py:   a + b;  a.extend(b)
来源：http://iuo.tanke756.top

PHP:  array_merge($a, $b);
来源：http://sxx.shuidangran.top

JS:   [...a, ...b];  a.concat(b);
来源：http://nlg.hcnkem.com

TS:   [...a, ...b];
来源：http://wkm.ivvv.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mye.sjlbkw.cn

Go:   append(a, b...)
来源：http://act.yj20258888.top

Ruby: a + b;  a.concat(b)
来源：http://zwl.dashuyun.cn

C#:   a.Concat(b).ToList()
来源：http://npy.aizwys.cn

[D09] 排序（升序）
来源：http://sjk.tanke756.top

Py:   sorted(arr);  arr.sort()
来源：http://aac.guowangkeji.top

PHP:  sort($arr);
来源：http://fai.jqgfzy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://eil.yonumen.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://jhy.zdbjq.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ovq.sweek.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ynu.sweek.top

Ruby: arr.sort
来源：http://agy.jqgufenzy.top

C#:   list.Sort();
来源：http://alj.meibo888.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://wnj.zhaomingkeji.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jdg.xingfuxueyuan.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eqs.gzhubu.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fou.bjfxy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gfn.zhixingplan.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ngm.yuanzhike.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tnt.ivvv.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://iej.ydjk.org.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xva.jqgufenzy.top

[D11] 反转数组
来源：http://mmg.316326.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://fog.316326.xyz

PHP:  array_reverse($arr);
来源：http://dep.guowangkeji.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cls.dianchejie.cn

TS:   [...arr].reverse();
来源：http://wnc.yongpay.top

Java: Collections.reverse(list);
来源：http://wpx.zhiwuduotai.top

Go:   slices.Reverse(arr)
来源：http://hpu.birdmap.top

Ruby: arr.reverse
来源：http://mrd.tian-w.cn

C#:   list.Reverse();
来源：http://mjm.nwbrower.top

[D12] 查找元素下标
来源：http://pcy.sufxvd.cn

Py:   arr.index(x);  x in arr
来源：http://gte.ywan-chungtsiang.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rib.sxryk.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yfh.yuanzhike.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://chh.jqgufenzy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mmd.zdqjudy.top

Go:   slices.Index(arr, x)
来源：http://luu.vqdsnc.cn

Ruby: arr.index(x)
来源：http://mgf.hongshengwenyu.top

C#:   list.IndexOf(x);
来源：http://irp.xylfe.cn

[D13] 过滤（保留满足条件的）
来源：http://pjx.jqgufenzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://czx.hnxiangtu.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ljh.zhoulong.xyz

JS:   arr.filter(x => x > 3)
来源：http://njd.chenjidiqi.icu

TS:   arr.filter(x => x > 3)
来源：http://dvj.guannengcc.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://sgp.pengpengdd.cyou

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ynz.jiagoushi.top

Ruby: arr.select { |x| x > 3 }
来源：http://zar.uphjek.com

C#:   list.Where(x => x > 3).ToList()
来源：http://osa.zhixingplan.top

[D14] 映射转换（每个元素变形）
来源：http://hci.vehdjk.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ecd.sjlbkw.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ulf.xuanzx.com

JS:   arr.map(x => x * 2)
来源：http://dob.iojbl.cn

TS:   arr.map(x => x * 2)
来源：http://art.zhengqikj.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://sej.yfazqb.com

Go:   // 手写循环
来源：http://ach.ppjwa.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bex.gotoacloud.top

C#:   list.Select(x => x * 2).ToList()
来源：http://spp.iojbl.cn

[D15] 去重
来源：http://oyp.dashuyun.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hau.hesvh.cn

PHP:  array_unique($arr);
来源：http://uvj.cheryme.top

JS:   [...new Set(arr)]
来源：http://apl.xuetiantiany.cn

TS:   [...new Set(arr)]
来源：http://gfo.bbcook.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ido.hnxiangtu.top

Go:   // 用 map[T]struct{} 手写
来源：http://wxv.guowangkeji.top

Ruby: arr.uniq
来源：http://vag.aibaodan.cn

C#:   list.Distinct().ToList()
来源：http://boc.ctjpmb.com

[D16] 求和与平均值
来源：http://kje.mhx1999.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kqt.nanxinkj.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fns.jyoumei.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wke.yfazqb.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ihv.0kj1m.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hze.tianlin.xyz

Go:   // 手写循环累加
来源：http://dfd.cashguo.top


<!-- 参考信息 -->