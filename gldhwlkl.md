代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://adr.gogol.net.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qzm.yuxming.cn

Java: // 无解构
来源：http://oue.svipenyu.cn

Go:   // 无解构
来源：http://wgv.jianghu66.top

Ruby: a, b = pair
来源：http://qck.jinyuanbaomall.cn

C#:   var (a, b) = pair;
来源：http://gxx.tianlin.xyz

[C16] 函数 / 方法重载
来源：http://deu.nanxuanxn.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ooo.yanxiufei.cn

PHP:  // 无重载
来源：http://ypm.daria6918.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://cht.yfazqb.com

TS:   // 用联合类型或重载签名声明
来源：http://bej.tianlin.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://uvd.hesvh.cn

Go:   // 无重载：用不同函数名
来源：http://vpj.xziqi.cn

Ruby: # 无重载：靠动态参数
来源：http://rau.kuanghao11.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://krr.ywan-chungtsiang.top

================================================================================
来源：http://dfv.c1oappe.top

D. 数组 / 列表 / 集合
来源：http://umi.fktsv.cn

================================================================================
来源：http://fxm.ydjk.org.cn

[D01] 创建数组 / 列表
来源：http://snn.hfpthk.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mpo.daxiang520.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wyz.hywenlv.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://svb.chenzaomai.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://vnh.xziqi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kwt.shanyushiyangkeji.top

Go:   arr := []int{1, 2, 3}
来源：http://rex.hammf.cn

Ruby: arr = [1, 2, 3]
来源：http://efd.jqgufenzy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kep.0kj1m.cn

[D02] 追加元素到末尾
来源：http://oao.fehbvm.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://izr.cdnleiting.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://riy.feifeiyinyue.top

JS:   arr.push(4);
来源：http://wrn.cqqwz.cn

TS:   arr.push(4);
来源：http://ikl.jyoumei.cn

Java: list.add(4);
来源：http://wnn.cqqwz.cn

Go:   arr = append(arr, 4)
来源：http://xtz.dashuyun.cn

Ruby: arr << 4; arr.push(5)
来源：http://ctc.ppjwa.cn

C#:   list.Add(4);
来源：http://cny.daxiang520.top

[D03] 在指定位置插入元素
来源：http://uaw.aibaodan.cn

Py:   arr.insert(0, 0)
来源：http://aqr.jqgfzy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://har.yuanzhike.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kgr.cashguo.top

TS:   arr.splice(0, 0, 0);
来源：http://jxh.iojbl.cn

Java: list.add(0, 0);
来源：http://jbq.shanyushiyangtech.top

Go:   arr = append([]int{0}, arr...)
来源：http://slt.hongshengwenyu.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lwy.zhijiandao.cn

C#:   list.Insert(0, 0);
来源：http://lfa.yvedp.cn

[D04] 删除元素
来源：http://urc.ivvv.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wve.jiagoushi.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ymb.hcnkem.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jub.wangshuangyany.cn

TS:   arr.splice(0, 1);
来源：http://fkn.xuetiantiany.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gpl.zhaomingkeji.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tky.vehdjk.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://uoq.ydjk.org.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nve.nwbrower.top

[D05] 访问与修改元素
来源：http://ikv.shanyushiyangtech.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lin.xziqi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cra.shangyingyoupin.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cpo.iojbl.cn

TS:   arr[0]; arr.at(-1);
来源：http://ahh.fengsongda.top

Java: list.get(0); list.set(0, 9);
来源：http://tey.zhengqikj.top

Go:   arr[0]; arr[0] = 9
来源：http://ohm.shzxlz.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wsa.dashuyun.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wma.smart0.xyz

[D06] 数组长度
来源：http://iig.zhijiandao.cn

Py:   len(arr)
来源：http://jtd.snrcjt.cn

PHP:  count($arr);
来源：http://qzh.c1oappe.top

JS:   arr.length
来源：http://emq.cdnleiting.top

TS:   arr.length
来源：http://tpu.ehwqpu.com

Java: list.size();
来源：http://wew.cdnleiting.top

Go:   len(arr)
来源：http://flr.jiagoushi.top

Ruby: arr.length; arr.size
来源：http://cbu.zhaomingkeji.xyz

C#:   list.Count;
来源：http://iog.chenlongwang.top

[D07] 切片 / 取子数组
来源：http://cgc.birdmap.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nsr.ywan-chungtsiang.top

PHP:  array_slice($arr, 1, 3);
来源：http://ryw.svipenyu.cn

JS:   arr.slice(1, 4);
来源：http://fiw.iojbl.cn

TS:   arr.slice(1, 4);
来源：http://ccu.gotoacloud.top

Java: list.subList(1, 4);
来源：http://mmn.yfazqb.com

Go:   arr[1:4]
来源：http://ejj.kuanghao11.cn

Ruby: arr[1, 3]
来源：http://pzb.svipenyu.cn

C#:   list.GetRange(1, 3);
来源：http://yvv.birdmap.top

[D08] 合并两个数组
来源：http://gdp.tanke756.top

Py:   a + b;  a.extend(b)
来源：http://qlu.zhaomingkeji.xyz

PHP:  array_merge($a, $b);
来源：http://uqn.tarul.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gsc.zdbjq.cn

TS:   [...a, ...b];
来源：http://idc.ivvv.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ajf.yanxiufei.cn

Go:   append(a, b...)
来源：http://gnb.vehdjk.com

Ruby: a + b;  a.concat(b)
来源：http://got.ybcxt.top

C#:   a.Concat(b).ToList()
来源：http://nae.shanyushiyangtech.top

[D09] 排序（升序）
来源：http://xyx.nanxinkj.top

Py:   sorted(arr);  arr.sort()
来源：http://jie.cashguo.top

PHP:  sort($arr);
来源：http://cil.hnqzz.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://axx.sysykeji.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ucq.hysaishi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mrb.nanxuanxn.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xyg.zhongyouzk.top

Ruby: arr.sort
来源：http://gpe.shanyushiyangkeji.top

C#:   list.Sort();
来源：http://tfc.0kj1m.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://rlg.cashguo.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vnn.smart0.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wer.sxryk.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://awa.sxryk.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hov.jianghu66.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://njy.shanyushiyangtech.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lka.cucudq.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nkj.haohaochexian.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xae.sweek.top

[D11] 反转数组
来源：http://pvu.andypj.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://yar.tarul.cn

PHP:  array_reverse($arr);
来源：http://dck.gotoacloud.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kos.zhixingplan.top

TS:   [...arr].reverse();
来源：http://ija.hywenlv.cn

Java: Collections.reverse(list);
来源：http://gwj.cqqwz.cn

Go:   slices.Reverse(arr)
来源：http://hgk.yuanzhike.top

Ruby: arr.reverse
来源：http://mhp.shuidangran.top

C#:   list.Reverse();
来源：http://qkp.vehdjk.com

[D12] 查找元素下标
来源：http://kwp.fehbvm.com

Py:   arr.index(x);  x in arr
来源：http://ybc.xingfuxueyuan.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uvk.nwbrower.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cax.shzxlz.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lbo.tian-w.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kji.jlsjyb.cn

Go:   slices.Index(arr, x)
来源：http://syx.kuanghao11.cn

Ruby: arr.index(x)
来源：http://dve.chenzaomai.com

C#:   list.IndexOf(x);
来源：http://yco.zhixingplan.top

[D13] 过滤（保留满足条件的）
来源：http://cec.chenlongwang.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ykr.9152youxi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tkm.hammf.cn

JS:   arr.filter(x => x > 3)
来源：http://yne.gzhubu.top

TS:   arr.filter(x => x > 3)
来源：http://fol.zhijiandao.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qiz.shuidangran.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wcj.ppjwa.cn

Ruby: arr.select { |x| x > 3 }
来源：http://owd.xingfuxueyuan.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://lbu.gaohongyu789.top

[D14] 映射转换（每个元素变形）
来源：http://dra.yvedp.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mmr.tianlin.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vfy.guowangkeji.top

JS:   arr.map(x => x * 2)
来源：http://lra.hesvh.cn

TS:   arr.map(x => x * 2)
来源：http://rou.hongshengwenyu.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://twj.wangdashe.top

Go:   // 手写循环
来源：http://ylu.redwolf501.top

Ruby: arr.map { |x| x * 2 }
来源：http://wch.jinqigufen.top

C#:   list.Select(x => x * 2).ToList()
来源：http://npt.guannengcc.top

[D15] 去重
来源：http://dld.zhixingplan.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nkq.sysykeji.top

PHP:  array_unique($arr);
来源：http://emf.zhiwuduotai.top

JS:   [...new Set(arr)]
来源：http://whv.9152youxi.cn

TS:   [...new Set(arr)]
来源：http://xaj.shzxlz.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vvs.vqdsnc.cn

Go:   // 用 map[T]struct{} 手写
来源：http://mlh.ydzc1.top

Ruby: arr.uniq
来源：http://wyt.cheryme.top

C#:   list.Distinct().ToList()
来源：http://ztm.andypj.xyz

[D16] 求和与平均值
来源：http://rte.hnqzz.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wld.jqgfzy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://emg.dianchejie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gpp.hcnkem.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zyz.bjfxy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vqb.c1oappe.top

Go:   // 手写循环累加
来源：http://hxb.ehwqpu.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://eqp.sysykeji.top

C#:   list.Sum();  list.Average()
来源：http://tnq.yongpay.top

[D17] 最大值与最小值
来源：http://kle.dianchejie.cn

Py:   max(arr);  min(arr)
来源：http://tjl.yongpay.top

PHP:  max($arr);  min($arr);
来源：http://mwj.ehwqpu.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cus.hnxiangtu.top

TS:   Math.max(...arr);
来源：http://lpy.hongshengwenyu.top

Java: Collections.max(list);  Collections.min(list);
来源：http://vdx.meibo888.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qoj.xingfuxueyuan.xyz

Ruby: arr.max;  arr.min
来源：http://sma.sxryk.cn

C#:   list.Max();  list.Min()
来源：http://yvq.xinyue.icu

[D18] 扁平化嵌套数组
来源：http://ent.zhijiandao.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nch.dianchejie.cn

PHP:  array_merge(...$nested);
来源：http://wxt.zhongyouzk.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ycd.yj20258888.top

TS:   nested.flat();
来源：http://vku.yvedp.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qet.jqgufenzy.top

Go:   // 手写双层循环
来源：http://qzv.vqdsnc.cn

Ruby: nested.flatten
来源：http://bna.shuidangran.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://oyu.yongpay.top

[D19] 按字段分组
来源：http://xtj.fengsongda.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pqv.zycfv.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bsa.sjlbkw.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xhn.redwolf501.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://udv.jqgufenzy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://uoj.xziqi.cn

Go:   // 手写 map[string][]T
来源：http://kmb.ywan-chungtsiang.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://tzz.cqqwz.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tek.kuanghao11.cn

[D20] 统计每个元素出现次数
来源：http://ktt.xuetiantiany.cn

Py:   Counter(arr)
来源：http://zvw.ctjpmb.com

PHP:  array_count_values($arr);
来源：http://xis.ydzc1.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ccm.yj20258888.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xsw.zhongyouzk.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dzw.yuxming.cn

Go:   // 手写 map[T]int
来源：http://upg.uphjek.com

Ruby: arr.tally
来源：http://tjm.zhoulong.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wsg.dashuyun.cn

[D21] 判断是否包含某元素
来源：http://zgw.316326.xyz

Py:   x in arr
来源：http://vof.daria6918.cn

PHP:  in_array($x, $arr, true);
来源：http://kjq.ydzc1.top

JS:   arr.includes(x)
来源：http://wbh.yj20258.top

TS:   arr.includes(x)
来源：http://tvn.316326.xyz

Java: list.contains(x)
来源：http://nmx.zhongyouzk.top

Go:   slices.Contains(arr, x)
来源：http://xdt.jinqigufen.top

Ruby: arr.include?(x)
来源：http://ydf.sxryk.cn

C#:   list.Contains(x)
来源：http://ifs.9152youxi.cn

[D22] 复制数组（避免共享引用）
来源：http://juq.jinqigufen.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dfh.daria6918.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dqh.xuanzx.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://byu.52xcode.cn

TS:   [...arr];
来源：http://ric.iojbl.cn

Java: new ArrayList<>(list);
来源：http://myh.9152youxi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://jeo.fehbvm.com

Ruby: arr.dup;  arr.clone
来源：http://crf.iojbl.cn

C#:   new List<int>(list);
来源：http://zmv.fehbvm.com

[D23] reduce 累积计算
来源：http://lzv.zdqjudy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xax.shangyingyoupin.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mnx.zdqjudy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mpi.xingfuxueyuan.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cqu.cqqwz.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://kku.xuanzx.com

Go:   // 手写循环
来源：http://iar.9152youxi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bax.52xcode.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wij.chenjidiqi.icu

[D24] 字典 / Map 基本操作
来源：http://mym.jlsjyb.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ber.chenzaomai.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bzy.c1oappe.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ptv.shuidangran.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wud.yonumen.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://msn.yueranfly.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gqt.guannengcc.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xks.fanxiaobao.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cvy.52xcode.cn

[D25] Set 集合去重与交并差
来源：http://qup.jlsjyb.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wkp.zdqjudy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dib.zhongyouzk.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://you.epnwcf.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dns.pengpengdd.cyou

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bte.hongshengwenyu.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rap.cqqwz.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://eqk.aizwys.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qkb.jianghu66.top

[D26] 数组转字符串
来源：http://etx.yonumen.top

Py:   ", ".join(map(str, arr))
来源：http://gcn.vehdjk.com

PHP:  implode(", ", $arr);
来源：http://nad.hnqzz.top

JS:   arr.join(", ")
来源：http://wcm.cucudq.cn

TS:   arr.join(", ")
来源：http://bji.zycfv.cn

Java: String.join(", ", list)
来源：http://azj.mhx1999.top

Go:   strings.Join(strs, ", ")
来源：http://qbf.fzhhl.top

Ruby: arr.join(", ")
来源：http://vbh.yueranfly.top

C#:   string.Join(", ", list)
来源：http://gpj.gogol.net.cn

================================================================================
来源：http://nqy.daxiang520.top

E. 字符串处理
来源：http://bho.yj20258888.top

================================================================================
来源：http://qmb.svipenyu.cn

[E01] 拼接字符串
来源：http://tgs.iojbl.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tnv.ydzc1.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bux.zhaomingkeji.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vvw.xingfuxueyuan.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wgs.havefunace.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pgl.aibaodan.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bjd.tian-w.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dnd.zhoulong.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jlz.andypj.xyz

[E02] 重复字符串
来源：http://kpe.sweek.top

Py:   "ab" * 3
来源：http://jct.9152youxi.cn

PHP:  str_repeat("ab", 3);
来源：http://gql.jinyuanbaomall.cn

JS:   "ab".repeat(3)
来源：http://dxv.jyoumei.cn

TS:   "ab".repeat(3)
来源：http://mye.c1oappe.top

Java: "ab".repeat(3)
来源：http://ppb.jianghu66.top

Go:   strings.Repeat("ab", 3)
来源：http://rsu.shanyushiyangkeji.top

Ruby: "ab" * 3
来源：http://zos.hongshengwenyu.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://crl.gzhubu.top

[E03] 截取子串
来源：http://ptx.fengsongda.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ibf.jinghuilouyu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hqv.ydjk.org.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://opt.mhx1999.top

TS:   s.slice(1, 4)
来源：http://yss.guannengcc.top

Java: s.substring(1, 4)
来源：http://dtj.haohaochexian.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ptk.xingfuxueyuan.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://tss.yj202588.top

C#:   s.Substring(1, 3)
来源：http://oim.sufxvd.cn

[E04] 查找子串位置
来源：http://glr.zhongyouzk.top

Py:   s.find("x");  s.index("x")
来源：http://xme.gogol.net.cn

PHP:  strpos($s, "x");
来源：http://zej.zhijiandao.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://twe.yonumen.top

TS:   s.indexOf("x")
来源：http://ykg.nwbrower.top

Java: s.indexOf("x")
来源：http://zhy.dashuyun.cn

Go:   strings.Index(s, "x")
来源：http://nsc.jiagoushi.top

Ruby: s.index("x")
来源：http://riy.jqgufenzy.top

C#:   s.IndexOf("x")
来源：http://xak.yueranfly.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://niz.meibo888.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jyn.guowangkeji.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zfj.fktsv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://aaz.gaohongyu789.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://mes.yvedp.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dgs.52xcode.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fcl.iojbl.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://flf.smart0.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qbp.tarul.cn


<!-- 参考信息 -->