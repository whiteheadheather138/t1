代发 wailian999

[B13] 判断是否为数字
来源：http://spf.jianghu66.top

Py:   isinstance(x, (int, float))
来源：http://egb.pengpengdd.cyou

PHP:  is_numeric($x)
来源：http://tqo.jinqigufen.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tew.feifeiyinyue.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xna.jianghu66.top

Java: x instanceof Number
来源：http://gpy.fzhhl.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hem.yfazqb.com

Ruby: x.is_a?(Numeric)
来源：http://cgy.hnqzz.top

C#:   x is int or double or decimal
来源：http://xkc.jqgfzy.top

[B14] 判断值是否在集合内
来源：http://pek.xylfe.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jmo.yangfankeji.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://upx.birdmap.top

JS:   [1, 2, 3].includes(x)
来源：http://fak.nanxinkj.top

TS:   [1, 2, 3].includes(x)
来源：http://gea.sweek.top

Java: List.of(1, 2, 3).contains(x)
来源：http://otw.sysykeji.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ksy.ybcxt.top

Ruby: [1, 2, 3].include?(x)
来源：http://qed.yuanzhike.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zsk.yangfankeji.com

[B15] 布尔运算与取反
来源：http://ppj.fzhhl.top

Py:   a and b or not c
来源：http://ehh.redwolf501.top

PHP:  $a && $b || !$c
来源：http://xjh.tarul.cn

JS:   a && b || !c
来源：http://awy.nanxinkj.top

TS:   a && b || !c
来源：http://hqc.zhoulong.xyz

Java: a && b || !c
来源：http://ejc.hysaishi.cn

Go:   a && b || !c
来源：http://cgt.hcnkem.com

Ruby: a && b || !c
来源：http://oki.jiagoushi.top

C#:   a && b || !c
来源：http://iwy.wangshuangyany.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vjs.hnqzz.top

Py:   if not data: return
来源：http://joy.52xcode.cn

PHP:  if (!$data) { return; }
来源：http://qnx.zdbjq.cn

JS:   if (!data) return;
来源：http://pnf.c1oappe.top

TS:   if (!data) return;
来源：http://kac.guannengcc.top

Java: if (data == null) return;
来源：http://ncb.gogol.net.cn

Go:   if data == nil { return }
来源：http://eym.zycfv.cn

Ruby: return if data.nil?
来源：http://rbx.xuanzx.com

C#:   if (data == null) return;
来源：http://cqs.ybcxt.top

================================================================================
来源：http://eqv.shzxlz.cn

C. 函数与作用域
来源：http://qyd.ydjk.org.cn

================================================================================
来源：http://jqf.wangshuangyany.cn

[C01] 定义函数
来源：http://bcm.havefunace.top

Py:   def add(a, b): return a + b
来源：http://txm.hfpthk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pvn.gotoacloud.top

JS:   function add(a, b) { return a + b; }
来源：http://doi.cdnleiting.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nzh.ybcxt.top

Java: static int add(int a, int b) { return a + b; }
来源：http://mbh.nanxinkj.top

Go:   func add(a, b int) int { return a + b }
来源：http://iuz.fengsongda.top

Ruby: def add(a, b); a + b; end
来源：http://zma.tian-w.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kpf.xingfuxueyuan.xyz

[C02] 默认参数
来源：http://bpe.zhijiandao.cn

Py:   def greet(name="World"): return name
来源：http://ydd.yangfankeji.com

PHP:  function greet($name = "World") { return $name; }
来源：http://igu.zhiwuduotai.top

JS:   function greet(name = "World") { return name; }
来源：http://qpx.hesvh.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rdm.shangyingyoupin.top

Java: // 无默认参数：方法重载或 Optional
来源：http://tao.316326.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://odk.xuetiantiany.cn

Ruby: def greet(name = "World") = name
来源：http://ahf.hnxiangtu.top

C#:   string Greet(string name = "World") => name;
来源：http://vmy.c1oappe.top

[C03] 可变参数
来源：http://jof.hesvh.cn

Py:   def total(*args): return sum(args)
来源：http://imn.sxryk.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xku.c1oappe.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ruh.mhx1999.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tzw.yj202588.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://suk.ybcxt.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://uai.vqdsnc.cn

Ruby: def total(*nums); nums.sum; end
来源：http://drx.yueranfly.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xpx.havefunace.top

[C04] 命名参数 / 关键字参数
来源：http://qgs.ydzc1.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://oms.bjfxy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ztm.yvedp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qut.zhiwuduotai.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wdx.havefunace.top

Java: // 无：用 Builder 模式或 record
来源：http://oql.zhoulong.xyz

Go:   // 无：用配置结构体参数
来源：http://sef.havefunace.top

Ruby: f(a: 1, b: 2)
来源：http://ygn.sjlbkw.cn

C#:   f(a: 1, b: 2)
来源：http://lij.jqgfzy.top

[C05] 返回多个值
来源：http://anq.hesvh.cn

Py:   return a, b
来源：http://pmh.epnwcf.com

PHP:  return [$a, $b];
来源：http://awk.yuanzhike.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://fuq.aibaodan.cn

TS:   return { a, b };
来源：http://uuy.hesvh.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fpv.nanxuanxn.top

Go:   return a, b
来源：http://sdl.zhijiandao.cn

Ruby: return a, b
来源：http://upn.sysykeji.top

C#:   return (a, b);              // ValueTuple
来源：http://lwp.ydzc1.top

[C06] 匿名函数 / lambda
来源：http://fml.bbcook.cn

Py:   square = lambda x: x * x
来源：http://aww.sjlbkw.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ozz.nwbrower.top

JS:   const square = x => x * x;
来源：http://xic.wangdashe.top

TS:   const square = (x: number): number => x * x;
来源：http://bjz.daria6918.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cto.jlsjyb.cn

Go:   sq := func(x int) int { return x * x }
来源：http://lyf.meibo888.top

Ruby: square = ->(x) { x * x }
来源：http://xga.cheryme.top

C#:   Func<int, int> square = x => x * x;
来源：http://bxg.ivvv.top

[C07] 把函数作为参数传入
来源：http://fqb.fengsongda.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zhi.cqqwz.cn

PHP:  array_map("strtoupper", $arr);
来源：http://huk.tanke756.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fay.xylfe.cn

TS:   arr.map(String)
来源：http://jgo.yfazqb.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fow.hongshengwenyu.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://efw.hnxiangtu.top

Ruby: arr.map(&:upcase)
来源：http://ymm.gaohongyu789.top

C#:   arr.Select(s => s.ToUpper())
来源：http://zoo.yj202588.top

[C08] 闭包
来源：http://ljl.zhaomingkeji.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hut.wangdashe.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bbi.bjfxy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://aki.yuxming.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rve.ybcxt.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ddt.haohaochexian.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rtg.shanyushiyangtech.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hql.jqgfzy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vhi.tianlin.xyz

[C09] 递归
来源：http://dap.gzhubu.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://iew.chenlongwang.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tzf.yueranfly.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xof.nanxuanxn.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yim.tian-w.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yxo.meibo888.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pbi.pengpengdd.cyou

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nli.jqgfzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://duo.meibo888.top

[C10] 变量作用域
来源：http://akf.gaohongyu789.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fek.kuanghao11.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tle.yvedp.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jmp.xuetiantiany.cn

TS:   同 JS
来源：http://ivc.gotoacloud.top

Java: 方法内为块级作用域
来源：http://mcx.ybcxt.top

Go:   花括号块级作用域
来源：http://hvy.hywenlv.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hcz.yfazqb.com

C#:   块级作用域
来源：http://zml.cdnleiting.top

[C11] 模块导入与导出
来源：http://goy.bjfxy.top

Py:   from module import func
来源：http://cfe.andypj.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://kxu.yonumen.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://fqc.316326.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vrr.shanyushiyangtech.top

Java: import java.util.List;
来源：http://akf.yfazqb.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ycj.ydzc1.top

Ruby: require "json"; require_relative "./util"
来源：http://wlm.mhx1999.top

C#:   using System.Text;
来源：http://xna.cheryme.top

[C12] 立即执行函数 IIFE
来源：http://hsu.pycfn.com

Py:   (lambda: print("run"))()
来源：http://jpw.redwolf501.top

PHP:  (function () { echo "run"; })();
来源：http://fvd.ppjwa.cn

JS:   (() => { console.log("run"); })();
来源：http://gis.yj202588.top

TS:   (() => { console.log("run"); })();
来源：http://ziu.aizwys.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lfs.nanxuanxn.top

Go:   func() { fmt.Println("run") }()
来源：http://sqf.wangdashe.top

Ruby: -> { puts "run" }.call
来源：http://cfu.shanyushiyangkeji.top

C#:   // 无 IIFE：用静态构造函数
来源：http://dgu.iojbl.cn

[C13] 类型声明 / 类型注解
来源：http://klv.jinqigufen.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dus.feifeiyinyue.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ypi.jiagoushi.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pzo.cdnleiting.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qqj.hnqzz.top

Java: int add(int a, int b) { return a + b; }
来源：http://vgb.kuanghao11.cn

Go:   func add(a, b int) int
来源：http://nmq.redwolf501.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://chg.zdbjq.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ykw.0kj1m.cn

[C14] 泛型函数
来源：http://dwm.jqgufenzy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ezx.nwbrower.top

PHP:  // 无泛型
来源：http://hei.guowangkeji.top

JS:   // 无泛型
来源：http://zwi.cqqwz.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jsf.chenjidiqi.icu

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://btk.shanyushiyangtech.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rwk.gaohongyu789.top

Ruby: # 无泛型
来源：http://ffq.yj20258.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://anw.xziqi.cn

[C15] 解构 / 展开参数
来源：http://voz.shanyushiyangtech.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nus.aibaodan.cn

PHP:  [$a, $b] = $pair;
来源：http://dvd.hammf.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gss.haohaochexian.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://apk.jinqigufen.top

Java: // 无解构
来源：http://hxi.guowangkeji.top

Go:   // 无解构
来源：http://yxr.tianlin.xyz

Ruby: a, b = pair
来源：http://kum.tarul.cn

C#:   var (a, b) = pair;
来源：http://ida.fanxiaobao.xyz

[C16] 函数 / 方法重载
来源：http://ust.xingfuxueyuan.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wlk.tanke756.top

PHP:  // 无重载
来源：http://qyh.yuxming.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://edg.yvedp.cn

TS:   // 用联合类型或重载签名声明
来源：http://qac.feifeiyinyue.top

Java: void f(int a) {}  void f(String a) {}
来源：http://pqy.meibo888.top

Go:   // 无重载：用不同函数名
来源：http://rrb.quarkkingdee.top

Ruby: # 无重载：靠动态参数
来源：http://uef.aizwys.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://jey.jqgfzy.top

================================================================================
来源：http://pmi.jinqigfzy.top

D. 数组 / 列表 / 集合
来源：http://dnz.tianlin.xyz

================================================================================
来源：http://qgv.haohaochexian.top

[D01] 创建数组 / 列表
来源：http://psa.tian-w.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://cyf.kuanghao11.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yxe.0kj1m.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ysl.hywenlv.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://glb.cashguo.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kic.yvedp.cn

Go:   arr := []int{1, 2, 3}
来源：http://oai.yongpay.top

Ruby: arr = [1, 2, 3]
来源：http://dhq.jlsjyb.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qls.ppjwa.cn

[D02] 追加元素到末尾
来源：http://goo.cashguo.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ayj.guowangkeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ueb.nwbrower.top

JS:   arr.push(4);
来源：http://lmd.wangdashe.top

TS:   arr.push(4);
来源：http://uek.zhiwuduotai.top

Java: list.add(4);
来源：http://gpj.ppjwa.cn

Go:   arr = append(arr, 4)
来源：http://sep.hnxiangtu.top

Ruby: arr << 4; arr.push(5)
来源：http://usy.yj202588.top

C#:   list.Add(4);
来源：http://syv.ivvv.top

[D03] 在指定位置插入元素
来源：http://htt.dashuyun.cn

Py:   arr.insert(0, 0)
来源：http://fhh.zhoulong.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qht.yangfankeji.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hlq.daxiang520.top

TS:   arr.splice(0, 0, 0);
来源：http://uez.chenjidiqi.icu

Java: list.add(0, 0);
来源：http://ghr.52xcode.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jqm.jinghuilouyu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sxe.zhixingplan.top

C#:   list.Insert(0, 0);
来源：http://mlu.ivvv.top

[D04] 删除元素
来源：http://tvz.zhongyouzk.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ytt.zhixingplan.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fvo.ehwqpu.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mqa.sweek.top

TS:   arr.splice(0, 1);
来源：http://cdu.bjfxy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dih.yueranfly.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rmo.cucudq.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://aha.gaohongyu789.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vsz.wangdashe.top

[D05] 访问与修改元素
来源：http://wob.tian-w.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xai.iojbl.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zew.wangdashe.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://iep.hnqzz.top

TS:   arr[0]; arr.at(-1);
来源：http://ehb.feifeiyinyue.top

Java: list.get(0); list.set(0, 9);
来源：http://kkj.fengsongda.top

Go:   arr[0]; arr[0] = 9
来源：http://gbe.fengsongda.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://txi.jqgufenzy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xwj.shanyushiyangtech.top

[D06] 数组长度
来源：http://hvz.nwbrower.top

Py:   len(arr)
来源：http://jzi.yongpay.top

PHP:  count($arr);
来源：http://nud.sweek.top

JS:   arr.length
来源：http://pgk.yanxiufei.cn

TS:   arr.length
来源：http://zov.xylfe.cn

Java: list.size();
来源：http://yye.meibo888.top

Go:   len(arr)
来源：http://itv.yangfankeji.com

Ruby: arr.length; arr.size
来源：http://xkz.jyoumei.cn

C#:   list.Count;
来源：http://rdk.dashuyun.cn

[D07] 切片 / 取子数组
来源：http://vsb.ywan-chungtsiang.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://oyv.hesvh.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vol.iojbl.cn

JS:   arr.slice(1, 4);
来源：http://kvz.zdqjudy.top

TS:   arr.slice(1, 4);
来源：http://klp.meibo888.top

Java: list.subList(1, 4);
来源：http://cnt.smart0.xyz

Go:   arr[1:4]
来源：http://lrm.fehbvm.com

Ruby: arr[1, 3]
来源：http://wjm.yangfankeji.com

C#:   list.GetRange(1, 3);
来源：http://pox.hongshengwenyu.top

[D08] 合并两个数组
来源：http://lak.ehwqpu.com

Py:   a + b;  a.extend(b)
来源：http://aif.xuetiantiany.cn

PHP:  array_merge($a, $b);
来源：http://bjz.xinyue.icu

JS:   [...a, ...b];  a.concat(b);
来源：http://nxp.vehdjk.com

TS:   [...a, ...b];
来源：http://auy.jlsjyb.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gdr.ybcxt.top

Go:   append(a, b...)
来源：http://bie.jiagoushi.top

Ruby: a + b;  a.concat(b)
来源：http://efq.feifeiyinyue.top

C#:   a.Concat(b).ToList()
来源：http://uyh.hammf.cn

[D09] 排序（升序）
来源：http://can.uphjek.com

Py:   sorted(arr);  arr.sort()
来源：http://ljn.fzhhl.top

PHP:  sort($arr);
来源：http://spz.yueranfly.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gmr.kuanghao11.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gia.yj20258888.top

Java: Collections.sort(list);  list.sort(null);
来源：http://lkl.shangyingyoupin.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ioz.pengpengdd.cyou

Ruby: arr.sort
来源：http://nvc.gogol.net.cn

C#:   list.Sort();
来源：http://oms.tarul.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qwx.ctjpmb.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yxd.cdnleiting.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vlb.fanxiaobao.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yqq.sweek.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wtf.fehbvm.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fhu.yuxming.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://oiu.cqqwz.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mrn.chenjidiqi.icu

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://iav.zhongyouzk.top

[D11] 反转数组
来源：http://owy.zhiwuduotai.top

Py:   arr[::-1];  arr.reverse()
来源：http://kct.jyoumei.cn

PHP:  array_reverse($arr);
来源：http://qqb.yonumen.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://evz.sjlbkw.cn

TS:   [...arr].reverse();
来源：http://fja.tarul.cn

Java: Collections.reverse(list);
来源：http://tjj.kuanghao11.cn

Go:   slices.Reverse(arr)
来源：http://wyt.jianghu66.top

Ruby: arr.reverse
来源：http://ynf.cucudq.cn

C#:   list.Reverse();
来源：http://wrt.mhx1999.top

[D12] 查找元素下标
来源：http://ijg.xingfuxueyuan.xyz

Py:   arr.index(x);  x in arr
来源：http://kos.sweek.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sti.uphjek.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kmc.fktsv.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tmi.zhaomingkeji.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tpv.316326.xyz

Go:   slices.Index(arr, x)
来源：http://tch.cdnleiting.top

Ruby: arr.index(x)
来源：http://vaw.sysykeji.top

C#:   list.IndexOf(x);
来源：http://kng.daria6918.cn

[D13] 过滤（保留满足条件的）
来源：http://hps.cucudq.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cyr.guowangkeji.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lku.jianghu66.top

JS:   arr.filter(x => x > 3)
来源：http://vtw.bbcook.cn

TS:   arr.filter(x => x > 3)
来源：http://nru.cdnleiting.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ltk.nanxinkj.top


<!-- 参考信息 -->