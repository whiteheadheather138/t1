代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bcy.cdnleiting.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cnc.xingfuxueyuan.xyz

JS:   arr.push(4);
来源：http://jru.ywan-chungtsiang.top

TS:   arr.push(4);
来源：http://oxy.andypj.xyz

Java: list.add(4);
来源：http://zmc.cheryme.top

Go:   arr = append(arr, 4)
来源：http://npo.wangshuangyany.cn

Ruby: arr << 4; arr.push(5)
来源：http://duy.hfpthk.cn

C#:   list.Add(4);
来源：http://tga.wangdashe.top

[D03] 在指定位置插入元素
来源：http://orz.dianchejie.cn

Py:   arr.insert(0, 0)
来源：http://uxc.fanxiaobao.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yhz.havefunace.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zmv.cqqwz.cn

TS:   arr.splice(0, 0, 0);
来源：http://lch.jqgfzy.top

Java: list.add(0, 0);
来源：http://ltx.tanke756.top

Go:   arr = append([]int{0}, arr...)
来源：http://fya.shuidangran.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zfd.tarul.cn

C#:   list.Insert(0, 0);
来源：http://etf.zhoulong.xyz

[D04] 删除元素
来源：http://itr.yueranfly.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jfb.yonumen.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jsf.xziqi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gsh.smart0.xyz

TS:   arr.splice(0, 1);
来源：http://xqk.chenlongwang.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hyu.xziqi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://emn.cashguo.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://aax.ppjwa.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://efj.9152youxi.cn

[D05] 访问与修改元素
来源：http://pwi.jianghu66.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://stg.jinghuilouyu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bye.xziqi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mmg.andypj.xyz

TS:   arr[0]; arr.at(-1);
来源：http://wkv.jinyuanbaomall.cn

Java: list.get(0); list.set(0, 9);
来源：http://tuz.feifeiyinyue.top

Go:   arr[0]; arr[0] = 9
来源：http://tte.hammf.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ovf.shzxlz.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rrp.fktsv.cn

[D06] 数组长度
来源：http://uom.aizwys.cn

Py:   len(arr)
来源：http://fhi.hcnkem.com

PHP:  count($arr);
来源：http://imc.fanxiaobao.xyz

JS:   arr.length
来源：http://zdd.yvedp.cn

TS:   arr.length
来源：http://pjj.ydzc1.top

Java: list.size();
来源：http://xaz.epnwcf.com

Go:   len(arr)
来源：http://fwu.yanxiufei.cn

Ruby: arr.length; arr.size
来源：http://cao.dashuyun.cn

C#:   list.Count;
来源：http://qle.dashuyun.cn

[D07] 切片 / 取子数组
来源：http://kcu.cdnleiting.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qxv.yonumen.top

PHP:  array_slice($arr, 1, 3);
来源：http://fes.hnqzz.top

JS:   arr.slice(1, 4);
来源：http://rkw.hammf.cn

TS:   arr.slice(1, 4);
来源：http://glj.birdmap.top

Java: list.subList(1, 4);
来源：http://mll.gzhubu.top

Go:   arr[1:4]
来源：http://sbl.zhoulong.xyz

Ruby: arr[1, 3]
来源：http://lqh.mhx1999.top

C#:   list.GetRange(1, 3);
来源：http://goj.vqdsnc.cn

[D08] 合并两个数组
来源：http://edp.pycfn.com

Py:   a + b;  a.extend(b)
来源：http://kgk.yvedp.cn

PHP:  array_merge($a, $b);
来源：http://yvy.aibaodan.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://bly.gzhubu.top

TS:   [...a, ...b];
来源：http://vbr.zhaomingkeji.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zyg.ehwqpu.com

Go:   append(a, b...)
来源：http://pyd.jiagoushi.top

Ruby: a + b;  a.concat(b)
来源：http://mgy.dashuyun.cn

C#:   a.Concat(b).ToList()
来源：http://tln.sjlbkw.cn

[D09] 排序（升序）
来源：http://nbq.chenzaomai.com

Py:   sorted(arr);  arr.sort()
来源：http://rxk.gotoacloud.top

PHP:  sort($arr);
来源：http://oxy.jiagoushi.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://beb.ehwqpu.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://xho.tarul.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://kyt.jlsjyb.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bey.hnxiangtu.top

Ruby: arr.sort
来源：http://qpv.cdnleiting.top

C#:   list.Sort();
来源：http://kpt.gogol.net.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://alm.cheryme.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://glu.yuanzhike.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yxz.svipenyu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zzh.daxiang520.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://scn.ivvv.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dzs.xylfe.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ryu.316326.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fgp.andypj.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sfy.ywan-chungtsiang.top

[D11] 反转数组
来源：http://nnk.yuxming.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ebj.jqgufenzy.top

PHP:  array_reverse($arr);
来源：http://gcz.zdqjudy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://afb.bbcook.cn

TS:   [...arr].reverse();
来源：http://yzh.zhijiandao.cn

Java: Collections.reverse(list);
来源：http://bnk.zdqjudy.top

Go:   slices.Reverse(arr)
来源：http://psh.hfpthk.cn

Ruby: arr.reverse
来源：http://nun.guowangkeji.top

C#:   list.Reverse();
来源：http://jil.gzhubu.top

[D12] 查找元素下标
来源：http://qbt.feifeiyinyue.top

Py:   arr.index(x);  x in arr
来源：http://ujs.hnxiangtu.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hzq.yj202588.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uui.fanxiaobao.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://isz.jiagoushi.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ubk.cqqwz.cn

Go:   slices.Index(arr, x)
来源：http://doo.zhixingplan.top

Ruby: arr.index(x)
来源：http://afc.tian-w.cn

C#:   list.IndexOf(x);
来源：http://kuo.0kj1m.cn

[D13] 过滤（保留满足条件的）
来源：http://jps.chenlongwang.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cbh.haohaochexian.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zyl.shzxlz.cn

JS:   arr.filter(x => x > 3)
来源：http://wyb.fengsongda.top

TS:   arr.filter(x => x > 3)
来源：http://sct.ywan-chungtsiang.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gvi.ppjwa.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jym.fehbvm.com

Ruby: arr.select { |x| x > 3 }
来源：http://ecc.chenzaomai.com

C#:   list.Where(x => x > 3).ToList()
来源：http://lcs.ydjk.org.cn

[D14] 映射转换（每个元素变形）
来源：http://ved.vehdjk.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fka.zhijiandao.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xgi.hesvh.cn

JS:   arr.map(x => x * 2)
来源：http://ahx.jinghuilouyu.cn

TS:   arr.map(x => x * 2)
来源：http://jvc.meibo888.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://qlr.jlsjyb.cn

Go:   // 手写循环
来源：http://cyu.meibo888.top

Ruby: arr.map { |x| x * 2 }
来源：http://cjr.zhaomingkeji.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://xpu.wangshuangyany.cn

[D15] 去重
来源：http://vqe.dianchejie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://oli.daxiang520.top

PHP:  array_unique($arr);
来源：http://ldo.mhx1999.top

JS:   [...new Set(arr)]
来源：http://lbs.0kj1m.cn

TS:   [...new Set(arr)]
来源：http://vzn.jinyuanbaomall.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ueq.hesvh.cn

Go:   // 用 map[T]struct{} 手写
来源：http://liy.nanxinkj.top

Ruby: arr.uniq
来源：http://pmg.sweek.top

C#:   list.Distinct().ToList()
来源：http://pgs.ivvv.top

[D16] 求和与平均值
来源：http://ywl.gogol.net.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://men.yfazqb.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bhw.daxiang520.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sks.sxryk.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://llh.shanyushiyangtech.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cww.nanxuanxn.top

Go:   // 手写循环累加
来源：http://nrn.yonumen.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pyn.9152youxi.cn

C#:   list.Sum();  list.Average()
来源：http://ufx.c1oappe.top

[D17] 最大值与最小值
来源：http://xzk.9152youxi.cn

Py:   max(arr);  min(arr)
来源：http://yva.yvedp.cn

PHP:  max($arr);  min($arr);
来源：http://qhm.ctjpmb.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ryt.hammf.cn

TS:   Math.max(...arr);
来源：http://zvm.hesvh.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xfa.fanxiaobao.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vxy.bjfxy.top

Ruby: arr.max;  arr.min
来源：http://gcy.shanyushiyangtech.top

C#:   list.Max();  list.Min()
来源：http://diw.zhijiandao.cn

[D18] 扁平化嵌套数组
来源：http://tuh.yvedp.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bmw.zdbjq.cn

PHP:  array_merge(...$nested);
来源：http://rik.yfazqb.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ind.vqdsnc.cn

TS:   nested.flat();
来源：http://nfh.quarkkingdee.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zyp.nanxinkj.top

Go:   // 手写双层循环
来源：http://hfi.snrcjt.cn

Ruby: nested.flatten
来源：http://svo.yj20258.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://rnx.fzhhl.top

[D19] 按字段分组
来源：http://djj.cqqwz.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rdo.cdnleiting.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mym.cdnleiting.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://muh.uphjek.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://anh.ivvv.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fpl.sjlbkw.cn

Go:   // 手写 map[string][]T
来源：http://val.nwbrower.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://aji.hnqzz.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lez.ybcxt.top

[D20] 统计每个元素出现次数
来源：http://ezr.aibaodan.cn

Py:   Counter(arr)
来源：http://hag.haohaochexian.top

PHP:  array_count_values($arr);
来源：http://pix.yj20258.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ohz.xylfe.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dkt.wangdashe.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zmy.zhongyouzk.top

Go:   // 手写 map[T]int
来源：http://zqo.gaohongyu789.top

Ruby: arr.tally
来源：http://bno.cashguo.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://etz.chenzaomai.com

[D21] 判断是否包含某元素
来源：http://oas.ydzc1.top

Py:   x in arr
来源：http://jzp.shangyingyoupin.top

PHP:  in_array($x, $arr, true);
来源：http://wct.jqgfzy.top

JS:   arr.includes(x)
来源：http://qvy.yanxiufei.cn

TS:   arr.includes(x)
来源：http://jaj.guannengcc.top

Java: list.contains(x)
来源：http://dsv.redwolf501.top

Go:   slices.Contains(arr, x)
来源：http://blo.zhixingplan.top

Ruby: arr.include?(x)
来源：http://gxr.ctjpmb.com

C#:   list.Contains(x)
来源：http://cpw.jyoumei.cn

[D22] 复制数组（避免共享引用）
来源：http://cez.sysykeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vns.cheryme.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://icc.cdnleiting.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://aod.hywenlv.cn

TS:   [...arr];
来源：http://yhb.hfpthk.cn

Java: new ArrayList<>(list);
来源：http://euj.fktsv.cn

Go:   copied := append([]int(nil), arr...)
来源：http://wdl.hesvh.cn

Ruby: arr.dup;  arr.clone
来源：http://yam.shanyushiyangkeji.top

C#:   new List<int>(list);
来源：http://lvh.iojbl.cn

[D23] reduce 累积计算
来源：http://amh.yuxming.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pgd.xuetiantiany.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rsj.cdnleiting.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nuh.daria6918.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tfv.zhixingplan.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://dkl.xingfuxueyuan.xyz

Go:   // 手写循环
来源：http://dmm.0kj1m.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fju.epnwcf.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xwp.cashguo.top

[D24] 字典 / Map 基本操作
来源：http://lna.xuetiantiany.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://myp.hnqzz.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ogr.epnwcf.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fmf.fehbvm.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zxc.hongshengwenyu.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://idq.fzhhl.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ynu.zhaomingkeji.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://axz.gogol.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gio.feifeiyinyue.top

[D25] Set 集合去重与交并差
来源：http://zdt.zhiwuduotai.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xgz.uphjek.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qey.redwolf501.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fon.zhongyouzk.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fdq.cashguo.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://frd.pengpengdd.cyou

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hhz.yj20258888.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vkl.yanxiufei.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vea.jianghu66.top

[D26] 数组转字符串
来源：http://iyt.aizwys.cn

Py:   ", ".join(map(str, arr))
来源：http://mlz.vqdsnc.cn

PHP:  implode(", ", $arr);
来源：http://rzd.gogol.net.cn

JS:   arr.join(", ")
来源：http://bna.shanyushiyangtech.top

TS:   arr.join(", ")
来源：http://ozq.ppjwa.cn

Java: String.join(", ", list)
来源：http://hda.shangyingyoupin.top

Go:   strings.Join(strs, ", ")
来源：http://yqe.yj20258888.top

Ruby: arr.join(", ")
来源：http://tmq.yvedp.cn

C#:   string.Join(", ", list)
来源：http://hhb.cdnleiting.top

================================================================================
来源：http://vhr.cucudq.cn

E. 字符串处理
来源：http://yix.jinyuanbaomall.cn

================================================================================
来源：http://cet.ywan-chungtsiang.top

[E01] 拼接字符串
来源：http://uib.316326.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://san.redwolf501.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zte.nwbrower.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jbe.ppjwa.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cbz.cucudq.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wjd.aizwys.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qdy.jlsjyb.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pue.shuidangran.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jsa.kuanghao11.cn

[E02] 重复字符串
来源：http://mtx.zhiwuduotai.top

Py:   "ab" * 3
来源：http://qoq.yueranfly.top

PHP:  str_repeat("ab", 3);
来源：http://zas.dashuyun.cn

JS:   "ab".repeat(3)
来源：http://nls.bjfxy.top

TS:   "ab".repeat(3)
来源：http://qhr.52xcode.cn

Java: "ab".repeat(3)
来源：http://wtz.jqgufenzy.top

Go:   strings.Repeat("ab", 3)
来源：http://lab.nanxuanxn.top

Ruby: "ab" * 3
来源：http://iiv.nanxinkj.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tsp.yfazqb.com

[E03] 截取子串
来源：http://ffm.nanxuanxn.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qoq.xuetiantiany.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bbz.chenjidiqi.icu

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://eah.shuidangran.top

TS:   s.slice(1, 4)
来源：http://alg.aibaodan.cn

Java: s.substring(1, 4)
来源：http://kav.hnqzz.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qek.nanxinkj.top

Ruby: s[1, 3];  s[1..3]
来源：http://dah.kuanghao11.cn

C#:   s.Substring(1, 3)
来源：http://lge.52xcode.cn

[E04] 查找子串位置
来源：http://bab.gogol.net.cn

Py:   s.find("x");  s.index("x")
来源：http://qrm.cashguo.top

PHP:  strpos($s, "x");
来源：http://wly.epnwcf.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://owm.ehwqpu.com

TS:   s.indexOf("x")
来源：http://xkr.vqdsnc.cn

Java: s.indexOf("x")
来源：http://hdz.yangfankeji.com

Go:   strings.Index(s, "x")
来源：http://oux.xziqi.cn

Ruby: s.index("x")
来源：http://jjm.jinqigufen.top

C#:   s.IndexOf("x")
来源：http://ebt.wangdashe.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://paj.jinyuanbaomall.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pdm.jyoumei.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://swy.haohaochexian.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bwv.gaohongyu789.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://urj.tanke756.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kqk.jyoumei.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zuq.xingfuxueyuan.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://akc.yj20258.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wma.jqgfzy.top

[E06] 替换子串
来源：http://thr.cheryme.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tzm.xuanzx.com

PHP:  str_replace("a", "b", $s);
来源：http://tnn.c1oappe.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ezk.xylfe.cn

TS:   s.replaceAll("a", "b")
来源：http://byr.yfazqb.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ifa.sysykeji.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xci.fktsv.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ypt.gzhubu.top

C#:   s.Replace("a", "b")
来源：http://acm.epnwcf.com

[E07] 按分隔符拆分
来源：http://tqx.nwbrower.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xml.jqgfzy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://buf.fehbvm.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://cie.c1oappe.top

TS:   s.split(",")
来源：http://oyk.hfpthk.cn

Java: s.split(",");  s.split("\\s+")
来源：http://icj.dianchejie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tiy.52xcode.cn

Ruby: s.split(",");  s.split
来源：http://mkc.yj20258888.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pwv.bbcook.cn

[E08] 数组按分隔符合并
来源：http://zbj.sysykeji.top

Py:   ",".join(items)
来源：http://oeq.bjfxy.top

PHP:  implode(",", $items);
来源：http://bay.wangshuangyany.cn

JS:   items.join(",")
来源：http://stj.shzxlz.cn

TS:   items.join(",")
来源：http://jed.dashuyun.cn

Java: String.join(",", items)
来源：http://pfk.52xcode.cn

Go:   strings.Join(items, ",")
来源：http://hct.hesvh.cn

Ruby: items.join(",")
来源：http://omg.xingfuxueyuan.xyz

C#:   string.Join(",", items)
来源：http://opr.svipenyu.cn

[E09] 去除所有空白字符
来源：http://iim.dianchejie.cn


<!-- 参考信息 -->