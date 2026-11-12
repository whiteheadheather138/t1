代发 wailian999

Py:   if not data: return
来源：http://mta.pengpengdd.cyou

PHP:  if (!$data) { return; }
来源：http://ycf.pengpengdd.cyou

JS:   if (!data) return;
来源：http://ema.ctjpmb.com

TS:   if (!data) return;
来源：http://aev.fzhhl.top

Java: if (data == null) return;
来源：http://ldq.yangfankeji.com

Go:   if data == nil { return }
来源：http://tec.jiagoushi.top

Ruby: return if data.nil?
来源：http://sov.mhx1999.top

C#:   if (data == null) return;
来源：http://lmq.zhijiandao.cn

================================================================================
来源：http://rij.hfpthk.cn

C. 函数与作用域
来源：http://qvu.zdqjudy.top

================================================================================
来源：http://fkz.xuetiantiany.cn

[C01] 定义函数
来源：http://npi.yvedp.cn

Py:   def add(a, b): return a + b
来源：http://wvw.jinqigfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uvk.xinyue.icu

JS:   function add(a, b) { return a + b; }
来源：http://pbd.fktsv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oua.ydzc1.top

Java: static int add(int a, int b) { return a + b; }
来源：http://cor.shanyushiyangkeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://zub.yfazqb.com

Ruby: def add(a, b); a + b; end
来源：http://wcn.jinqigufen.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nka.cashguo.top

[C02] 默认参数
来源：http://vba.ctjpmb.com

Py:   def greet(name="World"): return name
来源：http://jnp.tian-w.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hki.jqgufenzy.top

JS:   function greet(name = "World") { return name; }
来源：http://haz.svipenyu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://mln.hesvh.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://xoz.shuidangran.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ajv.c1oappe.top

Ruby: def greet(name = "World") = name
来源：http://tvm.yanxiufei.cn

C#:   string Greet(string name = "World") => name;
来源：http://oii.wangdashe.top

[C03] 可变参数
来源：http://pdr.tarul.cn

Py:   def total(*args): return sum(args)
来源：http://lef.xinyue.icu

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bil.wangshuangyany.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ftp.yvedp.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fiq.hywenlv.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bzo.jyoumei.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cxz.ivvv.top

Ruby: def total(*nums); nums.sum; end
来源：http://fps.fengsongda.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vrt.0kj1m.cn

[C04] 命名参数 / 关键字参数
来源：http://tpm.52xcode.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kpn.zhijiandao.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wgj.yfazqb.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xrn.daria6918.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wow.jianghu66.top

Java: // 无：用 Builder 模式或 record
来源：http://ajp.daxiang520.top

Go:   // 无：用配置结构体参数
来源：http://mzh.xuanzx.com

Ruby: f(a: 1, b: 2)
来源：http://jpo.ppjwa.cn

C#:   f(a: 1, b: 2)
来源：http://qul.jinyuanbaomall.cn

[C05] 返回多个值
来源：http://pjb.zhoulong.xyz

Py:   return a, b
来源：http://ypp.uphjek.com

PHP:  return [$a, $b];
来源：http://fhw.yanxiufei.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ixh.wangshuangyany.cn

TS:   return { a, b };
来源：http://ddt.316326.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rrl.ywan-chungtsiang.top

Go:   return a, b
来源：http://hvi.hammf.cn

Ruby: return a, b
来源：http://fhr.c1oappe.top

C#:   return (a, b);              // ValueTuple
来源：http://oid.gogol.net.cn

[C06] 匿名函数 / lambda
来源：http://dbr.zdbjq.cn

Py:   square = lambda x: x * x
来源：http://ggn.jlsjyb.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://eho.gotoacloud.top

JS:   const square = x => x * x;
来源：http://vrx.gotoacloud.top

TS:   const square = (x: number): number => x * x;
来源：http://qlu.ctjpmb.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://svb.feifeiyinyue.top

Go:   sq := func(x int) int { return x * x }
来源：http://ead.zhixingplan.top

Ruby: square = ->(x) { x * x }
来源：http://hpq.jianghu66.top

C#:   Func<int, int> square = x => x * x;
来源：http://cpx.nanxuanxn.top

[C07] 把函数作为参数传入
来源：http://ahb.xingfuxueyuan.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dfp.0kj1m.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xir.chenjidiqi.icu

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://iej.shanyushiyangkeji.top

TS:   arr.map(String)
来源：http://pyo.yuanzhike.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ayw.yanxiufei.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mzw.chenzaomai.com

Ruby: arr.map(&:upcase)
来源：http://noc.xingfuxueyuan.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://soc.yvedp.cn

[C08] 闭包
来源：http://iww.vqdsnc.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://amv.c1oappe.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gmu.wangshuangyany.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ejh.ybcxt.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wad.jyoumei.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fws.hysaishi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qyp.0kj1m.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://oxy.cdnleiting.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ixk.zhixingplan.top

[C09] 递归
来源：http://tqf.shangyingyoupin.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lxm.shzxlz.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qet.xinyue.icu

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tyi.guannengcc.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mex.tarul.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vhc.316326.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qrk.yj202588.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zji.gaohongyu789.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://amv.jlsjyb.cn

[C10] 变量作用域
来源：http://uam.ydzc1.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vpk.hongshengwenyu.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kks.ehwqpu.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mpc.chenzaomai.com

TS:   同 JS
来源：http://ref.9152youxi.cn

Java: 方法内为块级作用域
来源：http://eqv.c1oappe.top

Go:   花括号块级作用域
来源：http://jtp.haohaochexian.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://prz.hywenlv.cn

C#:   块级作用域
来源：http://sxd.wangshuangyany.cn

[C11] 模块导入与导出
来源：http://xwm.yangfankeji.com

Py:   from module import func
来源：http://dpf.sufxvd.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://kyk.pengpengdd.cyou

JS:   export default function f() {};  import f from "./m.js";
来源：http://eyo.sweek.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gqe.yfazqb.com

Java: import java.util.List;
来源：http://eas.zhixingplan.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yzf.zdqjudy.top

Ruby: require "json"; require_relative "./util"
来源：http://ods.nanxuanxn.top

C#:   using System.Text;
来源：http://ioy.aibaodan.cn

[C12] 立即执行函数 IIFE
来源：http://aox.yangfankeji.com

Py:   (lambda: print("run"))()
来源：http://oaz.yj202588.top

PHP:  (function () { echo "run"; })();
来源：http://tdp.ydjk.org.cn

JS:   (() => { console.log("run"); })();
来源：http://brk.guannengcc.top

TS:   (() => { console.log("run"); })();
来源：http://vfa.sjlbkw.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kab.snrcjt.cn

Go:   func() { fmt.Println("run") }()
来源：http://pda.vehdjk.com

Ruby: -> { puts "run" }.call
来源：http://cez.zhaomingkeji.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://rqf.zycfv.cn

[C13] 类型声明 / 类型注解
来源：http://cvz.feifeiyinyue.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hfa.iojbl.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ltn.ydjk.org.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://awj.ctjpmb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xfh.ehwqpu.com

Java: int add(int a, int b) { return a + b; }
来源：http://haq.cucudq.cn

Go:   func add(a, b int) int
来源：http://dzn.cheryme.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ybm.sjlbkw.cn

C#:   int Add(int a, int b) => a + b;
来源：http://yth.shanyushiyangkeji.top

[C14] 泛型函数
来源：http://jcb.jinqigufen.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pex.yongpay.top

PHP:  // 无泛型
来源：http://tcu.sweek.top

JS:   // 无泛型
来源：http://tyq.nanxinkj.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qkp.zhaomingkeji.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nrg.wangdashe.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://njq.sufxvd.cn

Ruby: # 无泛型
来源：http://nsj.uphjek.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://iyw.zhiwuduotai.top

[C15] 解构 / 展开参数
来源：http://hwh.snrcjt.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kux.jinghuilouyu.cn

PHP:  [$a, $b] = $pair;
来源：http://fmi.sjlbkw.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://snr.andypj.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ycy.dianchejie.cn

Java: // 无解构
来源：http://bqz.yj20258888.top

Go:   // 无解构
来源：http://hwp.jinqigufen.top

Ruby: a, b = pair
来源：http://dwi.pengpengdd.cyou

C#:   var (a, b) = pair;
来源：http://gyy.jyoumei.cn

[C16] 函数 / 方法重载
来源：http://cdf.yj20258888.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zpj.shanyushiyangkeji.top

PHP:  // 无重载
来源：http://gaz.daxiang520.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://gqf.ydjk.org.cn

TS:   // 用联合类型或重载签名声明
来源：http://vcr.hammf.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://mkh.redwolf501.top

Go:   // 无重载：用不同函数名
来源：http://frf.shangyingyoupin.top

Ruby: # 无重载：靠动态参数
来源：http://xcl.pycfn.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://ctj.ybcxt.top

================================================================================
来源：http://iso.zdbjq.cn

D. 数组 / 列表 / 集合
来源：http://lya.guowangkeji.top

================================================================================
来源：http://xfy.tianlin.xyz

[D01] 创建数组 / 列表
来源：http://try.jiagoushi.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ndr.redwolf501.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jpt.aizwys.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fjt.shanyushiyangkeji.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://tto.zhixingplan.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qvj.ehwqpu.com

Go:   arr := []int{1, 2, 3}
来源：http://nwd.tanke756.top

Ruby: arr = [1, 2, 3]
来源：http://qkr.ywan-chungtsiang.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ewc.xingfuxueyuan.xyz

[D02] 追加元素到末尾
来源：http://hrk.xinyue.icu

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yeh.quarkkingdee.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lvq.tarul.cn

JS:   arr.push(4);
来源：http://qwi.yangfankeji.com

TS:   arr.push(4);
来源：http://qzu.daria6918.cn

Java: list.add(4);
来源：http://thv.pycfn.com

Go:   arr = append(arr, 4)
来源：http://joe.yuanzhike.top

Ruby: arr << 4; arr.push(5)
来源：http://jlm.zhaomingkeji.xyz

C#:   list.Add(4);
来源：http://nuc.jqgfzy.top

[D03] 在指定位置插入元素
来源：http://ylf.jinqigfzy.top

Py:   arr.insert(0, 0)
来源：http://rud.yueranfly.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://khp.dianchejie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gem.zdbjq.cn

TS:   arr.splice(0, 0, 0);
来源：http://hxy.yvedp.cn

Java: list.add(0, 0);
来源：http://mec.zhoulong.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://cqq.hnxiangtu.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hek.daxiang520.top

C#:   list.Insert(0, 0);
来源：http://syr.shzxlz.cn

[D04] 删除元素
来源：http://apm.yj202588.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://udg.quarkkingdee.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uld.aizwys.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yxy.guannengcc.top

TS:   arr.splice(0, 1);
来源：http://pok.ivvv.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xqi.redwolf501.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vtz.svipenyu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cgs.yvedp.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cvj.guowangkeji.top

[D05] 访问与修改元素
来源：http://enp.feifeiyinyue.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yws.zhijiandao.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vww.cqqwz.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://iid.wangshuangyany.cn

TS:   arr[0]; arr.at(-1);
来源：http://iip.ydzc1.top

Java: list.get(0); list.set(0, 9);
来源：http://lzb.chenlongwang.top

Go:   arr[0]; arr[0] = 9
来源：http://jcm.zhongyouzk.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pzm.c1oappe.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bmv.cucudq.cn

[D06] 数组长度
来源：http://ylh.tianlin.xyz

Py:   len(arr)
来源：http://lje.jianghu66.top

PHP:  count($arr);
来源：http://qth.yfazqb.com

JS:   arr.length
来源：http://pwl.bbcook.cn

TS:   arr.length
来源：http://rsn.fanxiaobao.xyz

Java: list.size();
来源：http://wvm.svipenyu.cn

Go:   len(arr)
来源：http://pob.yj202588.top

Ruby: arr.length; arr.size
来源：http://mtw.hesvh.cn

C#:   list.Count;
来源：http://wwh.yongpay.top

[D07] 切片 / 取子数组
来源：http://nfl.meibo888.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bkl.zhixingplan.top

PHP:  array_slice($arr, 1, 3);
来源：http://rsq.dashuyun.cn

JS:   arr.slice(1, 4);
来源：http://xtb.jlsjyb.cn

TS:   arr.slice(1, 4);
来源：http://lhe.tarul.cn

Java: list.subList(1, 4);
来源：http://nqs.jinyuanbaomall.cn

Go:   arr[1:4]
来源：http://oaa.vqdsnc.cn

Ruby: arr[1, 3]
来源：http://rci.hesvh.cn

C#:   list.GetRange(1, 3);
来源：http://lmh.sysykeji.top

[D08] 合并两个数组
来源：http://qre.andypj.xyz

Py:   a + b;  a.extend(b)
来源：http://dyw.tanke756.top

PHP:  array_merge($a, $b);
来源：http://tug.tianlin.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://yeq.shuidangran.top

TS:   [...a, ...b];
来源：http://jbe.ehwqpu.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bzc.shangyingyoupin.top

Go:   append(a, b...)
来源：http://mte.tianlin.xyz

Ruby: a + b;  a.concat(b)
来源：http://sae.hcnkem.com

C#:   a.Concat(b).ToList()
来源：http://irn.yonumen.top

[D09] 排序（升序）
来源：http://gjn.zhongyouzk.top

Py:   sorted(arr);  arr.sort()
来源：http://wfr.xziqi.cn

PHP:  sort($arr);
来源：http://tor.gotoacloud.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yvi.hfpthk.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://rsg.daria6918.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://wpj.yuxming.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ayh.gotoacloud.top

Ruby: arr.sort
来源：http://zlw.snrcjt.cn

C#:   list.Sort();
来源：http://ukj.andypj.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://ffh.quarkkingdee.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://udv.gogol.net.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fde.shzxlz.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hez.cashguo.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dmf.tarul.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ukt.snrcjt.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jxn.fengsongda.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://enn.xuanzx.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lok.aibaodan.cn

[D11] 反转数组
来源：http://tkt.xziqi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://tql.jinqigfzy.top

PHP:  array_reverse($arr);
来源：http://jem.ydjk.org.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sdr.chenjidiqi.icu

TS:   [...arr].reverse();
来源：http://dqt.316326.xyz

Java: Collections.reverse(list);
来源：http://bke.yvedp.cn

Go:   slices.Reverse(arr)
来源：http://nfv.jinqigufen.top

Ruby: arr.reverse
来源：http://lsa.tanke756.top

C#:   list.Reverse();
来源：http://fqn.iojbl.cn

[D12] 查找元素下标
来源：http://dbm.yuanzhike.top

Py:   arr.index(x);  x in arr
来源：http://npp.zhengqikj.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://otf.c1oappe.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dxm.jianghu66.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rqk.vehdjk.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ofa.hnqzz.top

Go:   slices.Index(arr, x)
来源：http://eko.zhengqikj.top

Ruby: arr.index(x)
来源：http://ree.ybcxt.top

C#:   list.IndexOf(x);
来源：http://qma.hnxiangtu.top

[D13] 过滤（保留满足条件的）
来源：http://hac.yj202588.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cep.guowangkeji.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://woj.9152youxi.cn

JS:   arr.filter(x => x > 3)
来源：http://kyp.zhiwuduotai.top

TS:   arr.filter(x => x > 3)
来源：http://uhn.zhoulong.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yrv.epnwcf.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bbf.uphjek.com

Ruby: arr.select { |x| x > 3 }
来源：http://pnq.hfpthk.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ubc.hysaishi.cn

[D14] 映射转换（每个元素变形）
来源：http://ymh.jinyuanbaomall.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zkb.zycfv.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://geq.zhaomingkeji.xyz

JS:   arr.map(x => x * 2)
来源：http://scq.hfpthk.cn

TS:   arr.map(x => x * 2)
来源：http://uls.havefunace.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ptq.yongpay.top

Go:   // 手写循环
来源：http://yid.yuxming.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dop.vqdsnc.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://baz.epnwcf.com

[D15] 去重
来源：http://ntl.jyoumei.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ryu.zhijiandao.cn

PHP:  array_unique($arr);
来源：http://lyg.yuxming.cn

JS:   [...new Set(arr)]
来源：http://imx.xuetiantiany.cn

TS:   [...new Set(arr)]
来源：http://neo.yongpay.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://own.zhoulong.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://omc.guowangkeji.top

Ruby: arr.uniq
来源：http://nkz.chenlongwang.top

C#:   list.Distinct().ToList()
来源：http://ojh.yangfankeji.com

[D16] 求和与平均值
来源：http://tvn.dashuyun.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://woy.52xcode.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jkq.aibaodan.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zva.meibo888.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://uer.hesvh.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hfg.wangshuangyany.cn

Go:   // 手写循环累加
来源：http://sgn.meibo888.top


<!-- 参考信息 -->