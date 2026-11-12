代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://smb.316326.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://foy.smart0.xyz

[B15] 布尔运算与取反
来源：http://kjl.shanyushiyangtech.top

Py:   a and b or not c
来源：http://enx.xziqi.cn

PHP:  $a && $b || !$c
来源：http://opk.havefunace.top

JS:   a && b || !c
来源：http://adb.yj20258888.top

TS:   a && b || !c
来源：http://vuo.aizwys.cn

Java: a && b || !c
来源：http://zzq.ydzc1.top

Go:   a && b || !c
来源：http://kxk.aizwys.cn

Ruby: a && b || !c
来源：http://tkd.chenzaomai.com

C#:   a && b || !c
来源：http://cti.guannengcc.top

[B16] 卫语句：不满足条件提前返回
来源：http://vwk.hfpthk.cn

Py:   if not data: return
来源：http://nes.yj20258.top

PHP:  if (!$data) { return; }
来源：http://mdi.hysaishi.cn

JS:   if (!data) return;
来源：http://ija.9152youxi.cn

TS:   if (!data) return;
来源：http://ipo.sysykeji.top

Java: if (data == null) return;
来源：http://qpn.nanxinkj.top

Go:   if data == nil { return }
来源：http://ivq.gogol.net.cn

Ruby: return if data.nil?
来源：http://qsh.dashuyun.cn

C#:   if (data == null) return;
来源：http://udz.zhixingplan.top

================================================================================
来源：http://cwj.meibo888.top

C. 函数与作用域
来源：http://ixb.yj20258.top

================================================================================
来源：http://lod.ctjpmb.com

[C01] 定义函数
来源：http://gou.dashuyun.cn

Py:   def add(a, b): return a + b
来源：http://goo.guannengcc.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://asg.shuidangran.top

JS:   function add(a, b) { return a + b; }
来源：http://xcp.zdqjudy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://amk.yuanzhike.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ozi.nwbrower.top

Go:   func add(a, b int) int { return a + b }
来源：http://wgs.316326.xyz

Ruby: def add(a, b); a + b; end
来源：http://dtk.xylfe.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://erz.aizwys.cn

[C02] 默认参数
来源：http://yvh.uphjek.com

Py:   def greet(name="World"): return name
来源：http://zpf.fanxiaobao.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://jnk.ivvv.top

JS:   function greet(name = "World") { return name; }
来源：http://mzz.jqgfzy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://kae.dianchejie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://csg.bbcook.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qcn.hesvh.cn

Ruby: def greet(name = "World") = name
来源：http://trn.yueranfly.top

C#:   string Greet(string name = "World") => name;
来源：http://ywc.hysaishi.cn

[C03] 可变参数
来源：http://xxv.jlsjyb.cn

Py:   def total(*args): return sum(args)
来源：http://sdz.yj20258.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://oup.quarkkingdee.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gbe.hywenlv.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://iec.nanxuanxn.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bfq.sysykeji.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nst.sweek.top

Ruby: def total(*nums); nums.sum; end
来源：http://pye.zdbjq.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://afx.nwbrower.top

[C04] 命名参数 / 关键字参数
来源：http://zkm.andypj.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vye.zhoulong.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wbx.hnxiangtu.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rxk.ywan-chungtsiang.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tbs.tianlin.xyz

Java: // 无：用 Builder 模式或 record
来源：http://pqu.gaohongyu789.top

Go:   // 无：用配置结构体参数
来源：http://kvr.chenzaomai.com

Ruby: f(a: 1, b: 2)
来源：http://ncd.haohaochexian.top

C#:   f(a: 1, b: 2)
来源：http://yzz.iojbl.cn

[C05] 返回多个值
来源：http://jxu.vqdsnc.cn

Py:   return a, b
来源：http://zgf.gotoacloud.top

PHP:  return [$a, $b];
来源：http://qyg.yangfankeji.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://sie.zdqjudy.top

TS:   return { a, b };
来源：http://pqm.shuidangran.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mka.nanxuanxn.top

Go:   return a, b
来源：http://zao.shanyushiyangkeji.top

Ruby: return a, b
来源：http://rmm.ybcxt.top

C#:   return (a, b);              // ValueTuple
来源：http://lra.quarkkingdee.top

[C06] 匿名函数 / lambda
来源：http://uvz.hnqzz.top

Py:   square = lambda x: x * x
来源：http://ofl.nanxinkj.top

PHP:  $square = fn($x) => $x * $x;
来源：http://tdb.xuanzx.com

JS:   const square = x => x * x;
来源：http://hls.yj202588.top

TS:   const square = (x: number): number => x * x;
来源：http://fte.nanxinkj.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cgj.shanyushiyangtech.top

Go:   sq := func(x int) int { return x * x }
来源：http://jmq.wangshuangyany.cn

Ruby: square = ->(x) { x * x }
来源：http://cdr.jinghuilouyu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fic.jinghuilouyu.cn

[C07] 把函数作为参数传入
来源：http://oby.shanyushiyangkeji.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jmo.guowangkeji.top

PHP:  array_map("strtoupper", $arr);
来源：http://avz.zhixingplan.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wgm.zhiwuduotai.top

TS:   arr.map(String)
来源：http://dew.vqdsnc.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://feu.pycfn.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mat.redwolf501.top

Ruby: arr.map(&:upcase)
来源：http://cnm.jinyuanbaomall.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://aqw.shangyingyoupin.top

[C08] 闭包
来源：http://upc.redwolf501.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://deh.chenzaomai.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ees.hesvh.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vib.gogol.net.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rzl.ehwqpu.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ggc.ydjk.org.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ljq.daxiang520.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jif.yj20258.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fdf.jinqigfzy.top

[C09] 递归
来源：http://umt.feifeiyinyue.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gln.bjfxy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ogu.cdnleiting.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hjn.zhoulong.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zws.hcnkem.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vgr.nanxinkj.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uow.gotoacloud.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://eak.yongpay.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rnd.haohaochexian.top

[C10] 变量作用域
来源：http://chi.svipenyu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://eer.shzxlz.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qnj.snrcjt.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://uwg.jlsjyb.cn

TS:   同 JS
来源：http://nai.wangshuangyany.cn

Java: 方法内为块级作用域
来源：http://kyv.fktsv.cn

Go:   花括号块级作用域
来源：http://yvk.9152youxi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hyb.hywenlv.cn

C#:   块级作用域
来源：http://jnl.ctjpmb.com

[C11] 模块导入与导出
来源：http://cwk.c1oappe.top

Py:   from module import func
来源：http://xdl.xuanzx.com

PHP:  require "file.php";  或 use App\Service;
来源：http://zdm.xylfe.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://qou.jianghu66.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lbd.andypj.xyz

Java: import java.util.List;
来源：http://ryu.jyoumei.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://oaz.nanxinkj.top

Ruby: require "json"; require_relative "./util"
来源：http://gdl.zdqjudy.top

C#:   using System.Text;
来源：http://ngt.vehdjk.com

[C12] 立即执行函数 IIFE
来源：http://sbs.0kj1m.cn

Py:   (lambda: print("run"))()
来源：http://uwq.zdbjq.cn

PHP:  (function () { echo "run"; })();
来源：http://wtf.xylfe.cn

JS:   (() => { console.log("run"); })();
来源：http://hnz.fengsongda.top

TS:   (() => { console.log("run"); })();
来源：http://baw.daxiang520.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://def.wangdashe.top

Go:   func() { fmt.Println("run") }()
来源：http://bxk.hywenlv.cn

Ruby: -> { puts "run" }.call
来源：http://mwx.haohaochexian.top

C#:   // 无 IIFE：用静态构造函数
来源：http://nxc.yj20258888.top

[C13] 类型声明 / 类型注解
来源：http://ztw.gaohongyu789.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://apu.gzhubu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zni.nwbrower.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://piv.jyoumei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fca.shzxlz.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wsf.xinyue.icu

Go:   func add(a, b int) int
来源：http://rmh.chenzaomai.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://duo.zhengqikj.top

C#:   int Add(int a, int b) => a + b;
来源：http://mbf.cdnleiting.top

[C14] 泛型函数
来源：http://cng.tianlin.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gad.pycfn.com

PHP:  // 无泛型
来源：http://bvz.fehbvm.com

JS:   // 无泛型
来源：http://evz.daria6918.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tvu.jqgufenzy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hik.tian-w.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cpl.xinyue.icu

Ruby: # 无泛型
来源：http://aja.jianghu66.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xbr.zhongyouzk.top

[C15] 解构 / 展开参数
来源：http://swa.jinghuilouyu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ist.meibo888.top

PHP:  [$a, $b] = $pair;
来源：http://znu.nanxuanxn.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zdj.fengsongda.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://iiu.hysaishi.cn

Java: // 无解构
来源：http://ram.kuanghao11.cn

Go:   // 无解构
来源：http://ngg.pycfn.com

Ruby: a, b = pair
来源：http://efy.fengsongda.top

C#:   var (a, b) = pair;
来源：http://ddm.redwolf501.top

[C16] 函数 / 方法重载
来源：http://oat.dianchejie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://olv.birdmap.top

PHP:  // 无重载
来源：http://bvf.xylfe.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://grh.fanxiaobao.xyz

TS:   // 用联合类型或重载签名声明
来源：http://geg.cdnleiting.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ghf.yvedp.cn

Go:   // 无重载：用不同函数名
来源：http://rzn.feifeiyinyue.top

Ruby: # 无重载：靠动态参数
来源：http://wgd.ybcxt.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ujx.sxryk.cn

================================================================================
来源：http://ahe.uphjek.com

D. 数组 / 列表 / 集合
来源：http://sft.yj20258888.top

================================================================================
来源：http://bif.jinqigufen.top

[D01] 创建数组 / 列表
来源：http://htj.cdnleiting.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://azx.pycfn.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lnn.jqgufenzy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hhu.yonumen.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://now.yanxiufei.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xof.uphjek.com

Go:   arr := []int{1, 2, 3}
来源：http://rls.nanxinkj.top

Ruby: arr = [1, 2, 3]
来源：http://ehk.wangshuangyany.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://aly.quarkkingdee.top

[D02] 追加元素到末尾
来源：http://kqb.cheryme.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lwx.shuidangran.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qug.zhengqikj.top

JS:   arr.push(4);
来源：http://ljz.chenlongwang.top

TS:   arr.push(4);
来源：http://vwb.smart0.xyz

Java: list.add(4);
来源：http://zwo.tianlin.xyz

Go:   arr = append(arr, 4)
来源：http://qol.yuxming.cn

Ruby: arr << 4; arr.push(5)
来源：http://ajp.sweek.top

C#:   list.Add(4);
来源：http://tsv.ivvv.top

[D03] 在指定位置插入元素
来源：http://dme.hywenlv.cn

Py:   arr.insert(0, 0)
来源：http://noh.hysaishi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://obl.tian-w.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wrk.yj20258.top

TS:   arr.splice(0, 0, 0);
来源：http://qny.hywenlv.cn

Java: list.add(0, 0);
来源：http://ubm.iojbl.cn

Go:   arr = append([]int{0}, arr...)
来源：http://amv.zhongyouzk.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vmb.yueranfly.top

C#:   list.Insert(0, 0);
来源：http://sxp.hnxiangtu.top

[D04] 删除元素
来源：http://xjn.vehdjk.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ufe.xylfe.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vao.fktsv.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mjv.iojbl.cn

TS:   arr.splice(0, 1);
来源：http://kna.shangyingyoupin.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lid.hammf.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sgz.ehwqpu.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://czc.quarkkingdee.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wof.aibaodan.cn

[D05] 访问与修改元素
来源：http://emx.yangfankeji.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tdg.jinqigfzy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hyd.jqgufenzy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://edz.ehwqpu.com

TS:   arr[0]; arr.at(-1);
来源：http://izy.tianlin.xyz

Java: list.get(0); list.set(0, 9);
来源：http://olk.feifeiyinyue.top

Go:   arr[0]; arr[0] = 9
来源：http://owz.xinyue.icu

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ffn.bjfxy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lgn.shanyushiyangtech.top

[D06] 数组长度
来源：http://owp.gogol.net.cn

Py:   len(arr)
来源：http://oxk.shangyingyoupin.top

PHP:  count($arr);
来源：http://kgm.fktsv.cn

JS:   arr.length
来源：http://qjh.jianghu66.top

TS:   arr.length
来源：http://kmd.shanyushiyangtech.top

Java: list.size();
来源：http://ybc.fzhhl.top

Go:   len(arr)
来源：http://dml.0kj1m.cn

Ruby: arr.length; arr.size
来源：http://hww.sxryk.cn

C#:   list.Count;
来源：http://fva.yj20258.top

[D07] 切片 / 取子数组
来源：http://jln.hywenlv.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mzl.zycfv.cn

PHP:  array_slice($arr, 1, 3);
来源：http://kuf.tianlin.xyz

JS:   arr.slice(1, 4);
来源：http://qgo.cqqwz.cn

TS:   arr.slice(1, 4);
来源：http://vzq.yvedp.cn

Java: list.subList(1, 4);
来源：http://lch.cashguo.top

Go:   arr[1:4]
来源：http://dap.meibo888.top

Ruby: arr[1, 3]
来源：http://mdo.zycfv.cn

C#:   list.GetRange(1, 3);
来源：http://lcz.zdqjudy.top

[D08] 合并两个数组
来源：http://jon.aibaodan.cn

Py:   a + b;  a.extend(b)
来源：http://emf.pengpengdd.cyou

PHP:  array_merge($a, $b);
来源：http://zno.52xcode.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hgq.jqgufenzy.top

TS:   [...a, ...b];
来源：http://emz.shzxlz.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lco.zhiwuduotai.top

Go:   append(a, b...)
来源：http://lcg.xuetiantiany.cn

Ruby: a + b;  a.concat(b)
来源：http://fdj.aibaodan.cn

C#:   a.Concat(b).ToList()
来源：http://jnc.xinyue.icu

[D09] 排序（升序）
来源：http://dtl.cucudq.cn

Py:   sorted(arr);  arr.sort()
来源：http://tyf.yonumen.top

PHP:  sort($arr);
来源：http://gde.yuanzhike.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tab.gaohongyu789.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://xea.yuxming.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://sfj.gotoacloud.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gkz.jinyuanbaomall.cn

Ruby: arr.sort
来源：http://nsv.zhaomingkeji.xyz

C#:   list.Sort();
来源：http://wov.c1oappe.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://zzv.zdqjudy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kio.pengpengdd.cyou

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gvr.zdbjq.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fnw.dianchejie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hcg.wangdashe.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wey.yj202588.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pqc.bbcook.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yma.snrcjt.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://djy.yuanzhike.top

[D11] 反转数组
来源：http://vhw.yueranfly.top

Py:   arr[::-1];  arr.reverse()
来源：http://gkh.ywan-chungtsiang.top

PHP:  array_reverse($arr);
来源：http://gao.jianghu66.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tcw.meibo888.top

TS:   [...arr].reverse();
来源：http://fsi.bjfxy.top

Java: Collections.reverse(list);
来源：http://ybc.fzhhl.top

Go:   slices.Reverse(arr)
来源：http://emk.hcnkem.com

Ruby: arr.reverse
来源：http://fnw.meibo888.top

C#:   list.Reverse();
来源：http://xsl.hcnkem.com

[D12] 查找元素下标
来源：http://npa.jianghu66.top

Py:   arr.index(x);  x in arr
来源：http://blf.hysaishi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yne.gzhubu.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://syk.jiagoushi.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://swf.hesvh.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qys.andypj.xyz

Go:   slices.Index(arr, x)
来源：http://rfm.9152youxi.cn

Ruby: arr.index(x)
来源：http://zud.yanxiufei.cn

C#:   list.IndexOf(x);
来源：http://rod.xuanzx.com

[D13] 过滤（保留满足条件的）
来源：http://ybf.ctjpmb.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lur.cqqwz.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nmb.ybcxt.top

JS:   arr.filter(x => x > 3)
来源：http://ylj.kuanghao11.cn

TS:   arr.filter(x => x > 3)
来源：http://utj.birdmap.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qdj.dashuyun.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nqw.quarkkingdee.top

Ruby: arr.select { |x| x > 3 }
来源：http://wxk.tian-w.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://mpf.yonumen.top

[D14] 映射转换（每个元素变形）
来源：http://rsi.zhengqikj.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uoz.cashguo.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://clh.yanxiufei.cn

JS:   arr.map(x => x * 2)
来源：http://alt.guannengcc.top

TS:   arr.map(x => x * 2)
来源：http://cat.yonumen.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://imf.dianchejie.cn

Go:   // 手写循环
来源：http://yio.cashguo.top

Ruby: arr.map { |x| x * 2 }
来源：http://nwo.bbcook.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://sjk.ctjpmb.com

[D15] 去重
来源：http://daa.xziqi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rjn.sysykeji.top

PHP:  array_unique($arr);
来源：http://vpz.guowangkeji.top

JS:   [...new Set(arr)]
来源：http://nkp.yj20258888.top


<!-- 参考信息 -->