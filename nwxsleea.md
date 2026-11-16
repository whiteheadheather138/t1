代发 wailian999

Java: if (data == null) return;
来源：http://zcd.andypj.xyz

Go:   if data == nil { return }
来源：http://jnj.jyoumei.cn

Ruby: return if data.nil?
来源：http://tom.fengsongda.top

C#:   if (data == null) return;
来源：http://gua.nanxinkj.top

================================================================================
来源：http://czd.yonumen.top

C. 函数与作用域
来源：http://ups.gaohongyu789.top

================================================================================
来源：http://ynn.xuanzx.com

[C01] 定义函数
来源：http://pfv.meibo888.top

Py:   def add(a, b): return a + b
来源：http://tbj.hfpthk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uoo.yuanzhike.top

JS:   function add(a, b) { return a + b; }
来源：http://fty.guowangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://umg.ppjwa.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://iob.tanke756.top

Go:   func add(a, b int) int { return a + b }
来源：http://ltp.yonumen.top

Ruby: def add(a, b); a + b; end
来源：http://jov.zhixingplan.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rvi.guowangkeji.top

[C02] 默认参数
来源：http://qno.guannengcc.top

Py:   def greet(name="World"): return name
来源：http://rdy.jyoumei.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://eqm.hongshengwenyu.top

JS:   function greet(name = "World") { return name; }
来源：http://jux.yj20258888.top

TS:   function greet(name: string = "World") { return name; }
来源：http://cda.aizwys.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://eka.hysaishi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ffo.jqgfzy.top

Ruby: def greet(name = "World") = name
来源：http://vyz.sjlbkw.cn

C#:   string Greet(string name = "World") => name;
来源：http://qwt.aizwys.cn

[C03] 可变参数
来源：http://rjf.sjlbkw.cn

Py:   def total(*args): return sum(args)
来源：http://aur.zdbjq.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vyl.xingfuxueyuan.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bkt.guowangkeji.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wwn.ehwqpu.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ibq.ybcxt.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tii.jinyuanbaomall.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hzu.yj20258.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wyw.andypj.xyz

[C04] 命名参数 / 关键字参数
来源：http://ewa.zdbjq.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vkw.yj20258.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qjm.xingfuxueyuan.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://htl.jinghuilouyu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bgz.birdmap.top

Java: // 无：用 Builder 模式或 record
来源：http://ijr.xuetiantiany.cn

Go:   // 无：用配置结构体参数
来源：http://nye.zhongyouzk.top

Ruby: f(a: 1, b: 2)
来源：http://knb.zhongyouzk.top

C#:   f(a: 1, b: 2)
来源：http://dod.zhaomingkeji.xyz

[C05] 返回多个值
来源：http://vyz.52xcode.cn

Py:   return a, b
来源：http://auz.yuanzhike.top

PHP:  return [$a, $b];
来源：http://cfi.cdnleiting.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://mal.pycfn.com

TS:   return { a, b };
来源：http://keb.zhengqikj.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bja.yongpay.top

Go:   return a, b
来源：http://pqq.jinyuanbaomall.cn

Ruby: return a, b
来源：http://jki.yuxming.cn

C#:   return (a, b);              // ValueTuple
来源：http://qtl.pengpengdd.cyou

[C06] 匿名函数 / lambda
来源：http://heo.ctjpmb.com

Py:   square = lambda x: x * x
来源：http://qaw.hesvh.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://iic.zhongyouzk.top

JS:   const square = x => x * x;
来源：http://cnq.birdmap.top

TS:   const square = (x: number): number => x * x;
来源：http://zoo.birdmap.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dqt.fanxiaobao.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://xif.sysykeji.top

Ruby: square = ->(x) { x * x }
来源：http://mfg.shanyushiyangtech.top

C#:   Func<int, int> square = x => x * x;
来源：http://wld.jqgfzy.top

[C07] 把函数作为参数传入
来源：http://zrl.uphjek.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lpk.tarul.cn

PHP:  array_map("strtoupper", $arr);
来源：http://qrw.jinqigufen.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://osz.cqqwz.cn

TS:   arr.map(String)
来源：http://csq.yj202588.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gqy.yvedp.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://axt.nwbrower.top

Ruby: arr.map(&:upcase)
来源：http://ieh.pycfn.com

C#:   arr.Select(s => s.ToUpper())
来源：http://qkv.xingfuxueyuan.xyz

[C08] 闭包
来源：http://jht.xziqi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qbe.aizwys.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lhq.wangdashe.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://col.jinqigufen.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nms.vqdsnc.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dzl.cheryme.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://uuk.tarul.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://utx.fehbvm.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mdz.yvedp.cn

[C09] 递归
来源：http://eho.fengsongda.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hfi.sysykeji.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fdz.fengsongda.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yui.jinyuanbaomall.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xna.zdbjq.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sar.fktsv.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ryj.yuanzhike.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xtz.jiagoushi.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ggd.jinghuilouyu.cn

[C10] 变量作用域
来源：http://axr.cheryme.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dyp.tarul.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nbg.ctjpmb.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gor.yj202588.top

TS:   同 JS
来源：http://ihk.chenjidiqi.icu

Java: 方法内为块级作用域
来源：http://rjs.52xcode.cn

Go:   花括号块级作用域
来源：http://fod.daxiang520.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nbu.pengpengdd.cyou

C#:   块级作用域
来源：http://tei.yvedp.cn

[C11] 模块导入与导出
来源：http://ojw.yj202588.top

Py:   from module import func
来源：http://yhj.cashguo.top

PHP:  require "file.php";  或 use App\Service;
来源：http://dlt.cqqwz.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://adi.zhoulong.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pok.hfpthk.cn

Java: import java.util.List;
来源：http://nbv.ydzc1.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lzi.cdnleiting.top

Ruby: require "json"; require_relative "./util"
来源：http://vqc.cucudq.cn

C#:   using System.Text;
来源：http://vae.vqdsnc.cn

[C12] 立即执行函数 IIFE
来源：http://nou.zhaomingkeji.xyz

Py:   (lambda: print("run"))()
来源：http://vvr.xuanzx.com

PHP:  (function () { echo "run"; })();
来源：http://cgc.kuanghao11.cn

JS:   (() => { console.log("run"); })();
来源：http://fsq.zdbjq.cn

TS:   (() => { console.log("run"); })();
来源：http://hmm.cdnleiting.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jqp.sweek.top

Go:   func() { fmt.Println("run") }()
来源：http://qdk.xinyue.icu

Ruby: -> { puts "run" }.call
来源：http://dwm.hywenlv.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://llj.bbcook.cn

[C13] 类型声明 / 类型注解
来源：http://bcw.yfazqb.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qhs.jlsjyb.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fzg.wangdashe.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ieh.ctjpmb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qvg.fzhhl.top

Java: int add(int a, int b) { return a + b; }
来源：http://nlx.smart0.xyz

Go:   func add(a, b int) int
来源：http://dmu.cqqwz.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://uiz.birdmap.top

C#:   int Add(int a, int b) => a + b;
来源：http://xvw.yangfankeji.com

[C14] 泛型函数
来源：http://gmi.hesvh.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ovx.shangyingyoupin.top

PHP:  // 无泛型
来源：http://oot.cdnleiting.top

JS:   // 无泛型
来源：http://xeh.fehbvm.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zxw.sweek.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xuh.hfpthk.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ayr.dashuyun.cn

Ruby: # 无泛型
来源：http://lam.havefunace.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ncc.jinqigufen.top

[C15] 解构 / 展开参数
来源：http://kiu.shanyushiyangkeji.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://aos.haohaochexian.top

PHP:  [$a, $b] = $pair;
来源：http://quz.c1oappe.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://eyf.ydjk.org.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://thr.chenjidiqi.icu

Java: // 无解构
来源：http://lqn.wangshuangyany.cn

Go:   // 无解构
来源：http://ome.uphjek.com

Ruby: a, b = pair
来源：http://zna.quarkkingdee.top

C#:   var (a, b) = pair;
来源：http://dyk.nanxuanxn.top

[C16] 函数 / 方法重载
来源：http://mqe.ehwqpu.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dgt.snrcjt.cn

PHP:  // 无重载
来源：http://icz.hywenlv.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://erd.guowangkeji.top

TS:   // 用联合类型或重载签名声明
来源：http://hdj.zhongyouzk.top

Java: void f(int a) {}  void f(String a) {}
来源：http://uuj.gaohongyu789.top

Go:   // 无重载：用不同函数名
来源：http://imz.52xcode.cn

Ruby: # 无重载：靠动态参数
来源：http://elq.nanxuanxn.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://tsp.gogol.net.cn

================================================================================
来源：http://gvk.zhixingplan.top

D. 数组 / 列表 / 集合
来源：http://cmc.yuxming.cn

================================================================================
来源：http://tjj.fanxiaobao.xyz

[D01] 创建数组 / 列表
来源：http://ddx.yongpay.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://mxf.wangshuangyany.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://evh.andypj.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qsv.jyoumei.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://edk.redwolf501.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wyr.jqgfzy.top

Go:   arr := []int{1, 2, 3}
来源：http://lto.hnxiangtu.top

Ruby: arr = [1, 2, 3]
来源：http://qhb.kuanghao11.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://omk.ppjwa.cn

[D02] 追加元素到末尾
来源：http://olp.shangyingyoupin.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://etj.hysaishi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mkt.uphjek.com

JS:   arr.push(4);
来源：http://mvm.cqqwz.cn

TS:   arr.push(4);
来源：http://moi.ehwqpu.com

Java: list.add(4);
来源：http://ucb.shuidangran.top

Go:   arr = append(arr, 4)
来源：http://wuj.aibaodan.cn

Ruby: arr << 4; arr.push(5)
来源：http://kac.ybcxt.top

C#:   list.Add(4);
来源：http://tvz.ywan-chungtsiang.top

[D03] 在指定位置插入元素
来源：http://cml.jqgufenzy.top

Py:   arr.insert(0, 0)
来源：http://aic.zhaomingkeji.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://udd.mhx1999.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hoz.jlsjyb.cn

TS:   arr.splice(0, 0, 0);
来源：http://siz.fengsongda.top

Java: list.add(0, 0);
来源：http://qpw.zhoulong.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://ddc.chenzaomai.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tkr.vqdsnc.cn

C#:   list.Insert(0, 0);
来源：http://mnc.hnqzz.top

[D04] 删除元素
来源：http://rib.ehwqpu.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uqa.chenlongwang.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gdu.ehwqpu.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gvi.zhijiandao.cn

TS:   arr.splice(0, 1);
来源：http://gsk.ivvv.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rhj.chenlongwang.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hew.yj202588.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hpr.pengpengdd.cyou

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xne.svipenyu.cn

[D05] 访问与修改元素
来源：http://jec.hammf.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cua.jinqigfzy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qzy.yuxming.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://utc.nanxinkj.top

TS:   arr[0]; arr.at(-1);
来源：http://nof.c1oappe.top

Java: list.get(0); list.set(0, 9);
来源：http://mvz.zdbjq.cn

Go:   arr[0]; arr[0] = 9
来源：http://zmh.andypj.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xbs.sxryk.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jlv.zdqjudy.top

[D06] 数组长度
来源：http://vcf.cqqwz.cn

Py:   len(arr)
来源：http://soj.havefunace.top

PHP:  count($arr);
来源：http://xxb.fehbvm.com

JS:   arr.length
来源：http://jaf.316326.xyz

TS:   arr.length
来源：http://grs.cashguo.top

Java: list.size();
来源：http://pid.jinqigfzy.top

Go:   len(arr)
来源：http://nxs.0kj1m.cn

Ruby: arr.length; arr.size
来源：http://euf.andypj.xyz

C#:   list.Count;
来源：http://ogp.gzhubu.top

[D07] 切片 / 取子数组
来源：http://qly.nwbrower.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vcj.zdqjudy.top

PHP:  array_slice($arr, 1, 3);
来源：http://vic.jyoumei.cn

JS:   arr.slice(1, 4);
来源：http://oiv.ydjk.org.cn

TS:   arr.slice(1, 4);
来源：http://cyn.sufxvd.cn

Java: list.subList(1, 4);
来源：http://khi.shanyushiyangkeji.top

Go:   arr[1:4]
来源：http://pvx.dashuyun.cn

Ruby: arr[1, 3]
来源：http://xio.sysykeji.top

C#:   list.GetRange(1, 3);
来源：http://gon.ybcxt.top

[D08] 合并两个数组
来源：http://phx.svipenyu.cn

Py:   a + b;  a.extend(b)
来源：http://bfd.yongpay.top

PHP:  array_merge($a, $b);
来源：http://jwk.0kj1m.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://izp.jqgfzy.top

TS:   [...a, ...b];
来源：http://apc.xuanzx.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jce.havefunace.top

Go:   append(a, b...)
来源：http://uym.bjfxy.top

Ruby: a + b;  a.concat(b)
来源：http://tuo.9152youxi.cn

C#:   a.Concat(b).ToList()
来源：http://qpl.wangdashe.top

[D09] 排序（升序）
来源：http://buo.havefunace.top

Py:   sorted(arr);  arr.sort()
来源：http://gwz.meibo888.top

PHP:  sort($arr);
来源：http://oha.hcnkem.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qno.ppjwa.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://clc.shzxlz.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vdh.316326.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://coh.aizwys.cn

Ruby: arr.sort
来源：http://djz.shzxlz.cn

C#:   list.Sort();
来源：http://xss.yj20258.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://zoy.fktsv.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wkv.sufxvd.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dre.jianghu66.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ngv.yvedp.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gsk.xziqi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xzx.yangfankeji.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vbw.sjlbkw.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://twq.pengpengdd.cyou

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yxf.ywan-chungtsiang.top

[D11] 反转数组
来源：http://glp.shzxlz.cn

Py:   arr[::-1];  arr.reverse()
来源：http://jcz.dashuyun.cn

PHP:  array_reverse($arr);
来源：http://pqo.vehdjk.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://omj.hongshengwenyu.top

TS:   [...arr].reverse();
来源：http://kjd.guannengcc.top

Java: Collections.reverse(list);
来源：http://ffc.xingfuxueyuan.xyz

Go:   slices.Reverse(arr)
来源：http://ceh.fengsongda.top

Ruby: arr.reverse
来源：http://jxf.chenlongwang.top

C#:   list.Reverse();
来源：http://ogq.xuetiantiany.cn

[D12] 查找元素下标
来源：http://wwi.iojbl.cn

Py:   arr.index(x);  x in arr
来源：http://nuh.shangyingyoupin.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gjc.sjlbkw.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://huq.ctjpmb.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rxa.fengsongda.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ddp.gogol.net.cn

Go:   slices.Index(arr, x)
来源：http://amu.dianchejie.cn

Ruby: arr.index(x)
来源：http://yth.316326.xyz

C#:   list.IndexOf(x);
来源：http://vpa.vehdjk.com

[D13] 过滤（保留满足条件的）
来源：http://fgj.yuanzhike.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sep.pengpengdd.cyou

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bhh.xinyue.icu

JS:   arr.filter(x => x > 3)
来源：http://zhf.yvedp.cn

TS:   arr.filter(x => x > 3)
来源：http://iav.zhoulong.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://prz.dashuyun.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dxd.fanxiaobao.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://sux.bbcook.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://omq.yj202588.top

[D14] 映射转换（每个元素变形）
来源：http://dme.yj20258.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://urk.yonumen.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mjf.yj20258.top

JS:   arr.map(x => x * 2)
来源：http://ifm.fanxiaobao.xyz

TS:   arr.map(x => x * 2)
来源：http://pup.kuanghao11.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sbq.hywenlv.cn

Go:   // 手写循环
来源：http://uct.tianlin.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://czd.yj20258.top

C#:   list.Select(x => x * 2).ToList()
来源：http://zeg.daxiang520.top

[D15] 去重
来源：http://aqf.gogol.net.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vqe.fzhhl.top

PHP:  array_unique($arr);
来源：http://xda.hysaishi.cn

JS:   [...new Set(arr)]
来源：http://rss.yj202588.top

TS:   [...new Set(arr)]
来源：http://wcr.9152youxi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://msu.dashuyun.cn

Go:   // 用 map[T]struct{} 手写
来源：http://dhh.nanxuanxn.top

Ruby: arr.uniq
来源：http://roe.bbcook.cn

C#:   list.Distinct().ToList()
来源：http://adf.aibaodan.cn

[D16] 求和与平均值
来源：http://ftu.fengsongda.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jyi.xuanzx.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jrw.smart0.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://uij.sxryk.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lcs.haohaochexian.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xzp.yuanzhike.top

Go:   // 手写循环累加
来源：http://waa.shzxlz.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pbz.epnwcf.com

C#:   list.Sum();  list.Average()
来源：http://equ.sweek.top

[D17] 最大值与最小值
来源：http://qbe.hywenlv.cn

Py:   max(arr);  min(arr)
来源：http://nat.haohaochexian.top


<!-- 参考信息 -->