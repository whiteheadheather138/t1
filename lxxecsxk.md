代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gvi.hcnkem.com

[C15] 解构 / 展开参数
来源：http://luj.dianchejie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ovm.tianlin.xyz

PHP:  [$a, $b] = $pair;
来源：http://hyy.gzhubu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qru.sysykeji.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sdm.ctjpmb.com

Java: // 无解构
来源：http://njz.jyoumei.cn

Go:   // 无解构
来源：http://qpl.tarul.cn

Ruby: a, b = pair
来源：http://dua.9152youxi.cn

C#:   var (a, b) = pair;
来源：http://fzb.jinyuanbaomall.cn

[C16] 函数 / 方法重载
来源：http://pch.xinyue.icu

Py:   # 无重载：用默认参数或 *args 变通
来源：http://unt.jinghuilouyu.cn

PHP:  // 无重载
来源：http://qip.zhoulong.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://dev.jinyuanbaomall.cn

TS:   // 用联合类型或重载签名声明
来源：http://lsp.yangfankeji.com

Java: void f(int a) {}  void f(String a) {}
来源：http://frv.andypj.xyz

Go:   // 无重载：用不同函数名
来源：http://vfd.sjlbkw.cn

Ruby: # 无重载：靠动态参数
来源：http://aas.vehdjk.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://vxm.dashuyun.cn

================================================================================
来源：http://exb.hfpthk.cn

D. 数组 / 列表 / 集合
来源：http://txp.bbcook.cn

================================================================================
来源：http://otp.yfazqb.com

[D01] 创建数组 / 列表
来源：http://zce.tian-w.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://fec.vehdjk.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hws.jlsjyb.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mfo.shangyingyoupin.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://oal.jinghuilouyu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tdw.daria6918.cn

Go:   arr := []int{1, 2, 3}
来源：http://qtb.yj20258888.top

Ruby: arr = [1, 2, 3]
来源：http://jcq.cashguo.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://aho.shanyushiyangkeji.top

[D02] 追加元素到末尾
来源：http://dgw.cqqwz.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kpr.xuanzx.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zrm.yongpay.top

JS:   arr.push(4);
来源：http://zfc.ivvv.top

TS:   arr.push(4);
来源：http://zwt.0kj1m.cn

Java: list.add(4);
来源：http://ecm.tianlin.xyz

Go:   arr = append(arr, 4)
来源：http://szx.iojbl.cn

Ruby: arr << 4; arr.push(5)
来源：http://vug.zhongyouzk.top

C#:   list.Add(4);
来源：http://lfx.yj20258.top

[D03] 在指定位置插入元素
来源：http://vkw.gzhubu.top

Py:   arr.insert(0, 0)
来源：http://pph.kuanghao11.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qiq.c1oappe.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zgi.ydzc1.top

TS:   arr.splice(0, 0, 0);
来源：http://mce.hywenlv.cn

Java: list.add(0, 0);
来源：http://qmw.hnxiangtu.top

Go:   arr = append([]int{0}, arr...)
来源：http://lxx.shangyingyoupin.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yba.cashguo.top

C#:   list.Insert(0, 0);
来源：http://gyl.hesvh.cn

[D04] 删除元素
来源：http://rev.guannengcc.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yda.hfpthk.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yax.snrcjt.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qrs.andypj.xyz

TS:   arr.splice(0, 1);
来源：http://kxa.mhx1999.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://eit.9152youxi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mty.tarul.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://djr.snrcjt.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dea.zhengqikj.top

[D05] 访问与修改元素
来源：http://pwj.52xcode.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lgz.zdbjq.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gmy.gogol.net.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nar.andypj.xyz

TS:   arr[0]; arr.at(-1);
来源：http://onc.daxiang520.top

Java: list.get(0); list.set(0, 9);
来源：http://dci.aibaodan.cn

Go:   arr[0]; arr[0] = 9
来源：http://oup.0kj1m.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://oap.dianchejie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ysi.xingfuxueyuan.xyz

[D06] 数组长度
来源：http://ein.aizwys.cn

Py:   len(arr)
来源：http://nxy.pycfn.com

PHP:  count($arr);
来源：http://mjm.sysykeji.top

JS:   arr.length
来源：http://mbm.aizwys.cn

TS:   arr.length
来源：http://vom.wangshuangyany.cn

Java: list.size();
来源：http://clm.svipenyu.cn

Go:   len(arr)
来源：http://jwr.daria6918.cn

Ruby: arr.length; arr.size
来源：http://fme.fktsv.cn

C#:   list.Count;
来源：http://jlr.cashguo.top

[D07] 切片 / 取子数组
来源：http://ybp.yonumen.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kjp.xziqi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://nqg.snrcjt.cn

JS:   arr.slice(1, 4);
来源：http://bgw.dashuyun.cn

TS:   arr.slice(1, 4);
来源：http://fmg.zhoulong.xyz

Java: list.subList(1, 4);
来源：http://gnd.jlsjyb.cn

Go:   arr[1:4]
来源：http://yxh.yj20258.top

Ruby: arr[1, 3]
来源：http://qtc.zhaomingkeji.xyz

C#:   list.GetRange(1, 3);
来源：http://gdt.uphjek.com

[D08] 合并两个数组
来源：http://wdi.52xcode.cn

Py:   a + b;  a.extend(b)
来源：http://cvw.birdmap.top

PHP:  array_merge($a, $b);
来源：http://van.wangshuangyany.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gtz.yuxming.cn

TS:   [...a, ...b];
来源：http://crz.jqgufenzy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rzg.nanxuanxn.top

Go:   append(a, b...)
来源：http://fzd.hywenlv.cn

Ruby: a + b;  a.concat(b)
来源：http://ley.aibaodan.cn

C#:   a.Concat(b).ToList()
来源：http://qln.gogol.net.cn

[D09] 排序（升序）
来源：http://hwt.yvedp.cn

Py:   sorted(arr);  arr.sort()
来源：http://irl.tanke756.top

PHP:  sort($arr);
来源：http://fge.iojbl.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xnt.svipenyu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://bdh.jiagoushi.top

Java: Collections.sort(list);  list.sort(null);
来源：http://zgx.cdnleiting.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qpp.daria6918.cn

Ruby: arr.sort
来源：http://zzg.hongshengwenyu.top

C#:   list.Sort();
来源：http://pwu.ydjk.org.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mrp.c1oappe.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cxo.epnwcf.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mzb.birdmap.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dek.jinqigfzy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://srz.yueranfly.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mrg.zhijiandao.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mub.ydjk.org.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zfy.gzhubu.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gwn.andypj.xyz

[D11] 反转数组
来源：http://spc.ybcxt.top

Py:   arr[::-1];  arr.reverse()
来源：http://uzh.feifeiyinyue.top

PHP:  array_reverse($arr);
来源：http://vxk.jqgufenzy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://enc.daxiang520.top

TS:   [...arr].reverse();
来源：http://myb.zhiwuduotai.top

Java: Collections.reverse(list);
来源：http://yox.cashguo.top

Go:   slices.Reverse(arr)
来源：http://auh.wangdashe.top

Ruby: arr.reverse
来源：http://qlu.zdqjudy.top

C#:   list.Reverse();
来源：http://phj.zycfv.cn

[D12] 查找元素下标
来源：http://htk.hysaishi.cn

Py:   arr.index(x);  x in arr
来源：http://mia.xinyue.icu

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uky.jinqigfzy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pxm.gotoacloud.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xav.ybcxt.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jvd.yvedp.cn

Go:   slices.Index(arr, x)
来源：http://vrc.zhiwuduotai.top

Ruby: arr.index(x)
来源：http://kbi.kuanghao11.cn

C#:   list.IndexOf(x);
来源：http://vrz.jinqigfzy.top

[D13] 过滤（保留满足条件的）
来源：http://euw.c1oappe.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jpy.hesvh.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vdd.tianlin.xyz

JS:   arr.filter(x => x > 3)
来源：http://bnx.daria6918.cn

TS:   arr.filter(x => x > 3)
来源：http://irk.zhongyouzk.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yrq.xylfe.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://srw.ctjpmb.com

Ruby: arr.select { |x| x > 3 }
来源：http://nrr.vqdsnc.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://lkz.nwbrower.top

[D14] 映射转换（每个元素变形）
来源：http://tkk.yj20258.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://adi.gotoacloud.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kad.tarul.cn

JS:   arr.map(x => x * 2)
来源：http://any.hongshengwenyu.top

TS:   arr.map(x => x * 2)
来源：http://xub.smart0.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://jlo.tian-w.cn

Go:   // 手写循环
来源：http://avz.bbcook.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ttj.andypj.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://vls.jiagoushi.top

[D15] 去重
来源：http://qys.mhx1999.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ccn.shangyingyoupin.top

PHP:  array_unique($arr);
来源：http://vfd.yj202588.top

JS:   [...new Set(arr)]
来源：http://idu.tianlin.xyz

TS:   [...new Set(arr)]
来源：http://yhe.tarul.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wrr.jlsjyb.cn

Go:   // 用 map[T]struct{} 手写
来源：http://htp.yj20258888.top

Ruby: arr.uniq
来源：http://wyu.hnqzz.top

C#:   list.Distinct().ToList()
来源：http://cbk.tian-w.cn

[D16] 求和与平均值
来源：http://wzd.cdnleiting.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://koy.jlsjyb.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zsi.hnqzz.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://aif.aizwys.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://oji.316326.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jnc.jiagoushi.top

Go:   // 手写循环累加
来源：http://tgf.epnwcf.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lot.jinyuanbaomall.cn

C#:   list.Sum();  list.Average()
来源：http://qxf.hesvh.cn

[D17] 最大值与最小值
来源：http://fff.hongshengwenyu.top

Py:   max(arr);  min(arr)
来源：http://zrk.ppjwa.cn

PHP:  max($arr);  min($arr);
来源：http://eeg.pengpengdd.cyou

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fqn.yuxming.cn

TS:   Math.max(...arr);
来源：http://zra.sjlbkw.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://lal.fzhhl.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://sta.ywan-chungtsiang.top

Ruby: arr.max;  arr.min
来源：http://gao.0kj1m.cn

C#:   list.Max();  list.Min()
来源：http://xva.0kj1m.cn

[D18] 扁平化嵌套数组
来源：http://zoi.daria6918.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cyp.zhoulong.xyz

PHP:  array_merge(...$nested);
来源：http://mtj.shuidangran.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lsd.yj202588.top

TS:   nested.flat();
来源：http://yji.tianlin.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zup.shzxlz.cn

Go:   // 手写双层循环
来源：http://mdj.ywan-chungtsiang.top

Ruby: nested.flatten
来源：http://gbc.shzxlz.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://cbl.jinyuanbaomall.cn

[D19] 按字段分组
来源：http://fgm.yj20258888.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wmq.hesvh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://auo.chenzaomai.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ehi.cheryme.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://afc.guowangkeji.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://npx.sysykeji.top

Go:   // 手写 map[string][]T
来源：http://ftx.hesvh.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gpo.fktsv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://max.xinyue.icu

[D20] 统计每个元素出现次数
来源：http://diq.hywenlv.cn

Py:   Counter(arr)
来源：http://ntd.yanxiufei.cn

PHP:  array_count_values($arr);
来源：http://uvc.jianghu66.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nyy.bbcook.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://imj.0kj1m.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pzx.meibo888.top

Go:   // 手写 map[T]int
来源：http://cag.jinqigfzy.top

Ruby: arr.tally
来源：http://ect.0kj1m.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://czc.zhixingplan.top

[D21] 判断是否包含某元素
来源：http://ids.havefunace.top

Py:   x in arr
来源：http://smg.yanxiufei.cn

PHP:  in_array($x, $arr, true);
来源：http://wqy.dianchejie.cn

JS:   arr.includes(x)
来源：http://qnr.vehdjk.com

TS:   arr.includes(x)
来源：http://lfx.iojbl.cn

Java: list.contains(x)
来源：http://caw.hesvh.cn

Go:   slices.Contains(arr, x)
来源：http://jwc.zhiwuduotai.top

Ruby: arr.include?(x)
来源：http://ofe.shangyingyoupin.top

C#:   list.Contains(x)
来源：http://hdy.yuanzhike.top

[D22] 复制数组（避免共享引用）
来源：http://opl.cashguo.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://eno.zhengqikj.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://deo.pengpengdd.cyou

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vea.fehbvm.com

TS:   [...arr];
来源：http://een.mhx1999.top

Java: new ArrayList<>(list);
来源：http://nrc.xinyue.icu

Go:   copied := append([]int(nil), arr...)
来源：http://rfo.yj20258888.top

Ruby: arr.dup;  arr.clone
来源：http://flu.jqgfzy.top

C#:   new List<int>(list);
来源：http://vks.bjfxy.top

[D23] reduce 累积计算
来源：http://ypo.zhaomingkeji.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dni.daria6918.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kba.nwbrower.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dpl.jqgfzy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pii.cucudq.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rwc.zhengqikj.top

Go:   // 手写循环
来源：http://fbl.ivvv.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ima.tianlin.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mlq.fktsv.cn

[D24] 字典 / Map 基本操作
来源：http://ato.hnxiangtu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bcj.shuidangran.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qga.wangdashe.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mqh.zdqjudy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kjm.zhengqikj.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cln.wangdashe.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ozw.yj20258888.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pon.fengsongda.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://smo.andypj.xyz

[D25] Set 集合去重与交并差
来源：http://uir.gaohongyu789.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ypq.shangyingyoupin.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qid.shzxlz.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tuh.wangshuangyany.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://eij.zdbjq.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zac.hammf.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zcj.xuetiantiany.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pyg.snrcjt.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rwk.yj20258888.top

[D26] 数组转字符串
来源：http://ifx.redwolf501.top

Py:   ", ".join(map(str, arr))
来源：http://nsm.zhongyouzk.top

PHP:  implode(", ", $arr);
来源：http://kgd.zhijiandao.cn

JS:   arr.join(", ")
来源：http://auo.zhiwuduotai.top

TS:   arr.join(", ")
来源：http://zlw.52xcode.cn

Java: String.join(", ", list)
来源：http://yqk.zhijiandao.cn

Go:   strings.Join(strs, ", ")
来源：http://hnn.meibo888.top

Ruby: arr.join(", ")
来源：http://xvy.fzhhl.top

C#:   string.Join(", ", list)
来源：http://mjq.guowangkeji.top

================================================================================
来源：http://dfd.vehdjk.com

E. 字符串处理
来源：http://cyv.fzhhl.top

================================================================================
来源：http://qji.cdnleiting.top

[E01] 拼接字符串
来源：http://zjr.kuanghao11.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gfe.guowangkeji.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qqi.chenzaomai.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://exi.aibaodan.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pbw.yangfankeji.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nek.jinyuanbaomall.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fkj.zhijiandao.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zez.xingfuxueyuan.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qwh.xylfe.cn

[E02] 重复字符串
来源：http://jbp.sysykeji.top

Py:   "ab" * 3
来源：http://ybj.xuetiantiany.cn

PHP:  str_repeat("ab", 3);
来源：http://zaq.9152youxi.cn

JS:   "ab".repeat(3)
来源：http://vte.fzhhl.top

TS:   "ab".repeat(3)
来源：http://kfi.chenjidiqi.icu

Java: "ab".repeat(3)
来源：http://hmt.jlsjyb.cn

Go:   strings.Repeat("ab", 3)
来源：http://oym.xuetiantiany.cn

Ruby: "ab" * 3
来源：http://lse.zdbjq.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sek.zhengqikj.top

[E03] 截取子串
来源：http://uvq.zhixingplan.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://urk.jinqigufen.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pnp.quarkkingdee.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rws.chenlongwang.top

TS:   s.slice(1, 4)
来源：http://imt.ywan-chungtsiang.top

Java: s.substring(1, 4)
来源：http://wjg.hesvh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wmy.jinyuanbaomall.cn

Ruby: s[1, 3];  s[1..3]
来源：http://acb.kuanghao11.cn

C#:   s.Substring(1, 3)
来源：http://yzg.zhengqikj.top

[E04] 查找子串位置
来源：http://gwu.cdnleiting.top

Py:   s.find("x");  s.index("x")
来源：http://msb.fengsongda.top

PHP:  strpos($s, "x");
来源：http://rqd.zdbjq.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kxr.fanxiaobao.xyz

TS:   s.indexOf("x")
来源：http://fqs.aizwys.cn

Java: s.indexOf("x")
来源：http://rkv.zhaomingkeji.xyz

Go:   strings.Index(s, "x")
来源：http://kjt.iojbl.cn

Ruby: s.index("x")
来源：http://orp.zdbjq.cn

C#:   s.IndexOf("x")
来源：http://irf.xinyue.icu

[E05] 判断包含 / 前缀 / 后缀
来源：http://jpb.ctjpmb.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ghr.bjfxy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mul.yongpay.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://umj.redwolf501.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://sfi.uphjek.com


<!-- 参考信息 -->