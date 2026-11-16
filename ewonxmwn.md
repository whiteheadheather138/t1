代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hsr.9152youxi.cn

TS:   arr.map(String)
来源：http://fom.yj20258888.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wrc.jyoumei.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hde.ppjwa.cn

Ruby: arr.map(&:upcase)
来源：http://jqe.pycfn.com

C#:   arr.Select(s => s.ToUpper())
来源：http://izk.0kj1m.cn

[C08] 闭包
来源：http://xfv.gogol.net.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kmm.ydzc1.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nuv.xziqi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://czv.zhengqikj.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://klz.xylfe.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://guo.wangdashe.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://goi.zhaomingkeji.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uer.fzhhl.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ayc.pengpengdd.cyou

[C09] 递归
来源：http://exb.zhongyouzk.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yxo.gaohongyu789.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hvb.epnwcf.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ymw.zdqjudy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lbo.hywenlv.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sem.smart0.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ans.jyoumei.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qvl.xingfuxueyuan.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lsq.yuxming.cn

[C10] 变量作用域
来源：http://wbk.pengpengdd.cyou

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sbq.gotoacloud.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://elf.xuetiantiany.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kmd.zycfv.cn

TS:   同 JS
来源：http://mmb.zhaomingkeji.xyz

Java: 方法内为块级作用域
来源：http://wvp.yuanzhike.top

Go:   花括号块级作用域
来源：http://hfv.aibaodan.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ymu.cdnleiting.top

C#:   块级作用域
来源：http://vhf.zhixingplan.top

[C11] 模块导入与导出
来源：http://aoz.yanxiufei.cn

Py:   from module import func
来源：http://ntu.vqdsnc.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bjd.yangfankeji.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://wep.52xcode.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hfv.kuanghao11.cn

Java: import java.util.List;
来源：http://wfc.bjfxy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ofb.jqgufenzy.top

Ruby: require "json"; require_relative "./util"
来源：http://ghl.shanyushiyangtech.top

C#:   using System.Text;
来源：http://iks.fehbvm.com

[C12] 立即执行函数 IIFE
来源：http://pmw.yj202588.top

Py:   (lambda: print("run"))()
来源：http://xia.yongpay.top

PHP:  (function () { echo "run"; })();
来源：http://yfj.haohaochexian.top

JS:   (() => { console.log("run"); })();
来源：http://kui.jyoumei.cn

TS:   (() => { console.log("run"); })();
来源：http://tke.hnqzz.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fhd.zycfv.cn

Go:   func() { fmt.Println("run") }()
来源：http://pkm.zhijiandao.cn

Ruby: -> { puts "run" }.call
来源：http://igt.ywan-chungtsiang.top

C#:   // 无 IIFE：用静态构造函数
来源：http://qkq.hywenlv.cn

[C13] 类型声明 / 类型注解
来源：http://ard.yj20258.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kwp.chenzaomai.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wdq.fengsongda.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hxk.hfpthk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://npv.pycfn.com

Java: int add(int a, int b) { return a + b; }
来源：http://erd.ctjpmb.com

Go:   func add(a, b int) int
来源：http://uqg.aibaodan.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://aqg.tarul.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tcw.jlsjyb.cn

[C14] 泛型函数
来源：http://jvz.wangshuangyany.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nij.svipenyu.cn

PHP:  // 无泛型
来源：http://zlq.xylfe.cn

JS:   // 无泛型
来源：http://qyr.hcnkem.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jzh.snrcjt.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wlm.xuetiantiany.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://scg.quarkkingdee.top

Ruby: # 无泛型
来源：http://rpa.snrcjt.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kzf.cdnleiting.top

[C15] 解构 / 展开参数
来源：http://omx.chenzaomai.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fmi.mhx1999.top

PHP:  [$a, $b] = $pair;
来源：http://sfu.meibo888.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://sdt.zhixingplan.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rvm.yuxming.cn

Java: // 无解构
来源：http://mqo.xuetiantiany.cn

Go:   // 无解构
来源：http://piv.yj20258888.top

Ruby: a, b = pair
来源：http://hnv.nanxuanxn.top

C#:   var (a, b) = pair;
来源：http://wqm.hesvh.cn

[C16] 函数 / 方法重载
来源：http://rkg.yj20258.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://len.aizwys.cn

PHP:  // 无重载
来源：http://xvq.xuetiantiany.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bni.hnxiangtu.top

TS:   // 用联合类型或重载签名声明
来源：http://hkk.ydzc1.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ynd.jqgufenzy.top

Go:   // 无重载：用不同函数名
来源：http://cgc.zhaomingkeji.xyz

Ruby: # 无重载：靠动态参数
来源：http://hsl.fanxiaobao.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://ixg.jinqigfzy.top

================================================================================
来源：http://rmn.jinyuanbaomall.cn

D. 数组 / 列表 / 集合
来源：http://cpd.ywan-chungtsiang.top

================================================================================
来源：http://hzh.birdmap.top

[D01] 创建数组 / 列表
来源：http://esa.zhoulong.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://wlz.yonumen.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lwc.jiagoushi.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lsw.gogol.net.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://mfy.52xcode.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://oyx.zhiwuduotai.top

Go:   arr := []int{1, 2, 3}
来源：http://ecm.ivvv.top

Ruby: arr = [1, 2, 3]
来源：http://fqq.redwolf501.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://coi.yonumen.top

[D02] 追加元素到末尾
来源：http://epi.bbcook.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://eig.yj202588.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sbs.svipenyu.cn

JS:   arr.push(4);
来源：http://hrq.hcnkem.com

TS:   arr.push(4);
来源：http://uos.tianlin.xyz

Java: list.add(4);
来源：http://kla.cqqwz.cn

Go:   arr = append(arr, 4)
来源：http://tet.yj20258888.top

Ruby: arr << 4; arr.push(5)
来源：http://dan.tanke756.top

C#:   list.Add(4);
来源：http://mcf.zhixingplan.top

[D03] 在指定位置插入元素
来源：http://kgk.dashuyun.cn

Py:   arr.insert(0, 0)
来源：http://ydk.gotoacloud.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vcl.shanyushiyangtech.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://luv.fanxiaobao.xyz

TS:   arr.splice(0, 0, 0);
来源：http://qoo.kuanghao11.cn

Java: list.add(0, 0);
来源：http://dil.yj202588.top

Go:   arr = append([]int{0}, arr...)
来源：http://gxy.fanxiaobao.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pok.yongpay.top

C#:   list.Insert(0, 0);
来源：http://ybl.fktsv.cn

[D04] 删除元素
来源：http://lxl.pycfn.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yrn.chenjidiqi.icu

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nvs.jlsjyb.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ray.dianchejie.cn

TS:   arr.splice(0, 1);
来源：http://nnz.ehwqpu.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://adk.fktsv.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pla.daxiang520.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wuq.jqgufenzy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cym.fanxiaobao.xyz

[D05] 访问与修改元素
来源：http://ldk.ybcxt.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jbn.cheryme.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kdt.meibo888.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://erz.c1oappe.top

TS:   arr[0]; arr.at(-1);
来源：http://exo.vehdjk.com

Java: list.get(0); list.set(0, 9);
来源：http://oxe.jinghuilouyu.cn

Go:   arr[0]; arr[0] = 9
来源：http://xna.wangdashe.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://buy.daria6918.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zjd.cheryme.top

[D06] 数组长度
来源：http://tck.vqdsnc.cn

Py:   len(arr)
来源：http://yic.yongpay.top

PHP:  count($arr);
来源：http://zqp.jqgufenzy.top

JS:   arr.length
来源：http://sjr.hysaishi.cn

TS:   arr.length
来源：http://pco.yangfankeji.com

Java: list.size();
来源：http://rvt.jinqigfzy.top

Go:   len(arr)
来源：http://psw.cashguo.top

Ruby: arr.length; arr.size
来源：http://eqw.sysykeji.top

C#:   list.Count;
来源：http://eki.ehwqpu.com

[D07] 切片 / 取子数组
来源：http://cuo.zycfv.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ecl.nanxuanxn.top

PHP:  array_slice($arr, 1, 3);
来源：http://gon.feifeiyinyue.top

JS:   arr.slice(1, 4);
来源：http://zdy.gotoacloud.top

TS:   arr.slice(1, 4);
来源：http://lro.ybcxt.top

Java: list.subList(1, 4);
来源：http://xsb.svipenyu.cn

Go:   arr[1:4]
来源：http://myq.dianchejie.cn

Ruby: arr[1, 3]
来源：http://pyb.nwbrower.top

C#:   list.GetRange(1, 3);
来源：http://hcv.xuanzx.com

[D08] 合并两个数组
来源：http://xka.yongpay.top

Py:   a + b;  a.extend(b)
来源：http://lfj.sysykeji.top

PHP:  array_merge($a, $b);
来源：http://hzx.meibo888.top

JS:   [...a, ...b];  a.concat(b);
来源：http://hmm.zhengqikj.top

TS:   [...a, ...b];
来源：http://hec.0kj1m.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nza.dashuyun.cn

Go:   append(a, b...)
来源：http://pic.kuanghao11.cn

Ruby: a + b;  a.concat(b)
来源：http://zku.zdqjudy.top

C#:   a.Concat(b).ToList()
来源：http://wdg.daria6918.cn

[D09] 排序（升序）
来源：http://osk.yueranfly.top

Py:   sorted(arr);  arr.sort()
来源：http://bss.316326.xyz

PHP:  sort($arr);
来源：http://qhq.jianghu66.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lyc.hesvh.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://lim.zhongyouzk.top

Java: Collections.sort(list);  list.sort(null);
来源：http://pyn.cdnleiting.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://upp.yj20258888.top

Ruby: arr.sort
来源：http://gtn.zhijiandao.cn

C#:   list.Sort();
来源：http://abl.xingfuxueyuan.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://cpt.ivvv.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yhg.ywan-chungtsiang.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ldq.yj20258888.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://whv.zhongyouzk.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tqa.ywan-chungtsiang.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rdy.aibaodan.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ckn.uphjek.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kgs.nwbrower.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nwx.guowangkeji.top

[D11] 反转数组
来源：http://kkj.jyoumei.cn

Py:   arr[::-1];  arr.reverse()
来源：http://rkf.sysykeji.top

PHP:  array_reverse($arr);
来源：http://ipn.jianghu66.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kjo.cdnleiting.top

TS:   [...arr].reverse();
来源：http://dii.gzhubu.top

Java: Collections.reverse(list);
来源：http://fjw.fzhhl.top

Go:   slices.Reverse(arr)
来源：http://pgs.yueranfly.top

Ruby: arr.reverse
来源：http://yib.gotoacloud.top

C#:   list.Reverse();
来源：http://xew.kuanghao11.cn

[D12] 查找元素下标
来源：http://ekf.yangfankeji.com

Py:   arr.index(x);  x in arr
来源：http://ryc.yj202588.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cae.xuanzx.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dmm.jinqigfzy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fqr.chenlongwang.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://srk.fehbvm.com

Go:   slices.Index(arr, x)
来源：http://cjc.meibo888.top

Ruby: arr.index(x)
来源：http://pal.zhiwuduotai.top

C#:   list.IndexOf(x);
来源：http://aew.xingfuxueyuan.xyz

[D13] 过滤（保留满足条件的）
来源：http://irj.fehbvm.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://apc.hnxiangtu.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://eib.fktsv.cn

JS:   arr.filter(x => x > 3)
来源：http://sqx.kuanghao11.cn

TS:   arr.filter(x => x > 3)
来源：http://xul.fktsv.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://eyg.zhengqikj.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lbs.feifeiyinyue.top

Ruby: arr.select { |x| x > 3 }
来源：http://bun.haohaochexian.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ocx.cheryme.top

[D14] 映射转换（每个元素变形）
来源：http://wnl.jlsjyb.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rbm.gotoacloud.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hxi.uphjek.com

JS:   arr.map(x => x * 2)
来源：http://znd.bjfxy.top

TS:   arr.map(x => x * 2)
来源：http://ddo.fanxiaobao.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://lfk.fengsongda.top

Go:   // 手写循环
来源：http://cnn.yangfankeji.com

Ruby: arr.map { |x| x * 2 }
来源：http://fzr.fktsv.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://onp.gogol.net.cn

[D15] 去重
来源：http://mzd.nwbrower.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ygx.shangyingyoupin.top

PHP:  array_unique($arr);
来源：http://dso.jinqigufen.top

JS:   [...new Set(arr)]
来源：http://kfo.shanyushiyangtech.top

TS:   [...new Set(arr)]
来源：http://kpe.aizwys.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gvn.nwbrower.top

Go:   // 用 map[T]struct{} 手写
来源：http://zxk.hfpthk.cn

Ruby: arr.uniq
来源：http://txm.zhiwuduotai.top

C#:   list.Distinct().ToList()
来源：http://bqw.dashuyun.cn

[D16] 求和与平均值
来源：http://tlx.zhongyouzk.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xrh.guannengcc.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://buw.chenzaomai.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pmn.jianghu66.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gcu.birdmap.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://owo.jinghuilouyu.cn

Go:   // 手写循环累加
来源：http://mxn.fktsv.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bfz.gaohongyu789.top

C#:   list.Sum();  list.Average()
来源：http://qoe.smart0.xyz

[D17] 最大值与最小值
来源：http://lhd.hnqzz.top

Py:   max(arr);  min(arr)
来源：http://ald.yvedp.cn

PHP:  max($arr);  min($arr);
来源：http://oxh.jiagoushi.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sew.jqgufenzy.top

TS:   Math.max(...arr);
来源：http://fvq.haohaochexian.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ehr.shanyushiyangkeji.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qdw.dianchejie.cn

Ruby: arr.max;  arr.min
来源：http://nbd.meibo888.top

C#:   list.Max();  list.Min()
来源：http://huz.pycfn.com

[D18] 扁平化嵌套数组
来源：http://kvk.xuetiantiany.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wib.zdqjudy.top

PHP:  array_merge(...$nested);
来源：http://omy.zdbjq.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hoq.snrcjt.cn

TS:   nested.flat();
来源：http://krq.ehwqpu.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bfr.jianghu66.top

Go:   // 手写双层循环
来源：http://tbw.yonumen.top

Ruby: nested.flatten
来源：http://lpi.havefunace.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://dsv.zdqjudy.top

[D19] 按字段分组
来源：http://awk.xziqi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vzy.yonumen.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zfw.jqgufenzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sge.9152youxi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rlw.uphjek.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://voo.birdmap.top

Go:   // 手写 map[string][]T
来源：http://aof.cheryme.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://qgh.feifeiyinyue.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://sgw.fanxiaobao.xyz

[D20] 统计每个元素出现次数
来源：http://zal.dianchejie.cn

Py:   Counter(arr)
来源：http://nhs.yfazqb.com

PHP:  array_count_values($arr);
来源：http://ytt.dashuyun.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sex.hnxiangtu.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mba.yongpay.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cbl.hfpthk.cn

Go:   // 手写 map[T]int
来源：http://jgi.shangyingyoupin.top

Ruby: arr.tally
来源：http://ajo.vehdjk.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rtw.xylfe.cn

[D21] 判断是否包含某元素
来源：http://yip.yanxiufei.cn

Py:   x in arr
来源：http://jtf.ybcxt.top

PHP:  in_array($x, $arr, true);
来源：http://zqi.birdmap.top

JS:   arr.includes(x)
来源：http://ing.yvedp.cn

TS:   arr.includes(x)
来源：http://gse.tanke756.top

Java: list.contains(x)
来源：http://jxh.jinyuanbaomall.cn

Go:   slices.Contains(arr, x)
来源：http://omd.yueranfly.top

Ruby: arr.include?(x)
来源：http://bvu.gzhubu.top

C#:   list.Contains(x)
来源：http://fup.hnxiangtu.top

[D22] 复制数组（避免共享引用）
来源：http://mpx.zdqjudy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://opo.pengpengdd.cyou

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xdi.fanxiaobao.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://miu.hnxiangtu.top

TS:   [...arr];
来源：http://kmn.ppjwa.cn

Java: new ArrayList<>(list);
来源：http://bts.nwbrower.top

Go:   copied := append([]int(nil), arr...)
来源：http://hkc.hesvh.cn

Ruby: arr.dup;  arr.clone
来源：http://slz.dianchejie.cn

C#:   new List<int>(list);
来源：http://rxj.yj20258.top

[D23] reduce 累积计算
来源：http://dji.gogol.net.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qug.shuidangran.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zrv.aizwys.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mhz.hnxiangtu.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pzs.gaohongyu789.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://jvo.cheryme.top

Go:   // 手写循环
来源：http://bkw.yonumen.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tuw.zdqjudy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wvl.9152youxi.cn

[D24] 字典 / Map 基本操作
来源：http://wyi.cheryme.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://iia.bjfxy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pxt.ybcxt.top


<!-- 参考信息 -->