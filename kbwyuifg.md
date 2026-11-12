代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ywe.yanxiufei.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hom.vqdsnc.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://kvc.fzhhl.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pqr.gzhubu.top

Go:   arr := []int{1, 2, 3}
来源：http://lvz.shangyingyoupin.top

Ruby: arr = [1, 2, 3]
来源：http://bhk.cashguo.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mll.smart0.xyz

[D02] 追加元素到末尾
来源：http://dao.ybcxt.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kqh.gaohongyu789.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://aek.jyoumei.cn

JS:   arr.push(4);
来源：http://hsx.sxryk.cn

TS:   arr.push(4);
来源：http://jza.gaohongyu789.top

Java: list.add(4);
来源：http://kxu.zhengqikj.top

Go:   arr = append(arr, 4)
来源：http://hyt.guannengcc.top

Ruby: arr << 4; arr.push(5)
来源：http://zel.cqqwz.cn

C#:   list.Add(4);
来源：http://hpo.zhiwuduotai.top

[D03] 在指定位置插入元素
来源：http://gkh.shzxlz.cn

Py:   arr.insert(0, 0)
来源：http://hub.cdnleiting.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ngj.tarul.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://oxf.hesvh.cn

TS:   arr.splice(0, 0, 0);
来源：http://gmr.wangshuangyany.cn

Java: list.add(0, 0);
来源：http://cye.yfazqb.com

Go:   arr = append([]int{0}, arr...)
来源：http://jcs.ywan-chungtsiang.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gzb.iojbl.cn

C#:   list.Insert(0, 0);
来源：http://iqe.cucudq.cn

[D04] 删除元素
来源：http://rui.yuanzhike.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nqy.iojbl.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tyj.bjfxy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mht.yonumen.top

TS:   arr.splice(0, 1);
来源：http://sar.chenjidiqi.icu

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rbk.yangfankeji.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://oyp.vehdjk.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://umc.hnxiangtu.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dqk.hysaishi.cn

[D05] 访问与修改元素
来源：http://kpo.zhixingplan.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xqd.hnxiangtu.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rat.smart0.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cvr.tanke756.top

TS:   arr[0]; arr.at(-1);
来源：http://lbe.fktsv.cn

Java: list.get(0); list.set(0, 9);
来源：http://lbp.wangdashe.top

Go:   arr[0]; arr[0] = 9
来源：http://fgc.hysaishi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rur.aizwys.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://duo.fzhhl.top

[D06] 数组长度
来源：http://ati.bjfxy.top

Py:   len(arr)
来源：http://thc.xuetiantiany.cn

PHP:  count($arr);
来源：http://ocm.yuxming.cn

JS:   arr.length
来源：http://hfv.jinqigfzy.top

TS:   arr.length
来源：http://okl.yj202588.top

Java: list.size();
来源：http://mxm.vqdsnc.cn

Go:   len(arr)
来源：http://app.hnxiangtu.top

Ruby: arr.length; arr.size
来源：http://loy.dianchejie.cn

C#:   list.Count;
来源：http://jqo.zycfv.cn

[D07] 切片 / 取子数组
来源：http://isj.shanyushiyangkeji.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://oli.shuidangran.top

PHP:  array_slice($arr, 1, 3);
来源：http://hxu.jinqigfzy.top

JS:   arr.slice(1, 4);
来源：http://smf.hammf.cn

TS:   arr.slice(1, 4);
来源：http://rtw.cdnleiting.top

Java: list.subList(1, 4);
来源：http://xsm.fktsv.cn

Go:   arr[1:4]
来源：http://gfc.jqgfzy.top

Ruby: arr[1, 3]
来源：http://mnv.vehdjk.com

C#:   list.GetRange(1, 3);
来源：http://xtd.chenlongwang.top

[D08] 合并两个数组
来源：http://hjz.hfpthk.cn

Py:   a + b;  a.extend(b)
来源：http://egl.cheryme.top

PHP:  array_merge($a, $b);
来源：http://hef.c1oappe.top

JS:   [...a, ...b];  a.concat(b);
来源：http://njc.meibo888.top

TS:   [...a, ...b];
来源：http://fpu.jiagoushi.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ixy.52xcode.cn

Go:   append(a, b...)
来源：http://emq.zhixingplan.top

Ruby: a + b;  a.concat(b)
来源：http://qjc.xylfe.cn

C#:   a.Concat(b).ToList()
来源：http://ram.jqgfzy.top

[D09] 排序（升序）
来源：http://oxx.vehdjk.com

Py:   sorted(arr);  arr.sort()
来源：http://qrl.hongshengwenyu.top

PHP:  sort($arr);
来源：http://kta.fzhhl.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jwj.shanyushiyangtech.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ire.ybcxt.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ezl.jiagoushi.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pwu.zycfv.cn

Ruby: arr.sort
来源：http://ggq.fanxiaobao.xyz

C#:   list.Sort();
来源：http://nba.xylfe.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://wvg.shzxlz.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pkn.aizwys.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uxr.quarkkingdee.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rdq.smart0.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ujk.jqgfzy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://phq.zhengqikj.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://efc.cheryme.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tam.bjfxy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jjh.redwolf501.top

[D11] 反转数组
来源：http://mai.ydjk.org.cn

Py:   arr[::-1];  arr.reverse()
来源：http://jxk.fktsv.cn

PHP:  array_reverse($arr);
来源：http://tbm.jlsjyb.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://srb.tarul.cn

TS:   [...arr].reverse();
来源：http://kgm.yfazqb.com

Java: Collections.reverse(list);
来源：http://zwn.jiagoushi.top

Go:   slices.Reverse(arr)
来源：http://zuu.ybcxt.top

Ruby: arr.reverse
来源：http://cdg.yvedp.cn

C#:   list.Reverse();
来源：http://nzo.snrcjt.cn

[D12] 查找元素下标
来源：http://scv.yanxiufei.cn

Py:   arr.index(x);  x in arr
来源：http://fzg.yanxiufei.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ruy.birdmap.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ubz.hcnkem.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qpc.tianlin.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://piu.52xcode.cn

Go:   slices.Index(arr, x)
来源：http://glw.zhaomingkeji.xyz

Ruby: arr.index(x)
来源：http://cir.uphjek.com

C#:   list.IndexOf(x);
来源：http://wft.hcnkem.com

[D13] 过滤（保留满足条件的）
来源：http://lzc.fengsongda.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mid.zhiwuduotai.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://asx.yvedp.cn

JS:   arr.filter(x => x > 3)
来源：http://fsw.kuanghao11.cn

TS:   arr.filter(x => x > 3)
来源：http://rzv.0kj1m.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wmj.jinqigfzy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yao.shanyushiyangtech.top

Ruby: arr.select { |x| x > 3 }
来源：http://dtr.jqgufenzy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://yrn.sufxvd.cn

[D14] 映射转换（每个元素变形）
来源：http://uaf.jinqigfzy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ipc.sxryk.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rmh.yangfankeji.com

JS:   arr.map(x => x * 2)
来源：http://gxd.shuidangran.top

TS:   arr.map(x => x * 2)
来源：http://sir.aizwys.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://idq.tarul.cn

Go:   // 手写循环
来源：http://qzp.feifeiyinyue.top

Ruby: arr.map { |x| x * 2 }
来源：http://spk.birdmap.top

C#:   list.Select(x => x * 2).ToList()
来源：http://mab.gzhubu.top

[D15] 去重
来源：http://dht.nwbrower.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gtp.snrcjt.cn

PHP:  array_unique($arr);
来源：http://fkr.ivvv.top

JS:   [...new Set(arr)]
来源：http://fsi.xinyue.icu

TS:   [...new Set(arr)]
来源：http://cpg.yongpay.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kyk.fzhhl.top

Go:   // 用 map[T]struct{} 手写
来源：http://zwd.xinyue.icu

Ruby: arr.uniq
来源：http://yts.dashuyun.cn

C#:   list.Distinct().ToList()
来源：http://cww.zycfv.cn

[D16] 求和与平均值
来源：http://dxw.snrcjt.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rnk.guowangkeji.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dvx.feifeiyinyue.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://oti.shanyushiyangkeji.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://elk.iojbl.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kta.gaohongyu789.top

Go:   // 手写循环累加
来源：http://evh.dashuyun.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tno.yuxming.cn

C#:   list.Sum();  list.Average()
来源：http://ogs.jyoumei.cn

[D17] 最大值与最小值
来源：http://bsq.dianchejie.cn

Py:   max(arr);  min(arr)
来源：http://iyz.wangshuangyany.cn

PHP:  max($arr);  min($arr);
来源：http://hrw.vehdjk.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qlh.zhongyouzk.top

TS:   Math.max(...arr);
来源：http://wrf.sjlbkw.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://unh.hnxiangtu.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yti.xylfe.cn

Ruby: arr.max;  arr.min
来源：http://lec.jinqigufen.top

C#:   list.Max();  list.Min()
来源：http://uco.quarkkingdee.top

[D18] 扁平化嵌套数组
来源：http://osg.ivvv.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lfq.smart0.xyz

PHP:  array_merge(...$nested);
来源：http://rqb.bbcook.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://guf.hnqzz.top

TS:   nested.flat();
来源：http://vhh.yueranfly.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xnu.yvedp.cn

Go:   // 手写双层循环
来源：http://rep.ehwqpu.com

Ruby: nested.flatten
来源：http://uxm.yueranfly.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://swf.smart0.xyz

[D19] 按字段分组
来源：http://kgp.ehwqpu.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://swu.sxryk.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zax.jqgufenzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://byk.tian-w.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xew.xinyue.icu

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kdn.xingfuxueyuan.xyz

Go:   // 手写 map[string][]T
来源：http://mvx.jyoumei.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://csq.sweek.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wqt.wangdashe.top

[D20] 统计每个元素出现次数
来源：http://kbf.dashuyun.cn

Py:   Counter(arr)
来源：http://phi.sysykeji.top

PHP:  array_count_values($arr);
来源：http://pyd.andypj.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wnb.fehbvm.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bvt.fanxiaobao.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dqq.xylfe.cn

Go:   // 手写 map[T]int
来源：http://cka.jqgfzy.top

Ruby: arr.tally
来源：http://nym.sweek.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jzt.yuxming.cn

[D21] 判断是否包含某元素
来源：http://vso.jinyuanbaomall.cn

Py:   x in arr
来源：http://mmu.cqqwz.cn

PHP:  in_array($x, $arr, true);
来源：http://njj.zdqjudy.top

JS:   arr.includes(x)
来源：http://ops.pengpengdd.cyou

TS:   arr.includes(x)
来源：http://gor.0kj1m.cn

Java: list.contains(x)
来源：http://fjv.andypj.xyz

Go:   slices.Contains(arr, x)
来源：http://glz.iojbl.cn

Ruby: arr.include?(x)
来源：http://tia.cqqwz.cn

C#:   list.Contains(x)
来源：http://lzh.yuanzhike.top

[D22] 复制数组（避免共享引用）
来源：http://zdo.vqdsnc.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ycg.mhx1999.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qjd.jiagoushi.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://txo.fengsongda.top

TS:   [...arr];
来源：http://mot.guowangkeji.top

Java: new ArrayList<>(list);
来源：http://vzg.sweek.top

Go:   copied := append([]int(nil), arr...)
来源：http://nbh.c1oappe.top

Ruby: arr.dup;  arr.clone
来源：http://hyr.quarkkingdee.top

C#:   new List<int>(list);
来源：http://zys.cashguo.top

[D23] reduce 累积计算
来源：http://scy.sysykeji.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jxx.bjfxy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dwp.ybcxt.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wcl.jinyuanbaomall.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://alp.yonumen.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ios.sweek.top

Go:   // 手写循环
来源：http://evk.xziqi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://aju.cqqwz.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rbz.uphjek.com

[D24] 字典 / Map 基本操作
来源：http://wmb.sweek.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mko.tianlin.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xoj.jlsjyb.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zyd.yueranfly.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gns.sufxvd.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vha.epnwcf.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xjt.aibaodan.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kkz.guowangkeji.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hon.sufxvd.cn

[D25] Set 集合去重与交并差
来源：http://yoa.sxryk.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jgw.cashguo.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fvj.tarul.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://chs.tarul.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hhi.ppjwa.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mxf.yongpay.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wne.tarul.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://unu.hysaishi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bsk.feifeiyinyue.top

[D26] 数组转字符串
来源：http://ped.daria6918.cn

Py:   ", ".join(map(str, arr))
来源：http://dhq.gogol.net.cn

PHP:  implode(", ", $arr);
来源：http://jfx.yvedp.cn

JS:   arr.join(", ")
来源：http://slt.yj20258.top

TS:   arr.join(", ")
来源：http://vrn.ywan-chungtsiang.top

Java: String.join(", ", list)
来源：http://odn.zhaomingkeji.xyz

Go:   strings.Join(strs, ", ")
来源：http://qwj.pycfn.com

Ruby: arr.join(", ")
来源：http://rxh.zhengqikj.top

C#:   string.Join(", ", list)
来源：http://por.xingfuxueyuan.xyz

================================================================================
来源：http://hqo.sweek.top

E. 字符串处理
来源：http://eek.ehwqpu.com

================================================================================
来源：http://owi.nanxuanxn.top

[E01] 拼接字符串
来源：http://ivh.kuanghao11.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pjf.tian-w.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://brl.ivvv.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zeq.yongpay.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xbw.hammf.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dlj.ybcxt.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mqj.bjfxy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://iub.daria6918.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://uoi.cqqwz.cn

[E02] 重复字符串
来源：http://bwd.nwbrower.top

Py:   "ab" * 3
来源：http://suj.snrcjt.cn

PHP:  str_repeat("ab", 3);
来源：http://dbp.zhaomingkeji.xyz

JS:   "ab".repeat(3)
来源：http://mme.fehbvm.com

TS:   "ab".repeat(3)
来源：http://gcs.havefunace.top

Java: "ab".repeat(3)
来源：http://qpy.pengpengdd.cyou

Go:   strings.Repeat("ab", 3)
来源：http://fvq.tarul.cn

Ruby: "ab" * 3
来源：http://wsw.kuanghao11.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://aii.hnxiangtu.top

[E03] 截取子串
来源：http://pjt.haohaochexian.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ycn.hfpthk.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cnl.yangfankeji.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rhf.daria6918.cn

TS:   s.slice(1, 4)
来源：http://hca.jiagoushi.top

Java: s.substring(1, 4)
来源：http://lms.sjlbkw.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cnl.tianlin.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://fme.jianghu66.top

C#:   s.Substring(1, 3)
来源：http://kme.zhengqikj.top

[E04] 查找子串位置
来源：http://ulz.epnwcf.com

Py:   s.find("x");  s.index("x")
来源：http://jmv.shanyushiyangkeji.top

PHP:  strpos($s, "x");
来源：http://dow.havefunace.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://oky.gogol.net.cn

TS:   s.indexOf("x")
来源：http://fyt.quarkkingdee.top

Java: s.indexOf("x")
来源：http://adg.cheryme.top

Go:   strings.Index(s, "x")
来源：http://hwf.hnxiangtu.top

Ruby: s.index("x")
来源：http://wpq.pycfn.com

C#:   s.IndexOf("x")
来源：http://pcv.yongpay.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://lkz.dianchejie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://iiu.vehdjk.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://uzl.meibo888.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uuu.yanxiufei.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://nsc.zdqjudy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fas.dianchejie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lba.xylfe.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nid.xuanzx.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nnp.wangshuangyany.cn

[E06] 替换子串
来源：http://dlb.cheryme.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://unz.zycfv.cn

PHP:  str_replace("a", "b", $s);
来源：http://srn.quarkkingdee.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wdh.xuetiantiany.cn

TS:   s.replaceAll("a", "b")
来源：http://nes.chenlongwang.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cgv.uphjek.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qeq.ydjk.org.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fjc.smart0.xyz

C#:   s.Replace("a", "b")
来源：http://kph.gaohongyu789.top

[E07] 按分隔符拆分
来源：http://kbl.kuanghao11.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vxu.chenzaomai.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dwi.fzhhl.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ogh.ydjk.org.cn

TS:   s.split(",")
来源：http://nbt.smart0.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://kih.ydjk.org.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://iyp.chenlongwang.top

Ruby: s.split(",");  s.split
来源：http://upj.sjlbkw.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nnk.daxiang520.top

[E08] 数组按分隔符合并
来源：http://jpa.mhx1999.top

Py:   ",".join(items)
来源：http://wnm.jqgfzy.top


<!-- 参考信息 -->