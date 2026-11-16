代发 wailian999

Go:   a && b || !c
来源：http://fwp.jiagoushi.top

Ruby: a && b || !c
来源：http://ufd.feifeiyinyue.top

C#:   a && b || !c
来源：http://zkm.0kj1m.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ypx.ppjwa.cn

Py:   if not data: return
来源：http://kyi.dianchejie.cn

PHP:  if (!$data) { return; }
来源：http://nbk.guannengcc.top

JS:   if (!data) return;
来源：http://kbf.pengpengdd.cyou

TS:   if (!data) return;
来源：http://xtm.jlsjyb.cn

Java: if (data == null) return;
来源：http://ypz.cucudq.cn

Go:   if data == nil { return }
来源：http://trr.ybcxt.top

Ruby: return if data.nil?
来源：http://xrv.guannengcc.top

C#:   if (data == null) return;
来源：http://nsr.dashuyun.cn

================================================================================
来源：http://oco.ehwqpu.com

C. 函数与作用域
来源：http://hkd.quarkkingdee.top

================================================================================
来源：http://bqw.ivvv.top

[C01] 定义函数
来源：http://vvb.xylfe.cn

Py:   def add(a, b): return a + b
来源：http://ezz.meibo888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uti.chenjidiqi.icu

JS:   function add(a, b) { return a + b; }
来源：http://drl.jinyuanbaomall.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://val.fzhhl.top

Java: static int add(int a, int b) { return a + b; }
来源：http://zcm.ehwqpu.com

Go:   func add(a, b int) int { return a + b }
来源：http://ctf.pengpengdd.cyou

Ruby: def add(a, b); a + b; end
来源：http://fpw.jinghuilouyu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://eam.xingfuxueyuan.xyz

[C02] 默认参数
来源：http://hty.cqqwz.cn

Py:   def greet(name="World"): return name
来源：http://toq.fzhhl.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ifb.hcnkem.com

JS:   function greet(name = "World") { return name; }
来源：http://cbe.pengpengdd.cyou

TS:   function greet(name: string = "World") { return name; }
来源：http://fah.zdqjudy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://jum.xinyue.icu

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hbu.wangshuangyany.cn

Ruby: def greet(name = "World") = name
来源：http://cjd.feifeiyinyue.top

C#:   string Greet(string name = "World") => name;
来源：http://mxg.shzxlz.cn

[C03] 可变参数
来源：http://imx.sjlbkw.cn

Py:   def total(*args): return sum(args)
来源：http://yhp.yj20258.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pbf.aibaodan.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wnt.yongpay.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://aqo.ppjwa.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vfu.fktsv.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jgo.sweek.top

Ruby: def total(*nums); nums.sum; end
来源：http://gay.fktsv.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bxc.bbcook.cn

[C04] 命名参数 / 关键字参数
来源：http://jlw.gogol.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ryl.yj20258.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://phd.cdnleiting.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pxn.cheryme.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pid.yuxming.cn

Java: // 无：用 Builder 模式或 record
来源：http://gru.ctjpmb.com

Go:   // 无：用配置结构体参数
来源：http://kyo.bjfxy.top

Ruby: f(a: 1, b: 2)
来源：http://hch.snrcjt.cn

C#:   f(a: 1, b: 2)
来源：http://moo.sufxvd.cn

[C05] 返回多个值
来源：http://xgp.yvedp.cn

Py:   return a, b
来源：http://zpz.fzhhl.top

PHP:  return [$a, $b];
来源：http://blw.andypj.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://qrp.zdbjq.cn

TS:   return { a, b };
来源：http://umo.bjfxy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://njy.shanyushiyangtech.top

Go:   return a, b
来源：http://dzm.haohaochexian.top

Ruby: return a, b
来源：http://prg.daria6918.cn

C#:   return (a, b);              // ValueTuple
来源：http://nvy.cheryme.top

[C06] 匿名函数 / lambda
来源：http://oui.daxiang520.top

Py:   square = lambda x: x * x
来源：http://hfo.fzhhl.top

PHP:  $square = fn($x) => $x * $x;
来源：http://bmb.ppjwa.cn

JS:   const square = x => x * x;
来源：http://tkk.guannengcc.top

TS:   const square = (x: number): number => x * x;
来源：http://hhv.shuidangran.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cwy.fehbvm.com

Go:   sq := func(x int) int { return x * x }
来源：http://peq.redwolf501.top

Ruby: square = ->(x) { x * x }
来源：http://deu.daxiang520.top

C#:   Func<int, int> square = x => x * x;
来源：http://hus.yuanzhike.top

[C07] 把函数作为参数传入
来源：http://qzr.yvedp.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sxb.fanxiaobao.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://qvx.jinyuanbaomall.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nzh.smart0.xyz

TS:   arr.map(String)
来源：http://cbp.ybcxt.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://chh.ctjpmb.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tvh.svipenyu.cn

Ruby: arr.map(&:upcase)
来源：http://lnp.cqqwz.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mgv.birdmap.top

[C08] 闭包
来源：http://fua.iojbl.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zxp.redwolf501.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jlz.zhixingplan.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kkn.nanxuanxn.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sdr.hnxiangtu.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bxw.uphjek.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jmg.ppjwa.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gua.tarul.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nbu.yuxming.cn

[C09] 递归
来源：http://sro.cucudq.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://doa.tian-w.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ypy.zdqjudy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://srq.cheryme.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sxp.wangdashe.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kpw.vehdjk.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jrd.hfpthk.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fkh.yueranfly.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mbv.sxryk.cn

[C10] 变量作用域
来源：http://tcv.hnqzz.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hem.shanyushiyangkeji.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://egy.guannengcc.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mjd.chenjidiqi.icu

TS:   同 JS
来源：http://ylx.ydzc1.top

Java: 方法内为块级作用域
来源：http://zdh.tarul.cn

Go:   花括号块级作用域
来源：http://cjd.hesvh.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ohu.9152youxi.cn

C#:   块级作用域
来源：http://odu.ywan-chungtsiang.top

[C11] 模块导入与导出
来源：http://iac.cheryme.top

Py:   from module import func
来源：http://yvw.shanyushiyangkeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://vrs.xinyue.icu

JS:   export default function f() {};  import f from "./m.js";
来源：http://irm.vqdsnc.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://akk.kuanghao11.cn

Java: import java.util.List;
来源：http://qyh.fzhhl.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ams.yuanzhike.top

Ruby: require "json"; require_relative "./util"
来源：http://uoe.sxryk.cn

C#:   using System.Text;
来源：http://oyr.guowangkeji.top

[C12] 立即执行函数 IIFE
来源：http://pmc.svipenyu.cn

Py:   (lambda: print("run"))()
来源：http://aom.vqdsnc.cn

PHP:  (function () { echo "run"; })();
来源：http://nyz.shuidangran.top

JS:   (() => { console.log("run"); })();
来源：http://uhk.0kj1m.cn

TS:   (() => { console.log("run"); })();
来源：http://zyo.bjfxy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://khf.aizwys.cn

Go:   func() { fmt.Println("run") }()
来源：http://xwq.sysykeji.top

Ruby: -> { puts "run" }.call
来源：http://rti.yueranfly.top

C#:   // 无 IIFE：用静态构造函数
来源：http://wgr.zhiwuduotai.top

[C13] 类型声明 / 类型注解
来源：http://rib.fanxiaobao.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yuf.hammf.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bur.yanxiufei.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mmn.yueranfly.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nig.yvedp.cn

Java: int add(int a, int b) { return a + b; }
来源：http://zng.316326.xyz

Go:   func add(a, b int) int
来源：http://brd.jyoumei.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://oex.yj20258888.top

C#:   int Add(int a, int b) => a + b;
来源：http://vyb.vqdsnc.cn

[C14] 泛型函数
来源：http://cee.yongpay.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jgr.yangfankeji.com

PHP:  // 无泛型
来源：http://nig.smart0.xyz

JS:   // 无泛型
来源：http://jbh.shzxlz.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uky.guowangkeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lsh.tanke756.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pxr.jianghu66.top

Ruby: # 无泛型
来源：http://whe.ivvv.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hls.9152youxi.cn

[C15] 解构 / 展开参数
来源：http://frs.zycfv.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ccr.uphjek.com

PHP:  [$a, $b] = $pair;
来源：http://mlt.yj20258.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wzi.guowangkeji.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fga.sxryk.cn

Java: // 无解构
来源：http://ytb.redwolf501.top

Go:   // 无解构
来源：http://fkk.sysykeji.top

Ruby: a, b = pair
来源：http://qmv.ppjwa.cn

C#:   var (a, b) = pair;
来源：http://jbe.xingfuxueyuan.xyz

[C16] 函数 / 方法重载
来源：http://eif.cashguo.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xtq.yfazqb.com

PHP:  // 无重载
来源：http://gwl.zdqjudy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://axo.zhijiandao.cn

TS:   // 用联合类型或重载签名声明
来源：http://sbm.uphjek.com

Java: void f(int a) {}  void f(String a) {}
来源：http://asl.c1oappe.top

Go:   // 无重载：用不同函数名
来源：http://tur.wangshuangyany.cn

Ruby: # 无重载：靠动态参数
来源：http://btz.sysykeji.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://mpx.nanxuanxn.top

================================================================================
来源：http://oms.sweek.top

D. 数组 / 列表 / 集合
来源：http://dbz.shangyingyoupin.top

================================================================================
来源：http://cyk.shanyushiyangkeji.top

[D01] 创建数组 / 列表
来源：http://dfi.nanxuanxn.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://cqx.jinqigfzy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jfh.shanyushiyangkeji.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wzc.zycfv.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ehr.gotoacloud.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qvu.yfazqb.com

Go:   arr := []int{1, 2, 3}
来源：http://gpz.hysaishi.cn

Ruby: arr = [1, 2, 3]
来源：http://ana.zdbjq.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xml.zhoulong.xyz

[D02] 追加元素到末尾
来源：http://njj.wangdashe.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://emy.gaohongyu789.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gkg.hnqzz.top

JS:   arr.push(4);
来源：http://iri.yangfankeji.com

TS:   arr.push(4);
来源：http://gtx.cqqwz.cn

Java: list.add(4);
来源：http://jrx.sufxvd.cn

Go:   arr = append(arr, 4)
来源：http://smn.shangyingyoupin.top

Ruby: arr << 4; arr.push(5)
来源：http://lvr.jinqigfzy.top

C#:   list.Add(4);
来源：http://itf.jinghuilouyu.cn

[D03] 在指定位置插入元素
来源：http://mhi.shanyushiyangkeji.top

Py:   arr.insert(0, 0)
来源：http://knr.epnwcf.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kwk.shanyushiyangtech.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://acn.shzxlz.cn

TS:   arr.splice(0, 0, 0);
来源：http://vpu.hongshengwenyu.top

Java: list.add(0, 0);
来源：http://hun.yuanzhike.top

Go:   arr = append([]int{0}, arr...)
来源：http://gza.cqqwz.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cwx.vqdsnc.cn

C#:   list.Insert(0, 0);
来源：http://ltb.hysaishi.cn

[D04] 删除元素
来源：http://kpm.yonumen.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cbl.wangshuangyany.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tom.tarul.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mqz.mhx1999.top

TS:   arr.splice(0, 1);
来源：http://kga.yonumen.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://poz.zdqjudy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zvk.xinyue.icu

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mph.yongpay.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://oli.shanyushiyangkeji.top

[D05] 访问与修改元素
来源：http://zfo.zhiwuduotai.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mfv.xziqi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lek.hnqzz.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://orq.yuanzhike.top

TS:   arr[0]; arr.at(-1);
来源：http://nxa.ydzc1.top

Java: list.get(0); list.set(0, 9);
来源：http://pti.smart0.xyz

Go:   arr[0]; arr[0] = 9
来源：http://xac.sysykeji.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lal.ydjk.org.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wpx.ivvv.top

[D06] 数组长度
来源：http://pqc.sufxvd.cn

Py:   len(arr)
来源：http://oub.fehbvm.com

PHP:  count($arr);
来源：http://xgl.pengpengdd.cyou

JS:   arr.length
来源：http://fcx.jlsjyb.cn

TS:   arr.length
来源：http://ijw.sweek.top

Java: list.size();
来源：http://eqp.316326.xyz

Go:   len(arr)
来源：http://hvq.bjfxy.top

Ruby: arr.length; arr.size
来源：http://wxg.yueranfly.top

C#:   list.Count;
来源：http://oeq.gogol.net.cn

[D07] 切片 / 取子数组
来源：http://jjh.haohaochexian.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bhw.jinqigfzy.top

PHP:  array_slice($arr, 1, 3);
来源：http://ujm.gzhubu.top

JS:   arr.slice(1, 4);
来源：http://wvg.aizwys.cn

TS:   arr.slice(1, 4);
来源：http://gja.hammf.cn

Java: list.subList(1, 4);
来源：http://ysy.316326.xyz

Go:   arr[1:4]
来源：http://enk.xziqi.cn

Ruby: arr[1, 3]
来源：http://pcy.xuanzx.com

C#:   list.GetRange(1, 3);
来源：http://cyp.bbcook.cn

[D08] 合并两个数组
来源：http://rvc.shzxlz.cn

Py:   a + b;  a.extend(b)
来源：http://ijt.wangdashe.top

PHP:  array_merge($a, $b);
来源：http://aqi.chenzaomai.com

JS:   [...a, ...b];  a.concat(b);
来源：http://cyx.zhixingplan.top

TS:   [...a, ...b];
来源：http://jic.pengpengdd.cyou

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lai.yj20258.top

Go:   append(a, b...)
来源：http://zyy.aibaodan.cn

Ruby: a + b;  a.concat(b)
来源：http://wtq.meibo888.top

C#:   a.Concat(b).ToList()
来源：http://rne.meibo888.top

[D09] 排序（升序）
来源：http://kke.c1oappe.top

Py:   sorted(arr);  arr.sort()
来源：http://lor.yj20258.top

PHP:  sort($arr);
来源：http://sda.cheryme.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tbv.zhoulong.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://vsa.redwolf501.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ykb.fktsv.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vam.jqgufenzy.top

Ruby: arr.sort
来源：http://tfs.bbcook.cn

C#:   list.Sort();
来源：http://drb.xuanzx.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://piv.jinyuanbaomall.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://elw.shanyushiyangkeji.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wft.gotoacloud.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://irm.tarul.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://sok.snrcjt.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://csh.hnxiangtu.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wov.ctjpmb.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vix.quarkkingdee.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://prs.jlsjyb.cn

[D11] 反转数组
来源：http://qww.daxiang520.top

Py:   arr[::-1];  arr.reverse()
来源：http://cne.zhijiandao.cn

PHP:  array_reverse($arr);
来源：http://qye.yueranfly.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mps.hongshengwenyu.top

TS:   [...arr].reverse();
来源：http://byf.tian-w.cn

Java: Collections.reverse(list);
来源：http://fzo.tanke756.top

Go:   slices.Reverse(arr)
来源：http://yhc.pycfn.com

Ruby: arr.reverse
来源：http://hlt.jyoumei.cn

C#:   list.Reverse();
来源：http://ssm.ywan-chungtsiang.top

[D12] 查找元素下标
来源：http://ewl.cheryme.top

Py:   arr.index(x);  x in arr
来源：http://pks.wangdashe.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rtv.xuetiantiany.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mma.nanxinkj.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pjy.yanxiufei.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lug.chenlongwang.top

Go:   slices.Index(arr, x)
来源：http://aan.tian-w.cn

Ruby: arr.index(x)
来源：http://djc.kuanghao11.cn

C#:   list.IndexOf(x);
来源：http://txj.tian-w.cn

[D13] 过滤（保留满足条件的）
来源：http://ycq.bjfxy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xhx.ctjpmb.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pxu.sysykeji.top

JS:   arr.filter(x => x > 3)
来源：http://pyf.zhoulong.xyz

TS:   arr.filter(x => x > 3)
来源：http://iaj.ivvv.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://eyz.bjfxy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://onz.havefunace.top

Ruby: arr.select { |x| x > 3 }
来源：http://ugp.epnwcf.com

C#:   list.Where(x => x > 3).ToList()
来源：http://faz.jinyuanbaomall.cn

[D14] 映射转换（每个元素变形）
来源：http://ueg.vehdjk.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qki.cqqwz.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cvg.yuxming.cn

JS:   arr.map(x => x * 2)
来源：http://nmx.vqdsnc.cn

TS:   arr.map(x => x * 2)
来源：http://afm.zhaomingkeji.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://fxn.yj20258.top

Go:   // 手写循环
来源：http://mng.shzxlz.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dqo.quarkkingdee.top

C#:   list.Select(x => x * 2).ToList()
来源：http://iqy.guannengcc.top

[D15] 去重
来源：http://vdb.shzxlz.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dwf.shangyingyoupin.top

PHP:  array_unique($arr);
来源：http://emg.gotoacloud.top

JS:   [...new Set(arr)]
来源：http://uyu.gzhubu.top

TS:   [...new Set(arr)]
来源：http://lel.yj20258888.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bvp.xingfuxueyuan.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://tfq.zhijiandao.cn

Ruby: arr.uniq
来源：http://yej.chenzaomai.com

C#:   list.Distinct().ToList()
来源：http://jsx.shanyushiyangkeji.top

[D16] 求和与平均值
来源：http://ssq.xylfe.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zsb.ivvv.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wom.hongshengwenyu.top


<!-- 参考信息 -->