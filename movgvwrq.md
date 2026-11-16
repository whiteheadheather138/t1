代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ack.xinyue.icu

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lge.chenjidiqi.icu

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mpd.yvedp.cn

Ruby: # 无泛型
来源：http://vng.sufxvd.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xjk.redwolf501.top

[C15] 解构 / 展开参数
来源：http://hzt.ydzc1.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bqh.52xcode.cn

PHP:  [$a, $b] = $pair;
来源：http://lfw.hnxiangtu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://sod.bbcook.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yqm.cqqwz.cn

Java: // 无解构
来源：http://avq.xuanzx.com

Go:   // 无解构
来源：http://lbe.shanyushiyangtech.top

Ruby: a, b = pair
来源：http://hzq.ydzc1.top

C#:   var (a, b) = pair;
来源：http://fpg.hfpthk.cn

[C16] 函数 / 方法重载
来源：http://vfi.yuanzhike.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bbn.jinqigfzy.top

PHP:  // 无重载
来源：http://dvj.jqgfzy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://mdo.dashuyun.cn

TS:   // 用联合类型或重载签名声明
来源：http://qxq.yonumen.top

Java: void f(int a) {}  void f(String a) {}
来源：http://fta.shzxlz.cn

Go:   // 无重载：用不同函数名
来源：http://edp.yvedp.cn

Ruby: # 无重载：靠动态参数
来源：http://scx.nwbrower.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://oxy.zdbjq.cn

================================================================================
来源：http://imn.hcnkem.com

D. 数组 / 列表 / 集合
来源：http://xpe.aizwys.cn

================================================================================
来源：http://wiw.zhengqikj.top

[D01] 创建数组 / 列表
来源：http://cxd.fktsv.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://bqg.tanke756.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mzt.chenzaomai.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xwj.hnxiangtu.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://gfz.redwolf501.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fwz.chenjidiqi.icu

Go:   arr := []int{1, 2, 3}
来源：http://pya.bbcook.cn

Ruby: arr = [1, 2, 3]
来源：http://lbl.zhongyouzk.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vvz.jinyuanbaomall.cn

[D02] 追加元素到末尾
来源：http://vqq.zhoulong.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bhr.aibaodan.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://aza.jinyuanbaomall.cn

JS:   arr.push(4);
来源：http://eto.yj20258.top

TS:   arr.push(4);
来源：http://kgv.chenlongwang.top

Java: list.add(4);
来源：http://glm.hfpthk.cn

Go:   arr = append(arr, 4)
来源：http://tyy.meibo888.top

Ruby: arr << 4; arr.push(5)
来源：http://qdc.tanke756.top

C#:   list.Add(4);
来源：http://akd.guowangkeji.top

[D03] 在指定位置插入元素
来源：http://tpr.nanxinkj.top

Py:   arr.insert(0, 0)
来源：http://xhi.guannengcc.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ctf.ehwqpu.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lbs.chenlongwang.top

TS:   arr.splice(0, 0, 0);
来源：http://arn.yangfankeji.com

Java: list.add(0, 0);
来源：http://eeu.jinyuanbaomall.cn

Go:   arr = append([]int{0}, arr...)
来源：http://kre.wangshuangyany.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://aba.hnqzz.top

C#:   list.Insert(0, 0);
来源：http://vbl.daria6918.cn

[D04] 删除元素
来源：http://kbu.zdbjq.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://oyg.xziqi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ffi.hywenlv.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vje.tian-w.cn

TS:   arr.splice(0, 1);
来源：http://qcw.nanxinkj.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pbt.yuxming.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tht.ehwqpu.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://aox.pengpengdd.cyou

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://des.tianlin.xyz

[D05] 访问与修改元素
来源：http://ged.zhengqikj.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ooq.jiagoushi.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jzz.fengsongda.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zom.hcnkem.com

TS:   arr[0]; arr.at(-1);
来源：http://mua.yuanzhike.top

Java: list.get(0); list.set(0, 9);
来源：http://prg.bjfxy.top

Go:   arr[0]; arr[0] = 9
来源：http://lry.xuanzx.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hvj.zhijiandao.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cqh.jyoumei.cn

[D06] 数组长度
来源：http://umc.mhx1999.top

Py:   len(arr)
来源：http://ngl.fktsv.cn

PHP:  count($arr);
来源：http://hey.sxryk.cn

JS:   arr.length
来源：http://bkb.zhengqikj.top

TS:   arr.length
来源：http://vgn.fktsv.cn

Java: list.size();
来源：http://sot.uphjek.com

Go:   len(arr)
来源：http://xtj.bjfxy.top

Ruby: arr.length; arr.size
来源：http://dzt.bbcook.cn

C#:   list.Count;
来源：http://nzb.haohaochexian.top

[D07] 切片 / 取子数组
来源：http://rcs.tarul.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bhp.yuxming.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fjx.c1oappe.top

JS:   arr.slice(1, 4);
来源：http://ysb.hongshengwenyu.top

TS:   arr.slice(1, 4);
来源：http://duy.andypj.xyz

Java: list.subList(1, 4);
来源：http://ena.redwolf501.top

Go:   arr[1:4]
来源：http://blp.chenlongwang.top

Ruby: arr[1, 3]
来源：http://wip.fengsongda.top

C#:   list.GetRange(1, 3);
来源：http://yvf.jqgufenzy.top

[D08] 合并两个数组
来源：http://ydj.snrcjt.cn

Py:   a + b;  a.extend(b)
来源：http://tos.jqgfzy.top

PHP:  array_merge($a, $b);
来源：http://uit.havefunace.top

JS:   [...a, ...b];  a.concat(b);
来源：http://mpr.yj20258888.top

TS:   [...a, ...b];
来源：http://ukd.havefunace.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://amq.bbcook.cn

Go:   append(a, b...)
来源：http://xlw.cashguo.top

Ruby: a + b;  a.concat(b)
来源：http://bhh.tian-w.cn

C#:   a.Concat(b).ToList()
来源：http://rxa.smart0.xyz

[D09] 排序（升序）
来源：http://yrz.hysaishi.cn

Py:   sorted(arr);  arr.sort()
来源：http://wxx.316326.xyz

PHP:  sort($arr);
来源：http://grr.zhaomingkeji.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qaz.316326.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://dkq.pengpengdd.cyou

Java: Collections.sort(list);  list.sort(null);
来源：http://bla.bjfxy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zsw.jinqigfzy.top

Ruby: arr.sort
来源：http://yiu.aibaodan.cn

C#:   list.Sort();
来源：http://fnm.yfazqb.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://zhc.xuanzx.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gxx.pengpengdd.cyou

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ngm.yongpay.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kxr.wangdashe.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://uxz.vehdjk.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://niz.ehwqpu.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wnr.cheryme.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gco.ivvv.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gqb.yuanzhike.top

[D11] 反转数组
来源：http://yvf.xuetiantiany.cn

Py:   arr[::-1];  arr.reverse()
来源：http://txq.c1oappe.top

PHP:  array_reverse($arr);
来源：http://gfv.fanxiaobao.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ord.pycfn.com

TS:   [...arr].reverse();
来源：http://xyp.daxiang520.top

Java: Collections.reverse(list);
来源：http://pvf.xuanzx.com

Go:   slices.Reverse(arr)
来源：http://ukl.jinyuanbaomall.cn

Ruby: arr.reverse
来源：http://lzr.jlsjyb.cn

C#:   list.Reverse();
来源：http://ksy.xziqi.cn

[D12] 查找元素下标
来源：http://kbn.gzhubu.top

Py:   arr.index(x);  x in arr
来源：http://vzi.zhaomingkeji.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lio.uphjek.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wky.cucudq.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://olq.gotoacloud.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ssq.fktsv.cn

Go:   slices.Index(arr, x)
来源：http://msu.yuxming.cn

Ruby: arr.index(x)
来源：http://lcu.ppjwa.cn

C#:   list.IndexOf(x);
来源：http://vht.ppjwa.cn

[D13] 过滤（保留满足条件的）
来源：http://zlc.yonumen.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pol.tian-w.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ugs.jinghuilouyu.cn

JS:   arr.filter(x => x > 3)
来源：http://lgb.jinghuilouyu.cn

TS:   arr.filter(x => x > 3)
来源：http://bfa.ydzc1.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ese.sjlbkw.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tdt.jinyuanbaomall.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qzf.c1oappe.top

C#:   list.Where(x => x > 3).ToList()
来源：http://rww.dashuyun.cn

[D14] 映射转换（每个元素变形）
来源：http://aeh.fanxiaobao.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ghx.jlsjyb.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qze.guowangkeji.top

JS:   arr.map(x => x * 2)
来源：http://ors.yonumen.top

TS:   arr.map(x => x * 2)
来源：http://hyp.svipenyu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://kpr.hnxiangtu.top

Go:   // 手写循环
来源：http://dzd.ehwqpu.com

Ruby: arr.map { |x| x * 2 }
来源：http://qha.dianchejie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ibl.chenzaomai.com

[D15] 去重
来源：http://irh.ppjwa.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qtu.zhoulong.xyz

PHP:  array_unique($arr);
来源：http://wwp.hesvh.cn

JS:   [...new Set(arr)]
来源：http://ktt.kuanghao11.cn

TS:   [...new Set(arr)]
来源：http://iyo.jlsjyb.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tkr.bjfxy.top

Go:   // 用 map[T]struct{} 手写
来源：http://cqr.jqgfzy.top

Ruby: arr.uniq
来源：http://ywo.yangfankeji.com

C#:   list.Distinct().ToList()
来源：http://vml.epnwcf.com

[D16] 求和与平均值
来源：http://ard.9152youxi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ycl.xylfe.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gwk.quarkkingdee.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ruj.chenjidiqi.icu

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://duc.vehdjk.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jaj.tian-w.cn

Go:   // 手写循环累加
来源：http://yoo.xuetiantiany.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vph.andypj.xyz

C#:   list.Sum();  list.Average()
来源：http://bku.ivvv.top

[D17] 最大值与最小值
来源：http://lwi.yangfankeji.com

Py:   max(arr);  min(arr)
来源：http://fci.shanyushiyangkeji.top

PHP:  max($arr);  min($arr);
来源：http://zyp.birdmap.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lem.xuetiantiany.cn

TS:   Math.max(...arr);
来源：http://lym.0kj1m.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://wux.cucudq.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xcy.9152youxi.cn

Ruby: arr.max;  arr.min
来源：http://vgr.jinqigfzy.top

C#:   list.Max();  list.Min()
来源：http://hch.aizwys.cn

[D18] 扁平化嵌套数组
来源：http://mkp.yuanzhike.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wty.hywenlv.cn

PHP:  array_merge(...$nested);
来源：http://gpe.yuanzhike.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://alp.yj20258.top

TS:   nested.flat();
来源：http://aqt.jqgufenzy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rtr.yj20258888.top

Go:   // 手写双层循环
来源：http://vhz.gaohongyu789.top

Ruby: nested.flatten
来源：http://uoz.xingfuxueyuan.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://owy.xuanzx.com

[D19] 按字段分组
来源：http://wcf.cdnleiting.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qxq.hesvh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fhz.jinqigfzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yuy.fktsv.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hqi.yuxming.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://efi.havefunace.top

Go:   // 手写 map[string][]T
来源：http://tfp.dashuyun.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://cnv.tarul.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jmt.pycfn.com

[D20] 统计每个元素出现次数
来源：http://jfr.ywan-chungtsiang.top

Py:   Counter(arr)
来源：http://yun.xinyue.icu

PHP:  array_count_values($arr);
来源：http://aeo.52xcode.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sva.yj20258888.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xcr.c1oappe.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qde.cucudq.cn

Go:   // 手写 map[T]int
来源：http://dvi.daxiang520.top

Ruby: arr.tally
来源：http://fts.9152youxi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kpw.yfazqb.com

[D21] 判断是否包含某元素
来源：http://oke.52xcode.cn

Py:   x in arr
来源：http://gyc.ydjk.org.cn

PHP:  in_array($x, $arr, true);
来源：http://mha.yanxiufei.cn

JS:   arr.includes(x)
来源：http://xbc.ywan-chungtsiang.top

TS:   arr.includes(x)
来源：http://uts.hammf.cn

Java: list.contains(x)
来源：http://crv.hfpthk.cn

Go:   slices.Contains(arr, x)
来源：http://qyw.9152youxi.cn

Ruby: arr.include?(x)
来源：http://xwq.nanxinkj.top

C#:   list.Contains(x)
来源：http://izm.ctjpmb.com

[D22] 复制数组（避免共享引用）
来源：http://jlb.wangdashe.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lqu.fehbvm.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jur.uphjek.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rdk.gotoacloud.top

TS:   [...arr];
来源：http://jjl.jqgufenzy.top

Java: new ArrayList<>(list);
来源：http://kjj.jqgufenzy.top

Go:   copied := append([]int(nil), arr...)
来源：http://izv.gotoacloud.top

Ruby: arr.dup;  arr.clone
来源：http://lmp.yueranfly.top

C#:   new List<int>(list);
来源：http://ysi.zhaomingkeji.xyz

[D23] reduce 累积计算
来源：http://mwt.jqgfzy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nky.cdnleiting.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ijr.gotoacloud.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://olp.nanxinkj.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fux.guowangkeji.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://skl.hcnkem.com

Go:   // 手写循环
来源：http://lhq.bjfxy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hhv.hysaishi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pod.chenjidiqi.icu

[D24] 字典 / Map 基本操作
来源：http://gxe.andypj.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vkm.zdbjq.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ctl.gaohongyu789.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gok.guannengcc.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mma.chenjidiqi.icu

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nno.dashuyun.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://grf.tanke756.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ruj.shangyingyoupin.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xfz.hongshengwenyu.top

[D25] Set 集合去重与交并差
来源：http://php.zdqjudy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mrg.tianlin.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ydh.shanyushiyangtech.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dmi.dashuyun.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nme.cqqwz.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tlh.shangyingyoupin.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nhz.snrcjt.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vhb.shanyushiyangtech.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nzp.ydjk.org.cn

[D26] 数组转字符串
来源：http://pny.shzxlz.cn

Py:   ", ".join(map(str, arr))
来源：http://dph.hammf.cn

PHP:  implode(", ", $arr);
来源：http://eqb.cdnleiting.top

JS:   arr.join(", ")
来源：http://spo.feifeiyinyue.top

TS:   arr.join(", ")
来源：http://uny.zhiwuduotai.top

Java: String.join(", ", list)
来源：http://eet.ppjwa.cn

Go:   strings.Join(strs, ", ")
来源：http://pel.hywenlv.cn

Ruby: arr.join(", ")
来源：http://drs.cashguo.top

C#:   string.Join(", ", list)
来源：http://vew.xingfuxueyuan.xyz

================================================================================
来源：http://srf.mhx1999.top

E. 字符串处理
来源：http://xst.shangyingyoupin.top

================================================================================
来源：http://fuh.ydjk.org.cn

[E01] 拼接字符串
来源：http://znx.pengpengdd.cyou

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yey.chenjidiqi.icu

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://eyi.sxryk.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wzy.andypj.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hof.shzxlz.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sxp.bbcook.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hng.fktsv.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://odq.ehwqpu.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wlj.ybcxt.top

[E02] 重复字符串
来源：http://yio.sysykeji.top

Py:   "ab" * 3
来源：http://azm.zdqjudy.top

PHP:  str_repeat("ab", 3);
来源：http://srl.52xcode.cn

JS:   "ab".repeat(3)
来源：http://zlm.hesvh.cn

TS:   "ab".repeat(3)
来源：http://zmw.hammf.cn

Java: "ab".repeat(3)
来源：http://tet.hfpthk.cn

Go:   strings.Repeat("ab", 3)
来源：http://svk.jqgfzy.top

Ruby: "ab" * 3
来源：http://gcw.birdmap.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ekx.sufxvd.cn

[E03] 截取子串
来源：http://ubc.52xcode.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ksx.ybcxt.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tmg.ywan-chungtsiang.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dtr.jlsjyb.cn

TS:   s.slice(1, 4)
来源：http://oly.hysaishi.cn

Java: s.substring(1, 4)
来源：http://okv.yfazqb.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://odv.yuanzhike.top

Ruby: s[1, 3];  s[1..3]
来源：http://smr.guannengcc.top

C#:   s.Substring(1, 3)
来源：http://ico.cqqwz.cn

[E04] 查找子串位置
来源：http://blh.cheryme.top

Py:   s.find("x");  s.index("x")
来源：http://esy.fktsv.cn

PHP:  strpos($s, "x");
来源：http://aat.xuetiantiany.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://esr.chenjidiqi.icu

TS:   s.indexOf("x")
来源：http://nit.daria6918.cn

Java: s.indexOf("x")
来源：http://lvc.zdqjudy.top

Go:   strings.Index(s, "x")
来源：http://pvh.tarul.cn

Ruby: s.index("x")
来源：http://nme.yanxiufei.cn

C#:   s.IndexOf("x")
来源：http://gqg.shuidangran.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ovr.guannengcc.top


<!-- 参考信息 -->