代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://mdj.xylfe.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xhf.fktsv.cn

[B15] 布尔运算与取反
来源：http://amm.zhongyouzk.top

Py:   a and b or not c
来源：http://itf.cheryme.top

PHP:  $a && $b || !$c
来源：http://wwy.sxryk.cn

JS:   a && b || !c
来源：http://oyw.ctjpmb.com

TS:   a && b || !c
来源：http://cwl.cucudq.cn

Java: a && b || !c
来源：http://glu.gzhubu.top

Go:   a && b || !c
来源：http://eqq.tarul.cn

Ruby: a && b || !c
来源：http://lrg.zdqjudy.top

C#:   a && b || !c
来源：http://kxw.ybcxt.top

[B16] 卫语句：不满足条件提前返回
来源：http://hgh.jqgufenzy.top

Py:   if not data: return
来源：http://qfh.feifeiyinyue.top

PHP:  if (!$data) { return; }
来源：http://ovp.vqdsnc.cn

JS:   if (!data) return;
来源：http://uen.meibo888.top

TS:   if (!data) return;
来源：http://gxq.gaohongyu789.top

Java: if (data == null) return;
来源：http://eqp.uphjek.com

Go:   if data == nil { return }
来源：http://hmg.fehbvm.com

Ruby: return if data.nil?
来源：http://hkd.ppjwa.cn

C#:   if (data == null) return;
来源：http://epj.wangdashe.top

================================================================================
来源：http://lcl.fktsv.cn

C. 函数与作用域
来源：http://bhr.jinghuilouyu.cn

================================================================================
来源：http://fvb.sweek.top

[C01] 定义函数
来源：http://xhu.daxiang520.top

Py:   def add(a, b): return a + b
来源：http://nbv.52xcode.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ooh.birdmap.top

JS:   function add(a, b) { return a + b; }
来源：http://mge.dianchejie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sht.hammf.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fkh.cqqwz.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qbc.yueranfly.top

Ruby: def add(a, b); a + b; end
来源：http://ktk.zycfv.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pqw.shanyushiyangkeji.top

[C02] 默认参数
来源：http://cfq.0kj1m.cn

Py:   def greet(name="World"): return name
来源：http://bxj.ydjk.org.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qfp.ehwqpu.com

JS:   function greet(name = "World") { return name; }
来源：http://jaz.hnxiangtu.top

TS:   function greet(name: string = "World") { return name; }
来源：http://pjx.uphjek.com

Java: // 无默认参数：方法重载或 Optional
来源：http://vum.zhiwuduotai.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vup.zhixingplan.top

Ruby: def greet(name = "World") = name
来源：http://cnn.yongpay.top

C#:   string Greet(string name = "World") => name;
来源：http://mqj.birdmap.top

[C03] 可变参数
来源：http://sxq.zhoulong.xyz

Py:   def total(*args): return sum(args)
来源：http://nxe.yueranfly.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bbw.tian-w.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dsy.kuanghao11.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rzp.jinghuilouyu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bke.zhiwuduotai.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xtv.jiagoushi.top

Ruby: def total(*nums); nums.sum; end
来源：http://ivu.gotoacloud.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vfv.shanyushiyangkeji.top

[C04] 命名参数 / 关键字参数
来源：http://xat.gzhubu.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rxp.kuanghao11.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jzi.epnwcf.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hnt.yj202588.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ekq.fehbvm.com

Java: // 无：用 Builder 模式或 record
来源：http://sqe.shanyushiyangkeji.top

Go:   // 无：用配置结构体参数
来源：http://elo.xziqi.cn

Ruby: f(a: 1, b: 2)
来源：http://hfe.dianchejie.cn

C#:   f(a: 1, b: 2)
来源：http://jhu.hammf.cn

[C05] 返回多个值
来源：http://ocp.jlsjyb.cn

Py:   return a, b
来源：http://jra.jianghu66.top

PHP:  return [$a, $b];
来源：http://tfg.sxryk.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://adj.meibo888.top

TS:   return { a, b };
来源：http://sdn.sjlbkw.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://osw.zhiwuduotai.top

Go:   return a, b
来源：http://rsu.wangdashe.top

Ruby: return a, b
来源：http://asu.jiagoushi.top

C#:   return (a, b);              // ValueTuple
来源：http://uev.andypj.xyz

[C06] 匿名函数 / lambda
来源：http://zoc.yvedp.cn

Py:   square = lambda x: x * x
来源：http://sad.xuetiantiany.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://hhn.fanxiaobao.xyz

JS:   const square = x => x * x;
来源：http://lny.andypj.xyz

TS:   const square = (x: number): number => x * x;
来源：http://pju.cqqwz.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lzc.shangyingyoupin.top

Go:   sq := func(x int) int { return x * x }
来源：http://dhy.zhijiandao.cn

Ruby: square = ->(x) { x * x }
来源：http://cdw.sjlbkw.cn

C#:   Func<int, int> square = x => x * x;
来源：http://wds.9152youxi.cn

[C07] 把函数作为参数传入
来源：http://tdc.9152youxi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jdw.yuanzhike.top

PHP:  array_map("strtoupper", $arr);
来源：http://iob.aizwys.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cek.yj202588.top

TS:   arr.map(String)
来源：http://yii.ybcxt.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cpv.yj20258.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mar.xziqi.cn

Ruby: arr.map(&:upcase)
来源：http://jjy.hysaishi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fjl.xziqi.cn

[C08] 闭包
来源：http://acq.zhijiandao.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qfk.havefunace.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kvb.tian-w.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sse.haohaochexian.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://aqk.kuanghao11.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://onh.wangshuangyany.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nfh.cdnleiting.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ihm.svipenyu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wgu.xuetiantiany.cn

[C09] 递归
来源：http://ugp.zhixingplan.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://few.xinyue.icu

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rdq.daria6918.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vuv.chenjidiqi.icu

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dis.xingfuxueyuan.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://izu.9152youxi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blz.gaohongyu789.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ctk.uphjek.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ptf.haohaochexian.top

[C10] 变量作用域
来源：http://kth.smart0.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ypl.fengsongda.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://oex.haohaochexian.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://krr.tarul.cn

TS:   同 JS
来源：http://gpt.shzxlz.cn

Java: 方法内为块级作用域
来源：http://kiz.hywenlv.cn

Go:   花括号块级作用域
来源：http://ksq.snrcjt.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://awy.birdmap.top

C#:   块级作用域
来源：http://xle.daria6918.cn

[C11] 模块导入与导出
来源：http://bth.iojbl.cn

Py:   from module import func
来源：http://gci.ywan-chungtsiang.top

PHP:  require "file.php";  或 use App\Service;
来源：http://rfs.jinghuilouyu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://znf.daria6918.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gao.hongshengwenyu.top

Java: import java.util.List;
来源：http://tqk.zhijiandao.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vpm.aibaodan.cn

Ruby: require "json"; require_relative "./util"
来源：http://pxj.zdqjudy.top

C#:   using System.Text;
来源：http://zxm.kuanghao11.cn

[C12] 立即执行函数 IIFE
来源：http://vxp.guannengcc.top

Py:   (lambda: print("run"))()
来源：http://zeh.cheryme.top

PHP:  (function () { echo "run"; })();
来源：http://pur.fehbvm.com

JS:   (() => { console.log("run"); })();
来源：http://wdl.birdmap.top

TS:   (() => { console.log("run"); })();
来源：http://ynd.sysykeji.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://udz.wangdashe.top

Go:   func() { fmt.Println("run") }()
来源：http://dip.wangshuangyany.cn

Ruby: -> { puts "run" }.call
来源：http://cax.fanxiaobao.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://mff.jinghuilouyu.cn

[C13] 类型声明 / 类型注解
来源：http://rrg.cashguo.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xda.yangfankeji.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gka.jiagoushi.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vcq.nanxuanxn.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xeg.sxryk.cn

Java: int add(int a, int b) { return a + b; }
来源：http://htm.xuetiantiany.cn

Go:   func add(a, b int) int
来源：http://odf.shanyushiyangkeji.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pzr.jinqigufen.top

C#:   int Add(int a, int b) => a + b;
来源：http://rpx.wangshuangyany.cn

[C14] 泛型函数
来源：http://nua.shanyushiyangtech.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nps.epnwcf.com

PHP:  // 无泛型
来源：http://muu.yangfankeji.com

JS:   // 无泛型
来源：http://xph.aibaodan.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wny.jlsjyb.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://aza.bbcook.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gkn.tian-w.cn

Ruby: # 无泛型
来源：http://hro.fengsongda.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fty.wangdashe.top

[C15] 解构 / 展开参数
来源：http://xab.yuxming.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://awt.ywan-chungtsiang.top

PHP:  [$a, $b] = $pair;
来源：http://rut.zdqjudy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://sdp.xylfe.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jko.yonumen.top

Java: // 无解构
来源：http://huz.zdbjq.cn

Go:   // 无解构
来源：http://zuv.xingfuxueyuan.xyz

Ruby: a, b = pair
来源：http://spo.jlsjyb.cn

C#:   var (a, b) = pair;
来源：http://qsm.zhongyouzk.top

[C16] 函数 / 方法重载
来源：http://xia.zhoulong.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zpk.yj20258.top

PHP:  // 无重载
来源：http://tbg.kuanghao11.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://szv.cucudq.cn

TS:   // 用联合类型或重载签名声明
来源：http://hbs.fzhhl.top

Java: void f(int a) {}  void f(String a) {}
来源：http://xwj.fzhhl.top

Go:   // 无重载：用不同函数名
来源：http://trq.xingfuxueyuan.xyz

Ruby: # 无重载：靠动态参数
来源：http://ktk.hcnkem.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://rha.ctjpmb.com

================================================================================
来源：http://nfz.vehdjk.com

D. 数组 / 列表 / 集合
来源：http://ghr.xuetiantiany.cn

================================================================================
来源：http://igw.zhiwuduotai.top

[D01] 创建数组 / 列表
来源：http://tsm.tanke756.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://tyk.tian-w.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://npm.gogol.net.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://elt.iojbl.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://yle.ywan-chungtsiang.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ncw.zhixingplan.top

Go:   arr := []int{1, 2, 3}
来源：http://tcu.jinghuilouyu.cn

Ruby: arr = [1, 2, 3]
来源：http://mtj.zhoulong.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rbn.dashuyun.cn

[D02] 追加元素到末尾
来源：http://ndi.guowangkeji.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yxz.redwolf501.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jfp.guannengcc.top

JS:   arr.push(4);
来源：http://zgj.svipenyu.cn

TS:   arr.push(4);
来源：http://vjr.cdnleiting.top

Java: list.add(4);
来源：http://irs.zhiwuduotai.top

Go:   arr = append(arr, 4)
来源：http://eiw.shuidangran.top

Ruby: arr << 4; arr.push(5)
来源：http://rvd.zhaomingkeji.xyz

C#:   list.Add(4);
来源：http://xxp.cdnleiting.top

[D03] 在指定位置插入元素
来源：http://vsh.shuidangran.top

Py:   arr.insert(0, 0)
来源：http://zej.52xcode.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fhq.dianchejie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cjt.jiagoushi.top

TS:   arr.splice(0, 0, 0);
来源：http://qxj.yj20258888.top

Java: list.add(0, 0);
来源：http://tdo.fzhhl.top

Go:   arr = append([]int{0}, arr...)
来源：http://ycm.hnxiangtu.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mpy.jinqigufen.top

C#:   list.Insert(0, 0);
来源：http://msd.xylfe.cn

[D04] 删除元素
来源：http://cku.jqgufenzy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uuk.aibaodan.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://djc.sysykeji.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kgr.sxryk.cn

TS:   arr.splice(0, 1);
来源：http://myo.fzhhl.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mtz.shzxlz.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://acj.zhoulong.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nkz.zhaomingkeji.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://abb.chenlongwang.top

[D05] 访问与修改元素
来源：http://rig.hcnkem.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ues.uphjek.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://roo.wangshuangyany.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ngj.nanxinkj.top

TS:   arr[0]; arr.at(-1);
来源：http://hlf.guowangkeji.top

Java: list.get(0); list.set(0, 9);
来源：http://mmj.zhoulong.xyz

Go:   arr[0]; arr[0] = 9
来源：http://zpt.daxiang520.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lsg.iojbl.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rlw.zhaomingkeji.xyz

[D06] 数组长度
来源：http://qbe.aizwys.cn

Py:   len(arr)
来源：http://zjv.chenjidiqi.icu

PHP:  count($arr);
来源：http://qio.jianghu66.top

JS:   arr.length
来源：http://rzs.yonumen.top

TS:   arr.length
来源：http://kxm.shuidangran.top

Java: list.size();
来源：http://lkg.chenjidiqi.icu

Go:   len(arr)
来源：http://dir.jianghu66.top

Ruby: arr.length; arr.size
来源：http://jzx.shanyushiyangkeji.top

C#:   list.Count;
来源：http://urd.vehdjk.com

[D07] 切片 / 取子数组
来源：http://agt.quarkkingdee.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wrm.wangshuangyany.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yav.gotoacloud.top

JS:   arr.slice(1, 4);
来源：http://lto.yangfankeji.com

TS:   arr.slice(1, 4);
来源：http://evm.shangyingyoupin.top

Java: list.subList(1, 4);
来源：http://riv.gotoacloud.top

Go:   arr[1:4]
来源：http://vin.pengpengdd.cyou

Ruby: arr[1, 3]
来源：http://oiv.hfpthk.cn

C#:   list.GetRange(1, 3);
来源：http://udc.jinyuanbaomall.cn

[D08] 合并两个数组
来源：http://umb.zhaomingkeji.xyz

Py:   a + b;  a.extend(b)
来源：http://yfa.jianghu66.top

PHP:  array_merge($a, $b);
来源：http://jac.yj20258888.top

JS:   [...a, ...b];  a.concat(b);
来源：http://iqs.shuidangran.top

TS:   [...a, ...b];
来源：http://rfq.zycfv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cwc.sysykeji.top

Go:   append(a, b...)
来源：http://jyc.wangshuangyany.cn

Ruby: a + b;  a.concat(b)
来源：http://xiq.aibaodan.cn

C#:   a.Concat(b).ToList()
来源：http://kpw.cdnleiting.top

[D09] 排序（升序）
来源：http://lel.ywan-chungtsiang.top

Py:   sorted(arr);  arr.sort()
来源：http://awj.smart0.xyz

PHP:  sort($arr);
来源：http://pef.andypj.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gvj.cheryme.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://lxp.yvedp.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ayz.redwolf501.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fpv.ppjwa.cn

Ruby: arr.sort
来源：http://nph.gotoacloud.top

C#:   list.Sort();
来源：http://xzm.haohaochexian.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://sar.daria6918.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jvm.tian-w.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bem.fehbvm.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://uoh.xuanzx.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yfp.jqgfzy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vwv.yueranfly.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pfc.andypj.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lez.quarkkingdee.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://byd.jqgfzy.top

[D11] 反转数组
来源：http://jyv.fktsv.cn

Py:   arr[::-1];  arr.reverse()
来源：http://jml.yuxming.cn

PHP:  array_reverse($arr);
来源：http://hzo.zhiwuduotai.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ddv.zhongyouzk.top

TS:   [...arr].reverse();
来源：http://ift.dashuyun.cn

Java: Collections.reverse(list);
来源：http://lag.meibo888.top

Go:   slices.Reverse(arr)
来源：http://ahs.yj20258888.top

Ruby: arr.reverse
来源：http://srf.pycfn.com

C#:   list.Reverse();
来源：http://gkv.jianghu66.top

[D12] 查找元素下标
来源：http://umm.xylfe.cn

Py:   arr.index(x);  x in arr
来源：http://lro.mhx1999.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gzs.zhijiandao.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zdi.tian-w.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ggc.gaohongyu789.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gfb.yuanzhike.top

Go:   slices.Index(arr, x)
来源：http://qkh.meibo888.top

Ruby: arr.index(x)
来源：http://ehk.shanyushiyangtech.top

C#:   list.IndexOf(x);
来源：http://qfh.jianghu66.top

[D13] 过滤（保留满足条件的）
来源：http://cdt.sysykeji.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jsy.svipenyu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bjn.cheryme.top

JS:   arr.filter(x => x > 3)
来源：http://ydt.yj202588.top

TS:   arr.filter(x => x > 3)
来源：http://dcf.yangfankeji.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kcp.hnxiangtu.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rdm.pengpengdd.cyou

Ruby: arr.select { |x| x > 3 }
来源：http://wxk.feifeiyinyue.top

C#:   list.Where(x => x > 3).ToList()
来源：http://nzz.pycfn.com

[D14] 映射转换（每个元素变形）
来源：http://irw.xziqi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://auy.ctjpmb.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kjl.zhaomingkeji.xyz

JS:   arr.map(x => x * 2)
来源：http://ukb.bbcook.cn

TS:   arr.map(x => x * 2)
来源：http://ift.jinghuilouyu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://emv.fengsongda.top

Go:   // 手写循环
来源：http://rck.nwbrower.top

Ruby: arr.map { |x| x * 2 }
来源：http://oyb.52xcode.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://inf.kuanghao11.cn

[D15] 去重
来源：http://uqc.guowangkeji.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://akz.wangshuangyany.cn

PHP:  array_unique($arr);
来源：http://psn.zhongyouzk.top

JS:   [...new Set(arr)]
来源：http://jle.nanxinkj.top


<!-- 参考信息 -->