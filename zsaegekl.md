代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nso.daria6918.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dzf.yvedp.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bej.tianlin.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vcw.wangdashe.top

[B13] 判断是否为数字
来源：http://yob.sjlbkw.cn

Py:   isinstance(x, (int, float))
来源：http://dwc.jlsjyb.cn

PHP:  is_numeric($x)
来源：http://wtl.hesvh.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dwf.bjfxy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yji.shangyingyoupin.top

Java: x instanceof Number
来源：http://trf.ppjwa.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jhr.gogol.net.cn

Ruby: x.is_a?(Numeric)
来源：http://wzh.hywenlv.cn

C#:   x is int or double or decimal
来源：http://otq.shzxlz.cn

[B14] 判断值是否在集合内
来源：http://fls.ywan-chungtsiang.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pvs.52xcode.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jpm.zhixingplan.top

JS:   [1, 2, 3].includes(x)
来源：http://xko.chenzaomai.com

TS:   [1, 2, 3].includes(x)
来源：http://ika.ppjwa.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://whm.guowangkeji.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qcs.ctjpmb.com

Ruby: [1, 2, 3].include?(x)
来源：http://vul.jyoumei.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tfy.zhixingplan.top

[B15] 布尔运算与取反
来源：http://vla.redwolf501.top

Py:   a and b or not c
来源：http://nea.yangfankeji.com

PHP:  $a && $b || !$c
来源：http://rzj.yvedp.cn

JS:   a && b || !c
来源：http://wrd.dianchejie.cn

TS:   a && b || !c
来源：http://pzu.fengsongda.top

Java: a && b || !c
来源：http://ksz.pycfn.com

Go:   a && b || !c
来源：http://llp.ctjpmb.com

Ruby: a && b || !c
来源：http://daq.dianchejie.cn

C#:   a && b || !c
来源：http://oam.yj202588.top

[B16] 卫语句：不满足条件提前返回
来源：http://cas.0kj1m.cn

Py:   if not data: return
来源：http://jkw.yanxiufei.cn

PHP:  if (!$data) { return; }
来源：http://fhg.ivvv.top

JS:   if (!data) return;
来源：http://bvk.hnxiangtu.top

TS:   if (!data) return;
来源：http://kvv.hcnkem.com

Java: if (data == null) return;
来源：http://wnu.zhengqikj.top

Go:   if data == nil { return }
来源：http://wfj.pengpengdd.cyou

Ruby: return if data.nil?
来源：http://yax.zdqjudy.top

C#:   if (data == null) return;
来源：http://ifv.birdmap.top

================================================================================
来源：http://nqg.ppjwa.cn

C. 函数与作用域
来源：http://tup.sufxvd.cn

================================================================================
来源：http://xqw.vehdjk.com

[C01] 定义函数
来源：http://pza.epnwcf.com

Py:   def add(a, b): return a + b
来源：http://rns.nwbrower.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dzd.sufxvd.cn

JS:   function add(a, b) { return a + b; }
来源：http://fwz.pengpengdd.cyou

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hss.9152youxi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fbm.feifeiyinyue.top

Go:   func add(a, b int) int { return a + b }
来源：http://ckz.epnwcf.com

Ruby: def add(a, b); a + b; end
来源：http://xuo.xingfuxueyuan.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://uvu.ppjwa.cn

[C02] 默认参数
来源：http://dbo.ydzc1.top

Py:   def greet(name="World"): return name
来源：http://nzb.chenlongwang.top

PHP:  function greet($name = "World") { return $name; }
来源：http://bow.shuidangran.top

JS:   function greet(name = "World") { return name; }
来源：http://jls.52xcode.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ktu.hongshengwenyu.top

Java: // 无默认参数：方法重载或 Optional
来源：http://rbz.ehwqpu.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xyu.daria6918.cn

Ruby: def greet(name = "World") = name
来源：http://xxu.nanxinkj.top

C#:   string Greet(string name = "World") => name;
来源：http://gcd.xingfuxueyuan.xyz

[C03] 可变参数
来源：http://rco.jqgfzy.top

Py:   def total(*args): return sum(args)
来源：http://ywo.nwbrower.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jrs.shanyushiyangkeji.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hwc.birdmap.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://aaq.dashuyun.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hgq.wangdashe.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nfy.hfpthk.cn

Ruby: def total(*nums); nums.sum; end
来源：http://wrx.shanyushiyangkeji.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lfz.shanyushiyangtech.top

[C04] 命名参数 / 关键字参数
来源：http://aza.jiagoushi.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uma.jlsjyb.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wvj.zhaomingkeji.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://oim.pycfn.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ljy.sysykeji.top

Java: // 无：用 Builder 模式或 record
来源：http://cpz.ybcxt.top

Go:   // 无：用配置结构体参数
来源：http://wvl.haohaochexian.top

Ruby: f(a: 1, b: 2)
来源：http://mfk.svipenyu.cn

C#:   f(a: 1, b: 2)
来源：http://iwf.guannengcc.top

[C05] 返回多个值
来源：http://lbk.aizwys.cn

Py:   return a, b
来源：http://tis.sjlbkw.cn

PHP:  return [$a, $b];
来源：http://lgq.fanxiaobao.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://fnn.0kj1m.cn

TS:   return { a, b };
来源：http://bth.tarul.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hbw.ivvv.top

Go:   return a, b
来源：http://zml.epnwcf.com

Ruby: return a, b
来源：http://hik.zdbjq.cn

C#:   return (a, b);              // ValueTuple
来源：http://uwa.smart0.xyz

[C06] 匿名函数 / lambda
来源：http://mzv.dianchejie.cn

Py:   square = lambda x: x * x
来源：http://fdq.ivvv.top

PHP:  $square = fn($x) => $x * $x;
来源：http://blr.zhixingplan.top

JS:   const square = x => x * x;
来源：http://jkv.dianchejie.cn

TS:   const square = (x: number): number => x * x;
来源：http://pdu.jinqigfzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bdi.ppjwa.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hof.jinqigufen.top

Ruby: square = ->(x) { x * x }
来源：http://tgk.gotoacloud.top

C#:   Func<int, int> square = x => x * x;
来源：http://dqn.wangshuangyany.cn

[C07] 把函数作为参数传入
来源：http://wkr.svipenyu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fad.shzxlz.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xrz.xuetiantiany.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://crw.9152youxi.cn

TS:   arr.map(String)
来源：http://ody.hnqzz.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fer.yj20258.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vto.zhoulong.xyz

Ruby: arr.map(&:upcase)
来源：http://lku.jyoumei.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://gzp.shuidangran.top

[C08] 闭包
来源：http://wqm.cashguo.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qsp.cheryme.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uxe.hysaishi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yjp.guowangkeji.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fff.zhengqikj.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ebz.tianlin.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://abw.ydjk.org.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ebt.ehwqpu.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rbs.havefunace.top

[C09] 递归
来源：http://bwf.epnwcf.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://knt.ehwqpu.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jiu.sxryk.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gyp.jianghu66.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lze.nanxuanxn.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wmm.xingfuxueyuan.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kog.yj202588.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nso.kuanghao11.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bez.yj20258.top

[C10] 变量作用域
来源：http://xgr.tianlin.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hye.fktsv.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://shc.hammf.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://djv.dashuyun.cn

TS:   同 JS
来源：http://xjz.wangdashe.top

Java: 方法内为块级作用域
来源：http://ijp.epnwcf.com

Go:   花括号块级作用域
来源：http://ljr.jqgufenzy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://knw.smart0.xyz

C#:   块级作用域
来源：http://cec.zhaomingkeji.xyz

[C11] 模块导入与导出
来源：http://eyk.zhongyouzk.top

Py:   from module import func
来源：http://kwd.zycfv.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://nua.haohaochexian.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://yak.xingfuxueyuan.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lbr.kuanghao11.cn

Java: import java.util.List;
来源：http://ryg.zhixingplan.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zzw.redwolf501.top

Ruby: require "json"; require_relative "./util"
来源：http://lkd.hnxiangtu.top

C#:   using System.Text;
来源：http://rvd.epnwcf.com

[C12] 立即执行函数 IIFE
来源：http://tsb.tanke756.top

Py:   (lambda: print("run"))()
来源：http://cqf.kuanghao11.cn

PHP:  (function () { echo "run"; })();
来源：http://ubh.jianghu66.top

JS:   (() => { console.log("run"); })();
来源：http://qji.havefunace.top

TS:   (() => { console.log("run"); })();
来源：http://uxq.zhoulong.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bds.yfazqb.com

Go:   func() { fmt.Println("run") }()
来源：http://sgm.chenjidiqi.icu

Ruby: -> { puts "run" }.call
来源：http://nnz.yonumen.top

C#:   // 无 IIFE：用静态构造函数
来源：http://kba.jinqigfzy.top

[C13] 类型声明 / 类型注解
来源：http://uxi.zhijiandao.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bea.nanxinkj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gsx.zhengqikj.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xes.yueranfly.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xbu.ydjk.org.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ypf.xinyue.icu

Go:   func add(a, b int) int
来源：http://hfk.nanxuanxn.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fcf.shzxlz.cn

C#:   int Add(int a, int b) => a + b;
来源：http://nlq.zhaomingkeji.xyz

[C14] 泛型函数
来源：http://qiz.shuidangran.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zym.0kj1m.cn

PHP:  // 无泛型
来源：http://wkw.xylfe.cn

JS:   // 无泛型
来源：http://szl.andypj.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://sjj.sxryk.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cek.yanxiufei.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zjo.yuxming.cn

Ruby: # 无泛型
来源：http://yzj.smart0.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rcx.tarul.cn

[C15] 解构 / 展开参数
来源：http://tvo.nanxinkj.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nbs.hcnkem.com

PHP:  [$a, $b] = $pair;
来源：http://lbq.sjlbkw.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qqp.jiagoushi.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jlf.hfpthk.cn

Java: // 无解构
来源：http://pwo.zhoulong.xyz

Go:   // 无解构
来源：http://gzj.shuidangran.top

Ruby: a, b = pair
来源：http://fkc.zhixingplan.top

C#:   var (a, b) = pair;
来源：http://euo.jinghuilouyu.cn

[C16] 函数 / 方法重载
来源：http://seb.zhaomingkeji.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://irg.yuanzhike.top

PHP:  // 无重载
来源：http://hrx.zhengqikj.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://hnr.sufxvd.cn

TS:   // 用联合类型或重载签名声明
来源：http://tzb.xuetiantiany.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qzg.shangyingyoupin.top

Go:   // 无重载：用不同函数名
来源：http://wig.ehwqpu.com

Ruby: # 无重载：靠动态参数
来源：http://zhz.sufxvd.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ygf.dianchejie.cn

================================================================================
来源：http://prv.fanxiaobao.xyz

D. 数组 / 列表 / 集合
来源：http://mjo.ywan-chungtsiang.top

================================================================================
来源：http://ddc.ivvv.top

[D01] 创建数组 / 列表
来源：http://fwc.meibo888.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://uex.daria6918.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tqd.zhixingplan.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pdq.pycfn.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://lul.gotoacloud.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pnk.wangdashe.top

Go:   arr := []int{1, 2, 3}
来源：http://rxj.xuetiantiany.cn

Ruby: arr = [1, 2, 3]
来源：http://npt.yvedp.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vze.shanyushiyangkeji.top

[D02] 追加元素到末尾
来源：http://ipa.jinghuilouyu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fjy.cheryme.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://etr.bjfxy.top

JS:   arr.push(4);
来源：http://tbv.cdnleiting.top

TS:   arr.push(4);
来源：http://sqm.birdmap.top

Java: list.add(4);
来源：http://yuc.chenjidiqi.icu

Go:   arr = append(arr, 4)
来源：http://ydn.jinyuanbaomall.cn

Ruby: arr << 4; arr.push(5)
来源：http://stb.zhoulong.xyz

C#:   list.Add(4);
来源：http://rrd.fehbvm.com

[D03] 在指定位置插入元素
来源：http://jtn.jianghu66.top

Py:   arr.insert(0, 0)
来源：http://lvt.ehwqpu.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://biq.wangshuangyany.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fvx.wangdashe.top

TS:   arr.splice(0, 0, 0);
来源：http://uef.fehbvm.com

Java: list.add(0, 0);
来源：http://etc.ydjk.org.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ttd.jiagoushi.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://okf.fktsv.cn

C#:   list.Insert(0, 0);
来源：http://mtu.shuidangran.top

[D04] 删除元素
来源：http://cie.xylfe.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ssb.shanyushiyangkeji.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ttq.sxryk.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zsm.sufxvd.cn

TS:   arr.splice(0, 1);
来源：http://kle.xuetiantiany.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pzj.uphjek.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sha.yuanzhike.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xdb.nanxinkj.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lan.fktsv.cn

[D05] 访问与修改元素
来源：http://zbi.gzhubu.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dyj.zhiwuduotai.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://whp.sjlbkw.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qbg.shanyushiyangkeji.top

TS:   arr[0]; arr.at(-1);
来源：http://zzb.zhengqikj.top

Java: list.get(0); list.set(0, 9);
来源：http://xut.shangyingyoupin.top

Go:   arr[0]; arr[0] = 9
来源：http://zkp.yueranfly.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://duo.zhengqikj.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kdp.yanxiufei.cn

[D06] 数组长度
来源：http://vvh.birdmap.top

Py:   len(arr)
来源：http://iml.wangshuangyany.cn

PHP:  count($arr);
来源：http://ibr.cheryme.top

JS:   arr.length
来源：http://alj.hnqzz.top

TS:   arr.length
来源：http://spm.xingfuxueyuan.xyz

Java: list.size();
来源：http://xyu.9152youxi.cn

Go:   len(arr)
来源：http://lom.cashguo.top

Ruby: arr.length; arr.size
来源：http://paa.52xcode.cn

C#:   list.Count;
来源：http://cbm.nwbrower.top

[D07] 切片 / 取子数组
来源：http://vtd.xuetiantiany.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cir.redwolf501.top

PHP:  array_slice($arr, 1, 3);
来源：http://stg.tarul.cn

JS:   arr.slice(1, 4);
来源：http://fjb.yj20258.top

TS:   arr.slice(1, 4);
来源：http://qgx.ywan-chungtsiang.top

Java: list.subList(1, 4);
来源：http://jtb.chenjidiqi.icu

Go:   arr[1:4]
来源：http://xma.quarkkingdee.top

Ruby: arr[1, 3]
来源：http://ikj.yuxming.cn

C#:   list.GetRange(1, 3);
来源：http://rag.chenzaomai.com

[D08] 合并两个数组
来源：http://ydr.redwolf501.top

Py:   a + b;  a.extend(b)
来源：http://czz.yonumen.top

PHP:  array_merge($a, $b);
来源：http://gva.ybcxt.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ukh.zdbjq.cn

TS:   [...a, ...b];
来源：http://ors.uphjek.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ouv.aizwys.cn

Go:   append(a, b...)
来源：http://lgp.daxiang520.top

Ruby: a + b;  a.concat(b)
来源：http://nhq.daxiang520.top

C#:   a.Concat(b).ToList()
来源：http://ypy.jinyuanbaomall.cn

[D09] 排序（升序）
来源：http://nvp.vqdsnc.cn

Py:   sorted(arr);  arr.sort()
来源：http://pgc.cashguo.top

PHP:  sort($arr);
来源：http://stt.jqgfzy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sgn.zhongyouzk.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://gqh.dashuyun.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://htx.yongpay.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fwz.jinqigfzy.top

Ruby: arr.sort
来源：http://wcj.jqgufenzy.top

C#:   list.Sort();
来源：http://vlc.aizwys.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://gtn.ivvv.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qed.jianghu66.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qto.svipenyu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nbv.iojbl.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://uuf.jqgufenzy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rjp.shuidangran.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hmu.yfazqb.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bue.sxryk.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fud.sxryk.cn

[D11] 反转数组
来源：http://kxt.hysaishi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://kbu.tarul.cn

PHP:  array_reverse($arr);
来源：http://tqp.tian-w.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gtn.tarul.cn

TS:   [...arr].reverse();
来源：http://hin.zhiwuduotai.top

Java: Collections.reverse(list);
来源：http://mlu.yj20258.top

Go:   slices.Reverse(arr)
来源：http://yqz.sxryk.cn

Ruby: arr.reverse
来源：http://wpm.jqgfzy.top

C#:   list.Reverse();
来源：http://aib.gotoacloud.top

[D12] 查找元素下标
来源：http://hah.ppjwa.cn

Py:   arr.index(x);  x in arr
来源：http://xcp.zhaomingkeji.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bec.jinghuilouyu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bkt.jyoumei.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eyl.hammf.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gpm.c1oappe.top

Go:   slices.Index(arr, x)
来源：http://nzw.zdqjudy.top

Ruby: arr.index(x)
来源：http://qhf.nanxinkj.top

C#:   list.IndexOf(x);
来源：http://rau.316326.xyz

[D13] 过滤（保留满足条件的）
来源：http://gxh.ybcxt.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ypd.xuetiantiany.cn


<!-- 参考信息 -->