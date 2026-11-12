代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://trj.dashuyun.cn

JS:   (() => { console.log("run"); })();
来源：http://awn.bjfxy.top

TS:   (() => { console.log("run"); })();
来源：http://hzu.c1oappe.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://eso.ywan-chungtsiang.top

Go:   func() { fmt.Println("run") }()
来源：http://zsc.haohaochexian.top

Ruby: -> { puts "run" }.call
来源：http://vrr.shuidangran.top

C#:   // 无 IIFE：用静态构造函数
来源：http://pxj.meibo888.top

[C13] 类型声明 / 类型注解
来源：http://psn.fktsv.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ryu.sweek.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tjw.hysaishi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bzb.ctjpmb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qff.0kj1m.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cyx.jinqigfzy.top

Go:   func add(a, b int) int
来源：http://zdu.shanyushiyangtech.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jbf.gaohongyu789.top

C#:   int Add(int a, int b) => a + b;
来源：http://pdn.fanxiaobao.xyz

[C14] 泛型函数
来源：http://pcy.fzhhl.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vue.cucudq.cn

PHP:  // 无泛型
来源：http://zbt.zhaomingkeji.xyz

JS:   // 无泛型
来源：http://mfq.sufxvd.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qhd.jinqigufen.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dqf.daxiang520.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://chd.xuanzx.com

Ruby: # 无泛型
来源：http://uwi.fanxiaobao.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://eiu.nanxuanxn.top

[C15] 解构 / 展开参数
来源：http://zfz.yj20258888.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ncf.shzxlz.cn

PHP:  [$a, $b] = $pair;
来源：http://kzl.dashuyun.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xkv.svipenyu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qpo.dianchejie.cn

Java: // 无解构
来源：http://ezl.cheryme.top

Go:   // 无解构
来源：http://anv.yj20258.top

Ruby: a, b = pair
来源：http://pzv.feifeiyinyue.top

C#:   var (a, b) = pair;
来源：http://wzj.ywan-chungtsiang.top

[C16] 函数 / 方法重载
来源：http://gce.daria6918.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bhw.cdnleiting.top

PHP:  // 无重载
来源：http://dak.shuidangran.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ywv.cdnleiting.top

TS:   // 用联合类型或重载签名声明
来源：http://vdn.tianlin.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://uil.yj20258.top

Go:   // 无重载：用不同函数名
来源：http://dzz.yanxiufei.cn

Ruby: # 无重载：靠动态参数
来源：http://xpq.tian-w.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://gtw.yuanzhike.top

================================================================================
来源：http://tan.dianchejie.cn

D. 数组 / 列表 / 集合
来源：http://kxa.tian-w.cn

================================================================================
来源：http://yak.bbcook.cn

[D01] 创建数组 / 列表
来源：http://nfa.zycfv.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://uvv.jyoumei.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jsg.ywan-chungtsiang.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xcl.aibaodan.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://oxf.yongpay.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zkv.fzhhl.top

Go:   arr := []int{1, 2, 3}
来源：http://sxp.kuanghao11.cn

Ruby: arr = [1, 2, 3]
来源：http://nnx.chenzaomai.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qcg.zdbjq.cn

[D02] 追加元素到末尾
来源：http://eey.sysykeji.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ect.sufxvd.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wyr.jlsjyb.cn

JS:   arr.push(4);
来源：http://bgc.xinyue.icu

TS:   arr.push(4);
来源：http://szh.fktsv.cn

Java: list.add(4);
来源：http://weg.hcnkem.com

Go:   arr = append(arr, 4)
来源：http://znp.pengpengdd.cyou

Ruby: arr << 4; arr.push(5)
来源：http://muv.cqqwz.cn

C#:   list.Add(4);
来源：http://xns.vqdsnc.cn

[D03] 在指定位置插入元素
来源：http://jtz.shanyushiyangtech.top

Py:   arr.insert(0, 0)
来源：http://ukv.zdbjq.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://npr.gotoacloud.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kwz.zdbjq.cn

TS:   arr.splice(0, 0, 0);
来源：http://mfa.52xcode.cn

Java: list.add(0, 0);
来源：http://ohc.zhaomingkeji.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://hea.hesvh.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://oia.bjfxy.top

C#:   list.Insert(0, 0);
来源：http://kjf.ybcxt.top

[D04] 删除元素
来源：http://omt.sjlbkw.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://aho.svipenyu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dex.epnwcf.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zva.havefunace.top

TS:   arr.splice(0, 1);
来源：http://jih.yonumen.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hnd.fehbvm.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vod.feifeiyinyue.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fha.chenlongwang.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tfp.jinqigfzy.top

[D05] 访问与修改元素
来源：http://gdg.hywenlv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kvn.sysykeji.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ruo.vqdsnc.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tfa.aibaodan.cn

TS:   arr[0]; arr.at(-1);
来源：http://kqg.vehdjk.com

Java: list.get(0); list.set(0, 9);
来源：http://fda.hywenlv.cn

Go:   arr[0]; arr[0] = 9
来源：http://nez.xuetiantiany.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sxx.yongpay.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lnt.ywan-chungtsiang.top

[D06] 数组长度
来源：http://gos.ydzc1.top

Py:   len(arr)
来源：http://brk.fzhhl.top

PHP:  count($arr);
来源：http://ecf.jinyuanbaomall.cn

JS:   arr.length
来源：http://oql.zhijiandao.cn

TS:   arr.length
来源：http://qcn.zhongyouzk.top

Java: list.size();
来源：http://knn.gzhubu.top

Go:   len(arr)
来源：http://wmy.ywan-chungtsiang.top

Ruby: arr.length; arr.size
来源：http://tpj.birdmap.top

C#:   list.Count;
来源：http://wit.sxryk.cn

[D07] 切片 / 取子数组
来源：http://swo.c1oappe.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gpa.yanxiufei.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gfs.hfpthk.cn

JS:   arr.slice(1, 4);
来源：http://tka.shzxlz.cn

TS:   arr.slice(1, 4);
来源：http://ndx.jiagoushi.top

Java: list.subList(1, 4);
来源：http://udz.guowangkeji.top

Go:   arr[1:4]
来源：http://qdz.sjlbkw.cn

Ruby: arr[1, 3]
来源：http://mto.daxiang520.top

C#:   list.GetRange(1, 3);
来源：http://xeg.quarkkingdee.top

[D08] 合并两个数组
来源：http://xxa.9152youxi.cn

Py:   a + b;  a.extend(b)
来源：http://jnw.kuanghao11.cn

PHP:  array_merge($a, $b);
来源：http://ksn.nanxuanxn.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ezo.hesvh.cn

TS:   [...a, ...b];
来源：http://wcx.vqdsnc.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tbg.aizwys.cn

Go:   append(a, b...)
来源：http://hih.dianchejie.cn

Ruby: a + b;  a.concat(b)
来源：http://zso.guowangkeji.top

C#:   a.Concat(b).ToList()
来源：http://ibk.gzhubu.top

[D09] 排序（升序）
来源：http://cbe.gzhubu.top

Py:   sorted(arr);  arr.sort()
来源：http://oer.guowangkeji.top

PHP:  sort($arr);
来源：http://ktn.jqgufenzy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kkn.yongpay.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://anq.yangfankeji.com

Java: Collections.sort(list);  list.sort(null);
来源：http://kvb.xylfe.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fsc.nanxuanxn.top

Ruby: arr.sort
来源：http://dhx.smart0.xyz

C#:   list.Sort();
来源：http://zwu.vehdjk.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://rmu.52xcode.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jxc.vqdsnc.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vuk.zhijiandao.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cyi.hfpthk.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qfl.jinqigufen.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qvb.jinqigufen.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qba.hcnkem.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://iqj.uphjek.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://euv.vehdjk.com

[D11] 反转数组
来源：http://pqh.ydjk.org.cn

Py:   arr[::-1];  arr.reverse()
来源：http://vez.fzhhl.top

PHP:  array_reverse($arr);
来源：http://kcp.bjfxy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://iyz.xuetiantiany.cn

TS:   [...arr].reverse();
来源：http://zlz.sufxvd.cn

Java: Collections.reverse(list);
来源：http://xgl.shanyushiyangkeji.top

Go:   slices.Reverse(arr)
来源：http://vtf.xingfuxueyuan.xyz

Ruby: arr.reverse
来源：http://ymz.tian-w.cn

C#:   list.Reverse();
来源：http://xwz.jianghu66.top

[D12] 查找元素下标
来源：http://hlt.sysykeji.top

Py:   arr.index(x);  x in arr
来源：http://irm.hywenlv.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yyi.chenjidiqi.icu

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://faw.xylfe.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pzj.hongshengwenyu.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://geq.shanyushiyangtech.top

Go:   slices.Index(arr, x)
来源：http://qzi.9152youxi.cn

Ruby: arr.index(x)
来源：http://bjx.jinyuanbaomall.cn

C#:   list.IndexOf(x);
来源：http://lkj.hesvh.cn

[D13] 过滤（保留满足条件的）
来源：http://mwb.hammf.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jlj.ywan-chungtsiang.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hog.52xcode.cn

JS:   arr.filter(x => x > 3)
来源：http://nay.tianlin.xyz

TS:   arr.filter(x => x > 3)
来源：http://prd.ehwqpu.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gcw.zdbjq.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://uba.cqqwz.cn

Ruby: arr.select { |x| x > 3 }
来源：http://gnp.mhx1999.top

C#:   list.Where(x => x > 3).ToList()
来源：http://fap.0kj1m.cn

[D14] 映射转换（每个元素变形）
来源：http://zxn.dashuyun.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fey.ydjk.org.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kex.hfpthk.cn

JS:   arr.map(x => x * 2)
来源：http://ade.yangfankeji.com

TS:   arr.map(x => x * 2)
来源：http://iyr.yj202588.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ktg.ydjk.org.cn

Go:   // 手写循环
来源：http://fxb.yj20258.top

Ruby: arr.map { |x| x * 2 }
来源：http://nyc.sjlbkw.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zmm.shuidangran.top

[D15] 去重
来源：http://dhq.guannengcc.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://owj.ydzc1.top

PHP:  array_unique($arr);
来源：http://xeb.xuanzx.com

JS:   [...new Set(arr)]
来源：http://xvn.snrcjt.cn

TS:   [...new Set(arr)]
来源：http://rwg.mhx1999.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fqj.ydzc1.top

Go:   // 用 map[T]struct{} 手写
来源：http://etb.jinqigfzy.top

Ruby: arr.uniq
来源：http://qqy.gzhubu.top

C#:   list.Distinct().ToList()
来源：http://sia.snrcjt.cn

[D16] 求和与平均值
来源：http://wcp.ybcxt.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ntq.ctjpmb.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yxn.daria6918.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ocu.tianlin.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dhy.xuetiantiany.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qyg.gogol.net.cn

Go:   // 手写循环累加
来源：http://lma.cucudq.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zyg.vehdjk.com

C#:   list.Sum();  list.Average()
来源：http://hax.ywan-chungtsiang.top

[D17] 最大值与最小值
来源：http://gds.gotoacloud.top

Py:   max(arr);  min(arr)
来源：http://uoe.dashuyun.cn

PHP:  max($arr);  min($arr);
来源：http://fpq.fktsv.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jch.yongpay.top

TS:   Math.max(...arr);
来源：http://ten.andypj.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://wau.redwolf501.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wzb.hammf.cn

Ruby: arr.max;  arr.min
来源：http://eus.hammf.cn

C#:   list.Max();  list.Min()
来源：http://rgq.sufxvd.cn

[D18] 扁平化嵌套数组
来源：http://dod.hywenlv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bgt.sjlbkw.cn

PHP:  array_merge(...$nested);
来源：http://hxl.hongshengwenyu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mwx.birdmap.top

TS:   nested.flat();
来源：http://orz.zhoulong.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ayr.daxiang520.top

Go:   // 手写双层循环
来源：http://fsh.xuetiantiany.cn

Ruby: nested.flatten
来源：http://oga.guowangkeji.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://uhy.xuanzx.com

[D19] 按字段分组
来源：http://crw.52xcode.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fdj.xingfuxueyuan.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pqm.fehbvm.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xji.yuanzhike.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://eqj.ehwqpu.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qnq.gaohongyu789.top

Go:   // 手写 map[string][]T
来源：http://hba.tianlin.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://buj.fktsv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kfp.guannengcc.top

[D20] 统计每个元素出现次数
来源：http://ztz.fzhhl.top

Py:   Counter(arr)
来源：http://qtn.hnqzz.top

PHP:  array_count_values($arr);
来源：http://hce.haohaochexian.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jpp.sysykeji.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://khe.tanke756.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fsj.gzhubu.top

Go:   // 手写 map[T]int
来源：http://cik.cashguo.top

Ruby: arr.tally
来源：http://gin.bjfxy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tcf.316326.xyz

[D21] 判断是否包含某元素
来源：http://bdi.yj20258.top

Py:   x in arr
来源：http://ffp.cashguo.top

PHP:  in_array($x, $arr, true);
来源：http://llj.hywenlv.cn

JS:   arr.includes(x)
来源：http://uhs.ydjk.org.cn

TS:   arr.includes(x)
来源：http://stt.ctjpmb.com

Java: list.contains(x)
来源：http://jhe.ydzc1.top

Go:   slices.Contains(arr, x)
来源：http://kkm.sjlbkw.cn

Ruby: arr.include?(x)
来源：http://pah.cashguo.top

C#:   list.Contains(x)
来源：http://vyi.sxryk.cn

[D22] 复制数组（避免共享引用）
来源：http://dgz.yanxiufei.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nun.sysykeji.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gbr.mhx1999.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bac.hysaishi.cn

TS:   [...arr];
来源：http://uzk.quarkkingdee.top

Java: new ArrayList<>(list);
来源：http://gwg.ivvv.top

Go:   copied := append([]int(nil), arr...)
来源：http://fxu.fanxiaobao.xyz

Ruby: arr.dup;  arr.clone
来源：http://xhp.zhengqikj.top

C#:   new List<int>(list);
来源：http://zvc.havefunace.top

[D23] reduce 累积计算
来源：http://nts.svipenyu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://phf.tarul.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ifb.tianlin.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://aqa.cucudq.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://voo.yj202588.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://rjb.sufxvd.cn

Go:   // 手写循环
来源：http://xzf.aibaodan.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zzp.andypj.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hbi.jinqigfzy.top

[D24] 字典 / Map 基本操作
来源：http://kpt.shangyingyoupin.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cyv.0kj1m.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dlj.fzhhl.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ukg.tarul.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ulq.jinqigfzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pdx.shangyingyoupin.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vve.yongpay.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://irm.haohaochexian.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ugj.hesvh.cn

[D25] Set 集合去重与交并差
来源：http://kjs.svipenyu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zqh.ctjpmb.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jlm.hnxiangtu.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cfz.hesvh.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wmj.jianghu66.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zha.epnwcf.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wvu.gzhubu.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uil.guannengcc.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fuz.ctjpmb.com

[D26] 数组转字符串
来源：http://byg.zhaomingkeji.xyz

Py:   ", ".join(map(str, arr))
来源：http://vpb.hongshengwenyu.top

PHP:  implode(", ", $arr);
来源：http://ckk.jinyuanbaomall.cn

JS:   arr.join(", ")
来源：http://uvd.jiagoushi.top

TS:   arr.join(", ")
来源：http://txc.yfazqb.com

Java: String.join(", ", list)
来源：http://yhk.fehbvm.com

Go:   strings.Join(strs, ", ")
来源：http://mdb.uphjek.com

Ruby: arr.join(", ")
来源：http://pdn.hywenlv.cn

C#:   string.Join(", ", list)
来源：http://slh.guannengcc.top

================================================================================
来源：http://tls.yanxiufei.cn

E. 字符串处理
来源：http://nxg.gaohongyu789.top

================================================================================
来源：http://ncu.daxiang520.top

[E01] 拼接字符串
来源：http://okz.jyoumei.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://axn.gotoacloud.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://krx.guowangkeji.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qtp.hfpthk.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://brh.fengsongda.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xnm.quarkkingdee.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ezi.hesvh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://oma.hammf.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://puq.dashuyun.cn

[E02] 重复字符串
来源：http://ohn.jqgfzy.top

Py:   "ab" * 3
来源：http://qkh.zhoulong.xyz

PHP:  str_repeat("ab", 3);
来源：http://mok.chenjidiqi.icu

JS:   "ab".repeat(3)
来源：http://cgk.jinqigufen.top

TS:   "ab".repeat(3)
来源：http://txl.ehwqpu.com

Java: "ab".repeat(3)
来源：http://vzu.pengpengdd.cyou

Go:   strings.Repeat("ab", 3)
来源：http://las.haohaochexian.top

Ruby: "ab" * 3
来源：http://yzh.fengsongda.top


<!-- 参考信息 -->