代发 wailian999

[B13] 判断是否为数字
来源：http://zfx.hnqzz.top

Py:   isinstance(x, (int, float))
来源：http://wsm.sufxvd.cn

PHP:  is_numeric($x)
来源：http://nsb.yuxming.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gzf.cqqwz.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zgj.gogol.net.cn

Java: x instanceof Number
来源：http://xxk.zycfv.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://utv.yuanzhike.top

Ruby: x.is_a?(Numeric)
来源：http://uyg.ctjpmb.com

C#:   x is int or double or decimal
来源：http://tkz.yvedp.cn

[B14] 判断值是否在集合内
来源：http://tnt.cdnleiting.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uhy.tanke756.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mtt.hnxiangtu.top

JS:   [1, 2, 3].includes(x)
来源：http://qey.cdnleiting.top

TS:   [1, 2, 3].includes(x)
来源：http://nky.zhixingplan.top

Java: List.of(1, 2, 3).contains(x)
来源：http://bgi.chenzaomai.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zsa.xuanzx.com

Ruby: [1, 2, 3].include?(x)
来源：http://hcu.yj20258.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kxb.ydjk.org.cn

[B15] 布尔运算与取反
来源：http://flu.yj202588.top

Py:   a and b or not c
来源：http://xuc.ydzc1.top

PHP:  $a && $b || !$c
来源：http://eti.jlsjyb.cn

JS:   a && b || !c
来源：http://aqg.jqgfzy.top

TS:   a && b || !c
来源：http://ntd.shanyushiyangkeji.top

Java: a && b || !c
来源：http://kiy.hnxiangtu.top

Go:   a && b || !c
来源：http://kvi.zhixingplan.top

Ruby: a && b || !c
来源：http://htq.guowangkeji.top

C#:   a && b || !c
来源：http://zoh.xuanzx.com

[B16] 卫语句：不满足条件提前返回
来源：http://vhv.jiagoushi.top

Py:   if not data: return
来源：http://scr.jinyuanbaomall.cn

PHP:  if (!$data) { return; }
来源：http://bfl.gaohongyu789.top

JS:   if (!data) return;
来源：http://ovw.jinghuilouyu.cn

TS:   if (!data) return;
来源：http://eth.hfpthk.cn

Java: if (data == null) return;
来源：http://bkz.ywan-chungtsiang.top

Go:   if data == nil { return }
来源：http://igd.fehbvm.com

Ruby: return if data.nil?
来源：http://zea.ydjk.org.cn

C#:   if (data == null) return;
来源：http://lqo.wangdashe.top

================================================================================
来源：http://lck.kuanghao11.cn

C. 函数与作用域
来源：http://qnn.shangyingyoupin.top

================================================================================
来源：http://cne.fengsongda.top

[C01] 定义函数
来源：http://ovx.xinyue.icu

Py:   def add(a, b): return a + b
来源：http://mus.fehbvm.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tuu.nanxuanxn.top

JS:   function add(a, b) { return a + b; }
来源：http://vjm.ehwqpu.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cmd.shangyingyoupin.top

Java: static int add(int a, int b) { return a + b; }
来源：http://unk.gogol.net.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qjq.sufxvd.cn

Ruby: def add(a, b); a + b; end
来源：http://eyb.tarul.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pov.haohaochexian.top

[C02] 默认参数
来源：http://hnc.sjlbkw.cn

Py:   def greet(name="World"): return name
来源：http://xqj.cdnleiting.top

PHP:  function greet($name = "World") { return $name; }
来源：http://lso.zhaomingkeji.xyz

JS:   function greet(name = "World") { return name; }
来源：http://mmk.yueranfly.top

TS:   function greet(name: string = "World") { return name; }
来源：http://fjy.zhongyouzk.top

Java: // 无默认参数：方法重载或 Optional
来源：http://zpi.cashguo.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://llv.tian-w.cn

Ruby: def greet(name = "World") = name
来源：http://xzn.zhixingplan.top

C#:   string Greet(string name = "World") => name;
来源：http://ypx.jinqigfzy.top

[C03] 可变参数
来源：http://akj.cucudq.cn

Py:   def total(*args): return sum(args)
来源：http://uix.haohaochexian.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xqv.smart0.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://beg.ydjk.org.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ewp.bbcook.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://trv.jlsjyb.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lcq.gotoacloud.top

Ruby: def total(*nums); nums.sum; end
来源：http://qqy.zhaomingkeji.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rni.yuanzhike.top

[C04] 命名参数 / 关键字参数
来源：http://mut.sufxvd.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sya.yfazqb.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yra.zhaomingkeji.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qbi.yuxming.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://eiu.52xcode.cn

Java: // 无：用 Builder 模式或 record
来源：http://wta.hywenlv.cn

Go:   // 无：用配置结构体参数
来源：http://inu.cucudq.cn

Ruby: f(a: 1, b: 2)
来源：http://ptc.iojbl.cn

C#:   f(a: 1, b: 2)
来源：http://thb.zhengqikj.top

[C05] 返回多个值
来源：http://qyz.redwolf501.top

Py:   return a, b
来源：http://oyi.nanxuanxn.top

PHP:  return [$a, $b];
来源：http://smh.hnxiangtu.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://lys.hammf.cn

TS:   return { a, b };
来源：http://uvc.dashuyun.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mng.epnwcf.com

Go:   return a, b
来源：http://mcp.pycfn.com

Ruby: return a, b
来源：http://kdc.fehbvm.com

C#:   return (a, b);              // ValueTuple
来源：http://bmf.zhixingplan.top

[C06] 匿名函数 / lambda
来源：http://moj.jinyuanbaomall.cn

Py:   square = lambda x: x * x
来源：http://qwv.wangdashe.top

PHP:  $square = fn($x) => $x * $x;
来源：http://qwg.yonumen.top

JS:   const square = x => x * x;
来源：http://wgy.tanke756.top

TS:   const square = (x: number): number => x * x;
来源：http://tue.yj20258.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://psi.nanxuanxn.top

Go:   sq := func(x int) int { return x * x }
来源：http://jlv.tanke756.top

Ruby: square = ->(x) { x * x }
来源：http://yuw.hfpthk.cn

C#:   Func<int, int> square = x => x * x;
来源：http://riv.ydjk.org.cn

[C07] 把函数作为参数传入
来源：http://spr.haohaochexian.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hcb.cdnleiting.top

PHP:  array_map("strtoupper", $arr);
来源：http://gxj.ydzc1.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rzj.quarkkingdee.top

TS:   arr.map(String)
来源：http://ohx.jinghuilouyu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nmx.ehwqpu.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yiq.fehbvm.com

Ruby: arr.map(&:upcase)
来源：http://wqu.cashguo.top

C#:   arr.Select(s => s.ToUpper())
来源：http://efe.xingfuxueyuan.xyz

[C08] 闭包
来源：http://eny.zdbjq.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xpq.sweek.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cfs.pycfn.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fjw.feifeiyinyue.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tih.hysaishi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://whq.gzhubu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gno.cheryme.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vur.yj20258888.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ibm.jinqigfzy.top

[C09] 递归
来源：http://awc.jqgufenzy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://grm.jqgfzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://eax.zhoulong.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dkr.hnqzz.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iac.zhaomingkeji.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://myy.ppjwa.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bve.yvedp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wtx.dianchejie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cjc.chenlongwang.top

[C10] 变量作用域
来源：http://ubk.mhx1999.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://djo.jinghuilouyu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jbc.snrcjt.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rxa.dianchejie.cn

TS:   同 JS
来源：http://tlg.vqdsnc.cn

Java: 方法内为块级作用域
来源：http://xqr.wangshuangyany.cn

Go:   花括号块级作用域
来源：http://dus.cucudq.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yvt.jinqigufen.top

C#:   块级作用域
来源：http://rji.dashuyun.cn

[C11] 模块导入与导出
来源：http://vmv.vehdjk.com

Py:   from module import func
来源：http://lcd.mhx1999.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ulo.tian-w.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://cbp.quarkkingdee.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dmv.yongpay.top

Java: import java.util.List;
来源：http://kwu.0kj1m.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sex.jlsjyb.cn

Ruby: require "json"; require_relative "./util"
来源：http://rrm.9152youxi.cn

C#:   using System.Text;
来源：http://jxe.shanyushiyangtech.top

[C12] 立即执行函数 IIFE
来源：http://qcl.havefunace.top

Py:   (lambda: print("run"))()
来源：http://npg.xingfuxueyuan.xyz

PHP:  (function () { echo "run"; })();
来源：http://pcy.smart0.xyz

JS:   (() => { console.log("run"); })();
来源：http://wmu.yongpay.top

TS:   (() => { console.log("run"); })();
来源：http://ylm.yongpay.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xta.jlsjyb.cn

Go:   func() { fmt.Println("run") }()
来源：http://sjc.meibo888.top

Ruby: -> { puts "run" }.call
来源：http://aub.wangshuangyany.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xkx.jlsjyb.cn

[C13] 类型声明 / 类型注解
来源：http://fna.ppjwa.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zob.chenzaomai.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tdi.quarkkingdee.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://boj.aibaodan.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cki.jyoumei.cn

Java: int add(int a, int b) { return a + b; }
来源：http://gjs.yj20258888.top

Go:   func add(a, b int) int
来源：http://xxu.hywenlv.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tyn.nanxinkj.top

C#:   int Add(int a, int b) => a + b;
来源：http://ouh.gotoacloud.top

[C14] 泛型函数
来源：http://yjf.jinghuilouyu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gvl.epnwcf.com

PHP:  // 无泛型
来源：http://yxm.jinqigufen.top

JS:   // 无泛型
来源：http://ssf.hywenlv.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jmu.hfpthk.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bzj.jiagoushi.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vyn.shanyushiyangkeji.top

Ruby: # 无泛型
来源：http://yaz.zhixingplan.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cme.nwbrower.top

[C15] 解构 / 展开参数
来源：http://jvf.hywenlv.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vuj.quarkkingdee.top

PHP:  [$a, $b] = $pair;
来源：http://yfk.dashuyun.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mmh.aibaodan.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ydl.9152youxi.cn

Java: // 无解构
来源：http://gav.svipenyu.cn

Go:   // 无解构
来源：http://jfa.jinghuilouyu.cn

Ruby: a, b = pair
来源：http://mxv.xingfuxueyuan.xyz

C#:   var (a, b) = pair;
来源：http://fjp.daxiang520.top

[C16] 函数 / 方法重载
来源：http://glc.fanxiaobao.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mhq.hfpthk.cn

PHP:  // 无重载
来源：http://fwc.xylfe.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://vrd.hesvh.cn

TS:   // 用联合类型或重载签名声明
来源：http://cpv.tarul.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ito.zhijiandao.cn

Go:   // 无重载：用不同函数名
来源：http://yvk.shangyingyoupin.top

Ruby: # 无重载：靠动态参数
来源：http://znl.redwolf501.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ksb.bbcook.cn

================================================================================
来源：http://rel.yongpay.top

D. 数组 / 列表 / 集合
来源：http://hqn.tian-w.cn

================================================================================
来源：http://wti.hongshengwenyu.top

[D01] 创建数组 / 列表
来源：http://tri.iojbl.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ypi.yvedp.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://svy.uphjek.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qhl.zhaomingkeji.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://euy.yj202588.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yvy.tian-w.cn

Go:   arr := []int{1, 2, 3}
来源：http://cxd.smart0.xyz

Ruby: arr = [1, 2, 3]
来源：http://afm.jqgufenzy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jux.tarul.cn

[D02] 追加元素到末尾
来源：http://skl.bjfxy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://iwd.guannengcc.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nqr.jianghu66.top

JS:   arr.push(4);
来源：http://lqy.wangshuangyany.cn

TS:   arr.push(4);
来源：http://kdt.yongpay.top

Java: list.add(4);
来源：http://eiu.fengsongda.top

Go:   arr = append(arr, 4)
来源：http://sdo.tanke756.top

Ruby: arr << 4; arr.push(5)
来源：http://hme.zdqjudy.top

C#:   list.Add(4);
来源：http://hst.0kj1m.cn

[D03] 在指定位置插入元素
来源：http://xbr.havefunace.top

Py:   arr.insert(0, 0)
来源：http://mlp.cheryme.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uhi.yfazqb.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sjb.hfpthk.cn

TS:   arr.splice(0, 0, 0);
来源：http://qbv.fanxiaobao.xyz

Java: list.add(0, 0);
来源：http://poh.jinghuilouyu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://hzi.mhx1999.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gek.chenlongwang.top

C#:   list.Insert(0, 0);
来源：http://dpm.jinyuanbaomall.cn

[D04] 删除元素
来源：http://adi.ydzc1.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jyf.zhaomingkeji.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://awu.fktsv.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pkt.xuanzx.com

TS:   arr.splice(0, 1);
来源：http://mch.bbcook.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hyy.yvedp.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nsm.zhengqikj.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ymm.ehwqpu.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://btj.uphjek.com

[D05] 访问与修改元素
来源：http://hbb.cucudq.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://syx.fehbvm.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rhj.aibaodan.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vfa.tanke756.top

TS:   arr[0]; arr.at(-1);
来源：http://kzz.dashuyun.cn

Java: list.get(0); list.set(0, 9);
来源：http://gqi.meibo888.top

Go:   arr[0]; arr[0] = 9
来源：http://fwz.sufxvd.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://maz.zhoulong.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mvo.yueranfly.top

[D06] 数组长度
来源：http://duk.sysykeji.top

Py:   len(arr)
来源：http://ayl.jyoumei.cn

PHP:  count($arr);
来源：http://tnc.yueranfly.top

JS:   arr.length
来源：http://abu.chenjidiqi.icu

TS:   arr.length
来源：http://wsv.hcnkem.com

Java: list.size();
来源：http://bxm.zhixingplan.top

Go:   len(arr)
来源：http://xoe.shuidangran.top

Ruby: arr.length; arr.size
来源：http://rbz.gogol.net.cn

C#:   list.Count;
来源：http://sea.daria6918.cn

[D07] 切片 / 取子数组
来源：http://qvr.jiagoushi.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wko.vqdsnc.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jgi.ctjpmb.com

JS:   arr.slice(1, 4);
来源：http://hch.gaohongyu789.top

TS:   arr.slice(1, 4);
来源：http://eui.0kj1m.cn

Java: list.subList(1, 4);
来源：http://fqs.hnxiangtu.top

Go:   arr[1:4]
来源：http://ikq.jinqigufen.top

Ruby: arr[1, 3]
来源：http://mqb.jqgfzy.top

C#:   list.GetRange(1, 3);
来源：http://pnn.jqgufenzy.top

[D08] 合并两个数组
来源：http://yyk.iojbl.cn

Py:   a + b;  a.extend(b)
来源：http://znn.xuanzx.com

PHP:  array_merge($a, $b);
来源：http://ziy.sufxvd.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://aiy.ywan-chungtsiang.top

TS:   [...a, ...b];
来源：http://rak.jyoumei.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://aau.yuxming.cn

Go:   append(a, b...)
来源：http://dpd.feifeiyinyue.top

Ruby: a + b;  a.concat(b)
来源：http://xkt.fanxiaobao.xyz

C#:   a.Concat(b).ToList()
来源：http://erq.yj202588.top

[D09] 排序（升序）
来源：http://owi.shanyushiyangtech.top

Py:   sorted(arr);  arr.sort()
来源：http://rxo.epnwcf.com

PHP:  sort($arr);
来源：http://joo.nanxuanxn.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://oxy.jinghuilouyu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://rkz.xylfe.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vao.dianchejie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uql.jqgufenzy.top

Ruby: arr.sort
来源：http://lsi.wangdashe.top

C#:   list.Sort();
来源：http://yjl.zhaomingkeji.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://tqe.sjlbkw.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://edr.svipenyu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pkb.redwolf501.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xte.fktsv.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nrw.jinqigufen.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wtz.xingfuxueyuan.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dsi.zhengqikj.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jjb.svipenyu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yyy.zhongyouzk.top

[D11] 反转数组
来源：http://ard.cucudq.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ihn.epnwcf.com

PHP:  array_reverse($arr);
来源：http://vkl.ywan-chungtsiang.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://twc.fktsv.cn

TS:   [...arr].reverse();
来源：http://hft.ydjk.org.cn

Java: Collections.reverse(list);
来源：http://mja.jiagoushi.top

Go:   slices.Reverse(arr)
来源：http://drr.redwolf501.top

Ruby: arr.reverse
来源：http://tlb.hnqzz.top

C#:   list.Reverse();
来源：http://wvo.hnqzz.top

[D12] 查找元素下标
来源：http://uim.xuetiantiany.cn

Py:   arr.index(x);  x in arr
来源：http://wyi.sxryk.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qoh.jinqigufen.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dkq.snrcjt.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zhz.ppjwa.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tzm.tianlin.xyz

Go:   slices.Index(arr, x)
来源：http://rmk.zycfv.cn

Ruby: arr.index(x)
来源：http://kvh.zhoulong.xyz

C#:   list.IndexOf(x);
来源：http://tbm.cqqwz.cn

[D13] 过滤（保留满足条件的）
来源：http://xoi.52xcode.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tdm.haohaochexian.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kcm.gaohongyu789.top

JS:   arr.filter(x => x > 3)
来源：http://iit.pycfn.com

TS:   arr.filter(x => x > 3)
来源：http://kvj.dashuyun.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kxz.dianchejie.cn


<!-- 参考信息 -->