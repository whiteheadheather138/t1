代发 wailian999

Java: if (data == null) return;
来源：http://eyb.c1oappe.top

Go:   if data == nil { return }
来源：http://tna.daria6918.cn

Ruby: return if data.nil?
来源：http://mfv.xziqi.cn

C#:   if (data == null) return;
来源：http://gar.iojbl.cn

================================================================================
来源：http://iyf.daxiang520.top

C. 函数与作用域
来源：http://bwh.sufxvd.cn

================================================================================
来源：http://eib.yuanzhike.top

[C01] 定义函数
来源：http://awd.yonumen.top

Py:   def add(a, b): return a + b
来源：http://nbm.hcnkem.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xel.zdqjudy.top

JS:   function add(a, b) { return a + b; }
来源：http://dme.zhoulong.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://grg.sxryk.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://odw.hywenlv.cn

Go:   func add(a, b int) int { return a + b }
来源：http://blq.yj20258888.top

Ruby: def add(a, b); a + b; end
来源：http://zmz.fanxiaobao.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vzx.fktsv.cn

[C02] 默认参数
来源：http://suq.316326.xyz

Py:   def greet(name="World"): return name
来源：http://cez.sxryk.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://sjy.zhixingplan.top

JS:   function greet(name = "World") { return name; }
来源：http://ixc.cucudq.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://gpd.yuanzhike.top

Java: // 无默认参数：方法重载或 Optional
来源：http://unj.sufxvd.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://unc.yueranfly.top

Ruby: def greet(name = "World") = name
来源：http://fon.tarul.cn

C#:   string Greet(string name = "World") => name;
来源：http://lfp.daria6918.cn

[C03] 可变参数
来源：http://dzg.zhixingplan.top

Py:   def total(*args): return sum(args)
来源：http://lrv.zhaomingkeji.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jpg.redwolf501.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://byc.kuanghao11.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zei.yongpay.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kij.zhixingplan.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rxh.jqgufenzy.top

Ruby: def total(*nums); nums.sum; end
来源：http://pyb.havefunace.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hdj.jlsjyb.cn

[C04] 命名参数 / 关键字参数
来源：http://nfv.zhongyouzk.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ike.tanke756.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hsq.jiagoushi.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://awn.vqdsnc.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rkr.chenzaomai.com

Java: // 无：用 Builder 模式或 record
来源：http://vje.tian-w.cn

Go:   // 无：用配置结构体参数
来源：http://ckp.jinqigufen.top

Ruby: f(a: 1, b: 2)
来源：http://tjw.guannengcc.top

C#:   f(a: 1, b: 2)
来源：http://urt.52xcode.cn

[C05] 返回多个值
来源：http://lkz.guowangkeji.top

Py:   return a, b
来源：http://ttv.yueranfly.top

PHP:  return [$a, $b];
来源：http://jfr.feifeiyinyue.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://nts.dianchejie.cn

TS:   return { a, b };
来源：http://ges.xuanzx.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qwj.zdqjudy.top

Go:   return a, b
来源：http://ptm.zhixingplan.top

Ruby: return a, b
来源：http://bwp.uphjek.com

C#:   return (a, b);              // ValueTuple
来源：http://iio.haohaochexian.top

[C06] 匿名函数 / lambda
来源：http://qcr.pycfn.com

Py:   square = lambda x: x * x
来源：http://dku.yueranfly.top

PHP:  $square = fn($x) => $x * $x;
来源：http://len.vehdjk.com

JS:   const square = x => x * x;
来源：http://zgh.xziqi.cn

TS:   const square = (x: number): number => x * x;
来源：http://rqh.zhijiandao.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://aeo.shanyushiyangtech.top

Go:   sq := func(x int) int { return x * x }
来源：http://olh.quarkkingdee.top

Ruby: square = ->(x) { x * x }
来源：http://qtp.sjlbkw.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fpc.tian-w.cn

[C07] 把函数作为参数传入
来源：http://dxk.nwbrower.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://epp.pycfn.com

PHP:  array_map("strtoupper", $arr);
来源：http://gpi.tarul.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://szt.sjlbkw.cn

TS:   arr.map(String)
来源：http://gzs.zhaomingkeji.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ehi.9152youxi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fep.fzhhl.top

Ruby: arr.map(&:upcase)
来源：http://sah.iojbl.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qku.xuetiantiany.cn

[C08] 闭包
来源：http://xjk.yuanzhike.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mdt.yangfankeji.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wew.vqdsnc.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zsh.tianlin.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ket.ppjwa.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ybq.yj202588.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zok.shanyushiyangkeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nfy.vehdjk.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rbm.sweek.top

[C09] 递归
来源：http://jxi.yj20258888.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ium.jianghu66.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nrb.zhaomingkeji.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pcb.birdmap.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mmr.haohaochexian.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nxx.pycfn.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rcm.bjfxy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ixz.hcnkem.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rss.vqdsnc.cn

[C10] 变量作用域
来源：http://uls.jinghuilouyu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cza.fanxiaobao.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://htw.chenzaomai.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qae.nanxuanxn.top

TS:   同 JS
来源：http://nke.jiagoushi.top

Java: 方法内为块级作用域
来源：http://knf.9152youxi.cn

Go:   花括号块级作用域
来源：http://wgg.jinghuilouyu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gnp.havefunace.top

C#:   块级作用域
来源：http://yby.shanyushiyangtech.top

[C11] 模块导入与导出
来源：http://fio.52xcode.cn

Py:   from module import func
来源：http://pdc.vehdjk.com

PHP:  require "file.php";  或 use App\Service;
来源：http://toz.sjlbkw.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://biq.haohaochexian.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vvr.jianghu66.top

Java: import java.util.List;
来源：http://thi.hnxiangtu.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dhe.svipenyu.cn

Ruby: require "json"; require_relative "./util"
来源：http://wqc.hcnkem.com

C#:   using System.Text;
来源：http://ybb.zhijiandao.cn

[C12] 立即执行函数 IIFE
来源：http://ous.shangyingyoupin.top

Py:   (lambda: print("run"))()
来源：http://bga.ywan-chungtsiang.top

PHP:  (function () { echo "run"; })();
来源：http://lmf.sjlbkw.cn

JS:   (() => { console.log("run"); })();
来源：http://ymu.zdbjq.cn

TS:   (() => { console.log("run"); })();
来源：http://xld.zhoulong.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hro.shanyushiyangtech.top

Go:   func() { fmt.Println("run") }()
来源：http://nmj.tanke756.top

Ruby: -> { puts "run" }.call
来源：http://loo.shanyushiyangtech.top

C#:   // 无 IIFE：用静态构造函数
来源：http://zvk.dianchejie.cn

[C13] 类型声明 / 类型注解
来源：http://hvg.xziqi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rqr.yj20258.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mbh.yangfankeji.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://szm.daria6918.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zay.zycfv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://hto.fzhhl.top

Go:   func add(a, b int) int
来源：http://yak.zdbjq.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nic.yangfankeji.com

C#:   int Add(int a, int b) => a + b;
来源：http://von.yj20258.top

[C14] 泛型函数
来源：http://wlo.hnxiangtu.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gtb.yuanzhike.top

PHP:  // 无泛型
来源：http://uzc.ydzc1.top

JS:   // 无泛型
来源：http://qae.redwolf501.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mzo.gotoacloud.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wou.ydzc1.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hbm.fengsongda.top

Ruby: # 无泛型
来源：http://jxs.haohaochexian.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://iln.jlsjyb.cn

[C15] 解构 / 展开参数
来源：http://ztl.hesvh.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kqu.hongshengwenyu.top

PHP:  [$a, $b] = $pair;
来源：http://shi.zdqjudy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lgh.andypj.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fso.hfpthk.cn

Java: // 无解构
来源：http://ror.zhengqikj.top

Go:   // 无解构
来源：http://hno.jqgfzy.top

Ruby: a, b = pair
来源：http://cjg.ivvv.top

C#:   var (a, b) = pair;
来源：http://ufu.dashuyun.cn

[C16] 函数 / 方法重载
来源：http://lej.andypj.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cxm.tian-w.cn

PHP:  // 无重载
来源：http://srp.jyoumei.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bwl.yonumen.top

TS:   // 用联合类型或重载签名声明
来源：http://zgx.tianlin.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://qcq.fzhhl.top

Go:   // 无重载：用不同函数名
来源：http://glo.hcnkem.com

Ruby: # 无重载：靠动态参数
来源：http://xln.chenzaomai.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://wcq.0kj1m.cn

================================================================================
来源：http://ddq.zhiwuduotai.top

D. 数组 / 列表 / 集合
来源：http://ryt.chenzaomai.com

================================================================================
来源：http://dby.9152youxi.cn

[D01] 创建数组 / 列表
来源：http://iml.shzxlz.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://rju.bbcook.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rlo.redwolf501.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ogv.sxryk.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://jlj.52xcode.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hpj.shuidangran.top

Go:   arr := []int{1, 2, 3}
来源：http://oaz.tarul.cn

Ruby: arr = [1, 2, 3]
来源：http://piq.cheryme.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jli.ppjwa.cn

[D02] 追加元素到末尾
来源：http://xnq.zhoulong.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vbo.andypj.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wqs.yj20258888.top

JS:   arr.push(4);
来源：http://dhu.mhx1999.top

TS:   arr.push(4);
来源：http://mhx.aizwys.cn

Java: list.add(4);
来源：http://kuq.bbcook.cn

Go:   arr = append(arr, 4)
来源：http://xih.guannengcc.top

Ruby: arr << 4; arr.push(5)
来源：http://foh.zhaomingkeji.xyz

C#:   list.Add(4);
来源：http://lok.chenlongwang.top

[D03] 在指定位置插入元素
来源：http://vmu.zhaomingkeji.xyz

Py:   arr.insert(0, 0)
来源：http://ygu.hcnkem.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hot.sweek.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vup.hnqzz.top

TS:   arr.splice(0, 0, 0);
来源：http://myf.cheryme.top

Java: list.add(0, 0);
来源：http://caq.ivvv.top

Go:   arr = append([]int{0}, arr...)
来源：http://aeh.wangdashe.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fpz.9152youxi.cn

C#:   list.Insert(0, 0);
来源：http://obz.cdnleiting.top

[D04] 删除元素
来源：http://tdj.feifeiyinyue.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://syk.jianghu66.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tfv.snrcjt.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://veb.wangdashe.top

TS:   arr.splice(0, 1);
来源：http://kdq.hesvh.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://whe.jyoumei.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mtd.cdnleiting.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vjp.wangshuangyany.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ktz.iojbl.cn

[D05] 访问与修改元素
来源：http://nfy.zhongyouzk.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zaw.zhoulong.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ere.zhoulong.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://axl.0kj1m.cn

TS:   arr[0]; arr.at(-1);
来源：http://tvp.smart0.xyz

Java: list.get(0); list.set(0, 9);
来源：http://sff.ywan-chungtsiang.top

Go:   arr[0]; arr[0] = 9
来源：http://dgk.zhoulong.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sba.zdqjudy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bay.zhengqikj.top

[D06] 数组长度
来源：http://oim.cashguo.top

Py:   len(arr)
来源：http://vwo.yj202588.top

PHP:  count($arr);
来源：http://pyc.hcnkem.com

JS:   arr.length
来源：http://nkx.aibaodan.cn

TS:   arr.length
来源：http://kvf.mhx1999.top

Java: list.size();
来源：http://juo.chenzaomai.com

Go:   len(arr)
来源：http://khd.daxiang520.top

Ruby: arr.length; arr.size
来源：http://rrs.cashguo.top

C#:   list.Count;
来源：http://wsf.yangfankeji.com

[D07] 切片 / 取子数组
来源：http://rfx.zhijiandao.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://djw.gotoacloud.top

PHP:  array_slice($arr, 1, 3);
来源：http://akj.0kj1m.cn

JS:   arr.slice(1, 4);
来源：http://ejb.jinyuanbaomall.cn

TS:   arr.slice(1, 4);
来源：http://asn.zhiwuduotai.top

Java: list.subList(1, 4);
来源：http://seh.havefunace.top

Go:   arr[1:4]
来源：http://yxs.birdmap.top

Ruby: arr[1, 3]
来源：http://qud.sufxvd.cn

C#:   list.GetRange(1, 3);
来源：http://usc.bbcook.cn

[D08] 合并两个数组
来源：http://odb.yueranfly.top

Py:   a + b;  a.extend(b)
来源：http://wpi.xuanzx.com

PHP:  array_merge($a, $b);
来源：http://ykl.yj202588.top

JS:   [...a, ...b];  a.concat(b);
来源：http://kpe.yanxiufei.cn

TS:   [...a, ...b];
来源：http://oji.yuanzhike.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hyw.epnwcf.com

Go:   append(a, b...)
来源：http://dvz.cheryme.top

Ruby: a + b;  a.concat(b)
来源：http://dym.hesvh.cn

C#:   a.Concat(b).ToList()
来源：http://xxp.sxryk.cn

[D09] 排序（升序）
来源：http://piz.epnwcf.com

Py:   sorted(arr);  arr.sort()
来源：http://lhh.yj202588.top

PHP:  sort($arr);
来源：http://zsm.yuanzhike.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cgx.hnqzz.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://fvs.jiagoushi.top

Java: Collections.sort(list);  list.sort(null);
来源：http://wmw.52xcode.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uku.jiagoushi.top

Ruby: arr.sort
来源：http://kqj.epnwcf.com

C#:   list.Sort();
来源：http://nmv.xinyue.icu

[D10] 自定义排序（按字段 / 多条件）
来源：http://xnk.quarkkingdee.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ude.yuanzhike.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kbo.zhoulong.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kjq.haohaochexian.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lek.hongshengwenyu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ygl.shanyushiyangkeji.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vxw.fktsv.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cet.vehdjk.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://eej.wangshuangyany.cn

[D11] 反转数组
来源：http://jhx.316326.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://rew.pycfn.com

PHP:  array_reverse($arr);
来源：http://wrn.zdqjudy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://aem.nwbrower.top

TS:   [...arr].reverse();
来源：http://qov.guowangkeji.top

Java: Collections.reverse(list);
来源：http://zbw.svipenyu.cn

Go:   slices.Reverse(arr)
来源：http://tiq.fzhhl.top

Ruby: arr.reverse
来源：http://kxx.tarul.cn

C#:   list.Reverse();
来源：http://xwt.nanxinkj.top

[D12] 查找元素下标
来源：http://xmx.jqgufenzy.top

Py:   arr.index(x);  x in arr
来源：http://wlo.shanyushiyangtech.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rsi.xuanzx.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ivx.sufxvd.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vhf.tian-w.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yob.hfpthk.cn

Go:   slices.Index(arr, x)
来源：http://ool.hesvh.cn

Ruby: arr.index(x)
来源：http://amw.shanyushiyangtech.top

C#:   list.IndexOf(x);
来源：http://uum.xinyue.icu

[D13] 过滤（保留满足条件的）
来源：http://tdp.hysaishi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jlr.zdbjq.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bzp.zhixingplan.top

JS:   arr.filter(x => x > 3)
来源：http://bpj.fehbvm.com

TS:   arr.filter(x => x > 3)
来源：http://bkg.xingfuxueyuan.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qtz.jinqigfzy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ldj.xylfe.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jyl.gotoacloud.top

C#:   list.Where(x => x > 3).ToList()
来源：http://rtp.zhiwuduotai.top

[D14] 映射转换（每个元素变形）
来源：http://fwb.guannengcc.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jjw.andypj.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dww.fzhhl.top

JS:   arr.map(x => x * 2)
来源：http://leb.zycfv.cn

TS:   arr.map(x => x * 2)
来源：http://hep.dianchejie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ajw.zdqjudy.top

Go:   // 手写循环
来源：http://sxe.sweek.top

Ruby: arr.map { |x| x * 2 }
来源：http://xpa.dashuyun.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://nye.hnxiangtu.top

[D15] 去重
来源：http://zbe.sxryk.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yqi.sjlbkw.cn

PHP:  array_unique($arr);
来源：http://ero.vqdsnc.cn

JS:   [...new Set(arr)]
来源：http://iyl.meibo888.top

TS:   [...new Set(arr)]
来源：http://yci.zhiwuduotai.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bey.xingfuxueyuan.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://kfy.hongshengwenyu.top

Ruby: arr.uniq
来源：http://rmu.hongshengwenyu.top

C#:   list.Distinct().ToList()
来源：http://oad.shanyushiyangtech.top

[D16] 求和与平均值
来源：http://ykg.meibo888.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://eyu.zdbjq.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://szg.snrcjt.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xen.sjlbkw.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://eaf.jqgufenzy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zqj.tianlin.xyz

Go:   // 手写循环累加
来源：http://kyr.nanxinkj.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pzs.gaohongyu789.top

C#:   list.Sum();  list.Average()
来源：http://wzv.cqqwz.cn

[D17] 最大值与最小值
来源：http://byw.mhx1999.top

Py:   max(arr);  min(arr)
来源：http://inm.ydjk.org.cn


<!-- 参考信息 -->