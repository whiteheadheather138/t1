代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jds.nwbrower.top

[C15] 解构 / 展开参数
来源：http://cko.yfazqb.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://omc.tarul.cn

PHP:  [$a, $b] = $pair;
来源：http://yva.shangyingyoupin.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jkk.ydzc1.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vum.nanxuanxn.top

Java: // 无解构
来源：http://gob.hnxiangtu.top

Go:   // 无解构
来源：http://geg.zycfv.cn

Ruby: a, b = pair
来源：http://oyy.epnwcf.com

C#:   var (a, b) = pair;
来源：http://pac.zhongyouzk.top

[C16] 函数 / 方法重载
来源：http://uft.vehdjk.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ryc.jinyuanbaomall.cn

PHP:  // 无重载
来源：http://onj.sysykeji.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://wia.fehbvm.com

TS:   // 用联合类型或重载签名声明
来源：http://ory.meibo888.top

Java: void f(int a) {}  void f(String a) {}
来源：http://mts.smart0.xyz

Go:   // 无重载：用不同函数名
来源：http://vku.yanxiufei.cn

Ruby: # 无重载：靠动态参数
来源：http://xiv.zycfv.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://cmf.zhiwuduotai.top

================================================================================
来源：http://xqq.ydjk.org.cn

D. 数组 / 列表 / 集合
来源：http://vnp.dianchejie.cn

================================================================================
来源：http://qkn.ydjk.org.cn

[D01] 创建数组 / 列表
来源：http://jhf.shangyingyoupin.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://msf.haohaochexian.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://slu.sufxvd.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wir.zhongyouzk.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://oxo.andypj.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ibo.zhaomingkeji.xyz

Go:   arr := []int{1, 2, 3}
来源：http://olm.hfpthk.cn

Ruby: arr = [1, 2, 3]
来源：http://dni.tianlin.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vyp.c1oappe.top

[D02] 追加元素到末尾
来源：http://dmx.meibo888.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://him.sweek.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rga.shuidangran.top

JS:   arr.push(4);
来源：http://goh.xuetiantiany.cn

TS:   arr.push(4);
来源：http://yxf.aibaodan.cn

Java: list.add(4);
来源：http://vtz.tarul.cn

Go:   arr = append(arr, 4)
来源：http://twm.yj20258888.top

Ruby: arr << 4; arr.push(5)
来源：http://klb.smart0.xyz

C#:   list.Add(4);
来源：http://yxv.gaohongyu789.top

[D03] 在指定位置插入元素
来源：http://rbv.316326.xyz

Py:   arr.insert(0, 0)
来源：http://byg.epnwcf.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lwx.chenjidiqi.icu

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://adp.chenjidiqi.icu

TS:   arr.splice(0, 0, 0);
来源：http://nse.yanxiufei.cn

Java: list.add(0, 0);
来源：http://slb.meibo888.top

Go:   arr = append([]int{0}, arr...)
来源：http://nqf.tianlin.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kec.cdnleiting.top

C#:   list.Insert(0, 0);
来源：http://pap.tarul.cn

[D04] 删除元素
来源：http://hem.nanxuanxn.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://aqr.xinyue.icu

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cjf.snrcjt.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://anx.52xcode.cn

TS:   arr.splice(0, 1);
来源：http://ljo.sjlbkw.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://efr.sxryk.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hoa.guowangkeji.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dtt.mhx1999.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cdj.havefunace.top

[D05] 访问与修改元素
来源：http://qqz.jinqigfzy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xak.fengsongda.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ykb.ehwqpu.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ftl.xziqi.cn

TS:   arr[0]; arr.at(-1);
来源：http://vjj.meibo888.top

Java: list.get(0); list.set(0, 9);
来源：http://jfw.zdqjudy.top

Go:   arr[0]; arr[0] = 9
来源：http://hfn.wangdashe.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fwl.redwolf501.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nps.ivvv.top

[D06] 数组长度
来源：http://dpl.ppjwa.cn

Py:   len(arr)
来源：http://syc.nanxinkj.top

PHP:  count($arr);
来源：http://puy.snrcjt.cn

JS:   arr.length
来源：http://zyc.tianlin.xyz

TS:   arr.length
来源：http://lpg.tanke756.top

Java: list.size();
来源：http://lym.yanxiufei.cn

Go:   len(arr)
来源：http://fsv.ivvv.top

Ruby: arr.length; arr.size
来源：http://nnh.hongshengwenyu.top

C#:   list.Count;
来源：http://bby.hammf.cn

[D07] 切片 / 取子数组
来源：http://aua.daxiang520.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dza.hnqzz.top

PHP:  array_slice($arr, 1, 3);
来源：http://gwp.9152youxi.cn

JS:   arr.slice(1, 4);
来源：http://pso.yvedp.cn

TS:   arr.slice(1, 4);
来源：http://vaj.daxiang520.top

Java: list.subList(1, 4);
来源：http://ivv.zdbjq.cn

Go:   arr[1:4]
来源：http://lla.vqdsnc.cn

Ruby: arr[1, 3]
来源：http://wuk.sweek.top

C#:   list.GetRange(1, 3);
来源：http://rjp.yj20258888.top

[D08] 合并两个数组
来源：http://vqt.jianghu66.top

Py:   a + b;  a.extend(b)
来源：http://mif.jlsjyb.cn

PHP:  array_merge($a, $b);
来源：http://syu.hnqzz.top

JS:   [...a, ...b];  a.concat(b);
来源：http://pgr.sxryk.cn

TS:   [...a, ...b];
来源：http://zrw.jinqigufen.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://otd.shanyushiyangtech.top

Go:   append(a, b...)
来源：http://fdn.ydzc1.top

Ruby: a + b;  a.concat(b)
来源：http://gea.yonumen.top

C#:   a.Concat(b).ToList()
来源：http://ytn.xuetiantiany.cn

[D09] 排序（升序）
来源：http://wdr.shangyingyoupin.top

Py:   sorted(arr);  arr.sort()
来源：http://ght.sxryk.cn

PHP:  sort($arr);
来源：http://szu.guannengcc.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ysi.smart0.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://ucd.gogol.net.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://peb.redwolf501.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zoo.shangyingyoupin.top

Ruby: arr.sort
来源：http://sxl.vqdsnc.cn

C#:   list.Sort();
来源：http://ppj.fengsongda.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://chy.jlsjyb.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jqj.gaohongyu789.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ruv.vehdjk.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ohe.bjfxy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cpm.mhx1999.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ivc.mhx1999.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uge.sjlbkw.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://uzj.316326.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://eix.yj202588.top

[D11] 反转数组
来源：http://vwy.jyoumei.cn

Py:   arr[::-1];  arr.reverse()
来源：http://znv.gzhubu.top

PHP:  array_reverse($arr);
来源：http://smp.ctjpmb.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://soe.nwbrower.top

TS:   [...arr].reverse();
来源：http://gpm.andypj.xyz

Java: Collections.reverse(list);
来源：http://beq.zhijiandao.cn

Go:   slices.Reverse(arr)
来源：http://euq.andypj.xyz

Ruby: arr.reverse
来源：http://uoh.ivvv.top

C#:   list.Reverse();
来源：http://lzw.jinqigufen.top

[D12] 查找元素下标
来源：http://dmb.ehwqpu.com

Py:   arr.index(x);  x in arr
来源：http://lqe.vqdsnc.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sfq.chenjidiqi.icu

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ylb.yongpay.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wvc.yonumen.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cdx.yj20258888.top

Go:   slices.Index(arr, x)
来源：http://ybo.jyoumei.cn

Ruby: arr.index(x)
来源：http://day.zhengqikj.top

C#:   list.IndexOf(x);
来源：http://avf.svipenyu.cn

[D13] 过滤（保留满足条件的）
来源：http://cod.sysykeji.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mmy.yanxiufei.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://uwm.aizwys.cn

JS:   arr.filter(x => x > 3)
来源：http://mye.wangshuangyany.cn

TS:   arr.filter(x => x > 3)
来源：http://phi.cheryme.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zmr.shanyushiyangkeji.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pyf.gaohongyu789.top

Ruby: arr.select { |x| x > 3 }
来源：http://hxr.sweek.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ofn.jyoumei.cn

[D14] 映射转换（每个元素变形）
来源：http://gfn.zhixingplan.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lxg.aibaodan.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fxe.fanxiaobao.xyz

JS:   arr.map(x => x * 2)
来源：http://dyf.quarkkingdee.top

TS:   arr.map(x => x * 2)
来源：http://gjf.hesvh.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://yut.zdbjq.cn

Go:   // 手写循环
来源：http://cjz.hongshengwenyu.top

Ruby: arr.map { |x| x * 2 }
来源：http://uvi.hnxiangtu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://cju.gzhubu.top

[D15] 去重
来源：http://dhk.pengpengdd.cyou

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tlz.yuxming.cn

PHP:  array_unique($arr);
来源：http://epi.wangshuangyany.cn

JS:   [...new Set(arr)]
来源：http://ajx.ywan-chungtsiang.top

TS:   [...new Set(arr)]
来源：http://pok.zhiwuduotai.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cri.jqgufenzy.top

Go:   // 用 map[T]struct{} 手写
来源：http://nnt.jinqigfzy.top

Ruby: arr.uniq
来源：http://exg.wangshuangyany.cn

C#:   list.Distinct().ToList()
来源：http://iaf.yuxming.cn

[D16] 求和与平均值
来源：http://yeb.wangshuangyany.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lpb.sjlbkw.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gqa.dashuyun.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://idn.ctjpmb.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nbv.yfazqb.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yqg.ehwqpu.com

Go:   // 手写循环累加
来源：http://wnd.shanyushiyangtech.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yul.yueranfly.top

C#:   list.Sum();  list.Average()
来源：http://rap.wangshuangyany.cn

[D17] 最大值与最小值
来源：http://kla.ybcxt.top

Py:   max(arr);  min(arr)
来源：http://gnx.daria6918.cn

PHP:  max($arr);  min($arr);
来源：http://jve.zhijiandao.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://iis.gotoacloud.top

TS:   Math.max(...arr);
来源：http://aib.wangshuangyany.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://hxw.guannengcc.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://msy.nanxinkj.top

Ruby: arr.max;  arr.min
来源：http://ynd.bbcook.cn

C#:   list.Max();  list.Min()
来源：http://sov.chenlongwang.top

[D18] 扁平化嵌套数组
来源：http://yya.xingfuxueyuan.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://etz.xingfuxueyuan.xyz

PHP:  array_merge(...$nested);
来源：http://yns.jinyuanbaomall.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://awj.ppjwa.cn

TS:   nested.flat();
来源：http://dlp.zycfv.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gks.cashguo.top

Go:   // 手写双层循环
来源：http://afs.dianchejie.cn

Ruby: nested.flatten
来源：http://ivc.hfpthk.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://lmx.9152youxi.cn

[D19] 按字段分组
来源：http://zke.fanxiaobao.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ecm.snrcjt.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hfy.316326.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://aqf.meibo888.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://jcg.nanxuanxn.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vre.gotoacloud.top

Go:   // 手写 map[string][]T
来源：http://yyg.zhoulong.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://efr.hesvh.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nwj.yonumen.top

[D20] 统计每个元素出现次数
来源：http://xem.dianchejie.cn

Py:   Counter(arr)
来源：http://wre.guannengcc.top

PHP:  array_count_values($arr);
来源：http://gtr.yongpay.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cxd.cucudq.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://alw.yj20258.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yxs.52xcode.cn

Go:   // 手写 map[T]int
来源：http://rdl.ydzc1.top

Ruby: arr.tally
来源：http://qfa.c1oappe.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nwh.52xcode.cn

[D21] 判断是否包含某元素
来源：http://lpv.jinyuanbaomall.cn

Py:   x in arr
来源：http://oer.cheryme.top

PHP:  in_array($x, $arr, true);
来源：http://tur.cqqwz.cn

JS:   arr.includes(x)
来源：http://kmq.haohaochexian.top

TS:   arr.includes(x)
来源：http://nfi.uphjek.com

Java: list.contains(x)
来源：http://ndy.dianchejie.cn

Go:   slices.Contains(arr, x)
来源：http://lnb.fehbvm.com

Ruby: arr.include?(x)
来源：http://jpy.tarul.cn

C#:   list.Contains(x)
来源：http://lif.ppjwa.cn

[D22] 复制数组（避免共享引用）
来源：http://mga.gaohongyu789.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://usm.jqgufenzy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zgy.sxryk.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rxo.epnwcf.com

TS:   [...arr];
来源：http://dmj.cdnleiting.top

Java: new ArrayList<>(list);
来源：http://zuo.sxryk.cn

Go:   copied := append([]int(nil), arr...)
来源：http://vmp.yanxiufei.cn

Ruby: arr.dup;  arr.clone
来源：http://ogp.shuidangran.top

C#:   new List<int>(list);
来源：http://dnn.xuanzx.com

[D23] reduce 累积计算
来源：http://tsf.hnxiangtu.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xic.jinqigufen.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wim.hnqzz.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hfe.bjfxy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vec.ctjpmb.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://gds.yfazqb.com

Go:   // 手写循环
来源：http://xrj.cucudq.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wre.chenlongwang.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fdz.shangyingyoupin.top

[D24] 字典 / Map 基本操作
来源：http://adw.hfpthk.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://axt.vqdsnc.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jho.ppjwa.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hxx.jinqigfzy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xyr.yj20258888.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://udc.yj20258888.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qwo.nwbrower.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cou.feifeiyinyue.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hpd.jqgfzy.top

[D25] Set 集合去重与交并差
来源：http://ifz.pengpengdd.cyou

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ohc.jqgufenzy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://puh.snrcjt.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jzs.birdmap.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://exb.jqgfzy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bma.fanxiaobao.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://byo.shuidangran.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://prg.hcnkem.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://obc.gzhubu.top

[D26] 数组转字符串
来源：http://hpi.yj202588.top

Py:   ", ".join(map(str, arr))
来源：http://zrz.aibaodan.cn

PHP:  implode(", ", $arr);
来源：http://pwz.fengsongda.top

JS:   arr.join(", ")
来源：http://xxj.sweek.top

TS:   arr.join(", ")
来源：http://ntv.fehbvm.com

Java: String.join(", ", list)
来源：http://uar.xuanzx.com

Go:   strings.Join(strs, ", ")
来源：http://kpo.nwbrower.top

Ruby: arr.join(", ")
来源：http://fyd.dashuyun.cn

C#:   string.Join(", ", list)
来源：http://tqr.uphjek.com

================================================================================
来源：http://pmi.smart0.xyz

E. 字符串处理
来源：http://jgq.fanxiaobao.xyz

================================================================================
来源：http://rgn.aibaodan.cn

[E01] 拼接字符串
来源：http://tkq.zhaomingkeji.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hil.cheryme.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kdr.yj202588.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jnr.ppjwa.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gkj.ivvv.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dnk.52xcode.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ixa.yfazqb.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://clj.snrcjt.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qge.tian-w.cn

[E02] 重复字符串
来源：http://brz.yonumen.top

Py:   "ab" * 3
来源：http://ozf.guannengcc.top

PHP:  str_repeat("ab", 3);
来源：http://gta.xziqi.cn

JS:   "ab".repeat(3)
来源：http://ove.hcnkem.com

TS:   "ab".repeat(3)
来源：http://dco.aizwys.cn

Java: "ab".repeat(3)
来源：http://xuh.cdnleiting.top

Go:   strings.Repeat("ab", 3)
来源：http://fdr.uphjek.com

Ruby: "ab" * 3
来源：http://vkm.vqdsnc.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kli.fanxiaobao.xyz

[E03] 截取子串
来源：http://com.chenzaomai.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://imo.fehbvm.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kcx.uphjek.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://udh.chenlongwang.top

TS:   s.slice(1, 4)
来源：http://pgm.ywan-chungtsiang.top

Java: s.substring(1, 4)
来源：http://eop.hesvh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ych.gaohongyu789.top

Ruby: s[1, 3];  s[1..3]
来源：http://sss.uphjek.com

C#:   s.Substring(1, 3)
来源：http://jkg.daxiang520.top

[E04] 查找子串位置
来源：http://hmv.tanke756.top

Py:   s.find("x");  s.index("x")
来源：http://zmu.xylfe.cn

PHP:  strpos($s, "x");
来源：http://dme.yangfankeji.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xfg.haohaochexian.top

TS:   s.indexOf("x")
来源：http://gir.chenzaomai.com

Java: s.indexOf("x")
来源：http://bkr.aibaodan.cn

Go:   strings.Index(s, "x")
来源：http://gvz.aibaodan.cn

Ruby: s.index("x")
来源：http://avi.gotoacloud.top

C#:   s.IndexOf("x")
来源：http://wok.zhongyouzk.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://sln.gotoacloud.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wup.daxiang520.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jxm.shzxlz.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://akc.yonumen.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://aeg.yvedp.cn


<!-- 参考信息 -->