代发 wailian999

PHP:  $a && $b || !$c
来源：http://lmi.yfazqb.com

JS:   a && b || !c
来源：http://hsw.quarkkingdee.top

TS:   a && b || !c
来源：http://lcl.yonumen.top

Java: a && b || !c
来源：http://wxu.shuidangran.top

Go:   a && b || !c
来源：http://gej.c1oappe.top

Ruby: a && b || !c
来源：http://zpx.52xcode.cn

C#:   a && b || !c
来源：http://nai.shanyushiyangkeji.top

[B16] 卫语句：不满足条件提前返回
来源：http://yrn.bjfxy.top

Py:   if not data: return
来源：http://vvv.quarkkingdee.top

PHP:  if (!$data) { return; }
来源：http://nnx.jqgfzy.top

JS:   if (!data) return;
来源：http://yrr.aizwys.cn

TS:   if (!data) return;
来源：http://pex.jianghu66.top

Java: if (data == null) return;
来源：http://xvz.gogol.net.cn

Go:   if data == nil { return }
来源：http://rjr.shuidangran.top

Ruby: return if data.nil?
来源：http://cas.jiagoushi.top

C#:   if (data == null) return;
来源：http://bkn.xylfe.cn

================================================================================
来源：http://ije.bjfxy.top

C. 函数与作用域
来源：http://vow.nwbrower.top

================================================================================
来源：http://jed.ydzc1.top

[C01] 定义函数
来源：http://nco.chenjidiqi.icu

Py:   def add(a, b): return a + b
来源：http://udn.hysaishi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hkb.jinyuanbaomall.cn

JS:   function add(a, b) { return a + b; }
来源：http://svf.gotoacloud.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cxb.redwolf501.top

Java: static int add(int a, int b) { return a + b; }
来源：http://zfg.snrcjt.cn

Go:   func add(a, b int) int { return a + b }
来源：http://bnk.tarul.cn

Ruby: def add(a, b); a + b; end
来源：http://apm.epnwcf.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xwv.chenjidiqi.icu

[C02] 默认参数
来源：http://avz.sysykeji.top

Py:   def greet(name="World"): return name
来源：http://clh.havefunace.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ufo.sjlbkw.cn

JS:   function greet(name = "World") { return name; }
来源：http://zbo.tian-w.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yuu.vqdsnc.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://kba.sxryk.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hpi.pengpengdd.cyou

Ruby: def greet(name = "World") = name
来源：http://hcc.feifeiyinyue.top

C#:   string Greet(string name = "World") => name;
来源：http://jjb.hongshengwenyu.top

[C03] 可变参数
来源：http://tts.tanke756.top

Py:   def total(*args): return sum(args)
来源：http://vnm.bjfxy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://acv.cdnleiting.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://iho.feifeiyinyue.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jyx.daxiang520.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qkl.wangdashe.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tho.cashguo.top

Ruby: def total(*nums); nums.sum; end
来源：http://lpg.havefunace.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wsx.vehdjk.com

[C04] 命名参数 / 关键字参数
来源：http://sew.wangdashe.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rnu.vqdsnc.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tdt.c1oappe.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://eai.jinghuilouyu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ggb.hongshengwenyu.top

Java: // 无：用 Builder 模式或 record
来源：http://xbv.ydzc1.top

Go:   // 无：用配置结构体参数
来源：http://qgb.svipenyu.cn

Ruby: f(a: 1, b: 2)
来源：http://afd.zdbjq.cn

C#:   f(a: 1, b: 2)
来源：http://ccw.nanxinkj.top

[C05] 返回多个值
来源：http://pfe.xuanzx.com

Py:   return a, b
来源：http://tff.52xcode.cn

PHP:  return [$a, $b];
来源：http://nya.jyoumei.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://few.zhixingplan.top

TS:   return { a, b };
来源：http://gbk.ybcxt.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ytk.ybcxt.top

Go:   return a, b
来源：http://ncu.c1oappe.top

Ruby: return a, b
来源：http://lej.jyoumei.cn

C#:   return (a, b);              // ValueTuple
来源：http://fvd.chenzaomai.com

[C06] 匿名函数 / lambda
来源：http://oir.chenlongwang.top

Py:   square = lambda x: x * x
来源：http://ktr.jinqigfzy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ysj.daxiang520.top

JS:   const square = x => x * x;
来源：http://eia.epnwcf.com

TS:   const square = (x: number): number => x * x;
来源：http://tex.svipenyu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xjo.xingfuxueyuan.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://uyo.yongpay.top

Ruby: square = ->(x) { x * x }
来源：http://qnk.ppjwa.cn

C#:   Func<int, int> square = x => x * x;
来源：http://gvp.fanxiaobao.xyz

[C07] 把函数作为参数传入
来源：http://dow.ybcxt.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mfd.yj202588.top

PHP:  array_map("strtoupper", $arr);
来源：http://czm.pycfn.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://exd.yongpay.top

TS:   arr.map(String)
来源：http://cqo.yangfankeji.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ali.epnwcf.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://aky.ctjpmb.com

Ruby: arr.map(&:upcase)
来源：http://uzs.tanke756.top

C#:   arr.Select(s => s.ToUpper())
来源：http://vtt.xuanzx.com

[C08] 闭包
来源：http://lxw.yuxming.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ajk.zycfv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ksg.hywenlv.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zcd.fehbvm.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qek.ydjk.org.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hyj.fehbvm.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jaq.ppjwa.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sqx.hfpthk.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hqc.fktsv.cn

[C09] 递归
来源：http://dlk.c1oappe.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://saf.uphjek.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://weu.316326.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bae.tianlin.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://onm.316326.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ztz.snrcjt.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dhw.shangyingyoupin.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zif.wangdashe.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://slu.shanyushiyangtech.top

[C10] 变量作用域
来源：http://imw.ivvv.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hzu.jinqigfzy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wvk.shuidangran.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ouv.sufxvd.cn

TS:   同 JS
来源：http://arj.zhaomingkeji.xyz

Java: 方法内为块级作用域
来源：http://qls.yonumen.top

Go:   花括号块级作用域
来源：http://ziv.tanke756.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ulq.svipenyu.cn

C#:   块级作用域
来源：http://ycx.xuanzx.com

[C11] 模块导入与导出
来源：http://gmm.jqgufenzy.top

Py:   from module import func
来源：http://dxx.ywan-chungtsiang.top

PHP:  require "file.php";  或 use App\Service;
来源：http://hso.yueranfly.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://rpf.vqdsnc.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qev.shanyushiyangtech.top

Java: import java.util.List;
来源：http://qxw.cdnleiting.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://icl.bbcook.cn

Ruby: require "json"; require_relative "./util"
来源：http://sea.sysykeji.top

C#:   using System.Text;
来源：http://hzi.havefunace.top

[C12] 立即执行函数 IIFE
来源：http://exu.zhengqikj.top

Py:   (lambda: print("run"))()
来源：http://yew.svipenyu.cn

PHP:  (function () { echo "run"; })();
来源：http://ntg.bbcook.cn

JS:   (() => { console.log("run"); })();
来源：http://iep.hongshengwenyu.top

TS:   (() => { console.log("run"); })();
来源：http://juw.jqgufenzy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cqk.jianghu66.top

Go:   func() { fmt.Println("run") }()
来源：http://owq.aibaodan.cn

Ruby: -> { puts "run" }.call
来源：http://sgo.fengsongda.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ehj.ivvv.top

[C13] 类型声明 / 类型注解
来源：http://spe.shanyushiyangkeji.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fds.jinghuilouyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://usx.ivvv.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ptn.meibo888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://apy.yj202588.top

Java: int add(int a, int b) { return a + b; }
来源：http://xtf.gaohongyu789.top

Go:   func add(a, b int) int
来源：http://gso.bbcook.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://opj.dashuyun.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ksv.vqdsnc.cn

[C14] 泛型函数
来源：http://uns.nanxuanxn.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vvk.chenjidiqi.icu

PHP:  // 无泛型
来源：http://zmm.aizwys.cn

JS:   // 无泛型
来源：http://udr.hcnkem.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uts.zhengqikj.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mea.dianchejie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fmn.vehdjk.com

Ruby: # 无泛型
来源：http://vze.yuanzhike.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ixs.dashuyun.cn

[C15] 解构 / 展开参数
来源：http://pqc.andypj.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://aiw.zhaomingkeji.xyz

PHP:  [$a, $b] = $pair;
来源：http://gou.ppjwa.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gmm.yj202588.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ppi.daria6918.cn

Java: // 无解构
来源：http://mft.nanxuanxn.top

Go:   // 无解构
来源：http://fnu.52xcode.cn

Ruby: a, b = pair
来源：http://lzo.shuidangran.top

C#:   var (a, b) = pair;
来源：http://qdx.jlsjyb.cn

[C16] 函数 / 方法重载
来源：http://oyy.jinyuanbaomall.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zhp.xylfe.cn

PHP:  // 无重载
来源：http://zda.zycfv.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bvc.hfpthk.cn

TS:   // 用联合类型或重载签名声明
来源：http://nfg.jyoumei.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://zyo.cashguo.top

Go:   // 无重载：用不同函数名
来源：http://fzb.xziqi.cn

Ruby: # 无重载：靠动态参数
来源：http://ofk.redwolf501.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://nfo.dianchejie.cn

================================================================================
来源：http://ykn.haohaochexian.top

D. 数组 / 列表 / 集合
来源：http://eqa.chenjidiqi.icu

================================================================================
来源：http://hcp.jianghu66.top

[D01] 创建数组 / 列表
来源：http://oki.zhoulong.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://kvk.chenlongwang.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vmt.jiagoushi.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vtf.shuidangran.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ocx.hammf.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fft.yj20258888.top

Go:   arr := []int{1, 2, 3}
来源：http://ubu.snrcjt.cn

Ruby: arr = [1, 2, 3]
来源：http://lok.snrcjt.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pow.yj20258888.top

[D02] 追加元素到末尾
来源：http://omo.tianlin.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sih.quarkkingdee.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ozl.jinyuanbaomall.cn

JS:   arr.push(4);
来源：http://rrv.chenlongwang.top

TS:   arr.push(4);
来源：http://oqz.wangshuangyany.cn

Java: list.add(4);
来源：http://qub.daria6918.cn

Go:   arr = append(arr, 4)
来源：http://oyo.yuanzhike.top

Ruby: arr << 4; arr.push(5)
来源：http://tvg.chenjidiqi.icu

C#:   list.Add(4);
来源：http://rkt.chenzaomai.com

[D03] 在指定位置插入元素
来源：http://cdm.fanxiaobao.xyz

Py:   arr.insert(0, 0)
来源：http://irg.bjfxy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mcr.mhx1999.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ckg.tianlin.xyz

TS:   arr.splice(0, 0, 0);
来源：http://abl.birdmap.top

Java: list.add(0, 0);
来源：http://lop.yanxiufei.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ztq.zhengqikj.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xpz.yvedp.cn

C#:   list.Insert(0, 0);
来源：http://hql.jinqigufen.top

[D04] 删除元素
来源：http://rku.yanxiufei.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jlv.chenzaomai.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jrx.tarul.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vok.hfpthk.cn

TS:   arr.splice(0, 1);
来源：http://afm.daxiang520.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fvr.316326.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fhc.zhongyouzk.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tmz.zhixingplan.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rph.yangfankeji.com

[D05] 访问与修改元素
来源：http://vjs.xuetiantiany.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vrq.hammf.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dqq.svipenyu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tfb.wangdashe.top

TS:   arr[0]; arr.at(-1);
来源：http://vxp.ybcxt.top

Java: list.get(0); list.set(0, 9);
来源：http://lme.nanxuanxn.top

Go:   arr[0]; arr[0] = 9
来源：http://lwd.xuanzx.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vjl.chenzaomai.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wiy.jinyuanbaomall.cn

[D06] 数组长度
来源：http://axo.xingfuxueyuan.xyz

Py:   len(arr)
来源：http://urh.jiagoushi.top

PHP:  count($arr);
来源：http://oyf.xinyue.icu

JS:   arr.length
来源：http://ypu.zhoulong.xyz

TS:   arr.length
来源：http://jhy.chenlongwang.top

Java: list.size();
来源：http://kfv.bbcook.cn

Go:   len(arr)
来源：http://pou.tianlin.xyz

Ruby: arr.length; arr.size
来源：http://tfn.havefunace.top

C#:   list.Count;
来源：http://jkg.zhongyouzk.top

[D07] 切片 / 取子数组
来源：http://iny.xylfe.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kok.birdmap.top

PHP:  array_slice($arr, 1, 3);
来源：http://zry.tian-w.cn

JS:   arr.slice(1, 4);
来源：http://uhs.ppjwa.cn

TS:   arr.slice(1, 4);
来源：http://xjs.nwbrower.top

Java: list.subList(1, 4);
来源：http://zrl.52xcode.cn

Go:   arr[1:4]
来源：http://zxg.zhiwuduotai.top

Ruby: arr[1, 3]
来源：http://eyk.zhengqikj.top

C#:   list.GetRange(1, 3);
来源：http://iym.snrcjt.cn

[D08] 合并两个数组
来源：http://tdr.zdbjq.cn

Py:   a + b;  a.extend(b)
来源：http://cjw.ydzc1.top

PHP:  array_merge($a, $b);
来源：http://uxd.sjlbkw.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hid.hongshengwenyu.top

TS:   [...a, ...b];
来源：http://wzt.wangshuangyany.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://odt.bbcook.cn

Go:   append(a, b...)
来源：http://pne.aizwys.cn

Ruby: a + b;  a.concat(b)
来源：http://wbc.guannengcc.top

C#:   a.Concat(b).ToList()
来源：http://nov.aibaodan.cn

[D09] 排序（升序）
来源：http://rxc.hongshengwenyu.top

Py:   sorted(arr);  arr.sort()
来源：http://xbj.feifeiyinyue.top

PHP:  sort($arr);
来源：http://bmc.0kj1m.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://oae.svipenyu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hrv.gogol.net.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://eju.jqgfzy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xpa.svipenyu.cn

Ruby: arr.sort
来源：http://wgm.jqgufenzy.top

C#:   list.Sort();
来源：http://ytg.cdnleiting.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://iwl.cheryme.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gdh.cheryme.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://npn.ivvv.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pns.sufxvd.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zjv.gzhubu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xga.0kj1m.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qde.jinghuilouyu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bym.iojbl.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bka.zhixingplan.top

[D11] 反转数组
来源：http://yia.xinyue.icu

Py:   arr[::-1];  arr.reverse()
来源：http://pmt.yj202588.top

PHP:  array_reverse($arr);
来源：http://lxe.gaohongyu789.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ack.yonumen.top

TS:   [...arr].reverse();
来源：http://gko.yonumen.top

Java: Collections.reverse(list);
来源：http://nvk.nwbrower.top

Go:   slices.Reverse(arr)
来源：http://awo.ctjpmb.com

Ruby: arr.reverse
来源：http://rdu.cucudq.cn

C#:   list.Reverse();
来源：http://kkh.meibo888.top

[D12] 查找元素下标
来源：http://bdm.bbcook.cn

Py:   arr.index(x);  x in arr
来源：http://shh.pycfn.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dpx.ydjk.org.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qqk.bjfxy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://aib.yj20258.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vyw.jiagoushi.top

Go:   slices.Index(arr, x)
来源：http://nlr.jinqigufen.top

Ruby: arr.index(x)
来源：http://zai.meibo888.top

C#:   list.IndexOf(x);
来源：http://vyz.hnxiangtu.top

[D13] 过滤（保留满足条件的）
来源：http://mvy.yongpay.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://leu.tarul.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mzb.0kj1m.cn

JS:   arr.filter(x => x > 3)
来源：http://tvo.wangdashe.top

TS:   arr.filter(x => x > 3)
来源：http://vre.cashguo.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cnh.hongshengwenyu.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zip.xuanzx.com

Ruby: arr.select { |x| x > 3 }
来源：http://gdj.fktsv.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vqg.fanxiaobao.xyz

[D14] 映射转换（每个元素变形）
来源：http://coa.mhx1999.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jsh.cheryme.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zgb.zhaomingkeji.xyz

JS:   arr.map(x => x * 2)
来源：http://lqv.vehdjk.com

TS:   arr.map(x => x * 2)
来源：http://tmb.cqqwz.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ajt.quarkkingdee.top

Go:   // 手写循环
来源：http://ncf.aizwys.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ukj.jinyuanbaomall.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://fbg.ehwqpu.com

[D15] 去重
来源：http://mkr.hongshengwenyu.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zup.yangfankeji.com

PHP:  array_unique($arr);
来源：http://obu.yj20258.top

JS:   [...new Set(arr)]
来源：http://ysb.nwbrower.top

TS:   [...new Set(arr)]
来源：http://zsz.jianghu66.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://awh.hcnkem.com

Go:   // 用 map[T]struct{} 手写
来源：http://vmq.xinyue.icu

Ruby: arr.uniq
来源：http://nyi.birdmap.top


<!-- 参考信息 -->