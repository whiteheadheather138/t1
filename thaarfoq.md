代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://cwl.c1oappe.top

C#:   using System.Text;
来源：http://nde.ywan-chungtsiang.top

[C12] 立即执行函数 IIFE
来源：http://awf.hnxiangtu.top

Py:   (lambda: print("run"))()
来源：http://brf.mhx1999.top

PHP:  (function () { echo "run"; })();
来源：http://igz.xinyue.icu

JS:   (() => { console.log("run"); })();
来源：http://jim.nanxuanxn.top

TS:   (() => { console.log("run"); })();
来源：http://zcz.9152youxi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fot.gzhubu.top

Go:   func() { fmt.Println("run") }()
来源：http://eqb.shzxlz.cn

Ruby: -> { puts "run" }.call
来源：http://nim.sxryk.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ffd.mhx1999.top

[C13] 类型声明 / 类型注解
来源：http://ypw.zhoulong.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://snp.nwbrower.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dnp.xuanzx.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ctk.xuanzx.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://eat.hnxiangtu.top

Java: int add(int a, int b) { return a + b; }
来源：http://cjk.zhongyouzk.top

Go:   func add(a, b int) int
来源：http://ham.aibaodan.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hel.dashuyun.cn

C#:   int Add(int a, int b) => a + b;
来源：http://lfw.jlsjyb.cn

[C14] 泛型函数
来源：http://lpf.xuetiantiany.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://etc.gotoacloud.top

PHP:  // 无泛型
来源：http://syv.zhengqikj.top

JS:   // 无泛型
来源：http://jgq.kuanghao11.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hin.yanxiufei.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ctg.zhijiandao.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ibo.sweek.top

Ruby: # 无泛型
来源：http://eks.ivvv.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nzk.zdbjq.cn

[C15] 解构 / 展开参数
来源：http://wvg.jinyuanbaomall.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vka.zhengqikj.top

PHP:  [$a, $b] = $pair;
来源：http://wgq.jinghuilouyu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pvo.yj202588.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dvp.ivvv.top

Java: // 无解构
来源：http://hag.svipenyu.cn

Go:   // 无解构
来源：http://imp.feifeiyinyue.top

Ruby: a, b = pair
来源：http://dow.feifeiyinyue.top

C#:   var (a, b) = pair;
来源：http://qtq.yonumen.top

[C16] 函数 / 方法重载
来源：http://zlj.tianlin.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://meq.shangyingyoupin.top

PHP:  // 无重载
来源：http://vru.fengsongda.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://fun.cucudq.cn

TS:   // 用联合类型或重载签名声明
来源：http://xsm.nwbrower.top

Java: void f(int a) {}  void f(String a) {}
来源：http://xek.sufxvd.cn

Go:   // 无重载：用不同函数名
来源：http://nqi.sufxvd.cn

Ruby: # 无重载：靠动态参数
来源：http://inp.kuanghao11.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://drc.daxiang520.top

================================================================================
来源：http://bim.redwolf501.top

D. 数组 / 列表 / 集合
来源：http://gkg.gaohongyu789.top

================================================================================
来源：http://btp.dianchejie.cn

[D01] 创建数组 / 列表
来源：http://nio.tanke756.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://zup.0kj1m.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ici.ybcxt.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://idn.dashuyun.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dix.snrcjt.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://psx.tarul.cn

Go:   arr := []int{1, 2, 3}
来源：http://ced.hfpthk.cn

Ruby: arr = [1, 2, 3]
来源：http://mpt.shanyushiyangtech.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://afm.guowangkeji.top

[D02] 追加元素到末尾
来源：http://bvc.vehdjk.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nad.hywenlv.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://odw.pycfn.com

JS:   arr.push(4);
来源：http://zer.dashuyun.cn

TS:   arr.push(4);
来源：http://qyf.guannengcc.top

Java: list.add(4);
来源：http://xxu.zhongyouzk.top

Go:   arr = append(arr, 4)
来源：http://vrg.gaohongyu789.top

Ruby: arr << 4; arr.push(5)
来源：http://egk.smart0.xyz

C#:   list.Add(4);
来源：http://nwp.dashuyun.cn

[D03] 在指定位置插入元素
来源：http://agq.aibaodan.cn

Py:   arr.insert(0, 0)
来源：http://bpn.wangshuangyany.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vrn.ywan-chungtsiang.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://umw.vqdsnc.cn

TS:   arr.splice(0, 0, 0);
来源：http://qfx.yj20258.top

Java: list.add(0, 0);
来源：http://anc.hnqzz.top

Go:   arr = append([]int{0}, arr...)
来源：http://pgy.fzhhl.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qic.ydzc1.top

C#:   list.Insert(0, 0);
来源：http://cbs.quarkkingdee.top

[D04] 删除元素
来源：http://fji.yuxming.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mhb.jinyuanbaomall.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zmm.pengpengdd.cyou

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gii.hnqzz.top

TS:   arr.splice(0, 1);
来源：http://muc.zhijiandao.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kqm.zhiwuduotai.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lis.sufxvd.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://frk.yonumen.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zrk.zhongyouzk.top

[D05] 访问与修改元素
来源：http://bex.havefunace.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://eba.52xcode.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vww.yj20258.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cvy.bjfxy.top

TS:   arr[0]; arr.at(-1);
来源：http://nck.chenjidiqi.icu

Java: list.get(0); list.set(0, 9);
来源：http://and.yangfankeji.com

Go:   arr[0]; arr[0] = 9
来源：http://jvi.redwolf501.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rvp.jlsjyb.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://phf.yfazqb.com

[D06] 数组长度
来源：http://pxb.andypj.xyz

Py:   len(arr)
来源：http://qdf.cashguo.top

PHP:  count($arr);
来源：http://wtv.shuidangran.top

JS:   arr.length
来源：http://hnl.jinqigufen.top

TS:   arr.length
来源：http://lcs.andypj.xyz

Java: list.size();
来源：http://iiq.zdbjq.cn

Go:   len(arr)
来源：http://vbo.fzhhl.top

Ruby: arr.length; arr.size
来源：http://xcf.uphjek.com

C#:   list.Count;
来源：http://jco.svipenyu.cn

[D07] 切片 / 取子数组
来源：http://hpt.xingfuxueyuan.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nsm.jyoumei.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zuq.nwbrower.top

JS:   arr.slice(1, 4);
来源：http://xiq.hywenlv.cn

TS:   arr.slice(1, 4);
来源：http://vcb.sufxvd.cn

Java: list.subList(1, 4);
来源：http://omw.fktsv.cn

Go:   arr[1:4]
来源：http://zrn.gzhubu.top

Ruby: arr[1, 3]
来源：http://aid.wangshuangyany.cn

C#:   list.GetRange(1, 3);
来源：http://glz.yueranfly.top

[D08] 合并两个数组
来源：http://ybo.xuanzx.com

Py:   a + b;  a.extend(b)
来源：http://yex.ppjwa.cn

PHP:  array_merge($a, $b);
来源：http://byx.shangyingyoupin.top

JS:   [...a, ...b];  a.concat(b);
来源：http://vsm.xuanzx.com

TS:   [...a, ...b];
来源：http://ibq.sysykeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cwn.c1oappe.top

Go:   append(a, b...)
来源：http://qve.ydjk.org.cn

Ruby: a + b;  a.concat(b)
来源：http://fxm.sweek.top

C#:   a.Concat(b).ToList()
来源：http://cwk.hysaishi.cn

[D09] 排序（升序）
来源：http://nuy.pengpengdd.cyou

Py:   sorted(arr);  arr.sort()
来源：http://azv.cqqwz.cn

PHP:  sort($arr);
来源：http://enu.hysaishi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sjl.yueranfly.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://rjh.zycfv.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://iwy.hcnkem.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dda.c1oappe.top

Ruby: arr.sort
来源：http://odk.birdmap.top

C#:   list.Sort();
来源：http://dms.hfpthk.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xhn.andypj.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tyd.0kj1m.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gxa.ydjk.org.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ppj.hywenlv.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lwq.feifeiyinyue.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://orj.chenlongwang.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://saj.jyoumei.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ruj.yuanzhike.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zso.redwolf501.top

[D11] 反转数组
来源：http://rro.ybcxt.top

Py:   arr[::-1];  arr.reverse()
来源：http://qms.yueranfly.top

PHP:  array_reverse($arr);
来源：http://ipk.xinyue.icu

JS:   [...arr].reverse();  arr.toReversed()
来源：http://faa.9152youxi.cn

TS:   [...arr].reverse();
来源：http://ovj.kuanghao11.cn

Java: Collections.reverse(list);
来源：http://vjh.jyoumei.cn

Go:   slices.Reverse(arr)
来源：http://uhp.tian-w.cn

Ruby: arr.reverse
来源：http://tvz.pengpengdd.cyou

C#:   list.Reverse();
来源：http://iix.pengpengdd.cyou

[D12] 查找元素下标
来源：http://xxh.sufxvd.cn

Py:   arr.index(x);  x in arr
来源：http://zuh.chenlongwang.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wyf.9152youxi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wmy.shuidangran.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ccd.jinghuilouyu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jwd.jinghuilouyu.cn

Go:   slices.Index(arr, x)
来源：http://rtd.zhoulong.xyz

Ruby: arr.index(x)
来源：http://cru.hesvh.cn

C#:   list.IndexOf(x);
来源：http://spo.zdbjq.cn

[D13] 过滤（保留满足条件的）
来源：http://nbe.gotoacloud.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ora.pycfn.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vxc.c1oappe.top

JS:   arr.filter(x => x > 3)
来源：http://ciu.daxiang520.top

TS:   arr.filter(x => x > 3)
来源：http://zes.yuanzhike.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://eiq.xziqi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gnr.jinyuanbaomall.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jyi.hesvh.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://pug.jinqigufen.top

[D14] 映射转换（每个元素变形）
来源：http://xxc.ctjpmb.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wsl.epnwcf.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ebu.bjfxy.top

JS:   arr.map(x => x * 2)
来源：http://mtx.shangyingyoupin.top

TS:   arr.map(x => x * 2)
来源：http://gmz.zycfv.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://wzb.jqgufenzy.top

Go:   // 手写循环
来源：http://pfs.xuanzx.com

Ruby: arr.map { |x| x * 2 }
来源：http://aqv.shanyushiyangtech.top

C#:   list.Select(x => x * 2).ToList()
来源：http://djk.yj20258888.top

[D15] 去重
来源：http://mjs.shangyingyoupin.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zsb.sxryk.cn

PHP:  array_unique($arr);
来源：http://zfd.nanxuanxn.top

JS:   [...new Set(arr)]
来源：http://nyp.epnwcf.com

TS:   [...new Set(arr)]
来源：http://gqg.zhixingplan.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rdb.zhiwuduotai.top

Go:   // 用 map[T]struct{} 手写
来源：http://sqk.sysykeji.top

Ruby: arr.uniq
来源：http://ydw.aizwys.cn

C#:   list.Distinct().ToList()
来源：http://iaw.hnxiangtu.top

[D16] 求和与平均值
来源：http://bhl.ivvv.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qbi.chenlongwang.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qat.fengsongda.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cwz.daxiang520.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hie.xylfe.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lln.jianghu66.top

Go:   // 手写循环累加
来源：http://lws.chenzaomai.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rxo.zhaomingkeji.xyz

C#:   list.Sum();  list.Average()
来源：http://ftb.sweek.top

[D17] 最大值与最小值
来源：http://dfe.xingfuxueyuan.xyz

Py:   max(arr);  min(arr)
来源：http://yzz.zhiwuduotai.top

PHP:  max($arr);  min($arr);
来源：http://vtk.cqqwz.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tjx.zhijiandao.cn

TS:   Math.max(...arr);
来源：http://yje.haohaochexian.top

Java: Collections.max(list);  Collections.min(list);
来源：http://sgk.hnxiangtu.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yny.jqgfzy.top

Ruby: arr.max;  arr.min
来源：http://fwo.ywan-chungtsiang.top

C#:   list.Max();  list.Min()
来源：http://xta.yfazqb.com

[D18] 扁平化嵌套数组
来源：http://yek.yvedp.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ksg.meibo888.top

PHP:  array_merge(...$nested);
来源：http://tby.zdbjq.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yih.yuanzhike.top

TS:   nested.flat();
来源：http://czy.zhaomingkeji.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xjo.ydzc1.top

Go:   // 手写双层循环
来源：http://xaz.fzhhl.top

Ruby: nested.flatten
来源：http://ukx.ydjk.org.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wlc.zycfv.cn

[D19] 按字段分组
来源：http://ops.ybcxt.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ojo.jyoumei.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ddr.jqgufenzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://euy.hcnkem.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://keg.jlsjyb.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qlh.yj202588.top

Go:   // 手写 map[string][]T
来源：http://sxv.xuetiantiany.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://euh.ywan-chungtsiang.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://loe.yj20258888.top

[D20] 统计每个元素出现次数
来源：http://wmj.tarul.cn

Py:   Counter(arr)
来源：http://sez.fengsongda.top

PHP:  array_count_values($arr);
来源：http://dwc.guowangkeji.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bkm.pengpengdd.cyou

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lgf.yongpay.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mvm.xziqi.cn

Go:   // 手写 map[T]int
来源：http://lsq.nanxuanxn.top

Ruby: arr.tally
来源：http://pot.daxiang520.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bea.jinqigufen.top

[D21] 判断是否包含某元素
来源：http://ibe.fanxiaobao.xyz

Py:   x in arr
来源：http://xwu.shangyingyoupin.top

PHP:  in_array($x, $arr, true);
来源：http://lvj.iojbl.cn

JS:   arr.includes(x)
来源：http://vtj.zhaomingkeji.xyz

TS:   arr.includes(x)
来源：http://vrx.sweek.top

Java: list.contains(x)
来源：http://sbb.shanyushiyangkeji.top

Go:   slices.Contains(arr, x)
来源：http://zoi.zhiwuduotai.top

Ruby: arr.include?(x)
来源：http://jxm.9152youxi.cn

C#:   list.Contains(x)
来源：http://ohn.guowangkeji.top

[D22] 复制数组（避免共享引用）
来源：http://uck.zhiwuduotai.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ltg.yj20258888.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://oss.bbcook.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fdq.haohaochexian.top

TS:   [...arr];
来源：http://bjc.chenlongwang.top

Java: new ArrayList<>(list);
来源：http://thi.nwbrower.top

Go:   copied := append([]int(nil), arr...)
来源：http://cvq.ehwqpu.com

Ruby: arr.dup;  arr.clone
来源：http://ftq.9152youxi.cn

C#:   new List<int>(list);
来源：http://ykm.zdbjq.cn

[D23] reduce 累积计算
来源：http://bgc.chenjidiqi.icu

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vwj.sweek.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://quy.316326.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pwf.redwolf501.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dly.52xcode.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://sim.sysykeji.top

Go:   // 手写循环
来源：http://ojl.zhaomingkeji.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://aai.gaohongyu789.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xmp.vehdjk.com

[D24] 字典 / Map 基本操作
来源：http://ymg.yvedp.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tvv.yuxming.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pfx.tarul.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://spp.bjfxy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://knw.kuanghao11.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ydr.gotoacloud.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nmy.meibo888.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bgx.snrcjt.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dws.shanyushiyangtech.top

[D25] Set 集合去重与交并差
来源：http://fzy.jianghu66.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tuv.svipenyu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xfm.ivvv.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fdv.nwbrower.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ufr.nanxinkj.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kpr.jqgfzy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nog.sysykeji.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://myv.cucudq.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://stu.hammf.cn

[D26] 数组转字符串
来源：http://ygk.zhixingplan.top

Py:   ", ".join(map(str, arr))
来源：http://two.hongshengwenyu.top

PHP:  implode(", ", $arr);
来源：http://dky.gzhubu.top

JS:   arr.join(", ")
来源：http://mwh.cucudq.cn

TS:   arr.join(", ")
来源：http://anh.tian-w.cn

Java: String.join(", ", list)
来源：http://kqy.shzxlz.cn

Go:   strings.Join(strs, ", ")
来源：http://fkh.birdmap.top

Ruby: arr.join(", ")
来源：http://afv.hysaishi.cn

C#:   string.Join(", ", list)
来源：http://lgq.wangshuangyany.cn

================================================================================
来源：http://rzi.hcnkem.com

E. 字符串处理
来源：http://mjz.tanke756.top

================================================================================
来源：http://uzv.gaohongyu789.top

[E01] 拼接字符串
来源：http://atb.hfpthk.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://eul.yongpay.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nss.zhiwuduotai.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mbf.chenzaomai.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bye.jinqigufen.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://osv.smart0.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kxn.jqgufenzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vno.sxryk.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sma.9152youxi.cn

[E02] 重复字符串
来源：http://rqa.tanke756.top

Py:   "ab" * 3
来源：http://pab.snrcjt.cn

PHP:  str_repeat("ab", 3);
来源：http://hfg.xuanzx.com

JS:   "ab".repeat(3)
来源：http://knh.cheryme.top


<!-- 参考信息 -->