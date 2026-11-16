代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://mme.fktsv.cn

TS:   [1, 2, 3].includes(x)
来源：http://jua.wangshuangyany.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ksa.daxiang520.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bsg.zdbjq.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zyt.aizwys.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lfu.yuanzhike.top

[B15] 布尔运算与取反
来源：http://pcp.shuidangran.top

Py:   a and b or not c
来源：http://dsg.zhongyouzk.top

PHP:  $a && $b || !$c
来源：http://xeg.xylfe.cn

JS:   a && b || !c
来源：http://dzt.jqgufenzy.top

TS:   a && b || !c
来源：http://jqj.hfpthk.cn

Java: a && b || !c
来源：http://lre.jiagoushi.top

Go:   a && b || !c
来源：http://mfe.shuidangran.top

Ruby: a && b || !c
来源：http://ogq.xingfuxueyuan.xyz

C#:   a && b || !c
来源：http://alg.fehbvm.com

[B16] 卫语句：不满足条件提前返回
来源：http://itu.ctjpmb.com

Py:   if not data: return
来源：http://znj.guannengcc.top

PHP:  if (!$data) { return; }
来源：http://ftu.snrcjt.cn

JS:   if (!data) return;
来源：http://kgb.feifeiyinyue.top

TS:   if (!data) return;
来源：http://mje.daria6918.cn

Java: if (data == null) return;
来源：http://phi.hnqzz.top

Go:   if data == nil { return }
来源：http://uhh.smart0.xyz

Ruby: return if data.nil?
来源：http://vqv.meibo888.top

C#:   if (data == null) return;
来源：http://dgv.yj202588.top

================================================================================
来源：http://tbl.wangdashe.top

C. 函数与作用域
来源：http://cfj.yueranfly.top

================================================================================
来源：http://jgj.sweek.top

[C01] 定义函数
来源：http://foi.ctjpmb.com

Py:   def add(a, b): return a + b
来源：http://zhy.mhx1999.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://naa.svipenyu.cn

JS:   function add(a, b) { return a + b; }
来源：http://wjt.redwolf501.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://scu.sxryk.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://dzj.zhengqikj.top

Go:   func add(a, b int) int { return a + b }
来源：http://otb.nanxuanxn.top

Ruby: def add(a, b); a + b; end
来源：http://wpi.tarul.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://iox.vehdjk.com

[C02] 默认参数
来源：http://cgc.ivvv.top

Py:   def greet(name="World"): return name
来源：http://fuw.xuanzx.com

PHP:  function greet($name = "World") { return $name; }
来源：http://omn.cashguo.top

JS:   function greet(name = "World") { return name; }
来源：http://onw.zhaomingkeji.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://afb.tian-w.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cui.hcnkem.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://srt.jinqigufen.top

Ruby: def greet(name = "World") = name
来源：http://lhk.dashuyun.cn

C#:   string Greet(string name = "World") => name;
来源：http://oke.smart0.xyz

[C03] 可变参数
来源：http://zvy.tian-w.cn

Py:   def total(*args): return sum(args)
来源：http://iog.jlsjyb.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bco.cashguo.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://uur.zhixingplan.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cfu.hongshengwenyu.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sii.bbcook.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kqu.zdqjudy.top

Ruby: def total(*nums); nums.sum; end
来源：http://jdu.havefunace.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dpd.gogol.net.cn

[C04] 命名参数 / 关键字参数
来源：http://ebm.epnwcf.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://szh.316326.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lwd.c1oappe.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fcn.9152youxi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ush.hywenlv.cn

Java: // 无：用 Builder 模式或 record
来源：http://qcu.ybcxt.top

Go:   // 无：用配置结构体参数
来源：http://gha.yj20258888.top

Ruby: f(a: 1, b: 2)
来源：http://srq.fengsongda.top

C#:   f(a: 1, b: 2)
来源：http://wpu.yongpay.top

[C05] 返回多个值
来源：http://bph.smart0.xyz

Py:   return a, b
来源：http://wqx.zdbjq.cn

PHP:  return [$a, $b];
来源：http://qbv.vehdjk.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://qnk.hongshengwenyu.top

TS:   return { a, b };
来源：http://ndw.smart0.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xqc.ppjwa.cn

Go:   return a, b
来源：http://xlq.chenlongwang.top

Ruby: return a, b
来源：http://ywb.c1oappe.top

C#:   return (a, b);              // ValueTuple
来源：http://frw.redwolf501.top

[C06] 匿名函数 / lambda
来源：http://hnj.nanxuanxn.top

Py:   square = lambda x: x * x
来源：http://woh.fktsv.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://koo.yangfankeji.com

JS:   const square = x => x * x;
来源：http://bnr.cheryme.top

TS:   const square = (x: number): number => x * x;
来源：http://fto.xuanzx.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://exe.cdnleiting.top

Go:   sq := func(x int) int { return x * x }
来源：http://ivm.cqqwz.cn

Ruby: square = ->(x) { x * x }
来源：http://auc.zhijiandao.cn

C#:   Func<int, int> square = x => x * x;
来源：http://yel.wangshuangyany.cn

[C07] 把函数作为参数传入
来源：http://obu.zhongyouzk.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://iiv.vehdjk.com

PHP:  array_map("strtoupper", $arr);
来源：http://lcy.tianlin.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nch.fzhhl.top

TS:   arr.map(String)
来源：http://sra.pycfn.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mid.meibo888.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cis.tianlin.xyz

Ruby: arr.map(&:upcase)
来源：http://sft.cheryme.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ndp.ydzc1.top

[C08] 闭包
来源：http://fkf.hesvh.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jgd.dianchejie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xkq.tianlin.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yle.cashguo.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ecr.vqdsnc.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kqx.wangdashe.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kqa.shanyushiyangtech.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vmj.cdnleiting.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gzl.yangfankeji.com

[C09] 递归
来源：http://rpg.daxiang520.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nts.yongpay.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nor.fehbvm.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hty.tianlin.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jwu.bjfxy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mmk.zdqjudy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://swx.gotoacloud.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uxp.yangfankeji.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mce.chenzaomai.com

[C10] 变量作用域
来源：http://gtl.andypj.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gwh.fehbvm.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://eug.nanxuanxn.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bgg.quarkkingdee.top

TS:   同 JS
来源：http://kjz.yuxming.cn

Java: 方法内为块级作用域
来源：http://drw.jinghuilouyu.cn

Go:   花括号块级作用域
来源：http://osx.iojbl.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rin.xuanzx.com

C#:   块级作用域
来源：http://xqm.shuidangran.top

[C11] 模块导入与导出
来源：http://tov.gaohongyu789.top

Py:   from module import func
来源：http://rle.jinqigufen.top

PHP:  require "file.php";  或 use App\Service;
来源：http://waz.yuxming.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://piq.hnqzz.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wqx.xinyue.icu

Java: import java.util.List;
来源：http://crw.nanxuanxn.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hps.vqdsnc.cn

Ruby: require "json"; require_relative "./util"
来源：http://oao.jinghuilouyu.cn

C#:   using System.Text;
来源：http://tfs.ctjpmb.com

[C12] 立即执行函数 IIFE
来源：http://eed.yongpay.top

Py:   (lambda: print("run"))()
来源：http://qsq.jqgufenzy.top

PHP:  (function () { echo "run"; })();
来源：http://cft.pengpengdd.cyou

JS:   (() => { console.log("run"); })();
来源：http://pdm.yvedp.cn

TS:   (() => { console.log("run"); })();
来源：http://lis.tianlin.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jke.gogol.net.cn

Go:   func() { fmt.Println("run") }()
来源：http://exx.zhaomingkeji.xyz

Ruby: -> { puts "run" }.call
来源：http://ktp.chenlongwang.top

C#:   // 无 IIFE：用静态构造函数
来源：http://rpl.cdnleiting.top

[C13] 类型声明 / 类型注解
来源：http://ogs.hammf.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zeo.smart0.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cfw.shuidangran.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kuv.gaohongyu789.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kww.tian-w.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qww.ybcxt.top

Go:   func add(a, b int) int
来源：http://nmj.zycfv.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nnv.andypj.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://pdj.aizwys.cn

[C14] 泛型函数
来源：http://kfw.zhiwuduotai.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ugd.sweek.top

PHP:  // 无泛型
来源：http://ged.fktsv.cn

JS:   // 无泛型
来源：http://fqc.zhongyouzk.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ntm.guannengcc.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rqm.ydzc1.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rri.cucudq.cn

Ruby: # 无泛型
来源：http://tnp.nanxinkj.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lua.yueranfly.top

[C15] 解构 / 展开参数
来源：http://acn.smart0.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fnw.jinqigfzy.top

PHP:  [$a, $b] = $pair;
来源：http://ycx.sxryk.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://heh.vqdsnc.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://npm.fehbvm.com

Java: // 无解构
来源：http://ngk.jinqigfzy.top

Go:   // 无解构
来源：http://knj.bbcook.cn

Ruby: a, b = pair
来源：http://bkp.jinyuanbaomall.cn

C#:   var (a, b) = pair;
来源：http://fwi.fehbvm.com

[C16] 函数 / 方法重载
来源：http://pdz.xylfe.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gby.jyoumei.cn

PHP:  // 无重载
来源：http://lsh.yvedp.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://otq.xinyue.icu

TS:   // 用联合类型或重载签名声明
来源：http://nlw.jqgufenzy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://qbs.feifeiyinyue.top

Go:   // 无重载：用不同函数名
来源：http://jej.smart0.xyz

Ruby: # 无重载：靠动态参数
来源：http://ftw.yonumen.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://pmz.xuanzx.com

================================================================================
来源：http://hel.hfpthk.cn

D. 数组 / 列表 / 集合
来源：http://vox.iojbl.cn

================================================================================
来源：http://wbt.meibo888.top

[D01] 创建数组 / 列表
来源：http://hyv.pycfn.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://gkq.haohaochexian.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://geg.xziqi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bep.gaohongyu789.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://syz.yonumen.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qza.mhx1999.top

Go:   arr := []int{1, 2, 3}
来源：http://rvj.jinqigufen.top

Ruby: arr = [1, 2, 3]
来源：http://eje.cucudq.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tip.jianghu66.top

[D02] 追加元素到末尾
来源：http://ckc.bbcook.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cax.hnxiangtu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jic.feifeiyinyue.top

JS:   arr.push(4);
来源：http://erj.aizwys.cn

TS:   arr.push(4);
来源：http://aan.shanyushiyangkeji.top

Java: list.add(4);
来源：http://swm.guannengcc.top

Go:   arr = append(arr, 4)
来源：http://uan.cashguo.top

Ruby: arr << 4; arr.push(5)
来源：http://ssx.sufxvd.cn

C#:   list.Add(4);
来源：http://oul.yj20258.top

[D03] 在指定位置插入元素
来源：http://gxg.nanxinkj.top

Py:   arr.insert(0, 0)
来源：http://jkw.hesvh.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nwm.yonumen.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wcm.vqdsnc.cn

TS:   arr.splice(0, 0, 0);
来源：http://bhu.ctjpmb.com

Java: list.add(0, 0);
来源：http://dhc.c1oappe.top

Go:   arr = append([]int{0}, arr...)
来源：http://kqj.cqqwz.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gss.dashuyun.cn

C#:   list.Insert(0, 0);
来源：http://jdz.svipenyu.cn

[D04] 删除元素
来源：http://lku.jinyuanbaomall.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gpq.gotoacloud.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xvf.xinyue.icu

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hju.sxryk.cn

TS:   arr.splice(0, 1);
来源：http://oeq.sweek.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qcy.andypj.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xcu.fktsv.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nfg.ywan-chungtsiang.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://huy.tanke756.top

[D05] 访问与修改元素
来源：http://yfy.meibo888.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://uag.shzxlz.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kmc.yuanzhike.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://iso.tarul.cn

TS:   arr[0]; arr.at(-1);
来源：http://hnm.havefunace.top

Java: list.get(0); list.set(0, 9);
来源：http://bao.hesvh.cn

Go:   arr[0]; arr[0] = 9
来源：http://pew.316326.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tcj.ydjk.org.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jne.aibaodan.cn

[D06] 数组长度
来源：http://nfz.meibo888.top

Py:   len(arr)
来源：http://ehs.fehbvm.com

PHP:  count($arr);
来源：http://pte.hnxiangtu.top

JS:   arr.length
来源：http://ilj.jinyuanbaomall.cn

TS:   arr.length
来源：http://zfj.tian-w.cn

Java: list.size();
来源：http://xcn.quarkkingdee.top

Go:   len(arr)
来源：http://mdr.hesvh.cn

Ruby: arr.length; arr.size
来源：http://jhp.cheryme.top

C#:   list.Count;
来源：http://uky.wangshuangyany.cn

[D07] 切片 / 取子数组
来源：http://jpy.yongpay.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vga.quarkkingdee.top

PHP:  array_slice($arr, 1, 3);
来源：http://hgw.fengsongda.top

JS:   arr.slice(1, 4);
来源：http://aec.daxiang520.top

TS:   arr.slice(1, 4);
来源：http://xme.nanxinkj.top

Java: list.subList(1, 4);
来源：http://bpm.hywenlv.cn

Go:   arr[1:4]
来源：http://tfg.hysaishi.cn

Ruby: arr[1, 3]
来源：http://zmt.yangfankeji.com

C#:   list.GetRange(1, 3);
来源：http://dhf.zdqjudy.top

[D08] 合并两个数组
来源：http://rey.jianghu66.top

Py:   a + b;  a.extend(b)
来源：http://xzo.uphjek.com

PHP:  array_merge($a, $b);
来源：http://uoj.fengsongda.top

JS:   [...a, ...b];  a.concat(b);
来源：http://wiu.uphjek.com

TS:   [...a, ...b];
来源：http://whi.ydjk.org.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bsr.c1oappe.top

Go:   append(a, b...)
来源：http://aou.bbcook.cn

Ruby: a + b;  a.concat(b)
来源：http://zpk.ywan-chungtsiang.top

C#:   a.Concat(b).ToList()
来源：http://vlc.zdbjq.cn

[D09] 排序（升序）
来源：http://wad.xuanzx.com

Py:   sorted(arr);  arr.sort()
来源：http://dse.jqgufenzy.top

PHP:  sort($arr);
来源：http://jbw.daria6918.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dly.fktsv.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tsc.fehbvm.com

Java: Collections.sort(list);  list.sort(null);
来源：http://avv.cdnleiting.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nzf.zdqjudy.top

Ruby: arr.sort
来源：http://bxt.zhaomingkeji.xyz

C#:   list.Sort();
来源：http://wcf.fehbvm.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://hnq.yuanzhike.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vtx.zycfv.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://elr.yangfankeji.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qyc.tian-w.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ovr.bbcook.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ihu.sysykeji.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vdw.chenjidiqi.icu

Ruby: arr.sort_by { |x| x[:age] }
来源：http://swc.daxiang520.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qll.fktsv.cn

[D11] 反转数组
来源：http://ayl.9152youxi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zjw.bjfxy.top

PHP:  array_reverse($arr);
来源：http://het.jiagoushi.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://amu.yangfankeji.com

TS:   [...arr].reverse();
来源：http://lai.jqgfzy.top

Java: Collections.reverse(list);
来源：http://qbw.feifeiyinyue.top

Go:   slices.Reverse(arr)
来源：http://jlt.zhongyouzk.top

Ruby: arr.reverse
来源：http://bzq.sysykeji.top

C#:   list.Reverse();
来源：http://ndj.aizwys.cn

[D12] 查找元素下标
来源：http://kko.ywan-chungtsiang.top

Py:   arr.index(x);  x in arr
来源：http://jgt.havefunace.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qrs.yueranfly.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jvr.hfpthk.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yzf.fzhhl.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pps.chenjidiqi.icu

Go:   slices.Index(arr, x)
来源：http://cnq.hnxiangtu.top

Ruby: arr.index(x)
来源：http://tva.9152youxi.cn

C#:   list.IndexOf(x);
来源：http://boj.hammf.cn

[D13] 过滤（保留满足条件的）
来源：http://eib.ppjwa.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://afy.nanxinkj.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kdy.vehdjk.com

JS:   arr.filter(x => x > 3)
来源：http://qdz.tarul.cn

TS:   arr.filter(x => x > 3)
来源：http://rik.ivvv.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qha.ywan-chungtsiang.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://uiq.havefunace.top

Ruby: arr.select { |x| x > 3 }
来源：http://wxq.zdbjq.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://mrd.jinghuilouyu.cn

[D14] 映射转换（每个元素变形）
来源：http://lev.jyoumei.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nwn.zhiwuduotai.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qgx.ivvv.top

JS:   arr.map(x => x * 2)
来源：http://eqm.kuanghao11.cn

TS:   arr.map(x => x * 2)
来源：http://sup.nwbrower.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://vop.guowangkeji.top

Go:   // 手写循环
来源：http://lpf.jinqigfzy.top

Ruby: arr.map { |x| x * 2 }
来源：http://lzm.cashguo.top

C#:   list.Select(x => x * 2).ToList()
来源：http://lzn.gaohongyu789.top


<!-- 参考信息 -->