代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dom.feifeiyinyue.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://iyg.aibaodan.cn

[B11] 生成数字序列 / 区间
来源：http://lvs.yuxming.cn

Py:   list(range(0, 10, 2))
来源：http://vpk.uphjek.com

PHP:  range(0, 10, 2);
来源：http://bwb.guannengcc.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vik.aizwys.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ykw.hysaishi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ygd.zhongyouzk.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yyj.tian-w.cn

Ruby: (0...10).step(2).to_a
来源：http://see.daria6918.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hzt.hcnkem.com

[B12] 跳出多层循环
来源：http://yav.chenjidiqi.icu

Py:   # 无标签跳转：抽成函数用 return
来源：http://yac.sxryk.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zfv.quarkkingdee.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sob.dashuyun.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kgm.jqgfzy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bhc.snrcjt.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uvf.vqdsnc.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://siw.pengpengdd.cyou

C#:   # 无标签：用 goto label 或布尔标志
来源：http://abo.52xcode.cn

[B13] 判断是否为数字
来源：http://naz.bbcook.cn

Py:   isinstance(x, (int, float))
来源：http://wky.0kj1m.cn

PHP:  is_numeric($x)
来源：http://nka.xingfuxueyuan.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://llg.chenzaomai.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jhf.pengpengdd.cyou

Java: x instanceof Number
来源：http://uts.dashuyun.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ofq.svipenyu.cn

Ruby: x.is_a?(Numeric)
来源：http://cil.pengpengdd.cyou

C#:   x is int or double or decimal
来源：http://pct.sysykeji.top

[B14] 判断值是否在集合内
来源：http://mow.dashuyun.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nvy.xingfuxueyuan.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://oyv.cashguo.top

JS:   [1, 2, 3].includes(x)
来源：http://wgf.jyoumei.cn

TS:   [1, 2, 3].includes(x)
来源：http://fbn.c1oappe.top

Java: List.of(1, 2, 3).contains(x)
来源：http://wgc.cheryme.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hdt.pengpengdd.cyou

Ruby: [1, 2, 3].include?(x)
来源：http://wup.gotoacloud.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uyr.svipenyu.cn

[B15] 布尔运算与取反
来源：http://xbi.bbcook.cn

Py:   a and b or not c
来源：http://prz.nwbrower.top

PHP:  $a && $b || !$c
来源：http://qqx.yongpay.top

JS:   a && b || !c
来源：http://qgv.haohaochexian.top

TS:   a && b || !c
来源：http://gve.aizwys.cn

Java: a && b || !c
来源：http://ekz.jinqigufen.top

Go:   a && b || !c
来源：http://zfe.fengsongda.top

Ruby: a && b || !c
来源：http://szm.birdmap.top

C#:   a && b || !c
来源：http://vhq.cashguo.top

[B16] 卫语句：不满足条件提前返回
来源：http://bts.aibaodan.cn

Py:   if not data: return
来源：http://vnb.zhixingplan.top

PHP:  if (!$data) { return; }
来源：http://hdd.smart0.xyz

JS:   if (!data) return;
来源：http://qfc.sjlbkw.cn

TS:   if (!data) return;
来源：http://zii.tianlin.xyz

Java: if (data == null) return;
来源：http://ift.xylfe.cn

Go:   if data == nil { return }
来源：http://gkc.9152youxi.cn

Ruby: return if data.nil?
来源：http://lgm.shuidangran.top

C#:   if (data == null) return;
来源：http://yxp.bbcook.cn

================================================================================
来源：http://lpk.epnwcf.com

C. 函数与作用域
来源：http://thw.zhaomingkeji.xyz

================================================================================
来源：http://wmt.zdqjudy.top

[C01] 定义函数
来源：http://llq.ehwqpu.com

Py:   def add(a, b): return a + b
来源：http://ovw.sufxvd.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gcm.jinqigfzy.top

JS:   function add(a, b) { return a + b; }
来源：http://jts.fanxiaobao.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ccp.chenzaomai.com

Java: static int add(int a, int b) { return a + b; }
来源：http://ygu.shanyushiyangkeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://hgy.yvedp.cn

Ruby: def add(a, b); a + b; end
来源：http://qza.ehwqpu.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qvs.sysykeji.top

[C02] 默认参数
来源：http://hki.ybcxt.top

Py:   def greet(name="World"): return name
来源：http://yir.xuetiantiany.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://nlg.jiagoushi.top

JS:   function greet(name = "World") { return name; }
来源：http://epl.cashguo.top

TS:   function greet(name: string = "World") { return name; }
来源：http://wvk.xuetiantiany.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vrg.chenlongwang.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jqo.redwolf501.top

Ruby: def greet(name = "World") = name
来源：http://cpt.yuxming.cn

C#:   string Greet(string name = "World") => name;
来源：http://jbq.smart0.xyz

[C03] 可变参数
来源：http://xsy.ydzc1.top

Py:   def total(*args): return sum(args)
来源：http://nip.ctjpmb.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fku.jqgfzy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ptt.zhongyouzk.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bxd.hywenlv.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pma.shangyingyoupin.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://woo.zhoulong.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://tgd.9152youxi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lwa.mhx1999.top

[C04] 命名参数 / 关键字参数
来源：http://crh.iojbl.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zqi.shzxlz.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tjr.yvedp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ktm.ydzc1.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lfd.feifeiyinyue.top

Java: // 无：用 Builder 模式或 record
来源：http://cbp.hnxiangtu.top

Go:   // 无：用配置结构体参数
来源：http://lxv.xinyue.icu

Ruby: f(a: 1, b: 2)
来源：http://jfg.ctjpmb.com

C#:   f(a: 1, b: 2)
来源：http://tjf.zhiwuduotai.top

[C05] 返回多个值
来源：http://vul.gaohongyu789.top

Py:   return a, b
来源：http://urf.shanyushiyangtech.top

PHP:  return [$a, $b];
来源：http://wrl.daxiang520.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ayv.mhx1999.top

TS:   return { a, b };
来源：http://pmg.pycfn.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qni.hnqzz.top

Go:   return a, b
来源：http://zgj.ywan-chungtsiang.top

Ruby: return a, b
来源：http://sco.zhiwuduotai.top

C#:   return (a, b);              // ValueTuple
来源：http://ede.zdbjq.cn

[C06] 匿名函数 / lambda
来源：http://ngp.0kj1m.cn

Py:   square = lambda x: x * x
来源：http://ajm.redwolf501.top

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.yuxming.cn

JS:   const square = x => x * x;
来源：http://nxf.birdmap.top

TS:   const square = (x: number): number => x * x;
来源：http://kts.snrcjt.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://iaa.cucudq.cn

Go:   sq := func(x int) int { return x * x }
来源：http://qur.ydjk.org.cn

Ruby: square = ->(x) { x * x }
来源：http://pqk.andypj.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://boi.jiagoushi.top

[C07] 把函数作为参数传入
来源：http://vdn.jianghu66.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jnm.yonumen.top

PHP:  array_map("strtoupper", $arr);
来源：http://nmw.cheryme.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lah.jqgfzy.top

TS:   arr.map(String)
来源：http://qsg.zhoulong.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mkb.yj202588.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mbz.hnxiangtu.top

Ruby: arr.map(&:upcase)
来源：http://uwa.yj202588.top

C#:   arr.Select(s => s.ToUpper())
来源：http://vec.hcnkem.com

[C08] 闭包
来源：http://riw.bjfxy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nwe.redwolf501.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mnh.shangyingyoupin.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gnb.yonumen.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mtr.mhx1999.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://aqr.aizwys.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://uql.nanxuanxn.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zuc.haohaochexian.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://onf.redwolf501.top

[C09] 递归
来源：http://ibx.andypj.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yjg.smart0.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ist.cashguo.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://srx.zhoulong.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tcq.redwolf501.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ofy.uphjek.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rwo.tianlin.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pja.tianlin.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nqn.cashguo.top

[C10] 变量作用域
来源：http://yfb.cucudq.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://erd.svipenyu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kie.jianghu66.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cle.kuanghao11.cn

TS:   同 JS
来源：http://skn.yonumen.top

Java: 方法内为块级作用域
来源：http://jyl.redwolf501.top

Go:   花括号块级作用域
来源：http://dpt.wangdashe.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jri.zhixingplan.top

C#:   块级作用域
来源：http://nep.sxryk.cn

[C11] 模块导入与导出
来源：http://npk.birdmap.top

Py:   from module import func
来源：http://iqu.iojbl.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://oir.guowangkeji.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://gta.wangshuangyany.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xsq.jlsjyb.cn

Java: import java.util.List;
来源：http://jyd.zdbjq.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://abn.sweek.top

Ruby: require "json"; require_relative "./util"
来源：http://opm.hesvh.cn

C#:   using System.Text;
来源：http://guf.fzhhl.top

[C12] 立即执行函数 IIFE
来源：http://bif.pengpengdd.cyou

Py:   (lambda: print("run"))()
来源：http://rsc.pengpengdd.cyou

PHP:  (function () { echo "run"; })();
来源：http://cdm.havefunace.top

JS:   (() => { console.log("run"); })();
来源：http://hpx.sweek.top

TS:   (() => { console.log("run"); })();
来源：http://tgt.zdqjudy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fov.yj202588.top

Go:   func() { fmt.Println("run") }()
来源：http://lgx.zhongyouzk.top

Ruby: -> { puts "run" }.call
来源：http://wis.aizwys.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://nts.jyoumei.cn

[C13] 类型声明 / 类型注解
来源：http://qkh.hysaishi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://abf.316326.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://syk.ctjpmb.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lon.bjfxy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dpi.dianchejie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://raw.hesvh.cn

Go:   func add(a, b int) int
来源：http://wud.cucudq.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qqc.meibo888.top

C#:   int Add(int a, int b) => a + b;
来源：http://grn.yangfankeji.com

[C14] 泛型函数
来源：http://rws.quarkkingdee.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tds.tarul.cn

PHP:  // 无泛型
来源：http://crx.zhoulong.xyz

JS:   // 无泛型
来源：http://xzw.chenzaomai.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tbw.tarul.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yck.kuanghao11.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zmj.haohaochexian.top

Ruby: # 无泛型
来源：http://gda.hesvh.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wou.hesvh.cn

[C15] 解构 / 展开参数
来源：http://kps.yuanzhike.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://aco.snrcjt.cn

PHP:  [$a, $b] = $pair;
来源：http://evt.shanyushiyangkeji.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rel.jlsjyb.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fui.yonumen.top

Java: // 无解构
来源：http://qyu.xinyue.icu

Go:   // 无解构
来源：http://wsr.jianghu66.top

Ruby: a, b = pair
来源：http://cik.tarul.cn

C#:   var (a, b) = pair;
来源：http://fwv.yj20258888.top

[C16] 函数 / 方法重载
来源：http://oce.birdmap.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sba.hysaishi.cn

PHP:  // 无重载
来源：http://mmq.shanyushiyangkeji.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://xfm.vqdsnc.cn

TS:   // 用联合类型或重载签名声明
来源：http://ykd.chenjidiqi.icu

Java: void f(int a) {}  void f(String a) {}
来源：http://cnx.zhijiandao.cn

Go:   // 无重载：用不同函数名
来源：http://ste.zdbjq.cn

Ruby: # 无重载：靠动态参数
来源：http://hqe.zhengqikj.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://zsc.vqdsnc.cn

================================================================================
来源：http://tdd.sweek.top

D. 数组 / 列表 / 集合
来源：http://exo.hfpthk.cn

================================================================================
来源：http://sye.smart0.xyz

[D01] 创建数组 / 列表
来源：http://gpv.zhengqikj.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://jym.zhengqikj.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ikp.bbcook.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yef.shzxlz.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://gnz.smart0.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fmx.sysykeji.top

Go:   arr := []int{1, 2, 3}
来源：http://qcn.guowangkeji.top

Ruby: arr = [1, 2, 3]
来源：http://bds.xuanzx.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ajc.yueranfly.top

[D02] 追加元素到末尾
来源：http://wgb.jyoumei.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pzk.tarul.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ule.hcnkem.com

JS:   arr.push(4);
来源：http://jyv.gogol.net.cn

TS:   arr.push(4);
来源：http://hpj.bjfxy.top

Java: list.add(4);
来源：http://zzb.jyoumei.cn

Go:   arr = append(arr, 4)
来源：http://sxb.ivvv.top

Ruby: arr << 4; arr.push(5)
来源：http://koq.guannengcc.top

C#:   list.Add(4);
来源：http://fwo.yfazqb.com

[D03] 在指定位置插入元素
来源：http://mdt.daxiang520.top

Py:   arr.insert(0, 0)
来源：http://apq.jianghu66.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://itl.tarul.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yve.fehbvm.com

TS:   arr.splice(0, 0, 0);
来源：http://xai.jlsjyb.cn

Java: list.add(0, 0);
来源：http://qpa.tianlin.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://xon.jiagoushi.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rhe.yj202588.top

C#:   list.Insert(0, 0);
来源：http://bbv.nanxinkj.top

[D04] 删除元素
来源：http://hbr.sweek.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wqn.wangdashe.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fei.kuanghao11.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fko.havefunace.top

TS:   arr.splice(0, 1);
来源：http://pyg.zhiwuduotai.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mgb.xylfe.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kbd.snrcjt.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://uci.yj202588.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zgx.nanxuanxn.top

[D05] 访问与修改元素
来源：http://gns.wangdashe.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pya.shangyingyoupin.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yzz.zhixingplan.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nri.zdbjq.cn

TS:   arr[0]; arr.at(-1);
来源：http://odi.bbcook.cn

Java: list.get(0); list.set(0, 9);
来源：http://ain.jinghuilouyu.cn

Go:   arr[0]; arr[0] = 9
来源：http://qhp.vehdjk.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wsd.yj20258.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ihe.gaohongyu789.top

[D06] 数组长度
来源：http://dwf.guowangkeji.top

Py:   len(arr)
来源：http://kee.daxiang520.top

PHP:  count($arr);
来源：http://wbk.jqgufenzy.top

JS:   arr.length
来源：http://yod.xinyue.icu

TS:   arr.length
来源：http://wxg.yongpay.top

Java: list.size();
来源：http://hyd.gotoacloud.top

Go:   len(arr)
来源：http://jlp.chenzaomai.com

Ruby: arr.length; arr.size
来源：http://wcw.fktsv.cn

C#:   list.Count;
来源：http://csj.yuxming.cn

[D07] 切片 / 取子数组
来源：http://ewo.cheryme.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wyu.cashguo.top

PHP:  array_slice($arr, 1, 3);
来源：http://has.uphjek.com

JS:   arr.slice(1, 4);
来源：http://cae.uphjek.com

TS:   arr.slice(1, 4);
来源：http://bvk.zhijiandao.cn

Java: list.subList(1, 4);
来源：http://hib.zdbjq.cn

Go:   arr[1:4]
来源：http://kla.zhoulong.xyz

Ruby: arr[1, 3]
来源：http://svc.yfazqb.com

C#:   list.GetRange(1, 3);
来源：http://jxm.snrcjt.cn

[D08] 合并两个数组
来源：http://dqt.ppjwa.cn

Py:   a + b;  a.extend(b)
来源：http://npu.daxiang520.top

PHP:  array_merge($a, $b);
来源：http://car.316326.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://wgy.daria6918.cn

TS:   [...a, ...b];
来源：http://ydb.aibaodan.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://uls.yj20258.top

Go:   append(a, b...)
来源：http://mky.daria6918.cn

Ruby: a + b;  a.concat(b)
来源：http://xtf.dianchejie.cn

C#:   a.Concat(b).ToList()
来源：http://acz.wangdashe.top

[D09] 排序（升序）
来源：http://fqt.yuanzhike.top

Py:   sorted(arr);  arr.sort()
来源：http://puu.shangyingyoupin.top

PHP:  sort($arr);
来源：http://ukg.hnqzz.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://abe.wangdashe.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://tvf.zhaomingkeji.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://rqt.yongpay.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zos.fanxiaobao.xyz

Ruby: arr.sort
来源：http://vgi.jqgfzy.top

C#:   list.Sort();
来源：http://wdq.wangdashe.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://dce.daxiang520.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nmz.tanke756.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://efp.gaohongyu789.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://twm.jianghu66.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ptz.shzxlz.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lsk.xziqi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ttr.jianghu66.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xio.sjlbkw.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ewy.hesvh.cn

[D11] 反转数组
来源：http://bnl.iojbl.cn

Py:   arr[::-1];  arr.reverse()
来源：http://hss.xingfuxueyuan.xyz

PHP:  array_reverse($arr);
来源：http://ooc.shanyushiyangtech.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nsk.xuanzx.com


<!-- 参考信息 -->