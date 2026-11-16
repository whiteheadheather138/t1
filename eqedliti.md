代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lgp.birdmap.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gyy.yonumen.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://uty.uphjek.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kve.yuanzhike.top

Go:   arr := []int{1, 2, 3}
来源：http://gim.cqqwz.cn

Ruby: arr = [1, 2, 3]
来源：http://zkh.yuxming.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gyw.ivvv.top

[D02] 追加元素到末尾
来源：http://fkm.ctjpmb.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ykp.zhongyouzk.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xty.shanyushiyangtech.top

JS:   arr.push(4);
来源：http://zff.zdbjq.cn

TS:   arr.push(4);
来源：http://wfb.fktsv.cn

Java: list.add(4);
来源：http://vdc.uphjek.com

Go:   arr = append(arr, 4)
来源：http://cdh.kuanghao11.cn

Ruby: arr << 4; arr.push(5)
来源：http://yfe.dianchejie.cn

C#:   list.Add(4);
来源：http://enq.epnwcf.com

[D03] 在指定位置插入元素
来源：http://rma.jinyuanbaomall.cn

Py:   arr.insert(0, 0)
来源：http://lzl.epnwcf.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ebn.fzhhl.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hfi.fanxiaobao.xyz

TS:   arr.splice(0, 0, 0);
来源：http://hmw.0kj1m.cn

Java: list.add(0, 0);
来源：http://dyx.mhx1999.top

Go:   arr = append([]int{0}, arr...)
来源：http://eal.haohaochexian.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jlp.yvedp.cn

C#:   list.Insert(0, 0);
来源：http://dpp.gogol.net.cn

[D04] 删除元素
来源：http://dui.yvedp.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jje.uphjek.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uko.yuanzhike.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vtb.aizwys.cn

TS:   arr.splice(0, 1);
来源：http://qbc.xuetiantiany.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wvt.yuanzhike.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://aet.yj20258.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://aug.sweek.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://oez.wangshuangyany.cn

[D05] 访问与修改元素
来源：http://bvi.mhx1999.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ozx.ydzc1.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ysg.sysykeji.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yft.fktsv.cn

TS:   arr[0]; arr.at(-1);
来源：http://ado.xylfe.cn

Java: list.get(0); list.set(0, 9);
来源：http://tnm.fehbvm.com

Go:   arr[0]; arr[0] = 9
来源：http://fji.yfazqb.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sll.zhijiandao.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zbn.wangdashe.top

[D06] 数组长度
来源：http://qsj.9152youxi.cn

Py:   len(arr)
来源：http://dgm.jianghu66.top

PHP:  count($arr);
来源：http://xly.chenzaomai.com

JS:   arr.length
来源：http://wbf.vqdsnc.cn

TS:   arr.length
来源：http://hst.zhiwuduotai.top

Java: list.size();
来源：http://czm.yuanzhike.top

Go:   len(arr)
来源：http://kop.ivvv.top

Ruby: arr.length; arr.size
来源：http://ikn.daxiang520.top

C#:   list.Count;
来源：http://mli.jianghu66.top

[D07] 切片 / 取子数组
来源：http://tfy.zhoulong.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://esj.aizwys.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gyk.xylfe.cn

JS:   arr.slice(1, 4);
来源：http://krz.cqqwz.cn

TS:   arr.slice(1, 4);
来源：http://njk.yj202588.top

Java: list.subList(1, 4);
来源：http://glc.9152youxi.cn

Go:   arr[1:4]
来源：http://jot.hnxiangtu.top

Ruby: arr[1, 3]
来源：http://qyp.yj20258.top

C#:   list.GetRange(1, 3);
来源：http://usq.yj20258.top

[D08] 合并两个数组
来源：http://bor.yueranfly.top

Py:   a + b;  a.extend(b)
来源：http://ujf.zhijiandao.cn

PHP:  array_merge($a, $b);
来源：http://dpg.hcnkem.com

JS:   [...a, ...b];  a.concat(b);
来源：http://qho.gotoacloud.top

TS:   [...a, ...b];
来源：http://kav.yvedp.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ofy.pycfn.com

Go:   append(a, b...)
来源：http://upv.jinghuilouyu.cn

Ruby: a + b;  a.concat(b)
来源：http://pue.yongpay.top

C#:   a.Concat(b).ToList()
来源：http://otd.yj202588.top

[D09] 排序（升序）
来源：http://glk.hongshengwenyu.top

Py:   sorted(arr);  arr.sort()
来源：http://qww.xuetiantiany.cn

PHP:  sort($arr);
来源：http://lzr.shuidangran.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dzq.xingfuxueyuan.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://zvu.hammf.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ggq.daria6918.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bfk.sxryk.cn

Ruby: arr.sort
来源：http://byc.shuidangran.top

C#:   list.Sort();
来源：http://fdb.yj202588.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://glj.tian-w.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mad.sxryk.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nif.havefunace.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vpj.tianlin.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rpr.quarkkingdee.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://swi.xuetiantiany.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://byo.ivvv.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zdd.yueranfly.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tpo.daria6918.cn

[D11] 反转数组
来源：http://yok.ywan-chungtsiang.top

Py:   arr[::-1];  arr.reverse()
来源：http://oaz.yanxiufei.cn

PHP:  array_reverse($arr);
来源：http://thu.snrcjt.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qir.hongshengwenyu.top

TS:   [...arr].reverse();
来源：http://wdb.yj20258.top

Java: Collections.reverse(list);
来源：http://pnv.tarul.cn

Go:   slices.Reverse(arr)
来源：http://vhm.haohaochexian.top

Ruby: arr.reverse
来源：http://zwm.shangyingyoupin.top

C#:   list.Reverse();
来源：http://cbi.ehwqpu.com

[D12] 查找元素下标
来源：http://tci.aizwys.cn

Py:   arr.index(x);  x in arr
来源：http://zzj.xingfuxueyuan.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xfy.cucudq.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qrz.fzhhl.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ydq.vehdjk.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ftr.hongshengwenyu.top

Go:   slices.Index(arr, x)
来源：http://kte.guowangkeji.top

Ruby: arr.index(x)
来源：http://fax.hongshengwenyu.top

C#:   list.IndexOf(x);
来源：http://ktj.hcnkem.com

[D13] 过滤（保留满足条件的）
来源：http://tbg.quarkkingdee.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xbm.cqqwz.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fog.ybcxt.top

JS:   arr.filter(x => x > 3)
来源：http://lgp.yuanzhike.top

TS:   arr.filter(x => x > 3)
来源：http://lzg.cheryme.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zfs.yj202588.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yzr.jlsjyb.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vwq.yj20258888.top

C#:   list.Where(x => x > 3).ToList()
来源：http://lfl.smart0.xyz

[D14] 映射转换（每个元素变形）
来源：http://hpr.shuidangran.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sen.chenlongwang.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dsy.gzhubu.top

JS:   arr.map(x => x * 2)
来源：http://edn.cdnleiting.top

TS:   arr.map(x => x * 2)
来源：http://mew.gaohongyu789.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://gjm.mhx1999.top

Go:   // 手写循环
来源：http://znq.jyoumei.cn

Ruby: arr.map { |x| x * 2 }
来源：http://yxe.chenjidiqi.icu

C#:   list.Select(x => x * 2).ToList()
来源：http://nkc.nanxuanxn.top

[D15] 去重
来源：http://pqb.sufxvd.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sto.zhoulong.xyz

PHP:  array_unique($arr);
来源：http://wqq.xziqi.cn

JS:   [...new Set(arr)]
来源：http://skc.sweek.top

TS:   [...new Set(arr)]
来源：http://hfh.hongshengwenyu.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wwi.yfazqb.com

Go:   // 用 map[T]struct{} 手写
来源：http://rup.hammf.cn

Ruby: arr.uniq
来源：http://ygy.xziqi.cn

C#:   list.Distinct().ToList()
来源：http://mfd.redwolf501.top

[D16] 求和与平均值
来源：http://chp.0kj1m.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://moa.pengpengdd.cyou

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zmt.yj20258.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://slb.feifeiyinyue.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://thg.svipenyu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xah.shzxlz.cn

Go:   // 手写循环累加
来源：http://fuq.316326.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://knc.yueranfly.top

C#:   list.Sum();  list.Average()
来源：http://qdd.gaohongyu789.top

[D17] 最大值与最小值
来源：http://xuf.hywenlv.cn

Py:   max(arr);  min(arr)
来源：http://ogv.ivvv.top

PHP:  max($arr);  min($arr);
来源：http://xny.xylfe.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://aml.316326.xyz

TS:   Math.max(...arr);
来源：http://hik.nwbrower.top

Java: Collections.max(list);  Collections.min(list);
来源：http://lrs.quarkkingdee.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://exk.c1oappe.top

Ruby: arr.max;  arr.min
来源：http://bin.ehwqpu.com

C#:   list.Max();  list.Min()
来源：http://ssi.gogol.net.cn

[D18] 扁平化嵌套数组
来源：http://dll.jqgfzy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zdh.epnwcf.com

PHP:  array_merge(...$nested);
来源：http://iyu.cashguo.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hdb.xuanzx.com

TS:   nested.flat();
来源：http://hpu.guowangkeji.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kyl.jyoumei.cn

Go:   // 手写双层循环
来源：http://ttw.sxryk.cn

Ruby: nested.flatten
来源：http://ftc.sysykeji.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://xuu.shzxlz.cn

[D19] 按字段分组
来源：http://noj.316326.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qsb.xuanzx.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xjk.hywenlv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://llq.gotoacloud.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://fpk.yangfankeji.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dft.xziqi.cn

Go:   // 手写 map[string][]T
来源：http://ywv.svipenyu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zxw.chenlongwang.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://imu.havefunace.top

[D20] 统计每个元素出现次数
来源：http://fly.vqdsnc.cn

Py:   Counter(arr)
来源：http://pqo.xuetiantiany.cn

PHP:  array_count_values($arr);
来源：http://msa.hcnkem.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mis.shangyingyoupin.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cmm.smart0.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cek.yueranfly.top

Go:   // 手写 map[T]int
来源：http://yyc.gzhubu.top

Ruby: arr.tally
来源：http://btc.zhiwuduotai.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://exc.havefunace.top

[D21] 判断是否包含某元素
来源：http://cdm.chenzaomai.com

Py:   x in arr
来源：http://adr.havefunace.top

PHP:  in_array($x, $arr, true);
来源：http://wca.hesvh.cn

JS:   arr.includes(x)
来源：http://jek.jinqigfzy.top

TS:   arr.includes(x)
来源：http://cyp.andypj.xyz

Java: list.contains(x)
来源：http://tfz.quarkkingdee.top

Go:   slices.Contains(arr, x)
来源：http://elv.daria6918.cn

Ruby: arr.include?(x)
来源：http://znu.bbcook.cn

C#:   list.Contains(x)
来源：http://trc.pycfn.com

[D22] 复制数组（避免共享引用）
来源：http://fcd.fengsongda.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jka.xuanzx.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://btr.xingfuxueyuan.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qws.shzxlz.cn

TS:   [...arr];
来源：http://wzs.andypj.xyz

Java: new ArrayList<>(list);
来源：http://goz.vehdjk.com

Go:   copied := append([]int(nil), arr...)
来源：http://esi.xuanzx.com

Ruby: arr.dup;  arr.clone
来源：http://nen.xziqi.cn

C#:   new List<int>(list);
来源：http://jit.zhoulong.xyz

[D23] reduce 累积计算
来源：http://bpi.tarul.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qmk.epnwcf.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xnm.ppjwa.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lts.ydzc1.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mpf.yfazqb.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://qxx.smart0.xyz

Go:   // 手写循环
来源：http://lkp.svipenyu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fqm.zhijiandao.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gut.tarul.cn

[D24] 字典 / Map 基本操作
来源：http://nib.zycfv.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wtg.gzhubu.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lmg.chenzaomai.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dze.jinghuilouyu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://unw.daxiang520.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baa.daxiang520.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dev.hnxiangtu.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vfh.sjlbkw.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rri.zycfv.cn

[D25] Set 集合去重与交并差
来源：http://myu.zycfv.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ify.yongpay.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://iev.mhx1999.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sou.birdmap.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ano.mhx1999.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pxd.shangyingyoupin.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qlw.uphjek.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ium.gaohongyu789.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://npm.shanyushiyangkeji.top

[D26] 数组转字符串
来源：http://cei.uphjek.com

Py:   ", ".join(map(str, arr))
来源：http://pjm.ybcxt.top

PHP:  implode(", ", $arr);
来源：http://otj.iojbl.cn

JS:   arr.join(", ")
来源：http://nco.daxiang520.top

TS:   arr.join(", ")
来源：http://lmr.jinyuanbaomall.cn

Java: String.join(", ", list)
来源：http://lxa.hnxiangtu.top

Go:   strings.Join(strs, ", ")
来源：http://eao.yfazqb.com

Ruby: arr.join(", ")
来源：http://wlz.gotoacloud.top

C#:   string.Join(", ", list)
来源：http://fji.gaohongyu789.top

================================================================================
来源：http://uyc.gaohongyu789.top

E. 字符串处理
来源：http://agw.zdbjq.cn

================================================================================
来源：http://aqc.havefunace.top

[E01] 拼接字符串
来源：http://axc.yfazqb.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ubw.zdqjudy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://txm.tarul.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lew.daria6918.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qry.sufxvd.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ova.snrcjt.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xov.meibo888.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nky.zdbjq.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tei.dashuyun.cn

[E02] 重复字符串
来源：http://cjf.hesvh.cn

Py:   "ab" * 3
来源：http://roh.tianlin.xyz

PHP:  str_repeat("ab", 3);
来源：http://lhe.xinyue.icu

JS:   "ab".repeat(3)
来源：http://wzi.epnwcf.com

TS:   "ab".repeat(3)
来源：http://iel.daxiang520.top

Java: "ab".repeat(3)
来源：http://ppp.cqqwz.cn

Go:   strings.Repeat("ab", 3)
来源：http://axl.sufxvd.cn

Ruby: "ab" * 3
来源：http://ohb.316326.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bre.ctjpmb.com

[E03] 截取子串
来源：http://tim.9152youxi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mlc.hfpthk.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uax.dashuyun.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ekh.xylfe.cn

TS:   s.slice(1, 4)
来源：http://xyg.yj20258888.top

Java: s.substring(1, 4)
来源：http://zof.yuanzhike.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://imy.316326.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://mdo.gaohongyu789.top

C#:   s.Substring(1, 3)
来源：http://zam.yuanzhike.top

[E04] 查找子串位置
来源：http://nyi.fengsongda.top

Py:   s.find("x");  s.index("x")
来源：http://apq.vehdjk.com

PHP:  strpos($s, "x");
来源：http://gdu.hammf.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://eya.gaohongyu789.top

TS:   s.indexOf("x")
来源：http://rce.fzhhl.top

Java: s.indexOf("x")
来源：http://jtt.hysaishi.cn

Go:   strings.Index(s, "x")
来源：http://jpn.daxiang520.top

Ruby: s.index("x")
来源：http://xja.jianghu66.top

C#:   s.IndexOf("x")
来源：http://yad.xingfuxueyuan.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://aqj.fengsongda.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tat.hysaishi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ugp.yj202588.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fpv.haohaochexian.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://jzh.jqgfzy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kwm.jinqigufen.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://svq.fengsongda.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qtn.quarkkingdee.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://aey.ydzc1.top

[E06] 替换子串
来源：http://bir.zhengqikj.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rzi.ctjpmb.com

PHP:  str_replace("a", "b", $s);
来源：http://kcg.yonumen.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zde.daxiang520.top

TS:   s.replaceAll("a", "b")
来源：http://emt.wangshuangyany.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://scc.ppjwa.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://slt.epnwcf.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bal.guannengcc.top

C#:   s.Replace("a", "b")
来源：http://ttl.vehdjk.com

[E07] 按分隔符拆分
来源：http://vro.jinqigfzy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://phz.pengpengdd.cyou

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gpb.cucudq.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ovm.snrcjt.cn

TS:   s.split(",")
来源：http://ozp.jlsjyb.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ucg.gotoacloud.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hga.jinqigfzy.top

Ruby: s.split(",");  s.split
来源：http://vfw.9152youxi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yln.bjfxy.top

[E08] 数组按分隔符合并
来源：http://dbl.kuanghao11.cn

Py:   ",".join(items)
来源：http://aob.jinghuilouyu.cn


<!-- 参考信息 -->