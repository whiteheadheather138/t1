代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bne.cqqwz.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vqx.zhijiandao.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ind.haohaochexian.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qbn.hesvh.cn

Ruby: def total(*nums); nums.sum; end
来源：http://sdb.gotoacloud.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dtx.tianlin.xyz

[C04] 命名参数 / 关键字参数
来源：http://kpr.birdmap.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ryw.birdmap.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nlb.fehbvm.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mby.bjfxy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zaz.ybcxt.top

Java: // 无：用 Builder 模式或 record
来源：http://uhw.ctjpmb.com

Go:   // 无：用配置结构体参数
来源：http://hnw.mhx1999.top

Ruby: f(a: 1, b: 2)
来源：http://jdn.aibaodan.cn

C#:   f(a: 1, b: 2)
来源：http://pgt.xingfuxueyuan.xyz

[C05] 返回多个值
来源：http://hea.jyoumei.cn

Py:   return a, b
来源：http://sva.sjlbkw.cn

PHP:  return [$a, $b];
来源：http://kzd.quarkkingdee.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://byj.ywan-chungtsiang.top

TS:   return { a, b };
来源：http://xsj.dianchejie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fbt.chenlongwang.top

Go:   return a, b
来源：http://wnl.redwolf501.top

Ruby: return a, b
来源：http://fde.ydzc1.top

C#:   return (a, b);              // ValueTuple
来源：http://qph.ppjwa.cn

[C06] 匿名函数 / lambda
来源：http://ewb.yfazqb.com

Py:   square = lambda x: x * x
来源：http://wwi.zhijiandao.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://zrk.sjlbkw.cn

JS:   const square = x => x * x;
来源：http://czo.jqgufenzy.top

TS:   const square = (x: number): number => x * x;
来源：http://ajh.cashguo.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dkk.hnxiangtu.top

Go:   sq := func(x int) int { return x * x }
来源：http://pvx.shzxlz.cn

Ruby: square = ->(x) { x * x }
来源：http://lfo.jinqigfzy.top

C#:   Func<int, int> square = x => x * x;
来源：http://lbs.yueranfly.top

[C07] 把函数作为参数传入
来源：http://amu.pycfn.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sqk.daria6918.cn

PHP:  array_map("strtoupper", $arr);
来源：http://rnb.yangfankeji.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hie.zhaomingkeji.xyz

TS:   arr.map(String)
来源：http://iqi.yuanzhike.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kbc.sjlbkw.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://aph.shanyushiyangtech.top

Ruby: arr.map(&:upcase)
来源：http://xzt.shanyushiyangkeji.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ihk.jqgufenzy.top

[C08] 闭包
来源：http://sam.xinyue.icu

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://iib.pycfn.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xxb.andypj.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cgx.zhaomingkeji.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pzb.sweek.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ist.fanxiaobao.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jfq.xuanzx.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ciu.tarul.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ctt.hfpthk.cn

[C09] 递归
来源：http://jkj.zhixingplan.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://raw.c1oappe.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jew.zhiwuduotai.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pjb.hnxiangtu.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fnz.ppjwa.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wup.redwolf501.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sxp.jyoumei.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://sbe.jinyuanbaomall.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sqz.hywenlv.cn

[C10] 变量作用域
来源：http://gae.cdnleiting.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jec.nanxinkj.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fim.xylfe.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dan.ydjk.org.cn

TS:   同 JS
来源：http://cjp.uphjek.com

Java: 方法内为块级作用域
来源：http://hfx.pycfn.com

Go:   花括号块级作用域
来源：http://pna.yueranfly.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tjj.316326.xyz

C#:   块级作用域
来源：http://dfd.jinqigfzy.top

[C11] 模块导入与导出
来源：http://uvw.yj202588.top

Py:   from module import func
来源：http://xam.ybcxt.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ixy.ehwqpu.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://prg.c1oappe.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://inl.ctjpmb.com

Java: import java.util.List;
来源：http://jgh.tianlin.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://llx.jinqigufen.top

Ruby: require "json"; require_relative "./util"
来源：http://zzo.jlsjyb.cn

C#:   using System.Text;
来源：http://mbo.jinqigufen.top

[C12] 立即执行函数 IIFE
来源：http://ybg.jinghuilouyu.cn

Py:   (lambda: print("run"))()
来源：http://ojy.svipenyu.cn

PHP:  (function () { echo "run"; })();
来源：http://xys.nanxuanxn.top

JS:   (() => { console.log("run"); })();
来源：http://bts.hfpthk.cn

TS:   (() => { console.log("run"); })();
来源：http://zus.jinghuilouyu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fuh.hfpthk.cn

Go:   func() { fmt.Println("run") }()
来源：http://bek.ybcxt.top

Ruby: -> { puts "run" }.call
来源：http://aox.tianlin.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://joz.tanke756.top

[C13] 类型声明 / 类型注解
来源：http://eaj.bjfxy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zwn.hesvh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jxx.wangdashe.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ouv.snrcjt.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yba.iojbl.cn

Java: int add(int a, int b) { return a + b; }
来源：http://yqq.wangshuangyany.cn

Go:   func add(a, b int) int
来源：http://iam.tanke756.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cyn.aizwys.cn

C#:   int Add(int a, int b) => a + b;
来源：http://eag.hammf.cn

[C14] 泛型函数
来源：http://jqx.meibo888.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wlw.fengsongda.top

PHP:  // 无泛型
来源：http://mzs.zhiwuduotai.top

JS:   // 无泛型
来源：http://hku.cdnleiting.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cag.ppjwa.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sge.ivvv.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nmm.zdqjudy.top

Ruby: # 无泛型
来源：http://nny.jinghuilouyu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fbq.hywenlv.cn

[C15] 解构 / 展开参数
来源：http://hjt.iojbl.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vpc.xziqi.cn

PHP:  [$a, $b] = $pair;
来源：http://xmq.tian-w.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pgl.shanyushiyangtech.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vth.cqqwz.cn

Java: // 无解构
来源：http://isn.smart0.xyz

Go:   // 无解构
来源：http://fdz.hesvh.cn

Ruby: a, b = pair
来源：http://vmd.jiagoushi.top

C#:   var (a, b) = pair;
来源：http://fnh.jinyuanbaomall.cn

[C16] 函数 / 方法重载
来源：http://fby.wangshuangyany.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rfo.meibo888.top

PHP:  // 无重载
来源：http://ibw.yj20258888.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://icg.shangyingyoupin.top

TS:   // 用联合类型或重载签名声明
来源：http://iyi.zhiwuduotai.top

Java: void f(int a) {}  void f(String a) {}
来源：http://mgz.shanyushiyangtech.top

Go:   // 无重载：用不同函数名
来源：http://wvk.uphjek.com

Ruby: # 无重载：靠动态参数
来源：http://kzw.chenjidiqi.icu

C#:   void F(int a) {}  void F(string a) {}
来源：http://msu.tarul.cn

================================================================================
来源：http://qgt.wangshuangyany.cn

D. 数组 / 列表 / 集合
来源：http://qgw.ydjk.org.cn

================================================================================
来源：http://ofm.yj20258.top

[D01] 创建数组 / 列表
来源：http://dhh.jinqigufen.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://yus.jinghuilouyu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vst.tanke756.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gsa.ppjwa.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://tfg.wangshuangyany.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gvx.kuanghao11.cn

Go:   arr := []int{1, 2, 3}
来源：http://mdx.hnxiangtu.top

Ruby: arr = [1, 2, 3]
来源：http://ufd.zhiwuduotai.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://uld.ydzc1.top

[D02] 追加元素到末尾
来源：http://ahj.bjfxy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kpd.haohaochexian.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yfg.snrcjt.cn

JS:   arr.push(4);
来源：http://xzb.meibo888.top

TS:   arr.push(4);
来源：http://jeh.yanxiufei.cn

Java: list.add(4);
来源：http://jfr.kuanghao11.cn

Go:   arr = append(arr, 4)
来源：http://muo.shuidangran.top

Ruby: arr << 4; arr.push(5)
来源：http://pqw.gogol.net.cn

C#:   list.Add(4);
来源：http://xdm.bbcook.cn

[D03] 在指定位置插入元素
来源：http://znl.cdnleiting.top

Py:   arr.insert(0, 0)
来源：http://val.yongpay.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lqr.jiagoushi.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://usi.epnwcf.com

TS:   arr.splice(0, 0, 0);
来源：http://jac.guannengcc.top

Java: list.add(0, 0);
来源：http://wji.hammf.cn

Go:   arr = append([]int{0}, arr...)
来源：http://myy.cqqwz.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qbv.ppjwa.cn

C#:   list.Insert(0, 0);
来源：http://mvw.xziqi.cn

[D04] 删除元素
来源：http://glj.ehwqpu.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wrh.316326.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mys.sysykeji.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://exu.gzhubu.top

TS:   arr.splice(0, 1);
来源：http://lhr.zhiwuduotai.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gjb.gzhubu.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fix.aibaodan.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kni.hongshengwenyu.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sya.ydzc1.top

[D05] 访问与修改元素
来源：http://gyk.jinqigufen.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lnu.iojbl.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vsj.aizwys.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jhn.fanxiaobao.xyz

TS:   arr[0]; arr.at(-1);
来源：http://wdf.xziqi.cn

Java: list.get(0); list.set(0, 9);
来源：http://jdl.ybcxt.top

Go:   arr[0]; arr[0] = 9
来源：http://dpl.ppjwa.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ewm.yj20258.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mff.guannengcc.top

[D06] 数组长度
来源：http://igg.smart0.xyz

Py:   len(arr)
来源：http://fch.shangyingyoupin.top

PHP:  count($arr);
来源：http://jhf.cheryme.top

JS:   arr.length
来源：http://lcp.shzxlz.cn

TS:   arr.length
来源：http://gqs.ydzc1.top

Java: list.size();
来源：http://yqj.haohaochexian.top

Go:   len(arr)
来源：http://pyl.zycfv.cn

Ruby: arr.length; arr.size
来源：http://eyg.sxryk.cn

C#:   list.Count;
来源：http://qqz.zdbjq.cn

[D07] 切片 / 取子数组
来源：http://awx.kuanghao11.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xpg.shanyushiyangkeji.top

PHP:  array_slice($arr, 1, 3);
来源：http://wwl.c1oappe.top

JS:   arr.slice(1, 4);
来源：http://tpf.cashguo.top

TS:   arr.slice(1, 4);
来源：http://gwx.dashuyun.cn

Java: list.subList(1, 4);
来源：http://dfe.chenlongwang.top

Go:   arr[1:4]
来源：http://jpv.ywan-chungtsiang.top

Ruby: arr[1, 3]
来源：http://bmv.cashguo.top

C#:   list.GetRange(1, 3);
来源：http://giu.ehwqpu.com

[D08] 合并两个数组
来源：http://yvr.yangfankeji.com

Py:   a + b;  a.extend(b)
来源：http://ahq.xingfuxueyuan.xyz

PHP:  array_merge($a, $b);
来源：http://nww.yj202588.top

JS:   [...a, ...b];  a.concat(b);
来源：http://tap.yj202588.top

TS:   [...a, ...b];
来源：http://kfk.zdbjq.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xrr.jianghu66.top

Go:   append(a, b...)
来源：http://xpw.jlsjyb.cn

Ruby: a + b;  a.concat(b)
来源：http://six.zhengqikj.top

C#:   a.Concat(b).ToList()
来源：http://yxr.ywan-chungtsiang.top

[D09] 排序（升序）
来源：http://vma.sjlbkw.cn

Py:   sorted(arr);  arr.sort()
来源：http://ejz.jyoumei.cn

PHP:  sort($arr);
来源：http://jge.snrcjt.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jvs.daxiang520.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://bnc.gotoacloud.top

Java: Collections.sort(list);  list.sort(null);
来源：http://aoa.zhengqikj.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://les.yj202588.top

Ruby: arr.sort
来源：http://ewq.wangdashe.top

C#:   list.Sort();
来源：http://wbb.daxiang520.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://akz.chenjidiqi.icu

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fht.chenjidiqi.icu

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ute.xziqi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ctl.yj202588.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xdu.zhongyouzk.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hvc.jinyuanbaomall.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ggc.nanxinkj.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://obc.ehwqpu.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dan.yueranfly.top

[D11] 反转数组
来源：http://qvp.zdqjudy.top

Py:   arr[::-1];  arr.reverse()
来源：http://ztq.zhaomingkeji.xyz

PHP:  array_reverse($arr);
来源：http://cmo.bjfxy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://del.chenjidiqi.icu

TS:   [...arr].reverse();
来源：http://epz.hcnkem.com

Java: Collections.reverse(list);
来源：http://iuz.xuetiantiany.cn

Go:   slices.Reverse(arr)
来源：http://gcy.redwolf501.top

Ruby: arr.reverse
来源：http://pye.shanyushiyangkeji.top

C#:   list.Reverse();
来源：http://sca.xingfuxueyuan.xyz

[D12] 查找元素下标
来源：http://pek.andypj.xyz

Py:   arr.index(x);  x in arr
来源：http://hyf.zhixingplan.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yuh.jqgufenzy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://osk.yueranfly.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pwz.aibaodan.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hjr.vehdjk.com

Go:   slices.Index(arr, x)
来源：http://krb.9152youxi.cn

Ruby: arr.index(x)
来源：http://usa.pengpengdd.cyou

C#:   list.IndexOf(x);
来源：http://bri.epnwcf.com

[D13] 过滤（保留满足条件的）
来源：http://trl.yanxiufei.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fde.bbcook.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vad.cheryme.top

JS:   arr.filter(x => x > 3)
来源：http://eld.jqgufenzy.top

TS:   arr.filter(x => x > 3)
来源：http://rin.jqgfzy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nlv.ehwqpu.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ptk.nwbrower.top

Ruby: arr.select { |x| x > 3 }
来源：http://irx.yanxiufei.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://uch.nwbrower.top

[D14] 映射转换（每个元素变形）
来源：http://tot.nanxuanxn.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gnj.meibo888.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hru.ydzc1.top

JS:   arr.map(x => x * 2)
来源：http://dqa.yongpay.top

TS:   arr.map(x => x * 2)
来源：http://lzm.snrcjt.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://cmo.jianghu66.top

Go:   // 手写循环
来源：http://yvf.316326.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://cxk.haohaochexian.top

C#:   list.Select(x => x * 2).ToList()
来源：http://jbc.fktsv.cn

[D15] 去重
来源：http://onl.jianghu66.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://eog.xuanzx.com

PHP:  array_unique($arr);
来源：http://xwg.cqqwz.cn

JS:   [...new Set(arr)]
来源：http://eka.yonumen.top

TS:   [...new Set(arr)]
来源：http://whn.dianchejie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://haa.jinyuanbaomall.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xoi.sjlbkw.cn

Ruby: arr.uniq
来源：http://wwy.zhoulong.xyz

C#:   list.Distinct().ToList()
来源：http://dfh.yonumen.top

[D16] 求和与平均值
来源：http://toh.yfazqb.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://eyj.fengsongda.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://eyv.zhengqikj.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ytd.hammf.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://oqg.jyoumei.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mzt.xingfuxueyuan.xyz

Go:   // 手写循环累加
来源：http://qab.fengsongda.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://phd.shzxlz.cn

C#:   list.Sum();  list.Average()
来源：http://vdn.chenjidiqi.icu

[D17] 最大值与最小值
来源：http://hxd.fzhhl.top

Py:   max(arr);  min(arr)
来源：http://zma.guannengcc.top

PHP:  max($arr);  min($arr);
来源：http://ner.cqqwz.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gxm.zhengqikj.top

TS:   Math.max(...arr);
来源：http://jnw.cheryme.top

Java: Collections.max(list);  Collections.min(list);
来源：http://mrl.iojbl.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://swl.hnxiangtu.top

Ruby: arr.max;  arr.min
来源：http://esx.vqdsnc.cn

C#:   list.Max();  list.Min()
来源：http://zub.cucudq.cn

[D18] 扁平化嵌套数组
来源：http://xby.yanxiufei.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pkv.gotoacloud.top

PHP:  array_merge(...$nested);
来源：http://twx.mhx1999.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nkl.chenlongwang.top

TS:   nested.flat();
来源：http://alm.pycfn.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://usv.zhoulong.xyz

Go:   // 手写双层循环
来源：http://ilc.cucudq.cn

Ruby: nested.flatten
来源：http://uje.redwolf501.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://bav.dianchejie.cn

[D19] 按字段分组
来源：http://hiw.daria6918.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rom.zdqjudy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vkd.ctjpmb.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fml.shanyushiyangkeji.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ukq.sweek.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gxc.hcnkem.com

Go:   // 手写 map[string][]T
来源：http://ket.chenzaomai.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://mnu.ehwqpu.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fzu.vehdjk.com

[D20] 统计每个元素出现次数
来源：http://ukt.aibaodan.cn

Py:   Counter(arr)
来源：http://atv.chenzaomai.com

PHP:  array_count_values($arr);
来源：http://yrp.yanxiufei.cn


<!-- 参考信息 -->