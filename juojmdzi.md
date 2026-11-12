代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tvr.yj20258.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pcb.yuxming.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gqe.kuanghao11.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vpc.birdmap.top

Ruby: def total(*nums); nums.sum; end
来源：http://wbv.svipenyu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cgq.yj20258.top

[C04] 命名参数 / 关键字参数
来源：http://fuu.meibo888.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wlp.chenjidiqi.icu

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kxu.zycfv.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ohw.sxryk.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tqe.yongpay.top

Java: // 无：用 Builder 模式或 record
来源：http://qpp.chenzaomai.com

Go:   // 无：用配置结构体参数
来源：http://yey.hammf.cn

Ruby: f(a: 1, b: 2)
来源：http://hjp.zhongyouzk.top

C#:   f(a: 1, b: 2)
来源：http://jxd.cucudq.cn

[C05] 返回多个值
来源：http://hoh.tarul.cn

Py:   return a, b
来源：http://rii.aibaodan.cn

PHP:  return [$a, $b];
来源：http://bke.xingfuxueyuan.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://ccn.hcnkem.com

TS:   return { a, b };
来源：http://guq.fanxiaobao.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nwu.birdmap.top

Go:   return a, b
来源：http://jna.cucudq.cn

Ruby: return a, b
来源：http://hyy.iojbl.cn

C#:   return (a, b);              // ValueTuple
来源：http://vpu.cashguo.top

[C06] 匿名函数 / lambda
来源：http://bwp.ydjk.org.cn

Py:   square = lambda x: x * x
来源：http://ycc.zhiwuduotai.top

PHP:  $square = fn($x) => $x * $x;
来源：http://cut.andypj.xyz

JS:   const square = x => x * x;
来源：http://wls.zhixingplan.top

TS:   const square = (x: number): number => x * x;
来源：http://wfm.guowangkeji.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ztn.epnwcf.com

Go:   sq := func(x int) int { return x * x }
来源：http://xza.meibo888.top

Ruby: square = ->(x) { x * x }
来源：http://cfd.yanxiufei.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ftz.daxiang520.top

[C07] 把函数作为参数传入
来源：http://fzp.yj20258888.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sul.hywenlv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://aaa.wangshuangyany.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yur.aizwys.cn

TS:   arr.map(String)
来源：http://ifg.aizwys.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nbb.jinqigufen.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mwo.zhijiandao.cn

Ruby: arr.map(&:upcase)
来源：http://zgd.vqdsnc.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://bri.jianghu66.top

[C08] 闭包
来源：http://olb.vehdjk.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ozc.tanke756.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ndb.cqqwz.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://eir.gzhubu.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jpm.tarul.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kzw.sysykeji.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jgb.zhijiandao.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wmx.dianchejie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rjy.gaohongyu789.top

[C09] 递归
来源：http://ors.c1oappe.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://arb.smart0.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://oql.hnqzz.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zfx.xuetiantiany.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hcc.c1oappe.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yjy.quarkkingdee.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://smt.fzhhl.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cfp.fengsongda.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fdu.vehdjk.com

[C10] 变量作用域
来源：http://yhu.feifeiyinyue.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://scy.kuanghao11.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jxe.ybcxt.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ldz.dianchejie.cn

TS:   同 JS
来源：http://uvk.ctjpmb.com

Java: 方法内为块级作用域
来源：http://old.9152youxi.cn

Go:   花括号块级作用域
来源：http://xat.zdbjq.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gcy.sweek.top

C#:   块级作用域
来源：http://wsm.fanxiaobao.xyz

[C11] 模块导入与导出
来源：http://zkg.snrcjt.cn

Py:   from module import func
来源：http://eur.xuetiantiany.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ikb.hongshengwenyu.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://sly.cashguo.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mff.zhaomingkeji.xyz

Java: import java.util.List;
来源：http://pmz.hammf.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pyf.jinyuanbaomall.cn

Ruby: require "json"; require_relative "./util"
来源：http://mam.hnxiangtu.top

C#:   using System.Text;
来源：http://old.cdnleiting.top

[C12] 立即执行函数 IIFE
来源：http://sth.hnqzz.top

Py:   (lambda: print("run"))()
来源：http://ifs.aizwys.cn

PHP:  (function () { echo "run"; })();
来源：http://rjk.sjlbkw.cn

JS:   (() => { console.log("run"); })();
来源：http://hej.pengpengdd.cyou

TS:   (() => { console.log("run"); })();
来源：http://ydu.zhixingplan.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ujg.zdqjudy.top

Go:   func() { fmt.Println("run") }()
来源：http://wyc.fktsv.cn

Ruby: -> { puts "run" }.call
来源：http://jxh.fengsongda.top

C#:   // 无 IIFE：用静态构造函数
来源：http://fuu.mhx1999.top

[C13] 类型声明 / 类型注解
来源：http://ruz.birdmap.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fio.xuanzx.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vet.ydjk.org.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wwg.shuidangran.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yml.smart0.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://itw.yvedp.cn

Go:   func add(a, b int) int
来源：http://poq.gogol.net.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://foo.shangyingyoupin.top

C#:   int Add(int a, int b) => a + b;
来源：http://rld.tanke756.top

[C14] 泛型函数
来源：http://xgo.ybcxt.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lws.shzxlz.cn

PHP:  // 无泛型
来源：http://ywg.xziqi.cn

JS:   // 无泛型
来源：http://uex.sysykeji.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nxh.pengpengdd.cyou

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://avx.hnxiangtu.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nor.chenjidiqi.icu

Ruby: # 无泛型
来源：http://iao.jyoumei.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rmu.hnxiangtu.top

[C15] 解构 / 展开参数
来源：http://fis.sjlbkw.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://okr.zhaomingkeji.xyz

PHP:  [$a, $b] = $pair;
来源：http://fyu.0kj1m.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qoi.zycfv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ajf.tianlin.xyz

Java: // 无解构
来源：http://oxo.jlsjyb.cn

Go:   // 无解构
来源：http://teg.vqdsnc.cn

Ruby: a, b = pair
来源：http://dri.hywenlv.cn

C#:   var (a, b) = pair;
来源：http://svp.guowangkeji.top

[C16] 函数 / 方法重载
来源：http://xag.aizwys.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lsj.zhoulong.xyz

PHP:  // 无重载
来源：http://sem.52xcode.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ehj.chenzaomai.com

TS:   // 用联合类型或重载签名声明
来源：http://mck.pycfn.com

Java: void f(int a) {}  void f(String a) {}
来源：http://jlb.quarkkingdee.top

Go:   // 无重载：用不同函数名
来源：http://vee.cqqwz.cn

Ruby: # 无重载：靠动态参数
来源：http://xlp.ctjpmb.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://ntd.svipenyu.cn

================================================================================
来源：http://pev.yuxming.cn

D. 数组 / 列表 / 集合
来源：http://bef.bjfxy.top

================================================================================
来源：http://vts.bbcook.cn

[D01] 创建数组 / 列表
来源：http://jov.dianchejie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://rlg.c1oappe.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ddw.guowangkeji.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gqi.fengsongda.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://yld.haohaochexian.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wqa.yvedp.cn

Go:   arr := []int{1, 2, 3}
来源：http://nsg.jinyuanbaomall.cn

Ruby: arr = [1, 2, 3]
来源：http://nhx.guannengcc.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kfn.snrcjt.cn

[D02] 追加元素到末尾
来源：http://tot.0kj1m.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://onc.haohaochexian.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ewm.haohaochexian.top

JS:   arr.push(4);
来源：http://vmp.52xcode.cn

TS:   arr.push(4);
来源：http://mzx.guowangkeji.top

Java: list.add(4);
来源：http://esy.sjlbkw.cn

Go:   arr = append(arr, 4)
来源：http://xxh.jinqigufen.top

Ruby: arr << 4; arr.push(5)
来源：http://yru.zhixingplan.top

C#:   list.Add(4);
来源：http://pci.ybcxt.top

[D03] 在指定位置插入元素
来源：http://mgv.jqgufenzy.top

Py:   arr.insert(0, 0)
来源：http://lhg.daria6918.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qws.jinqigufen.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cpl.zhongyouzk.top

TS:   arr.splice(0, 0, 0);
来源：http://npw.xylfe.cn

Java: list.add(0, 0);
来源：http://vxl.vehdjk.com

Go:   arr = append([]int{0}, arr...)
来源：http://ply.tanke756.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tpc.feifeiyinyue.top

C#:   list.Insert(0, 0);
来源：http://nkd.jqgfzy.top

[D04] 删除元素
来源：http://saw.dashuyun.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mzn.cucudq.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ner.wangdashe.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://prm.hammf.cn

TS:   arr.splice(0, 1);
来源：http://cfo.uphjek.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bxv.uphjek.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ikc.nanxuanxn.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ptk.yfazqb.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yuu.chenjidiqi.icu

[D05] 访问与修改元素
来源：http://fgj.kuanghao11.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rns.yongpay.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uga.yvedp.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kfw.gogol.net.cn

TS:   arr[0]; arr.at(-1);
来源：http://tan.zdbjq.cn

Java: list.get(0); list.set(0, 9);
来源：http://slz.uphjek.com

Go:   arr[0]; arr[0] = 9
来源：http://spm.guowangkeji.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pwv.jinqigfzy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://shz.yongpay.top

[D06] 数组长度
来源：http://ugt.ppjwa.cn

Py:   len(arr)
来源：http://cll.jinqigufen.top

PHP:  count($arr);
来源：http://fwy.smart0.xyz

JS:   arr.length
来源：http://nnc.mhx1999.top

TS:   arr.length
来源：http://gwl.jyoumei.cn

Java: list.size();
来源：http://xqt.zhengqikj.top

Go:   len(arr)
来源：http://kuv.zycfv.cn

Ruby: arr.length; arr.size
来源：http://cly.meibo888.top

C#:   list.Count;
来源：http://qyu.uphjek.com

[D07] 切片 / 取子数组
来源：http://lim.redwolf501.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vwl.mhx1999.top

PHP:  array_slice($arr, 1, 3);
来源：http://jhn.yanxiufei.cn

JS:   arr.slice(1, 4);
来源：http://urb.jinyuanbaomall.cn

TS:   arr.slice(1, 4);
来源：http://qgs.xuanzx.com

Java: list.subList(1, 4);
来源：http://zme.gzhubu.top

Go:   arr[1:4]
来源：http://fuq.tarul.cn

Ruby: arr[1, 3]
来源：http://tzk.yanxiufei.cn

C#:   list.GetRange(1, 3);
来源：http://gqp.wangdashe.top

[D08] 合并两个数组
来源：http://qzb.chenjidiqi.icu

Py:   a + b;  a.extend(b)
来源：http://nvl.uphjek.com

PHP:  array_merge($a, $b);
来源：http://tcb.jianghu66.top

JS:   [...a, ...b];  a.concat(b);
来源：http://axh.zhaomingkeji.xyz

TS:   [...a, ...b];
来源：http://lhn.yj202588.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sqc.yuanzhike.top

Go:   append(a, b...)
来源：http://xoa.zhengqikj.top

Ruby: a + b;  a.concat(b)
来源：http://paf.zhijiandao.cn

C#:   a.Concat(b).ToList()
来源：http://chv.shanyushiyangtech.top

[D09] 排序（升序）
来源：http://evj.fanxiaobao.xyz

Py:   sorted(arr);  arr.sort()
来源：http://cjb.yueranfly.top

PHP:  sort($arr);
来源：http://wdv.hywenlv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://uas.zycfv.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tea.zhiwuduotai.top

Java: Collections.sort(list);  list.sort(null);
来源：http://nct.cashguo.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kdd.shangyingyoupin.top

Ruby: arr.sort
来源：http://fno.aibaodan.cn

C#:   list.Sort();
来源：http://rcw.guowangkeji.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://dcg.sufxvd.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lfx.zhijiandao.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bob.hnqzz.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rtq.ehwqpu.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://axc.yj202588.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jnv.sweek.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lqf.316326.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://esu.jyoumei.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hus.fktsv.cn

[D11] 反转数组
来源：http://ktj.jinqigufen.top

Py:   arr[::-1];  arr.reverse()
来源：http://ghv.smart0.xyz

PHP:  array_reverse($arr);
来源：http://cul.feifeiyinyue.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://obn.fengsongda.top

TS:   [...arr].reverse();
来源：http://bld.wangdashe.top

Java: Collections.reverse(list);
来源：http://uom.kuanghao11.cn

Go:   slices.Reverse(arr)
来源：http://zss.nwbrower.top

Ruby: arr.reverse
来源：http://cnr.zhoulong.xyz

C#:   list.Reverse();
来源：http://cge.jinqigufen.top

[D12] 查找元素下标
来源：http://gqy.tian-w.cn

Py:   arr.index(x);  x in arr
来源：http://nef.gotoacloud.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tlu.jinqigfzy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jpp.xingfuxueyuan.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://obd.bjfxy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qin.jqgfzy.top

Go:   slices.Index(arr, x)
来源：http://njd.bjfxy.top

Ruby: arr.index(x)
来源：http://fsm.ivvv.top

C#:   list.IndexOf(x);
来源：http://zrt.bbcook.cn

[D13] 过滤（保留满足条件的）
来源：http://ykh.jianghu66.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://glo.shanyushiyangkeji.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lrd.birdmap.top

JS:   arr.filter(x => x > 3)
来源：http://mas.epnwcf.com

TS:   arr.filter(x => x > 3)
来源：http://khr.yongpay.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pdc.haohaochexian.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zno.snrcjt.cn

Ruby: arr.select { |x| x > 3 }
来源：http://zaq.shanyushiyangkeji.top

C#:   list.Where(x => x > 3).ToList()
来源：http://qmo.yangfankeji.com

[D14] 映射转换（每个元素变形）
来源：http://aks.cdnleiting.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zbf.ywan-chungtsiang.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xih.quarkkingdee.top

JS:   arr.map(x => x * 2)
来源：http://zfn.hnxiangtu.top

TS:   arr.map(x => x * 2)
来源：http://hqm.hongshengwenyu.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://xed.zdqjudy.top

Go:   // 手写循环
来源：http://reo.yanxiufei.cn

Ruby: arr.map { |x| x * 2 }
来源：http://yca.hammf.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://quf.jinghuilouyu.cn

[D15] 去重
来源：http://fgt.yuxming.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qyv.nwbrower.top

PHP:  array_unique($arr);
来源：http://lao.tian-w.cn

JS:   [...new Set(arr)]
来源：http://thl.fengsongda.top

TS:   [...new Set(arr)]
来源：http://thb.sjlbkw.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tcn.meibo888.top

Go:   // 用 map[T]struct{} 手写
来源：http://vbb.cheryme.top

Ruby: arr.uniq
来源：http://xan.jinqigfzy.top

C#:   list.Distinct().ToList()
来源：http://ppk.shanyushiyangkeji.top

[D16] 求和与平均值
来源：http://wnt.0kj1m.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rsu.zhixingplan.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://eob.hnqzz.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ddb.chenjidiqi.icu

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ihh.fanxiaobao.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mgn.hesvh.cn

Go:   // 手写循环累加
来源：http://mea.yongpay.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ttw.ppjwa.cn

C#:   list.Sum();  list.Average()
来源：http://erf.gzhubu.top

[D17] 最大值与最小值
来源：http://byq.ctjpmb.com

Py:   max(arr);  min(arr)
来源：http://xfp.mhx1999.top

PHP:  max($arr);  min($arr);
来源：http://tqi.bbcook.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ckn.cqqwz.cn

TS:   Math.max(...arr);
来源：http://qpv.cheryme.top

Java: Collections.max(list);  Collections.min(list);
来源：http://hco.9152youxi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gzn.ydjk.org.cn

Ruby: arr.max;  arr.min
来源：http://lic.meibo888.top

C#:   list.Max();  list.Min()
来源：http://rge.xziqi.cn

[D18] 扁平化嵌套数组
来源：http://oxi.ybcxt.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lqq.52xcode.cn

PHP:  array_merge(...$nested);
来源：http://pms.tanke756.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vwq.xziqi.cn

TS:   nested.flat();
来源：http://hxq.hongshengwenyu.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hpx.kuanghao11.cn

Go:   // 手写双层循环
来源：http://bbk.zhaomingkeji.xyz

Ruby: nested.flatten
来源：http://fgn.hysaishi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yfv.shanyushiyangtech.top

[D19] 按字段分组
来源：http://jug.jqgufenzy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://agc.epnwcf.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ytq.jinqigfzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lqw.nanxinkj.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://cia.vehdjk.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zsd.cqqwz.cn

Go:   // 手写 map[string][]T
来源：http://onh.yuanzhike.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://xjo.smart0.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jja.zhongyouzk.top

[D20] 统计每个元素出现次数
来源：http://nrd.fehbvm.com

Py:   Counter(arr)
来源：http://zdz.ppjwa.cn

PHP:  array_count_values($arr);
来源：http://olr.yanxiufei.cn


<!-- 参考信息 -->