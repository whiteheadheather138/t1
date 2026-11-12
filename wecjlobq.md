代发 wailian999

C#:   块级作用域
来源：http://lzr.tian-w.cn

[C11] 模块导入与导出
来源：http://voa.guowangkeji.top

Py:   from module import func
来源：http://kdo.cashguo.top

PHP:  require "file.php";  或 use App\Service;
来源：http://tka.vqdsnc.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://cze.cdnleiting.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://iok.shzxlz.cn

Java: import java.util.List;
来源：http://rdi.cdnleiting.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ags.vehdjk.com

Ruby: require "json"; require_relative "./util"
来源：http://rdm.fanxiaobao.xyz

C#:   using System.Text;
来源：http://sqg.jyoumei.cn

[C12] 立即执行函数 IIFE
来源：http://yfr.quarkkingdee.top

Py:   (lambda: print("run"))()
来源：http://frj.zhaomingkeji.xyz

PHP:  (function () { echo "run"; })();
来源：http://umo.sjlbkw.cn

JS:   (() => { console.log("run"); })();
来源：http://nld.hcnkem.com

TS:   (() => { console.log("run"); })();
来源：http://kcr.guowangkeji.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ffg.vehdjk.com

Go:   func() { fmt.Println("run") }()
来源：http://gdg.52xcode.cn

Ruby: -> { puts "run" }.call
来源：http://lvg.hywenlv.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://oim.yfazqb.com

[C13] 类型声明 / 类型注解
来源：http://oun.yvedp.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kem.andypj.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qew.xylfe.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://uxr.tanke756.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gsj.andypj.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://dgx.bjfxy.top

Go:   func add(a, b int) int
来源：http://nkl.jqgufenzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fti.jinqigfzy.top

C#:   int Add(int a, int b) => a + b;
来源：http://hfd.cdnleiting.top

[C14] 泛型函数
来源：http://vcf.zhengqikj.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ujv.xuetiantiany.cn

PHP:  // 无泛型
来源：http://adm.cashguo.top

JS:   // 无泛型
来源：http://fjf.chenzaomai.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qty.daxiang520.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yiw.quarkkingdee.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://znn.xuanzx.com

Ruby: # 无泛型
来源：http://brq.yanxiufei.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://omd.zhongyouzk.top

[C15] 解构 / 展开参数
来源：http://hqz.jqgufenzy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bes.hnxiangtu.top

PHP:  [$a, $b] = $pair;
来源：http://stz.vehdjk.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rst.yj20258888.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ody.svipenyu.cn

Java: // 无解构
来源：http://ycj.tanke756.top

Go:   // 无解构
来源：http://vug.bbcook.cn

Ruby: a, b = pair
来源：http://rof.feifeiyinyue.top

C#:   var (a, b) = pair;
来源：http://pzz.xuetiantiany.cn

[C16] 函数 / 方法重载
来源：http://jvy.xziqi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pyp.fktsv.cn

PHP:  // 无重载
来源：http://hne.dianchejie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://iya.gaohongyu789.top

TS:   // 用联合类型或重载签名声明
来源：http://ghj.fanxiaobao.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://rea.pycfn.com

Go:   // 无重载：用不同函数名
来源：http://aof.fzhhl.top

Ruby: # 无重载：靠动态参数
来源：http://upr.yanxiufei.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://byz.xziqi.cn

================================================================================
来源：http://dwt.daria6918.cn

D. 数组 / 列表 / 集合
来源：http://rar.dashuyun.cn

================================================================================
来源：http://hds.aibaodan.cn

[D01] 创建数组 / 列表
来源：http://rya.shanyushiyangkeji.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://rso.shanyushiyangkeji.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://aks.jqgufenzy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ojx.chenzaomai.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://frj.havefunace.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mko.feifeiyinyue.top

Go:   arr := []int{1, 2, 3}
来源：http://eny.bjfxy.top

Ruby: arr = [1, 2, 3]
来源：http://mcw.wangdashe.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yca.feifeiyinyue.top

[D02] 追加元素到末尾
来源：http://vas.kuanghao11.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://woz.yuanzhike.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blc.fehbvm.com

JS:   arr.push(4);
来源：http://bpl.cheryme.top

TS:   arr.push(4);
来源：http://dac.iojbl.cn

Java: list.add(4);
来源：http://cuw.hfpthk.cn

Go:   arr = append(arr, 4)
来源：http://dxn.jianghu66.top

Ruby: arr << 4; arr.push(5)
来源：http://qwt.shuidangran.top

C#:   list.Add(4);
来源：http://azj.aibaodan.cn

[D03] 在指定位置插入元素
来源：http://dav.jinyuanbaomall.cn

Py:   arr.insert(0, 0)
来源：http://zti.fzhhl.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://oha.sufxvd.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nwr.feifeiyinyue.top

TS:   arr.splice(0, 0, 0);
来源：http://vgx.pengpengdd.cyou

Java: list.add(0, 0);
来源：http://mkt.wangdashe.top

Go:   arr = append([]int{0}, arr...)
来源：http://cxk.ivvv.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ljo.ydzc1.top

C#:   list.Insert(0, 0);
来源：http://hva.tian-w.cn

[D04] 删除元素
来源：http://api.dianchejie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://szo.sysykeji.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jfl.hfpthk.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vze.sjlbkw.cn

TS:   arr.splice(0, 1);
来源：http://fhz.zdbjq.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://paj.jlsjyb.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xob.ehwqpu.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mzx.gaohongyu789.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dtp.tarul.cn

[D05] 访问与修改元素
来源：http://pzd.zdbjq.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wwc.zhijiandao.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yyq.jiagoushi.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lgw.dashuyun.cn

TS:   arr[0]; arr.at(-1);
来源：http://wmy.yvedp.cn

Java: list.get(0); list.set(0, 9);
来源：http://itt.chenlongwang.top

Go:   arr[0]; arr[0] = 9
来源：http://bcg.kuanghao11.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xoo.xuanzx.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://brd.yonumen.top

[D06] 数组长度
来源：http://srv.zhengqikj.top

Py:   len(arr)
来源：http://jbr.zycfv.cn

PHP:  count($arr);
来源：http://krd.ctjpmb.com

JS:   arr.length
来源：http://ybs.9152youxi.cn

TS:   arr.length
来源：http://lxp.fehbvm.com

Java: list.size();
来源：http://eme.hcnkem.com

Go:   len(arr)
来源：http://brf.hongshengwenyu.top

Ruby: arr.length; arr.size
来源：http://rrw.ehwqpu.com

C#:   list.Count;
来源：http://dkb.zhengqikj.top

[D07] 切片 / 取子数组
来源：http://fwr.aibaodan.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://joc.guannengcc.top

PHP:  array_slice($arr, 1, 3);
来源：http://xdh.fktsv.cn

JS:   arr.slice(1, 4);
来源：http://mcj.sufxvd.cn

TS:   arr.slice(1, 4);
来源：http://xhi.dashuyun.cn

Java: list.subList(1, 4);
来源：http://gaa.yvedp.cn

Go:   arr[1:4]
来源：http://coc.tianlin.xyz

Ruby: arr[1, 3]
来源：http://nvf.zhiwuduotai.top

C#:   list.GetRange(1, 3);
来源：http://kjo.xuanzx.com

[D08] 合并两个数组
来源：http://odj.ydjk.org.cn

Py:   a + b;  a.extend(b)
来源：http://sjf.cashguo.top

PHP:  array_merge($a, $b);
来源：http://iab.fehbvm.com

JS:   [...a, ...b];  a.concat(b);
来源：http://jhi.wangdashe.top

TS:   [...a, ...b];
来源：http://fbb.316326.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mam.xziqi.cn

Go:   append(a, b...)
来源：http://olo.zdbjq.cn

Ruby: a + b;  a.concat(b)
来源：http://eaa.xinyue.icu

C#:   a.Concat(b).ToList()
来源：http://cgq.ehwqpu.com

[D09] 排序（升序）
来源：http://axz.chenzaomai.com

Py:   sorted(arr);  arr.sort()
来源：http://yim.epnwcf.com

PHP:  sort($arr);
来源：http://uqh.316326.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://crr.zhengqikj.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://uns.kuanghao11.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://uxs.hfpthk.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pjh.hcnkem.com

Ruby: arr.sort
来源：http://gou.tianlin.xyz

C#:   list.Sort();
来源：http://xcd.mhx1999.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://dzv.hcnkem.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bjs.zhixingplan.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dvd.quarkkingdee.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vsc.zhiwuduotai.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://avy.aizwys.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ioa.jianghu66.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bxj.shuidangran.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://iiy.jqgufenzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://svv.hnxiangtu.top

[D11] 反转数组
来源：http://ilg.zhijiandao.cn

Py:   arr[::-1];  arr.reverse()
来源：http://hvl.jinghuilouyu.cn

PHP:  array_reverse($arr);
来源：http://tnm.yj202588.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vvz.xylfe.cn

TS:   [...arr].reverse();
来源：http://qtg.xinyue.icu

Java: Collections.reverse(list);
来源：http://ffw.9152youxi.cn

Go:   slices.Reverse(arr)
来源：http://lxz.nwbrower.top

Ruby: arr.reverse
来源：http://uth.quarkkingdee.top

C#:   list.Reverse();
来源：http://qzt.andypj.xyz

[D12] 查找元素下标
来源：http://zia.aizwys.cn

Py:   arr.index(x);  x in arr
来源：http://ouj.xuetiantiany.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vla.sysykeji.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sxo.xinyue.icu

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hji.jinyuanbaomall.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://czc.52xcode.cn

Go:   slices.Index(arr, x)
来源：http://zva.fehbvm.com

Ruby: arr.index(x)
来源：http://ale.hammf.cn

C#:   list.IndexOf(x);
来源：http://tdn.nanxinkj.top

[D13] 过滤（保留满足条件的）
来源：http://xka.kuanghao11.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vwt.zhongyouzk.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mtf.jiagoushi.top

JS:   arr.filter(x => x > 3)
来源：http://cmj.aizwys.cn

TS:   arr.filter(x => x > 3)
来源：http://kaq.snrcjt.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://amo.jinqigfzy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://syg.wangshuangyany.cn

Ruby: arr.select { |x| x > 3 }
来源：http://pnk.dianchejie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://zfz.jinyuanbaomall.cn

[D14] 映射转换（每个元素变形）
来源：http://wft.shanyushiyangtech.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fbx.guowangkeji.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://eig.xziqi.cn

JS:   arr.map(x => x * 2)
来源：http://tkm.yj202588.top

TS:   arr.map(x => x * 2)
来源：http://zrf.bjfxy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://zrv.cashguo.top

Go:   // 手写循环
来源：http://fta.hammf.cn

Ruby: arr.map { |x| x * 2 }
来源：http://imi.uphjek.com

C#:   list.Select(x => x * 2).ToList()
来源：http://frg.cqqwz.cn

[D15] 去重
来源：http://hav.zhiwuduotai.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ylr.quarkkingdee.top

PHP:  array_unique($arr);
来源：http://osv.zhiwuduotai.top

JS:   [...new Set(arr)]
来源：http://ivk.sysykeji.top

TS:   [...new Set(arr)]
来源：http://ktp.xinyue.icu

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://syt.ppjwa.cn

Go:   // 用 map[T]struct{} 手写
来源：http://kwh.zhoulong.xyz

Ruby: arr.uniq
来源：http://zai.quarkkingdee.top

C#:   list.Distinct().ToList()
来源：http://rln.mhx1999.top

[D16] 求和与平均值
来源：http://mrq.gotoacloud.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hhl.chenjidiqi.icu

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fxt.redwolf501.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wlm.hcnkem.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ixp.xingfuxueyuan.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xtc.mhx1999.top

Go:   // 手写循环累加
来源：http://urh.hongshengwenyu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yei.jinqigfzy.top

C#:   list.Sum();  list.Average()
来源：http://uwy.ehwqpu.com

[D17] 最大值与最小值
来源：http://buj.feifeiyinyue.top

Py:   max(arr);  min(arr)
来源：http://izz.mhx1999.top

PHP:  max($arr);  min($arr);
来源：http://vfo.redwolf501.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zvo.vehdjk.com

TS:   Math.max(...arr);
来源：http://fmh.xziqi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://swn.nwbrower.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rig.hesvh.cn

Ruby: arr.max;  arr.min
来源：http://ifj.chenjidiqi.icu

C#:   list.Max();  list.Min()
来源：http://fjg.cqqwz.cn

[D18] 扁平化嵌套数组
来源：http://qip.yuanzhike.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://aee.ehwqpu.com

PHP:  array_merge(...$nested);
来源：http://ljn.zhoulong.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sns.bbcook.cn

TS:   nested.flat();
来源：http://yog.ctjpmb.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qvx.zhiwuduotai.top

Go:   // 手写双层循环
来源：http://zwz.cucudq.cn

Ruby: nested.flatten
来源：http://hrd.shangyingyoupin.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://zme.ppjwa.cn

[D19] 按字段分组
来源：http://uxx.svipenyu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://btv.xziqi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hnh.xuanzx.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://oxb.hesvh.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ozx.aibaodan.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lpw.pengpengdd.cyou

Go:   // 手写 map[string][]T
来源：http://ngo.daria6918.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://wnm.bjfxy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ptl.hammf.cn

[D20] 统计每个元素出现次数
来源：http://hlt.hongshengwenyu.top

Py:   Counter(arr)
来源：http://cyq.bjfxy.top

PHP:  array_count_values($arr);
来源：http://pof.wangshuangyany.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ymq.ywan-chungtsiang.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lgp.c1oappe.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://raa.hammf.cn

Go:   // 手写 map[T]int
来源：http://saf.xylfe.cn

Ruby: arr.tally
来源：http://spo.meibo888.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ggr.ctjpmb.com

[D21] 判断是否包含某元素
来源：http://pxg.sjlbkw.cn

Py:   x in arr
来源：http://yye.meibo888.top

PHP:  in_array($x, $arr, true);
来源：http://ayd.zhiwuduotai.top

JS:   arr.includes(x)
来源：http://xte.fehbvm.com

TS:   arr.includes(x)
来源：http://rbz.yj20258.top

Java: list.contains(x)
来源：http://bvo.fzhhl.top

Go:   slices.Contains(arr, x)
来源：http://moe.jianghu66.top

Ruby: arr.include?(x)
来源：http://nkg.haohaochexian.top

C#:   list.Contains(x)
来源：http://stc.andypj.xyz

[D22] 复制数组（避免共享引用）
来源：http://iiq.gzhubu.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://uqf.fengsongda.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yth.iojbl.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lud.yuanzhike.top

TS:   [...arr];
来源：http://lpt.sysykeji.top

Java: new ArrayList<>(list);
来源：http://qmw.kuanghao11.cn

Go:   copied := append([]int(nil), arr...)
来源：http://uba.sxryk.cn

Ruby: arr.dup;  arr.clone
来源：http://xba.yongpay.top

C#:   new List<int>(list);
来源：http://zzh.ehwqpu.com

[D23] reduce 累积计算
来源：http://mhf.zdqjudy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ppl.gaohongyu789.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://drs.sufxvd.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gov.hnxiangtu.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vob.fengsongda.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://nql.yj202588.top

Go:   // 手写循环
来源：http://non.sjlbkw.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ojf.tarul.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gdr.yj20258.top

[D24] 字典 / Map 基本操作
来源：http://uya.yanxiufei.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tui.shzxlz.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ffw.yj202588.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hny.zhijiandao.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sdp.havefunace.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ohu.pengpengdd.cyou

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yyg.kuanghao11.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hcv.sjlbkw.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://val.cashguo.top

[D25] Set 集合去重与交并差
来源：http://vax.xuetiantiany.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ywg.cqqwz.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qwi.gzhubu.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://otu.316326.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://oab.tianlin.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xwx.zhengqikj.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ngz.daria6918.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jgi.smart0.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wiz.shangyingyoupin.top

[D26] 数组转字符串
来源：http://msh.mhx1999.top

Py:   ", ".join(map(str, arr))
来源：http://ixs.haohaochexian.top

PHP:  implode(", ", $arr);
来源：http://fdi.pengpengdd.cyou

JS:   arr.join(", ")
来源：http://zay.cucudq.cn

TS:   arr.join(", ")
来源：http://xxw.jqgufenzy.top

Java: String.join(", ", list)
来源：http://qyh.nanxinkj.top

Go:   strings.Join(strs, ", ")
来源：http://tll.gaohongyu789.top

Ruby: arr.join(", ")
来源：http://yvr.shuidangran.top

C#:   string.Join(", ", list)
来源：http://vgs.zhiwuduotai.top

================================================================================
来源：http://xmi.xylfe.cn

E. 字符串处理
来源：http://wvh.yj20258888.top

================================================================================
来源：http://zwe.shangyingyoupin.top

[E01] 拼接字符串
来源：http://fek.smart0.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yrl.wangshuangyany.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://phj.vqdsnc.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kzf.cucudq.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://utx.c1oappe.top


<!-- 参考信息 -->