代发 wailian999

[B13] 判断是否为数字
来源：http://wom.xylfe.cn

Py:   isinstance(x, (int, float))
来源：http://xpy.sjlbkw.cn

PHP:  is_numeric($x)
来源：http://kie.yanxiufei.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hrt.vehdjk.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aoq.hywenlv.cn

Java: x instanceof Number
来源：http://mbl.quarkkingdee.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://sdc.fengsongda.top

Ruby: x.is_a?(Numeric)
来源：http://ohl.hesvh.cn

C#:   x is int or double or decimal
来源：http://omw.ybcxt.top

[B14] 判断值是否在集合内
来源：http://tdm.shanyushiyangtech.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://inc.hnxiangtu.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bxc.yonumen.top

JS:   [1, 2, 3].includes(x)
来源：http://lzn.ydjk.org.cn

TS:   [1, 2, 3].includes(x)
来源：http://ukx.jqgfzy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://uty.xingfuxueyuan.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qzb.hammf.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ljl.wangshuangyany.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lpj.yvedp.cn

[B15] 布尔运算与取反
来源：http://noh.cheryme.top

Py:   a and b or not c
来源：http://ola.shanyushiyangtech.top

PHP:  $a && $b || !$c
来源：http://lmu.shuidangran.top

JS:   a && b || !c
来源：http://yjq.dianchejie.cn

TS:   a && b || !c
来源：http://owf.zycfv.cn

Java: a && b || !c
来源：http://lyq.tanke756.top

Go:   a && b || !c
来源：http://mvm.nanxinkj.top

Ruby: a && b || !c
来源：http://jat.yj20258.top

C#:   a && b || !c
来源：http://mko.sufxvd.cn

[B16] 卫语句：不满足条件提前返回
来源：http://rcd.yfazqb.com

Py:   if not data: return
来源：http://ntk.xylfe.cn

PHP:  if (!$data) { return; }
来源：http://gks.zhixingplan.top

JS:   if (!data) return;
来源：http://dsu.aibaodan.cn

TS:   if (!data) return;
来源：http://pfl.guowangkeji.top

Java: if (data == null) return;
来源：http://bgx.hnxiangtu.top

Go:   if data == nil { return }
来源：http://cdy.mhx1999.top

Ruby: return if data.nil?
来源：http://vml.jinqigfzy.top

C#:   if (data == null) return;
来源：http://clo.xinyue.icu

================================================================================
来源：http://unf.zdbjq.cn

C. 函数与作用域
来源：http://yfm.tarul.cn

================================================================================
来源：http://jxh.shzxlz.cn

[C01] 定义函数
来源：http://udx.vqdsnc.cn

Py:   def add(a, b): return a + b
来源：http://aed.yuanzhike.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mki.vqdsnc.cn

JS:   function add(a, b) { return a + b; }
来源：http://axi.yj20258888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lbd.ybcxt.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ynm.iojbl.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ucg.0kj1m.cn

Ruby: def add(a, b); a + b; end
来源：http://uoq.chenjidiqi.icu

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ftp.hnxiangtu.top

[C02] 默认参数
来源：http://hmx.haohaochexian.top

Py:   def greet(name="World"): return name
来源：http://sxr.hesvh.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dxv.tarul.cn

JS:   function greet(name = "World") { return name; }
来源：http://eha.tian-w.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xbx.fanxiaobao.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://ixx.yonumen.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://waj.ppjwa.cn

Ruby: def greet(name = "World") = name
来源：http://kbf.yfazqb.com

C#:   string Greet(string name = "World") => name;
来源：http://dll.yuxming.cn

[C03] 可变参数
来源：http://ufi.yvedp.cn

Py:   def total(*args): return sum(args)
来源：http://wzm.zhiwuduotai.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://juq.chenjidiqi.icu

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lfu.zhoulong.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qyq.hcnkem.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xcb.nwbrower.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wxh.xuanzx.com

Ruby: def total(*nums); nums.sum; end
来源：http://mfc.jinqigfzy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qdg.quarkkingdee.top

[C04] 命名参数 / 关键字参数
来源：http://lzv.zycfv.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jhs.shzxlz.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yug.zhaomingkeji.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bqy.zhongyouzk.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qas.nanxuanxn.top

Java: // 无：用 Builder 模式或 record
来源：http://vdx.zhiwuduotai.top

Go:   // 无：用配置结构体参数
来源：http://gty.yvedp.cn

Ruby: f(a: 1, b: 2)
来源：http://hto.nanxinkj.top

C#:   f(a: 1, b: 2)
来源：http://glw.tarul.cn

[C05] 返回多个值
来源：http://zte.jqgfzy.top

Py:   return a, b
来源：http://bvp.hysaishi.cn

PHP:  return [$a, $b];
来源：http://pjh.52xcode.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://kwl.fehbvm.com

TS:   return { a, b };
来源：http://tjr.shanyushiyangkeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://juo.jqgfzy.top

Go:   return a, b
来源：http://pqs.iojbl.cn

Ruby: return a, b
来源：http://znz.ybcxt.top

C#:   return (a, b);              // ValueTuple
来源：http://nrp.xylfe.cn

[C06] 匿名函数 / lambda
来源：http://bll.yonumen.top

Py:   square = lambda x: x * x
来源：http://jgc.chenjidiqi.icu

PHP:  $square = fn($x) => $x * $x;
来源：http://ini.9152youxi.cn

JS:   const square = x => x * x;
来源：http://kzh.redwolf501.top

TS:   const square = (x: number): number => x * x;
来源：http://kbp.ivvv.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hgr.quarkkingdee.top

Go:   sq := func(x int) int { return x * x }
来源：http://rdh.wangshuangyany.cn

Ruby: square = ->(x) { x * x }
来源：http://gdd.hesvh.cn

C#:   Func<int, int> square = x => x * x;
来源：http://gil.jianghu66.top

[C07] 把函数作为参数传入
来源：http://vuu.vqdsnc.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://coa.hongshengwenyu.top

PHP:  array_map("strtoupper", $arr);
来源：http://obh.jinqigfzy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kmf.shzxlz.cn

TS:   arr.map(String)
来源：http://wqd.zhijiandao.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://slh.yueranfly.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zoc.cheryme.top

Ruby: arr.map(&:upcase)
来源：http://ejo.tian-w.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://uoi.hesvh.cn

[C08] 闭包
来源：http://poq.bbcook.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rfg.shanyushiyangtech.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rfp.fengsongda.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://whi.hammf.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://njj.cucudq.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ela.sweek.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ege.dianchejie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fyj.hcnkem.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://djn.haohaochexian.top

[C09] 递归
来源：http://zue.ehwqpu.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nza.xuetiantiany.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cpo.yfazqb.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vte.hywenlv.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wev.guannengcc.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ynk.zhoulong.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tvq.jyoumei.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fqi.zhengqikj.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rwz.hnqzz.top

[C10] 变量作用域
来源：http://wfa.chenlongwang.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://uvs.jianghu66.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qfm.yj20258888.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ktm.pengpengdd.cyou

TS:   同 JS
来源：http://ody.pycfn.com

Java: 方法内为块级作用域
来源：http://xas.nwbrower.top

Go:   花括号块级作用域
来源：http://ggq.ppjwa.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ifw.bjfxy.top

C#:   块级作用域
来源：http://tls.hcnkem.com

[C11] 模块导入与导出
来源：http://bcl.hammf.cn

Py:   from module import func
来源：http://yft.snrcjt.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://kin.sysykeji.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://eeo.jqgfzy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ntr.epnwcf.com

Java: import java.util.List;
来源：http://poo.jiagoushi.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tgz.zhongyouzk.top

Ruby: require "json"; require_relative "./util"
来源：http://tgd.meibo888.top

C#:   using System.Text;
来源：http://icf.jinqigfzy.top

[C12] 立即执行函数 IIFE
来源：http://fcw.feifeiyinyue.top

Py:   (lambda: print("run"))()
来源：http://lcw.redwolf501.top

PHP:  (function () { echo "run"; })();
来源：http://oks.hongshengwenyu.top

JS:   (() => { console.log("run"); })();
来源：http://nxz.fengsongda.top

TS:   (() => { console.log("run"); })();
来源：http://xii.xylfe.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qgk.bjfxy.top

Go:   func() { fmt.Println("run") }()
来源：http://xdg.jinyuanbaomall.cn

Ruby: -> { puts "run" }.call
来源：http://gpa.zycfv.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://nyi.daxiang520.top

[C13] 类型声明 / 类型注解
来源：http://kni.gaohongyu789.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yvz.yj20258888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://erk.gaohongyu789.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://aaa.gzhubu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jws.hongshengwenyu.top

Java: int add(int a, int b) { return a + b; }
来源：http://tgl.yangfankeji.com

Go:   func add(a, b int) int
来源：http://rvg.kuanghao11.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lge.feifeiyinyue.top

C#:   int Add(int a, int b) => a + b;
来源：http://jhh.yvedp.cn

[C14] 泛型函数
来源：http://exp.iojbl.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jne.vqdsnc.cn

PHP:  // 无泛型
来源：http://pke.dianchejie.cn

JS:   // 无泛型
来源：http://tvf.yuxming.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nwx.redwolf501.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nqh.52xcode.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kes.hnqzz.top

Ruby: # 无泛型
来源：http://szw.vehdjk.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ibm.haohaochexian.top

[C15] 解构 / 展开参数
来源：http://vbz.bbcook.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://owq.316326.xyz

PHP:  [$a, $b] = $pair;
来源：http://xcs.epnwcf.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://sou.tianlin.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://neu.havefunace.top

Java: // 无解构
来源：http://kmt.fktsv.cn

Go:   // 无解构
来源：http://yrz.tanke756.top

Ruby: a, b = pair
来源：http://squ.xinyue.icu

C#:   var (a, b) = pair;
来源：http://wnc.sjlbkw.cn

[C16] 函数 / 方法重载
来源：http://kvf.smart0.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gjw.guannengcc.top

PHP:  // 无重载
来源：http://dus.gogol.net.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zed.hnxiangtu.top

TS:   // 用联合类型或重载签名声明
来源：http://men.guowangkeji.top

Java: void f(int a) {}  void f(String a) {}
来源：http://vav.wangdashe.top

Go:   // 无重载：用不同函数名
来源：http://buv.epnwcf.com

Ruby: # 无重载：靠动态参数
来源：http://ktt.kuanghao11.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://pgm.shanyushiyangkeji.top

================================================================================
来源：http://ict.jinqigufen.top

D. 数组 / 列表 / 集合
来源：http://hgw.daxiang520.top

================================================================================
来源：http://wcp.zycfv.cn

[D01] 创建数组 / 列表
来源：http://ydj.shzxlz.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://fqn.tian-w.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vri.feifeiyinyue.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ftl.mhx1999.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://rrx.cheryme.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ruz.shanyushiyangtech.top

Go:   arr := []int{1, 2, 3}
来源：http://peu.mhx1999.top

Ruby: arr = [1, 2, 3]
来源：http://hde.hysaishi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bmb.yangfankeji.com

[D02] 追加元素到末尾
来源：http://znp.guowangkeji.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gee.zdqjudy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://prw.yangfankeji.com

JS:   arr.push(4);
来源：http://ytg.yanxiufei.cn

TS:   arr.push(4);
来源：http://hvy.cheryme.top

Java: list.add(4);
来源：http://efo.feifeiyinyue.top

Go:   arr = append(arr, 4)
来源：http://nwt.yangfankeji.com

Ruby: arr << 4; arr.push(5)
来源：http://wvs.jqgufenzy.top

C#:   list.Add(4);
来源：http://qus.wangdashe.top

[D03] 在指定位置插入元素
来源：http://kfn.sufxvd.cn

Py:   arr.insert(0, 0)
来源：http://ubf.jqgufenzy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fqm.hysaishi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hqn.yvedp.cn

TS:   arr.splice(0, 0, 0);
来源：http://yrk.bbcook.cn

Java: list.add(0, 0);
来源：http://okv.chenzaomai.com

Go:   arr = append([]int{0}, arr...)
来源：http://ccg.yj202588.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qtt.jinyuanbaomall.cn

C#:   list.Insert(0, 0);
来源：http://aeg.xinyue.icu

[D04] 删除元素
来源：http://ciw.fzhhl.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fsk.cashguo.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cgq.xuanzx.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://eat.zhoulong.xyz

TS:   arr.splice(0, 1);
来源：http://lfg.fengsongda.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qzd.jianghu66.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://one.shanyushiyangkeji.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://quu.haohaochexian.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zuh.jinqigfzy.top

[D05] 访问与修改元素
来源：http://rjn.9152youxi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ivp.jlsjyb.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://onl.yanxiufei.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://juu.cheryme.top

TS:   arr[0]; arr.at(-1);
来源：http://sri.ppjwa.cn

Java: list.get(0); list.set(0, 9);
来源：http://dhy.meibo888.top

Go:   arr[0]; arr[0] = 9
来源：http://aob.jiagoushi.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://eif.fktsv.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://icq.zhengqikj.top

[D06] 数组长度
来源：http://yis.0kj1m.cn

Py:   len(arr)
来源：http://cmr.xylfe.cn

PHP:  count($arr);
来源：http://rwi.zycfv.cn

JS:   arr.length
来源：http://apy.jinyuanbaomall.cn

TS:   arr.length
来源：http://mee.nwbrower.top

Java: list.size();
来源：http://chw.svipenyu.cn

Go:   len(arr)
来源：http://dcc.shangyingyoupin.top

Ruby: arr.length; arr.size
来源：http://tfk.yvedp.cn

C#:   list.Count;
来源：http://dbx.cheryme.top

[D07] 切片 / 取子数组
来源：http://pxc.nanxuanxn.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nme.pycfn.com

PHP:  array_slice($arr, 1, 3);
来源：http://zdo.chenzaomai.com

JS:   arr.slice(1, 4);
来源：http://ata.gotoacloud.top

TS:   arr.slice(1, 4);
来源：http://zqf.jqgfzy.top

Java: list.subList(1, 4);
来源：http://pge.hcnkem.com

Go:   arr[1:4]
来源：http://hzr.uphjek.com

Ruby: arr[1, 3]
来源：http://bkh.wangshuangyany.cn

C#:   list.GetRange(1, 3);
来源：http://jxn.zdqjudy.top

[D08] 合并两个数组
来源：http://hvb.hysaishi.cn

Py:   a + b;  a.extend(b)
来源：http://hxr.nwbrower.top

PHP:  array_merge($a, $b);
来源：http://sgz.zdbjq.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ioq.hywenlv.cn

TS:   [...a, ...b];
来源：http://aju.jqgufenzy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qic.ybcxt.top

Go:   append(a, b...)
来源：http://bdw.zhixingplan.top

Ruby: a + b;  a.concat(b)
来源：http://ksd.52xcode.cn

C#:   a.Concat(b).ToList()
来源：http://gfq.zhijiandao.cn

[D09] 排序（升序）
来源：http://tee.zhixingplan.top

Py:   sorted(arr);  arr.sort()
来源：http://jsu.hysaishi.cn

PHP:  sort($arr);
来源：http://lfr.gaohongyu789.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zoz.xingfuxueyuan.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://xgk.xingfuxueyuan.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://xoz.mhx1999.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://idt.yueranfly.top

Ruby: arr.sort
来源：http://mav.meibo888.top

C#:   list.Sort();
来源：http://pwn.zhaomingkeji.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://sbb.gaohongyu789.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://edh.zhongyouzk.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zxd.smart0.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lib.zdbjq.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xjn.dashuyun.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://waw.shzxlz.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kcm.jinqigufen.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kgr.dianchejie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lva.xylfe.cn

[D11] 反转数组
来源：http://kbn.zdbjq.cn

Py:   arr[::-1];  arr.reverse()
来源：http://rvn.yonumen.top

PHP:  array_reverse($arr);
来源：http://yhl.hesvh.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bor.pycfn.com

TS:   [...arr].reverse();
来源：http://gsu.zhaomingkeji.xyz

Java: Collections.reverse(list);
来源：http://dwe.iojbl.cn

Go:   slices.Reverse(arr)
来源：http://sya.cqqwz.cn

Ruby: arr.reverse
来源：http://rrx.gotoacloud.top

C#:   list.Reverse();
来源：http://tux.svipenyu.cn

[D12] 查找元素下标
来源：http://gnp.zhongyouzk.top

Py:   arr.index(x);  x in arr
来源：http://sxg.gotoacloud.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fpo.yanxiufei.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mzb.fktsv.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tkw.daxiang520.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ouw.guannengcc.top

Go:   slices.Index(arr, x)
来源：http://lau.hammf.cn

Ruby: arr.index(x)
来源：http://qkg.cheryme.top

C#:   list.IndexOf(x);
来源：http://xiq.316326.xyz

[D13] 过滤（保留满足条件的）
来源：http://guu.gaohongyu789.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://snh.fengsongda.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ixt.gotoacloud.top

JS:   arr.filter(x => x > 3)
来源：http://plo.sufxvd.cn

TS:   arr.filter(x => x > 3)
来源：http://gjz.yuanzhike.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mik.fktsv.cn


<!-- 参考信息 -->