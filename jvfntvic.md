代发 wailian999

D. 数组 / 列表 / 集合
来源：http://hdw.mhx1999.top

================================================================================
来源：http://cpl.ybcxt.top

[D01] 创建数组 / 列表
来源：http://unm.ppjwa.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jss.jinqigfzy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kqf.haohaochexian.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://huz.ybcxt.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ipz.fehbvm.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pmd.uphjek.com

Go:   arr := []int{1, 2, 3}
来源：http://skm.jqgufenzy.top

Ruby: arr = [1, 2, 3]
来源：http://mpf.smart0.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gee.jqgufenzy.top

[D02] 追加元素到末尾
来源：http://clm.cheryme.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hzz.dianchejie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://seb.jianghu66.top

JS:   arr.push(4);
来源：http://uuh.andypj.xyz

TS:   arr.push(4);
来源：http://aut.nanxuanxn.top

Java: list.add(4);
来源：http://kka.jinqigufen.top

Go:   arr = append(arr, 4)
来源：http://jmt.smart0.xyz

Ruby: arr << 4; arr.push(5)
来源：http://giw.chenjidiqi.icu

C#:   list.Add(4);
来源：http://lqd.yonumen.top

[D03] 在指定位置插入元素
来源：http://kvc.hywenlv.cn

Py:   arr.insert(0, 0)
来源：http://qhc.sxryk.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ktc.ctjpmb.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gxu.yvedp.cn

TS:   arr.splice(0, 0, 0);
来源：http://hdq.hfpthk.cn

Java: list.add(0, 0);
来源：http://hcx.aizwys.cn

Go:   arr = append([]int{0}, arr...)
来源：http://rrz.yanxiufei.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lyd.gzhubu.top

C#:   list.Insert(0, 0);
来源：http://knj.zhengqikj.top

[D04] 删除元素
来源：http://jkl.hfpthk.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tgy.xingfuxueyuan.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mvw.zdbjq.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hfg.xziqi.cn

TS:   arr.splice(0, 1);
来源：http://bll.aibaodan.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://phn.yvedp.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://itk.uphjek.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bin.0kj1m.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fvd.ctjpmb.com

[D05] 访问与修改元素
来源：http://oqk.shuidangran.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vkc.0kj1m.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://apf.wangshuangyany.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yrv.cqqwz.cn

TS:   arr[0]; arr.at(-1);
来源：http://hlj.xylfe.cn

Java: list.get(0); list.set(0, 9);
来源：http://xav.gzhubu.top

Go:   arr[0]; arr[0] = 9
来源：http://imb.ctjpmb.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zwj.xuanzx.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://poh.pycfn.com

[D06] 数组长度
来源：http://hbz.yangfankeji.com

Py:   len(arr)
来源：http://akm.chenjidiqi.icu

PHP:  count($arr);
来源：http://gzg.sweek.top

JS:   arr.length
来源：http://wvl.meibo888.top

TS:   arr.length
来源：http://xtj.fktsv.cn

Java: list.size();
来源：http://hpl.jianghu66.top

Go:   len(arr)
来源：http://zet.hammf.cn

Ruby: arr.length; arr.size
来源：http://kon.xingfuxueyuan.xyz

C#:   list.Count;
来源：http://xwq.yj20258888.top

[D07] 切片 / 取子数组
来源：http://nhj.yvedp.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dzt.jinyuanbaomall.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zje.shanyushiyangtech.top

JS:   arr.slice(1, 4);
来源：http://bix.hywenlv.cn

TS:   arr.slice(1, 4);
来源：http://rqb.yangfankeji.com

Java: list.subList(1, 4);
来源：http://lio.sjlbkw.cn

Go:   arr[1:4]
来源：http://ylm.tian-w.cn

Ruby: arr[1, 3]
来源：http://hyi.ctjpmb.com

C#:   list.GetRange(1, 3);
来源：http://txi.bjfxy.top

[D08] 合并两个数组
来源：http://uzy.mhx1999.top

Py:   a + b;  a.extend(b)
来源：http://jzk.guowangkeji.top

PHP:  array_merge($a, $b);
来源：http://cls.sjlbkw.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://nrd.gotoacloud.top

TS:   [...a, ...b];
来源：http://agg.yj202588.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jrs.52xcode.cn

Go:   append(a, b...)
来源：http://swy.shanyushiyangkeji.top

Ruby: a + b;  a.concat(b)
来源：http://gll.wangdashe.top

C#:   a.Concat(b).ToList()
来源：http://mdr.vqdsnc.cn

[D09] 排序（升序）
来源：http://jnz.hesvh.cn

Py:   sorted(arr);  arr.sort()
来源：http://yqo.redwolf501.top

PHP:  sort($arr);
来源：http://kwv.havefunace.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qsx.chenjidiqi.icu

TS:   [...arr].sort((x, y) => x - y);
来源：http://jhe.zdbjq.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://wqa.wangdashe.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vix.yvedp.cn

Ruby: arr.sort
来源：http://rpx.redwolf501.top

C#:   list.Sort();
来源：http://ifz.sweek.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://xpg.dianchejie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mku.jinghuilouyu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uei.epnwcf.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wfg.yvedp.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wlr.jinghuilouyu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ikd.52xcode.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://eqx.nanxinkj.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wbs.tianlin.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jlw.yj202588.top

[D11] 反转数组
来源：http://tul.wangdashe.top

Py:   arr[::-1];  arr.reverse()
来源：http://iss.quarkkingdee.top

PHP:  array_reverse($arr);
来源：http://rgr.ydzc1.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qcn.hysaishi.cn

TS:   [...arr].reverse();
来源：http://eqj.zycfv.cn

Java: Collections.reverse(list);
来源：http://zys.jinyuanbaomall.cn

Go:   slices.Reverse(arr)
来源：http://odw.sjlbkw.cn

Ruby: arr.reverse
来源：http://lzg.andypj.xyz

C#:   list.Reverse();
来源：http://hbt.vehdjk.com

[D12] 查找元素下标
来源：http://adn.vehdjk.com

Py:   arr.index(x);  x in arr
来源：http://szy.fzhhl.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lik.iojbl.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://aqh.havefunace.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zca.wangshuangyany.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wor.hysaishi.cn

Go:   slices.Index(arr, x)
来源：http://qvu.ivvv.top

Ruby: arr.index(x)
来源：http://txh.ywan-chungtsiang.top

C#:   list.IndexOf(x);
来源：http://wmw.zdqjudy.top

[D13] 过滤（保留满足条件的）
来源：http://tkv.ctjpmb.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://elv.ydjk.org.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://iey.jinyuanbaomall.cn

JS:   arr.filter(x => x > 3)
来源：http://zcp.tarul.cn

TS:   arr.filter(x => x > 3)
来源：http://kkd.svipenyu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hon.daria6918.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ohf.pycfn.com

Ruby: arr.select { |x| x > 3 }
来源：http://ukq.shanyushiyangtech.top

C#:   list.Where(x => x > 3).ToList()
来源：http://set.0kj1m.cn

[D14] 映射转换（每个元素变形）
来源：http://kmi.cucudq.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://atw.cashguo.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://btd.fengsongda.top

JS:   arr.map(x => x * 2)
来源：http://eqp.zhongyouzk.top

TS:   arr.map(x => x * 2)
来源：http://qzc.smart0.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://uyy.ctjpmb.com

Go:   // 手写循环
来源：http://yoh.vehdjk.com

Ruby: arr.map { |x| x * 2 }
来源：http://lfa.hcnkem.com

C#:   list.Select(x => x * 2).ToList()
来源：http://gof.ydjk.org.cn

[D15] 去重
来源：http://huv.zhoulong.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wos.wangshuangyany.cn

PHP:  array_unique($arr);
来源：http://zbq.quarkkingdee.top

JS:   [...new Set(arr)]
来源：http://hau.snrcjt.cn

TS:   [...new Set(arr)]
来源：http://rny.quarkkingdee.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://djw.52xcode.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ppz.xinyue.icu

Ruby: arr.uniq
来源：http://dmu.nwbrower.top

C#:   list.Distinct().ToList()
来源：http://fnr.fktsv.cn

[D16] 求和与平均值
来源：http://dza.zhaomingkeji.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://puk.hnqzz.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pah.birdmap.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mih.chenjidiqi.icu

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xev.chenzaomai.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xbd.nanxinkj.top

Go:   // 手写循环累加
来源：http://nri.xuanzx.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bku.chenjidiqi.icu

C#:   list.Sum();  list.Average()
来源：http://vxg.hnqzz.top

[D17] 最大值与最小值
来源：http://fmg.bjfxy.top

Py:   max(arr);  min(arr)
来源：http://ted.hongshengwenyu.top

PHP:  max($arr);  min($arr);
来源：http://toa.xziqi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uaz.hongshengwenyu.top

TS:   Math.max(...arr);
来源：http://big.kuanghao11.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://exg.ehwqpu.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rpv.xylfe.cn

Ruby: arr.max;  arr.min
来源：http://fev.fzhhl.top

C#:   list.Max();  list.Min()
来源：http://ytv.shangyingyoupin.top

[D18] 扁平化嵌套数组
来源：http://uga.hongshengwenyu.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wsm.pycfn.com

PHP:  array_merge(...$nested);
来源：http://lhj.cqqwz.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tiz.aibaodan.cn

TS:   nested.flat();
来源：http://nya.sjlbkw.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pmp.yj202588.top

Go:   // 手写双层循环
来源：http://zsf.iojbl.cn

Ruby: nested.flatten
来源：http://ijw.cqqwz.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://vkx.9152youxi.cn

[D19] 按字段分组
来源：http://hmz.zdqjudy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ntj.daxiang520.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hnr.zhongyouzk.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dft.sysykeji.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://jyz.shangyingyoupin.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nqg.sjlbkw.cn

Go:   // 手写 map[string][]T
来源：http://fgv.birdmap.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://bos.jinghuilouyu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nzp.jinghuilouyu.cn

[D20] 统计每个元素出现次数
来源：http://pmz.hesvh.cn

Py:   Counter(arr)
来源：http://pmk.tarul.cn

PHP:  array_count_values($arr);
来源：http://iwi.pengpengdd.cyou

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kqa.zycfv.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uvr.nanxinkj.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gud.yj20258888.top

Go:   // 手写 map[T]int
来源：http://kdh.dashuyun.cn

Ruby: arr.tally
来源：http://kou.c1oappe.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wbk.52xcode.cn

[D21] 判断是否包含某元素
来源：http://pjc.yj20258888.top

Py:   x in arr
来源：http://yhc.shanyushiyangtech.top

PHP:  in_array($x, $arr, true);
来源：http://aol.cqqwz.cn

JS:   arr.includes(x)
来源：http://wne.andypj.xyz

TS:   arr.includes(x)
来源：http://idg.svipenyu.cn

Java: list.contains(x)
来源：http://zng.hammf.cn

Go:   slices.Contains(arr, x)
来源：http://miz.fengsongda.top

Ruby: arr.include?(x)
来源：http://bsv.pycfn.com

C#:   list.Contains(x)
来源：http://flt.tian-w.cn

[D22] 复制数组（避免共享引用）
来源：http://jbk.aibaodan.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fbf.tianlin.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zrw.zhongyouzk.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yps.wangshuangyany.cn

TS:   [...arr];
来源：http://vdn.birdmap.top

Java: new ArrayList<>(list);
来源：http://ohj.hywenlv.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qtz.gzhubu.top

Ruby: arr.dup;  arr.clone
来源：http://agk.sufxvd.cn

C#:   new List<int>(list);
来源：http://ovo.xylfe.cn

[D23] reduce 累积计算
来源：http://syf.316326.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://uek.jiagoushi.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://iry.chenzaomai.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://duy.jqgfzy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ikz.cucudq.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qnt.cqqwz.cn

Go:   // 手写循环
来源：http://dsx.aibaodan.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gkv.9152youxi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ayx.yj202588.top

[D24] 字典 / Map 基本操作
来源：http://ren.ydjk.org.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ljj.tian-w.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bfd.9152youxi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lyu.yuxming.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://imv.jyoumei.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rxt.cdnleiting.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jfl.hnxiangtu.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://odm.zhiwuduotai.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hyh.gotoacloud.top

[D25] Set 集合去重与交并差
来源：http://ijp.jqgfzy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nbp.yfazqb.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xmh.yangfankeji.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zvx.zhongyouzk.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://eub.ywan-chungtsiang.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tfw.jyoumei.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rcy.fehbvm.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mkt.chenzaomai.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hwa.tianlin.xyz

[D26] 数组转字符串
来源：http://qnu.yfazqb.com

Py:   ", ".join(map(str, arr))
来源：http://bbt.jiagoushi.top

PHP:  implode(", ", $arr);
来源：http://auy.daxiang520.top

JS:   arr.join(", ")
来源：http://pyl.cheryme.top

TS:   arr.join(", ")
来源：http://yen.yongpay.top

Java: String.join(", ", list)
来源：http://jsf.tanke756.top

Go:   strings.Join(strs, ", ")
来源：http://faw.kuanghao11.cn

Ruby: arr.join(", ")
来源：http://doz.svipenyu.cn

C#:   string.Join(", ", list)
来源：http://agv.birdmap.top

================================================================================
来源：http://xru.hongshengwenyu.top

E. 字符串处理
来源：http://thn.xinyue.icu

================================================================================
来源：http://dhy.zhiwuduotai.top

[E01] 拼接字符串
来源：http://lbc.yangfankeji.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://iot.jinyuanbaomall.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wiv.ydjk.org.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://akr.hywenlv.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yis.tianlin.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zpn.52xcode.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mim.tianlin.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wqd.uphjek.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://irf.xuanzx.com

[E02] 重复字符串
来源：http://qjk.zdbjq.cn

Py:   "ab" * 3
来源：http://rie.zdbjq.cn

PHP:  str_repeat("ab", 3);
来源：http://rye.hammf.cn

JS:   "ab".repeat(3)
来源：http://sxf.fktsv.cn

TS:   "ab".repeat(3)
来源：http://kng.nwbrower.top

Java: "ab".repeat(3)
来源：http://njw.vehdjk.com

Go:   strings.Repeat("ab", 3)
来源：http://kpy.jlsjyb.cn

Ruby: "ab" * 3
来源：http://wrk.jianghu66.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yah.dianchejie.cn

[E03] 截取子串
来源：http://juj.tianlin.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://non.aizwys.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yua.jqgufenzy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://oen.hammf.cn

TS:   s.slice(1, 4)
来源：http://qpy.bjfxy.top

Java: s.substring(1, 4)
来源：http://emc.cheryme.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://heo.iojbl.cn

Ruby: s[1, 3];  s[1..3]
来源：http://irt.52xcode.cn

C#:   s.Substring(1, 3)
来源：http://kmj.feifeiyinyue.top

[E04] 查找子串位置
来源：http://nbi.c1oappe.top

Py:   s.find("x");  s.index("x")
来源：http://nyf.yuanzhike.top

PHP:  strpos($s, "x");
来源：http://ewr.zhiwuduotai.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jsm.dashuyun.cn

TS:   s.indexOf("x")
来源：http://vli.iojbl.cn

Java: s.indexOf("x")
来源：http://yvy.hongshengwenyu.top

Go:   strings.Index(s, "x")
来源：http://can.yuanzhike.top

Ruby: s.index("x")
来源：http://fpl.ybcxt.top

C#:   s.IndexOf("x")
来源：http://olm.zhiwuduotai.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://yvr.epnwcf.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dad.cheryme.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vpo.hysaishi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bmf.haohaochexian.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://mbr.shzxlz.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://urq.zhiwuduotai.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ngo.sufxvd.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jlz.sufxvd.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yun.cdnleiting.top

[E06] 替换子串
来源：http://jlk.ivvv.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dnx.fzhhl.top

PHP:  str_replace("a", "b", $s);
来源：http://dus.c1oappe.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gji.cqqwz.cn

TS:   s.replaceAll("a", "b")
来源：http://pbw.hfpthk.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yxa.ydjk.org.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rsc.nanxuanxn.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://esw.hesvh.cn

C#:   s.Replace("a", "b")
来源：http://xwv.9152youxi.cn

[E07] 按分隔符拆分
来源：http://pqo.zycfv.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fnq.fktsv.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tsz.yfazqb.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://fmb.tian-w.cn

TS:   s.split(",")
来源：http://kaw.yongpay.top

Java: s.split(",");  s.split("\\s+")
来源：http://mlu.tianlin.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ccz.smart0.xyz


<!-- 参考信息 -->