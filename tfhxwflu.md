代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sto.ivvv.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gfs.pengpengdd.cyou

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xpe.wangshuangyany.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wbi.jinqigfzy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fhi.redwolf501.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tqr.zdqjudy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://eac.jianghu66.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ajy.pengpengdd.cyou

[C10] 变量作用域
来源：http://phm.yangfankeji.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://owp.xingfuxueyuan.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://apv.sufxvd.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rtj.dianchejie.cn

TS:   同 JS
来源：http://zde.hnxiangtu.top

Java: 方法内为块级作用域
来源：http://qan.chenjidiqi.icu

Go:   花括号块级作用域
来源：http://rin.hywenlv.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hmp.jqgufenzy.top

C#:   块级作用域
来源：http://nif.yuanzhike.top

[C11] 模块导入与导出
来源：http://qgi.jinyuanbaomall.cn

Py:   from module import func
来源：http://ouu.shanyushiyangkeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://eet.tarul.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://btm.vehdjk.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ayj.pengpengdd.cyou

Java: import java.util.List;
来源：http://zsj.hnqzz.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://itj.hfpthk.cn

Ruby: require "json"; require_relative "./util"
来源：http://xnu.yuanzhike.top

C#:   using System.Text;
来源：http://ztj.xziqi.cn

[C12] 立即执行函数 IIFE
来源：http://rob.yonumen.top

Py:   (lambda: print("run"))()
来源：http://kee.yueranfly.top

PHP:  (function () { echo "run"; })();
来源：http://fag.dashuyun.cn

JS:   (() => { console.log("run"); })();
来源：http://phi.pycfn.com

TS:   (() => { console.log("run"); })();
来源：http://uyg.ppjwa.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nbf.jinghuilouyu.cn

Go:   func() { fmt.Println("run") }()
来源：http://vzg.zhaomingkeji.xyz

Ruby: -> { puts "run" }.call
来源：http://erw.jlsjyb.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://irr.jiagoushi.top

[C13] 类型声明 / 类型注解
来源：http://rzx.shuidangran.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ikj.aizwys.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wxt.gzhubu.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vzq.xinyue.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kqw.hfpthk.cn

Java: int add(int a, int b) { return a + b; }
来源：http://slf.havefunace.top

Go:   func add(a, b int) int
来源：http://qih.tian-w.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gec.zhiwuduotai.top

C#:   int Add(int a, int b) => a + b;
来源：http://vge.xuetiantiany.cn

[C14] 泛型函数
来源：http://fxj.ydzc1.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zen.iojbl.cn

PHP:  // 无泛型
来源：http://wws.yuxming.cn

JS:   // 无泛型
来源：http://spx.ywan-chungtsiang.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://upl.guowangkeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dnc.hesvh.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://sat.c1oappe.top

Ruby: # 无泛型
来源：http://cvu.wangshuangyany.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blc.shanyushiyangtech.top

[C15] 解构 / 展开参数
来源：http://fxa.havefunace.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lzd.c1oappe.top

PHP:  [$a, $b] = $pair;
来源：http://mcx.pycfn.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xaq.fehbvm.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kme.ivvv.top

Java: // 无解构
来源：http://hlq.daxiang520.top

Go:   // 无解构
来源：http://gbz.316326.xyz

Ruby: a, b = pair
来源：http://jpj.sysykeji.top

C#:   var (a, b) = pair;
来源：http://lwo.tarul.cn

[C16] 函数 / 方法重载
来源：http://civ.pycfn.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sda.wangdashe.top

PHP:  // 无重载
来源：http://kyw.shanyushiyangtech.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ycm.sjlbkw.cn

TS:   // 用联合类型或重载签名声明
来源：http://szb.aizwys.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rzo.zhongyouzk.top

Go:   // 无重载：用不同函数名
来源：http://mpl.yfazqb.com

Ruby: # 无重载：靠动态参数
来源：http://ttw.smart0.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://nlm.vehdjk.com

================================================================================
来源：http://lnb.yj202588.top

D. 数组 / 列表 / 集合
来源：http://bec.yongpay.top

================================================================================
来源：http://lkz.yangfankeji.com

[D01] 创建数组 / 列表
来源：http://mbb.uphjek.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://fhz.xinyue.icu

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xer.chenlongwang.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nkx.haohaochexian.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://smc.yj202588.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cqi.sjlbkw.cn

Go:   arr := []int{1, 2, 3}
来源：http://cai.ydzc1.top

Ruby: arr = [1, 2, 3]
来源：http://vxw.cheryme.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yob.kuanghao11.cn

[D02] 追加元素到末尾
来源：http://jpi.gaohongyu789.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://czg.quarkkingdee.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kdf.hnxiangtu.top

JS:   arr.push(4);
来源：http://pfq.vehdjk.com

TS:   arr.push(4);
来源：http://vnj.9152youxi.cn

Java: list.add(4);
来源：http://nbr.daria6918.cn

Go:   arr = append(arr, 4)
来源：http://ojg.svipenyu.cn

Ruby: arr << 4; arr.push(5)
来源：http://elm.zhengqikj.top

C#:   list.Add(4);
来源：http://liz.cucudq.cn

[D03] 在指定位置插入元素
来源：http://hlh.jiagoushi.top

Py:   arr.insert(0, 0)
来源：http://pfp.yongpay.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://umm.ehwqpu.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ilc.zycfv.cn

TS:   arr.splice(0, 0, 0);
来源：http://swo.yonumen.top

Java: list.add(0, 0);
来源：http://lpy.epnwcf.com

Go:   arr = append([]int{0}, arr...)
来源：http://fes.tarul.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rgz.xuanzx.com

C#:   list.Insert(0, 0);
来源：http://zbn.gotoacloud.top

[D04] 删除元素
来源：http://cmi.zhijiandao.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qvo.zhijiandao.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://avp.zhiwuduotai.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xpy.zycfv.cn

TS:   arr.splice(0, 1);
来源：http://uir.yuanzhike.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gro.xziqi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fhz.jiagoushi.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ocx.birdmap.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rgb.zdqjudy.top

[D05] 访问与修改元素
来源：http://ylj.fengsongda.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ymu.wangdashe.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hkz.ppjwa.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://coc.zycfv.cn

TS:   arr[0]; arr.at(-1);
来源：http://tbb.yj20258888.top

Java: list.get(0); list.set(0, 9);
来源：http://zrc.aizwys.cn

Go:   arr[0]; arr[0] = 9
来源：http://kme.guannengcc.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vlp.svipenyu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ofz.fzhhl.top

[D06] 数组长度
来源：http://bex.uphjek.com

Py:   len(arr)
来源：http://vlg.redwolf501.top

PHP:  count($arr);
来源：http://baf.yvedp.cn

JS:   arr.length
来源：http://ref.chenjidiqi.icu

TS:   arr.length
来源：http://flu.ehwqpu.com

Java: list.size();
来源：http://yft.bjfxy.top

Go:   len(arr)
来源：http://knm.vqdsnc.cn

Ruby: arr.length; arr.size
来源：http://abw.vehdjk.com

C#:   list.Count;
来源：http://yzk.yvedp.cn

[D07] 切片 / 取子数组
来源：http://sgx.mhx1999.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ptx.kuanghao11.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zaf.havefunace.top

JS:   arr.slice(1, 4);
来源：http://gim.yueranfly.top

TS:   arr.slice(1, 4);
来源：http://swb.haohaochexian.top

Java: list.subList(1, 4);
来源：http://tjg.zhengqikj.top

Go:   arr[1:4]
来源：http://vkc.andypj.xyz

Ruby: arr[1, 3]
来源：http://czd.haohaochexian.top

C#:   list.GetRange(1, 3);
来源：http://vzp.pycfn.com

[D08] 合并两个数组
来源：http://yvn.0kj1m.cn

Py:   a + b;  a.extend(b)
来源：http://tcx.jinyuanbaomall.cn

PHP:  array_merge($a, $b);
来源：http://zhk.shangyingyoupin.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ill.shangyingyoupin.top

TS:   [...a, ...b];
来源：http://may.ywan-chungtsiang.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zzn.chenlongwang.top

Go:   append(a, b...)
来源：http://cjh.hfpthk.cn

Ruby: a + b;  a.concat(b)
来源：http://dzj.havefunace.top

C#:   a.Concat(b).ToList()
来源：http://lhn.snrcjt.cn

[D09] 排序（升序）
来源：http://gjx.chenlongwang.top

Py:   sorted(arr);  arr.sort()
来源：http://smz.zhaomingkeji.xyz

PHP:  sort($arr);
来源：http://hkz.bbcook.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kaf.jinqigufen.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://wqc.nanxuanxn.top

Java: Collections.sort(list);  list.sort(null);
来源：http://tjl.fehbvm.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://heu.xingfuxueyuan.xyz

Ruby: arr.sort
来源：http://ugf.ywan-chungtsiang.top

C#:   list.Sort();
来源：http://rtq.gaohongyu789.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://pzv.cucudq.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bqh.gzhubu.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://poe.zhongyouzk.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://evu.zdbjq.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nao.dianchejie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qoo.birdmap.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dqn.yongpay.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rhd.hysaishi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yex.jianghu66.top

[D11] 反转数组
来源：http://crh.yvedp.cn

Py:   arr[::-1];  arr.reverse()
来源：http://bzp.chenjidiqi.icu

PHP:  array_reverse($arr);
来源：http://lrc.jianghu66.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dls.fanxiaobao.xyz

TS:   [...arr].reverse();
来源：http://car.birdmap.top

Java: Collections.reverse(list);
来源：http://cyp.feifeiyinyue.top

Go:   slices.Reverse(arr)
来源：http://vbc.yangfankeji.com

Ruby: arr.reverse
来源：http://klt.pengpengdd.cyou

C#:   list.Reverse();
来源：http://zdl.xziqi.cn

[D12] 查找元素下标
来源：http://svc.zdqjudy.top

Py:   arr.index(x);  x in arr
来源：http://hbe.daxiang520.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ers.yonumen.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iaw.fktsv.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qzd.cucudq.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zjd.hysaishi.cn

Go:   slices.Index(arr, x)
来源：http://jev.zycfv.cn

Ruby: arr.index(x)
来源：http://tws.sjlbkw.cn

C#:   list.IndexOf(x);
来源：http://dph.daria6918.cn

[D13] 过滤（保留满足条件的）
来源：http://igh.ehwqpu.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zaw.meibo888.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xwz.yvedp.cn

JS:   arr.filter(x => x > 3)
来源：http://moo.hcnkem.com

TS:   arr.filter(x => x > 3)
来源：http://hub.zdbjq.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wnp.nanxuanxn.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://omb.nwbrower.top

Ruby: arr.select { |x| x > 3 }
来源：http://njj.c1oappe.top

C#:   list.Where(x => x > 3).ToList()
来源：http://hdx.xylfe.cn

[D14] 映射转换（每个元素变形）
来源：http://aoc.pycfn.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kgx.pengpengdd.cyou

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://twv.redwolf501.top

JS:   arr.map(x => x * 2)
来源：http://ixb.yanxiufei.cn

TS:   arr.map(x => x * 2)
来源：http://szn.uphjek.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://ndg.zhengqikj.top

Go:   // 手写循环
来源：http://zah.yangfankeji.com

Ruby: arr.map { |x| x * 2 }
来源：http://lrt.sweek.top

C#:   list.Select(x => x * 2).ToList()
来源：http://avk.shangyingyoupin.top

[D15] 去重
来源：http://xea.sxryk.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fos.fktsv.cn

PHP:  array_unique($arr);
来源：http://taz.aizwys.cn

JS:   [...new Set(arr)]
来源：http://vrb.shuidangran.top

TS:   [...new Set(arr)]
来源：http://bsb.ppjwa.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zka.meibo888.top

Go:   // 用 map[T]struct{} 手写
来源：http://bnh.cucudq.cn

Ruby: arr.uniq
来源：http://vsx.feifeiyinyue.top

C#:   list.Distinct().ToList()
来源：http://eup.bjfxy.top

[D16] 求和与平均值
来源：http://bvi.jinghuilouyu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sjw.yuanzhike.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sea.ybcxt.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qww.gogol.net.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ivl.aibaodan.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xys.hammf.cn

Go:   // 手写循环累加
来源：http://xln.sysykeji.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qfg.gaohongyu789.top

C#:   list.Sum();  list.Average()
来源：http://irf.hammf.cn

[D17] 最大值与最小值
来源：http://ucv.gzhubu.top

Py:   max(arr);  min(arr)
来源：http://eoe.ywan-chungtsiang.top

PHP:  max($arr);  min($arr);
来源：http://kpx.shuidangran.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qwm.cqqwz.cn

TS:   Math.max(...arr);
来源：http://qbs.iojbl.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://iwr.xuetiantiany.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wpp.52xcode.cn

Ruby: arr.max;  arr.min
来源：http://mir.jinqigfzy.top

C#:   list.Max();  list.Min()
来源：http://zmm.jqgfzy.top

[D18] 扁平化嵌套数组
来源：http://box.zycfv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://asy.pycfn.com

PHP:  array_merge(...$nested);
来源：http://znj.kuanghao11.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://boj.fengsongda.top

TS:   nested.flat();
来源：http://zlq.9152youxi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ftl.yongpay.top

Go:   // 手写双层循环
来源：http://pao.svipenyu.cn

Ruby: nested.flatten
来源：http://ris.jinghuilouyu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://jlt.ctjpmb.com

[D19] 按字段分组
来源：http://vfn.pycfn.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sat.cheryme.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nug.zhoulong.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uzk.hywenlv.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://auk.xylfe.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ksz.sysykeji.top

Go:   // 手写 map[string][]T
来源：http://uss.yj20258888.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://bkw.jlsjyb.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bkh.fengsongda.top

[D20] 统计每个元素出现次数
来源：http://zfr.yj20258888.top

Py:   Counter(arr)
来源：http://cmi.zhengqikj.top

PHP:  array_count_values($arr);
来源：http://rxc.zycfv.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jkk.cashguo.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dnf.ydjk.org.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zcf.fehbvm.com

Go:   // 手写 map[T]int
来源：http://vwk.jinghuilouyu.cn

Ruby: arr.tally
来源：http://bas.hcnkem.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fig.xuetiantiany.cn

[D21] 判断是否包含某元素
来源：http://vac.0kj1m.cn

Py:   x in arr
来源：http://ttg.tanke756.top

PHP:  in_array($x, $arr, true);
来源：http://jrm.zhongyouzk.top

JS:   arr.includes(x)
来源：http://ont.andypj.xyz

TS:   arr.includes(x)
来源：http://waq.fengsongda.top

Java: list.contains(x)
来源：http://hbd.yueranfly.top

Go:   slices.Contains(arr, x)
来源：http://elp.jinghuilouyu.cn

Ruby: arr.include?(x)
来源：http://evc.fzhhl.top

C#:   list.Contains(x)
来源：http://qdr.ywan-chungtsiang.top

[D22] 复制数组（避免共享引用）
来源：http://ola.nwbrower.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mlj.fktsv.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gdc.gaohongyu789.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://akb.hysaishi.cn

TS:   [...arr];
来源：http://noe.quarkkingdee.top

Java: new ArrayList<>(list);
来源：http://ouu.nanxinkj.top

Go:   copied := append([]int(nil), arr...)
来源：http://yda.feifeiyinyue.top

Ruby: arr.dup;  arr.clone
来源：http://kjg.guannengcc.top

C#:   new List<int>(list);
来源：http://evl.yvedp.cn

[D23] reduce 累积计算
来源：http://tqz.zhiwuduotai.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ohr.andypj.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wak.ehwqpu.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wpu.svipenyu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://aqi.zycfv.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://quk.daria6918.cn

Go:   // 手写循环
来源：http://ucq.sweek.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wyo.yangfankeji.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fet.chenjidiqi.icu

[D24] 字典 / Map 基本操作
来源：http://ask.daxiang520.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xco.jinqigufen.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ici.ybcxt.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xyy.jqgufenzy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sok.hcnkem.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zqs.xuetiantiany.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wbf.yuxming.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qcl.ywan-chungtsiang.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hqr.wangdashe.top

[D25] Set 集合去重与交并差
来源：http://ppi.havefunace.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qcg.tanke756.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yev.sweek.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ior.mhx1999.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ugn.zhijiandao.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://grx.hnqzz.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nws.fktsv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vbo.meibo888.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ifj.dianchejie.cn

[D26] 数组转字符串
来源：http://afb.jiagoushi.top


<!-- 参考信息 -->