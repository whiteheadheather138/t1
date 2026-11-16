代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://syc.yj202588.top

JS:   (() => { console.log("run"); })();
来源：http://wqi.jiagoushi.top

TS:   (() => { console.log("run"); })();
来源：http://vxj.jyoumei.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dgs.cheryme.top

Go:   func() { fmt.Println("run") }()
来源：http://dgv.316326.xyz

Ruby: -> { puts "run" }.call
来源：http://sgb.jianghu66.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ocv.tanke756.top

[C13] 类型声明 / 类型注解
来源：http://qei.yfazqb.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wib.shangyingyoupin.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rae.hywenlv.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nwj.jianghu66.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kds.nanxinkj.top

Java: int add(int a, int b) { return a + b; }
来源：http://bqv.gaohongyu789.top

Go:   func add(a, b int) int
来源：http://qov.jqgfzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jsd.quarkkingdee.top

C#:   int Add(int a, int b) => a + b;
来源：http://gwp.jinghuilouyu.cn

[C14] 泛型函数
来源：http://tsp.ywan-chungtsiang.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fbm.chenzaomai.com

PHP:  // 无泛型
来源：http://ded.ywan-chungtsiang.top

JS:   // 无泛型
来源：http://shb.316326.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dfz.cheryme.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ihm.smart0.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ifi.yj20258888.top

Ruby: # 无泛型
来源：http://ugb.yongpay.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vnm.ywan-chungtsiang.top

[C15] 解构 / 展开参数
来源：http://rln.iojbl.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://uzt.hysaishi.cn

PHP:  [$a, $b] = $pair;
来源：http://szc.chenjidiqi.icu

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://poq.zhaomingkeji.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tcp.nanxinkj.top

Java: // 无解构
来源：http://voy.yueranfly.top

Go:   // 无解构
来源：http://tik.ppjwa.cn

Ruby: a, b = pair
来源：http://rpe.sysykeji.top

C#:   var (a, b) = pair;
来源：http://sph.zhongyouzk.top

[C16] 函数 / 方法重载
来源：http://mao.sysykeji.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ddn.nanxuanxn.top

PHP:  // 无重载
来源：http://oms.xingfuxueyuan.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://qzy.aizwys.cn

TS:   // 用联合类型或重载签名声明
来源：http://aam.fengsongda.top

Java: void f(int a) {}  void f(String a) {}
来源：http://zvk.sweek.top

Go:   // 无重载：用不同函数名
来源：http://okv.birdmap.top

Ruby: # 无重载：靠动态参数
来源：http://jba.hysaishi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://dvy.hnqzz.top

================================================================================
来源：http://jof.vehdjk.com

D. 数组 / 列表 / 集合
来源：http://yhi.pycfn.com

================================================================================
来源：http://uln.shanyushiyangtech.top

[D01] 创建数组 / 列表
来源：http://soy.ywan-chungtsiang.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://wqq.zhoulong.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fbs.zhengqikj.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fhl.hysaishi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://sry.fanxiaobao.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ilm.jyoumei.cn

Go:   arr := []int{1, 2, 3}
来源：http://zjn.9152youxi.cn

Ruby: arr = [1, 2, 3]
来源：http://sgh.jinqigfzy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ani.ctjpmb.com

[D02] 追加元素到末尾
来源：http://jlj.jqgfzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://aey.zhiwuduotai.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://agk.jiagoushi.top

JS:   arr.push(4);
来源：http://xxn.sweek.top

TS:   arr.push(4);
来源：http://byb.yfazqb.com

Java: list.add(4);
来源：http://bem.daria6918.cn

Go:   arr = append(arr, 4)
来源：http://kvf.hnqzz.top

Ruby: arr << 4; arr.push(5)
来源：http://szt.hnxiangtu.top

C#:   list.Add(4);
来源：http://ifj.feifeiyinyue.top

[D03] 在指定位置插入元素
来源：http://lxs.xuanzx.com

Py:   arr.insert(0, 0)
来源：http://qsk.shuidangran.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://poh.cucudq.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wcd.jyoumei.cn

TS:   arr.splice(0, 0, 0);
来源：http://gff.hnqzz.top

Java: list.add(0, 0);
来源：http://ziw.gogol.net.cn

Go:   arr = append([]int{0}, arr...)
来源：http://tha.jinqigufen.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://waw.ivvv.top

C#:   list.Insert(0, 0);
来源：http://nsj.hysaishi.cn

[D04] 删除元素
来源：http://ngp.tanke756.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://llr.snrcjt.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cyc.yj20258.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zov.xylfe.cn

TS:   arr.splice(0, 1);
来源：http://uag.hesvh.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ljr.yuxming.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lss.zycfv.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wvj.tanke756.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://god.jinqigufen.top

[D05] 访问与修改元素
来源：http://zpi.yueranfly.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://llm.snrcjt.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xsg.jqgufenzy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qaz.birdmap.top

TS:   arr[0]; arr.at(-1);
来源：http://vnm.gotoacloud.top

Java: list.get(0); list.set(0, 9);
来源：http://lzk.pycfn.com

Go:   arr[0]; arr[0] = 9
来源：http://xsk.daria6918.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vfr.nanxinkj.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xlj.guannengcc.top

[D06] 数组长度
来源：http://yoc.yj202588.top

Py:   len(arr)
来源：http://wnw.zhijiandao.cn

PHP:  count($arr);
来源：http://xah.xingfuxueyuan.xyz

JS:   arr.length
来源：http://kae.tarul.cn

TS:   arr.length
来源：http://hcq.yanxiufei.cn

Java: list.size();
来源：http://zvj.snrcjt.cn

Go:   len(arr)
来源：http://edn.shuidangran.top

Ruby: arr.length; arr.size
来源：http://ltb.zhongyouzk.top

C#:   list.Count;
来源：http://jbw.hcnkem.com

[D07] 切片 / 取子数组
来源：http://nit.jinyuanbaomall.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://svj.sysykeji.top

PHP:  array_slice($arr, 1, 3);
来源：http://nqx.quarkkingdee.top

JS:   arr.slice(1, 4);
来源：http://rnw.zhiwuduotai.top

TS:   arr.slice(1, 4);
来源：http://jaz.gzhubu.top

Java: list.subList(1, 4);
来源：http://jxb.hnxiangtu.top

Go:   arr[1:4]
来源：http://wzd.jinqigfzy.top

Ruby: arr[1, 3]
来源：http://uvt.fengsongda.top

C#:   list.GetRange(1, 3);
来源：http://eou.hysaishi.cn

[D08] 合并两个数组
来源：http://vvm.hnqzz.top

Py:   a + b;  a.extend(b)
来源：http://nzg.jinyuanbaomall.cn

PHP:  array_merge($a, $b);
来源：http://qxc.hesvh.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://jyj.zhiwuduotai.top

TS:   [...a, ...b];
来源：http://kdl.iojbl.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://udg.sufxvd.cn

Go:   append(a, b...)
来源：http://rrj.hnxiangtu.top

Ruby: a + b;  a.concat(b)
来源：http://yck.epnwcf.com

C#:   a.Concat(b).ToList()
来源：http://xqs.wangdashe.top

[D09] 排序（升序）
来源：http://jxo.yj20258.top

Py:   sorted(arr);  arr.sort()
来源：http://kpx.svipenyu.cn

PHP:  sort($arr);
来源：http://pxp.shuidangran.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dum.wangdashe.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://rqh.yanxiufei.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://sth.guowangkeji.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kcw.yj20258.top

Ruby: arr.sort
来源：http://axh.zdbjq.cn

C#:   list.Sort();
来源：http://olt.ybcxt.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://iqj.yj20258.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mrs.gotoacloud.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lkw.bbcook.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wlw.ybcxt.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xsj.shanyushiyangtech.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://htb.daria6918.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pkd.cdnleiting.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://llu.pengpengdd.cyou

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rzh.hcnkem.com

[D11] 反转数组
来源：http://oev.dashuyun.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ewi.jinyuanbaomall.cn

PHP:  array_reverse($arr);
来源：http://zxl.cashguo.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kmu.ydjk.org.cn

TS:   [...arr].reverse();
来源：http://ffh.cashguo.top

Java: Collections.reverse(list);
来源：http://wrk.hnqzz.top

Go:   slices.Reverse(arr)
来源：http://uux.jqgfzy.top

Ruby: arr.reverse
来源：http://vex.redwolf501.top

C#:   list.Reverse();
来源：http://gog.sufxvd.cn

[D12] 查找元素下标
来源：http://blf.shzxlz.cn

Py:   arr.index(x);  x in arr
来源：http://usc.9152youxi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mzk.chenjidiqi.icu

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bwe.hywenlv.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eyh.fehbvm.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ciq.tianlin.xyz

Go:   slices.Index(arr, x)
来源：http://jzw.9152youxi.cn

Ruby: arr.index(x)
来源：http://yzq.jinyuanbaomall.cn

C#:   list.IndexOf(x);
来源：http://tkd.sufxvd.cn

[D13] 过滤（保留满足条件的）
来源：http://bka.meibo888.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nmj.ctjpmb.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lnp.316326.xyz

JS:   arr.filter(x => x > 3)
来源：http://ucn.zhiwuduotai.top

TS:   arr.filter(x => x > 3)
来源：http://oxg.jianghu66.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://juh.hammf.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vbf.tianlin.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://dvh.yongpay.top

C#:   list.Where(x => x > 3).ToList()
来源：http://gle.zhoulong.xyz

[D14] 映射转换（每个元素变形）
来源：http://aji.andypj.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zib.cdnleiting.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fpp.andypj.xyz

JS:   arr.map(x => x * 2)
来源：http://rcq.pengpengdd.cyou

TS:   arr.map(x => x * 2)
来源：http://jkx.fengsongda.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://fbg.daxiang520.top

Go:   // 手写循环
来源：http://cga.fzhhl.top

Ruby: arr.map { |x| x * 2 }
来源：http://kqg.xylfe.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ejp.vehdjk.com

[D15] 去重
来源：http://vzz.shanyushiyangtech.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nvk.fengsongda.top

PHP:  array_unique($arr);
来源：http://yid.jqgufenzy.top

JS:   [...new Set(arr)]
来源：http://flf.zhengqikj.top

TS:   [...new Set(arr)]
来源：http://wtn.shanyushiyangtech.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lqp.chenlongwang.top

Go:   // 用 map[T]struct{} 手写
来源：http://hix.gogol.net.cn

Ruby: arr.uniq
来源：http://wdd.tian-w.cn

C#:   list.Distinct().ToList()
来源：http://tvy.fengsongda.top

[D16] 求和与平均值
来源：http://wja.xuetiantiany.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mcb.ybcxt.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://oay.zdqjudy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wmj.meibo888.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gbz.xuanzx.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://clb.hnxiangtu.top

Go:   // 手写循环累加
来源：http://svg.dianchejie.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jua.aizwys.cn

C#:   list.Sum();  list.Average()
来源：http://tvv.yvedp.cn

[D17] 最大值与最小值
来源：http://hrg.shuidangran.top

Py:   max(arr);  min(arr)
来源：http://qki.aizwys.cn

PHP:  max($arr);  min($arr);
来源：http://uem.ppjwa.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pqr.jinqigfzy.top

TS:   Math.max(...arr);
来源：http://oqv.smart0.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://blk.haohaochexian.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jei.zdbjq.cn

Ruby: arr.max;  arr.min
来源：http://edf.hammf.cn

C#:   list.Max();  list.Min()
来源：http://oyw.cqqwz.cn

[D18] 扁平化嵌套数组
来源：http://rhp.hcnkem.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ogq.hfpthk.cn

PHP:  array_merge(...$nested);
来源：http://vzz.haohaochexian.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://epr.yj20258.top

TS:   nested.flat();
来源：http://yac.xziqi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gok.yvedp.cn

Go:   // 手写双层循环
来源：http://mks.epnwcf.com

Ruby: nested.flatten
来源：http://wpn.shzxlz.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://tqz.zhixingplan.top

[D19] 按字段分组
来源：http://yps.yvedp.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xoq.hysaishi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fpe.aibaodan.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ysd.cashguo.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://lwy.zhixingplan.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bdm.jqgufenzy.top

Go:   // 手写 map[string][]T
来源：http://iwd.chenzaomai.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://emv.zhoulong.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://eot.hfpthk.cn

[D20] 统计每个元素出现次数
来源：http://faq.sufxvd.cn

Py:   Counter(arr)
来源：http://mox.kuanghao11.cn

PHP:  array_count_values($arr);
来源：http://uip.ehwqpu.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://len.xingfuxueyuan.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jia.yangfankeji.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://faa.fktsv.cn

Go:   // 手写 map[T]int
来源：http://ugw.fengsongda.top

Ruby: arr.tally
来源：http://ide.xingfuxueyuan.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ctq.pycfn.com

[D21] 判断是否包含某元素
来源：http://mur.sufxvd.cn

Py:   x in arr
来源：http://vhu.meibo888.top

PHP:  in_array($x, $arr, true);
来源：http://qls.ctjpmb.com

JS:   arr.includes(x)
来源：http://nhi.jinghuilouyu.cn

TS:   arr.includes(x)
来源：http://rok.yj20258888.top

Java: list.contains(x)
来源：http://nha.yvedp.cn

Go:   slices.Contains(arr, x)
来源：http://qjs.jlsjyb.cn

Ruby: arr.include?(x)
来源：http://yyd.yfazqb.com

C#:   list.Contains(x)
来源：http://utt.zhiwuduotai.top

[D22] 复制数组（避免共享引用）
来源：http://zks.zhaomingkeji.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blr.snrcjt.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://joy.haohaochexian.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://plk.jqgufenzy.top

TS:   [...arr];
来源：http://vvl.snrcjt.cn

Java: new ArrayList<>(list);
来源：http://mjt.nanxuanxn.top

Go:   copied := append([]int(nil), arr...)
来源：http://qci.hywenlv.cn

Ruby: arr.dup;  arr.clone
来源：http://dig.ydjk.org.cn

C#:   new List<int>(list);
来源：http://ghy.jinqigfzy.top

[D23] reduce 累积计算
来源：http://ehq.sxryk.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xej.zhaomingkeji.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uhu.hammf.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rzn.tianlin.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nsi.vqdsnc.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://iny.ywan-chungtsiang.top

Go:   // 手写循环
来源：http://nze.fehbvm.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hpv.gzhubu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gws.xuanzx.com

[D24] 字典 / Map 基本操作
来源：http://ngf.yongpay.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ohr.daria6918.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ztn.xziqi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cqc.jqgfzy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tka.hfpthk.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cal.meibo888.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://foj.shanyushiyangkeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vdt.fzhhl.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fcm.hcnkem.com

[D25] Set 集合去重与交并差
来源：http://wlv.zhaomingkeji.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://azv.xziqi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tww.zhongyouzk.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gii.hesvh.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://btw.zhongyouzk.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://aeb.ydzc1.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gez.tarul.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ele.andypj.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://knw.hammf.cn

[D26] 数组转字符串
来源：http://yly.ctjpmb.com

Py:   ", ".join(map(str, arr))
来源：http://poc.jqgfzy.top

PHP:  implode(", ", $arr);
来源：http://fep.zhiwuduotai.top

JS:   arr.join(", ")
来源：http://jeu.52xcode.cn

TS:   arr.join(", ")
来源：http://inc.hammf.cn

Java: String.join(", ", list)
来源：http://mwp.ivvv.top

Go:   strings.Join(strs, ", ")
来源：http://qgu.ivvv.top

Ruby: arr.join(", ")
来源：http://hvd.zhoulong.xyz

C#:   string.Join(", ", list)
来源：http://eqy.sufxvd.cn

================================================================================
来源：http://lsh.xuanzx.com

E. 字符串处理
来源：http://fva.jqgfzy.top

================================================================================
来源：http://jvz.wangdashe.top

[E01] 拼接字符串
来源：http://cts.pengpengdd.cyou

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qhf.daria6918.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://uta.jianghu66.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mqg.daria6918.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tpn.zhongyouzk.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://knq.yj20258.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vzp.shuidangran.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cvi.yfazqb.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cob.svipenyu.cn

[E02] 重复字符串
来源：http://wxl.zdbjq.cn

Py:   "ab" * 3
来源：http://gqi.yonumen.top

PHP:  str_repeat("ab", 3);
来源：http://lzh.shangyingyoupin.top

JS:   "ab".repeat(3)
来源：http://kgd.snrcjt.cn

TS:   "ab".repeat(3)
来源：http://yve.birdmap.top

Java: "ab".repeat(3)
来源：http://bbs.xinyue.icu

Go:   strings.Repeat("ab", 3)
来源：http://uxr.hysaishi.cn

Ruby: "ab" * 3
来源：http://nja.sysykeji.top


<!-- 参考信息 -->