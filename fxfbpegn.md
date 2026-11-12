代发 wailian999

Py:   if not data: return
来源：http://zyg.chenjidiqi.icu

PHP:  if (!$data) { return; }
来源：http://rlj.fktsv.cn

JS:   if (!data) return;
来源：http://hon.meibo888.top

TS:   if (!data) return;
来源：http://myf.cucudq.cn

Java: if (data == null) return;
来源：http://nxl.fengsongda.top

Go:   if data == nil { return }
来源：http://egr.xuanzx.com

Ruby: return if data.nil?
来源：http://jmg.jinqigufen.top

C#:   if (data == null) return;
来源：http://qag.nanxuanxn.top

================================================================================
来源：http://ctz.yongpay.top

C. 函数与作用域
来源：http://hqk.cdnleiting.top

================================================================================
来源：http://dft.c1oappe.top

[C01] 定义函数
来源：http://uqa.quarkkingdee.top

Py:   def add(a, b): return a + b
来源：http://url.ywan-chungtsiang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://scr.pycfn.com

JS:   function add(a, b) { return a + b; }
来源：http://ouj.yongpay.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hqn.shzxlz.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://nqp.jyoumei.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ulq.feifeiyinyue.top

Ruby: def add(a, b); a + b; end
来源：http://ewq.shanyushiyangtech.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ukv.hcnkem.com

[C02] 默认参数
来源：http://iua.shuidangran.top

Py:   def greet(name="World"): return name
来源：http://lon.0kj1m.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vha.yanxiufei.cn

JS:   function greet(name = "World") { return name; }
来源：http://vrq.xuanzx.com

TS:   function greet(name: string = "World") { return name; }
来源：http://fpi.quarkkingdee.top

Java: // 无默认参数：方法重载或 Optional
来源：http://nqz.mhx1999.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://awg.shanyushiyangtech.top

Ruby: def greet(name = "World") = name
来源：http://gwc.jinghuilouyu.cn

C#:   string Greet(string name = "World") => name;
来源：http://wxy.nwbrower.top

[C03] 可变参数
来源：http://ndt.shanyushiyangkeji.top

Py:   def total(*args): return sum(args)
来源：http://sms.yonumen.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xpd.yangfankeji.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ehz.fanxiaobao.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nlr.xuetiantiany.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jys.wangdashe.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://chc.52xcode.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hiv.fehbvm.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://eyl.cashguo.top

[C04] 命名参数 / 关键字参数
来源：http://gys.cheryme.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yry.shuidangran.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lgf.cashguo.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jth.wangdashe.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sur.jianghu66.top

Java: // 无：用 Builder 模式或 record
来源：http://phb.ydzc1.top

Go:   // 无：用配置结构体参数
来源：http://utw.zhiwuduotai.top

Ruby: f(a: 1, b: 2)
来源：http://obt.yj20258888.top

C#:   f(a: 1, b: 2)
来源：http://jdr.hcnkem.com

[C05] 返回多个值
来源：http://ztv.jinyuanbaomall.cn

Py:   return a, b
来源：http://nnd.yuxming.cn

PHP:  return [$a, $b];
来源：http://ypm.birdmap.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://eoi.zycfv.cn

TS:   return { a, b };
来源：http://gpp.yueranfly.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://puq.hnxiangtu.top

Go:   return a, b
来源：http://nvr.yongpay.top

Ruby: return a, b
来源：http://ivv.nanxinkj.top

C#:   return (a, b);              // ValueTuple
来源：http://mwq.ydzc1.top

[C06] 匿名函数 / lambda
来源：http://mod.tianlin.xyz

Py:   square = lambda x: x * x
来源：http://uyh.yvedp.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wem.feifeiyinyue.top

JS:   const square = x => x * x;
来源：http://wvj.wangdashe.top

TS:   const square = (x: number): number => x * x;
来源：http://dwl.daxiang520.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ffl.jinghuilouyu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://bfc.yfazqb.com

Ruby: square = ->(x) { x * x }
来源：http://nwt.yanxiufei.cn

C#:   Func<int, int> square = x => x * x;
来源：http://dht.hfpthk.cn

[C07] 把函数作为参数传入
来源：http://ivf.andypj.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ycy.shzxlz.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ema.gogol.net.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ium.yuanzhike.top

TS:   arr.map(String)
来源：http://dgi.shanyushiyangkeji.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vcs.wangdashe.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xun.zhengqikj.top

Ruby: arr.map(&:upcase)
来源：http://cnn.fehbvm.com

C#:   arr.Select(s => s.ToUpper())
来源：http://cmz.quarkkingdee.top

[C08] 闭包
来源：http://mwo.andypj.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://stp.bbcook.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://aqm.yueranfly.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tsw.zhiwuduotai.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://msy.yj202588.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xur.yongpay.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hjp.hcnkem.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zfj.zhaomingkeji.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tne.hongshengwenyu.top

[C09] 递归
来源：http://ajw.xuanzx.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jjt.nanxuanxn.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sef.tian-w.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ysa.hywenlv.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iel.wangshuangyany.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qqy.smart0.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rtr.shangyingyoupin.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jtw.ywan-chungtsiang.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ozg.shangyingyoupin.top

[C10] 变量作用域
来源：http://htq.jinqigufen.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fyz.sysykeji.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zhe.zhongyouzk.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://acs.ydzc1.top

TS:   同 JS
来源：http://ttv.cashguo.top

Java: 方法内为块级作用域
来源：http://yhu.nanxuanxn.top

Go:   花括号块级作用域
来源：http://pfh.jiagoushi.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mcc.tianlin.xyz

C#:   块级作用域
来源：http://shh.jyoumei.cn

[C11] 模块导入与导出
来源：http://iwt.sxryk.cn

Py:   from module import func
来源：http://hzl.yuxming.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bzu.uphjek.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://ozh.jqgfzy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gon.cheryme.top

Java: import java.util.List;
来源：http://ftu.gzhubu.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rbr.dianchejie.cn

Ruby: require "json"; require_relative "./util"
来源：http://nal.zhijiandao.cn

C#:   using System.Text;
来源：http://mrm.ywan-chungtsiang.top

[C12] 立即执行函数 IIFE
来源：http://ftd.daxiang520.top

Py:   (lambda: print("run"))()
来源：http://eun.xinyue.icu

PHP:  (function () { echo "run"; })();
来源：http://mux.hfpthk.cn

JS:   (() => { console.log("run"); })();
来源：http://avv.nanxinkj.top

TS:   (() => { console.log("run"); })();
来源：http://tsy.yfazqb.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://awa.chenjidiqi.icu

Go:   func() { fmt.Println("run") }()
来源：http://iug.yj20258.top

Ruby: -> { puts "run" }.call
来源：http://zap.guowangkeji.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ljn.kuanghao11.cn

[C13] 类型声明 / 类型注解
来源：http://oik.pycfn.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lru.yongpay.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fxb.redwolf501.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lsh.yj20258888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tue.jinghuilouyu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://dmm.iojbl.cn

Go:   func add(a, b int) int
来源：http://mrw.yanxiufei.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yao.tanke756.top

C#:   int Add(int a, int b) => a + b;
来源：http://usj.fehbvm.com

[C14] 泛型函数
来源：http://nak.guannengcc.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lln.yfazqb.com

PHP:  // 无泛型
来源：http://rrh.ctjpmb.com

JS:   // 无泛型
来源：http://stu.fzhhl.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mpt.zhongyouzk.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ynb.yanxiufei.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bvw.yfazqb.com

Ruby: # 无泛型
来源：http://hlx.nanxinkj.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kkl.jqgfzy.top

[C15] 解构 / 展开参数
来源：http://qtx.yangfankeji.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xoh.yongpay.top

PHP:  [$a, $b] = $pair;
来源：http://yqa.jinqigfzy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cfx.jinghuilouyu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rue.birdmap.top

Java: // 无解构
来源：http://eto.jiagoushi.top

Go:   // 无解构
来源：http://sam.hfpthk.cn

Ruby: a, b = pair
来源：http://aeg.fzhhl.top

C#:   var (a, b) = pair;
来源：http://rqb.ivvv.top

[C16] 函数 / 方法重载
来源：http://vgy.cheryme.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ecr.jinqigfzy.top

PHP:  // 无重载
来源：http://sth.fzhhl.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://npy.yj20258.top

TS:   // 用联合类型或重载签名声明
来源：http://uie.xziqi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://vtb.jiagoushi.top

Go:   // 无重载：用不同函数名
来源：http://iox.guannengcc.top

Ruby: # 无重载：靠动态参数
来源：http://oes.gogol.net.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ncj.jqgufenzy.top

================================================================================
来源：http://hrn.cashguo.top

D. 数组 / 列表 / 集合
来源：http://kkz.vqdsnc.cn

================================================================================
来源：http://khj.guowangkeji.top

[D01] 创建数组 / 列表
来源：http://nwi.cheryme.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://nvg.dianchejie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vfv.9152youxi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://voq.zycfv.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://gas.aibaodan.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ywi.yuxming.cn

Go:   arr := []int{1, 2, 3}
来源：http://igw.gzhubu.top

Ruby: arr = [1, 2, 3]
来源：http://yqo.chenlongwang.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dwp.wangshuangyany.cn

[D02] 追加元素到末尾
来源：http://ewl.snrcjt.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://oer.nanxinkj.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://muu.yj20258888.top

JS:   arr.push(4);
来源：http://wpb.yj202588.top

TS:   arr.push(4);
来源：http://iqv.zhixingplan.top

Java: list.add(4);
来源：http://sqh.zhoulong.xyz

Go:   arr = append(arr, 4)
来源：http://xso.xuetiantiany.cn

Ruby: arr << 4; arr.push(5)
来源：http://lqu.havefunace.top

C#:   list.Add(4);
来源：http://lyk.yuanzhike.top

[D03] 在指定位置插入元素
来源：http://zpq.yfazqb.com

Py:   arr.insert(0, 0)
来源：http://bxz.sjlbkw.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kib.shzxlz.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wmp.cqqwz.cn

TS:   arr.splice(0, 0, 0);
来源：http://iar.yj20258888.top

Java: list.add(0, 0);
来源：http://xgd.fengsongda.top

Go:   arr = append([]int{0}, arr...)
来源：http://pjc.chenjidiqi.icu

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://apm.xziqi.cn

C#:   list.Insert(0, 0);
来源：http://fpi.quarkkingdee.top

[D04] 删除元素
来源：http://xss.hnxiangtu.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tun.vehdjk.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hvw.cucudq.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zhw.haohaochexian.top

TS:   arr.splice(0, 1);
来源：http://lsv.sufxvd.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://chr.jinqigufen.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://udv.yueranfly.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pxs.cheryme.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://eti.feifeiyinyue.top

[D05] 访问与修改元素
来源：http://evh.iojbl.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rgh.cqqwz.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xdi.9152youxi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ysw.birdmap.top

TS:   arr[0]; arr.at(-1);
来源：http://uhq.hcnkem.com

Java: list.get(0); list.set(0, 9);
来源：http://yzy.sufxvd.cn

Go:   arr[0]; arr[0] = 9
来源：http://cig.zhijiandao.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cyp.xuanzx.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xvh.tanke756.top

[D06] 数组长度
来源：http://wxl.xingfuxueyuan.xyz

Py:   len(arr)
来源：http://rfq.fehbvm.com

PHP:  count($arr);
来源：http://tzh.yueranfly.top

JS:   arr.length
来源：http://kqm.quarkkingdee.top

TS:   arr.length
来源：http://rov.sufxvd.cn

Java: list.size();
来源：http://pkn.fktsv.cn

Go:   len(arr)
来源：http://daw.gzhubu.top

Ruby: arr.length; arr.size
来源：http://krd.aizwys.cn

C#:   list.Count;
来源：http://uxq.wangdashe.top

[D07] 切片 / 取子数组
来源：http://kev.hywenlv.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://stz.chenjidiqi.icu

PHP:  array_slice($arr, 1, 3);
来源：http://eys.hcnkem.com

JS:   arr.slice(1, 4);
来源：http://kwy.jiagoushi.top

TS:   arr.slice(1, 4);
来源：http://hcm.aizwys.cn

Java: list.subList(1, 4);
来源：http://sqp.guannengcc.top

Go:   arr[1:4]
来源：http://zrh.yj20258.top

Ruby: arr[1, 3]
来源：http://uqq.fengsongda.top

C#:   list.GetRange(1, 3);
来源：http://tac.jiagoushi.top

[D08] 合并两个数组
来源：http://iyb.gotoacloud.top

Py:   a + b;  a.extend(b)
来源：http://ysd.yongpay.top

PHP:  array_merge($a, $b);
来源：http://tql.guannengcc.top

JS:   [...a, ...b];  a.concat(b);
来源：http://yvt.hongshengwenyu.top

TS:   [...a, ...b];
来源：http://ngg.mhx1999.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://uzs.52xcode.cn

Go:   append(a, b...)
来源：http://htw.daxiang520.top

Ruby: a + b;  a.concat(b)
来源：http://rwn.cdnleiting.top

C#:   a.Concat(b).ToList()
来源：http://ehv.zhaomingkeji.xyz

[D09] 排序（升序）
来源：http://hxa.52xcode.cn

Py:   sorted(arr);  arr.sort()
来源：http://suc.gzhubu.top

PHP:  sort($arr);
来源：http://oet.ywan-chungtsiang.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://irh.fktsv.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://rki.316326.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://sif.ivvv.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kcw.zhengqikj.top

Ruby: arr.sort
来源：http://nuq.fktsv.cn

C#:   list.Sort();
来源：http://poq.zdbjq.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://sof.chenlongwang.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://usk.quarkkingdee.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wso.aizwys.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ydt.c1oappe.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dpm.bbcook.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xer.zhaomingkeji.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hrj.meibo888.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cod.ctjpmb.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rix.sweek.top

[D11] 反转数组
来源：http://xyk.fengsongda.top

Py:   arr[::-1];  arr.reverse()
来源：http://ovj.jqgfzy.top

PHP:  array_reverse($arr);
来源：http://aos.fengsongda.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://usj.havefunace.top

TS:   [...arr].reverse();
来源：http://vwe.xziqi.cn

Java: Collections.reverse(list);
来源：http://qzm.zhoulong.xyz

Go:   slices.Reverse(arr)
来源：http://crn.cucudq.cn

Ruby: arr.reverse
来源：http://unz.uphjek.com

C#:   list.Reverse();
来源：http://mox.wangshuangyany.cn

[D12] 查找元素下标
来源：http://cgz.0kj1m.cn

Py:   arr.index(x);  x in arr
来源：http://gsi.zhixingplan.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qjd.fengsongda.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://taz.yuanzhike.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lyu.zhiwuduotai.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kwj.jianghu66.top

Go:   slices.Index(arr, x)
来源：http://xfy.9152youxi.cn

Ruby: arr.index(x)
来源：http://lpa.gaohongyu789.top

C#:   list.IndexOf(x);
来源：http://xwm.zycfv.cn

[D13] 过滤（保留满足条件的）
来源：http://hdr.nwbrower.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hgm.hesvh.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://khm.yonumen.top

JS:   arr.filter(x => x > 3)
来源：http://kee.havefunace.top

TS:   arr.filter(x => x > 3)
来源：http://oso.guowangkeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xay.wangdashe.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://plf.zhongyouzk.top

Ruby: arr.select { |x| x > 3 }
来源：http://aus.hcnkem.com

C#:   list.Where(x => x > 3).ToList()
来源：http://jjc.yuxming.cn

[D14] 映射转换（每个元素变形）
来源：http://fvi.sjlbkw.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://igr.zdqjudy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://itd.tanke756.top

JS:   arr.map(x => x * 2)
来源：http://tcx.chenzaomai.com

TS:   arr.map(x => x * 2)
来源：http://fgc.epnwcf.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://sjr.ivvv.top

Go:   // 手写循环
来源：http://vze.zdbjq.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lfe.smart0.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://rtk.ivvv.top

[D15] 去重
来源：http://cbu.smart0.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vwc.sxryk.cn

PHP:  array_unique($arr);
来源：http://cro.bbcook.cn

JS:   [...new Set(arr)]
来源：http://zrh.gogol.net.cn

TS:   [...new Set(arr)]
来源：http://atk.shanyushiyangkeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pnv.xuetiantiany.cn

Go:   // 用 map[T]struct{} 手写
来源：http://bca.zhaomingkeji.xyz

Ruby: arr.uniq
来源：http://lgu.jqgufenzy.top

C#:   list.Distinct().ToList()
来源：http://wcw.pengpengdd.cyou

[D16] 求和与平均值
来源：http://roj.hywenlv.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tbp.shanyushiyangkeji.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hym.yuanzhike.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://svj.sweek.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qgh.shzxlz.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hdo.guannengcc.top

Go:   // 手写循环累加
来源：http://rne.yueranfly.top


<!-- 参考信息 -->