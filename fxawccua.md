代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kay.yonumen.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tee.feifeiyinyue.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tbb.tianlin.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zqh.sweek.top

Ruby: def total(*nums); nums.sum; end
来源：http://gxy.jinqigufen.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hmo.shanyushiyangtech.top

[C04] 命名参数 / 关键字参数
来源：http://xju.shangyingyoupin.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pyv.jinyuanbaomall.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://avp.sufxvd.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ckm.nwbrower.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://omb.hysaishi.cn

Java: // 无：用 Builder 模式或 record
来源：http://ozh.jqgfzy.top

Go:   // 无：用配置结构体参数
来源：http://mil.hysaishi.cn

Ruby: f(a: 1, b: 2)
来源：http://qrl.zhijiandao.cn

C#:   f(a: 1, b: 2)
来源：http://eyt.bjfxy.top

[C05] 返回多个值
来源：http://eab.jinyuanbaomall.cn

Py:   return a, b
来源：http://ikl.hfpthk.cn

PHP:  return [$a, $b];
来源：http://csp.yfazqb.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://gpa.aizwys.cn

TS:   return { a, b };
来源：http://ubx.guannengcc.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dru.daria6918.cn

Go:   return a, b
来源：http://gyj.tianlin.xyz

Ruby: return a, b
来源：http://kfg.redwolf501.top

C#:   return (a, b);              // ValueTuple
来源：http://xul.hongshengwenyu.top

[C06] 匿名函数 / lambda
来源：http://nbl.jianghu66.top

Py:   square = lambda x: x * x
来源：http://sjw.ivvv.top

PHP:  $square = fn($x) => $x * $x;
来源：http://cvy.ppjwa.cn

JS:   const square = x => x * x;
来源：http://kts.mhx1999.top

TS:   const square = (x: number): number => x * x;
来源：http://vax.zycfv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://chd.hfpthk.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ntd.haohaochexian.top

Ruby: square = ->(x) { x * x }
来源：http://mpi.pycfn.com

C#:   Func<int, int> square = x => x * x;
来源：http://jdf.jlsjyb.cn

[C07] 把函数作为参数传入
来源：http://lts.tarul.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rrv.vqdsnc.cn

PHP:  array_map("strtoupper", $arr);
来源：http://qpd.vqdsnc.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vhz.yj202588.top

TS:   arr.map(String)
来源：http://olw.zhiwuduotai.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rjj.shzxlz.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lux.sjlbkw.cn

Ruby: arr.map(&:upcase)
来源：http://hus.jianghu66.top

C#:   arr.Select(s => s.ToUpper())
来源：http://zrp.316326.xyz

[C08] 闭包
来源：http://mrb.tian-w.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kca.wangshuangyany.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wol.zhaomingkeji.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qxx.yueranfly.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ive.epnwcf.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://orr.daxiang520.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://uad.9152youxi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://atn.xingfuxueyuan.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://teq.meibo888.top

[C09] 递归
来源：http://nrz.zdqjudy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bdd.vqdsnc.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rtb.zhoulong.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wbx.andypj.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nzm.pycfn.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fij.gaohongyu789.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cib.yueranfly.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wmt.tianlin.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qlo.ywan-chungtsiang.top

[C10] 变量作用域
来源：http://nbp.gogol.net.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ity.smart0.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gpl.guowangkeji.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mpy.birdmap.top

TS:   同 JS
来源：http://iez.cdnleiting.top

Java: 方法内为块级作用域
来源：http://vjj.yj20258888.top

Go:   花括号块级作用域
来源：http://cpe.jiagoushi.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uab.vqdsnc.cn

C#:   块级作用域
来源：http://zmi.wangshuangyany.cn

[C11] 模块导入与导出
来源：http://zze.redwolf501.top

Py:   from module import func
来源：http://wcf.mhx1999.top

PHP:  require "file.php";  或 use App\Service;
来源：http://cjq.c1oappe.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://koz.wangdashe.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nlo.yuanzhike.top

Java: import java.util.List;
来源：http://efm.shanyushiyangkeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wyx.fzhhl.top

Ruby: require "json"; require_relative "./util"
来源：http://oha.ywan-chungtsiang.top

C#:   using System.Text;
来源：http://qvq.zhiwuduotai.top

[C12] 立即执行函数 IIFE
来源：http://hty.hongshengwenyu.top

Py:   (lambda: print("run"))()
来源：http://ced.cqqwz.cn

PHP:  (function () { echo "run"; })();
来源：http://cif.snrcjt.cn

JS:   (() => { console.log("run"); })();
来源：http://ixn.mhx1999.top

TS:   (() => { console.log("run"); })();
来源：http://xrj.sufxvd.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nvb.guowangkeji.top

Go:   func() { fmt.Println("run") }()
来源：http://xcy.tanke756.top

Ruby: -> { puts "run" }.call
来源：http://wnc.zdbjq.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://knp.daria6918.cn

[C13] 类型声明 / 类型注解
来源：http://yly.wangshuangyany.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://btd.zhongyouzk.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wyv.cdnleiting.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://udo.cqqwz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ibz.jqgufenzy.top

Java: int add(int a, int b) { return a + b; }
来源：http://hch.ctjpmb.com

Go:   func add(a, b int) int
来源：http://hls.ybcxt.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tun.ivvv.top

C#:   int Add(int a, int b) => a + b;
来源：http://tln.yangfankeji.com

[C14] 泛型函数
来源：http://pxb.jianghu66.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rdy.tianlin.xyz

PHP:  // 无泛型
来源：http://wfa.jlsjyb.cn

JS:   // 无泛型
来源：http://ugt.yuxming.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vou.aizwys.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cdu.zhoulong.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zlx.tianlin.xyz

Ruby: # 无泛型
来源：http://wsz.hesvh.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ood.xziqi.cn

[C15] 解构 / 展开参数
来源：http://ado.hywenlv.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mzp.jlsjyb.cn

PHP:  [$a, $b] = $pair;
来源：http://dmd.nanxuanxn.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tvb.bbcook.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zlk.sweek.top

Java: // 无解构
来源：http://rzr.jyoumei.cn

Go:   // 无解构
来源：http://oyo.nanxuanxn.top

Ruby: a, b = pair
来源：http://czs.zhongyouzk.top

C#:   var (a, b) = pair;
来源：http://exo.yuanzhike.top

[C16] 函数 / 方法重载
来源：http://gfv.vqdsnc.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://afx.uphjek.com

PHP:  // 无重载
来源：http://tha.smart0.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://atc.dianchejie.cn

TS:   // 用联合类型或重载签名声明
来源：http://cge.shzxlz.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://agi.gzhubu.top

Go:   // 无重载：用不同函数名
来源：http://nvu.meibo888.top

Ruby: # 无重载：靠动态参数
来源：http://mlf.yj202588.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://cqx.birdmap.top

================================================================================
来源：http://nxw.nwbrower.top

D. 数组 / 列表 / 集合
来源：http://lso.quarkkingdee.top

================================================================================
来源：http://yxj.mhx1999.top

[D01] 创建数组 / 列表
来源：http://ysf.pengpengdd.cyou

Py:   arr = [1, 2, 3];  empty = []
来源：http://ysd.iojbl.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xyq.gotoacloud.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zpd.fktsv.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ody.yj20258.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ebc.yj20258.top

Go:   arr := []int{1, 2, 3}
来源：http://yqt.xingfuxueyuan.xyz

Ruby: arr = [1, 2, 3]
来源：http://zrz.xinyue.icu

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://sra.kuanghao11.cn

[D02] 追加元素到末尾
来源：http://fld.jinghuilouyu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fme.xingfuxueyuan.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vkc.yangfankeji.com

JS:   arr.push(4);
来源：http://tku.hywenlv.cn

TS:   arr.push(4);
来源：http://tfs.yfazqb.com

Java: list.add(4);
来源：http://flb.hongshengwenyu.top

Go:   arr = append(arr, 4)
来源：http://oqc.yuxming.cn

Ruby: arr << 4; arr.push(5)
来源：http://pej.daxiang520.top

C#:   list.Add(4);
来源：http://sxi.svipenyu.cn

[D03] 在指定位置插入元素
来源：http://pfr.ywan-chungtsiang.top

Py:   arr.insert(0, 0)
来源：http://zng.uphjek.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://irr.chenjidiqi.icu

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://irg.yangfankeji.com

TS:   arr.splice(0, 0, 0);
来源：http://zvy.hnxiangtu.top

Java: list.add(0, 0);
来源：http://qwq.yonumen.top

Go:   arr = append([]int{0}, arr...)
来源：http://tte.shanyushiyangtech.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jtb.uphjek.com

C#:   list.Insert(0, 0);
来源：http://oxe.dashuyun.cn

[D04] 删除元素
来源：http://xaq.cdnleiting.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gxp.ehwqpu.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gib.daria6918.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rjt.nanxuanxn.top

TS:   arr.splice(0, 1);
来源：http://kzb.hnxiangtu.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gpr.zhijiandao.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://szw.hesvh.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hld.cheryme.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qlt.xylfe.cn

[D05] 访问与修改元素
来源：http://fac.ivvv.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ior.dianchejie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lwn.jqgufenzy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hxj.chenzaomai.com

TS:   arr[0]; arr.at(-1);
来源：http://bss.dianchejie.cn

Java: list.get(0); list.set(0, 9);
来源：http://jyp.xuanzx.com

Go:   arr[0]; arr[0] = 9
来源：http://kqs.shanyushiyangtech.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://acn.dashuyun.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://shs.guannengcc.top

[D06] 数组长度
来源：http://psl.sweek.top

Py:   len(arr)
来源：http://vrh.tianlin.xyz

PHP:  count($arr);
来源：http://hrz.kuanghao11.cn

JS:   arr.length
来源：http://ivn.hcnkem.com

TS:   arr.length
来源：http://uzs.fzhhl.top

Java: list.size();
来源：http://dzi.nanxuanxn.top

Go:   len(arr)
来源：http://mea.hammf.cn

Ruby: arr.length; arr.size
来源：http://aud.shzxlz.cn

C#:   list.Count;
来源：http://csl.ywan-chungtsiang.top

[D07] 切片 / 取子数组
来源：http://ine.jinyuanbaomall.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://poz.fanxiaobao.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://pvo.feifeiyinyue.top

JS:   arr.slice(1, 4);
来源：http://gng.xuanzx.com

TS:   arr.slice(1, 4);
来源：http://qtp.sweek.top

Java: list.subList(1, 4);
来源：http://yrz.ybcxt.top

Go:   arr[1:4]
来源：http://for.c1oappe.top

Ruby: arr[1, 3]
来源：http://upe.gogol.net.cn

C#:   list.GetRange(1, 3);
来源：http://edj.gaohongyu789.top

[D08] 合并两个数组
来源：http://cvd.gzhubu.top

Py:   a + b;  a.extend(b)
来源：http://plc.redwolf501.top

PHP:  array_merge($a, $b);
来源：http://jmw.zhaomingkeji.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://doc.jinqigufen.top

TS:   [...a, ...b];
来源：http://iid.tarul.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tds.hywenlv.cn

Go:   append(a, b...)
来源：http://zhy.hysaishi.cn

Ruby: a + b;  a.concat(b)
来源：http://snk.ehwqpu.com

C#:   a.Concat(b).ToList()
来源：http://qtj.daxiang520.top

[D09] 排序（升序）
来源：http://cjj.yuanzhike.top

Py:   sorted(arr);  arr.sort()
来源：http://xlb.52xcode.cn

PHP:  sort($arr);
来源：http://cte.aibaodan.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vtp.andypj.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://nqe.zhixingplan.top

Java: Collections.sort(list);  list.sort(null);
来源：http://agd.zdbjq.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://npe.gotoacloud.top

Ruby: arr.sort
来源：http://bhx.hfpthk.cn

C#:   list.Sort();
来源：http://equ.guannengcc.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://sca.c1oappe.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nxt.jqgufenzy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rxx.jiagoushi.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://uaf.quarkkingdee.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://elt.shuidangran.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mgp.jiagoushi.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vae.hammf.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://izk.tian-w.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://iso.gaohongyu789.top

[D11] 反转数组
来源：http://bpk.bbcook.cn

Py:   arr[::-1];  arr.reverse()
来源：http://uow.jlsjyb.cn

PHP:  array_reverse($arr);
来源：http://blv.zhoulong.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bnk.fehbvm.com

TS:   [...arr].reverse();
来源：http://obr.xuanzx.com

Java: Collections.reverse(list);
来源：http://rvk.jinqigufen.top

Go:   slices.Reverse(arr)
来源：http://jyc.chenzaomai.com

Ruby: arr.reverse
来源：http://zkm.yj202588.top

C#:   list.Reverse();
来源：http://diu.fktsv.cn

[D12] 查找元素下标
来源：http://wee.quarkkingdee.top

Py:   arr.index(x);  x in arr
来源：http://mfi.yongpay.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xmo.andypj.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ezk.tian-w.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hhx.gotoacloud.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cfj.hesvh.cn

Go:   slices.Index(arr, x)
来源：http://jas.zhengqikj.top

Ruby: arr.index(x)
来源：http://wcz.quarkkingdee.top

C#:   list.IndexOf(x);
来源：http://xyv.yonumen.top

[D13] 过滤（保留满足条件的）
来源：http://kcr.52xcode.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qpk.0kj1m.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tpn.fktsv.cn

JS:   arr.filter(x => x > 3)
来源：http://qas.yueranfly.top

TS:   arr.filter(x => x > 3)
来源：http://bbt.c1oappe.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ahl.yj202588.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tpa.hcnkem.com

Ruby: arr.select { |x| x > 3 }
来源：http://mwi.chenjidiqi.icu

C#:   list.Where(x => x > 3).ToList()
来源：http://yij.yongpay.top

[D14] 映射转换（每个元素变形）
来源：http://clh.aizwys.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uxt.jinqigfzy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://opu.hammf.cn

JS:   arr.map(x => x * 2)
来源：http://jgx.c1oappe.top

TS:   arr.map(x => x * 2)
来源：http://fok.guannengcc.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://xze.ppjwa.cn

Go:   // 手写循环
来源：http://irk.gzhubu.top

Ruby: arr.map { |x| x * 2 }
来源：http://ouq.bjfxy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://cfy.ehwqpu.com

[D15] 去重
来源：http://vde.nanxuanxn.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xhe.cdnleiting.top

PHP:  array_unique($arr);
来源：http://kpx.jinghuilouyu.cn

JS:   [...new Set(arr)]
来源：http://jok.chenjidiqi.icu

TS:   [...new Set(arr)]
来源：http://rjb.yuxming.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://haq.shangyingyoupin.top

Go:   // 用 map[T]struct{} 手写
来源：http://vrn.hysaishi.cn

Ruby: arr.uniq
来源：http://rrc.yueranfly.top

C#:   list.Distinct().ToList()
来源：http://xsx.yj20258.top

[D16] 求和与平均值
来源：http://mhh.daria6918.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://oeu.aizwys.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://imk.havefunace.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jne.fzhhl.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ilz.cqqwz.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ihw.bjfxy.top

Go:   // 手写循环累加
来源：http://fkz.chenzaomai.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yjl.zhixingplan.top

C#:   list.Sum();  list.Average()
来源：http://tzg.zdbjq.cn

[D17] 最大值与最小值
来源：http://ony.yanxiufei.cn

Py:   max(arr);  min(arr)
来源：http://uwn.yueranfly.top

PHP:  max($arr);  min($arr);
来源：http://hae.chenzaomai.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cez.xuanzx.com

TS:   Math.max(...arr);
来源：http://gpz.xingfuxueyuan.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://ols.guannengcc.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://adz.bbcook.cn

Ruby: arr.max;  arr.min
来源：http://dsh.fehbvm.com

C#:   list.Max();  list.Min()
来源：http://vfz.ywan-chungtsiang.top

[D18] 扁平化嵌套数组
来源：http://pik.yongpay.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ibf.gaohongyu789.top

PHP:  array_merge(...$nested);
来源：http://tda.316326.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gul.vehdjk.com

TS:   nested.flat();
来源：http://ioc.ivvv.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xib.gaohongyu789.top

Go:   // 手写双层循环
来源：http://pbs.uphjek.com

Ruby: nested.flatten
来源：http://vbf.ctjpmb.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://gcq.ywan-chungtsiang.top

[D19] 按字段分组
来源：http://uio.guannengcc.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ihh.fanxiaobao.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gqo.chenzaomai.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pak.hnqzz.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://qzu.zhongyouzk.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wgh.pengpengdd.cyou

Go:   // 手写 map[string][]T
来源：http://uwr.shanyushiyangkeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://voi.gaohongyu789.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ptn.quarkkingdee.top

[D20] 统计每个元素出现次数
来源：http://lwu.aizwys.cn

Py:   Counter(arr)
来源：http://bqv.xuetiantiany.cn

PHP:  array_count_values($arr);
来源：http://rco.redwolf501.top


<!-- 参考信息 -->