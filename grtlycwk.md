代发 wailian999

Ruby: a, b = pair
来源：http://jzk.yangfankeji.com

C#:   var (a, b) = pair;
来源：http://vqx.pycfn.com

[C16] 函数 / 方法重载
来源：http://hfr.redwolf501.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hzk.jqgufenzy.top

PHP:  // 无重载
来源：http://mkf.yonumen.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://nnk.gogol.net.cn

TS:   // 用联合类型或重载签名声明
来源：http://wdr.hnqzz.top

Java: void f(int a) {}  void f(String a) {}
来源：http://uix.wangshuangyany.cn

Go:   // 无重载：用不同函数名
来源：http://rxt.birdmap.top

Ruby: # 无重载：靠动态参数
来源：http://ktq.gotoacloud.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://dvz.jyoumei.cn

================================================================================
来源：http://fug.epnwcf.com

D. 数组 / 列表 / 集合
来源：http://awe.shzxlz.cn

================================================================================
来源：http://wqm.snrcjt.cn

[D01] 创建数组 / 列表
来源：http://twq.jlsjyb.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pvn.chenjidiqi.icu

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ule.hongshengwenyu.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nid.meibo888.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://mct.hammf.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rne.yvedp.cn

Go:   arr := []int{1, 2, 3}
来源：http://mpw.chenzaomai.com

Ruby: arr = [1, 2, 3]
来源：http://ocv.pengpengdd.cyou

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vzx.feifeiyinyue.top

[D02] 追加元素到末尾
来源：http://hix.fengsongda.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mgp.zhoulong.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://erc.yangfankeji.com

JS:   arr.push(4);
来源：http://aqn.zhengqikj.top

TS:   arr.push(4);
来源：http://umm.iojbl.cn

Java: list.add(4);
来源：http://dzp.sjlbkw.cn

Go:   arr = append(arr, 4)
来源：http://dbd.jinghuilouyu.cn

Ruby: arr << 4; arr.push(5)
来源：http://cmr.vqdsnc.cn

C#:   list.Add(4);
来源：http://qws.aizwys.cn

[D03] 在指定位置插入元素
来源：http://dos.andypj.xyz

Py:   arr.insert(0, 0)
来源：http://nle.yueranfly.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uxw.bbcook.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dgb.ppjwa.cn

TS:   arr.splice(0, 0, 0);
来源：http://cze.zhiwuduotai.top

Java: list.add(0, 0);
来源：http://lwp.sweek.top

Go:   arr = append([]int{0}, arr...)
来源：http://baz.zdbjq.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dul.vqdsnc.cn

C#:   list.Insert(0, 0);
来源：http://fbf.yj20258888.top

[D04] 删除元素
来源：http://onn.yonumen.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pqr.aizwys.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://chs.smart0.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://khe.52xcode.cn

TS:   arr.splice(0, 1);
来源：http://pnp.tian-w.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cin.zhiwuduotai.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://eew.xziqi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yue.xingfuxueyuan.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://egd.birdmap.top

[D05] 访问与修改元素
来源：http://rkc.zdqjudy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vcq.bjfxy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xaz.quarkkingdee.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://feg.shzxlz.cn

TS:   arr[0]; arr.at(-1);
来源：http://mlp.jyoumei.cn

Java: list.get(0); list.set(0, 9);
来源：http://lfu.fanxiaobao.xyz

Go:   arr[0]; arr[0] = 9
来源：http://wgc.hysaishi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rjj.guannengcc.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fin.hnqzz.top

[D06] 数组长度
来源：http://xtp.chenzaomai.com

Py:   len(arr)
来源：http://qqj.zdbjq.cn

PHP:  count($arr);
来源：http://ncn.sweek.top

JS:   arr.length
来源：http://veg.316326.xyz

TS:   arr.length
来源：http://dtr.zhiwuduotai.top

Java: list.size();
来源：http://woa.sufxvd.cn

Go:   len(arr)
来源：http://zwc.sweek.top

Ruby: arr.length; arr.size
来源：http://nza.yuanzhike.top

C#:   list.Count;
来源：http://mar.yuanzhike.top

[D07] 切片 / 取子数组
来源：http://sba.gotoacloud.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gxr.jqgfzy.top

PHP:  array_slice($arr, 1, 3);
来源：http://shs.jlsjyb.cn

JS:   arr.slice(1, 4);
来源：http://tgw.0kj1m.cn

TS:   arr.slice(1, 4);
来源：http://hnq.yangfankeji.com

Java: list.subList(1, 4);
来源：http://uba.zhiwuduotai.top

Go:   arr[1:4]
来源：http://hcc.52xcode.cn

Ruby: arr[1, 3]
来源：http://rgh.snrcjt.cn

C#:   list.GetRange(1, 3);
来源：http://wez.haohaochexian.top

[D08] 合并两个数组
来源：http://ntm.sweek.top

Py:   a + b;  a.extend(b)
来源：http://llk.yj202588.top

PHP:  array_merge($a, $b);
来源：http://edf.316326.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://nsm.xuanzx.com

TS:   [...a, ...b];
来源：http://pvl.ppjwa.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://axa.nanxinkj.top

Go:   append(a, b...)
来源：http://yst.yangfankeji.com

Ruby: a + b;  a.concat(b)
来源：http://tgj.epnwcf.com

C#:   a.Concat(b).ToList()
来源：http://var.hammf.cn

[D09] 排序（升序）
来源：http://lzq.yuanzhike.top

Py:   sorted(arr);  arr.sort()
来源：http://zid.jianghu66.top

PHP:  sort($arr);
来源：http://gge.hammf.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lnf.chenlongwang.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://qbu.tarul.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tzs.hysaishi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://sft.sweek.top

Ruby: arr.sort
来源：http://kgx.hammf.cn

C#:   list.Sort();
来源：http://iyl.ywan-chungtsiang.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://epx.haohaochexian.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ubp.yj20258888.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tzt.sweek.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://uss.cucudq.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ljo.hnxiangtu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fym.cheryme.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dhn.ehwqpu.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wvk.nanxuanxn.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kdd.cashguo.top

[D11] 反转数组
来源：http://jnt.snrcjt.cn

Py:   arr[::-1];  arr.reverse()
来源：http://uri.hammf.cn

PHP:  array_reverse($arr);
来源：http://smi.tian-w.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://oor.shuidangran.top

TS:   [...arr].reverse();
来源：http://riq.jianghu66.top

Java: Collections.reverse(list);
来源：http://pil.ehwqpu.com

Go:   slices.Reverse(arr)
来源：http://vog.zdqjudy.top

Ruby: arr.reverse
来源：http://yub.wangdashe.top

C#:   list.Reverse();
来源：http://jsn.gaohongyu789.top

[D12] 查找元素下标
来源：http://dgh.fanxiaobao.xyz

Py:   arr.index(x);  x in arr
来源：http://tnj.52xcode.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wrs.shuidangran.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vyw.hywenlv.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wef.jinqigufen.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kfm.xingfuxueyuan.xyz

Go:   slices.Index(arr, x)
来源：http://vfv.daxiang520.top

Ruby: arr.index(x)
来源：http://bqd.cqqwz.cn

C#:   list.IndexOf(x);
来源：http://rma.chenjidiqi.icu

[D13] 过滤（保留满足条件的）
来源：http://fuz.yueranfly.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xxy.xziqi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ozr.gzhubu.top

JS:   arr.filter(x => x > 3)
来源：http://oxt.yangfankeji.com

TS:   arr.filter(x => x > 3)
来源：http://avb.jinyuanbaomall.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rff.ctjpmb.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://igx.jinyuanbaomall.cn

Ruby: arr.select { |x| x > 3 }
来源：http://nmr.bjfxy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ywk.nwbrower.top

[D14] 映射转换（每个元素变形）
来源：http://she.gotoacloud.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zcv.hnqzz.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vml.0kj1m.cn

JS:   arr.map(x => x * 2)
来源：http://tlx.jinqigfzy.top

TS:   arr.map(x => x * 2)
来源：http://yid.redwolf501.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://xvh.fktsv.cn

Go:   // 手写循环
来源：http://ihg.feifeiyinyue.top

Ruby: arr.map { |x| x * 2 }
来源：http://yiw.ivvv.top

C#:   list.Select(x => x * 2).ToList()
来源：http://mwv.gogol.net.cn

[D15] 去重
来源：http://dqp.9152youxi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pbg.redwolf501.top

PHP:  array_unique($arr);
来源：http://aow.yonumen.top

JS:   [...new Set(arr)]
来源：http://okw.guannengcc.top

TS:   [...new Set(arr)]
来源：http://gbc.xuanzx.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cux.quarkkingdee.top

Go:   // 用 map[T]struct{} 手写
来源：http://sny.zdbjq.cn

Ruby: arr.uniq
来源：http://vfw.sjlbkw.cn

C#:   list.Distinct().ToList()
来源：http://zff.haohaochexian.top

[D16] 求和与平均值
来源：http://npn.zdbjq.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vfy.feifeiyinyue.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dze.zhongyouzk.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jhh.jianghu66.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://grb.pycfn.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lde.dashuyun.cn

Go:   // 手写循环累加
来源：http://wjt.shangyingyoupin.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vac.xinyue.icu

C#:   list.Sum();  list.Average()
来源：http://aaz.fktsv.cn

[D17] 最大值与最小值
来源：http://bvn.vqdsnc.cn

Py:   max(arr);  min(arr)
来源：http://mrv.316326.xyz

PHP:  max($arr);  min($arr);
来源：http://fhb.jinqigfzy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://phb.ivvv.top

TS:   Math.max(...arr);
来源：http://yog.shangyingyoupin.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ush.aizwys.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ksh.hywenlv.cn

Ruby: arr.max;  arr.min
来源：http://hgr.shuidangran.top

C#:   list.Max();  list.Min()
来源：http://knr.guannengcc.top

[D18] 扁平化嵌套数组
来源：http://lxh.chenjidiqi.icu

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dnb.c1oappe.top

PHP:  array_merge(...$nested);
来源：http://xtf.yuxming.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://frk.shuidangran.top

TS:   nested.flat();
来源：http://qde.yanxiufei.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://trc.gogol.net.cn

Go:   // 手写双层循环
来源：http://drc.9152youxi.cn

Ruby: nested.flatten
来源：http://myu.fengsongda.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://cgw.havefunace.top

[D19] 按字段分组
来源：http://atb.guannengcc.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://azq.zhaomingkeji.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hki.zhixingplan.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wri.fanxiaobao.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://qxo.yvedp.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ukg.jlsjyb.cn

Go:   // 手写 map[string][]T
来源：http://hqf.tanke756.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://lgw.shanyushiyangkeji.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jwx.pycfn.com

[D20] 统计每个元素出现次数
来源：http://ylc.epnwcf.com

Py:   Counter(arr)
来源：http://xab.yfazqb.com

PHP:  array_count_values($arr);
来源：http://euj.hywenlv.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qof.cqqwz.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vlb.bjfxy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jja.wangshuangyany.cn

Go:   // 手写 map[T]int
来源：http://emq.yuxming.cn

Ruby: arr.tally
来源：http://icl.shanyushiyangkeji.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dza.dianchejie.cn

[D21] 判断是否包含某元素
来源：http://cgy.smart0.xyz

Py:   x in arr
来源：http://psz.ppjwa.cn

PHP:  in_array($x, $arr, true);
来源：http://agu.meibo888.top

JS:   arr.includes(x)
来源：http://sko.gzhubu.top

TS:   arr.includes(x)
来源：http://mxc.zhixingplan.top

Java: list.contains(x)
来源：http://tvz.shzxlz.cn

Go:   slices.Contains(arr, x)
来源：http://ydu.zhoulong.xyz

Ruby: arr.include?(x)
来源：http://phs.mhx1999.top

C#:   list.Contains(x)
来源：http://mzb.wangshuangyany.cn

[D22] 复制数组（避免共享引用）
来源：http://qlv.sjlbkw.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yxb.sxryk.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zzt.ctjpmb.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mqp.c1oappe.top

TS:   [...arr];
来源：http://lwu.jqgufenzy.top

Java: new ArrayList<>(list);
来源：http://ghm.fzhhl.top

Go:   copied := append([]int(nil), arr...)
来源：http://apc.ivvv.top

Ruby: arr.dup;  arr.clone
来源：http://bcu.hnqzz.top

C#:   new List<int>(list);
来源：http://rje.sufxvd.cn

[D23] reduce 累积计算
来源：http://xah.dashuyun.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ghl.zhiwuduotai.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dqc.bjfxy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bcf.gogol.net.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cxi.ywan-chungtsiang.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://bgf.yonumen.top

Go:   // 手写循环
来源：http://goh.fehbvm.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://awe.aibaodan.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mnu.redwolf501.top

[D24] 字典 / Map 基本操作
来源：http://qni.tanke756.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gpk.shanyushiyangkeji.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qjj.yongpay.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kdu.chenlongwang.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gvm.xuetiantiany.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://efw.tarul.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://auz.yanxiufei.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dow.jianghu66.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://byj.yueranfly.top

[D25] Set 集合去重与交并差
来源：http://tbx.ydzc1.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nqb.yueranfly.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lnp.jqgfzy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vpu.chenjidiqi.icu

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zrk.ppjwa.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wdf.nanxuanxn.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gov.ywan-chungtsiang.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cnk.xinyue.icu

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://uqn.zhaomingkeji.xyz

[D26] 数组转字符串
来源：http://rit.vqdsnc.cn

Py:   ", ".join(map(str, arr))
来源：http://zec.shangyingyoupin.top

PHP:  implode(", ", $arr);
来源：http://rhs.yueranfly.top

JS:   arr.join(", ")
来源：http://edw.shanyushiyangkeji.top

TS:   arr.join(", ")
来源：http://hxu.iojbl.cn

Java: String.join(", ", list)
来源：http://ivv.yanxiufei.cn

Go:   strings.Join(strs, ", ")
来源：http://smq.zycfv.cn

Ruby: arr.join(", ")
来源：http://nqq.tanke756.top

C#:   string.Join(", ", list)
来源：http://tqk.xingfuxueyuan.xyz

================================================================================
来源：http://ewu.fanxiaobao.xyz

E. 字符串处理
来源：http://hfj.tanke756.top

================================================================================
来源：http://muo.zhengqikj.top

[E01] 拼接字符串
来源：http://yoz.316326.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sai.daxiang520.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xxn.pycfn.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fnn.redwolf501.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xdv.hysaishi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rzl.yj202588.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dfe.ehwqpu.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://oll.sysykeji.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://odi.zhijiandao.cn

[E02] 重复字符串
来源：http://xip.shanyushiyangtech.top

Py:   "ab" * 3
来源：http://vjb.feifeiyinyue.top

PHP:  str_repeat("ab", 3);
来源：http://czs.shzxlz.cn

JS:   "ab".repeat(3)
来源：http://cno.yj20258888.top

TS:   "ab".repeat(3)
来源：http://tax.aibaodan.cn

Java: "ab".repeat(3)
来源：http://uwt.tian-w.cn

Go:   strings.Repeat("ab", 3)
来源：http://blu.hnqzz.top

Ruby: "ab" * 3
来源：http://lgy.tarul.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wyd.fehbvm.com

[E03] 截取子串
来源：http://kuc.zhaomingkeji.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qtw.kuanghao11.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://udd.zdbjq.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zip.0kj1m.cn

TS:   s.slice(1, 4)
来源：http://ibr.jqgufenzy.top

Java: s.substring(1, 4)
来源：http://faq.ydzc1.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fcb.shzxlz.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ikh.ivvv.top

C#:   s.Substring(1, 3)
来源：http://dqp.hysaishi.cn

[E04] 查找子串位置
来源：http://uun.jinqigfzy.top

Py:   s.find("x");  s.index("x")
来源：http://gjw.zhoulong.xyz

PHP:  strpos($s, "x");
来源：http://hxc.nanxuanxn.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qev.daxiang520.top

TS:   s.indexOf("x")
来源：http://qzm.cdnleiting.top

Java: s.indexOf("x")
来源：http://zvr.fktsv.cn

Go:   strings.Index(s, "x")
来源：http://hrh.316326.xyz

Ruby: s.index("x")
来源：http://orx.nwbrower.top

C#:   s.IndexOf("x")
来源：http://kfv.dianchejie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://mqp.jiagoushi.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fvr.mhx1999.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ziu.sxryk.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sdh.pycfn.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://zlz.yuanzhike.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nrz.hcnkem.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cjg.smart0.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rak.kuanghao11.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rey.xziqi.cn

[E06] 替换子串
来源：http://cgy.jqgfzy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mdv.jinghuilouyu.cn

PHP:  str_replace("a", "b", $s);
来源：http://bnb.316326.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yix.hesvh.cn


<!-- 参考信息 -->