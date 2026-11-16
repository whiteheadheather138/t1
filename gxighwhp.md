代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://zva.fanxiaobao.xyz

JS:   (() => { console.log("run"); })();
来源：http://zts.epnwcf.com

TS:   (() => { console.log("run"); })();
来源：http://iju.jyoumei.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baf.meibo888.top

Go:   func() { fmt.Println("run") }()
来源：http://fxf.yj20258888.top

Ruby: -> { puts "run" }.call
来源：http://stc.yangfankeji.com

C#:   // 无 IIFE：用静态构造函数
来源：http://zqs.shzxlz.cn

[C13] 类型声明 / 类型注解
来源：http://ika.xuanzx.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wfw.guowangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://itq.ehwqpu.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mhr.hammf.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lyi.tanke756.top

Java: int add(int a, int b) { return a + b; }
来源：http://bmv.0kj1m.cn

Go:   func add(a, b int) int
来源：http://znp.tian-w.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rzq.cashguo.top

C#:   int Add(int a, int b) => a + b;
来源：http://yqg.svipenyu.cn

[C14] 泛型函数
来源：http://hbi.yueranfly.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fns.haohaochexian.top

PHP:  // 无泛型
来源：http://iqj.yj20258.top

JS:   // 无泛型
来源：http://ohl.aizwys.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wrt.birdmap.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://akp.shuidangran.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cum.zdqjudy.top

Ruby: # 无泛型
来源：http://aag.yonumen.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mom.zhaomingkeji.xyz

[C15] 解构 / 展开参数
来源：http://ckz.cheryme.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://okb.xuanzx.com

PHP:  [$a, $b] = $pair;
来源：http://vba.jinyuanbaomall.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xyp.meibo888.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wps.andypj.xyz

Java: // 无解构
来源：http://jbz.xuetiantiany.cn

Go:   // 无解构
来源：http://foa.hysaishi.cn

Ruby: a, b = pair
来源：http://ztu.bbcook.cn

C#:   var (a, b) = pair;
来源：http://thr.xuanzx.com

[C16] 函数 / 方法重载
来源：http://jjf.bbcook.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dgg.9152youxi.cn

PHP:  // 无重载
来源：http://qfr.hfpthk.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://uwc.zhengqikj.top

TS:   // 用联合类型或重载签名声明
来源：http://dtg.guowangkeji.top

Java: void f(int a) {}  void f(String a) {}
来源：http://twj.birdmap.top

Go:   // 无重载：用不同函数名
来源：http://drh.xylfe.cn

Ruby: # 无重载：靠动态参数
来源：http://nav.yj202588.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://gtf.cdnleiting.top

================================================================================
来源：http://oyv.zhengqikj.top

D. 数组 / 列表 / 集合
来源：http://fhu.sweek.top

================================================================================
来源：http://jki.daxiang520.top

[D01] 创建数组 / 列表
来源：http://pqt.ivvv.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://yvf.yj202588.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ryz.chenjidiqi.icu

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://elw.vqdsnc.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xbv.cdnleiting.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yzn.ydjk.org.cn

Go:   arr := []int{1, 2, 3}
来源：http://vku.yonumen.top

Ruby: arr = [1, 2, 3]
来源：http://jax.gotoacloud.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tgh.hongshengwenyu.top

[D02] 追加元素到末尾
来源：http://ydg.pycfn.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qzv.haohaochexian.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ytn.yueranfly.top

JS:   arr.push(4);
来源：http://grh.cdnleiting.top

TS:   arr.push(4);
来源：http://etn.dianchejie.cn

Java: list.add(4);
来源：http://gpf.yj20258.top

Go:   arr = append(arr, 4)
来源：http://fvm.zhongyouzk.top

Ruby: arr << 4; arr.push(5)
来源：http://kts.nanxuanxn.top

C#:   list.Add(4);
来源：http://adk.shanyushiyangtech.top

[D03] 在指定位置插入元素
来源：http://yko.hesvh.cn

Py:   arr.insert(0, 0)
来源：http://bhc.tianlin.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://izj.nwbrower.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mrs.jinghuilouyu.cn

TS:   arr.splice(0, 0, 0);
来源：http://rsk.ppjwa.cn

Java: list.add(0, 0);
来源：http://yjp.jinyuanbaomall.cn

Go:   arr = append([]int{0}, arr...)
来源：http://lxp.guannengcc.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pdo.zhengqikj.top

C#:   list.Insert(0, 0);
来源：http://kov.guannengcc.top

[D04] 删除元素
来源：http://qby.daxiang520.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tzg.jinghuilouyu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nky.aibaodan.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gsr.nanxuanxn.top

TS:   arr.splice(0, 1);
来源：http://fsr.yanxiufei.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://abt.epnwcf.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uqu.fehbvm.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://esx.hnqzz.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nme.cashguo.top

[D05] 访问与修改元素
来源：http://pes.guowangkeji.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://erm.gaohongyu789.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xlu.andypj.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wul.ywan-chungtsiang.top

TS:   arr[0]; arr.at(-1);
来源：http://iit.smart0.xyz

Java: list.get(0); list.set(0, 9);
来源：http://dlj.c1oappe.top

Go:   arr[0]; arr[0] = 9
来源：http://oea.iojbl.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rah.tarul.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://aga.epnwcf.com

[D06] 数组长度
来源：http://vuq.xingfuxueyuan.xyz

Py:   len(arr)
来源：http://ijr.tian-w.cn

PHP:  count($arr);
来源：http://zon.hnxiangtu.top

JS:   arr.length
来源：http://hez.hysaishi.cn

TS:   arr.length
来源：http://rdy.quarkkingdee.top

Java: list.size();
来源：http://cqg.dianchejie.cn

Go:   len(arr)
来源：http://rdm.gzhubu.top

Ruby: arr.length; arr.size
来源：http://vcb.ydzc1.top

C#:   list.Count;
来源：http://xaa.snrcjt.cn

[D07] 切片 / 取子数组
来源：http://mov.wangdashe.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lhn.hysaishi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wce.ydjk.org.cn

JS:   arr.slice(1, 4);
来源：http://omy.zhoulong.xyz

TS:   arr.slice(1, 4);
来源：http://ryo.jinghuilouyu.cn

Java: list.subList(1, 4);
来源：http://vzo.fengsongda.top

Go:   arr[1:4]
来源：http://boc.ehwqpu.com

Ruby: arr[1, 3]
来源：http://yqt.bjfxy.top

C#:   list.GetRange(1, 3);
来源：http://vsd.sufxvd.cn

[D08] 合并两个数组
来源：http://zdy.hammf.cn

Py:   a + b;  a.extend(b)
来源：http://whv.tian-w.cn

PHP:  array_merge($a, $b);
来源：http://wai.jiagoushi.top

JS:   [...a, ...b];  a.concat(b);
来源：http://nck.shangyingyoupin.top

TS:   [...a, ...b];
来源：http://qbo.xinyue.icu

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vja.zycfv.cn

Go:   append(a, b...)
来源：http://vcj.zhijiandao.cn

Ruby: a + b;  a.concat(b)
来源：http://qqc.guannengcc.top

C#:   a.Concat(b).ToList()
来源：http://gyt.chenlongwang.top

[D09] 排序（升序）
来源：http://rix.sysykeji.top

Py:   sorted(arr);  arr.sort()
来源：http://slo.daria6918.cn

PHP:  sort($arr);
来源：http://mkb.shuidangran.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kdt.xinyue.icu

TS:   [...arr].sort((x, y) => x - y);
来源：http://yla.yj20258888.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ruh.fktsv.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://eak.yanxiufei.cn

Ruby: arr.sort
来源：http://ymg.zdbjq.cn

C#:   list.Sort();
来源：http://jfd.52xcode.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://htd.uphjek.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://quy.zhijiandao.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uij.jianghu66.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cki.haohaochexian.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://utm.sjlbkw.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nuq.ybcxt.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://aht.chenzaomai.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cfj.jinqigufen.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ims.fktsv.cn

[D11] 反转数组
来源：http://rkt.aibaodan.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xfu.zhixingplan.top

PHP:  array_reverse($arr);
来源：http://jri.chenlongwang.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://onk.hcnkem.com

TS:   [...arr].reverse();
来源：http://ejv.zhiwuduotai.top

Java: Collections.reverse(list);
来源：http://uov.bbcook.cn

Go:   slices.Reverse(arr)
来源：http://myc.fanxiaobao.xyz

Ruby: arr.reverse
来源：http://ifg.vqdsnc.cn

C#:   list.Reverse();
来源：http://apw.mhx1999.top

[D12] 查找元素下标
来源：http://vhq.kuanghao11.cn

Py:   arr.index(x);  x in arr
来源：http://ikb.gotoacloud.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ydt.yangfankeji.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://luo.ehwqpu.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lgy.shanyushiyangkeji.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jyb.hysaishi.cn

Go:   slices.Index(arr, x)
来源：http://okm.vehdjk.com

Ruby: arr.index(x)
来源：http://acz.vqdsnc.cn

C#:   list.IndexOf(x);
来源：http://uyx.wangshuangyany.cn

[D13] 过滤（保留满足条件的）
来源：http://rcw.kuanghao11.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vvy.nanxuanxn.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wvz.ydjk.org.cn

JS:   arr.filter(x => x > 3)
来源：http://vpe.dianchejie.cn

TS:   arr.filter(x => x > 3)
来源：http://xks.yuanzhike.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qxm.hcnkem.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pfh.sufxvd.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ian.svipenyu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fkl.bjfxy.top

[D14] 映射转换（每个元素变形）
来源：http://umf.yangfankeji.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zec.zdqjudy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zhm.zhiwuduotai.top

JS:   arr.map(x => x * 2)
来源：http://eoj.cdnleiting.top

TS:   arr.map(x => x * 2)
来源：http://wgj.dashuyun.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://wkl.fanxiaobao.xyz

Go:   // 手写循环
来源：http://zis.bjfxy.top

Ruby: arr.map { |x| x * 2 }
来源：http://jhz.gzhubu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://kpm.c1oappe.top

[D15] 去重
来源：http://jon.bjfxy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ngl.zhongyouzk.top

PHP:  array_unique($arr);
来源：http://rrj.feifeiyinyue.top

JS:   [...new Set(arr)]
来源：http://tls.gaohongyu789.top

TS:   [...new Set(arr)]
来源：http://mck.yj202588.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://var.sxryk.cn

Go:   // 用 map[T]struct{} 手写
来源：http://obj.zhixingplan.top

Ruby: arr.uniq
来源：http://hqg.yvedp.cn

C#:   list.Distinct().ToList()
来源：http://htj.yongpay.top

[D16] 求和与平均值
来源：http://jyo.wangshuangyany.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://geq.hnqzz.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xao.fanxiaobao.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xjp.nanxinkj.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xwg.hammf.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sva.xziqi.cn

Go:   // 手写循环累加
来源：http://ylv.nanxinkj.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bux.xylfe.cn

C#:   list.Sum();  list.Average()
来源：http://piw.bbcook.cn

[D17] 最大值与最小值
来源：http://gcg.mhx1999.top

Py:   max(arr);  min(arr)
来源：http://byj.bjfxy.top

PHP:  max($arr);  min($arr);
来源：http://hxm.yj20258.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yfr.shanyushiyangtech.top

TS:   Math.max(...arr);
来源：http://gsy.0kj1m.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jen.wangshuangyany.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://uny.tianlin.xyz

Ruby: arr.max;  arr.min
来源：http://rwu.9152youxi.cn

C#:   list.Max();  list.Min()
来源：http://hpd.hesvh.cn

[D18] 扁平化嵌套数组
来源：http://eqj.hysaishi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://uvw.cashguo.top

PHP:  array_merge(...$nested);
来源：http://pxy.cucudq.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nmx.pengpengdd.cyou

TS:   nested.flat();
来源：http://ffl.bjfxy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zzi.ywan-chungtsiang.top

Go:   // 手写双层循环
来源：http://ukt.mhx1999.top

Ruby: nested.flatten
来源：http://nut.chenjidiqi.icu

C#:   nested.SelectMany(x => x).ToList()
来源：http://pzl.sweek.top

[D19] 按字段分组
来源：http://wxa.xinyue.icu

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xus.hammf.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://csu.gzhubu.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zvo.yongpay.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ije.hesvh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wwf.cucudq.cn

Go:   // 手写 map[string][]T
来源：http://toc.shanyushiyangtech.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://jam.shzxlz.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gqk.zhongyouzk.top

[D20] 统计每个元素出现次数
来源：http://khz.iojbl.cn

Py:   Counter(arr)
来源：http://css.jiagoushi.top

PHP:  array_count_values($arr);
来源：http://usc.zycfv.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qke.hnxiangtu.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wtm.yonumen.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rue.shuidangran.top

Go:   // 手写 map[T]int
来源：http://voi.epnwcf.com

Ruby: arr.tally
来源：http://wkt.wangdashe.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://maq.cheryme.top

[D21] 判断是否包含某元素
来源：http://swi.gotoacloud.top

Py:   x in arr
来源：http://bfv.ctjpmb.com

PHP:  in_array($x, $arr, true);
来源：http://fen.cdnleiting.top

JS:   arr.includes(x)
来源：http://mft.daxiang520.top

TS:   arr.includes(x)
来源：http://kfc.bjfxy.top

Java: list.contains(x)
来源：http://pre.fengsongda.top

Go:   slices.Contains(arr, x)
来源：http://ytt.nwbrower.top

Ruby: arr.include?(x)
来源：http://iet.pengpengdd.cyou

C#:   list.Contains(x)
来源：http://vuy.chenjidiqi.icu

[D22] 复制数组（避免共享引用）
来源：http://qyv.epnwcf.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hid.yj20258888.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://uuu.shangyingyoupin.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://szc.zdqjudy.top

TS:   [...arr];
来源：http://lgv.zhongyouzk.top

Java: new ArrayList<>(list);
来源：http://xkb.feifeiyinyue.top

Go:   copied := append([]int(nil), arr...)
来源：http://njc.shanyushiyangkeji.top

Ruby: arr.dup;  arr.clone
来源：http://qmk.guowangkeji.top

C#:   new List<int>(list);
来源：http://dxh.fktsv.cn

[D23] reduce 累积计算
来源：http://oft.jinyuanbaomall.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ujs.zhengqikj.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bqj.yvedp.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ovq.tanke756.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yld.birdmap.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://glj.gogol.net.cn

Go:   // 手写循环
来源：http://hnl.zhixingplan.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://abo.hnqzz.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hez.bjfxy.top

[D24] 字典 / Map 基本操作
来源：http://xae.zhengqikj.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xed.fzhhl.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sfx.tarul.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cfi.andypj.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tjp.ehwqpu.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kcg.jyoumei.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cma.tanke756.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mtb.zhengqikj.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zen.yangfankeji.com

[D25] Set 集合去重与交并差
来源：http://lwu.birdmap.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ybw.yongpay.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xsq.bbcook.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://stb.fktsv.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qxp.yfazqb.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nuw.iojbl.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bty.hnxiangtu.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://clo.sxryk.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://eru.svipenyu.cn

[D26] 数组转字符串
来源：http://xgz.quarkkingdee.top

Py:   ", ".join(map(str, arr))
来源：http://hoz.sxryk.cn

PHP:  implode(", ", $arr);
来源：http://wbd.fengsongda.top

JS:   arr.join(", ")
来源：http://gxf.sxryk.cn

TS:   arr.join(", ")
来源：http://pns.gogol.net.cn

Java: String.join(", ", list)
来源：http://ilm.aizwys.cn

Go:   strings.Join(strs, ", ")
来源：http://mbx.tanke756.top

Ruby: arr.join(", ")
来源：http://wen.pycfn.com

C#:   string.Join(", ", list)
来源：http://jfx.guowangkeji.top

================================================================================
来源：http://sfz.yj20258.top

E. 字符串处理
来源：http://zre.nanxinkj.top

================================================================================
来源：http://ccf.cheryme.top

[E01] 拼接字符串
来源：http://gjj.iojbl.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://plb.zhongyouzk.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ztc.xziqi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pvd.jqgufenzy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ifb.nanxinkj.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nwr.sufxvd.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ssc.tanke756.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jws.andypj.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://trr.nanxuanxn.top

[E02] 重复字符串
来源：http://zfa.yongpay.top

Py:   "ab" * 3
来源：http://idu.yongpay.top

PHP:  str_repeat("ab", 3);
来源：http://zdq.yfazqb.com

JS:   "ab".repeat(3)
来源：http://iih.pycfn.com

TS:   "ab".repeat(3)
来源：http://oxd.guannengcc.top

Java: "ab".repeat(3)
来源：http://xmd.jqgufenzy.top

Go:   strings.Repeat("ab", 3)
来源：http://pvp.svipenyu.cn

Ruby: "ab" * 3
来源：http://ghb.fengsongda.top


<!-- 参考信息 -->