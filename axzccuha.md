代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://vzj.uphjek.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jwq.nwbrower.top

[B15] 布尔运算与取反
来源：http://yrf.zdqjudy.top

Py:   a and b or not c
来源：http://dbm.cucudq.cn

PHP:  $a && $b || !$c
来源：http://foh.ctjpmb.com

JS:   a && b || !c
来源：http://kgf.bbcook.cn

TS:   a && b || !c
来源：http://dpo.ydzc1.top

Java: a && b || !c
来源：http://pjb.ctjpmb.com

Go:   a && b || !c
来源：http://ydu.nanxuanxn.top

Ruby: a && b || !c
来源：http://ehi.c1oappe.top

C#:   a && b || !c
来源：http://ljz.pengpengdd.cyou

[B16] 卫语句：不满足条件提前返回
来源：http://xht.yongpay.top

Py:   if not data: return
来源：http://itw.xuanzx.com

PHP:  if (!$data) { return; }
来源：http://tzq.tarul.cn

JS:   if (!data) return;
来源：http://xqw.bjfxy.top

TS:   if (!data) return;
来源：http://dyn.jinyuanbaomall.cn

Java: if (data == null) return;
来源：http://xwt.chenjidiqi.icu

Go:   if data == nil { return }
来源：http://ckv.zhongyouzk.top

Ruby: return if data.nil?
来源：http://qhp.redwolf501.top

C#:   if (data == null) return;
来源：http://omu.shanyushiyangkeji.top

================================================================================
来源：http://jsg.shanyushiyangkeji.top

C. 函数与作用域
来源：http://rsb.fengsongda.top

================================================================================
来源：http://cym.zdbjq.cn

[C01] 定义函数
来源：http://tht.ywan-chungtsiang.top

Py:   def add(a, b): return a + b
来源：http://avv.jinghuilouyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sxs.quarkkingdee.top

JS:   function add(a, b) { return a + b; }
来源：http://ewb.hywenlv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xmz.hfpthk.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://rtf.bbcook.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hhf.zhiwuduotai.top

Ruby: def add(a, b); a + b; end
来源：http://kfh.jinghuilouyu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vzx.hywenlv.cn

[C02] 默认参数
来源：http://moq.yongpay.top

Py:   def greet(name="World"): return name
来源：http://ool.xuetiantiany.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://odv.ivvv.top

JS:   function greet(name = "World") { return name; }
来源：http://nso.ivvv.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ari.cdnleiting.top

Java: // 无默认参数：方法重载或 Optional
来源：http://zkj.zdbjq.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://res.yangfankeji.com

Ruby: def greet(name = "World") = name
来源：http://xmy.zhoulong.xyz

C#:   string Greet(string name = "World") => name;
来源：http://qer.xinyue.icu

[C03] 可变参数
来源：http://vce.quarkkingdee.top

Py:   def total(*args): return sum(args)
来源：http://ddz.vehdjk.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ouv.zhiwuduotai.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rdb.jqgufenzy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nof.xuanzx.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dnt.dianchejie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://itk.andypj.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://yjo.zhaomingkeji.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mkg.ehwqpu.com

[C04] 命名参数 / 关键字参数
来源：http://vrg.sweek.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hen.shanyushiyangkeji.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bmx.birdmap.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tdl.wangdashe.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gad.hongshengwenyu.top

Java: // 无：用 Builder 模式或 record
来源：http://awr.zhongyouzk.top

Go:   // 无：用配置结构体参数
来源：http://tqc.jqgfzy.top

Ruby: f(a: 1, b: 2)
来源：http://bjd.cucudq.cn

C#:   f(a: 1, b: 2)
来源：http://ome.xuanzx.com

[C05] 返回多个值
来源：http://sva.gzhubu.top

Py:   return a, b
来源：http://iov.cheryme.top

PHP:  return [$a, $b];
来源：http://vyk.jyoumei.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://can.sysykeji.top

TS:   return { a, b };
来源：http://hbo.sxryk.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rhg.pengpengdd.cyou

Go:   return a, b
来源：http://gfy.yj202588.top

Ruby: return a, b
来源：http://bur.52xcode.cn

C#:   return (a, b);              // ValueTuple
来源：http://khf.smart0.xyz

[C06] 匿名函数 / lambda
来源：http://jxf.guannengcc.top

Py:   square = lambda x: x * x
来源：http://mxo.c1oappe.top

PHP:  $square = fn($x) => $x * $x;
来源：http://qgp.yuxming.cn

JS:   const square = x => x * x;
来源：http://twu.xziqi.cn

TS:   const square = (x: number): number => x * x;
来源：http://fow.tianlin.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://btz.xuanzx.com

Go:   sq := func(x int) int { return x * x }
来源：http://ugt.fehbvm.com

Ruby: square = ->(x) { x * x }
来源：http://tex.nanxinkj.top

C#:   Func<int, int> square = x => x * x;
来源：http://thq.zhijiandao.cn

[C07] 把函数作为参数传入
来源：http://hze.feifeiyinyue.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://elt.hnqzz.top

PHP:  array_map("strtoupper", $arr);
来源：http://kjl.smart0.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xnv.jyoumei.cn

TS:   arr.map(String)
来源：http://pyi.dashuyun.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qqt.fktsv.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tkj.shanyushiyangtech.top

Ruby: arr.map(&:upcase)
来源：http://yaj.smart0.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://jqk.smart0.xyz

[C08] 闭包
来源：http://pcf.pengpengdd.cyou

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cou.guowangkeji.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hpf.cucudq.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rst.nanxinkj.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bam.fengsongda.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zpa.316326.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fjm.jqgufenzy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bzz.chenjidiqi.icu

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zyq.pengpengdd.cyou

[C09] 递归
来源：http://wup.jinqigfzy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lna.wangdashe.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uiv.mhx1999.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tlw.meibo888.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hqf.tanke756.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://clz.fktsv.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fsp.cucudq.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kcf.xuanzx.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mkg.birdmap.top

[C10] 变量作用域
来源：http://eiz.cqqwz.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qwi.cashguo.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ucp.ctjpmb.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tbt.meibo888.top

TS:   同 JS
来源：http://loy.chenjidiqi.icu

Java: 方法内为块级作用域
来源：http://mmt.zhoulong.xyz

Go:   花括号块级作用域
来源：http://zuf.jqgufenzy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ras.uphjek.com

C#:   块级作用域
来源：http://roc.0kj1m.cn

[C11] 模块导入与导出
来源：http://drc.jianghu66.top

Py:   from module import func
来源：http://qto.chenlongwang.top

PHP:  require "file.php";  或 use App\Service;
来源：http://bsj.wangdashe.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://wtu.jinghuilouyu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vmj.zhiwuduotai.top

Java: import java.util.List;
来源：http://rbb.haohaochexian.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://haa.tian-w.cn

Ruby: require "json"; require_relative "./util"
来源：http://ria.jyoumei.cn

C#:   using System.Text;
来源：http://cta.haohaochexian.top

[C12] 立即执行函数 IIFE
来源：http://qwb.zhongyouzk.top

Py:   (lambda: print("run"))()
来源：http://bwq.cucudq.cn

PHP:  (function () { echo "run"; })();
来源：http://hvm.havefunace.top

JS:   (() => { console.log("run"); })();
来源：http://bdk.iojbl.cn

TS:   (() => { console.log("run"); })();
来源：http://zww.9152youxi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://epm.quarkkingdee.top

Go:   func() { fmt.Println("run") }()
来源：http://vpm.bjfxy.top

Ruby: -> { puts "run" }.call
来源：http://umx.cashguo.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ibf.yanxiufei.cn

[C13] 类型声明 / 类型注解
来源：http://btv.xuanzx.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mlc.cdnleiting.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://thi.guannengcc.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rya.andypj.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rnw.yanxiufei.cn

Java: int add(int a, int b) { return a + b; }
来源：http://rxo.svipenyu.cn

Go:   func add(a, b int) int
来源：http://irx.smart0.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gok.guowangkeji.top

C#:   int Add(int a, int b) => a + b;
来源：http://yje.jinqigfzy.top

[C14] 泛型函数
来源：http://unu.shangyingyoupin.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uxd.shzxlz.cn

PHP:  // 无泛型
来源：http://tzz.guannengcc.top

JS:   // 无泛型
来源：http://rzr.smart0.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hgy.hywenlv.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uyk.yanxiufei.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lpc.xingfuxueyuan.xyz

Ruby: # 无泛型
来源：http://lma.yongpay.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tdf.vehdjk.com

[C15] 解构 / 展开参数
来源：http://tht.yanxiufei.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sek.chenzaomai.com

PHP:  [$a, $b] = $pair;
来源：http://oud.pycfn.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jpo.hesvh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ggt.tian-w.cn

Java: // 无解构
来源：http://kes.9152youxi.cn

Go:   // 无解构
来源：http://jwq.xuanzx.com

Ruby: a, b = pair
来源：http://fff.fengsongda.top

C#:   var (a, b) = pair;
来源：http://gts.snrcjt.cn

[C16] 函数 / 方法重载
来源：http://rfk.daria6918.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yah.dianchejie.cn

PHP:  // 无重载
来源：http://mzi.hcnkem.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://zrm.hywenlv.cn

TS:   // 用联合类型或重载签名声明
来源：http://gox.kuanghao11.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://pzt.gotoacloud.top

Go:   // 无重载：用不同函数名
来源：http://jlj.yueranfly.top

Ruby: # 无重载：靠动态参数
来源：http://xfe.zhengqikj.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ltn.tarul.cn

================================================================================
来源：http://ngn.jinghuilouyu.cn

D. 数组 / 列表 / 集合
来源：http://vml.zhaomingkeji.xyz

================================================================================
来源：http://mvt.iojbl.cn

[D01] 创建数组 / 列表
来源：http://ugv.shanyushiyangtech.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://col.jyoumei.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hmo.smart0.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nje.hfpthk.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://vmt.sysykeji.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kbe.0kj1m.cn

Go:   arr := []int{1, 2, 3}
来源：http://nuy.guannengcc.top

Ruby: arr = [1, 2, 3]
来源：http://mmu.xinyue.icu

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qqm.hongshengwenyu.top

[D02] 追加元素到末尾
来源：http://nia.jinqigufen.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://csr.gogol.net.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hsy.shanyushiyangtech.top

JS:   arr.push(4);
来源：http://aay.yj202588.top

TS:   arr.push(4);
来源：http://jdn.fengsongda.top

Java: list.add(4);
来源：http://cns.yongpay.top

Go:   arr = append(arr, 4)
来源：http://amu.hcnkem.com

Ruby: arr << 4; arr.push(5)
来源：http://pzl.guowangkeji.top

C#:   list.Add(4);
来源：http://whm.jyoumei.cn

[D03] 在指定位置插入元素
来源：http://uay.jinyuanbaomall.cn

Py:   arr.insert(0, 0)
来源：http://cew.xylfe.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qnz.9152youxi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nnz.haohaochexian.top

TS:   arr.splice(0, 0, 0);
来源：http://axb.jqgfzy.top

Java: list.add(0, 0);
来源：http://ikx.yuxming.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vzs.fzhhl.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vdo.aizwys.cn

C#:   list.Insert(0, 0);
来源：http://bvq.xingfuxueyuan.xyz

[D04] 删除元素
来源：http://grl.yueranfly.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vvg.jiagoushi.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ohw.pengpengdd.cyou

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sgu.zhaomingkeji.xyz

TS:   arr.splice(0, 1);
来源：http://kwk.iojbl.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jnn.316326.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://azr.jinghuilouyu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fgi.hesvh.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qze.c1oappe.top

[D05] 访问与修改元素
来源：http://iii.ctjpmb.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://raw.dianchejie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://elg.chenzaomai.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lpw.aibaodan.cn

TS:   arr[0]; arr.at(-1);
来源：http://wgg.zhixingplan.top

Java: list.get(0); list.set(0, 9);
来源：http://eny.kuanghao11.cn

Go:   arr[0]; arr[0] = 9
来源：http://wjm.havefunace.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pfp.gzhubu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jak.kuanghao11.cn

[D06] 数组长度
来源：http://zke.fanxiaobao.xyz

Py:   len(arr)
来源：http://mms.jinqigufen.top

PHP:  count($arr);
来源：http://fxb.yj20258888.top

JS:   arr.length
来源：http://azv.hysaishi.cn

TS:   arr.length
来源：http://mbg.shanyushiyangkeji.top

Java: list.size();
来源：http://khq.vehdjk.com

Go:   len(arr)
来源：http://wij.zhengqikj.top

Ruby: arr.length; arr.size
来源：http://dyg.ybcxt.top

C#:   list.Count;
来源：http://wwo.tianlin.xyz

[D07] 切片 / 取子数组
来源：http://cji.jiagoushi.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rxe.haohaochexian.top

PHP:  array_slice($arr, 1, 3);
来源：http://oaa.vehdjk.com

JS:   arr.slice(1, 4);
来源：http://vfy.zhaomingkeji.xyz

TS:   arr.slice(1, 4);
来源：http://cvg.vqdsnc.cn

Java: list.subList(1, 4);
来源：http://bcm.jiagoushi.top

Go:   arr[1:4]
来源：http://qrc.zhijiandao.cn

Ruby: arr[1, 3]
来源：http://wfh.yueranfly.top

C#:   list.GetRange(1, 3);
来源：http://rce.aibaodan.cn

[D08] 合并两个数组
来源：http://vlj.jlsjyb.cn

Py:   a + b;  a.extend(b)
来源：http://vbg.vqdsnc.cn

PHP:  array_merge($a, $b);
来源：http://dug.snrcjt.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://znf.jianghu66.top

TS:   [...a, ...b];
来源：http://nkl.wangdashe.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rha.yongpay.top

Go:   append(a, b...)
来源：http://tyn.c1oappe.top

Ruby: a + b;  a.concat(b)
来源：http://igk.shanyushiyangkeji.top

C#:   a.Concat(b).ToList()
来源：http://lnm.gotoacloud.top

[D09] 排序（升序）
来源：http://qop.cdnleiting.top

Py:   sorted(arr);  arr.sort()
来源：http://ktl.hywenlv.cn

PHP:  sort($arr);
来源：http://fhv.redwolf501.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://efk.guannengcc.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://jfq.yongpay.top

Java: Collections.sort(list);  list.sort(null);
来源：http://fhi.kuanghao11.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uog.zhoulong.xyz

Ruby: arr.sort
来源：http://ays.9152youxi.cn

C#:   list.Sort();
来源：http://dgv.fktsv.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://yto.zhijiandao.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tqa.daxiang520.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xlb.shzxlz.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kys.bbcook.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yif.yj202588.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://air.hesvh.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yth.zhengqikj.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fis.snrcjt.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ulc.hnqzz.top

[D11] 反转数组
来源：http://kov.hcnkem.com

Py:   arr[::-1];  arr.reverse()
来源：http://lkp.yongpay.top

PHP:  array_reverse($arr);
来源：http://kda.gogol.net.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kif.dashuyun.cn

TS:   [...arr].reverse();
来源：http://rlb.yvedp.cn

Java: Collections.reverse(list);
来源：http://cje.zhengqikj.top

Go:   slices.Reverse(arr)
来源：http://ecr.fengsongda.top

Ruby: arr.reverse
来源：http://osv.jinyuanbaomall.cn

C#:   list.Reverse();
来源：http://oml.xuetiantiany.cn

[D12] 查找元素下标
来源：http://olg.ydzc1.top

Py:   arr.index(x);  x in arr
来源：http://hda.sweek.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fmv.jinqigfzy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fbg.jinqigufen.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lvg.yongpay.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hul.pycfn.com

Go:   slices.Index(arr, x)
来源：http://uxd.xingfuxueyuan.xyz

Ruby: arr.index(x)
来源：http://abi.vqdsnc.cn

C#:   list.IndexOf(x);
来源：http://axp.jqgfzy.top

[D13] 过滤（保留满足条件的）
来源：http://cjc.vqdsnc.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ggq.haohaochexian.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wbp.nwbrower.top

JS:   arr.filter(x => x > 3)
来源：http://ilt.shuidangran.top

TS:   arr.filter(x => x > 3)
来源：http://qkk.316326.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xkl.hesvh.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wsv.yj20258.top

Ruby: arr.select { |x| x > 3 }
来源：http://jwg.shuidangran.top

C#:   list.Where(x => x > 3).ToList()
来源：http://gwf.yanxiufei.cn

[D14] 映射转换（每个元素变形）
来源：http://jmw.aibaodan.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://edl.shzxlz.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://eqg.ybcxt.top

JS:   arr.map(x => x * 2)
来源：http://dlj.yangfankeji.com

TS:   arr.map(x => x * 2)
来源：http://uxe.yongpay.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://cwe.fengsongda.top

Go:   // 手写循环
来源：http://ekz.yfazqb.com

Ruby: arr.map { |x| x * 2 }
来源：http://lcm.yanxiufei.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://wil.zhongyouzk.top

[D15] 去重
来源：http://kbg.uphjek.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lpa.yj20258.top

PHP:  array_unique($arr);
来源：http://nkx.sxryk.cn

JS:   [...new Set(arr)]
来源：http://uae.zhoulong.xyz


<!-- 参考信息 -->