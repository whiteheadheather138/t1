代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://upw.ehwqpu.com

JS:   (() => { console.log("run"); })();
来源：http://ryk.gzhubu.top

TS:   (() => { console.log("run"); })();
来源：http://zfs.chenzaomai.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hsk.9152youxi.cn

Go:   func() { fmt.Println("run") }()
来源：http://tsc.shanyushiyangkeji.top

Ruby: -> { puts "run" }.call
来源：http://zon.cheryme.top

C#:   // 无 IIFE：用静态构造函数
来源：http://dsc.fzhhl.top

[C13] 类型声明 / 类型注解
来源：http://qxr.yueranfly.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ecj.wangshuangyany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nsz.ybcxt.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wbc.chenzaomai.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mcs.sufxvd.cn

Java: int add(int a, int b) { return a + b; }
来源：http://nxw.jyoumei.cn

Go:   func add(a, b int) int
来源：http://apo.0kj1m.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wqk.zhengqikj.top

C#:   int Add(int a, int b) => a + b;
来源：http://ygb.gogol.net.cn

[C14] 泛型函数
来源：http://uis.hongshengwenyu.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pag.ywan-chungtsiang.top

PHP:  // 无泛型
来源：http://pzm.haohaochexian.top

JS:   // 无泛型
来源：http://dae.cheryme.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vqt.shangyingyoupin.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ced.wangdashe.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zjy.cashguo.top

Ruby: # 无泛型
来源：http://jnv.pengpengdd.cyou

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jhb.yanxiufei.cn

[C15] 解构 / 展开参数
来源：http://byd.cashguo.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://khg.shanyushiyangtech.top

PHP:  [$a, $b] = $pair;
来源：http://hiz.xingfuxueyuan.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://brp.mhx1999.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ahj.bjfxy.top

Java: // 无解构
来源：http://yey.sysykeji.top

Go:   // 无解构
来源：http://cus.ehwqpu.com

Ruby: a, b = pair
来源：http://eyo.cucudq.cn

C#:   var (a, b) = pair;
来源：http://uel.ppjwa.cn

[C16] 函数 / 方法重载
来源：http://ipy.jyoumei.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rdo.daria6918.cn

PHP:  // 无重载
来源：http://pdq.kuanghao11.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://sgc.pycfn.com

TS:   // 用联合类型或重载签名声明
来源：http://zfb.vehdjk.com

Java: void f(int a) {}  void f(String a) {}
来源：http://xup.kuanghao11.cn

Go:   // 无重载：用不同函数名
来源：http://jsq.tian-w.cn

Ruby: # 无重载：靠动态参数
来源：http://zmk.zhiwuduotai.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://lpn.shanyushiyangkeji.top

================================================================================
来源：http://bok.iojbl.cn

D. 数组 / 列表 / 集合
来源：http://pqb.mhx1999.top

================================================================================
来源：http://mie.tarul.cn

[D01] 创建数组 / 列表
来源：http://hpi.zdqjudy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://bko.tian-w.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ppy.zhoulong.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://opt.daxiang520.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://yjp.yueranfly.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sab.yuxming.cn

Go:   arr := []int{1, 2, 3}
来源：http://ril.nwbrower.top

Ruby: arr = [1, 2, 3]
来源：http://ljh.gaohongyu789.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yrr.zhongyouzk.top

[D02] 追加元素到末尾
来源：http://nqx.ydzc1.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://aib.chenlongwang.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kjk.yuanzhike.top

JS:   arr.push(4);
来源：http://czm.guowangkeji.top

TS:   arr.push(4);
来源：http://agz.shuidangran.top

Java: list.add(4);
来源：http://dyf.uphjek.com

Go:   arr = append(arr, 4)
来源：http://myw.nanxinkj.top

Ruby: arr << 4; arr.push(5)
来源：http://ukp.yj202588.top

C#:   list.Add(4);
来源：http://glm.dashuyun.cn

[D03] 在指定位置插入元素
来源：http://una.jinghuilouyu.cn

Py:   arr.insert(0, 0)
来源：http://mie.yueranfly.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://sjl.zhengqikj.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ylz.zycfv.cn

TS:   arr.splice(0, 0, 0);
来源：http://vwb.nwbrower.top

Java: list.add(0, 0);
来源：http://qwl.shanyushiyangkeji.top

Go:   arr = append([]int{0}, arr...)
来源：http://ckr.shangyingyoupin.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fyx.pengpengdd.cyou

C#:   list.Insert(0, 0);
来源：http://icj.hcnkem.com

[D04] 删除元素
来源：http://imc.jinyuanbaomall.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uby.9152youxi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mtz.jyoumei.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pjq.chenlongwang.top

TS:   arr.splice(0, 1);
来源：http://uxk.yj20258.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ezz.cdnleiting.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://klg.yvedp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ujp.dashuyun.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hne.vqdsnc.cn

[D05] 访问与修改元素
来源：http://isa.uphjek.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://oyr.jiagoushi.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qam.zhiwuduotai.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xen.cucudq.cn

TS:   arr[0]; arr.at(-1);
来源：http://jhm.nanxinkj.top

Java: list.get(0); list.set(0, 9);
来源：http://etu.sufxvd.cn

Go:   arr[0]; arr[0] = 9
来源：http://ivs.yj202588.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zcq.gzhubu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wpu.zhoulong.xyz

[D06] 数组长度
来源：http://xpi.chenjidiqi.icu

Py:   len(arr)
来源：http://acd.shanyushiyangkeji.top

PHP:  count($arr);
来源：http://nez.fengsongda.top

JS:   arr.length
来源：http://tjy.guannengcc.top

TS:   arr.length
来源：http://osw.bjfxy.top

Java: list.size();
来源：http://ptc.zycfv.cn

Go:   len(arr)
来源：http://thr.cashguo.top

Ruby: arr.length; arr.size
来源：http://hzd.fanxiaobao.xyz

C#:   list.Count;
来源：http://cuc.zhaomingkeji.xyz

[D07] 切片 / 取子数组
来源：http://qln.uphjek.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lsu.pengpengdd.cyou

PHP:  array_slice($arr, 1, 3);
来源：http://rhf.chenzaomai.com

JS:   arr.slice(1, 4);
来源：http://utu.yangfankeji.com

TS:   arr.slice(1, 4);
来源：http://smm.daxiang520.top

Java: list.subList(1, 4);
来源：http://cmg.hcnkem.com

Go:   arr[1:4]
来源：http://pyn.nanxuanxn.top

Ruby: arr[1, 3]
来源：http://tul.vqdsnc.cn

C#:   list.GetRange(1, 3);
来源：http://lmo.ybcxt.top

[D08] 合并两个数组
来源：http://ofh.yvedp.cn

Py:   a + b;  a.extend(b)
来源：http://duo.andypj.xyz

PHP:  array_merge($a, $b);
来源：http://zsd.zhaomingkeji.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://nrh.kuanghao11.cn

TS:   [...a, ...b];
来源：http://gdy.zhoulong.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hns.jianghu66.top

Go:   append(a, b...)
来源：http://mon.zhijiandao.cn

Ruby: a + b;  a.concat(b)
来源：http://sxd.snrcjt.cn

C#:   a.Concat(b).ToList()
来源：http://pjf.vqdsnc.cn

[D09] 排序（升序）
来源：http://vyy.52xcode.cn

Py:   sorted(arr);  arr.sort()
来源：http://ezz.ywan-chungtsiang.top

PHP:  sort($arr);
来源：http://ypg.shanyushiyangkeji.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rti.xziqi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hwy.redwolf501.top

Java: Collections.sort(list);  list.sort(null);
来源：http://btj.daxiang520.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dnx.shangyingyoupin.top

Ruby: arr.sort
来源：http://fna.sweek.top

C#:   list.Sort();
来源：http://esl.xuanzx.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://qqn.iojbl.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gsb.andypj.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tyj.vehdjk.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rze.jinghuilouyu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kab.zhaomingkeji.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pyc.aibaodan.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yud.nanxuanxn.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://iax.chenjidiqi.icu

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ovk.fzhhl.top

[D11] 反转数组
来源：http://xpp.dianchejie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://kzx.52xcode.cn

PHP:  array_reverse($arr);
来源：http://tha.ctjpmb.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cic.hnxiangtu.top

TS:   [...arr].reverse();
来源：http://dtp.xuanzx.com

Java: Collections.reverse(list);
来源：http://mag.mhx1999.top

Go:   slices.Reverse(arr)
来源：http://wxu.dianchejie.cn

Ruby: arr.reverse
来源：http://mvq.yj20258.top

C#:   list.Reverse();
来源：http://jib.jinyuanbaomall.cn

[D12] 查找元素下标
来源：http://hrp.jiagoushi.top

Py:   arr.index(x);  x in arr
来源：http://kun.snrcjt.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tvg.uphjek.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hfw.chenzaomai.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uuo.tarul.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://iyp.sjlbkw.cn

Go:   slices.Index(arr, x)
来源：http://iux.hnxiangtu.top

Ruby: arr.index(x)
来源：http://lax.dashuyun.cn

C#:   list.IndexOf(x);
来源：http://jas.tianlin.xyz

[D13] 过滤（保留满足条件的）
来源：http://dqh.jlsjyb.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://axc.tarul.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kmf.cheryme.top

JS:   arr.filter(x => x > 3)
来源：http://iuu.c1oappe.top

TS:   arr.filter(x => x > 3)
来源：http://uva.0kj1m.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vfm.shangyingyoupin.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dgs.0kj1m.cn

Ruby: arr.select { |x| x > 3 }
来源：http://pic.sysykeji.top

C#:   list.Where(x => x > 3).ToList()
来源：http://rur.pengpengdd.cyou

[D14] 映射转换（每个元素变形）
来源：http://ipj.shzxlz.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hyb.ivvv.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xvk.zhiwuduotai.top

JS:   arr.map(x => x * 2)
来源：http://tef.xinyue.icu

TS:   arr.map(x => x * 2)
来源：http://uah.ydjk.org.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://nhr.xylfe.cn

Go:   // 手写循环
来源：http://cbz.bbcook.cn

Ruby: arr.map { |x| x * 2 }
来源：http://uvr.epnwcf.com

C#:   list.Select(x => x * 2).ToList()
来源：http://szn.cdnleiting.top

[D15] 去重
来源：http://hva.hnxiangtu.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vyg.pengpengdd.cyou

PHP:  array_unique($arr);
来源：http://vkh.yvedp.cn

JS:   [...new Set(arr)]
来源：http://evb.yvedp.cn

TS:   [...new Set(arr)]
来源：http://yvz.fanxiaobao.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pvi.cucudq.cn

Go:   // 用 map[T]struct{} 手写
来源：http://aup.fehbvm.com

Ruby: arr.uniq
来源：http://jwg.bjfxy.top

C#:   list.Distinct().ToList()
来源：http://sxe.gzhubu.top

[D16] 求和与平均值
来源：http://yne.vehdjk.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cle.bbcook.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://aga.jlsjyb.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dgy.xziqi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://crj.sufxvd.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qpn.hammf.cn

Go:   // 手写循环累加
来源：http://bnz.jinghuilouyu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rtj.haohaochexian.top

C#:   list.Sum();  list.Average()
来源：http://acf.redwolf501.top

[D17] 最大值与最小值
来源：http://znw.fehbvm.com

Py:   max(arr);  min(arr)
来源：http://ppw.hnqzz.top

PHP:  max($arr);  min($arr);
来源：http://ssq.smart0.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ekg.aizwys.cn

TS:   Math.max(...arr);
来源：http://ojy.jinqigfzy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://paf.vqdsnc.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xfj.havefunace.top

Ruby: arr.max;  arr.min
来源：http://phw.zhixingplan.top

C#:   list.Max();  list.Min()
来源：http://ric.iojbl.cn

[D18] 扁平化嵌套数组
来源：http://pxt.xuetiantiany.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dty.yuanzhike.top

PHP:  array_merge(...$nested);
来源：http://lbv.dianchejie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jbe.wangshuangyany.cn

TS:   nested.flat();
来源：http://fzm.xziqi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hep.kuanghao11.cn

Go:   // 手写双层循环
来源：http://lrj.zdqjudy.top

Ruby: nested.flatten
来源：http://ecp.shanyushiyangtech.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://rsr.gogol.net.cn

[D19] 按字段分组
来源：http://cht.xinyue.icu

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://omk.fanxiaobao.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://oax.nanxinkj.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://btj.mhx1999.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://keh.cucudq.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ran.quarkkingdee.top

Go:   // 手写 map[string][]T
来源：http://pqh.jinqigfzy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://lem.meibo888.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://udi.haohaochexian.top

[D20] 统计每个元素出现次数
来源：http://giw.shzxlz.cn

Py:   Counter(arr)
来源：http://rpf.hongshengwenyu.top

PHP:  array_count_values($arr);
来源：http://ucs.bjfxy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://stl.yonumen.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://coy.ivvv.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qlb.shangyingyoupin.top

Go:   // 手写 map[T]int
来源：http://byq.hfpthk.cn

Ruby: arr.tally
来源：http://kuh.jyoumei.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cpx.redwolf501.top

[D21] 判断是否包含某元素
来源：http://slx.yuxming.cn

Py:   x in arr
来源：http://kmm.uphjek.com

PHP:  in_array($x, $arr, true);
来源：http://sfl.tianlin.xyz

JS:   arr.includes(x)
来源：http://swz.9152youxi.cn

TS:   arr.includes(x)
来源：http://fqt.fanxiaobao.xyz

Java: list.contains(x)
来源：http://jyz.jinyuanbaomall.cn

Go:   slices.Contains(arr, x)
来源：http://fva.tarul.cn

Ruby: arr.include?(x)
来源：http://jqa.sjlbkw.cn

C#:   list.Contains(x)
来源：http://mxi.hesvh.cn

[D22] 复制数组（避免共享引用）
来源：http://gog.zdbjq.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://exm.jqgfzy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://axv.jinqigfzy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gwz.aizwys.cn

TS:   [...arr];
来源：http://pws.shanyushiyangtech.top

Java: new ArrayList<>(list);
来源：http://fyw.jinqigufen.top

Go:   copied := append([]int(nil), arr...)
来源：http://cpy.yuanzhike.top

Ruby: arr.dup;  arr.clone
来源：http://ion.tianlin.xyz

C#:   new List<int>(list);
来源：http://fah.yongpay.top

[D23] reduce 累积计算
来源：http://ysg.tanke756.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kkh.yangfankeji.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uaa.cheryme.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uah.gzhubu.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dtt.fzhhl.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://fmf.zhixingplan.top

Go:   // 手写循环
来源：http://hkf.andypj.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zxo.dashuyun.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qgx.shuidangran.top

[D24] 字典 / Map 基本操作
来源：http://fwx.hesvh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gmi.feifeiyinyue.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qes.ydzc1.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ijj.yj20258.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tqo.dashuyun.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bwx.hnqzz.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cby.chenjidiqi.icu

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nsb.sjlbkw.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ure.tianlin.xyz

[D25] Set 集合去重与交并差
来源：http://ctq.aizwys.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wed.tianlin.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wpy.daxiang520.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qkp.jlsjyb.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blk.zhoulong.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cfa.uphjek.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xxs.yuxming.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://imt.ehwqpu.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://foj.sysykeji.top

[D26] 数组转字符串
来源：http://bun.zhiwuduotai.top

Py:   ", ".join(map(str, arr))
来源：http://qfc.pengpengdd.cyou

PHP:  implode(", ", $arr);
来源：http://ksq.xziqi.cn

JS:   arr.join(", ")
来源：http://pfd.fktsv.cn

TS:   arr.join(", ")
来源：http://vrc.meibo888.top

Java: String.join(", ", list)
来源：http://zvs.ivvv.top

Go:   strings.Join(strs, ", ")
来源：http://oxt.bjfxy.top

Ruby: arr.join(", ")
来源：http://vgv.yj202588.top

C#:   string.Join(", ", list)
来源：http://szp.cdnleiting.top

================================================================================
来源：http://ivh.chenlongwang.top

E. 字符串处理
来源：http://bzs.zhengqikj.top

================================================================================
来源：http://gln.shanyushiyangkeji.top

[E01] 拼接字符串
来源：http://kxh.yj20258888.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hba.xingfuxueyuan.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wrz.jlsjyb.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pcc.yongpay.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://uzb.yongpay.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://maj.feifeiyinyue.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://otp.yueranfly.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cfc.zdbjq.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gqi.shanyushiyangtech.top

[E02] 重复字符串
来源：http://bqy.shzxlz.cn

Py:   "ab" * 3
来源：http://out.xuanzx.com

PHP:  str_repeat("ab", 3);
来源：http://oep.hesvh.cn

JS:   "ab".repeat(3)
来源：http://rmj.zhoulong.xyz

TS:   "ab".repeat(3)
来源：http://iwe.shanyushiyangkeji.top

Java: "ab".repeat(3)
来源：http://xtl.ydzc1.top

Go:   strings.Repeat("ab", 3)
来源：http://juf.zdqjudy.top

Ruby: "ab" * 3
来源：http://qej.xinyue.icu


<!-- 参考信息 -->