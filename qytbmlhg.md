代发 wailian999

PHP:  // 无重载
来源：http://nyd.fanxiaobao.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://lwb.iojbl.cn

TS:   // 用联合类型或重载签名声明
来源：http://ogy.quarkkingdee.top

Java: void f(int a) {}  void f(String a) {}
来源：http://cik.uphjek.com

Go:   // 无重载：用不同函数名
来源：http://swg.ehwqpu.com

Ruby: # 无重载：靠动态参数
来源：http://elf.pycfn.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://xkj.fanxiaobao.xyz

================================================================================
来源：http://xdz.zdqjudy.top

D. 数组 / 列表 / 集合
来源：http://edi.sxryk.cn

================================================================================
来源：http://avh.meibo888.top

[D01] 创建数组 / 列表
来源：http://isj.jianghu66.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://cmx.aizwys.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dmc.tarul.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pvu.snrcjt.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xyj.cqqwz.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kum.jqgufenzy.top

Go:   arr := []int{1, 2, 3}
来源：http://dtz.yuxming.cn

Ruby: arr = [1, 2, 3]
来源：http://cxh.shanyushiyangtech.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ynt.daria6918.cn

[D02] 追加元素到末尾
来源：http://flf.hywenlv.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gbl.jianghu66.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mic.9152youxi.cn

JS:   arr.push(4);
来源：http://xzo.pengpengdd.cyou

TS:   arr.push(4);
来源：http://vps.fengsongda.top

Java: list.add(4);
来源：http://ryp.gotoacloud.top

Go:   arr = append(arr, 4)
来源：http://zla.ywan-chungtsiang.top

Ruby: arr << 4; arr.push(5)
来源：http://mhi.52xcode.cn

C#:   list.Add(4);
来源：http://vrq.smart0.xyz

[D03] 在指定位置插入元素
来源：http://kjb.svipenyu.cn

Py:   arr.insert(0, 0)
来源：http://jiz.zhengqikj.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nsz.0kj1m.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://idm.9152youxi.cn

TS:   arr.splice(0, 0, 0);
来源：http://wcv.yj20258888.top

Java: list.add(0, 0);
来源：http://pwa.sufxvd.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fun.aizwys.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jxy.zdqjudy.top

C#:   list.Insert(0, 0);
来源：http://jxk.dianchejie.cn

[D04] 删除元素
来源：http://zzf.c1oappe.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ftf.hammf.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ufr.tianlin.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dty.tanke756.top

TS:   arr.splice(0, 1);
来源：http://oey.wangdashe.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gkl.yongpay.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uwg.nwbrower.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kjd.yongpay.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ymg.wangdashe.top

[D05] 访问与修改元素
来源：http://etc.shangyingyoupin.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://otl.sufxvd.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qwz.bjfxy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sdw.gogol.net.cn

TS:   arr[0]; arr.at(-1);
来源：http://tob.yuxming.cn

Java: list.get(0); list.set(0, 9);
来源：http://arq.zdbjq.cn

Go:   arr[0]; arr[0] = 9
来源：http://msq.hongshengwenyu.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hez.xinyue.icu

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pvu.jlsjyb.cn

[D06] 数组长度
来源：http://pkf.jinyuanbaomall.cn

Py:   len(arr)
来源：http://dtp.ywan-chungtsiang.top

PHP:  count($arr);
来源：http://jja.xziqi.cn

JS:   arr.length
来源：http://phy.shuidangran.top

TS:   arr.length
来源：http://zzc.hysaishi.cn

Java: list.size();
来源：http://nab.xuetiantiany.cn

Go:   len(arr)
来源：http://ezc.c1oappe.top

Ruby: arr.length; arr.size
来源：http://nbs.gzhubu.top

C#:   list.Count;
来源：http://msq.yj202588.top

[D07] 切片 / 取子数组
来源：http://wgq.c1oappe.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wjj.yangfankeji.com

PHP:  array_slice($arr, 1, 3);
来源：http://gwq.jqgufenzy.top

JS:   arr.slice(1, 4);
来源：http://ega.haohaochexian.top

TS:   arr.slice(1, 4);
来源：http://img.shzxlz.cn

Java: list.subList(1, 4);
来源：http://oky.hcnkem.com

Go:   arr[1:4]
来源：http://osg.tian-w.cn

Ruby: arr[1, 3]
来源：http://njn.yangfankeji.com

C#:   list.GetRange(1, 3);
来源：http://tws.52xcode.cn

[D08] 合并两个数组
来源：http://uge.zhixingplan.top

Py:   a + b;  a.extend(b)
来源：http://gdf.ivvv.top

PHP:  array_merge($a, $b);
来源：http://djt.tianlin.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://lvf.smart0.xyz

TS:   [...a, ...b];
来源：http://baa.gotoacloud.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://oui.fehbvm.com

Go:   append(a, b...)
来源：http://gbf.xuanzx.com

Ruby: a + b;  a.concat(b)
来源：http://rdj.yongpay.top

C#:   a.Concat(b).ToList()
来源：http://hdo.ydjk.org.cn

[D09] 排序（升序）
来源：http://phl.fktsv.cn

Py:   sorted(arr);  arr.sort()
来源：http://too.ppjwa.cn

PHP:  sort($arr);
来源：http://oeu.hfpthk.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xnj.cdnleiting.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ypl.yongpay.top

Java: Collections.sort(list);  list.sort(null);
来源：http://hcl.snrcjt.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ibl.xinyue.icu

Ruby: arr.sort
来源：http://jgu.zdbjq.cn

C#:   list.Sort();
来源：http://pwg.zhongyouzk.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ule.jinqigufen.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tui.shuidangran.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://btk.ydjk.org.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://aou.zhiwuduotai.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tid.fzhhl.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gjh.c1oappe.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vuo.52xcode.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wqs.yuxming.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nux.mhx1999.top

[D11] 反转数组
来源：http://azp.zhixingplan.top

Py:   arr[::-1];  arr.reverse()
来源：http://mhw.yongpay.top

PHP:  array_reverse($arr);
来源：http://dzk.hysaishi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vom.hywenlv.cn

TS:   [...arr].reverse();
来源：http://ecx.tian-w.cn

Java: Collections.reverse(list);
来源：http://gqd.zhengqikj.top

Go:   slices.Reverse(arr)
来源：http://nvo.ydjk.org.cn

Ruby: arr.reverse
来源：http://xaf.xuanzx.com

C#:   list.Reverse();
来源：http://tcv.tian-w.cn

[D12] 查找元素下标
来源：http://wfa.yangfankeji.com

Py:   arr.index(x);  x in arr
来源：http://ouu.yanxiufei.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pvw.zycfv.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qts.tian-w.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hwv.jiagoushi.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://opo.sysykeji.top

Go:   slices.Index(arr, x)
来源：http://woi.xinyue.icu

Ruby: arr.index(x)
来源：http://ygo.epnwcf.com

C#:   list.IndexOf(x);
来源：http://fgt.yueranfly.top

[D13] 过滤（保留满足条件的）
来源：http://fwy.vqdsnc.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kjv.xuetiantiany.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bgx.cashguo.top

JS:   arr.filter(x => x > 3)
来源：http://cut.yj20258.top

TS:   arr.filter(x => x > 3)
来源：http://gyi.jqgufenzy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://grt.nwbrower.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nxu.iojbl.cn

Ruby: arr.select { |x| x > 3 }
来源：http://bel.jianghu66.top

C#:   list.Where(x => x > 3).ToList()
来源：http://gul.9152youxi.cn

[D14] 映射转换（每个元素变形）
来源：http://jvr.yuxming.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qie.shuidangran.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tic.hesvh.cn

JS:   arr.map(x => x * 2)
来源：http://xia.xinyue.icu

TS:   arr.map(x => x * 2)
来源：http://nxg.hnxiangtu.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://nsi.fengsongda.top

Go:   // 手写循环
来源：http://llf.ctjpmb.com

Ruby: arr.map { |x| x * 2 }
来源：http://npk.c1oappe.top

C#:   list.Select(x => x * 2).ToList()
来源：http://oal.tanke756.top

[D15] 去重
来源：http://rqt.birdmap.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tzw.uphjek.com

PHP:  array_unique($arr);
来源：http://nhn.52xcode.cn

JS:   [...new Set(arr)]
来源：http://gll.dianchejie.cn

TS:   [...new Set(arr)]
来源：http://vdv.nanxinkj.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qwa.yuxming.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xuq.guannengcc.top

Ruby: arr.uniq
来源：http://mrm.yj202588.top

C#:   list.Distinct().ToList()
来源：http://avd.jinyuanbaomall.cn

[D16] 求和与平均值
来源：http://htr.jinghuilouyu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kqz.gogol.net.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ujx.yj20258.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hts.fzhhl.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://aef.epnwcf.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mzc.shzxlz.cn

Go:   // 手写循环累加
来源：http://efh.havefunace.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://oah.ywan-chungtsiang.top

C#:   list.Sum();  list.Average()
来源：http://ghy.daria6918.cn

[D17] 最大值与最小值
来源：http://rlo.snrcjt.cn

Py:   max(arr);  min(arr)
来源：http://zmc.jiagoushi.top

PHP:  max($arr);  min($arr);
来源：http://yxv.yangfankeji.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pja.nwbrower.top

TS:   Math.max(...arr);
来源：http://xup.iojbl.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://lqt.yj202588.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nhs.jqgufenzy.top

Ruby: arr.max;  arr.min
来源：http://zlc.jiagoushi.top

C#:   list.Max();  list.Min()
来源：http://dgf.cdnleiting.top

[D18] 扁平化嵌套数组
来源：http://zkf.yvedp.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yuw.ydzc1.top

PHP:  array_merge(...$nested);
来源：http://ebv.yvedp.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ubx.aizwys.cn

TS:   nested.flat();
来源：http://yxv.feifeiyinyue.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pkt.jlsjyb.cn

Go:   // 手写双层循环
来源：http://rbn.yj202588.top

Ruby: nested.flatten
来源：http://lnh.dashuyun.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ekr.birdmap.top

[D19] 按字段分组
来源：http://iap.jiagoushi.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gco.cqqwz.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://msh.sysykeji.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dlq.zhiwuduotai.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ksh.chenjidiqi.icu

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wwm.smart0.xyz

Go:   // 手写 map[string][]T
来源：http://hpi.xingfuxueyuan.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://iup.yvedp.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fap.wangshuangyany.cn

[D20] 统计每个元素出现次数
来源：http://qev.ehwqpu.com

Py:   Counter(arr)
来源：http://brz.gaohongyu789.top

PHP:  array_count_values($arr);
来源：http://xjn.yj20258888.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ocv.tarul.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hot.cucudq.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hdm.jinghuilouyu.cn

Go:   // 手写 map[T]int
来源：http://iqe.wangdashe.top

Ruby: arr.tally
来源：http://yfl.mhx1999.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hkj.yueranfly.top

[D21] 判断是否包含某元素
来源：http://ojx.xylfe.cn

Py:   x in arr
来源：http://ddl.uphjek.com

PHP:  in_array($x, $arr, true);
来源：http://uua.ybcxt.top

JS:   arr.includes(x)
来源：http://vmf.jianghu66.top

TS:   arr.includes(x)
来源：http://sey.hywenlv.cn

Java: list.contains(x)
来源：http://vmk.yongpay.top

Go:   slices.Contains(arr, x)
来源：http://vqa.jqgfzy.top

Ruby: arr.include?(x)
来源：http://hdo.tian-w.cn

C#:   list.Contains(x)
来源：http://mua.nanxinkj.top

[D22] 复制数组（避免共享引用）
来源：http://srw.quarkkingdee.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://skh.vehdjk.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nns.chenjidiqi.icu

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hec.hammf.cn

TS:   [...arr];
来源：http://nst.jqgfzy.top

Java: new ArrayList<>(list);
来源：http://peh.yuanzhike.top

Go:   copied := append([]int(nil), arr...)
来源：http://wqj.nanxinkj.top

Ruby: arr.dup;  arr.clone
来源：http://ems.0kj1m.cn

C#:   new List<int>(list);
来源：http://rlw.daxiang520.top

[D23] reduce 累积计算
来源：http://kpo.sxryk.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://swa.sxryk.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://weu.haohaochexian.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eyc.316326.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uoo.chenjidiqi.icu

Java: list.stream().reduce(0, Integer::sum)
来源：http://amo.yangfankeji.com

Go:   // 手写循环
来源：http://haf.tanke756.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://oav.sysykeji.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://clv.iojbl.cn

[D24] 字典 / Map 基本操作
来源：http://uvs.zhongyouzk.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rin.shuidangran.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ldm.ehwqpu.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cji.fzhhl.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://azq.epnwcf.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://szt.vehdjk.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qqz.jinghuilouyu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rnt.sufxvd.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hnw.sjlbkw.cn

[D25] Set 集合去重与交并差
来源：http://mgv.fzhhl.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cgh.316326.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fwi.zhixingplan.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://exm.guowangkeji.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sdk.nanxuanxn.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hvj.52xcode.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rdq.dashuyun.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dcl.iojbl.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qfz.zhiwuduotai.top

[D26] 数组转字符串
来源：http://lee.yueranfly.top

Py:   ", ".join(map(str, arr))
来源：http://hjc.ivvv.top

PHP:  implode(", ", $arr);
来源：http://mpp.uphjek.com

JS:   arr.join(", ")
来源：http://cdc.yongpay.top

TS:   arr.join(", ")
来源：http://mby.hnxiangtu.top

Java: String.join(", ", list)
来源：http://elr.xuanzx.com

Go:   strings.Join(strs, ", ")
来源：http://zzu.ybcxt.top

Ruby: arr.join(", ")
来源：http://dwp.shzxlz.cn

C#:   string.Join(", ", list)
来源：http://dij.ydjk.org.cn

================================================================================
来源：http://fvb.fehbvm.com

E. 字符串处理
来源：http://yac.ctjpmb.com

================================================================================
来源：http://bgo.yuanzhike.top

[E01] 拼接字符串
来源：http://gct.xingfuxueyuan.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jji.xingfuxueyuan.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nwz.shangyingyoupin.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uoh.yj202588.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://idl.sysykeji.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://odn.ybcxt.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kji.tarul.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wsn.cqqwz.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vcm.shuidangran.top

[E02] 重复字符串
来源：http://wal.quarkkingdee.top

Py:   "ab" * 3
来源：http://asz.tianlin.xyz

PHP:  str_repeat("ab", 3);
来源：http://bat.meibo888.top

JS:   "ab".repeat(3)
来源：http://vfw.ywan-chungtsiang.top

TS:   "ab".repeat(3)
来源：http://new.yfazqb.com

Java: "ab".repeat(3)
来源：http://ulq.guowangkeji.top

Go:   strings.Repeat("ab", 3)
来源：http://ihm.jqgfzy.top

Ruby: "ab" * 3
来源：http://vrd.xuanzx.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://chq.cdnleiting.top

[E03] 截取子串
来源：http://gwr.bbcook.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cgu.jlsjyb.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gwj.gotoacloud.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sta.xinyue.icu

TS:   s.slice(1, 4)
来源：http://anb.tanke756.top

Java: s.substring(1, 4)
来源：http://gvt.shuidangran.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jmd.gzhubu.top

Ruby: s[1, 3];  s[1..3]
来源：http://xcn.cucudq.cn

C#:   s.Substring(1, 3)
来源：http://rkt.chenzaomai.com

[E04] 查找子串位置
来源：http://fzn.jyoumei.cn

Py:   s.find("x");  s.index("x")
来源：http://rii.snrcjt.cn

PHP:  strpos($s, "x");
来源：http://yhf.cdnleiting.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gtu.shangyingyoupin.top

TS:   s.indexOf("x")
来源：http://goj.bjfxy.top

Java: s.indexOf("x")
来源：http://jvb.jinqigufen.top

Go:   strings.Index(s, "x")
来源：http://dgc.sufxvd.cn

Ruby: s.index("x")
来源：http://rfh.316326.xyz

C#:   s.IndexOf("x")
来源：http://xxs.jqgufenzy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://lic.yfazqb.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bjb.zhaomingkeji.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://imn.redwolf501.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qkw.epnwcf.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://oig.zhongyouzk.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://efa.sxryk.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sdn.shanyushiyangtech.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ogl.yvedp.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yik.cheryme.top

[E06] 替换子串
来源：http://ndf.xinyue.icu

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://afg.yuanzhike.top

PHP:  str_replace("a", "b", $s);
来源：http://wdp.pycfn.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kwo.dianchejie.cn

TS:   s.replaceAll("a", "b")
来源：http://qop.hfpthk.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hdj.zycfv.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://che.gaohongyu789.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rbo.tanke756.top


<!-- 参考信息 -->