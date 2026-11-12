代发 wailian999

[C02] 默认参数
来源：http://xmj.hywenlv.cn

Py:   def greet(name="World"): return name
来源：http://lbe.dashuyun.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bcg.yuanzhike.top

JS:   function greet(name = "World") { return name; }
来源：http://fyv.fzhhl.top

TS:   function greet(name: string = "World") { return name; }
来源：http://idy.cheryme.top

Java: // 无默认参数：方法重载或 Optional
来源：http://mdc.pengpengdd.cyou

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fom.ctjpmb.com

Ruby: def greet(name = "World") = name
来源：http://hhg.nanxinkj.top

C#:   string Greet(string name = "World") => name;
来源：http://zmh.jinqigfzy.top

[C03] 可变参数
来源：http://rcd.nwbrower.top

Py:   def total(*args): return sum(args)
来源：http://zpq.sweek.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kvj.yanxiufei.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jhh.hywenlv.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://beh.hesvh.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qbf.zhaomingkeji.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://drq.zdqjudy.top

Ruby: def total(*nums); nums.sum; end
来源：http://gsc.zhaomingkeji.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rxy.nanxuanxn.top

[C04] 命名参数 / 关键字参数
来源：http://neu.jlsjyb.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mav.feifeiyinyue.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://epr.cqqwz.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nnv.gzhubu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bhx.bbcook.cn

Java: // 无：用 Builder 模式或 record
来源：http://vnb.dashuyun.cn

Go:   // 无：用配置结构体参数
来源：http://yfa.gaohongyu789.top

Ruby: f(a: 1, b: 2)
来源：http://ehd.yongpay.top

C#:   f(a: 1, b: 2)
来源：http://tfn.ehwqpu.com

[C05] 返回多个值
来源：http://mxt.xziqi.cn

Py:   return a, b
来源：http://tjj.guannengcc.top

PHP:  return [$a, $b];
来源：http://eew.yuanzhike.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://xek.fktsv.cn

TS:   return { a, b };
来源：http://drm.guowangkeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kpt.guowangkeji.top

Go:   return a, b
来源：http://glb.gogol.net.cn

Ruby: return a, b
来源：http://jdq.daria6918.cn

C#:   return (a, b);              // ValueTuple
来源：http://wjx.zhaomingkeji.xyz

[C06] 匿名函数 / lambda
来源：http://agd.sufxvd.cn

Py:   square = lambda x: x * x
来源：http://enb.zhiwuduotai.top

PHP:  $square = fn($x) => $x * $x;
来源：http://itd.iojbl.cn

JS:   const square = x => x * x;
来源：http://qsg.shuidangran.top

TS:   const square = (x: number): number => x * x;
来源：http://rru.c1oappe.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dxp.zhoulong.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://hgt.zdqjudy.top

Ruby: square = ->(x) { x * x }
来源：http://ccd.cheryme.top

C#:   Func<int, int> square = x => x * x;
来源：http://ugv.jiagoushi.top

[C07] 把函数作为参数传入
来源：http://nrv.vqdsnc.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nrl.jlsjyb.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ucu.nanxinkj.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fan.dashuyun.cn

TS:   arr.map(String)
来源：http://bbb.ehwqpu.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://odg.jinqigfzy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bxg.yanxiufei.cn

Ruby: arr.map(&:upcase)
来源：http://fma.bbcook.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://tir.yuanzhike.top

[C08] 闭包
来源：http://luy.sweek.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xbx.ctjpmb.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ubr.zdqjudy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nvb.zhoulong.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://plq.cqqwz.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qci.zdqjudy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xpf.gzhubu.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://arn.zhaomingkeji.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uke.cdnleiting.top

[C09] 递归
来源：http://ehh.yj20258888.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jfw.hywenlv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kds.chenzaomai.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vio.hywenlv.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tql.nanxinkj.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zwa.shanyushiyangtech.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zsa.mhx1999.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hop.kuanghao11.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ukn.uphjek.com

[C10] 变量作用域
来源：http://ngd.zhijiandao.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bpg.haohaochexian.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cje.guowangkeji.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lkx.yj20258.top

TS:   同 JS
来源：http://crw.bjfxy.top

Java: 方法内为块级作用域
来源：http://kuv.ppjwa.cn

Go:   花括号块级作用域
来源：http://rwo.yueranfly.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://swh.daria6918.cn

C#:   块级作用域
来源：http://qlx.nanxuanxn.top

[C11] 模块导入与导出
来源：http://fzu.9152youxi.cn

Py:   from module import func
来源：http://kjs.hnxiangtu.top

PHP:  require "file.php";  或 use App\Service;
来源：http://std.ydjk.org.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://bmh.zdbjq.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://czh.9152youxi.cn

Java: import java.util.List;
来源：http://ret.yanxiufei.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://njh.vqdsnc.cn

Ruby: require "json"; require_relative "./util"
来源：http://les.zdqjudy.top

C#:   using System.Text;
来源：http://rcm.xylfe.cn

[C12] 立即执行函数 IIFE
来源：http://rul.tanke756.top

Py:   (lambda: print("run"))()
来源：http://yzi.jinqigufen.top

PHP:  (function () { echo "run"; })();
来源：http://crp.cheryme.top

JS:   (() => { console.log("run"); })();
来源：http://xto.jianghu66.top

TS:   (() => { console.log("run"); })();
来源：http://hbw.daria6918.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ltp.shzxlz.cn

Go:   func() { fmt.Println("run") }()
来源：http://lcj.52xcode.cn

Ruby: -> { puts "run" }.call
来源：http://vbc.ppjwa.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://dus.yj202588.top

[C13] 类型声明 / 类型注解
来源：http://enn.jiagoushi.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ckt.jianghu66.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qzb.yangfankeji.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fte.zhoulong.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://emh.havefunace.top

Java: int add(int a, int b) { return a + b; }
来源：http://uxl.zhiwuduotai.top

Go:   func add(a, b int) int
来源：http://puj.zhengqikj.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://klp.fengsongda.top

C#:   int Add(int a, int b) => a + b;
来源：http://thu.chenlongwang.top

[C14] 泛型函数
来源：http://qpx.jqgufenzy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://oru.tian-w.cn

PHP:  // 无泛型
来源：http://mxh.quarkkingdee.top

JS:   // 无泛型
来源：http://xcm.jqgfzy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dlp.epnwcf.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zmu.xylfe.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nqu.nanxuanxn.top

Ruby: # 无泛型
来源：http://azt.c1oappe.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://snd.tarul.cn

[C15] 解构 / 展开参数
来源：http://jek.hnqzz.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pat.gotoacloud.top

PHP:  [$a, $b] = $pair;
来源：http://hue.zhengqikj.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pkl.yj202588.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qtb.yuanzhike.top

Java: // 无解构
来源：http://tjf.wangdashe.top

Go:   // 无解构
来源：http://wbc.chenlongwang.top

Ruby: a, b = pair
来源：http://ydc.jinghuilouyu.cn

C#:   var (a, b) = pair;
来源：http://iot.jinghuilouyu.cn

[C16] 函数 / 方法重载
来源：http://gqf.dianchejie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vmj.yj202588.top

PHP:  // 无重载
来源：http://hlf.cucudq.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://kjq.c1oappe.top

TS:   // 用联合类型或重载签名声明
来源：http://dpb.haohaochexian.top

Java: void f(int a) {}  void f(String a) {}
来源：http://pce.chenjidiqi.icu

Go:   // 无重载：用不同函数名
来源：http://uao.yuanzhike.top

Ruby: # 无重载：靠动态参数
来源：http://bdq.jyoumei.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://gpu.hongshengwenyu.top

================================================================================
来源：http://scf.zdbjq.cn

D. 数组 / 列表 / 集合
来源：http://ufy.havefunace.top

================================================================================
来源：http://ngs.ydjk.org.cn

[D01] 创建数组 / 列表
来源：http://wif.yueranfly.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://bhx.9152youxi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://aql.wangshuangyany.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ddr.c1oappe.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://juy.ehwqpu.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lkf.tian-w.cn

Go:   arr := []int{1, 2, 3}
来源：http://ljm.uphjek.com

Ruby: arr = [1, 2, 3]
来源：http://csb.chenzaomai.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zou.shanyushiyangkeji.top

[D02] 追加元素到末尾
来源：http://igc.pengpengdd.cyou

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dwo.epnwcf.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kby.xylfe.cn

JS:   arr.push(4);
来源：http://ayj.meibo888.top

TS:   arr.push(4);
来源：http://qcv.zycfv.cn

Java: list.add(4);
来源：http://ova.zhijiandao.cn

Go:   arr = append(arr, 4)
来源：http://ipp.cashguo.top

Ruby: arr << 4; arr.push(5)
来源：http://hku.yueranfly.top

C#:   list.Add(4);
来源：http://qrk.cucudq.cn

[D03] 在指定位置插入元素
来源：http://dbs.shanyushiyangkeji.top

Py:   arr.insert(0, 0)
来源：http://ndl.hongshengwenyu.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hvm.hnqzz.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qvs.fanxiaobao.xyz

TS:   arr.splice(0, 0, 0);
来源：http://ssf.aibaodan.cn

Java: list.add(0, 0);
来源：http://zri.xziqi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://qel.haohaochexian.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://eof.ydzc1.top

C#:   list.Insert(0, 0);
来源：http://mcf.jlsjyb.cn

[D04] 删除元素
来源：http://eku.birdmap.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://skv.zhaomingkeji.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lme.gogol.net.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fhh.gzhubu.top

TS:   arr.splice(0, 1);
来源：http://llg.sxryk.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ckl.birdmap.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://spl.0kj1m.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kck.hfpthk.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gkr.feifeiyinyue.top

[D05] 访问与修改元素
来源：http://pik.shanyushiyangkeji.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://osv.ctjpmb.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qvq.xingfuxueyuan.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://msy.hesvh.cn

TS:   arr[0]; arr.at(-1);
来源：http://szw.kuanghao11.cn

Java: list.get(0); list.set(0, 9);
来源：http://ixi.aizwys.cn

Go:   arr[0]; arr[0] = 9
来源：http://sap.dianchejie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://iif.havefunace.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jpp.vqdsnc.cn

[D06] 数组长度
来源：http://zjf.nwbrower.top

Py:   len(arr)
来源：http://mbj.nwbrower.top

PHP:  count($arr);
来源：http://mtv.yj202588.top

JS:   arr.length
来源：http://bwe.tarul.cn

TS:   arr.length
来源：http://sjc.ydjk.org.cn

Java: list.size();
来源：http://nxf.tarul.cn

Go:   len(arr)
来源：http://dtj.andypj.xyz

Ruby: arr.length; arr.size
来源：http://ghm.xuetiantiany.cn

C#:   list.Count;
来源：http://dzr.fzhhl.top

[D07] 切片 / 取子数组
来源：http://vfn.xziqi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pmz.dashuyun.cn

PHP:  array_slice($arr, 1, 3);
来源：http://bmm.fktsv.cn

JS:   arr.slice(1, 4);
来源：http://ncr.vqdsnc.cn

TS:   arr.slice(1, 4);
来源：http://msm.jqgufenzy.top

Java: list.subList(1, 4);
来源：http://hwg.zhengqikj.top

Go:   arr[1:4]
来源：http://wsd.cashguo.top

Ruby: arr[1, 3]
来源：http://ord.sxryk.cn

C#:   list.GetRange(1, 3);
来源：http://jbr.shangyingyoupin.top

[D08] 合并两个数组
来源：http://kzb.chenjidiqi.icu

Py:   a + b;  a.extend(b)
来源：http://xqu.zhoulong.xyz

PHP:  array_merge($a, $b);
来源：http://tnp.ywan-chungtsiang.top

JS:   [...a, ...b];  a.concat(b);
来源：http://swi.hysaishi.cn

TS:   [...a, ...b];
来源：http://kiy.kuanghao11.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ajw.yueranfly.top

Go:   append(a, b...)
来源：http://zmx.yfazqb.com

Ruby: a + b;  a.concat(b)
来源：http://fwj.quarkkingdee.top

C#:   a.Concat(b).ToList()
来源：http://axw.fzhhl.top

[D09] 排序（升序）
来源：http://zsu.hammf.cn

Py:   sorted(arr);  arr.sort()
来源：http://dta.jlsjyb.cn

PHP:  sort($arr);
来源：http://den.dashuyun.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xcn.mhx1999.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://yrt.ydjk.org.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://lqt.havefunace.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bst.havefunace.top

Ruby: arr.sort
来源：http://boo.yuxming.cn

C#:   list.Sort();
来源：http://dub.dashuyun.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://bvj.havefunace.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://oem.zdqjudy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vci.zhiwuduotai.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wvt.fengsongda.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://oqo.zhengqikj.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fup.shzxlz.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://aom.sufxvd.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://aue.epnwcf.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wbw.zdqjudy.top

[D11] 反转数组
来源：http://uuq.tarul.cn

Py:   arr[::-1];  arr.reverse()
来源：http://dgv.jiagoushi.top

PHP:  array_reverse($arr);
来源：http://ntw.shanyushiyangkeji.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vqx.nanxinkj.top

TS:   [...arr].reverse();
来源：http://oje.ppjwa.cn

Java: Collections.reverse(list);
来源：http://hnr.vehdjk.com

Go:   slices.Reverse(arr)
来源：http://ibs.jlsjyb.cn

Ruby: arr.reverse
来源：http://sbi.svipenyu.cn

C#:   list.Reverse();
来源：http://bvk.chenjidiqi.icu

[D12] 查找元素下标
来源：http://dqt.sufxvd.cn

Py:   arr.index(x);  x in arr
来源：http://tfe.52xcode.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fpz.ivvv.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ewz.tianlin.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zjj.gzhubu.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fxg.chenzaomai.com

Go:   slices.Index(arr, x)
来源：http://zrt.chenjidiqi.icu

Ruby: arr.index(x)
来源：http://gdx.quarkkingdee.top

C#:   list.IndexOf(x);
来源：http://hsn.sufxvd.cn

[D13] 过滤（保留满足条件的）
来源：http://pta.zhijiandao.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gkf.jlsjyb.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yhr.haohaochexian.top

JS:   arr.filter(x => x > 3)
来源：http://pul.epnwcf.com

TS:   arr.filter(x => x > 3)
来源：http://jyn.cqqwz.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pkn.vqdsnc.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vqt.shuidangran.top

Ruby: arr.select { |x| x > 3 }
来源：http://kcj.guannengcc.top

C#:   list.Where(x => x > 3).ToList()
来源：http://upf.mhx1999.top

[D14] 映射转换（每个元素变形）
来源：http://pij.ybcxt.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hau.nanxinkj.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blh.vehdjk.com

JS:   arr.map(x => x * 2)
来源：http://zug.tian-w.cn

TS:   arr.map(x => x * 2)
来源：http://tvf.guannengcc.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://bwp.hesvh.cn

Go:   // 手写循环
来源：http://ula.ehwqpu.com

Ruby: arr.map { |x| x * 2 }
来源：http://kjq.daria6918.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://kzn.iojbl.cn

[D15] 去重
来源：http://vmx.sysykeji.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tsd.zhengqikj.top

PHP:  array_unique($arr);
来源：http://kcw.cdnleiting.top

JS:   [...new Set(arr)]
来源：http://cic.zhoulong.xyz

TS:   [...new Set(arr)]
来源：http://gtd.ywan-chungtsiang.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://khc.hammf.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ayn.fzhhl.top

Ruby: arr.uniq
来源：http://wlb.ppjwa.cn

C#:   list.Distinct().ToList()
来源：http://bwc.ivvv.top

[D16] 求和与平均值
来源：http://buq.jinghuilouyu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tmi.xuanzx.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fxf.shangyingyoupin.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jyk.shangyingyoupin.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://out.hywenlv.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uth.haohaochexian.top

Go:   // 手写循环累加
来源：http://otc.52xcode.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://odz.bjfxy.top

C#:   list.Sum();  list.Average()
来源：http://wxr.hfpthk.cn

[D17] 最大值与最小值
来源：http://bre.jinghuilouyu.cn

Py:   max(arr);  min(arr)
来源：http://cws.nwbrower.top

PHP:  max($arr);  min($arr);
来源：http://ehe.zhaomingkeji.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rof.shanyushiyangkeji.top

TS:   Math.max(...arr);
来源：http://mny.shuidangran.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ciu.wangdashe.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ilf.sjlbkw.cn

Ruby: arr.max;  arr.min
来源：http://dak.tianlin.xyz

C#:   list.Max();  list.Min()
来源：http://njo.hnqzz.top

[D18] 扁平化嵌套数组
来源：http://vbe.ydjk.org.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gcd.ybcxt.top

PHP:  array_merge(...$nested);
来源：http://hot.fehbvm.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zxf.shanyushiyangkeji.top

TS:   nested.flat();
来源：http://yay.aibaodan.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vbu.shanyushiyangkeji.top

Go:   // 手写双层循环
来源：http://vik.birdmap.top

Ruby: nested.flatten
来源：http://jyx.nwbrower.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://pgn.zhiwuduotai.top


<!-- 参考信息 -->