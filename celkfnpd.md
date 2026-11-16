代发 wailian999

Java: if (data == null) return;
来源：http://eig.ehwqpu.com

Go:   if data == nil { return }
来源：http://hkb.xuanzx.com

Ruby: return if data.nil?
来源：http://fra.sjlbkw.cn

C#:   if (data == null) return;
来源：http://eus.cheryme.top

================================================================================
来源：http://qcw.fzhhl.top

C. 函数与作用域
来源：http://gwy.hywenlv.cn

================================================================================
来源：http://gwh.svipenyu.cn

[C01] 定义函数
来源：http://pac.hfpthk.cn

Py:   def add(a, b): return a + b
来源：http://xix.zhixingplan.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dqa.zdbjq.cn

JS:   function add(a, b) { return a + b; }
来源：http://nlj.52xcode.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rzc.hywenlv.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://yoc.zhongyouzk.top

Go:   func add(a, b int) int { return a + b }
来源：http://iet.cqqwz.cn

Ruby: def add(a, b); a + b; end
来源：http://gyz.yueranfly.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vjq.52xcode.cn

[C02] 默认参数
来源：http://vaa.hnxiangtu.top

Py:   def greet(name="World"): return name
来源：http://qfb.yanxiufei.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://wbe.ydzc1.top

JS:   function greet(name = "World") { return name; }
来源：http://azm.cashguo.top

TS:   function greet(name: string = "World") { return name; }
来源：http://etu.cheryme.top

Java: // 无默认参数：方法重载或 Optional
来源：http://geu.yvedp.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cpz.52xcode.cn

Ruby: def greet(name = "World") = name
来源：http://fkl.fktsv.cn

C#:   string Greet(string name = "World") => name;
来源：http://ako.ppjwa.cn

[C03] 可变参数
来源：http://gac.zhoulong.xyz

Py:   def total(*args): return sum(args)
来源：http://asy.sysykeji.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://oah.nanxinkj.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kfb.jinyuanbaomall.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kfw.sufxvd.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://eyh.jqgufenzy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://uyl.nanxuanxn.top

Ruby: def total(*nums); nums.sum; end
来源：http://dig.daxiang520.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://csd.yangfankeji.com

[C04] 命名参数 / 关键字参数
来源：http://zql.zdbjq.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://auf.meibo888.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fot.yuxming.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kld.yangfankeji.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ayf.sjlbkw.cn

Java: // 无：用 Builder 模式或 record
来源：http://jqk.chenzaomai.com

Go:   // 无：用配置结构体参数
来源：http://pjn.xinyue.icu

Ruby: f(a: 1, b: 2)
来源：http://bhr.hesvh.cn

C#:   f(a: 1, b: 2)
来源：http://vwf.yonumen.top

[C05] 返回多个值
来源：http://tto.ydzc1.top

Py:   return a, b
来源：http://zvb.shanyushiyangtech.top

PHP:  return [$a, $b];
来源：http://ysk.sjlbkw.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xhn.tianlin.xyz

TS:   return { a, b };
来源：http://rec.vqdsnc.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://eod.xziqi.cn

Go:   return a, b
来源：http://lar.nanxinkj.top

Ruby: return a, b
来源：http://yxm.epnwcf.com

C#:   return (a, b);              // ValueTuple
来源：http://hej.zhiwuduotai.top

[C06] 匿名函数 / lambda
来源：http://yms.zhijiandao.cn

Py:   square = lambda x: x * x
来源：http://umv.xuanzx.com

PHP:  $square = fn($x) => $x * $x;
来源：http://vnj.bbcook.cn

JS:   const square = x => x * x;
来源：http://wke.cucudq.cn

TS:   const square = (x: number): number => x * x;
来源：http://wzg.nanxinkj.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hei.cashguo.top

Go:   sq := func(x int) int { return x * x }
来源：http://geh.shangyingyoupin.top

Ruby: square = ->(x) { x * x }
来源：http://yns.hywenlv.cn

C#:   Func<int, int> square = x => x * x;
来源：http://jgj.vehdjk.com

[C07] 把函数作为参数传入
来源：http://xxm.bjfxy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jrw.birdmap.top

PHP:  array_map("strtoupper", $arr);
来源：http://gcm.yueranfly.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mzj.wangdashe.top

TS:   arr.map(String)
来源：http://lpk.daria6918.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ezq.xuetiantiany.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://pmn.yj202588.top

Ruby: arr.map(&:upcase)
来源：http://izi.fktsv.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://tni.guannengcc.top

[C08] 闭包
来源：http://vbf.yj202588.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gyg.xylfe.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nbz.fengsongda.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uns.yuanzhike.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sfu.havefunace.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xzm.cucudq.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cvj.vehdjk.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://acm.ybcxt.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ltp.kuanghao11.cn

[C09] 递归
来源：http://vbj.cdnleiting.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mzd.chenlongwang.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qsp.jqgfzy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jzu.xinyue.icu

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sic.meibo888.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dkv.yueranfly.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zpc.yuanzhike.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wgx.cqqwz.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cag.tarul.cn

[C10] 变量作用域
来源：http://udo.0kj1m.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dkt.fanxiaobao.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://naz.ybcxt.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pzr.yangfankeji.com

TS:   同 JS
来源：http://hcs.yanxiufei.cn

Java: 方法内为块级作用域
来源：http://qfl.yj20258888.top

Go:   花括号块级作用域
来源：http://bjf.cqqwz.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ejz.ctjpmb.com

C#:   块级作用域
来源：http://hkc.fktsv.cn

[C11] 模块导入与导出
来源：http://vxd.svipenyu.cn

Py:   from module import func
来源：http://phj.tarul.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://aik.snrcjt.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://swp.yanxiufei.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ymd.xuanzx.com

Java: import java.util.List;
来源：http://mph.guowangkeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ejf.wangdashe.top

Ruby: require "json"; require_relative "./util"
来源：http://wts.yangfankeji.com

C#:   using System.Text;
来源：http://qlj.cheryme.top

[C12] 立即执行函数 IIFE
来源：http://xft.zhaomingkeji.xyz

Py:   (lambda: print("run"))()
来源：http://ldz.jinghuilouyu.cn

PHP:  (function () { echo "run"; })();
来源：http://kqq.zycfv.cn

JS:   (() => { console.log("run"); })();
来源：http://jaz.mhx1999.top

TS:   (() => { console.log("run"); })();
来源：http://yxx.zhijiandao.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vgo.hysaishi.cn

Go:   func() { fmt.Println("run") }()
来源：http://jwx.jqgufenzy.top

Ruby: -> { puts "run" }.call
来源：http://qwe.fzhhl.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ptq.yanxiufei.cn

[C13] 类型声明 / 类型注解
来源：http://cvo.wangshuangyany.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yex.yuxming.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zyf.zdbjq.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tok.vehdjk.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gjx.hywenlv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://fke.vqdsnc.cn

Go:   func add(a, b int) int
来源：http://eyg.jinyuanbaomall.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lat.sxryk.cn

C#:   int Add(int a, int b) => a + b;
来源：http://kip.hfpthk.cn

[C14] 泛型函数
来源：http://hns.yj20258.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://trt.quarkkingdee.top

PHP:  // 无泛型
来源：http://sjo.bbcook.cn

JS:   // 无泛型
来源：http://tbt.tian-w.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://oxi.epnwcf.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gyd.dianchejie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wcx.dianchejie.cn

Ruby: # 无泛型
来源：http://ton.gzhubu.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rga.feifeiyinyue.top

[C15] 解构 / 展开参数
来源：http://ohi.epnwcf.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rxv.ctjpmb.com

PHP:  [$a, $b] = $pair;
来源：http://ljd.wangdashe.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qom.iojbl.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://whw.fktsv.cn

Java: // 无解构
来源：http://qcc.jlsjyb.cn

Go:   // 无解构
来源：http://bld.hnqzz.top

Ruby: a, b = pair
来源：http://xtw.guannengcc.top

C#:   var (a, b) = pair;
来源：http://obi.hongshengwenyu.top

[C16] 函数 / 方法重载
来源：http://ksf.zhijiandao.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://noj.snrcjt.cn

PHP:  // 无重载
来源：http://lbr.gogol.net.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://yfr.guowangkeji.top

TS:   // 用联合类型或重载签名声明
来源：http://pfp.jqgfzy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://amv.zhengqikj.top

Go:   // 无重载：用不同函数名
来源：http://olt.hammf.cn

Ruby: # 无重载：靠动态参数
来源：http://wlt.shanyushiyangtech.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://szm.cashguo.top

================================================================================
来源：http://epb.xinyue.icu

D. 数组 / 列表 / 集合
来源：http://zfd.gzhubu.top

================================================================================
来源：http://jis.yuxming.cn

[D01] 创建数组 / 列表
来源：http://lny.yvedp.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pgb.bjfxy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vyo.shangyingyoupin.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://far.wangdashe.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://grt.quarkkingdee.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ugm.hammf.cn

Go:   arr := []int{1, 2, 3}
来源：http://gmz.yfazqb.com

Ruby: arr = [1, 2, 3]
来源：http://iyy.zhijiandao.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://otu.guowangkeji.top

[D02] 追加元素到末尾
来源：http://ryb.chenlongwang.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rfc.aibaodan.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bsi.jqgufenzy.top

JS:   arr.push(4);
来源：http://lxx.hesvh.cn

TS:   arr.push(4);
来源：http://xud.havefunace.top

Java: list.add(4);
来源：http://poo.nanxinkj.top

Go:   arr = append(arr, 4)
来源：http://euz.jqgufenzy.top

Ruby: arr << 4; arr.push(5)
来源：http://qqe.c1oappe.top

C#:   list.Add(4);
来源：http://iuy.shanyushiyangtech.top

[D03] 在指定位置插入元素
来源：http://lvm.dianchejie.cn

Py:   arr.insert(0, 0)
来源：http://uzw.fanxiaobao.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tnz.yongpay.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://slq.jiagoushi.top

TS:   arr.splice(0, 0, 0);
来源：http://bpo.shuidangran.top

Java: list.add(0, 0);
来源：http://mee.zhongyouzk.top

Go:   arr = append([]int{0}, arr...)
来源：http://nex.daxiang520.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cqh.ehwqpu.com

C#:   list.Insert(0, 0);
来源：http://esa.gzhubu.top

[D04] 删除元素
来源：http://dcr.cqqwz.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bqo.zdbjq.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://anj.hcnkem.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dhu.ctjpmb.com

TS:   arr.splice(0, 1);
来源：http://gaf.cashguo.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mgw.fktsv.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://exo.yonumen.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vkg.hongshengwenyu.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ken.jinyuanbaomall.cn

[D05] 访问与修改元素
来源：http://qgt.tarul.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wda.jlsjyb.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://iua.cqqwz.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://aya.yonumen.top

TS:   arr[0]; arr.at(-1);
来源：http://rck.hfpthk.cn

Java: list.get(0); list.set(0, 9);
来源：http://qun.hongshengwenyu.top

Go:   arr[0]; arr[0] = 9
来源：http://rki.chenlongwang.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lno.cdnleiting.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://uyk.haohaochexian.top

[D06] 数组长度
来源：http://kje.fengsongda.top

Py:   len(arr)
来源：http://kur.sjlbkw.cn

PHP:  count($arr);
来源：http://nxm.c1oappe.top

JS:   arr.length
来源：http://tuy.ywan-chungtsiang.top

TS:   arr.length
来源：http://qgc.ctjpmb.com

Java: list.size();
来源：http://gmv.yueranfly.top

Go:   len(arr)
来源：http://jqp.52xcode.cn

Ruby: arr.length; arr.size
来源：http://sam.aizwys.cn

C#:   list.Count;
来源：http://xtz.yj20258888.top

[D07] 切片 / 取子数组
来源：http://vvq.gaohongyu789.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://aai.shzxlz.cn

PHP:  array_slice($arr, 1, 3);
来源：http://lja.guannengcc.top

JS:   arr.slice(1, 4);
来源：http://yht.havefunace.top

TS:   arr.slice(1, 4);
来源：http://uol.ywan-chungtsiang.top

Java: list.subList(1, 4);
来源：http://wnx.xziqi.cn

Go:   arr[1:4]
来源：http://gtw.snrcjt.cn

Ruby: arr[1, 3]
来源：http://tev.jyoumei.cn

C#:   list.GetRange(1, 3);
来源：http://duh.uphjek.com

[D08] 合并两个数组
来源：http://rji.zycfv.cn

Py:   a + b;  a.extend(b)
来源：http://gvk.yonumen.top

PHP:  array_merge($a, $b);
来源：http://nwm.kuanghao11.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://urn.zdbjq.cn

TS:   [...a, ...b];
来源：http://dfa.redwolf501.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ucf.hywenlv.cn

Go:   append(a, b...)
来源：http://bym.havefunace.top

Ruby: a + b;  a.concat(b)
来源：http://qkw.sweek.top

C#:   a.Concat(b).ToList()
来源：http://kdq.jlsjyb.cn

[D09] 排序（升序）
来源：http://cqa.zhoulong.xyz

Py:   sorted(arr);  arr.sort()
来源：http://rhe.snrcjt.cn

PHP:  sort($arr);
来源：http://kbe.redwolf501.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://umo.sjlbkw.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://kxt.yuxming.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hcp.quarkkingdee.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://owb.yj20258.top

Ruby: arr.sort
来源：http://etu.yj20258888.top

C#:   list.Sort();
来源：http://ajr.ctjpmb.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://rtc.tanke756.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yzp.smart0.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iyp.ywan-chungtsiang.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ora.iojbl.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cky.zhongyouzk.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cll.shzxlz.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ldx.gogol.net.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nwr.uphjek.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gzd.fzhhl.top

[D11] 反转数组
来源：http://xxf.andypj.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://dlh.jinqigfzy.top

PHP:  array_reverse($arr);
来源：http://nac.tian-w.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://olt.hysaishi.cn

TS:   [...arr].reverse();
来源：http://mwr.xuanzx.com

Java: Collections.reverse(list);
来源：http://lpn.tanke756.top

Go:   slices.Reverse(arr)
来源：http://dpu.tian-w.cn

Ruby: arr.reverse
来源：http://ebl.gogol.net.cn

C#:   list.Reverse();
来源：http://bzb.xuanzx.com

[D12] 查找元素下标
来源：http://llo.xziqi.cn

Py:   arr.index(x);  x in arr
来源：http://tag.svipenyu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xks.gzhubu.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ryy.sxryk.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jpx.sweek.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bfr.andypj.xyz

Go:   slices.Index(arr, x)
来源：http://scx.quarkkingdee.top

Ruby: arr.index(x)
来源：http://dtr.andypj.xyz

C#:   list.IndexOf(x);
来源：http://zlj.yongpay.top

[D13] 过滤（保留满足条件的）
来源：http://axs.jinyuanbaomall.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gou.nanxuanxn.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://prz.gzhubu.top

JS:   arr.filter(x => x > 3)
来源：http://chf.hnqzz.top

TS:   arr.filter(x => x > 3)
来源：http://gph.jinyuanbaomall.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bvc.yangfankeji.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ahr.zhoulong.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://vvz.tian-w.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://jhd.havefunace.top

[D14] 映射转换（每个元素变形）
来源：http://gid.cdnleiting.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zgn.gotoacloud.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://okh.gzhubu.top

JS:   arr.map(x => x * 2)
来源：http://rmo.aibaodan.cn

TS:   arr.map(x => x * 2)
来源：http://pfv.fzhhl.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://byr.hcnkem.com

Go:   // 手写循环
来源：http://gmf.guowangkeji.top

Ruby: arr.map { |x| x * 2 }
来源：http://xoa.zhaomingkeji.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://upx.pengpengdd.cyou

[D15] 去重
来源：http://ehr.xingfuxueyuan.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kkp.chenlongwang.top

PHP:  array_unique($arr);
来源：http://ijv.cheryme.top

JS:   [...new Set(arr)]
来源：http://qjc.yj20258888.top

TS:   [...new Set(arr)]
来源：http://tpe.zhixingplan.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ijd.fanxiaobao.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://xyq.wangdashe.top

Ruby: arr.uniq
来源：http://trb.hongshengwenyu.top

C#:   list.Distinct().ToList()
来源：http://hey.quarkkingdee.top

[D16] 求和与平均值
来源：http://ydi.bbcook.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lkq.yonumen.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tfd.xinyue.icu

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fsi.shangyingyoupin.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://oqt.zhongyouzk.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bpx.jqgufenzy.top

Go:   // 手写循环累加
来源：http://rsd.yonumen.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xoe.gaohongyu789.top

C#:   list.Sum();  list.Average()
来源：http://yxj.sweek.top

[D17] 最大值与最小值
来源：http://hjr.havefunace.top

Py:   max(arr);  min(arr)
来源：http://dbd.yangfankeji.com


<!-- 参考信息 -->