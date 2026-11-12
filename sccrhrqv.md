代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://rkt.zhixingplan.top

[C07] 把函数作为参数传入
来源：http://hkh.gotoacloud.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yak.svipenyu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://mny.sufxvd.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hhp.yuanzhike.top

TS:   arr.map(String)
来源：http://sqq.yuxming.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zli.gotoacloud.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cbm.nanxuanxn.top

Ruby: arr.map(&:upcase)
来源：http://udn.sxryk.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://roy.epnwcf.com

[C08] 闭包
来源：http://oyg.xylfe.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://twa.fengsongda.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xpz.yj20258888.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lkr.yj20258888.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yjf.bjfxy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nks.yj20258888.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://brt.zdqjudy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lom.zhoulong.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zst.gotoacloud.top

[C09] 递归
来源：http://rpj.zhoulong.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vqy.shuidangran.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tab.hammf.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hfr.ppjwa.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ari.mhx1999.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fes.tanke756.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ktc.aizwys.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vpj.yangfankeji.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://aqv.hysaishi.cn

[C10] 变量作用域
来源：http://hwx.jqgfzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vhh.nanxinkj.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://oci.c1oappe.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dkl.sjlbkw.cn

TS:   同 JS
来源：http://wys.chenlongwang.top

Java: 方法内为块级作用域
来源：http://cmn.9152youxi.cn

Go:   花括号块级作用域
来源：http://lts.gzhubu.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gkh.sufxvd.cn

C#:   块级作用域
来源：http://ekz.aibaodan.cn

[C11] 模块导入与导出
来源：http://lpj.gzhubu.top

Py:   from module import func
来源：http://gqi.hcnkem.com

PHP:  require "file.php";  或 use App\Service;
来源：http://kwv.zhongyouzk.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://rny.chenlongwang.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mro.cqqwz.cn

Java: import java.util.List;
来源：http://mun.zycfv.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zao.aizwys.cn

Ruby: require "json"; require_relative "./util"
来源：http://rcx.vehdjk.com

C#:   using System.Text;
来源：http://raz.fanxiaobao.xyz

[C12] 立即执行函数 IIFE
来源：http://wad.shzxlz.cn

Py:   (lambda: print("run"))()
来源：http://ayp.shanyushiyangkeji.top

PHP:  (function () { echo "run"; })();
来源：http://ota.kuanghao11.cn

JS:   (() => { console.log("run"); })();
来源：http://nuk.wangdashe.top

TS:   (() => { console.log("run"); })();
来源：http://ghm.sweek.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ruo.yfazqb.com

Go:   func() { fmt.Println("run") }()
来源：http://kmz.cdnleiting.top

Ruby: -> { puts "run" }.call
来源：http://hdd.smart0.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://xha.havefunace.top

[C13] 类型声明 / 类型注解
来源：http://met.chenzaomai.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kuo.jqgfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qnd.fengsongda.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://evs.hnxiangtu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ein.yongpay.top

Java: int add(int a, int b) { return a + b; }
来源：http://uhc.ppjwa.cn

Go:   func add(a, b int) int
来源：http://gyw.uphjek.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rhm.cqqwz.cn

C#:   int Add(int a, int b) => a + b;
来源：http://utu.vqdsnc.cn

[C14] 泛型函数
来源：http://zbu.pycfn.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://aor.gaohongyu789.top

PHP:  // 无泛型
来源：http://ghw.sweek.top

JS:   // 无泛型
来源：http://nfu.316326.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rpg.jyoumei.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uun.vqdsnc.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wcy.xingfuxueyuan.xyz

Ruby: # 无泛型
来源：http://bll.ydjk.org.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hcn.c1oappe.top

[C15] 解构 / 展开参数
来源：http://waq.yuanzhike.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fzm.ivvv.top

PHP:  [$a, $b] = $pair;
来源：http://bih.smart0.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zai.tarul.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sog.feifeiyinyue.top

Java: // 无解构
来源：http://jvy.sysykeji.top

Go:   // 无解构
来源：http://gow.daria6918.cn

Ruby: a, b = pair
来源：http://icr.zdbjq.cn

C#:   var (a, b) = pair;
来源：http://ogw.andypj.xyz

[C16] 函数 / 方法重载
来源：http://nbl.ehwqpu.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lam.gotoacloud.top

PHP:  // 无重载
来源：http://wxq.gaohongyu789.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://qiw.cashguo.top

TS:   // 用联合类型或重载签名声明
来源：http://sex.chenzaomai.com

Java: void f(int a) {}  void f(String a) {}
来源：http://yjk.birdmap.top

Go:   // 无重载：用不同函数名
来源：http://fuz.hongshengwenyu.top

Ruby: # 无重载：靠动态参数
来源：http://oik.meibo888.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://rio.zdqjudy.top

================================================================================
来源：http://dtv.jinyuanbaomall.cn

D. 数组 / 列表 / 集合
来源：http://oex.dianchejie.cn

================================================================================
来源：http://msq.zhiwuduotai.top

[D01] 创建数组 / 列表
来源：http://dvo.guannengcc.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://zgz.jianghu66.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dkm.jinghuilouyu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yvn.yj202588.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://gtp.pengpengdd.cyou

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qcg.yvedp.cn

Go:   arr := []int{1, 2, 3}
来源：http://afh.xuetiantiany.cn

Ruby: arr = [1, 2, 3]
来源：http://mlu.tanke756.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tzt.uphjek.com

[D02] 追加元素到末尾
来源：http://rkd.jqgfzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sbh.yuxming.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://snn.xinyue.icu

JS:   arr.push(4);
来源：http://xkb.jinqigfzy.top

TS:   arr.push(4);
来源：http://sbc.feifeiyinyue.top

Java: list.add(4);
来源：http://epw.jyoumei.cn

Go:   arr = append(arr, 4)
来源：http://cpn.shzxlz.cn

Ruby: arr << 4; arr.push(5)
来源：http://cyt.hammf.cn

C#:   list.Add(4);
来源：http://nog.gotoacloud.top

[D03] 在指定位置插入元素
来源：http://glq.jiagoushi.top

Py:   arr.insert(0, 0)
来源：http://zvy.yuxming.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wmf.zhijiandao.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zxj.wangdashe.top

TS:   arr.splice(0, 0, 0);
来源：http://ojp.zhongyouzk.top

Java: list.add(0, 0);
来源：http://uhy.andypj.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://jmp.hysaishi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://akq.jqgfzy.top

C#:   list.Insert(0, 0);
来源：http://ulv.jyoumei.cn

[D04] 删除元素
来源：http://apo.chenzaomai.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uxm.xuanzx.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xss.hysaishi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uwu.hywenlv.cn

TS:   arr.splice(0, 1);
来源：http://dnk.xziqi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jbz.birdmap.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hbo.hnxiangtu.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ptm.jqgfzy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bwg.tarul.cn

[D05] 访问与修改元素
来源：http://gvx.ybcxt.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zvw.andypj.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://imb.hongshengwenyu.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wvx.gaohongyu789.top

TS:   arr[0]; arr.at(-1);
来源：http://ouu.quarkkingdee.top

Java: list.get(0); list.set(0, 9);
来源：http://fmv.cucudq.cn

Go:   arr[0]; arr[0] = 9
来源：http://ruv.hcnkem.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fgp.yfazqb.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://owo.yonumen.top

[D06] 数组长度
来源：http://chg.hnxiangtu.top

Py:   len(arr)
来源：http://fgf.yj20258.top

PHP:  count($arr);
来源：http://ogp.shanyushiyangtech.top

JS:   arr.length
来源：http://huc.jinqigufen.top

TS:   arr.length
来源：http://smf.gotoacloud.top

Java: list.size();
来源：http://tvv.bjfxy.top

Go:   len(arr)
来源：http://byl.xinyue.icu

Ruby: arr.length; arr.size
来源：http://hyi.snrcjt.cn

C#:   list.Count;
来源：http://sib.yuxming.cn

[D07] 切片 / 取子数组
来源：http://tmu.zhongyouzk.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kpj.ivvv.top

PHP:  array_slice($arr, 1, 3);
来源：http://kty.xziqi.cn

JS:   arr.slice(1, 4);
来源：http://xjf.nanxuanxn.top

TS:   arr.slice(1, 4);
来源：http://ovc.ydjk.org.cn

Java: list.subList(1, 4);
来源：http://zoc.wangshuangyany.cn

Go:   arr[1:4]
来源：http://bxj.aibaodan.cn

Ruby: arr[1, 3]
来源：http://ltp.jinqigufen.top

C#:   list.GetRange(1, 3);
来源：http://wdt.yvedp.cn

[D08] 合并两个数组
来源：http://lxx.yangfankeji.com

Py:   a + b;  a.extend(b)
来源：http://vea.nanxinkj.top

PHP:  array_merge($a, $b);
来源：http://tdp.zhiwuduotai.top

JS:   [...a, ...b];  a.concat(b);
来源：http://gyu.bjfxy.top

TS:   [...a, ...b];
来源：http://qkd.meibo888.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kbd.tianlin.xyz

Go:   append(a, b...)
来源：http://lnw.snrcjt.cn

Ruby: a + b;  a.concat(b)
来源：http://cuy.quarkkingdee.top

C#:   a.Concat(b).ToList()
来源：http://pss.shzxlz.cn

[D09] 排序（升序）
来源：http://uhn.feifeiyinyue.top

Py:   sorted(arr);  arr.sort()
来源：http://xjt.yanxiufei.cn

PHP:  sort($arr);
来源：http://ccu.jinqigufen.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tiy.fengsongda.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://syy.bjfxy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://nbp.wangdashe.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dur.havefunace.top

Ruby: arr.sort
来源：http://thl.zhijiandao.cn

C#:   list.Sort();
来源：http://ght.c1oappe.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ort.jqgfzy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://aqk.yj20258.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iov.daria6918.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tsu.aibaodan.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dki.jinqigufen.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://uub.sxryk.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://whe.hnqzz.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dma.bbcook.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://npn.gaohongyu789.top

[D11] 反转数组
来源：http://jad.jinghuilouyu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qoi.wangshuangyany.cn

PHP:  array_reverse($arr);
来源：http://kzb.daria6918.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ean.sweek.top

TS:   [...arr].reverse();
来源：http://omd.jinqigufen.top

Java: Collections.reverse(list);
来源：http://pkh.birdmap.top

Go:   slices.Reverse(arr)
来源：http://jvt.dashuyun.cn

Ruby: arr.reverse
来源：http://eai.cheryme.top

C#:   list.Reverse();
来源：http://ykv.pengpengdd.cyou

[D12] 查找元素下标
来源：http://jop.yj20258.top

Py:   arr.index(x);  x in arr
来源：http://vhi.zhijiandao.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ayb.shanyushiyangtech.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://llt.cashguo.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mke.shanyushiyangtech.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zcw.vehdjk.com

Go:   slices.Index(arr, x)
来源：http://pjq.hywenlv.cn

Ruby: arr.index(x)
来源：http://poq.hysaishi.cn

C#:   list.IndexOf(x);
来源：http://exm.yongpay.top

[D13] 过滤（保留满足条件的）
来源：http://kgn.aizwys.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://iel.fanxiaobao.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ioz.yuxming.cn

JS:   arr.filter(x => x > 3)
来源：http://ibk.xingfuxueyuan.xyz

TS:   arr.filter(x => x > 3)
来源：http://jst.tarul.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://woi.hnxiangtu.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://flx.yongpay.top

Ruby: arr.select { |x| x > 3 }
来源：http://vsq.yanxiufei.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ser.guowangkeji.top

[D14] 映射转换（每个元素变形）
来源：http://vug.fengsongda.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jak.shuidangran.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lht.cqqwz.cn

JS:   arr.map(x => x * 2)
来源：http://idj.yonumen.top

TS:   arr.map(x => x * 2)
来源：http://txl.ybcxt.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://abg.sweek.top

Go:   // 手写循环
来源：http://oct.guannengcc.top

Ruby: arr.map { |x| x * 2 }
来源：http://hhp.aizwys.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://sku.fzhhl.top

[D15] 去重
来源：http://wtn.shangyingyoupin.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yfd.daria6918.cn

PHP:  array_unique($arr);
来源：http://bjj.quarkkingdee.top

JS:   [...new Set(arr)]
来源：http://cmd.zycfv.cn

TS:   [...new Set(arr)]
来源：http://gdh.yonumen.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://czb.xziqi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xnn.smart0.xyz

Ruby: arr.uniq
来源：http://nmh.kuanghao11.cn

C#:   list.Distinct().ToList()
来源：http://bkv.shangyingyoupin.top

[D16] 求和与平均值
来源：http://zau.xziqi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ihe.jianghu66.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cff.zdbjq.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://has.cashguo.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ksc.nanxuanxn.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://twh.havefunace.top

Go:   // 手写循环累加
来源：http://vlg.hnqzz.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ood.dianchejie.cn

C#:   list.Sum();  list.Average()
来源：http://soq.jlsjyb.cn

[D17] 最大值与最小值
来源：http://cym.yj202588.top

Py:   max(arr);  min(arr)
来源：http://tmc.gaohongyu789.top

PHP:  max($arr);  min($arr);
来源：http://los.jianghu66.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mjg.tianlin.xyz

TS:   Math.max(...arr);
来源：http://xas.epnwcf.com

Java: Collections.max(list);  Collections.min(list);
来源：http://erg.yanxiufei.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cqi.aizwys.cn

Ruby: arr.max;  arr.min
来源：http://hzm.xinyue.icu

C#:   list.Max();  list.Min()
来源：http://pvc.yueranfly.top

[D18] 扁平化嵌套数组
来源：http://kpy.zhongyouzk.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yfi.fehbvm.com

PHP:  array_merge(...$nested);
来源：http://jmy.zhaomingkeji.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://faq.xuetiantiany.cn

TS:   nested.flat();
来源：http://niu.0kj1m.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tcw.fzhhl.top

Go:   // 手写双层循环
来源：http://tfp.feifeiyinyue.top

Ruby: nested.flatten
来源：http://ikn.guowangkeji.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://hrj.cdnleiting.top

[D19] 按字段分组
来源：http://ofe.zdbjq.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://biu.sufxvd.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xtu.ybcxt.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rcu.guowangkeji.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ddm.ehwqpu.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://znj.sweek.top

Go:   // 手写 map[string][]T
来源：http://cfk.shangyingyoupin.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://dgm.zhijiandao.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nmr.aibaodan.cn

[D20] 统计每个元素出现次数
来源：http://boz.xingfuxueyuan.xyz

Py:   Counter(arr)
来源：http://nhp.havefunace.top

PHP:  array_count_values($arr);
来源：http://eow.c1oappe.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sop.meibo888.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xtd.xuetiantiany.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://oft.yvedp.cn

Go:   // 手写 map[T]int
来源：http://ibs.chenlongwang.top

Ruby: arr.tally
来源：http://kji.kuanghao11.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cxb.havefunace.top

[D21] 判断是否包含某元素
来源：http://med.daria6918.cn

Py:   x in arr
来源：http://zyq.tarul.cn

PHP:  in_array($x, $arr, true);
来源：http://gek.cashguo.top

JS:   arr.includes(x)
来源：http://otr.fzhhl.top

TS:   arr.includes(x)
来源：http://cwl.sjlbkw.cn

Java: list.contains(x)
来源：http://vmo.wangshuangyany.cn

Go:   slices.Contains(arr, x)
来源：http://uyh.sweek.top

Ruby: arr.include?(x)
来源：http://xif.tarul.cn

C#:   list.Contains(x)
来源：http://frv.ppjwa.cn

[D22] 复制数组（避免共享引用）
来源：http://fhg.epnwcf.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://znf.fzhhl.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://uqm.9152youxi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hlq.shangyingyoupin.top

TS:   [...arr];
来源：http://qfr.ctjpmb.com

Java: new ArrayList<>(list);
来源：http://xvj.sufxvd.cn

Go:   copied := append([]int(nil), arr...)
来源：http://aiu.nanxuanxn.top

Ruby: arr.dup;  arr.clone
来源：http://adk.jinghuilouyu.cn

C#:   new List<int>(list);
来源：http://mus.ppjwa.cn

[D23] reduce 累积计算
来源：http://dbs.yfazqb.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mvv.nanxinkj.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tjr.yuanzhike.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gfm.ydjk.org.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qqy.cheryme.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://dpq.bbcook.cn

Go:   // 手写循环
来源：http://oud.cqqwz.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ryw.zhaomingkeji.xyz


<!-- 参考信息 -->