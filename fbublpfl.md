代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xlc.svipenyu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jkh.zhaomingkeji.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://eis.nanxinkj.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yed.cashguo.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uoq.mhx1999.top

[B10] 遍历同时拿索引
来源：http://ymy.zhengqikj.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://sos.haohaochexian.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kuz.dashuyun.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://khp.xinyue.icu

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://stf.zhaomingkeji.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ycq.jinqigufen.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wav.jqgfzy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fnl.nanxinkj.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wuf.ybcxt.top

[B11] 生成数字序列 / 区间
来源：http://oox.nanxuanxn.top

Py:   list(range(0, 10, 2))
来源：http://jkb.fktsv.cn

PHP:  range(0, 10, 2);
来源：http://bww.fzhhl.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mgf.dianchejie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://trp.sufxvd.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://eij.shangyingyoupin.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dgo.yongpay.top

Ruby: (0...10).step(2).to_a
来源：http://msy.shangyingyoupin.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://znc.sufxvd.cn

[B12] 跳出多层循环
来源：http://bor.yj20258.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://cpj.xziqi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ast.uphjek.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://skt.yj20258.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ygr.hesvh.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nmf.sweek.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ccb.yfazqb.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kdt.cashguo.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gnh.wangshuangyany.cn

[B13] 判断是否为数字
来源：http://tdn.hesvh.cn

Py:   isinstance(x, (int, float))
来源：http://wno.jyoumei.cn

PHP:  is_numeric($x)
来源：http://ytn.fktsv.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tca.hnqzz.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ckg.ctjpmb.com

Java: x instanceof Number
来源：http://cjs.hnqzz.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://eyf.jyoumei.cn

Ruby: x.is_a?(Numeric)
来源：http://dld.sweek.top

C#:   x is int or double or decimal
来源：http://ksk.ppjwa.cn

[B14] 判断值是否在集合内
来源：http://qcl.nanxinkj.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cfr.zhongyouzk.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tkh.yueranfly.top

JS:   [1, 2, 3].includes(x)
来源：http://gtc.sjlbkw.cn

TS:   [1, 2, 3].includes(x)
来源：http://nxg.bbcook.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://yvt.yj202588.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://csv.jinqigufen.top

Ruby: [1, 2, 3].include?(x)
来源：http://htn.jlsjyb.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ztx.ivvv.top

[B15] 布尔运算与取反
来源：http://lqe.ybcxt.top

Py:   a and b or not c
来源：http://npo.shanyushiyangkeji.top

PHP:  $a && $b || !$c
来源：http://qkm.iojbl.cn

JS:   a && b || !c
来源：http://ykf.yj20258888.top

TS:   a && b || !c
来源：http://xmc.snrcjt.cn

Java: a && b || !c
来源：http://ryq.dashuyun.cn

Go:   a && b || !c
来源：http://upd.vehdjk.com

Ruby: a && b || !c
来源：http://oyv.ydjk.org.cn

C#:   a && b || !c
来源：http://bfh.fzhhl.top

[B16] 卫语句：不满足条件提前返回
来源：http://fih.shanyushiyangkeji.top

Py:   if not data: return
来源：http://vua.aizwys.cn

PHP:  if (!$data) { return; }
来源：http://wrr.hesvh.cn

JS:   if (!data) return;
来源：http://dfk.aibaodan.cn

TS:   if (!data) return;
来源：http://ybr.yvedp.cn

Java: if (data == null) return;
来源：http://qhj.hnxiangtu.top

Go:   if data == nil { return }
来源：http://xxn.epnwcf.com

Ruby: return if data.nil?
来源：http://wot.gotoacloud.top

C#:   if (data == null) return;
来源：http://tvw.daria6918.cn

================================================================================
来源：http://rfu.yongpay.top

C. 函数与作用域
来源：http://mlp.snrcjt.cn

================================================================================
来源：http://ntm.tanke756.top

[C01] 定义函数
来源：http://ndv.hcnkem.com

Py:   def add(a, b): return a + b
来源：http://kih.yj20258.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yyu.meibo888.top

JS:   function add(a, b) { return a + b; }
来源：http://vcy.ywan-chungtsiang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zpv.aizwys.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://vez.birdmap.top

Go:   func add(a, b int) int { return a + b }
来源：http://zkm.hongshengwenyu.top

Ruby: def add(a, b); a + b; end
来源：http://xef.quarkkingdee.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://luo.nanxuanxn.top

[C02] 默认参数
来源：http://kce.tianlin.xyz

Py:   def greet(name="World"): return name
来源：http://bvk.redwolf501.top

PHP:  function greet($name = "World") { return $name; }
来源：http://jqi.redwolf501.top

JS:   function greet(name = "World") { return name; }
来源：http://uwx.havefunace.top

TS:   function greet(name: string = "World") { return name; }
来源：http://aju.9152youxi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://zgx.gzhubu.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kdn.gogol.net.cn

Ruby: def greet(name = "World") = name
来源：http://vch.jqgufenzy.top

C#:   string Greet(string name = "World") => name;
来源：http://cdb.yongpay.top

[C03] 可变参数
来源：http://wkh.xziqi.cn

Py:   def total(*args): return sum(args)
来源：http://qbl.wangshuangyany.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gei.52xcode.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ztv.shuidangran.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mwv.ydzc1.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hyu.gotoacloud.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wld.yuxming.cn

Ruby: def total(*nums); nums.sum; end
来源：http://cwa.guowangkeji.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dkf.tarul.cn

[C04] 命名参数 / 关键字参数
来源：http://osk.jinghuilouyu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tub.vehdjk.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bdy.bbcook.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tqw.havefunace.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mit.zycfv.cn

Java: // 无：用 Builder 模式或 record
来源：http://ydf.c1oappe.top

Go:   // 无：用配置结构体参数
来源：http://dkh.jinghuilouyu.cn

Ruby: f(a: 1, b: 2)
来源：http://ukx.cashguo.top

C#:   f(a: 1, b: 2)
来源：http://uil.quarkkingdee.top

[C05] 返回多个值
来源：http://mqt.andypj.xyz

Py:   return a, b
来源：http://voi.nanxinkj.top

PHP:  return [$a, $b];
来源：http://egf.nanxinkj.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://bhw.aibaodan.cn

TS:   return { a, b };
来源：http://mkz.andypj.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yve.yj20258888.top

Go:   return a, b
来源：http://vtc.tianlin.xyz

Ruby: return a, b
来源：http://sdh.zdqjudy.top

C#:   return (a, b);              // ValueTuple
来源：http://dni.yonumen.top

[C06] 匿名函数 / lambda
来源：http://jiv.hfpthk.cn

Py:   square = lambda x: x * x
来源：http://hxs.yongpay.top

PHP:  $square = fn($x) => $x * $x;
来源：http://uhw.shangyingyoupin.top

JS:   const square = x => x * x;
来源：http://fmo.hammf.cn

TS:   const square = (x: number): number => x * x;
来源：http://ibz.smart0.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zoz.fengsongda.top

Go:   sq := func(x int) int { return x * x }
来源：http://hvf.feifeiyinyue.top

Ruby: square = ->(x) { x * x }
来源：http://wrv.sysykeji.top

C#:   Func<int, int> square = x => x * x;
来源：http://ltn.gogol.net.cn

[C07] 把函数作为参数传入
来源：http://taz.aizwys.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ztc.hcnkem.com

PHP:  array_map("strtoupper", $arr);
来源：http://rjl.hywenlv.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qce.hysaishi.cn

TS:   arr.map(String)
来源：http://gfu.feifeiyinyue.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://uss.nwbrower.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rso.gzhubu.top

Ruby: arr.map(&:upcase)
来源：http://jzq.zhongyouzk.top

C#:   arr.Select(s => s.ToUpper())
来源：http://oqf.chenlongwang.top

[C08] 闭包
来源：http://aoz.hammf.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gpm.bjfxy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://spc.jqgufenzy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yvl.9152youxi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zkz.tanke756.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hye.shanyushiyangtech.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gft.0kj1m.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mmx.zhaomingkeji.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ltk.bbcook.cn

[C09] 递归
来源：http://sby.andypj.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mwr.sweek.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://itn.bjfxy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zfa.tanke756.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kqy.svipenyu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://olo.tarul.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wpv.tian-w.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ups.jqgfzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lzq.sufxvd.cn

[C10] 变量作用域
来源：http://zqt.daxiang520.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pez.zdbjq.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nrk.tianlin.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nzm.yueranfly.top

TS:   同 JS
来源：http://gaw.ctjpmb.com

Java: 方法内为块级作用域
来源：http://pyq.dianchejie.cn

Go:   花括号块级作用域
来源：http://zla.nanxuanxn.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fjq.yj20258.top

C#:   块级作用域
来源：http://ajt.cucudq.cn

[C11] 模块导入与导出
来源：http://coe.yj202588.top

Py:   from module import func
来源：http://vnb.smart0.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://mbj.yuxming.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://pid.ppjwa.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fye.yuxming.cn

Java: import java.util.List;
来源：http://cjq.zhengqikj.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jcx.shuidangran.top

Ruby: require "json"; require_relative "./util"
来源：http://tqk.fktsv.cn

C#:   using System.Text;
来源：http://vif.meibo888.top

[C12] 立即执行函数 IIFE
来源：http://zig.hnxiangtu.top

Py:   (lambda: print("run"))()
来源：http://tfy.dianchejie.cn

PHP:  (function () { echo "run"; })();
来源：http://niz.yfazqb.com

JS:   (() => { console.log("run"); })();
来源：http://tsb.yfazqb.com

TS:   (() => { console.log("run"); })();
来源：http://ttc.zhengqikj.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xaj.gotoacloud.top

Go:   func() { fmt.Println("run") }()
来源：http://elx.yvedp.cn

Ruby: -> { puts "run" }.call
来源：http://got.zdbjq.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://eye.yongpay.top

[C13] 类型声明 / 类型注解
来源：http://rhq.guowangkeji.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wsc.316326.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rlm.hnqzz.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://syd.c1oappe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yzq.jianghu66.top

Java: int add(int a, int b) { return a + b; }
来源：http://gwm.aibaodan.cn

Go:   func add(a, b int) int
来源：http://ibp.zhijiandao.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pll.sxryk.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fym.hfpthk.cn

[C14] 泛型函数
来源：http://bbl.quarkkingdee.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://aqk.havefunace.top

PHP:  // 无泛型
来源：http://iuw.smart0.xyz

JS:   // 无泛型
来源：http://zgn.zhongyouzk.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nao.jinqigufen.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dbe.yongpay.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xfb.nanxuanxn.top

Ruby: # 无泛型
来源：http://uuv.fktsv.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xqq.zhiwuduotai.top

[C15] 解构 / 展开参数
来源：http://qiv.yuxming.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nku.hongshengwenyu.top

PHP:  [$a, $b] = $pair;
来源：http://dyy.hfpthk.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://eis.tanke756.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pna.zycfv.cn

Java: // 无解构
来源：http://foy.jqgufenzy.top

Go:   // 无解构
来源：http://egy.shanyushiyangtech.top

Ruby: a, b = pair
来源：http://vvs.vqdsnc.cn

C#:   var (a, b) = pair;
来源：http://nmn.xziqi.cn

[C16] 函数 / 方法重载
来源：http://dxh.jianghu66.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nvb.feifeiyinyue.top

PHP:  // 无重载
来源：http://kuv.sufxvd.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://dcs.jinyuanbaomall.cn

TS:   // 用联合类型或重载签名声明
来源：http://wsw.quarkkingdee.top

Java: void f(int a) {}  void f(String a) {}
来源：http://xnx.birdmap.top

Go:   // 无重载：用不同函数名
来源：http://ibh.jinqigfzy.top

Ruby: # 无重载：靠动态参数
来源：http://rek.daria6918.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://vpy.cqqwz.cn

================================================================================
来源：http://vka.yueranfly.top

D. 数组 / 列表 / 集合
来源：http://ptl.yanxiufei.cn

================================================================================
来源：http://uos.chenjidiqi.icu

[D01] 创建数组 / 列表
来源：http://mkr.yongpay.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://kzl.dashuyun.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://beb.jinqigufen.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fwa.aizwys.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dyw.iojbl.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ang.shzxlz.cn

Go:   arr := []int{1, 2, 3}
来源：http://hpc.chenlongwang.top

Ruby: arr = [1, 2, 3]
来源：http://yog.hywenlv.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lbg.tian-w.cn

[D02] 追加元素到末尾
来源：http://pju.vehdjk.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pou.svipenyu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vbz.nanxuanxn.top

JS:   arr.push(4);
来源：http://alt.svipenyu.cn

TS:   arr.push(4);
来源：http://eah.yanxiufei.cn

Java: list.add(4);
来源：http://xxf.xziqi.cn

Go:   arr = append(arr, 4)
来源：http://jjk.yangfankeji.com

Ruby: arr << 4; arr.push(5)
来源：http://xtv.9152youxi.cn

C#:   list.Add(4);
来源：http://yqx.yonumen.top

[D03] 在指定位置插入元素
来源：http://ugh.zdbjq.cn

Py:   arr.insert(0, 0)
来源：http://dep.nwbrower.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://aum.ywan-chungtsiang.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yaj.dianchejie.cn

TS:   arr.splice(0, 0, 0);
来源：http://ufm.jiagoushi.top

Java: list.add(0, 0);
来源：http://iox.feifeiyinyue.top

Go:   arr = append([]int{0}, arr...)
来源：http://vbx.shangyingyoupin.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://iin.jiagoushi.top

C#:   list.Insert(0, 0);
来源：http://rtn.fzhhl.top

[D04] 删除元素
来源：http://kzf.ybcxt.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ivv.bjfxy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jer.cdnleiting.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fcm.shanyushiyangkeji.top

TS:   arr.splice(0, 1);
来源：http://ija.quarkkingdee.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rsi.bbcook.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lhw.ehwqpu.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lwg.jqgufenzy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mqa.xuanzx.com

[D05] 访问与修改元素
来源：http://gni.xylfe.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gpu.jqgufenzy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qwd.nwbrower.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://oas.chenjidiqi.icu

TS:   arr[0]; arr.at(-1);
来源：http://syi.fehbvm.com

Java: list.get(0); list.set(0, 9);
来源：http://szy.hysaishi.cn

Go:   arr[0]; arr[0] = 9
来源：http://evm.jqgufenzy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sxz.xylfe.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sbp.yonumen.top

[D06] 数组长度
来源：http://zmt.yueranfly.top

Py:   len(arr)
来源：http://ifp.birdmap.top

PHP:  count($arr);
来源：http://unz.yuanzhike.top

JS:   arr.length
来源：http://cgz.ywan-chungtsiang.top

TS:   arr.length
来源：http://wph.shuidangran.top

Java: list.size();
来源：http://cdr.yangfankeji.com

Go:   len(arr)
来源：http://nzm.fehbvm.com

Ruby: arr.length; arr.size
来源：http://jfc.yongpay.top

C#:   list.Count;
来源：http://ksm.tanke756.top

[D07] 切片 / 取子数组
来源：http://mhb.zdbjq.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pog.jlsjyb.cn

PHP:  array_slice($arr, 1, 3);
来源：http://lma.xylfe.cn

JS:   arr.slice(1, 4);
来源：http://ovw.shzxlz.cn

TS:   arr.slice(1, 4);
来源：http://lnn.316326.xyz

Java: list.subList(1, 4);
来源：http://kda.yueranfly.top

Go:   arr[1:4]
来源：http://xry.cdnleiting.top

Ruby: arr[1, 3]
来源：http://yoh.sysykeji.top

C#:   list.GetRange(1, 3);
来源：http://rvj.nanxinkj.top

[D08] 合并两个数组
来源：http://fra.zhoulong.xyz

Py:   a + b;  a.extend(b)
来源：http://wxo.quarkkingdee.top

PHP:  array_merge($a, $b);
来源：http://apq.bbcook.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://kgt.hnxiangtu.top

TS:   [...a, ...b];
来源：http://gxz.guannengcc.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sxn.c1oappe.top

Go:   append(a, b...)
来源：http://mue.jiagoushi.top

Ruby: a + b;  a.concat(b)
来源：http://qfm.fktsv.cn

C#:   a.Concat(b).ToList()
来源：http://wit.wangshuangyany.cn

[D09] 排序（升序）
来源：http://toj.ehwqpu.com

Py:   sorted(arr);  arr.sort()
来源：http://yae.jinqigufen.top

PHP:  sort($arr);
来源：http://gaz.yj20258.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pis.shanyushiyangtech.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://psb.chenlongwang.top

Java: Collections.sort(list);  list.sort(null);
来源：http://nkt.cdnleiting.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ccb.jqgfzy.top

Ruby: arr.sort
来源：http://haj.jqgfzy.top

C#:   list.Sort();
来源：http://kei.xylfe.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://cva.quarkkingdee.top


<!-- 参考信息 -->