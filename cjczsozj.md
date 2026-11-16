代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://wwl.birdmap.top

Ruby: -> { puts "run" }.call
来源：http://nvs.meibo888.top

C#:   // 无 IIFE：用静态构造函数
来源：http://blc.tianlin.xyz

[C13] 类型声明 / 类型注解
来源：http://daz.birdmap.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yar.bjfxy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ndq.chenjidiqi.icu

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tfw.shanyushiyangtech.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pfj.ydzc1.top

Java: int add(int a, int b) { return a + b; }
来源：http://qvi.aibaodan.cn

Go:   func add(a, b int) int
来源：http://ocn.iojbl.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xhd.sxryk.cn

C#:   int Add(int a, int b) => a + b;
来源：http://yml.feifeiyinyue.top

[C14] 泛型函数
来源：http://oue.hnqzz.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xwe.bjfxy.top

PHP:  // 无泛型
来源：http://zaj.guowangkeji.top

JS:   // 无泛型
来源：http://ykg.jyoumei.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ocq.fehbvm.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wht.zhixingplan.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vmr.jiagoushi.top

Ruby: # 无泛型
来源：http://iat.kuanghao11.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dmy.yvedp.cn

[C15] 解构 / 展开参数
来源：http://fmj.xinyue.icu

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zje.bbcook.cn

PHP:  [$a, $b] = $pair;
来源：http://jal.xziqi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xxd.kuanghao11.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://awc.sweek.top

Java: // 无解构
来源：http://edb.jiagoushi.top

Go:   // 无解构
来源：http://pij.hongshengwenyu.top

Ruby: a, b = pair
来源：http://cwy.yfazqb.com

C#:   var (a, b) = pair;
来源：http://mbh.shanyushiyangkeji.top

[C16] 函数 / 方法重载
来源：http://yxc.0kj1m.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cvc.jinyuanbaomall.cn

PHP:  // 无重载
来源：http://exf.zhaomingkeji.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://zoz.ppjwa.cn

TS:   // 用联合类型或重载签名声明
来源：http://hcz.redwolf501.top

Java: void f(int a) {}  void f(String a) {}
来源：http://rdg.chenlongwang.top

Go:   // 无重载：用不同函数名
来源：http://vyv.jinyuanbaomall.cn

Ruby: # 无重载：靠动态参数
来源：http://uwy.iojbl.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://oax.hammf.cn

================================================================================
来源：http://red.fktsv.cn

D. 数组 / 列表 / 集合
来源：http://noe.wangshuangyany.cn

================================================================================
来源：http://apf.xuetiantiany.cn

[D01] 创建数组 / 列表
来源：http://kue.nanxinkj.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ufp.zhoulong.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zpa.xziqi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qyl.chenjidiqi.icu

TS:   const arr: number[] = [1, 2, 3];
来源：http://fpv.yonumen.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://acg.jinghuilouyu.cn

Go:   arr := []int{1, 2, 3}
来源：http://rnn.kuanghao11.cn

Ruby: arr = [1, 2, 3]
来源：http://sfa.ybcxt.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://oow.yuanzhike.top

[D02] 追加元素到末尾
来源：http://hoh.jinqigufen.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sdz.ybcxt.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fae.yongpay.top

JS:   arr.push(4);
来源：http://ioj.uphjek.com

TS:   arr.push(4);
来源：http://ons.meibo888.top

Java: list.add(4);
来源：http://kke.andypj.xyz

Go:   arr = append(arr, 4)
来源：http://ivp.zhongyouzk.top

Ruby: arr << 4; arr.push(5)
来源：http://xaz.hcnkem.com

C#:   list.Add(4);
来源：http://lqa.jyoumei.cn

[D03] 在指定位置插入元素
来源：http://jcz.zycfv.cn

Py:   arr.insert(0, 0)
来源：http://jkw.jinqigfzy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wxh.guowangkeji.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lpj.52xcode.cn

TS:   arr.splice(0, 0, 0);
来源：http://gur.hfpthk.cn

Java: list.add(0, 0);
来源：http://nmm.chenzaomai.com

Go:   arr = append([]int{0}, arr...)
来源：http://xfe.52xcode.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://owm.cucudq.cn

C#:   list.Insert(0, 0);
来源：http://ksp.cucudq.cn

[D04] 删除元素
来源：http://puo.jinghuilouyu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://llj.mhx1999.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://guc.cheryme.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ncv.zhengqikj.top

TS:   arr.splice(0, 1);
来源：http://rae.pengpengdd.cyou

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://maj.yongpay.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sxn.ctjpmb.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mfe.jinghuilouyu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dpl.fanxiaobao.xyz

[D05] 访问与修改元素
来源：http://vpz.gogol.net.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ivh.dianchejie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wvt.ctjpmb.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jqu.smart0.xyz

TS:   arr[0]; arr.at(-1);
来源：http://xcc.shzxlz.cn

Java: list.get(0); list.set(0, 9);
来源：http://mdi.dashuyun.cn

Go:   arr[0]; arr[0] = 9
来源：http://jys.hesvh.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ugn.nanxuanxn.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ouz.zhijiandao.cn

[D06] 数组长度
来源：http://bmt.meibo888.top

Py:   len(arr)
来源：http://ufd.chenzaomai.com

PHP:  count($arr);
来源：http://iwt.zdbjq.cn

JS:   arr.length
来源：http://wfm.xinyue.icu

TS:   arr.length
来源：http://izh.xuetiantiany.cn

Java: list.size();
来源：http://lgx.xuanzx.com

Go:   len(arr)
来源：http://iuw.yuanzhike.top

Ruby: arr.length; arr.size
来源：http://svg.jqgufenzy.top

C#:   list.Count;
来源：http://nfx.zhijiandao.cn

[D07] 切片 / 取子数组
来源：http://tvs.hysaishi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://uaz.sxryk.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fec.shuidangran.top

JS:   arr.slice(1, 4);
来源：http://pkt.snrcjt.cn

TS:   arr.slice(1, 4);
来源：http://gyz.daxiang520.top

Java: list.subList(1, 4);
来源：http://soh.jinqigufen.top

Go:   arr[1:4]
来源：http://pzz.xziqi.cn

Ruby: arr[1, 3]
来源：http://riq.redwolf501.top

C#:   list.GetRange(1, 3);
来源：http://sjm.yongpay.top

[D08] 合并两个数组
来源：http://wos.cucudq.cn

Py:   a + b;  a.extend(b)
来源：http://zee.meibo888.top

PHP:  array_merge($a, $b);
来源：http://ris.aizwys.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gut.sxryk.cn

TS:   [...a, ...b];
来源：http://svf.ehwqpu.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tdi.ydzc1.top

Go:   append(a, b...)
来源：http://hgv.yangfankeji.com

Ruby: a + b;  a.concat(b)
来源：http://lnm.yj202588.top

C#:   a.Concat(b).ToList()
来源：http://rnf.yuanzhike.top

[D09] 排序（升序）
来源：http://dln.guowangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://eni.jlsjyb.cn

PHP:  sort($arr);
来源：http://cmi.sufxvd.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dxc.meibo888.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://pot.hfpthk.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://zly.nwbrower.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wnx.tianlin.xyz

Ruby: arr.sort
来源：http://tkw.haohaochexian.top

C#:   list.Sort();
来源：http://qpt.zhaomingkeji.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://oci.jlsjyb.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jsj.birdmap.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://amt.xylfe.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://eqw.zhixingplan.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yci.yj20258.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jmc.zhengqikj.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://iyg.yuxming.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yso.xinyue.icu

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lcn.tarul.cn

[D11] 反转数组
来源：http://crt.xuetiantiany.cn

Py:   arr[::-1];  arr.reverse()
来源：http://tfy.jinghuilouyu.cn

PHP:  array_reverse($arr);
来源：http://ves.zdqjudy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zyo.fzhhl.top

TS:   [...arr].reverse();
来源：http://hgg.tanke756.top

Java: Collections.reverse(list);
来源：http://ykg.jinqigufen.top

Go:   slices.Reverse(arr)
来源：http://pkf.zhoulong.xyz

Ruby: arr.reverse
来源：http://oiz.yangfankeji.com

C#:   list.Reverse();
来源：http://mur.hysaishi.cn

[D12] 查找元素下标
来源：http://cgh.daxiang520.top

Py:   arr.index(x);  x in arr
来源：http://ets.zhaomingkeji.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zzk.hcnkem.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://siv.sweek.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nxo.cashguo.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xwd.daxiang520.top

Go:   slices.Index(arr, x)
来源：http://dtj.bbcook.cn

Ruby: arr.index(x)
来源：http://usp.tanke756.top

C#:   list.IndexOf(x);
来源：http://rru.yueranfly.top

[D13] 过滤（保留满足条件的）
来源：http://xwx.shangyingyoupin.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vph.svipenyu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kit.feifeiyinyue.top

JS:   arr.filter(x => x > 3)
来源：http://ibe.xuetiantiany.cn

TS:   arr.filter(x => x > 3)
来源：http://vni.bbcook.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rqt.quarkkingdee.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mcs.sufxvd.cn

Ruby: arr.select { |x| x > 3 }
来源：http://pck.ppjwa.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://svb.chenlongwang.top

[D14] 映射转换（每个元素变形）
来源：http://rnc.redwolf501.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wrw.0kj1m.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://whl.sysykeji.top

JS:   arr.map(x => x * 2)
来源：http://hmx.havefunace.top

TS:   arr.map(x => x * 2)
来源：http://zkq.birdmap.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://kad.feifeiyinyue.top

Go:   // 手写循环
来源：http://ppx.yj202588.top

Ruby: arr.map { |x| x * 2 }
来源：http://dxu.cashguo.top

C#:   list.Select(x => x * 2).ToList()
来源：http://umk.epnwcf.com

[D15] 去重
来源：http://fei.jiagoushi.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cgf.xuetiantiany.cn

PHP:  array_unique($arr);
来源：http://ynn.yangfankeji.com

JS:   [...new Set(arr)]
来源：http://kav.hesvh.cn

TS:   [...new Set(arr)]
来源：http://lxz.pycfn.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qma.jianghu66.top

Go:   // 用 map[T]struct{} 手写
来源：http://jko.hesvh.cn

Ruby: arr.uniq
来源：http://xun.chenzaomai.com

C#:   list.Distinct().ToList()
来源：http://ord.sysykeji.top

[D16] 求和与平均值
来源：http://hua.zhiwuduotai.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ebz.uphjek.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jmy.yj202588.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://esq.sweek.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ukx.yfazqb.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zfl.hfpthk.cn

Go:   // 手写循环累加
来源：http://bvy.yuanzhike.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xgh.fzhhl.top

C#:   list.Sum();  list.Average()
来源：http://jdv.cucudq.cn

[D17] 最大值与最小值
来源：http://mum.jinyuanbaomall.cn

Py:   max(arr);  min(arr)
来源：http://wto.chenzaomai.com

PHP:  max($arr);  min($arr);
来源：http://ylf.tarul.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://azz.uphjek.com

TS:   Math.max(...arr);
来源：http://zox.ybcxt.top

Java: Collections.max(list);  Collections.min(list);
来源：http://myq.sufxvd.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kfi.kuanghao11.cn

Ruby: arr.max;  arr.min
来源：http://ddp.zycfv.cn

C#:   list.Max();  list.Min()
来源：http://vbm.cashguo.top

[D18] 扁平化嵌套数组
来源：http://jjj.zhongyouzk.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://glh.birdmap.top

PHP:  array_merge(...$nested);
来源：http://djf.gotoacloud.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://udx.jyoumei.cn

TS:   nested.flat();
来源：http://gbd.shangyingyoupin.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nqj.ybcxt.top

Go:   // 手写双层循环
来源：http://xfy.redwolf501.top

Ruby: nested.flatten
来源：http://gpo.epnwcf.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://gxc.yangfankeji.com

[D19] 按字段分组
来源：http://jfk.dianchejie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gim.birdmap.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ryd.daxiang520.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dqk.gzhubu.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://bps.aizwys.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lna.jinyuanbaomall.cn

Go:   // 手写 map[string][]T
来源：http://buo.ybcxt.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://tnn.nanxuanxn.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rlx.hcnkem.com

[D20] 统计每个元素出现次数
来源：http://ufg.redwolf501.top

Py:   Counter(arr)
来源：http://ekb.sufxvd.cn

PHP:  array_count_values($arr);
来源：http://szz.hysaishi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://diy.fehbvm.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rob.jianghu66.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zyc.jqgufenzy.top

Go:   // 手写 map[T]int
来源：http://izc.snrcjt.cn

Ruby: arr.tally
来源：http://gjk.shuidangran.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rmg.epnwcf.com

[D21] 判断是否包含某元素
来源：http://esb.yueranfly.top

Py:   x in arr
来源：http://vjh.yangfankeji.com

PHP:  in_array($x, $arr, true);
来源：http://sxj.ydzc1.top

JS:   arr.includes(x)
来源：http://bdg.chenlongwang.top

TS:   arr.includes(x)
来源：http://rbw.vqdsnc.cn

Java: list.contains(x)
来源：http://xao.yuxming.cn

Go:   slices.Contains(arr, x)
来源：http://yob.gotoacloud.top

Ruby: arr.include?(x)
来源：http://kjg.ivvv.top

C#:   list.Contains(x)
来源：http://jdl.jinyuanbaomall.cn

[D22] 复制数组（避免共享引用）
来源：http://msj.aibaodan.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cre.wangdashe.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ztj.shuidangran.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hvz.shzxlz.cn

TS:   [...arr];
来源：http://qzl.jiagoushi.top

Java: new ArrayList<>(list);
来源：http://ufe.xylfe.cn

Go:   copied := append([]int(nil), arr...)
来源：http://agi.ctjpmb.com

Ruby: arr.dup;  arr.clone
来源：http://jph.ppjwa.cn

C#:   new List<int>(list);
来源：http://suo.nwbrower.top

[D23] reduce 累积计算
来源：http://pqy.havefunace.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bjw.ybcxt.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kxg.cucudq.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bgy.zycfv.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vrl.xuanzx.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://yry.shanyushiyangkeji.top

Go:   // 手写循环
来源：http://jld.redwolf501.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jgz.yueranfly.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zmz.zhixingplan.top

[D24] 字典 / Map 基本操作
来源：http://fpz.aizwys.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ebq.jqgufenzy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wnb.vqdsnc.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dkt.vqdsnc.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ktn.jinghuilouyu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hop.jiagoushi.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kjq.fehbvm.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://beb.sufxvd.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bug.shzxlz.cn

[D25] Set 集合去重与交并差
来源：http://tuj.gzhubu.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wwg.zhixingplan.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://skm.jianghu66.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://oeg.ydzc1.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pps.ppjwa.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zkw.nwbrower.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wad.mhx1999.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zkf.hcnkem.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rfr.sjlbkw.cn

[D26] 数组转字符串
来源：http://cua.ydjk.org.cn

Py:   ", ".join(map(str, arr))
来源：http://nlr.zhengqikj.top

PHP:  implode(", ", $arr);
来源：http://imt.ehwqpu.com

JS:   arr.join(", ")
来源：http://ayb.chenzaomai.com

TS:   arr.join(", ")
来源：http://qar.andypj.xyz

Java: String.join(", ", list)
来源：http://jjg.sjlbkw.cn

Go:   strings.Join(strs, ", ")
来源：http://mzh.cucudq.cn

Ruby: arr.join(", ")
来源：http://eeo.cashguo.top

C#:   string.Join(", ", list)
来源：http://qrr.ybcxt.top

================================================================================
来源：http://psh.hysaishi.cn

E. 字符串处理
来源：http://gyb.snrcjt.cn

================================================================================
来源：http://zqh.gotoacloud.top

[E01] 拼接字符串
来源：http://gxa.wangdashe.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lae.xingfuxueyuan.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lnl.xingfuxueyuan.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tmd.xingfuxueyuan.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://atu.yanxiufei.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://aoe.chenlongwang.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vyo.yj20258888.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://out.svipenyu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dgy.tanke756.top

[E02] 重复字符串
来源：http://vkd.xuetiantiany.cn

Py:   "ab" * 3
来源：http://gaa.hammf.cn

PHP:  str_repeat("ab", 3);
来源：http://vhh.guowangkeji.top

JS:   "ab".repeat(3)
来源：http://nak.jinghuilouyu.cn

TS:   "ab".repeat(3)
来源：http://asi.jinyuanbaomall.cn

Java: "ab".repeat(3)
来源：http://jim.nwbrower.top

Go:   strings.Repeat("ab", 3)
来源：http://xhh.nanxuanxn.top

Ruby: "ab" * 3
来源：http://aqe.uphjek.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mgm.yj20258.top

[E03] 截取子串
来源：http://osb.jinqigufen.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pqj.yangfankeji.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fdm.meibo888.top


<!-- 参考信息 -->