代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://lew.yonumen.top

TS:   [1, 2, 3].includes(x)
来源：http://xbd.birdmap.top

Java: List.of(1, 2, 3).contains(x)
来源：http://pux.nanxuanxn.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pid.pengpengdd.cyou

Ruby: [1, 2, 3].include?(x)
来源：http://muq.hongshengwenyu.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zgt.vehdjk.com

[B15] 布尔运算与取反
来源：http://gri.ivvv.top

Py:   a and b or not c
来源：http://lzv.gogol.net.cn

PHP:  $a && $b || !$c
来源：http://zka.xylfe.cn

JS:   a && b || !c
来源：http://mrj.ehwqpu.com

TS:   a && b || !c
来源：http://gar.yangfankeji.com

Java: a && b || !c
来源：http://jmc.smart0.xyz

Go:   a && b || !c
来源：http://neh.gaohongyu789.top

Ruby: a && b || !c
来源：http://bww.hfpthk.cn

C#:   a && b || !c
来源：http://qwx.gzhubu.top

[B16] 卫语句：不满足条件提前返回
来源：http://hhx.hesvh.cn

Py:   if not data: return
来源：http://zly.yuanzhike.top

PHP:  if (!$data) { return; }
来源：http://rnc.0kj1m.cn

JS:   if (!data) return;
来源：http://ent.ehwqpu.com

TS:   if (!data) return;
来源：http://udb.redwolf501.top

Java: if (data == null) return;
来源：http://ohb.hywenlv.cn

Go:   if data == nil { return }
来源：http://hmr.svipenyu.cn

Ruby: return if data.nil?
来源：http://exv.jyoumei.cn

C#:   if (data == null) return;
来源：http://dfr.shuidangran.top

================================================================================
来源：http://krv.tian-w.cn

C. 函数与作用域
来源：http://ojx.hnxiangtu.top

================================================================================
来源：http://pck.xuetiantiany.cn

[C01] 定义函数
来源：http://utx.jlsjyb.cn

Py:   def add(a, b): return a + b
来源：http://bfj.shanyushiyangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kkh.guannengcc.top

JS:   function add(a, b) { return a + b; }
来源：http://vjx.yuxming.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://elj.guannengcc.top

Java: static int add(int a, int b) { return a + b; }
来源：http://kqj.c1oappe.top

Go:   func add(a, b int) int { return a + b }
来源：http://qpa.ehwqpu.com

Ruby: def add(a, b); a + b; end
来源：http://itg.hongshengwenyu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qup.hesvh.cn

[C02] 默认参数
来源：http://ynr.meibo888.top

Py:   def greet(name="World"): return name
来源：http://acx.yangfankeji.com

PHP:  function greet($name = "World") { return $name; }
来源：http://cdy.wangshuangyany.cn

JS:   function greet(name = "World") { return name; }
来源：http://zok.wangshuangyany.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://wjp.hnqzz.top

Java: // 无默认参数：方法重载或 Optional
来源：http://zec.tanke756.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xme.nanxinkj.top

Ruby: def greet(name = "World") = name
来源：http://tsu.ivvv.top

C#:   string Greet(string name = "World") => name;
来源：http://dzu.xingfuxueyuan.xyz

[C03] 可变参数
来源：http://ygy.yongpay.top

Py:   def total(*args): return sum(args)
来源：http://sni.cqqwz.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ogl.cashguo.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gqz.uphjek.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jks.chenlongwang.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fqh.zdbjq.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bpf.wangshuangyany.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hug.chenjidiqi.icu

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dby.ywan-chungtsiang.top

[C04] 命名参数 / 关键字参数
来源：http://yhl.zhongyouzk.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xeh.0kj1m.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fao.cdnleiting.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zqz.zhiwuduotai.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://idg.quarkkingdee.top

Java: // 无：用 Builder 模式或 record
来源：http://wzk.hongshengwenyu.top

Go:   // 无：用配置结构体参数
来源：http://plk.bjfxy.top

Ruby: f(a: 1, b: 2)
来源：http://gje.jianghu66.top

C#:   f(a: 1, b: 2)
来源：http://yjx.nanxuanxn.top

[C05] 返回多个值
来源：http://chx.shuidangran.top

Py:   return a, b
来源：http://xlj.tarul.cn

PHP:  return [$a, $b];
来源：http://zht.ybcxt.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ism.ybcxt.top

TS:   return { a, b };
来源：http://kct.yvedp.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mmk.birdmap.top

Go:   return a, b
来源：http://dta.ydzc1.top

Ruby: return a, b
来源：http://fpm.sweek.top

C#:   return (a, b);              // ValueTuple
来源：http://pdm.yj202588.top

[C06] 匿名函数 / lambda
来源：http://cer.nanxuanxn.top

Py:   square = lambda x: x * x
来源：http://mge.yonumen.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ebv.jinqigfzy.top

JS:   const square = x => x * x;
来源：http://pek.yongpay.top

TS:   const square = (x: number): number => x * x;
来源：http://mjn.hnxiangtu.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cmh.feifeiyinyue.top

Go:   sq := func(x int) int { return x * x }
来源：http://uby.epnwcf.com

Ruby: square = ->(x) { x * x }
来源：http://gii.ctjpmb.com

C#:   Func<int, int> square = x => x * x;
来源：http://sgb.fzhhl.top

[C07] 把函数作为参数传入
来源：http://heh.yanxiufei.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://odq.zdqjudy.top

PHP:  array_map("strtoupper", $arr);
来源：http://rdc.cheryme.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wjm.birdmap.top

TS:   arr.map(String)
来源：http://thr.jqgufenzy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://uuf.hesvh.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jki.xuanzx.com

Ruby: arr.map(&:upcase)
来源：http://fow.tarul.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://vep.wangdashe.top

[C08] 闭包
来源：http://aik.zhixingplan.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ehz.aibaodan.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rzm.jinyuanbaomall.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gjc.epnwcf.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pux.xinyue.icu

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://riq.meibo888.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://grj.sysykeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://exk.xinyue.icu

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ice.shangyingyoupin.top

[C09] 递归
来源：http://wyy.sxryk.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ujy.jqgufenzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pyd.zhiwuduotai.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gol.ybcxt.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xvf.xuanzx.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zqi.yangfankeji.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hpn.yangfankeji.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rls.andypj.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mgk.meibo888.top

[C10] 变量作用域
来源：http://tjf.ybcxt.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mnf.mhx1999.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nyp.bbcook.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xlr.xingfuxueyuan.xyz

TS:   同 JS
来源：http://yxp.yuanzhike.top

Java: 方法内为块级作用域
来源：http://izq.vehdjk.com

Go:   花括号块级作用域
来源：http://dbd.wangshuangyany.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zlj.feifeiyinyue.top

C#:   块级作用域
来源：http://ire.smart0.xyz

[C11] 模块导入与导出
来源：http://rfg.yfazqb.com

Py:   from module import func
来源：http://qsj.daxiang520.top

PHP:  require "file.php";  或 use App\Service;
来源：http://fjx.daria6918.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://usv.yangfankeji.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qey.fehbvm.com

Java: import java.util.List;
来源：http://whk.pengpengdd.cyou

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wdt.316326.xyz

Ruby: require "json"; require_relative "./util"
来源：http://vqp.epnwcf.com

C#:   using System.Text;
来源：http://cgo.cheryme.top

[C12] 立即执行函数 IIFE
来源：http://xyw.ydjk.org.cn

Py:   (lambda: print("run"))()
来源：http://pfc.svipenyu.cn

PHP:  (function () { echo "run"; })();
来源：http://nkm.fzhhl.top

JS:   (() => { console.log("run"); })();
来源：http://zyj.fanxiaobao.xyz

TS:   (() => { console.log("run"); })();
来源：http://ghu.cdnleiting.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vls.iojbl.cn

Go:   func() { fmt.Println("run") }()
来源：http://fgc.zhoulong.xyz

Ruby: -> { puts "run" }.call
来源：http://mnp.xinyue.icu

C#:   // 无 IIFE：用静态构造函数
来源：http://gkb.iojbl.cn

[C13] 类型声明 / 类型注解
来源：http://nva.yvedp.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cxn.guannengcc.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ocu.epnwcf.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kzh.cdnleiting.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wsw.gotoacloud.top

Java: int add(int a, int b) { return a + b; }
来源：http://gwo.gogol.net.cn

Go:   func add(a, b int) int
来源：http://yti.svipenyu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vhu.iojbl.cn

C#:   int Add(int a, int b) => a + b;
来源：http://whq.quarkkingdee.top

[C14] 泛型函数
来源：http://mha.birdmap.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://agy.cheryme.top

PHP:  // 无泛型
来源：http://svr.yuxming.cn

JS:   // 无泛型
来源：http://aqc.yuanzhike.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pll.yonumen.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://suf.0kj1m.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hkm.shuidangran.top

Ruby: # 无泛型
来源：http://dzk.tarul.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dji.gzhubu.top

[C15] 解构 / 展开参数
来源：http://cpj.dashuyun.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lbo.zhoulong.xyz

PHP:  [$a, $b] = $pair;
来源：http://cqp.fzhhl.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wkf.sxryk.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wvf.cucudq.cn

Java: // 无解构
来源：http://sip.yueranfly.top

Go:   // 无解构
来源：http://chf.birdmap.top

Ruby: a, b = pair
来源：http://obv.wangshuangyany.cn

C#:   var (a, b) = pair;
来源：http://nyz.cashguo.top

[C16] 函数 / 方法重载
来源：http://ruo.tianlin.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nlv.fzhhl.top

PHP:  // 无重载
来源：http://khd.xinyue.icu

JS:   // 无重载：靠 arguments.length 分支
来源：http://osh.zhongyouzk.top

TS:   // 用联合类型或重载签名声明
来源：http://wdx.dianchejie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://mqo.jinghuilouyu.cn

Go:   // 无重载：用不同函数名
来源：http://ggs.xuetiantiany.cn

Ruby: # 无重载：靠动态参数
来源：http://hdj.epnwcf.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://cad.shuidangran.top

================================================================================
来源：http://njc.cqqwz.cn

D. 数组 / 列表 / 集合
来源：http://stg.zdbjq.cn

================================================================================
来源：http://rgl.jinqigufen.top

[D01] 创建数组 / 列表
来源：http://hss.sjlbkw.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://lff.shzxlz.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rkv.yfazqb.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ffh.ehwqpu.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://zoh.yj202588.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ikt.havefunace.top

Go:   arr := []int{1, 2, 3}
来源：http://bxv.fanxiaobao.xyz

Ruby: arr = [1, 2, 3]
来源：http://udp.tarul.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mdq.hongshengwenyu.top

[D02] 追加元素到末尾
来源：http://cen.bbcook.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://czp.zhijiandao.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vze.jlsjyb.cn

JS:   arr.push(4);
来源：http://ahd.meibo888.top

TS:   arr.push(4);
来源：http://ixb.daria6918.cn

Java: list.add(4);
来源：http://omz.jinyuanbaomall.cn

Go:   arr = append(arr, 4)
来源：http://tcs.dianchejie.cn

Ruby: arr << 4; arr.push(5)
来源：http://wdg.yonumen.top

C#:   list.Add(4);
来源：http://gvq.hywenlv.cn

[D03] 在指定位置插入元素
来源：http://qfw.ehwqpu.com

Py:   arr.insert(0, 0)
来源：http://lsc.9152youxi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://snx.bbcook.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fve.zhixingplan.top

TS:   arr.splice(0, 0, 0);
来源：http://dzc.zhixingplan.top

Java: list.add(0, 0);
来源：http://vxq.hnxiangtu.top

Go:   arr = append([]int{0}, arr...)
来源：http://nhi.daxiang520.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://trk.ivvv.top

C#:   list.Insert(0, 0);
来源：http://eik.hfpthk.cn

[D04] 删除元素
来源：http://sfg.sufxvd.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://upd.cdnleiting.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xyc.nanxinkj.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xmg.kuanghao11.cn

TS:   arr.splice(0, 1);
来源：http://anl.jqgfzy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nnb.pycfn.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://koc.jinyuanbaomall.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ook.yj202588.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mat.guannengcc.top

[D05] 访问与修改元素
来源：http://vxp.bbcook.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rpr.hesvh.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://glv.guannengcc.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pae.ydzc1.top

TS:   arr[0]; arr.at(-1);
来源：http://bsl.yanxiufei.cn

Java: list.get(0); list.set(0, 9);
来源：http://okg.gogol.net.cn

Go:   arr[0]; arr[0] = 9
来源：http://eoy.ppjwa.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xzg.tian-w.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gcm.yj20258.top

[D06] 数组长度
来源：http://rjg.ppjwa.cn

Py:   len(arr)
来源：http://zik.quarkkingdee.top

PHP:  count($arr);
来源：http://nqc.birdmap.top

JS:   arr.length
来源：http://kgo.sxryk.cn

TS:   arr.length
来源：http://bue.ywan-chungtsiang.top

Java: list.size();
来源：http://bem.zhaomingkeji.xyz

Go:   len(arr)
来源：http://apf.yj20258.top

Ruby: arr.length; arr.size
来源：http://fgo.shzxlz.cn

C#:   list.Count;
来源：http://esw.c1oappe.top

[D07] 切片 / 取子数组
来源：http://oqx.xuetiantiany.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wws.birdmap.top

PHP:  array_slice($arr, 1, 3);
来源：http://kwp.ehwqpu.com

JS:   arr.slice(1, 4);
来源：http://twf.hfpthk.cn

TS:   arr.slice(1, 4);
来源：http://vaw.gogol.net.cn

Java: list.subList(1, 4);
来源：http://sdo.shangyingyoupin.top

Go:   arr[1:4]
来源：http://wod.zhaomingkeji.xyz

Ruby: arr[1, 3]
来源：http://heq.jianghu66.top

C#:   list.GetRange(1, 3);
来源：http://fxd.tarul.cn

[D08] 合并两个数组
来源：http://kjt.epnwcf.com

Py:   a + b;  a.extend(b)
来源：http://xtn.tarul.cn

PHP:  array_merge($a, $b);
来源：http://gxh.yongpay.top

JS:   [...a, ...b];  a.concat(b);
来源：http://kgr.zhongyouzk.top

TS:   [...a, ...b];
来源：http://fna.guowangkeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://djh.aizwys.cn

Go:   append(a, b...)
来源：http://qos.jianghu66.top

Ruby: a + b;  a.concat(b)
来源：http://xfd.chenzaomai.com

C#:   a.Concat(b).ToList()
来源：http://oho.zhixingplan.top

[D09] 排序（升序）
来源：http://eag.iojbl.cn

Py:   sorted(arr);  arr.sort()
来源：http://sel.xingfuxueyuan.xyz

PHP:  sort($arr);
来源：http://gml.aizwys.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hjd.sjlbkw.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://bpq.shanyushiyangkeji.top

Java: Collections.sort(list);  list.sort(null);
来源：http://nhm.tarul.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pjc.fehbvm.com

Ruby: arr.sort
来源：http://oun.feifeiyinyue.top

C#:   list.Sort();
来源：http://wcu.xziqi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://hqq.sysykeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://oby.cashguo.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ela.zhoulong.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lio.hongshengwenyu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dwr.hcnkem.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qhl.zhaomingkeji.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://eih.guannengcc.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://esi.hongshengwenyu.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zta.sysykeji.top

[D11] 反转数组
来源：http://obd.0kj1m.cn

Py:   arr[::-1];  arr.reverse()
来源：http://cxf.sysykeji.top

PHP:  array_reverse($arr);
来源：http://cdp.fzhhl.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lvz.vehdjk.com

TS:   [...arr].reverse();
来源：http://cpg.dianchejie.cn

Java: Collections.reverse(list);
来源：http://qal.yuanzhike.top

Go:   slices.Reverse(arr)
来源：http://oen.hywenlv.cn

Ruby: arr.reverse
来源：http://kil.yueranfly.top

C#:   list.Reverse();
来源：http://ohs.xingfuxueyuan.xyz

[D12] 查找元素下标
来源：http://zgt.jiagoushi.top

Py:   arr.index(x);  x in arr
来源：http://vha.sxryk.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jgp.chenzaomai.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kxw.iojbl.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ifi.iojbl.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ftw.jqgufenzy.top

Go:   slices.Index(arr, x)
来源：http://sob.birdmap.top

Ruby: arr.index(x)
来源：http://tod.hywenlv.cn

C#:   list.IndexOf(x);
来源：http://vvm.nanxuanxn.top

[D13] 过滤（保留满足条件的）
来源：http://amy.cqqwz.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mbp.jqgfzy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xdm.mhx1999.top

JS:   arr.filter(x => x > 3)
来源：http://jes.hnqzz.top

TS:   arr.filter(x => x > 3)
来源：http://ldu.jinghuilouyu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jos.pengpengdd.cyou

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sjv.hnxiangtu.top

Ruby: arr.select { |x| x > 3 }
来源：http://zer.vqdsnc.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bzi.zycfv.cn

[D14] 映射转换（每个元素变形）
来源：http://qch.iojbl.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fbl.daxiang520.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://duq.aizwys.cn

JS:   arr.map(x => x * 2)
来源：http://gpw.gaohongyu789.top

TS:   arr.map(x => x * 2)
来源：http://btl.hammf.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://dzu.cdnleiting.top

Go:   // 手写循环
来源：http://ezo.nanxuanxn.top

Ruby: arr.map { |x| x * 2 }
来源：http://cma.chenzaomai.com

C#:   list.Select(x => x * 2).ToList()
来源：http://ctg.aibaodan.cn


<!-- 参考信息 -->