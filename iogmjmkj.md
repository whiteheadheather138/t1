代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uph.yfazqb.com

Java: x instanceof Number
来源：http://rhe.chenjidiqi.icu

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zlv.nwbrower.top

Ruby: x.is_a?(Numeric)
来源：http://nkf.zhengqikj.top

C#:   x is int or double or decimal
来源：http://qqb.jqgufenzy.top

[B14] 判断值是否在集合内
来源：http://jya.meibo888.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ula.hcnkem.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xkj.sweek.top

JS:   [1, 2, 3].includes(x)
来源：http://jmh.gotoacloud.top

TS:   [1, 2, 3].includes(x)
来源：http://zcn.xziqi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vnf.jinqigfzy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bec.gaohongyu789.top

Ruby: [1, 2, 3].include?(x)
来源：http://bbd.ydjk.org.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mad.zhixingplan.top

[B15] 布尔运算与取反
来源：http://tur.jqgufenzy.top

Py:   a and b or not c
来源：http://vph.havefunace.top

PHP:  $a && $b || !$c
来源：http://mbu.daria6918.cn

JS:   a && b || !c
来源：http://nlq.316326.xyz

TS:   a && b || !c
来源：http://wmm.jlsjyb.cn

Java: a && b || !c
来源：http://awg.tian-w.cn

Go:   a && b || !c
来源：http://qhs.tanke756.top

Ruby: a && b || !c
来源：http://evw.cdnleiting.top

C#:   a && b || !c
来源：http://buy.nwbrower.top

[B16] 卫语句：不满足条件提前返回
来源：http://cut.yj20258.top

Py:   if not data: return
来源：http://dba.redwolf501.top

PHP:  if (!$data) { return; }
来源：http://nba.ydzc1.top

JS:   if (!data) return;
来源：http://dox.yvedp.cn

TS:   if (!data) return;
来源：http://ejt.yj202588.top

Java: if (data == null) return;
来源：http://yqq.ybcxt.top

Go:   if data == nil { return }
来源：http://yev.tanke756.top

Ruby: return if data.nil?
来源：http://hyj.yj202588.top

C#:   if (data == null) return;
来源：http://jaj.guannengcc.top

================================================================================
来源：http://dhu.bbcook.cn

C. 函数与作用域
来源：http://jau.zdbjq.cn

================================================================================
来源：http://xla.zhoulong.xyz

[C01] 定义函数
来源：http://yqs.shzxlz.cn

Py:   def add(a, b): return a + b
来源：http://uuv.tarul.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dzs.ppjwa.cn

JS:   function add(a, b) { return a + b; }
来源：http://lup.zhijiandao.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fdx.daxiang520.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ark.tanke756.top

Go:   func add(a, b int) int { return a + b }
来源：http://nie.jinqigfzy.top

Ruby: def add(a, b); a + b; end
来源：http://tmc.xziqi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://awx.ydjk.org.cn

[C02] 默认参数
来源：http://rqq.daxiang520.top

Py:   def greet(name="World"): return name
来源：http://tfd.ywan-chungtsiang.top

PHP:  function greet($name = "World") { return $name; }
来源：http://jtd.hesvh.cn

JS:   function greet(name = "World") { return name; }
来源：http://npw.mhx1999.top

TS:   function greet(name: string = "World") { return name; }
来源：http://hml.sxryk.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jtd.gotoacloud.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://iuj.ydjk.org.cn

Ruby: def greet(name = "World") = name
来源：http://vjd.svipenyu.cn

C#:   string Greet(string name = "World") => name;
来源：http://ffs.yfazqb.com

[C03] 可变参数
来源：http://cll.tian-w.cn

Py:   def total(*args): return sum(args)
来源：http://qdz.gzhubu.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dkw.9152youxi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tvh.jlsjyb.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ykc.9152youxi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ooh.vqdsnc.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hjl.9152youxi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://czm.yuxming.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yyt.tianlin.xyz

[C04] 命名参数 / 关键字参数
来源：http://xtj.hongshengwenyu.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tex.jiagoushi.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qah.daria6918.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gny.jyoumei.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cta.ywan-chungtsiang.top

Java: // 无：用 Builder 模式或 record
来源：http://bjc.ydzc1.top

Go:   // 无：用配置结构体参数
来源：http://jrj.aibaodan.cn

Ruby: f(a: 1, b: 2)
来源：http://cwv.ppjwa.cn

C#:   f(a: 1, b: 2)
来源：http://ein.hfpthk.cn

[C05] 返回多个值
来源：http://sxl.dashuyun.cn

Py:   return a, b
来源：http://mdz.chenzaomai.com

PHP:  return [$a, $b];
来源：http://drx.zhengqikj.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://mte.bbcook.cn

TS:   return { a, b };
来源：http://mbj.fzhhl.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://uhd.hongshengwenyu.top

Go:   return a, b
来源：http://zup.hywenlv.cn

Ruby: return a, b
来源：http://ibo.svipenyu.cn

C#:   return (a, b);              // ValueTuple
来源：http://axc.zdqjudy.top

[C06] 匿名函数 / lambda
来源：http://ywb.chenlongwang.top

Py:   square = lambda x: x * x
来源：http://ava.shzxlz.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://hjn.ehwqpu.com

JS:   const square = x => x * x;
来源：http://hgv.zdqjudy.top

TS:   const square = (x: number): number => x * x;
来源：http://rms.yj20258.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wzv.iojbl.cn

Go:   sq := func(x int) int { return x * x }
来源：http://uyc.iojbl.cn

Ruby: square = ->(x) { x * x }
来源：http://qro.chenzaomai.com

C#:   Func<int, int> square = x => x * x;
来源：http://tay.xingfuxueyuan.xyz

[C07] 把函数作为参数传入
来源：http://jxo.fanxiaobao.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cxa.birdmap.top

PHP:  array_map("strtoupper", $arr);
来源：http://egq.zhoulong.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fnd.vqdsnc.cn

TS:   arr.map(String)
来源：http://mfb.fanxiaobao.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://thi.yuanzhike.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tqq.quarkkingdee.top

Ruby: arr.map(&:upcase)
来源：http://aso.yuxming.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://zco.tian-w.cn

[C08] 闭包
来源：http://zuk.zdqjudy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ded.zhengqikj.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mwx.nanxuanxn.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qnr.sjlbkw.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dqp.sysykeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://smw.sufxvd.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://leo.jinghuilouyu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jmg.hnxiangtu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://omm.yanxiufei.cn

[C09] 递归
来源：http://fhd.hammf.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tdd.jinghuilouyu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yby.jianghu66.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bog.zhoulong.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rzq.yj20258888.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://suc.jiagoushi.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vvq.52xcode.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://azu.zycfv.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ngj.andypj.xyz

[C10] 变量作用域
来源：http://nik.zhixingplan.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mqf.tianlin.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://srt.havefunace.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wwn.chenlongwang.top

TS:   同 JS
来源：http://btm.hongshengwenyu.top

Java: 方法内为块级作用域
来源：http://psm.chenzaomai.com

Go:   花括号块级作用域
来源：http://ayx.cqqwz.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kyl.zhixingplan.top

C#:   块级作用域
来源：http://lts.hnxiangtu.top

[C11] 模块导入与导出
来源：http://ijr.ehwqpu.com

Py:   from module import func
来源：http://xaf.fengsongda.top

PHP:  require "file.php";  或 use App\Service;
来源：http://rew.dianchejie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://qhj.ydjk.org.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tuo.ydjk.org.cn

Java: import java.util.List;
来源：http://flf.tianlin.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tft.9152youxi.cn

Ruby: require "json"; require_relative "./util"
来源：http://mlj.xziqi.cn

C#:   using System.Text;
来源：http://del.zdqjudy.top

[C12] 立即执行函数 IIFE
来源：http://mei.chenzaomai.com

Py:   (lambda: print("run"))()
来源：http://bam.cashguo.top

PHP:  (function () { echo "run"; })();
来源：http://fzw.andypj.xyz

JS:   (() => { console.log("run"); })();
来源：http://akp.iojbl.cn

TS:   (() => { console.log("run"); })();
来源：http://cez.316326.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ksj.ybcxt.top

Go:   func() { fmt.Println("run") }()
来源：http://ouj.hesvh.cn

Ruby: -> { puts "run" }.call
来源：http://jum.bjfxy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://njt.zhoulong.xyz

[C13] 类型声明 / 类型注解
来源：http://yqo.xylfe.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gsk.tianlin.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://njk.cdnleiting.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wco.yuanzhike.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rmq.sysykeji.top

Java: int add(int a, int b) { return a + b; }
来源：http://bko.xuetiantiany.cn

Go:   func add(a, b int) int
来源：http://ruz.chenjidiqi.icu

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kux.ydzc1.top

C#:   int Add(int a, int b) => a + b;
来源：http://iod.sjlbkw.cn

[C14] 泛型函数
来源：http://tuy.gogol.net.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ken.jinghuilouyu.cn

PHP:  // 无泛型
来源：http://pba.daxiang520.top

JS:   // 无泛型
来源：http://iso.daxiang520.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zir.jqgufenzy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ngj.ybcxt.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cbg.sufxvd.cn

Ruby: # 无泛型
来源：http://wni.fengsongda.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hpe.wangshuangyany.cn

[C15] 解构 / 展开参数
来源：http://tns.tanke756.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://len.ctjpmb.com

PHP:  [$a, $b] = $pair;
来源：http://uvi.smart0.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nrk.ybcxt.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wxu.0kj1m.cn

Java: // 无解构
来源：http://ijf.shuidangran.top

Go:   // 无解构
来源：http://ppx.kuanghao11.cn

Ruby: a, b = pair
来源：http://znx.bbcook.cn

C#:   var (a, b) = pair;
来源：http://gzo.guannengcc.top

[C16] 函数 / 方法重载
来源：http://zsy.daria6918.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gjc.fanxiaobao.xyz

PHP:  // 无重载
来源：http://qzu.aizwys.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bqi.zdqjudy.top

TS:   // 用联合类型或重载签名声明
来源：http://tvz.havefunace.top

Java: void f(int a) {}  void f(String a) {}
来源：http://fnn.nwbrower.top

Go:   // 无重载：用不同函数名
来源：http://fkz.zycfv.cn

Ruby: # 无重载：靠动态参数
来源：http://jsu.vehdjk.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://cak.yuxming.cn

================================================================================
来源：http://unf.nanxuanxn.top

D. 数组 / 列表 / 集合
来源：http://zlp.shuidangran.top

================================================================================
来源：http://nys.nanxuanxn.top

[D01] 创建数组 / 列表
来源：http://rez.birdmap.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://huj.gzhubu.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jnp.jqgufenzy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kfe.vqdsnc.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://kpk.jianghu66.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://csk.wangdashe.top

Go:   arr := []int{1, 2, 3}
来源：http://oqf.hcnkem.com

Ruby: arr = [1, 2, 3]
来源：http://ztc.shangyingyoupin.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ezp.fanxiaobao.xyz

[D02] 追加元素到末尾
来源：http://xtv.fzhhl.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://oyk.hongshengwenyu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://czu.zhiwuduotai.top

JS:   arr.push(4);
来源：http://plp.zdqjudy.top

TS:   arr.push(4);
来源：http://ijg.hysaishi.cn

Java: list.add(4);
来源：http://nmm.xingfuxueyuan.xyz

Go:   arr = append(arr, 4)
来源：http://snf.xingfuxueyuan.xyz

Ruby: arr << 4; arr.push(5)
来源：http://ulg.ydzc1.top

C#:   list.Add(4);
来源：http://ucf.xylfe.cn

[D03] 在指定位置插入元素
来源：http://xbx.guowangkeji.top

Py:   arr.insert(0, 0)
来源：http://vsp.dianchejie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xoz.jinqigfzy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lms.xinyue.icu

TS:   arr.splice(0, 0, 0);
来源：http://ukf.jqgufenzy.top

Java: list.add(0, 0);
来源：http://tlb.ydjk.org.cn

Go:   arr = append([]int{0}, arr...)
来源：http://bzr.0kj1m.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nrd.zdqjudy.top

C#:   list.Insert(0, 0);
来源：http://dbb.sjlbkw.cn

[D04] 删除元素
来源：http://ecd.bbcook.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rjo.hammf.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zkw.xziqi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://smy.52xcode.cn

TS:   arr.splice(0, 1);
来源：http://wgu.hammf.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mjc.feifeiyinyue.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://oms.shzxlz.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cyj.jlsjyb.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://krw.gzhubu.top

[D05] 访问与修改元素
来源：http://zpi.gotoacloud.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ixe.mhx1999.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mds.sysykeji.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://iru.c1oappe.top

TS:   arr[0]; arr.at(-1);
来源：http://rpd.jianghu66.top

Java: list.get(0); list.set(0, 9);
来源：http://clo.quarkkingdee.top

Go:   arr[0]; arr[0] = 9
来源：http://tee.jlsjyb.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nfz.yj20258888.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://htj.zhoulong.xyz

[D06] 数组长度
来源：http://ivv.vqdsnc.cn

Py:   len(arr)
来源：http://bno.jiagoushi.top

PHP:  count($arr);
来源：http://lqk.meibo888.top

JS:   arr.length
来源：http://fzc.jyoumei.cn

TS:   arr.length
来源：http://aft.chenlongwang.top

Java: list.size();
来源：http://qse.gogol.net.cn

Go:   len(arr)
来源：http://fxd.uphjek.com

Ruby: arr.length; arr.size
来源：http://uza.dashuyun.cn

C#:   list.Count;
来源：http://inf.chenzaomai.com

[D07] 切片 / 取子数组
来源：http://hqo.gogol.net.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://flg.yonumen.top

PHP:  array_slice($arr, 1, 3);
来源：http://qqi.yfazqb.com

JS:   arr.slice(1, 4);
来源：http://uda.yuxming.cn

TS:   arr.slice(1, 4);
来源：http://gpb.zhengqikj.top

Java: list.subList(1, 4);
来源：http://tgw.316326.xyz

Go:   arr[1:4]
来源：http://xnc.316326.xyz

Ruby: arr[1, 3]
来源：http://pwr.9152youxi.cn

C#:   list.GetRange(1, 3);
来源：http://qel.iojbl.cn

[D08] 合并两个数组
来源：http://wwb.cucudq.cn

Py:   a + b;  a.extend(b)
来源：http://xhu.ywan-chungtsiang.top

PHP:  array_merge($a, $b);
来源：http://pps.yvedp.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://jtd.yangfankeji.com

TS:   [...a, ...b];
来源：http://juq.xuetiantiany.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rlq.guowangkeji.top

Go:   append(a, b...)
来源：http://dss.jinyuanbaomall.cn

Ruby: a + b;  a.concat(b)
来源：http://oue.zhengqikj.top

C#:   a.Concat(b).ToList()
来源：http://kti.jianghu66.top

[D09] 排序（升序）
来源：http://jrg.ywan-chungtsiang.top

Py:   sorted(arr);  arr.sort()
来源：http://jpm.ctjpmb.com

PHP:  sort($arr);
来源：http://cqw.tanke756.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cqa.hnqzz.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://nas.xuanzx.com

Java: Collections.sort(list);  list.sort(null);
来源：http://hym.sufxvd.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hvk.sxryk.cn

Ruby: arr.sort
来源：http://zwb.zhaomingkeji.xyz

C#:   list.Sort();
来源：http://fbj.dashuyun.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fau.tianlin.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qgi.cheryme.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aic.yj202588.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pbf.0kj1m.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zqx.pycfn.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mpk.vqdsnc.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lzc.daria6918.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vzt.shzxlz.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rjp.vehdjk.com

[D11] 反转数组
来源：http://cgc.yuanzhike.top

Py:   arr[::-1];  arr.reverse()
来源：http://ydu.iojbl.cn

PHP:  array_reverse($arr);
来源：http://jud.jqgufenzy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://edr.quarkkingdee.top

TS:   [...arr].reverse();
来源：http://nse.ctjpmb.com

Java: Collections.reverse(list);
来源：http://jpm.nanxuanxn.top

Go:   slices.Reverse(arr)
来源：http://wnj.hammf.cn

Ruby: arr.reverse
来源：http://zls.jqgfzy.top

C#:   list.Reverse();
来源：http://rft.jinqigufen.top

[D12] 查找元素下标
来源：http://qon.guannengcc.top

Py:   arr.index(x);  x in arr
来源：http://dfz.ehwqpu.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vcj.fzhhl.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lqq.svipenyu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jvr.guannengcc.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jpz.vqdsnc.cn

Go:   slices.Index(arr, x)
来源：http://zdv.xuetiantiany.cn

Ruby: arr.index(x)
来源：http://ewz.hammf.cn

C#:   list.IndexOf(x);
来源：http://tjs.jianghu66.top

[D13] 过滤（保留满足条件的）
来源：http://ehk.yj202588.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://prw.svipenyu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zjm.aizwys.cn

JS:   arr.filter(x => x > 3)
来源：http://fie.chenlongwang.top

TS:   arr.filter(x => x > 3)
来源：http://ybi.smart0.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nea.ppjwa.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ndq.tanke756.top

Ruby: arr.select { |x| x > 3 }
来源：http://crr.zhiwuduotai.top

C#:   list.Where(x => x > 3).ToList()
来源：http://yle.fktsv.cn

[D14] 映射转换（每个元素变形）
来源：http://rlz.fzhhl.top


<!-- 参考信息 -->