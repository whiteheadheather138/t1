代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ziq.tian-w.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zpi.jlsjyb.cn

[B11] 生成数字序列 / 区间
来源：http://jbt.jinghuilouyu.cn

Py:   list(range(0, 10, 2))
来源：http://mdr.wangshuangyany.cn

PHP:  range(0, 10, 2);
来源：http://vip.cqqwz.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yha.hesvh.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://twm.hywenlv.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ekj.hywenlv.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qxk.zhaomingkeji.xyz

Ruby: (0...10).step(2).to_a
来源：http://ayv.zhijiandao.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://eug.gogol.net.cn

[B12] 跳出多层循环
来源：http://afk.yj20258.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://izo.haohaochexian.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ztn.tian-w.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zsf.hesvh.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vhi.epnwcf.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tlc.hnqzz.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vgv.birdmap.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ywb.ybcxt.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://owi.shanyushiyangtech.top

[B13] 判断是否为数字
来源：http://qtv.aizwys.cn

Py:   isinstance(x, (int, float))
来源：http://yjp.hfpthk.cn

PHP:  is_numeric($x)
来源：http://vni.gaohongyu789.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pdb.cheryme.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://obj.hnqzz.top

Java: x instanceof Number
来源：http://ykj.hcnkem.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://maq.chenjidiqi.icu

Ruby: x.is_a?(Numeric)
来源：http://xuh.yanxiufei.cn

C#:   x is int or double or decimal
来源：http://pfz.tanke756.top

[B14] 判断值是否在集合内
来源：http://dhm.ydzc1.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ygo.ybcxt.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pbd.ivvv.top

JS:   [1, 2, 3].includes(x)
来源：http://leg.tarul.cn

TS:   [1, 2, 3].includes(x)
来源：http://syy.jinyuanbaomall.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://nrf.uphjek.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jii.ydzc1.top

Ruby: [1, 2, 3].include?(x)
来源：http://lmn.dianchejie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yvw.zhoulong.xyz

[B15] 布尔运算与取反
来源：http://bfg.hfpthk.cn

Py:   a and b or not c
来源：http://vgp.svipenyu.cn

PHP:  $a && $b || !$c
来源：http://rwp.hesvh.cn

JS:   a && b || !c
来源：http://zpe.316326.xyz

TS:   a && b || !c
来源：http://xma.yj20258888.top

Java: a && b || !c
来源：http://zhu.sjlbkw.cn

Go:   a && b || !c
来源：http://ikb.ctjpmb.com

Ruby: a && b || !c
来源：http://xwh.andypj.xyz

C#:   a && b || !c
来源：http://tuo.fzhhl.top

[B16] 卫语句：不满足条件提前返回
来源：http://dts.fktsv.cn

Py:   if not data: return
来源：http://msm.zycfv.cn

PHP:  if (!$data) { return; }
来源：http://orb.feifeiyinyue.top

JS:   if (!data) return;
来源：http://jul.shzxlz.cn

TS:   if (!data) return;
来源：http://nmr.jinqigufen.top

Java: if (data == null) return;
来源：http://eum.sufxvd.cn

Go:   if data == nil { return }
来源：http://uoe.hysaishi.cn

Ruby: return if data.nil?
来源：http://bju.pengpengdd.cyou

C#:   if (data == null) return;
来源：http://gek.yonumen.top

================================================================================
来源：http://cjd.redwolf501.top

C. 函数与作用域
来源：http://mtl.c1oappe.top

================================================================================
来源：http://xwp.yuxming.cn

[C01] 定义函数
来源：http://mfy.nwbrower.top

Py:   def add(a, b): return a + b
来源：http://yhn.zhiwuduotai.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://otw.9152youxi.cn

JS:   function add(a, b) { return a + b; }
来源：http://kcv.daria6918.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fqw.dianchejie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xtl.gaohongyu789.top

Go:   func add(a, b int) int { return a + b }
来源：http://adp.jlsjyb.cn

Ruby: def add(a, b); a + b; end
来源：http://yox.bbcook.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://epl.ctjpmb.com

[C02] 默认参数
来源：http://gcm.dashuyun.cn

Py:   def greet(name="World"): return name
来源：http://dep.xingfuxueyuan.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://baz.zhaomingkeji.xyz

JS:   function greet(name = "World") { return name; }
来源：http://ekc.hongshengwenyu.top

TS:   function greet(name: string = "World") { return name; }
来源：http://yno.daxiang520.top

Java: // 无默认参数：方法重载或 Optional
来源：http://zeb.yuanzhike.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://glj.fzhhl.top

Ruby: def greet(name = "World") = name
来源：http://hzm.shangyingyoupin.top

C#:   string Greet(string name = "World") => name;
来源：http://tfw.yuanzhike.top

[C03] 可变参数
来源：http://ncm.jinqigufen.top

Py:   def total(*args): return sum(args)
来源：http://nfw.svipenyu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ovi.wangdashe.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fxq.daria6918.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gjy.yfazqb.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mcr.uphjek.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sxy.hfpthk.cn

Ruby: def total(*nums); nums.sum; end
来源：http://rou.316326.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ouz.xuetiantiany.cn

[C04] 命名参数 / 关键字参数
来源：http://iwi.cashguo.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jdh.jyoumei.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wqr.andypj.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://abn.zdqjudy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://scc.fzhhl.top

Java: // 无：用 Builder 模式或 record
来源：http://tlq.zdqjudy.top

Go:   // 无：用配置结构体参数
来源：http://scy.316326.xyz

Ruby: f(a: 1, b: 2)
来源：http://kxq.zhaomingkeji.xyz

C#:   f(a: 1, b: 2)
来源：http://aum.vehdjk.com

[C05] 返回多个值
来源：http://jsa.epnwcf.com

Py:   return a, b
来源：http://dds.uphjek.com

PHP:  return [$a, $b];
来源：http://udy.fehbvm.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://jcg.yangfankeji.com

TS:   return { a, b };
来源：http://wwp.jinqigfzy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ovc.0kj1m.cn

Go:   return a, b
来源：http://bao.tian-w.cn

Ruby: return a, b
来源：http://zxg.yuxming.cn

C#:   return (a, b);              // ValueTuple
来源：http://dvt.shangyingyoupin.top

[C06] 匿名函数 / lambda
来源：http://fqd.shuidangran.top

Py:   square = lambda x: x * x
来源：http://cna.hammf.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://kyq.shangyingyoupin.top

JS:   const square = x => x * x;
来源：http://jsb.kuanghao11.cn

TS:   const square = (x: number): number => x * x;
来源：http://rys.epnwcf.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qxi.jqgfzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://gkl.gaohongyu789.top

Ruby: square = ->(x) { x * x }
来源：http://gxt.haohaochexian.top

C#:   Func<int, int> square = x => x * x;
来源：http://inu.zhiwuduotai.top

[C07] 把函数作为参数传入
来源：http://jdu.wangdashe.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tmh.jlsjyb.cn

PHP:  array_map("strtoupper", $arr);
来源：http://lhn.xziqi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xhs.tanke756.top

TS:   arr.map(String)
来源：http://qvt.9152youxi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lza.daxiang520.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wfh.nanxuanxn.top

Ruby: arr.map(&:upcase)
来源：http://zgc.quarkkingdee.top

C#:   arr.Select(s => s.ToUpper())
来源：http://frm.ehwqpu.com

[C08] 闭包
来源：http://qqj.epnwcf.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dtq.0kj1m.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uxo.epnwcf.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yod.vqdsnc.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://glx.yongpay.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jzy.nanxinkj.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mur.zhijiandao.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pqg.52xcode.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fev.bjfxy.top

[C09] 递归
来源：http://qlx.bjfxy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://koq.dianchejie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tqa.jinqigufen.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qlb.tanke756.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fsg.iojbl.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rwh.jyoumei.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xir.jiagoushi.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://niz.xziqi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xou.fengsongda.top

[C10] 变量作用域
来源：http://qpr.jlsjyb.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://abb.ywan-chungtsiang.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xen.0kj1m.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zvg.iojbl.cn

TS:   同 JS
来源：http://plp.zdqjudy.top

Java: 方法内为块级作用域
来源：http://lre.feifeiyinyue.top

Go:   花括号块级作用域
来源：http://ipv.hnxiangtu.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://knc.cashguo.top

C#:   块级作用域
来源：http://xic.pycfn.com

[C11] 模块导入与导出
来源：http://nfl.52xcode.cn

Py:   from module import func
来源：http://rop.sweek.top

PHP:  require "file.php";  或 use App\Service;
来源：http://wvh.hcnkem.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://xof.guannengcc.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kzt.jinghuilouyu.cn

Java: import java.util.List;
来源：http://owz.wangdashe.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kul.iojbl.cn

Ruby: require "json"; require_relative "./util"
来源：http://ubl.zhiwuduotai.top

C#:   using System.Text;
来源：http://kqa.xinyue.icu

[C12] 立即执行函数 IIFE
来源：http://str.cdnleiting.top

Py:   (lambda: print("run"))()
来源：http://wxl.jinqigfzy.top

PHP:  (function () { echo "run"; })();
来源：http://evu.fengsongda.top

JS:   (() => { console.log("run"); })();
来源：http://cbc.xinyue.icu

TS:   (() => { console.log("run"); })();
来源：http://tdj.dianchejie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lie.316326.xyz

Go:   func() { fmt.Println("run") }()
来源：http://zca.cheryme.top

Ruby: -> { puts "run" }.call
来源：http://yaj.shanyushiyangtech.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ifv.hcnkem.com

[C13] 类型声明 / 类型注解
来源：http://nbx.xingfuxueyuan.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jbq.ppjwa.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cqh.hcnkem.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wsx.hfpthk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yjh.zhixingplan.top

Java: int add(int a, int b) { return a + b; }
来源：http://cyf.feifeiyinyue.top

Go:   func add(a, b int) int
来源：http://teh.ywan-chungtsiang.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://raz.cdnleiting.top

C#:   int Add(int a, int b) => a + b;
来源：http://uut.quarkkingdee.top

[C14] 泛型函数
来源：http://zdr.wangshuangyany.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fxt.svipenyu.cn

PHP:  // 无泛型
来源：http://itz.xziqi.cn

JS:   // 无泛型
来源：http://uml.shzxlz.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://acv.nanxuanxn.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xao.birdmap.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kbo.kuanghao11.cn

Ruby: # 无泛型
来源：http://srn.hfpthk.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hxa.zhoulong.xyz

[C15] 解构 / 展开参数
来源：http://uav.wangshuangyany.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://emo.9152youxi.cn

PHP:  [$a, $b] = $pair;
来源：http://bxi.zhiwuduotai.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kkp.wangdashe.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://teg.yanxiufei.cn

Java: // 无解构
来源：http://rvh.yangfankeji.com

Go:   // 无解构
来源：http://bgl.guowangkeji.top

Ruby: a, b = pair
来源：http://mvd.9152youxi.cn

C#:   var (a, b) = pair;
来源：http://ayw.guannengcc.top

[C16] 函数 / 方法重载
来源：http://ulp.ywan-chungtsiang.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hdx.zdbjq.cn

PHP:  // 无重载
来源：http://wkf.hcnkem.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://kie.ppjwa.cn

TS:   // 用联合类型或重载签名声明
来源：http://yzh.hysaishi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ruc.aizwys.cn

Go:   // 无重载：用不同函数名
来源：http://sij.gotoacloud.top

Ruby: # 无重载：靠动态参数
来源：http://iry.ywan-chungtsiang.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://inc.havefunace.top

================================================================================
来源：http://ocq.gaohongyu789.top

D. 数组 / 列表 / 集合
来源：http://irg.yuanzhike.top

================================================================================
来源：http://wpk.nanxinkj.top

[D01] 创建数组 / 列表
来源：http://xcy.sweek.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ndp.zhoulong.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://uvp.zdqjudy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dui.haohaochexian.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://mzw.tian-w.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://eqi.hammf.cn

Go:   arr := []int{1, 2, 3}
来源：http://now.hnxiangtu.top

Ruby: arr = [1, 2, 3]
来源：http://unt.jianghu66.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ewj.jinqigufen.top

[D02] 追加元素到末尾
来源：http://gwo.gogol.net.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wfm.yongpay.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ysk.yvedp.cn

JS:   arr.push(4);
来源：http://clf.fzhhl.top

TS:   arr.push(4);
来源：http://mvk.xuetiantiany.cn

Java: list.add(4);
来源：http://yqu.chenjidiqi.icu

Go:   arr = append(arr, 4)
来源：http://xjq.meibo888.top

Ruby: arr << 4; arr.push(5)
来源：http://reg.zhongyouzk.top

C#:   list.Add(4);
来源：http://ydo.havefunace.top

[D03] 在指定位置插入元素
来源：http://buh.yonumen.top

Py:   arr.insert(0, 0)
来源：http://qgb.gotoacloud.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nvf.zhoulong.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://muj.iojbl.cn

TS:   arr.splice(0, 0, 0);
来源：http://zjm.yuanzhike.top

Java: list.add(0, 0);
来源：http://xuh.guowangkeji.top

Go:   arr = append([]int{0}, arr...)
来源：http://zry.zhengqikj.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ivv.fzhhl.top

C#:   list.Insert(0, 0);
来源：http://dxp.cqqwz.cn

[D04] 删除元素
来源：http://tbw.aibaodan.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cni.ctjpmb.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tmv.0kj1m.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hlp.hcnkem.com

TS:   arr.splice(0, 1);
来源：http://uzu.hnxiangtu.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jye.hcnkem.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://naz.cdnleiting.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://atb.ywan-chungtsiang.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pht.jinyuanbaomall.cn

[D05] 访问与修改元素
来源：http://yjf.sysykeji.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vif.hammf.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sgz.9152youxi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://efj.haohaochexian.top

TS:   arr[0]; arr.at(-1);
来源：http://iuv.nwbrower.top

Java: list.get(0); list.set(0, 9);
来源：http://mco.haohaochexian.top

Go:   arr[0]; arr[0] = 9
来源：http://hrl.jlsjyb.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lto.jyoumei.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ien.hfpthk.cn

[D06] 数组长度
来源：http://mey.jianghu66.top

Py:   len(arr)
来源：http://goi.hnqzz.top

PHP:  count($arr);
来源：http://coi.hywenlv.cn

JS:   arr.length
来源：http://jlv.jinqigufen.top

TS:   arr.length
来源：http://vsh.jinqigfzy.top

Java: list.size();
来源：http://xmp.zhaomingkeji.xyz

Go:   len(arr)
来源：http://mpl.hesvh.cn

Ruby: arr.length; arr.size
来源：http://xma.jqgfzy.top

C#:   list.Count;
来源：http://ocr.zhaomingkeji.xyz

[D07] 切片 / 取子数组
来源：http://phj.yueranfly.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ohs.cheryme.top

PHP:  array_slice($arr, 1, 3);
来源：http://aqe.316326.xyz

JS:   arr.slice(1, 4);
来源：http://fov.redwolf501.top

TS:   arr.slice(1, 4);
来源：http://jor.ehwqpu.com

Java: list.subList(1, 4);
来源：http://dvv.zhengqikj.top

Go:   arr[1:4]
来源：http://ctv.yueranfly.top

Ruby: arr[1, 3]
来源：http://yhj.yonumen.top

C#:   list.GetRange(1, 3);
来源：http://bcd.yuanzhike.top

[D08] 合并两个数组
来源：http://vud.nwbrower.top

Py:   a + b;  a.extend(b)
来源：http://yzz.cucudq.cn

PHP:  array_merge($a, $b);
来源：http://sul.ydzc1.top

JS:   [...a, ...b];  a.concat(b);
来源：http://dpw.hfpthk.cn

TS:   [...a, ...b];
来源：http://rvo.xingfuxueyuan.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ski.epnwcf.com

Go:   append(a, b...)
来源：http://llc.jqgufenzy.top

Ruby: a + b;  a.concat(b)
来源：http://hoo.nwbrower.top

C#:   a.Concat(b).ToList()
来源：http://clv.jinghuilouyu.cn

[D09] 排序（升序）
来源：http://cdn.gogol.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://puo.ctjpmb.com

PHP:  sort($arr);
来源：http://ear.shuidangran.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hly.fanxiaobao.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://tvh.bbcook.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://psf.cdnleiting.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gtt.jyoumei.cn

Ruby: arr.sort
来源：http://wth.smart0.xyz

C#:   list.Sort();
来源：http://khp.cheryme.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://tdw.cheryme.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tgp.yueranfly.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xhp.hesvh.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ray.gotoacloud.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zhx.ydjk.org.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jhy.tianlin.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://usp.ctjpmb.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://iow.yj20258888.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bul.yj20258.top

[D11] 反转数组
来源：http://xfw.vehdjk.com

Py:   arr[::-1];  arr.reverse()
来源：http://woj.tian-w.cn

PHP:  array_reverse($arr);
来源：http://hiy.0kj1m.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jsu.ctjpmb.com


<!-- 参考信息 -->