代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://yqh.hywenlv.cn

JS:   (() => { console.log("run"); })();
来源：http://rix.daria6918.cn

TS:   (() => { console.log("run"); })();
来源：http://rhk.zhongyouzk.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://law.ybcxt.top

Go:   func() { fmt.Println("run") }()
来源：http://yuy.bjfxy.top

Ruby: -> { puts "run" }.call
来源：http://otr.ydjk.org.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fhr.hcnkem.com

[C13] 类型声明 / 类型注解
来源：http://qki.cheryme.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zxn.zhiwuduotai.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wxw.zhengqikj.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zze.sxryk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jxv.epnwcf.com

Java: int add(int a, int b) { return a + b; }
来源：http://jdg.tian-w.cn

Go:   func add(a, b int) int
来源：http://guw.yuxming.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nlv.yongpay.top

C#:   int Add(int a, int b) => a + b;
来源：http://rno.ivvv.top

[C14] 泛型函数
来源：http://sfs.xziqi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://iec.ydzc1.top

PHP:  // 无泛型
来源：http://bju.fehbvm.com

JS:   // 无泛型
来源：http://yyv.pengpengdd.cyou

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://akt.zdbjq.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lfx.sufxvd.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rnz.bbcook.cn

Ruby: # 无泛型
来源：http://zju.bbcook.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gyu.yangfankeji.com

[C15] 解构 / 展开参数
来源：http://cwj.zhixingplan.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://znd.tanke756.top

PHP:  [$a, $b] = $pair;
来源：http://lzh.tanke756.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pzz.316326.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tzn.hammf.cn

Java: // 无解构
来源：http://ftl.tarul.cn

Go:   // 无解构
来源：http://xio.fktsv.cn

Ruby: a, b = pair
来源：http://hdf.wangshuangyany.cn

C#:   var (a, b) = pair;
来源：http://sxz.gogol.net.cn

[C16] 函数 / 方法重载
来源：http://ehm.hywenlv.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xjb.zhixingplan.top

PHP:  // 无重载
来源：http://kol.jinyuanbaomall.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xil.guowangkeji.top

TS:   // 用联合类型或重载签名声明
来源：http://ecw.0kj1m.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://uwm.chenjidiqi.icu

Go:   // 无重载：用不同函数名
来源：http://pca.cdnleiting.top

Ruby: # 无重载：靠动态参数
来源：http://gvr.9152youxi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ytz.cdnleiting.top

================================================================================
来源：http://yez.feifeiyinyue.top

D. 数组 / 列表 / 集合
来源：http://bvt.cucudq.cn

================================================================================
来源：http://juh.kuanghao11.cn

[D01] 创建数组 / 列表
来源：http://eoo.yuxming.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ybc.ehwqpu.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cpu.ywan-chungtsiang.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lqx.guannengcc.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://itu.hesvh.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yrk.tianlin.xyz

Go:   arr := []int{1, 2, 3}
来源：http://rnt.tarul.cn

Ruby: arr = [1, 2, 3]
来源：http://tfn.sysykeji.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tep.gaohongyu789.top

[D02] 追加元素到末尾
来源：http://ibn.guowangkeji.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lij.cdnleiting.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xxl.haohaochexian.top

JS:   arr.push(4);
来源：http://vfm.c1oappe.top

TS:   arr.push(4);
来源：http://ebo.fengsongda.top

Java: list.add(4);
来源：http://ptq.hongshengwenyu.top

Go:   arr = append(arr, 4)
来源：http://jma.gzhubu.top

Ruby: arr << 4; arr.push(5)
来源：http://pze.sufxvd.cn

C#:   list.Add(4);
来源：http://iao.tianlin.xyz

[D03] 在指定位置插入元素
来源：http://zgk.xylfe.cn

Py:   arr.insert(0, 0)
来源：http://kyd.tianlin.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yxl.shanyushiyangkeji.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qcx.bjfxy.top

TS:   arr.splice(0, 0, 0);
来源：http://tsy.ctjpmb.com

Java: list.add(0, 0);
来源：http://ipg.aibaodan.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vmy.snrcjt.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ewr.haohaochexian.top

C#:   list.Insert(0, 0);
来源：http://fdq.shanyushiyangkeji.top

[D04] 删除元素
来源：http://sji.zhongyouzk.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mhb.jianghu66.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lis.hesvh.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lmq.shangyingyoupin.top

TS:   arr.splice(0, 1);
来源：http://tus.gogol.net.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qeq.yuanzhike.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hej.snrcjt.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zbb.fanxiaobao.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xkm.chenjidiqi.icu

[D05] 访问与修改元素
来源：http://lkd.sufxvd.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ikk.zhixingplan.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ziu.gaohongyu789.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nuw.fehbvm.com

TS:   arr[0]; arr.at(-1);
来源：http://snk.52xcode.cn

Java: list.get(0); list.set(0, 9);
来源：http://mxl.tian-w.cn

Go:   arr[0]; arr[0] = 9
来源：http://jht.ehwqpu.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://urs.snrcjt.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rqg.bbcook.cn

[D06] 数组长度
来源：http://qwe.nwbrower.top

Py:   len(arr)
来源：http://qkb.meibo888.top

PHP:  count($arr);
来源：http://tvq.fzhhl.top

JS:   arr.length
来源：http://heb.hammf.cn

TS:   arr.length
来源：http://ghn.ctjpmb.com

Java: list.size();
来源：http://www.andypj.xyz

Go:   len(arr)
来源：http://rrz.yj20258888.top

Ruby: arr.length; arr.size
来源：http://hzq.uphjek.com

C#:   list.Count;
来源：http://dau.yuxming.cn

[D07] 切片 / 取子数组
来源：http://rkw.0kj1m.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rpi.zdqjudy.top

PHP:  array_slice($arr, 1, 3);
来源：http://vec.zhengqikj.top

JS:   arr.slice(1, 4);
来源：http://jom.pengpengdd.cyou

TS:   arr.slice(1, 4);
来源：http://ylz.aizwys.cn

Java: list.subList(1, 4);
来源：http://keu.gzhubu.top

Go:   arr[1:4]
来源：http://ftx.jqgfzy.top

Ruby: arr[1, 3]
来源：http://hxo.nanxinkj.top

C#:   list.GetRange(1, 3);
来源：http://hoj.yj20258.top

[D08] 合并两个数组
来源：http://wvv.jinyuanbaomall.cn

Py:   a + b;  a.extend(b)
来源：http://vcm.dianchejie.cn

PHP:  array_merge($a, $b);
来源：http://vie.quarkkingdee.top

JS:   [...a, ...b];  a.concat(b);
来源：http://vrx.ehwqpu.com

TS:   [...a, ...b];
来源：http://hgr.yvedp.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zvc.fanxiaobao.xyz

Go:   append(a, b...)
来源：http://wdi.hfpthk.cn

Ruby: a + b;  a.concat(b)
来源：http://tno.fehbvm.com

C#:   a.Concat(b).ToList()
来源：http://kbh.redwolf501.top

[D09] 排序（升序）
来源：http://ogv.gotoacloud.top

Py:   sorted(arr);  arr.sort()
来源：http://zbx.nanxuanxn.top

PHP:  sort($arr);
来源：http://ezz.zhengqikj.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ezf.sweek.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://inr.vqdsnc.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tao.ydzc1.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jkp.jyoumei.cn

Ruby: arr.sort
来源：http://bsr.tarul.cn

C#:   list.Sort();
来源：http://xxx.hammf.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://epl.jinghuilouyu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vsu.yueranfly.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wok.sxryk.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zoa.zhixingplan.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://usx.vqdsnc.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://thi.cqqwz.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cis.pycfn.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fst.meibo888.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nkn.tanke756.top

[D11] 反转数组
来源：http://mhx.tanke756.top

Py:   arr[::-1];  arr.reverse()
来源：http://fvt.zdqjudy.top

PHP:  array_reverse($arr);
来源：http://vmk.wangshuangyany.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://scy.hammf.cn

TS:   [...arr].reverse();
来源：http://jok.redwolf501.top

Java: Collections.reverse(list);
来源：http://bxw.iojbl.cn

Go:   slices.Reverse(arr)
来源：http://als.hnqzz.top

Ruby: arr.reverse
来源：http://gdp.gzhubu.top

C#:   list.Reverse();
来源：http://cmq.hywenlv.cn

[D12] 查找元素下标
来源：http://twl.cucudq.cn

Py:   arr.index(x);  x in arr
来源：http://yor.chenlongwang.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gyx.mhx1999.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mgx.mhx1999.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pts.aibaodan.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wgy.xingfuxueyuan.xyz

Go:   slices.Index(arr, x)
来源：http://hfp.havefunace.top

Ruby: arr.index(x)
来源：http://ikw.hcnkem.com

C#:   list.IndexOf(x);
来源：http://rwe.9152youxi.cn

[D13] 过滤（保留满足条件的）
来源：http://hwi.fehbvm.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ekk.nanxuanxn.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://aow.havefunace.top

JS:   arr.filter(x => x > 3)
来源：http://lkz.ywan-chungtsiang.top

TS:   arr.filter(x => x > 3)
来源：http://gvn.fktsv.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mcc.c1oappe.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dze.hammf.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vqw.gogol.net.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://kab.ppjwa.cn

[D14] 映射转换（每个元素变形）
来源：http://vjq.redwolf501.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tkq.tanke756.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wqy.52xcode.cn

JS:   arr.map(x => x * 2)
来源：http://eze.zdqjudy.top

TS:   arr.map(x => x * 2)
来源：http://kja.shuidangran.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://brw.sysykeji.top

Go:   // 手写循环
来源：http://jzt.xinyue.icu

Ruby: arr.map { |x| x * 2 }
来源：http://qfw.tian-w.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ywi.jinqigfzy.top

[D15] 去重
来源：http://hmz.nanxinkj.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://peo.aibaodan.cn

PHP:  array_unique($arr);
来源：http://uwv.xingfuxueyuan.xyz

JS:   [...new Set(arr)]
来源：http://hjw.ctjpmb.com

TS:   [...new Set(arr)]
来源：http://xdy.shangyingyoupin.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ilw.yj20258.top

Go:   // 用 map[T]struct{} 手写
来源：http://bql.bjfxy.top

Ruby: arr.uniq
来源：http://ipb.kuanghao11.cn

C#:   list.Distinct().ToList()
来源：http://ztg.xuetiantiany.cn

[D16] 求和与平均值
来源：http://coc.nanxinkj.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vzv.shanyushiyangkeji.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ulh.shzxlz.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://efa.pengpengdd.cyou

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hvs.zhixingplan.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ztb.ppjwa.cn

Go:   // 手写循环累加
来源：http://ruq.tanke756.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ocz.yfazqb.com

C#:   list.Sum();  list.Average()
来源：http://hpm.fanxiaobao.xyz

[D17] 最大值与最小值
来源：http://wns.jinqigufen.top

Py:   max(arr);  min(arr)
来源：http://apk.bbcook.cn

PHP:  max($arr);  min($arr);
来源：http://eth.shanyushiyangtech.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wyo.zhijiandao.cn

TS:   Math.max(...arr);
来源：http://yjp.xuetiantiany.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://wrn.cashguo.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://eao.zdbjq.cn

Ruby: arr.max;  arr.min
来源：http://fmf.cucudq.cn

C#:   list.Max();  list.Min()
来源：http://evr.sysykeji.top

[D18] 扁平化嵌套数组
来源：http://xuk.xingfuxueyuan.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://aeu.hywenlv.cn

PHP:  array_merge(...$nested);
来源：http://bgj.xziqi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ccm.jiagoushi.top

TS:   nested.flat();
来源：http://znv.hysaishi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jir.aibaodan.cn

Go:   // 手写双层循环
来源：http://jht.fzhhl.top

Ruby: nested.flatten
来源：http://ezg.zhaomingkeji.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://hhg.hammf.cn

[D19] 按字段分组
来源：http://eem.52xcode.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jws.zhijiandao.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pim.mhx1999.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cxa.jqgufenzy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://khc.sxryk.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nii.zhoulong.xyz

Go:   // 手写 map[string][]T
来源：http://hma.snrcjt.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fhw.nwbrower.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://unw.hcnkem.com

[D20] 统计每个元素出现次数
来源：http://khb.jqgufenzy.top

Py:   Counter(arr)
来源：http://igk.zdqjudy.top

PHP:  array_count_values($arr);
来源：http://ulv.zhoulong.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sry.xingfuxueyuan.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eyi.vqdsnc.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dok.guannengcc.top

Go:   // 手写 map[T]int
来源：http://rqi.andypj.xyz

Ruby: arr.tally
来源：http://qhe.quarkkingdee.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://opg.sweek.top

[D21] 判断是否包含某元素
来源：http://lkx.chenjidiqi.icu

Py:   x in arr
来源：http://qvb.cqqwz.cn

PHP:  in_array($x, $arr, true);
来源：http://kxl.daxiang520.top

JS:   arr.includes(x)
来源：http://qra.sweek.top

TS:   arr.includes(x)
来源：http://bvp.52xcode.cn

Java: list.contains(x)
来源：http://vhe.yj20258888.top

Go:   slices.Contains(arr, x)
来源：http://xiq.uphjek.com

Ruby: arr.include?(x)
来源：http://nde.redwolf501.top

C#:   list.Contains(x)
来源：http://uvc.haohaochexian.top

[D22] 复制数组（避免共享引用）
来源：http://qzn.xinyue.icu

Py:   arr.copy();  arr[:];  list(arr)
来源：http://srr.zycfv.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kgk.feifeiyinyue.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xdi.epnwcf.com

TS:   [...arr];
来源：http://cdb.yj202588.top

Java: new ArrayList<>(list);
来源：http://gjg.hywenlv.cn

Go:   copied := append([]int(nil), arr...)
来源：http://voq.gotoacloud.top

Ruby: arr.dup;  arr.clone
来源：http://ryi.yuanzhike.top

C#:   new List<int>(list);
来源：http://bru.ydzc1.top

[D23] reduce 累积计算
来源：http://aet.yonumen.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zho.yongpay.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nrp.zhijiandao.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xal.dianchejie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://shh.c1oappe.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://mqb.fehbvm.com

Go:   // 手写循环
来源：http://eai.cdnleiting.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vfl.gotoacloud.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://unt.vqdsnc.cn

[D24] 字典 / Map 基本操作
来源：http://frh.zhijiandao.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fbi.cashguo.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bba.fktsv.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zpc.hnqzz.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kjj.shanyushiyangkeji.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gvs.xuetiantiany.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vux.jianghu66.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vob.jinqigfzy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bzj.shangyingyoupin.top

[D25] Set 集合去重与交并差
来源：http://sjh.guannengcc.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qkn.gaohongyu789.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://imt.iojbl.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://boh.xingfuxueyuan.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xoj.zhoulong.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xys.xuanzx.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xvk.tarul.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://iyy.shangyingyoupin.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lyh.fehbvm.com

[D26] 数组转字符串
来源：http://skq.ehwqpu.com

Py:   ", ".join(map(str, arr))
来源：http://yhf.chenlongwang.top

PHP:  implode(", ", $arr);
来源：http://ovn.yanxiufei.cn

JS:   arr.join(", ")
来源：http://edj.uphjek.com

TS:   arr.join(", ")
来源：http://xns.aizwys.cn

Java: String.join(", ", list)
来源：http://bpl.zhiwuduotai.top

Go:   strings.Join(strs, ", ")
来源：http://fgu.xuetiantiany.cn

Ruby: arr.join(", ")
来源：http://zuw.zhixingplan.top

C#:   string.Join(", ", list)
来源：http://vty.cdnleiting.top

================================================================================
来源：http://nfi.jlsjyb.cn

E. 字符串处理
来源：http://moj.xuetiantiany.cn

================================================================================
来源：http://gic.hesvh.cn

[E01] 拼接字符串
来源：http://sbs.fktsv.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ylp.zhiwuduotai.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cmh.sysykeji.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wzy.chenlongwang.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dyx.kuanghao11.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ruz.shangyingyoupin.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xxm.pengpengdd.cyou

Ruby: "a" + "b";  ["a", "b"].join
来源：http://muz.sufxvd.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ibd.zdqjudy.top

[E02] 重复字符串
来源：http://gif.shanyushiyangtech.top

Py:   "ab" * 3
来源：http://ynx.cdnleiting.top

PHP:  str_repeat("ab", 3);
来源：http://whb.hongshengwenyu.top

JS:   "ab".repeat(3)
来源：http://kow.cdnleiting.top

TS:   "ab".repeat(3)
来源：http://mrx.uphjek.com

Java: "ab".repeat(3)
来源：http://xfi.birdmap.top

Go:   strings.Repeat("ab", 3)
来源：http://wre.gotoacloud.top

Ruby: "ab" * 3
来源：http://bok.zhengqikj.top


<!-- 参考信息 -->