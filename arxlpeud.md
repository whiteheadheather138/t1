代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://hqu.ppjwa.cn

Ruby: -> { puts "run" }.call
来源：http://met.jinqigufen.top

C#:   // 无 IIFE：用静态构造函数
来源：http://kyp.yj20258.top

[C13] 类型声明 / 类型注解
来源：http://ool.aizwys.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bog.bbcook.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://glg.jqgfzy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bqt.sufxvd.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hpa.nanxuanxn.top

Java: int add(int a, int b) { return a + b; }
来源：http://ahz.tarul.cn

Go:   func add(a, b int) int
来源：http://pjw.meibo888.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fzs.jyoumei.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xdb.wangshuangyany.cn

[C14] 泛型函数
来源：http://hyp.jinqigfzy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://twp.cdnleiting.top

PHP:  // 无泛型
来源：http://vtj.havefunace.top

JS:   // 无泛型
来源：http://hao.xingfuxueyuan.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://klt.ehwqpu.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mwx.zdbjq.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://sdo.sufxvd.cn

Ruby: # 无泛型
来源：http://pgl.xuetiantiany.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ejh.cucudq.cn

[C15] 解构 / 展开参数
来源：http://fxe.havefunace.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yzb.jlsjyb.cn

PHP:  [$a, $b] = $pair;
来源：http://ivt.sxryk.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wuw.316326.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ijp.ydzc1.top

Java: // 无解构
来源：http://htp.hnxiangtu.top

Go:   // 无解构
来源：http://jzi.shanyushiyangkeji.top

Ruby: a, b = pair
来源：http://hhg.sysykeji.top

C#:   var (a, b) = pair;
来源：http://prk.ehwqpu.com

[C16] 函数 / 方法重载
来源：http://wwj.daria6918.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cms.yvedp.cn

PHP:  // 无重载
来源：http://saj.gaohongyu789.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ojj.gaohongyu789.top

TS:   // 用联合类型或重载签名声明
来源：http://wja.sufxvd.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://fjo.nanxinkj.top

Go:   // 无重载：用不同函数名
来源：http://jke.snrcjt.cn

Ruby: # 无重载：靠动态参数
来源：http://tvm.0kj1m.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://gvm.shanyushiyangtech.top

================================================================================
来源：http://gho.xziqi.cn

D. 数组 / 列表 / 集合
来源：http://nty.epnwcf.com

================================================================================
来源：http://fxw.sysykeji.top

[D01] 创建数组 / 列表
来源：http://bkv.cdnleiting.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://kdi.yj20258.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lpz.yfazqb.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gcl.vqdsnc.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://nwp.xziqi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xll.shangyingyoupin.top

Go:   arr := []int{1, 2, 3}
来源：http://qqo.pengpengdd.cyou

Ruby: arr = [1, 2, 3]
来源：http://yyr.yanxiufei.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://opt.tian-w.cn

[D02] 追加元素到末尾
来源：http://upr.yvedp.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://deh.zhijiandao.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wyb.jlsjyb.cn

JS:   arr.push(4);
来源：http://hdt.zhijiandao.cn

TS:   arr.push(4);
来源：http://cep.cheryme.top

Java: list.add(4);
来源：http://xsg.zhixingplan.top

Go:   arr = append(arr, 4)
来源：http://hnj.xylfe.cn

Ruby: arr << 4; arr.push(5)
来源：http://fir.fehbvm.com

C#:   list.Add(4);
来源：http://fpm.hongshengwenyu.top

[D03] 在指定位置插入元素
来源：http://jpf.cucudq.cn

Py:   arr.insert(0, 0)
来源：http://kfr.zdqjudy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://eta.zycfv.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hyd.yangfankeji.com

TS:   arr.splice(0, 0, 0);
来源：http://wtm.sweek.top

Java: list.add(0, 0);
来源：http://luv.sufxvd.cn

Go:   arr = append([]int{0}, arr...)
来源：http://mes.yvedp.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sdi.jinqigfzy.top

C#:   list.Insert(0, 0);
来源：http://lts.yfazqb.com

[D04] 删除元素
来源：http://urn.0kj1m.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://thu.gotoacloud.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://szm.zycfv.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://efb.pycfn.com

TS:   arr.splice(0, 1);
来源：http://sab.epnwcf.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://oiu.fanxiaobao.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rra.meibo888.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vru.andypj.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dji.zhiwuduotai.top

[D05] 访问与修改元素
来源：http://iud.shuidangran.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://oql.hongshengwenyu.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wjv.xuanzx.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kxj.sufxvd.cn

TS:   arr[0]; arr.at(-1);
来源：http://tmj.hywenlv.cn

Java: list.get(0); list.set(0, 9);
来源：http://ewy.yvedp.cn

Go:   arr[0]; arr[0] = 9
来源：http://jzo.yfazqb.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vla.0kj1m.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rrc.nanxinkj.top

[D06] 数组长度
来源：http://sht.yj20258.top

Py:   len(arr)
来源：http://skv.jlsjyb.cn

PHP:  count($arr);
来源：http://yzi.yj202588.top

JS:   arr.length
来源：http://xkt.hysaishi.cn

TS:   arr.length
来源：http://tvy.sysykeji.top

Java: list.size();
来源：http://qqc.tianlin.xyz

Go:   len(arr)
来源：http://fhb.zhixingplan.top

Ruby: arr.length; arr.size
来源：http://nku.yuxming.cn

C#:   list.Count;
来源：http://xdi.zhaomingkeji.xyz

[D07] 切片 / 取子数组
来源：http://ccl.chenjidiqi.icu

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://khr.fzhhl.top

PHP:  array_slice($arr, 1, 3);
来源：http://oji.fengsongda.top

JS:   arr.slice(1, 4);
来源：http://wwr.yfazqb.com

TS:   arr.slice(1, 4);
来源：http://ejh.jinqigufen.top

Java: list.subList(1, 4);
来源：http://rpj.nanxuanxn.top

Go:   arr[1:4]
来源：http://reu.gaohongyu789.top

Ruby: arr[1, 3]
来源：http://tnk.sysykeji.top

C#:   list.GetRange(1, 3);
来源：http://ovm.fehbvm.com

[D08] 合并两个数组
来源：http://qci.gzhubu.top

Py:   a + b;  a.extend(b)
来源：http://rcy.epnwcf.com

PHP:  array_merge($a, $b);
来源：http://uuv.sysykeji.top

JS:   [...a, ...b];  a.concat(b);
来源：http://rnm.bjfxy.top

TS:   [...a, ...b];
来源：http://pkr.feifeiyinyue.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kcr.zdbjq.cn

Go:   append(a, b...)
来源：http://lyt.fehbvm.com

Ruby: a + b;  a.concat(b)
来源：http://pvs.cdnleiting.top

C#:   a.Concat(b).ToList()
来源：http://jic.meibo888.top

[D09] 排序（升序）
来源：http://cmx.jianghu66.top

Py:   sorted(arr);  arr.sort()
来源：http://xjs.fktsv.cn

PHP:  sort($arr);
来源：http://jij.gzhubu.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dia.feifeiyinyue.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://kbl.jiagoushi.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ngj.daria6918.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yzd.ybcxt.top

Ruby: arr.sort
来源：http://ahq.feifeiyinyue.top

C#:   list.Sort();
来源：http://rdj.jianghu66.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://khc.cashguo.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://afx.shanyushiyangtech.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bfz.bbcook.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hxz.svipenyu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tku.zhiwuduotai.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tlz.shanyushiyangtech.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://iwi.zdqjudy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://egl.nanxinkj.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fsh.ydzc1.top

[D11] 反转数组
来源：http://inw.chenzaomai.com

Py:   arr[::-1];  arr.reverse()
来源：http://ndk.hcnkem.com

PHP:  array_reverse($arr);
来源：http://fpe.gogol.net.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://shn.jinqigfzy.top

TS:   [...arr].reverse();
来源：http://qnl.nanxuanxn.top

Java: Collections.reverse(list);
来源：http://gvl.snrcjt.cn

Go:   slices.Reverse(arr)
来源：http://yna.wangshuangyany.cn

Ruby: arr.reverse
来源：http://rwx.haohaochexian.top

C#:   list.Reverse();
来源：http://ppa.jinqigufen.top

[D12] 查找元素下标
来源：http://xrd.hnqzz.top

Py:   arr.index(x);  x in arr
来源：http://mjh.yj20258.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tnu.c1oappe.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zpo.vehdjk.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hwf.ywan-chungtsiang.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mek.havefunace.top

Go:   slices.Index(arr, x)
来源：http://wjh.yj20258888.top

Ruby: arr.index(x)
来源：http://myj.316326.xyz

C#:   list.IndexOf(x);
来源：http://azh.jqgfzy.top

[D13] 过滤（保留满足条件的）
来源：http://rex.fktsv.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pmo.cashguo.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ymp.vehdjk.com

JS:   arr.filter(x => x > 3)
来源：http://wcz.guowangkeji.top

TS:   arr.filter(x => x > 3)
来源：http://wnf.nanxinkj.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://uci.zhoulong.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ock.ywan-chungtsiang.top

Ruby: arr.select { |x| x > 3 }
来源：http://brs.xuetiantiany.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ycm.ivvv.top

[D14] 映射转换（每个元素变形）
来源：http://pgs.guannengcc.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lqq.kuanghao11.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rjp.hesvh.cn

JS:   arr.map(x => x * 2)
来源：http://ffe.uphjek.com

TS:   arr.map(x => x * 2)
来源：http://ozj.fengsongda.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://pdd.chenjidiqi.icu

Go:   // 手写循环
来源：http://eap.uphjek.com

Ruby: arr.map { |x| x * 2 }
来源：http://pqe.zdqjudy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://abu.hongshengwenyu.top

[D15] 去重
来源：http://qog.guannengcc.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://has.cucudq.cn

PHP:  array_unique($arr);
来源：http://gmg.bbcook.cn

JS:   [...new Set(arr)]
来源：http://ryc.wangshuangyany.cn

TS:   [...new Set(arr)]
来源：http://ryz.yanxiufei.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xki.jinyuanbaomall.cn

Go:   // 用 map[T]struct{} 手写
来源：http://rfa.shanyushiyangkeji.top

Ruby: arr.uniq
来源：http://lpx.gzhubu.top

C#:   list.Distinct().ToList()
来源：http://zpo.bjfxy.top

[D16] 求和与平均值
来源：http://koi.zhiwuduotai.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fjq.snrcjt.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://chv.sjlbkw.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rxs.dashuyun.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qxo.chenzaomai.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tgg.sysykeji.top

Go:   // 手写循环累加
来源：http://kko.gogol.net.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://opb.jianghu66.top

C#:   list.Sum();  list.Average()
来源：http://ert.guowangkeji.top

[D17] 最大值与最小值
来源：http://ufc.aibaodan.cn

Py:   max(arr);  min(arr)
来源：http://cut.0kj1m.cn

PHP:  max($arr);  min($arr);
来源：http://stg.smart0.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://eop.c1oappe.top

TS:   Math.max(...arr);
来源：http://pge.yj20258.top

Java: Collections.max(list);  Collections.min(list);
来源：http://uep.cqqwz.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fzj.fehbvm.com

Ruby: arr.max;  arr.min
来源：http://ggj.yangfankeji.com

C#:   list.Max();  list.Min()
来源：http://ztd.sxryk.cn

[D18] 扁平化嵌套数组
来源：http://plc.wangdashe.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ykb.ydzc1.top

PHP:  array_merge(...$nested);
来源：http://mqh.cheryme.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hqw.xinyue.icu

TS:   nested.flat();
来源：http://ivq.sjlbkw.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rxd.mhx1999.top

Go:   // 手写双层循环
来源：http://cfk.ctjpmb.com

Ruby: nested.flatten
来源：http://nec.yj20258888.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://vnl.yfazqb.com

[D19] 按字段分组
来源：http://sxa.jianghu66.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dxt.svipenyu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://els.chenlongwang.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mhf.9152youxi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jjs.ppjwa.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wjq.aizwys.cn

Go:   // 手写 map[string][]T
来源：http://osf.jyoumei.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://lpg.nwbrower.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hqt.hesvh.cn

[D20] 统计每个元素出现次数
来源：http://qdw.c1oappe.top

Py:   Counter(arr)
来源：http://hsf.shzxlz.cn

PHP:  array_count_values($arr);
来源：http://kuv.nanxuanxn.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kpm.zhiwuduotai.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pmn.tarul.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tvb.hammf.cn

Go:   // 手写 map[T]int
来源：http://qta.gotoacloud.top

Ruby: arr.tally
来源：http://vcg.sxryk.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lry.zhixingplan.top

[D21] 判断是否包含某元素
来源：http://rue.aibaodan.cn

Py:   x in arr
来源：http://xsf.meibo888.top

PHP:  in_array($x, $arr, true);
来源：http://mgc.sjlbkw.cn

JS:   arr.includes(x)
来源：http://wwo.zhiwuduotai.top

TS:   arr.includes(x)
来源：http://lmo.52xcode.cn

Java: list.contains(x)
来源：http://rie.sufxvd.cn

Go:   slices.Contains(arr, x)
来源：http://jdd.yangfankeji.com

Ruby: arr.include?(x)
来源：http://iwl.ehwqpu.com

C#:   list.Contains(x)
来源：http://mju.yueranfly.top

[D22] 复制数组（避免共享引用）
来源：http://nvp.ppjwa.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://efb.shanyushiyangkeji.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://msv.xuetiantiany.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bxm.yueranfly.top

TS:   [...arr];
来源：http://obw.hnqzz.top

Java: new ArrayList<>(list);
来源：http://rcf.fengsongda.top

Go:   copied := append([]int(nil), arr...)
来源：http://isy.guowangkeji.top

Ruby: arr.dup;  arr.clone
来源：http://klr.shanyushiyangtech.top

C#:   new List<int>(list);
来源：http://yno.9152youxi.cn

[D23] reduce 累积计算
来源：http://pfa.wangdashe.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://eof.ehwqpu.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xel.xuetiantiany.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xbl.hnxiangtu.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://shu.sweek.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://eka.smart0.xyz

Go:   // 手写循环
来源：http://dnw.haohaochexian.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kyp.yj202588.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rjl.guannengcc.top

[D24] 字典 / Map 基本操作
来源：http://ywc.yonumen.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://oed.chenjidiqi.icu

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mkx.svipenyu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ylg.ivvv.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ewn.gzhubu.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hns.yangfankeji.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cvc.snrcjt.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lfx.zhongyouzk.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tee.xylfe.cn

[D25] Set 集合去重与交并差
来源：http://kdg.andypj.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kid.hnxiangtu.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://uef.zhiwuduotai.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://uzm.daxiang520.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pjf.epnwcf.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ssd.meibo888.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wlc.9152youxi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ezv.fktsv.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zki.chenlongwang.top

[D26] 数组转字符串
来源：http://tjo.zycfv.cn

Py:   ", ".join(map(str, arr))
来源：http://crf.tanke756.top

PHP:  implode(", ", $arr);
来源：http://xiu.fanxiaobao.xyz

JS:   arr.join(", ")
来源：http://dal.tarul.cn

TS:   arr.join(", ")
来源：http://hrb.yfazqb.com

Java: String.join(", ", list)
来源：http://ndr.aizwys.cn

Go:   strings.Join(strs, ", ")
来源：http://ibx.vehdjk.com

Ruby: arr.join(", ")
来源：http://znk.jqgfzy.top

C#:   string.Join(", ", list)
来源：http://ajd.yangfankeji.com

================================================================================
来源：http://bda.zhoulong.xyz

E. 字符串处理
来源：http://uau.gogol.net.cn

================================================================================
来源：http://dmh.feifeiyinyue.top

[E01] 拼接字符串
来源：http://dwo.andypj.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ohg.ywan-chungtsiang.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ect.kuanghao11.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ycz.shuidangran.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gyw.shuidangran.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lze.gaohongyu789.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://axv.redwolf501.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fdu.nanxinkj.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yth.svipenyu.cn

[E02] 重复字符串
来源：http://gpg.ydjk.org.cn

Py:   "ab" * 3
来源：http://lql.sysykeji.top

PHP:  str_repeat("ab", 3);
来源：http://vjb.52xcode.cn

JS:   "ab".repeat(3)
来源：http://ybj.ybcxt.top

TS:   "ab".repeat(3)
来源：http://cnz.ydzc1.top

Java: "ab".repeat(3)
来源：http://awz.zhijiandao.cn

Go:   strings.Repeat("ab", 3)
来源：http://ajz.kuanghao11.cn

Ruby: "ab" * 3
来源：http://gfv.ydzc1.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://iyx.ehwqpu.com

[E03] 截取子串
来源：http://uxn.tanke756.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://upo.hcnkem.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vbf.daria6918.cn


<!-- 参考信息 -->