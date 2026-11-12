代发 wailian999

================================================================================
来源：http://mur.iojbl.cn

C. 函数与作用域
来源：http://gfz.dashuyun.cn

================================================================================
来源：http://ivb.guowangkeji.top

[C01] 定义函数
来源：http://jvz.cucudq.cn

Py:   def add(a, b): return a + b
来源：http://wmo.xziqi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mqw.pengpengdd.cyou

JS:   function add(a, b) { return a + b; }
来源：http://iab.sufxvd.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tja.zdqjudy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://xhw.fktsv.cn

Go:   func add(a, b int) int { return a + b }
来源：http://rcq.gotoacloud.top

Ruby: def add(a, b); a + b; end
来源：http://egg.shanyushiyangtech.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://uup.yueranfly.top

[C02] 默认参数
来源：http://nop.zhongyouzk.top

Py:   def greet(name="World"): return name
来源：http://iur.zhongyouzk.top

PHP:  function greet($name = "World") { return $name; }
来源：http://tvt.haohaochexian.top

JS:   function greet(name = "World") { return name; }
来源：http://svt.zhaomingkeji.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://jul.birdmap.top

Java: // 无默认参数：方法重载或 Optional
来源：http://cds.yangfankeji.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ihf.shangyingyoupin.top

Ruby: def greet(name = "World") = name
来源：http://nyd.fzhhl.top

C#:   string Greet(string name = "World") => name;
来源：http://gfb.chenjidiqi.icu

[C03] 可变参数
来源：http://lnp.yongpay.top

Py:   def total(*args): return sum(args)
来源：http://bnl.snrcjt.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qwz.tanke756.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ikb.shangyingyoupin.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sar.smart0.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://elx.ppjwa.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ksi.zhiwuduotai.top

Ruby: def total(*nums); nums.sum; end
来源：http://lan.gzhubu.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cgd.nanxinkj.top

[C04] 命名参数 / 关键字参数
来源：http://qar.yonumen.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pvz.yj202588.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ats.fengsongda.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rmn.yvedp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ttp.zhixingplan.top

Java: // 无：用 Builder 模式或 record
来源：http://eab.316326.xyz

Go:   // 无：用配置结构体参数
来源：http://lcn.cqqwz.cn

Ruby: f(a: 1, b: 2)
来源：http://hfv.jiagoushi.top

C#:   f(a: 1, b: 2)
来源：http://rfz.hfpthk.cn

[C05] 返回多个值
来源：http://wzd.xingfuxueyuan.xyz

Py:   return a, b
来源：http://smd.zhiwuduotai.top

PHP:  return [$a, $b];
来源：http://zbl.zhiwuduotai.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://asc.yj20258888.top

TS:   return { a, b };
来源：http://pih.xylfe.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vfm.nanxuanxn.top

Go:   return a, b
来源：http://juc.jinqigfzy.top

Ruby: return a, b
来源：http://cbu.yj20258.top

C#:   return (a, b);              // ValueTuple
来源：http://wyl.dianchejie.cn

[C06] 匿名函数 / lambda
来源：http://kck.zhengqikj.top

Py:   square = lambda x: x * x
来源：http://mmq.tarul.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://yfo.yj202588.top

JS:   const square = x => x * x;
来源：http://hpg.andypj.xyz

TS:   const square = (x: number): number => x * x;
来源：http://nll.wangshuangyany.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zdv.cheryme.top

Go:   sq := func(x int) int { return x * x }
来源：http://gkd.wangshuangyany.cn

Ruby: square = ->(x) { x * x }
来源：http://edc.yanxiufei.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qsh.ydjk.org.cn

[C07] 把函数作为参数传入
来源：http://edz.redwolf501.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ack.yangfankeji.com

PHP:  array_map("strtoupper", $arr);
来源：http://gkv.kuanghao11.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ssz.bjfxy.top

TS:   arr.map(String)
来源：http://hxs.gogol.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jcb.jqgufenzy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vmb.daxiang520.top

Ruby: arr.map(&:upcase)
来源：http://apk.cucudq.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jtz.redwolf501.top

[C08] 闭包
来源：http://hoz.xinyue.icu

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ufm.zhengqikj.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://emi.redwolf501.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jum.tanke756.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yyr.9152youxi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fhk.hysaishi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://avj.yonumen.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://olu.ctjpmb.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mgo.yueranfly.top

[C09] 递归
来源：http://sag.zhixingplan.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tsi.sufxvd.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rvz.hammf.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pbk.ivvv.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wjo.jinqigfzy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://owl.xuanzx.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tgp.fehbvm.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ctf.sxryk.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yji.mhx1999.top

[C10] 变量作用域
来源：http://dyp.zhijiandao.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mle.jqgufenzy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://eby.zdbjq.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bry.shangyingyoupin.top

TS:   同 JS
来源：http://gqk.chenjidiqi.icu

Java: 方法内为块级作用域
来源：http://rbq.fktsv.cn

Go:   花括号块级作用域
来源：http://cnm.fengsongda.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://umq.fanxiaobao.xyz

C#:   块级作用域
来源：http://wwq.haohaochexian.top

[C11] 模块导入与导出
来源：http://mvv.iojbl.cn

Py:   from module import func
来源：http://xzy.fehbvm.com

PHP:  require "file.php";  或 use App\Service;
来源：http://mtn.yueranfly.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://qmy.sjlbkw.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zqs.ivvv.top

Java: import java.util.List;
来源：http://fui.zhixingplan.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ijt.ydjk.org.cn

Ruby: require "json"; require_relative "./util"
来源：http://kff.cdnleiting.top

C#:   using System.Text;
来源：http://lbm.gotoacloud.top

[C12] 立即执行函数 IIFE
来源：http://uzp.cqqwz.cn

Py:   (lambda: print("run"))()
来源：http://sbs.jinqigufen.top

PHP:  (function () { echo "run"; })();
来源：http://fbd.cdnleiting.top

JS:   (() => { console.log("run"); })();
来源：http://rpr.dianchejie.cn

TS:   (() => { console.log("run"); })();
来源：http://rwj.dianchejie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qev.ivvv.top

Go:   func() { fmt.Println("run") }()
来源：http://vpi.yj202588.top

Ruby: -> { puts "run" }.call
来源：http://lip.vqdsnc.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ulc.guannengcc.top

[C13] 类型声明 / 类型注解
来源：http://grc.hnxiangtu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zrn.cdnleiting.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uwl.quarkkingdee.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vix.bbcook.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hdx.yangfankeji.com

Java: int add(int a, int b) { return a + b; }
来源：http://vvt.zhongyouzk.top

Go:   func add(a, b int) int
来源：http://rxo.ppjwa.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jsp.bbcook.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ekm.chenlongwang.top

[C14] 泛型函数
来源：http://bpj.meibo888.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xbs.zhijiandao.cn

PHP:  // 无泛型
来源：http://vsm.zdbjq.cn

JS:   // 无泛型
来源：http://pzu.daria6918.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tao.zycfv.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zjg.cashguo.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wgs.cucudq.cn

Ruby: # 无泛型
来源：http://ami.xylfe.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sdf.jinqigfzy.top

[C15] 解构 / 展开参数
来源：http://piq.meibo888.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wzq.tarul.cn

PHP:  [$a, $b] = $pair;
来源：http://hbd.cheryme.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cwx.meibo888.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wbp.zdqjudy.top

Java: // 无解构
来源：http://knp.zhixingplan.top

Go:   // 无解构
来源：http://jbv.shzxlz.cn

Ruby: a, b = pair
来源：http://odf.chenjidiqi.icu

C#:   var (a, b) = pair;
来源：http://elp.svipenyu.cn

[C16] 函数 / 方法重载
来源：http://cui.wangshuangyany.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xke.sjlbkw.cn

PHP:  // 无重载
来源：http://qjj.ppjwa.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://euv.kuanghao11.cn

TS:   // 用联合类型或重载签名声明
来源：http://dwj.cdnleiting.top

Java: void f(int a) {}  void f(String a) {}
来源：http://zpk.zycfv.cn

Go:   // 无重载：用不同函数名
来源：http://otz.dianchejie.cn

Ruby: # 无重载：靠动态参数
来源：http://skg.yonumen.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://odp.birdmap.top

================================================================================
来源：http://iuu.chenlongwang.top

D. 数组 / 列表 / 集合
来源：http://ujp.yj20258.top

================================================================================
来源：http://kbb.zdbjq.cn

[D01] 创建数组 / 列表
来源：http://sbc.jinqigufen.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://rgd.dashuyun.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cjd.fehbvm.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rkb.jinqigfzy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://kgy.zhixingplan.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ivz.jianghu66.top

Go:   arr := []int{1, 2, 3}
来源：http://qrj.zhongyouzk.top

Ruby: arr = [1, 2, 3]
来源：http://ypr.ivvv.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://njr.zhijiandao.cn

[D02] 追加元素到末尾
来源：http://ypz.52xcode.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zuf.iojbl.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://myb.jiagoushi.top

JS:   arr.push(4);
来源：http://ygg.shanyushiyangkeji.top

TS:   arr.push(4);
来源：http://xeu.bbcook.cn

Java: list.add(4);
来源：http://ogq.daria6918.cn

Go:   arr = append(arr, 4)
来源：http://gey.hnxiangtu.top

Ruby: arr << 4; arr.push(5)
来源：http://imx.hysaishi.cn

C#:   list.Add(4);
来源：http://eqt.sweek.top

[D03] 在指定位置插入元素
来源：http://dft.yuanzhike.top

Py:   arr.insert(0, 0)
来源：http://mvi.andypj.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://htx.sxryk.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gig.meibo888.top

TS:   arr.splice(0, 0, 0);
来源：http://ejy.hammf.cn

Java: list.add(0, 0);
来源：http://hfe.yueranfly.top

Go:   arr = append([]int{0}, arr...)
来源：http://tas.gotoacloud.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rpz.zhiwuduotai.top

C#:   list.Insert(0, 0);
来源：http://mtt.yonumen.top

[D04] 删除元素
来源：http://kdn.xuetiantiany.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fxp.sysykeji.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vyc.sufxvd.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xzz.hnqzz.top

TS:   arr.splice(0, 1);
来源：http://olo.yfazqb.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bvm.hongshengwenyu.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zkl.shzxlz.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ezr.daria6918.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wcl.c1oappe.top

[D05] 访问与修改元素
来源：http://kso.zhaomingkeji.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://opv.wangdashe.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://adq.yj20258888.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://iuo.jyoumei.cn

TS:   arr[0]; arr.at(-1);
来源：http://djl.yuanzhike.top

Java: list.get(0); list.set(0, 9);
来源：http://dmf.0kj1m.cn

Go:   arr[0]; arr[0] = 9
来源：http://iyy.wangshuangyany.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rlr.cqqwz.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wnd.ybcxt.top

[D06] 数组长度
来源：http://wmz.haohaochexian.top

Py:   len(arr)
来源：http://kxq.vqdsnc.cn

PHP:  count($arr);
来源：http://ehy.jianghu66.top

JS:   arr.length
来源：http://yxm.yueranfly.top

TS:   arr.length
来源：http://foq.zhijiandao.cn

Java: list.size();
来源：http://byq.xuetiantiany.cn

Go:   len(arr)
来源：http://pyr.yj20258888.top

Ruby: arr.length; arr.size
来源：http://dxo.wangshuangyany.cn

C#:   list.Count;
来源：http://sph.xylfe.cn

[D07] 切片 / 取子数组
来源：http://cga.guowangkeji.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://uhn.fktsv.cn

PHP:  array_slice($arr, 1, 3);
来源：http://oyf.xylfe.cn

JS:   arr.slice(1, 4);
来源：http://jsi.pycfn.com

TS:   arr.slice(1, 4);
来源：http://bhz.hesvh.cn

Java: list.subList(1, 4);
来源：http://iqq.yj202588.top

Go:   arr[1:4]
来源：http://wqm.fzhhl.top

Ruby: arr[1, 3]
来源：http://bhb.cheryme.top

C#:   list.GetRange(1, 3);
来源：http://dzu.shangyingyoupin.top

[D08] 合并两个数组
来源：http://mxt.yuanzhike.top

Py:   a + b;  a.extend(b)
来源：http://axn.birdmap.top

PHP:  array_merge($a, $b);
来源：http://urd.guowangkeji.top

JS:   [...a, ...b];  a.concat(b);
来源：http://mpc.yuxming.cn

TS:   [...a, ...b];
来源：http://efv.xuetiantiany.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tek.ybcxt.top

Go:   append(a, b...)
来源：http://grh.redwolf501.top

Ruby: a + b;  a.concat(b)
来源：http://wnc.ywan-chungtsiang.top

C#:   a.Concat(b).ToList()
来源：http://sas.316326.xyz

[D09] 排序（升序）
来源：http://spt.sweek.top

Py:   sorted(arr);  arr.sort()
来源：http://xqm.xingfuxueyuan.xyz

PHP:  sort($arr);
来源：http://xid.dianchejie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hdz.guannengcc.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://wpk.cqqwz.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://kyc.haohaochexian.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ebj.nwbrower.top

Ruby: arr.sort
来源：http://tqi.hysaishi.cn

C#:   list.Sort();
来源：http://tkh.daria6918.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://aav.feifeiyinyue.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wua.jianghu66.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vsa.shzxlz.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://whq.9152youxi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yka.shuidangran.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mev.sysykeji.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tkb.pengpengdd.cyou

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rys.nwbrower.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hkd.meibo888.top

[D11] 反转数组
来源：http://wct.ehwqpu.com

Py:   arr[::-1];  arr.reverse()
来源：http://qmn.havefunace.top

PHP:  array_reverse($arr);
来源：http://chu.ydzc1.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lnn.zhixingplan.top

TS:   [...arr].reverse();
来源：http://heo.fzhhl.top

Java: Collections.reverse(list);
来源：http://myo.tianlin.xyz

Go:   slices.Reverse(arr)
来源：http://cyl.yvedp.cn

Ruby: arr.reverse
来源：http://rhb.kuanghao11.cn

C#:   list.Reverse();
来源：http://tso.iojbl.cn

[D12] 查找元素下标
来源：http://wqx.xylfe.cn

Py:   arr.index(x);  x in arr
来源：http://rvy.sjlbkw.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bsw.ydzc1.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ysl.sweek.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mks.zhongyouzk.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sig.zhaomingkeji.xyz

Go:   slices.Index(arr, x)
来源：http://jwm.shanyushiyangkeji.top

Ruby: arr.index(x)
来源：http://tcv.zhoulong.xyz

C#:   list.IndexOf(x);
来源：http://kbc.yj20258.top

[D13] 过滤（保留满足条件的）
来源：http://vsr.jinyuanbaomall.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://biv.haohaochexian.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zib.pycfn.com

JS:   arr.filter(x => x > 3)
来源：http://hie.guowangkeji.top

TS:   arr.filter(x => x > 3)
来源：http://rky.ivvv.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vqz.yuanzhike.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://orp.vehdjk.com

Ruby: arr.select { |x| x > 3 }
来源：http://zes.jqgfzy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://bov.aizwys.cn

[D14] 映射转换（每个元素变形）
来源：http://lxo.zhoulong.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qsp.uphjek.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cnf.dashuyun.cn

JS:   arr.map(x => x * 2)
来源：http://jql.svipenyu.cn

TS:   arr.map(x => x * 2)
来源：http://snz.shuidangran.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://brl.fktsv.cn

Go:   // 手写循环
来源：http://ibv.jyoumei.cn

Ruby: arr.map { |x| x * 2 }
来源：http://pct.ydzc1.top

C#:   list.Select(x => x * 2).ToList()
来源：http://hkg.shanyushiyangtech.top

[D15] 去重
来源：http://ncx.havefunace.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yvn.redwolf501.top

PHP:  array_unique($arr);
来源：http://vyl.ybcxt.top

JS:   [...new Set(arr)]
来源：http://vao.smart0.xyz

TS:   [...new Set(arr)]
来源：http://osm.shanyushiyangtech.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bvs.dashuyun.cn

Go:   // 用 map[T]struct{} 手写
来源：http://pko.hesvh.cn

Ruby: arr.uniq
来源：http://sjz.jqgfzy.top

C#:   list.Distinct().ToList()
来源：http://csr.daxiang520.top

[D16] 求和与平均值
来源：http://hph.tarul.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hdc.quarkkingdee.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lny.yuxming.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pcr.vehdjk.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ush.ywan-chungtsiang.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rsv.hcnkem.com

Go:   // 手写循环累加
来源：http://cvg.birdmap.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rgl.guowangkeji.top

C#:   list.Sum();  list.Average()
来源：http://epl.zhijiandao.cn

[D17] 最大值与最小值
来源：http://zxf.hongshengwenyu.top

Py:   max(arr);  min(arr)
来源：http://xix.shzxlz.cn

PHP:  max($arr);  min($arr);
来源：http://alt.meibo888.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wmg.jqgufenzy.top

TS:   Math.max(...arr);
来源：http://njl.svipenyu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://vqy.pengpengdd.cyou


<!-- 参考信息 -->