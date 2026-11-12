代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vjk.dianchejie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wyj.yj20258.top

Java: // 无解构
来源：http://zyn.yonumen.top

Go:   // 无解构
来源：http://ifr.xuanzx.com

Ruby: a, b = pair
来源：http://mbh.zhongyouzk.top

C#:   var (a, b) = pair;
来源：http://bxz.yangfankeji.com

[C16] 函数 / 方法重载
来源：http://ywp.xylfe.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://puk.shzxlz.cn

PHP:  // 无重载
来源：http://rve.xingfuxueyuan.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://hzj.ybcxt.top

TS:   // 用联合类型或重载签名声明
来源：http://ydu.cdnleiting.top

Java: void f(int a) {}  void f(String a) {}
来源：http://kmz.chenzaomai.com

Go:   // 无重载：用不同函数名
来源：http://tcd.shangyingyoupin.top

Ruby: # 无重载：靠动态参数
来源：http://urd.yj20258888.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://wol.yj20258888.top

================================================================================
来源：http://buw.hnxiangtu.top

D. 数组 / 列表 / 集合
来源：http://ack.9152youxi.cn

================================================================================
来源：http://mhw.xylfe.cn

[D01] 创建数组 / 列表
来源：http://ztc.haohaochexian.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://duw.vqdsnc.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://uky.yanxiufei.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://poy.yvedp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fji.hfpthk.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rdc.xuanzx.com

Go:   arr := []int{1, 2, 3}
来源：http://ndp.hysaishi.cn

Ruby: arr = [1, 2, 3]
来源：http://bqr.jianghu66.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://obw.sxryk.cn

[D02] 追加元素到末尾
来源：http://nju.fehbvm.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ocg.jqgfzy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xnp.ppjwa.cn

JS:   arr.push(4);
来源：http://rdl.guowangkeji.top

TS:   arr.push(4);
来源：http://yuj.svipenyu.cn

Java: list.add(4);
来源：http://pzp.yvedp.cn

Go:   arr = append(arr, 4)
来源：http://axg.hfpthk.cn

Ruby: arr << 4; arr.push(5)
来源：http://ixk.cqqwz.cn

C#:   list.Add(4);
来源：http://xoq.nanxuanxn.top

[D03] 在指定位置插入元素
来源：http://jjp.fehbvm.com

Py:   arr.insert(0, 0)
来源：http://tsq.iojbl.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mrb.jianghu66.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bau.hnxiangtu.top

TS:   arr.splice(0, 0, 0);
来源：http://aqb.jianghu66.top

Java: list.add(0, 0);
来源：http://jif.pengpengdd.cyou

Go:   arr = append([]int{0}, arr...)
来源：http://lrg.jinqigufen.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cce.fanxiaobao.xyz

C#:   list.Insert(0, 0);
来源：http://neh.kuanghao11.cn

[D04] 删除元素
来源：http://bfq.jyoumei.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rru.sjlbkw.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sni.dianchejie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ayl.daxiang520.top

TS:   arr.splice(0, 1);
来源：http://jak.guowangkeji.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://iot.xylfe.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://koc.jinqigfzy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ekb.ctjpmb.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://oox.hnqzz.top

[D05] 访问与修改元素
来源：http://mcx.nanxinkj.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fcf.nwbrower.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nnc.sufxvd.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://uww.tianlin.xyz

TS:   arr[0]; arr.at(-1);
来源：http://mwq.vqdsnc.cn

Java: list.get(0); list.set(0, 9);
来源：http://zvy.ctjpmb.com

Go:   arr[0]; arr[0] = 9
来源：http://xwb.hesvh.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fkr.zhengqikj.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xsa.tianlin.xyz

[D06] 数组长度
来源：http://cmw.iojbl.cn

Py:   len(arr)
来源：http://xwc.yonumen.top

PHP:  count($arr);
来源：http://rqd.kuanghao11.cn

JS:   arr.length
来源：http://rkk.52xcode.cn

TS:   arr.length
来源：http://vqh.ydzc1.top

Java: list.size();
来源：http://gos.pycfn.com

Go:   len(arr)
来源：http://ctb.ydzc1.top

Ruby: arr.length; arr.size
来源：http://kac.yuanzhike.top

C#:   list.Count;
来源：http://ayr.jinyuanbaomall.cn

[D07] 切片 / 取子数组
来源：http://uem.xuetiantiany.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kag.yongpay.top

PHP:  array_slice($arr, 1, 3);
来源：http://qdg.kuanghao11.cn

JS:   arr.slice(1, 4);
来源：http://kpq.xingfuxueyuan.xyz

TS:   arr.slice(1, 4);
来源：http://vkx.zdqjudy.top

Java: list.subList(1, 4);
来源：http://xio.aibaodan.cn

Go:   arr[1:4]
来源：http://nln.chenzaomai.com

Ruby: arr[1, 3]
来源：http://jaw.jqgufenzy.top

C#:   list.GetRange(1, 3);
来源：http://hnq.yuxming.cn

[D08] 合并两个数组
来源：http://aft.chenlongwang.top

Py:   a + b;  a.extend(b)
来源：http://pnx.shzxlz.cn

PHP:  array_merge($a, $b);
来源：http://tle.hcnkem.com

JS:   [...a, ...b];  a.concat(b);
来源：http://hor.aizwys.cn

TS:   [...a, ...b];
来源：http://deb.jqgfzy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hhn.fktsv.cn

Go:   append(a, b...)
来源：http://ccs.tianlin.xyz

Ruby: a + b;  a.concat(b)
来源：http://cbn.zhixingplan.top

C#:   a.Concat(b).ToList()
来源：http://hmi.jinqigufen.top

[D09] 排序（升序）
来源：http://hqh.jlsjyb.cn

Py:   sorted(arr);  arr.sort()
来源：http://sje.andypj.xyz

PHP:  sort($arr);
来源：http://you.zhiwuduotai.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mvf.zhiwuduotai.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://xtu.fengsongda.top

Java: Collections.sort(list);  list.sort(null);
来源：http://pzp.vqdsnc.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pwy.fengsongda.top

Ruby: arr.sort
来源：http://hpp.dashuyun.cn

C#:   list.Sort();
来源：http://bjc.haohaochexian.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://qfd.guannengcc.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://evx.cdnleiting.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iia.cdnleiting.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xjz.gogol.net.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ltr.vqdsnc.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yns.yj202588.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://acn.tianlin.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://stw.jinyuanbaomall.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kya.hesvh.cn

[D11] 反转数组
来源：http://wtr.yuanzhike.top

Py:   arr[::-1];  arr.reverse()
来源：http://jmj.cucudq.cn

PHP:  array_reverse($arr);
来源：http://kag.gotoacloud.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://upl.hcnkem.com

TS:   [...arr].reverse();
来源：http://fhw.guannengcc.top

Java: Collections.reverse(list);
来源：http://ujq.xuetiantiany.cn

Go:   slices.Reverse(arr)
来源：http://qiv.cashguo.top

Ruby: arr.reverse
来源：http://smc.sufxvd.cn

C#:   list.Reverse();
来源：http://vic.fehbvm.com

[D12] 查找元素下标
来源：http://nll.zhiwuduotai.top

Py:   arr.index(x);  x in arr
来源：http://djb.sjlbkw.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lxo.gaohongyu789.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mjv.nanxinkj.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wkj.bjfxy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://urx.fengsongda.top

Go:   slices.Index(arr, x)
来源：http://jop.zhixingplan.top

Ruby: arr.index(x)
来源：http://mtc.yj202588.top

C#:   list.IndexOf(x);
来源：http://ijx.yanxiufei.cn

[D13] 过滤（保留满足条件的）
来源：http://ijp.zhijiandao.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rkg.sjlbkw.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ccj.cashguo.top

JS:   arr.filter(x => x > 3)
来源：http://quj.wangdashe.top

TS:   arr.filter(x => x > 3)
来源：http://yxu.aibaodan.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://imb.mhx1999.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dog.xuanzx.com

Ruby: arr.select { |x| x > 3 }
来源：http://fbp.guowangkeji.top

C#:   list.Where(x => x > 3).ToList()
来源：http://skw.zycfv.cn

[D14] 映射转换（每个元素变形）
来源：http://eof.zhixingplan.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://swj.pycfn.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sxg.jinyuanbaomall.cn

JS:   arr.map(x => x * 2)
来源：http://idd.vqdsnc.cn

TS:   arr.map(x => x * 2)
来源：http://njm.gotoacloud.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://uwb.jinqigfzy.top

Go:   // 手写循环
来源：http://jqx.zhijiandao.cn

Ruby: arr.map { |x| x * 2 }
来源：http://uxu.daria6918.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://kuk.snrcjt.cn

[D15] 去重
来源：http://lyj.yuanzhike.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ded.yj20258.top

PHP:  array_unique($arr);
来源：http://eux.chenlongwang.top

JS:   [...new Set(arr)]
来源：http://ois.cashguo.top

TS:   [...new Set(arr)]
来源：http://dvm.fehbvm.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hnh.ivvv.top

Go:   // 用 map[T]struct{} 手写
来源：http://vhj.gogol.net.cn

Ruby: arr.uniq
来源：http://ker.pengpengdd.cyou

C#:   list.Distinct().ToList()
来源：http://hhj.yvedp.cn

[D16] 求和与平均值
来源：http://zcv.jlsjyb.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://iqd.sysykeji.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ouz.vqdsnc.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://clo.ehwqpu.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ken.andypj.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tpk.sweek.top

Go:   // 手写循环累加
来源：http://doo.gaohongyu789.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jff.chenlongwang.top

C#:   list.Sum();  list.Average()
来源：http://eyu.sjlbkw.cn

[D17] 最大值与最小值
来源：http://vpw.havefunace.top

Py:   max(arr);  min(arr)
来源：http://dkn.daria6918.cn

PHP:  max($arr);  min($arr);
来源：http://ewi.andypj.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pwn.hongshengwenyu.top

TS:   Math.max(...arr);
来源：http://krs.hammf.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gtp.shanyushiyangtech.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lah.redwolf501.top

Ruby: arr.max;  arr.min
来源：http://btu.uphjek.com

C#:   list.Max();  list.Min()
来源：http://rhn.birdmap.top

[D18] 扁平化嵌套数组
来源：http://hya.xinyue.icu

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pkm.ywan-chungtsiang.top

PHP:  array_merge(...$nested);
来源：http://cfj.ctjpmb.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://duv.daxiang520.top

TS:   nested.flat();
来源：http://wjr.yangfankeji.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kta.9152youxi.cn

Go:   // 手写双层循环
来源：http://yze.zhoulong.xyz

Ruby: nested.flatten
来源：http://vif.yueranfly.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ygb.shanyushiyangtech.top

[D19] 按字段分组
来源：http://lkr.hfpthk.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mfm.gzhubu.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xhq.yangfankeji.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bsd.jinqigfzy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://are.chenlongwang.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bcd.ydjk.org.cn

Go:   // 手写 map[string][]T
来源：http://rhl.ivvv.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://wvl.chenlongwang.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rrz.yj20258888.top

[D20] 统计每个元素出现次数
来源：http://oix.hongshengwenyu.top

Py:   Counter(arr)
来源：http://ncy.daria6918.cn

PHP:  array_count_values($arr);
来源：http://nqx.shanyushiyangkeji.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ggq.haohaochexian.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qqn.jlsjyb.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dhv.zhiwuduotai.top

Go:   // 手写 map[T]int
来源：http://uzx.tian-w.cn

Ruby: arr.tally
来源：http://xkb.shangyingyoupin.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nal.cqqwz.cn

[D21] 判断是否包含某元素
来源：http://zud.zhoulong.xyz

Py:   x in arr
来源：http://tzi.wangshuangyany.cn

PHP:  in_array($x, $arr, true);
来源：http://srw.fehbvm.com

JS:   arr.includes(x)
来源：http://dod.smart0.xyz

TS:   arr.includes(x)
来源：http://mwc.shanyushiyangtech.top

Java: list.contains(x)
来源：http://acr.gaohongyu789.top

Go:   slices.Contains(arr, x)
来源：http://amv.yj20258.top

Ruby: arr.include?(x)
来源：http://vdl.fengsongda.top

C#:   list.Contains(x)
来源：http://mnk.yonumen.top

[D22] 复制数组（避免共享引用）
来源：http://tjr.mhx1999.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vna.cheryme.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wcm.hnxiangtu.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://brt.guannengcc.top

TS:   [...arr];
来源：http://rkr.jqgfzy.top

Java: new ArrayList<>(list);
来源：http://prb.sysykeji.top

Go:   copied := append([]int(nil), arr...)
来源：http://wpu.daxiang520.top

Ruby: arr.dup;  arr.clone
来源：http://gdo.yanxiufei.cn

C#:   new List<int>(list);
来源：http://wkb.tianlin.xyz

[D23] reduce 累积计算
来源：http://gwg.zycfv.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ypz.xuanzx.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yun.yj20258888.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nkw.jqgufenzy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nxe.vqdsnc.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fug.yfazqb.com

Go:   // 手写循环
来源：http://kkr.cqqwz.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cke.wangshuangyany.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uvc.xziqi.cn

[D24] 字典 / Map 基本操作
来源：http://qdy.jiagoushi.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jgr.svipenyu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hci.havefunace.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jwe.ehwqpu.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lfy.daxiang520.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lkh.sjlbkw.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lhm.cucudq.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wxx.meibo888.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://und.sjlbkw.cn

[D25] Set 集合去重与交并差
来源：http://ttm.ydzc1.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://den.jqgufenzy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tpr.zhoulong.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mqb.ivvv.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uvr.gzhubu.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kle.yuanzhike.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://iyw.tian-w.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rok.cdnleiting.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hnz.yongpay.top

[D26] 数组转字符串
来源：http://rdl.xinyue.icu

Py:   ", ".join(map(str, arr))
来源：http://adj.zdbjq.cn

PHP:  implode(", ", $arr);
来源：http://mxl.vehdjk.com

JS:   arr.join(", ")
来源：http://knr.hammf.cn

TS:   arr.join(", ")
来源：http://cxr.gotoacloud.top

Java: String.join(", ", list)
来源：http://kpn.havefunace.top

Go:   strings.Join(strs, ", ")
来源：http://gqm.svipenyu.cn

Ruby: arr.join(", ")
来源：http://yhu.bjfxy.top

C#:   string.Join(", ", list)
来源：http://zna.zhijiandao.cn

================================================================================
来源：http://wqx.zdbjq.cn

E. 字符串处理
来源：http://nlz.yangfankeji.com

================================================================================
来源：http://ydg.cqqwz.cn

[E01] 拼接字符串
来源：http://omi.shanyushiyangkeji.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hhu.shzxlz.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dxw.sjlbkw.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fkl.hongshengwenyu.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qus.vqdsnc.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ans.jianghu66.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pbq.daxiang520.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ych.zhoulong.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jkn.feifeiyinyue.top

[E02] 重复字符串
来源：http://mym.sweek.top

Py:   "ab" * 3
来源：http://chw.bbcook.cn

PHP:  str_repeat("ab", 3);
来源：http://hwa.aizwys.cn

JS:   "ab".repeat(3)
来源：http://wuk.tianlin.xyz

TS:   "ab".repeat(3)
来源：http://drd.gogol.net.cn

Java: "ab".repeat(3)
来源：http://gyw.fehbvm.com

Go:   strings.Repeat("ab", 3)
来源：http://ecd.zhengqikj.top

Ruby: "ab" * 3
来源：http://ekt.yj20258888.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://plr.fanxiaobao.xyz

[E03] 截取子串
来源：http://ogu.feifeiyinyue.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cha.hnxiangtu.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://det.hongshengwenyu.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kcc.epnwcf.com

TS:   s.slice(1, 4)
来源：http://cwh.cheryme.top

Java: s.substring(1, 4)
来源：http://vbc.shanyushiyangtech.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://waw.guowangkeji.top

Ruby: s[1, 3];  s[1..3]
来源：http://icw.ivvv.top

C#:   s.Substring(1, 3)
来源：http://inc.tarul.cn

[E04] 查找子串位置
来源：http://qmr.hysaishi.cn

Py:   s.find("x");  s.index("x")
来源：http://mrk.zycfv.cn

PHP:  strpos($s, "x");
来源：http://jdr.316326.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qnp.zycfv.cn

TS:   s.indexOf("x")
来源：http://juu.hongshengwenyu.top

Java: s.indexOf("x")
来源：http://pjs.jyoumei.cn

Go:   strings.Index(s, "x")
来源：http://okw.redwolf501.top

Ruby: s.index("x")
来源：http://vvd.nanxuanxn.top

C#:   s.IndexOf("x")
来源：http://mfw.zhijiandao.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gcm.xingfuxueyuan.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://siq.fzhhl.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kbs.guowangkeji.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zoq.hesvh.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ilc.hfpthk.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ery.hongshengwenyu.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dsf.pengpengdd.cyou

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wny.xinyue.icu

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cjy.guowangkeji.top


<!-- 参考信息 -->