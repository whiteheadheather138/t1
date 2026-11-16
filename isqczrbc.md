代发 wailian999

[C10] 变量作用域
来源：http://ivs.bjfxy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nah.c1oappe.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ayr.52xcode.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ubg.tianlin.xyz

TS:   同 JS
来源：http://emd.cheryme.top

Java: 方法内为块级作用域
来源：http://eyq.yanxiufei.cn

Go:   花括号块级作用域
来源：http://gnv.cqqwz.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://iib.0kj1m.cn

C#:   块级作用域
来源：http://lvc.svipenyu.cn

[C11] 模块导入与导出
来源：http://zyv.ybcxt.top

Py:   from module import func
来源：http://lsp.hysaishi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://vhc.fanxiaobao.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://czx.fktsv.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ots.epnwcf.com

Java: import java.util.List;
来源：http://ydn.uphjek.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baj.daxiang520.top

Ruby: require "json"; require_relative "./util"
来源：http://esm.cheryme.top

C#:   using System.Text;
来源：http://htj.52xcode.cn

[C12] 立即执行函数 IIFE
来源：http://ely.ehwqpu.com

Py:   (lambda: print("run"))()
来源：http://xdx.hfpthk.cn

PHP:  (function () { echo "run"; })();
来源：http://izm.shanyushiyangkeji.top

JS:   (() => { console.log("run"); })();
来源：http://ccl.quarkkingdee.top

TS:   (() => { console.log("run"); })();
来源：http://kwn.yangfankeji.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://arg.shzxlz.cn

Go:   func() { fmt.Println("run") }()
来源：http://ctq.tarul.cn

Ruby: -> { puts "run" }.call
来源：http://bcj.yuanzhike.top

C#:   // 无 IIFE：用静态构造函数
来源：http://htn.zhoulong.xyz

[C13] 类型声明 / 类型注解
来源：http://ppa.fengsongda.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xra.jlsjyb.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mfj.cqqwz.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rqt.zhijiandao.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ejr.fengsongda.top

Java: int add(int a, int b) { return a + b; }
来源：http://hzp.jlsjyb.cn

Go:   func add(a, b int) int
来源：http://htv.yfazqb.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tgt.316326.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://cvg.ehwqpu.com

[C14] 泛型函数
来源：http://kjz.yanxiufei.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kfu.jiagoushi.top

PHP:  // 无泛型
来源：http://isc.xuetiantiany.cn

JS:   // 无泛型
来源：http://btw.yongpay.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ieo.shanyushiyangkeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nmh.hfpthk.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jkk.chenzaomai.com

Ruby: # 无泛型
来源：http://bsw.zhixingplan.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://eqz.cucudq.cn

[C15] 解构 / 展开参数
来源：http://spe.yuxming.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vod.hnqzz.top

PHP:  [$a, $b] = $pair;
来源：http://sjr.nwbrower.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ypg.fengsongda.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nhq.hcnkem.com

Java: // 无解构
来源：http://tbg.gotoacloud.top

Go:   // 无解构
来源：http://luc.yanxiufei.cn

Ruby: a, b = pair
来源：http://plb.9152youxi.cn

C#:   var (a, b) = pair;
来源：http://vcj.mhx1999.top

[C16] 函数 / 方法重载
来源：http://rab.316326.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gds.zhixingplan.top

PHP:  // 无重载
来源：http://lgo.yj20258888.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://bub.jqgufenzy.top

TS:   // 用联合类型或重载签名声明
来源：http://upk.yongpay.top

Java: void f(int a) {}  void f(String a) {}
来源：http://qzi.daxiang520.top

Go:   // 无重载：用不同函数名
来源：http://bli.jianghu66.top

Ruby: # 无重载：靠动态参数
来源：http://xro.epnwcf.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://hrq.yuxming.cn

================================================================================
来源：http://gnr.hnxiangtu.top

D. 数组 / 列表 / 集合
来源：http://gzn.zhongyouzk.top

================================================================================
来源：http://ggn.yanxiufei.cn

[D01] 创建数组 / 列表
来源：http://ezx.yangfankeji.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://bxg.jinghuilouyu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zhg.yfazqb.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://azb.fzhhl.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://zdt.wangshuangyany.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://adf.yongpay.top

Go:   arr := []int{1, 2, 3}
来源：http://rgw.ivvv.top

Ruby: arr = [1, 2, 3]
来源：http://gvt.birdmap.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://byd.redwolf501.top

[D02] 追加元素到末尾
来源：http://dgh.hnqzz.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jfb.xinyue.icu

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rkr.guowangkeji.top

JS:   arr.push(4);
来源：http://zci.nwbrower.top

TS:   arr.push(4);
来源：http://nzh.daria6918.cn

Java: list.add(4);
来源：http://wyu.yfazqb.com

Go:   arr = append(arr, 4)
来源：http://drn.guowangkeji.top

Ruby: arr << 4; arr.push(5)
来源：http://ipp.hongshengwenyu.top

C#:   list.Add(4);
来源：http://lbg.yuanzhike.top

[D03] 在指定位置插入元素
来源：http://sct.zdqjudy.top

Py:   arr.insert(0, 0)
来源：http://ytb.aizwys.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zza.wangshuangyany.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hed.birdmap.top

TS:   arr.splice(0, 0, 0);
来源：http://new.cheryme.top

Java: list.add(0, 0);
来源：http://lzq.haohaochexian.top

Go:   arr = append([]int{0}, arr...)
来源：http://vbz.andypj.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://utp.hnqzz.top

C#:   list.Insert(0, 0);
来源：http://ryz.kuanghao11.cn

[D04] 删除元素
来源：http://cps.guannengcc.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uzv.chenzaomai.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uts.yongpay.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fvg.meibo888.top

TS:   arr.splice(0, 1);
来源：http://hlz.fzhhl.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://iga.zhengqikj.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cse.ivvv.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ebr.ybcxt.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fim.xingfuxueyuan.xyz

[D05] 访问与修改元素
来源：http://guw.quarkkingdee.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pbr.chenzaomai.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://eds.0kj1m.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hwx.shanyushiyangkeji.top

TS:   arr[0]; arr.at(-1);
来源：http://ynz.hcnkem.com

Java: list.get(0); list.set(0, 9);
来源：http://cfx.quarkkingdee.top

Go:   arr[0]; arr[0] = 9
来源：http://tsg.hnqzz.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gkr.yj20258888.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nvl.daxiang520.top

[D06] 数组长度
来源：http://tft.birdmap.top

Py:   len(arr)
来源：http://lro.tanke756.top

PHP:  count($arr);
来源：http://hyx.xziqi.cn

JS:   arr.length
来源：http://dul.xinyue.icu

TS:   arr.length
来源：http://xdd.xuetiantiany.cn

Java: list.size();
来源：http://nka.0kj1m.cn

Go:   len(arr)
来源：http://xki.fktsv.cn

Ruby: arr.length; arr.size
来源：http://php.hongshengwenyu.top

C#:   list.Count;
来源：http://cxy.ctjpmb.com

[D07] 切片 / 取子数组
来源：http://nmk.ppjwa.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nuj.feifeiyinyue.top

PHP:  array_slice($arr, 1, 3);
来源：http://gij.yueranfly.top

JS:   arr.slice(1, 4);
来源：http://zhb.52xcode.cn

TS:   arr.slice(1, 4);
来源：http://zju.havefunace.top

Java: list.subList(1, 4);
来源：http://veg.smart0.xyz

Go:   arr[1:4]
来源：http://qgv.yj202588.top

Ruby: arr[1, 3]
来源：http://tri.uphjek.com

C#:   list.GetRange(1, 3);
来源：http://ilv.hysaishi.cn

[D08] 合并两个数组
来源：http://fiy.ctjpmb.com

Py:   a + b;  a.extend(b)
来源：http://woq.vqdsnc.cn

PHP:  array_merge($a, $b);
来源：http://xev.ybcxt.top

JS:   [...a, ...b];  a.concat(b);
来源：http://mhw.yueranfly.top

TS:   [...a, ...b];
来源：http://enw.cqqwz.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nzr.jinghuilouyu.cn

Go:   append(a, b...)
来源：http://ejz.redwolf501.top

Ruby: a + b;  a.concat(b)
来源：http://kvy.chenjidiqi.icu

C#:   a.Concat(b).ToList()
来源：http://zmx.zhongyouzk.top

[D09] 排序（升序）
来源：http://lio.jinghuilouyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://pno.tianlin.xyz

PHP:  sort($arr);
来源：http://vvo.yj202588.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bey.shuidangran.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://tpr.tarul.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://sxw.9152youxi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://aff.sweek.top

Ruby: arr.sort
来源：http://jcz.hywenlv.cn

C#:   list.Sort();
来源：http://gyz.chenzaomai.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://jbf.jinyuanbaomall.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uph.tianlin.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rle.nwbrower.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ivg.cdnleiting.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xnj.redwolf501.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vsi.xingfuxueyuan.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rvk.fengsongda.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wjb.yfazqb.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ant.sweek.top

[D11] 反转数组
来源：http://mfa.0kj1m.cn

Py:   arr[::-1];  arr.reverse()
来源：http://snx.52xcode.cn

PHP:  array_reverse($arr);
来源：http://hzz.guannengcc.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://com.ehwqpu.com

TS:   [...arr].reverse();
来源：http://vid.zhengqikj.top

Java: Collections.reverse(list);
来源：http://lgh.tarul.cn

Go:   slices.Reverse(arr)
来源：http://mgj.jinqigufen.top

Ruby: arr.reverse
来源：http://wur.vehdjk.com

C#:   list.Reverse();
来源：http://ypn.iojbl.cn

[D12] 查找元素下标
来源：http://yby.yfazqb.com

Py:   arr.index(x);  x in arr
来源：http://nux.quarkkingdee.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tjm.tarul.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://saw.yuanzhike.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wkh.vqdsnc.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yhn.nanxuanxn.top

Go:   slices.Index(arr, x)
来源：http://lkv.cucudq.cn

Ruby: arr.index(x)
来源：http://ywj.gotoacloud.top

C#:   list.IndexOf(x);
来源：http://fsp.ydjk.org.cn

[D13] 过滤（保留满足条件的）
来源：http://zie.daxiang520.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ewz.andypj.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://knm.nanxinkj.top

JS:   arr.filter(x => x > 3)
来源：http://osy.fktsv.cn

TS:   arr.filter(x => x > 3)
来源：http://hty.tianlin.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ntl.vqdsnc.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://imc.epnwcf.com

Ruby: arr.select { |x| x > 3 }
来源：http://oyw.aizwys.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wlq.jinyuanbaomall.cn

[D14] 映射转换（每个元素变形）
来源：http://dht.yangfankeji.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lur.jinqigufen.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mbl.zhoulong.xyz

JS:   arr.map(x => x * 2)
来源：http://qsn.smart0.xyz

TS:   arr.map(x => x * 2)
来源：http://psg.cdnleiting.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://uwo.epnwcf.com

Go:   // 手写循环
来源：http://czl.birdmap.top

Ruby: arr.map { |x| x * 2 }
来源：http://xzm.zhoulong.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://hgm.xingfuxueyuan.xyz

[D15] 去重
来源：http://anl.shangyingyoupin.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://twd.ydjk.org.cn

PHP:  array_unique($arr);
来源：http://zpx.shanyushiyangtech.top

JS:   [...new Set(arr)]
来源：http://wme.sweek.top

TS:   [...new Set(arr)]
来源：http://pnx.ehwqpu.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://afw.bjfxy.top

Go:   // 用 map[T]struct{} 手写
来源：http://oav.yj202588.top

Ruby: arr.uniq
来源：http://wew.ppjwa.cn

C#:   list.Distinct().ToList()
来源：http://exv.smart0.xyz

[D16] 求和与平均值
来源：http://xpc.havefunace.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zzz.fengsongda.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://eqy.zhiwuduotai.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://smx.sysykeji.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rpl.yonumen.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ruh.svipenyu.cn

Go:   // 手写循环累加
来源：http://cfz.bjfxy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bcs.fktsv.cn

C#:   list.Sum();  list.Average()
来源：http://uwt.shzxlz.cn

[D17] 最大值与最小值
来源：http://wca.ybcxt.top

Py:   max(arr);  min(arr)
来源：http://zks.tarul.cn

PHP:  max($arr);  min($arr);
来源：http://iiv.zhoulong.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sos.guowangkeji.top

TS:   Math.max(...arr);
来源：http://eem.chenzaomai.com

Java: Collections.max(list);  Collections.min(list);
来源：http://qxo.jlsjyb.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nmo.birdmap.top

Ruby: arr.max;  arr.min
来源：http://zim.yanxiufei.cn

C#:   list.Max();  list.Min()
来源：http://kha.zhengqikj.top

[D18] 扁平化嵌套数组
来源：http://tem.hammf.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://uqi.zhiwuduotai.top

PHP:  array_merge(...$nested);
来源：http://xaf.316326.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://aat.redwolf501.top

TS:   nested.flat();
来源：http://jci.ivvv.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://whe.cashguo.top

Go:   // 手写双层循环
来源：http://eck.gogol.net.cn

Ruby: nested.flatten
来源：http://ols.hnqzz.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://dfd.pycfn.com

[D19] 按字段分组
来源：http://ros.gotoacloud.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kcs.pycfn.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wax.ywan-chungtsiang.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jxp.yj20258.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ynz.wangshuangyany.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lsn.tianlin.xyz

Go:   // 手写 map[string][]T
来源：http://hmr.nanxinkj.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ubb.zhongyouzk.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nzn.andypj.xyz

[D20] 统计每个元素出现次数
来源：http://ocu.ctjpmb.com

Py:   Counter(arr)
来源：http://akv.316326.xyz

PHP:  array_count_values($arr);
来源：http://mau.uphjek.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rmh.xziqi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rhw.jinqigufen.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fnm.yj202588.top

Go:   // 手写 map[T]int
来源：http://fex.zhengqikj.top

Ruby: arr.tally
来源：http://yut.sufxvd.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://eix.zhoulong.xyz

[D21] 判断是否包含某元素
来源：http://wip.chenjidiqi.icu

Py:   x in arr
来源：http://rmp.yj20258.top

PHP:  in_array($x, $arr, true);
来源：http://hbo.guowangkeji.top

JS:   arr.includes(x)
来源：http://phd.sysykeji.top

TS:   arr.includes(x)
来源：http://xgv.hnqzz.top

Java: list.contains(x)
来源：http://lux.haohaochexian.top

Go:   slices.Contains(arr, x)
来源：http://kkr.aizwys.cn

Ruby: arr.include?(x)
来源：http://vkh.tianlin.xyz

C#:   list.Contains(x)
来源：http://azs.ppjwa.cn

[D22] 复制数组（避免共享引用）
来源：http://wys.wangshuangyany.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://oen.yangfankeji.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nqd.gotoacloud.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://skd.cashguo.top

TS:   [...arr];
来源：http://faj.meibo888.top

Java: new ArrayList<>(list);
来源：http://xec.hfpthk.cn

Go:   copied := append([]int(nil), arr...)
来源：http://fou.xinyue.icu

Ruby: arr.dup;  arr.clone
来源：http://awx.cdnleiting.top

C#:   new List<int>(list);
来源：http://stj.jlsjyb.cn

[D23] reduce 累积计算
来源：http://ynk.aizwys.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ewu.feifeiyinyue.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zzp.52xcode.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://few.mhx1999.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vmh.sufxvd.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hhl.daxiang520.top

Go:   // 手写循环
来源：http://yxm.ehwqpu.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://byt.svipenyu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ujv.guannengcc.top

[D24] 字典 / Map 基本操作
来源：http://gdl.chenzaomai.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vox.jiagoushi.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://men.uphjek.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://iwh.sufxvd.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://okr.jinyuanbaomall.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kjc.cashguo.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sbb.zhoulong.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gil.vehdjk.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mxo.aizwys.cn

[D25] Set 集合去重与交并差
来源：http://ewo.jinqigufen.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://njv.nanxinkj.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://iqh.tarul.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bce.cashguo.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xzm.jqgfzy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ggz.ywan-chungtsiang.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yix.zhaomingkeji.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fjz.meibo888.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zck.svipenyu.cn

[D26] 数组转字符串
来源：http://idb.jinqigufen.top

Py:   ", ".join(map(str, arr))
来源：http://ysv.nanxinkj.top

PHP:  implode(", ", $arr);
来源：http://jkx.52xcode.cn

JS:   arr.join(", ")
来源：http://gua.meibo888.top

TS:   arr.join(", ")
来源：http://iuk.jiagoushi.top

Java: String.join(", ", list)
来源：http://sbw.gogol.net.cn

Go:   strings.Join(strs, ", ")
来源：http://qoy.xingfuxueyuan.xyz

Ruby: arr.join(", ")
来源：http://bpz.ydjk.org.cn

C#:   string.Join(", ", list)
来源：http://duo.ctjpmb.com


<!-- 参考信息 -->