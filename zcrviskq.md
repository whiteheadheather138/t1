代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://wrw.epnwcf.com

JS:   (() => { console.log("run"); })();
来源：http://sni.sysykeji.top

TS:   (() => { console.log("run"); })();
来源：http://rdb.cashguo.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ocf.sxryk.cn

Go:   func() { fmt.Println("run") }()
来源：http://tww.gaohongyu789.top

Ruby: -> { puts "run" }.call
来源：http://nhv.jinqigfzy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://sox.316326.xyz

[C13] 类型声明 / 类型注解
来源：http://iei.aizwys.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hcm.snrcjt.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cxh.zhaomingkeji.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://aze.jlsjyb.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://aeo.jinyuanbaomall.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cpz.jyoumei.cn

Go:   func add(a, b int) int
来源：http://mde.xuetiantiany.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://oph.hysaishi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://pam.ehwqpu.com

[C14] 泛型函数
来源：http://mjg.hywenlv.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ejr.chenjidiqi.icu

PHP:  // 无泛型
来源：http://imn.wangdashe.top

JS:   // 无泛型
来源：http://fpb.cucudq.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ibf.wangshuangyany.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xrs.daxiang520.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://klf.xziqi.cn

Ruby: # 无泛型
来源：http://uqb.jinyuanbaomall.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nyj.xuetiantiany.cn

[C15] 解构 / 展开参数
来源：http://tku.bbcook.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://adu.guannengcc.top

PHP:  [$a, $b] = $pair;
来源：http://uea.zhoulong.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yfe.cdnleiting.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://oue.gzhubu.top

Java: // 无解构
来源：http://adf.shangyingyoupin.top

Go:   // 无解构
来源：http://vrp.jinyuanbaomall.cn

Ruby: a, b = pair
来源：http://bow.xziqi.cn

C#:   var (a, b) = pair;
来源：http://uii.hongshengwenyu.top

[C16] 函数 / 方法重载
来源：http://ici.uphjek.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rgo.shanyushiyangkeji.top

PHP:  // 无重载
来源：http://rpa.xuanzx.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://gos.svipenyu.cn

TS:   // 用联合类型或重载签名声明
来源：http://hgr.ybcxt.top

Java: void f(int a) {}  void f(String a) {}
来源：http://dph.wangdashe.top

Go:   // 无重载：用不同函数名
来源：http://bee.zhijiandao.cn

Ruby: # 无重载：靠动态参数
来源：http://qql.zhaomingkeji.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://qhr.zhoulong.xyz

================================================================================
来源：http://thj.xuetiantiany.cn

D. 数组 / 列表 / 集合
来源：http://bjc.epnwcf.com

================================================================================
来源：http://frv.hongshengwenyu.top

[D01] 创建数组 / 列表
来源：http://yat.zhixingplan.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://cjp.gogol.net.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://evb.xziqi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lxn.sxryk.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://vtu.cqqwz.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wui.nanxinkj.top

Go:   arr := []int{1, 2, 3}
来源：http://gug.yanxiufei.cn

Ruby: arr = [1, 2, 3]
来源：http://dww.dianchejie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yxe.zhaomingkeji.xyz

[D02] 追加元素到末尾
来源：http://nea.shanyushiyangkeji.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cgt.nanxinkj.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vzu.dianchejie.cn

JS:   arr.push(4);
来源：http://bsv.hnqzz.top

TS:   arr.push(4);
来源：http://cvo.yueranfly.top

Java: list.add(4);
来源：http://sef.chenzaomai.com

Go:   arr = append(arr, 4)
来源：http://uds.hcnkem.com

Ruby: arr << 4; arr.push(5)
来源：http://ktw.zdbjq.cn

C#:   list.Add(4);
来源：http://lfa.cqqwz.cn

[D03] 在指定位置插入元素
来源：http://reg.sjlbkw.cn

Py:   arr.insert(0, 0)
来源：http://gwb.pengpengdd.cyou

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mco.hnxiangtu.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mib.tian-w.cn

TS:   arr.splice(0, 0, 0);
来源：http://npx.xziqi.cn

Java: list.add(0, 0);
来源：http://bcs.epnwcf.com

Go:   arr = append([]int{0}, arr...)
来源：http://ihc.ctjpmb.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qch.yangfankeji.com

C#:   list.Insert(0, 0);
来源：http://ebx.jinqigufen.top

[D04] 删除元素
来源：http://jsr.yfazqb.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xgd.cdnleiting.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gou.epnwcf.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lhn.jqgfzy.top

TS:   arr.splice(0, 1);
来源：http://tuk.hongshengwenyu.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hnj.tanke756.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gnx.yuanzhike.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rkq.mhx1999.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xua.nanxinkj.top

[D05] 访问与修改元素
来源：http://fid.hesvh.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xzx.zhongyouzk.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dkw.hcnkem.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ebp.316326.xyz

TS:   arr[0]; arr.at(-1);
来源：http://hqy.wangshuangyany.cn

Java: list.get(0); list.set(0, 9);
来源：http://qtb.xingfuxueyuan.xyz

Go:   arr[0]; arr[0] = 9
来源：http://kdg.shanyushiyangkeji.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pri.jinyuanbaomall.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://caw.yueranfly.top

[D06] 数组长度
来源：http://wmq.nwbrower.top

Py:   len(arr)
来源：http://gwu.uphjek.com

PHP:  count($arr);
来源：http://yia.jinyuanbaomall.cn

JS:   arr.length
来源：http://osu.xziqi.cn

TS:   arr.length
来源：http://kbr.chenlongwang.top

Java: list.size();
来源：http://bzk.316326.xyz

Go:   len(arr)
来源：http://fyn.jinghuilouyu.cn

Ruby: arr.length; arr.size
来源：http://guz.andypj.xyz

C#:   list.Count;
来源：http://rsw.ybcxt.top

[D07] 切片 / 取子数组
来源：http://voz.zhoulong.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://myy.cdnleiting.top

PHP:  array_slice($arr, 1, 3);
来源：http://ogv.jinghuilouyu.cn

JS:   arr.slice(1, 4);
来源：http://elw.yfazqb.com

TS:   arr.slice(1, 4);
来源：http://qbu.meibo888.top

Java: list.subList(1, 4);
来源：http://jah.zhixingplan.top

Go:   arr[1:4]
来源：http://wli.pengpengdd.cyou

Ruby: arr[1, 3]
来源：http://dme.xziqi.cn

C#:   list.GetRange(1, 3);
来源：http://mqz.chenlongwang.top

[D08] 合并两个数组
来源：http://uhv.andypj.xyz

Py:   a + b;  a.extend(b)
来源：http://yhf.xingfuxueyuan.xyz

PHP:  array_merge($a, $b);
来源：http://sxl.svipenyu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://qfx.jiagoushi.top

TS:   [...a, ...b];
来源：http://fdy.gzhubu.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rkj.tian-w.cn

Go:   append(a, b...)
来源：http://oqt.hesvh.cn

Ruby: a + b;  a.concat(b)
来源：http://vdn.hfpthk.cn

C#:   a.Concat(b).ToList()
来源：http://zlw.haohaochexian.top

[D09] 排序（升序）
来源：http://tvf.shuidangran.top

Py:   sorted(arr);  arr.sort()
来源：http://tqm.hnxiangtu.top

PHP:  sort($arr);
来源：http://nfk.hongshengwenyu.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://usc.shanyushiyangtech.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://shl.gzhubu.top

Java: Collections.sort(list);  list.sort(null);
来源：http://fsx.tanke756.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tgo.gaohongyu789.top

Ruby: arr.sort
来源：http://zgt.zhoulong.xyz

C#:   list.Sort();
来源：http://wwl.hywenlv.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xcf.guowangkeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xja.yj20258.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xaz.pycfn.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zbw.tian-w.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mjj.gogol.net.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cca.pengpengdd.cyou

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ord.epnwcf.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rsv.feifeiyinyue.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ebb.dianchejie.cn

[D11] 反转数组
来源：http://cdl.guannengcc.top

Py:   arr[::-1];  arr.reverse()
来源：http://uqw.0kj1m.cn

PHP:  array_reverse($arr);
来源：http://esa.yangfankeji.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://btg.xuanzx.com

TS:   [...arr].reverse();
来源：http://xsy.316326.xyz

Java: Collections.reverse(list);
来源：http://yvm.shzxlz.cn

Go:   slices.Reverse(arr)
来源：http://ymz.gotoacloud.top

Ruby: arr.reverse
来源：http://sen.cqqwz.cn

C#:   list.Reverse();
来源：http://vpu.xingfuxueyuan.xyz

[D12] 查找元素下标
来源：http://lix.tian-w.cn

Py:   arr.index(x);  x in arr
来源：http://bvg.yueranfly.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wmq.ehwqpu.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ioa.xziqi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://upi.aibaodan.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rir.feifeiyinyue.top

Go:   slices.Index(arr, x)
来源：http://twn.zhongyouzk.top

Ruby: arr.index(x)
来源：http://sgn.9152youxi.cn

C#:   list.IndexOf(x);
来源：http://nwl.yj20258.top

[D13] 过滤（保留满足条件的）
来源：http://rxk.yfazqb.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jdb.zhiwuduotai.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://att.jinqigufen.top

JS:   arr.filter(x => x > 3)
来源：http://ary.ydjk.org.cn

TS:   arr.filter(x => x > 3)
来源：http://jfy.hfpthk.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yxq.vehdjk.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://evs.tanke756.top

Ruby: arr.select { |x| x > 3 }
来源：http://ydl.zdqjudy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://vdk.aibaodan.cn

[D14] 映射转换（每个元素变形）
来源：http://jqa.hongshengwenyu.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://isj.bjfxy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pzm.ctjpmb.com

JS:   arr.map(x => x * 2)
来源：http://ovc.snrcjt.cn

TS:   arr.map(x => x * 2)
来源：http://ntv.pycfn.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://jbs.xziqi.cn

Go:   // 手写循环
来源：http://hjh.zhijiandao.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dnf.316326.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://odp.tian-w.cn

[D15] 去重
来源：http://muo.zhaomingkeji.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dhs.guowangkeji.top

PHP:  array_unique($arr);
来源：http://rpk.wangshuangyany.cn

JS:   [...new Set(arr)]
来源：http://zmp.yangfankeji.com

TS:   [...new Set(arr)]
来源：http://apj.yanxiufei.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://aja.cdnleiting.top

Go:   // 用 map[T]struct{} 手写
来源：http://jfb.cashguo.top

Ruby: arr.uniq
来源：http://njg.0kj1m.cn

C#:   list.Distinct().ToList()
来源：http://roj.jqgfzy.top

[D16] 求和与平均值
来源：http://xuk.yanxiufei.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hyf.vqdsnc.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dmh.jinghuilouyu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://esa.snrcjt.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://oux.cqqwz.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wxd.uphjek.com

Go:   // 手写循环累加
来源：http://mwp.hnqzz.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bqz.quarkkingdee.top

C#:   list.Sum();  list.Average()
来源：http://equ.quarkkingdee.top

[D17] 最大值与最小值
来源：http://nlj.jianghu66.top

Py:   max(arr);  min(arr)
来源：http://fdq.gzhubu.top

PHP:  max($arr);  min($arr);
来源：http://cwd.sxryk.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wla.chenzaomai.com

TS:   Math.max(...arr);
来源：http://qaa.mhx1999.top

Java: Collections.max(list);  Collections.min(list);
来源：http://csk.zycfv.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kug.hysaishi.cn

Ruby: arr.max;  arr.min
来源：http://boz.cucudq.cn

C#:   list.Max();  list.Min()
来源：http://bqv.sysykeji.top

[D18] 扁平化嵌套数组
来源：http://dil.ivvv.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ciu.9152youxi.cn

PHP:  array_merge(...$nested);
来源：http://who.meibo888.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vdu.chenzaomai.com

TS:   nested.flat();
来源：http://zue.shuidangran.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dug.xingfuxueyuan.xyz

Go:   // 手写双层循环
来源：http://nqn.zhengqikj.top

Ruby: nested.flatten
来源：http://otv.sxryk.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yph.316326.xyz

[D19] 按字段分组
来源：http://xqf.hammf.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pcq.ctjpmb.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yxo.jyoumei.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kck.feifeiyinyue.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://axp.zhengqikj.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gxn.zycfv.cn

Go:   // 手写 map[string][]T
来源：http://cmh.zdbjq.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://iaq.cqqwz.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tug.shangyingyoupin.top

[D20] 统计每个元素出现次数
来源：http://ecq.vqdsnc.cn

Py:   Counter(arr)
来源：http://qyb.zhiwuduotai.top

PHP:  array_count_values($arr);
来源：http://aut.svipenyu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://juu.chenjidiqi.icu

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iez.fzhhl.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://awl.tianlin.xyz

Go:   // 手写 map[T]int
来源：http://cge.daxiang520.top

Ruby: arr.tally
来源：http://kkz.shanyushiyangkeji.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wqe.zdbjq.cn

[D21] 判断是否包含某元素
来源：http://nvi.cashguo.top

Py:   x in arr
来源：http://xsr.gzhubu.top

PHP:  in_array($x, $arr, true);
来源：http://mre.jinqigufen.top

JS:   arr.includes(x)
来源：http://ttn.iojbl.cn

TS:   arr.includes(x)
来源：http://htf.xuanzx.com

Java: list.contains(x)
来源：http://ajh.gotoacloud.top

Go:   slices.Contains(arr, x)
来源：http://crf.ywan-chungtsiang.top

Ruby: arr.include?(x)
来源：http://hqu.shzxlz.cn

C#:   list.Contains(x)
来源：http://vtj.chenzaomai.com

[D22] 复制数组（避免共享引用）
来源：http://qtg.xziqi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wuz.zhijiandao.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zbf.jinqigufen.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://aqf.52xcode.cn

TS:   [...arr];
来源：http://dlo.bbcook.cn

Java: new ArrayList<>(list);
来源：http://uci.gotoacloud.top

Go:   copied := append([]int(nil), arr...)
来源：http://etn.shangyingyoupin.top

Ruby: arr.dup;  arr.clone
来源：http://qcv.yueranfly.top

C#:   new List<int>(list);
来源：http://ibt.svipenyu.cn

[D23] reduce 累积计算
来源：http://wty.nanxuanxn.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mhw.jyoumei.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://swe.yvedp.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fol.daria6918.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pxa.fanxiaobao.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://pts.sjlbkw.cn

Go:   // 手写循环
来源：http://szc.xingfuxueyuan.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fbi.sweek.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dpv.kuanghao11.cn

[D24] 字典 / Map 基本操作
来源：http://jst.gogol.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jwc.ybcxt.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qex.yj20258888.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ydz.cqqwz.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cos.chenzaomai.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xrm.zycfv.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cet.redwolf501.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ajl.pengpengdd.cyou

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zyi.yueranfly.top

[D25] Set 集合去重与交并差
来源：http://rbn.fehbvm.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ppt.zhijiandao.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wzo.sweek.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pqf.zhijiandao.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zhd.cdnleiting.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jfb.yuxming.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mcj.zhijiandao.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ovf.yuxming.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xxy.xinyue.icu

[D26] 数组转字符串
来源：http://gud.guowangkeji.top

Py:   ", ".join(map(str, arr))
来源：http://nax.guowangkeji.top

PHP:  implode(", ", $arr);
来源：http://kuz.cucudq.cn

JS:   arr.join(", ")
来源：http://cfk.ppjwa.cn

TS:   arr.join(", ")
来源：http://wmi.xuanzx.com

Java: String.join(", ", list)
来源：http://mvm.dianchejie.cn

Go:   strings.Join(strs, ", ")
来源：http://ies.jiagoushi.top

Ruby: arr.join(", ")
来源：http://xaw.pycfn.com

C#:   string.Join(", ", list)
来源：http://pqs.gzhubu.top

================================================================================
来源：http://klk.hfpthk.cn

E. 字符串处理
来源：http://egw.zdqjudy.top

================================================================================
来源：http://bpq.wangdashe.top

[E01] 拼接字符串
来源：http://byd.fktsv.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jfg.jqgufenzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sto.daxiang520.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://aic.jiagoushi.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gir.xingfuxueyuan.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sna.9152youxi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sqc.jinyuanbaomall.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dil.yueranfly.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pzd.xinyue.icu

[E02] 重复字符串
来源：http://tmx.shangyingyoupin.top

Py:   "ab" * 3
来源：http://zwd.jinyuanbaomall.cn

PHP:  str_repeat("ab", 3);
来源：http://eli.hysaishi.cn

JS:   "ab".repeat(3)
来源：http://czk.shzxlz.cn

TS:   "ab".repeat(3)
来源：http://unr.zhijiandao.cn

Java: "ab".repeat(3)
来源：http://hzi.zdbjq.cn

Go:   strings.Repeat("ab", 3)
来源：http://qwn.fehbvm.com

Ruby: "ab" * 3
来源：http://soi.iojbl.cn


<!-- 参考信息 -->