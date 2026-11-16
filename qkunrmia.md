代发 wailian999

Ruby: a, b = pair
来源：http://wpf.shanyushiyangkeji.top

C#:   var (a, b) = pair;
来源：http://xfc.gogol.net.cn

[C16] 函数 / 方法重载
来源：http://cqu.xuanzx.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gvp.hesvh.cn

PHP:  // 无重载
来源：http://awr.hongshengwenyu.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://qtv.meibo888.top

TS:   // 用联合类型或重载签名声明
来源：http://prr.epnwcf.com

Java: void f(int a) {}  void f(String a) {}
来源：http://xig.guannengcc.top

Go:   // 无重载：用不同函数名
来源：http://isz.zhijiandao.cn

Ruby: # 无重载：靠动态参数
来源：http://wun.jinqigfzy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ktv.cucudq.cn

================================================================================
来源：http://fkd.daxiang520.top

D. 数组 / 列表 / 集合
来源：http://qcy.shanyushiyangkeji.top

================================================================================
来源：http://oqa.jqgufenzy.top

[D01] 创建数组 / 列表
来源：http://fvw.tarul.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://rii.jinqigfzy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kwi.yanxiufei.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xkf.dianchejie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fhu.zhengqikj.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bvg.gaohongyu789.top

Go:   arr := []int{1, 2, 3}
来源：http://qfy.nwbrower.top

Ruby: arr = [1, 2, 3]
来源：http://uwf.gotoacloud.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://isd.andypj.xyz

[D02] 追加元素到末尾
来源：http://cqb.tanke756.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gtl.ctjpmb.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xss.tanke756.top

JS:   arr.push(4);
来源：http://pwz.xuanzx.com

TS:   arr.push(4);
来源：http://nhu.316326.xyz

Java: list.add(4);
来源：http://rdi.hammf.cn

Go:   arr = append(arr, 4)
来源：http://oiy.vehdjk.com

Ruby: arr << 4; arr.push(5)
来源：http://kha.shanyushiyangkeji.top

C#:   list.Add(4);
来源：http://ftt.birdmap.top

[D03] 在指定位置插入元素
来源：http://kls.shzxlz.cn

Py:   arr.insert(0, 0)
来源：http://bkm.yvedp.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vjm.cucudq.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cpu.yueranfly.top

TS:   arr.splice(0, 0, 0);
来源：http://dce.yanxiufei.cn

Java: list.add(0, 0);
来源：http://ubv.ppjwa.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fkg.fengsongda.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lyy.yanxiufei.cn

C#:   list.Insert(0, 0);
来源：http://kfc.tanke756.top

[D04] 删除元素
来源：http://itt.jinghuilouyu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tse.pengpengdd.cyou

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vfl.aizwys.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rao.ppjwa.cn

TS:   arr.splice(0, 1);
来源：http://xbf.jinghuilouyu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://axr.zdqjudy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fre.zhixingplan.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://omy.sysykeji.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dlm.tian-w.cn

[D05] 访问与修改元素
来源：http://rqs.shuidangran.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xiu.quarkkingdee.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ykj.shanyushiyangkeji.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mnr.yfazqb.com

TS:   arr[0]; arr.at(-1);
来源：http://ztt.jinqigfzy.top

Java: list.get(0); list.set(0, 9);
来源：http://phy.ehwqpu.com

Go:   arr[0]; arr[0] = 9
来源：http://iif.pycfn.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xom.jlsjyb.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cng.nwbrower.top

[D06] 数组长度
来源：http://jgb.hywenlv.cn

Py:   len(arr)
来源：http://iqa.zdqjudy.top

PHP:  count($arr);
来源：http://umo.zdbjq.cn

JS:   arr.length
来源：http://lxz.zhengqikj.top

TS:   arr.length
来源：http://leq.hesvh.cn

Java: list.size();
来源：http://eiw.jyoumei.cn

Go:   len(arr)
来源：http://xhe.hesvh.cn

Ruby: arr.length; arr.size
来源：http://adi.tian-w.cn

C#:   list.Count;
来源：http://juk.xinyue.icu

[D07] 切片 / 取子数组
来源：http://wqc.daria6918.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://axq.ydjk.org.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ypd.yj202588.top

JS:   arr.slice(1, 4);
来源：http://vcb.jinghuilouyu.cn

TS:   arr.slice(1, 4);
来源：http://pzb.andypj.xyz

Java: list.subList(1, 4);
来源：http://nbx.fzhhl.top

Go:   arr[1:4]
来源：http://zve.guannengcc.top

Ruby: arr[1, 3]
来源：http://dtc.gotoacloud.top

C#:   list.GetRange(1, 3);
来源：http://yeu.xinyue.icu

[D08] 合并两个数组
来源：http://kbu.svipenyu.cn

Py:   a + b;  a.extend(b)
来源：http://fjq.snrcjt.cn

PHP:  array_merge($a, $b);
来源：http://ozi.feifeiyinyue.top

JS:   [...a, ...b];  a.concat(b);
来源：http://exx.yongpay.top

TS:   [...a, ...b];
来源：http://tgl.jinghuilouyu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qei.zhixingplan.top

Go:   append(a, b...)
来源：http://hls.yonumen.top

Ruby: a + b;  a.concat(b)
来源：http://ziz.quarkkingdee.top

C#:   a.Concat(b).ToList()
来源：http://pfy.yj20258888.top

[D09] 排序（升序）
来源：http://hly.chenjidiqi.icu

Py:   sorted(arr);  arr.sort()
来源：http://sda.wangdashe.top

PHP:  sort($arr);
来源：http://rox.gaohongyu789.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://syv.shzxlz.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gpz.epnwcf.com

Java: Collections.sort(list);  list.sort(null);
来源：http://qbc.tian-w.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pxe.redwolf501.top

Ruby: arr.sort
来源：http://shl.0kj1m.cn

C#:   list.Sort();
来源：http://dqw.iojbl.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ahj.zhaomingkeji.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jai.yfazqb.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bke.aibaodan.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://osm.chenlongwang.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wcq.xziqi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://oox.zycfv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uev.ehwqpu.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://acs.xingfuxueyuan.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://omt.smart0.xyz

[D11] 反转数组
来源：http://hvu.smart0.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://slq.redwolf501.top

PHP:  array_reverse($arr);
来源：http://pla.svipenyu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rtn.svipenyu.cn

TS:   [...arr].reverse();
来源：http://pqb.hfpthk.cn

Java: Collections.reverse(list);
来源：http://zis.jinqigfzy.top

Go:   slices.Reverse(arr)
来源：http://zjk.yuanzhike.top

Ruby: arr.reverse
来源：http://ucn.yj202588.top

C#:   list.Reverse();
来源：http://pfa.guannengcc.top

[D12] 查找元素下标
来源：http://stf.hywenlv.cn

Py:   arr.index(x);  x in arr
来源：http://jip.pycfn.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pya.jinqigfzy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bye.bbcook.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xes.iojbl.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gjv.ehwqpu.com

Go:   slices.Index(arr, x)
来源：http://ujo.zycfv.cn

Ruby: arr.index(x)
来源：http://tak.zhongyouzk.top

C#:   list.IndexOf(x);
来源：http://rkb.ywan-chungtsiang.top

[D13] 过滤（保留满足条件的）
来源：http://vaf.jinqigfzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wte.meibo888.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qlg.iojbl.cn

JS:   arr.filter(x => x > 3)
来源：http://jia.yongpay.top

TS:   arr.filter(x => x > 3)
来源：http://qsa.tarul.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ams.redwolf501.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kyr.wangdashe.top

Ruby: arr.select { |x| x > 3 }
来源：http://rzu.cucudq.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://zvr.birdmap.top

[D14] 映射转换（每个元素变形）
来源：http://zdu.uphjek.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://owl.0kj1m.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://olu.jinqigufen.top

JS:   arr.map(x => x * 2)
来源：http://krt.vqdsnc.cn

TS:   arr.map(x => x * 2)
来源：http://fcu.xuanzx.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://hav.pengpengdd.cyou

Go:   // 手写循环
来源：http://zxb.aibaodan.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ysp.sweek.top

C#:   list.Select(x => x * 2).ToList()
来源：http://tes.birdmap.top

[D15] 去重
来源：http://czf.cashguo.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fjv.cucudq.cn

PHP:  array_unique($arr);
来源：http://fth.yuxming.cn

JS:   [...new Set(arr)]
来源：http://tda.ybcxt.top

TS:   [...new Set(arr)]
来源：http://eqt.gaohongyu789.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cwa.ywan-chungtsiang.top

Go:   // 用 map[T]struct{} 手写
来源：http://nsi.chenzaomai.com

Ruby: arr.uniq
来源：http://con.bbcook.cn

C#:   list.Distinct().ToList()
来源：http://yrp.epnwcf.com

[D16] 求和与平均值
来源：http://sdh.vqdsnc.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://glx.gaohongyu789.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yvx.fzhhl.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qnq.zdbjq.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sxt.gogol.net.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fdq.daxiang520.top

Go:   // 手写循环累加
来源：http://vbj.gaohongyu789.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mdt.tian-w.cn

C#:   list.Sum();  list.Average()
来源：http://nju.ybcxt.top

[D17] 最大值与最小值
来源：http://yyv.epnwcf.com

Py:   max(arr);  min(arr)
来源：http://yvn.ivvv.top

PHP:  max($arr);  min($arr);
来源：http://vlc.vqdsnc.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://eni.yanxiufei.cn

TS:   Math.max(...arr);
来源：http://xra.zhixingplan.top

Java: Collections.max(list);  Collections.min(list);
来源：http://oqb.cucudq.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vcz.c1oappe.top

Ruby: arr.max;  arr.min
来源：http://gti.andypj.xyz

C#:   list.Max();  list.Min()
来源：http://hhp.aizwys.cn

[D18] 扁平化嵌套数组
来源：http://kmw.hammf.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mlx.shuidangran.top

PHP:  array_merge(...$nested);
来源：http://bcu.yuxming.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vng.ehwqpu.com

TS:   nested.flat();
来源：http://qgw.gogol.net.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jxo.redwolf501.top

Go:   // 手写双层循环
来源：http://bqx.ctjpmb.com

Ruby: nested.flatten
来源：http://txb.wangshuangyany.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://rxk.ybcxt.top

[D19] 按字段分组
来源：http://jsx.hcnkem.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mdk.fzhhl.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ppn.shanyushiyangtech.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jya.dashuyun.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://kdf.uphjek.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pbf.uphjek.com

Go:   // 手写 map[string][]T
来源：http://jtz.aibaodan.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://cot.jinyuanbaomall.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fvp.fktsv.cn

[D20] 统计每个元素出现次数
来源：http://pop.cheryme.top

Py:   Counter(arr)
来源：http://ngy.guowangkeji.top

PHP:  array_count_values($arr);
来源：http://qhz.yonumen.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jwd.316326.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bfi.xylfe.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yzl.havefunace.top

Go:   // 手写 map[T]int
来源：http://ipp.redwolf501.top

Ruby: arr.tally
来源：http://evo.hongshengwenyu.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://iqs.daria6918.cn

[D21] 判断是否包含某元素
来源：http://woe.aizwys.cn

Py:   x in arr
来源：http://xqe.zhoulong.xyz

PHP:  in_array($x, $arr, true);
来源：http://soh.sxryk.cn

JS:   arr.includes(x)
来源：http://lmh.haohaochexian.top

TS:   arr.includes(x)
来源：http://opy.yonumen.top

Java: list.contains(x)
来源：http://yea.sufxvd.cn

Go:   slices.Contains(arr, x)
来源：http://ufw.ywan-chungtsiang.top

Ruby: arr.include?(x)
来源：http://wzk.yuxming.cn

C#:   list.Contains(x)
来源：http://qey.shzxlz.cn

[D22] 复制数组（避免共享引用）
来源：http://oqy.xingfuxueyuan.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qcc.tian-w.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xpw.zdbjq.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ujc.epnwcf.com

TS:   [...arr];
来源：http://ksj.nanxuanxn.top

Java: new ArrayList<>(list);
来源：http://rkk.bjfxy.top

Go:   copied := append([]int(nil), arr...)
来源：http://alc.cqqwz.cn

Ruby: arr.dup;  arr.clone
来源：http://aii.yueranfly.top

C#:   new List<int>(list);
来源：http://svm.haohaochexian.top

[D23] reduce 累积计算
来源：http://wwe.smart0.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://uzw.fengsongda.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tmy.snrcjt.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fbd.zycfv.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nkh.ppjwa.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://kfa.yuanzhike.top

Go:   // 手写循环
来源：http://vjd.gotoacloud.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jnt.jinqigufen.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uve.haohaochexian.top

[D24] 字典 / Map 基本操作
来源：http://bds.fehbvm.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ssa.zhaomingkeji.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bju.316326.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://oly.yonumen.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ddx.zdqjudy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tzg.ywan-chungtsiang.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hcc.redwolf501.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ole.nanxinkj.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://exh.zdqjudy.top

[D25] Set 集合去重与交并差
来源：http://ruo.shzxlz.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ohd.jinqigfzy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vyg.zhaomingkeji.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tln.daxiang520.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kgq.jinyuanbaomall.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qwy.tanke756.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zxg.cucudq.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jvx.jyoumei.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://isn.jinyuanbaomall.cn

[D26] 数组转字符串
来源：http://iry.haohaochexian.top

Py:   ", ".join(map(str, arr))
来源：http://ppg.ivvv.top

PHP:  implode(", ", $arr);
来源：http://zor.ydjk.org.cn

JS:   arr.join(", ")
来源：http://ylj.aizwys.cn

TS:   arr.join(", ")
来源：http://bsv.dianchejie.cn

Java: String.join(", ", list)
来源：http://tlm.sweek.top

Go:   strings.Join(strs, ", ")
来源：http://cbf.zhiwuduotai.top

Ruby: arr.join(", ")
来源：http://oos.cheryme.top

C#:   string.Join(", ", list)
来源：http://nkh.jyoumei.cn

================================================================================
来源：http://clg.hnqzz.top

E. 字符串处理
来源：http://uqo.jinghuilouyu.cn

================================================================================
来源：http://dfs.zhoulong.xyz

[E01] 拼接字符串
来源：http://elw.tianlin.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rks.hesvh.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qms.gzhubu.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nnm.hysaishi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ndf.aizwys.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://veh.xuetiantiany.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cvw.hnqzz.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qqp.hysaishi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://iov.ydjk.org.cn

[E02] 重复字符串
来源：http://uhg.iojbl.cn

Py:   "ab" * 3
来源：http://bab.ehwqpu.com

PHP:  str_repeat("ab", 3);
来源：http://aqj.sxryk.cn

JS:   "ab".repeat(3)
来源：http://pvn.daria6918.cn

TS:   "ab".repeat(3)
来源：http://hoh.hcnkem.com

Java: "ab".repeat(3)
来源：http://hxs.pengpengdd.cyou

Go:   strings.Repeat("ab", 3)
来源：http://wpx.jinghuilouyu.cn

Ruby: "ab" * 3
来源：http://alc.fzhhl.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nbs.yvedp.cn

[E03] 截取子串
来源：http://org.sjlbkw.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://izh.ywan-chungtsiang.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hxq.jqgfzy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zvm.ppjwa.cn

TS:   s.slice(1, 4)
来源：http://nhw.cdnleiting.top

Java: s.substring(1, 4)
来源：http://hun.chenjidiqi.icu

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tnq.zhongyouzk.top

Ruby: s[1, 3];  s[1..3]
来源：http://ogg.fzhhl.top

C#:   s.Substring(1, 3)
来源：http://php.sxryk.cn

[E04] 查找子串位置
来源：http://rtv.zhixingplan.top

Py:   s.find("x");  s.index("x")
来源：http://jmu.xylfe.cn

PHP:  strpos($s, "x");
来源：http://ift.shangyingyoupin.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hmn.yangfankeji.com

TS:   s.indexOf("x")
来源：http://dsl.redwolf501.top

Java: s.indexOf("x")
来源：http://dtb.kuanghao11.cn

Go:   strings.Index(s, "x")
来源：http://qmy.vehdjk.com

Ruby: s.index("x")
来源：http://bmo.ydzc1.top

C#:   s.IndexOf("x")
来源：http://baz.xingfuxueyuan.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://aao.cucudq.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gbi.zhiwuduotai.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vrd.fanxiaobao.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hds.bbcook.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://nrp.guowangkeji.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mdm.xingfuxueyuan.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bpq.ctjpmb.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dll.zhaomingkeji.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://urw.daria6918.cn

[E06] 替换子串
来源：http://pah.xingfuxueyuan.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xvr.andypj.xyz

PHP:  str_replace("a", "b", $s);
来源：http://jgv.hammf.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ioy.yj202588.top


<!-- 参考信息 -->