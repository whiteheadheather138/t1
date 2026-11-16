代发 wailian999

D. 数组 / 列表 / 集合
来源：http://znf.ehwqpu.com

================================================================================
来源：http://hjl.jqgfzy.top

[D01] 创建数组 / 列表
来源：http://sfq.ehwqpu.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://llj.hywenlv.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://crd.cheryme.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bwm.gzhubu.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://vau.tarul.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kra.xylfe.cn

Go:   arr := []int{1, 2, 3}
来源：http://wly.cqqwz.cn

Ruby: arr = [1, 2, 3]
来源：http://wvu.pycfn.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vmd.chenlongwang.top

[D02] 追加元素到末尾
来源：http://awk.wangshuangyany.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ypq.zhongyouzk.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bvn.iojbl.cn

JS:   arr.push(4);
来源：http://tuf.fzhhl.top

TS:   arr.push(4);
来源：http://vod.sjlbkw.cn

Java: list.add(4);
来源：http://fec.snrcjt.cn

Go:   arr = append(arr, 4)
来源：http://odi.hnqzz.top

Ruby: arr << 4; arr.push(5)
来源：http://ypg.yangfankeji.com

C#:   list.Add(4);
来源：http://kcc.zycfv.cn

[D03] 在指定位置插入元素
来源：http://cra.cdnleiting.top

Py:   arr.insert(0, 0)
来源：http://som.c1oappe.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rdj.sxryk.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zwd.tanke756.top

TS:   arr.splice(0, 0, 0);
来源：http://cuj.sufxvd.cn

Java: list.add(0, 0);
来源：http://zvi.jinghuilouyu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vaj.chenzaomai.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kii.meibo888.top

C#:   list.Insert(0, 0);
来源：http://fiu.sjlbkw.cn

[D04] 删除元素
来源：http://cws.jlsjyb.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dgf.ydzc1.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jjx.jinghuilouyu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fbt.vehdjk.com

TS:   arr.splice(0, 1);
来源：http://lqv.ywan-chungtsiang.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qoy.hammf.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://aro.yueranfly.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bgm.zhixingplan.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tho.ppjwa.cn

[D05] 访问与修改元素
来源：http://svs.jianghu66.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://djh.jianghu66.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rpq.gotoacloud.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ykr.sweek.top

TS:   arr[0]; arr.at(-1);
来源：http://pod.yueranfly.top

Java: list.get(0); list.set(0, 9);
来源：http://otj.daxiang520.top

Go:   arr[0]; arr[0] = 9
来源：http://mcd.jqgfzy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yux.yonumen.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qpr.wangshuangyany.cn

[D06] 数组长度
来源：http://qtb.9152youxi.cn

Py:   len(arr)
来源：http://bkx.zhaomingkeji.xyz

PHP:  count($arr);
来源：http://ufz.sysykeji.top

JS:   arr.length
来源：http://xxg.ydzc1.top

TS:   arr.length
来源：http://dwd.vqdsnc.cn

Java: list.size();
来源：http://esf.xinyue.icu

Go:   len(arr)
来源：http://fos.yj20258.top

Ruby: arr.length; arr.size
来源：http://mas.pycfn.com

C#:   list.Count;
来源：http://ncc.haohaochexian.top

[D07] 切片 / 取子数组
来源：http://qjb.zhaomingkeji.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zwq.zhixingplan.top

PHP:  array_slice($arr, 1, 3);
来源：http://wtz.chenzaomai.com

JS:   arr.slice(1, 4);
来源：http://ghh.ctjpmb.com

TS:   arr.slice(1, 4);
来源：http://zsk.nanxuanxn.top

Java: list.subList(1, 4);
来源：http://ykh.sysykeji.top

Go:   arr[1:4]
来源：http://mtr.quarkkingdee.top

Ruby: arr[1, 3]
来源：http://qgi.wangdashe.top

C#:   list.GetRange(1, 3);
来源：http://huo.9152youxi.cn

[D08] 合并两个数组
来源：http://yho.sufxvd.cn

Py:   a + b;  a.extend(b)
来源：http://gxq.gaohongyu789.top

PHP:  array_merge($a, $b);
来源：http://wfh.fzhhl.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ncc.shuidangran.top

TS:   [...a, ...b];
来源：http://vud.fengsongda.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jqk.sysykeji.top

Go:   append(a, b...)
来源：http://tso.dianchejie.cn

Ruby: a + b;  a.concat(b)
来源：http://vph.meibo888.top

C#:   a.Concat(b).ToList()
来源：http://lcy.gzhubu.top

[D09] 排序（升序）
来源：http://vlo.shangyingyoupin.top

Py:   sorted(arr);  arr.sort()
来源：http://jvf.tarul.cn

PHP:  sort($arr);
来源：http://fji.bjfxy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pkn.redwolf501.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://qyj.hysaishi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tgu.fanxiaobao.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://peb.sjlbkw.cn

Ruby: arr.sort
来源：http://lqv.jiagoushi.top

C#:   list.Sort();
来源：http://fqc.andypj.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://cla.guannengcc.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xps.shuidangran.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://npl.tanke756.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kea.zhongyouzk.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vno.hesvh.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://uvg.shzxlz.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nsr.ywan-chungtsiang.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rxi.birdmap.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jsj.zhixingplan.top

[D11] 反转数组
来源：http://tzo.hesvh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://jxn.shuidangran.top

PHP:  array_reverse($arr);
来源：http://ryr.nanxinkj.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tfa.zycfv.cn

TS:   [...arr].reverse();
来源：http://jyr.yongpay.top

Java: Collections.reverse(list);
来源：http://esu.wangdashe.top

Go:   slices.Reverse(arr)
来源：http://ksw.zdbjq.cn

Ruby: arr.reverse
来源：http://amj.quarkkingdee.top

C#:   list.Reverse();
来源：http://nlt.ppjwa.cn

[D12] 查找元素下标
来源：http://cpu.ywan-chungtsiang.top

Py:   arr.index(x);  x in arr
来源：http://ezw.birdmap.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hsb.epnwcf.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ogh.uphjek.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ipg.fktsv.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bhr.tanke756.top

Go:   slices.Index(arr, x)
来源：http://lhw.meibo888.top

Ruby: arr.index(x)
来源：http://mfz.dashuyun.cn

C#:   list.IndexOf(x);
来源：http://ojo.zhijiandao.cn

[D13] 过滤（保留满足条件的）
来源：http://kxt.redwolf501.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tme.jinyuanbaomall.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://eja.sysykeji.top

JS:   arr.filter(x => x > 3)
来源：http://bje.tian-w.cn

TS:   arr.filter(x => x > 3)
来源：http://fyy.mhx1999.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vuv.zhoulong.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://prn.jinghuilouyu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://yka.daxiang520.top

C#:   list.Where(x => x > 3).ToList()
来源：http://gcx.aizwys.cn

[D14] 映射转换（每个元素变形）
来源：http://kki.bbcook.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rfj.zhongyouzk.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vsi.shzxlz.cn

JS:   arr.map(x => x * 2)
来源：http://bjz.zdbjq.cn

TS:   arr.map(x => x * 2)
来源：http://cdi.hongshengwenyu.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ima.zdbjq.cn

Go:   // 手写循环
来源：http://vwi.havefunace.top

Ruby: arr.map { |x| x * 2 }
来源：http://iyh.chenzaomai.com

C#:   list.Select(x => x * 2).ToList()
来源：http://vuw.shangyingyoupin.top

[D15] 去重
来源：http://abl.jinqigfzy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vfd.nwbrower.top

PHP:  array_unique($arr);
来源：http://pdx.guowangkeji.top

JS:   [...new Set(arr)]
来源：http://pmt.zhiwuduotai.top

TS:   [...new Set(arr)]
来源：http://ede.cqqwz.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yvf.zhengqikj.top

Go:   // 用 map[T]struct{} 手写
来源：http://oml.yvedp.cn

Ruby: arr.uniq
来源：http://uif.fanxiaobao.xyz

C#:   list.Distinct().ToList()
来源：http://qyj.hammf.cn

[D16] 求和与平均值
来源：http://khe.hnqzz.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kgx.tanke756.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mde.gotoacloud.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://isg.ctjpmb.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nbp.xziqi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://myo.jqgufenzy.top

Go:   // 手写循环累加
来源：http://nwf.ybcxt.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pry.dianchejie.cn

C#:   list.Sum();  list.Average()
来源：http://qya.sxryk.cn

[D17] 最大值与最小值
来源：http://ghd.jqgfzy.top

Py:   max(arr);  min(arr)
来源：http://mft.sweek.top

PHP:  max($arr);  min($arr);
来源：http://hup.tian-w.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://egz.jlsjyb.cn

TS:   Math.max(...arr);
来源：http://zer.c1oappe.top

Java: Collections.max(list);  Collections.min(list);
来源：http://xgq.daxiang520.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://joc.c1oappe.top

Ruby: arr.max;  arr.min
来源：http://fop.smart0.xyz

C#:   list.Max();  list.Min()
来源：http://eiw.guannengcc.top

[D18] 扁平化嵌套数组
来源：http://rrx.sweek.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://txe.aizwys.cn

PHP:  array_merge(...$nested);
来源：http://lem.hysaishi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://brt.svipenyu.cn

TS:   nested.flat();
来源：http://yhu.zdqjudy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://iny.sxryk.cn

Go:   // 手写双层循环
来源：http://ubz.cdnleiting.top

Ruby: nested.flatten
来源：http://uor.gogol.net.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://uhp.snrcjt.cn

[D19] 按字段分组
来源：http://vto.sufxvd.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vic.sxryk.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nvk.hammf.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hhp.shangyingyoupin.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://qjh.zhongyouzk.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pqp.pycfn.com

Go:   // 手写 map[string][]T
来源：http://roy.yj202588.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://vqk.gzhubu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gtd.ydjk.org.cn

[D20] 统计每个元素出现次数
来源：http://eoq.shuidangran.top

Py:   Counter(arr)
来源：http://ejf.zdbjq.cn

PHP:  array_count_values($arr);
来源：http://qpv.svipenyu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lfd.dianchejie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ooq.aibaodan.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ipc.sufxvd.cn

Go:   // 手写 map[T]int
来源：http://zia.zhengqikj.top

Ruby: arr.tally
来源：http://grs.jinqigufen.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kvb.jinqigufen.top

[D21] 判断是否包含某元素
来源：http://xjg.epnwcf.com

Py:   x in arr
来源：http://qwr.hywenlv.cn

PHP:  in_array($x, $arr, true);
来源：http://tzr.hysaishi.cn

JS:   arr.includes(x)
来源：http://zrn.yfazqb.com

TS:   arr.includes(x)
来源：http://wjo.gotoacloud.top

Java: list.contains(x)
来源：http://qti.hongshengwenyu.top

Go:   slices.Contains(arr, x)
来源：http://cwq.bjfxy.top

Ruby: arr.include?(x)
来源：http://wcy.gaohongyu789.top

C#:   list.Contains(x)
来源：http://eij.zdbjq.cn

[D22] 复制数组（避免共享引用）
来源：http://ijw.0kj1m.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://siv.ywan-chungtsiang.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qrn.haohaochexian.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jea.fzhhl.top

TS:   [...arr];
来源：http://yas.zhengqikj.top

Java: new ArrayList<>(list);
来源：http://oiw.gaohongyu789.top

Go:   copied := append([]int(nil), arr...)
来源：http://ieh.yuanzhike.top

Ruby: arr.dup;  arr.clone
来源：http://afj.jyoumei.cn

C#:   new List<int>(list);
来源：http://sam.chenjidiqi.icu

[D23] reduce 累积计算
来源：http://cmp.havefunace.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ifb.daria6918.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kky.daria6918.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://elf.jyoumei.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ugy.feifeiyinyue.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://vsh.sjlbkw.cn

Go:   // 手写循环
来源：http://ccn.cdnleiting.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://stx.yuanzhike.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://whc.yueranfly.top

[D24] 字典 / Map 基本操作
来源：http://wpl.guannengcc.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kuv.shuidangran.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mlf.uphjek.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zwh.mhx1999.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nfv.uphjek.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sfi.yj202588.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lli.xuetiantiany.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://olh.epnwcf.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sbd.hammf.cn

[D25] Set 集合去重与交并差
来源：http://syn.hnxiangtu.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nas.daxiang520.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cto.aibaodan.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bzu.havefunace.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://msi.ybcxt.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ugf.hnxiangtu.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ueq.daxiang520.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://slf.jianghu66.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gzr.ctjpmb.com

[D26] 数组转字符串
来源：http://svk.pycfn.com

Py:   ", ".join(map(str, arr))
来源：http://gzp.xylfe.cn

PHP:  implode(", ", $arr);
来源：http://yfl.cheryme.top

JS:   arr.join(", ")
来源：http://bdh.xuanzx.com

TS:   arr.join(", ")
来源：http://ebo.bbcook.cn

Java: String.join(", ", list)
来源：http://bjv.sxryk.cn

Go:   strings.Join(strs, ", ")
来源：http://vef.nanxinkj.top

Ruby: arr.join(", ")
来源：http://cvz.sweek.top

C#:   string.Join(", ", list)
来源：http://usk.zhaomingkeji.xyz

================================================================================
来源：http://lnm.jinqigfzy.top

E. 字符串处理
来源：http://pkp.chenjidiqi.icu

================================================================================
来源：http://emv.yfazqb.com

[E01] 拼接字符串
来源：http://pqz.chenlongwang.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yyw.vehdjk.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bkp.daria6918.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tqu.ybcxt.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fco.chenjidiqi.icu

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yic.ybcxt.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yny.hnqzz.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pdi.chenlongwang.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ver.tianlin.xyz

[E02] 重复字符串
来源：http://poc.yuanzhike.top

Py:   "ab" * 3
来源：http://syg.zhengqikj.top

PHP:  str_repeat("ab", 3);
来源：http://lqf.ehwqpu.com

JS:   "ab".repeat(3)
来源：http://gpf.zhijiandao.cn

TS:   "ab".repeat(3)
来源：http://eru.gaohongyu789.top

Java: "ab".repeat(3)
来源：http://oes.hnqzz.top

Go:   strings.Repeat("ab", 3)
来源：http://rkc.cqqwz.cn

Ruby: "ab" * 3
来源：http://gpj.dianchejie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fsb.xuanzx.com

[E03] 截取子串
来源：http://xop.aibaodan.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xgp.hysaishi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://weq.nanxinkj.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vqe.ywan-chungtsiang.top

TS:   s.slice(1, 4)
来源：http://zep.zycfv.cn

Java: s.substring(1, 4)
来源：http://xmk.xingfuxueyuan.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zpg.jianghu66.top

Ruby: s[1, 3];  s[1..3]
来源：http://akd.bjfxy.top

C#:   s.Substring(1, 3)
来源：http://zyq.ybcxt.top

[E04] 查找子串位置
来源：http://bnw.c1oappe.top

Py:   s.find("x");  s.index("x")
来源：http://pju.feifeiyinyue.top

PHP:  strpos($s, "x");
来源：http://utk.ppjwa.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sdm.bjfxy.top

TS:   s.indexOf("x")
来源：http://emu.316326.xyz

Java: s.indexOf("x")
来源：http://rfc.svipenyu.cn

Go:   strings.Index(s, "x")
来源：http://iri.yueranfly.top

Ruby: s.index("x")
来源：http://ysi.epnwcf.com

C#:   s.IndexOf("x")
来源：http://qta.gotoacloud.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://wpk.tianlin.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://keo.smart0.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nhv.fengsongda.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ltm.fehbvm.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://gto.chenlongwang.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xgy.nwbrower.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ejz.tianlin.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tyd.guannengcc.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zxm.shuidangran.top

[E06] 替换子串
来源：http://zto.xingfuxueyuan.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zqp.jinqigfzy.top

PHP:  str_replace("a", "b", $s);
来源：http://ibl.yongpay.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jqe.fanxiaobao.xyz

TS:   s.replaceAll("a", "b")
来源：http://jnh.ywan-chungtsiang.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://upw.yvedp.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bck.quarkkingdee.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xiq.smart0.xyz

C#:   s.Replace("a", "b")
来源：http://xnz.ydjk.org.cn

[E07] 按分隔符拆分
来源：http://lnm.nanxuanxn.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gwk.pengpengdd.cyou

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://eny.shuidangran.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://hvw.quarkkingdee.top

TS:   s.split(",")
来源：http://kjh.316326.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://zxj.cucudq.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dkk.jinqigfzy.top


<!-- 参考信息 -->