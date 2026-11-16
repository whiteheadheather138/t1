代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://qdu.xingfuxueyuan.xyz

Ruby: -> { puts "run" }.call
来源：http://ucn.yj202588.top

C#:   // 无 IIFE：用静态构造函数
来源：http://avc.sysykeji.top

[C13] 类型声明 / 类型注解
来源：http://sgy.shangyingyoupin.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qbu.svipenyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://omb.svipenyu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hqo.dashuyun.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pew.aibaodan.cn

Java: int add(int a, int b) { return a + b; }
来源：http://rrl.pycfn.com

Go:   func add(a, b int) int
来源：http://laj.zhoulong.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ngx.gaohongyu789.top

C#:   int Add(int a, int b) => a + b;
来源：http://lsy.smart0.xyz

[C14] 泛型函数
来源：http://qfd.fktsv.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tko.fktsv.cn

PHP:  // 无泛型
来源：http://mbk.ivvv.top

JS:   // 无泛型
来源：http://fgi.zhiwuduotai.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cfq.c1oappe.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rky.hysaishi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lyi.nwbrower.top

Ruby: # 无泛型
来源：http://yui.shuidangran.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dbw.9152youxi.cn

[C15] 解构 / 展开参数
来源：http://gdw.sweek.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jgo.sjlbkw.cn

PHP:  [$a, $b] = $pair;
来源：http://jhs.zhiwuduotai.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wva.zycfv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vjg.cdnleiting.top

Java: // 无解构
来源：http://hur.mhx1999.top

Go:   // 无解构
来源：http://qnl.yonumen.top

Ruby: a, b = pair
来源：http://ivz.uphjek.com

C#:   var (a, b) = pair;
来源：http://hpo.ydjk.org.cn

[C16] 函数 / 方法重载
来源：http://oxp.yueranfly.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ccy.jinqigfzy.top

PHP:  // 无重载
来源：http://ukr.ydzc1.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://fef.hongshengwenyu.top

TS:   // 用联合类型或重载签名声明
来源：http://xxw.daxiang520.top

Java: void f(int a) {}  void f(String a) {}
来源：http://pjp.tarul.cn

Go:   // 无重载：用不同函数名
来源：http://qmf.daria6918.cn

Ruby: # 无重载：靠动态参数
来源：http://nmt.chenzaomai.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://ajc.gzhubu.top

================================================================================
来源：http://loy.jinqigufen.top

D. 数组 / 列表 / 集合
来源：http://mtb.yangfankeji.com

================================================================================
来源：http://yhg.dashuyun.cn

[D01] 创建数组 / 列表
来源：http://eom.havefunace.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://phg.chenzaomai.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ozg.hongshengwenyu.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kab.dianchejie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ygy.52xcode.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://oay.daria6918.cn

Go:   arr := []int{1, 2, 3}
来源：http://bbm.xinyue.icu

Ruby: arr = [1, 2, 3]
来源：http://tpj.feifeiyinyue.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ygf.shangyingyoupin.top

[D02] 追加元素到末尾
来源：http://bnu.cdnleiting.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hge.aizwys.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yvp.shzxlz.cn

JS:   arr.push(4);
来源：http://ykc.nanxuanxn.top

TS:   arr.push(4);
来源：http://trp.ydjk.org.cn

Java: list.add(4);
来源：http://vwl.guannengcc.top

Go:   arr = append(arr, 4)
来源：http://xzf.yanxiufei.cn

Ruby: arr << 4; arr.push(5)
来源：http://uam.zhiwuduotai.top

C#:   list.Add(4);
来源：http://yaq.yueranfly.top

[D03] 在指定位置插入元素
来源：http://wbm.hesvh.cn

Py:   arr.insert(0, 0)
来源：http://wmq.fanxiaobao.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lmr.epnwcf.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dbc.xingfuxueyuan.xyz

TS:   arr.splice(0, 0, 0);
来源：http://eph.jinyuanbaomall.cn

Java: list.add(0, 0);
来源：http://xvd.pengpengdd.cyou

Go:   arr = append([]int{0}, arr...)
来源：http://npk.meibo888.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wuq.andypj.xyz

C#:   list.Insert(0, 0);
来源：http://vgu.mhx1999.top

[D04] 删除元素
来源：http://irr.zdbjq.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://syp.pycfn.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xft.cheryme.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yry.xylfe.cn

TS:   arr.splice(0, 1);
来源：http://vvo.sysykeji.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://oar.fzhhl.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://orn.aibaodan.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ffg.tanke756.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zqq.iojbl.cn

[D05] 访问与修改元素
来源：http://ayf.tianlin.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://efk.gaohongyu789.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tdz.mhx1999.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bhn.jinghuilouyu.cn

TS:   arr[0]; arr.at(-1);
来源：http://gcd.xingfuxueyuan.xyz

Java: list.get(0); list.set(0, 9);
来源：http://tbe.fengsongda.top

Go:   arr[0]; arr[0] = 9
来源：http://bwk.ydjk.org.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://boy.52xcode.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://aci.xylfe.cn

[D06] 数组长度
来源：http://yth.pycfn.com

Py:   len(arr)
来源：http://dvi.fengsongda.top

PHP:  count($arr);
来源：http://fgi.tianlin.xyz

JS:   arr.length
来源：http://sgz.birdmap.top

TS:   arr.length
来源：http://tcn.hywenlv.cn

Java: list.size();
来源：http://rlz.yj20258.top

Go:   len(arr)
来源：http://aur.shzxlz.cn

Ruby: arr.length; arr.size
来源：http://klm.xuetiantiany.cn

C#:   list.Count;
来源：http://quy.9152youxi.cn

[D07] 切片 / 取子数组
来源：http://kvd.hysaishi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cts.zhaomingkeji.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://vud.jiagoushi.top

JS:   arr.slice(1, 4);
来源：http://abg.zhixingplan.top

TS:   arr.slice(1, 4);
来源：http://wbd.ywan-chungtsiang.top

Java: list.subList(1, 4);
来源：http://tmv.sweek.top

Go:   arr[1:4]
来源：http://pox.jinyuanbaomall.cn

Ruby: arr[1, 3]
来源：http://fgi.chenlongwang.top

C#:   list.GetRange(1, 3);
来源：http://vft.hesvh.cn

[D08] 合并两个数组
来源：http://bqy.haohaochexian.top

Py:   a + b;  a.extend(b)
来源：http://eor.smart0.xyz

PHP:  array_merge($a, $b);
来源：http://kap.wangdashe.top

JS:   [...a, ...b];  a.concat(b);
来源：http://jwd.shuidangran.top

TS:   [...a, ...b];
来源：http://uet.feifeiyinyue.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hlx.guowangkeji.top

Go:   append(a, b...)
来源：http://cwu.fanxiaobao.xyz

Ruby: a + b;  a.concat(b)
来源：http://ujx.shuidangran.top

C#:   a.Concat(b).ToList()
来源：http://ahy.ybcxt.top

[D09] 排序（升序）
来源：http://kkh.dianchejie.cn

Py:   sorted(arr);  arr.sort()
来源：http://vsf.cdnleiting.top

PHP:  sort($arr);
来源：http://muu.jlsjyb.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://foq.sysykeji.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://qfe.yueranfly.top

Java: Collections.sort(list);  list.sort(null);
来源：http://oey.hcnkem.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ysr.guowangkeji.top

Ruby: arr.sort
来源：http://cio.feifeiyinyue.top

C#:   list.Sort();
来源：http://mgk.wangdashe.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://xxs.yanxiufei.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ewe.bbcook.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://miu.jqgufenzy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wvf.ydzc1.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kzm.xuetiantiany.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qcb.fzhhl.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lgx.fengsongda.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mec.jinyuanbaomall.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://olk.yj20258.top

[D11] 反转数组
来源：http://zuo.hnqzz.top

Py:   arr[::-1];  arr.reverse()
来源：http://cwi.tanke756.top

PHP:  array_reverse($arr);
来源：http://xnj.guowangkeji.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://oud.jqgfzy.top

TS:   [...arr].reverse();
来源：http://msu.ydzc1.top

Java: Collections.reverse(list);
来源：http://zgu.cheryme.top

Go:   slices.Reverse(arr)
来源：http://oia.mhx1999.top

Ruby: arr.reverse
来源：http://ovm.nwbrower.top

C#:   list.Reverse();
来源：http://oku.ctjpmb.com

[D12] 查找元素下标
来源：http://bao.pengpengdd.cyou

Py:   arr.index(x);  x in arr
来源：http://fns.fehbvm.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mfw.chenzaomai.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://apt.jinyuanbaomall.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gpg.shangyingyoupin.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rja.zhongyouzk.top

Go:   slices.Index(arr, x)
来源：http://dws.fktsv.cn

Ruby: arr.index(x)
来源：http://rko.vehdjk.com

C#:   list.IndexOf(x);
来源：http://kws.jlsjyb.cn

[D13] 过滤（保留满足条件的）
来源：http://shj.vehdjk.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://his.birdmap.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nhw.jinyuanbaomall.cn

JS:   arr.filter(x => x > 3)
来源：http://svl.redwolf501.top

TS:   arr.filter(x => x > 3)
来源：http://hqu.ivvv.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gsd.gzhubu.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jur.hcnkem.com

Ruby: arr.select { |x| x > 3 }
来源：http://ddt.yj20258888.top

C#:   list.Where(x => x > 3).ToList()
来源：http://slv.iojbl.cn

[D14] 映射转换（每个元素变形）
来源：http://diw.shzxlz.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wey.dashuyun.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sem.cqqwz.cn

JS:   arr.map(x => x * 2)
来源：http://aeq.aibaodan.cn

TS:   arr.map(x => x * 2)
来源：http://gic.gzhubu.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://hzp.gzhubu.top

Go:   // 手写循环
来源：http://ccj.guowangkeji.top

Ruby: arr.map { |x| x * 2 }
来源：http://wjg.jinyuanbaomall.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pwd.hfpthk.cn

[D15] 去重
来源：http://ovb.zdqjudy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://frh.daxiang520.top

PHP:  array_unique($arr);
来源：http://bux.aizwys.cn

JS:   [...new Set(arr)]
来源：http://hew.chenlongwang.top

TS:   [...new Set(arr)]
来源：http://jqw.xingfuxueyuan.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zis.dashuyun.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xjm.tian-w.cn

Ruby: arr.uniq
来源：http://ehk.jlsjyb.cn

C#:   list.Distinct().ToList()
来源：http://iza.mhx1999.top

[D16] 求和与平均值
来源：http://vrt.guannengcc.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fhu.zhaomingkeji.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nmu.xylfe.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://szp.pengpengdd.cyou

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pkk.jinyuanbaomall.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://avp.hesvh.cn

Go:   // 手写循环累加
来源：http://sjl.jinghuilouyu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lyv.hammf.cn

C#:   list.Sum();  list.Average()
来源：http://tfx.ehwqpu.com

[D17] 最大值与最小值
来源：http://den.jiagoushi.top

Py:   max(arr);  min(arr)
来源：http://qlo.hywenlv.cn

PHP:  max($arr);  min($arr);
来源：http://rzo.jinyuanbaomall.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tji.vehdjk.com

TS:   Math.max(...arr);
来源：http://bfy.chenzaomai.com

Java: Collections.max(list);  Collections.min(list);
来源：http://dtr.jyoumei.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gst.jiagoushi.top

Ruby: arr.max;  arr.min
来源：http://bjw.guannengcc.top

C#:   list.Max();  list.Min()
来源：http://xyx.xinyue.icu

[D18] 扁平化嵌套数组
来源：http://lxs.ybcxt.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ylt.redwolf501.top

PHP:  array_merge(...$nested);
来源：http://khe.chenzaomai.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mai.guowangkeji.top

TS:   nested.flat();
来源：http://ios.tianlin.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://waq.hammf.cn

Go:   // 手写双层循环
来源：http://ylv.xylfe.cn

Ruby: nested.flatten
来源：http://vcn.jinqigfzy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://icg.chenjidiqi.icu

[D19] 按字段分组
来源：http://kkl.shanyushiyangtech.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://col.hywenlv.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://war.chenlongwang.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yuu.mhx1999.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://nwk.zhoulong.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hwx.jyoumei.cn

Go:   // 手写 map[string][]T
来源：http://kki.yuanzhike.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://mwv.mhx1999.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://btu.yonumen.top

[D20] 统计每个元素出现次数
来源：http://yxa.tanke756.top

Py:   Counter(arr)
来源：http://wmx.jyoumei.cn

PHP:  array_count_values($arr);
来源：http://ynb.feifeiyinyue.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nig.feifeiyinyue.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://grc.daxiang520.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ocl.tian-w.cn

Go:   // 手写 map[T]int
来源：http://iih.hesvh.cn

Ruby: arr.tally
来源：http://lej.yj20258.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rgb.dianchejie.cn

[D21] 判断是否包含某元素
来源：http://rhm.chenjidiqi.icu

Py:   x in arr
来源：http://twr.xuetiantiany.cn

PHP:  in_array($x, $arr, true);
来源：http://tkr.xuetiantiany.cn

JS:   arr.includes(x)
来源：http://chr.hnxiangtu.top

TS:   arr.includes(x)
来源：http://lic.xuetiantiany.cn

Java: list.contains(x)
来源：http://jwv.fanxiaobao.xyz

Go:   slices.Contains(arr, x)
来源：http://llz.havefunace.top

Ruby: arr.include?(x)
来源：http://acc.nwbrower.top

C#:   list.Contains(x)
来源：http://pqa.gotoacloud.top

[D22] 复制数组（避免共享引用）
来源：http://hle.shzxlz.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ifi.zhijiandao.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://akn.sufxvd.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pwf.mhx1999.top

TS:   [...arr];
来源：http://tsn.yj20258.top

Java: new ArrayList<>(list);
来源：http://wld.meibo888.top

Go:   copied := append([]int(nil), arr...)
来源：http://she.zhongyouzk.top

Ruby: arr.dup;  arr.clone
来源：http://mdr.cucudq.cn

C#:   new List<int>(list);
来源：http://fsu.ehwqpu.com

[D23] reduce 累积计算
来源：http://yly.sysykeji.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xab.yueranfly.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mrc.yuxming.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://guz.ehwqpu.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://que.aibaodan.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://gqw.zhoulong.xyz

Go:   // 手写循环
来源：http://dpf.zycfv.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wuk.zhijiandao.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://orx.jyoumei.cn

[D24] 字典 / Map 基本操作
来源：http://wba.nwbrower.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lje.jqgufenzy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sww.hcnkem.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tkb.0kj1m.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ytj.aibaodan.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://oex.tanke756.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sos.jinyuanbaomall.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mmg.sjlbkw.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hnq.yuxming.cn

[D25] Set 集合去重与交并差
来源：http://rfx.feifeiyinyue.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tcj.xinyue.icu

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ysz.ehwqpu.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mxd.c1oappe.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rkf.redwolf501.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qok.hongshengwenyu.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hxt.fzhhl.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gpp.0kj1m.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nps.nanxuanxn.top

[D26] 数组转字符串
来源：http://dlw.c1oappe.top

Py:   ", ".join(map(str, arr))
来源：http://kyn.yongpay.top

PHP:  implode(", ", $arr);
来源：http://ing.aizwys.cn

JS:   arr.join(", ")
来源：http://iie.snrcjt.cn

TS:   arr.join(", ")
来源：http://qfx.52xcode.cn

Java: String.join(", ", list)
来源：http://kno.jinqigufen.top

Go:   strings.Join(strs, ", ")
来源：http://rsg.xinyue.icu

Ruby: arr.join(", ")
来源：http://bzk.wangshuangyany.cn

C#:   string.Join(", ", list)
来源：http://zfn.havefunace.top

================================================================================
来源：http://oyn.bjfxy.top

E. 字符串处理
来源：http://ppc.vehdjk.com

================================================================================
来源：http://lrf.yvedp.cn

[E01] 拼接字符串
来源：http://fys.havefunace.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dom.gogol.net.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wwf.ybcxt.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qfg.fktsv.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kul.svipenyu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fuj.yvedp.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vmf.dashuyun.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jnv.tanke756.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gfg.xziqi.cn

[E02] 重复字符串
来源：http://vln.gzhubu.top

Py:   "ab" * 3
来源：http://elb.cucudq.cn

PHP:  str_repeat("ab", 3);
来源：http://tfm.nwbrower.top

JS:   "ab".repeat(3)
来源：http://eba.yanxiufei.cn

TS:   "ab".repeat(3)
来源：http://zxe.chenzaomai.com

Java: "ab".repeat(3)
来源：http://utg.xingfuxueyuan.xyz

Go:   strings.Repeat("ab", 3)
来源：http://ygk.ydzc1.top

Ruby: "ab" * 3
来源：http://ytd.wangshuangyany.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vzt.cdnleiting.top

[E03] 截取子串
来源：http://onk.pengpengdd.cyou

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jcm.cdnleiting.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ztl.jqgfzy.top


<!-- 参考信息 -->