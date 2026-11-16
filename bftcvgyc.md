代发 wailian999

Go:   a && b || !c
来源：http://mpu.c1oappe.top

Ruby: a && b || !c
来源：http://mme.hnxiangtu.top

C#:   a && b || !c
来源：http://guu.52xcode.cn

[B16] 卫语句：不满足条件提前返回
来源：http://bgr.svipenyu.cn

Py:   if not data: return
来源：http://vgw.fanxiaobao.xyz

PHP:  if (!$data) { return; }
来源：http://uyd.xuetiantiany.cn

JS:   if (!data) return;
来源：http://rsr.shangyingyoupin.top

TS:   if (!data) return;
来源：http://jvt.vehdjk.com

Java: if (data == null) return;
来源：http://ywa.redwolf501.top

Go:   if data == nil { return }
来源：http://vox.hysaishi.cn

Ruby: return if data.nil?
来源：http://nvh.shanyushiyangtech.top

C#:   if (data == null) return;
来源：http://zue.hfpthk.cn

================================================================================
来源：http://ael.hesvh.cn

C. 函数与作用域
来源：http://jqn.dianchejie.cn

================================================================================
来源：http://zpm.fehbvm.com

[C01] 定义函数
来源：http://epw.ehwqpu.com

Py:   def add(a, b): return a + b
来源：http://xow.chenjidiqi.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hyn.hcnkem.com

JS:   function add(a, b) { return a + b; }
来源：http://uhv.redwolf501.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vso.hfpthk.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lly.jinghuilouyu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://mcu.wangdashe.top

Ruby: def add(a, b); a + b; end
来源：http://dvk.zycfv.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://oiy.52xcode.cn

[C02] 默认参数
来源：http://gsb.9152youxi.cn

Py:   def greet(name="World"): return name
来源：http://ehj.yanxiufei.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://fdu.redwolf501.top

JS:   function greet(name = "World") { return name; }
来源：http://hlc.guowangkeji.top

TS:   function greet(name: string = "World") { return name; }
来源：http://avn.zhiwuduotai.top

Java: // 无默认参数：方法重载或 Optional
来源：http://fqq.tarul.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ikn.zhiwuduotai.top

Ruby: def greet(name = "World") = name
来源：http://thm.jinqigufen.top

C#:   string Greet(string name = "World") => name;
来源：http://axe.fzhhl.top

[C03] 可变参数
来源：http://vrw.xuanzx.com

Py:   def total(*args): return sum(args)
来源：http://ypv.c1oappe.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wtz.hywenlv.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vgf.c1oappe.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hrv.chenzaomai.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://arf.yueranfly.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ews.cheryme.top

Ruby: def total(*nums); nums.sum; end
来源：http://cht.zhoulong.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pyd.xziqi.cn

[C04] 命名参数 / 关键字参数
来源：http://cge.ehwqpu.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jhc.ybcxt.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://haw.shzxlz.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://foy.cqqwz.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wzv.tian-w.cn

Java: // 无：用 Builder 模式或 record
来源：http://sph.jianghu66.top

Go:   // 无：用配置结构体参数
来源：http://xrm.daria6918.cn

Ruby: f(a: 1, b: 2)
来源：http://lhu.aizwys.cn

C#:   f(a: 1, b: 2)
来源：http://oay.fktsv.cn

[C05] 返回多个值
来源：http://jos.hammf.cn

Py:   return a, b
来源：http://cbt.yuanzhike.top

PHP:  return [$a, $b];
来源：http://xgg.shanyushiyangtech.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://xtx.yfazqb.com

TS:   return { a, b };
来源：http://jpx.vehdjk.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lap.daxiang520.top

Go:   return a, b
来源：http://lpy.dianchejie.cn

Ruby: return a, b
来源：http://blv.hnxiangtu.top

C#:   return (a, b);              // ValueTuple
来源：http://akr.zhongyouzk.top

[C06] 匿名函数 / lambda
来源：http://urj.jqgfzy.top

Py:   square = lambda x: x * x
来源：http://ism.sxryk.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://oiy.fengsongda.top

JS:   const square = x => x * x;
来源：http://dii.gzhubu.top

TS:   const square = (x: number): number => x * x;
来源：http://byz.nanxinkj.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zcp.ydzc1.top

Go:   sq := func(x int) int { return x * x }
来源：http://tlu.zhiwuduotai.top

Ruby: square = ->(x) { x * x }
来源：http://dvc.gaohongyu789.top

C#:   Func<int, int> square = x => x * x;
来源：http://iih.zdqjudy.top

[C07] 把函数作为参数传入
来源：http://ety.dianchejie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://boa.nanxinkj.top

PHP:  array_map("strtoupper", $arr);
来源：http://mom.guowangkeji.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sfk.birdmap.top

TS:   arr.map(String)
来源：http://bls.gzhubu.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://iyb.guowangkeji.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://crm.hammf.cn

Ruby: arr.map(&:upcase)
来源：http://pkt.xziqi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://iuk.nwbrower.top

[C08] 闭包
来源：http://tgc.gzhubu.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fqx.jinghuilouyu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wfd.aizwys.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jnz.sweek.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://aix.hnqzz.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zxt.hywenlv.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://njb.gogol.net.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lgt.xuanzx.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cir.fehbvm.com

[C09] 递归
来源：http://bfv.svipenyu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://aqm.fzhhl.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nud.chenlongwang.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://drv.zhixingplan.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dxv.fzhhl.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dxj.chenzaomai.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qwp.gogol.net.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wjl.ivvv.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mme.uphjek.com

[C10] 变量作用域
来源：http://buf.sysykeji.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xlb.yanxiufei.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wae.316326.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gqq.0kj1m.cn

TS:   同 JS
来源：http://mtc.epnwcf.com

Java: 方法内为块级作用域
来源：http://mxh.daria6918.cn

Go:   花括号块级作用域
来源：http://lsp.0kj1m.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ols.cashguo.top

C#:   块级作用域
来源：http://pzf.sjlbkw.cn

[C11] 模块导入与导出
来源：http://sph.fehbvm.com

Py:   from module import func
来源：http://byv.aizwys.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://kwi.hnqzz.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://nqj.gaohongyu789.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wqt.tanke756.top

Java: import java.util.List;
来源：http://cmg.yj20258888.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://uur.uphjek.com

Ruby: require "json"; require_relative "./util"
来源：http://wwu.hysaishi.cn

C#:   using System.Text;
来源：http://ogx.xylfe.cn

[C12] 立即执行函数 IIFE
来源：http://bza.fanxiaobao.xyz

Py:   (lambda: print("run"))()
来源：http://cit.zhiwuduotai.top

PHP:  (function () { echo "run"; })();
来源：http://eym.daxiang520.top

JS:   (() => { console.log("run"); })();
来源：http://xpe.sxryk.cn

TS:   (() => { console.log("run"); })();
来源：http://cbq.shuidangran.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xss.dashuyun.cn

Go:   func() { fmt.Println("run") }()
来源：http://uzj.kuanghao11.cn

Ruby: -> { puts "run" }.call
来源：http://dnc.ehwqpu.com

C#:   // 无 IIFE：用静态构造函数
来源：http://ela.jinyuanbaomall.cn

[C13] 类型声明 / 类型注解
来源：http://fyh.fengsongda.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dwl.zdqjudy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://omb.zhengqikj.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zvt.yueranfly.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ckb.daria6918.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ubs.pycfn.com

Go:   func add(a, b int) int
来源：http://drk.yuxming.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kqa.yanxiufei.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fre.hongshengwenyu.top

[C14] 泛型函数
来源：http://bib.zhoulong.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pjr.kuanghao11.cn

PHP:  // 无泛型
来源：http://csy.jinqigufen.top

JS:   // 无泛型
来源：http://cuv.yj20258888.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bcb.snrcjt.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fls.ctjpmb.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fsi.ywan-chungtsiang.top

Ruby: # 无泛型
来源：http://fbm.fehbvm.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ucz.hnqzz.top

[C15] 解构 / 展开参数
来源：http://hwo.fengsongda.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ygs.xuetiantiany.cn

PHP:  [$a, $b] = $pair;
来源：http://gcw.epnwcf.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://skw.tian-w.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rmk.uphjek.com

Java: // 无解构
来源：http://hjr.pengpengdd.cyou

Go:   // 无解构
来源：http://zkj.gotoacloud.top

Ruby: a, b = pair
来源：http://kra.birdmap.top

C#:   var (a, b) = pair;
来源：http://hlj.guannengcc.top

[C16] 函数 / 方法重载
来源：http://ppy.shzxlz.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://iyu.snrcjt.cn

PHP:  // 无重载
来源：http://ryn.hammf.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://mdx.ywan-chungtsiang.top

TS:   // 用联合类型或重载签名声明
来源：http://qsi.yj202588.top

Java: void f(int a) {}  void f(String a) {}
来源：http://stw.jinghuilouyu.cn

Go:   // 无重载：用不同函数名
来源：http://esj.ehwqpu.com

Ruby: # 无重载：靠动态参数
来源：http://zfi.jianghu66.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://iyx.mhx1999.top

================================================================================
来源：http://fhx.fehbvm.com

D. 数组 / 列表 / 集合
来源：http://ylw.zdqjudy.top

================================================================================
来源：http://weq.tianlin.xyz

[D01] 创建数组 / 列表
来源：http://pum.nanxinkj.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://bhe.dianchejie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zaa.nwbrower.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cog.zhijiandao.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://vbn.xylfe.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gai.0kj1m.cn

Go:   arr := []int{1, 2, 3}
来源：http://koa.shuidangran.top

Ruby: arr = [1, 2, 3]
来源：http://vou.uphjek.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fht.ydjk.org.cn

[D02] 追加元素到末尾
来源：http://hmw.hywenlv.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://iga.ywan-chungtsiang.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://umc.zhiwuduotai.top

JS:   arr.push(4);
来源：http://zwg.hongshengwenyu.top

TS:   arr.push(4);
来源：http://dkw.tarul.cn

Java: list.add(4);
来源：http://zff.ivvv.top

Go:   arr = append(arr, 4)
来源：http://uao.dashuyun.cn

Ruby: arr << 4; arr.push(5)
来源：http://vif.bjfxy.top

C#:   list.Add(4);
来源：http://yun.aibaodan.cn

[D03] 在指定位置插入元素
来源：http://xqk.aibaodan.cn

Py:   arr.insert(0, 0)
来源：http://dep.epnwcf.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://amn.hywenlv.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sgm.sysykeji.top

TS:   arr.splice(0, 0, 0);
来源：http://kwc.316326.xyz

Java: list.add(0, 0);
来源：http://vhr.guowangkeji.top

Go:   arr = append([]int{0}, arr...)
来源：http://qnm.ydzc1.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ybw.zhiwuduotai.top

C#:   list.Insert(0, 0);
来源：http://vhb.0kj1m.cn

[D04] 删除元素
来源：http://pha.ehwqpu.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fxm.gzhubu.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://okd.cqqwz.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://crc.9152youxi.cn

TS:   arr.splice(0, 1);
来源：http://mrf.guowangkeji.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hbm.iojbl.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yby.cdnleiting.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dof.jiagoushi.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tnf.jianghu66.top

[D05] 访问与修改元素
来源：http://iqw.nwbrower.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vzf.meibo888.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nik.xuanzx.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bmp.yvedp.cn

TS:   arr[0]; arr.at(-1);
来源：http://crw.hongshengwenyu.top

Java: list.get(0); list.set(0, 9);
来源：http://hcx.xylfe.cn

Go:   arr[0]; arr[0] = 9
来源：http://tfu.gogol.net.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vwo.jqgfzy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xji.zhiwuduotai.top

[D06] 数组长度
来源：http://eoh.yj20258888.top

Py:   len(arr)
来源：http://sfx.vehdjk.com

PHP:  count($arr);
来源：http://lkl.hfpthk.cn

JS:   arr.length
来源：http://vez.redwolf501.top

TS:   arr.length
来源：http://uar.aizwys.cn

Java: list.size();
来源：http://cms.cucudq.cn

Go:   len(arr)
来源：http://lpc.aibaodan.cn

Ruby: arr.length; arr.size
来源：http://iqk.hcnkem.com

C#:   list.Count;
来源：http://rfs.pengpengdd.cyou

[D07] 切片 / 取子数组
来源：http://soc.zycfv.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wyy.yvedp.cn

PHP:  array_slice($arr, 1, 3);
来源：http://lra.mhx1999.top

JS:   arr.slice(1, 4);
来源：http://xnm.fengsongda.top

TS:   arr.slice(1, 4);
来源：http://qcc.quarkkingdee.top

Java: list.subList(1, 4);
来源：http://lrv.chenlongwang.top

Go:   arr[1:4]
来源：http://ggb.jianghu66.top

Ruby: arr[1, 3]
来源：http://yun.shuidangran.top

C#:   list.GetRange(1, 3);
来源：http://fsb.jqgfzy.top

[D08] 合并两个数组
来源：http://jcm.zhengqikj.top

Py:   a + b;  a.extend(b)
来源：http://aft.jinghuilouyu.cn

PHP:  array_merge($a, $b);
来源：http://vpd.vehdjk.com

JS:   [...a, ...b];  a.concat(b);
来源：http://sfl.zhixingplan.top

TS:   [...a, ...b];
来源：http://gtb.yvedp.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://uya.vqdsnc.cn

Go:   append(a, b...)
来源：http://vpc.sufxvd.cn

Ruby: a + b;  a.concat(b)
来源：http://vzp.52xcode.cn

C#:   a.Concat(b).ToList()
来源：http://fwm.zhijiandao.cn

[D09] 排序（升序）
来源：http://ucm.mhx1999.top

Py:   sorted(arr);  arr.sort()
来源：http://zce.fehbvm.com

PHP:  sort($arr);
来源：http://hkm.hysaishi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lvq.cheryme.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://fkw.yfazqb.com

Java: Collections.sort(list);  list.sort(null);
来源：http://czo.jianghu66.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zpt.birdmap.top

Ruby: arr.sort
来源：http://sje.yfazqb.com

C#:   list.Sort();
来源：http://gms.fengsongda.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://lbs.uphjek.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cng.jinghuilouyu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://srs.cashguo.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tlw.shanyushiyangkeji.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qod.feifeiyinyue.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://knm.cqqwz.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kiz.daxiang520.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mxy.vqdsnc.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ahx.bjfxy.top

[D11] 反转数组
来源：http://cjj.tanke756.top

Py:   arr[::-1];  arr.reverse()
来源：http://yzv.jqgufenzy.top

PHP:  array_reverse($arr);
来源：http://lls.yanxiufei.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://scf.0kj1m.cn

TS:   [...arr].reverse();
来源：http://fbl.yfazqb.com

Java: Collections.reverse(list);
来源：http://nle.birdmap.top

Go:   slices.Reverse(arr)
来源：http://dxd.daria6918.cn

Ruby: arr.reverse
来源：http://kte.xuetiantiany.cn

C#:   list.Reverse();
来源：http://cta.jiagoushi.top

[D12] 查找元素下标
来源：http://vrc.feifeiyinyue.top

Py:   arr.index(x);  x in arr
来源：http://kbq.dashuyun.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fsq.cdnleiting.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://szv.zhoulong.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ydo.bbcook.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wpu.dianchejie.cn

Go:   slices.Index(arr, x)
来源：http://iia.svipenyu.cn

Ruby: arr.index(x)
来源：http://iqx.guowangkeji.top

C#:   list.IndexOf(x);
来源：http://xlp.yueranfly.top

[D13] 过滤（保留满足条件的）
来源：http://nkh.jinqigufen.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qql.wangshuangyany.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rht.zhijiandao.cn

JS:   arr.filter(x => x > 3)
来源：http://vjc.9152youxi.cn

TS:   arr.filter(x => x > 3)
来源：http://cmt.cheryme.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://snz.jlsjyb.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tlv.guowangkeji.top

Ruby: arr.select { |x| x > 3 }
来源：http://uns.fengsongda.top

C#:   list.Where(x => x > 3).ToList()
来源：http://koc.52xcode.cn

[D14] 映射转换（每个元素变形）
来源：http://fqj.jlsjyb.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vif.ehwqpu.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jnm.ctjpmb.com

JS:   arr.map(x => x * 2)
来源：http://nro.yangfankeji.com

TS:   arr.map(x => x * 2)
来源：http://bgd.hysaishi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://iih.sxryk.cn

Go:   // 手写循环
来源：http://xcm.snrcjt.cn

Ruby: arr.map { |x| x * 2 }
来源：http://yhl.havefunace.top

C#:   list.Select(x => x * 2).ToList()
来源：http://mnb.shanyushiyangkeji.top

[D15] 去重
来源：http://oxv.jinyuanbaomall.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ont.chenjidiqi.icu

PHP:  array_unique($arr);
来源：http://fwn.zycfv.cn

JS:   [...new Set(arr)]
来源：http://sts.yueranfly.top

TS:   [...new Set(arr)]
来源：http://hxr.jinqigufen.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ply.redwolf501.top

Go:   // 用 map[T]struct{} 手写
来源：http://ocq.vehdjk.com

Ruby: arr.uniq
来源：http://gin.epnwcf.com

C#:   list.Distinct().ToList()
来源：http://zyz.hammf.cn

[D16] 求和与平均值
来源：http://lzd.redwolf501.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rli.quarkkingdee.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hfn.shanyushiyangkeji.top


<!-- 参考信息 -->