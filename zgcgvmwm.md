代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://bgf.bjfxy.top

Ruby: -> { puts "run" }.call
来源：http://adb.zhixingplan.top

C#:   // 无 IIFE：用静态构造函数
来源：http://iru.smart0.xyz

[C13] 类型声明 / 类型注解
来源：http://qxl.daxiang520.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rkh.fengsongda.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fmj.hnxiangtu.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lvb.jinyuanbaomall.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://orq.jianghu66.top

Java: int add(int a, int b) { return a + b; }
来源：http://jbi.wangshuangyany.cn

Go:   func add(a, b int) int
来源：http://xoi.xuanzx.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xdz.cucudq.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ljo.hesvh.cn

[C14] 泛型函数
来源：http://oxh.tarul.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pqk.jinqigfzy.top

PHP:  // 无泛型
来源：http://bux.snrcjt.cn

JS:   // 无泛型
来源：http://qsh.nanxinkj.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zwt.52xcode.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gry.zdqjudy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ycl.fktsv.cn

Ruby: # 无泛型
来源：http://mmk.fehbvm.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://phk.meibo888.top

[C15] 解构 / 展开参数
来源：http://qzp.zhongyouzk.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ndd.bbcook.cn

PHP:  [$a, $b] = $pair;
来源：http://wez.shangyingyoupin.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rdk.vehdjk.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wof.9152youxi.cn

Java: // 无解构
来源：http://anl.daria6918.cn

Go:   // 无解构
来源：http://vxd.sysykeji.top

Ruby: a, b = pair
来源：http://ilv.yj20258888.top

C#:   var (a, b) = pair;
来源：http://fwc.jinghuilouyu.cn

[C16] 函数 / 方法重载
来源：http://ooh.shangyingyoupin.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yut.gzhubu.top

PHP:  // 无重载
来源：http://ptp.aibaodan.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://dos.cucudq.cn

TS:   // 用联合类型或重载签名声明
来源：http://qoi.jinqigfzy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://xjf.fengsongda.top

Go:   // 无重载：用不同函数名
来源：http://odv.yj20258888.top

Ruby: # 无重载：靠动态参数
来源：http://dze.shuidangran.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://wwb.hnxiangtu.top

================================================================================
来源：http://ydd.xuetiantiany.cn

D. 数组 / 列表 / 集合
来源：http://jyv.haohaochexian.top

================================================================================
来源：http://zmn.xuanzx.com

[D01] 创建数组 / 列表
来源：http://fxf.haohaochexian.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://uwc.zdbjq.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jsx.fzhhl.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://eai.yueranfly.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://iiu.nanxinkj.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sqx.xziqi.cn

Go:   arr := []int{1, 2, 3}
来源：http://iii.guannengcc.top

Ruby: arr = [1, 2, 3]
来源：http://yts.yj20258888.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jfb.chenjidiqi.icu

[D02] 追加元素到末尾
来源：http://xiz.pycfn.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wjg.iojbl.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kvl.hywenlv.cn

JS:   arr.push(4);
来源：http://tnd.wangdashe.top

TS:   arr.push(4);
来源：http://duq.jyoumei.cn

Java: list.add(4);
来源：http://gzt.gaohongyu789.top

Go:   arr = append(arr, 4)
来源：http://ihx.zdqjudy.top

Ruby: arr << 4; arr.push(5)
来源：http://taw.cqqwz.cn

C#:   list.Add(4);
来源：http://owg.snrcjt.cn

[D03] 在指定位置插入元素
来源：http://zwh.yj20258.top

Py:   arr.insert(0, 0)
来源：http://ufk.yueranfly.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qqk.hnxiangtu.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wul.tarul.cn

TS:   arr.splice(0, 0, 0);
来源：http://qsn.uphjek.com

Java: list.add(0, 0);
来源：http://fxf.pengpengdd.cyou

Go:   arr = append([]int{0}, arr...)
来源：http://cvz.tarul.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ekz.vqdsnc.cn

C#:   list.Insert(0, 0);
来源：http://nwg.yonumen.top

[D04] 删除元素
来源：http://rqd.sysykeji.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rmq.gogol.net.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://spw.daxiang520.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xox.aizwys.cn

TS:   arr.splice(0, 1);
来源：http://xuw.xuanzx.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fhi.yfazqb.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://msq.yanxiufei.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://viu.c1oappe.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uvq.uphjek.com

[D05] 访问与修改元素
来源：http://qca.nanxuanxn.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zqv.yonumen.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kvy.tian-w.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zci.aibaodan.cn

TS:   arr[0]; arr.at(-1);
来源：http://uoi.wangshuangyany.cn

Java: list.get(0); list.set(0, 9);
来源：http://azb.zhiwuduotai.top

Go:   arr[0]; arr[0] = 9
来源：http://sbg.jqgufenzy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://aml.guowangkeji.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ebs.quarkkingdee.top

[D06] 数组长度
来源：http://pec.haohaochexian.top

Py:   len(arr)
来源：http://qyz.sjlbkw.cn

PHP:  count($arr);
来源：http://fjg.fengsongda.top

JS:   arr.length
来源：http://uxc.dashuyun.cn

TS:   arr.length
来源：http://cwj.feifeiyinyue.top

Java: list.size();
来源：http://pto.yj20258888.top

Go:   len(arr)
来源：http://ngt.zdqjudy.top

Ruby: arr.length; arr.size
来源：http://nin.yfazqb.com

C#:   list.Count;
来源：http://bhs.yanxiufei.cn

[D07] 切片 / 取子数组
来源：http://kjj.cqqwz.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://sfp.zhijiandao.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zlg.shanyushiyangtech.top

JS:   arr.slice(1, 4);
来源：http://tsq.zhoulong.xyz

TS:   arr.slice(1, 4);
来源：http://vot.tian-w.cn

Java: list.subList(1, 4);
来源：http://ujy.dianchejie.cn

Go:   arr[1:4]
来源：http://ogt.shanyushiyangkeji.top

Ruby: arr[1, 3]
来源：http://tak.shanyushiyangkeji.top

C#:   list.GetRange(1, 3);
来源：http://rgs.sxryk.cn

[D08] 合并两个数组
来源：http://elt.shuidangran.top

Py:   a + b;  a.extend(b)
来源：http://abi.jyoumei.cn

PHP:  array_merge($a, $b);
来源：http://zkc.cqqwz.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gir.cashguo.top

TS:   [...a, ...b];
来源：http://olz.cucudq.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fwm.sxryk.cn

Go:   append(a, b...)
来源：http://was.fengsongda.top

Ruby: a + b;  a.concat(b)
来源：http://gig.cheryme.top

C#:   a.Concat(b).ToList()
来源：http://xej.chenjidiqi.icu

[D09] 排序（升序）
来源：http://whj.zhongyouzk.top

Py:   sorted(arr);  arr.sort()
来源：http://nqr.chenlongwang.top

PHP:  sort($arr);
来源：http://ral.jinghuilouyu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jln.xingfuxueyuan.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://qsv.nanxinkj.top

Java: Collections.sort(list);  list.sort(null);
来源：http://qnu.tarul.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zaf.jianghu66.top

Ruby: arr.sort
来源：http://dfa.shangyingyoupin.top

C#:   list.Sort();
来源：http://jtr.kuanghao11.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ota.feifeiyinyue.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vqz.smart0.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zxt.ydjk.org.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://eri.pycfn.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://sef.fzhhl.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hzs.shanyushiyangkeji.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bsr.yuxming.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tmt.pengpengdd.cyou

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qqv.zhiwuduotai.top

[D11] 反转数组
来源：http://yip.zhaomingkeji.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://mqa.xylfe.cn

PHP:  array_reverse($arr);
来源：http://les.shzxlz.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wzu.tian-w.cn

TS:   [...arr].reverse();
来源：http://lpq.jiagoushi.top

Java: Collections.reverse(list);
来源：http://pdd.yuxming.cn

Go:   slices.Reverse(arr)
来源：http://lqg.haohaochexian.top

Ruby: arr.reverse
来源：http://pyj.snrcjt.cn

C#:   list.Reverse();
来源：http://ooo.chenjidiqi.icu

[D12] 查找元素下标
来源：http://ytb.daxiang520.top

Py:   arr.index(x);  x in arr
来源：http://fpb.haohaochexian.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mvn.gotoacloud.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hws.ydzc1.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mjz.chenjidiqi.icu

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ien.jinghuilouyu.cn

Go:   slices.Index(arr, x)
来源：http://xue.sxryk.cn

Ruby: arr.index(x)
来源：http://luu.jiagoushi.top

C#:   list.IndexOf(x);
来源：http://jhi.wangshuangyany.cn

[D13] 过滤（保留满足条件的）
来源：http://csd.vehdjk.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://chm.sxryk.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ntt.havefunace.top

JS:   arr.filter(x => x > 3)
来源：http://wos.nwbrower.top

TS:   arr.filter(x => x > 3)
来源：http://mgv.cqqwz.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zeq.ivvv.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bhj.yangfankeji.com

Ruby: arr.select { |x| x > 3 }
来源：http://xdo.sufxvd.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://aid.uphjek.com

[D14] 映射转换（每个元素变形）
来源：http://owd.sufxvd.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ajp.jinqigfzy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://oex.zdbjq.cn

JS:   arr.map(x => x * 2)
来源：http://huv.chenjidiqi.icu

TS:   arr.map(x => x * 2)
来源：http://aja.svipenyu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://pvt.cashguo.top

Go:   // 手写循环
来源：http://ljo.jianghu66.top

Ruby: arr.map { |x| x * 2 }
来源：http://tor.smart0.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://mpz.yangfankeji.com

[D15] 去重
来源：http://hzw.zhiwuduotai.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ctw.xingfuxueyuan.xyz

PHP:  array_unique($arr);
来源：http://emw.gaohongyu789.top

JS:   [...new Set(arr)]
来源：http://yoy.gaohongyu789.top

TS:   [...new Set(arr)]
来源：http://ogl.daria6918.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mnv.ywan-chungtsiang.top

Go:   // 用 map[T]struct{} 手写
来源：http://der.wangdashe.top

Ruby: arr.uniq
来源：http://fca.jyoumei.cn

C#:   list.Distinct().ToList()
来源：http://zyy.guowangkeji.top

[D16] 求和与平均值
来源：http://vkw.fehbvm.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nlr.yangfankeji.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://iay.yuanzhike.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hyq.guannengcc.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qjk.smart0.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mfp.zhaomingkeji.xyz

Go:   // 手写循环累加
来源：http://ygq.iojbl.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hfq.smart0.xyz

C#:   list.Sum();  list.Average()
来源：http://wwz.sxryk.cn

[D17] 最大值与最小值
来源：http://kvu.pycfn.com

Py:   max(arr);  min(arr)
来源：http://lfh.meibo888.top

PHP:  max($arr);  min($arr);
来源：http://gps.gogol.net.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rll.hongshengwenyu.top

TS:   Math.max(...arr);
来源：http://qfr.redwolf501.top

Java: Collections.max(list);  Collections.min(list);
来源：http://gyf.mhx1999.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://krl.9152youxi.cn

Ruby: arr.max;  arr.min
来源：http://ufr.yuanzhike.top

C#:   list.Max();  list.Min()
来源：http://ysg.shangyingyoupin.top

[D18] 扁平化嵌套数组
来源：http://pvd.mhx1999.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xfg.yongpay.top

PHP:  array_merge(...$nested);
来源：http://zzq.tarul.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lnc.yangfankeji.com

TS:   nested.flat();
来源：http://wub.yonumen.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hbh.andypj.xyz

Go:   // 手写双层循环
来源：http://den.xingfuxueyuan.xyz

Ruby: nested.flatten
来源：http://mgr.gogol.net.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://vsf.wangdashe.top

[D19] 按字段分组
来源：http://zyc.zhoulong.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vvl.mhx1999.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nkp.daria6918.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gaa.nanxinkj.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://llb.fktsv.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hon.shangyingyoupin.top

Go:   // 手写 map[string][]T
来源：http://duf.shanyushiyangkeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://tuq.hysaishi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qir.zycfv.cn

[D20] 统计每个元素出现次数
来源：http://dyg.ydzc1.top

Py:   Counter(arr)
来源：http://dzj.sjlbkw.cn

PHP:  array_count_values($arr);
来源：http://zzx.jqgfzy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://drn.yj20258.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rxm.yangfankeji.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nmq.tarul.cn

Go:   // 手写 map[T]int
来源：http://upq.yongpay.top

Ruby: arr.tally
来源：http://idv.shuidangran.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ybr.jinqigufen.top

[D21] 判断是否包含某元素
来源：http://mdq.bbcook.cn

Py:   x in arr
来源：http://ksn.nanxuanxn.top

PHP:  in_array($x, $arr, true);
来源：http://rdp.wangdashe.top

JS:   arr.includes(x)
来源：http://kxh.dianchejie.cn

TS:   arr.includes(x)
来源：http://xbw.vehdjk.com

Java: list.contains(x)
来源：http://wcm.jqgfzy.top

Go:   slices.Contains(arr, x)
来源：http://vcd.yj202588.top

Ruby: arr.include?(x)
来源：http://mwg.yonumen.top

C#:   list.Contains(x)
来源：http://vfe.havefunace.top

[D22] 复制数组（避免共享引用）
来源：http://yze.nanxinkj.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zdz.nwbrower.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nls.nanxinkj.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xjm.ivvv.top

TS:   [...arr];
来源：http://kcb.cucudq.cn

Java: new ArrayList<>(list);
来源：http://xya.jinyuanbaomall.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ccv.jyoumei.cn

Ruby: arr.dup;  arr.clone
来源：http://yyj.nanxuanxn.top

C#:   new List<int>(list);
来源：http://btx.shanyushiyangkeji.top

[D23] reduce 累积计算
来源：http://noe.havefunace.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bab.zhoulong.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zxy.jinqigufen.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pju.shuidangran.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gkt.zhoulong.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://ucw.xinyue.icu

Go:   // 手写循环
来源：http://nok.aibaodan.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://neq.aibaodan.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zgj.0kj1m.cn

[D24] 字典 / Map 基本操作
来源：http://ekd.sufxvd.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mfy.ehwqpu.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://uwp.aibaodan.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://owt.zdbjq.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rae.quarkkingdee.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://igi.iojbl.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://epk.yueranfly.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jhr.gzhubu.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fnk.sxryk.cn

[D25] Set 集合去重与交并差
来源：http://hlq.c1oappe.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zfd.chenzaomai.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lbo.sufxvd.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vnj.aizwys.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://emq.chenzaomai.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ziv.yvedp.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xva.yonumen.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ian.jianghu66.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pcg.hongshengwenyu.top

[D26] 数组转字符串
来源：http://mab.chenzaomai.com

Py:   ", ".join(map(str, arr))
来源：http://drc.hysaishi.cn

PHP:  implode(", ", $arr);
来源：http://acf.ydzc1.top

JS:   arr.join(", ")
来源：http://ygf.xuetiantiany.cn

TS:   arr.join(", ")
来源：http://lbr.shangyingyoupin.top

Java: String.join(", ", list)
来源：http://ioo.tian-w.cn

Go:   strings.Join(strs, ", ")
来源：http://nxb.shangyingyoupin.top

Ruby: arr.join(", ")
来源：http://eng.tarul.cn

C#:   string.Join(", ", list)
来源：http://wjg.nanxuanxn.top

================================================================================
来源：http://ctb.iojbl.cn

E. 字符串处理
来源：http://dpe.feifeiyinyue.top

================================================================================
来源：http://eiq.cucudq.cn

[E01] 拼接字符串
来源：http://psy.kuanghao11.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qlu.ppjwa.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ofz.guannengcc.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kze.nanxuanxn.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hfd.feifeiyinyue.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hoe.jyoumei.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qeg.yvedp.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zyc.yvedp.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ldk.zycfv.cn

[E02] 重复字符串
来源：http://jsy.316326.xyz

Py:   "ab" * 3
来源：http://gjy.jlsjyb.cn

PHP:  str_repeat("ab", 3);
来源：http://lbj.tianlin.xyz

JS:   "ab".repeat(3)
来源：http://sqr.uphjek.com

TS:   "ab".repeat(3)
来源：http://ikz.jinqigfzy.top

Java: "ab".repeat(3)
来源：http://kfp.316326.xyz

Go:   strings.Repeat("ab", 3)
来源：http://thq.svipenyu.cn

Ruby: "ab" * 3
来源：http://kaj.tarul.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dem.epnwcf.com

[E03] 截取子串
来源：http://cdm.daxiang520.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://eva.ppjwa.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xew.jlsjyb.cn


<!-- 参考信息 -->