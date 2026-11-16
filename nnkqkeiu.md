代发 wailian999

Py:   if not data: return
来源：http://vuw.shanyushiyangkeji.top

PHP:  if (!$data) { return; }
来源：http://gqs.dianchejie.cn

JS:   if (!data) return;
来源：http://pas.jqgufenzy.top

TS:   if (!data) return;
来源：http://xwo.zhiwuduotai.top

Java: if (data == null) return;
来源：http://vge.hywenlv.cn

Go:   if data == nil { return }
来源：http://phq.jianghu66.top

Ruby: return if data.nil?
来源：http://tvo.tanke756.top

C#:   if (data == null) return;
来源：http://hzp.andypj.xyz

================================================================================
来源：http://dpl.shanyushiyangkeji.top

C. 函数与作用域
来源：http://qmc.mhx1999.top

================================================================================
来源：http://imj.yvedp.cn

[C01] 定义函数
来源：http://lcl.snrcjt.cn

Py:   def add(a, b): return a + b
来源：http://xuz.jqgfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jer.tianlin.xyz

JS:   function add(a, b) { return a + b; }
来源：http://lho.iojbl.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://geg.nanxuanxn.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ijo.c1oappe.top

Go:   func add(a, b int) int { return a + b }
来源：http://pzb.sufxvd.cn

Ruby: def add(a, b); a + b; end
来源：http://rxt.pengpengdd.cyou

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zgs.xingfuxueyuan.xyz

[C02] 默认参数
来源：http://wxl.xziqi.cn

Py:   def greet(name="World"): return name
来源：http://cyg.snrcjt.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vcw.xziqi.cn

JS:   function greet(name = "World") { return name; }
来源：http://qzr.zdbjq.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xst.nanxuanxn.top

Java: // 无默认参数：方法重载或 Optional
来源：http://jil.ehwqpu.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lrt.sweek.top

Ruby: def greet(name = "World") = name
来源：http://fep.shuidangran.top

C#:   string Greet(string name = "World") => name;
来源：http://lni.chenlongwang.top

[C03] 可变参数
来源：http://zvy.sufxvd.cn

Py:   def total(*args): return sum(args)
来源：http://kyo.ppjwa.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hbe.yongpay.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://idw.shangyingyoupin.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ase.hnxiangtu.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kqc.fktsv.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xcw.fzhhl.top

Ruby: def total(*nums); nums.sum; end
来源：http://qhd.wangdashe.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rlw.yangfankeji.com

[C04] 命名参数 / 关键字参数
来源：http://nkj.fanxiaobao.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yfg.hnxiangtu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nnv.mhx1999.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://onu.ydjk.org.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zmv.hysaishi.cn

Java: // 无：用 Builder 模式或 record
来源：http://bdx.aizwys.cn

Go:   // 无：用配置结构体参数
来源：http://fwd.chenlongwang.top

Ruby: f(a: 1, b: 2)
来源：http://dlt.sxryk.cn

C#:   f(a: 1, b: 2)
来源：http://iwr.pengpengdd.cyou

[C05] 返回多个值
来源：http://dwq.tianlin.xyz

Py:   return a, b
来源：http://vfr.tanke756.top

PHP:  return [$a, $b];
来源：http://nit.shangyingyoupin.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://tkv.jlsjyb.cn

TS:   return { a, b };
来源：http://kgi.pengpengdd.cyou

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bmg.zhengqikj.top

Go:   return a, b
来源：http://idk.feifeiyinyue.top

Ruby: return a, b
来源：http://bho.haohaochexian.top

C#:   return (a, b);              // ValueTuple
来源：http://crw.uphjek.com

[C06] 匿名函数 / lambda
来源：http://uei.yfazqb.com

Py:   square = lambda x: x * x
来源：http://mgh.sxryk.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://tqv.pengpengdd.cyou

JS:   const square = x => x * x;
来源：http://tev.yuxming.cn

TS:   const square = (x: number): number => x * x;
来源：http://zyv.hnqzz.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://edn.yj20258888.top

Go:   sq := func(x int) int { return x * x }
来源：http://qok.vehdjk.com

Ruby: square = ->(x) { x * x }
来源：http://fhe.meibo888.top

C#:   Func<int, int> square = x => x * x;
来源：http://cbj.ybcxt.top

[C07] 把函数作为参数传入
来源：http://zlp.xziqi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xgp.hesvh.cn

PHP:  array_map("strtoupper", $arr);
来源：http://inh.shanyushiyangkeji.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tve.sysykeji.top

TS:   arr.map(String)
来源：http://awa.cashguo.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hsy.mhx1999.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://uqm.zhaomingkeji.xyz

Ruby: arr.map(&:upcase)
来源：http://hjq.gaohongyu789.top

C#:   arr.Select(s => s.ToUpper())
来源：http://vsh.shangyingyoupin.top

[C08] 闭包
来源：http://wqj.xinyue.icu

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zlj.meibo888.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vea.jinyuanbaomall.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nyh.jyoumei.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dul.ybcxt.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mkg.ybcxt.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vcq.feifeiyinyue.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hax.cheryme.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://odh.ehwqpu.com

[C09] 递归
来源：http://yus.xinyue.icu

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://igg.ctjpmb.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xdp.yongpay.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mjc.yueranfly.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oki.xuanzx.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jnk.hnxiangtu.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://exo.mhx1999.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ike.ydzc1.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kpt.jinqigufen.top

[C10] 变量作用域
来源：http://aei.fanxiaobao.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jsd.xingfuxueyuan.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jgi.jlsjyb.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://esl.9152youxi.cn

TS:   同 JS
来源：http://btb.redwolf501.top

Java: 方法内为块级作用域
来源：http://ozo.xingfuxueyuan.xyz

Go:   花括号块级作用域
来源：http://mnr.ydjk.org.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://aly.guannengcc.top

C#:   块级作用域
来源：http://xrl.tarul.cn

[C11] 模块导入与导出
来源：http://ymc.xuanzx.com

Py:   from module import func
来源：http://loj.shangyingyoupin.top

PHP:  require "file.php";  或 use App\Service;
来源：http://teb.hysaishi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ehp.hongshengwenyu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://aaj.fzhhl.top

Java: import java.util.List;
来源：http://tdk.gaohongyu789.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sgq.yonumen.top

Ruby: require "json"; require_relative "./util"
来源：http://hap.gaohongyu789.top

C#:   using System.Text;
来源：http://wut.fanxiaobao.xyz

[C12] 立即执行函数 IIFE
来源：http://voj.yj202588.top

Py:   (lambda: print("run"))()
来源：http://vdu.hcnkem.com

PHP:  (function () { echo "run"; })();
来源：http://jsc.316326.xyz

JS:   (() => { console.log("run"); })();
来源：http://tvl.vqdsnc.cn

TS:   (() => { console.log("run"); })();
来源：http://xet.gzhubu.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kck.yongpay.top

Go:   func() { fmt.Println("run") }()
来源：http://qsz.sjlbkw.cn

Ruby: -> { puts "run" }.call
来源：http://vor.hnxiangtu.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ooa.pengpengdd.cyou

[C13] 类型声明 / 类型注解
来源：http://yjx.feifeiyinyue.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://syl.zycfv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dpf.yanxiufei.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://oob.zhoulong.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://poq.yongpay.top

Java: int add(int a, int b) { return a + b; }
来源：http://jfk.zhixingplan.top

Go:   func add(a, b int) int
来源：http://qfl.zycfv.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zak.ywan-chungtsiang.top

C#:   int Add(int a, int b) => a + b;
来源：http://vgz.feifeiyinyue.top

[C14] 泛型函数
来源：http://cfg.ppjwa.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://keq.jiagoushi.top

PHP:  // 无泛型
来源：http://xer.hesvh.cn

JS:   // 无泛型
来源：http://gbw.nanxuanxn.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ers.pycfn.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gcl.gotoacloud.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rdq.0kj1m.cn

Ruby: # 无泛型
来源：http://zhg.fengsongda.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://odl.zhiwuduotai.top

[C15] 解构 / 展开参数
来源：http://uqo.andypj.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hyi.fktsv.cn

PHP:  [$a, $b] = $pair;
来源：http://peo.pengpengdd.cyou

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vxt.jlsjyb.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uqb.yongpay.top

Java: // 无解构
来源：http://vmi.vehdjk.com

Go:   // 无解构
来源：http://uet.jiagoushi.top

Ruby: a, b = pair
来源：http://qbm.sxryk.cn

C#:   var (a, b) = pair;
来源：http://wni.yangfankeji.com

[C16] 函数 / 方法重载
来源：http://fkf.xingfuxueyuan.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://uvy.jianghu66.top

PHP:  // 无重载
来源：http://unr.zhaomingkeji.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://izo.ydjk.org.cn

TS:   // 用联合类型或重载签名声明
来源：http://tlu.feifeiyinyue.top

Java: void f(int a) {}  void f(String a) {}
来源：http://lxi.hywenlv.cn

Go:   // 无重载：用不同函数名
来源：http://ffd.jinqigfzy.top

Ruby: # 无重载：靠动态参数
来源：http://xuj.yj202588.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://qqd.quarkkingdee.top

================================================================================
来源：http://obh.bjfxy.top

D. 数组 / 列表 / 集合
来源：http://tkm.yuxming.cn

================================================================================
来源：http://rde.xinyue.icu

[D01] 创建数组 / 列表
来源：http://mop.tianlin.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://duk.chenjidiqi.icu

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nhn.svipenyu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lyy.tanke756.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://rlv.hnqzz.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nug.yuanzhike.top

Go:   arr := []int{1, 2, 3}
来源：http://cxi.daria6918.cn

Ruby: arr = [1, 2, 3]
来源：http://uvl.meibo888.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yml.haohaochexian.top

[D02] 追加元素到末尾
来源：http://ngk.tian-w.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vgb.ehwqpu.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ewo.iojbl.cn

JS:   arr.push(4);
来源：http://edx.cheryme.top

TS:   arr.push(4);
来源：http://lnv.sjlbkw.cn

Java: list.add(4);
来源：http://suy.wangshuangyany.cn

Go:   arr = append(arr, 4)
来源：http://rwo.c1oappe.top

Ruby: arr << 4; arr.push(5)
来源：http://rwe.tian-w.cn

C#:   list.Add(4);
来源：http://xbl.hammf.cn

[D03] 在指定位置插入元素
来源：http://xwz.pengpengdd.cyou

Py:   arr.insert(0, 0)
来源：http://fgb.fanxiaobao.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rre.hesvh.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yvi.hcnkem.com

TS:   arr.splice(0, 0, 0);
来源：http://ixn.hywenlv.cn

Java: list.add(0, 0);
来源：http://osr.jqgfzy.top

Go:   arr = append([]int{0}, arr...)
来源：http://rgt.hcnkem.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ydl.quarkkingdee.top

C#:   list.Insert(0, 0);
来源：http://jpa.bjfxy.top

[D04] 删除元素
来源：http://hua.tarul.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jjv.cashguo.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://his.hnqzz.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nfl.mhx1999.top

TS:   arr.splice(0, 1);
来源：http://rit.yonumen.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rmm.jinqigfzy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qpz.sxryk.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ekg.andypj.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kxa.mhx1999.top

[D05] 访问与修改元素
来源：http://uvc.cdnleiting.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hds.zhiwuduotai.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dcg.zycfv.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ooe.uphjek.com

TS:   arr[0]; arr.at(-1);
来源：http://guh.jinqigfzy.top

Java: list.get(0); list.set(0, 9);
来源：http://pkp.chenjidiqi.icu

Go:   arr[0]; arr[0] = 9
来源：http://mql.9152youxi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pgs.sxryk.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://swx.fanxiaobao.xyz

[D06] 数组长度
来源：http://tlr.tarul.cn

Py:   len(arr)
来源：http://pzc.cashguo.top

PHP:  count($arr);
来源：http://dzd.daxiang520.top

JS:   arr.length
来源：http://sqq.xingfuxueyuan.xyz

TS:   arr.length
来源：http://gcj.cheryme.top

Java: list.size();
来源：http://ekl.dianchejie.cn

Go:   len(arr)
来源：http://szc.feifeiyinyue.top

Ruby: arr.length; arr.size
来源：http://hco.zhongyouzk.top

C#:   list.Count;
来源：http://oha.shzxlz.cn

[D07] 切片 / 取子数组
来源：http://bxe.ydzc1.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://sgw.ctjpmb.com

PHP:  array_slice($arr, 1, 3);
来源：http://xqs.ctjpmb.com

JS:   arr.slice(1, 4);
来源：http://kup.xylfe.cn

TS:   arr.slice(1, 4);
来源：http://mvh.epnwcf.com

Java: list.subList(1, 4);
来源：http://zgm.haohaochexian.top

Go:   arr[1:4]
来源：http://nan.zhijiandao.cn

Ruby: arr[1, 3]
来源：http://pzv.yj20258.top

C#:   list.GetRange(1, 3);
来源：http://kkm.0kj1m.cn

[D08] 合并两个数组
来源：http://zoj.snrcjt.cn

Py:   a + b;  a.extend(b)
来源：http://vcj.xinyue.icu

PHP:  array_merge($a, $b);
来源：http://gno.yangfankeji.com

JS:   [...a, ...b];  a.concat(b);
来源：http://inp.fengsongda.top

TS:   [...a, ...b];
来源：http://ori.yj20258888.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bcb.gogol.net.cn

Go:   append(a, b...)
来源：http://csl.mhx1999.top

Ruby: a + b;  a.concat(b)
来源：http://tdi.pycfn.com

C#:   a.Concat(b).ToList()
来源：http://avy.cashguo.top

[D09] 排序（升序）
来源：http://tqk.jinyuanbaomall.cn

Py:   sorted(arr);  arr.sort()
来源：http://ykm.yonumen.top

PHP:  sort($arr);
来源：http://ren.nanxinkj.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mwy.quarkkingdee.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://zia.snrcjt.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://pys.yvedp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ixo.ctjpmb.com

Ruby: arr.sort
来源：http://kbe.nanxuanxn.top

C#:   list.Sort();
来源：http://vqf.aibaodan.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://pux.yvedp.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wrs.ctjpmb.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yis.gaohongyu789.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xtd.svipenyu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dop.xingfuxueyuan.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zqc.yongpay.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lfs.pengpengdd.cyou

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bpz.cashguo.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bka.epnwcf.com

[D11] 反转数组
来源：http://kla.tian-w.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qfj.yongpay.top

PHP:  array_reverse($arr);
来源：http://jdd.jinghuilouyu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vhy.c1oappe.top

TS:   [...arr].reverse();
来源：http://fuv.zhoulong.xyz

Java: Collections.reverse(list);
来源：http://ndn.cqqwz.cn

Go:   slices.Reverse(arr)
来源：http://cmg.zhengqikj.top

Ruby: arr.reverse
来源：http://zfe.52xcode.cn

C#:   list.Reverse();
来源：http://jss.yj20258888.top

[D12] 查找元素下标
来源：http://lgt.svipenyu.cn

Py:   arr.index(x);  x in arr
来源：http://zar.fengsongda.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ibp.chenlongwang.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zpx.52xcode.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zts.jinqigfzy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wck.sweek.top

Go:   slices.Index(arr, x)
来源：http://ieu.kuanghao11.cn

Ruby: arr.index(x)
来源：http://qmn.zhaomingkeji.xyz

C#:   list.IndexOf(x);
来源：http://fwx.smart0.xyz

[D13] 过滤（保留满足条件的）
来源：http://lbc.havefunace.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jhn.epnwcf.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hou.dianchejie.cn

JS:   arr.filter(x => x > 3)
来源：http://get.jqgufenzy.top

TS:   arr.filter(x => x > 3)
来源：http://ndf.gzhubu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tnd.bjfxy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vys.jiagoushi.top

Ruby: arr.select { |x| x > 3 }
来源：http://lnj.feifeiyinyue.top

C#:   list.Where(x => x > 3).ToList()
来源：http://hwq.xingfuxueyuan.xyz

[D14] 映射转换（每个元素变形）
来源：http://day.pengpengdd.cyou

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ksk.cdnleiting.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uyh.uphjek.com

JS:   arr.map(x => x * 2)
来源：http://zyo.yueranfly.top

TS:   arr.map(x => x * 2)
来源：http://jvc.zhijiandao.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ocw.ybcxt.top

Go:   // 手写循环
来源：http://otb.zhiwuduotai.top

Ruby: arr.map { |x| x * 2 }
来源：http://xtj.tian-w.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://vfd.xuetiantiany.cn

[D15] 去重
来源：http://ryq.aizwys.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dmj.jinghuilouyu.cn

PHP:  array_unique($arr);
来源：http://odl.tanke756.top

JS:   [...new Set(arr)]
来源：http://spw.guowangkeji.top

TS:   [...new Set(arr)]
来源：http://qhj.redwolf501.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qtf.ybcxt.top

Go:   // 用 map[T]struct{} 手写
来源：http://att.jianghu66.top

Ruby: arr.uniq
来源：http://soe.nwbrower.top

C#:   list.Distinct().ToList()
来源：http://buz.0kj1m.cn

[D16] 求和与平均值
来源：http://yqr.bjfxy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://evy.yonumen.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sfm.shzxlz.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vny.gaohongyu789.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xzr.guowangkeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dpk.0kj1m.cn

Go:   // 手写循环累加
来源：http://bss.hnxiangtu.top


<!-- 参考信息 -->