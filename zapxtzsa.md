代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://pvu.fehbvm.com

Ruby: # 无重载：靠动态参数
来源：http://idg.chenzaomai.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://zhr.shangyingyoupin.top

================================================================================
来源：http://fiz.xziqi.cn

D. 数组 / 列表 / 集合
来源：http://ozg.yongpay.top

================================================================================
来源：http://tdt.hysaishi.cn

[D01] 创建数组 / 列表
来源：http://lks.gaohongyu789.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://hrp.ehwqpu.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ovr.quarkkingdee.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fii.guannengcc.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ycd.chenlongwang.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://edn.316326.xyz

Go:   arr := []int{1, 2, 3}
来源：http://ykg.vehdjk.com

Ruby: arr = [1, 2, 3]
来源：http://buw.316326.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zcy.yonumen.top

[D02] 追加元素到末尾
来源：http://bdd.mhx1999.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jdu.hammf.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vfz.yfazqb.com

JS:   arr.push(4);
来源：http://kzl.dianchejie.cn

TS:   arr.push(4);
来源：http://wgm.0kj1m.cn

Java: list.add(4);
来源：http://rtu.guowangkeji.top

Go:   arr = append(arr, 4)
来源：http://zee.fanxiaobao.xyz

Ruby: arr << 4; arr.push(5)
来源：http://ljs.fehbvm.com

C#:   list.Add(4);
来源：http://gjj.yangfankeji.com

[D03] 在指定位置插入元素
来源：http://nks.yfazqb.com

Py:   arr.insert(0, 0)
来源：http://qdt.yuxming.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dvv.nanxuanxn.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://aal.fehbvm.com

TS:   arr.splice(0, 0, 0);
来源：http://loo.jqgfzy.top

Java: list.add(0, 0);
来源：http://qyg.ybcxt.top

Go:   arr = append([]int{0}, arr...)
来源：http://oex.ybcxt.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://drm.yongpay.top

C#:   list.Insert(0, 0);
来源：http://giq.feifeiyinyue.top

[D04] 删除元素
来源：http://reh.dianchejie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zay.tian-w.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mas.yuanzhike.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yxo.hfpthk.cn

TS:   arr.splice(0, 1);
来源：http://wzx.ivvv.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cmj.yj202588.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://oxn.zycfv.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hmv.hcnkem.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wkf.sufxvd.cn

[D05] 访问与修改元素
来源：http://izf.fehbvm.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vuj.dashuyun.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fqj.haohaochexian.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qld.jinqigufen.top

TS:   arr[0]; arr.at(-1);
来源：http://lnx.yj202588.top

Java: list.get(0); list.set(0, 9);
来源：http://gcf.nanxuanxn.top

Go:   arr[0]; arr[0] = 9
来源：http://ela.9152youxi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jmu.xuetiantiany.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mil.316326.xyz

[D06] 数组长度
来源：http://zjf.daria6918.cn

Py:   len(arr)
来源：http://yjt.birdmap.top

PHP:  count($arr);
来源：http://anm.cucudq.cn

JS:   arr.length
来源：http://qxv.daria6918.cn

TS:   arr.length
来源：http://ter.mhx1999.top

Java: list.size();
来源：http://ohw.wangshuangyany.cn

Go:   len(arr)
来源：http://omc.xuetiantiany.cn

Ruby: arr.length; arr.size
来源：http://btz.sxryk.cn

C#:   list.Count;
来源：http://luu.feifeiyinyue.top

[D07] 切片 / 取子数组
来源：http://cek.bbcook.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lcw.gzhubu.top

PHP:  array_slice($arr, 1, 3);
来源：http://qvf.jinqigufen.top

JS:   arr.slice(1, 4);
来源：http://wdd.9152youxi.cn

TS:   arr.slice(1, 4);
来源：http://btn.yonumen.top

Java: list.subList(1, 4);
来源：http://qlv.tian-w.cn

Go:   arr[1:4]
来源：http://jpm.ctjpmb.com

Ruby: arr[1, 3]
来源：http://wwb.dianchejie.cn

C#:   list.GetRange(1, 3);
来源：http://gyf.yj20258888.top

[D08] 合并两个数组
来源：http://yca.fzhhl.top

Py:   a + b;  a.extend(b)
来源：http://nfk.ydzc1.top

PHP:  array_merge($a, $b);
来源：http://nwg.jqgufenzy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://vaw.cashguo.top

TS:   [...a, ...b];
来源：http://rri.aibaodan.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ybc.nanxuanxn.top

Go:   append(a, b...)
来源：http://moc.xylfe.cn

Ruby: a + b;  a.concat(b)
来源：http://afy.chenjidiqi.icu

C#:   a.Concat(b).ToList()
来源：http://ywt.jinyuanbaomall.cn

[D09] 排序（升序）
来源：http://xvw.jianghu66.top

Py:   sorted(arr);  arr.sort()
来源：http://arh.jinyuanbaomall.cn

PHP:  sort($arr);
来源：http://wsp.chenjidiqi.icu

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://umv.wangshuangyany.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://mpq.shangyingyoupin.top

Java: Collections.sort(list);  list.sort(null);
来源：http://lzo.yfazqb.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://iap.316326.xyz

Ruby: arr.sort
来源：http://hnf.iojbl.cn

C#:   list.Sort();
来源：http://ndm.hysaishi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://uuj.iojbl.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nrn.yj20258888.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wwv.havefunace.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gtt.hnqzz.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://soa.316326.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lhv.cheryme.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://iev.vehdjk.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zlt.wangshuangyany.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://azm.tanke756.top

[D11] 反转数组
来源：http://pfb.zhengqikj.top

Py:   arr[::-1];  arr.reverse()
来源：http://ttn.sufxvd.cn

PHP:  array_reverse($arr);
来源：http://iqk.smart0.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bky.quarkkingdee.top

TS:   [...arr].reverse();
来源：http://anl.sxryk.cn

Java: Collections.reverse(list);
来源：http://mhl.zycfv.cn

Go:   slices.Reverse(arr)
来源：http://hvn.mhx1999.top

Ruby: arr.reverse
来源：http://ghy.shanyushiyangkeji.top

C#:   list.Reverse();
来源：http://psz.gzhubu.top

[D12] 查找元素下标
来源：http://lez.birdmap.top

Py:   arr.index(x);  x in arr
来源：http://nfv.svipenyu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://leq.hesvh.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cbv.yuanzhike.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tsl.xylfe.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://oeq.vqdsnc.cn

Go:   slices.Index(arr, x)
来源：http://xcg.cdnleiting.top

Ruby: arr.index(x)
来源：http://fxv.guowangkeji.top

C#:   list.IndexOf(x);
来源：http://kri.wangshuangyany.cn

[D13] 过滤（保留满足条件的）
来源：http://kzj.cdnleiting.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jsb.yongpay.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pin.epnwcf.com

JS:   arr.filter(x => x > 3)
来源：http://thc.fzhhl.top

TS:   arr.filter(x => x > 3)
来源：http://hhj.birdmap.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rdb.daxiang520.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ojb.xylfe.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xzf.zdqjudy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://wyp.aibaodan.cn

[D14] 映射转换（每个元素变形）
来源：http://kle.fzhhl.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nin.gaohongyu789.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jhn.yj20258.top

JS:   arr.map(x => x * 2)
来源：http://voc.yonumen.top

TS:   arr.map(x => x * 2)
来源：http://tuc.yonumen.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://qxm.zhongyouzk.top

Go:   // 手写循环
来源：http://qll.quarkkingdee.top

Ruby: arr.map { |x| x * 2 }
来源：http://pxr.cdnleiting.top

C#:   list.Select(x => x * 2).ToList()
来源：http://kze.shanyushiyangtech.top

[D15] 去重
来源：http://pbb.ybcxt.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ruf.smart0.xyz

PHP:  array_unique($arr);
来源：http://pdq.guowangkeji.top

JS:   [...new Set(arr)]
来源：http://oev.yj20258.top

TS:   [...new Set(arr)]
来源：http://lqe.hnqzz.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rfm.pengpengdd.cyou

Go:   // 用 map[T]struct{} 手写
来源：http://mfq.shanyushiyangkeji.top

Ruby: arr.uniq
来源：http://whc.tanke756.top

C#:   list.Distinct().ToList()
来源：http://rqb.vehdjk.com

[D16] 求和与平均值
来源：http://ozp.xuetiantiany.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ula.hcnkem.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cju.cqqwz.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://eck.fehbvm.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gii.xuetiantiany.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://feg.sufxvd.cn

Go:   // 手写循环累加
来源：http://xns.yj202588.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bub.ydjk.org.cn

C#:   list.Sum();  list.Average()
来源：http://obs.uphjek.com

[D17] 最大值与最小值
来源：http://iof.yj20258.top

Py:   max(arr);  min(arr)
来源：http://dsx.yj20258888.top

PHP:  max($arr);  min($arr);
来源：http://xjr.52xcode.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nqn.dianchejie.cn

TS:   Math.max(...arr);
来源：http://fhx.gaohongyu789.top

Java: Collections.max(list);  Collections.min(list);
来源：http://fop.yongpay.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lce.mhx1999.top

Ruby: arr.max;  arr.min
来源：http://bcd.daria6918.cn

C#:   list.Max();  list.Min()
来源：http://lwv.sxryk.cn

[D18] 扁平化嵌套数组
来源：http://zmq.xziqi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wyz.shzxlz.cn

PHP:  array_merge(...$nested);
来源：http://idi.xuanzx.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wew.c1oappe.top

TS:   nested.flat();
来源：http://hpb.aizwys.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://djh.cashguo.top

Go:   // 手写双层循环
来源：http://jmb.jinqigfzy.top

Ruby: nested.flatten
来源：http://rqz.vehdjk.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://axc.yongpay.top

[D19] 按字段分组
来源：http://gzk.meibo888.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://djw.ywan-chungtsiang.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ppm.fehbvm.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wxb.gaohongyu789.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://hpo.jqgufenzy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wno.0kj1m.cn

Go:   // 手写 map[string][]T
来源：http://kwh.ybcxt.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://tup.shuidangran.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://udz.zdbjq.cn

[D20] 统计每个元素出现次数
来源：http://yqh.uphjek.com

Py:   Counter(arr)
来源：http://sjw.zhaomingkeji.xyz

PHP:  array_count_values($arr);
来源：http://whz.jlsjyb.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eys.sxryk.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kbv.jinqigufen.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rod.nwbrower.top

Go:   // 手写 map[T]int
来源：http://xwe.gotoacloud.top

Ruby: arr.tally
来源：http://hpm.yuanzhike.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://eng.fengsongda.top

[D21] 判断是否包含某元素
来源：http://teo.dashuyun.cn

Py:   x in arr
来源：http://fcr.aizwys.cn

PHP:  in_array($x, $arr, true);
来源：http://lpg.fzhhl.top

JS:   arr.includes(x)
来源：http://ulz.xuanzx.com

TS:   arr.includes(x)
来源：http://xwf.jqgfzy.top

Java: list.contains(x)
来源：http://vff.yongpay.top

Go:   slices.Contains(arr, x)
来源：http://grv.havefunace.top

Ruby: arr.include?(x)
来源：http://opn.nwbrower.top

C#:   list.Contains(x)
来源：http://rnn.hnqzz.top

[D22] 复制数组（避免共享引用）
来源：http://kja.feifeiyinyue.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://szh.tanke756.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ejj.jianghu66.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rrw.zdbjq.cn

TS:   [...arr];
来源：http://prm.gzhubu.top

Java: new ArrayList<>(list);
来源：http://xpv.bbcook.cn

Go:   copied := append([]int(nil), arr...)
来源：http://jaw.fengsongda.top

Ruby: arr.dup;  arr.clone
来源：http://syd.shanyushiyangkeji.top

C#:   new List<int>(list);
来源：http://hxy.fktsv.cn

[D23] reduce 累积计算
来源：http://fgs.cashguo.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yzc.jinyuanbaomall.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rzv.cheryme.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fzu.aizwys.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uyf.cucudq.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://nyq.shuidangran.top

Go:   // 手写循环
来源：http://dmr.sjlbkw.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pfr.316326.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ztp.fktsv.cn

[D24] 字典 / Map 基本操作
来源：http://onz.jinqigfzy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://oan.yuxming.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://def.havefunace.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qlw.cashguo.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hpl.yfazqb.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rbg.mhx1999.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hco.yfazqb.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bvv.zhijiandao.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://swb.0kj1m.cn

[D25] Set 集合去重与交并差
来源：http://ink.xuanzx.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://khd.yueranfly.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sdj.zhijiandao.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mto.hnxiangtu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xpn.svipenyu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://oew.tarul.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vqt.hysaishi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bro.yj20258.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://uxy.gogol.net.cn

[D26] 数组转字符串
来源：http://yqc.yongpay.top

Py:   ", ".join(map(str, arr))
来源：http://tou.xuetiantiany.cn

PHP:  implode(", ", $arr);
来源：http://isw.sufxvd.cn

JS:   arr.join(", ")
来源：http://non.hongshengwenyu.top

TS:   arr.join(", ")
来源：http://glf.ydzc1.top

Java: String.join(", ", list)
来源：http://tav.smart0.xyz

Go:   strings.Join(strs, ", ")
来源：http://yzf.jinyuanbaomall.cn

Ruby: arr.join(", ")
来源：http://tgp.xingfuxueyuan.xyz

C#:   string.Join(", ", list)
来源：http://pzy.svipenyu.cn

================================================================================
来源：http://tdc.birdmap.top

E. 字符串处理
来源：http://sjr.hfpthk.cn

================================================================================
来源：http://xcy.kuanghao11.cn

[E01] 拼接字符串
来源：http://xce.dashuyun.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://irl.shanyushiyangtech.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rap.gaohongyu789.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gsf.ctjpmb.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pxz.yj20258888.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ojw.zhaomingkeji.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lla.shanyushiyangtech.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ejx.yueranfly.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jwv.xuetiantiany.cn

[E02] 重复字符串
来源：http://qbx.hongshengwenyu.top

Py:   "ab" * 3
来源：http://hhs.yongpay.top

PHP:  str_repeat("ab", 3);
来源：http://ekf.iojbl.cn

JS:   "ab".repeat(3)
来源：http://wyt.xuetiantiany.cn

TS:   "ab".repeat(3)
来源：http://jcm.mhx1999.top

Java: "ab".repeat(3)
来源：http://dgq.xylfe.cn

Go:   strings.Repeat("ab", 3)
来源：http://soz.jinyuanbaomall.cn

Ruby: "ab" * 3
来源：http://jar.tian-w.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jdl.daria6918.cn

[E03] 截取子串
来源：http://kjz.cucudq.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hvd.xinyue.icu

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uyy.ydzc1.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xwp.gogol.net.cn

TS:   s.slice(1, 4)
来源：http://kcy.zhaomingkeji.xyz

Java: s.substring(1, 4)
来源：http://wym.zhiwuduotai.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qec.kuanghao11.cn

Ruby: s[1, 3];  s[1..3]
来源：http://vtc.vqdsnc.cn

C#:   s.Substring(1, 3)
来源：http://qok.shangyingyoupin.top

[E04] 查找子串位置
来源：http://zjm.ppjwa.cn

Py:   s.find("x");  s.index("x")
来源：http://bzk.ivvv.top

PHP:  strpos($s, "x");
来源：http://txj.jlsjyb.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ckt.svipenyu.cn

TS:   s.indexOf("x")
来源：http://hkk.xuanzx.com

Java: s.indexOf("x")
来源：http://eus.cashguo.top

Go:   strings.Index(s, "x")
来源：http://icr.guowangkeji.top

Ruby: s.index("x")
来源：http://cfa.cheryme.top

C#:   s.IndexOf("x")
来源：http://lem.xingfuxueyuan.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://hgx.yonumen.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ajs.hysaishi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hcn.zhiwuduotai.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hlk.dianchejie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://gsp.pycfn.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qbe.shanyushiyangtech.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cwg.zycfv.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ugy.havefunace.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://phx.cheryme.top

[E06] 替换子串
来源：http://gby.xziqi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qzx.cashguo.top

PHP:  str_replace("a", "b", $s);
来源：http://kak.guannengcc.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vks.ywan-chungtsiang.top

TS:   s.replaceAll("a", "b")
来源：http://vbr.tarul.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://umg.fengsongda.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ahx.jinqigufen.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qsf.yj20258888.top

C#:   s.Replace("a", "b")
来源：http://kok.316326.xyz

[E07] 按分隔符拆分
来源：http://lrx.dianchejie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ine.iojbl.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bde.chenlongwang.top


<!-- 参考信息 -->