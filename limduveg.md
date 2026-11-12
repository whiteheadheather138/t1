代发 wailian999

[B13] 判断是否为数字
来源：http://xdc.gogol.net.cn

Py:   isinstance(x, (int, float))
来源：http://hyc.shzxlz.cn

PHP:  is_numeric($x)
来源：http://ihf.yangfankeji.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nid.chenzaomai.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rmh.hfpthk.cn

Java: x instanceof Number
来源：http://vqh.jlsjyb.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nme.svipenyu.cn

Ruby: x.is_a?(Numeric)
来源：http://mcd.0kj1m.cn

C#:   x is int or double or decimal
来源：http://dme.yuxming.cn

[B14] 判断值是否在集合内
来源：http://dgc.gzhubu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wld.yueranfly.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xfk.cqqwz.cn

JS:   [1, 2, 3].includes(x)
来源：http://vae.bjfxy.top

TS:   [1, 2, 3].includes(x)
来源：http://ttg.dashuyun.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://lnr.yj20258888.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qzt.jqgufenzy.top

Ruby: [1, 2, 3].include?(x)
来源：http://mjj.hysaishi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gec.sweek.top

[B15] 布尔运算与取反
来源：http://sdn.chenjidiqi.icu

Py:   a and b or not c
来源：http://djb.gogol.net.cn

PHP:  $a && $b || !$c
来源：http://ruq.sjlbkw.cn

JS:   a && b || !c
来源：http://ssn.ydzc1.top

TS:   a && b || !c
来源：http://ffn.snrcjt.cn

Java: a && b || !c
来源：http://ucd.xuetiantiany.cn

Go:   a && b || !c
来源：http://ldy.yanxiufei.cn

Ruby: a && b || !c
来源：http://qxo.daxiang520.top

C#:   a && b || !c
来源：http://yyl.nanxinkj.top

[B16] 卫语句：不满足条件提前返回
来源：http://ocd.aizwys.cn

Py:   if not data: return
来源：http://gcd.yj20258888.top

PHP:  if (!$data) { return; }
来源：http://eey.hnxiangtu.top

JS:   if (!data) return;
来源：http://kkm.shanyushiyangkeji.top

TS:   if (!data) return;
来源：http://mtw.jqgfzy.top

Java: if (data == null) return;
来源：http://yfx.shuidangran.top

Go:   if data == nil { return }
来源：http://whg.daxiang520.top

Ruby: return if data.nil?
来源：http://oqz.bjfxy.top

C#:   if (data == null) return;
来源：http://onw.xziqi.cn

================================================================================
来源：http://zhm.yuxming.cn

C. 函数与作用域
来源：http://cmj.jiagoushi.top

================================================================================
来源：http://rku.cdnleiting.top

[C01] 定义函数
来源：http://sks.tarul.cn

Py:   def add(a, b): return a + b
来源：http://emc.chenlongwang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jqa.zhiwuduotai.top

JS:   function add(a, b) { return a + b; }
来源：http://sat.fktsv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gke.gaohongyu789.top

Java: static int add(int a, int b) { return a + b; }
来源：http://grm.fehbvm.com

Go:   func add(a, b int) int { return a + b }
来源：http://crq.fengsongda.top

Ruby: def add(a, b); a + b; end
来源：http://wby.fzhhl.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wwc.jqgufenzy.top

[C02] 默认参数
来源：http://irb.havefunace.top

Py:   def greet(name="World"): return name
来源：http://rpq.ivvv.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ljc.hammf.cn

JS:   function greet(name = "World") { return name; }
来源：http://nat.yangfankeji.com

TS:   function greet(name: string = "World") { return name; }
来源：http://evj.wangshuangyany.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qqe.tarul.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gnx.nwbrower.top

Ruby: def greet(name = "World") = name
来源：http://lxu.zhongyouzk.top

C#:   string Greet(string name = "World") => name;
来源：http://dfq.yuxming.cn

[C03] 可变参数
来源：http://ikc.hysaishi.cn

Py:   def total(*args): return sum(args)
来源：http://vqm.xuetiantiany.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wzi.guowangkeji.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://boa.sweek.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://trl.52xcode.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mww.wangdashe.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.gaohongyu789.top

Ruby: def total(*nums); nums.sum; end
来源：http://ctk.nanxuanxn.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://atb.havefunace.top

[C04] 命名参数 / 关键字参数
来源：http://xqd.xuetiantiany.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ids.xinyue.icu

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xsc.sjlbkw.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jtl.sxryk.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ger.dianchejie.cn

Java: // 无：用 Builder 模式或 record
来源：http://ntf.yanxiufei.cn

Go:   // 无：用配置结构体参数
来源：http://gen.c1oappe.top

Ruby: f(a: 1, b: 2)
来源：http://vwy.daxiang520.top

C#:   f(a: 1, b: 2)
来源：http://ich.jiagoushi.top

[C05] 返回多个值
来源：http://kuj.ctjpmb.com

Py:   return a, b
来源：http://stv.daxiang520.top

PHP:  return [$a, $b];
来源：http://ytw.cucudq.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://kgt.hnxiangtu.top

TS:   return { a, b };
来源：http://sbh.pengpengdd.cyou

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qtq.hongshengwenyu.top

Go:   return a, b
来源：http://uon.bjfxy.top

Ruby: return a, b
来源：http://irt.fanxiaobao.xyz

C#:   return (a, b);              // ValueTuple
来源：http://yum.ehwqpu.com

[C06] 匿名函数 / lambda
来源：http://wop.ivvv.top

Py:   square = lambda x: x * x
来源：http://wiu.shanyushiyangkeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://jdx.sweek.top

JS:   const square = x => x * x;
来源：http://jxh.tanke756.top

TS:   const square = (x: number): number => x * x;
来源：http://jec.xuanzx.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mgb.shzxlz.cn

Go:   sq := func(x int) int { return x * x }
来源：http://yuz.52xcode.cn

Ruby: square = ->(x) { x * x }
来源：http://mgl.zhoulong.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://uxu.epnwcf.com

[C07] 把函数作为参数传入
来源：http://mkn.tianlin.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sxo.shuidangran.top

PHP:  array_map("strtoupper", $arr);
来源：http://pqb.zdbjq.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nbn.cdnleiting.top

TS:   arr.map(String)
来源：http://gpg.jqgufenzy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hlt.yfazqb.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://uni.jqgfzy.top

Ruby: arr.map(&:upcase)
来源：http://iru.hesvh.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xjz.yuxming.cn

[C08] 闭包
来源：http://yyv.sufxvd.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wqi.zhoulong.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bum.ehwqpu.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://myi.jinghuilouyu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gmg.jinqigfzy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vyz.zycfv.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://loh.aibaodan.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mkd.hammf.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://klv.kuanghao11.cn

[C09] 递归
来源：http://wyk.shuidangran.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vbb.quarkkingdee.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ucy.uphjek.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://frg.yj20258.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nwi.sufxvd.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ftw.jinqigfzy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ivx.wangdashe.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ktb.sysykeji.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zvl.xziqi.cn

[C10] 变量作用域
来源：http://zsy.9152youxi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ddr.aibaodan.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tfe.bbcook.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nwn.shanyushiyangtech.top

TS:   同 JS
来源：http://hpr.jinqigufen.top

Java: 方法内为块级作用域
来源：http://hdj.zhixingplan.top

Go:   花括号块级作用域
来源：http://non.xziqi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nla.hammf.cn

C#:   块级作用域
来源：http://wsf.shangyingyoupin.top

[C11] 模块导入与导出
来源：http://nwc.xinyue.icu

Py:   from module import func
来源：http://pna.daxiang520.top

PHP:  require "file.php";  或 use App\Service;
来源：http://xcd.jinyuanbaomall.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://yzg.jlsjyb.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pac.shuidangran.top

Java: import java.util.List;
来源：http://lyu.quarkkingdee.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://myp.hcnkem.com

Ruby: require "json"; require_relative "./util"
来源：http://dcx.quarkkingdee.top

C#:   using System.Text;
来源：http://gut.yvedp.cn

[C12] 立即执行函数 IIFE
来源：http://plc.yueranfly.top

Py:   (lambda: print("run"))()
来源：http://zdq.aizwys.cn

PHP:  (function () { echo "run"; })();
来源：http://jcz.zhaomingkeji.xyz

JS:   (() => { console.log("run"); })();
来源：http://ssl.jinyuanbaomall.cn

TS:   (() => { console.log("run"); })();
来源：http://nxv.aizwys.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xdd.ehwqpu.com

Go:   func() { fmt.Println("run") }()
来源：http://fna.ybcxt.top

Ruby: -> { puts "run" }.call
来源：http://spm.vqdsnc.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mbw.yangfankeji.com

[C13] 类型声明 / 类型注解
来源：http://yja.jianghu66.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qfl.zhijiandao.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ryy.jinqigufen.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ixz.xingfuxueyuan.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bjs.pengpengdd.cyou

Java: int add(int a, int b) { return a + b; }
来源：http://wgn.yj202588.top

Go:   func add(a, b int) int
来源：http://lgg.chenzaomai.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://oks.guowangkeji.top

C#:   int Add(int a, int b) => a + b;
来源：http://fob.nwbrower.top

[C14] 泛型函数
来源：http://eil.xuetiantiany.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vtr.sjlbkw.cn

PHP:  // 无泛型
来源：http://iuw.fktsv.cn

JS:   // 无泛型
来源：http://eoy.fengsongda.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hld.xuanzx.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hik.sjlbkw.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tmw.vqdsnc.cn

Ruby: # 无泛型
来源：http://sax.tian-w.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wea.xingfuxueyuan.xyz

[C15] 解构 / 展开参数
来源：http://ffy.nanxinkj.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ncp.aizwys.cn

PHP:  [$a, $b] = $pair;
来源：http://gju.zhoulong.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xns.birdmap.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lza.hcnkem.com

Java: // 无解构
来源：http://nju.sufxvd.cn

Go:   // 无解构
来源：http://xjp.ydzc1.top

Ruby: a, b = pair
来源：http://xvr.zycfv.cn

C#:   var (a, b) = pair;
来源：http://xkd.wangdashe.top

[C16] 函数 / 方法重载
来源：http://sqk.hammf.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ksi.hammf.cn

PHP:  // 无重载
来源：http://kbk.tanke756.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://hjp.zhongyouzk.top

TS:   // 用联合类型或重载签名声明
来源：http://emn.316326.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://xjh.wangdashe.top

Go:   // 无重载：用不同函数名
来源：http://ict.aizwys.cn

Ruby: # 无重载：靠动态参数
来源：http://yqi.bbcook.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://dnt.hcnkem.com

================================================================================
来源：http://wko.bbcook.cn

D. 数组 / 列表 / 集合
来源：http://ykz.chenjidiqi.icu

================================================================================
来源：http://zcs.smart0.xyz

[D01] 创建数组 / 列表
来源：http://sef.dianchejie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://rvl.sysykeji.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vhs.zhoulong.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nqu.epnwcf.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://kbz.nwbrower.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://esg.fzhhl.top

Go:   arr := []int{1, 2, 3}
来源：http://dgf.guowangkeji.top

Ruby: arr = [1, 2, 3]
来源：http://hds.hysaishi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kdk.52xcode.cn

[D02] 追加元素到末尾
来源：http://vpn.wangdashe.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://umd.jinqigufen.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://noe.hesvh.cn

JS:   arr.push(4);
来源：http://gfg.hongshengwenyu.top

TS:   arr.push(4);
来源：http://wlj.xuanzx.com

Java: list.add(4);
来源：http://qlb.fzhhl.top

Go:   arr = append(arr, 4)
来源：http://ycs.jinyuanbaomall.cn

Ruby: arr << 4; arr.push(5)
来源：http://wnl.zhengqikj.top

C#:   list.Add(4);
来源：http://eug.ehwqpu.com

[D03] 在指定位置插入元素
来源：http://nhv.snrcjt.cn

Py:   arr.insert(0, 0)
来源：http://eoe.ybcxt.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vmm.zhixingplan.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wff.zdbjq.cn

TS:   arr.splice(0, 0, 0);
来源：http://ghh.jinqigfzy.top

Java: list.add(0, 0);
来源：http://gza.shuidangran.top

Go:   arr = append([]int{0}, arr...)
来源：http://uex.yueranfly.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ken.sufxvd.cn

C#:   list.Insert(0, 0);
来源：http://lgy.hongshengwenyu.top

[D04] 删除元素
来源：http://sdc.ppjwa.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jgq.zhoulong.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://twa.ydjk.org.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kbs.redwolf501.top

TS:   arr.splice(0, 1);
来源：http://lxt.jyoumei.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ndq.zhixingplan.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://abe.wangdashe.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://syd.jinghuilouyu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mvm.birdmap.top

[D05] 访问与修改元素
来源：http://cfq.daxiang520.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rtu.yj20258.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hul.gotoacloud.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kjm.hnxiangtu.top

TS:   arr[0]; arr.at(-1);
来源：http://zbu.redwolf501.top

Java: list.get(0); list.set(0, 9);
来源：http://kmq.chenlongwang.top

Go:   arr[0]; arr[0] = 9
来源：http://xpa.zycfv.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ttg.yvedp.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rdt.gotoacloud.top

[D06] 数组长度
来源：http://lyk.shanyushiyangtech.top

Py:   len(arr)
来源：http://api.gaohongyu789.top

PHP:  count($arr);
来源：http://ydi.tianlin.xyz

JS:   arr.length
来源：http://fvm.jlsjyb.cn

TS:   arr.length
来源：http://apn.kuanghao11.cn

Java: list.size();
来源：http://ggl.daria6918.cn

Go:   len(arr)
来源：http://gzo.shuidangran.top

Ruby: arr.length; arr.size
来源：http://snc.jinyuanbaomall.cn

C#:   list.Count;
来源：http://inu.andypj.xyz

[D07] 切片 / 取子数组
来源：http://ugv.aibaodan.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dzk.yj20258888.top

PHP:  array_slice($arr, 1, 3);
来源：http://fmk.pycfn.com

JS:   arr.slice(1, 4);
来源：http://xwa.daxiang520.top

TS:   arr.slice(1, 4);
来源：http://qta.uphjek.com

Java: list.subList(1, 4);
来源：http://svk.iojbl.cn

Go:   arr[1:4]
来源：http://tud.sufxvd.cn

Ruby: arr[1, 3]
来源：http://spn.xuanzx.com

C#:   list.GetRange(1, 3);
来源：http://okr.dianchejie.cn

[D08] 合并两个数组
来源：http://ndd.zdbjq.cn

Py:   a + b;  a.extend(b)
来源：http://iag.jinghuilouyu.cn

PHP:  array_merge($a, $b);
来源：http://hyf.hesvh.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://uop.iojbl.cn

TS:   [...a, ...b];
来源：http://vxz.jyoumei.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://awv.xinyue.icu

Go:   append(a, b...)
来源：http://ske.daria6918.cn

Ruby: a + b;  a.concat(b)
来源：http://zxk.jlsjyb.cn

C#:   a.Concat(b).ToList()
来源：http://ejg.gaohongyu789.top

[D09] 排序（升序）
来源：http://xqq.52xcode.cn

Py:   sorted(arr);  arr.sort()
来源：http://inm.redwolf501.top

PHP:  sort($arr);
来源：http://qni.redwolf501.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mxp.nanxinkj.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://vws.jqgufenzy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://igy.yuanzhike.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pxk.gogol.net.cn

Ruby: arr.sort
来源：http://jps.jinqigfzy.top

C#:   list.Sort();
来源：http://dya.9152youxi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://gyr.bbcook.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bik.316326.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xbw.snrcjt.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mrz.hywenlv.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mya.xziqi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gkl.gaohongyu789.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bxa.sjlbkw.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://edg.yj20258.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jgw.zdqjudy.top

[D11] 反转数组
来源：http://mhk.birdmap.top

Py:   arr[::-1];  arr.reverse()
来源：http://fud.aibaodan.cn

PHP:  array_reverse($arr);
来源：http://yiv.yanxiufei.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ahr.ywan-chungtsiang.top

TS:   [...arr].reverse();
来源：http://rhz.yfazqb.com

Java: Collections.reverse(list);
来源：http://oft.hcnkem.com

Go:   slices.Reverse(arr)
来源：http://ifm.ctjpmb.com

Ruby: arr.reverse
来源：http://mmd.hysaishi.cn

C#:   list.Reverse();
来源：http://pkc.yvedp.cn

[D12] 查找元素下标
来源：http://iyg.gotoacloud.top

Py:   arr.index(x);  x in arr
来源：http://tde.tian-w.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ooa.birdmap.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qjg.sysykeji.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sfc.jqgfzy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bvv.yj20258.top

Go:   slices.Index(arr, x)
来源：http://pkx.pengpengdd.cyou

Ruby: arr.index(x)
来源：http://vcr.zhoulong.xyz

C#:   list.IndexOf(x);
来源：http://kdi.gaohongyu789.top

[D13] 过滤（保留满足条件的）
来源：http://ynw.meibo888.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ybh.zhijiandao.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wmr.zhaomingkeji.xyz

JS:   arr.filter(x => x > 3)
来源：http://pkr.daria6918.cn

TS:   arr.filter(x => x > 3)
来源：http://nvb.tarul.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hrl.tianlin.xyz


<!-- 参考信息 -->