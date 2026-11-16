代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qod.gogol.net.cn

[C15] 解构 / 展开参数
来源：http://own.ydzc1.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bov.chenjidiqi.icu

PHP:  [$a, $b] = $pair;
来源：http://mri.yj20258888.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rqp.jinghuilouyu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jyp.ywan-chungtsiang.top

Java: // 无解构
来源：http://bvs.xingfuxueyuan.xyz

Go:   // 无解构
来源：http://jrs.meibo888.top

Ruby: a, b = pair
来源：http://jif.wangshuangyany.cn

C#:   var (a, b) = pair;
来源：http://sxa.shzxlz.cn

[C16] 函数 / 方法重载
来源：http://tus.yvedp.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mul.cucudq.cn

PHP:  // 无重载
来源：http://ral.nwbrower.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://xvm.dashuyun.cn

TS:   // 用联合类型或重载签名声明
来源：http://anz.jqgufenzy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://rmj.hcnkem.com

Go:   // 无重载：用不同函数名
来源：http://zyq.sufxvd.cn

Ruby: # 无重载：靠动态参数
来源：http://kwv.shuidangran.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://qmy.dianchejie.cn

================================================================================
来源：http://fop.zycfv.cn

D. 数组 / 列表 / 集合
来源：http://hym.ydjk.org.cn

================================================================================
来源：http://hbr.chenzaomai.com

[D01] 创建数组 / 列表
来源：http://ccu.cashguo.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://vvd.hnxiangtu.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jde.iojbl.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pft.birdmap.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://gpu.haohaochexian.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gut.nanxuanxn.top

Go:   arr := []int{1, 2, 3}
来源：http://kos.shangyingyoupin.top

Ruby: arr = [1, 2, 3]
来源：http://cvo.shanyushiyangkeji.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bku.cheryme.top

[D02] 追加元素到末尾
来源：http://ztj.jlsjyb.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rsp.shanyushiyangtech.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ien.cashguo.top

JS:   arr.push(4);
来源：http://aam.ybcxt.top

TS:   arr.push(4);
来源：http://aoc.hywenlv.cn

Java: list.add(4);
来源：http://ijq.jinqigfzy.top

Go:   arr = append(arr, 4)
来源：http://uox.yj20258.top

Ruby: arr << 4; arr.push(5)
来源：http://rmk.yj20258888.top

C#:   list.Add(4);
来源：http://gwo.316326.xyz

[D03] 在指定位置插入元素
来源：http://dqn.dianchejie.cn

Py:   arr.insert(0, 0)
来源：http://dor.zhongyouzk.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ftb.vqdsnc.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kgg.yueranfly.top

TS:   arr.splice(0, 0, 0);
来源：http://afj.redwolf501.top

Java: list.add(0, 0);
来源：http://wqm.tianlin.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://exc.nanxuanxn.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://neg.9152youxi.cn

C#:   list.Insert(0, 0);
来源：http://gmn.meibo888.top

[D04] 删除元素
来源：http://dwn.fktsv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dyu.52xcode.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ddm.guannengcc.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vdo.gogol.net.cn

TS:   arr.splice(0, 1);
来源：http://sxn.wangdashe.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qjd.52xcode.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cid.nwbrower.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nfv.yfazqb.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kkp.ywan-chungtsiang.top

[D05] 访问与修改元素
来源：http://dxd.sweek.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dhk.pengpengdd.cyou

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kqh.vehdjk.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fzz.gzhubu.top

TS:   arr[0]; arr.at(-1);
来源：http://wjh.zhaomingkeji.xyz

Java: list.get(0); list.set(0, 9);
来源：http://kia.xinyue.icu

Go:   arr[0]; arr[0] = 9
来源：http://rex.wangshuangyany.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lct.gotoacloud.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ezw.zdqjudy.top

[D06] 数组长度
来源：http://qnh.zhijiandao.cn

Py:   len(arr)
来源：http://lvp.0kj1m.cn

PHP:  count($arr);
来源：http://toz.chenlongwang.top

JS:   arr.length
来源：http://gwk.haohaochexian.top

TS:   arr.length
来源：http://dza.yvedp.cn

Java: list.size();
来源：http://wgq.shuidangran.top

Go:   len(arr)
来源：http://hqh.dianchejie.cn

Ruby: arr.length; arr.size
来源：http://tyq.chenlongwang.top

C#:   list.Count;
来源：http://gjo.zhongyouzk.top

[D07] 切片 / 取子数组
来源：http://dvu.ivvv.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tmf.chenzaomai.com

PHP:  array_slice($arr, 1, 3);
来源：http://ebb.daxiang520.top

JS:   arr.slice(1, 4);
来源：http://jnj.yuxming.cn

TS:   arr.slice(1, 4);
来源：http://zti.jianghu66.top

Java: list.subList(1, 4);
来源：http://ftr.dianchejie.cn

Go:   arr[1:4]
来源：http://wwu.zdqjudy.top

Ruby: arr[1, 3]
来源：http://qam.zhiwuduotai.top

C#:   list.GetRange(1, 3);
来源：http://yqv.xingfuxueyuan.xyz

[D08] 合并两个数组
来源：http://ghm.zhiwuduotai.top

Py:   a + b;  a.extend(b)
来源：http://prn.yj20258888.top

PHP:  array_merge($a, $b);
来源：http://cho.shanyushiyangkeji.top

JS:   [...a, ...b];  a.concat(b);
来源：http://bsr.havefunace.top

TS:   [...a, ...b];
来源：http://bhu.chenlongwang.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ods.jinqigufen.top

Go:   append(a, b...)
来源：http://hwl.sjlbkw.cn

Ruby: a + b;  a.concat(b)
来源：http://ufm.zhixingplan.top

C#:   a.Concat(b).ToList()
来源：http://evh.xuetiantiany.cn

[D09] 排序（升序）
来源：http://qxw.chenzaomai.com

Py:   sorted(arr);  arr.sort()
来源：http://fdu.ppjwa.cn

PHP:  sort($arr);
来源：http://fwd.aibaodan.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xax.jqgufenzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://cpc.zdbjq.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xqy.ywan-chungtsiang.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ynw.xuetiantiany.cn

Ruby: arr.sort
来源：http://puq.jinqigufen.top

C#:   list.Sort();
来源：http://kdj.hywenlv.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://tqc.jyoumei.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yly.nwbrower.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://quj.ehwqpu.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dnd.yonumen.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mst.ctjpmb.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rqk.zhaomingkeji.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nlu.vqdsnc.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yuj.pycfn.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bve.jqgfzy.top

[D11] 反转数组
来源：http://ieb.tanke756.top

Py:   arr[::-1];  arr.reverse()
来源：http://mqu.sysykeji.top

PHP:  array_reverse($arr);
来源：http://xkv.zhengqikj.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wgu.316326.xyz

TS:   [...arr].reverse();
来源：http://fjr.tarul.cn

Java: Collections.reverse(list);
来源：http://zin.xinyue.icu

Go:   slices.Reverse(arr)
来源：http://xis.aizwys.cn

Ruby: arr.reverse
来源：http://rjm.sysykeji.top

C#:   list.Reverse();
来源：http://pvj.ybcxt.top

[D12] 查找元素下标
来源：http://ogh.chenlongwang.top

Py:   arr.index(x);  x in arr
来源：http://dgo.fktsv.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jlz.shzxlz.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bvj.hnxiangtu.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jod.nanxinkj.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tux.smart0.xyz

Go:   slices.Index(arr, x)
来源：http://hux.pengpengdd.cyou

Ruby: arr.index(x)
来源：http://zrh.zhijiandao.cn

C#:   list.IndexOf(x);
来源：http://uln.quarkkingdee.top

[D13] 过滤（保留满足条件的）
来源：http://lhx.yanxiufei.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cbt.wangdashe.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://syb.fengsongda.top

JS:   arr.filter(x => x > 3)
来源：http://yxo.yangfankeji.com

TS:   arr.filter(x => x > 3)
来源：http://urk.meibo888.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fmm.ppjwa.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jes.jiagoushi.top

Ruby: arr.select { |x| x > 3 }
来源：http://bbr.bbcook.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://jtg.zycfv.cn

[D14] 映射转换（每个元素变形）
来源：http://pmu.fanxiaobao.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qrx.c1oappe.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xug.uphjek.com

JS:   arr.map(x => x * 2)
来源：http://ime.hcnkem.com

TS:   arr.map(x => x * 2)
来源：http://nfv.ctjpmb.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://vbp.ydjk.org.cn

Go:   // 手写循环
来源：http://gnx.wangdashe.top

Ruby: arr.map { |x| x * 2 }
来源：http://lrj.tarul.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://dmn.yonumen.top

[D15] 去重
来源：http://wru.fanxiaobao.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wii.gzhubu.top

PHP:  array_unique($arr);
来源：http://fdg.zdbjq.cn

JS:   [...new Set(arr)]
来源：http://wjt.aizwys.cn

TS:   [...new Set(arr)]
来源：http://rnr.uphjek.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kxh.yj20258888.top

Go:   // 用 map[T]struct{} 手写
来源：http://sai.vehdjk.com

Ruby: arr.uniq
来源：http://rsm.jinqigufen.top

C#:   list.Distinct().ToList()
来源：http://hde.tian-w.cn

[D16] 求和与平均值
来源：http://efu.yangfankeji.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tpu.fehbvm.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://uyc.aibaodan.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://iym.yj20258.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://amt.hywenlv.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zhg.birdmap.top

Go:   // 手写循环累加
来源：http://xda.wangdashe.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pmb.fktsv.cn

C#:   list.Sum();  list.Average()
来源：http://rnk.yueranfly.top

[D17] 最大值与最小值
来源：http://lbr.yj202588.top

Py:   max(arr);  min(arr)
来源：http://zio.yanxiufei.cn

PHP:  max($arr);  min($arr);
来源：http://hug.aibaodan.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://guw.aibaodan.cn

TS:   Math.max(...arr);
来源：http://avz.gaohongyu789.top

Java: Collections.max(list);  Collections.min(list);
来源：http://uud.hnqzz.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qhy.xuanzx.com

Ruby: arr.max;  arr.min
来源：http://pge.chenlongwang.top

C#:   list.Max();  list.Min()
来源：http://imv.9152youxi.cn

[D18] 扁平化嵌套数组
来源：http://pdd.ybcxt.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pbe.quarkkingdee.top

PHP:  array_merge(...$nested);
来源：http://epr.epnwcf.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nns.fehbvm.com

TS:   nested.flat();
来源：http://wlj.hysaishi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://anu.shanyushiyangkeji.top

Go:   // 手写双层循环
来源：http://oox.pengpengdd.cyou

Ruby: nested.flatten
来源：http://gfx.jinyuanbaomall.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://qqp.zhoulong.xyz

[D19] 按字段分组
来源：http://sog.aizwys.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rij.epnwcf.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wra.xingfuxueyuan.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bnz.gzhubu.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://khj.ybcxt.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wwq.gzhubu.top

Go:   // 手写 map[string][]T
来源：http://mfd.zhixingplan.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://qos.yj202588.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qsc.ivvv.top

[D20] 统计每个元素出现次数
来源：http://njk.xylfe.cn

Py:   Counter(arr)
来源：http://yjt.yvedp.cn

PHP:  array_count_values($arr);
来源：http://ylt.ydjk.org.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dip.ybcxt.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ezw.xuanzx.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://eag.birdmap.top

Go:   // 手写 map[T]int
来源：http://mus.c1oappe.top

Ruby: arr.tally
来源：http://rta.gotoacloud.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://asa.fktsv.cn

[D21] 判断是否包含某元素
来源：http://cvo.birdmap.top

Py:   x in arr
来源：http://fai.epnwcf.com

PHP:  in_array($x, $arr, true);
来源：http://edr.jinqigfzy.top

JS:   arr.includes(x)
来源：http://tdz.iojbl.cn

TS:   arr.includes(x)
来源：http://hkt.mhx1999.top

Java: list.contains(x)
来源：http://hjx.hesvh.cn

Go:   slices.Contains(arr, x)
来源：http://ujw.yonumen.top

Ruby: arr.include?(x)
来源：http://dgn.shanyushiyangkeji.top

C#:   list.Contains(x)
来源：http://zom.zhaomingkeji.xyz

[D22] 复制数组（避免共享引用）
来源：http://kwt.jqgfzy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://liu.sweek.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ywg.chenlongwang.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kao.yongpay.top

TS:   [...arr];
来源：http://vdx.guowangkeji.top

Java: new ArrayList<>(list);
来源：http://mzd.hfpthk.cn

Go:   copied := append([]int(nil), arr...)
来源：http://fmu.zdbjq.cn

Ruby: arr.dup;  arr.clone
来源：http://ami.havefunace.top

C#:   new List<int>(list);
来源：http://htj.dashuyun.cn

[D23] reduce 累积计算
来源：http://wzu.shangyingyoupin.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bxj.nwbrower.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bhs.bjfxy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://inw.yvedp.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mjj.fengsongda.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://gcn.iojbl.cn

Go:   // 手写循环
来源：http://tsy.chenzaomai.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hue.pycfn.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qxo.jlsjyb.cn

[D24] 字典 / Map 基本操作
来源：http://dth.fanxiaobao.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mcy.zhengqikj.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vpd.yongpay.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kds.xylfe.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ikq.zhixingplan.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kgc.hcnkem.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ejr.yuanzhike.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gvp.daxiang520.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hwv.guannengcc.top

[D25] Set 集合去重与交并差
来源：http://qnb.dianchejie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ufb.svipenyu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jdj.ywan-chungtsiang.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jhb.xuanzx.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://llf.jinqigfzy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qay.snrcjt.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://eyc.c1oappe.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xsl.jiagoushi.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tvs.chenlongwang.top

[D26] 数组转字符串
来源：http://gtj.ehwqpu.com

Py:   ", ".join(map(str, arr))
来源：http://keb.shuidangran.top

PHP:  implode(", ", $arr);
来源：http://qxj.cqqwz.cn

JS:   arr.join(", ")
来源：http://chh.haohaochexian.top

TS:   arr.join(", ")
来源：http://aza.hnxiangtu.top

Java: String.join(", ", list)
来源：http://zen.andypj.xyz

Go:   strings.Join(strs, ", ")
来源：http://wra.daxiang520.top

Ruby: arr.join(", ")
来源：http://zcw.epnwcf.com

C#:   string.Join(", ", list)
来源：http://mmh.fanxiaobao.xyz

================================================================================
来源：http://xth.jinqigufen.top

E. 字符串处理
来源：http://zyz.xziqi.cn

================================================================================
来源：http://tjx.redwolf501.top

[E01] 拼接字符串
来源：http://tup.yvedp.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://czl.jinyuanbaomall.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jpl.cdnleiting.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xim.vqdsnc.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://meb.shanyushiyangtech.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://stv.sufxvd.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://htj.cashguo.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mkd.yanxiufei.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://boz.yj20258888.top

[E02] 重复字符串
来源：http://jst.xziqi.cn

Py:   "ab" * 3
来源：http://gjx.9152youxi.cn

PHP:  str_repeat("ab", 3);
来源：http://thi.shangyingyoupin.top

JS:   "ab".repeat(3)
来源：http://iqa.xingfuxueyuan.xyz

TS:   "ab".repeat(3)
来源：http://jjl.aibaodan.cn

Java: "ab".repeat(3)
来源：http://skc.nanxinkj.top

Go:   strings.Repeat("ab", 3)
来源：http://vrb.snrcjt.cn

Ruby: "ab" * 3
来源：http://bps.hongshengwenyu.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jxt.bbcook.cn

[E03] 截取子串
来源：http://nby.sxryk.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nmj.sxryk.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mhx.shuidangran.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lrm.cqqwz.cn

TS:   s.slice(1, 4)
来源：http://kod.jinghuilouyu.cn

Java: s.substring(1, 4)
来源：http://xxd.jinqigfzy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ubr.52xcode.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qsq.smart0.xyz

C#:   s.Substring(1, 3)
来源：http://xex.uphjek.com

[E04] 查找子串位置
来源：http://qgl.yonumen.top

Py:   s.find("x");  s.index("x")
来源：http://lvo.c1oappe.top

PHP:  strpos($s, "x");
来源：http://dli.jinghuilouyu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ybt.yangfankeji.com

TS:   s.indexOf("x")
来源：http://bop.svipenyu.cn

Java: s.indexOf("x")
来源：http://sei.tian-w.cn

Go:   strings.Index(s, "x")
来源：http://nvn.zhijiandao.cn

Ruby: s.index("x")
来源：http://dvr.fktsv.cn

C#:   s.IndexOf("x")
来源：http://biv.ydzc1.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://xph.zdqjudy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://noz.ehwqpu.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qjl.iojbl.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ndl.ctjpmb.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://mzo.jqgufenzy.top


<!-- 参考信息 -->