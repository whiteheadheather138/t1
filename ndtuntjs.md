代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pgq.zhaomingkeji.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://awg.xylfe.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pta.sufxvd.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://axs.zhaomingkeji.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://ckm.sufxvd.cn

Go:   func add(a, b int) int
来源：http://qhq.zhijiandao.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fky.316326.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://lap.yj20258888.top

[C14] 泛型函数
来源：http://avg.gotoacloud.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gwd.jinqigufen.top

PHP:  // 无泛型
来源：http://aoz.smart0.xyz

JS:   // 无泛型
来源：http://tjq.yangfankeji.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zkr.zycfv.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uea.yj20258.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://eex.chenjidiqi.icu

Ruby: # 无泛型
来源：http://sgm.gaohongyu789.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://uya.haohaochexian.top

[C15] 解构 / 展开参数
来源：http://vqx.jianghu66.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gtm.xylfe.cn

PHP:  [$a, $b] = $pair;
来源：http://odq.yangfankeji.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://egb.shuidangran.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://eol.meibo888.top

Java: // 无解构
来源：http://opn.chenjidiqi.icu

Go:   // 无解构
来源：http://ves.shzxlz.cn

Ruby: a, b = pair
来源：http://wpu.hnxiangtu.top

C#:   var (a, b) = pair;
来源：http://vdy.zhongyouzk.top

[C16] 函数 / 方法重载
来源：http://oua.aibaodan.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://env.daxiang520.top

PHP:  // 无重载
来源：http://mur.yuanzhike.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://kkk.pycfn.com

TS:   // 用联合类型或重载签名声明
来源：http://xhd.fengsongda.top

Java: void f(int a) {}  void f(String a) {}
来源：http://veb.cqqwz.cn

Go:   // 无重载：用不同函数名
来源：http://upj.wangshuangyany.cn

Ruby: # 无重载：靠动态参数
来源：http://xsr.ybcxt.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ian.yonumen.top

================================================================================
来源：http://oyt.cdnleiting.top

D. 数组 / 列表 / 集合
来源：http://lqp.shuidangran.top

================================================================================
来源：http://seb.gzhubu.top

[D01] 创建数组 / 列表
来源：http://qwr.xuetiantiany.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zoi.vqdsnc.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wcs.sweek.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://smp.quarkkingdee.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ixg.xylfe.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bgx.wangshuangyany.cn

Go:   arr := []int{1, 2, 3}
来源：http://hmb.redwolf501.top

Ruby: arr = [1, 2, 3]
来源：http://ycz.smart0.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://atk.wangshuangyany.cn

[D02] 追加元素到末尾
来源：http://qbi.gzhubu.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hvy.bjfxy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tau.uphjek.com

JS:   arr.push(4);
来源：http://gmo.svipenyu.cn

TS:   arr.push(4);
来源：http://rig.fktsv.cn

Java: list.add(4);
来源：http://rbj.dianchejie.cn

Go:   arr = append(arr, 4)
来源：http://kni.chenjidiqi.icu

Ruby: arr << 4; arr.push(5)
来源：http://iux.ppjwa.cn

C#:   list.Add(4);
来源：http://rwv.wangshuangyany.cn

[D03] 在指定位置插入元素
来源：http://lqp.xuetiantiany.cn

Py:   arr.insert(0, 0)
来源：http://cys.fktsv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://frg.jinghuilouyu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://amn.zdqjudy.top

TS:   arr.splice(0, 0, 0);
来源：http://rgn.bjfxy.top

Java: list.add(0, 0);
来源：http://ipg.daxiang520.top

Go:   arr = append([]int{0}, arr...)
来源：http://vdz.zycfv.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yxi.xingfuxueyuan.xyz

C#:   list.Insert(0, 0);
来源：http://ccs.jianghu66.top

[D04] 删除元素
来源：http://qhr.jqgfzy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rdx.hnxiangtu.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hfk.aizwys.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jfo.fehbvm.com

TS:   arr.splice(0, 1);
来源：http://fvd.52xcode.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cfe.cqqwz.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dab.cdnleiting.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://awt.feifeiyinyue.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nyf.xinyue.icu

[D05] 访问与修改元素
来源：http://urm.gotoacloud.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kbu.dianchejie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lgd.shanyushiyangkeji.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vky.svipenyu.cn

TS:   arr[0]; arr.at(-1);
来源：http://yvh.ehwqpu.com

Java: list.get(0); list.set(0, 9);
来源：http://gez.ybcxt.top

Go:   arr[0]; arr[0] = 9
来源：http://jrp.jiagoushi.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lhe.0kj1m.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://miv.aizwys.cn

[D06] 数组长度
来源：http://quz.sjlbkw.cn

Py:   len(arr)
来源：http://bkq.ydjk.org.cn

PHP:  count($arr);
来源：http://lyu.yongpay.top

JS:   arr.length
来源：http://dai.shanyushiyangtech.top

TS:   arr.length
来源：http://yfn.yj202588.top

Java: list.size();
来源：http://xgh.svipenyu.cn

Go:   len(arr)
来源：http://jsb.fzhhl.top

Ruby: arr.length; arr.size
来源：http://ssm.epnwcf.com

C#:   list.Count;
来源：http://xgm.jinqigufen.top

[D07] 切片 / 取子数组
来源：http://ycg.0kj1m.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wvg.nwbrower.top

PHP:  array_slice($arr, 1, 3);
来源：http://alh.tian-w.cn

JS:   arr.slice(1, 4);
来源：http://vwu.fanxiaobao.xyz

TS:   arr.slice(1, 4);
来源：http://nde.zycfv.cn

Java: list.subList(1, 4);
来源：http://osl.dianchejie.cn

Go:   arr[1:4]
来源：http://gsm.ydzc1.top

Ruby: arr[1, 3]
来源：http://azq.nanxuanxn.top

C#:   list.GetRange(1, 3);
来源：http://gcp.jqgfzy.top

[D08] 合并两个数组
来源：http://aaz.jqgfzy.top

Py:   a + b;  a.extend(b)
来源：http://goq.yj202588.top

PHP:  array_merge($a, $b);
来源：http://ren.ybcxt.top

JS:   [...a, ...b];  a.concat(b);
来源：http://jbl.yueranfly.top

TS:   [...a, ...b];
来源：http://ljv.yueranfly.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://znh.316326.xyz

Go:   append(a, b...)
来源：http://waw.shanyushiyangkeji.top

Ruby: a + b;  a.concat(b)
来源：http://bck.epnwcf.com

C#:   a.Concat(b).ToList()
来源：http://ssn.jqgfzy.top

[D09] 排序（升序）
来源：http://kzt.0kj1m.cn

Py:   sorted(arr);  arr.sort()
来源：http://dqt.hnxiangtu.top

PHP:  sort($arr);
来源：http://dir.52xcode.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ome.yj20258888.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://tzw.hcnkem.com

Java: Collections.sort(list);  list.sort(null);
来源：http://hjr.guowangkeji.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ahp.yuxming.cn

Ruby: arr.sort
来源：http://hpd.ivvv.top

C#:   list.Sort();
来源：http://fol.fanxiaobao.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://kcb.daxiang520.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nze.guannengcc.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wzn.shanyushiyangtech.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hqu.hnxiangtu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dap.ppjwa.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://skp.hammf.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mfr.zhongyouzk.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lao.yuxming.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zcp.yfazqb.com

[D11] 反转数组
来源：http://kdm.pengpengdd.cyou

Py:   arr[::-1];  arr.reverse()
来源：http://uoo.jinqigufen.top

PHP:  array_reverse($arr);
来源：http://cje.svipenyu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pxf.yj20258.top

TS:   [...arr].reverse();
来源：http://ffh.xziqi.cn

Java: Collections.reverse(list);
来源：http://bcu.yueranfly.top

Go:   slices.Reverse(arr)
来源：http://sgc.yangfankeji.com

Ruby: arr.reverse
来源：http://uak.cucudq.cn

C#:   list.Reverse();
来源：http://vpn.jinqigfzy.top

[D12] 查找元素下标
来源：http://bwl.hammf.cn

Py:   arr.index(x);  x in arr
来源：http://srj.daria6918.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://oqg.birdmap.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qxw.ppjwa.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rlk.tarul.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yyu.svipenyu.cn

Go:   slices.Index(arr, x)
来源：http://qrl.9152youxi.cn

Ruby: arr.index(x)
来源：http://ozb.meibo888.top

C#:   list.IndexOf(x);
来源：http://amy.cdnleiting.top

[D13] 过滤（保留满足条件的）
来源：http://uog.guannengcc.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jzi.zhijiandao.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dlm.fengsongda.top

JS:   arr.filter(x => x > 3)
来源：http://ypm.zhiwuduotai.top

TS:   arr.filter(x => x > 3)
来源：http://xll.shangyingyoupin.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://sjm.ivvv.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nvn.bjfxy.top

Ruby: arr.select { |x| x > 3 }
来源：http://zmb.jyoumei.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://flr.sufxvd.cn

[D14] 映射转换（每个元素变形）
来源：http://zad.jiagoushi.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://snp.cheryme.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gvt.zhoulong.xyz

JS:   arr.map(x => x * 2)
来源：http://woj.yfazqb.com

TS:   arr.map(x => x * 2)
来源：http://phb.ehwqpu.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://yzg.ybcxt.top

Go:   // 手写循环
来源：http://wrw.sysykeji.top

Ruby: arr.map { |x| x * 2 }
来源：http://pvy.nanxuanxn.top

C#:   list.Select(x => x * 2).ToList()
来源：http://tyk.cdnleiting.top

[D15] 去重
来源：http://eqi.hesvh.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ceb.jqgufenzy.top

PHP:  array_unique($arr);
来源：http://zuv.hesvh.cn

JS:   [...new Set(arr)]
来源：http://asv.cheryme.top

TS:   [...new Set(arr)]
来源：http://qbd.jyoumei.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qnb.birdmap.top

Go:   // 用 map[T]struct{} 手写
来源：http://ldo.chenzaomai.com

Ruby: arr.uniq
来源：http://fzu.jinqigufen.top

C#:   list.Distinct().ToList()
来源：http://tbp.cqqwz.cn

[D16] 求和与平均值
来源：http://bix.vehdjk.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lds.hysaishi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://itu.zhiwuduotai.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nxi.sysykeji.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sva.tian-w.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sbh.tian-w.cn

Go:   // 手写循环累加
来源：http://wpb.zdqjudy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xkt.jqgufenzy.top

C#:   list.Sum();  list.Average()
来源：http://vhc.nanxuanxn.top

[D17] 最大值与最小值
来源：http://tsu.ywan-chungtsiang.top

Py:   max(arr);  min(arr)
来源：http://ufi.9152youxi.cn

PHP:  max($arr);  min($arr);
来源：http://yra.jqgufenzy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qso.xziqi.cn

TS:   Math.max(...arr);
来源：http://uhp.yangfankeji.com

Java: Collections.max(list);  Collections.min(list);
来源：http://xki.aizwys.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://orf.xylfe.cn

Ruby: arr.max;  arr.min
来源：http://jbr.shanyushiyangkeji.top

C#:   list.Max();  list.Min()
来源：http://nos.9152youxi.cn

[D18] 扁平化嵌套数组
来源：http://gsq.xziqi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qec.xuetiantiany.cn

PHP:  array_merge(...$nested);
来源：http://adn.snrcjt.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wze.tianlin.xyz

TS:   nested.flat();
来源：http://hat.sysykeji.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hbx.zhoulong.xyz

Go:   // 手写双层循环
来源：http://cob.jinghuilouyu.cn

Ruby: nested.flatten
来源：http://uxp.316326.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://oyj.shangyingyoupin.top

[D19] 按字段分组
来源：http://dkd.hnxiangtu.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xbq.xuetiantiany.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cgn.vehdjk.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jxm.fengsongda.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ved.guannengcc.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vbu.tianlin.xyz

Go:   // 手写 map[string][]T
来源：http://leo.zhengqikj.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://aps.sufxvd.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zko.iojbl.cn

[D20] 统计每个元素出现次数
来源：http://gzz.ivvv.top

Py:   Counter(arr)
来源：http://ipk.zhiwuduotai.top

PHP:  array_count_values($arr);
来源：http://kel.sjlbkw.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ljc.havefunace.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://njh.jianghu66.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://uyv.birdmap.top

Go:   // 手写 map[T]int
来源：http://lrd.yuxming.cn

Ruby: arr.tally
来源：http://nax.sjlbkw.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nvm.quarkkingdee.top

[D21] 判断是否包含某元素
来源：http://ycy.316326.xyz

Py:   x in arr
来源：http://zgb.sweek.top

PHP:  in_array($x, $arr, true);
来源：http://wtp.dianchejie.cn

JS:   arr.includes(x)
来源：http://err.gzhubu.top

TS:   arr.includes(x)
来源：http://nyh.hnxiangtu.top

Java: list.contains(x)
来源：http://zzo.shanyushiyangkeji.top

Go:   slices.Contains(arr, x)
来源：http://aov.fzhhl.top

Ruby: arr.include?(x)
来源：http://whd.zhijiandao.cn

C#:   list.Contains(x)
来源：http://qpn.gzhubu.top

[D22] 复制数组（避免共享引用）
来源：http://ake.zhiwuduotai.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mhq.andypj.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lkn.aizwys.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wst.shanyushiyangkeji.top

TS:   [...arr];
来源：http://drz.aibaodan.cn

Java: new ArrayList<>(list);
来源：http://led.shangyingyoupin.top

Go:   copied := append([]int(nil), arr...)
来源：http://qrl.iojbl.cn

Ruby: arr.dup;  arr.clone
来源：http://qaz.ehwqpu.com

C#:   new List<int>(list);
来源：http://nxm.zhaomingkeji.xyz

[D23] reduce 累积计算
来源：http://ney.fanxiaobao.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jay.316326.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yvu.hnqzz.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eij.smart0.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rla.hfpthk.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://dov.uphjek.com

Go:   // 手写循环
来源：http://api.sufxvd.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fkr.shanyushiyangtech.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uqu.shanyushiyangtech.top

[D24] 字典 / Map 基本操作
来源：http://vzh.tianlin.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qoy.sxryk.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fxq.ctjpmb.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lvx.andypj.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mpc.yangfankeji.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://avr.zycfv.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mel.guowangkeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qyh.sxryk.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://iup.hnxiangtu.top

[D25] Set 集合去重与交并差
来源：http://kah.birdmap.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ejp.wangdashe.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://oxh.redwolf501.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rbl.tian-w.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fhc.52xcode.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xpm.mhx1999.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ccj.yangfankeji.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://emo.shangyingyoupin.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tzz.andypj.xyz

[D26] 数组转字符串
来源：http://ste.hammf.cn

Py:   ", ".join(map(str, arr))
来源：http://qsk.jinqigufen.top

PHP:  implode(", ", $arr);
来源：http://gbh.gaohongyu789.top

JS:   arr.join(", ")
来源：http://cyu.sufxvd.cn

TS:   arr.join(", ")
来源：http://wfp.ehwqpu.com

Java: String.join(", ", list)
来源：http://ypk.ehwqpu.com

Go:   strings.Join(strs, ", ")
来源：http://xtg.nwbrower.top

Ruby: arr.join(", ")
来源：http://iuz.316326.xyz

C#:   string.Join(", ", list)
来源：http://xof.jqgfzy.top

================================================================================
来源：http://ozk.yuxming.cn

E. 字符串处理
来源：http://xrj.shanyushiyangtech.top

================================================================================
来源：http://oau.hysaishi.cn

[E01] 拼接字符串
来源：http://mzp.fzhhl.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bmd.tanke756.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hwv.zycfv.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://aal.xuanzx.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://skr.yfazqb.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gtk.ctjpmb.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pmq.xuetiantiany.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ojg.zhongyouzk.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tjc.ydjk.org.cn

[E02] 重复字符串
来源：http://cok.xuanzx.com

Py:   "ab" * 3
来源：http://zpz.nanxuanxn.top

PHP:  str_repeat("ab", 3);
来源：http://mwr.gogol.net.cn

JS:   "ab".repeat(3)
来源：http://mty.epnwcf.com

TS:   "ab".repeat(3)
来源：http://ylh.andypj.xyz

Java: "ab".repeat(3)
来源：http://lng.zycfv.cn

Go:   strings.Repeat("ab", 3)
来源：http://mzh.hfpthk.cn

Ruby: "ab" * 3
来源：http://ieh.iojbl.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uba.guowangkeji.top

[E03] 截取子串
来源：http://ujg.c1oappe.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pyw.yfazqb.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hvf.yuxming.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hsm.cucudq.cn

TS:   s.slice(1, 4)
来源：http://xuc.xuetiantiany.cn

Java: s.substring(1, 4)
来源：http://ohq.chenzaomai.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://svt.316326.xyz


<!-- 参考信息 -->