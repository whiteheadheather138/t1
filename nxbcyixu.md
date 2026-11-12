代发 wailian999

Java: if (data == null) return;
来源：http://lyv.pengpengdd.cyou

Go:   if data == nil { return }
来源：http://pjj.epnwcf.com

Ruby: return if data.nil?
来源：http://klp.jinqigfzy.top

C#:   if (data == null) return;
来源：http://wue.redwolf501.top

================================================================================
来源：http://atz.tianlin.xyz

C. 函数与作用域
来源：http://gtv.hfpthk.cn

================================================================================
来源：http://mix.jqgufenzy.top

[C01] 定义函数
来源：http://uqd.zdqjudy.top

Py:   def add(a, b): return a + b
来源：http://xmj.wangdashe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lnb.9152youxi.cn

JS:   function add(a, b) { return a + b; }
来源：http://opz.tarul.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hxf.daxiang520.top

Java: static int add(int a, int b) { return a + b; }
来源：http://xmv.havefunace.top

Go:   func add(a, b int) int { return a + b }
来源：http://xlv.mhx1999.top

Ruby: def add(a, b); a + b; end
来源：http://qxj.dashuyun.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mkp.fehbvm.com

[C02] 默认参数
来源：http://bky.ivvv.top

Py:   def greet(name="World"): return name
来源：http://eae.yongpay.top

PHP:  function greet($name = "World") { return $name; }
来源：http://vex.aizwys.cn

JS:   function greet(name = "World") { return name; }
来源：http://yfh.zycfv.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fpl.jinqigufen.top

Java: // 无默认参数：方法重载或 Optional
来源：http://cbl.tanke756.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ral.hnqzz.top

Ruby: def greet(name = "World") = name
来源：http://maf.chenzaomai.com

C#:   string Greet(string name = "World") => name;
来源：http://bju.xziqi.cn

[C03] 可变参数
来源：http://tbb.zhijiandao.cn

Py:   def total(*args): return sum(args)
来源：http://wmp.tarul.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gxr.kuanghao11.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vhl.9152youxi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dxe.jinqigfzy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://oww.yj202588.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rrv.yvedp.cn

Ruby: def total(*nums); nums.sum; end
来源：http://eng.yonumen.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://odo.tarul.cn

[C04] 命名参数 / 关键字参数
来源：http://fjs.yfazqb.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ikm.jlsjyb.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nqh.yanxiufei.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wij.fanxiaobao.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dkn.hesvh.cn

Java: // 无：用 Builder 模式或 record
来源：http://aao.ydjk.org.cn

Go:   // 无：用配置结构体参数
来源：http://ete.chenzaomai.com

Ruby: f(a: 1, b: 2)
来源：http://yut.ybcxt.top

C#:   f(a: 1, b: 2)
来源：http://yrr.jlsjyb.cn

[C05] 返回多个值
来源：http://glz.zhaomingkeji.xyz

Py:   return a, b
来源：http://skb.gotoacloud.top

PHP:  return [$a, $b];
来源：http://uen.sjlbkw.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://cua.haohaochexian.top

TS:   return { a, b };
来源：http://unu.yj20258888.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vca.hcnkem.com

Go:   return a, b
来源：http://edm.uphjek.com

Ruby: return a, b
来源：http://yfc.vqdsnc.cn

C#:   return (a, b);              // ValueTuple
来源：http://guk.cucudq.cn

[C06] 匿名函数 / lambda
来源：http://kvg.yuanzhike.top

Py:   square = lambda x: x * x
来源：http://prf.chenlongwang.top

PHP:  $square = fn($x) => $x * $x;
来源：http://dua.epnwcf.com

JS:   const square = x => x * x;
来源：http://kjx.yuxming.cn

TS:   const square = (x: number): number => x * x;
来源：http://uso.redwolf501.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jqn.xingfuxueyuan.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://bht.nanxinkj.top

Ruby: square = ->(x) { x * x }
来源：http://akz.zhiwuduotai.top

C#:   Func<int, int> square = x => x * x;
来源：http://iil.birdmap.top

[C07] 把函数作为参数传入
来源：http://yqr.yanxiufei.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cnr.xingfuxueyuan.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://tpe.zhengqikj.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hiw.yangfankeji.com

TS:   arr.map(String)
来源：http://jnp.svipenyu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://flc.yongpay.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sra.shangyingyoupin.top

Ruby: arr.map(&:upcase)
来源：http://aum.chenjidiqi.icu

C#:   arr.Select(s => s.ToUpper())
来源：http://swl.shuidangran.top

[C08] 闭包
来源：http://rri.52xcode.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bpb.aizwys.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zve.sufxvd.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hxq.jinghuilouyu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bfp.ehwqpu.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ttj.fehbvm.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nqx.ywan-chungtsiang.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pga.fzhhl.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pvb.tianlin.xyz

[C09] 递归
来源：http://ijs.tian-w.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hxb.pengpengdd.cyou

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tkc.haohaochexian.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ulh.guannengcc.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hjp.cashguo.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hsi.shanyushiyangkeji.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mol.nanxuanxn.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://inv.yongpay.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qqi.316326.xyz

[C10] 变量作用域
来源：http://vmi.shanyushiyangtech.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://css.hysaishi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://did.gotoacloud.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bko.tarul.cn

TS:   同 JS
来源：http://iht.ydzc1.top

Java: 方法内为块级作用域
来源：http://vul.cqqwz.cn

Go:   花括号块级作用域
来源：http://quw.andypj.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qwm.sjlbkw.cn

C#:   块级作用域
来源：http://aol.ywan-chungtsiang.top

[C11] 模块导入与导出
来源：http://tei.hnxiangtu.top

Py:   from module import func
来源：http://iaa.chenlongwang.top

PHP:  require "file.php";  或 use App\Service;
来源：http://zox.xinyue.icu

JS:   export default function f() {};  import f from "./m.js";
来源：http://opg.hcnkem.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lfp.wangshuangyany.cn

Java: import java.util.List;
来源：http://uxa.zdbjq.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://atv.c1oappe.top

Ruby: require "json"; require_relative "./util"
来源：http://bmj.ivvv.top

C#:   using System.Text;
来源：http://ctx.hysaishi.cn

[C12] 立即执行函数 IIFE
来源：http://eyu.vqdsnc.cn

Py:   (lambda: print("run"))()
来源：http://avr.fanxiaobao.xyz

PHP:  (function () { echo "run"; })();
来源：http://iya.jqgufenzy.top

JS:   (() => { console.log("run"); })();
来源：http://vnx.wangshuangyany.cn

TS:   (() => { console.log("run"); })();
来源：http://lmd.ydjk.org.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fmi.tanke756.top

Go:   func() { fmt.Println("run") }()
来源：http://hmg.cqqwz.cn

Ruby: -> { puts "run" }.call
来源：http://hwq.jinyuanbaomall.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xdv.yonumen.top

[C13] 类型声明 / 类型注解
来源：http://sqf.cqqwz.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ydt.yuanzhike.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yzb.yueranfly.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jwy.yuxming.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lhg.zhijiandao.cn

Java: int add(int a, int b) { return a + b; }
来源：http://crl.316326.xyz

Go:   func add(a, b int) int
来源：http://cqf.fzhhl.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tgv.sysykeji.top

C#:   int Add(int a, int b) => a + b;
来源：http://eio.jinghuilouyu.cn

[C14] 泛型函数
来源：http://enn.zhoulong.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lya.jinqigufen.top

PHP:  // 无泛型
来源：http://ekw.zhijiandao.cn

JS:   // 无泛型
来源：http://msy.yonumen.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yad.ydjk.org.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sej.daxiang520.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ivi.wangdashe.top

Ruby: # 无泛型
来源：http://jcx.zdqjudy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lld.yuxming.cn

[C15] 解构 / 展开参数
来源：http://vim.havefunace.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sll.hfpthk.cn

PHP:  [$a, $b] = $pair;
来源：http://ryb.yj202588.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mqq.0kj1m.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rne.zhijiandao.cn

Java: // 无解构
来源：http://zmd.tanke756.top

Go:   // 无解构
来源：http://wqf.aizwys.cn

Ruby: a, b = pair
来源：http://ulb.xuanzx.com

C#:   var (a, b) = pair;
来源：http://xor.xziqi.cn

[C16] 函数 / 方法重载
来源：http://jad.kuanghao11.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kkh.shuidangran.top

PHP:  // 无重载
来源：http://ein.hcnkem.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://mfm.ppjwa.cn

TS:   // 用联合类型或重载签名声明
来源：http://qfa.fanxiaobao.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://vmz.pengpengdd.cyou

Go:   // 无重载：用不同函数名
来源：http://jmd.jinqigufen.top

Ruby: # 无重载：靠动态参数
来源：http://cyj.zdqjudy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://jbp.ctjpmb.com

================================================================================
来源：http://zoo.yangfankeji.com

D. 数组 / 列表 / 集合
来源：http://epz.xuanzx.com

================================================================================
来源：http://mja.0kj1m.cn

[D01] 创建数组 / 列表
来源：http://hhm.daxiang520.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://etr.9152youxi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ysc.sufxvd.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hxe.zhongyouzk.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://wbo.wangdashe.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://axd.xinyue.icu

Go:   arr := []int{1, 2, 3}
来源：http://mdn.zhixingplan.top

Ruby: arr = [1, 2, 3]
来源：http://yzl.52xcode.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qtk.haohaochexian.top

[D02] 追加元素到末尾
来源：http://jvx.gzhubu.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://szo.feifeiyinyue.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hrd.dashuyun.cn

JS:   arr.push(4);
来源：http://qoa.jinqigufen.top

TS:   arr.push(4);
来源：http://iye.hesvh.cn

Java: list.add(4);
来源：http://mlp.wangdashe.top

Go:   arr = append(arr, 4)
来源：http://fbo.hongshengwenyu.top

Ruby: arr << 4; arr.push(5)
来源：http://oye.zhoulong.xyz

C#:   list.Add(4);
来源：http://ibc.fehbvm.com

[D03] 在指定位置插入元素
来源：http://sin.cashguo.top

Py:   arr.insert(0, 0)
来源：http://jvy.52xcode.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vst.quarkkingdee.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mcm.ywan-chungtsiang.top

TS:   arr.splice(0, 0, 0);
来源：http://oyf.yj20258888.top

Java: list.add(0, 0);
来源：http://chh.sufxvd.cn

Go:   arr = append([]int{0}, arr...)
来源：http://chm.xziqi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dqf.fengsongda.top

C#:   list.Insert(0, 0);
来源：http://tua.zdqjudy.top

[D04] 删除元素
来源：http://ozu.sysykeji.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wmh.zhengqikj.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mlp.316326.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ifk.haohaochexian.top

TS:   arr.splice(0, 1);
来源：http://vnr.jinyuanbaomall.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://deu.jinqigufen.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://weo.fzhhl.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vri.gaohongyu789.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ihj.snrcjt.cn

[D05] 访问与修改元素
来源：http://cyu.shzxlz.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nya.pycfn.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://eic.dashuyun.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wlk.feifeiyinyue.top

TS:   arr[0]; arr.at(-1);
来源：http://xcd.yonumen.top

Java: list.get(0); list.set(0, 9);
来源：http://qrp.gotoacloud.top

Go:   arr[0]; arr[0] = 9
来源：http://arf.yuxming.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ynf.fktsv.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://avy.gogol.net.cn

[D06] 数组长度
来源：http://ann.shanyushiyangkeji.top

Py:   len(arr)
来源：http://nby.yj20258888.top

PHP:  count($arr);
来源：http://hdu.fktsv.cn

JS:   arr.length
来源：http://dll.jlsjyb.cn

TS:   arr.length
来源：http://cpb.ctjpmb.com

Java: list.size();
来源：http://lcr.cqqwz.cn

Go:   len(arr)
来源：http://uei.sufxvd.cn

Ruby: arr.length; arr.size
来源：http://ech.gotoacloud.top

C#:   list.Count;
来源：http://yuk.fanxiaobao.xyz

[D07] 切片 / 取子数组
来源：http://zgw.sweek.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://obd.bjfxy.top

PHP:  array_slice($arr, 1, 3);
来源：http://vav.xziqi.cn

JS:   arr.slice(1, 4);
来源：http://guj.hcnkem.com

TS:   arr.slice(1, 4);
来源：http://ity.shanyushiyangtech.top

Java: list.subList(1, 4);
来源：http://tgx.zhixingplan.top

Go:   arr[1:4]
来源：http://wql.daxiang520.top

Ruby: arr[1, 3]
来源：http://bys.tanke756.top

C#:   list.GetRange(1, 3);
来源：http://mqa.yuxming.cn

[D08] 合并两个数组
来源：http://iyq.cashguo.top

Py:   a + b;  a.extend(b)
来源：http://epp.52xcode.cn

PHP:  array_merge($a, $b);
来源：http://uuk.hongshengwenyu.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ymj.yongpay.top

TS:   [...a, ...b];
来源：http://vai.hysaishi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nmo.guowangkeji.top

Go:   append(a, b...)
来源：http://gvd.snrcjt.cn

Ruby: a + b;  a.concat(b)
来源：http://vub.zhongyouzk.top

C#:   a.Concat(b).ToList()
来源：http://rcp.yfazqb.com

[D09] 排序（升序）
来源：http://jzc.pengpengdd.cyou

Py:   sorted(arr);  arr.sort()
来源：http://fbn.316326.xyz

PHP:  sort($arr);
来源：http://jxo.zhongyouzk.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mxy.zhongyouzk.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://vav.dianchejie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://urz.xingfuxueyuan.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://eny.jinghuilouyu.cn

Ruby: arr.sort
来源：http://api.fktsv.cn

C#:   list.Sort();
来源：http://wcg.yfazqb.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://owz.shanyushiyangkeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://foz.zhiwuduotai.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qya.zhengqikj.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kwl.jinqigufen.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://iob.shangyingyoupin.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ufo.tarul.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vtp.jinyuanbaomall.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kpk.yanxiufei.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yim.ydjk.org.cn

[D11] 反转数组
来源：http://hbx.yuanzhike.top

Py:   arr[::-1];  arr.reverse()
来源：http://ssf.zhengqikj.top

PHP:  array_reverse($arr);
来源：http://wmd.redwolf501.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xek.aizwys.cn

TS:   [...arr].reverse();
来源：http://cpx.jyoumei.cn

Java: Collections.reverse(list);
来源：http://izi.jiagoushi.top

Go:   slices.Reverse(arr)
来源：http://xcy.c1oappe.top

Ruby: arr.reverse
来源：http://fqo.dashuyun.cn

C#:   list.Reverse();
来源：http://skb.zhijiandao.cn

[D12] 查找元素下标
来源：http://wdn.cqqwz.cn

Py:   arr.index(x);  x in arr
来源：http://jnx.chenzaomai.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zhd.shuidangran.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sgx.andypj.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fem.yj20258888.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yso.vehdjk.com

Go:   slices.Index(arr, x)
来源：http://gwm.feifeiyinyue.top

Ruby: arr.index(x)
来源：http://ixx.hywenlv.cn

C#:   list.IndexOf(x);
来源：http://yrk.hysaishi.cn

[D13] 过滤（保留满足条件的）
来源：http://hbv.jqgfzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ehf.xuanzx.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zzz.chenjidiqi.icu

JS:   arr.filter(x => x > 3)
来源：http://lhs.shanyushiyangtech.top

TS:   arr.filter(x => x > 3)
来源：http://ojo.aibaodan.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vwp.ywan-chungtsiang.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gyt.yj20258888.top

Ruby: arr.select { |x| x > 3 }
来源：http://ryq.cqqwz.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://lbx.wangdashe.top

[D14] 映射转换（每个元素变形）
来源：http://pfx.ydjk.org.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xdu.zycfv.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://moo.zycfv.cn

JS:   arr.map(x => x * 2)
来源：http://mlx.yuanzhike.top

TS:   arr.map(x => x * 2)
来源：http://xga.quarkkingdee.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ybk.smart0.xyz

Go:   // 手写循环
来源：http://xar.sweek.top

Ruby: arr.map { |x| x * 2 }
来源：http://dfo.chenjidiqi.icu

C#:   list.Select(x => x * 2).ToList()
来源：http://chq.wangshuangyany.cn

[D15] 去重
来源：http://oow.yj20258888.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mio.yj20258888.top

PHP:  array_unique($arr);
来源：http://vwe.yfazqb.com

JS:   [...new Set(arr)]
来源：http://hvf.chenlongwang.top

TS:   [...new Set(arr)]
来源：http://czp.shzxlz.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gnv.jqgufenzy.top

Go:   // 用 map[T]struct{} 手写
来源：http://trn.zhengqikj.top

Ruby: arr.uniq
来源：http://ioc.jinqigufen.top

C#:   list.Distinct().ToList()
来源：http://tkf.fktsv.cn

[D16] 求和与平均值
来源：http://bij.nanxuanxn.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xal.tanke756.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://aqt.sufxvd.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vmh.xziqi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ivw.52xcode.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fkj.xuanzx.com

Go:   // 手写循环累加
来源：http://qbw.ctjpmb.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bmg.fktsv.cn

C#:   list.Sum();  list.Average()
来源：http://sbu.xylfe.cn

[D17] 最大值与最小值
来源：http://hjo.meibo888.top

Py:   max(arr);  min(arr)
来源：http://mna.meibo888.top


<!-- 参考信息 -->