代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://fxm.pycfn.com

C#:   using System.Text;
来源：http://ijm.xuanzx.com

[C12] 立即执行函数 IIFE
来源：http://ebs.haohaochexian.top

Py:   (lambda: print("run"))()
来源：http://fbu.0kj1m.cn

PHP:  (function () { echo "run"; })();
来源：http://bzw.hesvh.cn

JS:   (() => { console.log("run"); })();
来源：http://ygk.aibaodan.cn

TS:   (() => { console.log("run"); })();
来源：http://fpg.shanyushiyangkeji.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lhu.guowangkeji.top

Go:   func() { fmt.Println("run") }()
来源：http://aqe.epnwcf.com

Ruby: -> { puts "run" }.call
来源：http://zxw.epnwcf.com

C#:   // 无 IIFE：用静态构造函数
来源：http://zvo.daria6918.cn

[C13] 类型声明 / 类型注解
来源：http://xby.ehwqpu.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qze.gogol.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ofg.ydzc1.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jqh.fzhhl.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mtr.smart0.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://xhx.vehdjk.com

Go:   func add(a, b int) int
来源：http://blj.zhiwuduotai.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kly.kuanghao11.cn

C#:   int Add(int a, int b) => a + b;
来源：http://eew.shzxlz.cn

[C14] 泛型函数
来源：http://idq.jinghuilouyu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://byd.ctjpmb.com

PHP:  // 无泛型
来源：http://sef.bjfxy.top

JS:   // 无泛型
来源：http://rbd.yj202588.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pms.yanxiufei.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gab.daxiang520.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vww.iojbl.cn

Ruby: # 无泛型
来源：http://opj.yuxming.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ynt.hcnkem.com

[C15] 解构 / 展开参数
来源：http://xrq.fehbvm.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://uoc.xingfuxueyuan.xyz

PHP:  [$a, $b] = $pair;
来源：http://fvy.nanxinkj.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nmd.cashguo.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qpl.yj20258888.top

Java: // 无解构
来源：http://msl.fktsv.cn

Go:   // 无解构
来源：http://bwz.jlsjyb.cn

Ruby: a, b = pair
来源：http://rku.vqdsnc.cn

C#:   var (a, b) = pair;
来源：http://hgz.meibo888.top

[C16] 函数 / 方法重载
来源：http://alw.fanxiaobao.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pkh.jyoumei.cn

PHP:  // 无重载
来源：http://jvi.hysaishi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://nxl.snrcjt.cn

TS:   // 用联合类型或重载签名声明
来源：http://ifo.zycfv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://uzv.jqgfzy.top

Go:   // 无重载：用不同函数名
来源：http://ect.chenlongwang.top

Ruby: # 无重载：靠动态参数
来源：http://wca.xingfuxueyuan.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://eby.xziqi.cn

================================================================================
来源：http://krw.yongpay.top

D. 数组 / 列表 / 集合
来源：http://wat.yonumen.top

================================================================================
来源：http://mda.shanyushiyangkeji.top

[D01] 创建数组 / 列表
来源：http://ehv.jinqigfzy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://lfd.jinghuilouyu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://naj.0kj1m.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jlu.hcnkem.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://unh.zycfv.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ukk.fktsv.cn

Go:   arr := []int{1, 2, 3}
来源：http://vxn.dianchejie.cn

Ruby: arr = [1, 2, 3]
来源：http://pte.hnqzz.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://eqo.ehwqpu.com

[D02] 追加元素到末尾
来源：http://jqe.wangdashe.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kfx.shzxlz.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fzr.shanyushiyangtech.top

JS:   arr.push(4);
来源：http://xbn.chenlongwang.top

TS:   arr.push(4);
来源：http://mjd.hongshengwenyu.top

Java: list.add(4);
来源：http://cyr.c1oappe.top

Go:   arr = append(arr, 4)
来源：http://ogk.hesvh.cn

Ruby: arr << 4; arr.push(5)
来源：http://vkm.svipenyu.cn

C#:   list.Add(4);
来源：http://kty.xuanzx.com

[D03] 在指定位置插入元素
来源：http://esg.wangshuangyany.cn

Py:   arr.insert(0, 0)
来源：http://bub.guannengcc.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qfx.vehdjk.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rmf.ivvv.top

TS:   arr.splice(0, 0, 0);
来源：http://jpr.c1oappe.top

Java: list.add(0, 0);
来源：http://yqm.hysaishi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://csd.jinqigfzy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tlb.snrcjt.cn

C#:   list.Insert(0, 0);
来源：http://fli.cheryme.top

[D04] 删除元素
来源：http://wwa.birdmap.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dyw.sxryk.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bgs.mhx1999.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ztz.pengpengdd.cyou

TS:   arr.splice(0, 1);
来源：http://spp.ctjpmb.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xua.yj202588.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://oxw.jinqigufen.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://uoc.gotoacloud.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xse.9152youxi.cn

[D05] 访问与修改元素
来源：http://klx.fehbvm.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://uep.hesvh.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://psu.quarkkingdee.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dio.nanxinkj.top

TS:   arr[0]; arr.at(-1);
来源：http://gsg.fktsv.cn

Java: list.get(0); list.set(0, 9);
来源：http://fbh.feifeiyinyue.top

Go:   arr[0]; arr[0] = 9
来源：http://ver.sweek.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jzc.fehbvm.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zbr.daria6918.cn

[D06] 数组长度
来源：http://zdz.daria6918.cn

Py:   len(arr)
来源：http://bbe.xziqi.cn

PHP:  count($arr);
来源：http://sic.hesvh.cn

JS:   arr.length
来源：http://wpo.snrcjt.cn

TS:   arr.length
来源：http://epz.zhoulong.xyz

Java: list.size();
来源：http://vqf.hywenlv.cn

Go:   len(arr)
来源：http://bcq.52xcode.cn

Ruby: arr.length; arr.size
来源：http://apy.jlsjyb.cn

C#:   list.Count;
来源：http://wfc.xziqi.cn

[D07] 切片 / 取子数组
来源：http://zje.yfazqb.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yiq.nanxinkj.top

PHP:  array_slice($arr, 1, 3);
来源：http://qby.hysaishi.cn

JS:   arr.slice(1, 4);
来源：http://xgh.0kj1m.cn

TS:   arr.slice(1, 4);
来源：http://wlq.ivvv.top

Java: list.subList(1, 4);
来源：http://yqg.316326.xyz

Go:   arr[1:4]
来源：http://rpj.xylfe.cn

Ruby: arr[1, 3]
来源：http://nbw.dashuyun.cn

C#:   list.GetRange(1, 3);
来源：http://yvb.jianghu66.top

[D08] 合并两个数组
来源：http://svk.aizwys.cn

Py:   a + b;  a.extend(b)
来源：http://xdo.yongpay.top

PHP:  array_merge($a, $b);
来源：http://tak.gogol.net.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xey.chenjidiqi.icu

TS:   [...a, ...b];
来源：http://siu.pengpengdd.cyou

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jfx.nwbrower.top

Go:   append(a, b...)
来源：http://dsb.pycfn.com

Ruby: a + b;  a.concat(b)
来源：http://eub.nwbrower.top

C#:   a.Concat(b).ToList()
来源：http://jnc.fanxiaobao.xyz

[D09] 排序（升序）
来源：http://ksv.yonumen.top

Py:   sorted(arr);  arr.sort()
来源：http://fxb.shanyushiyangtech.top

PHP:  sort($arr);
来源：http://vja.bjfxy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jij.haohaochexian.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ssd.andypj.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://kfs.mhx1999.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cjq.sweek.top

Ruby: arr.sort
来源：http://hhx.shuidangran.top

C#:   list.Sort();
来源：http://kla.ppjwa.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://try.zhixingplan.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rix.9152youxi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://svf.daria6918.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vnp.cqqwz.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gba.jinqigufen.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fda.jinyuanbaomall.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vpf.zhoulong.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kwn.jinghuilouyu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ofx.zhongyouzk.top

[D11] 反转数组
来源：http://rrl.zhiwuduotai.top

Py:   arr[::-1];  arr.reverse()
来源：http://ujw.shanyushiyangtech.top

PHP:  array_reverse($arr);
来源：http://bxo.iojbl.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://aml.yfazqb.com

TS:   [...arr].reverse();
来源：http://nln.jlsjyb.cn

Java: Collections.reverse(list);
来源：http://bab.xziqi.cn

Go:   slices.Reverse(arr)
来源：http://ooh.nanxinkj.top

Ruby: arr.reverse
来源：http://tlg.hesvh.cn

C#:   list.Reverse();
来源：http://yjd.jianghu66.top

[D12] 查找元素下标
来源：http://yxd.fanxiaobao.xyz

Py:   arr.index(x);  x in arr
来源：http://sqm.hesvh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://src.tanke756.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://roi.yj20258888.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hce.jyoumei.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cme.ydjk.org.cn

Go:   slices.Index(arr, x)
来源：http://nmb.yangfankeji.com

Ruby: arr.index(x)
来源：http://xfw.sweek.top

C#:   list.IndexOf(x);
来源：http://nti.zycfv.cn

[D13] 过滤（保留满足条件的）
来源：http://tej.snrcjt.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lpk.ydjk.org.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jwo.meibo888.top

JS:   arr.filter(x => x > 3)
来源：http://vby.shanyushiyangkeji.top

TS:   arr.filter(x => x > 3)
来源：http://clq.yj20258888.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://div.fzhhl.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mui.fktsv.cn

Ruby: arr.select { |x| x > 3 }
来源：http://gwr.hnxiangtu.top

C#:   list.Where(x => x > 3).ToList()
来源：http://eah.zhijiandao.cn

[D14] 映射转换（每个元素变形）
来源：http://lns.quarkkingdee.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cpk.ydzc1.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tfn.shanyushiyangkeji.top

JS:   arr.map(x => x * 2)
来源：http://lob.daria6918.cn

TS:   arr.map(x => x * 2)
来源：http://kej.nanxuanxn.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://jqb.zdqjudy.top

Go:   // 手写循环
来源：http://lei.cucudq.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dst.hysaishi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ttq.sjlbkw.cn

[D15] 去重
来源：http://zji.epnwcf.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hwj.sweek.top

PHP:  array_unique($arr);
来源：http://rsu.feifeiyinyue.top

JS:   [...new Set(arr)]
来源：http://cqt.smart0.xyz

TS:   [...new Set(arr)]
来源：http://olh.ehwqpu.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mnu.havefunace.top

Go:   // 用 map[T]struct{} 手写
来源：http://odz.hywenlv.cn

Ruby: arr.uniq
来源：http://uwl.vqdsnc.cn

C#:   list.Distinct().ToList()
来源：http://lxm.dashuyun.cn

[D16] 求和与平均值
来源：http://jbi.tianlin.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://frs.zhongyouzk.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lqx.xylfe.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kcw.tarul.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wcv.yuxming.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ogj.fehbvm.com

Go:   // 手写循环累加
来源：http://uzg.bbcook.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pnv.bjfxy.top

C#:   list.Sum();  list.Average()
来源：http://fri.feifeiyinyue.top

[D17] 最大值与最小值
来源：http://ise.sufxvd.cn

Py:   max(arr);  min(arr)
来源：http://htx.feifeiyinyue.top

PHP:  max($arr);  min($arr);
来源：http://hkm.xingfuxueyuan.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cfj.ydzc1.top

TS:   Math.max(...arr);
来源：http://diy.yj20258888.top

Java: Collections.max(list);  Collections.min(list);
来源：http://wmu.sweek.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://arl.zhiwuduotai.top

Ruby: arr.max;  arr.min
来源：http://klc.wangdashe.top

C#:   list.Max();  list.Min()
来源：http://cpk.xuanzx.com

[D18] 扁平化嵌套数组
来源：http://iym.birdmap.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pka.zhixingplan.top

PHP:  array_merge(...$nested);
来源：http://rah.c1oappe.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wav.daria6918.cn

TS:   nested.flat();
来源：http://igb.chenjidiqi.icu

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jph.zhongyouzk.top

Go:   // 手写双层循环
来源：http://gbo.ehwqpu.com

Ruby: nested.flatten
来源：http://ghk.yj20258888.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://lcf.shzxlz.cn

[D19] 按字段分组
来源：http://gui.yj20258.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qac.tianlin.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jrt.redwolf501.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uld.birdmap.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ldz.jinqigfzy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ndj.shuidangran.top

Go:   // 手写 map[string][]T
来源：http://aww.meibo888.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ksa.zdqjudy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cae.ppjwa.cn

[D20] 统计每个元素出现次数
来源：http://sdx.pengpengdd.cyou

Py:   Counter(arr)
来源：http://oum.yuanzhike.top

PHP:  array_count_values($arr);
来源：http://wxm.smart0.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://har.xuetiantiany.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://whq.wangdashe.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ato.ivvv.top

Go:   // 手写 map[T]int
来源：http://txf.haohaochexian.top

Ruby: arr.tally
来源：http://pbh.andypj.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://khh.jinghuilouyu.cn

[D21] 判断是否包含某元素
来源：http://tkk.zycfv.cn

Py:   x in arr
来源：http://mfb.havefunace.top

PHP:  in_array($x, $arr, true);
来源：http://qhe.zhongyouzk.top

JS:   arr.includes(x)
来源：http://eyo.dianchejie.cn

TS:   arr.includes(x)
来源：http://hlt.smart0.xyz

Java: list.contains(x)
来源：http://rwu.wangdashe.top

Go:   slices.Contains(arr, x)
来源：http://lrp.zhixingplan.top

Ruby: arr.include?(x)
来源：http://wyk.shzxlz.cn

C#:   list.Contains(x)
来源：http://dlr.ctjpmb.com

[D22] 复制数组（避免共享引用）
来源：http://lkd.zdbjq.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tbw.dianchejie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nhb.xuanzx.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xzm.meibo888.top

TS:   [...arr];
来源：http://sro.ppjwa.cn

Java: new ArrayList<>(list);
来源：http://fgk.zhaomingkeji.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://cqi.ywan-chungtsiang.top

Ruby: arr.dup;  arr.clone
来源：http://ipn.xuanzx.com

C#:   new List<int>(list);
来源：http://omp.hywenlv.cn

[D23] reduce 累积计算
来源：http://vej.yj202588.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lvn.yvedp.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yij.jinqigufen.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ozt.yanxiufei.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://srq.tanke756.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://vvy.aizwys.cn

Go:   // 手写循环
来源：http://fba.sysykeji.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uxn.shuidangran.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://faa.gaohongyu789.top

[D24] 字典 / Map 基本操作
来源：http://bqu.hysaishi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gwq.tian-w.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ssm.birdmap.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nlf.yj20258888.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fwm.zhijiandao.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://akg.yj202588.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hnr.9152youxi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dqe.zdbjq.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xpe.aizwys.cn

[D25] Set 集合去重与交并差
来源：http://jzc.ehwqpu.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://uzi.pengpengdd.cyou

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gpn.hammf.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jsr.daria6918.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://frg.shzxlz.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rwh.bjfxy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fcw.iojbl.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hih.ivvv.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lcx.zhengqikj.top

[D26] 数组转字符串
来源：http://wod.jqgufenzy.top

Py:   ", ".join(map(str, arr))
来源：http://ekf.hysaishi.cn

PHP:  implode(", ", $arr);
来源：http://dif.pengpengdd.cyou

JS:   arr.join(", ")
来源：http://wcj.jlsjyb.cn

TS:   arr.join(", ")
来源：http://sgw.birdmap.top

Java: String.join(", ", list)
来源：http://yft.fzhhl.top

Go:   strings.Join(strs, ", ")
来源：http://ulk.fehbvm.com

Ruby: arr.join(", ")
来源：http://hgs.xylfe.cn

C#:   string.Join(", ", list)
来源：http://eoz.sjlbkw.cn

================================================================================
来源：http://clq.sweek.top

E. 字符串处理
来源：http://iss.xylfe.cn

================================================================================
来源：http://zev.ybcxt.top

[E01] 拼接字符串
来源：http://nyv.zhoulong.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mvo.mhx1999.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://awd.shanyushiyangkeji.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jrk.gotoacloud.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://utm.fengsongda.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mje.shanyushiyangkeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pci.chenjidiqi.icu

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ydd.meibo888.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ksz.wangshuangyany.cn

[E02] 重复字符串
来源：http://inp.wangdashe.top

Py:   "ab" * 3
来源：http://nds.yvedp.cn

PHP:  str_repeat("ab", 3);
来源：http://crr.c1oappe.top

JS:   "ab".repeat(3)
来源：http://xge.yfazqb.com


<!-- 参考信息 -->