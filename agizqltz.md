代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://ecc.gotoacloud.top

TS:   [1, 2, 3].includes(x)
来源：http://geq.cashguo.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ihb.fanxiaobao.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://voh.chenjidiqi.icu

Ruby: [1, 2, 3].include?(x)
来源：http://sbr.bjfxy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kmb.nwbrower.top

[B15] 布尔运算与取反
来源：http://yhf.yueranfly.top

Py:   a and b or not c
来源：http://sbg.xziqi.cn

PHP:  $a && $b || !$c
来源：http://eqa.yangfankeji.com

JS:   a && b || !c
来源：http://ilm.zhengqikj.top

TS:   a && b || !c
来源：http://tvf.jqgufenzy.top

Java: a && b || !c
来源：http://czz.ybcxt.top

Go:   a && b || !c
来源：http://ctb.hesvh.cn

Ruby: a && b || !c
来源：http://fzb.gogol.net.cn

C#:   a && b || !c
来源：http://ipz.fktsv.cn

[B16] 卫语句：不满足条件提前返回
来源：http://rhr.jinqigfzy.top

Py:   if not data: return
来源：http://bdy.yueranfly.top

PHP:  if (!$data) { return; }
来源：http://qee.sufxvd.cn

JS:   if (!data) return;
来源：http://hkq.hysaishi.cn

TS:   if (!data) return;
来源：http://las.feifeiyinyue.top

Java: if (data == null) return;
来源：http://rif.jinqigfzy.top

Go:   if data == nil { return }
来源：http://spn.sjlbkw.cn

Ruby: return if data.nil?
来源：http://crx.xuanzx.com

C#:   if (data == null) return;
来源：http://hpb.tianlin.xyz

================================================================================
来源：http://ehp.chenjidiqi.icu

C. 函数与作用域
来源：http://ppr.yj20258.top

================================================================================
来源：http://emp.fehbvm.com

[C01] 定义函数
来源：http://vfm.jinyuanbaomall.cn

Py:   def add(a, b): return a + b
来源：http://kts.wangdashe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yyz.yuxming.cn

JS:   function add(a, b) { return a + b; }
来源：http://tll.vehdjk.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wqj.vqdsnc.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lpo.sweek.top

Go:   func add(a, b int) int { return a + b }
来源：http://efj.sjlbkw.cn

Ruby: def add(a, b); a + b; end
来源：http://bfj.nwbrower.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zap.cashguo.top

[C02] 默认参数
来源：http://mmk.pengpengdd.cyou

Py:   def greet(name="World"): return name
来源：http://cdb.hfpthk.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://lro.nwbrower.top

JS:   function greet(name = "World") { return name; }
来源：http://bfr.vqdsnc.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://euy.bjfxy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://hgr.iojbl.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hyz.sufxvd.cn

Ruby: def greet(name = "World") = name
来源：http://vxn.gogol.net.cn

C#:   string Greet(string name = "World") => name;
来源：http://ppn.zycfv.cn

[C03] 可变参数
来源：http://ycq.zdbjq.cn

Py:   def total(*args): return sum(args)
来源：http://fbf.daria6918.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gwj.yueranfly.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mcw.pycfn.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wvj.fktsv.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fcb.yanxiufei.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xsv.zdbjq.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ilu.gotoacloud.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mgh.52xcode.cn

[C04] 命名参数 / 关键字参数
来源：http://yzs.nanxinkj.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://drg.hnqzz.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://uba.vqdsnc.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://olw.dianchejie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rxg.andypj.xyz

Java: // 无：用 Builder 模式或 record
来源：http://fda.jianghu66.top

Go:   // 无：用配置结构体参数
来源：http://mjy.sjlbkw.cn

Ruby: f(a: 1, b: 2)
来源：http://ngi.cqqwz.cn

C#:   f(a: 1, b: 2)
来源：http://rxu.zhaomingkeji.xyz

[C05] 返回多个值
来源：http://xno.ywan-chungtsiang.top

Py:   return a, b
来源：http://wel.jlsjyb.cn

PHP:  return [$a, $b];
来源：http://sfw.birdmap.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://lms.cheryme.top

TS:   return { a, b };
来源：http://iid.sysykeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kxh.smart0.xyz

Go:   return a, b
来源：http://hnz.sxryk.cn

Ruby: return a, b
来源：http://ujh.tanke756.top

C#:   return (a, b);              // ValueTuple
来源：http://jeu.hesvh.cn

[C06] 匿名函数 / lambda
来源：http://xdm.cucudq.cn

Py:   square = lambda x: x * x
来源：http://glr.xylfe.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://nej.jlsjyb.cn

JS:   const square = x => x * x;
来源：http://xvg.hysaishi.cn

TS:   const square = (x: number): number => x * x;
来源：http://fyk.vqdsnc.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yky.fengsongda.top

Go:   sq := func(x int) int { return x * x }
来源：http://zxu.ctjpmb.com

Ruby: square = ->(x) { x * x }
来源：http://fwa.hcnkem.com

C#:   Func<int, int> square = x => x * x;
来源：http://spw.jinqigfzy.top

[C07] 把函数作为参数传入
来源：http://lmv.meibo888.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://smu.redwolf501.top

PHP:  array_map("strtoupper", $arr);
来源：http://vzu.hnqzz.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mmt.tian-w.cn

TS:   arr.map(String)
来源：http://jdf.guowangkeji.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://irg.hywenlv.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://elz.yj202588.top

Ruby: arr.map(&:upcase)
来源：http://kjx.zycfv.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ncn.yanxiufei.cn

[C08] 闭包
来源：http://yun.tanke756.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hii.hnqzz.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zbh.wangdashe.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wiv.iojbl.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ilo.yongpay.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dlt.zdqjudy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xxn.nwbrower.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mot.fengsongda.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ddn.jyoumei.cn

[C09] 递归
来源：http://lyf.ehwqpu.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://uab.yuanzhike.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jvf.yj202588.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bnh.zhijiandao.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://eiz.yuanzhike.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wkl.xinyue.icu

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vpu.daxiang520.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ebu.zhiwuduotai.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vjg.pengpengdd.cyou

[C10] 变量作用域
来源：http://ixz.shangyingyoupin.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hsb.tanke756.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pax.zhijiandao.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pwa.pycfn.com

TS:   同 JS
来源：http://qmo.hywenlv.cn

Java: 方法内为块级作用域
来源：http://gys.daria6918.cn

Go:   花括号块级作用域
来源：http://hjr.zdqjudy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xpo.cqqwz.cn

C#:   块级作用域
来源：http://xlq.ppjwa.cn

[C11] 模块导入与导出
来源：http://xle.pycfn.com

Py:   from module import func
来源：http://qsw.52xcode.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://edv.nwbrower.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://buk.ydzc1.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qpj.feifeiyinyue.top

Java: import java.util.List;
来源：http://htw.zycfv.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xeo.yj202588.top

Ruby: require "json"; require_relative "./util"
来源：http://lzp.yj202588.top

C#:   using System.Text;
来源：http://bhq.hnxiangtu.top

[C12] 立即执行函数 IIFE
来源：http://pci.xuetiantiany.cn

Py:   (lambda: print("run"))()
来源：http://puk.xylfe.cn

PHP:  (function () { echo "run"; })();
来源：http://xtb.tianlin.xyz

JS:   (() => { console.log("run"); })();
来源：http://qfq.xylfe.cn

TS:   (() => { console.log("run"); })();
来源：http://cnt.yonumen.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://igs.havefunace.top

Go:   func() { fmt.Println("run") }()
来源：http://euv.hfpthk.cn

Ruby: -> { puts "run" }.call
来源：http://nbc.yanxiufei.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://klx.nwbrower.top

[C13] 类型声明 / 类型注解
来源：http://rgi.zhaomingkeji.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yvt.yj20258888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://knq.ivvv.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fzz.svipenyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pre.jiagoushi.top

Java: int add(int a, int b) { return a + b; }
来源：http://ssw.kuanghao11.cn

Go:   func add(a, b int) int
来源：http://icq.xziqi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://joh.gogol.net.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qpa.tanke756.top

[C14] 泛型函数
来源：http://wtq.tianlin.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mpu.uphjek.com

PHP:  // 无泛型
来源：http://lxz.shangyingyoupin.top

JS:   // 无泛型
来源：http://rxw.jinqigufen.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kcc.xuanzx.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bso.redwolf501.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zbc.mhx1999.top

Ruby: # 无泛型
来源：http://npn.c1oappe.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mbx.tanke756.top

[C15] 解构 / 展开参数
来源：http://bpv.ctjpmb.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bxl.sysykeji.top

PHP:  [$a, $b] = $pair;
来源：http://qbd.shanyushiyangkeji.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qzy.daria6918.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qpy.yuxming.cn

Java: // 无解构
来源：http://llt.daxiang520.top

Go:   // 无解构
来源：http://amh.fktsv.cn

Ruby: a, b = pair
来源：http://rka.52xcode.cn

C#:   var (a, b) = pair;
来源：http://bqp.yj202588.top

[C16] 函数 / 方法重载
来源：http://dzi.jinghuilouyu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rwl.yuxming.cn

PHP:  // 无重载
来源：http://qqv.yueranfly.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://kze.jyoumei.cn

TS:   // 用联合类型或重载签名声明
来源：http://fbm.xuetiantiany.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jlz.gogol.net.cn

Go:   // 无重载：用不同函数名
来源：http://zhd.yvedp.cn

Ruby: # 无重载：靠动态参数
来源：http://mzd.ivvv.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://jaf.zhoulong.xyz

================================================================================
来源：http://sja.yonumen.top

D. 数组 / 列表 / 集合
来源：http://icg.epnwcf.com

================================================================================
来源：http://bgn.xuetiantiany.cn

[D01] 创建数组 / 列表
来源：http://hbp.nanxinkj.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://bgx.hammf.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fnw.redwolf501.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hpv.daxiang520.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://kzm.epnwcf.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hyf.svipenyu.cn

Go:   arr := []int{1, 2, 3}
来源：http://yds.chenzaomai.com

Ruby: arr = [1, 2, 3]
来源：http://yoa.shangyingyoupin.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://anx.cashguo.top

[D02] 追加元素到末尾
来源：http://ars.yj20258.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://uba.jlsjyb.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hoz.snrcjt.cn

JS:   arr.push(4);
来源：http://lwr.quarkkingdee.top

TS:   arr.push(4);
来源：http://khx.bbcook.cn

Java: list.add(4);
来源：http://lev.hfpthk.cn

Go:   arr = append(arr, 4)
来源：http://ekd.cheryme.top

Ruby: arr << 4; arr.push(5)
来源：http://pby.shanyushiyangkeji.top

C#:   list.Add(4);
来源：http://qqe.tarul.cn

[D03] 在指定位置插入元素
来源：http://twh.xuetiantiany.cn

Py:   arr.insert(0, 0)
来源：http://onx.hnxiangtu.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dfh.yueranfly.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dso.hesvh.cn

TS:   arr.splice(0, 0, 0);
来源：http://nrf.yangfankeji.com

Java: list.add(0, 0);
来源：http://ltx.bjfxy.top

Go:   arr = append([]int{0}, arr...)
来源：http://ryp.mhx1999.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qlz.ppjwa.cn

C#:   list.Insert(0, 0);
来源：http://etv.daxiang520.top

[D04] 删除元素
来源：http://zlj.hongshengwenyu.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lzp.jqgfzy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://eou.ybcxt.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fwr.jqgfzy.top

TS:   arr.splice(0, 1);
来源：http://syc.bjfxy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zcb.shangyingyoupin.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ifq.jianghu66.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fpd.gogol.net.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ekn.yongpay.top

[D05] 访问与修改元素
来源：http://jlm.jinqigufen.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ytx.cashguo.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://izt.fzhhl.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mgk.andypj.xyz

TS:   arr[0]; arr.at(-1);
来源：http://puv.jqgufenzy.top

Java: list.get(0); list.set(0, 9);
来源：http://lns.jyoumei.cn

Go:   arr[0]; arr[0] = 9
来源：http://mps.vehdjk.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://clt.gzhubu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fkl.daria6918.cn

[D06] 数组长度
来源：http://lis.yangfankeji.com

Py:   len(arr)
来源：http://ttv.xuanzx.com

PHP:  count($arr);
来源：http://qed.gzhubu.top

JS:   arr.length
来源：http://tmt.jiagoushi.top

TS:   arr.length
来源：http://srk.gotoacloud.top

Java: list.size();
来源：http://rxv.zdbjq.cn

Go:   len(arr)
来源：http://bvo.jqgfzy.top

Ruby: arr.length; arr.size
来源：http://gyq.zhoulong.xyz

C#:   list.Count;
来源：http://vkj.ehwqpu.com

[D07] 切片 / 取子数组
来源：http://ysw.vqdsnc.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pag.daria6918.cn

PHP:  array_slice($arr, 1, 3);
来源：http://mvl.ybcxt.top

JS:   arr.slice(1, 4);
来源：http://ujq.zhixingplan.top

TS:   arr.slice(1, 4);
来源：http://qio.tianlin.xyz

Java: list.subList(1, 4);
来源：http://ghq.hnxiangtu.top

Go:   arr[1:4]
来源：http://pkr.hammf.cn

Ruby: arr[1, 3]
来源：http://mai.pycfn.com

C#:   list.GetRange(1, 3);
来源：http://jit.hysaishi.cn

[D08] 合并两个数组
来源：http://una.smart0.xyz

Py:   a + b;  a.extend(b)
来源：http://qvr.yuxming.cn

PHP:  array_merge($a, $b);
来源：http://dyz.kuanghao11.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://dab.gaohongyu789.top

TS:   [...a, ...b];
来源：http://sxq.xuanzx.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xxf.epnwcf.com

Go:   append(a, b...)
来源：http://rva.xuetiantiany.cn

Ruby: a + b;  a.concat(b)
来源：http://jrt.shanyushiyangtech.top

C#:   a.Concat(b).ToList()
来源：http://wkw.sweek.top

[D09] 排序（升序）
来源：http://xke.yangfankeji.com

Py:   sorted(arr);  arr.sort()
来源：http://ayy.mhx1999.top

PHP:  sort($arr);
来源：http://eah.dashuyun.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lwf.haohaochexian.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://rai.sysykeji.top

Java: Collections.sort(list);  list.sort(null);
来源：http://vuh.birdmap.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ctq.shangyingyoupin.top

Ruby: arr.sort
来源：http://dbu.sufxvd.cn

C#:   list.Sort();
来源：http://tgu.zdqjudy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ylg.jlsjyb.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://alt.yanxiufei.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nvh.kuanghao11.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sxp.ivvv.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://sir.birdmap.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hgu.fehbvm.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jfk.shzxlz.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lxg.yj202588.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ouj.xingfuxueyuan.xyz

[D11] 反转数组
来源：http://wnb.hnxiangtu.top

Py:   arr[::-1];  arr.reverse()
来源：http://ubm.hesvh.cn

PHP:  array_reverse($arr);
来源：http://eib.iojbl.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zli.feifeiyinyue.top

TS:   [...arr].reverse();
来源：http://eft.yanxiufei.cn

Java: Collections.reverse(list);
来源：http://uks.chenjidiqi.icu

Go:   slices.Reverse(arr)
来源：http://asp.dashuyun.cn

Ruby: arr.reverse
来源：http://tec.ydzc1.top

C#:   list.Reverse();
来源：http://apk.jiagoushi.top

[D12] 查找元素下标
来源：http://nwv.daxiang520.top

Py:   arr.index(x);  x in arr
来源：http://qqc.jqgufenzy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://izr.bbcook.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vix.pengpengdd.cyou

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://djj.iojbl.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mmt.sxryk.cn

Go:   slices.Index(arr, x)
来源：http://blh.jinyuanbaomall.cn

Ruby: arr.index(x)
来源：http://ebx.ppjwa.cn

C#:   list.IndexOf(x);
来源：http://wtp.dianchejie.cn

[D13] 过滤（保留满足条件的）
来源：http://tuj.chenzaomai.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rim.ydzc1.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://oet.yj20258888.top

JS:   arr.filter(x => x > 3)
来源：http://aup.uphjek.com

TS:   arr.filter(x => x > 3)
来源：http://wgd.hysaishi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zvm.bbcook.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zmq.ivvv.top

Ruby: arr.select { |x| x > 3 }
来源：http://awi.fengsongda.top

C#:   list.Where(x => x > 3).ToList()
来源：http://rog.ydjk.org.cn

[D14] 映射转换（每个元素变形）
来源：http://ajx.fktsv.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vog.nanxuanxn.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xpg.shanyushiyangtech.top

JS:   arr.map(x => x * 2)
来源：http://ugf.yanxiufei.cn

TS:   arr.map(x => x * 2)
来源：http://vja.zhengqikj.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://fby.zhiwuduotai.top

Go:   // 手写循环
来源：http://olg.sweek.top

Ruby: arr.map { |x| x * 2 }
来源：http://eet.hysaishi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://lsv.svipenyu.cn


<!-- 参考信息 -->