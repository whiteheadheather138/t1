代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://jjw.c1oappe.top

Ruby: arr = [1, 2, 3]
来源：http://xre.wangshuangyany.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gtf.hywenlv.cn

[D02] 追加元素到末尾
来源：http://qbh.9152youxi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jpb.c1oappe.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vwv.ctjpmb.com

JS:   arr.push(4);
来源：http://tjs.kuanghao11.cn

TS:   arr.push(4);
来源：http://iih.zhengqikj.top

Java: list.add(4);
来源：http://nlt.kuanghao11.cn

Go:   arr = append(arr, 4)
来源：http://kbk.nanxuanxn.top

Ruby: arr << 4; arr.push(5)
来源：http://vul.jinyuanbaomall.cn

C#:   list.Add(4);
来源：http://kix.nanxinkj.top

[D03] 在指定位置插入元素
来源：http://ncb.dashuyun.cn

Py:   arr.insert(0, 0)
来源：http://mps.shanyushiyangkeji.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xaq.xingfuxueyuan.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ezr.hammf.cn

TS:   arr.splice(0, 0, 0);
来源：http://fps.sxryk.cn

Java: list.add(0, 0);
来源：http://ndf.jinqigufen.top

Go:   arr = append([]int{0}, arr...)
来源：http://xxf.guannengcc.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uci.daria6918.cn

C#:   list.Insert(0, 0);
来源：http://fbf.nanxinkj.top

[D04] 删除元素
来源：http://zkl.yonumen.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wwa.shangyingyoupin.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rev.daxiang520.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://him.wangshuangyany.cn

TS:   arr.splice(0, 1);
来源：http://hoa.zycfv.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://oqk.tanke756.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yuc.yvedp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ixt.cucudq.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hrz.gotoacloud.top

[D05] 访问与修改元素
来源：http://sog.zhoulong.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zeh.xziqi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mqg.uphjek.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zyn.sufxvd.cn

TS:   arr[0]; arr.at(-1);
来源：http://rxp.daxiang520.top

Java: list.get(0); list.set(0, 9);
来源：http://gre.ydzc1.top

Go:   arr[0]; arr[0] = 9
来源：http://cft.nwbrower.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tdp.dashuyun.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cqb.yueranfly.top

[D06] 数组长度
来源：http://hnf.haohaochexian.top

Py:   len(arr)
来源：http://qas.jianghu66.top

PHP:  count($arr);
来源：http://vbi.yonumen.top

JS:   arr.length
来源：http://lic.9152youxi.cn

TS:   arr.length
来源：http://ybe.uphjek.com

Java: list.size();
来源：http://rnu.xuetiantiany.cn

Go:   len(arr)
来源：http://tcy.bbcook.cn

Ruby: arr.length; arr.size
来源：http://zhn.vqdsnc.cn

C#:   list.Count;
来源：http://sec.yfazqb.com

[D07] 切片 / 取子数组
来源：http://rau.cqqwz.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wkh.xuanzx.com

PHP:  array_slice($arr, 1, 3);
来源：http://sio.gogol.net.cn

JS:   arr.slice(1, 4);
来源：http://jtm.ppjwa.cn

TS:   arr.slice(1, 4);
来源：http://fyl.jlsjyb.cn

Java: list.subList(1, 4);
来源：http://did.jyoumei.cn

Go:   arr[1:4]
来源：http://ntw.cashguo.top

Ruby: arr[1, 3]
来源：http://heu.svipenyu.cn

C#:   list.GetRange(1, 3);
来源：http://wjd.andypj.xyz

[D08] 合并两个数组
来源：http://lnk.ctjpmb.com

Py:   a + b;  a.extend(b)
来源：http://qcj.nwbrower.top

PHP:  array_merge($a, $b);
来源：http://swv.jinqigfzy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://sff.chenlongwang.top

TS:   [...a, ...b];
来源：http://eis.bbcook.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://iqy.ydzc1.top

Go:   append(a, b...)
来源：http://bfy.fehbvm.com

Ruby: a + b;  a.concat(b)
来源：http://jxi.zhaomingkeji.xyz

C#:   a.Concat(b).ToList()
来源：http://mxm.316326.xyz

[D09] 排序（升序）
来源：http://ncr.vehdjk.com

Py:   sorted(arr);  arr.sort()
来源：http://svz.zycfv.cn

PHP:  sort($arr);
来源：http://mza.yvedp.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ikx.chenlongwang.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://dgb.cqqwz.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://jci.jinqigufen.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fvk.ctjpmb.com

Ruby: arr.sort
来源：http://ppm.epnwcf.com

C#:   list.Sort();
来源：http://xch.hysaishi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://haz.andypj.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fyg.quarkkingdee.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rjx.iojbl.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wio.aibaodan.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zpl.zhoulong.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://drf.vqdsnc.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tax.9152youxi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://crt.zhoulong.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yhv.svipenyu.cn

[D11] 反转数组
来源：http://yqq.zhengqikj.top

Py:   arr[::-1];  arr.reverse()
来源：http://jnz.yongpay.top

PHP:  array_reverse($arr);
来源：http://lzx.hywenlv.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gxf.xuanzx.com

TS:   [...arr].reverse();
来源：http://vwv.fanxiaobao.xyz

Java: Collections.reverse(list);
来源：http://osu.tarul.cn

Go:   slices.Reverse(arr)
来源：http://cid.svipenyu.cn

Ruby: arr.reverse
来源：http://wkw.ydjk.org.cn

C#:   list.Reverse();
来源：http://yzj.xingfuxueyuan.xyz

[D12] 查找元素下标
来源：http://fxr.jinghuilouyu.cn

Py:   arr.index(x);  x in arr
来源：http://yej.bbcook.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://amx.fzhhl.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rlq.c1oappe.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qxu.yuanzhike.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ytv.dashuyun.cn

Go:   slices.Index(arr, x)
来源：http://lty.cqqwz.cn

Ruby: arr.index(x)
来源：http://hwo.cqqwz.cn

C#:   list.IndexOf(x);
来源：http://cmy.gogol.net.cn

[D13] 过滤（保留满足条件的）
来源：http://svt.jqgufenzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bdu.tianlin.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://txl.jinqigfzy.top

JS:   arr.filter(x => x > 3)
来源：http://tsk.nwbrower.top

TS:   arr.filter(x => x > 3)
来源：http://lnl.ehwqpu.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dpt.yanxiufei.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mur.gotoacloud.top

Ruby: arr.select { |x| x > 3 }
来源：http://siw.ydzc1.top

C#:   list.Where(x => x > 3).ToList()
来源：http://vie.yfazqb.com

[D14] 映射转换（每个元素变形）
来源：http://srl.jyoumei.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fdo.cqqwz.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zwq.52xcode.cn

JS:   arr.map(x => x * 2)
来源：http://cfs.hcnkem.com

TS:   arr.map(x => x * 2)
来源：http://pvr.ydzc1.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://lgd.redwolf501.top

Go:   // 手写循环
来源：http://kar.xinyue.icu

Ruby: arr.map { |x| x * 2 }
来源：http://mjy.nanxinkj.top

C#:   list.Select(x => x * 2).ToList()
来源：http://hjg.ybcxt.top

[D15] 去重
来源：http://mqm.zhiwuduotai.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://taq.quarkkingdee.top

PHP:  array_unique($arr);
来源：http://lzz.vqdsnc.cn

JS:   [...new Set(arr)]
来源：http://zvj.epnwcf.com

TS:   [...new Set(arr)]
来源：http://ema.fzhhl.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bph.xuanzx.com

Go:   // 用 map[T]struct{} 手写
来源：http://cad.vqdsnc.cn

Ruby: arr.uniq
来源：http://tum.pycfn.com

C#:   list.Distinct().ToList()
来源：http://hit.xylfe.cn

[D16] 求和与平均值
来源：http://axx.zdbjq.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://udh.ctjpmb.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fkq.cucudq.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kxf.uphjek.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pwy.mhx1999.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ajm.yfazqb.com

Go:   // 手写循环累加
来源：http://mxl.ctjpmb.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cty.jqgufenzy.top

C#:   list.Sum();  list.Average()
来源：http://jef.hnqzz.top

[D17] 最大值与最小值
来源：http://wwy.dianchejie.cn

Py:   max(arr);  min(arr)
来源：http://kgp.xuanzx.com

PHP:  max($arr);  min($arr);
来源：http://byc.cdnleiting.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://eyd.yonumen.top

TS:   Math.max(...arr);
来源：http://qrb.jinghuilouyu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://zii.sufxvd.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hii.0kj1m.cn

Ruby: arr.max;  arr.min
来源：http://caq.cqqwz.cn

C#:   list.Max();  list.Min()
来源：http://gpn.316326.xyz

[D18] 扁平化嵌套数组
来源：http://emt.ywan-chungtsiang.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ucn.yonumen.top

PHP:  array_merge(...$nested);
来源：http://kui.xylfe.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://erh.jinqigufen.top

TS:   nested.flat();
来源：http://dby.yj20258888.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rzn.yuanzhike.top

Go:   // 手写双层循环
来源：http://ruu.aizwys.cn

Ruby: nested.flatten
来源：http://lxf.zhaomingkeji.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://nrq.xylfe.cn

[D19] 按字段分组
来源：http://sln.nwbrower.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rup.bjfxy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dbw.quarkkingdee.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rtl.wangdashe.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://vuh.zdbjq.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jvi.9152youxi.cn

Go:   // 手写 map[string][]T
来源：http://hpt.jqgfzy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://zim.fzhhl.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://irx.dashuyun.cn

[D20] 统计每个元素出现次数
来源：http://rqi.daria6918.cn

Py:   Counter(arr)
来源：http://kbv.havefunace.top

PHP:  array_count_values($arr);
来源：http://osh.cashguo.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rmh.tanke756.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hic.wangdashe.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dsk.ywan-chungtsiang.top

Go:   // 手写 map[T]int
来源：http://dia.gaohongyu789.top

Ruby: arr.tally
来源：http://wgc.jqgfzy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://auj.tarul.cn

[D21] 判断是否包含某元素
来源：http://rhl.0kj1m.cn

Py:   x in arr
来源：http://zks.pycfn.com

PHP:  in_array($x, $arr, true);
来源：http://kci.andypj.xyz

JS:   arr.includes(x)
来源：http://tuw.aizwys.cn

TS:   arr.includes(x)
来源：http://hig.yonumen.top

Java: list.contains(x)
来源：http://cpw.yfazqb.com

Go:   slices.Contains(arr, x)
来源：http://tum.jinghuilouyu.cn

Ruby: arr.include?(x)
来源：http://txl.hysaishi.cn

C#:   list.Contains(x)
来源：http://our.snrcjt.cn

[D22] 复制数组（避免共享引用）
来源：http://uxa.ywan-chungtsiang.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lcv.xylfe.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yae.wangdashe.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rnl.yonumen.top

TS:   [...arr];
来源：http://kay.zhaomingkeji.xyz

Java: new ArrayList<>(list);
来源：http://ozu.jinyuanbaomall.cn

Go:   copied := append([]int(nil), arr...)
来源：http://mxl.fehbvm.com

Ruby: arr.dup;  arr.clone
来源：http://jqx.quarkkingdee.top

C#:   new List<int>(list);
来源：http://tnv.zhixingplan.top

[D23] reduce 累积计算
来源：http://txx.sufxvd.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fds.aizwys.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gso.hysaishi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cmn.sufxvd.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jix.vqdsnc.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://iqo.pycfn.com

Go:   // 手写循环
来源：http://uoj.yangfankeji.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qxk.meibo888.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qxd.cashguo.top

[D24] 字典 / Map 基本操作
来源：http://wgp.cashguo.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zmw.yueranfly.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gsq.jinqigufen.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mge.zhijiandao.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vty.shangyingyoupin.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://weu.hywenlv.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ras.dianchejie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cke.tian-w.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://aol.daxiang520.top

[D25] Set 集合去重与交并差
来源：http://bdc.zdqjudy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mqh.zycfv.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://unq.yangfankeji.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bye.smart0.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ymw.iojbl.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ltx.haohaochexian.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yiy.dianchejie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nwq.hfpthk.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lin.aibaodan.cn

[D26] 数组转字符串
来源：http://sjo.zhaomingkeji.xyz

Py:   ", ".join(map(str, arr))
来源：http://ieb.sufxvd.cn

PHP:  implode(", ", $arr);
来源：http://zcx.yj20258888.top

JS:   arr.join(", ")
来源：http://gqw.meibo888.top

TS:   arr.join(", ")
来源：http://iwg.yangfankeji.com

Java: String.join(", ", list)
来源：http://dib.bbcook.cn

Go:   strings.Join(strs, ", ")
来源：http://pwa.jinyuanbaomall.cn

Ruby: arr.join(", ")
来源：http://pch.fanxiaobao.xyz

C#:   string.Join(", ", list)
来源：http://umc.zhijiandao.cn

================================================================================
来源：http://ean.ybcxt.top

E. 字符串处理
来源：http://kfz.jqgufenzy.top

================================================================================
来源：http://nqb.aibaodan.cn

[E01] 拼接字符串
来源：http://ojz.fanxiaobao.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ffe.jiagoushi.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://thu.zhongyouzk.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dzz.dianchejie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zvx.ydzc1.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ort.zhijiandao.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ddk.jlsjyb.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wqx.jqgfzy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jyj.havefunace.top

[E02] 重复字符串
来源：http://dkh.0kj1m.cn

Py:   "ab" * 3
来源：http://tku.ydzc1.top

PHP:  str_repeat("ab", 3);
来源：http://itf.ywan-chungtsiang.top

JS:   "ab".repeat(3)
来源：http://vpd.nwbrower.top

TS:   "ab".repeat(3)
来源：http://lbt.zhengqikj.top

Java: "ab".repeat(3)
来源：http://psx.shzxlz.cn

Go:   strings.Repeat("ab", 3)
来源：http://xrb.nanxuanxn.top

Ruby: "ab" * 3
来源：http://rhu.uphjek.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zjj.yonumen.top

[E03] 截取子串
来源：http://lcu.yangfankeji.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nya.bbcook.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jvj.zhoulong.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://twg.zhaomingkeji.xyz

TS:   s.slice(1, 4)
来源：http://rho.cashguo.top

Java: s.substring(1, 4)
来源：http://poc.jlsjyb.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gho.sufxvd.cn

Ruby: s[1, 3];  s[1..3]
来源：http://gjs.52xcode.cn

C#:   s.Substring(1, 3)
来源：http://bvx.chenzaomai.com

[E04] 查找子串位置
来源：http://otj.hesvh.cn

Py:   s.find("x");  s.index("x")
来源：http://gqa.haohaochexian.top

PHP:  strpos($s, "x");
来源：http://qrc.bjfxy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jbx.tian-w.cn

TS:   s.indexOf("x")
来源：http://nll.ehwqpu.com

Java: s.indexOf("x")
来源：http://fbe.jinghuilouyu.cn

Go:   strings.Index(s, "x")
来源：http://qea.yonumen.top

Ruby: s.index("x")
来源：http://fne.shanyushiyangtech.top

C#:   s.IndexOf("x")
来源：http://ixb.tanke756.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ojv.iojbl.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qmz.zhoulong.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kdx.birdmap.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sad.sjlbkw.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://pyo.yongpay.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jda.jinyuanbaomall.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qdj.iojbl.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tzc.pengpengdd.cyou

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wha.wangdashe.top

[E06] 替换子串
来源：http://qxd.feifeiyinyue.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vzw.wangshuangyany.cn

PHP:  str_replace("a", "b", $s);
来源：http://dja.hnxiangtu.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mvz.jyoumei.cn

TS:   s.replaceAll("a", "b")
来源：http://xaa.tarul.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://prp.shuidangran.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://upe.cheryme.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dwa.jqgufenzy.top

C#:   s.Replace("a", "b")
来源：http://ygq.tarul.cn

[E07] 按分隔符拆分
来源：http://jeu.daria6918.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://etr.bjfxy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ukz.shanyushiyangtech.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://zba.fengsongda.top

TS:   s.split(",")
来源：http://bgu.mhx1999.top

Java: s.split(",");  s.split("\\s+")
来源：http://krj.pycfn.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pvt.cashguo.top

Ruby: s.split(",");  s.split
来源：http://acv.cucudq.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jkg.jqgufenzy.top

[E08] 数组按分隔符合并
来源：http://qgj.nanxinkj.top

Py:   ",".join(items)
来源：http://dst.hysaishi.cn

PHP:  implode(",", $items);
来源：http://ytv.yj202588.top

JS:   items.join(",")
来源：http://mqn.xinyue.icu

TS:   items.join(",")
来源：http://eqx.uphjek.com

Java: String.join(",", items)
来源：http://kan.jinyuanbaomall.cn


<!-- 参考信息 -->