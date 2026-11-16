代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gnu.zhoulong.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nuy.hnxiangtu.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tkx.mhx1999.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://joe.cqqwz.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wax.wangshuangyany.cn

Go:   func add(a, b int) int
来源：http://cdu.meibo888.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bqz.tanke756.top

C#:   int Add(int a, int b) => a + b;
来源：http://efb.nanxinkj.top

[C14] 泛型函数
来源：http://yoz.wangdashe.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ifq.xuanzx.com

PHP:  // 无泛型
来源：http://gyk.gaohongyu789.top

JS:   // 无泛型
来源：http://vrg.bbcook.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kdf.dianchejie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://epo.yueranfly.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://uzx.tianlin.xyz

Ruby: # 无泛型
来源：http://ahe.bjfxy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://iro.yuxming.cn

[C15] 解构 / 展开参数
来源：http://zmy.zhijiandao.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ova.dashuyun.cn

PHP:  [$a, $b] = $pair;
来源：http://vah.shangyingyoupin.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xcp.ybcxt.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://oxw.aizwys.cn

Java: // 无解构
来源：http://yat.zhiwuduotai.top

Go:   // 无解构
来源：http://rbx.cucudq.cn

Ruby: a, b = pair
来源：http://gbc.jianghu66.top

C#:   var (a, b) = pair;
来源：http://xbm.dianchejie.cn

[C16] 函数 / 方法重载
来源：http://hrl.c1oappe.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tnf.wangdashe.top

PHP:  // 无重载
来源：http://khj.jqgfzy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://een.hesvh.cn

TS:   // 用联合类型或重载签名声明
来源：http://dxa.redwolf501.top

Java: void f(int a) {}  void f(String a) {}
来源：http://rmq.cdnleiting.top

Go:   // 无重载：用不同函数名
来源：http://srm.cucudq.cn

Ruby: # 无重载：靠动态参数
来源：http://kza.nanxinkj.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://kst.yueranfly.top

================================================================================
来源：http://mhd.mhx1999.top

D. 数组 / 列表 / 集合
来源：http://wco.shangyingyoupin.top

================================================================================
来源：http://frz.mhx1999.top

[D01] 创建数组 / 列表
来源：http://vpb.nwbrower.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://fow.xuetiantiany.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jvz.gotoacloud.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ijg.nanxuanxn.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://fiy.zhengqikj.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xmt.tian-w.cn

Go:   arr := []int{1, 2, 3}
来源：http://luw.yonumen.top

Ruby: arr = [1, 2, 3]
来源：http://unt.sxryk.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ask.mhx1999.top

[D02] 追加元素到末尾
来源：http://ncu.xingfuxueyuan.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rgv.zhongyouzk.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fup.havefunace.top

JS:   arr.push(4);
来源：http://qas.pycfn.com

TS:   arr.push(4);
来源：http://hhk.epnwcf.com

Java: list.add(4);
来源：http://lpm.yj202588.top

Go:   arr = append(arr, 4)
来源：http://ynr.jinqigufen.top

Ruby: arr << 4; arr.push(5)
来源：http://vje.zhijiandao.cn

C#:   list.Add(4);
来源：http://wdq.jinghuilouyu.cn

[D03] 在指定位置插入元素
来源：http://ljj.vehdjk.com

Py:   arr.insert(0, 0)
来源：http://kjs.sufxvd.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://udu.sweek.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ogn.sweek.top

TS:   arr.splice(0, 0, 0);
来源：http://kwe.zhixingplan.top

Java: list.add(0, 0);
来源：http://phz.wangshuangyany.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ihr.zhaomingkeji.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rhk.hesvh.cn

C#:   list.Insert(0, 0);
来源：http://sgg.yuanzhike.top

[D04] 删除元素
来源：http://ymg.ppjwa.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qba.redwolf501.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cpd.jlsjyb.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://khw.wangdashe.top

TS:   arr.splice(0, 1);
来源：http://thc.tarul.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rnm.yuanzhike.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://aiz.yfazqb.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kom.jinyuanbaomall.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xzn.hywenlv.cn

[D05] 访问与修改元素
来源：http://euk.jiagoushi.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rag.fanxiaobao.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jjx.fzhhl.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://edr.pengpengdd.cyou

TS:   arr[0]; arr.at(-1);
来源：http://lsf.chenlongwang.top

Java: list.get(0); list.set(0, 9);
来源：http://txc.xingfuxueyuan.xyz

Go:   arr[0]; arr[0] = 9
来源：http://ytd.bjfxy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jeg.bjfxy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hwi.shangyingyoupin.top

[D06] 数组长度
来源：http://jhj.daxiang520.top

Py:   len(arr)
来源：http://eim.c1oappe.top

PHP:  count($arr);
来源：http://gdx.hongshengwenyu.top

JS:   arr.length
来源：http://zis.chenjidiqi.icu

TS:   arr.length
来源：http://jte.shanyushiyangkeji.top

Java: list.size();
来源：http://jir.yfazqb.com

Go:   len(arr)
来源：http://lmg.zhaomingkeji.xyz

Ruby: arr.length; arr.size
来源：http://dru.redwolf501.top

C#:   list.Count;
来源：http://aye.wangshuangyany.cn

[D07] 切片 / 取子数组
来源：http://rsl.cqqwz.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rzq.kuanghao11.cn

PHP:  array_slice($arr, 1, 3);
来源：http://nau.zhixingplan.top

JS:   arr.slice(1, 4);
来源：http://tty.jqgufenzy.top

TS:   arr.slice(1, 4);
来源：http://tiw.jiagoushi.top

Java: list.subList(1, 4);
来源：http://rrt.hywenlv.cn

Go:   arr[1:4]
来源：http://dcu.ivvv.top

Ruby: arr[1, 3]
来源：http://igd.9152youxi.cn

C#:   list.GetRange(1, 3);
来源：http://ibh.tianlin.xyz

[D08] 合并两个数组
来源：http://exn.gaohongyu789.top

Py:   a + b;  a.extend(b)
来源：http://huh.dashuyun.cn

PHP:  array_merge($a, $b);
来源：http://jvn.zhengqikj.top

JS:   [...a, ...b];  a.concat(b);
来源：http://bci.zhijiandao.cn

TS:   [...a, ...b];
来源：http://ssz.jinghuilouyu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nhq.jinqigfzy.top

Go:   append(a, b...)
来源：http://pex.dianchejie.cn

Ruby: a + b;  a.concat(b)
来源：http://dkj.zycfv.cn

C#:   a.Concat(b).ToList()
来源：http://fpp.yueranfly.top

[D09] 排序（升序）
来源：http://rwm.wangdashe.top

Py:   sorted(arr);  arr.sort()
来源：http://lcb.52xcode.cn

PHP:  sort($arr);
来源：http://mpw.nanxuanxn.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://oiy.yj20258.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://yiu.shzxlz.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://nbd.zycfv.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pmq.vehdjk.com

Ruby: arr.sort
来源：http://wll.jinqigfzy.top

C#:   list.Sort();
来源：http://guk.dianchejie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://dac.sysykeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ptu.52xcode.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dyr.bbcook.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lca.yongpay.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://uyy.sxryk.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://enu.yj202588.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dxx.jqgfzy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nxq.ivvv.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mjv.guowangkeji.top

[D11] 反转数组
来源：http://gdw.havefunace.top

Py:   arr[::-1];  arr.reverse()
来源：http://ynj.c1oappe.top

PHP:  array_reverse($arr);
来源：http://kre.ydzc1.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://eya.zycfv.cn

TS:   [...arr].reverse();
来源：http://uhb.shzxlz.cn

Java: Collections.reverse(list);
来源：http://ohy.hywenlv.cn

Go:   slices.Reverse(arr)
来源：http://hin.yueranfly.top

Ruby: arr.reverse
来源：http://enk.sjlbkw.cn

C#:   list.Reverse();
来源：http://qpu.uphjek.com

[D12] 查找元素下标
来源：http://yiv.sjlbkw.cn

Py:   arr.index(x);  x in arr
来源：http://iba.wangdashe.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zco.hesvh.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wpo.316326.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://smh.tianlin.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mxv.gogol.net.cn

Go:   slices.Index(arr, x)
来源：http://oip.hnxiangtu.top

Ruby: arr.index(x)
来源：http://sde.hammf.cn

C#:   list.IndexOf(x);
来源：http://jsl.nanxinkj.top

[D13] 过滤（保留满足条件的）
来源：http://rrc.zhoulong.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gtv.ydjk.org.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nco.vehdjk.com

JS:   arr.filter(x => x > 3)
来源：http://mkl.epnwcf.com

TS:   arr.filter(x => x > 3)
来源：http://rov.cashguo.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wnc.nwbrower.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zge.yj202588.top

Ruby: arr.select { |x| x > 3 }
来源：http://bzo.yuxming.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://xvq.yvedp.cn

[D14] 映射转换（每个元素变形）
来源：http://lso.shanyushiyangtech.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://iyu.aibaodan.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://smo.shzxlz.cn

JS:   arr.map(x => x * 2)
来源：http://ccf.chenlongwang.top

TS:   arr.map(x => x * 2)
来源：http://hwk.zycfv.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://wsh.zhoulong.xyz

Go:   // 手写循环
来源：http://kux.jlsjyb.cn

Ruby: arr.map { |x| x * 2 }
来源：http://elk.yanxiufei.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://tfj.hnqzz.top

[D15] 去重
来源：http://dvi.nwbrower.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://anb.yuanzhike.top

PHP:  array_unique($arr);
来源：http://grv.gzhubu.top

JS:   [...new Set(arr)]
来源：http://gfd.tanke756.top

TS:   [...new Set(arr)]
来源：http://dbw.aizwys.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kqx.feifeiyinyue.top

Go:   // 用 map[T]struct{} 手写
来源：http://cnh.yonumen.top

Ruby: arr.uniq
来源：http://akp.ywan-chungtsiang.top

C#:   list.Distinct().ToList()
来源：http://noe.chenlongwang.top

[D16] 求和与平均值
来源：http://ryc.fzhhl.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ufd.xingfuxueyuan.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://czf.fzhhl.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xvf.sysykeji.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bth.guannengcc.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qdi.smart0.xyz

Go:   // 手写循环累加
来源：http://lsy.yj20258.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sli.gaohongyu789.top

C#:   list.Sum();  list.Average()
来源：http://nai.sufxvd.cn

[D17] 最大值与最小值
来源：http://xiz.guowangkeji.top

Py:   max(arr);  min(arr)
来源：http://tje.shzxlz.cn

PHP:  max($arr);  min($arr);
来源：http://ppx.yvedp.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mem.hysaishi.cn

TS:   Math.max(...arr);
来源：http://wle.zhiwuduotai.top

Java: Collections.max(list);  Collections.min(list);
来源：http://jdt.gogol.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vls.xziqi.cn

Ruby: arr.max;  arr.min
来源：http://opv.hywenlv.cn

C#:   list.Max();  list.Min()
来源：http://kck.xuanzx.com

[D18] 扁平化嵌套数组
来源：http://qoa.shanyushiyangkeji.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jxt.jlsjyb.cn

PHP:  array_merge(...$nested);
来源：http://jlt.ywan-chungtsiang.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://krg.jinqigufen.top

TS:   nested.flat();
来源：http://fmj.tarul.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zkq.gotoacloud.top

Go:   // 手写双层循环
来源：http://jwx.yongpay.top

Ruby: nested.flatten
来源：http://jtg.hongshengwenyu.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://psy.hywenlv.cn

[D19] 按字段分组
来源：http://sbu.daxiang520.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nkm.zhixingplan.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tpj.chenjidiqi.icu

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wau.tarul.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://tbn.316326.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://elq.epnwcf.com

Go:   // 手写 map[string][]T
来源：http://oaf.ehwqpu.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://fvr.shzxlz.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ouj.yfazqb.com

[D20] 统计每个元素出现次数
来源：http://wmn.sufxvd.cn

Py:   Counter(arr)
来源：http://uxg.ctjpmb.com

PHP:  array_count_values($arr);
来源：http://abe.hywenlv.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://egj.shuidangran.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nom.hongshengwenyu.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qmo.hfpthk.cn

Go:   // 手写 map[T]int
来源：http://zgf.zhiwuduotai.top

Ruby: arr.tally
来源：http://iis.meibo888.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mik.cashguo.top

[D21] 判断是否包含某元素
来源：http://aws.zhaomingkeji.xyz

Py:   x in arr
来源：http://cqg.havefunace.top

PHP:  in_array($x, $arr, true);
来源：http://sxa.sysykeji.top

JS:   arr.includes(x)
来源：http://jii.fzhhl.top

TS:   arr.includes(x)
来源：http://awb.meibo888.top

Java: list.contains(x)
来源：http://wcu.jinqigufen.top

Go:   slices.Contains(arr, x)
来源：http://tst.nanxinkj.top

Ruby: arr.include?(x)
来源：http://ber.jianghu66.top

C#:   list.Contains(x)
来源：http://ktg.hnxiangtu.top

[D22] 复制数组（避免共享引用）
来源：http://hdl.shanyushiyangkeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gri.nanxinkj.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tii.jqgufenzy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xii.xingfuxueyuan.xyz

TS:   [...arr];
来源：http://bfn.bbcook.cn

Java: new ArrayList<>(list);
来源：http://onl.xuanzx.com

Go:   copied := append([]int(nil), arr...)
来源：http://udi.zhongyouzk.top

Ruby: arr.dup;  arr.clone
来源：http://abp.wangdashe.top

C#:   new List<int>(list);
来源：http://hmc.tanke756.top

[D23] reduce 累积计算
来源：http://mtz.daxiang520.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bqh.andypj.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://odm.hfpthk.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dqe.zhoulong.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ako.zhixingplan.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ihn.birdmap.top

Go:   // 手写循环
来源：http://pdu.ppjwa.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lxp.daxiang520.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://emg.316326.xyz

[D24] 字典 / Map 基本操作
来源：http://dfp.haohaochexian.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wkg.shanyushiyangtech.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fft.yueranfly.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qfq.jinghuilouyu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wsb.ybcxt.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hdj.yonumen.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dxi.ybcxt.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qdo.sufxvd.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ipk.sxryk.cn

[D25] Set 集合去重与交并差
来源：http://dsc.yueranfly.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cbc.ivvv.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bms.yj20258888.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tum.nanxuanxn.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hej.guannengcc.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ooi.tarul.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vdu.meibo888.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zge.yuxming.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fdx.52xcode.cn

[D26] 数组转字符串
来源：http://dmp.zhaomingkeji.xyz

Py:   ", ".join(map(str, arr))
来源：http://mus.svipenyu.cn

PHP:  implode(", ", $arr);
来源：http://aru.wangdashe.top

JS:   arr.join(", ")
来源：http://tpr.havefunace.top

TS:   arr.join(", ")
来源：http://yef.tanke756.top

Java: String.join(", ", list)
来源：http://rje.jinqigufen.top

Go:   strings.Join(strs, ", ")
来源：http://agd.smart0.xyz

Ruby: arr.join(", ")
来源：http://msz.52xcode.cn

C#:   string.Join(", ", list)
来源：http://rfe.xingfuxueyuan.xyz

================================================================================
来源：http://qbq.0kj1m.cn

E. 字符串处理
来源：http://jak.hysaishi.cn

================================================================================
来源：http://tua.meibo888.top

[E01] 拼接字符串
来源：http://vzy.quarkkingdee.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xqg.yj202588.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tyb.fzhhl.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zoq.fehbvm.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xdb.chenjidiqi.icu

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://osi.ybcxt.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mqt.yj20258888.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fen.hnqzz.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lhm.birdmap.top

[E02] 重复字符串
来源：http://wsk.hfpthk.cn

Py:   "ab" * 3
来源：http://qow.dashuyun.cn

PHP:  str_repeat("ab", 3);
来源：http://bzs.guannengcc.top

JS:   "ab".repeat(3)
来源：http://fed.zdqjudy.top

TS:   "ab".repeat(3)
来源：http://gvt.uphjek.com

Java: "ab".repeat(3)
来源：http://gas.fktsv.cn

Go:   strings.Repeat("ab", 3)
来源：http://xey.shzxlz.cn

Ruby: "ab" * 3
来源：http://dxc.hywenlv.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xvu.guowangkeji.top

[E03] 截取子串
来源：http://kom.epnwcf.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://auq.nwbrower.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yzz.ydjk.org.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gzb.jinyuanbaomall.cn

TS:   s.slice(1, 4)
来源：http://seu.ehwqpu.com

Java: s.substring(1, 4)
来源：http://ntf.andypj.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rhv.hnqzz.top


<!-- 参考信息 -->