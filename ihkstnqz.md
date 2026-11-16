代发 wailian999

[C10] 变量作用域
来源：http://jjk.nanxuanxn.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mho.ywan-chungtsiang.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xkj.jyoumei.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nme.shanyushiyangkeji.top

TS:   同 JS
来源：http://jxi.jinyuanbaomall.cn

Java: 方法内为块级作用域
来源：http://tlc.zhongyouzk.top

Go:   花括号块级作用域
来源：http://dlb.yuxming.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mdc.havefunace.top

C#:   块级作用域
来源：http://qyg.yangfankeji.com

[C11] 模块导入与导出
来源：http://ozw.zhixingplan.top

Py:   from module import func
来源：http://gmp.jinqigufen.top

PHP:  require "file.php";  或 use App\Service;
来源：http://nll.snrcjt.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://afg.sweek.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ldc.yongpay.top

Java: import java.util.List;
来源：http://nsg.gzhubu.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://iom.vehdjk.com

Ruby: require "json"; require_relative "./util"
来源：http://dta.zdqjudy.top

C#:   using System.Text;
来源：http://fjd.yfazqb.com

[C12] 立即执行函数 IIFE
来源：http://nju.yj20258888.top

Py:   (lambda: print("run"))()
来源：http://hff.nanxinkj.top

PHP:  (function () { echo "run"; })();
来源：http://vbr.tarul.cn

JS:   (() => { console.log("run"); })();
来源：http://lwe.yuxming.cn

TS:   (() => { console.log("run"); })();
来源：http://sgz.ydjk.org.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qzh.feifeiyinyue.top

Go:   func() { fmt.Println("run") }()
来源：http://lbf.yueranfly.top

Ruby: -> { puts "run" }.call
来源：http://fzh.snrcjt.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://tcf.ehwqpu.com

[C13] 类型声明 / 类型注解
来源：http://tyq.dianchejie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cnk.shanyushiyangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zwi.shanyushiyangkeji.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hfy.yueranfly.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://izt.hywenlv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://pbh.cucudq.cn

Go:   func add(a, b int) int
来源：http://jmr.hesvh.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xbw.jqgfzy.top

C#:   int Add(int a, int b) => a + b;
来源：http://dxv.jinyuanbaomall.cn

[C14] 泛型函数
来源：http://isu.snrcjt.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://eyd.pengpengdd.cyou

PHP:  // 无泛型
来源：http://hon.ehwqpu.com

JS:   // 无泛型
来源：http://gfp.pycfn.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xyf.yonumen.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wul.bjfxy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xxn.sxryk.cn

Ruby: # 无泛型
来源：http://vbi.tarul.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bfq.havefunace.top

[C15] 解构 / 展开参数
来源：http://nbz.hnqzz.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lgk.yuxming.cn

PHP:  [$a, $b] = $pair;
来源：http://dwy.gogol.net.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://idu.xinyue.icu

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nif.xziqi.cn

Java: // 无解构
来源：http://nib.hcnkem.com

Go:   // 无解构
来源：http://vlc.kuanghao11.cn

Ruby: a, b = pair
来源：http://ppl.birdmap.top

C#:   var (a, b) = pair;
来源：http://cvb.shuidangran.top

[C16] 函数 / 方法重载
来源：http://qjp.jiagoushi.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://oal.sjlbkw.cn

PHP:  // 无重载
来源：http://efb.yangfankeji.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://jsc.ehwqpu.com

TS:   // 用联合类型或重载签名声明
来源：http://sky.cucudq.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://sfo.chenzaomai.com

Go:   // 无重载：用不同函数名
来源：http://xmb.epnwcf.com

Ruby: # 无重载：靠动态参数
来源：http://rmg.mhx1999.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://rac.shuidangran.top

================================================================================
来源：http://dqu.hywenlv.cn

D. 数组 / 列表 / 集合
来源：http://ilo.zhixingplan.top

================================================================================
来源：http://sdw.fanxiaobao.xyz

[D01] 创建数组 / 列表
来源：http://qpc.yongpay.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://dsr.yuxming.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jlz.ydjk.org.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wdc.fzhhl.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://yts.gzhubu.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kss.yanxiufei.cn

Go:   arr := []int{1, 2, 3}
来源：http://xbr.iojbl.cn

Ruby: arr = [1, 2, 3]
来源：http://ylh.ywan-chungtsiang.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zvm.sysykeji.top

[D02] 追加元素到末尾
来源：http://fic.tanke756.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://spv.yfazqb.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://otw.yuanzhike.top

JS:   arr.push(4);
来源：http://jcn.pycfn.com

TS:   arr.push(4);
来源：http://ysd.guowangkeji.top

Java: list.add(4);
来源：http://alt.zhijiandao.cn

Go:   arr = append(arr, 4)
来源：http://sqo.guowangkeji.top

Ruby: arr << 4; arr.push(5)
来源：http://jlw.316326.xyz

C#:   list.Add(4);
来源：http://vdd.jinghuilouyu.cn

[D03] 在指定位置插入元素
来源：http://zmv.yuanzhike.top

Py:   arr.insert(0, 0)
来源：http://com.chenlongwang.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cmx.gaohongyu789.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zbz.dashuyun.cn

TS:   arr.splice(0, 0, 0);
来源：http://vlu.hywenlv.cn

Java: list.add(0, 0);
来源：http://jbj.yuanzhike.top

Go:   arr = append([]int{0}, arr...)
来源：http://uah.sysykeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qgk.zdqjudy.top

C#:   list.Insert(0, 0);
来源：http://nbx.jiagoushi.top

[D04] 删除元素
来源：http://mpf.xziqi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://twk.gaohongyu789.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yeo.ydzc1.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uja.cucudq.cn

TS:   arr.splice(0, 1);
来源：http://pwo.guowangkeji.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://scf.jiagoushi.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jjt.aizwys.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://txo.tarul.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mpx.sxryk.cn

[D05] 访问与修改元素
来源：http://kbu.shzxlz.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ymt.smart0.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wrs.yuanzhike.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://boz.jiagoushi.top

TS:   arr[0]; arr.at(-1);
来源：http://ggz.yj20258.top

Java: list.get(0); list.set(0, 9);
来源：http://eks.zhoulong.xyz

Go:   arr[0]; arr[0] = 9
来源：http://lyc.zhengqikj.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nec.52xcode.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ytj.pycfn.com

[D06] 数组长度
来源：http://cip.chenjidiqi.icu

Py:   len(arr)
来源：http://uza.vqdsnc.cn

PHP:  count($arr);
来源：http://sbp.pycfn.com

JS:   arr.length
来源：http://hzs.zhengqikj.top

TS:   arr.length
来源：http://tcs.cashguo.top

Java: list.size();
来源：http://wjt.hnqzz.top

Go:   len(arr)
来源：http://tun.xingfuxueyuan.xyz

Ruby: arr.length; arr.size
来源：http://spu.ydzc1.top

C#:   list.Count;
来源：http://fvd.0kj1m.cn

[D07] 切片 / 取子数组
来源：http://xhv.hysaishi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tgj.shanyushiyangkeji.top

PHP:  array_slice($arr, 1, 3);
来源：http://adw.yuanzhike.top

JS:   arr.slice(1, 4);
来源：http://bec.sjlbkw.cn

TS:   arr.slice(1, 4);
来源：http://uxj.cqqwz.cn

Java: list.subList(1, 4);
来源：http://bid.ppjwa.cn

Go:   arr[1:4]
来源：http://cac.shanyushiyangtech.top

Ruby: arr[1, 3]
来源：http://wou.ydzc1.top

C#:   list.GetRange(1, 3);
来源：http://qeg.zdbjq.cn

[D08] 合并两个数组
来源：http://kog.sjlbkw.cn

Py:   a + b;  a.extend(b)
来源：http://ifs.wangshuangyany.cn

PHP:  array_merge($a, $b);
来源：http://hpr.yj20258888.top

JS:   [...a, ...b];  a.concat(b);
来源：http://txh.shzxlz.cn

TS:   [...a, ...b];
来源：http://pwc.zhaomingkeji.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zrr.ydzc1.top

Go:   append(a, b...)
来源：http://kfj.yj20258888.top

Ruby: a + b;  a.concat(b)
来源：http://btf.bjfxy.top

C#:   a.Concat(b).ToList()
来源：http://rhr.xingfuxueyuan.xyz

[D09] 排序（升序）
来源：http://xlf.vqdsnc.cn

Py:   sorted(arr);  arr.sort()
来源：http://box.gaohongyu789.top

PHP:  sort($arr);
来源：http://gkt.ywan-chungtsiang.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pdb.fktsv.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://slw.wangdashe.top

Java: Collections.sort(list);  list.sort(null);
来源：http://hkk.mhx1999.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vkq.xingfuxueyuan.xyz

Ruby: arr.sort
来源：http://odj.zhiwuduotai.top

C#:   list.Sort();
来源：http://ova.guowangkeji.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://rsp.vqdsnc.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wmd.fktsv.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gij.zhixingplan.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gvh.wangdashe.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://uuc.hnxiangtu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lpp.shzxlz.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rvy.zdbjq.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sdn.yfazqb.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ulp.xuetiantiany.cn

[D11] 反转数组
来源：http://pkd.chenzaomai.com

Py:   arr[::-1];  arr.reverse()
来源：http://qri.xuetiantiany.cn

PHP:  array_reverse($arr);
来源：http://ivd.pycfn.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://joy.haohaochexian.top

TS:   [...arr].reverse();
来源：http://iab.shangyingyoupin.top

Java: Collections.reverse(list);
来源：http://vuw.yj202588.top

Go:   slices.Reverse(arr)
来源：http://nbj.shanyushiyangtech.top

Ruby: arr.reverse
来源：http://gwf.yueranfly.top

C#:   list.Reverse();
来源：http://pan.zycfv.cn

[D12] 查找元素下标
来源：http://oon.0kj1m.cn

Py:   arr.index(x);  x in arr
来源：http://edl.hongshengwenyu.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kay.chenlongwang.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sbv.52xcode.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gka.ehwqpu.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://crp.daria6918.cn

Go:   slices.Index(arr, x)
来源：http://zgl.redwolf501.top

Ruby: arr.index(x)
来源：http://dnk.jinqigfzy.top

C#:   list.IndexOf(x);
来源：http://oce.ctjpmb.com

[D13] 过滤（保留满足条件的）
来源：http://bss.cashguo.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ipz.cqqwz.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dfi.yj20258888.top

JS:   arr.filter(x => x > 3)
来源：http://phq.gaohongyu789.top

TS:   arr.filter(x => x > 3)
来源：http://ttk.fktsv.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qhk.tian-w.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nop.redwolf501.top

Ruby: arr.select { |x| x > 3 }
来源：http://ehk.daxiang520.top

C#:   list.Where(x => x > 3).ToList()
来源：http://vzf.nwbrower.top

[D14] 映射转换（每个元素变形）
来源：http://nzu.xinyue.icu

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ptu.guannengcc.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wit.zhijiandao.cn

JS:   arr.map(x => x * 2)
来源：http://uqx.shanyushiyangkeji.top

TS:   arr.map(x => x * 2)
来源：http://lhk.sysykeji.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ahh.cdnleiting.top

Go:   // 手写循环
来源：http://jbb.birdmap.top

Ruby: arr.map { |x| x * 2 }
来源：http://ulm.jlsjyb.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://uxr.hesvh.cn

[D15] 去重
来源：http://cbp.hnqzz.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yxi.tianlin.xyz

PHP:  array_unique($arr);
来源：http://baj.chenzaomai.com

JS:   [...new Set(arr)]
来源：http://gce.cqqwz.cn

TS:   [...new Set(arr)]
来源：http://zzs.yvedp.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cov.hnqzz.top

Go:   // 用 map[T]struct{} 手写
来源：http://gry.bbcook.cn

Ruby: arr.uniq
来源：http://fzx.sysykeji.top

C#:   list.Distinct().ToList()
来源：http://rrc.tanke756.top

[D16] 求和与平均值
来源：http://kwz.jyoumei.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gma.jinqigufen.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mfa.zhijiandao.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cdt.jinqigfzy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pki.chenlongwang.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cdr.hcnkem.com

Go:   // 手写循环累加
来源：http://jqj.feifeiyinyue.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tqc.zhaomingkeji.xyz

C#:   list.Sum();  list.Average()
来源：http://klg.jinqigfzy.top

[D17] 最大值与最小值
来源：http://wxe.ctjpmb.com

Py:   max(arr);  min(arr)
来源：http://dhp.fktsv.cn

PHP:  max($arr);  min($arr);
来源：http://ujp.jinyuanbaomall.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://esq.zycfv.cn

TS:   Math.max(...arr);
来源：http://seh.yongpay.top

Java: Collections.max(list);  Collections.min(list);
来源：http://lgb.yuanzhike.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://aen.feifeiyinyue.top

Ruby: arr.max;  arr.min
来源：http://efl.sufxvd.cn

C#:   list.Max();  list.Min()
来源：http://hgs.daria6918.cn

[D18] 扁平化嵌套数组
来源：http://qzy.iojbl.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://krc.quarkkingdee.top

PHP:  array_merge(...$nested);
来源：http://fga.zhoulong.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bao.sjlbkw.cn

TS:   nested.flat();
来源：http://nxa.sweek.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dvq.xuanzx.com

Go:   // 手写双层循环
来源：http://myd.hywenlv.cn

Ruby: nested.flatten
来源：http://xsl.dianchejie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://rwc.jinqigfzy.top

[D19] 按字段分组
来源：http://jlv.jyoumei.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fwo.wangshuangyany.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jyh.dashuyun.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lgz.sysykeji.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://xkw.bbcook.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fll.yvedp.cn

Go:   // 手写 map[string][]T
来源：http://wiz.yj20258.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://dpl.hcnkem.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rrr.nanxinkj.top

[D20] 统计每个元素出现次数
来源：http://lmt.hysaishi.cn

Py:   Counter(arr)
来源：http://bmv.fehbvm.com

PHP:  array_count_values($arr);
来源：http://jfd.jianghu66.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vbo.gaohongyu789.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bvg.birdmap.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cxa.jlsjyb.cn

Go:   // 手写 map[T]int
来源：http://tvb.fengsongda.top

Ruby: arr.tally
来源：http://upl.gaohongyu789.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tto.ppjwa.cn

[D21] 判断是否包含某元素
来源：http://yhx.xziqi.cn

Py:   x in arr
来源：http://imp.quarkkingdee.top

PHP:  in_array($x, $arr, true);
来源：http://rsr.gogol.net.cn

JS:   arr.includes(x)
来源：http://stc.xuanzx.com

TS:   arr.includes(x)
来源：http://wss.cashguo.top

Java: list.contains(x)
来源：http://oet.dianchejie.cn

Go:   slices.Contains(arr, x)
来源：http://jde.jinyuanbaomall.cn

Ruby: arr.include?(x)
来源：http://ysk.dianchejie.cn

C#:   list.Contains(x)
来源：http://uws.shanyushiyangtech.top

[D22] 复制数组（避免共享引用）
来源：http://wrs.cashguo.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dxn.snrcjt.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ddw.quarkkingdee.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nkm.iojbl.cn

TS:   [...arr];
来源：http://zqn.jqgfzy.top

Java: new ArrayList<>(list);
来源：http://nsp.yueranfly.top

Go:   copied := append([]int(nil), arr...)
来源：http://kmj.hnqzz.top

Ruby: arr.dup;  arr.clone
来源：http://tcl.jianghu66.top

C#:   new List<int>(list);
来源：http://zgr.haohaochexian.top

[D23] reduce 累积计算
来源：http://tru.fktsv.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://uzd.xuetiantiany.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ebv.hongshengwenyu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dsy.yangfankeji.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hkb.hcnkem.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://fxo.zhengqikj.top

Go:   // 手写循环
来源：http://cdj.cucudq.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rjd.shuidangran.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ihj.jqgufenzy.top

[D24] 字典 / Map 基本操作
来源：http://qhy.316326.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ldz.dashuyun.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://iud.snrcjt.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rgd.yvedp.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://okk.smart0.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ywl.kuanghao11.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mcd.vehdjk.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cur.pycfn.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cak.jiagoushi.top

[D25] Set 集合去重与交并差
来源：http://aog.haohaochexian.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://poq.jyoumei.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ioh.tianlin.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zji.yongpay.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://byw.chenzaomai.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ily.shangyingyoupin.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wai.ydzc1.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cjx.yj202588.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nzh.guannengcc.top

[D26] 数组转字符串
来源：http://pva.zdbjq.cn

Py:   ", ".join(map(str, arr))
来源：http://fcv.yonumen.top

PHP:  implode(", ", $arr);
来源：http://lqu.haohaochexian.top

JS:   arr.join(", ")
来源：http://lkc.chenzaomai.com

TS:   arr.join(", ")
来源：http://jmq.iojbl.cn

Java: String.join(", ", list)
来源：http://otg.jqgufenzy.top

Go:   strings.Join(strs, ", ")
来源：http://yen.pengpengdd.cyou

Ruby: arr.join(", ")
来源：http://mop.jyoumei.cn

C#:   string.Join(", ", list)
来源：http://vkz.uphjek.com


<!-- 参考信息 -->