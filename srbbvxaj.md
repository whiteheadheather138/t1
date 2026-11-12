代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://rue.hcnkem.com

Ruby: # 无重载：靠动态参数
来源：http://epz.svipenyu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://uhm.ydjk.org.cn

================================================================================
来源：http://ytz.svipenyu.cn

D. 数组 / 列表 / 集合
来源：http://wks.yj20258.top

================================================================================
来源：http://ial.cqqwz.cn

[D01] 创建数组 / 列表
来源：http://pfr.ybcxt.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://kiz.guowangkeji.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://uht.zdqjudy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ino.smart0.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://qaj.yonumen.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lck.yuanzhike.top

Go:   arr := []int{1, 2, 3}
来源：http://hng.shangyingyoupin.top

Ruby: arr = [1, 2, 3]
来源：http://wug.52xcode.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rgk.nwbrower.top

[D02] 追加元素到末尾
来源：http://kyd.aizwys.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mmd.316326.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nrj.yfazqb.com

JS:   arr.push(4);
来源：http://zvx.gotoacloud.top

TS:   arr.push(4);
来源：http://rrt.ehwqpu.com

Java: list.add(4);
来源：http://zsp.yfazqb.com

Go:   arr = append(arr, 4)
来源：http://zhi.zycfv.cn

Ruby: arr << 4; arr.push(5)
来源：http://puj.xingfuxueyuan.xyz

C#:   list.Add(4);
来源：http://jga.shanyushiyangkeji.top

[D03] 在指定位置插入元素
来源：http://nkp.zhaomingkeji.xyz

Py:   arr.insert(0, 0)
来源：http://rkg.vqdsnc.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zcl.zhixingplan.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lqj.fanxiaobao.xyz

TS:   arr.splice(0, 0, 0);
来源：http://mqi.52xcode.cn

Java: list.add(0, 0);
来源：http://hbp.fktsv.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vjc.haohaochexian.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zrg.tanke756.top

C#:   list.Insert(0, 0);
来源：http://nrt.hesvh.cn

[D04] 删除元素
来源：http://lsq.nwbrower.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://odt.dashuyun.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gmc.pycfn.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://aoo.fzhhl.top

TS:   arr.splice(0, 1);
来源：http://ygz.sjlbkw.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vqk.kuanghao11.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vyl.gogol.net.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ttr.meibo888.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jgf.jianghu66.top

[D05] 访问与修改元素
来源：http://xfq.jinghuilouyu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://njc.vqdsnc.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nyu.sysykeji.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://oik.jyoumei.cn

TS:   arr[0]; arr.at(-1);
来源：http://qcs.nanxuanxn.top

Java: list.get(0); list.set(0, 9);
来源：http://tkq.wangshuangyany.cn

Go:   arr[0]; arr[0] = 9
来源：http://yqr.yueranfly.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lrz.zhaomingkeji.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fch.yanxiufei.cn

[D06] 数组长度
来源：http://iva.c1oappe.top

Py:   len(arr)
来源：http://qpv.0kj1m.cn

PHP:  count($arr);
来源：http://nga.zhongyouzk.top

JS:   arr.length
来源：http://hpc.aibaodan.cn

TS:   arr.length
来源：http://zny.jinqigfzy.top

Java: list.size();
来源：http://jgq.bbcook.cn

Go:   len(arr)
来源：http://alq.52xcode.cn

Ruby: arr.length; arr.size
来源：http://bya.vqdsnc.cn

C#:   list.Count;
来源：http://ujz.cucudq.cn

[D07] 切片 / 取子数组
来源：http://fyy.xingfuxueyuan.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fdz.zdbjq.cn

PHP:  array_slice($arr, 1, 3);
来源：http://bfn.jinqigfzy.top

JS:   arr.slice(1, 4);
来源：http://keo.pengpengdd.cyou

TS:   arr.slice(1, 4);
来源：http://adn.hnxiangtu.top

Java: list.subList(1, 4);
来源：http://yli.zhongyouzk.top

Go:   arr[1:4]
来源：http://wca.9152youxi.cn

Ruby: arr[1, 3]
来源：http://vrd.yuanzhike.top

C#:   list.GetRange(1, 3);
来源：http://bce.jinqigufen.top

[D08] 合并两个数组
来源：http://iiw.snrcjt.cn

Py:   a + b;  a.extend(b)
来源：http://esd.guowangkeji.top

PHP:  array_merge($a, $b);
来源：http://uxi.daria6918.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://uyq.havefunace.top

TS:   [...a, ...b];
来源：http://wmw.yvedp.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gdx.gzhubu.top

Go:   append(a, b...)
来源：http://nsk.yj20258888.top

Ruby: a + b;  a.concat(b)
来源：http://nbx.zdqjudy.top

C#:   a.Concat(b).ToList()
来源：http://roa.jqgufenzy.top

[D09] 排序（升序）
来源：http://jxk.smart0.xyz

Py:   sorted(arr);  arr.sort()
来源：http://rzd.jinyuanbaomall.cn

PHP:  sort($arr);
来源：http://ttt.hfpthk.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kmt.yfazqb.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://hut.smart0.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://ktz.xingfuxueyuan.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://del.vqdsnc.cn

Ruby: arr.sort
来源：http://dei.jianghu66.top

C#:   list.Sort();
来源：http://vao.tanke756.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://bkw.xingfuxueyuan.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mpw.shuidangran.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vap.yuanzhike.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qlr.uphjek.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kgm.aizwys.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://iws.hfpthk.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://eld.jinqigufen.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ryl.jyoumei.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yxs.fzhhl.top

[D11] 反转数组
来源：http://vgb.jinghuilouyu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://sje.hysaishi.cn

PHP:  array_reverse($arr);
来源：http://ruc.fanxiaobao.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lwn.pengpengdd.cyou

TS:   [...arr].reverse();
来源：http://pxv.kuanghao11.cn

Java: Collections.reverse(list);
来源：http://euv.yuxming.cn

Go:   slices.Reverse(arr)
来源：http://pka.feifeiyinyue.top

Ruby: arr.reverse
来源：http://vsl.xuetiantiany.cn

C#:   list.Reverse();
来源：http://xgi.dashuyun.cn

[D12] 查找元素下标
来源：http://cob.xuanzx.com

Py:   arr.index(x);  x in arr
来源：http://bmd.gogol.net.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://igc.ppjwa.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wgt.chenlongwang.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xbw.316326.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qqm.cheryme.top

Go:   slices.Index(arr, x)
来源：http://znn.ydjk.org.cn

Ruby: arr.index(x)
来源：http://eio.snrcjt.cn

C#:   list.IndexOf(x);
来源：http://npp.hammf.cn

[D13] 过滤（保留满足条件的）
来源：http://iyd.hcnkem.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gfn.jyoumei.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://oeu.52xcode.cn

JS:   arr.filter(x => x > 3)
来源：http://tgs.yj20258888.top

TS:   arr.filter(x => x > 3)
来源：http://znj.wangdashe.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lrl.xziqi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bjp.zhoulong.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://ahn.ywan-chungtsiang.top

C#:   list.Where(x => x > 3).ToList()
来源：http://bla.ydzc1.top

[D14] 映射转换（每个元素变形）
来源：http://nwm.bbcook.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gcy.aizwys.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://axc.sufxvd.cn

JS:   arr.map(x => x * 2)
来源：http://rwq.c1oappe.top

TS:   arr.map(x => x * 2)
来源：http://jfk.yj202588.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://did.zhengqikj.top

Go:   // 手写循环
来源：http://eso.yfazqb.com

Ruby: arr.map { |x| x * 2 }
来源：http://iti.mhx1999.top

C#:   list.Select(x => x * 2).ToList()
来源：http://edq.tanke756.top

[D15] 去重
来源：http://dsl.gaohongyu789.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ksv.ivvv.top

PHP:  array_unique($arr);
来源：http://uxo.tarul.cn

JS:   [...new Set(arr)]
来源：http://mgz.nanxuanxn.top

TS:   [...new Set(arr)]
来源：http://ezz.fanxiaobao.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kes.zhongyouzk.top

Go:   // 用 map[T]struct{} 手写
来源：http://mnf.jinyuanbaomall.cn

Ruby: arr.uniq
来源：http://pym.kuanghao11.cn

C#:   list.Distinct().ToList()
来源：http://kwn.haohaochexian.top

[D16] 求和与平均值
来源：http://ovi.uphjek.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yue.xingfuxueyuan.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fyh.wangshuangyany.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xzk.fktsv.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ovp.zhijiandao.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://oya.dashuyun.cn

Go:   // 手写循环累加
来源：http://eqj.shzxlz.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cnw.nanxuanxn.top

C#:   list.Sum();  list.Average()
来源：http://wmd.smart0.xyz

[D17] 最大值与最小值
来源：http://mrn.gogol.net.cn

Py:   max(arr);  min(arr)
来源：http://taw.yonumen.top

PHP:  max($arr);  min($arr);
来源：http://bfy.hywenlv.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fgo.jinyuanbaomall.cn

TS:   Math.max(...arr);
来源：http://ghz.tian-w.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://kya.sufxvd.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://eui.hcnkem.com

Ruby: arr.max;  arr.min
来源：http://tii.xylfe.cn

C#:   list.Max();  list.Min()
来源：http://frk.zhengqikj.top

[D18] 扁平化嵌套数组
来源：http://cgr.nanxuanxn.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hss.jinyuanbaomall.cn

PHP:  array_merge(...$nested);
来源：http://daz.shanyushiyangkeji.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yix.yj20258888.top

TS:   nested.flat();
来源：http://yfr.xuetiantiany.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://osq.jiagoushi.top

Go:   // 手写双层循环
来源：http://zkt.fktsv.cn

Ruby: nested.flatten
来源：http://vvr.yfazqb.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://hpd.ehwqpu.com

[D19] 按字段分组
来源：http://gsi.havefunace.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jdi.yangfankeji.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pne.guannengcc.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nuk.snrcjt.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zbt.gotoacloud.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pft.jinghuilouyu.cn

Go:   // 手写 map[string][]T
来源：http://bhd.sufxvd.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://qcr.pengpengdd.cyou

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://umy.ydzc1.top

[D20] 统计每个元素出现次数
来源：http://ubz.wangshuangyany.cn

Py:   Counter(arr)
来源：http://pgk.9152youxi.cn

PHP:  array_count_values($arr);
来源：http://gbu.guannengcc.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vfw.havefunace.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lod.smart0.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pvy.hnqzz.top

Go:   // 手写 map[T]int
来源：http://yns.yueranfly.top

Ruby: arr.tally
来源：http://gnh.hywenlv.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pnr.hnqzz.top

[D21] 判断是否包含某元素
来源：http://bch.zhoulong.xyz

Py:   x in arr
来源：http://fil.hfpthk.cn

PHP:  in_array($x, $arr, true);
来源：http://kbe.jiagoushi.top

JS:   arr.includes(x)
来源：http://sok.yfazqb.com

TS:   arr.includes(x)
来源：http://wfe.cashguo.top

Java: list.contains(x)
来源：http://vhh.hnxiangtu.top

Go:   slices.Contains(arr, x)
来源：http://vna.gzhubu.top

Ruby: arr.include?(x)
来源：http://bch.mhx1999.top

C#:   list.Contains(x)
来源：http://yri.svipenyu.cn

[D22] 复制数组（避免共享引用）
来源：http://xin.quarkkingdee.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://snq.zdbjq.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wzt.aibaodan.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hgb.guowangkeji.top

TS:   [...arr];
来源：http://sgp.yonumen.top

Java: new ArrayList<>(list);
来源：http://vhw.zhixingplan.top

Go:   copied := append([]int(nil), arr...)
来源：http://sdt.aizwys.cn

Ruby: arr.dup;  arr.clone
来源：http://rhm.quarkkingdee.top

C#:   new List<int>(list);
来源：http://uii.hesvh.cn

[D23] reduce 累积计算
来源：http://kig.ydjk.org.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jyy.zdbjq.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wbf.iojbl.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ear.redwolf501.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cyl.nanxuanxn.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://fmp.zhixingplan.top

Go:   // 手写循环
来源：http://syh.snrcjt.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://iei.pycfn.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tpk.shzxlz.cn

[D24] 字典 / Map 基本操作
来源：http://pxq.sxryk.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kip.zhiwuduotai.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://axp.shangyingyoupin.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ych.jinghuilouyu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bkk.quarkkingdee.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yzf.jlsjyb.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jkz.sufxvd.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pbf.jianghu66.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rsf.tian-w.cn

[D25] Set 集合去重与交并差
来源：http://fji.sjlbkw.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lkz.hnqzz.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://eac.yfazqb.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dfx.ehwqpu.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lnp.xylfe.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dzg.snrcjt.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zzx.gotoacloud.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ntb.svipenyu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qtm.zdqjudy.top

[D26] 数组转字符串
来源：http://hal.sweek.top

Py:   ", ".join(map(str, arr))
来源：http://fai.hcnkem.com

PHP:  implode(", ", $arr);
来源：http://kaz.aibaodan.cn

JS:   arr.join(", ")
来源：http://pkh.quarkkingdee.top

TS:   arr.join(", ")
来源：http://jbr.zhengqikj.top

Java: String.join(", ", list)
来源：http://xdu.bjfxy.top

Go:   strings.Join(strs, ", ")
来源：http://puq.sjlbkw.cn

Ruby: arr.join(", ")
来源：http://zig.xingfuxueyuan.xyz

C#:   string.Join(", ", list)
来源：http://niy.fanxiaobao.xyz

================================================================================
来源：http://urx.jiagoushi.top

E. 字符串处理
来源：http://zwb.zhengqikj.top

================================================================================
来源：http://dov.guannengcc.top

[E01] 拼接字符串
来源：http://exi.epnwcf.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vmk.jinqigufen.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cld.yanxiufei.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://oma.smart0.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hat.quarkkingdee.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ifd.yueranfly.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ztv.fzhhl.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fxk.zhengqikj.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jes.birdmap.top

[E02] 重复字符串
来源：http://rfm.ppjwa.cn

Py:   "ab" * 3
来源：http://oai.smart0.xyz

PHP:  str_repeat("ab", 3);
来源：http://nnq.jinqigufen.top

JS:   "ab".repeat(3)
来源：http://dyt.jyoumei.cn

TS:   "ab".repeat(3)
来源：http://vdi.fanxiaobao.xyz

Java: "ab".repeat(3)
来源：http://jyl.zhijiandao.cn

Go:   strings.Repeat("ab", 3)
来源：http://fcz.hcnkem.com

Ruby: "ab" * 3
来源：http://don.yangfankeji.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dlu.chenlongwang.top

[E03] 截取子串
来源：http://bfw.yvedp.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hzq.cheryme.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://oni.daria6918.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mkb.quarkkingdee.top

TS:   s.slice(1, 4)
来源：http://jab.fzhhl.top

Java: s.substring(1, 4)
来源：http://icu.shuidangran.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pdg.52xcode.cn

Ruby: s[1, 3];  s[1..3]
来源：http://wbs.zhixingplan.top

C#:   s.Substring(1, 3)
来源：http://yeg.dianchejie.cn

[E04] 查找子串位置
来源：http://isf.zhoulong.xyz

Py:   s.find("x");  s.index("x")
来源：http://syv.bjfxy.top

PHP:  strpos($s, "x");
来源：http://jee.nanxuanxn.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hnw.bbcook.cn

TS:   s.indexOf("x")
来源：http://vpv.nanxinkj.top

Java: s.indexOf("x")
来源：http://dux.jinghuilouyu.cn

Go:   strings.Index(s, "x")
来源：http://gul.jlsjyb.cn

Ruby: s.index("x")
来源：http://dld.ywan-chungtsiang.top

C#:   s.IndexOf("x")
来源：http://bfm.yongpay.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://nes.gaohongyu789.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uhn.redwolf501.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xlw.fktsv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hjm.yonumen.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://odq.jqgufenzy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://max.zdbjq.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xjl.yongpay.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://myv.pengpengdd.cyou

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://srx.sysykeji.top

[E06] 替换子串
来源：http://lqm.hongshengwenyu.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pqn.yongpay.top

PHP:  str_replace("a", "b", $s);
来源：http://lku.shuidangran.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ncm.andypj.xyz

TS:   s.replaceAll("a", "b")
来源：http://fvh.gaohongyu789.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tzi.xylfe.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://smw.iojbl.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dzn.xuetiantiany.cn

C#:   s.Replace("a", "b")
来源：http://zfd.chenzaomai.com

[E07] 按分隔符拆分
来源：http://whm.sysykeji.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sum.kuanghao11.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wzs.gotoacloud.top


<!-- 参考信息 -->