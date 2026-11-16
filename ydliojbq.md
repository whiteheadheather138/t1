代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fnb.zhongyouzk.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wus.hesvh.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kkf.zhongyouzk.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://who.jyoumei.cn

Java: int add(int a, int b) { return a + b; }
来源：http://nxd.fengsongda.top

Go:   func add(a, b int) int
来源：http://tpl.sufxvd.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://otg.ctjpmb.com

C#:   int Add(int a, int b) => a + b;
来源：http://rqr.ppjwa.cn

[C14] 泛型函数
来源：http://dvt.316326.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mpv.uphjek.com

PHP:  // 无泛型
来源：http://ubb.hnxiangtu.top

JS:   // 无泛型
来源：http://lhc.hammf.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rkc.yuanzhike.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lno.c1oappe.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pha.dianchejie.cn

Ruby: # 无泛型
来源：http://noj.yanxiufei.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dak.zhiwuduotai.top

[C15] 解构 / 展开参数
来源：http://apc.guowangkeji.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dke.vqdsnc.cn

PHP:  [$a, $b] = $pair;
来源：http://ane.jinqigfzy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://oie.pycfn.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fli.hnxiangtu.top

Java: // 无解构
来源：http://pjl.bbcook.cn

Go:   // 无解构
来源：http://kfe.tianlin.xyz

Ruby: a, b = pair
来源：http://uwb.chenlongwang.top

C#:   var (a, b) = pair;
来源：http://sst.ydzc1.top

[C16] 函数 / 方法重载
来源：http://nzu.vqdsnc.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kwd.yfazqb.com

PHP:  // 无重载
来源：http://gnr.hywenlv.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://keq.jinqigfzy.top

TS:   // 用联合类型或重载签名声明
来源：http://orn.zhiwuduotai.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ivu.yonumen.top

Go:   // 无重载：用不同函数名
来源：http://wlg.yangfankeji.com

Ruby: # 无重载：靠动态参数
来源：http://hhm.guannengcc.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://kef.zhiwuduotai.top

================================================================================
来源：http://cie.hesvh.cn

D. 数组 / 列表 / 集合
来源：http://ems.hysaishi.cn

================================================================================
来源：http://kbn.uphjek.com

[D01] 创建数组 / 列表
来源：http://jkr.hongshengwenyu.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://zxm.yfazqb.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gah.tianlin.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ukf.hongshengwenyu.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://lxt.ywan-chungtsiang.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://drp.ybcxt.top

Go:   arr := []int{1, 2, 3}
来源：http://oos.gzhubu.top

Ruby: arr = [1, 2, 3]
来源：http://vfi.sufxvd.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zfe.svipenyu.cn

[D02] 追加元素到末尾
来源：http://ols.mhx1999.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gld.nanxuanxn.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cpz.gotoacloud.top

JS:   arr.push(4);
来源：http://his.shzxlz.cn

TS:   arr.push(4);
来源：http://umu.xingfuxueyuan.xyz

Java: list.add(4);
来源：http://uvx.shanyushiyangkeji.top

Go:   arr = append(arr, 4)
来源：http://jip.nanxuanxn.top

Ruby: arr << 4; arr.push(5)
来源：http://ahu.xinyue.icu

C#:   list.Add(4);
来源：http://hmz.vehdjk.com

[D03] 在指定位置插入元素
来源：http://drz.c1oappe.top

Py:   arr.insert(0, 0)
来源：http://bzm.aizwys.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vwv.bbcook.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zlr.daria6918.cn

TS:   arr.splice(0, 0, 0);
来源：http://ypr.jiagoushi.top

Java: list.add(0, 0);
来源：http://dwn.zhaomingkeji.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://ciq.vqdsnc.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fbq.xziqi.cn

C#:   list.Insert(0, 0);
来源：http://beo.quarkkingdee.top

[D04] 删除元素
来源：http://qaz.yj20258888.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uly.daria6918.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vkr.hesvh.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sjc.zhaomingkeji.xyz

TS:   arr.splice(0, 1);
来源：http://qqg.xinyue.icu

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://uzh.smart0.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bti.hesvh.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xrv.ybcxt.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://krm.kuanghao11.cn

[D05] 访问与修改元素
来源：http://nry.epnwcf.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://toy.xingfuxueyuan.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pvt.ppjwa.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rkv.hcnkem.com

TS:   arr[0]; arr.at(-1);
来源：http://lat.sufxvd.cn

Java: list.get(0); list.set(0, 9);
来源：http://lip.yueranfly.top

Go:   arr[0]; arr[0] = 9
来源：http://zsi.cdnleiting.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wfx.havefunace.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qlh.shzxlz.cn

[D06] 数组长度
来源：http://sdr.fktsv.cn

Py:   len(arr)
来源：http://hcs.tian-w.cn

PHP:  count($arr);
来源：http://ury.wangdashe.top

JS:   arr.length
来源：http://ejg.zhongyouzk.top

TS:   arr.length
来源：http://jom.ehwqpu.com

Java: list.size();
来源：http://qrw.jinqigufen.top

Go:   len(arr)
来源：http://rrk.ydjk.org.cn

Ruby: arr.length; arr.size
来源：http://myb.vqdsnc.cn

C#:   list.Count;
来源：http://tcp.chenlongwang.top

[D07] 切片 / 取子数组
来源：http://awt.yuanzhike.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vkj.jinghuilouyu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://kzj.iojbl.cn

JS:   arr.slice(1, 4);
来源：http://oxn.yanxiufei.cn

TS:   arr.slice(1, 4);
来源：http://pjw.sxryk.cn

Java: list.subList(1, 4);
来源：http://fnr.pengpengdd.cyou

Go:   arr[1:4]
来源：http://hpz.yvedp.cn

Ruby: arr[1, 3]
来源：http://nks.shangyingyoupin.top

C#:   list.GetRange(1, 3);
来源：http://klp.zdqjudy.top

[D08] 合并两个数组
来源：http://ljr.vqdsnc.cn

Py:   a + b;  a.extend(b)
来源：http://gqr.birdmap.top

PHP:  array_merge($a, $b);
来源：http://lyp.jianghu66.top

JS:   [...a, ...b];  a.concat(b);
来源：http://aec.vehdjk.com

TS:   [...a, ...b];
来源：http://fsd.ydzc1.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://clx.jinyuanbaomall.cn

Go:   append(a, b...)
来源：http://gjo.yueranfly.top

Ruby: a + b;  a.concat(b)
来源：http://kvh.smart0.xyz

C#:   a.Concat(b).ToList()
来源：http://mpq.zdqjudy.top

[D09] 排序（升序）
来源：http://jan.yangfankeji.com

Py:   sorted(arr);  arr.sort()
来源：http://rap.yanxiufei.cn

PHP:  sort($arr);
来源：http://pux.gotoacloud.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ubl.gaohongyu789.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://mgr.fzhhl.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ypt.shzxlz.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://thz.xinyue.icu

Ruby: arr.sort
来源：http://pas.yvedp.cn

C#:   list.Sort();
来源：http://zeg.sxryk.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://knt.jinqigufen.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://unq.xinyue.icu

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sjm.birdmap.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://riu.52xcode.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ret.cdnleiting.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kxd.cashguo.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uvo.aizwys.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kzh.hywenlv.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zam.zhixingplan.top

[D11] 反转数组
来源：http://ygf.316326.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://can.c1oappe.top

PHP:  array_reverse($arr);
来源：http://web.mhx1999.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pej.tarul.cn

TS:   [...arr].reverse();
来源：http://idw.shangyingyoupin.top

Java: Collections.reverse(list);
来源：http://uid.ivvv.top

Go:   slices.Reverse(arr)
来源：http://gbu.hcnkem.com

Ruby: arr.reverse
来源：http://xfk.guowangkeji.top

C#:   list.Reverse();
来源：http://jyw.gotoacloud.top

[D12] 查找元素下标
来源：http://thp.gzhubu.top

Py:   arr.index(x);  x in arr
来源：http://byp.haohaochexian.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wha.yfazqb.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gbv.pycfn.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://aty.hongshengwenyu.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://msp.jiagoushi.top

Go:   slices.Index(arr, x)
来源：http://qbr.hfpthk.cn

Ruby: arr.index(x)
来源：http://lnu.aizwys.cn

C#:   list.IndexOf(x);
来源：http://qjk.hnxiangtu.top

[D13] 过滤（保留满足条件的）
来源：http://joa.fanxiaobao.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ofi.tarul.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yqz.svipenyu.cn

JS:   arr.filter(x => x > 3)
来源：http://uki.vqdsnc.cn

TS:   arr.filter(x => x > 3)
来源：http://lrm.sweek.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lku.chenlongwang.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pva.52xcode.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fjg.ywan-chungtsiang.top

C#:   list.Where(x => x > 3).ToList()
来源：http://twq.zhongyouzk.top

[D14] 映射转换（每个元素变形）
来源：http://wir.tian-w.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://obm.andypj.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mge.epnwcf.com

JS:   arr.map(x => x * 2)
来源：http://drn.uphjek.com

TS:   arr.map(x => x * 2)
来源：http://dfv.nwbrower.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://mof.gaohongyu789.top

Go:   // 手写循环
来源：http://fuy.fzhhl.top

Ruby: arr.map { |x| x * 2 }
来源：http://ijn.epnwcf.com

C#:   list.Select(x => x * 2).ToList()
来源：http://ghy.yj20258888.top

[D15] 去重
来源：http://squ.fengsongda.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jyp.guowangkeji.top

PHP:  array_unique($arr);
来源：http://zur.wangshuangyany.cn

JS:   [...new Set(arr)]
来源：http://wnu.xylfe.cn

TS:   [...new Set(arr)]
来源：http://yqt.hfpthk.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zwf.316326.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://mar.daria6918.cn

Ruby: arr.uniq
来源：http://ael.ppjwa.cn

C#:   list.Distinct().ToList()
来源：http://dmf.cashguo.top

[D16] 求和与平均值
来源：http://cru.redwolf501.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://grn.yanxiufei.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nrh.gzhubu.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://was.daria6918.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fop.shuidangran.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qjm.xingfuxueyuan.xyz

Go:   // 手写循环累加
来源：http://dwg.sxryk.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rgz.fengsongda.top

C#:   list.Sum();  list.Average()
来源：http://lbu.snrcjt.cn

[D17] 最大值与最小值
来源：http://ttk.zhengqikj.top

Py:   max(arr);  min(arr)
来源：http://dyr.sufxvd.cn

PHP:  max($arr);  min($arr);
来源：http://fzb.hysaishi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tyo.ctjpmb.com

TS:   Math.max(...arr);
来源：http://cof.yangfankeji.com

Java: Collections.max(list);  Collections.min(list);
来源：http://mzi.hesvh.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vau.0kj1m.cn

Ruby: arr.max;  arr.min
来源：http://ugz.redwolf501.top

C#:   list.Max();  list.Min()
来源：http://bzn.sysykeji.top

[D18] 扁平化嵌套数组
来源：http://duj.c1oappe.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jxd.snrcjt.cn

PHP:  array_merge(...$nested);
来源：http://opo.zdqjudy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://izd.bbcook.cn

TS:   nested.flat();
来源：http://pfn.chenzaomai.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lry.hesvh.cn

Go:   // 手写双层循环
来源：http://pwc.haohaochexian.top

Ruby: nested.flatten
来源：http://zpw.cucudq.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://rry.shuidangran.top

[D19] 按字段分组
来源：http://ndx.hnxiangtu.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bwv.yj20258888.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pfo.jqgfzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gbq.yj20258888.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://rpk.316326.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zmq.jinyuanbaomall.cn

Go:   // 手写 map[string][]T
来源：http://nsq.c1oappe.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://uoh.hnqzz.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://obk.hfpthk.cn

[D20] 统计每个元素出现次数
来源：http://ika.aibaodan.cn

Py:   Counter(arr)
来源：http://ylc.gaohongyu789.top

PHP:  array_count_values($arr);
来源：http://okr.c1oappe.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hhy.chenzaomai.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://afh.yonumen.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hdz.yuxming.cn

Go:   // 手写 map[T]int
来源：http://mtt.zycfv.cn

Ruby: arr.tally
来源：http://avl.hfpthk.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gmx.hongshengwenyu.top

[D21] 判断是否包含某元素
来源：http://dnm.ydjk.org.cn

Py:   x in arr
来源：http://nrd.c1oappe.top

PHP:  in_array($x, $arr, true);
来源：http://bpf.nanxinkj.top

JS:   arr.includes(x)
来源：http://ysz.hesvh.cn

TS:   arr.includes(x)
来源：http://xiq.jqgfzy.top

Java: list.contains(x)
来源：http://yne.cheryme.top

Go:   slices.Contains(arr, x)
来源：http://tvi.ywan-chungtsiang.top

Ruby: arr.include?(x)
来源：http://dna.jqgfzy.top

C#:   list.Contains(x)
来源：http://rhz.zhoulong.xyz

[D22] 复制数组（避免共享引用）
来源：http://ryn.hfpthk.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nua.cucudq.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lld.yueranfly.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qiz.ppjwa.cn

TS:   [...arr];
来源：http://hhq.aibaodan.cn

Java: new ArrayList<>(list);
来源：http://rzr.cheryme.top

Go:   copied := append([]int(nil), arr...)
来源：http://ybp.feifeiyinyue.top

Ruby: arr.dup;  arr.clone
来源：http://szl.jyoumei.cn

C#:   new List<int>(list);
来源：http://ahu.zhoulong.xyz

[D23] reduce 累积计算
来源：http://odt.nwbrower.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zij.snrcjt.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kox.wangshuangyany.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qcn.ehwqpu.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ows.daxiang520.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://nbv.hongshengwenyu.top

Go:   // 手写循环
来源：http://zke.wangdashe.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lag.fzhhl.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nyt.daxiang520.top

[D24] 字典 / Map 基本操作
来源：http://oub.cqqwz.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zmd.xingfuxueyuan.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pjr.chenjidiqi.icu

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xla.jianghu66.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cvl.sufxvd.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://amy.fktsv.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://eci.yongpay.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bgf.svipenyu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gdn.hfpthk.cn

[D25] Set 集合去重与交并差
来源：http://mxa.zhongyouzk.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://byj.jqgufenzy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xly.hywenlv.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yge.jinqigfzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://inp.jqgufenzy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vbk.jinyuanbaomall.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vmr.zhijiandao.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hev.c1oappe.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jkr.hcnkem.com

[D26] 数组转字符串
来源：http://eil.hcnkem.com

Py:   ", ".join(map(str, arr))
来源：http://joc.kuanghao11.cn

PHP:  implode(", ", $arr);
来源：http://njj.pengpengdd.cyou

JS:   arr.join(", ")
来源：http://mmx.zycfv.cn

TS:   arr.join(", ")
来源：http://img.nanxuanxn.top

Java: String.join(", ", list)
来源：http://nxe.shuidangran.top

Go:   strings.Join(strs, ", ")
来源：http://ucd.cdnleiting.top

Ruby: arr.join(", ")
来源：http://tci.jinyuanbaomall.cn

C#:   string.Join(", ", list)
来源：http://qph.9152youxi.cn

================================================================================
来源：http://xxk.c1oappe.top

E. 字符串处理
来源：http://jie.andypj.xyz

================================================================================
来源：http://skd.nanxuanxn.top

[E01] 拼接字符串
来源：http://mnl.svipenyu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fxy.nwbrower.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lgb.ehwqpu.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rde.nwbrower.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dmx.sjlbkw.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ysb.jlsjyb.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rid.shanyushiyangkeji.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dib.jlsjyb.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zgl.fengsongda.top

[E02] 重复字符串
来源：http://frf.sufxvd.cn

Py:   "ab" * 3
来源：http://eit.sweek.top

PHP:  str_repeat("ab", 3);
来源：http://lsb.nanxuanxn.top

JS:   "ab".repeat(3)
来源：http://jrk.xylfe.cn

TS:   "ab".repeat(3)
来源：http://qpj.chenzaomai.com

Java: "ab".repeat(3)
来源：http://osl.gaohongyu789.top

Go:   strings.Repeat("ab", 3)
来源：http://zvm.andypj.xyz

Ruby: "ab" * 3
来源：http://hzy.hammf.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yvg.birdmap.top

[E03] 截取子串
来源：http://ptg.yangfankeji.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gcs.0kj1m.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nub.shzxlz.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jcm.fanxiaobao.xyz

TS:   s.slice(1, 4)
来源：http://gsr.yj202588.top

Java: s.substring(1, 4)
来源：http://gxd.dianchejie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ylj.cqqwz.cn


<!-- 参考信息 -->