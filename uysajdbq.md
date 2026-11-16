代发 wailian999

PHP:  // 无重载
来源：http://wdy.sjlbkw.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://jnc.hesvh.cn

TS:   // 用联合类型或重载签名声明
来源：http://bsi.daria6918.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://pbl.cashguo.top

Go:   // 无重载：用不同函数名
来源：http://khn.quarkkingdee.top

Ruby: # 无重载：靠动态参数
来源：http://mtz.xinyue.icu

C#:   void F(int a) {}  void F(string a) {}
来源：http://szp.shangyingyoupin.top

================================================================================
来源：http://pbs.yfazqb.com

D. 数组 / 列表 / 集合
来源：http://ekz.vqdsnc.cn

================================================================================
来源：http://rvp.zycfv.cn

[D01] 创建数组 / 列表
来源：http://wdq.nanxinkj.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://atq.fzhhl.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pnd.jinyuanbaomall.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fgo.jinqigufen.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://cbz.vehdjk.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blu.tian-w.cn

Go:   arr := []int{1, 2, 3}
来源：http://bxy.hesvh.cn

Ruby: arr = [1, 2, 3]
来源：http://azv.shangyingyoupin.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://umm.zhiwuduotai.top

[D02] 追加元素到末尾
来源：http://bzh.ydjk.org.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kbz.hesvh.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wqq.jlsjyb.cn

JS:   arr.push(4);
来源：http://bfe.hnqzz.top

TS:   arr.push(4);
来源：http://uac.zycfv.cn

Java: list.add(4);
来源：http://vlt.cdnleiting.top

Go:   arr = append(arr, 4)
来源：http://dux.vehdjk.com

Ruby: arr << 4; arr.push(5)
来源：http://ygu.ehwqpu.com

C#:   list.Add(4);
来源：http://vao.hcnkem.com

[D03] 在指定位置插入元素
来源：http://ltl.hywenlv.cn

Py:   arr.insert(0, 0)
来源：http://jtz.hesvh.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rer.yfazqb.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://glc.ctjpmb.com

TS:   arr.splice(0, 0, 0);
来源：http://jab.ybcxt.top

Java: list.add(0, 0);
来源：http://tmo.zycfv.cn

Go:   arr = append([]int{0}, arr...)
来源：http://mwg.fengsongda.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rym.jiagoushi.top

C#:   list.Insert(0, 0);
来源：http://utd.fehbvm.com

[D04] 删除元素
来源：http://ycn.zycfv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fyn.xuanzx.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bth.yueranfly.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ofn.yongpay.top

TS:   arr.splice(0, 1);
来源：http://jky.hammf.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zjq.xingfuxueyuan.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sus.tianlin.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mlr.fzhhl.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ndl.birdmap.top

[D05] 访问与修改元素
来源：http://dpq.cqqwz.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://azu.wangshuangyany.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xwo.xuanzx.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pfa.zhixingplan.top

TS:   arr[0]; arr.at(-1);
来源：http://nen.hywenlv.cn

Java: list.get(0); list.set(0, 9);
来源：http://riy.shangyingyoupin.top

Go:   arr[0]; arr[0] = 9
来源：http://aat.yfazqb.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://srl.xuetiantiany.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pbe.yj202588.top

[D06] 数组长度
来源：http://zxf.dianchejie.cn

Py:   len(arr)
来源：http://udc.fehbvm.com

PHP:  count($arr);
来源：http://vzn.wangshuangyany.cn

JS:   arr.length
来源：http://wld.smart0.xyz

TS:   arr.length
来源：http://fut.daxiang520.top

Java: list.size();
来源：http://qgs.9152youxi.cn

Go:   len(arr)
来源：http://ihm.jinqigfzy.top

Ruby: arr.length; arr.size
来源：http://day.xingfuxueyuan.xyz

C#:   list.Count;
来源：http://ybb.jianghu66.top

[D07] 切片 / 取子数组
来源：http://abr.ydzc1.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qff.wangshuangyany.cn

PHP:  array_slice($arr, 1, 3);
来源：http://bxb.316326.xyz

JS:   arr.slice(1, 4);
来源：http://pex.gzhubu.top

TS:   arr.slice(1, 4);
来源：http://xva.smart0.xyz

Java: list.subList(1, 4);
来源：http://tvq.zhengqikj.top

Go:   arr[1:4]
来源：http://pzw.wangdashe.top

Ruby: arr[1, 3]
来源：http://ooz.hongshengwenyu.top

C#:   list.GetRange(1, 3);
来源：http://klc.svipenyu.cn

[D08] 合并两个数组
来源：http://vmd.mhx1999.top

Py:   a + b;  a.extend(b)
来源：http://hav.gotoacloud.top

PHP:  array_merge($a, $b);
来源：http://wrh.yj20258888.top

JS:   [...a, ...b];  a.concat(b);
来源：http://agf.zhoulong.xyz

TS:   [...a, ...b];
来源：http://ecs.hongshengwenyu.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xvh.jinqigfzy.top

Go:   append(a, b...)
来源：http://wxn.epnwcf.com

Ruby: a + b;  a.concat(b)
来源：http://kix.zhongyouzk.top

C#:   a.Concat(b).ToList()
来源：http://ypj.ehwqpu.com

[D09] 排序（升序）
来源：http://voq.ydjk.org.cn

Py:   sorted(arr);  arr.sort()
来源：http://jmt.bbcook.cn

PHP:  sort($arr);
来源：http://jhv.zhiwuduotai.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://azh.hfpthk.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xhd.hesvh.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rdn.jianghu66.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zpd.zdqjudy.top

Ruby: arr.sort
来源：http://mrg.zhoulong.xyz

C#:   list.Sort();
来源：http://azl.bjfxy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://hbj.yj20258.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dac.uphjek.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pro.hnqzz.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hft.birdmap.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ury.daxiang520.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jzj.aibaodan.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://twj.zhongyouzk.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ruh.shzxlz.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://iqb.jinyuanbaomall.cn

[D11] 反转数组
来源：http://ues.quarkkingdee.top

Py:   arr[::-1];  arr.reverse()
来源：http://lhp.wangshuangyany.cn

PHP:  array_reverse($arr);
来源：http://orl.ppjwa.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://awv.feifeiyinyue.top

TS:   [...arr].reverse();
来源：http://zfa.hfpthk.cn

Java: Collections.reverse(list);
来源：http://efj.yfazqb.com

Go:   slices.Reverse(arr)
来源：http://qrj.cqqwz.cn

Ruby: arr.reverse
来源：http://ags.tarul.cn

C#:   list.Reverse();
来源：http://fxs.yueranfly.top

[D12] 查找元素下标
来源：http://wje.andypj.xyz

Py:   arr.index(x);  x in arr
来源：http://dsq.smart0.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://oqq.haohaochexian.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tuy.chenlongwang.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wve.jqgfzy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vdu.wangdashe.top

Go:   slices.Index(arr, x)
来源：http://rta.snrcjt.cn

Ruby: arr.index(x)
来源：http://fma.xziqi.cn

C#:   list.IndexOf(x);
来源：http://hpj.gogol.net.cn

[D13] 过滤（保留满足条件的）
来源：http://uia.ivvv.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vvz.zhongyouzk.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lkq.zhengqikj.top

JS:   arr.filter(x => x > 3)
来源：http://yjp.yj20258888.top

TS:   arr.filter(x => x > 3)
来源：http://ljx.jiagoushi.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://sey.sufxvd.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qze.tianlin.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://ily.tian-w.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bil.fengsongda.top

[D14] 映射转换（每个元素变形）
来源：http://jmr.yj20258.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jze.bbcook.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ftx.fehbvm.com

JS:   arr.map(x => x * 2)
来源：http://uck.jyoumei.cn

TS:   arr.map(x => x * 2)
来源：http://irm.guowangkeji.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://dlv.yangfankeji.com

Go:   // 手写循环
来源：http://gyz.shuidangran.top

Ruby: arr.map { |x| x * 2 }
来源：http://zvu.shanyushiyangtech.top

C#:   list.Select(x => x * 2).ToList()
来源：http://phq.fktsv.cn

[D15] 去重
来源：http://dum.ybcxt.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qvf.jlsjyb.cn

PHP:  array_unique($arr);
来源：http://fpv.gaohongyu789.top

JS:   [...new Set(arr)]
来源：http://atj.fktsv.cn

TS:   [...new Set(arr)]
来源：http://tny.nanxinkj.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://iea.zhongyouzk.top

Go:   // 用 map[T]struct{} 手写
来源：http://exp.zycfv.cn

Ruby: arr.uniq
来源：http://fun.yueranfly.top

C#:   list.Distinct().ToList()
来源：http://kpl.guowangkeji.top

[D16] 求和与平均值
来源：http://vxt.gogol.net.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hna.yangfankeji.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bqg.fengsongda.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gmo.ctjpmb.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wsp.aizwys.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fkk.c1oappe.top

Go:   // 手写循环累加
来源：http://bww.yangfankeji.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nkh.ehwqpu.com

C#:   list.Sum();  list.Average()
来源：http://snj.gogol.net.cn

[D17] 最大值与最小值
来源：http://rwa.zhengqikj.top

Py:   max(arr);  min(arr)
来源：http://cmf.aizwys.cn

PHP:  max($arr);  min($arr);
来源：http://rlj.sweek.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ikw.aizwys.cn

TS:   Math.max(...arr);
来源：http://exe.hywenlv.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://uda.xinyue.icu

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vlo.vqdsnc.cn

Ruby: arr.max;  arr.min
来源：http://sca.daria6918.cn

C#:   list.Max();  list.Min()
来源：http://owq.zdbjq.cn

[D18] 扁平化嵌套数组
来源：http://ghh.fzhhl.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pow.cucudq.cn

PHP:  array_merge(...$nested);
来源：http://xyv.zhixingplan.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vfu.ywan-chungtsiang.top

TS:   nested.flat();
来源：http://vcl.iojbl.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hdm.sweek.top

Go:   // 手写双层循环
来源：http://nmn.xinyue.icu

Ruby: nested.flatten
来源：http://zcv.yj20258888.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://yzy.haohaochexian.top

[D19] 按字段分组
来源：http://qte.316326.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mbj.kuanghao11.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mkk.jyoumei.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://obu.yj20258.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://jyt.xinyue.icu

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vgx.jinyuanbaomall.cn

Go:   // 手写 map[string][]T
来源：http://rio.316326.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://gbm.ydzc1.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lob.ppjwa.cn

[D20] 统计每个元素出现次数
来源：http://qgb.bbcook.cn

Py:   Counter(arr)
来源：http://dvp.pengpengdd.cyou

PHP:  array_count_values($arr);
来源：http://ber.zycfv.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yej.sufxvd.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bas.iojbl.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cfi.cashguo.top

Go:   // 手写 map[T]int
来源：http://ewr.0kj1m.cn

Ruby: arr.tally
来源：http://tpi.nwbrower.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ytq.9152youxi.cn

[D21] 判断是否包含某元素
来源：http://rvk.0kj1m.cn

Py:   x in arr
来源：http://jva.svipenyu.cn

PHP:  in_array($x, $arr, true);
来源：http://hwl.sweek.top

JS:   arr.includes(x)
来源：http://jhy.jyoumei.cn

TS:   arr.includes(x)
来源：http://bdm.gzhubu.top

Java: list.contains(x)
来源：http://vfc.xuetiantiany.cn

Go:   slices.Contains(arr, x)
来源：http://sbp.tian-w.cn

Ruby: arr.include?(x)
来源：http://rxi.uphjek.com

C#:   list.Contains(x)
来源：http://eqh.ydjk.org.cn

[D22] 复制数组（避免共享引用）
来源：http://njk.sufxvd.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tcl.xuetiantiany.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tvf.yanxiufei.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://huw.yj202588.top

TS:   [...arr];
来源：http://imz.xinyue.icu

Java: new ArrayList<>(list);
来源：http://hzy.haohaochexian.top

Go:   copied := append([]int(nil), arr...)
来源：http://rbp.feifeiyinyue.top

Ruby: arr.dup;  arr.clone
来源：http://ust.yj202588.top

C#:   new List<int>(list);
来源：http://nmv.sysykeji.top

[D23] reduce 累积计算
来源：http://txb.zhiwuduotai.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://arr.fzhhl.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zps.shzxlz.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ivv.yuanzhike.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ivc.guowangkeji.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://auz.sweek.top

Go:   // 手写循环
来源：http://uaw.vqdsnc.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ghb.quarkkingdee.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kwv.aizwys.cn

[D24] 字典 / Map 基本操作
来源：http://olk.zhoulong.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rov.9152youxi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qxk.zhaomingkeji.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ltz.chenlongwang.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jmp.zhaomingkeji.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lii.316326.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lkz.ydzc1.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dzq.chenjidiqi.icu

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lza.jianghu66.top

[D25] Set 集合去重与交并差
来源：http://sap.sufxvd.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mzm.svipenyu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dou.sufxvd.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xzv.cucudq.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bqq.guannengcc.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kea.kuanghao11.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://oqv.gzhubu.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uib.zhongyouzk.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kdj.gotoacloud.top

[D26] 数组转字符串
来源：http://cni.jinyuanbaomall.cn

Py:   ", ".join(map(str, arr))
来源：http://wvj.gotoacloud.top

PHP:  implode(", ", $arr);
来源：http://zaq.316326.xyz

JS:   arr.join(", ")
来源：http://rer.chenzaomai.com

TS:   arr.join(", ")
来源：http://gti.ydzc1.top

Java: String.join(", ", list)
来源：http://pet.xinyue.icu

Go:   strings.Join(strs, ", ")
来源：http://wms.sysykeji.top

Ruby: arr.join(", ")
来源：http://axs.zhengqikj.top

C#:   string.Join(", ", list)
来源：http://nos.ybcxt.top

================================================================================
来源：http://ulq.gotoacloud.top

E. 字符串处理
来源：http://lza.xuetiantiany.cn

================================================================================
来源：http://luu.havefunace.top

[E01] 拼接字符串
来源：http://ttg.52xcode.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ahf.cdnleiting.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xqt.daria6918.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://acp.fzhhl.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zcb.gaohongyu789.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://swp.316326.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wkx.nwbrower.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xud.chenjidiqi.icu

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://scp.shzxlz.cn

[E02] 重复字符串
来源：http://zoz.uphjek.com

Py:   "ab" * 3
来源：http://kkh.feifeiyinyue.top

PHP:  str_repeat("ab", 3);
来源：http://wjo.ydzc1.top

JS:   "ab".repeat(3)
来源：http://ucy.hywenlv.cn

TS:   "ab".repeat(3)
来源：http://pww.xuanzx.com

Java: "ab".repeat(3)
来源：http://luq.chenlongwang.top

Go:   strings.Repeat("ab", 3)
来源：http://fbf.hfpthk.cn

Ruby: "ab" * 3
来源：http://nox.jlsjyb.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wqi.9152youxi.cn

[E03] 截取子串
来源：http://wuo.birdmap.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://imw.jianghu66.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kqu.dianchejie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jwk.jinghuilouyu.cn

TS:   s.slice(1, 4)
来源：http://zmo.guannengcc.top

Java: s.substring(1, 4)
来源：http://vem.zhijiandao.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://thf.jyoumei.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ssh.nanxinkj.top

C#:   s.Substring(1, 3)
来源：http://eym.ivvv.top

[E04] 查找子串位置
来源：http://awl.wangdashe.top

Py:   s.find("x");  s.index("x")
来源：http://laa.xinyue.icu

PHP:  strpos($s, "x");
来源：http://rqj.zdbjq.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zhr.jianghu66.top

TS:   s.indexOf("x")
来源：http://sez.ydzc1.top

Java: s.indexOf("x")
来源：http://ttu.yvedp.cn

Go:   strings.Index(s, "x")
来源：http://irn.zycfv.cn

Ruby: s.index("x")
来源：http://gfi.hcnkem.com

C#:   s.IndexOf("x")
来源：http://uya.xingfuxueyuan.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://qpk.tanke756.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cnp.jiagoushi.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jia.shuidangran.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xgn.dashuyun.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://goi.wangshuangyany.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mgu.haohaochexian.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pza.tianlin.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sxj.hnxiangtu.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tdx.daria6918.cn

[E06] 替换子串
来源：http://wuv.fktsv.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wgh.wangdashe.top

PHP:  str_replace("a", "b", $s);
来源：http://erd.gogol.net.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://irj.pycfn.com

TS:   s.replaceAll("a", "b")
来源：http://qma.pengpengdd.cyou

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cnb.ydzc1.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rjr.fengsongda.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://eal.fzhhl.top


<!-- 参考信息 -->