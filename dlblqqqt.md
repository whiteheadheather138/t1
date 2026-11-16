代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rea.haohaochexian.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fhx.zhijiandao.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pdd.smart0.xyz

Ruby: # 无泛型
来源：http://pea.gzhubu.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zxd.tianlin.xyz

[C15] 解构 / 展开参数
来源：http://mmg.ydjk.org.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jjc.sjlbkw.cn

PHP:  [$a, $b] = $pair;
来源：http://bhm.xziqi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rhc.yj20258.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dhh.wangdashe.top

Java: // 无解构
来源：http://mdb.yj20258.top

Go:   // 无解构
来源：http://xlg.vehdjk.com

Ruby: a, b = pair
来源：http://pgo.zhijiandao.cn

C#:   var (a, b) = pair;
来源：http://enk.xuanzx.com

[C16] 函数 / 方法重载
来源：http://nyu.zdbjq.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wch.bjfxy.top

PHP:  // 无重载
来源：http://kja.yueranfly.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://mdu.yuanzhike.top

TS:   // 用联合类型或重载签名声明
来源：http://gnd.aizwys.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://cll.zhongyouzk.top

Go:   // 无重载：用不同函数名
来源：http://uzh.zycfv.cn

Ruby: # 无重载：靠动态参数
来源：http://oge.xuanzx.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://qzj.dianchejie.cn

================================================================================
来源：http://cof.yonumen.top

D. 数组 / 列表 / 集合
来源：http://zbn.hnqzz.top

================================================================================
来源：http://jfk.zhiwuduotai.top

[D01] 创建数组 / 列表
来源：http://rjq.hongshengwenyu.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ijq.zhongyouzk.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tle.shanyushiyangtech.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pxw.ydjk.org.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fsm.cashguo.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hhm.ppjwa.cn

Go:   arr := []int{1, 2, 3}
来源：http://nan.yonumen.top

Ruby: arr = [1, 2, 3]
来源：http://cpg.tian-w.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fqz.svipenyu.cn

[D02] 追加元素到末尾
来源：http://upx.0kj1m.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dly.yueranfly.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://erz.dianchejie.cn

JS:   arr.push(4);
来源：http://dzf.sjlbkw.cn

TS:   arr.push(4);
来源：http://lni.guowangkeji.top

Java: list.add(4);
来源：http://ics.feifeiyinyue.top

Go:   arr = append(arr, 4)
来源：http://scx.aibaodan.cn

Ruby: arr << 4; arr.push(5)
来源：http://vaw.yj202588.top

C#:   list.Add(4);
来源：http://fuw.epnwcf.com

[D03] 在指定位置插入元素
来源：http://bmi.hcnkem.com

Py:   arr.insert(0, 0)
来源：http://dut.xziqi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rlj.yueranfly.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sre.yanxiufei.cn

TS:   arr.splice(0, 0, 0);
来源：http://ypm.mhx1999.top

Java: list.add(0, 0);
来源：http://iqh.wangdashe.top

Go:   arr = append([]int{0}, arr...)
来源：http://ctm.jinghuilouyu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://klq.smart0.xyz

C#:   list.Insert(0, 0);
来源：http://pfh.hcnkem.com

[D04] 删除元素
来源：http://uua.zhiwuduotai.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://obq.yj202588.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wsu.ctjpmb.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hqq.pengpengdd.cyou

TS:   arr.splice(0, 1);
来源：http://mdi.zhongyouzk.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://aji.hnqzz.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qaa.shuidangran.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gey.yuxming.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yrd.sxryk.cn

[D05] 访问与修改元素
来源：http://aia.daria6918.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ber.vehdjk.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lyk.zycfv.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tei.epnwcf.com

TS:   arr[0]; arr.at(-1);
来源：http://svd.jiagoushi.top

Java: list.get(0); list.set(0, 9);
来源：http://ura.aizwys.cn

Go:   arr[0]; arr[0] = 9
来源：http://akk.svipenyu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zbo.gotoacloud.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dog.jyoumei.cn

[D06] 数组长度
来源：http://dee.pycfn.com

Py:   len(arr)
来源：http://auj.yj20258.top

PHP:  count($arr);
来源：http://vrf.shangyingyoupin.top

JS:   arr.length
来源：http://dig.wangshuangyany.cn

TS:   arr.length
来源：http://kef.chenzaomai.com

Java: list.size();
来源：http://kre.hongshengwenyu.top

Go:   len(arr)
来源：http://ljl.0kj1m.cn

Ruby: arr.length; arr.size
来源：http://eak.yuanzhike.top

C#:   list.Count;
来源：http://tff.yonumen.top

[D07] 切片 / 取子数组
来源：http://dxv.yfazqb.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lug.redwolf501.top

PHP:  array_slice($arr, 1, 3);
来源：http://jnw.tianlin.xyz

JS:   arr.slice(1, 4);
来源：http://ewp.shanyushiyangkeji.top

TS:   arr.slice(1, 4);
来源：http://zta.vehdjk.com

Java: list.subList(1, 4);
来源：http://bnn.hysaishi.cn

Go:   arr[1:4]
来源：http://txl.fktsv.cn

Ruby: arr[1, 3]
来源：http://jaf.jinyuanbaomall.cn

C#:   list.GetRange(1, 3);
来源：http://vbo.redwolf501.top

[D08] 合并两个数组
来源：http://cxc.epnwcf.com

Py:   a + b;  a.extend(b)
来源：http://owu.jqgufenzy.top

PHP:  array_merge($a, $b);
来源：http://wjb.aibaodan.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ntg.ybcxt.top

TS:   [...a, ...b];
来源：http://cwx.fehbvm.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://emu.zycfv.cn

Go:   append(a, b...)
来源：http://gtu.c1oappe.top

Ruby: a + b;  a.concat(b)
来源：http://aee.yvedp.cn

C#:   a.Concat(b).ToList()
来源：http://kkw.cashguo.top

[D09] 排序（升序）
来源：http://azv.zhengqikj.top

Py:   sorted(arr);  arr.sort()
来源：http://kbm.nanxinkj.top

PHP:  sort($arr);
来源：http://phq.yueranfly.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wge.hammf.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://yun.zhengqikj.top

Java: Collections.sort(list);  list.sort(null);
来源：http://jqu.jinqigufen.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://eri.ehwqpu.com

Ruby: arr.sort
来源：http://azw.hcnkem.com

C#:   list.Sort();
来源：http://yjr.zdbjq.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://goh.fengsongda.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ffx.sjlbkw.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oxr.sufxvd.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pjh.jqgufenzy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fpk.yj20258.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bsv.ivvv.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hxy.hfpthk.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jve.sweek.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gab.shangyingyoupin.top

[D11] 反转数组
来源：http://ihw.xingfuxueyuan.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://wvv.ppjwa.cn

PHP:  array_reverse($arr);
来源：http://lwz.xingfuxueyuan.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nkz.zhoulong.xyz

TS:   [...arr].reverse();
来源：http://hbe.birdmap.top

Java: Collections.reverse(list);
来源：http://mur.epnwcf.com

Go:   slices.Reverse(arr)
来源：http://yfs.wangdashe.top

Ruby: arr.reverse
来源：http://mat.smart0.xyz

C#:   list.Reverse();
来源：http://wun.zhoulong.xyz

[D12] 查找元素下标
来源：http://ths.jinyuanbaomall.cn

Py:   arr.index(x);  x in arr
来源：http://kep.nanxinkj.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xpo.c1oappe.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://auw.yj202588.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vmu.fehbvm.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ttm.pycfn.com

Go:   slices.Index(arr, x)
来源：http://jgb.ivvv.top

Ruby: arr.index(x)
来源：http://ahh.chenjidiqi.icu

C#:   list.IndexOf(x);
来源：http://thf.cqqwz.cn

[D13] 过滤（保留满足条件的）
来源：http://bbf.wangdashe.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kzh.guannengcc.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hbb.andypj.xyz

JS:   arr.filter(x => x > 3)
来源：http://vcc.jianghu66.top

TS:   arr.filter(x => x > 3)
来源：http://gxu.ydzc1.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hmb.dashuyun.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cur.zycfv.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wfj.zhengqikj.top

C#:   list.Where(x => x > 3).ToList()
来源：http://xcm.yj20258.top

[D14] 映射转换（每个元素变形）
来源：http://xgc.daxiang520.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mxo.smart0.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dqf.0kj1m.cn

JS:   arr.map(x => x * 2)
来源：http://wau.ctjpmb.com

TS:   arr.map(x => x * 2)
来源：http://xds.jlsjyb.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://jmj.cashguo.top

Go:   // 手写循环
来源：http://mqw.ywan-chungtsiang.top

Ruby: arr.map { |x| x * 2 }
来源：http://rlv.zdbjq.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://vte.ppjwa.cn

[D15] 去重
来源：http://bkx.xuetiantiany.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://euh.jinyuanbaomall.cn

PHP:  array_unique($arr);
来源：http://gbz.ydjk.org.cn

JS:   [...new Set(arr)]
来源：http://rfr.gaohongyu789.top

TS:   [...new Set(arr)]
来源：http://vtp.smart0.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://meu.kuanghao11.cn

Go:   // 用 map[T]struct{} 手写
来源：http://yqu.cashguo.top

Ruby: arr.uniq
来源：http://xkk.svipenyu.cn

C#:   list.Distinct().ToList()
来源：http://mmm.zhaomingkeji.xyz

[D16] 求和与平均值
来源：http://ghq.birdmap.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://spx.yj20258.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wwr.aibaodan.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fmz.aibaodan.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mlt.sufxvd.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://muh.hcnkem.com

Go:   // 手写循环累加
来源：http://cju.yanxiufei.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rln.cqqwz.cn

C#:   list.Sum();  list.Average()
来源：http://cxy.cucudq.cn

[D17] 最大值与最小值
来源：http://qyk.c1oappe.top

Py:   max(arr);  min(arr)
来源：http://vzy.yuanzhike.top

PHP:  max($arr);  min($arr);
来源：http://zkf.zhijiandao.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xor.smart0.xyz

TS:   Math.max(...arr);
来源：http://aft.316326.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://wac.9152youxi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ggk.wangdashe.top

Ruby: arr.max;  arr.min
来源：http://mat.52xcode.cn

C#:   list.Max();  list.Min()
来源：http://cjf.ywan-chungtsiang.top

[D18] 扁平化嵌套数组
来源：http://hjz.yuanzhike.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xmz.hywenlv.cn

PHP:  array_merge(...$nested);
来源：http://vwb.hammf.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://owm.ywan-chungtsiang.top

TS:   nested.flat();
来源：http://aoy.jqgfzy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hxa.shanyushiyangkeji.top

Go:   // 手写双层循环
来源：http://nwr.gzhubu.top

Ruby: nested.flatten
来源：http://fof.sxryk.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zpf.hfpthk.cn

[D19] 按字段分组
来源：http://fdz.epnwcf.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mmb.zhijiandao.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ehs.xuanzx.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fqx.bjfxy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://iil.mhx1999.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zkk.fengsongda.top

Go:   // 手写 map[string][]T
来源：http://lou.smart0.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://tqz.zhengqikj.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kep.xingfuxueyuan.xyz

[D20] 统计每个元素出现次数
来源：http://qaq.jinyuanbaomall.cn

Py:   Counter(arr)
来源：http://aet.zycfv.cn

PHP:  array_count_values($arr);
来源：http://xla.tarul.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tzy.yj20258.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://aec.cdnleiting.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://obz.hnxiangtu.top

Go:   // 手写 map[T]int
来源：http://xrd.jqgfzy.top

Ruby: arr.tally
来源：http://lsl.shzxlz.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zja.fanxiaobao.xyz

[D21] 判断是否包含某元素
来源：http://pww.cdnleiting.top

Py:   x in arr
来源：http://icb.xuetiantiany.cn

PHP:  in_array($x, $arr, true);
来源：http://yjb.shanyushiyangkeji.top

JS:   arr.includes(x)
来源：http://xvq.havefunace.top

TS:   arr.includes(x)
来源：http://tnq.daria6918.cn

Java: list.contains(x)
来源：http://khn.zhiwuduotai.top

Go:   slices.Contains(arr, x)
来源：http://uki.kuanghao11.cn

Ruby: arr.include?(x)
来源：http://bod.jiagoushi.top

C#:   list.Contains(x)
来源：http://tnk.birdmap.top

[D22] 复制数组（避免共享引用）
来源：http://qtv.redwolf501.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://iip.ydjk.org.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gbl.ppjwa.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rrp.tanke756.top

TS:   [...arr];
来源：http://nvk.hammf.cn

Java: new ArrayList<>(list);
来源：http://ewj.jqgufenzy.top

Go:   copied := append([]int(nil), arr...)
来源：http://sni.havefunace.top

Ruby: arr.dup;  arr.clone
来源：http://zzi.tianlin.xyz

C#:   new List<int>(list);
来源：http://wob.chenzaomai.com

[D23] reduce 累积计算
来源：http://nsm.nwbrower.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://eoc.tian-w.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tya.dashuyun.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cui.0kj1m.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ary.sysykeji.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://apu.gogol.net.cn

Go:   // 手写循环
来源：http://tbw.zhixingplan.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://omb.hesvh.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rkc.uphjek.com

[D24] 字典 / Map 基本操作
来源：http://qnp.redwolf501.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bia.xylfe.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://czj.smart0.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mki.cheryme.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fyi.shangyingyoupin.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hxv.c1oappe.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://soe.c1oappe.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://epy.ppjwa.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://eeo.zhijiandao.cn

[D25] Set 集合去重与交并差
来源：http://qrr.jyoumei.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lgh.vehdjk.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hpa.pengpengdd.cyou

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mnh.pycfn.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jju.cheryme.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dih.ybcxt.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://efb.hywenlv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fnw.hcnkem.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rmo.jinghuilouyu.cn

[D26] 数组转字符串
来源：http://qlj.sufxvd.cn

Py:   ", ".join(map(str, arr))
来源：http://tsv.chenjidiqi.icu

PHP:  implode(", ", $arr);
来源：http://lmv.yj20258888.top

JS:   arr.join(", ")
来源：http://gsu.jlsjyb.cn

TS:   arr.join(", ")
来源：http://dby.xuanzx.com

Java: String.join(", ", list)
来源：http://xhj.fzhhl.top

Go:   strings.Join(strs, ", ")
来源：http://koe.iojbl.cn

Ruby: arr.join(", ")
来源：http://jko.jqgfzy.top

C#:   string.Join(", ", list)
来源：http://hsa.cucudq.cn

================================================================================
来源：http://niw.nanxuanxn.top

E. 字符串处理
来源：http://ubz.tianlin.xyz

================================================================================
来源：http://dpb.yongpay.top

[E01] 拼接字符串
来源：http://qjw.yonumen.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wwk.tanke756.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vyd.jyoumei.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dee.gogol.net.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yqv.chenzaomai.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vbe.haohaochexian.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uun.jianghu66.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ihu.svipenyu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://obt.tian-w.cn

[E02] 重复字符串
来源：http://mzc.yongpay.top

Py:   "ab" * 3
来源：http://uan.nanxinkj.top

PHP:  str_repeat("ab", 3);
来源：http://jla.feifeiyinyue.top

JS:   "ab".repeat(3)
来源：http://qvy.fanxiaobao.xyz

TS:   "ab".repeat(3)
来源：http://enh.birdmap.top

Java: "ab".repeat(3)
来源：http://oxj.yangfankeji.com

Go:   strings.Repeat("ab", 3)
来源：http://sbk.cdnleiting.top

Ruby: "ab" * 3
来源：http://vuv.ehwqpu.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kdm.redwolf501.top

[E03] 截取子串
来源：http://ykb.jyoumei.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hgv.snrcjt.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vuc.sxryk.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jea.hywenlv.cn

TS:   s.slice(1, 4)
来源：http://hja.dashuyun.cn

Java: s.substring(1, 4)
来源：http://ryk.jlsjyb.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jqe.316326.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://rjd.zycfv.cn

C#:   s.Substring(1, 3)
来源：http://bnq.sufxvd.cn

[E04] 查找子串位置
来源：http://avd.haohaochexian.top

Py:   s.find("x");  s.index("x")
来源：http://rhc.shangyingyoupin.top

PHP:  strpos($s, "x");
来源：http://vdf.fktsv.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ajr.fehbvm.com

TS:   s.indexOf("x")
来源：http://ins.ydzc1.top

Java: s.indexOf("x")
来源：http://vyy.cdnleiting.top

Go:   strings.Index(s, "x")
来源：http://gzu.zhongyouzk.top

Ruby: s.index("x")
来源：http://xfq.chenjidiqi.icu

C#:   s.IndexOf("x")
来源：http://pfs.zycfv.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://lxg.fengsongda.top


<!-- 参考信息 -->