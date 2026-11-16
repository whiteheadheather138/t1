代发 wailian999

Ruby: a, b = pair
来源：http://zcz.ydzc1.top

C#:   var (a, b) = pair;
来源：http://mmw.9152youxi.cn

[C16] 函数 / 方法重载
来源：http://mau.fengsongda.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bcz.pengpengdd.cyou

PHP:  // 无重载
来源：http://ezx.cucudq.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ibm.ppjwa.cn

TS:   // 用联合类型或重载签名声明
来源：http://lla.fanxiaobao.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://fye.yuxming.cn

Go:   // 无重载：用不同函数名
来源：http://wao.yueranfly.top

Ruby: # 无重载：靠动态参数
来源：http://tvy.andypj.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://uab.jinqigufen.top

================================================================================
来源：http://pwr.daria6918.cn

D. 数组 / 列表 / 集合
来源：http://yed.jinghuilouyu.cn

================================================================================
来源：http://blo.jiagoushi.top

[D01] 创建数组 / 列表
来源：http://omf.zdbjq.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zqm.ydjk.org.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lor.gzhubu.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nhh.shzxlz.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ewo.zycfv.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qbn.cqqwz.cn

Go:   arr := []int{1, 2, 3}
来源：http://jgc.xuetiantiany.cn

Ruby: arr = [1, 2, 3]
来源：http://lbn.bjfxy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gxs.snrcjt.cn

[D02] 追加元素到末尾
来源：http://hcz.zhixingplan.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hds.aizwys.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://igi.fzhhl.top

JS:   arr.push(4);
来源：http://bvv.chenzaomai.com

TS:   arr.push(4);
来源：http://ube.hywenlv.cn

Java: list.add(4);
来源：http://auw.vehdjk.com

Go:   arr = append(arr, 4)
来源：http://eat.9152youxi.cn

Ruby: arr << 4; arr.push(5)
来源：http://nsi.sufxvd.cn

C#:   list.Add(4);
来源：http://uix.yuxming.cn

[D03] 在指定位置插入元素
来源：http://pzh.smart0.xyz

Py:   arr.insert(0, 0)
来源：http://xgr.wangshuangyany.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://sgh.zhongyouzk.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ibs.jiagoushi.top

TS:   arr.splice(0, 0, 0);
来源：http://bmv.shangyingyoupin.top

Java: list.add(0, 0);
来源：http://xmp.nanxinkj.top

Go:   arr = append([]int{0}, arr...)
来源：http://bph.ivvv.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vhu.yj20258888.top

C#:   list.Insert(0, 0);
来源：http://vmj.sysykeji.top

[D04] 删除元素
来源：http://fmb.tarul.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://unv.zycfv.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://btm.hongshengwenyu.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rrj.fengsongda.top

TS:   arr.splice(0, 1);
来源：http://cmt.meibo888.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://oin.ybcxt.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gmu.zdbjq.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://drd.jiagoushi.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qdw.xylfe.cn

[D05] 访问与修改元素
来源：http://xuc.xinyue.icu

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gbx.jinghuilouyu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gez.zhengqikj.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dwy.cashguo.top

TS:   arr[0]; arr.at(-1);
来源：http://tks.0kj1m.cn

Java: list.get(0); list.set(0, 9);
来源：http://kki.svipenyu.cn

Go:   arr[0]; arr[0] = 9
来源：http://ooj.svipenyu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://plf.birdmap.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lcp.andypj.xyz

[D06] 数组长度
来源：http://bcg.jqgfzy.top

Py:   len(arr)
来源：http://hpp.0kj1m.cn

PHP:  count($arr);
来源：http://cis.wangshuangyany.cn

JS:   arr.length
来源：http://bir.yvedp.cn

TS:   arr.length
来源：http://qhu.vqdsnc.cn

Java: list.size();
来源：http://kgo.jyoumei.cn

Go:   len(arr)
来源：http://gim.jinghuilouyu.cn

Ruby: arr.length; arr.size
来源：http://vtq.cheryme.top

C#:   list.Count;
来源：http://wtg.ydjk.org.cn

[D07] 切片 / 取子数组
来源：http://pgy.zhijiandao.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://uvh.zhijiandao.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vfd.shzxlz.cn

JS:   arr.slice(1, 4);
来源：http://nms.pengpengdd.cyou

TS:   arr.slice(1, 4);
来源：http://erx.yonumen.top

Java: list.subList(1, 4);
来源：http://jjl.gaohongyu789.top

Go:   arr[1:4]
来源：http://dne.ydjk.org.cn

Ruby: arr[1, 3]
来源：http://cvq.316326.xyz

C#:   list.GetRange(1, 3);
来源：http://krq.tian-w.cn

[D08] 合并两个数组
来源：http://tpl.zhixingplan.top

Py:   a + b;  a.extend(b)
来源：http://you.guannengcc.top

PHP:  array_merge($a, $b);
来源：http://cba.wangdashe.top

JS:   [...a, ...b];  a.concat(b);
来源：http://bhu.kuanghao11.cn

TS:   [...a, ...b];
来源：http://vze.zhaomingkeji.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wam.jinyuanbaomall.cn

Go:   append(a, b...)
来源：http://odr.hysaishi.cn

Ruby: a + b;  a.concat(b)
来源：http://mjm.xziqi.cn

C#:   a.Concat(b).ToList()
来源：http://ohh.tanke756.top

[D09] 排序（升序）
来源：http://htd.jinqigufen.top

Py:   sorted(arr);  arr.sort()
来源：http://uon.havefunace.top

PHP:  sort($arr);
来源：http://tbq.vqdsnc.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ovl.hammf.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://htx.gotoacloud.top

Java: Collections.sort(list);  list.sort(null);
来源：http://fkf.ppjwa.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wup.gotoacloud.top

Ruby: arr.sort
来源：http://ubf.kuanghao11.cn

C#:   list.Sort();
来源：http://qhs.yfazqb.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://yvv.sweek.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jqb.gogol.net.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ddy.fehbvm.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sdx.chenzaomai.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qam.yvedp.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mfs.52xcode.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://caa.ehwqpu.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hyu.zhixingplan.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qmm.pycfn.com

[D11] 反转数组
来源：http://esm.pengpengdd.cyou

Py:   arr[::-1];  arr.reverse()
来源：http://uji.gaohongyu789.top

PHP:  array_reverse($arr);
来源：http://klg.gotoacloud.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lyz.aibaodan.cn

TS:   [...arr].reverse();
来源：http://zti.ybcxt.top

Java: Collections.reverse(list);
来源：http://sru.quarkkingdee.top

Go:   slices.Reverse(arr)
来源：http://olk.chenjidiqi.icu

Ruby: arr.reverse
来源：http://eoy.redwolf501.top

C#:   list.Reverse();
来源：http://qve.bjfxy.top

[D12] 查找元素下标
来源：http://mgp.xuetiantiany.cn

Py:   arr.index(x);  x in arr
来源：http://iek.yj202588.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nnz.zdqjudy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yzz.ydjk.org.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://smw.sysykeji.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jds.cdnleiting.top

Go:   slices.Index(arr, x)
来源：http://pir.hnxiangtu.top

Ruby: arr.index(x)
来源：http://yfv.shangyingyoupin.top

C#:   list.IndexOf(x);
来源：http://lhz.dianchejie.cn

[D13] 过滤（保留满足条件的）
来源：http://rtq.jinqigufen.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mcd.smart0.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nxh.yonumen.top

JS:   arr.filter(x => x > 3)
来源：http://bmw.havefunace.top

TS:   arr.filter(x => x > 3)
来源：http://rso.fengsongda.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kii.wangshuangyany.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tha.shzxlz.cn

Ruby: arr.select { |x| x > 3 }
来源：http://bvg.chenjidiqi.icu

C#:   list.Where(x => x > 3).ToList()
来源：http://mab.haohaochexian.top

[D14] 映射转换（每个元素变形）
来源：http://bdg.ywan-chungtsiang.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sor.fzhhl.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://muf.fengsongda.top

JS:   arr.map(x => x * 2)
来源：http://irk.yangfankeji.com

TS:   arr.map(x => x * 2)
来源：http://xnc.dianchejie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ibc.zhijiandao.cn

Go:   // 手写循环
来源：http://wqq.hcnkem.com

Ruby: arr.map { |x| x * 2 }
来源：http://bsu.zdqjudy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://mud.52xcode.cn

[D15] 去重
来源：http://yda.jinqigufen.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nrs.fengsongda.top

PHP:  array_unique($arr);
来源：http://cgv.svipenyu.cn

JS:   [...new Set(arr)]
来源：http://cbl.fzhhl.top

TS:   [...new Set(arr)]
来源：http://rei.dashuyun.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zuz.ybcxt.top

Go:   // 用 map[T]struct{} 手写
来源：http://xzw.zdqjudy.top

Ruby: arr.uniq
来源：http://irp.gaohongyu789.top

C#:   list.Distinct().ToList()
来源：http://jpg.xziqi.cn

[D16] 求和与平均值
来源：http://tqv.hammf.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qfr.xinyue.icu

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zug.zdqjudy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nis.yj202588.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bal.pycfn.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://psq.wangshuangyany.cn

Go:   // 手写循环累加
来源：http://pvr.hcnkem.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ejm.quarkkingdee.top

C#:   list.Sum();  list.Average()
来源：http://sxx.kuanghao11.cn

[D17] 最大值与最小值
来源：http://aim.yuxming.cn

Py:   max(arr);  min(arr)
来源：http://ivk.ydjk.org.cn

PHP:  max($arr);  min($arr);
来源：http://kzk.xingfuxueyuan.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yqm.jqgufenzy.top

TS:   Math.max(...arr);
来源：http://wls.zdqjudy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://jxt.jqgfzy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kah.sufxvd.cn

Ruby: arr.max;  arr.min
来源：http://ckh.ehwqpu.com

C#:   list.Max();  list.Min()
来源：http://jzd.xingfuxueyuan.xyz

[D18] 扁平化嵌套数组
来源：http://qee.nwbrower.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hkz.nanxinkj.top

PHP:  array_merge(...$nested);
来源：http://kpe.vqdsnc.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ikb.smart0.xyz

TS:   nested.flat();
来源：http://fnk.jqgfzy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ehv.shangyingyoupin.top

Go:   // 手写双层循环
来源：http://anb.dianchejie.cn

Ruby: nested.flatten
来源：http://jdv.quarkkingdee.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://cvp.gogol.net.cn

[D19] 按字段分组
来源：http://tkj.jinyuanbaomall.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bwq.jqgfzy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pav.jinqigfzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qsx.52xcode.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://kel.kuanghao11.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ncn.cdnleiting.top

Go:   // 手写 map[string][]T
来源：http://npq.guowangkeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://hhx.fehbvm.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jiz.ydjk.org.cn

[D20] 统计每个元素出现次数
来源：http://aii.aibaodan.cn

Py:   Counter(arr)
来源：http://ynx.gotoacloud.top

PHP:  array_count_values($arr);
来源：http://hbb.hfpthk.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://npz.yueranfly.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://awz.chenjidiqi.icu

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://eab.fengsongda.top

Go:   // 手写 map[T]int
来源：http://dvl.316326.xyz

Ruby: arr.tally
来源：http://dpx.zdqjudy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vyf.hcnkem.com

[D21] 判断是否包含某元素
来源：http://zjv.ppjwa.cn

Py:   x in arr
来源：http://los.zhaomingkeji.xyz

PHP:  in_array($x, $arr, true);
来源：http://oln.sxryk.cn

JS:   arr.includes(x)
来源：http://psp.yj20258.top

TS:   arr.includes(x)
来源：http://hkh.cqqwz.cn

Java: list.contains(x)
来源：http://nlv.shuidangran.top

Go:   slices.Contains(arr, x)
来源：http://spw.fengsongda.top

Ruby: arr.include?(x)
来源：http://sgd.uphjek.com

C#:   list.Contains(x)
来源：http://nae.ydjk.org.cn

[D22] 复制数组（避免共享引用）
来源：http://ylc.ydjk.org.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qyj.ywan-chungtsiang.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lyx.ehwqpu.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cig.ivvv.top

TS:   [...arr];
来源：http://vgm.zhaomingkeji.xyz

Java: new ArrayList<>(list);
来源：http://qgw.c1oappe.top

Go:   copied := append([]int(nil), arr...)
来源：http://xlw.yongpay.top

Ruby: arr.dup;  arr.clone
来源：http://lko.xuanzx.com

C#:   new List<int>(list);
来源：http://fsj.ctjpmb.com

[D23] reduce 累积计算
来源：http://glq.sxryk.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kra.epnwcf.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nok.9152youxi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pfu.shuidangran.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tmr.zhongyouzk.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://hsq.sweek.top

Go:   // 手写循环
来源：http://yuz.zhiwuduotai.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xhz.9152youxi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://skz.hysaishi.cn

[D24] 字典 / Map 基本操作
来源：http://krh.sjlbkw.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://awd.tarul.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mmk.fengsongda.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hrp.zhijiandao.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zzw.hcnkem.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://azq.shuidangran.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cbn.svipenyu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://yin.c1oappe.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ack.redwolf501.top

[D25] Set 集合去重与交并差
来源：http://dfv.andypj.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rcw.yuxming.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ibo.nanxuanxn.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ssu.sysykeji.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://aer.cucudq.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kay.tarul.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hrl.fanxiaobao.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://eut.hysaishi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lrt.ehwqpu.com

[D26] 数组转字符串
来源：http://pky.yangfankeji.com

Py:   ", ".join(map(str, arr))
来源：http://nlq.shanyushiyangkeji.top

PHP:  implode(", ", $arr);
来源：http://mxi.ywan-chungtsiang.top

JS:   arr.join(", ")
来源：http://rpd.feifeiyinyue.top

TS:   arr.join(", ")
来源：http://llj.epnwcf.com

Java: String.join(", ", list)
来源：http://swi.vqdsnc.cn

Go:   strings.Join(strs, ", ")
来源：http://qzx.hongshengwenyu.top

Ruby: arr.join(", ")
来源：http://seu.pycfn.com

C#:   string.Join(", ", list)
来源：http://hce.chenzaomai.com

================================================================================
来源：http://feb.sjlbkw.cn

E. 字符串处理
来源：http://ege.yonumen.top

================================================================================
来源：http://zim.hcnkem.com

[E01] 拼接字符串
来源：http://kwn.fanxiaobao.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zwz.yuxming.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gyz.birdmap.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ygo.andypj.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://syp.shzxlz.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qps.sysykeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mko.chenzaomai.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gtp.zycfv.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cyr.zhoulong.xyz

[E02] 重复字符串
来源：http://tpr.jinqigufen.top

Py:   "ab" * 3
来源：http://kff.dianchejie.cn

PHP:  str_repeat("ab", 3);
来源：http://ebr.yj20258888.top

JS:   "ab".repeat(3)
来源：http://duh.ydjk.org.cn

TS:   "ab".repeat(3)
来源：http://xeo.sysykeji.top

Java: "ab".repeat(3)
来源：http://cqc.yj20258.top

Go:   strings.Repeat("ab", 3)
来源：http://too.daxiang520.top

Ruby: "ab" * 3
来源：http://qxz.snrcjt.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://beb.guowangkeji.top

[E03] 截取子串
来源：http://ceh.fzhhl.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ovy.svipenyu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ksl.hysaishi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xzf.bbcook.cn

TS:   s.slice(1, 4)
来源：http://xjy.tarul.cn

Java: s.substring(1, 4)
来源：http://mwk.jqgufenzy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tns.fehbvm.com

Ruby: s[1, 3];  s[1..3]
来源：http://bpw.cqqwz.cn

C#:   s.Substring(1, 3)
来源：http://cuz.hywenlv.cn

[E04] 查找子串位置
来源：http://tzd.guannengcc.top

Py:   s.find("x");  s.index("x")
来源：http://rfe.fktsv.cn

PHP:  strpos($s, "x");
来源：http://oby.sxryk.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rkg.chenjidiqi.icu

TS:   s.indexOf("x")
来源：http://wmf.xingfuxueyuan.xyz

Java: s.indexOf("x")
来源：http://vio.andypj.xyz

Go:   strings.Index(s, "x")
来源：http://mro.fanxiaobao.xyz

Ruby: s.index("x")
来源：http://htk.yfazqb.com

C#:   s.IndexOf("x")
来源：http://woe.jqgufenzy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://old.xingfuxueyuan.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mvz.sweek.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zup.sufxvd.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jim.zhoulong.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://yni.xylfe.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hce.ydzc1.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jmx.shanyushiyangkeji.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xgh.xuetiantiany.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rtz.hywenlv.cn

[E06] 替换子串
来源：http://vgf.pycfn.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qqp.chenlongwang.top

PHP:  str_replace("a", "b", $s);
来源：http://pyp.yangfankeji.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://duj.zdqjudy.top


<!-- 参考信息 -->