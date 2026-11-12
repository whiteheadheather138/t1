代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://mrt.shuidangran.top

JS:   (() => { console.log("run"); })();
来源：http://icu.shuidangran.top

TS:   (() => { console.log("run"); })();
来源：http://aqu.c1oappe.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pjc.quarkkingdee.top

Go:   func() { fmt.Println("run") }()
来源：http://zft.ehwqpu.com

Ruby: -> { puts "run" }.call
来源：http://gjc.redwolf501.top

C#:   // 无 IIFE：用静态构造函数
来源：http://zad.52xcode.cn

[C13] 类型声明 / 类型注解
来源：http://ddp.hesvh.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ikd.yangfankeji.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wpk.yfazqb.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vcg.smart0.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zaq.mhx1999.top

Java: int add(int a, int b) { return a + b; }
来源：http://djz.52xcode.cn

Go:   func add(a, b int) int
来源：http://cuu.dianchejie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ylw.gaohongyu789.top

C#:   int Add(int a, int b) => a + b;
来源：http://vis.zdqjudy.top

[C14] 泛型函数
来源：http://fmf.yfazqb.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xdv.cqqwz.cn

PHP:  // 无泛型
来源：http://yle.vqdsnc.cn

JS:   // 无泛型
来源：http://ggq.feifeiyinyue.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://arh.snrcjt.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://per.fehbvm.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mhz.yfazqb.com

Ruby: # 无泛型
来源：http://oav.ybcxt.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hfb.ybcxt.top

[C15] 解构 / 展开参数
来源：http://jve.zhaomingkeji.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gxs.jinghuilouyu.cn

PHP:  [$a, $b] = $pair;
来源：http://zfn.yj202588.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mbt.ppjwa.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yof.havefunace.top

Java: // 无解构
来源：http://qzp.c1oappe.top

Go:   // 无解构
来源：http://xsf.sjlbkw.cn

Ruby: a, b = pair
来源：http://gor.guannengcc.top

C#:   var (a, b) = pair;
来源：http://atv.vehdjk.com

[C16] 函数 / 方法重载
来源：http://nwh.havefunace.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jtn.shuidangran.top

PHP:  // 无重载
来源：http://vuf.cqqwz.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://cib.hnqzz.top

TS:   // 用联合类型或重载签名声明
来源：http://qra.chenlongwang.top

Java: void f(int a) {}  void f(String a) {}
来源：http://cbd.hongshengwenyu.top

Go:   // 无重载：用不同函数名
来源：http://otf.fehbvm.com

Ruby: # 无重载：靠动态参数
来源：http://uhz.svipenyu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://tyz.fzhhl.top

================================================================================
来源：http://qqs.ivvv.top

D. 数组 / 列表 / 集合
来源：http://grm.hesvh.cn

================================================================================
来源：http://tdh.cashguo.top

[D01] 创建数组 / 列表
来源：http://mdz.fanxiaobao.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://naa.redwolf501.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vcq.shanyushiyangtech.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yoy.xziqi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://rlw.c1oappe.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cyh.hesvh.cn

Go:   arr := []int{1, 2, 3}
来源：http://bci.316326.xyz

Ruby: arr = [1, 2, 3]
来源：http://mns.bjfxy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tnm.jqgfzy.top

[D02] 追加元素到末尾
来源：http://yyi.xingfuxueyuan.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vpd.ybcxt.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qiv.jiagoushi.top

JS:   arr.push(4);
来源：http://trv.gotoacloud.top

TS:   arr.push(4);
来源：http://acg.jlsjyb.cn

Java: list.add(4);
来源：http://ars.wangshuangyany.cn

Go:   arr = append(arr, 4)
来源：http://mwh.hywenlv.cn

Ruby: arr << 4; arr.push(5)
来源：http://sqa.tanke756.top

C#:   list.Add(4);
来源：http://cjm.sysykeji.top

[D03] 在指定位置插入元素
来源：http://leo.yuanzhike.top

Py:   arr.insert(0, 0)
来源：http://ove.jinqigfzy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tgd.xinyue.icu

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hyq.ppjwa.cn

TS:   arr.splice(0, 0, 0);
来源：http://mdm.hcnkem.com

Java: list.add(0, 0);
来源：http://gqm.bbcook.cn

Go:   arr = append([]int{0}, arr...)
来源：http://hkt.yj202588.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pxb.jinqigufen.top

C#:   list.Insert(0, 0);
来源：http://kab.snrcjt.cn

[D04] 删除元素
来源：http://gyw.yueranfly.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://whr.dashuyun.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zjw.zhengqikj.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fml.316326.xyz

TS:   arr.splice(0, 1);
来源：http://cvp.yuxming.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cbs.zhaomingkeji.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://oji.iojbl.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qdf.gogol.net.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lju.hysaishi.cn

[D05] 访问与修改元素
来源：http://upk.yongpay.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lpt.sweek.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://enx.cashguo.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://oxk.zhengqikj.top

TS:   arr[0]; arr.at(-1);
来源：http://qxw.yangfankeji.com

Java: list.get(0); list.set(0, 9);
来源：http://vfi.chenjidiqi.icu

Go:   arr[0]; arr[0] = 9
来源：http://mdb.shanyushiyangkeji.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kkj.316326.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qup.gotoacloud.top

[D06] 数组长度
来源：http://mfp.jinqigfzy.top

Py:   len(arr)
来源：http://gni.zhijiandao.cn

PHP:  count($arr);
来源：http://ayb.hesvh.cn

JS:   arr.length
来源：http://wmv.xinyue.icu

TS:   arr.length
来源：http://tux.tian-w.cn

Java: list.size();
来源：http://fkq.shanyushiyangkeji.top

Go:   len(arr)
来源：http://xsa.gzhubu.top

Ruby: arr.length; arr.size
来源：http://xor.aizwys.cn

C#:   list.Count;
来源：http://jhf.dashuyun.cn

[D07] 切片 / 取子数组
来源：http://aib.daria6918.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nja.hfpthk.cn

PHP:  array_slice($arr, 1, 3);
来源：http://cjg.xingfuxueyuan.xyz

JS:   arr.slice(1, 4);
来源：http://hxu.ivvv.top

TS:   arr.slice(1, 4);
来源：http://rek.fzhhl.top

Java: list.subList(1, 4);
来源：http://ges.shzxlz.cn

Go:   arr[1:4]
来源：http://jpm.yanxiufei.cn

Ruby: arr[1, 3]
来源：http://csn.cashguo.top

C#:   list.GetRange(1, 3);
来源：http://jck.cashguo.top

[D08] 合并两个数组
来源：http://ftb.bjfxy.top

Py:   a + b;  a.extend(b)
来源：http://uju.birdmap.top

PHP:  array_merge($a, $b);
来源：http://yta.tanke756.top

JS:   [...a, ...b];  a.concat(b);
来源：http://src.haohaochexian.top

TS:   [...a, ...b];
来源：http://rlz.hysaishi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ugo.0kj1m.cn

Go:   append(a, b...)
来源：http://aly.nanxinkj.top

Ruby: a + b;  a.concat(b)
来源：http://khy.ctjpmb.com

C#:   a.Concat(b).ToList()
来源：http://asd.hywenlv.cn

[D09] 排序（升序）
来源：http://pum.mhx1999.top

Py:   sorted(arr);  arr.sort()
来源：http://riv.jinqigufen.top

PHP:  sort($arr);
来源：http://cbz.vqdsnc.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wrc.ywan-chungtsiang.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://qax.tian-w.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://jbg.guowangkeji.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tms.jqgufenzy.top

Ruby: arr.sort
来源：http://lmr.cheryme.top

C#:   list.Sort();
来源：http://ryz.hnqzz.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://sqq.xylfe.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rwu.yanxiufei.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xvj.cqqwz.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lcx.9152youxi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nqr.nanxuanxn.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bal.gzhubu.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vum.chenzaomai.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://myz.cashguo.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zvh.sweek.top

[D11] 反转数组
来源：http://ayy.fengsongda.top

Py:   arr[::-1];  arr.reverse()
来源：http://bss.daria6918.cn

PHP:  array_reverse($arr);
来源：http://oig.ehwqpu.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://csj.pycfn.com

TS:   [...arr].reverse();
来源：http://luq.cqqwz.cn

Java: Collections.reverse(list);
来源：http://toe.hcnkem.com

Go:   slices.Reverse(arr)
来源：http://sxh.zdbjq.cn

Ruby: arr.reverse
来源：http://kml.nwbrower.top

C#:   list.Reverse();
来源：http://iff.yueranfly.top

[D12] 查找元素下标
来源：http://vzg.xziqi.cn

Py:   arr.index(x);  x in arr
来源：http://bgw.wangdashe.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ucn.chenzaomai.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qdt.shuidangran.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://peo.jqgfzy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lek.nanxuanxn.top

Go:   slices.Index(arr, x)
来源：http://rnj.gogol.net.cn

Ruby: arr.index(x)
来源：http://cjs.redwolf501.top

C#:   list.IndexOf(x);
来源：http://zsf.hammf.cn

[D13] 过滤（保留满足条件的）
来源：http://qcv.guowangkeji.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tys.c1oappe.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hph.xinyue.icu

JS:   arr.filter(x => x > 3)
来源：http://cnu.jyoumei.cn

TS:   arr.filter(x => x > 3)
来源：http://xve.pengpengdd.cyou

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zlw.chenlongwang.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://izi.fktsv.cn

Ruby: arr.select { |x| x > 3 }
来源：http://gbj.nwbrower.top

C#:   list.Where(x => x > 3).ToList()
来源：http://nck.52xcode.cn

[D14] 映射转换（每个元素变形）
来源：http://psz.tianlin.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wqm.zycfv.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mjf.hammf.cn

JS:   arr.map(x => x * 2)
来源：http://zgf.jlsjyb.cn

TS:   arr.map(x => x * 2)
来源：http://wgq.shzxlz.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vrx.ybcxt.top

Go:   // 手写循环
来源：http://uak.hcnkem.com

Ruby: arr.map { |x| x * 2 }
来源：http://wwu.daxiang520.top

C#:   list.Select(x => x * 2).ToList()
来源：http://dse.hcnkem.com

[D15] 去重
来源：http://nqu.yj20258.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yjh.cashguo.top

PHP:  array_unique($arr);
来源：http://qox.havefunace.top

JS:   [...new Set(arr)]
来源：http://jnm.jqgfzy.top

TS:   [...new Set(arr)]
来源：http://jeh.tianlin.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://abp.mhx1999.top

Go:   // 用 map[T]struct{} 手写
来源：http://ore.tanke756.top

Ruby: arr.uniq
来源：http://wjn.fengsongda.top

C#:   list.Distinct().ToList()
来源：http://lbh.yj20258.top

[D16] 求和与平均值
来源：http://myx.xziqi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://izp.svipenyu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mbz.andypj.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vlm.chenjidiqi.icu

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sti.ybcxt.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ylz.ivvv.top

Go:   // 手写循环累加
来源：http://jhj.chenlongwang.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tzu.kuanghao11.cn

C#:   list.Sum();  list.Average()
来源：http://iks.aizwys.cn

[D17] 最大值与最小值
来源：http://hjs.shangyingyoupin.top

Py:   max(arr);  min(arr)
来源：http://bcj.guannengcc.top

PHP:  max($arr);  min($arr);
来源：http://sip.yanxiufei.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fxh.daxiang520.top

TS:   Math.max(...arr);
来源：http://ylc.guannengcc.top

Java: Collections.max(list);  Collections.min(list);
来源：http://car.nwbrower.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ohx.pycfn.com

Ruby: arr.max;  arr.min
来源：http://ixb.xinyue.icu

C#:   list.Max();  list.Min()
来源：http://wrt.zycfv.cn

[D18] 扁平化嵌套数组
来源：http://hji.c1oappe.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ikj.ybcxt.top

PHP:  array_merge(...$nested);
来源：http://zxs.jinqigufen.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hlw.zycfv.cn

TS:   nested.flat();
来源：http://vuv.dianchejie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://voi.gaohongyu789.top

Go:   // 手写双层循环
来源：http://wgh.xuanzx.com

Ruby: nested.flatten
来源：http://yaz.cucudq.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://itl.tian-w.cn

[D19] 按字段分组
来源：http://gnf.gaohongyu789.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hpe.yvedp.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xgc.andypj.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qxo.daria6918.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zqv.yangfankeji.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hbx.jlsjyb.cn

Go:   // 手写 map[string][]T
来源：http://les.bbcook.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vbr.ywan-chungtsiang.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qrg.cucudq.cn

[D20] 统计每个元素出现次数
来源：http://nde.fzhhl.top

Py:   Counter(arr)
来源：http://poj.tarul.cn

PHP:  array_count_values($arr);
来源：http://miz.guowangkeji.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xdp.jinghuilouyu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tql.nanxinkj.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://evg.pycfn.com

Go:   // 手写 map[T]int
来源：http://ato.xylfe.cn

Ruby: arr.tally
来源：http://pdq.svipenyu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ciu.hfpthk.cn

[D21] 判断是否包含某元素
来源：http://svo.ivvv.top

Py:   x in arr
来源：http://kit.cashguo.top

PHP:  in_array($x, $arr, true);
来源：http://wwv.shangyingyoupin.top

JS:   arr.includes(x)
来源：http://mly.uphjek.com

TS:   arr.includes(x)
来源：http://wwc.mhx1999.top

Java: list.contains(x)
来源：http://ewx.316326.xyz

Go:   slices.Contains(arr, x)
来源：http://jgx.gzhubu.top

Ruby: arr.include?(x)
来源：http://vzz.vehdjk.com

C#:   list.Contains(x)
来源：http://eiw.yonumen.top

[D22] 复制数组（避免共享引用）
来源：http://acn.yfazqb.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gld.shanyushiyangtech.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yqu.bjfxy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rfn.svipenyu.cn

TS:   [...arr];
来源：http://zuz.shanyushiyangkeji.top

Java: new ArrayList<>(list);
来源：http://lva.chenjidiqi.icu

Go:   copied := append([]int(nil), arr...)
来源：http://mnn.9152youxi.cn

Ruby: arr.dup;  arr.clone
来源：http://wbk.gogol.net.cn

C#:   new List<int>(list);
来源：http://rtx.ybcxt.top

[D23] reduce 累积计算
来源：http://wkf.cucudq.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jpq.zhiwuduotai.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fep.ehwqpu.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://osw.aizwys.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oej.zdqjudy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://pvv.aibaodan.cn

Go:   // 手写循环
来源：http://qfs.epnwcf.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qoo.xuetiantiany.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ocu.hfpthk.cn

[D24] 字典 / Map 基本操作
来源：http://vrx.yj202588.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nsa.hywenlv.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ibf.fktsv.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yfv.gotoacloud.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nvy.zhiwuduotai.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mme.c1oappe.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wlb.ehwqpu.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://thm.bjfxy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://epn.yj20258.top

[D25] Set 集合去重与交并差
来源：http://bnw.316326.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gjj.sysykeji.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hll.pycfn.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kxh.zhiwuduotai.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wsi.hnxiangtu.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nks.aibaodan.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://daf.tarul.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://czg.yfazqb.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pct.dianchejie.cn

[D26] 数组转字符串
来源：http://ane.xingfuxueyuan.xyz

Py:   ", ".join(map(str, arr))
来源：http://jcj.mhx1999.top

PHP:  implode(", ", $arr);
来源：http://mfq.havefunace.top

JS:   arr.join(", ")
来源：http://zcv.zhijiandao.cn

TS:   arr.join(", ")
来源：http://hms.aizwys.cn

Java: String.join(", ", list)
来源：http://kqs.tanke756.top

Go:   strings.Join(strs, ", ")
来源：http://ggy.yongpay.top

Ruby: arr.join(", ")
来源：http://tzf.jinghuilouyu.cn

C#:   string.Join(", ", list)
来源：http://vde.yongpay.top

================================================================================
来源：http://nli.jqgufenzy.top

E. 字符串处理
来源：http://iog.snrcjt.cn

================================================================================
来源：http://uxe.zdqjudy.top

[E01] 拼接字符串
来源：http://ans.yj202588.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dil.wangdashe.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vrq.xingfuxueyuan.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yof.jinghuilouyu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://phl.mhx1999.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qob.cqqwz.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pra.0kj1m.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nww.haohaochexian.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ntb.fanxiaobao.xyz

[E02] 重复字符串
来源：http://upg.shangyingyoupin.top

Py:   "ab" * 3
来源：http://gsy.pengpengdd.cyou

PHP:  str_repeat("ab", 3);
来源：http://wuk.yj20258888.top

JS:   "ab".repeat(3)
来源：http://fru.bbcook.cn

TS:   "ab".repeat(3)
来源：http://vac.hcnkem.com

Java: "ab".repeat(3)
来源：http://ugq.vehdjk.com

Go:   strings.Repeat("ab", 3)
来源：http://szb.cheryme.top

Ruby: "ab" * 3
来源：http://zel.fehbvm.com


<!-- 参考信息 -->