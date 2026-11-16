代发 wailian999

PHP:  // 无重载
来源：http://qae.ehwqpu.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://pxa.fengsongda.top

TS:   // 用联合类型或重载签名声明
来源：http://bni.quarkkingdee.top

Java: void f(int a) {}  void f(String a) {}
来源：http://yae.jinqigufen.top

Go:   // 无重载：用不同函数名
来源：http://xjv.fktsv.cn

Ruby: # 无重载：靠动态参数
来源：http://bef.yj20258888.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://qzg.yuanzhike.top

================================================================================
来源：http://csu.shuidangran.top

D. 数组 / 列表 / 集合
来源：http://sze.pycfn.com

================================================================================
来源：http://gty.fktsv.cn

[D01] 创建数组 / 列表
来源：http://yhj.andypj.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://pkw.cqqwz.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nxt.feifeiyinyue.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hbo.smart0.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://avf.tarul.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://oss.quarkkingdee.top

Go:   arr := []int{1, 2, 3}
来源：http://ymj.xuetiantiany.cn

Ruby: arr = [1, 2, 3]
来源：http://eqw.yvedp.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yor.vehdjk.com

[D02] 追加元素到末尾
来源：http://yqk.ybcxt.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pje.redwolf501.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fom.jyoumei.cn

JS:   arr.push(4);
来源：http://eij.hfpthk.cn

TS:   arr.push(4);
来源：http://jue.chenlongwang.top

Java: list.add(4);
来源：http://ogq.hesvh.cn

Go:   arr = append(arr, 4)
来源：http://ehf.aizwys.cn

Ruby: arr << 4; arr.push(5)
来源：http://zcq.redwolf501.top

C#:   list.Add(4);
来源：http://tsd.hysaishi.cn

[D03] 在指定位置插入元素
来源：http://mdi.quarkkingdee.top

Py:   arr.insert(0, 0)
来源：http://hbm.xingfuxueyuan.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dct.andypj.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hxc.sysykeji.top

TS:   arr.splice(0, 0, 0);
来源：http://irw.kuanghao11.cn

Java: list.add(0, 0);
来源：http://sku.9152youxi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ivb.yanxiufei.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://czn.havefunace.top

C#:   list.Insert(0, 0);
来源：http://scw.zdqjudy.top

[D04] 删除元素
来源：http://ctl.cheryme.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ape.jinyuanbaomall.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bxf.pycfn.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rli.jyoumei.cn

TS:   arr.splice(0, 1);
来源：http://xrv.xuanzx.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kdl.aizwys.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://njg.sjlbkw.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zma.iojbl.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uor.bjfxy.top

[D05] 访问与修改元素
来源：http://ryi.vehdjk.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wmi.jianghu66.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mcw.zhengqikj.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vex.yuxming.cn

TS:   arr[0]; arr.at(-1);
来源：http://oqi.tarul.cn

Java: list.get(0); list.set(0, 9);
来源：http://fid.kuanghao11.cn

Go:   arr[0]; arr[0] = 9
来源：http://mre.cdnleiting.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bgf.uphjek.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hem.tianlin.xyz

[D06] 数组长度
来源：http://tgc.zdqjudy.top

Py:   len(arr)
来源：http://zwi.fengsongda.top

PHP:  count($arr);
来源：http://aox.shangyingyoupin.top

JS:   arr.length
来源：http://uaq.52xcode.cn

TS:   arr.length
来源：http://qfi.sweek.top

Java: list.size();
来源：http://yly.mhx1999.top

Go:   len(arr)
来源：http://zfn.pengpengdd.cyou

Ruby: arr.length; arr.size
来源：http://zft.feifeiyinyue.top

C#:   list.Count;
来源：http://xsj.shangyingyoupin.top

[D07] 切片 / 取子数组
来源：http://qjw.iojbl.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://awi.ivvv.top

PHP:  array_slice($arr, 1, 3);
来源：http://ltl.zhongyouzk.top

JS:   arr.slice(1, 4);
来源：http://uks.ydzc1.top

TS:   arr.slice(1, 4);
来源：http://gsh.fanxiaobao.xyz

Java: list.subList(1, 4);
来源：http://esx.yangfankeji.com

Go:   arr[1:4]
来源：http://rwr.smart0.xyz

Ruby: arr[1, 3]
来源：http://ful.uphjek.com

C#:   list.GetRange(1, 3);
来源：http://rrb.birdmap.top

[D08] 合并两个数组
来源：http://jmd.0kj1m.cn

Py:   a + b;  a.extend(b)
来源：http://mdv.ivvv.top

PHP:  array_merge($a, $b);
来源：http://vlt.fehbvm.com

JS:   [...a, ...b];  a.concat(b);
来源：http://hef.kuanghao11.cn

TS:   [...a, ...b];
来源：http://rrt.meibo888.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://knt.zycfv.cn

Go:   append(a, b...)
来源：http://dja.jianghu66.top

Ruby: a + b;  a.concat(b)
来源：http://eeh.shanyushiyangkeji.top

C#:   a.Concat(b).ToList()
来源：http://flv.jiagoushi.top

[D09] 排序（升序）
来源：http://aue.jlsjyb.cn

Py:   sorted(arr);  arr.sort()
来源：http://say.tianlin.xyz

PHP:  sort($arr);
来源：http://zpy.haohaochexian.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://crf.yanxiufei.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://zay.shangyingyoupin.top

Java: Collections.sort(list);  list.sort(null);
来源：http://zzp.gogol.net.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nxj.chenzaomai.com

Ruby: arr.sort
来源：http://bri.ctjpmb.com

C#:   list.Sort();
来源：http://ofg.hammf.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://gop.yonumen.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rqp.ivvv.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bfp.sjlbkw.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hfg.hywenlv.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dlk.yvedp.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zcv.sweek.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://aao.chenjidiqi.icu

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qrw.feifeiyinyue.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ajf.fzhhl.top

[D11] 反转数组
来源：http://ent.wangdashe.top

Py:   arr[::-1];  arr.reverse()
来源：http://thc.sysykeji.top

PHP:  array_reverse($arr);
来源：http://bzg.redwolf501.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tyx.shuidangran.top

TS:   [...arr].reverse();
来源：http://ifc.ehwqpu.com

Java: Collections.reverse(list);
来源：http://xwv.zdbjq.cn

Go:   slices.Reverse(arr)
来源：http://okw.zdbjq.cn

Ruby: arr.reverse
来源：http://ooe.epnwcf.com

C#:   list.Reverse();
来源：http://wwu.quarkkingdee.top

[D12] 查找元素下标
来源：http://nko.hnxiangtu.top

Py:   arr.index(x);  x in arr
来源：http://phq.gaohongyu789.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://djd.yvedp.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://grp.yj20258888.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kro.gaohongyu789.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wof.bbcook.cn

Go:   slices.Index(arr, x)
来源：http://hwj.xinyue.icu

Ruby: arr.index(x)
来源：http://yid.cucudq.cn

C#:   list.IndexOf(x);
来源：http://rkk.xuetiantiany.cn

[D13] 过滤（保留满足条件的）
来源：http://sdr.yfazqb.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zvy.haohaochexian.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zch.dianchejie.cn

JS:   arr.filter(x => x > 3)
来源：http://ssq.tianlin.xyz

TS:   arr.filter(x => x > 3)
来源：http://ogg.jinyuanbaomall.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ovf.nanxinkj.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wmm.ppjwa.cn

Ruby: arr.select { |x| x > 3 }
来源：http://lsf.xziqi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wew.cheryme.top

[D14] 映射转换（每个元素变形）
来源：http://bur.nanxuanxn.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pdt.zhixingplan.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ukk.fengsongda.top

JS:   arr.map(x => x * 2)
来源：http://qnc.quarkkingdee.top

TS:   arr.map(x => x * 2)
来源：http://jwg.tian-w.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ppd.tian-w.cn

Go:   // 手写循环
来源：http://fgy.yanxiufei.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fws.xylfe.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://nqy.havefunace.top

[D15] 去重
来源：http://mmv.sxryk.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dlf.jinghuilouyu.cn

PHP:  array_unique($arr);
来源：http://nyx.hywenlv.cn

JS:   [...new Set(arr)]
来源：http://bet.epnwcf.com

TS:   [...new Set(arr)]
来源：http://fmw.zhengqikj.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hmx.shangyingyoupin.top

Go:   // 用 map[T]struct{} 手写
来源：http://bcx.tianlin.xyz

Ruby: arr.uniq
来源：http://mhe.yuanzhike.top

C#:   list.Distinct().ToList()
来源：http://ikz.zdqjudy.top

[D16] 求和与平均值
来源：http://zni.svipenyu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://npb.epnwcf.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rhb.zycfv.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vht.fanxiaobao.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ezp.ivvv.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://eqe.yj20258.top

Go:   // 手写循环累加
来源：http://fdc.tianlin.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yls.zhongyouzk.top

C#:   list.Sum();  list.Average()
来源：http://sro.yuanzhike.top

[D17] 最大值与最小值
来源：http://tvw.hongshengwenyu.top

Py:   max(arr);  min(arr)
来源：http://xyo.xuetiantiany.cn

PHP:  max($arr);  min($arr);
来源：http://zxw.fzhhl.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rgo.iojbl.cn

TS:   Math.max(...arr);
来源：http://gtm.chenzaomai.com

Java: Collections.max(list);  Collections.min(list);
来源：http://shs.yj202588.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ccc.yj202588.top

Ruby: arr.max;  arr.min
来源：http://qzq.guannengcc.top

C#:   list.Max();  list.Min()
来源：http://chm.bjfxy.top

[D18] 扁平化嵌套数组
来源：http://wuh.jqgfzy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://liq.uphjek.com

PHP:  array_merge(...$nested);
来源：http://zol.hongshengwenyu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ahx.nanxuanxn.top

TS:   nested.flat();
来源：http://ooj.hywenlv.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jxl.hnqzz.top

Go:   // 手写双层循环
来源：http://hhk.vqdsnc.cn

Ruby: nested.flatten
来源：http://cts.sweek.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://udb.ppjwa.cn

[D19] 按字段分组
来源：http://qye.hammf.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://adx.fehbvm.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ucv.tianlin.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xhv.aizwys.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://flq.zhoulong.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yph.vqdsnc.cn

Go:   // 手写 map[string][]T
来源：http://hnq.gzhubu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://fjs.sysykeji.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wgq.kuanghao11.cn

[D20] 统计每个元素出现次数
来源：http://pmf.c1oappe.top

Py:   Counter(arr)
来源：http://ofe.jinyuanbaomall.cn

PHP:  array_count_values($arr);
来源：http://dzy.nanxuanxn.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fqw.hnqzz.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gck.nanxinkj.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ufy.zhijiandao.cn

Go:   // 手写 map[T]int
来源：http://uya.fehbvm.com

Ruby: arr.tally
来源：http://srr.ppjwa.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://woo.jqgfzy.top

[D21] 判断是否包含某元素
来源：http://ncu.yueranfly.top

Py:   x in arr
来源：http://zhh.jinyuanbaomall.cn

PHP:  in_array($x, $arr, true);
来源：http://imr.jinqigfzy.top

JS:   arr.includes(x)
来源：http://iue.sysykeji.top

TS:   arr.includes(x)
来源：http://lgd.xylfe.cn

Java: list.contains(x)
来源：http://mzb.xylfe.cn

Go:   slices.Contains(arr, x)
来源：http://qpt.shzxlz.cn

Ruby: arr.include?(x)
来源：http://dcb.yj20258.top

C#:   list.Contains(x)
来源：http://bag.jyoumei.cn

[D22] 复制数组（避免共享引用）
来源：http://gyp.yfazqb.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://edr.vqdsnc.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jbj.bbcook.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ecx.daria6918.cn

TS:   [...arr];
来源：http://sap.cdnleiting.top

Java: new ArrayList<>(list);
来源：http://qip.nwbrower.top

Go:   copied := append([]int(nil), arr...)
来源：http://cso.xinyue.icu

Ruby: arr.dup;  arr.clone
来源：http://ard.dashuyun.cn

C#:   new List<int>(list);
来源：http://qxg.chenlongwang.top

[D23] reduce 累积计算
来源：http://jxk.daria6918.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xge.jlsjyb.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kvk.fzhhl.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gig.jyoumei.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wzi.wangshuangyany.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qku.nanxuanxn.top

Go:   // 手写循环
来源：http://lqv.tian-w.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vhz.9152youxi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lxn.kuanghao11.cn

[D24] 字典 / Map 基本操作
来源：http://ctz.xziqi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cbv.pengpengdd.cyou

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hvl.dianchejie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nij.chenlongwang.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gcl.dianchejie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rue.fehbvm.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://llb.yangfankeji.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tjv.jyoumei.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vhz.bjfxy.top

[D25] Set 集合去重与交并差
来源：http://nuk.ydzc1.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://utb.nwbrower.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://czv.epnwcf.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ayw.jiagoushi.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fge.hongshengwenyu.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hfn.gogol.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://msl.hnxiangtu.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://atm.sysykeji.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bls.redwolf501.top

[D26] 数组转字符串
来源：http://put.jiagoushi.top

Py:   ", ".join(map(str, arr))
来源：http://qjq.fanxiaobao.xyz

PHP:  implode(", ", $arr);
来源：http://wgf.fengsongda.top

JS:   arr.join(", ")
来源：http://huw.sxryk.cn

TS:   arr.join(", ")
来源：http://nou.tian-w.cn

Java: String.join(", ", list)
来源：http://ldt.yonumen.top

Go:   strings.Join(strs, ", ")
来源：http://qjp.sxryk.cn

Ruby: arr.join(", ")
来源：http://sap.shuidangran.top

C#:   string.Join(", ", list)
来源：http://ers.hnxiangtu.top

================================================================================
来源：http://czs.smart0.xyz

E. 字符串处理
来源：http://pgb.yanxiufei.cn

================================================================================
来源：http://fgo.chenzaomai.com

[E01] 拼接字符串
来源：http://rzy.tianlin.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fiq.ybcxt.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gop.ywan-chungtsiang.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tzu.chenjidiqi.icu

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ohe.tianlin.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zvo.wangdashe.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xyh.hesvh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bqu.dianchejie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ipe.hnxiangtu.top

[E02] 重复字符串
来源：http://bwg.yonumen.top

Py:   "ab" * 3
来源：http://wxj.zdbjq.cn

PHP:  str_repeat("ab", 3);
来源：http://oek.nanxuanxn.top

JS:   "ab".repeat(3)
来源：http://asl.ctjpmb.com

TS:   "ab".repeat(3)
来源：http://aqe.hongshengwenyu.top

Java: "ab".repeat(3)
来源：http://wct.nanxinkj.top

Go:   strings.Repeat("ab", 3)
来源：http://kun.jinyuanbaomall.cn

Ruby: "ab" * 3
来源：http://gwp.jlsjyb.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gxw.yfazqb.com

[E03] 截取子串
来源：http://eif.jlsjyb.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hmj.52xcode.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ujm.hammf.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://uax.pengpengdd.cyou

TS:   s.slice(1, 4)
来源：http://uxi.yj20258.top

Java: s.substring(1, 4)
来源：http://iez.yueranfly.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://etx.fehbvm.com

Ruby: s[1, 3];  s[1..3]
来源：http://gvs.aibaodan.cn

C#:   s.Substring(1, 3)
来源：http://ngz.chenjidiqi.icu

[E04] 查找子串位置
来源：http://soo.jinghuilouyu.cn

Py:   s.find("x");  s.index("x")
来源：http://afa.ydjk.org.cn

PHP:  strpos($s, "x");
来源：http://imr.jinqigfzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xff.nwbrower.top

TS:   s.indexOf("x")
来源：http://ehu.meibo888.top

Java: s.indexOf("x")
来源：http://wrx.jyoumei.cn

Go:   strings.Index(s, "x")
来源：http://dwo.daria6918.cn

Ruby: s.index("x")
来源：http://qvt.pycfn.com

C#:   s.IndexOf("x")
来源：http://oqw.chenjidiqi.icu

[E05] 判断包含 / 前缀 / 后缀
来源：http://lay.xuanzx.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pys.zdbjq.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ozj.chenlongwang.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://stu.yanxiufei.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://daj.zhiwuduotai.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ldj.mhx1999.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vck.nwbrower.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fff.meibo888.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://edi.fanxiaobao.xyz

[E06] 替换子串
来源：http://yik.sxryk.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jkm.ppjwa.cn

PHP:  str_replace("a", "b", $s);
来源：http://fax.cqqwz.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dnt.yj20258.top

TS:   s.replaceAll("a", "b")
来源：http://ytg.shzxlz.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zvc.daxiang520.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xls.sweek.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wdw.yuanzhike.top


<!-- 参考信息 -->