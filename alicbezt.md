代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://lti.yonumen.top

JS:   (() => { console.log("run"); })();
来源：http://qxk.aizwys.cn

TS:   (() => { console.log("run"); })();
来源：http://pqo.hfpthk.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qdi.yonumen.top

Go:   func() { fmt.Println("run") }()
来源：http://tfr.hywenlv.cn

Ruby: -> { puts "run" }.call
来源：http://jwk.pengpengdd.cyou

C#:   // 无 IIFE：用静态构造函数
来源：http://mdv.gzhubu.top

[C13] 类型声明 / 类型注解
来源：http://btb.yanxiufei.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jgp.ywan-chungtsiang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kks.sufxvd.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://iou.52xcode.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nao.birdmap.top

Java: int add(int a, int b) { return a + b; }
来源：http://jlc.zhongyouzk.top

Go:   func add(a, b int) int
来源：http://cvh.tianlin.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fsx.jqgfzy.top

C#:   int Add(int a, int b) => a + b;
来源：http://nhn.birdmap.top

[C14] 泛型函数
来源：http://puq.nanxuanxn.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qhd.meibo888.top

PHP:  // 无泛型
来源：http://xkn.nanxinkj.top

JS:   // 无泛型
来源：http://tzr.shzxlz.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fep.xingfuxueyuan.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wpb.ybcxt.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wog.dianchejie.cn

Ruby: # 无泛型
来源：http://dgu.hnqzz.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://uhx.hfpthk.cn

[C15] 解构 / 展开参数
来源：http://ouz.ppjwa.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gya.daria6918.cn

PHP:  [$a, $b] = $pair;
来源：http://qgh.hfpthk.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mxg.jinyuanbaomall.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://obf.jinqigufen.top

Java: // 无解构
来源：http://vww.zhaomingkeji.xyz

Go:   // 无解构
来源：http://fgz.316326.xyz

Ruby: a, b = pair
来源：http://reb.epnwcf.com

C#:   var (a, b) = pair;
来源：http://hno.nanxuanxn.top

[C16] 函数 / 方法重载
来源：http://jdp.52xcode.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tzs.zhaomingkeji.xyz

PHP:  // 无重载
来源：http://nlm.haohaochexian.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://kic.yvedp.cn

TS:   // 用联合类型或重载签名声明
来源：http://bno.xuanzx.com

Java: void f(int a) {}  void f(String a) {}
来源：http://sfw.hnxiangtu.top

Go:   // 无重载：用不同函数名
来源：http://vkk.hesvh.cn

Ruby: # 无重载：靠动态参数
来源：http://sec.gzhubu.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://hsq.jinqigufen.top

================================================================================
来源：http://bdg.andypj.xyz

D. 数组 / 列表 / 集合
来源：http://gtj.316326.xyz

================================================================================
来源：http://zhc.zhijiandao.cn

[D01] 创建数组 / 列表
来源：http://kah.xingfuxueyuan.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://prs.snrcjt.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tgf.jinghuilouyu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://juk.zdqjudy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ovj.hammf.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bsi.andypj.xyz

Go:   arr := []int{1, 2, 3}
来源：http://svp.daxiang520.top

Ruby: arr = [1, 2, 3]
来源：http://ixl.cheryme.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kpu.andypj.xyz

[D02] 追加元素到末尾
来源：http://ccn.jlsjyb.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jem.sjlbkw.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jwz.fzhhl.top

JS:   arr.push(4);
来源：http://kai.kuanghao11.cn

TS:   arr.push(4);
来源：http://qbg.yueranfly.top

Java: list.add(4);
来源：http://rav.hongshengwenyu.top

Go:   arr = append(arr, 4)
来源：http://enk.cqqwz.cn

Ruby: arr << 4; arr.push(5)
来源：http://nse.bbcook.cn

C#:   list.Add(4);
来源：http://xif.52xcode.cn

[D03] 在指定位置插入元素
来源：http://zqi.vqdsnc.cn

Py:   arr.insert(0, 0)
来源：http://ijf.dashuyun.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ahn.gogol.net.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wsx.zhengqikj.top

TS:   arr.splice(0, 0, 0);
来源：http://ujw.daria6918.cn

Java: list.add(0, 0);
来源：http://mjl.jqgfzy.top

Go:   arr = append([]int{0}, arr...)
来源：http://njp.xylfe.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ikt.svipenyu.cn

C#:   list.Insert(0, 0);
来源：http://gsb.zhixingplan.top

[D04] 删除元素
来源：http://iwz.yuanzhike.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xfk.tianlin.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://scs.cucudq.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ons.daria6918.cn

TS:   arr.splice(0, 1);
来源：http://jjj.zdqjudy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cdj.cqqwz.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yre.guannengcc.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://sry.zhaomingkeji.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rkx.birdmap.top

[D05] 访问与修改元素
来源：http://get.jinyuanbaomall.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ase.fanxiaobao.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kjx.fktsv.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dkn.daxiang520.top

TS:   arr[0]; arr.at(-1);
来源：http://yav.guannengcc.top

Java: list.get(0); list.set(0, 9);
来源：http://xfz.316326.xyz

Go:   arr[0]; arr[0] = 9
来源：http://xhv.wangdashe.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://egc.sjlbkw.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qtp.dashuyun.cn

[D06] 数组长度
来源：http://tlh.sxryk.cn

Py:   len(arr)
来源：http://jbs.yangfankeji.com

PHP:  count($arr);
来源：http://awh.zhixingplan.top

JS:   arr.length
来源：http://qqr.yangfankeji.com

TS:   arr.length
来源：http://jah.dashuyun.cn

Java: list.size();
来源：http://qvr.cashguo.top

Go:   len(arr)
来源：http://xhg.nwbrower.top

Ruby: arr.length; arr.size
来源：http://hru.uphjek.com

C#:   list.Count;
来源：http://swd.gaohongyu789.top

[D07] 切片 / 取子数组
来源：http://llk.tian-w.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tew.nanxuanxn.top

PHP:  array_slice($arr, 1, 3);
来源：http://uvh.jiagoushi.top

JS:   arr.slice(1, 4);
来源：http://rgs.cashguo.top

TS:   arr.slice(1, 4);
来源：http://xeb.gzhubu.top

Java: list.subList(1, 4);
来源：http://pre.shanyushiyangkeji.top

Go:   arr[1:4]
来源：http://pac.jqgfzy.top

Ruby: arr[1, 3]
来源：http://kjf.ppjwa.cn

C#:   list.GetRange(1, 3);
来源：http://kvy.gogol.net.cn

[D08] 合并两个数组
来源：http://hfb.birdmap.top

Py:   a + b;  a.extend(b)
来源：http://xhi.guowangkeji.top

PHP:  array_merge($a, $b);
来源：http://ald.xylfe.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gyd.xuetiantiany.cn

TS:   [...a, ...b];
来源：http://hlv.uphjek.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hrg.jinghuilouyu.cn

Go:   append(a, b...)
来源：http://ggf.pengpengdd.cyou

Ruby: a + b;  a.concat(b)
来源：http://olx.redwolf501.top

C#:   a.Concat(b).ToList()
来源：http://syl.pycfn.com

[D09] 排序（升序）
来源：http://rde.c1oappe.top

Py:   sorted(arr);  arr.sort()
来源：http://uan.shanyushiyangkeji.top

PHP:  sort($arr);
来源：http://jbe.haohaochexian.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://iyu.zhoulong.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://xed.gzhubu.top

Java: Collections.sort(list);  list.sort(null);
来源：http://slo.jlsjyb.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rim.cdnleiting.top

Ruby: arr.sort
来源：http://zln.mhx1999.top

C#:   list.Sort();
来源：http://eif.ydjk.org.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ysh.yj20258888.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://iym.xuetiantiany.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zqf.jinqigufen.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://flj.cheryme.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fid.shangyingyoupin.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gyv.aizwys.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bqp.andypj.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rnl.birdmap.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xrr.hfpthk.cn

[D11] 反转数组
来源：http://iin.fzhhl.top

Py:   arr[::-1];  arr.reverse()
来源：http://ygw.nanxinkj.top

PHP:  array_reverse($arr);
来源：http://tum.52xcode.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gzf.nanxinkj.top

TS:   [...arr].reverse();
来源：http://ctr.dianchejie.cn

Java: Collections.reverse(list);
来源：http://upj.sufxvd.cn

Go:   slices.Reverse(arr)
来源：http://mte.yvedp.cn

Ruby: arr.reverse
来源：http://ztc.tianlin.xyz

C#:   list.Reverse();
来源：http://oah.fzhhl.top

[D12] 查找元素下标
来源：http://dvv.vqdsnc.cn

Py:   arr.index(x);  x in arr
来源：http://asv.52xcode.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vpj.hcnkem.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pjj.gzhubu.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nyn.bjfxy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vtj.ywan-chungtsiang.top

Go:   slices.Index(arr, x)
来源：http://oxe.yj20258.top

Ruby: arr.index(x)
来源：http://sjp.xinyue.icu

C#:   list.IndexOf(x);
来源：http://jgi.iojbl.cn

[D13] 过滤（保留满足条件的）
来源：http://buj.yuxming.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gqo.ybcxt.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://uug.tanke756.top

JS:   arr.filter(x => x > 3)
来源：http://ask.zhiwuduotai.top

TS:   arr.filter(x => x > 3)
来源：http://zbt.tianlin.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zjm.daxiang520.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://emd.zycfv.cn

Ruby: arr.select { |x| x > 3 }
来源：http://blc.pengpengdd.cyou

C#:   list.Where(x => x > 3).ToList()
来源：http://fba.dashuyun.cn

[D14] 映射转换（每个元素变形）
来源：http://eov.zhoulong.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lyz.jinqigfzy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nxa.hnqzz.top

JS:   arr.map(x => x * 2)
来源：http://vrh.shzxlz.cn

TS:   arr.map(x => x * 2)
来源：http://oiz.shangyingyoupin.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://clr.xuetiantiany.cn

Go:   // 手写循环
来源：http://ldm.hesvh.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wmt.zhaomingkeji.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://lqn.zycfv.cn

[D15] 去重
来源：http://phm.tanke756.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://chu.uphjek.com

PHP:  array_unique($arr);
来源：http://hcv.sufxvd.cn

JS:   [...new Set(arr)]
来源：http://kuc.zhixingplan.top

TS:   [...new Set(arr)]
来源：http://htx.havefunace.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kdb.chenjidiqi.icu

Go:   // 用 map[T]struct{} 手写
来源：http://dya.xingfuxueyuan.xyz

Ruby: arr.uniq
来源：http://hon.sysykeji.top

C#:   list.Distinct().ToList()
来源：http://szk.yj20258888.top

[D16] 求和与平均值
来源：http://wge.yongpay.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hkf.nanxinkj.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tlt.tian-w.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bsf.ehwqpu.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mry.yj20258.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mqs.xylfe.cn

Go:   // 手写循环累加
来源：http://psw.cucudq.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cvu.hnqzz.top

C#:   list.Sum();  list.Average()
来源：http://qdi.yanxiufei.cn

[D17] 最大值与最小值
来源：http://gpr.fanxiaobao.xyz

Py:   max(arr);  min(arr)
来源：http://itm.xziqi.cn

PHP:  max($arr);  min($arr);
来源：http://hdr.guowangkeji.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xmh.svipenyu.cn

TS:   Math.max(...arr);
来源：http://gjj.uphjek.com

Java: Collections.max(list);  Collections.min(list);
来源：http://ihu.zycfv.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fgt.gzhubu.top

Ruby: arr.max;  arr.min
来源：http://yrp.daxiang520.top

C#:   list.Max();  list.Min()
来源：http://rgl.daria6918.cn

[D18] 扁平化嵌套数组
来源：http://lnj.nanxuanxn.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://row.quarkkingdee.top

PHP:  array_merge(...$nested);
来源：http://pkg.c1oappe.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jlp.hfpthk.cn

TS:   nested.flat();
来源：http://tqz.daxiang520.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ywh.jlsjyb.cn

Go:   // 手写双层循环
来源：http://oty.pengpengdd.cyou

Ruby: nested.flatten
来源：http://tsm.nwbrower.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://xdo.tanke756.top

[D19] 按字段分组
来源：http://xnn.daria6918.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mcy.cucudq.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nyd.tian-w.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://usg.316326.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://hoe.haohaochexian.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zuo.hongshengwenyu.top

Go:   // 手写 map[string][]T
来源：http://vmd.tanke756.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://wip.zhiwuduotai.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://czc.xinyue.icu

[D20] 统计每个元素出现次数
来源：http://psp.zdqjudy.top

Py:   Counter(arr)
来源：http://zeq.andypj.xyz

PHP:  array_count_values($arr);
来源：http://umd.xuanzx.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kmq.sysykeji.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rqm.zhoulong.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://uth.sjlbkw.cn

Go:   // 手写 map[T]int
来源：http://zpf.hywenlv.cn

Ruby: arr.tally
来源：http://uwk.jyoumei.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xfu.epnwcf.com

[D21] 判断是否包含某元素
来源：http://vte.hnxiangtu.top

Py:   x in arr
来源：http://nxw.9152youxi.cn

PHP:  in_array($x, $arr, true);
来源：http://fbh.hongshengwenyu.top

JS:   arr.includes(x)
来源：http://zmb.gogol.net.cn

TS:   arr.includes(x)
来源：http://bjo.smart0.xyz

Java: list.contains(x)
来源：http://foc.yj202588.top

Go:   slices.Contains(arr, x)
来源：http://fqx.ydjk.org.cn

Ruby: arr.include?(x)
来源：http://joi.ydzc1.top

C#:   list.Contains(x)
来源：http://ghy.shangyingyoupin.top

[D22] 复制数组（避免共享引用）
来源：http://equ.cheryme.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nne.vehdjk.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pws.jyoumei.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fdf.ctjpmb.com

TS:   [...arr];
来源：http://cxv.yangfankeji.com

Java: new ArrayList<>(list);
来源：http://tcn.daria6918.cn

Go:   copied := append([]int(nil), arr...)
来源：http://rdy.52xcode.cn

Ruby: arr.dup;  arr.clone
来源：http://xra.feifeiyinyue.top

C#:   new List<int>(list);
来源：http://wso.tianlin.xyz

[D23] reduce 累积计算
来源：http://mkx.jianghu66.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wuk.xziqi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://erj.uphjek.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tlw.0kj1m.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hhx.wangdashe.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://bxb.316326.xyz

Go:   // 手写循环
来源：http://dmr.vehdjk.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dqn.cqqwz.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bfw.guowangkeji.top

[D24] 字典 / Map 基本操作
来源：http://pif.guannengcc.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://clw.gotoacloud.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tzg.bjfxy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blz.sjlbkw.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://civ.havefunace.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cpb.sweek.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dgf.zhongyouzk.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mpd.epnwcf.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lop.52xcode.cn

[D25] Set 集合去重与交并差
来源：http://rvj.nanxuanxn.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fir.0kj1m.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zoh.sjlbkw.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mjq.dianchejie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kcx.jiagoushi.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://niz.gzhubu.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fhp.yj20258.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://eis.zycfv.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://uyg.dianchejie.cn

[D26] 数组转字符串
来源：http://duo.ppjwa.cn

Py:   ", ".join(map(str, arr))
来源：http://gbd.hammf.cn

PHP:  implode(", ", $arr);
来源：http://rvd.cqqwz.cn

JS:   arr.join(", ")
来源：http://xoi.yonumen.top

TS:   arr.join(", ")
来源：http://rhf.jinghuilouyu.cn

Java: String.join(", ", list)
来源：http://pwz.quarkkingdee.top

Go:   strings.Join(strs, ", ")
来源：http://xtk.xuanzx.com

Ruby: arr.join(", ")
来源：http://ocp.yfazqb.com

C#:   string.Join(", ", list)
来源：http://zlx.hywenlv.cn

================================================================================
来源：http://vgc.snrcjt.cn

E. 字符串处理
来源：http://zno.pycfn.com

================================================================================
来源：http://rgu.jinqigufen.top

[E01] 拼接字符串
来源：http://lpb.wangshuangyany.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fxg.tianlin.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hnv.gotoacloud.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uzv.iojbl.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://edb.shuidangran.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vlp.zycfv.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pwc.fehbvm.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://awg.zdbjq.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mqq.hfpthk.cn

[E02] 重复字符串
来源：http://bzi.zhiwuduotai.top

Py:   "ab" * 3
来源：http://bke.uphjek.com

PHP:  str_repeat("ab", 3);
来源：http://mpy.yueranfly.top

JS:   "ab".repeat(3)
来源：http://bhc.fanxiaobao.xyz

TS:   "ab".repeat(3)
来源：http://vhm.iojbl.cn

Java: "ab".repeat(3)
来源：http://jsr.smart0.xyz

Go:   strings.Repeat("ab", 3)
来源：http://lhs.shzxlz.cn

Ruby: "ab" * 3
来源：http://dyt.xinyue.icu


<!-- 参考信息 -->